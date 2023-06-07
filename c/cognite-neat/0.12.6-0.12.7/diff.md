# Comparing `tmp/cognite_neat-0.12.6.tar.gz` & `tmp/cognite_neat-0.12.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_neat-0.12.6.tar", max compression
+gzip compressed data, was "cognite_neat-0.12.7.tar", max compression
```

## Comparing `cognite_neat-0.12.6.tar` & `cognite_neat-0.12.7.tar`

### file list

```diff
@@ -1,94 +1,94 @@
--rw-r--r--   0        0        0    11351 2023-06-06 15:05:06.171516 cognite_neat-0.12.6/LICENSE
--rw-r--r--   0        0        0     8765 2023-06-06 15:05:06.171516 cognite_neat-0.12.6/README.md
--rw-r--r--   0        0        0       23 2023-06-06 15:05:06.175516 cognite_neat-0.12.6/cognite/neat/__init__.py
--rw-r--r--   0        0        0      761 2023-06-06 15:05:06.175516 cognite_neat-0.12.6/cognite/neat/constants.py
--rw-r--r--   0        0        0        0 2023-06-06 15:05:06.175516 cognite_neat-0.12.6/cognite/neat/core/__init__.py
--rw-r--r--   0        0        0     2652 2023-06-06 15:05:06.175516 cognite_neat-0.12.6/cognite/neat/core/app.py
--rw-r--r--   0        0        0     1344 2023-06-06 15:05:06.175516 cognite_neat-0.12.6/cognite/neat/core/configuration.py
--rw-r--r--   0        0        0      408 2023-06-06 15:05:06.175516 cognite_neat-0.12.6/cognite/neat/core/data_classes/__init__.py
--rw-r--r--   0        0        0     4775 2023-06-06 15:05:06.175516 cognite_neat-0.12.6/cognite/neat/core/data_classes/config.py
--rw-r--r--   0        0        0     8132 2023-06-06 15:05:06.175516 cognite_neat-0.12.6/cognite/neat/core/data_classes/rules.py
--rw-r--r--   0        0        0    30296 2023-06-06 15:05:06.175516 cognite_neat-0.12.6/cognite/neat/core/data_classes/transformation_rules.py
--rw-r--r--   0        0        0        0 2023-06-06 15:05:06.175516 cognite_neat-0.12.6/cognite/neat/core/data_stores/__init__.py
--rw-r--r--   0        0        0     1520 2023-06-06 15:05:06.175516 cognite_neat-0.12.6/cognite/neat/core/data_stores/metrics.py
--rw-r--r--   0        0        0     9436 2023-06-06 15:05:06.175516 cognite_neat-0.12.6/cognite/neat/core/data_stores/oxrdflib.py
--rw-r--r--   0        0        0      646 2023-06-06 15:05:06.175516 cognite_neat-0.12.6/cognite/neat/core/extractors/__init__.py
--rw-r--r--   0        0        0     5449 2023-06-06 15:05:06.175516 cognite_neat-0.12.6/cognite/neat/core/extractors/graph_sheet_to_graph.py
--rw-r--r--   0        0        0     2250 2023-06-06 15:05:06.175516 cognite_neat-0.12.6/cognite/neat/core/extractors/labels.py
--rw-r--r--   0        0        0    35453 2023-06-06 15:05:06.175516 cognite_neat-0.12.6/cognite/neat/core/extractors/rdf_to_assets.py
--rw-r--r--   0        0        0    17870 2023-06-06 15:05:06.175516 cognite_neat-0.12.6/cognite/neat/core/extractors/rdf_to_relationships.py
--rw-r--r--   0        0        0     5400 2023-06-06 15:05:06.175516 cognite_neat-0.12.6/cognite/neat/core/extractors/rules_to_graph_capturing_sheet.py
--rw-r--r--   0        0        0     6700 2023-06-06 15:05:06.175516 cognite_neat-0.12.6/cognite/neat/core/extractors/rules_to_graphql.py
--rw-r--r--   0        0        0      138 2023-06-06 15:05:06.175516 cognite_neat-0.12.6/cognite/neat/core/loader/__init__.py
--rw-r--r--   0        0        0      711 2023-06-06 15:05:06.175516 cognite_neat-0.12.6/cognite/neat/core/loader/config.py
--rw-r--r--   0        0        0     1210 2023-06-06 15:05:06.175516 cognite_neat-0.12.6/cognite/neat/core/loader/graph.py
--rw-r--r--   0        0        0      938 2023-06-06 15:05:06.175516 cognite_neat-0.12.6/cognite/neat/core/loader/graph_capturing_sheet.py
--rw-r--r--   0        0        0    10647 2023-06-06 15:05:06.175516 cognite_neat-0.12.6/cognite/neat/core/loader/graph_store.py
--rw-r--r--   0        0        0      913 2023-06-06 15:05:06.175516 cognite_neat-0.12.6/cognite/neat/core/loader/rules.py
--rw-r--r--   0        0        0        0 2023-06-06 15:05:06.175516 cognite_neat-0.12.6/cognite/neat/core/mocks/__init__.py
--rw-r--r--   0        0        0    10373 2023-06-06 15:05:06.175516 cognite_neat-0.12.6/cognite/neat/core/mocks/graph.py
--rw-r--r--   0        0        0    15303 2023-06-06 15:05:06.175516 cognite_neat-0.12.6/cognite/neat/core/modeler.py
--rw-r--r--   0        0        0      110 2023-06-06 15:05:06.175516 cognite_neat-0.12.6/cognite/neat/core/parser/__init__.py
--rw-r--r--   0        0        0     1727 2023-06-06 15:05:06.175516 cognite_neat-0.12.6/cognite/neat/core/parser/transformation_rules.py
--rw-r--r--   0        0        0       73 2023-06-06 15:05:06.175516 cognite_neat-0.12.6/cognite/neat/core/query_generator/__init__.py
--rw-r--r--   0        0        0     9595 2023-06-06 15:05:06.175516 cognite_neat-0.12.6/cognite/neat/core/query_generator/sparql.py
--rw-r--r--   0        0        0    11914 2023-06-06 15:05:06.175516 cognite_neat-0.12.6/cognite/neat/core/transformer.py
--rw-r--r--   0        0        0     6092 2023-06-06 15:05:06.175516 cognite_neat-0.12.6/cognite/neat/core/utils.py
--rw-r--r--   0        0        0     2558 2023-06-06 15:05:06.175516 cognite_neat-0.12.6/cognite/neat/core/validator.py
--rw-r--r--   0        0        0      311 2023-06-06 15:05:06.175516 cognite_neat-0.12.6/cognite/neat/core/workflow/__init__.py
--rw-r--r--   0        0        0    18503 2023-06-06 15:05:06.175516 cognite_neat-0.12.6/cognite/neat/core/workflow/base.py
--rw-r--r--   0        0        0    17764 2023-06-06 15:05:06.175516 cognite_neat-0.12.6/cognite/neat/core/workflow/cdf_store.py
--rw-r--r--   0        0        0     6200 2023-06-06 15:05:06.175516 cognite_neat-0.12.6/cognite/neat/core/workflow/manager.py
--rw-r--r--   0        0        0     4103 2023-06-06 15:05:06.175516 cognite_neat-0.12.6/cognite/neat/core/workflow/model.py
--rw-r--r--   0        0        0      781 2023-06-06 15:05:06.175516 cognite_neat-0.12.6/cognite/neat/core/workflow/tasks.py
--rw-r--r--   0        0        0     6648 2023-06-06 15:05:06.175516 cognite_neat-0.12.6/cognite/neat/core/workflow/triggers.py
--rw-r--r--   0        0        0      453 2023-06-06 15:05:06.175516 cognite_neat-0.12.6/cognite/neat/core/workflow/utils.py
--rw-r--r--   0        0        0      286 2023-06-06 15:05:06.175516 cognite_neat-0.12.6/cognite/neat/examples/data-models/power-grid-v0_1_0.graphql
--rw-r--r--   0        0        0    94607 2023-06-06 15:05:06.175516 cognite_neat-0.12.6/cognite/neat/examples/graph-sheets/sheet2cdf-graph-capturing.xlsx
--rw-r--r--   0        0        0    79580 2023-06-06 15:05:06.175516 cognite_neat-0.12.6/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx
--rw-r--r--   0        0        0    77438 2023-06-06 15:05:06.175516 cognite_neat-0.12.6/cognite/neat/examples/rules/power-grid-example.xlsx
--rw-r--r--   0        0        0    75865 2023-06-06 15:05:06.175516 cognite_neat-0.12.6/cognite/neat/examples/rules/rules-template.xlsx
--rw-r--r--   0        0        0    52178 2023-06-06 15:05:06.179516 cognite_neat-0.12.6/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx
--rw-r--r--   0        0        0    79427 2023-06-06 15:05:06.179516 cognite_neat-0.12.6/cognite/neat/examples/rules/source-to-solution-mapping-rules.xlsx
--rw-r--r--   0        0        0  1437851 2023-06-06 15:05:06.183516 cognite_neat-0.12.6/cognite/neat/examples/source-graphs/Knowledge-Graph-Nordic44.xml
--rw-r--r--   0        0        0     1461 2023-06-06 15:05:06.183516 cognite_neat-0.12.6/cognite/neat/examples/workflows/basic/workflow.py
--rw-r--r--   0        0        0     1782 2023-06-06 15:05:06.183516 cognite_neat-0.12.6/cognite/neat/examples/workflows/basic/workflow.yaml
--rw-r--r--   0        0        0    15632 2023-06-06 15:05:06.183516 cognite_neat-0.12.6/cognite/neat/examples/workflows/default/workflow.py
--rw-r--r--   0        0        0     6774 2023-06-06 15:05:06.183516 cognite_neat-0.12.6/cognite/neat/examples/workflows/default/workflow.yaml
--rw-r--r--   0        0        0     3630 2023-06-06 15:05:06.183516 cognite_neat-0.12.6/cognite/neat/examples/workflows/fdm_schema_generation/workflow.py
--rw-r--r--   0        0        0     2573 2023-06-06 15:05:06.183516 cognite_neat-0.12.6/cognite/neat/examples/workflows/fdm_schema_generation/workflow.yaml
--rw-r--r--   0        0        0    11477 2023-06-06 15:05:06.183516 cognite_neat-0.12.6/cognite/neat/examples/workflows/graph_db_import/workflow.py
--rw-r--r--   0        0        0     4792 2023-06-06 15:05:06.183516 cognite_neat-0.12.6/cognite/neat/examples/workflows/graph_db_import/workflow.yaml
--rw-r--r--   0        0        0    16421 2023-06-06 15:05:06.183516 cognite_neat-0.12.6/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.py
--rw-r--r--   0        0        0     8083 2023-06-06 15:05:06.183516 cognite_neat-0.12.6/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.yaml
--rw-r--r--   0        0        0    13115 2023-06-06 15:05:06.183516 cognite_neat-0.12.6/cognite/neat/examples/workflows/sheet2cdf/workflow.py
--rw-r--r--   0        0        0     6025 2023-06-06 15:05:06.183516 cognite_neat-0.12.6/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml
--rw-r--r--   0        0        0    11867 2023-06-06 15:05:06.183516 cognite_neat-0.12.6/cognite/neat/examples/workflows/sme_graph_capture/workflow.py
--rw-r--r--   0        0        0     6837 2023-06-06 15:05:06.183516 cognite_neat-0.12.6/cognite/neat/examples/workflows/sme_graph_capture/workflow.yaml
--rw-r--r--   0        0        0        0 2023-06-06 15:05:06.223516 cognite_neat-0.12.6/cognite/neat/explorer/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 15:05:06.223516 cognite_neat-0.12.6/cognite/neat/explorer/data_classes/__init__.py
--rw-r--r--   0        0        0     1013 2023-06-06 15:05:06.223516 cognite_neat-0.12.6/cognite/neat/explorer/data_classes/rest.py
--rw-r--r--   0        0        0    21517 2023-06-06 15:05:06.223516 cognite_neat-0.12.6/cognite/neat/explorer/explorer.py
--rw-r--r--   0        0        0        0 2023-06-06 15:05:06.223516 cognite_neat-0.12.6/cognite/neat/explorer/utils/__init__.py
--rw-r--r--   0        0        0      412 2023-06-06 15:05:06.223516 cognite_neat-0.12.6/cognite/neat/explorer/utils/data_mapping.py
--rw-r--r--   0        0        0     4003 2023-06-06 15:05:06.223516 cognite_neat-0.12.6/cognite/neat/explorer/utils/query_templates.py
--rw-r--r--   0        0        0       16 2023-06-06 15:05:06.183516 cognite_neat-0.12.6/cognite/neat/explorer-ui/index.html
--rw-r--r--   0        0        0      312 2023-06-06 15:05:06.183516 cognite_neat-0.12.6/cognite/neat/explorer-ui/neat-app/.gitignore
--rw-r--r--   0        0        0     3359 2023-06-06 15:05:06.183516 cognite_neat-0.12.6/cognite/neat/explorer-ui/neat-app/README.md
--rw-r--r--   0        0        0      464 2023-06-06 15:05:06.183516 cognite_neat-0.12.6/cognite/neat/explorer-ui/neat-app/build/asset-manifest.json
--rw-r--r--   0        0        0     3870 2023-06-06 15:05:06.183516 cognite_neat-0.12.6/cognite/neat/explorer-ui/neat-app/build/favicon.ico
--rw-r--r--   0        0        0      630 2023-06-06 15:05:06.183516 cognite_neat-0.12.6/cognite/neat/explorer-ui/neat-app/build/index.html
--rw-r--r--   0        0        0     5347 2023-06-06 15:05:06.183516 cognite_neat-0.12.6/cognite/neat/explorer-ui/neat-app/build/logo192.png
--rw-r--r--   0        0        0      492 2023-06-06 15:05:06.183516 cognite_neat-0.12.6/cognite/neat/explorer-ui/neat-app/build/manifest.json
--rw-r--r--   0        0        0       67 2023-06-06 15:05:06.183516 cognite_neat-0.12.6/cognite/neat/explorer-ui/neat-app/build/robots.txt
--rw-r--r--   0        0        0     8524 2023-06-06 15:05:06.183516 cognite_neat-0.12.6/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css
--rw-r--r--   0        0        0    13319 2023-06-06 15:05:06.183516 cognite_neat-0.12.6/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css.map
--rw-r--r--   0        0        0  1359583 2023-06-06 15:05:06.191516 cognite_neat-0.12.6/cognite/neat/explorer-ui/neat-app/build/static/js/main.97e96de0.js
--rw-r--r--   0        0        0     2667 2023-06-06 15:05:06.191516 cognite_neat-0.12.6/cognite/neat/explorer-ui/neat-app/build/static/js/main.97e96de0.js.LICENSE.txt
--rw-r--r--   0        0        0  5853485 2023-06-06 15:05:06.219516 cognite_neat-0.12.6/cognite/neat/explorer-ui/neat-app/build/static/js/main.97e96de0.js.map
--rw-r--r--   0        0        0     2633 2023-06-06 15:05:06.219516 cognite_neat-0.12.6/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg
--rw-r--r--   0        0        0      358 2023-06-06 15:05:06.223516 cognite_neat-0.12.6/cognite/neat/main.py
--rw-r--r--   0        0        0        0 2023-06-06 15:05:06.227517 cognite_neat-0.12.6/cognite/neat/migration/__init__.py
--rw-r--r--   0        0        0     1581 2023-06-06 15:05:06.227517 cognite_neat-0.12.6/cognite/neat/migration/wf_manifests.py
--rw-r--r--   0        0        0     2471 2023-06-06 15:05:06.687521 cognite_neat-0.12.6/pyproject.toml
--rw-r--r--   0        0        0    10241 1970-01-01 00:00:00.000000 cognite_neat-0.12.6/PKG-INFO
+-rw-r--r--   0        0        0    11351 2023-06-07 15:11:33.541119 cognite_neat-0.12.7/LICENSE
+-rw-r--r--   0        0        0     8765 2023-06-07 15:11:33.541119 cognite_neat-0.12.7/README.md
+-rw-r--r--   0        0        0       23 2023-06-07 15:11:33.541119 cognite_neat-0.12.7/cognite/neat/__init__.py
+-rw-r--r--   0        0        0      761 2023-06-07 15:11:33.541119 cognite_neat-0.12.7/cognite/neat/constants.py
+-rw-r--r--   0        0        0        0 2023-06-07 15:11:33.541119 cognite_neat-0.12.7/cognite/neat/core/__init__.py
+-rw-r--r--   0        0        0     2652 2023-06-07 15:11:33.541119 cognite_neat-0.12.7/cognite/neat/core/app.py
+-rw-r--r--   0        0        0     1344 2023-06-07 15:11:33.541119 cognite_neat-0.12.7/cognite/neat/core/configuration.py
+-rw-r--r--   0        0        0      408 2023-06-07 15:11:33.541119 cognite_neat-0.12.7/cognite/neat/core/data_classes/__init__.py
+-rw-r--r--   0        0        0     4775 2023-06-07 15:11:33.541119 cognite_neat-0.12.7/cognite/neat/core/data_classes/config.py
+-rw-r--r--   0        0        0     8132 2023-06-07 15:11:33.541119 cognite_neat-0.12.7/cognite/neat/core/data_classes/rules.py
+-rw-r--r--   0        0        0    30296 2023-06-07 15:11:33.541119 cognite_neat-0.12.7/cognite/neat/core/data_classes/transformation_rules.py
+-rw-r--r--   0        0        0        0 2023-06-07 15:11:33.541119 cognite_neat-0.12.7/cognite/neat/core/data_stores/__init__.py
+-rw-r--r--   0        0        0     1520 2023-06-07 15:11:33.541119 cognite_neat-0.12.7/cognite/neat/core/data_stores/metrics.py
+-rw-r--r--   0        0        0     9436 2023-06-07 15:11:33.541119 cognite_neat-0.12.7/cognite/neat/core/data_stores/oxrdflib.py
+-rw-r--r--   0        0        0      646 2023-06-07 15:11:33.541119 cognite_neat-0.12.7/cognite/neat/core/extractors/__init__.py
+-rw-r--r--   0        0        0     5449 2023-06-07 15:11:33.541119 cognite_neat-0.12.7/cognite/neat/core/extractors/graph_sheet_to_graph.py
+-rw-r--r--   0        0        0     2250 2023-06-07 15:11:33.541119 cognite_neat-0.12.7/cognite/neat/core/extractors/labels.py
+-rw-r--r--   0        0        0    36972 2023-06-07 15:11:33.541119 cognite_neat-0.12.7/cognite/neat/core/extractors/rdf_to_assets.py
+-rw-r--r--   0        0        0    17870 2023-06-07 15:11:33.541119 cognite_neat-0.12.7/cognite/neat/core/extractors/rdf_to_relationships.py
+-rw-r--r--   0        0        0     5400 2023-06-07 15:11:33.541119 cognite_neat-0.12.7/cognite/neat/core/extractors/rules_to_graph_capturing_sheet.py
+-rw-r--r--   0        0        0     6700 2023-06-07 15:11:33.541119 cognite_neat-0.12.7/cognite/neat/core/extractors/rules_to_graphql.py
+-rw-r--r--   0        0        0      138 2023-06-07 15:11:33.541119 cognite_neat-0.12.7/cognite/neat/core/loader/__init__.py
+-rw-r--r--   0        0        0      711 2023-06-07 15:11:33.541119 cognite_neat-0.12.7/cognite/neat/core/loader/config.py
+-rw-r--r--   0        0        0     1210 2023-06-07 15:11:33.541119 cognite_neat-0.12.7/cognite/neat/core/loader/graph.py
+-rw-r--r--   0        0        0      938 2023-06-07 15:11:33.541119 cognite_neat-0.12.7/cognite/neat/core/loader/graph_capturing_sheet.py
+-rw-r--r--   0        0        0    10647 2023-06-07 15:11:33.541119 cognite_neat-0.12.7/cognite/neat/core/loader/graph_store.py
+-rw-r--r--   0        0        0      913 2023-06-07 15:11:33.545119 cognite_neat-0.12.7/cognite/neat/core/loader/rules.py
+-rw-r--r--   0        0        0        0 2023-06-07 15:11:33.545119 cognite_neat-0.12.7/cognite/neat/core/mocks/__init__.py
+-rw-r--r--   0        0        0    10373 2023-06-07 15:11:33.545119 cognite_neat-0.12.7/cognite/neat/core/mocks/graph.py
+-rw-r--r--   0        0        0    15303 2023-06-07 15:11:33.545119 cognite_neat-0.12.7/cognite/neat/core/modeler.py
+-rw-r--r--   0        0        0      110 2023-06-07 15:11:33.545119 cognite_neat-0.12.7/cognite/neat/core/parser/__init__.py
+-rw-r--r--   0        0        0     1727 2023-06-07 15:11:33.545119 cognite_neat-0.12.7/cognite/neat/core/parser/transformation_rules.py
+-rw-r--r--   0        0        0       73 2023-06-07 15:11:33.545119 cognite_neat-0.12.7/cognite/neat/core/query_generator/__init__.py
+-rw-r--r--   0        0        0     9595 2023-06-07 15:11:33.545119 cognite_neat-0.12.7/cognite/neat/core/query_generator/sparql.py
+-rw-r--r--   0        0        0    11914 2023-06-07 15:11:33.545119 cognite_neat-0.12.7/cognite/neat/core/transformer.py
+-rw-r--r--   0        0        0     6092 2023-06-07 15:11:33.545119 cognite_neat-0.12.7/cognite/neat/core/utils.py
+-rw-r--r--   0        0        0     2559 2023-06-07 15:11:33.545119 cognite_neat-0.12.7/cognite/neat/core/validator.py
+-rw-r--r--   0        0        0      311 2023-06-07 15:11:33.545119 cognite_neat-0.12.7/cognite/neat/core/workflow/__init__.py
+-rw-r--r--   0        0        0    18503 2023-06-07 15:11:33.545119 cognite_neat-0.12.7/cognite/neat/core/workflow/base.py
+-rw-r--r--   0        0        0    17764 2023-06-07 15:11:33.545119 cognite_neat-0.12.7/cognite/neat/core/workflow/cdf_store.py
+-rw-r--r--   0        0        0     6200 2023-06-07 15:11:33.545119 cognite_neat-0.12.7/cognite/neat/core/workflow/manager.py
+-rw-r--r--   0        0        0     4103 2023-06-07 15:11:33.545119 cognite_neat-0.12.7/cognite/neat/core/workflow/model.py
+-rw-r--r--   0        0        0      781 2023-06-07 15:11:33.545119 cognite_neat-0.12.7/cognite/neat/core/workflow/tasks.py
+-rw-r--r--   0        0        0     6648 2023-06-07 15:11:33.545119 cognite_neat-0.12.7/cognite/neat/core/workflow/triggers.py
+-rw-r--r--   0        0        0      453 2023-06-07 15:11:33.545119 cognite_neat-0.12.7/cognite/neat/core/workflow/utils.py
+-rw-r--r--   0        0        0      286 2023-06-07 15:11:33.545119 cognite_neat-0.12.7/cognite/neat/examples/data-models/power-grid-v0_1_0.graphql
+-rw-r--r--   0        0        0    94607 2023-06-07 15:11:33.545119 cognite_neat-0.12.7/cognite/neat/examples/graph-sheets/sheet2cdf-graph-capturing.xlsx
+-rw-r--r--   0        0        0    79580 2023-06-07 15:11:33.545119 cognite_neat-0.12.7/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx
+-rw-r--r--   0        0        0    77438 2023-06-07 15:11:33.545119 cognite_neat-0.12.7/cognite/neat/examples/rules/power-grid-example.xlsx
+-rw-r--r--   0        0        0    75865 2023-06-07 15:11:33.545119 cognite_neat-0.12.7/cognite/neat/examples/rules/rules-template.xlsx
+-rw-r--r--   0        0        0    52178 2023-06-07 15:11:33.545119 cognite_neat-0.12.7/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx
+-rw-r--r--   0        0        0    79427 2023-06-07 15:11:33.545119 cognite_neat-0.12.7/cognite/neat/examples/rules/source-to-solution-mapping-rules.xlsx
+-rw-r--r--   0        0        0  1437851 2023-06-07 15:11:33.549119 cognite_neat-0.12.7/cognite/neat/examples/source-graphs/Knowledge-Graph-Nordic44.xml
+-rw-r--r--   0        0        0     1461 2023-06-07 15:11:33.549119 cognite_neat-0.12.7/cognite/neat/examples/workflows/basic/workflow.py
+-rw-r--r--   0        0        0     1782 2023-06-07 15:11:33.549119 cognite_neat-0.12.7/cognite/neat/examples/workflows/basic/workflow.yaml
+-rw-r--r--   0        0        0    15632 2023-06-07 15:11:33.549119 cognite_neat-0.12.7/cognite/neat/examples/workflows/default/workflow.py
+-rw-r--r--   0        0        0     6774 2023-06-07 15:11:33.549119 cognite_neat-0.12.7/cognite/neat/examples/workflows/default/workflow.yaml
+-rw-r--r--   0        0        0     3630 2023-06-07 15:11:33.549119 cognite_neat-0.12.7/cognite/neat/examples/workflows/fdm_schema_generation/workflow.py
+-rw-r--r--   0        0        0     2573 2023-06-07 15:11:33.549119 cognite_neat-0.12.7/cognite/neat/examples/workflows/fdm_schema_generation/workflow.yaml
+-rw-r--r--   0        0        0    11477 2023-06-07 15:11:33.549119 cognite_neat-0.12.7/cognite/neat/examples/workflows/graph_db_import/workflow.py
+-rw-r--r--   0        0        0     4792 2023-06-07 15:11:33.549119 cognite_neat-0.12.7/cognite/neat/examples/workflows/graph_db_import/workflow.yaml
+-rw-r--r--   0        0        0    16421 2023-06-07 15:11:33.549119 cognite_neat-0.12.7/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.py
+-rw-r--r--   0        0        0     8083 2023-06-07 15:11:33.549119 cognite_neat-0.12.7/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.yaml
+-rw-r--r--   0        0        0    13242 2023-06-07 15:11:33.549119 cognite_neat-0.12.7/cognite/neat/examples/workflows/sheet2cdf/workflow.py
+-rw-r--r--   0        0        0     6025 2023-06-07 15:11:33.549119 cognite_neat-0.12.7/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml
+-rw-r--r--   0        0        0    11867 2023-06-07 15:11:33.549119 cognite_neat-0.12.7/cognite/neat/examples/workflows/sme_graph_capture/workflow.py
+-rw-r--r--   0        0        0     6837 2023-06-07 15:11:33.549119 cognite_neat-0.12.7/cognite/neat/examples/workflows/sme_graph_capture/workflow.yaml
+-rw-r--r--   0        0        0        0 2023-06-07 15:11:33.589120 cognite_neat-0.12.7/cognite/neat/explorer/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-07 15:11:33.589120 cognite_neat-0.12.7/cognite/neat/explorer/data_classes/__init__.py
+-rw-r--r--   0        0        0     1013 2023-06-07 15:11:33.589120 cognite_neat-0.12.7/cognite/neat/explorer/data_classes/rest.py
+-rw-r--r--   0        0        0    21517 2023-06-07 15:11:33.589120 cognite_neat-0.12.7/cognite/neat/explorer/explorer.py
+-rw-r--r--   0        0        0        0 2023-06-07 15:11:33.589120 cognite_neat-0.12.7/cognite/neat/explorer/utils/__init__.py
+-rw-r--r--   0        0        0      412 2023-06-07 15:11:33.589120 cognite_neat-0.12.7/cognite/neat/explorer/utils/data_mapping.py
+-rw-r--r--   0        0        0     4003 2023-06-07 15:11:33.589120 cognite_neat-0.12.7/cognite/neat/explorer/utils/query_templates.py
+-rw-r--r--   0        0        0       16 2023-06-07 15:11:33.549119 cognite_neat-0.12.7/cognite/neat/explorer-ui/index.html
+-rw-r--r--   0        0        0      312 2023-06-07 15:11:33.549119 cognite_neat-0.12.7/cognite/neat/explorer-ui/neat-app/.gitignore
+-rw-r--r--   0        0        0     3359 2023-06-07 15:11:33.549119 cognite_neat-0.12.7/cognite/neat/explorer-ui/neat-app/README.md
+-rw-r--r--   0        0        0      464 2023-06-07 15:11:33.549119 cognite_neat-0.12.7/cognite/neat/explorer-ui/neat-app/build/asset-manifest.json
+-rw-r--r--   0        0        0     3870 2023-06-07 15:11:33.549119 cognite_neat-0.12.7/cognite/neat/explorer-ui/neat-app/build/favicon.ico
+-rw-r--r--   0        0        0      630 2023-06-07 15:11:33.549119 cognite_neat-0.12.7/cognite/neat/explorer-ui/neat-app/build/index.html
+-rw-r--r--   0        0        0     5347 2023-06-07 15:11:33.549119 cognite_neat-0.12.7/cognite/neat/explorer-ui/neat-app/build/logo192.png
+-rw-r--r--   0        0        0      492 2023-06-07 15:11:33.549119 cognite_neat-0.12.7/cognite/neat/explorer-ui/neat-app/build/manifest.json
+-rw-r--r--   0        0        0       67 2023-06-07 15:11:33.549119 cognite_neat-0.12.7/cognite/neat/explorer-ui/neat-app/build/robots.txt
+-rw-r--r--   0        0        0     8524 2023-06-07 15:11:33.553119 cognite_neat-0.12.7/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css
+-rw-r--r--   0        0        0    13319 2023-06-07 15:11:33.553119 cognite_neat-0.12.7/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css.map
+-rw-r--r--   0        0        0  1359583 2023-06-07 15:11:33.557119 cognite_neat-0.12.7/cognite/neat/explorer-ui/neat-app/build/static/js/main.97e96de0.js
+-rw-r--r--   0        0        0     2667 2023-06-07 15:11:33.557119 cognite_neat-0.12.7/cognite/neat/explorer-ui/neat-app/build/static/js/main.97e96de0.js.LICENSE.txt
+-rw-r--r--   0        0        0  5853485 2023-06-07 15:11:33.585119 cognite_neat-0.12.7/cognite/neat/explorer-ui/neat-app/build/static/js/main.97e96de0.js.map
+-rw-r--r--   0        0        0     2633 2023-06-07 15:11:33.585119 cognite_neat-0.12.7/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg
+-rw-r--r--   0        0        0      358 2023-06-07 15:11:33.589120 cognite_neat-0.12.7/cognite/neat/main.py
+-rw-r--r--   0        0        0        0 2023-06-07 15:11:33.589120 cognite_neat-0.12.7/cognite/neat/migration/__init__.py
+-rw-r--r--   0        0        0     1581 2023-06-07 15:11:33.589120 cognite_neat-0.12.7/cognite/neat/migration/wf_manifests.py
+-rw-r--r--   0        0        0     2471 2023-06-07 15:11:33.993125 cognite_neat-0.12.7/pyproject.toml
+-rw-r--r--   0        0        0    10241 1970-01-01 00:00:00.000000 cognite_neat-0.12.7/PKG-INFO
```

### Comparing `cognite_neat-0.12.6/LICENSE` & `cognite_neat-0.12.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/README.md` & `cognite_neat-0.12.7/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/constants.py` & `cognite_neat-0.12.7/cognite/neat/constants.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/core/app.py` & `cognite_neat-0.12.7/cognite/neat/core/app.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/core/configuration.py` & `cognite_neat-0.12.7/cognite/neat/core/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/core/data_classes/config.py` & `cognite_neat-0.12.7/cognite/neat/core/data_classes/config.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/core/data_classes/rules.py` & `cognite_neat-0.12.7/cognite/neat/core/data_classes/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/core/data_classes/transformation_rules.py` & `cognite_neat-0.12.7/cognite/neat/core/data_classes/transformation_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/core/data_stores/metrics.py` & `cognite_neat-0.12.7/cognite/neat/core/data_stores/metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/core/data_stores/oxrdflib.py` & `cognite_neat-0.12.7/cognite/neat/core/data_stores/oxrdflib.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/core/extractors/__init__.py` & `cognite_neat-0.12.7/cognite/neat/core/extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/core/extractors/graph_sheet_to_graph.py` & `cognite_neat-0.12.7/cognite/neat/core/extractors/graph_sheet_to_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/core/extractors/labels.py` & `cognite_neat-0.12.7/cognite/neat/core/extractors/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/core/extractors/rdf_to_assets.py` & `cognite_neat-0.12.7/cognite/neat/core/extractors/rdf_to_assets.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 import warnings
+from collections.abc import Sequence
 from datetime import datetime, timezone
-from typing import Dict, List, Optional, Tuple, Union
+from typing import Dict, List, Optional, Tuple, Union, overload
 from warnings import warn
 
 import numpy as np
 import pandas as pd
 from cognite.client import CogniteClient
 from cognite.client.data_classes import Asset, AssetHierarchy, AssetList
 from deepdiff import DeepDiff
@@ -336,15 +337,15 @@
 
 
 def rdf2assets(
     graph_store: NeatGraphStore,
     transformation_rules: TransformationRules,
     stop_on_exception: bool = False,
     use_orphanage: bool = True,
-) -> Dict[str, Asset]:
+) -> dict[str, Asset]:
     """Creates assets from RDF graph
 
     Parameters
     ----------
     graph : Graph
         Graph containing RDF data
     transformation_rules : TransformationRules
@@ -363,15 +364,15 @@
     graph = graph_store.get_graph()
     # Step 1: Create rdf to asset property mapping
     logging.info("Generating rdf to asset property mapping")
     asset_class_mapping = _define_asset_class_mapping(transformation_rules)
 
     # Step 4: Get ids of classes
     logging.info("Get ids of instances of classes")
-    assets = {}
+    assets: dict[str, Asset] = {}
     class_ids = {
         class_: _get_class_instance_ids(graph, class_, transformation_rules.metadata.namespace)
         for class_ in asset_class_mapping
     }
     # Step 5: Create Assets based on class instances
     logging.info("Create Assets based on class instances")
     for class_ in asset_class_mapping:
@@ -430,14 +431,15 @@
                     raise ValidationError
 
         logging.debug(f"Class <{class_}> processed")
 
     if orphanage_asset_external_id not in assets:
         _extracted_from_rdf2asset_dictionary_95(orphanage_asset_external_id, transformation_rules, assets)
     logging.info("Assets dictionary created")
+
     return assets
 
 
 def rdf2asset_dictionary(
     graph_store: NeatGraphStore,
     transformation_rules: TransformationRules,
     stop_on_exception: bool = False,
@@ -511,15 +513,19 @@
         Number of partitions
 
     Returns
     -------
     Tuple[Optional[pd.DataFrame], dict]
         CDF assets as pandas dataframe and dictionary with categorized assets
     """
-    cdf_assets = client.assets.list(data_set_ids=data_set_id, limit=None, partitions=partitions).to_pandas()
+    cdf_assets = client.assets.list(data_set_ids=data_set_id, limit=None, partitions=partitions)
+
+    cdf_assets = remove_non_existing_labels(client, cdf_assets)
+
+    cdf_assets = AssetList(resources=cdf_assets).to_pandas()
 
     logging.info(f"Number of assets in CDF {len(cdf_assets)} that have been fetched")
 
     if cdf_assets.empty:
         return None, {"non-historic": set(), "historic": set()}
     if "labels" not in cdf_assets:
         # Add empty list for labels column.
@@ -869,15 +875,15 @@
         msg = f"{message} {counter} of {total} assets, batch processing time: {delta_time:.2f} "
         msg += f"seconds ETC: {delta_time * (total - counter) / (60*batch_size) :.2f} minutes"
         logging.info(msg)
 
 
 def upload_assets(
     client: CogniteClient,
-    categorized_assets: Dict[str, list],
+    categorized_assets: Dict[str, Sequence[Asset]],
     batch_size: int = 5000,
     max_retries: int = 1,
     retry_delay: int = 3,
 ):
     """Uploads categorized assets to CDF
 
     Parameters
@@ -946,7 +952,46 @@
             if categorized_assets["resurrect"]:
                 client.assets.create_hierarchy(categorized_assets["resurrect"], upsert=True, upsert_mode="replace")
 
             if categorized_assets["decommission"]:
                 client.assets.create_hierarchy(categorized_assets["decommission"], upsert=True, upsert_mode="replace")
 
         create_assets()
+
+
+@overload
+def remove_non_existing_labels(client: CogniteClient, assets: Sequence[Asset]) -> Sequence[Asset]:
+    ...
+
+
+@overload
+def remove_non_existing_labels(client: CogniteClient, assets: dict[str, Asset]) -> dict[str, Asset]:
+    ...
+
+
+def remove_non_existing_labels(
+    client: CogniteClient, assets: Sequence[Asset] | dict[str, Asset]
+) -> Sequence[Asset] | dict[str, Asset]:
+    cdf_labels = client.labels.list(limit=-1)
+    if not cdf_labels:
+        # No labels, nothing to check.
+        return assets
+
+    available_labels = {label.external_id for label in cdf_labels}
+
+    if isinstance(assets, Sequence):
+        cleaned_assets: list[Asset] = []
+        for asset in assets:
+            if hasattr(asset, "labels"):
+                asset.labels = [label for label in asset.labels if label.external_id in available_labels]
+            cleaned_assets.append(asset)
+        return cleaned_assets
+
+    elif isinstance(assets, dict):
+        cleaned_assets: dict[str, Asset] = {}
+        for asset_id, asset in assets.items():
+            if hasattr(asset, "labels"):
+                asset.labels = [label for label in asset.labels if label.external_id in available_labels]
+            cleaned_assets[asset_id] = asset
+        return cleaned_assets
+
+    raise ValueError(f"Invalid format for Assets={type(assets)}")
```

### Comparing `cognite_neat-0.12.6/cognite/neat/core/extractors/rdf_to_relationships.py` & `cognite_neat-0.12.7/cognite/neat/core/extractors/rdf_to_relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/core/extractors/rules_to_graph_capturing_sheet.py` & `cognite_neat-0.12.7/cognite/neat/core/extractors/rules_to_graph_capturing_sheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/core/extractors/rules_to_graphql.py` & `cognite_neat-0.12.7/cognite/neat/core/extractors/rules_to_graphql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/core/loader/config.py` & `cognite_neat-0.12.7/cognite/neat/core/loader/config.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/core/loader/graph.py` & `cognite_neat-0.12.7/cognite/neat/core/loader/graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/core/loader/graph_capturing_sheet.py` & `cognite_neat-0.12.7/cognite/neat/core/loader/graph_capturing_sheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/core/loader/graph_store.py` & `cognite_neat-0.12.7/cognite/neat/core/loader/graph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/core/loader/rules.py` & `cognite_neat-0.12.7/cognite/neat/core/loader/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/core/mocks/graph.py` & `cognite_neat-0.12.7/cognite/neat/core/mocks/graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/core/modeler.py` & `cognite_neat-0.12.7/cognite/neat/core/modeler.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/core/parser/transformation_rules.py` & `cognite_neat-0.12.7/cognite/neat/core/parser/transformation_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/core/query_generator/sparql.py` & `cognite_neat-0.12.7/cognite/neat/core/query_generator/sparql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/core/transformer.py` & `cognite_neat-0.12.7/cognite/neat/core/transformer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/core/utils.py` & `cognite_neat-0.12.7/cognite/neat/core/utils.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/core/validator.py` & `cognite_neat-0.12.7/cognite/neat/core/validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         msg = f"Your asset hierarchy is too deep. Max depth is {max_hierarchy_depth}. You probably have a circular reference."
         logging.error(msg)
         return circle
     else:
         return []
 
 
-def validate_asset_hierarchy(assets: dict[str, dict]) -> Tuple[List[str], List[List[str]]]:
+def validate_asset_hierarchy(assets: dict[str, Asset]) -> Tuple[List[str], List[List[str]]]:
     """Validates asset hierarchy and reports on orphan assets and circular dependency
 
     Parameters
     ----------
     assets : dict[str, Asset]
         A dictionary of assets with external_id as key
```

### Comparing `cognite_neat-0.12.6/cognite/neat/core/workflow/base.py` & `cognite_neat-0.12.7/cognite/neat/core/workflow/base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/core/workflow/cdf_store.py` & `cognite_neat-0.12.7/cognite/neat/core/workflow/cdf_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/core/workflow/manager.py` & `cognite_neat-0.12.7/cognite/neat/core/workflow/manager.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/core/workflow/model.py` & `cognite_neat-0.12.7/cognite/neat/core/workflow/model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/core/workflow/tasks.py` & `cognite_neat-0.12.7/cognite/neat/core/workflow/tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/core/workflow/triggers.py` & `cognite_neat-0.12.7/cognite/neat/core/workflow/triggers.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/examples/graph-sheets/sheet2cdf-graph-capturing.xlsx` & `cognite_neat-0.12.7/cognite/neat/examples/graph-sheets/sheet2cdf-graph-capturing.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx` & `cognite_neat-0.12.7/cognite/neat/examples/rules/Rules-Nordic44-to-TNT.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/examples/rules/power-grid-example.xlsx` & `cognite_neat-0.12.7/cognite/neat/examples/rules/power-grid-example.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/examples/rules/rules-template.xlsx` & `cognite_neat-0.12.7/cognite/neat/examples/rules/rules-template.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx` & `cognite_neat-0.12.7/cognite/neat/examples/rules/sheet2cdf-transformation-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/examples/rules/source-to-solution-mapping-rules.xlsx` & `cognite_neat-0.12.7/cognite/neat/examples/rules/source-to-solution-mapping-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/examples/source-graphs/Knowledge-Graph-Nordic44.xml` & `cognite_neat-0.12.7/cognite/neat/examples/source-graphs/Knowledge-Graph-Nordic44.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/examples/workflows/basic/workflow.py` & `cognite_neat-0.12.7/cognite/neat/examples/workflows/basic/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/examples/workflows/basic/workflow.yaml` & `cognite_neat-0.12.7/cognite/neat/examples/workflows/basic/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/examples/workflows/default/workflow.py` & `cognite_neat-0.12.7/cognite/neat/examples/workflows/default/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/examples/workflows/default/workflow.yaml` & `cognite_neat-0.12.7/cognite/neat/examples/workflows/default/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/examples/workflows/fdm_schema_generation/workflow.py` & `cognite_neat-0.12.7/cognite/neat/examples/workflows/fdm_schema_generation/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/examples/workflows/fdm_schema_generation/workflow.yaml` & `cognite_neat-0.12.7/cognite/neat/examples/workflows/fdm_schema_generation/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/examples/workflows/graph_db_import/workflow.py` & `cognite_neat-0.12.7/cognite/neat/examples/workflows/graph_db_import/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/examples/workflows/graph_db_import/workflow.yaml` & `cognite_neat-0.12.7/cognite/neat/examples/workflows/graph_db_import/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.py` & `cognite_neat-0.12.7/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.yaml` & `cognite_neat-0.12.7/cognite/neat/examples/workflows/graph_to_asset_hierarchy/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/examples/workflows/sheet2cdf/workflow.py` & `cognite_neat-0.12.7/cognite/neat/examples/workflows/sheet2cdf/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,20 @@
 from cognite.client import CogniteClient
 from cognite.client.data_classes import AssetFilter
 from prometheus_client import Gauge
 
 from cognite.neat.core import loader, parser
 from cognite.neat.core.data_classes.transformation_rules import TransformationRules
 from cognite.neat.core.extractors.labels import upload_labels
-from cognite.neat.core.extractors.rdf_to_assets import categorize_assets, rdf2assets, upload_assets
+from cognite.neat.core.extractors.rdf_to_assets import (
+    categorize_assets,
+    rdf2assets,
+    remove_non_existing_labels,
+    upload_assets,
+)
 from cognite.neat.core.extractors.rdf_to_relationships import (
     categorize_relationships,
     rdf2relationships,
     upload_relationships,
 )
 from cognite.neat.core.loader.graph_store import NeatGraphStore
 from cognite.neat.core.validator import validate_asset_hierarchy
@@ -129,14 +134,16 @@
             stop_on_exception=self.stop_on_error,
         )
 
         if not self.cdf_client:
             logging.info("Dry run, no CDF client available")
             return
 
+        rdf_assets = remove_non_existing_labels(self.cdf_client, rdf_assets)
+
         # UPDATE: 2023-04-05 - correct aggregation of assets in CDF for specific dataset
         total_assets_before = self.cdf_client.assets.aggregate(
             filter=AssetFilter(data_set_ids=[{"id": self.dataset_id}])
         )[0]["count"]
 
         prom_cdf_resource_stats.labels(resource_type="asset", state="count_before_neat_update").set(total_assets_before)
         logging.info(f"Total count of assets in CDF before upload: { total_assets_before }")
```

### Comparing `cognite_neat-0.12.6/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml` & `cognite_neat-0.12.7/cognite/neat/examples/workflows/sheet2cdf/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/examples/workflows/sme_graph_capture/workflow.py` & `cognite_neat-0.12.7/cognite/neat/examples/workflows/sme_graph_capture/workflow.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/examples/workflows/sme_graph_capture/workflow.yaml` & `cognite_neat-0.12.7/cognite/neat/examples/workflows/sme_graph_capture/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/explorer/data_classes/rest.py` & `cognite_neat-0.12.7/cognite/neat/explorer/data_classes/rest.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/explorer/explorer.py` & `cognite_neat-0.12.7/cognite/neat/explorer/explorer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/explorer/utils/query_templates.py` & `cognite_neat-0.12.7/cognite/neat/explorer/utils/query_templates.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/explorer-ui/neat-app/README.md` & `cognite_neat-0.12.7/cognite/neat/explorer-ui/neat-app/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/explorer-ui/neat-app/build/favicon.ico` & `cognite_neat-0.12.7/cognite/neat/explorer-ui/neat-app/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/explorer-ui/neat-app/build/index.html` & `cognite_neat-0.12.7/cognite/neat/explorer-ui/neat-app/build/index.html`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/explorer-ui/neat-app/build/logo192.png` & `cognite_neat-0.12.7/cognite/neat/explorer-ui/neat-app/build/logo192.png`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css` & `cognite_neat-0.12.7/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css.map` & `cognite_neat-0.12.7/cognite/neat/explorer-ui/neat-app/build/static/css/main.38a62222.css.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/explorer-ui/neat-app/build/static/js/main.97e96de0.js` & `cognite_neat-0.12.7/cognite/neat/explorer-ui/neat-app/build/static/js/main.97e96de0.js`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/explorer-ui/neat-app/build/static/js/main.97e96de0.js.LICENSE.txt` & `cognite_neat-0.12.7/cognite/neat/explorer-ui/neat-app/build/static/js/main.97e96de0.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/explorer-ui/neat-app/build/static/js/main.97e96de0.js.map` & `cognite_neat-0.12.7/cognite/neat/explorer-ui/neat-app/build/static/js/main.97e96de0.js.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg` & `cognite_neat-0.12.7/cognite/neat/explorer-ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/cognite/neat/migration/wf_manifests.py` & `cognite_neat-0.12.7/cognite/neat/migration/wf_manifests.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.12.6/pyproject.toml` & `cognite_neat-0.12.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-neat"
-version = "0.12.6"
+version = "0.12.7"
 readme = "README.md"
 description = "Knowledge graph transformation"
 authors = ["Nikola Vasiljevic <nikola.vasiljevic@cognite.com>",
     "Anders Albert <anders.albert@cognite.com>",
     "Aleksandrs Livincovs <aleksandrs.livincovs@cognite.com>"]
 license = "Apache-2.0"
 packages = [
```

### Comparing `cognite_neat-0.12.6/PKG-INFO` & `cognite_neat-0.12.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-neat
-Version: 0.12.6
+Version: 0.12.7
 Summary: Knowledge graph transformation
 License: Apache-2.0
 Author: Nikola Vasiljevic
 Author-email: nikola.vasiljevic@cognite.com
 Requires-Python: >=3.11,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

