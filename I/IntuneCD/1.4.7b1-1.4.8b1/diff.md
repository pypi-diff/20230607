# Comparing `tmp/IntuneCD-1.4.7b1.tar.gz` & `tmp/IntuneCD-1.4.8b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IntuneCD-1.4.7b1.tar", last modified: Sat May 27 12:22:39 2023, max compression
+gzip compressed data, was "IntuneCD-1.4.8b1.tar", last modified: Wed Jun  7 14:15:04 2023, max compression
```

## Comparing `IntuneCD-1.4.7b1.tar` & `IntuneCD-1.4.8b1.tar`

### file list

```diff
@@ -1,96 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:22:39.003552 IntuneCD-1.4.7b1/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-05-27 12:22:39.003552 IntuneCD-1.4.7b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-27 12:22:39.003552 IntuneCD-1.4.7b1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:22:38.995552 IntuneCD-1.4.7b1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:22:39.003552 IntuneCD-1.4.7b1/src/IntuneCD/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/assignment_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_AppProtection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_apns.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_appConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_appleEnrollmentProfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_applications.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_assignmentFilters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_autopilotDevices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_compliance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_compliancePartner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_conditionalAccess.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_configurationPolicies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_customAttributeShellScript.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_deviceManagementSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_enrollmentConfigurations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_enrollmentStatusPage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_groupPolicyConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_managedGPlay.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_managementIntents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_managementPartner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_notificationTemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_powershellScripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_proactiveRemediation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_remoteAssistancePartner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_shellScripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_vppTokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/backup_windowsEnrollmentProfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/check_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/clean_filename.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/diff_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    17705 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/documentation_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/get_accesstoken.py
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/get_authparams.py
--rw-r--r--   0 runner    (1001) docker     (123)    10342 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/graph_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/graph_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/load_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/remove_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)    12362 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/run_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)    12987 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/run_documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11471 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/run_update.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/save_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_appConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_appProtection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_appleEnrollmentProfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     7443 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_assignmentFilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_compliance.py
--rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_conditionalAccess.py
--rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_configurationPolicies.py
--rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_customAttributeShellScript.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_deviceManagementSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)    11648 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_enrollmentConfigurations.py
--rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_enrollmentStatusPage.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)    24286 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_groupPolicyConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9069 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_managementIntents.py
--rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_notificationTemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_powershellScripts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_proactiveRemediation.py
--rw-r--r--   0 runner    (1001) docker     (123)    16118 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     8385 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_shellScripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/src/IntuneCD/update_windowsEnrollmentProfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:22:39.003552 IntuneCD-1.4.7b1/src/IntuneCD.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-05-27 12:22:38.000000 IntuneCD-1.4.7b1/src/IntuneCD.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-05-27 12:22:38.000000 IntuneCD-1.4.7b1/src/IntuneCD.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 12:22:38.000000 IntuneCD-1.4.7b1/src/IntuneCD.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-27 12:22:38.000000 IntuneCD-1.4.7b1/src/IntuneCD.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-27 12:22:38.000000 IntuneCD-1.4.7b1/src/IntuneCD.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-27 12:22:38.000000 IntuneCD-1.4.7b1/src/IntuneCD.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:22:39.003552 IntuneCD-1.4.7b1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/tests/test_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/tests/test_check_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/tests/test_clean_filename.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/tests/test_diff_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/tests/test_documentation_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/tests/test_get_added_removed.py
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/tests/test_get_authparams.py
--rw-r--r--   0 runner    (1001) docker     (123)    12241 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/tests/test_graph_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    17428 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/tests/test_graph_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/tests/test_group_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/tests/test_load_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/tests/test_match.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/tests/test_remove_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/tests/test_save_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-27 12:22:25.000000 IntuneCD-1.4.7b1/tests/test_update_frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:15:04.657343 IntuneCD-1.4.8b1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-06-07 14:15:04.657343 IntuneCD-1.4.8b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-07 14:15:04.657343 IntuneCD-1.4.8b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:15:04.645342 IntuneCD-1.4.8b1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:15:04.653342 IntuneCD-1.4.8b1/src/IntuneCD/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/assignment_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_AppProtection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_apns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_appConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_appleEnrollmentProfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_assignmentFilters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_autopilotDevices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_compliance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_compliancePartner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_conditionalAccess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_configurationPolicies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_customAttributeShellScript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_deviceCategories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_deviceManagementSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_enrollmentConfigurations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_enrollmentStatusPage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_groupPolicyConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_managedGPlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_managementIntents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_managementPartner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_notificationTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_powershellScripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_proactiveRemediation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_remoteAssistancePartner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_shellScripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_vppTokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_windowsEnrollmentProfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/check_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/clean_filename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/diff_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17705 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/documentation_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/get_accesstoken.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/get_authparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10342 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/graph_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/graph_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/load_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/remove_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12500 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/run_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13245 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/run_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11212 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/run_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/save_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/update_appConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/update_appProtection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/update_appleEnrollmentProfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7443 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/update_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/update_assignmentFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/update_compliance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/update_conditionalAccess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/update_configurationPolicies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/update_customAttributeShellScript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/update_deviceCategories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/update_deviceManagementSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11648 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/update_enrollmentConfigurations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/update_enrollmentStatusPage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/update_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24286 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/update_groupPolicyConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9069 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/update_managementIntents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/update_notificationTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/update_powershellScripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/update_proactiveRemediation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16118 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/update_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8385 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/update_shellScripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/update_windowsEnrollmentProfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:15:04.653342 IntuneCD-1.4.8b1/src/IntuneCD.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-06-07 14:15:04.000000 IntuneCD-1.4.8b1/src/IntuneCD.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-06-07 14:15:04.000000 IntuneCD-1.4.8b1/src/IntuneCD.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 14:15:04.000000 IntuneCD-1.4.8b1/src/IntuneCD.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-07 14:15:04.000000 IntuneCD-1.4.8b1/src/IntuneCD.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-07 14:15:04.000000 IntuneCD-1.4.8b1/src/IntuneCD.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-07 14:15:04.000000 IntuneCD-1.4.8b1/src/IntuneCD.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:15:04.657343 IntuneCD-1.4.8b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/tests/test_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/tests/test_check_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/tests/test_clean_filename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/tests/test_diff_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7432 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/tests/test_documentation_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/tests/test_get_added_removed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/tests/test_get_authparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12241 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/tests/test_graph_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17428 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/tests/test_graph_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/tests/test_group_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/tests/test_load_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/tests/test_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/tests/test_remove_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/tests/test_save_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/tests/test_update_frontend.py
```

### Comparing `IntuneCD-1.4.7b1/LICENSE` & `IntuneCD-1.4.8b1/LICENSE`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/PKG-INFO` & `IntuneCD-1.4.8b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IntuneCD
-Version: 1.4.7b1
+Version: 1.4.8b1
 Summary: Tool to backup and update configurations in Intune
 Home-page: https://github.com/almenscorner/IntuneCD
 Author: Tobias Almén
 Author-email: almenscorner@outlook.com
 Project-URL: Bug Tracker, https://github.com/almenscorner/IntuneCD/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `IntuneCD-1.4.7b1/README.md` & `IntuneCD-1.4.8b1/README.md`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/setup.cfg` & `IntuneCD-1.4.8b1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = IntuneCD
-version = 1.4.7.beta1
+version = 1.4.8.beta1
 author = Tobias Almén
 author_email = almenscorner@outlook.com
 description = Tool to backup and update configurations in Intune
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/almenscorner/IntuneCD
 project_urls =
```

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/archive.py` & `IntuneCD-1.4.8b1/src/IntuneCD/archive.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/assignment_report.py` & `IntuneCD-1.4.8b1/src/IntuneCD/assignment_report.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/backup_AppProtection.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_AppProtection.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/backup_apns.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_apns.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/backup_appConfiguration.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_appConfiguration.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/backup_appleEnrollmentProfile.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_appleEnrollmentProfile.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/backup_applications.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_applications.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/backup_assignmentFilters.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_assignmentFilters.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/backup_autopilotDevices.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_autopilotDevices.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/backup_compliance.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_compliance.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/backup_compliancePartner.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_compliancePartner.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/backup_conditionalAccess.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_conditionalAccess.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/backup_configurationPolicies.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_configurationPolicies.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/backup_customAttributeShellScript.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_customAttributeShellScript.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/backup_deviceManagementSettings.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_deviceManagementSettings.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/backup_enrollmentConfigurations.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_enrollmentConfigurations.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/backup_enrollmentStatusPage.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_enrollmentStatusPage.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/backup_groupPolicyConfiguration.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_groupPolicyConfiguration.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/backup_managedGPlay.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_managedGPlay.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/backup_managementIntents.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_managementIntents.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/backup_managementPartner.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_managementPartner.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/backup_notificationTemplate.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_notificationTemplate.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/backup_powershellScripts.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_powershellScripts.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/backup_proactiveRemediation.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_proactiveRemediation.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/backup_profiles.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_profiles.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/backup_remoteAssistancePartner.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_remoteAssistancePartner.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/backup_shellScripts.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_shellScripts.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/backup_vppTokens.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_vppTokens.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/backup_windowsEnrollmentProfile.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_windowsEnrollmentProfile.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/check_file.py` & `IntuneCD-1.4.8b1/src/IntuneCD/check_file.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/clean_filename.py` & `IntuneCD-1.4.8b1/src/IntuneCD/clean_filename.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/diff_summary.py` & `IntuneCD-1.4.8b1/src/IntuneCD/diff_summary.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/documentation_functions.py` & `IntuneCD-1.4.8b1/src/IntuneCD/documentation_functions.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/get_accesstoken.py` & `IntuneCD-1.4.8b1/src/IntuneCD/get_accesstoken.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/get_authparams.py` & `IntuneCD-1.4.8b1/src/IntuneCD/get_authparams.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/graph_batch.py` & `IntuneCD-1.4.8b1/src/IntuneCD/graph_batch.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/graph_request.py` & `IntuneCD-1.4.8b1/src/IntuneCD/graph_request.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/load_file.py` & `IntuneCD-1.4.8b1/src/IntuneCD/load_file.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/remove_keys.py` & `IntuneCD-1.4.8b1/src/IntuneCD/remove_keys.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/run_backup.py` & `IntuneCD-1.4.8b1/src/IntuneCD/run_backup.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,14 +109,15 @@
             "PowershellScripts",
             "ShellScripts",
             "ConfigurationPolicies",
             "ConditionalAccess",
             "EnrollmentConfigurations",
             "DeviceManagementSettings",
             "CustomAttributes",
+            "DeviceCategories",
         ],
         nargs="+",
     )
     parser.add_argument(
         "-f",
         "--frontend",
         help="Set the frontend URL to update with configuration count and backup stream",
@@ -189,14 +190,19 @@
             results.append(savebackup(path, output, exclude, token))
 
         if "DeviceManagementSettings" not in exclude:
             from .backup_deviceManagementSettings import savebackup
 
             results.append(savebackup(path, output, token))
 
+        if "deviceCategories" not in exclude:
+            from .backup_deviceCategories import savebackup
+
+            results.append(savebackup(path, output, token))
+
         if "NotificationTemplate" not in exclude:
             from .backup_notificationTemplate import savebackup
 
             results.append(savebackup(path, output, token))
 
         if "Profiles" not in exclude:
             from .backup_profiles import savebackup
@@ -354,17 +360,15 @@
                                     "groupType": assignment["groupType"],
                                     "membershipRule": assignment["membershipRule"],
                                     "assignedTo": assignment["assignedTo"],
                                 }
                             )
 
                         if len(body) > 0:
-                            update_frontend(
-                                f"{args.frontend}/api/assignments/summary", body
-                            )
+                            update_frontend(f"{args.frontend}/api/assignments/summary", body)
 
         else:
             run_backup(args.path, args.output, exclude, token)
 
     else:
         print("Please enter a valid output format, json or yaml")
```

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/run_documentation.py` & `IntuneCD-1.4.8b1/src/IntuneCD/run_documentation.py`

 * *Files 1% similar despite different names*

```diff
@@ -314,14 +314,25 @@
             "Enrollment Configurations",
             maxlength,
             split,
             cleanup,
             decode,
         )
 
+        # Document Device Categories
+        document_configs(
+            f"{configpath}/Device Categories",
+            outpath,
+            "Device Categories",
+            maxlength,
+            split,
+            cleanup,
+            decode,
+        )
+
         # Document filters
         document_configs(f"{configpath}/Filters", outpath, "Filters", maxlength, split, cleanup, decode)
 
         # Managed Google Play
         document_configs(
             f"{configpath}/Managed Google Play",
             outpath,
```

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/run_update.py` & `IntuneCD-1.4.8b1/src/IntuneCD/run_update.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,17 +28,15 @@
 from .get_authparams import getAuth
 from .update_frontend import update_frontend
 
 REPO_DIR = os.environ.get("REPO_DIR")
 
 
 def start():
-    parser = argparse.ArgumentParser(
-        description="Update Intune configurations with values from backup"
-    )
+    parser = argparse.ArgumentParser(description="Update Intune configurations with values from backup")
     parser.add_argument(
         "-p",
         "--path",
         help="The path to which the configurations are saved. Default value is $(Build.SourcesDirectory)",
         default=REPO_DIR,
     )
     parser.add_argument(
@@ -105,14 +103,15 @@
             "PowershellScripts",
             "ShellScripts",
             "ConfigurationPolicies",
             "ConditionalAccess",
             "EnrollmentConfigurations",
             "DeviceManagementSettings",
             "CustomAttributes",
+            "DeviceCategories",
         ],
         nargs="+",
     )
     parser.add_argument(
         "-r",
         "--report",
         help="When this parameter is set, no updates are pushed to Intune but the change summary is pushed to the frontend",
@@ -160,133 +159,108 @@
     def run_update(path, token, assignment, exclude, report, create_groups, remove):
         diff_count = 0
         diff_summary = []
 
         if "AppConfigurations" not in exclude:
             from .update_appConfiguration import update
 
-            diff_summary.append(
-                update(path, token, assignment, report, create_groups, remove)
-            )
+            diff_summary.append(update(path, token, assignment, report, create_groups, remove))
 
         if "AppProtection" not in exclude:
             from .update_appProtection import update
 
-            diff_summary.append(
-                update(path, token, assignment, report, create_groups, remove)
-            )
+            diff_summary.append(update(path, token, assignment, report, create_groups, remove))
 
         if "Compliance" not in exclude:
             from .update_compliance import update
 
-            diff_summary.append(
-                update(path, token, assignment, report, create_groups, remove)
-            )
+            diff_summary.append(update(path, token, assignment, report, create_groups, remove))
 
         if "DeviceManagementSettings" not in exclude and args.interactiveauth is True:
             from .update_deviceManagementSettings import update
 
             diff_summary.append(update(path, token, report))
         else:
             print("-" * 90)
-            print(
-                "***Device Management Settings is only available with interactive auth***"
-            )
+            print("***Device Management Settings is only available with interactive auth***")
+
+        if "deviceCategories" not in exclude:
+            from .update_deviceCategories import update
+
+            diff_summary.append(update(path, token, report, remove))
 
         if "NotificationTemplate" not in exclude:
             from .update_notificationTemplate import update
 
             diff_summary.append(update(path, token, report, remove))
 
         if "Profiles" not in exclude:
             from .update_profiles import update
 
-            diff_summary.append(
-                update(path, token, assignment, report, create_groups, remove)
-            )
+            diff_summary.append(update(path, token, assignment, report, create_groups, remove))
 
         if "GPOConfigurations" not in exclude:
             from .update_groupPolicyConfiguration import update
 
-            diff_summary.append(
-                update(path, token, assignment, report, create_groups, remove)
-            )
+            diff_summary.append(update(path, token, assignment, report, create_groups, remove))
 
         if "AppleEnrollmentProfile" not in exclude:
             from .update_appleEnrollmentProfile import update
 
             diff_summary.append(update(path, token, report))
 
         if "WindowsEnrollmentProfile" not in exclude:
             from .update_windowsEnrollmentProfile import update
 
-            diff_summary.append(
-                update(path, token, assignment, report, create_groups, remove)
-            )
+            diff_summary.append(update(path, token, assignment, report, create_groups, remove))
 
         if "EnrollmentStatusPage" not in exclude:
             from .update_enrollmentStatusPage import update
 
-            diff_summary.append(
-                update(path, token, assignment, report, create_groups, remove)
-            )
+            diff_summary.append(update(path, token, assignment, report, create_groups, remove))
 
         if "EnrollmentConfigurations" not in exclude:
             from .update_enrollmentConfigurations import update
 
-            diff_summary.append(
-                update(path, token, assignment, report, create_groups, remove)
-            )
+            diff_summary.append(update(path, token, assignment, report, create_groups, remove))
 
         if "Filters" not in exclude:
             from .update_assignmentFilter import update
 
             diff_summary.append(update(path, token, report))
 
         if "Intents" not in exclude:
             from .update_managementIntents import update
 
-            diff_summary.append(
-                update(path, token, assignment, report, create_groups, remove)
-            )
+            diff_summary.append(update(path, token, assignment, report, create_groups, remove))
 
         if "ProactiveRemediation" not in exclude:
             from .update_proactiveRemediation import update
 
-            diff_summary.append(
-                update(path, token, assignment, report, create_groups, remove)
-            )
+            diff_summary.append(update(path, token, assignment, report, create_groups, remove))
 
         if "PowershellScripts" not in exclude:
             from .update_powershellScripts import update
 
-            diff_summary.append(
-                update(path, token, assignment, report, create_groups, remove)
-            )
+            diff_summary.append(update(path, token, assignment, report, create_groups, remove))
 
         if "ShellScripts" not in exclude:
             from .update_shellScripts import update
 
-            diff_summary.append(
-                update(path, token, assignment, report, create_groups, remove)
-            )
+            diff_summary.append(update(path, token, assignment, report, create_groups, remove))
 
         if "CustomAttribute" not in exclude:
             from .update_customAttributeShellScript import update
 
-            diff_summary.append(
-                update(path, token, assignment, report, create_groups, remove)
-            )
+            diff_summary.append(update(path, token, assignment, report, create_groups, remove))
 
         if "ConfigurationPolicies" not in exclude:
             from .update_configurationPolicies import update
 
-            diff_summary.append(
-                update(path, token, assignment, report, create_groups, remove)
-            )
+            diff_summary.append(update(path, token, assignment, report, create_groups, remove))
 
         if "ConditionalAccess" not in exclude:
             from .update_conditionalAccess import update
 
             diff_count += update(path, token, report, remove)
 
         for sum in diff_summary:
```

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/save_output.py` & `IntuneCD-1.4.8b1/src/IntuneCD/save_output.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/update_appConfiguration.py` & `IntuneCD-1.4.8b1/src/IntuneCD/update_appConfiguration.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/update_appProtection.py` & `IntuneCD-1.4.8b1/src/IntuneCD/update_appProtection.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/update_appleEnrollmentProfile.py` & `IntuneCD-1.4.8b1/src/IntuneCD/update_appleEnrollmentProfile.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/update_assignment.py` & `IntuneCD-1.4.8b1/src/IntuneCD/update_assignment.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/update_assignmentFilter.py` & `IntuneCD-1.4.8b1/src/IntuneCD/update_assignmentFilter.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/update_compliance.py` & `IntuneCD-1.4.8b1/src/IntuneCD/update_compliance.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/update_conditionalAccess.py` & `IntuneCD-1.4.8b1/src/IntuneCD/update_conditionalAccess.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/update_configurationPolicies.py` & `IntuneCD-1.4.8b1/src/IntuneCD/update_configurationPolicies.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/update_customAttributeShellScript.py` & `IntuneCD-1.4.8b1/src/IntuneCD/update_customAttributeShellScript.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/update_deviceManagementSettings.py` & `IntuneCD-1.4.8b1/src/IntuneCD/update_deviceManagementSettings.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/update_enrollmentConfigurations.py` & `IntuneCD-1.4.8b1/src/IntuneCD/update_enrollmentConfigurations.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/update_enrollmentStatusPage.py` & `IntuneCD-1.4.8b1/src/IntuneCD/update_enrollmentStatusPage.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/update_frontend.py` & `IntuneCD-1.4.8b1/src/IntuneCD/update_frontend.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/update_groupPolicyConfiguration.py` & `IntuneCD-1.4.8b1/src/IntuneCD/update_groupPolicyConfiguration.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/update_managementIntents.py` & `IntuneCD-1.4.8b1/src/IntuneCD/update_managementIntents.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/update_notificationTemplate.py` & `IntuneCD-1.4.8b1/src/IntuneCD/update_notificationTemplate.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/update_powershellScripts.py` & `IntuneCD-1.4.8b1/src/IntuneCD/update_powershellScripts.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/update_proactiveRemediation.py` & `IntuneCD-1.4.8b1/src/IntuneCD/update_proactiveRemediation.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/update_profiles.py` & `IntuneCD-1.4.8b1/src/IntuneCD/update_profiles.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/update_shellScripts.py` & `IntuneCD-1.4.8b1/src/IntuneCD/update_shellScripts.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD/update_windowsEnrollmentProfile.py` & `IntuneCD-1.4.8b1/src/IntuneCD/update_windowsEnrollmentProfile.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD.egg-info/PKG-INFO` & `IntuneCD-1.4.8b1/src/IntuneCD.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IntuneCD
-Version: 1.4.7b1
+Version: 1.4.8b1
 Summary: Tool to backup and update configurations in Intune
 Home-page: https://github.com/almenscorner/IntuneCD
 Author: Tobias Almén
 Author-email: almenscorner@outlook.com
 Project-URL: Bug Tracker, https://github.com/almenscorner/IntuneCD/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `IntuneCD-1.4.7b1/src/IntuneCD.egg-info/SOURCES.txt` & `IntuneCD-1.4.8b1/src/IntuneCD.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 src/IntuneCD/backup_assignmentFilters.py
 src/IntuneCD/backup_autopilotDevices.py
 src/IntuneCD/backup_compliance.py
 src/IntuneCD/backup_compliancePartner.py
 src/IntuneCD/backup_conditionalAccess.py
 src/IntuneCD/backup_configurationPolicies.py
 src/IntuneCD/backup_customAttributeShellScript.py
+src/IntuneCD/backup_deviceCategories.py
 src/IntuneCD/backup_deviceManagementSettings.py
 src/IntuneCD/backup_enrollmentConfigurations.py
 src/IntuneCD/backup_enrollmentStatusPage.py
 src/IntuneCD/backup_groupPolicyConfiguration.py
 src/IntuneCD/backup_managedGPlay.py
 src/IntuneCD/backup_managementIntents.py
 src/IntuneCD/backup_managementPartner.py
@@ -51,14 +52,15 @@
 src/IntuneCD/update_appleEnrollmentProfile.py
 src/IntuneCD/update_assignment.py
 src/IntuneCD/update_assignmentFilter.py
 src/IntuneCD/update_compliance.py
 src/IntuneCD/update_conditionalAccess.py
 src/IntuneCD/update_configurationPolicies.py
 src/IntuneCD/update_customAttributeShellScript.py
+src/IntuneCD/update_deviceCategories.py
 src/IntuneCD/update_deviceManagementSettings.py
 src/IntuneCD/update_enrollmentConfigurations.py
 src/IntuneCD/update_enrollmentStatusPage.py
 src/IntuneCD/update_frontend.py
 src/IntuneCD/update_groupPolicyConfiguration.py
 src/IntuneCD/update_managementIntents.py
 src/IntuneCD/update_notificationTemplate.py
```

### Comparing `IntuneCD-1.4.7b1/tests/test_archive.py` & `IntuneCD-1.4.8b1/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/tests/test_check_file.py` & `IntuneCD-1.4.8b1/tests/test_check_file.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/tests/test_clean_filename.py` & `IntuneCD-1.4.8b1/tests/test_clean_filename.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/tests/test_diff_summary.py` & `IntuneCD-1.4.8b1/tests/test_diff_summary.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/tests/test_documentation_functions.py` & `IntuneCD-1.4.8b1/tests/test_documentation_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,27 +107,27 @@
 
         self.assertEqual(self.result, self.expected_list)
 
     def test_document_configs(self):
         """The list should be returned."""
         self.directory.write(
             "config/test_file_name.json",
-            '{"@odata.type":"test","test":"test","name":"test","description":"test","testvals":"1,2","testbool":false,"testlist":["test"],"testlistdict":[{"test":{"test":{"test":["1"]}}}],"testdict2":{"test":{"test":{"test":["1"]}}},"testdictlist":{"test":["a","b","c"]},"assignments":[{"intent":"apply","target":{"@odata.type":"#test","groupName":"test-group","deviceAndAppManagementAssignmentFilterId":"test-filter","deviceAndAppManagementAssignmentFilterType":"test"}}]}',
+            '{"@odata.type":"test","test":"test","name":"test","description":"test","testvals":"1,2","testbool":false,"testlist":["test"],"testlistdict":[{"test":{"test":{"test":["1"],"testb64":"dW5pY29ybg=="}}}],"testdict2":{"test":{"test":{"test":["1"]}}},"testdictlist":{"test":["a","b","c"]},"assignments":[{"intent":"apply","target":{"@odata.type":"#test","groupName":"test-group","deviceAndAppManagementAssignmentFilterId":"test-filter","deviceAndAppManagementAssignmentFilterType":"test"}}]}',
             encoding="utf-8",
         )
-        self.expected_data = "#test##testDescription:test###Assignments|intent|target|filtertype|filtername||------|----------|-----------|-----------||apply|test-group|test|test-filter|###Configuration|setting|value||------------|-------------------------------------------------------||Odatatype|test||Test|test||Name|test||Testvals|1,2||Testbool|False||Testlist|test<br/>||Testlistdict|**test:**<ul>**test:**<ul><li>1</li></ul></ul><br/>||Testdict2|**test**<ul>**test:**<ul><li>1</li></ul><br/></ul>||Testdictlist|**test:**<ul><li>a</li><li>b</li><li>c</li></ul>|"
+        self.expected_data = "#test##testDescription:test###Assignments|intent|target|filtertype|filtername||------|----------|-----------|-----------||apply|test-group|test|test-filter|###Configuration|setting|value||------------|--------------------------------------------------------------------------------||Odatatype|test||Test|test||Name|test||Testvals|1,2||Testbool|False||Testlist|test<br/>||Testlistdict|**test:**<ul>**test:**<ul><li>1</li></ul>**testb64:**unicorn</br></ul><br/>||Testdict2|**test**<ul>**test:**<ul><li>1</li></ul><br/></ul>||Testdictlist|**test:**<ul><li>a</li><li>b</li><li>c</li></ul>|"
 
         document_configs(
             f"{self.directory.path}/config",
             f"{self.directory.path}/test.md",
             "test",
             100,
             split=False,
             cleanup=True,
-            decode=False,
+            decode=True,
         )
 
         with open(f"{self.directory.path}/test.md", "r") as f:
             self.data = f.read()
             self.result = "".join([line.strip() for line in self.data])
 
         self.assertEqual(self.result, self.expected_data)
```

### Comparing `IntuneCD-1.4.7b1/tests/test_get_added_removed.py` & `IntuneCD-1.4.8b1/tests/test_get_added_removed.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/tests/test_get_authparams.py` & `IntuneCD-1.4.8b1/tests/test_get_authparams.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/tests/test_graph_batch.py` & `IntuneCD-1.4.8b1/tests/test_graph_batch.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/tests/test_graph_request.py` & `IntuneCD-1.4.8b1/tests/test_graph_request.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/tests/test_group_report.py` & `IntuneCD-1.4.8b1/tests/test_group_report.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/tests/test_load_file.py` & `IntuneCD-1.4.8b1/tests/test_load_file.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/tests/test_match.py` & `IntuneCD-1.4.8b1/tests/test_match.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/tests/test_remove_keys.py` & `IntuneCD-1.4.8b1/tests/test_remove_keys.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/tests/test_save_output.py` & `IntuneCD-1.4.8b1/tests/test_save_output.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.7b1/tests/test_update_frontend.py` & `IntuneCD-1.4.8b1/tests/test_update_frontend.py`

 * *Files identical despite different names*

