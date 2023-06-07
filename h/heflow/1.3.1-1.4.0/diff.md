# Comparing `tmp/heflow-1.3.1.tar.gz` & `tmp/heflow-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heflow-1.3.1.tar", last modified: Mon Apr 24 14:57:00 2023, max compression
+gzip compressed data, was "heflow-1.4.0.tar", last modified: Wed Jun  7 11:16:16 2023, max compression
```

## Comparing `heflow-1.3.1.tar` & `heflow-1.4.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:57:00.175976 heflow-1.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:57:00.159975 heflow-1.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:57:00.163976 heflow-1.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-24 14:56:50.000000 heflow-1.3.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-04-24 14:56:50.000000 heflow-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-24 14:56:50.000000 heflow-1.3.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-04-24 14:57:00.175976 heflow-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-04-24 14:56:50.000000 heflow-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:57:00.163976 heflow-1.3.1/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   383186 2023-04-24 14:56:50.000000 heflow-1.3.1/assets/heflow-ppmlops.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:57:00.159975 heflow-1.3.1/charts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:57:00.163976 heflow-1.3.1/charts/heflow/
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-24 14:56:50.000000 heflow-1.3.1/charts/heflow/Chart.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-24 14:56:50.000000 heflow-1.3.1/charts/heflow/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:57:00.163976 heflow-1.3.1/charts/heflow/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-24 14:56:50.000000 heflow-1.3.1/charts/heflow/templates/NOTES.txt
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-24 14:56:50.000000 heflow-1.3.1/charts/heflow/templates/_helpers.tpl
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-24 14:56:50.000000 heflow-1.3.1/charts/heflow/templates/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-24 14:56:50.000000 heflow-1.3.1/charts/heflow/templates/secret.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-24 14:56:50.000000 heflow-1.3.1/charts/heflow/templates/service-account.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-24 14:56:50.000000 heflow-1.3.1/charts/heflow/templates/service.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-04-24 14:56:50.000000 heflow-1.3.1/charts/heflow/values.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-24 14:56:50.000000 heflow-1.3.1/charts/heflow/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:57:00.167976 heflow-1.3.1/docker/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-24 14:56:50.000000 heflow-1.3.1/docker/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-24 14:56:50.000000 heflow-1.3.1/docker/dev.Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:57:00.159975 heflow-1.3.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:57:00.167976 heflow-1.3.1/examples/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-24 14:56:50.000000 heflow-1.3.1/examples/sklearn/MLproject
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-24 14:56:50.000000 heflow-1.3.1/examples/sklearn/python_env.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-24 14:56:50.000000 heflow-1.3.1/examples/sklearn/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:57:00.167976 heflow-1.3.1/heflow/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-24 14:56:50.000000 heflow-1.3.1/heflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:57:00.171976 heflow-1.3.1/heflow/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:56:50.000000 heflow-1.3.1/heflow/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-04-24 14:56:50.000000 heflow-1.3.1/heflow/cli/keygen.py
--rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-04-24 14:56:50.000000 heflow-1.3.1/heflow/codecs.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-24 14:56:50.000000 heflow-1.3.1/heflow/contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-04-24 14:56:50.000000 heflow-1.3.1/heflow/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-04-24 14:56:50.000000 heflow-1.3.1/heflow/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:57:00.171976 heflow-1.3.1/heflow/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:56:50.000000 heflow-1.3.1/heflow/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-24 14:56:50.000000 heflow-1.3.1/heflow/plugins/contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 14:56:50.000000 heflow-1.3.1/heflow/plugins/keys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:57:00.175976 heflow-1.3.1/heflow/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-24 14:56:50.000000 heflow-1.3.1/heflow/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-24 14:56:50.000000 heflow-1.3.1/heflow/sklearn/linear_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:57:00.175976 heflow-1.3.1/heflow/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:56:50.000000 heflow-1.3.1/heflow/tensorflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:57:00.175976 heflow-1.3.1/heflow/tensorflow/keras/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 14:56:50.000000 heflow-1.3.1/heflow/tensorflow/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-24 14:56:50.000000 heflow-1.3.1/heflow/tensorflow/keras/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-04-24 14:56:50.000000 heflow-1.3.1/heflow/tensors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:57:00.175976 heflow-1.3.1/heflow/ui/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-24 14:56:50.000000 heflow-1.3.1/heflow/ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:57:00.171976 heflow-1.3.1/heflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-04-24 14:57:00.000000 heflow-1.3.1/heflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-24 14:57:00.000000 heflow-1.3.1/heflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 14:57:00.000000 heflow-1.3.1/heflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-24 14:57:00.000000 heflow-1.3.1/heflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-24 14:57:00.000000 heflow-1.3.1/heflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 14:57:00.000000 heflow-1.3.1/heflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-24 14:56:50.000000 heflow-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-24 14:56:50.000000 heflow-1.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-24 14:56:50.000000 heflow-1.3.1/runtime.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 14:57:00.175976 heflow-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-04-24 14:56:50.000000 heflow-1.3.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-24 14:56:50.000000 heflow-1.3.1/start
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:16:16.663152 heflow-1.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:16:16.655152 heflow-1.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:16:16.659152 heflow-1.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-07 11:16:07.000000 heflow-1.4.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-06-07 11:16:07.000000 heflow-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-07 11:16:07.000000 heflow-1.4.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-06-07 11:16:16.663152 heflow-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-06-07 11:16:07.000000 heflow-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:16:16.659152 heflow-1.4.0/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   383186 2023-06-07 11:16:07.000000 heflow-1.4.0/assets/heflow-ppmlops.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:16:16.655152 heflow-1.4.0/charts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:16:16.659152 heflow-1.4.0/charts/heflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-07 11:16:07.000000 heflow-1.4.0/charts/heflow/Chart.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-07 11:16:07.000000 heflow-1.4.0/charts/heflow/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:16:16.659152 heflow-1.4.0/charts/heflow/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-07 11:16:07.000000 heflow-1.4.0/charts/heflow/templates/NOTES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-07 11:16:07.000000 heflow-1.4.0/charts/heflow/templates/_helpers.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-07 11:16:07.000000 heflow-1.4.0/charts/heflow/templates/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-07 11:16:07.000000 heflow-1.4.0/charts/heflow/templates/secret.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-07 11:16:07.000000 heflow-1.4.0/charts/heflow/templates/service-account.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-07 11:16:07.000000 heflow-1.4.0/charts/heflow/templates/service.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-07 11:16:07.000000 heflow-1.4.0/charts/heflow/values.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-07 11:16:07.000000 heflow-1.4.0/charts/heflow/values.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:16:16.659152 heflow-1.4.0/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-07 11:16:07.000000 heflow-1.4.0/docker/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-07 11:16:07.000000 heflow-1.4.0/docker/dev.Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:16:16.655152 heflow-1.4.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:16:16.659152 heflow-1.4.0/examples/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-07 11:16:07.000000 heflow-1.4.0/examples/sklearn/MLproject
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-07 11:16:07.000000 heflow-1.4.0/examples/sklearn/python_env.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-07 11:16:07.000000 heflow-1.4.0/examples/sklearn/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:16:16.663152 heflow-1.4.0/heflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-07 11:16:07.000000 heflow-1.4.0/heflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:16:16.663152 heflow-1.4.0/heflow/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 11:16:07.000000 heflow-1.4.0/heflow/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-06-07 11:16:07.000000 heflow-1.4.0/heflow/cli/keygen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-06-07 11:16:07.000000 heflow-1.4.0/heflow/codecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-07 11:16:07.000000 heflow-1.4.0/heflow/contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-06-07 11:16:07.000000 heflow-1.4.0/heflow/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-06-07 11:16:07.000000 heflow-1.4.0/heflow/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:16:16.663152 heflow-1.4.0/heflow/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 11:16:07.000000 heflow-1.4.0/heflow/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-07 11:16:07.000000 heflow-1.4.0/heflow/plugins/contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-07 11:16:07.000000 heflow-1.4.0/heflow/plugins/keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:16:16.663152 heflow-1.4.0/heflow/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-07 11:16:07.000000 heflow-1.4.0/heflow/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-07 11:16:07.000000 heflow-1.4.0/heflow/sklearn/linear_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:16:16.663152 heflow-1.4.0/heflow/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 11:16:07.000000 heflow-1.4.0/heflow/tensorflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:16:16.663152 heflow-1.4.0/heflow/tensorflow/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 11:16:07.000000 heflow-1.4.0/heflow/tensorflow/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-07 11:16:07.000000 heflow-1.4.0/heflow/tensorflow/keras/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-06-07 11:16:07.000000 heflow-1.4.0/heflow/tensors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:16:16.663152 heflow-1.4.0/heflow/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-07 11:16:07.000000 heflow-1.4.0/heflow/ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:16:16.663152 heflow-1.4.0/heflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-06-07 11:16:16.000000 heflow-1.4.0/heflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-07 11:16:16.000000 heflow-1.4.0/heflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 11:16:16.000000 heflow-1.4.0/heflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-07 11:16:16.000000 heflow-1.4.0/heflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-07 11:16:16.000000 heflow-1.4.0/heflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-07 11:16:16.000000 heflow-1.4.0/heflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-07 11:16:07.000000 heflow-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-07 11:16:07.000000 heflow-1.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-07 11:16:07.000000 heflow-1.4.0/runtime.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 11:16:16.663152 heflow-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-07 11:16:07.000000 heflow-1.4.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-07 11:16:07.000000 heflow-1.4.0/start
```

### Comparing `heflow-1.3.1/.github/workflows/release.yml` & `heflow-1.4.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `heflow-1.3.1/LICENSE` & `heflow-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `heflow-1.3.1/PKG-INFO` & `heflow-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heflow
-Version: 1.3.1
+Version: 1.4.0
 Summary: HEflow: A platform for the privacy-preserving machine learning lifecycle
 Home-page: https://github.com/inaccel/heflow
 Author: InAccel
 Author-email: info@inaccel.com
 License: Apache-2.0
 Platform: Linux
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `heflow-1.3.1/README.md` & `heflow-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `heflow-1.3.1/assets/heflow-ppmlops.svg` & `heflow-1.4.0/assets/heflow-ppmlops.svg`

 * *Files identical despite different names*

### Comparing `heflow-1.3.1/charts/heflow/Chart.yaml` & `heflow-1.4.0/charts/heflow/Chart.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -26,8 +26,8 @@
 maintainers:
 - email: info@inaccel.com
   name: InAccel
 name: heflow
 sources:
 - https://github.com/inaccel/heflow
 type: application
-version: 1.0.0
+version: 1.1.0
```

### Comparing `heflow-1.3.1/charts/heflow/README.md` & `heflow-1.4.0/charts/heflow/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -27,21 +27,22 @@
 deletes the release.
 
 ## Parameters
 
 The following table lists the configurable parameters of the HEflow chart and
 their default values.
 
-| Parameter           | Description                                   | Default          |
-| ------------------- | --------------------------------------------- | ---------------- |
-| `heflow.image`      | Container image name.                         | `inaccel/heflow` |
-| `heflow.pullPolicy` | Image pull policy.                            |                  |
-| `heflow.resources`  | Compute resources required by this container. |                  |
-| `heflow.tag`        | Release version.                              | `latest`         |
-| `replicas`          | Number of desired pods.                       |                  |
+| Parameter           | Description                                                                       | Default          |
+| ------------------- | --------------------------------------------------------------------------------- | ---------------- |
+| `heflow.image`      | Container image name.                                                             | `inaccel/heflow` |
+| `heflow.pullPolicy` | Image pull policy.                                                                |                  |
+| `heflow.resources`  | Compute resources required by this container.                                     |                  |
+| `heflow.tag`        | Release version.                                                                  | `latest`         |
+| `nodeSelector`      | Selector which must match a node's labels for a pod to be scheduled on that node. |                  |
+| `replicas`          | Number of desired pods.                                                           |                  |
 
 Specify each parameter using the `--set key=value[,key=value]` argument to
 `helm install`.
 
 Alternatively, a YAML file that specifies the values for the parameters can be
 provided while installing the chart. For example,
```

### Comparing `heflow-1.3.1/charts/heflow/templates/_helpers.tpl` & `heflow-1.4.0/charts/heflow/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `heflow-1.3.1/charts/heflow/templates/deployment.yaml` & `heflow-1.4.0/charts/heflow/templates/deployment.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -63,9 +63,13 @@
         resources:
           {{- $.Values.heflow.resources | toYaml | nindent 10 }}
         {{- end }}
       hostAliases:
       - hostnames:
         - heflow
         ip: 127.0.0.1
+      {{- if $.Values.nodeSelector }}
+      nodeSelector:
+        {{- $.Values.nodeSelector | toYaml | nindent 8 }}
+      {{- end }}
       priorityClassName: system-cluster-critical
       serviceAccountName: {{ $.Release.Name }}
```

### Comparing `heflow-1.3.1/charts/heflow/templates/secret.yaml` & `heflow-1.4.0/charts/heflow/templates/secret.yaml`

 * *Files identical despite different names*

### Comparing `heflow-1.3.1/charts/heflow/values.schema.json` & `heflow-1.4.0/charts/heflow/values.schema.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9722222222222222%*

 * *Differences: {"'properties'": '{\'nodeSelector\': OrderedDict([(\'description\', "Selector which must match a '*

 * *                 'node\'s labels for a pod to be scheduled on that node."), (\'title\', '*

 * *                 "'nodeSelector'), ('type', 'object')])}"}*

```diff
@@ -37,14 +37,19 @@
             "required": [
                 "image",
                 "tag"
             ],
             "title": "heflow",
             "type": "object"
         },
+        "nodeSelector": {
+            "description": "Selector which must match a node's labels for a pod to be scheduled on that node.",
+            "title": "nodeSelector",
+            "type": "object"
+        },
         "replicas": {
             "description": "Number of desired pods.",
             "exclusiveMinimum": 0,
             "form": true,
             "multipleOf": 1,
             "title": "replicas",
             "type": "integer"
```

### Comparing `heflow-1.3.1/examples/sklearn/train.py` & `heflow-1.4.0/examples/sklearn/train.py`

 * *Files identical despite different names*

### Comparing `heflow-1.3.1/heflow/cli/keygen.py` & `heflow-1.4.0/heflow/cli/keygen.py`

 * *Files identical despite different names*

### Comparing `heflow-1.3.1/heflow/codecs.py` & `heflow-1.4.0/heflow/codecs.py`

 * *Files identical despite different names*

### Comparing `heflow-1.3.1/heflow/contexts.py` & `heflow-1.4.0/heflow/contexts.py`

 * *Files identical despite different names*

### Comparing `heflow-1.3.1/heflow/keys.py` & `heflow-1.4.0/heflow/keys.py`

 * *Files identical despite different names*

### Comparing `heflow-1.3.1/heflow/models.py` & `heflow-1.4.0/heflow/models.py`

 * *Files identical despite different names*

### Comparing `heflow-1.3.1/heflow/sklearn/__init__.py` & `heflow-1.4.0/heflow/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `heflow-1.3.1/heflow/sklearn/linear_model.py` & `heflow-1.4.0/heflow/sklearn/linear_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
     def he_decision_function(self, he_X):
         he_scores = he_X.dot_(self.he_coef_).add_(self.he_intercept_)
         return he_scores.reshape_(
             (he_scores.shape[0], )) if he_scores.shape[1] == 1 else he_scores
 
     def predict(self, X):
-        he_X = heflow.ckks_tensor(X)
+        he_X = heflow.as_ckks_tensor(X)
         he_scores = self.he_decision_function(he_X)
         scores = he_scores.numpy()
         if len(scores.shape) == 1:
             indices = (scores > 0).astype(int)
         else:
             indices = numpy.argmax(scores, axis=1)
         return numpy.take(self.classes_, indices, axis=0)
```

### Comparing `heflow-1.3.1/heflow/tensors.py` & `heflow-1.4.0/heflow/tensors.py`

 * *Files 3% similar despite different names*

```diff
@@ -157,9 +157,25 @@
         return CKKSTensor(self.backend.transpose())
 
     def transpose_(self):
         self.backend.transpose_()
         return self
 
 
+@functools.singledispatch
+def as_ckks_tensor(data):
+    return CKKSTensor(data)
+
+
+@as_ckks_tensor.register
+def _(tensor: CKKSTensor):
+    return tensor
+
+
+@functools.singledispatch
 def ckks_tensor(data):
     return CKKSTensor(data)
+
+
+@ckks_tensor.register
+def _(tensor: CKKSTensor):
+    return tensor.clone()
```

### Comparing `heflow-1.3.1/heflow.egg-info/PKG-INFO` & `heflow-1.4.0/heflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heflow
-Version: 1.3.1
+Version: 1.4.0
 Summary: HEflow: A platform for the privacy-preserving machine learning lifecycle
 Home-page: https://github.com/inaccel/heflow
 Author: InAccel
 Author-email: info@inaccel.com
 License: Apache-2.0
 Platform: Linux
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `heflow-1.3.1/heflow.egg-info/SOURCES.txt` & `heflow-1.4.0/heflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heflow-1.3.1/setup.py` & `heflow-1.4.0/setup.py`

 * *Files identical despite different names*

