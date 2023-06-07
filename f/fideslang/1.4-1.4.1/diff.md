# Comparing `tmp/fideslang-1.4.tar.gz` & `tmp/fideslang-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fideslang-1.4.tar", last modified: Wed May 31 15:23:42 2023, max compression
+gzip compressed data, was "fideslang-1.4.1.tar", last modified: Wed Jun  7 19:00:34 2023, max compression
```

## Comparing `fideslang-1.4.tar` & `fideslang-1.4.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:23:42.411170 fideslang-1.4/
--rw-r--r--   0 runner    (1001) docker     (123)    18656 2023-05-31 15:23:37.000000 fideslang-1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-31 15:23:37.000000 fideslang-1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-05-31 15:23:42.411170 fideslang-1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-05-31 15:23:37.000000 fideslang-1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-31 15:23:37.000000 fideslang-1.4/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-05-31 15:23:37.000000 fideslang-1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-31 15:23:37.000000 fideslang-1.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-31 15:23:42.411170 fideslang-1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-31 15:23:37.000000 fideslang-1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:23:42.407170 fideslang-1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:23:42.411170 fideslang-1.4/src/fideslang/
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-31 15:23:37.000000 fideslang-1.4/src/fideslang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-31 15:23:42.411170 fideslang-1.4/src/fideslang/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    12917 2023-05-31 15:23:37.000000 fideslang-1.4/src/fideslang/default_fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:23:42.411170 fideslang-1.4/src/fideslang/default_taxonomy/
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-31 15:23:37.000000 fideslang-1.4/src/fideslang/default_taxonomy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15437 2023-05-31 15:23:37.000000 fideslang-1.4/src/fideslang/default_taxonomy/data_categories.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-05-31 15:23:37.000000 fideslang-1.4/src/fideslang/default_taxonomy/data_qualifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-05-31 15:23:37.000000 fideslang-1.4/src/fideslang/default_taxonomy/data_subjects.py
--rw-r--r--   0 runner    (1001) docker     (123)    14996 2023-05-31 15:23:37.000000 fideslang-1.4/src/fideslang/default_taxonomy/data_uses.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-31 15:23:37.000000 fideslang-1.4/src/fideslang/default_taxonomy/organizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-31 15:23:37.000000 fideslang-1.4/src/fideslang/manifests.py
--rw-r--r--   0 runner    (1001) docker     (123)    35055 2023-05-31 15:23:37.000000 fideslang-1.4/src/fideslang/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-31 15:23:37.000000 fideslang-1.4/src/fideslang/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:23:37.000000 fideslang-1.4/src/fideslang/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-31 15:23:37.000000 fideslang-1.4/src/fideslang/relationships.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-31 15:23:37.000000 fideslang-1.4/src/fideslang/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-05-31 15:23:37.000000 fideslang-1.4/src/fideslang/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:23:42.407170 fideslang-1.4/src/fideslang.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-05-31 15:23:42.000000 fideslang-1.4/src/fideslang.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-31 15:23:42.000000 fideslang-1.4/src/fideslang.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 15:23:42.000000 fideslang-1.4/src/fideslang.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-31 15:23:42.000000 fideslang-1.4/src/fideslang.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-31 15:23:42.000000 fideslang-1.4/src/fideslang.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    57971 2023-05-31 15:23:37.000000 fideslang-1.4/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:00:34.811407 fideslang-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    18656 2023-06-07 19:00:29.000000 fideslang-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-07 19:00:29.000000 fideslang-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-06-07 19:00:34.811407 fideslang-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-06-07 19:00:29.000000 fideslang-1.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-07 19:00:29.000000 fideslang-1.4.1/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-06-07 19:00:29.000000 fideslang-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-07 19:00:29.000000 fideslang-1.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-07 19:00:34.811407 fideslang-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-07 19:00:29.000000 fideslang-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:00:34.807407 fideslang-1.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:00:34.811407 fideslang-1.4.1/src/fideslang/
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-07 19:00:29.000000 fideslang-1.4.1/src/fideslang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-07 19:00:34.811407 fideslang-1.4.1/src/fideslang/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12917 2023-06-07 19:00:29.000000 fideslang-1.4.1/src/fideslang/default_fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:00:34.811407 fideslang-1.4.1/src/fideslang/default_taxonomy/
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-06-07 19:00:29.000000 fideslang-1.4.1/src/fideslang/default_taxonomy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15437 2023-06-07 19:00:29.000000 fideslang-1.4.1/src/fideslang/default_taxonomy/data_categories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-06-07 19:00:29.000000 fideslang-1.4.1/src/fideslang/default_taxonomy/data_qualifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-06-07 19:00:29.000000 fideslang-1.4.1/src/fideslang/default_taxonomy/data_subjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14996 2023-06-07 19:00:29.000000 fideslang-1.4.1/src/fideslang/default_taxonomy/data_uses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-07 19:00:29.000000 fideslang-1.4.1/src/fideslang/default_taxonomy/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-06-07 19:00:29.000000 fideslang-1.4.1/src/fideslang/manifests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34869 2023-06-07 19:00:29.000000 fideslang-1.4.1/src/fideslang/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-07 19:00:29.000000 fideslang-1.4.1/src/fideslang/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:00:29.000000 fideslang-1.4.1/src/fideslang/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-07 19:00:29.000000 fideslang-1.4.1/src/fideslang/relationships.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-07 19:00:29.000000 fideslang-1.4.1/src/fideslang/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-06-07 19:00:29.000000 fideslang-1.4.1/src/fideslang/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:00:34.811407 fideslang-1.4.1/src/fideslang.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-06-07 19:00:34.000000 fideslang-1.4.1/src/fideslang.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-06-07 19:00:34.000000 fideslang-1.4.1/src/fideslang.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 19:00:34.000000 fideslang-1.4.1/src/fideslang.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-07 19:00:34.000000 fideslang-1.4.1/src/fideslang.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-07 19:00:34.000000 fideslang-1.4.1/src/fideslang.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    57971 2023-06-07 19:00:29.000000 fideslang-1.4.1/versioneer.py
```

### Comparing `fideslang-1.4/LICENSE` & `fideslang-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fideslang-1.4/PKG-INFO` & `fideslang-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fideslang
-Version: 1.4
+Version: 1.4.1
 Summary: Fides Taxonomy Language
 Home-page: https://github.com/ethyca/fideslang
 Author: Ethyca, Inc.
 Author-email: fidesteam@ethyca.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `fideslang-1.4/README.md` & `fideslang-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `fideslang-1.4/pyproject.toml` & `fideslang-1.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fideslang-1.4/setup.cfg` & `fideslang-1.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `fideslang-1.4/setup.py` & `fideslang-1.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `fideslang-1.4/src/fideslang/__init__.py` & `fideslang-1.4.1/src/fideslang/__init__.py`

 * *Files identical despite different names*

### Comparing `fideslang-1.4/src/fideslang/default_fixtures.py` & `fideslang-1.4.1/src/fideslang/default_fixtures.py`

 * *Files identical despite different names*

### Comparing `fideslang-1.4/src/fideslang/default_taxonomy/__init__.py` & `fideslang-1.4.1/src/fideslang/default_taxonomy/__init__.py`

 * *Files identical despite different names*

### Comparing `fideslang-1.4/src/fideslang/default_taxonomy/data_categories.py` & `fideslang-1.4.1/src/fideslang/default_taxonomy/data_categories.py`

 * *Files identical despite different names*

### Comparing `fideslang-1.4/src/fideslang/default_taxonomy/data_qualifiers.py` & `fideslang-1.4.1/src/fideslang/default_taxonomy/data_qualifiers.py`

 * *Files identical despite different names*

### Comparing `fideslang-1.4/src/fideslang/default_taxonomy/data_subjects.py` & `fideslang-1.4.1/src/fideslang/default_taxonomy/data_subjects.py`

 * *Files identical despite different names*

### Comparing `fideslang-1.4/src/fideslang/default_taxonomy/data_uses.py` & `fideslang-1.4.1/src/fideslang/default_taxonomy/data_uses.py`

 * *Files identical despite different names*

### Comparing `fideslang-1.4/src/fideslang/manifests.py` & `fideslang-1.4.1/src/fideslang/manifests.py`

 * *Files identical despite different names*

### Comparing `fideslang-1.4/src/fideslang/models.py` & `fideslang-1.4.1/src/fideslang/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,34 +29,39 @@
     matching_parent_key,
     no_self_reference,
     parse_data_type_string,
     sort_list_objects_by_name,
     valid_data_type,
 )
 
-# Reusable components
+# Reusable Validators
 country_code_validator = validator("third_country_transfers", allow_reuse=True)(
     check_valid_country_code
 )
 
 matching_parent_key_validator = validator("parent_key", allow_reuse=True, always=True)(
     matching_parent_key
 )
 no_self_reference_validator = validator("parent_key", allow_reuse=True)(
     no_self_reference
 )
 
+# Reusable Fields
 name_field = Field(description="Human-Readable name for this resource.")
 description_field = Field(
     description="A detailed description of what this resource is."
 )
 is_default_field = Field(
     default=False,
     description="Denotes whether the resource is part of the default taxonomy or not.",
 )
+meta_field = Field(
+    default=None,
+    description="An optional property to store any extra information for a resource. Data can be structured in any way: simple set of `key: value` pairs or deeply nested objects.",
+)
 
 
 # Fides Base Model
 class FidesModel(BaseModel):
     """The base model for all Fides Resources."""
 
     fides_key: FidesKey = Field(
@@ -525,17 +530,15 @@
     resource_id: Optional[str]
     after: Optional[List[FidesKey]]
 
 
 class Dataset(FidesModel, FidesopsMetaBackwardsCompat):
     """The Dataset resource model."""
 
-    meta: Optional[Dict[str, str]] = Field(
-        description="An optional object that provides additional information about the Dataset. You can structure the object however you like. It can be a simple set of `key: value` properties or a deeply nested hierarchy of objects. How you use the object is up to you: Fides ignores it."
-    )
+    meta: Optional[Dict] = meta_field
     data_categories: Optional[List[FidesKey]] = Field(
         description="Array of Data Category resources identified by `fides_key`, that apply to all collections in the Dataset.",
     )
     data_qualifier: FidesKey = Field(
         default="aggregated.anonymized.unlinked_pseudonymized.pseudonymized.identified",
         description="Array of Data Qualifier resources identified by `fides_key`, that apply to all collections in the Dataset.",
     )
@@ -918,17 +921,15 @@
 
     Describes an application and includes a list of PrivacyDeclaration resources.
     """
 
     registry_id: Optional[int] = Field(
         description="The id of the system registry, if used.",
     )
-    meta: Optional[Dict[str, str]] = Field(
-        description="An optional property to store any extra information for a system. Not used by fidesctl.",
-    )
+    meta: Optional[Dict] = meta_field
     fidesctl_meta: Optional[SystemMetadata] = Field(
         description=SystemMetadata.__doc__,
     )
     system_type: str = Field(
         description="A required value to describe the type of system being modeled, examples include: Service, Application, Third Party, etc.",
     )
     data_responsibility_title: DataResponsibilityTitle = Field(
```

### Comparing `fideslang-1.4/src/fideslang/parse.py` & `fideslang-1.4.1/src/fideslang/parse.py`

 * *Files identical despite different names*

### Comparing `fideslang-1.4/src/fideslang/relationships.py` & `fideslang-1.4.1/src/fideslang/relationships.py`

 * *Files identical despite different names*

### Comparing `fideslang-1.4/src/fideslang/utils.py` & `fideslang-1.4.1/src/fideslang/utils.py`

 * *Files identical despite different names*

### Comparing `fideslang-1.4/src/fideslang/validation.py` & `fideslang-1.4.1/src/fideslang/validation.py`

 * *Files identical despite different names*

### Comparing `fideslang-1.4/src/fideslang.egg-info/PKG-INFO` & `fideslang-1.4.1/src/fideslang.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fideslang
-Version: 1.4
+Version: 1.4.1
 Summary: Fides Taxonomy Language
 Home-page: https://github.com/ethyca/fideslang
 Author: Ethyca, Inc.
 Author-email: fidesteam@ethyca.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `fideslang-1.4/src/fideslang.egg-info/SOURCES.txt` & `fideslang-1.4.1/src/fideslang.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fideslang-1.4/versioneer.py` & `fideslang-1.4.1/versioneer.py`

 * *Files identical despite different names*

