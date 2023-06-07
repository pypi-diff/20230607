# Comparing `tmp/yog-2.2.3.tar.gz` & `tmp/yog-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yog-2.2.3.tar", max compression
+gzip compressed data, was "yog-2.2.4.tar", max compression
```

## Comparing `yog-2.2.3.tar` & `yog-2.2.4.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0    10174 2023-02-25 02:02:07.903436 yog-2.2.3/README.md
--rw-r--r--   0        0        0      541 2023-05-30 01:54:05.386243 yog-2.2.3/pyproject.toml
--rw-r--r--   0        0        0        0 2021-07-16 04:35:58.316463 yog-2.2.3/yog/__init__.py
--rw-r--r--   0        0        0      465 2023-02-22 20:50:59.508191 yog-2.2.3/yog/command.py
--rw-r--r--   0        0        0      636 2021-11-19 21:53:36.530661 yog-2.2.3/yog/git_utils.py
--rw-r--r--   0        0        0        0 2021-11-19 21:18:00.056940 yog-2.2.3/yog/host/__init__.py
--rw-r--r--   0        0        0    12156 2023-04-17 17:51:32.509096 yog-2.2.3/yog/host/docker_attrs.py
--rw-r--r--   0        0        0      499 2023-02-22 04:11:12.414451 yog-2.2.3/yog/host/main.py
--rw-r--r--   0        0        0     7454 2023-05-30 01:28:33.283278 yog-2.2.3/yog/host/manage.py
--rw-r--r--   0        0        0     8791 2023-05-30 01:28:33.283278 yog-2.2.3/yog/host/necronomicon.py
--rw-r--r--   0        0        0     1050 2023-05-30 01:28:33.283278 yog-2.2.3/yog/host/os_utils.py
--rw-r--r--   0        0        0    12672 2023-05-30 01:53:37.105511 yog-2.2.3/yog/host/pki.py
--rw-r--r--   0        0        0      752 2023-05-30 01:36:44.675981 yog-2.2.3/yog/host/pki_model.py
--rw-r--r--   0        0        0    11039 2023-02-01 20:50:54.524689 yog-2.2.3/yog/host/test_docker_attrs.py
--rw-r--r--   0        0        0      936 2023-02-22 04:11:12.414451 yog-2.2.3/yog/logging_utils.py
--rw-r--r--   0        0        0      389 2023-02-22 04:11:12.414451 yog-2.2.3/yog/model_utils.py
--rw-r--r--   0        0        0        0 2021-11-19 21:17:46.640293 yog-2.2.3/yog/repo/__init__.py
--rw-r--r--   0        0        0     4580 2022-12-28 04:50:30.284835 yog-2.2.3/yog/repo/main.py
--rw-r--r--   0        0        0      120 2021-07-25 01:26:53.898074 yog-2.2.3/yog/res/__init__.py
--rw-r--r--   0        0        0       80 2023-02-22 04:11:12.414451 yog-2.2.3/yog/res/cas.yml
--rw-r--r--   0        0        0      707 2023-02-01 20:50:54.524689 yog-2.2.3/yog/res/docker_test.yml
--rw-r--r--   0        0        0      434 2023-02-01 20:50:54.524689 yog-2.2.3/yog/res/sample_necronomicon.yml
--rw-r--r--   0        0        0      426 2021-07-30 04:19:50.436971 yog-2.2.3/yog/res/sample_needs_tunnel_back.yml
--rw-r--r--   0        0        0      195 2023-05-30 01:31:38.821403 yog-2.2.3/yog/res/sample_pki_necronomicon.yml
--rw-r--r--   0        0        0       50 2021-07-25 01:26:25.424796 yog-2.2.3/yog/res/sample_site_necronomicon.yml
--rw-r--r--   0        0        0    11032 2023-05-30 01:53:37.125512 yog-2.2.3/yog/ssh_utils.py
--rw-r--r--   0        0        0    10804 1970-01-01 00:00:00.000000 yog-2.2.3/PKG-INFO
+-rw-r--r--   0        0        0    10174 2023-02-25 02:02:07.903436 yog-2.2.4/README.md
+-rw-r--r--   0        0        0      541 2023-06-07 04:40:28.802373 yog-2.2.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-07-16 04:35:58.316463 yog-2.2.4/yog/__init__.py
+-rw-r--r--   0        0        0      465 2023-02-22 20:50:59.508191 yog-2.2.4/yog/command.py
+-rw-r--r--   0        0        0      636 2021-11-19 21:53:36.530661 yog-2.2.4/yog/git_utils.py
+-rw-r--r--   0        0        0        0 2021-11-19 21:18:00.056940 yog-2.2.4/yog/host/__init__.py
+-rw-r--r--   0        0        0    12156 2023-04-17 17:51:32.509096 yog-2.2.4/yog/host/docker_attrs.py
+-rw-r--r--   0        0        0      499 2023-02-22 04:11:12.414451 yog-2.2.4/yog/host/main.py
+-rw-r--r--   0        0        0     7573 2023-06-07 04:40:13.632348 yog-2.2.4/yog/host/manage.py
+-rw-r--r--   0        0        0     9656 2023-06-07 04:40:13.632348 yog-2.2.4/yog/host/necronomicon.py
+-rw-r--r--   0        0        0     1050 2023-05-30 01:28:33.283278 yog-2.2.4/yog/host/os_utils.py
+-rw-r--r--   0        0        0    12672 2023-05-30 01:53:37.105511 yog-2.2.4/yog/host/pki.py
+-rw-r--r--   0        0        0      752 2023-05-30 01:36:44.675981 yog-2.2.4/yog/host/pki_model.py
+-rw-r--r--   0        0        0     1516 2023-06-07 04:40:13.632348 yog-2.2.4/yog/host/systemd.py
+-rw-r--r--   0        0        0    11039 2023-02-01 20:50:54.524689 yog-2.2.4/yog/host/test_docker_attrs.py
+-rw-r--r--   0        0        0      936 2023-02-22 04:11:12.414451 yog-2.2.4/yog/logging_utils.py
+-rw-r--r--   0        0        0      389 2023-02-22 04:11:12.414451 yog-2.2.4/yog/model_utils.py
+-rw-r--r--   0        0        0        0 2021-11-19 21:17:46.640293 yog-2.2.4/yog/repo/__init__.py
+-rw-r--r--   0        0        0     4580 2022-12-28 04:50:30.284835 yog-2.2.4/yog/repo/main.py
+-rw-r--r--   0        0        0      120 2021-07-25 01:26:53.898074 yog-2.2.4/yog/res/__init__.py
+-rw-r--r--   0        0        0       80 2023-02-22 04:11:12.414451 yog-2.2.4/yog/res/cas.yml
+-rw-r--r--   0        0        0      707 2023-02-01 20:50:54.524689 yog-2.2.4/yog/res/docker_test.yml
+-rw-r--r--   0        0        0      434 2023-02-01 20:50:54.524689 yog-2.2.4/yog/res/sample_necronomicon.yml
+-rw-r--r--   0        0        0      426 2021-07-30 04:19:50.436971 yog-2.2.4/yog/res/sample_needs_tunnel_back.yml
+-rw-r--r--   0        0        0      195 2023-05-30 01:31:38.821403 yog-2.2.4/yog/res/sample_pki_necronomicon.yml
+-rw-r--r--   0        0        0       50 2021-07-25 01:26:25.424796 yog-2.2.4/yog/res/sample_site_necronomicon.yml
+-rw-r--r--   0        0        0    11032 2023-05-30 01:53:37.125512 yog-2.2.4/yog/ssh_utils.py
+-rw-r--r--   0        0        0    10804 1970-01-01 00:00:00.000000 yog-2.2.4/PKG-INFO
```

### Comparing `yog-2.2.3/README.md` & `yog-2.2.4/README.md`

 * *Files identical despite different names*

### Comparing `yog-2.2.3/pyproject.toml` & `yog-2.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yog"
-version = "2.2.3"
+version = "2.2.4"
 description = "The Gate and Key"
 authors = ["Josh Hertlein <jmhertlein@gmail.com>"]
 license = "AGPLv3"
 readme = "README.md"
 
 [tool.poetry.scripts]
 yog = "yog.host.main:main"
```

### Comparing `yog-2.2.3/yog/git_utils.py` & `yog-2.2.4/yog/git_utils.py`

 * *Files identical despite different names*

### Comparing `yog-2.2.3/yog/host/docker_attrs.py` & `yog-2.2.4/yog/host/docker_attrs.py`

 * *Files identical despite different names*

### Comparing `yog-2.2.3/yog/host/manage.py` & `yog-2.2.4/yog/host/manage.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from paramiko.ssh_exception import NoValidConnectionsError
 from yog.host.pki_model import load_cas
 
 from yog.host import necronomicon
 from yog.host.docker_attrs import build_run_kwargs_dict, diff_container
 from yog.host.necronomicon import Necronomicon, File
 import yog.host.pki as pki
+import yog.host.systemd as systemd
 from yog.ssh_utils import check_call, ScopedProxiedRemoteSSHTunnel, compare_local_and_remote
 
 log = logging.getLogger(__name__)
 
 
 def apply_necronomicon(host: str, root_dir):
     ssh = SSHClient()
@@ -62,14 +63,16 @@
             apply_files_section(host, n, ssh, root_dir)
         if n.docker.containers:
             apply_docker_section(host, n)
         if n.cron.crons:
             apply_cron_section(host, n, ssh)
         if n.pki.certs:
             pki.apply_pki_section(host, n, ssh, root_dir)
+        if n.systemd.units:
+            systemd.apply_systemd_section(host, n, ssh)
 
 
 def apply_cron_section(host: str, n: Necronomicon, ssh: SSHClient):
     cronfile_lines = []
     line1_length = max([len(c.expr) for c in n.cron.crons])
     line2_length = max([len(c.user) for c in n.cron.crons])
     for cron in n.cron.crons:
```

### Comparing `yog-2.2.3/yog/host/necronomicon.py` & `yog-2.2.4/yog/host/necronomicon.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import re
 import typing as t
 from dataclasses import dataclass
 from ipaddress import ip_address, IPv4Address
 
 import yaml
 from paramiko.client import SSHClient
 from yog.model_utils import HostPathStr, parse_hostpath
@@ -68,24 +69,30 @@
     if 'pki' in parsed_necronomicon:
         pki = PKI([CertEntry.from_parsed(e) for e in parsed_necronomicon['pki']['certs']] if 'certs' in parsed_necronomicon['pki'] else [],
                   # parsed_necronomicon['pki']['authorities'] if 'authorities' in parsed_necronomicon['pki'] else []
                   )
     else:
         pki = PKI([])
 
-    return Necronomicon(ident, tunnels, ds, cs, fs, pki)
+    if 'systemd' in parsed_necronomicon:
+        systemd = SystemdSection.from_parsed(parsed_necronomicon['systemd'])
+    else:
+        systemd = SystemdSection(units=[])
+
+    return Necronomicon(ident, tunnels, ds, cs, fs, pki, systemd)
 
 
 class Necronomicon(t.NamedTuple):
     ident: str
     tunnels: 'NeededTunnelsSection'
     docker: 'DockerSection'
     cron: 'CronSection'
     files: 'FileSection'
     pki: 'PKI'
+    systemd: 'SystemdSection'
 
     def inflate(self, host: str, ssh: SSHClient) -> 'Necronomicon':
         inflated_containers = []
         for desired_container in self.docker.containers:
             inflated_desired_container_env = {}
             for name, value in desired_container.env.items():
                 value = str(value)
@@ -114,14 +121,15 @@
         return Necronomicon(
             self.ident,
             self.tunnels,
             DockerSection(inflated_containers),
             self.cron,
             self.files,
             self.pki,
+            self.systemd
         )
 
 
 class DockerSection(t.NamedTuple):
     containers: t.List['DockerContainer']
 
 
@@ -282,7 +290,28 @@
             o['chown'] if 'chown' in o else "root:root",
         )
 
 
 class PKI(t.NamedTuple):
     certs: t.List[CertEntry]
 
+
+class SystemdUnit(t.NamedTuple):
+    name: str
+    description: str
+    user: str
+    cmd: str
+
+    @staticmethod
+    def from_parsed(p) -> 'SystemdUnit':
+        if not re.match(r'[a-zA-Z0-9-_.]+', p['name']):
+            raise ValueError("Systemd unit names must be [a-zA-Z0-9-_.]")
+        return SystemdUnit(p['name'], p['description'], p['user'] if 'user' in p else 'root', p['cmd'])
+
+
+class SystemdSection(t.NamedTuple):
+    units: t.List[SystemdUnit]
+
+    @staticmethod
+    def from_parsed(parsed) -> 'SystemdSection':
+        return SystemdSection(units=[SystemdUnit.from_parsed(p) for p in parsed['units']])
+
```

### Comparing `yog-2.2.3/yog/host/os_utils.py` & `yog-2.2.4/yog/host/os_utils.py`

 * *Files identical despite different names*

### Comparing `yog-2.2.3/yog/host/pki.py` & `yog-2.2.4/yog/host/pki.py`

 * *Files identical despite different names*

### Comparing `yog-2.2.3/yog/host/pki_model.py` & `yog-2.2.4/yog/host/pki_model.py`

 * *Files identical despite different names*

### Comparing `yog-2.2.3/yog/host/test_docker_attrs.py` & `yog-2.2.4/yog/host/test_docker_attrs.py`

 * *Files identical despite different names*

### Comparing `yog-2.2.3/yog/logging_utils.py` & `yog-2.2.4/yog/logging_utils.py`

 * *Files identical despite different names*

### Comparing `yog-2.2.3/yog/repo/main.py` & `yog-2.2.4/yog/repo/main.py`

 * *Files identical despite different names*

### Comparing `yog-2.2.3/yog/res/docker_test.yml` & `yog-2.2.4/yog/res/docker_test.yml`

 * *Files identical despite different names*

### Comparing `yog-2.2.3/yog/ssh_utils.py` & `yog-2.2.4/yog/ssh_utils.py`

 * *Files identical despite different names*

### Comparing `yog-2.2.3/PKG-INFO` & `yog-2.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yog
-Version: 2.2.3
+Version: 2.2.4
 Summary: The Gate and Key
 License: AGPLv3
 Author: Josh Hertlein
 Author-email: jmhertlein@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

