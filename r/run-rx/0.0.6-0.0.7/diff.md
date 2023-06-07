# Comparing `tmp/run_rx-0.0.6.tar.gz` & `tmp/run_rx-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "run_rx-0.0.6.tar", max compression
+gzip compressed data, was "run_rx-0.0.7.tar", max compression
```

## Comparing `run_rx-0.0.6.tar` & `run_rx-0.0.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1069 2023-05-16 20:24:41.276898 run_rx-0.0.6/LICENSE.txt
--rw-r--r--   0        0        0     1679 2023-05-19 14:53:21.015913 run_rx-0.0.6/README.md
--rw-r--r--   0        0        0      313 2023-06-01 23:35:09.526681 run_rx-0.0.6/install/.rxignore
--rw-r--r--   0        0        0      274 2023-06-04 16:34:29.656668 run_rx-0.0.6/install/README.md
--rw-r--r--   0        0        0       98 2023-05-16 20:24:41.277933 run_rx-0.0.6/install/python-cpu
--rw-r--r--   0        0        0       98 2023-06-06 18:01:13.521487 run_rx-0.0.6/install/python-gpu
--rw-r--r--   0        0        0      736 2023-06-06 18:24:21.616376 run_rx-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      300 2023-05-16 20:24:41.279362 run_rx-0.0.6/rx/__main__.py
--rw-r--r--   0        0        0     2818 2023-06-06 18:25:15.327114 run_rx-0.0.6/rx/client/commands/exec.py
--rw-r--r--   0        0        0     1284 2023-06-06 18:01:13.522952 run_rx-0.0.6/rx/client/commands/init.py
--rw-r--r--   0        0        0     2109 2023-06-04 16:41:38.419103 run_rx-0.0.6/rx/client/configuration/config_base.py
--rw-r--r--   0        0        0     7016 2023-06-06 18:24:36.468419 run_rx-0.0.6/rx/client/configuration/local.py
--rw-r--r--   0        0        0      641 2023-06-06 18:04:41.546820 run_rx-0.0.6/rx/client/configuration/remote.py
--rw-r--r--   0        0        0     3017 2023-06-06 18:07:01.812095 run_rx-0.0.6/rx/client/executor.py
--rw-r--r--   0        0        0      256 2023-05-16 20:24:41.281715 run_rx-0.0.6/rx/client/grpc_helper.py
--rw-r--r--   0        0        0     5307 2023-06-06 18:09:45.366400 run_rx-0.0.6/rx/client/init_client.py
--rw-r--r--   0        0        0     9694 2023-05-16 20:24:41.282187 run_rx-0.0.6/rx/client/login.py
--rw-r--r--   0        0        0     2029 2023-05-16 20:24:41.282556 run_rx-0.0.6/rx/client/menu.py
--rw-r--r--   0        0        0     1092 2023-05-16 20:24:41.282728 run_rx-0.0.6/rx/client/output_handler.py
--rw-r--r--   0        0        0     3306 2023-06-06 18:01:13.524830 run_rx-0.0.6/rx/client/rsync.py
--rw-r--r--   0        0        0     1603 2023-05-16 20:24:41.283538 run_rx-0.0.6/rx/client/user.py
--rw-r--r--   0        0        0     5866 2023-05-09 18:41:10.568989 run_rx-0.0.6/rx/proto/rx_pb2.py
--rw-r--r--   0        0        0     7595 2023-05-09 18:41:10.570471 run_rx-0.0.6/rx/proto/rx_pb2.pyi
--rw-r--r--   0        0        0    12663 2023-05-09 18:41:10.570796 run_rx-0.0.6/rx/proto/rx_pb2_grpc.py
--rw-r--r--   0        0        0     2597 1970-01-01 00:00:00.000000 run_rx-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-16 20:24:41.276898 run_rx-0.0.7/LICENSE.txt
+-rw-r--r--   0        0        0     1679 2023-05-19 14:53:21.015913 run_rx-0.0.7/README.md
+-rw-r--r--   0        0        0      313 2023-06-01 23:35:09.526681 run_rx-0.0.7/install/.rxignore
+-rw-r--r--   0        0        0      274 2023-06-04 16:34:29.656668 run_rx-0.0.7/install/README.md
+-rw-r--r--   0        0        0       98 2023-05-16 20:24:41.277933 run_rx-0.0.7/install/python-cpu
+-rw-r--r--   0        0        0       98 2023-06-06 18:01:13.521487 run_rx-0.0.7/install/python-gpu
+-rw-r--r--   0        0        0      736 2023-06-07 13:36:28.564487 run_rx-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      300 2023-05-16 20:24:41.279362 run_rx-0.0.7/rx/__main__.py
+-rw-r--r--   0        0        0     2850 2023-06-06 23:31:04.918753 run_rx-0.0.7/rx/client/commands/exec.py
+-rw-r--r--   0        0        0     1284 2023-06-06 19:06:15.414502 run_rx-0.0.7/rx/client/commands/init.py
+-rw-r--r--   0        0        0     2109 2023-06-04 16:41:38.419103 run_rx-0.0.7/rx/client/configuration/config_base.py
+-rw-r--r--   0        0        0     7016 2023-06-07 13:36:36.440622 run_rx-0.0.7/rx/client/configuration/local.py
+-rw-r--r--   0        0        0      641 2023-06-06 18:04:41.546820 run_rx-0.0.7/rx/client/configuration/remote.py
+-rw-r--r--   0        0        0      256 2023-05-16 20:24:41.281715 run_rx-0.0.7/rx/client/grpc_helper.py
+-rw-r--r--   0        0        0     9694 2023-05-16 20:24:41.282187 run_rx-0.0.7/rx/client/login.py
+-rw-r--r--   0        0        0     2029 2023-05-16 20:24:41.282556 run_rx-0.0.7/rx/client/menu.py
+-rw-r--r--   0        0        0     1092 2023-05-16 20:24:41.282728 run_rx-0.0.7/rx/client/output_handler.py
+-rw-r--r--   0        0        0     3306 2023-06-06 18:01:13.524830 run_rx-0.0.7/rx/client/rsync.py
+-rw-r--r--   0        0        0     4668 2023-06-07 12:43:18.155388 run_rx-0.0.7/rx/client/trex_client.py
+-rw-r--r--   0        0        0     1603 2023-05-16 20:24:41.283538 run_rx-0.0.7/rx/client/user.py
+-rw-r--r--   0        0        0     5565 2023-06-07 13:22:07.723770 run_rx-0.0.7/rx/client/worker_client.py
+-rw-r--r--   0        0        0     6391 2023-06-06 22:54:37.232578 run_rx-0.0.7/rx/proto/rx_pb2.py
+-rw-r--r--   0        0        0     8466 2023-06-06 22:54:37.232746 run_rx-0.0.7/rx/proto/rx_pb2.pyi
+-rw-r--r--   0        0        0    12622 2023-06-06 22:54:37.233305 run_rx-0.0.7/rx/proto/rx_pb2_grpc.py
+-rw-r--r--   0        0        0     2597 1970-01-01 00:00:00.000000 run_rx-0.0.7/PKG-INFO
```

### Comparing `run_rx-0.0.6/LICENSE.txt` & `run_rx-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.6/README.md` & `run_rx-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.6/pyproject.toml` & `run_rx-0.0.7/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "run-rx"
-version = "0.0.6"
+version = "0.0.7"
 description = "A tool to simplify remote execution"
 authors = ["Kris Chodorow <k.chodorow@gmail.com>"]
 license = "LICENSE.txt"
 readme = "README.md"
 homepage = "https://www.run-rx.com"
 repository = "https://github.com/run-rx/rx"
 packages = [
```

### Comparing `run_rx-0.0.6/rx/client/commands/exec.py` & `run_rx-0.0.7/rx/client/commands/exec.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import pathlib
 import tempfile
 from typing import List
 
 from absl import app
 from absl import logging
 
-from rx.client import executor
+from rx.client import worker_client
 from rx.client import grpc_helper
 from rx.client.commands import init
 from rx.client.configuration import config_base
 from rx.client.configuration import local
 from rx.client.configuration import remote
 
 
@@ -38,34 +38,34 @@
 
   def run(self) -> int:
     if self._config is None:
       print ('Run `rx init` first!')
       return -1
     remote_cfg = remote.Remote(self._config.cwd)
     with grpc_helper.get_channel(remote_cfg.worker_addr) as ch:
-      client = executor.Client(ch, self._config, remote_cfg)
+      client = worker_client.create_authed_client(ch, self._config)
       return self._try_exec(client)
 
-  def _try_exec(self, client: executor.Client) -> int:
+  def _try_exec(self, client: worker_client.Client) -> int:
     """Sends the command to the server."""
     if len(self._argv) < 1:
       print('No command given.')
       return 1
 
     if len(self._argv) == 1:
       # If this is a quoted arg, break it into pieces. E.g., to pass "ls -l" it
       # must be quoted so that absl doesn't try to capture the -l.
       # TODO: is there a better way to handle this with absl flags?
       self._argv = self._argv[0].split(' ')
     try:
       return client.exec(self._argv)
     except KeyboardInterrupt:
       client.maybe_kill()
-      return executor.SIGINT_CODE
-    except executor.UnreachableError as e:
+      return worker_client.SIGINT_CODE
+    except worker_client.UnreachableError as e:
       print(
         f'Worker {e.worker} was unrechable, run `rx init` to get a new '
         'instance.')
       return e.code
 
 
 class VersionCommand:
@@ -94,12 +94,12 @@
         # "rx run foo" is generally the same as "rx foo", but the extra "run"
         # can be handy when running a script called "init", say, on the remote
         # machine.
         argv = argv[1:]
       cmd = ExecCommand(argv[1:])
     return cmd.run()
   except KeyboardInterrupt:
-    return executor.SIGINT_CODE
+    return worker_client.SIGINT_CODE
 
 
 def run():
   app.run(main)
```

### Comparing `run_rx-0.0.6/rx/client/commands/init.py` & `run_rx-0.0.7/rx/client/commands/init.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pathlib
 import sys
 
 from absl import flags
 from absl import logging
 
 from rx.client import grpc_helper
-from rx.client import init_client
+from rx.client import trex_client
 from rx.client.configuration import config_base
 from rx.client.configuration import local
 
 _DRY_RUN = flags.DEFINE_bool(
   'dry-run', False, 'Shows a list of files that would be uploaded by rx init')
 
 
@@ -26,20 +26,20 @@
     if self._config is None:
       local.install_local_files(self._cwd)
     else:
       logging.info('Workspace already exists, resetting it.')
     try:
       self._config = local.create_local_config(self._cwd)
       with grpc_helper.get_channel(config_base.TREX_HOST.value) as ch:
-        client = init_client.Client(ch, self._config)
+        client = trex_client.Client(ch, self._config)
         if _DRY_RUN.value:
           client.dry_run()
           return 0
         client.create_user_or_log_in()
         return client.init()
-    except init_client.InitError as e:
+    except trex_client.InitError as e:
       sys.stderr.write(f'{e}\n')
       sys.stderr.flush()
       return e.code
 
 if __name__ == '__main__':
   print('Call exec.')
```

### Comparing `run_rx-0.0.6/rx/client/configuration/config_base.py` & `run_rx-0.0.7/rx/client/configuration/config_base.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.6/rx/client/configuration/local.py` & `run_rx-0.0.7/rx/client/configuration/local.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from absl import flags
 from absl import logging
 import sty
 
 from rx.client.configuration import config_base
 from rx.proto import rx_pb2
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 
 IGNORE = pathlib.Path('.rxignore')
 
 _REMOTE = flags.DEFINE_string(
   'remote', None,
   'The path to the remote configuration file to use (see .rx/README.md).')
 _RSYNC_PATH = flags.DEFINE_string('rsync_path', None, 'Path to rsync binary')
```

### Comparing `run_rx-0.0.6/rx/client/configuration/remote.py` & `run_rx-0.0.7/rx/client/configuration/remote.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.6/rx/client/init_client.py` & `run_rx-0.0.7/rx/client/trex_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from google.protobuf import empty_pb2
 import grpc
 
 from rx.client import grpc_helper
 from rx.client import login
 from rx.client import rsync
 from rx.client import user
+from rx.client import worker_client
 from rx.client.configuration import local
 from rx.client.configuration import remote
 from rx.proto import rx_pb2
 from rx.proto import rx_pb2_grpc
 
 _TIMEOUT = 10
 
@@ -58,36 +59,37 @@
             'enthusiasm! Try setting --remote=python-cpu for now.')
       return -1
     req = rx_pb2.InitRequest(
       project_name=self._local_cfg['project_name'],
       rsync_source=self._local_cfg.rsync_source,
       target_env=target_env,
     )
+    # TODO: create a threaded UserStatus class with __enter__/__exit__.
     sys.stdout.write('Finding a remote worker... ')
     sys.stdout.flush()
     try:
       # Five minute timeout.
       resp = self._stub.Init(req, metadata=self._metadata, timeout=(5 * 60))
       sys.stdout.write('Done.\n')
     except grpc.RpcError as e:
       e = cast(grpc.Call, e)
       raise InitError(f'Could not initialize worker: {e.details()}', -1)
     if resp.result.code != 0:
       raise InitError(resp.result.message, -1)
 
-    # TODO: create a threaded UserStatus class with __enter__/__exit__.
-    sys.stdout.write('Copying source code... ')
-    sys.stdout.flush()
     with remote.WritableRemote(self._local_cfg.cwd) as r:
       r['workspace_id'] = resp.workspace_id
       r['worker_addr'] = resp.worker_addr
       r['daemon_module'] = resp.rsync_dest.daemon_module
-    self._run_initial_rsync()
+
+    # Create a container on the worker.
+    with grpc_helper.get_channel(resp.worker_addr) as ch:
+      worker = worker_client.create_authed_client(ch, self._local_cfg)
+      worker.init()
     sys.stdout.write('Done.\n')
-    self._install_deps(resp.worker_addr, resp.workspace_id)
     print('\nDone setting up rx! To use, run:\n\n\t$ rx <your command>\n')
     return 0
 
   def _create_username(self) -> str:
     username = user.username_prompt(self._login.id_token['email'])
     req = rx_pb2.SetUsernameRequest(username=username)
     try:
@@ -114,39 +116,20 @@
       resp = self._stub.GetUser(
         empty_pb2.Empty(), metadata=self._metadata, timeout=_TIMEOUT)
     except grpc.RpcError as e:
       e = cast(grpc.Call, e)
       raise InitError(f'Could not get user from rx: {e.details()}', -1)
     return resp.username
 
-  def _run_initial_rsync(self):
-    r = rsync.RsyncClient(
-      self._local_cfg, remote.Remote(self._local_cfg.cwd))
+  def _run_initial_rsync(self, remote_cfg: remote.Remote):
+    r = rsync.RsyncClient(self._local_cfg, remote_cfg)
     return_code = r.to_remote()
     if return_code == 0:
       logging.info('Copied files to %s', r.host)
 
-  def _install_deps(self, worker_addr: str, workspace_id: str) -> int:
-    channel = grpc_helper.get_channel(worker_addr)
-    stub = rx_pb2_grpc.ExecutionServiceStub(channel)
-    req = rx_pb2.InstallDepsRequest(workspace_id=workspace_id)
-    resp = None
-    try:
-      for resp in stub.InstallDeps(
-        req, metadata=self._metadata, timeout=(10 * 60)):
-        if resp.stdout:
-          sys.stdout.buffer.write(resp.stdout)
-          sys.stdout.buffer.flush()
-    except grpc.RpcError as e:
-      e = cast(grpc.Call, e)
-      raise InitError(e.details(), -1)
-    if resp and resp.HasField('result') and resp.result.code:
-      raise InitError(resp.result.message, resp.result.code)
-    return 0
-
 
 class InitError(RuntimeError):
   """Class to repackage any init errors that happen and add an exit code."""
 
   def __init__(self, message, code, *args):
     super().__init__(message, *args)
     self._code = code
```

### Comparing `run_rx-0.0.6/rx/client/login.py` & `run_rx-0.0.7/rx/client/login.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.6/rx/client/menu.py` & `run_rx-0.0.7/rx/client/menu.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.6/rx/client/output_handler.py` & `run_rx-0.0.7/rx/client/output_handler.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.6/rx/client/rsync.py` & `run_rx-0.0.7/rx/client/rsync.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.6/rx/client/user.py` & `run_rx-0.0.7/rx/client/user.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.6/rx/proto/rx_pb2.py` & `run_rx-0.0.7/rx/proto/rx_pb2.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,61 +10,65 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11rx/proto/rx.proto\x12\x02rx\x1a\x1bgoogle/protobuf/empty.proto\"\x95\x01\n\x06Remote\x12\x1f\n\x05image\x18\x01 \x01(\x0b\x32\x10.rx.Remote.Image\x12%\n\x08hardware\x18\x02 \x01(\x0b\x32\x13.rx.Remote.Hardware\x1a$\n\x05Image\x12\x0e\n\x06\x64ocker\x18\x01 \x01(\t\x12\x0b\n\x03tag\x18\x02 \x01(\t\x1a\x1d\n\x08Hardware\x12\x11\n\tprocessor\x18\x01 \x01(\t\"\x08\n\x06Python\"D\n\x0b\x45nvironment\x12\x19\n\x05\x61lloc\x18\x01 \x01(\x0b\x32\n.rx.Remote\x12\x1a\n\x06python\x18\x02 \x01(\x0b\x32\n.rx.Python\"?\n\x05\x44\x65lta\x12\x10\n\x08\x61\x64\x64_path\x18\x01 \x03(\t\x12\x0f\n\x07\x61\x64\x64_dir\x18\x02 \x03(\t\x12\x13\n\x0bremove_path\x18\x03 \x03(\t\"7\n\x06Result\x12\x1c\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x0e.rx.StatusCode\x12\x0f\n\x07message\x18\x02 \x01(\t\"H\n\x0bRsyncSource\x12\x12\n\nmachine_id\x18\x01 \x01(\x03\x12\x11\n\tdirectory\x18\x02 \x01(\t\x12\x12\n\npublic_key\x18\x03 \x01(\x0c\")\n\x10RsyncDestination\x12\x15\n\rdaemon_module\x18\x01 \x01(\t\")\n\x11\x41llocNewWorkerReq\x12\x14\n\x0cworkspace_id\x18\x01 \x01(\t\"X\n\x0b\x45xecRequest\x12\x14\n\x0cworkspace_id\x18\x01 \x01(\t\x12\x0c\n\x04\x61rgv\x18\x02 \x03(\t\x12%\n\x0crsync_source\x18\x03 \x01(\x0b\x32\x0f.rx.RsyncSource\"v\n\x0c\x45xecResponse\x12\x1a\n\x06result\x18\x01 \x01(\x0b\x32\n.rx.Result\x12\x14\n\x0c\x65xecution_id\x18\x02 \x01(\t\x12\x0e\n\x06stdout\x18\x03 \x01(\x0c\x12\x0e\n\x06stderr\x18\x04 \x01(\x0c\x12\x14\n\x0coutput_files\x18\x05 \x03(\t\"?\n\x0fGetUserResponse\x12\x1a\n\x06result\x18\x01 \x01(\x0b\x32\n.rx.Result\x12\x10\n\x08username\x18\x02 \x01(\t\"o\n\x0bInitRequest\x12\x14\n\x0cproject_name\x18\x01 \x01(\t\x12%\n\x0crsync_source\x18\x02 \x01(\x0b\x32\x0f.rx.RsyncSource\x12#\n\ntarget_env\x18\x03 \x01(\x0b\x32\x0f.rx.Environment\"\x7f\n\x0cInitResponse\x12\x1a\n\x06result\x18\x01 \x01(\x0b\x32\n.rx.Result\x12(\n\nrsync_dest\x18\x02 \x01(\x0b\x32\x14.rx.RsyncDestination\x12\x13\n\x0bworker_addr\x18\x03 \x01(\t\x12\x14\n\x0cworkspace_id\x18\x04 \x01(\t\"*\n\x12InstallDepsRequest\x12\x14\n\x0cworkspace_id\x18\x01 \x01(\t\"A\n\x13InstallDepsResponse\x12\x1a\n\x06result\x18\x01 \x01(\x0b\x32\n.rx.Result\x12\x0e\n\x06stdout\x18\x02 \x01(\x0c\"9\n\x0bKillRequest\x12\x14\n\x0cworkspace_id\x18\x01 \x01(\t\x12\x14\n\x0c\x65xecution_id\x18\x02 \x01(\t\"&\n\x12SetUsernameRequest\x12\x10\n\x08username\x18\x01 \x01(\t\"1\n\x13SetUsernameResponse\x12\x1a\n\x06result\x18\x01 \x01(\x0b\x32\n.rx.Result*O\n\nStatusCode\x12\x06\n\x02OK\x10\x00\x12\x0b\n\x07UNKNOWN\x10\x01\x12\x0b\n\x07INVALID\x10\x02\x12\r\n\tNOT_FOUND\x10\x03\x12\x10\n\x0cUNAUTHORIZED\x10\x04\x32\xb8\x01\n\x10\x45xecutionService\x12\x42\n\x0bInstallDeps\x12\x16.rx.InstallDepsRequest\x1a\x17.rx.InstallDepsResponse\"\x00\x30\x01\x12-\n\x04\x45xec\x12\x0f.rx.ExecRequest\x1a\x10.rx.ExecResponse\"\x00\x30\x01\x12\x31\n\x04Kill\x12\x0f.rx.KillRequest\x1a\x16.google.protobuf.Empty\"\x00\x32\xf4\x01\n\x0cSetupService\x12;\n\x0e\x41llocNewWorker\x12\x15.rx.AllocNewWorkerReq\x1a\x10.rx.InitResponse\"\x00\x12\x38\n\x07GetUser\x12\x16.google.protobuf.Empty\x1a\x13.rx.GetUserResponse\"\x00\x12+\n\x04Init\x12\x0f.rx.InitRequest\x1a\x10.rx.InitResponse\"\x00\x12@\n\x0bSetUsername\x12\x16.rx.SetUsernameRequest\x1a\x17.rx.SetUsernameResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11rx/proto/rx.proto\x12\x02rx\x1a\x1bgoogle/protobuf/empty.proto\"\x95\x01\n\x06Remote\x12\x1f\n\x05image\x18\x01 \x01(\x0b\x32\x10.rx.Remote.Image\x12%\n\x08hardware\x18\x02 \x01(\x0b\x32\x13.rx.Remote.Hardware\x1a$\n\x05Image\x12\x0e\n\x06\x64ocker\x18\x01 \x01(\t\x12\x0b\n\x03tag\x18\x02 \x01(\t\x1a\x1d\n\x08Hardware\x12\x11\n\tprocessor\x18\x01 \x01(\t\"\x08\n\x06Python\"D\n\x0b\x45nvironment\x12\x19\n\x05\x61lloc\x18\x01 \x01(\x0b\x32\n.rx.Remote\x12\x1a\n\x06python\x18\x02 \x01(\x0b\x32\n.rx.Python\"?\n\x05\x44\x65lta\x12\x10\n\x08\x61\x64\x64_path\x18\x01 \x03(\t\x12\x0f\n\x07\x61\x64\x64_dir\x18\x02 \x03(\t\x12\x13\n\x0bremove_path\x18\x03 \x03(\t\"U\n\x17\x44ockerImagePullProgress\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\r\n\x05total\x18\x03 \x01(\x05\x12\x0f\n\x07\x63urrent\x18\x04 \x01(\x05\"7\n\x06Result\x12\x1c\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x0e.rx.StatusCode\x12\x0f\n\x07message\x18\x02 \x01(\t\"H\n\x0bRsyncSource\x12\x12\n\nmachine_id\x18\x01 \x01(\x03\x12\x11\n\tdirectory\x18\x02 \x01(\t\x12\x12\n\npublic_key\x18\x03 \x01(\x0c\")\n\x10RsyncDestination\x12\x15\n\rdaemon_module\x18\x01 \x01(\t\"X\n\x0b\x45xecRequest\x12\x14\n\x0cworkspace_id\x18\x01 \x01(\t\x12\x0c\n\x04\x61rgv\x18\x02 \x03(\t\x12%\n\x0crsync_source\x18\x03 \x01(\x0b\x32\x0f.rx.RsyncSource\"v\n\x0c\x45xecResponse\x12\x1a\n\x06result\x18\x01 \x01(\x0b\x32\n.rx.Result\x12\x14\n\x0c\x65xecution_id\x18\x02 \x01(\t\x12\x0e\n\x06stdout\x18\x03 \x01(\x0c\x12\x0e\n\x06stderr\x18\x04 \x01(\x0c\x12\x14\n\x0coutput_files\x18\x05 \x03(\t\"?\n\x0fGetUserResponse\x12\x1a\n\x06result\x18\x01 \x01(\x0b\x32\n.rx.Result\x12\x10\n\x08username\x18\x02 \x01(\t\"o\n\x0bInitRequest\x12\x14\n\x0cproject_name\x18\x01 \x01(\t\x12%\n\x0crsync_source\x18\x02 \x01(\x0b\x32\x0f.rx.RsyncSource\x12#\n\ntarget_env\x18\x03 \x01(\x0b\x32\x0f.rx.Environment\"\x7f\n\x0cInitResponse\x12\x1a\n\x06result\x18\x01 \x01(\x0b\x32\n.rx.Result\x12(\n\nrsync_dest\x18\x02 \x01(\x0b\x32\x14.rx.RsyncDestination\x12\x13\n\x0bworker_addr\x18\x03 \x01(\t\x12\x14\n\x0cworkspace_id\x18\x04 \x01(\t\"*\n\x12InstallDepsRequest\x12\x14\n\x0cworkspace_id\x18\x01 \x01(\t\"A\n\x13InstallDepsResponse\x12\x1a\n\x06result\x18\x01 \x01(\x0b\x32\n.rx.Result\x12\x0e\n\x06stdout\x18\x02 \x01(\x0c\"9\n\x0bKillRequest\x12\x14\n\x0cworkspace_id\x18\x01 \x01(\t\x12\x14\n\x0c\x65xecution_id\x18\x02 \x01(\t\"&\n\x12SetUsernameRequest\x12\x10\n\x08username\x18\x01 \x01(\t\"1\n\x13SetUsernameResponse\x12\x1a\n\x06result\x18\x01 \x01(\x0b\x32\n.rx.Result\")\n\x11WorkerInitRequest\x12\x14\n\x0cworkspace_id\x18\x01 \x01(\t\"d\n\x12WorkerInitResponse\x12\x1a\n\x06result\x18\x01 \x01(\x0b\x32\n.rx.Result\x12\x32\n\rpull_progress\x18\x02 \x01(\x0b\x32\x1b.rx.DockerImagePullProgress*O\n\nStatusCode\x12\x06\n\x02OK\x10\x00\x12\x0b\n\x07UNKNOWN\x10\x01\x12\x0b\n\x07INVALID\x10\x02\x12\r\n\tNOT_FOUND\x10\x03\x12\x10\n\x0cUNAUTHORIZED\x10\x04\x32\xf3\x01\n\x10\x45xecutionService\x12\x39\n\x04Init\x12\x15.rx.WorkerInitRequest\x1a\x16.rx.WorkerInitResponse\"\x00\x30\x01\x12\x42\n\x0bInstallDeps\x12\x16.rx.InstallDepsRequest\x1a\x17.rx.InstallDepsResponse\"\x00\x30\x01\x12-\n\x04\x45xec\x12\x0f.rx.ExecRequest\x1a\x10.rx.ExecResponse\"\x00\x30\x01\x12\x31\n\x04Kill\x12\x0f.rx.KillRequest\x1a\x16.google.protobuf.Empty\"\x00\x32\xb7\x01\n\x0cSetupService\x12\x38\n\x07GetUser\x12\x16.google.protobuf.Empty\x1a\x13.rx.GetUserResponse\"\x00\x12+\n\x04Init\x12\x0f.rx.InitRequest\x1a\x10.rx.InitResponse\"\x00\x12@\n\x0bSetUsername\x12\x16.rx.SetUsernameRequest\x1a\x17.rx.SetUsernameResponse\"\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'rx.proto.rx_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _STATUSCODE._serialized_start=1346
-  _STATUSCODE._serialized_end=1425
+  _STATUSCODE._serialized_start=1535
+  _STATUSCODE._serialized_end=1614
   _REMOTE._serialized_start=55
   _REMOTE._serialized_end=204
   _REMOTE_IMAGE._serialized_start=137
   _REMOTE_IMAGE._serialized_end=173
   _REMOTE_HARDWARE._serialized_start=175
   _REMOTE_HARDWARE._serialized_end=204
   _PYTHON._serialized_start=206
   _PYTHON._serialized_end=214
   _ENVIRONMENT._serialized_start=216
   _ENVIRONMENT._serialized_end=284
   _DELTA._serialized_start=286
   _DELTA._serialized_end=349
-  _RESULT._serialized_start=351
-  _RESULT._serialized_end=406
-  _RSYNCSOURCE._serialized_start=408
-  _RSYNCSOURCE._serialized_end=480
-  _RSYNCDESTINATION._serialized_start=482
-  _RSYNCDESTINATION._serialized_end=523
-  _ALLOCNEWWORKERREQ._serialized_start=525
-  _ALLOCNEWWORKERREQ._serialized_end=566
-  _EXECREQUEST._serialized_start=568
-  _EXECREQUEST._serialized_end=656
-  _EXECRESPONSE._serialized_start=658
-  _EXECRESPONSE._serialized_end=776
-  _GETUSERRESPONSE._serialized_start=778
-  _GETUSERRESPONSE._serialized_end=841
-  _INITREQUEST._serialized_start=843
-  _INITREQUEST._serialized_end=954
-  _INITRESPONSE._serialized_start=956
-  _INITRESPONSE._serialized_end=1083
-  _INSTALLDEPSREQUEST._serialized_start=1085
-  _INSTALLDEPSREQUEST._serialized_end=1127
-  _INSTALLDEPSRESPONSE._serialized_start=1129
-  _INSTALLDEPSRESPONSE._serialized_end=1194
-  _KILLREQUEST._serialized_start=1196
-  _KILLREQUEST._serialized_end=1253
-  _SETUSERNAMEREQUEST._serialized_start=1255
-  _SETUSERNAMEREQUEST._serialized_end=1293
-  _SETUSERNAMERESPONSE._serialized_start=1295
-  _SETUSERNAMERESPONSE._serialized_end=1344
-  _EXECUTIONSERVICE._serialized_start=1428
-  _EXECUTIONSERVICE._serialized_end=1612
-  _SETUPSERVICE._serialized_start=1615
-  _SETUPSERVICE._serialized_end=1859
+  _DOCKERIMAGEPULLPROGRESS._serialized_start=351
+  _DOCKERIMAGEPULLPROGRESS._serialized_end=436
+  _RESULT._serialized_start=438
+  _RESULT._serialized_end=493
+  _RSYNCSOURCE._serialized_start=495
+  _RSYNCSOURCE._serialized_end=567
+  _RSYNCDESTINATION._serialized_start=569
+  _RSYNCDESTINATION._serialized_end=610
+  _EXECREQUEST._serialized_start=612
+  _EXECREQUEST._serialized_end=700
+  _EXECRESPONSE._serialized_start=702
+  _EXECRESPONSE._serialized_end=820
+  _GETUSERRESPONSE._serialized_start=822
+  _GETUSERRESPONSE._serialized_end=885
+  _INITREQUEST._serialized_start=887
+  _INITREQUEST._serialized_end=998
+  _INITRESPONSE._serialized_start=1000
+  _INITRESPONSE._serialized_end=1127
+  _INSTALLDEPSREQUEST._serialized_start=1129
+  _INSTALLDEPSREQUEST._serialized_end=1171
+  _INSTALLDEPSRESPONSE._serialized_start=1173
+  _INSTALLDEPSRESPONSE._serialized_end=1238
+  _KILLREQUEST._serialized_start=1240
+  _KILLREQUEST._serialized_end=1297
+  _SETUSERNAMEREQUEST._serialized_start=1299
+  _SETUSERNAMEREQUEST._serialized_end=1337
+  _SETUSERNAMERESPONSE._serialized_start=1339
+  _SETUSERNAMERESPONSE._serialized_end=1388
+  _WORKERINITREQUEST._serialized_start=1390
+  _WORKERINITREQUEST._serialized_end=1431
+  _WORKERINITRESPONSE._serialized_start=1433
+  _WORKERINITRESPONSE._serialized_end=1533
+  _EXECUTIONSERVICE._serialized_start=1617
+  _EXECUTIONSERVICE._serialized_end=1860
+  _SETUPSERVICE._serialized_start=1863
+  _SETUPSERVICE._serialized_end=2046
 # @@protoc_insertion_point(module_scope)
```

### Comparing `run_rx-0.0.6/rx/proto/rx_pb2.pyi` & `run_rx-0.0.7/rx/proto/rx_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -8,30 +8,36 @@
 DESCRIPTOR: _descriptor.FileDescriptor
 INVALID: StatusCode
 NOT_FOUND: StatusCode
 OK: StatusCode
 UNAUTHORIZED: StatusCode
 UNKNOWN: StatusCode
 
-class AllocNewWorkerReq(_message.Message):
-    __slots__ = ["workspace_id"]
-    WORKSPACE_ID_FIELD_NUMBER: _ClassVar[int]
-    workspace_id: str
-    def __init__(self, workspace_id: _Optional[str] = ...) -> None: ...
-
 class Delta(_message.Message):
     __slots__ = ["add_dir", "add_path", "remove_path"]
     ADD_DIR_FIELD_NUMBER: _ClassVar[int]
     ADD_PATH_FIELD_NUMBER: _ClassVar[int]
     REMOVE_PATH_FIELD_NUMBER: _ClassVar[int]
     add_dir: _containers.RepeatedScalarFieldContainer[str]
     add_path: _containers.RepeatedScalarFieldContainer[str]
     remove_path: _containers.RepeatedScalarFieldContainer[str]
     def __init__(self, add_path: _Optional[_Iterable[str]] = ..., add_dir: _Optional[_Iterable[str]] = ..., remove_path: _Optional[_Iterable[str]] = ...) -> None: ...
 
+class DockerImagePullProgress(_message.Message):
+    __slots__ = ["current", "id", "status", "total"]
+    CURRENT_FIELD_NUMBER: _ClassVar[int]
+    ID_FIELD_NUMBER: _ClassVar[int]
+    STATUS_FIELD_NUMBER: _ClassVar[int]
+    TOTAL_FIELD_NUMBER: _ClassVar[int]
+    current: int
+    id: str
+    status: str
+    total: int
+    def __init__(self, id: _Optional[str] = ..., status: _Optional[str] = ..., total: _Optional[int] = ..., current: _Optional[int] = ...) -> None: ...
+
 class Environment(_message.Message):
     __slots__ = ["alloc", "python"]
     ALLOC_FIELD_NUMBER: _ClassVar[int]
     PYTHON_FIELD_NUMBER: _ClassVar[int]
     alloc: Remote
     python: Python
     def __init__(self, alloc: _Optional[_Union[Remote, _Mapping]] = ..., python: _Optional[_Union[Python, _Mapping]] = ...) -> None: ...
@@ -168,9 +174,23 @@
 
 class SetUsernameResponse(_message.Message):
     __slots__ = ["result"]
     RESULT_FIELD_NUMBER: _ClassVar[int]
     result: Result
     def __init__(self, result: _Optional[_Union[Result, _Mapping]] = ...) -> None: ...
 
+class WorkerInitRequest(_message.Message):
+    __slots__ = ["workspace_id"]
+    WORKSPACE_ID_FIELD_NUMBER: _ClassVar[int]
+    workspace_id: str
+    def __init__(self, workspace_id: _Optional[str] = ...) -> None: ...
+
+class WorkerInitResponse(_message.Message):
+    __slots__ = ["pull_progress", "result"]
+    PULL_PROGRESS_FIELD_NUMBER: _ClassVar[int]
+    RESULT_FIELD_NUMBER: _ClassVar[int]
+    pull_progress: DockerImagePullProgress
+    result: Result
+    def __init__(self, result: _Optional[_Union[Result, _Mapping]] = ..., pull_progress: _Optional[_Union[DockerImagePullProgress, _Mapping]] = ...) -> None: ...
+
 class StatusCode(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = []
```

### Comparing `run_rx-0.0.6/rx/proto/rx_pb2_grpc.py` & `run_rx-0.0.7/rx/proto/rx_pb2_grpc.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,19 @@
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
+        self.Init = channel.unary_stream(
+                '/rx.ExecutionService/Init',
+                request_serializer=rx_dot_proto_dot_rx__pb2.WorkerInitRequest.SerializeToString,
+                response_deserializer=rx_dot_proto_dot_rx__pb2.WorkerInitResponse.FromString,
+                )
         self.InstallDeps = channel.unary_stream(
                 '/rx.ExecutionService/InstallDeps',
                 request_serializer=rx_dot_proto_dot_rx__pb2.InstallDepsRequest.SerializeToString,
                 response_deserializer=rx_dot_proto_dot_rx__pb2.InstallDepsResponse.FromString,
                 )
         self.Exec = channel.unary_stream(
                 '/rx.ExecutionService/Exec',
@@ -31,14 +36,20 @@
                 response_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                 )
 
 
 class ExecutionServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
+    def Init(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def InstallDeps(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def Exec(self, request, context):
@@ -52,14 +63,19 @@
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_ExecutionServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
+            'Init': grpc.unary_stream_rpc_method_handler(
+                    servicer.Init,
+                    request_deserializer=rx_dot_proto_dot_rx__pb2.WorkerInitRequest.FromString,
+                    response_serializer=rx_dot_proto_dot_rx__pb2.WorkerInitResponse.SerializeToString,
+            ),
             'InstallDeps': grpc.unary_stream_rpc_method_handler(
                     servicer.InstallDeps,
                     request_deserializer=rx_dot_proto_dot_rx__pb2.InstallDepsRequest.FromString,
                     response_serializer=rx_dot_proto_dot_rx__pb2.InstallDepsResponse.SerializeToString,
             ),
             'Exec': grpc.unary_stream_rpc_method_handler(
                     servicer.Exec,
@@ -78,14 +94,31 @@
 
 
  # This class is part of an EXPERIMENTAL API.
 class ExecutionService(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
+    def Init(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_stream(request, target, '/rx.ExecutionService/Init',
+            rx_dot_proto_dot_rx__pb2.WorkerInitRequest.SerializeToString,
+            rx_dot_proto_dot_rx__pb2.WorkerInitResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def InstallDeps(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -138,19 +171,14 @@
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
-        self.AllocNewWorker = channel.unary_unary(
-                '/rx.SetupService/AllocNewWorker',
-                request_serializer=rx_dot_proto_dot_rx__pb2.AllocNewWorkerReq.SerializeToString,
-                response_deserializer=rx_dot_proto_dot_rx__pb2.InitResponse.FromString,
-                )
         self.GetUser = channel.unary_unary(
                 '/rx.SetupService/GetUser',
                 request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
                 response_deserializer=rx_dot_proto_dot_rx__pb2.GetUserResponse.FromString,
                 )
         self.Init = channel.unary_unary(
                 '/rx.SetupService/Init',
@@ -163,21 +191,14 @@
                 response_deserializer=rx_dot_proto_dot_rx__pb2.SetUsernameResponse.FromString,
                 )
 
 
 class SetupServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
-    def AllocNewWorker(self, request, context):
-        """Creates a new worker for an existing workspace.
-        """
-        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
-        context.set_details('Method not implemented!')
-        raise NotImplementedError('Method not implemented!')
-
     def GetUser(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def Init(self, request, context):
@@ -191,19 +212,14 @@
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_SetupServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
-            'AllocNewWorker': grpc.unary_unary_rpc_method_handler(
-                    servicer.AllocNewWorker,
-                    request_deserializer=rx_dot_proto_dot_rx__pb2.AllocNewWorkerReq.FromString,
-                    response_serializer=rx_dot_proto_dot_rx__pb2.InitResponse.SerializeToString,
-            ),
             'GetUser': grpc.unary_unary_rpc_method_handler(
                     servicer.GetUser,
                     request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                     response_serializer=rx_dot_proto_dot_rx__pb2.GetUserResponse.SerializeToString,
             ),
             'Init': grpc.unary_unary_rpc_method_handler(
                     servicer.Init,
@@ -222,31 +238,14 @@
 
 
  # This class is part of an EXPERIMENTAL API.
 class SetupService(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
-    def AllocNewWorker(request,
-            target,
-            options=(),
-            channel_credentials=None,
-            call_credentials=None,
-            insecure=False,
-            compression=None,
-            wait_for_ready=None,
-            timeout=None,
-            metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/rx.SetupService/AllocNewWorker',
-            rx_dot_proto_dot_rx__pb2.AllocNewWorkerReq.SerializeToString,
-            rx_dot_proto_dot_rx__pb2.InitResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
-
-    @staticmethod
     def GetUser(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

### Comparing `run_rx-0.0.6/PKG-INFO` & `run_rx-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: run-rx
-Version: 0.0.6
+Version: 0.0.7
 Summary: A tool to simplify remote execution
 Home-page: https://www.run-rx.com
 License: LICENSE.txt
 Author: Kris Chodorow
 Author-email: k.chodorow@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
```

