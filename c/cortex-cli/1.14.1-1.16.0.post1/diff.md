# Comparing `tmp/cortex_cli-1.14.1.tar.gz` & `tmp/cortex_cli-1.16.0.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cortex_cli-1.14.1.tar", last modified: Mon May 22 18:22:55 2023, max compression
+gzip compressed data, was "cortex_cli-1.16.0.post1.tar", last modified: Wed Jun  7 16:13:38 2023, max compression
```

## Comparing `cortex_cli-1.14.1.tar` & `cortex_cli-1.16.0.post1.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-22 18:22:55.374894 cortex_cli-1.14.1/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      260 2023-05-22 18:22:55.374894 cortex_cli-1.14.1/PKG-INFO
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     5733 2023-05-15 20:17:46.000000 cortex_cli-1.14.1/README.md
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-22 18:22:55.364894 cortex_cli-1.14.1/cortex_cli/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       22 2023-05-19 19:10:27.000000 cortex_cli-1.14.1/cortex_cli/__init__.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-22 18:22:55.364894 cortex_cli-1.14.1/cortex_cli/cli/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 23:15:18.000000 cortex_cli-1.14.1/cortex_cli/cli/__init__.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-22 18:22:55.364894 cortex_cli-1.14.1/cortex_cli/cli/api/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.14.1/cortex_cli/cli/api/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3992 2023-05-02 16:03:43.000000 cortex_cli-1.14.1/cortex_cli/cli/api/github_api.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      575 2023-03-09 15:57:05.000000 cortex_cli-1.14.1/cortex_cli/cli/api/http_api.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2789 2023-03-16 20:39:49.000000 cortex_cli-1.14.1/cortex_cli/cli/cli_api_base.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2792 2023-03-16 20:39:49.000000 cortex_cli-1.14.1/cortex_cli/cli/cli_api_base_config.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3782 2023-05-15 21:55:08.000000 cortex_cli-1.14.1/cortex_cli/cli/cli_multipart_upload.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       90 2023-03-09 15:57:05.000000 cortex_cli-1.14.1/cortex_cli/cli/clients.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2027 2023-05-02 16:03:43.000000 cortex_cli-1.14.1/cortex_cli/cli/configure.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      973 2023-05-15 20:17:46.000000 cortex_cli-1.14.1/cortex_cli/cli/cortex_cli.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      994 2023-03-16 20:39:49.000000 cortex_cli-1.14.1/cortex_cli/cli/generic_get.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1005 2023-03-09 15:57:05.000000 cortex_cli-1.14.1/cortex_cli/cli/inferences.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    24630 2023-05-22 18:21:42.000000 cortex_cli-1.14.1/cortex_cli/cli/models.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3259 2023-05-15 20:17:46.000000 cortex_cli-1.14.1/cortex_cli/cli/pipelines.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-22 18:22:55.364894 cortex_cli-1.14.1/cortex_cli/core/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.14.1/cortex_cli/core/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     4182 2023-04-17 18:14:34.000000 cortex_cli-1.14.1/cortex_cli/core/cortex_data.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3648 2023-03-09 15:57:05.000000 cortex_cli-1.14.1/cortex_cli/core/drift_checks.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    11022 2023-04-17 18:14:34.000000 cortex_cli-1.14.1/cortex_cli/core/ethics_checks.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-22 18:22:55.364894 cortex_cli-1.14.1/cortex_cli/core/mlflow/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.14.1/cortex_cli/core/mlflow/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    13976 2023-03-09 15:57:05.000000 cortex_cli-1.14.1/cortex_cli/core/mlflow/mlflow_cortex.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-22 18:22:55.364894 cortex_cli-1.14.1/cortex_cli/core/models/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.14.1/cortex_cli/core/models/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     8121 2023-04-20 17:50:53.000000 cortex_cli-1.14.1/cortex_cli/core/models/cortex_model.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2828 2023-04-25 18:48:24.000000 cortex_cli-1.14.1/cortex_cli/core/secrets_manager.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-22 18:22:55.364894 cortex_cli-1.14.1/cortex_cli/model_templates/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.14.1/cortex_cli/model_templates/__init__.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-22 18:22:55.364894 cortex_cli-1.14.1/cortex_cli/model_templates/chatgpt_model/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2399 2023-04-25 18:48:24.000000 cortex_cli-1.14.1/cortex_cli/model_templates/chatgpt_model/.gitignore
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      972 2023-04-25 18:48:24.000000 cortex_cli-1.14.1/cortex_cli/model_templates/chatgpt_model/README.md
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.14.1/cortex_cli/model_templates/chatgpt_model/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      301 2023-04-25 18:48:24.000000 cortex_cli-1.14.1/cortex_cli/model_templates/chatgpt_model/cookiecutter.json
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       12 2023-04-25 18:48:24.000000 cortex_cli-1.14.1/cortex_cli/model_templates/chatgpt_model/requirements.txt
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-22 18:22:55.374894 cortex_cli-1.14.1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2330 2023-04-25 18:48:24.000000 cortex_cli-1.14.1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/.gitignore
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1645 2023-05-02 16:03:43.000000 cortex_cli-1.14.1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/README.md
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      162 2023-04-25 18:48:24.000000 cortex_cli-1.14.1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/conda.yml
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      322 2023-05-05 19:39:27.000000 cortex_cli-1.14.1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/cortex.yml
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-22 18:22:55.374894 cortex_cli-1.14.1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/data/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.14.1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/data/.gitkeep
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-22 18:22:55.374894 cortex_cli-1.14.1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/notebooks/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.14.1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/notebooks/.gitkeep
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-22 18:22:55.364894 cortex_cli-1.14.1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-22 18:22:55.374894 cortex_cli-1.14.1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.14.1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1654 2023-04-25 18:48:24.000000 cortex_cli-1.14.1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-22 18:22:55.374894 cortex_cli-1.14.1/cortex_cli/model_templates/digits_model/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2399 2023-04-25 18:48:24.000000 cortex_cli-1.14.1/cortex_cli/model_templates/digits_model/.gitignore
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      972 2023-04-25 18:48:24.000000 cortex_cli-1.14.1/cortex_cli/model_templates/digits_model/README.md
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.14.1/cortex_cli/model_templates/digits_model/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      301 2023-04-25 18:48:24.000000 cortex_cli-1.14.1/cortex_cli/model_templates/digits_model/cookiecutter.json
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       12 2023-04-25 18:48:24.000000 cortex_cli-1.14.1/cortex_cli/model_templates/digits_model/requirements.txt
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-22 18:22:55.374894 cortex_cli-1.14.1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2330 2023-04-25 18:48:24.000000 cortex_cli-1.14.1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/.gitignore
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1645 2023-05-02 16:03:43.000000 cortex_cli-1.14.1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/README.md
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      162 2023-04-25 18:48:24.000000 cortex_cli-1.14.1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/conda.yml
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      455 2023-05-05 19:39:27.000000 cortex_cli-1.14.1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/cortex.yml
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-22 18:22:55.374894 cortex_cli-1.14.1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/data/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.14.1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/data/.gitkeep
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-22 18:22:55.374894 cortex_cli-1.14.1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/notebooks/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.14.1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/notebooks/.gitkeep
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-22 18:22:55.364894 cortex_cli-1.14.1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-22 18:22:55.374894 cortex_cli-1.14.1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.14.1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2377 2023-04-25 18:48:24.000000 cortex_cli-1.14.1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-22 18:22:55.374894 cortex_cli-1.14.1/cortex_cli/tests/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.14.1/cortex_cli/tests/__init__.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1801 2023-03-09 15:57:05.000000 cortex_cli-1.14.1/cortex_cli/tests/test_cortex_data.py
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1825 2023-03-09 15:57:05.000000 cortex_cli-1.14.1/cortex_cli/tests/test_ethics_checks.py
-drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-05-22 18:22:55.364894 cortex_cli-1.14.1/cortex_cli.egg-info/
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      260 2023-05-22 18:22:55.000000 cortex_cli-1.14.1/cortex_cli.egg-info/PKG-INFO
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3162 2023-05-22 18:22:55.000000 cortex_cli-1.14.1/cortex_cli.egg-info/SOURCES.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        1 2023-05-22 18:22:55.000000 cortex_cli-1.14.1/cortex_cli.egg-info/dependency_links.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       62 2023-05-22 18:22:55.000000 cortex_cli-1.14.1/cortex_cli.egg-info/entry_points.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      110 2023-05-22 18:22:55.000000 cortex_cli-1.14.1/cortex_cli.egg-info/requires.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       11 2023-05-22 18:22:55.000000 cortex_cli-1.14.1/cortex_cli.egg-info/top_level.txt
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       89 2023-03-01 03:50:43.000000 cortex_cli-1.14.1/pyproject.toml
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      228 2023-05-22 18:22:55.374894 cortex_cli-1.14.1/setup.cfg
--rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1076 2023-04-25 18:48:24.000000 cortex_cli-1.14.1/setup.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-07 16:13:38.253787 cortex_cli-1.16.0.post1/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      266 2023-06-07 16:13:38.253787 cortex_cli-1.16.0.post1/PKG-INFO
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     5733 2023-05-15 20:17:46.000000 cortex_cli-1.16.0.post1/README.md
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-07 16:13:38.243787 cortex_cli-1.16.0.post1/cortex_cli/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       25 2023-06-06 19:56:18.000000 cortex_cli-1.16.0.post1/cortex_cli/__init__.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-07 16:13:38.243787 cortex_cli-1.16.0.post1/cortex_cli/cli/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 23:15:18.000000 cortex_cli-1.16.0.post1/cortex_cli/cli/__init__.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-07 16:13:38.243787 cortex_cli-1.16.0.post1/cortex_cli/cli/api/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.16.0.post1/cortex_cli/cli/api/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3992 2023-05-02 16:03:43.000000 cortex_cli-1.16.0.post1/cortex_cli/cli/api/github_api.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      575 2023-03-09 15:57:05.000000 cortex_cli-1.16.0.post1/cortex_cli/cli/api/http_api.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2789 2023-03-16 20:39:49.000000 cortex_cli-1.16.0.post1/cortex_cli/cli/cli_api_base.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2792 2023-03-16 20:39:49.000000 cortex_cli-1.16.0.post1/cortex_cli/cli/cli_api_base_config.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3782 2023-05-31 17:19:24.000000 cortex_cli-1.16.0.post1/cortex_cli/cli/cli_multipart_upload.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       90 2023-03-09 15:57:05.000000 cortex_cli-1.16.0.post1/cortex_cli/cli/clients.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2027 2023-05-02 16:03:43.000000 cortex_cli-1.16.0.post1/cortex_cli/cli/configure.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      973 2023-05-15 20:17:46.000000 cortex_cli-1.16.0.post1/cortex_cli/cli/cortex_cli.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      994 2023-03-16 20:39:49.000000 cortex_cli-1.16.0.post1/cortex_cli/cli/generic_get.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1005 2023-03-09 15:57:05.000000 cortex_cli-1.16.0.post1/cortex_cli/cli/inferences.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    24745 2023-06-06 19:55:06.000000 cortex_cli-1.16.0.post1/cortex_cli/cli/models.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3259 2023-05-15 20:17:46.000000 cortex_cli-1.16.0.post1/cortex_cli/cli/pipelines.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-07 16:13:38.243787 cortex_cli-1.16.0.post1/cortex_cli/core/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.16.0.post1/cortex_cli/core/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     4817 2023-06-06 19:50:26.000000 cortex_cli-1.16.0.post1/cortex_cli/core/cortex_data.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3648 2023-03-09 15:57:05.000000 cortex_cli-1.16.0.post1/cortex_cli/core/drift_checks.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    11022 2023-04-17 18:14:34.000000 cortex_cli-1.16.0.post1/cortex_cli/core/ethics_checks.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-07 16:13:38.243787 cortex_cli-1.16.0.post1/cortex_cli/core/mlflow/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.16.0.post1/cortex_cli/core/mlflow/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)    13976 2023-03-09 15:57:05.000000 cortex_cli-1.16.0.post1/cortex_cli/core/mlflow/mlflow_cortex.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-07 16:13:38.243787 cortex_cli-1.16.0.post1/cortex_cli/core/models/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.16.0.post1/cortex_cli/core/models/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     8121 2023-04-20 17:50:53.000000 cortex_cli-1.16.0.post1/cortex_cli/core/models/cortex_model.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2828 2023-04-25 18:48:24.000000 cortex_cli-1.16.0.post1/cortex_cli/core/secrets_manager.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-07 16:13:38.243787 cortex_cli-1.16.0.post1/cortex_cli/model_templates/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.16.0.post1/cortex_cli/model_templates/__init__.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-07 16:13:38.243787 cortex_cli-1.16.0.post1/cortex_cli/model_templates/chatgpt_model/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2399 2023-04-25 18:48:24.000000 cortex_cli-1.16.0.post1/cortex_cli/model_templates/chatgpt_model/.gitignore
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      972 2023-04-25 18:48:24.000000 cortex_cli-1.16.0.post1/cortex_cli/model_templates/chatgpt_model/README.md
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.16.0.post1/cortex_cli/model_templates/chatgpt_model/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      301 2023-04-25 18:48:24.000000 cortex_cli-1.16.0.post1/cortex_cli/model_templates/chatgpt_model/cookiecutter.json
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       12 2023-04-25 18:48:24.000000 cortex_cli-1.16.0.post1/cortex_cli/model_templates/chatgpt_model/requirements.txt
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-07 16:13:38.243787 cortex_cli-1.16.0.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2330 2023-04-25 18:48:24.000000 cortex_cli-1.16.0.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/.gitignore
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1645 2023-05-02 16:03:43.000000 cortex_cli-1.16.0.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/README.md
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      162 2023-04-25 18:48:24.000000 cortex_cli-1.16.0.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/conda.yml
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      322 2023-05-05 19:39:27.000000 cortex_cli-1.16.0.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/cortex.yml
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-07 16:13:38.243787 cortex_cli-1.16.0.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/data/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.16.0.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/data/.gitkeep
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-07 16:13:38.243787 cortex_cli-1.16.0.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/notebooks/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.16.0.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/notebooks/.gitkeep
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-07 16:13:38.243787 cortex_cli-1.16.0.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-07 16:13:38.243787 cortex_cli-1.16.0.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.16.0.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1654 2023-04-25 18:48:24.000000 cortex_cli-1.16.0.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-07 16:13:38.243787 cortex_cli-1.16.0.post1/cortex_cli/model_templates/digits_model/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2399 2023-04-25 18:48:24.000000 cortex_cli-1.16.0.post1/cortex_cli/model_templates/digits_model/.gitignore
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      972 2023-04-25 18:48:24.000000 cortex_cli-1.16.0.post1/cortex_cli/model_templates/digits_model/README.md
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.16.0.post1/cortex_cli/model_templates/digits_model/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      301 2023-04-25 18:48:24.000000 cortex_cli-1.16.0.post1/cortex_cli/model_templates/digits_model/cookiecutter.json
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       12 2023-04-25 18:48:24.000000 cortex_cli-1.16.0.post1/cortex_cli/model_templates/digits_model/requirements.txt
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-07 16:13:38.253787 cortex_cli-1.16.0.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2330 2023-04-25 18:48:24.000000 cortex_cli-1.16.0.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/.gitignore
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1645 2023-05-02 16:03:43.000000 cortex_cli-1.16.0.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/README.md
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      162 2023-04-25 18:48:24.000000 cortex_cli-1.16.0.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/conda.yml
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      455 2023-05-05 19:39:27.000000 cortex_cli-1.16.0.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/cortex.yml
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-07 16:13:38.253787 cortex_cli-1.16.0.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/data/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.16.0.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/data/.gitkeep
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-07 16:13:38.253787 cortex_cli-1.16.0.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/notebooks/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.16.0.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/notebooks/.gitkeep
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-07 16:13:38.243787 cortex_cli-1.16.0.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-07 16:13:38.253787 cortex_cli-1.16.0.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-04-25 18:48:24.000000 cortex_cli-1.16.0.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     2377 2023-04-25 18:48:24.000000 cortex_cli-1.16.0.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-07 16:13:38.253787 cortex_cli-1.16.0.post1/cortex_cli/tests/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        0 2023-03-09 15:57:05.000000 cortex_cli-1.16.0.post1/cortex_cli/tests/__init__.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1801 2023-03-09 15:57:05.000000 cortex_cli-1.16.0.post1/cortex_cli/tests/test_cortex_data.py
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1825 2023-03-09 15:57:05.000000 cortex_cli-1.16.0.post1/cortex_cli/tests/test_ethics_checks.py
+drwxr-xr-x   0 mattgroho  (1000) mattgroho  (1000)        0 2023-06-07 16:13:38.243787 cortex_cli-1.16.0.post1/cortex_cli.egg-info/
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      266 2023-06-07 16:13:38.000000 cortex_cli-1.16.0.post1/cortex_cli.egg-info/PKG-INFO
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     3162 2023-06-07 16:13:38.000000 cortex_cli-1.16.0.post1/cortex_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)        1 2023-06-07 16:13:38.000000 cortex_cli-1.16.0.post1/cortex_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       62 2023-06-07 16:13:38.000000 cortex_cli-1.16.0.post1/cortex_cli.egg-info/entry_points.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      110 2023-06-07 16:13:38.000000 cortex_cli-1.16.0.post1/cortex_cli.egg-info/requires.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       11 2023-06-07 16:13:38.000000 cortex_cli-1.16.0.post1/cortex_cli.egg-info/top_level.txt
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)       89 2023-03-01 03:50:43.000000 cortex_cli-1.16.0.post1/pyproject.toml
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)      228 2023-06-07 16:13:38.253787 cortex_cli-1.16.0.post1/setup.cfg
+-rw-r--r--   0 mattgroho  (1000) mattgroho  (1000)     1076 2023-04-25 18:48:24.000000 cortex_cli-1.16.0.post1/setup.py
```

### Comparing `cortex_cli-1.14.1/README.md` & `cortex_cli-1.16.0.post1/README.md`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.14.1/cortex_cli/cli/api/github_api.py` & `cortex_cli-1.16.0.post1/cortex_cli/cli/api/github_api.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.14.1/cortex_cli/cli/api/http_api.py` & `cortex_cli-1.16.0.post1/cortex_cli/cli/api/http_api.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.14.1/cortex_cli/cli/cli_api_base.py` & `cortex_cli-1.16.0.post1/cortex_cli/cli/cli_api_base.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.14.1/cortex_cli/cli/cli_api_base_config.py` & `cortex_cli-1.16.0.post1/cortex_cli/cli/cli_api_base_config.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.14.1/cortex_cli/cli/cli_multipart_upload.py` & `cortex_cli-1.16.0.post1/cortex_cli/cli/cli_multipart_upload.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.14.1/cortex_cli/cli/configure.py` & `cortex_cli-1.16.0.post1/cortex_cli/cli/configure.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.14.1/cortex_cli/cli/cortex_cli.py` & `cortex_cli-1.16.0.post1/cortex_cli/cli/cortex_cli.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.14.1/cortex_cli/cli/generic_get.py` & `cortex_cli-1.16.0.post1/cortex_cli/cli/generic_get.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.14.1/cortex_cli/cli/inferences.py` & `cortex_cli-1.16.0.post1/cortex_cli/cli/inferences.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.14.1/cortex_cli/cli/models.py` & `cortex_cli-1.16.0.post1/cortex_cli/cli/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -342,17 +342,14 @@
         try:
             self._model_json = self._get_model()
             # Step 1 - Get live model data
             if self._tracking:
                 self._mlflow_client = self._setup_mlflow()
                 self._setup_pipeline()
 
-            # Step 2 - Load the Model Class
-            self.model = self._instantiate_model()
-
             # Step 3 - Initialize the pipeline steps
             self._initialize_steps()
 
             # Step 4 - Run the pipeline
             if self._tracking:
                 self._pipeline_json = self._run_pipeline()
 
@@ -379,22 +376,29 @@
             else:
                 self._pass('Completed Cortex Pipeline Run')
 
 # -------------------------------------------------------------------------------
 
     def _initialize_steps(self):
         # Convert yaml steps to ml-api format
-        _steps = []
+        _steps = [
+            {
+                'name':   'Initialize model class',
+                'type':   '_initialize_model',
+                'config': {}
+            },
+            {
+                'name':   'Download model data',
+                'type':   'download_data',
+                'config': {}
+            }
+        ]
 
         # Add default download data step
-        _steps.append({
-            'name':   'Download data',
-            'type':   'download_data',
-            'config': {}
-        })
+        _steps.append()
 
         for step in self._pipeline_steps:
             _steps.append({
                 'name':   step.name,
                 'type':   step.type,
                 'config': {}
             })
@@ -740,13 +744,13 @@
         # LOAD MODEL MODULE
         model_module = self._load_module(
             '{}/{}.py'.format(self._config['module_path'], self._config['model_module']),
             self._config['model_module']
         )
 
         model_params = dict(ChainMap(*self._config['params'])) if self._config['params'] else {}
-        return getattr(model_module, self._config['model_class'])(model_params, self._model_id, self._api_url, self._headers)
+        self.model = getattr(model_module, self._config['model_class'])(model_params, self._model_id, self._api_url, self._headers)
 
 
     def _setup_mlflow(self):
         # Create a client to make API calls to the tracking server
         return mlflow.tracking.MlflowClient()
```

### Comparing `cortex_cli-1.14.1/cortex_cli/cli/pipelines.py` & `cortex_cli-1.16.0.post1/cortex_cli/cli/pipelines.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.14.1/cortex_cli/core/cortex_data.py` & `cortex_cli-1.16.0.post1/cortex_cli/core/cortex_data.py`

 * *Files 15% similar despite different names*

```diff
@@ -35,23 +35,37 @@
 
 
     @property
     def isPandasLoadable(self):
         return self.type in ['xls', 'xlsx', 'xlsm', 'xlsb', 'odf', 'ods', 'odt', 'csv']
 
 
-    def load(self):
+    def load(self, as_polars=False):
+        if as_polars:
+            try:
+                import polars as pl
+            except ImportError:
+                raise Exception('Polars library is not installed. Please install it using "pip install polars"')
         try:
             with open(self.local_path, 'rb') as file:
                 if self.type in ['xls', 'xlsx', 'xlsm', 'xlsb', 'odf', 'ods', 'odt']:
-                    self._loaded_data = pd.read_excel(file)
+                    if as_polars:
+                        self._loaded_data = pl.read_excel(file)
+                    else:
+                        self._loaded_data = pd.read_excel(file)
                 if self.type=='csv':
-                    self._loaded_data = pd.read_csv(file)
+                    if as_polars:
+                        self._loaded_data = pl.read_csv(file)
+                    else:
+                        self._loaded_data = pd.read_csv(file)
                 if self.type=='parquet':
-                    self._loaded_data = pd.read_parquet(file)
+                    if as_polars:
+                        self._loaded_data = pl.read_parquet(file)
+                    else:
+                        self._loaded_data = pd.read_parquet(file)
                 if self.type=='pkl':
                     self._loaded_data = pickle.load(file)
                 if self.type=='json':
                     self._loaded_data = json.load(file)
                 if self.type=='yml':
                     self._loaded_data = yaml.load(file)
                 return self._loaded_data
```

### Comparing `cortex_cli-1.14.1/cortex_cli/core/drift_checks.py` & `cortex_cli-1.16.0.post1/cortex_cli/core/drift_checks.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.14.1/cortex_cli/core/ethics_checks.py` & `cortex_cli-1.16.0.post1/cortex_cli/core/ethics_checks.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.14.1/cortex_cli/core/mlflow/mlflow_cortex.py` & `cortex_cli-1.16.0.post1/cortex_cli/core/mlflow/mlflow_cortex.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.14.1/cortex_cli/core/models/cortex_model.py` & `cortex_cli-1.16.0.post1/cortex_cli/core/models/cortex_model.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.14.1/cortex_cli/core/secrets_manager.py` & `cortex_cli-1.16.0.post1/cortex_cli/core/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.14.1/cortex_cli/model_templates/chatgpt_model/.gitignore` & `cortex_cli-1.16.0.post1/cortex_cli/model_templates/chatgpt_model/.gitignore`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.14.1/cortex_cli/model_templates/chatgpt_model/README.md` & `cortex_cli-1.16.0.post1/cortex_cli/model_templates/chatgpt_model/README.md`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.14.1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/.gitignore` & `cortex_cli-1.16.0.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/.gitignore`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.14.1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/README.md` & `cortex_cli-1.16.0.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/README.md`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.14.1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py` & `cortex_cli-1.16.0.post1/cortex_cli/model_templates/chatgpt_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.14.1/cortex_cli/model_templates/digits_model/.gitignore` & `cortex_cli-1.16.0.post1/cortex_cli/model_templates/digits_model/.gitignore`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.14.1/cortex_cli/model_templates/digits_model/README.md` & `cortex_cli-1.16.0.post1/cortex_cli/model_templates/digits_model/README.md`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.14.1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/.gitignore` & `cortex_cli-1.16.0.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/.gitignore`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.14.1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/README.md` & `cortex_cli-1.16.0.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/README.md`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.14.1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py` & `cortex_cli-1.16.0.post1/cortex_cli/model_templates/digits_model/{{cookiecutter.model_repo}}/src/{{cookiecutter.__model_name}}/{{cookiecutter.__model_name}}.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.14.1/cortex_cli/tests/test_cortex_data.py` & `cortex_cli-1.16.0.post1/cortex_cli/tests/test_cortex_data.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.14.1/cortex_cli/tests/test_ethics_checks.py` & `cortex_cli-1.16.0.post1/cortex_cli/tests/test_ethics_checks.py`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.14.1/cortex_cli.egg-info/SOURCES.txt` & `cortex_cli-1.16.0.post1/cortex_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cortex_cli-1.14.1/setup.py` & `cortex_cli-1.16.0.post1/setup.py`

 * *Files identical despite different names*

