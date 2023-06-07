# Comparing `tmp/stackdiac-0.0.1.dev25.tar.gz` & `tmp/stackdiac-0.0.1.dev26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stackdiac-0.0.1.dev25.tar", max compression
+gzip compressed data, was "stackdiac-0.0.1.dev26.tar", max compression
```

## Comparing `stackdiac-0.0.1.dev25.tar` & `stackdiac-0.0.1.dev26.tar`

### file list

```diff
@@ -1,30 +1,33 @@
--rw-r--r--   0        0        0     1066 2023-05-17 10:08:01.271455 stackdiac-0.0.1.dev25/LICENSE
--rw-r--r--   0        0        0     1415 2023-05-17 10:08:01.271455 stackdiac-0.0.1.dev25/README.md
--rw-r--r--   0        0        0      576 2023-05-17 10:08:20.623623 stackdiac-0.0.1.dev25/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-17 10:08:01.275455 stackdiac-0.0.1.dev25/stackdiac/__init__.py
--rw-r--r--   0        0        0       23 2023-05-17 10:08:01.275455 stackdiac-0.0.1.dev25/stackdiac/api/__init__.py
--rw-r--r--   0        0        0     1179 2023-05-17 10:08:01.275455 stackdiac-0.0.1.dev25/stackdiac/api/server.py
--rw-r--r--   0        0        0     1800 2023-05-17 10:08:01.275455 stackdiac-0.0.1.dev25/stackdiac/cli/__init__.py
--rw-r--r--   0        0        0      729 2023-05-17 10:08:01.275455 stackdiac-0.0.1.dev25/stackdiac/cli/build.py
--rw-r--r--   0        0        0     1594 2023-05-17 10:08:01.275455 stackdiac-0.0.1.dev25/stackdiac/cli/create.py
--rw-r--r--   0        0        0      464 2023-05-17 10:08:01.275455 stackdiac-0.0.1.dev25/stackdiac/cli/ui.py
--rw-r--r--   0        0        0      381 2023-05-17 10:08:01.275455 stackdiac-0.0.1.dev25/stackdiac/models/__init__.py
--rw-r--r--   0        0        0     1145 2023-05-17 10:08:01.275455 stackdiac-0.0.1.dev25/stackdiac/models/backend.py
--rw-r--r--   0        0        0     2582 2023-05-17 10:08:01.275455 stackdiac-0.0.1.dev25/stackdiac/models/binary.py
--rw-r--r--   0        0        0     3975 2023-05-17 10:08:01.275455 stackdiac-0.0.1.dev25/stackdiac/models/cluster.py
--rw-r--r--   0        0        0     2769 2023-05-17 10:08:01.275455 stackdiac-0.0.1.dev25/stackdiac/models/config.py
--rw-r--r--   0        0        0     1499 2023-05-17 10:08:01.275455 stackdiac-0.0.1.dev25/stackdiac/models/operation.py
--rw-r--r--   0        0        0      161 2023-05-17 10:08:01.275455 stackdiac-0.0.1.dev25/stackdiac/models/provider.py
--rw-r--r--   0        0        0     5276 2023-05-17 10:08:01.275455 stackdiac-0.0.1.dev25/stackdiac/models/repo.py
--rw-r--r--   0        0        0     1716 2023-05-17 10:08:01.275455 stackdiac-0.0.1.dev25/stackdiac/models/spec.py
--rw-r--r--   0        0        0     9330 2023-05-17 10:08:01.275455 stackdiac-0.0.1.dev25/stackdiac/models/stack.py
--rw-r--r--   0        0        0      108 2023-05-17 10:08:01.275455 stackdiac-0.0.1.dev25/stackdiac/stackd/__init__.py
--rw-r--r--   0        0        0      193 2023-05-17 10:08:01.275455 stackdiac-0.0.1.dev25/stackdiac/stackd/filters.py
--rw-r--r--   0        0        0      297 2023-05-17 10:08:01.275455 stackdiac-0.0.1.dev25/stackdiac/stackd/sdmod.py
--rw-r--r--   0        0        0    10541 2023-05-17 10:08:01.275455 stackdiac-0.0.1.dev25/stackdiac/stackd/stackd.py
--rw-r--r--   0        0        0   164360 2023-05-17 10:08:01.275455 stackdiac-0.0.1.dev25/stackdiac/ui/4753c5ba57962b4d7bf8.woff
--rw-r--r--   0        0        0   121340 2023-05-17 10:08:01.275455 stackdiac-0.0.1.dev25/stackdiac/ui/6d63d0501e5ed7b79dab.woff2
--rw-r--r--   0        0        0  1312554 2023-05-17 10:08:01.287455 stackdiac-0.0.1.dev25/stackdiac/ui/bundle.js
--rw-r--r--   0        0        0     2766 2023-05-17 10:08:01.287455 stackdiac-0.0.1.dev25/stackdiac/ui/bundle.js.LICENSE.txt
--rw-r--r--   0        0        0      415 2023-05-17 10:08:01.287455 stackdiac-0.0.1.dev25/stackdiac/ui/index.html
--rw-r--r--   0        0        0     2290 1970-01-01 00:00:00.000000 stackdiac-0.0.1.dev25/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/LICENSE
+-rw-r--r--   0        0        0     1415 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/README.md
+-rw-r--r--   0        0        0      592 2023-06-06 23:58:58.401808 stackdiac-0.0.1.dev26/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/stackdiac/__init__.py
+-rw-r--r--   0        0        0       23 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/stackdiac/api/__init__.py
+-rw-r--r--   0        0        0     1179 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/stackdiac/api/server.py
+-rw-r--r--   0        0        0     1800 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/stackdiac/cli/__init__.py
+-rw-r--r--   0        0        0      729 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/stackdiac/cli/build.py
+-rw-r--r--   0        0        0     1594 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/stackdiac/cli/create.py
+-rw-r--r--   0        0        0      464 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/stackdiac/cli/ui.py
+-rw-r--r--   0        0        0      381 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/stackdiac/models/__init__.py
+-rw-r--r--   0        0        0     1145 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/stackdiac/models/backend.py
+-rw-r--r--   0        0        0     2582 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/stackdiac/models/binary.py
+-rw-r--r--   0        0        0    12716 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/stackdiac/models/cluster.py
+-rw-r--r--   0        0        0     2769 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/stackdiac/models/config.py
+-rw-r--r--   0        0        0     2325 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/stackdiac/models/operation.py
+-rw-r--r--   0        0        0      161 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/stackdiac/models/provider.py
+-rw-r--r--   0        0        0     5276 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/stackdiac/models/repo.py
+-rw-r--r--   0        0        0      411 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/stackdiac/models/secret.py
+-rw-r--r--   0        0        0     1716 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/stackdiac/models/spec.py
+-rw-r--r--   0        0        0    12726 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/stackdiac/models/stack.py
+-rw-r--r--   0        0        0      108 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/stackdiac/stackd/__init__.py
+-rw-r--r--   0        0        0      193 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/stackdiac/stackd/filters.py
+-rw-r--r--   0        0        0      297 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/stackdiac/stackd/sdmod.py
+-rw-r--r--   0        0        0    11387 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/stackdiac/stackd/stackd.py
+-rw-r--r--   0        0        0   164360 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/stackdiac/ui/4753c5ba57962b4d7bf8.woff
+-rw-r--r--   0        0        0   121340 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/stackdiac/ui/6d63d0501e5ed7b79dab.woff2
+-rw-r--r--   0        0        0  2216438 2023-06-06 23:58:41.897349 stackdiac-0.0.1.dev26/stackdiac/ui/bundle.js
+-rw-r--r--   0        0        0     3087 2023-06-06 23:58:41.897349 stackdiac-0.0.1.dev26/stackdiac/ui/bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0      415 2023-06-06 23:58:41.897349 stackdiac-0.0.1.dev26/stackdiac/ui/index.html
+-rw-r--r--   0        0        0        0 2023-06-06 23:58:41.897349 stackdiac-0.0.1.dev26/stackdiac/views/__init__.py
+-rw-r--r--   0        0        0      780 2023-06-06 23:58:41.897349 stackdiac-0.0.1.dev26/stackdiac/views/module.py
+-rw-r--r--   0        0        0     2327 1970-01-01 00:00:00.000000 stackdiac-0.0.1.dev26/PKG-INFO
```

### Comparing `stackdiac-0.0.1.dev25/LICENSE` & `stackdiac-0.0.1.dev26/LICENSE`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev25/README.md` & `stackdiac-0.0.1.dev26/README.md`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev25/pyproject.toml` & `stackdiac-0.0.1.dev26/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stackdiac"
-version = "0.0.1-dev25"
+version = "0.0.1-dev26"
 description = ""
 authors = ["sysr9 <38893296+sysr9@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -15,14 +15,15 @@
 gitpython = "^3.1.31"
 requests = "^2.28.2"
 jinja2 = "^3.1.2"
 deepmerge = "^1.1.0"
 fastapi = "^0.95.0"
 uvicorn = "^0.21.1"
 mergedeep = "^1.3.4"
+hvac = "^1.1.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
```

### Comparing `stackdiac-0.0.1.dev25/stackdiac/api/server.py` & `stackdiac-0.0.1.dev26/stackdiac/api/server.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev25/stackdiac/cli/__init__.py` & `stackdiac-0.0.1.dev26/stackdiac/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev25/stackdiac/cli/build.py` & `stackdiac-0.0.1.dev26/stackdiac/cli/build.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev25/stackdiac/cli/create.py` & `stackdiac-0.0.1.dev26/stackdiac/cli/create.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev25/stackdiac/models/backend.py` & `stackdiac-0.0.1.dev26/stackdiac/models/backend.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev25/stackdiac/models/binary.py` & `stackdiac-0.0.1.dev26/stackdiac/models/binary.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev25/stackdiac/models/config.py` & `stackdiac-0.0.1.dev26/stackdiac/models/config.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev25/stackdiac/models/operation.py` & `stackdiac-0.0.1.dev26/stackdiac/models/operation.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,26 +15,52 @@
 #         name: hcloud-flannel
 #         modules: [pki, dns-zone, nodes, inventory, kubernetes, cluster-secret, hcloud-ccm]
 
 class Configuration(BaseModel):
     title: str | None = None
     name: str | None = None
     modules: list[str]
-    command: str = "plan"
+    command: str | list[str] = "plan"
 
-class Operation(BaseModel):
-    """
-    can be set in cluster config and in stack config
-    selected configuration configured via cluster config
-    """
+class PipelineStep(BaseModel):
+    module: str
+    title: str | None = None
+    command: str | list[str] = "apply"
+
+    def run(self, sd, cluster, cluster_stack, **kwargs):
+        if self.title is None:
+            self.title = f"run {self.command} on {self.module}"
+            
+        if self.command is not list:
+            self.command = self.command.split(" ")
+        
+        
+        sd.terragrunt(target=cluster_stack.stack.modules[self.module].built_vars["build_path"], 
+                      terragrunt_options=self.command, 
+                      cluster=cluster, **kwargs)
+        logger.info(f"finished running step <{self.title}>")
+
+
+class Operation(BaseModel):    
+    name: str | None = None
     configurations: dict[str, Configuration] = {}
     configuration: str = "default"
 
-    def run(self, sd, target, cluster, stack, **kwargs):
-        logger.info(f"{self} running operation {self} {self.configuration}")
+    pipeline: list[PipelineStep] = []
+    
+
+    def run(self, sd, target, cluster, cluster_stack, **kwargs):
+        logger.info(f"{self} running {len(self.pipeline)} steps pipeline")
+
+        for step in self.pipeline:
+            logger.info(f"running step {step}")
+            step.run(sd, cluster, cluster_stack, **kwargs)
+
+
+    def run_old(self, sd, target, cluster, stack, **kwargs):
         op = self.configurations[self.configuration]
         dest = os.path.join(sd.builddir, cluster.name, stack.name)
         args = ["run-all"]
         for module in op.modules:
             args.append("--terragrunt-include-dir")
             args.append(os.path.join(dest, module))
```

### Comparing `stackdiac-0.0.1.dev25/stackdiac/models/repo.py` & `stackdiac-0.0.1.dev26/stackdiac/models/repo.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev25/stackdiac/models/spec.py` & `stackdiac-0.0.1.dev26/stackdiac/models/spec.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev25/stackdiac/models/stack.py` & `stackdiac-0.0.1.dev26/stackdiac/models/stack.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 
 from urllib.parse import urlparse
-from pydantic import BaseModel, parse_obj_as
+from pydantic import BaseModel, parse_obj_as, Field
 from deepmerge import always_merger
 from copy import deepcopy
 import logging, os
 from typing import Any
+
+import yaml
 from stackdiac.models.backend import Backend
 from stackdiac.models.spec import Spec, SpecModel
 
 from stackdiac.models.operation import Operation
 from stackdiac.models.provider import Provider
 
+import hvac
+from enum import Enum
+
 logger = logging.getLogger(__name__)
 
         
 
 
 class Variable(BaseModel):
     """
@@ -31,50 +36,106 @@
     module_name: str
     stack_name: str
 
     @property
     def varname(self) -> str:
         return f"{self.stack_name}_{self.module_name}".replace("-", "_")
 
+class ModuleSecretStatus(Enum):
+    UNKNOWN = "unknown"
+    NOT_EXISTS = "not_exists"
+    EXISTS = "exists"
+    VALID   = "valid"
+
+class ModuleSecret(BaseModel):
+    name: str | None = None
+    secret_type: str | None = None
+    secret_schema: dict | None = None
+    required: bool = False
+    status: ModuleSecretStatus = ModuleSecretStatus.UNKNOWN
+
+    def build(self, cluster, cluster_stack, stack, sd, module, status, **kwargs):
+        logger.info(f"building secret {self.name} for {module.name}")
+
+        if self.secret_schema is None and self.secret_type is not None:
+            # extracting schema from stack.schema.components.schemas
+            self.secret_schema = stack.stack_schema['components']['schemas'][self.secret_type]
+            self.status = status
+
+class ModuleSchemas(BaseModel):
+    secrets: dict[str, ModuleSecret] = {}
+    vars: str | None = None
+
+    schemas: dict[str, Any] = {}
+
+    def build(self, cluster, cluster_stack, stack, sd, module, **kwargs):
+        logger.info(f"building schemas for {module.name}")
+
+        if self.vars:
+            self.schemas["vars"] = stack.stack_schema['components']['schemas'][self.vars]
+
+        # if self.secrets:
+        #     for name, secret in self.secrets.items():
+        #         secret.build(cluster, cluster_stack, stack, sd, module, status, **kwargs)
+        #         self.schemas[name] = SpecModel.parse_obj(secret.secret_schema)
 
 class Module(BaseModel):
     name: str | None = None
     source: str | None = None
     src: str | None = None
     vars: dict[str, Any] = {}
+    module_vars: dict[str, Any] = {}
     built_vars: dict[str, Any] = {}
     providers: list[str] = []
     provider_overrides: dict[str, Any] = {}
     inputs: list[str] = []
     deps: list[str] = []
     tf_state_key: str | None = None
     tf_state_bucket: str | None = None
     tf_state_bucket_region: str | None = None
     tf_backend: str = "s3"
     tf_backend_config: dict[str, Any] = {}
     backend: Backend | None = None
+    secrets: dict[str, ModuleSecret] = {}
+    schemas: ModuleSchemas | None = None
     
 
     def __str__(self) -> str:
         return f"<{self.__class__.__name__}:{self.name}>"
 
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
         if self.source:
             self.src = self.source            
 
+        for name, secret in self.secrets.items():
+            if secret.name is None:
+                secret.name = name
+
     @property
     def abssrc(self) -> str:
         from stackdiac.stackd import sd
         assert self.src
         return os.path.join(sd.root, self.src)
 
     @property
     def absdeps(self) -> list[str]:
         return [ os.path.join(os.path.dirname(self.abssrc), d) for d in self.deps ]
+    
+    
+    def build_vars_file(self, sd, cluster_stack, cluster, **kwargs) -> str:
+        return os.path.join(sd.root, "vars",  cluster.name, cluster_stack.name, self.name, "vars.yaml")
+    
+    def build_module_vars(self, sd, cluster_stack, cluster, **kwargs) -> dict[str, Any]:
+        vars_file = self.build_vars_file(sd, cluster_stack, cluster)
+        if os.path.exists(vars_file):
+            return yaml.load(open(vars_file), Loader=yaml.FullLoader)
+        else:
+            return {}
+   
 
     def build_deps(self, stack, module, cluster, deps:list[str], sd, **kwargs) -> list[ModuleDependency]:
         for d in deps:
             parts = [x for x in d.split("/") if x]
             if len(parts) == 2:
                 stack_name, module_name = parts
             elif len(parts) == 1:
@@ -140,14 +201,15 @@
             tg_abspath=self.abssrc,
             group="all", # legacy
             environment=cluster.name,
             ingress_host=self.get_ingress_host(cluster, stack),
             namespace=self.get_namespace(stack),
             charts_root=self.charts_root,
             module_secret=f"kv/{cluster.name}/module/{stack.name}/{self.name}",
+            module_secret_path=f"{cluster.name}/module/{stack.name}/{self.name}",
         )
 
     @property
     def tg_module_src(self):
         """
             adding // before last path component to avoid terragrunt to download the module 
         """
@@ -161,30 +223,36 @@
         #from stackdiac.stackd import sd
         path = sd.resolve_module_path(self.src)
         dest = self.get_build_dir(cluster, stack)
         os.makedirs(dest, exist_ok=True)
         _vars = {
             'build_path': dest,
             'module_path': path,
+            'project_root': sd.root,
         }
         
         varSources = [
             self.build_vars(sd, cluster, cluster_stack, stack, **kwargs),                      
         ]
         
         for v in varSources:
             always_merger.merge(_vars, deepcopy(v))       
         
         _build_vars = deepcopy(_vars)
 
+        self.module_vars = self.build_module_vars(sd, cluster_stack, cluster, **kwargs)
+
         for v in [
-            self.vars,
-            sd.conf.vars,
-            cluster.vars,
-            cluster_stack.vars]:
+                self.vars,
+                sd.conf.vars,
+                cluster.vars,
+                cluster_stack.vars,
+                cluster_stack.module_vars.get(self.name, {}),
+                self.module_vars
+                ]:
             always_merger.merge(_vars, deepcopy(v))
 
         self.built_vars = deepcopy(_vars)
 
         exclude_list = [
             "vault_address",
             "location",
@@ -222,14 +290,35 @@
                 else:
                     logger.warn(f"unknown type for var {k}={v} (type={type(v)})")
                     var_type = "string"
                 yield Variable(name=k, value=v, type=var_type)
         
         bk = self.backend or Backend()
 
+        # building secrets
+        vault_module_secrets = []
+        if self.secrets:
+            try:
+                resp = sd.vault.kv.v2.list_secrets(path=self.built_vars["module_secret_path"], mount_point='kv')
+            except hvac.exceptions.InvalidPath:
+                pass
+            else:
+                vault_module_secrets = resp["data"]["keys"]          
+
+
+        for s in self.secrets.values():
+            
+            status = ModuleSecretStatus.EXISTS if s.name in vault_module_secrets else ModuleSecretStatus.NOT_EXISTS
+            s.build(cluster, cluster_stack, stack, sd, module=self, status=status, **kwargs)
+        
+        # building schemas
+
+        if self.schemas:
+            self.schemas.build(cluster, cluster_stack, stack, sd, module=self, **kwargs)
+        
         ctx = dict(module=self, cluster=cluster, stackd=sd, vars=_vars, 
             inputs=list(self.build_deps(stack=stack, cluster=cluster, module=self, deps=self.inputs, sd=sd, **kwargs)),
             module_deps=[ d.abspath for d in list(self.build_deps(stack=stack, cluster=cluster, module=self, 
                 deps=self.deps, sd=sd, **kwargs)) ],
             vars_list=list(get_vars_list()),
             tf_backend=bk.build(sd, stack, self, cluster, cluster_stack, **kwargs),
              **kwargs)
@@ -257,14 +346,15 @@
     src: str | None = None
     example_vars: dict[str, Any] = {}  
     operations: dict[str, Operation] = {}
     modules: dict[str, Module]
     vars: dict[str, Any] = {}
     backend: Backend | None = None
     spec: SpecModel | None = None
+    stack_schema: Any = Field({}, alias="schema")
 
 
 class Stack(StackModel):
     spec: Spec | None = None
 
     class Config:
         orm_mode = True
```

### Comparing `stackdiac-0.0.1.dev25/stackdiac/stackd/stackd.py` & `stackdiac-0.0.1.dev26/stackdiac/stackd/stackd.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 from deepmerge import always_merger
 
 
 from stackdiac import models
 from stackdiac.models.provider import Provider
 from ..models import spec
 
+import hvac
+
 from . import filters
 
 logger = logging.getLogger(__name__)
 
 class StackdCounters(BaseModel):
     clusters: int = 0
     stacks: int = 0
@@ -51,20 +53,21 @@
     root: str = os.environ.get("STACKD_ROOT", ".")
     clusters: dict[str, models.ClusterModel] = {}    
     providers: dict[str, models.Provider] = {}
     
 class Stackd(StackdModel):
     conf: models.Config | None = None
     counters: StackdCounters = StackdCounters()
+    vault: hvac.Client | None = None
 
     class Config:
         # orm_mode = True
         exceptions = True
-        exclude = {"versions", "counters"}
-   #     exclude = {'clusters', 'versions', 'conf'}
+        exclude = {"versions", "counters", "vault"}   
+        arbitrary_types_allowed = True
 
     @property
     def dns_zone(self) -> str:
         return self.conf.project.domain
 
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
@@ -82,16 +85,14 @@
         
         spec = dict(
             ssh = {},
             remote = {},
             local = {},
         )
 
-        # server=tun@ssh.data.production.v10.link:22223&remote=mongodb-client.state:27017&local=dp-state-db.tun:27017
-
         qs = parse_qs(tunnel_qs)
 
         spec["ssh"]["username"], server_hostport = qs["server"][0].split("@")
         spec["ssh"]["host"], spec["ssh"]["port"] = server_hostport.split(":")
         spec["ssh"]["port"] = int(spec["ssh"]["port"])
 
         spec["remote"]["host"], spec["remote"]["port"] = qs["remote"][0].split(":")
@@ -119,14 +120,28 @@
         logger.debug(f"{self} chdir to {self.root}")
 
         self.conf = spec.Spec(path=self.config_file,
                 merge_from=models.get_initial_config(name="unconfigured", domain="example.com", 
                                                         vault_address="http://127.0.0.1:9090").dict()
                                             ).parse_obj_as(config.Config)
 
+        try:
+            self.vault = hvac.Client(url=self.conf.vars['vault_address'],
+                                    token=os.environ['TF_VAR_vault_token'])
+        except KeyError:
+            logger.error(f"{self} vault not configured. set TF_VAR_vault_token")
+            raise ProcessException("vault not configured. set TF_VAR_vault_token")
+        else:
+            logger.debug(f"{self} vault configured: {self.conf.vars['vault_address']}")
+
+        self.vault.secrets.kv.v2.configure(
+            max_versions=20,
+            mount_point='kv',
+        )
+
         # with open(self.config_file) as f:
         #     conf_data = models.get_initial_config(name="unconfigured", domain="example.com", vault_address="http://127.0.0.1:9090").dict()
         #     initial = copy.deepcopy(conf_data)
         #     data = yaml.safe_load(f.read())
         #     conf_data = always_merger.merge(conf_data, data)
         #     self.conf = parse_obj_as(config.Config, conf_data)
         #    # logger.debug(f"{self} loaded config: conf: {self.conf} \n\n data: {data} \n\n initial: {initial}\n\n")
@@ -261,14 +276,17 @@
     resolve_module_path = resolve_path
 
     def terragrunt(self, target, terragrunt_options:list[str], **kwargs):
         env = dict(
             TERRAGRUNT_WORKING_DIR=target,
             TERRAGRUNT_TFPATH=self.conf.binaries.terraform.abspath,
             TF_INPUT="false",
+            TERRAGRUNT_DOWNLOAD=os.path.join(self.cacheroot, "terragrunt-downloads"),
+            TERRAGRUNT_CACHE=os.path.join(self.cacheroot, "terragrunt-cache"),
+            TF_PLUGIN_CACHE_DIR=os.path.join(self.cacheroot, "terraform-plugins"),
         )
         opts = " ".join(terragrunt_options)
         cmd = f"{self.conf.binaries.terragrunt.abspath} {opts}"
         logger.debug(f"{self} terragrunt {target} {cmd} {env}")
 
         process = subprocess.Popen(cmd, shell=True, env=dict(**os.environ, **env))
         process.wait()
@@ -281,8 +299,10 @@
         running  self.terragrunt with configured module path
     
         """
         cluster, stack, operation = target.split("/")
         self.clusters[cluster].stacks[stack].build(cluster=self.clusters[cluster], sd=self, **kwargs)
         self.clusters[cluster].stacks[stack].stack.operations[operation].run(target=target, sd=self, 
             cluster=self.clusters[cluster],
-            stack=self.clusters[cluster].stacks[stack],**kwargs)
+            stack=self.clusters[cluster].stacks[stack],
+            cluster_stack=self.clusters[cluster].stacks[stack], # < more logical name
+            **kwargs)
```

### Comparing `stackdiac-0.0.1.dev25/stackdiac/ui/4753c5ba57962b4d7bf8.woff` & `stackdiac-0.0.1.dev26/stackdiac/ui/4753c5ba57962b4d7bf8.woff`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev25/stackdiac/ui/6d63d0501e5ed7b79dab.woff2` & `stackdiac-0.0.1.dev26/stackdiac/ui/6d63d0501e5ed7b79dab.woff2`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev25/stackdiac/ui/bundle.js.LICENSE.txt` & `stackdiac-0.0.1.dev26/stackdiac/ui/bundle.js.LICENSE.txt`

 * *Files 7% similar despite different names*

```diff
@@ -71,15 +71,15 @@
  * Copyright (c) Facebook, Inc. and its affiliates.
  *
  * This source code is licensed under the MIT license found in the
  * LICENSE file in the root directory of this source tree.
  */
 
 /**
- * @remix-run/router v1.4.0
+ * @remix-run/router v1.6.2
  *
  * Copyright (c) Remix Software Inc.
  *
  * This source code is licensed under the MIT license found in the
  * LICENSE.md file in the root directory of this source tree.
  *
  * @license MIT
@@ -91,15 +91,26 @@
  * @license MIT <https://opensource.org/licenses/MIT>
  * @author Lea Verou <https://lea.verou.me>
  * @namespace
  * @public
  */
 
 /**
- * React Router DOM v6.9.0
+ * React Router DOM v6.11.2
+ *
+ * Copyright (c) Remix Software Inc.
+ *
+ * This source code is licensed under the MIT license found in the
+ * LICENSE.md file in the root directory of this source tree.
+ *
+ * @license MIT
+ */
+
+/**
+ * React Router v6.11.2
  *
  * Copyright (c) Remix Software Inc.
  *
  * This source code is licensed under the MIT license found in the
  * LICENSE.md file in the root directory of this source tree.
  *
  * @license MIT
@@ -109,7 +120,9 @@
  * react-is.production.min.js
  *
  * Copyright (c) Facebook, Inc. and its affiliates.
  *
  * This source code is licensed under the MIT license found in the
  * LICENSE file in the root directory of this source tree.
  */
+
+/** @license URI.js v4.4.1 (c) 2011 Gary Court. License: http://github.com/garycourt/uri-js */
```

### Comparing `stackdiac-0.0.1.dev25/PKG-INFO` & `stackdiac-0.0.1.dev26/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: stackdiac
-Version: 0.0.1.dev25
+Version: 0.0.1.dev26
 Summary: 
 License: MIT
 Author: sysr9
 Author-email: 38893296+sysr9@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: coloredlogs (>=15.0.1,<16.0.0)
 Requires-Dist: deepmerge (>=1.1.0,<2.0.0)
 Requires-Dist: fastapi (>=0.95.0,<0.96.0)
 Requires-Dist: gitpython (>=3.1.31,<4.0.0)
+Requires-Dist: hvac (>=1.1.0,<2.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: mergedeep (>=1.3.4,<2.0.0)
 Requires-Dist: pydantic (>=1.10.6,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: uvicorn (>=0.21.1,<0.22.0)
 Description-Content-Type: text/markdown
```

