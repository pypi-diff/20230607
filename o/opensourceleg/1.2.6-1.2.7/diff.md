# Comparing `tmp/opensourceleg-1.2.6.tar.gz` & `tmp/opensourceleg-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opensourceleg-1.2.6.tar", max compression
+gzip compressed data, was "opensourceleg-1.2.7.tar", max compression
```

## Comparing `opensourceleg-1.2.6.tar` & `opensourceleg-1.2.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    32471 2023-01-26 01:08:26.114591 opensourceleg-1.2.6/LICENSE
--rw-r--r--   0        0        0     1510 2023-04-13 18:12:03.062127 opensourceleg-1.2.6/README.md
--rw-r--r--   0        0        0      411 2023-04-13 17:30:19.791723 opensourceleg-1.2.6/opensourceleg/__init__.py
--rw-r--r--   0        0        0    22954 2023-06-06 02:22:42.448913 opensourceleg-1.2.6/opensourceleg/actuators.py
--rw-r--r--   0        0        0      136 2023-06-05 20:47:17.478958 opensourceleg-1.2.6/opensourceleg/ankle_encoder_map.npy
--rw-r--r--   0        0        0     1156 2023-06-06 13:48:00.772459 opensourceleg-1.2.6/opensourceleg/constants.py
--rw-r--r--   0        0        0      805 2023-06-06 13:04:42.094571 opensourceleg-1.2.6/opensourceleg/control.py
--rw-r--r--   0        0        0     6550 2023-06-06 14:57:46.304774 opensourceleg-1.2.6/opensourceleg/demo.py
--rw-r--r--   0        0        0      184 2023-05-11 15:09:10.436317 opensourceleg-1.2.6/opensourceleg/example.py
--rw-r--r--   0        0        0    10820 2023-06-06 14:59:16.262812 opensourceleg-1.2.6/opensourceleg/joints.py
--rw-r--r--   0        0        0      136 2023-03-19 23:25:36.020226 opensourceleg-1.2.6/opensourceleg/knee_encoder_map.npy
--rw-r--r--   0        0        0     8513 2023-06-06 02:25:22.342625 opensourceleg-1.2.6/opensourceleg/loadcell.py
--rw-r--r--   0        0        0     3799 2023-06-02 05:24:50.983197 opensourceleg-1.2.6/opensourceleg/logger.py
--rw-r--r--   0        0        0    17217 2023-06-06 15:00:18.710389 opensourceleg-1.2.6/opensourceleg/osl.py
--rw-r--r--   0        0        0    14963 2023-06-05 15:50:42.804893 opensourceleg-1.2.6/opensourceleg/state_machine.py
--rw-r--r--   0        0        0     6361 2023-06-02 18:52:35.890633 opensourceleg-1.2.6/opensourceleg/thermal.py
--rw-r--r--   0        0        0    21242 2023-06-06 15:01:15.079436 opensourceleg-1.2.6/opensourceleg/tui.py
--rw-r--r--   0        0        0     4331 2023-06-05 20:47:20.793114 opensourceleg-1.2.6/opensourceleg/units.py
--rw-r--r--   0        0        0    11587 2023-06-06 02:26:59.481937 opensourceleg-1.2.6/opensourceleg/utilities.py
--rw-r--r--   0        0        0     3668 2023-06-06 15:01:21.796614 opensourceleg-1.2.6/pyproject.toml
--rw-r--r--   0        0        0     2825 1970-01-01 00:00:00.000000 opensourceleg-1.2.6/PKG-INFO
+-rw-r--r--   0        0        0    32471 2023-01-26 01:08:26.114591 opensourceleg-1.2.7/LICENSE
+-rw-r--r--   0        0        0     1510 2023-04-13 18:12:03.062127 opensourceleg-1.2.7/README.md
+-rw-r--r--   0        0        0      411 2023-04-13 17:30:19.791723 opensourceleg-1.2.7/opensourceleg/__init__.py
+-rw-r--r--   0        0        0    22954 2023-06-06 02:22:42.448913 opensourceleg-1.2.7/opensourceleg/actuators.py
+-rw-r--r--   0        0        0      136 2023-06-05 20:47:17.478958 opensourceleg-1.2.7/opensourceleg/ankle_encoder_map.npy
+-rw-r--r--   0        0        0     1156 2023-06-06 13:48:00.772459 opensourceleg-1.2.7/opensourceleg/constants.py
+-rw-r--r--   0        0        0      805 2023-06-06 13:04:42.094571 opensourceleg-1.2.7/opensourceleg/control.py
+-rw-r--r--   0        0        0     6668 2023-06-07 03:52:26.170016 opensourceleg-1.2.7/opensourceleg/demo.py
+-rw-r--r--   0        0        0      184 2023-05-11 15:09:10.436317 opensourceleg-1.2.7/opensourceleg/example.py
+-rw-r--r--   0        0        0    10820 2023-06-06 14:59:16.262812 opensourceleg-1.2.7/opensourceleg/joints.py
+-rw-r--r--   0        0        0      136 2023-03-19 23:25:36.020226 opensourceleg-1.2.7/opensourceleg/knee_encoder_map.npy
+-rw-r--r--   0        0        0     8513 2023-06-06 02:25:22.342625 opensourceleg-1.2.7/opensourceleg/loadcell.py
+-rw-r--r--   0        0        0     3799 2023-06-02 05:24:50.983197 opensourceleg-1.2.7/opensourceleg/logger.py
+-rw-r--r--   0        0        0    17214 2023-06-07 03:50:21.478357 opensourceleg-1.2.7/opensourceleg/osl.py
+-rw-r--r--   0        0        0    14963 2023-06-05 15:50:42.804893 opensourceleg-1.2.7/opensourceleg/state_machine.py
+-rw-r--r--   0        0        0     6361 2023-06-02 18:52:35.890633 opensourceleg-1.2.7/opensourceleg/thermal.py
+-rw-r--r--   0        0        0    21242 2023-06-07 02:24:24.140310 opensourceleg-1.2.7/opensourceleg/tui.py
+-rw-r--r--   0        0        0     4331 2023-06-05 20:47:20.793114 opensourceleg-1.2.7/opensourceleg/units.py
+-rw-r--r--   0        0        0    11587 2023-06-06 02:26:59.481937 opensourceleg-1.2.7/opensourceleg/utilities.py
+-rw-r--r--   0        0        0     3668 2023-06-07 03:53:10.358519 opensourceleg-1.2.7/pyproject.toml
+-rw-r--r--   0        0        0     2825 1970-01-01 00:00:00.000000 opensourceleg-1.2.7/PKG-INFO
```

### Comparing `opensourceleg-1.2.6/LICENSE` & `opensourceleg-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.6/README.md` & `opensourceleg-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.6/opensourceleg/actuators.py` & `opensourceleg-1.2.7/opensourceleg/actuators.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.6/opensourceleg/constants.py` & `opensourceleg-1.2.7/opensourceleg/constants.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.6/opensourceleg/control.py` & `opensourceleg-1.2.7/opensourceleg/control.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.6/opensourceleg/demo.py` & `opensourceleg-1.2.7/opensourceleg/demo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,79 +1,83 @@
 import time
 
 from opensourceleg.osl import OpenSourceLeg
 from opensourceleg.state_machine import Event, State
 
 # ------------- FSM PARAMETERS ---------------- #
 
-BODY_WEIGHT = 130
+BODY_WEIGHT = 80
 
 # STATE 1: EARLY STANCE
 
-KNEE_K_ESTANCE = 130
-KNEE_B_ESTANCE = 0
+KNEE_K_ESTANCE = 250
+KNEE_B_ESTANCE = 1000
 KNEE_THETA_ESTANCE = 5
 
-LOAD_LSTANCE: float = -1.0 * BODY_WEIGHT * 0.3 * 4.4
+LOAD_LSTANCE: float = -1.0 * BODY_WEIGHT * 0.25
+ANKLE_THETA_ESTANCE_TO_LSTANCE = 6.0
 
 ANKLE_K_ESTANCE = 50
 ANKLE_B_ESTANCE = 0
-ANKLE_THETA_ESTANCE = 0
+ANKLE_THETA_ESTANCE = -2
 
 # --------------------------------------------- #
 # STATE 2: LATE STANCE
 
-KNEE_K_LSTANCE = 150
-KNEE_B_LSTANCE = 0
-KNEE_THETA_LSTANCE = 5
-
-LOAD_ESWING: float = -1.0 * BODY_WEIGHT * 0.2 * 4.4
-
-ANKLE_K_LSTANCE = 90
-ANKLE_B_LSTANCE = 0
-ANKLE_THETA_LSTANCE = 15
+KNEE_K_LSTANCE = 250
+KNEE_B_LSTANCE = 400
+KNEE_THETA_LSTANCE = 8
+
+LOAD_ESWING: float = -1.0 * BODY_WEIGHT * 0.15
+
+ANKLE_K_LSTANCE = 200
+ANKLE_B_LSTANCE = 20
+ANKLE_THETA_LSTANCE = -20
 
 # --------------------------------------------- #
 # STATE 3: EARLY SWING
 
-KNEE_K_ESWING = 30
-KNEE_B_ESWING = 40
-KNEE_THETA_ESWING = 85
+KNEE_K_ESWING = 100
+KNEE_B_ESWING = 20
+KNEE_THETA_ESWING = 65
 
-KNEE_THETA_ESWING_TO_LSWING = 60
+KNEE_THETA_ESWING_TO_LSWING = 55
 KNEE_DTHETA_ESWING_TO_LSWING = 3
 
 ANKLE_K_ESWING = 20
 ANKLE_B_ESWING = 0
-ANKLE_THETA_ESWING = -25
+ANKLE_THETA_ESWING = 25
 
 # --------------------------------------------- #
 # STATE 4: LATE SWING
 
-KNEE_K_LSWING = 20
-KNEE_B_LSWING = 60
+KNEE_K_LSWING = 40
+KNEE_B_LSWING = 1200
 KNEE_THETA_LSWING = 5
 
-LOAD_ESTANCE: float = -1.0 * BODY_WEIGHT * 0.3 * 4.4
-KNEE_THETA_LSWING_TO_ESTANCE = 20
+LOAD_ESTANCE: float = -1.0 * BODY_WEIGHT * 0.4
+KNEE_THETA_LSWING_TO_ESTANCE = 30
 
 ANKLE_K_LSWING = 20
 ANKLE_B_LSWING = 0
-ANKLE_THETA_LSWING = -25
+ANKLE_THETA_LSWING = 15
 
 # ------------- FSM TRANSITIONS --------------- #
 
 
 def estance_to_lstance(osl: OpenSourceLeg) -> bool:
     """
     Transition from early stance to late stance when the loadcell
     reads a force greater than a threshold.
     """
     assert osl.loadcell is not None
-    if osl.loadcell.fz < LOAD_ESTANCE:
+    if (
+        osl.loadcell.fz < LOAD_LSTANCE
+        and osl.ankle.output_position > ANKLE_THETA_ESTANCE_TO_LSTANCE
+    ):
         return True
     else:
         return False
 
 
 def lstance_to_eswing(osl: OpenSourceLeg) -> bool:
     """
@@ -91,15 +95,15 @@
     """
     Transition from early swing to late swing when the knee angle
     is greater than a threshold and the knee velocity is less than
     a threshold.
     """
     assert osl.knee is not None
     if (
-        osl.knee.output_position < KNEE_THETA_ESWING_TO_LSWING
+        osl.knee.output_position > KNEE_THETA_ESWING_TO_LSWING
         and osl.knee.output_velocity < KNEE_DTHETA_ESWING_TO_LSWING
     ):
         return True
     else:
         return False
 
 
@@ -120,15 +124,15 @@
     Transition from late swing to early stance when the loadcell
     reads a force greater than a threshold or the knee angle is
     less than a threshold.
     """
     assert osl.knee is not None and osl.loadcell is not None
     if (
         osl.loadcell.fz < LOAD_ESTANCE
-        or osl.knee.output_position > KNEE_THETA_LSWING_TO_ESTANCE
+        or osl.knee.output_position < KNEE_THETA_LSWING_TO_ESTANCE
     ):
         return True
     else:
         return False
 
 
 def state_machine_controller():
@@ -146,15 +150,15 @@
         gear_ratio=41.4999,
     )
 
     osl.add_loadcell(
         dephy_mode=False,
     )
 
-    osl.add_state_machine(spoof=True)
+    osl.add_state_machine(spoof=False)
 
     early_stance = State(name="e_stance")
     early_stance.set_knee_impedance_paramters(
         theta=KNEE_THETA_ESTANCE, k=KNEE_K_ESTANCE, b=KNEE_B_ESTANCE
     )
     early_stance.make_knee_active()
```

### Comparing `opensourceleg-1.2.6/opensourceleg/joints.py` & `opensourceleg-1.2.7/opensourceleg/joints.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.6/opensourceleg/loadcell.py` & `opensourceleg-1.2.7/opensourceleg/loadcell.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.6/opensourceleg/logger.py` & `opensourceleg-1.2.7/opensourceleg/logger.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.6/opensourceleg/osl.py` & `opensourceleg-1.2.7/opensourceleg/osl.py`

 * *Files 0% similar despite different names*

```diff
@@ -365,19 +365,20 @@
             osl.log.warn(
                 f"[OSL] Please run the homing routine by calling `osl.home()` before starting the state-machine."
             )
             exit()
 
         self.update(set_state_machine_parameters=set_state_machine_parameters)
 
+        time.sleep(0.1)
+
         if not self.has_tui:
             self.update(set_state_machine_parameters=set_state_machine_parameters)
 
         else:
-            time.sleep(0.1)
             self.tui.add_update_callback(callback=self.update, args=set_state_machine_parameters)  # type: ignore
             self.tui.run()  # type: ignore
 
     def initialize_sm_tui(self) -> None:
 
         from opensourceleg.tui import COLORS
```

### Comparing `opensourceleg-1.2.6/opensourceleg/state_machine.py` & `opensourceleg-1.2.7/opensourceleg/state_machine.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.6/opensourceleg/thermal.py` & `opensourceleg-1.2.7/opensourceleg/thermal.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.6/opensourceleg/tui.py` & `opensourceleg-1.2.7/opensourceleg/tui.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.6/opensourceleg/units.py` & `opensourceleg-1.2.7/opensourceleg/units.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.6/opensourceleg/utilities.py` & `opensourceleg-1.2.7/opensourceleg/utilities.py`

 * *Files identical despite different names*

### Comparing `opensourceleg-1.2.6/pyproject.toml` & `opensourceleg-1.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "opensourceleg"
-version = "1.2.6"
+version = "1.2.7"
 description = "An open-source software library for numerical computation, data acquisition, and control of lower-limb robotic prosthesis."
 readme = "README.md"
 authors = ["Open-source Leg <opensourceleg@gmail.com>"]
 license = "GNU GPL v3.0"
 repository = "https://github.com/neurobionics/opensourceleg"
 homepage = "https://github.com/neurobionics/opensourceleg"
```

### Comparing `opensourceleg-1.2.6/PKG-INFO` & `opensourceleg-1.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opensourceleg
-Version: 1.2.6
+Version: 1.2.7
 Summary: An open-source software library for numerical computation, data acquisition, and control of lower-limb robotic prosthesis.
 Home-page: https://github.com/neurobionics/opensourceleg
 License: GNU GPL v3.0
 Author: Open-source Leg
 Author-email: opensourceleg@gmail.com
 Requires-Python: >=3.9,<4.0.0
 Classifier: Development Status :: 3 - Alpha
```

