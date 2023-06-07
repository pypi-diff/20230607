# Comparing `tmp/aliyun-python-sdk-swas-open-1.0.0.tar.gz` & `tmp/aliyun-python-sdk-swas-open-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-swas-open-1.0.0.tar", last modified: Thu Mar  2 02:16:04 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-swas-open-1.0.1.tar", last modified: Wed Jun  7 10:05:40 2023, max compression
```

## Comparing `aliyun-python-sdk-swas-open-1.0.0.tar` & `aliyun-python-sdk-swas-open-1.0.1.tar`

### file list

```diff
@@ -1,63 +1,86 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      575 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1567 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      539 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyun_python_sdk_swas_open.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1567 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyun_python_sdk_swas_open.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3384 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyun_python_sdk_swas_open.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyun_python_sdk_swas_open.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyun_python_sdk_swas_open.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyun_python_sdk_swas_open.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/
--rw-r--r--   0 root         (0) root         (0)     1472 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/AllocatePublicConnectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2234 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/CreateCustomImageRequest.py
--rw-r--r--   0 root         (0) root         (0)     1937 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/CreateFirewallRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     2693 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/CreateInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1583 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/CreateSnapshotRequest.py
--rw-r--r--   0 root         (0) root         (0)     1392 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/DeleteCustomImageRequest.py
--rw-r--r--   0 root         (0) root         (0)     1579 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/DeleteFirewallRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1404 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/DeleteSnapshotRequest.py
--rw-r--r--   0 root         (0) root         (0)     1637 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/DescribeCloudAssistantStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     2009 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/DescribeDatabaseErrorLogsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1844 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/DescribeDatabaseInstanceMetricDataRequest.py
--rw-r--r--   0 root         (0) root         (0)     1295 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/DescribeDatabaseInstanceParametersRequest.py
--rw-r--r--   0 root         (0) root         (0)     1657 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/DescribeDatabaseInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2019 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/DescribeDatabaseSlowLogRecordsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1406 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/DescribeInvocationResultRequest.py
--rw-r--r--   0 root         (0) root         (0)     1794 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/DescribeInvocationsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1249 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/InstallCloudAssistantRequest.py
--rw-r--r--   0 root         (0) root         (0)     1744 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/ListDisksRequest.py
--rw-r--r--   0 root         (0) root         (0)     1587 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/ListFirewallRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1372 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/ListImagesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1237 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/ListInstancePlansModificationRequest.py
--rw-r--r--   0 root         (0) root         (0)     2009 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/ListInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1241 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/ListInstancesTrafficPackagesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1006 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/ListPlansRequest.py
--rw-r--r--   0 root         (0) root         (0)     1010 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/ListRegionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1943 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/ListSnapshotsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1563 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/LoginInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1783 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/ModifyDatabaseInstanceDescriptionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1882 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/ModifyDatabaseInstanceParameterRequest.py
--rw-r--r--   0 root         (0) root         (0)     1587 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/ModifyImageShareStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     1404 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/RebootInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1470 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/ReleasePublicConnectionRequest.py
--rw-r--r--   0 root         (0) root         (0)     1571 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/RenewInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1701 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/ResetDatabaseAccountPasswordRequest.py
--rw-r--r--   0 root         (0) root         (0)     1561 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/ResetDiskRequest.py
--rw-r--r--   0 root         (0) root         (0)     1571 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/ResetSystemRequest.py
--rw-r--r--   0 root         (0) root         (0)     1470 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/RestartDatabaseInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2964 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/RunCommandRequest.py
--rw-r--r--   0 root         (0) root         (0)     1466 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/StartDatabaseInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1402 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/StartInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1464 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/StopDatabaseInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1400 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/StopInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1804 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/UpdateInstanceAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     1573 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/UpgradeInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2482 2023-03-02 02:16:04.000000 aliyun-python-sdk-swas-open-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      539 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyun_python_sdk_swas_open.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyun_python_sdk_swas_open.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4963 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyun_python_sdk_swas_open.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyun_python_sdk_swas_open.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyun_python_sdk_swas_open.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyun_python_sdk_swas_open.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/
+-rw-r--r--   0 root         (0) root         (0)     1472 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/AllocatePublicConnectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2234 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/CreateCustomImageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1937 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/CreateFirewallRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1645 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/CreateFirewallRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1615 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/CreateInstanceKeyPairRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2693 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/CreateInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1583 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/CreateSnapshotRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1392 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/DeleteCustomImageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1579 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/DeleteFirewallRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1418 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/DeleteInstanceKeyPairRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1404 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/DeleteSnapshotRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1412 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/DeleteSnapshotsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1637 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/DescribeCloudAssistantStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1448 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/DescribeCloudMonitorAgentStatusesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2009 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/DescribeDatabaseErrorLogsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1844 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/DescribeDatabaseInstanceMetricDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1295 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/DescribeDatabaseInstanceParametersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1657 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/DescribeDatabaseInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2019 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/DescribeDatabaseSlowLogRecordsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1422 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/DescribeInstanceKeyPairRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/DescribeInstancePasswordsSettingRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1420 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/DescribeInstanceVncUrlRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1406 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/DescribeInvocationResultRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1794 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/DescribeInvocationsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2482 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/DescribeMonitorDataRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1430 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/DescribeSecurityAgentStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1748 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/DisableFirewallRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1949 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/EnableFirewallRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1249 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/InstallCloudAssistantRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1587 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/InstallCloudMonitorAgentRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2403 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/ListCustomImagesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1923 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/ListDisksRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1587 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/ListFirewallRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1372 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/ListImagesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1237 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/ListInstancePlansModificationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/ListInstanceStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2009 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/ListInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1241 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/ListInstancesTrafficPackagesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/ListPlansRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/ListRegionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2158 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/ListSnapshotsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1563 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/LoginInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1783 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/ModifyDatabaseInstanceDescriptionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1882 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/ModifyDatabaseInstanceParameterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2307 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/ModifyFirewallRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1587 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/ModifyImageShareStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1623 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/ModifyInstanceVncPasswordRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1404 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/RebootInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1611 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/RebootInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1470 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/ReleasePublicConnectionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1571 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/RenewInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1701 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/ResetDatabaseAccountPasswordRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1561 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/ResetDiskRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1571 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/ResetSystemRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1470 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/RestartDatabaseInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2964 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/RunCommandRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1466 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/StartDatabaseInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1402 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/StartInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1410 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/StartInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1464 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/StopDatabaseInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1400 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/StopInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/StopInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1557 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/UpdateDiskAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1804 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/UpdateInstanceAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1589 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/UpdateSnapshotAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1573 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/UpgradeInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1800 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/UploadInstanceKeyPairRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2482 2023-06-07 10:05:40.000000 aliyun-python-sdk-swas-open-1.0.1/setup.py
```

### Comparing `aliyun-python-sdk-swas-open-1.0.0/LICENSE` & `aliyun-python-sdk-swas-open-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.0/PKG-INFO` & `aliyun-python-sdk-swas-open-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-swas-open
-Version: 1.0.0
+Version: 1.0.1
 Summary: The swas-open module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-swas-open
```

### Comparing `aliyun-python-sdk-swas-open-1.0.0/README.rst` & `aliyun-python-sdk-swas-open-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.0/aliyun_python_sdk_swas_open.egg-info/PKG-INFO` & `aliyun-python-sdk-swas-open-1.0.1/aliyun_python_sdk_swas_open.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-swas-open
-Version: 1.0.0
+Version: 1.0.1
 Summary: The swas-open module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-swas-open
```

### Comparing `aliyun-python-sdk-swas-open-1.0.0/aliyun_python_sdk_swas_open.egg-info/SOURCES.txt` & `aliyun-python-sdk-swas-open-1.0.1/aliyun_python_sdk_swas_open.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -9,49 +9,72 @@
 aliyun_python_sdk_swas_open.egg-info/requires.txt
 aliyun_python_sdk_swas_open.egg-info/top_level.txt
 aliyunsdkswas_open/__init__.py
 aliyunsdkswas_open/request/__init__.py
 aliyunsdkswas_open/request/v20200601/AllocatePublicConnectionRequest.py
 aliyunsdkswas_open/request/v20200601/CreateCustomImageRequest.py
 aliyunsdkswas_open/request/v20200601/CreateFirewallRuleRequest.py
+aliyunsdkswas_open/request/v20200601/CreateFirewallRulesRequest.py
+aliyunsdkswas_open/request/v20200601/CreateInstanceKeyPairRequest.py
 aliyunsdkswas_open/request/v20200601/CreateInstancesRequest.py
 aliyunsdkswas_open/request/v20200601/CreateSnapshotRequest.py
 aliyunsdkswas_open/request/v20200601/DeleteCustomImageRequest.py
 aliyunsdkswas_open/request/v20200601/DeleteFirewallRuleRequest.py
+aliyunsdkswas_open/request/v20200601/DeleteInstanceKeyPairRequest.py
 aliyunsdkswas_open/request/v20200601/DeleteSnapshotRequest.py
+aliyunsdkswas_open/request/v20200601/DeleteSnapshotsRequest.py
 aliyunsdkswas_open/request/v20200601/DescribeCloudAssistantStatusRequest.py
+aliyunsdkswas_open/request/v20200601/DescribeCloudMonitorAgentStatusesRequest.py
 aliyunsdkswas_open/request/v20200601/DescribeDatabaseErrorLogsRequest.py
 aliyunsdkswas_open/request/v20200601/DescribeDatabaseInstanceMetricDataRequest.py
 aliyunsdkswas_open/request/v20200601/DescribeDatabaseInstanceParametersRequest.py
 aliyunsdkswas_open/request/v20200601/DescribeDatabaseInstancesRequest.py
 aliyunsdkswas_open/request/v20200601/DescribeDatabaseSlowLogRecordsRequest.py
+aliyunsdkswas_open/request/v20200601/DescribeInstanceKeyPairRequest.py
+aliyunsdkswas_open/request/v20200601/DescribeInstancePasswordsSettingRequest.py
+aliyunsdkswas_open/request/v20200601/DescribeInstanceVncUrlRequest.py
 aliyunsdkswas_open/request/v20200601/DescribeInvocationResultRequest.py
 aliyunsdkswas_open/request/v20200601/DescribeInvocationsRequest.py
+aliyunsdkswas_open/request/v20200601/DescribeMonitorDataRequest.py
+aliyunsdkswas_open/request/v20200601/DescribeSecurityAgentStatusRequest.py
+aliyunsdkswas_open/request/v20200601/DisableFirewallRuleRequest.py
+aliyunsdkswas_open/request/v20200601/EnableFirewallRuleRequest.py
 aliyunsdkswas_open/request/v20200601/InstallCloudAssistantRequest.py
+aliyunsdkswas_open/request/v20200601/InstallCloudMonitorAgentRequest.py
+aliyunsdkswas_open/request/v20200601/ListCustomImagesRequest.py
 aliyunsdkswas_open/request/v20200601/ListDisksRequest.py
 aliyunsdkswas_open/request/v20200601/ListFirewallRulesRequest.py
 aliyunsdkswas_open/request/v20200601/ListImagesRequest.py
 aliyunsdkswas_open/request/v20200601/ListInstancePlansModificationRequest.py
+aliyunsdkswas_open/request/v20200601/ListInstanceStatusRequest.py
 aliyunsdkswas_open/request/v20200601/ListInstancesRequest.py
 aliyunsdkswas_open/request/v20200601/ListInstancesTrafficPackagesRequest.py
 aliyunsdkswas_open/request/v20200601/ListPlansRequest.py
 aliyunsdkswas_open/request/v20200601/ListRegionsRequest.py
 aliyunsdkswas_open/request/v20200601/ListSnapshotsRequest.py
 aliyunsdkswas_open/request/v20200601/LoginInstanceRequest.py
 aliyunsdkswas_open/request/v20200601/ModifyDatabaseInstanceDescriptionRequest.py
 aliyunsdkswas_open/request/v20200601/ModifyDatabaseInstanceParameterRequest.py
+aliyunsdkswas_open/request/v20200601/ModifyFirewallRuleRequest.py
 aliyunsdkswas_open/request/v20200601/ModifyImageShareStatusRequest.py
+aliyunsdkswas_open/request/v20200601/ModifyInstanceVncPasswordRequest.py
 aliyunsdkswas_open/request/v20200601/RebootInstanceRequest.py
+aliyunsdkswas_open/request/v20200601/RebootInstancesRequest.py
 aliyunsdkswas_open/request/v20200601/ReleasePublicConnectionRequest.py
 aliyunsdkswas_open/request/v20200601/RenewInstanceRequest.py
 aliyunsdkswas_open/request/v20200601/ResetDatabaseAccountPasswordRequest.py
 aliyunsdkswas_open/request/v20200601/ResetDiskRequest.py
 aliyunsdkswas_open/request/v20200601/ResetSystemRequest.py
 aliyunsdkswas_open/request/v20200601/RestartDatabaseInstanceRequest.py
 aliyunsdkswas_open/request/v20200601/RunCommandRequest.py
 aliyunsdkswas_open/request/v20200601/StartDatabaseInstanceRequest.py
 aliyunsdkswas_open/request/v20200601/StartInstanceRequest.py
+aliyunsdkswas_open/request/v20200601/StartInstancesRequest.py
 aliyunsdkswas_open/request/v20200601/StopDatabaseInstanceRequest.py
 aliyunsdkswas_open/request/v20200601/StopInstanceRequest.py
+aliyunsdkswas_open/request/v20200601/StopInstancesRequest.py
+aliyunsdkswas_open/request/v20200601/UpdateDiskAttributeRequest.py
 aliyunsdkswas_open/request/v20200601/UpdateInstanceAttributeRequest.py
+aliyunsdkswas_open/request/v20200601/UpdateSnapshotAttributeRequest.py
 aliyunsdkswas_open/request/v20200601/UpgradeInstanceRequest.py
+aliyunsdkswas_open/request/v20200601/UploadInstanceKeyPairRequest.py
 aliyunsdkswas_open/request/v20200601/__init__.py
```

### Comparing `aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/AllocatePublicConnectionRequest.py` & `aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/AllocatePublicConnectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/CreateCustomImageRequest.py` & `aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/CreateCustomImageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/CreateFirewallRuleRequest.py` & `aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/CreateFirewallRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/CreateInstancesRequest.py` & `aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/CreateInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/CreateSnapshotRequest.py` & `aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/CreateSnapshotRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/DeleteCustomImageRequest.py` & `aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/DeleteCustomImageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/DeleteFirewallRuleRequest.py` & `aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/DeleteFirewallRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/DeleteSnapshotRequest.py` & `aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/DeleteSnapshotRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/DescribeCloudAssistantStatusRequest.py` & `aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/DescribeCloudAssistantStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/DescribeDatabaseErrorLogsRequest.py` & `aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/DescribeDatabaseErrorLogsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/DescribeDatabaseInstanceMetricDataRequest.py` & `aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/DescribeDatabaseInstanceMetricDataRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/DescribeDatabaseInstanceParametersRequest.py` & `aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/DescribeDatabaseInstanceParametersRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/DescribeDatabaseInstancesRequest.py` & `aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/DescribeDatabaseInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/DescribeDatabaseSlowLogRecordsRequest.py` & `aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/DescribeDatabaseSlowLogRecordsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/DescribeInvocationResultRequest.py` & `aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/DescribeInvocationResultRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/DescribeInvocationsRequest.py` & `aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/DescribeInvocationsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/InstallCloudAssistantRequest.py` & `aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/InstallCloudAssistantRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/ListDisksRequest.py` & `aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/ListFirewallRulesRequest.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
-class ListDisksRequest(RpcRequest):
+class ListFirewallRulesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'SWAS-OPEN', '2020-06-01', 'ListDisks','SWAS-OPEN')
+		RpcRequest.__init__(self, 'SWAS-OPEN', '2020-06-01', 'ListFirewallRules','SWAS-OPEN')
 		self.set_method('POST')
 
 	def get_PageNumber(self): # Integer
 		return self.get_query_params().get('PageNumber')
 
 	def set_PageNumber(self, PageNumber):  # Integer
 		self.add_query_param('PageNumber', PageNumber)
@@ -36,12 +36,7 @@
 	def set_InstanceId(self, InstanceId):  # String
 		self.add_query_param('InstanceId', InstanceId)
 	def get_PageSize(self): # Integer
 		return self.get_query_params().get('PageSize')
 
 	def set_PageSize(self, PageSize):  # Integer
 		self.add_query_param('PageSize', PageSize)
-	def get_DiskIds(self): # String
-		return self.get_query_params().get('DiskIds')
-
-	def set_DiskIds(self, DiskIds):  # String
-		self.add_query_param('DiskIds', DiskIds)
```

### Comparing `aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/ListFirewallRulesRequest.py` & `aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/ListInstanceStatusRequest.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,28 +15,28 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
-class ListFirewallRulesRequest(RpcRequest):
+class ListInstanceStatusRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'SWAS-OPEN', '2020-06-01', 'ListFirewallRules','SWAS-OPEN')
+		RpcRequest.__init__(self, 'SWAS-OPEN', '2020-06-01', 'ListInstanceStatus','SWAS-OPEN')
 		self.set_method('POST')
 
 	def get_PageNumber(self): # Integer
 		return self.get_query_params().get('PageNumber')
 
 	def set_PageNumber(self, PageNumber):  # Integer
 		self.add_query_param('PageNumber', PageNumber)
-	def get_InstanceId(self): # String
-		return self.get_query_params().get('InstanceId')
+	def get_InstanceIds(self): # String
+		return self.get_query_params().get('InstanceIds')
 
-	def set_InstanceId(self, InstanceId):  # String
-		self.add_query_param('InstanceId', InstanceId)
+	def set_InstanceIds(self, InstanceIds):  # String
+		self.add_query_param('InstanceIds', InstanceIds)
 	def get_PageSize(self): # Integer
 		return self.get_query_params().get('PageSize')
 
 	def set_PageSize(self, PageSize):  # Integer
 		self.add_query_param('PageSize', PageSize)
```

### Comparing `aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/ListImagesRequest.py` & `aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/ListImagesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/ListInstancePlansModificationRequest.py` & `aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/ListInstancePlansModificationRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/ListInstancesRequest.py` & `aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/ListInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/ListInstancesTrafficPackagesRequest.py` & `aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/ListInstancesTrafficPackagesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/ListPlansRequest.py` & `aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/ListPlansRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/ListRegionsRequest.py` & `aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/ListRegionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/ListSnapshotsRequest.py` & `aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/ListDisksRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,25 +15,25 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
-class ListSnapshotsRequest(RpcRequest):
+class ListDisksRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'SWAS-OPEN', '2020-06-01', 'ListSnapshots','SWAS-OPEN')
+		RpcRequest.__init__(self, 'SWAS-OPEN', '2020-06-01', 'ListDisks','SWAS-OPEN')
 		self.set_method('POST')
 
-	def get_SnapshotIds(self): # String
-		return self.get_query_params().get('SnapshotIds')
+	def get_DiskType(self): # String
+		return self.get_query_params().get('DiskType')
 
-	def set_SnapshotIds(self, SnapshotIds):  # String
-		self.add_query_param('SnapshotIds', SnapshotIds)
+	def set_DiskType(self, DiskType):  # String
+		self.add_query_param('DiskType', DiskType)
 	def get_PageNumber(self): # Integer
 		return self.get_query_params().get('PageNumber')
 
 	def set_PageNumber(self, PageNumber):  # Integer
 		self.add_query_param('PageNumber', PageNumber)
 	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
@@ -41,12 +41,12 @@
 	def set_InstanceId(self, InstanceId):  # String
 		self.add_query_param('InstanceId', InstanceId)
 	def get_PageSize(self): # Integer
 		return self.get_query_params().get('PageSize')
 
 	def set_PageSize(self, PageSize):  # Integer
 		self.add_query_param('PageSize', PageSize)
-	def get_DiskId(self): # String
-		return self.get_query_params().get('DiskId')
+	def get_DiskIds(self): # String
+		return self.get_query_params().get('DiskIds')
 
-	def set_DiskId(self, DiskId):  # String
-		self.add_query_param('DiskId', DiskId)
+	def set_DiskIds(self, DiskIds):  # String
+		self.add_query_param('DiskIds', DiskIds)
```

### Comparing `aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/LoginInstanceRequest.py` & `aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/LoginInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/ModifyDatabaseInstanceDescriptionRequest.py` & `aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/ModifyDatabaseInstanceDescriptionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/ModifyDatabaseInstanceParameterRequest.py` & `aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/ModifyDatabaseInstanceParameterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/ModifyImageShareStatusRequest.py` & `aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/ModifyImageShareStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/RebootInstanceRequest.py` & `aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/RebootInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/ReleasePublicConnectionRequest.py` & `aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/ReleasePublicConnectionRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/RenewInstanceRequest.py` & `aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/RenewInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/ResetDatabaseAccountPasswordRequest.py` & `aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/ResetDatabaseAccountPasswordRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/ResetDiskRequest.py` & `aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/ResetDiskRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/ResetSystemRequest.py` & `aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/ResetSystemRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/RestartDatabaseInstanceRequest.py` & `aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/RestartDatabaseInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/RunCommandRequest.py` & `aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/RunCommandRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/StartDatabaseInstanceRequest.py` & `aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/StartDatabaseInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/StartInstanceRequest.py` & `aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/StartInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/StopDatabaseInstanceRequest.py` & `aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/StopDatabaseInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/StopInstanceRequest.py` & `aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/StopInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/UpdateInstanceAttributeRequest.py` & `aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/UpdateInstanceAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.0/aliyunsdkswas_open/request/v20200601/UpgradeInstanceRequest.py` & `aliyun-python-sdk-swas-open-1.0.1/aliyunsdkswas_open/request/v20200601/UpgradeInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-swas-open-1.0.0/setup.py` & `aliyun-python-sdk-swas-open-1.0.1/setup.py`

 * *Files identical despite different names*

