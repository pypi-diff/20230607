# Comparing `tmp/dbt_coves-1.5.1.tar.gz` & `tmp/dbt_coves-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_coves-1.5.1.tar", max compression
+gzip compressed data, was "dbt_coves-1.5.2.tar", max compression
```

## Comparing `dbt_coves-1.5.1.tar` & `dbt_coves-1.5.2.tar`

### file list

```diff
@@ -1,59 +1,58 @@
--rw-r--r--   0        0        0    11357 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/LICENSE
--rw-r--r--   0        0        0    21746 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/README.md
--rw-r--r--   0        0        0       22 2023-05-19 17:40:19.080273 dbt_coves-1.5.1/dbt_coves/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/config/__init__.py
--rw-r--r--   0        0        0     9689 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/config/config.py
--rw-r--r--   0        0        0        0 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/core/__init__.py
--rw-r--r--   0        0        0      650 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/core/exceptions.py
--rw-r--r--   0        0        0     8193 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/core/main.py
--rw-r--r--   0        0        0        0 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/__init__.py
--rw-r--r--   0        0        0     3008 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/base.py
--rw-r--r--   0        0        0     5056 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/dbt/main.py
--rw-r--r--   0        0        0        0 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/extract/__init__.py
--rw-r--r--   0        0        0    12365 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/extract/airbyte.py
--rw-r--r--   0        0        0      475 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/extract/base.py
--rw-r--r--   0        0        0     4574 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/extract/fivetran.py
--rw-r--r--   0        0        0      963 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/extract/main.py
--rw-r--r--   0        0        0        0 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/generate/__init__.py
--rw-r--r--   0        0        0    18472 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/generate/base.py
--rw-r--r--   0        0        0     1520 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/generate/main.py
--rw-r--r--   0        0        0    10624 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/generate/metadata.py
--rw-r--r--   0        0        0     8942 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/generate/properties.py
--rw-r--r--   0        0        0    14017 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/generate/sources.py
--rw-r--r--   0        0        0     2715 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/generate/templates.py
--rw-r--r--   0        0        0        0 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/load/__init__.py
--rw-r--r--   0        0        0    25744 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/load/airbyte.py
--rw-r--r--   0        0        0     2259 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/load/base.py
--rw-r--r--   0        0        0    18452 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/load/fivetran.py
--rw-r--r--   0        0        0      946 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/load/main.py
--rw-r--r--   0        0        0        0 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/setup/__init__.py
--rw-r--r--   0        0        0     2004 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/setup/all.py
--rw-r--r--   0        0        0      494 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/setup/base.py
--rw-r--r--   0        0        0     4287 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/setup/dbt.py
--rw-r--r--   0        0        0     6751 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/setup/git.py
--rw-r--r--   0        0        0     1266 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/setup/main.py
--rw-r--r--   0        0        0     1664 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/setup/pre_commit.py
--rw-r--r--   0        0        0    10262 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/setup/ssh.py
--rw-r--r--   0        0        0      845 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/setup/templates/pre_commit/copier.yml
--rw-r--r--   0        0        0     2110 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/setup/templates/pre_commit/{% if use_sqlfluff or use_yamllint or use_dbt_checkpoint %}pre-commit-config.yaml{% endif %}.jinja
--rw-r--r--   0        0        0       75 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_sqlfluff %}.sqlfluffignore{% endif %}
--rw-r--r--   0        0        0     2743 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_sqlfluff %}.sqlfluff{% endif %}.jinja
--rw-r--r--   0        0        0      668 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_yamllint %}.yamllint{% endif %}
--rw-r--r--   0        0        0      102 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{{ _copier_conf.answers_file }}-precommit.yaml.jinja
--rw-r--r--   0        0        0     1371 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/tasks/setup/utils.py
--rw-r--r--   0        0        0      255 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/templates/model_props.yml
--rw-r--r--   0        0        0      214 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/templates/source_props.yml
--rw-r--r--   0        0        0     1201 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/templates/staging_model.sql
--rw-r--r--   0        0        0      495 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/templates/staging_model_props.yml
--rw-r--r--   0        0        0        0 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/ui/__init__.py
--rw-r--r--   0        0        0     1202 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/ui/traceback.py
--rw-r--r--   0        0        0        0 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/utils/__init__.py
--rw-r--r--   0        0        0    11270 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/utils/api_caller.py
--rw-r--r--   0        0        0    14725 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/utils/flags.py
--rw-r--r--   0        0        0     1132 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/utils/jinja.py
--rw-r--r--   0        0        0      785 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/utils/log.py
--rw-r--r--   0        0        0      791 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/utils/shell.py
--rw-r--r--   0        0        0     1765 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/utils/tracking.py
--rw-r--r--   0        0        0     1010 2023-05-19 17:39:36.411845 dbt_coves-1.5.1/dbt_coves/utils/yaml.py
--rw-r--r--   0        0        0     3606 2023-05-19 17:40:19.076274 dbt_coves-1.5.1/pyproject.toml
--rw-r--r--   0        0        0    23695 1970-01-01 00:00:00.000000 dbt_coves-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/LICENSE
+-rw-r--r--   0        0        0    22554 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/README.md
+-rw-r--r--   0        0        0       22 2023-06-07 19:29:31.316032 dbt_coves-1.5.2/dbt_coves/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/config/__init__.py
+-rw-r--r--   0        0        0     9769 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/config/config.py
+-rw-r--r--   0        0        0        0 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/core/__init__.py
+-rw-r--r--   0        0        0      650 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/core/exceptions.py
+-rw-r--r--   0        0        0     8193 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/core/main.py
+-rw-r--r--   0        0        0        0 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/tasks/__init__.py
+-rw-r--r--   0        0        0     3008 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/tasks/base.py
+-rw-r--r--   0        0        0     5056 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/tasks/dbt/main.py
+-rw-r--r--   0        0        0        0 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/tasks/extract/__init__.py
+-rw-r--r--   0        0        0    12365 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/tasks/extract/airbyte.py
+-rw-r--r--   0        0        0      475 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/tasks/extract/base.py
+-rw-r--r--   0        0        0     4574 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/tasks/extract/fivetran.py
+-rw-r--r--   0        0        0      963 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/tasks/extract/main.py
+-rw-r--r--   0        0        0        0 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/tasks/generate/__init__.py
+-rw-r--r--   0        0        0    18472 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/tasks/generate/base.py
+-rw-r--r--   0        0        0     1329 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/tasks/generate/main.py
+-rw-r--r--   0        0        0    10624 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/tasks/generate/metadata.py
+-rw-r--r--   0        0        0     8942 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/tasks/generate/properties.py
+-rw-r--r--   0        0        0    15026 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/tasks/generate/sources.py
+-rw-r--r--   0        0        0     2715 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/tasks/generate/templates.py
+-rw-r--r--   0        0        0        0 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/tasks/load/__init__.py
+-rw-r--r--   0        0        0    25744 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/tasks/load/airbyte.py
+-rw-r--r--   0        0        0     2259 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/tasks/load/base.py
+-rw-r--r--   0        0        0    18452 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/tasks/load/fivetran.py
+-rw-r--r--   0        0        0      946 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/tasks/load/main.py
+-rw-r--r--   0        0        0        0 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/tasks/setup/__init__.py
+-rw-r--r--   0        0        0      494 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/tasks/setup/base.py
+-rw-r--r--   0        0        0     4287 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/tasks/setup/dbt.py
+-rw-r--r--   0        0        0     6751 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/tasks/setup/git.py
+-rw-r--r--   0        0        0     1214 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/tasks/setup/main.py
+-rw-r--r--   0        0        0     1664 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/tasks/setup/pre_commit.py
+-rw-r--r--   0        0        0    10262 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/tasks/setup/ssh.py
+-rw-r--r--   0        0        0      845 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/tasks/setup/templates/pre_commit/copier.yml
+-rw-r--r--   0        0        0     2110 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/tasks/setup/templates/pre_commit/{% if use_sqlfluff or use_yamllint or use_dbt_checkpoint %}pre-commit-config.yaml{% endif %}.jinja
+-rw-r--r--   0        0        0       75 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_sqlfluff %}.sqlfluffignore{% endif %}
+-rw-r--r--   0        0        0     2743 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_sqlfluff %}.sqlfluff{% endif %}.jinja
+-rw-r--r--   0        0        0      668 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_yamllint %}.yamllint{% endif %}
+-rw-r--r--   0        0        0      102 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{{ _copier_conf.answers_file }}-precommit.yaml.jinja
+-rw-r--r--   0        0        0     1371 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/tasks/setup/utils.py
+-rw-r--r--   0        0        0      255 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/templates/model_props.yml
+-rw-r--r--   0        0        0      214 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/templates/source_props.yml
+-rw-r--r--   0        0        0     1201 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/templates/staging_model.sql
+-rw-r--r--   0        0        0      495 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/templates/staging_model_props.yml
+-rw-r--r--   0        0        0        0 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/ui/__init__.py
+-rw-r--r--   0        0        0     1202 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/ui/traceback.py
+-rw-r--r--   0        0        0        0 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/utils/__init__.py
+-rw-r--r--   0        0        0    11270 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/utils/api_caller.py
+-rw-r--r--   0        0        0    14980 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/utils/flags.py
+-rw-r--r--   0        0        0     1132 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/utils/jinja.py
+-rw-r--r--   0        0        0      785 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/utils/log.py
+-rw-r--r--   0        0        0      791 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/utils/shell.py
+-rw-r--r--   0        0        0     1872 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/utils/tracking.py
+-rw-r--r--   0        0        0     1010 2023-06-07 19:28:53.923801 dbt_coves-1.5.2/dbt_coves/utils/yaml.py
+-rw-r--r--   0        0        0     3606 2023-06-07 19:29:31.316032 dbt_coves-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0    24503 1970-01-01 00:00:00.000000 dbt_coves-1.5.2/PKG-INFO
```

### Comparing `dbt_coves-1.5.1/LICENSE` & `dbt_coves-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.1/README.md` & `dbt_coves-1.5.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -59,42 +59,40 @@
 ```console
 dbt-coves -h
 dbt-coves <command> -h
 ```
 
 ## Environment setup
 
-Setting up your environment can be done in two different ways:
-
-Runs a set of scripts in your local environment to configure your project components: `ssh keys`, `git` and `dbt`
-
-```console
-dbt-coves setup all
-```
-
-You can configure individual components:
+You can configure different components:
 
 Set up `git` repository of dbt-coves project
 
 ```console
 dbt-coves setup git
 ```
 
-Setup `dbt` within the project (delegates to dbt init)
+Set up `dbt` within the project (delegates to dbt init)
 
 ```console
 dbt-coves setup dbt
 ```
 
 Set up SSH Keys for dbt project. Supports the argument `--open_ssl_public_key` which generates an extra Public Key in Open SSL format, useful for configuring certain providers (i.e. Snowflake authentication)
 
 ```console
 dbt-coves setup ssh
 ```
 
+Set up pre-commit for your dbt project. In this, you can configure different tools that we consider essential for proper dbt usage: `sqlfluff`, `yaml-lint`, and `dbt-checkpoint`
+
+```console
+dbt-coves setup precommit
+```
+
 ## Models generation
 
 ```console
 dbt-coves generate <resource>
 ```
 
 Where _\<resource\>_ could be _sources_, _properties_ or _metadata_.
@@ -176,14 +174,29 @@
 
 ```console
 --metadata
 # Path to csv file containing metadata, i.e. 'metadata.csv'
 ```
 
 ```console
+--flatten-json-fields
+# Flag: flatten model JSON fields
+```
+
+```console
+--overwrite-staging-models
+# Flag: overwrite existent staging (SQL) files
+```
+
+```console
+--skip-model-props
+# Flag: don't create model's property (yml) files
+```
+
+```console
 --no-prompt
 # Silently generate source dbt models
 ```
 
 ### Properties Generation Arguments
 
 You can use dbt-coves to generate and update the properties(yml) file for a given dbt model(sql) file.
@@ -441,16 +454,15 @@
 dbt-coves dbt --project-dir /opt/user/dbt_project --virtualenv /opt/user/virtualenvs/airflow -- run -s model --vars \"{key: value}\"
 # Make sure to escape special characters such as quotation marks
 # Double dash (--) between <arguments> and <command> are mandatory
 ```
 
 # Settings
 
-dbt-coves will read settings from `.dbt_coves/config.yml`. A standard settings files could look like
-this:
+dbt-coves will read settings from `.dbt_coves/config.yml`. A standard settings files could look like this:
 
 ```yaml
 generate:
   sources:
     database: "RAW" # Database where to look for source tables
     schemas: # List of schema names where to look for source tables
       - RAW
@@ -515,14 +527,24 @@
     api_key: [KEY] # Fivetran API Key
     api_secret: [SECRET] # Fivetran API Secret
     secrets_path: /config/workspace/secrets/fivetran # Fivetran secret fields
     credentials: /opt/fivetran_credentials.yml # Fivetran set of key:secret pairs
     # 'api_key' + 'api_secret' are mutually exclusive with 'credentials', use one or the other
 ```
 
+## Telemetry
+
+dbt-coves has telemetry built in to help the maintainers from Datacoves understand which commands are being used and which are not to prioritize future development of dbt-coves. We do not track credentials nor details of your dbt execution such as model names. The one detail we do use related to dbt is the anonymous user_id to help us identify distinct users.
+
+By default this is turned on – you can opt out of event tracking at any time by adding the following to your dbt-coves `config.yaml` file:
+
+```yaml
+disable-tracking: true
+```
+
 ## Override generation templates
 
 Customizing generated models and model properties requires placing
 template files under the `.dbt-coves/templates` folder.
 
 There are different variables available in the templates:
```

### Comparing `dbt_coves-1.5.1/dbt_coves/config/config.py` & `dbt_coves-1.5.2/dbt_coves/config/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,17 @@
     sources_destination: Optional[str] = "models/staging/{{schema}}/{{schema}}.yml"
     models_destination: Optional[str] = "models/staging/{{schema}}/{{relation}}.sql"
     model_props_destination: Optional[str] = "models/staging/{{schema}}/{{relation}}.yml"
     update_strategy: Optional[str] = "ask"
     templates_folder: Optional[str] = ".dbt_coves/templates"
     metadata: Optional[str] = ""
     no_prompt: Optional[bool] = False
+    flatten_json_fields: Optional[bool] = False
+    overwrite_staging_models: Optional[bool] = False
+    skip_model_props: Optional[bool] = False
 
 
 class GenerateMetadataModel(BaseModel):
     database: Optional[str] = ""
     schemas: Optional[List[str]] = []
     select_relations: Optional[List[str]] = []
     exclude_relations: Optional[List[str]] = []
@@ -45,15 +48,14 @@
     no_prompt: Optional[bool] = False
 
 
 class GenerateModel(BaseModel):
     sources: Optional[GenerateSourcesModel] = GenerateSourcesModel()
     properties: Optional[GeneratePropertiesModel] = GeneratePropertiesModel()
     metadata: Optional[GenerateMetadataModel] = GenerateMetadataModel()
-    no_prompt: Optional[bool] = False
 
 
 class ExtractAirbyteModel(BaseModel):
     path: Optional[str] = ""
     host: Optional[str] = ""
     port: Optional[str] = ""
 
@@ -98,28 +100,23 @@
 
 
 class LoadModel(BaseModel):
     airbyte: Optional[LoadAirbyteModel] = LoadAirbyteModel()
     fivetran: Optional[LoadFivetranModel] = LoadFivetranModel()
 
 
-class SetupAllModel(BaseModel):
-    open_ssl_public_key: Optional[bool] = False
-
-
 class SetupSshModel(BaseModel):
     open_ssl_public_key: Optional[bool] = False
 
 
 class SetupGitModel(BaseModel):
     no_prompt: Optional[bool] = False
 
 
 class SetupModel(BaseModel):
-    all: Optional[SetupAllModel] = SetupAllModel()
     ssh: Optional[SetupSshModel] = SetupSshModel()
     git: Optional[SetupGitModel] = SetupGitModel()
 
 
 class RunDbtModel(BaseModel):
     command: Optional[str] = ""
     project_dir: Optional[str] = ""
@@ -155,14 +152,17 @@
         "generate.sources.sources_destination",
         "generate.sources.models_destination",
         "generate.sources.model_props_destination",
         "generate.sources.update_strategy",
         "generate.sources.templates_folder",
         "generate.sources.metadata",
         "generate.sources.no_prompt",
+        "generate.sources.flatten_json_fields",
+        "generate.sources.overwrite_staging_models",
+        "generate.sources.skip_model_props",
         "generate.metadata.database",
         "generate.metadata.schemas",
         "generate.metadata.select_relations",
         "generate.metadata.exclude_relations",
         "generate.metadata.destination",
         "generate.metadata.no_prompt",
         "extract.airbyte.path",
@@ -174,15 +174,14 @@
         "load.airbyte.secrets_path",
         "load.airbyte.secrets_manager",
         "load.airbyte.secrets_url",
         "load.airbyte.secrets_token",
         "load.airbyte.secrets_project",
         "load.airbyte.secrets_tags",
         "load.airbyte.secrets_key",
-        "setup.all.open_ssl_public_key",
         "setup.ssh.open_ssl_public_key",
         "setup.git.no_prompt",
         "dbt.command",
         "dbt.project_dir",
         "dbt.virtualenv",
         "dbt.cleanup",
         "extract.fivetran.path",
```

### Comparing `dbt_coves-1.5.1/dbt_coves/core/exceptions.py` & `dbt_coves-1.5.2/dbt_coves/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.1/dbt_coves/core/main.py` & `dbt_coves-1.5.2/dbt_coves/core/main.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.1/dbt_coves/tasks/base.py` & `dbt_coves-1.5.2/dbt_coves/tasks/base.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.1/dbt_coves/tasks/dbt/main.py` & `dbt_coves-1.5.2/dbt_coves/tasks/dbt/main.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.1/dbt_coves/tasks/extract/airbyte.py` & `dbt_coves-1.5.2/dbt_coves/tasks/extract/airbyte.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.1/dbt_coves/tasks/extract/fivetran.py` & `dbt_coves-1.5.2/dbt_coves/tasks/extract/fivetran.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.1/dbt_coves/tasks/extract/main.py` & `dbt_coves-1.5.2/dbt_coves/tasks/extract/main.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.1/dbt_coves/tasks/generate/base.py` & `dbt_coves-1.5.2/dbt_coves/tasks/generate/base.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.1/dbt_coves/tasks/generate/main.py` & `dbt_coves-1.5.2/dbt_coves/tasks/generate/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -29,20 +29,14 @@
     def register_parser(cls, sub_parsers, base_subparser):
         gen_subparser = sub_parsers.add_parser(
             "generate",
             parents=[base_subparser],
             help="""Generates dbt source and staging files, model property files and extracts
              metadata for tables (used as input for sources and properties)""",
         )
-        gen_subparser.add_argument(
-            "--no-prompt",
-            help="Silently generate dbt-coves resources",
-            action="store_true",
-            default=False,
-        )
         gen_subparser.set_defaults(cls=cls, which="generate")
         sub_parsers = gen_subparser.add_subparsers(title="dbt-coves generate commands", dest="task")
 
         # Register a separate sub parser for each sub task.
         [x.register_parser(sub_parsers, base_subparser) for x in cls.tasks]
         cls.arg_parser = gen_subparser
         return gen_subparser
```

### Comparing `dbt_coves-1.5.1/dbt_coves/tasks/generate/metadata.py` & `dbt_coves-1.5.2/dbt_coves/tasks/generate/metadata.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.1/dbt_coves/tasks/generate/properties.py` & `dbt_coves-1.5.2/dbt_coves/tasks/generate/properties.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.1/dbt_coves/tasks/generate/sources.py` & `dbt_coves-1.5.2/dbt_coves/tasks/generate/sources.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,14 +81,29 @@
         )
         subparser.add_argument(
             "--metadata",
             type=str,
             help="Path to csv file containing metadata, i.e. 'metadata.csv'",
         )
         subparser.add_argument(
+            "--flatten-json-fields", help="Flatten JSON fields", action="store_true", default=False
+        )
+        subparser.add_argument(
+            "--overwrite-staging-models",
+            help="Overwrite existent staging files",
+            action="store_true",
+            default=False,
+        )
+        subparser.add_argument(
+            "--skip-model-props",
+            help="Don't create model's property (yml) files",
+            action="store_true",
+            default=False,
+        )
+        subparser.add_argument(
             "--no-prompt",
             help="Silently generate source dbt models",
             action="store_true",
             default=False,
         )
         cls.arg_parser = base_subparser
         subparser.set_defaults(cls=cls, which="sources")
@@ -111,23 +126,28 @@
                     Choice(f"[{rel.schema}] {rel.name}", checked=True, value=rel) for rel in rels
                 ],
             ).ask()
 
             return selected_rels
 
     def generate(self, rels):
+        self.flatten_json = self.get_config_value("flatten_json_fields")
+        self.overwrite_sqls = self.get_config_value("overwrite_staging_models")
         models_destination = self.get_config_value("models_destination")
         options = {
-            "override_all": "Yes" if self.no_prompt else None,
-            "flatten_all": "Yes" if self.no_prompt else None,
+            "override_all": "Yes" if self.overwrite_sqls else None,
+            "flatten_all": "Yes" if self.flatten_json else None,
             "model_prop_update_all": False,
             "model_prop_recreate_all": False,
             "source_prop_update_all": False,
             "source_prop_recreate_all": False,
         }
+        if self.no_prompt:
+            options["override_all"] = options["override_all"] or "No"
+            options["flatten_all"] = options["flatten_all"] or "No"
         for rel in rels:
             model_dest = self.render_path_template(models_destination, rel)
             model_sql = Path(self.config.project_root).joinpath(model_dest)
             if not options["override_all"]:
                 if model_sql.exists():
                     overwrite = questionary.select(
                         f"{model_dest} already exists. Would you like to overwrite it?",
@@ -243,14 +263,15 @@
         config_db = self.get_config_value("database")
         if config_db:
             context["source_database"] = config_db
 
         return context
 
     def render_templates_with_context(self, context, sql_destination, options):
+        skip_model_props = self.get_config_value("skip_model_props")
         templates_folder = self.get_config_value("templates_folder")
         update_strategy = self.get_config_value("update_strategy")
         model_property_destination = self.get_config_value("model_props_destination")
         source_property_destination = self.get_config_value("sources_destination")
         rel = context["relation"]
 
         # Render model SQL
@@ -259,25 +280,26 @@
             context,
             sql_destination,
             templates_folder=templates_folder,
         )
         console.print(f"Model [green][b]{sql_destination}[/green][/b] created")
 
         # Render model and source YMLs
-        model_yml_dest = self.render_path_template(model_property_destination, rel)
-        model_yml_path = Path(self.config.project_root).joinpath(model_yml_dest)
-        self.render_property_files(
-            context,
-            options,
-            templates_folder,
-            update_strategy,
-            "model",
-            model_yml_path,
-            "staging_model_props.yml",
-        )
+        if not skip_model_props:
+            model_yml_dest = self.render_path_template(model_property_destination, rel)
+            model_yml_path = Path(self.config.project_root).joinpath(model_yml_dest)
+            self.render_property_files(
+                context,
+                options,
+                templates_folder,
+                update_strategy,
+                "model",
+                model_yml_path,
+                "staging_model_props.yml",
+            )
 
         source_yml_dest = self.render_path_template(source_property_destination, rel)
         source_yml_path = Path(self.config.project_root).joinpath(source_yml_dest)
         self.render_property_files(
             context,
             options,
             templates_folder,
```

### Comparing `dbt_coves-1.5.1/dbt_coves/tasks/generate/templates.py` & `dbt_coves-1.5.2/dbt_coves/tasks/generate/templates.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.1/dbt_coves/tasks/load/airbyte.py` & `dbt_coves-1.5.2/dbt_coves/tasks/load/airbyte.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.1/dbt_coves/tasks/load/base.py` & `dbt_coves-1.5.2/dbt_coves/tasks/load/base.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.1/dbt_coves/tasks/load/fivetran.py` & `dbt_coves-1.5.2/dbt_coves/tasks/load/fivetran.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.1/dbt_coves/tasks/load/main.py` & `dbt_coves-1.5.2/dbt_coves/tasks/load/main.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.1/dbt_coves/tasks/setup/dbt.py` & `dbt_coves-1.5.2/dbt_coves/tasks/setup/dbt.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.1/dbt_coves/tasks/setup/git.py` & `dbt_coves-1.5.2/dbt_coves/tasks/setup/git.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.1/dbt_coves/tasks/setup/main.py` & `dbt_coves-1.5.2/dbt_coves/tasks/setup/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from rich.console import Console
 
 from dbt_coves.tasks.base import NonDbtBaseTask
 
-from .all import SetupAllTask
 from .dbt import SetupDbtTask
 from .git import SetupGitTask
 from .pre_commit import SetupPrecommitTask
 from .ssh import SetupSSHTask
 
 console = Console()
 
@@ -17,15 +16,14 @@
 
 class SetupTask(NonDbtBaseTask):
     """
     Task that code-gen dbt resources
     """
 
     tasks = [
-        SetupAllTask,
         SetupGitTask,
         SetupDbtTask,
         SetupSSHTask,
         SetupPrecommitTask,
     ]
 
     key_column_with = 20
```

### Comparing `dbt_coves-1.5.1/dbt_coves/tasks/setup/pre_commit.py` & `dbt_coves-1.5.2/dbt_coves/tasks/setup/pre_commit.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.1/dbt_coves/tasks/setup/ssh.py` & `dbt_coves-1.5.2/dbt_coves/tasks/setup/ssh.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.1/dbt_coves/tasks/setup/templates/pre_commit/copier.yml` & `dbt_coves-1.5.2/dbt_coves/tasks/setup/templates/pre_commit/copier.yml`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.1/dbt_coves/tasks/setup/templates/pre_commit/{% if use_sqlfluff or use_yamllint or use_dbt_checkpoint %}pre-commit-config.yaml{% endif %}.jinja` & `dbt_coves-1.5.2/dbt_coves/tasks/setup/templates/pre_commit/{% if use_sqlfluff or use_yamllint or use_dbt_checkpoint %}pre-commit-config.yaml{% endif %}.jinja`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.1/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_sqlfluff %}.sqlfluff{% endif %}.jinja` & `dbt_coves-1.5.2/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_sqlfluff %}.sqlfluff{% endif %}.jinja`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.1/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_yamllint %}.yamllint{% endif %}` & `dbt_coves-1.5.2/dbt_coves/tasks/setup/templates/pre_commit/{{ dbt_project_dir }}/{% if use_yamllint %}.yamllint{% endif %}`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.1/dbt_coves/tasks/setup/utils.py` & `dbt_coves-1.5.2/dbt_coves/tasks/setup/utils.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.1/dbt_coves/templates/staging_model.sql` & `dbt_coves-1.5.2/dbt_coves/templates/staging_model.sql`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.1/dbt_coves/ui/traceback.py` & `dbt_coves-1.5.2/dbt_coves/ui/traceback.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.1/dbt_coves/utils/api_caller.py` & `dbt_coves-1.5.2/dbt_coves/utils/api_caller.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.1/dbt_coves/utils/flags.py` & `dbt_coves-1.5.2/dbt_coves/utils/flags.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,14 +42,17 @@
                 "sources_destination": None,
                 "models_destination": None,
                 "model_props_destination": None,
                 "update_strategy": None,
                 "templates_folder": None,
                 "metadata": None,
                 "no_prompt": False,
+                "flatten_json_fields": False,
+                "overwrite_staging_models": False,
+                "skip_model_props": False,
             },
             "properties": {
                 "templates_folder": None,
                 "metadata": None,
                 "destination": None,
                 "update_strategy": None,
                 "select": None,
@@ -107,15 +110,14 @@
             },
         }
         self.init = {
             "template": "https://github.com/datacoves/cookiecutter-dbt.git",
             "current-dir": False,
         }
         self.setup = {
-            "all": {"open_ssl_public_key": False},
             "ssh": {"open_ssl_public_key": False},
             "git": {"no_prompt": False},
         }
         self.dbt = {"command": None, "project_dir": None, "virtualenv": None, "cleanup": False}
 
     def parse_args(self, cli_args: List[str] = list()) -> None:
         self.args = self.cli_parser.parse_args(cli_args or sys.argv[1:])
@@ -182,14 +184,22 @@
                     self.generate["sources"]["metadata"] = self.args.metadata
                 if self.args.exclude_relations:
                     self.generate["sources"][
                         "exclude_relations"
                     ] = self.args.exclude_relations.split(",")
                 if self.args.no_prompt:
                     self.generate["sources"]["no_prompt"] = True
+                if self.args.flatten_json_fields:
+                    self.generate["sources"]["flatten_json_fields"] = True
+                if self.args.overwrite_staging_models:
+                    self.generate["sources"]["overwrite_staging_models"] = True
+                if self.args.skip_model_props:
+                    self.generate["sources"]["skip_model_props"] = True
+
+            # generate properties
             if self.args.cls.__name__ == "GeneratePropertiesTask":
                 if self.args.templates_folder:
                     self.generate["properties"]["templates_folder"] = self.args.templates_folder
                 if self.args.metadata:
                     self.generate["properties"]["metadata"] = self.args.metadata
                 if self.args.destination:
                     self.generate["properties"]["destination"] = self.args.destination
@@ -199,14 +209,16 @@
                     self.generate["properties"]["select"] = self.args.select
                 if self.args.exclude:
                     self.generate["properties"]["exclude"] = self.args.exclude
                 if self.args.selector:
                     self.generate["properties"]["selector"] = self.args.selector
                 if self.args.no_prompt:
                     self.generate["properties"]["no_prompt"] = True
+
+            # generate metadata
             if self.args.cls.__name__ == "GenerateMetadataTask":
                 if self.args.database:
                     self.generate["metadata"]["database"] = self.args.database
                 if self.args.schemas:
                     self.generate["metadata"]["schemas"] = [
                         schema.strip() for schema in self.args.schemas.split(",")
                     ]
@@ -219,20 +231,15 @@
                         relation.strip() for relation in self.args.exclude_relations.split(",")
                     ]
                 if self.args.destination:
                     self.generate["metadata"]["destination"] = self.args.destination
                 if self.args.no_prompt:
                     self.generate["metadata"]["no_prompt"] = True
 
-            if self.args.cls.__name__ == "InitTask":
-                if self.args.template:
-                    self.init["template"] = self.args.template
-                if self.args.current_dir:
-                    self.init["current-dir"] = self.args.current_dir
-
+            # load airbyte
             if self.args.cls.__name__ == "LoadAirbyteTask":
                 if self.args.path:
                     self.load["airbyte"]["path"] = self.args.path
 
                 if self.args.host and self.args.port:
                     self.load["airbyte"]["port"] = self.args.port
                     self.load["airbyte"]["host"] = self.args.host
@@ -249,14 +256,15 @@
                 if self.args.secrets_tags:
                     self.load["airbyte"]["secrets_tags"] = [
                         tag.strip() for tag in self.args.secrets_tags.split(",")
                     ]
                 if self.args.secrets_key:
                     self.load["airbyte"]["secrets_key"] = self.args.secrets_key
 
+            # load fivetran
             if self.args.cls.__name__ == "LoadFivetranTask":
                 if self.args.path:
                     self.load["fivetran"]["path"] = self.args.path
                 if self.args.api_key:
                     self.load["fivetran"]["api_key"] = self.args.api_key
                 if self.args.api_secret:
                     self.load["fivetran"]["api_secret"] = self.args.api_secret
@@ -275,42 +283,44 @@
                 if self.args.secrets_tags:
                     self.load["fivetran"]["secrets_tags"] = [
                         tag.strip() for tag in self.args.secrets_tags.split(",")
                     ]
                 if self.args.secrets_key:
                     self.load["fivetran"]["secrets_key"] = self.args.secrets_key
 
+            # extract airbyte
             if self.args.cls.__name__ == "ExtractAirbyteTask":
                 if self.args.path:
                     self.extract["airbyte"]["path"] = self.args.path
                 if self.args.host and self.args.port:
                     self.extract["airbyte"]["host"] = self.args.host
                     self.extract["airbyte"]["port"] = self.args.port
 
+            # extract fivetran
             if self.args.cls.__name__ == "ExtractFivetranTask":
                 if self.args.path:
                     self.extract["fivetran"]["path"] = self.args.path
                 if self.args.api_key:
                     self.extract["fivetran"]["api_key"] = self.args.api_key
                 if self.args.api_secret:
                     self.extract["fivetran"]["api_secret"] = self.args.api_secret
                 if self.args.credentials:
                     self.extract["fivetran"]["credentials"] = self.args.credentials
-            if self.args.cls.__name__ == "SetupAllTask":
-                if self.args.open_ssl_public_key:
-                    self.setup["all"]["open_ssl_public_key"] = self.args.open_ssl_public_key
 
+            # setup ssh
             if self.args.cls.__name__ == "SetupSSHTask":
                 if self.args.open_ssl_public_key:
                     self.setup["ssh"]["open_ssl_public_key"] = self.args.open_ssl_public_key
 
+            # setup git
             if self.args.cls.__name__ == "SetupGitTask":
                 if self.args.no_prompt:
                     self.setup["git"]["no_prompt"] = self.args.no_prompt
 
+            # run dbt
             if self.args.cls.__name__ == "RunDbtTask":
                 if self.args.command:
                     self.dbt["command"] = self.args.command
                 if self.args.project_dir:
                     self.dbt["project_dir"] = self.args.project_dir
                 if self.args.virtualenv:
                     self.dbt["virtualenv"] = self.args.virtualenv
```

### Comparing `dbt_coves-1.5.1/dbt_coves/utils/jinja.py` & `dbt_coves-1.5.2/dbt_coves/utils/jinja.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.1/dbt_coves/utils/log.py` & `dbt_coves-1.5.2/dbt_coves/utils/log.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.1/dbt_coves/utils/shell.py` & `dbt_coves-1.5.2/dbt_coves/utils/shell.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.1/dbt_coves/utils/tracking.py` & `dbt_coves-1.5.2/dbt_coves/utils/tracking.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,16 @@
 def trackable(task, **kwargs):
     def wrapper(task_instance, **kwargs):
         exit_code = task(task_instance)
         if not task_instance.args.disable_tracking:
             task_execution_props = _gen_task_usage_props(task_instance, exit_code)
             mixpanel.track(
                 distinct_id=task_instance.args.uuid,
-                event_name="dbt-coves usage",
+                event_name=f"{task_execution_props['dbt-coves command']}\
+                      {task_execution_props.get('dbt-coves subcommand', '')}",
                 properties=task_execution_props,
             )
         return exit_code
 
     return wrapper
```

### Comparing `dbt_coves-1.5.1/dbt_coves/utils/yaml.py` & `dbt_coves-1.5.2/dbt_coves/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `dbt_coves-1.5.1/pyproject.toml` & `dbt_coves-1.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbt_coves"
-version = "1.5.1"
+version = "1.5.2"
 description = "CLI tool for dbt users adopting analytics engineering best practices."
 authors = ["Datacoves <hello@datacoves.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Information Technology",
```

### Comparing `dbt_coves-1.5.1/PKG-INFO` & `dbt_coves-1.5.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-coves
-Version: 1.5.1
+Version: 1.5.2
 Summary: CLI tool for dbt users adopting analytics engineering best practices.
 Home-page: https://datacoves.com
 License: Apache 2.0
 Keywords: data engineering,analytics engineering,dbt,ETL,data modelling
 Author: Datacoves
 Author-email: hello@datacoves.com
 Requires-Python: >=3.7.2,<3.11
@@ -104,42 +104,40 @@
 ```console
 dbt-coves -h
 dbt-coves <command> -h
 ```
 
 ## Environment setup
 
-Setting up your environment can be done in two different ways:
-
-Runs a set of scripts in your local environment to configure your project components: `ssh keys`, `git` and `dbt`
-
-```console
-dbt-coves setup all
-```
-
-You can configure individual components:
+You can configure different components:
 
 Set up `git` repository of dbt-coves project
 
 ```console
 dbt-coves setup git
 ```
 
-Setup `dbt` within the project (delegates to dbt init)
+Set up `dbt` within the project (delegates to dbt init)
 
 ```console
 dbt-coves setup dbt
 ```
 
 Set up SSH Keys for dbt project. Supports the argument `--open_ssl_public_key` which generates an extra Public Key in Open SSL format, useful for configuring certain providers (i.e. Snowflake authentication)
 
 ```console
 dbt-coves setup ssh
 ```
 
+Set up pre-commit for your dbt project. In this, you can configure different tools that we consider essential for proper dbt usage: `sqlfluff`, `yaml-lint`, and `dbt-checkpoint`
+
+```console
+dbt-coves setup precommit
+```
+
 ## Models generation
 
 ```console
 dbt-coves generate <resource>
 ```
 
 Where _\<resource\>_ could be _sources_, _properties_ or _metadata_.
@@ -221,14 +219,29 @@
 
 ```console
 --metadata
 # Path to csv file containing metadata, i.e. 'metadata.csv'
 ```
 
 ```console
+--flatten-json-fields
+# Flag: flatten model JSON fields
+```
+
+```console
+--overwrite-staging-models
+# Flag: overwrite existent staging (SQL) files
+```
+
+```console
+--skip-model-props
+# Flag: don't create model's property (yml) files
+```
+
+```console
 --no-prompt
 # Silently generate source dbt models
 ```
 
 ### Properties Generation Arguments
 
 You can use dbt-coves to generate and update the properties(yml) file for a given dbt model(sql) file.
@@ -486,16 +499,15 @@
 dbt-coves dbt --project-dir /opt/user/dbt_project --virtualenv /opt/user/virtualenvs/airflow -- run -s model --vars \"{key: value}\"
 # Make sure to escape special characters such as quotation marks
 # Double dash (--) between <arguments> and <command> are mandatory
 ```
 
 # Settings
 
-dbt-coves will read settings from `.dbt_coves/config.yml`. A standard settings files could look like
-this:
+dbt-coves will read settings from `.dbt_coves/config.yml`. A standard settings files could look like this:
 
 ```yaml
 generate:
   sources:
     database: "RAW" # Database where to look for source tables
     schemas: # List of schema names where to look for source tables
       - RAW
@@ -560,14 +572,24 @@
     api_key: [KEY] # Fivetran API Key
     api_secret: [SECRET] # Fivetran API Secret
     secrets_path: /config/workspace/secrets/fivetran # Fivetran secret fields
     credentials: /opt/fivetran_credentials.yml # Fivetran set of key:secret pairs
     # 'api_key' + 'api_secret' are mutually exclusive with 'credentials', use one or the other
 ```
 
+## Telemetry
+
+dbt-coves has telemetry built in to help the maintainers from Datacoves understand which commands are being used and which are not to prioritize future development of dbt-coves. We do not track credentials nor details of your dbt execution such as model names. The one detail we do use related to dbt is the anonymous user_id to help us identify distinct users.
+
+By default this is turned on – you can opt out of event tracking at any time by adding the following to your dbt-coves `config.yaml` file:
+
+```yaml
+disable-tracking: true
+```
+
 ## Override generation templates
 
 Customizing generated models and model properties requires placing
 template files under the `.dbt-coves/templates` folder.
 
 There are different variables available in the templates:
```

