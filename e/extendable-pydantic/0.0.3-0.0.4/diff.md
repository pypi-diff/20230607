# Comparing `tmp/extendable_pydantic-0.0.3.tar.gz` & `tmp/extendable_pydantic-0.0.4.tar.gz`

## Comparing `extendable_pydantic-0.0.3.tar` & `extendable_pydantic-0.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 extendable_pydantic-0.0.3/extendable_pydantic_patcher.pth
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 extendable_pydantic-0.0.3/src/extendable_pydantic/__init__.py
--rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 extendable_pydantic-0.0.3/src/extendable_pydantic/_patch.py
--rw-r--r--   0        0        0     4538 2020-02-02 00:00:00.000000 extendable_pydantic-0.0.3/src/extendable_pydantic/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extendable_pydantic-0.0.3/src/extendable_pydantic/py.typed
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 extendable_pydantic-0.0.3/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 extendable_pydantic-0.0.3/LICENSE
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 extendable_pydantic-0.0.3/README.md
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 extendable_pydantic-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3318 2020-02-02 00:00:00.000000 extendable_pydantic-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 extendable_pydantic-0.0.4/extendable_pydantic_patcher.pth
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 extendable_pydantic-0.0.4/src/extendable_pydantic/__init__.py
+-rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 extendable_pydantic-0.0.4/src/extendable_pydantic/_patch.py
+-rw-r--r--   0        0        0     4538 2020-02-02 00:00:00.000000 extendable_pydantic-0.0.4/src/extendable_pydantic/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extendable_pydantic-0.0.4/src/extendable_pydantic/py.typed
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 extendable_pydantic-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 extendable_pydantic-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 extendable_pydantic-0.0.4/README.md
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 extendable_pydantic-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3442 2020-02-02 00:00:00.000000 extendable_pydantic-0.0.4/PKG-INFO
```

### Comparing `extendable_pydantic-0.0.3/src/extendable_pydantic/_patch.py` & `extendable_pydantic-0.0.4/src/extendable_pydantic/_patch.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,14 +9,22 @@
     # of the assembled class instead of the base class to make the extendable
     # models work with fastapi.
     def _model_process_schema_wrapper(wrapped, instance, args, kwargs):
         model = args[0]
         if hasattr(model, "_get_assembled_cls"):
             model = model._get_assembled_cls()
             args = (model,) + args[1:]
+            from pydantic import schema as schema_module
+
+            # we must also extend the list ok know model name to the
+            # assembled classes since fastapi by default restrict this list
+            # to the classes defined in the service definition
+            flat_models = schema_module.get_flat_models_from_models([model])
+            model_name_map = schema_module.get_model_name_map(flat_models)
+            kwargs["model_name_map"] = model_name_map
         return wrapped(*args, **kwargs)
 
     wrapt.wrap_function_wrapper(
         schema, "model_process_schema", _model_process_schema_wrapper
     )
```

### Comparing `extendable_pydantic-0.0.3/src/extendable_pydantic/main.py` & `extendable_pydantic-0.0.4/src/extendable_pydantic/main.py`

 * *Files identical despite different names*

### Comparing `extendable_pydantic-0.0.3/.gitignore` & `extendable_pydantic-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `extendable_pydantic-0.0.3/LICENSE` & `extendable_pydantic-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `extendable_pydantic-0.0.3/README.md` & `extendable_pydantic-0.0.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -32,7 +32,13 @@
 ```
 
 ## Development
 
 `pip install -e .`
 
 Then, copy `extendable_pydantic_patcher.pth` to `$VIRTUAL_ENV/lib/python3.10/site-packages`.
+
+## Release
+
+* Tag the sources: `git tag x.y.z`
+* Build the package: `hatch build`
+* Publish to pypi: `twine upload dist/*`
```

### Comparing `extendable_pydantic-0.0.3/pyproject.toml` & `extendable_pydantic-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `extendable_pydantic-0.0.3/PKG-INFO` & `extendable_pydantic-0.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extendable_pydantic
-Version: 0.0.3
+Version: 0.0.4
 Project-URL: Source, https://github.com/lmignon/extendable-pydantic
 Author-email: Laurent Mignon <laurent.mignon@acsone.eu>
 License: MIT License
         
         Copyright (c) 2021 Laurent Mignon (ACSONE)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -73,7 +73,13 @@
 ```
 
 ## Development
 
 `pip install -e .`
 
 Then, copy `extendable_pydantic_patcher.pth` to `$VIRTUAL_ENV/lib/python3.10/site-packages`.
+
+## Release
+
+* Tag the sources: `git tag x.y.z`
+* Build the package: `hatch build`
+* Publish to pypi: `twine upload dist/*`
```

