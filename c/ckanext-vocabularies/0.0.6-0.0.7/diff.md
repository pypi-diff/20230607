# Comparing `tmp/ckanext-vocabularies-0.0.6.tar.gz` & `tmp/ckanext-vocabularies-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-vocabularies-0.0.6.tar", last modified: Thu Mar 30 14:19:20 2023, max compression
+gzip compressed data, was "ckanext-vocabularies-0.0.7.tar", last modified: Wed Jun  7 10:01:16 2023, max compression
```

## Comparing `ckanext-vocabularies-0.0.6.tar` & `ckanext-vocabularies-0.0.7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-30 14:19:20.860007 ckanext-vocabularies-0.0.6/
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)    34500 2023-03-29 11:02:44.000000 ckanext-vocabularies-0.0.6/LICENSE
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      209 2023-03-29 11:02:44.000000 ckanext-vocabularies-0.0.6/MANIFEST.in
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     4391 2023-03-30 14:19:20.860007 ckanext-vocabularies-0.0.6/PKG-INFO
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     3730 2023-03-29 11:02:44.000000 ckanext-vocabularies-0.0.6/README.md
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-30 14:19:20.860007 ckanext-vocabularies-0.0.6/ckanext/
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      219 2023-03-29 11:02:44.000000 ckanext-vocabularies-0.0.6/ckanext/__init__.py
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-30 14:19:20.860007 ckanext-vocabularies-0.0.6/ckanext/vocabularies/
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-29 11:02:44.000000 ckanext-vocabularies-0.0.6/ckanext/vocabularies/__init__.py
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-30 14:19:20.860007 ckanext-vocabularies-0.0.6/ckanext/vocabularies/assets/
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      335 2023-03-29 11:02:44.000000 ckanext-vocabularies-0.0.6/ckanext/vocabularies/assets/webassets.yml
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      734 2023-03-29 11:02:44.000000 ckanext-vocabularies-0.0.6/ckanext/vocabularies/blueprints.py
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-30 14:19:20.860007 ckanext-vocabularies-0.0.6/ckanext/vocabularies/dsc/
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-29 11:02:44.000000 ckanext-vocabularies-0.0.6/ckanext/vocabularies/dsc/__init__.py
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     3087 2023-03-29 11:02:44.000000 ckanext-vocabularies-0.0.6/ckanext/vocabularies/dsc/idsapi.py
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     4650 2023-03-29 11:02:44.000000 ckanext-vocabularies-0.0.6/ckanext/vocabularies/dsc/resourceapi.py
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     7006 2023-03-30 11:56:00.000000 ckanext-vocabularies-0.0.6/ckanext/vocabularies/dsc/subscribe.py
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     1535 2023-03-29 11:02:44.000000 ckanext-vocabularies-0.0.6/ckanext/vocabularies/dsc/subscriptionapi.py
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     5603 2023-03-29 11:02:44.000000 ckanext-vocabularies-0.0.6/ckanext/vocabularies/helpers.py
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      795 2023-03-29 11:02:44.000000 ckanext-vocabularies-0.0.6/ckanext/vocabularies/logic.py
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     2496 2023-03-29 11:02:44.000000 ckanext-vocabularies-0.0.6/ckanext/vocabularies/plugin.py
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-30 14:19:20.860007 ckanext-vocabularies-0.0.6/ckanext/vocabularies/templates/
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      827 2023-03-29 11:02:44.000000 ckanext-vocabularies-0.0.6/ckanext/vocabularies/templates/base.html
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-30 14:19:20.860007 ckanext-vocabularies-0.0.6/ckanext/vocabularies/templates/scheming/
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-30 14:19:20.860007 ckanext-vocabularies-0.0.6/ckanext/vocabularies/templates/scheming/form_snippets/
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     1392 2023-03-29 11:02:44.000000 ckanext-vocabularies-0.0.6/ckanext/vocabularies/templates/scheming/form_snippets/autocomplete_dropdown.html
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-30 14:19:20.860007 ckanext-vocabularies-0.0.6/ckanext/vocabularies/tests/
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-29 11:02:44.000000 ckanext-vocabularies-0.0.6/ckanext/vocabularies/tests/__init__.py
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     1262 2023-03-29 11:02:44.000000 ckanext-vocabularies-0.0.6/ckanext/vocabularies/tests/test_plugin.py
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-30 14:19:20.860007 ckanext-vocabularies-0.0.6/ckanext_vocabularies.egg-info/
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     4391 2023-03-30 14:19:20.000000 ckanext-vocabularies-0.0.6/ckanext_vocabularies.egg-info/PKG-INFO
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      961 2023-03-30 14:19:20.000000 ckanext-vocabularies-0.0.6/ckanext_vocabularies.egg-info/SOURCES.txt
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)        1 2023-03-30 14:19:20.000000 ckanext-vocabularies-0.0.6/ckanext_vocabularies.egg-info/dependency_links.txt
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      134 2023-03-30 14:19:20.000000 ckanext-vocabularies-0.0.6/ckanext_vocabularies.egg-info/entry_points.txt
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)        8 2023-03-30 14:19:20.000000 ckanext-vocabularies-0.0.6/ckanext_vocabularies.egg-info/namespace_packages.txt
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)        8 2023-03-30 14:19:20.000000 ckanext-vocabularies-0.0.6/ckanext_vocabularies.egg-info/top_level.txt
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)       77 2023-03-29 11:24:53.000000 ckanext-vocabularies-0.0.6/requirements.txt
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      613 2023-03-30 14:19:20.864007 ckanext-vocabularies-0.0.6/setup.cfg
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     3882 2023-03-30 14:18:36.000000 ckanext-vocabularies-0.0.6/setup.py
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-06-07 10:01:16.846673 ckanext-vocabularies-0.0.7/
+-rw-r--r--   0 karampatakiss  (1001) karampatakiss  (1001)    34500 2022-03-18 16:18:05.000000 ckanext-vocabularies-0.0.7/LICENSE
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      209 2022-03-18 16:18:05.000000 ckanext-vocabularies-0.0.7/MANIFEST.in
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     4411 2023-06-07 10:01:16.846673 ckanext-vocabularies-0.0.7/PKG-INFO
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     3730 2023-06-07 09:54:08.000000 ckanext-vocabularies-0.0.7/README.md
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-06-07 10:01:16.846673 ckanext-vocabularies-0.0.7/ckanext/
+-rw-r--r--   0 karampatakiss  (1001) karampatakiss  (1001)      219 2022-03-18 16:18:05.000000 ckanext-vocabularies-0.0.7/ckanext/__init__.py
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-06-07 10:01:16.846673 ckanext-vocabularies-0.0.7/ckanext/vocabularies/
+-rw-r--r--   0 karampatakiss  (1001) karampatakiss  (1001)        0 2022-03-18 16:18:05.000000 ckanext-vocabularies-0.0.7/ckanext/vocabularies/__init__.py
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-06-07 10:01:16.846673 ckanext-vocabularies-0.0.7/ckanext/vocabularies/assets/
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      335 2022-03-18 16:18:05.000000 ckanext-vocabularies-0.0.7/ckanext/vocabularies/assets/webassets.yml
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      734 2022-05-04 12:37:14.000000 ckanext-vocabularies-0.0.7/ckanext/vocabularies/blueprints.py
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-06-07 10:01:16.846673 ckanext-vocabularies-0.0.7/ckanext/vocabularies/dsc/
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)        0 2022-05-03 12:07:07.000000 ckanext-vocabularies-0.0.7/ckanext/vocabularies/dsc/__init__.py
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     3087 2022-05-05 15:35:58.000000 ckanext-vocabularies-0.0.7/ckanext/vocabularies/dsc/idsapi.py
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     4650 2022-12-15 08:00:30.000000 ckanext-vocabularies-0.0.7/ckanext/vocabularies/dsc/resourceapi.py
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     7006 2023-06-07 09:54:08.000000 ckanext-vocabularies-0.0.7/ckanext/vocabularies/dsc/subscribe.py
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     1535 2022-04-22 07:36:30.000000 ckanext-vocabularies-0.0.7/ckanext/vocabularies/dsc/subscriptionapi.py
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     6285 2023-06-07 09:55:42.000000 ckanext-vocabularies-0.0.7/ckanext/vocabularies/helpers.py
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      795 2022-05-04 12:35:14.000000 ckanext-vocabularies-0.0.7/ckanext/vocabularies/logic.py
+-rw-r--r--   0 karampatakiss  (1001) karampatakiss  (1001)     2496 2022-05-05 05:51:21.000000 ckanext-vocabularies-0.0.7/ckanext/vocabularies/plugin.py
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-06-07 10:01:16.846673 ckanext-vocabularies-0.0.7/ckanext/vocabularies/templates/
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      827 2022-03-22 13:04:43.000000 ckanext-vocabularies-0.0.7/ckanext/vocabularies/templates/base.html
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-06-07 10:01:16.842673 ckanext-vocabularies-0.0.7/ckanext/vocabularies/templates/scheming/
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-06-07 10:01:16.846673 ckanext-vocabularies-0.0.7/ckanext/vocabularies/templates/scheming/form_snippets/
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     1392 2022-03-22 13:20:59.000000 ckanext-vocabularies-0.0.7/ckanext/vocabularies/templates/scheming/form_snippets/autocomplete_dropdown.html
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-06-07 10:01:16.846673 ckanext-vocabularies-0.0.7/ckanext/vocabularies/tests/
+-rw-r--r--   0 karampatakiss  (1001) karampatakiss  (1001)        0 2022-03-18 16:18:05.000000 ckanext-vocabularies-0.0.7/ckanext/vocabularies/tests/__init__.py
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     1262 2022-03-18 16:18:05.000000 ckanext-vocabularies-0.0.7/ckanext/vocabularies/tests/test_plugin.py
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-06-07 10:01:16.846673 ckanext-vocabularies-0.0.7/ckanext_vocabularies.egg-info/
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     4411 2023-06-07 10:01:16.000000 ckanext-vocabularies-0.0.7/ckanext_vocabularies.egg-info/PKG-INFO
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      961 2023-06-07 10:01:16.000000 ckanext-vocabularies-0.0.7/ckanext_vocabularies.egg-info/SOURCES.txt
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)        1 2023-06-07 10:01:16.000000 ckanext-vocabularies-0.0.7/ckanext_vocabularies.egg-info/dependency_links.txt
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      169 2023-06-07 10:01:16.000000 ckanext-vocabularies-0.0.7/ckanext_vocabularies.egg-info/entry_points.txt
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)        8 2023-06-07 10:01:16.000000 ckanext-vocabularies-0.0.7/ckanext_vocabularies.egg-info/namespace_packages.txt
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)        8 2023-06-07 10:01:16.000000 ckanext-vocabularies-0.0.7/ckanext_vocabularies.egg-info/top_level.txt
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)       77 2023-06-07 09:54:08.000000 ckanext-vocabularies-0.0.7/requirements.txt
+-rw-r--r--   0 karampatakiss  (1001) karampatakiss  (1001)      613 2023-06-07 10:01:16.846673 ckanext-vocabularies-0.0.7/setup.cfg
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     3882 2023-06-07 09:54:08.000000 ckanext-vocabularies-0.0.7/setup.py
```

### Comparing `ckanext-vocabularies-0.0.6/LICENSE` & `ckanext-vocabularies-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-vocabularies-0.0.6/PKG-INFO` & `ckanext-vocabularies-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: ckanext-vocabularies
-Version: 0.0.6
+Version: 0.0.7
 Summary: Getting choices options for the scheming choise type of field, based on SKOS vocabulary served on a remote SPARQL endpoint
 Home-page: https://github.com/s.karampatakis@gmail.com/ckanext-vocabularies
 Author: Sotirios Karampatakis
 Author-email: sotiris.karampatakis@semantic-web.com
 License: AGPL
 Keywords: CKAN vocabularies SKOS scheming
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 2.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Tests](https://github.com/s.karampatakis@gmail.com/ckanext-vocabularies/workflows/Tests/badge.svg?branch=main)](https://github.com/s.karampatakis@gmail.com/ckanext-vocabularies/actions)
@@ -140,7 +141,9 @@
 ## Funding
 This code was created as part of project TRUSTS: Trusted secure data sharing space.
 
 This project has received funding from the European Union's Horizon 2020 research and innovation programme under grant agreement [No 871481](https://cordis.europa.eu/project/id/871481).
 
 
 
+
+
```

### Comparing `ckanext-vocabularies-0.0.6/README.md` & `ckanext-vocabularies-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-vocabularies-0.0.6/ckanext/vocabularies/blueprints.py` & `ckanext-vocabularies-0.0.7/ckanext/vocabularies/blueprints.py`

 * *Files identical despite different names*

### Comparing `ckanext-vocabularies-0.0.6/ckanext/vocabularies/dsc/idsapi.py` & `ckanext-vocabularies-0.0.7/ckanext/vocabularies/dsc/idsapi.py`

 * *Files identical despite different names*

### Comparing `ckanext-vocabularies-0.0.6/ckanext/vocabularies/dsc/resourceapi.py` & `ckanext-vocabularies-0.0.7/ckanext/vocabularies/dsc/resourceapi.py`

 * *Files identical despite different names*

### Comparing `ckanext-vocabularies-0.0.6/ckanext/vocabularies/dsc/subscribe.py` & `ckanext-vocabularies-0.0.7/ckanext/vocabularies/dsc/subscribe.py`

 * *Files identical despite different names*

### Comparing `ckanext-vocabularies-0.0.6/ckanext/vocabularies/dsc/subscriptionapi.py` & `ckanext-vocabularies-0.0.7/ckanext/vocabularies/dsc/subscriptionapi.py`

 * *Files identical despite different names*

### Comparing `ckanext-vocabularies-0.0.6/ckanext/vocabularies/helpers.py` & `ckanext-vocabularies-0.0.7/ckanext/vocabularies/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from SPARQLWrapper import SPARQLWrapper, JSON
 import requests
 import json
 import logging
+import uuid
 
 import ckan.plugins.toolkit as toolkit
 from rdflib import plugin, URIRef
 from rdflib.graph import Graph
 #from rdflib.store import Store
 #from rdflib_sqlalchemy import registerplugins
 
@@ -92,14 +93,27 @@
         data = subscription.consume_resource()
 
         graph.parse(data=data, format="text/turtle")
         graphs[dsc_resource] = graph
     results = json.loads(graph.query(query).serialize(format='json'))
     return results
 
+def query_local_resource(local_resource, query):
+    graph_id = uuid.uuid4(local_resource)
+    if graph_id in graphs:
+        graph = graphs[graph_id]
+        log.debug('Graph exists in triplestore...querying')
+    else:
+        log.warn('Graph does not exist on triplestore...adding triples')
+        graph = Graph()
+        graph.parse(local_resource, format="text/turtle")
+        graphs[graph_id] = graph
+    results = json.loads(graph.query(query).serialize(format='json'))
+    return results
+
 # deprecated
 # def query_dsc_resource_rdbms(dsc_resource, query):
 #     graph = Graph(store, identifier=dsc_resource)
 #     try:
 #         graph.open(URIRef(toolkit.config.get('ckanext.vocabularies.triplestore')), create=False)
 #         log.info('Graph exists in triplestore...querying')
 #     except RuntimeError as error:
@@ -122,23 +136,26 @@
 
 def skos_choices_sparql_helper(field):
     '''Return a list of the concepts of a concept scheme served from a SPARQL endpoint'''
 
     sparql_endpoint = field.get('skos_choices_sparql_endpoint', None)
     is_poolparty = field.get('skos_choices_is_poolparty', False)
     concept_scheme = field.get('skos_choices_concept_scheme', None)
+    local_resource = field.get('skos_choices_local_resource', None)
     dsc_resource = field.get('skos_choices_dsc_resource', None)
     dsc_resource_contract = field.get('skos_choices_dsc_resource_contract_offer', None)
 
     query = query_with_in_scheme(concept_scheme)
     if dsc_resource is not None:
         log.info('querying dsc')
         results = query_dsc_resource(dsc_resource, dsc_resource_contract, query)
+    elif local_resource is not None:
+        results = query_local_resource(local_resource, query)
     elif is_poolparty:
-        results = query_poolparty(sparql_endpoint, query)
+        results = query_poolparty(sparql_endpoint, query)    
     else:
         results = query_public_endpoint(sparql_endpoint, query)
 
     log.info('received results')
     return format_results(results)
```

### Comparing `ckanext-vocabularies-0.0.6/ckanext/vocabularies/logic.py` & `ckanext-vocabularies-0.0.7/ckanext/vocabularies/logic.py`

 * *Files identical despite different names*

### Comparing `ckanext-vocabularies-0.0.6/ckanext/vocabularies/plugin.py` & `ckanext-vocabularies-0.0.7/ckanext/vocabularies/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-vocabularies-0.0.6/ckanext/vocabularies/templates/base.html` & `ckanext-vocabularies-0.0.7/ckanext/vocabularies/templates/base.html`

 * *Files identical despite different names*

### Comparing `ckanext-vocabularies-0.0.6/ckanext/vocabularies/templates/scheming/form_snippets/autocomplete_dropdown.html` & `ckanext-vocabularies-0.0.7/ckanext/vocabularies/templates/scheming/form_snippets/autocomplete_dropdown.html`

 * *Files identical despite different names*

### Comparing `ckanext-vocabularies-0.0.6/ckanext/vocabularies/tests/test_plugin.py` & `ckanext-vocabularies-0.0.7/ckanext/vocabularies/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-vocabularies-0.0.6/ckanext_vocabularies.egg-info/PKG-INFO` & `ckanext-vocabularies-0.0.7/ckanext_vocabularies.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: ckanext-vocabularies
-Version: 0.0.6
+Version: 0.0.7
 Summary: Getting choices options for the scheming choise type of field, based on SKOS vocabulary served on a remote SPARQL endpoint
 Home-page: https://github.com/s.karampatakis@gmail.com/ckanext-vocabularies
 Author: Sotirios Karampatakis
 Author-email: sotiris.karampatakis@semantic-web.com
 License: AGPL
 Keywords: CKAN vocabularies SKOS scheming
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 2.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Tests](https://github.com/s.karampatakis@gmail.com/ckanext-vocabularies/workflows/Tests/badge.svg?branch=main)](https://github.com/s.karampatakis@gmail.com/ckanext-vocabularies/actions)
@@ -140,7 +141,9 @@
 ## Funding
 This code was created as part of project TRUSTS: Trusted secure data sharing space.
 
 This project has received funding from the European Union's Horizon 2020 research and innovation programme under grant agreement [No 871481](https://cordis.europa.eu/project/id/871481).
 
 
 
+
+
```

### Comparing `ckanext-vocabularies-0.0.6/ckanext_vocabularies.egg-info/SOURCES.txt` & `ckanext-vocabularies-0.0.7/ckanext_vocabularies.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-vocabularies-0.0.6/setup.cfg` & `ckanext-vocabularies-0.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `ckanext-vocabularies-0.0.6/setup.py` & `ckanext-vocabularies-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 setup(
     name='''ckanext-vocabularies''',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # http://packaging.python.org/en/latest/tutorial.html#version
-    version='0.0.6',
+    version='0.0.7',
 
     description='''Getting choices options for the scheming choise type of field, based on SKOS vocabulary served on a remote SPARQL endpoint''',
     long_description=long_description,
     long_description_content_type="text/markdown",
 
     # The project's main homepage.
     url='https://github.com/s.karampatakis@gmail.com/ckanext-vocabularies',
```

