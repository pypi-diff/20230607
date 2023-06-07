# Comparing `tmp/bosdyn_choreography_protos-3.2.3-py3-none-any.whl.zip` & `tmp/bosdyn_choreography_protos-3.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 20676 bytes, number of entries: 13
--rw-r--r--  2.0 unx       64 b- defN 23-Mar-24 15:44 bosdyn/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-24 15:44 bosdyn/api/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Mar-24 15:44 bosdyn/api/spot/__init__.py
--rw-r--r--  2.0 unx    41786 b- defN 23-Mar-24 15:44 bosdyn/api/spot/choreography_params_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/spot/choreography_params_pb2_grpc.py
--rw-r--r--  2.0 unx    46685 b- defN 23-Mar-24 15:44 bosdyn/api/spot/choreography_sequence_pb2.py
--rw-r--r--  2.0 unx      159 b- defN 23-Mar-24 15:44 bosdyn/api/spot/choreography_sequence_pb2_grpc.py
--rw-r--r--  2.0 unx     2838 b- defN 23-Mar-24 15:44 bosdyn/api/spot/choreography_service_pb2.py
--rw-r--r--  2.0 unx    24074 b- defN 23-Mar-24 15:44 bosdyn/api/spot/choreography_service_pb2_grpc.py
--rw-r--r--  2.0 unx     1378 b- defN 23-Mar-24 15:44 bosdyn_choreography_protos-3.2.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-24 15:44 bosdyn_choreography_protos-3.2.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Mar-24 15:44 bosdyn_choreography_protos-3.2.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1219 b- defN 23-Mar-24 15:44 bosdyn_choreography_protos-3.2.3.dist-info/RECORD
-13 files, 118461 bytes uncompressed, 18578 bytes compressed:  84.3%
+Zip file size: 23511 bytes, number of entries: 13
+-rw-r--r--  2.0 unx       64 b- defN 23-Jun-07 02:50 bosdyn/__init__.py
+-rw-r--r--  2.0 unx       64 b- defN 23-Jun-07 02:50 bosdyn/api/__init__.py
+-rw-r--r--  2.0 unx       64 b- defN 23-Jun-07 02:50 bosdyn/api/spot/__init__.py
+-rw-r--r--  2.0 unx    52917 b- defN 23-Jun-07 02:50 bosdyn/api/spot/choreography_params_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/spot/choreography_params_pb2_grpc.py
+-rw-r--r--  2.0 unx    53517 b- defN 23-Jun-07 02:50 bosdyn/api/spot/choreography_sequence_pb2.py
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-07 02:50 bosdyn/api/spot/choreography_sequence_pb2_grpc.py
+-rw-r--r--  2.0 unx     3109 b- defN 23-Jun-07 02:50 bosdyn/api/spot/choreography_service_pb2.py
+-rw-r--r--  2.0 unx    27930 b- defN 23-Jun-07 02:50 bosdyn/api/spot/choreography_service_pb2_grpc.py
+-rw-r--r--  2.0 unx     1542 b- defN 23-Jun-07 02:50 bosdyn_choreography_protos-3.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 02:50 bosdyn_choreography_protos-3.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-07 02:50 bosdyn_choreography_protos-3.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1221 b- defN 23-Jun-07 02:50 bosdyn_choreography_protos-3.3.0.dist-info/RECORD
+13 files, 140845 bytes uncompressed, 21413 bytes compressed:  84.8%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: bosdyn/api/spot/choreography_service_pb2.py
 Comment: 
 
 Filename: bosdyn/api/spot/choreography_service_pb2_grpc.py
 Comment: 
 
-Filename: bosdyn_choreography_protos-3.2.3.dist-info/METADATA
+Filename: bosdyn_choreography_protos-3.3.0.dist-info/METADATA
 Comment: 
 
-Filename: bosdyn_choreography_protos-3.2.3.dist-info/WHEEL
+Filename: bosdyn_choreography_protos-3.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: bosdyn_choreography_protos-3.2.3.dist-info/top_level.txt
+Filename: bosdyn_choreography_protos-3.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: bosdyn_choreography_protos-3.2.3.dist-info/RECORD
+Filename: bosdyn_choreography_protos-3.3.0.dist-info/RECORD
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

## bosdyn/api/spot/__init__.py

```diff
@@ -0,0 +1,4 @@
+00000000: 5f5f 7061 7468 5f5f 203d 205f 5f69 6d70  __path__ = __imp
+00000010: 6f72 745f 5f28 2770 6b67 7574 696c 2729  ort__('pkgutil')
+00000020: 2e65 7874 656e 645f 7061 7468 285f 5f70  .extend_path(__p
+00000030: 6174 685f 5f2c 205f 5f6e 616d 655f 5f29  ath__, __name__)
```

## bosdyn/api/spot/choreography_params_pb2.py

```diff
@@ -13,15 +13,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from bosdyn.api import geometry_pb2 as bosdyn_dot_api_dot_geometry__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)bosdyn/api/spot/choreography_params.proto\x12\x0f\x62osdyn.api.spot\x1a\x19\x62osdyn/api/geometry.proto\x1a\x1egoogle/protobuf/wrappers.proto\"\x93\x01\n\rEulerZYXValue\x12*\n\x04roll\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12+\n\x05pitch\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12)\n\x03yaw\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\x97\x01\n\x11\x45ulerRateZYXValue\x12*\n\x04roll\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12+\n\x05pitch\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12)\n\x03yaw\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\xd5\x01\n\x0e\x42odyHoldParams\x12\x30\n\x08rotation\x18\x01 \x01(\x0b\x32\x1e.bosdyn.api.spot.EulerZYXValue\x12*\n\x0btranslation\x18\x02 \x01(\x0b\x32\x15.bosdyn.api.Vec3Value\x12\x32\n\x0c\x65ntry_slices\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x31\n\x0b\x65xit_slices\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\x96\x04\n\nSwayParams\x12.\n\x08vertical\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x30\n\nhorizontal\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12*\n\x04roll\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12%\n\x05pivot\x18\x04 \x01(\x0e\x32\x16.bosdyn.api.spot.Pivot\x12\x34\n\x05style\x18\x05 \x01(\x0e\x32%.bosdyn.api.spot.SwayParams.SwayStyle\x12\x30\n\npronounced\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x32\n\x0ehold_zero_axes\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\"\xb6\x01\n\tSwayStyle\x12\x16\n\x12SWAY_STYLE_UNKNOWN\x10\x00\x12\x17\n\x13SWAY_STYLE_STANDARD\x10\x01\x12\x17\n\x13SWAY_STYLE_FAST_OUT\x10\x02\x12\x1a\n\x16SWAY_STYLE_FAST_RETURN\x10\x03\x12\x15\n\x11SWAY_STYLE_SQUARE\x10\x04\x12\x14\n\x10SWAY_STYLE_SPIKE\x10\x05\x12\x16\n\x12SWAY_STYLE_PLATEAU\x10\x06\"\x87\x03\n\rArmMoveParams\x12\x30\n\nshoulder_0\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x30\n\nshoulder_1\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12-\n\x07\x65lbow_0\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12-\n\x07\x65lbow_1\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12-\n\x07wrist_0\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12-\n\x07wrist_1\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\'\n\x06\x65\x61sing\x18\x07 \x01(\x0e\x32\x17.bosdyn.api.spot.Easing\x12-\n\x07gripper\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\xb0\x02\n\x16WorkspaceArmMoveParams\x12\x30\n\x08rotation\x18\x01 \x01(\x0b\x32\x1e.bosdyn.api.spot.EulerZYXValue\x12*\n\x0btranslation\x18\x02 \x01(\x0b\x32\x15.bosdyn.api.Vec3Value\x12,\n\x08\x61\x62solute\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12,\n\x05\x66rame\x18\x04 \x01(\x0e\x32\x1d.bosdyn.api.spot.ArmMoveFrame\x12\'\n\x06\x65\x61sing\x18\x05 \x01(\x0e\x32\x17.bosdyn.api.spot.Easing\x12\x33\n\x0e\x64\x61nce_frame_id\x18\x06 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\"\xa1\x01\n\rFigure8Params\x12,\n\x06height\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12+\n\x05width\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x35\n\x0f\x62\x65\x61ts_per_cycle\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"i\n\rGripperParams\x12+\n\x05\x61ngle\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12+\n\x05speed\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\xef\x01\n\x12KneelLegMoveParams\x12+\n\x05hip_x\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12+\n\x05hip_y\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12*\n\x04knee\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12*\n\x06mirror\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\'\n\x06\x65\x61sing\x18\x05 \x01(\x0e\x32\x17.bosdyn.api.spot.Easing\"\x9d\x03\n\x13KneelLegMove2Params\x12\x30\n\nleft_hip_x\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x30\n\nleft_hip_y\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12/\n\tleft_knee\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x31\n\x0bright_hip_x\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x31\n\x0bright_hip_y\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x30\n\nright_knee\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\'\n\x06\x65\x61sing\x18\x07 \x01(\x0e\x32\x17.bosdyn.api.spot.Easing\x12\x30\n\x0clink_to_next\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\"\x9c\x03\n\x10RunningManParams\x12\'\n\x08velocity\x18\x01 \x01(\x0b\x32\x15.bosdyn.api.Vec2Value\x12\x32\n\x0cswing_height\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12,\n\x06spread\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12+\n\x07reverse\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x34\n\x0fpre_move_cycles\x18\x05 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\x12\x36\n\x10speed_multiplier\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x30\n\nduty_cycle\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x30\n\ncom_height\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\x96\x01\n\tHopParams\x12\'\n\x08velocity\x18\x01 \x01(\x0b\x32\x15.bosdyn.api.Vec2Value\x12.\n\x08yaw_rate\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x30\n\nstand_time\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\x9d\x02\n\x12RandomRotateParams\x12\x31\n\tamplitude\x18\x01 \x01(\x0b\x32\x1e.bosdyn.api.spot.EulerZYXValue\x12\x31\n\x05speed\x18\x02 \x01(\x0b\x32\".bosdyn.api.spot.EulerRateZYXValue\x12\x35\n\x0fspeed_variation\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x34\n\x0fnum_speed_tiers\x18\x04 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\x12\x34\n\x0etier_variation\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\xd3\x01\n\x0b\x43rawlParams\x12\x32\n\x0cswing_slices\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\'\n\x08velocity\x18\x02 \x01(\x0b\x32\x15.bosdyn.api.Vec2Value\x12\x32\n\x0cstance_width\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x33\n\rstance_length\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\x95\x02\n\nGotoParams\x12\x30\n\x11\x61\x62solute_position\x18\x01 \x01(\x0b\x32\x15.bosdyn.api.Vec2Value\x12\x32\n\x0c\x61\x62solute_yaw\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12=\n\x17step_position_stiffness\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x30\n\nduty_cycle\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x30\n\x0clink_to_next\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\"\x9d\x01\n\rBourreeParams\x12\'\n\x08velocity\x18\x01 \x01(\x0b\x32\x15.bosdyn.api.Vec2Value\x12.\n\x08yaw_rate\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x33\n\rstance_length\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"u\n\nSideParams\x12.\n\x04side\x18\x01 \x01(\x0e\x32 .bosdyn.api.spot.SideParams.Side\"7\n\x04Side\x12\x10\n\x0cSIDE_UNKNOWN\x10\x00\x12\r\n\tSIDE_LEFT\x10\x01\x12\x0e\n\nSIDE_RIGHT\x10\x02\"\x98\x06\n\nJumpParams\x12)\n\x03yaw\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x33\n\rflight_slices\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x32\n\x0cstance_width\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x33\n\rstance_length\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12*\n\x0btranslation\x18\x06 \x01(\x0b\x32\x15.bosdyn.api.Vec2Value\x12\x34\n\x0esplit_fraction\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x37\n\rlead_leg_pair\x18\x08 \x01(\x0e\x32 .bosdyn.api.spot.JumpParams.Lead\x12\x33\n\x0fyaw_is_absolute\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12;\n\x17translation_is_absolute\x18\x0c \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x32\n\x0c\x61\x62solute_yaw\x18\t \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x33\n\x14\x61\x62solute_translation\x18\n \x01(\x0b\x32\x15.bosdyn.api.Vec2Value\x12\x32\n\x0cswing_height\x18\r \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x30\n\x08\x61\x62solute\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValueB\x02\x18\x01\"e\n\x04Lead\x12\x10\n\x0cLEAD_UNKNOWN\x10\x00\x12\r\n\tLEAD_AUTO\x10\x01\x12\x0e\n\nLEAD_FRONT\x10\x02\x12\r\n\tLEAD_HIND\x10\x03\x12\r\n\tLEAD_LEFT\x10\x04\x12\x0e\n\nLEAD_RIGHT\x10\x05\"\xf1\x04\n\nStepParams\x12\"\n\x04\x66oot\x18\x01 \x01(\x0e\x32\x14.bosdyn.api.spot.Leg\x12%\n\x06offset\x18\x02 \x01(\x0b\x32\x15.bosdyn.api.Vec2Value\x12)\n\x0bsecond_foot\x18\x03 \x01(\x0e\x32\x14.bosdyn.api.spot.Leg\x12-\n\x0eswing_waypoint\x18\x05 \x01(\x0b\x32\x15.bosdyn.api.Vec3Value\x12\x32\n\x0cswing_height\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x36\n\x10liftoff_velocity\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x38\n\x12touchdown_velocity\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12,\n\x08mirror_x\x18\t \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12,\n\x08mirror_y\x18\n \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12.\n\x06mirror\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.BoolValueB\x02\x18\x01\x12\x34\n\x0ewaypoint_dwell\x18\x0b \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12)\n\x05touch\x18\x0c \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12+\n\x0ctouch_offset\x18\r \x01(\x0b\x32\x15.bosdyn.api.Vec2Value\"~\n\x10RotateBodyParams\x12\x30\n\x08rotation\x18\x01 \x01(\x0b\x32\x1e.bosdyn.api.spot.EulerZYXValue\x12\x38\n\x14return_to_start_pose\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\"\xbd\x02\n\x10\x42uttCircleParams\x12,\n\x06radius\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x36\n\x10\x62\x65\x61ts_per_circle\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x37\n\x11number_of_circles\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12%\n\x05pivot\x18\x04 \x01(\x0e\x32\x16.bosdyn.api.spot.Pivot\x12-\n\tclockwise\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x34\n\x0estarting_angle\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\";\n\x0bTwerkParams\x12,\n\x06height\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\xcb\x03\n\nTurnParams\x12)\n\x03yaw\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x32\n\x0c\x61\x62solute_yaw\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x33\n\x0fyaw_is_absolute\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x32\n\x0cswing_height\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x34\n\x0eswing_velocity\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12%\n\x06motion\x18\x07 \x01(\x0b\x32\x15.bosdyn.api.Vec2Value\x12.\n\x0f\x61\x62solute_motion\x18\x08 \x01(\x0b\x32\x15.bosdyn.api.Vec2Value\x12\x36\n\x12motion_is_absolute\x18\t \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x30\n\x08\x61\x62solute\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.BoolValueB\x02\x18\x01\"\xcc\x03\n\x0fPace2StepParams\x12%\n\x06motion\x18\x01 \x01(\x0b\x32\x15.bosdyn.api.Vec2Value\x12.\n\x0f\x61\x62solute_motion\x18\x06 \x01(\x0b\x32\x15.bosdyn.api.Vec2Value\x12\x36\n\x12motion_is_absolute\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x32\n\x0cswing_height\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x34\n\x0eswing_velocity\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12)\n\x03yaw\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x32\n\x0c\x61\x62solute_yaw\x18\t \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x33\n\x0fyaw_is_absolute\x18\n \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12,\n\x08\x61\x62solute\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\"\xa3\x01\n\x11\x43hickenHeadParams\x12,\n\rbob_magnitude\x18\x01 \x01(\x0b\x32\x15.bosdyn.api.Vec3Value\x12\x34\n\x0f\x62\x65\x61ts_per_cycle\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\x12*\n\x06\x66ollow\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\"\xc1\x01\n\nClapParams\x12(\n\tdirection\x18\x01 \x01(\x0b\x32\x15.bosdyn.api.Vec3Value\x12\'\n\x08location\x18\x02 \x01(\x0b\x32\x15.bosdyn.api.Vec3Value\x12+\n\x05speed\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x33\n\rclap_distance\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\xb5\x02\n\x11KneelCircleParams\x12\'\n\x08location\x18\x01 \x01(\x0b\x32\x15.bosdyn.api.Vec3Value\x12\x35\n\x10\x62\x65\x61ts_per_circle\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\x12\x37\n\x11number_of_circles\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12,\n\x06offset\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12,\n\x06radius\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12+\n\x07reverse\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\";\n\rFrontUpParams\x12*\n\x06mirror\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\"\xd3\x07\n\x11\x46idgetStandParams\x12?\n\x06preset\x18\x01 \x01(\x0e\x32/.bosdyn.api.spot.FidgetStandParams.FidgetPreset\x12\x34\n\x0emin_gaze_pitch\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x34\n\x0emax_gaze_pitch\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x36\n\x10gaze_mean_period\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12.\n\x0fgaze_center_cfp\x18\x05 \x01(\x0b\x32\x15.bosdyn.api.Vec3Value\x12\x37\n\x11shift_mean_period\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12?\n\x19shift_max_transition_time\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x32\n\x0c\x62reath_min_z\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x32\n\x0c\x62reath_max_z\x18\t \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x37\n\x11\x62reath_max_period\x18\n \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12=\n\x17leg_gesture_mean_period\x18\x0b \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x34\n\x0egaze_slew_rate\x18\x0c \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12<\n\x1dgaze_position_generation_gain\x18\r \x01(\x0b\x32\x15.bosdyn.api.Vec3Value\x12?\n\x19gaze_roll_generation_gain\x18\x0e \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\x99\x01\n\x0c\x46idgetPreset\x12\x12\n\x0ePRESET_UNKNOWN\x10\x00\x12\x11\n\rPRESET_CUSTOM\x10\x01\x12\x13\n\x0fPRESET_INTEREST\x10\x02\x12\x12\n\x0ePRESET_PLAYFUL\x10\x03\x12\x0f\n\x0bPRESET_FEAR\x10\x04\x12\x12\n\x0ePRESET_NERVOUS\x10\x05\x12\x14\n\x10PRESET_EXHAUSTED\x10\x06\"\xd8\x04\n\x13\x46rameSnapshotParams\x12-\n\x08\x66rame_id\x18\x01 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\x12\x34\n\x0f\x66iducial_number\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\x12N\n\x16include_front_left_leg\x18\x03 \x01(\x0e\x32..bosdyn.api.spot.FrameSnapshotParams.Inclusion\x12O\n\x17include_front_right_leg\x18\x04 \x01(\x0e\x32..bosdyn.api.spot.FrameSnapshotParams.Inclusion\x12M\n\x15include_hind_left_leg\x18\x05 \x01(\x0e\x32..bosdyn.api.spot.FrameSnapshotParams.Inclusion\x12N\n\x16include_hind_right_leg\x18\x06 \x01(\x0e\x32..bosdyn.api.spot.FrameSnapshotParams.Inclusion\x12/\n\x0b\x63ompensated\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\"k\n\tInclusion\x12\x15\n\x11INCLUSION_UNKNOWN\x10\x00\x12\x17\n\x13INCLUSION_IF_STANCE\x10\x01\x12\x16\n\x12INCLUSION_INCLUDED\x10\x02\x12\x16\n\x12INCLUSION_EXCLUDED\x10\x03\"\x8e\x02\n\x0eSetColorParams\x12*\n\nleft_color\x18\x01 \x01(\x0b\x32\x16.bosdyn.api.spot.Color\x12\x36\n\x12right_same_as_left\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12+\n\x0bright_color\x18\x03 \x01(\x0b\x32\x16.bosdyn.api.spot.Color\x12\x34\n\x0e\x66\x61\x64\x65_in_slices\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x35\n\x0f\x66\x61\x64\x65_out_slices\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\xd7\x01\n\x0f\x46\x61\x64\x65\x43olorParams\x12)\n\ttop_color\x18\x01 \x01(\x0b\x32\x16.bosdyn.api.spot.Color\x12,\n\x0c\x62ottom_color\x18\x02 \x01(\x0b\x32\x16.bosdyn.api.spot.Color\x12\x34\n\x0e\x66\x61\x64\x65_in_slices\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x35\n\x0f\x66\x61\x64\x65_out_slices\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\xf7\x03\n\x16IndependentColorParams\x12(\n\x08top_left\x18\x01 \x01(\x0b\x32\x16.bosdyn.api.spot.Color\x12.\n\x0eupper_mid_left\x18\x02 \x01(\x0b\x32\x16.bosdyn.api.spot.Color\x12.\n\x0elower_mid_left\x18\x03 \x01(\x0b\x32\x16.bosdyn.api.spot.Color\x12+\n\x0b\x62ottom_left\x18\x04 \x01(\x0b\x32\x16.bosdyn.api.spot.Color\x12)\n\ttop_right\x18\x05 \x01(\x0b\x32\x16.bosdyn.api.spot.Color\x12/\n\x0fupper_mid_right\x18\x06 \x01(\x0b\x32\x16.bosdyn.api.spot.Color\x12/\n\x0flower_mid_right\x18\x07 \x01(\x0b\x32\x16.bosdyn.api.spot.Color\x12,\n\x0c\x62ottom_right\x18\x08 \x01(\x0b\x32\x16.bosdyn.api.spot.Color\x12\x34\n\x0e\x66\x61\x64\x65_in_slices\x18\t \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x35\n\x0f\x66\x61\x64\x65_out_slices\x18\n \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\x8b\x01\n\x05\x43olor\x12)\n\x03red\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12+\n\x05green\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12*\n\x04\x62lue\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\xbe\x04\n\x11RippleColorParams\x12$\n\x04main\x18\x01 \x01(\x0b\x32\x16.bosdyn.api.spot.Color\x12)\n\tsecondary\x18\x02 \x01(\x0b\x32\x16.bosdyn.api.spot.Color\x12;\n\x07pattern\x18\x03 \x01(\x0e\x32*.bosdyn.api.spot.RippleColorParams.Pattern\x12@\n\nlight_side\x18\x04 \x01(\x0e\x32,.bosdyn.api.spot.RippleColorParams.LightSide\x12\x36\n\x10increment_slices\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\x90\x01\n\x07Pattern\x12\x13\n\x0fPATTERN_UNKNOWN\x10\x00\x12\x14\n\x10PATTERN_FLASHING\x10\x01\x12\x11\n\rPATTERN_SNAKE\x10\x02\x12\x1c\n\x18PATTERN_ALTERNATE_COLORS\x10\x03\x12)\n%PATTERN_FINE_GRAINED_ALTERNATE_COLORS\x10\x04\"\x8d\x01\n\tLightSide\x12\x16\n\x12LIGHT_SIDE_UNKNOWN\x10\x00\x12\x13\n\x0fLIGHT_SIDE_LEFT\x10\x01\x12\x14\n\x10LIGHT_SIDE_RIGHT\x10\x02\x12\x1f\n\x1bLIGHT_SIDE_BOTH_IN_SEQUENCE\x10\x03\x12\x1c\n\x18LIGHT_SIDE_BOTH_MATCHING\x10\x04\"\x99\x08\n\rAnimateParams\x12\x16\n\x0e\x61nimation_name\x18\x01 \x01(\t\x12\x37\n\x11\x62ody_entry_slices\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x36\n\x10\x62ody_exit_slices\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x35\n\x16translation_multiplier\x18\x04 \x01(\x0b\x32\x15.bosdyn.api.Vec3Value\x12;\n\x13rotation_multiplier\x18\x05 \x01(\x0b\x32\x1e.bosdyn.api.spot.EulerZYXValue\x12\x36\n\x10\x61rm_entry_slices\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x37\n\x11shoulder_0_offset\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x37\n\x11shoulder_1_offset\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x34\n\x0e\x65lbow_0_offset\x18\t \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x34\n\x0e\x65lbow_1_offset\x18\n \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x34\n\x0ewrist_0_offset\x18\x0b \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x34\n\x0ewrist_1_offset\x18\x0c \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x34\n\x0egripper_offset\x18\r \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12+\n\x05speed\x18\x0e \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x33\n\roffset_slices\x18\x0f \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x38\n\x12gripper_multiplier\x18\x10 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12?\n\x19gripper_strength_fraction\x18\x11 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x37\n\x12\x61rm_dance_frame_id\x18\x12 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\x12=\n\x17\x62ody_tracking_stiffness\x18\x13 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue*M\n\x05Pivot\x12\x11\n\rPIVOT_UNKNOWN\x10\x00\x12\x0f\n\x0bPIVOT_FRONT\x10\x01\x12\x0e\n\nPIVOT_HIND\x10\x02\x12\x10\n\x0cPIVOT_CENTER\x10\x03*\xab\x02\n\x06\x45\x61sing\x12\x12\n\x0e\x45\x41SING_UNKNOWN\x10\x00\x12\x11\n\rEASING_LINEAR\x10\x01\x12\x1a\n\x16\x45\x41SING_QUADRATIC_INPUT\x10\x02\x12\x1b\n\x17\x45\x41SING_QUADRATIC_OUTPUT\x10\x03\x12\x1b\n\x17\x45\x41SING_QUADRATIC_IN_OUT\x10\x04\x12\x16\n\x12\x45\x41SING_CUBIC_INPUT\x10\x05\x12\x17\n\x13\x45\x41SING_CUBIC_OUTPUT\x10\x06\x12\x17\n\x13\x45\x41SING_CUBIC_IN_OUT\x10\x07\x12\x1c\n\x18\x45\x41SING_EXPONENTIAL_INPUT\x10\x08\x12\x1d\n\x19\x45\x41SING_EXPONENTIAL_OUTPUT\x10\t\x12\x1d\n\x19\x45\x41SING_EXPONENTIAL_IN_OUT\x10\n*\xd6\x01\n\x0c\x41rmMoveFrame\x12\x1a\n\x16\x41RM_MOVE_FRAME_UNKNOWN\x10\x00\x12&\n\"ARM_MOVE_FRAME_CENTER_OF_FOOTPRINT\x10\x01\x12\x17\n\x13\x41RM_MOVE_FRAME_HAND\x10\x02\x12\x17\n\x13\x41RM_MOVE_FRAME_BODY\x10\x03\x12\x1b\n\x17\x41RM_MOVE_FRAME_SHOULDER\x10\x04\x12\x19\n\x15\x41RM_MOVE_FRAME_SHADOW\x10\x05\x12\x18\n\x14\x41RM_MOVE_FRAME_DANCE\x10\x06*\x7f\n\x03Leg\x12\x0f\n\x0bLEG_UNKNOWN\x10\x00\x12\x12\n\x0eLEG_FRONT_LEFT\x10\x01\x12\x13\n\x0fLEG_FRONT_RIGHT\x10\x02\x12\x11\n\rLEG_HIND_LEFT\x10\x03\x12\x12\n\x0eLEG_HIND_RIGHT\x10\x04\x12\x17\n\nLEG_NO_LEG\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01*\xcd\x01\n\x08LedLight\x12\x15\n\x11LED_LIGHT_UNKNOWN\x10\x00\x12\x13\n\x0fLED_LIGHT_LEFT1\x10\x01\x12\x13\n\x0fLED_LIGHT_LEFT2\x10\x02\x12\x13\n\x0fLED_LIGHT_LEFT3\x10\x03\x12\x13\n\x0fLED_LIGHT_LEFT4\x10\x04\x12\x14\n\x10LED_LIGHT_RIGHT1\x10\x05\x12\x14\n\x10LED_LIGHT_RIGHT2\x10\x06\x12\x14\n\x10LED_LIGHT_RIGHT3\x10\x07\x12\x14\n\x10LED_LIGHT_RIGHT4\x10\x08\x42\x19\x42\x17\x43horeographyParamsProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)bosdyn/api/spot/choreography_params.proto\x12\x0f\x62osdyn.api.spot\x1a\x19\x62osdyn/api/geometry.proto\x1a\x1egoogle/protobuf/wrappers.proto\"4\n\x08\x45ulerZYX\x12\x0c\n\x04roll\x18\x01 \x01(\x01\x12\r\n\x05pitch\x18\x02 \x01(\x01\x12\x0b\n\x03yaw\x18\x03 \x01(\x01\"\x93\x01\n\rEulerZYXValue\x12*\n\x04roll\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12+\n\x05pitch\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12)\n\x03yaw\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\x97\x01\n\x11\x45ulerRateZYXValue\x12*\n\x04roll\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12+\n\x05pitch\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12)\n\x03yaw\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\xd5\x01\n\x0e\x42odyHoldParams\x12\x30\n\x08rotation\x18\x01 \x01(\x0b\x32\x1e.bosdyn.api.spot.EulerZYXValue\x12*\n\x0btranslation\x18\x02 \x01(\x0b\x32\x15.bosdyn.api.Vec3Value\x12\x32\n\x0c\x65ntry_slices\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x31\n\x0b\x65xit_slices\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\x96\x04\n\nSwayParams\x12.\n\x08vertical\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x30\n\nhorizontal\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12*\n\x04roll\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12%\n\x05pivot\x18\x04 \x01(\x0e\x32\x16.bosdyn.api.spot.Pivot\x12\x34\n\x05style\x18\x05 \x01(\x0e\x32%.bosdyn.api.spot.SwayParams.SwayStyle\x12\x30\n\npronounced\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x32\n\x0ehold_zero_axes\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\"\xb6\x01\n\tSwayStyle\x12\x16\n\x12SWAY_STYLE_UNKNOWN\x10\x00\x12\x17\n\x13SWAY_STYLE_STANDARD\x10\x01\x12\x17\n\x13SWAY_STYLE_FAST_OUT\x10\x02\x12\x1a\n\x16SWAY_STYLE_FAST_RETURN\x10\x03\x12\x15\n\x11SWAY_STYLE_SQUARE\x10\x04\x12\x14\n\x10SWAY_STYLE_SPIKE\x10\x05\x12\x16\n\x12SWAY_STYLE_PLATEAU\x10\x06\"\x87\x03\n\rArmMoveParams\x12\x30\n\nshoulder_0\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x30\n\nshoulder_1\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12-\n\x07\x65lbow_0\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12-\n\x07\x65lbow_1\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12-\n\x07wrist_0\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12-\n\x07wrist_1\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\'\n\x06\x65\x61sing\x18\x07 \x01(\x0e\x32\x17.bosdyn.api.spot.Easing\x12-\n\x07gripper\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\xb0\x02\n\x16WorkspaceArmMoveParams\x12\x30\n\x08rotation\x18\x01 \x01(\x0b\x32\x1e.bosdyn.api.spot.EulerZYXValue\x12*\n\x0btranslation\x18\x02 \x01(\x0b\x32\x15.bosdyn.api.Vec3Value\x12,\n\x08\x61\x62solute\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12,\n\x05\x66rame\x18\x04 \x01(\x0e\x32\x1d.bosdyn.api.spot.ArmMoveFrame\x12\'\n\x06\x65\x61sing\x18\x05 \x01(\x0e\x32\x17.bosdyn.api.spot.Easing\x12\x33\n\x0e\x64\x61nce_frame_id\x18\x06 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\"\xa1\x01\n\rFigure8Params\x12,\n\x06height\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12+\n\x05width\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x35\n\x0f\x62\x65\x61ts_per_cycle\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"i\n\rGripperParams\x12+\n\x05\x61ngle\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12+\n\x05speed\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\xef\x01\n\x12KneelLegMoveParams\x12+\n\x05hip_x\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12+\n\x05hip_y\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12*\n\x04knee\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12*\n\x06mirror\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\'\n\x06\x65\x61sing\x18\x05 \x01(\x0e\x32\x17.bosdyn.api.spot.Easing\"\x9d\x03\n\x13KneelLegMove2Params\x12\x30\n\nleft_hip_x\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x30\n\nleft_hip_y\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12/\n\tleft_knee\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x31\n\x0bright_hip_x\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x31\n\x0bright_hip_y\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x30\n\nright_knee\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\'\n\x06\x65\x61sing\x18\x07 \x01(\x0e\x32\x17.bosdyn.api.spot.Easing\x12\x30\n\x0clink_to_next\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\"\x9c\x03\n\x10RunningManParams\x12\'\n\x08velocity\x18\x01 \x01(\x0b\x32\x15.bosdyn.api.Vec2Value\x12\x32\n\x0cswing_height\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12,\n\x06spread\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12+\n\x07reverse\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x34\n\x0fpre_move_cycles\x18\x05 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\x12\x36\n\x10speed_multiplier\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x30\n\nduty_cycle\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x30\n\ncom_height\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\x96\x01\n\tHopParams\x12\'\n\x08velocity\x18\x01 \x01(\x0b\x32\x15.bosdyn.api.Vec2Value\x12.\n\x08yaw_rate\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x30\n\nstand_time\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\x9d\x02\n\x12RandomRotateParams\x12\x31\n\tamplitude\x18\x01 \x01(\x0b\x32\x1e.bosdyn.api.spot.EulerZYXValue\x12\x31\n\x05speed\x18\x02 \x01(\x0b\x32\".bosdyn.api.spot.EulerRateZYXValue\x12\x35\n\x0fspeed_variation\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x34\n\x0fnum_speed_tiers\x18\x04 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\x12\x34\n\x0etier_variation\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\xd3\x01\n\x0b\x43rawlParams\x12\x32\n\x0cswing_slices\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\'\n\x08velocity\x18\x02 \x01(\x0b\x32\x15.bosdyn.api.Vec2Value\x12\x32\n\x0cstance_width\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x33\n\rstance_length\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\x95\x02\n\nGotoParams\x12\x30\n\x11\x61\x62solute_position\x18\x01 \x01(\x0b\x32\x15.bosdyn.api.Vec2Value\x12\x32\n\x0c\x61\x62solute_yaw\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12=\n\x17step_position_stiffness\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x30\n\nduty_cycle\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x30\n\x0clink_to_next\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\"\x9d\x01\n\rBourreeParams\x12\'\n\x08velocity\x18\x01 \x01(\x0b\x32\x15.bosdyn.api.Vec2Value\x12.\n\x08yaw_rate\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x33\n\rstance_length\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"u\n\nSideParams\x12.\n\x04side\x18\x01 \x01(\x0e\x32 .bosdyn.api.spot.SideParams.Side\"7\n\x04Side\x12\x10\n\x0cSIDE_UNKNOWN\x10\x00\x12\r\n\tSIDE_LEFT\x10\x01\x12\x0e\n\nSIDE_RIGHT\x10\x02\"\x98\x06\n\nJumpParams\x12)\n\x03yaw\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x33\n\rflight_slices\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x32\n\x0cstance_width\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x33\n\rstance_length\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12*\n\x0btranslation\x18\x06 \x01(\x0b\x32\x15.bosdyn.api.Vec2Value\x12\x34\n\x0esplit_fraction\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x37\n\rlead_leg_pair\x18\x08 \x01(\x0e\x32 .bosdyn.api.spot.JumpParams.Lead\x12\x33\n\x0fyaw_is_absolute\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12;\n\x17translation_is_absolute\x18\x0c \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x32\n\x0c\x61\x62solute_yaw\x18\t \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x33\n\x14\x61\x62solute_translation\x18\n \x01(\x0b\x32\x15.bosdyn.api.Vec2Value\x12\x32\n\x0cswing_height\x18\r \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x30\n\x08\x61\x62solute\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValueB\x02\x18\x01\"e\n\x04Lead\x12\x10\n\x0cLEAD_UNKNOWN\x10\x00\x12\r\n\tLEAD_AUTO\x10\x01\x12\x0e\n\nLEAD_FRONT\x10\x02\x12\r\n\tLEAD_HIND\x10\x03\x12\r\n\tLEAD_LEFT\x10\x04\x12\x0e\n\nLEAD_RIGHT\x10\x05\"\xf1\x04\n\nStepParams\x12\"\n\x04\x66oot\x18\x01 \x01(\x0e\x32\x14.bosdyn.api.spot.Leg\x12%\n\x06offset\x18\x02 \x01(\x0b\x32\x15.bosdyn.api.Vec2Value\x12)\n\x0bsecond_foot\x18\x03 \x01(\x0e\x32\x14.bosdyn.api.spot.Leg\x12-\n\x0eswing_waypoint\x18\x05 \x01(\x0b\x32\x15.bosdyn.api.Vec3Value\x12\x32\n\x0cswing_height\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x36\n\x10liftoff_velocity\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x38\n\x12touchdown_velocity\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12,\n\x08mirror_x\x18\t \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12,\n\x08mirror_y\x18\n \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12.\n\x06mirror\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.BoolValueB\x02\x18\x01\x12\x34\n\x0ewaypoint_dwell\x18\x0b \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12)\n\x05touch\x18\x0c \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12+\n\x0ctouch_offset\x18\r \x01(\x0b\x32\x15.bosdyn.api.Vec2Value\"~\n\x10RotateBodyParams\x12\x30\n\x08rotation\x18\x01 \x01(\x0b\x32\x1e.bosdyn.api.spot.EulerZYXValue\x12\x38\n\x14return_to_start_pose\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\"\xbd\x02\n\x10\x42uttCircleParams\x12,\n\x06radius\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x36\n\x10\x62\x65\x61ts_per_circle\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x37\n\x11number_of_circles\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12%\n\x05pivot\x18\x04 \x01(\x0e\x32\x16.bosdyn.api.spot.Pivot\x12-\n\tclockwise\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x34\n\x0estarting_angle\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\";\n\x0bTwerkParams\x12,\n\x06height\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\xcb\x03\n\nTurnParams\x12)\n\x03yaw\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x32\n\x0c\x61\x62solute_yaw\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x33\n\x0fyaw_is_absolute\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x32\n\x0cswing_height\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x34\n\x0eswing_velocity\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12%\n\x06motion\x18\x07 \x01(\x0b\x32\x15.bosdyn.api.Vec2Value\x12.\n\x0f\x61\x62solute_motion\x18\x08 \x01(\x0b\x32\x15.bosdyn.api.Vec2Value\x12\x36\n\x12motion_is_absolute\x18\t \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x30\n\x08\x61\x62solute\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.BoolValueB\x02\x18\x01\"\xcc\x03\n\x0fPace2StepParams\x12%\n\x06motion\x18\x01 \x01(\x0b\x32\x15.bosdyn.api.Vec2Value\x12.\n\x0f\x61\x62solute_motion\x18\x06 \x01(\x0b\x32\x15.bosdyn.api.Vec2Value\x12\x36\n\x12motion_is_absolute\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x32\n\x0cswing_height\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x34\n\x0eswing_velocity\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12)\n\x03yaw\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x32\n\x0c\x61\x62solute_yaw\x18\t \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x33\n\x0fyaw_is_absolute\x18\n \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12,\n\x08\x61\x62solute\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\"\xa3\x01\n\x11\x43hickenHeadParams\x12,\n\rbob_magnitude\x18\x01 \x01(\x0b\x32\x15.bosdyn.api.Vec3Value\x12\x34\n\x0f\x62\x65\x61ts_per_cycle\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\x12*\n\x06\x66ollow\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\"\xc1\x01\n\nClapParams\x12(\n\tdirection\x18\x01 \x01(\x0b\x32\x15.bosdyn.api.Vec3Value\x12\'\n\x08location\x18\x02 \x01(\x0b\x32\x15.bosdyn.api.Vec3Value\x12+\n\x05speed\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x33\n\rclap_distance\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\xb5\x02\n\x11KneelCircleParams\x12\'\n\x08location\x18\x01 \x01(\x0b\x32\x15.bosdyn.api.Vec3Value\x12\x35\n\x10\x62\x65\x61ts_per_circle\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\x12\x37\n\x11number_of_circles\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12,\n\x06offset\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12,\n\x06radius\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12+\n\x07reverse\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\";\n\rFrontUpParams\x12*\n\x06mirror\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\"\xd3\x07\n\x11\x46idgetStandParams\x12?\n\x06preset\x18\x01 \x01(\x0e\x32/.bosdyn.api.spot.FidgetStandParams.FidgetPreset\x12\x34\n\x0emin_gaze_pitch\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x34\n\x0emax_gaze_pitch\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x36\n\x10gaze_mean_period\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12.\n\x0fgaze_center_cfp\x18\x05 \x01(\x0b\x32\x15.bosdyn.api.Vec3Value\x12\x37\n\x11shift_mean_period\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12?\n\x19shift_max_transition_time\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x32\n\x0c\x62reath_min_z\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x32\n\x0c\x62reath_max_z\x18\t \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x37\n\x11\x62reath_max_period\x18\n \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12=\n\x17leg_gesture_mean_period\x18\x0b \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x34\n\x0egaze_slew_rate\x18\x0c \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12<\n\x1dgaze_position_generation_gain\x18\r \x01(\x0b\x32\x15.bosdyn.api.Vec3Value\x12?\n\x19gaze_roll_generation_gain\x18\x0e \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\x99\x01\n\x0c\x46idgetPreset\x12\x12\n\x0ePRESET_UNKNOWN\x10\x00\x12\x11\n\rPRESET_CUSTOM\x10\x01\x12\x13\n\x0fPRESET_INTEREST\x10\x02\x12\x12\n\x0ePRESET_PLAYFUL\x10\x03\x12\x0f\n\x0bPRESET_FEAR\x10\x04\x12\x12\n\x0ePRESET_NERVOUS\x10\x05\x12\x14\n\x10PRESET_EXHAUSTED\x10\x06\"\xd8\x04\n\x13\x46rameSnapshotParams\x12-\n\x08\x66rame_id\x18\x01 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\x12\x34\n\x0f\x66iducial_number\x18\x02 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\x12N\n\x16include_front_left_leg\x18\x03 \x01(\x0e\x32..bosdyn.api.spot.FrameSnapshotParams.Inclusion\x12O\n\x17include_front_right_leg\x18\x04 \x01(\x0e\x32..bosdyn.api.spot.FrameSnapshotParams.Inclusion\x12M\n\x15include_hind_left_leg\x18\x05 \x01(\x0e\x32..bosdyn.api.spot.FrameSnapshotParams.Inclusion\x12N\n\x16include_hind_right_leg\x18\x06 \x01(\x0e\x32..bosdyn.api.spot.FrameSnapshotParams.Inclusion\x12/\n\x0b\x63ompensated\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\"k\n\tInclusion\x12\x15\n\x11INCLUSION_UNKNOWN\x10\x00\x12\x17\n\x13INCLUSION_IF_STANCE\x10\x01\x12\x16\n\x12INCLUSION_INCLUDED\x10\x02\x12\x16\n\x12INCLUSION_EXCLUDED\x10\x03\"\x8e\x02\n\x0eSetColorParams\x12*\n\nleft_color\x18\x01 \x01(\x0b\x32\x16.bosdyn.api.spot.Color\x12\x36\n\x12right_same_as_left\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12+\n\x0bright_color\x18\x03 \x01(\x0b\x32\x16.bosdyn.api.spot.Color\x12\x34\n\x0e\x66\x61\x64\x65_in_slices\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x35\n\x0f\x66\x61\x64\x65_out_slices\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\xd7\x01\n\x0f\x46\x61\x64\x65\x43olorParams\x12)\n\ttop_color\x18\x01 \x01(\x0b\x32\x16.bosdyn.api.spot.Color\x12,\n\x0c\x62ottom_color\x18\x02 \x01(\x0b\x32\x16.bosdyn.api.spot.Color\x12\x34\n\x0e\x66\x61\x64\x65_in_slices\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x35\n\x0f\x66\x61\x64\x65_out_slices\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\xf7\x03\n\x16IndependentColorParams\x12(\n\x08top_left\x18\x01 \x01(\x0b\x32\x16.bosdyn.api.spot.Color\x12.\n\x0eupper_mid_left\x18\x02 \x01(\x0b\x32\x16.bosdyn.api.spot.Color\x12.\n\x0elower_mid_left\x18\x03 \x01(\x0b\x32\x16.bosdyn.api.spot.Color\x12+\n\x0b\x62ottom_left\x18\x04 \x01(\x0b\x32\x16.bosdyn.api.spot.Color\x12)\n\ttop_right\x18\x05 \x01(\x0b\x32\x16.bosdyn.api.spot.Color\x12/\n\x0fupper_mid_right\x18\x06 \x01(\x0b\x32\x16.bosdyn.api.spot.Color\x12/\n\x0flower_mid_right\x18\x07 \x01(\x0b\x32\x16.bosdyn.api.spot.Color\x12,\n\x0c\x62ottom_right\x18\x08 \x01(\x0b\x32\x16.bosdyn.api.spot.Color\x12\x34\n\x0e\x66\x61\x64\x65_in_slices\x18\t \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x35\n\x0f\x66\x61\x64\x65_out_slices\x18\n \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\x8b\x01\n\x05\x43olor\x12)\n\x03red\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12+\n\x05green\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12*\n\x04\x62lue\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\xbe\x04\n\x11RippleColorParams\x12$\n\x04main\x18\x01 \x01(\x0b\x32\x16.bosdyn.api.spot.Color\x12)\n\tsecondary\x18\x02 \x01(\x0b\x32\x16.bosdyn.api.spot.Color\x12;\n\x07pattern\x18\x03 \x01(\x0e\x32*.bosdyn.api.spot.RippleColorParams.Pattern\x12@\n\nlight_side\x18\x04 \x01(\x0e\x32,.bosdyn.api.spot.RippleColorParams.LightSide\x12\x36\n\x10increment_slices\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\x90\x01\n\x07Pattern\x12\x13\n\x0fPATTERN_UNKNOWN\x10\x00\x12\x14\n\x10PATTERN_FLASHING\x10\x01\x12\x11\n\rPATTERN_SNAKE\x10\x02\x12\x1c\n\x18PATTERN_ALTERNATE_COLORS\x10\x03\x12)\n%PATTERN_FINE_GRAINED_ALTERNATE_COLORS\x10\x04\"\x8d\x01\n\tLightSide\x12\x16\n\x12LIGHT_SIDE_UNKNOWN\x10\x00\x12\x13\n\x0fLIGHT_SIDE_LEFT\x10\x01\x12\x14\n\x10LIGHT_SIDE_RIGHT\x10\x02\x12\x1f\n\x1bLIGHT_SIDE_BOTH_IN_SEQUENCE\x10\x03\x12\x1c\n\x18LIGHT_SIDE_BOTH_MATCHING\x10\x04\"\xac\x04\n\x0eLegJointParams\x12+\n\x05\x66l_hx\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12+\n\x05\x66l_hy\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12+\n\x05\x66l_kn\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12+\n\x05\x66r_hx\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12+\n\x05\x66r_hy\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12+\n\x05\x66r_kn\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12+\n\x05hl_hx\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12+\n\x05hl_hy\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12+\n\x05hl_kn\x18\t \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12+\n\x05hr_hx\x18\n \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12+\n\x05hr_hy\x18\x0b \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12+\n\x05hr_kn\x18\x0c \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\xa0\x02\n\x0bStanceShape\x12,\n\x06length\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12+\n\x05width\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12;\n\x15\x66ront_wider_than_hind\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12<\n\x16left_longer_than_right\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12;\n\x15left_forward_of_right\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"y\n\x0bSwingPhases\x12\x33\n\rliftoff_phase\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x35\n\x0ftouchdown_phase\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\x8b\x03\n\x0bSwingParams\x12,\n\x06height\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x33\n\rliftoff_speed\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x34\n\x0evertical_speed\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12;\n\x15vertical_acceleration\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x35\n\x0foverlay_outside\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x35\n\x0foverlay_forward\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x38\n\x12low_speed_fraction\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\xfa\x01\n\x13\x41nimatedCycleParams\x12\x34\n\x0e\x61nimation_name\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12=\n\x19\x65nable_animation_duration\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x35\n\x11\x65nable_leg_timing\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x37\n\x13\x65nable_stance_shape\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\"\xc2\x13\n\x10\x43ustomGaitParams\x12+\n\x0cmax_velocity\x18\x03 \x01(\x0b\x32\x15.bosdyn.api.Vec2Value\x12\x32\n\x0cmax_yaw_rate\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12:\n\x14\x61\x63\x63\x65leration_scaling\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x34\n\x0e\x63ycle_duration\x18\x33 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12.\n\x08\x66l_swing\x18\x34 \x01(\x0b\x32\x1c.bosdyn.api.spot.SwingPhases\x12\x31\n\rtwo_fl_swings\x18\x35 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x35\n\x0fsecond_fl_swing\x18\x36 \x01(\x0b\x32\x1c.bosdyn.api.spot.SwingPhases\x12.\n\x08\x66r_swing\x18\x37 \x01(\x0b\x32\x1c.bosdyn.api.spot.SwingPhases\x12\x31\n\rtwo_fr_swings\x18\x38 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x35\n\x0fsecond_fr_swing\x18\x39 \x01(\x0b\x32\x1c.bosdyn.api.spot.SwingPhases\x12.\n\x08hl_swing\x18: \x01(\x0b\x32\x1c.bosdyn.api.spot.SwingPhases\x12\x31\n\rtwo_hl_swings\x18; \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x35\n\x0fsecond_hl_swing\x18< \x01(\x0b\x32\x1c.bosdyn.api.spot.SwingPhases\x12.\n\x08hr_swing\x18= \x01(\x0b\x32\x1c.bosdyn.api.spot.SwingPhases\x12\x31\n\rtwo_hr_swings\x18> \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x35\n\x0fsecond_hr_swing\x18? \x01(\x0b\x32\x1c.bosdyn.api.spot.SwingPhases\x12\x35\n\x11show_stance_shape\x18\n \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x32\n\x0cstance_shape\x18\x0b \x01(\x0b\x32\x1c.bosdyn.api.spot.StanceShape\x12\x30\n\ncom_height\x18\x14 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x36\n\x17\x62ody_translation_offset\x18\x15 \x01(\x0b\x32\x15.bosdyn.api.Vec3Value\x12<\n\x14\x62ody_rotation_offset\x18\x16 \x01(\x0b\x32\x1e.bosdyn.api.spot.EulerZYXValue\x12=\n\x17low_speed_body_fraction\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12:\n\x14general_swing_params\x18P \x01(\x0b\x32\x1c.bosdyn.api.spot.SwingParams\x12\x37\n\x13use_fl_swing_params\x18Q \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x35\n\x0f\x66l_swing_params\x18R \x01(\x0b\x32\x1c.bosdyn.api.spot.SwingParams\x12\x37\n\x13use_fr_swing_params\x18S \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x35\n\x0f\x66r_swing_params\x18T \x01(\x0b\x32\x1c.bosdyn.api.spot.SwingParams\x12\x37\n\x13use_hl_swing_params\x18U \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x35\n\x0fhl_swing_params\x18V \x01(\x0b\x32\x1c.bosdyn.api.spot.SwingParams\x12\x37\n\x13use_hr_swing_params\x18W \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x35\n\x0fhr_swing_params\x18X \x01(\x0b\x32\x1c.bosdyn.api.spot.SwingParams\x12\x32\n\x0estand_in_place\x18Z \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x39\n\x15standard_final_stance\x18[ \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x39\n\x15show_stability_params\x18\x64 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12(\n\x02mu\x18\x65 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x36\n\x10timing_stiffness\x18\x66 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12=\n\x17step_position_stiffness\x18g \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12I\n$enable_perception_obstacle_avoidance\x18\x82\x01 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x41\n\x1aobstacle_avoidance_padding\x18\x83\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x45\n enable_perception_terrain_height\x18\x84\x01 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x45\n enable_perception_step_placement\x18\x85\x01 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12?\n\x18maximum_stumble_distance\x18\x8c\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x37\n\x10trip_sensitivity\x18\x8d\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x44\n\x15\x61nimated_cycle_params\x18\xa1\x01 \x01(\x0b\x32$.bosdyn.api.spot.AnimatedCycleParams\"\xca\x01\n\x11\x43ustomGaitCommand\x12\x34\n\x13\x64rive_velocity_body\x18\x01 \x01(\x0b\x32\x17.bosdyn.api.SE2Velocity\x12\x10\n\x08\x66inished\x18\x02 \x01(\x08\x12\x31\n\x17\x62ody_translation_offset\x18\x03 \x01(\x0b\x32\x10.bosdyn.api.Vec3\x12:\n\x17\x62ody_orientation_offset\x18\x04 \x01(\x0b\x32\x19.bosdyn.api.spot.EulerZYX\"\xd6\x01\n\x17\x43ustomGaitCommandLimits\x12<\n\x1bmaximum_drive_velocity_body\x18\x01 \x01(\x0b\x32\x17.bosdyn.api.SE2Velocity\x12\x39\n\x1fmaximum_body_translation_offset\x18\x03 \x01(\x0b\x32\x10.bosdyn.api.Vec3\x12\x42\n\x1fmaximum_body_orientation_offset\x18\x04 \x01(\x0b\x32\x19.bosdyn.api.spot.EulerZYX\"\x99\x08\n\rAnimateParams\x12\x16\n\x0e\x61nimation_name\x18\x01 \x01(\t\x12\x37\n\x11\x62ody_entry_slices\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x36\n\x10\x62ody_exit_slices\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x35\n\x16translation_multiplier\x18\x04 \x01(\x0b\x32\x15.bosdyn.api.Vec3Value\x12;\n\x13rotation_multiplier\x18\x05 \x01(\x0b\x32\x1e.bosdyn.api.spot.EulerZYXValue\x12\x36\n\x10\x61rm_entry_slices\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x37\n\x11shoulder_0_offset\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x37\n\x11shoulder_1_offset\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x34\n\x0e\x65lbow_0_offset\x18\t \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x34\n\x0e\x65lbow_1_offset\x18\n \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x34\n\x0ewrist_0_offset\x18\x0b \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x34\n\x0ewrist_1_offset\x18\x0c \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x34\n\x0egripper_offset\x18\r \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12+\n\x05speed\x18\x0e \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x33\n\roffset_slices\x18\x0f \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x38\n\x12gripper_multiplier\x18\x10 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12?\n\x19gripper_strength_fraction\x18\x11 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x37\n\x12\x61rm_dance_frame_id\x18\x12 \x01(\x0b\x32\x1b.google.protobuf.Int32Value\x12=\n\x17\x62ody_tracking_stiffness\x18\x13 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue*M\n\x05Pivot\x12\x11\n\rPIVOT_UNKNOWN\x10\x00\x12\x0f\n\x0bPIVOT_FRONT\x10\x01\x12\x0e\n\nPIVOT_HIND\x10\x02\x12\x10\n\x0cPIVOT_CENTER\x10\x03*\xab\x02\n\x06\x45\x61sing\x12\x12\n\x0e\x45\x41SING_UNKNOWN\x10\x00\x12\x11\n\rEASING_LINEAR\x10\x01\x12\x1a\n\x16\x45\x41SING_QUADRATIC_INPUT\x10\x02\x12\x1b\n\x17\x45\x41SING_QUADRATIC_OUTPUT\x10\x03\x12\x1b\n\x17\x45\x41SING_QUADRATIC_IN_OUT\x10\x04\x12\x16\n\x12\x45\x41SING_CUBIC_INPUT\x10\x05\x12\x17\n\x13\x45\x41SING_CUBIC_OUTPUT\x10\x06\x12\x17\n\x13\x45\x41SING_CUBIC_IN_OUT\x10\x07\x12\x1c\n\x18\x45\x41SING_EXPONENTIAL_INPUT\x10\x08\x12\x1d\n\x19\x45\x41SING_EXPONENTIAL_OUTPUT\x10\t\x12\x1d\n\x19\x45\x41SING_EXPONENTIAL_IN_OUT\x10\n*\xd6\x01\n\x0c\x41rmMoveFrame\x12\x1a\n\x16\x41RM_MOVE_FRAME_UNKNOWN\x10\x00\x12&\n\"ARM_MOVE_FRAME_CENTER_OF_FOOTPRINT\x10\x01\x12\x17\n\x13\x41RM_MOVE_FRAME_HAND\x10\x02\x12\x17\n\x13\x41RM_MOVE_FRAME_BODY\x10\x03\x12\x1b\n\x17\x41RM_MOVE_FRAME_SHOULDER\x10\x04\x12\x19\n\x15\x41RM_MOVE_FRAME_SHADOW\x10\x05\x12\x18\n\x14\x41RM_MOVE_FRAME_DANCE\x10\x06*\x7f\n\x03Leg\x12\x0f\n\x0bLEG_UNKNOWN\x10\x00\x12\x12\n\x0eLEG_FRONT_LEFT\x10\x01\x12\x13\n\x0fLEG_FRONT_RIGHT\x10\x02\x12\x11\n\rLEG_HIND_LEFT\x10\x03\x12\x12\n\x0eLEG_HIND_RIGHT\x10\x04\x12\x17\n\nLEG_NO_LEG\x10\xff\xff\xff\xff\xff\xff\xff\xff\xff\x01*\xcd\x01\n\x08LedLight\x12\x15\n\x11LED_LIGHT_UNKNOWN\x10\x00\x12\x13\n\x0fLED_LIGHT_LEFT1\x10\x01\x12\x13\n\x0fLED_LIGHT_LEFT2\x10\x02\x12\x13\n\x0fLED_LIGHT_LEFT3\x10\x03\x12\x13\n\x0fLED_LIGHT_LEFT4\x10\x04\x12\x14\n\x10LED_LIGHT_RIGHT1\x10\x05\x12\x14\n\x10LED_LIGHT_RIGHT2\x10\x06\x12\x14\n\x10LED_LIGHT_RIGHT3\x10\x07\x12\x14\n\x10LED_LIGHT_RIGHT4\x10\x08\x42\x19\x42\x17\x43horeographyParamsProtob\x06proto3')
 
 _PIVOT = DESCRIPTOR.enum_types_by_name['Pivot']
 Pivot = enum_type_wrapper.EnumTypeWrapper(_PIVOT)
 _EASING = DESCRIPTOR.enum_types_by_name['Easing']
 Easing = enum_type_wrapper.EnumTypeWrapper(_EASING)
 _ARMMOVEFRAME = DESCRIPTOR.enum_types_by_name['ArmMoveFrame']
 ArmMoveFrame = enum_type_wrapper.EnumTypeWrapper(_ARMMOVEFRAME)
@@ -64,14 +64,15 @@
 LED_LIGHT_LEFT4 = 4
 LED_LIGHT_RIGHT1 = 5
 LED_LIGHT_RIGHT2 = 6
 LED_LIGHT_RIGHT3 = 7
 LED_LIGHT_RIGHT4 = 8
 
 
+_EULERZYX = DESCRIPTOR.message_types_by_name['EulerZYX']
 _EULERZYXVALUE = DESCRIPTOR.message_types_by_name['EulerZYXValue']
 _EULERRATEZYXVALUE = DESCRIPTOR.message_types_by_name['EulerRateZYXValue']
 _BODYHOLDPARAMS = DESCRIPTOR.message_types_by_name['BodyHoldParams']
 _SWAYPARAMS = DESCRIPTOR.message_types_by_name['SwayParams']
 _ARMMOVEPARAMS = DESCRIPTOR.message_types_by_name['ArmMoveParams']
 _WORKSPACEARMMOVEPARAMS = DESCRIPTOR.message_types_by_name['WorkspaceArmMoveParams']
 _FIGURE8PARAMS = DESCRIPTOR.message_types_by_name['Figure8Params']
@@ -99,22 +100,37 @@
 _FIDGETSTANDPARAMS = DESCRIPTOR.message_types_by_name['FidgetStandParams']
 _FRAMESNAPSHOTPARAMS = DESCRIPTOR.message_types_by_name['FrameSnapshotParams']
 _SETCOLORPARAMS = DESCRIPTOR.message_types_by_name['SetColorParams']
 _FADECOLORPARAMS = DESCRIPTOR.message_types_by_name['FadeColorParams']
 _INDEPENDENTCOLORPARAMS = DESCRIPTOR.message_types_by_name['IndependentColorParams']
 _COLOR = DESCRIPTOR.message_types_by_name['Color']
 _RIPPLECOLORPARAMS = DESCRIPTOR.message_types_by_name['RippleColorParams']
+_LEGJOINTPARAMS = DESCRIPTOR.message_types_by_name['LegJointParams']
+_STANCESHAPE = DESCRIPTOR.message_types_by_name['StanceShape']
+_SWINGPHASES = DESCRIPTOR.message_types_by_name['SwingPhases']
+_SWINGPARAMS = DESCRIPTOR.message_types_by_name['SwingParams']
+_ANIMATEDCYCLEPARAMS = DESCRIPTOR.message_types_by_name['AnimatedCycleParams']
+_CUSTOMGAITPARAMS = DESCRIPTOR.message_types_by_name['CustomGaitParams']
+_CUSTOMGAITCOMMAND = DESCRIPTOR.message_types_by_name['CustomGaitCommand']
+_CUSTOMGAITCOMMANDLIMITS = DESCRIPTOR.message_types_by_name['CustomGaitCommandLimits']
 _ANIMATEPARAMS = DESCRIPTOR.message_types_by_name['AnimateParams']
 _SWAYPARAMS_SWAYSTYLE = _SWAYPARAMS.enum_types_by_name['SwayStyle']
 _SIDEPARAMS_SIDE = _SIDEPARAMS.enum_types_by_name['Side']
 _JUMPPARAMS_LEAD = _JUMPPARAMS.enum_types_by_name['Lead']
 _FIDGETSTANDPARAMS_FIDGETPRESET = _FIDGETSTANDPARAMS.enum_types_by_name['FidgetPreset']
 _FRAMESNAPSHOTPARAMS_INCLUSION = _FRAMESNAPSHOTPARAMS.enum_types_by_name['Inclusion']
 _RIPPLECOLORPARAMS_PATTERN = _RIPPLECOLORPARAMS.enum_types_by_name['Pattern']
 _RIPPLECOLORPARAMS_LIGHTSIDE = _RIPPLECOLORPARAMS.enum_types_by_name['LightSide']
+EulerZYX = _reflection.GeneratedProtocolMessageType('EulerZYX', (_message.Message,), {
+  'DESCRIPTOR' : _EULERZYX,
+  '__module__' : 'bosdyn.api.spot.choreography_params_pb2'
+  # @@protoc_insertion_point(class_scope:bosdyn.api.spot.EulerZYX)
+  })
+_sym_db.RegisterMessage(EulerZYX)
+
 EulerZYXValue = _reflection.GeneratedProtocolMessageType('EulerZYXValue', (_message.Message,), {
   'DESCRIPTOR' : _EULERZYXVALUE,
   '__module__' : 'bosdyn.api.spot.choreography_params_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.spot.EulerZYXValue)
   })
 _sym_db.RegisterMessage(EulerZYXValue)
 
@@ -352,14 +368,70 @@
 RippleColorParams = _reflection.GeneratedProtocolMessageType('RippleColorParams', (_message.Message,), {
   'DESCRIPTOR' : _RIPPLECOLORPARAMS,
   '__module__' : 'bosdyn.api.spot.choreography_params_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.spot.RippleColorParams)
   })
 _sym_db.RegisterMessage(RippleColorParams)
 
+LegJointParams = _reflection.GeneratedProtocolMessageType('LegJointParams', (_message.Message,), {
+  'DESCRIPTOR' : _LEGJOINTPARAMS,
+  '__module__' : 'bosdyn.api.spot.choreography_params_pb2'
+  # @@protoc_insertion_point(class_scope:bosdyn.api.spot.LegJointParams)
+  })
+_sym_db.RegisterMessage(LegJointParams)
+
+StanceShape = _reflection.GeneratedProtocolMessageType('StanceShape', (_message.Message,), {
+  'DESCRIPTOR' : _STANCESHAPE,
+  '__module__' : 'bosdyn.api.spot.choreography_params_pb2'
+  # @@protoc_insertion_point(class_scope:bosdyn.api.spot.StanceShape)
+  })
+_sym_db.RegisterMessage(StanceShape)
+
+SwingPhases = _reflection.GeneratedProtocolMessageType('SwingPhases', (_message.Message,), {
+  'DESCRIPTOR' : _SWINGPHASES,
+  '__module__' : 'bosdyn.api.spot.choreography_params_pb2'
+  # @@protoc_insertion_point(class_scope:bosdyn.api.spot.SwingPhases)
+  })
+_sym_db.RegisterMessage(SwingPhases)
+
+SwingParams = _reflection.GeneratedProtocolMessageType('SwingParams', (_message.Message,), {
+  'DESCRIPTOR' : _SWINGPARAMS,
+  '__module__' : 'bosdyn.api.spot.choreography_params_pb2'
+  # @@protoc_insertion_point(class_scope:bosdyn.api.spot.SwingParams)
+  })
+_sym_db.RegisterMessage(SwingParams)
+
+AnimatedCycleParams = _reflection.GeneratedProtocolMessageType('AnimatedCycleParams', (_message.Message,), {
+  'DESCRIPTOR' : _ANIMATEDCYCLEPARAMS,
+  '__module__' : 'bosdyn.api.spot.choreography_params_pb2'
+  # @@protoc_insertion_point(class_scope:bosdyn.api.spot.AnimatedCycleParams)
+  })
+_sym_db.RegisterMessage(AnimatedCycleParams)
+
+CustomGaitParams = _reflection.GeneratedProtocolMessageType('CustomGaitParams', (_message.Message,), {
+  'DESCRIPTOR' : _CUSTOMGAITPARAMS,
+  '__module__' : 'bosdyn.api.spot.choreography_params_pb2'
+  # @@protoc_insertion_point(class_scope:bosdyn.api.spot.CustomGaitParams)
+  })
+_sym_db.RegisterMessage(CustomGaitParams)
+
+CustomGaitCommand = _reflection.GeneratedProtocolMessageType('CustomGaitCommand', (_message.Message,), {
+  'DESCRIPTOR' : _CUSTOMGAITCOMMAND,
+  '__module__' : 'bosdyn.api.spot.choreography_params_pb2'
+  # @@protoc_insertion_point(class_scope:bosdyn.api.spot.CustomGaitCommand)
+  })
+_sym_db.RegisterMessage(CustomGaitCommand)
+
+CustomGaitCommandLimits = _reflection.GeneratedProtocolMessageType('CustomGaitCommandLimits', (_message.Message,), {
+  'DESCRIPTOR' : _CUSTOMGAITCOMMANDLIMITS,
+  '__module__' : 'bosdyn.api.spot.choreography_params_pb2'
+  # @@protoc_insertion_point(class_scope:bosdyn.api.spot.CustomGaitCommandLimits)
+  })
+_sym_db.RegisterMessage(CustomGaitCommandLimits)
+
 AnimateParams = _reflection.GeneratedProtocolMessageType('AnimateParams', (_message.Message,), {
   'DESCRIPTOR' : _ANIMATEPARAMS,
   '__module__' : 'bosdyn.api.spot.choreography_params_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.spot.AnimateParams)
   })
 _sym_db.RegisterMessage(AnimateParams)
 
@@ -369,104 +441,122 @@
   DESCRIPTOR._serialized_options = b'B\027ChoreographyParamsProto'
   _JUMPPARAMS.fields_by_name['absolute']._options = None
   _JUMPPARAMS.fields_by_name['absolute']._serialized_options = b'\030\001'
   _STEPPARAMS.fields_by_name['mirror']._options = None
   _STEPPARAMS.fields_by_name['mirror']._serialized_options = b'\030\001'
   _TURNPARAMS.fields_by_name['absolute']._options = None
   _TURNPARAMS.fields_by_name['absolute']._serialized_options = b'\030\001'
-  _PIVOT._serialized_start=12382
-  _PIVOT._serialized_end=12459
-  _EASING._serialized_start=12462
-  _EASING._serialized_end=12761
-  _ARMMOVEFRAME._serialized_start=12764
-  _ARMMOVEFRAME._serialized_end=12978
-  _LEG._serialized_start=12980
-  _LEG._serialized_end=13107
-  _LEDLIGHT._serialized_start=13110
-  _LEDLIGHT._serialized_end=13315
-  _EULERZYXVALUE._serialized_start=122
-  _EULERZYXVALUE._serialized_end=269
-  _EULERRATEZYXVALUE._serialized_start=272
-  _EULERRATEZYXVALUE._serialized_end=423
-  _BODYHOLDPARAMS._serialized_start=426
-  _BODYHOLDPARAMS._serialized_end=639
-  _SWAYPARAMS._serialized_start=642
-  _SWAYPARAMS._serialized_end=1176
-  _SWAYPARAMS_SWAYSTYLE._serialized_start=994
-  _SWAYPARAMS_SWAYSTYLE._serialized_end=1176
-  _ARMMOVEPARAMS._serialized_start=1179
-  _ARMMOVEPARAMS._serialized_end=1570
-  _WORKSPACEARMMOVEPARAMS._serialized_start=1573
-  _WORKSPACEARMMOVEPARAMS._serialized_end=1877
-  _FIGURE8PARAMS._serialized_start=1880
-  _FIGURE8PARAMS._serialized_end=2041
-  _GRIPPERPARAMS._serialized_start=2043
-  _GRIPPERPARAMS._serialized_end=2148
-  _KNEELLEGMOVEPARAMS._serialized_start=2151
-  _KNEELLEGMOVEPARAMS._serialized_end=2390
-  _KNEELLEGMOVE2PARAMS._serialized_start=2393
-  _KNEELLEGMOVE2PARAMS._serialized_end=2806
-  _RUNNINGMANPARAMS._serialized_start=2809
-  _RUNNINGMANPARAMS._serialized_end=3221
-  _HOPPARAMS._serialized_start=3224
-  _HOPPARAMS._serialized_end=3374
-  _RANDOMROTATEPARAMS._serialized_start=3377
-  _RANDOMROTATEPARAMS._serialized_end=3662
-  _CRAWLPARAMS._serialized_start=3665
-  _CRAWLPARAMS._serialized_end=3876
-  _GOTOPARAMS._serialized_start=3879
-  _GOTOPARAMS._serialized_end=4156
-  _BOURREEPARAMS._serialized_start=4159
-  _BOURREEPARAMS._serialized_end=4316
-  _SIDEPARAMS._serialized_start=4318
-  _SIDEPARAMS._serialized_end=4435
-  _SIDEPARAMS_SIDE._serialized_start=4380
-  _SIDEPARAMS_SIDE._serialized_end=4435
-  _JUMPPARAMS._serialized_start=4438
-  _JUMPPARAMS._serialized_end=5230
-  _JUMPPARAMS_LEAD._serialized_start=5129
-  _JUMPPARAMS_LEAD._serialized_end=5230
-  _STEPPARAMS._serialized_start=5233
-  _STEPPARAMS._serialized_end=5858
-  _ROTATEBODYPARAMS._serialized_start=5860
-  _ROTATEBODYPARAMS._serialized_end=5986
-  _BUTTCIRCLEPARAMS._serialized_start=5989
-  _BUTTCIRCLEPARAMS._serialized_end=6306
-  _TWERKPARAMS._serialized_start=6308
-  _TWERKPARAMS._serialized_end=6367
-  _TURNPARAMS._serialized_start=6370
-  _TURNPARAMS._serialized_end=6829
-  _PACE2STEPPARAMS._serialized_start=6832
-  _PACE2STEPPARAMS._serialized_end=7292
-  _CHICKENHEADPARAMS._serialized_start=7295
-  _CHICKENHEADPARAMS._serialized_end=7458
-  _CLAPPARAMS._serialized_start=7461
-  _CLAPPARAMS._serialized_end=7654
-  _KNEELCIRCLEPARAMS._serialized_start=7657
-  _KNEELCIRCLEPARAMS._serialized_end=7966
-  _FRONTUPPARAMS._serialized_start=7968
-  _FRONTUPPARAMS._serialized_end=8027
-  _FIDGETSTANDPARAMS._serialized_start=8030
-  _FIDGETSTANDPARAMS._serialized_end=9009
-  _FIDGETSTANDPARAMS_FIDGETPRESET._serialized_start=8856
-  _FIDGETSTANDPARAMS_FIDGETPRESET._serialized_end=9009
-  _FRAMESNAPSHOTPARAMS._serialized_start=9012
-  _FRAMESNAPSHOTPARAMS._serialized_end=9612
-  _FRAMESNAPSHOTPARAMS_INCLUSION._serialized_start=9505
-  _FRAMESNAPSHOTPARAMS_INCLUSION._serialized_end=9612
-  _SETCOLORPARAMS._serialized_start=9615
-  _SETCOLORPARAMS._serialized_end=9885
-  _FADECOLORPARAMS._serialized_start=9888
-  _FADECOLORPARAMS._serialized_end=10103
-  _INDEPENDENTCOLORPARAMS._serialized_start=10106
-  _INDEPENDENTCOLORPARAMS._serialized_end=10609
-  _COLOR._serialized_start=10612
-  _COLOR._serialized_end=10751
-  _RIPPLECOLORPARAMS._serialized_start=10754
-  _RIPPLECOLORPARAMS._serialized_end=11328
-  _RIPPLECOLORPARAMS_PATTERN._serialized_start=11040
-  _RIPPLECOLORPARAMS_PATTERN._serialized_end=11184
-  _RIPPLECOLORPARAMS_LIGHTSIDE._serialized_start=11187
-  _RIPPLECOLORPARAMS_LIGHTSIDE._serialized_end=11328
-  _ANIMATEPARAMS._serialized_start=11331
-  _ANIMATEPARAMS._serialized_end=12380
+  _PIVOT._serialized_start=16983
+  _PIVOT._serialized_end=17060
+  _EASING._serialized_start=17063
+  _EASING._serialized_end=17362
+  _ARMMOVEFRAME._serialized_start=17365
+  _ARMMOVEFRAME._serialized_end=17579
+  _LEG._serialized_start=17581
+  _LEG._serialized_end=17708
+  _LEDLIGHT._serialized_start=17711
+  _LEDLIGHT._serialized_end=17916
+  _EULERZYX._serialized_start=121
+  _EULERZYX._serialized_end=173
+  _EULERZYXVALUE._serialized_start=176
+  _EULERZYXVALUE._serialized_end=323
+  _EULERRATEZYXVALUE._serialized_start=326
+  _EULERRATEZYXVALUE._serialized_end=477
+  _BODYHOLDPARAMS._serialized_start=480
+  _BODYHOLDPARAMS._serialized_end=693
+  _SWAYPARAMS._serialized_start=696
+  _SWAYPARAMS._serialized_end=1230
+  _SWAYPARAMS_SWAYSTYLE._serialized_start=1048
+  _SWAYPARAMS_SWAYSTYLE._serialized_end=1230
+  _ARMMOVEPARAMS._serialized_start=1233
+  _ARMMOVEPARAMS._serialized_end=1624
+  _WORKSPACEARMMOVEPARAMS._serialized_start=1627
+  _WORKSPACEARMMOVEPARAMS._serialized_end=1931
+  _FIGURE8PARAMS._serialized_start=1934
+  _FIGURE8PARAMS._serialized_end=2095
+  _GRIPPERPARAMS._serialized_start=2097
+  _GRIPPERPARAMS._serialized_end=2202
+  _KNEELLEGMOVEPARAMS._serialized_start=2205
+  _KNEELLEGMOVEPARAMS._serialized_end=2444
+  _KNEELLEGMOVE2PARAMS._serialized_start=2447
+  _KNEELLEGMOVE2PARAMS._serialized_end=2860
+  _RUNNINGMANPARAMS._serialized_start=2863
+  _RUNNINGMANPARAMS._serialized_end=3275
+  _HOPPARAMS._serialized_start=3278
+  _HOPPARAMS._serialized_end=3428
+  _RANDOMROTATEPARAMS._serialized_start=3431
+  _RANDOMROTATEPARAMS._serialized_end=3716
+  _CRAWLPARAMS._serialized_start=3719
+  _CRAWLPARAMS._serialized_end=3930
+  _GOTOPARAMS._serialized_start=3933
+  _GOTOPARAMS._serialized_end=4210
+  _BOURREEPARAMS._serialized_start=4213
+  _BOURREEPARAMS._serialized_end=4370
+  _SIDEPARAMS._serialized_start=4372
+  _SIDEPARAMS._serialized_end=4489
+  _SIDEPARAMS_SIDE._serialized_start=4434
+  _SIDEPARAMS_SIDE._serialized_end=4489
+  _JUMPPARAMS._serialized_start=4492
+  _JUMPPARAMS._serialized_end=5284
+  _JUMPPARAMS_LEAD._serialized_start=5183
+  _JUMPPARAMS_LEAD._serialized_end=5284
+  _STEPPARAMS._serialized_start=5287
+  _STEPPARAMS._serialized_end=5912
+  _ROTATEBODYPARAMS._serialized_start=5914
+  _ROTATEBODYPARAMS._serialized_end=6040
+  _BUTTCIRCLEPARAMS._serialized_start=6043
+  _BUTTCIRCLEPARAMS._serialized_end=6360
+  _TWERKPARAMS._serialized_start=6362
+  _TWERKPARAMS._serialized_end=6421
+  _TURNPARAMS._serialized_start=6424
+  _TURNPARAMS._serialized_end=6883
+  _PACE2STEPPARAMS._serialized_start=6886
+  _PACE2STEPPARAMS._serialized_end=7346
+  _CHICKENHEADPARAMS._serialized_start=7349
+  _CHICKENHEADPARAMS._serialized_end=7512
+  _CLAPPARAMS._serialized_start=7515
+  _CLAPPARAMS._serialized_end=7708
+  _KNEELCIRCLEPARAMS._serialized_start=7711
+  _KNEELCIRCLEPARAMS._serialized_end=8020
+  _FRONTUPPARAMS._serialized_start=8022
+  _FRONTUPPARAMS._serialized_end=8081
+  _FIDGETSTANDPARAMS._serialized_start=8084
+  _FIDGETSTANDPARAMS._serialized_end=9063
+  _FIDGETSTANDPARAMS_FIDGETPRESET._serialized_start=8910
+  _FIDGETSTANDPARAMS_FIDGETPRESET._serialized_end=9063
+  _FRAMESNAPSHOTPARAMS._serialized_start=9066
+  _FRAMESNAPSHOTPARAMS._serialized_end=9666
+  _FRAMESNAPSHOTPARAMS_INCLUSION._serialized_start=9559
+  _FRAMESNAPSHOTPARAMS_INCLUSION._serialized_end=9666
+  _SETCOLORPARAMS._serialized_start=9669
+  _SETCOLORPARAMS._serialized_end=9939
+  _FADECOLORPARAMS._serialized_start=9942
+  _FADECOLORPARAMS._serialized_end=10157
+  _INDEPENDENTCOLORPARAMS._serialized_start=10160
+  _INDEPENDENTCOLORPARAMS._serialized_end=10663
+  _COLOR._serialized_start=10666
+  _COLOR._serialized_end=10805
+  _RIPPLECOLORPARAMS._serialized_start=10808
+  _RIPPLECOLORPARAMS._serialized_end=11382
+  _RIPPLECOLORPARAMS_PATTERN._serialized_start=11094
+  _RIPPLECOLORPARAMS_PATTERN._serialized_end=11238
+  _RIPPLECOLORPARAMS_LIGHTSIDE._serialized_start=11241
+  _RIPPLECOLORPARAMS_LIGHTSIDE._serialized_end=11382
+  _LEGJOINTPARAMS._serialized_start=11385
+  _LEGJOINTPARAMS._serialized_end=11941
+  _STANCESHAPE._serialized_start=11944
+  _STANCESHAPE._serialized_end=12232
+  _SWINGPHASES._serialized_start=12234
+  _SWINGPHASES._serialized_end=12355
+  _SWINGPARAMS._serialized_start=12358
+  _SWINGPARAMS._serialized_end=12753
+  _ANIMATEDCYCLEPARAMS._serialized_start=12756
+  _ANIMATEDCYCLEPARAMS._serialized_end=13006
+  _CUSTOMGAITPARAMS._serialized_start=13009
+  _CUSTOMGAITPARAMS._serialized_end=15507
+  _CUSTOMGAITCOMMAND._serialized_start=15510
+  _CUSTOMGAITCOMMAND._serialized_end=15712
+  _CUSTOMGAITCOMMANDLIMITS._serialized_start=15715
+  _CUSTOMGAITCOMMANDLIMITS._serialized_end=15929
+  _ANIMATEPARAMS._serialized_start=15932
+  _ANIMATEPARAMS._serialized_end=16981
 # @@protoc_insertion_point(module_scope)
```

## bosdyn/api/spot/choreography_sequence_pb2.py

```diff
@@ -18,15 +18,15 @@
 from bosdyn.api import geometry_pb2 as bosdyn_dot_api_dot_geometry__pb2
 from bosdyn.api import header_pb2 as bosdyn_dot_api_dot_header__pb2
 from bosdyn.api import lease_pb2 as bosdyn_dot_api_dot_lease__pb2
 from bosdyn.api.spot import choreography_params_pb2 as bosdyn_dot_api_dot_spot_dot_choreography__params__pb2
 from bosdyn.api import data_chunk_pb2 as bosdyn_dot_api_dot_data__chunk__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n+bosdyn/api/spot/choreography_sequence.proto\x12\x0f\x62osdyn.api.spot\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x19\x62osdyn/api/geometry.proto\x1a\x17\x62osdyn/api/header.proto\x1a\x16\x62osdyn/api/lease.proto\x1a)bosdyn/api/spot/choreography_params.proto\x1a\x1b\x62osdyn/api/data_chunk.proto\"@\n\x13ListAllMovesRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"\x87\x01\n\x14ListAllMovesResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12(\n\x05moves\x18\x02 \x03(\x0b\x32\x19.bosdyn.api.spot.MoveInfo\x12\x19\n\x11move_param_config\x18\x03 \x01(\t\"D\n\x17ListAllSequencesRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"\x99\x01\n\x18ListAllSequencesResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x1b\n\x0fknown_sequences\x18\x02 \x03(\tB\x02\x18\x01\x12\x34\n\rsequence_info\x18\x03 \x03(\x0b\x32\x1d.bosdyn.api.spot.SequenceInfo\"\xe2\x01\n\x0cSequenceInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06labels\x18\x02 \x03(\t\x12=\n\x0bsaved_state\x18\x03 \x01(\x0e\x32(.bosdyn.api.spot.SequenceInfo.SavedState\"u\n\nSavedState\x12\x17\n\x13SAVED_STATE_UNKNOWN\x10\x00\x12\x19\n\x15SAVED_STATE_TEMPORARY\x10\x01\x12\x18\n\x14SAVED_STATE_RETAINED\x10\x02\x12\x19\n\x15SAVED_STATE_PERMANENT\x10\x03\"Y\n\x15\x44\x65leteSequenceRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x15\n\rsequence_name\x18\x02 \x01(\t\"\x8c\x02\n\x16\x44\x65leteSequenceResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12>\n\x06status\x18\x02 \x01(\x0e\x32..bosdyn.api.spot.DeleteSequenceResponse.Status\"\x85\x01\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1b\n\x17STATUS_UNKNOWN_SEQUENCE\x10\x02\x12\x1c\n\x18STATUS_ALREADY_TEMPORARY\x10\x03\x12\x1d\n\x19STATUS_PERMANENT_SEQUENCE\x10\x04\"k\n\x13SaveSequenceRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x15\n\rsequence_name\x18\x02 \x01(\t\x12\x12\n\nadd_labels\x18\x03 \x03(\t\"\x85\x02\n\x14SaveSequenceResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12<\n\x06status\x18\x02 \x01(\x0e\x32,.bosdyn.api.spot.SaveSequenceResponse.Status\"\x82\x01\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1b\n\x17STATUS_UNKNOWN_SEQUENCE\x10\x02\x12\x1d\n\x19STATUS_PERMANENT_SEQUENCE\x10\x03\x12\x19\n\x15STATUS_FAILED_TO_SAVE\x10\x04\"\x8c\x01\n\x1dModifyChoreographyInfoRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x15\n\rsequence_name\x18\x02 \x01(\t\x12\x12\n\nadd_labels\x18\x03 \x03(\t\x12\x15\n\rremove_labels\x18\x04 \x03(\t\"\x9b\x02\n\x1eModifyChoreographyInfoResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x46\n\x06status\x18\x02 \x01(\x0e\x32\x36.bosdyn.api.spot.ModifyChoreographyInfoResponse.Status\"\x84\x01\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1b\n\x17STATUS_UNKNOWN_SEQUENCE\x10\x02\x12\x1d\n\x19STATUS_PERMANENT_SEQUENCE\x10\x03\x12\x1b\n\x17STATUS_FAILED_TO_UPDATE\x10\x04\"I\n\x1c\x43learAllSequenceFilesRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"\xdc\x01\n\x1d\x43learAllSequenceFilesResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x45\n\x06status\x18\x02 \x01(\x0e\x32\x35.bosdyn.api.spot.ClearAllSequenceFilesResponse.Status\"H\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1b\n\x17STATUS_FAILED_TO_DELETE\x10\x02\"\xa8\x01\n\x19UploadChoreographyRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x44\n\x15\x63horeography_sequence\x18\x02 \x01(\x0b\x32%.bosdyn.api.spot.ChoreographySequence\x12\x1a\n\x12non_strict_parsing\x18\x03 \x01(\x08\"Z\n\x1aUploadChoreographyResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x10\n\x08warnings\x18\x03 \x03(\t\"\xbb\x01\n\x19UploadAnimatedMoveRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12@\n\x1a\x61nimated_move_generated_id\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\ranimated_move\x18\x02 \x01(\x0b\x32\x1a.bosdyn.api.spot.Animation\"\x8d\x02\n\x1aUploadAnimatedMoveResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x42\n\x06status\x18\x02 \x01(\x0e\x32\x32.bosdyn.api.spot.UploadAnimatedMoveResponse.Status\x12\x10\n\x08warnings\x18\x03 \x03(\t\"m\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12&\n\"STATUS_ANIMATION_VALIDATION_FAILED\x10\x02\x12\x18\n\x14STATUS_PING_RESPONSE\x10\x03\"\xe2\x01\n\x1a\x45xecuteChoreographyRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\"\n\x1a\x63horeography_sequence_name\x18\x02 \x01(\t\x12.\n\nstart_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12#\n\x1b\x63horeography_starting_slice\x18\x04 \x01(\x01\x12 \n\x05lease\x18\x06 \x01(\x0b\x32\x11.bosdyn.api.Lease\"\xd5\x02\n\x1b\x45xecuteChoreographyResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x34\n\x10lease_use_result\x18\x02 \x01(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12\x43\n\x06status\x18\x03 \x01(\x0e\x32\x33.bosdyn.api.spot.ExecuteChoreographyResponse.Status\"\x8e\x01\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12(\n$STATUS_INVALID_UPLOADED_CHOREOGRAPHY\x10\x02\x12\x1f\n\x1bSTATUS_ROBOT_COMMAND_ISSUES\x10\x03\x12\x16\n\x12STATUS_LEASE_ERROR\x10\x04\"\xa5\x01\n\x1aStartRecordingStateRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12>\n\x1b\x63ontinue_recording_duration\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x1c\n\x14recording_session_id\x18\x03 \x01(\x04\"\xa4\x02\n\x1bStartRecordingStateResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x43\n\x06status\x18\x02 \x01(\x0e\x32\x33.bosdyn.api.spot.StartRecordingStateResponse.Status\x12\x1c\n\x14recording_session_id\x18\x03 \x01(\x04\"v\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\'\n#STATUS_UNKNOWN_RECORDING_SESSION_ID\x10\x02\x12 \n\x1cSTATUS_RECORDING_BUFFER_FULL\x10\x03\"F\n\x19StopRecordingStateRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"H\n\x1aStopRecordingStateResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\"\xe8\x01\n\x1c\x44ownloadRobotStateLogRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12G\n\x08log_type\x18\x02 \x01(\x0e\x32\x35.bosdyn.api.spot.DownloadRobotStateLogRequest.LogType\"T\n\x07LogType\x12\x14\n\x10LOG_TYPE_UNKNOWN\x10\x00\x12\x13\n\x0fLOG_TYPE_MANUAL\x10\x01\x12\x1e\n\x1aLOG_TYPE_LAST_CHOREOGRAPHY\x10\x02\"\xa5\x02\n\x0cLoggedJoints\x12+\n\x02\x66l\x18\x01 \x01(\x0b\x32\x1f.bosdyn.api.spot.LegJointAngles\x12+\n\x02\x66r\x18\x02 \x01(\x0b\x32\x1f.bosdyn.api.spot.LegJointAngles\x12+\n\x02hl\x18\x03 \x01(\x0b\x32\x1f.bosdyn.api.spot.LegJointAngles\x12+\n\x02hr\x18\x04 \x01(\x0b\x32\x1f.bosdyn.api.spot.LegJointAngles\x12,\n\x03\x61rm\x18\x05 \x01(\x0b\x32\x1f.bosdyn.api.spot.ArmJointAngles\x12\x33\n\rgripper_angle\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"d\n\x12LoggedFootContacts\x12\x12\n\nfr_contact\x18\x01 \x01(\x08\x12\x12\n\nfl_contact\x18\x02 \x01(\x08\x12\x12\n\nhr_contact\x18\x03 \x01(\x08\x12\x12\n\nhl_contact\x18\x04 \x01(\x08\"\xed\x01\n\x13LoggedStateKeyFrame\x12\x33\n\x0cjoint_angles\x18\x01 \x01(\x0b\x32\x1d.bosdyn.api.spot.LoggedJoints\x12?\n\x12\x66oot_contact_state\x18\x04 \x01(\x0b\x32#.bosdyn.api.spot.LoggedFootContacts\x12\x31\n\x14\x61nimation_tform_body\x18\x02 \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\x12-\n\ttimestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"P\n\x14\x43horeographyStateLog\x12\x38\n\nkey_frames\x18\x01 \x03(\x0b\x32$.bosdyn.api.spot.LoggedStateKeyFrame\"\xa5\x02\n\x1d\x44ownloadRobotStateLogResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x45\n\x06status\x18\x02 \x01(\x0e\x32\x35.bosdyn.api.spot.DownloadRobotStateLogResponse.Status\x12$\n\x05\x63hunk\x18\x03 \x01(\x0b\x32\x15.bosdyn.api.DataChunk\"k\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\"\n\x1eSTATUS_NO_RECORDED_INFORMATION\x10\x02\x12\x1a\n\x16STATUS_INCOMPLETE_DATA\x10\x03\"\xb8\x10\n\nMoveParams\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x13\n\x0bstart_slice\x18\x02 \x01(\x05\x12\x18\n\x10requested_slices\x18\x03 \x01(\x05\x12\x32\n\x0bjump_params\x18\x0b \x01(\x0b\x32\x1b.bosdyn.api.spot.JumpParamsH\x00\x12?\n\x12rotate_body_params\x18\x0c \x01(\x0b\x32!.bosdyn.api.spot.RotateBodyParamsH\x00\x12\x32\n\x0bstep_params\x18\r \x01(\x0b\x32\x1b.bosdyn.api.spot.StepParamsH\x00\x12?\n\x12\x62utt_circle_params\x18\x0e \x01(\x0b\x32!.bosdyn.api.spot.ButtCircleParamsH\x00\x12\x32\n\x0bturn_params\x18\x0f \x01(\x0b\x32\x1b.bosdyn.api.spot.TurnParamsH\x00\x12=\n\x11pace_2step_params\x18\x10 \x01(\x0b\x32 .bosdyn.api.spot.Pace2StepParamsH\x00\x12\x34\n\x0ctwerk_params\x18\x11 \x01(\x0b\x32\x1c.bosdyn.api.spot.TwerkParamsH\x00\x12\x41\n\x13\x63hicken_head_params\x18\x12 \x01(\x0b\x32\".bosdyn.api.spot.ChickenHeadParamsH\x00\x12\x32\n\x0b\x63lap_params\x18\x13 \x01(\x0b\x32\x1b.bosdyn.api.spot.ClapParamsH\x00\x12\x39\n\x0f\x66ront_up_params\x18\x14 \x01(\x0b\x32\x1e.bosdyn.api.spot.FrontUpParamsH\x00\x12\x32\n\x0bsway_params\x18\x15 \x01(\x0b\x32\x1b.bosdyn.api.spot.SwayParamsH\x00\x12;\n\x10\x62ody_hold_params\x18\x16 \x01(\x0b\x32\x1f.bosdyn.api.spot.BodyHoldParamsH\x00\x12\x39\n\x0f\x61rm_move_params\x18\x17 \x01(\x0b\x32\x1e.bosdyn.api.spot.ArmMoveParamsH\x00\x12\x44\n\x15kneel_leg_move_params\x18\x18 \x01(\x0b\x32#.bosdyn.api.spot.KneelLegMoveParamsH\x00\x12?\n\x12running_man_params\x18\x19 \x01(\x0b\x32!.bosdyn.api.spot.RunningManParamsH\x00\x12\x41\n\x13kneel_circle_params\x18\x1a \x01(\x0b\x32\".bosdyn.api.spot.KneelCircleParamsH\x00\x12\x38\n\x0egripper_params\x18\x1b \x01(\x0b\x32\x1e.bosdyn.api.spot.GripperParamsH\x00\x12\x30\n\nhop_params\x18\x1c \x01(\x0b\x32\x1a.bosdyn.api.spot.HopParamsH\x00\x12\x43\n\x14random_rotate_params\x18\x1d \x01(\x0b\x32#.bosdyn.api.spot.RandomRotateParamsH\x00\x12\x34\n\x0c\x63rawl_params\x18\x1e \x01(\x0b\x32\x1c.bosdyn.api.spot.CrawlParamsH\x00\x12\x32\n\x0bside_params\x18\x1f \x01(\x0b\x32\x1b.bosdyn.api.spot.SideParamsH\x00\x12\x38\n\x0e\x62ourree_params\x18  \x01(\x0b\x32\x1e.bosdyn.api.spot.BourreeParamsH\x00\x12L\n\x19workspace_arm_move_params\x18! \x01(\x0b\x32\'.bosdyn.api.spot.WorkspaceArmMoveParamsH\x00\x12\x38\n\x0e\x66igure8_params\x18\" \x01(\x0b\x32\x1e.bosdyn.api.spot.Figure8ParamsH\x00\x12\x46\n\x16kneel_leg_move2_params\x18# \x01(\x0b\x32$.bosdyn.api.spot.KneelLegMove2ParamsH\x00\x12\x41\n\x13\x66idget_stand_params\x18$ \x01(\x0b\x32\".bosdyn.api.spot.FidgetStandParamsH\x00\x12\x32\n\x0bgoto_params\x18% \x01(\x0b\x32\x1b.bosdyn.api.spot.GotoParamsH\x00\x12\x45\n\x15\x66rame_snapshot_params\x18& \x01(\x0b\x32$.bosdyn.api.spot.FrameSnapshotParamsH\x00\x12;\n\x10set_color_params\x18\' \x01(\x0b\x32\x1f.bosdyn.api.spot.SetColorParamsH\x00\x12\x41\n\x13ripple_color_params\x18( \x01(\x0b\x32\".bosdyn.api.spot.RippleColorParamsH\x00\x12=\n\x11\x66\x61\x64\x65_color_params\x18) \x01(\x0b\x32 .bosdyn.api.spot.FadeColorParamsH\x00\x12K\n\x18independent_color_params\x18* \x01(\x0b\x32\'.bosdyn.api.spot.IndependentColorParamsH\x00\x12\x39\n\x0e\x61nimate_params\x18\xe8\x07 \x01(\x0b\x32\x1e.bosdyn.api.spot.AnimateParamsH\x00\x42\x08\n\x06params\"\x80\x06\n\x08MoveInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1a\n\x12move_length_slices\x18\x02 \x01(\x05\x12\x18\n\x10move_length_time\x18\x0f \x01(\x01\x12\x15\n\ris_extendable\x18\x03 \x01(\x08\x12\x1e\n\x16min_move_length_slices\x18\r \x01(\x05\x12\x1e\n\x16max_move_length_slices\x18\x0e \x01(\x05\x12\x10\n\x08min_time\x18\x06 \x01(\x01\x12\x10\n\x08max_time\x18\x07 \x01(\x01\x12\x42\n\x0f\x65ntrance_states\x18\x04 \x03(\x0e\x32).bosdyn.api.spot.MoveInfo.TransitionState\x12=\n\nexit_state\x18\x05 \x01(\x0e\x32).bosdyn.api.spot.MoveInfo.TransitionState\x12\x14\n\x0c\x63ontrols_arm\x18\x08 \x01(\x08\x12\x15\n\rcontrols_legs\x18\t \x01(\x08\x12\x15\n\rcontrols_body\x18\n \x01(\x08\x12\x18\n\x10\x63ontrols_gripper\x18\x0c \x01(\x08\x12\x17\n\x0f\x63ontrols_lights\x18\x11 \x01(\x08\x12\x1c\n\x14\x63ontrols_annotations\x18\x12 \x01(\x08\x12:\n\x07\x64isplay\x18\x0b \x01(\x0b\x32).bosdyn.api.spot.ChoreographerDisplayInfo\x12@\n\x1a\x61nimated_move_generated_id\x18\x10 \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\x9e\x01\n\x0fTransitionState\x12\x1c\n\x18TRANSITION_STATE_UNKNOWN\x10\x00\x12\x1a\n\x16TRANSITION_STATE_STAND\x10\x01\x12\x1a\n\x16TRANSITION_STATE_KNEEL\x10\x02\x12\x18\n\x14TRANSITION_STATE_SIT\x10\x03\x12\x1b\n\x17TRANSITION_STATE_SPRAWL\x10\x04\"\x81\x04\n\x18\x43horeographerDisplayInfo\x12>\n\x05\x63olor\x18\x01 \x01(\x0b\x32/.bosdyn.api.spot.ChoreographerDisplayInfo.Color\x12\x0f\n\x07markers\x18\r \x03(\x05\x12\x13\n\x0b\x64\x65scription\x18\x0e \x01(\t\x12\r\n\x05image\x18\x0f \x01(\t\x12\x44\n\x08\x63\x61tegory\x18\x10 \x01(\x0e\x32\x32.bosdyn.api.spot.ChoreographerDisplayInfo.Category\x1a\x33\n\x05\x43olor\x12\t\n\x01r\x18\x01 \x01(\x05\x12\t\n\x01g\x18\x02 \x01(\x05\x12\t\n\x01\x62\x18\x03 \x01(\x05\x12\t\n\x01\x61\x18\x04 \x01(\x01\"\xf4\x01\n\x08\x43\x61tegory\x12\x14\n\x10\x43\x41TEGORY_UNKNOWN\x10\x00\x12\x11\n\rCATEGORY_BODY\x10\x01\x12\x11\n\rCATEGORY_STEP\x10\x02\x12\x14\n\x10\x43\x41TEGORY_DYNAMIC\x10\x03\x12\x17\n\x13\x43\x41TEGORY_TRANSITION\x10\x04\x12\x12\n\x0e\x43\x41TEGORY_KNEEL\x10\x05\x12\x10\n\x0c\x43\x41TEGORY_ARM\x10\x06\x12\x16\n\x12\x43\x41TEGORY_ANIMATION\x10\x07\x12\x10\n\x0c\x43\x41TEGORY_MPC\x10\x08\x12\x13\n\x0f\x43\x41TEGORY_LIGHTS\x10\t\x12\x18\n\x14\x43\x41TEGORY_ANNOTATIONS\x10\n\"\xa9\x01\n\x14\x43horeographySequence\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x19\n\x11slices_per_minute\x18\x02 \x01(\x01\x12*\n\x05moves\x18\x03 \x03(\x0b\x32\x1b.bosdyn.api.spot.MoveParams\x12<\n\x11\x63horeography_info\x18\x04 \x01(\x0b\x32!.bosdyn.api.spot.ChoreographyInfo\"\"\n\x10\x43horeographyInfo\x12\x0e\n\x06labels\x18\x04 \x03(\t\"\xaa\x01\n\x11\x43horeographerSave\x12\x44\n\x15\x63horeography_sequence\x18\x01 \x01(\x0b\x32%.bosdyn.api.spot.ChoreographySequence\x12\x12\n\nmusic_file\x18\x02 \x01(\t\x12\x19\n\x11music_start_slice\x18\x03 \x01(\x01\x12 \n\x18\x63horeography_start_slice\x18\x04 \x01(\x01\"\xdb\x06\n\tAnimation\x12\x0c\n\x04name\x18\x01 \x01(\t\x12?\n\x13\x61nimation_keyframes\x18\x02 \x03(\x0b\x32\".bosdyn.api.spot.AnimationKeyframe\x12\x14\n\x0c\x63ontrols_arm\x18\x03 \x01(\x08\x12\x15\n\rcontrols_legs\x18\x04 \x01(\x08\x12\x15\n\rcontrols_body\x18\x05 \x01(\x08\x12\x18\n\x10\x63ontrols_gripper\x18\x06 \x01(\x08\x12 \n\x18track_swing_trajectories\x18\x10 \x01(\x08\x12\"\n\x1a\x61ssume_zero_roll_and_pitch\x18\x13 \x01(\x08\x12<\n\x0c\x61rm_playback\x18\x11 \x01(\x0e\x32&.bosdyn.api.spot.Animation.ArmPlayback\x12\x0b\n\x03\x62pm\x18\x07 \x01(\x01\x12 \n\x18retime_to_integer_slices\x18\x08 \x01(\x08\x12:\n\x12minimum_parameters\x18\t \x01(\x0b\x32\x1e.bosdyn.api.spot.AnimateParams\x12:\n\x12\x64\x65\x66\x61ult_parameters\x18\n \x01(\x0b\x32\x1e.bosdyn.api.spot.AnimateParams\x12:\n\x12maximum_parameters\x18\x0b \x01(\x0b\x32\x1e.bosdyn.api.spot.AnimateParams\x12\x13\n\x0btruncatable\x18\x0c \x01(\x08\x12\x12\n\nextendable\x18\r \x01(\x08\x12\x15\n\rneutral_start\x18\x0e \x01(\x08\x12\x15\n\rprecise_steps\x18\x0f \x01(\x08\x12\x16\n\x0eprecise_timing\x18\x12 \x01(\x08\x12\x14\n\x0c\x61rm_required\x18\x14 \x01(\x08\x12\x16\n\x0e\x61rm_prohibited\x18\x16 \x01(\x08\x12\x12\n\nno_looping\x18\x15 \x01(\x08\"\x88\x01\n\x0b\x41rmPlayback\x12\x18\n\x14\x41RM_PLAYBACK_DEFAULT\x10\x00\x12\x1b\n\x17\x41RM_PLAYBACK_JOINTSPACE\x10\x01\x12\x1a\n\x16\x41RM_PLAYBACK_WORKSPACE\x10\x02\x12&\n\"ARM_PLAYBACK_WORKSPACE_DANCE_FRAME\x10\x03\"\xd5\x01\n\x11\x41nimationKeyframe\x12\x0c\n\x04time\x18\x01 \x01(\x01\x12\x30\n\x07gripper\x18\x02 \x01(\x0b\x32\x1f.bosdyn.api.spot.AnimateGripper\x12(\n\x03\x61rm\x18\x03 \x01(\x0b\x32\x1b.bosdyn.api.spot.AnimateArm\x12*\n\x04\x62ody\x18\x04 \x01(\x0b\x32\x1c.bosdyn.api.spot.AnimateBody\x12*\n\x04legs\x18\x05 \x01(\x0b\x32\x1c.bosdyn.api.spot.AnimateLegs\"E\n\x0e\x41nimateGripper\x12\x33\n\rgripper_angle\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\xb2\x02\n\nAnimateArm\x12\x37\n\x0cjoint_angles\x18\x01 \x01(\x0b\x32\x1f.bosdyn.api.spot.ArmJointAnglesH\x00\x12\x39\n\thand_pose\x18\x02 \x01(\x0b\x32$.bosdyn.api.spot.AnimateArm.HandPoseH\x00\x1a\xa8\x01\n\x08HandPose\x12\'\n\x08position\x18\x01 \x01(\x0b\x32\x15.bosdyn.api.Vec3Value\x12\x36\n\x0c\x65uler_angles\x18\x03 \x01(\x0b\x32\x1e.bosdyn.api.spot.EulerZYXValueH\x00\x12,\n\nquaternion\x18\x04 \x01(\x0b\x32\x16.bosdyn.api.QuaternionH\x00\x42\r\n\x0borientationB\x05\n\x03\x61rm\"\xb0\x02\n\x0e\x41rmJointAngles\x12\x30\n\nshoulder_0\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x30\n\nshoulder_1\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12-\n\x07\x65lbow_0\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12-\n\x07\x65lbow_1\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12-\n\x07wrist_0\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12-\n\x07wrist_1\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\xe3\x01\n\x0b\x41nimateBody\x12)\n\x08\x62ody_pos\x18\x01 \x01(\x0b\x32\x15.bosdyn.api.Vec3ValueH\x00\x12(\n\x07\x63om_pos\x18\x02 \x01(\x0b\x32\x15.bosdyn.api.Vec3ValueH\x00\x12\x36\n\x0c\x65uler_angles\x18\x03 \x01(\x0b\x32\x1e.bosdyn.api.spot.EulerZYXValueH\x01\x12,\n\nquaternion\x18\x04 \x01(\x0b\x32\x16.bosdyn.api.QuaternionH\x01\x42\n\n\x08positionB\r\n\x0borientation\"\xc9\x01\n\x0b\x41nimateLegs\x12-\n\x02\x66l\x18\x01 \x01(\x0b\x32!.bosdyn.api.spot.AnimateSingleLeg\x12-\n\x02\x66r\x18\x02 \x01(\x0b\x32!.bosdyn.api.spot.AnimateSingleLeg\x12-\n\x02hl\x18\x03 \x01(\x0b\x32!.bosdyn.api.spot.AnimateSingleLeg\x12-\n\x02hr\x18\x04 \x01(\x0b\x32!.bosdyn.api.spot.AnimateSingleLeg\"\xa9\x01\n\x10\x41nimateSingleLeg\x12\x37\n\x0cjoint_angles\x18\x01 \x01(\x0b\x32\x1f.bosdyn.api.spot.LegJointAnglesH\x00\x12)\n\x08\x66oot_pos\x18\x02 \x01(\x0b\x32\x15.bosdyn.api.Vec3ValueH\x00\x12*\n\x06stance\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.BoolValueB\x05\n\x03leg\"<\n\x0eLegJointAngles\x12\r\n\x05hip_x\x18\x01 \x01(\x01\x12\r\n\x05hip_y\x18\x02 \x01(\x01\x12\x0c\n\x04knee\x18\x03 \x01(\x01\x42\x13\x42\x11\x43horeographyProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n+bosdyn/api/spot/choreography_sequence.proto\x12\x0f\x62osdyn.api.spot\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x19\x62osdyn/api/geometry.proto\x1a\x17\x62osdyn/api/header.proto\x1a\x16\x62osdyn/api/lease.proto\x1a)bosdyn/api/spot/choreography_params.proto\x1a\x1b\x62osdyn/api/data_chunk.proto\"@\n\x13ListAllMovesRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"\x87\x01\n\x14ListAllMovesResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12(\n\x05moves\x18\x02 \x03(\x0b\x32\x19.bosdyn.api.spot.MoveInfo\x12\x19\n\x11move_param_config\x18\x03 \x01(\t\"D\n\x17ListAllSequencesRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"\x99\x01\n\x18ListAllSequencesResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x1b\n\x0fknown_sequences\x18\x02 \x03(\tB\x02\x18\x01\x12\x34\n\rsequence_info\x18\x03 \x03(\x0b\x32\x1d.bosdyn.api.spot.SequenceInfo\"\xa1\x02\n\x0cSequenceInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06labels\x18\x02 \x03(\t\x12=\n\x0bsaved_state\x18\x03 \x01(\x0e\x32(.bosdyn.api.spot.SequenceInfo.SavedState\x12=\n\nexit_state\x18\x04 \x01(\x0e\x32).bosdyn.api.spot.MoveInfo.TransitionState\"u\n\nSavedState\x12\x17\n\x13SAVED_STATE_UNKNOWN\x10\x00\x12\x19\n\x15SAVED_STATE_TEMPORARY\x10\x01\x12\x18\n\x14SAVED_STATE_RETAINED\x10\x02\x12\x19\n\x15SAVED_STATE_PERMANENT\x10\x03\"Y\n\x15\x44\x65leteSequenceRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x15\n\rsequence_name\x18\x02 \x01(\t\"\x8c\x02\n\x16\x44\x65leteSequenceResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12>\n\x06status\x18\x02 \x01(\x0e\x32..bosdyn.api.spot.DeleteSequenceResponse.Status\"\x85\x01\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1b\n\x17STATUS_UNKNOWN_SEQUENCE\x10\x02\x12\x1c\n\x18STATUS_ALREADY_TEMPORARY\x10\x03\x12\x1d\n\x19STATUS_PERMANENT_SEQUENCE\x10\x04\"k\n\x13SaveSequenceRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x15\n\rsequence_name\x18\x02 \x01(\t\x12\x12\n\nadd_labels\x18\x03 \x03(\t\"\x85\x02\n\x14SaveSequenceResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12<\n\x06status\x18\x02 \x01(\x0e\x32,.bosdyn.api.spot.SaveSequenceResponse.Status\"\x82\x01\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1b\n\x17STATUS_UNKNOWN_SEQUENCE\x10\x02\x12\x1d\n\x19STATUS_PERMANENT_SEQUENCE\x10\x03\x12\x19\n\x15STATUS_FAILED_TO_SAVE\x10\x04\"\x8c\x01\n\x1dModifyChoreographyInfoRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x15\n\rsequence_name\x18\x02 \x01(\t\x12\x12\n\nadd_labels\x18\x03 \x03(\t\x12\x15\n\rremove_labels\x18\x04 \x03(\t\"\x9b\x02\n\x1eModifyChoreographyInfoResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x46\n\x06status\x18\x02 \x01(\x0e\x32\x36.bosdyn.api.spot.ModifyChoreographyInfoResponse.Status\"\x84\x01\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1b\n\x17STATUS_UNKNOWN_SEQUENCE\x10\x02\x12\x1d\n\x19STATUS_PERMANENT_SEQUENCE\x10\x03\x12\x1b\n\x17STATUS_FAILED_TO_UPDATE\x10\x04\"I\n\x1c\x43learAllSequenceFilesRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"\xdc\x01\n\x1d\x43learAllSequenceFilesResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x45\n\x06status\x18\x02 \x01(\x0e\x32\x35.bosdyn.api.spot.ClearAllSequenceFilesResponse.Status\"H\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\x1b\n\x17STATUS_FAILED_TO_DELETE\x10\x02\"\xa8\x01\n\x19UploadChoreographyRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\x44\n\x15\x63horeography_sequence\x18\x02 \x01(\x0b\x32%.bosdyn.api.spot.ChoreographySequence\x12\x1a\n\x12non_strict_parsing\x18\x03 \x01(\x08\"Z\n\x1aUploadChoreographyResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x10\n\x08warnings\x18\x03 \x03(\t\"\xbb\x01\n\x19UploadAnimatedMoveRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12@\n\x1a\x61nimated_move_generated_id\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\ranimated_move\x18\x02 \x01(\x0b\x32\x1a.bosdyn.api.spot.Animation\"\x8d\x02\n\x1aUploadAnimatedMoveResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x42\n\x06status\x18\x02 \x01(\x0e\x32\x32.bosdyn.api.spot.UploadAnimatedMoveResponse.Status\x12\x10\n\x08warnings\x18\x03 \x03(\t\"m\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12&\n\"STATUS_ANIMATION_VALIDATION_FAILED\x10\x02\x12\x18\n\x14STATUS_PING_RESPONSE\x10\x03\"\xe2\x01\n\x1a\x45xecuteChoreographyRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12\"\n\x1a\x63horeography_sequence_name\x18\x02 \x01(\t\x12.\n\nstart_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12#\n\x1b\x63horeography_starting_slice\x18\x04 \x01(\x01\x12 \n\x05lease\x18\x06 \x01(\x0b\x32\x11.bosdyn.api.Lease\"\xeb\x02\n\x1b\x45xecuteChoreographyResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x34\n\x10lease_use_result\x18\x02 \x01(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12\x43\n\x06status\x18\x03 \x01(\x0e\x32\x33.bosdyn.api.spot.ExecuteChoreographyResponse.Status\x12\x14\n\x0c\x65xecution_id\x18\x04 \x01(\x05\"\x8e\x01\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12(\n$STATUS_INVALID_UPLOADED_CHOREOGRAPHY\x10\x02\x12\x1f\n\x1bSTATUS_ROBOT_COMMAND_ISSUES\x10\x03\x12\x16\n\x12STATUS_LEASE_ERROR\x10\x04\"\xa5\x01\n\x1aStartRecordingStateRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12>\n\x1b\x63ontinue_recording_duration\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x1c\n\x14recording_session_id\x18\x03 \x01(\x04\"\xa4\x02\n\x1bStartRecordingStateResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x43\n\x06status\x18\x02 \x01(\x0e\x32\x33.bosdyn.api.spot.StartRecordingStateResponse.Status\x12\x1c\n\x14recording_session_id\x18\x03 \x01(\x04\"v\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\'\n#STATUS_UNKNOWN_RECORDING_SESSION_ID\x10\x02\x12 \n\x1cSTATUS_RECORDING_BUFFER_FULL\x10\x03\"F\n\x19StopRecordingStateRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"H\n\x1aStopRecordingStateResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\"\xe8\x01\n\x1c\x44ownloadRobotStateLogRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12G\n\x08log_type\x18\x02 \x01(\x0e\x32\x35.bosdyn.api.spot.DownloadRobotStateLogRequest.LogType\"T\n\x07LogType\x12\x14\n\x10LOG_TYPE_UNKNOWN\x10\x00\x12\x13\n\x0fLOG_TYPE_MANUAL\x10\x01\x12\x1e\n\x1aLOG_TYPE_LAST_CHOREOGRAPHY\x10\x02\"\xa5\x02\n\x0cLoggedJoints\x12+\n\x02\x66l\x18\x01 \x01(\x0b\x32\x1f.bosdyn.api.spot.LegJointAngles\x12+\n\x02\x66r\x18\x02 \x01(\x0b\x32\x1f.bosdyn.api.spot.LegJointAngles\x12+\n\x02hl\x18\x03 \x01(\x0b\x32\x1f.bosdyn.api.spot.LegJointAngles\x12+\n\x02hr\x18\x04 \x01(\x0b\x32\x1f.bosdyn.api.spot.LegJointAngles\x12,\n\x03\x61rm\x18\x05 \x01(\x0b\x32\x1f.bosdyn.api.spot.ArmJointAngles\x12\x33\n\rgripper_angle\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"d\n\x12LoggedFootContacts\x12\x12\n\nfr_contact\x18\x01 \x01(\x08\x12\x12\n\nfl_contact\x18\x02 \x01(\x08\x12\x12\n\nhr_contact\x18\x03 \x01(\x08\x12\x12\n\nhl_contact\x18\x04 \x01(\x08\"\xed\x01\n\x13LoggedStateKeyFrame\x12\x33\n\x0cjoint_angles\x18\x01 \x01(\x0b\x32\x1d.bosdyn.api.spot.LoggedJoints\x12?\n\x12\x66oot_contact_state\x18\x04 \x01(\x0b\x32#.bosdyn.api.spot.LoggedFootContacts\x12\x31\n\x14\x61nimation_tform_body\x18\x02 \x01(\x0b\x32\x13.bosdyn.api.SE3Pose\x12-\n\ttimestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"P\n\x14\x43horeographyStateLog\x12\x38\n\nkey_frames\x18\x01 \x03(\x0b\x32$.bosdyn.api.spot.LoggedStateKeyFrame\"\xa5\x02\n\x1d\x44ownloadRobotStateLogResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x45\n\x06status\x18\x02 \x01(\x0e\x32\x35.bosdyn.api.spot.DownloadRobotStateLogResponse.Status\x12$\n\x05\x63hunk\x18\x03 \x01(\x0b\x32\x15.bosdyn.api.DataChunk\"k\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12\"\n\x1eSTATUS_NO_RECORDED_INFORMATION\x10\x02\x12\x1a\n\x16STATUS_INCOMPLETE_DATA\x10\x03\"\xc2\x11\n\nMoveParams\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x13\n\x0bstart_slice\x18\x02 \x01(\x05\x12\x18\n\x10requested_slices\x18\x03 \x01(\x05\x12\n\n\x02id\x18\x04 \x01(\x05\x12\x32\n\x0bjump_params\x18\x0b \x01(\x0b\x32\x1b.bosdyn.api.spot.JumpParamsH\x00\x12?\n\x12rotate_body_params\x18\x0c \x01(\x0b\x32!.bosdyn.api.spot.RotateBodyParamsH\x00\x12\x32\n\x0bstep_params\x18\r \x01(\x0b\x32\x1b.bosdyn.api.spot.StepParamsH\x00\x12?\n\x12\x62utt_circle_params\x18\x0e \x01(\x0b\x32!.bosdyn.api.spot.ButtCircleParamsH\x00\x12\x32\n\x0bturn_params\x18\x0f \x01(\x0b\x32\x1b.bosdyn.api.spot.TurnParamsH\x00\x12=\n\x11pace_2step_params\x18\x10 \x01(\x0b\x32 .bosdyn.api.spot.Pace2StepParamsH\x00\x12\x34\n\x0ctwerk_params\x18\x11 \x01(\x0b\x32\x1c.bosdyn.api.spot.TwerkParamsH\x00\x12\x41\n\x13\x63hicken_head_params\x18\x12 \x01(\x0b\x32\".bosdyn.api.spot.ChickenHeadParamsH\x00\x12\x32\n\x0b\x63lap_params\x18\x13 \x01(\x0b\x32\x1b.bosdyn.api.spot.ClapParamsH\x00\x12\x39\n\x0f\x66ront_up_params\x18\x14 \x01(\x0b\x32\x1e.bosdyn.api.spot.FrontUpParamsH\x00\x12\x32\n\x0bsway_params\x18\x15 \x01(\x0b\x32\x1b.bosdyn.api.spot.SwayParamsH\x00\x12;\n\x10\x62ody_hold_params\x18\x16 \x01(\x0b\x32\x1f.bosdyn.api.spot.BodyHoldParamsH\x00\x12\x39\n\x0f\x61rm_move_params\x18\x17 \x01(\x0b\x32\x1e.bosdyn.api.spot.ArmMoveParamsH\x00\x12\x44\n\x15kneel_leg_move_params\x18\x18 \x01(\x0b\x32#.bosdyn.api.spot.KneelLegMoveParamsH\x00\x12?\n\x12running_man_params\x18\x19 \x01(\x0b\x32!.bosdyn.api.spot.RunningManParamsH\x00\x12\x41\n\x13kneel_circle_params\x18\x1a \x01(\x0b\x32\".bosdyn.api.spot.KneelCircleParamsH\x00\x12\x38\n\x0egripper_params\x18\x1b \x01(\x0b\x32\x1e.bosdyn.api.spot.GripperParamsH\x00\x12\x30\n\nhop_params\x18\x1c \x01(\x0b\x32\x1a.bosdyn.api.spot.HopParamsH\x00\x12\x43\n\x14random_rotate_params\x18\x1d \x01(\x0b\x32#.bosdyn.api.spot.RandomRotateParamsH\x00\x12\x34\n\x0c\x63rawl_params\x18\x1e \x01(\x0b\x32\x1c.bosdyn.api.spot.CrawlParamsH\x00\x12\x32\n\x0bside_params\x18\x1f \x01(\x0b\x32\x1b.bosdyn.api.spot.SideParamsH\x00\x12\x38\n\x0e\x62ourree_params\x18  \x01(\x0b\x32\x1e.bosdyn.api.spot.BourreeParamsH\x00\x12L\n\x19workspace_arm_move_params\x18! \x01(\x0b\x32\'.bosdyn.api.spot.WorkspaceArmMoveParamsH\x00\x12\x38\n\x0e\x66igure8_params\x18\" \x01(\x0b\x32\x1e.bosdyn.api.spot.Figure8ParamsH\x00\x12\x46\n\x16kneel_leg_move2_params\x18# \x01(\x0b\x32$.bosdyn.api.spot.KneelLegMove2ParamsH\x00\x12\x41\n\x13\x66idget_stand_params\x18$ \x01(\x0b\x32\".bosdyn.api.spot.FidgetStandParamsH\x00\x12\x32\n\x0bgoto_params\x18% \x01(\x0b\x32\x1b.bosdyn.api.spot.GotoParamsH\x00\x12\x45\n\x15\x66rame_snapshot_params\x18& \x01(\x0b\x32$.bosdyn.api.spot.FrameSnapshotParamsH\x00\x12;\n\x10set_color_params\x18\' \x01(\x0b\x32\x1f.bosdyn.api.spot.SetColorParamsH\x00\x12\x41\n\x13ripple_color_params\x18( \x01(\x0b\x32\".bosdyn.api.spot.RippleColorParamsH\x00\x12=\n\x11\x66\x61\x64\x65_color_params\x18) \x01(\x0b\x32 .bosdyn.api.spot.FadeColorParamsH\x00\x12K\n\x18independent_color_params\x18* \x01(\x0b\x32\'.bosdyn.api.spot.IndependentColorParamsH\x00\x12?\n\x12\x63ustom_gait_params\x18+ \x01(\x0b\x32!.bosdyn.api.spot.CustomGaitParamsH\x00\x12;\n\x10leg_joint_params\x18\x64 \x01(\x0b\x32\x1f.bosdyn.api.spot.LegJointParamsH\x00\x12\x39\n\x0e\x61nimate_params\x18\xe8\x07 \x01(\x0b\x32\x1e.bosdyn.api.spot.AnimateParamsH\x00\x42\x08\n\x06params\"\x7f\n\x0bMoveCommand\x12\x11\n\tmove_type\x18\x01 \x01(\t\x12\x0f\n\x07move_id\x18\x02 \x01(\x05\x12\x41\n\x13\x63ustom_gait_command\x18\x03 \x01(\x0b\x32\".bosdyn.api.spot.CustomGaitCommandH\x00\x42\t\n\x07\x63ommand\"\xcf\x01\n\x1a\x43horeographyCommandRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\x12.\n\x08\x63ommands\x18\x02 \x03(\x0b\x32\x1c.bosdyn.api.spot.MoveCommand\x12 \n\x05lease\x18\x03 \x01(\x0b\x32\x11.bosdyn.api.Lease\x12\x34\n\x10\x63ommand_end_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x86\x03\n\x1b\x43horeographyCommandResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x34\n\x10lease_use_result\x18\x02 \x01(\x0b\x32\x1a.bosdyn.api.LeaseUseResult\x12\x43\n\x06status\x18\x03 \x03(\x0e\x32\x33.bosdyn.api.spot.ChoreographyCommandResponse.Status\"\xbf\x01\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\r\n\tSTATUS_OK\x10\x01\x12%\n!STATUS_ACCEPTED_WITH_MODIFICATION\x10\x02\x12\x16\n\x12STATUS_LEASE_ERROR\x10\x03\x12\x1b\n\x17STATUS_NO_MATCHING_MOVE\x10\x04\x12\x1a\n\x16STATUS_INVALID_COMMAND\x10\x05\x12\x1a\n\x16STATUS_ALREADY_EXPIRED\x10\x06\"\x94\x06\n\x08MoveInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x1a\n\x12move_length_slices\x18\x02 \x01(\x05\x12\x18\n\x10move_length_time\x18\x0f \x01(\x01\x12\x15\n\ris_extendable\x18\x03 \x01(\x08\x12\x1e\n\x16min_move_length_slices\x18\r \x01(\x05\x12\x1e\n\x16max_move_length_slices\x18\x0e \x01(\x05\x12\x10\n\x08min_time\x18\x06 \x01(\x01\x12\x10\n\x08max_time\x18\x07 \x01(\x01\x12\x42\n\x0f\x65ntrance_states\x18\x04 \x03(\x0e\x32).bosdyn.api.spot.MoveInfo.TransitionState\x12=\n\nexit_state\x18\x05 \x01(\x0e\x32).bosdyn.api.spot.MoveInfo.TransitionState\x12\x14\n\x0c\x63ontrols_arm\x18\x08 \x01(\x08\x12\x15\n\rcontrols_legs\x18\t \x01(\x08\x12\x15\n\rcontrols_body\x18\n \x01(\x08\x12\x18\n\x10\x63ontrols_gripper\x18\x0c \x01(\x08\x12\x17\n\x0f\x63ontrols_lights\x18\x11 \x01(\x08\x12\x1c\n\x14\x63ontrols_annotations\x18\x12 \x01(\x08\x12\x12\n\nis_looping\x18\x13 \x01(\x08\x12:\n\x07\x64isplay\x18\x0b \x01(\x0b\x32).bosdyn.api.spot.ChoreographerDisplayInfo\x12@\n\x1a\x61nimated_move_generated_id\x18\x10 \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\x9e\x01\n\x0fTransitionState\x12\x1c\n\x18TRANSITION_STATE_UNKNOWN\x10\x00\x12\x1a\n\x16TRANSITION_STATE_STAND\x10\x01\x12\x1a\n\x16TRANSITION_STATE_KNEEL\x10\x02\x12\x18\n\x14TRANSITION_STATE_SIT\x10\x03\x12\x1b\n\x17TRANSITION_STATE_SPRAWL\x10\x04\"\x81\x04\n\x18\x43horeographerDisplayInfo\x12>\n\x05\x63olor\x18\x01 \x01(\x0b\x32/.bosdyn.api.spot.ChoreographerDisplayInfo.Color\x12\x0f\n\x07markers\x18\r \x03(\x05\x12\x13\n\x0b\x64\x65scription\x18\x0e \x01(\t\x12\r\n\x05image\x18\x0f \x01(\t\x12\x44\n\x08\x63\x61tegory\x18\x10 \x01(\x0e\x32\x32.bosdyn.api.spot.ChoreographerDisplayInfo.Category\x1a\x33\n\x05\x43olor\x12\t\n\x01r\x18\x01 \x01(\x05\x12\t\n\x01g\x18\x02 \x01(\x05\x12\t\n\x01\x62\x18\x03 \x01(\x05\x12\t\n\x01\x61\x18\x04 \x01(\x01\"\xf4\x01\n\x08\x43\x61tegory\x12\x14\n\x10\x43\x41TEGORY_UNKNOWN\x10\x00\x12\x11\n\rCATEGORY_BODY\x10\x01\x12\x11\n\rCATEGORY_STEP\x10\x02\x12\x14\n\x10\x43\x41TEGORY_DYNAMIC\x10\x03\x12\x17\n\x13\x43\x41TEGORY_TRANSITION\x10\x04\x12\x12\n\x0e\x43\x41TEGORY_KNEEL\x10\x05\x12\x10\n\x0c\x43\x41TEGORY_ARM\x10\x06\x12\x16\n\x12\x43\x41TEGORY_ANIMATION\x10\x07\x12\x10\n\x0c\x43\x41TEGORY_MPC\x10\x08\x12\x13\n\x0f\x43\x41TEGORY_LIGHTS\x10\t\x12\x18\n\x14\x43\x41TEGORY_ANNOTATIONS\x10\n\"\xec\x01\n\x14\x43horeographySequence\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x19\n\x11slices_per_minute\x18\x02 \x01(\x01\x12*\n\x05moves\x18\x03 \x03(\x0b\x32\x1b.bosdyn.api.spot.MoveParams\x12<\n\x11\x63horeography_info\x18\x04 \x01(\x0b\x32!.bosdyn.api.spot.ChoreographyInfo\x12\x41\n\x0e\x65ntrance_state\x18\x05 \x01(\x0e\x32).bosdyn.api.spot.MoveInfo.TransitionState\"\"\n\x10\x43horeographyInfo\x12\x0e\n\x06labels\x18\x04 \x03(\t\"\xaa\x01\n\x11\x43horeographerSave\x12\x44\n\x15\x63horeography_sequence\x18\x01 \x01(\x0b\x32%.bosdyn.api.spot.ChoreographySequence\x12\x12\n\nmusic_file\x18\x02 \x01(\t\x12\x19\n\x11music_start_slice\x18\x03 \x01(\x01\x12 \n\x18\x63horeography_start_slice\x18\x04 \x01(\x01\"\xb0\x07\n\tAnimation\x12\x0c\n\x04name\x18\x01 \x01(\t\x12?\n\x13\x61nimation_keyframes\x18\x02 \x03(\x0b\x32\".bosdyn.api.spot.AnimationKeyframe\x12\x14\n\x0c\x63ontrols_arm\x18\x03 \x01(\x08\x12\x15\n\rcontrols_legs\x18\x04 \x01(\x08\x12\x15\n\rcontrols_body\x18\x05 \x01(\x08\x12\x18\n\x10\x63ontrols_gripper\x18\x06 \x01(\x08\x12 \n\x18track_swing_trajectories\x18\x10 \x01(\x08\x12\"\n\x1a\x61ssume_zero_roll_and_pitch\x18\x13 \x01(\x08\x12<\n\x0c\x61rm_playback\x18\x11 \x01(\x0e\x32&.bosdyn.api.spot.Animation.ArmPlayback\x12\x0b\n\x03\x62pm\x18\x07 \x01(\x01\x12 \n\x18retime_to_integer_slices\x18\x08 \x01(\x08\x12:\n\x12minimum_parameters\x18\t \x01(\x0b\x32\x1e.bosdyn.api.spot.AnimateParams\x12:\n\x12\x64\x65\x66\x61ult_parameters\x18\n \x01(\x0b\x32\x1e.bosdyn.api.spot.AnimateParams\x12:\n\x12maximum_parameters\x18\x0b \x01(\x0b\x32\x1e.bosdyn.api.spot.AnimateParams\x12\x13\n\x0btruncatable\x18\x0c \x01(\x08\x12\x12\n\nextendable\x18\r \x01(\x08\x12\x15\n\rneutral_start\x18\x0e \x01(\x08\x12\x15\n\rprecise_steps\x18\x0f \x01(\x08\x12\x1a\n\x0eprecise_timing\x18\x12 \x01(\x08\x42\x02\x18\x01\x12\x1c\n\x14timing_adjustability\x18\x17 \x01(\x01\x12\x14\n\x0c\x61rm_required\x18\x14 \x01(\x08\x12\x16\n\x0e\x61rm_prohibited\x18\x16 \x01(\x08\x12\x12\n\nno_looping\x18\x15 \x01(\x08\x12\x16\n\x0estarts_sitting\x18\x18 \x01(\x08\x12\x19\n\x11\x63ustom_gait_cycle\x18\x1b \x01(\x08\"\x88\x01\n\x0b\x41rmPlayback\x12\x18\n\x14\x41RM_PLAYBACK_DEFAULT\x10\x00\x12\x1b\n\x17\x41RM_PLAYBACK_JOINTSPACE\x10\x01\x12\x1a\n\x16\x41RM_PLAYBACK_WORKSPACE\x10\x02\x12&\n\"ARM_PLAYBACK_WORKSPACE_DANCE_FRAME\x10\x03\"\xd5\x01\n\x11\x41nimationKeyframe\x12\x0c\n\x04time\x18\x01 \x01(\x01\x12\x30\n\x07gripper\x18\x02 \x01(\x0b\x32\x1f.bosdyn.api.spot.AnimateGripper\x12(\n\x03\x61rm\x18\x03 \x01(\x0b\x32\x1b.bosdyn.api.spot.AnimateArm\x12*\n\x04\x62ody\x18\x04 \x01(\x0b\x32\x1c.bosdyn.api.spot.AnimateBody\x12*\n\x04legs\x18\x05 \x01(\x0b\x32\x1c.bosdyn.api.spot.AnimateLegs\"E\n\x0e\x41nimateGripper\x12\x33\n\rgripper_angle\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\xb2\x02\n\nAnimateArm\x12\x37\n\x0cjoint_angles\x18\x01 \x01(\x0b\x32\x1f.bosdyn.api.spot.ArmJointAnglesH\x00\x12\x39\n\thand_pose\x18\x02 \x01(\x0b\x32$.bosdyn.api.spot.AnimateArm.HandPoseH\x00\x1a\xa8\x01\n\x08HandPose\x12\'\n\x08position\x18\x01 \x01(\x0b\x32\x15.bosdyn.api.Vec3Value\x12\x36\n\x0c\x65uler_angles\x18\x03 \x01(\x0b\x32\x1e.bosdyn.api.spot.EulerZYXValueH\x00\x12,\n\nquaternion\x18\x04 \x01(\x0b\x32\x16.bosdyn.api.QuaternionH\x00\x42\r\n\x0borientationB\x05\n\x03\x61rm\"\xb0\x02\n\x0e\x41rmJointAngles\x12\x30\n\nshoulder_0\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12\x30\n\nshoulder_1\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12-\n\x07\x65lbow_0\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12-\n\x07\x65lbow_1\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12-\n\x07wrist_0\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\x12-\n\x07wrist_1\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.DoubleValue\"\xe3\x01\n\x0b\x41nimateBody\x12)\n\x08\x62ody_pos\x18\x01 \x01(\x0b\x32\x15.bosdyn.api.Vec3ValueH\x00\x12(\n\x07\x63om_pos\x18\x02 \x01(\x0b\x32\x15.bosdyn.api.Vec3ValueH\x00\x12\x36\n\x0c\x65uler_angles\x18\x03 \x01(\x0b\x32\x1e.bosdyn.api.spot.EulerZYXValueH\x01\x12,\n\nquaternion\x18\x04 \x01(\x0b\x32\x16.bosdyn.api.QuaternionH\x01\x42\n\n\x08positionB\r\n\x0borientation\"\xc9\x01\n\x0b\x41nimateLegs\x12-\n\x02\x66l\x18\x01 \x01(\x0b\x32!.bosdyn.api.spot.AnimateSingleLeg\x12-\n\x02\x66r\x18\x02 \x01(\x0b\x32!.bosdyn.api.spot.AnimateSingleLeg\x12-\n\x02hl\x18\x03 \x01(\x0b\x32!.bosdyn.api.spot.AnimateSingleLeg\x12-\n\x02hr\x18\x04 \x01(\x0b\x32!.bosdyn.api.spot.AnimateSingleLeg\"\xa9\x01\n\x10\x41nimateSingleLeg\x12\x37\n\x0cjoint_angles\x18\x01 \x01(\x0b\x32\x1f.bosdyn.api.spot.LegJointAnglesH\x00\x12)\n\x08\x66oot_pos\x18\x02 \x01(\x0b\x32\x15.bosdyn.api.Vec3ValueH\x00\x12*\n\x06stance\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.BoolValueB\x05\n\x03leg\"<\n\x0eLegJointAngles\x12\r\n\x05hip_x\x18\x01 \x01(\x01\x12\r\n\x05hip_y\x18\x02 \x01(\x01\x12\x0c\n\x04knee\x18\x03 \x01(\x01\"\x99\x01\n\nActiveMove\x12)\n\x04move\x18\x01 \x01(\x0b\x32\x1b.bosdyn.api.spot.MoveParams\x12N\n\x1a\x63ustom_gait_command_limits\x18\x02 \x01(\x0b\x32(.bosdyn.api.spot.CustomGaitCommandLimitsH\x00\x42\x10\n\x0e\x63ommand_limits\"F\n\x19\x43horeographyStatusRequest\x12)\n\x06header\x18\x01 \x01(\x0b\x32\x19.bosdyn.api.RequestHeader\"\xd2\x04\n\x1a\x43horeographyStatusResponse\x12*\n\x06header\x18\x01 \x01(\x0b\x32\x1a.bosdyn.api.ResponseHeader\x12\x42\n\x06status\x18\x02 \x01(\x0e\x32\x32.bosdyn.api.spot.ChoreographyStatusResponse.Status\x12\x14\n\x0c\x65xecution_id\x18\x03 \x01(\x05\x12\x15\n\rcurrent_slice\x18\x04 \x01(\x01\x12\x31\n\x0c\x61\x63tive_moves\x18\x05 \x03(\x0b\x32\x1b.bosdyn.api.spot.ActiveMove\x12\x17\n\x0fsequence_slices\x18\x06 \x01(\x05\x12\"\n\x1asequence_slices_per_minute\x18\x07 \x01(\x01\x12\x31\n\rvalidity_time\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xf3\x01\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x12\n\x0eSTATUS_DANCING\x10\x01\x12\x1d\n\x19STATUS_COMPLETED_SEQUENCE\x10\x02\x12\x13\n\x0fSTATUS_PREPPING\x10\x03\x12!\n\x1dSTATUS_WAITING_FOR_START_TIME\x10\x04\x12\x15\n\x11STATUS_VALIDATING\x10\x05\x12\x16\n\x12STATUS_INTERRUPTED\x10\x06\x12\x11\n\rSTATUS_FALLEN\x10\x07\x12\x16\n\x12STATUS_POWERED_OFF\x10\x08\x12\x10\n\x0cSTATUS_OTHER\x10\tB\x13\x42\x11\x43horeographyProtob\x06proto3')
 
 
 
 _LISTALLMOVESREQUEST = DESCRIPTOR.message_types_by_name['ListAllMovesRequest']
 _LISTALLMOVESRESPONSE = DESCRIPTOR.message_types_by_name['ListAllMovesResponse']
 _LISTALLSEQUENCESREQUEST = DESCRIPTOR.message_types_by_name['ListAllSequencesRequest']
 _LISTALLSEQUENCESRESPONSE = DESCRIPTOR.message_types_by_name['ListAllSequencesResponse']
@@ -52,14 +52,17 @@
 _DOWNLOADROBOTSTATELOGREQUEST = DESCRIPTOR.message_types_by_name['DownloadRobotStateLogRequest']
 _LOGGEDJOINTS = DESCRIPTOR.message_types_by_name['LoggedJoints']
 _LOGGEDFOOTCONTACTS = DESCRIPTOR.message_types_by_name['LoggedFootContacts']
 _LOGGEDSTATEKEYFRAME = DESCRIPTOR.message_types_by_name['LoggedStateKeyFrame']
 _CHOREOGRAPHYSTATELOG = DESCRIPTOR.message_types_by_name['ChoreographyStateLog']
 _DOWNLOADROBOTSTATELOGRESPONSE = DESCRIPTOR.message_types_by_name['DownloadRobotStateLogResponse']
 _MOVEPARAMS = DESCRIPTOR.message_types_by_name['MoveParams']
+_MOVECOMMAND = DESCRIPTOR.message_types_by_name['MoveCommand']
+_CHOREOGRAPHYCOMMANDREQUEST = DESCRIPTOR.message_types_by_name['ChoreographyCommandRequest']
+_CHOREOGRAPHYCOMMANDRESPONSE = DESCRIPTOR.message_types_by_name['ChoreographyCommandResponse']
 _MOVEINFO = DESCRIPTOR.message_types_by_name['MoveInfo']
 _CHOREOGRAPHERDISPLAYINFO = DESCRIPTOR.message_types_by_name['ChoreographerDisplayInfo']
 _CHOREOGRAPHERDISPLAYINFO_COLOR = _CHOREOGRAPHERDISPLAYINFO.nested_types_by_name['Color']
 _CHOREOGRAPHYSEQUENCE = DESCRIPTOR.message_types_by_name['ChoreographySequence']
 _CHOREOGRAPHYINFO = DESCRIPTOR.message_types_by_name['ChoreographyInfo']
 _CHOREOGRAPHERSAVE = DESCRIPTOR.message_types_by_name['ChoreographerSave']
 _ANIMATION = DESCRIPTOR.message_types_by_name['Animation']
@@ -68,27 +71,32 @@
 _ANIMATEARM = DESCRIPTOR.message_types_by_name['AnimateArm']
 _ANIMATEARM_HANDPOSE = _ANIMATEARM.nested_types_by_name['HandPose']
 _ARMJOINTANGLES = DESCRIPTOR.message_types_by_name['ArmJointAngles']
 _ANIMATEBODY = DESCRIPTOR.message_types_by_name['AnimateBody']
 _ANIMATELEGS = DESCRIPTOR.message_types_by_name['AnimateLegs']
 _ANIMATESINGLELEG = DESCRIPTOR.message_types_by_name['AnimateSingleLeg']
 _LEGJOINTANGLES = DESCRIPTOR.message_types_by_name['LegJointAngles']
+_ACTIVEMOVE = DESCRIPTOR.message_types_by_name['ActiveMove']
+_CHOREOGRAPHYSTATUSREQUEST = DESCRIPTOR.message_types_by_name['ChoreographyStatusRequest']
+_CHOREOGRAPHYSTATUSRESPONSE = DESCRIPTOR.message_types_by_name['ChoreographyStatusResponse']
 _SEQUENCEINFO_SAVEDSTATE = _SEQUENCEINFO.enum_types_by_name['SavedState']
 _DELETESEQUENCERESPONSE_STATUS = _DELETESEQUENCERESPONSE.enum_types_by_name['Status']
 _SAVESEQUENCERESPONSE_STATUS = _SAVESEQUENCERESPONSE.enum_types_by_name['Status']
 _MODIFYCHOREOGRAPHYINFORESPONSE_STATUS = _MODIFYCHOREOGRAPHYINFORESPONSE.enum_types_by_name['Status']
 _CLEARALLSEQUENCEFILESRESPONSE_STATUS = _CLEARALLSEQUENCEFILESRESPONSE.enum_types_by_name['Status']
 _UPLOADANIMATEDMOVERESPONSE_STATUS = _UPLOADANIMATEDMOVERESPONSE.enum_types_by_name['Status']
 _EXECUTECHOREOGRAPHYRESPONSE_STATUS = _EXECUTECHOREOGRAPHYRESPONSE.enum_types_by_name['Status']
 _STARTRECORDINGSTATERESPONSE_STATUS = _STARTRECORDINGSTATERESPONSE.enum_types_by_name['Status']
 _DOWNLOADROBOTSTATELOGREQUEST_LOGTYPE = _DOWNLOADROBOTSTATELOGREQUEST.enum_types_by_name['LogType']
 _DOWNLOADROBOTSTATELOGRESPONSE_STATUS = _DOWNLOADROBOTSTATELOGRESPONSE.enum_types_by_name['Status']
+_CHOREOGRAPHYCOMMANDRESPONSE_STATUS = _CHOREOGRAPHYCOMMANDRESPONSE.enum_types_by_name['Status']
 _MOVEINFO_TRANSITIONSTATE = _MOVEINFO.enum_types_by_name['TransitionState']
 _CHOREOGRAPHERDISPLAYINFO_CATEGORY = _CHOREOGRAPHERDISPLAYINFO.enum_types_by_name['Category']
 _ANIMATION_ARMPLAYBACK = _ANIMATION.enum_types_by_name['ArmPlayback']
+_CHOREOGRAPHYSTATUSRESPONSE_STATUS = _CHOREOGRAPHYSTATUSRESPONSE.enum_types_by_name['Status']
 ListAllMovesRequest = _reflection.GeneratedProtocolMessageType('ListAllMovesRequest', (_message.Message,), {
   'DESCRIPTOR' : _LISTALLMOVESREQUEST,
   '__module__' : 'bosdyn.api.spot.choreography_sequence_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.spot.ListAllMovesRequest)
   })
 _sym_db.RegisterMessage(ListAllMovesRequest)
 
@@ -291,14 +299,35 @@
 MoveParams = _reflection.GeneratedProtocolMessageType('MoveParams', (_message.Message,), {
   'DESCRIPTOR' : _MOVEPARAMS,
   '__module__' : 'bosdyn.api.spot.choreography_sequence_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.spot.MoveParams)
   })
 _sym_db.RegisterMessage(MoveParams)
 
+MoveCommand = _reflection.GeneratedProtocolMessageType('MoveCommand', (_message.Message,), {
+  'DESCRIPTOR' : _MOVECOMMAND,
+  '__module__' : 'bosdyn.api.spot.choreography_sequence_pb2'
+  # @@protoc_insertion_point(class_scope:bosdyn.api.spot.MoveCommand)
+  })
+_sym_db.RegisterMessage(MoveCommand)
+
+ChoreographyCommandRequest = _reflection.GeneratedProtocolMessageType('ChoreographyCommandRequest', (_message.Message,), {
+  'DESCRIPTOR' : _CHOREOGRAPHYCOMMANDREQUEST,
+  '__module__' : 'bosdyn.api.spot.choreography_sequence_pb2'
+  # @@protoc_insertion_point(class_scope:bosdyn.api.spot.ChoreographyCommandRequest)
+  })
+_sym_db.RegisterMessage(ChoreographyCommandRequest)
+
+ChoreographyCommandResponse = _reflection.GeneratedProtocolMessageType('ChoreographyCommandResponse', (_message.Message,), {
+  'DESCRIPTOR' : _CHOREOGRAPHYCOMMANDRESPONSE,
+  '__module__' : 'bosdyn.api.spot.choreography_sequence_pb2'
+  # @@protoc_insertion_point(class_scope:bosdyn.api.spot.ChoreographyCommandResponse)
+  })
+_sym_db.RegisterMessage(ChoreographyCommandResponse)
+
 MoveInfo = _reflection.GeneratedProtocolMessageType('MoveInfo', (_message.Message,), {
   'DESCRIPTOR' : _MOVEINFO,
   '__module__' : 'bosdyn.api.spot.choreography_sequence_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.spot.MoveInfo)
   })
 _sym_db.RegisterMessage(MoveInfo)
 
@@ -405,132 +434,171 @@
 LegJointAngles = _reflection.GeneratedProtocolMessageType('LegJointAngles', (_message.Message,), {
   'DESCRIPTOR' : _LEGJOINTANGLES,
   '__module__' : 'bosdyn.api.spot.choreography_sequence_pb2'
   # @@protoc_insertion_point(class_scope:bosdyn.api.spot.LegJointAngles)
   })
 _sym_db.RegisterMessage(LegJointAngles)
 
+ActiveMove = _reflection.GeneratedProtocolMessageType('ActiveMove', (_message.Message,), {
+  'DESCRIPTOR' : _ACTIVEMOVE,
+  '__module__' : 'bosdyn.api.spot.choreography_sequence_pb2'
+  # @@protoc_insertion_point(class_scope:bosdyn.api.spot.ActiveMove)
+  })
+_sym_db.RegisterMessage(ActiveMove)
+
+ChoreographyStatusRequest = _reflection.GeneratedProtocolMessageType('ChoreographyStatusRequest', (_message.Message,), {
+  'DESCRIPTOR' : _CHOREOGRAPHYSTATUSREQUEST,
+  '__module__' : 'bosdyn.api.spot.choreography_sequence_pb2'
+  # @@protoc_insertion_point(class_scope:bosdyn.api.spot.ChoreographyStatusRequest)
+  })
+_sym_db.RegisterMessage(ChoreographyStatusRequest)
+
+ChoreographyStatusResponse = _reflection.GeneratedProtocolMessageType('ChoreographyStatusResponse', (_message.Message,), {
+  'DESCRIPTOR' : _CHOREOGRAPHYSTATUSRESPONSE,
+  '__module__' : 'bosdyn.api.spot.choreography_sequence_pb2'
+  # @@protoc_insertion_point(class_scope:bosdyn.api.spot.ChoreographyStatusResponse)
+  })
+_sym_db.RegisterMessage(ChoreographyStatusResponse)
+
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'B\021ChoreographyProto'
   _LISTALLSEQUENCESRESPONSE.fields_by_name['known_sequences']._options = None
   _LISTALLSEQUENCESRESPONSE.fields_by_name['known_sequences']._serialized_options = b'\030\001'
+  _ANIMATION.fields_by_name['precise_timing']._options = None
+  _ANIMATION.fields_by_name['precise_timing']._serialized_options = b'\030\001'
   _LISTALLMOVESREQUEST._serialized_start=309
   _LISTALLMOVESREQUEST._serialized_end=373
   _LISTALLMOVESRESPONSE._serialized_start=376
   _LISTALLMOVESRESPONSE._serialized_end=511
   _LISTALLSEQUENCESREQUEST._serialized_start=513
   _LISTALLSEQUENCESREQUEST._serialized_end=581
   _LISTALLSEQUENCESRESPONSE._serialized_start=584
   _LISTALLSEQUENCESRESPONSE._serialized_end=737
   _SEQUENCEINFO._serialized_start=740
-  _SEQUENCEINFO._serialized_end=966
-  _SEQUENCEINFO_SAVEDSTATE._serialized_start=849
-  _SEQUENCEINFO_SAVEDSTATE._serialized_end=966
-  _DELETESEQUENCEREQUEST._serialized_start=968
-  _DELETESEQUENCEREQUEST._serialized_end=1057
-  _DELETESEQUENCERESPONSE._serialized_start=1060
-  _DELETESEQUENCERESPONSE._serialized_end=1328
-  _DELETESEQUENCERESPONSE_STATUS._serialized_start=1195
-  _DELETESEQUENCERESPONSE_STATUS._serialized_end=1328
-  _SAVESEQUENCEREQUEST._serialized_start=1330
-  _SAVESEQUENCEREQUEST._serialized_end=1437
-  _SAVESEQUENCERESPONSE._serialized_start=1440
-  _SAVESEQUENCERESPONSE._serialized_end=1701
-  _SAVESEQUENCERESPONSE_STATUS._serialized_start=1571
-  _SAVESEQUENCERESPONSE_STATUS._serialized_end=1701
-  _MODIFYCHOREOGRAPHYINFOREQUEST._serialized_start=1704
-  _MODIFYCHOREOGRAPHYINFOREQUEST._serialized_end=1844
-  _MODIFYCHOREOGRAPHYINFORESPONSE._serialized_start=1847
-  _MODIFYCHOREOGRAPHYINFORESPONSE._serialized_end=2130
-  _MODIFYCHOREOGRAPHYINFORESPONSE_STATUS._serialized_start=1998
-  _MODIFYCHOREOGRAPHYINFORESPONSE_STATUS._serialized_end=2130
-  _CLEARALLSEQUENCEFILESREQUEST._serialized_start=2132
-  _CLEARALLSEQUENCEFILESREQUEST._serialized_end=2205
-  _CLEARALLSEQUENCEFILESRESPONSE._serialized_start=2208
-  _CLEARALLSEQUENCEFILESRESPONSE._serialized_end=2428
-  _CLEARALLSEQUENCEFILESRESPONSE_STATUS._serialized_start=2356
-  _CLEARALLSEQUENCEFILESRESPONSE_STATUS._serialized_end=2428
-  _UPLOADCHOREOGRAPHYREQUEST._serialized_start=2431
-  _UPLOADCHOREOGRAPHYREQUEST._serialized_end=2599
-  _UPLOADCHOREOGRAPHYRESPONSE._serialized_start=2601
-  _UPLOADCHOREOGRAPHYRESPONSE._serialized_end=2691
-  _UPLOADANIMATEDMOVEREQUEST._serialized_start=2694
-  _UPLOADANIMATEDMOVEREQUEST._serialized_end=2881
-  _UPLOADANIMATEDMOVERESPONSE._serialized_start=2884
-  _UPLOADANIMATEDMOVERESPONSE._serialized_end=3153
-  _UPLOADANIMATEDMOVERESPONSE_STATUS._serialized_start=3044
-  _UPLOADANIMATEDMOVERESPONSE_STATUS._serialized_end=3153
-  _EXECUTECHOREOGRAPHYREQUEST._serialized_start=3156
-  _EXECUTECHOREOGRAPHYREQUEST._serialized_end=3382
-  _EXECUTECHOREOGRAPHYRESPONSE._serialized_start=3385
-  _EXECUTECHOREOGRAPHYRESPONSE._serialized_end=3726
-  _EXECUTECHOREOGRAPHYRESPONSE_STATUS._serialized_start=3584
-  _EXECUTECHOREOGRAPHYRESPONSE_STATUS._serialized_end=3726
-  _STARTRECORDINGSTATEREQUEST._serialized_start=3729
-  _STARTRECORDINGSTATEREQUEST._serialized_end=3894
-  _STARTRECORDINGSTATERESPONSE._serialized_start=3897
-  _STARTRECORDINGSTATERESPONSE._serialized_end=4189
-  _STARTRECORDINGSTATERESPONSE_STATUS._serialized_start=4071
-  _STARTRECORDINGSTATERESPONSE_STATUS._serialized_end=4189
-  _STOPRECORDINGSTATEREQUEST._serialized_start=4191
-  _STOPRECORDINGSTATEREQUEST._serialized_end=4261
-  _STOPRECORDINGSTATERESPONSE._serialized_start=4263
-  _STOPRECORDINGSTATERESPONSE._serialized_end=4335
-  _DOWNLOADROBOTSTATELOGREQUEST._serialized_start=4338
-  _DOWNLOADROBOTSTATELOGREQUEST._serialized_end=4570
-  _DOWNLOADROBOTSTATELOGREQUEST_LOGTYPE._serialized_start=4486
-  _DOWNLOADROBOTSTATELOGREQUEST_LOGTYPE._serialized_end=4570
-  _LOGGEDJOINTS._serialized_start=4573
-  _LOGGEDJOINTS._serialized_end=4866
-  _LOGGEDFOOTCONTACTS._serialized_start=4868
-  _LOGGEDFOOTCONTACTS._serialized_end=4968
-  _LOGGEDSTATEKEYFRAME._serialized_start=4971
-  _LOGGEDSTATEKEYFRAME._serialized_end=5208
-  _CHOREOGRAPHYSTATELOG._serialized_start=5210
-  _CHOREOGRAPHYSTATELOG._serialized_end=5290
-  _DOWNLOADROBOTSTATELOGRESPONSE._serialized_start=5293
-  _DOWNLOADROBOTSTATELOGRESPONSE._serialized_end=5586
-  _DOWNLOADROBOTSTATELOGRESPONSE_STATUS._serialized_start=5479
-  _DOWNLOADROBOTSTATELOGRESPONSE_STATUS._serialized_end=5586
-  _MOVEPARAMS._serialized_start=5589
-  _MOVEPARAMS._serialized_end=7693
-  _MOVEINFO._serialized_start=7696
-  _MOVEINFO._serialized_end=8464
-  _MOVEINFO_TRANSITIONSTATE._serialized_start=8306
-  _MOVEINFO_TRANSITIONSTATE._serialized_end=8464
-  _CHOREOGRAPHERDISPLAYINFO._serialized_start=8467
-  _CHOREOGRAPHERDISPLAYINFO._serialized_end=8980
-  _CHOREOGRAPHERDISPLAYINFO_COLOR._serialized_start=8682
-  _CHOREOGRAPHERDISPLAYINFO_COLOR._serialized_end=8733
-  _CHOREOGRAPHERDISPLAYINFO_CATEGORY._serialized_start=8736
-  _CHOREOGRAPHERDISPLAYINFO_CATEGORY._serialized_end=8980
-  _CHOREOGRAPHYSEQUENCE._serialized_start=8983
-  _CHOREOGRAPHYSEQUENCE._serialized_end=9152
-  _CHOREOGRAPHYINFO._serialized_start=9154
-  _CHOREOGRAPHYINFO._serialized_end=9188
-  _CHOREOGRAPHERSAVE._serialized_start=9191
-  _CHOREOGRAPHERSAVE._serialized_end=9361
-  _ANIMATION._serialized_start=9364
-  _ANIMATION._serialized_end=10223
-  _ANIMATION_ARMPLAYBACK._serialized_start=10087
-  _ANIMATION_ARMPLAYBACK._serialized_end=10223
-  _ANIMATIONKEYFRAME._serialized_start=10226
-  _ANIMATIONKEYFRAME._serialized_end=10439
-  _ANIMATEGRIPPER._serialized_start=10441
-  _ANIMATEGRIPPER._serialized_end=10510
-  _ANIMATEARM._serialized_start=10513
-  _ANIMATEARM._serialized_end=10819
-  _ANIMATEARM_HANDPOSE._serialized_start=10644
-  _ANIMATEARM_HANDPOSE._serialized_end=10812
-  _ARMJOINTANGLES._serialized_start=10822
-  _ARMJOINTANGLES._serialized_end=11126
-  _ANIMATEBODY._serialized_start=11129
-  _ANIMATEBODY._serialized_end=11356
-  _ANIMATELEGS._serialized_start=11359
-  _ANIMATELEGS._serialized_end=11560
-  _ANIMATESINGLELEG._serialized_start=11563
-  _ANIMATESINGLELEG._serialized_end=11732
-  _LEGJOINTANGLES._serialized_start=11734
-  _LEGJOINTANGLES._serialized_end=11794
+  _SEQUENCEINFO._serialized_end=1029
+  _SEQUENCEINFO_SAVEDSTATE._serialized_start=912
+  _SEQUENCEINFO_SAVEDSTATE._serialized_end=1029
+  _DELETESEQUENCEREQUEST._serialized_start=1031
+  _DELETESEQUENCEREQUEST._serialized_end=1120
+  _DELETESEQUENCERESPONSE._serialized_start=1123
+  _DELETESEQUENCERESPONSE._serialized_end=1391
+  _DELETESEQUENCERESPONSE_STATUS._serialized_start=1258
+  _DELETESEQUENCERESPONSE_STATUS._serialized_end=1391
+  _SAVESEQUENCEREQUEST._serialized_start=1393
+  _SAVESEQUENCEREQUEST._serialized_end=1500
+  _SAVESEQUENCERESPONSE._serialized_start=1503
+  _SAVESEQUENCERESPONSE._serialized_end=1764
+  _SAVESEQUENCERESPONSE_STATUS._serialized_start=1634
+  _SAVESEQUENCERESPONSE_STATUS._serialized_end=1764
+  _MODIFYCHOREOGRAPHYINFOREQUEST._serialized_start=1767
+  _MODIFYCHOREOGRAPHYINFOREQUEST._serialized_end=1907
+  _MODIFYCHOREOGRAPHYINFORESPONSE._serialized_start=1910
+  _MODIFYCHOREOGRAPHYINFORESPONSE._serialized_end=2193
+  _MODIFYCHOREOGRAPHYINFORESPONSE_STATUS._serialized_start=2061
+  _MODIFYCHOREOGRAPHYINFORESPONSE_STATUS._serialized_end=2193
+  _CLEARALLSEQUENCEFILESREQUEST._serialized_start=2195
+  _CLEARALLSEQUENCEFILESREQUEST._serialized_end=2268
+  _CLEARALLSEQUENCEFILESRESPONSE._serialized_start=2271
+  _CLEARALLSEQUENCEFILESRESPONSE._serialized_end=2491
+  _CLEARALLSEQUENCEFILESRESPONSE_STATUS._serialized_start=2419
+  _CLEARALLSEQUENCEFILESRESPONSE_STATUS._serialized_end=2491
+  _UPLOADCHOREOGRAPHYREQUEST._serialized_start=2494
+  _UPLOADCHOREOGRAPHYREQUEST._serialized_end=2662
+  _UPLOADCHOREOGRAPHYRESPONSE._serialized_start=2664
+  _UPLOADCHOREOGRAPHYRESPONSE._serialized_end=2754
+  _UPLOADANIMATEDMOVEREQUEST._serialized_start=2757
+  _UPLOADANIMATEDMOVEREQUEST._serialized_end=2944
+  _UPLOADANIMATEDMOVERESPONSE._serialized_start=2947
+  _UPLOADANIMATEDMOVERESPONSE._serialized_end=3216
+  _UPLOADANIMATEDMOVERESPONSE_STATUS._serialized_start=3107
+  _UPLOADANIMATEDMOVERESPONSE_STATUS._serialized_end=3216
+  _EXECUTECHOREOGRAPHYREQUEST._serialized_start=3219
+  _EXECUTECHOREOGRAPHYREQUEST._serialized_end=3445
+  _EXECUTECHOREOGRAPHYRESPONSE._serialized_start=3448
+  _EXECUTECHOREOGRAPHYRESPONSE._serialized_end=3811
+  _EXECUTECHOREOGRAPHYRESPONSE_STATUS._serialized_start=3669
+  _EXECUTECHOREOGRAPHYRESPONSE_STATUS._serialized_end=3811
+  _STARTRECORDINGSTATEREQUEST._serialized_start=3814
+  _STARTRECORDINGSTATEREQUEST._serialized_end=3979
+  _STARTRECORDINGSTATERESPONSE._serialized_start=3982
+  _STARTRECORDINGSTATERESPONSE._serialized_end=4274
+  _STARTRECORDINGSTATERESPONSE_STATUS._serialized_start=4156
+  _STARTRECORDINGSTATERESPONSE_STATUS._serialized_end=4274
+  _STOPRECORDINGSTATEREQUEST._serialized_start=4276
+  _STOPRECORDINGSTATEREQUEST._serialized_end=4346
+  _STOPRECORDINGSTATERESPONSE._serialized_start=4348
+  _STOPRECORDINGSTATERESPONSE._serialized_end=4420
+  _DOWNLOADROBOTSTATELOGREQUEST._serialized_start=4423
+  _DOWNLOADROBOTSTATELOGREQUEST._serialized_end=4655
+  _DOWNLOADROBOTSTATELOGREQUEST_LOGTYPE._serialized_start=4571
+  _DOWNLOADROBOTSTATELOGREQUEST_LOGTYPE._serialized_end=4655
+  _LOGGEDJOINTS._serialized_start=4658
+  _LOGGEDJOINTS._serialized_end=4951
+  _LOGGEDFOOTCONTACTS._serialized_start=4953
+  _LOGGEDFOOTCONTACTS._serialized_end=5053
+  _LOGGEDSTATEKEYFRAME._serialized_start=5056
+  _LOGGEDSTATEKEYFRAME._serialized_end=5293
+  _CHOREOGRAPHYSTATELOG._serialized_start=5295
+  _CHOREOGRAPHYSTATELOG._serialized_end=5375
+  _DOWNLOADROBOTSTATELOGRESPONSE._serialized_start=5378
+  _DOWNLOADROBOTSTATELOGRESPONSE._serialized_end=5671
+  _DOWNLOADROBOTSTATELOGRESPONSE_STATUS._serialized_start=5564
+  _DOWNLOADROBOTSTATELOGRESPONSE_STATUS._serialized_end=5671
+  _MOVEPARAMS._serialized_start=5674
+  _MOVEPARAMS._serialized_end=7916
+  _MOVECOMMAND._serialized_start=7918
+  _MOVECOMMAND._serialized_end=8045
+  _CHOREOGRAPHYCOMMANDREQUEST._serialized_start=8048
+  _CHOREOGRAPHYCOMMANDREQUEST._serialized_end=8255
+  _CHOREOGRAPHYCOMMANDRESPONSE._serialized_start=8258
+  _CHOREOGRAPHYCOMMANDRESPONSE._serialized_end=8648
+  _CHOREOGRAPHYCOMMANDRESPONSE_STATUS._serialized_start=8457
+  _CHOREOGRAPHYCOMMANDRESPONSE_STATUS._serialized_end=8648
+  _MOVEINFO._serialized_start=8651
+  _MOVEINFO._serialized_end=9439
+  _MOVEINFO_TRANSITIONSTATE._serialized_start=9281
+  _MOVEINFO_TRANSITIONSTATE._serialized_end=9439
+  _CHOREOGRAPHERDISPLAYINFO._serialized_start=9442
+  _CHOREOGRAPHERDISPLAYINFO._serialized_end=9955
+  _CHOREOGRAPHERDISPLAYINFO_COLOR._serialized_start=9657
+  _CHOREOGRAPHERDISPLAYINFO_COLOR._serialized_end=9708
+  _CHOREOGRAPHERDISPLAYINFO_CATEGORY._serialized_start=9711
+  _CHOREOGRAPHERDISPLAYINFO_CATEGORY._serialized_end=9955
+  _CHOREOGRAPHYSEQUENCE._serialized_start=9958
+  _CHOREOGRAPHYSEQUENCE._serialized_end=10194
+  _CHOREOGRAPHYINFO._serialized_start=10196
+  _CHOREOGRAPHYINFO._serialized_end=10230
+  _CHOREOGRAPHERSAVE._serialized_start=10233
+  _CHOREOGRAPHERSAVE._serialized_end=10403
+  _ANIMATION._serialized_start=10406
+  _ANIMATION._serialized_end=11350
+  _ANIMATION_ARMPLAYBACK._serialized_start=11214
+  _ANIMATION_ARMPLAYBACK._serialized_end=11350
+  _ANIMATIONKEYFRAME._serialized_start=11353
+  _ANIMATIONKEYFRAME._serialized_end=11566
+  _ANIMATEGRIPPER._serialized_start=11568
+  _ANIMATEGRIPPER._serialized_end=11637
+  _ANIMATEARM._serialized_start=11640
+  _ANIMATEARM._serialized_end=11946
+  _ANIMATEARM_HANDPOSE._serialized_start=11771
+  _ANIMATEARM_HANDPOSE._serialized_end=11939
+  _ARMJOINTANGLES._serialized_start=11949
+  _ARMJOINTANGLES._serialized_end=12253
+  _ANIMATEBODY._serialized_start=12256
+  _ANIMATEBODY._serialized_end=12483
+  _ANIMATELEGS._serialized_start=12486
+  _ANIMATELEGS._serialized_end=12687
+  _ANIMATESINGLELEG._serialized_start=12690
+  _ANIMATESINGLELEG._serialized_end=12859
+  _LEGJOINTANGLES._serialized_start=12861
+  _LEGJOINTANGLES._serialized_end=12921
+  _ACTIVEMOVE._serialized_start=12924
+  _ACTIVEMOVE._serialized_end=13077
+  _CHOREOGRAPHYSTATUSREQUEST._serialized_start=13079
+  _CHOREOGRAPHYSTATUSREQUEST._serialized_end=13149
+  _CHOREOGRAPHYSTATUSRESPONSE._serialized_start=13152
+  _CHOREOGRAPHYSTATUSRESPONSE._serialized_end=13746
+  _CHOREOGRAPHYSTATUSRESPONSE_STATUS._serialized_start=13503
+  _CHOREOGRAPHYSTATUSRESPONSE_STATUS._serialized_end=13746
 # @@protoc_insertion_point(module_scope)
```

## bosdyn/api/spot/choreography_service_pb2.py

```diff
@@ -11,19 +11,19 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from bosdyn.api.spot import choreography_sequence_pb2 as bosdyn_dot_api_dot_spot_dot_choreography__sequence__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n*bosdyn/api/spot/choreography_service.proto\x12\x0f\x62osdyn.api.spot\x1a+bosdyn/api/spot/choreography_sequence.proto2\xd1\n\n\x13\x43horeographyService\x12]\n\x0cListAllMoves\x12$.bosdyn.api.spot.ListAllMovesRequest\x1a%.bosdyn.api.spot.ListAllMovesResponse\"\x00\x12i\n\x10ListAllSequences\x12(.bosdyn.api.spot.ListAllSequencesRequest\x1a).bosdyn.api.spot.ListAllSequencesResponse\"\x00\x12\x63\n\x0e\x44\x65leteSequence\x12&.bosdyn.api.spot.DeleteSequenceRequest\x1a\'.bosdyn.api.spot.DeleteSequenceResponse\"\x00\x12]\n\x0cSaveSequence\x12$.bosdyn.api.spot.SaveSequenceRequest\x1a%.bosdyn.api.spot.SaveSequenceResponse\"\x00\x12{\n\x16ModifyChoreographyInfo\x12..bosdyn.api.spot.ModifyChoreographyInfoRequest\x1a/.bosdyn.api.spot.ModifyChoreographyInfoResponse\"\x00\x12x\n\x15\x43learAllSequenceFiles\x12-.bosdyn.api.spot.ClearAllSequenceFilesRequest\x1a..bosdyn.api.spot.ClearAllSequenceFilesResponse\"\x00\x12o\n\x12UploadChoreography\x12*.bosdyn.api.spot.UploadChoreographyRequest\x1a+.bosdyn.api.spot.UploadChoreographyResponse\"\x00\x12o\n\x12UploadAnimatedMove\x12*.bosdyn.api.spot.UploadAnimatedMoveRequest\x1a+.bosdyn.api.spot.UploadAnimatedMoveResponse\"\x00\x12r\n\x13\x45xecuteChoreography\x12+.bosdyn.api.spot.ExecuteChoreographyRequest\x1a,.bosdyn.api.spot.ExecuteChoreographyResponse\"\x00\x12r\n\x13StartRecordingState\x12+.bosdyn.api.spot.StartRecordingStateRequest\x1a,.bosdyn.api.spot.StartRecordingStateResponse\"\x00\x12o\n\x12StopRecordingState\x12*.bosdyn.api.spot.StopRecordingStateRequest\x1a+.bosdyn.api.spot.StopRecordingStateResponse\"\x00\x12z\n\x15\x44ownloadRobotStateLog\x12-.bosdyn.api.spot.DownloadRobotStateLogRequest\x1a..bosdyn.api.spot.DownloadRobotStateLogResponse\"\x00\x30\x01\x42\x1a\x42\x18\x43horeographyServiceProtob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n*bosdyn/api/spot/choreography_service.proto\x12\x0f\x62osdyn.api.spot\x1a+bosdyn/api/spot/choreography_sequence.proto2\xb6\x0c\n\x13\x43horeographyService\x12]\n\x0cListAllMoves\x12$.bosdyn.api.spot.ListAllMovesRequest\x1a%.bosdyn.api.spot.ListAllMovesResponse\"\x00\x12i\n\x10ListAllSequences\x12(.bosdyn.api.spot.ListAllSequencesRequest\x1a).bosdyn.api.spot.ListAllSequencesResponse\"\x00\x12\x63\n\x0e\x44\x65leteSequence\x12&.bosdyn.api.spot.DeleteSequenceRequest\x1a\'.bosdyn.api.spot.DeleteSequenceResponse\"\x00\x12]\n\x0cSaveSequence\x12$.bosdyn.api.spot.SaveSequenceRequest\x1a%.bosdyn.api.spot.SaveSequenceResponse\"\x00\x12{\n\x16ModifyChoreographyInfo\x12..bosdyn.api.spot.ModifyChoreographyInfoRequest\x1a/.bosdyn.api.spot.ModifyChoreographyInfoResponse\"\x00\x12x\n\x15\x43learAllSequenceFiles\x12-.bosdyn.api.spot.ClearAllSequenceFilesRequest\x1a..bosdyn.api.spot.ClearAllSequenceFilesResponse\"\x00\x12o\n\x12UploadChoreography\x12*.bosdyn.api.spot.UploadChoreographyRequest\x1a+.bosdyn.api.spot.UploadChoreographyResponse\"\x00\x12o\n\x12UploadAnimatedMove\x12*.bosdyn.api.spot.UploadAnimatedMoveRequest\x1a+.bosdyn.api.spot.UploadAnimatedMoveResponse\"\x00\x12r\n\x13\x45xecuteChoreography\x12+.bosdyn.api.spot.ExecuteChoreographyRequest\x1a,.bosdyn.api.spot.ExecuteChoreographyResponse\"\x00\x12r\n\x13StartRecordingState\x12+.bosdyn.api.spot.StartRecordingStateRequest\x1a,.bosdyn.api.spot.StartRecordingStateResponse\"\x00\x12o\n\x12StopRecordingState\x12*.bosdyn.api.spot.StopRecordingStateRequest\x1a+.bosdyn.api.spot.StopRecordingStateResponse\"\x00\x12z\n\x15\x44ownloadRobotStateLog\x12-.bosdyn.api.spot.DownloadRobotStateLogRequest\x1a..bosdyn.api.spot.DownloadRobotStateLogResponse\"\x00\x30\x01\x12o\n\x12\x43horeographyStatus\x12*.bosdyn.api.spot.ChoreographyStatusRequest\x1a+.bosdyn.api.spot.ChoreographyStatusResponse\"\x00\x12r\n\x13\x43horeographyCommand\x12+.bosdyn.api.spot.ChoreographyCommandRequest\x1a,.bosdyn.api.spot.ChoreographyCommandResponse\"\x00\x42\x1a\x42\x18\x43horeographyServiceProtob\x06proto3')
 
 
 
 _CHOREOGRAPHYSERVICE = DESCRIPTOR.services_by_name['ChoreographyService']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'B\030ChoreographyServiceProto'
   _CHOREOGRAPHYSERVICE._serialized_start=109
-  _CHOREOGRAPHYSERVICE._serialized_end=1470
+  _CHOREOGRAPHYSERVICE._serialized_end=1699
 # @@protoc_insertion_point(module_scope)
```

## bosdyn/api/spot/choreography_service_pb2_grpc.py

```diff
@@ -70,14 +70,24 @@
                 response_deserializer=bosdyn_dot_api_dot_spot_dot_choreography__sequence__pb2.StopRecordingStateResponse.FromString,
                 )
         self.DownloadRobotStateLog = channel.unary_stream(
                 '/bosdyn.api.spot.ChoreographyService/DownloadRobotStateLog',
                 request_serializer=bosdyn_dot_api_dot_spot_dot_choreography__sequence__pb2.DownloadRobotStateLogRequest.SerializeToString,
                 response_deserializer=bosdyn_dot_api_dot_spot_dot_choreography__sequence__pb2.DownloadRobotStateLogResponse.FromString,
                 )
+        self.ChoreographyStatus = channel.unary_unary(
+                '/bosdyn.api.spot.ChoreographyService/ChoreographyStatus',
+                request_serializer=bosdyn_dot_api_dot_spot_dot_choreography__sequence__pb2.ChoreographyStatusRequest.SerializeToString,
+                response_deserializer=bosdyn_dot_api_dot_spot_dot_choreography__sequence__pb2.ChoreographyStatusResponse.FromString,
+                )
+        self.ChoreographyCommand = channel.unary_unary(
+                '/bosdyn.api.spot.ChoreographyService/ChoreographyCommand',
+                request_serializer=bosdyn_dot_api_dot_spot_dot_choreography__sequence__pb2.ChoreographyCommandRequest.SerializeToString,
+                response_deserializer=bosdyn_dot_api_dot_spot_dot_choreography__sequence__pb2.ChoreographyCommandResponse.FromString,
+                )
 
 
 class ChoreographyServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def ListAllMoves(self, request, context):
         """List the available dance moves and their parameter information.
@@ -161,14 +171,28 @@
     def DownloadRobotStateLog(self, request, context):
         """Download log of the latest recorded robot state information.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def ChoreographyStatus(self, request, context):
+        """Report the status of a dancing robot.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def ChoreographyCommand(self, request, context):
+        """Commands intended for individual dance moves that are currently executing.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_ChoreographyServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'ListAllMoves': grpc.unary_unary_rpc_method_handler(
                     servicer.ListAllMoves,
                     request_deserializer=bosdyn_dot_api_dot_spot_dot_choreography__sequence__pb2.ListAllMovesRequest.FromString,
                     response_serializer=bosdyn_dot_api_dot_spot_dot_choreography__sequence__pb2.ListAllMovesResponse.SerializeToString,
@@ -224,14 +248,24 @@
                     response_serializer=bosdyn_dot_api_dot_spot_dot_choreography__sequence__pb2.StopRecordingStateResponse.SerializeToString,
             ),
             'DownloadRobotStateLog': grpc.unary_stream_rpc_method_handler(
                     servicer.DownloadRobotStateLog,
                     request_deserializer=bosdyn_dot_api_dot_spot_dot_choreography__sequence__pb2.DownloadRobotStateLogRequest.FromString,
                     response_serializer=bosdyn_dot_api_dot_spot_dot_choreography__sequence__pb2.DownloadRobotStateLogResponse.SerializeToString,
             ),
+            'ChoreographyStatus': grpc.unary_unary_rpc_method_handler(
+                    servicer.ChoreographyStatus,
+                    request_deserializer=bosdyn_dot_api_dot_spot_dot_choreography__sequence__pb2.ChoreographyStatusRequest.FromString,
+                    response_serializer=bosdyn_dot_api_dot_spot_dot_choreography__sequence__pb2.ChoreographyStatusResponse.SerializeToString,
+            ),
+            'ChoreographyCommand': grpc.unary_unary_rpc_method_handler(
+                    servicer.ChoreographyCommand,
+                    request_deserializer=bosdyn_dot_api_dot_spot_dot_choreography__sequence__pb2.ChoreographyCommandRequest.FromString,
+                    response_serializer=bosdyn_dot_api_dot_spot_dot_choreography__sequence__pb2.ChoreographyCommandResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'bosdyn.api.spot.ChoreographyService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -437,7 +471,41 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_stream(request, target, '/bosdyn.api.spot.ChoreographyService/DownloadRobotStateLog',
             bosdyn_dot_api_dot_spot_dot_choreography__sequence__pb2.DownloadRobotStateLogRequest.SerializeToString,
             bosdyn_dot_api_dot_spot_dot_choreography__sequence__pb2.DownloadRobotStateLogResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def ChoreographyStatus(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/bosdyn.api.spot.ChoreographyService/ChoreographyStatus',
+            bosdyn_dot_api_dot_spot_dot_choreography__sequence__pb2.ChoreographyStatusRequest.SerializeToString,
+            bosdyn_dot_api_dot_spot_dot_choreography__sequence__pb2.ChoreographyStatusResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def ChoreographyCommand(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/bosdyn.api.spot.ChoreographyService/ChoreographyCommand',
+            bosdyn_dot_api_dot_spot_dot_choreography__sequence__pb2.ChoreographyCommandRequest.SerializeToString,
+            bosdyn_dot_api_dot_spot_dot_choreography__sequence__pb2.ChoreographyCommandResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

## Comparing `bosdyn_choreography_protos-3.2.3.dist-info/METADATA` & `bosdyn_choreography_protos-3.3.0.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: bosdyn-choreography-protos
-Version: 3.2.3
+Version: 3.3.0
 Summary: Boston Dynamics API Choreography protobufs
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
 Requires-Dist: protobuf (>=3.3.0)
 
 <!--
-Copyright (c) 2022 Boston Dynamics, Inc.  All rights reserved.
+Copyright (c) 2023 Boston Dynamics, Inc.  All rights reserved.
 
 Downloading, reproducing, distributing or otherwise using the SDK Software
 is subject to the terms and conditions of the Boston Dynamics Software
 Development Kit License (20191101-BDSDK-SL).
 -->
 
 # bosdyn-choreography-protos
 
 <p align="center">
 <img src="https://www.bostondynamics.com/sites/default/files/2020-05/spot.png" style="max-width:50%;">
 </p>
 
 The bosdyn-choreography-protos wheel contains the Protobuf definitions in the Boston Dynamics Choreography API. The message and service types defined in this wheel are used by the clients in [bosdyn-choreography-client](https://pypi.org/project/bosdyn-choreography-client/) wheel to communicate with the services running on the Spot robots.
-
-
```

