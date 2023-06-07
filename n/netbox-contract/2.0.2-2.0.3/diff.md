# Comparing `tmp/netbox-contract-2.0.2.tar.gz` & `tmp/netbox-contract-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-contract-2.0.2.tar", last modified: Sun Jun  4 08:16:25 2023, max compression
+gzip compressed data, was "netbox-contract-2.0.3.tar", last modified: Wed Jun  7 19:32:38 2023, max compression
```

## Comparing `netbox-contract-2.0.2.tar` & `netbox-contract-2.0.3.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-04 08:16:25.767368 netbox-contract-2.0.2/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1056 2023-01-03 17:10:18.000000 netbox-contract-2.0.2/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)       87 2023-03-12 14:44:04.000000 netbox-contract-2.0.2/MANIFEST.in
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2895 2023-06-04 08:16:25.767368 netbox-contract-2.0.2/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2356 2023-06-04 08:14:44.000000 netbox-contract-2.0.2/README.md
--rw-r--r--   0 vscode    (1000) vscode    (1000)      774 2023-06-04 08:15:08.000000 netbox-contract-2.0.2/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-06-04 08:16:25.767368 netbox-contract-2.0.2/setup.cfg
--rw-rw-r--   0 vscode    (1000) vscode    (1000)       52 2023-01-03 18:27:10.000000 netbox-contract-2.0.2/setup.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-04 08:16:25.691366 netbox-contract-2.0.2/src/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-04 08:16:25.715367 netbox-contract-2.0.2/src/netbox_contract/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      469 2023-06-04 08:14:58.000000 netbox-contract-2.0.2/src/netbox_contract/__init__.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-04 08:16:25.735367 netbox-contract-2.0.2/src/netbox_contract/api/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-03-12 14:46:55.000000 netbox-contract-2.0.2/src/netbox_contract/api/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4016 2023-06-01 20:59:57.000000 netbox-contract-2.0.2/src/netbox_contract/api/serializers.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      387 2023-06-01 20:59:57.000000 netbox-contract-2.0.2/src/netbox_contract/api/urls.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      955 2023-06-01 20:59:57.000000 netbox-contract-2.0.2/src/netbox_contract/api/views.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1369 2023-06-01 20:59:57.000000 netbox-contract-2.0.2/src/netbox_contract/filtersets.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5650 2023-06-01 21:20:01.000000 netbox-contract-2.0.2/src/netbox_contract/forms.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-04 08:16:25.743367 netbox-contract-2.0.2/src/netbox_contract/migrations/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4598 2023-03-12 14:46:55.000000 netbox-contract-2.0.2/src/netbox_contract/migrations/0001_initial.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      764 2023-03-12 14:46:55.000000 netbox-contract-2.0.2/src/netbox_contract/migrations/0002_alter_contract_circuit_and_more.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1579 2023-03-12 14:46:55.000000 netbox-contract-2.0.2/src/netbox_contract/migrations/0003_alter_contract_custom_field_data_and_more.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      601 2023-03-12 14:46:55.000000 netbox-contract-2.0.2/src/netbox_contract/migrations/0004_contract_currency_invoice_currency.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      584 2023-03-12 14:46:55.000000 netbox-contract-2.0.2/src/netbox_contract/migrations/0005_contract_accounting_dimensions_and_more.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      563 2023-03-12 14:46:55.000000 netbox-contract-2.0.2/src/netbox_contract/migrations/0006_alter_contract_circuit.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      403 2023-03-12 14:46:55.000000 netbox-contract-2.0.2/src/netbox_contract/migrations/0007_invoice_date.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      386 2023-03-12 14:46:55.000000 netbox-contract-2.0.2/src/netbox_contract/migrations/0008_invoice_comments.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      428 2023-03-12 14:46:55.000000 netbox-contract-2.0.2/src/netbox_contract/migrations/0009_contract_external_reference.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      494 2023-03-12 14:46:55.000000 netbox-contract-2.0.2/src/netbox_contract/migrations/0010_invoice_contracts.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      610 2023-03-12 14:46:55.000000 netbox-contract-2.0.2/src/netbox_contract/migrations/0011_auto_20230122_2112.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      339 2023-03-12 14:46:55.000000 netbox-contract-2.0.2/src/netbox_contract/migrations/0012_remove_invoice_contract.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      549 2023-03-12 14:46:55.000000 netbox-contract-2.0.2/src/netbox_contract/migrations/0013_contract_documents_invoice_documents.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      422 2023-03-12 14:46:55.000000 netbox-contract-2.0.2/src/netbox_contract/migrations/0014_contract_end_date.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2104 2023-06-01 20:59:57.000000 netbox-contract-2.0.2/src/netbox_contract/migrations/0015_contractassignement.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-03-12 14:46:55.000000 netbox-contract-2.0.2/src/netbox_contract/migrations/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5517 2023-06-01 20:59:57.000000 netbox-contract-2.0.2/src/netbox_contract/models.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1644 2023-03-12 18:00:52.000000 netbox-contract-2.0.2/src/netbox_contract/navigation.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      559 2023-03-12 14:46:55.000000 netbox-contract-2.0.2/src/netbox_contract/search.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3712 2023-06-01 20:59:57.000000 netbox-contract-2.0.2/src/netbox_contract/tables.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2027 2023-06-01 20:59:57.000000 netbox-contract-2.0.2/src/netbox_contract/template_content.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-04 08:16:25.743367 netbox-contract-2.0.2/src/netbox_contract/templates/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      775 2023-06-01 20:59:57.000000 netbox-contract-2.0.2/src/netbox_contract/templates/contract_assignements_bottom.html
--rw-r--r--   0 vscode    (1000) vscode    (1000)      305 2023-05-24 18:09:51.000000 netbox-contract-2.0.2/src/netbox_contract/templates/contract_list_bottom.html
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-04 08:16:25.767368 netbox-contract-2.0.2/src/netbox_contract/templates/netbox_contract/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4257 2023-06-01 20:59:57.000000 netbox-contract-2.0.2/src/netbox_contract/templates/netbox_contract/contract.html
--rw-r--r--   0 vscode    (1000) vscode    (1000)      810 2023-06-01 20:59:57.000000 netbox-contract-2.0.2/src/netbox_contract/templates/netbox_contract/contract_assignement.html
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2284 2023-03-12 17:52:54.000000 netbox-contract-2.0.2/src/netbox_contract/templates/netbox_contract/invoice.html
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1128 2023-03-12 14:46:55.000000 netbox-contract-2.0.2/src/netbox_contract/templates/netbox_contract/serviceprovider.html
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3751 2023-06-01 20:59:57.000000 netbox-contract-2.0.2/src/netbox_contract/urls.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8388 2023-06-01 20:59:57.000000 netbox-contract-2.0.2/src/netbox_contract/views.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-04 08:16:25.727367 netbox-contract-2.0.2/src/netbox_contract.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2895 2023-06-04 08:16:25.000000 netbox-contract-2.0.2/src/netbox_contract.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2145 2023-06-04 08:16:25.000000 netbox-contract-2.0.2/src/netbox_contract.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-04 08:16:25.000000 netbox-contract-2.0.2/src/netbox_contract.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-02-19 10:47:00.000000 netbox-contract-2.0.2/src/netbox_contract.egg-info/not-zip-safe
--rw-r--r--   0 vscode    (1000) vscode    (1000)       16 2023-06-04 08:16:25.000000 netbox-contract-2.0.2/src/netbox_contract.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       16 2023-06-04 08:16:25.000000 netbox-contract-2.0.2/src/netbox_contract.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-07 19:32:38.865804 netbox-contract-2.0.3/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1056 2023-01-03 17:10:18.000000 netbox-contract-2.0.3/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       87 2023-03-12 14:44:04.000000 netbox-contract-2.0.3/MANIFEST.in
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3156 2023-06-07 19:32:38.861803 netbox-contract-2.0.3/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2617 2023-06-07 19:30:34.000000 netbox-contract-2.0.3/README.md
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      774 2023-06-07 19:31:19.000000 netbox-contract-2.0.3/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-06-07 19:32:38.865804 netbox-contract-2.0.3/setup.cfg
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)       52 2023-01-03 18:27:10.000000 netbox-contract-2.0.3/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-07 19:32:38.765802 netbox-contract-2.0.3/src/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-07 19:32:38.809802 netbox-contract-2.0.3/src/netbox_contract/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      469 2023-06-07 19:31:06.000000 netbox-contract-2.0.3/src/netbox_contract/__init__.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-07 19:32:38.829803 netbox-contract-2.0.3/src/netbox_contract/api/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-03-12 14:46:55.000000 netbox-contract-2.0.3/src/netbox_contract/api/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4016 2023-06-01 20:59:57.000000 netbox-contract-2.0.3/src/netbox_contract/api/serializers.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      387 2023-06-01 20:59:57.000000 netbox-contract-2.0.3/src/netbox_contract/api/urls.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      955 2023-06-01 20:59:57.000000 netbox-contract-2.0.3/src/netbox_contract/api/views.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1435 2023-06-04 09:17:47.000000 netbox-contract-2.0.3/src/netbox_contract/filtersets.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5650 2023-06-04 08:54:12.000000 netbox-contract-2.0.3/src/netbox_contract/forms.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-07 19:32:38.853803 netbox-contract-2.0.3/src/netbox_contract/migrations/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4598 2023-03-12 14:46:55.000000 netbox-contract-2.0.3/src/netbox_contract/migrations/0001_initial.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      764 2023-03-12 14:46:55.000000 netbox-contract-2.0.3/src/netbox_contract/migrations/0002_alter_contract_circuit_and_more.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1579 2023-03-12 14:46:55.000000 netbox-contract-2.0.3/src/netbox_contract/migrations/0003_alter_contract_custom_field_data_and_more.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      601 2023-03-12 14:46:55.000000 netbox-contract-2.0.3/src/netbox_contract/migrations/0004_contract_currency_invoice_currency.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      584 2023-03-12 14:46:55.000000 netbox-contract-2.0.3/src/netbox_contract/migrations/0005_contract_accounting_dimensions_and_more.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      563 2023-03-12 14:46:55.000000 netbox-contract-2.0.3/src/netbox_contract/migrations/0006_alter_contract_circuit.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      403 2023-03-12 14:46:55.000000 netbox-contract-2.0.3/src/netbox_contract/migrations/0007_invoice_date.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      386 2023-03-12 14:46:55.000000 netbox-contract-2.0.3/src/netbox_contract/migrations/0008_invoice_comments.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      428 2023-03-12 14:46:55.000000 netbox-contract-2.0.3/src/netbox_contract/migrations/0009_contract_external_reference.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      494 2023-03-12 14:46:55.000000 netbox-contract-2.0.3/src/netbox_contract/migrations/0010_invoice_contracts.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      610 2023-03-12 14:46:55.000000 netbox-contract-2.0.3/src/netbox_contract/migrations/0011_auto_20230122_2112.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      339 2023-03-12 14:46:55.000000 netbox-contract-2.0.3/src/netbox_contract/migrations/0012_remove_invoice_contract.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      549 2023-03-12 14:46:55.000000 netbox-contract-2.0.3/src/netbox_contract/migrations/0013_contract_documents_invoice_documents.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      422 2023-03-12 14:46:55.000000 netbox-contract-2.0.3/src/netbox_contract/migrations/0014_contract_end_date.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2104 2023-06-01 20:59:57.000000 netbox-contract-2.0.3/src/netbox_contract/migrations/0015_contractassignement.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-03-12 14:46:55.000000 netbox-contract-2.0.3/src/netbox_contract/migrations/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5517 2023-06-01 20:59:57.000000 netbox-contract-2.0.3/src/netbox_contract/models.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1982 2023-06-07 19:20:38.000000 netbox-contract-2.0.3/src/netbox_contract/navigation.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      559 2023-03-12 14:46:55.000000 netbox-contract-2.0.3/src/netbox_contract/search.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3712 2023-06-01 20:59:57.000000 netbox-contract-2.0.3/src/netbox_contract/tables.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2027 2023-06-01 20:59:57.000000 netbox-contract-2.0.3/src/netbox_contract/template_content.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-07 19:32:38.857803 netbox-contract-2.0.3/src/netbox_contract/templates/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      917 2023-06-07 19:05:00.000000 netbox-contract-2.0.3/src/netbox_contract/templates/contract_assignements_bottom.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      362 2023-06-07 19:03:26.000000 netbox-contract-2.0.3/src/netbox_contract/templates/contract_list_bottom.html
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-07 19:32:38.861803 netbox-contract-2.0.3/src/netbox_contract/templates/netbox_contract/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4390 2023-06-07 19:24:12.000000 netbox-contract-2.0.3/src/netbox_contract/templates/netbox_contract/contract.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      810 2023-06-01 20:59:57.000000 netbox-contract-2.0.3/src/netbox_contract/templates/netbox_contract/contract_assignement.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2284 2023-03-12 17:52:54.000000 netbox-contract-2.0.3/src/netbox_contract/templates/netbox_contract/invoice.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1128 2023-03-12 14:46:55.000000 netbox-contract-2.0.3/src/netbox_contract/templates/netbox_contract/serviceprovider.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3751 2023-06-01 20:59:57.000000 netbox-contract-2.0.3/src/netbox_contract/urls.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8388 2023-06-01 20:59:57.000000 netbox-contract-2.0.3/src/netbox_contract/views.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-07 19:32:38.825803 netbox-contract-2.0.3/src/netbox_contract.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3156 2023-06-07 19:32:38.000000 netbox-contract-2.0.3/src/netbox_contract.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2145 2023-06-07 19:32:38.000000 netbox-contract-2.0.3/src/netbox_contract.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-07 19:32:38.000000 netbox-contract-2.0.3/src/netbox_contract.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-02-19 10:47:00.000000 netbox-contract-2.0.3/src/netbox_contract.egg-info/not-zip-safe
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       16 2023-06-07 19:32:38.000000 netbox-contract-2.0.3/src/netbox_contract.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       16 2023-06-07 19:32:38.000000 netbox-contract-2.0.3/src/netbox_contract.egg-info/top_level.txt
```

### Comparing `netbox-contract-2.0.2/LICENSE` & `netbox-contract-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.2/PKG-INFO` & `netbox-contract-2.0.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: netbox-contract
-Version: 2.0.2
-Summary: Contract management plugin for Netbox
-Author-email: Marc Lebreuil <marc@famillelebreuil.net>
-Project-URL: Homepage, https://github.com/mlebreuil/netbox-contract
-Project-URL: Bug Tracker, https://github.com/mlebreuil/netbox-contract/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Contract pluggin
 ## Overview
 The pluggin adds contracts and invoices model to Netbox.  
 It allows to register contract with objects.  
 Add invoices to contracts.  
 
 ## Installation
@@ -87,8 +73,13 @@
 
 #### version 2.0.1
 
 Add support contract assignement panel to devices.
 
 #### version 2.0.2
 
-Add support for Netbox 3.5 whcih become the minimum version supported to accoodate the removal of NetBoxModelCSVForm class (replaced by NetBoxModelImportForm) .
+Add support for Netbox 3.5 which become the minimum version supported to accomodate the removal of NetBoxModelCSVForm class (replaced by NetBoxModelImportForm) .
+
+#### version 2.0.3
+
+* [#60](https://github.com/mlebreuil/netbox-contract/issues/60) Update contract quick search to also filter on fields "External reference" and "Comments".
+* [#49](https://github.com/mlebreuil/netbox-contract/issues/49) Manage permissions.
```

### Comparing `netbox-contract-2.0.2/README.md` & `netbox-contract-2.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: netbox-contract
+Version: 2.0.3
+Summary: Contract management plugin for Netbox
+Author-email: Marc Lebreuil <marc@famillelebreuil.net>
+Project-URL: Homepage, https://github.com/mlebreuil/netbox-contract
+Project-URL: Bug Tracker, https://github.com/mlebreuil/netbox-contract/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Contract pluggin
 ## Overview
 The pluggin adds contracts and invoices model to Netbox.  
 It allows to register contract with objects.  
 Add invoices to contracts.  
 
 ## Installation
@@ -73,8 +87,13 @@
 
 #### version 2.0.1
 
 Add support contract assignement panel to devices.
 
 #### version 2.0.2
 
-Add support for Netbox 3.5 whcih become the minimum version supported to accoodate the removal of NetBoxModelCSVForm class (replaced by NetBoxModelImportForm) .
+Add support for Netbox 3.5 which become the minimum version supported to accomodate the removal of NetBoxModelCSVForm class (replaced by NetBoxModelImportForm) .
+
+#### version 2.0.3
+
+* [#60](https://github.com/mlebreuil/netbox-contract/issues/60) Update contract quick search to also filter on fields "External reference" and "Comments".
+* [#49](https://github.com/mlebreuil/netbox-contract/issues/49) Manage permissions.
```

### Comparing `netbox-contract-2.0.2/pyproject.toml` & `netbox-contract-2.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "netbox-contract"
-version = "2.0.2"
+version = "2.0.3"
 authors = [
   { name="Marc Lebreuil", email="marc@famillelebreuil.net" },
 ]
 description = "Contract management plugin for Netbox"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
```

### Comparing `netbox-contract-2.0.2/src/netbox_contract/api/serializers.py` & `netbox-contract-2.0.3/src/netbox_contract/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.2/src/netbox_contract/api/views.py` & `netbox-contract-2.0.3/src/netbox_contract/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.2/src/netbox_contract/filtersets.py` & `netbox-contract-2.0.3/src/netbox_contract/filtersets.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 class ContractFilterSet(NetBoxModelFilterSet):
 
     class Meta:
         model = Contract
         fields = ('id', 'external_partie', 'internal_partie', 'status','circuit')
 
     def search(self, queryset, name, value):
-        return queryset.filter( Q(name__icontains=value) 
-                               | Q(circuit__cid__icontains=value) 
-                               | Q(external_partie__name__icontains=value))
+        return queryset.filter( Q(name__icontains=value)
+                               | Q(external_partie__name__icontains=value)
+                               | Q(external_reference__icontains=value)
+                               | Q(comments__icontains=value))
 
 class InvoiceFilterSet(NetBoxModelFilterSet):
 
     class Meta:
         model = Invoice
         fields = ('id', 'contracts')
```

### Comparing `netbox-contract-2.0.2/src/netbox_contract/forms.py` & `netbox-contract-2.0.3/src/netbox_contract/forms.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.2/src/netbox_contract/migrations/0001_initial.py` & `netbox-contract-2.0.3/src/netbox_contract/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.2/src/netbox_contract/migrations/0002_alter_contract_circuit_and_more.py` & `netbox-contract-2.0.3/src/netbox_contract/migrations/0002_alter_contract_circuit_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.2/src/netbox_contract/migrations/0003_alter_contract_custom_field_data_and_more.py` & `netbox-contract-2.0.3/src/netbox_contract/migrations/0003_alter_contract_custom_field_data_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.2/src/netbox_contract/migrations/0004_contract_currency_invoice_currency.py` & `netbox-contract-2.0.3/src/netbox_contract/migrations/0004_contract_currency_invoice_currency.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.2/src/netbox_contract/migrations/0005_contract_accounting_dimensions_and_more.py` & `netbox-contract-2.0.3/src/netbox_contract/migrations/0005_contract_accounting_dimensions_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.2/src/netbox_contract/migrations/0006_alter_contract_circuit.py` & `netbox-contract-2.0.3/src/netbox_contract/migrations/0006_alter_contract_circuit.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.2/src/netbox_contract/migrations/0011_auto_20230122_2112.py` & `netbox-contract-2.0.3/src/netbox_contract/migrations/0011_auto_20230122_2112.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.2/src/netbox_contract/migrations/0013_contract_documents_invoice_documents.py` & `netbox-contract-2.0.3/src/netbox_contract/migrations/0013_contract_documents_invoice_documents.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.2/src/netbox_contract/migrations/0015_contractassignement.py` & `netbox-contract-2.0.3/src/netbox_contract/migrations/0015_contractassignement.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.2/src/netbox_contract/models.py` & `netbox-contract-2.0.3/src/netbox_contract/models.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.2/src/netbox_contract/navigation.py` & `netbox-contract-2.0.3/src/netbox_contract/navigation.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,52 +5,58 @@
 plugin_settings = settings.PLUGINS_CONFIG["netbox_contract"]
 
 contract_buttons = [
     PluginMenuButton(
         link='plugins:netbox_contract:contract_add',
         title='Add',
         icon_class='mdi mdi-plus-thick',
-        color=ButtonColorChoices.GREEN
+        color=ButtonColorChoices.GREEN,
+        permissions=['netbox_contract.add_contract']
     )
 ]
 
 invoice_buttons = [
     PluginMenuButton(
         link='plugins:netbox_contract:invoice_add',
         title='Add',
         icon_class='mdi mdi-plus-thick',
-        color=ButtonColorChoices.GREEN
+        color=ButtonColorChoices.GREEN,
+        permissions=['netbox_contract.add_invoice']
     )
 ]
 
 serviceprovider_buttons = [
     PluginMenuButton(
         link='plugins:netbox_contract:serviceprovider_add',
         title='Add',
         icon_class='mdi mdi-plus-thick',
-        color=ButtonColorChoices.GREEN
+        color=ButtonColorChoices.GREEN,
+        permissions=['netbox_contract.add_serviceprovider']
     )
 ]
- 
+
 contract_menu_item = PluginMenuItem(
         link='plugins:netbox_contract:contract_list',
         link_text='Contracts',
-        buttons=contract_buttons
+        buttons=contract_buttons,
+        permissions=['netbox_contract.view_contract']
     )
 
 invoices_menu_item = PluginMenuItem(
         link='plugins:netbox_contract:invoice_list',
         link_text='Invoices',
-        buttons=invoice_buttons
+        buttons=invoice_buttons,
+        permissions=['netbox_contract.view_invoice']
     )
 
 service_provider_menu_item = PluginMenuItem(
         link='plugins:netbox_contract:serviceprovider_list',
         link_text='Service Providers',
-        buttons=serviceprovider_buttons
+        buttons=serviceprovider_buttons,
+        permissions=['netbox_contract.view_serviceprovider']
     )
 
 items = (contract_menu_item,invoices_menu_item,service_provider_menu_item)
 
 if plugin_settings.get("top_level_menu"):
     menu = PluginMenu(
         label="Contracts",
```

### Comparing `netbox-contract-2.0.2/src/netbox_contract/search.py` & `netbox-contract-2.0.3/src/netbox_contract/search.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.2/src/netbox_contract/tables.py` & `netbox-contract-2.0.3/src/netbox_contract/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.2/src/netbox_contract/template_content.py` & `netbox-contract-2.0.3/src/netbox_contract/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.2/src/netbox_contract/templates/contract_assignements_bottom.html` & `netbox-contract-2.0.3/src/netbox_contract/templates/contract_assignements_bottom.html`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 {% load render_table from django_tables2 %}
+{% if perms.netbox_contract.view_contract %}
 <div class="row">
     <div class="col col-md-12">
       <div class="card">
         <h5 class="card-header">Contracts Assignements</h5>
         {% if assignements_table %}
         <div class="card-body table-responsive">
           {% render_table assignements_table %}
         </div>
         {% endif %}
+        {% if perms.netbox_contract.add_contractassignement %}
         <div class="card-footer text-end noprint">
           <a href="{% url 'plugins:netbox_contract:contractassignement_add' %}?content_type={{ object|content_type_id }}&object_id={{ object.pk }}&return_url={{ object.get_absolute_url }}" class="btn btn-primary btn-sm">
               <i class="mdi mdi-plus-thick" aria-hidden="true"></i>
               Add assignement
           </a>
-      </div>
+        </div>
+        {% endif %}
       </div>
     </div>
-</div>
+</div>
+{% endif %}
```

#### html2text {}

```diff
@@ -1,6 +1,9 @@
-{% load render_table from django_tables2 %}
+{% load render_table from django_tables2 %} {% if
+perms.netbox_contract.view_contract %}
 ** Contracts Assignements **
 {% if assignements_table %}
 {% render_table assignements_table %}
-{% endif %}
+{% endif %} {% if perms.netbox_contract.add_contractassignement %}
  Add_assignement
+{% endif %}
+{% endif %}
```

### Comparing `netbox-contract-2.0.2/src/netbox_contract/templates/netbox_contract/contract.html` & `netbox-contract-2.0.3/src/netbox_contract/templates/netbox_contract/contract.html`

 * *Files 3% similar despite different names*

```diff
@@ -107,24 +107,28 @@
         <h5 class="card-header">Assignements</h5>
         <div class="card-body table-responsive">
           {% render_table assignements_table %}
         </div>
       </div>
     </div>
   </div>
+  {% if perms.netbox_contract.view_invoice %}
   <div class="row">
     <div class="col col-md-12">
       <div class="card">
         <h5 class="card-header">Invoices</h5>
         <div class="card-body table-responsive">
           {% render_table invoices_table %}
         </div>
+        {% if perms.netbox_contract.add_invoice %}
         <div class="card-footer text-end noprint">
           <a href="{% url 'plugins:netbox_contract:invoice_add' %}?contracts={{ object.pk }}" class="btn btn-primary btn-sm">
               <i class="mdi mdi-plus-thick" aria-hidden="true"></i>
               Add an invoice
           </a>
-      </div>
+        </div>
+        {% endif %}
       </div>
     </div>
   </div>
+  {% endif %}
 {% endblock content %}
```

#### html2text {}

```diff
@@ -21,11 +21,14 @@
 Documents              Documents
 {% include 'inc/panels/custom_fields.html' %}
 {% include 'inc/panels/tags.html' %} {% include 'inc/panels/comments.html' %}
 ** Circuits **
 {% render_table circuit_table %}
 ** Assignements **
 {% render_table assignements_table %}
+{% if perms.netbox_contract.view_invoice %}
 ** Invoices **
 {% render_table invoices_table %}
+{% if perms.netbox_contract.add_invoice %}
  Add_an_invoice
-{% endblock content %}
+{% endif %}
+{% endif %} {% endblock content %}
```

### Comparing `netbox-contract-2.0.2/src/netbox_contract/templates/netbox_contract/contract_assignement.html` & `netbox-contract-2.0.3/src/netbox_contract/templates/netbox_contract/contract_assignement.html`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.2/src/netbox_contract/templates/netbox_contract/invoice.html` & `netbox-contract-2.0.3/src/netbox_contract/templates/netbox_contract/invoice.html`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.2/src/netbox_contract/templates/netbox_contract/serviceprovider.html` & `netbox-contract-2.0.3/src/netbox_contract/templates/netbox_contract/serviceprovider.html`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.2/src/netbox_contract/urls.py` & `netbox-contract-2.0.3/src/netbox_contract/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.2/src/netbox_contract/views.py` & `netbox-contract-2.0.3/src/netbox_contract/views.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.2/src/netbox_contract.egg-info/PKG-INFO` & `netbox-contract-2.0.3/src/netbox_contract.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-contract
-Version: 2.0.2
+Version: 2.0.3
 Summary: Contract management plugin for Netbox
 Author-email: Marc Lebreuil <marc@famillelebreuil.net>
 Project-URL: Homepage, https://github.com/mlebreuil/netbox-contract
 Project-URL: Bug Tracker, https://github.com/mlebreuil/netbox-contract/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -87,8 +87,13 @@
 
 #### version 2.0.1
 
 Add support contract assignement panel to devices.
 
 #### version 2.0.2
 
-Add support for Netbox 3.5 whcih become the minimum version supported to accoodate the removal of NetBoxModelCSVForm class (replaced by NetBoxModelImportForm) .
+Add support for Netbox 3.5 which become the minimum version supported to accomodate the removal of NetBoxModelCSVForm class (replaced by NetBoxModelImportForm) .
+
+#### version 2.0.3
+
+* [#60](https://github.com/mlebreuil/netbox-contract/issues/60) Update contract quick search to also filter on fields "External reference" and "Comments".
+* [#49](https://github.com/mlebreuil/netbox-contract/issues/49) Manage permissions.
```

### Comparing `netbox-contract-2.0.2/src/netbox_contract.egg-info/SOURCES.txt` & `netbox-contract-2.0.3/src/netbox_contract.egg-info/SOURCES.txt`

 * *Files identical despite different names*

