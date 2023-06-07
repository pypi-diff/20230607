# Comparing `tmp/psytricks-2.1.2.tar.gz` & `tmp/psytricks-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psytricks-2.1.2.tar", max compression
+gzip compressed data, was "psytricks-2.1.3.tar", max compression
```

## Comparing `psytricks-2.1.2.tar` & `psytricks-2.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    35059 2022-12-20 15:40:57.930292 psytricks-2.1.2/LICENSE
--rw-r--r--   0        0        0     7269 2023-06-06 15:08:16.471093 psytricks-2.1.2/README.md
--rw-r--r--   0        0        0     1112 2023-06-06 15:19:43.333680 psytricks-2.1.2/pyproject.toml
--rw-r--r--   0        0        0       93 2023-06-06 15:19:43.337680 psytricks-2.1.2/src/psytricks/__init__.py
--rw-r--r--   0        0        0     6146 2023-06-06 15:19:43.337680 psytricks-2.1.2/src/psytricks/__ps1__/psytricks-lib.ps1
--rw-r--r--   0        0        0     6392 2023-05-10 19:08:40.530093 psytricks-2.1.2/src/psytricks/__ps1__/psytricks-wrapper.ps1
--rw-r--r--   0        0        0     1961 2023-05-10 19:08:40.530093 psytricks-2.1.2/src/psytricks/__ps1__/restricks-server.example.xml
--rw-r--r--   0        0        0    16072 2023-05-12 13:28:43.291864 psytricks-2.1.2/src/psytricks/__ps1__/restricks-server.ps1
--rw-r--r--   0        0        0     3014 2023-05-10 19:08:40.530093 psytricks-2.1.2/src/psytricks/__ps1__/sampledata/GetAccessUsers.json
--rw-r--r--   0        0        0    18009 2023-05-10 19:08:40.530093 psytricks-2.1.2/src/psytricks/__ps1__/sampledata/GetMachineStatus.json
--rw-r--r--   0        0        0     4623 2023-05-10 19:08:40.530093 psytricks-2.1.2/src/psytricks/__ps1__/sampledata/GetSessions.json
--rw-r--r--   0        0        0     5977 2023-05-12 16:25:07.522674 psytricks-2.1.2/src/psytricks/cli.py
--rw-r--r--   0        0        0     1880 2023-04-27 09:47:02.646410 psytricks-2.1.2/src/psytricks/decoder.py
--rw-r--r--   0        0        0      671 2023-05-10 19:08:40.530093 psytricks-2.1.2/src/psytricks/literals.py
--rw-r--r--   0        0        0     3516 2023-04-27 10:47:48.965859 psytricks-2.1.2/src/psytricks/mappings.py
--rw-r--r--   0        0        0    23720 2023-05-12 19:24:30.404582 psytricks-2.1.2/src/psytricks/wrapper.py
--rw-r--r--   0        0        0     8206 1970-01-01 00:00:00.000000 psytricks-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35059 2022-12-20 15:40:57.930292 psytricks-2.1.3/LICENSE
+-rw-r--r--   0        0        0     7868 2023-06-07 09:29:33.837553 psytricks-2.1.3/README.md
+-rw-r--r--   0        0        0     1112 2023-06-07 10:49:31.762388 psytricks-2.1.3/pyproject.toml
+-rw-r--r--   0        0        0       93 2023-06-07 10:49:31.762388 psytricks-2.1.3/src/psytricks/__init__.py
+-rw-r--r--   0        0        0     6146 2023-06-07 10:49:31.762388 psytricks-2.1.3/src/psytricks/__ps1__/psytricks-lib.ps1
+-rw-r--r--   0        0        0     6392 2023-05-10 19:08:40.530093 psytricks-2.1.3/src/psytricks/__ps1__/psytricks-wrapper.ps1
+-rw-r--r--   0        0        0     1961 2023-05-10 19:08:40.530093 psytricks-2.1.3/src/psytricks/__ps1__/restricks-server.example.xml
+-rw-r--r--   0        0        0    16072 2023-05-12 13:28:43.291864 psytricks-2.1.3/src/psytricks/__ps1__/restricks-server.ps1
+-rw-r--r--   0        0        0     3014 2023-05-10 19:08:40.530093 psytricks-2.1.3/src/psytricks/__ps1__/sampledata/GetAccessUsers.json
+-rw-r--r--   0        0        0    18009 2023-05-10 19:08:40.530093 psytricks-2.1.3/src/psytricks/__ps1__/sampledata/GetMachineStatus.json
+-rw-r--r--   0        0        0     4623 2023-05-10 19:08:40.530093 psytricks-2.1.3/src/psytricks/__ps1__/sampledata/GetSessions.json
+-rw-r--r--   0        0        0     5977 2023-05-12 16:25:07.522674 psytricks-2.1.3/src/psytricks/cli.py
+-rw-r--r--   0        0        0     1880 2023-04-27 09:47:02.646410 psytricks-2.1.3/src/psytricks/decoder.py
+-rw-r--r--   0        0        0      671 2023-05-10 19:08:40.530093 psytricks-2.1.3/src/psytricks/literals.py
+-rw-r--r--   0        0        0     3516 2023-04-27 10:47:48.965859 psytricks-2.1.3/src/psytricks/mappings.py
+-rw-r--r--   0        0        0    24284 2023-06-07 10:47:03.912474 psytricks-2.1.3/src/psytricks/wrapper.py
+-rw-r--r--   0        0        0     8805 1970-01-01 00:00:00.000000 psytricks-2.1.3/PKG-INFO
```

### Comparing `psytricks-2.1.2/LICENSE` & `psytricks-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.2/README.md` & `psytricks-2.1.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 To be very clear: performance of the wrapper script is abysmal, but this is *not
 at all* an issue for us. Abysmal, as in: for every wrapped call a full (new)
 PowerShell process needs to be instantiated, usually taking something like 1-2
 seconds. ⏳
 
 The REST interface provides a much better performance, at the cost of some
 additional setup. If you're happy to take on this approach, the package offers a
-very smooth experience. 🎢🎡
+very smooth ride. 🎢🎡
 
 ## 🛠🚧 Installation
 
 ### Prerequisites
 
 As mentioned above, the *Citrix Broker PowerShell Snap-In* is required to be
 installed on the machine that will run the wrapper script, since its commands
@@ -69,25 +69,32 @@
 point).
 
 To install the snap-in, look for an MSI package like this in the `Delivery
 Controller` or `XenDesktop` installation media and install it as usual:
 
 * `Broker_PowerShellSnapIn_x64.msi`
 
-### Installing the package
+### Installing the 🐍 package
 
-For installing `psytricks` please create a `venv`, then run:
+In case you're planning to use `psytricks` via the subprocess approach
+(discouraged but less components to set up), you will have to install the
+package itself on the Windows machine having the above mentioned *Snap-In*
+installed. For the `REST` approach (recommended) only the PowerShell service
+described in the section below has to run on that machine - the Python package
+can be installed on any computer that is able to talk to the `REST` service.
+
+For installing `psytricks` please create and activate a `venv`, then run:
 
 ```bash
 pip install psytricks
 ```
 
-This will also register the CLI tool `psytricks.exe` although that one is mostly
-meant for testing and demonstration purposes, otherwise the `*-Broker*` commands
-provided by the PowerShell snap-in could be used directly.
+NOTE: this will also register the `psytricks` CLI tool although that one is
+mostly meant for testing and demonstration purposes, otherwise the `*-Broker*`
+commands provided by the PowerShell snap-in could be used directly.
 
 ### Setting up the REST service
 
 The easiest way for installing the REST service is to use [WinSW (Windows
 Service Wrapper)][www_winsw] but you may choose anything you like to launch the
 server process like NSSM, Scheduled Tasks 📅, homegrown dark magic 🪄🔮 or
 others.
@@ -132,39 +139,42 @@
 anything that controls who / what can access the service will do the job.
 
 ## 🎪 What does it provide?
 
 To interact with CVAD, a wrapper object needs to be
 instantiated and instructed how to communicate with the stack.
 
-### Using the subprocess wrapper
-
-To create a wrapper object using the subprocess variant, a
-`psytricks.wrapper.PSyTricksWrapper` with the address of the *Delivery
-Controller* to connect to has to be instantiated, for example:
-
-```Python
-from psytricks.wrapper import PSyTricksWrapper
-
-wrapper = PSyTricksWrapper(deliverycontroller="cdc01.vdi.example.xy")
-```
-
 ### Using the REST service - *recommended*
 
 After setting up the REST service as described above and making sure to be able
 to connect to it (firewall rules, ssh tunnel, ...), a
 `psytricks.wrapper.ResTricksWrapper` object can be used while passing the URL
 under which the REST service is reachable, e.g.
 
 ```Python
 from psytricks.wrapper import ResTricksWrapper
 
 wrapper = ResTricksWrapper(base_url="http://localhost:8080/")
 ```
 
+### Using the subprocess wrapper - *use with caution*
+
+(This is only recommended for testing or if for some reason you don't want /
+can't set up the REST service.)
+
+To create a wrapper object using the subprocess variant, a
+`psytricks.wrapper.PSyTricksWrapper` with the address of the *Delivery
+Controller* to connect to has to be instantiated, for example:
+
+```Python
+from psytricks.wrapper import PSyTricksWrapper
+
+wrapper = PSyTricksWrapper(deliverycontroller="cdc01.vdi.example.xy")
+```
+
 ### Fetching status information
 
 The wrapper object can then be used to e.g. retrieve information on the machines
 controlled ("brokered") by Citrix:
 
 ```Python
 machines = wrapper.get_machine_status()
```

### Comparing `psytricks-2.1.2/pyproject.toml` & `psytricks-2.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 authors = ["Niko Ehrenfeuchter <nikolaus.ehrenfeuchter@unibas.ch>"]
 description = "PowerShell Python Citrix Tricks."
 documentation = "https://imcf.one/apidocs/psytricks/psytricks.html"
 license = "GPL-3.0-or-later"
 name = "psytricks"
 readme = "README.md"
-version = "2.1.2"
+version = "2.1.3"
 
 [tool.poetry.urls]
 "Changelog" = "https://github.com/imcf/psytricks/blob/main/CHANGELOG.md"
 "Organisation Homepage" = "https://imcf.one/"
 "Twitter" = "https://twitter.com/imcf_basel"
 
 [tool.poetry.dependencies]
```

### Comparing `psytricks-2.1.2/src/psytricks/__ps1__/psytricks-lib.ps1` & `psytricks-2.1.3/src/psytricks/__ps1__/psytricks-lib.ps1`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <#
 
 Collection of functions and other definitions to be sourced by other scripts.
 
 #>
 
 # the version variable will be filled by poetry at build time:
-$Version = "2.1.2"
+$Version = "2.1.3"
 
 
 #region properties-selectors
 
 $MachineProperties = @(
     "AgentVersion",
     "AssociatedUserUPNs",
```

### Comparing `psytricks-2.1.2/src/psytricks/__ps1__/psytricks-wrapper.ps1` & `psytricks-2.1.3/src/psytricks/__ps1__/psytricks-wrapper.ps1`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.2/src/psytricks/__ps1__/restricks-server.example.xml` & `psytricks-2.1.3/src/psytricks/__ps1__/restricks-server.example.xml`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.2/src/psytricks/__ps1__/restricks-server.ps1` & `psytricks-2.1.3/src/psytricks/__ps1__/restricks-server.ps1`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.2/src/psytricks/__ps1__/sampledata/GetAccessUsers.json` & `psytricks-2.1.3/src/psytricks/__ps1__/sampledata/GetAccessUsers.json`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.2/src/psytricks/__ps1__/sampledata/GetMachineStatus.json` & `psytricks-2.1.3/src/psytricks/__ps1__/sampledata/GetMachineStatus.json`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.2/src/psytricks/__ps1__/sampledata/GetSessions.json` & `psytricks-2.1.3/src/psytricks/__ps1__/sampledata/GetSessions.json`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.2/src/psytricks/cli.py` & `psytricks-2.1.3/src/psytricks/cli.py`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.2/src/psytricks/decoder.py` & `psytricks-2.1.3/src/psytricks/decoder.py`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.2/src/psytricks/literals.py` & `psytricks-2.1.3/src/psytricks/literals.py`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.2/src/psytricks/mappings.py` & `psytricks-2.1.3/src/psytricks/mappings.py`

 * *Files identical despite different names*

### Comparing `psytricks-2.1.2/src/psytricks/wrapper.py` & `psytricks-2.1.3/src/psytricks/wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -352,69 +352,82 @@
         self.base_url = base_url
         self.timeout = 5
         self.server_version = [0, 0, 0, 0]
         try:
             status = self.send_get_request("version")["Status"]
             log.trace(f"Server status: [{status}]")
             server_version = status["PSyTricksVersion"]
-            log.info(f"Server version: [{server_version}]")
 
-            log.success("Successfully tested connection 🔌 to ResTricks server 🆗")
+            log.success("Successfully connected 🔌 to ResTricks server 🆗")
             if verify:
                 version_matching = self.validate_version(server_version)
                 if not version_matching:
                     raise ValueError(f"Unexpected server version: {server_version}")
+            else:
+                log.warning(f"Skipping version check (server: {server_version})")
         except Exception as ex:  # pylint: disable-msg=broad-except
             if verify:
                 raise ConnectionError(f"Connecting to [{base_url}] failed!") from ex
 
         log.debug(f"Initialized {self.__class__.__name__}({base_url}) ✨")
 
     def validate_version(self, server_ver):
         """Validate the server version against the local module.
 
         Parse the version strings of the local module and the server response
         and compare them for equality (ignoring the 4th component, which may
         denote a pre- or development-release).
 
+        If the 3rd component (PATCH level) is differing a warning message will
+        be issued to the log but the method will still return True.
+
         Parameters
         ----------
         server_ver : dict
             The dict parsed from the JSON response when sending a `version` GET
             request to the server.
 
         Returns
         -------
         bool
-            True in case the versions are matching, False otherwise.
+            True in case the versions are matching (at least MAJOR and MINOR
+            levels), False otherwise.
         """
 
         def parse_ver(ver):
             log.trace(f"Parsing version string: [{ver}]")
-            _split = ver.split(".")
-            version = [int(x) for x in _split[:3]]
-            version.append(0)
-            if len(_split) > 3:
-                # the 4th component is usually a string, so do not cast it if present:
-                version[3] = _split[3]
+            # pre / alpha versions are separated by a dash "-" char according to
+            # semantic versioning rules (use "0" if no dash is present):
+            pre = 0
+            if "-" in ver:
+                ver, pre = ver.split("-")
+
+            version = [int(x) for x in ver.split(".")]
+            version.append(pre)
+            log.trace(f"Parsed version: {version}")
             return version
 
         try:
             self.server_version = parse_ver(server_ver)
-            log.info(f"Server version: {self.server_version} 🪪")
+            log.debug(f"Server version: {self.server_version} 🪪")
         except Exception as ex:  # pylint: disable-msg=broad-except
             log.warning(f"Unable to parse server version [{server_ver}]: {ex}")
             return False
 
         client_version = parse_ver(__version__)
-        log.info(f"Client version: {client_version} 🪪")
+        log.debug(f"Client version: {client_version} 🪪")
 
         # compare versions, ignoring the 4th component (dev/pre/alpha/...)
         if client_version[:3] == self.server_version[:3]:
-            log.success("Versions are matching! 🏅")
+            log.info("Versions are matching! 🏅")
+            return True
+
+        # be lenient on patch-level mismatches (but issue a warning message)
+        if client_version[:2] == self.server_version[:2]:
+            log.warning("Versions are differing in PATCH level! 🔍")
             return True
 
         log.error("Version mismatch! 🧨")
         return False
 
     @staticmethod
     def _check_response(response):
```

### Comparing `psytricks-2.1.2/PKG-INFO` & `psytricks-2.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psytricks
-Version: 2.1.2
+Version: 2.1.3
 Summary: PowerShell Python Citrix Tricks.
 License: GPL-3.0-or-later
 Author: Niko Ehrenfeuchter
 Author-email: nikolaus.ehrenfeuchter@unibas.ch
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
@@ -71,15 +71,15 @@
 To be very clear: performance of the wrapper script is abysmal, but this is *not
 at all* an issue for us. Abysmal, as in: for every wrapped call a full (new)
 PowerShell process needs to be instantiated, usually taking something like 1-2
 seconds. ⏳
 
 The REST interface provides a much better performance, at the cost of some
 additional setup. If you're happy to take on this approach, the package offers a
-very smooth experience. 🎢🎡
+very smooth ride. 🎢🎡
 
 ## 🛠🚧 Installation
 
 ### Prerequisites
 
 As mentioned above, the *Citrix Broker PowerShell Snap-In* is required to be
 installed on the machine that will run the wrapper script, since its commands
@@ -91,25 +91,32 @@
 point).
 
 To install the snap-in, look for an MSI package like this in the `Delivery
 Controller` or `XenDesktop` installation media and install it as usual:
 
 * `Broker_PowerShellSnapIn_x64.msi`
 
-### Installing the package
+### Installing the 🐍 package
 
-For installing `psytricks` please create a `venv`, then run:
+In case you're planning to use `psytricks` via the subprocess approach
+(discouraged but less components to set up), you will have to install the
+package itself on the Windows machine having the above mentioned *Snap-In*
+installed. For the `REST` approach (recommended) only the PowerShell service
+described in the section below has to run on that machine - the Python package
+can be installed on any computer that is able to talk to the `REST` service.
+
+For installing `psytricks` please create and activate a `venv`, then run:
 
 ```bash
 pip install psytricks
 ```
 
-This will also register the CLI tool `psytricks.exe` although that one is mostly
-meant for testing and demonstration purposes, otherwise the `*-Broker*` commands
-provided by the PowerShell snap-in could be used directly.
+NOTE: this will also register the `psytricks` CLI tool although that one is
+mostly meant for testing and demonstration purposes, otherwise the `*-Broker*`
+commands provided by the PowerShell snap-in could be used directly.
 
 ### Setting up the REST service
 
 The easiest way for installing the REST service is to use [WinSW (Windows
 Service Wrapper)][www_winsw] but you may choose anything you like to launch the
 server process like NSSM, Scheduled Tasks 📅, homegrown dark magic 🪄🔮 or
 others.
@@ -154,39 +161,42 @@
 anything that controls who / what can access the service will do the job.
 
 ## 🎪 What does it provide?
 
 To interact with CVAD, a wrapper object needs to be
 instantiated and instructed how to communicate with the stack.
 
-### Using the subprocess wrapper
-
-To create a wrapper object using the subprocess variant, a
-`psytricks.wrapper.PSyTricksWrapper` with the address of the *Delivery
-Controller* to connect to has to be instantiated, for example:
-
-```Python
-from psytricks.wrapper import PSyTricksWrapper
-
-wrapper = PSyTricksWrapper(deliverycontroller="cdc01.vdi.example.xy")
-```
-
 ### Using the REST service - *recommended*
 
 After setting up the REST service as described above and making sure to be able
 to connect to it (firewall rules, ssh tunnel, ...), a
 `psytricks.wrapper.ResTricksWrapper` object can be used while passing the URL
 under which the REST service is reachable, e.g.
 
 ```Python
 from psytricks.wrapper import ResTricksWrapper
 
 wrapper = ResTricksWrapper(base_url="http://localhost:8080/")
 ```
 
+### Using the subprocess wrapper - *use with caution*
+
+(This is only recommended for testing or if for some reason you don't want /
+can't set up the REST service.)
+
+To create a wrapper object using the subprocess variant, a
+`psytricks.wrapper.PSyTricksWrapper` with the address of the *Delivery
+Controller* to connect to has to be instantiated, for example:
+
+```Python
+from psytricks.wrapper import PSyTricksWrapper
+
+wrapper = PSyTricksWrapper(deliverycontroller="cdc01.vdi.example.xy")
+```
+
 ### Fetching status information
 
 The wrapper object can then be used to e.g. retrieve information on the machines
 controlled ("brokered") by Citrix:
 
 ```Python
 machines = wrapper.get_machine_status()
```

