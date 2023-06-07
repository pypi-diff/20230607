# Comparing `tmp/weconnect-cupra-daern-0.49.20.tar.gz` & `tmp/weconnect-cupra-daern-0.50.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weconnect-cupra-daern-0.49.20.tar", last modified: Fri Jun  2 08:46:43 2023, max compression
+gzip compressed data, was "weconnect-cupra-daern-0.50.1.tar", last modified: Wed Jun  7 21:37:55 2023, max compression
```

## Comparing `weconnect-cupra-daern-0.49.20.tar` & `weconnect-cupra-daern-0.50.1.tar`

### file list

```diff
@@ -1,122 +1,113 @@
-drwxr-xr-x   0 daern     (1000) daern     (1000)        0 2023-06-02 08:46:43.897645 weconnect-cupra-daern-0.49.20/
--rw-r--r--   0 daern     (1000) daern     (1000)       51 2023-03-23 10:39:07.000000 weconnect-cupra-daern-0.49.20/MANIFEST.in
--rw-r--r--   0 daern     (1000) daern     (1000)     5580 2023-06-02 08:46:43.897645 weconnect-cupra-daern-0.49.20/PKG-INFO
--rw-r--r--   0 daern     (1000) daern     (1000)     4046 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/README.md
--rw-r--r--   0 daern     (1000) daern     (1000)     2998 2023-06-02 08:46:43.897645 weconnect-cupra-daern-0.49.20/setup.cfg
--rw-r--r--   0 daern     (1000) daern     (1000)     1924 2023-03-23 09:54:10.000000 weconnect-cupra-daern-0.49.20/setup.py
-drwxr-xr-x   0 daern     (1000) daern     (1000)        0 2023-06-02 08:46:43.887645 weconnect-cupra-daern-0.49.20/tests/
--rw-r--r--   0 daern     (1000) daern     (1000)        0 2023-01-12 20:52:24.000000 weconnect-cupra-daern-0.49.20/tests/__init__.py
--rw-r--r--   0 daern     (1000) daern     (1000)     8774 2023-01-12 20:52:24.000000 weconnect-cupra-daern-0.49.20/tests/test_addressable.py
--rw-r--r--   0 daern     (1000) daern     (1000)    13494 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/tests/test_cupra.py
--rw-r--r--   0 daern     (1000) daern     (1000)     1002 2023-01-12 20:52:24.000000 weconnect-cupra-daern-0.49.20/tests/test_elements.py
-drwxr-xr-x   0 daern     (1000) daern     (1000)        0 2023-06-02 08:46:43.887645 weconnect-cupra-daern-0.49.20/weconnect/
--rw-r--r--   0 daern     (1000) daern     (1000)        0 2023-01-12 20:52:24.000000 weconnect-cupra-daern-0.49.20/weconnect/__init__.py
--rw-r--r--   0 daern     (1000) daern     (1000)       24 2023-06-02 08:46:17.000000 weconnect-cupra-daern-0.49.20/weconnect/__version.py
--rw-r--r--   0 daern     (1000) daern     (1000)    25432 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/addressable.py
-drwxr-xr-x   0 daern     (1000) daern     (1000)        0 2023-06-02 08:46:43.887645 weconnect-cupra-daern-0.49.20/weconnect/api/
--rw-r--r--   0 daern     (1000) daern     (1000)        0 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/__init__.py
-drwxr-xr-x   0 daern     (1000) daern     (1000)        0 2023-06-02 08:46:43.887645 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/
--rw-r--r--   0 daern     (1000) daern     (1000)        0 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/__init__.py
--rw-r--r--   0 daern     (1000) daern     (1000)     3885 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/api.py
-drwxr-xr-x   0 daern     (1000) daern     (1000)        0 2023-06-02 08:46:43.887645 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/auth/
--rw-r--r--   0 daern     (1000) daern     (1000)        0 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/auth/__init__.py
--rw-r--r--   0 daern     (1000) daern     (1000)    17224 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/auth/my_cupra_session.py
--rw-r--r--   0 daern     (1000) daern     (1000)      362 2023-03-09 16:56:41.000000 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/domain.py
-drwxr-xr-x   0 daern     (1000) daern     (1000)        0 2023-06-02 08:46:43.887645 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/
--rw-r--r--   0 daern     (1000) daern     (1000)        0 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/__init__.py
--rw-r--r--   0 daern     (1000) daern     (1000)    12708 2023-03-10 15:19:25.000000 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/access_status.py
--rw-r--r--   0 daern     (1000) daern     (1000)     2670 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/battery_status.py
--rw-r--r--   0 daern     (1000) daern     (1000)     4483 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/charging_settings.py
--rw-r--r--   0 daern     (1000) daern     (1000)    14443 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/charging_station.py
--rw-r--r--   0 daern     (1000) daern     (1000)     7736 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/charging_status.py
--rw-r--r--   0 daern     (1000) daern     (1000)     8558 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/climatization_settings.py
--rw-r--r--   0 daern     (1000) daern     (1000)     2762 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/climatization_status.py
--rw-r--r--   0 daern     (1000) daern     (1000)    12294 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/controls.py
--rw-r--r--   0 daern     (1000) daern     (1000)     2228 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/engine_state.py
--rw-r--r--   0 daern     (1000) daern     (1000)      796 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/enums.py
--rw-r--r--   0 daern     (1000) daern     (1000)     3424 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/error.py
--rw-r--r--   0 daern     (1000) daern     (1000)     3387 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/generic_capability.py
--rw-r--r--   0 daern     (1000) daern     (1000)     5260 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/generic_settings.py
-drwxr-xr-x   0 daern     (1000) daern     (1000)        0 2023-06-02 08:46:43.887645 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/helpers/
--rw-r--r--   0 daern     (1000) daern     (1000)        0 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/helpers/__init__.py
--rw-r--r--   0 daern     (1000) daern     (1000)     3492 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/helpers/request_tracker.py
--rw-r--r--   0 daern     (1000) daern     (1000)     2235 2023-01-12 20:57:33.000000 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/odometer_measurement.py
--rw-r--r--   0 daern     (1000) daern     (1000)     1500 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/parking_position.py
--rw-r--r--   0 daern     (1000) daern     (1000)    22369 2023-03-28 15:48:23.000000 weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/vehicle.py
-drwxr-xr-x   0 daern     (1000) daern     (1000)        0 2023-06-02 08:46:43.887645 weconnect-cupra-daern-0.49.20/weconnect/api/vw/
--rw-r--r--   0 daern     (1000) daern     (1000)        0 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/__init__.py
--rw-r--r--   0 daern     (1000) daern     (1000)     7626 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/api.py
-drwxr-xr-x   0 daern     (1000) daern     (1000)        0 2023-06-02 08:46:43.887645 weconnect-cupra-daern-0.49.20/weconnect/api/vw/auth/
--rw-r--r--   0 daern     (1000) daern     (1000)        0 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/auth/__init__.py
--rw-r--r--   0 daern     (1000) daern     (1000)    16437 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/auth/we_charge_session.py
--rw-r--r--   0 daern     (1000) daern     (1000)    17759 2023-01-12 20:58:10.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/auth/we_connect_session.py
-drwxr-xr-x   0 daern     (1000) daern     (1000)        0 2023-06-02 08:46:43.887645 weconnect-cupra-daern-0.49.20/weconnect/api/vw/badges/
--rw-r--r--   0 daern     (1000) daern     (1000)     5504 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/badges/charging.png
--rw-r--r--   0 daern     (1000) daern     (1000)     7170 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/badges/connected.png
--rw-r--r--   0 daern     (1000) daern     (1000)     9627 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/badges/cooling.png
--rw-r--r--   0 daern     (1000) daern     (1000)     7549 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/badges/heating.png
--rw-r--r--   0 daern     (1000) daern     (1000)     7022 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/badges/locked.png
--rw-r--r--   0 daern     (1000) daern     (1000)     5710 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/badges/parking.png
--rw-r--r--   0 daern     (1000) daern     (1000)     6941 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/badges/unlocked.png
--rw-r--r--   0 daern     (1000) daern     (1000)     8409 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/badges/ventilating.png
--rw-r--r--   0 daern     (1000) daern     (1000)     8199 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/badges/warning.png
--rw-r--r--   0 daern     (1000) daern     (1000)      659 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/domain.py
-drwxr-xr-x   0 daern     (1000) daern     (1000)        0 2023-06-02 08:46:43.887645 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/
--rw-r--r--   0 daern     (1000) daern     (1000)        0 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/__init__.py
--rw-r--r--   0 daern     (1000) daern     (1000)    10015 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/access_status.py
--rw-r--r--   0 daern     (1000) daern     (1000)     2443 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/battery_status.py
--rw-r--r--   0 daern     (1000) daern     (1000)     1970 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/capability_status.py
--rw-r--r--   0 daern     (1000) daern     (1000)     3692 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/charge_mode.py
--rw-r--r--   0 daern     (1000) daern     (1000)    11793 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/charging_profiles.py
--rw-r--r--   0 daern     (1000) daern     (1000)     4295 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/charging_settings.py
--rw-r--r--   0 daern     (1000) daern     (1000)    19151 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/charging_station.py
--rw-r--r--   0 daern     (1000) daern     (1000)     7701 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/charging_status.py
--rw-r--r--   0 daern     (1000) daern     (1000)     8079 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/climatization_settings.py
--rw-r--r--   0 daern     (1000) daern     (1000)     2868 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/climatization_status.py
--rw-r--r--   0 daern     (1000) daern     (1000)     2691 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/climatization_timer.py
--rw-r--r--   0 daern     (1000) daern     (1000)     9402 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/controls.py
--rw-r--r--   0 daern     (1000) daern     (1000)      562 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/enums.py
--rw-r--r--   0 daern     (1000) daern     (1000)     3391 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/generic_capability.py
--rw-r--r--   0 daern     (1000) daern     (1000)     2083 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/generic_request_status.py
--rw-r--r--   0 daern     (1000) daern     (1000)     3104 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/generic_settings.py
-drwxr-xr-x   0 daern     (1000) daern     (1000)        0 2023-06-02 08:46:43.887645 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/helpers/
--rw-r--r--   0 daern     (1000) daern     (1000)        0 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/helpers/__init__.py
--rw-r--r--   0 daern     (1000) daern     (1000)     3486 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/helpers/request_tracker.py
--rw-r--r--   0 daern     (1000) daern     (1000)     3331 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/lights_status.py
--rw-r--r--   0 daern     (1000) daern     (1000)     1639 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/lv_battery_status.py
--rw-r--r--   0 daern     (1000) daern     (1000)     3760 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/maintenance_status.py
--rw-r--r--   0 daern     (1000) daern     (1000)     2319 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/odometer_measurement.py
--rw-r--r--   0 daern     (1000) daern     (1000)     1661 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/parking_position.py
--rw-r--r--   0 daern     (1000) daern     (1000)     1610 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/range_measurements.py
--rw-r--r--   0 daern     (1000) daern     (1000)     5078 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/range_status.py
--rw-r--r--   0 daern     (1000) daern     (1000)     6696 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/readiness_status.py
--rw-r--r--   0 daern     (1000) daern     (1000)     7627 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/timer.py
--rw-r--r--   0 daern     (1000) daern     (1000)    46165 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/vehicle.py
--rw-r--r--   0 daern     (1000) daern     (1000)     7969 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/warning_lights_status.py
-drwxr-xr-x   0 daern     (1000) daern     (1000)        0 2023-06-02 08:46:43.887645 weconnect-cupra-daern-0.49.20/weconnect/auth/
--rw-r--r--   0 daern     (1000) daern     (1000)        0 2023-01-12 20:52:24.000000 weconnect-cupra-daern-0.49.20/weconnect/auth/__init__.py
--rw-r--r--   0 daern     (1000) daern     (1000)      142 2023-01-12 20:52:24.000000 weconnect-cupra-daern-0.49.20/weconnect/auth/auth_util.py
--rw-r--r--   0 daern     (1000) daern     (1000)     7234 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/auth/openid_session.py
--rw-r--r--   0 daern     (1000) daern     (1000)     3101 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/auth/session_manager.py
--rw-r--r--   0 daern     (1000) daern     (1000)      232 2023-01-12 20:52:24.000000 weconnect-cupra-daern-0.49.20/weconnect/auth/vw_web_session.py
-drwxr-xr-x   0 daern     (1000) daern     (1000)        0 2023-06-02 08:46:43.897645 weconnect-cupra-daern-0.49.20/weconnect/elements/
--rw-r--r--   0 daern     (1000) daern     (1000)        0 2023-01-12 20:52:24.000000 weconnect-cupra-daern-0.49.20/weconnect/elements/__init__.py
--rw-r--r--   0 daern     (1000) daern     (1000)      880 2023-03-10 15:22:13.000000 weconnect-cupra-daern-0.49.20/weconnect/elements/access_control_state.py
--rw-r--r--   0 daern     (1000) daern     (1000)      927 2023-01-12 20:52:24.000000 weconnect-cupra-daern-0.49.20/weconnect/elements/control_operation.py
--rw-r--r--   0 daern     (1000) daern     (1000)     3426 2023-01-12 20:52:24.000000 weconnect-cupra-daern-0.49.20/weconnect/elements/error.py
--rw-r--r--   0 daern     (1000) daern     (1000)     9952 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/elements/generic_status.py
--rw-r--r--   0 daern     (1000) daern     (1000)     3437 2023-01-12 20:58:26.000000 weconnect-cupra-daern-0.49.20/weconnect/elements/plug_status.py
--rw-r--r--   0 daern     (1000) daern     (1000)     3818 2023-01-12 20:58:33.000000 weconnect-cupra-daern-0.49.20/weconnect/elements/window_heating_status.py
--rw-r--r--   0 daern     (1000) daern     (1000)     2338 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/errors.py
--rw-r--r--   0 daern     (1000) daern     (1000)     7387 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/fetch.py
--rw-r--r--   0 daern     (1000) daern     (1000)      182 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/service.py
--rw-r--r--   0 daern     (1000) daern     (1000)     3695 2023-01-12 20:57:00.000000 weconnect-cupra-daern-0.49.20/weconnect/util.py
--rw-r--r--   0 daern     (1000) daern     (1000)     9001 2023-01-12 20:57:09.000000 weconnect-cupra-daern-0.49.20/weconnect/weconnect.py
--rw-r--r--   0 daern     (1000) daern     (1000)      184 2023-01-12 20:52:44.000000 weconnect-cupra-daern-0.49.20/weconnect/weconnect_errors.py
-drwxr-xr-x   0 daern     (1000) daern     (1000)        0 2023-06-02 08:46:43.897645 weconnect-cupra-daern-0.49.20/weconnect_cupra_daern.egg-info/
--rw-r--r--   0 daern     (1000) daern     (1000)     5580 2023-06-02 08:46:43.000000 weconnect-cupra-daern-0.49.20/weconnect_cupra_daern.egg-info/PKG-INFO
--rw-r--r--   0 daern     (1000) daern     (1000)     3995 2023-06-02 08:46:43.000000 weconnect-cupra-daern-0.49.20/weconnect_cupra_daern.egg-info/SOURCES.txt
--rw-r--r--   0 daern     (1000) daern     (1000)        1 2023-06-02 08:46:43.000000 weconnect-cupra-daern-0.49.20/weconnect_cupra_daern.egg-info/dependency_links.txt
--rw-r--r--   0 daern     (1000) daern     (1000)        1 2023-03-23 10:05:32.000000 weconnect-cupra-daern-0.49.20/weconnect_cupra_daern.egg-info/not-zip-safe
--rw-r--r--   0 daern     (1000) daern     (1000)       76 2023-06-02 08:46:43.000000 weconnect-cupra-daern-0.49.20/weconnect_cupra_daern.egg-info/requires.txt
--rw-r--r--   0 daern     (1000) daern     (1000)       16 2023-06-02 08:46:43.000000 weconnect-cupra-daern-0.49.20/weconnect_cupra_daern.egg-info/top_level.txt
+drwxrwxr-x   0 daern     (1000) daern     (1000)        0 2023-06-07 21:37:55.721311 weconnect-cupra-daern-0.50.1/
+-rw-rw-r--   0 daern     (1000) daern     (1000)     1071 2023-06-07 12:56:04.000000 weconnect-cupra-daern-0.50.1/LICENSE
+-rw-rw-r--   0 daern     (1000) daern     (1000)       51 2023-06-07 12:57:58.000000 weconnect-cupra-daern-0.50.1/MANIFEST.in
+-rw-rw-r--   0 daern     (1000) daern     (1000)     4786 2023-06-07 21:37:55.721311 weconnect-cupra-daern-0.50.1/PKG-INFO
+-rw-rw-r--   0 daern     (1000) daern     (1000)     3613 2023-06-07 21:18:32.000000 weconnect-cupra-daern-0.50.1/README.md
+-rw-rw-r--   0 daern     (1000) daern     (1000)     3004 2023-06-07 21:37:55.721311 weconnect-cupra-daern-0.50.1/setup.cfg
+-rw-rw-r--   0 daern     (1000) daern     (1000)     2053 2023-06-07 19:53:45.000000 weconnect-cupra-daern-0.50.1/setup.py
+drwxrwxr-x   0 daern     (1000) daern     (1000)        0 2023-06-07 21:37:55.709311 weconnect-cupra-daern-0.50.1/tests/
+-rw-rw-r--   0 daern     (1000) daern     (1000)        0 2023-06-07 12:56:04.000000 weconnect-cupra-daern-0.50.1/tests/__init__.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     8774 2023-06-07 12:56:04.000000 weconnect-cupra-daern-0.50.1/tests/test_addressable.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)    13494 2023-06-07 12:57:58.000000 weconnect-cupra-daern-0.50.1/tests/test_cupra.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     1002 2023-06-07 12:56:04.000000 weconnect-cupra-daern-0.50.1/tests/test_elements.py
+drwxrwxr-x   0 daern     (1000) daern     (1000)        0 2023-06-07 21:37:55.709311 weconnect-cupra-daern-0.50.1/weconnect_cupra/
+-rw-rw-r--   0 daern     (1000) daern     (1000)        0 2023-06-07 12:56:04.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/__init__.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)       24 2023-06-07 20:29:13.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/__version.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)    25444 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/addressable.py
+drwxrwxr-x   0 daern     (1000) daern     (1000)        0 2023-06-07 21:37:55.709311 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/
+-rw-rw-r--   0 daern     (1000) daern     (1000)        0 2023-06-07 12:57:58.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/__init__.py
+drwxrwxr-x   0 daern     (1000) daern     (1000)        0 2023-06-07 21:37:55.709311 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/cupra/
+-rw-rw-r--   0 daern     (1000) daern     (1000)        0 2023-06-07 12:57:58.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/cupra/__init__.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     3951 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/cupra/api.py
+drwxrwxr-x   0 daern     (1000) daern     (1000)        0 2023-06-07 21:37:55.713311 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/cupra/auth/
+-rw-rw-r--   0 daern     (1000) daern     (1000)        0 2023-06-07 12:57:58.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/cupra/auth/__init__.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)    17254 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/cupra/auth/my_cupra_session.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)      362 2023-06-07 12:57:58.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/cupra/domain.py
+drwxrwxr-x   0 daern     (1000) daern     (1000)        0 2023-06-07 21:37:55.713311 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/cupra/elements/
+-rw-rw-r--   0 daern     (1000) daern     (1000)        0 2023-06-07 12:57:58.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/cupra/elements/__init__.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)    12732 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/cupra/elements/access_status.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     2688 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/cupra/elements/battery_status.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     4507 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/cupra/elements/charging_settings.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)    14455 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/cupra/elements/charging_station.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     7754 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/cupra/elements/charging_status.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     8582 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/cupra/elements/climatization_settings.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     2786 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/cupra/elements/climatization_status.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)    12348 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/cupra/elements/controls.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     2246 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/cupra/elements/engine_state.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)      802 2023-06-07 19:36:31.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/cupra/elements/enums.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     3442 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/cupra/elements/error.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     3399 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/cupra/elements/generic_capability.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     5296 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/cupra/elements/generic_settings.py
+drwxrwxr-x   0 daern     (1000) daern     (1000)        0 2023-06-07 21:37:55.713311 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/cupra/elements/helpers/
+-rw-rw-r--   0 daern     (1000) daern     (1000)        0 2023-06-07 12:57:58.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/cupra/elements/helpers/__init__.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     3516 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/cupra/elements/helpers/request_tracker.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     2253 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/cupra/elements/odometer_measurement.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     1518 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/cupra/elements/parking_position.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)    22489 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/cupra/elements/vehicle.py
+drwxrwxr-x   0 daern     (1000) daern     (1000)        0 2023-06-07 21:37:55.713311 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/
+-rw-rw-r--   0 daern     (1000) daern     (1000)        0 2023-06-07 12:57:58.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/__init__.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     7704 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/api.py
+drwxrwxr-x   0 daern     (1000) daern     (1000)        0 2023-06-07 21:37:55.713311 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/auth/
+-rw-rw-r--   0 daern     (1000) daern     (1000)        0 2023-06-07 12:57:58.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/auth/__init__.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)    16467 2023-06-07 19:53:10.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/auth/we_charge_session.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)    17807 2023-06-07 19:53:10.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/auth/we_connect_session.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)      659 2023-06-07 12:57:58.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/domain.py
+drwxrwxr-x   0 daern     (1000) daern     (1000)        0 2023-06-07 21:37:55.717311 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/
+-rw-rw-r--   0 daern     (1000) daern     (1000)        0 2023-06-07 12:57:58.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/__init__.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)    10033 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/access_status.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     2461 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/battery_status.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     1994 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/capability_status.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     3710 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/charge_mode.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)    11823 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/charging_profiles.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     4319 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/charging_settings.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)    19163 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/charging_station.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     7719 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/charging_status.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     8103 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/climatization_settings.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     2886 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/climatization_status.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     2715 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/climatization_timer.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     9456 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/controls.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)      568 2023-06-07 19:36:31.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/enums.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     3403 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/generic_capability.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     2101 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/generic_request_status.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     3140 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/generic_settings.py
+drwxrwxr-x   0 daern     (1000) daern     (1000)        0 2023-06-07 21:37:55.717311 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/helpers/
+-rw-rw-r--   0 daern     (1000) daern     (1000)        0 2023-06-07 12:57:58.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/helpers/__init__.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     3510 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/helpers/request_tracker.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     3349 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/lights_status.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     1657 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/lv_battery_status.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     3778 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/maintenance_status.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     2337 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/odometer_measurement.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     1679 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/parking_position.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     1628 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/range_measurements.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     5096 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/range_status.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     6720 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/readiness_status.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     7645 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/timer.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)    46375 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/vehicle.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     7987 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/warning_lights_status.py
+drwxrwxr-x   0 daern     (1000) daern     (1000)        0 2023-06-07 21:37:55.717311 weconnect-cupra-daern-0.50.1/weconnect_cupra/auth/
+-rw-rw-r--   0 daern     (1000) daern     (1000)        0 2023-06-07 12:56:04.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/auth/__init__.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)      142 2023-06-07 12:56:04.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/auth/auth_util.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     7252 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/auth/openid_session.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     3137 2023-06-07 19:46:42.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/auth/session_manager.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)      238 2023-06-07 19:36:31.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/auth/vw_web_session.py
+drwxrwxr-x   0 daern     (1000) daern     (1000)        0 2023-06-07 21:37:55.721311 weconnect-cupra-daern-0.50.1/weconnect_cupra/elements/
+-rw-rw-r--   0 daern     (1000) daern     (1000)        0 2023-06-07 12:56:04.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/elements/__init__.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)      880 2023-06-07 12:57:58.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/elements/access_control_state.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)      927 2023-06-07 12:56:04.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/elements/control_operation.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     3444 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/elements/error.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     9988 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/elements/generic_status.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     3455 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/elements/plug_status.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     3836 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/elements/window_heating_status.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     2356 2023-06-07 19:40:00.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/errors.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     7417 2023-06-07 19:37:35.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/fetch.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)      182 2023-06-07 19:45:56.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/service.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     3695 2023-06-07 12:57:58.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/util.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)     9137 2023-06-07 20:09:50.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/weconnect_cupra.py
+-rw-rw-r--   0 daern     (1000) daern     (1000)      184 2023-06-07 12:57:58.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra/weconnect_errors.py
+drwxrwxr-x   0 daern     (1000) daern     (1000)        0 2023-06-07 21:37:55.721311 weconnect-cupra-daern-0.50.1/weconnect_cupra_daern.egg-info/
+-rw-rw-r--   0 daern     (1000) daern     (1000)     4786 2023-06-07 21:37:55.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra_daern.egg-info/PKG-INFO
+-rw-rw-r--   0 daern     (1000) daern     (1000)     4170 2023-06-07 21:37:55.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra_daern.egg-info/SOURCES.txt
+-rw-rw-r--   0 daern     (1000) daern     (1000)        1 2023-06-07 21:37:55.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra_daern.egg-info/dependency_links.txt
+-rw-rw-r--   0 daern     (1000) daern     (1000)        1 2023-06-07 20:04:08.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra_daern.egg-info/not-zip-safe
+-rw-rw-r--   0 daern     (1000) daern     (1000)       76 2023-06-07 21:37:55.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra_daern.egg-info/requires.txt
+-rw-rw-r--   0 daern     (1000) daern     (1000)       22 2023-06-07 21:37:55.000000 weconnect-cupra-daern-0.50.1/weconnect_cupra_daern.egg-info/top_level.txt
```

### Comparing `weconnect-cupra-daern-0.49.20/PKG-INFO` & `weconnect-cupra-daern-0.50.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,84 +1,82 @@
 Metadata-Version: 2.1
 Name: weconnect-cupra-daern
-Version: 0.49.20
-Summary: Fork of Python API for the Volkswagen WeConnect Services to support Cupra Born
-Home-page: https://github.com/daernsinstantfortress/WeConnect-python
+Version: 0.50.1
+Summary: Python API for the Cupra Born online services
+Home-page: https://github.com/daernsinstantfortress/WeConnect-Cupra-python
 Author: Till Steinbach / Alan Gibson / Stuart Hall
 License: MIT
 Project-URL: Funding, https://github.com/sponsors/tillsteinbach
-Project-URL: Source, https://github.com/daernsinstantfortress/WeConnect-python
-Project-URL: Bug Tracker, https://github.com/tillsteinbach/WeConnect-python/issues
-Description: 
-        
-        # WeConnect-python
-        [![GitHub sourcecode](https://img.shields.io/badge/Source-GitHub-green)](https://github.com/tillsteinbach/WeConnect-python/)
-        [![GitHub release (latest by date)](https://img.shields.io/github/v/release/tillsteinbach/WeConnect-python)](https://github.com/tillsteinbach/WeConnect-python/releases/latest)
-        [![GitHub](https://img.shields.io/github/license/tillsteinbach/WeConnect-python)](https://github.com/tillsteinbach/WeConnect-python/blob/master/LICENSE)
-        [![GitHub issues](https://img.shields.io/github/issues/tillsteinbach/WeConnect-python)](https://github.com/tillsteinbach/WeConnect-python/issues)
-        [![PyPI - Downloads](https://img.shields.io/pypi/dm/weconnect?label=PyPI%20Downloads)](https://pypi.org/project/weconnect/)
-        [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/weconnect)](https://pypi.org/project/weconnect/)
-        [![Donate at PayPal](https://img.shields.io/badge/Donate-PayPal-2997d8)](https://www.paypal.com/donate?hosted_button_id=2BVFF5GJ9SXAJ)
-        [![Sponsor at Github](https://img.shields.io/badge/Sponsor-GitHub-28a745)](https://github.com/sponsors/tillsteinbach)
-        
-        Python API for the Volkswagen WeConnect and Cupra MyCupra Services. If you are not a developer and ended up here you probably want to check out a project using this library (see below).
-        
-        ## Projects in which the library is used
-        - [VWsFriend](https://github.com/tillsteinbach/VWsFriend): VWsFriend records statistics about your car (charging sessions, battery, trips, fueling, etc.) and displays them nicely. It also allows you to forward data from the car to other applications such as [A better routeplanner](https://abetterrouteplanner.com/) and allows you to integrate your car into [Apple HomeKit](https://www.apple.com/ios/home/)
-        - [WeConnect-cli](https://github.com/tillsteinbach/WeConnect-cli): A commandline interface to interact with WeConnect
-        - [WeConnect-MQTT](https://github.com/tillsteinbach/WeConnect-mqtt): A MQTT Client that provides WeConnect data to the MQTT Broker of your choice (e.g. your home automation solution such as [ioBroker](https://www.iobroker.net), [FHEM](https://fhem.de) or [Home Assistant](https://www.home-assistant.io))
-        
-        ## Install
-        ```
-        pip3 install weconnect[Images]
-        ```
-        
-        ## Package
-        ```
-        python3 -m pip install --upgrade build
-        python3 -m build --sdist
-        python3 -m build --wheel
-        ```
-        
-        ## Distribute
-        ```
-        python3 -m pip install --upgrade twine
-        python3 -m twine upload --repository pypi dist/*
-        ```
-        
-        ## Getting started
-        - To get started have a look in the [examples folder](https://github.com/tillsteinbach/WeConnect-python/tree/main/examples)
-        
-        ## Tested with
-        - Volkswagen ID.3 Modelyear 2021
-        - Volkswagen Passat GTE Modelyear 2021
-        - Cupra Born Modelyear 2022
-        
-        ## Login & Consent
-        WeConnect-python is based on the new WeConnect ID API that was introduced with the new series of ID cars. If you use another car or hybrid you probably need to agree to the terms and conditions of the WeConnect ID interface. Easiest to do so is by installing the WeConnect ID app on your smartphone and login there. If necessary you will be asked to agree to the terms and conditions.
-        
-        ## Reporting Issues
-        Please feel free to open an issue at [GitHub Issue page](https://github.com/tillsteinbach/WeConnect-python/issues) to report problems you found.
-        
-        ### Known Issues
-        - The API is in alpha state and may change unexpectedly at any time! Please conscider this and pin to a specific version if you depend on it.
-        - Examples and API documentation is missing
-        
-        ## Credits
-        Inspired by [TA2k/ioBroker.vw-connect](https://github.com/TA2k/ioBroker.vw-connect/) that gave me a point to start working with the API
-        
-        ## Seat, Cupra, Skoda IV, ...
-        In an effort to try to make WeConnect-python also to work with latest generation of vehicles from other volkswagen brands I'm looking for users to temporarily share access to their accounts. If you are willing to support please send me a message.
-        - Already tried: Cupra Born (The API looks a bit different, maybe it is older, I will check again in some weeks), thanks to the user initdebugs
-        
-Keywords: weconnect,we connect,carnet,car net,volkswagen,vw,telemetry
+Project-URL: Source, https://github.com/daernsinstantfortress/WeConnect-Cupra-python
+Project-URL: Bug Tracker, https://github.com/daernsinstantfortress/WeConnect-Cupra-python/issues
+Keywords: weconnect_cupra,weconnect,we connect,carnet,car net,volkswagen,vw,telemetry,cupra
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: Images
+License-File: LICENSE
+
+
+
+# WeConnect-Cupra-python
+[![GitHub sourcecode](https://img.shields.io/badge/Source-GitHub-green)](https://github.com/daernsinstantfortress/WeConnect-Cupra-python)
+[![GitHub release (latest by date)](https://img.shields.io/github/v/release/daernsinstantfortress/WeConnect-Cupra-python)](https://github.com/daernsinstantfortress/WeConnect-Cupra-python/releases/latest)
+[![GitHub](https://img.shields.io/github/license/daernsinstantfortress/WeConnect-Cupra-python)](https://github.com/daernsinstantfortress/WeConnect-Cupra-python/blob/master/LICENSE)
+[![GitHub issues](https://img.shields.io/github/issues/daernsinstantfortress/WeConnect-Cupra-python)](https://github.com/daernsinstantfortress/WeConnect-Cupra-python/issues)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/weconnect-cupra-daern?label=PyPI%20Downloads)](https://pypi.org/project/weconnect-cupra-daern/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/weconnect-cupra-daern)](https://pypi.org/project/weconnect-cupra-daern/)
+
+Python API for the MyCupra Services. If you are not a developer and ended up here you probably want to check out a project using this library (see below).
+
+## Projects in which the library is used
+- [VWsFriend](https://github.com/tillsteinbach/VWsFriend): VWsFriend records statistics about your car (charging sessions, battery, trips, fueling, etc.) and displays them nicely. It also allows you to forward data from the car to other applications such as [A better routeplanner](https://abetterrouteplanner.com/) and allows you to integrate your car into [Apple HomeKit](https://www.apple.com/ios/home/)
+- [WeConnect-cli](https://github.com/tillsteinbach/WeConnect-cli): A commandline interface to interact with WeConnect
+- [WeConnect-MQTT](https://github.com/tillsteinbach/WeConnect-mqtt): A MQTT Client that provides WeConnect data to the MQTT Broker of your choice (e.g. your home automation solution such as [ioBroker](https://www.iobroker.net), [FHEM](https://fhem.de) or [Home Assistant](https://www.home-assistant.io))
+
+## Install
+```
+pip3 install weconnect-cupra-daern[Images]
+```
+
+## Package
+```
+python3 -m pip install --upgrade build
+python3 -m build --sdist
+python3 -m build --wheel
+```
+
+## Distribute
+```
+python3 -m pip install --upgrade twine
+python3 -m twine upload --repository pypi dist/*
+```
+
+## Getting started
+- To get started have a look in the [examples folder](https://github.com/daernsinstantfortress/WeConnect-Cupra-python/tree/main/examples)
+
+## Tested with
+- Cupra Born Model year 2022/23
+
+## Login & Consent
+WeConnect-python is based on the new WeConnect ID API that was introduced with the new series of ID cars. If you use another car or hybrid you probably need to agree to the terms and conditions of the WeConnect ID interface. Easiest to do so is by installing the WeConnect ID app on your smartphone and login there. If necessary you will be asked to agree to the terms and conditions.
+
+## Reporting Issues
+Please feel free to open an issue at [GitHub Issue page](https://github.com/daernsinstantfortress/WeConnect-Cupra-python/issues) to report problems you found.
+
+### Known Issues
+- The API is in alpha state and may change unexpectedly at any time! Please conscider this and pin to a specific version if you depend on it.
+- Examples and API documentation is missing
+
+## Credits
+Largely based on WeConnect-python for VW from https://github.com/tillsteinbach/WeConnect-python, with the initial Cupra port developed by Alan Gibson
+Inspired by [TA2k/ioBroker.vw-connect](https://github.com/TA2k/ioBroker.vw-connect/) that gave me a point to start working with the API
+
+
```

### Comparing `weconnect-cupra-daern-0.49.20/README.md` & `weconnect-cupra-daern-0.50.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 
 
-# WeConnect-python
-[![GitHub sourcecode](https://img.shields.io/badge/Source-GitHub-green)](https://github.com/tillsteinbach/WeConnect-python/)
-[![GitHub release (latest by date)](https://img.shields.io/github/v/release/tillsteinbach/WeConnect-python)](https://github.com/tillsteinbach/WeConnect-python/releases/latest)
-[![GitHub](https://img.shields.io/github/license/tillsteinbach/WeConnect-python)](https://github.com/tillsteinbach/WeConnect-python/blob/master/LICENSE)
-[![GitHub issues](https://img.shields.io/github/issues/tillsteinbach/WeConnect-python)](https://github.com/tillsteinbach/WeConnect-python/issues)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/weconnect?label=PyPI%20Downloads)](https://pypi.org/project/weconnect/)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/weconnect)](https://pypi.org/project/weconnect/)
-[![Donate at PayPal](https://img.shields.io/badge/Donate-PayPal-2997d8)](https://www.paypal.com/donate?hosted_button_id=2BVFF5GJ9SXAJ)
-[![Sponsor at Github](https://img.shields.io/badge/Sponsor-GitHub-28a745)](https://github.com/sponsors/tillsteinbach)
+# WeConnect-Cupra-python
+[![GitHub sourcecode](https://img.shields.io/badge/Source-GitHub-green)](https://github.com/daernsinstantfortress/WeConnect-Cupra-python)
+[![GitHub release (latest by date)](https://img.shields.io/github/v/release/daernsinstantfortress/WeConnect-Cupra-python)](https://github.com/daernsinstantfortress/WeConnect-Cupra-python/releases/latest)
+[![GitHub](https://img.shields.io/github/license/daernsinstantfortress/WeConnect-Cupra-python)](https://github.com/daernsinstantfortress/WeConnect-Cupra-python/blob/master/LICENSE)
+[![GitHub issues](https://img.shields.io/github/issues/daernsinstantfortress/WeConnect-Cupra-python)](https://github.com/daernsinstantfortress/WeConnect-Cupra-python/issues)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/weconnect-cupra-daern?label=PyPI%20Downloads)](https://pypi.org/project/weconnect-cupra-daern/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/weconnect-cupra-daern)](https://pypi.org/project/weconnect-cupra-daern/)
 
-Python API for the Volkswagen WeConnect and Cupra MyCupra Services. If you are not a developer and ended up here you probably want to check out a project using this library (see below).
+Python API for the MyCupra Services. If you are not a developer and ended up here you probably want to check out a project using this library (see below).
 
 ## Projects in which the library is used
 - [VWsFriend](https://github.com/tillsteinbach/VWsFriend): VWsFriend records statistics about your car (charging sessions, battery, trips, fueling, etc.) and displays them nicely. It also allows you to forward data from the car to other applications such as [A better routeplanner](https://abetterrouteplanner.com/) and allows you to integrate your car into [Apple HomeKit](https://www.apple.com/ios/home/)
 - [WeConnect-cli](https://github.com/tillsteinbach/WeConnect-cli): A commandline interface to interact with WeConnect
 - [WeConnect-MQTT](https://github.com/tillsteinbach/WeConnect-mqtt): A MQTT Client that provides WeConnect data to the MQTT Broker of your choice (e.g. your home automation solution such as [ioBroker](https://www.iobroker.net), [FHEM](https://fhem.de) or [Home Assistant](https://www.home-assistant.io))
 
 ## Install
 ```
-pip3 install weconnect[Images]
+pip3 install weconnect-cupra-daern[Images]
 ```
 
 ## Package
 ```
 python3 -m pip install --upgrade build
 python3 -m build --sdist
 python3 -m build --wheel
@@ -32,30 +30,25 @@
 ## Distribute
 ```
 python3 -m pip install --upgrade twine
 python3 -m twine upload --repository pypi dist/*
 ```
 
 ## Getting started
-- To get started have a look in the [examples folder](https://github.com/tillsteinbach/WeConnect-python/tree/main/examples)
+- To get started have a look in the [examples folder](https://github.com/daernsinstantfortress/WeConnect-Cupra-python/tree/main/examples)
 
 ## Tested with
-- Volkswagen ID.3 Modelyear 2021
-- Volkswagen Passat GTE Modelyear 2021
-- Cupra Born Modelyear 2022
+- Cupra Born Model year 2022/23
 
 ## Login & Consent
 WeConnect-python is based on the new WeConnect ID API that was introduced with the new series of ID cars. If you use another car or hybrid you probably need to agree to the terms and conditions of the WeConnect ID interface. Easiest to do so is by installing the WeConnect ID app on your smartphone and login there. If necessary you will be asked to agree to the terms and conditions.
 
 ## Reporting Issues
-Please feel free to open an issue at [GitHub Issue page](https://github.com/tillsteinbach/WeConnect-python/issues) to report problems you found.
+Please feel free to open an issue at [GitHub Issue page](https://github.com/daernsinstantfortress/WeConnect-Cupra-python/issues) to report problems you found.
 
 ### Known Issues
 - The API is in alpha state and may change unexpectedly at any time! Please conscider this and pin to a specific version if you depend on it.
 - Examples and API documentation is missing
 
 ## Credits
+Largely based on WeConnect-python for VW from https://github.com/tillsteinbach/WeConnect-python, with the initial Cupra port developed by Alan Gibson
 Inspired by [TA2k/ioBroker.vw-connect](https://github.com/TA2k/ioBroker.vw-connect/) that gave me a point to start working with the API
-
-## Seat, Cupra, Skoda IV, ...
-In an effort to try to make WeConnect-python also to work with latest generation of vehicles from other volkswagen brands I'm looking for users to temporarily share access to their accounts. If you are willing to support please send me a message.
-- Already tried: Cupra Born (The API looks a bit different, maybe it is older, I will check again in some weeks), thanks to the user initdebugs
```

### Comparing `weconnect-cupra-daern-0.49.20/setup.cfg` & `weconnect-cupra-daern-0.50.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 	docs
 ignore = 
 	W503
 max-line-length = 160
 max-complexity = 10
 
 [bandit]
-targets = weconnect
+targets = weconnect_cupra
 skips = B311
 
 [pylint]
 persistent = yes
 load-plugins = pylint.extensions.no_self_use
 jobs = 1
 unsafe-load-any-extension = no
```

### Comparing `weconnect-cupra-daern-0.49.20/setup.py` & `weconnect-cupra-daern-0.50.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,40 +9,42 @@
 IMAGE_EXTRA_REQUIRED = (HERE / "image_extra_requirements.txt").read_text()
 SETUP_REQUIRED = (HERE / "setup_requirements.txt").read_text()
 TEST_REQUIRED = (HERE / "test_requirements.txt").read_text()
 
 setup(
     name='weconnect-cupra-daern',
     packages=find_packages(),
-    version=open("weconnect/__version.py").readlines()[-1].split()[-1].strip("\"'"),
-    description='Fork of Python API for the Volkswagen WeConnect Services to support Cupra Born',
+    version=open("weconnect_cupra/__version.py").readlines()[-1].split()[-1].strip("\"'"),
+    description='Python API for the Cupra Born online services',
     long_description=README,
     long_description_content_type="text/markdown",
     author='Till Steinbach / Alan Gibson / Stuart Hall',
-    keywords='weconnect, we connect, carnet, car net, volkswagen, vw, telemetry',
-    url='https://github.com/daernsinstantfortress/WeConnect-python',
+    keywords='weconnect_cupra, weconnect, we connect, carnet, car net, volkswagen, vw, telemetry, cupra',
+    url='https://github.com/daernsinstantfortress/WeConnect-Cupra-python',
     project_urls={
         'Funding': 'https://github.com/sponsors/tillsteinbach',
-        'Source': 'https://github.com/daernsinstantfortress/WeConnect-python',
-        'Bug Tracker': 'https://github.com/tillsteinbach/WeConnect-python/issues'
+        'Source': 'https://github.com/daernsinstantfortress/WeConnect-Cupra-python',
+        'Bug Tracker': 'https://github.com/daernsinstantfortress/WeConnect-Cupra-python/issues'
     },
     license='MIT',
     install_requires=INSTALL_REQUIRED,
     extras_require={
         "Images": IMAGE_EXTRA_REQUIRED,
     },
     classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
         'Intended Audience :: Developers',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Software Development :: Libraries',
     ],
     python_requires='>=3.7',
     setup_requires=SETUP_REQUIRED,
     tests_require=TEST_REQUIRED,
     include_package_data=True,
     zip_safe=False,
-    package_data={'': ['weconnect/api/vw/badges/*.png']}
+    package_data={'': ['weconnect_cupra/api/vw/badges/*.png']}
 )
```

### Comparing `weconnect-cupra-daern-0.49.20/tests/test_addressable.py` & `weconnect-cupra-daern-0.50.1/tests/test_addressable.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.20/tests/test_cupra.py` & `weconnect-cupra-daern-0.50.1/tests/test_cupra.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.20/tests/test_elements.py` & `weconnect-cupra-daern-0.50.1/tests/test_elements.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/addressable.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/addressable.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import json
 import logging
 import time as timemodule
 from datetime import datetime, timezone, time
 from enum import Enum, IntEnum, Flag, auto
 
-from weconnect.util import toBool, imgToASCIIArt, robustTimeParse, ExtendedWithNullEncoder
+from weconnect_cupra.util import toBool, imgToASCIIArt, robustTimeParse, ExtendedWithNullEncoder
 
 SUPPORT_IMAGES = False
 try:
     from PIL import Image  # type: ignore
     SUPPORT_IMAGES = True
 except ImportError:
     pass
@@ -19,15 +19,15 @@
 SUPPORT_ASCII_IMAGES = False
 try:
     import ascii_magic  # type: ignore
     SUPPORT_ASCII_IMAGES = True
 except ImportError:
     pass
 
-LOG: logging.Logger = logging.getLogger("weconnect")
+LOG: logging.Logger = logging.getLogger("weconnect_cupra")
 
 
 class AddressableLeaf():
     def __init__(
         self,
         localAddress: str,
         parent: Optional[AddressableObject],
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/cupra/api.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/cupra/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from __future__ import annotations
 from typing import Dict, List, Set, Tuple, Callable, Any, Optional
 import logging
 from datetime import datetime
 
-from weconnect.addressable import AddressableObject, AddressableDict
-from weconnect.fetch import Fetcher
-from weconnect.addressable import AddressableDict
-from weconnect.errors import RetrievalError
-from weconnect.api.cupra.domain import Domain
-from weconnect.api.cupra.elements.vehicle import Vehicle
-from weconnect.api.cupra.elements.charging_station import ChargingStation
+from weconnect_cupra.addressable import AddressableObject, AddressableDict
+from weconnect_cupra.fetch import Fetcher
+from weconnect_cupra.addressable import AddressableDict
+from weconnect_cupra.errors import RetrievalError
+from weconnect_cupra.api.cupra.domain import Domain
+from weconnect_cupra.api.cupra.elements.vehicle import Vehicle
+from weconnect_cupra.api.cupra.elements.charging_station import ChargingStation
 
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class CupraApi:
-    def __init__(self, weconnect: AddressableObject, fetcher: Fetcher, enableTracker: bool = False, fixAPI: bool = True):
+    def __init__(self, weconnect_cupra: AddressableObject, fetcher: Fetcher, enableTracker: bool = False, fixAPI: bool = True):
         # https://github.com/evcc-io/evcc/blob/7abee00aa98a29d46d9d3c2a7a16a601558129b7/vehicle/seat/cupra/api.go
         self.base_url = 'https://ola.prod.code.seat.cloud.vwgroup.com'
-        self.__vehicles: AddressableDict[str, Vehicle] = AddressableDict(localAddress='vehicles', parent=weconnect)
-        self.__stations: AddressableDict[str, ChargingStation] = AddressableDict(localAddress='chargingStations', parent=weconnect)
+        self.__vehicles: AddressableDict[str, Vehicle] = AddressableDict(localAddress='vehicles', parent=weconnect_cupra)
+        self.__stations: AddressableDict[str, ChargingStation] = AddressableDict(localAddress='chargingStations', parent=weconnect_cupra)
         self.__fetcher: Fetcher = fetcher
         self.__enableTracker: bool = enableTracker
         self.fixAPI: bool = fixAPI
 
     @property
     def vehicles(self) -> AddressableDict[str, Vehicle]:
         return self.__vehicles
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/cupra/auth/my_cupra_session.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/cupra/auth/my_cupra_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 from requests.adapters import HTTPAdapter
 
 from oauthlib.common import to_unicode
 from oauthlib.oauth2 import InsecureTransportError
 from oauthlib.oauth2 import is_secure_transport
 
 from requests.models import CaseInsensitiveDict
-from weconnect.auth.openid_session import AccessType
+from weconnect_cupra.auth.openid_session import AccessType
 
-from weconnect.auth.vw_web_session import VWWebSession
-from weconnect.errors import APICompatibilityError, AuthentificationError, RetrievalError, TemporaryAuthentificationError
+from weconnect_cupra.auth.vw_web_session import VWWebSession
+from weconnect_cupra.errors import APICompatibilityError, AuthentificationError, RetrievalError, TemporaryAuthentificationError
 
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class MyCupraSession(VWWebSession):
     def __init__(self, sessionuser, **kwargs):
         super(MyCupraSession, self).__init__(client_id='3c756d46-f1ba-4d78-9f9a-cff0d5292d51@apps_vw-dilab_com',
                                              refresh_url='https://identity.vwgroup.io/oidc/v1/token',
                                              scope='openid profile nickname birthdate phone',
@@ -187,15 +187,15 @@
         # Check for user id
         if 'userId' not in params or not params['userId']:
             if 'updated' in params and params['updated'] == 'dataprivacy':
                 raise AuthentificationError('You have to login at myvolkswagen.de and accept the terms and conditions')
             raise APICompatibilityError('No user id provided')
         self.__userId = params['userId']  # pylint: disable=unused-private-member
 
-        # Now follow the forwarding until forwarding URL starts with 'weconnect://authenticated#'
+        # Now follow the forwarding until forwarding URL starts with 'weconnect_cupra://authenticated#'
         afterLoginUrl: str = login3Response.headers['Location']
 
         consentURL = None
         while True:
             if 'consent' in afterLoginUrl:
                 consentURL = afterLoginUrl
             afterLoginResponse = self.get(afterLoginUrl, allow_redirects=False, access_type=AccessType.NONE)
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/access_status.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/cupra/elements/access_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from enum import Enum
 import logging
 
-from weconnect.addressable import AddressableObject, AddressableAttribute, AddressableDict
-from weconnect.elements.generic_status import GenericStatus
-from weconnect.elements.access_control_state import AccessControlState
+from weconnect_cupra.addressable import AddressableObject, AddressableAttribute, AddressableDict
+from weconnect_cupra.elements.generic_status import GenericStatus
+from weconnect_cupra.elements.access_control_state import AccessControlState
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class AccessStatus(GenericStatus):
     def __init__(
         self,
         vehicle,
         parent,
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/battery_status.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/cupra/elements/battery_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 
-from weconnect.addressable import AddressableAttribute
-from weconnect.elements.generic_status import GenericStatus
+from weconnect_cupra.addressable import AddressableAttribute
+from weconnect_cupra.elements.generic_status import GenericStatus
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class BatteryStatus(GenericStatus):
     def __init__(
         self,
         vehicle,
         parent,
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/charging_settings.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/cupra/elements/charging_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 
-from weconnect.addressable import AddressableLeaf, ChangeableAttribute
-from weconnect.api.cupra.elements.generic_settings import GenericSettings
-from weconnect.api.cupra.elements.enums import UnlockPlugState, MaximumChargeCurrent
+from weconnect_cupra.addressable import AddressableLeaf, ChangeableAttribute
+from weconnect_cupra.api.cupra.elements.generic_settings import GenericSettings
+from weconnect_cupra.api.cupra.elements.enums import UnlockPlugState, MaximumChargeCurrent
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class ChargingSettings(GenericSettings):
     def __init__(
         self,
         vehicle,
         parent,
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/charging_station.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/cupra/elements/charging_station.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from enum import Enum
 
-from weconnect.addressable import AddressableObject, AddressableAttribute, AddressableList
+from weconnect_cupra.addressable import AddressableObject, AddressableAttribute, AddressableList
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class ChargingStation(AddressableObject):  # pylint: disable=too-many-instance-attributes
 
     def __init__(
         self,
         weConnect,
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/charging_status.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/cupra/elements/charging_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from enum import Enum
 import logging
 
-from weconnect.addressable import AddressableAttribute
-from weconnect.elements.generic_status import GenericStatus
+from weconnect_cupra.addressable import AddressableAttribute
+from weconnect_cupra.elements.generic_status import GenericStatus
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class ChargingStatus(GenericStatus):
     def __init__(
         self,
         vehicle,
         parent,
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/climatization_settings.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/cupra/elements/climatization_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from enum import Enum
 import logging
 
-from weconnect.addressable import AddressableLeaf, ChangeableAttribute, AddressableAttribute, AliasChangeableAttribute
-from weconnect.api.cupra.elements.generic_settings import GenericSettings
-from weconnect.util import celsiusToKelvin, farenheitToKelvin, kelvinToCelsius, kelvinToFarenheit
+from weconnect_cupra.addressable import AddressableLeaf, ChangeableAttribute, AddressableAttribute, AliasChangeableAttribute
+from weconnect_cupra.api.cupra.elements.generic_settings import GenericSettings
+from weconnect_cupra.util import celsiusToKelvin, farenheitToKelvin, kelvinToCelsius, kelvinToFarenheit
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class ClimatizationSettings(GenericSettings):
     def __init__(
         self,
         vehicle,
         parent,
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/climatization_status.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/cupra/elements/climatization_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from enum import Enum
 import logging
 
-from weconnect.addressable import AddressableAttribute
-from weconnect.api.cupra.elements.enums import ClimatizationState
-from weconnect.elements.generic_status import GenericStatus
+from weconnect_cupra.addressable import AddressableAttribute
+from weconnect_cupra.api.cupra.elements.enums import ClimatizationState
+from weconnect_cupra.elements.generic_status import GenericStatus
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class ClimatizationStatus(GenericStatus):
     def __init__(
         self,
         vehicle,
         parent,
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/controls.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/cupra/elements/controls.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import logging
 import json
 import requests
 
-from weconnect.addressable import AddressableObject, ChangeableAttribute
-from weconnect.elements.control_operation import ControlOperation
-from weconnect.api.cupra.elements.charging_settings import ChargingSettings
-from weconnect.api.cupra.elements.climatization_settings import ClimatizationSettings
-from weconnect.elements.error import Error
-from weconnect.errors import ControlError, SetterError
-from weconnect.util import celsiusToKelvin, farenheitToKelvin
-from weconnect.api.vw.domain import Domain
+from weconnect_cupra.addressable import AddressableObject, ChangeableAttribute
+from weconnect_cupra.elements.control_operation import ControlOperation
+from weconnect_cupra.api.cupra.elements.charging_settings import ChargingSettings
+from weconnect_cupra.api.cupra.elements.climatization_settings import ClimatizationSettings
+from weconnect_cupra.elements.error import Error
+from weconnect_cupra.errors import ControlError, SetterError
+from weconnect_cupra.util import celsiusToKelvin, farenheitToKelvin
+from weconnect_cupra.api.vw.domain import Domain
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class Controls(AddressableObject):
     def __init__(
         self,
         localAddress,
         vehicle,
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/engine_state.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/cupra/elements/engine_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from enum import Enum
 import logging
 
-from weconnect.addressable import AddressableAttribute
-from weconnect.elements.generic_status import GenericStatus
+from weconnect_cupra.addressable import AddressableAttribute
+from weconnect_cupra.elements.generic_status import GenericStatus
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class EngineState(GenericStatus):
     def __init__(
         self,
         vehicle,
         parent,
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/enums.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/cupra/elements/enums.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import Enum
-from weconnect.elements.control_operation import ControlInputEnum
+from weconnect_cupra.elements.control_operation import ControlInputEnum
 
 
 class MaximumChargeCurrent(ControlInputEnum,):
     MAXIMUM = 'maximum'
     REDUCED = 'reduced'
     INVALID = 'invalid'
     UNKNOWN = 'unknown'
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/error.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/elements/error.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import TYPE_CHECKING, Optional, Dict, Any
 
 import logging
 
 from datetime import datetime
 
-from weconnect.addressable import AddressableObject, AddressableAttribute
+from weconnect_cupra.addressable import AddressableObject, AddressableAttribute
 
 if TYPE_CHECKING:
-    from weconnect.elements.generic_status import GenericStatus
+    from weconnect_cupra.elements.generic_status import GenericStatus
 
-LOG: logging.Logger = logging.getLogger("weconnect")
+LOG: logging.Logger = logging.getLogger("weconnect_cupra")
 
 
 class Error(AddressableObject):
     def __init__(
         self,
         localAddress: str,
         parent: Optional['GenericStatus'],
@@ -63,11 +63,11 @@
                 and not self.retry.enabled:
             self.enabled = False
         else:
             self.enabled = True
 
         for key, value in {key: value for key, value in fromDict.items()
                            if key not in ['code', 'message', 'group', 'info', 'errorTimeStamp', 'retry']}.items():
-            LOG.debug('%s: Unknown attribute %s with value %s', self.getGlobalAddress(), key, value)
+            LOG.warning('%s: Unknown attribute %s with value %s', self.getGlobalAddress(), key, value)
 
     def __str__(self) -> str:
         return f'Error {self.code.value}: {self.message.value} \n\tinfo: {self.info.value} \n\ttimestamp: {self.timestamp.value}'
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/generic_capability.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/cupra/elements/generic_capability.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from enum import IntEnum
 import logging
 from datetime import datetime
 
-from weconnect.addressable import AddressableObject, AddressableAttribute
+from weconnect_cupra.addressable import AddressableObject, AddressableAttribute
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class GenericCapability(AddressableObject):
     def __init__(
         self,
         capabilityId,
         parent,
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/generic_settings.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/cupra/elements/generic_settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from enum import Enum
 import logging
 import json
 
 import requests
 
-from weconnect.addressable import AddressableLeaf, ChangeableAttribute, AliasChangeableAttribute
-from weconnect.elements.generic_status import GenericStatus
-from weconnect.elements.error import Error
-from weconnect.errors import SetterError
-from weconnect.api.cupra.domain import Domain
+from weconnect_cupra.addressable import AddressableLeaf, ChangeableAttribute, AliasChangeableAttribute
+from weconnect_cupra.elements.generic_status import GenericStatus
+from weconnect_cupra.elements.error import Error
+from weconnect_cupra.errors import SetterError
+from weconnect_cupra.api.cupra.domain import Domain
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class GenericSettings(GenericStatus):
     def valueChanged(self, element, flags):  # noqa: C901
         del element
         if flags & AddressableLeaf.ObserverEvent.VALUE_CHANGED \
                 and not flags & AddressableLeaf.ObserverEvent.UPDATED_FROM_SERVER:
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/helpers/request_tracker.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/helpers/request_tracker.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typing import TYPE_CHECKING, Tuple
 from datetime import datetime, timedelta
 from threading import Timer
 import logging
 
 if TYPE_CHECKING:
-    from weconnect.api.cupra.elements.vehicle import Vehicle
+    from weconnect_cupra.api.vw.elements.vehicle import Vehicle
 
-from weconnect.elements.generic_status import GenericStatus
-from weconnect.api.cupra.domain import Domain
+from weconnect_cupra.elements.generic_status import GenericStatus
+from weconnect_cupra.api.vw.domain import Domain
 
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class RequestTracker:
     def __init__(self, vehicle: 'Vehicle') -> None:
         self.vehicle: 'Vehicle' = vehicle
         self.requests: dict[Domain, list[Tuple[str, datetime, datetime]]] = {}
         self.__timer = None
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/odometer_measurement.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/cupra/elements/odometer_measurement.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 
-from weconnect.addressable import AddressableAttribute
-from weconnect.elements.generic_status import GenericStatus
+from weconnect_cupra.addressable import AddressableAttribute
+from weconnect_cupra.elements.generic_status import GenericStatus
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class OdometerMeasurement(GenericStatus):
     def __init__(
         self,
         vehicle,
         parent,
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/parking_position.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/cupra/elements/parking_position.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 
-from weconnect.addressable import AddressableAttribute
-from weconnect.elements.generic_status import GenericStatus
+from weconnect_cupra.addressable import AddressableAttribute
+from weconnect_cupra.elements.generic_status import GenericStatus
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class ParkingPosition(GenericStatus):
     def __init__(
         self,
         vehicle,
         parent,
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/cupra/elements/vehicle.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/cupra/elements/vehicle.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from __future__ import annotations
 from typing import Dict, List, Any, Optional
 from enum import Enum
 import logging
 
-from weconnect.addressable import AddressableObject, AddressableAttribute, AddressableDict, AddressableList
-from weconnect.api.cupra.elements.odometer_measurement import OdometerMeasurement
-from weconnect.api.cupra.elements.parking_position import ParkingPosition
-from weconnect.elements.error import Error
-from weconnect.elements.window_heating_status import WindowHeatingStatus
-from weconnect.errors import APICompatibilityError, APIError
-from weconnect.util import toBool
-from weconnect.api.cupra.domain import Domain
-from weconnect.fetch import Fetcher
-from weconnect.elements.plug_status import PlugStatus
-from weconnect.api.cupra.elements.climatization_status import ClimatizationStatus
-from weconnect.api.cupra.elements.climatization_settings import ClimatizationSettings
-from weconnect.api.cupra.elements.charging_settings import ChargingSettings
-from weconnect.api.cupra.elements.controls import Controls
-from weconnect.api.cupra.elements.generic_capability import GenericCapability
-from weconnect.api.cupra.elements.charging_status import ChargingStatus
-from weconnect.api.cupra.elements.helpers.request_tracker import RequestTracker
-from weconnect.api.cupra.elements.battery_status import BatteryStatus
-from weconnect.api.cupra.elements.access_status import AccessStatus
+from weconnect_cupra.addressable import AddressableObject, AddressableAttribute, AddressableDict, AddressableList
+from weconnect_cupra.api.cupra.elements.odometer_measurement import OdometerMeasurement
+from weconnect_cupra.api.cupra.elements.parking_position import ParkingPosition
+from weconnect_cupra.elements.error import Error
+from weconnect_cupra.elements.window_heating_status import WindowHeatingStatus
+from weconnect_cupra.errors import APICompatibilityError, APIError
+from weconnect_cupra.util import toBool
+from weconnect_cupra.api.cupra.domain import Domain
+from weconnect_cupra.fetch import Fetcher
+from weconnect_cupra.elements.plug_status import PlugStatus
+from weconnect_cupra.api.cupra.elements.climatization_status import ClimatizationStatus
+from weconnect_cupra.api.cupra.elements.climatization_settings import ClimatizationSettings
+from weconnect_cupra.api.cupra.elements.charging_settings import ChargingSettings
+from weconnect_cupra.api.cupra.elements.controls import Controls
+from weconnect_cupra.api.cupra.elements.generic_capability import GenericCapability
+from weconnect_cupra.api.cupra.elements.charging_status import ChargingStatus
+from weconnect_cupra.api.cupra.elements.helpers.request_tracker import RequestTracker
+from weconnect_cupra.api.cupra.elements.battery_status import BatteryStatus
+from weconnect_cupra.api.cupra.elements.access_status import AccessStatus
 
 
-LOG: logging.Logger = logging.getLogger("weconnect")
+LOG: logging.Logger = logging.getLogger("weconnect_cupra")
 
 
 class DomainDict(AddressableDict):
     def __init__(self, **kwargs):
         self.error: Error = Error(localAddress='error', parent=self)
         super().__init__(**kwargs)
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/vw/api.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 from __future__ import annotations
 from typing import List, Tuple, Optional
 import logging
 import locale
 
-from weconnect.addressable import AddressableDict, AddressableObject
-from weconnect.errors import RetrievalError
-from weconnect.api.vw.domain import Domain
-from weconnect.api.vw.elements.vehicle import Vehicle
-from weconnect.api.vw.elements.charging_station import ChargingStation
-from weconnect.fetch import Fetcher
+from weconnect_cupra.addressable import AddressableDict, AddressableObject
+from weconnect_cupra.errors import RetrievalError
+from weconnect_cupra.api.vw.domain import Domain
+from weconnect_cupra.api.vw.elements.vehicle import Vehicle
+from weconnect_cupra.api.vw.elements.charging_station import ChargingStation
+from weconnect_cupra.fetch import Fetcher
 
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class VwApi:
-    def __init__(self, weconnect: AddressableObject, fetcher: Fetcher, enableTracker: bool = False, fixAPI: bool = True):
+    def __init__(self, weconnect_cupra: AddressableObject, fetcher: Fetcher, enableTracker: bool = False, fixAPI: bool = True):
         self.base_url = 'https://mobileapi.apps.emea.vwapps.io'
-        self.__vehicles: AddressableDict[str, Vehicle] = AddressableDict(localAddress='vehicles', parent=weconnect)
-        self.__stations: AddressableDict[str, ChargingStation] = AddressableDict(localAddress='chargingStations', parent=weconnect)
+        self.__vehicles: AddressableDict[str, Vehicle] = AddressableDict(localAddress='vehicles', parent=weconnect_cupra)
+        self.__stations: AddressableDict[str, ChargingStation] = AddressableDict(localAddress='chargingStations', parent=weconnect_cupra)
         self.__fetcher: Fetcher = fetcher
         self.__enableTracker: bool = enableTracker
         self.fixAPI: bool = fixAPI
 
         # Used for charging station support
-        # Public api used by weconnect-mqtt
+        # Public api used by weconnect_cupra-mqtt
         self.latitude: Optional[float] = None
-        # Public api used by weconnect-mqtt
+        # Public api used by weconnect_cupra-mqtt
         self.longitude: Optional[float] = None
-        # Public api used by weconnect-mqtt
+        # Public api used by weconnect_cupra-mqtt
         self.searchRadius: Optional[int] = None
         self.market: Optional[str] = None
         self.useLocale: Optional[str] = locale.getlocale()[0]
 
 
     @property
     def vehicles(self) -> AddressableDict[str, Vehicle]:
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/vw/auth/we_charge_session.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/auth/we_charge_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 from requests.adapters import HTTPAdapter
 
 from oauthlib.common import add_params_to_uri
 from oauthlib.oauth2 import InsecureTransportError, is_secure_transport
 
 from requests.models import CaseInsensitiveDict
 
-from weconnect.auth.openid_session import AccessType
-from weconnect.auth.vw_web_session import VWWebSession
-from weconnect.errors import APICompatibilityError, AuthentificationError, RetrievalError, TemporaryAuthentificationError
+from weconnect_cupra.auth.openid_session import AccessType
+from weconnect_cupra.auth.vw_web_session import VWWebSession
+from weconnect_cupra.errors import APICompatibilityError, AuthentificationError, RetrievalError, TemporaryAuthentificationError
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class WeChargeSession(VWWebSession):
     def __init__(self, sessionuser, **kwargs):
         super(WeChargeSession, self).__init__(client_id='0fa5ae01-ebc0-4901-a2aa-4dd60572ea0e@apps_vw-dilab_com',
                                               refresh_url='https://identity.vwgroup.io/oidc/v1/token',
                                               scope='openid profile address email cars vin',
@@ -195,15 +195,15 @@
         # Check for user id
         if 'userId' not in params or not params['userId']:
             if 'updated' in params and params['updated'] == 'dataprivacy':
                 raise AuthentificationError('You have to login at myvolkswagen.de and accept the terms and conditions')
             raise AuthentificationError('No user id provided')
         self.__userId = params['userId']  # pylint: disable=unused-private-member
 
-        # Now follow the forwarding until forwarding URL starts with 'weconnect://authenticated#'
+        # Now follow the forwarding until forwarding URL starts with 'weconnect_cupra://authenticated#'
         afterLoginUrl: str = login3Response.headers['Location']
 
         while True:
             if 'consent' in afterLoginUrl:
                 consentURL = afterLoginUrl
             afterLoginResponse = self.get(afterLoginUrl, allow_redirects=False, access_type=AccessType.NONE)
             if afterLoginResponse.status_code == requests.codes['internal_server_error']:
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/vw/auth/we_connect_session.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/auth/we_connect_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 from requests.adapters import HTTPAdapter
 
 from oauthlib.common import add_params_to_uri, generate_nonce, to_unicode
 from oauthlib.oauth2 import InsecureTransportError
 from oauthlib.oauth2 import is_secure_transport
 
 from requests.models import CaseInsensitiveDict
-from weconnect.auth.openid_session import AccessType
+from weconnect_cupra.auth.openid_session import AccessType
 
-from weconnect.auth.vw_web_session import VWWebSession
-from weconnect.errors import APICompatibilityError, AuthentificationError, RetrievalError, TemporaryAuthentificationError
+from weconnect_cupra.auth.vw_web_session import VWWebSession
+from weconnect_cupra.errors import APICompatibilityError, AuthentificationError, RetrievalError, TemporaryAuthentificationError
 
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class WeConnectSession(VWWebSession):
     def __init__(self, sessionuser, **kwargs):
         super(WeConnectSession, self).__init__(client_id='a24fba63-34b3-4d43-b181-942111e6bda8@apps_vw-dilab_com',
                                                refresh_url='https://identity.vwgroup.io/oidc/v1/token',
                                                scope='openid profile badge cars dealers vin',
-                                               redirect_uri='weconnect://authenticated',
+                                               redirect_uri='weconnect_cupra://authenticated',
                                                state=None,
                                                sessionuser=sessionuser,
                                                **kwargs)
 
         self.headers = CaseInsensitiveDict({
             'accept': '*/*',
             'content-type': 'application/json',
@@ -51,21 +51,21 @@
         headers=None,
         withhold_token=False,
         access_type=AccessType.ACCESS,
         token=None,
         timeout=None,
         **kwargs
     ):
-        """Intercept all requests and add weconnect-trace-id header."""
+        """Intercept all requests and add weconnect_cupra-trace-id header."""
 
         import secrets
         traceId = secrets.token_hex(16)
         weConnectTraceId = (traceId[:8] + '-' + traceId[8:12] + '-' + traceId[12:16] + '-' + traceId[16:20] + '-' + traceId[20:]).upper()
         headers = headers or {}
-        headers['weconnect-trace-id'] = weConnectTraceId
+        headers['weconnect_cupra-trace-id'] = weConnectTraceId
 
         return super(WeConnectSession, self).request(
             method, url, headers=headers, data=data, withhold_token=withhold_token, access_type=access_type, token=token, timeout=timeout, **kwargs
         )
 
     def login(self):
         authorizationUrl = self.authorizationUrl(url='https://identity.vwgroup.io/oidc/v1/authorize')
@@ -234,15 +234,15 @@
         # Check for user id
         if 'userId' not in params or not params['userId']:
             if 'updated' in params and params['updated'] == 'dataprivacy':
                 raise AuthentificationError('You have to login at myvolkswagen.de and accept the terms and conditions')
             raise APICompatibilityError('No user id provided')
         self.__userId = params['userId']  # pylint: disable=unused-private-member
 
-        # Now follow the forwarding until forwarding URL starts with 'weconnect://authenticated#'
+        # Now follow the forwarding until forwarding URL starts with 'weconnect_cupra://authenticated#'
         afterLoginUrl: str = login3Response.headers['Location']
 
         consentURL = None
         while True:
             if 'consent' in afterLoginUrl:
                 consentURL = afterLoginUrl
             afterLoginResponse = self.get(afterLoginUrl, allow_redirects=False, access_type=AccessType.NONE)
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/vw/domain.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/domain.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/access_status.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/access_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from enum import Enum
 import logging
 
-from weconnect.addressable import AddressableObject, AddressableAttribute, AddressableDict
-from weconnect.elements.generic_status import GenericStatus
+from weconnect_cupra.addressable import AddressableObject, AddressableAttribute, AddressableDict
+from weconnect_cupra.elements.generic_status import GenericStatus
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class AccessStatus(GenericStatus):
     def __init__(
         self,
         vehicle,
         parent,
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/battery_status.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/battery_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 
-from weconnect.addressable import AddressableAttribute
-from weconnect.elements.generic_status import GenericStatus
+from weconnect_cupra.addressable import AddressableAttribute
+from weconnect_cupra.elements.generic_status import GenericStatus
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class BatteryStatus(GenericStatus):
     def __init__(
         self,
         vehicle,
         parent,
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/capability_status.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/capability_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 
-from weconnect.addressable import AddressableDict
-from weconnect.elements.generic_status import GenericStatus
-from weconnect.api.vw.elements.generic_capability import GenericCapability
+from weconnect_cupra.addressable import AddressableDict
+from weconnect_cupra.elements.generic_status import GenericStatus
+from weconnect_cupra.api.vw.elements.generic_capability import GenericCapability
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class CapabilityStatus(GenericStatus):
     def __init__(
         self,
         vehicle,
         parent,
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/charge_mode.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/charge_mode.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from enum import Enum
 from typing import List
 import logging
 
-from weconnect.addressable import AddressableAttribute, AddressableObject
-from weconnect.elements.generic_status import GenericStatus
+from weconnect_cupra.addressable import AddressableAttribute, AddressableObject
+from weconnect_cupra.elements.generic_status import GenericStatus
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class ChargeMode(GenericStatus):
     def __init__(
         self,
         vehicle,
         parent,
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/charging_profiles.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/charging_profiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from datetime import datetime, time
 import logging
 
-from weconnect.addressable import AddressableAttribute, AddressableDict, AddressableObject
-from weconnect.api.vw.elements.enums import UnlockPlugState
-from weconnect.api.vw.elements.generic_settings import GenericSettings
-from weconnect.api.vw.elements.timer import Timer
+from weconnect_cupra.addressable import AddressableAttribute, AddressableDict, AddressableObject
+from weconnect_cupra.api.vw.elements.enums import UnlockPlugState
+from weconnect_cupra.api.vw.elements.generic_settings import GenericSettings
+from weconnect_cupra.api.vw.elements.timer import Timer
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class ChargingProfiles(GenericSettings):
     def __init__(
         self,
         vehicle,
         parent,
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/charging_settings.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/charging_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 
-from weconnect.addressable import AddressableLeaf, ChangeableAttribute
-from weconnect.api.vw.elements.generic_settings import GenericSettings
-from weconnect.api.vw.elements.enums import UnlockPlugState, MaximumChargeCurrent
+from weconnect_cupra.addressable import AddressableLeaf, ChangeableAttribute
+from weconnect_cupra.api.vw.elements.generic_settings import GenericSettings
+from weconnect_cupra.api.vw.elements.enums import UnlockPlugState, MaximumChargeCurrent
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class ChargingSettings(GenericSettings):
     def __init__(
         self,
         vehicle,
         parent,
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/charging_station.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/charging_station.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from enum import Enum
 
-from weconnect.addressable import AddressableObject, AddressableAttribute, AddressableList
+from weconnect_cupra.addressable import AddressableObject, AddressableAttribute, AddressableList
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class ChargingStation(AddressableObject):  # pylint: disable=too-many-instance-attributes
 
     def __init__(
         self,
         weConnect,
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/charging_status.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/charging_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from enum import Enum
 import logging
 
-from weconnect.addressable import AddressableAttribute
-from weconnect.elements.generic_status import GenericStatus
+from weconnect_cupra.addressable import AddressableAttribute
+from weconnect_cupra.elements.generic_status import GenericStatus
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class ChargingStatus(GenericStatus):
     def __init__(
         self,
         vehicle,
         parent,
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/climatization_settings.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/climatization_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from enum import Enum
 import logging
 
-from weconnect.addressable import AddressableLeaf, ChangeableAttribute, AddressableAttribute, AliasChangeableAttribute
-from weconnect.api.vw.elements.generic_settings import GenericSettings
-from weconnect.util import celsiusToKelvin, farenheitToKelvin
+from weconnect_cupra.addressable import AddressableLeaf, ChangeableAttribute, AddressableAttribute, AliasChangeableAttribute
+from weconnect_cupra.api.vw.elements.generic_settings import GenericSettings
+from weconnect_cupra.util import celsiusToKelvin, farenheitToKelvin
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class ClimatizationSettings(GenericSettings):
     def __init__(
         self,
         vehicle,
         parent,
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/climatization_status.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/climatization_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from enum import Enum
 import logging
 
-from weconnect.addressable import AddressableAttribute
-from weconnect.elements.generic_status import GenericStatus
+from weconnect_cupra.addressable import AddressableAttribute
+from weconnect_cupra.elements.generic_status import GenericStatus
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class ClimatizationStatus(GenericStatus):
     def __init__(
         self,
         vehicle,
         parent,
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/climatization_timer.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/climatization_timer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from datetime import datetime
 import logging
 
-from weconnect.addressable import AddressableAttribute, AddressableDict
-from weconnect.elements.generic_status import GenericStatus
-from weconnect.api.vw.elements.timer import Timer
+from weconnect_cupra.addressable import AddressableAttribute, AddressableDict
+from weconnect_cupra.elements.generic_status import GenericStatus
+from weconnect_cupra.api.vw.elements.timer import Timer
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class ClimatizationTimer(GenericStatus):
     def __init__(
         self,
         vehicle,
         parent,
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/controls.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/controls.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import logging
 import json
 import requests
 
-from weconnect.addressable import AddressableObject, ChangeableAttribute
-from weconnect.elements.control_operation import ControlOperation
-from weconnect.api.vw.elements.charging_settings import ChargingSettings
-from weconnect.api.vw.elements.climatization_settings import ClimatizationSettings
-from weconnect.elements.error import Error
-from weconnect.errors import ControlError, SetterError
-from weconnect.util import celsiusToKelvin, farenheitToKelvin
-from weconnect.api.vw.domain import Domain
+from weconnect_cupra.addressable import AddressableObject, ChangeableAttribute
+from weconnect_cupra.elements.control_operation import ControlOperation
+from weconnect_cupra.api.vw.elements.charging_settings import ChargingSettings
+from weconnect_cupra.api.vw.elements.climatization_settings import ClimatizationSettings
+from weconnect_cupra.elements.error import Error
+from weconnect_cupra.errors import ControlError, SetterError
+from weconnect_cupra.util import celsiusToKelvin, farenheitToKelvin
+from weconnect_cupra.api.vw.domain import Domain
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class Controls(AddressableObject):
     def __init__(
         self,
         localAddress,
         vehicle,
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/enums.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/enums.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from weconnect.elements.control_operation import ControlInputEnum
+from weconnect_cupra.elements.control_operation import ControlInputEnum
 
 
 class MaximumChargeCurrent(ControlInputEnum,):
     MAXIMUM = 'maximum'
     REDUCED = 'reduced'
     INVALID = 'invalid'
     UNKNOWN = 'unknown'
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/generic_capability.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/generic_capability.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from enum import IntEnum
 import logging
 from datetime import datetime
 
-from weconnect.addressable import AddressableObject, AddressableAttribute
+from weconnect_cupra.addressable import AddressableObject, AddressableAttribute
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class GenericCapability(AddressableObject):
     def __init__(
         self,
         capabilityId,
         parent,
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/generic_request_status.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/generic_request_status.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from enum import Enum
 import logging
 
-from weconnect.addressable import AddressableAttribute
-from weconnect.elements.generic_status import GenericStatus
+from weconnect_cupra.addressable import AddressableAttribute
+from weconnect_cupra.elements.generic_status import GenericStatus
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class GenericRequestStatus(GenericStatus):
     def __init__(
         self,
         vehicle,
         parent,
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/generic_settings.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/generic_settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from enum import Enum
 import logging
 
 import json
 import requests
 
-from weconnect.addressable import AddressableLeaf, ChangeableAttribute, AliasChangeableAttribute
-from weconnect.elements.generic_status import GenericStatus
-from weconnect.elements.error import Error
-from weconnect.errors import SetterError
-from weconnect.api.vw.domain import Domain
+from weconnect_cupra.addressable import AddressableLeaf, ChangeableAttribute, AliasChangeableAttribute
+from weconnect_cupra.elements.generic_status import GenericStatus
+from weconnect_cupra.elements.error import Error
+from weconnect_cupra.errors import SetterError
+from weconnect_cupra.api.vw.domain import Domain
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class GenericSettings(GenericStatus):
     def valueChanged(self, element, flags):  # noqa: C901
         del element
         if flags & AddressableLeaf.ObserverEvent.VALUE_CHANGED \
                 and not flags & AddressableLeaf.ObserverEvent.UPDATED_FROM_SERVER:
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/helpers/request_tracker.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/cupra/elements/helpers/request_tracker.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typing import TYPE_CHECKING, Tuple
 from datetime import datetime, timedelta
 from threading import Timer
 import logging
 
 if TYPE_CHECKING:
-    from weconnect.api.vw.elements.vehicle import Vehicle
+    from weconnect_cupra.api.cupra.elements.vehicle import Vehicle
 
-from weconnect.elements.generic_status import GenericStatus
-from weconnect.api.vw.domain import Domain
+from weconnect_cupra.elements.generic_status import GenericStatus
+from weconnect_cupra.api.cupra.domain import Domain
 
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class RequestTracker:
     def __init__(self, vehicle: 'Vehicle') -> None:
         self.vehicle: 'Vehicle' = vehicle
         self.requests: dict[Domain, list[Tuple[str, datetime, datetime]]] = {}
         self.__timer = None
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/lights_status.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/lights_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from enum import Enum
 import logging
 
-from weconnect.addressable import AddressableAttribute, AddressableObject, AddressableDict
-from weconnect.elements.generic_status import GenericStatus
+from weconnect_cupra.addressable import AddressableAttribute, AddressableObject, AddressableDict
+from weconnect_cupra.elements.generic_status import GenericStatus
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class LightsStatus(GenericStatus):
     def __init__(
         self,
         vehicle,
         parent,
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/lv_battery_status.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/lv_battery_status.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from enum import Enum
 import logging
 
-from weconnect.addressable import AddressableAttribute
-from weconnect.elements.generic_status import GenericStatus
+from weconnect_cupra.addressable import AddressableAttribute
+from weconnect_cupra.elements.generic_status import GenericStatus
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class LVBatteryStatus(GenericStatus):
     def __init__(
         self,
         vehicle,
         parent,
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/maintenance_status.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/maintenance_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 
-from weconnect.addressable import AddressableAttribute
-from weconnect.elements.generic_status import GenericStatus
+from weconnect_cupra.addressable import AddressableAttribute
+from weconnect_cupra.elements.generic_status import GenericStatus
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class MaintenanceStatus(GenericStatus):
     def __init__(
         self,
         vehicle,
         parent,
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/odometer_measurement.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/odometer_measurement.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 
-from weconnect.addressable import AddressableAttribute
-from weconnect.elements.generic_status import GenericStatus
+from weconnect_cupra.addressable import AddressableAttribute
+from weconnect_cupra.elements.generic_status import GenericStatus
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class OdometerMeasurement(GenericStatus):
     def __init__(
         self,
         vehicle,
         parent,
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/parking_position.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/parking_position.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 
-from weconnect.addressable import AddressableAttribute
-from weconnect.elements.generic_status import GenericStatus
+from weconnect_cupra.addressable import AddressableAttribute
+from weconnect_cupra.elements.generic_status import GenericStatus
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class ParkingPosition(GenericStatus):
     def __init__(
         self,
         vehicle,
         parent,
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/range_measurements.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/range_measurements.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 
-from weconnect.addressable import AddressableAttribute
-from weconnect.elements.generic_status import GenericStatus
+from weconnect_cupra.addressable import AddressableAttribute
+from weconnect_cupra.elements.generic_status import GenericStatus
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class RangeMeasurements(GenericStatus):
     def __init__(
         self,
         vehicle,
         parent,
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/range_status.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/range_status.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from enum import Enum
 import logging
 
-from weconnect.addressable import AddressableAttribute, AddressableObject
-from weconnect.elements.generic_status import GenericStatus
+from weconnect_cupra.addressable import AddressableAttribute, AddressableObject
+from weconnect_cupra.elements.generic_status import GenericStatus
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class RangeStatus(GenericStatus):
     def __init__(
         self,
         vehicle,
         parent,
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/readiness_status.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/readiness_status.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from enum import Enum
 import logging
 
-from weconnect.addressable import AddressableObject, AddressableAttribute
-from weconnect.elements.generic_status import GenericStatus
-from weconnect.util import toBool
+from weconnect_cupra.addressable import AddressableObject, AddressableAttribute
+from weconnect_cupra.elements.generic_status import GenericStatus
+from weconnect_cupra.util import toBool
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class ReadinessStatus(GenericStatus):
     def __init__(
         self,
         vehicle,
         parent,
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/timer.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/timer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from datetime import datetime
 import logging
 
-from weconnect.addressable import AddressableObject, AddressableAttribute, AddressableDict
+from weconnect_cupra.addressable import AddressableObject, AddressableAttribute, AddressableDict
 
-from weconnect.util import robustTimeParse, toBool
+from weconnect_cupra.util import robustTimeParse, toBool
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class Timer(AddressableObject):
     def __init__(
         self,
         parent,
         fromDict=None,
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/vehicle.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/vehicle.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,57 +5,57 @@
 from datetime import datetime, timedelta
 import base64
 import io
 import logging
 
 from requests import exceptions, codes
 
-from weconnect.api.vw.elements.generic_settings import GenericSettings
-from weconnect.elements.generic_status import GenericStatus
-from weconnect.addressable import AddressableObject, AddressableAttribute, AddressableDict, AddressableList
-from weconnect.fetch import Fetcher
-from weconnect.elements.plug_status import PlugStatus
-from weconnect.elements.window_heating_status import WindowHeatingStatus
-from weconnect.api.vw.elements.generic_capability import GenericCapability
-from weconnect.api.vw.elements.generic_request_status import GenericRequestStatus
-from weconnect.api.vw.elements.controls import Controls
-from weconnect.api.vw.elements.access_status import AccessStatus
-from weconnect.api.vw.elements.battery_status import BatteryStatus
-from weconnect.api.vw.elements.lv_battery_status import LVBatteryStatus
-from weconnect.api.vw.elements.capability_status import CapabilityStatus
-from weconnect.api.vw.elements.charging_status import ChargingStatus
-from weconnect.api.vw.elements.charging_settings import ChargingSettings
-from weconnect.api.vw.elements.charge_mode import ChargeMode
-from weconnect.api.vw.elements.climatization_status import ClimatizationStatus
-from weconnect.api.vw.elements.climatization_settings import ClimatizationSettings
-from weconnect.api.vw.elements.climatization_timer import ClimatizationTimer
-from weconnect.api.vw.elements.lights_status import LightsStatus
-from weconnect.api.vw.elements.maintenance_status import MaintenanceStatus
-from weconnect.api.vw.elements.warning_lights_status import WarningLightsStatus
-from weconnect.api.vw.elements.parking_position import ParkingPosition
-from weconnect.api.vw.elements.range_status import RangeStatus
-from weconnect.api.vw.elements.odometer_measurement import OdometerMeasurement
-from weconnect.api.vw.elements.range_measurements import RangeMeasurements
-from weconnect.api.vw.elements.readiness_status import ReadinessStatus
-from weconnect.api.vw.elements.charging_profiles import ChargingProfiles
-from weconnect.errors import APICompatibilityError, RetrievalError, APIError
-from weconnect.util import toBool
-from weconnect.weconnect_errors import ErrorEventType
-from weconnect.api.vw.domain import Domain
-from weconnect.elements.error import Error
-from weconnect.api.vw.elements.helpers.request_tracker import RequestTracker
+from weconnect_cupra.api.vw.elements.generic_settings import GenericSettings
+from weconnect_cupra.elements.generic_status import GenericStatus
+from weconnect_cupra.addressable import AddressableObject, AddressableAttribute, AddressableDict, AddressableList
+from weconnect_cupra.fetch import Fetcher
+from weconnect_cupra.elements.plug_status import PlugStatus
+from weconnect_cupra.elements.window_heating_status import WindowHeatingStatus
+from weconnect_cupra.api.vw.elements.generic_capability import GenericCapability
+from weconnect_cupra.api.vw.elements.generic_request_status import GenericRequestStatus
+from weconnect_cupra.api.vw.elements.controls import Controls
+from weconnect_cupra.api.vw.elements.access_status import AccessStatus
+from weconnect_cupra.api.vw.elements.battery_status import BatteryStatus
+from weconnect_cupra.api.vw.elements.lv_battery_status import LVBatteryStatus
+from weconnect_cupra.api.vw.elements.capability_status import CapabilityStatus
+from weconnect_cupra.api.vw.elements.charging_status import ChargingStatus
+from weconnect_cupra.api.vw.elements.charging_settings import ChargingSettings
+from weconnect_cupra.api.vw.elements.charge_mode import ChargeMode
+from weconnect_cupra.api.vw.elements.climatization_status import ClimatizationStatus
+from weconnect_cupra.api.vw.elements.climatization_settings import ClimatizationSettings
+from weconnect_cupra.api.vw.elements.climatization_timer import ClimatizationTimer
+from weconnect_cupra.api.vw.elements.lights_status import LightsStatus
+from weconnect_cupra.api.vw.elements.maintenance_status import MaintenanceStatus
+from weconnect_cupra.api.vw.elements.warning_lights_status import WarningLightsStatus
+from weconnect_cupra.api.vw.elements.parking_position import ParkingPosition
+from weconnect_cupra.api.vw.elements.range_status import RangeStatus
+from weconnect_cupra.api.vw.elements.odometer_measurement import OdometerMeasurement
+from weconnect_cupra.api.vw.elements.range_measurements import RangeMeasurements
+from weconnect_cupra.api.vw.elements.readiness_status import ReadinessStatus
+from weconnect_cupra.api.vw.elements.charging_profiles import ChargingProfiles
+from weconnect_cupra.errors import APICompatibilityError, RetrievalError, APIError
+from weconnect_cupra.util import toBool
+from weconnect_cupra.weconnect_errors import ErrorEventType
+from weconnect_cupra.api.vw.domain import Domain
+from weconnect_cupra.elements.error import Error
+from weconnect_cupra.api.vw.elements.helpers.request_tracker import RequestTracker
 
 SUPPORT_IMAGES = False
 try:
     from PIL import Image as PILImage, ImageDraw  # type: ignore
     SUPPORT_IMAGES = True
 except ImportError:
     pass
 
-LOG: logging.Logger = logging.getLogger("weconnect")
+LOG: logging.Logger = logging.getLogger("weconnect_cupra")
 
 
 class DomainDict(AddressableDict):
     def __init__(self, **kwargs):
         self.error: Error = Error(localAddress='error', parent=self)
         super(DomainDict, self).__init__(**kwargs)
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/api/vw/elements/warning_lights_status.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/vw/elements/warning_lights_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from enum import Enum
 import base64
 import io
 import logging
 
-from weconnect.addressable import AddressableAttribute, AddressableObject, AddressableDict
-from weconnect.elements.generic_status import GenericStatus
+from weconnect_cupra.addressable import AddressableAttribute, AddressableObject, AddressableDict
+from weconnect_cupra.elements.generic_status import GenericStatus
 
 SUPPORT_IMAGES = False
 try:
     from PIL import Image  # type: ignore
     SUPPORT_IMAGES = True
 except ImportError:
     pass
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class WarningLightsStatus(GenericStatus):
     def __init__(
         self,
         vehicle,
         parent,
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/auth/openid_session.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/auth/openid_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 
 from oauthlib.common import UNICODE_ASCII_CHARACTER_SET, generate_nonce, generate_token
 from oauthlib.oauth2.rfc6749.parameters import parse_authorization_code_response, parse_token_response, prepare_grant_uri
 
 from urllib3.util.retry import Retry
 from requests.adapters import HTTPAdapter
 
-from weconnect.auth.auth_util import addBearerAuthHeader
-from weconnect.errors import AuthentificationError, RetrievalError
+from weconnect_cupra.auth.auth_util import addBearerAuthHeader
+from weconnect_cupra.errors import AuthentificationError, RetrievalError
 
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class AccessType(Enum):
     NONE = auto()
     ACCESS = auto()
     ID = auto()
     REFRESH = auto()
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/auth/session_manager.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/auth/session_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 
 import hashlib
 
 import json
 import logging
 
-from weconnect.auth.openid_session import OpenIDSession
-from weconnect.service import Service
+from weconnect_cupra.auth.openid_session import OpenIDSession
+from weconnect_cupra.service import Service
 # VW specific
-from weconnect.api.vw.auth.we_connect_session import WeConnectSession
-from weconnect.api.vw.auth.we_charge_session import WeChargeSession
+from weconnect_cupra.api.vw.auth.we_connect_session import WeConnectSession
+from weconnect_cupra.api.vw.auth.we_charge_session import WeChargeSession
 # Cupra specific
-from weconnect.api.cupra.auth.my_cupra_session import MyCupraSession
+from weconnect_cupra.api.cupra.auth.my_cupra_session import MyCupraSession
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class SessionUser():
     def __init__(self, username: str, password: str) -> None:
         self.username = username
         self.password = password
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/elements/access_control_state.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/elements/access_control_state.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/elements/control_operation.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/elements/control_operation.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/elements/error.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/api/cupra/elements/error.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import TYPE_CHECKING, Optional, Dict, Any
 
 import logging
 
 from datetime import datetime
 
-from weconnect.addressable import AddressableObject, AddressableAttribute
+from weconnect_cupra.addressable import AddressableObject, AddressableAttribute
 
 if TYPE_CHECKING:
-    from weconnect.elements.generic_status import GenericStatus
+    from weconnect_cupra.elements.generic_status import GenericStatus
 
-LOG: logging.Logger = logging.getLogger("weconnect")
+LOG: logging.Logger = logging.getLogger("weconnect_cupra")
 
 
 class Error(AddressableObject):
     def __init__(
         self,
         localAddress: str,
         parent: Optional['GenericStatus'],
@@ -63,11 +63,11 @@
                 and not self.retry.enabled:
             self.enabled = False
         else:
             self.enabled = True
 
         for key, value in {key: value for key, value in fromDict.items()
                            if key not in ['code', 'message', 'group', 'info', 'errorTimeStamp', 'retry']}.items():
-            LOG.warning('%s: Unknown attribute %s with value %s', self.getGlobalAddress(), key, value)
+            LOG.debug('%s: Unknown attribute %s with value %s', self.getGlobalAddress(), key, value)
 
     def __str__(self) -> str:
         return f'Error {self.code.value}: {self.message.value} \n\tinfo: {self.info.value} \n\ttimestamp: {self.timestamp.value}'
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/elements/generic_status.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/elements/generic_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING, Optional, Dict, Any, List
 
 from enum import Enum
 import logging
 from datetime import datetime, timedelta, timezone
 
-from weconnect.util import robustTimeParse
-from weconnect.addressable import AddressableObject, AddressableAttribute, AddressableList, AddressableDict
-from weconnect.elements.control_operation import ControlOperation
-from weconnect.elements.error import Error
+from weconnect_cupra.util import robustTimeParse
+from weconnect_cupra.addressable import AddressableObject, AddressableAttribute, AddressableList, AddressableDict
+from weconnect_cupra.elements.control_operation import ControlOperation
+from weconnect_cupra.elements.error import Error
 
-LOG: logging.Logger = logging.getLogger("weconnect")
+LOG: logging.Logger = logging.getLogger("weconnect_cupra")
 
 
 class GenericStatus(AddressableObject):
     def __init__(
         self,
         vehicle,
         parent: AddressableDict[str, GenericStatus],
@@ -56,15 +56,15 @@
                     # interval is large
                     fixed: timedelta = timedelta(hours=0, minutes=0)
                     while carCapturedTimestamp > datetime.utcnow().replace(tzinfo=timezone.utc):
                         carCapturedTimestamp -= timedelta(hours=0, minutes=30)
                         fixed -= timedelta(hours=0, minutes=30)
                     if fixed > timedelta(hours=0, minutes=0):
                         LOG.debug('%s: Attribute carCapturedTimestamp was in the future. Substracted %s to fix this.'
-                                    ' This is a problem of the weconnect API and might be fixed in the future',
+                                    ' This is a problem of the weconnect_cupra API and might be fixed in the future',
                                     self.getGlobalAddress(), fixed)
                     if carCapturedTimestamp == datetime(year=2000, month=1, day=1, hour=0, minute=0, second=0,
                                                         tzinfo=timezone.utc):
                         carCapturedTimestamp = None
 
                 self.carCapturedTimestamp.setValueWithCarTime(carCapturedTimestamp, lastUpdateFromCar=None, fromServer=True)
                 if self.carCapturedTimestamp.value is None:
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/elements/plug_status.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/elements/plug_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from enum import Enum
 import logging
 
-from weconnect.addressable import AddressableAttribute
-from weconnect.elements.generic_status import GenericStatus
+from weconnect_cupra.addressable import AddressableAttribute
+from weconnect_cupra.elements.generic_status import GenericStatus
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class PlugStatus(GenericStatus):
     def __init__(
         self,
         vehicle,
         parent,
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/elements/window_heating_status.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/elements/window_heating_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from enum import Enum
 import logging
 
-from weconnect.addressable import AddressableAttribute, AddressableDict, AddressableObject
-from weconnect.elements.generic_status import GenericStatus
+from weconnect_cupra.addressable import AddressableAttribute, AddressableDict, AddressableObject
+from weconnect_cupra.elements.generic_status import GenericStatus
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class WindowHeatingStatus(GenericStatus):
     def __init__(
         self,
         vehicle,
         parent,
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/errors.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 from typing import Dict, List, Set, Tuple, Callable, Any, Optional
 import logging
 
-from weconnect.weconnect_errors import ErrorEventType
-from weconnect.addressable import AddressableLeaf, AddressableObject, AddressableDict
+from weconnect_cupra.weconnect_errors import ErrorEventType
+from weconnect_cupra.addressable import AddressableLeaf, AddressableObject, AddressableDict
 
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class RetrievalError(Exception):
     pass
 
 
 class SetterError(Exception):
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/fetch.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/fetch.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 from datetime import datetime, timedelta
 import logging
 import json
 import os
 
 import requests
 
-from weconnect.auth.openid_session import OpenIDSession
-from weconnect.weconnect_errors import ErrorEventType
-from weconnect.errors import ErrorBus, RetrievalError
-from weconnect.util import ExtendedEncoder
+from weconnect_cupra.auth.openid_session import OpenIDSession
+from weconnect_cupra.weconnect_errors import ErrorEventType
+from weconnect_cupra.errors import ErrorBus, RetrievalError
+from weconnect_cupra.util import ExtendedEncoder
 
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 
 class Fetcher:
 
     def __init__(self,
         session: OpenIDSession,
         errorBus: ErrorBus,
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/util.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/util.py`

 * *Files identical despite different names*

### Comparing `weconnect-cupra-daern-0.49.20/weconnect/weconnect.py` & `weconnect-cupra-daern-0.50.1/weconnect_cupra/weconnect_cupra.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from __future__ import annotations
 from typing import Dict, List, Any, Optional
 
 import locale
 import logging
 from datetime import timedelta
 
-from weconnect.auth.openid_session import OpenIDSession
-from weconnect.auth.session_manager import SessionManager, Service, SessionUser
-from weconnect.addressable import AddressableLeaf, AddressableObject, AddressableDict
-from weconnect.fetch import Fetcher
-from weconnect.errors import ErrorBus
+from weconnect_cupra.auth.openid_session import OpenIDSession
+from weconnect_cupra.auth.session_manager import SessionManager, Service, SessionUser
+from weconnect_cupra.addressable import AddressableLeaf, AddressableObject, AddressableDict
+from weconnect_cupra.fetch import Fetcher
+from weconnect_cupra.errors import ErrorBus
 # VW specific
-from weconnect.api.vw.domain import Domain
-from weconnect.api.vw.api import VwApi
-from weconnect.api.vw.elements.vehicle import Vehicle as VwVehicle
+from weconnect_cupra.api.vw.domain import Domain
+from weconnect_cupra.api.vw.api import VwApi
+from weconnect_cupra.api.vw.elements.vehicle import Vehicle as VwVehicle
 # Cupra specific
-from weconnect.api.cupra.api import CupraApi
-from weconnect.api.cupra.elements.vehicle import Vehicle as CupraVehicle
+from weconnect_cupra.api.cupra.api import CupraApi
+from weconnect_cupra.api.cupra.elements.vehicle import Vehicle as CupraVehicle
 
-from weconnect.__version import __version__ as VERSION
+from weconnect_cupra.__version import __version__ as VERSION
 
-LOG = logging.getLogger("weconnect")
+LOG = logging.getLogger("weconnect_cupra")
 
 class WeConnect(AddressableObject):  # pylint: disable=too-many-instance-attributes, too-many-public-methods
     """Main class used to interact with WeConnect"""
 
     def __init__(  # noqa: C901 # pylint: disable=too-many-arguments
         self,
         username: str,
@@ -60,15 +60,15 @@
             updatePictures (bool, optional):  Also fetch and update pictures. Defaults to True.
             numRetries (int, optional): Number of retries when http requests are failing. Defaults to 3.
             timeout (bool, optional, optional): Timeout in seconds used for http connections to the VW servers
             selective (list[Domain], optional): Domains to request data for
         """
         super().__init__(localAddress='', parent=None)
 
-        LOG.info(f'Weconnect-python version {VERSION}')
+        LOG.info(f'Weconnect-Cupra-python version {VERSION}')
 
         self.username: str = username
         self.password: str = password
 
         self.__userId: Optional[str] = None  # pylint: disable=unused-private-member
 
         self.fixAPI: bool = fixAPI
@@ -87,17 +87,17 @@
         self.__fetcher: Fetcher = Fetcher(session=self.__session, maxAge=maxAge, maxAgePictures=maxAgePictures, errorBus=ErrorBus())
 
         if loginOnInit:
             self.__session.login()
 
         # Construct the actual service adapter
         if service == Service.MY_CUPRA:
-            self.__api = CupraApi(weconnect=self, fetcher=self.__fetcher)
-        else:
-            self.__api = VwApi(weconnect=self, fetcher=self.__fetcher)
+            self.__api = CupraApi(weconnect_cupra=self, fetcher=self.__fetcher)
+        # else:
+        #     self.__api = VwApi(weconnect_cupra=self, fetcher=self.__fetcher)
         self.__fetcher.base_url = self.__api.base_url
 
         if updateAfterLogin:
             self.update(updateCapabilities=updateCapabilities, updatePictures=updatePictures, selective=selective)
 
 
     def __del__(self) -> None:
@@ -109,27 +109,27 @@
         return self.__session
 
     @property
     def cache(self) -> Dict[str, Any]:
         return self.__fetcher.cache
 
     # Used for charging station support
-    # Public api used by weconnect-mqtt
+    # Public api used by weconnect_cupra-mqtt
     @property
     def latitude(self) -> Optional[float]:
         return self.__api.latitude
 
     # Used for charging station support
-    # Public api used by weconnect-mqtt
+    # Public api used by weconnect_cupra-mqtt
     @property
     def longitude(self) -> Optional[float]:
         return self.__api.longitude
 
     # Used for charging station support
-    # Public api used by weconnect-mqtt
+    # Public api used by weconnect_cupra-mqtt
     @property
     def searchRadius(self) -> Optional[int]:
         return self.__api.searchRadius
 
     # Used for charging station support
     @property
     def market(self) -> Optional[str]:
@@ -141,39 +141,39 @@
         return self.__api.useLocale
 
     # Public api used by HA volkswagen_we_connect_id
     @property
     def vehicles(self) -> AddressableDict[str, VwVehicle|CupraVehicle]:
         return self.__api.vehicles
 
-    # Public api used by weconnect-mqtt
+    # Public api used by weconnect_cupra-mqtt
     def persistTokens(self) -> None:
         if self.__manager is not None and self.tokenfile is not None:
             self.__manager.saveTokenstore(self.tokenfile)
 
-    # Public api used by weconnect-mqtt
+    # Public api used by weconnect_cupra-mqtt
     def enableTracker(self) -> None:
         self.__enableTracker = True
         for vehicle in self.vehicles.values():
             vehicle.enableTracker()
 
     def disableTracker(self) -> None:
         self.__enableTracker = True
         for vehicle in self.vehicles.values():
             vehicle.disableTracker()
 
     # Public api used by HA volkswagen_we_connect_id
     def login(self) -> None:
         self.__session.login()
 
-    # Public api used by weconnect-mqtt
+    # Public api used by weconnect_cupra-mqtt
     def disconnect(self) -> None:
         pass
 
-    # Public api used by weconnect-mqtt, HA volkswagen_we_connect_id
+    # Public api used by weconnect_cupra-mqtt, HA volkswagen_we_connect_id
     def update(self, updateCapabilities: bool = True, updatePictures: bool = True, force: bool = False,
                selective: Optional[list[Domain]] = None) -> None:
         self.__elapsed.clear()
         self.__api.update(updateCapabilities=updateCapabilities, updatePictures=updatePictures, force=force, selective=selective)
         self.updateComplete()
 
     def setChargingStationSearchParameters(self, latitude: float, longitude: float, searchRadius: Optional[int] = None, market: Optional[str] = None,
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect_cupra_daern.egg-info/PKG-INFO` & `weconnect-cupra-daern-0.50.1/weconnect_cupra_daern.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,84 +1,82 @@
 Metadata-Version: 2.1
 Name: weconnect-cupra-daern
-Version: 0.49.20
-Summary: Fork of Python API for the Volkswagen WeConnect Services to support Cupra Born
-Home-page: https://github.com/daernsinstantfortress/WeConnect-python
+Version: 0.50.1
+Summary: Python API for the Cupra Born online services
+Home-page: https://github.com/daernsinstantfortress/WeConnect-Cupra-python
 Author: Till Steinbach / Alan Gibson / Stuart Hall
 License: MIT
 Project-URL: Funding, https://github.com/sponsors/tillsteinbach
-Project-URL: Source, https://github.com/daernsinstantfortress/WeConnect-python
-Project-URL: Bug Tracker, https://github.com/tillsteinbach/WeConnect-python/issues
-Description: 
-        
-        # WeConnect-python
-        [![GitHub sourcecode](https://img.shields.io/badge/Source-GitHub-green)](https://github.com/tillsteinbach/WeConnect-python/)
-        [![GitHub release (latest by date)](https://img.shields.io/github/v/release/tillsteinbach/WeConnect-python)](https://github.com/tillsteinbach/WeConnect-python/releases/latest)
-        [![GitHub](https://img.shields.io/github/license/tillsteinbach/WeConnect-python)](https://github.com/tillsteinbach/WeConnect-python/blob/master/LICENSE)
-        [![GitHub issues](https://img.shields.io/github/issues/tillsteinbach/WeConnect-python)](https://github.com/tillsteinbach/WeConnect-python/issues)
-        [![PyPI - Downloads](https://img.shields.io/pypi/dm/weconnect?label=PyPI%20Downloads)](https://pypi.org/project/weconnect/)
-        [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/weconnect)](https://pypi.org/project/weconnect/)
-        [![Donate at PayPal](https://img.shields.io/badge/Donate-PayPal-2997d8)](https://www.paypal.com/donate?hosted_button_id=2BVFF5GJ9SXAJ)
-        [![Sponsor at Github](https://img.shields.io/badge/Sponsor-GitHub-28a745)](https://github.com/sponsors/tillsteinbach)
-        
-        Python API for the Volkswagen WeConnect and Cupra MyCupra Services. If you are not a developer and ended up here you probably want to check out a project using this library (see below).
-        
-        ## Projects in which the library is used
-        - [VWsFriend](https://github.com/tillsteinbach/VWsFriend): VWsFriend records statistics about your car (charging sessions, battery, trips, fueling, etc.) and displays them nicely. It also allows you to forward data from the car to other applications such as [A better routeplanner](https://abetterrouteplanner.com/) and allows you to integrate your car into [Apple HomeKit](https://www.apple.com/ios/home/)
-        - [WeConnect-cli](https://github.com/tillsteinbach/WeConnect-cli): A commandline interface to interact with WeConnect
-        - [WeConnect-MQTT](https://github.com/tillsteinbach/WeConnect-mqtt): A MQTT Client that provides WeConnect data to the MQTT Broker of your choice (e.g. your home automation solution such as [ioBroker](https://www.iobroker.net), [FHEM](https://fhem.de) or [Home Assistant](https://www.home-assistant.io))
-        
-        ## Install
-        ```
-        pip3 install weconnect[Images]
-        ```
-        
-        ## Package
-        ```
-        python3 -m pip install --upgrade build
-        python3 -m build --sdist
-        python3 -m build --wheel
-        ```
-        
-        ## Distribute
-        ```
-        python3 -m pip install --upgrade twine
-        python3 -m twine upload --repository pypi dist/*
-        ```
-        
-        ## Getting started
-        - To get started have a look in the [examples folder](https://github.com/tillsteinbach/WeConnect-python/tree/main/examples)
-        
-        ## Tested with
-        - Volkswagen ID.3 Modelyear 2021
-        - Volkswagen Passat GTE Modelyear 2021
-        - Cupra Born Modelyear 2022
-        
-        ## Login & Consent
-        WeConnect-python is based on the new WeConnect ID API that was introduced with the new series of ID cars. If you use another car or hybrid you probably need to agree to the terms and conditions of the WeConnect ID interface. Easiest to do so is by installing the WeConnect ID app on your smartphone and login there. If necessary you will be asked to agree to the terms and conditions.
-        
-        ## Reporting Issues
-        Please feel free to open an issue at [GitHub Issue page](https://github.com/tillsteinbach/WeConnect-python/issues) to report problems you found.
-        
-        ### Known Issues
-        - The API is in alpha state and may change unexpectedly at any time! Please conscider this and pin to a specific version if you depend on it.
-        - Examples and API documentation is missing
-        
-        ## Credits
-        Inspired by [TA2k/ioBroker.vw-connect](https://github.com/TA2k/ioBroker.vw-connect/) that gave me a point to start working with the API
-        
-        ## Seat, Cupra, Skoda IV, ...
-        In an effort to try to make WeConnect-python also to work with latest generation of vehicles from other volkswagen brands I'm looking for users to temporarily share access to their accounts. If you are willing to support please send me a message.
-        - Already tried: Cupra Born (The API looks a bit different, maybe it is older, I will check again in some weeks), thanks to the user initdebugs
-        
-Keywords: weconnect,we connect,carnet,car net,volkswagen,vw,telemetry
+Project-URL: Source, https://github.com/daernsinstantfortress/WeConnect-Cupra-python
+Project-URL: Bug Tracker, https://github.com/daernsinstantfortress/WeConnect-Cupra-python/issues
+Keywords: weconnect_cupra,weconnect,we connect,carnet,car net,volkswagen,vw,telemetry,cupra
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: Images
+License-File: LICENSE
+
+
+
+# WeConnect-Cupra-python
+[![GitHub sourcecode](https://img.shields.io/badge/Source-GitHub-green)](https://github.com/daernsinstantfortress/WeConnect-Cupra-python)
+[![GitHub release (latest by date)](https://img.shields.io/github/v/release/daernsinstantfortress/WeConnect-Cupra-python)](https://github.com/daernsinstantfortress/WeConnect-Cupra-python/releases/latest)
+[![GitHub](https://img.shields.io/github/license/daernsinstantfortress/WeConnect-Cupra-python)](https://github.com/daernsinstantfortress/WeConnect-Cupra-python/blob/master/LICENSE)
+[![GitHub issues](https://img.shields.io/github/issues/daernsinstantfortress/WeConnect-Cupra-python)](https://github.com/daernsinstantfortress/WeConnect-Cupra-python/issues)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/weconnect-cupra-daern?label=PyPI%20Downloads)](https://pypi.org/project/weconnect-cupra-daern/)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/weconnect-cupra-daern)](https://pypi.org/project/weconnect-cupra-daern/)
+
+Python API for the MyCupra Services. If you are not a developer and ended up here you probably want to check out a project using this library (see below).
+
+## Projects in which the library is used
+- [VWsFriend](https://github.com/tillsteinbach/VWsFriend): VWsFriend records statistics about your car (charging sessions, battery, trips, fueling, etc.) and displays them nicely. It also allows you to forward data from the car to other applications such as [A better routeplanner](https://abetterrouteplanner.com/) and allows you to integrate your car into [Apple HomeKit](https://www.apple.com/ios/home/)
+- [WeConnect-cli](https://github.com/tillsteinbach/WeConnect-cli): A commandline interface to interact with WeConnect
+- [WeConnect-MQTT](https://github.com/tillsteinbach/WeConnect-mqtt): A MQTT Client that provides WeConnect data to the MQTT Broker of your choice (e.g. your home automation solution such as [ioBroker](https://www.iobroker.net), [FHEM](https://fhem.de) or [Home Assistant](https://www.home-assistant.io))
+
+## Install
+```
+pip3 install weconnect-cupra-daern[Images]
+```
+
+## Package
+```
+python3 -m pip install --upgrade build
+python3 -m build --sdist
+python3 -m build --wheel
+```
+
+## Distribute
+```
+python3 -m pip install --upgrade twine
+python3 -m twine upload --repository pypi dist/*
+```
+
+## Getting started
+- To get started have a look in the [examples folder](https://github.com/daernsinstantfortress/WeConnect-Cupra-python/tree/main/examples)
+
+## Tested with
+- Cupra Born Model year 2022/23
+
+## Login & Consent
+WeConnect-python is based on the new WeConnect ID API that was introduced with the new series of ID cars. If you use another car or hybrid you probably need to agree to the terms and conditions of the WeConnect ID interface. Easiest to do so is by installing the WeConnect ID app on your smartphone and login there. If necessary you will be asked to agree to the terms and conditions.
+
+## Reporting Issues
+Please feel free to open an issue at [GitHub Issue page](https://github.com/daernsinstantfortress/WeConnect-Cupra-python/issues) to report problems you found.
+
+### Known Issues
+- The API is in alpha state and may change unexpectedly at any time! Please conscider this and pin to a specific version if you depend on it.
+- Examples and API documentation is missing
+
+## Credits
+Largely based on WeConnect-python for VW from https://github.com/tillsteinbach/WeConnect-python, with the initial Cupra port developed by Alan Gibson
+Inspired by [TA2k/ioBroker.vw-connect](https://github.com/TA2k/ioBroker.vw-connect/) that gave me a point to start working with the API
+
+
```

### Comparing `weconnect-cupra-daern-0.49.20/weconnect_cupra_daern.egg-info/SOURCES.txt` & `weconnect-cupra-daern-0.50.1/weconnect_cupra_daern.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,105 +1,97 @@
+LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 tests/__init__.py
 tests/test_addressable.py
 tests/test_cupra.py
 tests/test_elements.py
-weconnect/__init__.py
-weconnect/__version.py
-weconnect/addressable.py
-weconnect/errors.py
-weconnect/fetch.py
-weconnect/service.py
-weconnect/util.py
-weconnect/weconnect.py
-weconnect/weconnect_errors.py
-weconnect/api/__init__.py
-weconnect/api/cupra/__init__.py
-weconnect/api/cupra/api.py
-weconnect/api/cupra/domain.py
-weconnect/api/cupra/auth/__init__.py
-weconnect/api/cupra/auth/my_cupra_session.py
-weconnect/api/cupra/elements/__init__.py
-weconnect/api/cupra/elements/access_status.py
-weconnect/api/cupra/elements/battery_status.py
-weconnect/api/cupra/elements/charging_settings.py
-weconnect/api/cupra/elements/charging_station.py
-weconnect/api/cupra/elements/charging_status.py
-weconnect/api/cupra/elements/climatization_settings.py
-weconnect/api/cupra/elements/climatization_status.py
-weconnect/api/cupra/elements/controls.py
-weconnect/api/cupra/elements/engine_state.py
-weconnect/api/cupra/elements/enums.py
-weconnect/api/cupra/elements/error.py
-weconnect/api/cupra/elements/generic_capability.py
-weconnect/api/cupra/elements/generic_settings.py
-weconnect/api/cupra/elements/odometer_measurement.py
-weconnect/api/cupra/elements/parking_position.py
-weconnect/api/cupra/elements/vehicle.py
-weconnect/api/cupra/elements/helpers/__init__.py
-weconnect/api/cupra/elements/helpers/request_tracker.py
-weconnect/api/vw/__init__.py
-weconnect/api/vw/api.py
-weconnect/api/vw/domain.py
-weconnect/api/vw/auth/__init__.py
-weconnect/api/vw/auth/we_charge_session.py
-weconnect/api/vw/auth/we_connect_session.py
-weconnect/api/vw/badges/charging.png
-weconnect/api/vw/badges/connected.png
-weconnect/api/vw/badges/cooling.png
-weconnect/api/vw/badges/heating.png
-weconnect/api/vw/badges/locked.png
-weconnect/api/vw/badges/parking.png
-weconnect/api/vw/badges/unlocked.png
-weconnect/api/vw/badges/ventilating.png
-weconnect/api/vw/badges/warning.png
-weconnect/api/vw/elements/__init__.py
-weconnect/api/vw/elements/access_status.py
-weconnect/api/vw/elements/battery_status.py
-weconnect/api/vw/elements/capability_status.py
-weconnect/api/vw/elements/charge_mode.py
-weconnect/api/vw/elements/charging_profiles.py
-weconnect/api/vw/elements/charging_settings.py
-weconnect/api/vw/elements/charging_station.py
-weconnect/api/vw/elements/charging_status.py
-weconnect/api/vw/elements/climatization_settings.py
-weconnect/api/vw/elements/climatization_status.py
-weconnect/api/vw/elements/climatization_timer.py
-weconnect/api/vw/elements/controls.py
-weconnect/api/vw/elements/enums.py
-weconnect/api/vw/elements/generic_capability.py
-weconnect/api/vw/elements/generic_request_status.py
-weconnect/api/vw/elements/generic_settings.py
-weconnect/api/vw/elements/lights_status.py
-weconnect/api/vw/elements/lv_battery_status.py
-weconnect/api/vw/elements/maintenance_status.py
-weconnect/api/vw/elements/odometer_measurement.py
-weconnect/api/vw/elements/parking_position.py
-weconnect/api/vw/elements/range_measurements.py
-weconnect/api/vw/elements/range_status.py
-weconnect/api/vw/elements/readiness_status.py
-weconnect/api/vw/elements/timer.py
-weconnect/api/vw/elements/vehicle.py
-weconnect/api/vw/elements/warning_lights_status.py
-weconnect/api/vw/elements/helpers/__init__.py
-weconnect/api/vw/elements/helpers/request_tracker.py
-weconnect/auth/__init__.py
-weconnect/auth/auth_util.py
-weconnect/auth/openid_session.py
-weconnect/auth/session_manager.py
-weconnect/auth/vw_web_session.py
-weconnect/elements/__init__.py
-weconnect/elements/access_control_state.py
-weconnect/elements/control_operation.py
-weconnect/elements/error.py
-weconnect/elements/generic_status.py
-weconnect/elements/plug_status.py
-weconnect/elements/window_heating_status.py
+weconnect_cupra/__init__.py
+weconnect_cupra/__version.py
+weconnect_cupra/addressable.py
+weconnect_cupra/errors.py
+weconnect_cupra/fetch.py
+weconnect_cupra/service.py
+weconnect_cupra/util.py
+weconnect_cupra/weconnect_cupra.py
+weconnect_cupra/weconnect_errors.py
+weconnect_cupra/api/__init__.py
+weconnect_cupra/api/cupra/__init__.py
+weconnect_cupra/api/cupra/api.py
+weconnect_cupra/api/cupra/domain.py
+weconnect_cupra/api/cupra/auth/__init__.py
+weconnect_cupra/api/cupra/auth/my_cupra_session.py
+weconnect_cupra/api/cupra/elements/__init__.py
+weconnect_cupra/api/cupra/elements/access_status.py
+weconnect_cupra/api/cupra/elements/battery_status.py
+weconnect_cupra/api/cupra/elements/charging_settings.py
+weconnect_cupra/api/cupra/elements/charging_station.py
+weconnect_cupra/api/cupra/elements/charging_status.py
+weconnect_cupra/api/cupra/elements/climatization_settings.py
+weconnect_cupra/api/cupra/elements/climatization_status.py
+weconnect_cupra/api/cupra/elements/controls.py
+weconnect_cupra/api/cupra/elements/engine_state.py
+weconnect_cupra/api/cupra/elements/enums.py
+weconnect_cupra/api/cupra/elements/error.py
+weconnect_cupra/api/cupra/elements/generic_capability.py
+weconnect_cupra/api/cupra/elements/generic_settings.py
+weconnect_cupra/api/cupra/elements/odometer_measurement.py
+weconnect_cupra/api/cupra/elements/parking_position.py
+weconnect_cupra/api/cupra/elements/vehicle.py
+weconnect_cupra/api/cupra/elements/helpers/__init__.py
+weconnect_cupra/api/cupra/elements/helpers/request_tracker.py
+weconnect_cupra/api/vw/__init__.py
+weconnect_cupra/api/vw/api.py
+weconnect_cupra/api/vw/domain.py
+weconnect_cupra/api/vw/auth/__init__.py
+weconnect_cupra/api/vw/auth/we_charge_session.py
+weconnect_cupra/api/vw/auth/we_connect_session.py
+weconnect_cupra/api/vw/elements/__init__.py
+weconnect_cupra/api/vw/elements/access_status.py
+weconnect_cupra/api/vw/elements/battery_status.py
+weconnect_cupra/api/vw/elements/capability_status.py
+weconnect_cupra/api/vw/elements/charge_mode.py
+weconnect_cupra/api/vw/elements/charging_profiles.py
+weconnect_cupra/api/vw/elements/charging_settings.py
+weconnect_cupra/api/vw/elements/charging_station.py
+weconnect_cupra/api/vw/elements/charging_status.py
+weconnect_cupra/api/vw/elements/climatization_settings.py
+weconnect_cupra/api/vw/elements/climatization_status.py
+weconnect_cupra/api/vw/elements/climatization_timer.py
+weconnect_cupra/api/vw/elements/controls.py
+weconnect_cupra/api/vw/elements/enums.py
+weconnect_cupra/api/vw/elements/generic_capability.py
+weconnect_cupra/api/vw/elements/generic_request_status.py
+weconnect_cupra/api/vw/elements/generic_settings.py
+weconnect_cupra/api/vw/elements/lights_status.py
+weconnect_cupra/api/vw/elements/lv_battery_status.py
+weconnect_cupra/api/vw/elements/maintenance_status.py
+weconnect_cupra/api/vw/elements/odometer_measurement.py
+weconnect_cupra/api/vw/elements/parking_position.py
+weconnect_cupra/api/vw/elements/range_measurements.py
+weconnect_cupra/api/vw/elements/range_status.py
+weconnect_cupra/api/vw/elements/readiness_status.py
+weconnect_cupra/api/vw/elements/timer.py
+weconnect_cupra/api/vw/elements/vehicle.py
+weconnect_cupra/api/vw/elements/warning_lights_status.py
+weconnect_cupra/api/vw/elements/helpers/__init__.py
+weconnect_cupra/api/vw/elements/helpers/request_tracker.py
+weconnect_cupra/auth/__init__.py
+weconnect_cupra/auth/auth_util.py
+weconnect_cupra/auth/openid_session.py
+weconnect_cupra/auth/session_manager.py
+weconnect_cupra/auth/vw_web_session.py
+weconnect_cupra/elements/__init__.py
+weconnect_cupra/elements/access_control_state.py
+weconnect_cupra/elements/control_operation.py
+weconnect_cupra/elements/error.py
+weconnect_cupra/elements/generic_status.py
+weconnect_cupra/elements/plug_status.py
+weconnect_cupra/elements/window_heating_status.py
 weconnect_cupra_daern.egg-info/PKG-INFO
 weconnect_cupra_daern.egg-info/SOURCES.txt
 weconnect_cupra_daern.egg-info/dependency_links.txt
 weconnect_cupra_daern.egg-info/not-zip-safe
 weconnect_cupra_daern.egg-info/requires.txt
 weconnect_cupra_daern.egg-info/top_level.txt
```

