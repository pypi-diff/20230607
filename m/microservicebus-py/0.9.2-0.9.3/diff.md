# Comparing `tmp/microservicebus-py-0.9.2.tar.gz` & `tmp/microservicebus-py-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microservicebus-py-0.9.2.tar", last modified: Fri Jun  2 10:03:27 2023, max compression
+gzip compressed data, was "microservicebus-py-0.9.3.tar", last modified: Wed Jun  7 20:30:31 2023, max compression
```

## Comparing `microservicebus-py-0.9.2.tar` & `microservicebus-py-0.9.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 mikael    (1000) mikael    (1000)        0 2023-06-02 10:03:27.388543 microservicebus-py-0.9.2/
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4745 2023-06-02 10:03:27.383549 microservicebus-py-0.9.2/PKG-INFO
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3680 2022-12-12 08:25:32.000000 microservicebus-py-0.9.2/README.md
-drwxrwxrwx   0 mikael    (1000) mikael    (1000)        0 2023-06-02 10:03:26.963785 microservicebus-py-0.9.2/microservicebus_py.egg-info/
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4745 2023-06-02 10:03:26.000000 microservicebus-py-0.9.2/microservicebus_py.egg-info/PKG-INFO
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)      455 2023-06-02 10:03:26.000000 microservicebus-py-0.9.2/microservicebus_py.egg-info/SOURCES.txt
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)        1 2023-06-02 10:03:26.000000 microservicebus-py-0.9.2/microservicebus_py.egg-info/dependency_links.txt
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)       55 2023-06-02 10:03:26.000000 microservicebus-py-0.9.2/microservicebus_py.egg-info/entry_points.txt
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)        4 2023-06-02 10:03:26.000000 microservicebus-py-0.9.2/microservicebus_py.egg-info/top_level.txt
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)       38 2023-06-02 10:03:27.389544 microservicebus-py-0.9.2/setup.cfg
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     1707 2023-06-02 09:59:05.000000 microservicebus-py-0.9.2/setup.py
-drwxrwxrwx   0 mikael    (1000) mikael    (1000)        0 2023-06-02 10:03:27.351061 microservicebus-py-0.9.2/src/
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)      807 2022-12-19 11:22:24.000000 microservicebus-py-0.9.2/src/axians.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     5689 2023-05-31 17:27:32.000000 microservicebus-py-0.9.2/src/base_service.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     1324 2023-01-05 09:33:48.000000 microservicebus-py-0.9.2/src/logger_service.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)    29617 2023-06-02 09:27:26.000000 microservicebus-py-0.9.2/src/msb_handler.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     6536 2023-03-06 08:30:37.000000 microservicebus-py-0.9.2/src/orchestrator_service.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)      340 2022-03-14 19:13:32.000000 microservicebus-py-0.9.2/src/queue_message.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4414 2022-12-02 13:59:45.000000 microservicebus-py-0.9.2/src/rauc_handler.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)      846 2023-06-02 09:05:37.000000 microservicebus-py-0.9.2/src/start.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3311 2023-01-09 21:54:56.000000 microservicebus-py-0.9.2/src/terminal_service.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)      672 2022-03-23 09:36:17.000000 microservicebus-py-0.9.2/src/test.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3971 2023-06-02 09:05:37.000000 microservicebus-py-0.9.2/src/utils.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3136 2022-12-12 08:35:01.000000 microservicebus-py-0.9.2/src/vpn_helper.py
+drwxrwxrwx   0 mikael    (1000) mikael    (1000)        0 2023-06-07 20:30:31.608461 microservicebus-py-0.9.3/
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4745 2023-06-07 20:30:31.597964 microservicebus-py-0.9.3/PKG-INFO
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3680 2022-12-12 08:25:32.000000 microservicebus-py-0.9.3/README.md
+drwxrwxrwx   0 mikael    (1000) mikael    (1000)        0 2023-06-07 20:30:30.848069 microservicebus-py-0.9.3/microservicebus_py.egg-info/
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4745 2023-06-07 20:30:29.000000 microservicebus-py-0.9.3/microservicebus_py.egg-info/PKG-INFO
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)      455 2023-06-07 20:30:30.000000 microservicebus-py-0.9.3/microservicebus_py.egg-info/SOURCES.txt
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)        1 2023-06-07 20:30:29.000000 microservicebus-py-0.9.3/microservicebus_py.egg-info/dependency_links.txt
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)       55 2023-06-07 20:30:29.000000 microservicebus-py-0.9.3/microservicebus_py.egg-info/entry_points.txt
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)        4 2023-06-07 20:30:29.000000 microservicebus-py-0.9.3/microservicebus_py.egg-info/top_level.txt
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)       38 2023-06-07 20:30:31.611930 microservicebus-py-0.9.3/setup.cfg
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     1707 2023-06-02 09:59:05.000000 microservicebus-py-0.9.3/setup.py
+drwxrwxrwx   0 mikael    (1000) mikael    (1000)        0 2023-06-07 20:30:31.535830 microservicebus-py-0.9.3/src/
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)      807 2022-12-19 11:22:24.000000 microservicebus-py-0.9.3/src/axians.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     5689 2023-05-31 17:27:32.000000 microservicebus-py-0.9.3/src/base_service.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     1324 2023-01-05 09:33:48.000000 microservicebus-py-0.9.3/src/logger_service.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)    30492 2023-06-07 20:25:29.000000 microservicebus-py-0.9.3/src/msb_handler.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     6536 2023-03-06 08:30:37.000000 microservicebus-py-0.9.3/src/orchestrator_service.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)      340 2022-03-14 19:13:32.000000 microservicebus-py-0.9.3/src/queue_message.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4414 2022-12-02 13:59:45.000000 microservicebus-py-0.9.3/src/rauc_handler.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)      846 2023-06-02 09:05:37.000000 microservicebus-py-0.9.3/src/start.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3311 2023-01-09 21:54:56.000000 microservicebus-py-0.9.3/src/terminal_service.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)      672 2022-03-23 09:36:17.000000 microservicebus-py-0.9.3/src/test.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3971 2023-06-02 09:05:37.000000 microservicebus-py-0.9.3/src/utils.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3136 2022-12-12 08:35:01.000000 microservicebus-py-0.9.3/src/vpn_helper.py
```

### Comparing `microservicebus-py-0.9.2/PKG-INFO` & `microservicebus-py-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microservicebus-py
-Version: 0.9.2
+Version: 0.9.3
 Summary: Python agent for microServiceBus.com. Please visit https://microservicebus.com for more information.
 Home-page: https://github.com/axians/microservicebus-py
 Author: AXIANS IoT Operations
 Author-email: microservicebus@axians.com
 License: MIT
 Description: # microservicebus-py
```

### Comparing `microservicebus-py-0.9.2/README.md` & `microservicebus-py-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.2/microservicebus_py.egg-info/PKG-INFO` & `microservicebus-py-0.9.3/microservicebus_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microservicebus-py
-Version: 0.9.2
+Version: 0.9.3
 Summary: Python agent for microServiceBus.com. Please visit https://microservicebus.com for more information.
 Home-page: https://github.com/axians/microservicebus-py
 Author: AXIANS IoT Operations
 Author-email: microservicebus@axians.com
 License: MIT
 Description: # microservicebus-py
```

### Comparing `microservicebus-py-0.9.2/setup.py` & `microservicebus-py-0.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.2/src/axians.py` & `microservicebus-py-0.9.3/src/axians.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.2/src/base_service.py` & `microservicebus-py-0.9.3/src/base_service.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.2/src/logger_service.py` & `microservicebus-py-0.9.3/src/logger_service.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.2/src/msb_handler.py` & `microservicebus-py-0.9.3/src/msb_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,14 +115,16 @@
         content = (root / "package.json").read_text()
         packageInfo = json.loads(content)
         return packageInfo
 
     def save_settings(self, settings):
         with open(self.msb_settings_path, 'w') as settings_file:
             json.dump(settings, settings_file)
+            self.settings = settings
+            self.printf("Settings saved")
 
     async def sign_in(self, settings, first_sign_in):
         if(first_sign_in == True):
             self.printf("Node created successfully")
             settings["hubUri"] = self.settings["hubUri"] 
             self.settings = settings
             self.save_settings(settings)
@@ -207,15 +209,19 @@
             asyncio.run(self.Debug(f"Loading module {module_name}"))
 
         except Exception as e:
             asyncio.run(self.ThrowError(
                 f"Error in msb.start_azure_iot_service: {e}"))
 
     async def refresh_vpn_settings(self, args):
-        self.connection.send("getVpnSettings", [""])
+        try:
+            await self.Debug(f"refresh_vpn_settings")
+            self.connection.send("getVpnSettings", [""])
+        except Exception as e:
+            await self.Debug(f"Error in refresh_vpn_settings: {e}")
 
     async def update_vpn_endpoint(self, args):
         self.connection.send("updateVpnEndpoint", [args.message[0]["ip"]])
 
     # endregion
     # region SignalR event listeners
 
@@ -339,102 +345,110 @@
 
         self.connection.start()
         time.sleep(1)
         self.set_interval(self.sendHeartbeat, 60 * 3)
     # endregion
     # region SignalR callback functions
     def successful_sign_in(self, sign_in_response):
-        node_name = sign_in_response["nodeName"]
-        tag_list = sign_in_response["tags"]
-
-        asyncio.run(self.Debug(f"Node {node_name} signed in successfully"))
-        
-        if "hubUri" not in self.settings:
-            sign_in_response["hubUri"] = self.settings["hubUri"]
-        
-        sign_in_response["hubUri"] = self.base_uri
-        self.save_settings(sign_in_response)        
-        
-        asyncio.run(self.SubmitAction("*", "msb_signed_in", {}))
-        
-        if os.path.isdir(self.service_path) == False:
-            os.mkdir(self.service_path)
-
-        state = self.settings["state"]
-        asyncio.run(self.Debug(f"Node state {state}"))
-        asyncio.run(self.SubmitAction("orchestrator", "_set_state", {"state": state}))
-
-        if sign_in_response['itineraries'] is not None and state == "Active":
-            for itinerary in sign_in_response['itineraries']:
-                pythonActivities = [srv for srv in itinerary["activities"]
-                                    if "baseType" in srv["userData"] and srv["userData"]["baseType"] == 'pythonfile']
-                for pythonActivity in pythonActivities:
-                    try:
-                        host_config = [srv for srv in pythonActivity["userData"]
-                                    ["config"]["generalConfig"] if srv["id"] == 'host']
-
-                        # Check if activity is set to run on node
-                        if host_config[0]["value"] != node_name and host_config[0]["value"] not in tag_list:
-                            continue
-
-                        organization_id = sign_in_response["organizationId"]
-                        file_name = pythonActivity["userData"]["type"].replace(
-                            "_py", ".py")
-
-                        uri = f"{self.base_uri}/api/Scripts/{organization_id}/{file_name}" if pythonActivity["userData"][
-                            "isCustom"] == True else f"{self.base_uri}/api/Scripts/00000000-0000-0000-0000-000000000001/{file_name}"
-
-                        service_file = requests.get(uri, allow_redirects=True, verify=False)
-                        service_file_name = os.path.join(
-                            self.service_path, file_name)
-
-                        file = open(service_file_name, 'wb+')
-                        file.write(service_file.content)
-                        file.close()
-
-                        module_name = pythonActivity["userData"]["type"].replace(
-                            "_py", "")
-                        service_name = pythonActivity["userData"]["type"]
-                        service_config = pythonActivity["userData"]["config"]
+        try:
+            node_name = sign_in_response["nodeName"]
+            tag_list = sign_in_response["tags"]
 
+            if "hubUri" not in self.settings:
+                sign_in_response["hubUri"] = self.settings["hubUri"]
+            
+            sign_in_response["hubUri"] = self.base_uri
+            self.save_settings(sign_in_response)        
+            
+            asyncio.run(self.SubmitAction("*", "msb_signed_in", {}))
+            
+            if os.path.isdir(self.service_path) == False:
+                os.mkdir(self.service_path)
+
+            state = self.settings["state"]
+            asyncio.run(self.Debug(f"Node state {state}"))
+            asyncio.run(self.SubmitAction("orchestrator", "_set_state", {"state": state}))
+
+            if sign_in_response['itineraries'] is not None and state == "Active":
+                for itinerary in sign_in_response['itineraries']:
+                    pythonActivities = [srv for srv in itinerary["activities"]
+                                        if "baseType" in srv["userData"] and srv["userData"]["baseType"] == 'pythonfile']
+                    for pythonActivity in pythonActivities:
                         try:
-                            spec = importlib.util.spec_from_file_location(
-                                module_name, service_file_name)
-                            module = importlib.util.module_from_spec(spec)
-                            spec.loader.exec_module(module)
-                            MicroService = getattr(module, module_name)
-                            
-                            microService = MicroService(service_name.lower(), self.queue, service_config)  # (id, queue, config)
-                            asyncio.run(self.StartService(microService))
-                            asyncio.run(self.Debug(f"Loading module {module_name}"))
-                        except Exception as loadEx:
-                            asyncio.run(self.Debug(f"Unable to load {module_name}service: Error: {loadEx}"))
-                            print(f"Unable to load {module_name}service: Error: {loadEx}")
-
-                    except Exception as ex:
-                        print("Unable to start service")
-
-        settings = self.get_settings()
-        self.connection.send("signedIn", [ settings["nodeName"], socket.gethostname(), "Online", settings["organizationId"], False])
-        self.sendHeartbeat()
+                            host_config = [srv for srv in pythonActivity["userData"]
+                                        ["config"]["generalConfig"] if srv["id"] == 'host']
+
+                            # Check if activity is set to run on node
+                            if host_config[0]["value"] != node_name and host_config[0]["value"] not in tag_list:
+                                continue
+
+                            organization_id = sign_in_response["organizationId"]
+                            file_name = pythonActivity["userData"]["type"].replace(
+                                "_py", ".py")
+
+                            uri = f"{self.base_uri}/api/Scripts/{organization_id}/{file_name}" if pythonActivity["userData"][
+                                "isCustom"] == True else f"{self.base_uri}/api/Scripts/00000000-0000-0000-0000-000000000001/{file_name}"
+
+                            service_file = requests.get(uri, allow_redirects=True, verify=False)
+                            service_file_name = os.path.join(
+                                self.service_path, file_name)
+
+                            file = open(service_file_name, 'wb+')
+                            file.write(service_file.content)
+                            file.close()
+
+                            module_name = pythonActivity["userData"]["type"].replace(
+                                "_py", "")
+                            service_name = pythonActivity["userData"]["type"]
+                            service_config = pythonActivity["userData"]["config"]
+
+                            try:
+                                spec = importlib.util.spec_from_file_location(
+                                    module_name, service_file_name)
+                                module = importlib.util.module_from_spec(spec)
+                                spec.loader.exec_module(module)
+                                MicroService = getattr(module, module_name)
+                                
+                                microService = MicroService(service_name.lower(), self.queue, service_config)  # (id, queue, config)
+                                asyncio.run(self.StartService(microService))
+                                asyncio.run(self.Debug(f"Loading module {module_name}"))
+                            except Exception as loadEx:
+                                asyncio.run(self.Debug(f"Unable to load {module_name}service: Error: {loadEx}"))
+                                print(f"Unable to load {module_name}service: Error: {loadEx}")
+
+                        except Exception as ex:
+                            print("Unable to start service")
+
+            settings = self.get_settings()
+            self.connection.send("signedIn", [ settings["nodeName"], socket.gethostname(), "Online", settings["organizationId"], False])
+            self.sendHeartbeat()
+            asyncio.run(self.Debug(f"Node {node_name} signed in successfully"))
+            
+        except Exception as ex:
+            asyncio.run(self.Debug(f"sign_in_response error: {ex}"))
+            asyncio.run(self.Debug(f"sign_in_response: {sign_in_response}"))
 
     def update_token(self, token):
         self.settings["sas"] = token
         self.save_settings(self.settings)
         self.debug_sync(f"SAS token has been updated.")
         #self.restart()
 
     def not_implemented(self, event_handler):
         asyncio.run(self.ThrowError(
             f'SignalR event handler \033[93m"{event_handler}"\033[0m is not implemented in the Python Node'))
 
     def ping_response(self, conn_id):
-        settings = self.get_settings()
-        self.connection.send("pingResponse", [ settings["nodeName"], socket.gethostname(), "Online", conn_id, False])
-        asyncio.run(self.Debug("Ping response"))
+        try:
+            asyncio.run(self.Debug(f"Ping request"))
+            settings = self.get_settings()
+            self.connection.send("pingResponse", [ settings["nodeName"], socket.gethostname(), "Online", conn_id, False])
+            asyncio.run(self.Debug("Ping response"))
+        except Exception as e:
+            asyncio.run(self.Debug(f"Error in ping_response: {e}"))
     
     def connected(self):
         self.debug_sync("Connection opened and handshake received ready to send messages")
         self._connected = True
 
         if(self._reconnect is True):
             id = self.settings["id"]
```

### Comparing `microservicebus-py-0.9.2/src/orchestrator_service.py` & `microservicebus-py-0.9.3/src/orchestrator_service.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.2/src/rauc_handler.py` & `microservicebus-py-0.9.3/src/rauc_handler.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.2/src/start.py` & `microservicebus-py-0.9.3/src/start.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.2/src/terminal_service.py` & `microservicebus-py-0.9.3/src/terminal_service.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.2/src/test.py` & `microservicebus-py-0.9.3/src/test.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.2/src/utils.py` & `microservicebus-py-0.9.3/src/utils.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.2/src/vpn_helper.py` & `microservicebus-py-0.9.3/src/vpn_helper.py`

 * *Files identical despite different names*

