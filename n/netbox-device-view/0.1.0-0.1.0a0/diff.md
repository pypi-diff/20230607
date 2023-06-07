# Comparing `tmp/netbox-device-view-0.1.0.tar.gz` & `tmp/netbox-device-view-0.1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-device-view-0.1.0.tar", last modified: Wed Jun  7 18:39:59 2023, max compression
+gzip compressed data, was "netbox-device-view-0.1.0a0.tar", last modified: Fri Jun  2 18:50:17 2023, max compression
```

## Comparing `netbox-device-view-0.1.0.tar` & `netbox-device-view-0.1.0a0.tar`

### file list

```diff
@@ -1,30 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:39:59.159445 netbox-device-view-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-06-07 18:39:59.155445 netbox-device-view-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-06-07 18:39:49.000000 netbox-device-view-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:39:59.155445 netbox-device-view-0.1.0/netbox_device_view/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-07 18:39:49.000000 netbox-device-view-0.1.0/netbox_device_view/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:39:59.155445 netbox-device-view-0.1.0/netbox_device_view/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:39:49.000000 netbox-device-view-0.1.0/netbox_device_view/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-07 18:39:49.000000 netbox-device-view-0.1.0/netbox_device_view/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-07 18:39:49.000000 netbox-device-view-0.1.0/netbox_device_view/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-07 18:39:49.000000 netbox-device-view-0.1.0/netbox_device_view/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-07 18:39:49.000000 netbox-device-view-0.1.0/netbox_device_view/filtersets.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-07 18:39:49.000000 netbox-device-view-0.1.0/netbox_device_view/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:39:59.155445 netbox-device-view-0.1.0/netbox_device_view/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-07 18:39:49.000000 netbox-device-view-0.1.0/netbox_device_view/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:39:49.000000 netbox-device-view-0.1.0/netbox_device_view/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-07 18:39:49.000000 netbox-device-view-0.1.0/netbox_device_view/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-07 18:39:49.000000 netbox-device-view-0.1.0/netbox_device_view/navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-07 18:39:49.000000 netbox-device-view-0.1.0/netbox_device_view/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-07 18:39:49.000000 netbox-device-view-0.1.0/netbox_device_view/template_content.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-07 18:39:49.000000 netbox-device-view-0.1.0/netbox_device_view/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-07 18:39:49.000000 netbox-device-view-0.1.0/netbox_device_view/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-07 18:39:49.000000 netbox-device-view-0.1.0/netbox_device_view/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:39:59.155445 netbox-device-view-0.1.0/netbox_device_view.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-06-07 18:39:59.000000 netbox-device-view-0.1.0/netbox_device_view.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-07 18:39:59.000000 netbox-device-view-0.1.0/netbox_device_view.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 18:39:59.000000 netbox-device-view-0.1.0/netbox_device_view.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 18:39:58.000000 netbox-device-view-0.1.0/netbox_device_view.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-07 18:39:59.000000 netbox-device-view-0.1.0/netbox_device_view.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 18:39:59.159445 netbox-device-view-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-07 18:39:49.000000 netbox-device-view-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:50:17.019214 netbox-device-view-0.1.0a0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-02 18:50:17.019214 netbox-device-view-0.1.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-02 18:50:04.000000 netbox-device-view-0.1.0a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:50:17.019214 netbox-device-view-0.1.0a0/netbox_device_view/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-02 18:50:04.000000 netbox-device-view-0.1.0a0/netbox_device_view/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:50:17.019214 netbox-device-view-0.1.0a0/netbox_device_view/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 18:50:04.000000 netbox-device-view-0.1.0a0/netbox_device_view/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-02 18:50:04.000000 netbox-device-view-0.1.0a0/netbox_device_view/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-02 18:50:04.000000 netbox-device-view-0.1.0a0/netbox_device_view/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-02 18:50:04.000000 netbox-device-view-0.1.0a0/netbox_device_view/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-02 18:50:04.000000 netbox-device-view-0.1.0a0/netbox_device_view/filtersets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-02 18:50:04.000000 netbox-device-view-0.1.0a0/netbox_device_view/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:50:17.019214 netbox-device-view-0.1.0a0/netbox_device_view/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-02 18:50:04.000000 netbox-device-view-0.1.0a0/netbox_device_view/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 18:50:04.000000 netbox-device-view-0.1.0a0/netbox_device_view/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-02 18:50:04.000000 netbox-device-view-0.1.0a0/netbox_device_view/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-02 18:50:04.000000 netbox-device-view-0.1.0a0/netbox_device_view/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-02 18:50:04.000000 netbox-device-view-0.1.0a0/netbox_device_view/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-06-02 18:50:04.000000 netbox-device-view-0.1.0a0/netbox_device_view/template_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-02 18:50:04.000000 netbox-device-view-0.1.0a0/netbox_device_view/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-02 18:50:04.000000 netbox-device-view-0.1.0a0/netbox_device_view/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:50:17.019214 netbox-device-view-0.1.0a0/netbox_device_view.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-02 18:50:17.000000 netbox-device-view-0.1.0a0/netbox_device_view.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-02 18:50:17.000000 netbox-device-view-0.1.0a0/netbox_device_view.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 18:50:17.000000 netbox-device-view-0.1.0a0/netbox_device_view.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 18:50:16.000000 netbox-device-view-0.1.0a0/netbox_device_view.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-02 18:50:17.000000 netbox-device-view-0.1.0a0/netbox_device_view.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 18:50:17.019214 netbox-device-view-0.1.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-02 18:50:04.000000 netbox-device-view-0.1.0a0/setup.py
```

### Comparing `netbox-device-view-0.1.0/README.md` & `netbox-device-view-0.1.0a0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,71 +1,28 @@
-# Netbox Device View Plugin
-![Version](https://img.shields.io/pypi/v/netbox-device-view) ![Downloads](https://img.shields.io/pypi/dm/netbox-device-view)
+Metadata-Version: 2.1
+Name: netbox-device-view
+Version: 0.1.0a0
+Summary: NetBox Device View plugin
+Home-page: https://github.com/peterbaumert/netbox-device-view
+Author: Peter Baumert
+Description-Content-Type: text/markdown
 
-## Install
+## netbox-device-view
 
-The plugin is available as a Python package and can be installed with pip.
+Display Device Ports
 
-Run `pip install netbox-device-view` in your virtual env.
-
-To ensure NetBox Device View plugin is automatically re-installed during future upgrades, create a file named `local_requirements.txt` (if not already existing) in the NetBox root directory (alongside `requirements.txt`) and list the `netbox-device-view` package:
-
-```no-highlight
-# echo netbox-device-view >> local_requirements.txt
-```
-
-Once installed, the plugin needs to be enabled in your `configuration.py` and optionally the `show_on_device_tab` setting enabled.
-
-```python
-# In your configuration.py
-PLUGINS = ["netbox-device-view"]
-
-PLUGINS_CONFIG = {
-    'netbox_device_view': {
-        'show_on_device_tab': True,
-    },
-}
-```
-
-First run `source /opt/netbox/venv/bin/activate` to enter the Python virtual environment.
-
-
-Then run 
-```bash
-cd /opt/netbox/netbox
-pip3 install netbox-device-view
-python3 manage.py migrate netbox-device-view
-python3 manage.py collectstatic --no-input
-```
-
-## How To Use
+Usage:
 
 For each Device Type you need to add a DeviceView.
 
-It is based on a CSS grid view with 32 columns and 2 rows.
-You need to specify the grid-template-areas. 
-- Interface positions will use the following format: {interfacename}{module}-{port}
-- leading "empties" can be specified as x
-- trailing "empties" can be specified as z
-- between "empties" can be named s{0-99}
-
 Example for Cisco C9300-24T with 8x 10G module
 
 ```
-/* C9300-24T */
+/* C9300-24T-8T */
 .switchview.area {
-	grid-template-areas:
-	"x x x x x x x x x x x x x x gigabitethernet0-1 gigabitethernet0-3 gigabitethernet0-5 gigabitethernet0-7 gigabitethernet0-9 gigabitethernet0-11 s0 gigabitethernet0-13 gigabitethernet0-15 gigabitethernet0-17 gigabitethernet0-19 gigabitethernet0-21 gigabitethernet0-23 z z z z z"
-	"x x x x x x x x x x x x x x gigabitethernet0-2 gigabitethernet0-4 gigabitethernet0-6 gigabitethernet0-8 gigabitethernet0-10 gigabitethernet0-12 s0 gigabitethernet0-14 gigabitethernet0-16 gigabitethernet0-18 gigabitethernet0-20 gigabitethernet0-22 gigabitethernet0-24 z z z z z";
-}
-
-/* C9300-24T with C9300-NM-8X */
-.switchview.moduleC9300-NM-8X.area {
-	grid-template-areas:
-	"x x x x x x x x x x x x x x gigabitethernet0-1 gigabitethernet0-3 gigabitethernet0-5 gigabitethernet0-7 gigabitethernet0-9 gigabitethernet0-11 s0 gigabitethernet0-13 gigabitethernet0-15 gigabitethernet0-17 gigabitethernet0-19 gigabitethernet0-21 gigabitethernet0-23 s1 tengigabitethernet1-1 tengigabitethernet1-3 tengigabitethernet1-5 tengigabitethernet1-7"
-	"x x x x x x x x x x x x x x gigabitethernet0-2 gigabitethernet0-4 gigabitethernet0-6 gigabitethernet0-8 gigabitethernet0-10 gigabitethernet0-12 s0 gigabitethernet0-14 gigabitethernet0-16 gigabitethernet0-18 gigabitethernet0-20 gigabitethernet0-22 gigabitethernet0-24 s1 tengigabitethernet1-2 tengigabitethernet1-4 tengigabitethernet1-6 tengigabitethernet1-8";
+	grid-template-areas: "x x x x x x x x x x x x x x gigabitethernet0-1 gigabitethernet0-3 gigabitethernet0-5 gigabitethernet0-7 gigabitethernet0-9 gigabitethernet0-11 s0 gigabitethernet0-13 gigabitethernet0-15 gigabitethernet0-17 gigabitethernet0-19 gigabitethernet0-21 gigabitethernet0-23 s1 tengigabitethernet1-1 tengigabitethernet1-3 tengigabitethernet1-5 tengigabitethernet1-7 s2" "x x x x x x x x x x x x x x gigabitethernet0-2 gigabitethernet0-4 gigabitethernet0-6 gigabitethernet0-8 gigabitethernet0-10 gigabitethernet0-12 s0 gigabitethernet0-14 gigabitethernet0-16 gigabitethernet0-18 gigabitethernet0-20 gigabitethernet0-22 gigabitethernet0-24 s1 tengigabitethernet1-2 tengigabitethernet1-4 tengigabitethernet1-6 tengigabitethernet1-8 s2";
 }
 ```
 
 It will look like
 
-![example](https://github.com/peterbaumert/netbox-device-view/blob/main/docs/example_view.png?raw=true)
+![example](docs/example_view.png)
```

### Comparing `netbox-device-view-0.1.0/netbox_device_view/migrations/0001_initial.py` & `netbox-device-view-0.1.0a0/netbox_device_view/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-device-view-0.1.0/netbox_device_view/urls.py` & `netbox-device-view-0.1.0a0/netbox_device_view/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-device-view-0.1.0/netbox_device_view/utils.py` & `netbox-device-view-0.1.0a0/netbox_device_view/template_content.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,66 +1,67 @@
-from dcim.models import ConsolePort
+from extras.plugins import PluginTemplateExtension
 from .models import DeviceView
-from django.core.exceptions import ObjectDoesNotExist
-
 import re
 
 
-def process_interfaces(interfaces, ports_chassis, switch=1):
-    if interfaces is not None:
+class Ports(PluginTemplateExtension):
+    def page(self):
+        ports_chassis = {}
+        dv = {}
+        modules = {}
+
+        obj = self.context["object"]
+        request = self.context["request"]
+        url = request.build_absolute_uri(obj.get_absolute_url())
+        try:
+            if obj.virtual_chassis is None:
+                dv[1] = DeviceView.objects.get(
+                    device_type=obj.device_type
+                ).grid_template_area.replace(".area", ".area1")
+                modules[1] = obj.modules.all()
+            else:
+                for member in obj.virtual_chassis.members.all():
+                    dv[member.vc_position] = DeviceView.objects.get(
+                        device_type=member.device_type
+                    ).grid_template_area.replace(
+                        ".area", ".area" + str(member.vc_position)
+                    )
+                    modules[member.vc_position] = member.modules.all()
+        except:
+            return ""
+
+        interfaces = obj.vc_interfaces()
+
         for itf in interfaces:
             regex = r"^(?P<type>([a-z]+))((?P<switch>[0-9]+)\/)?((?P<module>[0-9]+)\/)?((?P<port>[0-9]+))$"
             matches = re.search(regex, itf.name.lower())
             if matches:
                 itf.stylename = (
                     (matches["type"] or "")
                     + (matches["module"] or "")
                     + "-"
                     + matches["port"]
                 )
                 sw = int(matches["switch"] or 0)
-                if (
-                    hasattr(itf, "mgmt_only")
-                    and itf.mgmt_only
-                    and itf.type != "virtual"
-                ) or hasattr(itf, "mgmt_only") == False:
-                    sw = switch
                 if sw not in ports_chassis and sw != 0:
                     ports_chassis[sw] = []
                 if sw != 0:
                     ports_chassis[sw].append(itf)
-    return ports_chassis
 
+        return self.render(
+            "netbox_device_view/ports.html",
+            extra_context={
+                "ports_chassis": ports_chassis,
+                "dv": dv,
+                "modules": modules,
+            },
+        )
+
+
+class DevicePorts(Ports):
+    model = "dcim.device"
+
+    def full_width_page(self):
+        return self.page()
 
-def prepare(obj):
-    ports_chassis = {}
-    dv = {}
-    modules = {}
-
-    try:
-        if obj.virtual_chassis is None:
-            dv[1] = DeviceView.objects.get(
-                device_type=obj.device_type
-            ).grid_template_area.replace(".area", ".area1")
-            modules[1] = obj.modules.all()
-            ports_chassis = process_interfaces(obj.interfaces.all(), ports_chassis)
-            ports_chassis = process_interfaces(
-                ConsolePort.objects.filter(device_id=obj.id), ports_chassis
-            )
-        else:
-            for member in obj.virtual_chassis.members.all():
-                dv[member.vc_position] = DeviceView.objects.get(
-                    device_type=member.device_type
-                ).grid_template_area.replace(".area", ".area" + str(member.vc_position))
-                modules[member.vc_position] = member.modules.all()
-                ports_chassis = process_interfaces(
-                    member.interfaces.all(), ports_chassis, member.vc_position
-                )
-                ports_chassis = process_interfaces(
-                    ConsolePort.objects.filter(device_id=member.id),
-                    ports_chassis,
-                    member.vc_position,
-                )
-    except ObjectDoesNotExist:
-        return None, None, None
 
-    return dv, modules, ports_chassis
+template_extensions = [DevicePorts]
```

### Comparing `netbox-device-view-0.1.0/netbox_device_view.egg-info/SOURCES.txt` & `netbox-device-view-0.1.0a0/netbox_device_view.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 netbox_device_view/filtersets.py
 netbox_device_view/forms.py
 netbox_device_view/models.py
 netbox_device_view/navigation.py
 netbox_device_view/tables.py
 netbox_device_view/template_content.py
 netbox_device_view/urls.py
-netbox_device_view/utils.py
 netbox_device_view/views.py
 netbox_device_view.egg-info/PKG-INFO
 netbox_device_view.egg-info/SOURCES.txt
 netbox_device_view.egg-info/dependency_links.txt
 netbox_device_view.egg-info/not-zip-safe
 netbox_device_view.egg-info/top_level.txt
 netbox_device_view/api/__init__.py
```

