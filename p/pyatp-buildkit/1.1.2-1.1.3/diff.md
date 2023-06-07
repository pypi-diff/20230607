# Comparing `tmp/pyatp_buildkit-1.1.2.tar.gz` & `tmp/pyatp_buildkit-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyatp_buildkit-1.1.2.tar", max compression
+gzip compressed data, was "pyatp_buildkit-1.1.3.tar", max compression
```

## Comparing `pyatp_buildkit-1.1.2.tar` & `pyatp_buildkit-1.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      501 2023-06-07 02:54:51.850910 pyatp_buildkit-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     1148 2023-06-06 06:46:33.737928 pyatp_buildkit-1.1.2/src/pyatp_buildkit/__init__.py
--rw-r--r--   0        0        0    11435 2023-06-07 02:53:26.524927 pyatp_buildkit-1.1.2/src/pyatp_buildkit/build.py
--rw-r--r--   0        0        0      542 2023-06-06 06:46:33.738272 pyatp_buildkit-1.1.2/src/pyatp_buildkit/config.py
--rw-r--r--   0        0        0      529 2023-06-06 06:46:33.738346 pyatp_buildkit-1.1.2/src/pyatp_buildkit/dotdict.py
--rw-r--r--   0        0        0      610 2023-06-06 06:46:33.738426 pyatp_buildkit-1.1.2/src/pyatp_buildkit/error.py
--rw-r--r--   0        0        0  2680354 2023-06-06 06:46:33.750086 pyatp_buildkit-1.1.2/src/pyatp_buildkit/get-pip.py
--rw-r--r--   0        0        0     1249 2023-06-06 07:31:52.608041 pyatp_buildkit-1.1.2/src/pyatp_buildkit/templates/Dockerfile.j2
--rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 pyatp_buildkit-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0      501 2023-06-07 03:26:38.953657 pyatp_buildkit-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1148 2023-06-06 06:46:33.737928 pyatp_buildkit-1.1.3/src/pyatp_buildkit/__init__.py
+-rw-r--r--   0        0        0    11546 2023-06-07 03:26:16.377637 pyatp_buildkit-1.1.3/src/pyatp_buildkit/build.py
+-rw-r--r--   0        0        0      542 2023-06-06 06:46:33.738272 pyatp_buildkit-1.1.3/src/pyatp_buildkit/config.py
+-rw-r--r--   0        0        0      529 2023-06-06 06:46:33.738346 pyatp_buildkit-1.1.3/src/pyatp_buildkit/dotdict.py
+-rw-r--r--   0        0        0      610 2023-06-06 06:46:33.738426 pyatp_buildkit-1.1.3/src/pyatp_buildkit/error.py
+-rw-r--r--   0        0        0  2680354 2023-06-06 06:46:33.750086 pyatp_buildkit-1.1.3/src/pyatp_buildkit/get-pip.py
+-rw-r--r--   0        0        0     1249 2023-06-06 07:31:52.608041 pyatp_buildkit-1.1.3/src/pyatp_buildkit/templates/Dockerfile.j2
+-rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 pyatp_buildkit-1.1.3/PKG-INFO
```

### Comparing `pyatp_buildkit-1.1.2/src/pyatp_buildkit/__init__.py` & `pyatp_buildkit-1.1.3/src/pyatp_buildkit/__init__.py`

 * *Files identical despite different names*

### Comparing `pyatp_buildkit-1.1.2/src/pyatp_buildkit/build.py` & `pyatp_buildkit-1.1.3/src/pyatp_buildkit/build.py`

 * *Files 1% similar despite different names*

```diff
@@ -320,25 +320,29 @@
             log.info(f.read())
         f.close()
         cmd = f"docker buildx build . -t artifacts.iflytek.com/docker-private/atp/train/{self.inference_task}:{self.tag} --push"
         log.info(cmd)
 
     def buildx(self):
         # 1. check buildx command
+        global dockerfile_dir
         mock = True
         docker_bin = "/usr/local/bin/docker"
         if os.path.exists(docker_bin):
             mock = False
 
         if mock:
             self.mock_buildx()
             return
+        pwd = os.getcwd()
         cmd = f"docker buildx build . -t artifacts.iflytek.com/docker-private/atp/train/{self.inference_task}:{self.tag} --push"
         log.info(cmd)
+        os.chdir(dockerfile_dir)
         subprocess.call(cmd, shell=True)
+        os.chdir(pwd)
 
     def render(self, render_vars):
         s = self.template.render(**render_vars)
         return s
 
     def get_regsitry(self):
         if self.use_github:
```

### Comparing `pyatp_buildkit-1.1.2/src/pyatp_buildkit/config.py` & `pyatp_buildkit-1.1.3/src/pyatp_buildkit/config.py`

 * *Files identical despite different names*

### Comparing `pyatp_buildkit-1.1.2/src/pyatp_buildkit/dotdict.py` & `pyatp_buildkit-1.1.3/src/pyatp_buildkit/dotdict.py`

 * *Files identical despite different names*

### Comparing `pyatp_buildkit-1.1.2/src/pyatp_buildkit/error.py` & `pyatp_buildkit-1.1.3/src/pyatp_buildkit/error.py`

 * *Files identical despite different names*

### Comparing `pyatp_buildkit-1.1.2/src/pyatp_buildkit/get-pip.py` & `pyatp_buildkit-1.1.3/src/pyatp_buildkit/get-pip.py`

 * *Files identical despite different names*

### Comparing `pyatp_buildkit-1.1.2/src/pyatp_buildkit/templates/Dockerfile.j2` & `pyatp_buildkit-1.1.3/src/pyatp_buildkit/templates/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `pyatp_buildkit-1.1.2/PKG-INFO` & `pyatp_buildkit-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatp-buildkit
-Version: 1.1.2
+Version: 1.1.3
 Summary: a iflytek ailab library ...
 License: Apache License 2
 Author: mjchen
 Author-email: mjchen@iflytek.com
 Requires-Python: >3.7
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

