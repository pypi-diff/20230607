# Comparing `tmp/bosdyn_mission-3.2.3-py2.py3-none-any.whl.zip` & `tmp/bosdyn_mission-3.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 15137 bytes, number of entries: 12
--rw-r--r--  2.0 unx      330 b- defN 23-Mar-24 15:44 bosdyn/__init__.py
--rw-r--r--  2.0 unx      483 b- defN 23-Mar-24 15:44 bosdyn/mission/__init__.py
--rw-r--r--  2.0 unx    18838 b- defN 23-Mar-24 15:44 bosdyn/mission/client.py
--rw-r--r--  2.0 unx      433 b- defN 23-Mar-24 15:44 bosdyn/mission/constants.py
--rw-r--r--  2.0 unx     3982 b- defN 23-Mar-24 15:44 bosdyn/mission/exceptions.py
--rw-r--r--  2.0 unx    10812 b- defN 23-Mar-24 15:44 bosdyn/mission/remote_client.py
--rw-r--r--  2.0 unx     1654 b- defN 23-Mar-24 15:44 bosdyn/mission/server_util.py
--rw-r--r--  2.0 unx    13310 b- defN 23-Mar-24 15:44 bosdyn/mission/util.py
--rw-r--r--  2.0 unx     1731 b- defN 23-Mar-24 15:44 bosdyn_mission-3.2.3.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Mar-24 15:44 bosdyn_mission-3.2.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Mar-24 15:44 bosdyn_mission-3.2.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      987 b- defN 23-Mar-24 15:44 bosdyn_mission-3.2.3.dist-info/RECORD
-12 files, 52677 bytes uncompressed, 13481 bytes compressed:  74.4%
+Zip file size: 15542 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      330 b- defN 23-Jun-07 02:50 bosdyn/__init__.py
+-rw-r--r--  2.0 unx      483 b- defN 23-Jun-07 02:50 bosdyn/mission/__init__.py
+-rw-r--r--  2.0 unx    20860 b- defN 23-Jun-07 02:50 bosdyn/mission/client.py
+-rw-r--r--  2.0 unx      435 b- defN 23-Jun-07 02:50 bosdyn/mission/constants.py
+-rw-r--r--  2.0 unx     3941 b- defN 23-Jun-07 02:50 bosdyn/mission/exceptions.py
+-rw-r--r--  2.0 unx    12196 b- defN 23-Jun-07 02:50 bosdyn/mission/remote_client.py
+-rw-r--r--  2.0 unx     1661 b- defN 23-Jun-07 02:50 bosdyn/mission/server_util.py
+-rw-r--r--  2.0 unx    13192 b- defN 23-Jun-07 02:50 bosdyn/mission/util.py
+-rw-r--r--  2.0 unx     1782 b- defN 23-Jun-07 02:50 bosdyn_mission-3.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 02:50 bosdyn_mission-3.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-07 02:50 bosdyn_mission-3.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      986 b- defN 23-Jun-07 02:50 bosdyn_mission-3.3.0.dist-info/RECORD
+12 files, 55965 bytes uncompressed, 13886 bytes compressed:  75.2%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: bosdyn/mission/server_util.py
 Comment: 
 
 Filename: bosdyn/mission/util.py
 Comment: 
 
-Filename: bosdyn_mission-3.2.3.dist-info/METADATA
+Filename: bosdyn_mission-3.3.0.dist-info/METADATA
 Comment: 
 
-Filename: bosdyn_mission-3.2.3.dist-info/WHEEL
+Filename: bosdyn_mission-3.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: bosdyn_mission-3.2.3.dist-info/top_level.txt
+Filename: bosdyn_mission-3.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: bosdyn_mission-3.2.3.dist-info/RECORD
+Filename: bosdyn_mission-3.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bosdyn/__init__.py

```diff
@@ -1,7 +1,7 @@
-# Copyright (c) 2022 Boston Dynamics, Inc.  All rights reserved.
+# Copyright (c) 2023 Boston Dynamics, Inc.  All rights reserved.
 #
 # Downloading, reproducing, distributing or otherwise using the SDK Software
 # is subject to the terms and conditions of the Boston Dynamics Software
 # Development Kit License (20191101-BDSDK-SL).
 
 __path__ = __import__('pkgutil').extend_path(__path__, __name__)
```

## bosdyn/mission/__init__.py

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 Boston Dynamics, Inc.  All rights reserved.
+# Copyright (c) 2023 Boston Dynamics, Inc.  All rights reserved.
 #
 # Downloading, reproducing, distributing or otherwise using the SDK Software
 # is subject to the terms and conditions of the Boston Dynamics Software
 # Development Kit License (20191101-BDSDK-SL).
 
 """The mission library package.
 Sets up some convenience imports for commonly used classes and functions.
```

## bosdyn/mission/client.py

```diff
@@ -1,25 +1,26 @@
-# Copyright (c) 2022 Boston Dynamics, Inc.  All rights reserved.
+# Copyright (c) 2023 Boston Dynamics, Inc.  All rights reserved.
 #
 # Downloading, reproducing, distributing or otherwise using the SDK Software
 # is subject to the terms and conditions of the Boston Dynamics Software
 # Development Kit License (20191101-BDSDK-SL).
 
 """For clients to the mission service."""
 
 import collections
 from builtins import str as text
 
 from google.protobuf import timestamp_pb2
 
 from bosdyn.api.mission import mission_pb2, mission_service_pb2_grpc
+from bosdyn.client import data_chunk
 from bosdyn.client.common import (BaseClient, common_header_errors, error_factory,
                                   handle_common_header_errors, handle_lease_use_result_errors,
                                   handle_unset_status_error)
-from bosdyn.client.exceptions import ResponseError, TimeSyncRequired
+from bosdyn.client.exceptions import ResponseError, TimeSyncRequired, UnimplementedError
 from bosdyn.client.lease import add_lease_wallet_processors
 
 
 class MissionResponseError(ResponseError):
     """General class of errors for mission service."""
 
 
@@ -156,37 +157,72 @@
             RpcError: Problem communicating with the robot.
             bosdyn.mission.client.CompilationError: The mission failed to compile.
             bosdyn.mission.client.ValidationError: The mission failed to validate.
         """
         req = self._load_mission_request(root, leases)
         self._apply_request_processors(req, copy_request=False)
         return self.call(self._stub.LoadMissionAsChunks,
-                         BaseClient.chunk_message(req, data_chunk_byte_size), None,
+                         data_chunk.chunk_message(req, data_chunk_byte_size), None,
                          _load_mission_error_from_response, **kwargs)
 
-    def play_mission(self, pause_time_secs, leases=[], settings=None, **kwargs):
+    def load_mission_as_chunks2(self, root, leases=[], data_chunk_byte_size=1000 * 1000, **kwargs):
+        """Load a mission onto the robot.
+        Args:
+            root: Root node in a mission.
+            leases: All leases necessary to initialize a mission.
+            data_chunk_byte_size: max size of each streamed message
+        Raises:
+            RpcError: Problem communicating with the robot.
+            bosdyn.mission.client.CompilationError: The mission failed to compile.
+            bosdyn.mission.client.ValidationError: The mission failed to validate.
+        """
+        req = self._load_mission_request(root, leases)
+        self._apply_request_processors(req, copy_request=False)
+        return self.call(self._stub.LoadMissionAsChunks2,
+                         data_chunk.chunk_message(req, data_chunk_byte_size),
+                         error_from_response=_load_mission_error_from_response,
+                         assemble_type=mission_pb2.LoadMissionResponse, copy_request=False,
+                         **kwargs)
+
+    def play_mission(
+            self,
+            pause_time_secs,
+            leases=[],
+            settings=None,
+            **kwargs):
         """Play the loaded mission.
 
         Args:
           pause_time_secs: Absolute time when the mission should pause execution. Subsequent RPCs
               will override this value, so you can use this to say "if you don't hear from me again,
               stop running the mission at this time."
           leases: Leases the mission service will need to use. Unlike other clients, these MUST
               be specified.
         Raises:
             RpcError: Problem communicating with the robot.
             NoMissionError: No mission Loaded.
         """
-        req = self._play_mission_request(pause_time_secs, leases, settings)
+        req = self._play_mission_request(
+            pause_time_secs,
+            leases,
+            settings)
         return self.call(self._stub.PlayMission, req, None, _play_mission_error_from_response,
                          copy_request=False, **kwargs)
 
-    def play_mission_async(self, pause_time_secs, leases=[], settings=None, **kwargs):
+    def play_mission_async(
+            self,
+            pause_time_secs,
+            leases=[],
+            settings=None,
+            **kwargs):
         """Async version of play_mission."""
-        req = self._play_mission_request(pause_time_secs, leases, settings)
+        req = self._play_mission_request(
+            pause_time_secs,
+            leases,
+            settings)
         return self.call_async(self._stub.PlayMission, req, None, _play_mission_error_from_response,
                                copy_request=False, **kwargs)
 
     def restart_mission(self, pause_time_secs, leases=[], settings=None, **kwargs):
         """Restart the loaded mission.
 
         Args:
@@ -263,23 +299,34 @@
     def get_mission(self, **kwargs):
         """Get the loaded mission.
 
         Raises:
             RpcError: Problem communicating with the robot.
         """
         req = self._get_mission_request()
-        return self.call(self._stub.GetMission, req, None, common_header_errors, copy_request=False,
-                         **kwargs)
+        try:
+            return self._get_mission_as_chunks_call(req)
+        except UnimplementedError as err:
+            # This indicates that the software release running on robot does not yet have
+            # the implementation for the streaming response of GetMission.
+            return self.call(self._stub.GetMission, req, None, common_header_errors,
+                             copy_request=False, **kwargs)
 
     def get_mission_async(self, **kwargs):
         """Async version of get_mission()."""
         req = self._get_mission_request()
         return self.call_async(self._stub.GetMission, req, None, common_header_errors,
                                copy_request=False, **kwargs)
 
+    def _get_mission_as_chunks_call(self, req, **kwargs):
+        """Issues the GetMissionAsChunks RPC to the mission service."""
+        return self.call(self._stub.GetMissionAsChunks, req, value_from_response=None,
+                         error_from_response=common_header_errors,
+                         assemble_type=mission_pb2.GetMissionResponse, copy_request=False, **kwargs)
+
     @staticmethod
     def _get_state_request(upper_tick_bound, lower_tick_bound, past_ticks):
         if lower_tick_bound is not None and past_ticks is not None:
             raise ValueError('Cannot specify both lower_tick_bound and past_ticks')
         request = mission_pb2.GetStateRequest(history_lower_tick_bound=lower_tick_bound,
                                               history_past_ticks=past_ticks)
         if upper_tick_bound is not None:
@@ -293,15 +340,19 @@
     @staticmethod
     def _load_mission_request(root, leases):
         request = mission_pb2.LoadMissionRequest(root=root)
         for lease in leases:
             request.leases.add().CopyFrom(lease.lease_proto)
         return request
 
-    def _play_mission_request(self, pause_time_secs, leases, settings):
+    def _play_mission_request(
+            self,
+            pause_time_secs,
+            leases,
+            settings):
         request = mission_pb2.PlayMissionRequest(
             pause_time=self.timesync_endpoint.robot_timestamp_from_local_secs(pause_time_secs),
             settings=settings)
         for lease in leases:
             request.leases.add().CopyFrom(lease.lease_proto)
         return request
```

## bosdyn/mission/constants.py

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 Boston Dynamics, Inc.  All rights reserved.
+# Copyright (c) 2023 Boston Dynamics, Inc.  All rights reserved.
 #
 # Downloading, reproducing, distributing or otherwise using the SDK Software
 # is subject to the terms and conditions of the Boston Dynamics Software
 # Development Kit License (20191101-BDSDK-SL).
 
 """Constants relevant to the missions service."""
 
@@ -11,7 +11,9 @@
 
 @enum.unique
 class Result(enum.IntEnum):
     FAILURE = 1
     RUNNING = 2
     SUCCESS = 3
     ERROR = 4
+
+
```

## bosdyn/mission/exceptions.py

```diff
@@ -1,15 +1,13 @@
-# Copyright (c) 2022 Boston Dynamics, Inc.  All rights reserved.
+# Copyright (c) 2023 Boston Dynamics, Inc.  All rights reserved.
 #
 # Downloading, reproducing, distributing or otherwise using the SDK Software
 # is subject to the terms and conditions of the Boston Dynamics Software
 # Development Kit License (20191101-BDSDK-SL).
 
-from __future__ import unicode_literals
-
 from builtins import str as text
 
 from bosdyn.mission import util
 
 
 class Error(Exception):
     """Base exception"""
```

## bosdyn/mission/remote_client.py

```diff
@@ -1,21 +1,21 @@
-# Copyright (c) 2022 Boston Dynamics, Inc.  All rights reserved.
+# Copyright (c) 2023 Boston Dynamics, Inc.  All rights reserved.
 #
 # Downloading, reproducing, distributing or otherwise using the SDK Software
 # is subject to the terms and conditions of the Boston Dynamics Software
 # Development Kit License (20191101-BDSDK-SL).
 
 """Client for the RemoteMission service."""
 
 import collections
 
 from bosdyn.api.mission import remote_pb2, remote_service_pb2_grpc
 from bosdyn.client.common import (BaseClient, common_header_errors, error_factory,
-                                  handle_common_header_errors, handle_lease_use_result_errors,
-                                  handle_unset_status_error)
+                                  handle_common_header_errors, handle_custom_params_errors,
+                                  handle_lease_use_result_errors, handle_unset_status_error)
 from bosdyn.client.exceptions import ResponseError
 from bosdyn.client.lease import (DEFAULT_RESOURCES, LeaseWalletRequestProcessor,
                                  LeaseWalletResponseProcessor)
 from bosdyn.mission import constants
 
 
 class Error(Exception):
@@ -81,35 +81,38 @@
         req = self._build_establish_session_request(inputs=inputs, leases=leases,
                                                     lease_resources=lease_resources)
         return self.call_async(self._stub.EstablishSession, req,
                                value_from_response=_session_id_from_response,
                                error_from_response=_establish_error_from_response,
                                copy_request=False, **kwargs)
 
-    def tick(self, session_id, leases=(), inputs=None, lease_resources=DEFAULT_RESOURCES, **kwargs):
+    def tick(self, session_id, leases=(), inputs=None, lease_resources=DEFAULT_RESOURCES,
+             group_name=None, params=None, **kwargs):
         """Tick the remote node.
 
         Args:
             session_id: session
             leases (Iterable[Lease]): List of lease protobufs to use during the tick.
             inputs (Iterable[bosdyn.api.mission.KeyValue]): any inputs needed by by the remote node.
             lease_resources (Iterable[str]): List of resource names to use from the lease wallet.
                 Only applied if no leases are provided.
         """
         req = self._build_tick_request(inputs=inputs, leases=leases, session_id=session_id,
-                                       lease_resources=lease_resources)
+                                       lease_resources=lease_resources, group_name=group_name,
+                                       params=params)
         return self.call(self._stub.Tick, req, value_from_response=None,
                          error_from_response=_tick_error_from_response, copy_request=False,
                          **kwargs)
 
     def tick_async(self, session_id, leases=(), inputs=None, lease_resources=DEFAULT_RESOURCES,
-                   **kwargs):
+                   group_name=None, params=None, **kwargs):
         """Async version of tick()"""
         req = self._build_tick_request(inputs=inputs, leases=leases, session_id=session_id,
-                                       lease_resources=lease_resources)
+                                       lease_resources=lease_resources, group_name=group_name,
+                                       params=params)
         return self.call_async(self._stub.Tick, req, value_from_response=None,
                                error_from_response=_tick_error_from_response, copy_request=False,
                                **kwargs)
 
     def stop(self, session_id, **kwargs):
         req = remote_pb2.StopRequest(session_id=session_id)
         return self.call(self._stub.Stop, req, value_from_response=None,
@@ -130,24 +133,49 @@
 
     def teardown_session_async(self, session_id, **kwargs):
         req = remote_pb2.TeardownSessionRequest(session_id=session_id)
         return self.call_async(self._stub.TeardownSession, req, value_from_response=None,
                                error_from_response=_teardown_error_from_response,
                                copy_request=False, **kwargs)
 
+    def get_service_info(self, **kwargs):
+        """Get information about the service itself, such as a custom parameter spec.
+
+        Raises:
+            RpcError: problem communicating with the robot.
+
+        Returns:
+            A GetRemoteMissionServiceInfoResponse message describing this service.
+        """
+        req = remote_pb2.GetRemoteMissionServiceInfoRequest()
+        return self.call(self._stub.GetRemoteMissionServiceInfo, req,
+                         error_from_response=common_header_errors, copy_request=False, **kwargs)
+
+    def get_service_info_async(self, **kwargs):
+        """Async version of get_service_info()"""
+        req = remote_pb2.GetRemoteMissionServiceInfoRequest()
+        return self.call_async(self._stub.GetRemoteMissionServiceInfo, req,
+                               error_from_response=common_header_errors, copy_request=False,
+                               **kwargs)
+
     def _build_establish_session_request(self, inputs, leases, lease_resources):
         req = remote_pb2.EstablishSessionRequest(inputs=inputs)
         _copy_leases(req, leases)
         if self.lease_processor:
             self.lease_processor.mutate(req, resource_list=lease_resources)
 
         return req
 
-    def _build_tick_request(self, inputs, leases, session_id, lease_resources):
+    def _build_tick_request(self, inputs, leases, session_id, lease_resources, group_name=None,
+                            params=None):
         req = remote_pb2.TickRequest(inputs=inputs, session_id=session_id)
+        if group_name:
+            req.group_name = group_name
+        if params:
+            req.params.CopyFrom(params)
         _copy_leases(req, leases)
         if self.lease_processor:
             self.lease_processor.mutate(req, resource_list=lease_resources)
         return req
 
 
 def _copy_leases(req, leases):
@@ -197,14 +225,15 @@
     remote_pb2.TickResponse.STATUS_MISSING_INPUTS: (MissingInputs, MissingInputs.__doc__),
     remote_pb2.TickResponse.STATUS_INVALID_SESSION_ID: (InvalidSessionId, InvalidSessionId.__doc__),
 })
 
 
 @handle_common_header_errors
 @handle_lease_use_result_errors
+@handle_custom_params_errors
 @handle_unset_status_error(unset='STATUS_UNKNOWN')
 def _tick_error_from_response(response):
     return error_factory(response, response.status,
                          status_to_string=remote_pb2.TickResponse.Status.Name,
                          status_to_error=_TICK_STATUS_TO_ERROR)
```

## bosdyn/mission/server_util.py

```diff
@@ -1,14 +1,14 @@
-# Copyright (c) 2022 Boston Dynamics, Inc.  All rights reserved.
+# Copyright (c) 2023 Boston Dynamics, Inc.  All rights reserved.
 #
 # Downloading, reproducing, distributing or otherwise using the SDK Software
 # is subject to the terms and conditions of the Boston Dynamics Software
 # Development Kit License (20191101-BDSDK-SL).
 
-from deprecated import deprecated
+from deprecated.sphinx import deprecated
 
 import bosdyn.util
 from bosdyn.api import header_pb2
 
 
 
 @deprecated(reason='The ResponseContext helper class has moved to a common location. Please use '
```

## bosdyn/mission/util.py

```diff
@@ -1,35 +1,33 @@
-# Copyright (c) 2022 Boston Dynamics, Inc.  All rights reserved.
+# Copyright (c) 2023 Boston Dynamics, Inc.  All rights reserved.
 #
 # Downloading, reproducing, distributing or otherwise using the SDK Software
 # is subject to the terms and conditions of the Boston Dynamics Software
 # Development Kit License (20191101-BDSDK-SL).
 
-from __future__ import unicode_literals
-
 import copy
+import json
 import operator
 import re
 from builtins import str as text
 
 import google.protobuf.message
+import google.protobuf.struct_pb2
 import google.protobuf.text_format
-import six
 
 from bosdyn.api import data_acquisition_pb2, geometry_pb2, gripper_camera_param_pb2
+from bosdyn.api.autowalk import walks_pb2
 from bosdyn.api.docking import docking_pb2
 from bosdyn.api.graph_nav import graph_nav_pb2
 from bosdyn.api.mission import mission_pb2, nodes_pb2, util_pb2
 from bosdyn.mission import constants
 
 # This is a special dummy message we'll use for TYPE_MESSAGE parameters.
 DUMMY_MESSAGE = nodes_pb2.Node(name='dummy-message-for-parameterization')
 
-UNEXPECTED_EXCEPTION_EVENT_TYPE = 'bosdyn:mission:exception'
-
 
 
 class Error(Exception):
     pass
 
 
 class InvalidConversion(Error):
@@ -40,15 +38,15 @@
         self.destination_typename = destination_typename
 
     def __str__(self):
         return 'Could not convert "{}" to type "{}"'.format(self.original_value,
                                                             self.destination_typename)
 
 
-_python_identifier_regex = re.compile('[A-Za-z_]\w*$')
+_python_identifier_regex = re.compile(r'[A-Za-z_]\w*$')
 
 
 def tree_to_string(root, start_level=0, include_status=False):
     """Get a string representation of a Node, interpreted as a tree."""
     string = ''
     if start_level == 0:
         string += '\n'
@@ -93,28 +91,28 @@
     if isinstance(name_or_dict, dict):
         node.name = name_or_dict.get('name', '')
         node.reference_id = name_or_dict.get('reference_id', '')
         node.node_reference = name_or_dict.get('node_reference', '')
         if 'user_data' in name_or_dict:
             node.user_data.CopyFrom(name_or_dict['user_data'])
 
-        for name, pb_type in six.iteritems(name_or_dict.get('parameters', {})):
+        for name, pb_type in name_or_dict.get('parameters', {}).items():
             parameter = util_pb2.VariableDeclaration(name=name, type=pb_type)
             node.parameters.add().CopyFrom(parameter)
 
-        for key, value in six.iteritems(name_or_dict.get('parameter_values', {})):
+        for key, value in name_or_dict.get('parameter_values', {}).items():
             parameter_value = util_pb2.KeyValue(key=key)
-            if isinstance(value, six.string_types) and value[0] == '$':
+            if isinstance(value, str) and value[0] == '$':
                 parameter_value.value.parameter.name = value[1:]
                 # Leave type unspecified, since we can't look it up easily yet.
             else:
                 parameter_value.value.constant.CopyFrom(python_var_to_value(value))
             node.parameter_values.add().CopyFrom(parameter_value)
 
-        for key, value in six.iteritems(name_or_dict.get('overrides', {})):
+        for key, value in name_or_dict.get('overrides', {}).items():
             # Rather than keep this matching the compiler functionality, just omit the check.
             # It's not even a CompileError anyway.
             #if key not in inner_proto.DESCRIPTOR.fields_by_name:
             #    raise CompileError('Override specified for "{}" but no such field in "{}"'.format(
             #        key, inner_proto.DESCRIPTOR.full_name))
             override = util_pb2.KeyValue(key=key)
             override.value.parameter.name = value
@@ -156,37 +154,37 @@
 
 
 def python_var_to_value(var):
     """Returns a ConstantValue with the appropriate oneof set."""
     value = util_pb2.ConstantValue()
     if isinstance(var, bool):
         value.bool_value = var
-    elif isinstance(var, six.integer_types):
+    elif isinstance(var, int):
         value.int_value = var
     elif isinstance(var, float):
         value.float_value = var
-    elif isinstance(var, six.string_types):
+    elif isinstance(var, str):
         value.string_value = var
     elif isinstance(var, google.protobuf.message.Message):
         value.msg_value.Pack(var)
     else:
         raise Error('Invalid type "{}"'.format(type(var)))
     return value
 
 
 def python_type_to_pb_type(var):
     """Returns the protobuf-schema variable type that corresponds to the given variable."""
     if isinstance(var, bool):
         return util_pb2.VariableDeclaration.TYPE_BOOL
-    elif isinstance(var, six.integer_types):
+    elif isinstance(var, int):
         return util_pb2.VariableDeclaration.TYPE_INT
     elif isinstance(var, float):
         # Python floating point is typically a C double.
         return util_pb2.VariableDeclaration.TYPE_FLOAT
-    elif isinstance(var, six.string_types):
+    elif isinstance(var, str):
         return util_pb2.VariableDeclaration.TYPE_STRING
     elif isinstance(var, google.protobuf.message.Message):
         return util_pb2.VariableDeclaration.TYPE_MESSAGE
     raise InvalidConversion(var, util_pb2.VariableDeclaration.Type.DESCRIPTOR.full_name)
 
 
 def is_string_identifier(string):
@@ -239,15 +237,15 @@
     results_from_proto = {
         util_pb2.RESULT_FAILURE: constants.Result.FAILURE,
         util_pb2.RESULT_RUNNING: constants.Result.RUNNING,
         util_pb2.RESULT_SUCCESS: constants.Result.SUCCESS,
         util_pb2.RESULT_ERROR: constants.Result.ERROR,
     }
 
-    proto_from_results = {v: k for k, v in six.iteritems(results_from_proto)}
+    proto_from_results = {v: k for k, v in results_from_proto.items()}
 
 
 def proto_enum_to_result_constant(proto_msg):
     """Returns a Result enum from a util_pb2.Result, or throws InvalidConversion error."""
     try:
         return ResultFromProto.results_from_proto[proto_msg]
     except KeyError:
@@ -325,7 +323,9 @@
 
 def safe_pb_enum_to_string(value, pb_enum_obj):
     try:
         return pb_enum_obj.Name(value)
     except ValueError:
         pass
     return '<unknown> (value: {})'.format(value)
+
+
```

## Comparing `bosdyn_mission-3.2.3.dist-info/METADATA` & `bosdyn_mission-3.3.0.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: bosdyn-mission
-Version: 3.2.3
+Version: 3.3.0
 Summary: Boston Dynamics mission code
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
-Requires-Dist: bosdyn-client (==3.2.3)
-Requires-Dist: bosdyn-api (==3.2.3)
-Requires-Dist: six
-Requires-Dist: future ; python_version < "3.3"
-Requires-Dist: enum34 ; python_version < "3.4"
+Requires-Dist: bosdyn-client (==3.3.0)
+Requires-Dist: bosdyn-api (==3.3.0)
 
 <!--
-Copyright (c) 2022 Boston Dynamics, Inc.  All rights reserved.
+Copyright (c) 2023 Boston Dynamics, Inc.  All rights reserved.
 
 Downloading, reproducing, distributing or otherwise using the SDK Software
 is subject to the terms and conditions of the Boston Dynamics Software
 Development Kit License (20191101-BDSDK-SL).
 -->
 
 # bosdyn-mission
@@ -36,9 +35,7 @@
 The bosdyn-mission wheel contains client interfaces and helper functionality for managing
 missions, which are part of the Boston Dynamics Spot API. The client interfaces in this wheel
 implement the mission-related Remote Procedure Calls (RPCs) defined in
 [bosdyn-api wheel](https://pypi.org/project/bosdyn-api/) and they utilize code included in the
 [bosdyn-client wheel](https://pypi.org/project/bosdyn-client/). Full design documentation for the
 functionality included in this wheel can be found
 [here](https://dev.bostondynamics.com/docs/concepts/autonomy/missions_service).
-
-
```

