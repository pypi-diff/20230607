# Comparing `tmp/bosdyn_api-3.2.3-py2.py3-none-any.whl.zip` & `tmp/bosdyn_api-3.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,249 +1,273 @@
-Zip file size: 299961 bytes, number of entries: 247
--rw-r--r--  2.0 unx       64 b- defN 23-Mar-24 15:44 bosdyn/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-24 15:44 bosdyn/api/__init__.py
--rw-r--r--  2.0 unx     2009 b- defN 23-Mar-24 15:44 bosdyn/api/alerts_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/alerts_pb2_grpc.py
--rw-r--r--  2.0 unx    29332 b- defN 23-Mar-24 15:44 bosdyn/api/arm_command_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/arm_command_pb2_grpc.py
--rw-r--r--  2.0 unx     5850 b- defN 23-Mar-24 15:44 bosdyn/api/arm_surface_contact_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/arm_surface_contact_pb2_grpc.py
--rw-r--r--  2.0 unx     3050 b- defN 23-Mar-24 15:44 bosdyn/api/arm_surface_contact_service_pb2.py
--rw-r--r--  2.0 unx     2967 b- defN 23-Mar-24 15:44 bosdyn/api/arm_surface_contact_service_pb2_grpc.py
--rw-r--r--  2.0 unx     3056 b- defN 23-Mar-24 15:44 bosdyn/api/auth_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/auth_pb2_grpc.py
--rw-r--r--  2.0 unx     1216 b- defN 23-Mar-24 15:44 bosdyn/api/auth_service_pb2.py
--rw-r--r--  2.0 unx     3110 b- defN 23-Mar-24 15:44 bosdyn/api/auth_service_pb2_grpc.py
--rw-r--r--  2.0 unx    32794 b- defN 23-Mar-24 15:44 bosdyn/api/basic_command_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/basic_command_pb2_grpc.py
--rw-r--r--  2.0 unx    14051 b- defN 23-Mar-24 15:44 bosdyn/api/bddf_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/bddf_pb2_grpc.py
--rw-r--r--  2.0 unx    23347 b- defN 23-Mar-24 15:44 bosdyn/api/data_acquisition_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/data_acquisition_pb2_grpc.py
--rw-r--r--  2.0 unx     1714 b- defN 23-Mar-24 15:44 bosdyn/api/data_acquisition_plugin_service_pb2.py
--rw-r--r--  2.0 unx     8973 b- defN 23-Mar-24 15:44 bosdyn/api/data_acquisition_plugin_service_pb2_grpc.py
--rw-r--r--  2.0 unx     1663 b- defN 23-Mar-24 15:44 bosdyn/api/data_acquisition_service_pb2.py
--rw-r--r--  2.0 unx     8608 b- defN 23-Mar-24 15:44 bosdyn/api/data_acquisition_service_pb2_grpc.py
--rw-r--r--  2.0 unx    15792 b- defN 23-Mar-24 15:44 bosdyn/api/data_acquisition_store_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/data_acquisition_store_pb2_grpc.py
--rw-r--r--  2.0 unx     2249 b- defN 23-Mar-24 15:44 bosdyn/api/data_acquisition_store_service_pb2.py
--rw-r--r--  2.0 unx    19213 b- defN 23-Mar-24 15:44 bosdyn/api/data_acquisition_store_service_pb2_grpc.py
--rw-r--r--  2.0 unx    22413 b- defN 23-Mar-24 15:44 bosdyn/api/data_buffer_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/data_buffer_pb2_grpc.py
--rw-r--r--  2.0 unx     1916 b- defN 23-Mar-24 15:44 bosdyn/api/data_buffer_service_pb2.py
--rw-r--r--  2.0 unx    11709 b- defN 23-Mar-24 15:44 bosdyn/api/data_buffer_service_pb2_grpc.py
--rw-r--r--  2.0 unx     1349 b- defN 23-Mar-24 15:44 bosdyn/api/data_chunk_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/data_chunk_pb2_grpc.py
--rw-r--r--  2.0 unx    18846 b- defN 23-Mar-24 15:44 bosdyn/api/data_index_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/data_index_pb2_grpc.py
--rw-r--r--  2.0 unx     1716 b- defN 23-Mar-24 15:44 bosdyn/api/data_service_pb2.py
--rw-r--r--  2.0 unx     9683 b- defN 23-Mar-24 15:44 bosdyn/api/data_service_pb2_grpc.py
--rw-r--r--  2.0 unx     5585 b- defN 23-Mar-24 15:44 bosdyn/api/directory_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/directory_pb2_grpc.py
--rw-r--r--  2.0 unx     6451 b- defN 23-Mar-24 15:44 bosdyn/api/directory_registration_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/directory_registration_pb2_grpc.py
--rw-r--r--  2.0 unx     1639 b- defN 23-Mar-24 15:44 bosdyn/api/directory_registration_service_pb2.py
--rw-r--r--  2.0 unx     7495 b- defN 23-Mar-24 15:44 bosdyn/api/directory_registration_service_pb2_grpc.py
--rw-r--r--  2.0 unx     1393 b- defN 23-Mar-24 15:44 bosdyn/api/directory_service_pb2.py
--rw-r--r--  2.0 unx     4568 b- defN 23-Mar-24 15:44 bosdyn/api/directory_service_pb2_grpc.py
--rw-r--r--  2.0 unx    15480 b- defN 23-Mar-24 15:44 bosdyn/api/estop_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/estop_pb2_grpc.py
--rw-r--r--  2.0 unx     1853 b- defN 23-Mar-24 15:44 bosdyn/api/estop_service_pb2.py
--rw-r--r--  2.0 unx    12256 b- defN 23-Mar-24 15:44 bosdyn/api/estop_service_pb2_grpc.py
--rw-r--r--  2.0 unx     1408 b- defN 23-Mar-24 15:44 bosdyn/api/fault_service_pb2.py
--rw-r--r--  2.0 unx     4661 b- defN 23-Mar-24 15:44 bosdyn/api/fault_service_pb2_grpc.py
--rw-r--r--  2.0 unx     4458 b- defN 23-Mar-24 15:44 bosdyn/api/full_body_command_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/full_body_command_pb2_grpc.py
--rw-r--r--  2.0 unx    21667 b- defN 23-Mar-24 15:44 bosdyn/api/geometry_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/geometry_pb2_grpc.py
--rw-r--r--  2.0 unx     8424 b- defN 23-Mar-24 15:44 bosdyn/api/gripper_camera_param_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/gripper_camera_param_pb2_grpc.py
--rw-r--r--  2.0 unx     1503 b- defN 23-Mar-24 15:44 bosdyn/api/gripper_camera_param_service_pb2.py
--rw-r--r--  2.0 unx     4677 b- defN 23-Mar-24 15:44 bosdyn/api/gripper_camera_param_service_pb2_grpc.py
--rw-r--r--  2.0 unx     5623 b- defN 23-Mar-24 15:44 bosdyn/api/gripper_command_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/gripper_command_pb2_grpc.py
--rw-r--r--  2.0 unx     3507 b- defN 23-Mar-24 15:44 bosdyn/api/header_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/header_pb2_grpc.py
--rw-r--r--  2.0 unx    11451 b- defN 23-Mar-24 15:44 bosdyn/api/image_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/image_pb2_grpc.py
--rw-r--r--  2.0 unx     1334 b- defN 23-Mar-24 15:44 bosdyn/api/image_service_pb2.py
--rw-r--r--  2.0 unx     5046 b- defN 23-Mar-24 15:44 bosdyn/api/image_service_pb2_grpc.py
--rw-r--r--  2.0 unx     2621 b- defN 23-Mar-24 15:44 bosdyn/api/ir_enable_disable_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/ir_enable_disable_pb2_grpc.py
--rw-r--r--  2.0 unx     1351 b- defN 23-Mar-24 15:44 bosdyn/api/ir_enable_disable_service_pb2.py
--rw-r--r--  2.0 unx     2840 b- defN 23-Mar-24 15:44 bosdyn/api/ir_enable_disable_service_pb2_grpc.py
--rw-r--r--  2.0 unx    12499 b- defN 23-Mar-24 15:44 bosdyn/api/lease_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/lease_pb2_grpc.py
--rw-r--r--  2.0 unx     1609 b- defN 23-Mar-24 15:44 bosdyn/api/lease_service_pb2.py
--rw-r--r--  2.0 unx    10495 b- defN 23-Mar-24 15:44 bosdyn/api/lease_service_pb2_grpc.py
--rw-r--r--  2.0 unx     5939 b- defN 23-Mar-24 15:44 bosdyn/api/license_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/license_pb2_grpc.py
--rw-r--r--  2.0 unx     1371 b- defN 23-Mar-24 15:44 bosdyn/api/license_service_pb2.py
--rw-r--r--  2.0 unx     4677 b- defN 23-Mar-24 15:44 bosdyn/api/license_service_pb2_grpc.py
--rw-r--r--  2.0 unx     8596 b- defN 23-Mar-24 15:44 bosdyn/api/local_grid_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/local_grid_pb2_grpc.py
--rw-r--r--  2.0 unx     1395 b- defN 23-Mar-24 15:44 bosdyn/api/local_grid_service_pb2.py
--rw-r--r--  2.0 unx     5131 b- defN 23-Mar-24 15:44 bosdyn/api/local_grid_service_pb2_grpc.py
--rw-r--r--  2.0 unx     6174 b- defN 23-Mar-24 15:44 bosdyn/api/log_annotation_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/log_annotation_pb2_grpc.py
--rw-r--r--  2.0 unx     1337 b- defN 23-Mar-24 15:44 bosdyn/api/log_annotation_service_pb2.py
--rw-r--r--  2.0 unx     3704 b- defN 23-Mar-24 15:44 bosdyn/api/log_annotation_service_pb2_grpc.py
--rw-r--r--  2.0 unx    20772 b- defN 23-Mar-24 15:44 bosdyn/api/manipulation_api_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/manipulation_api_pb2_grpc.py
--rw-r--r--  2.0 unx     1485 b- defN 23-Mar-24 15:44 bosdyn/api/manipulation_api_service_pb2.py
--rw-r--r--  2.0 unx     6493 b- defN 23-Mar-24 15:44 bosdyn/api/manipulation_api_service_pb2_grpc.py
--rw-r--r--  2.0 unx     4165 b- defN 23-Mar-24 15:44 bosdyn/api/mobility_command_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/mobility_command_pb2_grpc.py
--rw-r--r--  2.0 unx    11849 b- defN 23-Mar-24 15:44 bosdyn/api/network_compute_bridge_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/network_compute_bridge_pb2_grpc.py
--rw-r--r--  2.0 unx     1850 b- defN 23-Mar-24 15:44 bosdyn/api/network_compute_bridge_service_pb2.py
--rw-r--r--  2.0 unx     9782 b- defN 23-Mar-24 15:44 bosdyn/api/network_compute_bridge_service_pb2_grpc.py
--rw-r--r--  2.0 unx     3691 b- defN 23-Mar-24 15:44 bosdyn/api/network_stats_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/network_stats_pb2_grpc.py
--rw-r--r--  2.0 unx     2030 b- defN 23-Mar-24 15:44 bosdyn/api/parameter_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/parameter_pb2_grpc.py
--rw-r--r--  2.0 unx     3914 b- defN 23-Mar-24 15:44 bosdyn/api/payload_estimation_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/payload_estimation_pb2_grpc.py
--rw-r--r--  2.0 unx     7114 b- defN 23-Mar-24 15:44 bosdyn/api/payload_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/payload_pb2_grpc.py
--rw-r--r--  2.0 unx    10889 b- defN 23-Mar-24 15:44 bosdyn/api/payload_registration_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/payload_registration_pb2_grpc.py
--rw-r--r--  2.0 unx     1749 b- defN 23-Mar-24 15:44 bosdyn/api/payload_registration_service_pb2.py
--rw-r--r--  2.0 unx     8567 b- defN 23-Mar-24 15:44 bosdyn/api/payload_registration_service_pb2_grpc.py
--rw-r--r--  2.0 unx     1243 b- defN 23-Mar-24 15:44 bosdyn/api/payload_service_pb2.py
--rw-r--r--  2.0 unx     2716 b- defN 23-Mar-24 15:44 bosdyn/api/payload_service_pb2_grpc.py
--rw-r--r--  2.0 unx     8374 b- defN 23-Mar-24 15:44 bosdyn/api/point_cloud_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/point_cloud_pb2_grpc.py
--rw-r--r--  2.0 unx     1416 b- defN 23-Mar-24 15:44 bosdyn/api/point_cloud_service_pb2.py
--rw-r--r--  2.0 unx     5382 b- defN 23-Mar-24 15:44 bosdyn/api/point_cloud_service_pb2_grpc.py
--rw-r--r--  2.0 unx    11191 b- defN 23-Mar-24 15:44 bosdyn/api/power_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/power_pb2_grpc.py
--rw-r--r--  2.0 unx     1616 b- defN 23-Mar-24 15:44 bosdyn/api/power_service_pb2.py
--rw-r--r--  2.0 unx     8130 b- defN 23-Mar-24 15:44 bosdyn/api/power_service_pb2_grpc.py
--rw-r--r--  2.0 unx     4105 b- defN 23-Mar-24 15:44 bosdyn/api/ray_cast_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/ray_cast_pb2_grpc.py
--rw-r--r--  2.0 unx     1237 b- defN 23-Mar-24 15:44 bosdyn/api/ray_cast_service_pb2.py
--rw-r--r--  2.0 unx     2683 b- defN 23-Mar-24 15:44 bosdyn/api/ray_cast_service_pb2_grpc.py
--rw-r--r--  2.0 unx    10116 b- defN 23-Mar-24 15:44 bosdyn/api/robot_command_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/robot_command_pb2_grpc.py
--rw-r--r--  2.0 unx     1566 b- defN 23-Mar-24 15:44 bosdyn/api/robot_command_service_pb2.py
--rw-r--r--  2.0 unx     6817 b- defN 23-Mar-24 15:44 bosdyn/api/robot_command_service_pb2_grpc.py
--rw-r--r--  2.0 unx     4643 b- defN 23-Mar-24 15:44 bosdyn/api/robot_id_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/robot_id_pb2_grpc.py
--rw-r--r--  2.0 unx     1235 b- defN 23-Mar-24 15:44 bosdyn/api/robot_id_service_pb2.py
--rw-r--r--  2.0 unx     3171 b- defN 23-Mar-24 15:44 bosdyn/api/robot_id_service_pb2_grpc.py
--rw-r--r--  2.0 unx    34808 b- defN 23-Mar-24 15:44 bosdyn/api/robot_state_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/robot_state_pb2_grpc.py
--rw-r--r--  2.0 unx     1662 b- defN 23-Mar-24 15:44 bosdyn/api/robot_state_service_pb2.py
--rw-r--r--  2.0 unx     8496 b- defN 23-Mar-24 15:44 bosdyn/api/robot_state_service_pb2_grpc.py
--rw-r--r--  2.0 unx     6687 b- defN 23-Mar-24 15:44 bosdyn/api/service_fault_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/service_fault_pb2_grpc.py
--rw-r--r--  2.0 unx     3705 b- defN 23-Mar-24 15:44 bosdyn/api/sparse_features_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/sparse_features_pb2_grpc.py
--rw-r--r--  2.0 unx     3710 b- defN 23-Mar-24 15:44 bosdyn/api/stairs_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/stairs_pb2_grpc.py
--rw-r--r--  2.0 unx     3460 b- defN 23-Mar-24 15:44 bosdyn/api/synchronized_command_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/synchronized_command_pb2_grpc.py
--rw-r--r--  2.0 unx     1520 b- defN 23-Mar-24 15:44 bosdyn/api/time_range_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/time_range_pb2_grpc.py
--rw-r--r--  2.0 unx     5177 b- defN 23-Mar-24 15:44 bosdyn/api/time_sync_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/time_sync_pb2_grpc.py
--rw-r--r--  2.0 unx     1263 b- defN 23-Mar-24 15:44 bosdyn/api/time_sync_service_pb2.py
--rw-r--r--  2.0 unx     4473 b- defN 23-Mar-24 15:44 bosdyn/api/time_sync_service_pb2_grpc.py
--rw-r--r--  2.0 unx     9596 b- defN 23-Mar-24 15:44 bosdyn/api/trajectory_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/trajectory_pb2_grpc.py
--rw-r--r--  2.0 unx    18773 b- defN 23-Mar-24 15:44 bosdyn/api/world_object_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/world_object_pb2_grpc.py
--rw-r--r--  2.0 unx     1430 b- defN 23-Mar-24 15:44 bosdyn/api/world_object_service_pb2.py
--rw-r--r--  2.0 unx     4752 b- defN 23-Mar-24 15:44 bosdyn/api/world_object_service_pb2_grpc.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-24 15:44 bosdyn/api/auto_return/__init__.py
--rw-r--r--  2.0 unx     6273 b- defN 23-Mar-24 15:44 bosdyn/api/auto_return/auto_return_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/auto_return/auto_return_pb2_grpc.py
--rw-r--r--  2.0 unx     1607 b- defN 23-Mar-24 15:44 bosdyn/api/auto_return/auto_return_service_pb2.py
--rw-r--r--  2.0 unx     6398 b- defN 23-Mar-24 15:44 bosdyn/api/auto_return/auto_return_service_pb2_grpc.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-24 15:44 bosdyn/api/autowalk/__init__.py
--rw-r--r--  2.0 unx     9934 b- defN 23-Mar-24 15:44 bosdyn/api/autowalk/autowalk_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/autowalk/autowalk_pb2_grpc.py
--rw-r--r--  2.0 unx     1411 b- defN 23-Mar-24 15:44 bosdyn/api/autowalk/autowalk_service_pb2.py
--rw-r--r--  2.0 unx     4716 b- defN 23-Mar-24 15:44 bosdyn/api/autowalk/autowalk_service_pb2_grpc.py
--rw-r--r--  2.0 unx    25377 b- defN 23-Mar-24 15:44 bosdyn/api/autowalk/walks_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/autowalk/walks_pb2_grpc.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-24 15:44 bosdyn/api/docking/__init__.py
--rw-r--r--  2.0 unx    12591 b- defN 23-Mar-24 15:44 bosdyn/api/docking/docking_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/docking/docking_pb2_grpc.py
--rw-r--r--  2.0 unx     1747 b- defN 23-Mar-24 15:44 bosdyn/api/docking/docking_service_pb2.py
--rw-r--r--  2.0 unx     8632 b- defN 23-Mar-24 15:44 bosdyn/api/docking/docking_service_pb2_grpc.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-24 15:44 bosdyn/api/graph_nav/__init__.py
--rw-r--r--  2.0 unx    16817 b- defN 23-Mar-24 15:44 bosdyn/api/graph_nav/area_callback_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/graph_nav/area_callback_pb2_grpc.py
--rw-r--r--  2.0 unx     1954 b- defN 23-Mar-24 15:44 bosdyn/api/graph_nav/area_callback_service_pb2.py
--rw-r--r--  2.0 unx    11049 b- defN 23-Mar-24 15:44 bosdyn/api/graph_nav/area_callback_service_pb2_grpc.py
--rw-r--r--  2.0 unx    49710 b- defN 23-Mar-24 15:44 bosdyn/api/graph_nav/graph_nav_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/graph_nav/graph_nav_pb2_grpc.py
--rw-r--r--  2.0 unx     3186 b- defN 23-Mar-24 15:44 bosdyn/api/graph_nav/graph_nav_service_pb2.py
--rw-r--r--  2.0 unx    27993 b- defN 23-Mar-24 15:44 bosdyn/api/graph_nav/graph_nav_service_pb2_grpc.py
--rw-r--r--  2.0 unx    23190 b- defN 23-Mar-24 15:44 bosdyn/api/graph_nav/map_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/graph_nav/map_pb2_grpc.py
--rw-r--r--  2.0 unx    20037 b- defN 23-Mar-24 15:44 bosdyn/api/graph_nav/map_processing_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/graph_nav/map_processing_pb2_grpc.py
--rw-r--r--  2.0 unx     1566 b- defN 23-Mar-24 15:44 bosdyn/api/graph_nav/map_processing_service_pb2.py
--rw-r--r--  2.0 unx     5125 b- defN 23-Mar-24 15:44 bosdyn/api/graph_nav/map_processing_service_pb2_grpc.py
--rw-r--r--  2.0 unx     2440 b- defN 23-Mar-24 15:44 bosdyn/api/graph_nav/nav_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/graph_nav/nav_pb2_grpc.py
--rw-r--r--  2.0 unx    15825 b- defN 23-Mar-24 15:44 bosdyn/api/graph_nav/recording_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/graph_nav/recording_pb2_grpc.py
--rw-r--r--  2.0 unx     2070 b- defN 23-Mar-24 15:44 bosdyn/api/graph_nav/recording_service_pb2.py
--rw-r--r--  2.0 unx    15653 b- defN 23-Mar-24 15:44 bosdyn/api/graph_nav/recording_service_pb2_grpc.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-24 15:44 bosdyn/api/mission/__init__.py
--rw-r--r--  2.0 unx    23899 b- defN 23-Mar-24 15:44 bosdyn/api/mission/mission_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/mission/mission_pb2_grpc.py
--rw-r--r--  2.0 unx     2466 b- defN 23-Mar-24 15:44 bosdyn/api/mission/mission_service_pb2.py
--rw-r--r--  2.0 unx    19058 b- defN 23-Mar-24 15:44 bosdyn/api/mission/mission_service_pb2_grpc.py
--rw-r--r--  2.0 unx    35343 b- defN 23-Mar-24 15:44 bosdyn/api/mission/nodes_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/mission/nodes_pb2_grpc.py
--rw-r--r--  2.0 unx     8546 b- defN 23-Mar-24 15:44 bosdyn/api/mission/remote_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/mission/remote_pb2_grpc.py
--rw-r--r--  2.0 unx     1677 b- defN 23-Mar-24 15:44 bosdyn/api/mission/remote_service_pb2.py
--rw-r--r--  2.0 unx     8610 b- defN 23-Mar-24 15:44 bosdyn/api/mission/remote_service_pb2_grpc.py
--rw-r--r--  2.0 unx     4891 b- defN 23-Mar-24 15:44 bosdyn/api/mission/util_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/mission/util_pb2_grpc.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-24 15:44 bosdyn/api/spot/__init__.py
--rw-r--r--  2.0 unx    11176 b- defN 23-Mar-24 15:44 bosdyn/api/spot/door_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/spot/door_pb2_grpc.py
--rw-r--r--  2.0 unx     1405 b- defN 23-Mar-24 15:44 bosdyn/api/spot/door_service_pb2.py
--rw-r--r--  2.0 unx     4442 b- defN 23-Mar-24 15:44 bosdyn/api/spot/door_service_pb2_grpc.py
--rw-r--r--  2.0 unx    10278 b- defN 23-Mar-24 15:44 bosdyn/api/spot/robot_command_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/spot/robot_command_pb2_grpc.py
--rw-r--r--  2.0 unx    26549 b- defN 23-Mar-24 15:44 bosdyn/api/spot/spot_check_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/spot/spot_check_pb2_grpc.py
--rw-r--r--  2.0 unx     1793 b- defN 23-Mar-24 15:44 bosdyn/api/spot/spot_check_service_pb2.py
--rw-r--r--  2.0 unx     9156 b- defN 23-Mar-24 15:44 bosdyn/api/spot/spot_check_service_pb2_grpc.py
--rw-r--r--  2.0 unx     4579 b- defN 23-Mar-24 15:44 bosdyn/api/spot_cam/LED_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/spot_cam/LED_pb2_grpc.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-24 15:44 bosdyn/api/spot_cam/__init__.py
--rw-r--r--  2.0 unx    15517 b- defN 23-Mar-24 15:44 bosdyn/api/spot_cam/audio_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/spot_cam/audio_pb2_grpc.py
--rw-r--r--  2.0 unx     3538 b- defN 23-Mar-24 15:44 bosdyn/api/spot_cam/camera_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/spot_cam/camera_pb2_grpc.py
--rw-r--r--  2.0 unx    15452 b- defN 23-Mar-24 15:44 bosdyn/api/spot_cam/compositor_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/spot_cam/compositor_pb2_grpc.py
--rw-r--r--  2.0 unx     8084 b- defN 23-Mar-24 15:44 bosdyn/api/spot_cam/health_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/spot_cam/health_pb2_grpc.py
--rw-r--r--  2.0 unx    18025 b- defN 23-Mar-24 15:44 bosdyn/api/spot_cam/logging_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/spot_cam/logging_pb2_grpc.py
--rw-r--r--  2.0 unx     8137 b- defN 23-Mar-24 15:44 bosdyn/api/spot_cam/network_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/spot_cam/network_pb2_grpc.py
--rw-r--r--  2.0 unx     5834 b- defN 23-Mar-24 15:44 bosdyn/api/spot_cam/power_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/spot_cam/power_pb2_grpc.py
--rw-r--r--  2.0 unx    11901 b- defN 23-Mar-24 15:44 bosdyn/api/spot_cam/ptz_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/spot_cam/ptz_pb2_grpc.py
--rw-r--r--  2.0 unx     9653 b- defN 23-Mar-24 15:44 bosdyn/api/spot_cam/service_pb2.py
--rw-r--r--  2.0 unx    96507 b- defN 23-Mar-24 15:44 bosdyn/api/spot_cam/service_pb2_grpc.py
--rw-r--r--  2.0 unx     7466 b- defN 23-Mar-24 15:44 bosdyn/api/spot_cam/streamquality_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/spot_cam/streamquality_pb2_grpc.py
--rw-r--r--  2.0 unx     2518 b- defN 23-Mar-24 15:44 bosdyn/api/spot_cam/version_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/spot_cam/version_pb2_grpc.py
--rw-r--r--  2.0 unx     1403 b- defN 23-Mar-24 15:44 bosdyn_api-3.2.3.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Mar-24 15:44 bosdyn_api-3.2.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Mar-24 15:44 bosdyn_api-3.2.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    22959 b- defN 23-Mar-24 15:44 bosdyn_api-3.2.3.dist-info/RECORD
-247 files, 1414616 bytes uncompressed, 263175 bytes compressed:  81.4%
+Zip file size: 334244 bytes, number of entries: 271
+-rw-r--r--  2.0 unx       64 b- defN 23-Jun-07 02:50 bosdyn/__init__.py
+-rw-r--r--  2.0 unx       64 b- defN 23-Jun-07 02:50 bosdyn/api/__init__.py
+-rw-r--r--  2.0 unx     2009 b- defN 23-Jun-07 02:50 bosdyn/api/alerts_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/alerts_pb2_grpc.py
+-rw-r--r--  2.0 unx    30436 b- defN 23-Jun-07 02:50 bosdyn/api/arm_command_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/arm_command_pb2_grpc.py
+-rw-r--r--  2.0 unx     5850 b- defN 23-Jun-07 02:50 bosdyn/api/arm_surface_contact_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/arm_surface_contact_pb2_grpc.py
+-rw-r--r--  2.0 unx     3050 b- defN 23-Jun-07 02:50 bosdyn/api/arm_surface_contact_service_pb2.py
+-rw-r--r--  2.0 unx     2967 b- defN 23-Jun-07 02:50 bosdyn/api/arm_surface_contact_service_pb2_grpc.py
+-rw-r--r--  2.0 unx     3056 b- defN 23-Jun-07 02:50 bosdyn/api/auth_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/auth_pb2_grpc.py
+-rw-r--r--  2.0 unx     1216 b- defN 23-Jun-07 02:50 bosdyn/api/auth_service_pb2.py
+-rw-r--r--  2.0 unx     3110 b- defN 23-Jun-07 02:50 bosdyn/api/auth_service_pb2_grpc.py
+-rw-r--r--  2.0 unx    33736 b- defN 23-Jun-07 02:50 bosdyn/api/basic_command_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/basic_command_pb2_grpc.py
+-rw-r--r--  2.0 unx    14051 b- defN 23-Jun-07 02:50 bosdyn/api/bddf_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/bddf_pb2_grpc.py
+-rw-r--r--  2.0 unx    24749 b- defN 23-Jun-07 02:50 bosdyn/api/data_acquisition_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/data_acquisition_pb2_grpc.py
+-rw-r--r--  2.0 unx     1714 b- defN 23-Jun-07 02:50 bosdyn/api/data_acquisition_plugin_service_pb2.py
+-rw-r--r--  2.0 unx     9015 b- defN 23-Jun-07 02:50 bosdyn/api/data_acquisition_plugin_service_pb2_grpc.py
+-rw-r--r--  2.0 unx     1663 b- defN 23-Jun-07 02:50 bosdyn/api/data_acquisition_service_pb2.py
+-rw-r--r--  2.0 unx     8621 b- defN 23-Jun-07 02:50 bosdyn/api/data_acquisition_service_pb2_grpc.py
+-rw-r--r--  2.0 unx    15920 b- defN 23-Jun-07 02:50 bosdyn/api/data_acquisition_store_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/data_acquisition_store_pb2_grpc.py
+-rw-r--r--  2.0 unx     2249 b- defN 23-Jun-07 02:50 bosdyn/api/data_acquisition_store_service_pb2.py
+-rw-r--r--  2.0 unx    19213 b- defN 23-Jun-07 02:50 bosdyn/api/data_acquisition_store_service_pb2_grpc.py
+-rw-r--r--  2.0 unx    22413 b- defN 23-Jun-07 02:50 bosdyn/api/data_buffer_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/data_buffer_pb2_grpc.py
+-rw-r--r--  2.0 unx     1916 b- defN 23-Jun-07 02:50 bosdyn/api/data_buffer_service_pb2.py
+-rw-r--r--  2.0 unx    11709 b- defN 23-Jun-07 02:50 bosdyn/api/data_buffer_service_pb2_grpc.py
+-rw-r--r--  2.0 unx     1349 b- defN 23-Jun-07 02:50 bosdyn/api/data_chunk_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/data_chunk_pb2_grpc.py
+-rw-r--r--  2.0 unx    18846 b- defN 23-Jun-07 02:50 bosdyn/api/data_index_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/data_index_pb2_grpc.py
+-rw-r--r--  2.0 unx     1716 b- defN 23-Jun-07 02:50 bosdyn/api/data_service_pb2.py
+-rw-r--r--  2.0 unx     9683 b- defN 23-Jun-07 02:50 bosdyn/api/data_service_pb2_grpc.py
+-rw-r--r--  2.0 unx     5551 b- defN 23-Jun-07 02:50 bosdyn/api/directory_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/directory_pb2_grpc.py
+-rw-r--r--  2.0 unx     6451 b- defN 23-Jun-07 02:50 bosdyn/api/directory_registration_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/directory_registration_pb2_grpc.py
+-rw-r--r--  2.0 unx     1639 b- defN 23-Jun-07 02:50 bosdyn/api/directory_registration_service_pb2.py
+-rw-r--r--  2.0 unx     7495 b- defN 23-Jun-07 02:50 bosdyn/api/directory_registration_service_pb2_grpc.py
+-rw-r--r--  2.0 unx     1393 b- defN 23-Jun-07 02:50 bosdyn/api/directory_service_pb2.py
+-rw-r--r--  2.0 unx     4568 b- defN 23-Jun-07 02:50 bosdyn/api/directory_service_pb2_grpc.py
+-rw-r--r--  2.0 unx    15480 b- defN 23-Jun-07 02:50 bosdyn/api/estop_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/estop_pb2_grpc.py
+-rw-r--r--  2.0 unx     1853 b- defN 23-Jun-07 02:50 bosdyn/api/estop_service_pb2.py
+-rw-r--r--  2.0 unx    12256 b- defN 23-Jun-07 02:50 bosdyn/api/estop_service_pb2_grpc.py
+-rw-r--r--  2.0 unx     1408 b- defN 23-Jun-07 02:50 bosdyn/api/fault_service_pb2.py
+-rw-r--r--  2.0 unx     4661 b- defN 23-Jun-07 02:50 bosdyn/api/fault_service_pb2_grpc.py
+-rw-r--r--  2.0 unx     4458 b- defN 23-Jun-07 02:50 bosdyn/api/full_body_command_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/full_body_command_pb2_grpc.py
+-rw-r--r--  2.0 unx    21667 b- defN 23-Jun-07 02:50 bosdyn/api/geometry_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/geometry_pb2_grpc.py
+-rw-r--r--  2.0 unx    10402 b- defN 23-Jun-07 02:50 bosdyn/api/gripper_camera_param_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/gripper_camera_param_pb2_grpc.py
+-rw-r--r--  2.0 unx     1503 b- defN 23-Jun-07 02:50 bosdyn/api/gripper_camera_param_service_pb2.py
+-rw-r--r--  2.0 unx     4677 b- defN 23-Jun-07 02:50 bosdyn/api/gripper_camera_param_service_pb2_grpc.py
+-rw-r--r--  2.0 unx     5623 b- defN 23-Jun-07 02:50 bosdyn/api/gripper_command_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/gripper_command_pb2_grpc.py
+-rw-r--r--  2.0 unx     3507 b- defN 23-Jun-07 02:50 bosdyn/api/header_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/header_pb2_grpc.py
+-rw-r--r--  2.0 unx     2000 b- defN 23-Jun-07 02:50 bosdyn/api/image_geometry_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/image_geometry_pb2_grpc.py
+-rw-r--r--  2.0 unx    12659 b- defN 23-Jun-07 02:50 bosdyn/api/image_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/image_pb2_grpc.py
+-rw-r--r--  2.0 unx     1334 b- defN 23-Jun-07 02:50 bosdyn/api/image_service_pb2.py
+-rw-r--r--  2.0 unx     5046 b- defN 23-Jun-07 02:50 bosdyn/api/image_service_pb2_grpc.py
+-rw-r--r--  2.0 unx     2621 b- defN 23-Jun-07 02:50 bosdyn/api/ir_enable_disable_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/ir_enable_disable_pb2_grpc.py
+-rw-r--r--  2.0 unx     1351 b- defN 23-Jun-07 02:50 bosdyn/api/ir_enable_disable_service_pb2.py
+-rw-r--r--  2.0 unx     2840 b- defN 23-Jun-07 02:50 bosdyn/api/ir_enable_disable_service_pb2_grpc.py
+-rw-r--r--  2.0 unx    12697 b- defN 23-Jun-07 02:50 bosdyn/api/lease_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/lease_pb2_grpc.py
+-rw-r--r--  2.0 unx     1609 b- defN 23-Jun-07 02:50 bosdyn/api/lease_service_pb2.py
+-rw-r--r--  2.0 unx    10495 b- defN 23-Jun-07 02:50 bosdyn/api/lease_service_pb2_grpc.py
+-rw-r--r--  2.0 unx     5939 b- defN 23-Jun-07 02:50 bosdyn/api/license_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/license_pb2_grpc.py
+-rw-r--r--  2.0 unx     1371 b- defN 23-Jun-07 02:50 bosdyn/api/license_service_pb2.py
+-rw-r--r--  2.0 unx     4677 b- defN 23-Jun-07 02:50 bosdyn/api/license_service_pb2_grpc.py
+-rw-r--r--  2.0 unx     8596 b- defN 23-Jun-07 02:50 bosdyn/api/local_grid_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/local_grid_pb2_grpc.py
+-rw-r--r--  2.0 unx     1395 b- defN 23-Jun-07 02:50 bosdyn/api/local_grid_service_pb2.py
+-rw-r--r--  2.0 unx     5131 b- defN 23-Jun-07 02:50 bosdyn/api/local_grid_service_pb2_grpc.py
+-rw-r--r--  2.0 unx     6866 b- defN 23-Jun-07 02:50 bosdyn/api/log_annotation_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/log_annotation_pb2_grpc.py
+-rw-r--r--  2.0 unx     1337 b- defN 23-Jun-07 02:50 bosdyn/api/log_annotation_service_pb2.py
+-rw-r--r--  2.0 unx     3497 b- defN 23-Jun-07 02:50 bosdyn/api/log_annotation_service_pb2_grpc.py
+-rw-r--r--  2.0 unx    20772 b- defN 23-Jun-07 02:50 bosdyn/api/manipulation_api_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/manipulation_api_pb2_grpc.py
+-rw-r--r--  2.0 unx     1485 b- defN 23-Jun-07 02:50 bosdyn/api/manipulation_api_service_pb2.py
+-rw-r--r--  2.0 unx     6493 b- defN 23-Jun-07 02:50 bosdyn/api/manipulation_api_service_pb2_grpc.py
+-rw-r--r--  2.0 unx     4165 b- defN 23-Jun-07 02:50 bosdyn/api/mobility_command_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/mobility_command_pb2_grpc.py
+-rw-r--r--  2.0 unx    22449 b- defN 23-Jun-07 02:50 bosdyn/api/network_compute_bridge_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/network_compute_bridge_pb2_grpc.py
+-rw-r--r--  2.0 unx     2148 b- defN 23-Jun-07 02:50 bosdyn/api/network_compute_bridge_service_pb2.py
+-rw-r--r--  2.0 unx    11592 b- defN 23-Jun-07 02:50 bosdyn/api/network_compute_bridge_service_pb2_grpc.py
+-rw-r--r--  2.0 unx     3691 b- defN 23-Jun-07 02:50 bosdyn/api/network_stats_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/network_stats_pb2_grpc.py
+-rw-r--r--  2.0 unx     2030 b- defN 23-Jun-07 02:50 bosdyn/api/parameter_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/parameter_pb2_grpc.py
+-rw-r--r--  2.0 unx     3914 b- defN 23-Jun-07 02:50 bosdyn/api/payload_estimation_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/payload_estimation_pb2_grpc.py
+-rw-r--r--  2.0 unx     7249 b- defN 23-Jun-07 02:50 bosdyn/api/payload_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/payload_pb2_grpc.py
+-rw-r--r--  2.0 unx    10889 b- defN 23-Jun-07 02:50 bosdyn/api/payload_registration_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/payload_registration_pb2_grpc.py
+-rw-r--r--  2.0 unx     1749 b- defN 23-Jun-07 02:50 bosdyn/api/payload_registration_service_pb2.py
+-rw-r--r--  2.0 unx     8567 b- defN 23-Jun-07 02:50 bosdyn/api/payload_registration_service_pb2_grpc.py
+-rw-r--r--  2.0 unx     1243 b- defN 23-Jun-07 02:50 bosdyn/api/payload_service_pb2.py
+-rw-r--r--  2.0 unx     2716 b- defN 23-Jun-07 02:50 bosdyn/api/payload_service_pb2_grpc.py
+-rw-r--r--  2.0 unx     8374 b- defN 23-Jun-07 02:50 bosdyn/api/point_cloud_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/point_cloud_pb2_grpc.py
+-rw-r--r--  2.0 unx     1416 b- defN 23-Jun-07 02:50 bosdyn/api/point_cloud_service_pb2.py
+-rw-r--r--  2.0 unx     5382 b- defN 23-Jun-07 02:50 bosdyn/api/point_cloud_service_pb2_grpc.py
+-rw-r--r--  2.0 unx    11273 b- defN 23-Jun-07 02:50 bosdyn/api/power_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/power_pb2_grpc.py
+-rw-r--r--  2.0 unx     1616 b- defN 23-Jun-07 02:50 bosdyn/api/power_service_pb2.py
+-rw-r--r--  2.0 unx     8130 b- defN 23-Jun-07 02:50 bosdyn/api/power_service_pb2_grpc.py
+-rw-r--r--  2.0 unx     4105 b- defN 23-Jun-07 02:50 bosdyn/api/ray_cast_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/ray_cast_pb2_grpc.py
+-rw-r--r--  2.0 unx     1237 b- defN 23-Jun-07 02:50 bosdyn/api/ray_cast_service_pb2.py
+-rw-r--r--  2.0 unx     2683 b- defN 23-Jun-07 02:50 bosdyn/api/ray_cast_service_pb2_grpc.py
+-rw-r--r--  2.0 unx    10551 b- defN 23-Jun-07 02:50 bosdyn/api/robot_command_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/robot_command_pb2_grpc.py
+-rw-r--r--  2.0 unx     1566 b- defN 23-Jun-07 02:50 bosdyn/api/robot_command_service_pb2.py
+-rw-r--r--  2.0 unx     6817 b- defN 23-Jun-07 02:50 bosdyn/api/robot_command_service_pb2_grpc.py
+-rw-r--r--  2.0 unx     4643 b- defN 23-Jun-07 02:50 bosdyn/api/robot_id_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/robot_id_pb2_grpc.py
+-rw-r--r--  2.0 unx     1235 b- defN 23-Jun-07 02:50 bosdyn/api/robot_id_service_pb2.py
+-rw-r--r--  2.0 unx     3171 b- defN 23-Jun-07 02:50 bosdyn/api/robot_id_service_pb2_grpc.py
+-rw-r--r--  2.0 unx    34922 b- defN 23-Jun-07 02:50 bosdyn/api/robot_state_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/robot_state_pb2_grpc.py
+-rw-r--r--  2.0 unx     1662 b- defN 23-Jun-07 02:50 bosdyn/api/robot_state_service_pb2.py
+-rw-r--r--  2.0 unx     8496 b- defN 23-Jun-07 02:50 bosdyn/api/robot_state_service_pb2_grpc.py
+-rw-r--r--  2.0 unx    20717 b- defN 23-Jun-07 02:50 bosdyn/api/service_customization_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/service_customization_pb2_grpc.py
+-rw-r--r--  2.0 unx     6687 b- defN 23-Jun-07 02:50 bosdyn/api/service_fault_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/service_fault_pb2_grpc.py
+-rw-r--r--  2.0 unx     3705 b- defN 23-Jun-07 02:50 bosdyn/api/sparse_features_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/sparse_features_pb2_grpc.py
+-rw-r--r--  2.0 unx     8175 b- defN 23-Jun-07 02:50 bosdyn/api/stairs_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/stairs_pb2_grpc.py
+-rw-r--r--  2.0 unx     3460 b- defN 23-Jun-07 02:50 bosdyn/api/synchronized_command_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/synchronized_command_pb2_grpc.py
+-rw-r--r--  2.0 unx     1520 b- defN 23-Jun-07 02:50 bosdyn/api/time_range_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/time_range_pb2_grpc.py
+-rw-r--r--  2.0 unx     5177 b- defN 23-Jun-07 02:50 bosdyn/api/time_sync_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/time_sync_pb2_grpc.py
+-rw-r--r--  2.0 unx     1263 b- defN 23-Jun-07 02:50 bosdyn/api/time_sync_service_pb2.py
+-rw-r--r--  2.0 unx     4473 b- defN 23-Jun-07 02:50 bosdyn/api/time_sync_service_pb2_grpc.py
+-rw-r--r--  2.0 unx     9596 b- defN 23-Jun-07 02:50 bosdyn/api/trajectory_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/trajectory_pb2_grpc.py
+-rw-r--r--  2.0 unx     2467 b- defN 23-Jun-07 02:50 bosdyn/api/units_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/units_pb2_grpc.py
+-rw-r--r--  2.0 unx    20832 b- defN 23-Jun-07 02:50 bosdyn/api/world_object_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/world_object_pb2_grpc.py
+-rw-r--r--  2.0 unx     1430 b- defN 23-Jun-07 02:50 bosdyn/api/world_object_service_pb2.py
+-rw-r--r--  2.0 unx     4764 b- defN 23-Jun-07 02:50 bosdyn/api/world_object_service_pb2_grpc.py
+-rw-r--r--  2.0 unx       64 b- defN 23-Jun-07 02:50 bosdyn/api/auto_return/__init__.py
+-rw-r--r--  2.0 unx     6870 b- defN 23-Jun-07 02:50 bosdyn/api/auto_return/auto_return_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/auto_return/auto_return_pb2_grpc.py
+-rw-r--r--  2.0 unx     1607 b- defN 23-Jun-07 02:50 bosdyn/api/auto_return/auto_return_service_pb2.py
+-rw-r--r--  2.0 unx     6398 b- defN 23-Jun-07 02:50 bosdyn/api/auto_return/auto_return_service_pb2_grpc.py
+-rw-r--r--  2.0 unx       64 b- defN 23-Jun-07 02:50 bosdyn/api/autowalk/__init__.py
+-rw-r--r--  2.0 unx     9934 b- defN 23-Jun-07 02:50 bosdyn/api/autowalk/autowalk_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/autowalk/autowalk_pb2_grpc.py
+-rw-r--r--  2.0 unx     1411 b- defN 23-Jun-07 02:50 bosdyn/api/autowalk/autowalk_service_pb2.py
+-rw-r--r--  2.0 unx     4716 b- defN 23-Jun-07 02:50 bosdyn/api/autowalk/autowalk_service_pb2_grpc.py
+-rw-r--r--  2.0 unx    28007 b- defN 23-Jun-07 02:50 bosdyn/api/autowalk/walks_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/autowalk/walks_pb2_grpc.py
+-rw-r--r--  2.0 unx       64 b- defN 23-Jun-07 02:50 bosdyn/api/docking/__init__.py
+-rw-r--r--  2.0 unx    12713 b- defN 23-Jun-07 02:50 bosdyn/api/docking/docking_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/docking/docking_pb2_grpc.py
+-rw-r--r--  2.0 unx     1747 b- defN 23-Jun-07 02:50 bosdyn/api/docking/docking_service_pb2.py
+-rw-r--r--  2.0 unx     8632 b- defN 23-Jun-07 02:50 bosdyn/api/docking/docking_service_pb2_grpc.py
+-rw-r--r--  2.0 unx       64 b- defN 23-Jun-07 02:50 bosdyn/api/graph_nav/__init__.py
+-rw-r--r--  2.0 unx     1812 b- defN 23-Jun-07 02:50 bosdyn/api/graph_nav/area_callback_data_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/graph_nav/area_callback_data_pb2_grpc.py
+-rw-r--r--  2.0 unx    18870 b- defN 23-Jun-07 02:50 bosdyn/api/graph_nav/area_callback_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/graph_nav/area_callback_pb2_grpc.py
+-rw-r--r--  2.0 unx     1954 b- defN 23-Jun-07 02:50 bosdyn/api/graph_nav/area_callback_service_pb2.py
+-rw-r--r--  2.0 unx    11049 b- defN 23-Jun-07 02:50 bosdyn/api/graph_nav/area_callback_service_pb2_grpc.py
+-rw-r--r--  2.0 unx    54376 b- defN 23-Jun-07 02:50 bosdyn/api/graph_nav/graph_nav_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/graph_nav/graph_nav_pb2_grpc.py
+-rw-r--r--  2.0 unx     3186 b- defN 23-Jun-07 02:50 bosdyn/api/graph_nav/graph_nav_service_pb2.py
+-rw-r--r--  2.0 unx    27993 b- defN 23-Jun-07 02:50 bosdyn/api/graph_nav/graph_nav_service_pb2_grpc.py
+-rw-r--r--  2.0 unx    25984 b- defN 23-Jun-07 02:50 bosdyn/api/graph_nav/map_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/graph_nav/map_pb2_grpc.py
+-rw-r--r--  2.0 unx    20274 b- defN 23-Jun-07 02:50 bosdyn/api/graph_nav/map_processing_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/graph_nav/map_processing_pb2_grpc.py
+-rw-r--r--  2.0 unx     1566 b- defN 23-Jun-07 02:50 bosdyn/api/graph_nav/map_processing_service_pb2.py
+-rw-r--r--  2.0 unx     5125 b- defN 23-Jun-07 02:50 bosdyn/api/graph_nav/map_processing_service_pb2_grpc.py
+-rw-r--r--  2.0 unx     2440 b- defN 23-Jun-07 02:50 bosdyn/api/graph_nav/nav_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/graph_nav/nav_pb2_grpc.py
+-rw-r--r--  2.0 unx    16665 b- defN 23-Jun-07 02:50 bosdyn/api/graph_nav/recording_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/graph_nav/recording_pb2_grpc.py
+-rw-r--r--  2.0 unx     2070 b- defN 23-Jun-07 02:50 bosdyn/api/graph_nav/recording_service_pb2.py
+-rw-r--r--  2.0 unx    15653 b- defN 23-Jun-07 02:50 bosdyn/api/graph_nav/recording_service_pb2_grpc.py
+-rw-r--r--  2.0 unx       64 b- defN 23-Jun-07 02:50 bosdyn/api/keepalive/__init__.py
+-rw-r--r--  2.0 unx    12506 b- defN 23-Jun-07 02:50 bosdyn/api/keepalive/keepalive_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/keepalive/keepalive_pb2_grpc.py
+-rw-r--r--  2.0 unx     1574 b- defN 23-Jun-07 02:50 bosdyn/api/keepalive/keepalive_service_pb2.py
+-rw-r--r--  2.0 unx     7484 b- defN 23-Jun-07 02:50 bosdyn/api/keepalive/keepalive_service_pb2_grpc.py
+-rw-r--r--  2.0 unx       64 b- defN 23-Jun-07 02:50 bosdyn/api/log_status/__init__.py
+-rw-r--r--  2.0 unx    13805 b- defN 23-Jun-07 02:50 bosdyn/api/log_status/log_status_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/log_status/log_status_pb2_grpc.py
+-rw-r--r--  2.0 unx     1934 b- defN 23-Jun-07 02:50 bosdyn/api/log_status/log_status_service_pb2.py
+-rw-r--r--  2.0 unx    13599 b- defN 23-Jun-07 02:50 bosdyn/api/log_status/log_status_service_pb2_grpc.py
+-rw-r--r--  2.0 unx       64 b- defN 23-Jun-07 02:50 bosdyn/api/mission/__init__.py
+-rw-r--r--  2.0 unx    24846 b- defN 23-Jun-07 02:50 bosdyn/api/mission/mission_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/mission/mission_pb2_grpc.py
+-rw-r--r--  2.0 unx     2795 b- defN 23-Jun-07 02:50 bosdyn/api/mission/mission_service_pb2.py
+-rw-r--r--  2.0 unx    25418 b- defN 23-Jun-07 02:50 bosdyn/api/mission/mission_service_pb2_grpc.py
+-rw-r--r--  2.0 unx    39359 b- defN 23-Jun-07 02:50 bosdyn/api/mission/nodes_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/mission/nodes_pb2_grpc.py
+-rw-r--r--  2.0 unx    10873 b- defN 23-Jun-07 02:50 bosdyn/api/mission/remote_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/mission/remote_pb2_grpc.py
+-rw-r--r--  2.0 unx     1853 b- defN 23-Jun-07 02:50 bosdyn/api/mission/remote_service_pb2.py
+-rw-r--r--  2.0 unx    10655 b- defN 23-Jun-07 02:50 bosdyn/api/mission/remote_service_pb2_grpc.py
+-rw-r--r--  2.0 unx     4972 b- defN 23-Jun-07 02:50 bosdyn/api/mission/util_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/mission/util_pb2_grpc.py
+-rw-r--r--  2.0 unx       64 b- defN 23-Jun-07 02:50 bosdyn/api/spot/__init__.py
+-rw-r--r--  2.0 unx     1752 b- defN 23-Jun-07 02:50 bosdyn/api/spot/door_area_callback_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/spot/door_area_callback_pb2_grpc.py
+-rw-r--r--  2.0 unx    11446 b- defN 23-Jun-07 02:50 bosdyn/api/spot/door_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/spot/door_pb2_grpc.py
+-rw-r--r--  2.0 unx     1405 b- defN 23-Jun-07 02:50 bosdyn/api/spot/door_service_pb2.py
+-rw-r--r--  2.0 unx     4442 b- defN 23-Jun-07 02:50 bosdyn/api/spot/door_service_pb2_grpc.py
+-rw-r--r--  2.0 unx     9597 b- defN 23-Jun-07 02:50 bosdyn/api/spot/inverse_kinematics_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/spot/inverse_kinematics_pb2_grpc.py
+-rw-r--r--  2.0 unx     1429 b- defN 23-Jun-07 02:50 bosdyn/api/spot/inverse_kinematics_service_pb2.py
+-rw-r--r--  2.0 unx     2964 b- defN 23-Jun-07 02:50 bosdyn/api/spot/inverse_kinematics_service_pb2_grpc.py
+-rw-r--r--  2.0 unx    11055 b- defN 23-Jun-07 02:50 bosdyn/api/spot/robot_command_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/spot/robot_command_pb2_grpc.py
+-rw-r--r--  2.0 unx    26549 b- defN 23-Jun-07 02:50 bosdyn/api/spot/spot_check_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/spot/spot_check_pb2_grpc.py
+-rw-r--r--  2.0 unx     1793 b- defN 23-Jun-07 02:50 bosdyn/api/spot/spot_check_service_pb2.py
+-rw-r--r--  2.0 unx     9156 b- defN 23-Jun-07 02:50 bosdyn/api/spot/spot_check_service_pb2_grpc.py
+-rw-r--r--  2.0 unx     4579 b- defN 23-Jun-07 02:50 bosdyn/api/spot_cam/LED_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/spot_cam/LED_pb2_grpc.py
+-rw-r--r--  2.0 unx       64 b- defN 23-Jun-07 02:50 bosdyn/api/spot_cam/__init__.py
+-rw-r--r--  2.0 unx    15517 b- defN 23-Jun-07 02:50 bosdyn/api/spot_cam/audio_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/spot_cam/audio_pb2_grpc.py
+-rw-r--r--  2.0 unx     3538 b- defN 23-Jun-07 02:50 bosdyn/api/spot_cam/camera_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/spot_cam/camera_pb2_grpc.py
+-rw-r--r--  2.0 unx    18911 b- defN 23-Jun-07 02:50 bosdyn/api/spot_cam/compositor_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/spot_cam/compositor_pb2_grpc.py
+-rw-r--r--  2.0 unx     8084 b- defN 23-Jun-07 02:50 bosdyn/api/spot_cam/health_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/spot_cam/health_pb2_grpc.py
+-rw-r--r--  2.0 unx    18025 b- defN 23-Jun-07 02:50 bosdyn/api/spot_cam/logging_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/spot_cam/logging_pb2_grpc.py
+-rw-r--r--  2.0 unx    10120 b- defN 23-Jun-07 02:50 bosdyn/api/spot_cam/network_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/spot_cam/network_pb2_grpc.py
+-rw-r--r--  2.0 unx     5834 b- defN 23-Jun-07 02:50 bosdyn/api/spot_cam/power_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/spot_cam/power_pb2_grpc.py
+-rw-r--r--  2.0 unx    15674 b- defN 23-Jun-07 02:50 bosdyn/api/spot_cam/ptz_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/spot_cam/ptz_pb2_grpc.py
+-rw-r--r--  2.0 unx    10034 b- defN 23-Jun-07 02:50 bosdyn/api/spot_cam/service_pb2.py
+-rw-r--r--  2.0 unx   102016 b- defN 23-Jun-07 02:50 bosdyn/api/spot_cam/service_pb2_grpc.py
+-rw-r--r--  2.0 unx     9899 b- defN 23-Jun-07 02:50 bosdyn/api/spot_cam/streamquality_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/spot_cam/streamquality_pb2_grpc.py
+-rw-r--r--  2.0 unx     2518 b- defN 23-Jun-07 02:50 bosdyn/api/spot_cam/version_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/spot_cam/version_pb2_grpc.py
+-rw-r--r--  2.0 unx     1568 b- defN 23-Jun-07 02:50 bosdyn_api-3.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 02:50 bosdyn_api-3.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-07 02:50 bosdyn_api-3.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    25331 b- defN 23-Jun-07 02:50 bosdyn_api-3.3.0.dist-info/RECORD
+271 files, 1588968 bytes uncompressed, 293638 bytes compressed:  81.5%
```

## zipnote {}

```diff
@@ -186,14 +186,20 @@
 
 Filename: bosdyn/api/header_pb2.py
 Comment: 
 
 Filename: bosdyn/api/header_pb2_grpc.py
 Comment: 
 
+Filename: bosdyn/api/image_geometry_pb2.py
+Comment: 
+
+Filename: bosdyn/api/image_geometry_pb2_grpc.py
+Comment: 
+
 Filename: bosdyn/api/image_pb2.py
 Comment: 
 
 Filename: bosdyn/api/image_pb2_grpc.py
 Comment: 
 
 Filename: bosdyn/api/image_service_pb2.py
@@ -402,14 +408,20 @@
 
 Filename: bosdyn/api/robot_state_service_pb2.py
 Comment: 
 
 Filename: bosdyn/api/robot_state_service_pb2_grpc.py
 Comment: 
 
+Filename: bosdyn/api/service_customization_pb2.py
+Comment: 
+
+Filename: bosdyn/api/service_customization_pb2_grpc.py
+Comment: 
+
 Filename: bosdyn/api/service_fault_pb2.py
 Comment: 
 
 Filename: bosdyn/api/service_fault_pb2_grpc.py
 Comment: 
 
 Filename: bosdyn/api/sparse_features_pb2.py
@@ -450,14 +462,20 @@
 
 Filename: bosdyn/api/trajectory_pb2.py
 Comment: 
 
 Filename: bosdyn/api/trajectory_pb2_grpc.py
 Comment: 
 
+Filename: bosdyn/api/units_pb2.py
+Comment: 
+
+Filename: bosdyn/api/units_pb2_grpc.py
+Comment: 
+
 Filename: bosdyn/api/world_object_pb2.py
 Comment: 
 
 Filename: bosdyn/api/world_object_pb2_grpc.py
 Comment: 
 
 Filename: bosdyn/api/world_object_service_pb2.py
@@ -516,14 +534,20 @@
 
 Filename: bosdyn/api/docking/docking_service_pb2_grpc.py
 Comment: 
 
 Filename: bosdyn/api/graph_nav/__init__.py
 Comment: 
 
+Filename: bosdyn/api/graph_nav/area_callback_data_pb2.py
+Comment: 
+
+Filename: bosdyn/api/graph_nav/area_callback_data_pb2_grpc.py
+Comment: 
+
 Filename: bosdyn/api/graph_nav/area_callback_pb2.py
 Comment: 
 
 Filename: bosdyn/api/graph_nav/area_callback_pb2_grpc.py
 Comment: 
 
 Filename: bosdyn/api/graph_nav/area_callback_service_pb2.py
@@ -576,14 +600,44 @@
 
 Filename: bosdyn/api/graph_nav/recording_service_pb2.py
 Comment: 
 
 Filename: bosdyn/api/graph_nav/recording_service_pb2_grpc.py
 Comment: 
 
+Filename: bosdyn/api/keepalive/__init__.py
+Comment: 
+
+Filename: bosdyn/api/keepalive/keepalive_pb2.py
+Comment: 
+
+Filename: bosdyn/api/keepalive/keepalive_pb2_grpc.py
+Comment: 
+
+Filename: bosdyn/api/keepalive/keepalive_service_pb2.py
+Comment: 
+
+Filename: bosdyn/api/keepalive/keepalive_service_pb2_grpc.py
+Comment: 
+
+Filename: bosdyn/api/log_status/__init__.py
+Comment: 
+
+Filename: bosdyn/api/log_status/log_status_pb2.py
+Comment: 
+
+Filename: bosdyn/api/log_status/log_status_pb2_grpc.py
+Comment: 
+
+Filename: bosdyn/api/log_status/log_status_service_pb2.py
+Comment: 
+
+Filename: bosdyn/api/log_status/log_status_service_pb2_grpc.py
+Comment: 
+
 Filename: bosdyn/api/mission/__init__.py
 Comment: 
 
 Filename: bosdyn/api/mission/mission_pb2.py
 Comment: 
 
 Filename: bosdyn/api/mission/mission_pb2_grpc.py
@@ -618,26 +672,44 @@
 
 Filename: bosdyn/api/mission/util_pb2_grpc.py
 Comment: 
 
 Filename: bosdyn/api/spot/__init__.py
 Comment: 
 
+Filename: bosdyn/api/spot/door_area_callback_pb2.py
+Comment: 
+
+Filename: bosdyn/api/spot/door_area_callback_pb2_grpc.py
+Comment: 
+
 Filename: bosdyn/api/spot/door_pb2.py
 Comment: 
 
 Filename: bosdyn/api/spot/door_pb2_grpc.py
 Comment: 
 
 Filename: bosdyn/api/spot/door_service_pb2.py
 Comment: 
 
 Filename: bosdyn/api/spot/door_service_pb2_grpc.py
 Comment: 
 
+Filename: bosdyn/api/spot/inverse_kinematics_pb2.py
+Comment: 
+
+Filename: bosdyn/api/spot/inverse_kinematics_pb2_grpc.py
+Comment: 
+
+Filename: bosdyn/api/spot/inverse_kinematics_service_pb2.py
+Comment: 
+
+Filename: bosdyn/api/spot/inverse_kinematics_service_pb2_grpc.py
+Comment: 
+
 Filename: bosdyn/api/spot/robot_command_pb2.py
 Comment: 
 
 Filename: bosdyn/api/spot/robot_command_pb2_grpc.py
 Comment: 
 
 Filename: bosdyn/api/spot/spot_check_pb2.py
@@ -723,20 +795,20 @@
 
 Filename: bosdyn/api/spot_cam/version_pb2.py
 Comment: 
 
 Filename: bosdyn/api/spot_cam/version_pb2_grpc.py
 Comment: 
 
-Filename: bosdyn_api-3.2.3.dist-info/METADATA
+Filename: bosdyn_api-3.3.0.dist-info/METADATA
 Comment: 
 
-Filename: bosdyn_api-3.2.3.dist-info/WHEEL
+Filename: bosdyn_api-3.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: bosdyn_api-3.2.3.dist-info/top_level.txt
+Filename: bosdyn_api-3.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: bosdyn_api-3.2.3.dist-info/RECORD
+Filename: bosdyn_api-3.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bosdyn/api/__init__.py

```diff
@@ -0,0 +1,4 @@
+00000000: 5f5f 7061 7468 5f5f 203d 205f 5f69 6d70  __path__ = __imp
+00000010: 6f72 745f 5f28 2770 6b67 7574 696c 2729  ort__('pkgutil')
+00000020: 2e65 7874 656e 645f 7061 7468 285f 5f70  .extend_path(__p
+00000030: 6174 685f 5f2c 205f 5f6e 616d 655f 5f29  ath__, __name__)
```

## bosdyn/api/arm_command_pb2.py

```diff
@@ -16,15 +16,15 @@
 from bosdyn.api import geometry_pb2 as bosdyn_dot_api_dot_geometry__pb2
 from bosdyn.api import trajectory_pb2 as bosdyn_dot_api_dot_trajectory__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1c\x62osdyn/api/arm_command.proto\x12\nbosdyn.api\x1a\x1e\x62osdyn/api/basic_command.proto\x1a\x19\x62osdyn/api/geometry.proto\x1a\x1b\x62osdyn/api/trajectory.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x1egoogle/protobuf/duration.proto\"\xa2\n\n\nArmCommand\x1a\xf3\x04\n\x07Request\x12H\n\x15\x61rm_cartesian_command\x18\x03 \x01(\x0b\x32\'.bosdyn.api.ArmCartesianCommand.RequestH\x00\x12I\n\x16\x61rm_joint_move_command\x18\x04 \x01(\x0b\x32\'.bosdyn.api.ArmJointMoveCommand.RequestH\x00\x12R\n\x1anamed_arm_position_command\x18\x05 \x01(\x0b\x32,.bosdyn.api.NamedArmPositionsCommand.RequestH\x00\x12\x46\n\x14\x61rm_velocity_command\x18\x06 \x01(\x0b\x32&.bosdyn.api.ArmVelocityCommand.RequestH\x00\x12;\n\x10\x61rm_gaze_command\x18\x08 \x01(\x0b\x32\x1f.bosdyn.api.GazeCommand.RequestH\x00\x12>\n\x10\x61rm_stop_command\x18\t \x01(\x0b\x32\".bosdyn.api.ArmStopCommand.RequestH\x00\x12>\n\x10\x61rm_drag_command\x18\n \x01(\x0b\x32\".bosdyn.api.ArmDragCommand.RequestH\x00\x12H\n\x15\x61rm_impedance_command\x18\x0c \x01(\x0b\x32\'.bosdyn.api.ArmImpedanceCommand.RequestH\x00\x12%\n\x06params\x18\x0b \x01(\x0b\x32\x15.bosdyn.api.ArmParamsB\t\n\x07\x63ommand\x1a\x9d\x05\n\x08\x46\x65\x65\x64\x62\x61\x63k\x12J\n\x16\x61rm_cartesian_feedback\x18\x03 \x01(\x0b\x32(.bosdyn.api.ArmCartesianCommand.FeedbackH\x00\x12K\n\x17\x61rm_joint_move_feedback\x18\x04 \x01(\x0b\x32(.bosdyn.api.ArmJointMoveCommand.FeedbackH\x00\x12T\n\x1bnamed_arm_position_feedback\x18\x05 \x01(\x0b\x32-.bosdyn.api.NamedArmPositionsCommand.FeedbackH\x00\x12H\n\x15\x61rm_velocity_feedback\x18\x06 \x01(\x0b\x32\'.bosdyn.api.ArmVelocityCommand.FeedbackH\x00\x12=\n\x11\x61rm_gaze_feedback\x18\x08 \x01(\x0b\x32 .bosdyn.api.GazeCommand.FeedbackH\x00\x12@\n\x11\x61rm_stop_feedback\x18\t \x01(\x0b\x32#.bosdyn.api.ArmStopCommand.FeedbackH\x00\x12@\n\x11\x61rm_drag_feedback\x18\n \x01(\x0b\x32#.bosdyn.api.ArmDragCommand.FeedbackH\x00\x12J\n\x16\x61rm_impedance_feedback\x18\x0c \x01(\x0b\x32(.bosdyn.api.ArmImpedanceCommand.FeedbackH\x00\x12=\n\x06status\x18\x64 \x01(\x0e\x32-.bosdyn.api.RobotCommandFeedbackStatus.StatusB\n\n\x08\x66\x65\x65\x64\x62\x61\x63k\"K\n\tArmParams\x12>\n\x1a\x64isable_body_force_limiter\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\"\xf9\x04\n\x12\x41rmVelocityCommand\x1a\x8c\x01\n\x13\x43ylindricalVelocity\x12:\n\x0flinear_velocity\x18\x01 \x01(\x0b\x32!.bosdyn.api.CylindricalCoordinate\x12\x39\n\x13max_linear_velocity\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x1aY\n\x11\x43\x61rtesianVelocity\x12\x12\n\nframe_name\x18\x01 \x01(\t\x12\x30\n\x16velocity_in_frame_name\x18\x02 \x01(\x0b\x32\x10.bosdyn.api.Vec3\x1a\xec\x02\n\x07Request\x12R\n\x14\x63ylindrical_velocity\x18\x01 \x01(\x0b\x32\x32.bosdyn.api.ArmVelocityCommand.CylindricalVelocityH\x00\x12N\n\x12\x63\x61rtesian_velocity\x18\x02 \x01(\x0b\x32\x30.bosdyn.api.ArmVelocityCommand.CartesianVelocityH\x00\x12\x42\n(angular_velocity_of_hand_rt_odom_in_hand\x18\x06 \x01(\x0b\x32\x10.bosdyn.api.Vec3\x12:\n\x14maximum_acceleration\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12,\n\x08\x65nd_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\t\n\x07\x63ommandJ\x04\x08\x04\x10\x05\x1a\n\n\x08\x46\x65\x65\x64\x62\x61\x63k\"\x88\x03\n\x18NamedArmPositionsCommand\x1aK\n\x07Request\x12@\n\x08position\x18\x01 \x01(\x0e\x32..bosdyn.api.NamedArmPositionsCommand.Positions\x1a\xbc\x01\n\x08\x46\x65\x65\x64\x62\x61\x63k\x12\x44\n\x06status\x18\x01 \x01(\x0e\x32\x34.bosdyn.api.NamedArmPositionsCommand.Feedback.Status\"j\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x13\n\x0fSTATUS_COMPLETE\x10\x01\x12\x16\n\x12STATUS_IN_PROGRESS\x10\x02\x12\x1f\n\x1bSTATUS_STALLED_HOLDING_ITEM\x10\x03\"`\n\tPositions\x12\x15\n\x11POSITIONS_UNKNOWN\x10\x00\x12\x13\n\x0fPOSITIONS_CARRY\x10\x01\x12\x13\n\x0fPOSITIONS_READY\x10\x02\x12\x12\n\x0ePOSITIONS_STOW\x10\x03\"\xab\x0c\n\x13\x41rmCartesianCommand\x1a\x96\t\n\x07Request\x12\x17\n\x0froot_frame_name\x18\x13 \x01(\t\x12-\n\x10wrist_tform_tool\x18\x06 \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\x12,\n\x0froot_tform_task\x18\x14 \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\x12:\n\x17pose_trajectory_in_task\x18\x02 \x01(\x0b\x32\x19.bosdyn.api.SE3Trajectory\x12:\n\x14maximum_acceleration\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x39\n\x13max_linear_velocity\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12:\n\x14max_angular_velocity\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12<\n\x16max_pos_tracking_error\x18\x0f \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12<\n\x16max_rot_tracking_error\x18\x10 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x37\n-force_remain_near_current_joint_configuration\x18\x11 \x01(\x08H\x00\x12\x45\n\x1dpreferred_joint_configuration\x18\x12 \x01(\x0b\x32\x1c.bosdyn.api.ArmJointPositionH\x00\x12@\n\x06x_axis\x18\x08 \x01(\x0e\x32\x30.bosdyn.api.ArmCartesianCommand.Request.AxisMode\x12@\n\x06y_axis\x18\t \x01(\x0e\x32\x30.bosdyn.api.ArmCartesianCommand.Request.AxisMode\x12@\n\x06z_axis\x18\n \x01(\x0e\x32\x30.bosdyn.api.ArmCartesianCommand.Request.AxisMode\x12\x41\n\x07rx_axis\x18\x0b \x01(\x0e\x32\x30.bosdyn.api.ArmCartesianCommand.Request.AxisMode\x12\x41\n\x07ry_axis\x18\x0c \x01(\x0e\x32\x30.bosdyn.api.ArmCartesianCommand.Request.AxisMode\x12\x41\n\x07rz_axis\x18\r \x01(\x0e\x32\x30.bosdyn.api.ArmCartesianCommand.Request.AxisMode\x12?\n\x19wrench_trajectory_in_task\x18\x0e \x01(\x0b\x32\x1c.bosdyn.api.WrenchTrajectory\"7\n\x08\x41xisMode\x12\x16\n\x12\x41XIS_MODE_POSITION\x10\x00\x12\x13\n\x0f\x41XIS_MODE_FORCE\x10\x01\x42\x15\n\x13joint_configurationJ\x04\x08\x01\x10\x02J\x04\x08\x07\x10\x08\x1a\xfa\x02\n\x08\x46\x65\x65\x64\x62\x61\x63k\x12?\n\x06status\x18\x01 \x01(\x0e\x32/.bosdyn.api.ArmCartesianCommand.Feedback.Status\x12#\n\x1bmeasured_pos_tracking_error\x18\x02 \x01(\x01\x12#\n\x1bmeasured_rot_tracking_error\x18\x03 \x01(\x01\x12%\n\x1dmeasured_pos_distance_to_goal\x18\x04 \x01(\x01\x12%\n\x1dmeasured_rot_distance_to_goal\x18\x05 \x01(\x01\"\x94\x01\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x1e\n\x1aSTATUS_TRAJECTORY_COMPLETE\x10\x01\x12\x16\n\x12STATUS_IN_PROGRESS\x10\x02\x12\x1f\n\x1bSTATUS_TRAJECTORY_CANCELLED\x10\x03\x12\x1d\n\x19STATUS_TRAJECTORY_STALLED\x10\x04\"\xc0\x04\n\x13\x41rmJointMoveCommand\x1a=\n\x07Request\x12\x32\n\ntrajectory\x18\x01 \x01(\x0b\x32\x1e.bosdyn.api.ArmJointTrajectory\x1a\xe9\x03\n\x08\x46\x65\x65\x64\x62\x61\x63k\x12?\n\x06status\x18\x01 \x01(\x0e\x32/.bosdyn.api.ArmJointMoveCommand.Feedback.Status\x12N\n\x0eplanner_status\x18\x02 \x01(\x0e\x32\x36.bosdyn.api.ArmJointMoveCommand.Feedback.PlannerStatus\x12;\n\x0eplanned_points\x18\x03 \x03(\x0b\x32#.bosdyn.api.ArmJointTrajectoryPoint\x12/\n\x0ctime_to_goal\x18\x04 \x01(\x0b\x32\x19.google.protobuf.Duration\"]\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x13\n\x0fSTATUS_COMPLETE\x10\x01\x12\x16\n\x12STATUS_IN_PROGRESS\x10\x02\x12\x12\n\x0eSTATUS_STALLED\x10\x03\"\x7f\n\rPlannerStatus\x12\x1a\n\x16PLANNER_STATUS_UNKNOWN\x10\x00\x12\x1a\n\x16PLANNER_STATUS_SUCCESS\x10\x01\x12\x1b\n\x17PLANNER_STATUS_MODIFIED\x10\x02\x12\x19\n\x15PLANNER_STATUS_FAILED\x10\x03\"\x94\x02\n\x10\x41rmJointPosition\x12)\n\x03sh0\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12)\n\x03sh1\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12)\n\x03\x65l0\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12)\n\x03\x65l1\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12)\n\x03wr0\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12)\n\x03wr1\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\x94\x02\n\x10\x41rmJointVelocity\x12)\n\x03sh0\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12)\n\x03sh1\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12)\n\x03\x65l0\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12)\n\x03\x65l1\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12)\n\x03wr0\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12)\n\x03wr1\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\xb2\x01\n\x17\x41rmJointTrajectoryPoint\x12.\n\x08position\x18\x01 \x01(\x0b\x32\x1c.bosdyn.api.ArmJointPosition\x12.\n\x08velocity\x18\x02 \x01(\x0b\x32\x1c.bosdyn.api.ArmJointVelocity\x12\x37\n\x14time_since_reference\x18\x03 \x01(\x0b\x32\x19.google.protobuf.Duration\"\xf1\x01\n\x12\x41rmJointTrajectory\x12\x33\n\x06points\x18\x01 \x03(\x0b\x32#.bosdyn.api.ArmJointTrajectoryPoint\x12\x32\n\x0ereference_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x36\n\x10maximum_velocity\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12:\n\x14maximum_acceleration\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\x8b\x07\n\x0bGazeCommand\x1a\xea\x03\n\x07Request\x12?\n\x1btarget_trajectory_in_frame1\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.Vec3Trajectory\x12\x13\n\x0b\x66rame1_name\x18\x02 \x01(\t\x12<\n\x19tool_trajectory_in_frame2\x18\n \x01(\x0b\x32\x19.bosdyn.api.SE3Trajectory\x12\x13\n\x0b\x66rame2_name\x18\x0b \x01(\t\x12-\n\x10wrist_tform_tool\x18\t \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\x12H\n\"target_trajectory_initial_velocity\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12:\n\x14maximum_acceleration\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x39\n\x13max_linear_velocity\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12:\n\x14max_angular_velocity\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.DoubleValueJ\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05\x1a\x8e\x03\n\x08\x46\x65\x65\x64\x62\x61\x63k\x12\x37\n\x06status\x18\x01 \x01(\x0e\x32\'.bosdyn.api.GazeCommand.Feedback.Status\x12\x18\n\x10gazing_at_target\x18\x02 \x01(\x08\x12(\n gaze_to_target_rotation_measured\x18\x05 \x01(\x02\x12\x1d\n\x15hand_position_at_goal\x18\x03 \x01(\x08\x12&\n\x1ehand_distance_to_goal_measured\x18\x06 \x01(\x02\x12\x19\n\x11hand_roll_at_goal\x18\x04 \x01(\x08\x12)\n!hand_roll_to_target_roll_measured\x18\x07 \x01(\x02\"x\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x1e\n\x1aSTATUS_TRAJECTORY_COMPLETE\x10\x01\x12\x16\n\x12STATUS_IN_PROGRESS\x10\x02\x12\"\n\x1eSTATUS_TOOL_TRAJECTORY_STALLED\x10\x03\"\'\n\x0e\x41rmStopCommand\x1a\t\n\x07Request\x1a\n\n\x08\x46\x65\x65\x64\x62\x61\x63k\"\xff\x03\n\x13\x41rmImpedanceCommand\x1a\xdb\x03\n\x07Request\x12\x17\n\x0froot_frame_name\x18\x01 \x01(\t\x12,\n\x0froot_tform_task\x18\x02 \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\x12-\n\x10wrist_tform_tool\x18\x03 \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\x12:\n\x17task_tform_desired_tool\x18\x04 \x01(\x0b\x32\x19.bosdyn.api.SE3Trajectory\x12G\n+feed_forward_wrench_at_tool_in_desired_tool\x18\x05 \x01(\x0b\x32\x12.bosdyn.api.Wrench\x12\x35\n\x19\x64iagonal_stiffness_matrix\x18\x06 \x01(\x0b\x32\x12.bosdyn.api.Vector\x12\x33\n\x17\x64iagonal_damping_matrix\x18\x07 \x01(\x0b\x32\x12.bosdyn.api.Vector\x12\x33\n\rmax_force_mag\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x34\n\x0emax_torque_mag\x18\t \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x1a\n\n\x08\x46\x65\x65\x64\x62\x61\x63kB\x11\x42\x0f\x41rmCommandProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1c\x62osdyn/api/arm_command.proto\x12\nbosdyn.api\x1a\x1e\x62osdyn/api/basic_command.proto\x1a\x19\x62osdyn/api/geometry.proto\x1a\x1b\x62osdyn/api/trajectory.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x1egoogle/protobuf/duration.proto\"\xa2\n\n\nArmCommand\x1a\xf3\x04\n\x07Request\x12H\n\x15\x61rm_cartesian_command\x18\x03 \x01(\x0b\x32\'.bosdyn.api.ArmCartesianCommand.RequestH\x00\x12I\n\x16\x61rm_joint_move_command\x18\x04 \x01(\x0b\x32\'.bosdyn.api.ArmJointMoveCommand.RequestH\x00\x12R\n\x1anamed_arm_position_command\x18\x05 \x01(\x0b\x32,.bosdyn.api.NamedArmPositionsCommand.RequestH\x00\x12\x46\n\x14\x61rm_velocity_command\x18\x06 \x01(\x0b\x32&.bosdyn.api.ArmVelocityCommand.RequestH\x00\x12;\n\x10\x61rm_gaze_command\x18\x08 \x01(\x0b\x32\x1f.bosdyn.api.GazeCommand.RequestH\x00\x12>\n\x10\x61rm_stop_command\x18\t \x01(\x0b\x32\".bosdyn.api.ArmStopCommand.RequestH\x00\x12>\n\x10\x61rm_drag_command\x18\n \x01(\x0b\x32\".bosdyn.api.ArmDragCommand.RequestH\x00\x12H\n\x15\x61rm_impedance_command\x18\x0c \x01(\x0b\x32\'.bosdyn.api.ArmImpedanceCommand.RequestH\x00\x12%\n\x06params\x18\x0b \x01(\x0b\x32\x15.bosdyn.api.ArmParamsB\t\n\x07\x63ommand\x1a\x9d\x05\n\x08\x46\x65\x65\x64\x62\x61\x63k\x12J\n\x16\x61rm_cartesian_feedback\x18\x03 \x01(\x0b\x32(.bosdyn.api.ArmCartesianCommand.FeedbackH\x00\x12K\n\x17\x61rm_joint_move_feedback\x18\x04 \x01(\x0b\x32(.bosdyn.api.ArmJointMoveCommand.FeedbackH\x00\x12T\n\x1bnamed_arm_position_feedback\x18\x05 \x01(\x0b\x32-.bosdyn.api.NamedArmPositionsCommand.FeedbackH\x00\x12H\n\x15\x61rm_velocity_feedback\x18\x06 \x01(\x0b\x32\'.bosdyn.api.ArmVelocityCommand.FeedbackH\x00\x12=\n\x11\x61rm_gaze_feedback\x18\x08 \x01(\x0b\x32 .bosdyn.api.GazeCommand.FeedbackH\x00\x12@\n\x11\x61rm_stop_feedback\x18\t \x01(\x0b\x32#.bosdyn.api.ArmStopCommand.FeedbackH\x00\x12@\n\x11\x61rm_drag_feedback\x18\n \x01(\x0b\x32#.bosdyn.api.ArmDragCommand.FeedbackH\x00\x12J\n\x16\x61rm_impedance_feedback\x18\x0c \x01(\x0b\x32(.bosdyn.api.ArmImpedanceCommand.FeedbackH\x00\x12=\n\x06status\x18\x64 \x01(\x0e\x32-.bosdyn.api.RobotCommandFeedbackStatus.StatusB\n\n\x08\x66\x65\x65\x64\x62\x61\x63k\"K\n\tArmParams\x12>\n\x1a\x64isable_body_force_limiter\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\"\xf9\x04\n\x12\x41rmVelocityCommand\x1a\x8c\x01\n\x13\x43ylindricalVelocity\x12:\n\x0flinear_velocity\x18\x01 \x01(\x0b\x32!.bosdyn.api.CylindricalCoordinate\x12\x39\n\x13max_linear_velocity\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x1aY\n\x11\x43\x61rtesianVelocity\x12\x12\n\nframe_name\x18\x01 \x01(\t\x12\x30\n\x16velocity_in_frame_name\x18\x02 \x01(\x0b\x32\x10.bosdyn.api.Vec3\x1a\xec\x02\n\x07Request\x12R\n\x14\x63ylindrical_velocity\x18\x01 \x01(\x0b\x32\x32.bosdyn.api.ArmVelocityCommand.CylindricalVelocityH\x00\x12N\n\x12\x63\x61rtesian_velocity\x18\x02 \x01(\x0b\x32\x30.bosdyn.api.ArmVelocityCommand.CartesianVelocityH\x00\x12\x42\n(angular_velocity_of_hand_rt_odom_in_hand\x18\x06 \x01(\x0b\x32\x10.bosdyn.api.Vec3\x12:\n\x14maximum_acceleration\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12,\n\x08\x65nd_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\t\n\x07\x63ommandJ\x04\x08\x04\x10\x05\x1a\n\n\x08\x46\x65\x65\x64\x62\x61\x63k\"\x88\x03\n\x18NamedArmPositionsCommand\x1aK\n\x07Request\x12@\n\x08position\x18\x01 \x01(\x0e\x32..bosdyn.api.NamedArmPositionsCommand.Positions\x1a\xbc\x01\n\x08\x46\x65\x65\x64\x62\x61\x63k\x12\x44\n\x06status\x18\x01 \x01(\x0e\x32\x34.bosdyn.api.NamedArmPositionsCommand.Feedback.Status\"j\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x13\n\x0fSTATUS_COMPLETE\x10\x01\x12\x16\n\x12STATUS_IN_PROGRESS\x10\x02\x12\x1f\n\x1bSTATUS_STALLED_HOLDING_ITEM\x10\x03\"`\n\tPositions\x12\x15\n\x11POSITIONS_UNKNOWN\x10\x00\x12\x13\n\x0fPOSITIONS_CARRY\x10\x01\x12\x13\n\x0fPOSITIONS_READY\x10\x02\x12\x12\n\x0ePOSITIONS_STOW\x10\x03\"\xab\x0c\n\x13\x41rmCartesianCommand\x1a\x96\t\n\x07Request\x12\x17\n\x0froot_frame_name\x18\x13 \x01(\t\x12-\n\x10wrist_tform_tool\x18\x06 \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\x12,\n\x0froot_tform_task\x18\x14 \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\x12:\n\x17pose_trajectory_in_task\x18\x02 \x01(\x0b\x32\x19.bosdyn.api.SE3Trajectory\x12:\n\x14maximum_acceleration\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x39\n\x13max_linear_velocity\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12:\n\x14max_angular_velocity\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12<\n\x16max_pos_tracking_error\x18\x0f \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12<\n\x16max_rot_tracking_error\x18\x10 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x37\n-force_remain_near_current_joint_configuration\x18\x11 \x01(\x08H\x00\x12\x45\n\x1dpreferred_joint_configuration\x18\x12 \x01(\x0b\x32\x1c.bosdyn.api.ArmJointPositionH\x00\x12@\n\x06x_axis\x18\x08 \x01(\x0e\x32\x30.bosdyn.api.ArmCartesianCommand.Request.AxisMode\x12@\n\x06y_axis\x18\t \x01(\x0e\x32\x30.bosdyn.api.ArmCartesianCommand.Request.AxisMode\x12@\n\x06z_axis\x18\n \x01(\x0e\x32\x30.bosdyn.api.ArmCartesianCommand.Request.AxisMode\x12\x41\n\x07rx_axis\x18\x0b \x01(\x0e\x32\x30.bosdyn.api.ArmCartesianCommand.Request.AxisMode\x12\x41\n\x07ry_axis\x18\x0c \x01(\x0e\x32\x30.bosdyn.api.ArmCartesianCommand.Request.AxisMode\x12\x41\n\x07rz_axis\x18\r \x01(\x0e\x32\x30.bosdyn.api.ArmCartesianCommand.Request.AxisMode\x12?\n\x19wrench_trajectory_in_task\x18\x0e \x01(\x0b\x32\x1c.bosdyn.api.WrenchTrajectory\"7\n\x08\x41xisMode\x12\x16\n\x12\x41XIS_MODE_POSITION\x10\x00\x12\x13\n\x0f\x41XIS_MODE_FORCE\x10\x01\x42\x15\n\x13joint_configurationJ\x04\x08\x01\x10\x02J\x04\x08\x07\x10\x08\x1a\xfa\x02\n\x08\x46\x65\x65\x64\x62\x61\x63k\x12?\n\x06status\x18\x01 \x01(\x0e\x32/.bosdyn.api.ArmCartesianCommand.Feedback.Status\x12#\n\x1bmeasured_pos_tracking_error\x18\x02 \x01(\x01\x12#\n\x1bmeasured_rot_tracking_error\x18\x03 \x01(\x01\x12%\n\x1dmeasured_pos_distance_to_goal\x18\x04 \x01(\x01\x12%\n\x1dmeasured_rot_distance_to_goal\x18\x05 \x01(\x01\"\x94\x01\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x1e\n\x1aSTATUS_TRAJECTORY_COMPLETE\x10\x01\x12\x16\n\x12STATUS_IN_PROGRESS\x10\x02\x12\x1f\n\x1bSTATUS_TRAJECTORY_CANCELLED\x10\x03\x12\x1d\n\x19STATUS_TRAJECTORY_STALLED\x10\x04\"\xc0\x04\n\x13\x41rmJointMoveCommand\x1a=\n\x07Request\x12\x32\n\ntrajectory\x18\x01 \x01(\x0b\x32\x1e.bosdyn.api.ArmJointTrajectory\x1a\xe9\x03\n\x08\x46\x65\x65\x64\x62\x61\x63k\x12?\n\x06status\x18\x01 \x01(\x0e\x32/.bosdyn.api.ArmJointMoveCommand.Feedback.Status\x12N\n\x0eplanner_status\x18\x02 \x01(\x0e\x32\x36.bosdyn.api.ArmJointMoveCommand.Feedback.PlannerStatus\x12;\n\x0eplanned_points\x18\x03 \x03(\x0b\x32#.bosdyn.api.ArmJointTrajectoryPoint\x12/\n\x0ctime_to_goal\x18\x04 \x01(\x0b\x32\x19.google.protobuf.Duration\"]\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x13\n\x0fSTATUS_COMPLETE\x10\x01\x12\x16\n\x12STATUS_IN_PROGRESS\x10\x02\x12\x12\n\x0eSTATUS_STALLED\x10\x03\"\x7f\n\rPlannerStatus\x12\x1a\n\x16PLANNER_STATUS_UNKNOWN\x10\x00\x12\x1a\n\x16PLANNER_STATUS_SUCCESS\x10\x01\x12\x1b\n\x17PLANNER_STATUS_MODIFIED\x10\x02\x12\x19\n\x15PLANNER_STATUS_FAILED\x10\x03\"\x94\x02\n\x10\x41rmJointPosition\x12)\n\x03sh0\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12)\n\x03sh1\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12)\n\x03\x65l0\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12)\n\x03\x65l1\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12)\n\x03wr0\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12)\n\x03wr1\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\x94\x02\n\x10\x41rmJointVelocity\x12)\n\x03sh0\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12)\n\x03sh1\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12)\n\x03\x65l0\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12)\n\x03\x65l1\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12)\n\x03wr0\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12)\n\x03wr1\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\xb2\x01\n\x17\x41rmJointTrajectoryPoint\x12.\n\x08position\x18\x01 \x01(\x0b\x32\x1c.bosdyn.api.ArmJointPosition\x12.\n\x08velocity\x18\x02 \x01(\x0b\x32\x1c.bosdyn.api.ArmJointVelocity\x12\x37\n\x14time_since_reference\x18\x03 \x01(\x0b\x32\x19.google.protobuf.Duration\"\xf1\x01\n\x12\x41rmJointTrajectory\x12\x33\n\x06points\x18\x01 \x03(\x0b\x32#.bosdyn.api.ArmJointTrajectoryPoint\x12\x32\n\x0ereference_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x36\n\x10maximum_velocity\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12:\n\x14maximum_acceleration\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\x8b\x07\n\x0bGazeCommand\x1a\xea\x03\n\x07Request\x12?\n\x1btarget_trajectory_in_frame1\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.Vec3Trajectory\x12\x13\n\x0b\x66rame1_name\x18\x02 \x01(\t\x12<\n\x19tool_trajectory_in_frame2\x18\n \x01(\x0b\x32\x19.bosdyn.api.SE3Trajectory\x12\x13\n\x0b\x66rame2_name\x18\x0b \x01(\t\x12-\n\x10wrist_tform_tool\x18\t \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\x12H\n\"target_trajectory_initial_velocity\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12:\n\x14maximum_acceleration\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x39\n\x13max_linear_velocity\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12:\n\x14max_angular_velocity\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.DoubleValueJ\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05\x1a\x8e\x03\n\x08\x46\x65\x65\x64\x62\x61\x63k\x12\x37\n\x06status\x18\x01 \x01(\x0e\x32\'.bosdyn.api.GazeCommand.Feedback.Status\x12\x18\n\x10gazing_at_target\x18\x02 \x01(\x08\x12(\n gaze_to_target_rotation_measured\x18\x05 \x01(\x02\x12\x1d\n\x15hand_position_at_goal\x18\x03 \x01(\x08\x12&\n\x1ehand_distance_to_goal_measured\x18\x06 \x01(\x02\x12\x19\n\x11hand_roll_at_goal\x18\x04 \x01(\x08\x12)\n!hand_roll_to_target_roll_measured\x18\x07 \x01(\x02\"x\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x1e\n\x1aSTATUS_TRAJECTORY_COMPLETE\x10\x01\x12\x16\n\x12STATUS_IN_PROGRESS\x10\x02\x12\"\n\x1eSTATUS_TOOL_TRAJECTORY_STALLED\x10\x03\"\'\n\x0e\x41rmStopCommand\x1a\t\n\x07Request\x1a\n\n\x08\x46\x65\x65\x64\x62\x61\x63k\"\x89\t\n\x13\x41rmImpedanceCommand\x1a\xdb\x03\n\x07Request\x12\x17\n\x0froot_frame_name\x18\x01 \x01(\t\x12,\n\x0froot_tform_task\x18\x02 \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\x12-\n\x10wrist_tform_tool\x18\x03 \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\x12:\n\x17task_tform_desired_tool\x18\x04 \x01(\x0b\x32\x19.bosdyn.api.SE3Trajectory\x12G\n+feed_forward_wrench_at_tool_in_desired_tool\x18\x05 \x01(\x0b\x32\x12.bosdyn.api.Wrench\x12\x35\n\x19\x64iagonal_stiffness_matrix\x18\x06 \x01(\x0b\x32\x12.bosdyn.api.Vector\x12\x33\n\x17\x64iagonal_damping_matrix\x18\x07 \x01(\x0b\x32\x12.bosdyn.api.Vector\x12\x33\n\rmax_force_mag\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x34\n\x0emax_torque_mag\x18\t \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x1a\x93\x05\n\x08\x46\x65\x65\x64\x62\x61\x63k\x12?\n\x06status\x18\x01 \x01(\x0e\x32/.bosdyn.api.ArmImpedanceCommand.Feedback.Status\x12:\n\x13transforms_snapshot\x18\x02 \x01(\x0b\x32\x1d.bosdyn.api.FrameTreeSnapshot\x12S\n7commanded_wrench_from_stiffness_at_tool_in_desired_tool\x18\x03 \x01(\x0b\x32\x12.bosdyn.api.Wrench\x12Q\n5commanded_wrench_from_damping_at_tool_in_desired_tool\x18\x04 \x01(\x0b\x32\x12.bosdyn.api.Wrench\x12V\n:commanded_wrench_from_feed_forward_at_tool_in_desired_tool\x18\x05 \x01(\x0b\x32\x12.bosdyn.api.Wrench\x12J\n.total_commanded_wrench_at_tool_in_desired_tool\x18\x06 \x01(\x0b\x32\x12.bosdyn.api.Wrench\x12I\n-total_measured_wrench_at_tool_in_desired_tool\x18\x07 \x01(\x0b\x32\x12.bosdyn.api.Wrench\"s\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x1e\n\x1aSTATUS_TRAJECTORY_COMPLETE\x10\x01\x12\x16\n\x12STATUS_IN_PROGRESS\x10\x02\x12\x1d\n\x19STATUS_TRAJECTORY_STALLED\x10\x03\x42\x11\x42\x0f\x41rmCommandProtob\x06proto3')
 
 
 
 _ARMCOMMAND = DESCRIPTOR.message_types_by_name['ArmCommand']
 _ARMCOMMAND_REQUEST = _ARMCOMMAND.nested_types_by_name['Request']
 _ARMCOMMAND_FEEDBACK = _ARMCOMMAND.nested_types_by_name['Feedback']
 _ARMPARAMS = DESCRIPTOR.message_types_by_name['ArmParams']
@@ -58,14 +58,15 @@
 _NAMEDARMPOSITIONSCOMMAND_FEEDBACK_STATUS = _NAMEDARMPOSITIONSCOMMAND_FEEDBACK.enum_types_by_name['Status']
 _NAMEDARMPOSITIONSCOMMAND_POSITIONS = _NAMEDARMPOSITIONSCOMMAND.enum_types_by_name['Positions']
 _ARMCARTESIANCOMMAND_REQUEST_AXISMODE = _ARMCARTESIANCOMMAND_REQUEST.enum_types_by_name['AxisMode']
 _ARMCARTESIANCOMMAND_FEEDBACK_STATUS = _ARMCARTESIANCOMMAND_FEEDBACK.enum_types_by_name['Status']
 _ARMJOINTMOVECOMMAND_FEEDBACK_STATUS = _ARMJOINTMOVECOMMAND_FEEDBACK.enum_types_by_name['Status']
 _ARMJOINTMOVECOMMAND_FEEDBACK_PLANNERSTATUS = _ARMJOINTMOVECOMMAND_FEEDBACK.enum_types_by_name['PlannerStatus']
 _GAZECOMMAND_FEEDBACK_STATUS = _GAZECOMMAND_FEEDBACK.enum_types_by_name['Status']
+_ARMIMPEDANCECOMMAND_FEEDBACK_STATUS = _ARMIMPEDANCECOMMAND_FEEDBACK.enum_types_by_name['Status']
 ArmCommand = _reflection.GeneratedProtocolMessageType('ArmCommand', (_message.Message,), {
 
   'Request' : _reflection.GeneratedProtocolMessageType('Request', (_message.Message,), {
     'DESCRIPTOR' : _ARMCOMMAND_REQUEST,
     '__module__' : 'bosdyn.api.arm_command_pb2'
     # @@protoc_insertion_point(class_scope:bosdyn.api.ArmCommand.Request)
     })
@@ -368,13 +369,15 @@
   _ARMSTOPCOMMAND._serialized_start=6708
   _ARMSTOPCOMMAND._serialized_end=6747
   _ARMSTOPCOMMAND_REQUEST._serialized_start=245
   _ARMSTOPCOMMAND_REQUEST._serialized_end=254
   _ARMSTOPCOMMAND_FEEDBACK._serialized_start=875
   _ARMSTOPCOMMAND_FEEDBACK._serialized_end=885
   _ARMIMPEDANCECOMMAND._serialized_start=6750
-  _ARMIMPEDANCECOMMAND._serialized_end=7261
+  _ARMIMPEDANCECOMMAND._serialized_end=7911
   _ARMIMPEDANCECOMMAND_REQUEST._serialized_start=6774
   _ARMIMPEDANCECOMMAND_REQUEST._serialized_end=7249
-  _ARMIMPEDANCECOMMAND_FEEDBACK._serialized_start=875
-  _ARMIMPEDANCECOMMAND_FEEDBACK._serialized_end=885
+  _ARMIMPEDANCECOMMAND_FEEDBACK._serialized_start=7252
+  _ARMIMPEDANCECOMMAND_FEEDBACK._serialized_end=7911
+  _ARMIMPEDANCECOMMAND_FEEDBACK_STATUS._serialized_start=7796
+  _ARMIMPEDANCECOMMAND_FEEDBACK_STATUS._serialized_end=7911
 # @@protoc_insertion_point(module_scope)
```

## bosdyn/api/basic_command_pb2.py

```diff
@@ -14,15 +14,15 @@
 
 from bosdyn.api import geometry_pb2 as bosdyn_dot_api_dot_geometry__pb2
 from bosdyn.api import trajectory_pb2 as bosdyn_dot_api_dot_trajectory__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1e\x62osdyn/api/basic_command.proto\x12\nbosdyn.api\x1a\x19\x62osdyn/api/geometry.proto\x1a\x1b\x62osdyn/api/trajectory.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\xca\x01\n\x1aRobotCommandFeedbackStatus\"\xab\x01\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x15\n\x11STATUS_PROCESSING\x10\x01\x12\x1d\n\x19STATUS_COMMAND_OVERRIDDEN\x10\x02\x12\x1c\n\x18STATUS_COMMAND_TIMED_OUT\x10\x03\x12\x17\n\x13STATUS_ROBOT_FROZEN\x10\x04\x12 \n\x1cSTATUS_INCOMPATIBLE_HARDWARE\x10\x05\"\xee\x02\n\x18\x42\x61tteryChangePoseCommand\x1a\x9f\x01\n\x07Request\x12R\n\x0e\x64irection_hint\x18\x01 \x01(\x0e\x32:.bosdyn.api.BatteryChangePoseCommand.Request.DirectionHint\"@\n\rDirectionHint\x12\x10\n\x0cHINT_UNKNOWN\x10\x00\x12\x0e\n\nHINT_RIGHT\x10\x01\x12\r\n\tHINT_LEFT\x10\x02\x1a\xaf\x01\n\x08\x46\x65\x65\x64\x62\x61\x63k\x12\x44\n\x06status\x18\x01 \x01(\x0e\x32\x34.bosdyn.api.BatteryChangePoseCommand.Feedback.Status\"]\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x14\n\x10STATUS_COMPLETED\x10\x01\x12\x16\n\x12STATUS_IN_PROGRESS\x10\x02\x12\x11\n\rSTATUS_FAILED\x10\x03\"\xb4\x01\n\x10SelfRightCommand\x1a\t\n\x07Request\x1a\x94\x01\n\x08\x46\x65\x65\x64\x62\x61\x63k\x12<\n\x06status\x18\x01 \x01(\x0e\x32,.bosdyn.api.SelfRightCommand.Feedback.Status\"J\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x14\n\x10STATUS_COMPLETED\x10\x01\x12\x16\n\x12STATUS_IN_PROGRESS\x10\x02\"$\n\x0bStopCommand\x1a\t\n\x07Request\x1a\n\n\x08\x46\x65\x65\x64\x62\x61\x63k\"&\n\rFreezeCommand\x1a\t\n\x07Request\x1a\n\n\x08\x46\x65\x65\x64\x62\x61\x63k\"\xea\x02\n\x13SafePowerOffCommand\x1a\xb6\x01\n\x07Request\x12K\n\runsafe_action\x18\x01 \x01(\x0e\x32\x34.bosdyn.api.SafePowerOffCommand.Request.UnsafeAction\"^\n\x0cUnsafeAction\x12\x12\n\x0eUNSAFE_UNKNOWN\x10\x00\x12 \n\x1cUNSAFE_MOVE_TO_SAFE_POSITION\x10\x01\x12\x18\n\x14UNSAFE_FORCE_COMMAND\x10\x02\x1a\x99\x01\n\x08\x46\x65\x65\x64\x62\x61\x63k\x12?\n\x06status\x18\x01 \x01(\x0e\x32/.bosdyn.api.SafePowerOffCommand.Feedback.Status\"L\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x16\n\x12STATUS_POWERED_OFF\x10\x01\x12\x16\n\x12STATUS_IN_PROGRESS\x10\x02\"\x83\x04\n\x14SE2TrajectoryCommand\x1a~\n\x07Request\x12,\n\x08\x65nd_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0ese2_frame_name\x18\x03 \x01(\t\x12-\n\ntrajectory\x18\x02 \x01(\x0b\x32\x19.bosdyn.api.SE2Trajectory\x1a\xea\x02\n\x08\x46\x65\x65\x64\x62\x61\x63k\x12@\n\x06status\x18\x01 \x01(\x0e\x32\x30.bosdyn.api.SE2TrajectoryCommand.Feedback.Status\x12Z\n\x14\x62ody_movement_status\x18\x02 \x01(\x0e\x32<.bosdyn.api.SE2TrajectoryCommand.Feedback.BodyMovementStatus\"`\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x12\n\x0eSTATUS_AT_GOAL\x10\x01\x12\x14\n\x10STATUS_NEAR_GOAL\x10\x03\x12\x18\n\x14STATUS_GOING_TO_GOAL\x10\x02\"^\n\x12\x42odyMovementStatus\x12\x17\n\x13\x42ODY_STATUS_UNKNOWN\x10\x00\x12\x16\n\x12\x42ODY_STATUS_MOVING\x10\x01\x12\x17\n\x13\x42ODY_STATUS_SETTLED\x10\x02\"\xd5\x01\n\x12SE2VelocityCommand\x1a\xb2\x01\n\x07Request\x12,\n\x08\x65nd_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0ese2_frame_name\x18\x05 \x01(\t\x12)\n\x08velocity\x18\x02 \x01(\x0b\x32\x17.bosdyn.api.SE2Velocity\x12\x30\n\x0fslew_rate_limit\x18\x04 \x01(\x0b\x32\x17.bosdyn.api.SE2VelocityJ\x04\x08\x03\x10\x04\x1a\n\n\x08\x46\x65\x65\x64\x62\x61\x63k\"\xa9\x01\n\nSitCommand\x1a\t\n\x07Request\x1a\x8f\x01\n\x08\x46\x65\x65\x64\x62\x61\x63k\x12\x36\n\x06status\x18\x02 \x01(\x0e\x32&.bosdyn.api.SitCommand.Feedback.Status\"K\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x15\n\x11STATUS_IS_SITTING\x10\x01\x12\x16\n\x12STATUS_IN_PROGRESS\x10\x02\"\xcc\x02\n\x0cStandCommand\x1a\t\n\x07Request\x1a\xb0\x02\n\x08\x46\x65\x65\x64\x62\x61\x63k\x12\x38\n\x06status\x18\x01 \x01(\x0e\x32(.bosdyn.api.StandCommand.Feedback.Status\x12G\n\x0estanding_state\x18\x02 \x01(\x0e\x32/.bosdyn.api.StandCommand.Feedback.StandingState\"L\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x16\n\x12STATUS_IS_STANDING\x10\x01\x12\x16\n\x12STATUS_IN_PROGRESS\x10\x02\"S\n\rStandingState\x12\x14\n\x10STANDING_UNKNOWN\x10\x00\x12\x17\n\x13STANDING_CONTROLLED\x10\x01\x12\x13\n\x0fSTANDING_FROZEN\x10\x02\"\x9b\x02\n\rStanceCommand\x1a[\n\x07Request\x12,\n\x08\x65nd_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\"\n\x06stance\x18\x02 \x01(\x0b\x32\x12.bosdyn.api.Stance\x1a\xac\x01\n\x08\x46\x65\x65\x64\x62\x61\x63k\x12\x39\n\x06status\x18\x01 \x01(\x0e\x32).bosdyn.api.StanceCommand.Feedback.Status\"e\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x12\n\x0eSTATUS_STANCED\x10\x01\x12\x1a\n\x16STATUS_GOING_TO_STANCE\x10\x02\x12\x17\n\x13STATUS_TOO_FAR_AWAY\x10\x03\"\xb9\x01\n\x06Stance\x12\x16\n\x0ese2_frame_name\x18\x03 \x01(\t\x12=\n\x0e\x66oot_positions\x18\x02 \x03(\x0b\x32%.bosdyn.api.Stance.FootPositionsEntry\x12\x10\n\x08\x61\x63\x63uracy\x18\x04 \x01(\x02\x1a\x46\n\x12\x46ootPositionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1f\n\x05value\x18\x02 \x01(\x0b\x32\x10.bosdyn.api.Vec2:\x02\x38\x01\"w\n\x10\x46ollowArmCommand\x1aW\n\x07Request\x12/\n\x15\x62ody_offset_from_hand\x18\x01 \x01(\x0b\x32\x10.bosdyn.api.Vec3\x12\x1b\n\x0f\x64isable_walking\x18\x02 \x01(\x08\x42\x02\x18\x01\x1a\n\n\x08\x46\x65\x65\x64\x62\x61\x63k\"\xca\x01\n\x0e\x41rmDragCommand\x1a\t\n\x07Request\x1a\xac\x01\n\x08\x46\x65\x65\x64\x62\x61\x63k\x12:\n\x06status\x18\x01 \x01(\x0e\x32*.bosdyn.api.ArmDragCommand.Feedback.Status\"d\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x13\n\x0fSTATUS_DRAGGING\x10\x01\x12\x17\n\x13STATUS_GRASP_FAILED\x10\x02\x12\x18\n\x14STATUS_OTHER_FAILURE\x10\x03\"\xcd\x07\n\x1e\x43onstrainedManipulationCommand\x1a\xb5\x05\n\x07Request\x12\x12\n\nframe_name\x18\x01 \x01(\t\x12?\n#init_wrench_direction_in_frame_name\x18\x02 \x01(\x0b\x32\x12.bosdyn.api.Wrench\x12\x1a\n\x10tangential_speed\x18\x03 \x01(\x01H\x00\x12\x1a\n\x10rotational_speed\x18\x04 \x01(\x01H\x00\x12\x31\n\x0b\x66orce_limit\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x32\n\x0ctorque_limit\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12N\n\ttask_type\x18\x07 \x01(\x0e\x32;.bosdyn.api.ConstrainedManipulationCommand.Request.TaskType\x12,\n\x08\x65nd_time\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12;\n\x17\x65nable_robot_locomotion\x18\t \x01(\x0b\x32\x1a.google.protobuf.BoolValue\"\xec\x01\n\x08TaskType\x12\x15\n\x11TASK_TYPE_UNKNOWN\x10\x00\x12%\n!TASK_TYPE_SE3_CIRCLE_FORCE_TORQUE\x10\x01\x12&\n\"TASK_TYPE_R3_CIRCLE_EXTRADOF_FORCE\x10\x02\x12#\n\x1fTASK_TYPE_SE3_ROTATIONAL_TORQUE\x10\x03\x12\x1d\n\x19TASK_TYPE_R3_CIRCLE_FORCE\x10\x04\x12\x1d\n\x19TASK_TYPE_R3_LINEAR_FORCE\x10\x05\x12\x17\n\x13TASK_TYPE_HOLD_POSE\x10\x06\x42\x0c\n\ntask_speed\x1a\xf2\x01\n\x08\x46\x65\x65\x64\x62\x61\x63k\x12J\n\x06status\x18\x01 \x01(\x0e\x32:.bosdyn.api.ConstrainedManipulationCommand.Feedback.Status\x12\x35\n\x19\x64\x65sired_wrench_odom_frame\x18\x02 \x01(\x0b\x32\x12.bosdyn.api.Wrench\"c\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x12\n\x0eSTATUS_RUNNING\x10\x01\x12\x17\n\x13STATUS_ARM_IS_STUCK\x10\x02\x12\x18\n\x14STATUS_GRASP_IS_LOST\x10\x03\x42\x13\x42\x11\x42\x61sicCommandProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1e\x62osdyn/api/basic_command.proto\x12\nbosdyn.api\x1a\x19\x62osdyn/api/geometry.proto\x1a\x1b\x62osdyn/api/trajectory.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\xca\x01\n\x1aRobotCommandFeedbackStatus\"\xab\x01\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x15\n\x11STATUS_PROCESSING\x10\x01\x12\x1d\n\x19STATUS_COMMAND_OVERRIDDEN\x10\x02\x12\x1c\n\x18STATUS_COMMAND_TIMED_OUT\x10\x03\x12\x17\n\x13STATUS_ROBOT_FROZEN\x10\x04\x12 \n\x1cSTATUS_INCOMPATIBLE_HARDWARE\x10\x05\"\xee\x02\n\x18\x42\x61tteryChangePoseCommand\x1a\x9f\x01\n\x07Request\x12R\n\x0e\x64irection_hint\x18\x01 \x01(\x0e\x32:.bosdyn.api.BatteryChangePoseCommand.Request.DirectionHint\"@\n\rDirectionHint\x12\x10\n\x0cHINT_UNKNOWN\x10\x00\x12\x0e\n\nHINT_RIGHT\x10\x01\x12\r\n\tHINT_LEFT\x10\x02\x1a\xaf\x01\n\x08\x46\x65\x65\x64\x62\x61\x63k\x12\x44\n\x06status\x18\x01 \x01(\x0e\x32\x34.bosdyn.api.BatteryChangePoseCommand.Feedback.Status\"]\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x14\n\x10STATUS_COMPLETED\x10\x01\x12\x16\n\x12STATUS_IN_PROGRESS\x10\x02\x12\x11\n\rSTATUS_FAILED\x10\x03\"\xb4\x01\n\x10SelfRightCommand\x1a\t\n\x07Request\x1a\x94\x01\n\x08\x46\x65\x65\x64\x62\x61\x63k\x12<\n\x06status\x18\x01 \x01(\x0e\x32,.bosdyn.api.SelfRightCommand.Feedback.Status\"J\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x14\n\x10STATUS_COMPLETED\x10\x01\x12\x16\n\x12STATUS_IN_PROGRESS\x10\x02\"$\n\x0bStopCommand\x1a\t\n\x07Request\x1a\n\n\x08\x46\x65\x65\x64\x62\x61\x63k\"&\n\rFreezeCommand\x1a\t\n\x07Request\x1a\n\n\x08\x46\x65\x65\x64\x62\x61\x63k\"\xea\x02\n\x13SafePowerOffCommand\x1a\xb6\x01\n\x07Request\x12K\n\runsafe_action\x18\x01 \x01(\x0e\x32\x34.bosdyn.api.SafePowerOffCommand.Request.UnsafeAction\"^\n\x0cUnsafeAction\x12\x12\n\x0eUNSAFE_UNKNOWN\x10\x00\x12 \n\x1cUNSAFE_MOVE_TO_SAFE_POSITION\x10\x01\x12\x18\n\x14UNSAFE_FORCE_COMMAND\x10\x02\x1a\x99\x01\n\x08\x46\x65\x65\x64\x62\x61\x63k\x12?\n\x06status\x18\x01 \x01(\x0e\x32/.bosdyn.api.SafePowerOffCommand.Feedback.Status\"L\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x16\n\x12STATUS_POWERED_OFF\x10\x01\x12\x16\n\x12STATUS_IN_PROGRESS\x10\x02\"\x83\x04\n\x14SE2TrajectoryCommand\x1a~\n\x07Request\x12,\n\x08\x65nd_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0ese2_frame_name\x18\x03 \x01(\t\x12-\n\ntrajectory\x18\x02 \x01(\x0b\x32\x19.bosdyn.api.SE2Trajectory\x1a\xea\x02\n\x08\x46\x65\x65\x64\x62\x61\x63k\x12@\n\x06status\x18\x01 \x01(\x0e\x32\x30.bosdyn.api.SE2TrajectoryCommand.Feedback.Status\x12Z\n\x14\x62ody_movement_status\x18\x02 \x01(\x0e\x32<.bosdyn.api.SE2TrajectoryCommand.Feedback.BodyMovementStatus\"`\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x12\n\x0eSTATUS_AT_GOAL\x10\x01\x12\x14\n\x10STATUS_NEAR_GOAL\x10\x03\x12\x18\n\x14STATUS_GOING_TO_GOAL\x10\x02\"^\n\x12\x42odyMovementStatus\x12\x17\n\x13\x42ODY_STATUS_UNKNOWN\x10\x00\x12\x16\n\x12\x42ODY_STATUS_MOVING\x10\x01\x12\x17\n\x13\x42ODY_STATUS_SETTLED\x10\x02\"\xd5\x01\n\x12SE2VelocityCommand\x1a\xb2\x01\n\x07Request\x12,\n\x08\x65nd_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0ese2_frame_name\x18\x05 \x01(\t\x12)\n\x08velocity\x18\x02 \x01(\x0b\x32\x17.bosdyn.api.SE2Velocity\x12\x30\n\x0fslew_rate_limit\x18\x04 \x01(\x0b\x32\x17.bosdyn.api.SE2VelocityJ\x04\x08\x03\x10\x04\x1a\n\n\x08\x46\x65\x65\x64\x62\x61\x63k\"\xa9\x01\n\nSitCommand\x1a\t\n\x07Request\x1a\x8f\x01\n\x08\x46\x65\x65\x64\x62\x61\x63k\x12\x36\n\x06status\x18\x02 \x01(\x0e\x32&.bosdyn.api.SitCommand.Feedback.Status\"K\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x15\n\x11STATUS_IS_SITTING\x10\x01\x12\x16\n\x12STATUS_IN_PROGRESS\x10\x02\"\xcc\x02\n\x0cStandCommand\x1a\t\n\x07Request\x1a\xb0\x02\n\x08\x46\x65\x65\x64\x62\x61\x63k\x12\x38\n\x06status\x18\x01 \x01(\x0e\x32(.bosdyn.api.StandCommand.Feedback.Status\x12G\n\x0estanding_state\x18\x02 \x01(\x0e\x32/.bosdyn.api.StandCommand.Feedback.StandingState\"L\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x16\n\x12STATUS_IS_STANDING\x10\x01\x12\x16\n\x12STATUS_IN_PROGRESS\x10\x02\"S\n\rStandingState\x12\x14\n\x10STANDING_UNKNOWN\x10\x00\x12\x17\n\x13STANDING_CONTROLLED\x10\x01\x12\x13\n\x0fSTANDING_FROZEN\x10\x02\"\x9b\x02\n\rStanceCommand\x1a[\n\x07Request\x12,\n\x08\x65nd_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\"\n\x06stance\x18\x02 \x01(\x0b\x32\x12.bosdyn.api.Stance\x1a\xac\x01\n\x08\x46\x65\x65\x64\x62\x61\x63k\x12\x39\n\x06status\x18\x01 \x01(\x0e\x32).bosdyn.api.StanceCommand.Feedback.Status\"e\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x12\n\x0eSTATUS_STANCED\x10\x01\x12\x1a\n\x16STATUS_GOING_TO_STANCE\x10\x02\x12\x17\n\x13STATUS_TOO_FAR_AWAY\x10\x03\"\xb9\x01\n\x06Stance\x12\x16\n\x0ese2_frame_name\x18\x03 \x01(\t\x12=\n\x0e\x66oot_positions\x18\x02 \x03(\x0b\x32%.bosdyn.api.Stance.FootPositionsEntry\x12\x10\n\x08\x61\x63\x63uracy\x18\x04 \x01(\x02\x1a\x46\n\x12\x46ootPositionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1f\n\x05value\x18\x02 \x01(\x0b\x32\x10.bosdyn.api.Vec2:\x02\x38\x01\"w\n\x10\x46ollowArmCommand\x1aW\n\x07Request\x12/\n\x15\x62ody_offset_from_hand\x18\x01 \x01(\x0b\x32\x10.bosdyn.api.Vec3\x12\x1b\n\x0f\x64isable_walking\x18\x02 \x01(\x08\x42\x02\x18\x01\x1a\n\n\x08\x46\x65\x65\x64\x62\x61\x63k\"\xca\x01\n\x0e\x41rmDragCommand\x1a\t\n\x07Request\x1a\xac\x01\n\x08\x46\x65\x65\x64\x62\x61\x63k\x12:\n\x06status\x18\x01 \x01(\x0e\x32*.bosdyn.api.ArmDragCommand.Feedback.Status\"d\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x13\n\x0fSTATUS_DRAGGING\x10\x01\x12\x17\n\x13STATUS_GRASP_FAILED\x10\x02\x12\x18\n\x14STATUS_OTHER_FAILURE\x10\x03\"\xf6\n\n\x1e\x43onstrainedManipulationCommand\x1a\xa4\x08\n\x07Request\x12\x12\n\nframe_name\x18\x01 \x01(\t\x12?\n#init_wrench_direction_in_frame_name\x18\x02 \x01(\x0b\x32\x12.bosdyn.api.Wrench\x12\x1a\n\x10tangential_speed\x18\x03 \x01(\x01H\x00\x12\x1a\n\x10rotational_speed\x18\x04 \x01(\x01H\x00\x12\x31\n\x0b\x66orce_limit\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x32\n\x0ctorque_limit\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12N\n\ttask_type\x18\x07 \x01(\x0e\x32;.bosdyn.api.ConstrainedManipulationCommand.Request.TaskType\x12,\n\x08\x65nd_time\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12;\n\x17\x65nable_robot_locomotion\x18\t \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12T\n\x0c\x63ontrol_mode\x18\n \x01(\x0e\x32>.bosdyn.api.ConstrainedManipulationCommand.Request.ControlMode\x12 \n\x16target_linear_position\x18\x0b \x01(\x01H\x01\x12\x16\n\x0ctarget_angle\x18\x0c \x01(\x01H\x01\x12\x31\n\x0b\x61\x63\x63\x65l_limit\x18\r \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x33\n\x0freset_estimator\x18\x0e \x01(\x0b\x32\x1a.google.protobuf.BoolValue\"\xec\x01\n\x08TaskType\x12\x15\n\x11TASK_TYPE_UNKNOWN\x10\x00\x12%\n!TASK_TYPE_SE3_CIRCLE_FORCE_TORQUE\x10\x01\x12&\n\"TASK_TYPE_R3_CIRCLE_EXTRADOF_FORCE\x10\x02\x12#\n\x1fTASK_TYPE_SE3_ROTATIONAL_TORQUE\x10\x03\x12\x1d\n\x19TASK_TYPE_R3_CIRCLE_FORCE\x10\x04\x12\x1d\n\x19TASK_TYPE_R3_LINEAR_FORCE\x10\x05\x12\x17\n\x13TASK_TYPE_HOLD_POSE\x10\x06\"]\n\x0b\x43ontrolMode\x12\x18\n\x14\x43ONTROL_MODE_UNKNOWN\x10\x00\x12\x19\n\x15\x43ONTROL_MODE_POSITION\x10\x01\x12\x19\n\x15\x43ONTROL_MODE_VELOCITY\x10\x02\x42\x0c\n\ntask_speedB\x16\n\x14task_target_position\x1a\xac\x02\n\x08\x46\x65\x65\x64\x62\x61\x63k\x12J\n\x06status\x18\x01 \x01(\x0e\x32:.bosdyn.api.ConstrainedManipulationCommand.Feedback.Status\x12\x35\n\x19\x64\x65sired_wrench_odom_frame\x18\x02 \x01(\x0b\x32\x12.bosdyn.api.Wrench\x12\x38\n\x14\x65stimation_activated\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\"c\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x12\n\x0eSTATUS_RUNNING\x10\x01\x12\x17\n\x13STATUS_ARM_IS_STUCK\x10\x02\x12\x18\n\x14STATUS_GRASP_IS_LOST\x10\x03\x42\x13\x42\x11\x42\x61sicCommandProtob\x06proto3')
 
 
 
 _ROBOTCOMMANDFEEDBACKSTATUS = DESCRIPTOR.message_types_by_name['RobotCommandFeedbackStatus']
 _BATTERYCHANGEPOSECOMMAND = DESCRIPTOR.message_types_by_name['BatteryChangePoseCommand']
 _BATTERYCHANGEPOSECOMMAND_REQUEST = _BATTERYCHANGEPOSECOMMAND.nested_types_by_name['Request']
 _BATTERYCHANGEPOSECOMMAND_FEEDBACK = _BATTERYCHANGEPOSECOMMAND.nested_types_by_name['Feedback']
@@ -74,14 +74,15 @@
 _SE2TRAJECTORYCOMMAND_FEEDBACK_BODYMOVEMENTSTATUS = _SE2TRAJECTORYCOMMAND_FEEDBACK.enum_types_by_name['BodyMovementStatus']
 _SITCOMMAND_FEEDBACK_STATUS = _SITCOMMAND_FEEDBACK.enum_types_by_name['Status']
 _STANDCOMMAND_FEEDBACK_STATUS = _STANDCOMMAND_FEEDBACK.enum_types_by_name['Status']
 _STANDCOMMAND_FEEDBACK_STANDINGSTATE = _STANDCOMMAND_FEEDBACK.enum_types_by_name['StandingState']
 _STANCECOMMAND_FEEDBACK_STATUS = _STANCECOMMAND_FEEDBACK.enum_types_by_name['Status']
 _ARMDRAGCOMMAND_FEEDBACK_STATUS = _ARMDRAGCOMMAND_FEEDBACK.enum_types_by_name['Status']
 _CONSTRAINEDMANIPULATIONCOMMAND_REQUEST_TASKTYPE = _CONSTRAINEDMANIPULATIONCOMMAND_REQUEST.enum_types_by_name['TaskType']
+_CONSTRAINEDMANIPULATIONCOMMAND_REQUEST_CONTROLMODE = _CONSTRAINEDMANIPULATIONCOMMAND_REQUEST.enum_types_by_name['ControlMode']
 _CONSTRAINEDMANIPULATIONCOMMAND_FEEDBACK_STATUS = _CONSTRAINEDMANIPULATIONCOMMAND_FEEDBACK.enum_types_by_name['Status']
 RobotCommandFeedbackStatus = _reflection.GeneratedProtocolMessageType('RobotCommandFeedbackStatus', (_message.Message,), {
   'DESCRIPTOR' : _ROBOTCOMMANDFEEDBACKSTATUS,
   '__module__' : 'bosdyn.api.basic_command_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.RobotCommandFeedbackStatus)
   })
 _sym_db.RegisterMessage(RobotCommandFeedbackStatus)
@@ -509,17 +510,19 @@
   _ARMDRAGCOMMAND_REQUEST._serialized_start=402
   _ARMDRAGCOMMAND_REQUEST._serialized_end=411
   _ARMDRAGCOMMAND_FEEDBACK._serialized_start=3234
   _ARMDRAGCOMMAND_FEEDBACK._serialized_end=3406
   _ARMDRAGCOMMAND_FEEDBACK_STATUS._serialized_start=3306
   _ARMDRAGCOMMAND_FEEDBACK_STATUS._serialized_end=3406
   _CONSTRAINEDMANIPULATIONCOMMAND._serialized_start=3409
-  _CONSTRAINEDMANIPULATIONCOMMAND._serialized_end=4382
+  _CONSTRAINEDMANIPULATIONCOMMAND._serialized_end=4807
   _CONSTRAINEDMANIPULATIONCOMMAND_REQUEST._serialized_start=3444
-  _CONSTRAINEDMANIPULATIONCOMMAND_REQUEST._serialized_end=4137
-  _CONSTRAINEDMANIPULATIONCOMMAND_REQUEST_TASKTYPE._serialized_start=3887
-  _CONSTRAINEDMANIPULATIONCOMMAND_REQUEST_TASKTYPE._serialized_end=4123
-  _CONSTRAINEDMANIPULATIONCOMMAND_FEEDBACK._serialized_start=4140
-  _CONSTRAINEDMANIPULATIONCOMMAND_FEEDBACK._serialized_end=4382
-  _CONSTRAINEDMANIPULATIONCOMMAND_FEEDBACK_STATUS._serialized_start=4283
-  _CONSTRAINEDMANIPULATIONCOMMAND_FEEDBACK_STATUS._serialized_end=4382
+  _CONSTRAINEDMANIPULATIONCOMMAND_REQUEST._serialized_end=4504
+  _CONSTRAINEDMANIPULATIONCOMMAND_REQUEST_TASKTYPE._serialized_start=4135
+  _CONSTRAINEDMANIPULATIONCOMMAND_REQUEST_TASKTYPE._serialized_end=4371
+  _CONSTRAINEDMANIPULATIONCOMMAND_REQUEST_CONTROLMODE._serialized_start=4373
+  _CONSTRAINEDMANIPULATIONCOMMAND_REQUEST_CONTROLMODE._serialized_end=4466
+  _CONSTRAINEDMANIPULATIONCOMMAND_FEEDBACK._serialized_start=4507
+  _CONSTRAINEDMANIPULATIONCOMMAND_FEEDBACK._serialized_end=4807
+  _CONSTRAINEDMANIPULATIONCOMMAND_FEEDBACK_STATUS._serialized_start=4708
+  _CONSTRAINEDMANIPULATIONCOMMAND_FEEDBACK_STATUS._serialized_end=4807
 # @@protoc_insertion_point(module_scope)
```

## bosdyn/api/data_acquisition_pb2.py

```diff
@@ -12,21 +12,22 @@
 _sym_db = _symbol_database.Default()
 
 
 from bosdyn.api import alerts_pb2 as bosdyn_dot_api_dot_alerts__pb2
 from bosdyn.api import header_pb2 as bosdyn_dot_api_dot_header__pb2
 from bosdyn.api import image_pb2 as bosdyn_dot_api_dot_image__pb2
 from bosdyn.api import network_compute_bridge_pb2 as bosdyn_dot_api_dot_network__compute__bridge__pb2
+from bosdyn.api import service_customization_pb2 as bosdyn_dot_api_dot_service__customization__pb2
 from google.protobuf import any_pb2 as google_dot_protobuf_dot_any__pb2
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!bosdyn/api/data_acquisition.proto\x12\nbosdyn.api\x1a\x17\x62osdyn/api/alerts.proto\x1a\x17\x62osdyn/api/header.proto\x1a\x16\x62osdyn/api/image.proto\x1a\'bosdyn/api/network_compute_bridge.proto\x1a\x19google/protobuf/any.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"j\n\x19\x44\x61taAcquisitionCapability\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x14\n\x0c\x63hannel_name\x18\x03 \x01(\t\x12\x14\n\x0cservice_name\x18\x04 \x01(\t\"~\n\x1aImageAcquisitionCapability\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x1a\n\x12image_source_names\x18\x02 \x03(\t\x12.\n\rimage_sources\x18\x03 \x03(\x0b\x32\x17.bosdyn.api.ImageSource\"\xa3\x01\n\x18NetworkComputeCapability\x12\x44\n\rserver_config\x18\x01 \x01(\x0b\x32-.bosdyn.api.NetworkComputeServerConfiguration\x12\x18\n\x10\x61vailable_models\x18\x02 \x03(\t\x12\'\n\x06labels\x18\x06 \x03(\x0b\x32\x17.bosdyn.api.ModelLabels\"\xde\x01\n\x19\x41\x63quisitionCapabilityList\x12;\n\x0c\x64\x61ta_sources\x18\x01 \x03(\x0b\x32%.bosdyn.api.DataAcquisitionCapability\x12=\n\rimage_sources\x18\x03 \x03(\x0b\x32&.bosdyn.api.ImageAcquisitionCapability\x12\x45\n\x17network_compute_sources\x18\x05 \x03(\x0b\x32$.bosdyn.api.NetworkComputeCapability\"i\n\x0f\x43\x61ptureActionId\x12\x13\n\x0b\x61\x63tion_name\x18\x01 \x01(\t\x12\x12\n\ngroup_name\x18\x02 \x01(\t\x12-\n\ttimestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"d\n\x0e\x44\x61taIdentifier\x12.\n\taction_id\x18\x01 \x01(\x0b\x32\x1b.bosdyn.api.CaptureActionId\x12\x0f\n\x07\x63hannel\x18\x02 \x01(\t\x12\x11\n\tdata_name\x18\x03 \x01(\t\"1\n\x08Metadata\x12%\n\x04\x64\x61ta\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\"n\n\x12\x41ssociatedMetadata\x12\x30\n\x0creference_id\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.DataIdentifier\x12&\n\x08metadata\x18\x02 \x01(\x0b\x32\x14.bosdyn.api.Metadata\"r\n\x13\x41ssociatedAlertData\x12\x30\n\x0creference_id\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.DataIdentifier\x12)\n\nalert_data\x18\x02 \x01(\x0b\x32\x15.bosdyn.api.AlertData\"\xaf\x01\n\x12ImageSourceCapture\x12\x15\n\rimage_service\x18\x01 \x01(\t\x12/\n\rimage_request\x18\x04 \x01(\x0b\x32\x18.bosdyn.api.ImageRequest\x12\x18\n\x0cimage_source\x18\x02 \x01(\tB\x02\x18\x01\x12\x37\n\x0cpixel_format\x18\x03 \x01(\x0e\x32\x1d.bosdyn.api.Image.PixelFormatB\x02\x18\x01\"\x1b\n\x0b\x44\x61taCapture\x12\x0c\n\x04name\x18\x01 \x01(\t\"\x96\x01\n\x15NetworkComputeCapture\x12\x37\n\ninput_data\x18\x01 \x01(\x0b\x32#.bosdyn.api.NetworkComputeInputData\x12\x44\n\rserver_config\x18\x02 \x01(\x0b\x32-.bosdyn.api.NetworkComputeServerConfiguration\"\xc5\x01\n\x16\x41\x63quisitionRequestList\x12\x36\n\x0eimage_captures\x18\x01 \x03(\x0b\x32\x1e.bosdyn.api.ImageSourceCapture\x12.\n\rdata_captures\x18\x02 \x03(\x0b\x32\x17.bosdyn.api.DataCapture\x12\x43\n\x18network_compute_captures\x18\x04 \x03(\x0b\x32!.bosdyn.api.NetworkComputeCapture\"y\n\tDataError\x12+\n\x07\x64\x61ta_id\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.DataIdentifier\x12\x15\n\rerror_message\x18\x02 \x01(\t\x12(\n\nerror_data\x18\x03 \x01(\x0b\x32\x14.google.protobuf.Any\"\xe6\x01\n\x12PluginServiceError\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x37\n\x05\x65rror\x18\x02 \x01(\x0e\x32(.bosdyn.api.PluginServiceError.ErrorCode\x12\x0f\n\x07message\x18\x03 \x01(\t\"p\n\tErrorCode\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x18\n\x14STATUS_REQUEST_ERROR\x10\x01\x12\x1a\n\x16STATUS_GETSTATUS_ERROR\x10\x02\x12\x19\n\x15STATUS_INTERNAL_ERROR\x10\x03\"\xa8\x02\n\x13NetworkComputeError\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x38\n\x05\x65rror\x18\x02 \x01(\x0e\x32).bosdyn.api.NetworkComputeError.ErrorCode\x12@\n\x16network_compute_status\x18\x03 \x01(\x0e\x32 .bosdyn.api.NetworkComputeStatus\x12\x0f\n\x07message\x18\x04 \x01(\t\"n\n\tErrorCode\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x18\n\x14STATUS_REQUEST_ERROR\x10\x01\x12\x18\n\x14STATUS_NETWORK_ERROR\x10\x02\x12\x19\n\x15STATUS_INTERNAL_ERROR\x10\x03\"\x89\x02\n\x12\x41\x63quireDataRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12.\n\taction_id\x18\x02 \x01(\x0b\x32\x1b.bosdyn.api.CaptureActionId\x12&\n\x08metadata\x18\x03 \x01(\x0b\x32\x14.bosdyn.api.Metadata\x12@\n\x14\x61\x63quisition_requests\x18\x04 \x01(\x0b\x32\".bosdyn.api.AcquisitionRequestList\x12.\n\x0bmin_timeout\x18\x05 \x01(\x0b\x32\x19.google.protobuf.Duration\"\xdb\x01\n\x13\x41\x63quireDataResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x36\n\x06status\x18\x02 \x01(\x0e\x32&.bosdyn.api.AcquireDataResponse.Status\x12\x12\n\nrequest_id\x18\x03 \x01(\r\"L\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1f\n\x1bSTATUS_UNKNOWN_CAPTURE_TYPE\x10\x02\"\x8c\x02\n\x18\x41\x63quirePluginDataRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12+\n\x07\x64\x61ta_id\x18\x02 \x03(\x0b\x32\x1a.bosdyn.api.DataIdentifier\x12&\n\x08metadata\x18\x03 \x01(\x0b\x32\x14.bosdyn.api.Metadata\x12.\n\taction_id\x18\x04 \x01(\x0b\x32\x1b.bosdyn.api.CaptureActionId\x12@\n\x14\x61\x63quisition_requests\x18\x05 \x01(\x0b\x32\".bosdyn.api.AcquisitionRequestList\"\x9d\x02\n\x19\x41\x63quirePluginDataResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12<\n\x06status\x18\x02 \x01(\x0e\x32,.bosdyn.api.AcquirePluginDataResponse.Status\x12\x12\n\nrequest_id\x18\x03 \x01(\r\x12\x34\n\x10timeout_deadline\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"L\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1f\n\x1bSTATUS_UNKNOWN_CAPTURE_TYPE\x10\x02\"Q\n\x10GetStatusRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x12\n\nrequest_id\x18\x02 \x01(\r\"\xfb\x04\n\x11GetStatusResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x34\n\x06status\x18\x02 \x01(\x0e\x32$.bosdyn.api.GetStatusResponse.Status\x12.\n\ndata_saved\x18\x03 \x03(\x0b\x32\x1a.bosdyn.api.DataIdentifier\x12*\n\x0b\x64\x61ta_errors\x18\t \x03(\x0b\x32\x15.bosdyn.api.DataError\x12\x36\n\x0eservice_errors\x18\n \x03(\x0b\x32\x1e.bosdyn.api.PluginServiceError\x12?\n\x16network_compute_errors\x18\x0b \x03(\x0b\x32\x1f.bosdyn.api.NetworkComputeError\"\xae\x02\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x14\n\x10STATUS_ACQUIRING\x10\x01\x12\x11\n\rSTATUS_SAVING\x10\x02\x12\x13\n\x0fSTATUS_COMPLETE\x10\x03\x12\x1d\n\x19STATUS_CANCEL_IN_PROGRESS\x10\x04\x12 \n\x1cSTATUS_ACQUISITION_CANCELLED\x10\x05\x12\x15\n\x11STATUS_DATA_ERROR\x10\n\x12\x13\n\x0fSTATUS_TIMEDOUT\x10\x0b\x12\x19\n\x15STATUS_INTERNAL_ERROR\x10\x0c\x12$\n STATUS_CANCEL_ACQUISITION_FAILED\x10\x1e\x12$\n STATUS_REQUEST_ID_DOES_NOT_EXIST\x10\x14\"B\n\x15GetServiceInfoRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"\x81\x01\n\x16GetServiceInfoResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12;\n\x0c\x63\x61pabilities\x18\x02 \x01(\x0b\x32%.bosdyn.api.AcquisitionCapabilityList\"Y\n\x18\x43\x61ncelAcquisitionRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x12\n\nrequest_id\x18\x02 \x01(\r\"\xf5\x01\n\x19\x43\x61ncelAcquisitionResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12<\n\x06status\x18\x02 \x01(\x0e\x32,.bosdyn.api.CancelAcquisitionResponse.Status\"n\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1b\n\x17STATUS_FAILED_TO_CANCEL\x10\x02\x12$\n STATUS_REQUEST_ID_DOES_NOT_EXIST\x10\x03\x42\x16\x42\x14\x44\x61taAcquisitionProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!bosdyn/api/data_acquisition.proto\x12\nbosdyn.api\x1a\x17\x62osdyn/api/alerts.proto\x1a\x17\x62osdyn/api/header.proto\x1a\x16\x62osdyn/api/image.proto\x1a\'bosdyn/api/network_compute_bridge.proto\x1a&bosdyn/api/service_customization.proto\x1a\x19google/protobuf/any.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\x9d\x01\n\x19\x44\x61taAcquisitionCapability\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x14\n\x0c\x63hannel_name\x18\x03 \x01(\t\x12\x14\n\x0cservice_name\x18\x04 \x01(\t\x12\x31\n\rcustom_params\x18\x05 \x01(\x0b\x32\x1a.bosdyn.api.DictParam.Spec\"\x82\x01\n\x1aImageAcquisitionCapability\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x1e\n\x12image_source_names\x18\x02 \x03(\tB\x02\x18\x01\x12.\n\rimage_sources\x18\x03 \x03(\x0b\x32\x17.bosdyn.api.ImageSource\"\xd8\x01\n\x18NetworkComputeCapability\x12\x44\n\rserver_config\x18\x01 \x01(\x0b\x32-.bosdyn.api.NetworkComputeServerConfiguration\x12\x1c\n\x10\x61vailable_models\x18\x02 \x03(\tB\x02\x18\x01\x12+\n\x06labels\x18\x06 \x03(\x0b\x32\x17.bosdyn.api.ModelLabelsB\x02\x18\x01\x12+\n\x06models\x18\x03 \x01(\x0b\x32\x1b.bosdyn.api.AvailableModels\"\xde\x01\n\x19\x41\x63quisitionCapabilityList\x12;\n\x0c\x64\x61ta_sources\x18\x01 \x03(\x0b\x32%.bosdyn.api.DataAcquisitionCapability\x12=\n\rimage_sources\x18\x03 \x03(\x0b\x32&.bosdyn.api.ImageAcquisitionCapability\x12\x45\n\x17network_compute_sources\x18\x05 \x03(\x0b\x32$.bosdyn.api.NetworkComputeCapability\"o\n\x0f\x43\x61ptureActionId\x12\x13\n\x0b\x61\x63tion_name\x18\x01 \x01(\t\x12\x12\n\ngroup_name\x18\x02 \x01(\t\x12-\n\ttimestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampJ\x04\x08\x04\x10\x05\"p\n\x0e\x44\x61taIdentifier\x12.\n\taction_id\x18\x01 \x01(\x0b\x32\x1b.bosdyn.api.CaptureActionId\x12\x0f\n\x07\x63hannel\x18\x02 \x01(\t\x12\x11\n\tdata_name\x18\x03 \x01(\t\x12\n\n\x02id\x18\x04 \x01(\x04\"1\n\x08Metadata\x12%\n\x04\x64\x61ta\x18\x01 \x01(\x0b\x32\x17.google.protobuf.Struct\"n\n\x12\x41ssociatedMetadata\x12\x30\n\x0creference_id\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.DataIdentifier\x12&\n\x08metadata\x18\x02 \x01(\x0b\x32\x14.bosdyn.api.Metadata\"r\n\x13\x41ssociatedAlertData\x12\x30\n\x0creference_id\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.DataIdentifier\x12)\n\nalert_data\x18\x02 \x01(\x0b\x32\x15.bosdyn.api.AlertData\"\xaf\x01\n\x12ImageSourceCapture\x12\x15\n\rimage_service\x18\x01 \x01(\t\x12/\n\rimage_request\x18\x04 \x01(\x0b\x32\x18.bosdyn.api.ImageRequest\x12\x18\n\x0cimage_source\x18\x02 \x01(\tB\x02\x18\x01\x12\x37\n\x0cpixel_format\x18\x03 \x01(\x0e\x32\x1d.bosdyn.api.Image.PixelFormatB\x02\x18\x01\"I\n\x0b\x44\x61taCapture\x12\x0c\n\x04name\x18\x01 \x01(\t\x12,\n\rcustom_params\x18\t \x01(\x0b\x32\x15.bosdyn.api.DictParam\"\xed\x01\n\x15NetworkComputeCapture\x12=\n\ninput_data\x18\x01 \x01(\x0b\x32#.bosdyn.api.NetworkComputeInputDataB\x02\x18\x01H\x00\x12\x46\n\x11input_data_bridge\x18\x03 \x01(\x0b\x32).bosdyn.api.NetworkComputeInputDataBridgeH\x00\x12\x44\n\rserver_config\x18\x02 \x01(\x0b\x32-.bosdyn.api.NetworkComputeServerConfigurationB\x07\n\x05input\"\xc5\x01\n\x16\x41\x63quisitionRequestList\x12\x36\n\x0eimage_captures\x18\x01 \x03(\x0b\x32\x1e.bosdyn.api.ImageSourceCapture\x12.\n\rdata_captures\x18\x02 \x03(\x0b\x32\x17.bosdyn.api.DataCapture\x12\x43\n\x18network_compute_captures\x18\x04 \x03(\x0b\x32!.bosdyn.api.NetworkComputeCapture\"y\n\tDataError\x12+\n\x07\x64\x61ta_id\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.DataIdentifier\x12\x15\n\rerror_message\x18\x02 \x01(\t\x12(\n\nerror_data\x18\x03 \x01(\x0b\x32\x14.google.protobuf.Any\"\xe6\x01\n\x12PluginServiceError\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x37\n\x05\x65rror\x18\x02 \x01(\x0e\x32(.bosdyn.api.PluginServiceError.ErrorCode\x12\x0f\n\x07message\x18\x03 \x01(\t\"p\n\tErrorCode\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x18\n\x14STATUS_REQUEST_ERROR\x10\x01\x12\x1a\n\x16STATUS_GETSTATUS_ERROR\x10\x02\x12\x19\n\x15STATUS_INTERNAL_ERROR\x10\x03\"\xa8\x02\n\x13NetworkComputeError\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x38\n\x05\x65rror\x18\x02 \x01(\x0e\x32).bosdyn.api.NetworkComputeError.ErrorCode\x12@\n\x16network_compute_status\x18\x03 \x01(\x0e\x32 .bosdyn.api.NetworkComputeStatus\x12\x0f\n\x07message\x18\x04 \x01(\t\"n\n\tErrorCode\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x18\n\x14STATUS_REQUEST_ERROR\x10\x01\x12\x18\n\x14STATUS_NETWORK_ERROR\x10\x02\x12\x19\n\x15STATUS_INTERNAL_ERROR\x10\x03\"\x89\x02\n\x12\x41\x63quireDataRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12.\n\taction_id\x18\x02 \x01(\x0b\x32\x1b.bosdyn.api.CaptureActionId\x12&\n\x08metadata\x18\x03 \x01(\x0b\x32\x14.bosdyn.api.Metadata\x12@\n\x14\x61\x63quisition_requests\x18\x04 \x01(\x0b\x32\".bosdyn.api.AcquisitionRequestList\x12.\n\x0bmin_timeout\x18\x05 \x01(\x0b\x32\x19.google.protobuf.Duration\"\xdb\x01\n\x13\x41\x63quireDataResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x36\n\x06status\x18\x02 \x01(\x0e\x32&.bosdyn.api.AcquireDataResponse.Status\x12\x12\n\nrequest_id\x18\x03 \x01(\r\"L\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1f\n\x1bSTATUS_UNKNOWN_CAPTURE_TYPE\x10\x02\"\x8c\x02\n\x18\x41\x63quirePluginDataRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12+\n\x07\x64\x61ta_id\x18\x02 \x03(\x0b\x32\x1a.bosdyn.api.DataIdentifier\x12&\n\x08metadata\x18\x03 \x01(\x0b\x32\x14.bosdyn.api.Metadata\x12.\n\taction_id\x18\x04 \x01(\x0b\x32\x1b.bosdyn.api.CaptureActionId\x12@\n\x14\x61\x63quisition_requests\x18\x05 \x01(\x0b\x32\".bosdyn.api.AcquisitionRequestList\"\xf7\x02\n\x19\x41\x63quirePluginDataResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12<\n\x06status\x18\x02 \x01(\x0e\x32,.bosdyn.api.AcquirePluginDataResponse.Status\x12\x12\n\nrequest_id\x18\x03 \x01(\r\x12\x34\n\x10timeout_deadline\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x38\n\x12\x63ustom_param_error\x18\x06 \x01(\x0b\x32\x1c.bosdyn.api.CustomParamError\"l\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1f\n\x1bSTATUS_UNKNOWN_CAPTURE_TYPE\x10\x02\x12\x1e\n\x1aSTATUS_CUSTOM_PARAMS_ERROR\x10\x03\"Q\n\x10GetStatusRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x12\n\nrequest_id\x18\x02 \x01(\r\"\xfb\x04\n\x11GetStatusResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x34\n\x06status\x18\x02 \x01(\x0e\x32$.bosdyn.api.GetStatusResponse.Status\x12.\n\ndata_saved\x18\x03 \x03(\x0b\x32\x1a.bosdyn.api.DataIdentifier\x12*\n\x0b\x64\x61ta_errors\x18\t \x03(\x0b\x32\x15.bosdyn.api.DataError\x12\x36\n\x0eservice_errors\x18\n \x03(\x0b\x32\x1e.bosdyn.api.PluginServiceError\x12?\n\x16network_compute_errors\x18\x0b \x03(\x0b\x32\x1f.bosdyn.api.NetworkComputeError\"\xae\x02\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x14\n\x10STATUS_ACQUIRING\x10\x01\x12\x11\n\rSTATUS_SAVING\x10\x02\x12\x13\n\x0fSTATUS_COMPLETE\x10\x03\x12\x1d\n\x19STATUS_CANCEL_IN_PROGRESS\x10\x04\x12 \n\x1cSTATUS_ACQUISITION_CANCELLED\x10\x05\x12\x15\n\x11STATUS_DATA_ERROR\x10\n\x12\x13\n\x0fSTATUS_TIMEDOUT\x10\x0b\x12\x19\n\x15STATUS_INTERNAL_ERROR\x10\x0c\x12$\n STATUS_CANCEL_ACQUISITION_FAILED\x10\x1e\x12$\n STATUS_REQUEST_ID_DOES_NOT_EXIST\x10\x14\"B\n\x15GetServiceInfoRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"\x81\x01\n\x16GetServiceInfoResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12;\n\x0c\x63\x61pabilities\x18\x02 \x01(\x0b\x32%.bosdyn.api.AcquisitionCapabilityList\"Y\n\x18\x43\x61ncelAcquisitionRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x12\n\nrequest_id\x18\x02 \x01(\r\"\xf5\x01\n\x19\x43\x61ncelAcquisitionResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12<\n\x06status\x18\x02 \x01(\x0e\x32,.bosdyn.api.CancelAcquisitionResponse.Status\"n\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1b\n\x17STATUS_FAILED_TO_CANCEL\x10\x02\x12$\n STATUS_REQUEST_ID_DOES_NOT_EXIST\x10\x03\x42\x16\x42\x14\x44\x61taAcquisitionProtob\x06proto3')
 
 
 
 _DATAACQUISITIONCAPABILITY = DESCRIPTOR.message_types_by_name['DataAcquisitionCapability']
 _IMAGEACQUISITIONCAPABILITY = DESCRIPTOR.message_types_by_name['ImageAcquisitionCapability']
 _NETWORKCOMPUTECAPABILITY = DESCRIPTOR.message_types_by_name['NetworkComputeCapability']
 _ACQUISITIONCAPABILITYLIST = DESCRIPTOR.message_types_by_name['AcquisitionCapabilityList']
@@ -240,76 +241,84 @@
   })
 _sym_db.RegisterMessage(CancelAcquisitionResponse)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'B\024DataAcquisitionProto'
+  _IMAGEACQUISITIONCAPABILITY.fields_by_name['image_source_names']._options = None
+  _IMAGEACQUISITIONCAPABILITY.fields_by_name['image_source_names']._serialized_options = b'\030\001'
+  _NETWORKCOMPUTECAPABILITY.fields_by_name['available_models']._options = None
+  _NETWORKCOMPUTECAPABILITY.fields_by_name['available_models']._serialized_options = b'\030\001'
+  _NETWORKCOMPUTECAPABILITY.fields_by_name['labels']._options = None
+  _NETWORKCOMPUTECAPABILITY.fields_by_name['labels']._serialized_options = b'\030\001'
   _IMAGESOURCECAPTURE.fields_by_name['image_source']._options = None
   _IMAGESOURCECAPTURE.fields_by_name['image_source']._serialized_options = b'\030\001'
   _IMAGESOURCECAPTURE.fields_by_name['pixel_format']._options = None
   _IMAGESOURCECAPTURE.fields_by_name['pixel_format']._serialized_options = b'\030\001'
-  _DATAACQUISITIONCAPABILITY._serialized_start=286
-  _DATAACQUISITIONCAPABILITY._serialized_end=392
-  _IMAGEACQUISITIONCAPABILITY._serialized_start=394
-  _IMAGEACQUISITIONCAPABILITY._serialized_end=520
-  _NETWORKCOMPUTECAPABILITY._serialized_start=523
-  _NETWORKCOMPUTECAPABILITY._serialized_end=686
-  _ACQUISITIONCAPABILITYLIST._serialized_start=689
-  _ACQUISITIONCAPABILITYLIST._serialized_end=911
-  _CAPTUREACTIONID._serialized_start=913
-  _CAPTUREACTIONID._serialized_end=1018
-  _DATAIDENTIFIER._serialized_start=1020
-  _DATAIDENTIFIER._serialized_end=1120
-  _METADATA._serialized_start=1122
-  _METADATA._serialized_end=1171
-  _ASSOCIATEDMETADATA._serialized_start=1173
-  _ASSOCIATEDMETADATA._serialized_end=1283
-  _ASSOCIATEDALERTDATA._serialized_start=1285
-  _ASSOCIATEDALERTDATA._serialized_end=1399
-  _IMAGESOURCECAPTURE._serialized_start=1402
-  _IMAGESOURCECAPTURE._serialized_end=1577
-  _DATACAPTURE._serialized_start=1579
-  _DATACAPTURE._serialized_end=1606
-  _NETWORKCOMPUTECAPTURE._serialized_start=1609
-  _NETWORKCOMPUTECAPTURE._serialized_end=1759
-  _ACQUISITIONREQUESTLIST._serialized_start=1762
-  _ACQUISITIONREQUESTLIST._serialized_end=1959
-  _DATAERROR._serialized_start=1961
-  _DATAERROR._serialized_end=2082
-  _PLUGINSERVICEERROR._serialized_start=2085
-  _PLUGINSERVICEERROR._serialized_end=2315
-  _PLUGINSERVICEERROR_ERRORCODE._serialized_start=2203
-  _PLUGINSERVICEERROR_ERRORCODE._serialized_end=2315
-  _NETWORKCOMPUTEERROR._serialized_start=2318
-  _NETWORKCOMPUTEERROR._serialized_end=2614
-  _NETWORKCOMPUTEERROR_ERRORCODE._serialized_start=2504
-  _NETWORKCOMPUTEERROR_ERRORCODE._serialized_end=2614
-  _ACQUIREDATAREQUEST._serialized_start=2617
-  _ACQUIREDATAREQUEST._serialized_end=2882
-  _ACQUIREDATARESPONSE._serialized_start=2885
-  _ACQUIREDATARESPONSE._serialized_end=3104
-  _ACQUIREDATARESPONSE_STATUS._serialized_start=3028
-  _ACQUIREDATARESPONSE_STATUS._serialized_end=3104
-  _ACQUIREPLUGINDATAREQUEST._serialized_start=3107
-  _ACQUIREPLUGINDATAREQUEST._serialized_end=3375
-  _ACQUIREPLUGINDATARESPONSE._serialized_start=3378
-  _ACQUIREPLUGINDATARESPONSE._serialized_end=3663
-  _ACQUIREPLUGINDATARESPONSE_STATUS._serialized_start=3028
-  _ACQUIREPLUGINDATARESPONSE_STATUS._serialized_end=3104
-  _GETSTATUSREQUEST._serialized_start=3665
-  _GETSTATUSREQUEST._serialized_end=3746
-  _GETSTATUSRESPONSE._serialized_start=3749
-  _GETSTATUSRESPONSE._serialized_end=4384
-  _GETSTATUSRESPONSE_STATUS._serialized_start=4082
-  _GETSTATUSRESPONSE_STATUS._serialized_end=4384
-  _GETSERVICEINFOREQUEST._serialized_start=4386
-  _GETSERVICEINFOREQUEST._serialized_end=4452
-  _GETSERVICEINFORESPONSE._serialized_start=4455
-  _GETSERVICEINFORESPONSE._serialized_end=4584
-  _CANCELACQUISITIONREQUEST._serialized_start=4586
-  _CANCELACQUISITIONREQUEST._serialized_end=4675
-  _CANCELACQUISITIONRESPONSE._serialized_start=4678
-  _CANCELACQUISITIONRESPONSE._serialized_end=4923
-  _CANCELACQUISITIONRESPONSE_STATUS._serialized_start=4813
-  _CANCELACQUISITIONRESPONSE_STATUS._serialized_end=4923
+  _NETWORKCOMPUTECAPTURE.fields_by_name['input_data']._options = None
+  _NETWORKCOMPUTECAPTURE.fields_by_name['input_data']._serialized_options = b'\030\001'
+  _DATAACQUISITIONCAPABILITY._serialized_start=327
+  _DATAACQUISITIONCAPABILITY._serialized_end=484
+  _IMAGEACQUISITIONCAPABILITY._serialized_start=487
+  _IMAGEACQUISITIONCAPABILITY._serialized_end=617
+  _NETWORKCOMPUTECAPABILITY._serialized_start=620
+  _NETWORKCOMPUTECAPABILITY._serialized_end=836
+  _ACQUISITIONCAPABILITYLIST._serialized_start=839
+  _ACQUISITIONCAPABILITYLIST._serialized_end=1061
+  _CAPTUREACTIONID._serialized_start=1063
+  _CAPTUREACTIONID._serialized_end=1174
+  _DATAIDENTIFIER._serialized_start=1176
+  _DATAIDENTIFIER._serialized_end=1288
+  _METADATA._serialized_start=1290
+  _METADATA._serialized_end=1339
+  _ASSOCIATEDMETADATA._serialized_start=1341
+  _ASSOCIATEDMETADATA._serialized_end=1451
+  _ASSOCIATEDALERTDATA._serialized_start=1453
+  _ASSOCIATEDALERTDATA._serialized_end=1567
+  _IMAGESOURCECAPTURE._serialized_start=1570
+  _IMAGESOURCECAPTURE._serialized_end=1745
+  _DATACAPTURE._serialized_start=1747
+  _DATACAPTURE._serialized_end=1820
+  _NETWORKCOMPUTECAPTURE._serialized_start=1823
+  _NETWORKCOMPUTECAPTURE._serialized_end=2060
+  _ACQUISITIONREQUESTLIST._serialized_start=2063
+  _ACQUISITIONREQUESTLIST._serialized_end=2260
+  _DATAERROR._serialized_start=2262
+  _DATAERROR._serialized_end=2383
+  _PLUGINSERVICEERROR._serialized_start=2386
+  _PLUGINSERVICEERROR._serialized_end=2616
+  _PLUGINSERVICEERROR_ERRORCODE._serialized_start=2504
+  _PLUGINSERVICEERROR_ERRORCODE._serialized_end=2616
+  _NETWORKCOMPUTEERROR._serialized_start=2619
+  _NETWORKCOMPUTEERROR._serialized_end=2915
+  _NETWORKCOMPUTEERROR_ERRORCODE._serialized_start=2805
+  _NETWORKCOMPUTEERROR_ERRORCODE._serialized_end=2915
+  _ACQUIREDATAREQUEST._serialized_start=2918
+  _ACQUIREDATAREQUEST._serialized_end=3183
+  _ACQUIREDATARESPONSE._serialized_start=3186
+  _ACQUIREDATARESPONSE._serialized_end=3405
+  _ACQUIREDATARESPONSE_STATUS._serialized_start=3329
+  _ACQUIREDATARESPONSE_STATUS._serialized_end=3405
+  _ACQUIREPLUGINDATAREQUEST._serialized_start=3408
+  _ACQUIREPLUGINDATAREQUEST._serialized_end=3676
+  _ACQUIREPLUGINDATARESPONSE._serialized_start=3679
+  _ACQUIREPLUGINDATARESPONSE._serialized_end=4054
+  _ACQUIREPLUGINDATARESPONSE_STATUS._serialized_start=3946
+  _ACQUIREPLUGINDATARESPONSE_STATUS._serialized_end=4054
+  _GETSTATUSREQUEST._serialized_start=4056
+  _GETSTATUSREQUEST._serialized_end=4137
+  _GETSTATUSRESPONSE._serialized_start=4140
+  _GETSTATUSRESPONSE._serialized_end=4775
+  _GETSTATUSRESPONSE_STATUS._serialized_start=4473
+  _GETSTATUSRESPONSE_STATUS._serialized_end=4775
+  _GETSERVICEINFOREQUEST._serialized_start=4777
+  _GETSERVICEINFOREQUEST._serialized_end=4843
+  _GETSERVICEINFORESPONSE._serialized_start=4846
+  _GETSERVICEINFORESPONSE._serialized_end=4975
+  _CANCELACQUISITIONREQUEST._serialized_start=4977
+  _CANCELACQUISITIONREQUEST._serialized_end=5066
+  _CANCELACQUISITIONRESPONSE._serialized_start=5069
+  _CANCELACQUISITIONRESPONSE._serialized_end=5314
+  _CANCELACQUISITIONRESPONSE_STATUS._serialized_start=5204
+  _CANCELACQUISITIONRESPONSE_STATUS._serialized_end=5314
 # @@protoc_insertion_point(module_scope)
```

## bosdyn/api/data_acquisition_plugin_service_pb2_grpc.py

```diff
@@ -2,17 +2,17 @@
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
 from bosdyn.api import data_acquisition_pb2 as bosdyn_dot_api_dot_data__acquisition__pb2
 
 
 class DataAcquisitionPluginServiceStub(object):
-    """The DataAcquisitionPluginService is a gRPC service that a payload developer implements to retrieve
-    data from a sensor (or more generally perform some payload action) and optionally store that data
-    on the robot via the DataAcquisitionStore service.
+    """The DataAcquisitionPluginService is a gRPC service that a payload developer implements to
+    retrieve data from a sensor (or more generally perform some payload action) and optionally store
+    that data on the robot via the DataAcquisitionStore service.
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
@@ -36,36 +36,37 @@
                 '/bosdyn.api.DataAcquisitionPluginService/CancelAcquisition',
                 request_serializer=bosdyn_dot_api_dot_data__acquisition__pb2.CancelAcquisitionRequest.SerializeToString,
                 response_deserializer=bosdyn_dot_api_dot_data__acquisition__pb2.CancelAcquisitionResponse.FromString,
                 )
 
 
 class DataAcquisitionPluginServiceServicer(object):
-    """The DataAcquisitionPluginService is a gRPC service that a payload developer implements to retrieve
-    data from a sensor (or more generally perform some payload action) and optionally store that data
-    on the robot via the DataAcquisitionStore service.
+    """The DataAcquisitionPluginService is a gRPC service that a payload developer implements to
+    retrieve data from a sensor (or more generally perform some payload action) and optionally store
+    that data on the robot via the DataAcquisitionStore service.
     """
 
     def AcquirePluginData(self, request, context):
         """Trigger a data acquisition to save metadata and non-image data to the data buffer.
-        Sent by the main DAQ as a result of a data acquisition request from the tablet or a client.
+        Sent by the main Data Acquisition service as a result of a data acquisition request from the
+        tablet or a client.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetStatus(self, request, context):
         """Query the status of a data acquisition.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetServiceInfo(self, request, context):
-        """Get information from a DAQ service; lists acquisition capabilities.
+        """Get information from a Data Acquisition service; lists acquisition capabilities.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def CancelAcquisition(self, request, context):
         """Cancel an in-progress data acquisition.
@@ -101,17 +102,17 @@
     generic_handler = grpc.method_handlers_generic_handler(
             'bosdyn.api.DataAcquisitionPluginService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class DataAcquisitionPluginService(object):
-    """The DataAcquisitionPluginService is a gRPC service that a payload developer implements to retrieve
-    data from a sensor (or more generally perform some payload action) and optionally store that data
-    on the robot via the DataAcquisitionStore service.
+    """The DataAcquisitionPluginService is a gRPC service that a payload developer implements to
+    retrieve data from a sensor (or more generally perform some payload action) and optionally store
+    that data on the robot via the DataAcquisitionStore service.
     """
 
     @staticmethod
     def AcquirePluginData(request,
             target,
             options=(),
             channel_credentials=None,
```

## bosdyn/api/data_acquisition_service_pb2_grpc.py

```diff
@@ -55,15 +55,15 @@
         """Query the status of a data acquisition.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetServiceInfo(self, request, context):
-        """Get information from a DAQ service; lists acquisition capabilities.
+        """Get information from a Data Acquisition service; lists acquisition capabilities.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def CancelAcquisition(self, request, context):
         """Cancel an in-progress data acquisition.
```

## bosdyn/api/data_acquisition_store_pb2.py

```diff
@@ -14,15 +14,15 @@
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from bosdyn.api import header_pb2 as bosdyn_dot_api_dot_header__pb2
 from bosdyn.api import image_pb2 as bosdyn_dot_api_dot_image__pb2
 from bosdyn.api import data_acquisition_pb2 as bosdyn_dot_api_dot_data__acquisition__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'bosdyn/api/data_acquisition_store.proto\x12\nbosdyn.api\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x17\x62osdyn/api/header.proto\x1a\x16\x62osdyn/api/image.proto\x1a!bosdyn/api/data_acquisition.proto\"@\n\rActionIdQuery\x12/\n\naction_ids\x18\x01 \x03(\x0b\x32\x1b.bosdyn.api.CaptureActionId\"v\n\x0eTimeRangeQuery\x12\x32\n\x0e\x66rom_timestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0cto_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"}\n\x0f\x44\x61taQueryParams\x12\x30\n\ntime_range\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.TimeRangeQueryH\x00\x12/\n\naction_ids\x18\x02 \x01(\x0b\x32\x19.bosdyn.api.ActionIdQueryH\x00\x42\x07\n\x05query\"\x94\x01\n\x11StoreImageRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\'\n\x05image\x18\x02 \x01(\x0b\x32\x18.bosdyn.api.ImageCapture\x12+\n\x07\x64\x61ta_id\x18\x03 \x01(\x0b\x32\x1a.bosdyn.api.DataIdentifier\"@\n\x12StoreImageResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\"\xa0\x01\n\x14StoreMetadataRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x30\n\x08metadata\x18\x02 \x01(\x0b\x32\x1e.bosdyn.api.AssociatedMetadata\x12+\n\x07\x64\x61ta_id\x18\x03 \x01(\x0b\x32\x1a.bosdyn.api.DataIdentifier\"C\n\x15StoreMetadataResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\"\xa4\x01\n\x15StoreAlertDataRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x33\n\nalert_data\x18\x02 \x01(\x0b\x32\x1f.bosdyn.api.AssociatedAlertData\x12+\n\x07\x64\x61ta_id\x18\x03 \x01(\x0b\x32\x1a.bosdyn.api.DataIdentifier\"D\n\x16StoreAlertDataResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\"\x90\x01\n\x10StoreDataRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\x12+\n\x07\x64\x61ta_id\x18\x03 \x01(\x0b\x32\x1a.bosdyn.api.DataIdentifier\x12\x16\n\x0e\x66ile_extension\x18\x04 \x01(\t\"?\n\x11StoreDataResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\"r\n\x19ListCaptureActionsRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12*\n\x05query\x18\x02 \x01(\x0b\x32\x1b.bosdyn.api.DataQueryParams\"y\n\x1aListCaptureActionsResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12/\n\naction_ids\x18\x02 \x03(\x0b\x32\x1b.bosdyn.api.CaptureActionId\"p\n\x17ListStoredImagesRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12*\n\x05query\x18\x02 \x01(\x0b\x32\x1b.bosdyn.api.DataQueryParams\"t\n\x18ListStoredImagesResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12,\n\x08\x64\x61ta_ids\x18\x02 \x03(\x0b\x32\x1a.bosdyn.api.DataIdentifier\"r\n\x19ListStoredMetadataRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12*\n\x05query\x18\x02 \x01(\x0b\x32\x1b.bosdyn.api.DataQueryParams\"v\n\x1aListStoredMetadataResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12,\n\x08\x64\x61ta_ids\x18\x02 \x03(\x0b\x32\x1a.bosdyn.api.DataIdentifier\"s\n\x1aListStoredAlertDataRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12*\n\x05query\x18\x02 \x01(\x0b\x32\x1b.bosdyn.api.DataQueryParams\"w\n\x1bListStoredAlertDataResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12,\n\x08\x64\x61ta_ids\x18\x02 \x03(\x0b\x32\x1a.bosdyn.api.DataIdentifier\"n\n\x15ListStoredDataRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12*\n\x05query\x18\x02 \x01(\x0b\x32\x1b.bosdyn.api.DataQueryParams\"r\n\x16ListStoredDataResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12,\n\x08\x64\x61ta_ids\x18\x02 \x03(\x0b\x32\x1a.bosdyn.api.DataIdentifierB\x1b\x42\x19\x44\x61taAcquisitionStoreProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'bosdyn/api/data_acquisition_store.proto\x12\nbosdyn.api\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x17\x62osdyn/api/header.proto\x1a\x16\x62osdyn/api/image.proto\x1a!bosdyn/api/data_acquisition.proto\"@\n\rActionIdQuery\x12/\n\naction_ids\x18\x01 \x03(\x0b\x32\x1b.bosdyn.api.CaptureActionId\"v\n\x0eTimeRangeQuery\x12\x32\n\x0e\x66rom_timestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0cto_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"}\n\x0f\x44\x61taQueryParams\x12\x30\n\ntime_range\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.TimeRangeQueryH\x00\x12/\n\naction_ids\x18\x02 \x01(\x0b\x32\x19.bosdyn.api.ActionIdQueryH\x00\x42\x07\n\x05query\"\x94\x01\n\x11StoreImageRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\'\n\x05image\x18\x02 \x01(\x0b\x32\x18.bosdyn.api.ImageCapture\x12+\n\x07\x64\x61ta_id\x18\x03 \x01(\x0b\x32\x1a.bosdyn.api.DataIdentifier\"L\n\x12StoreImageResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\n\n\x02id\x18\x02 \x01(\x04\"\xa0\x01\n\x14StoreMetadataRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x30\n\x08metadata\x18\x02 \x01(\x0b\x32\x1e.bosdyn.api.AssociatedMetadata\x12+\n\x07\x64\x61ta_id\x18\x03 \x01(\x0b\x32\x1a.bosdyn.api.DataIdentifier\"O\n\x15StoreMetadataResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\n\n\x02id\x18\x02 \x01(\x04\"\xa4\x01\n\x15StoreAlertDataRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x33\n\nalert_data\x18\x02 \x01(\x0b\x32\x1f.bosdyn.api.AssociatedAlertData\x12+\n\x07\x64\x61ta_id\x18\x03 \x01(\x0b\x32\x1a.bosdyn.api.DataIdentifier\"P\n\x16StoreAlertDataResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\n\n\x02id\x18\x02 \x01(\x04\"\x90\x01\n\x10StoreDataRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\x12+\n\x07\x64\x61ta_id\x18\x03 \x01(\x0b\x32\x1a.bosdyn.api.DataIdentifier\x12\x16\n\x0e\x66ile_extension\x18\x04 \x01(\t\"K\n\x11StoreDataResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\n\n\x02id\x18\x02 \x01(\x04\"r\n\x19ListCaptureActionsRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12*\n\x05query\x18\x02 \x01(\x0b\x32\x1b.bosdyn.api.DataQueryParams\"y\n\x1aListCaptureActionsResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12/\n\naction_ids\x18\x02 \x03(\x0b\x32\x1b.bosdyn.api.CaptureActionId\"p\n\x17ListStoredImagesRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12*\n\x05query\x18\x02 \x01(\x0b\x32\x1b.bosdyn.api.DataQueryParams\"t\n\x18ListStoredImagesResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12,\n\x08\x64\x61ta_ids\x18\x02 \x03(\x0b\x32\x1a.bosdyn.api.DataIdentifier\"r\n\x19ListStoredMetadataRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12*\n\x05query\x18\x02 \x01(\x0b\x32\x1b.bosdyn.api.DataQueryParams\"v\n\x1aListStoredMetadataResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12,\n\x08\x64\x61ta_ids\x18\x02 \x03(\x0b\x32\x1a.bosdyn.api.DataIdentifier\"s\n\x1aListStoredAlertDataRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12*\n\x05query\x18\x02 \x01(\x0b\x32\x1b.bosdyn.api.DataQueryParams\"w\n\x1bListStoredAlertDataResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12,\n\x08\x64\x61ta_ids\x18\x02 \x03(\x0b\x32\x1a.bosdyn.api.DataIdentifier\"n\n\x15ListStoredDataRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12*\n\x05query\x18\x02 \x01(\x0b\x32\x1b.bosdyn.api.DataQueryParams\"r\n\x16ListStoredDataResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12,\n\x08\x64\x61ta_ids\x18\x02 \x03(\x0b\x32\x1a.bosdyn.api.DataIdentifierB\x1b\x42\x19\x44\x61taAcquisitionStoreProtob\x06proto3')
 
 
 
 _ACTIONIDQUERY = DESCRIPTOR.message_types_by_name['ActionIdQuery']
 _TIMERANGEQUERY = DESCRIPTOR.message_types_by_name['TimeRangeQuery']
 _DATAQUERYPARAMS = DESCRIPTOR.message_types_by_name['DataQueryParams']
 _STOREIMAGEREQUEST = DESCRIPTOR.message_types_by_name['StoreImageRequest']
@@ -199,41 +199,41 @@
   _TIMERANGEQUERY._serialized_start=238
   _TIMERANGEQUERY._serialized_end=356
   _DATAQUERYPARAMS._serialized_start=358
   _DATAQUERYPARAMS._serialized_end=483
   _STOREIMAGEREQUEST._serialized_start=486
   _STOREIMAGEREQUEST._serialized_end=634
   _STOREIMAGERESPONSE._serialized_start=636
-  _STOREIMAGERESPONSE._serialized_end=700
-  _STOREMETADATAREQUEST._serialized_start=703
-  _STOREMETADATAREQUEST._serialized_end=863
-  _STOREMETADATARESPONSE._serialized_start=865
-  _STOREMETADATARESPONSE._serialized_end=932
-  _STOREALERTDATAREQUEST._serialized_start=935
-  _STOREALERTDATAREQUEST._serialized_end=1099
-  _STOREALERTDATARESPONSE._serialized_start=1101
-  _STOREALERTDATARESPONSE._serialized_end=1169
-  _STOREDATAREQUEST._serialized_start=1172
-  _STOREDATAREQUEST._serialized_end=1316
-  _STOREDATARESPONSE._serialized_start=1318
-  _STOREDATARESPONSE._serialized_end=1381
-  _LISTCAPTUREACTIONSREQUEST._serialized_start=1383
-  _LISTCAPTUREACTIONSREQUEST._serialized_end=1497
-  _LISTCAPTUREACTIONSRESPONSE._serialized_start=1499
-  _LISTCAPTUREACTIONSRESPONSE._serialized_end=1620
-  _LISTSTOREDIMAGESREQUEST._serialized_start=1622
-  _LISTSTOREDIMAGESREQUEST._serialized_end=1734
-  _LISTSTOREDIMAGESRESPONSE._serialized_start=1736
-  _LISTSTOREDIMAGESRESPONSE._serialized_end=1852
-  _LISTSTOREDMETADATAREQUEST._serialized_start=1854
-  _LISTSTOREDMETADATAREQUEST._serialized_end=1968
-  _LISTSTOREDMETADATARESPONSE._serialized_start=1970
-  _LISTSTOREDMETADATARESPONSE._serialized_end=2088
-  _LISTSTOREDALERTDATAREQUEST._serialized_start=2090
-  _LISTSTOREDALERTDATAREQUEST._serialized_end=2205
-  _LISTSTOREDALERTDATARESPONSE._serialized_start=2207
-  _LISTSTOREDALERTDATARESPONSE._serialized_end=2326
-  _LISTSTOREDDATAREQUEST._serialized_start=2328
-  _LISTSTOREDDATAREQUEST._serialized_end=2438
-  _LISTSTOREDDATARESPONSE._serialized_start=2440
-  _LISTSTOREDDATARESPONSE._serialized_end=2554
+  _STOREIMAGERESPONSE._serialized_end=712
+  _STOREMETADATAREQUEST._serialized_start=715
+  _STOREMETADATAREQUEST._serialized_end=875
+  _STOREMETADATARESPONSE._serialized_start=877
+  _STOREMETADATARESPONSE._serialized_end=956
+  _STOREALERTDATAREQUEST._serialized_start=959
+  _STOREALERTDATAREQUEST._serialized_end=1123
+  _STOREALERTDATARESPONSE._serialized_start=1125
+  _STOREALERTDATARESPONSE._serialized_end=1205
+  _STOREDATAREQUEST._serialized_start=1208
+  _STOREDATAREQUEST._serialized_end=1352
+  _STOREDATARESPONSE._serialized_start=1354
+  _STOREDATARESPONSE._serialized_end=1429
+  _LISTCAPTUREACTIONSREQUEST._serialized_start=1431
+  _LISTCAPTUREACTIONSREQUEST._serialized_end=1545
+  _LISTCAPTUREACTIONSRESPONSE._serialized_start=1547
+  _LISTCAPTUREACTIONSRESPONSE._serialized_end=1668
+  _LISTSTOREDIMAGESREQUEST._serialized_start=1670
+  _LISTSTOREDIMAGESREQUEST._serialized_end=1782
+  _LISTSTOREDIMAGESRESPONSE._serialized_start=1784
+  _LISTSTOREDIMAGESRESPONSE._serialized_end=1900
+  _LISTSTOREDMETADATAREQUEST._serialized_start=1902
+  _LISTSTOREDMETADATAREQUEST._serialized_end=2016
+  _LISTSTOREDMETADATARESPONSE._serialized_start=2018
+  _LISTSTOREDMETADATARESPONSE._serialized_end=2136
+  _LISTSTOREDALERTDATAREQUEST._serialized_start=2138
+  _LISTSTOREDALERTDATAREQUEST._serialized_end=2253
+  _LISTSTOREDALERTDATARESPONSE._serialized_start=2255
+  _LISTSTOREDALERTDATARESPONSE._serialized_end=2374
+  _LISTSTOREDDATAREQUEST._serialized_start=2376
+  _LISTSTOREDDATAREQUEST._serialized_end=2486
+  _LISTSTOREDDATARESPONSE._serialized_start=2488
+  _LISTSTOREDDATARESPONSE._serialized_end=2602
 # @@protoc_insertion_point(module_scope)
```

## bosdyn/api/data_acquisition_store_service_pb2_grpc.py

```diff
@@ -4,16 +4,16 @@
 
 from bosdyn.api import data_acquisition_store_pb2 as bosdyn_dot_api_dot_data__acquisition__store__pb2
 
 
 class DataAcquisitionStoreServiceStub(object):
     """The DataAcquisitionStoreService is used to store data (images, data, metadata) on the robot
     in association with the DataIdentifiers specified by the DataAcquisitionService. Additionally,
-    requests can be made to the DataAcquisitionStoreService to identify different pieces of data or entire
-    capture actions which match query parameters, such as time ranges or action/group names.
+    requests can be made to the DataAcquisitionStoreService to identify different pieces of data or
+    entire capture actions which match query parameters, such as time ranges or action/group names.
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
@@ -64,16 +64,16 @@
                 response_deserializer=bosdyn_dot_api_dot_data__acquisition__store__pb2.StoreAlertDataResponse.FromString,
                 )
 
 
 class DataAcquisitionStoreServiceServicer(object):
     """The DataAcquisitionStoreService is used to store data (images, data, metadata) on the robot
     in association with the DataIdentifiers specified by the DataAcquisitionService. Additionally,
-    requests can be made to the DataAcquisitionStoreService to identify different pieces of data or entire
-    capture actions which match query parameters, such as time ranges or action/group names.
+    requests can be made to the DataAcquisitionStoreService to identify different pieces of data or
+    entire capture actions which match query parameters, such as time ranges or action/group names.
     """
 
     def ListCaptureActions(self, request, context):
         """List all CaptureActionIds (which identify an entire AcquireData RPC's data captures)
         that match the query parameters provided in the request.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
@@ -195,16 +195,16 @@
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class DataAcquisitionStoreService(object):
     """The DataAcquisitionStoreService is used to store data (images, data, metadata) on the robot
     in association with the DataIdentifiers specified by the DataAcquisitionService. Additionally,
-    requests can be made to the DataAcquisitionStoreService to identify different pieces of data or entire
-    capture actions which match query parameters, such as time ranges or action/group names.
+    requests can be made to the DataAcquisitionStoreService to identify different pieces of data or
+    entire capture actions which match query parameters, such as time ranges or action/group names.
     """
 
     @staticmethod
     def ListCaptureActions(request,
             target,
             options=(),
             channel_credentials=None,
```

## bosdyn/api/directory_pb2.py

```diff
@@ -12,15 +12,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from bosdyn.api import header_pb2 as bosdyn_dot_api_dot_header__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1a\x62osdyn/api/directory.proto\x12\nbosdyn.api\x1a\x17\x62osdyn/api/header.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\x96\x02\n\x0cServiceEntry\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x04type\x18\x02 \x01(\tH\x00\x12\x11\n\tauthority\x18\x03 \x01(\t\x12/\n\x0blast_update\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1b\n\x13user_token_required\x18\x05 \x01(\x08\x12\x1b\n\x13permission_required\x18\x07 \x01(\t\x12\x1d\n\x15liveness_timeout_secs\x18\x08 \x01(\x01\x12\x19\n\x11host_payload_guid\x18\t \x01(\tB\x0e\n\x0cservice_typeJ\x04\x08\x06\x10\x07R\x1a\x61pplication_token_required\")\n\x08\x45ndpoint\x12\x0f\n\x07host_ip\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\"Y\n\x16GetServiceEntryRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x14\n\x0cservice_name\x18\x02 \x01(\t\"\xff\x01\n\x17GetServiceEntryResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12:\n\x06status\x18\x02 \x01(\x0e\x32*.bosdyn.api.GetServiceEntryResponse.Status\x12/\n\rservice_entry\x18\x03 \x01(\x0b\x32\x18.bosdyn.api.ServiceEntry\"K\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1e\n\x1aSTATUS_NONEXISTENT_SERVICE\x10\x02\"F\n\x19ListServiceEntriesRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"{\n\x1aListServiceEntriesResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x31\n\x0fservice_entries\x18\x02 \x03(\x0b\x32\x18.bosdyn.api.ServiceEntryB\x10\x42\x0e\x44irectoryProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1a\x62osdyn/api/directory.proto\x12\nbosdyn.api\x1a\x17\x62osdyn/api/header.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\xfa\x01\n\x0cServiceEntry\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x04type\x18\x02 \x01(\tH\x00\x12\x11\n\tauthority\x18\x03 \x01(\t\x12/\n\x0blast_update\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1b\n\x13user_token_required\x18\x05 \x01(\x08\x12\x1b\n\x13permission_required\x18\x07 \x01(\t\x12\x1d\n\x15liveness_timeout_secs\x18\x08 \x01(\x01\x12\x19\n\x11host_payload_guid\x18\t \x01(\tB\x0e\n\x0cservice_typeJ\x04\x08\x06\x10\x07\")\n\x08\x45ndpoint\x12\x0f\n\x07host_ip\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\"Y\n\x16GetServiceEntryRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x14\n\x0cservice_name\x18\x02 \x01(\t\"\xff\x01\n\x17GetServiceEntryResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12:\n\x06status\x18\x02 \x01(\x0e\x32*.bosdyn.api.GetServiceEntryResponse.Status\x12/\n\rservice_entry\x18\x03 \x01(\x0b\x32\x18.bosdyn.api.ServiceEntry\"K\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1e\n\x1aSTATUS_NONEXISTENT_SERVICE\x10\x02\"F\n\x19ListServiceEntriesRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"{\n\x1aListServiceEntriesResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x31\n\x0fservice_entries\x18\x02 \x03(\x0b\x32\x18.bosdyn.api.ServiceEntryB\x10\x42\x0e\x44irectoryProtob\x06proto3')
 
 
 
 _SERVICEENTRY = DESCRIPTOR.message_types_by_name['ServiceEntry']
 _ENDPOINT = DESCRIPTOR.message_types_by_name['Endpoint']
 _GETSERVICEENTRYREQUEST = DESCRIPTOR.message_types_by_name['GetServiceEntryRequest']
 _GETSERVICEENTRYRESPONSE = DESCRIPTOR.message_types_by_name['GetServiceEntryResponse']
@@ -70,21 +70,21 @@
 _sym_db.RegisterMessage(ListServiceEntriesResponse)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'B\016DirectoryProto'
   _SERVICEENTRY._serialized_start=101
-  _SERVICEENTRY._serialized_end=379
-  _ENDPOINT._serialized_start=381
-  _ENDPOINT._serialized_end=422
-  _GETSERVICEENTRYREQUEST._serialized_start=424
-  _GETSERVICEENTRYREQUEST._serialized_end=513
-  _GETSERVICEENTRYRESPONSE._serialized_start=516
-  _GETSERVICEENTRYRESPONSE._serialized_end=771
-  _GETSERVICEENTRYRESPONSE_STATUS._serialized_start=696
-  _GETSERVICEENTRYRESPONSE_STATUS._serialized_end=771
-  _LISTSERVICEENTRIESREQUEST._serialized_start=773
-  _LISTSERVICEENTRIESREQUEST._serialized_end=843
-  _LISTSERVICEENTRIESRESPONSE._serialized_start=845
-  _LISTSERVICEENTRIESRESPONSE._serialized_end=968
+  _SERVICEENTRY._serialized_end=351
+  _ENDPOINT._serialized_start=353
+  _ENDPOINT._serialized_end=394
+  _GETSERVICEENTRYREQUEST._serialized_start=396
+  _GETSERVICEENTRYREQUEST._serialized_end=485
+  _GETSERVICEENTRYRESPONSE._serialized_start=488
+  _GETSERVICEENTRYRESPONSE._serialized_end=743
+  _GETSERVICEENTRYRESPONSE_STATUS._serialized_start=668
+  _GETSERVICEENTRYRESPONSE_STATUS._serialized_end=743
+  _LISTSERVICEENTRIESREQUEST._serialized_start=745
+  _LISTSERVICEENTRIESREQUEST._serialized_end=815
+  _LISTSERVICEENTRIESRESPONSE._serialized_start=817
+  _LISTSERVICEENTRIESRESPONSE._serialized_end=940
 # @@protoc_insertion_point(module_scope)
```

## bosdyn/api/gripper_camera_param_pb2.py

```diff
@@ -14,15 +14,15 @@
 
 
 from bosdyn.api import header_pb2 as bosdyn_dot_api_dot_header__pb2
 from bosdyn.api import geometry_pb2 as bosdyn_dot_api_dot_geometry__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%bosdyn/api/gripper_camera_param.proto\x12\nbosdyn.api\x1a\x17\x62osdyn/api/header.proto\x1a\x19\x62osdyn/api/geometry.proto\x1a\x1egoogle/protobuf/wrappers.proto\"w\n\x19GripperCameraParamRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12/\n\x06params\x18\x02 \x01(\x0b\x32\x1f.bosdyn.api.GripperCameraParams\"H\n\x1aGripperCameraParamResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\"I\n\x1cGripperCameraGetParamRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"|\n\x1dGripperCameraGetParamResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12/\n\x06params\x18\x02 \x01(\x0b\x32\x1f.bosdyn.api.GripperCameraParams\"\xbd\x08\n\x13GripperCameraParams\x12?\n\x0b\x63\x61mera_mode\x18\x01 \x01(\x0e\x32*.bosdyn.api.GripperCameraParams.CameraMode\x12/\n\nbrightness\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x12-\n\x08\x63ontrast\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x12/\n\nsaturation\x18\x04 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x12)\n\x04gain\x18\x07 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x12\x31\n\rexposure_auto\x18\n \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x36\n\x11\x65xposure_absolute\x18\x0b \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x12/\n\x0c\x65xposure_roi\x18\x10 \x01(\x0b\x32\x19.bosdyn.api.RoiParameters\x12.\n\nfocus_auto\x18\r \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x33\n\x0e\x66ocus_absolute\x18\x0c \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x12,\n\tfocus_roi\x18\x0e \x01(\x0b\x32\x19.bosdyn.api.RoiParameters\x12<\n\x18\x64raw_focus_roi_rectangle\x18\x12 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12&\n\x03hdr\x18\x11 \x01(\x0e\x32\x19.bosdyn.api.HdrParameters\x12\x39\n\x08led_mode\x18\x13 \x01(\x0e\x32\'.bosdyn.api.GripperCameraParams.LedMode\x12\x39\n\x14led_torch_brightness\x18\x14 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\"\xd6\x01\n\nCameraMode\x12\x10\n\x0cMODE_UNKNOWN\x10\x00\x12\x1c\n\x18MODE_1280_720_60FPS_UYVY\x10\x01\x12\x1c\n\x18MODE_640_480_120FPS_UYVY\x10\x0b\x12\x1d\n\x19MODE_1920_1080_60FPS_MJPG\x10\x0e\x12\x1d\n\x19MODE_3840_2160_30FPS_MJPG\x10\x0f\x12\x1d\n\x19MODE_4208_3120_20FPS_MJPG\x10\x10\x12\x1d\n\x19MODE_4096_2160_30FPS_MJPG\x10\x11\"E\n\x07LedMode\x12\x14\n\x10LED_MODE_UNKNOWN\x10\x00\x12\x10\n\x0cLED_MODE_OFF\x10\x01\x12\x12\n\x0eLED_MODE_TORCH\x10\x02\"\xe7\x02\n\rRoiParameters\x12\x31\n\x17roi_percentage_in_image\x18\x01 \x01(\x0b\x32\x10.bosdyn.api.Vec2\x12<\n\x0bwindow_size\x18\x02 \x01(\x0e\x32\'.bosdyn.api.RoiParameters.RoiWindowSize\"\xe4\x01\n\rRoiWindowSize\x12\x1b\n\x17ROI_WINDOW_SIZE_UNKNOWN\x10\x00\x12\x15\n\x11ROI_WINDOW_SIZE_1\x10\x01\x12\x15\n\x11ROI_WINDOW_SIZE_2\x10\x02\x12\x15\n\x11ROI_WINDOW_SIZE_3\x10\x03\x12\x15\n\x11ROI_WINDOW_SIZE_4\x10\x04\x12\x15\n\x11ROI_WINDOW_SIZE_5\x10\x05\x12\x15\n\x11ROI_WINDOW_SIZE_6\x10\x06\x12\x15\n\x11ROI_WINDOW_SIZE_7\x10\x07\x12\x15\n\x11ROI_WINDOW_SIZE_8\x10\x08*\x83\x01\n\rHdrParameters\x12\x0f\n\x0bHDR_UNKNOWN\x10\x00\x12\x0b\n\x07HDR_OFF\x10\x01\x12\x0c\n\x08HDR_AUTO\x10\x02\x12\x10\n\x0cHDR_MANUAL_1\x10\x03\x12\x10\n\x0cHDR_MANUAL_2\x10\x04\x12\x10\n\x0cHDR_MANUAL_3\x10\x05\x12\x10\n\x0cHDR_MANUAL_4\x10\x06\x42\x19\x42\x17GripperCameraParamProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%bosdyn/api/gripper_camera_param.proto\x12\nbosdyn.api\x1a\x17\x62osdyn/api/header.proto\x1a\x19\x62osdyn/api/geometry.proto\x1a\x1egoogle/protobuf/wrappers.proto\"w\n\x19GripperCameraParamRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12/\n\x06params\x18\x02 \x01(\x0b\x32\x1f.bosdyn.api.GripperCameraParams\"H\n\x1aGripperCameraParamResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\"I\n\x1cGripperCameraGetParamRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"|\n\x1dGripperCameraGetParamResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12/\n\x06params\x18\x02 \x01(\x0b\x32\x1f.bosdyn.api.GripperCameraParams\"\xae\x0b\n\x13GripperCameraParams\x12?\n\x0b\x63\x61mera_mode\x18\x01 \x01(\x0e\x32*.bosdyn.api.GripperCameraParams.CameraMode\x12/\n\nbrightness\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x12-\n\x08\x63ontrast\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x12/\n\nsaturation\x18\x04 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x12)\n\x04gain\x18\x07 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x12\x31\n\rexposure_auto\x18\n \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x36\n\x11\x65xposure_absolute\x18\x0b \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x12/\n\x0c\x65xposure_roi\x18\x10 \x01(\x0b\x32\x19.bosdyn.api.RoiParameters\x12.\n\nfocus_auto\x18\r \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x33\n\x0e\x66ocus_absolute\x18\x0c \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x12,\n\tfocus_roi\x18\x0e \x01(\x0b\x32\x19.bosdyn.api.RoiParameters\x12<\n\x18\x64raw_focus_roi_rectangle\x18\x12 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12&\n\x03hdr\x18\x11 \x01(\x0e\x32\x19.bosdyn.api.HdrParameters\x12\x39\n\x08led_mode\x18\x13 \x01(\x0e\x32\'.bosdyn.api.GripperCameraParams.LedMode\x12\x39\n\x14led_torch_brightness\x18\x14 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x12\x42\n\x1ewhite_balance_temperature_auto\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12*\n\x05gamma\x18\x06 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x12>\n\x19white_balance_temperature\x18\x08 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x12.\n\tsharpness\x18\t \x01(\x0b\x32\x1b.google.protobuf.FloatValue\"\xe7\x02\n\nCameraMode\x12\x10\n\x0cMODE_UNKNOWN\x10\x00\x12\x10\n\x0cMODE_640_480\x10\x0b\x12 \n\x18MODE_640_480_120FPS_UYVY\x10\x0b\x1a\x02\x08\x01\x12\x11\n\rMODE_1280_720\x10\x01\x12 \n\x18MODE_1280_720_60FPS_UYVY\x10\x01\x1a\x02\x08\x01\x12\x12\n\x0eMODE_1920_1080\x10\x0e\x12!\n\x19MODE_1920_1080_60FPS_MJPG\x10\x0e\x1a\x02\x08\x01\x12\x12\n\x0eMODE_3840_2160\x10\x0f\x12!\n\x19MODE_3840_2160_30FPS_MJPG\x10\x0f\x1a\x02\x08\x01\x12\x12\n\x0eMODE_4096_2160\x10\x11\x12!\n\x19MODE_4096_2160_30FPS_MJPG\x10\x11\x1a\x02\x08\x01\x12\x12\n\x0eMODE_4208_3120\x10\x10\x12!\n\x19MODE_4208_3120_20FPS_MJPG\x10\x10\x1a\x02\x08\x01\x1a\x02\x10\x01\"E\n\x07LedMode\x12\x14\n\x10LED_MODE_UNKNOWN\x10\x00\x12\x10\n\x0cLED_MODE_OFF\x10\x01\x12\x12\n\x0eLED_MODE_TORCH\x10\x02\"\xe7\x02\n\rRoiParameters\x12\x31\n\x17roi_percentage_in_image\x18\x01 \x01(\x0b\x32\x10.bosdyn.api.Vec2\x12<\n\x0bwindow_size\x18\x02 \x01(\x0e\x32\'.bosdyn.api.RoiParameters.RoiWindowSize\"\xe4\x01\n\rRoiWindowSize\x12\x1b\n\x17ROI_WINDOW_SIZE_UNKNOWN\x10\x00\x12\x15\n\x11ROI_WINDOW_SIZE_1\x10\x01\x12\x15\n\x11ROI_WINDOW_SIZE_2\x10\x02\x12\x15\n\x11ROI_WINDOW_SIZE_3\x10\x03\x12\x15\n\x11ROI_WINDOW_SIZE_4\x10\x04\x12\x15\n\x11ROI_WINDOW_SIZE_5\x10\x05\x12\x15\n\x11ROI_WINDOW_SIZE_6\x10\x06\x12\x15\n\x11ROI_WINDOW_SIZE_7\x10\x07\x12\x15\n\x11ROI_WINDOW_SIZE_8\x10\x08*\x83\x01\n\rHdrParameters\x12\x0f\n\x0bHDR_UNKNOWN\x10\x00\x12\x0b\n\x07HDR_OFF\x10\x01\x12\x0c\n\x08HDR_AUTO\x10\x02\x12\x10\n\x0cHDR_MANUAL_1\x10\x03\x12\x10\n\x0cHDR_MANUAL_2\x10\x04\x12\x10\n\x0cHDR_MANUAL_3\x10\x05\x12\x10\n\x0cHDR_MANUAL_4\x10\x06\x42\x19\x42\x17GripperCameraParamProtob\x06proto3')
 
 _HDRPARAMETERS = DESCRIPTOR.enum_types_by_name['HdrParameters']
 HdrParameters = enum_type_wrapper.EnumTypeWrapper(_HDRPARAMETERS)
 HDR_UNKNOWN = 0
 HDR_OFF = 1
 HDR_AUTO = 2
 HDR_MANUAL_1 = 3
@@ -82,28 +82,42 @@
   })
 _sym_db.RegisterMessage(RoiParameters)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'B\027GripperCameraParamProto'
-  _HDRPARAMETERS._serialized_start=1984
-  _HDRPARAMETERS._serialized_end=2115
+  _GRIPPERCAMERAPARAMS_CAMERAMODE._options = None
+  _GRIPPERCAMERAPARAMS_CAMERAMODE._serialized_options = b'\020\001'
+  _GRIPPERCAMERAPARAMS_CAMERAMODE.values_by_name["MODE_640_480_120FPS_UYVY"]._options = None
+  _GRIPPERCAMERAPARAMS_CAMERAMODE.values_by_name["MODE_640_480_120FPS_UYVY"]._serialized_options = b'\010\001'
+  _GRIPPERCAMERAPARAMS_CAMERAMODE.values_by_name["MODE_1280_720_60FPS_UYVY"]._options = None
+  _GRIPPERCAMERAPARAMS_CAMERAMODE.values_by_name["MODE_1280_720_60FPS_UYVY"]._serialized_options = b'\010\001'
+  _GRIPPERCAMERAPARAMS_CAMERAMODE.values_by_name["MODE_1920_1080_60FPS_MJPG"]._options = None
+  _GRIPPERCAMERAPARAMS_CAMERAMODE.values_by_name["MODE_1920_1080_60FPS_MJPG"]._serialized_options = b'\010\001'
+  _GRIPPERCAMERAPARAMS_CAMERAMODE.values_by_name["MODE_3840_2160_30FPS_MJPG"]._options = None
+  _GRIPPERCAMERAPARAMS_CAMERAMODE.values_by_name["MODE_3840_2160_30FPS_MJPG"]._serialized_options = b'\010\001'
+  _GRIPPERCAMERAPARAMS_CAMERAMODE.values_by_name["MODE_4096_2160_30FPS_MJPG"]._options = None
+  _GRIPPERCAMERAPARAMS_CAMERAMODE.values_by_name["MODE_4096_2160_30FPS_MJPG"]._serialized_options = b'\010\001'
+  _GRIPPERCAMERAPARAMS_CAMERAMODE.values_by_name["MODE_4208_3120_20FPS_MJPG"]._options = None
+  _GRIPPERCAMERAPARAMS_CAMERAMODE.values_by_name["MODE_4208_3120_20FPS_MJPG"]._serialized_options = b'\010\001'
+  _HDRPARAMETERS._serialized_start=2353
+  _HDRPARAMETERS._serialized_end=2484
   _GRIPPERCAMERAPARAMREQUEST._serialized_start=137
   _GRIPPERCAMERAPARAMREQUEST._serialized_end=256
   _GRIPPERCAMERAPARAMRESPONSE._serialized_start=258
   _GRIPPERCAMERAPARAMRESPONSE._serialized_end=330
   _GRIPPERCAMERAGETPARAMREQUEST._serialized_start=332
   _GRIPPERCAMERAGETPARAMREQUEST._serialized_end=405
   _GRIPPERCAMERAGETPARAMRESPONSE._serialized_start=407
   _GRIPPERCAMERAGETPARAMRESPONSE._serialized_end=531
   _GRIPPERCAMERAPARAMS._serialized_start=534
-  _GRIPPERCAMERAPARAMS._serialized_end=1619
-  _GRIPPERCAMERAPARAMS_CAMERAMODE._serialized_start=1334
-  _GRIPPERCAMERAPARAMS_CAMERAMODE._serialized_end=1548
-  _GRIPPERCAMERAPARAMS_LEDMODE._serialized_start=1550
-  _GRIPPERCAMERAPARAMS_LEDMODE._serialized_end=1619
-  _ROIPARAMETERS._serialized_start=1622
-  _ROIPARAMETERS._serialized_end=1981
-  _ROIPARAMETERS_ROIWINDOWSIZE._serialized_start=1753
-  _ROIPARAMETERS_ROIWINDOWSIZE._serialized_end=1981
+  _GRIPPERCAMERAPARAMS._serialized_end=1988
+  _GRIPPERCAMERAPARAMS_CAMERAMODE._serialized_start=1558
+  _GRIPPERCAMERAPARAMS_CAMERAMODE._serialized_end=1917
+  _GRIPPERCAMERAPARAMS_LEDMODE._serialized_start=1919
+  _GRIPPERCAMERAPARAMS_LEDMODE._serialized_end=1988
+  _ROIPARAMETERS._serialized_start=1991
+  _ROIPARAMETERS._serialized_end=2350
+  _ROIPARAMETERS_ROIWINDOWSIZE._serialized_start=2122
+  _ROIPARAMETERS_ROIWINDOWSIZE._serialized_end=2350
 # @@protoc_insertion_point(module_scope)
```

## bosdyn/api/image_pb2.py

```diff
@@ -10,33 +10,35 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from bosdyn.api import header_pb2 as bosdyn_dot_api_dot_header__pb2
 from bosdyn.api import geometry_pb2 as bosdyn_dot_api_dot_geometry__pb2
+from bosdyn.api import service_customization_pb2 as bosdyn_dot_api_dot_service__customization__pb2
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16\x62osdyn/api/image.proto\x12\nbosdyn.api\x1a\x17\x62osdyn/api/header.proto\x1a\x19\x62osdyn/api/geometry.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\x97\x03\n\x05Image\x12\x0c\n\x04\x63ols\x18\x02 \x01(\x05\x12\x0c\n\x04rows\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x0c\x12(\n\x06\x66ormat\x18\x05 \x01(\x0e\x32\x18.bosdyn.api.Image.Format\x12\x33\n\x0cpixel_format\x18\x06 \x01(\x0e\x32\x1d.bosdyn.api.Image.PixelFormat\"M\n\x06\x46ormat\x12\x12\n\x0e\x46ORMAT_UNKNOWN\x10\x00\x12\x0f\n\x0b\x46ORMAT_JPEG\x10\x01\x12\x0e\n\nFORMAT_RAW\x10\x02\x12\x0e\n\nFORMAT_RLE\x10\x03\"\xb5\x01\n\x0bPixelFormat\x12\x18\n\x14PIXEL_FORMAT_UNKNOWN\x10\x00\x12\x1d\n\x19PIXEL_FORMAT_GREYSCALE_U8\x10\x01\x12\x17\n\x13PIXEL_FORMAT_RGB_U8\x10\x03\x12\x18\n\x14PIXEL_FORMAT_RGBA_U8\x10\x04\x12\x1a\n\x16PIXEL_FORMAT_DEPTH_U16\x10\x05\x12\x1e\n\x1aPIXEL_FORMAT_GREYSCALE_U16\x10\x06\"W\n\x11\x43\x61ptureParameters\x12\x34\n\x11\x65xposure_duration\x18\x01 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x0c\n\x04gain\x18\x02 \x01(\x01\"\x86\x02\n\x0cImageCapture\x12\x34\n\x10\x61\x63quisition_time\x18\x1e \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x13transforms_snapshot\x18\x1f \x01(\x0b\x32\x1d.bosdyn.api.FrameTreeSnapshot\x12\x1f\n\x17\x66rame_name_image_sensor\x18\x05 \x01(\t\x12 \n\x05image\x18\x03 \x01(\x0b\x32\x11.bosdyn.api.Image\x12\x35\n\x0e\x63\x61pture_params\x18\x04 \x01(\x0b\x32\x1d.bosdyn.api.CaptureParametersJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03\"\xf6\x04\n\x0bImageSource\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63ols\x18\x04 \x01(\x05\x12\x0c\n\x04rows\x18\x05 \x01(\x05\x12\x13\n\x0b\x64\x65pth_scale\x18\x06 \x01(\x01\x12\x37\n\x07pinhole\x18\x08 \x01(\x0b\x32$.bosdyn.api.ImageSource.PinholeModelH\x00\x12\x35\n\nimage_type\x18\t \x01(\x0e\x32!.bosdyn.api.ImageSource.ImageType\x12\x34\n\rpixel_formats\x18\n \x03(\x0e\x32\x1d.bosdyn.api.Image.PixelFormat\x12/\n\rimage_formats\x18\x0b \x03(\x0e\x32\x18.bosdyn.api.Image.Format\x1a\xe1\x01\n\x0cPinholeModel\x12I\n\nintrinsics\x18\x01 \x01(\x0b\x32\x35.bosdyn.api.ImageSource.PinholeModel.CameraIntrinsics\x1a\x85\x01\n\x10\x43\x61meraIntrinsics\x12&\n\x0c\x66ocal_length\x18\x01 \x01(\x0b\x32\x10.bosdyn.api.Vec2\x12)\n\x0fprincipal_point\x18\x02 \x01(\x0b\x32\x10.bosdyn.api.Vec2\x12\x1e\n\x04skew\x18\x03 \x01(\x0b\x32\x10.bosdyn.api.Vec2\"P\n\tImageType\x12\x16\n\x12IMAGE_TYPE_UNKNOWN\x10\x00\x12\x15\n\x11IMAGE_TYPE_VISUAL\x10\x01\x12\x14\n\x10IMAGE_TYPE_DEPTH\x10\x02\x42\x0f\n\rcamera_modelsJ\x04\x08\x03\x10\x04J\x04\x08\x07\x10\x08\"D\n\x17ListImageSourcesRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"v\n\x18ListImageSourcesResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12.\n\rimage_sources\x18\x02 \x03(\x0b\x32\x17.bosdyn.api.ImageSource\"\xbd\x01\n\x0cImageRequest\x12\x19\n\x11image_source_name\x18\x01 \x01(\t\x12\x17\n\x0fquality_percent\x18\x02 \x01(\x01\x12.\n\x0cimage_format\x18\x03 \x01(\x0e\x32\x18.bosdyn.api.Image.Format\x12\x14\n\x0cresize_ratio\x18\x04 \x01(\x01\x12\x33\n\x0cpixel_format\x18\x05 \x01(\x0e\x32\x1d.bosdyn.api.Image.PixelFormat\"n\n\x0fGetImageRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x30\n\x0eimage_requests\x18\x02 \x03(\x0b\x32\x18.bosdyn.api.ImageRequest\"\xaf\x03\n\rImageResponse\x12&\n\x04shot\x18\x01 \x01(\x0b\x32\x18.bosdyn.api.ImageCapture\x12\'\n\x06source\x18\x02 \x01(\x0b\x32\x17.bosdyn.api.ImageSource\x12\x30\n\x06status\x18\x04 \x01(\x0e\x32 .bosdyn.api.ImageResponse.Status\"\x8e\x02\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x19\n\x15STATUS_UNKNOWN_CAMERA\x10\x02\x12\x1c\n\x18STATUS_SOURCE_DATA_ERROR\x10\x03\x12\x1b\n\x17STATUS_IMAGE_DATA_ERROR\x10\x04\x12-\n)STATUS_UNSUPPORTED_IMAGE_FORMAT_REQUESTED\x10\x05\x12-\n)STATUS_UNSUPPORTED_PIXEL_FORMAT_REQUESTED\x10\x06\x12-\n)STATUS_UNSUPPORTED_RESIZE_RATIO_REQUESTED\x10\x07J\x04\x08\x03\x10\x04J\x04\x08\x05\x10\x06\"r\n\x10GetImageResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x32\n\x0fimage_responses\x18\x02 \x03(\x0b\x32\x19.bosdyn.api.ImageResponseB\x0c\x42\nImageProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16\x62osdyn/api/image.proto\x12\nbosdyn.api\x1a\x17\x62osdyn/api/header.proto\x1a\x19\x62osdyn/api/geometry.proto\x1a&bosdyn/api/service_customization.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\x97\x03\n\x05Image\x12\x0c\n\x04\x63ols\x18\x02 \x01(\x05\x12\x0c\n\x04rows\x18\x03 \x01(\x05\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x0c\x12(\n\x06\x66ormat\x18\x05 \x01(\x0e\x32\x18.bosdyn.api.Image.Format\x12\x33\n\x0cpixel_format\x18\x06 \x01(\x0e\x32\x1d.bosdyn.api.Image.PixelFormat\"M\n\x06\x46ormat\x12\x12\n\x0e\x46ORMAT_UNKNOWN\x10\x00\x12\x0f\n\x0b\x46ORMAT_JPEG\x10\x01\x12\x0e\n\nFORMAT_RAW\x10\x02\x12\x0e\n\nFORMAT_RLE\x10\x03\"\xb5\x01\n\x0bPixelFormat\x12\x18\n\x14PIXEL_FORMAT_UNKNOWN\x10\x00\x12\x1d\n\x19PIXEL_FORMAT_GREYSCALE_U8\x10\x01\x12\x17\n\x13PIXEL_FORMAT_RGB_U8\x10\x03\x12\x18\n\x14PIXEL_FORMAT_RGBA_U8\x10\x04\x12\x1a\n\x16PIXEL_FORMAT_DEPTH_U16\x10\x05\x12\x1e\n\x1aPIXEL_FORMAT_GREYSCALE_U16\x10\x06\"\x85\x01\n\x11\x43\x61ptureParameters\x12\x34\n\x11\x65xposure_duration\x18\x01 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x0c\n\x04gain\x18\x02 \x01(\x01\x12,\n\rcustom_params\x18\x03 \x01(\x0b\x32\x15.bosdyn.api.DictParam\"\x86\x02\n\x0cImageCapture\x12\x34\n\x10\x61\x63quisition_time\x18\x1e \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x13transforms_snapshot\x18\x1f \x01(\x0b\x32\x1d.bosdyn.api.FrameTreeSnapshot\x12\x1f\n\x17\x66rame_name_image_sensor\x18\x05 \x01(\t\x12 \n\x05image\x18\x03 \x01(\x0b\x32\x11.bosdyn.api.Image\x12\x35\n\x0e\x63\x61pture_params\x18\x04 \x01(\x0b\x32\x1d.bosdyn.api.CaptureParametersJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03\"\xa9\x05\n\x0bImageSource\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0c\n\x04\x63ols\x18\x04 \x01(\x05\x12\x0c\n\x04rows\x18\x05 \x01(\x05\x12\x13\n\x0b\x64\x65pth_scale\x18\x06 \x01(\x01\x12\x37\n\x07pinhole\x18\x08 \x01(\x0b\x32$.bosdyn.api.ImageSource.PinholeModelH\x00\x12\x35\n\nimage_type\x18\t \x01(\x0e\x32!.bosdyn.api.ImageSource.ImageType\x12\x34\n\rpixel_formats\x18\n \x03(\x0e\x32\x1d.bosdyn.api.Image.PixelFormat\x12/\n\rimage_formats\x18\x0b \x03(\x0e\x32\x18.bosdyn.api.Image.Format\x12\x31\n\rcustom_params\x18\x0c \x01(\x0b\x32\x1a.bosdyn.api.DictParam.Spec\x1a\xe1\x01\n\x0cPinholeModel\x12I\n\nintrinsics\x18\x01 \x01(\x0b\x32\x35.bosdyn.api.ImageSource.PinholeModel.CameraIntrinsics\x1a\x85\x01\n\x10\x43\x61meraIntrinsics\x12&\n\x0c\x66ocal_length\x18\x01 \x01(\x0b\x32\x10.bosdyn.api.Vec2\x12)\n\x0fprincipal_point\x18\x02 \x01(\x0b\x32\x10.bosdyn.api.Vec2\x12\x1e\n\x04skew\x18\x03 \x01(\x0b\x32\x10.bosdyn.api.Vec2\"P\n\tImageType\x12\x16\n\x12IMAGE_TYPE_UNKNOWN\x10\x00\x12\x15\n\x11IMAGE_TYPE_VISUAL\x10\x01\x12\x14\n\x10IMAGE_TYPE_DEPTH\x10\x02\x42\x0f\n\rcamera_modelsJ\x04\x08\x03\x10\x04J\x04\x08\x07\x10\x08\"D\n\x17ListImageSourcesRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"v\n\x18ListImageSourcesResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12.\n\rimage_sources\x18\x02 \x03(\x0b\x32\x17.bosdyn.api.ImageSource\"\xeb\x01\n\x0cImageRequest\x12\x19\n\x11image_source_name\x18\x01 \x01(\t\x12\x17\n\x0fquality_percent\x18\x02 \x01(\x01\x12.\n\x0cimage_format\x18\x03 \x01(\x0e\x32\x18.bosdyn.api.Image.Format\x12\x14\n\x0cresize_ratio\x18\x04 \x01(\x01\x12\x33\n\x0cpixel_format\x18\x05 \x01(\x0e\x32\x1d.bosdyn.api.Image.PixelFormat\x12,\n\rcustom_params\x18\x06 \x01(\x0b\x32\x15.bosdyn.api.DictParam\"n\n\x0fGetImageRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x30\n\x0eimage_requests\x18\x02 \x03(\x0b\x32\x18.bosdyn.api.ImageRequest\"\x89\x04\n\rImageResponse\x12&\n\x04shot\x18\x01 \x01(\x0b\x32\x18.bosdyn.api.ImageCapture\x12\'\n\x06source\x18\x02 \x01(\x0b\x32\x17.bosdyn.api.ImageSource\x12\x30\n\x06status\x18\x04 \x01(\x0e\x32 .bosdyn.api.ImageResponse.Status\x12\x38\n\x12\x63ustom_param_error\x18\x06 \x01(\x0b\x32\x1c.bosdyn.api.CustomParamError\"\xae\x02\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x19\n\x15STATUS_UNKNOWN_CAMERA\x10\x02\x12\x1c\n\x18STATUS_SOURCE_DATA_ERROR\x10\x03\x12\x1b\n\x17STATUS_IMAGE_DATA_ERROR\x10\x04\x12-\n)STATUS_UNSUPPORTED_IMAGE_FORMAT_REQUESTED\x10\x05\x12-\n)STATUS_UNSUPPORTED_PIXEL_FORMAT_REQUESTED\x10\x06\x12-\n)STATUS_UNSUPPORTED_RESIZE_RATIO_REQUESTED\x10\x07\x12\x1e\n\x1aSTATUS_CUSTOM_PARAMS_ERROR\x10\x08J\x04\x08\x03\x10\x04J\x04\x08\x05\x10\x06\"\x7f\n\x15ImageCaptureAndSource\x12&\n\x04shot\x18\x01 \x01(\x0b\x32\x18.bosdyn.api.ImageCapture\x12\'\n\x06source\x18\x02 \x01(\x0b\x32\x17.bosdyn.api.ImageSource\x12\x15\n\rimage_service\x18\x03 \x01(\t\"r\n\x10GetImageResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x32\n\x0fimage_responses\x18\x02 \x03(\x0b\x32\x19.bosdyn.api.ImageResponseB\x0c\x42\nImageProtob\x06proto3')
 
 
 
 _IMAGE = DESCRIPTOR.message_types_by_name['Image']
 _CAPTUREPARAMETERS = DESCRIPTOR.message_types_by_name['CaptureParameters']
 _IMAGECAPTURE = DESCRIPTOR.message_types_by_name['ImageCapture']
 _IMAGESOURCE = DESCRIPTOR.message_types_by_name['ImageSource']
 _IMAGESOURCE_PINHOLEMODEL = _IMAGESOURCE.nested_types_by_name['PinholeModel']
 _IMAGESOURCE_PINHOLEMODEL_CAMERAINTRINSICS = _IMAGESOURCE_PINHOLEMODEL.nested_types_by_name['CameraIntrinsics']
 _LISTIMAGESOURCESREQUEST = DESCRIPTOR.message_types_by_name['ListImageSourcesRequest']
 _LISTIMAGESOURCESRESPONSE = DESCRIPTOR.message_types_by_name['ListImageSourcesResponse']
 _IMAGEREQUEST = DESCRIPTOR.message_types_by_name['ImageRequest']
 _GETIMAGEREQUEST = DESCRIPTOR.message_types_by_name['GetImageRequest']
 _IMAGERESPONSE = DESCRIPTOR.message_types_by_name['ImageResponse']
+_IMAGECAPTUREANDSOURCE = DESCRIPTOR.message_types_by_name['ImageCaptureAndSource']
 _GETIMAGERESPONSE = DESCRIPTOR.message_types_by_name['GetImageResponse']
 _IMAGE_FORMAT = _IMAGE.enum_types_by_name['Format']
 _IMAGE_PIXELFORMAT = _IMAGE.enum_types_by_name['PixelFormat']
 _IMAGESOURCE_IMAGETYPE = _IMAGESOURCE.enum_types_by_name['ImageType']
 _IMAGERESPONSE_STATUS = _IMAGERESPONSE.enum_types_by_name['Status']
 Image = _reflection.GeneratedProtocolMessageType('Image', (_message.Message,), {
   'DESCRIPTOR' : _IMAGE,
@@ -113,51 +115,60 @@
 ImageResponse = _reflection.GeneratedProtocolMessageType('ImageResponse', (_message.Message,), {
   'DESCRIPTOR' : _IMAGERESPONSE,
   '__module__' : 'bosdyn.api.image_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.ImageResponse)
   })
 _sym_db.RegisterMessage(ImageResponse)
 
+ImageCaptureAndSource = _reflection.GeneratedProtocolMessageType('ImageCaptureAndSource', (_message.Message,), {
+  'DESCRIPTOR' : _IMAGECAPTUREANDSOURCE,
+  '__module__' : 'bosdyn.api.image_pb2'
+  # @@protoc_insertion_point(class_scope:bosdyn.api.ImageCaptureAndSource)
+  })
+_sym_db.RegisterMessage(ImageCaptureAndSource)
+
 GetImageResponse = _reflection.GeneratedProtocolMessageType('GetImageResponse', (_message.Message,), {
   'DESCRIPTOR' : _GETIMAGERESPONSE,
   '__module__' : 'bosdyn.api.image_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.GetImageResponse)
   })
 _sym_db.RegisterMessage(GetImageResponse)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'B\nImageProto'
-  _IMAGE._serialized_start=156
-  _IMAGE._serialized_end=563
-  _IMAGE_FORMAT._serialized_start=302
-  _IMAGE_FORMAT._serialized_end=379
-  _IMAGE_PIXELFORMAT._serialized_start=382
-  _IMAGE_PIXELFORMAT._serialized_end=563
-  _CAPTUREPARAMETERS._serialized_start=565
-  _CAPTUREPARAMETERS._serialized_end=652
-  _IMAGECAPTURE._serialized_start=655
-  _IMAGECAPTURE._serialized_end=917
-  _IMAGESOURCE._serialized_start=920
-  _IMAGESOURCE._serialized_end=1550
-  _IMAGESOURCE_PINHOLEMODEL._serialized_start=1214
-  _IMAGESOURCE_PINHOLEMODEL._serialized_end=1439
-  _IMAGESOURCE_PINHOLEMODEL_CAMERAINTRINSICS._serialized_start=1306
-  _IMAGESOURCE_PINHOLEMODEL_CAMERAINTRINSICS._serialized_end=1439
-  _IMAGESOURCE_IMAGETYPE._serialized_start=1441
-  _IMAGESOURCE_IMAGETYPE._serialized_end=1521
-  _LISTIMAGESOURCESREQUEST._serialized_start=1552
-  _LISTIMAGESOURCESREQUEST._serialized_end=1620
-  _LISTIMAGESOURCESRESPONSE._serialized_start=1622
-  _LISTIMAGESOURCESRESPONSE._serialized_end=1740
-  _IMAGEREQUEST._serialized_start=1743
-  _IMAGEREQUEST._serialized_end=1932
-  _GETIMAGEREQUEST._serialized_start=1934
-  _GETIMAGEREQUEST._serialized_end=2044
-  _IMAGERESPONSE._serialized_start=2047
-  _IMAGERESPONSE._serialized_end=2478
-  _IMAGERESPONSE_STATUS._serialized_start=2196
-  _IMAGERESPONSE_STATUS._serialized_end=2466
-  _GETIMAGERESPONSE._serialized_start=2480
-  _GETIMAGERESPONSE._serialized_end=2594
+  _IMAGE._serialized_start=196
+  _IMAGE._serialized_end=603
+  _IMAGE_FORMAT._serialized_start=342
+  _IMAGE_FORMAT._serialized_end=419
+  _IMAGE_PIXELFORMAT._serialized_start=422
+  _IMAGE_PIXELFORMAT._serialized_end=603
+  _CAPTUREPARAMETERS._serialized_start=606
+  _CAPTUREPARAMETERS._serialized_end=739
+  _IMAGECAPTURE._serialized_start=742
+  _IMAGECAPTURE._serialized_end=1004
+  _IMAGESOURCE._serialized_start=1007
+  _IMAGESOURCE._serialized_end=1688
+  _IMAGESOURCE_PINHOLEMODEL._serialized_start=1352
+  _IMAGESOURCE_PINHOLEMODEL._serialized_end=1577
+  _IMAGESOURCE_PINHOLEMODEL_CAMERAINTRINSICS._serialized_start=1444
+  _IMAGESOURCE_PINHOLEMODEL_CAMERAINTRINSICS._serialized_end=1577
+  _IMAGESOURCE_IMAGETYPE._serialized_start=1579
+  _IMAGESOURCE_IMAGETYPE._serialized_end=1659
+  _LISTIMAGESOURCESREQUEST._serialized_start=1690
+  _LISTIMAGESOURCESREQUEST._serialized_end=1758
+  _LISTIMAGESOURCESRESPONSE._serialized_start=1760
+  _LISTIMAGESOURCESRESPONSE._serialized_end=1878
+  _IMAGEREQUEST._serialized_start=1881
+  _IMAGEREQUEST._serialized_end=2116
+  _GETIMAGEREQUEST._serialized_start=2118
+  _GETIMAGEREQUEST._serialized_end=2228
+  _IMAGERESPONSE._serialized_start=2231
+  _IMAGERESPONSE._serialized_end=2752
+  _IMAGERESPONSE_STATUS._serialized_start=2438
+  _IMAGERESPONSE_STATUS._serialized_end=2740
+  _IMAGECAPTUREANDSOURCE._serialized_start=2754
+  _IMAGECAPTUREANDSOURCE._serialized_end=2881
+  _GETIMAGERESPONSE._serialized_start=2883
+  _GETIMAGERESPONSE._serialized_end=2997
 # @@protoc_insertion_point(module_scope)
```

## bosdyn/api/lease_pb2.py

```diff
@@ -12,15 +12,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from bosdyn.api import header_pb2 as bosdyn_dot_api_dot_header__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16\x62osdyn/api/lease.proto\x12\nbosdyn.api\x1a\x17\x62osdyn/api/header.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"P\n\x05Lease\x12\x10\n\x08resource\x18\x01 \x01(\t\x12\r\n\x05\x65poch\x18\x02 \x01(\t\x12\x10\n\x08sequence\x18\x03 \x03(\r\x12\x14\n\x0c\x63lient_names\x18\x04 \x03(\t\"Q\n\x0cResourceTree\x12\x10\n\x08resource\x18\x01 \x01(\t\x12/\n\rsub_resources\x18\x02 \x03(\x0b\x32\x18.bosdyn.api.ResourceTree\"4\n\nLeaseOwner\x12\x13\n\x0b\x63lient_name\x18\x01 \x01(\t\x12\x11\n\tuser_name\x18\x02 \x01(\t\"\xb9\x03\n\x0eLeaseUseResult\x12\x31\n\x06status\x18\x01 \x01(\x0e\x32!.bosdyn.api.LeaseUseResult.Status\x12%\n\x05owner\x18\x02 \x01(\x0b\x32\x16.bosdyn.api.LeaseOwner\x12*\n\x0f\x61ttempted_lease\x18\x03 \x01(\x0b\x32\x11.bosdyn.api.Lease\x12)\n\x0eprevious_lease\x18\x04 \x01(\x0b\x32\x11.bosdyn.api.Lease\x12-\n\x12latest_known_lease\x18\x05 \x01(\x0b\x32\x11.bosdyn.api.Lease\x12+\n\x10latest_resources\x18\x06 \x03(\x0b\x32\x11.bosdyn.api.Lease\"\x99\x01\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x18\n\x14STATUS_INVALID_LEASE\x10\x02\x12\x10\n\x0cSTATUS_OLDER\x10\x03\x12\x12\n\x0eSTATUS_REVOKED\x10\x04\x12\x14\n\x10STATUS_UNMANAGED\x10\x05\x12\x16\n\x12STATUS_WRONG_EPOCH\x10\x06\"R\n\x13\x41\x63quireLeaseRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x10\n\x08resource\x18\x02 \x01(\t\"\xe0\x02\n\x14\x41\x63quireLeaseResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x37\n\x06status\x18\x02 \x01(\x0e\x32\'.bosdyn.api.AcquireLeaseResponse.Status\x12 \n\x05lease\x18\x03 \x01(\x0b\x32\x11.bosdyn.api.Lease\x12+\n\x0blease_owner\x18\x04 \x01(\x0b\x32\x16.bosdyn.api.LeaseOwner\"\x93\x01\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12#\n\x1fSTATUS_RESOURCE_ALREADY_CLAIMED\x10\x02\x12\x1b\n\x17STATUS_INVALID_RESOURCE\x10\x03\x12$\n STATUS_NOT_AUTHORITATIVE_SERVICE\x10\x04\"O\n\x10TakeLeaseRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x10\n\x08resource\x18\x02 \x01(\t\"\xb4\x02\n\x11TakeLeaseResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x34\n\x06status\x18\x02 \x01(\x0e\x32$.bosdyn.api.TakeLeaseResponse.Status\x12 \n\x05lease\x18\x03 \x01(\x0b\x32\x11.bosdyn.api.Lease\x12+\n\x0blease_owner\x18\x04 \x01(\x0b\x32\x16.bosdyn.api.LeaseOwner\"n\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1b\n\x17STATUS_INVALID_RESOURCE\x10\x02\x12$\n STATUS_NOT_AUTHORITATIVE_SERVICE\x10\x03\"a\n\x12ReturnLeaseRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12 \n\x05lease\x18\x02 \x01(\x0b\x32\x11.bosdyn.api.Lease\"\x87\x02\n\x13ReturnLeaseResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x36\n\x06status\x18\x02 \x01(\x0e\x32&.bosdyn.api.ReturnLeaseResponse.Status\"\x8b\x01\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1b\n\x17STATUS_INVALID_RESOURCE\x10\x02\x12\x1b\n\x17STATUS_NOT_ACTIVE_LEASE\x10\x03\x12$\n STATUS_NOT_AUTHORITATIVE_SERVICE\x10\x04\"_\n\x11ListLeasesRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x1f\n\x17include_full_lease_info\x18\x02 \x01(\x08\"\xa0\x01\n\rLeaseResource\x12\x10\n\x08resource\x18\x01 \x01(\t\x12 \n\x05lease\x18\x02 \x01(\x0b\x32\x11.bosdyn.api.Lease\x12+\n\x0blease_owner\x18\x03 \x01(\x0b\x32\x16.bosdyn.api.LeaseOwner\x12.\n\nstale_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x9f\x01\n\x12ListLeasesResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12,\n\tresources\x18\x02 \x03(\x0b\x32\x19.bosdyn.api.LeaseResource\x12/\n\rresource_tree\x18\x03 \x01(\x0b\x32\x18.bosdyn.api.ResourceTree\"a\n\x12RetainLeaseRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12 \n\x05lease\x18\x02 \x01(\x0b\x32\x11.bosdyn.api.Lease\"w\n\x13RetainLeaseResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x34\n\x10lease_use_result\x18\x02 \x01(\x0b\x32\x1a.bosdyn.api.LeaseUseResultB\x0c\x42\nLeaseProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16\x62osdyn/api/lease.proto\x12\nbosdyn.api\x1a\x17\x62osdyn/api/header.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"P\n\x05Lease\x12\x10\n\x08resource\x18\x01 \x01(\t\x12\r\n\x05\x65poch\x18\x02 \x01(\t\x12\x10\n\x08sequence\x18\x03 \x03(\r\x12\x14\n\x0c\x63lient_names\x18\x04 \x03(\t\"Q\n\x0cResourceTree\x12\x10\n\x08resource\x18\x01 \x01(\t\x12/\n\rsub_resources\x18\x02 \x03(\x0b\x32\x18.bosdyn.api.ResourceTree\"4\n\nLeaseOwner\x12\x13\n\x0b\x63lient_name\x18\x01 \x01(\t\x12\x11\n\tuser_name\x18\x02 \x01(\t\"\xb9\x03\n\x0eLeaseUseResult\x12\x31\n\x06status\x18\x01 \x01(\x0e\x32!.bosdyn.api.LeaseUseResult.Status\x12%\n\x05owner\x18\x02 \x01(\x0b\x32\x16.bosdyn.api.LeaseOwner\x12*\n\x0f\x61ttempted_lease\x18\x03 \x01(\x0b\x32\x11.bosdyn.api.Lease\x12)\n\x0eprevious_lease\x18\x04 \x01(\x0b\x32\x11.bosdyn.api.Lease\x12-\n\x12latest_known_lease\x18\x05 \x01(\x0b\x32\x11.bosdyn.api.Lease\x12+\n\x10latest_resources\x18\x06 \x03(\x0b\x32\x11.bosdyn.api.Lease\"\x99\x01\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x18\n\x14STATUS_INVALID_LEASE\x10\x02\x12\x10\n\x0cSTATUS_OLDER\x10\x03\x12\x12\n\x0eSTATUS_REVOKED\x10\x04\x12\x14\n\x10STATUS_UNMANAGED\x10\x05\x12\x16\n\x12STATUS_WRONG_EPOCH\x10\x06\"R\n\x13\x41\x63quireLeaseRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x10\n\x08resource\x18\x02 \x01(\t\"\xe0\x02\n\x14\x41\x63quireLeaseResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x37\n\x06status\x18\x02 \x01(\x0e\x32\'.bosdyn.api.AcquireLeaseResponse.Status\x12 \n\x05lease\x18\x03 \x01(\x0b\x32\x11.bosdyn.api.Lease\x12+\n\x0blease_owner\x18\x04 \x01(\x0b\x32\x16.bosdyn.api.LeaseOwner\"\x93\x01\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12#\n\x1fSTATUS_RESOURCE_ALREADY_CLAIMED\x10\x02\x12\x1b\n\x17STATUS_INVALID_RESOURCE\x10\x03\x12$\n STATUS_NOT_AUTHORITATIVE_SERVICE\x10\x04\"O\n\x10TakeLeaseRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x10\n\x08resource\x18\x02 \x01(\t\"\xb4\x02\n\x11TakeLeaseResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x34\n\x06status\x18\x02 \x01(\x0e\x32$.bosdyn.api.TakeLeaseResponse.Status\x12 \n\x05lease\x18\x03 \x01(\x0b\x32\x11.bosdyn.api.Lease\x12+\n\x0blease_owner\x18\x04 \x01(\x0b\x32\x16.bosdyn.api.LeaseOwner\"n\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1b\n\x17STATUS_INVALID_RESOURCE\x10\x02\x12$\n STATUS_NOT_AUTHORITATIVE_SERVICE\x10\x03\"a\n\x12ReturnLeaseRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12 \n\x05lease\x18\x02 \x01(\x0b\x32\x11.bosdyn.api.Lease\"\x87\x02\n\x13ReturnLeaseResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x36\n\x06status\x18\x02 \x01(\x0e\x32&.bosdyn.api.ReturnLeaseResponse.Status\"\x8b\x01\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1b\n\x17STATUS_INVALID_RESOURCE\x10\x02\x12\x1b\n\x17STATUS_NOT_ACTIVE_LEASE\x10\x03\x12$\n STATUS_NOT_AUTHORITATIVE_SERVICE\x10\x04\"_\n\x11ListLeasesRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x1f\n\x17include_full_lease_info\x18\x02 \x01(\x08\"\xb6\x01\n\rLeaseResource\x12\x10\n\x08resource\x18\x01 \x01(\t\x12 \n\x05lease\x18\x02 \x01(\x0b\x32\x11.bosdyn.api.Lease\x12+\n\x0blease_owner\x18\x03 \x01(\x0b\x32\x16.bosdyn.api.LeaseOwner\x12\x32\n\nstale_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x02\x18\x01\x12\x10\n\x08is_stale\x18\x05 \x01(\x08\"\x9f\x01\n\x12ListLeasesResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12,\n\tresources\x18\x02 \x03(\x0b\x32\x19.bosdyn.api.LeaseResource\x12/\n\rresource_tree\x18\x03 \x01(\x0b\x32\x18.bosdyn.api.ResourceTree\"a\n\x12RetainLeaseRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12 \n\x05lease\x18\x02 \x01(\x0b\x32\x11.bosdyn.api.Lease\"w\n\x13RetainLeaseResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x34\n\x10lease_use_result\x18\x02 \x01(\x0b\x32\x1a.bosdyn.api.LeaseUseResultB\x0c\x42\nLeaseProtob\x06proto3')
 
 
 
 _LEASE = DESCRIPTOR.message_types_by_name['Lease']
 _RESOURCETREE = DESCRIPTOR.message_types_by_name['ResourceTree']
 _LEASEOWNER = DESCRIPTOR.message_types_by_name['LeaseOwner']
 _LEASEUSERESULT = DESCRIPTOR.message_types_by_name['LeaseUseResult']
@@ -144,14 +144,16 @@
   })
 _sym_db.RegisterMessage(RetainLeaseResponse)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'B\nLeaseProto'
+  _LEASERESOURCE.fields_by_name['stale_time']._options = None
+  _LEASERESOURCE.fields_by_name['stale_time']._serialized_options = b'\030\001'
   _LEASE._serialized_start=96
   _LEASE._serialized_end=176
   _RESOURCETREE._serialized_start=178
   _RESOURCETREE._serialized_end=259
   _LEASEOWNER._serialized_start=261
   _LEASEOWNER._serialized_end=313
   _LEASEUSERESULT._serialized_start=316
@@ -175,15 +177,15 @@
   _RETURNLEASERESPONSE._serialized_start=1690
   _RETURNLEASERESPONSE._serialized_end=1953
   _RETURNLEASERESPONSE_STATUS._serialized_start=1814
   _RETURNLEASERESPONSE_STATUS._serialized_end=1953
   _LISTLEASESREQUEST._serialized_start=1955
   _LISTLEASESREQUEST._serialized_end=2050
   _LEASERESOURCE._serialized_start=2053
-  _LEASERESOURCE._serialized_end=2213
-  _LISTLEASESRESPONSE._serialized_start=2216
-  _LISTLEASESRESPONSE._serialized_end=2375
-  _RETAINLEASEREQUEST._serialized_start=2377
-  _RETAINLEASEREQUEST._serialized_end=2474
-  _RETAINLEASERESPONSE._serialized_start=2476
-  _RETAINLEASERESPONSE._serialized_end=2595
+  _LEASERESOURCE._serialized_end=2235
+  _LISTLEASESRESPONSE._serialized_start=2238
+  _LISTLEASESRESPONSE._serialized_end=2397
+  _RETAINLEASEREQUEST._serialized_start=2399
+  _RETAINLEASEREQUEST._serialized_end=2496
+  _RETAINLEASERESPONSE._serialized_start=2498
+  _RETAINLEASERESPONSE._serialized_end=2617
 # @@protoc_insertion_point(module_scope)
```

## bosdyn/api/log_annotation_pb2.py

```diff
@@ -12,15 +12,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from bosdyn.api import header_pb2 as bosdyn_dot_api_dot_header__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1f\x62osdyn/api/log_annotation.proto\x12\nbosdyn.api\x1a\x17\x62osdyn/api/header.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"u\n\x17\x41\x64\x64LogAnnotationRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12/\n\x0b\x61nnotations\x18\x02 \x01(\x0b\x32\x1a.bosdyn.api.LogAnnotations\"\xc7\x01\n\x0eLogAnnotations\x12;\n\rtext_messages\x18\x01 \x03(\x0b\x32$.bosdyn.api.LogAnnotationTextMessage\x12\x43\n\x11operator_messages\x18\x02 \x03(\x0b\x32(.bosdyn.api.LogAnnotationOperatorMessage\x12\x33\n\tblob_data\x18\x03 \x03(\x0b\x32 .bosdyn.api.LogAnnotationLogBlob\"\xee\x02\n\x18LogAnnotationTextMessage\x12\x0f\n\x07message\x18\x01 \x01(\t\x12-\n\ttimestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07service\x18\x03 \x01(\t\x12\x39\n\x05level\x18\x04 \x01(\x0e\x32*.bosdyn.api.LogAnnotationTextMessage.Level\x12\x0b\n\x03tag\x18\x05 \x01(\t\x12\x10\n\x08\x66ilename\x18\x06 \x01(\t\x12\x13\n\x0bline_number\x18\x07 \x01(\x05\x12\x34\n\x10timestamp_client\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\\\n\x05Level\x12\x11\n\rLEVEL_UNKNOWN\x10\x00\x12\x0f\n\x0bLEVEL_DEBUG\x10\x01\x12\x0e\n\nLEVEL_INFO\x10\x02\x12\x0e\n\nLEVEL_WARN\x10\x03\x12\x0f\n\x0bLEVEL_ERROR\x10\x04\"\x94\x01\n\x1cLogAnnotationOperatorMessage\x12\x0f\n\x07message\x18\x01 \x01(\t\x12-\n\ttimestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10timestamp_client\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xab\x01\n\x14LogAnnotationLogBlob\x12-\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07\x63hannel\x18\x02 \x01(\t\x12\x0f\n\x07type_id\x18\x03 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x0c\x12\x34\n\x10timestamp_client\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"L\n\x18\x41\x64\x64LogAnnotationResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeaderJ\x04\x08\x02\x10\x03\x42\x14\x42\x12LogAnnotationProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1f\x62osdyn/api/log_annotation.proto\x12\nbosdyn.api\x1a\x17\x62osdyn/api/header.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"y\n\x17\x41\x64\x64LogAnnotationRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12/\n\x0b\x61nnotations\x18\x02 \x01(\x0b\x32\x1a.bosdyn.api.LogAnnotations:\x02\x18\x01\"\xcb\x01\n\x0eLogAnnotations\x12;\n\rtext_messages\x18\x01 \x03(\x0b\x32$.bosdyn.api.LogAnnotationTextMessage\x12\x43\n\x11operator_messages\x18\x02 \x03(\x0b\x32(.bosdyn.api.LogAnnotationOperatorMessage\x12\x33\n\tblob_data\x18\x03 \x03(\x0b\x32 .bosdyn.api.LogAnnotationLogBlob:\x02\x18\x01\"\xf2\x02\n\x18LogAnnotationTextMessage\x12\x0f\n\x07message\x18\x01 \x01(\t\x12-\n\ttimestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07service\x18\x03 \x01(\t\x12\x39\n\x05level\x18\x04 \x01(\x0e\x32*.bosdyn.api.LogAnnotationTextMessage.Level\x12\x0b\n\x03tag\x18\x05 \x01(\t\x12\x10\n\x08\x66ilename\x18\x06 \x01(\t\x12\x13\n\x0bline_number\x18\x07 \x01(\x05\x12\x34\n\x10timestamp_client\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\\\n\x05Level\x12\x11\n\rLEVEL_UNKNOWN\x10\x00\x12\x0f\n\x0bLEVEL_DEBUG\x10\x01\x12\x0e\n\nLEVEL_INFO\x10\x02\x12\x0e\n\nLEVEL_WARN\x10\x03\x12\x0f\n\x0bLEVEL_ERROR\x10\x04:\x02\x18\x01\"\x98\x01\n\x1cLogAnnotationOperatorMessage\x12\x0f\n\x07message\x18\x01 \x01(\t\x12-\n\ttimestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10timestamp_client\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp:\x02\x18\x01\"\xaf\x01\n\x14LogAnnotationLogBlob\x12-\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07\x63hannel\x18\x02 \x01(\t\x12\x0f\n\x07type_id\x18\x03 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x04 \x01(\x0c\x12\x34\n\x10timestamp_client\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp:\x02\x18\x01\"P\n\x18\x41\x64\x64LogAnnotationResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader:\x02\x18\x01J\x04\x08\x02\x10\x03\x42\x14\x42\x12LogAnnotationProtob\x06proto3')
 
 
 
 _ADDLOGANNOTATIONREQUEST = DESCRIPTOR.message_types_by_name['AddLogAnnotationRequest']
 _LOGANNOTATIONS = DESCRIPTOR.message_types_by_name['LogAnnotations']
 _LOGANNOTATIONTEXTMESSAGE = DESCRIPTOR.message_types_by_name['LogAnnotationTextMessage']
 _LOGANNOTATIONOPERATORMESSAGE = DESCRIPTOR.message_types_by_name['LogAnnotationOperatorMessage']
@@ -69,22 +69,34 @@
   })
 _sym_db.RegisterMessage(AddLogAnnotationResponse)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'B\022LogAnnotationProto'
+  _ADDLOGANNOTATIONREQUEST._options = None
+  _ADDLOGANNOTATIONREQUEST._serialized_options = b'\030\001'
+  _LOGANNOTATIONS._options = None
+  _LOGANNOTATIONS._serialized_options = b'\030\001'
+  _LOGANNOTATIONTEXTMESSAGE._options = None
+  _LOGANNOTATIONTEXTMESSAGE._serialized_options = b'\030\001'
+  _LOGANNOTATIONOPERATORMESSAGE._options = None
+  _LOGANNOTATIONOPERATORMESSAGE._serialized_options = b'\030\001'
+  _LOGANNOTATIONLOGBLOB._options = None
+  _LOGANNOTATIONLOGBLOB._serialized_options = b'\030\001'
+  _ADDLOGANNOTATIONRESPONSE._options = None
+  _ADDLOGANNOTATIONRESPONSE._serialized_options = b'\030\001'
   _ADDLOGANNOTATIONREQUEST._serialized_start=105
-  _ADDLOGANNOTATIONREQUEST._serialized_end=222
-  _LOGANNOTATIONS._serialized_start=225
-  _LOGANNOTATIONS._serialized_end=424
-  _LOGANNOTATIONTEXTMESSAGE._serialized_start=427
-  _LOGANNOTATIONTEXTMESSAGE._serialized_end=793
-  _LOGANNOTATIONTEXTMESSAGE_LEVEL._serialized_start=701
-  _LOGANNOTATIONTEXTMESSAGE_LEVEL._serialized_end=793
-  _LOGANNOTATIONOPERATORMESSAGE._serialized_start=796
-  _LOGANNOTATIONOPERATORMESSAGE._serialized_end=944
-  _LOGANNOTATIONLOGBLOB._serialized_start=947
-  _LOGANNOTATIONLOGBLOB._serialized_end=1118
-  _ADDLOGANNOTATIONRESPONSE._serialized_start=1120
-  _ADDLOGANNOTATIONRESPONSE._serialized_end=1196
+  _ADDLOGANNOTATIONREQUEST._serialized_end=226
+  _LOGANNOTATIONS._serialized_start=229
+  _LOGANNOTATIONS._serialized_end=432
+  _LOGANNOTATIONTEXTMESSAGE._serialized_start=435
+  _LOGANNOTATIONTEXTMESSAGE._serialized_end=805
+  _LOGANNOTATIONTEXTMESSAGE_LEVEL._serialized_start=709
+  _LOGANNOTATIONTEXTMESSAGE_LEVEL._serialized_end=801
+  _LOGANNOTATIONOPERATORMESSAGE._serialized_start=808
+  _LOGANNOTATIONOPERATORMESSAGE._serialized_end=960
+  _LOGANNOTATIONLOGBLOB._serialized_start=963
+  _LOGANNOTATIONLOGBLOB._serialized_end=1138
+  _ADDLOGANNOTATIONRESPONSE._serialized_start=1140
+  _ADDLOGANNOTATIONRESPONSE._serialized_end=1220
 # @@protoc_insertion_point(module_scope)
```

## bosdyn/api/log_annotation_service_pb2_grpc.py

```diff
@@ -2,19 +2,17 @@
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
 from bosdyn.api import log_annotation_pb2 as bosdyn_dot_api_dot_log__annotation__pb2
 
 
 class LogAnnotationServiceStub(object):
-    """DEPRECATED as of 2.1.0: Please use the DataBufferService instead of the LogAnnotationService.
-    The LogAnnotationService is deprecated in release 2.1 and may be removed in the
-    future.
-    LogAnnotationService allows adding information to the robot's log files.
-    This service is a mechanism for adding information to the robot's log files.
+    """DEPRECATED as of 2.1.0 and will be removed in 4.0. Please use the DataBufferService instead of
+    the LogAnnotationService. LogAnnotationService allows adding information to the robot's log
+    files. This service is a mechanism for adding information to the robot's log files.
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
@@ -23,19 +21,17 @@
                 '/bosdyn.api.LogAnnotationService/AddLogAnnotation',
                 request_serializer=bosdyn_dot_api_dot_log__annotation__pb2.AddLogAnnotationRequest.SerializeToString,
                 response_deserializer=bosdyn_dot_api_dot_log__annotation__pb2.AddLogAnnotationResponse.FromString,
                 )
 
 
 class LogAnnotationServiceServicer(object):
-    """DEPRECATED as of 2.1.0: Please use the DataBufferService instead of the LogAnnotationService.
-    The LogAnnotationService is deprecated in release 2.1 and may be removed in the
-    future.
-    LogAnnotationService allows adding information to the robot's log files.
-    This service is a mechanism for adding information to the robot's log files.
+    """DEPRECATED as of 2.1.0 and will be removed in 4.0. Please use the DataBufferService instead of
+    the LogAnnotationService. LogAnnotationService allows adding information to the robot's log
+    files. This service is a mechanism for adding information to the robot's log files.
     """
 
     def AddLogAnnotation(self, request, context):
         """Add the specified information to the robot's log files.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
@@ -53,19 +49,17 @@
     generic_handler = grpc.method_handlers_generic_handler(
             'bosdyn.api.LogAnnotationService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class LogAnnotationService(object):
-    """DEPRECATED as of 2.1.0: Please use the DataBufferService instead of the LogAnnotationService.
-    The LogAnnotationService is deprecated in release 2.1 and may be removed in the
-    future.
-    LogAnnotationService allows adding information to the robot's log files.
-    This service is a mechanism for adding information to the robot's log files.
+    """DEPRECATED as of 2.1.0 and will be removed in 4.0. Please use the DataBufferService instead of
+    the LogAnnotationService. LogAnnotationService allows adding information to the robot's log
+    files. This service is a mechanism for adding information to the robot's log files.
     """
 
     @staticmethod
     def AddLogAnnotation(request,
             target,
             options=(),
             channel_credentials=None,
```

## bosdyn/api/network_compute_bridge_pb2.py

```diff
@@ -12,46 +12,59 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from bosdyn.api import alerts_pb2 as bosdyn_dot_api_dot_alerts__pb2
 from bosdyn.api import header_pb2 as bosdyn_dot_api_dot_header__pb2
 from bosdyn.api import image_pb2 as bosdyn_dot_api_dot_image__pb2
+from bosdyn.api import service_customization_pb2 as bosdyn_dot_api_dot_service__customization__pb2
 from bosdyn.api import world_object_pb2 as bosdyn_dot_api_dot_world__object__pb2
 from google.protobuf import any_pb2 as google_dot_protobuf_dot_any__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'bosdyn/api/network_compute_bridge.proto\x12\nbosdyn.api\x1a\x17\x62osdyn/api/alerts.proto\x1a\x17\x62osdyn/api/header.proto\x1a\x16\x62osdyn/api/image.proto\x1a\x1d\x62osdyn/api/world_object.proto\x1a\x19google/protobuf/any.proto\x1a\x1cgoogle/protobuf/struct.proto\"\x8d\x01\n\x1aListAvailableModelsRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x44\n\rserver_config\x18\x02 \x01(\x0b\x32-.bosdyn.api.NetworkComputeServerConfiguration\"\xc3\x01\n\x1bListAvailableModelsResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x18\n\x10\x61vailable_models\x18\x02 \x03(\t\x12\'\n\x06labels\x18\x06 \x03(\x0b\x32\x17.bosdyn.api.ModelLabels\x12\x35\n\x06status\x18\x05 \x01(\x0e\x32%.bosdyn.api.ListAvailableModelsStatus\";\n\x0bModelLabels\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x18\n\x10\x61vailable_labels\x18\x02 \x03(\t\"\xc1\x01\n\x15NetworkComputeRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x37\n\ninput_data\x18\x02 \x01(\x0b\x32#.bosdyn.api.NetworkComputeInputData\x12\x44\n\rserver_config\x18\x03 \x01(\x0b\x32-.bosdyn.api.NetworkComputeServerConfiguration\"\x89\x01\n\x15ImageSourceAndService\x12\x16\n\x0cimage_source\x18\x01 \x01(\tH\x00\x12\x31\n\rimage_request\x18\x03 \x01(\x0b\x32\x18.bosdyn.api.ImageRequestH\x00\x12\x15\n\rimage_service\x18\x02 \x01(\tB\x0e\n\x0crequest_data\"\xbd\x03\n\x17NetworkComputeInputData\x12\x45\n\x18image_source_and_service\x18\x07 \x01(\x0b\x32!.bosdyn.api.ImageSourceAndServiceH\x00\x12\"\n\x05image\x18\x02 \x01(\x0b\x32\x11.bosdyn.api.ImageH\x00\x12(\n\nother_data\x18\x03 \x01(\x0b\x32\x14.google.protobuf.Any\x12\x12\n\nmodel_name\x18\x04 \x01(\t\x12\x16\n\x0emin_confidence\x18\x05 \x01(\x02\x12\x45\n\x0crotate_image\x18\x06 \x01(\x0e\x32/.bosdyn.api.NetworkComputeInputData.RotateImage\"\x8a\x01\n\x0bRotateImage\x12\x18\n\x14ROTATE_IMAGE_UNKNOWN\x10\x00\x12\x1c\n\x18ROTATE_IMAGE_NO_ROTATION\x10\x03\x12!\n\x1dROTATE_IMAGE_ALIGN_HORIZONTAL\x10\x01\x12 \n\x1cROTATE_IMAGE_ALIGN_WITH_BODY\x10\x02\x42\x07\n\x05inputJ\x04\x08\x01\x10\x02\"E\n!NetworkComputeServerConfiguration\x12\x14\n\x0cservice_name\x18\x03 \x01(\tJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03\"\xc8\x01\n\x0bOutputImage\x12\x31\n\x0eimage_response\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.ImageResponse\x12)\n\x08metadata\x18\x02 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x30\n\x0fobject_in_image\x18\x03 \x03(\x0b\x32\x17.bosdyn.api.WorldObject\x12)\n\nalert_data\x18\x04 \x01(\x0b\x32\x15.bosdyn.api.AlertData\"\xe9\x03\n\x16NetworkComputeResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x30\n\x0fobject_in_image\x18\x02 \x03(\x0b\x32\x17.bosdyn.api.WorldObject\x12\x31\n\x0eimage_response\x18\x03 \x01(\x0b\x32\x19.bosdyn.api.ImageResponse\x12\x1c\n\x14image_rotation_angle\x18\x06 \x01(\x01\x12(\n\nother_data\x18\x04 \x01(\x0b\x32\x14.google.protobuf.Any\x12\x30\n\x06status\x18\x05 \x01(\x0e\x32 .bosdyn.api.NetworkComputeStatus\x12)\n\nalert_data\x18\x07 \x01(\x0b\x32\x15.bosdyn.api.AlertData\x12K\n\routput_images\x18\x08 \x03(\x0b\x32\x34.bosdyn.api.NetworkComputeResponse.OutputImagesEntry\x1aL\n\x11OutputImagesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12&\n\x05value\x18\x02 \x01(\x0b\x32\x17.bosdyn.api.OutputImage:\x02\x38\x01*\xf2\x01\n\x14NetworkComputeStatus\x12\"\n\x1eNETWORK_COMPUTE_STATUS_UNKNOWN\x10\x00\x12\"\n\x1eNETWORK_COMPUTE_STATUS_SUCCESS\x10\x01\x12\x35\n1NETWORK_COMPUTE_STATUS_EXTERNAL_SERVICE_NOT_FOUND\x10\x02\x12\x30\n,NETWORK_COMPUTE_STATUS_EXTERNAL_SERVER_ERROR\x10\x03\x12)\n%NETWORK_COMPUTE_STATUS_ROTATION_ERROR\x10\x04*\xe4\x01\n\x19ListAvailableModelsStatus\x12(\n$LIST_AVAILABLE_MODELS_STATUS_UNKNOWN\x10\x00\x12(\n$LIST_AVAILABLE_MODELS_STATUS_SUCCESS\x10\x01\x12;\n7LIST_AVAILABLE_MODELS_STATUS_EXTERNAL_SERVICE_NOT_FOUND\x10\x02\x12\x36\n2LIST_AVAILABLE_MODELS_STATUS_EXTERNAL_SERVER_ERROR\x10\x03\x42\x1b\x42\x19NetworkComputeBridgeProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'bosdyn/api/network_compute_bridge.proto\x12\nbosdyn.api\x1a\x17\x62osdyn/api/alerts.proto\x1a\x17\x62osdyn/api/header.proto\x1a\x16\x62osdyn/api/image.proto\x1a&bosdyn/api/service_customization.proto\x1a\x1d\x62osdyn/api/world_object.proto\x1a\x19google/protobuf/any.proto\x1a\x1cgoogle/protobuf/struct.proto\"\x8d\x01\n\x1aListAvailableModelsRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x44\n\rserver_config\x18\x02 \x01(\x0b\x32-.bosdyn.api.NetworkComputeServerConfiguration\"\xf8\x01\n\x1bListAvailableModelsResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x1c\n\x10\x61vailable_models\x18\x02 \x03(\tB\x02\x18\x01\x12+\n\x06labels\x18\x06 \x03(\x0b\x32\x17.bosdyn.api.ModelLabelsB\x02\x18\x01\x12+\n\x06models\x18\x03 \x01(\x0b\x32\x1b.bosdyn.api.AvailableModels\x12\x35\n\x06status\x18\x05 \x01(\x0e\x32%.bosdyn.api.ListAvailableModelsStatus\"6\n\x0f\x41vailableModels\x12#\n\x04\x64\x61ta\x18\x01 \x03(\x0b\x32\x15.bosdyn.api.ModelData\"\xa4\x01\n\tModelData\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x18\n\x10\x61vailable_labels\x18\x02 \x03(\t\x12\x36\n\x11output_image_spec\x18\x03 \x03(\x0b\x32\x1b.bosdyn.api.OutputImageSpec\x12\x31\n\rcustom_params\x18\x07 \x01(\x0b\x32\x1a.bosdyn.api.DictParam.Spec\";\n\x0bModelLabels\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x18\n\x10\x61vailable_labels\x18\x02 \x03(\t\"\x98\x02\n\x15NetworkComputeRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12=\n\ninput_data\x18\x02 \x01(\x0b\x32#.bosdyn.api.NetworkComputeInputDataB\x02\x18\x01H\x00\x12\x46\n\x11input_data_bridge\x18\x04 \x01(\x0b\x32).bosdyn.api.NetworkComputeInputDataBridgeH\x00\x12\x44\n\rserver_config\x18\x03 \x01(\x0b\x32-.bosdyn.api.NetworkComputeServerConfigurationB\x07\n\x05input\"\x89\x01\n\x15ImageSourceAndService\x12\x16\n\x0cimage_source\x18\x01 \x01(\tH\x00\x12\x31\n\rimage_request\x18\x03 \x01(\x0b\x32\x18.bosdyn.api.ImageRequestH\x00\x12\x15\n\rimage_service\x18\x02 \x01(\tB\x0e\n\x0crequest_data\"\xc2\x01\n\nOutputData\x12)\n\x08metadata\x18\x02 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x30\n\x0fobject_in_image\x18\x03 \x03(\x0b\x32\x17.bosdyn.api.WorldObject\x12)\n\nalert_data\x18\x04 \x01(\x0b\x32\x15.bosdyn.api.AlertData\x12(\n\nother_data\x18\x05 \x01(\x0b\x32\x14.google.protobuf.Any:\x02\x18\x01\"\xbc\x01\n\x11\x43omputeParameters\x12(\n\nother_data\x18\x03 \x01(\x0b\x32\x14.google.protobuf.Any\x12\x12\n\nmodel_name\x18\x04 \x01(\t\x12;\n\x10reference_images\x18\x06 \x03(\x0b\x32!.bosdyn.api.ImageCaptureAndSource\x12,\n\rcustom_params\x18\x07 \x01(\x0b\x32\x15.bosdyn.api.DictParam\"\x99\x01\n\x1dNetworkComputeInputDataBridge\x12\x45\n\x1aimage_sources_and_services\x18\x01 \x03(\x0b\x32!.bosdyn.api.ImageSourceAndService\x12\x31\n\nparameters\x18\x02 \x01(\x0b\x32\x1d.bosdyn.api.ComputeParameters\"\x85\x01\n\x1dNetworkComputeInputDataWorker\x12\x31\n\x06images\x18\x01 \x03(\x0b\x32!.bosdyn.api.ImageCaptureAndSource\x12\x31\n\nparameters\x18\x02 \x01(\x0b\x32\x1d.bosdyn.api.ComputeParameters\"\xc7\x03\n\x17NetworkComputeInputData\x12\x45\n\x18image_source_and_service\x18\x07 \x01(\x0b\x32!.bosdyn.api.ImageSourceAndServiceH\x00\x12\"\n\x05image\x18\x02 \x01(\x0b\x32\x11.bosdyn.api.ImageH\x00\x12(\n\nother_data\x18\x03 \x01(\x0b\x32\x14.google.protobuf.Any\x12\x12\n\nmodel_name\x18\x04 \x01(\t\x12\x16\n\x0emin_confidence\x18\x05 \x01(\x02\x12\x45\n\x0crotate_image\x18\x06 \x01(\x0e\x32/.bosdyn.api.NetworkComputeInputData.RotateImage\"\x8a\x01\n\x0bRotateImage\x12\x18\n\x14ROTATE_IMAGE_UNKNOWN\x10\x00\x12\x1c\n\x18ROTATE_IMAGE_NO_ROTATION\x10\x03\x12!\n\x1dROTATE_IMAGE_ALIGN_HORIZONTAL\x10\x01\x12 \n\x1cROTATE_IMAGE_ALIGN_WITH_BODY\x10\x02:\x02\x18\x01\x42\x07\n\x05inputJ\x04\x08\x01\x10\x02J\x04\x08\t\x10\n\"E\n!NetworkComputeServerConfiguration\x12\x14\n\x0cservice_name\x18\x03 \x01(\tJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03\"\xc8\x01\n\x0bOutputImage\x12\x31\n\x0eimage_response\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.ImageResponse\x12)\n\x08metadata\x18\x02 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x30\n\x0fobject_in_image\x18\x03 \x03(\x0b\x32\x17.bosdyn.api.WorldObject\x12)\n\nalert_data\x18\x04 \x01(\x0b\x32\x15.bosdyn.api.AlertData\",\n\x0fOutputImageSpec\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x8d\x06\n\x16NetworkComputeResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x30\n\x0fobject_in_image\x18\x02 \x03(\x0b\x32\x17.bosdyn.api.WorldObject\x12\x35\n\x0eimage_response\x18\x03 \x01(\x0b\x32\x19.bosdyn.api.ImageResponseB\x02\x18\x01\x12:\n\x0fimage_responses\x18\r \x03(\x0b\x32!.bosdyn.api.ImageCaptureAndSource\x12 \n\x14image_rotation_angle\x18\x06 \x01(\x01\x42\x02\x18\x01\x12(\n\nother_data\x18\x04 \x01(\x0b\x32\x14.google.protobuf.Any\x12\x30\n\x06status\x18\x05 \x01(\x0e\x32 .bosdyn.api.NetworkComputeStatus\x12\x38\n\x12\x63ustom_param_error\x18\x0b \x01(\x0b\x32\x1c.bosdyn.api.CustomParamError\x12-\n\nalert_data\x18\x07 \x01(\x0b\x32\x15.bosdyn.api.AlertDataB\x02\x18\x01\x12K\n\routput_images\x18\x08 \x03(\x0b\x32\x34.bosdyn.api.NetworkComputeResponse.OutputImagesEntry\x12R\n\x0froi_output_data\x18\n \x03(\x0b\x32\x35.bosdyn.api.NetworkComputeResponse.RoiOutputDataEntryB\x02\x18\x01\x1aL\n\x11OutputImagesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12&\n\x05value\x18\x02 \x01(\x0b\x32\x17.bosdyn.api.OutputImage:\x02\x38\x01\x1aL\n\x12RoiOutputDataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12%\n\x05value\x18\x02 \x01(\x0b\x32\x16.bosdyn.api.OutputData:\x02\x38\x01\"\x80\x01\n\x14WorkerComputeRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12=\n\ninput_data\x18\x02 \x01(\x0b\x32).bosdyn.api.NetworkComputeInputDataWorker\"\xff\x02\n\x15WorkerComputeResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12(\n\nother_data\x18\x02 \x01(\x0b\x32\x14.google.protobuf.Any\x12\x30\n\x06status\x18\x03 \x01(\x0e\x32 .bosdyn.api.NetworkComputeStatus\x12\x38\n\x12\x63ustom_param_error\x18\x04 \x01(\x0b\x32\x1c.bosdyn.api.CustomParamError\x12J\n\routput_images\x18\x07 \x03(\x0b\x32\x33.bosdyn.api.WorkerComputeResponse.OutputImagesEntry\x1aL\n\x11OutputImagesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12&\n\x05value\x18\x02 \x01(\x0b\x32\x17.bosdyn.api.OutputImage:\x02\x38\x01J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07*\xa2\x02\n\x14NetworkComputeStatus\x12\"\n\x1eNETWORK_COMPUTE_STATUS_UNKNOWN\x10\x00\x12\"\n\x1eNETWORK_COMPUTE_STATUS_SUCCESS\x10\x01\x12\x35\n1NETWORK_COMPUTE_STATUS_EXTERNAL_SERVICE_NOT_FOUND\x10\x02\x12\x30\n,NETWORK_COMPUTE_STATUS_EXTERNAL_SERVER_ERROR\x10\x03\x12)\n%NETWORK_COMPUTE_STATUS_ROTATION_ERROR\x10\x04\x12.\n*NETWORK_COMPUTE_STATUS_CUSTOM_PARAMS_ERROR\x10\x05*\xe4\x01\n\x19ListAvailableModelsStatus\x12(\n$LIST_AVAILABLE_MODELS_STATUS_UNKNOWN\x10\x00\x12(\n$LIST_AVAILABLE_MODELS_STATUS_SUCCESS\x10\x01\x12;\n7LIST_AVAILABLE_MODELS_STATUS_EXTERNAL_SERVICE_NOT_FOUND\x10\x02\x12\x36\n2LIST_AVAILABLE_MODELS_STATUS_EXTERNAL_SERVER_ERROR\x10\x03\x42\x1b\x42\x19NetworkComputeBridgeProtob\x06proto3')
 
 _NETWORKCOMPUTESTATUS = DESCRIPTOR.enum_types_by_name['NetworkComputeStatus']
 NetworkComputeStatus = enum_type_wrapper.EnumTypeWrapper(_NETWORKCOMPUTESTATUS)
 _LISTAVAILABLEMODELSSTATUS = DESCRIPTOR.enum_types_by_name['ListAvailableModelsStatus']
 ListAvailableModelsStatus = enum_type_wrapper.EnumTypeWrapper(_LISTAVAILABLEMODELSSTATUS)
 NETWORK_COMPUTE_STATUS_UNKNOWN = 0
 NETWORK_COMPUTE_STATUS_SUCCESS = 1
 NETWORK_COMPUTE_STATUS_EXTERNAL_SERVICE_NOT_FOUND = 2
 NETWORK_COMPUTE_STATUS_EXTERNAL_SERVER_ERROR = 3
 NETWORK_COMPUTE_STATUS_ROTATION_ERROR = 4
+NETWORK_COMPUTE_STATUS_CUSTOM_PARAMS_ERROR = 5
 LIST_AVAILABLE_MODELS_STATUS_UNKNOWN = 0
 LIST_AVAILABLE_MODELS_STATUS_SUCCESS = 1
 LIST_AVAILABLE_MODELS_STATUS_EXTERNAL_SERVICE_NOT_FOUND = 2
 LIST_AVAILABLE_MODELS_STATUS_EXTERNAL_SERVER_ERROR = 3
 
 
 _LISTAVAILABLEMODELSREQUEST = DESCRIPTOR.message_types_by_name['ListAvailableModelsRequest']
 _LISTAVAILABLEMODELSRESPONSE = DESCRIPTOR.message_types_by_name['ListAvailableModelsResponse']
+_AVAILABLEMODELS = DESCRIPTOR.message_types_by_name['AvailableModels']
+_MODELDATA = DESCRIPTOR.message_types_by_name['ModelData']
 _MODELLABELS = DESCRIPTOR.message_types_by_name['ModelLabels']
 _NETWORKCOMPUTEREQUEST = DESCRIPTOR.message_types_by_name['NetworkComputeRequest']
 _IMAGESOURCEANDSERVICE = DESCRIPTOR.message_types_by_name['ImageSourceAndService']
+_OUTPUTDATA = DESCRIPTOR.message_types_by_name['OutputData']
+_COMPUTEPARAMETERS = DESCRIPTOR.message_types_by_name['ComputeParameters']
+_NETWORKCOMPUTEINPUTDATABRIDGE = DESCRIPTOR.message_types_by_name['NetworkComputeInputDataBridge']
+_NETWORKCOMPUTEINPUTDATAWORKER = DESCRIPTOR.message_types_by_name['NetworkComputeInputDataWorker']
 _NETWORKCOMPUTEINPUTDATA = DESCRIPTOR.message_types_by_name['NetworkComputeInputData']
 _NETWORKCOMPUTESERVERCONFIGURATION = DESCRIPTOR.message_types_by_name['NetworkComputeServerConfiguration']
 _OUTPUTIMAGE = DESCRIPTOR.message_types_by_name['OutputImage']
+_OUTPUTIMAGESPEC = DESCRIPTOR.message_types_by_name['OutputImageSpec']
 _NETWORKCOMPUTERESPONSE = DESCRIPTOR.message_types_by_name['NetworkComputeResponse']
 _NETWORKCOMPUTERESPONSE_OUTPUTIMAGESENTRY = _NETWORKCOMPUTERESPONSE.nested_types_by_name['OutputImagesEntry']
+_NETWORKCOMPUTERESPONSE_ROIOUTPUTDATAENTRY = _NETWORKCOMPUTERESPONSE.nested_types_by_name['RoiOutputDataEntry']
+_WORKERCOMPUTEREQUEST = DESCRIPTOR.message_types_by_name['WorkerComputeRequest']
+_WORKERCOMPUTERESPONSE = DESCRIPTOR.message_types_by_name['WorkerComputeResponse']
+_WORKERCOMPUTERESPONSE_OUTPUTIMAGESENTRY = _WORKERCOMPUTERESPONSE.nested_types_by_name['OutputImagesEntry']
 _NETWORKCOMPUTEINPUTDATA_ROTATEIMAGE = _NETWORKCOMPUTEINPUTDATA.enum_types_by_name['RotateImage']
 ListAvailableModelsRequest = _reflection.GeneratedProtocolMessageType('ListAvailableModelsRequest', (_message.Message,), {
   'DESCRIPTOR' : _LISTAVAILABLEMODELSREQUEST,
   '__module__' : 'bosdyn.api.network_compute_bridge_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.ListAvailableModelsRequest)
   })
 _sym_db.RegisterMessage(ListAvailableModelsRequest)
@@ -59,14 +72,28 @@
 ListAvailableModelsResponse = _reflection.GeneratedProtocolMessageType('ListAvailableModelsResponse', (_message.Message,), {
   'DESCRIPTOR' : _LISTAVAILABLEMODELSRESPONSE,
   '__module__' : 'bosdyn.api.network_compute_bridge_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.ListAvailableModelsResponse)
   })
 _sym_db.RegisterMessage(ListAvailableModelsResponse)
 
+AvailableModels = _reflection.GeneratedProtocolMessageType('AvailableModels', (_message.Message,), {
+  'DESCRIPTOR' : _AVAILABLEMODELS,
+  '__module__' : 'bosdyn.api.network_compute_bridge_pb2'
+  # @@protoc_insertion_point(class_scope:bosdyn.api.AvailableModels)
+  })
+_sym_db.RegisterMessage(AvailableModels)
+
+ModelData = _reflection.GeneratedProtocolMessageType('ModelData', (_message.Message,), {
+  'DESCRIPTOR' : _MODELDATA,
+  '__module__' : 'bosdyn.api.network_compute_bridge_pb2'
+  # @@protoc_insertion_point(class_scope:bosdyn.api.ModelData)
+  })
+_sym_db.RegisterMessage(ModelData)
+
 ModelLabels = _reflection.GeneratedProtocolMessageType('ModelLabels', (_message.Message,), {
   'DESCRIPTOR' : _MODELLABELS,
   '__module__' : 'bosdyn.api.network_compute_bridge_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.ModelLabels)
   })
 _sym_db.RegisterMessage(ModelLabels)
 
@@ -80,14 +107,42 @@
 ImageSourceAndService = _reflection.GeneratedProtocolMessageType('ImageSourceAndService', (_message.Message,), {
   'DESCRIPTOR' : _IMAGESOURCEANDSERVICE,
   '__module__' : 'bosdyn.api.network_compute_bridge_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.ImageSourceAndService)
   })
 _sym_db.RegisterMessage(ImageSourceAndService)
 
+OutputData = _reflection.GeneratedProtocolMessageType('OutputData', (_message.Message,), {
+  'DESCRIPTOR' : _OUTPUTDATA,
+  '__module__' : 'bosdyn.api.network_compute_bridge_pb2'
+  # @@protoc_insertion_point(class_scope:bosdyn.api.OutputData)
+  })
+_sym_db.RegisterMessage(OutputData)
+
+ComputeParameters = _reflection.GeneratedProtocolMessageType('ComputeParameters', (_message.Message,), {
+  'DESCRIPTOR' : _COMPUTEPARAMETERS,
+  '__module__' : 'bosdyn.api.network_compute_bridge_pb2'
+  # @@protoc_insertion_point(class_scope:bosdyn.api.ComputeParameters)
+  })
+_sym_db.RegisterMessage(ComputeParameters)
+
+NetworkComputeInputDataBridge = _reflection.GeneratedProtocolMessageType('NetworkComputeInputDataBridge', (_message.Message,), {
+  'DESCRIPTOR' : _NETWORKCOMPUTEINPUTDATABRIDGE,
+  '__module__' : 'bosdyn.api.network_compute_bridge_pb2'
+  # @@protoc_insertion_point(class_scope:bosdyn.api.NetworkComputeInputDataBridge)
+  })
+_sym_db.RegisterMessage(NetworkComputeInputDataBridge)
+
+NetworkComputeInputDataWorker = _reflection.GeneratedProtocolMessageType('NetworkComputeInputDataWorker', (_message.Message,), {
+  'DESCRIPTOR' : _NETWORKCOMPUTEINPUTDATAWORKER,
+  '__module__' : 'bosdyn.api.network_compute_bridge_pb2'
+  # @@protoc_insertion_point(class_scope:bosdyn.api.NetworkComputeInputDataWorker)
+  })
+_sym_db.RegisterMessage(NetworkComputeInputDataWorker)
+
 NetworkComputeInputData = _reflection.GeneratedProtocolMessageType('NetworkComputeInputData', (_message.Message,), {
   'DESCRIPTOR' : _NETWORKCOMPUTEINPUTDATA,
   '__module__' : 'bosdyn.api.network_compute_bridge_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.NetworkComputeInputData)
   })
 _sym_db.RegisterMessage(NetworkComputeInputData)
 
@@ -101,55 +156,136 @@
 OutputImage = _reflection.GeneratedProtocolMessageType('OutputImage', (_message.Message,), {
   'DESCRIPTOR' : _OUTPUTIMAGE,
   '__module__' : 'bosdyn.api.network_compute_bridge_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.OutputImage)
   })
 _sym_db.RegisterMessage(OutputImage)
 
+OutputImageSpec = _reflection.GeneratedProtocolMessageType('OutputImageSpec', (_message.Message,), {
+  'DESCRIPTOR' : _OUTPUTIMAGESPEC,
+  '__module__' : 'bosdyn.api.network_compute_bridge_pb2'
+  # @@protoc_insertion_point(class_scope:bosdyn.api.OutputImageSpec)
+  })
+_sym_db.RegisterMessage(OutputImageSpec)
+
 NetworkComputeResponse = _reflection.GeneratedProtocolMessageType('NetworkComputeResponse', (_message.Message,), {
 
   'OutputImagesEntry' : _reflection.GeneratedProtocolMessageType('OutputImagesEntry', (_message.Message,), {
     'DESCRIPTOR' : _NETWORKCOMPUTERESPONSE_OUTPUTIMAGESENTRY,
     '__module__' : 'bosdyn.api.network_compute_bridge_pb2'
     # @@protoc_insertion_point(class_scope:bosdyn.api.NetworkComputeResponse.OutputImagesEntry)
     })
   ,
+
+  'RoiOutputDataEntry' : _reflection.GeneratedProtocolMessageType('RoiOutputDataEntry', (_message.Message,), {
+    'DESCRIPTOR' : _NETWORKCOMPUTERESPONSE_ROIOUTPUTDATAENTRY,
+    '__module__' : 'bosdyn.api.network_compute_bridge_pb2'
+    # @@protoc_insertion_point(class_scope:bosdyn.api.NetworkComputeResponse.RoiOutputDataEntry)
+    })
+  ,
   'DESCRIPTOR' : _NETWORKCOMPUTERESPONSE,
   '__module__' : 'bosdyn.api.network_compute_bridge_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.NetworkComputeResponse)
   })
 _sym_db.RegisterMessage(NetworkComputeResponse)
 _sym_db.RegisterMessage(NetworkComputeResponse.OutputImagesEntry)
+_sym_db.RegisterMessage(NetworkComputeResponse.RoiOutputDataEntry)
+
+WorkerComputeRequest = _reflection.GeneratedProtocolMessageType('WorkerComputeRequest', (_message.Message,), {
+  'DESCRIPTOR' : _WORKERCOMPUTEREQUEST,
+  '__module__' : 'bosdyn.api.network_compute_bridge_pb2'
+  # @@protoc_insertion_point(class_scope:bosdyn.api.WorkerComputeRequest)
+  })
+_sym_db.RegisterMessage(WorkerComputeRequest)
+
+WorkerComputeResponse = _reflection.GeneratedProtocolMessageType('WorkerComputeResponse', (_message.Message,), {
+
+  'OutputImagesEntry' : _reflection.GeneratedProtocolMessageType('OutputImagesEntry', (_message.Message,), {
+    'DESCRIPTOR' : _WORKERCOMPUTERESPONSE_OUTPUTIMAGESENTRY,
+    '__module__' : 'bosdyn.api.network_compute_bridge_pb2'
+    # @@protoc_insertion_point(class_scope:bosdyn.api.WorkerComputeResponse.OutputImagesEntry)
+    })
+  ,
+  'DESCRIPTOR' : _WORKERCOMPUTERESPONSE,
+  '__module__' : 'bosdyn.api.network_compute_bridge_pb2'
+  # @@protoc_insertion_point(class_scope:bosdyn.api.WorkerComputeResponse)
+  })
+_sym_db.RegisterMessage(WorkerComputeResponse)
+_sym_db.RegisterMessage(WorkerComputeResponse.OutputImagesEntry)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'B\031NetworkComputeBridgeProto'
+  _LISTAVAILABLEMODELSRESPONSE.fields_by_name['available_models']._options = None
+  _LISTAVAILABLEMODELSRESPONSE.fields_by_name['available_models']._serialized_options = b'\030\001'
+  _LISTAVAILABLEMODELSRESPONSE.fields_by_name['labels']._options = None
+  _LISTAVAILABLEMODELSRESPONSE.fields_by_name['labels']._serialized_options = b'\030\001'
+  _NETWORKCOMPUTEREQUEST.fields_by_name['input_data']._options = None
+  _NETWORKCOMPUTEREQUEST.fields_by_name['input_data']._serialized_options = b'\030\001'
+  _OUTPUTDATA._options = None
+  _OUTPUTDATA._serialized_options = b'\030\001'
+  _NETWORKCOMPUTEINPUTDATA._options = None
+  _NETWORKCOMPUTEINPUTDATA._serialized_options = b'\030\001'
   _NETWORKCOMPUTERESPONSE_OUTPUTIMAGESENTRY._options = None
   _NETWORKCOMPUTERESPONSE_OUTPUTIMAGESENTRY._serialized_options = b'8\001'
-  _NETWORKCOMPUTESTATUS._serialized_start=2171
-  _NETWORKCOMPUTESTATUS._serialized_end=2413
-  _LISTAVAILABLEMODELSSTATUS._serialized_start=2416
-  _LISTAVAILABLEMODELSSTATUS._serialized_end=2644
-  _LISTAVAILABLEMODELSREQUEST._serialized_start=218
-  _LISTAVAILABLEMODELSREQUEST._serialized_end=359
-  _LISTAVAILABLEMODELSRESPONSE._serialized_start=362
-  _LISTAVAILABLEMODELSRESPONSE._serialized_end=557
-  _MODELLABELS._serialized_start=559
-  _MODELLABELS._serialized_end=618
-  _NETWORKCOMPUTEREQUEST._serialized_start=621
-  _NETWORKCOMPUTEREQUEST._serialized_end=814
-  _IMAGESOURCEANDSERVICE._serialized_start=817
-  _IMAGESOURCEANDSERVICE._serialized_end=954
-  _NETWORKCOMPUTEINPUTDATA._serialized_start=957
-  _NETWORKCOMPUTEINPUTDATA._serialized_end=1402
-  _NETWORKCOMPUTEINPUTDATA_ROTATEIMAGE._serialized_start=1249
-  _NETWORKCOMPUTEINPUTDATA_ROTATEIMAGE._serialized_end=1387
-  _NETWORKCOMPUTESERVERCONFIGURATION._serialized_start=1404
-  _NETWORKCOMPUTESERVERCONFIGURATION._serialized_end=1473
-  _OUTPUTIMAGE._serialized_start=1476
-  _OUTPUTIMAGE._serialized_end=1676
-  _NETWORKCOMPUTERESPONSE._serialized_start=1679
-  _NETWORKCOMPUTERESPONSE._serialized_end=2168
-  _NETWORKCOMPUTERESPONSE_OUTPUTIMAGESENTRY._serialized_start=2092
-  _NETWORKCOMPUTERESPONSE_OUTPUTIMAGESENTRY._serialized_end=2168
+  _NETWORKCOMPUTERESPONSE_ROIOUTPUTDATAENTRY._options = None
+  _NETWORKCOMPUTERESPONSE_ROIOUTPUTDATAENTRY._serialized_options = b'8\001'
+  _NETWORKCOMPUTERESPONSE.fields_by_name['image_response']._options = None
+  _NETWORKCOMPUTERESPONSE.fields_by_name['image_response']._serialized_options = b'\030\001'
+  _NETWORKCOMPUTERESPONSE.fields_by_name['image_rotation_angle']._options = None
+  _NETWORKCOMPUTERESPONSE.fields_by_name['image_rotation_angle']._serialized_options = b'\030\001'
+  _NETWORKCOMPUTERESPONSE.fields_by_name['alert_data']._options = None
+  _NETWORKCOMPUTERESPONSE.fields_by_name['alert_data']._serialized_options = b'\030\001'
+  _NETWORKCOMPUTERESPONSE.fields_by_name['roi_output_data']._options = None
+  _NETWORKCOMPUTERESPONSE.fields_by_name['roi_output_data']._serialized_options = b'\030\001'
+  _WORKERCOMPUTERESPONSE_OUTPUTIMAGESENTRY._options = None
+  _WORKERCOMPUTERESPONSE_OUTPUTIMAGESENTRY._serialized_options = b'8\001'
+  _NETWORKCOMPUTESTATUS._serialized_start=4119
+  _NETWORKCOMPUTESTATUS._serialized_end=4409
+  _LISTAVAILABLEMODELSSTATUS._serialized_start=4412
+  _LISTAVAILABLEMODELSSTATUS._serialized_end=4640
+  _LISTAVAILABLEMODELSREQUEST._serialized_start=258
+  _LISTAVAILABLEMODELSREQUEST._serialized_end=399
+  _LISTAVAILABLEMODELSRESPONSE._serialized_start=402
+  _LISTAVAILABLEMODELSRESPONSE._serialized_end=650
+  _AVAILABLEMODELS._serialized_start=652
+  _AVAILABLEMODELS._serialized_end=706
+  _MODELDATA._serialized_start=709
+  _MODELDATA._serialized_end=873
+  _MODELLABELS._serialized_start=875
+  _MODELLABELS._serialized_end=934
+  _NETWORKCOMPUTEREQUEST._serialized_start=937
+  _NETWORKCOMPUTEREQUEST._serialized_end=1217
+  _IMAGESOURCEANDSERVICE._serialized_start=1220
+  _IMAGESOURCEANDSERVICE._serialized_end=1357
+  _OUTPUTDATA._serialized_start=1360
+  _OUTPUTDATA._serialized_end=1554
+  _COMPUTEPARAMETERS._serialized_start=1557
+  _COMPUTEPARAMETERS._serialized_end=1745
+  _NETWORKCOMPUTEINPUTDATABRIDGE._serialized_start=1748
+  _NETWORKCOMPUTEINPUTDATABRIDGE._serialized_end=1901
+  _NETWORKCOMPUTEINPUTDATAWORKER._serialized_start=1904
+  _NETWORKCOMPUTEINPUTDATAWORKER._serialized_end=2037
+  _NETWORKCOMPUTEINPUTDATA._serialized_start=2040
+  _NETWORKCOMPUTEINPUTDATA._serialized_end=2495
+  _NETWORKCOMPUTEINPUTDATA_ROTATEIMAGE._serialized_start=2332
+  _NETWORKCOMPUTEINPUTDATA_ROTATEIMAGE._serialized_end=2470
+  _NETWORKCOMPUTESERVERCONFIGURATION._serialized_start=2497
+  _NETWORKCOMPUTESERVERCONFIGURATION._serialized_end=2566
+  _OUTPUTIMAGE._serialized_start=2569
+  _OUTPUTIMAGE._serialized_end=2769
+  _OUTPUTIMAGESPEC._serialized_start=2771
+  _OUTPUTIMAGESPEC._serialized_end=2815
+  _NETWORKCOMPUTERESPONSE._serialized_start=2818
+  _NETWORKCOMPUTERESPONSE._serialized_end=3599
+  _NETWORKCOMPUTERESPONSE_OUTPUTIMAGESENTRY._serialized_start=3445
+  _NETWORKCOMPUTERESPONSE_OUTPUTIMAGESENTRY._serialized_end=3521
+  _NETWORKCOMPUTERESPONSE_ROIOUTPUTDATAENTRY._serialized_start=3523
+  _NETWORKCOMPUTERESPONSE_ROIOUTPUTDATAENTRY._serialized_end=3599
+  _WORKERCOMPUTEREQUEST._serialized_start=3602
+  _WORKERCOMPUTEREQUEST._serialized_end=3730
+  _WORKERCOMPUTERESPONSE._serialized_start=3733
+  _WORKERCOMPUTERESPONSE._serialized_end=4116
+  _WORKERCOMPUTERESPONSE_OUTPUTIMAGESENTRY._serialized_start=3445
+  _WORKERCOMPUTERESPONSE_OUTPUTIMAGESENTRY._serialized_end=3521
 # @@protoc_insertion_point(module_scope)
```

## bosdyn/api/network_compute_bridge_service_pb2.py

```diff
@@ -11,21 +11,23 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from bosdyn.api import network_compute_bridge_pb2 as bosdyn_dot_api_dot_network__compute__bridge__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n/bosdyn/api/network_compute_bridge_service.proto\x12\nbosdyn.api\x1a\'bosdyn/api/network_compute_bridge.proto2\xdb\x01\n\x14NetworkComputeBridge\x12Y\n\x0eNetworkCompute\x12!.bosdyn.api.NetworkComputeRequest\x1a\".bosdyn.api.NetworkComputeResponse\"\x00\x12h\n\x13ListAvailableModels\x12&.bosdyn.api.ListAvailableModelsRequest\x1a\'.bosdyn.api.ListAvailableModelsResponse\"\x00\x32\xe1\x01\n\x1aNetworkComputeBridgeWorker\x12Y\n\x0eNetworkCompute\x12!.bosdyn.api.NetworkComputeRequest\x1a\".bosdyn.api.NetworkComputeResponse\"\x00\x12h\n\x13ListAvailableModels\x12&.bosdyn.api.ListAvailableModelsRequest\x1a\'.bosdyn.api.ListAvailableModelsResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n/bosdyn/api/network_compute_bridge_service.proto\x12\nbosdyn.api\x1a\'bosdyn/api/network_compute_bridge.proto2\xdb\x01\n\x14NetworkComputeBridge\x12Y\n\x0eNetworkCompute\x12!.bosdyn.api.NetworkComputeRequest\x1a\".bosdyn.api.NetworkComputeResponse\"\x00\x12h\n\x13ListAvailableModels\x12&.bosdyn.api.ListAvailableModelsRequest\x1a\'.bosdyn.api.ListAvailableModelsResponse\"\x00\x32\xbc\x02\n\x1aNetworkComputeBridgeWorker\x12\\\n\x0eNetworkCompute\x12!.bosdyn.api.NetworkComputeRequest\x1a\".bosdyn.api.NetworkComputeResponse\"\x03\x88\x02\x01\x12V\n\rWorkerCompute\x12 .bosdyn.api.WorkerComputeRequest\x1a!.bosdyn.api.WorkerComputeResponse\"\x00\x12h\n\x13ListAvailableModels\x12&.bosdyn.api.ListAvailableModelsRequest\x1a\'.bosdyn.api.ListAvailableModelsResponse\"\x00\x62\x06proto3')
 
 
 
 _NETWORKCOMPUTEBRIDGE = DESCRIPTOR.services_by_name['NetworkComputeBridge']
 _NETWORKCOMPUTEBRIDGEWORKER = DESCRIPTOR.services_by_name['NetworkComputeBridgeWorker']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
+  _NETWORKCOMPUTEBRIDGEWORKER.methods_by_name['NetworkCompute']._options = None
+  _NETWORKCOMPUTEBRIDGEWORKER.methods_by_name['NetworkCompute']._serialized_options = b'\210\002\001'
   _NETWORKCOMPUTEBRIDGE._serialized_start=105
   _NETWORKCOMPUTEBRIDGE._serialized_end=324
   _NETWORKCOMPUTEBRIDGEWORKER._serialized_start=327
-  _NETWORKCOMPUTEBRIDGEWORKER._serialized_end=552
+  _NETWORKCOMPUTEBRIDGEWORKER._serialized_end=643
 # @@protoc_insertion_point(module_scope)
```

## bosdyn/api/network_compute_bridge_service_pb2_grpc.py

```diff
@@ -115,14 +115,19 @@
             channel: A grpc.Channel.
         """
         self.NetworkCompute = channel.unary_unary(
                 '/bosdyn.api.NetworkComputeBridgeWorker/NetworkCompute',
                 request_serializer=bosdyn_dot_api_dot_network__compute__bridge__pb2.NetworkComputeRequest.SerializeToString,
                 response_deserializer=bosdyn_dot_api_dot_network__compute__bridge__pb2.NetworkComputeResponse.FromString,
                 )
+        self.WorkerCompute = channel.unary_unary(
+                '/bosdyn.api.NetworkComputeBridgeWorker/WorkerCompute',
+                request_serializer=bosdyn_dot_api_dot_network__compute__bridge__pb2.WorkerComputeRequest.SerializeToString,
+                response_deserializer=bosdyn_dot_api_dot_network__compute__bridge__pb2.WorkerComputeResponse.FromString,
+                )
         self.ListAvailableModels = channel.unary_unary(
                 '/bosdyn.api.NetworkComputeBridgeWorker/ListAvailableModels',
                 request_serializer=bosdyn_dot_api_dot_network__compute__bridge__pb2.ListAvailableModelsRequest.SerializeToString,
                 response_deserializer=bosdyn_dot_api_dot_network__compute__bridge__pb2.ListAvailableModelsResponse.FromString,
                 )
 
 
@@ -134,28 +139,39 @@
 
     def NetworkCompute(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def WorkerCompute(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def ListAvailableModels(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_NetworkComputeBridgeWorkerServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'NetworkCompute': grpc.unary_unary_rpc_method_handler(
                     servicer.NetworkCompute,
                     request_deserializer=bosdyn_dot_api_dot_network__compute__bridge__pb2.NetworkComputeRequest.FromString,
                     response_serializer=bosdyn_dot_api_dot_network__compute__bridge__pb2.NetworkComputeResponse.SerializeToString,
             ),
+            'WorkerCompute': grpc.unary_unary_rpc_method_handler(
+                    servicer.WorkerCompute,
+                    request_deserializer=bosdyn_dot_api_dot_network__compute__bridge__pb2.WorkerComputeRequest.FromString,
+                    response_serializer=bosdyn_dot_api_dot_network__compute__bridge__pb2.WorkerComputeResponse.SerializeToString,
+            ),
             'ListAvailableModels': grpc.unary_unary_rpc_method_handler(
                     servicer.ListAvailableModels,
                     request_deserializer=bosdyn_dot_api_dot_network__compute__bridge__pb2.ListAvailableModelsRequest.FromString,
                     response_serializer=bosdyn_dot_api_dot_network__compute__bridge__pb2.ListAvailableModelsResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
@@ -184,14 +200,31 @@
         return grpc.experimental.unary_unary(request, target, '/bosdyn.api.NetworkComputeBridgeWorker/NetworkCompute',
             bosdyn_dot_api_dot_network__compute__bridge__pb2.NetworkComputeRequest.SerializeToString,
             bosdyn_dot_api_dot_network__compute__bridge__pb2.NetworkComputeResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def WorkerCompute(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/bosdyn.api.NetworkComputeBridgeWorker/WorkerCompute',
+            bosdyn_dot_api_dot_network__compute__bridge__pb2.WorkerComputeRequest.SerializeToString,
+            bosdyn_dot_api_dot_network__compute__bridge__pb2.WorkerComputeResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def ListAvailableModels(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

## bosdyn/api/payload_pb2.py

```diff
@@ -14,15 +14,15 @@
 
 
 from bosdyn.api import geometry_pb2 as bosdyn_dot_api_dot_geometry__pb2
 from bosdyn.api import header_pb2 as bosdyn_dot_api_dot_header__pb2
 from bosdyn.api import robot_id_pb2 as bosdyn_dot_api_dot_robot__id__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18\x62osdyn/api/payload.proto\x12\nbosdyn.api\x1a\x19\x62osdyn/api/geometry.proto\x1a\x17\x62osdyn/api/header.proto\x1a\x19\x62osdyn/api/robot_id.proto\"\xe4\x03\n\x07Payload\x12\x0c\n\x04GUID\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x14\n\x0clabel_prefix\x18\t \x03(\t\x12\x15\n\ris_authorized\x18\x04 \x01(\x08\x12\x12\n\nis_enabled\x18\x05 \x01(\x08\x12\x1d\n\x15is_noncompute_payload\x18\x06 \x01(\x08\x12,\n\x07version\x18\x0c \x01(\x0b\x32\x1b.bosdyn.api.SoftwareVersion\x12/\n\x12\x62ody_tform_payload\x18\x07 \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\x12\x30\n\x13mount_tform_payload\x18\x08 \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\x12\x34\n\x10mount_frame_name\x18\r \x01(\x0e\x32\x1a.bosdyn.api.MountFrameName\x12G\n\x16mass_volume_properties\x18\n \x01(\x0b\x32\'.bosdyn.api.PayloadMassVolumeProperties\x12\x38\n\x15preset_configurations\x18\x0b \x03(\x0b\x32\x19.bosdyn.api.PayloadPreset\"\x80\x02\n\rPayloadPreset\x12\x13\n\x0bpreset_name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x30\n\x13mount_tform_payload\x18\x03 \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\x12\x34\n\x10mount_frame_name\x18\x06 \x01(\x0e\x32\x1a.bosdyn.api.MountFrameName\x12G\n\x16mass_volume_properties\x18\x04 \x01(\x0b\x32\'.bosdyn.api.PayloadMassVolumeProperties\x12\x14\n\x0clabel_prefix\x18\x05 \x03(\t\"\xf1\x01\n\x1bPayloadMassVolumeProperties\x12\x12\n\ntotal_mass\x18\x02 \x01(\x02\x12,\n\x12\x63om_pos_rt_payload\x18\x03 \x01(\x0b\x32\x10.bosdyn.api.Vec3\x12\x30\n\nmoi_tensor\x18\x04 \x01(\x0b\x32\x1c.bosdyn.api.MomentOfIntertia\x12/\n\x0c\x62ounding_box\x18\x05 \x03(\x0b\x32\x19.bosdyn.api.Box3WithFrame\x12-\n\x0cjoint_limits\x18\x06 \x03(\x0b\x32\x17.bosdyn.api.JointLimits\"Z\n\x10MomentOfIntertia\x12\n\n\x02xx\x18\x02 \x01(\x02\x12\n\n\x02yy\x18\x03 \x01(\x02\x12\n\n\x02zz\x18\x04 \x01(\x02\x12\n\n\x02xy\x18\x05 \x01(\x02\x12\n\n\x02xz\x18\x06 \x01(\x02\x12\n\n\x02yz\x18\x07 \x01(\x02\"4\n\x0bJointLimits\x12\r\n\x05label\x18\x02 \x01(\t\x12\n\n\x02hy\x18\x03 \x03(\x02\x12\n\n\x02hx\x18\x04 \x03(\x02\"@\n\x13ListPayloadsRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"i\n\x14ListPayloadsResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12%\n\x08payloads\x18\x02 \x03(\x0b\x32\x13.bosdyn.api.Payload*}\n\x0eMountFrameName\x12\x17\n\x13MOUNT_FRAME_UNKNOWN\x10\x00\x12\x1c\n\x18MOUNT_FRAME_BODY_PAYLOAD\x10\x01\x12\x1f\n\x1bMOUNT_FRAME_GRIPPER_PAYLOAD\x10\x02\x12\x13\n\x0fMOUNT_FRAME_WR1\x10\x03\x42\x0e\x42\x0cPayloadProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18\x62osdyn/api/payload.proto\x12\nbosdyn.api\x1a\x19\x62osdyn/api/geometry.proto\x1a\x17\x62osdyn/api/header.proto\x1a\x19\x62osdyn/api/robot_id.proto\"\xad\x04\n\x07Payload\x12\x0c\n\x04GUID\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12\x14\n\x0clabel_prefix\x18\t \x03(\t\x12\x15\n\ris_authorized\x18\x04 \x01(\x08\x12\x12\n\nis_enabled\x18\x05 \x01(\x08\x12\x1d\n\x15is_noncompute_payload\x18\x06 \x01(\x08\x12,\n\x07version\x18\x0c \x01(\x0b\x32\x1b.bosdyn.api.SoftwareVersion\x12/\n\x12\x62ody_tform_payload\x18\x07 \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\x12\x30\n\x13mount_tform_payload\x18\x08 \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\x12\x34\n\x10mount_frame_name\x18\r \x01(\x0e\x32\x1a.bosdyn.api.MountFrameName\x12\x1d\n\x15liveness_timeout_secs\x18\x0f \x01(\x01\x12\x14\n\x0cipv4_address\x18\x10 \x01(\t\x12\x12\n\nlink_speed\x18\x11 \x01(\x05\x12G\n\x16mass_volume_properties\x18\n \x01(\x0b\x32\'.bosdyn.api.PayloadMassVolumeProperties\x12\x38\n\x15preset_configurations\x18\x0b \x03(\x0b\x32\x19.bosdyn.api.PayloadPreset\"\x80\x02\n\rPayloadPreset\x12\x13\n\x0bpreset_name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x30\n\x13mount_tform_payload\x18\x03 \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\x12\x34\n\x10mount_frame_name\x18\x06 \x01(\x0e\x32\x1a.bosdyn.api.MountFrameName\x12G\n\x16mass_volume_properties\x18\x04 \x01(\x0b\x32\'.bosdyn.api.PayloadMassVolumeProperties\x12\x14\n\x0clabel_prefix\x18\x05 \x03(\t\"\xf1\x01\n\x1bPayloadMassVolumeProperties\x12\x12\n\ntotal_mass\x18\x02 \x01(\x02\x12,\n\x12\x63om_pos_rt_payload\x18\x03 \x01(\x0b\x32\x10.bosdyn.api.Vec3\x12\x30\n\nmoi_tensor\x18\x04 \x01(\x0b\x32\x1c.bosdyn.api.MomentOfIntertia\x12/\n\x0c\x62ounding_box\x18\x05 \x03(\x0b\x32\x19.bosdyn.api.Box3WithFrame\x12-\n\x0cjoint_limits\x18\x06 \x03(\x0b\x32\x17.bosdyn.api.JointLimits\"Z\n\x10MomentOfIntertia\x12\n\n\x02xx\x18\x02 \x01(\x02\x12\n\n\x02yy\x18\x03 \x01(\x02\x12\n\n\x02zz\x18\x04 \x01(\x02\x12\n\n\x02xy\x18\x05 \x01(\x02\x12\n\n\x02xz\x18\x06 \x01(\x02\x12\n\n\x02yz\x18\x07 \x01(\x02\"4\n\x0bJointLimits\x12\r\n\x05label\x18\x02 \x01(\t\x12\n\n\x02hy\x18\x03 \x03(\x02\x12\n\n\x02hx\x18\x04 \x03(\x02\"@\n\x13ListPayloadsRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"i\n\x14ListPayloadsResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12%\n\x08payloads\x18\x02 \x03(\x0b\x32\x13.bosdyn.api.Payload*}\n\x0eMountFrameName\x12\x17\n\x13MOUNT_FRAME_UNKNOWN\x10\x00\x12\x1c\n\x18MOUNT_FRAME_BODY_PAYLOAD\x10\x01\x12\x1f\n\x1bMOUNT_FRAME_GRIPPER_PAYLOAD\x10\x02\x12\x13\n\x0fMOUNT_FRAME_WR1\x10\x03\x42\x0e\x42\x0cPayloadProtob\x06proto3')
 
 _MOUNTFRAMENAME = DESCRIPTOR.enum_types_by_name['MountFrameName']
 MountFrameName = enum_type_wrapper.EnumTypeWrapper(_MOUNTFRAMENAME)
 MOUNT_FRAME_UNKNOWN = 0
 MOUNT_FRAME_BODY_PAYLOAD = 1
 MOUNT_FRAME_GRIPPER_PAYLOAD = 2
 MOUNT_FRAME_WR1 = 3
@@ -84,24 +84,24 @@
   })
 _sym_db.RegisterMessage(ListPayloadsResponse)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'B\014PayloadProto'
-  _MOUNTFRAMENAME._serialized_start=1428
-  _MOUNTFRAMENAME._serialized_end=1553
+  _MOUNTFRAMENAME._serialized_start=1501
+  _MOUNTFRAMENAME._serialized_end=1626
   _PAYLOAD._serialized_start=120
-  _PAYLOAD._serialized_end=604
-  _PAYLOADPRESET._serialized_start=607
-  _PAYLOADPRESET._serialized_end=863
-  _PAYLOADMASSVOLUMEPROPERTIES._serialized_start=866
-  _PAYLOADMASSVOLUMEPROPERTIES._serialized_end=1107
-  _MOMENTOFINTERTIA._serialized_start=1109
-  _MOMENTOFINTERTIA._serialized_end=1199
-  _JOINTLIMITS._serialized_start=1201
-  _JOINTLIMITS._serialized_end=1253
-  _LISTPAYLOADSREQUEST._serialized_start=1255
-  _LISTPAYLOADSREQUEST._serialized_end=1319
-  _LISTPAYLOADSRESPONSE._serialized_start=1321
-  _LISTPAYLOADSRESPONSE._serialized_end=1426
+  _PAYLOAD._serialized_end=677
+  _PAYLOADPRESET._serialized_start=680
+  _PAYLOADPRESET._serialized_end=936
+  _PAYLOADMASSVOLUMEPROPERTIES._serialized_start=939
+  _PAYLOADMASSVOLUMEPROPERTIES._serialized_end=1180
+  _MOMENTOFINTERTIA._serialized_start=1182
+  _MOMENTOFINTERTIA._serialized_end=1272
+  _JOINTLIMITS._serialized_start=1274
+  _JOINTLIMITS._serialized_end=1326
+  _LISTPAYLOADSREQUEST._serialized_start=1328
+  _LISTPAYLOADSREQUEST._serialized_end=1392
+  _LISTPAYLOADSRESPONSE._serialized_start=1394
+  _LISTPAYLOADSRESPONSE._serialized_end=1499
 # @@protoc_insertion_point(module_scope)
```

## bosdyn/api/power_pb2.py

```diff
@@ -17,15 +17,15 @@
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from bosdyn.api import header_pb2 as bosdyn_dot_api_dot_header__pb2
 from bosdyn.api import lease_pb2 as bosdyn_dot_api_dot_lease__pb2
 from bosdyn.api import license_pb2 as bosdyn_dot_api_dot_license__pb2
 from bosdyn.api import robot_state_pb2 as bosdyn_dot_api_dot_robot__state__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16\x62osdyn/api/power.proto\x12\nbosdyn.api\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x17\x62osdyn/api/header.proto\x1a\x16\x62osdyn/api/lease.proto\x1a\x18\x62osdyn/api/license.proto\x1a\x1c\x62osdyn/api/robot_state.proto\"\xbd\x03\n\x13PowerCommandRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12 \n\x05lease\x18\x02 \x01(\x0b\x32\x11.bosdyn.api.Lease\x12\x38\n\x07request\x18\x03 \x01(\x0e\x32\'.bosdyn.api.PowerCommandRequest.Request\"\x9e\x02\n\x07Request\x12\x13\n\x0fREQUEST_UNKNOWN\x10\x00\x12\x13\n\x0bREQUEST_OFF\x10\x01\x1a\x02\x08\x01\x12\x12\n\nREQUEST_ON\x10\x02\x1a\x02\x08\x01\x12\x16\n\x12REQUEST_OFF_MOTORS\x10\x01\x12\x15\n\x11REQUEST_ON_MOTORS\x10\x02\x12\x15\n\x11REQUEST_OFF_ROBOT\x10\x03\x12\x17\n\x13REQUEST_CYCLE_ROBOT\x10\x04\x12\x1d\n\x19REQUEST_OFF_PAYLOAD_PORTS\x10\x05\x12\x1c\n\x18REQUEST_ON_PAYLOAD_PORTS\x10\x06\x12\x1a\n\x16REQUEST_OFF_WIFI_RADIO\x10\x07\x12\x19\n\x15REQUEST_ON_WIFI_RADIO\x10\x08\x1a\x02\x10\x01\"\xac\x02\n\x14PowerCommandResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x34\n\x10lease_use_result\x18\x02 \x01(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12.\n\x06status\x18\x03 \x01(\x0e\x32\x1e.bosdyn.api.PowerCommandStatus\x12\x18\n\x10power_command_id\x18\x04 \x01(\r\x12\x36\n\x0elicense_status\x18\x05 \x01(\x0e\x32\x1e.bosdyn.api.LicenseInfo.Status\x12\x30\n\x0f\x62locking_faults\x18\x06 \x03(\x0b\x32\x17.bosdyn.api.SystemFault\"b\n\x1bPowerCommandFeedbackRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x18\n\x10power_command_id\x18\x02 \x01(\r\"\xac\x01\n\x1cPowerCommandFeedbackResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12.\n\x06status\x18\x02 \x01(\x0e\x32\x1e.bosdyn.api.PowerCommandStatus\x12\x30\n\x0f\x62locking_faults\x18\x03 \x03(\x0b\x32\x17.bosdyn.api.SystemFault\"\xa9\x01\n\x16\x46\x61nPowerCommandRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12 \n\x05lease\x18\x02 \x01(\x0b\x32\x11.bosdyn.api.Lease\x12\x15\n\rpercent_power\x18\x03 \x01(\x05\x12+\n\x08\x64uration\x18\x04 \x01(\x0b\x32\x19.google.protobuf.Duration\"\xcf\x02\n\x17\x46\x61nPowerCommandResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x34\n\x10lease_use_result\x18\x02 \x01(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12:\n\x06status\x18\x03 \x01(\x0e\x32*.bosdyn.api.FanPowerCommandResponse.Status\x12\x34\n\x10\x64\x65sired_end_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\ncommand_id\x18\x05 \x01(\r\"L\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1f\n\x1bSTATUS_TEMPERATURE_TOO_HIGH\x10\x02\"_\n\x1e\x46\x61nPowerCommandFeedbackRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x12\n\ncommand_id\x18\x02 \x01(\r\"\x83\x03\n\x1f\x46\x61nPowerCommandFeedbackResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x42\n\x06status\x18\x02 \x01(\x0e\x32\x32.bosdyn.api.FanPowerCommandFeedbackResponse.Status\x12\x34\n\x10\x64\x65sired_end_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x33\n\x0f\x65\x61rly_stop_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x84\x01\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x13\n\x0fSTATUS_COMPLETE\x10\x01\x12\x12\n\x0eSTATUS_RUNNING\x10\x02\x12\x1b\n\x17STATUS_TEMPERATURE_STOP\x10\x03\x12 \n\x1cSTATUS_OVERRIDDEN_BY_COMMAND\x10\x04*\xc8\x02\n\x12PowerCommandStatus\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x16\n\x12STATUS_IN_PROGRESS\x10\x01\x12\x12\n\x0eSTATUS_SUCCESS\x10\x02\x12 \n\x1cSTATUS_SHORE_POWER_CONNECTED\x10\x03\x12\x1a\n\x16STATUS_BATTERY_MISSING\x10\x04\x12\x1e\n\x1aSTATUS_COMMAND_IN_PROGRESS\x10\x05\x12\x13\n\x0fSTATUS_ESTOPPED\x10\x06\x12\x12\n\x0eSTATUS_FAULTED\x10\x07\x12\x19\n\x15STATUS_INTERNAL_ERROR\x10\x08\x12\x18\n\x14STATUS_LICENSE_ERROR\x10\t\x12\x1f\n\x1bINCOMPATIBLE_HARDWARE_ERROR\x10\n\x12\x15\n\x11STATUS_OVERRIDDEN\x10\x0b\x42\x0c\x42\nPowerProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16\x62osdyn/api/power.proto\x12\nbosdyn.api\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x17\x62osdyn/api/header.proto\x1a\x16\x62osdyn/api/lease.proto\x1a\x18\x62osdyn/api/license.proto\x1a\x1c\x62osdyn/api/robot_state.proto\"\xbd\x03\n\x13PowerCommandRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12 \n\x05lease\x18\x02 \x01(\x0b\x32\x11.bosdyn.api.Lease\x12\x38\n\x07request\x18\x03 \x01(\x0e\x32\'.bosdyn.api.PowerCommandRequest.Request\"\x9e\x02\n\x07Request\x12\x13\n\x0fREQUEST_UNKNOWN\x10\x00\x12\x13\n\x0bREQUEST_OFF\x10\x01\x1a\x02\x08\x01\x12\x12\n\nREQUEST_ON\x10\x02\x1a\x02\x08\x01\x12\x16\n\x12REQUEST_OFF_MOTORS\x10\x01\x12\x15\n\x11REQUEST_ON_MOTORS\x10\x02\x12\x15\n\x11REQUEST_OFF_ROBOT\x10\x03\x12\x17\n\x13REQUEST_CYCLE_ROBOT\x10\x04\x12\x1d\n\x19REQUEST_OFF_PAYLOAD_PORTS\x10\x05\x12\x1c\n\x18REQUEST_ON_PAYLOAD_PORTS\x10\x06\x12\x1a\n\x16REQUEST_OFF_WIFI_RADIO\x10\x07\x12\x19\n\x15REQUEST_ON_WIFI_RADIO\x10\x08\x1a\x02\x10\x01\"\xac\x02\n\x14PowerCommandResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x34\n\x10lease_use_result\x18\x02 \x01(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12.\n\x06status\x18\x03 \x01(\x0e\x32\x1e.bosdyn.api.PowerCommandStatus\x12\x18\n\x10power_command_id\x18\x04 \x01(\r\x12\x36\n\x0elicense_status\x18\x05 \x01(\x0e\x32\x1e.bosdyn.api.LicenseInfo.Status\x12\x30\n\x0f\x62locking_faults\x18\x06 \x03(\x0b\x32\x17.bosdyn.api.SystemFault\"b\n\x1bPowerCommandFeedbackRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x18\n\x10power_command_id\x18\x02 \x01(\r\"\xac\x01\n\x1cPowerCommandFeedbackResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12.\n\x06status\x18\x02 \x01(\x0e\x32\x1e.bosdyn.api.PowerCommandStatus\x12\x30\n\x0f\x62locking_faults\x18\x03 \x03(\x0b\x32\x17.bosdyn.api.SystemFault\"\xa9\x01\n\x16\x46\x61nPowerCommandRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12 \n\x05lease\x18\x02 \x01(\x0b\x32\x11.bosdyn.api.Lease\x12\x15\n\rpercent_power\x18\x03 \x01(\x05\x12+\n\x08\x64uration\x18\x04 \x01(\x0b\x32\x19.google.protobuf.Duration\"\xcf\x02\n\x17\x46\x61nPowerCommandResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x34\n\x10lease_use_result\x18\x02 \x01(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12:\n\x06status\x18\x03 \x01(\x0e\x32*.bosdyn.api.FanPowerCommandResponse.Status\x12\x34\n\x10\x64\x65sired_end_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\ncommand_id\x18\x05 \x01(\r\"L\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1f\n\x1bSTATUS_TEMPERATURE_TOO_HIGH\x10\x02\"_\n\x1e\x46\x61nPowerCommandFeedbackRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x12\n\ncommand_id\x18\x02 \x01(\r\"\x83\x03\n\x1f\x46\x61nPowerCommandFeedbackResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x42\n\x06status\x18\x02 \x01(\x0e\x32\x32.bosdyn.api.FanPowerCommandFeedbackResponse.Status\x12\x34\n\x10\x64\x65sired_end_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x33\n\x0f\x65\x61rly_stop_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x84\x01\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x13\n\x0fSTATUS_COMPLETE\x10\x01\x12\x12\n\x0eSTATUS_RUNNING\x10\x02\x12\x1b\n\x17STATUS_TEMPERATURE_STOP\x10\x03\x12 \n\x1cSTATUS_OVERRIDDEN_BY_COMMAND\x10\x04*\xe9\x02\n\x12PowerCommandStatus\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x16\n\x12STATUS_IN_PROGRESS\x10\x01\x12\x12\n\x0eSTATUS_SUCCESS\x10\x02\x12 \n\x1cSTATUS_SHORE_POWER_CONNECTED\x10\x03\x12\x1a\n\x16STATUS_BATTERY_MISSING\x10\x04\x12\x1e\n\x1aSTATUS_COMMAND_IN_PROGRESS\x10\x05\x12\x13\n\x0fSTATUS_ESTOPPED\x10\x06\x12\x12\n\x0eSTATUS_FAULTED\x10\x07\x12\x19\n\x15STATUS_INTERNAL_ERROR\x10\x08\x12\x18\n\x14STATUS_LICENSE_ERROR\x10\t\x12\x1f\n\x1bINCOMPATIBLE_HARDWARE_ERROR\x10\n\x12\x15\n\x11STATUS_OVERRIDDEN\x10\x0b\x12\x1f\n\x1bSTATUS_KEEPALIVE_MOTORS_OFF\x10\x0c\x42\x0c\x42\nPowerProtob\x06proto3')
 
 _POWERCOMMANDSTATUS = DESCRIPTOR.enum_types_by_name['PowerCommandStatus']
 PowerCommandStatus = enum_type_wrapper.EnumTypeWrapper(_POWERCOMMANDSTATUS)
 STATUS_UNKNOWN = 0
 STATUS_IN_PROGRESS = 1
 STATUS_SUCCESS = 2
 STATUS_SHORE_POWER_CONNECTED = 3
@@ -33,14 +33,15 @@
 STATUS_COMMAND_IN_PROGRESS = 5
 STATUS_ESTOPPED = 6
 STATUS_FAULTED = 7
 STATUS_INTERNAL_ERROR = 8
 STATUS_LICENSE_ERROR = 9
 INCOMPATIBLE_HARDWARE_ERROR = 10
 STATUS_OVERRIDDEN = 11
+STATUS_KEEPALIVE_MOTORS_OFF = 12
 
 
 _POWERCOMMANDREQUEST = DESCRIPTOR.message_types_by_name['PowerCommandRequest']
 _POWERCOMMANDRESPONSE = DESCRIPTOR.message_types_by_name['PowerCommandResponse']
 _POWERCOMMANDFEEDBACKREQUEST = DESCRIPTOR.message_types_by_name['PowerCommandFeedbackRequest']
 _POWERCOMMANDFEEDBACKRESPONSE = DESCRIPTOR.message_types_by_name['PowerCommandFeedbackResponse']
 _FANPOWERCOMMANDREQUEST = DESCRIPTOR.message_types_by_name['FanPowerCommandRequest']
@@ -113,15 +114,15 @@
   _POWERCOMMANDREQUEST_REQUEST._options = None
   _POWERCOMMANDREQUEST_REQUEST._serialized_options = b'\020\001'
   _POWERCOMMANDREQUEST_REQUEST.values_by_name["REQUEST_OFF"]._options = None
   _POWERCOMMANDREQUEST_REQUEST.values_by_name["REQUEST_OFF"]._serialized_options = b'\010\001'
   _POWERCOMMANDREQUEST_REQUEST.values_by_name["REQUEST_ON"]._options = None
   _POWERCOMMANDREQUEST_REQUEST.values_by_name["REQUEST_ON"]._serialized_options = b'\010\001'
   _POWERCOMMANDSTATUS._serialized_start=2232
-  _POWERCOMMANDSTATUS._serialized_end=2560
+  _POWERCOMMANDSTATUS._serialized_end=2593
   _POWERCOMMANDREQUEST._serialized_start=209
   _POWERCOMMANDREQUEST._serialized_end=654
   _POWERCOMMANDREQUEST_REQUEST._serialized_start=368
   _POWERCOMMANDREQUEST_REQUEST._serialized_end=654
   _POWERCOMMANDRESPONSE._serialized_start=657
   _POWERCOMMANDRESPONSE._serialized_end=957
   _POWERCOMMANDFEEDBACKREQUEST._serialized_start=959
```

## bosdyn/api/robot_command_pb2.py

```diff
@@ -12,18 +12,19 @@
 _sym_db = _symbol_database.Default()
 
 
 from bosdyn.api import full_body_command_pb2 as bosdyn_dot_api_dot_full__body__command__pb2
 from bosdyn.api import header_pb2 as bosdyn_dot_api_dot_header__pb2
 from bosdyn.api import lease_pb2 as bosdyn_dot_api_dot_lease__pb2
 from bosdyn.api import mobility_command_pb2 as bosdyn_dot_api_dot_mobility__command__pb2
+from bosdyn.api import robot_state_pb2 as bosdyn_dot_api_dot_robot__state__pb2
 from bosdyn.api import synchronized_command_pb2 as bosdyn_dot_api_dot_synchronized__command__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1e\x62osdyn/api/robot_command.proto\x12\nbosdyn.api\x1a\"bosdyn/api/full_body_command.proto\x1a\x17\x62osdyn/api/header.proto\x1a\x16\x62osdyn/api/lease.proto\x1a!bosdyn/api/mobility_command.proto\x1a%bosdyn/api/synchronized_command.proto\"\xe9\x01\n\x0cRobotCommand\x12@\n\x11\x66ull_body_command\x18\x01 \x01(\x0b\x32#.bosdyn.api.FullBodyCommand.RequestH\x00\x12G\n\x14synchronized_command\x18\x03 \x01(\x0b\x32\'.bosdyn.api.SynchronizedCommand.RequestH\x00\x12\x43\n\x10mobility_command\x18\x02 \x01(\x0b\x32#.bosdyn.api.MobilityCommand.RequestB\x02\x18\x01H\x00\x42\t\n\x07\x63ommand\"\xf7\x01\n\x14RobotCommandFeedback\x12\x42\n\x12\x66ull_body_feedback\x18\x02 \x01(\x0b\x32$.bosdyn.api.FullBodyCommand.FeedbackH\x00\x12I\n\x15synchronized_feedback\x18\x03 \x01(\x0b\x32(.bosdyn.api.SynchronizedCommand.FeedbackH\x00\x12\x45\n\x11mobility_feedback\x18\x01 \x01(\x0b\x32$.bosdyn.api.MobilityCommand.FeedbackB\x02\x18\x01H\x00\x42\t\n\x07\x63ommand\"\xa7\x01\n\x13RobotCommandRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12 \n\x05lease\x18\x02 \x01(\x0b\x32\x11.bosdyn.api.Lease\x12)\n\x07\x63ommand\x18\x03 \x01(\x0b\x32\x18.bosdyn.api.RobotCommand\x12\x18\n\x10\x63lock_identifier\x18\x04 \x01(\t\"\xe5\x03\n\x14RobotCommandResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x34\n\x10lease_use_result\x18\x02 \x01(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12\x37\n\x06status\x18\x03 \x01(\x0e\x32\'.bosdyn.api.RobotCommandResponse.Status\x12\x0f\n\x07message\x18\x04 \x01(\t\x12\x18\n\x10robot_command_id\x18\x05 \x01(\r\"\x86\x02\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1a\n\x16STATUS_INVALID_REQUEST\x10\x02\x12\x16\n\x12STATUS_UNSUPPORTED\x10\x03\x12\x16\n\x12STATUS_NO_TIMESYNC\x10\x04\x12\x12\n\x0eSTATUS_EXPIRED\x10\x05\x12\x16\n\x12STATUS_TOO_DISTANT\x10\x06\x12\x19\n\x15STATUS_NOT_POWERED_ON\x10\x07\x12\x19\n\x15STATUS_BEHAVIOR_FAULT\x10\t\x12\x11\n\rSTATUS_DOCKED\x10\n\x12\x18\n\x14STATUS_UNKNOWN_FRAME\x10\x08\"b\n\x1bRobotCommandFeedbackRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x18\n\x10robot_command_id\x18\x02 \x01(\r\"\x9a\x03\n\x1cRobotCommandFeedbackResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x34\n\x10lease_use_result\x18\x05 \x01(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12\x43\n\x06status\x18\x02 \x01(\x0e\x32/.bosdyn.api.RobotCommandFeedbackResponse.StatusB\x02\x18\x01\x12\x13\n\x07message\x18\x03 \x01(\tB\x02\x18\x01\x12\x32\n\x08\x66\x65\x65\x64\x62\x61\x63k\x18\x04 \x01(\x0b\x32 .bosdyn.api.RobotCommandFeedback\"\x89\x01\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x15\n\x11STATUS_PROCESSING\x10\x01\x12\x1d\n\x19STATUS_COMMAND_OVERRIDDEN\x10\x02\x12\x1c\n\x18STATUS_COMMAND_TIMED_OUT\x10\x03\x12\x17\n\x13STATUS_ROBOT_FROZEN\x10\x04\"\x83\x01\n\x19\x43learBehaviorFaultRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12 \n\x05lease\x18\x02 \x01(\x0b\x32\x11.bosdyn.api.Lease\x12\x19\n\x11\x62\x65havior_fault_id\x18\x03 \x01(\r\"\x87\x02\n\x1a\x43learBehaviorFaultResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x34\n\x10lease_use_result\x18\x02 \x01(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12=\n\x06status\x18\x03 \x01(\x0e\x32-.bosdyn.api.ClearBehaviorFaultResponse.Status\"H\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x12\n\x0eSTATUS_CLEARED\x10\x01\x12\x16\n\x12STATUS_NOT_CLEARED\x10\x02\x42\x13\x42\x11RobotCommandProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1e\x62osdyn/api/robot_command.proto\x12\nbosdyn.api\x1a\"bosdyn/api/full_body_command.proto\x1a\x17\x62osdyn/api/header.proto\x1a\x16\x62osdyn/api/lease.proto\x1a!bosdyn/api/mobility_command.proto\x1a\x1c\x62osdyn/api/robot_state.proto\x1a%bosdyn/api/synchronized_command.proto\"\xe9\x01\n\x0cRobotCommand\x12@\n\x11\x66ull_body_command\x18\x01 \x01(\x0b\x32#.bosdyn.api.FullBodyCommand.RequestH\x00\x12G\n\x14synchronized_command\x18\x03 \x01(\x0b\x32\'.bosdyn.api.SynchronizedCommand.RequestH\x00\x12\x43\n\x10mobility_command\x18\x02 \x01(\x0b\x32#.bosdyn.api.MobilityCommand.RequestB\x02\x18\x01H\x00\x42\t\n\x07\x63ommand\"\xf7\x01\n\x14RobotCommandFeedback\x12\x42\n\x12\x66ull_body_feedback\x18\x02 \x01(\x0b\x32$.bosdyn.api.FullBodyCommand.FeedbackH\x00\x12I\n\x15synchronized_feedback\x18\x03 \x01(\x0b\x32(.bosdyn.api.SynchronizedCommand.FeedbackH\x00\x12\x45\n\x11mobility_feedback\x18\x01 \x01(\x0b\x32$.bosdyn.api.MobilityCommand.FeedbackB\x02\x18\x01H\x00\x42\t\n\x07\x63ommand\"\xa7\x01\n\x13RobotCommandRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12 \n\x05lease\x18\x02 \x01(\x0b\x32\x11.bosdyn.api.Lease\x12)\n\x07\x63ommand\x18\x03 \x01(\x0b\x32\x18.bosdyn.api.RobotCommand\x12\x18\n\x10\x63lock_identifier\x18\x04 \x01(\t\"\xe5\x03\n\x14RobotCommandResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x34\n\x10lease_use_result\x18\x02 \x01(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12\x37\n\x06status\x18\x03 \x01(\x0e\x32\'.bosdyn.api.RobotCommandResponse.Status\x12\x0f\n\x07message\x18\x04 \x01(\t\x12\x18\n\x10robot_command_id\x18\x05 \x01(\r\"\x86\x02\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1a\n\x16STATUS_INVALID_REQUEST\x10\x02\x12\x16\n\x12STATUS_UNSUPPORTED\x10\x03\x12\x16\n\x12STATUS_NO_TIMESYNC\x10\x04\x12\x12\n\x0eSTATUS_EXPIRED\x10\x05\x12\x16\n\x12STATUS_TOO_DISTANT\x10\x06\x12\x19\n\x15STATUS_NOT_POWERED_ON\x10\x07\x12\x19\n\x15STATUS_BEHAVIOR_FAULT\x10\t\x12\x11\n\rSTATUS_DOCKED\x10\n\x12\x18\n\x14STATUS_UNKNOWN_FRAME\x10\x08\"b\n\x1bRobotCommandFeedbackRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x18\n\x10robot_command_id\x18\x02 \x01(\r\"\x9e\x03\n\x1cRobotCommandFeedbackResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x34\n\x10lease_use_result\x18\x05 \x01(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12\x43\n\x06status\x18\x02 \x01(\x0e\x32/.bosdyn.api.RobotCommandFeedbackResponse.StatusB\x02\x18\x01\x12\x13\n\x07message\x18\x03 \x01(\tB\x02\x18\x01\x12\x32\n\x08\x66\x65\x65\x64\x62\x61\x63k\x18\x04 \x01(\x0b\x32 .bosdyn.api.RobotCommandFeedback\"\x8d\x01\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x15\n\x11STATUS_PROCESSING\x10\x01\x12\x1d\n\x19STATUS_COMMAND_OVERRIDDEN\x10\x02\x12\x1c\n\x18STATUS_COMMAND_TIMED_OUT\x10\x03\x12\x17\n\x13STATUS_ROBOT_FROZEN\x10\x04\x1a\x02\x18\x01\"\x83\x01\n\x19\x43learBehaviorFaultRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12 \n\x05lease\x18\x02 \x01(\x0b\x32\x11.bosdyn.api.Lease\x12\x19\n\x11\x62\x65havior_fault_id\x18\x03 \x01(\r\"\xf3\x02\n\x1a\x43learBehaviorFaultResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x34\n\x10lease_use_result\x18\x02 \x01(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12=\n\x06status\x18\x03 \x01(\x0e\x32-.bosdyn.api.ClearBehaviorFaultResponse.Status\x12\x31\n\x0e\x62\x65havior_fault\x18\x04 \x01(\x0b\x32\x19.bosdyn.api.BehaviorFault\x12\x37\n\x16\x62locking_system_faults\x18\x05 \x03(\x0b\x32\x17.bosdyn.api.SystemFault\"H\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x12\n\x0eSTATUS_CLEARED\x10\x01\x12\x16\n\x12STATUS_NOT_CLEARED\x10\x02\x42\x13\x42\x11RobotCommandProtob\x06proto3')
 
 
 
 _ROBOTCOMMAND = DESCRIPTOR.message_types_by_name['RobotCommand']
 _ROBOTCOMMANDFEEDBACK = DESCRIPTOR.message_types_by_name['RobotCommandFeedback']
 _ROBOTCOMMANDREQUEST = DESCRIPTOR.message_types_by_name['RobotCommandRequest']
 _ROBOTCOMMANDRESPONSE = DESCRIPTOR.message_types_by_name['RobotCommandResponse']
@@ -94,34 +95,36 @@
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'B\021RobotCommandProto'
   _ROBOTCOMMAND.fields_by_name['mobility_command']._options = None
   _ROBOTCOMMAND.fields_by_name['mobility_command']._serialized_options = b'\030\001'
   _ROBOTCOMMANDFEEDBACK.fields_by_name['mobility_feedback']._options = None
   _ROBOTCOMMANDFEEDBACK.fields_by_name['mobility_feedback']._serialized_options = b'\030\001'
+  _ROBOTCOMMANDFEEDBACKRESPONSE_STATUS._options = None
+  _ROBOTCOMMANDFEEDBACKRESPONSE_STATUS._serialized_options = b'\030\001'
   _ROBOTCOMMANDFEEDBACKRESPONSE.fields_by_name['status']._options = None
   _ROBOTCOMMANDFEEDBACKRESPONSE.fields_by_name['status']._serialized_options = b'\030\001'
   _ROBOTCOMMANDFEEDBACKRESPONSE.fields_by_name['message']._options = None
   _ROBOTCOMMANDFEEDBACKRESPONSE.fields_by_name['message']._serialized_options = b'\030\001'
-  _ROBOTCOMMAND._serialized_start=206
-  _ROBOTCOMMAND._serialized_end=439
-  _ROBOTCOMMANDFEEDBACK._serialized_start=442
-  _ROBOTCOMMANDFEEDBACK._serialized_end=689
-  _ROBOTCOMMANDREQUEST._serialized_start=692
-  _ROBOTCOMMANDREQUEST._serialized_end=859
-  _ROBOTCOMMANDRESPONSE._serialized_start=862
-  _ROBOTCOMMANDRESPONSE._serialized_end=1347
-  _ROBOTCOMMANDRESPONSE_STATUS._serialized_start=1085
-  _ROBOTCOMMANDRESPONSE_STATUS._serialized_end=1347
-  _ROBOTCOMMANDFEEDBACKREQUEST._serialized_start=1349
-  _ROBOTCOMMANDFEEDBACKREQUEST._serialized_end=1447
-  _ROBOTCOMMANDFEEDBACKRESPONSE._serialized_start=1450
-  _ROBOTCOMMANDFEEDBACKRESPONSE._serialized_end=1860
-  _ROBOTCOMMANDFEEDBACKRESPONSE_STATUS._serialized_start=1723
-  _ROBOTCOMMANDFEEDBACKRESPONSE_STATUS._serialized_end=1860
-  _CLEARBEHAVIORFAULTREQUEST._serialized_start=1863
-  _CLEARBEHAVIORFAULTREQUEST._serialized_end=1994
-  _CLEARBEHAVIORFAULTRESPONSE._serialized_start=1997
-  _CLEARBEHAVIORFAULTRESPONSE._serialized_end=2260
-  _CLEARBEHAVIORFAULTRESPONSE_STATUS._serialized_start=2188
-  _CLEARBEHAVIORFAULTRESPONSE_STATUS._serialized_end=2260
+  _ROBOTCOMMAND._serialized_start=236
+  _ROBOTCOMMAND._serialized_end=469
+  _ROBOTCOMMANDFEEDBACK._serialized_start=472
+  _ROBOTCOMMANDFEEDBACK._serialized_end=719
+  _ROBOTCOMMANDREQUEST._serialized_start=722
+  _ROBOTCOMMANDREQUEST._serialized_end=889
+  _ROBOTCOMMANDRESPONSE._serialized_start=892
+  _ROBOTCOMMANDRESPONSE._serialized_end=1377
+  _ROBOTCOMMANDRESPONSE_STATUS._serialized_start=1115
+  _ROBOTCOMMANDRESPONSE_STATUS._serialized_end=1377
+  _ROBOTCOMMANDFEEDBACKREQUEST._serialized_start=1379
+  _ROBOTCOMMANDFEEDBACKREQUEST._serialized_end=1477
+  _ROBOTCOMMANDFEEDBACKRESPONSE._serialized_start=1480
+  _ROBOTCOMMANDFEEDBACKRESPONSE._serialized_end=1894
+  _ROBOTCOMMANDFEEDBACKRESPONSE_STATUS._serialized_start=1753
+  _ROBOTCOMMANDFEEDBACKRESPONSE_STATUS._serialized_end=1894
+  _CLEARBEHAVIORFAULTREQUEST._serialized_start=1897
+  _CLEARBEHAVIORFAULTREQUEST._serialized_end=2028
+  _CLEARBEHAVIORFAULTRESPONSE._serialized_start=2031
+  _CLEARBEHAVIORFAULTRESPONSE._serialized_end=2402
+  _CLEARBEHAVIORFAULTRESPONSE_STATUS._serialized_start=2330
+  _CLEARBEHAVIORFAULTRESPONSE_STATUS._serialized_end=2402
 # @@protoc_insertion_point(module_scope)
```

## bosdyn/api/robot_state_pb2.py

```diff
@@ -17,15 +17,15 @@
 from bosdyn.api import parameter_pb2 as bosdyn_dot_api_dot_parameter__pb2
 from bosdyn.api import service_fault_pb2 as bosdyn_dot_api_dot_service__fault__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1c\x62osdyn/api/robot_state.proto\x12\nbosdyn.api\x1a\x19\x62osdyn/api/geometry.proto\x1a\x17\x62osdyn/api/header.proto\x1a\x1a\x62osdyn/api/parameter.proto\x1a\x1e\x62osdyn/api/service_fault.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\xc6\x01\n\x08Skeleton\x12(\n\x05links\x18\x02 \x03(\x0b\x32\x19.bosdyn.api.Skeleton.Link\x12\x0c\n\x04urdf\x18\x03 \x01(\t\x1a\x81\x01\n\x04Link\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x35\n\tobj_model\x18\x02 \x01(\x0b\x32\".bosdyn.api.Skeleton.Link.ObjModel\x1a\x34\n\x08ObjModel\x12\x11\n\tfile_name\x18\x01 \x01(\t\x12\x15\n\rfile_contents\x18\x02 \x01(\t\"\xfa\x01\n\x15HardwareConfiguration\x12&\n\x08skeleton\x18\x01 \x01(\x0b\x32\x14.bosdyn.api.Skeleton\x12+\n#can_power_command_request_off_robot\x18\x02 \x01(\x08\x12-\n%can_power_command_request_cycle_robot\x18\x03 \x01(\x08\x12/\n\'can_power_command_request_payload_ports\x18\x04 \x01(\x08\x12,\n$can_power_command_request_wifi_radio\x18\x05 \x01(\x08\"\xcb\x04\n\nRobotState\x12+\n\x0bpower_state\x18\x01 \x01(\x0b\x32\x16.bosdyn.api.PowerState\x12\x30\n\x0e\x62\x61ttery_states\x18\x02 \x03(\x0b\x32\x18.bosdyn.api.BatteryState\x12,\n\x0c\x63omms_states\x18\x03 \x03(\x0b\x32\x16.bosdyn.api.CommsState\x12\x38\n\x12system_fault_state\x18\x04 \x01(\x0b\x32\x1c.bosdyn.api.SystemFaultState\x12,\n\x0c\x65stop_states\x18\x05 \x03(\x0b\x32\x16.bosdyn.api.EStopState\x12\x33\n\x0fkinematic_state\x18\x06 \x01(\x0b\x32\x1a.bosdyn.api.KinematicState\x12<\n\x14\x62\x65havior_fault_state\x18\x07 \x01(\x0b\x32\x1e.bosdyn.api.BehaviorFaultState\x12)\n\nfoot_state\x18\x08 \x03(\x0b\x32\x15.bosdyn.api.FootState\x12\x37\n\x11manipulator_state\x18\x0b \x01(\x0b\x32\x1c.bosdyn.api.ManipulatorState\x12:\n\x13service_fault_state\x18\n \x01(\x0b\x32\x1d.bosdyn.api.ServiceFaultState\x12/\n\rterrain_state\x18\x0c \x01(\x0b\x32\x18.bosdyn.api.TerrainStateJ\x04\x08\t\x10\n\"\xb3\x0b\n\nPowerState\x12-\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x41\n\x11motor_power_state\x18\x02 \x01(\x0e\x32&.bosdyn.api.PowerState.MotorPowerState\x12\x41\n\x11shore_power_state\x18\x03 \x01(\x0e\x32&.bosdyn.api.PowerState.ShorePowerState\x12\x41\n\x11robot_power_state\x18\x06 \x01(\x0e\x32&.bosdyn.api.PowerState.RobotPowerState\x12P\n\x19payload_ports_power_state\x18\x07 \x01(\x0e\x32-.bosdyn.api.PowerState.PayloadPortsPowerState\x12J\n\x16wifi_radio_power_state\x18\t \x01(\x0e\x32*.bosdyn.api.PowerState.WifiRadioPowerState\x12\x42\n\x1clocomotion_charge_percentage\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12?\n\x1clocomotion_estimated_runtime\x18\x05 \x01(\x0b\x32\x19.google.protobuf.Duration\"\xd5\x02\n\x0fMotorPowerState\x12\x15\n\rSTATE_UNKNOWN\x10\x00\x1a\x02\x08\x01\x12\x1d\n\x19MOTOR_POWER_STATE_UNKNOWN\x10\x00\x12\x11\n\tSTATE_OFF\x10\x01\x1a\x02\x08\x01\x12\x19\n\x15MOTOR_POWER_STATE_OFF\x10\x01\x12\x10\n\x08STATE_ON\x10\x02\x1a\x02\x08\x01\x12\x18\n\x14MOTOR_POWER_STATE_ON\x10\x02\x12\x19\n\x11STATE_POWERING_ON\x10\x03\x1a\x02\x08\x01\x12!\n\x1dMOTOR_POWER_STATE_POWERING_ON\x10\x03\x12\x1a\n\x12STATE_POWERING_OFF\x10\x04\x1a\x02\x08\x01\x12\"\n\x1eMOTOR_POWER_STATE_POWERING_OFF\x10\x04\x12\x13\n\x0bSTATE_ERROR\x10\x05\x1a\x02\x08\x01\x12\x1b\n\x17MOTOR_POWER_STATE_ERROR\x10\x05\x1a\x02\x10\x01\"\xc9\x01\n\x0fShorePowerState\x12!\n\x19STATE_UNKNOWN_SHORE_POWER\x10\x00\x1a\x02\x08\x01\x12\x1d\n\x19SHORE_POWER_STATE_UNKNOWN\x10\x00\x12\x1c\n\x14STATE_ON_SHORE_POWER\x10\x01\x1a\x02\x08\x01\x12\x18\n\x14SHORE_POWER_STATE_ON\x10\x01\x12\x1d\n\x15STATE_OFF_SHORE_POWER\x10\x02\x1a\x02\x08\x01\x12\x19\n\x15SHORE_POWER_STATE_OFF\x10\x02\x1a\x02\x10\x01\"e\n\x0fRobotPowerState\x12\x1d\n\x19ROBOT_POWER_STATE_UNKNOWN\x10\x00\x12\x18\n\x14ROBOT_POWER_STATE_ON\x10\x01\x12\x19\n\x15ROBOT_POWER_STATE_OFF\x10\x02\"\x84\x01\n\x16PayloadPortsPowerState\x12%\n!PAYLOAD_PORTS_POWER_STATE_UNKNOWN\x10\x00\x12 \n\x1cPAYLOAD_PORTS_POWER_STATE_ON\x10\x01\x12!\n\x1dPAYLOAD_PORTS_POWER_STATE_OFF\x10\x02\"x\n\x13WifiRadioPowerState\x12\"\n\x1eWIFI_RADIO_POWER_STATE_UNKNOWN\x10\x00\x12\x1d\n\x19WIFI_RADIO_POWER_STATE_ON\x10\x01\x12\x1e\n\x1aWIFI_RADIO_POWER_STATE_OFF\x10\x02\"\x86\x02\n\x10SystemFaultState\x12\'\n\x06\x66\x61ults\x18\x01 \x03(\x0b\x32\x17.bosdyn.api.SystemFault\x12\x32\n\x11historical_faults\x18\x02 \x03(\x0b\x32\x17.bosdyn.api.SystemFault\x12@\n\naggregated\x18\x03 \x03(\x0b\x32,.bosdyn.api.SystemFaultState.AggregatedEntry\x1aS\n\x0f\x41ggregatedEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0e\x32 .bosdyn.api.SystemFault.Severity:\x02\x38\x01\"\xd6\x02\n\x0bSystemFault\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x33\n\x0fonset_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x08\x64uration\x18\x03 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x0c\n\x04\x63ode\x18\x04 \x01(\x05\x12\x0b\n\x03uid\x18\x08 \x01(\x04\x12\x15\n\rerror_message\x18\x05 \x01(\t\x12\x12\n\nattributes\x18\x06 \x03(\t\x12\x32\n\x08severity\x18\x07 \x01(\x0e\x32 .bosdyn.api.SystemFault.Severity\"]\n\x08Severity\x12\x14\n\x10SEVERITY_UNKNOWN\x10\x00\x12\x11\n\rSEVERITY_INFO\x10\x01\x12\x11\n\rSEVERITY_WARN\x10\x02\x12\x15\n\x11SEVERITY_CRITICAL\x10\x03\"\xc4\x02\n\nEStopState\x12-\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0c\n\x04name\x18\x02 \x01(\t\x12)\n\x04type\x18\x03 \x01(\x0e\x32\x1b.bosdyn.api.EStopState.Type\x12+\n\x05state\x18\x04 \x01(\x0e\x32\x1c.bosdyn.api.EStopState.State\x12\x19\n\x11state_description\x18\x05 \x01(\t\">\n\x04Type\x12\x10\n\x0cTYPE_UNKNOWN\x10\x00\x12\x11\n\rTYPE_HARDWARE\x10\x01\x12\x11\n\rTYPE_SOFTWARE\x10\x02\"F\n\x05State\x12\x11\n\rSTATE_UNKNOWN\x10\x00\x12\x12\n\x0eSTATE_ESTOPPED\x10\x01\x12\x16\n\x12STATE_NOT_ESTOPPED\x10\x02\"\xd8\x03\n\x0c\x42\x61tteryState\x12-\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\nidentifier\x18\x02 \x01(\t\x12\x37\n\x11\x63harge_percentage\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x34\n\x11\x65stimated_runtime\x18\x04 \x01(\x0b\x32\x19.google.protobuf.Duration\x12-\n\x07\x63urrent\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12-\n\x07voltage\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x14\n\x0ctemperatures\x18\x07 \x03(\x01\x12/\n\x06status\x18\x08 \x01(\x0e\x32\x1f.bosdyn.api.BatteryState.Status\"q\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x12\n\x0eSTATUS_MISSING\x10\x01\x12\x13\n\x0fSTATUS_CHARGING\x10\x02\x12\x16\n\x12STATUS_DISCHARGING\x10\x03\x12\x12\n\x0eSTATUS_BOOTING\x10\x04\"\xdd\x02\n\x0eKinematicState\x12,\n\x0cjoint_states\x18\x02 \x03(\x0b\x32\x16.bosdyn.api.JointState\x12\x39\n\x15\x61\x63quisition_timestamp\x18\x1e \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x13transforms_snapshot\x18\x1f \x01(\x0b\x32\x1d.bosdyn.api.FrameTreeSnapshot\x12;\n\x1avelocity_of_body_in_vision\x18\x08 \x01(\x0b\x32\x17.bosdyn.api.SE3Velocity\x12\x39\n\x18velocity_of_body_in_odom\x18\x0c \x01(\x0b\x32\x17.bosdyn.api.SE3VelocityJ\x04\x08\x01\x10\x02J\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07J\x04\x08\t\x10\nJ\x04\x08\n\x10\x0bJ\x04\x08\x0b\x10\x0c\"\xda\x01\n\nJointState\x12\x0c\n\x04name\x18\x01 \x01(\t\x12.\n\x08position\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12.\n\x08velocity\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x32\n\x0c\x61\x63\x63\x65leration\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12*\n\x04load\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"?\n\x12\x42\x65haviorFaultState\x12)\n\x06\x66\x61ults\x18\x01 \x03(\x0b\x32\x19.bosdyn.api.BehaviorFault\"\xe6\x02\n\rBehaviorFault\x12\x19\n\x11\x62\x65havior_fault_id\x18\x01 \x01(\r\x12\x33\n\x0fonset_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\x05\x63\x61use\x18\x03 \x01(\x0e\x32\x1f.bosdyn.api.BehaviorFault.Cause\x12\x30\n\x06status\x18\x04 \x01(\x0e\x32 .bosdyn.api.BehaviorFault.Status\"W\n\x05\x43\x61use\x12\x11\n\rCAUSE_UNKNOWN\x10\x00\x12\x0e\n\nCAUSE_FALL\x10\x01\x12\x12\n\x0e\x43\x41USE_HARDWARE\x10\x02\x12\x17\n\x13\x43\x41USE_LEASE_TIMEOUT\x10\x03\"J\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x14\n\x10STATUS_CLEARABLE\x10\x01\x12\x16\n\x12STATUS_UNCLEARABLE\x10\x02\"e\n\x0cRobotMetrics\x12-\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12&\n\x07metrics\x18\x02 \x03(\x0b\x32\x15.bosdyn.api.Parameter\"q\n\nCommsState\x12-\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\nwifi_state\x18\x02 \x01(\x0b\x32\x15.bosdyn.api.WiFiStateH\x00\x42\x07\n\x05state\"\x8e\x01\n\tWiFiState\x12\x30\n\x0c\x63urrent_mode\x18\x01 \x01(\x0e\x32\x1a.bosdyn.api.WiFiState.Mode\x12\r\n\x05\x65ssid\x18\x02 \x01(\t\"@\n\x04Mode\x12\x10\n\x0cMODE_UNKNOWN\x10\x00\x12\x15\n\x11MODE_ACCESS_POINT\x10\x01\x12\x0f\n\x0bMODE_CLIENT\x10\x02\"\xa8\x04\n\tFootState\x12/\n\x15\x66oot_position_rt_body\x18\x01 \x01(\x0b\x32\x10.bosdyn.api.Vec3\x12.\n\x07\x63ontact\x18\x02 \x01(\x0e\x32\x1d.bosdyn.api.FootState.Contact\x12\x33\n\x07terrain\x18\x03 \x01(\x0b\x32\".bosdyn.api.FootState.TerrainState\x1a\xc0\x02\n\x0cTerrainState\x12\x15\n\rground_mu_est\x18\x01 \x01(\x01\x12\x12\n\nframe_name\x18\x02 \x01(\t\x12\x35\n\x1b\x66oot_slip_distance_rt_frame\x18\x03 \x01(\x0b\x32\x10.bosdyn.api.Vec3\x12\x35\n\x1b\x66oot_slip_velocity_rt_frame\x18\x04 \x01(\x0b\x32\x10.bosdyn.api.Vec3\x12\x38\n\x1eground_contact_normal_rt_frame\x18\x05 \x01(\x0b\x32\x10.bosdyn.api.Vec3\x12.\n&visual_surface_ground_penetration_mean\x18\x06 \x01(\x01\x12-\n%visual_surface_ground_penetration_std\x18\x07 \x01(\x01\"B\n\x07\x43ontact\x12\x13\n\x0f\x43ONTACT_UNKNOWN\x10\x00\x12\x10\n\x0c\x43ONTACT_MADE\x10\x01\x12\x10\n\x0c\x43ONTACT_LOST\x10\x02\"\x98\x05\n\x10ManipulatorState\x12\x1f\n\x17gripper_open_percentage\x18\x0c \x01(\x01\x12\x1f\n\x17is_gripper_holding_item\x18\x06 \x01(\x08\x12>\n$estimated_end_effector_force_in_hand\x18\r \x01(\x0b\x32\x10.bosdyn.api.Vec3\x12:\n\nstow_state\x18\t \x01(\x0e\x32&.bosdyn.api.ManipulatorState.StowState\x12;\n\x1avelocity_of_hand_in_vision\x18\x0e \x01(\x0b\x32\x17.bosdyn.api.SE3Velocity\x12\x39\n\x18velocity_of_hand_in_odom\x18\x0f \x01(\x0b\x32\x17.bosdyn.api.SE3Velocity\x12<\n\x0b\x63\x61rry_state\x18\x10 \x01(\x0e\x32\'.bosdyn.api.ManipulatorState.CarryState\"P\n\tStowState\x12\x15\n\x11STOWSTATE_UNKNOWN\x10\x00\x12\x14\n\x10STOWSTATE_STOWED\x10\x01\x12\x16\n\x12STOWSTATE_DEPLOYED\x10\x02\"\x87\x01\n\nCarryState\x12\x17\n\x13\x43\x41RRY_STATE_UNKNOWN\x10\x00\x12\x1d\n\x19\x43\x41RRY_STATE_NOT_CARRIABLE\x10\x01\x12\x19\n\x15\x43\x41RRY_STATE_CARRIABLE\x10\x02\x12&\n\"CARRY_STATE_CARRIABLE_AND_STOWABLE\x10\x03J\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x07\x10\x08J\x04\x08\x08\x10\tJ\x04\x08\n\x10\x0bJ\x04\x08\x0b\x10\x0c\"\x8b\x02\n\x11ServiceFaultState\x12(\n\x06\x66\x61ults\x18\x01 \x03(\x0b\x32\x18.bosdyn.api.ServiceFault\x12\x33\n\x11historical_faults\x18\x02 \x03(\x0b\x32\x18.bosdyn.api.ServiceFault\x12\x41\n\naggregated\x18\x03 \x03(\x0b\x32-.bosdyn.api.ServiceFaultState.AggregatedEntry\x1aT\n\x0f\x41ggregatedEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x30\n\x05value\x18\x02 \x01(\x0e\x32!.bosdyn.api.ServiceFault.Severity:\x02\x38\x01\"(\n\x0cTerrainState\x12\x18\n\x10is_unsafe_to_sit\x18\x01 \x01(\x08\">\n\x11RobotStateRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"m\n\x12RobotStateResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12+\n\x0brobot_state\x18\x02 \x01(\x0b\x32\x16.bosdyn.api.RobotState\"@\n\x13RobotMetricsRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"s\n\x14RobotMetricsResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12/\n\rrobot_metrics\x18\x02 \x01(\x0b\x32\x18.bosdyn.api.RobotMetrics\"N\n!RobotHardwareConfigurationRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"\x93\x01\n\"RobotHardwareConfigurationResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x41\n\x16hardware_configuration\x18\x02 \x01(\x0b\x32!.bosdyn.api.HardwareConfiguration\"U\n\x15RobotLinkModelRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x11\n\tlink_name\x18\x02 \x01(\t\"|\n\x16RobotLinkModelResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x36\n\nlink_model\x18\x02 \x01(\x0b\x32\".bosdyn.api.Skeleton.Link.ObjModel\"\x99\x04\n\x12RobotImpairedState\x12\x46\n\x0fimpaired_status\x18\x01 \x01(\x0e\x32-.bosdyn.api.RobotImpairedState.ImpairedStatus\x12.\n\rsystem_faults\x18\x02 \x03(\x0b\x32\x17.bosdyn.api.SystemFault\x12\x30\n\x0eservice_faults\x18\x03 \x03(\x0b\x32\x18.bosdyn.api.ServiceFault\x12\x32\n\x0f\x62\x65havior_faults\x18\x04 \x03(\x0b\x32\x19.bosdyn.api.BehaviorFault\"\xa4\x02\n\x0eImpairedStatus\x12\x1b\n\x17IMPAIRED_STATUS_UNKNOWN\x10\x00\x12\x16\n\x12IMPAIRED_STATUS_OK\x10\x01\x12!\n\x1dIMPAIRED_STATUS_NO_ROBOT_DATA\x10\x02\x12 \n\x1cIMPAIRED_STATUS_SYSTEM_FAULT\x10\x03\x12\"\n\x1eIMPAIRED_STATUS_NO_MOTOR_POWER\x10\x04\x12-\n)IMPAIRED_STATUS_REMOTE_CLOUDS_NOT_WORKING\x10\x05\x12!\n\x1dIMPAIRED_STATUS_SERVICE_FAULT\x10\x06\x12\"\n\x1eIMPAIRED_STATUS_BEHAVIOR_FAULT\x10\x07\x42\x11\x42\x0fRobotStateProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1c\x62osdyn/api/robot_state.proto\x12\nbosdyn.api\x1a\x19\x62osdyn/api/geometry.proto\x1a\x17\x62osdyn/api/header.proto\x1a\x1a\x62osdyn/api/parameter.proto\x1a\x1e\x62osdyn/api/service_fault.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\xc6\x01\n\x08Skeleton\x12(\n\x05links\x18\x02 \x03(\x0b\x32\x19.bosdyn.api.Skeleton.Link\x12\x0c\n\x04urdf\x18\x03 \x01(\t\x1a\x81\x01\n\x04Link\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x35\n\tobj_model\x18\x02 \x01(\x0b\x32\".bosdyn.api.Skeleton.Link.ObjModel\x1a\x34\n\x08ObjModel\x12\x11\n\tfile_name\x18\x01 \x01(\t\x12\x15\n\rfile_contents\x18\x02 \x01(\t\"\x9b\x02\n\x15HardwareConfiguration\x12&\n\x08skeleton\x18\x01 \x01(\x0b\x32\x14.bosdyn.api.Skeleton\x12+\n#can_power_command_request_off_robot\x18\x02 \x01(\x08\x12-\n%can_power_command_request_cycle_robot\x18\x03 \x01(\x08\x12/\n\'can_power_command_request_payload_ports\x18\x04 \x01(\x08\x12,\n$can_power_command_request_wifi_radio\x18\x05 \x01(\x08\x12\x1f\n\x17has_audio_visual_system\x18\x07 \x01(\x08\"\xcb\x04\n\nRobotState\x12+\n\x0bpower_state\x18\x01 \x01(\x0b\x32\x16.bosdyn.api.PowerState\x12\x30\n\x0e\x62\x61ttery_states\x18\x02 \x03(\x0b\x32\x18.bosdyn.api.BatteryState\x12,\n\x0c\x63omms_states\x18\x03 \x03(\x0b\x32\x16.bosdyn.api.CommsState\x12\x38\n\x12system_fault_state\x18\x04 \x01(\x0b\x32\x1c.bosdyn.api.SystemFaultState\x12,\n\x0c\x65stop_states\x18\x05 \x03(\x0b\x32\x16.bosdyn.api.EStopState\x12\x33\n\x0fkinematic_state\x18\x06 \x01(\x0b\x32\x1a.bosdyn.api.KinematicState\x12<\n\x14\x62\x65havior_fault_state\x18\x07 \x01(\x0b\x32\x1e.bosdyn.api.BehaviorFaultState\x12)\n\nfoot_state\x18\x08 \x03(\x0b\x32\x15.bosdyn.api.FootState\x12\x37\n\x11manipulator_state\x18\x0b \x01(\x0b\x32\x1c.bosdyn.api.ManipulatorState\x12:\n\x13service_fault_state\x18\n \x01(\x0b\x32\x1d.bosdyn.api.ServiceFaultState\x12/\n\rterrain_state\x18\x0c \x01(\x0b\x32\x18.bosdyn.api.TerrainStateJ\x04\x08\t\x10\n\"\xb3\x0b\n\nPowerState\x12-\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x41\n\x11motor_power_state\x18\x02 \x01(\x0e\x32&.bosdyn.api.PowerState.MotorPowerState\x12\x41\n\x11shore_power_state\x18\x03 \x01(\x0e\x32&.bosdyn.api.PowerState.ShorePowerState\x12\x41\n\x11robot_power_state\x18\x06 \x01(\x0e\x32&.bosdyn.api.PowerState.RobotPowerState\x12P\n\x19payload_ports_power_state\x18\x07 \x01(\x0e\x32-.bosdyn.api.PowerState.PayloadPortsPowerState\x12J\n\x16wifi_radio_power_state\x18\t \x01(\x0e\x32*.bosdyn.api.PowerState.WifiRadioPowerState\x12\x42\n\x1clocomotion_charge_percentage\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12?\n\x1clocomotion_estimated_runtime\x18\x05 \x01(\x0b\x32\x19.google.protobuf.Duration\"\xd5\x02\n\x0fMotorPowerState\x12\x15\n\rSTATE_UNKNOWN\x10\x00\x1a\x02\x08\x01\x12\x1d\n\x19MOTOR_POWER_STATE_UNKNOWN\x10\x00\x12\x11\n\tSTATE_OFF\x10\x01\x1a\x02\x08\x01\x12\x19\n\x15MOTOR_POWER_STATE_OFF\x10\x01\x12\x10\n\x08STATE_ON\x10\x02\x1a\x02\x08\x01\x12\x18\n\x14MOTOR_POWER_STATE_ON\x10\x02\x12\x19\n\x11STATE_POWERING_ON\x10\x03\x1a\x02\x08\x01\x12!\n\x1dMOTOR_POWER_STATE_POWERING_ON\x10\x03\x12\x1a\n\x12STATE_POWERING_OFF\x10\x04\x1a\x02\x08\x01\x12\"\n\x1eMOTOR_POWER_STATE_POWERING_OFF\x10\x04\x12\x13\n\x0bSTATE_ERROR\x10\x05\x1a\x02\x08\x01\x12\x1b\n\x17MOTOR_POWER_STATE_ERROR\x10\x05\x1a\x02\x10\x01\"\xc9\x01\n\x0fShorePowerState\x12!\n\x19STATE_UNKNOWN_SHORE_POWER\x10\x00\x1a\x02\x08\x01\x12\x1d\n\x19SHORE_POWER_STATE_UNKNOWN\x10\x00\x12\x1c\n\x14STATE_ON_SHORE_POWER\x10\x01\x1a\x02\x08\x01\x12\x18\n\x14SHORE_POWER_STATE_ON\x10\x01\x12\x1d\n\x15STATE_OFF_SHORE_POWER\x10\x02\x1a\x02\x08\x01\x12\x19\n\x15SHORE_POWER_STATE_OFF\x10\x02\x1a\x02\x10\x01\"e\n\x0fRobotPowerState\x12\x1d\n\x19ROBOT_POWER_STATE_UNKNOWN\x10\x00\x12\x18\n\x14ROBOT_POWER_STATE_ON\x10\x01\x12\x19\n\x15ROBOT_POWER_STATE_OFF\x10\x02\"\x84\x01\n\x16PayloadPortsPowerState\x12%\n!PAYLOAD_PORTS_POWER_STATE_UNKNOWN\x10\x00\x12 \n\x1cPAYLOAD_PORTS_POWER_STATE_ON\x10\x01\x12!\n\x1dPAYLOAD_PORTS_POWER_STATE_OFF\x10\x02\"x\n\x13WifiRadioPowerState\x12\"\n\x1eWIFI_RADIO_POWER_STATE_UNKNOWN\x10\x00\x12\x1d\n\x19WIFI_RADIO_POWER_STATE_ON\x10\x01\x12\x1e\n\x1aWIFI_RADIO_POWER_STATE_OFF\x10\x02\"\x86\x02\n\x10SystemFaultState\x12\'\n\x06\x66\x61ults\x18\x01 \x03(\x0b\x32\x17.bosdyn.api.SystemFault\x12\x32\n\x11historical_faults\x18\x02 \x03(\x0b\x32\x17.bosdyn.api.SystemFault\x12@\n\naggregated\x18\x03 \x03(\x0b\x32,.bosdyn.api.SystemFaultState.AggregatedEntry\x1aS\n\x0f\x41ggregatedEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0e\x32 .bosdyn.api.SystemFault.Severity:\x02\x38\x01\"\xd6\x02\n\x0bSystemFault\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x33\n\x0fonset_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x08\x64uration\x18\x03 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x0c\n\x04\x63ode\x18\x04 \x01(\x05\x12\x0b\n\x03uid\x18\x08 \x01(\x04\x12\x15\n\rerror_message\x18\x05 \x01(\t\x12\x12\n\nattributes\x18\x06 \x03(\t\x12\x32\n\x08severity\x18\x07 \x01(\x0e\x32 .bosdyn.api.SystemFault.Severity\"]\n\x08Severity\x12\x14\n\x10SEVERITY_UNKNOWN\x10\x00\x12\x11\n\rSEVERITY_INFO\x10\x01\x12\x11\n\rSEVERITY_WARN\x10\x02\x12\x15\n\x11SEVERITY_CRITICAL\x10\x03\"\xc4\x02\n\nEStopState\x12-\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0c\n\x04name\x18\x02 \x01(\t\x12)\n\x04type\x18\x03 \x01(\x0e\x32\x1b.bosdyn.api.EStopState.Type\x12+\n\x05state\x18\x04 \x01(\x0e\x32\x1c.bosdyn.api.EStopState.State\x12\x19\n\x11state_description\x18\x05 \x01(\t\">\n\x04Type\x12\x10\n\x0cTYPE_UNKNOWN\x10\x00\x12\x11\n\rTYPE_HARDWARE\x10\x01\x12\x11\n\rTYPE_SOFTWARE\x10\x02\"F\n\x05State\x12\x11\n\rSTATE_UNKNOWN\x10\x00\x12\x12\n\x0eSTATE_ESTOPPED\x10\x01\x12\x16\n\x12STATE_NOT_ESTOPPED\x10\x02\"\xd8\x03\n\x0c\x42\x61tteryState\x12-\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x12\n\nidentifier\x18\x02 \x01(\t\x12\x37\n\x11\x63harge_percentage\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x34\n\x11\x65stimated_runtime\x18\x04 \x01(\x0b\x32\x19.google.protobuf.Duration\x12-\n\x07\x63urrent\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12-\n\x07voltage\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x14\n\x0ctemperatures\x18\x07 \x03(\x01\x12/\n\x06status\x18\x08 \x01(\x0e\x32\x1f.bosdyn.api.BatteryState.Status\"q\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x12\n\x0eSTATUS_MISSING\x10\x01\x12\x13\n\x0fSTATUS_CHARGING\x10\x02\x12\x16\n\x12STATUS_DISCHARGING\x10\x03\x12\x12\n\x0eSTATUS_BOOTING\x10\x04\"\xdd\x02\n\x0eKinematicState\x12,\n\x0cjoint_states\x18\x02 \x03(\x0b\x32\x16.bosdyn.api.JointState\x12\x39\n\x15\x61\x63quisition_timestamp\x18\x1e \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x13transforms_snapshot\x18\x1f \x01(\x0b\x32\x1d.bosdyn.api.FrameTreeSnapshot\x12;\n\x1avelocity_of_body_in_vision\x18\x08 \x01(\x0b\x32\x17.bosdyn.api.SE3Velocity\x12\x39\n\x18velocity_of_body_in_odom\x18\x0c \x01(\x0b\x32\x17.bosdyn.api.SE3VelocityJ\x04\x08\x01\x10\x02J\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x06\x10\x07J\x04\x08\t\x10\nJ\x04\x08\n\x10\x0bJ\x04\x08\x0b\x10\x0c\"\xda\x01\n\nJointState\x12\x0c\n\x04name\x18\x01 \x01(\t\x12.\n\x08position\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12.\n\x08velocity\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x32\n\x0c\x61\x63\x63\x65leration\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12*\n\x04load\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"?\n\x12\x42\x65haviorFaultState\x12)\n\x06\x66\x61ults\x18\x01 \x03(\x0b\x32\x19.bosdyn.api.BehaviorFault\"\xe6\x02\n\rBehaviorFault\x12\x19\n\x11\x62\x65havior_fault_id\x18\x01 \x01(\r\x12\x33\n\x0fonset_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\x05\x63\x61use\x18\x03 \x01(\x0e\x32\x1f.bosdyn.api.BehaviorFault.Cause\x12\x30\n\x06status\x18\x04 \x01(\x0e\x32 .bosdyn.api.BehaviorFault.Status\"W\n\x05\x43\x61use\x12\x11\n\rCAUSE_UNKNOWN\x10\x00\x12\x0e\n\nCAUSE_FALL\x10\x01\x12\x12\n\x0e\x43\x41USE_HARDWARE\x10\x02\x12\x17\n\x13\x43\x41USE_LEASE_TIMEOUT\x10\x03\"J\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x14\n\x10STATUS_CLEARABLE\x10\x01\x12\x16\n\x12STATUS_UNCLEARABLE\x10\x02\"e\n\x0cRobotMetrics\x12-\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12&\n\x07metrics\x18\x02 \x03(\x0b\x32\x15.bosdyn.api.Parameter\"q\n\nCommsState\x12-\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\nwifi_state\x18\x02 \x01(\x0b\x32\x15.bosdyn.api.WiFiStateH\x00\x42\x07\n\x05state\"\x8e\x01\n\tWiFiState\x12\x30\n\x0c\x63urrent_mode\x18\x01 \x01(\x0e\x32\x1a.bosdyn.api.WiFiState.Mode\x12\r\n\x05\x65ssid\x18\x02 \x01(\t\"@\n\x04Mode\x12\x10\n\x0cMODE_UNKNOWN\x10\x00\x12\x15\n\x11MODE_ACCESS_POINT\x10\x01\x12\x0f\n\x0bMODE_CLIENT\x10\x02\"\xa8\x04\n\tFootState\x12/\n\x15\x66oot_position_rt_body\x18\x01 \x01(\x0b\x32\x10.bosdyn.api.Vec3\x12.\n\x07\x63ontact\x18\x02 \x01(\x0e\x32\x1d.bosdyn.api.FootState.Contact\x12\x33\n\x07terrain\x18\x03 \x01(\x0b\x32\".bosdyn.api.FootState.TerrainState\x1a\xc0\x02\n\x0cTerrainState\x12\x15\n\rground_mu_est\x18\x01 \x01(\x01\x12\x12\n\nframe_name\x18\x02 \x01(\t\x12\x35\n\x1b\x66oot_slip_distance_rt_frame\x18\x03 \x01(\x0b\x32\x10.bosdyn.api.Vec3\x12\x35\n\x1b\x66oot_slip_velocity_rt_frame\x18\x04 \x01(\x0b\x32\x10.bosdyn.api.Vec3\x12\x38\n\x1eground_contact_normal_rt_frame\x18\x05 \x01(\x0b\x32\x10.bosdyn.api.Vec3\x12.\n&visual_surface_ground_penetration_mean\x18\x06 \x01(\x01\x12-\n%visual_surface_ground_penetration_std\x18\x07 \x01(\x01\"B\n\x07\x43ontact\x12\x13\n\x0f\x43ONTACT_UNKNOWN\x10\x00\x12\x10\n\x0c\x43ONTACT_MADE\x10\x01\x12\x10\n\x0c\x43ONTACT_LOST\x10\x02\"\x98\x05\n\x10ManipulatorState\x12\x1f\n\x17gripper_open_percentage\x18\x0c \x01(\x01\x12\x1f\n\x17is_gripper_holding_item\x18\x06 \x01(\x08\x12>\n$estimated_end_effector_force_in_hand\x18\r \x01(\x0b\x32\x10.bosdyn.api.Vec3\x12:\n\nstow_state\x18\t \x01(\x0e\x32&.bosdyn.api.ManipulatorState.StowState\x12;\n\x1avelocity_of_hand_in_vision\x18\x0e \x01(\x0b\x32\x17.bosdyn.api.SE3Velocity\x12\x39\n\x18velocity_of_hand_in_odom\x18\x0f \x01(\x0b\x32\x17.bosdyn.api.SE3Velocity\x12<\n\x0b\x63\x61rry_state\x18\x10 \x01(\x0e\x32\'.bosdyn.api.ManipulatorState.CarryState\"P\n\tStowState\x12\x15\n\x11STOWSTATE_UNKNOWN\x10\x00\x12\x14\n\x10STOWSTATE_STOWED\x10\x01\x12\x16\n\x12STOWSTATE_DEPLOYED\x10\x02\"\x87\x01\n\nCarryState\x12\x17\n\x13\x43\x41RRY_STATE_UNKNOWN\x10\x00\x12\x1d\n\x19\x43\x41RRY_STATE_NOT_CARRIABLE\x10\x01\x12\x19\n\x15\x43\x41RRY_STATE_CARRIABLE\x10\x02\x12&\n\"CARRY_STATE_CARRIABLE_AND_STOWABLE\x10\x03J\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x07\x10\x08J\x04\x08\x08\x10\tJ\x04\x08\n\x10\x0bJ\x04\x08\x0b\x10\x0c\"\x8b\x02\n\x11ServiceFaultState\x12(\n\x06\x66\x61ults\x18\x01 \x03(\x0b\x32\x18.bosdyn.api.ServiceFault\x12\x33\n\x11historical_faults\x18\x02 \x03(\x0b\x32\x18.bosdyn.api.ServiceFault\x12\x41\n\naggregated\x18\x03 \x03(\x0b\x32-.bosdyn.api.ServiceFaultState.AggregatedEntry\x1aT\n\x0f\x41ggregatedEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x30\n\x05value\x18\x02 \x01(\x0e\x32!.bosdyn.api.ServiceFault.Severity:\x02\x38\x01\"(\n\x0cTerrainState\x12\x18\n\x10is_unsafe_to_sit\x18\x01 \x01(\x08\">\n\x11RobotStateRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"m\n\x12RobotStateResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12+\n\x0brobot_state\x18\x02 \x01(\x0b\x32\x16.bosdyn.api.RobotState\"@\n\x13RobotMetricsRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"s\n\x14RobotMetricsResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12/\n\rrobot_metrics\x18\x02 \x01(\x0b\x32\x18.bosdyn.api.RobotMetrics\"N\n!RobotHardwareConfigurationRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"\x93\x01\n\"RobotHardwareConfigurationResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x41\n\x16hardware_configuration\x18\x02 \x01(\x0b\x32!.bosdyn.api.HardwareConfiguration\"U\n\x15RobotLinkModelRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x11\n\tlink_name\x18\x02 \x01(\t\"|\n\x16RobotLinkModelResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x36\n\nlink_model\x18\x02 \x01(\x0b\x32\".bosdyn.api.Skeleton.Link.ObjModel\"\xca\x04\n\x12RobotImpairedState\x12\x46\n\x0fimpaired_status\x18\x01 \x01(\x0e\x32-.bosdyn.api.RobotImpairedState.ImpairedStatus\x12.\n\rsystem_faults\x18\x02 \x03(\x0b\x32\x17.bosdyn.api.SystemFault\x12\x30\n\x0eservice_faults\x18\x03 \x03(\x0b\x32\x18.bosdyn.api.ServiceFault\x12\x32\n\x0f\x62\x65havior_faults\x18\x04 \x03(\x0b\x32\x19.bosdyn.api.BehaviorFault\"\xd5\x02\n\x0eImpairedStatus\x12\x1b\n\x17IMPAIRED_STATUS_UNKNOWN\x10\x00\x12\x16\n\x12IMPAIRED_STATUS_OK\x10\x01\x12!\n\x1dIMPAIRED_STATUS_NO_ROBOT_DATA\x10\x02\x12 \n\x1cIMPAIRED_STATUS_SYSTEM_FAULT\x10\x03\x12\"\n\x1eIMPAIRED_STATUS_NO_MOTOR_POWER\x10\x04\x12-\n)IMPAIRED_STATUS_REMOTE_CLOUDS_NOT_WORKING\x10\x05\x12!\n\x1dIMPAIRED_STATUS_SERVICE_FAULT\x10\x06\x12\"\n\x1eIMPAIRED_STATUS_BEHAVIOR_FAULT\x10\x07\x12/\n+IMPAIRED_STATUS_ENTITY_DETECTOR_NOT_WORKING\x10\x08\x42\x11\x42\x0fRobotStateProtob\x06proto3')
 
 
 
 _SKELETON = DESCRIPTOR.message_types_by_name['Skeleton']
 _SKELETON_LINK = _SKELETON.nested_types_by_name['Link']
 _SKELETON_LINK_OBJMODEL = _SKELETON_LINK.nested_types_by_name['ObjModel']
 _HARDWARECONFIGURATION = DESCRIPTOR.message_types_by_name['HardwareConfiguration']
@@ -343,99 +343,99 @@
   _SKELETON._serialized_start=254
   _SKELETON._serialized_end=452
   _SKELETON_LINK._serialized_start=323
   _SKELETON_LINK._serialized_end=452
   _SKELETON_LINK_OBJMODEL._serialized_start=400
   _SKELETON_LINK_OBJMODEL._serialized_end=452
   _HARDWARECONFIGURATION._serialized_start=455
-  _HARDWARECONFIGURATION._serialized_end=705
-  _ROBOTSTATE._serialized_start=708
-  _ROBOTSTATE._serialized_end=1295
-  _POWERSTATE._serialized_start=1298
-  _POWERSTATE._serialized_end=2757
-  _POWERSTATE_MOTORPOWERSTATE._serialized_start=1852
-  _POWERSTATE_MOTORPOWERSTATE._serialized_end=2193
-  _POWERSTATE_SHOREPOWERSTATE._serialized_start=2196
-  _POWERSTATE_SHOREPOWERSTATE._serialized_end=2397
-  _POWERSTATE_ROBOTPOWERSTATE._serialized_start=2399
-  _POWERSTATE_ROBOTPOWERSTATE._serialized_end=2500
-  _POWERSTATE_PAYLOADPORTSPOWERSTATE._serialized_start=2503
-  _POWERSTATE_PAYLOADPORTSPOWERSTATE._serialized_end=2635
-  _POWERSTATE_WIFIRADIOPOWERSTATE._serialized_start=2637
-  _POWERSTATE_WIFIRADIOPOWERSTATE._serialized_end=2757
-  _SYSTEMFAULTSTATE._serialized_start=2760
-  _SYSTEMFAULTSTATE._serialized_end=3022
-  _SYSTEMFAULTSTATE_AGGREGATEDENTRY._serialized_start=2939
-  _SYSTEMFAULTSTATE_AGGREGATEDENTRY._serialized_end=3022
-  _SYSTEMFAULT._serialized_start=3025
-  _SYSTEMFAULT._serialized_end=3367
-  _SYSTEMFAULT_SEVERITY._serialized_start=3274
-  _SYSTEMFAULT_SEVERITY._serialized_end=3367
-  _ESTOPSTATE._serialized_start=3370
-  _ESTOPSTATE._serialized_end=3694
-  _ESTOPSTATE_TYPE._serialized_start=3560
-  _ESTOPSTATE_TYPE._serialized_end=3622
-  _ESTOPSTATE_STATE._serialized_start=3624
-  _ESTOPSTATE_STATE._serialized_end=3694
-  _BATTERYSTATE._serialized_start=3697
-  _BATTERYSTATE._serialized_end=4169
-  _BATTERYSTATE_STATUS._serialized_start=4056
-  _BATTERYSTATE_STATUS._serialized_end=4169
-  _KINEMATICSTATE._serialized_start=4172
-  _KINEMATICSTATE._serialized_end=4521
-  _JOINTSTATE._serialized_start=4524
-  _JOINTSTATE._serialized_end=4742
-  _BEHAVIORFAULTSTATE._serialized_start=4744
-  _BEHAVIORFAULTSTATE._serialized_end=4807
-  _BEHAVIORFAULT._serialized_start=4810
-  _BEHAVIORFAULT._serialized_end=5168
-  _BEHAVIORFAULT_CAUSE._serialized_start=5005
-  _BEHAVIORFAULT_CAUSE._serialized_end=5092
-  _BEHAVIORFAULT_STATUS._serialized_start=5094
-  _BEHAVIORFAULT_STATUS._serialized_end=5168
-  _ROBOTMETRICS._serialized_start=5170
-  _ROBOTMETRICS._serialized_end=5271
-  _COMMSSTATE._serialized_start=5273
-  _COMMSSTATE._serialized_end=5386
-  _WIFISTATE._serialized_start=5389
-  _WIFISTATE._serialized_end=5531
-  _WIFISTATE_MODE._serialized_start=5467
-  _WIFISTATE_MODE._serialized_end=5531
-  _FOOTSTATE._serialized_start=5534
-  _FOOTSTATE._serialized_end=6086
-  _FOOTSTATE_TERRAINSTATE._serialized_start=5698
-  _FOOTSTATE_TERRAINSTATE._serialized_end=6018
-  _FOOTSTATE_CONTACT._serialized_start=6020
-  _FOOTSTATE_CONTACT._serialized_end=6086
-  _MANIPULATORSTATE._serialized_start=6089
-  _MANIPULATORSTATE._serialized_end=6753
-  _MANIPULATORSTATE_STOWSTATE._serialized_start=6481
-  _MANIPULATORSTATE_STOWSTATE._serialized_end=6561
-  _MANIPULATORSTATE_CARRYSTATE._serialized_start=6564
-  _MANIPULATORSTATE_CARRYSTATE._serialized_end=6699
-  _SERVICEFAULTSTATE._serialized_start=6756
-  _SERVICEFAULTSTATE._serialized_end=7023
-  _SERVICEFAULTSTATE_AGGREGATEDENTRY._serialized_start=6939
-  _SERVICEFAULTSTATE_AGGREGATEDENTRY._serialized_end=7023
-  _TERRAINSTATE._serialized_start=7025
-  _TERRAINSTATE._serialized_end=7065
-  _ROBOTSTATEREQUEST._serialized_start=7067
-  _ROBOTSTATEREQUEST._serialized_end=7129
-  _ROBOTSTATERESPONSE._serialized_start=7131
-  _ROBOTSTATERESPONSE._serialized_end=7240
-  _ROBOTMETRICSREQUEST._serialized_start=7242
-  _ROBOTMETRICSREQUEST._serialized_end=7306
-  _ROBOTMETRICSRESPONSE._serialized_start=7308
-  _ROBOTMETRICSRESPONSE._serialized_end=7423
-  _ROBOTHARDWARECONFIGURATIONREQUEST._serialized_start=7425
-  _ROBOTHARDWARECONFIGURATIONREQUEST._serialized_end=7503
-  _ROBOTHARDWARECONFIGURATIONRESPONSE._serialized_start=7506
-  _ROBOTHARDWARECONFIGURATIONRESPONSE._serialized_end=7653
-  _ROBOTLINKMODELREQUEST._serialized_start=7655
-  _ROBOTLINKMODELREQUEST._serialized_end=7740
-  _ROBOTLINKMODELRESPONSE._serialized_start=7742
-  _ROBOTLINKMODELRESPONSE._serialized_end=7866
-  _ROBOTIMPAIREDSTATE._serialized_start=7869
-  _ROBOTIMPAIREDSTATE._serialized_end=8406
-  _ROBOTIMPAIREDSTATE_IMPAIREDSTATUS._serialized_start=8114
-  _ROBOTIMPAIREDSTATE_IMPAIREDSTATUS._serialized_end=8406
+  _HARDWARECONFIGURATION._serialized_end=738
+  _ROBOTSTATE._serialized_start=741
+  _ROBOTSTATE._serialized_end=1328
+  _POWERSTATE._serialized_start=1331
+  _POWERSTATE._serialized_end=2790
+  _POWERSTATE_MOTORPOWERSTATE._serialized_start=1885
+  _POWERSTATE_MOTORPOWERSTATE._serialized_end=2226
+  _POWERSTATE_SHOREPOWERSTATE._serialized_start=2229
+  _POWERSTATE_SHOREPOWERSTATE._serialized_end=2430
+  _POWERSTATE_ROBOTPOWERSTATE._serialized_start=2432
+  _POWERSTATE_ROBOTPOWERSTATE._serialized_end=2533
+  _POWERSTATE_PAYLOADPORTSPOWERSTATE._serialized_start=2536
+  _POWERSTATE_PAYLOADPORTSPOWERSTATE._serialized_end=2668
+  _POWERSTATE_WIFIRADIOPOWERSTATE._serialized_start=2670
+  _POWERSTATE_WIFIRADIOPOWERSTATE._serialized_end=2790
+  _SYSTEMFAULTSTATE._serialized_start=2793
+  _SYSTEMFAULTSTATE._serialized_end=3055
+  _SYSTEMFAULTSTATE_AGGREGATEDENTRY._serialized_start=2972
+  _SYSTEMFAULTSTATE_AGGREGATEDENTRY._serialized_end=3055
+  _SYSTEMFAULT._serialized_start=3058
+  _SYSTEMFAULT._serialized_end=3400
+  _SYSTEMFAULT_SEVERITY._serialized_start=3307
+  _SYSTEMFAULT_SEVERITY._serialized_end=3400
+  _ESTOPSTATE._serialized_start=3403
+  _ESTOPSTATE._serialized_end=3727
+  _ESTOPSTATE_TYPE._serialized_start=3593
+  _ESTOPSTATE_TYPE._serialized_end=3655
+  _ESTOPSTATE_STATE._serialized_start=3657
+  _ESTOPSTATE_STATE._serialized_end=3727
+  _BATTERYSTATE._serialized_start=3730
+  _BATTERYSTATE._serialized_end=4202
+  _BATTERYSTATE_STATUS._serialized_start=4089
+  _BATTERYSTATE_STATUS._serialized_end=4202
+  _KINEMATICSTATE._serialized_start=4205
+  _KINEMATICSTATE._serialized_end=4554
+  _JOINTSTATE._serialized_start=4557
+  _JOINTSTATE._serialized_end=4775
+  _BEHAVIORFAULTSTATE._serialized_start=4777
+  _BEHAVIORFAULTSTATE._serialized_end=4840
+  _BEHAVIORFAULT._serialized_start=4843
+  _BEHAVIORFAULT._serialized_end=5201
+  _BEHAVIORFAULT_CAUSE._serialized_start=5038
+  _BEHAVIORFAULT_CAUSE._serialized_end=5125
+  _BEHAVIORFAULT_STATUS._serialized_start=5127
+  _BEHAVIORFAULT_STATUS._serialized_end=5201
+  _ROBOTMETRICS._serialized_start=5203
+  _ROBOTMETRICS._serialized_end=5304
+  _COMMSSTATE._serialized_start=5306
+  _COMMSSTATE._serialized_end=5419
+  _WIFISTATE._serialized_start=5422
+  _WIFISTATE._serialized_end=5564
+  _WIFISTATE_MODE._serialized_start=5500
+  _WIFISTATE_MODE._serialized_end=5564
+  _FOOTSTATE._serialized_start=5567
+  _FOOTSTATE._serialized_end=6119
+  _FOOTSTATE_TERRAINSTATE._serialized_start=5731
+  _FOOTSTATE_TERRAINSTATE._serialized_end=6051
+  _FOOTSTATE_CONTACT._serialized_start=6053
+  _FOOTSTATE_CONTACT._serialized_end=6119
+  _MANIPULATORSTATE._serialized_start=6122
+  _MANIPULATORSTATE._serialized_end=6786
+  _MANIPULATORSTATE_STOWSTATE._serialized_start=6514
+  _MANIPULATORSTATE_STOWSTATE._serialized_end=6594
+  _MANIPULATORSTATE_CARRYSTATE._serialized_start=6597
+  _MANIPULATORSTATE_CARRYSTATE._serialized_end=6732
+  _SERVICEFAULTSTATE._serialized_start=6789
+  _SERVICEFAULTSTATE._serialized_end=7056
+  _SERVICEFAULTSTATE_AGGREGATEDENTRY._serialized_start=6972
+  _SERVICEFAULTSTATE_AGGREGATEDENTRY._serialized_end=7056
+  _TERRAINSTATE._serialized_start=7058
+  _TERRAINSTATE._serialized_end=7098
+  _ROBOTSTATEREQUEST._serialized_start=7100
+  _ROBOTSTATEREQUEST._serialized_end=7162
+  _ROBOTSTATERESPONSE._serialized_start=7164
+  _ROBOTSTATERESPONSE._serialized_end=7273
+  _ROBOTMETRICSREQUEST._serialized_start=7275
+  _ROBOTMETRICSREQUEST._serialized_end=7339
+  _ROBOTMETRICSRESPONSE._serialized_start=7341
+  _ROBOTMETRICSRESPONSE._serialized_end=7456
+  _ROBOTHARDWARECONFIGURATIONREQUEST._serialized_start=7458
+  _ROBOTHARDWARECONFIGURATIONREQUEST._serialized_end=7536
+  _ROBOTHARDWARECONFIGURATIONRESPONSE._serialized_start=7539
+  _ROBOTHARDWARECONFIGURATIONRESPONSE._serialized_end=7686
+  _ROBOTLINKMODELREQUEST._serialized_start=7688
+  _ROBOTLINKMODELREQUEST._serialized_end=7773
+  _ROBOTLINKMODELRESPONSE._serialized_start=7775
+  _ROBOTLINKMODELRESPONSE._serialized_end=7899
+  _ROBOTIMPAIREDSTATE._serialized_start=7902
+  _ROBOTIMPAIREDSTATE._serialized_end=8488
+  _ROBOTIMPAIREDSTATE_IMPAIREDSTATUS._serialized_start=8147
+  _ROBOTIMPAIREDSTATE_IMPAIREDSTATUS._serialized_end=8488
 # @@protoc_insertion_point(module_scope)
```

## bosdyn/api/stairs_pb2.py

```diff
@@ -11,29 +11,59 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from bosdyn.api import geometry_pb2 as bosdyn_dot_api_dot_geometry__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17\x62osdyn/api/stairs.proto\x12\nbosdyn.api\x1a\x19\x62osdyn/api/geometry.proto\"U\n\x0eStairTransform\x12/\n\x12\x66rame_tform_stairs\x18\x01 \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\x12\x12\n\nframe_name\x18\x02 \x01(\t\"\xce\x03\n\x11StraightStaircase\x12\x33\n\x14\x66rom_ko_tform_stairs\x18\x01 \x01(\x0b\x32\x13.bosdyn.api.SE3PoseH\x00\x12+\n\x05tform\x18\x05 \x01(\x0b\x32\x1a.bosdyn.api.StairTransformH\x00\x12\x33\n\x06stairs\x18\x02 \x03(\x0b\x32#.bosdyn.api.StraightStaircase.Stair\x12=\n\x0e\x62ottom_landing\x18\x03 \x01(\x0b\x32%.bosdyn.api.StraightStaircase.Landing\x12:\n\x0btop_landing\x18\x04 \x01(\x0b\x32%.bosdyn.api.StraightStaircase.Landing\x1a\"\n\x05Stair\x12\x0c\n\x04rise\x18\x01 \x01(\x02\x12\x0b\n\x03run\x18\x02 \x01(\x02\x1aw\n\x07Landing\x12\x38\n\x1bstairs_tform_landing_center\x18\x01 \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\x12\x18\n\x10landing_extent_x\x18\x02 \x01(\x01\x12\x18\n\x10landing_extent_y\x18\x03 \x01(\x01\x42\n\n\x08locationB\rB\x0bStairsProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17\x62osdyn/api/stairs.proto\x12\nbosdyn.api\x1a\x19\x62osdyn/api/geometry.proto\"U\n\x0eStairTransform\x12/\n\x12\x66rame_tform_stairs\x18\x01 \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\x12\x12\n\nframe_name\x18\x02 \x01(\t\"\xa8\x06\n\tStaircase\x12;\n\x0eknowledge_type\x18\x01 \x01(\x0e\x32#.bosdyn.api.Staircase.KnowledgeType\x12/\n\x0bstair_tform\x18\x02 \x01(\x0b\x32\x1a.bosdyn.api.StairTransform\x12\x17\n\x0fnumber_of_steps\x18\x03 \x01(\x05\x12\x14\n\x0c\x61verage_rise\x18\x04 \x01(\x01\x12\x13\n\x0b\x61verage_run\x18\x05 \x01(\x01\x12\x32\n\raverage_width\x18\x06 \x01(\x0b\x32\x1b.bosdyn.api.Staircase.Width\x12)\n\x05steps\x18\x07 \x03(\x0b\x32\x1a.bosdyn.api.Staircase.Step\x1a\xe6\x01\n\x05Width\x12\r\n\x05width\x18\x01 \x01(\x01\x12?\n\rbounded_width\x18\x02 \x01(\x0e\x32(.bosdyn.api.Staircase.Width.BoundedWidth\"\x8c\x01\n\x0c\x42oundedWidth\x12\x19\n\x15\x42OUNDED_WIDTH_UNKNOWN\x10\x00\x12\x19\n\x15\x42OUNDED_WIDTH_NEITHER\x10\x01\x12\x16\n\x12\x42OUNDED_WIDTH_WEST\x10\x02\x12\x16\n\x12\x42OUNDED_WIDTH_EAST\x10\x03\x12\x16\n\x12\x42OUNDED_WIDTH_BOTH\x10\x04\x1at\n\x04Step\x12\x1f\n\x05point\x18\x01 \x01(\x0b\x32\x10.bosdyn.api.Vec3\x12\x1f\n\x05north\x18\x02 \x01(\x0b\x32\x10.bosdyn.api.Vec2\x12*\n\x05width\x18\x03 \x01(\x0b\x32\x1b.bosdyn.api.Staircase.Width\"\xaa\x01\n\rKnowledgeType\x12\x1a\n\x16KNOWLEDGE_TYPE_UNKNOWN\x10\x00\x12\x19\n\x15KNOWLEDGE_TYPE_MAPPED\x10\x01\x12\"\n\x1eKNOWLEDGE_TYPE_TRACKED_ONGOING\x10\x02\x12$\n KNOWLEDGE_TYPE_TRACKED_COMPLETED\x10\x03\x12\x18\n\x14KNOWLEDGE_TYPE_OTHER\x10\x04\"\xd2\x03\n\x11StraightStaircase\x12\x33\n\x14\x66rom_ko_tform_stairs\x18\x01 \x01(\x0b\x32\x13.bosdyn.api.SE3PoseH\x00\x12+\n\x05tform\x18\x05 \x01(\x0b\x32\x1a.bosdyn.api.StairTransformH\x00\x12\x33\n\x06stairs\x18\x02 \x03(\x0b\x32#.bosdyn.api.StraightStaircase.Stair\x12=\n\x0e\x62ottom_landing\x18\x03 \x01(\x0b\x32%.bosdyn.api.StraightStaircase.Landing\x12:\n\x0btop_landing\x18\x04 \x01(\x0b\x32%.bosdyn.api.StraightStaircase.Landing\x1a\"\n\x05Stair\x12\x0c\n\x04rise\x18\x01 \x01(\x02\x12\x0b\n\x03run\x18\x02 \x01(\x02\x1aw\n\x07Landing\x12\x38\n\x1bstairs_tform_landing_center\x18\x01 \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\x12\x18\n\x10landing_extent_x\x18\x02 \x01(\x01\x12\x18\n\x10landing_extent_y\x18\x03 \x01(\x01:\x02\x18\x01\x42\n\n\x08location\"\x80\x01\n\x10StaircaseLanding\x12\x38\n\x1bstairs_tform_landing_center\x18\x01 \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\x12\x18\n\x10landing_extent_x\x18\x02 \x01(\x01\x12\x18\n\x10landing_extent_y\x18\x03 \x01(\x01\"\xaa\x01\n\x15StaircaseWithLandings\x12\x34\n\x0e\x62ottom_landing\x18\x01 \x01(\x0b\x32\x1c.bosdyn.api.StaircaseLanding\x12(\n\tstaircase\x18\x02 \x01(\x0b\x32\x15.bosdyn.api.Staircase\x12\x31\n\x0btop_landing\x18\x03 \x01(\x0b\x32\x1c.bosdyn.api.StaircaseLandingB\rB\x0bStairsProtob\x06proto3')
 
 
 
 _STAIRTRANSFORM = DESCRIPTOR.message_types_by_name['StairTransform']
+_STAIRCASE = DESCRIPTOR.message_types_by_name['Staircase']
+_STAIRCASE_WIDTH = _STAIRCASE.nested_types_by_name['Width']
+_STAIRCASE_STEP = _STAIRCASE.nested_types_by_name['Step']
 _STRAIGHTSTAIRCASE = DESCRIPTOR.message_types_by_name['StraightStaircase']
 _STRAIGHTSTAIRCASE_STAIR = _STRAIGHTSTAIRCASE.nested_types_by_name['Stair']
 _STRAIGHTSTAIRCASE_LANDING = _STRAIGHTSTAIRCASE.nested_types_by_name['Landing']
+_STAIRCASELANDING = DESCRIPTOR.message_types_by_name['StaircaseLanding']
+_STAIRCASEWITHLANDINGS = DESCRIPTOR.message_types_by_name['StaircaseWithLandings']
+_STAIRCASE_WIDTH_BOUNDEDWIDTH = _STAIRCASE_WIDTH.enum_types_by_name['BoundedWidth']
+_STAIRCASE_KNOWLEDGETYPE = _STAIRCASE.enum_types_by_name['KnowledgeType']
 StairTransform = _reflection.GeneratedProtocolMessageType('StairTransform', (_message.Message,), {
   'DESCRIPTOR' : _STAIRTRANSFORM,
   '__module__' : 'bosdyn.api.stairs_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.StairTransform)
   })
 _sym_db.RegisterMessage(StairTransform)
 
+Staircase = _reflection.GeneratedProtocolMessageType('Staircase', (_message.Message,), {
+
+  'Width' : _reflection.GeneratedProtocolMessageType('Width', (_message.Message,), {
+    'DESCRIPTOR' : _STAIRCASE_WIDTH,
+    '__module__' : 'bosdyn.api.stairs_pb2'
+    # @@protoc_insertion_point(class_scope:bosdyn.api.Staircase.Width)
+    })
+  ,
+
+  'Step' : _reflection.GeneratedProtocolMessageType('Step', (_message.Message,), {
+    'DESCRIPTOR' : _STAIRCASE_STEP,
+    '__module__' : 'bosdyn.api.stairs_pb2'
+    # @@protoc_insertion_point(class_scope:bosdyn.api.Staircase.Step)
+    })
+  ,
+  'DESCRIPTOR' : _STAIRCASE,
+  '__module__' : 'bosdyn.api.stairs_pb2'
+  # @@protoc_insertion_point(class_scope:bosdyn.api.Staircase)
+  })
+_sym_db.RegisterMessage(Staircase)
+_sym_db.RegisterMessage(Staircase.Width)
+_sym_db.RegisterMessage(Staircase.Step)
+
 StraightStaircase = _reflection.GeneratedProtocolMessageType('StraightStaircase', (_message.Message,), {
 
   'Stair' : _reflection.GeneratedProtocolMessageType('Stair', (_message.Message,), {
     'DESCRIPTOR' : _STRAIGHTSTAIRCASE_STAIR,
     '__module__' : 'bosdyn.api.stairs_pb2'
     # @@protoc_insertion_point(class_scope:bosdyn.api.StraightStaircase.Stair)
     })
@@ -49,20 +79,50 @@
   '__module__' : 'bosdyn.api.stairs_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.StraightStaircase)
   })
 _sym_db.RegisterMessage(StraightStaircase)
 _sym_db.RegisterMessage(StraightStaircase.Stair)
 _sym_db.RegisterMessage(StraightStaircase.Landing)
 
+StaircaseLanding = _reflection.GeneratedProtocolMessageType('StaircaseLanding', (_message.Message,), {
+  'DESCRIPTOR' : _STAIRCASELANDING,
+  '__module__' : 'bosdyn.api.stairs_pb2'
+  # @@protoc_insertion_point(class_scope:bosdyn.api.StaircaseLanding)
+  })
+_sym_db.RegisterMessage(StaircaseLanding)
+
+StaircaseWithLandings = _reflection.GeneratedProtocolMessageType('StaircaseWithLandings', (_message.Message,), {
+  'DESCRIPTOR' : _STAIRCASEWITHLANDINGS,
+  '__module__' : 'bosdyn.api.stairs_pb2'
+  # @@protoc_insertion_point(class_scope:bosdyn.api.StaircaseWithLandings)
+  })
+_sym_db.RegisterMessage(StaircaseWithLandings)
+
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'B\013StairsProto'
+  _STRAIGHTSTAIRCASE._options = None
+  _STRAIGHTSTAIRCASE._serialized_options = b'\030\001'
   _STAIRTRANSFORM._serialized_start=66
   _STAIRTRANSFORM._serialized_end=151
-  _STRAIGHTSTAIRCASE._serialized_start=154
-  _STRAIGHTSTAIRCASE._serialized_end=616
-  _STRAIGHTSTAIRCASE_STAIR._serialized_start=449
-  _STRAIGHTSTAIRCASE_STAIR._serialized_end=483
-  _STRAIGHTSTAIRCASE_LANDING._serialized_start=485
-  _STRAIGHTSTAIRCASE_LANDING._serialized_end=604
+  _STAIRCASE._serialized_start=154
+  _STAIRCASE._serialized_end=962
+  _STAIRCASE_WIDTH._serialized_start=441
+  _STAIRCASE_WIDTH._serialized_end=671
+  _STAIRCASE_WIDTH_BOUNDEDWIDTH._serialized_start=531
+  _STAIRCASE_WIDTH_BOUNDEDWIDTH._serialized_end=671
+  _STAIRCASE_STEP._serialized_start=673
+  _STAIRCASE_STEP._serialized_end=789
+  _STAIRCASE_KNOWLEDGETYPE._serialized_start=792
+  _STAIRCASE_KNOWLEDGETYPE._serialized_end=962
+  _STRAIGHTSTAIRCASE._serialized_start=965
+  _STRAIGHTSTAIRCASE._serialized_end=1431
+  _STRAIGHTSTAIRCASE_STAIR._serialized_start=1260
+  _STRAIGHTSTAIRCASE_STAIR._serialized_end=1294
+  _STRAIGHTSTAIRCASE_LANDING._serialized_start=1296
+  _STRAIGHTSTAIRCASE_LANDING._serialized_end=1415
+  _STAIRCASELANDING._serialized_start=1434
+  _STAIRCASELANDING._serialized_end=1562
+  _STAIRCASEWITHLANDINGS._serialized_start=1565
+  _STAIRCASEWITHLANDINGS._serialized_end=1735
 # @@protoc_insertion_point(module_scope)
```

## bosdyn/api/world_object_pb2.py

```diff
@@ -14,42 +14,48 @@
 
 
 from bosdyn.api.docking import docking_pb2 as bosdyn_dot_api_dot_docking_dot_docking__pb2
 from bosdyn.api import geometry_pb2 as bosdyn_dot_api_dot_geometry__pb2
 from bosdyn.api import header_pb2 as bosdyn_dot_api_dot_header__pb2
 from bosdyn.api import image_pb2 as bosdyn_dot_api_dot_image__pb2
 from bosdyn.api import sparse_features_pb2 as bosdyn_dot_api_dot_sparse__features__pb2
+from bosdyn.api import stairs_pb2 as bosdyn_dot_api_dot_stairs__pb2
+from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import any_pb2 as google_dot_protobuf_dot_any__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1d\x62osdyn/api/world_object.proto\x12\nbosdyn.api\x1a bosdyn/api/docking/docking.proto\x1a\x19\x62osdyn/api/geometry.proto\x1a\x17\x62osdyn/api/header.proto\x1a\x16\x62osdyn/api/image.proto\x1a bosdyn/api/sparse_features.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x19google/protobuf/any.proto\"\xab\x04\n\x0bWorldObject\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x34\n\x10\x61\x63quisition_time\x18\x1e \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x13transforms_snapshot\x18\x1f \x01(\x0b\x32\x1d.bosdyn.api.FrameTreeSnapshot\x12;\n\x13\x64rawable_properties\x18\x05 \x03(\x0b\x32\x1e.bosdyn.api.DrawableProperties\x12;\n\x13\x61priltag_properties\x18\x06 \x01(\x0b\x32\x1e.bosdyn.api.AprilTagProperties\x12\x35\n\x10image_properties\x18\t \x01(\x0b\x32\x1b.bosdyn.api.ImageProperties\x12\x33\n\x0f\x64ock_properties\x18\n \x01(\x0b\x32\x1a.bosdyn.api.DockProperties\x12\x31\n\x0eray_properties\x18\x0b \x01(\x0b\x32\x19.bosdyn.api.RayProperties\x12\x42\n\x17\x62ounding_box_properties\x18\x0c \x01(\x0b\x32!.bosdyn.api.BoundingBoxProperties\x12\x33\n\x15\x61\x64\x64itional_properties\x18\x64 \x01(\x0b\x32\x14.google.protobuf.Any\"\xab\x01\n\x16ListWorldObjectRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x30\n\x0bobject_type\x18\x02 \x03(\x0e\x32\x1b.bosdyn.api.WorldObjectType\x12\x34\n\x10timestamp_filter\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"u\n\x17ListWorldObjectResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12.\n\rworld_objects\x18\x02 \x03(\x0b\x32\x17.bosdyn.api.WorldObject\"\xcc\x02\n\x18MutateWorldObjectRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12?\n\x08mutation\x18\x02 \x01(\x0b\x32-.bosdyn.api.MutateWorldObjectRequest.Mutation\x1ap\n\x08Mutation\x12;\n\x06\x61\x63tion\x18\x01 \x01(\x0e\x32+.bosdyn.api.MutateWorldObjectRequest.Action\x12\'\n\x06object\x18\x02 \x01(\x0b\x32\x17.bosdyn.api.WorldObject\"R\n\x06\x41\x63tion\x12\x12\n\x0e\x41\x43TION_UNKNOWN\x10\x00\x12\x0e\n\nACTION_ADD\x10\x01\x12\x11\n\rACTION_CHANGE\x10\x02\x12\x11\n\rACTION_DELETE\x10\x03\"\x87\x02\n\x19MutateWorldObjectResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12<\n\x06status\x18\x02 \x01(\x0e\x32,.bosdyn.api.MutateWorldObjectResponse.Status\x12\x19\n\x11mutated_object_id\x18\x04 \x01(\x05\"e\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1e\n\x1aSTATUS_INVALID_MUTATION_ID\x10\x02\x12\x18\n\x14STATUS_NO_PERMISSION\x10\x03\"\x96\x02\n\x0fImageProperties\x12\x15\n\rcamera_source\x18\x01 \x01(\t\x12*\n\x0b\x63oordinates\x18\x02 \x01(\x0b\x32\x13.bosdyn.api.PolygonH\x00\x12,\n\tkeypoints\x18\x04 \x01(\x0b\x32\x17.bosdyn.api.KeypointSetH\x00\x12-\n\x0cimage_source\x18\x05 \x01(\x0b\x32\x17.bosdyn.api.ImageSource\x12/\n\rimage_capture\x18\x06 \x01(\x0b\x32\x18.bosdyn.api.ImageCapture\x12$\n\x1c\x66rame_name_image_coordinates\x18\x03 \x01(\tB\x0c\n\nimage_data\"\x8f\x01\n\x0e\x44ockProperties\x12\x0f\n\x07\x64ock_id\x18\x01 \x01(\r\x12*\n\x04type\x18\x02 \x01(\x0e\x32\x1c.bosdyn.api.docking.DockType\x12\x17\n\x0f\x66rame_name_dock\x18\x03 \x01(\t\x12\x13\n\x0bunavailable\x18\x04 \x01(\x08\x12\x12\n\nfrom_prior\x18\x05 \x01(\x08\"\xa0\x04\n\x12\x41prilTagProperties\x12\x0e\n\x06tag_id\x18\x01 \x01(\x05\x12$\n\ndimensions\x18\x02 \x01(\x0b\x32\x10.bosdyn.api.Vec2\x12\x1b\n\x13\x66rame_name_fiducial\x18\x03 \x01(\t\x12O\n\x14\x66iducial_pose_status\x18\x08 \x01(\x0e\x32\x31.bosdyn.api.AprilTagProperties.AprilTagPoseStatus\x12$\n\x1c\x66rame_name_fiducial_filtered\x18\x04 \x01(\t\x12X\n\x1d\x66iducial_filtered_pose_status\x18\t \x01(\x0e\x32\x31.bosdyn.api.AprilTagProperties.AprilTagPoseStatus\x12\x19\n\x11\x66rame_name_camera\x18\x07 \x01(\t\x12\x37\n\x14\x64\x65tection_covariance\x18\x05 \x01(\x0b\x32\x19.bosdyn.api.SE3Covariance\x12,\n$detection_covariance_reference_frame\x18\x06 \x01(\t\"d\n\x12\x41prilTagPoseStatus\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x14\n\x10STATUS_AMBIGUOUS\x10\x02\x12\x15\n\x11STATUS_HIGH_ERROR\x10\x03\"<\n\rRayProperties\x12\x1c\n\x03ray\x18\x01 \x01(\x0b\x32\x0f.bosdyn.api.Ray\x12\r\n\x05\x66rame\x18\x02 \x01(\t\"Q\n\x15\x42oundingBoxProperties\x12)\n\x0fsize_ewrt_frame\x18\x01 \x01(\x0b\x32\x10.bosdyn.api.Vec3\x12\r\n\x05\x66rame\x18\x02 \x01(\t\"\xbb\x04\n\x12\x44rawableProperties\x12\x33\n\x05\x63olor\x18\x01 \x01(\x0b\x32$.bosdyn.api.DrawableProperties.Color\x12\r\n\x05label\x18\x02 \x01(\t\x12\x11\n\twireframe\x18\x03 \x01(\x08\x12*\n\x05\x66rame\x18\x04 \x01(\x0b\x32\x19.bosdyn.api.DrawableFrameH\x00\x12,\n\x06sphere\x18\x05 \x01(\x0b\x32\x1a.bosdyn.api.DrawableSphereH\x00\x12&\n\x03\x62ox\x18\x06 \x01(\x0b\x32\x17.bosdyn.api.DrawableBoxH\x00\x12*\n\x05\x61rrow\x18\x07 \x01(\x0b\x32\x19.bosdyn.api.DrawableArrowH\x00\x12.\n\x07\x63\x61psule\x18\x08 \x01(\x0b\x32\x1b.bosdyn.api.DrawableCapsuleH\x00\x12\x30\n\x08\x63ylinder\x18\t \x01(\x0b\x32\x1c.bosdyn.api.DrawableCylinderH\x00\x12\x32\n\tlinestrip\x18\n \x01(\x0b\x32\x1d.bosdyn.api.DrawableLineStripH\x00\x12,\n\x06points\x18\x0b \x01(\x0b\x32\x1a.bosdyn.api.DrawablePointsH\x00\x12\x1b\n\x13\x66rame_name_drawable\x18\x0c \x01(\t\x1a\x33\n\x05\x43olor\x12\t\n\x01r\x18\x01 \x01(\x05\x12\t\n\x01g\x18\x02 \x01(\x05\x12\t\n\x01\x62\x18\x03 \x01(\x05\x12\t\n\x01\x61\x18\x04 \x01(\x01\x42\n\n\x08\x64rawable\";\n\rDrawableFrame\x12\x14\n\x0c\x61rrow_length\x18\x01 \x01(\x01\x12\x14\n\x0c\x61rrow_radius\x18\x02 \x01(\x01\" \n\x0e\x44rawableSphere\x12\x0e\n\x06radius\x18\x01 \x01(\x01\"-\n\x0b\x44rawableBox\x12\x1e\n\x04size\x18\x01 \x01(\x0b\x32\x10.bosdyn.api.Vec3\"D\n\rDrawableArrow\x12#\n\tdirection\x18\x01 \x01(\x0b\x32\x10.bosdyn.api.Vec3\x12\x0e\n\x06radius\x18\x02 \x01(\x01\"F\n\x0f\x44rawableCapsule\x12#\n\tdirection\x18\x01 \x01(\x0b\x32\x10.bosdyn.api.Vec3\x12\x0e\n\x06radius\x18\x02 \x01(\x01\"G\n\x10\x44rawableCylinder\x12#\n\tdirection\x18\x01 \x01(\x0b\x32\x10.bosdyn.api.Vec3\x12\x0e\n\x06radius\x18\x02 \x01(\x01\"5\n\x11\x44rawableLineStrip\x12 \n\x06points\x18\x01 \x01(\x0b\x32\x10.bosdyn.api.Vec3\"2\n\x0e\x44rawablePoints\x12 \n\x06points\x18\x01 \x03(\x0b\x32\x10.bosdyn.api.Vec3*\x9c\x01\n\x0fWorldObjectType\x12\x18\n\x14WORLD_OBJECT_UNKNOWN\x10\x00\x12\x19\n\x15WORLD_OBJECT_DRAWABLE\x10\x01\x12\x19\n\x15WORLD_OBJECT_APRILTAG\x10\x02\x12\"\n\x1eWORLD_OBJECT_IMAGE_COORDINATES\x10\x05\x12\x15\n\x11WORLD_OBJECT_DOCK\x10\x06\x42\x12\x42\x10WorldObjectProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1d\x62osdyn/api/world_object.proto\x12\nbosdyn.api\x1a bosdyn/api/docking/docking.proto\x1a\x19\x62osdyn/api/geometry.proto\x1a\x17\x62osdyn/api/header.proto\x1a\x16\x62osdyn/api/image.proto\x1a bosdyn/api/sparse_features.proto\x1a\x17\x62osdyn/api/stairs.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x19google/protobuf/any.proto\"\xe0\x05\n\x0bWorldObject\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x34\n\x10\x61\x63quisition_time\x18\x1e \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x13transforms_snapshot\x18\x1f \x01(\x0b\x32\x1d.bosdyn.api.FrameTreeSnapshot\x12\x32\n\x0fobject_lifetime\x18  \x01(\x0b\x32\x19.google.protobuf.Duration\x12;\n\x13\x64rawable_properties\x18\x05 \x03(\x0b\x32\x1e.bosdyn.api.DrawableProperties\x12;\n\x13\x61priltag_properties\x18\x06 \x01(\x0b\x32\x1e.bosdyn.api.AprilTagProperties\x12@\n\x16nogo_region_properties\x18\x0e \x01(\x0b\x32 .bosdyn.api.NoGoRegionProperties\x12\x35\n\x10image_properties\x18\t \x01(\x0b\x32\x1b.bosdyn.api.ImageProperties\x12\x33\n\x0f\x64ock_properties\x18\n \x01(\x0b\x32\x1a.bosdyn.api.DockProperties\x12\x31\n\x0eray_properties\x18\x0b \x01(\x0b\x32\x19.bosdyn.api.RayProperties\x12\x42\n\x17\x62ounding_box_properties\x18\x0c \x01(\x0b\x32!.bosdyn.api.BoundingBoxProperties\x12=\n\x14staircase_properties\x18\x0f \x01(\x0b\x32\x1f.bosdyn.api.StaircaseProperties\x12\x33\n\x15\x61\x64\x64itional_properties\x18\x64 \x01(\x0b\x32\x14.google.protobuf.Any\"\xab\x01\n\x16ListWorldObjectRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x30\n\x0bobject_type\x18\x02 \x03(\x0e\x32\x1b.bosdyn.api.WorldObjectType\x12\x34\n\x10timestamp_filter\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"u\n\x17ListWorldObjectResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12.\n\rworld_objects\x18\x02 \x03(\x0b\x32\x17.bosdyn.api.WorldObject\"\xcc\x02\n\x18MutateWorldObjectRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12?\n\x08mutation\x18\x02 \x01(\x0b\x32-.bosdyn.api.MutateWorldObjectRequest.Mutation\x1ap\n\x08Mutation\x12;\n\x06\x61\x63tion\x18\x01 \x01(\x0e\x32+.bosdyn.api.MutateWorldObjectRequest.Action\x12\'\n\x06object\x18\x02 \x01(\x0b\x32\x17.bosdyn.api.WorldObject\"R\n\x06\x41\x63tion\x12\x12\n\x0e\x41\x43TION_UNKNOWN\x10\x00\x12\x0e\n\nACTION_ADD\x10\x01\x12\x11\n\rACTION_CHANGE\x10\x02\x12\x11\n\rACTION_DELETE\x10\x03\"\xa9\x02\n\x19MutateWorldObjectResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12<\n\x06status\x18\x02 \x01(\x0e\x32,.bosdyn.api.MutateWorldObjectResponse.Status\x12\x19\n\x11mutated_object_id\x18\x04 \x01(\x05\"\x86\x01\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1e\n\x1aSTATUS_INVALID_MUTATION_ID\x10\x02\x12\x18\n\x14STATUS_NO_PERMISSION\x10\x03\x12\x1f\n\x1bSTATUS_INVALID_WORLD_OBJECT\x10\x04\"\xc7\x01\n\x14NoGoRegionProperties\x12(\n\x03\x62ox\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.Box2WithFrameH\x00\x12(\n disable_foot_obstacle_generation\x18\x02 \x01(\x08\x12(\n disable_body_obstacle_generation\x18\x03 \x01(\x08\x12\'\n\x1f\x64isable_foot_obstacle_inflation\x18\x04 \x01(\x08\x42\x08\n\x06region\"\x96\x02\n\x0fImageProperties\x12\x15\n\rcamera_source\x18\x01 \x01(\t\x12*\n\x0b\x63oordinates\x18\x02 \x01(\x0b\x32\x13.bosdyn.api.PolygonH\x00\x12,\n\tkeypoints\x18\x04 \x01(\x0b\x32\x17.bosdyn.api.KeypointSetH\x00\x12-\n\x0cimage_source\x18\x05 \x01(\x0b\x32\x17.bosdyn.api.ImageSource\x12/\n\rimage_capture\x18\x06 \x01(\x0b\x32\x18.bosdyn.api.ImageCapture\x12$\n\x1c\x66rame_name_image_coordinates\x18\x03 \x01(\tB\x0c\n\nimage_data\"\x8f\x01\n\x0e\x44ockProperties\x12\x0f\n\x07\x64ock_id\x18\x01 \x01(\r\x12*\n\x04type\x18\x02 \x01(\x0e\x32\x1c.bosdyn.api.docking.DockType\x12\x17\n\x0f\x66rame_name_dock\x18\x03 \x01(\t\x12\x13\n\x0bunavailable\x18\x04 \x01(\x08\x12\x12\n\nfrom_prior\x18\x05 \x01(\x08\"\xa0\x04\n\x12\x41prilTagProperties\x12\x0e\n\x06tag_id\x18\x01 \x01(\x05\x12$\n\ndimensions\x18\x02 \x01(\x0b\x32\x10.bosdyn.api.Vec2\x12\x1b\n\x13\x66rame_name_fiducial\x18\x03 \x01(\t\x12O\n\x14\x66iducial_pose_status\x18\x08 \x01(\x0e\x32\x31.bosdyn.api.AprilTagProperties.AprilTagPoseStatus\x12$\n\x1c\x66rame_name_fiducial_filtered\x18\x04 \x01(\t\x12X\n\x1d\x66iducial_filtered_pose_status\x18\t \x01(\x0e\x32\x31.bosdyn.api.AprilTagProperties.AprilTagPoseStatus\x12\x19\n\x11\x66rame_name_camera\x18\x07 \x01(\t\x12\x37\n\x14\x64\x65tection_covariance\x18\x05 \x01(\x0b\x32\x19.bosdyn.api.SE3Covariance\x12,\n$detection_covariance_reference_frame\x18\x06 \x01(\t\"d\n\x12\x41prilTagPoseStatus\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x14\n\x10STATUS_AMBIGUOUS\x10\x02\x12\x15\n\x11STATUS_HIGH_ERROR\x10\x03\"<\n\rRayProperties\x12\x1c\n\x03ray\x18\x01 \x01(\x0b\x32\x0f.bosdyn.api.Ray\x12\r\n\x05\x66rame\x18\x02 \x01(\t\"Q\n\x15\x42oundingBoxProperties\x12)\n\x0fsize_ewrt_frame\x18\x01 \x01(\x0b\x32\x10.bosdyn.api.Vec3\x12\r\n\x05\x66rame\x18\x02 \x01(\t\"\xbb\x04\n\x12\x44rawableProperties\x12\x33\n\x05\x63olor\x18\x01 \x01(\x0b\x32$.bosdyn.api.DrawableProperties.Color\x12\r\n\x05label\x18\x02 \x01(\t\x12\x11\n\twireframe\x18\x03 \x01(\x08\x12*\n\x05\x66rame\x18\x04 \x01(\x0b\x32\x19.bosdyn.api.DrawableFrameH\x00\x12,\n\x06sphere\x18\x05 \x01(\x0b\x32\x1a.bosdyn.api.DrawableSphereH\x00\x12&\n\x03\x62ox\x18\x06 \x01(\x0b\x32\x17.bosdyn.api.DrawableBoxH\x00\x12*\n\x05\x61rrow\x18\x07 \x01(\x0b\x32\x19.bosdyn.api.DrawableArrowH\x00\x12.\n\x07\x63\x61psule\x18\x08 \x01(\x0b\x32\x1b.bosdyn.api.DrawableCapsuleH\x00\x12\x30\n\x08\x63ylinder\x18\t \x01(\x0b\x32\x1c.bosdyn.api.DrawableCylinderH\x00\x12\x32\n\tlinestrip\x18\n \x01(\x0b\x32\x1d.bosdyn.api.DrawableLineStripH\x00\x12,\n\x06points\x18\x0b \x01(\x0b\x32\x1a.bosdyn.api.DrawablePointsH\x00\x12\x1b\n\x13\x66rame_name_drawable\x18\x0c \x01(\t\x1a\x33\n\x05\x43olor\x12\t\n\x01r\x18\x01 \x01(\x05\x12\t\n\x01g\x18\x02 \x01(\x05\x12\t\n\x01\x62\x18\x03 \x01(\x05\x12\t\n\x01\x61\x18\x04 \x01(\x01\x42\n\n\x08\x64rawable\"?\n\x13StaircaseProperties\x12(\n\tstaircase\x18\x01 \x01(\x0b\x32\x15.bosdyn.api.Staircase\";\n\rDrawableFrame\x12\x14\n\x0c\x61rrow_length\x18\x01 \x01(\x01\x12\x14\n\x0c\x61rrow_radius\x18\x02 \x01(\x01\" \n\x0e\x44rawableSphere\x12\x0e\n\x06radius\x18\x01 \x01(\x01\"-\n\x0b\x44rawableBox\x12\x1e\n\x04size\x18\x01 \x01(\x0b\x32\x10.bosdyn.api.Vec3\"D\n\rDrawableArrow\x12#\n\tdirection\x18\x01 \x01(\x0b\x32\x10.bosdyn.api.Vec3\x12\x0e\n\x06radius\x18\x02 \x01(\x01\"F\n\x0f\x44rawableCapsule\x12#\n\tdirection\x18\x01 \x01(\x0b\x32\x10.bosdyn.api.Vec3\x12\x0e\n\x06radius\x18\x02 \x01(\x01\"G\n\x10\x44rawableCylinder\x12#\n\tdirection\x18\x01 \x01(\x0b\x32\x10.bosdyn.api.Vec3\x12\x0e\n\x06radius\x18\x02 \x01(\x01\"5\n\x11\x44rawableLineStrip\x12 \n\x06points\x18\x01 \x01(\x0b\x32\x10.bosdyn.api.Vec3\"2\n\x0e\x44rawablePoints\x12 \n\x06points\x18\x01 \x03(\x0b\x32\x10.bosdyn.api.Vec3*\xd4\x01\n\x0fWorldObjectType\x12\x18\n\x14WORLD_OBJECT_UNKNOWN\x10\x00\x12\x19\n\x15WORLD_OBJECT_DRAWABLE\x10\x01\x12\x19\n\x15WORLD_OBJECT_APRILTAG\x10\x02\x12\"\n\x1eWORLD_OBJECT_IMAGE_COORDINATES\x10\x05\x12\x15\n\x11WORLD_OBJECT_DOCK\x10\x06\x12\x1a\n\x16WORLD_OBJECT_USER_NOGO\x10\x08\x12\x1a\n\x16WORLD_OBJECT_STAIRCASE\x10\tB\x12\x42\x10WorldObjectProtob\x06proto3')
 
 _WORLDOBJECTTYPE = DESCRIPTOR.enum_types_by_name['WorldObjectType']
 WorldObjectType = enum_type_wrapper.EnumTypeWrapper(_WORLDOBJECTTYPE)
 WORLD_OBJECT_UNKNOWN = 0
 WORLD_OBJECT_DRAWABLE = 1
 WORLD_OBJECT_APRILTAG = 2
 WORLD_OBJECT_IMAGE_COORDINATES = 5
 WORLD_OBJECT_DOCK = 6
+WORLD_OBJECT_USER_NOGO = 8
+WORLD_OBJECT_STAIRCASE = 9
 
 
 _WORLDOBJECT = DESCRIPTOR.message_types_by_name['WorldObject']
 _LISTWORLDOBJECTREQUEST = DESCRIPTOR.message_types_by_name['ListWorldObjectRequest']
 _LISTWORLDOBJECTRESPONSE = DESCRIPTOR.message_types_by_name['ListWorldObjectResponse']
 _MUTATEWORLDOBJECTREQUEST = DESCRIPTOR.message_types_by_name['MutateWorldObjectRequest']
 _MUTATEWORLDOBJECTREQUEST_MUTATION = _MUTATEWORLDOBJECTREQUEST.nested_types_by_name['Mutation']
 _MUTATEWORLDOBJECTRESPONSE = DESCRIPTOR.message_types_by_name['MutateWorldObjectResponse']
+_NOGOREGIONPROPERTIES = DESCRIPTOR.message_types_by_name['NoGoRegionProperties']
 _IMAGEPROPERTIES = DESCRIPTOR.message_types_by_name['ImageProperties']
 _DOCKPROPERTIES = DESCRIPTOR.message_types_by_name['DockProperties']
 _APRILTAGPROPERTIES = DESCRIPTOR.message_types_by_name['AprilTagProperties']
 _RAYPROPERTIES = DESCRIPTOR.message_types_by_name['RayProperties']
 _BOUNDINGBOXPROPERTIES = DESCRIPTOR.message_types_by_name['BoundingBoxProperties']
 _DRAWABLEPROPERTIES = DESCRIPTOR.message_types_by_name['DrawableProperties']
 _DRAWABLEPROPERTIES_COLOR = _DRAWABLEPROPERTIES.nested_types_by_name['Color']
+_STAIRCASEPROPERTIES = DESCRIPTOR.message_types_by_name['StaircaseProperties']
 _DRAWABLEFRAME = DESCRIPTOR.message_types_by_name['DrawableFrame']
 _DRAWABLESPHERE = DESCRIPTOR.message_types_by_name['DrawableSphere']
 _DRAWABLEBOX = DESCRIPTOR.message_types_by_name['DrawableBox']
 _DRAWABLEARROW = DESCRIPTOR.message_types_by_name['DrawableArrow']
 _DRAWABLECAPSULE = DESCRIPTOR.message_types_by_name['DrawableCapsule']
 _DRAWABLECYLINDER = DESCRIPTOR.message_types_by_name['DrawableCylinder']
 _DRAWABLELINESTRIP = DESCRIPTOR.message_types_by_name['DrawableLineStrip']
@@ -96,14 +102,21 @@
 MutateWorldObjectResponse = _reflection.GeneratedProtocolMessageType('MutateWorldObjectResponse', (_message.Message,), {
   'DESCRIPTOR' : _MUTATEWORLDOBJECTRESPONSE,
   '__module__' : 'bosdyn.api.world_object_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.MutateWorldObjectResponse)
   })
 _sym_db.RegisterMessage(MutateWorldObjectResponse)
 
+NoGoRegionProperties = _reflection.GeneratedProtocolMessageType('NoGoRegionProperties', (_message.Message,), {
+  'DESCRIPTOR' : _NOGOREGIONPROPERTIES,
+  '__module__' : 'bosdyn.api.world_object_pb2'
+  # @@protoc_insertion_point(class_scope:bosdyn.api.NoGoRegionProperties)
+  })
+_sym_db.RegisterMessage(NoGoRegionProperties)
+
 ImageProperties = _reflection.GeneratedProtocolMessageType('ImageProperties', (_message.Message,), {
   'DESCRIPTOR' : _IMAGEPROPERTIES,
   '__module__' : 'bosdyn.api.world_object_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.ImageProperties)
   })
 _sym_db.RegisterMessage(ImageProperties)
 
@@ -146,14 +159,21 @@
   'DESCRIPTOR' : _DRAWABLEPROPERTIES,
   '__module__' : 'bosdyn.api.world_object_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.DrawableProperties)
   })
 _sym_db.RegisterMessage(DrawableProperties)
 _sym_db.RegisterMessage(DrawableProperties.Color)
 
+StaircaseProperties = _reflection.GeneratedProtocolMessageType('StaircaseProperties', (_message.Message,), {
+  'DESCRIPTOR' : _STAIRCASEPROPERTIES,
+  '__module__' : 'bosdyn.api.world_object_pb2'
+  # @@protoc_insertion_point(class_scope:bosdyn.api.StaircaseProperties)
+  })
+_sym_db.RegisterMessage(StaircaseProperties)
+
 DrawableFrame = _reflection.GeneratedProtocolMessageType('DrawableFrame', (_message.Message,), {
   'DESCRIPTOR' : _DRAWABLEFRAME,
   '__module__' : 'bosdyn.api.world_object_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.DrawableFrame)
   })
 _sym_db.RegisterMessage(DrawableFrame)
 
@@ -206,58 +226,62 @@
   })
 _sym_db.RegisterMessage(DrawablePoints)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'B\020WorldObjectProto'
-  _WORLDOBJECTTYPE._serialized_start=3859
-  _WORLDOBJECTTYPE._serialized_end=4015
-  _WORLDOBJECT._serialized_start=250
-  _WORLDOBJECT._serialized_end=805
-  _LISTWORLDOBJECTREQUEST._serialized_start=808
-  _LISTWORLDOBJECTREQUEST._serialized_end=979
-  _LISTWORLDOBJECTRESPONSE._serialized_start=981
-  _LISTWORLDOBJECTRESPONSE._serialized_end=1098
-  _MUTATEWORLDOBJECTREQUEST._serialized_start=1101
-  _MUTATEWORLDOBJECTREQUEST._serialized_end=1433
-  _MUTATEWORLDOBJECTREQUEST_MUTATION._serialized_start=1237
-  _MUTATEWORLDOBJECTREQUEST_MUTATION._serialized_end=1349
-  _MUTATEWORLDOBJECTREQUEST_ACTION._serialized_start=1351
-  _MUTATEWORLDOBJECTREQUEST_ACTION._serialized_end=1433
-  _MUTATEWORLDOBJECTRESPONSE._serialized_start=1436
-  _MUTATEWORLDOBJECTRESPONSE._serialized_end=1699
-  _MUTATEWORLDOBJECTRESPONSE_STATUS._serialized_start=1598
-  _MUTATEWORLDOBJECTRESPONSE_STATUS._serialized_end=1699
-  _IMAGEPROPERTIES._serialized_start=1702
-  _IMAGEPROPERTIES._serialized_end=1980
-  _DOCKPROPERTIES._serialized_start=1983
-  _DOCKPROPERTIES._serialized_end=2126
-  _APRILTAGPROPERTIES._serialized_start=2129
-  _APRILTAGPROPERTIES._serialized_end=2673
-  _APRILTAGPROPERTIES_APRILTAGPOSESTATUS._serialized_start=2573
-  _APRILTAGPROPERTIES_APRILTAGPOSESTATUS._serialized_end=2673
-  _RAYPROPERTIES._serialized_start=2675
-  _RAYPROPERTIES._serialized_end=2735
-  _BOUNDINGBOXPROPERTIES._serialized_start=2737
-  _BOUNDINGBOXPROPERTIES._serialized_end=2818
-  _DRAWABLEPROPERTIES._serialized_start=2821
-  _DRAWABLEPROPERTIES._serialized_end=3392
-  _DRAWABLEPROPERTIES_COLOR._serialized_start=3329
-  _DRAWABLEPROPERTIES_COLOR._serialized_end=3380
-  _DRAWABLEFRAME._serialized_start=3394
-  _DRAWABLEFRAME._serialized_end=3453
-  _DRAWABLESPHERE._serialized_start=3455
-  _DRAWABLESPHERE._serialized_end=3487
-  _DRAWABLEBOX._serialized_start=3489
-  _DRAWABLEBOX._serialized_end=3534
-  _DRAWABLEARROW._serialized_start=3536
-  _DRAWABLEARROW._serialized_end=3604
-  _DRAWABLECAPSULE._serialized_start=3606
-  _DRAWABLECAPSULE._serialized_end=3676
-  _DRAWABLECYLINDER._serialized_start=3678
-  _DRAWABLECYLINDER._serialized_end=3749
-  _DRAWABLELINESTRIP._serialized_start=3751
-  _DRAWABLELINESTRIP._serialized_end=3804
-  _DRAWABLEPOINTS._serialized_start=3806
-  _DRAWABLEPOINTS._serialized_end=3856
+  _WORLDOBJECTTYPE._serialized_start=4398
+  _WORLDOBJECTTYPE._serialized_end=4610
+  _WORLDOBJECT._serialized_start=307
+  _WORLDOBJECT._serialized_end=1043
+  _LISTWORLDOBJECTREQUEST._serialized_start=1046
+  _LISTWORLDOBJECTREQUEST._serialized_end=1217
+  _LISTWORLDOBJECTRESPONSE._serialized_start=1219
+  _LISTWORLDOBJECTRESPONSE._serialized_end=1336
+  _MUTATEWORLDOBJECTREQUEST._serialized_start=1339
+  _MUTATEWORLDOBJECTREQUEST._serialized_end=1671
+  _MUTATEWORLDOBJECTREQUEST_MUTATION._serialized_start=1475
+  _MUTATEWORLDOBJECTREQUEST_MUTATION._serialized_end=1587
+  _MUTATEWORLDOBJECTREQUEST_ACTION._serialized_start=1589
+  _MUTATEWORLDOBJECTREQUEST_ACTION._serialized_end=1671
+  _MUTATEWORLDOBJECTRESPONSE._serialized_start=1674
+  _MUTATEWORLDOBJECTRESPONSE._serialized_end=1971
+  _MUTATEWORLDOBJECTRESPONSE_STATUS._serialized_start=1837
+  _MUTATEWORLDOBJECTRESPONSE_STATUS._serialized_end=1971
+  _NOGOREGIONPROPERTIES._serialized_start=1974
+  _NOGOREGIONPROPERTIES._serialized_end=2173
+  _IMAGEPROPERTIES._serialized_start=2176
+  _IMAGEPROPERTIES._serialized_end=2454
+  _DOCKPROPERTIES._serialized_start=2457
+  _DOCKPROPERTIES._serialized_end=2600
+  _APRILTAGPROPERTIES._serialized_start=2603
+  _APRILTAGPROPERTIES._serialized_end=3147
+  _APRILTAGPROPERTIES_APRILTAGPOSESTATUS._serialized_start=3047
+  _APRILTAGPROPERTIES_APRILTAGPOSESTATUS._serialized_end=3147
+  _RAYPROPERTIES._serialized_start=3149
+  _RAYPROPERTIES._serialized_end=3209
+  _BOUNDINGBOXPROPERTIES._serialized_start=3211
+  _BOUNDINGBOXPROPERTIES._serialized_end=3292
+  _DRAWABLEPROPERTIES._serialized_start=3295
+  _DRAWABLEPROPERTIES._serialized_end=3866
+  _DRAWABLEPROPERTIES_COLOR._serialized_start=3803
+  _DRAWABLEPROPERTIES_COLOR._serialized_end=3854
+  _STAIRCASEPROPERTIES._serialized_start=3868
+  _STAIRCASEPROPERTIES._serialized_end=3931
+  _DRAWABLEFRAME._serialized_start=3933
+  _DRAWABLEFRAME._serialized_end=3992
+  _DRAWABLESPHERE._serialized_start=3994
+  _DRAWABLESPHERE._serialized_end=4026
+  _DRAWABLEBOX._serialized_start=4028
+  _DRAWABLEBOX._serialized_end=4073
+  _DRAWABLEARROW._serialized_start=4075
+  _DRAWABLEARROW._serialized_end=4143
+  _DRAWABLECAPSULE._serialized_start=4145
+  _DRAWABLECAPSULE._serialized_end=4215
+  _DRAWABLECYLINDER._serialized_start=4217
+  _DRAWABLECYLINDER._serialized_end=4288
+  _DRAWABLELINESTRIP._serialized_start=4290
+  _DRAWABLELINESTRIP._serialized_end=4343
+  _DRAWABLEPOINTS._serialized_start=4345
+  _DRAWABLEPOINTS._serialized_end=4395
 # @@protoc_insertion_point(module_scope)
```

## bosdyn/api/world_object_service_pb2_grpc.py

```diff
@@ -2,15 +2,16 @@
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
 from bosdyn.api import world_object_pb2 as bosdyn_dot_api_dot_world__object__pb2
 
 
 class WorldObjectServiceStub(object):
-    """The world object service provides a way to track and store objects detected in the world around the robot.
+    """The world object service provides a way to track and store objects detected in the world around
+    the robot.
     """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
@@ -24,15 +25,16 @@
                 '/bosdyn.api.WorldObjectService/MutateWorldObjects',
                 request_serializer=bosdyn_dot_api_dot_world__object__pb2.MutateWorldObjectRequest.SerializeToString,
                 response_deserializer=bosdyn_dot_api_dot_world__object__pb2.MutateWorldObjectResponse.FromString,
                 )
 
 
 class WorldObjectServiceServicer(object):
-    """The world object service provides a way to track and store objects detected in the world around the robot.
+    """The world object service provides a way to track and store objects detected in the world around
+    the robot.
     """
 
     def ListWorldObjects(self, request, context):
         """Request a list of all the world objects in the robot's perception scene.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
@@ -62,15 +64,16 @@
     generic_handler = grpc.method_handlers_generic_handler(
             'bosdyn.api.WorldObjectService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
 class WorldObjectService(object):
-    """The world object service provides a way to track and store objects detected in the world around the robot.
+    """The world object service provides a way to track and store objects detected in the world around
+    the robot.
     """
 
     @staticmethod
     def ListWorldObjects(request,
             target,
             options=(),
             channel_credentials=None,
```

## bosdyn/api/auto_return/__init__.py

```diff
@@ -0,0 +1,4 @@
+00000000: 5f5f 7061 7468 5f5f 203d 205f 5f69 6d70  __path__ = __imp
+00000010: 6f72 745f 5f28 2770 6b67 7574 696c 2729  ort__('pkgutil')
+00000020: 2e65 7874 656e 645f 7061 7468 285f 5f70  .extend_path(__p
+00000030: 6174 685f 5f2c 205f 5f6e 616d 655f 5f29  ath__, __name__)
```

## bosdyn/api/auto_return/auto_return_pb2.py

```diff
@@ -14,26 +14,27 @@
 
 from google.protobuf import any_pb2 as google_dot_protobuf_dot_any__pb2
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from bosdyn.api import header_pb2 as bosdyn_dot_api_dot_header__pb2
 from bosdyn.api import lease_pb2 as bosdyn_dot_api_dot_lease__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(bosdyn/api/auto_return/auto_return.proto\x12\x16\x62osdyn.api.auto_return\x1a\x19google/protobuf/any.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x17\x62osdyn/api/header.proto\x1a\x16\x62osdyn/api/lease.proto\"\x82\x01\n\x06Params\x12-\n\x0fmobility_params\x18\x01 \x01(\x0b\x32\x14.google.protobuf.Any\x12\x18\n\x10max_displacement\x18\x02 \x01(\x02\x12/\n\x0cmax_duration\x18\x03 \x01(\x0b\x32\x19.google.protobuf.Duration\"\xa6\x01\n\x10\x43onfigureRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12!\n\x06leases\x18\x02 \x03(\x0b\x32\x11.bosdyn.api.Lease\x12.\n\x06params\x18\x03 \x01(\x0b\x32\x1e.bosdyn.api.auto_return.Params\x12\x14\n\x0c\x63lear_buffer\x18\x04 \x01(\x08\"\x81\x02\n\x11\x43onfigureResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12@\n\x06status\x18\x02 \x01(\x0e\x32\x30.bosdyn.api.auto_return.ConfigureResponse.Status\x12\x36\n\x0einvalid_params\x18\x03 \x01(\x0b\x32\x1e.bosdyn.api.auto_return.Params\"F\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x19\n\x15STATUS_INVALID_PARAMS\x10\x02\"D\n\x17GetConfigurationRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"\x92\x01\n\x18GetConfigurationResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x0f\n\x07\x65nabled\x18\x02 \x01(\x08\x12\x39\n\x07request\x18\x03 \x01(\x0b\x32(.bosdyn.api.auto_return.ConfigureRequest\"9\n\x0cStartRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\";\n\rStartResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeaderB\x11\x42\x0f\x41utoReturnProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(bosdyn/api/auto_return/auto_return.proto\x12\x16\x62osdyn.api.auto_return\x1a\x19google/protobuf/any.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x17\x62osdyn/api/header.proto\x1a\x16\x62osdyn/api/lease.proto\"\x82\x01\n\x06Params\x12-\n\x0fmobility_params\x18\x01 \x01(\x0b\x32\x14.google.protobuf.Any\x12\x18\n\x10max_displacement\x18\x02 \x01(\x02\x12/\n\x0cmax_duration\x18\x03 \x01(\x0b\x32\x19.google.protobuf.Duration\"\xa6\x01\n\x10\x43onfigureRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12!\n\x06leases\x18\x02 \x03(\x0b\x32\x11.bosdyn.api.Lease\x12.\n\x06params\x18\x03 \x01(\x0b\x32\x1e.bosdyn.api.auto_return.Params\x12\x14\n\x0c\x63lear_buffer\x18\x04 \x01(\x08\"\x81\x02\n\x11\x43onfigureResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12@\n\x06status\x18\x02 \x01(\x0e\x32\x30.bosdyn.api.auto_return.ConfigureResponse.Status\x12\x36\n\x0einvalid_params\x18\x03 \x01(\x0b\x32\x1e.bosdyn.api.auto_return.Params\"F\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x19\n\x15STATUS_INVALID_PARAMS\x10\x02\"D\n\x17GetConfigurationRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"\x92\x01\n\x18GetConfigurationResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x0f\n\x07\x65nabled\x18\x02 \x01(\x08\x12\x39\n\x07request\x18\x03 \x01(\x0b\x32(.bosdyn.api.auto_return.ConfigureRequest\"\x8c\x01\n\x0cStartRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12!\n\x06leases\x18\x02 \x03(\x0b\x32\x11.bosdyn.api.Lease\x12.\n\x06params\x18\x03 \x01(\x0b\x32\x1e.bosdyn.api.auto_return.Params\"\xf9\x01\n\rStartResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12<\n\x06status\x18\x02 \x01(\x0e\x32,.bosdyn.api.auto_return.StartResponse.Status\x12\x36\n\x0einvalid_params\x18\x03 \x01(\x0b\x32\x1e.bosdyn.api.auto_return.Params\"F\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x19\n\x15STATUS_INVALID_PARAMS\x10\x02\x42\x11\x42\x0f\x41utoReturnProtob\x06proto3')
 
 
 
 _PARAMS = DESCRIPTOR.message_types_by_name['Params']
 _CONFIGUREREQUEST = DESCRIPTOR.message_types_by_name['ConfigureRequest']
 _CONFIGURERESPONSE = DESCRIPTOR.message_types_by_name['ConfigureResponse']
 _GETCONFIGURATIONREQUEST = DESCRIPTOR.message_types_by_name['GetConfigurationRequest']
 _GETCONFIGURATIONRESPONSE = DESCRIPTOR.message_types_by_name['GetConfigurationResponse']
 _STARTREQUEST = DESCRIPTOR.message_types_by_name['StartRequest']
 _STARTRESPONSE = DESCRIPTOR.message_types_by_name['StartResponse']
 _CONFIGURERESPONSE_STATUS = _CONFIGURERESPONSE.enum_types_by_name['Status']
+_STARTRESPONSE_STATUS = _STARTRESPONSE.enum_types_by_name['Status']
 Params = _reflection.GeneratedProtocolMessageType('Params', (_message.Message,), {
   'DESCRIPTOR' : _PARAMS,
   '__module__' : 'bosdyn.api.auto_return.auto_return_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.auto_return.Params)
   })
 _sym_db.RegisterMessage(Params)
 
@@ -91,12 +92,14 @@
   _CONFIGURERESPONSE._serialized_end=736
   _CONFIGURERESPONSE_STATUS._serialized_start=666
   _CONFIGURERESPONSE_STATUS._serialized_end=736
   _GETCONFIGURATIONREQUEST._serialized_start=738
   _GETCONFIGURATIONREQUEST._serialized_end=806
   _GETCONFIGURATIONRESPONSE._serialized_start=809
   _GETCONFIGURATIONRESPONSE._serialized_end=955
-  _STARTREQUEST._serialized_start=957
-  _STARTREQUEST._serialized_end=1014
-  _STARTRESPONSE._serialized_start=1016
-  _STARTRESPONSE._serialized_end=1075
+  _STARTREQUEST._serialized_start=958
+  _STARTREQUEST._serialized_end=1098
+  _STARTRESPONSE._serialized_start=1101
+  _STARTRESPONSE._serialized_end=1350
+  _STARTRESPONSE_STATUS._serialized_start=666
+  _STARTRESPONSE_STATUS._serialized_end=736
 # @@protoc_insertion_point(module_scope)
```

## bosdyn/api/autowalk/__init__.py

```diff
@@ -0,0 +1,4 @@
+00000000: 5f5f 7061 7468 5f5f 203d 205f 5f69 6d70  __path__ = __imp
+00000010: 6f72 745f 5f28 2770 6b67 7574 696c 2729  ort__('pkgutil')
+00000020: 2e65 7874 656e 645f 7061 7468 285f 5f70  .extend_path(__p
+00000030: 6174 685f 5f2c 205f 5f6e 616d 655f 5f29  ath__, __name__)
```

## bosdyn/api/autowalk/walks_pb2.py

```diff
@@ -16,23 +16,25 @@
 from bosdyn.api.mission import nodes_pb2 as bosdyn_dot_api_dot_mission_dot_nodes__pb2
 from bosdyn.api.mission import util_pb2 as bosdyn_dot_api_dot_mission_dot_util__pb2
 from bosdyn.api import data_acquisition_pb2 as bosdyn_dot_api_dot_data__acquisition__pb2
 from bosdyn.api.graph_nav import graph_nav_pb2 as bosdyn_dot_api_dot_graph__nav_dot_graph__nav__pb2
 from bosdyn.api.graph_nav import nav_pb2 as bosdyn_dot_api_dot_graph__nav_dot_nav__pb2
 from bosdyn.api import gripper_command_pb2 as bosdyn_dot_api_dot_gripper__command__pb2
 from bosdyn.api import geometry_pb2 as bosdyn_dot_api_dot_geometry__pb2
+from bosdyn.api import image_pb2 as bosdyn_dot_api_dot_image__pb2
+from bosdyn.api import service_customization_pb2 as bosdyn_dot_api_dot_service__customization__pb2
 from bosdyn.api import trajectory_pb2 as bosdyn_dot_api_dot_trajectory__pb2
 from bosdyn.api.spot_cam import ptz_pb2 as bosdyn_dot_api_dot_spot__cam_dot_ptz__pb2
 from bosdyn.api.spot import robot_command_pb2 as bosdyn_dot_api_dot_spot_dot_robot__command__pb2
 from bosdyn.api import arm_command_pb2 as bosdyn_dot_api_dot_arm__command__pb2
 from bosdyn.api import basic_command_pb2 as bosdyn_dot_api_dot_basic__command__pb2
 from bosdyn.api import gripper_camera_param_pb2 as bosdyn_dot_api_dot_gripper__camera__param__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1f\x62osdyn/api/autowalk/walks.proto\x12\x13\x62osdyn.api.autowalk\x1a\x1egoogle/protobuf/duration.proto\x1a\x1e\x62osdyn/api/mission/nodes.proto\x1a\x1d\x62osdyn/api/mission/util.proto\x1a!bosdyn/api/data_acquisition.proto\x1a$bosdyn/api/graph_nav/graph_nav.proto\x1a\x1e\x62osdyn/api/graph_nav/nav.proto\x1a bosdyn/api/gripper_command.proto\x1a\x19\x62osdyn/api/geometry.proto\x1a\x1b\x62osdyn/api/trajectory.proto\x1a\x1d\x62osdyn/api/spot_cam/ptz.proto\x1a#bosdyn/api/spot/robot_command.proto\x1a\x1c\x62osdyn/api/arm_command.proto\x1a\x1e\x62osdyn/api/basic_command.proto\x1a%bosdyn/api/gripper_camera_param.proto\"\x8a\x02\n\x04Walk\x12@\n\x11global_parameters\x18\x01 \x01(\x0b\x32%.bosdyn.api.autowalk.GlobalParameters\x12\x38\n\rplayback_mode\x18\x02 \x01(\x0b\x32!.bosdyn.api.autowalk.PlaybackMode\x12\x10\n\x08map_name\x18\x07 \x01(\t\x12\x14\n\x0cmission_name\x18\x04 \x01(\t\x12.\n\x08\x65lements\x18\x05 \x03(\x0b\x32\x1c.bosdyn.api.autowalk.Element\x12(\n\x05\x64ocks\x18\x06 \x03(\x0b\x32\x19.bosdyn.api.autowalk.DockJ\x04\x08\x03\x10\x04\"\xbf\x01\n\x10GlobalParameters\x12\x12\n\ngroup_name\x18\x01 \x01(\t\x12\x1c\n\x14should_autofocus_ptz\x18\x02 \x01(\x08\x12\x1b\n\x13self_right_attempts\x18\x03 \x01(\x05\x12\x46\n\x16post_mission_callbacks\x18\x04 \x03(\x0b\x32&.bosdyn.api.autowalk.Action.RemoteGrpc\x12\x14\n\x0cskip_actions\x18\x05 \x01(\x08\"\x9e\x01\n\x04\x44ock\x12\x0f\n\x07\x64ock_id\x18\x01 \x01(\r\x12\x1a\n\x12\x64ocked_waypoint_id\x18\x02 \x01(\t\x12\x35\n\x10target_prep_pose\x18\x03 \x01(\x0b\x32\x1b.bosdyn.api.autowalk.Target\x12\x32\n\x0fprompt_duration\x18\x04 \x01(\x0b\x32\x19.google.protobuf.Duration\"\xdd\x02\n\x0cPlaybackMode\x12\x36\n\x04once\x18\x02 \x01(\x0b\x32&.bosdyn.api.autowalk.PlaybackMode.OnceH\x00\x12>\n\x08periodic\x18\x03 \x01(\x0b\x32*.bosdyn.api.autowalk.PlaybackMode.PeriodicH\x00\x12\x42\n\ncontinuous\x18\x04 \x01(\x0b\x32,.bosdyn.api.autowalk.PlaybackMode.ContinuousH\x00\x1a-\n\x04Once\x12%\n\x1dskip_docking_after_completion\x18\x01 \x01(\x08\x1aL\n\x08Periodic\x12+\n\x08interval\x18\x01 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x13\n\x0brepetitions\x18\x02 \x01(\x05\x1a\x0c\n\nContinuousB\x06\n\x04mode\"\xc1\x03\n\x07\x45lement\x12\x0c\n\x04name\x18\x01 \x01(\t\x12+\n\x06target\x18\x02 \x01(\x0b\x32\x1b.bosdyn.api.autowalk.Target\x12\x45\n\x17target_failure_behavior\x18\x03 \x01(\x0b\x32$.bosdyn.api.autowalk.FailureBehavior\x12+\n\x06\x61\x63tion\x18\x04 \x01(\x0b\x32\x1b.bosdyn.api.autowalk.Action\x12:\n\x0e\x61\x63tion_wrapper\x18\x05 \x01(\x0b\x32\".bosdyn.api.autowalk.ActionWrapper\x12\x45\n\x17\x61\x63tion_failure_behavior\x18\x06 \x01(\x0b\x32$.bosdyn.api.autowalk.FailureBehavior\x12\x12\n\nis_skipped\x18\x07 \x01(\x08\x12<\n\x0f\x62\x61ttery_monitor\x18\x08 \x01(\x0b\x32#.bosdyn.api.autowalk.BatteryMonitor\x12\x32\n\x0f\x61\x63tion_duration\x18\t \x01(\x0b\x32\x19.google.protobuf.Duration\"\x92\x04\n\x06Target\x12=\n\x0bnavigate_to\x18\x01 \x01(\x0b\x32&.bosdyn.api.autowalk.Target.NavigateToH\x00\x12\x43\n\x0enavigate_route\x18\x02 \x01(\x0b\x32).bosdyn.api.autowalk.Target.NavigateRouteH\x00\x12:\n\nrelocalize\x18\x03 \x01(\x0b\x32&.bosdyn.api.autowalk.Target.Relocalize\x1a\\\n\nRelocalize\x12N\n\x18set_localization_request\x18\x01 \x01(\x0b\x32,.bosdyn.api.graph_nav.SetLocalizationRequest\x1ah\n\nNavigateTo\x12\x1f\n\x17\x64\x65stination_waypoint_id\x18\x01 \x01(\t\x12\x39\n\rtravel_params\x18\x03 \x01(\x0b\x32\".bosdyn.api.graph_nav.TravelParams\x1av\n\rNavigateRoute\x12*\n\x05route\x18\x01 \x01(\x0b\x32\x1b.bosdyn.api.graph_nav.Route\x12\x39\n\rtravel_params\x18\x02 \x01(\x0b\x32\".bosdyn.api.graph_nav.TravelParamsB\x08\n\x06target\"\xf1\x04\n\x06\x41\x63tion\x12\x32\n\x05sleep\x18\x01 \x01(\x0b\x32!.bosdyn.api.autowalk.Action.SleepH\x00\x12G\n\x10\x64\x61ta_acquisition\x18\x02 \x01(\x0b\x32+.bosdyn.api.autowalk.Action.DataAcquisitionH\x00\x12=\n\x0bremote_grpc\x18\x03 \x01(\x0b\x32&.bosdyn.api.autowalk.Action.RemoteGrpcH\x00\x12(\n\x04node\x18\x04 \x01(\x0b\x32\x18.bosdyn.api.mission.NodeH\x00\x1a\x34\n\x05Sleep\x12+\n\x08\x64uration\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration\x1a\xa4\x01\n\x0f\x44\x61taAcquisition\x12<\n\x14\x61\x63quire_data_request\x18\x01 \x01(\x0b\x32\x1e.bosdyn.api.AcquireDataRequest\x12S\n\x13\x63ompletion_behavior\x18\x02 \x01(\x0e\x32\x36.bosdyn.api.mission.DataAcquisition.CompletionBehavior\x1a\x99\x01\n\nRemoteGrpc\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12.\n\x0brpc_timeout\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x17\n\x0flease_resources\x18\x03 \x03(\t\x12,\n\x06inputs\x18\x04 \x03(\x0b\x32\x1c.bosdyn.api.mission.KeyValueB\x08\n\x06\x61\x63tion\"\xd3\n\n\rActionWrapper\x12G\n\x0erobot_body_sit\x18\x01 \x01(\x0b\x32/.bosdyn.api.autowalk.ActionWrapper.RobotBodySit\x12I\n\x0frobot_body_pose\x18\x02 \x01(\x0b\x32\x30.bosdyn.api.autowalk.ActionWrapper.RobotBodyPose\x12\x43\n\x0cspot_cam_led\x18\x04 \x01(\x0b\x32-.bosdyn.api.autowalk.ActionWrapper.SpotCamLed\x12\x43\n\x0cspot_cam_ptz\x18\x05 \x01(\x0b\x32-.bosdyn.api.autowalk.ActionWrapper.SpotCamPtz\x12Q\n\x13\x61rm_sensor_pointing\x18\x06 \x01(\x0b\x32\x34.bosdyn.api.autowalk.ActionWrapper.ArmSensorPointing\x12U\n\x15gripper_camera_params\x18\x07 \x01(\x0b\x32\x36.bosdyn.api.autowalk.ActionWrapper.GripperCameraParams\x12J\n\x0fgripper_command\x18\x08 \x01(\x0b\x32\x31.bosdyn.api.autowalk.ActionWrapper.GripperCommand\x1a\x0e\n\x0cRobotBodySit\x1a?\n\rRobotBodyPose\x12.\n\x11target_tform_body\x18\x01 \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\x1a\x98\x01\n\nSpotCamLed\x12U\n\x0c\x62rightnesses\x18\x01 \x03(\x0b\x32?.bosdyn.api.autowalk.ActionWrapper.SpotCamLed.BrightnessesEntry\x1a\x33\n\x11\x42rightnessesEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\x02:\x02\x38\x01\x1a\x44\n\nSpotCamPtz\x12\x36\n\x0cptz_position\x18\x01 \x01(\x0b\x32 .bosdyn.api.spot_cam.PtzPosition\x1a\xec\x02\n\x11\x41rmSensorPointing\x12\x38\n\x10joint_trajectory\x18\x02 \x01(\x0b\x32\x1e.bosdyn.api.ArmJointTrajectory\x12-\n\x10wrist_tform_tool\x18\x03 \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\x12<\n\x19pose_trajectory_rt_target\x18\x04 \x01(\x0b\x32\x19.bosdyn.api.SE3Trajectory\x12\x39\n\x1ctarget_tform_measured_offset\x18\x07 \x01(\x0b\x32\x13.bosdyn.api.SE2Pose\x12X\n\x12\x62ody_assist_params\x18\x05 \x01(\x0b\x32<.bosdyn.api.spot.BodyControlParams.BodyAssistForManipulation\x12\x1b\n\x13\x66orce_stow_override\x18\x06 \x01(\x08\x1a\x46\n\x13GripperCameraParams\x12/\n\x06params\x18\x01 \x01(\x0b\x32\x1f.bosdyn.api.GripperCameraParams\x1a\x45\n\x0eGripperCommand\x12\x33\n\x07request\x18\x01 \x01(\x0b\x32\".bosdyn.api.GripperCommand.Request\"\xb3\x05\n\x0f\x46\x61ilureBehavior\x12\x13\n\x0bretry_count\x18\x01 \x01(\x05\x12\x32\n\x0fprompt_duration\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration\x12K\n\x0esafe_power_off\x18\x03 \x01(\x0b\x32\x31.bosdyn.api.autowalk.FailureBehavior.SafePowerOffH\x00\x12M\n\x0fproceed_if_able\x18\x04 \x01(\x0b\x32\x32.bosdyn.api.autowalk.FailureBehavior.ProceedIfAbleH\x00\x12q\n#return_to_start_and_try_again_later\x18\x05 \x01(\x0b\x32\x42.bosdyn.api.autowalk.FailureBehavior.ReturnToStartAndTryAgainLaterH\x00\x12g\n\x1dreturn_to_start_and_terminate\x18\x06 \x01(\x0b\x32>.bosdyn.api.autowalk.FailureBehavior.ReturnToStartAndTerminateH\x00\x1aH\n\x0cSafePowerOff\x12\x38\n\x07request\x18\x01 \x01(\x0b\x32\'.bosdyn.api.SafePowerOffCommand.Request\x1a\x0f\n\rProceedIfAble\x1aS\n\x1dReturnToStartAndTryAgainLater\x12\x32\n\x0ftry_again_delay\x18\x01 \x01(\x0b\x32\x19.google.protobuf.Duration\x1a\x1b\n\x19ReturnToStartAndTerminateB\x12\n\x10\x64\x65\x66\x61ult_behavior\"Q\n\x0e\x42\x61tteryMonitor\x12\x1f\n\x17\x62\x61ttery_start_threshold\x18\x02 \x01(\x02\x12\x1e\n\x16\x62\x61ttery_stop_threshold\x18\x03 \x01(\x02\x42\x0c\x42\nWalksProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1f\x62osdyn/api/autowalk/walks.proto\x12\x13\x62osdyn.api.autowalk\x1a\x1egoogle/protobuf/duration.proto\x1a\x1e\x62osdyn/api/mission/nodes.proto\x1a\x1d\x62osdyn/api/mission/util.proto\x1a!bosdyn/api/data_acquisition.proto\x1a$bosdyn/api/graph_nav/graph_nav.proto\x1a\x1e\x62osdyn/api/graph_nav/nav.proto\x1a bosdyn/api/gripper_command.proto\x1a\x19\x62osdyn/api/geometry.proto\x1a\x16\x62osdyn/api/image.proto\x1a&bosdyn/api/service_customization.proto\x1a\x1b\x62osdyn/api/trajectory.proto\x1a\x1d\x62osdyn/api/spot_cam/ptz.proto\x1a#bosdyn/api/spot/robot_command.proto\x1a\x1c\x62osdyn/api/arm_command.proto\x1a\x1e\x62osdyn/api/basic_command.proto\x1a%bosdyn/api/gripper_camera_param.proto\"\x96\x02\n\x04Walk\x12@\n\x11global_parameters\x18\x01 \x01(\x0b\x32%.bosdyn.api.autowalk.GlobalParameters\x12\x38\n\rplayback_mode\x18\x02 \x01(\x0b\x32!.bosdyn.api.autowalk.PlaybackMode\x12\x10\n\x08map_name\x18\x07 \x01(\t\x12\x14\n\x0cmission_name\x18\x04 \x01(\t\x12.\n\x08\x65lements\x18\x05 \x03(\x0b\x32\x1c.bosdyn.api.autowalk.Element\x12(\n\x05\x64ocks\x18\x06 \x03(\x0b\x32\x19.bosdyn.api.autowalk.Dock\x12\n\n\x02id\x18\x08 \x01(\tJ\x04\x08\x03\x10\x04\"\xbf\x01\n\x10GlobalParameters\x12\x12\n\ngroup_name\x18\x01 \x01(\t\x12\x1c\n\x14should_autofocus_ptz\x18\x02 \x01(\x08\x12\x1b\n\x13self_right_attempts\x18\x03 \x01(\x05\x12\x46\n\x16post_mission_callbacks\x18\x04 \x03(\x0b\x32&.bosdyn.api.autowalk.Action.RemoteGrpc\x12\x14\n\x0cskip_actions\x18\x05 \x01(\x08\"\x9e\x01\n\x04\x44ock\x12\x0f\n\x07\x64ock_id\x18\x01 \x01(\r\x12\x1a\n\x12\x64ocked_waypoint_id\x18\x02 \x01(\t\x12\x35\n\x10target_prep_pose\x18\x03 \x01(\x0b\x32\x1b.bosdyn.api.autowalk.Target\x12\x32\n\x0fprompt_duration\x18\x04 \x01(\x0b\x32\x19.google.protobuf.Duration\"\xdd\x02\n\x0cPlaybackMode\x12\x36\n\x04once\x18\x02 \x01(\x0b\x32&.bosdyn.api.autowalk.PlaybackMode.OnceH\x00\x12>\n\x08periodic\x18\x03 \x01(\x0b\x32*.bosdyn.api.autowalk.PlaybackMode.PeriodicH\x00\x12\x42\n\ncontinuous\x18\x04 \x01(\x0b\x32,.bosdyn.api.autowalk.PlaybackMode.ContinuousH\x00\x1a-\n\x04Once\x12%\n\x1dskip_docking_after_completion\x18\x01 \x01(\x08\x1aL\n\x08Periodic\x12+\n\x08interval\x18\x01 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x13\n\x0brepetitions\x18\x02 \x01(\x05\x1a\x0c\n\nContinuousB\x06\n\x04mode\"\xcd\x03\n\x07\x45lement\x12\x0c\n\x04name\x18\x01 \x01(\t\x12+\n\x06target\x18\x02 \x01(\x0b\x32\x1b.bosdyn.api.autowalk.Target\x12\x45\n\x17target_failure_behavior\x18\x03 \x01(\x0b\x32$.bosdyn.api.autowalk.FailureBehavior\x12+\n\x06\x61\x63tion\x18\x04 \x01(\x0b\x32\x1b.bosdyn.api.autowalk.Action\x12:\n\x0e\x61\x63tion_wrapper\x18\x05 \x01(\x0b\x32\".bosdyn.api.autowalk.ActionWrapper\x12\x45\n\x17\x61\x63tion_failure_behavior\x18\x06 \x01(\x0b\x32$.bosdyn.api.autowalk.FailureBehavior\x12\x12\n\nis_skipped\x18\x07 \x01(\x08\x12<\n\x0f\x62\x61ttery_monitor\x18\x08 \x01(\x0b\x32#.bosdyn.api.autowalk.BatteryMonitor\x12\x32\n\x0f\x61\x63tion_duration\x18\t \x01(\x0b\x32\x19.google.protobuf.Duration\x12\n\n\x02id\x18\n \x01(\t\"\x92\x04\n\x06Target\x12=\n\x0bnavigate_to\x18\x01 \x01(\x0b\x32&.bosdyn.api.autowalk.Target.NavigateToH\x00\x12\x43\n\x0enavigate_route\x18\x02 \x01(\x0b\x32).bosdyn.api.autowalk.Target.NavigateRouteH\x00\x12:\n\nrelocalize\x18\x03 \x01(\x0b\x32&.bosdyn.api.autowalk.Target.Relocalize\x1a\\\n\nRelocalize\x12N\n\x18set_localization_request\x18\x01 \x01(\x0b\x32,.bosdyn.api.graph_nav.SetLocalizationRequest\x1ah\n\nNavigateTo\x12\x1f\n\x17\x64\x65stination_waypoint_id\x18\x01 \x01(\t\x12\x39\n\rtravel_params\x18\x03 \x01(\x0b\x32\".bosdyn.api.graph_nav.TravelParams\x1av\n\rNavigateRoute\x12*\n\x05route\x18\x01 \x01(\x0b\x32\x1b.bosdyn.api.graph_nav.Route\x12\x39\n\rtravel_params\x18\x02 \x01(\x0b\x32\".bosdyn.api.graph_nav.TravelParamsB\x08\n\x06target\"\xf2\x06\n\x06\x41\x63tion\x12\x32\n\x05sleep\x18\x01 \x01(\x0b\x32!.bosdyn.api.autowalk.Action.SleepH\x00\x12G\n\x10\x64\x61ta_acquisition\x18\x02 \x01(\x0b\x32+.bosdyn.api.autowalk.Action.DataAcquisitionH\x00\x12=\n\x0bremote_grpc\x18\x03 \x01(\x0b\x32&.bosdyn.api.autowalk.Action.RemoteGrpcH\x00\x12(\n\x04node\x18\x04 \x01(\x0b\x32\x18.bosdyn.api.mission.NodeH\x00\x1a\x34\n\x05Sleep\x12+\n\x08\x64uration\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration\x1a\xab\x02\n\x0f\x44\x61taAcquisition\x12<\n\x14\x61\x63quire_data_request\x18\x01 \x01(\x0b\x32\x1e.bosdyn.api.AcquireDataRequest\x12S\n\x13\x63ompletion_behavior\x18\x02 \x01(\x0e\x32\x36.bosdyn.api.mission.DataAcquisition.CompletionBehavior\x12\x46\n\x17last_known_capabilities\x18\x03 \x01(\x0b\x32%.bosdyn.api.AcquisitionCapabilityList\x12=\n\x12record_time_images\x18\x04 \x03(\x0b\x32!.bosdyn.api.ImageCaptureAndSource\x1a\x93\x02\n\nRemoteGrpc\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12.\n\x0brpc_timeout\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x17\n\x0flease_resources\x18\x03 \x03(\t\x12\x30\n\x06inputs\x18\x04 \x03(\x0b\x32\x1c.bosdyn.api.mission.KeyValueB\x02\x18\x01\x12\x35\n\nparameters\x18\x05 \x01(\x0b\x32!.bosdyn.api.CustomParamCollection\x12=\n\x12record_time_images\x18\x06 \x03(\x0b\x32!.bosdyn.api.ImageCaptureAndSourceB\x08\n\x06\x61\x63tion\"\xd7\r\n\rActionWrapper\x12G\n\x0erobot_body_sit\x18\x01 \x01(\x0b\x32/.bosdyn.api.autowalk.ActionWrapper.RobotBodySit\x12I\n\x0frobot_body_pose\x18\x02 \x01(\x0b\x32\x30.bosdyn.api.autowalk.ActionWrapper.RobotBodyPose\x12\x43\n\x0cspot_cam_led\x18\x04 \x01(\x0b\x32-.bosdyn.api.autowalk.ActionWrapper.SpotCamLed\x12\x43\n\x0cspot_cam_ptz\x18\x05 \x01(\x0b\x32-.bosdyn.api.autowalk.ActionWrapper.SpotCamPtz\x12Q\n\x13\x61rm_sensor_pointing\x18\x06 \x01(\x0b\x32\x34.bosdyn.api.autowalk.ActionWrapper.ArmSensorPointing\x12O\n\x12spot_cam_alignment\x18\t \x01(\x0b\x32\x33.bosdyn.api.autowalk.ActionWrapper.SpotCamAlignment\x12U\n\x15gripper_camera_params\x18\x07 \x01(\x0b\x32\x36.bosdyn.api.autowalk.ActionWrapper.GripperCameraParams\x12J\n\x0fgripper_command\x18\x08 \x01(\x0b\x32\x31.bosdyn.api.autowalk.ActionWrapper.GripperCommand\x1a\x0e\n\x0cRobotBodySit\x1a?\n\rRobotBodyPose\x12.\n\x11target_tform_body\x18\x01 \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\x1a\x98\x01\n\nSpotCamLed\x12U\n\x0c\x62rightnesses\x18\x01 \x03(\x0b\x32?.bosdyn.api.autowalk.ActionWrapper.SpotCamLed.BrightnessesEntry\x1a\x33\n\x11\x42rightnessesEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\x02:\x02\x38\x01\x1a\x44\n\nSpotCamPtz\x12\x36\n\x0cptz_position\x18\x01 \x01(\x0b\x32 .bosdyn.api.spot_cam.PtzPosition\x1a\xb0\x02\n\x10SpotCamAlignment\x12Q\n\nalignments\x18\x02 \x03(\x0b\x32=.bosdyn.api.autowalk.ActionWrapper.SpotCamAlignment.Alignment\x12\x30\n\x13target_tform_sensor\x18\x03 \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\x12\x12\n\nfinal_zoom\x18\x04 \x01(\x02\x12\x19\n\x11target_sensor_ids\x18\x05 \x03(\t\x1ah\n\tAlignment\x12\x0c\n\x04zoom\x18\x01 \x01(\x02\x12\x11\n\tsensor_id\x18\x02 \x01(\t\x12\x19\n\x0fscene_object_id\x18\x03 \x01(\tH\x00\x12\x12\n\nis_skipped\x18\x04 \x01(\x08\x42\x0b\n\treference\x1a\xec\x02\n\x11\x41rmSensorPointing\x12\x38\n\x10joint_trajectory\x18\x02 \x01(\x0b\x32\x1e.bosdyn.api.ArmJointTrajectory\x12-\n\x10wrist_tform_tool\x18\x03 \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\x12<\n\x19pose_trajectory_rt_target\x18\x04 \x01(\x0b\x32\x19.bosdyn.api.SE3Trajectory\x12\x39\n\x1ctarget_tform_measured_offset\x18\x07 \x01(\x0b\x32\x13.bosdyn.api.SE2Pose\x12X\n\x12\x62ody_assist_params\x18\x05 \x01(\x0b\x32<.bosdyn.api.spot.BodyControlParams.BodyAssistForManipulation\x12\x1b\n\x13\x66orce_stow_override\x18\x06 \x01(\x08\x1a\x46\n\x13GripperCameraParams\x12/\n\x06params\x18\x01 \x01(\x0b\x32\x1f.bosdyn.api.GripperCameraParams\x1a\x45\n\x0eGripperCommand\x12\x33\n\x07request\x18\x01 \x01(\x0b\x32\".bosdyn.api.GripperCommand.Request\"\xb3\x05\n\x0f\x46\x61ilureBehavior\x12\x13\n\x0bretry_count\x18\x01 \x01(\x05\x12\x32\n\x0fprompt_duration\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration\x12K\n\x0esafe_power_off\x18\x03 \x01(\x0b\x32\x31.bosdyn.api.autowalk.FailureBehavior.SafePowerOffH\x00\x12M\n\x0fproceed_if_able\x18\x04 \x01(\x0b\x32\x32.bosdyn.api.autowalk.FailureBehavior.ProceedIfAbleH\x00\x12q\n#return_to_start_and_try_again_later\x18\x05 \x01(\x0b\x32\x42.bosdyn.api.autowalk.FailureBehavior.ReturnToStartAndTryAgainLaterH\x00\x12g\n\x1dreturn_to_start_and_terminate\x18\x06 \x01(\x0b\x32>.bosdyn.api.autowalk.FailureBehavior.ReturnToStartAndTerminateH\x00\x1aH\n\x0cSafePowerOff\x12\x38\n\x07request\x18\x01 \x01(\x0b\x32\'.bosdyn.api.SafePowerOffCommand.Request\x1a\x0f\n\rProceedIfAble\x1aS\n\x1dReturnToStartAndTryAgainLater\x12\x32\n\x0ftry_again_delay\x18\x01 \x01(\x0b\x32\x19.google.protobuf.Duration\x1a\x1b\n\x19ReturnToStartAndTerminateB\x12\n\x10\x64\x65\x66\x61ult_behavior\"Q\n\x0e\x42\x61tteryMonitor\x12\x1f\n\x17\x62\x61ttery_start_threshold\x18\x02 \x01(\x02\x12\x1e\n\x16\x62\x61ttery_stop_threshold\x18\x03 \x01(\x02\x42\x0c\x42\nWalksProtob\x06proto3')
 
 
 
 _WALK = DESCRIPTOR.message_types_by_name['Walk']
 _GLOBALPARAMETERS = DESCRIPTOR.message_types_by_name['GlobalParameters']
 _DOCK = DESCRIPTOR.message_types_by_name['Dock']
 _PLAYBACKMODE = DESCRIPTOR.message_types_by_name['PlaybackMode']
@@ -50,14 +52,16 @@
 _ACTION_REMOTEGRPC = _ACTION.nested_types_by_name['RemoteGrpc']
 _ACTIONWRAPPER = DESCRIPTOR.message_types_by_name['ActionWrapper']
 _ACTIONWRAPPER_ROBOTBODYSIT = _ACTIONWRAPPER.nested_types_by_name['RobotBodySit']
 _ACTIONWRAPPER_ROBOTBODYPOSE = _ACTIONWRAPPER.nested_types_by_name['RobotBodyPose']
 _ACTIONWRAPPER_SPOTCAMLED = _ACTIONWRAPPER.nested_types_by_name['SpotCamLed']
 _ACTIONWRAPPER_SPOTCAMLED_BRIGHTNESSESENTRY = _ACTIONWRAPPER_SPOTCAMLED.nested_types_by_name['BrightnessesEntry']
 _ACTIONWRAPPER_SPOTCAMPTZ = _ACTIONWRAPPER.nested_types_by_name['SpotCamPtz']
+_ACTIONWRAPPER_SPOTCAMALIGNMENT = _ACTIONWRAPPER.nested_types_by_name['SpotCamAlignment']
+_ACTIONWRAPPER_SPOTCAMALIGNMENT_ALIGNMENT = _ACTIONWRAPPER_SPOTCAMALIGNMENT.nested_types_by_name['Alignment']
 _ACTIONWRAPPER_ARMSENSORPOINTING = _ACTIONWRAPPER.nested_types_by_name['ArmSensorPointing']
 _ACTIONWRAPPER_GRIPPERCAMERAPARAMS = _ACTIONWRAPPER.nested_types_by_name['GripperCameraParams']
 _ACTIONWRAPPER_GRIPPERCOMMAND = _ACTIONWRAPPER.nested_types_by_name['GripperCommand']
 _FAILUREBEHAVIOR = DESCRIPTOR.message_types_by_name['FailureBehavior']
 _FAILUREBEHAVIOR_SAFEPOWEROFF = _FAILUREBEHAVIOR.nested_types_by_name['SafePowerOff']
 _FAILUREBEHAVIOR_PROCEEDIFABLE = _FAILUREBEHAVIOR.nested_types_by_name['ProceedIfAble']
 _FAILUREBEHAVIOR_RETURNTOSTARTANDTRYAGAINLATER = _FAILUREBEHAVIOR.nested_types_by_name['ReturnToStartAndTryAgainLater']
@@ -217,14 +221,28 @@
   'SpotCamPtz' : _reflection.GeneratedProtocolMessageType('SpotCamPtz', (_message.Message,), {
     'DESCRIPTOR' : _ACTIONWRAPPER_SPOTCAMPTZ,
     '__module__' : 'bosdyn.api.autowalk.walks_pb2'
     # @@protoc_insertion_point(class_scope:bosdyn.api.autowalk.ActionWrapper.SpotCamPtz)
     })
   ,
 
+  'SpotCamAlignment' : _reflection.GeneratedProtocolMessageType('SpotCamAlignment', (_message.Message,), {
+
+    'Alignment' : _reflection.GeneratedProtocolMessageType('Alignment', (_message.Message,), {
+      'DESCRIPTOR' : _ACTIONWRAPPER_SPOTCAMALIGNMENT_ALIGNMENT,
+      '__module__' : 'bosdyn.api.autowalk.walks_pb2'
+      # @@protoc_insertion_point(class_scope:bosdyn.api.autowalk.ActionWrapper.SpotCamAlignment.Alignment)
+      })
+    ,
+    'DESCRIPTOR' : _ACTIONWRAPPER_SPOTCAMALIGNMENT,
+    '__module__' : 'bosdyn.api.autowalk.walks_pb2'
+    # @@protoc_insertion_point(class_scope:bosdyn.api.autowalk.ActionWrapper.SpotCamAlignment)
+    })
+  ,
+
   'ArmSensorPointing' : _reflection.GeneratedProtocolMessageType('ArmSensorPointing', (_message.Message,), {
     'DESCRIPTOR' : _ACTIONWRAPPER_ARMSENSORPOINTING,
     '__module__' : 'bosdyn.api.autowalk.walks_pb2'
     # @@protoc_insertion_point(class_scope:bosdyn.api.autowalk.ActionWrapper.ArmSensorPointing)
     })
   ,
 
@@ -247,14 +265,16 @@
   })
 _sym_db.RegisterMessage(ActionWrapper)
 _sym_db.RegisterMessage(ActionWrapper.RobotBodySit)
 _sym_db.RegisterMessage(ActionWrapper.RobotBodyPose)
 _sym_db.RegisterMessage(ActionWrapper.SpotCamLed)
 _sym_db.RegisterMessage(ActionWrapper.SpotCamLed.BrightnessesEntry)
 _sym_db.RegisterMessage(ActionWrapper.SpotCamPtz)
+_sym_db.RegisterMessage(ActionWrapper.SpotCamAlignment)
+_sym_db.RegisterMessage(ActionWrapper.SpotCamAlignment.Alignment)
 _sym_db.RegisterMessage(ActionWrapper.ArmSensorPointing)
 _sym_db.RegisterMessage(ActionWrapper.GripperCameraParams)
 _sym_db.RegisterMessage(ActionWrapper.GripperCommand)
 
 FailureBehavior = _reflection.GeneratedProtocolMessageType('FailureBehavior', (_message.Message,), {
 
   'SafePowerOff' : _reflection.GeneratedProtocolMessageType('SafePowerOff', (_message.Message,), {
@@ -301,72 +321,78 @@
   })
 _sym_db.RegisterMessage(BatteryMonitor)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'B\nWalksProto'
+  _ACTION_REMOTEGRPC.fields_by_name['inputs']._options = None
+  _ACTION_REMOTEGRPC.fields_by_name['inputs']._serialized_options = b'\030\001'
   _ACTIONWRAPPER_SPOTCAMLED_BRIGHTNESSESENTRY._options = None
   _ACTIONWRAPPER_SPOTCAMLED_BRIGHTNESSESENTRY._serialized_options = b'8\001'
-  _WALK._serialized_start=516
-  _WALK._serialized_end=782
-  _GLOBALPARAMETERS._serialized_start=785
-  _GLOBALPARAMETERS._serialized_end=976
-  _DOCK._serialized_start=979
-  _DOCK._serialized_end=1137
-  _PLAYBACKMODE._serialized_start=1140
-  _PLAYBACKMODE._serialized_end=1489
-  _PLAYBACKMODE_ONCE._serialized_start=1344
-  _PLAYBACKMODE_ONCE._serialized_end=1389
-  _PLAYBACKMODE_PERIODIC._serialized_start=1391
-  _PLAYBACKMODE_PERIODIC._serialized_end=1467
-  _PLAYBACKMODE_CONTINUOUS._serialized_start=1469
-  _PLAYBACKMODE_CONTINUOUS._serialized_end=1481
-  _ELEMENT._serialized_start=1492
-  _ELEMENT._serialized_end=1941
-  _TARGET._serialized_start=1944
-  _TARGET._serialized_end=2474
-  _TARGET_RELOCALIZE._serialized_start=2146
-  _TARGET_RELOCALIZE._serialized_end=2238
-  _TARGET_NAVIGATETO._serialized_start=2240
-  _TARGET_NAVIGATETO._serialized_end=2344
-  _TARGET_NAVIGATEROUTE._serialized_start=2346
-  _TARGET_NAVIGATEROUTE._serialized_end=2464
-  _ACTION._serialized_start=2477
-  _ACTION._serialized_end=3102
-  _ACTION_SLEEP._serialized_start=2717
-  _ACTION_SLEEP._serialized_end=2769
-  _ACTION_DATAACQUISITION._serialized_start=2772
-  _ACTION_DATAACQUISITION._serialized_end=2936
-  _ACTION_REMOTEGRPC._serialized_start=2939
-  _ACTION_REMOTEGRPC._serialized_end=3092
-  _ACTIONWRAPPER._serialized_start=3105
-  _ACTIONWRAPPER._serialized_end=4468
-  _ACTIONWRAPPER_ROBOTBODYSIT._serialized_start=3654
-  _ACTIONWRAPPER_ROBOTBODYSIT._serialized_end=3668
-  _ACTIONWRAPPER_ROBOTBODYPOSE._serialized_start=3670
-  _ACTIONWRAPPER_ROBOTBODYPOSE._serialized_end=3733
-  _ACTIONWRAPPER_SPOTCAMLED._serialized_start=3736
-  _ACTIONWRAPPER_SPOTCAMLED._serialized_end=3888
-  _ACTIONWRAPPER_SPOTCAMLED_BRIGHTNESSESENTRY._serialized_start=3837
-  _ACTIONWRAPPER_SPOTCAMLED_BRIGHTNESSESENTRY._serialized_end=3888
-  _ACTIONWRAPPER_SPOTCAMPTZ._serialized_start=3890
-  _ACTIONWRAPPER_SPOTCAMPTZ._serialized_end=3958
-  _ACTIONWRAPPER_ARMSENSORPOINTING._serialized_start=3961
-  _ACTIONWRAPPER_ARMSENSORPOINTING._serialized_end=4325
-  _ACTIONWRAPPER_GRIPPERCAMERAPARAMS._serialized_start=4327
-  _ACTIONWRAPPER_GRIPPERCAMERAPARAMS._serialized_end=4397
-  _ACTIONWRAPPER_GRIPPERCOMMAND._serialized_start=4399
-  _ACTIONWRAPPER_GRIPPERCOMMAND._serialized_end=4468
-  _FAILUREBEHAVIOR._serialized_start=4471
-  _FAILUREBEHAVIOR._serialized_end=5162
-  _FAILUREBEHAVIOR_SAFEPOWEROFF._serialized_start=4939
-  _FAILUREBEHAVIOR_SAFEPOWEROFF._serialized_end=5011
-  _FAILUREBEHAVIOR_PROCEEDIFABLE._serialized_start=5013
-  _FAILUREBEHAVIOR_PROCEEDIFABLE._serialized_end=5028
-  _FAILUREBEHAVIOR_RETURNTOSTARTANDTRYAGAINLATER._serialized_start=5030
-  _FAILUREBEHAVIOR_RETURNTOSTARTANDTRYAGAINLATER._serialized_end=5113
-  _FAILUREBEHAVIOR_RETURNTOSTARTANDTERMINATE._serialized_start=5115
-  _FAILUREBEHAVIOR_RETURNTOSTARTANDTERMINATE._serialized_end=5142
-  _BATTERYMONITOR._serialized_start=5164
-  _BATTERYMONITOR._serialized_end=5245
+  _WALK._serialized_start=580
+  _WALK._serialized_end=858
+  _GLOBALPARAMETERS._serialized_start=861
+  _GLOBALPARAMETERS._serialized_end=1052
+  _DOCK._serialized_start=1055
+  _DOCK._serialized_end=1213
+  _PLAYBACKMODE._serialized_start=1216
+  _PLAYBACKMODE._serialized_end=1565
+  _PLAYBACKMODE_ONCE._serialized_start=1420
+  _PLAYBACKMODE_ONCE._serialized_end=1465
+  _PLAYBACKMODE_PERIODIC._serialized_start=1467
+  _PLAYBACKMODE_PERIODIC._serialized_end=1543
+  _PLAYBACKMODE_CONTINUOUS._serialized_start=1545
+  _PLAYBACKMODE_CONTINUOUS._serialized_end=1557
+  _ELEMENT._serialized_start=1568
+  _ELEMENT._serialized_end=2029
+  _TARGET._serialized_start=2032
+  _TARGET._serialized_end=2562
+  _TARGET_RELOCALIZE._serialized_start=2234
+  _TARGET_RELOCALIZE._serialized_end=2326
+  _TARGET_NAVIGATETO._serialized_start=2328
+  _TARGET_NAVIGATETO._serialized_end=2432
+  _TARGET_NAVIGATEROUTE._serialized_start=2434
+  _TARGET_NAVIGATEROUTE._serialized_end=2552
+  _ACTION._serialized_start=2565
+  _ACTION._serialized_end=3447
+  _ACTION_SLEEP._serialized_start=2805
+  _ACTION_SLEEP._serialized_end=2857
+  _ACTION_DATAACQUISITION._serialized_start=2860
+  _ACTION_DATAACQUISITION._serialized_end=3159
+  _ACTION_REMOTEGRPC._serialized_start=3162
+  _ACTION_REMOTEGRPC._serialized_end=3437
+  _ACTIONWRAPPER._serialized_start=3450
+  _ACTIONWRAPPER._serialized_end=5201
+  _ACTIONWRAPPER_ROBOTBODYSIT._serialized_start=4080
+  _ACTIONWRAPPER_ROBOTBODYSIT._serialized_end=4094
+  _ACTIONWRAPPER_ROBOTBODYPOSE._serialized_start=4096
+  _ACTIONWRAPPER_ROBOTBODYPOSE._serialized_end=4159
+  _ACTIONWRAPPER_SPOTCAMLED._serialized_start=4162
+  _ACTIONWRAPPER_SPOTCAMLED._serialized_end=4314
+  _ACTIONWRAPPER_SPOTCAMLED_BRIGHTNESSESENTRY._serialized_start=4263
+  _ACTIONWRAPPER_SPOTCAMLED_BRIGHTNESSESENTRY._serialized_end=4314
+  _ACTIONWRAPPER_SPOTCAMPTZ._serialized_start=4316
+  _ACTIONWRAPPER_SPOTCAMPTZ._serialized_end=4384
+  _ACTIONWRAPPER_SPOTCAMALIGNMENT._serialized_start=4387
+  _ACTIONWRAPPER_SPOTCAMALIGNMENT._serialized_end=4691
+  _ACTIONWRAPPER_SPOTCAMALIGNMENT_ALIGNMENT._serialized_start=4587
+  _ACTIONWRAPPER_SPOTCAMALIGNMENT_ALIGNMENT._serialized_end=4691
+  _ACTIONWRAPPER_ARMSENSORPOINTING._serialized_start=4694
+  _ACTIONWRAPPER_ARMSENSORPOINTING._serialized_end=5058
+  _ACTIONWRAPPER_GRIPPERCAMERAPARAMS._serialized_start=5060
+  _ACTIONWRAPPER_GRIPPERCAMERAPARAMS._serialized_end=5130
+  _ACTIONWRAPPER_GRIPPERCOMMAND._serialized_start=5132
+  _ACTIONWRAPPER_GRIPPERCOMMAND._serialized_end=5201
+  _FAILUREBEHAVIOR._serialized_start=5204
+  _FAILUREBEHAVIOR._serialized_end=5895
+  _FAILUREBEHAVIOR_SAFEPOWEROFF._serialized_start=5672
+  _FAILUREBEHAVIOR_SAFEPOWEROFF._serialized_end=5744
+  _FAILUREBEHAVIOR_PROCEEDIFABLE._serialized_start=5746
+  _FAILUREBEHAVIOR_PROCEEDIFABLE._serialized_end=5761
+  _FAILUREBEHAVIOR_RETURNTOSTARTANDTRYAGAINLATER._serialized_start=5763
+  _FAILUREBEHAVIOR_RETURNTOSTARTANDTRYAGAINLATER._serialized_end=5846
+  _FAILUREBEHAVIOR_RETURNTOSTARTANDTERMINATE._serialized_start=5848
+  _FAILUREBEHAVIOR_RETURNTOSTARTANDTERMINATE._serialized_end=5875
+  _BATTERYMONITOR._serialized_start=5897
+  _BATTERYMONITOR._serialized_end=5978
 # @@protoc_insertion_point(module_scope)
```

## bosdyn/api/docking/__init__.py

```diff
@@ -0,0 +1,4 @@
+00000000: 5f5f 7061 7468 5f5f 203d 205f 5f69 6d70  __path__ = __imp
+00000010: 6f72 745f 5f28 2770 6b67 7574 696c 2729  ort__('pkgutil')
+00000020: 2e65 7874 656e 645f 7061 7468 285f 5f70  .extend_path(__p
+00000030: 6174 685f 5f2c 205f 5f6e 616d 655f 5f29  ath__, __name__)
```

## bosdyn/api/docking/docking_pb2.py

```diff
@@ -14,23 +14,24 @@
 
 
 from bosdyn.api import header_pb2 as bosdyn_dot_api_dot_header__pb2
 from bosdyn.api import lease_pb2 as bosdyn_dot_api_dot_lease__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n bosdyn/api/docking/docking.proto\x12\x12\x62osdyn.api.docking\x1a\x17\x62osdyn/api/header.proto\x1a\x16\x62osdyn/api/lease.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\x8a\x02\n\x15\x44ockingCommandRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12 \n\x05lease\x18\x02 \x01(\x0b\x32\x11.bosdyn.api.Lease\x12\x1a\n\x12\x64ocking_station_id\x18\x03 \x01(\r\x12\x18\n\x10\x63lock_identifier\x18\x04 \x01(\t\x12,\n\x08\x65nd_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12@\n\x12prep_pose_behavior\x18\t \x01(\x0e\x32$.bosdyn.api.docking.PrepPoseBehavior\"\xbd\x03\n\x16\x44ockingCommandResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x34\n\x10lease_use_result\x18\x02 \x01(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12\x41\n\x06status\x18\x03 \x01(\x0e\x32\x31.bosdyn.api.docking.DockingCommandResponse.Status\x12\x1a\n\x12\x64ocking_command_id\x18\x05 \x01(\r\"\xe1\x01\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x16\n\x12STATUS_ERROR_LEASE\x10\x04\x12\x1f\n\x1bSTATUS_ERROR_DOCK_NOT_FOUND\x10\x05\x12\x1b\n\x17STATUS_ERROR_NOT_DOCKED\x10\x06\x12%\n!STATUS_ERROR_GRIPPER_HOLDING_ITEM\x10\x08\x12\x1e\n\x1aSTATUS_ERROR_NOT_AVAILABLE\x10\t\x12\x17\n\x13STATUS_ERROR_SYSTEM\x10\x07\"C\n\x13UpdateDockingParams\x12,\n\x08\x65nd_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xae\x01\n\x1d\x44ockingCommandFeedbackRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x1a\n\x12\x64ocking_command_id\x18\x02 \x01(\r\x12\x46\n\x15update_docking_params\x18\x03 \x01(\x0b\x32\'.bosdyn.api.docking.UpdateDockingParams\"\xee\x04\n\x1e\x44ockingCommandFeedbackResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x34\n\x10lease_use_result\x18\x02 \x01(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12I\n\x06status\x18\x03 \x01(\x0e\x32\x39.bosdyn.api.docking.DockingCommandFeedbackResponse.Status\"\x9e\x03\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x16\n\x12STATUS_IN_PROGRESS\x10\x01\x12\x11\n\rSTATUS_DOCKED\x10\x02\x12\x17\n\x13STATUS_AT_PREP_POSE\x10\x0b\x12\x15\n\x11STATUS_MISALIGNED\x10\n\x12\x1e\n\x1aSTATUS_OLD_DOCKING_COMMAND\x10\x03\x12\x1a\n\x16STATUS_ERROR_DOCK_LOST\x10\x04\x12\x16\n\x12STATUS_ERROR_LEASE\x10\x05\x12\"\n\x1eSTATUS_ERROR_COMMAND_TIMED_OUT\x10\x06\x12\x1c\n\x18STATUS_ERROR_NO_TIMESYNC\x10\x07\x12\x1c\n\x18STATUS_ERROR_TOO_DISTANT\x10\x08\x12\x1e\n\x1aSTATUS_ERROR_NOT_AVAILABLE\x10\x0c\x12 \n\x1cSTATUS_ERROR_UNREFINED_PRIOR\x10\r\x12\x16\n\x12STATUS_ERROR_STUCK\x10\x0e\x12\x17\n\x13STATUS_ERROR_SYSTEM\x10\t\"[\n\x0b\x43onfigRange\x12\x10\n\x08id_start\x18\x01 \x01(\r\x12\x0e\n\x06id_end\x18\x02 \x01(\r\x12*\n\x04type\x18\x03 \x01(\x0e\x32\x1c.bosdyn.api.docking.DockType\"D\n\x17GetDockingConfigRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"}\n\x18GetDockingConfigResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x35\n\x0c\x64ock_configs\x18\x02 \x03(\x0b\x32\x1f.bosdyn.api.docking.ConfigRange\"\xcd\x03\n\tDockState\x12:\n\x06status\x18\x01 \x01(\x0e\x32*.bosdyn.api.docking.DockState.DockedStatus\x12/\n\tdock_type\x18\x02 \x01(\x0e\x32\x1c.bosdyn.api.docking.DockType\x12\x0f\n\x07\x64ock_id\x18\x03 \x01(\r\x12>\n\x0cpower_status\x18\x04 \x01(\x0e\x32(.bosdyn.api.docking.DockState.LinkStatus\"\x8d\x01\n\x0c\x44ockedStatus\x12\x17\n\x13\x44OCK_STATUS_UNKNOWN\x10\x00\x12\x16\n\x12\x44OCK_STATUS_DOCKED\x10\x01\x12\x17\n\x13\x44OCK_STATUS_DOCKING\x10\x02\x12\x18\n\x14\x44OCK_STATUS_UNDOCKED\x10\x03\x12\x19\n\x15\x44OCK_STATUS_UNDOCKING\x10\x04\"r\n\nLinkStatus\x12\x17\n\x13LINK_STATUS_UNKNOWN\x10\x00\x12\x19\n\x15LINK_STATUS_DETECTING\x10\x03\x12\x19\n\x15LINK_STATUS_CONNECTED\x10\x01\x12\x15\n\x11LINK_STATUS_ERROR\x10\x02\"C\n\x16GetDockingStateRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"x\n\x17GetDockingStateResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x31\n\ndock_state\x18\x02 \x01(\x0b\x32\x1d.bosdyn.api.docking.DockState*[\n\x08\x44ockType\x12\x15\n\x11\x44OCK_TYPE_UNKNOWN\x10\x00\x12\x1f\n\x1b\x44OCK_TYPE_CONTACT_PROTOTYPE\x10\x02\x12\x17\n\x13\x44OCK_TYPE_SPOT_DOCK\x10\x03*\x89\x01\n\x10PrepPoseBehavior\x12\x15\n\x11PREP_POSE_UNKNOWN\x10\x00\x12\x16\n\x12PREP_POSE_USE_POSE\x10\x01\x12\x17\n\x13PREP_POSE_SKIP_POSE\x10\x02\x12\x17\n\x13PREP_POSE_ONLY_POSE\x10\x03\x12\x14\n\x10PREP_POSE_UNDOCK\x10\x04\x42\x0e\x42\x0c\x44ockingProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n bosdyn/api/docking/docking.proto\x12\x12\x62osdyn.api.docking\x1a\x17\x62osdyn/api/header.proto\x1a\x16\x62osdyn/api/lease.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\xa4\x02\n\x15\x44ockingCommandRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12 \n\x05lease\x18\x02 \x01(\x0b\x32\x11.bosdyn.api.Lease\x12\x1a\n\x12\x64ocking_station_id\x18\x03 \x01(\r\x12\x18\n\x10\x63lock_identifier\x18\x04 \x01(\t\x12,\n\x08\x65nd_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12@\n\x12prep_pose_behavior\x18\t \x01(\x0e\x32$.bosdyn.api.docking.PrepPoseBehavior\x12\x18\n\x10require_fiducial\x18\n \x01(\x08\"\xbd\x03\n\x16\x44ockingCommandResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x34\n\x10lease_use_result\x18\x02 \x01(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12\x41\n\x06status\x18\x03 \x01(\x0e\x32\x31.bosdyn.api.docking.DockingCommandResponse.Status\x12\x1a\n\x12\x64ocking_command_id\x18\x05 \x01(\r\"\xe1\x01\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x16\n\x12STATUS_ERROR_LEASE\x10\x04\x12\x1f\n\x1bSTATUS_ERROR_DOCK_NOT_FOUND\x10\x05\x12\x1b\n\x17STATUS_ERROR_NOT_DOCKED\x10\x06\x12%\n!STATUS_ERROR_GRIPPER_HOLDING_ITEM\x10\x08\x12\x1e\n\x1aSTATUS_ERROR_NOT_AVAILABLE\x10\t\x12\x17\n\x13STATUS_ERROR_SYSTEM\x10\x07\"C\n\x13UpdateDockingParams\x12,\n\x08\x65nd_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xae\x01\n\x1d\x44ockingCommandFeedbackRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x1a\n\x12\x64ocking_command_id\x18\x02 \x01(\r\x12\x46\n\x15update_docking_params\x18\x03 \x01(\x0b\x32\'.bosdyn.api.docking.UpdateDockingParams\"\xee\x04\n\x1e\x44ockingCommandFeedbackResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x34\n\x10lease_use_result\x18\x02 \x01(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12I\n\x06status\x18\x03 \x01(\x0e\x32\x39.bosdyn.api.docking.DockingCommandFeedbackResponse.Status\"\x9e\x03\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x16\n\x12STATUS_IN_PROGRESS\x10\x01\x12\x11\n\rSTATUS_DOCKED\x10\x02\x12\x17\n\x13STATUS_AT_PREP_POSE\x10\x0b\x12\x15\n\x11STATUS_MISALIGNED\x10\n\x12\x1e\n\x1aSTATUS_OLD_DOCKING_COMMAND\x10\x03\x12\x1a\n\x16STATUS_ERROR_DOCK_LOST\x10\x04\x12\x16\n\x12STATUS_ERROR_LEASE\x10\x05\x12\"\n\x1eSTATUS_ERROR_COMMAND_TIMED_OUT\x10\x06\x12\x1c\n\x18STATUS_ERROR_NO_TIMESYNC\x10\x07\x12\x1c\n\x18STATUS_ERROR_TOO_DISTANT\x10\x08\x12\x1e\n\x1aSTATUS_ERROR_NOT_AVAILABLE\x10\x0c\x12 \n\x1cSTATUS_ERROR_UNREFINED_PRIOR\x10\r\x12\x16\n\x12STATUS_ERROR_STUCK\x10\x0e\x12\x17\n\x13STATUS_ERROR_SYSTEM\x10\t\"[\n\x0b\x43onfigRange\x12\x10\n\x08id_start\x18\x01 \x01(\r\x12\x0e\n\x06id_end\x18\x02 \x01(\r\x12*\n\x04type\x18\x03 \x01(\x0e\x32\x1c.bosdyn.api.docking.DockType\"D\n\x17GetDockingConfigRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"}\n\x18GetDockingConfigResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x35\n\x0c\x64ock_configs\x18\x02 \x03(\x0b\x32\x1f.bosdyn.api.docking.ConfigRange\"\xcd\x03\n\tDockState\x12:\n\x06status\x18\x01 \x01(\x0e\x32*.bosdyn.api.docking.DockState.DockedStatus\x12/\n\tdock_type\x18\x02 \x01(\x0e\x32\x1c.bosdyn.api.docking.DockType\x12\x0f\n\x07\x64ock_id\x18\x03 \x01(\r\x12>\n\x0cpower_status\x18\x04 \x01(\x0e\x32(.bosdyn.api.docking.DockState.LinkStatus\"\x8d\x01\n\x0c\x44ockedStatus\x12\x17\n\x13\x44OCK_STATUS_UNKNOWN\x10\x00\x12\x16\n\x12\x44OCK_STATUS_DOCKED\x10\x01\x12\x17\n\x13\x44OCK_STATUS_DOCKING\x10\x02\x12\x18\n\x14\x44OCK_STATUS_UNDOCKED\x10\x03\x12\x19\n\x15\x44OCK_STATUS_UNDOCKING\x10\x04\"r\n\nLinkStatus\x12\x17\n\x13LINK_STATUS_UNKNOWN\x10\x00\x12\x19\n\x15LINK_STATUS_DETECTING\x10\x03\x12\x19\n\x15LINK_STATUS_CONNECTED\x10\x01\x12\x15\n\x11LINK_STATUS_ERROR\x10\x02\"C\n\x16GetDockingStateRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"x\n\x17GetDockingStateResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x31\n\ndock_state\x18\x02 \x01(\x0b\x32\x1d.bosdyn.api.docking.DockState*x\n\x08\x44ockType\x12\x15\n\x11\x44OCK_TYPE_UNKNOWN\x10\x00\x12\x1f\n\x1b\x44OCK_TYPE_CONTACT_PROTOTYPE\x10\x02\x12\x17\n\x13\x44OCK_TYPE_SPOT_DOCK\x10\x03\x12\x1b\n\x17\x44OCK_TYPE_SPOT_DOGHOUSE\x10\x04*\x89\x01\n\x10PrepPoseBehavior\x12\x15\n\x11PREP_POSE_UNKNOWN\x10\x00\x12\x16\n\x12PREP_POSE_USE_POSE\x10\x01\x12\x17\n\x13PREP_POSE_SKIP_POSE\x10\x02\x12\x17\n\x13PREP_POSE_ONLY_POSE\x10\x03\x12\x14\n\x10PREP_POSE_UNDOCK\x10\x04\x42\x0e\x42\x0c\x44ockingProtob\x06proto3')
 
 _DOCKTYPE = DESCRIPTOR.enum_types_by_name['DockType']
 DockType = enum_type_wrapper.EnumTypeWrapper(_DOCKTYPE)
 _PREPPOSEBEHAVIOR = DESCRIPTOR.enum_types_by_name['PrepPoseBehavior']
 PrepPoseBehavior = enum_type_wrapper.EnumTypeWrapper(_PREPPOSEBEHAVIOR)
 DOCK_TYPE_UNKNOWN = 0
 DOCK_TYPE_CONTACT_PROTOTYPE = 2
 DOCK_TYPE_SPOT_DOCK = 3
+DOCK_TYPE_SPOT_DOGHOUSE = 4
 PREP_POSE_UNKNOWN = 0
 PREP_POSE_USE_POSE = 1
 PREP_POSE_SKIP_POSE = 2
 PREP_POSE_ONLY_POSE = 3
 PREP_POSE_UNDOCK = 4
 
 
@@ -126,42 +127,42 @@
   })
 _sym_db.RegisterMessage(GetDockingStateResponse)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'B\014DockingProto'
-  _DOCKTYPE._serialized_start=2671
-  _DOCKTYPE._serialized_end=2762
-  _PREPPOSEBEHAVIOR._serialized_start=2765
-  _PREPPOSEBEHAVIOR._serialized_end=2902
+  _DOCKTYPE._serialized_start=2697
+  _DOCKTYPE._serialized_end=2817
+  _PREPPOSEBEHAVIOR._serialized_start=2820
+  _PREPPOSEBEHAVIOR._serialized_end=2957
   _DOCKINGCOMMANDREQUEST._serialized_start=139
-  _DOCKINGCOMMANDREQUEST._serialized_end=405
-  _DOCKINGCOMMANDRESPONSE._serialized_start=408
-  _DOCKINGCOMMANDRESPONSE._serialized_end=853
-  _DOCKINGCOMMANDRESPONSE_STATUS._serialized_start=628
-  _DOCKINGCOMMANDRESPONSE_STATUS._serialized_end=853
-  _UPDATEDOCKINGPARAMS._serialized_start=855
-  _UPDATEDOCKINGPARAMS._serialized_end=922
-  _DOCKINGCOMMANDFEEDBACKREQUEST._serialized_start=925
-  _DOCKINGCOMMANDFEEDBACKREQUEST._serialized_end=1099
-  _DOCKINGCOMMANDFEEDBACKRESPONSE._serialized_start=1102
-  _DOCKINGCOMMANDFEEDBACKRESPONSE._serialized_end=1724
-  _DOCKINGCOMMANDFEEDBACKRESPONSE_STATUS._serialized_start=1310
-  _DOCKINGCOMMANDFEEDBACKRESPONSE_STATUS._serialized_end=1724
-  _CONFIGRANGE._serialized_start=1726
-  _CONFIGRANGE._serialized_end=1817
-  _GETDOCKINGCONFIGREQUEST._serialized_start=1819
-  _GETDOCKINGCONFIGREQUEST._serialized_end=1887
-  _GETDOCKINGCONFIGRESPONSE._serialized_start=1889
-  _GETDOCKINGCONFIGRESPONSE._serialized_end=2014
-  _DOCKSTATE._serialized_start=2017
-  _DOCKSTATE._serialized_end=2478
-  _DOCKSTATE_DOCKEDSTATUS._serialized_start=2221
-  _DOCKSTATE_DOCKEDSTATUS._serialized_end=2362
-  _DOCKSTATE_LINKSTATUS._serialized_start=2364
-  _DOCKSTATE_LINKSTATUS._serialized_end=2478
-  _GETDOCKINGSTATEREQUEST._serialized_start=2480
-  _GETDOCKINGSTATEREQUEST._serialized_end=2547
-  _GETDOCKINGSTATERESPONSE._serialized_start=2549
-  _GETDOCKINGSTATERESPONSE._serialized_end=2669
+  _DOCKINGCOMMANDREQUEST._serialized_end=431
+  _DOCKINGCOMMANDRESPONSE._serialized_start=434
+  _DOCKINGCOMMANDRESPONSE._serialized_end=879
+  _DOCKINGCOMMANDRESPONSE_STATUS._serialized_start=654
+  _DOCKINGCOMMANDRESPONSE_STATUS._serialized_end=879
+  _UPDATEDOCKINGPARAMS._serialized_start=881
+  _UPDATEDOCKINGPARAMS._serialized_end=948
+  _DOCKINGCOMMANDFEEDBACKREQUEST._serialized_start=951
+  _DOCKINGCOMMANDFEEDBACKREQUEST._serialized_end=1125
+  _DOCKINGCOMMANDFEEDBACKRESPONSE._serialized_start=1128
+  _DOCKINGCOMMANDFEEDBACKRESPONSE._serialized_end=1750
+  _DOCKINGCOMMANDFEEDBACKRESPONSE_STATUS._serialized_start=1336
+  _DOCKINGCOMMANDFEEDBACKRESPONSE_STATUS._serialized_end=1750
+  _CONFIGRANGE._serialized_start=1752
+  _CONFIGRANGE._serialized_end=1843
+  _GETDOCKINGCONFIGREQUEST._serialized_start=1845
+  _GETDOCKINGCONFIGREQUEST._serialized_end=1913
+  _GETDOCKINGCONFIGRESPONSE._serialized_start=1915
+  _GETDOCKINGCONFIGRESPONSE._serialized_end=2040
+  _DOCKSTATE._serialized_start=2043
+  _DOCKSTATE._serialized_end=2504
+  _DOCKSTATE_DOCKEDSTATUS._serialized_start=2247
+  _DOCKSTATE_DOCKEDSTATUS._serialized_end=2388
+  _DOCKSTATE_LINKSTATUS._serialized_start=2390
+  _DOCKSTATE_LINKSTATUS._serialized_end=2504
+  _GETDOCKINGSTATEREQUEST._serialized_start=2506
+  _GETDOCKINGSTATEREQUEST._serialized_end=2573
+  _GETDOCKINGSTATERESPONSE._serialized_start=2575
+  _GETDOCKINGSTATERESPONSE._serialized_end=2695
 # @@protoc_insertion_point(module_scope)
```

## bosdyn/api/graph_nav/__init__.py

```diff
@@ -0,0 +1,4 @@
+00000000: 5f5f 7061 7468 5f5f 203d 205f 5f69 6d70  __path__ = __imp
+00000010: 6f72 745f 5f28 2770 6b67 7574 696c 2729  ort__('pkgutil')
+00000020: 2e65 7874 656e 645f 7061 7468 285f 5f70  .extend_path(__p
+00000030: 6174 685f 5f2c 205f 5f6e 616d 655f 5f29  ath__, __name__)
```

## bosdyn/api/graph_nav/area_callback_pb2.py

```diff
@@ -11,41 +11,45 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from bosdyn.api import header_pb2 as bosdyn_dot_api_dot_header__pb2
 from bosdyn.api import lease_pb2 as bosdyn_dot_api_dot_lease__pb2
+from bosdyn.api import service_customization_pb2 as bosdyn_dot_api_dot_service__customization__pb2
+from bosdyn.api.graph_nav import area_callback_data_pb2 as bosdyn_dot_api_dot_graph__nav_dot_area__callback__data__pb2
 from bosdyn.api.graph_nav import nav_pb2 as bosdyn_dot_api_dot_graph__nav_dot_nav__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(bosdyn/api/graph_nav/area_callback.proto\x12\x14\x62osdyn.api.graph_nav\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x17\x62osdyn/api/header.proto\x1a\x16\x62osdyn/api/lease.proto\x1a\x1e\x62osdyn/api/graph_nav/nav.proto\"\xf1\x03\n\x11\x41reaCallbackError\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12@\n\x05\x65rror\x18\x02 \x01(\x0e\x32\x31.bosdyn.api.graph_nav.AreaCallbackError.CallError\x12\x45\n\x0e\x62\x65gin_callback\x18\x03 \x01(\x0b\x32+.bosdyn.api.graph_nav.BeginCallbackResponseH\x00\x12\x43\n\rbegin_control\x18\x04 \x01(\x0b\x32*.bosdyn.api.graph_nav.BeginControlResponseH\x00\x12G\n\x0fupdate_callback\x18\x05 \x01(\x0b\x32,.bosdyn.api.graph_nav.UpdateCallbackResponseH\x00\x12\x41\n\x0c\x65nd_callback\x18\x06 \x01(\x0b\x32).bosdyn.api.graph_nav.EndCallbackResponseH\x00\"Z\n\tCallError\x12\x11\n\rERROR_UNKNOWN\x10\x00\x12\x13\n\x0f\x45RROR_TRANSPORT\x10\x01\x12\x12\n\x0e\x45RROR_RESPONSE\x10\x02\x12\x11\n\rERROR_SERVICE\x10\x03\x42\x10\n\x0eresponse_error\"K\n\x1e\x41reaCallbackInformationRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\";\n\x17\x41reaCallbackInformation\x12 \n\x18required_lease_resources\x18\x01 \x03(\t\"\x8a\x01\n\x1f\x41reaCallbackInformationResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12;\n\x04info\x18\x02 \x01(\x0b\x32-.bosdyn.api.graph_nav.AreaCallbackInformation\"g\n\x11RegionInformation\x12\x11\n\tregion_id\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12*\n\x05route\x18\x03 \x01(\x0b\x32\x1b.bosdyn.api.graph_nav.Route\"\xad\x01\n\x14\x42\x65ginCallbackRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12<\n\x0bregion_info\x18\x04 \x01(\x0b\x32\'.bosdyn.api.graph_nav.RegionInformation\x12,\n\x08\x65nd_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x87\x02\n\x15\x42\x65ginCallbackResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x42\n\x06status\x18\x02 \x01(\x0e\x32\x32.bosdyn.api.graph_nav.BeginCallbackResponse.Status\x12\x12\n\ncommand_id\x18\x03 \x01(\r\"j\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12 \n\x1cSTATUS_INVALID_CONFIGURATION\x10\x02\x12\x1b\n\x17STATUS_EXPIRED_END_TIME\x10\x03\"w\n\x13\x42\x65ginControlRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12!\n\x06leases\x18\x02 \x03(\x0b\x32\x11.bosdyn.api.Lease\x12\x12\n\ncommand_id\x18\x03 \x01(\r\"\xc5\x02\n\x14\x42\x65ginControlResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x35\n\x11lease_use_results\x18\x02 \x03(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12\x41\n\x06status\x18\x03 \x01(\x0e\x32\x31.bosdyn.api.graph_nav.BeginControlResponse.Status\"\x86\x01\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1d\n\x19STATUS_INVALID_COMMAND_ID\x10\x02\x12\"\n\x1eSTATUS_MISSING_LEASE_RESOURCES\x10\x03\x12\x16\n\x12STATUS_LEASE_ERROR\x10\x04\"\xae\x02\n\x15UpdateCallbackRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x12\n\ncommand_id\x18\x02 \x01(\r\x12,\n\x08\x65nd_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12@\n\x05stage\x18\x04 \x01(\x0e\x32\x31.bosdyn.api.graph_nav.UpdateCallbackRequest.Stage\"f\n\x05Stage\x12\x11\n\rSTAGE_UNKNOWN\x10\x00\x12\x12\n\x0eSTAGE_TO_START\x10\x01\x12\x12\n\x0eSTAGE_AT_START\x10\x02\x12\x10\n\x0cSTAGE_TO_END\x10\x03\x12\x10\n\x0cSTAGE_AT_END\x10\x04\"\xec\x07\n\x16UpdateCallbackResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x43\n\x06status\x18\x02 \x01(\x0e\x32\x33.bosdyn.api.graph_nav.UpdateCallbackResponse.Status\x12H\n\x06policy\x18\x03 \x01(\x0b\x32\x36.bosdyn.api.graph_nav.UpdateCallbackResponse.NavPolicyH\x00\x12\x43\n\x05\x65rror\x18\x04 \x01(\x0b\x32\x32.bosdyn.api.graph_nav.UpdateCallbackResponse.ErrorH\x00\x12I\n\x08\x63omplete\x18\x05 \x01(\x0b\x32\x35.bosdyn.api.graph_nav.UpdateCallbackResponse.CompleteH\x00\x1a\x83\x02\n\tNavPolicy\x12O\n\x08\x61t_start\x18\x01 \x01(\x0e\x32=.bosdyn.api.graph_nav.UpdateCallbackResponse.NavPolicy.Option\x12M\n\x06\x61t_end\x18\x02 \x01(\x0e\x32=.bosdyn.api.graph_nav.UpdateCallbackResponse.NavPolicy.Option\"V\n\x06Option\x12\x12\n\x0eOPTION_UNKNOWN\x10\x00\x12\x13\n\x0fOPTION_CONTINUE\x10\x01\x12\x0f\n\x0bOPTION_STOP\x10\x02\x12\x12\n\x0eOPTION_CONTROL\x10\x03\x1a\xff\x01\n\x05\x45rror\x12K\n\x05\x65rror\x18\x01 \x01(\x0e\x32<.bosdyn.api.graph_nav.UpdateCallbackResponse.Error.ErrorType\x12\x35\n\x11lease_use_results\x18\x02 \x03(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\"r\n\tErrorType\x12\x11\n\rERROR_UNKNOWN\x10\x00\x12\x11\n\rERROR_BLOCKED\x10\x01\x12\x19\n\x15\x45RROR_CALLBACK_FAILED\x10\x02\x12\x0f\n\x0b\x45RROR_LEASE\x10\x03\x12\x13\n\x0f\x45RROR_TIMED_OUT\x10\x04\x1a\n\n\x08\x43omplete\"g\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1d\n\x19STATUS_INVALID_COMMAND_ID\x10\x02\x12\x1b\n\x17STATUS_EXPIRED_END_TIME\x10\x03\x42\n\n\x08response\"S\n\x12\x45ndCallbackRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x12\n\ncommand_id\x18\x02 \x01(\r\"\xf4\x01\n\x13\x45ndCallbackResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12@\n\x06status\x18\x02 \x01(\x0e\x32\x30.bosdyn.api.graph_nav.EndCallbackResponse.Status\"o\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1d\n\x19STATUS_INVALID_COMMAND_ID\x10\x02\x12#\n\x1fSTATUS_SHUTDOWN_CALLBACK_FAILED\x10\x03\x42\x13\x42\x11\x41reaCallbackProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(bosdyn/api/graph_nav/area_callback.proto\x12\x14\x62osdyn.api.graph_nav\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x17\x62osdyn/api/header.proto\x1a\x16\x62osdyn/api/lease.proto\x1a&bosdyn/api/service_customization.proto\x1a-bosdyn/api/graph_nav/area_callback_data.proto\x1a\x1e\x62osdyn/api/graph_nav/nav.proto\"\xf1\x03\n\x11\x41reaCallbackError\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12@\n\x05\x65rror\x18\x02 \x01(\x0e\x32\x31.bosdyn.api.graph_nav.AreaCallbackError.CallError\x12\x45\n\x0e\x62\x65gin_callback\x18\x03 \x01(\x0b\x32+.bosdyn.api.graph_nav.BeginCallbackResponseH\x00\x12\x43\n\rbegin_control\x18\x04 \x01(\x0b\x32*.bosdyn.api.graph_nav.BeginControlResponseH\x00\x12G\n\x0fupdate_callback\x18\x05 \x01(\x0b\x32,.bosdyn.api.graph_nav.UpdateCallbackResponseH\x00\x12\x41\n\x0c\x65nd_callback\x18\x06 \x01(\x0b\x32).bosdyn.api.graph_nav.EndCallbackResponseH\x00\"Z\n\tCallError\x12\x11\n\rERROR_UNKNOWN\x10\x00\x12\x13\n\x0f\x45RROR_TRANSPORT\x10\x01\x12\x12\n\x0e\x45RROR_RESPONSE\x10\x02\x12\x11\n\rERROR_SERVICE\x10\x03\x42\x10\n\x0eresponse_error\"K\n\x1e\x41reaCallbackInformationRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"n\n\x17\x41reaCallbackInformation\x12 \n\x18required_lease_resources\x18\x01 \x03(\t\x12\x31\n\rcustom_params\x18\x04 \x01(\x0b\x32\x1a.bosdyn.api.DictParam.Spec\"\x8a\x01\n\x1f\x41reaCallbackInformationResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12;\n\x04info\x18\x02 \x01(\x0b\x32-.bosdyn.api.graph_nav.AreaCallbackInformation\"g\n\x11RegionInformation\x12\x11\n\tregion_id\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12*\n\x05route\x18\x03 \x01(\x0b\x32\x1b.bosdyn.api.graph_nav.Route\"\x9a\x02\n\x14\x42\x65ginCallbackRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12<\n\x0bregion_info\x18\x04 \x01(\x0b\x32\'.bosdyn.api.graph_nav.RegionInformation\x12,\n\x08\x65nd_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12=\n\rrecorded_data\x18\x05 \x01(\x0b\x32&.bosdyn.api.graph_nav.AreaCallbackData\x12,\n\rcustom_params\x18\x06 \x01(\x0b\x32\x15.bosdyn.api.DictParam\"\xe2\x02\n\x15\x42\x65ginCallbackResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x42\n\x06status\x18\x02 \x01(\x0e\x32\x32.bosdyn.api.graph_nav.BeginCallbackResponse.Status\x12\x12\n\ncommand_id\x18\x03 \x01(\r\x12\x38\n\x12\x63ustom_param_error\x18\x04 \x01(\x0b\x32\x1c.bosdyn.api.CustomParamError\"\x8a\x01\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12 \n\x1cSTATUS_INVALID_CONFIGURATION\x10\x02\x12\x1b\n\x17STATUS_EXPIRED_END_TIME\x10\x03\x12\x1e\n\x1aSTATUS_CUSTOM_PARAMS_ERROR\x10\x08\"w\n\x13\x42\x65ginControlRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12!\n\x06leases\x18\x02 \x03(\x0b\x32\x11.bosdyn.api.Lease\x12\x12\n\ncommand_id\x18\x03 \x01(\r\"\xc5\x02\n\x14\x42\x65ginControlResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x35\n\x11lease_use_results\x18\x02 \x03(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12\x41\n\x06status\x18\x03 \x01(\x0e\x32\x31.bosdyn.api.graph_nav.BeginControlResponse.Status\"\x86\x01\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1d\n\x19STATUS_INVALID_COMMAND_ID\x10\x02\x12\"\n\x1eSTATUS_MISSING_LEASE_RESOURCES\x10\x03\x12\x16\n\x12STATUS_LEASE_ERROR\x10\x04\"\xae\x02\n\x15UpdateCallbackRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x12\n\ncommand_id\x18\x02 \x01(\r\x12,\n\x08\x65nd_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12@\n\x05stage\x18\x04 \x01(\x0e\x32\x31.bosdyn.api.graph_nav.UpdateCallbackRequest.Stage\"f\n\x05Stage\x12\x11\n\rSTAGE_UNKNOWN\x10\x00\x12\x12\n\x0eSTAGE_TO_START\x10\x01\x12\x12\n\x0eSTAGE_AT_START\x10\x02\x12\x10\n\x0cSTAGE_TO_END\x10\x03\x12\x10\n\x0cSTAGE_AT_END\x10\x04\"\x87\n\n\x16UpdateCallbackResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x43\n\x06status\x18\x02 \x01(\x0e\x32\x33.bosdyn.api.graph_nav.UpdateCallbackResponse.Status\x12H\n\x06policy\x18\x03 \x01(\x0b\x32\x36.bosdyn.api.graph_nav.UpdateCallbackResponse.NavPolicyH\x00\x12\x43\n\x05\x65rror\x18\x04 \x01(\x0b\x32\x32.bosdyn.api.graph_nav.UpdateCallbackResponse.ErrorH\x00\x12I\n\x08\x63omplete\x18\x05 \x01(\x0b\x32\x35.bosdyn.api.graph_nav.UpdateCallbackResponse.CompleteH\x00\x12U\n\x0clocalization\x18\x06 \x01(\x0b\x32?.bosdyn.api.graph_nav.UpdateCallbackResponse.UpdateLocalization\x1a\xc1\x01\n\x12UpdateLocalization\x12\x62\n\x06\x63hange\x18\x01 \x01(\x0e\x32R.bosdyn.api.graph_nav.UpdateCallbackResponse.UpdateLocalization.LocalizationChange\"G\n\x12LocalizationChange\x12\x18\n\x14LOCALIZATION_UNKNOWN\x10\x00\x12\x17\n\x13LOCALIZATION_AT_END\x10\x01\x1a\x83\x02\n\tNavPolicy\x12O\n\x08\x61t_start\x18\x01 \x01(\x0e\x32=.bosdyn.api.graph_nav.UpdateCallbackResponse.NavPolicy.Option\x12M\n\x06\x61t_end\x18\x02 \x01(\x0e\x32=.bosdyn.api.graph_nav.UpdateCallbackResponse.NavPolicy.Option\"V\n\x06Option\x12\x12\n\x0eOPTION_UNKNOWN\x10\x00\x12\x13\n\x0fOPTION_CONTINUE\x10\x01\x12\x0f\n\x0bOPTION_STOP\x10\x02\x12\x12\n\x0eOPTION_CONTROL\x10\x03\x1a\xff\x01\n\x05\x45rror\x12K\n\x05\x65rror\x18\x01 \x01(\x0e\x32<.bosdyn.api.graph_nav.UpdateCallbackResponse.Error.ErrorType\x12\x35\n\x11lease_use_results\x18\x02 \x03(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\"r\n\tErrorType\x12\x11\n\rERROR_UNKNOWN\x10\x00\x12\x11\n\rERROR_BLOCKED\x10\x01\x12\x19\n\x15\x45RROR_CALLBACK_FAILED\x10\x02\x12\x0f\n\x0b\x45RROR_LEASE\x10\x03\x12\x13\n\x0f\x45RROR_TIMED_OUT\x10\x04\x1a\n\n\x08\x43omplete\"g\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1d\n\x19STATUS_INVALID_COMMAND_ID\x10\x02\x12\x1b\n\x17STATUS_EXPIRED_END_TIME\x10\x03\x42\n\n\x08response\"S\n\x12\x45ndCallbackRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x12\n\ncommand_id\x18\x02 \x01(\r\"\xf4\x01\n\x13\x45ndCallbackResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12@\n\x06status\x18\x02 \x01(\x0e\x32\x30.bosdyn.api.graph_nav.EndCallbackResponse.Status\"o\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1d\n\x19STATUS_INVALID_COMMAND_ID\x10\x02\x12#\n\x1fSTATUS_SHUTDOWN_CALLBACK_FAILED\x10\x03\x42\x13\x42\x11\x41reaCallbackProtob\x06proto3')
 
 
 
 _AREACALLBACKERROR = DESCRIPTOR.message_types_by_name['AreaCallbackError']
 _AREACALLBACKINFORMATIONREQUEST = DESCRIPTOR.message_types_by_name['AreaCallbackInformationRequest']
 _AREACALLBACKINFORMATION = DESCRIPTOR.message_types_by_name['AreaCallbackInformation']
 _AREACALLBACKINFORMATIONRESPONSE = DESCRIPTOR.message_types_by_name['AreaCallbackInformationResponse']
 _REGIONINFORMATION = DESCRIPTOR.message_types_by_name['RegionInformation']
 _BEGINCALLBACKREQUEST = DESCRIPTOR.message_types_by_name['BeginCallbackRequest']
 _BEGINCALLBACKRESPONSE = DESCRIPTOR.message_types_by_name['BeginCallbackResponse']
 _BEGINCONTROLREQUEST = DESCRIPTOR.message_types_by_name['BeginControlRequest']
 _BEGINCONTROLRESPONSE = DESCRIPTOR.message_types_by_name['BeginControlResponse']
 _UPDATECALLBACKREQUEST = DESCRIPTOR.message_types_by_name['UpdateCallbackRequest']
 _UPDATECALLBACKRESPONSE = DESCRIPTOR.message_types_by_name['UpdateCallbackResponse']
+_UPDATECALLBACKRESPONSE_UPDATELOCALIZATION = _UPDATECALLBACKRESPONSE.nested_types_by_name['UpdateLocalization']
 _UPDATECALLBACKRESPONSE_NAVPOLICY = _UPDATECALLBACKRESPONSE.nested_types_by_name['NavPolicy']
 _UPDATECALLBACKRESPONSE_ERROR = _UPDATECALLBACKRESPONSE.nested_types_by_name['Error']
 _UPDATECALLBACKRESPONSE_COMPLETE = _UPDATECALLBACKRESPONSE.nested_types_by_name['Complete']
 _ENDCALLBACKREQUEST = DESCRIPTOR.message_types_by_name['EndCallbackRequest']
 _ENDCALLBACKRESPONSE = DESCRIPTOR.message_types_by_name['EndCallbackResponse']
 _AREACALLBACKERROR_CALLERROR = _AREACALLBACKERROR.enum_types_by_name['CallError']
 _BEGINCALLBACKRESPONSE_STATUS = _BEGINCALLBACKRESPONSE.enum_types_by_name['Status']
 _BEGINCONTROLRESPONSE_STATUS = _BEGINCONTROLRESPONSE.enum_types_by_name['Status']
 _UPDATECALLBACKREQUEST_STAGE = _UPDATECALLBACKREQUEST.enum_types_by_name['Stage']
+_UPDATECALLBACKRESPONSE_UPDATELOCALIZATION_LOCALIZATIONCHANGE = _UPDATECALLBACKRESPONSE_UPDATELOCALIZATION.enum_types_by_name['LocalizationChange']
 _UPDATECALLBACKRESPONSE_NAVPOLICY_OPTION = _UPDATECALLBACKRESPONSE_NAVPOLICY.enum_types_by_name['Option']
 _UPDATECALLBACKRESPONSE_ERROR_ERRORTYPE = _UPDATECALLBACKRESPONSE_ERROR.enum_types_by_name['ErrorType']
 _UPDATECALLBACKRESPONSE_STATUS = _UPDATECALLBACKRESPONSE.enum_types_by_name['Status']
 _ENDCALLBACKRESPONSE_STATUS = _ENDCALLBACKRESPONSE.enum_types_by_name['Status']
 AreaCallbackError = _reflection.GeneratedProtocolMessageType('AreaCallbackError', (_message.Message,), {
   'DESCRIPTOR' : _AREACALLBACKERROR,
   '__module__' : 'bosdyn.api.graph_nav.area_callback_pb2'
@@ -114,14 +118,21 @@
   '__module__' : 'bosdyn.api.graph_nav.area_callback_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.graph_nav.UpdateCallbackRequest)
   })
 _sym_db.RegisterMessage(UpdateCallbackRequest)
 
 UpdateCallbackResponse = _reflection.GeneratedProtocolMessageType('UpdateCallbackResponse', (_message.Message,), {
 
+  'UpdateLocalization' : _reflection.GeneratedProtocolMessageType('UpdateLocalization', (_message.Message,), {
+    'DESCRIPTOR' : _UPDATECALLBACKRESPONSE_UPDATELOCALIZATION,
+    '__module__' : 'bosdyn.api.graph_nav.area_callback_pb2'
+    # @@protoc_insertion_point(class_scope:bosdyn.api.graph_nav.UpdateCallbackResponse.UpdateLocalization)
+    })
+  ,
+
   'NavPolicy' : _reflection.GeneratedProtocolMessageType('NavPolicy', (_message.Message,), {
     'DESCRIPTOR' : _UPDATECALLBACKRESPONSE_NAVPOLICY,
     '__module__' : 'bosdyn.api.graph_nav.area_callback_pb2'
     # @@protoc_insertion_point(class_scope:bosdyn.api.graph_nav.UpdateCallbackResponse.NavPolicy)
     })
   ,
 
@@ -139,14 +150,15 @@
     })
   ,
   'DESCRIPTOR' : _UPDATECALLBACKRESPONSE,
   '__module__' : 'bosdyn.api.graph_nav.area_callback_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.graph_nav.UpdateCallbackResponse)
   })
 _sym_db.RegisterMessage(UpdateCallbackResponse)
+_sym_db.RegisterMessage(UpdateCallbackResponse.UpdateLocalization)
 _sym_db.RegisterMessage(UpdateCallbackResponse.NavPolicy)
 _sym_db.RegisterMessage(UpdateCallbackResponse.Error)
 _sym_db.RegisterMessage(UpdateCallbackResponse.Complete)
 
 EndCallbackRequest = _reflection.GeneratedProtocolMessageType('EndCallbackRequest', (_message.Message,), {
   'DESCRIPTOR' : _ENDCALLBACKREQUEST,
   '__module__' : 'bosdyn.api.graph_nav.area_callback_pb2'
@@ -161,56 +173,60 @@
   })
 _sym_db.RegisterMessage(EndCallbackResponse)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'B\021AreaCallbackProto'
-  _AREACALLBACKERROR._serialized_start=181
-  _AREACALLBACKERROR._serialized_end=678
-  _AREACALLBACKERROR_CALLERROR._serialized_start=570
-  _AREACALLBACKERROR_CALLERROR._serialized_end=660
-  _AREACALLBACKINFORMATIONREQUEST._serialized_start=680
-  _AREACALLBACKINFORMATIONREQUEST._serialized_end=755
-  _AREACALLBACKINFORMATION._serialized_start=757
-  _AREACALLBACKINFORMATION._serialized_end=816
-  _AREACALLBACKINFORMATIONRESPONSE._serialized_start=819
-  _AREACALLBACKINFORMATIONRESPONSE._serialized_end=957
-  _REGIONINFORMATION._serialized_start=959
-  _REGIONINFORMATION._serialized_end=1062
-  _BEGINCALLBACKREQUEST._serialized_start=1065
-  _BEGINCALLBACKREQUEST._serialized_end=1238
-  _BEGINCALLBACKRESPONSE._serialized_start=1241
-  _BEGINCALLBACKRESPONSE._serialized_end=1504
-  _BEGINCALLBACKRESPONSE_STATUS._serialized_start=1398
-  _BEGINCALLBACKRESPONSE_STATUS._serialized_end=1504
-  _BEGINCONTROLREQUEST._serialized_start=1506
-  _BEGINCONTROLREQUEST._serialized_end=1625
-  _BEGINCONTROLRESPONSE._serialized_start=1628
-  _BEGINCONTROLRESPONSE._serialized_end=1953
-  _BEGINCONTROLRESPONSE_STATUS._serialized_start=1819
-  _BEGINCONTROLRESPONSE_STATUS._serialized_end=1953
-  _UPDATECALLBACKREQUEST._serialized_start=1956
-  _UPDATECALLBACKREQUEST._serialized_end=2258
-  _UPDATECALLBACKREQUEST_STAGE._serialized_start=2156
-  _UPDATECALLBACKREQUEST_STAGE._serialized_end=2258
-  _UPDATECALLBACKRESPONSE._serialized_start=2261
-  _UPDATECALLBACKRESPONSE._serialized_end=3265
-  _UPDATECALLBACKRESPONSE_NAVPOLICY._serialized_start=2619
-  _UPDATECALLBACKRESPONSE_NAVPOLICY._serialized_end=2878
-  _UPDATECALLBACKRESPONSE_NAVPOLICY_OPTION._serialized_start=2792
-  _UPDATECALLBACKRESPONSE_NAVPOLICY_OPTION._serialized_end=2878
-  _UPDATECALLBACKRESPONSE_ERROR._serialized_start=2881
-  _UPDATECALLBACKRESPONSE_ERROR._serialized_end=3136
-  _UPDATECALLBACKRESPONSE_ERROR_ERRORTYPE._serialized_start=3022
-  _UPDATECALLBACKRESPONSE_ERROR_ERRORTYPE._serialized_end=3136
-  _UPDATECALLBACKRESPONSE_COMPLETE._serialized_start=3138
-  _UPDATECALLBACKRESPONSE_COMPLETE._serialized_end=3148
-  _UPDATECALLBACKRESPONSE_STATUS._serialized_start=3150
-  _UPDATECALLBACKRESPONSE_STATUS._serialized_end=3253
-  _ENDCALLBACKREQUEST._serialized_start=3267
-  _ENDCALLBACKREQUEST._serialized_end=3350
-  _ENDCALLBACKRESPONSE._serialized_start=3353
-  _ENDCALLBACKRESPONSE._serialized_end=3597
-  _ENDCALLBACKRESPONSE_STATUS._serialized_start=3486
-  _ENDCALLBACKRESPONSE_STATUS._serialized_end=3597
+  _AREACALLBACKERROR._serialized_start=268
+  _AREACALLBACKERROR._serialized_end=765
+  _AREACALLBACKERROR_CALLERROR._serialized_start=657
+  _AREACALLBACKERROR_CALLERROR._serialized_end=747
+  _AREACALLBACKINFORMATIONREQUEST._serialized_start=767
+  _AREACALLBACKINFORMATIONREQUEST._serialized_end=842
+  _AREACALLBACKINFORMATION._serialized_start=844
+  _AREACALLBACKINFORMATION._serialized_end=954
+  _AREACALLBACKINFORMATIONRESPONSE._serialized_start=957
+  _AREACALLBACKINFORMATIONRESPONSE._serialized_end=1095
+  _REGIONINFORMATION._serialized_start=1097
+  _REGIONINFORMATION._serialized_end=1200
+  _BEGINCALLBACKREQUEST._serialized_start=1203
+  _BEGINCALLBACKREQUEST._serialized_end=1485
+  _BEGINCALLBACKRESPONSE._serialized_start=1488
+  _BEGINCALLBACKRESPONSE._serialized_end=1842
+  _BEGINCALLBACKRESPONSE_STATUS._serialized_start=1704
+  _BEGINCALLBACKRESPONSE_STATUS._serialized_end=1842
+  _BEGINCONTROLREQUEST._serialized_start=1844
+  _BEGINCONTROLREQUEST._serialized_end=1963
+  _BEGINCONTROLRESPONSE._serialized_start=1966
+  _BEGINCONTROLRESPONSE._serialized_end=2291
+  _BEGINCONTROLRESPONSE_STATUS._serialized_start=2157
+  _BEGINCONTROLRESPONSE_STATUS._serialized_end=2291
+  _UPDATECALLBACKREQUEST._serialized_start=2294
+  _UPDATECALLBACKREQUEST._serialized_end=2596
+  _UPDATECALLBACKREQUEST_STAGE._serialized_start=2494
+  _UPDATECALLBACKREQUEST_STAGE._serialized_end=2596
+  _UPDATECALLBACKRESPONSE._serialized_start=2599
+  _UPDATECALLBACKRESPONSE._serialized_end=3886
+  _UPDATECALLBACKRESPONSE_UPDATELOCALIZATION._serialized_start=3044
+  _UPDATECALLBACKRESPONSE_UPDATELOCALIZATION._serialized_end=3237
+  _UPDATECALLBACKRESPONSE_UPDATELOCALIZATION_LOCALIZATIONCHANGE._serialized_start=3166
+  _UPDATECALLBACKRESPONSE_UPDATELOCALIZATION_LOCALIZATIONCHANGE._serialized_end=3237
+  _UPDATECALLBACKRESPONSE_NAVPOLICY._serialized_start=3240
+  _UPDATECALLBACKRESPONSE_NAVPOLICY._serialized_end=3499
+  _UPDATECALLBACKRESPONSE_NAVPOLICY_OPTION._serialized_start=3413
+  _UPDATECALLBACKRESPONSE_NAVPOLICY_OPTION._serialized_end=3499
+  _UPDATECALLBACKRESPONSE_ERROR._serialized_start=3502
+  _UPDATECALLBACKRESPONSE_ERROR._serialized_end=3757
+  _UPDATECALLBACKRESPONSE_ERROR_ERRORTYPE._serialized_start=3643
+  _UPDATECALLBACKRESPONSE_ERROR_ERRORTYPE._serialized_end=3757
+  _UPDATECALLBACKRESPONSE_COMPLETE._serialized_start=3759
+  _UPDATECALLBACKRESPONSE_COMPLETE._serialized_end=3769
+  _UPDATECALLBACKRESPONSE_STATUS._serialized_start=3771
+  _UPDATECALLBACKRESPONSE_STATUS._serialized_end=3874
+  _ENDCALLBACKREQUEST._serialized_start=3888
+  _ENDCALLBACKREQUEST._serialized_end=3971
+  _ENDCALLBACKRESPONSE._serialized_start=3974
+  _ENDCALLBACKRESPONSE._serialized_end=4218
+  _ENDCALLBACKRESPONSE_STATUS._serialized_start=4107
+  _ENDCALLBACKRESPONSE_STATUS._serialized_end=4218
 # @@protoc_insertion_point(module_scope)
```

## bosdyn/api/graph_nav/graph_nav_pb2.py

```diff
@@ -18,29 +18,31 @@
 from bosdyn.api.graph_nav import nav_pb2 as bosdyn_dot_api_dot_graph__nav_dot_nav__pb2
 from bosdyn.api.graph_nav import map_pb2 as bosdyn_dot_api_dot_graph__nav_dot_map__pb2
 from bosdyn.api.graph_nav import area_callback_pb2 as bosdyn_dot_api_dot_graph__nav_dot_area__callback__pb2
 from bosdyn.api import header_pb2 as bosdyn_dot_api_dot_header__pb2
 from bosdyn.api import lease_pb2 as bosdyn_dot_api_dot_lease__pb2
 from bosdyn.api import license_pb2 as bosdyn_dot_api_dot_license__pb2
 from bosdyn.api import robot_state_pb2 as bosdyn_dot_api_dot_robot__state__pb2
+from bosdyn.api import service_fault_pb2 as bosdyn_dot_api_dot_service__fault__pb2
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$bosdyn/api/graph_nav/graph_nav.proto\x12\x14\x62osdyn.api.graph_nav\x1a\x1e\x62osdyn/api/basic_command.proto\x1a\x1b\x62osdyn/api/data_chunk.proto\x1a\x19\x62osdyn/api/geometry.proto\x1a\x1e\x62osdyn/api/graph_nav/nav.proto\x1a\x1e\x62osdyn/api/graph_nav/map.proto\x1a(bosdyn/api/graph_nav/area_callback.proto\x1a\x17\x62osdyn/api/header.proto\x1a\x16\x62osdyn/api/lease.proto\x1a\x18\x62osdyn/api/license.proto\x1a\x1c\x62osdyn/api/robot_state.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"<\n\x17VisualRefinementOptions\x12!\n\x19verify_refinement_quality\x18\x01 \x01(\x08\"\xc7\x05\n\x16SetLocalizationRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x39\n\rinitial_guess\x18\x03 \x01(\x0b\x32\".bosdyn.api.graph_nav.Localization\x12*\n\rko_tform_body\x18\x04 \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\x12\x14\n\x0cmax_distance\x18\x05 \x01(\x01\x12\x0f\n\x07max_yaw\x18\x06 \x01(\x01\x12P\n\rfiducial_init\x18\x07 \x01(\x0e\x32\x39.bosdyn.api.graph_nav.SetLocalizationRequest.FiducialInit\x12\x17\n\x0fuse_fiducial_id\x18\x08 \x01(\x05\x12\x1a\n\x12\x64o_ambiguity_check\x18\n \x01(\x08\x12\x37\n/restrict_fiducial_detections_to_target_waypoint\x18\x0b \x01(\x08\x12)\n\x1frefine_fiducial_result_with_icp\x18\t \x01(\x08H\x00\x12T\n\x1brefine_with_visual_features\x18\x0c \x01(\x0b\x32-.bosdyn.api.graph_nav.VisualRefinementOptionsH\x00\"\xa4\x01\n\x0c\x46iducialInit\x12\x19\n\x15\x46IDUCIAL_INIT_UNKNOWN\x10\x00\x12\x1d\n\x19\x46IDUCIAL_INIT_NO_FIDUCIAL\x10\x01\x12\x19\n\x15\x46IDUCIAL_INIT_NEAREST\x10\x02\x12#\n\x1f\x46IDUCIAL_INIT_NEAREST_AT_TARGET\x10\x03\x12\x1a\n\x16\x46IDUCIAL_INIT_SPECIFIC\x10\x04\x42\x0c\n\nrefinement\"[\n\x19SensorCompatibilityStatus\x12\x1a\n\x12map_has_lidar_data\x18\x01 \x01(\x08\x12\"\n\x1arobot_configured_for_lidar\x18\x02 \x01(\x08\"\x99\x07\n\x17SetLocalizationResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x34\n\x10lease_use_result\x18\x02 \x01(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12\x44\n\x06status\x18\x03 \x01(\x0e\x32\x34.bosdyn.api.graph_nav.SetLocalizationResponse.Status\x12\x14\n\x0c\x65rror_report\x18\x04 \x01(\t\x12\x38\n\x0clocalization\x18\x05 \x01(\x0b\x32\".bosdyn.api.graph_nav.Localization\x12]\n\x13suspected_ambiguity\x18\x07 \x01(\x0b\x32@.bosdyn.api.graph_nav.SetLocalizationResponse.SuspectedAmbiguity\x12\x36\n\x0eimpaired_state\x18\x08 \x01(\x0b\x32\x1e.bosdyn.api.RobotImpairedState\x12\x46\n\rsensor_status\x18\t \x01(\x0b\x32/.bosdyn.api.graph_nav.SensorCompatibilityStatus\x1aQ\n\x12SuspectedAmbiguity\x12;\n\x1e\x61lternate_robot_tform_waypoint\x18\x01 \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\"\xd3\x02\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x19\n\x15STATUS_ROBOT_IMPAIRED\x10\x02\x12\x1b\n\x17STATUS_UNKNOWN_WAYPOINT\x10\x03\x12\x12\n\x0eSTATUS_ABORTED\x10\x04\x12\x11\n\rSTATUS_FAILED\x10\x05\x12 \n\x1cSTATUS_FIDUCIAL_TOO_FAR_AWAY\x10\x06\x12\x1b\n\x17STATUS_FIDUCIAL_TOO_OLD\x10\x07\x12\x1f\n\x1bSTATUS_NO_MATCHING_FIDUCIAL\x10\x08\x12\"\n\x1eSTATUS_FIDUCIAL_POSE_UNCERTAIN\x10\t\x12\x1f\n\x1bSTATUS_INCOMPATIBLE_SENSORS\x10\n\x12\"\n\x1eSTATUS_VISUAL_ALIGNMENT_FAILED\x10\x0b\"\x10\n\x0eRouteGenParams\"\x99\x05\n\x0cTravelParams\x12\x14\n\x0cmax_distance\x18\x01 \x01(\x01\x12\x0f\n\x07max_yaw\x18\x02 \x01(\x01\x12\x34\n\x0evelocity_limit\x18\x03 \x01(\x0b\x32\x1c.bosdyn.api.SE2VelocityLimit\x12\x18\n\x10ignore_final_yaw\x18\x04 \x01(\x08\x12]\n\x19\x66\x65\x61ture_quality_tolerance\x18\x05 \x01(\x0e\x32:.bosdyn.api.graph_nav.TravelParams.FeatureQualityTolerance\x12$\n\x1c\x64isable_directed_exploration\x18\x06 \x01(\x08\x12\'\n\x1f\x64isable_alternate_route_finding\x18\x08 \x01(\x08\x12U\n\x13path_following_mode\x18\t \x01(\x0e\x32\x38.bosdyn.api.graph_nav.Edge.Annotations.PathFollowingMode\x12\x39\n\x16\x62locked_path_wait_time\x18\n \x01(\x0b\x32\x19.google.protobuf.Duration\x12^\n\x13ground_clutter_mode\x18\x0b \x01(\x0e\x32\x41.bosdyn.api.graph_nav.Edge.Annotations.GroundClutterAvoidanceMode\"r\n\x17\x46\x65\x61tureQualityTolerance\x12\x15\n\x11TOLERANCE_UNKNOWN\x10\x00\x12\x15\n\x11TOLERANCE_DEFAULT\x10\x01\x12)\n%TOLERANCE_IGNORE_POOR_FEATURE_QUALITY\x10\x02\"\x98\x03\n\x11NavigateToRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12!\n\x06leases\x18\x02 \x03(\x0b\x32\x11.bosdyn.api.Lease\x12\x1f\n\x17\x64\x65stination_waypoint_id\x18\x03 \x01(\t\x12:\n\x0croute_params\x18\x04 \x01(\x0b\x32$.bosdyn.api.graph_nav.RouteGenParams\x12\x39\n\rtravel_params\x18\x05 \x01(\x0b\x32\".bosdyn.api.graph_nav.TravelParams\x12,\n\x08\x65nd_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10\x63lock_identifier\x18\x07 \x01(\t\x12\x41\n$destination_waypoint_tform_body_goal\x18\x08 \x01(\x0b\x32\x13.bosdyn.api.SE2Pose\x12\x12\n\ncommand_id\x18\t \x01(\r\"\x84\x06\n\x12NavigateToResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x35\n\x11lease_use_results\x18\x02 \x03(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12?\n\x06status\x18\x03 \x01(\x0e\x32/.bosdyn.api.graph_nav.NavigateToResponse.Status\x12\x36\n\x0eimpaired_state\x18\x06 \x01(\x0b\x32\x1e.bosdyn.api.RobotImpairedState\x12\x12\n\ncommand_id\x18\x04 \x01(\r\x12\x1a\n\x12\x65rror_waypoint_ids\x18\x05 \x03(\t\x12K\n\x13\x61rea_callback_error\x18\n \x01(\x0b\x32..bosdyn.api.graph_nav.AreaCallbackServiceError\"\x94\x03\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x16\n\x12STATUS_NO_TIMESYNC\x10\x02\x12\x12\n\x0eSTATUS_EXPIRED\x10\x03\x12\x16\n\x12STATUS_TOO_DISTANT\x10\x04\x12\x19\n\x15STATUS_ROBOT_IMPAIRED\x10\x05\x12\x14\n\x10STATUS_RECORDING\x10\x06\x12\x1b\n\x17STATUS_UNKNOWN_WAYPOINT\x10\x07\x12\x12\n\x0eSTATUS_NO_PATH\x10\x08\x12\x19\n\x15STATUS_FEATURE_DESERT\x10\n\x12\x0f\n\x0bSTATUS_LOST\x10\x0b\x12\x1f\n\x1bSTATUS_NOT_LOCALIZED_TO_MAP\x10\r\x12!\n\x1dSTATUS_COULD_NOT_UPDATE_ROUTE\x10\x0c\x12\x10\n\x0cSTATUS_STUCK\x10\x0e\x12\x1f\n\x1bSTATUS_UNRECOGNIZED_COMMAND\x10\x0f\x12\x1e\n\x1aSTATUS_AREA_CALLBACK_ERROR\x10\x10\"\xf7\x04\n\x14RouteFollowingParams\x12W\n\x10new_cmd_behavior\x18\x01 \x01(\x0e\x32=.bosdyn.api.graph_nav.RouteFollowingParams.StartRouteBehavior\x12X\n\x15\x65xisting_cmd_behavior\x18\x02 \x01(\x0e\x32\x39.bosdyn.api.graph_nav.RouteFollowingParams.ResumeBehavior\x12_\n\x16route_blocked_behavior\x18\x03 \x01(\x0e\x32?.bosdyn.api.graph_nav.RouteFollowingParams.RouteBlockedBehavior\"u\n\x12StartRouteBehavior\x12\x11\n\rSTART_UNKNOWN\x10\x00\x12\x14\n\x10START_GOTO_START\x10\x01\x12\x14\n\x10START_GOTO_ROUTE\x10\x02\x12 \n\x1cSTART_FAIL_WHEN_NOT_ON_ROUTE\x10\x03\"n\n\x0eResumeBehavior\x12\x12\n\x0eRESUME_UNKNOWN\x10\x00\x12%\n!RESUME_RETURN_TO_UNFINISHED_ROUTE\x10\x01\x12!\n\x1dRESUME_FAIL_WHEN_NOT_ON_ROUTE\x10\x02\"d\n\x14RouteBlockedBehavior\x12\x19\n\x15ROUTE_BLOCKED_UNKNOWN\x10\x00\x12\x19\n\x15ROUTE_BLOCKED_REROUTE\x10\x01\x12\x16\n\x12ROUTE_BLOCKED_FAIL\x10\x02\"\xb3\x03\n\x14NavigateRouteRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12!\n\x06leases\x18\x02 \x03(\x0b\x32\x11.bosdyn.api.Lease\x12*\n\x05route\x18\x03 \x01(\x0b\x32\x1b.bosdyn.api.graph_nav.Route\x12G\n\x13route_follow_params\x18\t \x01(\x0b\x32*.bosdyn.api.graph_nav.RouteFollowingParams\x12\x39\n\rtravel_params\x18\x04 \x01(\x0b\x32\".bosdyn.api.graph_nav.TravelParams\x12,\n\x08\x65nd_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10\x63lock_identifier\x18\x06 \x01(\t\x12\x41\n$destination_waypoint_tform_body_goal\x18\x07 \x01(\x0b\x32\x13.bosdyn.api.SE2Pose\x12\x12\n\ncommand_id\x18\x08 \x01(\r\"\xa0\x07\n\x15NavigateRouteResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x35\n\x11lease_use_results\x18\x02 \x03(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12\x42\n\x06status\x18\x03 \x01(\x0e\x32\x32.bosdyn.api.graph_nav.NavigateRouteResponse.Status\x12\x36\n\x0eimpaired_state\x18\x07 \x01(\x0b\x32\x1e.bosdyn.api.RobotImpairedState\x12\x12\n\ncommand_id\x18\x04 \x01(\r\x12\x1a\n\x12\x65rror_waypoint_ids\x18\x05 \x03(\t\x12\x35\n\x0e\x65rror_edge_ids\x18\x06 \x03(\x0b\x32\x1d.bosdyn.api.graph_nav.Edge.Id\x12K\n\x13\x61rea_callback_error\x18\x08 \x01(\x0b\x32..bosdyn.api.graph_nav.AreaCallbackServiceError\"\xf3\x03\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x16\n\x12STATUS_NO_TIMESYNC\x10\x02\x12\x12\n\x0eSTATUS_EXPIRED\x10\x03\x12\x16\n\x12STATUS_TOO_DISTANT\x10\x04\x12\x19\n\x15STATUS_ROBOT_IMPAIRED\x10\x05\x12\x14\n\x10STATUS_RECORDING\x10\x06\x12!\n\x1dSTATUS_UNKNOWN_ROUTE_ELEMENTS\x10\x08\x12\x17\n\x13STATUS_INVALID_EDGE\x10\t\x12\x12\n\x0eSTATUS_NO_PATH\x10\x14\x12\x1b\n\x17STATUS_CONSTRAINT_FAULT\x10\x0b\x12\x19\n\x15STATUS_FEATURE_DESERT\x10\r\x12\x0f\n\x0bSTATUS_LOST\x10\x0e\x12!\n\x1dSTATUS_NOT_LOCALIZED_TO_ROUTE\x10\x10\x12\x1f\n\x1bSTATUS_NOT_LOCALIZED_TO_MAP\x10\x13\x12!\n\x1dSTATUS_COULD_NOT_UPDATE_ROUTE\x10\x0f\x12\x10\n\x0cSTATUS_STUCK\x10\x11\x12\x1f\n\x1bSTATUS_UNRECOGNIZED_COMMAND\x10\x12\x12\x1e\n\x1aSTATUS_AREA_CALLBACK_ERROR\x10\x15\"\xad\x03\n\x17NavigateToAnchorRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12!\n\x06leases\x18\x02 \x03(\x0b\x32\x11.bosdyn.api.Lease\x12,\n\x0fseed_tform_goal\x18\x03 \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\x12\x43\n)goal_waypoint_rt_seed_ewrt_seed_tolerance\x18\x04 \x01(\x0b\x32\x10.bosdyn.api.Vec3\x12:\n\x0croute_params\x18\x06 \x01(\x0b\x32$.bosdyn.api.graph_nav.RouteGenParams\x12\x39\n\rtravel_params\x18\x07 \x01(\x0b\x32\".bosdyn.api.graph_nav.TravelParams\x12,\n\x08\x65nd_time\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10\x63lock_identifier\x18\t \x01(\t\x12\x12\n\ncommand_id\x18\n \x01(\r\"\xa5\x06\n\x18NavigateToAnchorResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x35\n\x11lease_use_results\x18\x02 \x03(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12\x45\n\x06status\x18\x03 \x01(\x0e\x32\x35.bosdyn.api.graph_nav.NavigateToAnchorResponse.Status\x12\x36\n\x0eimpaired_state\x18\x06 \x01(\x0b\x32\x1e.bosdyn.api.RobotImpairedState\x12\x12\n\ncommand_id\x18\x04 \x01(\r\x12\x1a\n\x12\x65rror_waypoint_ids\x18\x05 \x03(\t\x12K\n\x13\x61rea_callback_error\x18\x07 \x01(\x0b\x32..bosdyn.api.graph_nav.AreaCallbackServiceError\"\xa9\x03\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x16\n\x12STATUS_NO_TIMESYNC\x10\x02\x12\x12\n\x0eSTATUS_EXPIRED\x10\x03\x12\x16\n\x12STATUS_TOO_DISTANT\x10\x04\x12\x19\n\x15STATUS_ROBOT_IMPAIRED\x10\x05\x12\x14\n\x10STATUS_RECORDING\x10\x06\x12\x17\n\x13STATUS_NO_ANCHORING\x10\x07\x12\x12\n\x0eSTATUS_NO_PATH\x10\x08\x12\x19\n\x15STATUS_FEATURE_DESERT\x10\n\x12\x0f\n\x0bSTATUS_LOST\x10\x0b\x12\x1f\n\x1bSTATUS_NOT_LOCALIZED_TO_MAP\x10\r\x12!\n\x1dSTATUS_COULD_NOT_UPDATE_ROUTE\x10\x0c\x12\x10\n\x0cSTATUS_STUCK\x10\x0e\x12\x1f\n\x1bSTATUS_UNRECOGNIZED_COMMAND\x10\x0f\x12\x17\n\x13STATUS_INVALID_POSE\x10\x10\x12\x1e\n\x1aSTATUS_AREA_CALLBACK_ERROR\x10\x11\"Z\n\x19NavigationFeedbackRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x12\n\ncommand_id\x18\x02 \x01(\r\"\xba\x11\n\x1aNavigationFeedbackResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12G\n\x06status\x18\x02 \x01(\x0e\x32\x37.bosdyn.api.graph_nav.NavigationFeedbackResponse.Status\x12\x36\n\x0eimpaired_state\x18\x06 \x01(\x0b\x32\x1e.bosdyn.api.RobotImpairedState\x12\x66\n\x14\x61rea_callback_errors\x18\t \x03(\x0b\x32H.bosdyn.api.graph_nav.NavigationFeedbackResponse.AreaCallbackErrorsEntry\x12\x34\n\x0fremaining_route\x18\x03 \x01(\x0b\x32\x1b.bosdyn.api.graph_nav.Route\x12\x12\n\ncommand_id\x18\x04 \x01(\r\x12/\n\x12last_ko_tform_goal\x18\x05 \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\x12Z\n\x14\x62ody_movement_status\x18\x07 \x01(\x0e\x32<.bosdyn.api.SE2TrajectoryCommand.Feedback.BodyMovementStatus\x12U\n\x13path_following_mode\x18\x08 \x01(\x0e\x32\x38.bosdyn.api.graph_nav.Edge.Annotations.PathFollowingMode\x12p\n\x19\x61\x63tive_region_information\x18\n \x03(\x0b\x32M.bosdyn.api.graph_nav.NavigationFeedbackResponse.ActiveRegionInformationEntry\x12\x66\n\x16route_following_status\x18\xe8\x07 \x01(\x0e\x32\x45.bosdyn.api.graph_nav.NavigationFeedbackResponse.RouteFollowingStatus\x12Y\n\x0f\x62lockage_status\x18\xe9\x07 \x01(\x0e\x32?.bosdyn.api.graph_nav.NavigationFeedbackResponse.BlockageStatus\x1a\x62\n\x17\x41reaCallbackErrorsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x36\n\x05value\x18\x02 \x01(\x0b\x32\'.bosdyn.api.graph_nav.AreaCallbackError:\x02\x38\x01\x1a\x88\x01\n\x1c\x41\x63tiveRegionInformationEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12W\n\x05value\x18\x02 \x01(\x0b\x32H.bosdyn.api.graph_nav.NavigationFeedbackResponse.ActiveRegionInformation:\x02\x38\x01\x1a\xad\x02\n\x17\x41\x63tiveRegionInformation\x12\x13\n\x0b\x64\x65scription\x18\x01 \x01(\t\x12\x14\n\x0cservice_name\x18\x02 \x01(\t\x12r\n\rregion_status\x18\x03 \x01(\x0e\x32[.bosdyn.api.graph_nav.NavigationFeedbackResponse.ActiveRegionInformation.AreaCallbackStatus\"s\n\x12\x41reaCallbackStatus\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x15\n\x11STATUS_NAVIGATING\x10\x01\x12\x12\n\x0eSTATUS_WAITING\x10\x02\x12\x1e\n\x1aSTATUS_CALLBACK_IN_CONTROL\x10\x03\"\xf5\x02\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x1a\n\x16STATUS_FOLLOWING_ROUTE\x10\x01\x12\x17\n\x13STATUS_REACHED_GOAL\x10\x02\x12\x13\n\x0fSTATUS_NO_ROUTE\x10\x03\x12\x1a\n\x16STATUS_NO_LOCALIZATION\x10\x04\x12\x0f\n\x0bSTATUS_LOST\x10\x05\x12\x10\n\x0cSTATUS_STUCK\x10\x06\x12\x1c\n\x18STATUS_COMMAND_TIMED_OUT\x10\x07\x12\x19\n\x15STATUS_ROBOT_IMPAIRED\x10\x08\x12\x1b\n\x17STATUS_CONSTRAINT_FAULT\x10\x0b\x12\x1d\n\x19STATUS_COMMAND_OVERRIDDEN\x10\x0c\x12!\n\x1dSTATUS_NOT_LOCALIZED_TO_ROUTE\x10\r\x12\x16\n\x12STATUS_LEASE_ERROR\x10\x0e\x12\x1e\n\x1aSTATUS_AREA_CALLBACK_ERROR\x10\x0f\"\xf1\x01\n\x14RouteFollowingStatus\x12\"\n\x1eROUTE_FOLLOWING_STATUS_UNKNOWN\x10\x00\x12*\n&ROUTE_FOLLOWING_STATUS_FOLLOWING_ROUTE\x10\x01\x12-\n)ROUTE_FOLLOWING_STATUS_RETURNING_TO_ROUTE\x10\x02\x12\x34\n0ROUTE_FOLLOWING_STATUS_FOLLOWING_ALTERNATE_ROUTE\x10\x03\x12$\n ROUTE_FOLLOWING_STATUS_EXPLORING\x10\x04\"\x98\x01\n\x0e\x42lockageStatus\x12\x1b\n\x17\x42LOCKAGE_STATUS_UNKNOWN\x10\x00\x12\x1f\n\x1b\x42LOCKAGE_STATUS_ROUTE_CLEAR\x10\x01\x12-\n)BLOCKAGE_STATUS_ROUTE_BLOCKED_TEMPORARILY\x10\x02\x12\x19\n\x15\x42LOCKAGE_STATUS_STUCK\x10\x03\"\xa8\x02\n\x1bGetLocalizationStateRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x13\n\x0bwaypoint_id\x18\x08 \x01(\t\x12 \n\x18request_live_point_cloud\x18\x02 \x01(\x08\x12\x1b\n\x13request_live_images\x18\x03 \x01(\x08\x12!\n\x19request_live_terrain_maps\x18\x04 \x01(\x08\x12\"\n\x1arequest_live_world_objects\x18\x05 \x01(\x08\x12 \n\x18request_live_robot_state\x18\x06 \x01(\x08\x12!\n\x19\x63ompress_live_point_cloud\x18\x07 \x01(\x08\"]\n\x16RemotePointCloudStatus\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x1b\n\x13\x65xists_in_directory\x18\x02 \x01(\x08\x12\x10\n\x08has_data\x18\x03 \x01(\x08\"$\n\x11LostDetectorState\x12\x0f\n\x07is_lost\x18\x01 \x01(\x08\"\x86\x03\n\x1cGetLocalizationStateResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x38\n\x0clocalization\x18\x02 \x01(\x0b\x32\".bosdyn.api.graph_nav.Localization\x12\x34\n\x10robot_kinematics\x18\x04 \x01(\x0b\x32\x1a.bosdyn.api.KinematicState\x12I\n\x13remote_cloud_status\x18\x05 \x03(\x0b\x32,.bosdyn.api.graph_nav.RemotePointCloudStatus\x12\x39\n\tlive_data\x18\x06 \x01(\x0b\x32&.bosdyn.api.graph_nav.WaypointSnapshot\x12\x44\n\x13lost_detector_state\x18\x07 \x01(\x0b\x32\'.bosdyn.api.graph_nav.LostDetectorState\"`\n\x11\x43learGraphRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12 \n\x05lease\x18\x02 \x01(\x0b\x32\x11.bosdyn.api.Lease\"\xfa\x01\n\x12\x43learGraphResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x34\n\x10lease_use_result\x18\x02 \x01(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12?\n\x06status\x18\x03 \x01(\x0e\x32/.bosdyn.api.graph_nav.ClearGraphResponse.Status\"A\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x14\n\x10STATUS_RECORDING\x10\x02\"\xad\x01\n\x12UploadGraphRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12*\n\x05graph\x18\x02 \x01(\x0b\x32\x1b.bosdyn.api.graph_nav.Graph\x12 \n\x05lease\x18\x03 \x01(\x0b\x32\x11.bosdyn.api.Lease\x12\x1e\n\x16generate_new_anchoring\x18\x04 \x01(\x08\"\xc3\x05\n\x13UploadGraphResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12@\n\x06status\x18\x08 \x01(\x0e\x32\x30.bosdyn.api.graph_nav.UploadGraphResponse.Status\x12\x34\n\x10lease_use_result\x18\x02 \x01(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12$\n\x1cloaded_waypoint_snapshot_ids\x18\x03 \x03(\t\x12%\n\x1dunknown_waypoint_snapshot_ids\x18\x04 \x03(\t\x12 \n\x18loaded_edge_snapshot_ids\x18\x05 \x03(\t\x12!\n\x19unknown_edge_snapshot_ids\x18\x06 \x03(\t\x12\x36\n\x0elicense_status\x18\x07 \x01(\x0e\x32\x1e.bosdyn.api.LicenseInfo.Status\x12\x46\n\rsensor_status\x18\t \x01(\x0b\x32/.bosdyn.api.graph_nav.SensorCompatibilityStatus\x12K\n\x13\x61rea_callback_error\x18\n \x01(\x0b\x32..bosdyn.api.graph_nav.AreaCallbackServiceError\"\xa8\x01\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12 \n\x1cSTATUS_MAP_TOO_LARGE_LICENSE\x10\x03\x12\x18\n\x14STATUS_INVALID_GRAPH\x10\x04\x12\x1f\n\x1bSTATUS_INCOMPATIBLE_SENSORS\x10\x05\x12\x1e\n\x1aSTATUS_AREA_CALLBACK_ERROR\x10\x06\"A\n\x14\x44ownloadGraphRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"o\n\x15\x44ownloadGraphResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12*\n\x05graph\x18\x02 \x01(\x0b\x32\x1b.bosdyn.api.graph_nav.Graph\"\x92\x01\n\x1dUploadWaypointSnapshotRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12$\n\x05\x63hunk\x18\x03 \x01(\x0b\x32\x15.bosdyn.api.DataChunk\x12 \n\x05lease\x18\x04 \x01(\x0b\x32\x11.bosdyn.api.Lease\"\xe5\x02\n\x1eUploadWaypointSnapshotResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x34\n\x10lease_use_result\x18\x02 \x01(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12K\n\x06status\x18\x03 \x01(\x0e\x32;.bosdyn.api.graph_nav.UploadWaypointSnapshotResponse.Status\x12\x46\n\rsensor_status\x18\x04 \x01(\x0b\x32/.bosdyn.api.graph_nav.SensorCompatibilityStatus\"L\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1f\n\x1bSTATUS_INCOMPATIBLE_SENSORS\x10\x02\"\x8e\x01\n\x19UploadEdgeSnapshotRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12$\n\x05\x63hunk\x18\x04 \x01(\x0b\x32\x15.bosdyn.api.DataChunk\x12 \n\x05lease\x18\x05 \x01(\x0b\x32\x11.bosdyn.api.Lease\"~\n\x1aUploadEdgeSnapshotResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x34\n\x10lease_use_result\x18\x02 \x01(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\"\xc6\x01\n\x1f\x44ownloadWaypointSnapshotRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x1c\n\x14waypoint_snapshot_id\x18\x02 \x01(\t\x12\x17\n\x0f\x64ownload_images\x18\x03 \x01(\x08\x12\x1c\n\x14\x63ompress_point_cloud\x18\x04 \x01(\x08\x12#\n\x1b\x64o_not_download_point_cloud\x18\x05 \x01(\x08\"\xb2\x02\n DownloadWaypointSnapshotResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12M\n\x06status\x18\x02 \x01(\x0e\x32=.bosdyn.api.graph_nav.DownloadWaypointSnapshotResponse.Status\x12\x1c\n\x14waypoint_snapshot_id\x18\x04 \x01(\t\x12$\n\x05\x63hunk\x18\x05 \x01(\x0b\x32\x15.bosdyn.api.DataChunk\"O\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\"\n\x1eSTATUS_SNAPSHOT_DOES_NOT_EXIST\x10\x02\"b\n\x1b\x44ownloadEdgeSnapshotRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x18\n\x10\x65\x64ge_snapshot_id\x18\x02 \x01(\t\"\xa6\x02\n\x1c\x44ownloadEdgeSnapshotResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12I\n\x06status\x18\x02 \x01(\x0e\x32\x39.bosdyn.api.graph_nav.DownloadEdgeSnapshotResponse.Status\x12\x18\n\x10\x65\x64ge_snapshot_id\x18\x04 \x01(\t\x12$\n\x05\x63hunk\x18\x05 \x01(\x0b\x32\x15.bosdyn.api.DataChunk\"O\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\"\n\x1eSTATUS_SNAPSHOT_DOES_NOT_EXIST\x10\x02\"4\n\x18\x41reaCallbackServiceError\x12\x18\n\x10missing_services\x18\x01 \x03(\t\"A\n\x14ValidateGraphRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"\x8a\x03\n\x15ValidateGraphResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x42\n\x06status\x18\x02 \x01(\x0e\x32\x32.bosdyn.api.graph_nav.ValidateGraphResponse.Status\x12\x46\n\rsensor_status\x18\x03 \x01(\x0b\x32/.bosdyn.api.graph_nav.SensorCompatibilityStatus\x12K\n\x13\x61rea_callback_error\x18\x04 \x01(\x0b\x32..bosdyn.api.graph_nav.AreaCallbackServiceError\"l\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1f\n\x1bSTATUS_INCOMPATIBLE_SENSORS\x10\x05\x12\x1e\n\x1aSTATUS_AREA_CALLBACK_ERROR\x10\x06\x42\x0f\x42\rGraphNavProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$bosdyn/api/graph_nav/graph_nav.proto\x12\x14\x62osdyn.api.graph_nav\x1a\x1e\x62osdyn/api/basic_command.proto\x1a\x1b\x62osdyn/api/data_chunk.proto\x1a\x19\x62osdyn/api/geometry.proto\x1a\x1e\x62osdyn/api/graph_nav/nav.proto\x1a\x1e\x62osdyn/api/graph_nav/map.proto\x1a(bosdyn/api/graph_nav/area_callback.proto\x1a\x17\x62osdyn/api/header.proto\x1a\x16\x62osdyn/api/lease.proto\x1a\x18\x62osdyn/api/license.proto\x1a\x1c\x62osdyn/api/robot_state.proto\x1a\x1e\x62osdyn/api/service_fault.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"<\n\x17VisualRefinementOptions\x12!\n\x19verify_refinement_quality\x18\x01 \x01(\x08\"\xc7\x05\n\x16SetLocalizationRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x39\n\rinitial_guess\x18\x03 \x01(\x0b\x32\".bosdyn.api.graph_nav.Localization\x12*\n\rko_tform_body\x18\x04 \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\x12\x14\n\x0cmax_distance\x18\x05 \x01(\x01\x12\x0f\n\x07max_yaw\x18\x06 \x01(\x01\x12P\n\rfiducial_init\x18\x07 \x01(\x0e\x32\x39.bosdyn.api.graph_nav.SetLocalizationRequest.FiducialInit\x12\x17\n\x0fuse_fiducial_id\x18\x08 \x01(\x05\x12\x1a\n\x12\x64o_ambiguity_check\x18\n \x01(\x08\x12\x37\n/restrict_fiducial_detections_to_target_waypoint\x18\x0b \x01(\x08\x12)\n\x1frefine_fiducial_result_with_icp\x18\t \x01(\x08H\x00\x12T\n\x1brefine_with_visual_features\x18\x0c \x01(\x0b\x32-.bosdyn.api.graph_nav.VisualRefinementOptionsH\x00\"\xa4\x01\n\x0c\x46iducialInit\x12\x19\n\x15\x46IDUCIAL_INIT_UNKNOWN\x10\x00\x12\x1d\n\x19\x46IDUCIAL_INIT_NO_FIDUCIAL\x10\x01\x12\x19\n\x15\x46IDUCIAL_INIT_NEAREST\x10\x02\x12#\n\x1f\x46IDUCIAL_INIT_NEAREST_AT_TARGET\x10\x03\x12\x1a\n\x16\x46IDUCIAL_INIT_SPECIFIC\x10\x04\x42\x0c\n\nrefinement\"[\n\x19SensorCompatibilityStatus\x12\x1a\n\x12map_has_lidar_data\x18\x01 \x01(\x08\x12\"\n\x1arobot_configured_for_lidar\x18\x02 \x01(\x08\"\xb5\t\n\x17SetLocalizationResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x34\n\x10lease_use_result\x18\x02 \x01(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12\x44\n\x06status\x18\x03 \x01(\x0e\x32\x34.bosdyn.api.graph_nav.SetLocalizationResponse.Status\x12\x14\n\x0c\x65rror_report\x18\x04 \x01(\t\x12\x38\n\x0clocalization\x18\x05 \x01(\x0b\x32\".bosdyn.api.graph_nav.Localization\x12]\n\x13suspected_ambiguity\x18\x07 \x01(\x0b\x32@.bosdyn.api.graph_nav.SetLocalizationResponse.SuspectedAmbiguity\x12\x36\n\x0eimpaired_state\x18\x08 \x01(\x0b\x32\x1e.bosdyn.api.RobotImpairedState\x12\x46\n\rsensor_status\x18\t \x01(\x0b\x32/.bosdyn.api.graph_nav.SensorCompatibilityStatus\x12^\n\x14quality_check_result\x18\n \x01(\x0e\x32@.bosdyn.api.graph_nav.SetLocalizationResponse.QualityCheckResult\x1aQ\n\x12SuspectedAmbiguity\x12;\n\x1e\x61lternate_robot_tform_waypoint\x18\x01 \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\"\xd3\x02\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x19\n\x15STATUS_ROBOT_IMPAIRED\x10\x02\x12\x1b\n\x17STATUS_UNKNOWN_WAYPOINT\x10\x03\x12\x12\n\x0eSTATUS_ABORTED\x10\x04\x12\x11\n\rSTATUS_FAILED\x10\x05\x12 \n\x1cSTATUS_FIDUCIAL_TOO_FAR_AWAY\x10\x06\x12\x1b\n\x17STATUS_FIDUCIAL_TOO_OLD\x10\x07\x12\x1f\n\x1bSTATUS_NO_MATCHING_FIDUCIAL\x10\x08\x12\"\n\x1eSTATUS_FIDUCIAL_POSE_UNCERTAIN\x10\t\x12\x1f\n\x1bSTATUS_INCOMPATIBLE_SENSORS\x10\n\x12\"\n\x1eSTATUS_VISUAL_ALIGNMENT_FAILED\x10\x0b\"\xb9\x01\n\x12QualityCheckResult\x12\x19\n\x15QUALITY_CHECK_UNKNOWN\x10\x00\x12\x19\n\x15QUALITY_CHECK_SUCCESS\x10\x01\x12(\n$QUALITY_CHECK_POOR_POINT_CLOUD_MATCH\x10\x02\x12(\n$QUALITY_CHECK_POOR_GRAVITY_ALIGNMENT\x10\x03\x12\x19\n\x15QUALITY_CHECK_SKIPPED\x10\x04\"\x10\n\x0eRouteGenParams\"\x99\x05\n\x0cTravelParams\x12\x14\n\x0cmax_distance\x18\x01 \x01(\x01\x12\x0f\n\x07max_yaw\x18\x02 \x01(\x01\x12\x34\n\x0evelocity_limit\x18\x03 \x01(\x0b\x32\x1c.bosdyn.api.SE2VelocityLimit\x12\x18\n\x10ignore_final_yaw\x18\x04 \x01(\x08\x12]\n\x19\x66\x65\x61ture_quality_tolerance\x18\x05 \x01(\x0e\x32:.bosdyn.api.graph_nav.TravelParams.FeatureQualityTolerance\x12$\n\x1c\x64isable_directed_exploration\x18\x06 \x01(\x08\x12\'\n\x1f\x64isable_alternate_route_finding\x18\x08 \x01(\x08\x12U\n\x13path_following_mode\x18\t \x01(\x0e\x32\x38.bosdyn.api.graph_nav.Edge.Annotations.PathFollowingMode\x12\x39\n\x16\x62locked_path_wait_time\x18\n \x01(\x0b\x32\x19.google.protobuf.Duration\x12^\n\x13ground_clutter_mode\x18\x0b \x01(\x0e\x32\x41.bosdyn.api.graph_nav.Edge.Annotations.GroundClutterAvoidanceMode\"r\n\x17\x46\x65\x61tureQualityTolerance\x12\x15\n\x11TOLERANCE_UNKNOWN\x10\x00\x12\x15\n\x11TOLERANCE_DEFAULT\x10\x01\x12)\n%TOLERANCE_IGNORE_POOR_FEATURE_QUALITY\x10\x02\"\x92\x02\n\x18ModifyNavigationResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x35\n\x11lease_use_results\x18\x02 \x03(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12\x45\n\x06status\x18\x03 \x01(\x0e\x32\x35.bosdyn.api.graph_nav.ModifyNavigationResponse.Status\"L\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1f\n\x1bSTATUS_UNRECOGNIZED_COMMAND\x10\x02\"\xf9\x03\n\x11NavigateToRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12!\n\x06leases\x18\x02 \x03(\x0b\x32\x11.bosdyn.api.Lease\x12\x1f\n\x17\x64\x65stination_waypoint_id\x18\x03 \x01(\t\x12:\n\x0croute_params\x18\x04 \x01(\x0b\x32$.bosdyn.api.graph_nav.RouteGenParams\x12\x39\n\rtravel_params\x18\x05 \x01(\x0b\x32\".bosdyn.api.graph_nav.TravelParams\x12,\n\x08\x65nd_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10\x63lock_identifier\x18\x07 \x01(\t\x12\x41\n$destination_waypoint_tform_body_goal\x18\x08 \x01(\x0b\x32\x13.bosdyn.api.SE2Pose\x12\x12\n\ncommand_id\x18\t \x01(\r\x12_\n\x16route_blocked_behavior\x18\n \x01(\x0e\x32?.bosdyn.api.graph_nav.RouteFollowingParams.RouteBlockedBehavior\"\x84\x06\n\x12NavigateToResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x35\n\x11lease_use_results\x18\x02 \x03(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12?\n\x06status\x18\x03 \x01(\x0e\x32/.bosdyn.api.graph_nav.NavigateToResponse.Status\x12\x36\n\x0eimpaired_state\x18\x06 \x01(\x0b\x32\x1e.bosdyn.api.RobotImpairedState\x12\x12\n\ncommand_id\x18\x04 \x01(\r\x12\x1a\n\x12\x65rror_waypoint_ids\x18\x05 \x03(\t\x12K\n\x13\x61rea_callback_error\x18\n \x01(\x0b\x32..bosdyn.api.graph_nav.AreaCallbackServiceError\"\x94\x03\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x16\n\x12STATUS_NO_TIMESYNC\x10\x02\x12\x12\n\x0eSTATUS_EXPIRED\x10\x03\x12\x16\n\x12STATUS_TOO_DISTANT\x10\x04\x12\x19\n\x15STATUS_ROBOT_IMPAIRED\x10\x05\x12\x14\n\x10STATUS_RECORDING\x10\x06\x12\x1b\n\x17STATUS_UNKNOWN_WAYPOINT\x10\x07\x12\x12\n\x0eSTATUS_NO_PATH\x10\x08\x12\x19\n\x15STATUS_FEATURE_DESERT\x10\n\x12\x0f\n\x0bSTATUS_LOST\x10\x0b\x12\x1f\n\x1bSTATUS_NOT_LOCALIZED_TO_MAP\x10\r\x12!\n\x1dSTATUS_COULD_NOT_UPDATE_ROUTE\x10\x0c\x12\x10\n\x0cSTATUS_STUCK\x10\x0e\x12\x1f\n\x1bSTATUS_UNRECOGNIZED_COMMAND\x10\x0f\x12\x1e\n\x1aSTATUS_AREA_CALLBACK_ERROR\x10\x10\"\xf7\x04\n\x14RouteFollowingParams\x12W\n\x10new_cmd_behavior\x18\x01 \x01(\x0e\x32=.bosdyn.api.graph_nav.RouteFollowingParams.StartRouteBehavior\x12X\n\x15\x65xisting_cmd_behavior\x18\x02 \x01(\x0e\x32\x39.bosdyn.api.graph_nav.RouteFollowingParams.ResumeBehavior\x12_\n\x16route_blocked_behavior\x18\x03 \x01(\x0e\x32?.bosdyn.api.graph_nav.RouteFollowingParams.RouteBlockedBehavior\"u\n\x12StartRouteBehavior\x12\x11\n\rSTART_UNKNOWN\x10\x00\x12\x14\n\x10START_GOTO_START\x10\x01\x12\x14\n\x10START_GOTO_ROUTE\x10\x02\x12 \n\x1cSTART_FAIL_WHEN_NOT_ON_ROUTE\x10\x03\"n\n\x0eResumeBehavior\x12\x12\n\x0eRESUME_UNKNOWN\x10\x00\x12%\n!RESUME_RETURN_TO_UNFINISHED_ROUTE\x10\x01\x12!\n\x1dRESUME_FAIL_WHEN_NOT_ON_ROUTE\x10\x02\"d\n\x14RouteBlockedBehavior\x12\x19\n\x15ROUTE_BLOCKED_UNKNOWN\x10\x00\x12\x19\n\x15ROUTE_BLOCKED_REROUTE\x10\x01\x12\x16\n\x12ROUTE_BLOCKED_FAIL\x10\x02\"\xb3\x03\n\x14NavigateRouteRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12!\n\x06leases\x18\x02 \x03(\x0b\x32\x11.bosdyn.api.Lease\x12*\n\x05route\x18\x03 \x01(\x0b\x32\x1b.bosdyn.api.graph_nav.Route\x12G\n\x13route_follow_params\x18\t \x01(\x0b\x32*.bosdyn.api.graph_nav.RouteFollowingParams\x12\x39\n\rtravel_params\x18\x04 \x01(\x0b\x32\".bosdyn.api.graph_nav.TravelParams\x12,\n\x08\x65nd_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10\x63lock_identifier\x18\x06 \x01(\t\x12\x41\n$destination_waypoint_tform_body_goal\x18\x07 \x01(\x0b\x32\x13.bosdyn.api.SE2Pose\x12\x12\n\ncommand_id\x18\x08 \x01(\r\"\xa0\x07\n\x15NavigateRouteResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x35\n\x11lease_use_results\x18\x02 \x03(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12\x42\n\x06status\x18\x03 \x01(\x0e\x32\x32.bosdyn.api.graph_nav.NavigateRouteResponse.Status\x12\x36\n\x0eimpaired_state\x18\x07 \x01(\x0b\x32\x1e.bosdyn.api.RobotImpairedState\x12\x12\n\ncommand_id\x18\x04 \x01(\r\x12\x1a\n\x12\x65rror_waypoint_ids\x18\x05 \x03(\t\x12\x35\n\x0e\x65rror_edge_ids\x18\x06 \x03(\x0b\x32\x1d.bosdyn.api.graph_nav.Edge.Id\x12K\n\x13\x61rea_callback_error\x18\x08 \x01(\x0b\x32..bosdyn.api.graph_nav.AreaCallbackServiceError\"\xf3\x03\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x16\n\x12STATUS_NO_TIMESYNC\x10\x02\x12\x12\n\x0eSTATUS_EXPIRED\x10\x03\x12\x16\n\x12STATUS_TOO_DISTANT\x10\x04\x12\x19\n\x15STATUS_ROBOT_IMPAIRED\x10\x05\x12\x14\n\x10STATUS_RECORDING\x10\x06\x12!\n\x1dSTATUS_UNKNOWN_ROUTE_ELEMENTS\x10\x08\x12\x17\n\x13STATUS_INVALID_EDGE\x10\t\x12\x12\n\x0eSTATUS_NO_PATH\x10\x14\x12\x1b\n\x17STATUS_CONSTRAINT_FAULT\x10\x0b\x12\x19\n\x15STATUS_FEATURE_DESERT\x10\r\x12\x0f\n\x0bSTATUS_LOST\x10\x0e\x12!\n\x1dSTATUS_NOT_LOCALIZED_TO_ROUTE\x10\x10\x12\x1f\n\x1bSTATUS_NOT_LOCALIZED_TO_MAP\x10\x13\x12!\n\x1dSTATUS_COULD_NOT_UPDATE_ROUTE\x10\x0f\x12\x10\n\x0cSTATUS_STUCK\x10\x11\x12\x1f\n\x1bSTATUS_UNRECOGNIZED_COMMAND\x10\x12\x12\x1e\n\x1aSTATUS_AREA_CALLBACK_ERROR\x10\x15\"\xad\x03\n\x17NavigateToAnchorRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12!\n\x06leases\x18\x02 \x03(\x0b\x32\x11.bosdyn.api.Lease\x12,\n\x0fseed_tform_goal\x18\x03 \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\x12\x43\n)goal_waypoint_rt_seed_ewrt_seed_tolerance\x18\x04 \x01(\x0b\x32\x10.bosdyn.api.Vec3\x12:\n\x0croute_params\x18\x06 \x01(\x0b\x32$.bosdyn.api.graph_nav.RouteGenParams\x12\x39\n\rtravel_params\x18\x07 \x01(\x0b\x32\".bosdyn.api.graph_nav.TravelParams\x12,\n\x08\x65nd_time\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x18\n\x10\x63lock_identifier\x18\t \x01(\t\x12\x12\n\ncommand_id\x18\n \x01(\r\"\xa5\x06\n\x18NavigateToAnchorResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x35\n\x11lease_use_results\x18\x02 \x03(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12\x45\n\x06status\x18\x03 \x01(\x0e\x32\x35.bosdyn.api.graph_nav.NavigateToAnchorResponse.Status\x12\x36\n\x0eimpaired_state\x18\x06 \x01(\x0b\x32\x1e.bosdyn.api.RobotImpairedState\x12\x12\n\ncommand_id\x18\x04 \x01(\r\x12\x1a\n\x12\x65rror_waypoint_ids\x18\x05 \x03(\t\x12K\n\x13\x61rea_callback_error\x18\x07 \x01(\x0b\x32..bosdyn.api.graph_nav.AreaCallbackServiceError\"\xa9\x03\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x16\n\x12STATUS_NO_TIMESYNC\x10\x02\x12\x12\n\x0eSTATUS_EXPIRED\x10\x03\x12\x16\n\x12STATUS_TOO_DISTANT\x10\x04\x12\x19\n\x15STATUS_ROBOT_IMPAIRED\x10\x05\x12\x14\n\x10STATUS_RECORDING\x10\x06\x12\x17\n\x13STATUS_NO_ANCHORING\x10\x07\x12\x12\n\x0eSTATUS_NO_PATH\x10\x08\x12\x19\n\x15STATUS_FEATURE_DESERT\x10\n\x12\x0f\n\x0bSTATUS_LOST\x10\x0b\x12\x1f\n\x1bSTATUS_NOT_LOCALIZED_TO_MAP\x10\r\x12!\n\x1dSTATUS_COULD_NOT_UPDATE_ROUTE\x10\x0c\x12\x10\n\x0cSTATUS_STUCK\x10\x0e\x12\x1f\n\x1bSTATUS_UNRECOGNIZED_COMMAND\x10\x0f\x12\x17\n\x13STATUS_INVALID_POSE\x10\x10\x12\x1e\n\x1aSTATUS_AREA_CALLBACK_ERROR\x10\x11\"Z\n\x19NavigationFeedbackRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x12\n\ncommand_id\x18\x02 \x01(\r\"\xc1\x13\n\x1aNavigationFeedbackResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12G\n\x06status\x18\x02 \x01(\x0e\x32\x37.bosdyn.api.graph_nav.NavigationFeedbackResponse.Status\x12\x36\n\x0eimpaired_state\x18\x06 \x01(\x0b\x32\x1e.bosdyn.api.RobotImpairedState\x12\x66\n\x14\x61rea_callback_errors\x18\t \x03(\x0b\x32H.bosdyn.api.graph_nav.NavigationFeedbackResponse.AreaCallbackErrorsEntry\x12\x34\n\x0fremaining_route\x18\x03 \x01(\x0b\x32\x1b.bosdyn.api.graph_nav.Route\x12\x12\n\ncommand_id\x18\x04 \x01(\r\x12/\n\x12last_ko_tform_goal\x18\x05 \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\x12Z\n\x14\x62ody_movement_status\x18\x07 \x01(\x0e\x32<.bosdyn.api.SE2TrajectoryCommand.Feedback.BodyMovementStatus\x12U\n\x13path_following_mode\x18\x08 \x01(\x0e\x32\x38.bosdyn.api.graph_nav.Edge.Annotations.PathFollowingMode\x12p\n\x19\x61\x63tive_region_information\x18\n \x03(\x0b\x32M.bosdyn.api.graph_nav.NavigationFeedbackResponse.ActiveRegionInformationEntry\x12\x66\n\x16route_following_status\x18\xe8\x07 \x01(\x0e\x32\x45.bosdyn.api.graph_nav.NavigationFeedbackResponse.RouteFollowingStatus\x12Y\n\x0f\x62lockage_status\x18\xe9\x07 \x01(\x0e\x32?.bosdyn.api.graph_nav.NavigationFeedbackResponse.BlockageStatus\x12R\n\x0cstuck_reason\x18\x0b \x01(\x0e\x32<.bosdyn.api.graph_nav.NavigationFeedbackResponse.StuckReason\x1a\x62\n\x17\x41reaCallbackErrorsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x36\n\x05value\x18\x02 \x01(\x0b\x32\'.bosdyn.api.graph_nav.AreaCallbackError:\x02\x38\x01\x1a\x88\x01\n\x1c\x41\x63tiveRegionInformationEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12W\n\x05value\x18\x02 \x01(\x0b\x32H.bosdyn.api.graph_nav.NavigationFeedbackResponse.ActiveRegionInformation:\x02\x38\x01\x1a\xad\x02\n\x17\x41\x63tiveRegionInformation\x12\x13\n\x0b\x64\x65scription\x18\x01 \x01(\t\x12\x14\n\x0cservice_name\x18\x02 \x01(\t\x12r\n\rregion_status\x18\x03 \x01(\x0e\x32[.bosdyn.api.graph_nav.NavigationFeedbackResponse.ActiveRegionInformation.AreaCallbackStatus\"s\n\x12\x41reaCallbackStatus\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x15\n\x11STATUS_NAVIGATING\x10\x01\x12\x12\n\x0eSTATUS_WAITING\x10\x02\x12\x1e\n\x1aSTATUS_CALLBACK_IN_CONTROL\x10\x03\"\xf5\x02\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x1a\n\x16STATUS_FOLLOWING_ROUTE\x10\x01\x12\x17\n\x13STATUS_REACHED_GOAL\x10\x02\x12\x13\n\x0fSTATUS_NO_ROUTE\x10\x03\x12\x1a\n\x16STATUS_NO_LOCALIZATION\x10\x04\x12\x0f\n\x0bSTATUS_LOST\x10\x05\x12\x10\n\x0cSTATUS_STUCK\x10\x06\x12\x1c\n\x18STATUS_COMMAND_TIMED_OUT\x10\x07\x12\x19\n\x15STATUS_ROBOT_IMPAIRED\x10\x08\x12\x1b\n\x17STATUS_CONSTRAINT_FAULT\x10\x0b\x12\x1d\n\x19STATUS_COMMAND_OVERRIDDEN\x10\x0c\x12!\n\x1dSTATUS_NOT_LOCALIZED_TO_ROUTE\x10\r\x12\x16\n\x12STATUS_LEASE_ERROR\x10\x0e\x12\x1e\n\x1aSTATUS_AREA_CALLBACK_ERROR\x10\x0f\"\xf1\x01\n\x14RouteFollowingStatus\x12\"\n\x1eROUTE_FOLLOWING_STATUS_UNKNOWN\x10\x00\x12*\n&ROUTE_FOLLOWING_STATUS_FOLLOWING_ROUTE\x10\x01\x12-\n)ROUTE_FOLLOWING_STATUS_RETURNING_TO_ROUTE\x10\x02\x12\x34\n0ROUTE_FOLLOWING_STATUS_FOLLOWING_ALTERNATE_ROUTE\x10\x03\x12$\n ROUTE_FOLLOWING_STATUS_EXPLORING\x10\x04\"\x98\x01\n\x0e\x42lockageStatus\x12\x1b\n\x17\x42LOCKAGE_STATUS_UNKNOWN\x10\x00\x12\x1f\n\x1b\x42LOCKAGE_STATUS_ROUTE_CLEAR\x10\x01\x12-\n)BLOCKAGE_STATUS_ROUTE_BLOCKED_TEMPORARILY\x10\x02\x12\x19\n\x15\x42LOCKAGE_STATUS_STUCK\x10\x03\"\xb0\x01\n\x0bStuckReason\x12\x18\n\x14STUCK_REASON_UNKNOWN\x10\x00\x12\x19\n\x15STUCK_REASON_OBSTACLE\x10\x01\x12&\n\"STUCK_REASON_AREA_CALLBACK_BLOCKED\x10\x02\x12%\n!STUCK_REASON_AREA_CALLBACK_FAILED\x10\x03\x12\x1d\n\x19STUCK_REASON_GOAL_BLOCKED\x10\x04\"\xa8\x02\n\x1bGetLocalizationStateRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x13\n\x0bwaypoint_id\x18\x08 \x01(\t\x12 \n\x18request_live_point_cloud\x18\x02 \x01(\x08\x12\x1b\n\x13request_live_images\x18\x03 \x01(\x08\x12!\n\x19request_live_terrain_maps\x18\x04 \x01(\x08\x12\"\n\x1arequest_live_world_objects\x18\x05 \x01(\x08\x12 \n\x18request_live_robot_state\x18\x06 \x01(\x08\x12!\n\x19\x63ompress_live_point_cloud\x18\x07 \x01(\x08\"]\n\x16RemotePointCloudStatus\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x1b\n\x13\x65xists_in_directory\x18\x02 \x01(\x08\x12\x10\n\x08has_data\x18\x03 \x01(\x08\"$\n\x11LostDetectorState\x12\x0f\n\x07is_lost\x18\x01 \x01(\x08\"\x86\x03\n\x1cGetLocalizationStateResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x38\n\x0clocalization\x18\x02 \x01(\x0b\x32\".bosdyn.api.graph_nav.Localization\x12\x34\n\x10robot_kinematics\x18\x04 \x01(\x0b\x32\x1a.bosdyn.api.KinematicState\x12I\n\x13remote_cloud_status\x18\x05 \x03(\x0b\x32,.bosdyn.api.graph_nav.RemotePointCloudStatus\x12\x39\n\tlive_data\x18\x06 \x01(\x0b\x32&.bosdyn.api.graph_nav.WaypointSnapshot\x12\x44\n\x13lost_detector_state\x18\x07 \x01(\x0b\x32\'.bosdyn.api.graph_nav.LostDetectorState\"`\n\x11\x43learGraphRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12 \n\x05lease\x18\x02 \x01(\x0b\x32\x11.bosdyn.api.Lease\"\xfa\x01\n\x12\x43learGraphResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x34\n\x10lease_use_result\x18\x02 \x01(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12?\n\x06status\x18\x03 \x01(\x0e\x32/.bosdyn.api.graph_nav.ClearGraphResponse.Status\"A\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x14\n\x10STATUS_RECORDING\x10\x02\"\xda\x01\n\x12UploadGraphRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12*\n\x05graph\x18\x02 \x01(\x0b\x32\x1b.bosdyn.api.graph_nav.Graph\x12 \n\x05lease\x18\x03 \x01(\x0b\x32\x11.bosdyn.api.Lease\x12\x1e\n\x16generate_new_anchoring\x18\x04 \x01(\x08\x12+\n#treat_validation_warnings_as_errors\x18\x05 \x01(\x08\"\xa3\x0b\n\x13UploadGraphResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12@\n\x06status\x18\x08 \x01(\x0e\x32\x30.bosdyn.api.graph_nav.UploadGraphResponse.Status\x12\x34\n\x10lease_use_result\x18\x02 \x01(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12$\n\x1cloaded_waypoint_snapshot_ids\x18\x03 \x03(\t\x12%\n\x1dunknown_waypoint_snapshot_ids\x18\x04 \x03(\t\x12 \n\x18loaded_edge_snapshot_ids\x18\x05 \x03(\t\x12!\n\x19unknown_edge_snapshot_ids\x18\x06 \x03(\t\x12\x36\n\x0elicense_status\x18\x07 \x01(\x0e\x32\x1e.bosdyn.api.LicenseInfo.Status\x12\x46\n\rsensor_status\x18\t \x01(\x0b\x32/.bosdyn.api.graph_nav.SensorCompatibilityStatus\x12K\n\x13\x61rea_callback_error\x18\n \x01(\x0b\x32..bosdyn.api.graph_nav.AreaCallbackServiceError\x12\x31\n\tmap_stats\x18\x0b \x01(\x0b\x32\x1e.bosdyn.api.graph_nav.MapStats\x12U\n\x11validation_status\x18\x0c \x01(\x0b\x32:.bosdyn.api.graph_nav.UploadGraphResponse.ValidationStatus\x1a\xd3\x04\n\x10ValidationStatus\x12%\n\x1dmissing_waypoint_ids_in_edges\x18\x01 \x03(\t\x12\'\n\x1fmissing_waypoint_ids_in_anchors\x18\x02 \x03(\t\x12\x41\n\x1a\x65\x64ge_ids_invalid_transform\x18\x03 \x03(\x0b\x32\x1d.bosdyn.api.graph_nav.Edge.Id\x12*\n\"waypoint_anchors_invalid_transform\x18\x04 \x03(\t\x12(\n object_anchors_invalid_transform\x18\x05 \x03(\t\x12\x1e\n\x16\x64uplicate_waypoint_ids\x18\x06 \x03(\t\x12%\n\x1d\x64uplicate_waypoint_anchor_ids\x18\x07 \x03(\t\x12#\n\x1b\x64uplicate_object_anchor_ids\x18\x08 \x03(\t\x12\x39\n\x12\x64uplicate_edge_ids\x18\t \x03(\x0b\x32\x1d.bosdyn.api.graph_nav.Edge.Id\x12\'\n\x1finvalid_waypoint_ids_self_edges\x18\n \x03(\t\x12\x1e\n\x16has_empty_waypoint_ids\x18\x0b \x01(\x08\x12\x1a\n\x12has_empty_edge_ids\x18\x0c \x01(\x08\x12%\n\x1dhas_empty_waypoint_anchor_ids\x18\r \x01(\x08\x12#\n\x1bhas_empty_object_anchor_ids\x18\x0e \x01(\x08\"\xa8\x01\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12 \n\x1cSTATUS_MAP_TOO_LARGE_LICENSE\x10\x03\x12\x18\n\x14STATUS_INVALID_GRAPH\x10\x04\x12\x1f\n\x1bSTATUS_INCOMPATIBLE_SENSORS\x10\x05\x12\x1e\n\x1aSTATUS_AREA_CALLBACK_ERROR\x10\x06\"A\n\x14\x44ownloadGraphRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"o\n\x15\x44ownloadGraphResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12*\n\x05graph\x18\x02 \x01(\x0b\x32\x1b.bosdyn.api.graph_nav.Graph\"\x92\x01\n\x1dUploadWaypointSnapshotRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12$\n\x05\x63hunk\x18\x03 \x01(\x0b\x32\x15.bosdyn.api.DataChunk\x12 \n\x05lease\x18\x04 \x01(\x0b\x32\x11.bosdyn.api.Lease\"\x98\x03\n\x1eUploadWaypointSnapshotResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x34\n\x10lease_use_result\x18\x02 \x01(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12K\n\x06status\x18\x03 \x01(\x0e\x32;.bosdyn.api.graph_nav.UploadWaypointSnapshotResponse.Status\x12\x46\n\rsensor_status\x18\x04 \x01(\x0b\x32/.bosdyn.api.graph_nav.SensorCompatibilityStatus\x12\x31\n\tmap_stats\x18\x05 \x01(\x0b\x32\x1e.bosdyn.api.graph_nav.MapStats\"L\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1f\n\x1bSTATUS_INCOMPATIBLE_SENSORS\x10\x02\"\x8e\x01\n\x19UploadEdgeSnapshotRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12$\n\x05\x63hunk\x18\x04 \x01(\x0b\x32\x15.bosdyn.api.DataChunk\x12 \n\x05lease\x18\x05 \x01(\x0b\x32\x11.bosdyn.api.Lease\"\xb1\x01\n\x1aUploadEdgeSnapshotResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x34\n\x10lease_use_result\x18\x02 \x01(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12\x31\n\tmap_stats\x18\x03 \x01(\x0b\x32\x1e.bosdyn.api.graph_nav.MapStats\"\xc6\x01\n\x1f\x44ownloadWaypointSnapshotRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x1c\n\x14waypoint_snapshot_id\x18\x02 \x01(\t\x12\x17\n\x0f\x64ownload_images\x18\x03 \x01(\x08\x12\x1c\n\x14\x63ompress_point_cloud\x18\x04 \x01(\x08\x12#\n\x1b\x64o_not_download_point_cloud\x18\x05 \x01(\x08\"\xb2\x02\n DownloadWaypointSnapshotResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12M\n\x06status\x18\x02 \x01(\x0e\x32=.bosdyn.api.graph_nav.DownloadWaypointSnapshotResponse.Status\x12\x1c\n\x14waypoint_snapshot_id\x18\x04 \x01(\t\x12$\n\x05\x63hunk\x18\x05 \x01(\x0b\x32\x15.bosdyn.api.DataChunk\"O\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\"\n\x1eSTATUS_SNAPSHOT_DOES_NOT_EXIST\x10\x02\"b\n\x1b\x44ownloadEdgeSnapshotRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x18\n\x10\x65\x64ge_snapshot_id\x18\x02 \x01(\t\"\xa6\x02\n\x1c\x44ownloadEdgeSnapshotResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12I\n\x06status\x18\x02 \x01(\x0e\x32\x39.bosdyn.api.graph_nav.DownloadEdgeSnapshotResponse.Status\x12\x18\n\x10\x65\x64ge_snapshot_id\x18\x04 \x01(\t\x12$\n\x05\x63hunk\x18\x05 \x01(\x0b\x32\x15.bosdyn.api.DataChunk\"O\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\"\n\x1eSTATUS_SNAPSHOT_DOES_NOT_EXIST\x10\x02\"h\n\x18\x41reaCallbackServiceError\x12\x18\n\x10missing_services\x18\x01 \x03(\t\x12\x32\n\x10\x66\x61ulted_services\x18\x02 \x03(\x0b\x32\x18.bosdyn.api.ServiceFault\"A\n\x14ValidateGraphRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"\x8a\x03\n\x15ValidateGraphResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x42\n\x06status\x18\x02 \x01(\x0e\x32\x32.bosdyn.api.graph_nav.ValidateGraphResponse.Status\x12\x46\n\rsensor_status\x18\x03 \x01(\x0b\x32/.bosdyn.api.graph_nav.SensorCompatibilityStatus\x12K\n\x13\x61rea_callback_error\x18\x04 \x01(\x0b\x32..bosdyn.api.graph_nav.AreaCallbackServiceError\"l\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1f\n\x1bSTATUS_INCOMPATIBLE_SENSORS\x10\x05\x12\x1e\n\x1aSTATUS_AREA_CALLBACK_ERROR\x10\x06\x42\x0f\x42\rGraphNavProtob\x06proto3')
 
 
 
 _VISUALREFINEMENTOPTIONS = DESCRIPTOR.message_types_by_name['VisualRefinementOptions']
 _SETLOCALIZATIONREQUEST = DESCRIPTOR.message_types_by_name['SetLocalizationRequest']
 _SENSORCOMPATIBILITYSTATUS = DESCRIPTOR.message_types_by_name['SensorCompatibilityStatus']
 _SETLOCALIZATIONRESPONSE = DESCRIPTOR.message_types_by_name['SetLocalizationResponse']
 _SETLOCALIZATIONRESPONSE_SUSPECTEDAMBIGUITY = _SETLOCALIZATIONRESPONSE.nested_types_by_name['SuspectedAmbiguity']
 _ROUTEGENPARAMS = DESCRIPTOR.message_types_by_name['RouteGenParams']
 _TRAVELPARAMS = DESCRIPTOR.message_types_by_name['TravelParams']
+_MODIFYNAVIGATIONRESPONSE = DESCRIPTOR.message_types_by_name['ModifyNavigationResponse']
 _NAVIGATETOREQUEST = DESCRIPTOR.message_types_by_name['NavigateToRequest']
 _NAVIGATETORESPONSE = DESCRIPTOR.message_types_by_name['NavigateToResponse']
 _ROUTEFOLLOWINGPARAMS = DESCRIPTOR.message_types_by_name['RouteFollowingParams']
 _NAVIGATEROUTEREQUEST = DESCRIPTOR.message_types_by_name['NavigateRouteRequest']
 _NAVIGATEROUTERESPONSE = DESCRIPTOR.message_types_by_name['NavigateRouteResponse']
 _NAVIGATETOANCHORREQUEST = DESCRIPTOR.message_types_by_name['NavigateToAnchorRequest']
 _NAVIGATETOANCHORRESPONSE = DESCRIPTOR.message_types_by_name['NavigateToAnchorResponse']
@@ -53,14 +55,15 @@
 _REMOTEPOINTCLOUDSTATUS = DESCRIPTOR.message_types_by_name['RemotePointCloudStatus']
 _LOSTDETECTORSTATE = DESCRIPTOR.message_types_by_name['LostDetectorState']
 _GETLOCALIZATIONSTATERESPONSE = DESCRIPTOR.message_types_by_name['GetLocalizationStateResponse']
 _CLEARGRAPHREQUEST = DESCRIPTOR.message_types_by_name['ClearGraphRequest']
 _CLEARGRAPHRESPONSE = DESCRIPTOR.message_types_by_name['ClearGraphResponse']
 _UPLOADGRAPHREQUEST = DESCRIPTOR.message_types_by_name['UploadGraphRequest']
 _UPLOADGRAPHRESPONSE = DESCRIPTOR.message_types_by_name['UploadGraphResponse']
+_UPLOADGRAPHRESPONSE_VALIDATIONSTATUS = _UPLOADGRAPHRESPONSE.nested_types_by_name['ValidationStatus']
 _DOWNLOADGRAPHREQUEST = DESCRIPTOR.message_types_by_name['DownloadGraphRequest']
 _DOWNLOADGRAPHRESPONSE = DESCRIPTOR.message_types_by_name['DownloadGraphResponse']
 _UPLOADWAYPOINTSNAPSHOTREQUEST = DESCRIPTOR.message_types_by_name['UploadWaypointSnapshotRequest']
 _UPLOADWAYPOINTSNAPSHOTRESPONSE = DESCRIPTOR.message_types_by_name['UploadWaypointSnapshotResponse']
 _UPLOADEDGESNAPSHOTREQUEST = DESCRIPTOR.message_types_by_name['UploadEdgeSnapshotRequest']
 _UPLOADEDGESNAPSHOTRESPONSE = DESCRIPTOR.message_types_by_name['UploadEdgeSnapshotResponse']
 _DOWNLOADWAYPOINTSNAPSHOTREQUEST = DESCRIPTOR.message_types_by_name['DownloadWaypointSnapshotRequest']
@@ -68,25 +71,28 @@
 _DOWNLOADEDGESNAPSHOTREQUEST = DESCRIPTOR.message_types_by_name['DownloadEdgeSnapshotRequest']
 _DOWNLOADEDGESNAPSHOTRESPONSE = DESCRIPTOR.message_types_by_name['DownloadEdgeSnapshotResponse']
 _AREACALLBACKSERVICEERROR = DESCRIPTOR.message_types_by_name['AreaCallbackServiceError']
 _VALIDATEGRAPHREQUEST = DESCRIPTOR.message_types_by_name['ValidateGraphRequest']
 _VALIDATEGRAPHRESPONSE = DESCRIPTOR.message_types_by_name['ValidateGraphResponse']
 _SETLOCALIZATIONREQUEST_FIDUCIALINIT = _SETLOCALIZATIONREQUEST.enum_types_by_name['FiducialInit']
 _SETLOCALIZATIONRESPONSE_STATUS = _SETLOCALIZATIONRESPONSE.enum_types_by_name['Status']
+_SETLOCALIZATIONRESPONSE_QUALITYCHECKRESULT = _SETLOCALIZATIONRESPONSE.enum_types_by_name['QualityCheckResult']
 _TRAVELPARAMS_FEATUREQUALITYTOLERANCE = _TRAVELPARAMS.enum_types_by_name['FeatureQualityTolerance']
+_MODIFYNAVIGATIONRESPONSE_STATUS = _MODIFYNAVIGATIONRESPONSE.enum_types_by_name['Status']
 _NAVIGATETORESPONSE_STATUS = _NAVIGATETORESPONSE.enum_types_by_name['Status']
 _ROUTEFOLLOWINGPARAMS_STARTROUTEBEHAVIOR = _ROUTEFOLLOWINGPARAMS.enum_types_by_name['StartRouteBehavior']
 _ROUTEFOLLOWINGPARAMS_RESUMEBEHAVIOR = _ROUTEFOLLOWINGPARAMS.enum_types_by_name['ResumeBehavior']
 _ROUTEFOLLOWINGPARAMS_ROUTEBLOCKEDBEHAVIOR = _ROUTEFOLLOWINGPARAMS.enum_types_by_name['RouteBlockedBehavior']
 _NAVIGATEROUTERESPONSE_STATUS = _NAVIGATEROUTERESPONSE.enum_types_by_name['Status']
 _NAVIGATETOANCHORRESPONSE_STATUS = _NAVIGATETOANCHORRESPONSE.enum_types_by_name['Status']
 _NAVIGATIONFEEDBACKRESPONSE_ACTIVEREGIONINFORMATION_AREACALLBACKSTATUS = _NAVIGATIONFEEDBACKRESPONSE_ACTIVEREGIONINFORMATION.enum_types_by_name['AreaCallbackStatus']
 _NAVIGATIONFEEDBACKRESPONSE_STATUS = _NAVIGATIONFEEDBACKRESPONSE.enum_types_by_name['Status']
 _NAVIGATIONFEEDBACKRESPONSE_ROUTEFOLLOWINGSTATUS = _NAVIGATIONFEEDBACKRESPONSE.enum_types_by_name['RouteFollowingStatus']
 _NAVIGATIONFEEDBACKRESPONSE_BLOCKAGESTATUS = _NAVIGATIONFEEDBACKRESPONSE.enum_types_by_name['BlockageStatus']
+_NAVIGATIONFEEDBACKRESPONSE_STUCKREASON = _NAVIGATIONFEEDBACKRESPONSE.enum_types_by_name['StuckReason']
 _CLEARGRAPHRESPONSE_STATUS = _CLEARGRAPHRESPONSE.enum_types_by_name['Status']
 _UPLOADGRAPHRESPONSE_STATUS = _UPLOADGRAPHRESPONSE.enum_types_by_name['Status']
 _UPLOADWAYPOINTSNAPSHOTRESPONSE_STATUS = _UPLOADWAYPOINTSNAPSHOTRESPONSE.enum_types_by_name['Status']
 _DOWNLOADWAYPOINTSNAPSHOTRESPONSE_STATUS = _DOWNLOADWAYPOINTSNAPSHOTRESPONSE.enum_types_by_name['Status']
 _DOWNLOADEDGESNAPSHOTRESPONSE_STATUS = _DOWNLOADEDGESNAPSHOTRESPONSE.enum_types_by_name['Status']
 _VALIDATEGRAPHRESPONSE_STATUS = _VALIDATEGRAPHRESPONSE.enum_types_by_name['Status']
 VisualRefinementOptions = _reflection.GeneratedProtocolMessageType('VisualRefinementOptions', (_message.Message,), {
@@ -135,14 +141,21 @@
 TravelParams = _reflection.GeneratedProtocolMessageType('TravelParams', (_message.Message,), {
   'DESCRIPTOR' : _TRAVELPARAMS,
   '__module__' : 'bosdyn.api.graph_nav.graph_nav_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.graph_nav.TravelParams)
   })
 _sym_db.RegisterMessage(TravelParams)
 
+ModifyNavigationResponse = _reflection.GeneratedProtocolMessageType('ModifyNavigationResponse', (_message.Message,), {
+  'DESCRIPTOR' : _MODIFYNAVIGATIONRESPONSE,
+  '__module__' : 'bosdyn.api.graph_nav.graph_nav_pb2'
+  # @@protoc_insertion_point(class_scope:bosdyn.api.graph_nav.ModifyNavigationResponse)
+  })
+_sym_db.RegisterMessage(ModifyNavigationResponse)
+
 NavigateToRequest = _reflection.GeneratedProtocolMessageType('NavigateToRequest', (_message.Message,), {
   'DESCRIPTOR' : _NAVIGATETOREQUEST,
   '__module__' : 'bosdyn.api.graph_nav.graph_nav_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.graph_nav.NavigateToRequest)
   })
 _sym_db.RegisterMessage(NavigateToRequest)
 
@@ -272,19 +285,27 @@
   'DESCRIPTOR' : _UPLOADGRAPHREQUEST,
   '__module__' : 'bosdyn.api.graph_nav.graph_nav_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.graph_nav.UploadGraphRequest)
   })
 _sym_db.RegisterMessage(UploadGraphRequest)
 
 UploadGraphResponse = _reflection.GeneratedProtocolMessageType('UploadGraphResponse', (_message.Message,), {
+
+  'ValidationStatus' : _reflection.GeneratedProtocolMessageType('ValidationStatus', (_message.Message,), {
+    'DESCRIPTOR' : _UPLOADGRAPHRESPONSE_VALIDATIONSTATUS,
+    '__module__' : 'bosdyn.api.graph_nav.graph_nav_pb2'
+    # @@protoc_insertion_point(class_scope:bosdyn.api.graph_nav.UploadGraphResponse.ValidationStatus)
+    })
+  ,
   'DESCRIPTOR' : _UPLOADGRAPHRESPONSE,
   '__module__' : 'bosdyn.api.graph_nav.graph_nav_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.graph_nav.UploadGraphResponse)
   })
 _sym_db.RegisterMessage(UploadGraphResponse)
+_sym_db.RegisterMessage(UploadGraphResponse.ValidationStatus)
 
 DownloadGraphRequest = _reflection.GeneratedProtocolMessageType('DownloadGraphRequest', (_message.Message,), {
   'DESCRIPTOR' : _DOWNLOADGRAPHREQUEST,
   '__module__' : 'bosdyn.api.graph_nav.graph_nav_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.graph_nav.DownloadGraphRequest)
   })
 _sym_db.RegisterMessage(DownloadGraphRequest)
@@ -377,126 +398,136 @@
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'B\rGraphNavProto'
   _NAVIGATIONFEEDBACKRESPONSE_AREACALLBACKERRORSENTRY._options = None
   _NAVIGATIONFEEDBACKRESPONSE_AREACALLBACKERRORSENTRY._serialized_options = b'8\001'
   _NAVIGATIONFEEDBACKRESPONSE_ACTIVEREGIONINFORMATIONENTRY._options = None
   _NAVIGATIONFEEDBACKRESPONSE_ACTIVEREGIONINFORMATIONENTRY._serialized_options = b'8\001'
-  _VISUALREFINEMENTOPTIONS._serialized_start=426
-  _VISUALREFINEMENTOPTIONS._serialized_end=486
-  _SETLOCALIZATIONREQUEST._serialized_start=489
-  _SETLOCALIZATIONREQUEST._serialized_end=1200
-  _SETLOCALIZATIONREQUEST_FIDUCIALINIT._serialized_start=1022
-  _SETLOCALIZATIONREQUEST_FIDUCIALINIT._serialized_end=1186
-  _SENSORCOMPATIBILITYSTATUS._serialized_start=1202
-  _SENSORCOMPATIBILITYSTATUS._serialized_end=1293
-  _SETLOCALIZATIONRESPONSE._serialized_start=1296
-  _SETLOCALIZATIONRESPONSE._serialized_end=2217
-  _SETLOCALIZATIONRESPONSE_SUSPECTEDAMBIGUITY._serialized_start=1794
-  _SETLOCALIZATIONRESPONSE_SUSPECTEDAMBIGUITY._serialized_end=1875
-  _SETLOCALIZATIONRESPONSE_STATUS._serialized_start=1878
-  _SETLOCALIZATIONRESPONSE_STATUS._serialized_end=2217
-  _ROUTEGENPARAMS._serialized_start=2219
-  _ROUTEGENPARAMS._serialized_end=2235
-  _TRAVELPARAMS._serialized_start=2238
-  _TRAVELPARAMS._serialized_end=2903
-  _TRAVELPARAMS_FEATUREQUALITYTOLERANCE._serialized_start=2789
-  _TRAVELPARAMS_FEATUREQUALITYTOLERANCE._serialized_end=2903
-  _NAVIGATETOREQUEST._serialized_start=2906
-  _NAVIGATETOREQUEST._serialized_end=3314
-  _NAVIGATETORESPONSE._serialized_start=3317
-  _NAVIGATETORESPONSE._serialized_end=4089
-  _NAVIGATETORESPONSE_STATUS._serialized_start=3685
-  _NAVIGATETORESPONSE_STATUS._serialized_end=4089
-  _ROUTEFOLLOWINGPARAMS._serialized_start=4092
-  _ROUTEFOLLOWINGPARAMS._serialized_end=4723
-  _ROUTEFOLLOWINGPARAMS_STARTROUTEBEHAVIOR._serialized_start=4392
-  _ROUTEFOLLOWINGPARAMS_STARTROUTEBEHAVIOR._serialized_end=4509
-  _ROUTEFOLLOWINGPARAMS_RESUMEBEHAVIOR._serialized_start=4511
-  _ROUTEFOLLOWINGPARAMS_RESUMEBEHAVIOR._serialized_end=4621
-  _ROUTEFOLLOWINGPARAMS_ROUTEBLOCKEDBEHAVIOR._serialized_start=4623
-  _ROUTEFOLLOWINGPARAMS_ROUTEBLOCKEDBEHAVIOR._serialized_end=4723
-  _NAVIGATEROUTEREQUEST._serialized_start=4726
-  _NAVIGATEROUTEREQUEST._serialized_end=5161
-  _NAVIGATEROUTERESPONSE._serialized_start=5164
-  _NAVIGATEROUTERESPONSE._serialized_end=6092
-  _NAVIGATEROUTERESPONSE_STATUS._serialized_start=5593
-  _NAVIGATEROUTERESPONSE_STATUS._serialized_end=6092
-  _NAVIGATETOANCHORREQUEST._serialized_start=6095
-  _NAVIGATETOANCHORREQUEST._serialized_end=6524
-  _NAVIGATETOANCHORRESPONSE._serialized_start=6527
-  _NAVIGATETOANCHORRESPONSE._serialized_end=7332
-  _NAVIGATETOANCHORRESPONSE_STATUS._serialized_start=6907
-  _NAVIGATETOANCHORRESPONSE_STATUS._serialized_end=7332
-  _NAVIGATIONFEEDBACKREQUEST._serialized_start=7334
-  _NAVIGATIONFEEDBACKREQUEST._serialized_end=7424
-  _NAVIGATIONFEEDBACKRESPONSE._serialized_start=7427
-  _NAVIGATIONFEEDBACKRESPONSE._serialized_end=9661
-  _NAVIGATIONFEEDBACKRESPONSE_AREACALLBACKERRORSENTRY._serialized_start=8345
-  _NAVIGATIONFEEDBACKRESPONSE_AREACALLBACKERRORSENTRY._serialized_end=8443
-  _NAVIGATIONFEEDBACKRESPONSE_ACTIVEREGIONINFORMATIONENTRY._serialized_start=8446
-  _NAVIGATIONFEEDBACKRESPONSE_ACTIVEREGIONINFORMATIONENTRY._serialized_end=8582
-  _NAVIGATIONFEEDBACKRESPONSE_ACTIVEREGIONINFORMATION._serialized_start=8585
-  _NAVIGATIONFEEDBACKRESPONSE_ACTIVEREGIONINFORMATION._serialized_end=8886
-  _NAVIGATIONFEEDBACKRESPONSE_ACTIVEREGIONINFORMATION_AREACALLBACKSTATUS._serialized_start=8771
-  _NAVIGATIONFEEDBACKRESPONSE_ACTIVEREGIONINFORMATION_AREACALLBACKSTATUS._serialized_end=8886
-  _NAVIGATIONFEEDBACKRESPONSE_STATUS._serialized_start=8889
-  _NAVIGATIONFEEDBACKRESPONSE_STATUS._serialized_end=9262
-  _NAVIGATIONFEEDBACKRESPONSE_ROUTEFOLLOWINGSTATUS._serialized_start=9265
-  _NAVIGATIONFEEDBACKRESPONSE_ROUTEFOLLOWINGSTATUS._serialized_end=9506
-  _NAVIGATIONFEEDBACKRESPONSE_BLOCKAGESTATUS._serialized_start=9509
-  _NAVIGATIONFEEDBACKRESPONSE_BLOCKAGESTATUS._serialized_end=9661
-  _GETLOCALIZATIONSTATEREQUEST._serialized_start=9664
-  _GETLOCALIZATIONSTATEREQUEST._serialized_end=9960
-  _REMOTEPOINTCLOUDSTATUS._serialized_start=9962
-  _REMOTEPOINTCLOUDSTATUS._serialized_end=10055
-  _LOSTDETECTORSTATE._serialized_start=10057
-  _LOSTDETECTORSTATE._serialized_end=10093
-  _GETLOCALIZATIONSTATERESPONSE._serialized_start=10096
-  _GETLOCALIZATIONSTATERESPONSE._serialized_end=10486
-  _CLEARGRAPHREQUEST._serialized_start=10488
-  _CLEARGRAPHREQUEST._serialized_end=10584
-  _CLEARGRAPHRESPONSE._serialized_start=10587
-  _CLEARGRAPHRESPONSE._serialized_end=10837
-  _CLEARGRAPHRESPONSE_STATUS._serialized_start=10772
-  _CLEARGRAPHRESPONSE_STATUS._serialized_end=10837
-  _UPLOADGRAPHREQUEST._serialized_start=10840
-  _UPLOADGRAPHREQUEST._serialized_end=11013
-  _UPLOADGRAPHRESPONSE._serialized_start=11016
-  _UPLOADGRAPHRESPONSE._serialized_end=11723
-  _UPLOADGRAPHRESPONSE_STATUS._serialized_start=11555
-  _UPLOADGRAPHRESPONSE_STATUS._serialized_end=11723
-  _DOWNLOADGRAPHREQUEST._serialized_start=11725
-  _DOWNLOADGRAPHREQUEST._serialized_end=11790
-  _DOWNLOADGRAPHRESPONSE._serialized_start=11792
-  _DOWNLOADGRAPHRESPONSE._serialized_end=11903
-  _UPLOADWAYPOINTSNAPSHOTREQUEST._serialized_start=11906
-  _UPLOADWAYPOINTSNAPSHOTREQUEST._serialized_end=12052
-  _UPLOADWAYPOINTSNAPSHOTRESPONSE._serialized_start=12055
-  _UPLOADWAYPOINTSNAPSHOTRESPONSE._serialized_end=12412
-  _UPLOADWAYPOINTSNAPSHOTRESPONSE_STATUS._serialized_start=12336
-  _UPLOADWAYPOINTSNAPSHOTRESPONSE_STATUS._serialized_end=12412
-  _UPLOADEDGESNAPSHOTREQUEST._serialized_start=12415
-  _UPLOADEDGESNAPSHOTREQUEST._serialized_end=12557
-  _UPLOADEDGESNAPSHOTRESPONSE._serialized_start=12559
-  _UPLOADEDGESNAPSHOTRESPONSE._serialized_end=12685
-  _DOWNLOADWAYPOINTSNAPSHOTREQUEST._serialized_start=12688
-  _DOWNLOADWAYPOINTSNAPSHOTREQUEST._serialized_end=12886
-  _DOWNLOADWAYPOINTSNAPSHOTRESPONSE._serialized_start=12889
-  _DOWNLOADWAYPOINTSNAPSHOTRESPONSE._serialized_end=13195
-  _DOWNLOADWAYPOINTSNAPSHOTRESPONSE_STATUS._serialized_start=13116
-  _DOWNLOADWAYPOINTSNAPSHOTRESPONSE_STATUS._serialized_end=13195
-  _DOWNLOADEDGESNAPSHOTREQUEST._serialized_start=13197
-  _DOWNLOADEDGESNAPSHOTREQUEST._serialized_end=13295
-  _DOWNLOADEDGESNAPSHOTRESPONSE._serialized_start=13298
-  _DOWNLOADEDGESNAPSHOTRESPONSE._serialized_end=13592
-  _DOWNLOADEDGESNAPSHOTRESPONSE_STATUS._serialized_start=13116
-  _DOWNLOADEDGESNAPSHOTRESPONSE_STATUS._serialized_end=13195
-  _AREACALLBACKSERVICEERROR._serialized_start=13594
-  _AREACALLBACKSERVICEERROR._serialized_end=13646
-  _VALIDATEGRAPHREQUEST._serialized_start=13648
-  _VALIDATEGRAPHREQUEST._serialized_end=13713
-  _VALIDATEGRAPHRESPONSE._serialized_start=13716
-  _VALIDATEGRAPHRESPONSE._serialized_end=14110
-  _VALIDATEGRAPHRESPONSE_STATUS._serialized_start=14002
-  _VALIDATEGRAPHRESPONSE_STATUS._serialized_end=14110
+  _VISUALREFINEMENTOPTIONS._serialized_start=458
+  _VISUALREFINEMENTOPTIONS._serialized_end=518
+  _SETLOCALIZATIONREQUEST._serialized_start=521
+  _SETLOCALIZATIONREQUEST._serialized_end=1232
+  _SETLOCALIZATIONREQUEST_FIDUCIALINIT._serialized_start=1054
+  _SETLOCALIZATIONREQUEST_FIDUCIALINIT._serialized_end=1218
+  _SENSORCOMPATIBILITYSTATUS._serialized_start=1234
+  _SENSORCOMPATIBILITYSTATUS._serialized_end=1325
+  _SETLOCALIZATIONRESPONSE._serialized_start=1328
+  _SETLOCALIZATIONRESPONSE._serialized_end=2533
+  _SETLOCALIZATIONRESPONSE_SUSPECTEDAMBIGUITY._serialized_start=1922
+  _SETLOCALIZATIONRESPONSE_SUSPECTEDAMBIGUITY._serialized_end=2003
+  _SETLOCALIZATIONRESPONSE_STATUS._serialized_start=2006
+  _SETLOCALIZATIONRESPONSE_STATUS._serialized_end=2345
+  _SETLOCALIZATIONRESPONSE_QUALITYCHECKRESULT._serialized_start=2348
+  _SETLOCALIZATIONRESPONSE_QUALITYCHECKRESULT._serialized_end=2533
+  _ROUTEGENPARAMS._serialized_start=2535
+  _ROUTEGENPARAMS._serialized_end=2551
+  _TRAVELPARAMS._serialized_start=2554
+  _TRAVELPARAMS._serialized_end=3219
+  _TRAVELPARAMS_FEATUREQUALITYTOLERANCE._serialized_start=3105
+  _TRAVELPARAMS_FEATUREQUALITYTOLERANCE._serialized_end=3219
+  _MODIFYNAVIGATIONRESPONSE._serialized_start=3222
+  _MODIFYNAVIGATIONRESPONSE._serialized_end=3496
+  _MODIFYNAVIGATIONRESPONSE_STATUS._serialized_start=3420
+  _MODIFYNAVIGATIONRESPONSE_STATUS._serialized_end=3496
+  _NAVIGATETOREQUEST._serialized_start=3499
+  _NAVIGATETOREQUEST._serialized_end=4004
+  _NAVIGATETORESPONSE._serialized_start=4007
+  _NAVIGATETORESPONSE._serialized_end=4779
+  _NAVIGATETORESPONSE_STATUS._serialized_start=4375
+  _NAVIGATETORESPONSE_STATUS._serialized_end=4779
+  _ROUTEFOLLOWINGPARAMS._serialized_start=4782
+  _ROUTEFOLLOWINGPARAMS._serialized_end=5413
+  _ROUTEFOLLOWINGPARAMS_STARTROUTEBEHAVIOR._serialized_start=5082
+  _ROUTEFOLLOWINGPARAMS_STARTROUTEBEHAVIOR._serialized_end=5199
+  _ROUTEFOLLOWINGPARAMS_RESUMEBEHAVIOR._serialized_start=5201
+  _ROUTEFOLLOWINGPARAMS_RESUMEBEHAVIOR._serialized_end=5311
+  _ROUTEFOLLOWINGPARAMS_ROUTEBLOCKEDBEHAVIOR._serialized_start=5313
+  _ROUTEFOLLOWINGPARAMS_ROUTEBLOCKEDBEHAVIOR._serialized_end=5413
+  _NAVIGATEROUTEREQUEST._serialized_start=5416
+  _NAVIGATEROUTEREQUEST._serialized_end=5851
+  _NAVIGATEROUTERESPONSE._serialized_start=5854
+  _NAVIGATEROUTERESPONSE._serialized_end=6782
+  _NAVIGATEROUTERESPONSE_STATUS._serialized_start=6283
+  _NAVIGATEROUTERESPONSE_STATUS._serialized_end=6782
+  _NAVIGATETOANCHORREQUEST._serialized_start=6785
+  _NAVIGATETOANCHORREQUEST._serialized_end=7214
+  _NAVIGATETOANCHORRESPONSE._serialized_start=7217
+  _NAVIGATETOANCHORRESPONSE._serialized_end=8022
+  _NAVIGATETOANCHORRESPONSE_STATUS._serialized_start=7597
+  _NAVIGATETOANCHORRESPONSE_STATUS._serialized_end=8022
+  _NAVIGATIONFEEDBACKREQUEST._serialized_start=8024
+  _NAVIGATIONFEEDBACKREQUEST._serialized_end=8114
+  _NAVIGATIONFEEDBACKRESPONSE._serialized_start=8117
+  _NAVIGATIONFEEDBACKRESPONSE._serialized_end=10614
+  _NAVIGATIONFEEDBACKRESPONSE_AREACALLBACKERRORSENTRY._serialized_start=9119
+  _NAVIGATIONFEEDBACKRESPONSE_AREACALLBACKERRORSENTRY._serialized_end=9217
+  _NAVIGATIONFEEDBACKRESPONSE_ACTIVEREGIONINFORMATIONENTRY._serialized_start=9220
+  _NAVIGATIONFEEDBACKRESPONSE_ACTIVEREGIONINFORMATIONENTRY._serialized_end=9356
+  _NAVIGATIONFEEDBACKRESPONSE_ACTIVEREGIONINFORMATION._serialized_start=9359
+  _NAVIGATIONFEEDBACKRESPONSE_ACTIVEREGIONINFORMATION._serialized_end=9660
+  _NAVIGATIONFEEDBACKRESPONSE_ACTIVEREGIONINFORMATION_AREACALLBACKSTATUS._serialized_start=9545
+  _NAVIGATIONFEEDBACKRESPONSE_ACTIVEREGIONINFORMATION_AREACALLBACKSTATUS._serialized_end=9660
+  _NAVIGATIONFEEDBACKRESPONSE_STATUS._serialized_start=9663
+  _NAVIGATIONFEEDBACKRESPONSE_STATUS._serialized_end=10036
+  _NAVIGATIONFEEDBACKRESPONSE_ROUTEFOLLOWINGSTATUS._serialized_start=10039
+  _NAVIGATIONFEEDBACKRESPONSE_ROUTEFOLLOWINGSTATUS._serialized_end=10280
+  _NAVIGATIONFEEDBACKRESPONSE_BLOCKAGESTATUS._serialized_start=10283
+  _NAVIGATIONFEEDBACKRESPONSE_BLOCKAGESTATUS._serialized_end=10435
+  _NAVIGATIONFEEDBACKRESPONSE_STUCKREASON._serialized_start=10438
+  _NAVIGATIONFEEDBACKRESPONSE_STUCKREASON._serialized_end=10614
+  _GETLOCALIZATIONSTATEREQUEST._serialized_start=10617
+  _GETLOCALIZATIONSTATEREQUEST._serialized_end=10913
+  _REMOTEPOINTCLOUDSTATUS._serialized_start=10915
+  _REMOTEPOINTCLOUDSTATUS._serialized_end=11008
+  _LOSTDETECTORSTATE._serialized_start=11010
+  _LOSTDETECTORSTATE._serialized_end=11046
+  _GETLOCALIZATIONSTATERESPONSE._serialized_start=11049
+  _GETLOCALIZATIONSTATERESPONSE._serialized_end=11439
+  _CLEARGRAPHREQUEST._serialized_start=11441
+  _CLEARGRAPHREQUEST._serialized_end=11537
+  _CLEARGRAPHRESPONSE._serialized_start=11540
+  _CLEARGRAPHRESPONSE._serialized_end=11790
+  _CLEARGRAPHRESPONSE_STATUS._serialized_start=11725
+  _CLEARGRAPHRESPONSE_STATUS._serialized_end=11790
+  _UPLOADGRAPHREQUEST._serialized_start=11793
+  _UPLOADGRAPHREQUEST._serialized_end=12011
+  _UPLOADGRAPHRESPONSE._serialized_start=12014
+  _UPLOADGRAPHRESPONSE._serialized_end=13457
+  _UPLOADGRAPHRESPONSE_VALIDATIONSTATUS._serialized_start=12691
+  _UPLOADGRAPHRESPONSE_VALIDATIONSTATUS._serialized_end=13286
+  _UPLOADGRAPHRESPONSE_STATUS._serialized_start=13289
+  _UPLOADGRAPHRESPONSE_STATUS._serialized_end=13457
+  _DOWNLOADGRAPHREQUEST._serialized_start=13459
+  _DOWNLOADGRAPHREQUEST._serialized_end=13524
+  _DOWNLOADGRAPHRESPONSE._serialized_start=13526
+  _DOWNLOADGRAPHRESPONSE._serialized_end=13637
+  _UPLOADWAYPOINTSNAPSHOTREQUEST._serialized_start=13640
+  _UPLOADWAYPOINTSNAPSHOTREQUEST._serialized_end=13786
+  _UPLOADWAYPOINTSNAPSHOTRESPONSE._serialized_start=13789
+  _UPLOADWAYPOINTSNAPSHOTRESPONSE._serialized_end=14197
+  _UPLOADWAYPOINTSNAPSHOTRESPONSE_STATUS._serialized_start=14121
+  _UPLOADWAYPOINTSNAPSHOTRESPONSE_STATUS._serialized_end=14197
+  _UPLOADEDGESNAPSHOTREQUEST._serialized_start=14200
+  _UPLOADEDGESNAPSHOTREQUEST._serialized_end=14342
+  _UPLOADEDGESNAPSHOTRESPONSE._serialized_start=14345
+  _UPLOADEDGESNAPSHOTRESPONSE._serialized_end=14522
+  _DOWNLOADWAYPOINTSNAPSHOTREQUEST._serialized_start=14525
+  _DOWNLOADWAYPOINTSNAPSHOTREQUEST._serialized_end=14723
+  _DOWNLOADWAYPOINTSNAPSHOTRESPONSE._serialized_start=14726
+  _DOWNLOADWAYPOINTSNAPSHOTRESPONSE._serialized_end=15032
+  _DOWNLOADWAYPOINTSNAPSHOTRESPONSE_STATUS._serialized_start=14953
+  _DOWNLOADWAYPOINTSNAPSHOTRESPONSE_STATUS._serialized_end=15032
+  _DOWNLOADEDGESNAPSHOTREQUEST._serialized_start=15034
+  _DOWNLOADEDGESNAPSHOTREQUEST._serialized_end=15132
+  _DOWNLOADEDGESNAPSHOTRESPONSE._serialized_start=15135
+  _DOWNLOADEDGESNAPSHOTRESPONSE._serialized_end=15429
+  _DOWNLOADEDGESNAPSHOTRESPONSE_STATUS._serialized_start=14953
+  _DOWNLOADEDGESNAPSHOTRESPONSE_STATUS._serialized_end=15032
+  _AREACALLBACKSERVICEERROR._serialized_start=15431
+  _AREACALLBACKSERVICEERROR._serialized_end=15535
+  _VALIDATEGRAPHREQUEST._serialized_start=15537
+  _VALIDATEGRAPHREQUEST._serialized_end=15602
+  _VALIDATEGRAPHRESPONSE._serialized_start=15605
+  _VALIDATEGRAPHRESPONSE._serialized_end=15999
+  _VALIDATEGRAPHRESPONSE_STATUS._serialized_start=15891
+  _VALIDATEGRAPHRESPONSE_STATUS._serialized_end=15999
 # @@protoc_insertion_point(module_scope)
```

## bosdyn/api/graph_nav/map_pb2.py

```diff
@@ -10,60 +10,62 @@
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from bosdyn.api import geometry_pb2 as bosdyn_dot_api_dot_geometry__pb2
+from bosdyn.api.graph_nav import area_callback_data_pb2 as bosdyn_dot_api_dot_graph__nav_dot_area__callback__data__pb2
 from bosdyn.api import image_pb2 as bosdyn_dot_api_dot_image__pb2
 from bosdyn.api import local_grid_pb2 as bosdyn_dot_api_dot_local__grid__pb2
 from bosdyn.api import payload_pb2 as bosdyn_dot_api_dot_payload__pb2
 from bosdyn.api import point_cloud_pb2 as bosdyn_dot_api_dot_point__cloud__pb2
 from bosdyn.api import robot_id_pb2 as bosdyn_dot_api_dot_robot__id__pb2
 from bosdyn.api import robot_state_pb2 as bosdyn_dot_api_dot_robot__state__pb2
 from bosdyn.api.spot import robot_command_pb2 as bosdyn_dot_api_dot_spot_dot_robot__command__pb2
 from bosdyn.api import stairs_pb2 as bosdyn_dot_api_dot_stairs__pb2
 from bosdyn.api import world_object_pb2 as bosdyn_dot_api_dot_world__object__pb2
-from google.protobuf import any_pb2 as google_dot_protobuf_dot_any__pb2
 from google.protobuf import field_mask_pb2 as google_dot_protobuf_dot_field__mask__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1e\x62osdyn/api/graph_nav/map.proto\x12\x14\x62osdyn.api.graph_nav\x1a\x19\x62osdyn/api/geometry.proto\x1a\x16\x62osdyn/api/image.proto\x1a\x1b\x62osdyn/api/local_grid.proto\x1a\x18\x62osdyn/api/payload.proto\x1a\x1c\x62osdyn/api/point_cloud.proto\x1a\x19\x62osdyn/api/robot_id.proto\x1a\x1c\x62osdyn/api/robot_state.proto\x1a#bosdyn/api/spot/robot_command.proto\x1a\x17\x62osdyn/api/stairs.proto\x1a\x1d\x62osdyn/api/world_object.proto\x1a\x19google/protobuf/any.proto\x1a google/protobuf/field_mask.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\xa3\x08\n\x08Waypoint\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0bsnapshot_id\x18\x02 \x01(\t\x12.\n\x11waypoint_tform_ko\x18\x03 \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\x12?\n\x0b\x61nnotations\x18\x04 \x01(\x0b\x32*.bosdyn.api.graph_nav.Waypoint.Annotations\x1a\xe5\x05\n\x0b\x41nnotations\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x31\n\rcreation_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0cicp_variance\x18\x02 \x01(\x0b\x32\x19.bosdyn.api.SE3Covariance\x12T\n\x11scan_match_region\x18\x03 \x01(\x0b\x32\x39.bosdyn.api.graph_nav.Waypoint.Annotations.LocalizeRegion\x12\x46\n\x0fwaypoint_source\x18\x05 \x01(\x0e\x32-.bosdyn.api.graph_nav.Waypoint.WaypointSource\x12=\n\x0f\x63lient_metadata\x18\x06 \x01(\x0b\x32$.bosdyn.api.graph_nav.ClientMetadata\x1a\x86\x03\n\x0eLocalizeRegion\x12\x34\n\x05state\x18\x01 \x01(\x0e\x32%.bosdyn.api.graph_nav.AnnotationState\x12[\n\x0e\x64\x65\x66\x61ult_region\x18\x02 \x01(\x0b\x32\x41.bosdyn.api.graph_nav.Waypoint.Annotations.LocalizeRegion.DefaultH\x00\x12P\n\x05\x65mpty\x18\x03 \x01(\x0b\x32?.bosdyn.api.graph_nav.Waypoint.Annotations.LocalizeRegion.EmptyH\x00\x12T\n\x06\x63ircle\x18\x04 \x01(\x0b\x32\x42.bosdyn.api.graph_nav.Waypoint.Annotations.LocalizeRegion.Circle2DH\x00\x1a\t\n\x07\x44\x65\x66\x61ult\x1a\x07\n\x05\x45mpty\x1a\x1b\n\x08\x43ircle2D\x12\x0f\n\x07\x64ist_2d\x18\x01 \x01(\x01\x42\x08\n\x06region\"\x9c\x01\n\x0eWaypointSource\x12\x1b\n\x17WAYPOINT_SOURCE_UNKNOWN\x10\x00\x12\x1e\n\x1aWAYPOINT_SOURCE_ROBOT_PATH\x10\x01\x12 \n\x1cWAYPOINT_SOURCE_USER_REQUEST\x10\x02\x12+\n\'WAYPOINT_SOURCE_ALTERNATE_ROUTE_FINDING\x10\x03\"\x88\x01\n\x0e\x43lientMetadata\x12\x14\n\x0csession_name\x18\x01 \x01(\t\x12\x17\n\x0f\x63lient_username\x18\x02 \x01(\t\x12\x1f\n\x17\x63lient_software_version\x18\x03 \x01(\t\x12\x11\n\tclient_id\x18\x04 \x01(\t\x12\x13\n\x0b\x63lient_type\x18\x05 \x01(\t\"\xa7\x04\n\x10WaypointSnapshot\x12\n\n\x02id\x18\x01 \x01(\t\x12)\n\x06images\x18\x02 \x03(\x0b\x32\x19.bosdyn.api.ImageResponse\x12+\n\x0bpoint_cloud\x18\x03 \x01(\x0b\x32\x16.bosdyn.api.PointCloud\x12(\n\x07objects\x18\x04 \x03(\x0b\x32\x17.bosdyn.api.WorldObject\x12+\n\x0brobot_state\x18\x05 \x01(\x0b\x32\x16.bosdyn.api.RobotState\x12\x30\n\x11robot_local_grids\x18\x06 \x03(\x0b\x32\x15.bosdyn.api.LocalGrid\x12 \n\x18is_point_cloud_processed\x18\x08 \x01(\x08\x12\x12\n\nversion_id\x18\t \x01(\t\x12%\n\x1dhas_remote_point_cloud_sensor\x18\n \x01(\x08\x12\x41\n$body_tform_remote_point_cloud_sensor\x18\x0b \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\x12%\n\x08payloads\x18\x0c \x03(\x0b\x32\x13.bosdyn.api.Payload\x12%\n\x08robot_id\x18\x0e \x01(\x0b\x32\x13.bosdyn.api.RobotId\x12\x38\n\x14recording_started_on\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x92\x10\n\x04\x45\x64ge\x12)\n\x02id\x18\x01 \x01(\x0b\x32\x1d.bosdyn.api.graph_nav.Edge.Id\x12\x13\n\x0bsnapshot_id\x18\x02 \x01(\t\x12*\n\rfrom_tform_to\x18\x03 \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\x12;\n\x0b\x61nnotations\x18\x04 \x01(\x0b\x32&.bosdyn.api.graph_nav.Edge.Annotations\x1a\x30\n\x02Id\x12\x15\n\rfrom_waypoint\x18\x01 \x01(\t\x12\x13\n\x0bto_waypoint\x18\x02 \x01(\t\x1a\xda\x0c\n\x0b\x41nnotations\x12\x33\n\tvel_limit\x18\x01 \x01(\x0b\x32\x1c.bosdyn.api.SE2VelocityLimitB\x02\x18\x01\x12@\n\x06stairs\x18\x02 \x01(\x0b\x32\x30.bosdyn.api.graph_nav.Edge.Annotations.StairData\x12X\n\x14\x64irection_constraint\x18\x04 \x01(\x0e\x32:.bosdyn.api.graph_nav.Edge.Annotations.DirectionConstraint\x12\x35\n\x11require_alignment\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12/\n\x0b\x66lat_ground\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x38\n\x0eground_mu_hint\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.DoubleValueB\x02\x18\x01\x12\x34\n\x0cgrated_floor\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.BoolValueB\x02\x18\x01\x12<\n\x18override_mobility_params\x18\t \x01(\x0b\x32\x1a.google.protobuf.FieldMask\x12\x38\n\x0fmobility_params\x18\n \x01(\x0b\x32\x1f.bosdyn.api.spot.MobilityParams\x12*\n\x04\x63ost\x18\x0b \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12:\n\x0b\x65\x64ge_source\x18\x0c \x01(\x0e\x32%.bosdyn.api.graph_nav.Edge.EdgeSource\x12\'\n\x1f\x64isable_alternate_route_finding\x18\r \x01(\x08\x12U\n\x13path_following_mode\x18\x0e \x01(\x0e\x32\x38.bosdyn.api.graph_nav.Edge.Annotations.PathFollowingMode\x12$\n\x1c\x64isable_directed_exploration\x18\x0f \x01(\x08\x12Q\n\x0e\x61rea_callbacks\x18\x10 \x03(\x0b\x32\x39.bosdyn.api.graph_nav.Edge.Annotations.AreaCallbacksEntry\x12^\n\x13ground_clutter_mode\x18\x11 \x01(\x0e\x32\x41.bosdyn.api.graph_nav.Edge.Annotations.GroundClutterAvoidanceMode\x1a|\n\tStairData\x12\x34\n\x05state\x18\x01 \x01(\x0e\x32%.bosdyn.api.graph_nav.AnnotationState\x12\x39\n\x12straight_staircase\x18\x02 \x01(\x0b\x32\x1d.bosdyn.api.StraightStaircase\x1a^\n\x12\x41reaCallbacksEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x37\n\x05value\x18\x02 \x01(\x0b\x32(.bosdyn.api.graph_nav.AreaCallbackRegion:\x02\x38\x01\"\xbc\x01\n\x13\x44irectionConstraint\x12 \n\x1c\x44IRECTION_CONSTRAINT_UNKNOWN\x10\x00\x12 \n\x1c\x44IRECTION_CONSTRAINT_NO_TURN\x10\x01\x12 \n\x1c\x44IRECTION_CONSTRAINT_FORWARD\x10\x02\x12 \n\x1c\x44IRECTION_CONSTRAINT_REVERSE\x10\x03\x12\x1d\n\x19\x44IRECTION_CONSTRAINT_NONE\x10\x04\"W\n\x11PathFollowingMode\x12\x15\n\x11PATH_MODE_UNKNOWN\x10\x00\x12\x15\n\x11PATH_MODE_DEFAULT\x10\x01\x12\x14\n\x10PATH_MODE_STRICT\x10\x02\"s\n\x1aGroundClutterAvoidanceMode\x12\x1a\n\x16GROUND_CLUTTER_UNKNOWN\x10\x00\x12\x16\n\x12GROUND_CLUTTER_OFF\x10\x01\x12!\n\x1dGROUND_CLUTTER_FROM_FOOTFALLS\x10\x02\"\xd1\x01\n\nEdgeSource\x12\x17\n\x13\x45\x44GE_SOURCE_UNKNOWN\x10\x00\x12\x18\n\x14\x45\x44GE_SOURCE_ODOMETRY\x10\x01\x12\"\n\x1e\x45\x44GE_SOURCE_SMALL_LOOP_CLOSURE\x10\x02\x12%\n!EDGE_SOURCE_FIDUCIAL_LOOP_CLOSURE\x10\x03\x12\'\n#EDGE_SOURCE_ALTERNATE_ROUTE_FINDING\x10\x04\x12\x1c\n\x18\x45\x44GE_SOURCE_USER_REQUEST\x10\x05\"\xf8\x03\n\x0c\x45\x64geSnapshot\x12\n\n\x02id\x18\x01 \x01(\t\x12:\n\x07stances\x18\x02 \x03(\x0b\x32).bosdyn.api.graph_nav.EdgeSnapshot.Stance\x12M\n\x0e\x61rea_callbacks\x18\x10 \x03(\x0b\x32\x35.bosdyn.api.graph_nav.EdgeSnapshot.AreaCallbacksEntry\x1a\xf2\x01\n\x06Stance\x12-\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12*\n\x0b\x66oot_states\x18\x02 \x03(\x0b\x32\x15.bosdyn.api.FootState\x12*\n\rko_tform_body\x18\x03 \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\x12.\n\x11vision_tform_body\x18\x05 \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\x12\x31\n\rplanar_ground\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x1a\\\n\x12\x41reaCallbacksEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x35\n\x05value\x18\x02 \x01(\x0b\x32&.bosdyn.api.graph_nav.AreaCallbackData:\x02\x38\x01\"F\n\x06\x41nchor\x12\n\n\x02id\x18\x01 \x01(\t\x12\x30\n\x13seed_tform_waypoint\x18\x02 \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\"Q\n\x13\x41nchoredWorldObject\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\x11seed_tform_object\x18\x02 \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\"v\n\tAnchoring\x12-\n\x07\x61nchors\x18\x01 \x03(\x0b\x32\x1c.bosdyn.api.graph_nav.Anchor\x12:\n\x07objects\x18\x02 \x03(\x0b\x32).bosdyn.api.graph_nav.AnchoredWorldObject\"?\n\x12\x41reaCallbackRegion\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\"=\n\x10\x41reaCallbackData\x12)\n\x0b\x63onfig_data\x18\x01 \x01(\x0b\x32\x14.google.protobuf.Any\"\x99\x01\n\x05Graph\x12\x31\n\twaypoints\x18\x01 \x03(\x0b\x32\x1e.bosdyn.api.graph_nav.Waypoint\x12)\n\x05\x65\x64ges\x18\x02 \x03(\x0b\x32\x1a.bosdyn.api.graph_nav.Edge\x12\x32\n\tanchoring\x18\x03 \x01(\x0b\x32\x1f.bosdyn.api.graph_nav.Anchoring*d\n\x0f\x41nnotationState\x12\x1c\n\x18\x41NNOTATION_STATE_UNKNOWN\x10\x00\x12\x18\n\x14\x41NNOTATION_STATE_SET\x10\x01\x12\x19\n\x15\x41NNOTATION_STATE_NONE\x10\x02\x42\nB\x08MapProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1e\x62osdyn/api/graph_nav/map.proto\x12\x14\x62osdyn.api.graph_nav\x1a\x19\x62osdyn/api/geometry.proto\x1a-bosdyn/api/graph_nav/area_callback_data.proto\x1a\x16\x62osdyn/api/image.proto\x1a\x1b\x62osdyn/api/local_grid.proto\x1a\x18\x62osdyn/api/payload.proto\x1a\x1c\x62osdyn/api/point_cloud.proto\x1a\x19\x62osdyn/api/robot_id.proto\x1a\x1c\x62osdyn/api/robot_state.proto\x1a#bosdyn/api/spot/robot_command.proto\x1a\x17\x62osdyn/api/stairs.proto\x1a\x1d\x62osdyn/api/world_object.proto\x1a google/protobuf/field_mask.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\x94\n\n\x08Waypoint\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0bsnapshot_id\x18\x02 \x01(\t\x12.\n\x11waypoint_tform_ko\x18\x03 \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\x12?\n\x0b\x61nnotations\x18\x04 \x01(\x0b\x32*.bosdyn.api.graph_nav.Waypoint.Annotations\x1a\xd6\x07\n\x0b\x41nnotations\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x31\n\rcreation_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0cicp_variance\x18\x02 \x01(\x0b\x32\x19.bosdyn.api.SE3Covariance\x12T\n\x11scan_match_region\x18\x03 \x01(\x0b\x32\x39.bosdyn.api.graph_nav.Waypoint.Annotations.LocalizeRegion\x12\x46\n\x0fwaypoint_source\x18\x05 \x01(\x0e\x32-.bosdyn.api.graph_nav.Waypoint.WaypointSource\x12=\n\x0f\x63lient_metadata\x18\x06 \x01(\x0b\x32$.bosdyn.api.graph_nav.ClientMetadata\x12]\n\x15loop_closure_settings\x18\x07 \x01(\x0b\x32>.bosdyn.api.graph_nav.Waypoint.Annotations.LoopClosureSettings\x1a\x86\x03\n\x0eLocalizeRegion\x12\x34\n\x05state\x18\x01 \x01(\x0e\x32%.bosdyn.api.graph_nav.AnnotationState\x12[\n\x0e\x64\x65\x66\x61ult_region\x18\x02 \x01(\x0b\x32\x41.bosdyn.api.graph_nav.Waypoint.Annotations.LocalizeRegion.DefaultH\x00\x12P\n\x05\x65mpty\x18\x03 \x01(\x0b\x32?.bosdyn.api.graph_nav.Waypoint.Annotations.LocalizeRegion.EmptyH\x00\x12T\n\x06\x63ircle\x18\x04 \x01(\x0b\x32\x42.bosdyn.api.graph_nav.Waypoint.Annotations.LocalizeRegion.Circle2DH\x00\x1a\t\n\x07\x44\x65\x66\x61ult\x1a\x07\n\x05\x45mpty\x1a\x1b\n\x08\x43ircle2D\x12\x0f\n\x07\x64ist_2d\x18\x01 \x01(\x01\x42\x08\n\x06region\x1a\x8f\x01\n\x13LoopClosureSettings\x12\x1c\n\x14\x64isable_loop_closure\x18\x01 \x01(\x08\x12\x1f\n\x17\x64isable_collision_check\x18\x02 \x01(\x08\x12\x17\n\x0fmax_edge_length\x18\x03 \x01(\x01\x12 \n\x18max_odometry_path_length\x18\x04 \x01(\x01\"\x9c\x01\n\x0eWaypointSource\x12\x1b\n\x17WAYPOINT_SOURCE_UNKNOWN\x10\x00\x12\x1e\n\x1aWAYPOINT_SOURCE_ROBOT_PATH\x10\x01\x12 \n\x1cWAYPOINT_SOURCE_USER_REQUEST\x10\x02\x12+\n\'WAYPOINT_SOURCE_ALTERNATE_ROUTE_FINDING\x10\x03\"\x88\x01\n\x0e\x43lientMetadata\x12\x14\n\x0csession_name\x18\x01 \x01(\t\x12\x17\n\x0f\x63lient_username\x18\x02 \x01(\t\x12\x1f\n\x17\x63lient_software_version\x18\x03 \x01(\t\x12\x11\n\tclient_id\x18\x04 \x01(\t\x12\x13\n\x0b\x63lient_type\x18\x05 \x01(\t\"\xa7\x04\n\x10WaypointSnapshot\x12\n\n\x02id\x18\x01 \x01(\t\x12)\n\x06images\x18\x02 \x03(\x0b\x32\x19.bosdyn.api.ImageResponse\x12+\n\x0bpoint_cloud\x18\x03 \x01(\x0b\x32\x16.bosdyn.api.PointCloud\x12(\n\x07objects\x18\x04 \x03(\x0b\x32\x17.bosdyn.api.WorldObject\x12+\n\x0brobot_state\x18\x05 \x01(\x0b\x32\x16.bosdyn.api.RobotState\x12\x30\n\x11robot_local_grids\x18\x06 \x03(\x0b\x32\x15.bosdyn.api.LocalGrid\x12 \n\x18is_point_cloud_processed\x18\x08 \x01(\x08\x12\x12\n\nversion_id\x18\t \x01(\t\x12%\n\x1dhas_remote_point_cloud_sensor\x18\n \x01(\x08\x12\x41\n$body_tform_remote_point_cloud_sensor\x18\x0b \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\x12%\n\x08payloads\x18\x0c \x03(\x0b\x32\x13.bosdyn.api.Payload\x12%\n\x08robot_id\x18\x0e \x01(\x0b\x32\x13.bosdyn.api.RobotId\x12\x38\n\x14recording_started_on\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xfd\x10\n\x04\x45\x64ge\x12)\n\x02id\x18\x01 \x01(\x0b\x32\x1d.bosdyn.api.graph_nav.Edge.Id\x12\x13\n\x0bsnapshot_id\x18\x02 \x01(\t\x12*\n\rfrom_tform_to\x18\x03 \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\x12;\n\x0b\x61nnotations\x18\x04 \x01(\x0b\x32&.bosdyn.api.graph_nav.Edge.Annotations\x1a\x30\n\x02Id\x12\x15\n\rfrom_waypoint\x18\x01 \x01(\t\x12\x13\n\x0bto_waypoint\x18\x02 \x01(\t\x1a\xa7\r\n\x0b\x41nnotations\x12\x33\n\tvel_limit\x18\x01 \x01(\x0b\x32\x1c.bosdyn.api.SE2VelocityLimitB\x02\x18\x01\x12@\n\x06stairs\x18\x02 \x01(\x0b\x32\x30.bosdyn.api.graph_nav.Edge.Annotations.StairData\x12X\n\x14\x64irection_constraint\x18\x04 \x01(\x0e\x32:.bosdyn.api.graph_nav.Edge.Annotations.DirectionConstraint\x12\x35\n\x11require_alignment\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x33\n\x0b\x66lat_ground\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.BoolValueB\x02\x18\x01\x12\x38\n\x0eground_mu_hint\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.DoubleValueB\x02\x18\x01\x12\x34\n\x0cgrated_floor\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.BoolValueB\x02\x18\x01\x12<\n\x18override_mobility_params\x18\t \x01(\x0b\x32\x1a.google.protobuf.FieldMask\x12\x38\n\x0fmobility_params\x18\n \x01(\x0b\x32\x1f.bosdyn.api.spot.MobilityParams\x12*\n\x04\x63ost\x18\x0b \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12:\n\x0b\x65\x64ge_source\x18\x0c \x01(\x0e\x32%.bosdyn.api.graph_nav.Edge.EdgeSource\x12\'\n\x1f\x64isable_alternate_route_finding\x18\r \x01(\x08\x12U\n\x13path_following_mode\x18\x0e \x01(\x0e\x32\x38.bosdyn.api.graph_nav.Edge.Annotations.PathFollowingMode\x12$\n\x1c\x64isable_directed_exploration\x18\x0f \x01(\x08\x12Q\n\x0e\x61rea_callbacks\x18\x10 \x03(\x0b\x32\x39.bosdyn.api.graph_nav.Edge.Annotations.AreaCallbacksEntry\x12^\n\x13ground_clutter_mode\x18\x11 \x01(\x0e\x32\x41.bosdyn.api.graph_nav.Edge.Annotations.GroundClutterAvoidanceMode\x1a\xc4\x01\n\tStairData\x12\x34\n\x05state\x18\x01 \x01(\x0e\x32%.bosdyn.api.graph_nav.AnnotationState\x12=\n\x12straight_staircase\x18\x02 \x01(\x0b\x32\x1d.bosdyn.api.StraightStaircaseB\x02\x18\x01\x12\x42\n\x17staircase_with_landings\x18\x03 \x01(\x0b\x32!.bosdyn.api.StaircaseWithLandings\x1a^\n\x12\x41reaCallbacksEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x37\n\x05value\x18\x02 \x01(\x0b\x32(.bosdyn.api.graph_nav.AreaCallbackRegion:\x02\x38\x01\"\xbc\x01\n\x13\x44irectionConstraint\x12 \n\x1c\x44IRECTION_CONSTRAINT_UNKNOWN\x10\x00\x12 \n\x1c\x44IRECTION_CONSTRAINT_NO_TURN\x10\x01\x12 \n\x1c\x44IRECTION_CONSTRAINT_FORWARD\x10\x02\x12 \n\x1c\x44IRECTION_CONSTRAINT_REVERSE\x10\x03\x12\x1d\n\x19\x44IRECTION_CONSTRAINT_NONE\x10\x04\"W\n\x11PathFollowingMode\x12\x15\n\x11PATH_MODE_UNKNOWN\x10\x00\x12\x15\n\x11PATH_MODE_DEFAULT\x10\x01\x12\x14\n\x10PATH_MODE_STRICT\x10\x02\"s\n\x1aGroundClutterAvoidanceMode\x12\x1a\n\x16GROUND_CLUTTER_UNKNOWN\x10\x00\x12\x16\n\x12GROUND_CLUTTER_OFF\x10\x01\x12!\n\x1dGROUND_CLUTTER_FROM_FOOTFALLS\x10\x02\"\xef\x01\n\nEdgeSource\x12\x17\n\x13\x45\x44GE_SOURCE_UNKNOWN\x10\x00\x12\x18\n\x14\x45\x44GE_SOURCE_ODOMETRY\x10\x01\x12\"\n\x1e\x45\x44GE_SOURCE_SMALL_LOOP_CLOSURE\x10\x02\x12%\n!EDGE_SOURCE_FIDUCIAL_LOOP_CLOSURE\x10\x03\x12\'\n#EDGE_SOURCE_ALTERNATE_ROUTE_FINDING\x10\x04\x12\x1c\n\x18\x45\x44GE_SOURCE_USER_REQUEST\x10\x05\x12\x1c\n\x18\x45\x44GE_SOURCE_LOCALIZATION\x10\x06\"\xf8\x03\n\x0c\x45\x64geSnapshot\x12\n\n\x02id\x18\x01 \x01(\t\x12:\n\x07stances\x18\x02 \x03(\x0b\x32).bosdyn.api.graph_nav.EdgeSnapshot.Stance\x12M\n\x0e\x61rea_callbacks\x18\x10 \x03(\x0b\x32\x35.bosdyn.api.graph_nav.EdgeSnapshot.AreaCallbacksEntry\x1a\xf2\x01\n\x06Stance\x12-\n\ttimestamp\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12*\n\x0b\x66oot_states\x18\x02 \x03(\x0b\x32\x15.bosdyn.api.FootState\x12*\n\rko_tform_body\x18\x03 \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\x12.\n\x11vision_tform_body\x18\x05 \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\x12\x31\n\rplanar_ground\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x1a\\\n\x12\x41reaCallbacksEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x35\n\x05value\x18\x02 \x01(\x0b\x32&.bosdyn.api.graph_nav.AreaCallbackData:\x02\x38\x01\"F\n\x06\x41nchor\x12\n\n\x02id\x18\x01 \x01(\t\x12\x30\n\x13seed_tform_waypoint\x18\x02 \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\"Q\n\x13\x41nchoredWorldObject\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\x11seed_tform_object\x18\x02 \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\"v\n\tAnchoring\x12-\n\x07\x61nchors\x18\x01 \x03(\x0b\x32\x1c.bosdyn.api.graph_nav.Anchor\x12:\n\x07objects\x18\x02 \x03(\x0b\x32).bosdyn.api.graph_nav.AnchoredWorldObject\"~\n\x12\x41reaCallbackRegion\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12=\n\rrecorded_data\x18\x04 \x01(\x0b\x32&.bosdyn.api.graph_nav.AreaCallbackData\"\x99\x01\n\x05Graph\x12\x31\n\twaypoints\x18\x01 \x03(\x0b\x32\x1e.bosdyn.api.graph_nav.Waypoint\x12)\n\x05\x65\x64ges\x18\x02 \x03(\x0b\x32\x1a.bosdyn.api.graph_nav.Edge\x12\x32\n\tanchoring\x18\x03 \x01(\x0b\x32\x1f.bosdyn.api.graph_nav.Anchoring\"\xb5\x04\n\x08MapStats\x12\x36\n\twaypoints\x18\x01 \x01(\x0b\x32#.bosdyn.api.graph_nav.MapStats.Stat\x12?\n\x12waypoint_snapshots\x18\x02 \x01(\x0b\x32#.bosdyn.api.graph_nav.MapStats.Stat\x12@\n\x13\x61lternate_waypoints\x18\x03 \x01(\x0b\x32#.bosdyn.api.graph_nav.MapStats.Stat\x12\x32\n\x05\x65\x64ges\x18\x04 \x01(\x0b\x32#.bosdyn.api.graph_nav.MapStats.Stat\x12;\n\x0e\x65\x64ge_snapshots\x18\x05 \x01(\x0b\x32#.bosdyn.api.graph_nav.MapStats.Stat\x12<\n\x0f\x61lternate_edges\x18\x06 \x01(\x0b\x32#.bosdyn.api.graph_nav.MapStats.Stat\x12=\n\x10waypoint_anchors\x18\x07 \x01(\x0b\x32#.bosdyn.api.graph_nav.MapStats.Stat\x12;\n\x0eobject_anchors\x18\x08 \x01(\x0b\x32#.bosdyn.api.graph_nav.MapStats.Stat\x12\x19\n\x11total_path_length\x18\t \x01(\x01\x1a(\n\x04Stat\x12\r\n\x05\x63ount\x18\x01 \x01(\x05\x12\x11\n\tnum_bytes\x18\x02 \x01(\x03*d\n\x0f\x41nnotationState\x12\x1c\n\x18\x41NNOTATION_STATE_UNKNOWN\x10\x00\x12\x18\n\x14\x41NNOTATION_STATE_SET\x10\x01\x12\x19\n\x15\x41NNOTATION_STATE_NONE\x10\x02\x42\nB\x08MapProtob\x06proto3')
 
 _ANNOTATIONSTATE = DESCRIPTOR.enum_types_by_name['AnnotationState']
 AnnotationState = enum_type_wrapper.EnumTypeWrapper(_ANNOTATIONSTATE)
 ANNOTATION_STATE_UNKNOWN = 0
 ANNOTATION_STATE_SET = 1
 ANNOTATION_STATE_NONE = 2
 
 
 _WAYPOINT = DESCRIPTOR.message_types_by_name['Waypoint']
 _WAYPOINT_ANNOTATIONS = _WAYPOINT.nested_types_by_name['Annotations']
 _WAYPOINT_ANNOTATIONS_LOCALIZEREGION = _WAYPOINT_ANNOTATIONS.nested_types_by_name['LocalizeRegion']
 _WAYPOINT_ANNOTATIONS_LOCALIZEREGION_DEFAULT = _WAYPOINT_ANNOTATIONS_LOCALIZEREGION.nested_types_by_name['Default']
 _WAYPOINT_ANNOTATIONS_LOCALIZEREGION_EMPTY = _WAYPOINT_ANNOTATIONS_LOCALIZEREGION.nested_types_by_name['Empty']
 _WAYPOINT_ANNOTATIONS_LOCALIZEREGION_CIRCLE2D = _WAYPOINT_ANNOTATIONS_LOCALIZEREGION.nested_types_by_name['Circle2D']
+_WAYPOINT_ANNOTATIONS_LOOPCLOSURESETTINGS = _WAYPOINT_ANNOTATIONS.nested_types_by_name['LoopClosureSettings']
 _CLIENTMETADATA = DESCRIPTOR.message_types_by_name['ClientMetadata']
 _WAYPOINTSNAPSHOT = DESCRIPTOR.message_types_by_name['WaypointSnapshot']
 _EDGE = DESCRIPTOR.message_types_by_name['Edge']
 _EDGE_ID = _EDGE.nested_types_by_name['Id']
 _EDGE_ANNOTATIONS = _EDGE.nested_types_by_name['Annotations']
 _EDGE_ANNOTATIONS_STAIRDATA = _EDGE_ANNOTATIONS.nested_types_by_name['StairData']
 _EDGE_ANNOTATIONS_AREACALLBACKSENTRY = _EDGE_ANNOTATIONS.nested_types_by_name['AreaCallbacksEntry']
 _EDGESNAPSHOT = DESCRIPTOR.message_types_by_name['EdgeSnapshot']
 _EDGESNAPSHOT_STANCE = _EDGESNAPSHOT.nested_types_by_name['Stance']
 _EDGESNAPSHOT_AREACALLBACKSENTRY = _EDGESNAPSHOT.nested_types_by_name['AreaCallbacksEntry']
 _ANCHOR = DESCRIPTOR.message_types_by_name['Anchor']
 _ANCHOREDWORLDOBJECT = DESCRIPTOR.message_types_by_name['AnchoredWorldObject']
 _ANCHORING = DESCRIPTOR.message_types_by_name['Anchoring']
 _AREACALLBACKREGION = DESCRIPTOR.message_types_by_name['AreaCallbackRegion']
-_AREACALLBACKDATA = DESCRIPTOR.message_types_by_name['AreaCallbackData']
 _GRAPH = DESCRIPTOR.message_types_by_name['Graph']
+_MAPSTATS = DESCRIPTOR.message_types_by_name['MapStats']
+_MAPSTATS_STAT = _MAPSTATS.nested_types_by_name['Stat']
 _WAYPOINT_WAYPOINTSOURCE = _WAYPOINT.enum_types_by_name['WaypointSource']
 _EDGE_ANNOTATIONS_DIRECTIONCONSTRAINT = _EDGE_ANNOTATIONS.enum_types_by_name['DirectionConstraint']
 _EDGE_ANNOTATIONS_PATHFOLLOWINGMODE = _EDGE_ANNOTATIONS.enum_types_by_name['PathFollowingMode']
 _EDGE_ANNOTATIONS_GROUNDCLUTTERAVOIDANCEMODE = _EDGE_ANNOTATIONS.enum_types_by_name['GroundClutterAvoidanceMode']
 _EDGE_EDGESOURCE = _EDGE.enum_types_by_name['EdgeSource']
 Waypoint = _reflection.GeneratedProtocolMessageType('Waypoint', (_message.Message,), {
 
@@ -92,14 +94,21 @@
         })
       ,
       'DESCRIPTOR' : _WAYPOINT_ANNOTATIONS_LOCALIZEREGION,
       '__module__' : 'bosdyn.api.graph_nav.map_pb2'
       # @@protoc_insertion_point(class_scope:bosdyn.api.graph_nav.Waypoint.Annotations.LocalizeRegion)
       })
     ,
+
+    'LoopClosureSettings' : _reflection.GeneratedProtocolMessageType('LoopClosureSettings', (_message.Message,), {
+      'DESCRIPTOR' : _WAYPOINT_ANNOTATIONS_LOOPCLOSURESETTINGS,
+      '__module__' : 'bosdyn.api.graph_nav.map_pb2'
+      # @@protoc_insertion_point(class_scope:bosdyn.api.graph_nav.Waypoint.Annotations.LoopClosureSettings)
+      })
+    ,
     'DESCRIPTOR' : _WAYPOINT_ANNOTATIONS,
     '__module__' : 'bosdyn.api.graph_nav.map_pb2'
     # @@protoc_insertion_point(class_scope:bosdyn.api.graph_nav.Waypoint.Annotations)
     })
   ,
   'DESCRIPTOR' : _WAYPOINT,
   '__module__' : 'bosdyn.api.graph_nav.map_pb2'
@@ -107,14 +116,15 @@
   })
 _sym_db.RegisterMessage(Waypoint)
 _sym_db.RegisterMessage(Waypoint.Annotations)
 _sym_db.RegisterMessage(Waypoint.Annotations.LocalizeRegion)
 _sym_db.RegisterMessage(Waypoint.Annotations.LocalizeRegion.Default)
 _sym_db.RegisterMessage(Waypoint.Annotations.LocalizeRegion.Empty)
 _sym_db.RegisterMessage(Waypoint.Annotations.LocalizeRegion.Circle2D)
+_sym_db.RegisterMessage(Waypoint.Annotations.LoopClosureSettings)
 
 ClientMetadata = _reflection.GeneratedProtocolMessageType('ClientMetadata', (_message.Message,), {
   'DESCRIPTOR' : _CLIENTMETADATA,
   '__module__' : 'bosdyn.api.graph_nav.map_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.graph_nav.ClientMetadata)
   })
 _sym_db.RegisterMessage(ClientMetadata)
@@ -212,92 +222,108 @@
 AreaCallbackRegion = _reflection.GeneratedProtocolMessageType('AreaCallbackRegion', (_message.Message,), {
   'DESCRIPTOR' : _AREACALLBACKREGION,
   '__module__' : 'bosdyn.api.graph_nav.map_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.graph_nav.AreaCallbackRegion)
   })
 _sym_db.RegisterMessage(AreaCallbackRegion)
 
-AreaCallbackData = _reflection.GeneratedProtocolMessageType('AreaCallbackData', (_message.Message,), {
-  'DESCRIPTOR' : _AREACALLBACKDATA,
-  '__module__' : 'bosdyn.api.graph_nav.map_pb2'
-  # @@protoc_insertion_point(class_scope:bosdyn.api.graph_nav.AreaCallbackData)
-  })
-_sym_db.RegisterMessage(AreaCallbackData)
-
 Graph = _reflection.GeneratedProtocolMessageType('Graph', (_message.Message,), {
   'DESCRIPTOR' : _GRAPH,
   '__module__' : 'bosdyn.api.graph_nav.map_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.graph_nav.Graph)
   })
 _sym_db.RegisterMessage(Graph)
 
+MapStats = _reflection.GeneratedProtocolMessageType('MapStats', (_message.Message,), {
+
+  'Stat' : _reflection.GeneratedProtocolMessageType('Stat', (_message.Message,), {
+    'DESCRIPTOR' : _MAPSTATS_STAT,
+    '__module__' : 'bosdyn.api.graph_nav.map_pb2'
+    # @@protoc_insertion_point(class_scope:bosdyn.api.graph_nav.MapStats.Stat)
+    })
+  ,
+  'DESCRIPTOR' : _MAPSTATS,
+  '__module__' : 'bosdyn.api.graph_nav.map_pb2'
+  # @@protoc_insertion_point(class_scope:bosdyn.api.graph_nav.MapStats)
+  })
+_sym_db.RegisterMessage(MapStats)
+_sym_db.RegisterMessage(MapStats.Stat)
+
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'B\010MapProto'
+  _EDGE_ANNOTATIONS_STAIRDATA.fields_by_name['straight_staircase']._options = None
+  _EDGE_ANNOTATIONS_STAIRDATA.fields_by_name['straight_staircase']._serialized_options = b'\030\001'
   _EDGE_ANNOTATIONS_AREACALLBACKSENTRY._options = None
   _EDGE_ANNOTATIONS_AREACALLBACKSENTRY._serialized_options = b'8\001'
   _EDGE_ANNOTATIONS.fields_by_name['vel_limit']._options = None
   _EDGE_ANNOTATIONS.fields_by_name['vel_limit']._serialized_options = b'\030\001'
+  _EDGE_ANNOTATIONS.fields_by_name['flat_ground']._options = None
+  _EDGE_ANNOTATIONS.fields_by_name['flat_ground']._serialized_options = b'\030\001'
   _EDGE_ANNOTATIONS.fields_by_name['ground_mu_hint']._options = None
   _EDGE_ANNOTATIONS.fields_by_name['ground_mu_hint']._serialized_options = b'\030\001'
   _EDGE_ANNOTATIONS.fields_by_name['grated_floor']._options = None
   _EDGE_ANNOTATIONS.fields_by_name['grated_floor']._serialized_options = b'\030\001'
   _EDGESNAPSHOT_AREACALLBACKSENTRY._options = None
   _EDGESNAPSHOT_AREACALLBACKSENTRY._serialized_options = b'8\001'
-  _ANNOTATIONSTATE._serialized_start=5358
-  _ANNOTATIONSTATE._serialized_end=5458
-  _WAYPOINT._serialized_start=469
-  _WAYPOINT._serialized_end=1528
-  _WAYPOINT_ANNOTATIONS._serialized_start=628
-  _WAYPOINT_ANNOTATIONS._serialized_end=1369
-  _WAYPOINT_ANNOTATIONS_LOCALIZEREGION._serialized_start=979
-  _WAYPOINT_ANNOTATIONS_LOCALIZEREGION._serialized_end=1369
-  _WAYPOINT_ANNOTATIONS_LOCALIZEREGION_DEFAULT._serialized_start=1312
-  _WAYPOINT_ANNOTATIONS_LOCALIZEREGION_DEFAULT._serialized_end=1321
-  _WAYPOINT_ANNOTATIONS_LOCALIZEREGION_EMPTY._serialized_start=1323
-  _WAYPOINT_ANNOTATIONS_LOCALIZEREGION_EMPTY._serialized_end=1330
-  _WAYPOINT_ANNOTATIONS_LOCALIZEREGION_CIRCLE2D._serialized_start=1332
-  _WAYPOINT_ANNOTATIONS_LOCALIZEREGION_CIRCLE2D._serialized_end=1359
-  _WAYPOINT_WAYPOINTSOURCE._serialized_start=1372
-  _WAYPOINT_WAYPOINTSOURCE._serialized_end=1528
-  _CLIENTMETADATA._serialized_start=1531
-  _CLIENTMETADATA._serialized_end=1667
-  _WAYPOINTSNAPSHOT._serialized_start=1670
-  _WAYPOINTSNAPSHOT._serialized_end=2221
-  _EDGE._serialized_start=2224
-  _EDGE._serialized_end=4290
-  _EDGE_ID._serialized_start=2401
-  _EDGE_ID._serialized_end=2449
-  _EDGE_ANNOTATIONS._serialized_start=2452
-  _EDGE_ANNOTATIONS._serialized_end=4078
-  _EDGE_ANNOTATIONS_STAIRDATA._serialized_start=3461
-  _EDGE_ANNOTATIONS_STAIRDATA._serialized_end=3585
-  _EDGE_ANNOTATIONS_AREACALLBACKSENTRY._serialized_start=3587
-  _EDGE_ANNOTATIONS_AREACALLBACKSENTRY._serialized_end=3681
-  _EDGE_ANNOTATIONS_DIRECTIONCONSTRAINT._serialized_start=3684
-  _EDGE_ANNOTATIONS_DIRECTIONCONSTRAINT._serialized_end=3872
-  _EDGE_ANNOTATIONS_PATHFOLLOWINGMODE._serialized_start=3874
-  _EDGE_ANNOTATIONS_PATHFOLLOWINGMODE._serialized_end=3961
-  _EDGE_ANNOTATIONS_GROUNDCLUTTERAVOIDANCEMODE._serialized_start=3963
-  _EDGE_ANNOTATIONS_GROUNDCLUTTERAVOIDANCEMODE._serialized_end=4078
-  _EDGE_EDGESOURCE._serialized_start=4081
-  _EDGE_EDGESOURCE._serialized_end=4290
-  _EDGESNAPSHOT._serialized_start=4293
-  _EDGESNAPSHOT._serialized_end=4797
-  _EDGESNAPSHOT_STANCE._serialized_start=4461
-  _EDGESNAPSHOT_STANCE._serialized_end=4703
-  _EDGESNAPSHOT_AREACALLBACKSENTRY._serialized_start=4705
-  _EDGESNAPSHOT_AREACALLBACKSENTRY._serialized_end=4797
-  _ANCHOR._serialized_start=4799
-  _ANCHOR._serialized_end=4869
-  _ANCHOREDWORLDOBJECT._serialized_start=4871
-  _ANCHOREDWORLDOBJECT._serialized_end=4952
-  _ANCHORING._serialized_start=4954
-  _ANCHORING._serialized_end=5072
-  _AREACALLBACKREGION._serialized_start=5074
-  _AREACALLBACKREGION._serialized_end=5137
-  _AREACALLBACKDATA._serialized_start=5139
-  _AREACALLBACKDATA._serialized_end=5200
-  _GRAPH._serialized_start=5203
-  _GRAPH._serialized_end=5356
+  _ANNOTATIONSTATE._serialized_start=6294
+  _ANNOTATIONSTATE._serialized_end=6394
+  _WAYPOINT._serialized_start=489
+  _WAYPOINT._serialized_end=1789
+  _WAYPOINT_ANNOTATIONS._serialized_start=648
+  _WAYPOINT_ANNOTATIONS._serialized_end=1630
+  _WAYPOINT_ANNOTATIONS_LOCALIZEREGION._serialized_start=1094
+  _WAYPOINT_ANNOTATIONS_LOCALIZEREGION._serialized_end=1484
+  _WAYPOINT_ANNOTATIONS_LOCALIZEREGION_DEFAULT._serialized_start=1427
+  _WAYPOINT_ANNOTATIONS_LOCALIZEREGION_DEFAULT._serialized_end=1436
+  _WAYPOINT_ANNOTATIONS_LOCALIZEREGION_EMPTY._serialized_start=1438
+  _WAYPOINT_ANNOTATIONS_LOCALIZEREGION_EMPTY._serialized_end=1445
+  _WAYPOINT_ANNOTATIONS_LOCALIZEREGION_CIRCLE2D._serialized_start=1447
+  _WAYPOINT_ANNOTATIONS_LOCALIZEREGION_CIRCLE2D._serialized_end=1474
+  _WAYPOINT_ANNOTATIONS_LOOPCLOSURESETTINGS._serialized_start=1487
+  _WAYPOINT_ANNOTATIONS_LOOPCLOSURESETTINGS._serialized_end=1630
+  _WAYPOINT_WAYPOINTSOURCE._serialized_start=1633
+  _WAYPOINT_WAYPOINTSOURCE._serialized_end=1789
+  _CLIENTMETADATA._serialized_start=1792
+  _CLIENTMETADATA._serialized_end=1928
+  _WAYPOINTSNAPSHOT._serialized_start=1931
+  _WAYPOINTSNAPSHOT._serialized_end=2482
+  _EDGE._serialized_start=2485
+  _EDGE._serialized_end=4658
+  _EDGE_ID._serialized_start=2662
+  _EDGE_ID._serialized_end=2710
+  _EDGE_ANNOTATIONS._serialized_start=2713
+  _EDGE_ANNOTATIONS._serialized_end=4416
+  _EDGE_ANNOTATIONS_STAIRDATA._serialized_start=3727
+  _EDGE_ANNOTATIONS_STAIRDATA._serialized_end=3923
+  _EDGE_ANNOTATIONS_AREACALLBACKSENTRY._serialized_start=3925
+  _EDGE_ANNOTATIONS_AREACALLBACKSENTRY._serialized_end=4019
+  _EDGE_ANNOTATIONS_DIRECTIONCONSTRAINT._serialized_start=4022
+  _EDGE_ANNOTATIONS_DIRECTIONCONSTRAINT._serialized_end=4210
+  _EDGE_ANNOTATIONS_PATHFOLLOWINGMODE._serialized_start=4212
+  _EDGE_ANNOTATIONS_PATHFOLLOWINGMODE._serialized_end=4299
+  _EDGE_ANNOTATIONS_GROUNDCLUTTERAVOIDANCEMODE._serialized_start=4301
+  _EDGE_ANNOTATIONS_GROUNDCLUTTERAVOIDANCEMODE._serialized_end=4416
+  _EDGE_EDGESOURCE._serialized_start=4419
+  _EDGE_EDGESOURCE._serialized_end=4658
+  _EDGESNAPSHOT._serialized_start=4661
+  _EDGESNAPSHOT._serialized_end=5165
+  _EDGESNAPSHOT_STANCE._serialized_start=4829
+  _EDGESNAPSHOT_STANCE._serialized_end=5071
+  _EDGESNAPSHOT_AREACALLBACKSENTRY._serialized_start=5073
+  _EDGESNAPSHOT_AREACALLBACKSENTRY._serialized_end=5165
+  _ANCHOR._serialized_start=5167
+  _ANCHOR._serialized_end=5237
+  _ANCHOREDWORLDOBJECT._serialized_start=5239
+  _ANCHOREDWORLDOBJECT._serialized_end=5320
+  _ANCHORING._serialized_start=5322
+  _ANCHORING._serialized_end=5440
+  _AREACALLBACKREGION._serialized_start=5442
+  _AREACALLBACKREGION._serialized_end=5568
+  _GRAPH._serialized_start=5571
+  _GRAPH._serialized_end=5724
+  _MAPSTATS._serialized_start=5727
+  _MAPSTATS._serialized_end=6292
+  _MAPSTATS_STAT._serialized_start=6252
+  _MAPSTATS_STAT._serialized_end=6292
 # @@protoc_insertion_point(module_scope)
```

## bosdyn/api/graph_nav/map_processing_pb2.py

```diff
@@ -14,15 +14,15 @@
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from bosdyn.api import geometry_pb2 as bosdyn_dot_api_dot_geometry__pb2
 from bosdyn.api import header_pb2 as bosdyn_dot_api_dot_header__pb2
 from bosdyn.api.graph_nav import map_pb2 as bosdyn_dot_api_dot_graph__nav_dot_map__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)bosdyn/api/graph_nav/map_processing.proto\x12\x14\x62osdyn.api.graph_nav\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x19\x62osdyn/api/geometry.proto\x1a\x17\x62osdyn/api/header.proto\x1a\x1e\x62osdyn/api/graph_nav/map.proto\"\xd9\r\n\x16ProcessTopologyRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x43\n\x06params\x18\x02 \x01(\x0b\x32\x33.bosdyn.api.graph_nav.ProcessTopologyRequest.Params\x12\x1c\n\x14modify_map_on_server\x18\x03 \x01(\x08\x1a{\n\tICPParams\x12.\n\ticp_iters\x18\x01 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\x12>\n\x18max_point_match_distance\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x1a\xf5\x02\n\x19OdometryLoopClosureParams\x12\x42\n\x1cmax_loop_closure_path_length\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x42\n\x1cmin_loop_closure_path_length\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x44\n\x1emax_loop_closure_height_change\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x42\n\x1cmax_loop_closure_edge_length\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x46\n!num_extra_loop_closure_iterations\x18\x05 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\x1a\xa6\x02\n\x19\x46iducialLoopClosureParams\x12\x42\n\x1cmin_loop_closure_path_length\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x42\n\x1cmax_loop_closure_edge_length\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12;\n\x15max_fiducial_distance\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x44\n\x1emax_loop_closure_height_change\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x1a\xe4\x01\n\x17\x43ollisionCheckingParams\x12=\n\x19\x63heck_edges_for_collision\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x42\n\x1c\x63ollision_check_robot_radius\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x46\n collision_check_height_variation\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x1a\xab\x04\n\x06Params\x12<\n\x18\x64o_odometry_loop_closure\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12l\n\x1codometry_loop_closure_params\x18\x02 \x01(\x0b\x32\x46.bosdyn.api.graph_nav.ProcessTopologyRequest.OdometryLoopClosureParams\x12J\n\nicp_params\x18\x03 \x01(\x0b\x32\x36.bosdyn.api.graph_nav.ProcessTopologyRequest.ICPParams\x12<\n\x18\x64o_fiducial_loop_closure\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12l\n\x1c\x66iducial_loop_closure_params\x18\x05 \x01(\x0b\x32\x46.bosdyn.api.graph_nav.ProcessTopologyRequest.FiducialLoopClosureParams\x12\x64\n\x16\x63ollision_check_params\x18\x06 \x01(\x0b\x32\x44.bosdyn.api.graph_nav.ProcessTopologyRequest.CollisionCheckingParams\x12\x17\n\x0ftimeout_seconds\x18\x07 \x01(\x01\"\xcb\x03\n\x17ProcessTopologyResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x44\n\x06status\x18\x02 \x01(\x0e\x32\x34.bosdyn.api.graph_nav.ProcessTopologyResponse.Status\x12\x31\n\x0cnew_subgraph\x18\x03 \x01(\x0b\x32\x1b.bosdyn.api.graph_nav.Graph\x12\"\n\x1amap_on_server_was_modified\x18\x04 \x01(\x08\x12\x1c\n\x14missing_snapshot_ids\x18\n \x03(\t\x12\x1c\n\x14missing_waypoint_ids\x18\x0b \x03(\t\x12\x11\n\ttimed_out\x18\x0c \x01(\x08\"\x97\x01\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12%\n!STATUS_MISSING_WAYPOINT_SNAPSHOTS\x10\x02\x12\x18\n\x14STATUS_INVALID_GRAPH\x10\x03\x12)\n%STATUS_MAP_MODIFIED_DURING_PROCESSING\x10\x04\"V\n\nPoseBounds\x12\x10\n\x08x_bounds\x18\x01 \x01(\x01\x12\x10\n\x08y_bounds\x18\x02 \x01(\x01\x12\x10\n\x08z_bounds\x18\x03 \x01(\x01\x12\x12\n\nyaw_bounds\x18\x04 \x01(\x01\"\x9a\x01\n\x15\x41nchorHintUncertainty\x12\x33\n\x0ese3_covariance\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.SE3CovarianceH\x00\x12=\n\x11\x63onfidence_bounds\x18\x02 \x01(\x0b\x32 .bosdyn.api.graph_nav.PoseBoundsH\x00\x42\r\n\x0buncertainty\"\xeb\x01\n\x12WaypointAnchorHint\x12\x35\n\x0fwaypoint_anchor\x18\x01 \x01(\x0b\x32\x1c.bosdyn.api.graph_nav.Anchor\x12T\n\x1fseed_tform_waypoint_uncertainty\x18\x02 \x01(\x0b\x32+.bosdyn.api.graph_nav.AnchorHintUncertainty\x12H\n\x1eseed_tform_waypoint_constraint\x18\x03 \x01(\x0b\x32 .bosdyn.api.graph_nav.PoseBounds\"\xf5\x01\n\x15WorldObjectAnchorHint\x12@\n\robject_anchor\x18\x01 \x01(\x0b\x32).bosdyn.api.graph_nav.AnchoredWorldObject\x12R\n\x1dseed_tform_object_uncertainty\x18\x02 \x01(\x0b\x32+.bosdyn.api.graph_nav.AnchorHintUncertainty\x12\x46\n\x1cseed_tform_object_constraint\x18\x03 \x01(\x0b\x32 .bosdyn.api.graph_nav.PoseBounds\"\x97\x01\n\rAnchoringHint\x12\x42\n\x10waypoint_anchors\x18\x01 \x03(\x0b\x32(.bosdyn.api.graph_nav.WaypointAnchorHint\x12\x42\n\rworld_objects\x18\x02 \x03(\x0b\x32+.bosdyn.api.graph_nav.WorldObjectAnchorHint\"\x86\n\n\x17ProcessAnchoringRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x44\n\x06params\x18\x02 \x01(\x0b\x32\x34.bosdyn.api.graph_nav.ProcessAnchoringRequest.Params\x12\x39\n\x0cinitial_hint\x18\x03 \x01(\x0b\x32#.bosdyn.api.graph_nav.AnchoringHint\x12\"\n\x1amodify_anchoring_on_server\x18\x04 \x01(\x08\x12#\n\x1bstream_intermediate_results\x18\x05 \x01(\x08\x1a\xf5\x07\n\x06Params\x12^\n\x10optimizer_params\x18\x01 \x01(\x0b\x32\x44.bosdyn.api.graph_nav.ProcessAnchoringRequest.Params.OptimizerParams\x12\x62\n\x12measurement_params\x18\x02 \x01(\x0b\x32\x46.bosdyn.api.graph_nav.ProcessAnchoringRequest.Params.MeasurementParams\x12M\n\x07weights\x18\x03 \x01(\x0b\x32<.bosdyn.api.graph_nav.ProcessAnchoringRequest.Params.Weights\x12?\n\x1boptimize_existing_anchoring\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12+\n\x11gravity_ewrt_seed\x18\x05 \x01(\x0b\x32\x10.bosdyn.api.Vec3\x1ay\n\x0fOptimizerParams\x12.\n\tmax_iters\x18\x01 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\x12\x36\n\x10max_time_seconds\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x1a\xb6\x02\n\x11MeasurementParams\x12:\n\x16use_kinematic_odometry\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x37\n\x13use_visual_odometry\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12>\n\x1ause_gyroscope_measurements\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x35\n\x11use_loop_closures\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x35\n\x11use_world_objects\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x1a\xb5\x01\n\x07Weights\x12!\n\x19kinematic_odometry_weight\x18\x01 \x01(\x01\x12\x1e\n\x16visual_odometry_weight\x18\x02 \x01(\x01\x12\x1b\n\x13world_object_weight\x18\x03 \x01(\x01\x12\x13\n\x0bhint_weight\x18\x04 \x01(\x01\x12\x18\n\x10gyroscope_weight\x18\x05 \x01(\x01\x12\x1b\n\x13loop_closure_weight\x18\x06 \x01(\x01\"\xcf\x07\n\x18ProcessAnchoringResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x45\n\x06status\x18\x02 \x01(\x0e\x32\x35.bosdyn.api.graph_nav.ProcessAnchoringResponse.Status\x12\x36\n\x10waypoint_results\x18\x03 \x03(\x0b\x32\x1c.bosdyn.api.graph_nav.Anchor\x12G\n\x14world_object_results\x18\x04 \x03(\x0b\x32).bosdyn.api.graph_nav.AnchoredWorldObject\x12(\n anchoring_on_server_was_modified\x18\x05 \x01(\x08\x12\x11\n\titeration\x18\x06 \x01(\x05\x12\x0c\n\x04\x63ost\x18\x07 \x01(\x01\x12\x17\n\x0f\x66inal_iteration\x18\x08 \x01(\x08\x12O\n\x1dviolated_waypoint_constraints\x18\t \x03(\x0b\x32(.bosdyn.api.graph_nav.WaypointAnchorHint\x12P\n\x1bviolated_object_constraints\x18\n \x03(\x0b\x32+.bosdyn.api.graph_nav.WorldObjectAnchorHint\x12\x1c\n\x14missing_snapshot_ids\x18\x0b \x03(\t\x12\x1c\n\x14missing_waypoint_ids\x18\x0c \x03(\t\x12\x15\n\rinvalid_hints\x18\r \x03(\t\"\xe4\x02\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12%\n!STATUS_MISSING_WAYPOINT_SNAPSHOTS\x10\x02\x12\x18\n\x14STATUS_INVALID_GRAPH\x10\x03\x12\x1f\n\x1bSTATUS_OPTIMIZATION_FAILURE\x10\x04\x12\x19\n\x15STATUS_INVALID_PARAMS\x10\x05\x12\x1f\n\x1bSTATUS_CONSTRAINT_VIOLATION\x10\x06\x12\x19\n\x15STATUS_MAX_ITERATIONS\x10\x07\x12\x13\n\x0fSTATUS_MAX_TIME\x10\x08\x12\x18\n\x14STATUS_INVALID_HINTS\x10\t\x12)\n%STATUS_MAP_MODIFIED_DURING_PROCESSING\x10\n\x12$\n STATUS_INVALID_GRAVITY_ALIGNMENT\x10\x0b\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)bosdyn/api/graph_nav/map_processing.proto\x12\x14\x62osdyn.api.graph_nav\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x19\x62osdyn/api/geometry.proto\x1a\x17\x62osdyn/api/header.proto\x1a\x1e\x62osdyn/api/graph_nav/map.proto\"\xbb\x0e\n\x16ProcessTopologyRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x43\n\x06params\x18\x02 \x01(\x0b\x32\x33.bosdyn.api.graph_nav.ProcessTopologyRequest.Params\x12\x1c\n\x14modify_map_on_server\x18\x03 \x01(\x08\x1a{\n\tICPParams\x12.\n\ticp_iters\x18\x01 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\x12>\n\x18max_point_match_distance\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x1a\xa6\x03\n\x19OdometryLoopClosureParams\x12\x42\n\x1cmax_loop_closure_path_length\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x42\n\x1cmin_loop_closure_path_length\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x44\n\x1emax_loop_closure_height_change\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x42\n\x1cmax_loop_closure_edge_length\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x46\n!num_extra_loop_closure_iterations\x18\x05 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\x12/\n\x0bprune_edges\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x1a\xd7\x02\n\x19\x46iducialLoopClosureParams\x12\x42\n\x1cmin_loop_closure_path_length\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x42\n\x1cmax_loop_closure_edge_length\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12;\n\x15max_fiducial_distance\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x44\n\x1emax_loop_closure_height_change\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12/\n\x0bprune_edges\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x1a\xe4\x01\n\x17\x43ollisionCheckingParams\x12=\n\x19\x63heck_edges_for_collision\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x42\n\x1c\x63ollision_check_robot_radius\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x46\n collision_check_height_variation\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x1a\xab\x04\n\x06Params\x12<\n\x18\x64o_odometry_loop_closure\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12l\n\x1codometry_loop_closure_params\x18\x02 \x01(\x0b\x32\x46.bosdyn.api.graph_nav.ProcessTopologyRequest.OdometryLoopClosureParams\x12J\n\nicp_params\x18\x03 \x01(\x0b\x32\x36.bosdyn.api.graph_nav.ProcessTopologyRequest.ICPParams\x12<\n\x18\x64o_fiducial_loop_closure\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12l\n\x1c\x66iducial_loop_closure_params\x18\x05 \x01(\x0b\x32\x46.bosdyn.api.graph_nav.ProcessTopologyRequest.FiducialLoopClosureParams\x12\x64\n\x16\x63ollision_check_params\x18\x06 \x01(\x0b\x32\x44.bosdyn.api.graph_nav.ProcessTopologyRequest.CollisionCheckingParams\x12\x17\n\x0ftimeout_seconds\x18\x07 \x01(\x01\"\xcb\x03\n\x17ProcessTopologyResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x44\n\x06status\x18\x02 \x01(\x0e\x32\x34.bosdyn.api.graph_nav.ProcessTopologyResponse.Status\x12\x31\n\x0cnew_subgraph\x18\x03 \x01(\x0b\x32\x1b.bosdyn.api.graph_nav.Graph\x12\"\n\x1amap_on_server_was_modified\x18\x04 \x01(\x08\x12\x1c\n\x14missing_snapshot_ids\x18\n \x03(\t\x12\x1c\n\x14missing_waypoint_ids\x18\x0b \x03(\t\x12\x11\n\ttimed_out\x18\x0c \x01(\x08\"\x97\x01\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12%\n!STATUS_MISSING_WAYPOINT_SNAPSHOTS\x10\x02\x12\x18\n\x14STATUS_INVALID_GRAPH\x10\x03\x12)\n%STATUS_MAP_MODIFIED_DURING_PROCESSING\x10\x04\"V\n\nPoseBounds\x12\x10\n\x08x_bounds\x18\x01 \x01(\x01\x12\x10\n\x08y_bounds\x18\x02 \x01(\x01\x12\x10\n\x08z_bounds\x18\x03 \x01(\x01\x12\x12\n\nyaw_bounds\x18\x04 \x01(\x01\"\x9a\x01\n\x15\x41nchorHintUncertainty\x12\x33\n\x0ese3_covariance\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.SE3CovarianceH\x00\x12=\n\x11\x63onfidence_bounds\x18\x02 \x01(\x0b\x32 .bosdyn.api.graph_nav.PoseBoundsH\x00\x42\r\n\x0buncertainty\"\xeb\x01\n\x12WaypointAnchorHint\x12\x35\n\x0fwaypoint_anchor\x18\x01 \x01(\x0b\x32\x1c.bosdyn.api.graph_nav.Anchor\x12T\n\x1fseed_tform_waypoint_uncertainty\x18\x02 \x01(\x0b\x32+.bosdyn.api.graph_nav.AnchorHintUncertainty\x12H\n\x1eseed_tform_waypoint_constraint\x18\x03 \x01(\x0b\x32 .bosdyn.api.graph_nav.PoseBounds\"\xf5\x01\n\x15WorldObjectAnchorHint\x12@\n\robject_anchor\x18\x01 \x01(\x0b\x32).bosdyn.api.graph_nav.AnchoredWorldObject\x12R\n\x1dseed_tform_object_uncertainty\x18\x02 \x01(\x0b\x32+.bosdyn.api.graph_nav.AnchorHintUncertainty\x12\x46\n\x1cseed_tform_object_constraint\x18\x03 \x01(\x0b\x32 .bosdyn.api.graph_nav.PoseBounds\"\x97\x01\n\rAnchoringHint\x12\x42\n\x10waypoint_anchors\x18\x01 \x03(\x0b\x32(.bosdyn.api.graph_nav.WaypointAnchorHint\x12\x42\n\rworld_objects\x18\x02 \x03(\x0b\x32+.bosdyn.api.graph_nav.WorldObjectAnchorHint\"\x86\n\n\x17ProcessAnchoringRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x44\n\x06params\x18\x02 \x01(\x0b\x32\x34.bosdyn.api.graph_nav.ProcessAnchoringRequest.Params\x12\x39\n\x0cinitial_hint\x18\x03 \x01(\x0b\x32#.bosdyn.api.graph_nav.AnchoringHint\x12\"\n\x1amodify_anchoring_on_server\x18\x04 \x01(\x08\x12#\n\x1bstream_intermediate_results\x18\x05 \x01(\x08\x1a\xf5\x07\n\x06Params\x12^\n\x10optimizer_params\x18\x01 \x01(\x0b\x32\x44.bosdyn.api.graph_nav.ProcessAnchoringRequest.Params.OptimizerParams\x12\x62\n\x12measurement_params\x18\x02 \x01(\x0b\x32\x46.bosdyn.api.graph_nav.ProcessAnchoringRequest.Params.MeasurementParams\x12M\n\x07weights\x18\x03 \x01(\x0b\x32<.bosdyn.api.graph_nav.ProcessAnchoringRequest.Params.Weights\x12?\n\x1boptimize_existing_anchoring\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12+\n\x11gravity_ewrt_seed\x18\x05 \x01(\x0b\x32\x10.bosdyn.api.Vec3\x1ay\n\x0fOptimizerParams\x12.\n\tmax_iters\x18\x01 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\x12\x36\n\x10max_time_seconds\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x1a\xb6\x02\n\x11MeasurementParams\x12:\n\x16use_kinematic_odometry\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x37\n\x13use_visual_odometry\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12>\n\x1ause_gyroscope_measurements\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x35\n\x11use_loop_closures\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x35\n\x11use_world_objects\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x1a\xb5\x01\n\x07Weights\x12!\n\x19kinematic_odometry_weight\x18\x01 \x01(\x01\x12\x1e\n\x16visual_odometry_weight\x18\x02 \x01(\x01\x12\x1b\n\x13world_object_weight\x18\x03 \x01(\x01\x12\x13\n\x0bhint_weight\x18\x04 \x01(\x01\x12\x18\n\x10gyroscope_weight\x18\x05 \x01(\x01\x12\x1b\n\x13loop_closure_weight\x18\x06 \x01(\x01\"\x8a\x08\n\x18ProcessAnchoringResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x45\n\x06status\x18\x02 \x01(\x0e\x32\x35.bosdyn.api.graph_nav.ProcessAnchoringResponse.Status\x12\x36\n\x10waypoint_results\x18\x03 \x03(\x0b\x32\x1c.bosdyn.api.graph_nav.Anchor\x12G\n\x14world_object_results\x18\x04 \x03(\x0b\x32).bosdyn.api.graph_nav.AnchoredWorldObject\x12(\n anchoring_on_server_was_modified\x18\x05 \x01(\x08\x12\x11\n\titeration\x18\x06 \x01(\x05\x12\x0c\n\x04\x63ost\x18\x07 \x01(\x01\x12\x17\n\x0f\x66inal_iteration\x18\x08 \x01(\x08\x12O\n\x1dviolated_waypoint_constraints\x18\t \x03(\x0b\x32(.bosdyn.api.graph_nav.WaypointAnchorHint\x12P\n\x1bviolated_object_constraints\x18\n \x03(\x0b\x32+.bosdyn.api.graph_nav.WorldObjectAnchorHint\x12\x1c\n\x14missing_snapshot_ids\x18\x0b \x03(\t\x12\x1c\n\x14missing_waypoint_ids\x18\x0c \x03(\t\x12\x15\n\rinvalid_hints\x18\r \x03(\t\x12\x39\n\x12inconsistent_edges\x18\x0e \x03(\x0b\x32\x1d.bosdyn.api.graph_nav.Edge.Id\"\xe4\x02\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12%\n!STATUS_MISSING_WAYPOINT_SNAPSHOTS\x10\x02\x12\x18\n\x14STATUS_INVALID_GRAPH\x10\x03\x12\x1f\n\x1bSTATUS_OPTIMIZATION_FAILURE\x10\x04\x12\x19\n\x15STATUS_INVALID_PARAMS\x10\x05\x12\x1f\n\x1bSTATUS_CONSTRAINT_VIOLATION\x10\x06\x12\x19\n\x15STATUS_MAX_ITERATIONS\x10\x07\x12\x13\n\x0fSTATUS_MAX_TIME\x10\x08\x12\x18\n\x14STATUS_INVALID_HINTS\x10\t\x12)\n%STATUS_MAP_MODIFIED_DURING_PROCESSING\x10\n\x12$\n STATUS_INVALID_GRAVITY_ALIGNMENT\x10\x0b\x62\x06proto3')
 
 
 
 _PROCESSTOPOLOGYREQUEST = DESCRIPTOR.message_types_by_name['ProcessTopologyRequest']
 _PROCESSTOPOLOGYREQUEST_ICPPARAMS = _PROCESSTOPOLOGYREQUEST.nested_types_by_name['ICPParams']
 _PROCESSTOPOLOGYREQUEST_ODOMETRYLOOPCLOSUREPARAMS = _PROCESSTOPOLOGYREQUEST.nested_types_by_name['OdometryLoopClosureParams']
 _PROCESSTOPOLOGYREQUEST_FIDUCIALLOOPCLOSUREPARAMS = _PROCESSTOPOLOGYREQUEST.nested_types_by_name['FiducialLoopClosureParams']
@@ -177,47 +177,47 @@
   })
 _sym_db.RegisterMessage(ProcessAnchoringResponse)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _PROCESSTOPOLOGYREQUEST._serialized_start=184
-  _PROCESSTOPOLOGYREQUEST._serialized_end=1937
+  _PROCESSTOPOLOGYREQUEST._serialized_end=2035
   _PROCESSTOPOLOGYREQUEST_ICPPARAMS._serialized_start=352
   _PROCESSTOPOLOGYREQUEST_ICPPARAMS._serialized_end=475
   _PROCESSTOPOLOGYREQUEST_ODOMETRYLOOPCLOSUREPARAMS._serialized_start=478
-  _PROCESSTOPOLOGYREQUEST_ODOMETRYLOOPCLOSUREPARAMS._serialized_end=851
-  _PROCESSTOPOLOGYREQUEST_FIDUCIALLOOPCLOSUREPARAMS._serialized_start=854
-  _PROCESSTOPOLOGYREQUEST_FIDUCIALLOOPCLOSUREPARAMS._serialized_end=1148
-  _PROCESSTOPOLOGYREQUEST_COLLISIONCHECKINGPARAMS._serialized_start=1151
-  _PROCESSTOPOLOGYREQUEST_COLLISIONCHECKINGPARAMS._serialized_end=1379
-  _PROCESSTOPOLOGYREQUEST_PARAMS._serialized_start=1382
-  _PROCESSTOPOLOGYREQUEST_PARAMS._serialized_end=1937
-  _PROCESSTOPOLOGYRESPONSE._serialized_start=1940
-  _PROCESSTOPOLOGYRESPONSE._serialized_end=2399
-  _PROCESSTOPOLOGYRESPONSE_STATUS._serialized_start=2248
-  _PROCESSTOPOLOGYRESPONSE_STATUS._serialized_end=2399
-  _POSEBOUNDS._serialized_start=2401
-  _POSEBOUNDS._serialized_end=2487
-  _ANCHORHINTUNCERTAINTY._serialized_start=2490
-  _ANCHORHINTUNCERTAINTY._serialized_end=2644
-  _WAYPOINTANCHORHINT._serialized_start=2647
-  _WAYPOINTANCHORHINT._serialized_end=2882
-  _WORLDOBJECTANCHORHINT._serialized_start=2885
-  _WORLDOBJECTANCHORHINT._serialized_end=3130
-  _ANCHORINGHINT._serialized_start=3133
-  _ANCHORINGHINT._serialized_end=3284
-  _PROCESSANCHORINGREQUEST._serialized_start=3287
-  _PROCESSANCHORINGREQUEST._serialized_end=4573
-  _PROCESSANCHORINGREQUEST_PARAMS._serialized_start=3560
-  _PROCESSANCHORINGREQUEST_PARAMS._serialized_end=4573
-  _PROCESSANCHORINGREQUEST_PARAMS_OPTIMIZERPARAMS._serialized_start=3955
-  _PROCESSANCHORINGREQUEST_PARAMS_OPTIMIZERPARAMS._serialized_end=4076
-  _PROCESSANCHORINGREQUEST_PARAMS_MEASUREMENTPARAMS._serialized_start=4079
-  _PROCESSANCHORINGREQUEST_PARAMS_MEASUREMENTPARAMS._serialized_end=4389
-  _PROCESSANCHORINGREQUEST_PARAMS_WEIGHTS._serialized_start=4392
-  _PROCESSANCHORINGREQUEST_PARAMS_WEIGHTS._serialized_end=4573
-  _PROCESSANCHORINGRESPONSE._serialized_start=4576
-  _PROCESSANCHORINGRESPONSE._serialized_end=5551
-  _PROCESSANCHORINGRESPONSE_STATUS._serialized_start=5195
-  _PROCESSANCHORINGRESPONSE_STATUS._serialized_end=5551
+  _PROCESSTOPOLOGYREQUEST_ODOMETRYLOOPCLOSUREPARAMS._serialized_end=900
+  _PROCESSTOPOLOGYREQUEST_FIDUCIALLOOPCLOSUREPARAMS._serialized_start=903
+  _PROCESSTOPOLOGYREQUEST_FIDUCIALLOOPCLOSUREPARAMS._serialized_end=1246
+  _PROCESSTOPOLOGYREQUEST_COLLISIONCHECKINGPARAMS._serialized_start=1249
+  _PROCESSTOPOLOGYREQUEST_COLLISIONCHECKINGPARAMS._serialized_end=1477
+  _PROCESSTOPOLOGYREQUEST_PARAMS._serialized_start=1480
+  _PROCESSTOPOLOGYREQUEST_PARAMS._serialized_end=2035
+  _PROCESSTOPOLOGYRESPONSE._serialized_start=2038
+  _PROCESSTOPOLOGYRESPONSE._serialized_end=2497
+  _PROCESSTOPOLOGYRESPONSE_STATUS._serialized_start=2346
+  _PROCESSTOPOLOGYRESPONSE_STATUS._serialized_end=2497
+  _POSEBOUNDS._serialized_start=2499
+  _POSEBOUNDS._serialized_end=2585
+  _ANCHORHINTUNCERTAINTY._serialized_start=2588
+  _ANCHORHINTUNCERTAINTY._serialized_end=2742
+  _WAYPOINTANCHORHINT._serialized_start=2745
+  _WAYPOINTANCHORHINT._serialized_end=2980
+  _WORLDOBJECTANCHORHINT._serialized_start=2983
+  _WORLDOBJECTANCHORHINT._serialized_end=3228
+  _ANCHORINGHINT._serialized_start=3231
+  _ANCHORINGHINT._serialized_end=3382
+  _PROCESSANCHORINGREQUEST._serialized_start=3385
+  _PROCESSANCHORINGREQUEST._serialized_end=4671
+  _PROCESSANCHORINGREQUEST_PARAMS._serialized_start=3658
+  _PROCESSANCHORINGREQUEST_PARAMS._serialized_end=4671
+  _PROCESSANCHORINGREQUEST_PARAMS_OPTIMIZERPARAMS._serialized_start=4053
+  _PROCESSANCHORINGREQUEST_PARAMS_OPTIMIZERPARAMS._serialized_end=4174
+  _PROCESSANCHORINGREQUEST_PARAMS_MEASUREMENTPARAMS._serialized_start=4177
+  _PROCESSANCHORINGREQUEST_PARAMS_MEASUREMENTPARAMS._serialized_end=4487
+  _PROCESSANCHORINGREQUEST_PARAMS_WEIGHTS._serialized_start=4490
+  _PROCESSANCHORINGREQUEST_PARAMS_WEIGHTS._serialized_end=4671
+  _PROCESSANCHORINGRESPONSE._serialized_start=4674
+  _PROCESSANCHORINGRESPONSE._serialized_end=5708
+  _PROCESSANCHORINGRESPONSE_STATUS._serialized_start=5352
+  _PROCESSANCHORINGRESPONSE_STATUS._serialized_end=5708
 # @@protoc_insertion_point(module_scope)
```

## bosdyn/api/graph_nav/recording_pb2.py

```diff
@@ -8,23 +8,24 @@
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from bosdyn.api import header_pb2 as bosdyn_dot_api_dot_header__pb2
 from bosdyn.api import lease_pb2 as bosdyn_dot_api_dot_lease__pb2
 from bosdyn.api import license_pb2 as bosdyn_dot_api_dot_license__pb2
 from bosdyn.api import robot_state_pb2 as bosdyn_dot_api_dot_robot__state__pb2
 from bosdyn.api import world_object_pb2 as bosdyn_dot_api_dot_world__object__pb2
 from bosdyn.api.graph_nav import map_pb2 as bosdyn_dot_api_dot_graph__nav_dot_map__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$bosdyn/api/graph_nav/recording.proto\x12\x14\x62osdyn.api.graph_nav\x1a\x17\x62osdyn/api/header.proto\x1a\x16\x62osdyn/api/lease.proto\x1a\x18\x62osdyn/api/license.proto\x1a\x1c\x62osdyn/api/robot_state.proto\x1a\x1d\x62osdyn/api/world_object.proto\x1a\x1e\x62osdyn/api/graph_nav/map.proto\"\xb7\x01\n\x14RecordingEnvironment\x12\x13\n\x0bname_prefix\x18\x01 \x01(\t\x12H\n\x14waypoint_environment\x18\x02 \x01(\x0b\x32*.bosdyn.api.graph_nav.Waypoint.Annotations\x12@\n\x10\x65\x64ge_environment\x18\x03 \x01(\x0b\x32&.bosdyn.api.graph_nav.Edge.Annotations\"\xae\x01\n\x1eSetRecordingEnvironmentRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12?\n\x0b\x65nvironment\x18\x02 \x01(\x0b\x32*.bosdyn.api.graph_nav.RecordingEnvironment\x12 \n\x05lease\x18\x03 \x01(\x0b\x32\x11.bosdyn.api.Lease\"\x83\x01\n\x1fSetRecordingEnvironmentResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x34\n\x10lease_use_result\x18\x02 \x01(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\"\xca\x01\n\x15StartRecordingRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12 \n\x05lease\x18\x02 \x01(\x0b\x32\x11.bosdyn.api.Lease\x12I\n\x15recording_environment\x18\x03 \x01(\x0b\x32*.bosdyn.api.graph_nav.RecordingEnvironment\x12\x19\n\x11require_fiducials\x18\x04 \x03(\x05\"\xb7\x06\n\x16StartRecordingResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x38\n\x10\x63reated_waypoint\x18\x02 \x01(\x0b\x32\x1e.bosdyn.api.graph_nav.Waypoint\x12\x34\n\x10lease_use_result\x18\x03 \x01(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12\x43\n\x06status\x18\x04 \x01(\x0e\x32\x33.bosdyn.api.graph_nav.StartRecordingResponse.Status\x12\x19\n\x11missing_fiducials\x18\x05 \x03(\x05\x12\x1a\n\x12\x62\x61\x64_pose_fiducials\x18\x07 \x03(\x05\x12\x36\n\x0elicense_status\x18\x06 \x01(\x0e\x32\x1e.bosdyn.api.LicenseInfo.Status\x12\x36\n\x0eimpaired_state\x18\x08 \x01(\x0b\x32\x1e.bosdyn.api.RobotImpairedState\"\x94\x03\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12$\n STATUS_COULD_NOT_CREATE_WAYPOINT\x10\x02\x12\x1a\n\x16STATUS_FOLLOWING_ROUTE\x10\x03\x12(\n$STATUS_NOT_LOCALIZED_TO_EXISTING_MAP\x10\x04\x12\x1c\n\x18STATUS_MISSING_FIDUCIALS\x10\x05\x12 \n\x1cSTATUS_MAP_TOO_LARGE_LICENSE\x10\x06\x12\x30\n,STATUS_REMOTE_CLOUD_FAILURE_NOT_IN_DIRECTORY\x10\x07\x12\'\n#STATUS_REMOTE_CLOUD_FAILURE_NO_DATA\x10\x08\x12\x1f\n\x1bSTATUS_FIDUCIAL_POSE_NOT_OK\x10\t\x12$\n STATUS_TOO_FAR_FROM_EXISTING_MAP\x10\n\x12\x19\n\x15STATUS_ROBOT_IMPAIRED\x10\x0b\"c\n\x14StopRecordingRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12 \n\x05lease\x18\x02 \x01(\x0b\x32\x11.bosdyn.api.Lease\"\xca\x02\n\x15StopRecordingResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x42\n\x06status\x18\x02 \x01(\x0e\x32\x32.bosdyn.api.graph_nav.StopRecordingResponse.Status\x12#\n\x1b\x65rror_waypoint_localized_id\x18\x03 \x01(\t\x12\x34\n\x10lease_use_result\x18\x04 \x01(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\"f\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1f\n\x1bSTATUS_NOT_LOCALIZED_TO_END\x10\x02\x12\x18\n\x14STATUS_NOT_READY_YET\x10\x03\"\x91\x02\n\x15\x43reateWaypointRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x15\n\rwaypoint_name\x18\x02 \x01(\t\x12I\n\x15recording_environment\x18\x03 \x01(\x0b\x32*.bosdyn.api.graph_nav.RecordingEnvironment\x12 \n\x05lease\x18\x04 \x01(\x0b\x32\x11.bosdyn.api.Lease\x12\x19\n\x11require_fiducials\x18\x05 \x03(\x05\x12.\n\rworld_objects\x18\x06 \x03(\x0b\x32\x17.bosdyn.api.WorldObject\"\xc4\x05\n\x16\x43reateWaypointResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x38\n\x10\x63reated_waypoint\x18\x02 \x01(\x0b\x32\x1e.bosdyn.api.graph_nav.Waypoint\x12\x30\n\x0c\x63reated_edge\x18\x03 \x01(\x0b\x32\x1a.bosdyn.api.graph_nav.Edge\x12\x43\n\x06status\x18\x05 \x01(\x0e\x32\x33.bosdyn.api.graph_nav.CreateWaypointResponse.Status\x12\x34\n\x10lease_use_result\x18\x04 \x01(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12\x19\n\x11missing_fiducials\x18\x06 \x03(\x05\x12\x1a\n\x12\x62\x61\x64_pose_fiducials\x18\x08 \x03(\x05\x12\x36\n\x0elicense_status\x18\x07 \x01(\x0e\x32\x1e.bosdyn.api.LicenseInfo.Status\"\xa7\x02\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x18\n\x14STATUS_NOT_RECORDING\x10\x02\x12$\n STATUS_COULD_NOT_CREATE_WAYPOINT\x10\x03\x12\x1c\n\x18STATUS_MISSING_FIDUCIALS\x10\x04\x12 \n\x1cSTATUS_MAP_TOO_LARGE_LICENSE\x10\x05\x12\x30\n,STATUS_REMOTE_CLOUD_FAILURE_NOT_IN_DIRECTORY\x10\x06\x12\'\n#STATUS_REMOTE_CLOUD_FAILURE_NO_DATA\x10\x07\x12\x1f\n\x1bSTATUS_FIDUCIAL_POSE_NOT_OK\x10\x08\"\x8a\x01\n\x11\x43reateEdgeRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12(\n\x04\x65\x64ge\x18\x02 \x01(\x0b\x32\x1a.bosdyn.api.graph_nav.Edge\x12 \n\x05lease\x18\x03 \x01(\x0b\x32\x11.bosdyn.api.Lease\"\x86\x03\n\x12\x43reateEdgeResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12?\n\x06status\x18\x02 \x01(\x0e\x32/.bosdyn.api.graph_nav.CreateEdgeResponse.Status\x12\x37\n\x13\x65rror_existing_edge\x18\x03 \x01(\x0b\x32\x1a.bosdyn.api.graph_nav.Edge\x12\x34\n\x10lease_use_result\x18\x04 \x01(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\"\x93\x01\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x11\n\rSTATUS_EXISTS\x10\x02\x12\x18\n\x14STATUS_NOT_RECORDING\x10\x03\x12\x1b\n\x17STATUS_UNKNOWN_WAYPOINT\x10\x04\x12\x1c\n\x18STATUS_MISSING_TRANSFORM\x10\x05\"C\n\x16GetRecordStatusRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"\x91\x04\n\x17GetRecordStatusResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x14\n\x0cis_recording\x18\x02 \x01(\x08\x12I\n\x15recording_environment\x18\x03 \x01(\x0b\x32*.bosdyn.api.graph_nav.RecordingEnvironment\x12I\n\tmap_state\x18\x04 \x01(\x0e\x32\x36.bosdyn.api.graph_nav.GetRecordStatusResponse.MapState\x12\x44\n\x06status\x18\x05 \x01(\x0e\x32\x34.bosdyn.api.graph_nav.GetRecordStatusResponse.Status\x12\x36\n\x0eimpaired_state\x18\x06 \x01(\x0b\x32\x1e.bosdyn.api.RobotImpairedState\"X\n\x08MapState\x12\x15\n\x11MAP_STATE_UNKNOWN\x10\x00\x12\x10\n\x0cMAP_STATE_OK\x10\x01\x12#\n\x1fMAP_STATE_TOO_LARGE_FOR_LICENSE\x10\x02\"F\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x19\n\x15STATUS_ROBOT_IMPAIRED\x10\x02\x42\x10\x42\x0eRecordingProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$bosdyn/api/graph_nav/recording.proto\x12\x14\x62osdyn.api.graph_nav\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x17\x62osdyn/api/header.proto\x1a\x16\x62osdyn/api/lease.proto\x1a\x18\x62osdyn/api/license.proto\x1a\x1c\x62osdyn/api/robot_state.proto\x1a\x1d\x62osdyn/api/world_object.proto\x1a\x1e\x62osdyn/api/graph_nav/map.proto\"\xb7\x01\n\x14RecordingEnvironment\x12\x13\n\x0bname_prefix\x18\x01 \x01(\t\x12H\n\x14waypoint_environment\x18\x02 \x01(\x0b\x32*.bosdyn.api.graph_nav.Waypoint.Annotations\x12@\n\x10\x65\x64ge_environment\x18\x03 \x01(\x0b\x32&.bosdyn.api.graph_nav.Edge.Annotations\"\xae\x01\n\x1eSetRecordingEnvironmentRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12?\n\x0b\x65nvironment\x18\x02 \x01(\x0b\x32*.bosdyn.api.graph_nav.RecordingEnvironment\x12 \n\x05lease\x18\x03 \x01(\x0b\x32\x11.bosdyn.api.Lease\"\x83\x01\n\x1fSetRecordingEnvironmentResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x34\n\x10lease_use_result\x18\x02 \x01(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\"\x82\x02\n\x15StartRecordingRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12 \n\x05lease\x18\x02 \x01(\x0b\x32\x11.bosdyn.api.Lease\x12I\n\x15recording_environment\x18\x03 \x01(\x0b\x32*.bosdyn.api.graph_nav.RecordingEnvironment\x12\x19\n\x11require_fiducials\x18\x04 \x03(\x05\x12\x36\n\x12session_start_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xa2\x07\n\x16StartRecordingResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x38\n\x10\x63reated_waypoint\x18\x02 \x01(\x0b\x32\x1e.bosdyn.api.graph_nav.Waypoint\x12\x34\n\x10lease_use_result\x18\x03 \x01(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12\x43\n\x06status\x18\x04 \x01(\x0e\x32\x33.bosdyn.api.graph_nav.StartRecordingResponse.Status\x12\x19\n\x11missing_fiducials\x18\x05 \x03(\x05\x12\x1a\n\x12\x62\x61\x64_pose_fiducials\x18\x07 \x03(\x05\x12\x36\n\x0elicense_status\x18\x06 \x01(\x0e\x32\x1e.bosdyn.api.LicenseInfo.Status\x12\x36\n\x0eimpaired_state\x18\x08 \x01(\x0b\x32\x1e.bosdyn.api.RobotImpairedState\x12\x36\n\x12session_start_time\x18\t \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\tmap_stats\x18\n \x01(\x0b\x32\x1e.bosdyn.api.graph_nav.MapStats\"\x94\x03\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12$\n STATUS_COULD_NOT_CREATE_WAYPOINT\x10\x02\x12\x1a\n\x16STATUS_FOLLOWING_ROUTE\x10\x03\x12(\n$STATUS_NOT_LOCALIZED_TO_EXISTING_MAP\x10\x04\x12\x1c\n\x18STATUS_MISSING_FIDUCIALS\x10\x05\x12 \n\x1cSTATUS_MAP_TOO_LARGE_LICENSE\x10\x06\x12\x30\n,STATUS_REMOTE_CLOUD_FAILURE_NOT_IN_DIRECTORY\x10\x07\x12\'\n#STATUS_REMOTE_CLOUD_FAILURE_NO_DATA\x10\x08\x12\x1f\n\x1bSTATUS_FIDUCIAL_POSE_NOT_OK\x10\t\x12$\n STATUS_TOO_FAR_FROM_EXISTING_MAP\x10\n\x12\x19\n\x15STATUS_ROBOT_IMPAIRED\x10\x0b\"c\n\x14StopRecordingRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12 \n\x05lease\x18\x02 \x01(\x0b\x32\x11.bosdyn.api.Lease\"\xb5\x03\n\x15StopRecordingResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x42\n\x06status\x18\x02 \x01(\x0e\x32\x32.bosdyn.api.graph_nav.StopRecordingResponse.Status\x12#\n\x1b\x65rror_waypoint_localized_id\x18\x03 \x01(\t\x12\x34\n\x10lease_use_result\x18\x04 \x01(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12\x36\n\x12session_start_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\tmap_stats\x18\x06 \x01(\x0b\x32\x1e.bosdyn.api.graph_nav.MapStats\"f\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1f\n\x1bSTATUS_NOT_LOCALIZED_TO_END\x10\x02\x12\x18\n\x14STATUS_NOT_READY_YET\x10\x03\"\x91\x02\n\x15\x43reateWaypointRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x15\n\rwaypoint_name\x18\x02 \x01(\t\x12I\n\x15recording_environment\x18\x03 \x01(\x0b\x32*.bosdyn.api.graph_nav.RecordingEnvironment\x12 \n\x05lease\x18\x04 \x01(\x0b\x32\x11.bosdyn.api.Lease\x12\x19\n\x11require_fiducials\x18\x05 \x03(\x05\x12.\n\rworld_objects\x18\x06 \x03(\x0b\x32\x17.bosdyn.api.WorldObject\"\xf7\x05\n\x16\x43reateWaypointResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x38\n\x10\x63reated_waypoint\x18\x02 \x01(\x0b\x32\x1e.bosdyn.api.graph_nav.Waypoint\x12\x30\n\x0c\x63reated_edge\x18\x03 \x01(\x0b\x32\x1a.bosdyn.api.graph_nav.Edge\x12\x43\n\x06status\x18\x05 \x01(\x0e\x32\x33.bosdyn.api.graph_nav.CreateWaypointResponse.Status\x12\x34\n\x10lease_use_result\x18\x04 \x01(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12\x19\n\x11missing_fiducials\x18\x06 \x03(\x05\x12\x1a\n\x12\x62\x61\x64_pose_fiducials\x18\x08 \x03(\x05\x12\x36\n\x0elicense_status\x18\x07 \x01(\x0e\x32\x1e.bosdyn.api.LicenseInfo.Status\x12\x31\n\tmap_stats\x18\t \x01(\x0b\x32\x1e.bosdyn.api.graph_nav.MapStats\"\xa7\x02\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x18\n\x14STATUS_NOT_RECORDING\x10\x02\x12$\n STATUS_COULD_NOT_CREATE_WAYPOINT\x10\x03\x12\x1c\n\x18STATUS_MISSING_FIDUCIALS\x10\x04\x12 \n\x1cSTATUS_MAP_TOO_LARGE_LICENSE\x10\x05\x12\x30\n,STATUS_REMOTE_CLOUD_FAILURE_NOT_IN_DIRECTORY\x10\x06\x12\'\n#STATUS_REMOTE_CLOUD_FAILURE_NO_DATA\x10\x07\x12\x1f\n\x1bSTATUS_FIDUCIAL_POSE_NOT_OK\x10\x08\"\x8a\x01\n\x11\x43reateEdgeRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12(\n\x04\x65\x64ge\x18\x02 \x01(\x0b\x32\x1a.bosdyn.api.graph_nav.Edge\x12 \n\x05lease\x18\x03 \x01(\x0b\x32\x11.bosdyn.api.Lease\"\xb9\x03\n\x12\x43reateEdgeResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12?\n\x06status\x18\x02 \x01(\x0e\x32/.bosdyn.api.graph_nav.CreateEdgeResponse.Status\x12\x37\n\x13\x65rror_existing_edge\x18\x03 \x01(\x0b\x32\x1a.bosdyn.api.graph_nav.Edge\x12\x34\n\x10lease_use_result\x18\x04 \x01(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12\x31\n\tmap_stats\x18\x05 \x01(\x0b\x32\x1e.bosdyn.api.graph_nav.MapStats\"\x93\x01\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x11\n\rSTATUS_EXISTS\x10\x02\x12\x18\n\x14STATUS_NOT_RECORDING\x10\x03\x12\x1b\n\x17STATUS_UNKNOWN_WAYPOINT\x10\x04\x12\x1c\n\x18STATUS_MISSING_TRANSFORM\x10\x05\"C\n\x16GetRecordStatusRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"\xfc\x04\n\x17GetRecordStatusResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x14\n\x0cis_recording\x18\x02 \x01(\x08\x12I\n\x15recording_environment\x18\x03 \x01(\x0b\x32*.bosdyn.api.graph_nav.RecordingEnvironment\x12I\n\tmap_state\x18\x04 \x01(\x0e\x32\x36.bosdyn.api.graph_nav.GetRecordStatusResponse.MapState\x12\x44\n\x06status\x18\x05 \x01(\x0e\x32\x34.bosdyn.api.graph_nav.GetRecordStatusResponse.Status\x12\x36\n\x0eimpaired_state\x18\x06 \x01(\x0b\x32\x1e.bosdyn.api.RobotImpairedState\x12\x36\n\x12session_start_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\tmap_stats\x18\x08 \x01(\x0b\x32\x1e.bosdyn.api.graph_nav.MapStats\"X\n\x08MapState\x12\x15\n\x11MAP_STATE_UNKNOWN\x10\x00\x12\x10\n\x0cMAP_STATE_OK\x10\x01\x12#\n\x1fMAP_STATE_TOO_LARGE_FOR_LICENSE\x10\x02\"F\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x19\n\x15STATUS_ROBOT_IMPAIRED\x10\x02\x42\x10\x42\x0eRecordingProtob\x06proto3')
 
 
 
 _RECORDINGENVIRONMENT = DESCRIPTOR.message_types_by_name['RecordingEnvironment']
 _SETRECORDINGENVIRONMENTREQUEST = DESCRIPTOR.message_types_by_name['SetRecordingEnvironmentRequest']
 _SETRECORDINGENVIRONMENTRESPONSE = DESCRIPTOR.message_types_by_name['SetRecordingEnvironmentResponse']
 _STARTRECORDINGREQUEST = DESCRIPTOR.message_types_by_name['StartRecordingRequest']
@@ -134,46 +135,46 @@
   })
 _sym_db.RegisterMessage(GetRecordStatusResponse)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'B\016RecordingProto'
-  _RECORDINGENVIRONMENT._serialized_start=231
-  _RECORDINGENVIRONMENT._serialized_end=414
-  _SETRECORDINGENVIRONMENTREQUEST._serialized_start=417
-  _SETRECORDINGENVIRONMENTREQUEST._serialized_end=591
-  _SETRECORDINGENVIRONMENTRESPONSE._serialized_start=594
-  _SETRECORDINGENVIRONMENTRESPONSE._serialized_end=725
-  _STARTRECORDINGREQUEST._serialized_start=728
-  _STARTRECORDINGREQUEST._serialized_end=930
-  _STARTRECORDINGRESPONSE._serialized_start=933
-  _STARTRECORDINGRESPONSE._serialized_end=1756
-  _STARTRECORDINGRESPONSE_STATUS._serialized_start=1352
-  _STARTRECORDINGRESPONSE_STATUS._serialized_end=1756
-  _STOPRECORDINGREQUEST._serialized_start=1758
-  _STOPRECORDINGREQUEST._serialized_end=1857
-  _STOPRECORDINGRESPONSE._serialized_start=1860
-  _STOPRECORDINGRESPONSE._serialized_end=2190
-  _STOPRECORDINGRESPONSE_STATUS._serialized_start=2088
-  _STOPRECORDINGRESPONSE_STATUS._serialized_end=2190
-  _CREATEWAYPOINTREQUEST._serialized_start=2193
-  _CREATEWAYPOINTREQUEST._serialized_end=2466
-  _CREATEWAYPOINTRESPONSE._serialized_start=2469
-  _CREATEWAYPOINTRESPONSE._serialized_end=3177
-  _CREATEWAYPOINTRESPONSE_STATUS._serialized_start=2882
-  _CREATEWAYPOINTRESPONSE_STATUS._serialized_end=3177
-  _CREATEEDGEREQUEST._serialized_start=3180
-  _CREATEEDGEREQUEST._serialized_end=3318
-  _CREATEEDGERESPONSE._serialized_start=3321
-  _CREATEEDGERESPONSE._serialized_end=3711
-  _CREATEEDGERESPONSE_STATUS._serialized_start=3564
-  _CREATEEDGERESPONSE_STATUS._serialized_end=3711
-  _GETRECORDSTATUSREQUEST._serialized_start=3713
-  _GETRECORDSTATUSREQUEST._serialized_end=3780
-  _GETRECORDSTATUSRESPONSE._serialized_start=3783
-  _GETRECORDSTATUSRESPONSE._serialized_end=4312
-  _GETRECORDSTATUSRESPONSE_MAPSTATE._serialized_start=4152
-  _GETRECORDSTATUSRESPONSE_MAPSTATE._serialized_end=4240
-  _GETRECORDSTATUSRESPONSE_STATUS._serialized_start=4242
-  _GETRECORDSTATUSRESPONSE_STATUS._serialized_end=4312
+  _RECORDINGENVIRONMENT._serialized_start=264
+  _RECORDINGENVIRONMENT._serialized_end=447
+  _SETRECORDINGENVIRONMENTREQUEST._serialized_start=450
+  _SETRECORDINGENVIRONMENTREQUEST._serialized_end=624
+  _SETRECORDINGENVIRONMENTRESPONSE._serialized_start=627
+  _SETRECORDINGENVIRONMENTRESPONSE._serialized_end=758
+  _STARTRECORDINGREQUEST._serialized_start=761
+  _STARTRECORDINGREQUEST._serialized_end=1019
+  _STARTRECORDINGRESPONSE._serialized_start=1022
+  _STARTRECORDINGRESPONSE._serialized_end=1952
+  _STARTRECORDINGRESPONSE_STATUS._serialized_start=1548
+  _STARTRECORDINGRESPONSE_STATUS._serialized_end=1952
+  _STOPRECORDINGREQUEST._serialized_start=1954
+  _STOPRECORDINGREQUEST._serialized_end=2053
+  _STOPRECORDINGRESPONSE._serialized_start=2056
+  _STOPRECORDINGRESPONSE._serialized_end=2493
+  _STOPRECORDINGRESPONSE_STATUS._serialized_start=2391
+  _STOPRECORDINGRESPONSE_STATUS._serialized_end=2493
+  _CREATEWAYPOINTREQUEST._serialized_start=2496
+  _CREATEWAYPOINTREQUEST._serialized_end=2769
+  _CREATEWAYPOINTRESPONSE._serialized_start=2772
+  _CREATEWAYPOINTRESPONSE._serialized_end=3531
+  _CREATEWAYPOINTRESPONSE_STATUS._serialized_start=3236
+  _CREATEWAYPOINTRESPONSE_STATUS._serialized_end=3531
+  _CREATEEDGEREQUEST._serialized_start=3534
+  _CREATEEDGEREQUEST._serialized_end=3672
+  _CREATEEDGERESPONSE._serialized_start=3675
+  _CREATEEDGERESPONSE._serialized_end=4116
+  _CREATEEDGERESPONSE_STATUS._serialized_start=3969
+  _CREATEEDGERESPONSE_STATUS._serialized_end=4116
+  _GETRECORDSTATUSREQUEST._serialized_start=4118
+  _GETRECORDSTATUSREQUEST._serialized_end=4185
+  _GETRECORDSTATUSRESPONSE._serialized_start=4188
+  _GETRECORDSTATUSRESPONSE._serialized_end=4824
+  _GETRECORDSTATUSRESPONSE_MAPSTATE._serialized_start=4664
+  _GETRECORDSTATUSRESPONSE_MAPSTATE._serialized_end=4752
+  _GETRECORDSTATUSRESPONSE_STATUS._serialized_start=4754
+  _GETRECORDSTATUSRESPONSE_STATUS._serialized_end=4824
 # @@protoc_insertion_point(module_scope)
```

## bosdyn/api/mission/__init__.py

```diff
@@ -0,0 +1,4 @@
+00000000: 5f5f 7061 7468 5f5f 203d 205f 5f69 6d70  __path__ = __imp
+00000010: 6f72 745f 5f28 2770 6b67 7574 696c 2729  ort__('pkgutil')
+00000020: 2e65 7874 656e 645f 7061 7468 285f 5f70  .extend_path(__p
+00000030: 6174 685f 5f2c 205f 5f6e 616d 655f 5f29  ath__, __name__)
```

## bosdyn/api/mission/mission_pb2.py

```diff
@@ -19,24 +19,25 @@
 from bosdyn.api import lease_pb2 as bosdyn_dot_api_dot_lease__pb2
 from bosdyn.api.mission import nodes_pb2 as bosdyn_dot_api_dot_mission_dot_nodes__pb2
 from bosdyn.api.mission import util_pb2 as bosdyn_dot_api_dot_mission_dot_util__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n bosdyn/api/mission/mission.proto\x12\x12\x62osdyn.api.mission\x1a\x17\x62osdyn/api/alerts.proto\x1a\x19\x62osdyn/api/geometry.proto\x1a\x1e\x62osdyn/api/graph_nav/map.proto\x1a\x17\x62osdyn/api/header.proto\x1a\x16\x62osdyn/api/lease.proto\x1a\x1e\x62osdyn/api/mission/nodes.proto\x1a\x1d\x62osdyn/api/mission/util.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\xcc\x01\n\x0fGetStateRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12=\n\x18history_upper_tick_bound\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.Int64Value\x12\"\n\x18history_lower_tick_bound\x18\x03 \x01(\x03H\x00\x12\x1c\n\x12history_past_ticks\x18\x04 \x01(\x03H\x00\x42\r\n\x0blower_bound\"h\n\x10GetStateResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12(\n\x05state\x18\x02 \x01(\x0b\x32\x19.bosdyn.api.mission.State\"\xb3\x06\n\x05State\x12/\n\tquestions\x18\x01 \x03(\x0b\x32\x1c.bosdyn.api.mission.Question\x12\x46\n\x12\x61nswered_questions\x18\x02 \x03(\x0b\x32*.bosdyn.api.mission.State.AnsweredQuestion\x12;\n\x07history\x18\x03 \x03(\x0b\x32*.bosdyn.api.mission.State.NodeStatesAtTick\x12\x30\n\x06status\x18\x04 \x01(\x0e\x32 .bosdyn.api.mission.State.Status\x12\r\n\x05\x65rror\x18\x05 \x01(\t\x12\x14\n\x0ctick_counter\x18\x06 \x01(\x03\x12\x12\n\nmission_id\x18\x07 \x01(\x03\x1a`\n\x10\x41nsweredQuestion\x12.\n\x08question\x18\x01 \x01(\x0b\x32\x1c.bosdyn.api.mission.Question\x12\x1c\n\x14\x61\x63\x63\x65pted_answer_code\x18\x02 \x01(\x03\x1a\x81\x02\n\x10NodeStatesAtTick\x12\x14\n\x0ctick_counter\x18\x01 \x01(\x03\x12\x38\n\x14tick_start_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12I\n\x0bnode_states\x18\x03 \x03(\x0b\x32\x34.bosdyn.api.mission.State.NodeStatesAtTick.NodeState\x1aR\n\tNodeState\x12*\n\x06result\x18\x01 \x01(\x0e\x32\x1a.bosdyn.api.mission.Result\x12\r\n\x05\x65rror\x18\x02 \x01(\t\x12\n\n\x02id\x18\x03 \x01(\x03\"\xa2\x01\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x12\n\x0eSTATUS_FAILURE\x10\x01\x12\x12\n\x0eSTATUS_RUNNING\x10\x02\x12\x12\n\x0eSTATUS_SUCCESS\x10\x03\x12\x11\n\rSTATUS_PAUSED\x10\x04\x12\x10\n\x0cSTATUS_ERROR\x10\x05\x12\x0f\n\x0bSTATUS_NONE\x10\x06\x12\x12\n\x0eSTATUS_STOPPED\x10\x07\"\xc2\x01\n\x08Question\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x0e\n\x06source\x18\x02 \x01(\t\x12\x0c\n\x04text\x18\x03 \x01(\t\x12\x32\n\x07options\x18\x04 \x03(\x0b\x32!.bosdyn.api.mission.Prompt.Option\x12!\n\x19\x66or_autonomous_processing\x18\x05 \x01(\x08\x12\x35\n\x08severity\x18\x06 \x01(\x0e\x32#.bosdyn.api.AlertData.SeverityLevel\"e\n\x15\x41nswerQuestionRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x13\n\x0bquestion_id\x18\x02 \x01(\x03\x12\x0c\n\x04\x63ode\x18\x03 \x01(\x03\"\x8b\x02\n\x16\x41nswerQuestionResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x41\n\x06status\x18\x02 \x01(\x0e\x32\x31.bosdyn.api.mission.AnswerQuestionResponse.Status\"\x81\x01\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1e\n\x1aSTATUS_INVALID_QUESTION_ID\x10\x02\x12\x17\n\x13STATUS_INVALID_CODE\x10\x03\x12\x1b\n\x17STATUS_ALREADY_ANSWERED\x10\x04\"E\n\x0bMissionInfo\x12\n\n\x02id\x18\x01 \x01(\x03\x12*\n\x04root\x18\x02 \x01(\x0b\x32\x1c.bosdyn.api.mission.NodeInfo\"\x85\x01\n\x08NodeInfo\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x0c\n\x04name\x18\x02 \x01(\t\x12/\n\tuser_data\x18\x03 \x01(\x0b\x32\x1c.bosdyn.api.mission.UserData\x12.\n\x08\x63hildren\x18\x04 \x03(\x0b\x32\x1c.bosdyn.api.mission.NodeInfo\"@\n\nFailedNode\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05\x65rror\x18\x02 \x01(\t\x12\x15\n\rimpl_typename\x18\x03 \x01(\t\"\xc6\x01\n\x12PlayMissionRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12.\n\npause_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12!\n\x06leases\x18\x04 \x03(\x0b\x32\x11.bosdyn.api.Lease\x12\x32\n\x08settings\x18\x05 \x01(\x0b\x32 .bosdyn.api.mission.PlaySettings\"\xca\x02\n\x0cPlaySettings\x12\x34\n\x0evelocity_limit\x18\x01 \x01(\x0b\x32\x1c.bosdyn.api.SE2VelocityLimit\x12$\n\x1c\x64isable_directed_exploration\x18\x02 \x01(\x08\x12\'\n\x1f\x64isable_alternate_route_finding\x18\x03 \x01(\x08\x12U\n\x13path_following_mode\x18\x04 \x01(\x0e\x32\x38.bosdyn.api.graph_nav.Edge.Annotations.PathFollowingMode\x12^\n\x13ground_clutter_mode\x18\x05 \x01(\x0e\x32\x41.bosdyn.api.graph_nav.Edge.Annotations.GroundClutterAvoidanceMode\"\xfc\x01\n\x13PlayMissionResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12>\n\x06status\x18\x02 \x01(\x0e\x32..bosdyn.api.mission.PlayMissionResponse.Status\x12\x35\n\x11lease_use_results\x18\x03 \x03(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\"B\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x15\n\x11STATUS_NO_MISSION\x10\x02\"\xc9\x01\n\x15RestartMissionRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12.\n\npause_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12!\n\x06leases\x18\x03 \x03(\x0b\x32\x11.bosdyn.api.Lease\x12\x32\n\x08settings\x18\x04 \x01(\x0b\x32 .bosdyn.api.mission.PlaySettings\"\xd3\x02\n\x16RestartMissionResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x41\n\x06status\x18\x02 \x01(\x0e\x32\x31.bosdyn.api.mission.RestartMissionResponse.Status\x12\x35\n\x11lease_use_results\x18\x03 \x03(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12\x34\n\x0c\x66\x61iled_nodes\x18\x04 \x03(\x0b\x32\x1e.bosdyn.api.mission.FailedNode\"]\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x15\n\x11STATUS_NO_MISSION\x10\x02\x12\x19\n\x15STATUS_VALIDATE_ERROR\x10\x03\"\x8a\x01\n\x12LoadMissionRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12&\n\x04root\x18\x02 \x01(\x0b\x32\x18.bosdyn.api.mission.Node\x12!\n\x06leases\x18\x03 \x03(\x0b\x32\x11.bosdyn.api.Lease\"\x87\x03\n\x13LoadMissionResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12>\n\x06status\x18\x02 \x01(\x0e\x32..bosdyn.api.mission.LoadMissionResponse.Status\x12\x35\n\x11lease_use_results\x18\x03 \x03(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12\x35\n\x0cmission_info\x18\x04 \x01(\x0b\x32\x1f.bosdyn.api.mission.MissionInfo\x12\x34\n\x0c\x66\x61iled_nodes\x18\x05 \x03(\x0b\x32\x1e.bosdyn.api.mission.FailedNode\"`\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x18\n\x14STATUS_COMPILE_ERROR\x10\x02\x12\x19\n\x15STATUS_VALIDATE_ERROR\x10\x03\";\n\x0eGetInfoRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"t\n\x0fGetInfoResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x35\n\x0cmission_info\x18\x02 \x01(\x0b\x32\x1f.bosdyn.api.mission.MissionInfo\"b\n\x13PauseMissionRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12 \n\x05lease\x18\x02 \x01(\x0b\x32\x11.bosdyn.api.Lease\"\x85\x02\n\x14PauseMissionResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12?\n\x06status\x18\x02 \x01(\x0e\x32/.bosdyn.api.mission.PauseMissionResponse.Status\x12\x34\n\x10lease_use_result\x18\x03 \x01(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\"J\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1d\n\x19STATUS_NO_MISSION_PLAYING\x10\x02\"a\n\x12StopMissionRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12 \n\x05lease\x18\x02 \x01(\x0b\x32\x11.bosdyn.api.Lease\"\x83\x02\n\x13StopMissionResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12>\n\x06status\x18\x02 \x01(\x0e\x32..bosdyn.api.mission.StopMissionResponse.Status\x12\x34\n\x10lease_use_result\x18\x03 \x01(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\"J\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1d\n\x19STATUS_NO_MISSION_PLAYING\x10\x02\">\n\x11GetMissionRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"t\n\x12GetMissionResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12&\n\x04root\x18\x02 \x01(\x0b\x32\x18.bosdyn.api.mission.Node\x12\n\n\x02id\x18\x03 \x01(\x03\x42\x0e\x42\x0cMissionProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n bosdyn/api/mission/mission.proto\x12\x12\x62osdyn.api.mission\x1a\x17\x62osdyn/api/alerts.proto\x1a\x19\x62osdyn/api/geometry.proto\x1a\x1e\x62osdyn/api/graph_nav/map.proto\x1a\x17\x62osdyn/api/header.proto\x1a\x16\x62osdyn/api/lease.proto\x1a\x1e\x62osdyn/api/mission/nodes.proto\x1a\x1d\x62osdyn/api/mission/util.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\xcc\x01\n\x0fGetStateRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12=\n\x18history_upper_tick_bound\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.Int64Value\x12\"\n\x18history_lower_tick_bound\x18\x03 \x01(\x03H\x00\x12\x1c\n\x12history_past_ticks\x18\x04 \x01(\x03H\x00\x42\r\n\x0blower_bound\"h\n\x10GetStateResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12(\n\x05state\x18\x02 \x01(\x0b\x32\x19.bosdyn.api.mission.State\"\xd2\x07\n\x05State\x12/\n\tquestions\x18\x01 \x03(\x0b\x32\x1c.bosdyn.api.mission.Question\x12\x46\n\x12\x61nswered_questions\x18\x02 \x03(\x0b\x32*.bosdyn.api.mission.State.AnsweredQuestion\x12;\n\x07history\x18\x03 \x03(\x0b\x32*.bosdyn.api.mission.State.NodeStatesAtTick\x12\x30\n\x06status\x18\x04 \x01(\x0e\x32 .bosdyn.api.mission.State.Status\x12\r\n\x05\x65rror\x18\x05 \x01(\t\x12\x14\n\x0ctick_counter\x18\x06 \x01(\x03\x12\x12\n\nmission_id\x18\x07 \x01(\x03\x1a`\n\x10\x41nsweredQuestion\x12.\n\x08question\x18\x01 \x01(\x0b\x32\x1c.bosdyn.api.mission.Question\x12\x1c\n\x14\x61\x63\x63\x65pted_answer_code\x18\x02 \x01(\x03\x1a\xa0\x03\n\x10NodeStatesAtTick\x12\x14\n\x0ctick_counter\x18\x01 \x01(\x03\x12\x38\n\x14tick_start_timestamp\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12I\n\x0bnode_states\x18\x03 \x03(\x0b\x32\x34.bosdyn.api.mission.State.NodeStatesAtTick.NodeState\x1a\xf0\x01\n\tNodeState\x12*\n\x06result\x18\x01 \x01(\x0e\x32\x1a.bosdyn.api.mission.Result\x12\r\n\x05\x65rror\x18\x02 \x01(\t\x12\n\n\x02id\x18\x03 \x01(\x03\x12X\n\nblackboard\x18\x05 \x01(\x0b\x32\x44.bosdyn.api.mission.State.NodeStatesAtTick.NodeState.BlackboardState\x1a\x42\n\x0f\x42lackboardState\x12/\n\tvariables\x18\x01 \x03(\x0b\x32\x1c.bosdyn.api.mission.KeyValue\"\xa2\x01\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x12\n\x0eSTATUS_FAILURE\x10\x01\x12\x12\n\x0eSTATUS_RUNNING\x10\x02\x12\x12\n\x0eSTATUS_SUCCESS\x10\x03\x12\x11\n\rSTATUS_PAUSED\x10\x04\x12\x10\n\x0cSTATUS_ERROR\x10\x05\x12\x0f\n\x0bSTATUS_NONE\x10\x06\x12\x12\n\x0eSTATUS_STOPPED\x10\x07\"\xc2\x01\n\x08Question\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x0e\n\x06source\x18\x02 \x01(\t\x12\x0c\n\x04text\x18\x03 \x01(\t\x12\x32\n\x07options\x18\x04 \x03(\x0b\x32!.bosdyn.api.mission.Prompt.Option\x12!\n\x19\x66or_autonomous_processing\x18\x05 \x01(\x08\x12\x35\n\x08severity\x18\x06 \x01(\x0e\x32#.bosdyn.api.AlertData.SeverityLevel\"e\n\x15\x41nswerQuestionRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x13\n\x0bquestion_id\x18\x02 \x01(\x03\x12\x0c\n\x04\x63ode\x18\x03 \x01(\x03\"\x8b\x02\n\x16\x41nswerQuestionResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x41\n\x06status\x18\x02 \x01(\x0e\x32\x31.bosdyn.api.mission.AnswerQuestionResponse.Status\"\x81\x01\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1e\n\x1aSTATUS_INVALID_QUESTION_ID\x10\x02\x12\x17\n\x13STATUS_INVALID_CODE\x10\x03\x12\x1b\n\x17STATUS_ALREADY_ANSWERED\x10\x04\"E\n\x0bMissionInfo\x12\n\n\x02id\x18\x01 \x01(\x03\x12*\n\x04root\x18\x02 \x01(\x0b\x32\x1c.bosdyn.api.mission.NodeInfo\"\x85\x01\n\x08NodeInfo\x12\n\n\x02id\x18\x01 \x01(\x03\x12\x0c\n\x04name\x18\x02 \x01(\t\x12/\n\tuser_data\x18\x03 \x01(\x0b\x32\x1c.bosdyn.api.mission.UserData\x12.\n\x08\x63hildren\x18\x04 \x03(\x0b\x32\x1c.bosdyn.api.mission.NodeInfo\"@\n\nFailedNode\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05\x65rror\x18\x02 \x01(\t\x12\x15\n\rimpl_typename\x18\x03 \x01(\t\"\xc6\x01\n\x12PlayMissionRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12.\n\npause_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12!\n\x06leases\x18\x04 \x03(\x0b\x32\x11.bosdyn.api.Lease\x12\x32\n\x08settings\x18\x05 \x01(\x0b\x32 .bosdyn.api.mission.PlaySettings\"\xca\x02\n\x0cPlaySettings\x12\x34\n\x0evelocity_limit\x18\x01 \x01(\x0b\x32\x1c.bosdyn.api.SE2VelocityLimit\x12$\n\x1c\x64isable_directed_exploration\x18\x02 \x01(\x08\x12\'\n\x1f\x64isable_alternate_route_finding\x18\x03 \x01(\x08\x12U\n\x13path_following_mode\x18\x04 \x01(\x0e\x32\x38.bosdyn.api.graph_nav.Edge.Annotations.PathFollowingMode\x12^\n\x13ground_clutter_mode\x18\x05 \x01(\x0e\x32\x41.bosdyn.api.graph_nav.Edge.Annotations.GroundClutterAvoidanceMode\"\xfc\x01\n\x13PlayMissionResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12>\n\x06status\x18\x02 \x01(\x0e\x32..bosdyn.api.mission.PlayMissionResponse.Status\x12\x35\n\x11lease_use_results\x18\x03 \x03(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\"B\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x15\n\x11STATUS_NO_MISSION\x10\x02\"\xc9\x01\n\x15RestartMissionRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12.\n\npause_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12!\n\x06leases\x18\x03 \x03(\x0b\x32\x11.bosdyn.api.Lease\x12\x32\n\x08settings\x18\x04 \x01(\x0b\x32 .bosdyn.api.mission.PlaySettings\"\xd3\x02\n\x16RestartMissionResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x41\n\x06status\x18\x02 \x01(\x0e\x32\x31.bosdyn.api.mission.RestartMissionResponse.Status\x12\x35\n\x11lease_use_results\x18\x03 \x03(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12\x34\n\x0c\x66\x61iled_nodes\x18\x04 \x03(\x0b\x32\x1e.bosdyn.api.mission.FailedNode\"]\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x15\n\x11STATUS_NO_MISSION\x10\x02\x12\x19\n\x15STATUS_VALIDATE_ERROR\x10\x03\"\x8a\x01\n\x12LoadMissionRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12&\n\x04root\x18\x02 \x01(\x0b\x32\x18.bosdyn.api.mission.Node\x12!\n\x06leases\x18\x03 \x03(\x0b\x32\x11.bosdyn.api.Lease\"\x87\x03\n\x13LoadMissionResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12>\n\x06status\x18\x02 \x01(\x0e\x32..bosdyn.api.mission.LoadMissionResponse.Status\x12\x35\n\x11lease_use_results\x18\x03 \x03(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12\x35\n\x0cmission_info\x18\x04 \x01(\x0b\x32\x1f.bosdyn.api.mission.MissionInfo\x12\x34\n\x0c\x66\x61iled_nodes\x18\x05 \x03(\x0b\x32\x1e.bosdyn.api.mission.FailedNode\"`\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x18\n\x14STATUS_COMPILE_ERROR\x10\x02\x12\x19\n\x15STATUS_VALIDATE_ERROR\x10\x03\";\n\x0eGetInfoRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"t\n\x0fGetInfoResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x35\n\x0cmission_info\x18\x02 \x01(\x0b\x32\x1f.bosdyn.api.mission.MissionInfo\"b\n\x13PauseMissionRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12 \n\x05lease\x18\x02 \x01(\x0b\x32\x11.bosdyn.api.Lease\"\x85\x02\n\x14PauseMissionResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12?\n\x06status\x18\x02 \x01(\x0e\x32/.bosdyn.api.mission.PauseMissionResponse.Status\x12\x34\n\x10lease_use_result\x18\x03 \x01(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\"J\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1d\n\x19STATUS_NO_MISSION_PLAYING\x10\x02\"a\n\x12StopMissionRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12 \n\x05lease\x18\x02 \x01(\x0b\x32\x11.bosdyn.api.Lease\"\x83\x02\n\x13StopMissionResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12>\n\x06status\x18\x02 \x01(\x0e\x32..bosdyn.api.mission.StopMissionResponse.Status\x12\x34\n\x10lease_use_result\x18\x03 \x01(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\"J\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1d\n\x19STATUS_NO_MISSION_PLAYING\x10\x02\">\n\x11GetMissionRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"t\n\x12GetMissionResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12&\n\x04root\x18\x02 \x01(\x0b\x32\x18.bosdyn.api.mission.Node\x12\n\n\x02id\x18\x03 \x01(\x03\x42\x0e\x42\x0cMissionProtob\x06proto3')
 
 
 
 _GETSTATEREQUEST = DESCRIPTOR.message_types_by_name['GetStateRequest']
 _GETSTATERESPONSE = DESCRIPTOR.message_types_by_name['GetStateResponse']
 _STATE = DESCRIPTOR.message_types_by_name['State']
 _STATE_ANSWEREDQUESTION = _STATE.nested_types_by_name['AnsweredQuestion']
 _STATE_NODESTATESATTICK = _STATE.nested_types_by_name['NodeStatesAtTick']
 _STATE_NODESTATESATTICK_NODESTATE = _STATE_NODESTATESATTICK.nested_types_by_name['NodeState']
+_STATE_NODESTATESATTICK_NODESTATE_BLACKBOARDSTATE = _STATE_NODESTATESATTICK_NODESTATE.nested_types_by_name['BlackboardState']
 _QUESTION = DESCRIPTOR.message_types_by_name['Question']
 _ANSWERQUESTIONREQUEST = DESCRIPTOR.message_types_by_name['AnswerQuestionRequest']
 _ANSWERQUESTIONRESPONSE = DESCRIPTOR.message_types_by_name['AnswerQuestionResponse']
 _MISSIONINFO = DESCRIPTOR.message_types_by_name['MissionInfo']
 _NODEINFO = DESCRIPTOR.message_types_by_name['NodeInfo']
 _FAILEDNODE = DESCRIPTOR.message_types_by_name['FailedNode']
 _PLAYMISSIONREQUEST = DESCRIPTOR.message_types_by_name['PlayMissionRequest']
@@ -83,14 +84,21 @@
     # @@protoc_insertion_point(class_scope:bosdyn.api.mission.State.AnsweredQuestion)
     })
   ,
 
   'NodeStatesAtTick' : _reflection.GeneratedProtocolMessageType('NodeStatesAtTick', (_message.Message,), {
 
     'NodeState' : _reflection.GeneratedProtocolMessageType('NodeState', (_message.Message,), {
+
+      'BlackboardState' : _reflection.GeneratedProtocolMessageType('BlackboardState', (_message.Message,), {
+        'DESCRIPTOR' : _STATE_NODESTATESATTICK_NODESTATE_BLACKBOARDSTATE,
+        '__module__' : 'bosdyn.api.mission.mission_pb2'
+        # @@protoc_insertion_point(class_scope:bosdyn.api.mission.State.NodeStatesAtTick.NodeState.BlackboardState)
+        })
+      ,
       'DESCRIPTOR' : _STATE_NODESTATESATTICK_NODESTATE,
       '__module__' : 'bosdyn.api.mission.mission_pb2'
       # @@protoc_insertion_point(class_scope:bosdyn.api.mission.State.NodeStatesAtTick.NodeState)
       })
     ,
     'DESCRIPTOR' : _STATE_NODESTATESATTICK,
     '__module__' : 'bosdyn.api.mission.mission_pb2'
@@ -101,14 +109,15 @@
   '__module__' : 'bosdyn.api.mission.mission_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.mission.State)
   })
 _sym_db.RegisterMessage(State)
 _sym_db.RegisterMessage(State.AnsweredQuestion)
 _sym_db.RegisterMessage(State.NodeStatesAtTick)
 _sym_db.RegisterMessage(State.NodeStatesAtTick.NodeState)
+_sym_db.RegisterMessage(State.NodeStatesAtTick.NodeState.BlackboardState)
 
 Question = _reflection.GeneratedProtocolMessageType('Question', (_message.Message,), {
   'DESCRIPTOR' : _QUESTION,
   '__module__' : 'bosdyn.api.mission.mission_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.mission.Question)
   })
 _sym_db.RegisterMessage(Question)
@@ -258,71 +267,73 @@
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'B\014MissionProto'
   _GETSTATEREQUEST._serialized_start=318
   _GETSTATEREQUEST._serialized_end=522
   _GETSTATERESPONSE._serialized_start=524
   _GETSTATERESPONSE._serialized_end=628
   _STATE._serialized_start=631
-  _STATE._serialized_end=1450
+  _STATE._serialized_end=1609
   _STATE_ANSWEREDQUESTION._serialized_start=929
   _STATE_ANSWEREDQUESTION._serialized_end=1025
   _STATE_NODESTATESATTICK._serialized_start=1028
-  _STATE_NODESTATESATTICK._serialized_end=1285
-  _STATE_NODESTATESATTICK_NODESTATE._serialized_start=1203
-  _STATE_NODESTATESATTICK_NODESTATE._serialized_end=1285
-  _STATE_STATUS._serialized_start=1288
-  _STATE_STATUS._serialized_end=1450
-  _QUESTION._serialized_start=1453
-  _QUESTION._serialized_end=1647
-  _ANSWERQUESTIONREQUEST._serialized_start=1649
-  _ANSWERQUESTIONREQUEST._serialized_end=1750
-  _ANSWERQUESTIONRESPONSE._serialized_start=1753
-  _ANSWERQUESTIONRESPONSE._serialized_end=2020
-  _ANSWERQUESTIONRESPONSE_STATUS._serialized_start=1891
-  _ANSWERQUESTIONRESPONSE_STATUS._serialized_end=2020
-  _MISSIONINFO._serialized_start=2022
-  _MISSIONINFO._serialized_end=2091
-  _NODEINFO._serialized_start=2094
-  _NODEINFO._serialized_end=2227
-  _FAILEDNODE._serialized_start=2229
-  _FAILEDNODE._serialized_end=2293
-  _PLAYMISSIONREQUEST._serialized_start=2296
-  _PLAYMISSIONREQUEST._serialized_end=2494
-  _PLAYSETTINGS._serialized_start=2497
-  _PLAYSETTINGS._serialized_end=2827
-  _PLAYMISSIONRESPONSE._serialized_start=2830
-  _PLAYMISSIONRESPONSE._serialized_end=3082
-  _PLAYMISSIONRESPONSE_STATUS._serialized_start=3016
-  _PLAYMISSIONRESPONSE_STATUS._serialized_end=3082
-  _RESTARTMISSIONREQUEST._serialized_start=3085
-  _RESTARTMISSIONREQUEST._serialized_end=3286
-  _RESTARTMISSIONRESPONSE._serialized_start=3289
-  _RESTARTMISSIONRESPONSE._serialized_end=3628
-  _RESTARTMISSIONRESPONSE_STATUS._serialized_start=3535
-  _RESTARTMISSIONRESPONSE_STATUS._serialized_end=3628
-  _LOADMISSIONREQUEST._serialized_start=3631
-  _LOADMISSIONREQUEST._serialized_end=3769
-  _LOADMISSIONRESPONSE._serialized_start=3772
-  _LOADMISSIONRESPONSE._serialized_end=4163
-  _LOADMISSIONRESPONSE_STATUS._serialized_start=4067
-  _LOADMISSIONRESPONSE_STATUS._serialized_end=4163
-  _GETINFOREQUEST._serialized_start=4165
-  _GETINFOREQUEST._serialized_end=4224
-  _GETINFORESPONSE._serialized_start=4226
-  _GETINFORESPONSE._serialized_end=4342
-  _PAUSEMISSIONREQUEST._serialized_start=4344
-  _PAUSEMISSIONREQUEST._serialized_end=4442
-  _PAUSEMISSIONRESPONSE._serialized_start=4445
-  _PAUSEMISSIONRESPONSE._serialized_end=4706
-  _PAUSEMISSIONRESPONSE_STATUS._serialized_start=4632
-  _PAUSEMISSIONRESPONSE_STATUS._serialized_end=4706
-  _STOPMISSIONREQUEST._serialized_start=4708
-  _STOPMISSIONREQUEST._serialized_end=4805
-  _STOPMISSIONRESPONSE._serialized_start=4808
-  _STOPMISSIONRESPONSE._serialized_end=5067
-  _STOPMISSIONRESPONSE_STATUS._serialized_start=4632
-  _STOPMISSIONRESPONSE_STATUS._serialized_end=4706
-  _GETMISSIONREQUEST._serialized_start=5069
-  _GETMISSIONREQUEST._serialized_end=5131
-  _GETMISSIONRESPONSE._serialized_start=5133
-  _GETMISSIONRESPONSE._serialized_end=5249
+  _STATE_NODESTATESATTICK._serialized_end=1444
+  _STATE_NODESTATESATTICK_NODESTATE._serialized_start=1204
+  _STATE_NODESTATESATTICK_NODESTATE._serialized_end=1444
+  _STATE_NODESTATESATTICK_NODESTATE_BLACKBOARDSTATE._serialized_start=1378
+  _STATE_NODESTATESATTICK_NODESTATE_BLACKBOARDSTATE._serialized_end=1444
+  _STATE_STATUS._serialized_start=1447
+  _STATE_STATUS._serialized_end=1609
+  _QUESTION._serialized_start=1612
+  _QUESTION._serialized_end=1806
+  _ANSWERQUESTIONREQUEST._serialized_start=1808
+  _ANSWERQUESTIONREQUEST._serialized_end=1909
+  _ANSWERQUESTIONRESPONSE._serialized_start=1912
+  _ANSWERQUESTIONRESPONSE._serialized_end=2179
+  _ANSWERQUESTIONRESPONSE_STATUS._serialized_start=2050
+  _ANSWERQUESTIONRESPONSE_STATUS._serialized_end=2179
+  _MISSIONINFO._serialized_start=2181
+  _MISSIONINFO._serialized_end=2250
+  _NODEINFO._serialized_start=2253
+  _NODEINFO._serialized_end=2386
+  _FAILEDNODE._serialized_start=2388
+  _FAILEDNODE._serialized_end=2452
+  _PLAYMISSIONREQUEST._serialized_start=2455
+  _PLAYMISSIONREQUEST._serialized_end=2653
+  _PLAYSETTINGS._serialized_start=2656
+  _PLAYSETTINGS._serialized_end=2986
+  _PLAYMISSIONRESPONSE._serialized_start=2989
+  _PLAYMISSIONRESPONSE._serialized_end=3241
+  _PLAYMISSIONRESPONSE_STATUS._serialized_start=3175
+  _PLAYMISSIONRESPONSE_STATUS._serialized_end=3241
+  _RESTARTMISSIONREQUEST._serialized_start=3244
+  _RESTARTMISSIONREQUEST._serialized_end=3445
+  _RESTARTMISSIONRESPONSE._serialized_start=3448
+  _RESTARTMISSIONRESPONSE._serialized_end=3787
+  _RESTARTMISSIONRESPONSE_STATUS._serialized_start=3694
+  _RESTARTMISSIONRESPONSE_STATUS._serialized_end=3787
+  _LOADMISSIONREQUEST._serialized_start=3790
+  _LOADMISSIONREQUEST._serialized_end=3928
+  _LOADMISSIONRESPONSE._serialized_start=3931
+  _LOADMISSIONRESPONSE._serialized_end=4322
+  _LOADMISSIONRESPONSE_STATUS._serialized_start=4226
+  _LOADMISSIONRESPONSE_STATUS._serialized_end=4322
+  _GETINFOREQUEST._serialized_start=4324
+  _GETINFOREQUEST._serialized_end=4383
+  _GETINFORESPONSE._serialized_start=4385
+  _GETINFORESPONSE._serialized_end=4501
+  _PAUSEMISSIONREQUEST._serialized_start=4503
+  _PAUSEMISSIONREQUEST._serialized_end=4601
+  _PAUSEMISSIONRESPONSE._serialized_start=4604
+  _PAUSEMISSIONRESPONSE._serialized_end=4865
+  _PAUSEMISSIONRESPONSE_STATUS._serialized_start=4791
+  _PAUSEMISSIONRESPONSE_STATUS._serialized_end=4865
+  _STOPMISSIONREQUEST._serialized_start=4867
+  _STOPMISSIONREQUEST._serialized_end=4964
+  _STOPMISSIONRESPONSE._serialized_start=4967
+  _STOPMISSIONRESPONSE._serialized_end=5226
+  _STOPMISSIONRESPONSE_STATUS._serialized_start=4791
+  _STOPMISSIONRESPONSE_STATUS._serialized_end=4865
+  _GETMISSIONREQUEST._serialized_start=5228
+  _GETMISSIONREQUEST._serialized_end=5290
+  _GETMISSIONRESPONSE._serialized_start=5292
+  _GETMISSIONRESPONSE._serialized_end=5408
 # @@protoc_insertion_point(module_scope)
```

## bosdyn/api/mission/mission_service_pb2.py

```diff
@@ -12,19 +12,19 @@
 _sym_db = _symbol_database.Default()
 
 
 from bosdyn.api import data_chunk_pb2 as bosdyn_dot_api_dot_data__chunk__pb2
 from bosdyn.api.mission import mission_pb2 as bosdyn_dot_api_dot_mission_dot_mission__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(bosdyn/api/mission/mission_service.proto\x12\x12\x62osdyn.api.mission\x1a\x1b\x62osdyn/api/data_chunk.proto\x1a bosdyn/api/mission/mission.proto2\xda\x07\n\x0eMissionService\x12`\n\x0bLoadMission\x12&.bosdyn.api.mission.LoadMissionRequest\x1a\'.bosdyn.api.mission.LoadMissionResponse\"\x00\x12Y\n\x13LoadMissionAsChunks\x12\x15.bosdyn.api.DataChunk\x1a\'.bosdyn.api.mission.LoadMissionResponse\"\x00(\x01\x12`\n\x0bPlayMission\x12&.bosdyn.api.mission.PlayMissionRequest\x1a\'.bosdyn.api.mission.PlayMissionResponse\"\x00\x12\x63\n\x0cPauseMission\x12\'.bosdyn.api.mission.PauseMissionRequest\x1a(.bosdyn.api.mission.PauseMissionResponse\"\x00\x12`\n\x0bStopMission\x12&.bosdyn.api.mission.StopMissionRequest\x1a\'.bosdyn.api.mission.StopMissionResponse\"\x00\x12i\n\x0eRestartMission\x12).bosdyn.api.mission.RestartMissionRequest\x1a*.bosdyn.api.mission.RestartMissionResponse\"\x00\x12W\n\x08GetState\x12#.bosdyn.api.mission.GetStateRequest\x1a$.bosdyn.api.mission.GetStateResponse\"\x00\x12T\n\x07GetInfo\x12\".bosdyn.api.mission.GetInfoRequest\x1a#.bosdyn.api.mission.GetInfoResponse\"\x00\x12]\n\nGetMission\x12%.bosdyn.api.mission.GetMissionRequest\x1a&.bosdyn.api.mission.GetMissionResponse\"\x00\x12i\n\x0e\x41nswerQuestion\x12).bosdyn.api.mission.AnswerQuestionRequest\x1a*.bosdyn.api.mission.AnswerQuestionResponse\"\x00\x42\x15\x42\x13MissionServiceProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(bosdyn/api/mission/mission_service.proto\x12\x12\x62osdyn.api.mission\x1a\x1b\x62osdyn/api/data_chunk.proto\x1a bosdyn/api/mission/mission.proto2\xd0\t\n\x0eMissionService\x12`\n\x0bLoadMission\x12&.bosdyn.api.mission.LoadMissionRequest\x1a\'.bosdyn.api.mission.LoadMissionResponse\"\x00\x12Y\n\x13LoadMissionAsChunks\x12\x15.bosdyn.api.DataChunk\x1a\'.bosdyn.api.mission.LoadMissionResponse\"\x00(\x01\x12J\n\x14LoadMissionAsChunks2\x12\x15.bosdyn.api.DataChunk\x1a\x15.bosdyn.api.DataChunk\"\x00(\x01\x30\x01\x12`\n\x0bPlayMission\x12&.bosdyn.api.mission.PlayMissionRequest\x1a\'.bosdyn.api.mission.PlayMissionResponse\"\x00\x12\x63\n\x0cPauseMission\x12\'.bosdyn.api.mission.PauseMissionRequest\x1a(.bosdyn.api.mission.PauseMissionResponse\"\x00\x12`\n\x0bStopMission\x12&.bosdyn.api.mission.StopMissionRequest\x1a\'.bosdyn.api.mission.StopMissionResponse\"\x00\x12i\n\x0eRestartMission\x12).bosdyn.api.mission.RestartMissionRequest\x1a*.bosdyn.api.mission.RestartMissionResponse\"\x00\x12W\n\x08GetState\x12#.bosdyn.api.mission.GetStateRequest\x1a$.bosdyn.api.mission.GetStateResponse\"\x00\x12T\n\x07GetInfo\x12\".bosdyn.api.mission.GetInfoRequest\x1a#.bosdyn.api.mission.GetInfoResponse\"\x00\x12P\n\x0fGetInfoAsChunks\x12\".bosdyn.api.mission.GetInfoRequest\x1a\x15.bosdyn.api.DataChunk\"\x00\x30\x01\x12]\n\nGetMission\x12%.bosdyn.api.mission.GetMissionRequest\x1a&.bosdyn.api.mission.GetMissionResponse\"\x00\x12V\n\x12GetMissionAsChunks\x12%.bosdyn.api.mission.GetMissionRequest\x1a\x15.bosdyn.api.DataChunk\"\x00\x30\x01\x12i\n\x0e\x41nswerQuestion\x12).bosdyn.api.mission.AnswerQuestionRequest\x1a*.bosdyn.api.mission.AnswerQuestionResponse\"\x00\x42\x15\x42\x13MissionServiceProtob\x06proto3')
 
 
 
 _MISSIONSERVICE = DESCRIPTOR.services_by_name['MissionService']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'B\023MissionServiceProto'
   _MISSIONSERVICE._serialized_start=128
-  _MISSIONSERVICE._serialized_end=1114
+  _MISSIONSERVICE._serialized_end=1360
 # @@protoc_insertion_point(module_scope)
```

## bosdyn/api/mission/mission_service_pb2_grpc.py

```diff
@@ -22,14 +22,19 @@
                 response_deserializer=bosdyn_dot_api_dot_mission_dot_mission__pb2.LoadMissionResponse.FromString,
                 )
         self.LoadMissionAsChunks = channel.stream_unary(
                 '/bosdyn.api.mission.MissionService/LoadMissionAsChunks',
                 request_serializer=bosdyn_dot_api_dot_data__chunk__pb2.DataChunk.SerializeToString,
                 response_deserializer=bosdyn_dot_api_dot_mission_dot_mission__pb2.LoadMissionResponse.FromString,
                 )
+        self.LoadMissionAsChunks2 = channel.stream_stream(
+                '/bosdyn.api.mission.MissionService/LoadMissionAsChunks2',
+                request_serializer=bosdyn_dot_api_dot_data__chunk__pb2.DataChunk.SerializeToString,
+                response_deserializer=bosdyn_dot_api_dot_data__chunk__pb2.DataChunk.FromString,
+                )
         self.PlayMission = channel.unary_unary(
                 '/bosdyn.api.mission.MissionService/PlayMission',
                 request_serializer=bosdyn_dot_api_dot_mission_dot_mission__pb2.PlayMissionRequest.SerializeToString,
                 response_deserializer=bosdyn_dot_api_dot_mission_dot_mission__pb2.PlayMissionResponse.FromString,
                 )
         self.PauseMission = channel.unary_unary(
                 '/bosdyn.api.mission.MissionService/PauseMission',
@@ -52,41 +57,63 @@
                 response_deserializer=bosdyn_dot_api_dot_mission_dot_mission__pb2.GetStateResponse.FromString,
                 )
         self.GetInfo = channel.unary_unary(
                 '/bosdyn.api.mission.MissionService/GetInfo',
                 request_serializer=bosdyn_dot_api_dot_mission_dot_mission__pb2.GetInfoRequest.SerializeToString,
                 response_deserializer=bosdyn_dot_api_dot_mission_dot_mission__pb2.GetInfoResponse.FromString,
                 )
+        self.GetInfoAsChunks = channel.unary_stream(
+                '/bosdyn.api.mission.MissionService/GetInfoAsChunks',
+                request_serializer=bosdyn_dot_api_dot_mission_dot_mission__pb2.GetInfoRequest.SerializeToString,
+                response_deserializer=bosdyn_dot_api_dot_data__chunk__pb2.DataChunk.FromString,
+                )
         self.GetMission = channel.unary_unary(
                 '/bosdyn.api.mission.MissionService/GetMission',
                 request_serializer=bosdyn_dot_api_dot_mission_dot_mission__pb2.GetMissionRequest.SerializeToString,
                 response_deserializer=bosdyn_dot_api_dot_mission_dot_mission__pb2.GetMissionResponse.FromString,
                 )
+        self.GetMissionAsChunks = channel.unary_stream(
+                '/bosdyn.api.mission.MissionService/GetMissionAsChunks',
+                request_serializer=bosdyn_dot_api_dot_mission_dot_mission__pb2.GetMissionRequest.SerializeToString,
+                response_deserializer=bosdyn_dot_api_dot_data__chunk__pb2.DataChunk.FromString,
+                )
         self.AnswerQuestion = channel.unary_unary(
                 '/bosdyn.api.mission.MissionService/AnswerQuestion',
                 request_serializer=bosdyn_dot_api_dot_mission_dot_mission__pb2.AnswerQuestionRequest.SerializeToString,
                 response_deserializer=bosdyn_dot_api_dot_mission_dot_mission__pb2.AnswerQuestionResponse.FromString,
                 )
 
 
 class MissionServiceServicer(object):
     """The MissionService can be used to specify high level autonomous behaviors for Spot using behavior trees.
     """
 
     def LoadMission(self, request, context):
-        """Load a mission to run later.
+        """RPCs for loading missions to the robot. NOTE: LoadMission and LoadMissionAsChunks may fail
+        for large missions because the request and response may exceed the maximum message size. Use
+        LoadMissionAsChunks2 instead.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def LoadMissionAsChunks(self, request_iterator, context):
-        """Alternative loading method for large missions, that allows you to break the 
-        mission up into multiple streamed requests.  The data chunks should deserialize
-        into a LoadMissionRequest
+        """This RPC may be deprecated in the future, please use LoadMissionAsChunks2 instead. Non-preferred
+        method for loading large missions to the robot because only the request is a streaming RPC. The data
+        chunks are deserialized into a LoadMissionRequest. NOTE: LoadMissionAsChunks may fail for large missions
+        because the response may exceed the maximum message size.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def LoadMissionAsChunks2(self, request_iterator, context):
+        """Preferred RPC for loading large missions to the robot because both the request and response
+        are streaming RPCs, allowing you to break the message up into multiple streamed messages. The
+        data chunks are deserialized into a LoadMissionRequest and LoadMissionResponse.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def PlayMission(self, request, context):
         """Start executing a loaded mission.
@@ -123,27 +150,47 @@
         """Get the state of the mission.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetInfo(self, request, context):
-        """Get static information regarding the mission. Used to interpret mission state.
+        """RPCs for getting static information regarding the mission. Used to interpret mission state.
+        NOTE: GetInfo may fail for large missions because the response may exceed the maximum message size.
+        Use GetInfoAsChunks instead.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def GetInfoAsChunks(self, request, context):
+        """Preferred RPC for getting the status of large missions from the robot because the response is a streaming
+        streaming RPC, allowing you to break the message up into multiple streamed messages. THe data chunks are
+        deserialized into a GetInfoResponse.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetMission(self, request, context):
         """Download the mission as it was uploaded to the service.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def GetMissionAsChunks(self, request, context):
+        """Alternative method to download large missions that allows you to break
+        the mission up into multiple streamed requests. Each data chunk message should be
+        deserialized as a GetMissionResponse protobuf message.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def AnswerQuestion(self, request, context):
         """Specify an answer to the question asked by the mission.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
@@ -156,14 +203,19 @@
                     response_serializer=bosdyn_dot_api_dot_mission_dot_mission__pb2.LoadMissionResponse.SerializeToString,
             ),
             'LoadMissionAsChunks': grpc.stream_unary_rpc_method_handler(
                     servicer.LoadMissionAsChunks,
                     request_deserializer=bosdyn_dot_api_dot_data__chunk__pb2.DataChunk.FromString,
                     response_serializer=bosdyn_dot_api_dot_mission_dot_mission__pb2.LoadMissionResponse.SerializeToString,
             ),
+            'LoadMissionAsChunks2': grpc.stream_stream_rpc_method_handler(
+                    servicer.LoadMissionAsChunks2,
+                    request_deserializer=bosdyn_dot_api_dot_data__chunk__pb2.DataChunk.FromString,
+                    response_serializer=bosdyn_dot_api_dot_data__chunk__pb2.DataChunk.SerializeToString,
+            ),
             'PlayMission': grpc.unary_unary_rpc_method_handler(
                     servicer.PlayMission,
                     request_deserializer=bosdyn_dot_api_dot_mission_dot_mission__pb2.PlayMissionRequest.FromString,
                     response_serializer=bosdyn_dot_api_dot_mission_dot_mission__pb2.PlayMissionResponse.SerializeToString,
             ),
             'PauseMission': grpc.unary_unary_rpc_method_handler(
                     servicer.PauseMission,
@@ -186,19 +238,29 @@
                     response_serializer=bosdyn_dot_api_dot_mission_dot_mission__pb2.GetStateResponse.SerializeToString,
             ),
             'GetInfo': grpc.unary_unary_rpc_method_handler(
                     servicer.GetInfo,
                     request_deserializer=bosdyn_dot_api_dot_mission_dot_mission__pb2.GetInfoRequest.FromString,
                     response_serializer=bosdyn_dot_api_dot_mission_dot_mission__pb2.GetInfoResponse.SerializeToString,
             ),
+            'GetInfoAsChunks': grpc.unary_stream_rpc_method_handler(
+                    servicer.GetInfoAsChunks,
+                    request_deserializer=bosdyn_dot_api_dot_mission_dot_mission__pb2.GetInfoRequest.FromString,
+                    response_serializer=bosdyn_dot_api_dot_data__chunk__pb2.DataChunk.SerializeToString,
+            ),
             'GetMission': grpc.unary_unary_rpc_method_handler(
                     servicer.GetMission,
                     request_deserializer=bosdyn_dot_api_dot_mission_dot_mission__pb2.GetMissionRequest.FromString,
                     response_serializer=bosdyn_dot_api_dot_mission_dot_mission__pb2.GetMissionResponse.SerializeToString,
             ),
+            'GetMissionAsChunks': grpc.unary_stream_rpc_method_handler(
+                    servicer.GetMissionAsChunks,
+                    request_deserializer=bosdyn_dot_api_dot_mission_dot_mission__pb2.GetMissionRequest.FromString,
+                    response_serializer=bosdyn_dot_api_dot_data__chunk__pb2.DataChunk.SerializeToString,
+            ),
             'AnswerQuestion': grpc.unary_unary_rpc_method_handler(
                     servicer.AnswerQuestion,
                     request_deserializer=bosdyn_dot_api_dot_mission_dot_mission__pb2.AnswerQuestionRequest.FromString,
                     response_serializer=bosdyn_dot_api_dot_mission_dot_mission__pb2.AnswerQuestionResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
@@ -242,14 +304,31 @@
         return grpc.experimental.stream_unary(request_iterator, target, '/bosdyn.api.mission.MissionService/LoadMissionAsChunks',
             bosdyn_dot_api_dot_data__chunk__pb2.DataChunk.SerializeToString,
             bosdyn_dot_api_dot_mission_dot_mission__pb2.LoadMissionResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def LoadMissionAsChunks2(request_iterator,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.stream_stream(request_iterator, target, '/bosdyn.api.mission.MissionService/LoadMissionAsChunks2',
+            bosdyn_dot_api_dot_data__chunk__pb2.DataChunk.SerializeToString,
+            bosdyn_dot_api_dot_data__chunk__pb2.DataChunk.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def PlayMission(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -344,14 +423,31 @@
         return grpc.experimental.unary_unary(request, target, '/bosdyn.api.mission.MissionService/GetInfo',
             bosdyn_dot_api_dot_mission_dot_mission__pb2.GetInfoRequest.SerializeToString,
             bosdyn_dot_api_dot_mission_dot_mission__pb2.GetInfoResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def GetInfoAsChunks(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_stream(request, target, '/bosdyn.api.mission.MissionService/GetInfoAsChunks',
+            bosdyn_dot_api_dot_mission_dot_mission__pb2.GetInfoRequest.SerializeToString,
+            bosdyn_dot_api_dot_data__chunk__pb2.DataChunk.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def GetMission(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -361,14 +457,31 @@
         return grpc.experimental.unary_unary(request, target, '/bosdyn.api.mission.MissionService/GetMission',
             bosdyn_dot_api_dot_mission_dot_mission__pb2.GetMissionRequest.SerializeToString,
             bosdyn_dot_api_dot_mission_dot_mission__pb2.GetMissionResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def GetMissionAsChunks(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_stream(request, target, '/bosdyn.api.mission.MissionService/GetMissionAsChunks',
+            bosdyn_dot_api_dot_mission_dot_mission__pb2.GetMissionRequest.SerializeToString,
+            bosdyn_dot_api_dot_data__chunk__pb2.DataChunk.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def AnswerQuestion(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

## bosdyn/api/mission/nodes_pb2.py

```diff
@@ -10,43 +10,47 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import any_pb2 as google_dot_protobuf_dot_any__pb2
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
+from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from bosdyn.api import alerts_pb2 as bosdyn_dot_api_dot_alerts__pb2
 from bosdyn.api.docking import docking_pb2 as bosdyn_dot_api_dot_docking_dot_docking__pb2
 from bosdyn.api import geometry_pb2 as bosdyn_dot_api_dot_geometry__pb2
 from bosdyn.api import gripper_camera_param_pb2 as bosdyn_dot_api_dot_gripper__camera__param__pb2
 from bosdyn.api.spot_cam import camera_pb2 as bosdyn_dot_api_dot_spot__cam_dot_camera__pb2
 from bosdyn.api.spot_cam import logging_pb2 as bosdyn_dot_api_dot_spot__cam_dot_logging__pb2
 from bosdyn.api.spot_cam import ptz_pb2 as bosdyn_dot_api_dot_spot__cam_dot_ptz__pb2
 from bosdyn.api import robot_command_pb2 as bosdyn_dot_api_dot_robot__command__pb2
 from bosdyn.api import power_pb2 as bosdyn_dot_api_dot_power__pb2
 from bosdyn.api import data_acquisition_pb2 as bosdyn_dot_api_dot_data__acquisition__pb2
 from bosdyn.api import data_buffer_pb2 as bosdyn_dot_api_dot_data__buffer__pb2
 from bosdyn.api.graph_nav import graph_nav_pb2 as bosdyn_dot_api_dot_graph__nav_dot_graph__nav__pb2
 from bosdyn.api.graph_nav import nav_pb2 as bosdyn_dot_api_dot_graph__nav_dot_nav__pb2
+from bosdyn.api import manipulation_api_pb2 as bosdyn_dot_api_dot_manipulation__api__pb2
 from bosdyn.api.mission import util_pb2 as bosdyn_dot_api_dot_mission_dot_util__pb2
+from bosdyn.api import service_customization_pb2 as bosdyn_dot_api_dot_service__customization__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1e\x62osdyn/api/mission/nodes.proto\x12\x12\x62osdyn.api.mission\x1a\x19google/protobuf/any.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x17\x62osdyn/api/alerts.proto\x1a bosdyn/api/docking/docking.proto\x1a\x19\x62osdyn/api/geometry.proto\x1a%bosdyn/api/gripper_camera_param.proto\x1a bosdyn/api/spot_cam/camera.proto\x1a!bosdyn/api/spot_cam/logging.proto\x1a\x1d\x62osdyn/api/spot_cam/ptz.proto\x1a\x1e\x62osdyn/api/robot_command.proto\x1a\x16\x62osdyn/api/power.proto\x1a!bosdyn/api/data_acquisition.proto\x1a\x1c\x62osdyn/api/data_buffer.proto\x1a$bosdyn/api/graph_nav/graph_nav.proto\x1a\x1e\x62osdyn/api/graph_nav/nav.proto\x1a\x1d\x62osdyn/api/mission/util.proto\"\xc9\x02\n\x04Node\x12\x0c\n\x04name\x18\x01 \x01(\t\x12/\n\tuser_data\x18\x02 \x01(\x0b\x32\x1c.bosdyn.api.mission.UserData\x12\x14\n\x0creference_id\x18\x03 \x01(\t\x12$\n\x04impl\x18\x04 \x01(\x0b\x32\x14.google.protobuf.AnyH\x00\x12\x18\n\x0enode_reference\x18\x05 \x01(\tH\x00\x12\x36\n\x10parameter_values\x18\x06 \x03(\x0b\x32\x1c.bosdyn.api.mission.KeyValue\x12/\n\toverrides\x18\x07 \x03(\x0b\x32\x1c.bosdyn.api.mission.KeyValue\x12;\n\nparameters\x18\x08 \x03(\x0b\x32\'.bosdyn.api.mission.VariableDeclarationB\x06\n\x04type\"N\n\x08Sequence\x12\x16\n\x0e\x61lways_restart\x18\x01 \x01(\x08\x12*\n\x08\x63hildren\x18\x02 \x03(\x0b\x32\x18.bosdyn.api.mission.Node\"N\n\x08Selector\x12\x16\n\x0e\x61lways_restart\x18\x01 \x01(\x08\x12*\n\x08\x63hildren\x18\x02 \x03(\x0b\x32\x18.bosdyn.api.mission.Node\"\x92\x02\n\x06Switch\x12.\n\x0bpivot_value\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.mission.Value\x12\x16\n\x0e\x61lways_restart\x18\x02 \x01(\x08\x12\x41\n\x0cint_children\x18\x03 \x03(\x0b\x32+.bosdyn.api.mission.Switch.IntChildrenEntry\x12/\n\rdefault_child\x18\x04 \x01(\x0b\x32\x18.bosdyn.api.mission.Node\x1aL\n\x10IntChildrenEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12\'\n\x05value\x18\x02 \x01(\x0b\x32\x18.bosdyn.api.mission.Node:\x02\x38\x01\"\x86\x01\n\x06Repeat\x12\x12\n\nmax_starts\x18\x01 \x01(\x05\x12\'\n\x05\x63hild\x18\x04 \x01(\x0b\x32\x18.bosdyn.api.mission.Node\x12 \n\x18start_counter_state_name\x18\x05 \x01(\t\x12\x1d\n\x15respect_child_failure\x18\x06 \x01(\x08\"j\n\x05Retry\x12\x14\n\x0cmax_attempts\x18\x01 \x01(\x05\x12\'\n\x05\x63hild\x18\x02 \x01(\x0b\x32\x18.bosdyn.api.mission.Node\x12\"\n\x1a\x61ttempt_counter_state_name\x18\x05 \x01(\t\"\xb1\x01\n\x0b\x46orDuration\x12+\n\x08\x64uration\x18\x01 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\'\n\x05\x63hild\x18\x02 \x01(\x0b\x32\x18.bosdyn.api.mission.Node\x12\x1b\n\x13time_remaining_name\x18\x03 \x01(\t\x12/\n\rtimeout_child\x18\x04 \x01(\x0b\x32\x18.bosdyn.api.mission.Node\"h\n\x0eSimpleParallel\x12)\n\x07primary\x18\x01 \x01(\x0b\x32\x18.bosdyn.api.mission.Node\x12+\n\tsecondary\x18\x02 \x01(\x0b\x32\x18.bosdyn.api.mission.Node\"\xfa\x04\n\tCondition\x12\x32\n\x03lhs\x18\x01 \x01(\x0b\x32%.bosdyn.api.mission.Condition.Operand\x12\x32\n\x03rhs\x18\x02 \x01(\x0b\x32%.bosdyn.api.mission.Condition.Operand\x12\x38\n\toperation\x18\x05 \x01(\x0e\x32%.bosdyn.api.mission.Condition.Compare\x12G\n\x10handle_staleness\x18\x06 \x01(\x0e\x32-.bosdyn.api.mission.Condition.HandleStaleness\x1a}\n\x07Operand\x12\x36\n\x03var\x18\x01 \x01(\x0b\x32\'.bosdyn.api.mission.VariableDeclarationH\x00\x12\x32\n\x05\x63onst\x18\x02 \x01(\x0b\x32!.bosdyn.api.mission.ConstantValueH\x00\x42\x06\n\x04type\"~\n\x07\x43ompare\x12\x13\n\x0f\x43OMPARE_UNKNOWN\x10\x00\x12\x0e\n\nCOMPARE_EQ\x10\x01\x12\x0e\n\nCOMPARE_NE\x10\x02\x12\x0e\n\nCOMPARE_LT\x10\x03\x12\x0e\n\nCOMPARE_GT\x10\x04\x12\x0e\n\nCOMPARE_LE\x10\x05\x12\x0e\n\nCOMPARE_GE\x10\x06\"\x82\x01\n\x0fHandleStaleness\x12\x18\n\x14HANDLE_STALE_UNKNOWN\x10\x00\x12\x1c\n\x18HANDLE_STALE_READ_ANYWAY\x10\x01\x12 \n\x1cHANDLE_STALE_RUN_UNTIL_FRESH\x10\x02\x12\x15\n\x11HANDLE_STALE_FAIL\x10\x03\"s\n\x10\x42osdynRobotState\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x0c\n\x04host\x18\x02 \x01(\t\x12\'\n\x05\x63hild\x18\x03 \x01(\x0b\x32\x18.bosdyn.api.mission.Node\x12\x12\n\nstate_name\x18\x04 \x01(\t\"r\n\x0f\x42osdynDockState\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x0c\n\x04host\x18\x02 \x01(\t\x12\'\n\x05\x63hild\x18\x03 \x01(\x0b\x32\x18.bosdyn.api.mission.Node\x12\x12\n\nstate_name\x18\x04 \x01(\t\"c\n\x12\x42osdynRobotCommand\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x0c\n\x04host\x18\x02 \x01(\t\x12)\n\x07\x63ommand\x18\x03 \x01(\x0b\x32\x18.bosdyn.api.RobotCommand\"r\n\x12\x42osdynPowerRequest\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x0c\n\x04host\x18\x02 \x01(\t\x12\x38\n\x07request\x18\x04 \x01(\x0e\x32\'.bosdyn.api.PowerCommandRequest.Request\"\xb4\x02\n\x10\x42osdynNavigateTo\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x0c\n\x04host\x18\x02 \x01(\t\x12\x1f\n\x17\x64\x65stination_waypoint_id\x18\x03 \x01(\t\x12>\n\x10route_gen_params\x18\x04 \x01(\x0b\x32$.bosdyn.api.graph_nav.RouteGenParams\x12\x39\n\rtravel_params\x18\x05 \x01(\x0b\x32\".bosdyn.api.graph_nav.TravelParams\x12\x33\n+navigation_feedback_response_blackboard_key\x18\x06 \x01(\t\x12+\n#navigate_to_response_blackboard_key\x18\x07 \x01(\t\"\xce\x02\n\x13\x42osdynNavigateRoute\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x0c\n\x04host\x18\x02 \x01(\t\x12*\n\x05route\x18\x03 \x01(\x0b\x32\x1b.bosdyn.api.graph_nav.Route\x12G\n\x13route_follow_params\x18\x04 \x01(\x0b\x32*.bosdyn.api.graph_nav.RouteFollowingParams\x12\x39\n\rtravel_params\x18\x05 \x01(\x0b\x32\".bosdyn.api.graph_nav.TravelParams\x12\x33\n+navigation_feedback_response_blackboard_key\x18\x06 \x01(\t\x12.\n&navigate_route_response_blackboard_key\x18\x07 \x01(\t\"\x8b\x01\n\x13\x42osdynGraphNavState\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x0c\n\x04host\x18\x02 \x01(\t\x12\'\n\x05\x63hild\x18\x03 \x01(\x0b\x32\x18.bosdyn.api.mission.Node\x12\x12\n\nstate_name\x18\x04 \x01(\t\x12\x13\n\x0bwaypoint_id\x18\x05 \x01(\t\"\x88\x01\n\x16\x42osdynGraphNavLocalize\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x0c\n\x04host\x18\x02 \x01(\t\x12J\n\x14localization_request\x18\x03 \x01(\x0b\x32,.bosdyn.api.graph_nav.SetLocalizationRequest\"\xa8\x02\n\x11\x42osdynRecordEvent\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x0c\n\x04host\x18\x02 \x01(\t\x12 \n\x05\x65vent\x18\x03 \x01(\x0b\x32\x11.bosdyn.api.Event\x12\x15\n\rsucceed_early\x18\x04 \x01(\x08\x12^\n\x15\x61\x64\x64itional_parameters\x18\x05 \x03(\x0b\x32?.bosdyn.api.mission.BosdynRecordEvent.AdditionalParametersEntry\x1aV\n\x19\x41\x64\x64itionalParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12(\n\x05value\x18\x02 \x01(\x0b\x32\x19.bosdyn.api.mission.Value:\x02\x38\x01\"\x88\x01\n\nRemoteGrpc\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x14\n\x0cservice_name\x18\x03 \x01(\t\x12\x0f\n\x07timeout\x18\x04 \x01(\x02\x12\x17\n\x0flease_resources\x18\x05 \x03(\t\x12,\n\x06inputs\x18\x06 \x03(\x0b\x32\x1c.bosdyn.api.mission.KeyValue\"4\n\x05Sleep\x12\x0f\n\x07seconds\x18\x01 \x01(\x02\x12\x1a\n\x12restart_after_stop\x18\x02 \x01(\x08\"\xa3\x02\n\x06Prompt\x12\x17\n\x0f\x61lways_reprompt\x18\x01 \x01(\x08\x12\x0c\n\x04text\x18\x02 \x01(\t\x12\x0e\n\x06source\x18\x03 \x01(\t\x12\x32\n\x07options\x18\x04 \x03(\x0b\x32!.bosdyn.api.mission.Prompt.Option\x12\'\n\x05\x63hild\x18\x05 \x01(\x0b\x32\x18.bosdyn.api.mission.Node\x12!\n\x19\x66or_autonomous_processing\x18\x06 \x01(\x08\x12\x35\n\x08severity\x18\x07 \x01(\x0e\x32#.bosdyn.api.AlertData.SeverityLevel\x1a+\n\x06Option\x12\x0c\n\x04text\x18\x01 \x01(\t\x12\x13\n\x0b\x61nswer_code\x18\x02 \x01(\x03\"\x81\x01\n\x1e\x42osdynGripperCameraParamsState\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x0c\n\x04host\x18\x02 \x01(\t\x12\'\n\x05\x63hild\x18\x03 \x01(\x0b\x32\x18.bosdyn.api.mission.Node\x12\x12\n\nstate_name\x18\x04 \x01(\t\"\xa1\x01\n\x16SetGripperCameraParams\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x0c\n\x04host\x18\x02 \x01(\t\x12\"\n\x18params_in_blackboard_key\x18\x03 \x01(\tH\x00\x12\x35\n\nnew_params\x18\x04 \x01(\x0b\x32\x1f.bosdyn.api.GripperCameraParamsH\x00\x42\x08\n\x06params\"\xad\x02\n\nSpotCamPtz\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x0c\n\x04host\x18\x02 \x01(\t\x12\x36\n\x0cptz_position\x18\x03 \x01(\x0b\x32 .bosdyn.api.spot_cam.PtzPosition\x12J\n\x11\x61\x64just_parameters\x18\x04 \x01(\x0b\x32/.bosdyn.api.mission.SpotCamPtz.AdjustParameters\x1aw\n\x10\x41\x64justParameters\x12\x1c\n\x14localization_varname\x18\x04 \x01(\t\x12\x13\n\x0bwaypoint_id\x18\x05 \x01(\t\x12\x30\n\x13waypoint_tform_body\x18\x06 \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\"\xa9\x01\n\x11SpotCamStoreMedia\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x0c\n\x04host\x18\x02 \x01(\t\x12+\n\x06\x63\x61mera\x18\x03 \x01(\x0b\x32\x1b.bosdyn.api.spot_cam.Camera\x12\x36\n\x04type\x18\x04 \x01(\x0e\x32(.bosdyn.api.spot_cam.Logpoint.RecordType\x12\x0b\n\x03tag\x18\x05 \x01(\t\"\xad\x01\n\nSpotCamLed\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x0c\n\x04host\x18\x02 \x01(\t\x12\x46\n\x0c\x62rightnesses\x18\x03 \x03(\x0b\x32\x30.bosdyn.api.mission.SpotCamLed.BrightnessesEntry\x1a\x33\n\x11\x42rightnessesEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\x02:\x02\x38\x01\";\n\x15SpotCamResetAutofocus\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x0c\n\x04host\x18\x02 \x01(\t\"\xe3\x02\n\x04\x44ock\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x0c\n\x04host\x18\x02 \x01(\t\x12\x1a\n\x12\x64ocking_station_id\x18\x03 \x01(\r\x12+\n\x05\x63hild\x18\x04 \x01(\x0b\x32\x18.bosdyn.api.mission.NodeB\x02\x18\x01\x12\x1f\n\x13\x63ommand_status_name\x18\x05 \x01(\tB\x02\x18\x01\x12 \n\x14\x66\x65\x65\x64\x62\x61\x63k_status_name\x18\x06 \x01(\tB\x02\x18\x01\x12@\n\x12prep_pose_behavior\x18\x07 \x01(\x0e\x32$.bosdyn.api.docking.PrepPoseBehavior\x12\x38\n0docking_command_feedback_response_blackboard_key\x18\x08 \x01(\t\x12/\n\'docking_command_response_blackboard_key\x18\t \x01(\t\"\x87\x01\n\rStoreMetadata\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x0c\n\x04host\x18\x02 \x01(\t\x12!\n\x19\x61\x63quire_data_request_name\x18\x03 \x01(\t\x12\x15\n\rmetadata_name\x18\x05 \x01(\t\x12\x18\n\x10metadata_channel\x18\x06 \x01(\t\"\xdd\x02\n\x0f\x44\x61taAcquisition\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x0c\n\x04host\x18\x02 \x01(\t\x12/\n\x07request\x18\x03 \x01(\x0b\x32\x1e.bosdyn.api.AcquireDataRequest\x12S\n\x13\x63ompletion_behavior\x18\x04 \x01(\x0e\x32\x36.bosdyn.api.mission.DataAcquisition.CompletionBehavior\x12\x19\n\x11group_name_format\x18\x05 \x01(\t\x12\"\n\x1arequest_name_in_blackboard\x18\x06 \x01(\t\"a\n\x12\x43ompletionBehavior\x12\x14\n\x10\x43OMPLETE_UNKNOWN\x10\x00\x12\x18\n\x14\x43OMPLETE_AFTER_SAVED\x10\x01\x12\x1b\n\x17\x43OMPLETE_AFTER_ACQUIRED\x10\x02\"1\n\x0bRetainLease\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x0c\n\x04host\x18\x02 \x01(\t\"w\n\x10\x44\x65\x66ineBlackboard\x12:\n\x14\x62lackboard_variables\x18\x01 \x03(\x0b\x32\x1c.bosdyn.api.mission.KeyValue\x12\'\n\x05\x63hild\x18\x02 \x01(\x0b\x32\x18.bosdyn.api.mission.Node\"K\n\rSetBlackboard\x12:\n\x14\x62lackboard_variables\x18\x01 \x03(\x0b\x32\x1c.bosdyn.api.mission.KeyValue\"/\n\x10\x46ormatBlackboard\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x0e\n\x06\x66ormat\x18\x02 \x01(\t\"\x1f\n\x10\x44\x61teToBlackboard\x12\x0b\n\x03key\x18\x01 \x01(\t\"<\n\x0e\x43onstantResult\x12*\n\x06result\x18\x01 \x01(\x0e\x32\x1a.bosdyn.api.mission.Result\"<\n\x11RestartWhenPaused\x12\'\n\x05\x63hild\x18\x01 \x01(\x0b\x32\x18.bosdyn.api.mission.Node\"\xef\x01\n\x13\x43learBehaviorFaults\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x0c\n\x04host\x18\x02 \x01(\t\x12#\n\x1brobot_state_blackboard_name\x18\x03 \x01(\t\x12*\n\"cleared_cause_fall_blackboard_name\x18\x04 \x01(\t\x12.\n&cleared_cause_hardware_blackboard_name\x18\x05 \x01(\t\x12\x33\n+cleared_cause_lease_timeout_blackboard_name\x18\x06 \x01(\tB\x0c\x42\nNodesProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1e\x62osdyn/api/mission/nodes.proto\x12\x12\x62osdyn.api.mission\x1a\x19google/protobuf/any.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x17\x62osdyn/api/alerts.proto\x1a bosdyn/api/docking/docking.proto\x1a\x19\x62osdyn/api/geometry.proto\x1a%bosdyn/api/gripper_camera_param.proto\x1a bosdyn/api/spot_cam/camera.proto\x1a!bosdyn/api/spot_cam/logging.proto\x1a\x1d\x62osdyn/api/spot_cam/ptz.proto\x1a\x1e\x62osdyn/api/robot_command.proto\x1a\x16\x62osdyn/api/power.proto\x1a!bosdyn/api/data_acquisition.proto\x1a\x1c\x62osdyn/api/data_buffer.proto\x1a$bosdyn/api/graph_nav/graph_nav.proto\x1a\x1e\x62osdyn/api/graph_nav/nav.proto\x1a!bosdyn/api/manipulation_api.proto\x1a\x1d\x62osdyn/api/mission/util.proto\x1a&bosdyn/api/service_customization.proto\"\xc9\x02\n\x04Node\x12\x0c\n\x04name\x18\x01 \x01(\t\x12/\n\tuser_data\x18\x02 \x01(\x0b\x32\x1c.bosdyn.api.mission.UserData\x12\x14\n\x0creference_id\x18\x03 \x01(\t\x12$\n\x04impl\x18\x04 \x01(\x0b\x32\x14.google.protobuf.AnyH\x00\x12\x18\n\x0enode_reference\x18\x05 \x01(\tH\x00\x12\x36\n\x10parameter_values\x18\x06 \x03(\x0b\x32\x1c.bosdyn.api.mission.KeyValue\x12/\n\toverrides\x18\x07 \x03(\x0b\x32\x1c.bosdyn.api.mission.KeyValue\x12;\n\nparameters\x18\x08 \x03(\x0b\x32\'.bosdyn.api.mission.VariableDeclarationB\x06\n\x04type\"N\n\x08Sequence\x12\x16\n\x0e\x61lways_restart\x18\x01 \x01(\x08\x12*\n\x08\x63hildren\x18\x02 \x03(\x0b\x32\x18.bosdyn.api.mission.Node\"N\n\x08Selector\x12\x16\n\x0e\x61lways_restart\x18\x01 \x01(\x08\x12*\n\x08\x63hildren\x18\x02 \x03(\x0b\x32\x18.bosdyn.api.mission.Node\"\x92\x02\n\x06Switch\x12.\n\x0bpivot_value\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.mission.Value\x12\x16\n\x0e\x61lways_restart\x18\x02 \x01(\x08\x12\x41\n\x0cint_children\x18\x03 \x03(\x0b\x32+.bosdyn.api.mission.Switch.IntChildrenEntry\x12/\n\rdefault_child\x18\x04 \x01(\x0b\x32\x18.bosdyn.api.mission.Node\x1aL\n\x10IntChildrenEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12\'\n\x05value\x18\x02 \x01(\x0b\x32\x18.bosdyn.api.mission.Node:\x02\x38\x01\"\x86\x01\n\x06Repeat\x12\x12\n\nmax_starts\x18\x01 \x01(\x05\x12\'\n\x05\x63hild\x18\x04 \x01(\x0b\x32\x18.bosdyn.api.mission.Node\x12 \n\x18start_counter_state_name\x18\x05 \x01(\t\x12\x1d\n\x15respect_child_failure\x18\x06 \x01(\x08\"j\n\x05Retry\x12\x14\n\x0cmax_attempts\x18\x01 \x01(\x05\x12\'\n\x05\x63hild\x18\x02 \x01(\x0b\x32\x18.bosdyn.api.mission.Node\x12\"\n\x1a\x61ttempt_counter_state_name\x18\x05 \x01(\t\"\xb1\x01\n\x0b\x46orDuration\x12+\n\x08\x64uration\x18\x01 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\'\n\x05\x63hild\x18\x02 \x01(\x0b\x32\x18.bosdyn.api.mission.Node\x12\x1b\n\x13time_remaining_name\x18\x03 \x01(\t\x12/\n\rtimeout_child\x18\x04 \x01(\x0b\x32\x18.bosdyn.api.mission.Node\"\x89\x01\n\x0eSimpleParallel\x12)\n\x07primary\x18\x01 \x01(\x0b\x32\x18.bosdyn.api.mission.Node\x12+\n\tsecondary\x18\x02 \x01(\x0b\x32\x18.bosdyn.api.mission.Node\x12\x1f\n\x17run_secondary_node_once\x18\x03 \x01(\x08\"T\n\x0bParallelAnd\x12*\n\x08\x63hildren\x18\x01 \x03(\x0b\x32\x18.bosdyn.api.mission.Node\x12\x19\n\x11\x66inish_every_node\x18\x02 \x01(\x08\"\xfa\x04\n\tCondition\x12\x32\n\x03lhs\x18\x01 \x01(\x0b\x32%.bosdyn.api.mission.Condition.Operand\x12\x32\n\x03rhs\x18\x02 \x01(\x0b\x32%.bosdyn.api.mission.Condition.Operand\x12\x38\n\toperation\x18\x05 \x01(\x0e\x32%.bosdyn.api.mission.Condition.Compare\x12G\n\x10handle_staleness\x18\x06 \x01(\x0e\x32-.bosdyn.api.mission.Condition.HandleStaleness\x1a}\n\x07Operand\x12\x36\n\x03var\x18\x01 \x01(\x0b\x32\'.bosdyn.api.mission.VariableDeclarationH\x00\x12\x32\n\x05\x63onst\x18\x02 \x01(\x0b\x32!.bosdyn.api.mission.ConstantValueH\x00\x42\x06\n\x04type\"~\n\x07\x43ompare\x12\x13\n\x0f\x43OMPARE_UNKNOWN\x10\x00\x12\x0e\n\nCOMPARE_EQ\x10\x01\x12\x0e\n\nCOMPARE_NE\x10\x02\x12\x0e\n\nCOMPARE_LT\x10\x03\x12\x0e\n\nCOMPARE_GT\x10\x04\x12\x0e\n\nCOMPARE_LE\x10\x05\x12\x0e\n\nCOMPARE_GE\x10\x06\"\x82\x01\n\x0fHandleStaleness\x12\x18\n\x14HANDLE_STALE_UNKNOWN\x10\x00\x12\x1c\n\x18HANDLE_STALE_READ_ANYWAY\x10\x01\x12 \n\x1cHANDLE_STALE_RUN_UNTIL_FRESH\x10\x02\x12\x15\n\x11HANDLE_STALE_FAIL\x10\x03\"s\n\x10\x42osdynRobotState\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x0c\n\x04host\x18\x02 \x01(\t\x12\'\n\x05\x63hild\x18\x03 \x01(\x0b\x32\x18.bosdyn.api.mission.Node\x12\x12\n\nstate_name\x18\x04 \x01(\t\"r\n\x0f\x42osdynDockState\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x0c\n\x04host\x18\x02 \x01(\t\x12\'\n\x05\x63hild\x18\x03 \x01(\x0b\x32\x18.bosdyn.api.mission.Node\x12\x12\n\nstate_name\x18\x04 \x01(\t\"c\n\x12\x42osdynRobotCommand\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x0c\n\x04host\x18\x02 \x01(\t\x12)\n\x07\x63ommand\x18\x03 \x01(\x0b\x32\x18.bosdyn.api.RobotCommand\"r\n\x12\x42osdynPowerRequest\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x0c\n\x04host\x18\x02 \x01(\t\x12\x38\n\x07request\x18\x04 \x01(\x0e\x32\'.bosdyn.api.PowerCommandRequest.Request\"\x95\x03\n\x10\x42osdynNavigateTo\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x0c\n\x04host\x18\x02 \x01(\t\x12\x1f\n\x17\x64\x65stination_waypoint_id\x18\x03 \x01(\t\x12>\n\x10route_gen_params\x18\x04 \x01(\x0b\x32$.bosdyn.api.graph_nav.RouteGenParams\x12\x39\n\rtravel_params\x18\x05 \x01(\x0b\x32\".bosdyn.api.graph_nav.TravelParams\x12\x33\n+navigation_feedback_response_blackboard_key\x18\x06 \x01(\t\x12+\n#navigate_to_response_blackboard_key\x18\x07 \x01(\t\x12_\n\x16route_blocked_behavior\x18\x08 \x01(\x0e\x32?.bosdyn.api.graph_nav.RouteFollowingParams.RouteBlockedBehavior\"\xce\x02\n\x13\x42osdynNavigateRoute\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x0c\n\x04host\x18\x02 \x01(\t\x12*\n\x05route\x18\x03 \x01(\x0b\x32\x1b.bosdyn.api.graph_nav.Route\x12G\n\x13route_follow_params\x18\x04 \x01(\x0b\x32*.bosdyn.api.graph_nav.RouteFollowingParams\x12\x39\n\rtravel_params\x18\x05 \x01(\x0b\x32\".bosdyn.api.graph_nav.TravelParams\x12\x33\n+navigation_feedback_response_blackboard_key\x18\x06 \x01(\t\x12.\n&navigate_route_response_blackboard_key\x18\x07 \x01(\t\"\x8b\x01\n\x13\x42osdynGraphNavState\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x0c\n\x04host\x18\x02 \x01(\t\x12\'\n\x05\x63hild\x18\x03 \x01(\x0b\x32\x18.bosdyn.api.mission.Node\x12\x12\n\nstate_name\x18\x04 \x01(\t\x12\x13\n\x0bwaypoint_id\x18\x05 \x01(\t\"\xbc\x01\n\x16\x42osdynGraphNavLocalize\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x0c\n\x04host\x18\x02 \x01(\t\x12J\n\x14localization_request\x18\x03 \x01(\x0b\x32,.bosdyn.api.graph_nav.SetLocalizationRequest\x12\x19\n\x11\x61llow_bad_quality\x18\x04 \x01(\x08\x12\x17\n\x0fresponse_bb_key\x18\x05 \x01(\t\"\xa8\x02\n\x11\x42osdynRecordEvent\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x0c\n\x04host\x18\x02 \x01(\t\x12 \n\x05\x65vent\x18\x03 \x01(\x0b\x32\x11.bosdyn.api.Event\x12\x15\n\rsucceed_early\x18\x04 \x01(\x08\x12^\n\x15\x61\x64\x64itional_parameters\x18\x05 \x03(\x0b\x32?.bosdyn.api.mission.BosdynRecordEvent.AdditionalParametersEntry\x1aV\n\x19\x41\x64\x64itionalParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12(\n\x05value\x18\x02 \x01(\x0b\x32\x19.bosdyn.api.mission.Value:\x02\x38\x01\"\xca\x01\n\nRemoteGrpc\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x14\n\x0cservice_name\x18\x03 \x01(\t\x12\x0f\n\x07timeout\x18\x04 \x01(\x02\x12\x17\n\x0flease_resources\x18\x05 \x03(\t\x12,\n\x06inputs\x18\x06 \x03(\x0b\x32\x1c.bosdyn.api.mission.KeyValue\x12\x19\n\x11group_name_format\x18\x08 \x01(\t\x12%\n\x06params\x18\t \x01(\x0b\x32\x15.bosdyn.api.DictParam\"4\n\x05Sleep\x12\x0f\n\x07seconds\x18\x01 \x01(\x02\x12\x1a\n\x12restart_after_stop\x18\x02 \x01(\x08\"\xc8\x02\n\x06Prompt\x12\x17\n\x0f\x61lways_reprompt\x18\x01 \x01(\x08\x12\x0c\n\x04text\x18\x02 \x01(\t\x12\x0e\n\x06source\x18\x03 \x01(\t\x12\x32\n\x07options\x18\x04 \x03(\x0b\x32!.bosdyn.api.mission.Prompt.Option\x12\'\n\x05\x63hild\x18\x05 \x01(\x0b\x32\x18.bosdyn.api.mission.Node\x12!\n\x19\x66or_autonomous_processing\x18\x06 \x01(\x08\x12\x35\n\x08severity\x18\x07 \x01(\x0e\x32#.bosdyn.api.AlertData.SeverityLevel\x12#\n\x1bquestion_name_in_blackboard\x18\x08 \x01(\t\x1a+\n\x06Option\x12\x0c\n\x04text\x18\x01 \x01(\t\x12\x13\n\x0b\x61nswer_code\x18\x02 \x01(\x03\"\x81\x01\n\x1e\x42osdynGripperCameraParamsState\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x0c\n\x04host\x18\x02 \x01(\t\x12\'\n\x05\x63hild\x18\x03 \x01(\x0b\x32\x18.bosdyn.api.mission.Node\x12\x12\n\nstate_name\x18\x04 \x01(\t\"\xa1\x01\n\x16SetGripperCameraParams\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x0c\n\x04host\x18\x02 \x01(\t\x12\"\n\x18params_in_blackboard_key\x18\x03 \x01(\tH\x00\x12\x35\n\nnew_params\x18\x04 \x01(\x0b\x32\x1f.bosdyn.api.GripperCameraParamsH\x00\x42\x08\n\x06params\"{\n\x10SetGraspOverride\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x0c\n\x04host\x18\x02 \x01(\t\x12\x43\n\x16grasp_override_request\x18\x03 \x01(\x0b\x32#.bosdyn.api.ApiGraspOverrideRequest\"\xad\x02\n\nSpotCamPtz\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x0c\n\x04host\x18\x02 \x01(\t\x12\x36\n\x0cptz_position\x18\x03 \x01(\x0b\x32 .bosdyn.api.spot_cam.PtzPosition\x12J\n\x11\x61\x64just_parameters\x18\x04 \x01(\x0b\x32/.bosdyn.api.mission.SpotCamPtz.AdjustParameters\x1aw\n\x10\x41\x64justParameters\x12\x1c\n\x14localization_varname\x18\x04 \x01(\t\x12\x13\n\x0bwaypoint_id\x18\x05 \x01(\t\x12\x30\n\x13waypoint_tform_body\x18\x06 \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\"\xa9\x01\n\x11SpotCamStoreMedia\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x0c\n\x04host\x18\x02 \x01(\t\x12+\n\x06\x63\x61mera\x18\x03 \x01(\x0b\x32\x1b.bosdyn.api.spot_cam.Camera\x12\x36\n\x04type\x18\x04 \x01(\x0e\x32(.bosdyn.api.spot_cam.Logpoint.RecordType\x12\x0b\n\x03tag\x18\x05 \x01(\t\"\xad\x01\n\nSpotCamLed\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x0c\n\x04host\x18\x02 \x01(\t\x12\x46\n\x0c\x62rightnesses\x18\x03 \x03(\x0b\x32\x30.bosdyn.api.mission.SpotCamLed.BrightnessesEntry\x1a\x33\n\x11\x42rightnessesEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\x02:\x02\x38\x01\";\n\x15SpotCamResetAutofocus\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x0c\n\x04host\x18\x02 \x01(\t\"\xfd\x02\n\x04\x44ock\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x0c\n\x04host\x18\x02 \x01(\t\x12\x1a\n\x12\x64ocking_station_id\x18\x03 \x01(\r\x12+\n\x05\x63hild\x18\x04 \x01(\x0b\x32\x18.bosdyn.api.mission.NodeB\x02\x18\x01\x12\x1f\n\x13\x63ommand_status_name\x18\x05 \x01(\tB\x02\x18\x01\x12 \n\x14\x66\x65\x65\x64\x62\x61\x63k_status_name\x18\x06 \x01(\tB\x02\x18\x01\x12@\n\x12prep_pose_behavior\x18\x07 \x01(\x0e\x32$.bosdyn.api.docking.PrepPoseBehavior\x12\x38\n0docking_command_feedback_response_blackboard_key\x18\x08 \x01(\t\x12/\n\'docking_command_response_blackboard_key\x18\t \x01(\t\x12\x18\n\x10require_fiducial\x18\n \x01(\x08\"\xc3\x01\n\rStoreMetadata\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x0c\n\x04host\x18\x02 \x01(\t\x12!\n\x19\x61\x63quire_data_request_name\x18\x03 \x01(\t\x12\x17\n\rmetadata_name\x18\x05 \x01(\tH\x00\x12\x30\n\rmetadata_json\x18\x07 \x01(\x0b\x32\x17.google.protobuf.StructH\x00\x12\x18\n\x10metadata_channel\x18\x06 \x01(\tB\x06\n\x04\x64\x61ta\"\xc7\x03\n\x0f\x44\x61taAcquisition\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x0c\n\x04host\x18\x02 \x01(\t\x12/\n\x07request\x18\x03 \x01(\x0b\x32\x1e.bosdyn.api.AcquireDataRequest\x12S\n\x13\x63ompletion_behavior\x18\x04 \x01(\x0e\x32\x36.bosdyn.api.mission.DataAcquisition.CompletionBehavior\x12\x19\n\x11group_name_format\x18\x05 \x01(\t\x12\"\n\x1arequest_name_in_blackboard\x18\x06 \x01(\t\x12#\n\x1bmetadata_name_in_blackboard\x18\t \x01(\t\x12\x1a\n\x12\x61\x63tion_name_format\x18\x07 \x01(\t\x12\'\n\x1f\x64isable_cancel_on_pause_or_stop\x18\x08 \x01(\x08\"a\n\x12\x43ompletionBehavior\x12\x14\n\x10\x43OMPLETE_UNKNOWN\x10\x00\x12\x18\n\x14\x43OMPLETE_AFTER_SAVED\x10\x01\x12\x1b\n\x17\x43OMPLETE_AFTER_ACQUIRED\x10\x02\"1\n\x0bRetainLease\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x0c\n\x04host\x18\x02 \x01(\t\"w\n\x10\x44\x65\x66ineBlackboard\x12:\n\x14\x62lackboard_variables\x18\x01 \x03(\x0b\x32\x1c.bosdyn.api.mission.KeyValue\x12\'\n\x05\x63hild\x18\x02 \x01(\x0b\x32\x18.bosdyn.api.mission.Node\"K\n\rSetBlackboard\x12:\n\x14\x62lackboard_variables\x18\x01 \x03(\x0b\x32\x1c.bosdyn.api.mission.KeyValue\"/\n\x10\x46ormatBlackboard\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x0e\n\x06\x66ormat\x18\x02 \x01(\t\"\x1f\n\x10\x44\x61teToBlackboard\x12\x0b\n\x03key\x18\x01 \x01(\t\"<\n\x0e\x43onstantResult\x12*\n\x06result\x18\x01 \x01(\x0e\x32\x1a.bosdyn.api.mission.Result\"<\n\x11RestartWhenPaused\x12\'\n\x05\x63hild\x18\x01 \x01(\x0b\x32\x18.bosdyn.api.mission.Node\"\xb2\x05\n\x1d\x44\x61taAcquisitionOnInterruption\x12\'\n\x05\x63hild\x18\x01 \x01(\x0b\x32\x18.bosdyn.api.mission.Node\x12\x45\n\x18request_when_interrupted\x18\x02 \x01(\x0b\x32#.bosdyn.api.mission.DataAcquisition\x12\x34\n\x16pause_mission_metadata\x18\x04 \x01(\x0b\x32\x14.bosdyn.api.Metadata\x12\x36\n\x18restart_mission_metadata\x18\x05 \x01(\x0b\x32\x14.bosdyn.api.Metadata\x12\x33\n\x15load_mission_metadata\x18\x06 \x01(\x0b\x32\x14.bosdyn.api.Metadata\x12\x33\n\x15stop_mission_metadata\x18\x07 \x01(\x0b\x32\x14.bosdyn.api.Metadata\x12\x36\n\x18lease_use_error_metadata\x18\x08 \x01(\x0b\x32\x14.bosdyn.api.Metadata\x12;\n\x1dplay_mission_timeout_metadata\x18\t \x01(\x0b\x32\x14.bosdyn.api.Metadata\x12\x37\n\x19\x63hild_node_error_metadata\x18\n \x01(\x0b\x32\x14.bosdyn.api.Metadata\x12;\n\x1d\x63hild_node_exception_metadata\x18\x0b \x01(\x0b\x32\x14.bosdyn.api.Metadata\x12.\n\x10\x64\x65\x66\x61ult_metadata\x18\x0c \x01(\x0b\x32\x14.bosdyn.api.Metadata\x12(\n keys_for_lease_use_error_message\x18\r \x03(\tJ\x04\x08\x03\x10\x04\"\xef\x01\n\x13\x43learBehaviorFaults\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x0c\n\x04host\x18\x02 \x01(\t\x12#\n\x1brobot_state_blackboard_name\x18\x03 \x01(\t\x12*\n\"cleared_cause_fall_blackboard_name\x18\x04 \x01(\t\x12.\n&cleared_cause_hardware_blackboard_name\x18\x05 \x01(\t\x12\x33\n+cleared_cause_lease_timeout_blackboard_name\x18\x06 \x01(\tB\x0c\x42\nNodesProtob\x06proto3')
 
 
 
 _NODE = DESCRIPTOR.message_types_by_name['Node']
 _SEQUENCE = DESCRIPTOR.message_types_by_name['Sequence']
 _SELECTOR = DESCRIPTOR.message_types_by_name['Selector']
 _SWITCH = DESCRIPTOR.message_types_by_name['Switch']
 _SWITCH_INTCHILDRENENTRY = _SWITCH.nested_types_by_name['IntChildrenEntry']
 _REPEAT = DESCRIPTOR.message_types_by_name['Repeat']
 _RETRY = DESCRIPTOR.message_types_by_name['Retry']
 _FORDURATION = DESCRIPTOR.message_types_by_name['ForDuration']
 _SIMPLEPARALLEL = DESCRIPTOR.message_types_by_name['SimpleParallel']
+_PARALLELAND = DESCRIPTOR.message_types_by_name['ParallelAnd']
 _CONDITION = DESCRIPTOR.message_types_by_name['Condition']
 _CONDITION_OPERAND = _CONDITION.nested_types_by_name['Operand']
 _BOSDYNROBOTSTATE = DESCRIPTOR.message_types_by_name['BosdynRobotState']
 _BOSDYNDOCKSTATE = DESCRIPTOR.message_types_by_name['BosdynDockState']
 _BOSDYNROBOTCOMMAND = DESCRIPTOR.message_types_by_name['BosdynRobotCommand']
 _BOSDYNPOWERREQUEST = DESCRIPTOR.message_types_by_name['BosdynPowerRequest']
 _BOSDYNNAVIGATETO = DESCRIPTOR.message_types_by_name['BosdynNavigateTo']
@@ -57,14 +61,15 @@
 _BOSDYNRECORDEVENT_ADDITIONALPARAMETERSENTRY = _BOSDYNRECORDEVENT.nested_types_by_name['AdditionalParametersEntry']
 _REMOTEGRPC = DESCRIPTOR.message_types_by_name['RemoteGrpc']
 _SLEEP = DESCRIPTOR.message_types_by_name['Sleep']
 _PROMPT = DESCRIPTOR.message_types_by_name['Prompt']
 _PROMPT_OPTION = _PROMPT.nested_types_by_name['Option']
 _BOSDYNGRIPPERCAMERAPARAMSSTATE = DESCRIPTOR.message_types_by_name['BosdynGripperCameraParamsState']
 _SETGRIPPERCAMERAPARAMS = DESCRIPTOR.message_types_by_name['SetGripperCameraParams']
+_SETGRASPOVERRIDE = DESCRIPTOR.message_types_by_name['SetGraspOverride']
 _SPOTCAMPTZ = DESCRIPTOR.message_types_by_name['SpotCamPtz']
 _SPOTCAMPTZ_ADJUSTPARAMETERS = _SPOTCAMPTZ.nested_types_by_name['AdjustParameters']
 _SPOTCAMSTOREMEDIA = DESCRIPTOR.message_types_by_name['SpotCamStoreMedia']
 _SPOTCAMLED = DESCRIPTOR.message_types_by_name['SpotCamLed']
 _SPOTCAMLED_BRIGHTNESSESENTRY = _SPOTCAMLED.nested_types_by_name['BrightnessesEntry']
 _SPOTCAMRESETAUTOFOCUS = DESCRIPTOR.message_types_by_name['SpotCamResetAutofocus']
 _DOCK = DESCRIPTOR.message_types_by_name['Dock']
@@ -73,14 +78,15 @@
 _RETAINLEASE = DESCRIPTOR.message_types_by_name['RetainLease']
 _DEFINEBLACKBOARD = DESCRIPTOR.message_types_by_name['DefineBlackboard']
 _SETBLACKBOARD = DESCRIPTOR.message_types_by_name['SetBlackboard']
 _FORMATBLACKBOARD = DESCRIPTOR.message_types_by_name['FormatBlackboard']
 _DATETOBLACKBOARD = DESCRIPTOR.message_types_by_name['DateToBlackboard']
 _CONSTANTRESULT = DESCRIPTOR.message_types_by_name['ConstantResult']
 _RESTARTWHENPAUSED = DESCRIPTOR.message_types_by_name['RestartWhenPaused']
+_DATAACQUISITIONONINTERRUPTION = DESCRIPTOR.message_types_by_name['DataAcquisitionOnInterruption']
 _CLEARBEHAVIORFAULTS = DESCRIPTOR.message_types_by_name['ClearBehaviorFaults']
 _CONDITION_COMPARE = _CONDITION.enum_types_by_name['Compare']
 _CONDITION_HANDLESTALENESS = _CONDITION.enum_types_by_name['HandleStaleness']
 _DATAACQUISITION_COMPLETIONBEHAVIOR = _DATAACQUISITION.enum_types_by_name['CompletionBehavior']
 Node = _reflection.GeneratedProtocolMessageType('Node', (_message.Message,), {
   'DESCRIPTOR' : _NODE,
   '__module__' : 'bosdyn.api.mission.nodes_pb2'
@@ -141,14 +147,21 @@
 SimpleParallel = _reflection.GeneratedProtocolMessageType('SimpleParallel', (_message.Message,), {
   'DESCRIPTOR' : _SIMPLEPARALLEL,
   '__module__' : 'bosdyn.api.mission.nodes_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.mission.SimpleParallel)
   })
 _sym_db.RegisterMessage(SimpleParallel)
 
+ParallelAnd = _reflection.GeneratedProtocolMessageType('ParallelAnd', (_message.Message,), {
+  'DESCRIPTOR' : _PARALLELAND,
+  '__module__' : 'bosdyn.api.mission.nodes_pb2'
+  # @@protoc_insertion_point(class_scope:bosdyn.api.mission.ParallelAnd)
+  })
+_sym_db.RegisterMessage(ParallelAnd)
+
 Condition = _reflection.GeneratedProtocolMessageType('Condition', (_message.Message,), {
 
   'Operand' : _reflection.GeneratedProtocolMessageType('Operand', (_message.Message,), {
     'DESCRIPTOR' : _CONDITION_OPERAND,
     '__module__' : 'bosdyn.api.mission.nodes_pb2'
     # @@protoc_insertion_point(class_scope:bosdyn.api.mission.Condition.Operand)
     })
@@ -270,14 +283,21 @@
 SetGripperCameraParams = _reflection.GeneratedProtocolMessageType('SetGripperCameraParams', (_message.Message,), {
   'DESCRIPTOR' : _SETGRIPPERCAMERAPARAMS,
   '__module__' : 'bosdyn.api.mission.nodes_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.mission.SetGripperCameraParams)
   })
 _sym_db.RegisterMessage(SetGripperCameraParams)
 
+SetGraspOverride = _reflection.GeneratedProtocolMessageType('SetGraspOverride', (_message.Message,), {
+  'DESCRIPTOR' : _SETGRASPOVERRIDE,
+  '__module__' : 'bosdyn.api.mission.nodes_pb2'
+  # @@protoc_insertion_point(class_scope:bosdyn.api.mission.SetGraspOverride)
+  })
+_sym_db.RegisterMessage(SetGraspOverride)
+
 SpotCamPtz = _reflection.GeneratedProtocolMessageType('SpotCamPtz', (_message.Message,), {
 
   'AdjustParameters' : _reflection.GeneratedProtocolMessageType('AdjustParameters', (_message.Message,), {
     'DESCRIPTOR' : _SPOTCAMPTZ_ADJUSTPARAMETERS,
     '__module__' : 'bosdyn.api.mission.nodes_pb2'
     # @@protoc_insertion_point(class_scope:bosdyn.api.mission.SpotCamPtz.AdjustParameters)
     })
@@ -384,14 +404,21 @@
 RestartWhenPaused = _reflection.GeneratedProtocolMessageType('RestartWhenPaused', (_message.Message,), {
   'DESCRIPTOR' : _RESTARTWHENPAUSED,
   '__module__' : 'bosdyn.api.mission.nodes_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.mission.RestartWhenPaused)
   })
 _sym_db.RegisterMessage(RestartWhenPaused)
 
+DataAcquisitionOnInterruption = _reflection.GeneratedProtocolMessageType('DataAcquisitionOnInterruption', (_message.Message,), {
+  'DESCRIPTOR' : _DATAACQUISITIONONINTERRUPTION,
+  '__module__' : 'bosdyn.api.mission.nodes_pb2'
+  # @@protoc_insertion_point(class_scope:bosdyn.api.mission.DataAcquisitionOnInterruption)
+  })
+_sym_db.RegisterMessage(DataAcquisitionOnInterruption)
+
 ClearBehaviorFaults = _reflection.GeneratedProtocolMessageType('ClearBehaviorFaults', (_message.Message,), {
   'DESCRIPTOR' : _CLEARBEHAVIORFAULTS,
   '__module__' : 'bosdyn.api.mission.nodes_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.mission.ClearBehaviorFaults)
   })
 _sym_db.RegisterMessage(ClearBehaviorFaults)
 
@@ -407,102 +434,108 @@
   _SPOTCAMLED_BRIGHTNESSESENTRY._serialized_options = b'8\001'
   _DOCK.fields_by_name['child']._options = None
   _DOCK.fields_by_name['child']._serialized_options = b'\030\001'
   _DOCK.fields_by_name['command_status_name']._options = None
   _DOCK.fields_by_name['command_status_name']._serialized_options = b'\030\001'
   _DOCK.fields_by_name['feedback_status_name']._options = None
   _DOCK.fields_by_name['feedback_status_name']._serialized_options = b'\030\001'
-  _NODE._serialized_start=561
-  _NODE._serialized_end=890
-  _SEQUENCE._serialized_start=892
-  _SEQUENCE._serialized_end=970
-  _SELECTOR._serialized_start=972
-  _SELECTOR._serialized_end=1050
-  _SWITCH._serialized_start=1053
-  _SWITCH._serialized_end=1327
-  _SWITCH_INTCHILDRENENTRY._serialized_start=1251
-  _SWITCH_INTCHILDRENENTRY._serialized_end=1327
-  _REPEAT._serialized_start=1330
-  _REPEAT._serialized_end=1464
-  _RETRY._serialized_start=1466
-  _RETRY._serialized_end=1572
-  _FORDURATION._serialized_start=1575
-  _FORDURATION._serialized_end=1752
-  _SIMPLEPARALLEL._serialized_start=1754
-  _SIMPLEPARALLEL._serialized_end=1858
-  _CONDITION._serialized_start=1861
-  _CONDITION._serialized_end=2495
-  _CONDITION_OPERAND._serialized_start=2109
-  _CONDITION_OPERAND._serialized_end=2234
-  _CONDITION_COMPARE._serialized_start=2236
-  _CONDITION_COMPARE._serialized_end=2362
-  _CONDITION_HANDLESTALENESS._serialized_start=2365
-  _CONDITION_HANDLESTALENESS._serialized_end=2495
-  _BOSDYNROBOTSTATE._serialized_start=2497
-  _BOSDYNROBOTSTATE._serialized_end=2612
-  _BOSDYNDOCKSTATE._serialized_start=2614
-  _BOSDYNDOCKSTATE._serialized_end=2728
-  _BOSDYNROBOTCOMMAND._serialized_start=2730
-  _BOSDYNROBOTCOMMAND._serialized_end=2829
-  _BOSDYNPOWERREQUEST._serialized_start=2831
-  _BOSDYNPOWERREQUEST._serialized_end=2945
-  _BOSDYNNAVIGATETO._serialized_start=2948
-  _BOSDYNNAVIGATETO._serialized_end=3256
-  _BOSDYNNAVIGATEROUTE._serialized_start=3259
-  _BOSDYNNAVIGATEROUTE._serialized_end=3593
-  _BOSDYNGRAPHNAVSTATE._serialized_start=3596
-  _BOSDYNGRAPHNAVSTATE._serialized_end=3735
-  _BOSDYNGRAPHNAVLOCALIZE._serialized_start=3738
-  _BOSDYNGRAPHNAVLOCALIZE._serialized_end=3874
-  _BOSDYNRECORDEVENT._serialized_start=3877
-  _BOSDYNRECORDEVENT._serialized_end=4173
-  _BOSDYNRECORDEVENT_ADDITIONALPARAMETERSENTRY._serialized_start=4087
-  _BOSDYNRECORDEVENT_ADDITIONALPARAMETERSENTRY._serialized_end=4173
-  _REMOTEGRPC._serialized_start=4176
-  _REMOTEGRPC._serialized_end=4312
-  _SLEEP._serialized_start=4314
-  _SLEEP._serialized_end=4366
-  _PROMPT._serialized_start=4369
-  _PROMPT._serialized_end=4660
-  _PROMPT_OPTION._serialized_start=4617
-  _PROMPT_OPTION._serialized_end=4660
-  _BOSDYNGRIPPERCAMERAPARAMSSTATE._serialized_start=4663
-  _BOSDYNGRIPPERCAMERAPARAMSSTATE._serialized_end=4792
-  _SETGRIPPERCAMERAPARAMS._serialized_start=4795
-  _SETGRIPPERCAMERAPARAMS._serialized_end=4956
-  _SPOTCAMPTZ._serialized_start=4959
-  _SPOTCAMPTZ._serialized_end=5260
-  _SPOTCAMPTZ_ADJUSTPARAMETERS._serialized_start=5141
-  _SPOTCAMPTZ_ADJUSTPARAMETERS._serialized_end=5260
-  _SPOTCAMSTOREMEDIA._serialized_start=5263
-  _SPOTCAMSTOREMEDIA._serialized_end=5432
-  _SPOTCAMLED._serialized_start=5435
-  _SPOTCAMLED._serialized_end=5608
-  _SPOTCAMLED_BRIGHTNESSESENTRY._serialized_start=5557
-  _SPOTCAMLED_BRIGHTNESSESENTRY._serialized_end=5608
-  _SPOTCAMRESETAUTOFOCUS._serialized_start=5610
-  _SPOTCAMRESETAUTOFOCUS._serialized_end=5669
-  _DOCK._serialized_start=5672
-  _DOCK._serialized_end=6027
-  _STOREMETADATA._serialized_start=6030
-  _STOREMETADATA._serialized_end=6165
-  _DATAACQUISITION._serialized_start=6168
-  _DATAACQUISITION._serialized_end=6517
-  _DATAACQUISITION_COMPLETIONBEHAVIOR._serialized_start=6420
-  _DATAACQUISITION_COMPLETIONBEHAVIOR._serialized_end=6517
-  _RETAINLEASE._serialized_start=6519
-  _RETAINLEASE._serialized_end=6568
-  _DEFINEBLACKBOARD._serialized_start=6570
-  _DEFINEBLACKBOARD._serialized_end=6689
-  _SETBLACKBOARD._serialized_start=6691
-  _SETBLACKBOARD._serialized_end=6766
-  _FORMATBLACKBOARD._serialized_start=6768
-  _FORMATBLACKBOARD._serialized_end=6815
-  _DATETOBLACKBOARD._serialized_start=6817
-  _DATETOBLACKBOARD._serialized_end=6848
-  _CONSTANTRESULT._serialized_start=6850
-  _CONSTANTRESULT._serialized_end=6910
-  _RESTARTWHENPAUSED._serialized_start=6912
-  _RESTARTWHENPAUSED._serialized_end=6972
-  _CLEARBEHAVIORFAULTS._serialized_start=6975
-  _CLEARBEHAVIORFAULTS._serialized_end=7214
+  _NODE._serialized_start=666
+  _NODE._serialized_end=995
+  _SEQUENCE._serialized_start=997
+  _SEQUENCE._serialized_end=1075
+  _SELECTOR._serialized_start=1077
+  _SELECTOR._serialized_end=1155
+  _SWITCH._serialized_start=1158
+  _SWITCH._serialized_end=1432
+  _SWITCH_INTCHILDRENENTRY._serialized_start=1356
+  _SWITCH_INTCHILDRENENTRY._serialized_end=1432
+  _REPEAT._serialized_start=1435
+  _REPEAT._serialized_end=1569
+  _RETRY._serialized_start=1571
+  _RETRY._serialized_end=1677
+  _FORDURATION._serialized_start=1680
+  _FORDURATION._serialized_end=1857
+  _SIMPLEPARALLEL._serialized_start=1860
+  _SIMPLEPARALLEL._serialized_end=1997
+  _PARALLELAND._serialized_start=1999
+  _PARALLELAND._serialized_end=2083
+  _CONDITION._serialized_start=2086
+  _CONDITION._serialized_end=2720
+  _CONDITION_OPERAND._serialized_start=2334
+  _CONDITION_OPERAND._serialized_end=2459
+  _CONDITION_COMPARE._serialized_start=2461
+  _CONDITION_COMPARE._serialized_end=2587
+  _CONDITION_HANDLESTALENESS._serialized_start=2590
+  _CONDITION_HANDLESTALENESS._serialized_end=2720
+  _BOSDYNROBOTSTATE._serialized_start=2722
+  _BOSDYNROBOTSTATE._serialized_end=2837
+  _BOSDYNDOCKSTATE._serialized_start=2839
+  _BOSDYNDOCKSTATE._serialized_end=2953
+  _BOSDYNROBOTCOMMAND._serialized_start=2955
+  _BOSDYNROBOTCOMMAND._serialized_end=3054
+  _BOSDYNPOWERREQUEST._serialized_start=3056
+  _BOSDYNPOWERREQUEST._serialized_end=3170
+  _BOSDYNNAVIGATETO._serialized_start=3173
+  _BOSDYNNAVIGATETO._serialized_end=3578
+  _BOSDYNNAVIGATEROUTE._serialized_start=3581
+  _BOSDYNNAVIGATEROUTE._serialized_end=3915
+  _BOSDYNGRAPHNAVSTATE._serialized_start=3918
+  _BOSDYNGRAPHNAVSTATE._serialized_end=4057
+  _BOSDYNGRAPHNAVLOCALIZE._serialized_start=4060
+  _BOSDYNGRAPHNAVLOCALIZE._serialized_end=4248
+  _BOSDYNRECORDEVENT._serialized_start=4251
+  _BOSDYNRECORDEVENT._serialized_end=4547
+  _BOSDYNRECORDEVENT_ADDITIONALPARAMETERSENTRY._serialized_start=4461
+  _BOSDYNRECORDEVENT_ADDITIONALPARAMETERSENTRY._serialized_end=4547
+  _REMOTEGRPC._serialized_start=4550
+  _REMOTEGRPC._serialized_end=4752
+  _SLEEP._serialized_start=4754
+  _SLEEP._serialized_end=4806
+  _PROMPT._serialized_start=4809
+  _PROMPT._serialized_end=5137
+  _PROMPT_OPTION._serialized_start=5094
+  _PROMPT_OPTION._serialized_end=5137
+  _BOSDYNGRIPPERCAMERAPARAMSSTATE._serialized_start=5140
+  _BOSDYNGRIPPERCAMERAPARAMSSTATE._serialized_end=5269
+  _SETGRIPPERCAMERAPARAMS._serialized_start=5272
+  _SETGRIPPERCAMERAPARAMS._serialized_end=5433
+  _SETGRASPOVERRIDE._serialized_start=5435
+  _SETGRASPOVERRIDE._serialized_end=5558
+  _SPOTCAMPTZ._serialized_start=5561
+  _SPOTCAMPTZ._serialized_end=5862
+  _SPOTCAMPTZ_ADJUSTPARAMETERS._serialized_start=5743
+  _SPOTCAMPTZ_ADJUSTPARAMETERS._serialized_end=5862
+  _SPOTCAMSTOREMEDIA._serialized_start=5865
+  _SPOTCAMSTOREMEDIA._serialized_end=6034
+  _SPOTCAMLED._serialized_start=6037
+  _SPOTCAMLED._serialized_end=6210
+  _SPOTCAMLED_BRIGHTNESSESENTRY._serialized_start=6159
+  _SPOTCAMLED_BRIGHTNESSESENTRY._serialized_end=6210
+  _SPOTCAMRESETAUTOFOCUS._serialized_start=6212
+  _SPOTCAMRESETAUTOFOCUS._serialized_end=6271
+  _DOCK._serialized_start=6274
+  _DOCK._serialized_end=6655
+  _STOREMETADATA._serialized_start=6658
+  _STOREMETADATA._serialized_end=6853
+  _DATAACQUISITION._serialized_start=6856
+  _DATAACQUISITION._serialized_end=7311
+  _DATAACQUISITION_COMPLETIONBEHAVIOR._serialized_start=7214
+  _DATAACQUISITION_COMPLETIONBEHAVIOR._serialized_end=7311
+  _RETAINLEASE._serialized_start=7313
+  _RETAINLEASE._serialized_end=7362
+  _DEFINEBLACKBOARD._serialized_start=7364
+  _DEFINEBLACKBOARD._serialized_end=7483
+  _SETBLACKBOARD._serialized_start=7485
+  _SETBLACKBOARD._serialized_end=7560
+  _FORMATBLACKBOARD._serialized_start=7562
+  _FORMATBLACKBOARD._serialized_end=7609
+  _DATETOBLACKBOARD._serialized_start=7611
+  _DATETOBLACKBOARD._serialized_end=7642
+  _CONSTANTRESULT._serialized_start=7644
+  _CONSTANTRESULT._serialized_end=7704
+  _RESTARTWHENPAUSED._serialized_start=7706
+  _RESTARTWHENPAUSED._serialized_end=7766
+  _DATAACQUISITIONONINTERRUPTION._serialized_start=7769
+  _DATAACQUISITIONONINTERRUPTION._serialized_end=8459
+  _CLEARBEHAVIORFAULTS._serialized_start=8462
+  _CLEARBEHAVIORFAULTS._serialized_end=8701
 # @@protoc_insertion_point(module_scope)
```

## bosdyn/api/mission/remote_pb2.py

```diff
@@ -10,29 +10,32 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from bosdyn.api import header_pb2 as bosdyn_dot_api_dot_header__pb2
 from bosdyn.api import lease_pb2 as bosdyn_dot_api_dot_lease__pb2
+from bosdyn.api import service_customization_pb2 as bosdyn_dot_api_dot_service__customization__pb2
 from bosdyn.api.mission import util_pb2 as bosdyn_dot_api_dot_mission_dot_util__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1f\x62osdyn/api/mission/remote.proto\x12\x12\x62osdyn.api.mission\x1a\x17\x62osdyn/api/header.proto\x1a\x16\x62osdyn/api/lease.proto\x1a\x1d\x62osdyn/api/mission/util.proto\"\xa0\x01\n\x17\x45stablishSessionRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12!\n\x06leases\x18\x02 \x03(\x0b\x32\x11.bosdyn.api.Lease\x12\x37\n\x06inputs\x18\x03 \x03(\x0b\x32\'.bosdyn.api.mission.VariableDeclaration\"\x9b\x03\n\x18\x45stablishSessionResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x43\n\x06status\x18\x02 \x01(\x0e\x32\x33.bosdyn.api.mission.EstablishSessionResponse.Status\x12\x12\n\nsession_id\x18\x03 \x01(\t\x12\x1f\n\x17missing_lease_resources\x18\x04 \x03(\t\x12\x35\n\x11lease_use_results\x18\x05 \x03(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12?\n\x0emissing_inputs\x18\x06 \x03(\x0b\x32\'.bosdyn.api.mission.VariableDeclaration\"a\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x19\n\x15STATUS_MISSING_LEASES\x10\x02\x12\x19\n\x15STATUS_MISSING_INPUTS\x10\x03\"\x9d\x01\n\x0bTickRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x12\n\nsession_id\x18\x02 \x01(\t\x12!\n\x06leases\x18\x03 \x03(\x0b\x32\x11.bosdyn.api.Lease\x12,\n\x06inputs\x18\x04 \x03(\x0b\x32\x1c.bosdyn.api.mission.KeyValue\"\xd3\x03\n\x0cTickResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x37\n\x06status\x18\x03 \x01(\x0e\x32\'.bosdyn.api.mission.TickResponse.Status\x12\x1f\n\x17missing_lease_resources\x18\x04 \x03(\t\x12\x35\n\x11lease_use_results\x18\x05 \x03(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12?\n\x0emissing_inputs\x18\x07 \x03(\x0b\x32\'.bosdyn.api.mission.VariableDeclaration\x12\x15\n\rerror_message\x18\x08 \x01(\t\"\xad\x01\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x12\n\x0eSTATUS_FAILURE\x10\x01\x12\x12\n\x0eSTATUS_RUNNING\x10\x02\x12\x12\n\x0eSTATUS_SUCCESS\x10\x03\x12\x1d\n\x19STATUS_INVALID_SESSION_ID\x10\x04\x12\x19\n\x15STATUS_MISSING_LEASES\x10\x05\x12\x19\n\x15STATUS_MISSING_INPUTS\x10\x06\"L\n\x0bStopRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x12\n\nsession_id\x18\x02 \x01(\t\"\xbf\x01\n\x0cStopResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x37\n\x06status\x18\x02 \x01(\x0e\x32\'.bosdyn.api.mission.StopResponse.Status\"J\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1d\n\x19STATUS_INVALID_SESSION_ID\x10\x02\"W\n\x16TeardownSessionRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x12\n\nsession_id\x18\x02 \x01(\t\"\xd5\x01\n\x17TeardownSessionResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x42\n\x06status\x18\x02 \x01(\x0e\x32\x32.bosdyn.api.mission.TeardownSessionResponse.Status\"J\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1d\n\x19STATUS_INVALID_SESSION_ID\x10\x02\x42\rB\x0bRemoteProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1f\x62osdyn/api/mission/remote.proto\x12\x12\x62osdyn.api.mission\x1a\x17\x62osdyn/api/header.proto\x1a\x16\x62osdyn/api/lease.proto\x1a&bosdyn/api/service_customization.proto\x1a\x1d\x62osdyn/api/mission/util.proto\"\xaa\x01\n\x17\x45stablishSessionRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12!\n\x06leases\x18\x02 \x03(\x0b\x32\x11.bosdyn.api.Lease\x12;\n\x06inputs\x18\x03 \x03(\x0b\x32\'.bosdyn.api.mission.VariableDeclarationB\x02\x18\x01J\x04\x08\x05\x10\x06\"\x9f\x03\n\x18\x45stablishSessionResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x43\n\x06status\x18\x02 \x01(\x0e\x32\x33.bosdyn.api.mission.EstablishSessionResponse.Status\x12\x12\n\nsession_id\x18\x03 \x01(\t\x12\x1f\n\x17missing_lease_resources\x18\x04 \x03(\t\x12\x35\n\x11lease_use_results\x18\x05 \x03(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12\x43\n\x0emissing_inputs\x18\x06 \x03(\x0b\x32\'.bosdyn.api.mission.VariableDeclarationB\x02\x18\x01\"a\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x19\n\x15STATUS_MISSING_LEASES\x10\x02\x12\x19\n\x15STATUS_MISSING_INPUTS\x10\x03\"\xd8\x01\n\x0bTickRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x12\n\nsession_id\x18\x02 \x01(\t\x12!\n\x06leases\x18\x03 \x03(\x0b\x32\x11.bosdyn.api.Lease\x12,\n\x06inputs\x18\x04 \x03(\x0b\x32\x1c.bosdyn.api.mission.KeyValue\x12%\n\x06params\x18\x05 \x01(\x0b\x32\x15.bosdyn.api.DictParam\x12\x12\n\ngroup_name\x18\x06 \x01(\t\"\xad\x04\n\x0cTickResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x37\n\x06status\x18\x03 \x01(\x0e\x32\'.bosdyn.api.mission.TickResponse.Status\x12\x1f\n\x17missing_lease_resources\x18\x04 \x03(\t\x12\x35\n\x11lease_use_results\x18\x05 \x03(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12?\n\x0emissing_inputs\x18\x07 \x03(\x0b\x32\'.bosdyn.api.mission.VariableDeclaration\x12\x15\n\rerror_message\x18\x08 \x01(\t\x12\x38\n\x12\x63ustom_param_error\x18\t \x01(\x0b\x32\x1c.bosdyn.api.CustomParamError\"\xcd\x01\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x12\n\x0eSTATUS_FAILURE\x10\x01\x12\x12\n\x0eSTATUS_RUNNING\x10\x02\x12\x12\n\x0eSTATUS_SUCCESS\x10\x03\x12\x1d\n\x19STATUS_INVALID_SESSION_ID\x10\x04\x12\x19\n\x15STATUS_MISSING_LEASES\x10\x05\x12\x19\n\x15STATUS_MISSING_INPUTS\x10\x06\x12\x1e\n\x1aSTATUS_CUSTOM_PARAMS_ERROR\x10\x07\"L\n\x0bStopRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x12\n\nsession_id\x18\x02 \x01(\t\"\xbf\x01\n\x0cStopResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x37\n\x06status\x18\x02 \x01(\x0e\x32\'.bosdyn.api.mission.StopResponse.Status\"J\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1d\n\x19STATUS_INVALID_SESSION_ID\x10\x02\"W\n\x16TeardownSessionRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x12\n\nsession_id\x18\x02 \x01(\t\"\xd5\x01\n\x17TeardownSessionResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x42\n\x06status\x18\x02 \x01(\x0e\x32\x32.bosdyn.api.mission.TeardownSessionResponse.Status\"J\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1d\n\x19STATUS_INVALID_SESSION_ID\x10\x02\"O\n\"GetRemoteMissionServiceInfoRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"\x84\x01\n#GetRemoteMissionServiceInfoResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x31\n\rcustom_params\x18\x02 \x01(\x0b\x32\x1a.bosdyn.api.DictParam.SpecB\rB\x0bRemoteProtob\x06proto3')
 
 
 
 _ESTABLISHSESSIONREQUEST = DESCRIPTOR.message_types_by_name['EstablishSessionRequest']
 _ESTABLISHSESSIONRESPONSE = DESCRIPTOR.message_types_by_name['EstablishSessionResponse']
 _TICKREQUEST = DESCRIPTOR.message_types_by_name['TickRequest']
 _TICKRESPONSE = DESCRIPTOR.message_types_by_name['TickResponse']
 _STOPREQUEST = DESCRIPTOR.message_types_by_name['StopRequest']
 _STOPRESPONSE = DESCRIPTOR.message_types_by_name['StopResponse']
 _TEARDOWNSESSIONREQUEST = DESCRIPTOR.message_types_by_name['TeardownSessionRequest']
 _TEARDOWNSESSIONRESPONSE = DESCRIPTOR.message_types_by_name['TeardownSessionResponse']
+_GETREMOTEMISSIONSERVICEINFOREQUEST = DESCRIPTOR.message_types_by_name['GetRemoteMissionServiceInfoRequest']
+_GETREMOTEMISSIONSERVICEINFORESPONSE = DESCRIPTOR.message_types_by_name['GetRemoteMissionServiceInfoResponse']
 _ESTABLISHSESSIONRESPONSE_STATUS = _ESTABLISHSESSIONRESPONSE.enum_types_by_name['Status']
 _TICKRESPONSE_STATUS = _TICKRESPONSE.enum_types_by_name['Status']
 _STOPRESPONSE_STATUS = _STOPRESPONSE.enum_types_by_name['Status']
 _TEARDOWNSESSIONRESPONSE_STATUS = _TEARDOWNSESSIONRESPONSE.enum_types_by_name['Status']
 EstablishSessionRequest = _reflection.GeneratedProtocolMessageType('EstablishSessionRequest', (_message.Message,), {
   'DESCRIPTOR' : _ESTABLISHSESSIONREQUEST,
   '__module__' : 'bosdyn.api.mission.remote_pb2'
@@ -85,36 +88,58 @@
 TeardownSessionResponse = _reflection.GeneratedProtocolMessageType('TeardownSessionResponse', (_message.Message,), {
   'DESCRIPTOR' : _TEARDOWNSESSIONRESPONSE,
   '__module__' : 'bosdyn.api.mission.remote_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.mission.TeardownSessionResponse)
   })
 _sym_db.RegisterMessage(TeardownSessionResponse)
 
+GetRemoteMissionServiceInfoRequest = _reflection.GeneratedProtocolMessageType('GetRemoteMissionServiceInfoRequest', (_message.Message,), {
+  'DESCRIPTOR' : _GETREMOTEMISSIONSERVICEINFOREQUEST,
+  '__module__' : 'bosdyn.api.mission.remote_pb2'
+  # @@protoc_insertion_point(class_scope:bosdyn.api.mission.GetRemoteMissionServiceInfoRequest)
+  })
+_sym_db.RegisterMessage(GetRemoteMissionServiceInfoRequest)
+
+GetRemoteMissionServiceInfoResponse = _reflection.GeneratedProtocolMessageType('GetRemoteMissionServiceInfoResponse', (_message.Message,), {
+  'DESCRIPTOR' : _GETREMOTEMISSIONSERVICEINFORESPONSE,
+  '__module__' : 'bosdyn.api.mission.remote_pb2'
+  # @@protoc_insertion_point(class_scope:bosdyn.api.mission.GetRemoteMissionServiceInfoResponse)
+  })
+_sym_db.RegisterMessage(GetRemoteMissionServiceInfoResponse)
+
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'B\013RemoteProto'
-  _ESTABLISHSESSIONREQUEST._serialized_start=136
-  _ESTABLISHSESSIONREQUEST._serialized_end=296
-  _ESTABLISHSESSIONRESPONSE._serialized_start=299
-  _ESTABLISHSESSIONRESPONSE._serialized_end=710
-  _ESTABLISHSESSIONRESPONSE_STATUS._serialized_start=613
-  _ESTABLISHSESSIONRESPONSE_STATUS._serialized_end=710
-  _TICKREQUEST._serialized_start=713
-  _TICKREQUEST._serialized_end=870
-  _TICKRESPONSE._serialized_start=873
-  _TICKRESPONSE._serialized_end=1340
-  _TICKRESPONSE_STATUS._serialized_start=1167
-  _TICKRESPONSE_STATUS._serialized_end=1340
-  _STOPREQUEST._serialized_start=1342
-  _STOPREQUEST._serialized_end=1418
-  _STOPRESPONSE._serialized_start=1421
-  _STOPRESPONSE._serialized_end=1612
-  _STOPRESPONSE_STATUS._serialized_start=1538
-  _STOPRESPONSE_STATUS._serialized_end=1612
-  _TEARDOWNSESSIONREQUEST._serialized_start=1614
-  _TEARDOWNSESSIONREQUEST._serialized_end=1701
-  _TEARDOWNSESSIONRESPONSE._serialized_start=1704
-  _TEARDOWNSESSIONRESPONSE._serialized_end=1917
-  _TEARDOWNSESSIONRESPONSE_STATUS._serialized_start=1538
-  _TEARDOWNSESSIONRESPONSE_STATUS._serialized_end=1612
+  _ESTABLISHSESSIONREQUEST.fields_by_name['inputs']._options = None
+  _ESTABLISHSESSIONREQUEST.fields_by_name['inputs']._serialized_options = b'\030\001'
+  _ESTABLISHSESSIONRESPONSE.fields_by_name['missing_inputs']._options = None
+  _ESTABLISHSESSIONRESPONSE.fields_by_name['missing_inputs']._serialized_options = b'\030\001'
+  _ESTABLISHSESSIONREQUEST._serialized_start=176
+  _ESTABLISHSESSIONREQUEST._serialized_end=346
+  _ESTABLISHSESSIONRESPONSE._serialized_start=349
+  _ESTABLISHSESSIONRESPONSE._serialized_end=764
+  _ESTABLISHSESSIONRESPONSE_STATUS._serialized_start=667
+  _ESTABLISHSESSIONRESPONSE_STATUS._serialized_end=764
+  _TICKREQUEST._serialized_start=767
+  _TICKREQUEST._serialized_end=983
+  _TICKRESPONSE._serialized_start=986
+  _TICKRESPONSE._serialized_end=1543
+  _TICKRESPONSE_STATUS._serialized_start=1338
+  _TICKRESPONSE_STATUS._serialized_end=1543
+  _STOPREQUEST._serialized_start=1545
+  _STOPREQUEST._serialized_end=1621
+  _STOPRESPONSE._serialized_start=1624
+  _STOPRESPONSE._serialized_end=1815
+  _STOPRESPONSE_STATUS._serialized_start=1741
+  _STOPRESPONSE_STATUS._serialized_end=1815
+  _TEARDOWNSESSIONREQUEST._serialized_start=1817
+  _TEARDOWNSESSIONREQUEST._serialized_end=1904
+  _TEARDOWNSESSIONRESPONSE._serialized_start=1907
+  _TEARDOWNSESSIONRESPONSE._serialized_end=2120
+  _TEARDOWNSESSIONRESPONSE_STATUS._serialized_start=1741
+  _TEARDOWNSESSIONRESPONSE_STATUS._serialized_end=1815
+  _GETREMOTEMISSIONSERVICEINFOREQUEST._serialized_start=2122
+  _GETREMOTEMISSIONSERVICEINFOREQUEST._serialized_end=2201
+  _GETREMOTEMISSIONSERVICEINFORESPONSE._serialized_start=2204
+  _GETREMOTEMISSIONSERVICEINFORESPONSE._serialized_end=2336
 # @@protoc_insertion_point(module_scope)
```

## bosdyn/api/mission/remote_service_pb2.py

```diff
@@ -11,19 +11,19 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from bosdyn.api.mission import remote_pb2 as bosdyn_dot_api_dot_mission_dot_remote__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'bosdyn/api/mission/remote_service.proto\x12\x12\x62osdyn.api.mission\x1a\x1f\x62osdyn/api/mission/remote.proto2\x8f\x03\n\x14RemoteMissionService\x12o\n\x10\x45stablishSession\x12+.bosdyn.api.mission.EstablishSessionRequest\x1a,.bosdyn.api.mission.EstablishSessionResponse\"\x00\x12K\n\x04Tick\x12\x1f.bosdyn.api.mission.TickRequest\x1a .bosdyn.api.mission.TickResponse\"\x00\x12K\n\x04Stop\x12\x1f.bosdyn.api.mission.StopRequest\x1a .bosdyn.api.mission.StopResponse\"\x00\x12l\n\x0fTeardownSession\x12*.bosdyn.api.mission.TeardownSessionRequest\x1a+.bosdyn.api.mission.TeardownSessionResponse\"\x00\x42\x14\x42\x12RemoteServiceProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'bosdyn/api/mission/remote_service.proto\x12\x12\x62osdyn.api.mission\x1a\x1f\x62osdyn/api/mission/remote.proto2\xa2\x04\n\x14RemoteMissionService\x12o\n\x10\x45stablishSession\x12+.bosdyn.api.mission.EstablishSessionRequest\x1a,.bosdyn.api.mission.EstablishSessionResponse\"\x00\x12K\n\x04Tick\x12\x1f.bosdyn.api.mission.TickRequest\x1a .bosdyn.api.mission.TickResponse\"\x00\x12K\n\x04Stop\x12\x1f.bosdyn.api.mission.StopRequest\x1a .bosdyn.api.mission.StopResponse\"\x00\x12l\n\x0fTeardownSession\x12*.bosdyn.api.mission.TeardownSessionRequest\x1a+.bosdyn.api.mission.TeardownSessionResponse\"\x00\x12\x90\x01\n\x1bGetRemoteMissionServiceInfo\x12\x36.bosdyn.api.mission.GetRemoteMissionServiceInfoRequest\x1a\x37.bosdyn.api.mission.GetRemoteMissionServiceInfoResponse\"\x00\x42\x14\x42\x12RemoteServiceProtob\x06proto3')
 
 
 
 _REMOTEMISSIONSERVICE = DESCRIPTOR.services_by_name['RemoteMissionService']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'B\022RemoteServiceProto'
   _REMOTEMISSIONSERVICE._serialized_start=97
-  _REMOTEMISSIONSERVICE._serialized_end=496
+  _REMOTEMISSIONSERVICE._serialized_end=643
 # @@protoc_insertion_point(module_scope)
```

## bosdyn/api/mission/remote_service_pb2_grpc.py

```diff
@@ -32,14 +32,19 @@
                 response_deserializer=bosdyn_dot_api_dot_mission_dot_remote__pb2.StopResponse.FromString,
                 )
         self.TeardownSession = channel.unary_unary(
                 '/bosdyn.api.mission.RemoteMissionService/TeardownSession',
                 request_serializer=bosdyn_dot_api_dot_mission_dot_remote__pb2.TeardownSessionRequest.SerializeToString,
                 response_deserializer=bosdyn_dot_api_dot_mission_dot_remote__pb2.TeardownSessionResponse.FromString,
                 )
+        self.GetRemoteMissionServiceInfo = channel.unary_unary(
+                '/bosdyn.api.mission.RemoteMissionService/GetRemoteMissionServiceInfo',
+                request_serializer=bosdyn_dot_api_dot_mission_dot_remote__pb2.GetRemoteMissionServiceInfoRequest.SerializeToString,
+                response_deserializer=bosdyn_dot_api_dot_mission_dot_remote__pb2.GetRemoteMissionServiceInfoResponse.FromString,
+                )
 
 
 class RemoteMissionServiceServicer(object):
     """Interface for mission callbacks.  Mission RemoteGrpc nodes will act as clients
     to this service type, calling out to this service when loaded, ticked, or unloaded.
     """
 
@@ -69,14 +74,22 @@
         """Tells the service it can forget any data associated with the given session ID.
         Should be called once for every EstablishSession call.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def GetRemoteMissionServiceInfo(self, request, context):
+        """Asks the service what to describe itself  Can be called by clients at mission
+        record time to parameterize a RemoteGrpc node.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_RemoteMissionServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'EstablishSession': grpc.unary_unary_rpc_method_handler(
                     servicer.EstablishSession,
                     request_deserializer=bosdyn_dot_api_dot_mission_dot_remote__pb2.EstablishSessionRequest.FromString,
                     response_serializer=bosdyn_dot_api_dot_mission_dot_remote__pb2.EstablishSessionResponse.SerializeToString,
@@ -92,14 +105,19 @@
                     response_serializer=bosdyn_dot_api_dot_mission_dot_remote__pb2.StopResponse.SerializeToString,
             ),
             'TeardownSession': grpc.unary_unary_rpc_method_handler(
                     servicer.TeardownSession,
                     request_deserializer=bosdyn_dot_api_dot_mission_dot_remote__pb2.TeardownSessionRequest.FromString,
                     response_serializer=bosdyn_dot_api_dot_mission_dot_remote__pb2.TeardownSessionResponse.SerializeToString,
             ),
+            'GetRemoteMissionServiceInfo': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetRemoteMissionServiceInfo,
+                    request_deserializer=bosdyn_dot_api_dot_mission_dot_remote__pb2.GetRemoteMissionServiceInfoRequest.FromString,
+                    response_serializer=bosdyn_dot_api_dot_mission_dot_remote__pb2.GetRemoteMissionServiceInfoResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'bosdyn.api.mission.RemoteMissionService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -171,7 +189,24 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/bosdyn.api.mission.RemoteMissionService/TeardownSession',
             bosdyn_dot_api_dot_mission_dot_remote__pb2.TeardownSessionRequest.SerializeToString,
             bosdyn_dot_api_dot_mission_dot_remote__pb2.TeardownSessionResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetRemoteMissionServiceInfo(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/bosdyn.api.mission.RemoteMissionService/GetRemoteMissionServiceInfo',
+            bosdyn_dot_api_dot_mission_dot_remote__pb2.GetRemoteMissionServiceInfoRequest.SerializeToString,
+            bosdyn_dot_api_dot_mission_dot_remote__pb2.GetRemoteMissionServiceInfoResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

## bosdyn/api/mission/util_pb2.py

```diff
@@ -12,15 +12,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import any_pb2 as google_dot_protobuf_dot_any__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1d\x62osdyn/api/mission/util.proto\x12\x12\x62osdyn.api.mission\x1a\x19google/protobuf/any.proto\"A\n\x08KeyValue\x12\x0b\n\x03key\x18\x01 \x01(\t\x12(\n\x05value\x18\x02 \x01(\x0b\x32\x19.bosdyn.api.mission.Value\"\xc6\x01\n\x05Value\x12\x35\n\x08\x63onstant\x18\x02 \x01(\x0b\x32!.bosdyn.api.mission.ConstantValueH\x00\x12>\n\x0bruntime_var\x18\x03 \x01(\x0b\x32\'.bosdyn.api.mission.VariableDeclarationH\x00\x12<\n\tparameter\x18\x04 \x01(\x0b\x32\'.bosdyn.api.mission.VariableDeclarationH\x00\x42\x08\n\x06source\"\xc9\x01\n\x13VariableDeclaration\x12\x0c\n\x04name\x18\x01 \x01(\t\x12:\n\x04type\x18\x02 \x01(\x0e\x32,.bosdyn.api.mission.VariableDeclaration.Type\"h\n\x04Type\x12\x10\n\x0cTYPE_UNKNOWN\x10\x00\x12\x0e\n\nTYPE_FLOAT\x10\x01\x12\x0f\n\x0bTYPE_STRING\x10\x02\x12\x0c\n\x08TYPE_INT\x10\x03\x12\r\n\tTYPE_BOOL\x10\x04\x12\x10\n\x0cTYPE_MESSAGE\x10\x05\"\x9d\x01\n\rConstantValue\x12\x15\n\x0b\x66loat_value\x18\x01 \x01(\x01H\x00\x12\x16\n\x0cstring_value\x18\x02 \x01(\tH\x00\x12\x13\n\tint_value\x18\x03 \x01(\x03H\x00\x12\x14\n\nbool_value\x18\x04 \x01(\x08H\x00\x12)\n\tmsg_value\x18\x05 \x01(\x0b\x32\x14.google.protobuf.AnyH\x00\x42\x07\n\x05value\"*\n\x08UserData\x12\n\n\x02id\x18\x01 \x01(\t\x12\x12\n\nbytestring\x18\x03 \x01(\x0c*j\n\x06Result\x12\x12\n\x0eRESULT_UNKNOWN\x10\x00\x12\x12\n\x0eRESULT_FAILURE\x10\x01\x12\x12\n\x0eRESULT_RUNNING\x10\x02\x12\x12\n\x0eRESULT_SUCCESS\x10\x03\x12\x10\n\x0cRESULT_ERROR\x10\x04\x42\x0b\x42\tUtilProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1d\x62osdyn/api/mission/util.proto\x12\x12\x62osdyn.api.mission\x1a\x19google/protobuf/any.proto\"A\n\x08KeyValue\x12\x0b\n\x03key\x18\x01 \x01(\t\x12(\n\x05value\x18\x02 \x01(\x0b\x32\x19.bosdyn.api.mission.Value\"\xc6\x01\n\x05Value\x12\x35\n\x08\x63onstant\x18\x02 \x01(\x0b\x32!.bosdyn.api.mission.ConstantValueH\x00\x12>\n\x0bruntime_var\x18\x03 \x01(\x0b\x32\'.bosdyn.api.mission.VariableDeclarationH\x00\x12<\n\tparameter\x18\x04 \x01(\x0b\x32\'.bosdyn.api.mission.VariableDeclarationH\x00\x42\x08\n\x06source\"\xc9\x01\n\x13VariableDeclaration\x12\x0c\n\x04name\x18\x01 \x01(\t\x12:\n\x04type\x18\x02 \x01(\x0e\x32,.bosdyn.api.mission.VariableDeclaration.Type\"h\n\x04Type\x12\x10\n\x0cTYPE_UNKNOWN\x10\x00\x12\x0e\n\nTYPE_FLOAT\x10\x01\x12\x0f\n\x0bTYPE_STRING\x10\x02\x12\x0c\n\x08TYPE_INT\x10\x03\x12\r\n\tTYPE_BOOL\x10\x04\x12\x10\n\x0cTYPE_MESSAGE\x10\x05\"\x9d\x01\n\rConstantValue\x12\x15\n\x0b\x66loat_value\x18\x01 \x01(\x01H\x00\x12\x16\n\x0cstring_value\x18\x02 \x01(\tH\x00\x12\x13\n\tint_value\x18\x03 \x01(\x03H\x00\x12\x14\n\nbool_value\x18\x04 \x01(\x08H\x00\x12)\n\tmsg_value\x18\x05 \x01(\x0b\x32\x14.google.protobuf.AnyH\x00\x42\x07\n\x05value\"_\n\x08UserData\x12\n\n\x02id\x18\x01 \x01(\t\x12\x12\n\nbytestring\x18\x03 \x01(\x0c\x12\x33\n\x15source_representation\x18\x04 \x01(\x0b\x32\x14.google.protobuf.Any*j\n\x06Result\x12\x12\n\x0eRESULT_UNKNOWN\x10\x00\x12\x12\n\x0eRESULT_FAILURE\x10\x01\x12\x12\n\x0eRESULT_RUNNING\x10\x02\x12\x12\n\x0eRESULT_SUCCESS\x10\x03\x12\x10\n\x0cRESULT_ERROR\x10\x04\x42\x0b\x42\tUtilProtob\x06proto3')
 
 _RESULT = DESCRIPTOR.enum_types_by_name['Result']
 Result = enum_type_wrapper.EnumTypeWrapper(_RESULT)
 RESULT_UNKNOWN = 0
 RESULT_FAILURE = 1
 RESULT_RUNNING = 2
 RESULT_SUCCESS = 3
@@ -68,22 +68,22 @@
   })
 _sym_db.RegisterMessage(UserData)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'B\tUtilProto'
-  _RESULT._serialized_start=756
-  _RESULT._serialized_end=862
+  _RESULT._serialized_start=809
+  _RESULT._serialized_end=915
   _KEYVALUE._serialized_start=80
   _KEYVALUE._serialized_end=145
   _VALUE._serialized_start=148
   _VALUE._serialized_end=346
   _VARIABLEDECLARATION._serialized_start=349
   _VARIABLEDECLARATION._serialized_end=550
   _VARIABLEDECLARATION_TYPE._serialized_start=446
   _VARIABLEDECLARATION_TYPE._serialized_end=550
   _CONSTANTVALUE._serialized_start=553
   _CONSTANTVALUE._serialized_end=710
   _USERDATA._serialized_start=712
-  _USERDATA._serialized_end=754
+  _USERDATA._serialized_end=807
 # @@protoc_insertion_point(module_scope)
```

## bosdyn/api/spot/__init__.py

```diff
@@ -0,0 +1,4 @@
+00000000: 5f5f 7061 7468 5f5f 203d 205f 5f69 6d70  __path__ = __imp
+00000010: 6f72 745f 5f28 2770 6b67 7574 696c 2729  ort__('pkgutil')
+00000020: 2e65 7874 656e 645f 7061 7468 285f 5f70  .extend_path(__p
+00000030: 6174 685f 5f2c 205f 5f6e 616d 655f 5f29  ath__, __name__)
```

## bosdyn/api/spot/door_pb2.py

```diff
@@ -14,15 +14,15 @@
 
 from bosdyn.api import basic_command_pb2 as bosdyn_dot_api_dot_basic__command__pb2
 from bosdyn.api import geometry_pb2 as bosdyn_dot_api_dot_geometry__pb2
 from bosdyn.api import header_pb2 as bosdyn_dot_api_dot_header__pb2
 from bosdyn.api import lease_pb2 as bosdyn_dot_api_dot_lease__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1a\x62osdyn/api/spot/door.proto\x12\x0f\x62osdyn.api.spot\x1a\x1e\x62osdyn/api/basic_command.proto\x1a\x19\x62osdyn/api/geometry.proto\x1a\x17\x62osdyn/api/header.proto\x1a\x16\x62osdyn/api/lease.proto\"\xa1\x01\n\x16OpenDoorCommandRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12 \n\x05lease\x18\x02 \x01(\x0b\x32\x11.bosdyn.api.Lease\x12:\n\x0c\x64oor_command\x18\x04 \x01(\x0b\x32$.bosdyn.api.spot.DoorCommand.Request\"\xb3\x02\n\x17OpenDoorCommandResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x34\n\x10lease_use_result\x18\x02 \x01(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12?\n\x06status\x18\x03 \x01(\x0e\x32/.bosdyn.api.spot.OpenDoorCommandResponse.Status\x12\x0f\n\x07message\x18\x04 \x01(\t\x12\x17\n\x0f\x64oor_command_id\x18\x05 \x01(\r\"K\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1e\n\x1aSTATUS_ROBOT_COMMAND_ERROR\x10\x02\"]\n\x17OpenDoorFeedbackRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x17\n\x0f\x64oor_command_id\x18\x02 \x01(\r\"\xbe\x01\n\x18OpenDoorFeedbackResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12=\n\x06status\x18\x64 \x01(\x0e\x32-.bosdyn.api.RobotCommandFeedbackStatus.Status\x12\x37\n\x08\x66\x65\x65\x64\x62\x61\x63k\x18\x02 \x01(\x0b\x32%.bosdyn.api.spot.DoorCommand.Feedback\"\x86\x0b\n\x0b\x44oorCommand\x1a\x90\x02\n\x10\x41utoGraspCommand\x12\x12\n\nframe_name\x18\x01 \x01(\t\x12\x33\n\x19search_ray_start_in_frame\x18\x02 \x01(\x0b\x32\x10.bosdyn.api.Vec3\x12\x31\n\x17search_ray_end_in_frame\x18\x03 \x01(\x0b\x32\x10.bosdyn.api.Vec3\x12:\n\nhinge_side\x18\x04 \x01(\x0e\x32&.bosdyn.api.spot.DoorCommand.HingeSide\x12\x44\n\x0fswing_direction\x18\x05 \x01(\x0e\x32+.bosdyn.api.spot.DoorCommand.SwingDirection\x1a\xd2\x01\n\x10WarmstartCommand\x12:\n\nhinge_side\x18\x01 \x01(\x0e\x32&.bosdyn.api.spot.DoorCommand.HingeSide\x12\x44\n\x0fswing_direction\x18\x02 \x01(\x0e\x32+.bosdyn.api.spot.DoorCommand.SwingDirection\x12<\n\x0bhandle_type\x18\x03 \x01(\x0e\x32\'.bosdyn.api.spot.DoorCommand.HandleType\x1a\x90\x01\n\x0f\x41utoPushCommand\x12\x12\n\nframe_name\x18\x01 \x01(\t\x12-\n\x13push_point_in_frame\x18\x02 \x01(\x0b\x32\x10.bosdyn.api.Vec3\x12:\n\nhinge_side\x18\x03 \x01(\x0e\x32&.bosdyn.api.spot.DoorCommand.HingeSide\x1a\xf8\x01\n\x07Request\x12K\n\x12\x61uto_grasp_command\x18\n \x01(\x0b\x32-.bosdyn.api.spot.DoorCommand.AutoGraspCommandH\x00\x12J\n\x11warmstart_command\x18\x0b \x01(\x0b\x32-.bosdyn.api.spot.DoorCommand.WarmstartCommandH\x00\x12I\n\x11\x61uto_push_command\x18\x0c \x01(\x0b\x32,.bosdyn.api.spot.DoorCommand.AutoPushCommandH\x00\x42\t\n\x07\x63ommand\x1a\x94\x01\n\x08\x46\x65\x65\x64\x62\x61\x63k\x12<\n\x06status\x18\x01 \x01(\x0e\x32,.bosdyn.api.spot.DoorCommand.Feedback.Status\"J\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x14\n\x10STATUS_COMPLETED\x10\x01\x12\x16\n\x12STATUS_IN_PROGRESS\x10\x02\"N\n\tHingeSide\x12\x16\n\x12HINGE_SIDE_UNKNOWN\x10\x00\x12\x13\n\x0fHINGE_SIDE_LEFT\x10\x01\x12\x14\n\x10HINGE_SIDE_RIGHT\x10\x02\"\xa8\x01\n\x0eSwingDirection\x12\x1b\n\x17SWING_DIRECTION_UNKNOWN\x10\x00\x12\x1f\n\x17SWING_DIRECTION_INSWING\x10\x01\x1a\x02\x08\x01\x12\x18\n\x14SWING_DIRECTION_PULL\x10\x01\x12 \n\x18SWING_DIRECTION_OUTSWING\x10\x02\x1a\x02\x08\x01\x12\x18\n\x14SWING_DIRECTION_PUSH\x10\x02\x1a\x02\x10\x01\"o\n\nHandleType\x12\x17\n\x13HANDLE_TYPE_UNKNOWN\x10\x00\x12\x15\n\x11HANDLE_TYPE_LEVER\x10\x01\x12\x14\n\x10HANDLE_TYPE_KNOB\x10\x02\x12\x1b\n\x17HANDLE_TYPE_FIXED_GRASP\x10\x03\x42\x12\x42\x10\x44oorCommandProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1a\x62osdyn/api/spot/door.proto\x12\x0f\x62osdyn.api.spot\x1a\x1e\x62osdyn/api/basic_command.proto\x1a\x19\x62osdyn/api/geometry.proto\x1a\x17\x62osdyn/api/header.proto\x1a\x16\x62osdyn/api/lease.proto\"\xa1\x01\n\x16OpenDoorCommandRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12 \n\x05lease\x18\x02 \x01(\x0b\x32\x11.bosdyn.api.Lease\x12:\n\x0c\x64oor_command\x18\x04 \x01(\x0b\x32$.bosdyn.api.spot.DoorCommand.Request\"\xd7\x02\n\x17OpenDoorCommandResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x34\n\x10lease_use_result\x18\x02 \x01(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12?\n\x06status\x18\x03 \x01(\x0e\x32/.bosdyn.api.spot.OpenDoorCommandResponse.Status\x12\x0f\n\x07message\x18\x04 \x01(\t\x12\x17\n\x0f\x64oor_command_id\x18\x05 \x01(\r\"o\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1e\n\x1aSTATUS_ROBOT_COMMAND_ERROR\x10\x02\x12\"\n\x1eSTATUS_DOOR_PLANE_NOT_DETECTED\x10\x03\"]\n\x17OpenDoorFeedbackRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x17\n\x0f\x64oor_command_id\x18\x02 \x01(\r\"\xf4\x01\n\x18OpenDoorFeedbackResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12=\n\x06status\x18\x64 \x01(\x0e\x32-.bosdyn.api.RobotCommandFeedbackStatus.Status\x12\x34\n\x10lease_use_result\x18\x03 \x01(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12\x37\n\x08\x66\x65\x65\x64\x62\x61\x63k\x18\x02 \x01(\x0b\x32%.bosdyn.api.spot.DoorCommand.Feedback\"\xd4\x0b\n\x0b\x44oorCommand\x1a\x90\x02\n\x10\x41utoGraspCommand\x12\x12\n\nframe_name\x18\x01 \x01(\t\x12\x33\n\x19search_ray_start_in_frame\x18\x02 \x01(\x0b\x32\x10.bosdyn.api.Vec3\x12\x31\n\x17search_ray_end_in_frame\x18\x03 \x01(\x0b\x32\x10.bosdyn.api.Vec3\x12:\n\nhinge_side\x18\x04 \x01(\x0e\x32&.bosdyn.api.spot.DoorCommand.HingeSide\x12\x44\n\x0fswing_direction\x18\x05 \x01(\x0e\x32+.bosdyn.api.spot.DoorCommand.SwingDirection\x1a\xd2\x01\n\x10WarmstartCommand\x12:\n\nhinge_side\x18\x01 \x01(\x0e\x32&.bosdyn.api.spot.DoorCommand.HingeSide\x12\x44\n\x0fswing_direction\x18\x02 \x01(\x0e\x32+.bosdyn.api.spot.DoorCommand.SwingDirection\x12<\n\x0bhandle_type\x18\x03 \x01(\x0e\x32\'.bosdyn.api.spot.DoorCommand.HandleType\x1a\x90\x01\n\x0f\x41utoPushCommand\x12\x12\n\nframe_name\x18\x01 \x01(\t\x12-\n\x13push_point_in_frame\x18\x02 \x01(\x0b\x32\x10.bosdyn.api.Vec3\x12:\n\nhinge_side\x18\x03 \x01(\x0e\x32&.bosdyn.api.spot.DoorCommand.HingeSide\x1a\xf8\x01\n\x07Request\x12K\n\x12\x61uto_grasp_command\x18\n \x01(\x0b\x32-.bosdyn.api.spot.DoorCommand.AutoGraspCommandH\x00\x12J\n\x11warmstart_command\x18\x0b \x01(\x0b\x32-.bosdyn.api.spot.DoorCommand.WarmstartCommandH\x00\x12I\n\x11\x61uto_push_command\x18\x0c \x01(\x0b\x32,.bosdyn.api.spot.DoorCommand.AutoPushCommandH\x00\x42\t\n\x07\x63ommand\x1a\xe2\x01\n\x08\x46\x65\x65\x64\x62\x61\x63k\x12<\n\x06status\x18\x01 \x01(\x0e\x32,.bosdyn.api.spot.DoorCommand.Feedback.Status\x12\x1f\n\x17\x64istance_past_threshold\x18\x02 \x01(\x01\"w\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x14\n\x10STATUS_COMPLETED\x10\x01\x12\x16\n\x12STATUS_IN_PROGRESS\x10\x02\x12\x12\n\x0eSTATUS_STALLED\x10\x03\x12\x17\n\x13STATUS_NOT_DETECTED\x10\x04\"N\n\tHingeSide\x12\x16\n\x12HINGE_SIDE_UNKNOWN\x10\x00\x12\x13\n\x0fHINGE_SIDE_LEFT\x10\x01\x12\x14\n\x10HINGE_SIDE_RIGHT\x10\x02\"\xa8\x01\n\x0eSwingDirection\x12\x1b\n\x17SWING_DIRECTION_UNKNOWN\x10\x00\x12\x1f\n\x17SWING_DIRECTION_INSWING\x10\x01\x1a\x02\x08\x01\x12\x18\n\x14SWING_DIRECTION_PULL\x10\x01\x12 \n\x18SWING_DIRECTION_OUTSWING\x10\x02\x1a\x02\x08\x01\x12\x18\n\x14SWING_DIRECTION_PUSH\x10\x02\x1a\x02\x10\x01\"o\n\nHandleType\x12\x17\n\x13HANDLE_TYPE_UNKNOWN\x10\x00\x12\x15\n\x11HANDLE_TYPE_LEVER\x10\x01\x12\x14\n\x10HANDLE_TYPE_KNOB\x10\x02\x12\x1b\n\x17HANDLE_TYPE_FIXED_GRASP\x10\x03\x42\x12\x42\x10\x44oorCommandProtob\x06proto3')
 
 
 
 _OPENDOORCOMMANDREQUEST = DESCRIPTOR.message_types_by_name['OpenDoorCommandRequest']
 _OPENDOORCOMMANDRESPONSE = DESCRIPTOR.message_types_by_name['OpenDoorCommandResponse']
 _OPENDOORFEEDBACKREQUEST = DESCRIPTOR.message_types_by_name['OpenDoorFeedbackRequest']
 _OPENDOORFEEDBACKRESPONSE = DESCRIPTOR.message_types_by_name['OpenDoorFeedbackResponse']
@@ -121,35 +121,35 @@
   _DOORCOMMAND_SWINGDIRECTION.values_by_name["SWING_DIRECTION_INSWING"]._options = None
   _DOORCOMMAND_SWINGDIRECTION.values_by_name["SWING_DIRECTION_INSWING"]._serialized_options = b'\010\001'
   _DOORCOMMAND_SWINGDIRECTION.values_by_name["SWING_DIRECTION_OUTSWING"]._options = None
   _DOORCOMMAND_SWINGDIRECTION.values_by_name["SWING_DIRECTION_OUTSWING"]._serialized_options = b'\010\001'
   _OPENDOORCOMMANDREQUEST._serialized_start=156
   _OPENDOORCOMMANDREQUEST._serialized_end=317
   _OPENDOORCOMMANDRESPONSE._serialized_start=320
-  _OPENDOORCOMMANDRESPONSE._serialized_end=627
+  _OPENDOORCOMMANDRESPONSE._serialized_end=663
   _OPENDOORCOMMANDRESPONSE_STATUS._serialized_start=552
-  _OPENDOORCOMMANDRESPONSE_STATUS._serialized_end=627
-  _OPENDOORFEEDBACKREQUEST._serialized_start=629
-  _OPENDOORFEEDBACKREQUEST._serialized_end=722
-  _OPENDOORFEEDBACKRESPONSE._serialized_start=725
-  _OPENDOORFEEDBACKRESPONSE._serialized_end=915
-  _DOORCOMMAND._serialized_start=918
-  _DOORCOMMAND._serialized_end=2332
-  _DOORCOMMAND_AUTOGRASPCOMMAND._serialized_start=934
-  _DOORCOMMAND_AUTOGRASPCOMMAND._serialized_end=1206
-  _DOORCOMMAND_WARMSTARTCOMMAND._serialized_start=1209
-  _DOORCOMMAND_WARMSTARTCOMMAND._serialized_end=1419
-  _DOORCOMMAND_AUTOPUSHCOMMAND._serialized_start=1422
-  _DOORCOMMAND_AUTOPUSHCOMMAND._serialized_end=1566
-  _DOORCOMMAND_REQUEST._serialized_start=1569
-  _DOORCOMMAND_REQUEST._serialized_end=1817
-  _DOORCOMMAND_FEEDBACK._serialized_start=1820
-  _DOORCOMMAND_FEEDBACK._serialized_end=1968
-  _DOORCOMMAND_FEEDBACK_STATUS._serialized_start=1894
-  _DOORCOMMAND_FEEDBACK_STATUS._serialized_end=1968
-  _DOORCOMMAND_HINGESIDE._serialized_start=1970
-  _DOORCOMMAND_HINGESIDE._serialized_end=2048
-  _DOORCOMMAND_SWINGDIRECTION._serialized_start=2051
-  _DOORCOMMAND_SWINGDIRECTION._serialized_end=2219
-  _DOORCOMMAND_HANDLETYPE._serialized_start=2221
-  _DOORCOMMAND_HANDLETYPE._serialized_end=2332
+  _OPENDOORCOMMANDRESPONSE_STATUS._serialized_end=663
+  _OPENDOORFEEDBACKREQUEST._serialized_start=665
+  _OPENDOORFEEDBACKREQUEST._serialized_end=758
+  _OPENDOORFEEDBACKRESPONSE._serialized_start=761
+  _OPENDOORFEEDBACKRESPONSE._serialized_end=1005
+  _DOORCOMMAND._serialized_start=1008
+  _DOORCOMMAND._serialized_end=2500
+  _DOORCOMMAND_AUTOGRASPCOMMAND._serialized_start=1024
+  _DOORCOMMAND_AUTOGRASPCOMMAND._serialized_end=1296
+  _DOORCOMMAND_WARMSTARTCOMMAND._serialized_start=1299
+  _DOORCOMMAND_WARMSTARTCOMMAND._serialized_end=1509
+  _DOORCOMMAND_AUTOPUSHCOMMAND._serialized_start=1512
+  _DOORCOMMAND_AUTOPUSHCOMMAND._serialized_end=1656
+  _DOORCOMMAND_REQUEST._serialized_start=1659
+  _DOORCOMMAND_REQUEST._serialized_end=1907
+  _DOORCOMMAND_FEEDBACK._serialized_start=1910
+  _DOORCOMMAND_FEEDBACK._serialized_end=2136
+  _DOORCOMMAND_FEEDBACK_STATUS._serialized_start=2017
+  _DOORCOMMAND_FEEDBACK_STATUS._serialized_end=2136
+  _DOORCOMMAND_HINGESIDE._serialized_start=2138
+  _DOORCOMMAND_HINGESIDE._serialized_end=2216
+  _DOORCOMMAND_SWINGDIRECTION._serialized_start=2219
+  _DOORCOMMAND_SWINGDIRECTION._serialized_end=2387
+  _DOORCOMMAND_HANDLETYPE._serialized_start=2389
+  _DOORCOMMAND_HANDLETYPE._serialized_end=2500
 # @@protoc_insertion_point(module_scope)
```

## bosdyn/api/spot/robot_command_pb2.py

```diff
@@ -14,15 +14,15 @@
 
 
 from bosdyn.api import geometry_pb2 as bosdyn_dot_api_dot_geometry__pb2
 from bosdyn.api import trajectory_pb2 as bosdyn_dot_api_dot_trajectory__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n#bosdyn/api/spot/robot_command.proto\x12\x0f\x62osdyn.api.spot\x1a\x19\x62osdyn/api/geometry.proto\x1a\x1b\x62osdyn/api/trajectory.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\xa5\x06\n\x0eMobilityParams\x12/\n\tvel_limit\x18\x01 \x01(\x0b\x32\x1c.bosdyn.api.SE2VelocityLimit\x12\x38\n\x0c\x62ody_control\x18\x02 \x01(\x0b\x32\".bosdyn.api.spot.BodyControlParams\x12\x38\n\x0flocomotion_hint\x18\x03 \x01(\x0e\x32\x1f.bosdyn.api.spot.LocomotionHint\x12\x16\n\nstair_hint\x18\x04 \x01(\x08\x42\x02\x18\x01\x12?\n\x0bstairs_mode\x18\x11 \x01(\x0e\x32*.bosdyn.api.spot.MobilityParams.StairsMode\x12!\n\x19\x61llow_degraded_perception\x18\x05 \x01(\x08\x12\x38\n\x0fobstacle_params\x18\x06 \x01(\x0b\x32\x1f.bosdyn.api.spot.ObstacleParams\x12\x32\n\x0cswing_height\x18\x07 \x01(\x0e\x32\x1c.bosdyn.api.spot.SwingHeight\x12\x36\n\x0eterrain_params\x18\x08 \x01(\x0b\x32\x1e.bosdyn.api.spot.TerrainParams\x12\x1e\n\x16\x64isallow_stair_tracker\x18\t \x01(\x08\x12(\n disable_stair_error_auto_descent\x18\x10 \x01(\x08\x12G\n\x15\x65xternal_force_params\x18\n \x01(\x0b\x32(.bosdyn.api.spot.BodyExternalForceParams\x12*\n\"disallow_non_stairs_pitch_limiting\x18\x0b \x01(\x08\x12\'\n\x1f\x64isable_nearmap_cliff_avoidance\x18\x0c \x01(\x08\"d\n\nStairsMode\x12\x17\n\x13STAIRS_MODE_UNKNOWN\x10\x00\x12\x13\n\x0fSTAIRS_MODE_OFF\x10\x01\x12\x12\n\x0eSTAIRS_MODE_ON\x10\x02\x12\x14\n\x10STAIRS_MODE_AUTO\x10\x03\"\xdb\x03\n\x11\x42odyControlParams\x12=\n\x18\x62\x61se_offset_rt_footprint\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.SE3TrajectoryH\x00\x12\x64\n\x1c\x62ody_assist_for_manipulation\x18\x03 \x01(\x0b\x32<.bosdyn.api.spot.BodyControlParams.BodyAssistForManipulationH\x00\x12L\n\x10rotation_setting\x18\x02 \x01(\x0e\x32\x32.bosdyn.api.spot.BodyControlParams.RotationSetting\x1a]\n\x19\x42odyAssistForManipulation\x12\x1e\n\x16\x65nable_body_yaw_assist\x18\x01 \x01(\x08\x12 \n\x18\x65nable_hip_height_assist\x18\x02 \x01(\x08\"k\n\x0fRotationSetting\x12\x1c\n\x18ROTATION_SETTING_UNKNOWN\x10\x00\x12\x1b\n\x17ROTATION_SETTING_OFFSET\x10\x01\x12\x1d\n\x19ROTATION_SETTING_ABSOLUTE\x10\x02\x42\x07\n\x05param\"\xa3\x02\n\x0eObstacleParams\x12.\n&disable_vision_foot_obstacle_avoidance\x18\x01 \x01(\x08\x12\x30\n(disable_vision_foot_constraint_avoidance\x18\x02 \x01(\x08\x12.\n&disable_vision_body_obstacle_avoidance\x18\x03 \x01(\x08\x12\"\n\x1aobstacle_avoidance_padding\x18\x04 \x01(\x01\x12\x30\n(disable_vision_foot_obstacle_body_assist\x18\x05 \x01(\x08\x12)\n!disable_vision_negative_obstacles\x18\x06 \x01(\x08\"\xca\x02\n\rTerrainParams\x12\x34\n\x0eground_mu_hint\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x1f\n\x13\x65nable_grated_floor\x18\x03 \x01(\x08\x42\x02\x18\x01\x12O\n\x14grated_surfaces_mode\x18\x04 \x01(\x0e\x32\x31.bosdyn.api.spot.TerrainParams.GratedSurfacesMode\"\x90\x01\n\x12GratedSurfacesMode\x12 \n\x1cGRATED_SURFACES_MODE_UNKNOWN\x10\x00\x12\x1c\n\x18GRATED_SURFACES_MODE_OFF\x10\x01\x12\x1b\n\x17GRATED_SURFACES_MODE_ON\x10\x02\x12\x1d\n\x19GRATED_SURFACES_MODE_AUTO\x10\x03\"\xbe\x02\n\x17\x42odyExternalForceParams\x12\x61\n\x18\x65xternal_force_indicator\x18\x01 \x01(\x0e\x32?.bosdyn.api.spot.BodyExternalForceParams.ExternalForceIndicator\x12\x12\n\nframe_name\x18\x04 \x01(\t\x12\x31\n\x17\x65xternal_force_override\x18\x03 \x01(\x0b\x32\x10.bosdyn.api.Vec3\"s\n\x16\x45xternalForceIndicator\x12\x17\n\x13\x45XTERNAL_FORCE_NONE\x10\x00\x12\x1f\n\x1b\x45XTERNAL_FORCE_USE_ESTIMATE\x10\x01\x12\x1f\n\x1b\x45XTERNAL_FORCE_USE_OVERRIDE\x10\x02J\x04\x08\x02\x10\x03*\xff\x01\n\x0eLocomotionHint\x12\x10\n\x0cHINT_UNKNOWN\x10\x00\x12\r\n\tHINT_AUTO\x10\x01\x12\r\n\tHINT_TROT\x10\x02\x12\x1a\n\x16HINT_SPEED_SELECT_TROT\x10\x03\x12\x0e\n\nHINT_CRAWL\x10\x04\x12\x1b\n\x17HINT_SPEED_SELECT_CRAWL\x10\n\x12\x0e\n\nHINT_AMBLE\x10\x05\x12\x1b\n\x17HINT_SPEED_SELECT_AMBLE\x10\x06\x12\x0c\n\x08HINT_JOG\x10\x07\x12\x0c\n\x08HINT_HOP\x10\x08\x12\x12\n\x0eHINT_AUTO_TROT\x10\x03\x12\x13\n\x0fHINT_AUTO_AMBLE\x10\x06\x1a\x02\x10\x01*m\n\x0bSwingHeight\x12\x18\n\x14SWING_HEIGHT_UNKNOWN\x10\x00\x12\x14\n\x10SWING_HEIGHT_LOW\x10\x01\x12\x17\n\x13SWING_HEIGHT_MEDIUM\x10\x02\x12\x15\n\x11SWING_HEIGHT_HIGH\x10\x03\x42\x13\x42\x11RobotCommandProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n#bosdyn/api/spot/robot_command.proto\x12\x0f\x62osdyn.api.spot\x1a\x19\x62osdyn/api/geometry.proto\x1a\x1b\x62osdyn/api/trajectory.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\xa5\x06\n\x0eMobilityParams\x12/\n\tvel_limit\x18\x01 \x01(\x0b\x32\x1c.bosdyn.api.SE2VelocityLimit\x12\x38\n\x0c\x62ody_control\x18\x02 \x01(\x0b\x32\".bosdyn.api.spot.BodyControlParams\x12\x38\n\x0flocomotion_hint\x18\x03 \x01(\x0e\x32\x1f.bosdyn.api.spot.LocomotionHint\x12\x16\n\nstair_hint\x18\x04 \x01(\x08\x42\x02\x18\x01\x12?\n\x0bstairs_mode\x18\x11 \x01(\x0e\x32*.bosdyn.api.spot.MobilityParams.StairsMode\x12!\n\x19\x61llow_degraded_perception\x18\x05 \x01(\x08\x12\x38\n\x0fobstacle_params\x18\x06 \x01(\x0b\x32\x1f.bosdyn.api.spot.ObstacleParams\x12\x32\n\x0cswing_height\x18\x07 \x01(\x0e\x32\x1c.bosdyn.api.spot.SwingHeight\x12\x36\n\x0eterrain_params\x18\x08 \x01(\x0b\x32\x1e.bosdyn.api.spot.TerrainParams\x12\x1e\n\x16\x64isallow_stair_tracker\x18\t \x01(\x08\x12(\n disable_stair_error_auto_descent\x18\x10 \x01(\x08\x12G\n\x15\x65xternal_force_params\x18\n \x01(\x0b\x32(.bosdyn.api.spot.BodyExternalForceParams\x12*\n\"disallow_non_stairs_pitch_limiting\x18\x0b \x01(\x08\x12\'\n\x1f\x64isable_nearmap_cliff_avoidance\x18\x0c \x01(\x08\"d\n\nStairsMode\x12\x17\n\x13STAIRS_MODE_UNKNOWN\x10\x00\x12\x13\n\x0fSTAIRS_MODE_OFF\x10\x01\x12\x12\n\x0eSTAIRS_MODE_ON\x10\x02\x12\x14\n\x10STAIRS_MODE_AUTO\x10\x03\"\xfa\x04\n\x11\x42odyControlParams\x12=\n\x18\x62\x61se_offset_rt_footprint\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.SE3TrajectoryH\x00\x12\x64\n\x1c\x62ody_assist_for_manipulation\x18\x03 \x01(\x0b\x32<.bosdyn.api.spot.BodyControlParams.BodyAssistForManipulationH\x00\x12@\n\tbody_pose\x18\x04 \x01(\x0b\x32+.bosdyn.api.spot.BodyControlParams.BodyPoseH\x00\x12L\n\x10rotation_setting\x18\x02 \x01(\x0e\x32\x32.bosdyn.api.spot.BodyControlParams.RotationSetting\x1a]\n\x19\x42odyAssistForManipulation\x12\x1e\n\x16\x65nable_body_yaw_assist\x18\x01 \x01(\x08\x12 \n\x18\x65nable_hip_height_assist\x18\x02 \x01(\x08\x1a[\n\x08\x42odyPose\x12\x17\n\x0froot_frame_name\x18\x01 \x01(\t\x12\x36\n\x13\x62\x61se_offset_rt_root\x18\x02 \x01(\x0b\x32\x19.bosdyn.api.SE3Trajectory\"k\n\x0fRotationSetting\x12\x1c\n\x18ROTATION_SETTING_UNKNOWN\x10\x00\x12\x1b\n\x17ROTATION_SETTING_OFFSET\x10\x01\x12\x1d\n\x19ROTATION_SETTING_ABSOLUTE\x10\x02\x42\x07\n\x05param\"\xa3\x02\n\x0eObstacleParams\x12.\n&disable_vision_foot_obstacle_avoidance\x18\x01 \x01(\x08\x12\x30\n(disable_vision_foot_constraint_avoidance\x18\x02 \x01(\x08\x12.\n&disable_vision_body_obstacle_avoidance\x18\x03 \x01(\x08\x12\"\n\x1aobstacle_avoidance_padding\x18\x04 \x01(\x01\x12\x30\n(disable_vision_foot_obstacle_body_assist\x18\x05 \x01(\x08\x12)\n!disable_vision_negative_obstacles\x18\x06 \x01(\x08\"\xca\x02\n\rTerrainParams\x12\x34\n\x0eground_mu_hint\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x1f\n\x13\x65nable_grated_floor\x18\x03 \x01(\x08\x42\x02\x18\x01\x12O\n\x14grated_surfaces_mode\x18\x04 \x01(\x0e\x32\x31.bosdyn.api.spot.TerrainParams.GratedSurfacesMode\"\x90\x01\n\x12GratedSurfacesMode\x12 \n\x1cGRATED_SURFACES_MODE_UNKNOWN\x10\x00\x12\x1c\n\x18GRATED_SURFACES_MODE_OFF\x10\x01\x12\x1b\n\x17GRATED_SURFACES_MODE_ON\x10\x02\x12\x1d\n\x19GRATED_SURFACES_MODE_AUTO\x10\x03\"\xbe\x02\n\x17\x42odyExternalForceParams\x12\x61\n\x18\x65xternal_force_indicator\x18\x01 \x01(\x0e\x32?.bosdyn.api.spot.BodyExternalForceParams.ExternalForceIndicator\x12\x12\n\nframe_name\x18\x04 \x01(\t\x12\x31\n\x17\x65xternal_force_override\x18\x03 \x01(\x0b\x32\x10.bosdyn.api.Vec3\"s\n\x16\x45xternalForceIndicator\x12\x17\n\x13\x45XTERNAL_FORCE_NONE\x10\x00\x12\x1f\n\x1b\x45XTERNAL_FORCE_USE_ESTIMATE\x10\x01\x12\x1f\n\x1b\x45XTERNAL_FORCE_USE_OVERRIDE\x10\x02J\x04\x08\x02\x10\x03*\xff\x01\n\x0eLocomotionHint\x12\x10\n\x0cHINT_UNKNOWN\x10\x00\x12\r\n\tHINT_AUTO\x10\x01\x12\r\n\tHINT_TROT\x10\x02\x12\x1a\n\x16HINT_SPEED_SELECT_TROT\x10\x03\x12\x0e\n\nHINT_CRAWL\x10\x04\x12\x1b\n\x17HINT_SPEED_SELECT_CRAWL\x10\n\x12\x0e\n\nHINT_AMBLE\x10\x05\x12\x1b\n\x17HINT_SPEED_SELECT_AMBLE\x10\x06\x12\x0c\n\x08HINT_JOG\x10\x07\x12\x0c\n\x08HINT_HOP\x10\x08\x12\x12\n\x0eHINT_AUTO_TROT\x10\x03\x12\x13\n\x0fHINT_AUTO_AMBLE\x10\x06\x1a\x02\x10\x01*m\n\x0bSwingHeight\x12\x18\n\x14SWING_HEIGHT_UNKNOWN\x10\x00\x12\x14\n\x10SWING_HEIGHT_LOW\x10\x01\x12\x17\n\x13SWING_HEIGHT_MEDIUM\x10\x02\x12\x15\n\x11SWING_HEIGHT_HIGH\x10\x03\x42\x13\x42\x11RobotCommandProtob\x06proto3')
 
 _LOCOMOTIONHINT = DESCRIPTOR.enum_types_by_name['LocomotionHint']
 LocomotionHint = enum_type_wrapper.EnumTypeWrapper(_LOCOMOTIONHINT)
 _SWINGHEIGHT = DESCRIPTOR.enum_types_by_name['SwingHeight']
 SwingHeight = enum_type_wrapper.EnumTypeWrapper(_SWINGHEIGHT)
 HINT_UNKNOWN = 0
 HINT_AUTO = 1
@@ -41,14 +41,15 @@
 SWING_HEIGHT_MEDIUM = 2
 SWING_HEIGHT_HIGH = 3
 
 
 _MOBILITYPARAMS = DESCRIPTOR.message_types_by_name['MobilityParams']
 _BODYCONTROLPARAMS = DESCRIPTOR.message_types_by_name['BodyControlParams']
 _BODYCONTROLPARAMS_BODYASSISTFORMANIPULATION = _BODYCONTROLPARAMS.nested_types_by_name['BodyAssistForManipulation']
+_BODYCONTROLPARAMS_BODYPOSE = _BODYCONTROLPARAMS.nested_types_by_name['BodyPose']
 _OBSTACLEPARAMS = DESCRIPTOR.message_types_by_name['ObstacleParams']
 _TERRAINPARAMS = DESCRIPTOR.message_types_by_name['TerrainParams']
 _BODYEXTERNALFORCEPARAMS = DESCRIPTOR.message_types_by_name['BodyExternalForceParams']
 _MOBILITYPARAMS_STAIRSMODE = _MOBILITYPARAMS.enum_types_by_name['StairsMode']
 _BODYCONTROLPARAMS_ROTATIONSETTING = _BODYCONTROLPARAMS.enum_types_by_name['RotationSetting']
 _TERRAINPARAMS_GRATEDSURFACESMODE = _TERRAINPARAMS.enum_types_by_name['GratedSurfacesMode']
 _BODYEXTERNALFORCEPARAMS_EXTERNALFORCEINDICATOR = _BODYEXTERNALFORCEPARAMS.enum_types_by_name['ExternalForceIndicator']
@@ -63,20 +64,28 @@
 
   'BodyAssistForManipulation' : _reflection.GeneratedProtocolMessageType('BodyAssistForManipulation', (_message.Message,), {
     'DESCRIPTOR' : _BODYCONTROLPARAMS_BODYASSISTFORMANIPULATION,
     '__module__' : 'bosdyn.api.spot.robot_command_pb2'
     # @@protoc_insertion_point(class_scope:bosdyn.api.spot.BodyControlParams.BodyAssistForManipulation)
     })
   ,
+
+  'BodyPose' : _reflection.GeneratedProtocolMessageType('BodyPose', (_message.Message,), {
+    'DESCRIPTOR' : _BODYCONTROLPARAMS_BODYPOSE,
+    '__module__' : 'bosdyn.api.spot.robot_command_pb2'
+    # @@protoc_insertion_point(class_scope:bosdyn.api.spot.BodyControlParams.BodyPose)
+    })
+  ,
   'DESCRIPTOR' : _BODYCONTROLPARAMS,
   '__module__' : 'bosdyn.api.spot.robot_command_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.spot.BodyControlParams)
   })
 _sym_db.RegisterMessage(BodyControlParams)
 _sym_db.RegisterMessage(BodyControlParams.BodyAssistForManipulation)
+_sym_db.RegisterMessage(BodyControlParams.BodyPose)
 
 ObstacleParams = _reflection.GeneratedProtocolMessageType('ObstacleParams', (_message.Message,), {
   'DESCRIPTOR' : _OBSTACLEPARAMS,
   '__module__' : 'bosdyn.api.spot.robot_command_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.spot.ObstacleParams)
   })
 _sym_db.RegisterMessage(ObstacleParams)
@@ -101,32 +110,34 @@
   DESCRIPTOR._serialized_options = b'B\021RobotCommandProto'
   _LOCOMOTIONHINT._options = None
   _LOCOMOTIONHINT._serialized_options = b'\020\001'
   _MOBILITYPARAMS.fields_by_name['stair_hint']._options = None
   _MOBILITYPARAMS.fields_by_name['stair_hint']._serialized_options = b'\030\001'
   _TERRAINPARAMS.fields_by_name['enable_grated_floor']._options = None
   _TERRAINPARAMS.fields_by_name['enable_grated_floor']._serialized_options = b'\030\001'
-  _LOCOMOTIONHINT._serialized_start=2379
-  _LOCOMOTIONHINT._serialized_end=2634
-  _SWINGHEIGHT._serialized_start=2636
-  _SWINGHEIGHT._serialized_end=2745
+  _LOCOMOTIONHINT._serialized_start=2538
+  _LOCOMOTIONHINT._serialized_end=2793
+  _SWINGHEIGHT._serialized_start=2795
+  _SWINGHEIGHT._serialized_end=2904
   _MOBILITYPARAMS._serialized_start=145
   _MOBILITYPARAMS._serialized_end=950
   _MOBILITYPARAMS_STAIRSMODE._serialized_start=850
   _MOBILITYPARAMS_STAIRSMODE._serialized_end=950
   _BODYCONTROLPARAMS._serialized_start=953
-  _BODYCONTROLPARAMS._serialized_end=1428
-  _BODYCONTROLPARAMS_BODYASSISTFORMANIPULATION._serialized_start=1217
-  _BODYCONTROLPARAMS_BODYASSISTFORMANIPULATION._serialized_end=1310
-  _BODYCONTROLPARAMS_ROTATIONSETTING._serialized_start=1312
-  _BODYCONTROLPARAMS_ROTATIONSETTING._serialized_end=1419
-  _OBSTACLEPARAMS._serialized_start=1431
-  _OBSTACLEPARAMS._serialized_end=1722
-  _TERRAINPARAMS._serialized_start=1725
-  _TERRAINPARAMS._serialized_end=2055
-  _TERRAINPARAMS_GRATEDSURFACESMODE._serialized_start=1911
-  _TERRAINPARAMS_GRATEDSURFACESMODE._serialized_end=2055
-  _BODYEXTERNALFORCEPARAMS._serialized_start=2058
-  _BODYEXTERNALFORCEPARAMS._serialized_end=2376
-  _BODYEXTERNALFORCEPARAMS_EXTERNALFORCEINDICATOR._serialized_start=2255
-  _BODYEXTERNALFORCEPARAMS_EXTERNALFORCEINDICATOR._serialized_end=2370
+  _BODYCONTROLPARAMS._serialized_end=1587
+  _BODYCONTROLPARAMS_BODYASSISTFORMANIPULATION._serialized_start=1283
+  _BODYCONTROLPARAMS_BODYASSISTFORMANIPULATION._serialized_end=1376
+  _BODYCONTROLPARAMS_BODYPOSE._serialized_start=1378
+  _BODYCONTROLPARAMS_BODYPOSE._serialized_end=1469
+  _BODYCONTROLPARAMS_ROTATIONSETTING._serialized_start=1471
+  _BODYCONTROLPARAMS_ROTATIONSETTING._serialized_end=1578
+  _OBSTACLEPARAMS._serialized_start=1590
+  _OBSTACLEPARAMS._serialized_end=1881
+  _TERRAINPARAMS._serialized_start=1884
+  _TERRAINPARAMS._serialized_end=2214
+  _TERRAINPARAMS_GRATEDSURFACESMODE._serialized_start=2070
+  _TERRAINPARAMS_GRATEDSURFACESMODE._serialized_end=2214
+  _BODYEXTERNALFORCEPARAMS._serialized_start=2217
+  _BODYEXTERNALFORCEPARAMS._serialized_end=2535
+  _BODYEXTERNALFORCEPARAMS_EXTERNALFORCEINDICATOR._serialized_start=2414
+  _BODYEXTERNALFORCEPARAMS_EXTERNALFORCEINDICATOR._serialized_end=2529
 # @@protoc_insertion_point(module_scope)
```

## bosdyn/api/spot_cam/__init__.py

```diff
@@ -0,0 +1,4 @@
+00000000: 5f5f 7061 7468 5f5f 203d 205f 5f69 6d70  __path__ = __imp
+00000010: 6f72 745f 5f28 2770 6b67 7574 696c 2729  ort__('pkgutil')
+00000020: 2e65 7874 656e 645f 7061 7468 285f 5f70  .extend_path(__p
+00000030: 6174 685f 5f2c 205f 5f6e 616d 655f 5f29  ath__, __name__)
```

## bosdyn/api/spot_cam/compositor_pb2.py

```diff
@@ -13,15 +13,15 @@
 
 
 from bosdyn.api import header_pb2 as bosdyn_dot_api_dot_header__pb2
 from bosdyn.api.spot_cam import camera_pb2 as bosdyn_dot_api_dot_spot__cam_dot_camera__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$bosdyn/api/spot_cam/compositor.proto\x12\x13\x62osdyn.api.spot_cam\x1a\x17\x62osdyn/api/header.proto\x1a bosdyn/api/spot_cam/camera.proto\x1a\x1egoogle/protobuf/wrappers.proto\"!\n\x11ScreenDescription\x12\x0c\n\x04name\x18\x01 \x01(\t\"=\n\x10GetScreenRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"M\n\x11GetScreenResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x0c\n\x04name\x18\x02 \x01(\t\"E\n\x18GetVisibleCamerasRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"\xe0\x02\n\x19GetVisibleCamerasResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x46\n\x07streams\x18\x02 \x03(\x0b\x32\x35.bosdyn.api.spot_cam.GetVisibleCamerasResponse.Stream\x1a\xce\x01\n\x06Stream\x12L\n\x06window\x18\x01 \x01(\x0b\x32<.bosdyn.api.spot_cam.GetVisibleCamerasResponse.Stream.Window\x12+\n\x06\x63\x61mera\x18\x02 \x01(\x0b\x32\x1b.bosdyn.api.spot_cam.Camera\x1aI\n\x06Window\x12\x0f\n\x07xoffset\x18\x01 \x01(\x05\x12\x0f\n\x07yoffset\x18\x02 \x01(\x05\x12\r\n\x05width\x18\x03 \x01(\x05\x12\x0e\n\x06height\x18\x04 \x01(\x05\"?\n\x12ListScreensRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"z\n\x13ListScreensResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x37\n\x07screens\x18\x02 \x03(\x0b\x32&.bosdyn.api.spot_cam.ScreenDescription\"K\n\x10SetScreenRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x0c\n\x04name\x18\x02 \x01(\t\"M\n\x11SetScreenResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x0c\n\x04name\x18\x02 \x01(\t\"\xd3\x02\n\nIrColorMap\x12:\n\x08\x63olormap\x18\x01 \x01(\x0e\x32(.bosdyn.api.spot_cam.IrColorMap.ColorMap\x12:\n\x05scale\x18\x02 \x01(\x0b\x32+.bosdyn.api.spot_cam.IrColorMap.ScalingPair\x12.\n\nauto_scale\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x1a\'\n\x0bScalingPair\x12\x0b\n\x03min\x18\x01 \x01(\x01\x12\x0b\n\x03max\x18\x02 \x01(\x01\"t\n\x08\x43olorMap\x12\x14\n\x10\x43OLORMAP_UNKNOWN\x10\x00\x12\x16\n\x12\x43OLORMAP_GREYSCALE\x10\x01\x12\x10\n\x0c\x43OLORMAP_JET\x10\x02\x12\x14\n\x10\x43OLORMAP_INFERNO\x10\x03\x12\x12\n\x0e\x43OLORMAP_TURBO\x10\x04\"o\n\x14SetIrColormapRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12,\n\x03map\x18\x02 \x01(\x0b\x32\x1f.bosdyn.api.spot_cam.IrColorMap\"C\n\x15SetIrColormapResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\"A\n\x14GetIrColormapRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"q\n\x15GetIrColormapResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12,\n\x03map\x18\x02 \x01(\x0b\x32\x1f.bosdyn.api.spot_cam.IrColorMap\"\x9a\x01\n\x0eIrMeterOverlay\x12\x0e\n\x06\x65nable\x18\x01 \x01(\x08\x12I\n\x06\x63oords\x18\x02 \x01(\x0b\x32\x39.bosdyn.api.spot_cam.IrMeterOverlay.NormalizedCoordinates\x1a-\n\x15NormalizedCoordinates\x12\t\n\x01x\x18\x01 \x01(\x01\x12\t\n\x01y\x18\x02 \x01(\x01\"{\n\x18SetIrMeterOverlayRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x34\n\x07overlay\x18\x02 \x01(\x0b\x32#.bosdyn.api.spot_cam.IrMeterOverlay\"G\n\x19SetIrMeterOverlayResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeaderB\x11\x42\x0f\x43ompositorProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$bosdyn/api/spot_cam/compositor.proto\x12\x13\x62osdyn.api.spot_cam\x1a\x17\x62osdyn/api/header.proto\x1a bosdyn/api/spot_cam/camera.proto\x1a\x1egoogle/protobuf/wrappers.proto\"!\n\x11ScreenDescription\x12\x0c\n\x04name\x18\x01 \x01(\t\"=\n\x10GetScreenRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"M\n\x11GetScreenResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x0c\n\x04name\x18\x02 \x01(\t\"E\n\x18GetVisibleCamerasRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"\xe0\x02\n\x19GetVisibleCamerasResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x46\n\x07streams\x18\x02 \x03(\x0b\x32\x35.bosdyn.api.spot_cam.GetVisibleCamerasResponse.Stream\x1a\xce\x01\n\x06Stream\x12L\n\x06window\x18\x01 \x01(\x0b\x32<.bosdyn.api.spot_cam.GetVisibleCamerasResponse.Stream.Window\x12+\n\x06\x63\x61mera\x18\x02 \x01(\x0b\x32\x1b.bosdyn.api.spot_cam.Camera\x1aI\n\x06Window\x12\x0f\n\x07xoffset\x18\x01 \x01(\x05\x12\x0f\n\x07yoffset\x18\x02 \x01(\x05\x12\r\n\x05width\x18\x03 \x01(\x05\x12\x0e\n\x06height\x18\x04 \x01(\x05\"?\n\x12ListScreensRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"z\n\x13ListScreensResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x37\n\x07screens\x18\x02 \x03(\x0b\x32&.bosdyn.api.spot_cam.ScreenDescription\"K\n\x10SetScreenRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x0c\n\x04name\x18\x02 \x01(\t\"M\n\x11SetScreenResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x0c\n\x04name\x18\x02 \x01(\t\"\xd3\x02\n\nIrColorMap\x12:\n\x08\x63olormap\x18\x01 \x01(\x0e\x32(.bosdyn.api.spot_cam.IrColorMap.ColorMap\x12:\n\x05scale\x18\x02 \x01(\x0b\x32+.bosdyn.api.spot_cam.IrColorMap.ScalingPair\x12.\n\nauto_scale\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x1a\'\n\x0bScalingPair\x12\x0b\n\x03min\x18\x01 \x01(\x01\x12\x0b\n\x03max\x18\x02 \x01(\x01\"t\n\x08\x43olorMap\x12\x14\n\x10\x43OLORMAP_UNKNOWN\x10\x00\x12\x16\n\x12\x43OLORMAP_GREYSCALE\x10\x01\x12\x10\n\x0c\x43OLORMAP_JET\x10\x02\x12\x14\n\x10\x43OLORMAP_INFERNO\x10\x03\x12\x12\n\x0e\x43OLORMAP_TURBO\x10\x04\"o\n\x14SetIrColormapRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12,\n\x03map\x18\x02 \x01(\x0b\x32\x1f.bosdyn.api.spot_cam.IrColorMap\"C\n\x15SetIrColormapResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\"A\n\x14GetIrColormapRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"q\n\x15GetIrColormapResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12,\n\x03map\x18\x02 \x01(\x0b\x32\x1f.bosdyn.api.spot_cam.IrColorMap\"\xc6\x04\n\x0eIrMeterOverlay\x12\x0e\n\x06\x65nable\x18\x01 \x01(\x08\x12M\n\x06\x63oords\x18\x02 \x01(\x0b\x32\x39.bosdyn.api.spot_cam.IrMeterOverlay.NormalizedCoordinatesB\x02\x18\x01\x12H\n\x05meter\x18\x03 \x03(\x0b\x32\x39.bosdyn.api.spot_cam.IrMeterOverlay.NormalizedCoordinates\x12:\n\x04unit\x18\x04 \x01(\x0b\x32,.bosdyn.api.spot_cam.IrMeterOverlay.TempUnit\x12<\n\x05\x64\x65lta\x18\x05 \x03(\x0b\x32-.bosdyn.api.spot_cam.IrMeterOverlay.DeltaPair\x1a-\n\x15NormalizedCoordinates\x12\t\n\x01x\x18\x01 \x01(\x01\x12\t\n\x01y\x18\x02 \x01(\x01\x1a\xbe\x01\n\x08TempUnit\x12H\n\x05value\x18\x01 \x01(\x0e\x32\x39.bosdyn.api.spot_cam.IrMeterOverlay.TempUnit.TempUnitType\"h\n\x0cTempUnitType\x12\x14\n\x10TEMPUNIT_UNKNOWN\x10\x00\x12\x14\n\x10TEMPUNIT_CELSIUS\x10\x01\x12\x17\n\x13TEMPUNIT_FAHRENHEIT\x10\x02\x12\x13\n\x0fTEMPUNIT_KELVIN\x10\x03\x1a!\n\tDeltaPair\x12\t\n\x01\x61\x18\x01 \x01(\x05\x12\t\n\x01\x62\x18\x02 \x01(\x05\"{\n\x18SetIrMeterOverlayRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x34\n\x07overlay\x18\x02 \x01(\x0b\x32#.bosdyn.api.spot_cam.IrMeterOverlay\"G\n\x19SetIrMeterOverlayResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\"E\n\x18GetIrMeterOverlayRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"}\n\x19GetIrMeterOverlayResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x34\n\x07overlay\x18\x02 \x01(\x0b\x32#.bosdyn.api.spot_cam.IrMeterOverlayB\x11\x42\x0f\x43ompositorProtob\x06proto3')
 
 
 
 _SCREENDESCRIPTION = DESCRIPTOR.message_types_by_name['ScreenDescription']
 _GETSCREENREQUEST = DESCRIPTOR.message_types_by_name['GetScreenRequest']
 _GETSCREENRESPONSE = DESCRIPTOR.message_types_by_name['GetScreenResponse']
 _GETVISIBLECAMERASREQUEST = DESCRIPTOR.message_types_by_name['GetVisibleCamerasRequest']
@@ -36,17 +36,22 @@
 _IRCOLORMAP_SCALINGPAIR = _IRCOLORMAP.nested_types_by_name['ScalingPair']
 _SETIRCOLORMAPREQUEST = DESCRIPTOR.message_types_by_name['SetIrColormapRequest']
 _SETIRCOLORMAPRESPONSE = DESCRIPTOR.message_types_by_name['SetIrColormapResponse']
 _GETIRCOLORMAPREQUEST = DESCRIPTOR.message_types_by_name['GetIrColormapRequest']
 _GETIRCOLORMAPRESPONSE = DESCRIPTOR.message_types_by_name['GetIrColormapResponse']
 _IRMETEROVERLAY = DESCRIPTOR.message_types_by_name['IrMeterOverlay']
 _IRMETEROVERLAY_NORMALIZEDCOORDINATES = _IRMETEROVERLAY.nested_types_by_name['NormalizedCoordinates']
+_IRMETEROVERLAY_TEMPUNIT = _IRMETEROVERLAY.nested_types_by_name['TempUnit']
+_IRMETEROVERLAY_DELTAPAIR = _IRMETEROVERLAY.nested_types_by_name['DeltaPair']
 _SETIRMETEROVERLAYREQUEST = DESCRIPTOR.message_types_by_name['SetIrMeterOverlayRequest']
 _SETIRMETEROVERLAYRESPONSE = DESCRIPTOR.message_types_by_name['SetIrMeterOverlayResponse']
+_GETIRMETEROVERLAYREQUEST = DESCRIPTOR.message_types_by_name['GetIrMeterOverlayRequest']
+_GETIRMETEROVERLAYRESPONSE = DESCRIPTOR.message_types_by_name['GetIrMeterOverlayResponse']
 _IRCOLORMAP_COLORMAP = _IRCOLORMAP.enum_types_by_name['ColorMap']
+_IRMETEROVERLAY_TEMPUNIT_TEMPUNITTYPE = _IRMETEROVERLAY_TEMPUNIT.enum_types_by_name['TempUnitType']
 ScreenDescription = _reflection.GeneratedProtocolMessageType('ScreenDescription', (_message.Message,), {
   'DESCRIPTOR' : _SCREENDESCRIPTION,
   '__module__' : 'bosdyn.api.spot_cam.compositor_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.spot_cam.ScreenDescription)
   })
 _sym_db.RegisterMessage(ScreenDescription)
 
@@ -169,20 +174,36 @@
 
   'NormalizedCoordinates' : _reflection.GeneratedProtocolMessageType('NormalizedCoordinates', (_message.Message,), {
     'DESCRIPTOR' : _IRMETEROVERLAY_NORMALIZEDCOORDINATES,
     '__module__' : 'bosdyn.api.spot_cam.compositor_pb2'
     # @@protoc_insertion_point(class_scope:bosdyn.api.spot_cam.IrMeterOverlay.NormalizedCoordinates)
     })
   ,
+
+  'TempUnit' : _reflection.GeneratedProtocolMessageType('TempUnit', (_message.Message,), {
+    'DESCRIPTOR' : _IRMETEROVERLAY_TEMPUNIT,
+    '__module__' : 'bosdyn.api.spot_cam.compositor_pb2'
+    # @@protoc_insertion_point(class_scope:bosdyn.api.spot_cam.IrMeterOverlay.TempUnit)
+    })
+  ,
+
+  'DeltaPair' : _reflection.GeneratedProtocolMessageType('DeltaPair', (_message.Message,), {
+    'DESCRIPTOR' : _IRMETEROVERLAY_DELTAPAIR,
+    '__module__' : 'bosdyn.api.spot_cam.compositor_pb2'
+    # @@protoc_insertion_point(class_scope:bosdyn.api.spot_cam.IrMeterOverlay.DeltaPair)
+    })
+  ,
   'DESCRIPTOR' : _IRMETEROVERLAY,
   '__module__' : 'bosdyn.api.spot_cam.compositor_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.spot_cam.IrMeterOverlay)
   })
 _sym_db.RegisterMessage(IrMeterOverlay)
 _sym_db.RegisterMessage(IrMeterOverlay.NormalizedCoordinates)
+_sym_db.RegisterMessage(IrMeterOverlay.TempUnit)
+_sym_db.RegisterMessage(IrMeterOverlay.DeltaPair)
 
 SetIrMeterOverlayRequest = _reflection.GeneratedProtocolMessageType('SetIrMeterOverlayRequest', (_message.Message,), {
   'DESCRIPTOR' : _SETIRMETEROVERLAYREQUEST,
   '__module__' : 'bosdyn.api.spot_cam.compositor_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.spot_cam.SetIrMeterOverlayRequest)
   })
 _sym_db.RegisterMessage(SetIrMeterOverlayRequest)
@@ -190,18 +211,34 @@
 SetIrMeterOverlayResponse = _reflection.GeneratedProtocolMessageType('SetIrMeterOverlayResponse', (_message.Message,), {
   'DESCRIPTOR' : _SETIRMETEROVERLAYRESPONSE,
   '__module__' : 'bosdyn.api.spot_cam.compositor_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.spot_cam.SetIrMeterOverlayResponse)
   })
 _sym_db.RegisterMessage(SetIrMeterOverlayResponse)
 
+GetIrMeterOverlayRequest = _reflection.GeneratedProtocolMessageType('GetIrMeterOverlayRequest', (_message.Message,), {
+  'DESCRIPTOR' : _GETIRMETEROVERLAYREQUEST,
+  '__module__' : 'bosdyn.api.spot_cam.compositor_pb2'
+  # @@protoc_insertion_point(class_scope:bosdyn.api.spot_cam.GetIrMeterOverlayRequest)
+  })
+_sym_db.RegisterMessage(GetIrMeterOverlayRequest)
+
+GetIrMeterOverlayResponse = _reflection.GeneratedProtocolMessageType('GetIrMeterOverlayResponse', (_message.Message,), {
+  'DESCRIPTOR' : _GETIRMETEROVERLAYRESPONSE,
+  '__module__' : 'bosdyn.api.spot_cam.compositor_pb2'
+  # @@protoc_insertion_point(class_scope:bosdyn.api.spot_cam.GetIrMeterOverlayResponse)
+  })
+_sym_db.RegisterMessage(GetIrMeterOverlayResponse)
+
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'B\017CompositorProto'
+  _IRMETEROVERLAY.fields_by_name['coords']._options = None
+  _IRMETEROVERLAY.fields_by_name['coords']._serialized_options = b'\030\001'
   _SCREENDESCRIPTION._serialized_start=152
   _SCREENDESCRIPTION._serialized_end=185
   _GETSCREENREQUEST._serialized_start=187
   _GETSCREENREQUEST._serialized_end=248
   _GETSCREENRESPONSE._serialized_start=250
   _GETSCREENRESPONSE._serialized_end=327
   _GETVISIBLECAMERASREQUEST._serialized_start=329
@@ -231,15 +268,25 @@
   _SETIRCOLORMAPRESPONSE._serialized_start=1555
   _SETIRCOLORMAPRESPONSE._serialized_end=1622
   _GETIRCOLORMAPREQUEST._serialized_start=1624
   _GETIRCOLORMAPREQUEST._serialized_end=1689
   _GETIRCOLORMAPRESPONSE._serialized_start=1691
   _GETIRCOLORMAPRESPONSE._serialized_end=1804
   _IRMETEROVERLAY._serialized_start=1807
-  _IRMETEROVERLAY._serialized_end=1961
-  _IRMETEROVERLAY_NORMALIZEDCOORDINATES._serialized_start=1916
-  _IRMETEROVERLAY_NORMALIZEDCOORDINATES._serialized_end=1961
-  _SETIRMETEROVERLAYREQUEST._serialized_start=1963
-  _SETIRMETEROVERLAYREQUEST._serialized_end=2086
-  _SETIRMETEROVERLAYRESPONSE._serialized_start=2088
-  _SETIRMETEROVERLAYRESPONSE._serialized_end=2159
+  _IRMETEROVERLAY._serialized_end=2389
+  _IRMETEROVERLAY_NORMALIZEDCOORDINATES._serialized_start=2116
+  _IRMETEROVERLAY_NORMALIZEDCOORDINATES._serialized_end=2161
+  _IRMETEROVERLAY_TEMPUNIT._serialized_start=2164
+  _IRMETEROVERLAY_TEMPUNIT._serialized_end=2354
+  _IRMETEROVERLAY_TEMPUNIT_TEMPUNITTYPE._serialized_start=2250
+  _IRMETEROVERLAY_TEMPUNIT_TEMPUNITTYPE._serialized_end=2354
+  _IRMETEROVERLAY_DELTAPAIR._serialized_start=2356
+  _IRMETEROVERLAY_DELTAPAIR._serialized_end=2389
+  _SETIRMETEROVERLAYREQUEST._serialized_start=2391
+  _SETIRMETEROVERLAYREQUEST._serialized_end=2514
+  _SETIRMETEROVERLAYRESPONSE._serialized_start=2516
+  _SETIRMETEROVERLAYRESPONSE._serialized_end=2587
+  _GETIRMETEROVERLAYREQUEST._serialized_start=2589
+  _GETIRMETEROVERLAYREQUEST._serialized_end=2658
+  _GETIRMETEROVERLAYRESPONSE._serialized_start=2660
+  _GETIRMETEROVERLAYRESPONSE._serialized_end=2785
 # @@protoc_insertion_point(module_scope)
```

## bosdyn/api/spot_cam/network_pb2.py

```diff
@@ -12,29 +12,32 @@
 _sym_db = _symbol_database.Default()
 
 
 from bosdyn.api import header_pb2 as bosdyn_dot_api_dot_header__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!bosdyn/api/spot_cam/network.proto\x12\x13\x62osdyn.api.spot_cam\x1a\x17\x62osdyn/api/header.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\xc6\x01\n\x0cNetworkTuple\x12-\n\x07\x61\x64\x64ress\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12-\n\x07netmask\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12-\n\x07gateway\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12)\n\x03mtu\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\"F\n\x19GetNetworkSettingsRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"}\n\x1aGetNetworkSettingsResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x33\n\x08settings\x18\x02 \x01(\x0b\x32!.bosdyn.api.spot_cam.NetworkTuple\">\n\x11GetSSLCertRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"U\n\x12GetSSLCertResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x13\n\x0b\x63\x65rtificate\x18\x02 \x01(\t\"\x92\x01\n\tICEServer\x12\x37\n\x04type\x18\x01 \x01(\x0e\x32).bosdyn.api.spot_cam.ICEServer.servertype\x12\x0f\n\x07\x61\x64\x64ress\x18\x02 \x01(\t\x12\x0c\n\x04port\x18\x03 \x01(\r\"-\n\nservertype\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04STUN\x10\x01\x12\x08\n\x04TURN\x10\x02\"G\n\x1aGetICEConfigurationRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"z\n\x1bGetICEConfigurationResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12/\n\x07servers\x18\x02 \x03(\x0b\x32\x1e.bosdyn.api.spot_cam.ICEServer\"x\n\x1aSetICEConfigurationRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12/\n\x07servers\x18\x02 \x03(\x0b\x32\x1e.bosdyn.api.spot_cam.ICEServer\"I\n\x1bSetICEConfigurationResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeaderB\x0e\x42\x0cNetworkProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!bosdyn/api/spot_cam/network.proto\x12\x13\x62osdyn.api.spot_cam\x1a\x17\x62osdyn/api/header.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\xc6\x01\n\x0cNetworkTuple\x12-\n\x07\x61\x64\x64ress\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12-\n\x07netmask\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12-\n\x07gateway\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12)\n\x03mtu\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\"F\n\x19GetNetworkSettingsRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"}\n\x1aGetNetworkSettingsResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x33\n\x08settings\x18\x02 \x01(\x0b\x32!.bosdyn.api.spot_cam.NetworkTuple\">\n\x11GetSSLCertRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"U\n\x12GetSSLCertResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x13\n\x0b\x63\x65rtificate\x18\x02 \x01(\t\"\xd4\x04\n\tICEServer\x12\x37\n\x04type\x18\x01 \x01(\x0e\x32).bosdyn.api.spot_cam.ICEServer.servertype\x12\x0f\n\x07\x61\x64\x64ress\x18\x02 \x01(\t\x12\x0c\n\x04port\x18\x03 \x01(\r\x12>\n\ttransport\x18\x04 \x01(\x0e\x32+.bosdyn.api.spot_cam.ICEServer.icetransport\x12\x38\n\x04\x61uth\x18\x05 \x01(\x0b\x32*.bosdyn.api.spot_cam.ICEServer.auth_params\x1a\xf8\x01\n\x0b\x61uth_params\x12.\n\x08username\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x46\n\x05oauth\x18\x02 \x01(\x0b\x32\x35.bosdyn.api.spot_cam.ICEServer.auth_params.oauth_pairH\x00\x12\x30\n\x08password\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValueH\x00\x1a\x31\n\noauth_pair\x12\x0e\n\x06MACKey\x18\x01 \x01(\t\x12\x13\n\x0b\x41\x63\x63\x65ssToken\x18\x02 \x01(\tB\x0c\n\ncredential\"-\n\nservertype\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04STUN\x10\x01\x12\x08\n\x04TURN\x10\x02\"K\n\x0cicetransport\x12\x15\n\x11TRANSPORT_UNKNOWN\x10\x00\x12\x11\n\rTRANSPORT_UDP\x10\x01\x12\x11\n\rTRANSPORT_TCP\x10\x02\"G\n\x1aGetICEConfigurationRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"z\n\x1bGetICEConfigurationResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12/\n\x07servers\x18\x02 \x03(\x0b\x32\x1e.bosdyn.api.spot_cam.ICEServer\"x\n\x1aSetICEConfigurationRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12/\n\x07servers\x18\x02 \x03(\x0b\x32\x1e.bosdyn.api.spot_cam.ICEServer\"I\n\x1bSetICEConfigurationResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeaderB\x0e\x42\x0cNetworkProtob\x06proto3')
 
 
 
 _NETWORKTUPLE = DESCRIPTOR.message_types_by_name['NetworkTuple']
 _GETNETWORKSETTINGSREQUEST = DESCRIPTOR.message_types_by_name['GetNetworkSettingsRequest']
 _GETNETWORKSETTINGSRESPONSE = DESCRIPTOR.message_types_by_name['GetNetworkSettingsResponse']
 _GETSSLCERTREQUEST = DESCRIPTOR.message_types_by_name['GetSSLCertRequest']
 _GETSSLCERTRESPONSE = DESCRIPTOR.message_types_by_name['GetSSLCertResponse']
 _ICESERVER = DESCRIPTOR.message_types_by_name['ICEServer']
+_ICESERVER_AUTH_PARAMS = _ICESERVER.nested_types_by_name['auth_params']
+_ICESERVER_AUTH_PARAMS_OAUTH_PAIR = _ICESERVER_AUTH_PARAMS.nested_types_by_name['oauth_pair']
 _GETICECONFIGURATIONREQUEST = DESCRIPTOR.message_types_by_name['GetICEConfigurationRequest']
 _GETICECONFIGURATIONRESPONSE = DESCRIPTOR.message_types_by_name['GetICEConfigurationResponse']
 _SETICECONFIGURATIONREQUEST = DESCRIPTOR.message_types_by_name['SetICEConfigurationRequest']
 _SETICECONFIGURATIONRESPONSE = DESCRIPTOR.message_types_by_name['SetICEConfigurationResponse']
 _ICESERVER_SERVERTYPE = _ICESERVER.enum_types_by_name['servertype']
+_ICESERVER_ICETRANSPORT = _ICESERVER.enum_types_by_name['icetransport']
 NetworkTuple = _reflection.GeneratedProtocolMessageType('NetworkTuple', (_message.Message,), {
   'DESCRIPTOR' : _NETWORKTUPLE,
   '__module__' : 'bosdyn.api.spot_cam.network_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.spot_cam.NetworkTuple)
   })
 _sym_db.RegisterMessage(NetworkTuple)
 
@@ -63,19 +66,35 @@
   'DESCRIPTOR' : _GETSSLCERTRESPONSE,
   '__module__' : 'bosdyn.api.spot_cam.network_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.spot_cam.GetSSLCertResponse)
   })
 _sym_db.RegisterMessage(GetSSLCertResponse)
 
 ICEServer = _reflection.GeneratedProtocolMessageType('ICEServer', (_message.Message,), {
+
+  'auth_params' : _reflection.GeneratedProtocolMessageType('auth_params', (_message.Message,), {
+
+    'oauth_pair' : _reflection.GeneratedProtocolMessageType('oauth_pair', (_message.Message,), {
+      'DESCRIPTOR' : _ICESERVER_AUTH_PARAMS_OAUTH_PAIR,
+      '__module__' : 'bosdyn.api.spot_cam.network_pb2'
+      # @@protoc_insertion_point(class_scope:bosdyn.api.spot_cam.ICEServer.auth_params.oauth_pair)
+      })
+    ,
+    'DESCRIPTOR' : _ICESERVER_AUTH_PARAMS,
+    '__module__' : 'bosdyn.api.spot_cam.network_pb2'
+    # @@protoc_insertion_point(class_scope:bosdyn.api.spot_cam.ICEServer.auth_params)
+    })
+  ,
   'DESCRIPTOR' : _ICESERVER,
   '__module__' : 'bosdyn.api.spot_cam.network_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.spot_cam.ICEServer)
   })
 _sym_db.RegisterMessage(ICEServer)
+_sym_db.RegisterMessage(ICEServer.auth_params)
+_sym_db.RegisterMessage(ICEServer.auth_params.oauth_pair)
 
 GetICEConfigurationRequest = _reflection.GeneratedProtocolMessageType('GetICEConfigurationRequest', (_message.Message,), {
   'DESCRIPTOR' : _GETICECONFIGURATIONREQUEST,
   '__module__' : 'bosdyn.api.spot_cam.network_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.spot_cam.GetICEConfigurationRequest)
   })
 _sym_db.RegisterMessage(GetICEConfigurationRequest)
@@ -112,19 +131,25 @@
   _GETNETWORKSETTINGSRESPONSE._serialized_start=388
   _GETNETWORKSETTINGSRESPONSE._serialized_end=513
   _GETSSLCERTREQUEST._serialized_start=515
   _GETSSLCERTREQUEST._serialized_end=577
   _GETSSLCERTRESPONSE._serialized_start=579
   _GETSSLCERTRESPONSE._serialized_end=664
   _ICESERVER._serialized_start=667
-  _ICESERVER._serialized_end=813
-  _ICESERVER_SERVERTYPE._serialized_start=768
-  _ICESERVER_SERVERTYPE._serialized_end=813
-  _GETICECONFIGURATIONREQUEST._serialized_start=815
-  _GETICECONFIGURATIONREQUEST._serialized_end=886
-  _GETICECONFIGURATIONRESPONSE._serialized_start=888
-  _GETICECONFIGURATIONRESPONSE._serialized_end=1010
-  _SETICECONFIGURATIONREQUEST._serialized_start=1012
-  _SETICECONFIGURATIONREQUEST._serialized_end=1132
-  _SETICECONFIGURATIONRESPONSE._serialized_start=1134
-  _SETICECONFIGURATIONRESPONSE._serialized_end=1207
+  _ICESERVER._serialized_end=1263
+  _ICESERVER_AUTH_PARAMS._serialized_start=891
+  _ICESERVER_AUTH_PARAMS._serialized_end=1139
+  _ICESERVER_AUTH_PARAMS_OAUTH_PAIR._serialized_start=1076
+  _ICESERVER_AUTH_PARAMS_OAUTH_PAIR._serialized_end=1125
+  _ICESERVER_SERVERTYPE._serialized_start=1141
+  _ICESERVER_SERVERTYPE._serialized_end=1186
+  _ICESERVER_ICETRANSPORT._serialized_start=1188
+  _ICESERVER_ICETRANSPORT._serialized_end=1263
+  _GETICECONFIGURATIONREQUEST._serialized_start=1265
+  _GETICECONFIGURATIONREQUEST._serialized_end=1336
+  _GETICECONFIGURATIONRESPONSE._serialized_start=1338
+  _GETICECONFIGURATIONRESPONSE._serialized_end=1460
+  _SETICECONFIGURATIONREQUEST._serialized_start=1462
+  _SETICECONFIGURATIONREQUEST._serialized_end=1582
+  _SETICECONFIGURATIONRESPONSE._serialized_start=1584
+  _SETICECONFIGURATIONRESPONSE._serialized_end=1657
 # @@protoc_insertion_point(module_scope)
```

## bosdyn/api/spot_cam/ptz_pb2.py

```diff
@@ -12,15 +12,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from bosdyn.api import header_pb2 as bosdyn_dot_api_dot_header__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1d\x62osdyn/api/spot_cam/ptz.proto\x12\x13\x62osdyn.api.spot_cam\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x17\x62osdyn/api/header.proto\"\xbb\x02\n\x0ePtzDescription\x12\x0c\n\x04name\x18\x01 \x01(\t\x12=\n\tpan_limit\x18\x02 \x01(\x0b\x32*.bosdyn.api.spot_cam.PtzDescription.Limits\x12>\n\ntilt_limit\x18\x03 \x01(\x0b\x32*.bosdyn.api.spot_cam.PtzDescription.Limits\x12>\n\nzoom_limit\x18\x04 \x01(\x0b\x32*.bosdyn.api.spot_cam.PtzDescription.Limits\x1a\\\n\x06Limits\x12(\n\x03min\x18\x01 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x12(\n\x03max\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\"\xbf\x01\n\x0bPtzPosition\x12\x30\n\x03ptz\x18\x02 \x01(\x0b\x32#.bosdyn.api.spot_cam.PtzDescription\x12(\n\x03pan\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x12)\n\x04tilt\x18\x04 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x12)\n\x04zoom\x18\x05 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\"\xbf\x01\n\x0bPtzVelocity\x12\x30\n\x03ptz\x18\x02 \x01(\x0b\x32#.bosdyn.api.spot_cam.PtzDescription\x12(\n\x03pan\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x12)\n\x04tilt\x18\x04 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x12)\n\x04zoom\x18\x05 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\"t\n\x15GetPtzPositionRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x30\n\x03ptz\x18\x02 \x01(\x0b\x32#.bosdyn.api.spot_cam.PtzDescription\"x\n\x16GetPtzPositionResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x32\n\x08position\x18\x02 \x01(\x0b\x32 .bosdyn.api.spot_cam.PtzPosition\"t\n\x15GetPtzVelocityRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x30\n\x03ptz\x18\x02 \x01(\x0b\x32#.bosdyn.api.spot_cam.PtzDescription\"x\n\x16GetPtzVelocityResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x32\n\x08velocity\x18\x02 \x01(\x0b\x32 .bosdyn.api.spot_cam.PtzVelocity\";\n\x0eListPtzRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"p\n\x0fListPtzResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x31\n\x04ptzs\x18\x02 \x03(\x0b\x32#.bosdyn.api.spot_cam.PtzDescription\"v\n\x15SetPtzPositionRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x32\n\x08position\x18\x02 \x01(\x0b\x32 .bosdyn.api.spot_cam.PtzPosition\"x\n\x16SetPtzPositionResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x32\n\x08position\x18\x02 \x01(\x0b\x32 .bosdyn.api.spot_cam.PtzPosition\"v\n\x15SetPtzVelocityRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x32\n\x08velocity\x18\x02 \x01(\x0b\x32 .bosdyn.api.spot_cam.PtzVelocity\"x\n\x16SetPtzVelocityResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x32\n\x08velocity\x18\x02 \x01(\x0b\x32 .bosdyn.api.spot_cam.PtzVelocity\"B\n\x15InitializeLensRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"D\n\x16InitializeLensResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeaderB\nB\x08PtzProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1d\x62osdyn/api/spot_cam/ptz.proto\x12\x13\x62osdyn.api.spot_cam\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x17\x62osdyn/api/header.proto\"\xbb\x02\n\x0ePtzDescription\x12\x0c\n\x04name\x18\x01 \x01(\t\x12=\n\tpan_limit\x18\x02 \x01(\x0b\x32*.bosdyn.api.spot_cam.PtzDescription.Limits\x12>\n\ntilt_limit\x18\x03 \x01(\x0b\x32*.bosdyn.api.spot_cam.PtzDescription.Limits\x12>\n\nzoom_limit\x18\x04 \x01(\x0b\x32*.bosdyn.api.spot_cam.PtzDescription.Limits\x1a\\\n\x06Limits\x12(\n\x03min\x18\x01 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x12(\n\x03max\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\"\xbf\x01\n\x0bPtzPosition\x12\x30\n\x03ptz\x18\x02 \x01(\x0b\x32#.bosdyn.api.spot_cam.PtzDescription\x12(\n\x03pan\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x12)\n\x04tilt\x18\x04 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x12)\n\x04zoom\x18\x05 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\"\xbf\x01\n\x0bPtzVelocity\x12\x30\n\x03ptz\x18\x02 \x01(\x0b\x32#.bosdyn.api.spot_cam.PtzDescription\x12(\n\x03pan\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x12)\n\x04tilt\x18\x04 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\x12)\n\x04zoom\x18\x05 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\"t\n\x15GetPtzPositionRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x30\n\x03ptz\x18\x02 \x01(\x0b\x32#.bosdyn.api.spot_cam.PtzDescription\"x\n\x16GetPtzPositionResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x32\n\x08position\x18\x02 \x01(\x0b\x32 .bosdyn.api.spot_cam.PtzPosition\"t\n\x15GetPtzVelocityRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x30\n\x03ptz\x18\x02 \x01(\x0b\x32#.bosdyn.api.spot_cam.PtzDescription\"x\n\x16GetPtzVelocityResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x32\n\x08velocity\x18\x02 \x01(\x0b\x32 .bosdyn.api.spot_cam.PtzVelocity\";\n\x0eListPtzRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"p\n\x0fListPtzResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x31\n\x04ptzs\x18\x02 \x03(\x0b\x32#.bosdyn.api.spot_cam.PtzDescription\"v\n\x15SetPtzPositionRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x32\n\x08position\x18\x02 \x01(\x0b\x32 .bosdyn.api.spot_cam.PtzPosition\"x\n\x16SetPtzPositionResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x32\n\x08position\x18\x02 \x01(\x0b\x32 .bosdyn.api.spot_cam.PtzPosition\"v\n\x15SetPtzVelocityRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x32\n\x08velocity\x18\x02 \x01(\x0b\x32 .bosdyn.api.spot_cam.PtzVelocity\"x\n\x16SetPtzVelocityResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x32\n\x08velocity\x18\x02 \x01(\x0b\x32 .bosdyn.api.spot_cam.PtzVelocity\"B\n\x15InitializeLensRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"D\n\x16InitializeLensResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\"\x8c\x02\n\rPtzFocusState\x12=\n\x04mode\x18\x01 \x01(\x0e\x32/.bosdyn.api.spot_cam.PtzFocusState.PtzFocusMode\x12\x33\n\x0e\x66ocus_position\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\x12\x34\n\x0f\x61pprox_distance\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\"Q\n\x0cPtzFocusMode\x12\x17\n\x13PTZ_FOCUS_UNDEFINED\x10\x00\x12\x12\n\x0ePTZ_FOCUS_AUTO\x10\x01\x12\x14\n\x10PTZ_FOCUS_MANUAL\x10\x02\"}\n\x17SetPtzFocusStateRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x37\n\x0b\x66ocus_state\x18\x02 \x01(\x0b\x32\".bosdyn.api.spot_cam.PtzFocusState\"F\n\x18SetPtzFocusStateResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\"D\n\x17GetPtzFocusStateRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"\x7f\n\x18GetPtzFocusStateResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x37\n\x0b\x66ocus_state\x18\x02 \x01(\x0b\x32\".bosdyn.api.spot_cam.PtzFocusStateB\nB\x08PtzProtob\x06proto3')
 
 
 
 _PTZDESCRIPTION = DESCRIPTOR.message_types_by_name['PtzDescription']
 _PTZDESCRIPTION_LIMITS = _PTZDESCRIPTION.nested_types_by_name['Limits']
 _PTZPOSITION = DESCRIPTOR.message_types_by_name['PtzPosition']
 _PTZVELOCITY = DESCRIPTOR.message_types_by_name['PtzVelocity']
@@ -32,14 +32,20 @@
 _LISTPTZRESPONSE = DESCRIPTOR.message_types_by_name['ListPtzResponse']
 _SETPTZPOSITIONREQUEST = DESCRIPTOR.message_types_by_name['SetPtzPositionRequest']
 _SETPTZPOSITIONRESPONSE = DESCRIPTOR.message_types_by_name['SetPtzPositionResponse']
 _SETPTZVELOCITYREQUEST = DESCRIPTOR.message_types_by_name['SetPtzVelocityRequest']
 _SETPTZVELOCITYRESPONSE = DESCRIPTOR.message_types_by_name['SetPtzVelocityResponse']
 _INITIALIZELENSREQUEST = DESCRIPTOR.message_types_by_name['InitializeLensRequest']
 _INITIALIZELENSRESPONSE = DESCRIPTOR.message_types_by_name['InitializeLensResponse']
+_PTZFOCUSSTATE = DESCRIPTOR.message_types_by_name['PtzFocusState']
+_SETPTZFOCUSSTATEREQUEST = DESCRIPTOR.message_types_by_name['SetPtzFocusStateRequest']
+_SETPTZFOCUSSTATERESPONSE = DESCRIPTOR.message_types_by_name['SetPtzFocusStateResponse']
+_GETPTZFOCUSSTATEREQUEST = DESCRIPTOR.message_types_by_name['GetPtzFocusStateRequest']
+_GETPTZFOCUSSTATERESPONSE = DESCRIPTOR.message_types_by_name['GetPtzFocusStateResponse']
+_PTZFOCUSSTATE_PTZFOCUSMODE = _PTZFOCUSSTATE.enum_types_by_name['PtzFocusMode']
 PtzDescription = _reflection.GeneratedProtocolMessageType('PtzDescription', (_message.Message,), {
 
   'Limits' : _reflection.GeneratedProtocolMessageType('Limits', (_message.Message,), {
     'DESCRIPTOR' : _PTZDESCRIPTION_LIMITS,
     '__module__' : 'bosdyn.api.spot_cam.ptz_pb2'
     # @@protoc_insertion_point(class_scope:bosdyn.api.spot_cam.PtzDescription.Limits)
     })
@@ -145,14 +151,49 @@
 InitializeLensResponse = _reflection.GeneratedProtocolMessageType('InitializeLensResponse', (_message.Message,), {
   'DESCRIPTOR' : _INITIALIZELENSRESPONSE,
   '__module__' : 'bosdyn.api.spot_cam.ptz_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.spot_cam.InitializeLensResponse)
   })
 _sym_db.RegisterMessage(InitializeLensResponse)
 
+PtzFocusState = _reflection.GeneratedProtocolMessageType('PtzFocusState', (_message.Message,), {
+  'DESCRIPTOR' : _PTZFOCUSSTATE,
+  '__module__' : 'bosdyn.api.spot_cam.ptz_pb2'
+  # @@protoc_insertion_point(class_scope:bosdyn.api.spot_cam.PtzFocusState)
+  })
+_sym_db.RegisterMessage(PtzFocusState)
+
+SetPtzFocusStateRequest = _reflection.GeneratedProtocolMessageType('SetPtzFocusStateRequest', (_message.Message,), {
+  'DESCRIPTOR' : _SETPTZFOCUSSTATEREQUEST,
+  '__module__' : 'bosdyn.api.spot_cam.ptz_pb2'
+  # @@protoc_insertion_point(class_scope:bosdyn.api.spot_cam.SetPtzFocusStateRequest)
+  })
+_sym_db.RegisterMessage(SetPtzFocusStateRequest)
+
+SetPtzFocusStateResponse = _reflection.GeneratedProtocolMessageType('SetPtzFocusStateResponse', (_message.Message,), {
+  'DESCRIPTOR' : _SETPTZFOCUSSTATERESPONSE,
+  '__module__' : 'bosdyn.api.spot_cam.ptz_pb2'
+  # @@protoc_insertion_point(class_scope:bosdyn.api.spot_cam.SetPtzFocusStateResponse)
+  })
+_sym_db.RegisterMessage(SetPtzFocusStateResponse)
+
+GetPtzFocusStateRequest = _reflection.GeneratedProtocolMessageType('GetPtzFocusStateRequest', (_message.Message,), {
+  'DESCRIPTOR' : _GETPTZFOCUSSTATEREQUEST,
+  '__module__' : 'bosdyn.api.spot_cam.ptz_pb2'
+  # @@protoc_insertion_point(class_scope:bosdyn.api.spot_cam.GetPtzFocusStateRequest)
+  })
+_sym_db.RegisterMessage(GetPtzFocusStateRequest)
+
+GetPtzFocusStateResponse = _reflection.GeneratedProtocolMessageType('GetPtzFocusStateResponse', (_message.Message,), {
+  'DESCRIPTOR' : _GETPTZFOCUSSTATERESPONSE,
+  '__module__' : 'bosdyn.api.spot_cam.ptz_pb2'
+  # @@protoc_insertion_point(class_scope:bosdyn.api.spot_cam.GetPtzFocusStateResponse)
+  })
+_sym_db.RegisterMessage(GetPtzFocusStateResponse)
+
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'B\010PtzProto'
   _PTZDESCRIPTION._serialized_start=112
   _PTZDESCRIPTION._serialized_end=427
   _PTZDESCRIPTION_LIMITS._serialized_start=335
@@ -181,8 +222,20 @@
   _SETPTZVELOCITYREQUEST._serialized_end=1832
   _SETPTZVELOCITYRESPONSE._serialized_start=1834
   _SETPTZVELOCITYRESPONSE._serialized_end=1954
   _INITIALIZELENSREQUEST._serialized_start=1956
   _INITIALIZELENSREQUEST._serialized_end=2022
   _INITIALIZELENSRESPONSE._serialized_start=2024
   _INITIALIZELENSRESPONSE._serialized_end=2092
+  _PTZFOCUSSTATE._serialized_start=2095
+  _PTZFOCUSSTATE._serialized_end=2363
+  _PTZFOCUSSTATE_PTZFOCUSMODE._serialized_start=2282
+  _PTZFOCUSSTATE_PTZFOCUSMODE._serialized_end=2363
+  _SETPTZFOCUSSTATEREQUEST._serialized_start=2365
+  _SETPTZFOCUSSTATEREQUEST._serialized_end=2490
+  _SETPTZFOCUSSTATERESPONSE._serialized_start=2492
+  _SETPTZFOCUSSTATERESPONSE._serialized_end=2562
+  _GETPTZFOCUSSTATEREQUEST._serialized_start=2564
+  _GETPTZFOCUSSTATEREQUEST._serialized_end=2632
+  _GETPTZFOCUSSTATERESPONSE._serialized_start=2634
+  _GETPTZFOCUSSTATERESPONSE._serialized_end=2761
 # @@protoc_insertion_point(module_scope)
```

## bosdyn/api/spot_cam/service_pb2.py

```diff
@@ -20,15 +20,15 @@
 from bosdyn.api.spot_cam import ptz_pb2 as bosdyn_dot_api_dot_spot__cam_dot_ptz__pb2
 from bosdyn.api.spot_cam import audio_pb2 as bosdyn_dot_api_dot_spot__cam_dot_audio__pb2
 from bosdyn.api.spot_cam import health_pb2 as bosdyn_dot_api_dot_spot__cam_dot_health__pb2
 from bosdyn.api.spot_cam import network_pb2 as bosdyn_dot_api_dot_spot__cam_dot_network__pb2
 from bosdyn.api.spot_cam import version_pb2 as bosdyn_dot_api_dot_spot__cam_dot_version__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!bosdyn/api/spot_cam/service.proto\x12\x13\x62osdyn.api.spot_cam\x1a$bosdyn/api/spot_cam/compositor.proto\x1a\'bosdyn/api/spot_cam/streamquality.proto\x1a\x1f\x62osdyn/api/spot_cam/power.proto\x1a\x1d\x62osdyn/api/spot_cam/LED.proto\x1a!bosdyn/api/spot_cam/logging.proto\x1a\x1d\x62osdyn/api/spot_cam/ptz.proto\x1a\x1f\x62osdyn/api/spot_cam/audio.proto\x1a bosdyn/api/spot_cam/health.proto\x1a!bosdyn/api/spot_cam/network.proto\x1a!bosdyn/api/spot_cam/version.proto2\xe5\x05\n\x11\x43ompositorService\x12Z\n\tSetScreen\x12%.bosdyn.api.spot_cam.SetScreenRequest\x1a&.bosdyn.api.spot_cam.SetScreenResponse\x12Z\n\tGetScreen\x12%.bosdyn.api.spot_cam.GetScreenRequest\x1a&.bosdyn.api.spot_cam.GetScreenResponse\x12`\n\x0bListScreens\x12\'.bosdyn.api.spot_cam.ListScreensRequest\x1a(.bosdyn.api.spot_cam.ListScreensResponse\x12r\n\x11GetVisibleCameras\x12-.bosdyn.api.spot_cam.GetVisibleCamerasRequest\x1a..bosdyn.api.spot_cam.GetVisibleCamerasResponse\x12\x66\n\rSetIrColormap\x12).bosdyn.api.spot_cam.SetIrColormapRequest\x1a*.bosdyn.api.spot_cam.SetIrColormapResponse\x12\x66\n\rGetIrColormap\x12).bosdyn.api.spot_cam.GetIrColormapRequest\x1a*.bosdyn.api.spot_cam.GetIrColormapResponse\x12r\n\x11SetIrMeterOverlay\x12-.bosdyn.api.spot_cam.SetIrMeterOverlayRequest\x1a..bosdyn.api.spot_cam.SetIrMeterOverlayResponse2\xf9\x02\n\x14StreamQualityService\x12l\n\x0fSetStreamParams\x12+.bosdyn.api.spot_cam.SetStreamParamsRequest\x1a,.bosdyn.api.spot_cam.SetStreamParamsResponse\x12l\n\x0fGetStreamParams\x12+.bosdyn.api.spot_cam.GetStreamParamsRequest\x1a,.bosdyn.api.spot_cam.GetStreamParamsResponse\x12\x84\x01\n\x17\x45nableCongestionControl\x12\x33.bosdyn.api.spot_cam.EnableCongestionControlRequest\x1a\x34.bosdyn.api.spot_cam.EnableCongestionControlResponse2\xc3\x02\n\x0cPowerService\x12i\n\x0eSetPowerStatus\x12*.bosdyn.api.spot_cam.SetPowerStatusRequest\x1a+.bosdyn.api.spot_cam.SetPowerStatusResponse\x12i\n\x0eGetPowerStatus\x12*.bosdyn.api.spot_cam.GetPowerStatusRequest\x1a+.bosdyn.api.spot_cam.GetPowerStatusResponse\x12]\n\nCyclePower\x12&.bosdyn.api.spot_cam.CyclePowerRequest\x1a\'.bosdyn.api.spot_cam.CyclePowerResponse2\xf3\x01\n\x0fLightingService\x12o\n\x10SetLEDBrightness\x12,.bosdyn.api.spot_cam.SetLEDBrightnessRequest\x1a-.bosdyn.api.spot_cam.SetLEDBrightnessResponse\x12o\n\x10GetLEDBrightness\x12,.bosdyn.api.spot_cam.GetLEDBrightnessRequest\x1a-.bosdyn.api.spot_cam.GetLEDBrightnessResponse2\xaf\x07\n\x0fMediaLogService\x12N\n\x05Store\x12!.bosdyn.api.spot_cam.StoreRequest\x1a\".bosdyn.api.spot_cam.StoreResponse\x12Z\n\tGetStatus\x12%.bosdyn.api.spot_cam.GetStatusRequest\x1a&.bosdyn.api.spot_cam.GetStatusResponse\x12H\n\x03Tag\x12\x1f.bosdyn.api.spot_cam.TagRequest\x1a .bosdyn.api.spot_cam.TagResponse\x12T\n\x0b\x45nableDebug\x12!.bosdyn.api.spot_cam.DebugRequest\x1a\".bosdyn.api.spot_cam.DebugResponse\x12`\n\x0bListCameras\x12\'.bosdyn.api.spot_cam.ListCamerasRequest\x1a(.bosdyn.api.spot_cam.ListCamerasResponse\x12n\n\x0fRetrieveRawData\x12+.bosdyn.api.spot_cam.RetrieveRawDataRequest\x1a,.bosdyn.api.spot_cam.RetrieveRawDataResponse0\x01\x12Y\n\x08Retrieve\x12$.bosdyn.api.spot_cam.RetrieveRequest\x1a%.bosdyn.api.spot_cam.RetrieveResponse0\x01\x12Q\n\x06\x44\x65lete\x12\".bosdyn.api.spot_cam.DeleteRequest\x1a#.bosdyn.api.spot_cam.DeleteResponse\x12h\n\rListLogpoints\x12).bosdyn.api.spot_cam.ListLogpointsRequest\x1a*.bosdyn.api.spot_cam.ListLogpointsResponse0\x01\x12\x66\n\rSetPassphrase\x12).bosdyn.api.spot_cam.SetPassphraseRequest\x1a*.bosdyn.api.spot_cam.SetPassphraseResponse2\xf9\x04\n\nPtzService\x12i\n\x0eSetPtzPosition\x12*.bosdyn.api.spot_cam.SetPtzPositionRequest\x1a+.bosdyn.api.spot_cam.SetPtzPositionResponse\x12i\n\x0eGetPtzPosition\x12*.bosdyn.api.spot_cam.GetPtzPositionRequest\x1a+.bosdyn.api.spot_cam.GetPtzPositionResponse\x12i\n\x0eSetPtzVelocity\x12*.bosdyn.api.spot_cam.SetPtzVelocityRequest\x1a+.bosdyn.api.spot_cam.SetPtzVelocityResponse\x12i\n\x0eGetPtzVelocity\x12*.bosdyn.api.spot_cam.GetPtzVelocityRequest\x1a+.bosdyn.api.spot_cam.GetPtzVelocityResponse\x12T\n\x07ListPtz\x12#.bosdyn.api.spot_cam.ListPtzRequest\x1a$.bosdyn.api.spot_cam.ListPtzResponse\x12i\n\x0eInitializeLens\x12*.bosdyn.api.spot_cam.InitializeLensRequest\x1a+.bosdyn.api.spot_cam.InitializeLensResponse2\xbd\x08\n\x0c\x41udioService\x12Z\n\tPlaySound\x12%.bosdyn.api.spot_cam.PlaySoundRequest\x1a&.bosdyn.api.spot_cam.PlaySoundResponse\x12\\\n\tLoadSound\x12%.bosdyn.api.spot_cam.LoadSoundRequest\x1a&.bosdyn.api.spot_cam.LoadSoundResponse(\x01\x12`\n\x0b\x44\x65leteSound\x12\'.bosdyn.api.spot_cam.DeleteSoundRequest\x1a(.bosdyn.api.spot_cam.DeleteSoundResponse\x12]\n\nListSounds\x12&.bosdyn.api.spot_cam.ListSoundsRequest\x1a\'.bosdyn.api.spot_cam.ListSoundsResponse\x12Z\n\tSetVolume\x12%.bosdyn.api.spot_cam.SetVolumeRequest\x1a&.bosdyn.api.spot_cam.SetVolumeResponse\x12Z\n\tGetVolume\x12%.bosdyn.api.spot_cam.GetVolumeRequest\x1a&.bosdyn.api.spot_cam.GetVolumeResponse\x12\x81\x01\n\x16SetAudioCaptureChannel\x12\x32.bosdyn.api.spot_cam.SetAudioCaptureChannelRequest\x1a\x33.bosdyn.api.spot_cam.SetAudioCaptureChannelResponse\x12\x81\x01\n\x16GetAudioCaptureChannel\x12\x32.bosdyn.api.spot_cam.GetAudioCaptureChannelRequest\x1a\x33.bosdyn.api.spot_cam.GetAudioCaptureChannelResponse\x12x\n\x13SetAudioCaptureGain\x12/.bosdyn.api.spot_cam.SetAudioCaptureGainRequest\x1a\x30.bosdyn.api.spot_cam.SetAudioCaptureGainResponse\x12x\n\x13GetAudioCaptureGain\x12/.bosdyn.api.spot_cam.GetAudioCaptureGainRequest\x1a\x30.bosdyn.api.spot_cam.GetAudioCaptureGainResponse2\xb1\x03\n\rHealthService\x12i\n\x0eGetTemperature\x12*.bosdyn.api.spot_cam.GetTemperatureRequest\x1a+.bosdyn.api.spot_cam.GetTemperatureResponse\x12\x63\n\x0cGetBITStatus\x12(.bosdyn.api.spot_cam.GetBITStatusRequest\x1a).bosdyn.api.spot_cam.GetBITStatusResponse\x12i\n\x0e\x43learBITEvents\x12*.bosdyn.api.spot_cam.ClearBITEventsRequest\x1a+.bosdyn.api.spot_cam.ClearBITEventsResponse\x12\x65\n\x0cGetSystemLog\x12(.bosdyn.api.spot_cam.GetSystemLogRequest\x1a).bosdyn.api.spot_cam.GetSystemLogResponse0\x01\x32\x84\x02\n\x0eNetworkService\x12x\n\x13SetICEConfiguration\x12/.bosdyn.api.spot_cam.SetICEConfigurationRequest\x1a\x30.bosdyn.api.spot_cam.SetICEConfigurationResponse\x12x\n\x13GetICEConfiguration\x12/.bosdyn.api.spot_cam.GetICEConfigurationRequest\x1a\x30.bosdyn.api.spot_cam.GetICEConfigurationResponse2\x87\x01\n\x0eVersionService\x12u\n\x12GetSoftwareVersion\x12..bosdyn.api.spot_cam.GetSoftwareVersionRequest\x1a/.bosdyn.api.spot_cam.GetSoftwareVersionResponseB\x0e\x42\x0cServiceProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!bosdyn/api/spot_cam/service.proto\x12\x13\x62osdyn.api.spot_cam\x1a$bosdyn/api/spot_cam/compositor.proto\x1a\'bosdyn/api/spot_cam/streamquality.proto\x1a\x1f\x62osdyn/api/spot_cam/power.proto\x1a\x1d\x62osdyn/api/spot_cam/LED.proto\x1a!bosdyn/api/spot_cam/logging.proto\x1a\x1d\x62osdyn/api/spot_cam/ptz.proto\x1a\x1f\x62osdyn/api/spot_cam/audio.proto\x1a bosdyn/api/spot_cam/health.proto\x1a!bosdyn/api/spot_cam/network.proto\x1a!bosdyn/api/spot_cam/version.proto2\xd9\x06\n\x11\x43ompositorService\x12Z\n\tSetScreen\x12%.bosdyn.api.spot_cam.SetScreenRequest\x1a&.bosdyn.api.spot_cam.SetScreenResponse\x12Z\n\tGetScreen\x12%.bosdyn.api.spot_cam.GetScreenRequest\x1a&.bosdyn.api.spot_cam.GetScreenResponse\x12`\n\x0bListScreens\x12\'.bosdyn.api.spot_cam.ListScreensRequest\x1a(.bosdyn.api.spot_cam.ListScreensResponse\x12r\n\x11GetVisibleCameras\x12-.bosdyn.api.spot_cam.GetVisibleCamerasRequest\x1a..bosdyn.api.spot_cam.GetVisibleCamerasResponse\x12\x66\n\rSetIrColormap\x12).bosdyn.api.spot_cam.SetIrColormapRequest\x1a*.bosdyn.api.spot_cam.SetIrColormapResponse\x12\x66\n\rGetIrColormap\x12).bosdyn.api.spot_cam.GetIrColormapRequest\x1a*.bosdyn.api.spot_cam.GetIrColormapResponse\x12r\n\x11SetIrMeterOverlay\x12-.bosdyn.api.spot_cam.SetIrMeterOverlayRequest\x1a..bosdyn.api.spot_cam.SetIrMeterOverlayResponse\x12r\n\x11GetIrMeterOverlay\x12-.bosdyn.api.spot_cam.GetIrMeterOverlayRequest\x1a..bosdyn.api.spot_cam.GetIrMeterOverlayResponse2\xf9\x02\n\x14StreamQualityService\x12l\n\x0fSetStreamParams\x12+.bosdyn.api.spot_cam.SetStreamParamsRequest\x1a,.bosdyn.api.spot_cam.SetStreamParamsResponse\x12l\n\x0fGetStreamParams\x12+.bosdyn.api.spot_cam.GetStreamParamsRequest\x1a,.bosdyn.api.spot_cam.GetStreamParamsResponse\x12\x84\x01\n\x17\x45nableCongestionControl\x12\x33.bosdyn.api.spot_cam.EnableCongestionControlRequest\x1a\x34.bosdyn.api.spot_cam.EnableCongestionControlResponse2\xc3\x02\n\x0cPowerService\x12i\n\x0eSetPowerStatus\x12*.bosdyn.api.spot_cam.SetPowerStatusRequest\x1a+.bosdyn.api.spot_cam.SetPowerStatusResponse\x12i\n\x0eGetPowerStatus\x12*.bosdyn.api.spot_cam.GetPowerStatusRequest\x1a+.bosdyn.api.spot_cam.GetPowerStatusResponse\x12]\n\nCyclePower\x12&.bosdyn.api.spot_cam.CyclePowerRequest\x1a\'.bosdyn.api.spot_cam.CyclePowerResponse2\xf3\x01\n\x0fLightingService\x12o\n\x10SetLEDBrightness\x12,.bosdyn.api.spot_cam.SetLEDBrightnessRequest\x1a-.bosdyn.api.spot_cam.SetLEDBrightnessResponse\x12o\n\x10GetLEDBrightness\x12,.bosdyn.api.spot_cam.GetLEDBrightnessRequest\x1a-.bosdyn.api.spot_cam.GetLEDBrightnessResponse2\xaf\x07\n\x0fMediaLogService\x12N\n\x05Store\x12!.bosdyn.api.spot_cam.StoreRequest\x1a\".bosdyn.api.spot_cam.StoreResponse\x12Z\n\tGetStatus\x12%.bosdyn.api.spot_cam.GetStatusRequest\x1a&.bosdyn.api.spot_cam.GetStatusResponse\x12H\n\x03Tag\x12\x1f.bosdyn.api.spot_cam.TagRequest\x1a .bosdyn.api.spot_cam.TagResponse\x12T\n\x0b\x45nableDebug\x12!.bosdyn.api.spot_cam.DebugRequest\x1a\".bosdyn.api.spot_cam.DebugResponse\x12`\n\x0bListCameras\x12\'.bosdyn.api.spot_cam.ListCamerasRequest\x1a(.bosdyn.api.spot_cam.ListCamerasResponse\x12n\n\x0fRetrieveRawData\x12+.bosdyn.api.spot_cam.RetrieveRawDataRequest\x1a,.bosdyn.api.spot_cam.RetrieveRawDataResponse0\x01\x12Y\n\x08Retrieve\x12$.bosdyn.api.spot_cam.RetrieveRequest\x1a%.bosdyn.api.spot_cam.RetrieveResponse0\x01\x12Q\n\x06\x44\x65lete\x12\".bosdyn.api.spot_cam.DeleteRequest\x1a#.bosdyn.api.spot_cam.DeleteResponse\x12h\n\rListLogpoints\x12).bosdyn.api.spot_cam.ListLogpointsRequest\x1a*.bosdyn.api.spot_cam.ListLogpointsResponse0\x01\x12\x66\n\rSetPassphrase\x12).bosdyn.api.spot_cam.SetPassphraseRequest\x1a*.bosdyn.api.spot_cam.SetPassphraseResponse2\xdb\x06\n\nPtzService\x12i\n\x0eSetPtzPosition\x12*.bosdyn.api.spot_cam.SetPtzPositionRequest\x1a+.bosdyn.api.spot_cam.SetPtzPositionResponse\x12i\n\x0eGetPtzPosition\x12*.bosdyn.api.spot_cam.GetPtzPositionRequest\x1a+.bosdyn.api.spot_cam.GetPtzPositionResponse\x12i\n\x0eSetPtzVelocity\x12*.bosdyn.api.spot_cam.SetPtzVelocityRequest\x1a+.bosdyn.api.spot_cam.SetPtzVelocityResponse\x12i\n\x0eGetPtzVelocity\x12*.bosdyn.api.spot_cam.GetPtzVelocityRequest\x1a+.bosdyn.api.spot_cam.GetPtzVelocityResponse\x12T\n\x07ListPtz\x12#.bosdyn.api.spot_cam.ListPtzRequest\x1a$.bosdyn.api.spot_cam.ListPtzResponse\x12i\n\x0eInitializeLens\x12*.bosdyn.api.spot_cam.InitializeLensRequest\x1a+.bosdyn.api.spot_cam.InitializeLensResponse\x12o\n\x10SetPtzFocusState\x12,.bosdyn.api.spot_cam.SetPtzFocusStateRequest\x1a-.bosdyn.api.spot_cam.SetPtzFocusStateResponse\x12o\n\x10GetPtzFocusState\x12,.bosdyn.api.spot_cam.GetPtzFocusStateRequest\x1a-.bosdyn.api.spot_cam.GetPtzFocusStateResponse2\xbd\x08\n\x0c\x41udioService\x12Z\n\tPlaySound\x12%.bosdyn.api.spot_cam.PlaySoundRequest\x1a&.bosdyn.api.spot_cam.PlaySoundResponse\x12\\\n\tLoadSound\x12%.bosdyn.api.spot_cam.LoadSoundRequest\x1a&.bosdyn.api.spot_cam.LoadSoundResponse(\x01\x12`\n\x0b\x44\x65leteSound\x12\'.bosdyn.api.spot_cam.DeleteSoundRequest\x1a(.bosdyn.api.spot_cam.DeleteSoundResponse\x12]\n\nListSounds\x12&.bosdyn.api.spot_cam.ListSoundsRequest\x1a\'.bosdyn.api.spot_cam.ListSoundsResponse\x12Z\n\tSetVolume\x12%.bosdyn.api.spot_cam.SetVolumeRequest\x1a&.bosdyn.api.spot_cam.SetVolumeResponse\x12Z\n\tGetVolume\x12%.bosdyn.api.spot_cam.GetVolumeRequest\x1a&.bosdyn.api.spot_cam.GetVolumeResponse\x12\x81\x01\n\x16SetAudioCaptureChannel\x12\x32.bosdyn.api.spot_cam.SetAudioCaptureChannelRequest\x1a\x33.bosdyn.api.spot_cam.SetAudioCaptureChannelResponse\x12\x81\x01\n\x16GetAudioCaptureChannel\x12\x32.bosdyn.api.spot_cam.GetAudioCaptureChannelRequest\x1a\x33.bosdyn.api.spot_cam.GetAudioCaptureChannelResponse\x12x\n\x13SetAudioCaptureGain\x12/.bosdyn.api.spot_cam.SetAudioCaptureGainRequest\x1a\x30.bosdyn.api.spot_cam.SetAudioCaptureGainResponse\x12x\n\x13GetAudioCaptureGain\x12/.bosdyn.api.spot_cam.GetAudioCaptureGainRequest\x1a\x30.bosdyn.api.spot_cam.GetAudioCaptureGainResponse2\xb1\x03\n\rHealthService\x12i\n\x0eGetTemperature\x12*.bosdyn.api.spot_cam.GetTemperatureRequest\x1a+.bosdyn.api.spot_cam.GetTemperatureResponse\x12\x63\n\x0cGetBITStatus\x12(.bosdyn.api.spot_cam.GetBITStatusRequest\x1a).bosdyn.api.spot_cam.GetBITStatusResponse\x12i\n\x0e\x43learBITEvents\x12*.bosdyn.api.spot_cam.ClearBITEventsRequest\x1a+.bosdyn.api.spot_cam.ClearBITEventsResponse\x12\x65\n\x0cGetSystemLog\x12(.bosdyn.api.spot_cam.GetSystemLogRequest\x1a).bosdyn.api.spot_cam.GetSystemLogResponse0\x01\x32\x84\x02\n\x0eNetworkService\x12x\n\x13SetICEConfiguration\x12/.bosdyn.api.spot_cam.SetICEConfigurationRequest\x1a\x30.bosdyn.api.spot_cam.SetICEConfigurationResponse\x12x\n\x13GetICEConfiguration\x12/.bosdyn.api.spot_cam.GetICEConfigurationRequest\x1a\x30.bosdyn.api.spot_cam.GetICEConfigurationResponse2\x87\x01\n\x0eVersionService\x12u\n\x12GetSoftwareVersion\x12..bosdyn.api.spot_cam.GetSoftwareVersionRequest\x1a/.bosdyn.api.spot_cam.GetSoftwareVersionResponseB\x0e\x42\x0cServiceProtob\x06proto3')
 
 
 
 _COMPOSITORSERVICE = DESCRIPTOR.services_by_name['CompositorService']
 _STREAMQUALITYSERVICE = DESCRIPTOR.services_by_name['StreamQualityService']
 _POWERSERVICE = DESCRIPTOR.services_by_name['PowerService']
 _LIGHTINGSERVICE = DESCRIPTOR.services_by_name['LightingService']
@@ -39,27 +39,27 @@
 _NETWORKSERVICE = DESCRIPTOR.services_by_name['NetworkService']
 _VERSIONSERVICE = DESCRIPTOR.services_by_name['VersionService']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'B\014ServiceProto'
   _COMPOSITORSERVICE._serialized_start=405
-  _COMPOSITORSERVICE._serialized_end=1146
-  _STREAMQUALITYSERVICE._serialized_start=1149
-  _STREAMQUALITYSERVICE._serialized_end=1526
-  _POWERSERVICE._serialized_start=1529
-  _POWERSERVICE._serialized_end=1852
-  _LIGHTINGSERVICE._serialized_start=1855
-  _LIGHTINGSERVICE._serialized_end=2098
-  _MEDIALOGSERVICE._serialized_start=2101
-  _MEDIALOGSERVICE._serialized_end=3044
-  _PTZSERVICE._serialized_start=3047
-  _PTZSERVICE._serialized_end=3680
-  _AUDIOSERVICE._serialized_start=3683
-  _AUDIOSERVICE._serialized_end=4768
-  _HEALTHSERVICE._serialized_start=4771
-  _HEALTHSERVICE._serialized_end=5204
-  _NETWORKSERVICE._serialized_start=5207
-  _NETWORKSERVICE._serialized_end=5467
-  _VERSIONSERVICE._serialized_start=5470
-  _VERSIONSERVICE._serialized_end=5605
+  _COMPOSITORSERVICE._serialized_end=1262
+  _STREAMQUALITYSERVICE._serialized_start=1265
+  _STREAMQUALITYSERVICE._serialized_end=1642
+  _POWERSERVICE._serialized_start=1645
+  _POWERSERVICE._serialized_end=1968
+  _LIGHTINGSERVICE._serialized_start=1971
+  _LIGHTINGSERVICE._serialized_end=2214
+  _MEDIALOGSERVICE._serialized_start=2217
+  _MEDIALOGSERVICE._serialized_end=3160
+  _PTZSERVICE._serialized_start=3163
+  _PTZSERVICE._serialized_end=4022
+  _AUDIOSERVICE._serialized_start=4025
+  _AUDIOSERVICE._serialized_end=5110
+  _HEALTHSERVICE._serialized_start=5113
+  _HEALTHSERVICE._serialized_end=5546
+  _NETWORKSERVICE._serialized_start=5549
+  _NETWORKSERVICE._serialized_end=5809
+  _VERSIONSERVICE._serialized_start=5812
+  _VERSIONSERVICE._serialized_end=5947
 # @@protoc_insertion_point(module_scope)
```

## bosdyn/api/spot_cam/service_pb2_grpc.py

```diff
@@ -55,14 +55,19 @@
                 response_deserializer=bosdyn_dot_api_dot_spot__cam_dot_compositor__pb2.GetIrColormapResponse.FromString,
                 )
         self.SetIrMeterOverlay = channel.unary_unary(
                 '/bosdyn.api.spot_cam.CompositorService/SetIrMeterOverlay',
                 request_serializer=bosdyn_dot_api_dot_spot__cam_dot_compositor__pb2.SetIrMeterOverlayRequest.SerializeToString,
                 response_deserializer=bosdyn_dot_api_dot_spot__cam_dot_compositor__pb2.SetIrMeterOverlayResponse.FromString,
                 )
+        self.GetIrMeterOverlay = channel.unary_unary(
+                '/bosdyn.api.spot_cam.CompositorService/GetIrMeterOverlay',
+                request_serializer=bosdyn_dot_api_dot_spot__cam_dot_compositor__pb2.GetIrMeterOverlayRequest.SerializeToString,
+                response_deserializer=bosdyn_dot_api_dot_spot__cam_dot_compositor__pb2.GetIrMeterOverlayResponse.FromString,
+                )
 
 
 class CompositorServiceServicer(object):
     """Change the layout of of the video stream between available presets.
     """
 
     def SetScreen(self, request, context):
@@ -110,14 +115,21 @@
     def SetIrMeterOverlay(self, request, context):
         """apply settings for the 'ir meter overlay'
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def GetIrMeterOverlay(self, request, context):
+        """retrieve settings for the 'ir meter overlay'
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_CompositorServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'SetScreen': grpc.unary_unary_rpc_method_handler(
                     servicer.SetScreen,
                     request_deserializer=bosdyn_dot_api_dot_spot__cam_dot_compositor__pb2.SetScreenRequest.FromString,
                     response_serializer=bosdyn_dot_api_dot_spot__cam_dot_compositor__pb2.SetScreenResponse.SerializeToString,
@@ -148,14 +160,19 @@
                     response_serializer=bosdyn_dot_api_dot_spot__cam_dot_compositor__pb2.GetIrColormapResponse.SerializeToString,
             ),
             'SetIrMeterOverlay': grpc.unary_unary_rpc_method_handler(
                     servicer.SetIrMeterOverlay,
                     request_deserializer=bosdyn_dot_api_dot_spot__cam_dot_compositor__pb2.SetIrMeterOverlayRequest.FromString,
                     response_serializer=bosdyn_dot_api_dot_spot__cam_dot_compositor__pb2.SetIrMeterOverlayResponse.SerializeToString,
             ),
+            'GetIrMeterOverlay': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetIrMeterOverlay,
+                    request_deserializer=bosdyn_dot_api_dot_spot__cam_dot_compositor__pb2.GetIrMeterOverlayRequest.FromString,
+                    response_serializer=bosdyn_dot_api_dot_spot__cam_dot_compositor__pb2.GetIrMeterOverlayResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'bosdyn.api.spot_cam.CompositorService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -278,14 +295,31 @@
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/bosdyn.api.spot_cam.CompositorService/SetIrMeterOverlay',
             bosdyn_dot_api_dot_spot__cam_dot_compositor__pb2.SetIrMeterOverlayRequest.SerializeToString,
             bosdyn_dot_api_dot_spot__cam_dot_compositor__pb2.SetIrMeterOverlayResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
+    @staticmethod
+    def GetIrMeterOverlay(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/bosdyn.api.spot_cam.CompositorService/GetIrMeterOverlay',
+            bosdyn_dot_api_dot_spot__cam_dot_compositor__pb2.GetIrMeterOverlayRequest.SerializeToString,
+            bosdyn_dot_api_dot_spot__cam_dot_compositor__pb2.GetIrMeterOverlayResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
 
 class StreamQualityServiceStub(object):
     """Set quality parameters for the stream, such as compression and image postprocessing settings.
     """
 
     def __init__(self, channel):
         """Constructor.
@@ -730,15 +764,16 @@
         """Tag updates the 'tag' field of the Logpoint that's passed, which must exist.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def EnableDebug(self, request, context):
-        """EnableDebug starts the periodic logging of health data to the database; this increases disk utilization, but will record data that is useful post-mortum
+        """EnableDebug starts the periodic logging of health data to the database; this increases disk
+        utilization, but will record data that is useful post-mortum
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def ListCameras(self, request, context):
         """ListCameras returns a list of strings that identify valid cameras for logging
@@ -1056,14 +1091,24 @@
                 response_deserializer=bosdyn_dot_api_dot_spot__cam_dot_ptz__pb2.ListPtzResponse.FromString,
                 )
         self.InitializeLens = channel.unary_unary(
                 '/bosdyn.api.spot_cam.PtzService/InitializeLens',
                 request_serializer=bosdyn_dot_api_dot_spot__cam_dot_ptz__pb2.InitializeLensRequest.SerializeToString,
                 response_deserializer=bosdyn_dot_api_dot_spot__cam_dot_ptz__pb2.InitializeLensResponse.FromString,
                 )
+        self.SetPtzFocusState = channel.unary_unary(
+                '/bosdyn.api.spot_cam.PtzService/SetPtzFocusState',
+                request_serializer=bosdyn_dot_api_dot_spot__cam_dot_ptz__pb2.SetPtzFocusStateRequest.SerializeToString,
+                response_deserializer=bosdyn_dot_api_dot_spot__cam_dot_ptz__pb2.SetPtzFocusStateResponse.FromString,
+                )
+        self.GetPtzFocusState = channel.unary_unary(
+                '/bosdyn.api.spot_cam.PtzService/GetPtzFocusState',
+                request_serializer=bosdyn_dot_api_dot_spot__cam_dot_ptz__pb2.GetPtzFocusStateRequest.SerializeToString,
+                response_deserializer=bosdyn_dot_api_dot_spot__cam_dot_ptz__pb2.GetPtzFocusStateResponse.FromString,
+                )
 
 
 class PtzServiceServicer(object):
     """Control real and virtual ptz mechanisms.
     """
 
     def SetPtzPosition(self, request, context):
@@ -1101,14 +1146,26 @@
     def InitializeLens(self, request, context):
         """Reinitializes PTZ autofocus
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def SetPtzFocusState(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def GetPtzFocusState(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_PtzServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'SetPtzPosition': grpc.unary_unary_rpc_method_handler(
                     servicer.SetPtzPosition,
                     request_deserializer=bosdyn_dot_api_dot_spot__cam_dot_ptz__pb2.SetPtzPositionRequest.FromString,
                     response_serializer=bosdyn_dot_api_dot_spot__cam_dot_ptz__pb2.SetPtzPositionResponse.SerializeToString,
@@ -1134,14 +1191,24 @@
                     response_serializer=bosdyn_dot_api_dot_spot__cam_dot_ptz__pb2.ListPtzResponse.SerializeToString,
             ),
             'InitializeLens': grpc.unary_unary_rpc_method_handler(
                     servicer.InitializeLens,
                     request_deserializer=bosdyn_dot_api_dot_spot__cam_dot_ptz__pb2.InitializeLensRequest.FromString,
                     response_serializer=bosdyn_dot_api_dot_spot__cam_dot_ptz__pb2.InitializeLensResponse.SerializeToString,
             ),
+            'SetPtzFocusState': grpc.unary_unary_rpc_method_handler(
+                    servicer.SetPtzFocusState,
+                    request_deserializer=bosdyn_dot_api_dot_spot__cam_dot_ptz__pb2.SetPtzFocusStateRequest.FromString,
+                    response_serializer=bosdyn_dot_api_dot_spot__cam_dot_ptz__pb2.SetPtzFocusStateResponse.SerializeToString,
+            ),
+            'GetPtzFocusState': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetPtzFocusState,
+                    request_deserializer=bosdyn_dot_api_dot_spot__cam_dot_ptz__pb2.GetPtzFocusStateRequest.FromString,
+                    response_serializer=bosdyn_dot_api_dot_spot__cam_dot_ptz__pb2.GetPtzFocusStateResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'bosdyn.api.spot_cam.PtzService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -1247,14 +1314,48 @@
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/bosdyn.api.spot_cam.PtzService/InitializeLens',
             bosdyn_dot_api_dot_spot__cam_dot_ptz__pb2.InitializeLensRequest.SerializeToString,
             bosdyn_dot_api_dot_spot__cam_dot_ptz__pb2.InitializeLensResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
+    @staticmethod
+    def SetPtzFocusState(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/bosdyn.api.spot_cam.PtzService/SetPtzFocusState',
+            bosdyn_dot_api_dot_spot__cam_dot_ptz__pb2.SetPtzFocusStateRequest.SerializeToString,
+            bosdyn_dot_api_dot_spot__cam_dot_ptz__pb2.SetPtzFocusStateResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetPtzFocusState(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/bosdyn.api.spot_cam.PtzService/GetPtzFocusState',
+            bosdyn_dot_api_dot_spot__cam_dot_ptz__pb2.GetPtzFocusStateRequest.SerializeToString,
+            bosdyn_dot_api_dot_spot__cam_dot_ptz__pb2.GetPtzFocusStateResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
 
 class AudioServiceStub(object):
     """Upload and play sounds over the SpotCam's speakers.
     """
 
     def __init__(self, channel):
         """Constructor.
@@ -1315,25 +1416,27 @@
 
 
 class AudioServiceServicer(object):
     """Upload and play sounds over the SpotCam's speakers.
     """
 
     def PlaySound(self, request, context):
-        """Given a soundRequest that identifies a single sound present in the system's sound effects table, PlaySound executes the sound effect.
+        """Given a soundRequest that identifies a single sound present in the system's sound effects
+        table, PlaySound executes the sound effect.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def LoadSound(self, request_iterator, context):
-        """LoadSound loads a sound effect into the system's sound table. The stream must contain a wav file, with a RIFF header describing it.
-        The arguement is a stream, to allow for sounds that are bigger then the MTU of the network; in this case, the complete stream must
-        contain the entire sound. If the stream ends early, an error will be returned. The header and sound fields of the entire stream must
-        be the same.
+        """LoadSound loads a sound effect into the system's sound table. The stream must contain a wav
+        file, with a RIFF header describing it. The arguement is a stream, to allow for sounds that
+        are bigger then the MTU of the network; in this case, the complete stream must contain the
+        entire sound. If the stream ends early, an error will be returned. The header and sound
+        fields of the entire stream must be the same.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def DeleteSound(self, request, context):
         """Delete the sound identified in the argument from the system's sound table.
@@ -1655,38 +1758,41 @@
 
 
 class HealthServiceServicer(object):
     """Query temperature and built-in test results.
     """
 
     def GetTemperature(self, request, context):
-        """GetTemperature returns a list of thermometers in the system, and the temperature that they measure.
+        """GetTemperature returns a list of thermometers in the system, and the temperature that they
+        measure.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetBITStatus(self, request, context):
-        """GetBitStatus returns two lists; a list of system events, and a list of ways that the system is degraded;
-        for instance, a degredation may include a missing PTZ unit, or a missing USB storage device.
+        """GetBitStatus returns two lists; a list of system events, and a list of ways that the system
+        is degraded; for instance, a degredation may include a missing PTZ unit, or a missing USB
+        storage device.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def ClearBITEvents(self, request, context):
         """ClearBitEvents clears out the events list of the BITStatus structure.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetSystemLog(self, request, context):
-        """GetSystemLog retrieves an encrypted log of system events, for factory diagnosis of possible issues.
-        The data streamed back should be concatenated to a single file, before sending to the manufacturer.
+        """GetSystemLog retrieves an encrypted log of system events, for factory diagnosis of possible
+        issues. The data streamed back should be concatenated to a single file, before sending to the
+        manufacturer.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_HealthServiceServicer_to_server(servicer, server):
@@ -1814,22 +1920,24 @@
 
 
 class NetworkServiceServicer(object):
     """Modify or query network settings of the SpotCam and ICE resolution servers.
     """
 
     def SetICEConfiguration(self, request, context):
-        """SetICEConfiguration sets up parameters for ICE, including addresses for STUN and TURN services
+        """SetICEConfiguration sets up parameters for ICE, including addresses for STUN and TURN
+        services
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetICEConfiguration(self, request, context):
-        """GetICEConfiguration retrieves currently set parameters for ICE, including addresses for STUN and TURN services
+        """GetICEConfiguration retrieves currently set parameters for ICE, including addresses for STUN
+        and TURN services
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_NetworkServiceServicer_to_server(servicer, server):
```

## bosdyn/api/spot_cam/streamquality_pb2.py

```diff
@@ -10,22 +10,26 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from bosdyn.api import header_pb2 as bosdyn_dot_api_dot_header__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
+from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'bosdyn/api/spot_cam/streamquality.proto\x12\x13\x62osdyn.api.spot_cam\x1a\x17\x62osdyn/api/header.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\xc6\x03\n\x0cStreamParams\x12\x32\n\rtargetbitrate\x18\x01 \x01(\x0b\x32\x1b.google.protobuf.Int64Value\x12\x34\n\x0frefreshinterval\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.Int64Value\x12\x30\n\x0bidrinterval\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.Int64Value\x12\x36\n\x03\x61wb\x18\x04 \x01(\x0b\x32).bosdyn.api.spot_cam.StreamParams.AwbMode\x1a\x45\n\x07\x41wbMode\x12:\n\x03\x61wb\x18\x01 \x01(\x0e\x32-.bosdyn.api.spot_cam.StreamParams.AwbModeEnum\"\x9a\x01\n\x0b\x41wbModeEnum\x12\x07\n\x03OFF\x10\x00\x12\x08\n\x04\x41UTO\x10\x01\x12\x10\n\x0cINCANDESCENT\x10\x02\x12\x0f\n\x0b\x46LUORESCENT\x10\x03\x12\x14\n\x10WARM_FLUORESCENT\x10\x04\x12\x0c\n\x08\x44\x41YLIGHT\x10\x05\x12\n\n\x06\x43LOUDY\x10\x06\x12\x0c\n\x08TWILIGHT\x10\x07\x12\t\n\x05SHADE\x10\x08\x12\x0c\n\x04\x44\x41RK\x10\t\x1a\x02\x08\x01\"C\n\x16GetStreamParamsRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"x\n\x17GetStreamParamsResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x31\n\x06params\x18\x02 \x01(\x0b\x32!.bosdyn.api.spot_cam.StreamParams\"v\n\x16SetStreamParamsRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x31\n\x06params\x18\x02 \x01(\x0b\x32!.bosdyn.api.spot_cam.StreamParams\"x\n\x17SetStreamParamsResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x31\n\x06params\x18\x02 \x01(\x0b\x32!.bosdyn.api.spot_cam.StreamParams\"n\n\x1e\x45nableCongestionControlRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12!\n\x19\x65nable_congestion_control\x18\x02 \x01(\x08\"M\n\x1f\x45nableCongestionControlResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeaderB\x14\x42\x12StreamQualityProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'bosdyn/api/spot_cam/streamquality.proto\x12\x13\x62osdyn.api.spot_cam\x1a\x17\x62osdyn/api/header.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x1egoogle/protobuf/duration.proto\"\xfb\x06\n\x0cStreamParams\x12\x32\n\rtargetbitrate\x18\x01 \x01(\x0b\x32\x1b.google.protobuf.Int64Value\x12\x34\n\x0frefreshinterval\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.Int64Value\x12\x30\n\x0bidrinterval\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.Int64Value\x12\x36\n\x03\x61wb\x18\x04 \x01(\x0b\x32).bosdyn.api.spot_cam.StreamParams.AwbMode\x12G\n\rauto_exposure\x18\x05 \x01(\x0b\x32..bosdyn.api.spot_cam.StreamParams.AutoExposureH\x00\x12K\n\rsync_exposure\x18\x06 \x01(\x0b\x32\x32.bosdyn.api.spot_cam.StreamParams.SyncAutoExposureH\x00\x12K\n\x0fmanual_exposure\x18\x07 \x01(\x0b\x32\x30.bosdyn.api.spot_cam.StreamParams.ManualExposureH\x00\x1a\x45\n\x07\x41wbMode\x12:\n\x03\x61wb\x18\x01 \x01(\x0e\x32-.bosdyn.api.spot_cam.StreamParams.AwbModeEnum\x1a\x0e\n\x0c\x41utoExposure\x1aJ\n\x10SyncAutoExposure\x12\x36\n\x11\x62rightness_target\x18\x01 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\x1ah\n\x0eManualExposure\x12+\n\x08\x65xposure\x18\x01 \x01(\x0b\x32\x19.google.protobuf.Duration\x12)\n\x04gain\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.FloatValue\"\x9a\x01\n\x0b\x41wbModeEnum\x12\x07\n\x03OFF\x10\x00\x12\x08\n\x04\x41UTO\x10\x01\x12\x10\n\x0cINCANDESCENT\x10\x02\x12\x0f\n\x0b\x46LUORESCENT\x10\x03\x12\x14\n\x10WARM_FLUORESCENT\x10\x04\x12\x0c\n\x08\x44\x41YLIGHT\x10\x05\x12\n\n\x06\x43LOUDY\x10\x06\x12\x0c\n\x08TWILIGHT\x10\x07\x12\t\n\x05SHADE\x10\x08\x12\x0c\n\x04\x44\x41RK\x10\t\x1a\x02\x08\x01\x42\n\n\x08\x65xposure\"C\n\x16GetStreamParamsRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"x\n\x17GetStreamParamsResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x31\n\x06params\x18\x02 \x01(\x0b\x32!.bosdyn.api.spot_cam.StreamParams\"v\n\x16SetStreamParamsRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x31\n\x06params\x18\x02 \x01(\x0b\x32!.bosdyn.api.spot_cam.StreamParams\"x\n\x17SetStreamParamsResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x31\n\x06params\x18\x02 \x01(\x0b\x32!.bosdyn.api.spot_cam.StreamParams\"n\n\x1e\x45nableCongestionControlRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12!\n\x19\x65nable_congestion_control\x18\x02 \x01(\x08\"M\n\x1f\x45nableCongestionControlResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeaderB\x14\x42\x12StreamQualityProtob\x06proto3')
 
 
 
 _STREAMPARAMS = DESCRIPTOR.message_types_by_name['StreamParams']
 _STREAMPARAMS_AWBMODE = _STREAMPARAMS.nested_types_by_name['AwbMode']
+_STREAMPARAMS_AUTOEXPOSURE = _STREAMPARAMS.nested_types_by_name['AutoExposure']
+_STREAMPARAMS_SYNCAUTOEXPOSURE = _STREAMPARAMS.nested_types_by_name['SyncAutoExposure']
+_STREAMPARAMS_MANUALEXPOSURE = _STREAMPARAMS.nested_types_by_name['ManualExposure']
 _GETSTREAMPARAMSREQUEST = DESCRIPTOR.message_types_by_name['GetStreamParamsRequest']
 _GETSTREAMPARAMSRESPONSE = DESCRIPTOR.message_types_by_name['GetStreamParamsResponse']
 _SETSTREAMPARAMSREQUEST = DESCRIPTOR.message_types_by_name['SetStreamParamsRequest']
 _SETSTREAMPARAMSRESPONSE = DESCRIPTOR.message_types_by_name['SetStreamParamsResponse']
 _ENABLECONGESTIONCONTROLREQUEST = DESCRIPTOR.message_types_by_name['EnableCongestionControlRequest']
 _ENABLECONGESTIONCONTROLRESPONSE = DESCRIPTOR.message_types_by_name['EnableCongestionControlResponse']
 _STREAMPARAMS_AWBMODEENUM = _STREAMPARAMS.enum_types_by_name['AwbModeEnum']
@@ -33,20 +37,44 @@
 
   'AwbMode' : _reflection.GeneratedProtocolMessageType('AwbMode', (_message.Message,), {
     'DESCRIPTOR' : _STREAMPARAMS_AWBMODE,
     '__module__' : 'bosdyn.api.spot_cam.streamquality_pb2'
     # @@protoc_insertion_point(class_scope:bosdyn.api.spot_cam.StreamParams.AwbMode)
     })
   ,
+
+  'AutoExposure' : _reflection.GeneratedProtocolMessageType('AutoExposure', (_message.Message,), {
+    'DESCRIPTOR' : _STREAMPARAMS_AUTOEXPOSURE,
+    '__module__' : 'bosdyn.api.spot_cam.streamquality_pb2'
+    # @@protoc_insertion_point(class_scope:bosdyn.api.spot_cam.StreamParams.AutoExposure)
+    })
+  ,
+
+  'SyncAutoExposure' : _reflection.GeneratedProtocolMessageType('SyncAutoExposure', (_message.Message,), {
+    'DESCRIPTOR' : _STREAMPARAMS_SYNCAUTOEXPOSURE,
+    '__module__' : 'bosdyn.api.spot_cam.streamquality_pb2'
+    # @@protoc_insertion_point(class_scope:bosdyn.api.spot_cam.StreamParams.SyncAutoExposure)
+    })
+  ,
+
+  'ManualExposure' : _reflection.GeneratedProtocolMessageType('ManualExposure', (_message.Message,), {
+    'DESCRIPTOR' : _STREAMPARAMS_MANUALEXPOSURE,
+    '__module__' : 'bosdyn.api.spot_cam.streamquality_pb2'
+    # @@protoc_insertion_point(class_scope:bosdyn.api.spot_cam.StreamParams.ManualExposure)
+    })
+  ,
   'DESCRIPTOR' : _STREAMPARAMS,
   '__module__' : 'bosdyn.api.spot_cam.streamquality_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.spot_cam.StreamParams)
   })
 _sym_db.RegisterMessage(StreamParams)
 _sym_db.RegisterMessage(StreamParams.AwbMode)
+_sym_db.RegisterMessage(StreamParams.AutoExposure)
+_sym_db.RegisterMessage(StreamParams.SyncAutoExposure)
+_sym_db.RegisterMessage(StreamParams.ManualExposure)
 
 GetStreamParamsRequest = _reflection.GeneratedProtocolMessageType('GetStreamParamsRequest', (_message.Message,), {
   'DESCRIPTOR' : _GETSTREAMPARAMSREQUEST,
   '__module__' : 'bosdyn.api.spot_cam.streamquality_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.spot_cam.GetStreamParamsRequest)
   })
 _sym_db.RegisterMessage(GetStreamParamsRequest)
@@ -88,26 +116,32 @@
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'B\022StreamQualityProto'
   _STREAMPARAMS_AWBMODEENUM.values_by_name["DARK"]._options = None
   _STREAMPARAMS_AWBMODEENUM.values_by_name["DARK"]._serialized_options = b'\010\001'
-  _STREAMPARAMS._serialized_start=122
-  _STREAMPARAMS._serialized_end=576
-  _STREAMPARAMS_AWBMODE._serialized_start=350
-  _STREAMPARAMS_AWBMODE._serialized_end=419
-  _STREAMPARAMS_AWBMODEENUM._serialized_start=422
-  _STREAMPARAMS_AWBMODEENUM._serialized_end=576
-  _GETSTREAMPARAMSREQUEST._serialized_start=578
-  _GETSTREAMPARAMSREQUEST._serialized_end=645
-  _GETSTREAMPARAMSRESPONSE._serialized_start=647
-  _GETSTREAMPARAMSRESPONSE._serialized_end=767
-  _SETSTREAMPARAMSREQUEST._serialized_start=769
-  _SETSTREAMPARAMSREQUEST._serialized_end=887
-  _SETSTREAMPARAMSRESPONSE._serialized_start=889
-  _SETSTREAMPARAMSRESPONSE._serialized_end=1009
-  _ENABLECONGESTIONCONTROLREQUEST._serialized_start=1011
-  _ENABLECONGESTIONCONTROLREQUEST._serialized_end=1121
-  _ENABLECONGESTIONCONTROLRESPONSE._serialized_start=1123
-  _ENABLECONGESTIONCONTROLRESPONSE._serialized_end=1200
+  _STREAMPARAMS._serialized_start=154
+  _STREAMPARAMS._serialized_end=1045
+  _STREAMPARAMS_AWBMODE._serialized_start=609
+  _STREAMPARAMS_AWBMODE._serialized_end=678
+  _STREAMPARAMS_AUTOEXPOSURE._serialized_start=680
+  _STREAMPARAMS_AUTOEXPOSURE._serialized_end=694
+  _STREAMPARAMS_SYNCAUTOEXPOSURE._serialized_start=696
+  _STREAMPARAMS_SYNCAUTOEXPOSURE._serialized_end=770
+  _STREAMPARAMS_MANUALEXPOSURE._serialized_start=772
+  _STREAMPARAMS_MANUALEXPOSURE._serialized_end=876
+  _STREAMPARAMS_AWBMODEENUM._serialized_start=879
+  _STREAMPARAMS_AWBMODEENUM._serialized_end=1033
+  _GETSTREAMPARAMSREQUEST._serialized_start=1047
+  _GETSTREAMPARAMSREQUEST._serialized_end=1114
+  _GETSTREAMPARAMSRESPONSE._serialized_start=1116
+  _GETSTREAMPARAMSRESPONSE._serialized_end=1236
+  _SETSTREAMPARAMSREQUEST._serialized_start=1238
+  _SETSTREAMPARAMSREQUEST._serialized_end=1356
+  _SETSTREAMPARAMSRESPONSE._serialized_start=1358
+  _SETSTREAMPARAMSRESPONSE._serialized_end=1478
+  _ENABLECONGESTIONCONTROLREQUEST._serialized_start=1480
+  _ENABLECONGESTIONCONTROLREQUEST._serialized_end=1590
+  _ENABLECONGESTIONCONTROLRESPONSE._serialized_start=1592
+  _ENABLECONGESTIONCONTROLRESPONSE._serialized_end=1669
 # @@protoc_insertion_point(module_scope)
```

## Comparing `bosdyn_api-3.2.3.dist-info/METADATA` & `bosdyn_api-3.3.0.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: bosdyn-api
-Version: 3.2.3
+Version: 3.3.0
 Summary: Boston Dynamics API definition of protobuf messages
 Home-page: https://dev.bostondynamics.com/
 Author: Boston Dynamics
 Author-email: support@bostondynamics.com
-License: UNKNOWN
 Project-URL: Documentation, https://dev.bostondynamics.com/
 Project-URL: Source, https://github.com/boston-dynamics/spot-sdk/
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Requires-Dist: protobuf (>=3.6.1)
+Requires-Dist: protobuf (>=3.19.4)
 
 <!--
-Copyright (c) 2022 Boston Dynamics, Inc.  All rights reserved.
+Copyright (c) 2023 Boston Dynamics, Inc.  All rights reserved.
 
 Downloading, reproducing, distributing or otherwise using the SDK Software
 is subject to the terms and conditions of the Boston Dynamics Software
 Development Kit License (20191101-BDSDK-SL).
 -->
 
 # bosdyn-api
@@ -30,9 +32,7 @@
 </p>
 
 The bosdyn-api wheel contains the Python implementation for the Protobuf definitions in the Boston 
 Dynamics Spot API. The message and service types defined in this wheel are used by the clients in 
 [bosdyn-client](https://pypi.org/project/bosdyn-client/) and 
 [bosdyn-mission](https://pypi.org/project/bosdyn-mission/) wheels to communicate with the services 
 running on the Spot robots.
-
-
```

## Comparing `bosdyn_api-3.2.3.dist-info/RECORD` & `bosdyn_api-3.3.0.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 bosdyn/__init__.py,sha256=h-QyvMVzDNpT3jyVskcSbUVFXxGCRxieFPrvTveZG9k,64
-bosdyn/api/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+bosdyn/api/__init__.py,sha256=h-QyvMVzDNpT3jyVskcSbUVFXxGCRxieFPrvTveZG9k,64
 bosdyn/api/alerts_pb2.py,sha256=scyMwCNzElHIsclHF5aWl-m1vR8KVSQVgB2Q990Zp-8,2009
 bosdyn/api/alerts_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
-bosdyn/api/arm_command_pb2.py,sha256=hkZ4t_g4LRvBKLfNTCy131fmU3qWhl5wPyIMbUBfPmc,29332
+bosdyn/api/arm_command_pb2.py,sha256=2wSYmOKQu8xCqvxPzgQCBsvDpd1jcA3NQqffDy9V5jc,30436
 bosdyn/api/arm_command_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/arm_surface_contact_pb2.py,sha256=OU6l9hRM1LFpUhG3tnY14yZgKhcOWx8S7_mRcDcZx9o,5850
 bosdyn/api/arm_surface_contact_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/arm_surface_contact_service_pb2.py,sha256=lNn9k8Pro_rHQP7YXWxERH_Hg0Pvjlp6KGZP_9nzIgQ,3050
 bosdyn/api/arm_surface_contact_service_pb2_grpc.py,sha256=KiyS-8v1VorObyZUAkrpnpIeyj1lF4h3yae029JZLEk,2967
 bosdyn/api/auth_pb2.py,sha256=LlwbdAGeJgFKwtSu9j4eFyNXpRsg-nhWeNkIA2XQUbU,3056
 bosdyn/api/auth_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/auth_service_pb2.py,sha256=FPcGPstvJh_5gtYCFpXesSM5nZkuBzvc9SXoTIxPwo0,1216
 bosdyn/api/auth_service_pb2_grpc.py,sha256=d_LvtDEhUzva2a9W9JUpw01QZkTcGdrQstFuJdyN8Gk,3110
-bosdyn/api/basic_command_pb2.py,sha256=mKDSChwvAgND8EYQj4ExZzLboLHMCJW8l79G4Plqlqw,32794
+bosdyn/api/basic_command_pb2.py,sha256=JkfBuayZ6qxPnH-Q8_EY87BQG8rQH6cISLDuTxONOG4,33736
 bosdyn/api/basic_command_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/bddf_pb2.py,sha256=kt9Mw1i5ztbNLURqG5SPT4lx2BK3E5qw1oOq8kyNAR4,14051
 bosdyn/api/bddf_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
-bosdyn/api/data_acquisition_pb2.py,sha256=1yeNqdTXCvCJSIcJnXYjrX4KX55Clsscmt4JdmrYZJ8,23347
+bosdyn/api/data_acquisition_pb2.py,sha256=k5lsR9_vd-8exDTsP7WQkLG8zJTCJcEEyZQfSyTkXks,24749
 bosdyn/api/data_acquisition_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/data_acquisition_plugin_service_pb2.py,sha256=WQx1-v0xunQXU3xA-gt-3a7C9nkLn_2eHpsyqpUNRkg,1714
-bosdyn/api/data_acquisition_plugin_service_pb2_grpc.py,sha256=RgoRaKZuntnsM4XvXlg17v4Ur4ycg0i9gZ4Sqi7_XEE,8973
+bosdyn/api/data_acquisition_plugin_service_pb2_grpc.py,sha256=H_oOVTkJC84QMk9fL9cZJ8CybKi5pbo8D4CwYlvK6CI,9015
 bosdyn/api/data_acquisition_service_pb2.py,sha256=Vj8hSpxMk6k-8nKq00EbT6X1E4LkcRjEcJSChsWO2Hc,1663
-bosdyn/api/data_acquisition_service_pb2_grpc.py,sha256=RTD9OhZ9kf8X4BIblQjZKypc7eHywPqwJ9WnY2mhNE4,8608
-bosdyn/api/data_acquisition_store_pb2.py,sha256=qvOy3bbNebM7iVq3SONUZONGGFpGtBRntglX6hG3Xoo,15792
+bosdyn/api/data_acquisition_service_pb2_grpc.py,sha256=A8TnVNa1zUMLGctKy83ACEC2aPfMA6Mvie7xB5m7h0o,8621
+bosdyn/api/data_acquisition_store_pb2.py,sha256=CdAdcgTmfc2C3tSngZrltmBdZXA9lOpyYynOuqw5KHM,15920
 bosdyn/api/data_acquisition_store_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/data_acquisition_store_service_pb2.py,sha256=mnRwTy6dyivFwwWRuVrCjRpVPAqnLXmL58J1cOIZ0BI,2249
-bosdyn/api/data_acquisition_store_service_pb2_grpc.py,sha256=KC6phfjFteAEk8a2o3yIEdI4x5kxcfFh0XCMqUdsGJE,19213
+bosdyn/api/data_acquisition_store_service_pb2_grpc.py,sha256=9tTJnUlV5l0OHexLbCGzsRCOOPYPD348qKmT67qr_UQ,19213
 bosdyn/api/data_buffer_pb2.py,sha256=l5WGDO36T7MhyMO0tIH9ZqhPGl72YN0GEu3aWioKSyU,22413
 bosdyn/api/data_buffer_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/data_buffer_service_pb2.py,sha256=Buv9aDGgSjz-6vdHjgQHiEnRVxIbfmDgQKmVtBgnNQ4,1916
 bosdyn/api/data_buffer_service_pb2_grpc.py,sha256=Zue_tm_-gWVbPxhRI5PkXHfToY4sQ8_Eay7qkOpl6ZQ,11709
 bosdyn/api/data_chunk_pb2.py,sha256=MRzwq6oSkIcNV88RDBPpHcTo28PWLK2njbhA9Ge2X_0,1349
 bosdyn/api/data_chunk_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/data_index_pb2.py,sha256=tCwQFgI8tn-wzeahdheTYo12PxFWdAvLOcgH6Lm3X60,18846
 bosdyn/api/data_index_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/data_service_pb2.py,sha256=etT3mM0EMXipskmt3BobSbpP0GziuqzxSnrtr2GGATs,1716
 bosdyn/api/data_service_pb2_grpc.py,sha256=-RlbozJp0hgcvdavtRMpNwtUj8kPNhLQQTt0zl-Bx5U,9683
-bosdyn/api/directory_pb2.py,sha256=cEaPcWaZuw9qLHYQy_Eqq4qXnCxThp2BlKC2zfa3nXs,5585
+bosdyn/api/directory_pb2.py,sha256=CiZd8c_IMaqXBZaSojqjbifhdRBv3ZzLxVcriTMgAA0,5551
 bosdyn/api/directory_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/directory_registration_pb2.py,sha256=MaA9T0ZMzj2vFytOmZ7VhfchQ9r-kZM3PWLaY8m4wE4,6451
 bosdyn/api/directory_registration_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/directory_registration_service_pb2.py,sha256=7jEEa3IHyI6Fu_ZKsx9VcJoBxdPe_a0xeD3CM1cbttA,1639
 bosdyn/api/directory_registration_service_pb2_grpc.py,sha256=rlnLTiEE-sRLzCaeMzAaS6pCSuJH7p9p9WvRZM3kJek,7495
 bosdyn/api/directory_service_pb2.py,sha256=2hr8irkC1ifPk_Rs1aoGP2y9LxD6twl9UrLm_XgRFP4,1393
 bosdyn/api/directory_service_pb2_grpc.py,sha256=_uA-qjNOjaMul2b9I1-SaHEyv0aEjcWdOF0z3NuF8yw,4568
@@ -50,198 +50,222 @@
 bosdyn/api/estop_service_pb2_grpc.py,sha256=Fu668JfvL3cHqRJfta2gcGyK9fA5YWZhiOVhOuwP22s,12256
 bosdyn/api/fault_service_pb2.py,sha256=sgk0JYOBzA4hCCFH7ZZU3fF91LoPuTFyi4up0N57c-Y,1408
 bosdyn/api/fault_service_pb2_grpc.py,sha256=xUYvx64CnpM-SIOqnoHyl6Jv1xyTMJPEz_4uyhL_XUk,4661
 bosdyn/api/full_body_command_pb2.py,sha256=Brha758-9V45OB1-xJa553IbKv8kM-W_qyPmA9aVOj8,4458
 bosdyn/api/full_body_command_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/geometry_pb2.py,sha256=_I0IAIwwnHlbtYbASwkjfhZEAAOg0GCZy0NWCvoun04,21667
 bosdyn/api/geometry_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
-bosdyn/api/gripper_camera_param_pb2.py,sha256=O8SiDBhe98KUTuRual9EcoCZgr_f4f88APur3xvhU-0,8424
+bosdyn/api/gripper_camera_param_pb2.py,sha256=HL1KcvBZA9B2F0CxeLh5PV4rjKPmwqa5M675D27aO2w,10402
 bosdyn/api/gripper_camera_param_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/gripper_camera_param_service_pb2.py,sha256=9OHgRLOEq1SvSJdKhm5VraI0afKxvdtd8qnR3u9E-eo,1503
 bosdyn/api/gripper_camera_param_service_pb2_grpc.py,sha256=wYioHn4N9QFIkqDAoPGj2DEG9lCbuSvwzGxlPZcmQP4,4677
 bosdyn/api/gripper_command_pb2.py,sha256=GgyOW6ntmjroJwTpKBvkJAWMvnyBcwBp-NlmuxDV9-g,5623
 bosdyn/api/gripper_command_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/header_pb2.py,sha256=jVuYfo6q88xL9wzCCJV6uy1G1G668tTDtJ6DMjTUtnY,3507
 bosdyn/api/header_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
-bosdyn/api/image_pb2.py,sha256=IiAL-2FG496y0rwgN1PHZYMWQStTcuVlePTHhki1Nvo,11451
+bosdyn/api/image_geometry_pb2.py,sha256=STNL1TILWaaJf8FSJsRI5DNoU8VHPMKIhJG2A41bd4c,2000
+bosdyn/api/image_geometry_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
+bosdyn/api/image_pb2.py,sha256=HjtkSGEpW1ehTKxSNzgD7X3hBosVUsMsyQDIvU2AB0A,12659
 bosdyn/api/image_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/image_service_pb2.py,sha256=TdieCviQfGcygUQYefywRFuGv4410CHvsz94CqaOuAs,1334
 bosdyn/api/image_service_pb2_grpc.py,sha256=Dz9TvhWsi05IPDTIgee_WFyYj-jsWNmZ_65zBrnQrA0,5046
 bosdyn/api/ir_enable_disable_pb2.py,sha256=H2haecheq16P4pG5copxoUShdr6lKeaiRBSKPAO8vng,2621
 bosdyn/api/ir_enable_disable_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/ir_enable_disable_service_pb2.py,sha256=Q6F0A6FfGBLGvgGtjMWodzArF1ZBwpyAHrCKTTczW00,1351
 bosdyn/api/ir_enable_disable_service_pb2_grpc.py,sha256=oAa3ue1bTTDm7sKAwDaMAQYm13O-3q96FGkGLCX0Qz0,2840
-bosdyn/api/lease_pb2.py,sha256=MIgfQA2bGIAyHaDfIZCmSY_2t9dbCeWQfddHiMA91sI,12499
+bosdyn/api/lease_pb2.py,sha256=qOkseoUEw6grLMdX1wFh4GEJjGPdh7qqIE5zFKuO1WE,12697
 bosdyn/api/lease_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/lease_service_pb2.py,sha256=x22AL0M5bGomS0YU35bxdzomQxyb2O-Kn9Z3zman8SM,1609
 bosdyn/api/lease_service_pb2_grpc.py,sha256=4f_ftWNgMfALtpX_-P3ltjexlsJurA95WwHNgHiGTuo,10495
 bosdyn/api/license_pb2.py,sha256=8WCZgBRA0djm23mSGD8Brkr446qAPS_Ia42P1OZITCU,5939
 bosdyn/api/license_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/license_service_pb2.py,sha256=z1Ax1AUiCm2vmn7s0BG7bA5bkVvvF41YITUFPQYUY0Q,1371
 bosdyn/api/license_service_pb2_grpc.py,sha256=_FPazAYIyHUZRurvR8k3J7CXHHfrIzLdJS-WFvIshdg,4677
 bosdyn/api/local_grid_pb2.py,sha256=XWcL7LDRuALTofr4L6Zd5PYHSi_n2G--jhBluaP5UxA,8596
 bosdyn/api/local_grid_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/local_grid_service_pb2.py,sha256=7MefLCt4msYS9ENtGOHkmaA8TLFYlfdO0TxJdlFW8qA,1395
 bosdyn/api/local_grid_service_pb2_grpc.py,sha256=9gMQj1pEA3ce1c7Zr6KxoGAsDqvdIrUsEBywZ1g24QI,5131
-bosdyn/api/log_annotation_pb2.py,sha256=aRhqXy0tCManCXhS4Pp2OruSxkgCkdMzBLOqlotOxeQ,6174
+bosdyn/api/log_annotation_pb2.py,sha256=8eQtnyV44rwL3La82FpuBLQRh770PFHxehwYOZHWFLY,6866
 bosdyn/api/log_annotation_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/log_annotation_service_pb2.py,sha256=4kciz907B9VX8T7WA3v1rSoE6r8HUgMjBYMrD94rQks,1337
-bosdyn/api/log_annotation_service_pb2_grpc.py,sha256=4UElHJOlogBXGnEgvLCMAzrKMsGCLNRWnk6_q_tXYU4,3704
+bosdyn/api/log_annotation_service_pb2_grpc.py,sha256=9A8wwzwawMupjAcPOF2Ow1O_qJulBuzFFUAX4k5-yuI,3497
 bosdyn/api/manipulation_api_pb2.py,sha256=11CzQIA7Du-Sh0zOYOz997lBhABLFfXcAspWP375E78,20772
 bosdyn/api/manipulation_api_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/manipulation_api_service_pb2.py,sha256=GrftCKcXQD-7fLN2YNcHUfNA0aA9_YmE80Mzgt73Vic,1485
 bosdyn/api/manipulation_api_service_pb2_grpc.py,sha256=Ga-p9YtvwS5kC95I8p8oq94_uPmDCU_1xLvU48Nbycw,6493
 bosdyn/api/mobility_command_pb2.py,sha256=qTkdahm6dEJcDvKhDSlmyMMU-dmGtd_Ar8HoNc0Djz0,4165
 bosdyn/api/mobility_command_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
-bosdyn/api/network_compute_bridge_pb2.py,sha256=LNbh5p328CncYOBYcjYAngRJEaom1YQyzDvTTmvEpaw,11849
+bosdyn/api/network_compute_bridge_pb2.py,sha256=xjAG-jecHRVTJEqSaY-2V-AQoV9yAjohZrP0TYQ-axo,22449
 bosdyn/api/network_compute_bridge_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
-bosdyn/api/network_compute_bridge_service_pb2.py,sha256=XttbNbtmlGi4CDDp-Avt9HJitBNw01HQdMXvdnBdOjA,1850
-bosdyn/api/network_compute_bridge_service_pb2_grpc.py,sha256=JKWqofWtUl5EFlNl8A78cvkQMPHuJKYKM1urhfbeE4c,9782
+bosdyn/api/network_compute_bridge_service_pb2.py,sha256=doOTBRBglZMqWFvF7XLJzJQENPZvyewi8EBjmVtsJgo,2148
+bosdyn/api/network_compute_bridge_service_pb2_grpc.py,sha256=-5ID_Red35zMLMb7YnBZO5b3vQtHMMzwLMmzMRU1_jw,11592
 bosdyn/api/network_stats_pb2.py,sha256=RJN57sB0ml1hb8HC5r0KrFDgUVIk81er70F4uE4zJ18,3691
 bosdyn/api/network_stats_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/parameter_pb2.py,sha256=rlJGGwuuj6laQLrMM7MBHAEXDDsnEtqwdu2UkZ88V6o,2030
 bosdyn/api/parameter_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/payload_estimation_pb2.py,sha256=Fg3sQdfY-9o9lUcaJXCLiCP0nWBYwWdIKkUUHXxsPlc,3914
 bosdyn/api/payload_estimation_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
-bosdyn/api/payload_pb2.py,sha256=msGzwwo93nCTZ9suWacGBX-tj-NofPzPe1_7RHUJQMU,7114
+bosdyn/api/payload_pb2.py,sha256=1s_9MrFPBnQAnefaYezZtf8XxFQU-vv76MYn7XcWQJI,7249
 bosdyn/api/payload_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/payload_registration_pb2.py,sha256=aobon3wDXtBnuHFixXtEudsIknmcFdAJ5J_DB4KMybA,10889
 bosdyn/api/payload_registration_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/payload_registration_service_pb2.py,sha256=RWCJ8xCUcEmvTuDkYrDur2besDp31BgyLlLlNZKbBjU,1749
 bosdyn/api/payload_registration_service_pb2_grpc.py,sha256=lIKoV7uQ9HwNesgotr9jhigbcxhyZjgqjXHejAorOfI,8567
 bosdyn/api/payload_service_pb2.py,sha256=_dwC7x3Ldbhd7V-VAah4653UpO2zrQeX7rmbgoekQsI,1243
 bosdyn/api/payload_service_pb2_grpc.py,sha256=J_TsaOuuDEruLoQPMSgUXe4xwPVZE6eUIbVNoZ-5OqA,2716
 bosdyn/api/point_cloud_pb2.py,sha256=VcWEfDUD4Y4nrSLeSZReNUDMBz42juWuNrNx3Cuc298,8374
 bosdyn/api/point_cloud_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/point_cloud_service_pb2.py,sha256=GywkW0BLSKyl0c8mabrQS9SS41vTZuxeejeA16f_buU,1416
 bosdyn/api/point_cloud_service_pb2_grpc.py,sha256=T--EC_pAd8lNvaVNDCOK8LcivIJdjQpSOpM3Hb0ulyc,5382
-bosdyn/api/power_pb2.py,sha256=gCpSyOSxxt8u36V5nzUi71s9S7c1WBX3FToQ4ztKxKE,11191
+bosdyn/api/power_pb2.py,sha256=S57kgL559YjkWUKKzUF8f0P5Amv7jbVjReo2aV1AmIA,11273
 bosdyn/api/power_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/power_service_pb2.py,sha256=9cExzyJsb0oUBNvvCyMWrvhmHaaZ9UYcObYuSC0LUrw,1616
 bosdyn/api/power_service_pb2_grpc.py,sha256=HSxNeCk0TlPONmVD7Pv4hKEbiBLwd3_Kry391O4BepU,8130
 bosdyn/api/ray_cast_pb2.py,sha256=--hOsoXOOZsZrEtn55rmb4oZfCL4x_3FkTMhJNJEMyI,4105
 bosdyn/api/ray_cast_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/ray_cast_service_pb2.py,sha256=YJyg_ylrNLQmqvNjdJjttJJzHNusoVE2U2nBfjAOkC4,1237
 bosdyn/api/ray_cast_service_pb2_grpc.py,sha256=9jCKT8sJpeaU6q3Ii8KbWh5UtlxEOzpGhGz0AxnRPig,2683
-bosdyn/api/robot_command_pb2.py,sha256=TWhJem1C0IWzRTBdkg73Dbys1hBC4UvKgMawIml59TQ,10116
+bosdyn/api/robot_command_pb2.py,sha256=nYGru1WJUzM-1s2J3FonKQQeZWmoKmdIjcwO5yfZehQ,10551
 bosdyn/api/robot_command_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/robot_command_service_pb2.py,sha256=JivGWBCZlySaj9pFuA1TrrmnhdCCDT4K04mokXdLKRs,1566
 bosdyn/api/robot_command_service_pb2_grpc.py,sha256=x_kI-z5llmwlCs1BD8e-0SpKRuuF6pNubdpUIJupfco,6817
 bosdyn/api/robot_id_pb2.py,sha256=Q-_gEyRIqUU6FyZ-WedatNRDFc7mbNEyFyxPQBSNj8g,4643
 bosdyn/api/robot_id_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/robot_id_service_pb2.py,sha256=upNdIQ3ozgZcMNN37C0grPITvacPV5MQrM2y3xKp0o8,1235
 bosdyn/api/robot_id_service_pb2_grpc.py,sha256=oM8I0UwutYj8STO5craTJmnYBCnmPFR553uOc-OeFLQ,3171
-bosdyn/api/robot_state_pb2.py,sha256=wJpa8ST75Swrqz7rlr41JdNUZWYVPedphrgL4CmLJa8,34808
+bosdyn/api/robot_state_pb2.py,sha256=ZB85SgvKPPqDsOd-jKaeWxKE_QOyUCWAH_zRDTcrHNk,34922
 bosdyn/api/robot_state_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/robot_state_service_pb2.py,sha256=rKwBE0bU5TCiTVfxaBNXxYgAhrHvw4Z5P-Ee264sohc,1662
 bosdyn/api/robot_state_service_pb2_grpc.py,sha256=QDgM0EVk2oDHxAU0lW62lTItJWc37aerKYvEsohkQsk,8496
+bosdyn/api/service_customization_pb2.py,sha256=APSNl8xB5RBhn0m7tHxdPl-gmxhBSZZPQCZtGqfe1yU,20717
+bosdyn/api/service_customization_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/service_fault_pb2.py,sha256=VWZSAHdy2fYAIEinS66CiMkzemqzv5qCskG93w24NpY,6687
 bosdyn/api/service_fault_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/sparse_features_pb2.py,sha256=mguZcwxcWV9qW8IhaDG7qGPq5wCumWQNNNb6dIZLGeI,3705
 bosdyn/api/sparse_features_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
-bosdyn/api/stairs_pb2.py,sha256=yIeDI5OEwZDBT3suUUh-jSKcEkh3_vA8H5urcRYvelI,3710
+bosdyn/api/stairs_pb2.py,sha256=-pN-2hUdBuw1vSRem0AHbo2naFFKykNNl3KROhc_HRE,8175
 bosdyn/api/stairs_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/synchronized_command_pb2.py,sha256=KG0-KWNM4yu1PORcYf7R-KmHWq6tMtSrhjqprzXy7bM,3460
 bosdyn/api/synchronized_command_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/time_range_pb2.py,sha256=1fX3jBhbG-hNsN-wQcQn7rID6KRn79Y_43PmuvG2sPM,1520
 bosdyn/api/time_range_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/time_sync_pb2.py,sha256=Fpe7KoNWoGzxy4pEcaBm0cgHi4VPCF9iZRku6jtq3t4,5177
 bosdyn/api/time_sync_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/time_sync_service_pb2.py,sha256=oMO-yoP9UTkutbwL-XqPUMOfJ7w98uBkTrRawOuFje0,1263
 bosdyn/api/time_sync_service_pb2_grpc.py,sha256=Cz8hYPDfnjews63uTiNlqiIhrWbAcoWGlCN2bL_vK6k,4473
 bosdyn/api/trajectory_pb2.py,sha256=w4Z2e0DvpxngEDgagvnT1rnOuMNYWcsvA4dlwMBtsdg,9596
 bosdyn/api/trajectory_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
-bosdyn/api/world_object_pb2.py,sha256=54sJ64M8-PF7nRh8IuvAFs7QsKND88UKi_7HGiGqErI,18773
+bosdyn/api/units_pb2.py,sha256=h7WQ6hkRzxup4OD9M6YWq9sBlnBUii46nkmkVD_Nv9w,2467
+bosdyn/api/units_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
+bosdyn/api/world_object_pb2.py,sha256=f9gfNaDU-MZxdKVD_MApT6LsvjG6XjuTkcplRf9SfFo,20832
 bosdyn/api/world_object_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/world_object_service_pb2.py,sha256=xTujGeWYS6k95uC4Qssb0zsAM__s-NgZ7zd1gayOLAY,1430
-bosdyn/api/world_object_service_pb2_grpc.py,sha256=At_YhVmF8jqcy8qdb-JiGt-vacfOXOEiqd6VZW9rt04,4752
-bosdyn/api/auto_return/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-bosdyn/api/auto_return/auto_return_pb2.py,sha256=v-0qCuxKQ3UXvyfuWRt-mRiyt6sLmL7uuSQsvBJF6Gc,6273
+bosdyn/api/world_object_service_pb2_grpc.py,sha256=JzB__BvmcuWbYmwjFNfquCcJqMtP3QT0duscsniWauI,4764
+bosdyn/api/auto_return/__init__.py,sha256=h-QyvMVzDNpT3jyVskcSbUVFXxGCRxieFPrvTveZG9k,64
+bosdyn/api/auto_return/auto_return_pb2.py,sha256=9hvJamSAneD6GsD9fuC-tyEjTgXXBbDtGfvk9R1Xj9Y,6870
 bosdyn/api/auto_return/auto_return_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/auto_return/auto_return_service_pb2.py,sha256=IB2RFJ06jz2PNURHmJ7yLTJM5AL8QLeh8Zyy_NpGgZA,1607
 bosdyn/api/auto_return/auto_return_service_pb2_grpc.py,sha256=lxZGKu3y1wfSWv169w2SS10oTmpJQUIxuSGb_FwwoVg,6398
-bosdyn/api/autowalk/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+bosdyn/api/autowalk/__init__.py,sha256=h-QyvMVzDNpT3jyVskcSbUVFXxGCRxieFPrvTveZG9k,64
 bosdyn/api/autowalk/autowalk_pb2.py,sha256=P1YEdFrN8DjtgtCwAr05k3AtDvfgWQMSPrgxHCjG6dY,9934
 bosdyn/api/autowalk/autowalk_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/autowalk/autowalk_service_pb2.py,sha256=M7mNPIBsRjLVDMdYhzSmJbbksJ11gIyj9b2R8AHXXHI,1411
 bosdyn/api/autowalk/autowalk_service_pb2_grpc.py,sha256=vpEaNUACkaQ8sKITCx93lq5SBy1DcybqY5yNiO-Cy6k,4716
-bosdyn/api/autowalk/walks_pb2.py,sha256=rtiw3wsOoHy8HiFaRPiiFDjiSgQw5bDyQHzZJ4uoqOc,25377
+bosdyn/api/autowalk/walks_pb2.py,sha256=eRVmdrV_w5rq-eKEcIuzyaA0aHpcGUW8gZFGk6Xz4hE,28007
 bosdyn/api/autowalk/walks_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
-bosdyn/api/docking/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-bosdyn/api/docking/docking_pb2.py,sha256=4y7Box5m4Wzly_2W2UvEO7XCEeaoq7PHLcDwc4udMbo,12591
+bosdyn/api/docking/__init__.py,sha256=h-QyvMVzDNpT3jyVskcSbUVFXxGCRxieFPrvTveZG9k,64
+bosdyn/api/docking/docking_pb2.py,sha256=bsA8CLYEBPT0lyTWskEYQHBujcqtm4lh8w7qtfMtvl0,12713
 bosdyn/api/docking/docking_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/docking/docking_service_pb2.py,sha256=X7gRfNQUNNzxfT01pkh34R2kaA38qafTEax8nmWewxI,1747
 bosdyn/api/docking/docking_service_pb2_grpc.py,sha256=K7JPkeuwdlxSOnyeIOO2OJqqcSreZc37gRExwyOtzwQ,8632
-bosdyn/api/graph_nav/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-bosdyn/api/graph_nav/area_callback_pb2.py,sha256=phQkHc_2kKFenLzRd7RoGmvybH2t11W2vyTbznquJ7I,16817
+bosdyn/api/graph_nav/__init__.py,sha256=h-QyvMVzDNpT3jyVskcSbUVFXxGCRxieFPrvTveZG9k,64
+bosdyn/api/graph_nav/area_callback_data_pb2.py,sha256=_sttM5fhTYpgxlB0QEEkubYUzgkTp3wLIwLBb-IfP6U,1812
+bosdyn/api/graph_nav/area_callback_data_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
+bosdyn/api/graph_nav/area_callback_pb2.py,sha256=Rq3x1mqlD4jaTavweRtjhtXHcPmc1a6EpKmNrYEcZxY,18870
 bosdyn/api/graph_nav/area_callback_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/graph_nav/area_callback_service_pb2.py,sha256=tkJnFg33-oIXG-qYzrxcoN806NM5KXml6uUQws_vrkQ,1954
 bosdyn/api/graph_nav/area_callback_service_pb2_grpc.py,sha256=eOA8eJmBdDvnMkxJJR-0U-HEbpntoE6_K7fHi3zy7nE,11049
-bosdyn/api/graph_nav/graph_nav_pb2.py,sha256=wmLmheru97daXClJXf0wsL_TnsqKdQg2fJT3t3NIUGM,49710
+bosdyn/api/graph_nav/graph_nav_pb2.py,sha256=J7NBPGuKlK_AhNzLPcR_qhLNOY-6UG3ZPRJWJg8Y7L8,54376
 bosdyn/api/graph_nav/graph_nav_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/graph_nav/graph_nav_service_pb2.py,sha256=ub0CCmwcjbM2QiV0TpzgfnE-fJQ-XBx7N65JxnrlDHM,3186
 bosdyn/api/graph_nav/graph_nav_service_pb2_grpc.py,sha256=0jS9-gFx-LLHwo4tvq-mbKDOMoyOMePZxpCOTmsw-c4,27993
-bosdyn/api/graph_nav/map_pb2.py,sha256=79sddV8hYg6u4I54D0dTYu7vLYmTwiHoj_A_rg9xcEs,23190
+bosdyn/api/graph_nav/map_pb2.py,sha256=5BelAx6yBBk_W76ZezskKzOSD40FoQRfX3IoF_jKvR4,25984
 bosdyn/api/graph_nav/map_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
-bosdyn/api/graph_nav/map_processing_pb2.py,sha256=s4Z04f2McynUCR_O2Az-qJlcPGmkKw_VFaUXjkyZMLQ,20037
+bosdyn/api/graph_nav/map_processing_pb2.py,sha256=kBTTKTVLi5TFpqe88kh72LCFzXdfM-SIuPrwN4j7AtQ,20274
 bosdyn/api/graph_nav/map_processing_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/graph_nav/map_processing_service_pb2.py,sha256=UtBitKJkqNV7g8E6sMcQSNImThcvv0V2kY_d7EEa_tk,1566
 bosdyn/api/graph_nav/map_processing_service_pb2_grpc.py,sha256=J8XAYkb7N92TKDi-kkC6sDfI-ZhH25Aan2LhX-d0MSI,5125
 bosdyn/api/graph_nav/nav_pb2.py,sha256=p0Y9Pb0JTCUJcw5NVYfUA0YGHmqc4Hl2ry0_k9Uh6jk,2440
 bosdyn/api/graph_nav/nav_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
-bosdyn/api/graph_nav/recording_pb2.py,sha256=i-oKKlcUmr3NQHDKY6YDp9lOu4rmiF4rWf4ol5Q-mH8,15825
+bosdyn/api/graph_nav/recording_pb2.py,sha256=XQgM2XY_queBHuNP-N8T6Yw-HVu2EmpO-UZpH7gJk7k,16665
 bosdyn/api/graph_nav/recording_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/graph_nav/recording_service_pb2.py,sha256=Rqal3rTSYQpqxoohafoX9hk9sdhMw8N98w22-nV5Syg,2070
 bosdyn/api/graph_nav/recording_service_pb2_grpc.py,sha256=LErRJDHOsOebjRhrJyT5LBPe7bjiYggln-egX6Jt7IE,15653
-bosdyn/api/mission/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-bosdyn/api/mission/mission_pb2.py,sha256=1TRYfXwVgVqRxS2EFjDwNN7JBgua4JptBSd4fdkVRr4,23899
+bosdyn/api/keepalive/__init__.py,sha256=h-QyvMVzDNpT3jyVskcSbUVFXxGCRxieFPrvTveZG9k,64
+bosdyn/api/keepalive/keepalive_pb2.py,sha256=T2YZFcsaYB6D-REN_yloP2JMQwrDcVBz3eI8-HV5WW4,12506
+bosdyn/api/keepalive/keepalive_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
+bosdyn/api/keepalive/keepalive_service_pb2.py,sha256=FZ-AnIE_yfyo531yu3T22wo3-G6n0Tnu9g1sfYgWo4c,1574
+bosdyn/api/keepalive/keepalive_service_pb2_grpc.py,sha256=tcqElPFPrALivnjbESdQw3dIYD9PpbORbik7IPFoGJY,7484
+bosdyn/api/log_status/__init__.py,sha256=h-QyvMVzDNpT3jyVskcSbUVFXxGCRxieFPrvTveZG9k,64
+bosdyn/api/log_status/log_status_pb2.py,sha256=lHWf7urS4yt5aTbrEj-Fj4e2LXQEvEYjolLkLo4QU6M,13805
+bosdyn/api/log_status/log_status_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
+bosdyn/api/log_status/log_status_service_pb2.py,sha256=QafVI5hznzU_s0sjSBRmG8n1o8nSwJ9TfdmcPHdPEDQ,1934
+bosdyn/api/log_status/log_status_service_pb2_grpc.py,sha256=irSB5Tjix1VMArhm7-e1MUx6e--OaDg6glxgzejZhqs,13599
+bosdyn/api/mission/__init__.py,sha256=h-QyvMVzDNpT3jyVskcSbUVFXxGCRxieFPrvTveZG9k,64
+bosdyn/api/mission/mission_pb2.py,sha256=EC7XmSBOGdoVsKAw5zU4__N7lG8AcTrzVIFKxy7ZApA,24846
 bosdyn/api/mission/mission_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
-bosdyn/api/mission/mission_service_pb2.py,sha256=YyMMUcYN_N5eJ7GVnQPm75GZ773SpbAy2bEX29vzYvg,2466
-bosdyn/api/mission/mission_service_pb2_grpc.py,sha256=2H1aweTYqib4mYXQOxFHQ5X5rFu3RHyyMb8x8lCVp7Q,19058
-bosdyn/api/mission/nodes_pb2.py,sha256=sAOb0qHvHHmAR4tfbjTR3FnysPsULBVdf8tNmDmv6O0,35343
+bosdyn/api/mission/mission_service_pb2.py,sha256=eDgOBZNh3bQMIQagNtHLBzx_awPb4kAMoY2QrWIeQlQ,2795
+bosdyn/api/mission/mission_service_pb2_grpc.py,sha256=QCjOnrOB-tFTqclsDKee83xRenrEcIIxOVnok-Z04Tw,25418
+bosdyn/api/mission/nodes_pb2.py,sha256=FP_0ZvmDvEJDuTT-o6NiPbZ4siaZGsU83OU2wmvAxGU,39359
 bosdyn/api/mission/nodes_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
-bosdyn/api/mission/remote_pb2.py,sha256=IxLgkYlR-iBVqUwOEWcK5YX2qCpNvjrLFcpiZEuXFNs,8546
+bosdyn/api/mission/remote_pb2.py,sha256=D_kLPRVQ5KNjiguWg_D3Z4iVWJc8HLTsdYpMMD92WsY,10873
 bosdyn/api/mission/remote_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
-bosdyn/api/mission/remote_service_pb2.py,sha256=NxnJqDspx9fprvfWqj5yMIq8GDIOKpRow32lpqXIj7Y,1677
-bosdyn/api/mission/remote_service_pb2_grpc.py,sha256=D9qAkmCF1WvTmyI7TvxkhRQahjGEbByS97sZpeNIaqI,8610
-bosdyn/api/mission/util_pb2.py,sha256=5hzxZE0sANfrYQL_govAjoE4gSha2ZlfBgGkdmax2Yw,4891
+bosdyn/api/mission/remote_service_pb2.py,sha256=9J4t7QejssWdxQ_PckuTu8t2V1n0qsUVvaBzC1VwviI,1853
+bosdyn/api/mission/remote_service_pb2_grpc.py,sha256=hN5Sy0tXoMHZzTski0ekQ1EwVIOnf67zzFhdsb473L0,10655
+bosdyn/api/mission/util_pb2.py,sha256=W7sTK7LQE-Z8gsyT1OwYmUkBjOdyWULds8kh2CxO7Ok,4972
 bosdyn/api/mission/util_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
-bosdyn/api/spot/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-bosdyn/api/spot/door_pb2.py,sha256=xHu8aybhFLgM04ykUiJDaFoRSPhvcLayeqL8KhKX1yc,11176
+bosdyn/api/spot/__init__.py,sha256=h-QyvMVzDNpT3jyVskcSbUVFXxGCRxieFPrvTveZG9k,64
+bosdyn/api/spot/door_area_callback_pb2.py,sha256=33NT0Mb43ijSd7Rzf42OTFflcK7jkzaB56VEtWQiyqQ,1752
+bosdyn/api/spot/door_area_callback_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
+bosdyn/api/spot/door_pb2.py,sha256=Tqc4QdOIDtpSP46W6B3b3clK45mu5TAcWPlVX3g_L-U,11446
 bosdyn/api/spot/door_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/spot/door_service_pb2.py,sha256=__NEUfm5rHDdP4_T-ongMicvDTeD7mUUNqKq7B-LCYQ,1405
 bosdyn/api/spot/door_service_pb2_grpc.py,sha256=SQU3X--UCFMVVLe7I-oYGfgli0FKnR4fQ3lKSgd8SHY,4442
-bosdyn/api/spot/robot_command_pb2.py,sha256=Ox4aYxnFtVgvTvA51S3fUS-bD3Z4QyhblvBl6oJ5pus,10278
+bosdyn/api/spot/inverse_kinematics_pb2.py,sha256=EhLFEepQkbrsO_TmGsjM_SoilFpfTOXU3IWLlX6qnJY,9597
+bosdyn/api/spot/inverse_kinematics_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
+bosdyn/api/spot/inverse_kinematics_service_pb2.py,sha256=HQp68MaWtErhnQYz71CFYqS9oV_2gf8sJKjCe0xHkjs,1429
+bosdyn/api/spot/inverse_kinematics_service_pb2_grpc.py,sha256=YhmVDKJ0Z2HpCee7yFyTbhNND36nKePl_04ZHKZShVg,2964
+bosdyn/api/spot/robot_command_pb2.py,sha256=9dvsEUh29u9hLuYV8-2N3PzlhSoh1EdBLnBBaa9a1q0,11055
 bosdyn/api/spot/robot_command_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/spot/spot_check_pb2.py,sha256=rtGEaVC4yAqj0Pu-e8i5jPXK1tUtUCeo7jXz-uH6fT4,26549
 bosdyn/api/spot/spot_check_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/spot/spot_check_service_pb2.py,sha256=spQKHwTnYGHMl2jM6MN1WUkzulaZ-ti5xcLiT6g9Ys4,1793
 bosdyn/api/spot/spot_check_service_pb2_grpc.py,sha256=Jujqoo-1951yx8rV9r5S1K1YXOrvLPPsVcse9QXDKd0,9156
 bosdyn/api/spot_cam/LED_pb2.py,sha256=6SQghlqbc4whQC0PZ7bVW5EgXhj7GvqemImcqusq69I,4579
 bosdyn/api/spot_cam/LED_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
-bosdyn/api/spot_cam/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+bosdyn/api/spot_cam/__init__.py,sha256=h-QyvMVzDNpT3jyVskcSbUVFXxGCRxieFPrvTveZG9k,64
 bosdyn/api/spot_cam/audio_pb2.py,sha256=S2Jaacc665Go48-fVif2ArHwz_blXLHM9Q6uw1FT7N0,15517
 bosdyn/api/spot_cam/audio_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/spot_cam/camera_pb2.py,sha256=6VNfcrsvqafziFwDn95NNbZv2nOj6YPzVcDUeh9zVdo,3538
 bosdyn/api/spot_cam/camera_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
-bosdyn/api/spot_cam/compositor_pb2.py,sha256=E_jcNfN380O_rN2msyZhDklvAjWW0ugFDknKrFdG-Ow,15452
+bosdyn/api/spot_cam/compositor_pb2.py,sha256=cJ4mgQkzJThXn5Qc_XT3MIoM5Bql8a8GpEZV11p541A,18911
 bosdyn/api/spot_cam/compositor_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/spot_cam/health_pb2.py,sha256=6yZuQKSokd9Qr62EHkFSncB9n-IMPMvYkAmjCliuwe8,8084
 bosdyn/api/spot_cam/health_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/spot_cam/logging_pb2.py,sha256=p0sVEp9bo0U_6tvN2Z50zygET1IKO9Ifw-I2IMSDsnw,18025
 bosdyn/api/spot_cam/logging_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
-bosdyn/api/spot_cam/network_pb2.py,sha256=lFU_9QRUeBk-RtNnGJ0LDFXnXxHm1kay9R50alPmxiI,8137
+bosdyn/api/spot_cam/network_pb2.py,sha256=IkErjOkPu17eIzuG1v_MoyAlsC2QuG-42-L-LFLN9qY,10120
 bosdyn/api/spot_cam/network_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/spot_cam/power_pb2.py,sha256=05DUC9-QRbbmcVlnuFQU1Mf0X6Ln2XA2lZMGgp1xPXg,5834
 bosdyn/api/spot_cam/power_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
-bosdyn/api/spot_cam/ptz_pb2.py,sha256=HnjM6TtSXP1uV9pFw41fDtsxEDemgQ7LDUwwQ8yPSWo,11901
+bosdyn/api/spot_cam/ptz_pb2.py,sha256=Pp9MmM0GtwF3zyKvSYRfcpCa9CGydzuxlvsGv1QV1Hw,15674
 bosdyn/api/spot_cam/ptz_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
-bosdyn/api/spot_cam/service_pb2.py,sha256=vtbDLjMt2YeS9thrpCfFd0Z0_pFHfTEnei8hEl5Hcyw,9653
-bosdyn/api/spot_cam/service_pb2_grpc.py,sha256=jJNk8UlqCFvFQfLiVCzP1V402-E0-526OKacy2rTSrM,96507
-bosdyn/api/spot_cam/streamquality_pb2.py,sha256=OcN0phQodEwdIhxBJuXACX0jwbnIgaLUMXIfYS5XePY,7466
+bosdyn/api/spot_cam/service_pb2.py,sha256=YZ77CQN32h69ElYoa1OjeaG98flhhWTuJzkBV1r-j80,10034
+bosdyn/api/spot_cam/service_pb2_grpc.py,sha256=L78ytxPYaQxgMxhYw0vcrJhh3QutjElOdDbgfSjoawc,102016
+bosdyn/api/spot_cam/streamquality_pb2.py,sha256=fw8XlwNW-bTWcD_452AGaOHK7X4zvXAE1dYbHDbfKe0,9899
 bosdyn/api/spot_cam/streamquality_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
 bosdyn/api/spot_cam/version_pb2.py,sha256=6cLKJEMeGthG_J-Cus1KjDyRKwZgFGQtt79Zha5QJfw,2518
 bosdyn/api/spot_cam/version_pb2_grpc.py,sha256=1oboBPFxaTEXt9Aw7EAj8gXHDCNMhZD2VXqocC9l_gk,159
-bosdyn_api-3.2.3.dist-info/METADATA,sha256=fUBAWLCK293-sNDuv6UQnsUHZCD2d58ZixCzfcLfqQY,1403
-bosdyn_api-3.2.3.dist-info/WHEEL,sha256=h_aVn5OB2IERUjMbi2pucmR_zzWJtk303YXvhh60NJ8,110
-bosdyn_api-3.2.3.dist-info/top_level.txt,sha256=an2OWgx1ej2jFjmBjPWNQ68ZglvUfKhmXWW-WhTtDmA,7
-bosdyn_api-3.2.3.dist-info/RECORD,,
+bosdyn_api-3.3.0.dist-info/METADATA,sha256=1TtrozVb2i8EvDCy2Y26jCOE436DU-rCrygYIrDBFLY,1568
+bosdyn_api-3.3.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+bosdyn_api-3.3.0.dist-info/top_level.txt,sha256=an2OWgx1ej2jFjmBjPWNQ68ZglvUfKhmXWW-WhTtDmA,7
+bosdyn_api-3.3.0.dist-info/RECORD,,
```

