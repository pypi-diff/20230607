# Comparing `tmp/olca-ipc-2.0.0a3.tar.gz` & `tmp/olca-ipc-2.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "olca-ipc-2.0.0a3.tar", last modified: Thu Feb  9 08:18:44 2023, max compression
+gzip compressed data, was "olca-ipc-2.0.0a4.tar", last modified: Fri Feb 10 09:58:43 2023, max compression
```

## Comparing `olca-ipc-2.0.0a3.tar` & `olca-ipc-2.0.0a4.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-02-09 08:18:44.889721 olca-ipc-2.0.0a3/
--rw-rw-rw-   0        0        0      161 2023-02-07 15:56:34.000000 olca-ipc-2.0.0a3/.editorconfig
--rw-rw-rw-   0        0        0       90 2023-02-07 15:55:48.000000 olca-ipc-2.0.0a3/.gitignore
--rw-rw-rw-   0        0        0    17099 2020-08-14 08:19:50.000000 olca-ipc-2.0.0a3/LICENSE
--rw-rw-rw-   0        0        0     2008 2023-02-09 08:18:44.889721 olca-ipc-2.0.0a3/PKG-INFO
--rw-rw-rw-   0        0        0     1268 2023-02-07 15:56:34.000000 olca-ipc-2.0.0a3/README.md
-drwxrwxrwx   0        0        0        0 2023-02-09 08:18:44.861795 olca-ipc-2.0.0a3/olca_ipc/
--rw-rw-rw-   0        0        0       20 2023-02-07 15:56:34.000000 olca-ipc-2.0.0a3/olca_ipc/__init__.py
--rw-rw-rw-   0        0        0    22291 2023-02-09 07:56:40.000000 olca-ipc-2.0.0a3/olca_ipc/ipc.py
--rw-rw-rw-   0        0        0     4141 2023-02-07 15:56:34.000000 olca-ipc-2.0.0a3/olca_ipc/ipc_types.py
--rw-rw-rw-   0        0        0     7140 2023-02-09 07:57:40.000000 olca-ipc-2.0.0a3/olca_ipc/protocol.py
--rw-rw-rw-   0        0        0    18190 2023-02-09 07:58:41.000000 olca-ipc-2.0.0a3/olca_ipc/rest.py
-drwxrwxrwx   0        0        0        0 2023-02-09 08:18:44.878749 olca-ipc-2.0.0a3/olca_ipc.egg-info/
--rw-rw-rw-   0        0        0     2008 2023-02-09 08:18:44.000000 olca-ipc-2.0.0a3/olca_ipc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      520 2023-02-09 08:18:44.000000 olca-ipc-2.0.0a3/olca_ipc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-09 08:18:44.000000 olca-ipc-2.0.0a3/olca_ipc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-02-09 08:18:44.000000 olca-ipc-2.0.0a3/olca_ipc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-02-09 08:18:44.000000 olca-ipc-2.0.0a3/olca_ipc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      953 2023-02-09 08:09:19.000000 olca-ipc-2.0.0a3/pyproject.toml
--rw-rw-rw-   0        0        0      333 2023-02-07 15:56:34.000000 olca-ipc-2.0.0a3/pyrightconfig.json
--rw-rw-rw-   0        0        0       39 2023-02-09 08:09:24.000000 olca-ipc-2.0.0a3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-02-09 08:18:44.889721 olca-ipc-2.0.0a3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-02-09 08:18:44.888723 olca-ipc-2.0.0a3/tests/
--rw-rw-rw-   0        0        0      329 2023-02-07 15:56:34.000000 olca-ipc-2.0.0a3/tests/config.py
--rw-rw-rw-   0        0        0     3254 2023-02-09 08:03:26.000000 olca-ipc-2.0.0a3/tests/test_allocation.py
--rw-rw-rw-   0        0        0     1940 2023-02-07 15:56:34.000000 olca-ipc-2.0.0a3/tests/test_crud.py
--rw-rw-rw-   0        0        0      945 2023-02-09 08:01:24.000000 olca-ipc-2.0.0a3/tests/test_get.py
--rw-rw-rw-   0        0        0     2100 2023-02-09 08:01:33.000000 olca-ipc-2.0.0a3/tests/test_mc_sim.py
--rw-rw-rw-   0        0        0      883 2023-02-09 08:02:00.000000 olca-ipc-2.0.0a3/tests/test_param.py
--rw-rw-rw-   0        0        0      734 2023-02-09 08:02:13.000000 olca-ipc-2.0.0a3/tests/test_qref.py
--rw-rw-rw-   0        0        0     5214 2023-02-09 08:02:41.000000 olca-ipc-2.0.0a3/tests/test_simple_calculation.py
+drwxrwxrwx   0        0        0        0 2023-02-10 09:58:43.477224 olca-ipc-2.0.0a4/
+-rw-rw-rw-   0        0        0      161 2023-02-07 15:56:34.000000 olca-ipc-2.0.0a4/.editorconfig
+-rw-rw-rw-   0        0        0       90 2023-02-07 15:55:48.000000 olca-ipc-2.0.0a4/.gitignore
+-rw-rw-rw-   0        0        0    17099 2020-08-14 08:19:50.000000 olca-ipc-2.0.0a4/LICENSE
+-rw-rw-rw-   0        0        0     2008 2023-02-10 09:58:43.477224 olca-ipc-2.0.0a4/PKG-INFO
+-rw-rw-rw-   0        0        0     1268 2023-02-07 15:56:34.000000 olca-ipc-2.0.0a4/README.md
+drwxrwxrwx   0        0        0        0 2023-02-10 09:58:43.449274 olca-ipc-2.0.0a4/olca_ipc/
+-rw-rw-rw-   0        0        0       20 2023-02-07 15:56:34.000000 olca-ipc-2.0.0a4/olca_ipc/__init__.py
+-rw-rw-rw-   0        0        0    23879 2023-02-10 09:52:14.000000 olca-ipc-2.0.0a4/olca_ipc/ipc.py
+-rw-rw-rw-   0        0        0     7571 2023-02-10 09:52:14.000000 olca-ipc-2.0.0a4/olca_ipc/protocol.py
+-rw-rw-rw-   0        0        0    18881 2023-02-10 09:52:14.000000 olca-ipc-2.0.0a4/olca_ipc/rest.py
+-rw-rw-rw-   0        0        0     4886 2023-02-10 09:52:14.000000 olca-ipc-2.0.0a4/olca_ipc/upstream_tree.py
+drwxrwxrwx   0        0        0        0 2023-02-10 09:58:43.467227 olca-ipc-2.0.0a4/olca_ipc.egg-info/
+-rw-rw-rw-   0        0        0     2008 2023-02-10 09:58:43.000000 olca-ipc-2.0.0a4/olca_ipc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      552 2023-02-10 09:58:43.000000 olca-ipc-2.0.0a4/olca_ipc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-10 09:58:43.000000 olca-ipc-2.0.0a4/olca_ipc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-02-10 09:58:43.000000 olca-ipc-2.0.0a4/olca_ipc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-02-10 09:58:43.000000 olca-ipc-2.0.0a4/olca_ipc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      953 2023-02-10 09:57:44.000000 olca-ipc-2.0.0a4/pyproject.toml
+-rw-rw-rw-   0        0        0      333 2023-02-07 15:56:34.000000 olca-ipc-2.0.0a4/pyrightconfig.json
+-rw-rw-rw-   0        0        0       39 2023-02-09 12:43:36.000000 olca-ipc-2.0.0a4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-02-10 09:58:43.478196 olca-ipc-2.0.0a4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-02-10 09:58:43.476230 olca-ipc-2.0.0a4/tests/
+-rw-rw-rw-   0        0        0      329 2023-02-07 15:56:34.000000 olca-ipc-2.0.0a4/tests/config.py
+-rw-rw-rw-   0        0        0     3254 2023-02-09 12:43:36.000000 olca-ipc-2.0.0a4/tests/test_allocation.py
+-rw-rw-rw-   0        0        0     1940 2023-02-07 15:56:34.000000 olca-ipc-2.0.0a4/tests/test_crud.py
+-rw-rw-rw-   0        0        0      945 2023-02-09 12:43:36.000000 olca-ipc-2.0.0a4/tests/test_get.py
+-rw-rw-rw-   0        0        0     2100 2023-02-09 12:43:36.000000 olca-ipc-2.0.0a4/tests/test_mc_sim.py
+-rw-rw-rw-   0        0        0      883 2023-02-09 12:43:36.000000 olca-ipc-2.0.0a4/tests/test_param.py
+-rw-rw-rw-   0        0        0      734 2023-02-09 12:43:36.000000 olca-ipc-2.0.0a4/tests/test_qref.py
+-rw-rw-rw-   0        0        0     5214 2023-02-09 12:43:36.000000 olca-ipc-2.0.0a4/tests/test_simple_calculation.py
+-rw-rw-rw-   0        0        0     2084 2023-02-10 09:52:14.000000 olca-ipc-2.0.0a4/tests/test_upstream_tree.py
```

### Comparing `olca-ipc-2.0.0a3/LICENSE` & `olca-ipc-2.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `olca-ipc-2.0.0a3/PKG-INFO` & `olca-ipc-2.0.0a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olca-ipc
-Version: 2.0.0a3
+Version: 2.0.0a4
 Summary: A package for calling openLCA functions from Python.
 Project-URL: Homepage, https://github.com/GreenDelta/olca-ipc.py
 Project-URL: Bug Tracker, https://github.com/GreenDelta/olca-ipc.py/issues
 Keywords: openLCA,life cycle assessment,LCA
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `olca-ipc-2.0.0a3/README.md` & `olca-ipc-2.0.0a4/README.md`

 * *Files identical despite different names*

### Comparing `olca-ipc-2.0.0a3/olca_ipc/ipc.py` & `olca-ipc-2.0.0a4/olca_ipc/ipc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import logging as log
 from dataclasses import dataclass
-from typing import cast, Any, Optional, Tuple, Type
+from typing import cast, Any, Callable, Optional, Tuple, Type, TypeVar
 
 import requests
 import olca_schema as o
 
 from .protocol import E, IpcProtocol, IpcResult
 
+_T = TypeVar("_T")
+
 
 class Client(IpcProtocol):
     """
     A client to communicate with an openLCA IPC server over the JSON-RPC
     protocol.
     """
 
@@ -184,14 +186,32 @@
             err_msg = "%i: %s" % (err.get("code"), err.get("message"))
             return None, err_msg
         result = resp.get("result")
         if result is None:
             return None, "No error and no result: invalid JSON-RPC response"
         return result, None
 
+    def _call(
+        self, method: str, transform: Callable[[Any], _T], data: Any = None
+    ) -> _T | None:
+        (resp, err) = self.rpc_call(method, data)
+        if err is not None:
+            log.error("failed to call method %s: %s", method, err)
+            return None
+        return transform(resp)
+
+    def _call_each(
+        self, method: str, transform: Callable[[Any], _T], data: Any = None
+    ) -> list[_T]:
+        (resp, err) = self.rpc_call(method, data)
+        if err is not None:
+            log.error("failed to call method %s: %s", method, err)
+            return []
+        return [transform(r) for r in resp]
+
 
 @dataclass
 class Result(IpcResult):
     uid: str
     client: "Client"
     error: Optional[o.ResultState]
 
@@ -248,14 +268,16 @@
         args = {"@id": self.uid}
         (r, err) = self.client.rpc_call("result/impact-categories", args)
         if err:
             log.error("request impact-categories failed: %s", err)
             return []
         return [o.Ref.from_dict(d) for d in r]
 
+    # region: tech-flows
+
     def get_total_requirements(self) -> list[o.TechFlowValue]:
         args = {"@id": self.uid}
         (r, err) = self.client.rpc_call("result/total-requirements", args)
         if err:
             log.error("request total-requirements failed: %s", err)
             return []
         return [o.TechFlowValue.from_dict(d) for d in r]
@@ -266,14 +288,41 @@
         args = {"@id": self.uid, "techFlow": tech_flow.to_dict()}
         (r, err) = self.client.rpc_call("result/total-requirements-of", args)
         if err:
             log.error("request total-requirements-of failed: %s", err)
             return o.TechFlowValue(amount=0, tech_flow=tech_flow)
         return o.TechFlowValue.from_dict(r)
 
+    def get_scaling_factors(self) -> list[o.TechFlowValue]:
+        return self.client._call_each(
+            "result/scaling-factors",
+            o.TechFlowValue.from_dict,
+            {"@id": self.uid},
+        )
+
+    def get_scaled_tech_flows_of(
+        self, tech_flow: o.TechFlow
+    ) -> list[o.TechFlowValue]:
+        return self.client._call_each(
+            "result/scaled-tech-flows-of",
+            o.TechFlowValue.from_dict,
+            {"@id": self.uid, "techFlow": tech_flow.to_dict()},
+        )
+
+    def get_unscaled_tech_flows_of(
+        self, tech_flow: o.TechFlow
+    ) -> list[o.TechFlowValue]:
+        return self.client._call_each(
+            "result/unscaled-tech-flows-of",
+            o.TechFlowValue.from_dict,
+            {"@id": self.uid, "techFlow": tech_flow.to_dict()},
+        )
+
+    # endregion
+
     # region: flows
 
     def get_total_flows(self) -> list[o.EnviFlowValue]:
         args = {"@id": self.uid}
         (r, err) = self.client.rpc_call("result/total-flows", args)
         if err:
             log.error("request total-flows failed: %s", err)
```

### Comparing `olca-ipc-2.0.0a3/olca_ipc/protocol.py` & `olca-ipc-2.0.0a4/olca_ipc/protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,25 +121,45 @@
     def get_envi_flows(self) -> list[o.EnviFlow]:
         pass
 
     @abstractmethod
     def get_impact_categories(self) -> list[o.Ref]:
         pass
 
+    # region: tech-flows
+
     @abstractmethod
     def get_total_requirements(self) -> list[o.TechFlowValue]:
         pass
 
     @abstractmethod
     def get_total_requirements_of(
         self, tech_flow: o.TechFlow
     ) -> o.TechFlowValue:
         pass
 
     @abstractmethod
+    def get_scaling_factors(self) -> list[o.TechFlowValue]:
+        pass
+
+    @abstractmethod
+    def get_scaled_tech_flows_of(
+        self, tech_flow: o.TechFlow
+    ) -> list[o.TechFlowValue]:
+        pass
+
+    @abstractmethod
+    def get_unscaled_tech_flows_of(
+        self, tech_flow: o.TechFlow
+    ) -> list[o.TechFlowValue]:
+        pass
+
+    # endregion
+
+    @abstractmethod
     def get_total_flows(self) -> list[o.EnviFlowValue]:
         pass
 
     @abstractmethod
     def get_total_flow_value_of(self, envi_flow: o.EnviFlow) -> o.EnviFlowValue:
         pass
```

### Comparing `olca-ipc-2.0.0a3/olca_ipc/rest.py` & `olca-ipc-2.0.0a4/olca_ipc/rest.py`

 * *Files 4% similar despite different names*

```diff
@@ -213,25 +213,48 @@
 
     def get_envi_flows(self) -> list[o.EnviFlow]:
         return self._get_each("envi-flows", o.EnviFlow.from_dict)
 
     def get_impact_categories(self) -> list[o.Ref]:
         return self._get_each("impact-categories", o.Ref.from_dict)
 
+    # region: tech-flows
+
     def get_total_requirements(self) -> list[o.TechFlowValue]:
         return self._get_each("total-requirements", o.TechFlowValue.from_dict)
 
     def get_total_requirements_of(
         self, tech_flow: o.TechFlow
     ) -> list[o.TechFlowValue]:
         return self._get_each(
             f"total-requirements-of/{_tech_id(tech_flow)}",
             o.TechFlowValue.from_dict,
         )
 
+    def get_scaling_factors(self) -> list[o.TechFlowValue]:
+        return self._get_each("scaling-factors", o.TechFlowValue.from_dict)
+
+    def get_scaled_tech_flows_of(
+        self, tech_flow: o.TechFlow
+    ) -> list[o.TechFlowValue]:
+        return self._get_each(
+            f"scaled-tech-flows-of/{_tech_id(tech_flow)}",
+            o.TechFlowValue.from_dict,
+        )
+
+    def get_unscaled_tech_flows_of(
+        self, tech_flow: o.TechFlow
+    ) -> list[o.TechFlowValue]:
+        return self._get_each(
+            f"unscaled-tech-flows-of/{_tech_id(tech_flow)}",
+            o.TechFlowValue.from_dict,
+        )
+
+    # endregion
+
     def get_total_flows(self) -> list[o.EnviFlowValue]:
         return self._get_each("total-flows", o.EnviFlowValue.from_dict)
 
     def get_total_flow_value_of(
         self, envi_flow: o.EnviFlow
     ) -> o.EnviFlowValue | None:
         return self._get(
```

### Comparing `olca-ipc-2.0.0a3/olca_ipc.egg-info/PKG-INFO` & `olca-ipc-2.0.0a4/olca_ipc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olca-ipc
-Version: 2.0.0a3
+Version: 2.0.0a4
 Summary: A package for calling openLCA functions from Python.
 Project-URL: Homepage, https://github.com/GreenDelta/olca-ipc.py
 Project-URL: Bug Tracker, https://github.com/GreenDelta/olca-ipc.py/issues
 Keywords: openLCA,life cycle assessment,LCA
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `olca-ipc-2.0.0a3/olca_ipc.egg-info/SOURCES.txt` & `olca-ipc-2.0.0a4/olca_ipc.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 LICENSE
 README.md
 pyproject.toml
 pyrightconfig.json
 requirements.txt
 olca_ipc/__init__.py
 olca_ipc/ipc.py
-olca_ipc/ipc_types.py
 olca_ipc/protocol.py
 olca_ipc/rest.py
+olca_ipc/upstream_tree.py
 olca_ipc.egg-info/PKG-INFO
 olca_ipc.egg-info/SOURCES.txt
 olca_ipc.egg-info/dependency_links.txt
 olca_ipc.egg-info/requires.txt
 olca_ipc.egg-info/top_level.txt
 tests/config.py
 tests/test_allocation.py
 tests/test_crud.py
 tests/test_get.py
 tests/test_mc_sim.py
 tests/test_param.py
 tests/test_qref.py
-tests/test_simple_calculation.py
+tests/test_simple_calculation.py
+tests/test_upstream_tree.py
```

### Comparing `olca-ipc-2.0.0a3/pyproject.toml` & `olca-ipc-2.0.0a4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "olca-ipc"
-version = "2.0.0a3"
+version = "2.0.0a4"
 description = "A package for calling openLCA functions from Python."
 readme = "README.md"
 requires-python = ">=3.11"
 keywords=["openLCA", "life cycle assessment", "LCA"]
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: 3",
```

### Comparing `olca-ipc-2.0.0a3/tests/test_allocation.py` & `olca-ipc-2.0.0a4/tests/test_allocation.py`

 * *Files identical despite different names*

### Comparing `olca-ipc-2.0.0a3/tests/test_crud.py` & `olca-ipc-2.0.0a4/tests/test_crud.py`

 * *Files identical despite different names*

### Comparing `olca-ipc-2.0.0a3/tests/test_get.py` & `olca-ipc-2.0.0a4/tests/test_get.py`

 * *Files identical despite different names*

### Comparing `olca-ipc-2.0.0a3/tests/test_mc_sim.py` & `olca-ipc-2.0.0a4/tests/test_mc_sim.py`

 * *Files identical despite different names*

### Comparing `olca-ipc-2.0.0a3/tests/test_param.py` & `olca-ipc-2.0.0a4/tests/test_param.py`

 * *Files identical despite different names*

### Comparing `olca-ipc-2.0.0a3/tests/test_qref.py` & `olca-ipc-2.0.0a4/tests/test_qref.py`

 * *Files identical despite different names*

### Comparing `olca-ipc-2.0.0a3/tests/test_simple_calculation.py` & `olca-ipc-2.0.0a4/tests/test_simple_calculation.py`

 * *Files identical despite different names*

