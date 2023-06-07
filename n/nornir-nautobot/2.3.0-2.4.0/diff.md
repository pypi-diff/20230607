# Comparing `tmp/nornir_nautobot-2.3.0.tar.gz` & `tmp/nornir_nautobot-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nornir_nautobot-2.3.0.tar", max compression
+gzip compressed data, was "nornir_nautobot-2.4.0.tar", max compression
```

## Comparing `nornir_nautobot-2.3.0.tar` & `nornir_nautobot-2.4.0.tar`

### file list

```diff
@@ -1,22 +1,25 @@
--rw-r--r--   0        0        0     1426 2022-10-28 21:57:42.350245 nornir_nautobot-2.3.0/README.md
--rw-r--r--   0        0        0       33 2022-10-28 21:57:42.350245 nornir_nautobot-2.3.0/nornir_nautobot/__init__.py
--rw-r--r--   0        0        0      126 2022-10-28 21:57:42.350245 nornir_nautobot-2.3.0/nornir_nautobot/exceptions.py
--rw-r--r--   0        0        0       33 2022-10-28 21:57:42.350245 nornir_nautobot-2.3.0/nornir_nautobot/plugins/__init__.py
--rw-r--r--   0        0        0       33 2022-10-28 21:57:42.350245 nornir_nautobot-2.3.0/nornir_nautobot/plugins/inventory/__init__.py
--rw-r--r--   0        0        0     5627 2022-10-28 21:57:42.350245 nornir_nautobot-2.3.0/nornir_nautobot/plugins/inventory/nautobot.py
--rw-r--r--   0        0        0     2667 2022-10-28 21:57:42.350245 nornir_nautobot-2.3.0/nornir_nautobot/plugins/processors/__init__.py
--rw-r--r--   0        0        0     5355 2022-10-28 21:57:42.350245 nornir_nautobot-2.3.0/nornir_nautobot/plugins/processors/get_config.py
--rw-r--r--   0        0        0     2750 2022-10-28 21:57:42.350245 nornir_nautobot-2.3.0/nornir_nautobot/plugins/tasks/dispatcher/__init__.py
--rw-r--r--   0        0        0      248 2022-10-28 21:57:42.350245 nornir_nautobot-2.3.0/nornir_nautobot/plugins/tasks/dispatcher/arista_eos.py
--rw-r--r--   0        0        0      217 2022-10-28 21:57:42.354245 nornir_nautobot-2.3.0/nornir_nautobot/plugins/tasks/dispatcher/cisco_asa.py
--rw-r--r--   0        0        0      217 2022-10-28 21:57:42.354245 nornir_nautobot-2.3.0/nornir_nautobot/plugins/tasks/dispatcher/cisco_ios.py
--rw-r--r--   0        0        0      223 2022-10-28 21:57:42.354245 nornir_nautobot-2.3.0/nornir_nautobot/plugins/tasks/dispatcher/cisco_ios_xr.py
--rw-r--r--   0        0        0      219 2022-10-28 21:57:42.354245 nornir_nautobot-2.3.0/nornir_nautobot/plugins/tasks/dispatcher/cisco_nxos.py
--rw-r--r--   0        0        0    12481 2022-10-28 21:57:42.354245 nornir_nautobot-2.3.0/nornir_nautobot/plugins/tasks/dispatcher/default.py
--rw-r--r--   0        0        0      263 2022-10-28 21:57:42.354245 nornir_nautobot-2.3.0/nornir_nautobot/plugins/tasks/dispatcher/juniper_junos.py
--rw-r--r--   0        0        0      434 2022-10-28 21:57:42.354245 nornir_nautobot-2.3.0/nornir_nautobot/utils/helpers.py
--rw-r--r--   0        0        0     2037 2022-10-28 21:57:42.354245 nornir_nautobot-2.3.0/nornir_nautobot/utils/logger.py
--rw-r--r--   0        0        0      913 2022-10-28 21:57:42.354245 nornir_nautobot-2.3.0/nornir_nautobot/utils/mock.py
--rw-r--r--   0        0        0     2491 2022-10-28 21:57:51.394353 nornir_nautobot-2.3.0/pyproject.toml
--rw-r--r--   0        0        0     2656 1970-01-01 00:00:00.000000 nornir_nautobot-2.3.0/setup.py
--rw-r--r--   0        0        0     2880 1970-01-01 00:00:00.000000 nornir_nautobot-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1743 2023-06-07 15:16:40.651064 nornir_nautobot-2.4.0/README.md
+-rw-r--r--   0        0        0       33 2023-06-07 15:16:40.655064 nornir_nautobot-2.4.0/nornir_nautobot/__init__.py
+-rw-r--r--   0        0        0      126 2023-06-07 15:16:40.655064 nornir_nautobot-2.4.0/nornir_nautobot/exceptions.py
+-rw-r--r--   0        0        0       33 2023-06-07 15:16:40.655064 nornir_nautobot-2.4.0/nornir_nautobot/plugins/__init__.py
+-rw-r--r--   0        0        0       33 2023-06-07 15:16:40.655064 nornir_nautobot-2.4.0/nornir_nautobot/plugins/inventory/__init__.py
+-rw-r--r--   0        0        0     5627 2023-06-07 15:16:40.655064 nornir_nautobot-2.4.0/nornir_nautobot/plugins/inventory/nautobot.py
+-rw-r--r--   0        0        0     2667 2023-06-07 15:16:40.655064 nornir_nautobot-2.4.0/nornir_nautobot/plugins/processors/__init__.py
+-rw-r--r--   0        0        0     5355 2023-06-07 15:16:40.655064 nornir_nautobot-2.4.0/nornir_nautobot/plugins/processors/get_config.py
+-rw-r--r--   0        0        0     3647 2023-06-07 15:16:40.655064 nornir_nautobot-2.4.0/nornir_nautobot/plugins/tasks/dispatcher/__init__.py
+-rw-r--r--   0        0        0      281 2023-06-07 15:16:40.655064 nornir_nautobot-2.4.0/nornir_nautobot/plugins/tasks/dispatcher/arista_eos.py
+-rw-r--r--   0        0        0      250 2023-06-07 15:16:40.655064 nornir_nautobot-2.4.0/nornir_nautobot/plugins/tasks/dispatcher/cisco_asa.py
+-rw-r--r--   0        0        0      250 2023-06-07 15:16:40.655064 nornir_nautobot-2.4.0/nornir_nautobot/plugins/tasks/dispatcher/cisco_ios.py
+-rw-r--r--   0        0        0      256 2023-06-07 15:16:40.655064 nornir_nautobot-2.4.0/nornir_nautobot/plugins/tasks/dispatcher/cisco_ios_xr.py
+-rw-r--r--   0        0        0      252 2023-06-07 15:16:40.655064 nornir_nautobot-2.4.0/nornir_nautobot/plugins/tasks/dispatcher/cisco_nxos.py
+-rw-r--r--   0        0        0    17833 2023-06-07 15:16:40.655064 nornir_nautobot-2.4.0/nornir_nautobot/plugins/tasks/dispatcher/default.py
+-rw-r--r--   0        0        0      320 2023-06-07 15:16:40.655064 nornir_nautobot-2.4.0/nornir_nautobot/plugins/tasks/dispatcher/juniper_junos.py
+-rw-r--r--   0        0        0     4219 2023-06-07 15:16:40.655064 nornir_nautobot-2.4.0/nornir_nautobot/plugins/tasks/dispatcher/mikrotik_routeros.py
+-rw-r--r--   0        0        0     6214 2023-06-07 15:16:40.655064 nornir_nautobot-2.4.0/nornir_nautobot/plugins/tasks/dispatcher/mikrotik_routeros_api.py
+-rw-r--r--   0        0        0      299 2023-06-07 15:16:40.655064 nornir_nautobot-2.4.0/nornir_nautobot/plugins/tasks/dispatcher/ruckus_fastiron.py
+-rw-r--r--   0        0        0     9095 2023-06-07 15:16:40.655064 nornir_nautobot-2.4.0/nornir_nautobot/plugins/tasks/dispatcher/ruckus_smartzone_api.py
+-rw-r--r--   0        0        0      434 2023-06-07 15:16:40.655064 nornir_nautobot-2.4.0/nornir_nautobot/utils/helpers.py
+-rw-r--r--   0        0        0     2119 2023-06-07 15:16:40.655064 nornir_nautobot-2.4.0/nornir_nautobot/utils/logger.py
+-rw-r--r--   0        0        0      913 2023-06-07 15:16:40.655064 nornir_nautobot-2.4.0/nornir_nautobot/utils/mock.py
+-rw-r--r--   0        0        0     2793 2023-06-07 15:16:52.463087 nornir_nautobot-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3104 1970-01-01 00:00:00.000000 nornir_nautobot-2.4.0/PKG-INFO
```

### Comparing `nornir_nautobot-2.3.0/nornir_nautobot/plugins/inventory/nautobot.py` & `nornir_nautobot-2.4.0/nornir_nautobot/plugins/inventory/nautobot.py`

 * *Files identical despite different names*

### Comparing `nornir_nautobot-2.3.0/nornir_nautobot/plugins/processors/__init__.py` & `nornir_nautobot-2.4.0/nornir_nautobot/plugins/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `nornir_nautobot-2.3.0/nornir_nautobot/plugins/processors/get_config.py` & `nornir_nautobot-2.4.0/nornir_nautobot/plugins/processors/get_config.py`

 * *Files identical despite different names*

### Comparing `nornir_nautobot-2.3.0/nornir_nautobot/plugins/tasks/dispatcher/__init__.py` & `nornir_nautobot-2.4.0/nornir_nautobot/plugins/tasks/dispatcher/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,14 +14,19 @@
     "default_netmiko": "nornir_nautobot.plugins.tasks.dispatcher.default.NetmikoNautobotNornirDriver",
     "cisco_asa": "nornir_nautobot.plugins.tasks.dispatcher.cisco_asa.NautobotNornirDriver",
     "cisco_nxos": "nornir_nautobot.plugins.tasks.dispatcher.cisco_nxos.NautobotNornirDriver",
     "cisco_ios": "nornir_nautobot.plugins.tasks.dispatcher.cisco_ios.NautobotNornirDriver",
     "cisco_xr": "nornir_nautobot.plugins.tasks.dispatcher.cisco_ios_xr.NautobotNornirDriver",
     "juniper_junos": "nornir_nautobot.plugins.tasks.dispatcher.juniper_junos.NautobotNornirDriver",
     "arista_eos": "nornir_nautobot.plugins.tasks.dispatcher.arista_eos.NautobotNornirDriver",
+    "mikrotik_routeros_api": "nornir_nautobot.plugins.tasks.dispatcher.mikrotik_routeros_api.NautobotNornirDriver",
+    "ruckus_fastiron": "nornir_nautobot.plugins.tasks.dispatcher.ruckus_fastiron.NautobotNornirDriver",
+    "mikrotik_routeros": "nornir_nautobot.plugins.tasks.dispatcher.mikrotik_routeros.NautobotNornirDriver",
+    "ruckus_smartzone_api": "nornir_nautobot.plugins.tasks.dispatcher.ruckus_smartzone_api.NautobotNornirDriver",
+    "ruckus_access_point": "nornir_nautobot.plugins.tasks.dispatcher.ruckus_smartzone_api.NautobotNornirDriver",
 }
 
 
 def dispatcher(task: Task, method: str, logger, obj, *args, **kwargs) -> Result:
     """Helper Task to retrieve a given Nornir task for a given platform.
 
     Args:
@@ -40,29 +45,33 @@
     logger.log_debug(f"Executing dispatcher for {task.host.name} ({task.host.platform})")
 
     # Get the platform specific driver, if not available, get the default driver
     driver = default_drivers_mapping.get(task.host.platform, default_drivers_mapping.get("default"))
     logger.log_debug(f"Found driver {driver}")
 
     if not driver:
-        logger.log_failure(obj, f"Unable to find the driver for {method} for platform: {task.host.platform}")
-        raise NornirNautobotException()
+        logger.log_failure(
+            obj, f"Unable to find the driver for {method} for platform: {task.host.platform}, preemptively failed."
+        )
+        raise NornirNautobotException(
+            f"Unable to find the driver for {method} for platform: {task.host.platform}, preemptively failed."
+        )
 
     module_name, class_name = driver.rsplit(".", 1)
     driver_class = getattr(importlib.import_module(module_name), class_name)
 
     if not driver_class:
-        logger.log_failure(obj, f"Unable to locate the class {driver}")
-        raise NornirNautobotException()
+        logger.log_failure(obj, f"Unable to locate the class {driver}, preemptively failed.")
+        raise NornirNautobotException(f"Unable to locate the class {driver}, preemptively failed.")
 
     try:
         driver_task = getattr(driver_class, method)
     except AttributeError:
-        logger.log_failure(obj, f"Unable to locate the method {method} for {driver}")
-        raise NornirNautobotException()
+        logger.log_failure(obj, f"Unable to locate the method {method} for {driver}, preemptively failed.")
+        raise NornirNautobotException(f"Unable to locate the method {method} for {driver}, preemptively failed.")
 
     result = task.run(task=driver_task, logger=logger, obj=obj, *args, **kwargs)
 
     return Result(
         host=task.host,
         result=result,
     )
```

### Comparing `nornir_nautobot-2.3.0/nornir_nautobot/plugins/tasks/dispatcher/default.py` & `nornir_nautobot-2.4.0/nornir_nautobot/plugins/tasks/dispatcher/default.py`

 * *Files 27% similar despite different names*

```diff
@@ -16,35 +16,30 @@
 from netutils.config.compliance import compliance
 from netutils.dns import is_fqdn_resolvable
 from netutils.ip import is_ip
 from netutils.ping import tcp_ping
 from nornir.core.exceptions import NornirSubTaskError
 from nornir.core.task import Result, Task
 from nornir_jinja2.plugins.tasks import template_file
-from nornir_napalm.plugins.tasks import napalm_get
+from nornir_napalm.plugins.tasks import napalm_get, napalm_configure
 from nornir_netmiko.tasks import netmiko_send_command
 
 from nornir_nautobot.exceptions import NornirNautobotException
 from nornir_nautobot.utils.helpers import make_folder
 
-RUN_COMMAND_MAPPING = {
-    "default": "show run",
-    "cisco_nxos": "show run",
-    "cisco_ios": "show run",
-    "cisco_xr": "show run",
-    "juniper_junos": "show configuration | display set",
-    "arista_eos": "show run",
-}
-
 
 class NautobotNornirDriver:
     """Default collection of Nornir Tasks based on Napalm."""
 
-    @staticmethod
-    def get_config(task: Task, logger, obj, backup_file: str, remove_lines: list, substitute_lines: list) -> Result:
+    config_command = "show run"
+
+    @classmethod
+    def get_config(
+        cls, task: Task, logger, obj, backup_file: str, remove_lines: list, substitute_lines: list
+    ) -> Result:
         """Get the latest configuration from the device.
 
         Args:
             task (Task): Nornir Task.
             logger (NornirLogger): Custom NornirLogger object to reflect job results (via Nautobot Jobs) and Python logger.
             obj (Device): A Nautobot Device Django ORM object instance.
             backup_file (str): The file location of where the back configuration should be saved.
@@ -57,19 +52,23 @@
         """
         logger.log_debug(f"Executing get_config for {task.host.name} on {task.host.platform}")
 
         # TODO: Find standard napalm exceptions and account for them
         try:
             result = task.run(task=napalm_get, getters=["config"], retrieve="running")
         except NornirSubTaskError as exc:
-            logger.log_failure(obj, f"Failed with a unknown issue. `{exc.result.exception}`")
-            raise NornirNautobotException()
+            logger.log_failure(obj, f"`get_config` method failed with an unexpected issue: `{exc.result.exception}`")
+            raise NornirNautobotException(
+                "`get_config` method failed with an unexpected issue: `{exc.result.exception}`"
+            )
 
         if result[0].failed:
-            logger.log_failure(obj, f"Failed with a unknown issue. `{str(result.exception)}`")
+            logger.log_failure(
+                obj, f"`get_config` nornir task failed with an unexpected issue: `{str(result.exception)}`"
+            )
             return result
 
         running_config = result[0].result.get("config", {}).get("running", None)
         if remove_lines:
             logger.log_debug("Removing lines from configuration based on `remove_lines` definition")
             running_config = clean_config(running_config, remove_lines)
 
@@ -95,23 +94,23 @@
         Returns:
             Result: Nornir Result object.
         """
         if is_ip(task.host.hostname):
             ip_addr = task.host.hostname
         else:
             if not is_fqdn_resolvable(task.host.hostname):
-                logger.log_failure(obj, "not an IP or resolvable.")
-                raise NornirNautobotException("not an IP or resolvable.")
+                logger.log_failure(obj, "There was not an IP or resolvable, preemptively failed.")
+                raise NornirNautobotException("There was not an IP or resolvable, preemptively failed.")
             ip_addr = socket.gethostbyname(task.host.hostname)
 
         # TODO: Allow port to be configurable
         port = 22
         if not tcp_ping(ip_addr, port):
-            logger.log_failure(obj, f"Attempting to connect to IP: {ip_addr} and port: {port} failed.")
-            raise NornirNautobotException(f"Attempting to connect to IP: {ip_addr} and port: {port} failed.")
+            logger.log_failure(obj, f"Could not connect to IP: {ip_addr} and port: {port}, preemptively failed.")
+            raise NornirNautobotException(f"Could not connect to IP: {ip_addr} and port: {port}, preemptively failed.")
         if not task.host.username:
             logger.log_failure(obj, "There was no username defined, preemptively failed.")
             raise NornirNautobotException("There was no username defined, preemptively failed.")
         if not task.host.password:
             logger.log_failure(obj, "There was no password defined, preemptively failed.")
             raise NornirNautobotException("There was no password defined, preemptively failed.")
 
@@ -132,26 +131,30 @@
             intended_file (str):  The file location of where the intended configuration should be saved.
             platform (str): The platform slug of the device.
 
         Returns:
             Result: Nornir Result object with a feature_data key of the compliance data.
         """
         if not os.path.exists(backup_file):
-            logger.log_failure(obj, f"Backup file Not Found at location: `{backup_file}`")
-            raise NornirNautobotException()
+            logger.log_failure(obj, f"Backup file Not Found at location: `{backup_file}`, preemptively failed.")
+            raise NornirNautobotException(f"Backup file Not Found at location: `{backup_file}`, preemptively failed.")
 
         if not os.path.exists(intended_file):
-            logger.log_failure(obj, f"Intended config file NOT Found at location: `{intended_file}`")
-            raise NornirNautobotException()
+            logger.log_failure(
+                obj, f"Intended config file NOT Found at location: `{intended_file}`, preemptively failed."
+            )
+            raise NornirNautobotException(
+                f"Intended config file NOT Found at location: `{intended_file}`, preemptively failed."
+            )
 
         try:
             feature_data = compliance(features, backup_file, intended_file, platform)
         except Exception as error:  # pylint: disable=broad-except
             logger.log_failure(obj, f"UNKNOWN Failure of: {str(error)}")
-            raise NornirNautobotException()
+            raise NornirNautobotException(f"UNKNOWN Failure of: {str(error)}")
         return Result(host=task.host, result={"feature_data": feature_data})
 
     @staticmethod
     def generate_config(
         task: Task,
         logger,
         obj,
@@ -184,88 +187,196 @@
             )[0].result
         except NornirSubTaskError as exc:
             if isinstance(exc.result.exception, jinja2.exceptions.UndefinedError):  # pylint: disable=no-else-raise
                 logger.log_failure(
                     obj,
                     f"There was a jinja2.exceptions.UndefinedError error: ``{str(exc.result.exception)}``",
                 )
-                raise NornirNautobotException()
+                raise NornirNautobotException(
+                    f"There was a jinja2.exceptions.UndefinedError error: ``{str(exc.result.exception)}``"
+                )
             elif isinstance(exc.result.exception, jinja2.TemplateSyntaxError):
                 logger.log_failure(
                     obj,
                     f"There was a jinja2.TemplateSyntaxError error: ``{str(exc.result.exception)}``",
                 )
-                raise NornirNautobotException()
+                raise NornirNautobotException(
+                    f"There was a jinja2.TemplateSyntaxError error: ``{str(exc.result.exception)}``"
+                )
             elif isinstance(exc.result.exception, jinja2.TemplateNotFound):
                 logger.log_failure(
                     obj,
                     f"There was an issue finding the template and a jinja2.TemplateNotFound error was raised: ``{str(exc.result.exception)}``",
                 )
-                raise NornirNautobotException()
+                raise NornirNautobotException(
+                    f"There was an issue finding the template and a jinja2.TemplateNotFound error was raised: ``{str(exc.result.exception)}``"
+                )
             elif isinstance(exc.result.exception, jinja2.TemplateError):
                 logger.log_failure(obj, f"There was an issue general Jinja error: ``{str(exc.result.exception)}``")
-                raise NornirNautobotException()
+                raise NornirNautobotException(
+                    f"There was an issue general Jinja error: ``{str(exc.result.exception)}``"
+                )
             raise
 
         make_folder(os.path.dirname(output_file_location))
         with open(output_file_location, "w", encoding="utf8") as filehandler:
             filehandler.write(filled_template)
         return Result(host=task.host, result={"config": filled_template})
 
+    @staticmethod
+    def _remove_lines(logger, _running_config: str, remove_lines: list) -> str:
+        """Removes lines in configuration as specified in Remove Lines list.
+
+        Args:
+            logger (NornirLogger): Custom NornirLogger object to reflect job results (via Nautobot Jobs) and Python logger.
+            _running_config (str): a device running configuration.
+            remove_lines (list): A list of regex lines to remove configurations.
+
+        Returns:
+            Result: Clean running configuration if remove lines set.
+        """
+        if not remove_lines:
+            return _running_config
+        logger.log_debug("Removing lines from configuration based on `remove_lines` definition")
+        return clean_config(_running_config, remove_lines)
+
+    @staticmethod
+    def _substitute_lines(logger, _running_config: str, substitute_lines: list) -> str:
+        """Substitutes lines in configuration as specified in substitute Lines list.
+
+        Args:
+            logger (NornirLogger): Custom NornirLogger object to reflect job results (via Nautobot Jobs) and Python logger.
+            _running_config (str): a device running configuration.
+            substitute_lines (list): A list of dictionaries with to remove and replace lines.
+
+        Returns:
+            Result: running configuration with substitutions.
+        """
+        if not substitute_lines:
+            return _running_config
+        logger.log_debug("Substitute lines from configuration based on `substitute_lines` definition")
+        return sanitize_config(_running_config, substitute_lines)
+
+    @staticmethod
+    def _save_file(logger, backup_file: str, _running_config: str) -> None:
+        """Saves Running Configuration to a specified file.
+
+        Args:
+            logger (NornirLogger): Custom NornirLogger object to reflect job results (via Nautobot Jobs) and Python logger.
+            _running_config (str): a device running configuration.
+            backup_file (str): String representing backup file path.
+
+        Returns:
+            Result: Running Config is saved into backup file path.
+        """
+        make_folder(os.path.dirname(backup_file))
+        logger.log_debug(f"Saving Configuration to file: {backup_file}")
+        with open(backup_file, "w", encoding="utf8") as filehandler:
+            filehandler.write(_running_config)
+
 
 class NetmikoNautobotNornirDriver(NautobotNornirDriver):
     """Default collection of Nornir Tasks based on Netmiko."""
 
-    @staticmethod
-    def get_config(task: Task, logger, obj, backup_file: str, remove_lines: list, substitute_lines: list) -> Result:
+    config_command = "show run"
+
+    @classmethod
+    def get_config(
+        cls, task: Task, logger, obj, backup_file: str, remove_lines: list, substitute_lines: list
+    ) -> Result:
         """Get the latest configuration from the device using Netmiko.
 
         Args:
             task (Task): Nornir Task.
             logger (NornirLogger): Custom NornirLogger object to reflect job results (via Nautobot Jobs) and Python logger.
             obj (Device): A Nautobot Device Django ORM object instance.
             remove_lines (list): A list of regex lines to remove configurations.
             substitute_lines (list): A list of dictionaries with to remove and replace lines.
 
         Returns:
             Result: Nornir Result object with a dict as a result containing the running configuration
                 { "config: <running configuration> }
         """
         logger.log_debug(f"Executing get_config for {task.host.name} on {task.host.platform}")
-        command = RUN_COMMAND_MAPPING.get(task.host.platform, RUN_COMMAND_MAPPING["default"])
+        command = cls.config_command
 
         try:
             result = task.run(task=netmiko_send_command, command_string=command)
         except NornirSubTaskError as exc:
             if isinstance(exc.result.exception, NetmikoAuthenticationException):
                 logger.log_failure(obj, f"Failed with an authentication issue: `{exc.result.exception}`")
-                raise NornirNautobotException()
+                raise NornirNautobotException(f"Failed with an authentication issue: `{exc.result.exception}`")
 
             if isinstance(exc.result.exception, NetmikoTimeoutException):
                 logger.log_failure(obj, f"Failed with a timeout issue. `{exc.result.exception}`")
-                raise NornirNautobotException()
+                raise NornirNautobotException(f"Failed with a timeout issue. `{exc.result.exception}`")
 
             logger.log_failure(obj, f"Failed with an unknown issue. `{exc.result.exception}`")
-            raise NornirNautobotException()
+            raise NornirNautobotException(f"Failed with an unknown issue. `{exc.result.exception}`")
 
         if result[0].failed:
             return result
 
         running_config = result[0].result
 
         # Primarily seen in Cisco devices.
         if "ERROR: % Invalid input detected at" in running_config:
             logger.log_failure(obj, "Discovered `ERROR: % Invalid input detected at` in the output")
-            raise NornirNautobotException()
+            raise NornirNautobotException("Discovered `ERROR: % Invalid input detected at` in the output")
 
         if remove_lines:
             logger.log_debug("Removing lines from configuration based on `remove_lines` definition")
             running_config = clean_config(running_config, remove_lines)
         if substitute_lines:
             logger.log_debug("Substitute lines from configuration based on `substitute_lines` definition")
             running_config = sanitize_config(running_config, substitute_lines)
 
         make_folder(os.path.dirname(backup_file))
 
         with open(backup_file, "w", encoding="utf8") as filehandler:
             filehandler.write(running_config)
         return Result(host=task.host, result={"config": running_config})
+
+    @staticmethod
+    def provision_config(
+        task: Task,
+        logger,
+        obj,
+        config: str,
+    ) -> Result:
+        """Push candidate configuration to the device.
+
+        Args:
+            task (Task): Nornir Task.
+            logger (NornirLogger): Custom NornirLogger object to reflect job_results (via Nautobot Jobs) and Python logger.
+            obj (Device): A Nautobot Device Django ORM object instance.
+            config (str): The candidate config.
+
+        Raises:
+            NornirNautobotException: Authentication error.
+            NornirNautobotException: Timeout error.
+            NornirNautobotException: Other exception.
+
+        Returns:
+            Result: Nornir Result object with a dict as a result containing the running configuration
+                { "config: <running configuration> }
+        """
+        logger.log_success(obj, "Config provision starting")
+        # Sending None to napalm_configure for revert_in will disable it, so we don't want a default value.
+        revert_in = os.getenv("NORNIR_NAUTOBOT_REVERT_IN_SECONDS")
+        if revert_in is not None:
+            revert_in = int(revert_in)
+
+        try:
+            push_result = task.run(
+                task=napalm_configure,
+                configuration=config,
+                replace=True,
+                revert_in=revert_in,
+            )
+        except NornirSubTaskError as exc:
+            logger.log_failure(obj, f"Failed with an unknown issue. `{exc.result.exception}`")
+            raise NornirNautobotException()
+
+        logger.log_success(obj, f"result: {push_result[0].result}, changed: {push_result.changed}")
+        logger.log_success(obj, "Config provision ended")
+        return Result(host=task.host, result={"changed": push_result.changed, "result": push_result[0].result})
```

### Comparing `nornir_nautobot-2.3.0/nornir_nautobot/utils/logger.py` & `nornir_nautobot-2.4.0/nornir_nautobot/utils/logger.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,50 +1,52 @@
 """Provide logging facility for Nautobot/Python usage."""
 
 import logging
 
+from typing import Any
+
 
 class NornirLogger:
     """Similar to a mixin, to utilize Python logging and Jobs Result obj."""
 
-    def __init__(self, name, nautobot_job=None, debug=False, job_result=None):
+    def __init__(self, name: str, nautobot_job=None, debug: bool = False, job_result=None):
         """Initialize the object."""
         self.job_result = job_result or nautobot_job
         self.logger = logging.getLogger(name)
         self.debug = debug
         self.nautobot_job = nautobot_job or job_result
         if job_result is not None:
             log_message = (
                 "The arg named `job_result` has been renamed to `nautobot_job`; please update to use this name."
             )
             self.logger.warning(log_message)
             job_result.log_warning(log_message)
 
-    def log_debug(self, message):
+    def log_debug(self, message: str):
         """Debug, does not take obj, and only logs to jobs result when in global debug mode."""
         if self.nautobot_job and self.debug:
             self.nautobot_job.log_debug(message)
         self.logger.debug(message)
 
-    def log_info(self, obj, message):
+    def log_info(self, obj: Any, message: str):
         """Log to Python logger and jogs results for info messages."""
         if self.nautobot_job:
             self.nautobot_job.log_info(obj, message)
         self.logger.info("%s | %s", str(obj), message)
 
-    def log_success(self, obj, message):
+    def log_success(self, obj: Any, message: str):
         """Log to Python logger and jogs results for success messages."""
         if self.nautobot_job:
             self.nautobot_job.log_success(obj, message)
         self.logger.info("%s | %s", str(obj), message)
 
-    def log_warning(self, obj, message):
+    def log_warning(self, obj: Any, message: str):
         """Log to Python logger and jogs results for warning messages."""
         if self.nautobot_job:
             self.nautobot_job.log_warning(obj, message)
         self.logger.warning("%s | %s", str(obj), message)
 
-    def log_failure(self, obj, message):
+    def log_failure(self, obj: Any, message: str):
         """Log to Python logger and jogs results for failure messages."""
         if self.nautobot_job:
             self.nautobot_job.log_failure(obj, message)
         self.logger.error("%s | %s", str(obj), message)
```

### Comparing `nornir_nautobot-2.3.0/nornir_nautobot/utils/mock.py` & `nornir_nautobot-2.4.0/nornir_nautobot/utils/mock.py`

 * *Files identical despite different names*

### Comparing `nornir_nautobot-2.3.0/pyproject.toml` & `nornir_nautobot-2.4.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nornir-nautobot"
-version = "v2.3.0"
+version = "v2.4.0"
 description = "Nornir Nautobot"
 authors = ["Network to Code, LLC <opensource@networktocode.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 keywords = ["Nautobot"]
 classifiers = [
   "Intended Audience :: Developers",
@@ -21,33 +21,44 @@
 
 
 [tool.poetry.dependencies]
 python = "^3.7"
 nornir = "^3.0.0"
 requests = "^2.25.1"
 nornir-utils = "^0"
-nornir-napalm = "^0"
+nornir-napalm = ">=0.4.0 <1.0.0"
 nornir-jinja2 = "^0"
 nornir-netmiko = "^0"
 pynautobot = "^1.0.1"
 netutils = "^1"
+routeros-api = {version = "^0.17.0", optional = true}
+httpx = "^0.24.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
 requests_mock = "*"
 pyyaml = "*"
 black = "*"
 pylint = "*"
 pydocstyle = "*"
 yamllint = "*"
 bandit = "*"
 invoke = "*"
 toml = "*"
 flake8 = "*"
 pydantic = {version = "^1.7.2", extras = ["dotenv"]}
+# documentation dependencies
+mkdocs = "1.3.1"
+mkdocs-material = "8.3.9"
+mkdocstrings = "0.19"
+mkdocstrings-python = "0.7.1"
+mkdocs-version-annotations = "1.0.0"
+
+[tool.poetry.extras]
+mikrotik_driver = ["routeros-api"]
 
 [tool.poetry.plugins."nornir.plugins.inventory"]
 "NautobotInventory" = "nornir_nautobot.plugins.inventory.nautobot:NautobotInventory"
 
 [tool.black]
 line-length = 120
 target-version = ['py37']
```

