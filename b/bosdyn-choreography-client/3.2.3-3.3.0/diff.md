# Comparing `tmp/bosdyn_choreography_client-3.2.3-py2.py3-none-any.whl.zip` & `tmp/bosdyn_choreography_client-3.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 20253 bytes, number of entries: 10
--rw-r--r--  2.0 unx      330 b- defN 23-Mar-24 15:44 bosdyn/__init__.py
--rw-r--r--  2.0 unx      330 b- defN 23-Mar-24 15:44 bosdyn/choreography/__init__.py
--rw-r--r--  2.0 unx      330 b- defN 23-Mar-24 15:44 bosdyn/choreography/client/__init__.py
--rw-r--r--  2.0 unx    18020 b- defN 23-Mar-24 15:44 bosdyn/choreography/client/animation_file_conversion_helpers.py
--rw-r--r--  2.0 unx    25360 b- defN 23-Mar-24 15:44 bosdyn/choreography/client/animation_file_to_proto.py
--rw-r--r--  2.0 unx    36272 b- defN 23-Mar-24 15:44 bosdyn/choreography/client/choreography.py
--rw-r--r--  2.0 unx     1482 b- defN 23-Mar-24 15:44 bosdyn_choreography_client-3.2.3.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Mar-24 15:44 bosdyn_choreography_client-3.2.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Mar-24 15:44 bosdyn_choreography_client-3.2.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      961 b- defN 23-Mar-24 15:44 bosdyn_choreography_client-3.2.3.dist-info/RECORD
-10 files, 83202 bytes uncompressed, 18573 bytes compressed:  77.7%
+Zip file size: 21426 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      330 b- defN 23-Jun-07 02:50 bosdyn/__init__.py
+-rw-r--r--  2.0 unx      330 b- defN 23-Jun-07 02:50 bosdyn/choreography/__init__.py
+-rw-r--r--  2.0 unx      330 b- defN 23-Jun-07 02:50 bosdyn/choreography/client/__init__.py
+-rw-r--r--  2.0 unx    18438 b- defN 23-Jun-07 02:50 bosdyn/choreography/client/animation_file_conversion_helpers.py
+-rw-r--r--  2.0 unx    25970 b- defN 23-Jun-07 02:50 bosdyn/choreography/client/animation_file_to_proto.py
+-rw-r--r--  2.0 unx    43561 b- defN 23-Jun-07 02:50 bosdyn/choreography/client/choreography.py
+-rw-r--r--  2.0 unx     1646 b- defN 23-Jun-07 02:50 bosdyn_choreography_client-3.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 02:50 bosdyn_choreography_client-3.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-07 02:50 bosdyn_choreography_client-3.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      960 b- defN 23-Jun-07 02:50 bosdyn_choreography_client-3.3.0.dist-info/RECORD
+10 files, 91664 bytes uncompressed, 19746 bytes compressed:  78.5%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: bosdyn/choreography/client/animation_file_to_proto.py
 Comment: 
 
 Filename: bosdyn/choreography/client/choreography.py
 Comment: 
 
-Filename: bosdyn_choreography_client-3.2.3.dist-info/METADATA
+Filename: bosdyn_choreography_client-3.3.0.dist-info/METADATA
 Comment: 
 
-Filename: bosdyn_choreography_client-3.2.3.dist-info/WHEEL
+Filename: bosdyn_choreography_client-3.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: bosdyn_choreography_client-3.2.3.dist-info/top_level.txt
+Filename: bosdyn_choreography_client-3.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: bosdyn_choreography_client-3.2.3.dist-info/RECORD
+Filename: bosdyn_choreography_client-3.3.0.dist-info/RECORD
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

## bosdyn/choreography/__init__.py

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

## bosdyn/choreography/client/__init__.py

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

## bosdyn/choreography/client/animation_file_conversion_helpers.py

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 Boston Dynamics, Inc.  All rights reserved.
+# Copyright (c) 2023 Boston Dynamics, Inc.  All rights reserved.
 #
 # Downloading, reproducing, distributing or otherwise using the SDK Software
 # is subject to the terms and conditions of the Boston Dynamics Software
 # Development Kit License (20191101-BDSDK-SL).
 
 """A set helpers which convert specific lines from an animation
 file into the animation-specific protobuf messages.
@@ -79,30 +79,30 @@
 
 def gripper_handler(val, animation_frame):
     animation_frame.gripper.gripper_angle.value = val
     return animation_frame
 
 
 def fl_contact_handler(val, animation_frame):
-    animation_frame.legs.fl.stance.value = val
+    animation_frame.legs.fl.stance.value = int(val)
     return animation_frame
 
 
 def fr_contact_handler(val, animation_frame):
-    animation_frame.legs.fr.stance.value = val
+    animation_frame.legs.fr.stance.value = int(val)
     return animation_frame
 
 
 def hl_contact_handler(val, animation_frame):
-    animation_frame.legs.hl.stance.value = val
+    animation_frame.legs.hl.stance.value = int(val)
     return animation_frame
 
 
 def hr_contact_handler(val, animation_frame):
-    animation_frame.legs.hr.stance.value = val
+    animation_frame.legs.hr.stance.value = int(val)
     return animation_frame
 
 
 def sh0_handler(val, animation_frame):
     animation_frame.arm.joint_angles.shoulder_0.value = val
     return animation_frame
 
@@ -383,18 +383,18 @@
     animation_frame.legs.hr.foot_pos.x.value = vals[9]
     animation_frame.legs.hr.foot_pos.y.value = vals[10]
     animation_frame.legs.hr.foot_pos.z.value = vals[11]
     return animation_frame
 
 
 def contact_handler(vals, animation_frame):
-    animation_frame.legs.fl.stance.value = vals[0]
-    animation_frame.legs.fr.stance.value = vals[1]
-    animation_frame.legs.hl.stance.value = vals[2]
-    animation_frame.legs.hr.stance.value = vals[3]
+    animation_frame.legs.fl.stance.value = int(vals[0])
+    animation_frame.legs.fr.stance.value = int(vals[1])
+    animation_frame.legs.hl.stance.value = int(vals[2])
+    animation_frame.legs.hr.stance.value = int(vals[3])
     return animation_frame
 
 
 def arm_joints_handler(vals, animation_frame):
     animation_frame.arm.joint_angles.shoulder_0.value = vals[0]
     animation_frame.arm.joint_angles.shoulder_1.value = vals[1]
     animation_frame.arm.joint_angles.elbow_0.value = vals[2]
@@ -523,29 +523,38 @@
 
 
 def precise_steps_option(file_line_split, animation):
     animation.proto.precise_steps = True
 
 
 def precise_timing_option(file_line_split, animation):
-    animation.proto.precise_timing = True
+    # Deprecated
+    animation.proto.timing_adjustability = -1
+
+
+def timing_adjustability_option(file_line_split, animation):
+    animation.proto.timing_adjustability = float(file_line_split[1])
 
 
 def no_looping_option(file_line_split, animation):
     animation.proto.no_looping = True
 
 
 def arm_required_option(file_line_split, animation):
     animation.proto.arm_required = True
 
 
 def arm_prohibited_option(file_line_split, animation):
     animation.proto.arm_prohibited = True
 
 
+def starts_sitting_option(file_line_split, animation):
+    animation.proto.starts_sitting = True
+
+
 def track_swing_trajectories_option(file_line_split, animation):
     animation.proto.track_swing_trajectories = True
     return animation
 
 
 def assume_zero_roll_and_pitch_option(file_line_split, animation):
     animation.proto.assume_zero_roll_and_pitch = True
@@ -594,7 +603,12 @@
 
 
 def description_option(file_line_split, animation):
     description = " ".join(file_line_split[1:])
     description = description.replace('"', '')  # remove any quotation marks
     animation.description = description
     return animation
+
+
+def custom_gait_cycle_option(file_line_split, animation):
+    animation.proto.custom_gait_cycle = True
+    return animation
```

## bosdyn/choreography/client/animation_file_to_proto.py

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 Boston Dynamics, Inc.  All rights reserved.
+# Copyright (c) 2023 Boston Dynamics, Inc.  All rights reserved.
 #
 # Downloading, reproducing, distributing or otherwise using the SDK Software
 # is subject to the terms and conditions of the Boston Dynamics Software
 # Development Kit License (20191101-BDSDK-SL).
 
 """A tool to convert animation files into protobuf messages which can be uploaded to the robot
 and used within choreography sequences."""
@@ -28,25 +28,28 @@
 OPTIONS_KEYWORDS_TO_FUNCTION = {
     "controls": controls_option,
     "bpm": bpm_option,
     "extendable": extendable_option,
     "truncatable": truncatable_option,
     "neutral_start": neutral_start_option,
     "precise_steps": precise_steps_option,
-    "precise_timing": precise_timing_option,
+    "precise_timing": precise_timing_option,  # Deprecated.
+    "timing_adjustability": timing_adjustability_option,
     "no_looping": no_looping_option,
     "arm_required": arm_required_option,
     "arm_prohibited": arm_prohibited_option,
+    "starts_sitting": starts_sitting_option,
     "track_swing_trajectories": track_swing_trajectories_option,
     "assume_zero_roll_and_pitch": assume_zero_roll_and_pitch_option,
     "arm_playback": arm_playback_option,
     "display_rgb": display_rgb_option,
     "frequency": frequency_option,
     "retime_to_integer_slices": retime_to_integer_slices_option,
     "description": description_option,
+    "custom_gait_cycle": custom_gait_cycle_option,
 }
 
 # The grouped headers represent animation keyframe values which can be used and specify multiple protobuf
 # values for a single header keyword. For example, body_pos has x/y/z position values.
 GROUPED_HEADERS = {
     "body_pos": (3, body_pos_handler),
     "com_pos": (3, com_pos_handler),
@@ -134,14 +137,19 @@
     "gripper": gripper_handler,
     "time": start_time_handler,
 }
 
 COMMENT_DELIMITERS = ["//", "#"]
 
 
+class AnimationFileFormatError(Exception):
+    """Specific Exception raised when we identify a issue with an animation (*.cha) file."""
+    pass
+
+
 class Animation():
     """Helper class to track values read from the animation file that are important to choreographer
     and necessary when uploading animated moves."""
 
     def __init__(self):
         # The name of the animated move.
         self.name = None
@@ -205,16 +213,21 @@
         move_info.display.category = choreography_sequence_pb2.ChoreographerDisplayInfo.CATEGORY_ANIMATION
         move_info.display.color.r = self.rgb[0]
         move_info.display.color.g = self.rgb[1]
         move_info.display.color.b = self.rgb[2]
         move_info.display.color.a = 1.0
         move_info.display.description = self.description
 
-        # Animations are required to start and end in a standing position.
-        move_info.entrance_states.append(choreography_sequence_pb2.MoveInfo.TRANSITION_STATE_STAND)
+        # Animations are required to start and end in a standing position (by default).
+        if self.proto.starts_sitting:
+            move_info.entrance_states.append(
+                choreography_sequence_pb2.MoveInfo.TRANSITION_STATE_SIT)
+        else:
+            move_info.entrance_states.append(
+                choreography_sequence_pb2.MoveInfo.TRANSITION_STATE_STAND)
         move_info.exit_state = choreography_sequence_pb2.MoveInfo.TRANSITION_STATE_STAND
 
         return move_info
 
 
 def set_proto(proto_object, attribute_name, attribute_value):
     """Helper function to set a field to a specific value in the protobuf message.
@@ -288,25 +301,25 @@
                 handle_nested_double_value_params(current_params_default, param_name,
                                                   min_max_default_vals[1])
                 handle_nested_double_value_params(current_params_max, param_name,
                                                   min_max_default_vals[2])
             except AttributeError:
                 err = "Cannot parse file %s: unknown parameter field name %s." % (animation.name,
                                                                                   param_name)
-                raise Exception(err)
+                raise AnimationFileFormatError(err)
         else:
             # Individual field using a DoubleValue proto.
             try:
                 set_proto(current_params_min, param_name, min_max_default_vals[0])
                 set_proto(current_params_default, param_name, min_max_default_vals[1])
                 set_proto(current_params_max, param_name, min_max_default_vals[2])
             except AttributeError:
                 err = "Cannot parse file %s: unknown parameter field name %s." % (animation.name,
                                                                                   param_name)
-                raise Exception(err)
+                raise AnimationFileFormatError(err)
     return animation
 
 
 def read_and_find_animation_params(animate_move_params_file, filepath_input=True):
     """Create a mapping of the parameter name to the default parameter values.
 
     Args:
@@ -440,15 +453,15 @@
                 # If the parameter name was provided with no user-specified min/max/default values,
                 # then attempt to use the default values from MoveParamsConfig.txt.
                 if split_line[0] in default_animate_params_values:
                     animation.parameter_lines.append(default_animate_params_values[split_line[0]])
                 else:
                     err = "Cannot parse file %s: parameter field name %s was provided but is not a default parameter." % (
                         animation.name, split_line[0])
-                    raise Exception(err)
+                    raise AnimationFileFormatError(err)
             else:
                 animation.parameter_lines.append(line)
 
         elif section_counter == 2:
             # The final section is the animated moves section.
             if len(movement_columns) == 0:
                 # The first line will contain all the different column headers.
@@ -456,15 +469,15 @@
 
                 # If "time" is not in the column, then we should set that for every keyframe based on frequency
                 if "time" not in movement_columns:
                     set_keyframe_times[0] = True
                     if animation.frequency is None:
                         prefix = "Cannot parse file %s: " % animation.name
                         err = prefix + "Either frequency or keyframe timestamps must be provided. Neither were found."
-                        raise Exception(err)
+                        raise AnimationFileFormatError(err)
                 continue
 
             vals = line.split()
             animation_keyframe = choreography_sequence_pb2.AnimationKeyframe()
             current_index = 0
             for header in movement_columns:
                 if header in GROUPED_HEADERS:
@@ -483,30 +496,30 @@
                         header_value = 1e-6
                     SINGLE_HEADERS[header](header_value, animation_keyframe)
                     current_index += 1
                 else:
                     # Don't fail silently and mismatch indices of other groups if one group header is not found.
                     err = "Cannot parse file %s: Unknown body movement keyword %s" % (
                         animation.name, header)
-                    raise Exception(err)
+                    raise AnimationFileFormatError(err)
 
             if set_keyframe_times[0]:
                 # Update the timestamp in the keyframe, then increment it based on the frequency
                 animation_keyframe.time = set_keyframe_times[1]
                 set_keyframe_times[1] += (1.0 / animation.frequency)
 
             # Add the animation frame into the animation proto.
             animation.proto.animation_keyframes.extend([animation_keyframe])
 
         else:
             # An animation file should only have 3 sections: the options, the parameters, and the body movement keyframes.
             err = (
                 "Cannot parse file %s: Animation file contains more than 3 sections delineated by whitespace."
                 " Make sure all comments are included in a existing section." % (animation.name))
-            raise Exception(err)
+            raise AnimationFileFormatError(err)
 
     animation.proto.name = animation.name
     if animation.bpm is not None:
         animation.proto.bpm = animation.bpm
 
     # Read out the parameters into protobuf messages.
     read_animation_params(animation)
```

## bosdyn/choreography/client/choreography.py

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 Boston Dynamics, Inc.  All rights reserved.
+# Copyright (c) 2023 Boston Dynamics, Inc.  All rights reserved.
 #
 # Downloading, reproducing, distributing or otherwise using the SDK Software
 # is subject to the terms and conditions of the Boston Dynamics Software
 # Development Kit License (20191101-BDSDK-SL).
 
 """For clients to use the choreography service"""
 import collections
@@ -170,14 +170,23 @@
             self._stub.UploadAnimatedMove,
             req,
             value_from_response=None,  # Return the complete response message
             error_from_response=_upload_animated_move_errors,
             copy_request=False,
             **kwargs)
 
+    def get_choreography_status(self, **kwargs):
+        """Get the dance related status information for a robot and the local time for which it was valid."""
+        request = choreography_sequence_pb2.ChoreographyStatusRequest()
+        status = self.call(self._stub.ChoreographyStatus, request, value_from_response=None,
+                           error_from_response=None, copy_request=False, **kwargs)
+        client_time = _TimeConverter(
+            self, self.timesync_endpoint).local_seconds_from_robot_timestamp(status.validity_time)
+        return (status, client_time)
+
     def choreography_log_to_animation_file(self, name, fpath, has_arm, *args):
         """Turn the choreography log from the proto into an animation `cha` file type.
 
         Args:
             name (string): Name that the `cha` file will be saved as.
             fpath (string): Location where the new `cha` file will be saved.
             has_arm (boolean): True if the robot has an arm, False if the robot doesn't have an arm. When False arm motion won't
@@ -372,14 +381,51 @@
             self._stub.ExecuteChoreography,
             req,
             value_from_response=None,  # Return the complete response message
             error_from_response=_execute_choreography_errors,
             copy_request=False,
             **kwargs)
 
+    def choreography_command(self, command_list, client_end_time, lease=None, **kwargs):
+        """Sends commands to interact with individual choreography moves.
+
+        Args:
+            command_list(list of choreography_sequence_pb2.MoveCommand protobuf): The commands.  Each 
+                command interacts with a single individual move.
+            client_end_time (float): The time (in seconds) that the command stops being valid. This time
+                should be provided in the local clock's timeframe and the client will convert it
+                to the required robot's clock timeframe.
+            lease (lease_pb2.Lease protobuf): A specific lease to use for the request. If nothing is
+                provided, the client will append the next lease sequence in this field by default.
+
+        Returns:
+            The full ChoreographyCommandResponse message.
+        """
+        req = self.build_choreography_command_request(command_list, client_end_time, lease)
+
+        return self.call(
+            self._stub.ChoreographyCommand,
+            req,
+            value_from_response=None,  # Return the complete response message
+            error_from_response=common_header_errors,
+            copy_request=False,
+            **kwargs)
+
+    def choreography_command_async(self, command_list, client_end_time, lease=None, **kwargs):
+        """Async version of choreography_command()."""
+        req = self.build_choreography_command_request(command_list, client_end_time, lease)
+
+        return self.call_async(
+            self._stub.ChoreographyCommand,
+            req,
+            value_from_response=None,  # Return the complete response message
+            error_from_response=common_header_errors,
+            copy_request=False,
+            **kwargs)
+
     def start_recording_state(self, duration_secs, continue_session_id=0, **kwargs):
         """Start (or continue) a manually recorded robot state log.
 
         Args:
             duration_secs (float): The duration of the recording request in seconds. This will
                 apply from when the StartRecording rpc is received.
             continue_session_id (int): If provided, the RPC will continue the recording
@@ -430,14 +476,82 @@
             self._stub.StopRecordingState,
             request,
             value_from_response=None,  # Return the complete response message
             error_from_response=common_header_errors,
             copy_request=False,
             **kwargs)
 
+    def save_sequence(self, seq_name, labels=[], **kwargs):
+        """Save an uploaded sequence to the robot. Saved sequences are 
+        automatically uploaded to the robot when it boots. 
+        
+        Returns:
+            The full SaveSequenceResponse proto."""
+        request = self.build_save_sequence_request(seq_name, labels)
+        return self.call(self._stub.SaveSequence, request, value_from_response=None,
+                         error_from_response=common_header_errors, copy_request=False, **kwargs)
+
+    def save_sequence_async(self, seq_name, labels=[], **kwargs):
+        """Async version of save_sequence()."""
+        request = self.build_save_sequence_request(seq_name, labels)
+        return self.call_async(self._stub.SaveSequence, request, value_from_response=None,
+                               error_from_response=common_header_errors, copy_request=False,
+                               **kwargs)
+
+    def delete_sequence(self, seq_name, **kwargs):
+        """Delete a sequence from temporary robot memory and 
+        delete any copies of the sequence saved to disk. 
+        
+        Returns:
+            The full DeleteSequenceResponse proto."""
+        request = choreography_sequence_pb2.DeleteSequenceRequest(sequence_name=seq_name)
+        return self.call(self._stub.DeleteSequence, request, value_from_response=None,
+                         error_from_response=common_header_errors, copy_request=False, **kwargs)
+
+    def delete_sequence_async(self, seq_name, **kwargs):
+        """Async version of delete_sequence()."""
+        request = choreography_sequence_pb2.DeleteSequenceRequest(sequence_name=seq_name)
+        return self.call_async(self._stub.DeleteSequence, request, value_from_response=None,
+                               error_from_response=common_header_errors, copy_request=False,
+                               **kwargs)
+
+    def modify_choreography_info(self, seq_name, add_labels=[], remove_labels=[], **kwargs):
+        """Modifies a sequence's ChoreographyInfo field to remove or 
+        add any labels attached to the sequence.
+        
+        Returns:
+            The full ModifyChoreographyInfoResponse proto."""
+        request = self.build_modify_choreography_info_request(seq_name, add_labels, remove_labels)
+        return self.call(self._stub.ModifyChoreographyInfo, request, value_from_response=None,
+                         error_from_response=common_header_errors, copy_request=False, **kwargs)
+
+    def modify_choreography_info_async(self, seq_name, add_labels=[], remove_labels=[], **kwargs):
+        """Async version of modify_choreography_info()."""
+        request = self.build_modify_choreography_info_request(seq_name, add_labels, remove_labels)
+        return self.call_async(self._stub.ModifyChoreographyInfo, request, value_from_response=None,
+                               error_from_response=common_header_errors, copy_request=False,
+                               **kwargs)
+
+    def clear_all_sequence_files(self, **kwargs):
+        """Completely clears all choreography files that are saved on the robot,
+        including animation proto files. 
+        
+        Returns:
+            The full ClearAllSequenceFilesResponse proto."""
+        request = choreography_sequence_pb2.ClearAllSequenceFilesRequest()
+        return self.call(self._stub.ClearAllSequenceFiles, request, value_from_response=None,
+                         error_from_response=common_header_errors, copy_request=False, **kwargs)
+
+    def clear_all_sequence_files_async(self, **kwargs):
+        """Async version of clear_all_sequence_files()."""
+        request = choreography_sequence_pb2.ClearAllSequenceFilesRequest()
+        return self.call_async(self._stub.ClearAllSequenceFiles, request, value_from_response=None,
+                               error_from_response=common_header_errors, copy_request=False,
+                               **kwargs)
+
 
     @staticmethod
     def build_start_recording_state_request(duration_seconds=None, continue_session_id=0):
         """Generate a StartRecordingStateRequest proto.
 
         Args:
             duration_seconds (float): The duration of the recording request in seconds. This will
@@ -482,14 +596,35 @@
             choreography_sequence_name=choreography_name,
             choreography_starting_slice=float(choreography_starting_slice), lease=lease)
         if client_start_time is not None:
             request.start_time.CopyFrom(
                 self._update_timestamp_filter(client_start_time, self.timesync_endpoint))
         return request
 
+    def build_choreography_command_request(self, command_list, client_end_time, lease=None):
+        req = choreography_sequence_pb2.ChoreographyCommandRequest(
+            lease=lease,
+            command_end_time=self._update_timestamp_filter(client_end_time, self.timesync_endpoint))
+        # Python list to repeated proto.
+        req.commands.extend(command_list)
+        return req
+
+    def build_save_sequence_request(self, sequence_name, labels=[]):
+        request = choreography_sequence_pb2.SaveSequenceRequest(sequence_name=sequence_name)
+        request.add_labels.extend(labels)
+        return request
+
+    def build_modify_choreography_info_request(self, sequence_name, add_labels=[],
+                                               remove_labels=[]):
+        request = choreography_sequence_pb2.ModifyChoreographyInfoRequest(
+            sequence_name=sequence_name)
+        request.add_labels.extend(add_labels)
+        request.remove_labels.extend(remove_labels)
+        return request
+
     def _update_timestamp_filter(self, timestamp, timesync_endpoint):
         """Set or convert fields of the proto that need timestamps in the robot's clock."""
         # Input timestamp is a google.protobuf.Timestamp
         if not timesync_endpoint:
             raise NoTimeSyncError("[choreography service] No timesync endpoint set for the robot.")
         converter = _TimeConverter(self, timesync_endpoint)
         return converter.robot_timestamp_from_local_secs(timestamp)
```

## Comparing `bosdyn_choreography_client-3.2.3.dist-info/METADATA` & `bosdyn_choreography_client-3.3.0.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: bosdyn-choreography-client
-Version: 3.2.3
+Version: 3.3.0
 Summary: Boston Dynamics API client code and interfaces for choreography
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
-Requires-Dist: bosdyn-api (==3.2.3)
-Requires-Dist: bosdyn-core (==3.2.3)
-Requires-Dist: bosdyn-client (==3.2.3)
-Requires-Dist: bosdyn-choreography-protos (==3.2.3)
+Requires-Dist: bosdyn-api (==3.3.0)
+Requires-Dist: bosdyn-core (==3.3.0)
+Requires-Dist: bosdyn-client (==3.3.0)
+Requires-Dist: bosdyn-choreography-protos (==3.3.0)
 
 <!--
-Copyright (c) 2022 Boston Dynamics, Inc.  All rights reserved.
+Copyright (c) 2023 Boston Dynamics, Inc.  All rights reserved.
 
 Downloading, reproducing, distributing or otherwise using the SDK Software
 is subject to the terms and conditions of the Boston Dynamics Software
 Development Kit License (20191101-BDSDK-SL).
 -->
 
 # bosdyn-choreography-client
 
 <p align="center">
 <img src="https://www.bostondynamics.com/sites/default/files/2020-05/spot.png" style="max-width:50%;">
 </p>
 
 The bosdyn-choreography-client wheel contains client interfaces for interacting with the Boston Dynamics Choreography API. The client interfaces implement the Remote Procedure Calls (RPCs) defined in the [bosdyn-choreography-protos wheel](https://pypi.org/project/bosdyn-choreography-protos/).
-
-
```

## Comparing `bosdyn_choreography_client-3.2.3.dist-info/RECORD` & `bosdyn_choreography_client-3.3.0.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-bosdyn/__init__.py,sha256=b1r4kW1ychwGnIX1yJJwTQGUy65mcdLWgOVKLE2Fgq0,330
-bosdyn/choreography/__init__.py,sha256=b1r4kW1ychwGnIX1yJJwTQGUy65mcdLWgOVKLE2Fgq0,330
-bosdyn/choreography/client/__init__.py,sha256=b1r4kW1ychwGnIX1yJJwTQGUy65mcdLWgOVKLE2Fgq0,330
-bosdyn/choreography/client/animation_file_conversion_helpers.py,sha256=bXoyYMWDfhVrvoaUaDgRr7ghfkDpI3uKqUgAtmRoWeE,18020
-bosdyn/choreography/client/animation_file_to_proto.py,sha256=keV7M18cai8AgZE_OsGA6zlPp0lKbMW24HD3Bt1xqwI,25360
-bosdyn/choreography/client/choreography.py,sha256=YhDfvOA_dBPF2UEC_8ZPYBLcoJ-XCtVyk_ZO-CRP2a8,36272
-bosdyn_choreography_client-3.2.3.dist-info/METADATA,sha256=JCpEiYv0A48cemC6W6H-n4dwxI2tVyidXTCkWnOvIsY,1482
-bosdyn_choreography_client-3.2.3.dist-info/WHEEL,sha256=h_aVn5OB2IERUjMbi2pucmR_zzWJtk303YXvhh60NJ8,110
-bosdyn_choreography_client-3.2.3.dist-info/top_level.txt,sha256=an2OWgx1ej2jFjmBjPWNQ68ZglvUfKhmXWW-WhTtDmA,7
-bosdyn_choreography_client-3.2.3.dist-info/RECORD,,
+bosdyn/__init__.py,sha256=CMQioQKK1NlMk3kZuY49b_Aw-JyvDeOtuqOCAul1I0s,330
+bosdyn/choreography/__init__.py,sha256=CMQioQKK1NlMk3kZuY49b_Aw-JyvDeOtuqOCAul1I0s,330
+bosdyn/choreography/client/__init__.py,sha256=CMQioQKK1NlMk3kZuY49b_Aw-JyvDeOtuqOCAul1I0s,330
+bosdyn/choreography/client/animation_file_conversion_helpers.py,sha256=iBEqEGAZknyh8WWxtxZrzoA-o8BDJ7a5pmft0kqNCrs,18438
+bosdyn/choreography/client/animation_file_to_proto.py,sha256=k59cAZEYWpk648BIWaNpJirs1am1p4ziKSR2Up_sWwU,25970
+bosdyn/choreography/client/choreography.py,sha256=QMPWWkrMf6KiyPIQjqGxJFfQbSHjhtjCVYOCo4rA3rU,43561
+bosdyn_choreography_client-3.3.0.dist-info/METADATA,sha256=pHDXAd4DCAh9U-qIa6CKqnyjZyoWgu1jS3xZTKmxPz8,1646
+bosdyn_choreography_client-3.3.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+bosdyn_choreography_client-3.3.0.dist-info/top_level.txt,sha256=an2OWgx1ej2jFjmBjPWNQ68ZglvUfKhmXWW-WhTtDmA,7
+bosdyn_choreography_client-3.3.0.dist-info/RECORD,,
```

