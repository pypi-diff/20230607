# Comparing `tmp/frequenz-api-microgrid-0.15.0.tar.gz` & `tmp/frequenz-api-microgrid-0.15.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frequenz-api-microgrid-0.15.0.tar", last modified: Tue Jun  6 12:05:44 2023, max compression
+gzip compressed data, was "frequenz-api-microgrid-0.15.1.tar", last modified: Wed Jun  7 11:21:02 2023, max compression
```

## Comparing `frequenz-api-microgrid-0.15.0.tar` & `frequenz-api-microgrid-0.15.1.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 12:05:44.713110 frequenz-api-microgrid-0.15.0/
--rw-r--r--   0 runner    (1001) docker     (122)     3141 2023-06-06 12:05:23.000000 frequenz-api-microgrid-0.15.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)     1090 2023-06-06 12:05:23.000000 frequenz-api-microgrid-0.15.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      264 2023-06-06 12:05:23.000000 frequenz-api-microgrid-0.15.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1523 2023-06-06 12:05:44.713110 frequenz-api-microgrid-0.15.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      513 2023-06-06 12:05:23.000000 frequenz-api-microgrid-0.15.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-06-06 12:05:23.000000 frequenz-api-microgrid-0.15.0/RELEASE_NOTES.md
--rw-r--r--   0 runner    (1001) docker     (122)       29 2023-06-06 12:05:23.000000 frequenz-api-microgrid-0.15.0/minimum-requirements-ci.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 12:05:44.673110 frequenz-api-microgrid-0.15.0/proto/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 12:05:44.673110 frequenz-api-microgrid-0.15.0/proto/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 12:05:44.673110 frequenz-api-microgrid-0.15.0/proto/frequenz/api/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 12:05:44.693110 frequenz-api-microgrid-0.15.0/proto/frequenz/api/microgrid/
--rw-r--r--   0 runner    (1001) docker     (122)     5438 2023-06-06 12:05:23.000000 frequenz-api-microgrid-0.15.0/proto/frequenz/api/microgrid/battery.proto
--rw-r--r--   0 runner    (1001) docker     (122)      577 2023-06-06 12:05:23.000000 frequenz-api-microgrid-0.15.0/proto/frequenz/api/microgrid/common.proto
--rw-r--r--   0 runner    (1001) docker     (122)     5584 2023-06-06 12:05:23.000000 frequenz-api-microgrid-0.15.0/proto/frequenz/api/microgrid/ev_charger.proto
--rw-r--r--   0 runner    (1001) docker     (122)      775 2023-06-06 12:05:23.000000 frequenz-api-microgrid-0.15.0/proto/frequenz/api/microgrid/grid.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3352 2023-06-06 12:05:23.000000 frequenz-api-microgrid-0.15.0/proto/frequenz/api/microgrid/inverter.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1876 2023-06-06 12:05:23.000000 frequenz-api-microgrid-0.15.0/proto/frequenz/api/microgrid/meter.proto
--rw-r--r--   0 runner    (1001) docker     (122)    17754 2023-06-06 12:05:23.000000 frequenz-api-microgrid-0.15.0/proto/frequenz/api/microgrid/microgrid.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2669 2023-06-06 12:05:23.000000 frequenz-api-microgrid-0.15.0/proto/frequenz/api/microgrid/sensor.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 12:05:44.677111 frequenz-api-microgrid-0.15.0/py/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 12:05:44.677111 frequenz-api-microgrid-0.15.0/py/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 12:05:44.677111 frequenz-api-microgrid-0.15.0/py/frequenz/api/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 12:05:44.693110 frequenz-api-microgrid-0.15.0/py/frequenz/api/microgrid/
--rw-r--r--   0 runner    (1001) docker     (122)      121 2023-06-06 12:05:23.000000 frequenz-api-microgrid-0.15.0/py/frequenz/api/microgrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-06 12:05:23.000000 frequenz-api-microgrid-0.15.0/py/frequenz/api/microgrid/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 12:05:44.697110 frequenz-api-microgrid-0.15.0/py/frequenz_api_microgrid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1523 2023-06-06 12:05:44.000000 frequenz-api-microgrid-0.15.0/py/frequenz_api_microgrid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4144 2023-06-06 12:05:44.000000 frequenz-api-microgrid-0.15.0/py/frequenz_api_microgrid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-06 12:05:44.000000 frequenz-api-microgrid-0.15.0/py/frequenz_api_microgrid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-06-06 12:05:44.000000 frequenz-api-microgrid-0.15.0/py/frequenz_api_microgrid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-06 12:05:44.000000 frequenz-api-microgrid-0.15.0/py/frequenz_api_microgrid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1530 2023-06-06 12:05:23.000000 frequenz-api-microgrid-0.15.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-06 12:05:44.713110 frequenz-api-microgrid-0.15.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2220 2023-06-06 12:05:23.000000 frequenz-api-microgrid-0.15.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 12:05:44.681110 frequenz-api-microgrid-0.15.0/submodules/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 12:05:44.677111 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 12:05:44.681110 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 12:05:44.705110 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/
--rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/annotations.proto
--rw-r--r--   0 runner    (1001) docker     (122)     7374 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/auth.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1808 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/backend.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2504 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/billing.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3392 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/client.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3169 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/config_change.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2719 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/consumer.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2008 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/context.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1225 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/control.proto
--rw-r--r--   0 runner    (1001) docker     (122)     8657 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/distribution.proto
--rw-r--r--   0 runner    (1001) docker     (122)     6132 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/documentation.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2824 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/endpoint.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3318 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/field_behavior.proto
--rw-r--r--   0 runner    (1001) docker     (122)    12099 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/http.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2605 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/httpbody.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1391 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/label.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2910 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/launch_stage.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2045 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/log.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3209 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/logging.proto
--rw-r--r--   0 runner    (1001) docker     (122)     6628 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/metric.proto
--rw-r--r--   0 runner    (1001) docker     (122)     5512 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/monitored_resource.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3524 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/monitoring.proto
--rw-r--r--   0 runner    (1001) docker     (122)    10854 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/quota.proto
--rw-r--r--   0 runner    (1001) docker     (122)    11347 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/resource.proto
--rw-r--r--   0 runner    (1001) docker     (122)    14929 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/routing.proto
--rw-r--r--   0 runner    (1001) docker     (122)     6099 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/service.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1093 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/source_info.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3472 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/system_parameter.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3513 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/usage.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 12:05:44.705110 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/cloud/
--rw-r--r--   0 runner    (1001) docker     (122)     6308 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/cloud/extended_operations.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 12:05:44.681110 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/iam/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 12:05:44.681110 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/iam/admin/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 12:05:44.705110 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/iam/admin/v1/
--rw-r--r--   0 runner    (1001) docker     (122)    41483 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/iam/admin/v1/iam.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 12:05:44.705110 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/iam/v1/
--rw-r--r--   0 runner    (1001) docker     (122)     5482 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/iam/v1/iam_policy.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 12:05:44.705110 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/iam/v1/logging/
--rw-r--r--   0 runner    (1001) docker     (122)     1287 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/iam/v1/options.proto
--rw-r--r--   0 runner    (1001) docker     (122)     8659 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/iam/v1/policy.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 12:05:44.681110 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/logging/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 12:05:44.705110 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/logging/type/
--rw-r--r--   0 runner    (1001) docker     (122)     3389 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/logging/type/http_request.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2508 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/logging/type/log_severity.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 12:05:44.705110 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/longrunning/
--rw-r--r--   0 runner    (1001) docker     (122)    10515 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/longrunning/operations.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 12:05:44.709110 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/rpc/
--rw-r--r--   0 runner    (1001) docker     (122)     7125 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/rpc/code.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 12:05:44.709110 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/rpc/context/
--rw-r--r--   0 runner    (1001) docker     (122)    12015 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/rpc/context/attribute_context.proto
--rw-r--r--   0 runner    (1001) docker     (122)     9504 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/rpc/error_details.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1924 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/rpc/status.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 12:05:44.709110 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/type/
--rw-r--r--   0 runner    (1001) docker     (122)     1766 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/type/calendar_period.proto
--rw-r--r--   0 runner    (1001) docker     (122)     6193 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/type/color.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/type/date.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3508 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/type/datetime.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/type/dayofweek.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1834 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/type/expr.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1176 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/type/fraction.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1447 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/type/latlng.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1603 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/type/money.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1482 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/type/month.proto
--rw-r--r--   0 runner    (1001) docker     (122)     6239 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/type/postal_address.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3795 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/type/quaternion.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1668 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/type/timeofday.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 12:05:44.685110 frequenz-api-microgrid-0.15.0/submodules/frequenz-api-common/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 12:05:44.685110 frequenz-api-microgrid-0.15.0/submodules/frequenz-api-common/proto/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 12:05:44.685110 frequenz-api-microgrid-0.15.0/submodules/frequenz-api-common/proto/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 12:05:44.685110 frequenz-api-microgrid-0.15.0/submodules/frequenz-api-common/proto/frequenz/api/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 12:05:44.709110 frequenz-api-microgrid-0.15.0/submodules/frequenz-api-common/proto/frequenz/api/common/
--rw-r--r--   0 runner    (1001) docker     (122)     2864 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/frequenz-api-common/proto/frequenz/api/common/components.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 12:05:44.713110 frequenz-api-microgrid-0.15.0/submodules/frequenz-api-common/proto/frequenz/api/common/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)     6145 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/frequenz-api-common/proto/frequenz/api/common/metrics/electrical.proto
--rw-r--r--   0 runner    (1001) docker     (122)     7405 2023-06-06 12:05:24.000000 frequenz-api-microgrid-0.15.0/submodules/frequenz-api-common/proto/frequenz/api/common/metrics.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:21:02.641787 frequenz-api-microgrid-0.15.1/
+-rw-r--r--   0 runner    (1001) docker     (122)     3141 2023-06-07 11:20:44.000000 frequenz-api-microgrid-0.15.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1090 2023-06-07 11:20:44.000000 frequenz-api-microgrid-0.15.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      264 2023-06-07 11:20:44.000000 frequenz-api-microgrid-0.15.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1523 2023-06-07 11:21:02.641787 frequenz-api-microgrid-0.15.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      513 2023-06-07 11:20:44.000000 frequenz-api-microgrid-0.15.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      617 2023-06-07 11:20:44.000000 frequenz-api-microgrid-0.15.1/RELEASE_NOTES.md
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-06-07 11:20:44.000000 frequenz-api-microgrid-0.15.1/minimum-requirements-ci.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:21:02.629787 frequenz-api-microgrid-0.15.1/proto/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:21:02.629787 frequenz-api-microgrid-0.15.1/proto/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:21:02.629787 frequenz-api-microgrid-0.15.1/proto/frequenz/api/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:21:02.633787 frequenz-api-microgrid-0.15.1/proto/frequenz/api/microgrid/
+-rw-r--r--   0 runner    (1001) docker     (122)     5438 2023-06-07 11:20:44.000000 frequenz-api-microgrid-0.15.1/proto/frequenz/api/microgrid/battery.proto
+-rw-r--r--   0 runner    (1001) docker     (122)      577 2023-06-07 11:20:44.000000 frequenz-api-microgrid-0.15.1/proto/frequenz/api/microgrid/common.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     5584 2023-06-07 11:20:44.000000 frequenz-api-microgrid-0.15.1/proto/frequenz/api/microgrid/ev_charger.proto
+-rw-r--r--   0 runner    (1001) docker     (122)      775 2023-06-07 11:20:44.000000 frequenz-api-microgrid-0.15.1/proto/frequenz/api/microgrid/grid.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3352 2023-06-07 11:20:44.000000 frequenz-api-microgrid-0.15.1/proto/frequenz/api/microgrid/inverter.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1876 2023-06-07 11:20:44.000000 frequenz-api-microgrid-0.15.1/proto/frequenz/api/microgrid/meter.proto
+-rw-r--r--   0 runner    (1001) docker     (122)    17755 2023-06-07 11:20:44.000000 frequenz-api-microgrid-0.15.1/proto/frequenz/api/microgrid/microgrid.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2669 2023-06-07 11:20:44.000000 frequenz-api-microgrid-0.15.1/proto/frequenz/api/microgrid/sensor.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:21:02.629787 frequenz-api-microgrid-0.15.1/py/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:21:02.629787 frequenz-api-microgrid-0.15.1/py/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:21:02.629787 frequenz-api-microgrid-0.15.1/py/frequenz/api/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:21:02.633787 frequenz-api-microgrid-0.15.1/py/frequenz/api/microgrid/
+-rw-r--r--   0 runner    (1001) docker     (122)      121 2023-06-07 11:20:44.000000 frequenz-api-microgrid-0.15.1/py/frequenz/api/microgrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 11:20:44.000000 frequenz-api-microgrid-0.15.1/py/frequenz/api/microgrid/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:21:02.633787 frequenz-api-microgrid-0.15.1/py/frequenz_api_microgrid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1523 2023-06-07 11:21:02.000000 frequenz-api-microgrid-0.15.1/py/frequenz_api_microgrid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4144 2023-06-07 11:21:02.000000 frequenz-api-microgrid-0.15.1/py/frequenz_api_microgrid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-07 11:21:02.000000 frequenz-api-microgrid-0.15.1/py/frequenz_api_microgrid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-06-07 11:21:02.000000 frequenz-api-microgrid-0.15.1/py/frequenz_api_microgrid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-07 11:21:02.000000 frequenz-api-microgrid-0.15.1/py/frequenz_api_microgrid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1530 2023-06-07 11:20:44.000000 frequenz-api-microgrid-0.15.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-07 11:21:02.641787 frequenz-api-microgrid-0.15.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2220 2023-06-07 11:20:44.000000 frequenz-api-microgrid-0.15.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:21:02.629787 frequenz-api-microgrid-0.15.1/submodules/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:21:02.629787 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:21:02.629787 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:21:02.637787 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/annotations.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     7374 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/auth.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1808 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/backend.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2504 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/billing.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3392 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/client.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3169 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/config_change.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2719 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/consumer.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2008 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/context.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1225 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/control.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     8657 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/distribution.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     6132 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/documentation.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2824 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/endpoint.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3318 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/field_behavior.proto
+-rw-r--r--   0 runner    (1001) docker     (122)    12099 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/http.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2605 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/httpbody.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1391 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/label.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2910 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/launch_stage.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2045 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/log.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3209 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/logging.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     6628 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/metric.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     5512 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/monitored_resource.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3524 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/monitoring.proto
+-rw-r--r--   0 runner    (1001) docker     (122)    10854 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/quota.proto
+-rw-r--r--   0 runner    (1001) docker     (122)    11347 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/resource.proto
+-rw-r--r--   0 runner    (1001) docker     (122)    14929 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/routing.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     6099 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/service.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1093 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/source_info.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3472 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/system_parameter.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3513 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/usage.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:21:02.637787 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/cloud/
+-rw-r--r--   0 runner    (1001) docker     (122)     6308 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/cloud/extended_operations.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:21:02.629787 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/iam/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:21:02.629787 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/iam/admin/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:21:02.637787 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/iam/admin/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)    41483 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/iam/admin/v1/iam.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:21:02.637787 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/iam/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)     5482 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/iam/v1/iam_policy.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:21:02.637787 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/iam/v1/logging/
+-rw-r--r--   0 runner    (1001) docker     (122)     1287 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/iam/v1/options.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     8659 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/iam/v1/policy.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:21:02.629787 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/logging/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:21:02.637787 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/logging/type/
+-rw-r--r--   0 runner    (1001) docker     (122)     3389 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/logging/type/http_request.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2508 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/logging/type/log_severity.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:21:02.637787 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/longrunning/
+-rw-r--r--   0 runner    (1001) docker     (122)    10515 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/longrunning/operations.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:21:02.637787 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/rpc/
+-rw-r--r--   0 runner    (1001) docker     (122)     7125 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/rpc/code.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:21:02.637787 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/rpc/context/
+-rw-r--r--   0 runner    (1001) docker     (122)    12015 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/rpc/context/attribute_context.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     9504 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/rpc/error_details.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1924 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/rpc/status.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:21:02.641787 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/type/
+-rw-r--r--   0 runner    (1001) docker     (122)     1766 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/type/calendar_period.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     6193 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/type/color.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/type/date.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3508 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/type/datetime.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/type/dayofweek.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1834 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/type/expr.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1176 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/type/fraction.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1447 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/type/latlng.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1603 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/type/money.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1482 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/type/month.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     6239 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/type/postal_address.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3795 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/type/quaternion.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1668 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/type/timeofday.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:21:02.629787 frequenz-api-microgrid-0.15.1/submodules/frequenz-api-common/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:21:02.629787 frequenz-api-microgrid-0.15.1/submodules/frequenz-api-common/proto/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:21:02.629787 frequenz-api-microgrid-0.15.1/submodules/frequenz-api-common/proto/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:21:02.629787 frequenz-api-microgrid-0.15.1/submodules/frequenz-api-common/proto/frequenz/api/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:21:02.641787 frequenz-api-microgrid-0.15.1/submodules/frequenz-api-common/proto/frequenz/api/common/
+-rw-r--r--   0 runner    (1001) docker     (122)     2864 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/frequenz-api-common/proto/frequenz/api/common/components.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 11:21:02.641787 frequenz-api-microgrid-0.15.1/submodules/frequenz-api-common/proto/frequenz/api/common/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)     6145 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/frequenz-api-common/proto/frequenz/api/common/metrics/electrical.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     7405 2023-06-07 11:20:45.000000 frequenz-api-microgrid-0.15.1/submodules/frequenz-api-common/proto/frequenz/api/common/metrics.proto
```

### Comparing `frequenz-api-microgrid-0.15.0/CONTRIBUTING.md` & `frequenz-api-microgrid-0.15.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/LICENSE` & `frequenz-api-microgrid-0.15.1/LICENSE`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/PKG-INFO` & `frequenz-api-microgrid-0.15.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-api-microgrid
-Version: 0.15.0
+Version: 0.15.1
 Summary: Frequenz gRPC API for monitoring and control of microgrids
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-api-microgrid/releases
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-api-microgrid
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-api-microgrid/issues
 Project-URL: Support, https://github.com/frequenz-floss/frequenz-api-microgrid/discussions/categories/support
```

### Comparing `frequenz-api-microgrid-0.15.0/README.md` & `frequenz-api-microgrid-0.15.1/README.md`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/proto/frequenz/api/microgrid/battery.proto` & `frequenz-api-microgrid-0.15.1/proto/frequenz/api/microgrid/battery.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/proto/frequenz/api/microgrid/common.proto` & `frequenz-api-microgrid-0.15.1/proto/frequenz/api/microgrid/common.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/proto/frequenz/api/microgrid/ev_charger.proto` & `frequenz-api-microgrid-0.15.1/proto/frequenz/api/microgrid/ev_charger.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/proto/frequenz/api/microgrid/grid.proto` & `frequenz-api-microgrid-0.15.1/proto/frequenz/api/microgrid/grid.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/proto/frequenz/api/microgrid/inverter.proto` & `frequenz-api-microgrid-0.15.1/proto/frequenz/api/microgrid/inverter.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/proto/frequenz/api/microgrid/meter.proto` & `frequenz-api-microgrid-0.15.1/proto/frequenz/api/microgrid/meter.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/proto/frequenz/api/microgrid/microgrid.proto` & `frequenz-api-microgrid-0.15.1/proto/frequenz/api/microgrid/microgrid.proto`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 service Microgrid {
   /// Returns the microgrid metadata
   /// The metadata consists of information that describes the overall
   /// microgrid, as opposed to its components,
   /// e.g., the microgrid ID, location.
   rpc GetMicrogridMetadata(google.protobuf.Empty) returns (MicrogridMetadata) {
     option (google.api.http) = {
-      get : "v1/metadata"
+      get : "/v1/metadata"
     };
   }
 
   // List components in the local microgrid, optionally filtered by a given list
   // of component IDs and component categories.
   //
   // If provided, the filters for component IDs and categories have an `AND`
```

### Comparing `frequenz-api-microgrid-0.15.0/proto/frequenz/api/microgrid/sensor.proto` & `frequenz-api-microgrid-0.15.1/proto/frequenz/api/microgrid/sensor.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/py/frequenz_api_microgrid.egg-info/PKG-INFO` & `frequenz-api-microgrid-0.15.1/py/frequenz_api_microgrid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-api-microgrid
-Version: 0.15.0
+Version: 0.15.1
 Summary: Frequenz gRPC API for monitoring and control of microgrids
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-api-microgrid/releases
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-api-microgrid
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-api-microgrid/issues
 Project-URL: Support, https://github.com/frequenz-floss/frequenz-api-microgrid/discussions/categories/support
```

### Comparing `frequenz-api-microgrid-0.15.0/py/frequenz_api_microgrid.egg-info/SOURCES.txt` & `frequenz-api-microgrid-0.15.1/py/frequenz_api_microgrid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/pyproject.toml` & `frequenz-api-microgrid-0.15.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
    "License :: OSI Approved :: MIT License",
    "Programming Language :: Python :: 3",
    "Programming Language :: Python :: 3 :: Only",
    "Topic :: Software Development :: Libraries",
 ]
 requires-python = ">= 3.11, < 4"
 dependencies = [
-    "frequenz-api-common == 0.2.0",
+    "frequenz-api-common == 0.3.0",
     "googleapis-common-protos >= 1.56.2, < 2",
     "grpcio >= 1.47.0, < 2",
 ]
 dynamic = [ "version" ]
 
 [[project.authors]]
 name ="Frequenz Energy-as-a-Service GmbH"
```

### Comparing `frequenz-api-microgrid-0.15.0/setup.py` & `frequenz-api-microgrid-0.15.1/setup.py`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/annotations.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/annotations.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/auth.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/auth.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/backend.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/backend.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/billing.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/billing.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/client.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/client.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/config_change.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/config_change.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/consumer.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/consumer.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/context.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/context.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/control.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/control.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/distribution.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/distribution.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/documentation.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/documentation.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/endpoint.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/endpoint.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/field_behavior.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/field_behavior.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/http.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/http.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/httpbody.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/httpbody.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/label.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/label.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/launch_stage.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/launch_stage.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/log.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/log.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/logging.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/logging.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/metric.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/metric.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/monitored_resource.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/monitored_resource.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/monitoring.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/monitoring.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/quota.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/quota.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/resource.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/resource.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/routing.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/routing.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/service.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/service.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/source_info.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/source_info.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/system_parameter.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/system_parameter.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/api/usage.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/api/usage.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/cloud/extended_operations.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/cloud/extended_operations.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/iam/admin/v1/iam.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/iam/admin/v1/iam.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/iam/v1/iam_policy.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/iam/v1/iam_policy.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/iam/v1/options.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/iam/v1/options.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/iam/v1/policy.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/iam/v1/policy.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/logging/type/http_request.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/logging/type/http_request.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/logging/type/log_severity.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/logging/type/log_severity.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/longrunning/operations.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/longrunning/operations.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/rpc/code.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/rpc/code.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/rpc/context/attribute_context.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/rpc/context/attribute_context.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/rpc/error_details.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/rpc/error_details.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/rpc/status.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/rpc/status.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/type/calendar_period.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/type/calendar_period.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/type/color.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/type/color.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/type/date.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/type/date.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/type/datetime.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/type/datetime.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/type/dayofweek.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/type/dayofweek.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/type/expr.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/type/expr.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/type/fraction.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/type/fraction.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/type/latlng.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/type/latlng.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/type/money.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/type/money.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/type/month.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/type/month.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/type/postal_address.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/type/postal_address.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/type/quaternion.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/type/quaternion.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/api-common-protos/google/type/timeofday.proto` & `frequenz-api-microgrid-0.15.1/submodules/api-common-protos/google/type/timeofday.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/frequenz-api-common/proto/frequenz/api/common/components.proto` & `frequenz-api-microgrid-0.15.1/submodules/frequenz-api-common/proto/frequenz/api/common/components.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/frequenz-api-common/proto/frequenz/api/common/metrics/electrical.proto` & `frequenz-api-microgrid-0.15.1/submodules/frequenz-api-common/proto/frequenz/api/common/metrics/electrical.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-microgrid-0.15.0/submodules/frequenz-api-common/proto/frequenz/api/common/metrics.proto` & `frequenz-api-microgrid-0.15.1/submodules/frequenz-api-common/proto/frequenz/api/common/metrics.proto`

 * *Files identical despite different names*

