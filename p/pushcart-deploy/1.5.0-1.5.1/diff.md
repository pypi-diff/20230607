# Comparing `tmp/pushcart_deploy-1.5.0.tar.gz` & `tmp/pushcart_deploy-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pushcart_deploy-1.5.0.tar", max compression
+gzip compressed data, was "pushcart_deploy-1.5.1.tar", max compression
```

## Comparing `pushcart_deploy-1.5.0.tar` & `pushcart_deploy-1.5.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    35149 2023-06-06 13:03:09.684078 pushcart_deploy-1.5.0/LICENSE
--rw-r--r--   0        0        0       80 2023-06-06 13:03:09.684078 pushcart_deploy-1.5.0/README.md
--rw-r--r--   0        0        0     2502 2023-06-06 13:04:29.701108 pushcart_deploy-1.5.0/pyproject.toml
--rw-r--r--   0        0        0      483 2023-06-06 13:03:09.684078 pushcart_deploy-1.5.0/src/pushcart_deploy/__init__.py
--rw-r--r--   0        0        0    15446 2023-06-06 13:03:09.684078 pushcart_deploy-1.5.0/src/pushcart_deploy/configuration.py
--rw-r--r--   0        0        0      500 2023-06-06 13:03:09.684078 pushcart_deploy-1.5.0/src/pushcart_deploy/databricks_api/__init__.py
--rw-r--r--   0        0        0     3482 2023-06-06 13:03:09.684078 pushcart_deploy-1.5.0/src/pushcart_deploy/databricks_api/jobs_wrapper.py
--rw-r--r--   0        0        0     4706 2023-06-06 13:03:09.684078 pushcart_deploy-1.5.0/src/pushcart_deploy/databricks_api/pipelines_wrapper.py
--rw-r--r--   0        0        0     4496 2023-06-06 13:03:09.684078 pushcart_deploy-1.5.0/src/pushcart_deploy/databricks_api/repos_wrapper.py
--rw-r--r--   0        0        0    12091 2023-06-06 13:03:09.684078 pushcart_deploy-1.5.0/src/pushcart_deploy/databricks_api/scheduler.py
--rw-r--r--   0        0        0     3173 2023-06-06 13:03:09.684078 pushcart_deploy-1.5.0/src/pushcart_deploy/databricks_api/secrets_wrapper.py
--rw-r--r--   0        0        0      254 2023-06-06 13:03:09.684078 pushcart_deploy-1.5.0/src/pushcart_deploy/databricks_api/settings/__init__.py
--rw-r--r--   0        0        0     4385 2023-06-06 13:03:09.684078 pushcart_deploy-1.5.0/src/pushcart_deploy/databricks_api/settings/base_settings.py
--rw-r--r--   0        0        0     4175 2023-06-06 13:03:09.684078 pushcart_deploy-1.5.0/src/pushcart_deploy/databricks_api/settings/job_settings.py
--rw-r--r--   0        0        0     6882 2023-06-06 13:03:09.684078 pushcart_deploy-1.5.0/src/pushcart_deploy/databricks_api/settings/pipeline_settings.py
--rw-r--r--   0        0        0     9394 2023-06-06 13:03:09.684078 pushcart_deploy-1.5.0/src/pushcart_deploy/metadata.py
--rw-r--r--   0        0        0     4201 2023-06-06 13:03:09.684078 pushcart_deploy-1.5.0/src/pushcart_deploy/setup.py
--rw-r--r--   0        0        0     3397 2023-06-06 13:03:09.684078 pushcart_deploy-1.5.0/src/pushcart_deploy/validation.py
--rw-r--r--   0        0        0     1285 1970-01-01 00:00:00.000000 pushcart_deploy-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-07 20:53:48.103196 pushcart_deploy-1.5.1/LICENSE
+-rw-r--r--   0        0        0       80 2023-06-07 20:53:48.103196 pushcart_deploy-1.5.1/README.md
+-rw-r--r--   0        0        0     2502 2023-06-07 20:55:12.632576 pushcart_deploy-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0      483 2023-06-07 20:53:48.103196 pushcart_deploy-1.5.1/src/pushcart_deploy/__init__.py
+-rw-r--r--   0        0        0    15944 2023-06-07 20:53:48.103196 pushcart_deploy-1.5.1/src/pushcart_deploy/configuration.py
+-rw-r--r--   0        0        0      500 2023-06-07 20:53:48.103196 pushcart_deploy-1.5.1/src/pushcart_deploy/databricks_api/__init__.py
+-rw-r--r--   0        0        0     3482 2023-06-07 20:53:48.103196 pushcart_deploy-1.5.1/src/pushcart_deploy/databricks_api/jobs_wrapper.py
+-rw-r--r--   0        0        0     4706 2023-06-07 20:53:48.103196 pushcart_deploy-1.5.1/src/pushcart_deploy/databricks_api/pipelines_wrapper.py
+-rw-r--r--   0        0        0     4496 2023-06-07 20:53:48.103196 pushcart_deploy-1.5.1/src/pushcart_deploy/databricks_api/repos_wrapper.py
+-rw-r--r--   0        0        0    12091 2023-06-07 20:53:48.103196 pushcart_deploy-1.5.1/src/pushcart_deploy/databricks_api/scheduler.py
+-rw-r--r--   0        0        0     3173 2023-06-07 20:53:48.107196 pushcart_deploy-1.5.1/src/pushcart_deploy/databricks_api/secrets_wrapper.py
+-rw-r--r--   0        0        0      254 2023-06-07 20:53:48.107196 pushcart_deploy-1.5.1/src/pushcart_deploy/databricks_api/settings/__init__.py
+-rw-r--r--   0        0        0     4385 2023-06-07 20:53:48.107196 pushcart_deploy-1.5.1/src/pushcart_deploy/databricks_api/settings/base_settings.py
+-rw-r--r--   0        0        0     4175 2023-06-07 20:53:48.107196 pushcart_deploy-1.5.1/src/pushcart_deploy/databricks_api/settings/job_settings.py
+-rw-r--r--   0        0        0     6882 2023-06-07 20:53:48.107196 pushcart_deploy-1.5.1/src/pushcart_deploy/databricks_api/settings/pipeline_settings.py
+-rw-r--r--   0        0        0     9661 2023-06-07 20:53:48.107196 pushcart_deploy-1.5.1/src/pushcart_deploy/metadata.py
+-rw-r--r--   0        0        0     4201 2023-06-07 20:53:48.107196 pushcart_deploy-1.5.1/src/pushcart_deploy/setup.py
+-rw-r--r--   0        0        0     3397 2023-06-07 20:53:48.107196 pushcart_deploy-1.5.1/src/pushcart_deploy/validation.py
+-rw-r--r--   0        0        0     1285 1970-01-01 00:00:00.000000 pushcart_deploy-1.5.1/PKG-INFO
```

### Comparing `pushcart_deploy-1.5.0/LICENSE` & `pushcart_deploy-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pushcart_deploy-1.5.0/pyproject.toml` & `pushcart_deploy-1.5.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -74,15 +74,15 @@
   "YTT",
 ]
 unfixable = []
 exclude = [".venv", "tests"]
 
 [tool.poetry]
 name = "pushcart-deploy"
-version = "1.5.0"
+version = "1.5.1"
 description = "Deployment helper for pipeline configurations using Pushcart"
 authors = ["Georgel Preput <georgelpreput@mailbox.org>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 classifiers = [
   "Programming Language :: Python :: 3.10",
   "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
```

### Comparing `pushcart_deploy-1.5.0/src/pushcart_deploy/configuration.py` & `pushcart_deploy-1.5.1/src/pushcart_deploy/configuration.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,14 +66,31 @@
         csv_file = StringIO(contents)
         reader = csv.DictReader(csv_file)
 
         for row in reader:
             yield row
 
 
+async def get_transformations_from_sql(sql_path: Path | str) -> str:
+    """Return transformations from SQL file.
+
+    Parameters
+    ----------
+    sql_path : Path | str
+        Path to an existing .sql file
+
+    Returns
+    -------
+    str
+        SQL string from input file
+    """
+    async with aiofiles.open(sql_path, "r") as sql_file:
+        return await sql_file.read()
+
+
 def expect_at_most_one_file(settings_path: Path | str) -> Path | None:
     """Check whether there is at most one configuration file for the given path.
 
     Parameters
     ----------
     settings_path : Path | str
         Path to a configuration file, may omit extension
@@ -266,15 +283,15 @@
 
     target_catalog_name: constr(strip_whitespace=True, min_length=1, strict=True)
     target_schema_name: constr(strip_whitespace=True, min_length=1, strict=True)
     pipeline_name: constr(strip_whitespace=True, min_length=1, strict=True)
 
     origin: constr(min_length=1, strict=True)
     target: constr(min_length=1, strict=True)
-    column_order: conint(ge=1) | None = None
+    column_order: conint(ge=1) | None = 1
     source_column_name: constr(strict=True) | None = None
     source_column_type: constr(
         strict=True,
         regex="\\A(string|int|double|date|timestamp|boolean|struct|array|map)\\Z",
     ) | None = None
     dest_column_name: constr(strict=True) | None = None
     dest_column_type: constr(
@@ -286,18 +303,24 @@
     default_value: constr(strict=True) | None = None
     validations: list[Validation] | None = Field(default_factory=list)
 
     @root_validator(pre=True)
     @classmethod
     def check_only_one_of_config_or_sql_query_defined(cls, values: dict) -> dict:
         """Check that one and only one of the config or sql_query fields is defined."""
-        if not any(values.get(v) is not None for v in ["column_order", "sql_query"]):
+        if not any(
+            values.get(v) is not None
+            for v in ["source_column_name", "dest_column_name", "sql_query"]
+        ):
             msg = f"No transformation defined. Please provide either a config or a sql_query.\nGot: {values}"
             raise ValueError(msg)
-        if all(values.get(t) for t in ["column_order", "sql_query"]):
+        if all(
+            values.get(t)
+            for t in ["source_column_name", "dest_column_name", "sql_query"]
+        ):
             msg = f"Only one of config or sql_query allowed.\nGot: {values}"
             raise ValueError(msg)
         return values
 
     @validator("validations")
     @classmethod
     def check_multiple_validations_with_same_rule(cls, value: dict) -> dict:
```

### Comparing `pushcart_deploy-1.5.0/src/pushcart_deploy/databricks_api/jobs_wrapper.py` & `pushcart_deploy-1.5.1/src/pushcart_deploy/databricks_api/jobs_wrapper.py`

 * *Files identical despite different names*

### Comparing `pushcart_deploy-1.5.0/src/pushcart_deploy/databricks_api/pipelines_wrapper.py` & `pushcart_deploy-1.5.1/src/pushcart_deploy/databricks_api/pipelines_wrapper.py`

 * *Files identical despite different names*

### Comparing `pushcart_deploy-1.5.0/src/pushcart_deploy/databricks_api/repos_wrapper.py` & `pushcart_deploy-1.5.1/src/pushcart_deploy/databricks_api/repos_wrapper.py`

 * *Files identical despite different names*

### Comparing `pushcart_deploy-1.5.0/src/pushcart_deploy/databricks_api/scheduler.py` & `pushcart_deploy-1.5.1/src/pushcart_deploy/databricks_api/scheduler.py`

 * *Files identical despite different names*

### Comparing `pushcart_deploy-1.5.0/src/pushcart_deploy/databricks_api/secrets_wrapper.py` & `pushcart_deploy-1.5.1/src/pushcart_deploy/databricks_api/secrets_wrapper.py`

 * *Files identical despite different names*

### Comparing `pushcart_deploy-1.5.0/src/pushcart_deploy/databricks_api/settings/base_settings.py` & `pushcart_deploy-1.5.1/src/pushcart_deploy/databricks_api/settings/base_settings.py`

 * *Files identical despite different names*

### Comparing `pushcart_deploy-1.5.0/src/pushcart_deploy/databricks_api/settings/job_settings.py` & `pushcart_deploy-1.5.1/src/pushcart_deploy/databricks_api/settings/job_settings.py`

 * *Files identical despite different names*

### Comparing `pushcart_deploy-1.5.0/src/pushcart_deploy/databricks_api/settings/pipeline_settings.py` & `pushcart_deploy-1.5.1/src/pushcart_deploy/databricks_api/settings/pipeline_settings.py`

 * *Files identical despite different names*

### Comparing `pushcart_deploy-1.5.0/src/pushcart_deploy/metadata.py` & `pushcart_deploy-1.5.1/src/pushcart_deploy/metadata.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,28 +11,28 @@
 Requires Databricks CLI to already be configured for your target Databricks environment
 
 """
 
 import asyncio
 import json
 import logging
-from collections import defaultdict
+from collections.abc import AsyncIterator
+from copy import deepcopy
 from dataclasses import asdict
 from glob import glob
-from itertools import groupby
-from operator import itemgetter
 from pathlib import Path
 
 from databricks.connect import DatabricksSession
 from pydantic import DirectoryPath, dataclasses
 
 from pushcart_deploy.configuration import (
     Configuration,
     get_config_from_file,
     get_transformations_from_csv,
+    get_transformations_from_sql,
 )
 from pushcart_deploy.validation import sanitize_empty_objects
 
 
 @dataclasses.dataclass
 class Metadata:
     """Read pipeline configuration files and create backend objects in Databricks.
@@ -56,17 +56,24 @@
     @staticmethod
     async def _load_pipeline_with_metadata(file_path: str) -> dict:
         config = await get_config_from_file(file_path)
         if config is None:
             return None
 
         file_path_obj = Path(file_path)
-        config["pipeline_name"] = file_path_obj.parent.name
-        config["target_schema_name"] = file_path_obj.parent.parent.name
-        config["target_catalog_name"] = file_path_obj.parent.parent.parent.name
+        metadata = {
+            "pipeline_name": file_path_obj.parent.name,
+            "target_schema_name": file_path_obj.parent.parent.name,
+            "target_catalog_name": file_path_obj.parent.parent.parent.name,
+        }
+
+        for key in ["sources", "transformations", "destinations"]:
+            if key in config:
+                for item in config[key]:
+                    item.update(metadata)
 
         if config.get("transformations"):
             for transformation in config["transformations"]:
                 if (
                     transformation.get("config")
                     and not Path(transformation["config"]).is_file()
                 ):
@@ -92,102 +99,108 @@
 
     @staticmethod
     async def _enrich_sources_config(sources_config: list) -> None:
         for source_dict in sources_config:
             if isinstance(source_dict.get("params"), dict):
                 source_dict["params"] = json.dumps(source_dict.get("params", {}))
 
+        return {"sources": sources_config}
+
     @staticmethod
-    async def _enrich_transformations_config(transformations_config: list) -> None:
-        for transformation_config in transformations_config:
-            if csv_path := transformation_config.get("config"):
-                async for row in get_transformations_from_csv(Path(csv_path).resolve()):
-                    row["column_order"] = (
-                        int(row["column_order"])
-                        if str(row["column_order"]).isdigit()
-                        else None
-                    )
-                    row["origin"] = transformation_config["origin"]
-                    row["target"] = transformation_config["target"]
+    async def _handle_csv_transformations(
+        transformation: dict,
+        config_path: Path,
+    ) -> AsyncIterator[dict]:
+        async for row in get_transformations_from_csv(config_path.resolve()):
+            row["column_order"] = (
+                int(row["column_order"]) if str(row["column_order"]).isdigit() else None
+            )
+
+            row.update(
+                origin=transformation["origin"],
+                target=transformation["target"],
+                target_catalog_name=transformation["target_catalog_name"],
+                target_schema_name=transformation["target_schema_name"],
+                pipeline_name=transformation["pipeline_name"],
+            )
+
+            if row.get("validation_rule") and row.get("validation_action"):
+                row["validations"] = [
+                    {
+                        "validation_rule": row["validation_rule"],
+                        "validation_action": row["validation_action"],
+                    },
+                ]
+                del row["validation_rule"], row["validation_action"]
+
+            yield row
+
+    @staticmethod
+    async def _handle_sql_transformations(
+        transformation: dict,
+        config_path: Path,
+    ) -> dict:
+        sql_transformation = deepcopy(transformation)
+        sql_transformation["sql_query"] = await get_transformations_from_sql(
+            config_path.resolve(),
+        )
 
-                    if row.get("validation_rule") and row.get("validation_action"):
-                        row["validations"] = [
-                            {
-                                "validation_rule": row["validation_rule"],
-                                "validation_action": row["validation_action"],
-                            },
-                        ]
-                        del row["validation_rule"]
-                        del row["validation_action"]
+        del sql_transformation["config"]
 
-                    transformations_config.append(row)
-                transformations_config.remove(transformation_config)
+        return sql_transformation
+
+    async def _enrich_transformations_config(
+        self,
+        transformations_config: list,
+    ) -> None:
+        enriched_transformations = []
+
+        for t in transformations_config:
+            if t.get("config"):
+                config_path = Path(t["config"])
+                if config_path.suffix == ".csv":
+                    async for row in self._handle_csv_transformations(t, config_path):
+                        enriched_transformations.append(row)
+                elif config_path.suffix == ".sql":
+                    enriched_transformations.append(
+                        await self._handle_sql_transformations(t, config_path),
+                    )
+                else:
+                    msg = "Transformation configurations can only be .csv or .sql files"
+                    raise TypeError(msg)
+
+        return {
+            "transformations": [t for t in transformations_config if "config" not in t]
+            + enriched_transformations,
+        }
 
     @staticmethod
     async def _enrich_destinations_config(destinations_config: list) -> None:
-        pass
+        return {"destinations": destinations_config}
 
     async def _enrich_pipeline_configs(self, pipeline_configs: list) -> None:
         enrichment_func = {
             "sources": self._enrich_sources_config,
             "transformations": self._enrich_transformations_config,
             "destinations": self._enrich_destinations_config,
         }
 
-        await asyncio.gather(
+        return await asyncio.gather(
             *[
                 enrichment_func[stage_name](stage_config)
                 for pipeline_config in pipeline_configs
                 for stage_name, stage_config in pipeline_config.items()
                 if stage_name in enrichment_func
             ],
         )
 
-    @staticmethod
-    def _group_pipeline_configs(pipeline_configs: list) -> list:
-        sorted_pipeline_configs = sorted(
-            pipeline_configs,
-            key=itemgetter(
-                "target_catalog_name",
-                "target_schema_name",
-                "pipeline_name",
-            ),
-        )
-        grouped_elements = groupby(
-            sorted_pipeline_configs,
-            key=itemgetter(
-                "target_catalog_name",
-                "target_schema_name",
-                "pipeline_name",
-            ),
-        )
-
-        grouped_pipeline_configs = []
-
-        for (catalog, schema, pipeline), group in grouped_elements:
-            merged_pipeline_stages_dict = defaultdict(list)
-            for d in group:
-                for k, v in d.items():
-                    if isinstance(v, list):
-                        for item in v:
-                            item["target_catalog_name"] = catalog
-                            item["target_schema_name"] = schema
-                            item["pipeline_name"] = pipeline
-                        merged_pipeline_stages_dict[k].extend(v)
-
-            grouped_pipeline_configs.append(dict(merged_pipeline_stages_dict))
-
-        return grouped_pipeline_configs
-
     def _validate_pipeline_configs(self, pipeline_configs: list) -> None:
-        grouped_pipeline_configs = self._group_pipeline_configs(pipeline_configs)
-
         validated_pipeline_configs = []
 
-        for pipeline_config in grouped_pipeline_configs:
+        for pipeline_config in pipeline_configs:
             validated_pipeline_configs.append(Configuration(**pipeline_config))
 
         return validated_pipeline_configs
 
     def _create_metadata_tables(self, pipeline_configs: list) -> None:
         spark = DatabricksSession.builder.getOrCreate()
 
@@ -211,16 +224,20 @@
             )
 
             self.log.info(f"Wrote {stage_name} metadata table.")
 
     def create_backend_objects(self) -> None:
         """Create metadata tables holding pipeline stages."""
         pipeline_configs = asyncio.run(self._collect_pipeline_configs())
-        asyncio.run(self._enrich_pipeline_configs(pipeline_configs))
-        validated_pipeline_configs = self._validate_pipeline_configs(pipeline_configs)
+        enriched_pipeline_configs = asyncio.run(
+            self._enrich_pipeline_configs(pipeline_configs),
+        )
+        validated_pipeline_configs = self._validate_pipeline_configs(
+            enriched_pipeline_configs,
+        )
         self._create_metadata_tables(validated_pipeline_configs)
 
     @staticmethod
     def get_pipeline_list_from_backend_objects() -> list:
         """Get a list of dicts with all the pipelines available in the metadata tables.
 
         Returns
```

### Comparing `pushcart_deploy-1.5.0/src/pushcart_deploy/setup.py` & `pushcart_deploy-1.5.1/src/pushcart_deploy/setup.py`

 * *Files identical despite different names*

### Comparing `pushcart_deploy-1.5.0/src/pushcart_deploy/validation.py` & `pushcart_deploy-1.5.1/src/pushcart_deploy/validation.py`

 * *Files identical despite different names*

### Comparing `pushcart_deploy-1.5.0/PKG-INFO` & `pushcart_deploy-1.5.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pushcart-deploy
-Version: 1.5.0
+Version: 1.5.1
 Summary: Deployment helper for pipeline configurations using Pushcart
 License: GPL-3.0-or-later
 Author: Georgel Preput
 Author-email: georgelpreput@mailbox.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

