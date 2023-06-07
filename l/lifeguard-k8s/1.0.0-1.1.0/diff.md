# Comparing `tmp/lifeguard-k8s-1.0.0.tar.gz` & `tmp/lifeguard-k8s-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifeguard-k8s-1.0.0.tar", last modified: Fri Jun  2 17:38:17 2023, max compression
+gzip compressed data, was "lifeguard-k8s-1.1.0.tar", last modified: Wed Jun  7 19:45:55 2023, max compression
```

## Comparing `lifeguard-k8s-1.0.0.tar` & `lifeguard-k8s-1.1.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:38:17.150241 lifeguard-k8s-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-02 17:38:17.150241 lifeguard-k8s-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-02 17:37:47.000000 lifeguard-k8s-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:38:17.150241 lifeguard-k8s-1.0.0/lifeguard_k8s/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-02 17:37:47.000000 lifeguard-k8s-1.0.0/lifeguard_k8s/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:38:17.150241 lifeguard-k8s-1.0.0/lifeguard_k8s/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:37:47.000000 lifeguard-k8s-1.0.0/lifeguard_k8s/actions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:38:17.150241 lifeguard-k8s-1.0.0/lifeguard_k8s/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:37:47.000000 lifeguard-k8s-1.0.0/lifeguard_k8s/infrastructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-02 17:37:47.000000 lifeguard-k8s-1.0.0/lifeguard_k8s/infrastructure/pods.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-02 17:37:47.000000 lifeguard-k8s-1.0.0/lifeguard_k8s/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:38:17.150241 lifeguard-k8s-1.0.0/lifeguard_k8s/validations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:37:47.000000 lifeguard-k8s-1.0.0/lifeguard_k8s/validations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-02 17:37:47.000000 lifeguard-k8s-1.0.0/lifeguard_k8s/validations/pods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:38:17.150241 lifeguard-k8s-1.0.0/lifeguard_k8s.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-02 17:38:17.000000 lifeguard-k8s-1.0.0/lifeguard_k8s.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-02 17:38:17.000000 lifeguard-k8s-1.0.0/lifeguard_k8s.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 17:38:17.000000 lifeguard-k8s-1.0.0/lifeguard_k8s.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-02 17:38:17.000000 lifeguard-k8s-1.0.0/lifeguard_k8s.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-02 17:38:17.000000 lifeguard-k8s-1.0.0/lifeguard_k8s.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 17:38:17.150241 lifeguard-k8s-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-02 17:37:47.000000 lifeguard-k8s-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:38:17.150241 lifeguard-k8s-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:37:47.000000 lifeguard-k8s-1.0.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:38:17.150241 lifeguard-k8s-1.0.0/tests/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:37:47.000000 lifeguard-k8s-1.0.0/tests/infrastructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-06-02 17:37:47.000000 lifeguard-k8s-1.0.0/tests/infrastructure/test_pods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 17:38:17.150241 lifeguard-k8s-1.0.0/tests/validations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 17:37:47.000000 lifeguard-k8s-1.0.0/tests/validations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-02 17:37:47.000000 lifeguard-k8s-1.0.0/tests/validations/test_pods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:45:55.805562 lifeguard-k8s-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-07 19:45:55.805562 lifeguard-k8s-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-07 19:45:28.000000 lifeguard-k8s-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:45:55.801562 lifeguard-k8s-1.1.0/lifeguard_k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-07 19:45:28.000000 lifeguard-k8s-1.1.0/lifeguard_k8s/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:45:55.805562 lifeguard-k8s-1.1.0/lifeguard_k8s/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:45:28.000000 lifeguard-k8s-1.1.0/lifeguard_k8s/actions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:45:55.805562 lifeguard-k8s-1.1.0/lifeguard_k8s/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:45:28.000000 lifeguard-k8s-1.1.0/lifeguard_k8s/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-06-07 19:45:28.000000 lifeguard-k8s-1.1.0/lifeguard_k8s/infrastructure/pods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-07 19:45:28.000000 lifeguard-k8s-1.1.0/lifeguard_k8s/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:45:55.805562 lifeguard-k8s-1.1.0/lifeguard_k8s/validations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:45:28.000000 lifeguard-k8s-1.1.0/lifeguard_k8s/validations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-06-07 19:45:28.000000 lifeguard-k8s-1.1.0/lifeguard_k8s/validations/pods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:45:55.805562 lifeguard-k8s-1.1.0/lifeguard_k8s.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-07 19:45:55.000000 lifeguard-k8s-1.1.0/lifeguard_k8s.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-07 19:45:55.000000 lifeguard-k8s-1.1.0/lifeguard_k8s.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 19:45:55.000000 lifeguard-k8s-1.1.0/lifeguard_k8s.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-07 19:45:55.000000 lifeguard-k8s-1.1.0/lifeguard_k8s.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-07 19:45:55.000000 lifeguard-k8s-1.1.0/lifeguard_k8s.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 19:45:55.805562 lifeguard-k8s-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-07 19:45:28.000000 lifeguard-k8s-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:45:55.805562 lifeguard-k8s-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:45:28.000000 lifeguard-k8s-1.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:45:55.805562 lifeguard-k8s-1.1.0/tests/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:45:28.000000 lifeguard-k8s-1.1.0/tests/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-06-07 19:45:28.000000 lifeguard-k8s-1.1.0/tests/infrastructure/test_pods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:45:55.805562 lifeguard-k8s-1.1.0/tests/validations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:45:28.000000 lifeguard-k8s-1.1.0/tests/validations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-06-07 19:45:28.000000 lifeguard-k8s-1.1.0/tests/validations/test_pods.py
```

### Comparing `lifeguard-k8s-1.0.0/lifeguard_k8s/infrastructure/pods.py` & `lifeguard-k8s-1.1.0/lifeguard_k8s/infrastructure/pods.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 from kubernetes import client, config
-from lifeguard_k8s.settings import LIFEGUARD_KUBERNETES_CONFIG
+from lifeguard_k8s.settings import (
+    LIFEGUARD_KUBERNETES_CONFIG,
+    LIFEGUARD_KUBERNETES_READ_LOG_MAX_SIZE,
+)
 
 RUNNING_STATUS = "Running"
 COMPLETED_STATUS = "Succeeded"
 
 NORMAL_STATUSES = [RUNNING_STATUS, COMPLETED_STATUS]
 
 
@@ -17,29 +20,63 @@
             job_pod.metadata.owner_references[0].name in pod.metadata.name
             and pod.status.phase == COMPLETED_STATUS
         ):
             return True
     return False
 
 
-def get_not_running_pods(namespace):
-    not_running_pods = []
-
+def _get_clients():
     if LIFEGUARD_KUBERNETES_CONFIG:
         config.load_kube_config(LIFEGUARD_KUBERNETES_CONFIG)
     else:
         config.load_incluster_config()
 
-    v1 = client.CoreV1Api()
+    return client.CoreV1Api()
+
+
+def get_not_running_pods(namespace):
+    not_running_pods = []
+
+    v1 = _get_clients()
     pods = v1.list_namespaced_pod(namespace)
 
     for pod in pods.items:
         if pod.status.phase not in NORMAL_STATUSES or (
             not all(container.ready for container in pod.status.container_statuses)
         ):
             if _check_if_job_pod(pod):
                 if not _exists_success_pod_after_job(pod, pods):
                     not_running_pods.append(pod.metadata.name)
             else:
                 not_running_pods.append(pod.metadata.name)
 
     return not_running_pods
+
+
+def get_events_from_pod(namespace, pod_name):
+    v1 = _get_clients()
+    events = v1.list_namespaced_event(
+        namespace, field_selector=f"involvedObject.name={pod_name}"
+    )
+    return [
+        {"event_type": item.type, "message": item.message, "reason": item.reason}
+        for item in events.items
+    ]
+
+
+def get_last_error_event_from_pod(namespace, pod_name):
+    events = get_events_from_pod(namespace, pod_name)
+    events = [event for event in events if event["event_type"] != "Normal"]
+
+    if events:
+        failed = [event for event in events if event["reason"] == "Failed"]
+        if failed:
+            return failed[-1]
+        return events[-1]
+
+    return None
+
+
+def get_logs_from_pod(namespace, pod_name):
+    v1 = _get_clients()
+    log = v1.read_namespaced_pod_log(pod_name, namespace)
+    return log[-LIFEGUARD_KUBERNETES_READ_LOG_MAX_SIZE:]
```

### Comparing `lifeguard-k8s-1.0.0/lifeguard_k8s.egg-info/SOURCES.txt` & `lifeguard-k8s-1.1.0/lifeguard_k8s.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lifeguard-k8s-1.0.0/setup.py` & `lifeguard-k8s-1.1.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="lifeguard-k8s",
-    version="1.0.0",
+    version="1.1.0",
     url="https://github.com/LifeguardSystem/lifeguard-k8s",
     author="Diego Rubin",
     author_email="contact@diegorubin.dev",
     license="GPL2",
     scripts=[],
     include_package_data=True,
     description="Lifeguard integration with Kubernetes",
```

