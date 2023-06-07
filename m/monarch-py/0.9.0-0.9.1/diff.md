# Comparing `tmp/monarch_py-0.9.0.tar.gz` & `tmp/monarch_py-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monarch_py-0.9.0.tar", max compression
+gzip compressed data, was "monarch_py-0.9.1.tar", max compression
```

## Comparing `monarch_py-0.9.0.tar` & `monarch_py-0.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      974 2023-06-02 02:55:36.296851 monarch_py-0.9.0/pyproject.toml
--rw-r--r--   0        0        0       77 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/__init__.py
--rw-r--r--   0        0        0     1150 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/association_type_mappings.yaml
--rw-r--r--   0        0        0     7319 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/cli.py
--rw-r--r--   0        0        0        0 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/datamodels/__init__.py
--rw-r--r--   0        0        0    11391 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/datamodels/model.py
--rw-r--r--   0        0        0     7485 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/datamodels/model.yaml
--rw-r--r--   0        0        0     3321 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/datamodels/solr.py
--rw-r--r--   0        0        0        0 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/implementations/__init__.py
--rw-r--r--   0        0        0        0 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/implementations/solr/__init__.py
--rw-r--r--   0        0        0    20304 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/implementations/solr/solr_implementation.py
--rw-r--r--   0        0        0        0 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/implementations/sql/__init__.py
--rw-r--r--   0        0        0     8909 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/implementations/sql/sql_implementation.py
--rw-r--r--   0        0        0        0 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/interfaces/__init__.py
--rw-r--r--   0        0        0     2343 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/interfaces/association_interface.py
--rw-r--r--   0        0        0      985 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/interfaces/entity_interface.py
--rw-r--r--   0        0        0      890 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/interfaces/query_interface.py
--rw-r--r--   0        0        0     4630 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/interfaces/search_interface.py
--rw-r--r--   0        0        0        0 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/service/__init__.py
--rw-r--r--   0        0        0     2052 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/service/solr_service.py
--rw-r--r--   0        0        0     9017 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/solr_cli.py
--rw-r--r--   0        0        0     3330 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/sql_cli.py
--rw-r--r--   0        0        0        0 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/utils/__init__.py
--rw-r--r--   0        0        0     3147 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/utils/association_type_utils.py
--rw-r--r--   0        0        0     3985 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/utils/solr_cli_utils.py
--rw-r--r--   0        0        0     4937 2023-06-02 02:55:36.296851 monarch_py-0.9.0/src/monarch_py/utils/utils.py
--rw-r--r--   0        0        0      750 1970-01-01 00:00:00.000000 monarch_py-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0      974 2023-06-07 21:31:17.078236 monarch_py-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0       77 2023-06-07 21:31:17.078236 monarch_py-0.9.1/src/monarch_py/__init__.py
+-rw-r--r--   0        0        0     1150 2023-06-07 21:31:17.078236 monarch_py-0.9.1/src/monarch_py/association_type_mappings.yaml
+-rw-r--r--   0        0        0     7464 2023-06-07 21:31:17.078236 monarch_py-0.9.1/src/monarch_py/cli.py
+-rw-r--r--   0        0        0        0 2023-06-07 21:31:17.078236 monarch_py-0.9.1/src/monarch_py/datamodels/__init__.py
+-rw-r--r--   0        0        0    11302 2023-06-07 21:31:17.078236 monarch_py-0.9.1/src/monarch_py/datamodels/model.py
+-rw-r--r--   0        0        0     7486 2023-06-07 21:31:17.078236 monarch_py-0.9.1/src/monarch_py/datamodels/model.yaml
+-rw-r--r--   0        0        0     3321 2023-06-07 21:31:17.078236 monarch_py-0.9.1/src/monarch_py/datamodels/solr.py
+-rw-r--r--   0        0        0        0 2023-06-07 21:31:17.078236 monarch_py-0.9.1/src/monarch_py/implementations/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-07 21:31:17.078236 monarch_py-0.9.1/src/monarch_py/implementations/solr/__init__.py
+-rw-r--r--   0        0        0    20304 2023-06-07 21:31:17.078236 monarch_py-0.9.1/src/monarch_py/implementations/solr/solr_implementation.py
+-rw-r--r--   0        0        0        0 2023-06-07 21:31:17.078236 monarch_py-0.9.1/src/monarch_py/implementations/sql/__init__.py
+-rw-r--r--   0        0        0     8909 2023-06-07 21:31:17.082236 monarch_py-0.9.1/src/monarch_py/implementations/sql/sql_implementation.py
+-rw-r--r--   0        0        0        0 2023-06-07 21:31:17.082236 monarch_py-0.9.1/src/monarch_py/interfaces/__init__.py
+-rw-r--r--   0        0        0     2343 2023-06-07 21:31:17.082236 monarch_py-0.9.1/src/monarch_py/interfaces/association_interface.py
+-rw-r--r--   0        0        0      985 2023-06-07 21:31:17.082236 monarch_py-0.9.1/src/monarch_py/interfaces/entity_interface.py
+-rw-r--r--   0        0        0      890 2023-06-07 21:31:17.082236 monarch_py-0.9.1/src/monarch_py/interfaces/query_interface.py
+-rw-r--r--   0        0        0     4630 2023-06-07 21:31:17.082236 monarch_py-0.9.1/src/monarch_py/interfaces/search_interface.py
+-rw-r--r--   0        0        0        0 2023-06-07 21:31:17.082236 monarch_py-0.9.1/src/monarch_py/service/__init__.py
+-rw-r--r--   0        0        0     2052 2023-06-07 21:31:17.082236 monarch_py-0.9.1/src/monarch_py/service/solr_service.py
+-rw-r--r--   0        0        0     9254 2023-06-07 21:31:17.082236 monarch_py-0.9.1/src/monarch_py/solr_cli.py
+-rw-r--r--   0        0        0     3330 2023-06-07 21:31:17.082236 monarch_py-0.9.1/src/monarch_py/sql_cli.py
+-rw-r--r--   0        0        0        0 2023-06-07 21:31:17.082236 monarch_py-0.9.1/src/monarch_py/utils/__init__.py
+-rw-r--r--   0        0        0     3145 2023-06-07 21:31:17.082236 monarch_py-0.9.1/src/monarch_py/utils/association_type_utils.py
+-rw-r--r--   0        0        0     3985 2023-06-07 21:31:17.082236 monarch_py-0.9.1/src/monarch_py/utils/solr_cli_utils.py
+-rw-r--r--   0        0        0     4937 2023-06-07 21:31:17.082236 monarch_py-0.9.1/src/monarch_py/utils/utils.py
+-rw-r--r--   0        0        0      750 1970-01-01 00:00:00.000000 monarch_py-0.9.1/PKG-INFO
```

### Comparing `monarch_py-0.9.0/pyproject.toml` & `monarch_py-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "monarch-py"
-version = "0.9.0"
+version = "0.9.1"
 description = "Monarch Initiative data access library"
 authors = [
     "Kevin Schaper <kevin@tislab.org>",
     "Glass Elsarboukh <glass@tislab.org>",
     "The Monarch Initiative <info@monarchinitiative.org>"
 ]
 packages = [
```

### Comparing `monarch_py-0.9.0/src/monarch_py/association_type_mappings.yaml` & `monarch_py-0.9.1/src/monarch_py/association_type_mappings.yaml`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.0/src/monarch_py/cli.py` & `monarch_py-0.9.1/src/monarch_py/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,16 @@
 
 
 @app.command("search")
 def search(
     q: str = typer.Option(None, "--query", "-q"),
     category: List[str] = typer.Option(None, "--category", "-c"),
     in_taxon: str = typer.Option(None, "--in-taxon", "-t"),
+    facet_fields: List[str] = typer.Option(None, "--facet-fields", "-ff"),
+    facet_queries: List[str] = typer.Option(None, "--facet-queries"),
     limit: int = typer.Option(20, "--limit", "-l"),
     offset: int = typer.Option(0, "--offset"),
     fmt: str = typer.Option(
         "json",
         "--format",
         "-f",
         help="The format of the output (json, yaml, tsv, table)",
```

### Comparing `monarch_py-0.9.0/src/monarch_py/datamodels/model.py` & `monarch_py-0.9.1/src/monarch_py/datamodels/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     original_object: Optional[str] = Field(None)
     object_namespace: Optional[str] = Field(None)
     object_category: Optional[List[str]] = Field(default_factory=list)
     object_closure: Optional[List[str]] = Field(default_factory=list)
     object_label: Optional[str] = Field(None)
     object_closure_label: Optional[List[str]] = Field(default_factory=list)
     primary_knowledge_source: Optional[List[str]] = Field(default_factory=list)
-    category: Optional[List[str]] = Field(default_factory=list)
+    category: Optional[str] = Field(None)
     negated: Optional[bool] = Field(None)
     provided_by: Optional[str] = Field(None)
     publications: Optional[List[str]] = Field(default_factory=list)
     qualifiers: Optional[List[str]] = Field(default_factory=list)
     frequency_qualifier: Optional[str] = Field(None)
     has_evidence: Optional[str] = Field(None)
     onset_qualifier: Optional[str] = Field(None)
@@ -102,15 +102,15 @@
     original_object: Optional[str] = Field(None)
     object_namespace: Optional[str] = Field(None)
     object_category: Optional[List[str]] = Field(default_factory=list)
     object_closure: Optional[List[str]] = Field(default_factory=list)
     object_label: Optional[str] = Field(None)
     object_closure_label: Optional[List[str]] = Field(default_factory=list)
     primary_knowledge_source: Optional[List[str]] = Field(default_factory=list)
-    category: Optional[List[str]] = Field(default_factory=list)
+    category: Optional[str] = Field(None)
     negated: Optional[bool] = Field(None)
     provided_by: Optional[str] = Field(None)
     publications: Optional[List[str]] = Field(default_factory=list)
     qualifiers: Optional[List[str]] = Field(default_factory=list)
     frequency_qualifier: Optional[str] = Field(None)
     has_evidence: Optional[str] = Field(None)
     onset_qualifier: Optional[str] = Field(None)
@@ -120,15 +120,15 @@
     pathway: Optional[str] = Field(None)
     relation: Optional[str] = Field(None)
 
 
 class Entity(ConfiguredBaseModel):
 
     id: str = Field(...)
-    category: Optional[List[str]] = Field(default_factory=list)
+    category: Optional[str] = Field(None)
     name: Optional[str] = Field(None)
     description: Optional[str] = Field(None)
     xref: Optional[List[str]] = Field(default_factory=list)
     provided_by: Optional[str] = Field(None)
     in_taxon: Optional[str] = Field(None)
     source: Optional[str] = Field(None)
     symbol: Optional[str] = Field(None)
@@ -187,15 +187,15 @@
 class SearchResult(Entity):
 
     highlight: Optional[str] = Field(
         None, description="""matching text snippet containing html tags"""
     )
     score: Optional[float] = Field(None)
     id: str = Field(...)
-    category: List[str] = Field(default_factory=list)
+    category: str = Field(...)
     name: str = Field(...)
     description: Optional[str] = Field(None)
     xref: Optional[List[str]] = Field(default_factory=list)
     provided_by: Optional[str] = Field(None)
     in_taxon: Optional[str] = Field(None)
     source: Optional[str] = Field(None)
     symbol: Optional[str] = Field(None)
```

### Comparing `monarch_py-0.9.0/src/monarch_py/datamodels/model.yaml` & `monarch_py-0.9.1/src/monarch_py/datamodels/model.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,15 @@
       items:
         range: AssociationCount
 
 slots:
   aggregator_knowledge_source:
     multivalued: true
   category:
-    multivalued: true
+    multivalued: false
   count:
     description: count of documents
     range: integer
   description:
     range: string
   direction:
     description: >-
```

### Comparing `monarch_py-0.9.0/src/monarch_py/datamodels/solr.py` & `monarch_py-0.9.1/src/monarch_py/datamodels/solr.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.0/src/monarch_py/implementations/solr/solr_implementation.py` & `monarch_py-0.9.1/src/monarch_py/implementations/solr/solr_implementation.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.0/src/monarch_py/implementations/sql/sql_implementation.py` & `monarch_py-0.9.1/src/monarch_py/implementations/sql/sql_implementation.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.0/src/monarch_py/interfaces/association_interface.py` & `monarch_py-0.9.1/src/monarch_py/interfaces/association_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.0/src/monarch_py/interfaces/entity_interface.py` & `monarch_py-0.9.1/src/monarch_py/interfaces/entity_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.0/src/monarch_py/interfaces/query_interface.py` & `monarch_py-0.9.1/src/monarch_py/interfaces/query_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.0/src/monarch_py/interfaces/search_interface.py` & `monarch_py-0.9.1/src/monarch_py/interfaces/search_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.0/src/monarch_py/service/solr_service.py` & `monarch_py-0.9.1/src/monarch_py/service/solr_service.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.0/src/monarch_py/solr_cli.py` & `monarch_py-0.9.1/src/monarch_py/solr_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,14 +135,16 @@
 
 
 @solr_app.command("search")
 def search(
     q: str = typer.Option(None, "--query", "-q"),
     category: List[str] = typer.Option(None, "--category", "-c"),
     in_taxon: str = typer.Option(None, "--in-taxon", "-t"),
+    facet_fields: List[str] = typer.Option(None, "--facet-fields", "-ff"),
+    facet_queries: List[str] = typer.Option(None, "--facet-queries"),
     limit: int = typer.Option(20, "--limit", "-l"),
     offset: int = typer.Option(0, "--offset"),
     fmt: str = typer.Option(
         "json",
         "--format",
         "-f",
         help="The format of the output (json, yaml, tsv, table)",
@@ -155,14 +157,16 @@
     """
     Search for entities
 
     Optional Args:
         q: The query string to search for
         category: The category of the entity
         taxon: The taxon of the entity
+        facet_fields: The fields to facet on
+        facet_queries: The queries to facet on
         limit: The number of entities to return
         offset: The offset of the first entity to be retrieved
         fmt (str): The format of the output (json, yaml, tsv, table). Default JSON
         output (str): The path to the output file. Default stdout
     """
     params = locals()
     params.pop("fmt", None)
```

### Comparing `monarch_py-0.9.0/src/monarch_py/sql_cli.py` & `monarch_py-0.9.1/src/monarch_py/sql_cli.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.0/src/monarch_py/utils/association_type_utils.py` & `monarch_py-0.9.1/src/monarch_py/utils/association_type_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,22 +17,20 @@
                 "AssociationTypeMappings is a singleton class, use getInstance() to get the instance."
             )
         else:
             AssociationTypeMappings.__instance = self
             self.mappings = None
             self.load_mappings()
 
-
     @staticmethod
     def get_mappings():
         if AssociationTypeMappings.__instance is None:
             AssociationTypeMappings()
         return AssociationTypeMappings.__instance.mappings
 
-
     def get_mapping(self, category: str):
         if AssociationTypeMappings.__instance is None:
             AssociationTypeMappings()
         for mapping in self.mappings:
             if mapping.category == category:
                 return mapping
```

### Comparing `monarch_py-0.9.0/src/monarch_py/utils/solr_cli_utils.py` & `monarch_py-0.9.1/src/monarch_py/utils/solr_cli_utils.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.0/src/monarch_py/utils/utils.py` & `monarch_py-0.9.1/src/monarch_py/utils/utils.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.9.0/PKG-INFO` & `monarch_py-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monarch-py
-Version: 0.9.0
+Version: 0.9.1
 Summary: Monarch Initiative data access library
 Author: Kevin Schaper
 Author-email: kevin@tislab.org
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

