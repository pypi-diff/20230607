# Comparing `tmp/kpops-1.1.4.tar.gz` & `tmp/kpops-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kpops-1.1.4.tar", max compression
+gzip compressed data, was "kpops-1.1.5.tar", max compression
```

## Comparing `kpops-1.1.4.tar` & `kpops-1.1.5.tar`

### file list

```diff
@@ -1,63 +1,64 @@
--rw-r--r--   0        0        0     1064 2023-05-22 10:02:06.851773 kpops-1.1.4/LICENSE
--rw-r--r--   0        0        0     2370 2023-05-22 10:02:06.851773 kpops-1.1.4/README.md
--rw-r--r--   0        0        0       22 2023-05-22 10:02:32.843686 kpops-1.1.4/kpops/__init__.py
--rw-r--r--   0        0        0        0 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/cli/__init__.py
--rw-r--r--   0        0        0      761 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/cli/custom_formatter.py
--rw-r--r--   0        0        0      122 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/cli/exception.py
--rw-r--r--   0        0        0    11727 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/cli/main.py
--rw-r--r--   0        0        0     4206 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/cli/pipeline_config.py
--rw-r--r--   0        0        0     1711 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/cli/registry.py
--rw-r--r--   0        0        0      688 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/component_handlers/__init__.py
--rw-r--r--   0        0        0        0 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/component_handlers/helm_wrapper/__init__.py
--rw-r--r--   0        0        0       52 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/component_handlers/helm_wrapper/exception.py
--rw-r--r--   0        0        0     9357 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/component_handlers/helm_wrapper/helm.py
--rw-r--r--   0        0        0     2152 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/component_handlers/helm_wrapper/helm_diff.py
--rw-r--r--   0        0        0     4373 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/component_handlers/helm_wrapper/model.py
--rw-r--r--   0        0        0      667 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/component_handlers/helm_wrapper/utils.py
--rw-r--r--   0        0        0        0 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/component_handlers/kafka_connect/__init__.py
--rw-r--r--   0        0        0     8202 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/component_handlers/kafka_connect/connect_wrapper.py
--rw-r--r--   0        0        0      182 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/component_handlers/kafka_connect/exception.py
--rw-r--r--   0        0        0     5890 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/component_handlers/kafka_connect/kafka_connect_handler.py
--rw-r--r--   0        0        0     1851 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/component_handlers/kafka_connect/model.py
--rw-r--r--   0        0        0      788 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/component_handlers/kafka_connect/timeout.py
--rw-r--r--   0        0        0        0 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/component_handlers/schema_handler/__init__.py
--rw-r--r--   0        0        0     6035 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/component_handlers/schema_handler/schema_handler.py
--rw-r--r--   0        0        0      361 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/component_handlers/schema_handler/schema_provider.py
--rw-r--r--   0        0        0        0 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/component_handlers/topic/__init__.py
--rw-r--r--   0        0        0      180 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/component_handlers/topic/exception.py
--rw-r--r--   0        0        0     9588 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/component_handlers/topic/handler.py
--rw-r--r--   0        0        0     2503 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/component_handlers/topic/model.py
--rw-r--r--   0        0        0     6937 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/component_handlers/topic/proxy_wrapper.py
--rw-r--r--   0        0        0     2385 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/component_handlers/topic/utils.py
--rw-r--r--   0        0        0        0 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/component_handlers/utils/__init__.py
--rw-r--r--   0        0        0      630 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/component_handlers/utils/exception.py
--rw-r--r--   0        0        0      492 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/components/__init__.py
--rw-r--r--   0        0        0      466 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/components/base_components/__init__.py
--rw-r--r--   0        0        0     8321 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/components/base_components/base_defaults_component.py
--rw-r--r--   0        0        0     7457 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/components/base_components/kafka_app.py
--rw-r--r--   0        0        0    16472 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/components/base_components/kafka_connector.py
--rw-r--r--   0        0        0     6775 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/components/base_components/kubernetes_app.py
--rw-r--r--   0        0        0        0 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/components/base_components/models/__init__.py
--rw-r--r--   0        0        0     2447 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/components/base_components/models/from_section.py
--rw-r--r--   0        0        0     3272 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/components/base_components/models/to_section.py
--rw-r--r--   0        0        0    11398 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/components/base_components/pipeline_component.py
--rw-r--r--   0        0        0      211 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/components/streams_bootstrap/__init__.py
--rw-r--r--   0        0        0      217 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/components/streams_bootstrap/app_type.py
--rw-r--r--   0        0        0        0 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/components/streams_bootstrap/producer/__init__.py
--rw-r--r--   0        0        0     1116 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/components/streams_bootstrap/producer/model.py
--rw-r--r--   0        0        0     2859 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/components/streams_bootstrap/producer/producer_app.py
--rw-r--r--   0        0        0        0 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/components/streams_bootstrap/streams/__init__.py
--rw-r--r--   0        0        0     9097 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/components/streams_bootstrap/streams/model.py
--rw-r--r--   0        0        0     4080 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/components/streams_bootstrap/streams/streams_app.py
--rw-r--r--   0        0        0        0 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/pipeline_generator/__init__.py
--rw-r--r--   0        0        0    10755 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/pipeline_generator/pipeline.py
--rw-r--r--   0        0        0        0 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/utils/__init__.py
--rw-r--r--   0        0        0      289 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/utils/colorify.py
--rw-r--r--   0        0        0     3043 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/utils/dict_differ.py
--rw-r--r--   0        0        0     2589 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/utils/docstring.py
--rw-r--r--   0        0        0     5808 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/utils/gen_schema.py
--rw-r--r--   0        0        0      594 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/utils/pydantic.py
--rw-r--r--   0        0        0     1189 2023-05-22 10:02:06.855773 kpops-1.1.4/kpops/utils/yaml_loading.py
--rw-r--r--   0        0        0     1892 2023-05-22 10:02:32.831686 kpops-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     3948 1970-01-01 00:00:00.000000 kpops-1.1.4/setup.py
--rw-r--r--   0        0        0     3965 1970-01-01 00:00:00.000000 kpops-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-07 12:01:07.240769 kpops-1.1.5/LICENSE
+-rw-r--r--   0        0        0     2370 2023-06-07 12:01:07.240769 kpops-1.1.5/README.md
+-rw-r--r--   0        0        0       22 2023-06-07 12:01:31.725022 kpops-1.1.5/kpops/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/cli/__init__.py
+-rw-r--r--   0        0        0      761 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/cli/custom_formatter.py
+-rw-r--r--   0        0        0      122 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/cli/exception.py
+-rw-r--r--   0        0        0    11727 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/cli/main.py
+-rw-r--r--   0        0        0     4206 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/cli/pipeline_config.py
+-rw-r--r--   0        0        0     1711 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/cli/registry.py
+-rw-r--r--   0        0        0      688 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/component_handlers/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/component_handlers/helm_wrapper/__init__.py
+-rw-r--r--   0        0        0       52 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/component_handlers/helm_wrapper/exception.py
+-rw-r--r--   0        0        0     9357 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/component_handlers/helm_wrapper/helm.py
+-rw-r--r--   0        0        0     2152 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/component_handlers/helm_wrapper/helm_diff.py
+-rw-r--r--   0        0        0     4373 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/component_handlers/helm_wrapper/model.py
+-rw-r--r--   0        0        0      667 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/component_handlers/helm_wrapper/utils.py
+-rw-r--r--   0        0        0        0 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/component_handlers/kafka_connect/__init__.py
+-rw-r--r--   0        0        0     8142 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/component_handlers/kafka_connect/connect_wrapper.py
+-rw-r--r--   0        0        0      235 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/component_handlers/kafka_connect/exception.py
+-rw-r--r--   0        0        0     5823 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/component_handlers/kafka_connect/kafka_connect_handler.py
+-rw-r--r--   0        0        0     1851 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/component_handlers/kafka_connect/model.py
+-rw-r--r--   0        0        0      999 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/component_handlers/kafka_connect/timeout.py
+-rw-r--r--   0        0        0        0 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/component_handlers/schema_handler/__init__.py
+-rw-r--r--   0        0        0     6035 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/component_handlers/schema_handler/schema_handler.py
+-rw-r--r--   0        0        0      361 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/component_handlers/schema_handler/schema_provider.py
+-rw-r--r--   0        0        0        0 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/component_handlers/topic/__init__.py
+-rw-r--r--   0        0        0      231 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/component_handlers/topic/exception.py
+-rw-r--r--   0        0        0     9454 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/component_handlers/topic/handler.py
+-rw-r--r--   0        0        0     2503 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/component_handlers/topic/model.py
+-rw-r--r--   0        0        0     6917 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/component_handlers/topic/proxy_wrapper.py
+-rw-r--r--   0        0        0     2385 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/component_handlers/topic/utils.py
+-rw-r--r--   0        0        0        0 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/component_handlers/utils/__init__.py
+-rw-r--r--   0        0        0      630 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/component_handlers/utils/exception.py
+-rw-r--r--   0        0        0      492 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/components/__init__.py
+-rw-r--r--   0        0        0      466 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/components/base_components/__init__.py
+-rw-r--r--   0        0        0     8338 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/components/base_components/base_defaults_component.py
+-rw-r--r--   0        0        0     7457 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/components/base_components/kafka_app.py
+-rw-r--r--   0        0        0    16472 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/components/base_components/kafka_connector.py
+-rw-r--r--   0        0        0     6778 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/components/base_components/kubernetes_app.py
+-rw-r--r--   0        0        0        0 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/components/base_components/models/__init__.py
+-rw-r--r--   0        0        0     2447 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/components/base_components/models/from_section.py
+-rw-r--r--   0        0        0     3272 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/components/base_components/models/to_section.py
+-rw-r--r--   0        0        0    11401 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/components/base_components/pipeline_component.py
+-rw-r--r--   0        0        0      211 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/components/streams_bootstrap/__init__.py
+-rw-r--r--   0        0        0      217 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/components/streams_bootstrap/app_type.py
+-rw-r--r--   0        0        0        0 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/components/streams_bootstrap/producer/__init__.py
+-rw-r--r--   0        0        0     1116 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/components/streams_bootstrap/producer/model.py
+-rw-r--r--   0        0        0     2859 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/components/streams_bootstrap/producer/producer_app.py
+-rw-r--r--   0        0        0        0 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/components/streams_bootstrap/streams/__init__.py
+-rw-r--r--   0        0        0     9097 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/components/streams_bootstrap/streams/model.py
+-rw-r--r--   0        0        0     4080 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/components/streams_bootstrap/streams/streams_app.py
+-rw-r--r--   0        0        0        0 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/pipeline_generator/__init__.py
+-rw-r--r--   0        0        0    10738 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/pipeline_generator/pipeline.py
+-rw-r--r--   0        0        0        0 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/utils/__init__.py
+-rw-r--r--   0        0        0      289 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/utils/colorify.py
+-rw-r--r--   0        0        0     3043 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/utils/dict_differ.py
+-rw-r--r--   0        0        0     2589 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/utils/docstring.py
+-rw-r--r--   0        0        0     1032 2023-06-07 12:01:07.244769 kpops-1.1.5/kpops/utils/environment.py
+-rw-r--r--   0        0        0     5808 2023-06-07 12:01:07.248770 kpops-1.1.5/kpops/utils/gen_schema.py
+-rw-r--r--   0        0        0      594 2023-06-07 12:01:07.248770 kpops-1.1.5/kpops/utils/pydantic.py
+-rw-r--r--   0        0        0     1221 2023-06-07 12:01:07.248770 kpops-1.1.5/kpops/utils/yaml_loading.py
+-rw-r--r--   0        0        0     1867 2023-06-07 12:01:31.709022 kpops-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3949 1970-01-01 00:00:00.000000 kpops-1.1.5/setup.py
+-rw-r--r--   0        0        0     3966 1970-01-01 00:00:00.000000 kpops-1.1.5/PKG-INFO
```

### Comparing `kpops-1.1.4/LICENSE` & `kpops-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kpops-1.1.4/README.md` & `kpops-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `kpops-1.1.4/kpops/cli/custom_formatter.py` & `kpops-1.1.5/kpops/cli/custom_formatter.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.4/kpops/cli/main.py` & `kpops-1.1.5/kpops/cli/main.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.4/kpops/cli/pipeline_config.py` & `kpops-1.1.5/kpops/cli/pipeline_config.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.4/kpops/cli/registry.py` & `kpops-1.1.5/kpops/cli/registry.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.4/kpops/component_handlers/__init__.py` & `kpops-1.1.5/kpops/component_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.4/kpops/component_handlers/helm_wrapper/helm.py` & `kpops-1.1.5/kpops/component_handlers/helm_wrapper/helm.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.4/kpops/component_handlers/helm_wrapper/helm_diff.py` & `kpops-1.1.5/kpops/component_handlers/helm_wrapper/helm_diff.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.4/kpops/component_handlers/helm_wrapper/model.py` & `kpops-1.1.5/kpops/component_handlers/helm_wrapper/model.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.4/kpops/component_handlers/helm_wrapper/utils.py` & `kpops-1.1.5/kpops/component_handlers/helm_wrapper/utils.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.4/kpops/component_handlers/kafka_connect/connect_wrapper.py` & `kpops-1.1.5/kpops/component_handlers/kafka_connect/connect_wrapper.py`

 * *Files 11% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         """
         Creates a new connector
         API Reference: https://docs.confluent.io/platform/current/connect/references/restapi.html#post--connectors
         :param connector_name: The name of the connector
         :param kafka_connect_config: The config of the connector
         :return: The current connector info if successful
         """
-        config_json = kafka_connect_config.dict(exclude_none=True, exclude_unset=True)
+        config_json = kafka_connect_config.dict(exclude_none=True)
         connect_data = {"name": connector_name, "config": config_json}
         response = requests.post(
             url=f"{self._host}/connectors", headers=HEADERS, json=connect_data
         )
         if response.status_code == requests.status_codes.codes.created:
             log.info(f"Connector {connector_name} created.")
             log.debug(response.json())
@@ -95,15 +95,15 @@
     ) -> KafkaConnectResponse:
         """
         Create a new connector using the given configuration, or update the configuration for an existing connector.
         :param connector_name: Name of the created connector
         :param kafka_connect_config: Configuration parameters for the connector.
         :return: Information about the connector after the change has been made.
         """
-        config_json = kafka_connect_config.dict(exclude_none=True, exclude_unset=True)
+        config_json = kafka_connect_config.dict(exclude_none=True)
         response = requests.put(
             url=f"{self._host}/connectors/{connector_name}/config",
             headers=HEADERS,
             json=config_json,
         )
         data: dict = response.json()
         if response.status_code == requests.status_codes.codes.ok:
@@ -122,15 +122,15 @@
             self.update_connector_config(connector_name, kafka_connect_config)
         raise KafkaConnectError(response)
 
     @classmethod
     def get_connector_config(
         cls, connector_name: str, config: KafkaConnectConfig
     ) -> dict[str, Any]:
-        connector_config = config.dict(exclude_none=True, exclude_unset=True)
+        connector_config = config.dict(exclude_none=True)
         if (name := connector_config.get("name")) and name != connector_name:
             raise ValueError("Connector name should be the same as component name")
         connector_config["name"] = connector_name
         return connector_config
 
     def validate_connector_config(
         self, connector_name: str, kafka_connect_config: KafkaConnectConfig
```

### Comparing `kpops-1.1.4/kpops/component_handlers/kafka_connect/kafka_connect_handler.py` & `kpops-1.1.5/kpops/component_handlers/kafka_connect/kafka_connect_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from __future__ import annotations
 
 import logging
-import sys
 from typing import TYPE_CHECKING
 
 from kpops.component_handlers.kafka_connect.connect_wrapper import ConnectWrapper
-from kpops.component_handlers.kafka_connect.exception import ConnectorNotFoundException
+from kpops.component_handlers.kafka_connect.exception import (
+    ConnectorNotFoundException,
+    ConnectorStateException,
+)
 from kpops.component_handlers.kafka_connect.model import KafkaConnectConfig
 from kpops.component_handlers.kafka_connect.timeout import timeout
 from kpops.utils.colorify import magentaify
 from kpops.utils.dict_differ import render_diff
 
 if TYPE_CHECKING:
     from kpops.cli.pipeline_config import PipelineConfig
@@ -97,36 +99,33 @@
                 connector_config.config,
                 ConnectWrapper.get_connector_config(
                     connector_name, kafka_connect_config
                 ),
             ):
                 log.info(f"Updating config:\n{diff}")
 
-            log.debug(kafka_connect_config.dict(exclude_unset=True, exclude_none=True))
+            log.debug(kafka_connect_config.dict(exclude_none=True))
             log.debug(f"PUT /connectors/{connector_name}/config HTTP/1.1")
             log.debug(f"HOST: {self._connect_wrapper.host}")
         except ConnectorNotFoundException:
             diff = render_diff({}, kafka_connect_config.dict())
             log.info(
                 f"Connector Creation: connector {connector_name} does not exist. Creating connector with config:\n{diff}"
             )
             log.debug("POST /connectors HTTP/1.1")
             log.debug(f"HOST: {self._connect_wrapper.host}")
 
         errors = self._connect_wrapper.validate_connector_config(
             connector_name, kafka_connect_config
         )
         if len(errors) > 0:
-            log.error(
-                f"Connector Creation: validating the connector config for connector {connector_name} resulted in the following errors:"
+            formatted_errors = "\n".join(errors)
+            raise ConnectorStateException(
+                f"Connector Creation: validating the connector config for connector {connector_name} resulted in the following errors: {formatted_errors}"
             )
-            log.error("\n".join(errors))
-            sys.exit(
-                1
-            )  # FIXME raise instead https://github.com/bakdata/kpops/issues/101
         else:
             log.info(
                 f"Connector Creation: connector config for {connector_name} is valid!"
             )
 
     def __dry_run_connector_deletion(self, connector_name: str) -> None:
         try:
```

### Comparing `kpops-1.1.4/kpops/component_handlers/kafka_connect/model.py` & `kpops-1.1.5/kpops/component_handlers/kafka_connect/model.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.4/kpops/component_handlers/schema_handler/schema_handler.py` & `kpops-1.1.5/kpops/component_handlers/schema_handler/schema_handler.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.4/kpops/component_handlers/topic/handler.py` & `kpops-1.1.5/kpops/component_handlers/topic/handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import logging
 
-from kpops.component_handlers.topic.exception import TopicNotFoundException
+from kpops.component_handlers.topic.exception import (
+    TopicNotFoundException,
+    TopicTransactionError,
+)
 from kpops.component_handlers.topic.model import (
     TopicConfigResponse,
     TopicResponse,
     TopicSpec,
 )
 from kpops.component_handlers.topic.proxy_wrapper import HEADERS, ProxyWrapper
 from kpops.component_handlers.topic.utils import (
@@ -143,18 +146,17 @@
         if partition_count == (
             topic_spec.partitions_count or int(broker_config["num.partitions"])
         ):
             log.debug(
                 f"Topic Creation: partition count of topic {topic_name} did not change. Current partitions count {partition_count}. Updating configs."
             )
         else:
-            log.error(
+            raise TopicTransactionError(
                 f"Topic Creation: partition count of topic {topic_name} changed! Partitions count of topic {topic_name} is {partition_count}. The given partitions count {topic_spec.partitions_count}."
             )
-            exit(1)  # FIXME raise instead https://github.com/bakdata/kpops/issues/101
 
     @staticmethod
     def __check_replication_factor(
         topic_in_cluster: TopicResponse,
         topic_spec: TopicSpec,
         broker_config: dict[str, str],
     ) -> None:
@@ -164,18 +166,17 @@
             topic_spec.replication_factor
             or int(broker_config["default.replication.factor"])
         ):
             log.debug(
                 f"Topic Creation: replication factor of topic {topic_name} did not change. Current replication factor {replication_factor}. Updating configs."
             )
         else:
-            log.error(
+            raise TopicTransactionError(
                 f"Topic Creation: replication factor of topic {topic_name} changed! Replication factor of topic {topic_name} is {replication_factor}. The given replication count {topic_spec.replication_factor}."
             )
-            exit(1)  # FIXME raise instead https://github.com/bakdata/kpops/issues/101
 
     def __dry_run_topic_deletion(self, topic_name: str) -> None:
         try:
             topic_in_cluster = self.proxy_wrapper.get_topic(topic_name=topic_name)
             log.info(
                 magentaify(
                     f"Topic Deletion: topic {topic_in_cluster.topic_name} exists in the cluster. Deleting topic."
@@ -208,15 +209,14 @@
         """
         topic_spec_json: dict = topic_config.dict(
             include={
                 "partitions_count": True,
                 "replication_factor": True,
                 "configs": True,
             },
-            exclude_unset=True,
             exclude_none=True,
         )
         configs = []
         for config_name, config_value in topic_spec_json["configs"].items():
             configs.append({"name": config_name, "value": config_value})
         topic_spec_json["configs"] = configs
         topic_spec_json["topic_name"] = topic_name
```

### Comparing `kpops-1.1.4/kpops/component_handlers/topic/model.py` & `kpops-1.1.5/kpops/component_handlers/topic/model.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.4/kpops/component_handlers/topic/proxy_wrapper.py` & `kpops-1.1.5/kpops/component_handlers/topic/proxy_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         Creates a topic.
         API Reference: https://docs.confluent.io/platform/current/kafka-rest/api.html#post--clusters-cluster_id-topics
         :param topic_spec: The topic specification.
         """
         response = requests.post(
             url=f"{self._host}/v3/clusters/{self.cluster_id}/topics",
             headers=HEADERS,
-            json=topic_spec.dict(exclude_unset=True, exclude_none=True),
+            json=topic_spec.dict(exclude_none=True),
         )
         if response.status_code == requests.status_codes.codes.created:
             log.info(f"Topic {topic_spec.topic_name} created.")
             log.debug(response.json())
             return
 
         raise KafkaRestProxyError(response)
```

### Comparing `kpops-1.1.4/kpops/component_handlers/topic/utils.py` & `kpops-1.1.5/kpops/component_handlers/topic/utils.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.4/kpops/component_handlers/utils/exception.py` & `kpops-1.1.5/kpops/component_handlers/utils/exception.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.4/kpops/components/base_components/base_defaults_component.py` & `kpops-1.1.5/kpops/components/base_components/base_defaults_component.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import inspect
 import logging
-import os
 from collections import deque
 from collections.abc import Mapping, Sequence
 from pathlib import Path
 from typing import TypeVar
 
 import typer
 from pydantic import BaseModel, Field
 
 from kpops.cli.pipeline_config import PipelineConfig
 from kpops.component_handlers import ComponentHandlers
 from kpops.utils.docstring import describe_attr
+from kpops.utils.environment import ENV
 from kpops.utils.pydantic import DescConfig
 from kpops.utils.yaml_loading import load_yaml_file
 
 log = logging.getLogger("PipelineComponentEnricher")
 
 
 class BaseDefaultsComponent(BaseModel):
@@ -154,15 +154,15 @@
     :returns: All defaults set for the given component in the provided yaml
     :rtype: dict
 
     :Example:
 
     kafka_app_defaults = defaults_from_yaml(Path("/path/to/defaults.yaml"), "kafka-app")
     """
-    content = load_yaml_file(path, substitution=dict(os.environ))
+    content = load_yaml_file(path, substitution=ENV)
     if not isinstance(content, dict):
         raise TypeError(
             "Default files should be structured as map ([app type] -> [default config]"
         )
     value = content.get(key)
     if value is None:
         return {}
```

### Comparing `kpops-1.1.4/kpops/components/base_components/kafka_app.py` & `kpops-1.1.5/kpops/components/base_components/kafka_app.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.4/kpops/components/base_components/kafka_connector.py` & `kpops-1.1.5/kpops/components/base_components/kafka_connector.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.4/kpops/components/base_components/kubernetes_app.py` & `kpops-1.1.5/kpops/components/base_components/kubernetes_app.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
 
     def to_helm_values(self) -> dict:
         """Generate a dictionary of values readable by Helm from `self.app`
 
         :returns: Thte values to be used by Helm
         :rtype: dict
         """
-        return self.app.dict(by_alias=True, exclude_none=True, exclude_unset=True)
+        return self.app.dict(by_alias=True, exclude_none=True, exclude_defaults=True)
 
     def print_helm_diff(self, stdout: str) -> None:
         """Print the diff of the last and current release of this component
 
         :param stdout: The output of a Helm command that installs or upgrades the release
         :type stdout: str
         """
```

### Comparing `kpops-1.1.4/kpops/components/base_components/models/from_section.py` & `kpops-1.1.5/kpops/components/base_components/models/from_section.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.4/kpops/components/base_components/models/to_section.py` & `kpops-1.1.5/kpops/components/base_components/models/to_section.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.4/kpops/components/base_components/pipeline_component.py` & `kpops-1.1.5/kpops/components/base_components/pipeline_component.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-import os
 from functools import cached_property
 from typing import Literal
 
 from pydantic import Extra, Field
 
 from kpops.components.base_components.base_defaults_component import (
     BaseDefaultsComponent,
@@ -16,14 +15,15 @@
 )
 from kpops.components.base_components.models.to_section import (
     OutputTopicTypes,
     TopicConfig,
     ToSection,
 )
 from kpops.utils.docstring import describe_attr, describe_object
+from kpops.utils.environment import ENV
 from kpops.utils.pydantic import CamelCaseConfig, DescConfig
 from kpops.utils.yaml_loading import substitute
 
 
 class PipelineComponent(BaseDefaultsComponent):
     """Base class for all components
 
@@ -114,20 +114,20 @@
 
         :param topic_name: topic name
         :return: final topic name
         """
         error_topic_name = self.substitute_component_names(
             self.config.topic_name_config.default_error_topic_name,
             self.type,
-            **os.environ,
+            **ENV,
         )
         output_topic_name = self.substitute_component_names(
             self.config.topic_name_config.default_output_topic_name,
             self.type,
-            **os.environ,
+            **ENV,
         )
         return self.substitute_component_names(
             topic_name,
             self.type,
             component_name=self.name,
             error_topic_name=error_topic_name,
             output_topic_name=output_topic_name,
@@ -324,8 +324,8 @@
 
         :param dry_run: Whether to do a dry run of the command
         :type dry_run: bool
         """
 
     def substitute_prefix(self) -> None:
         """Substitute $-placeholders in self.prefix with environment variables"""
-        self.prefix = substitute(self.prefix, dict(os.environ))
+        self.prefix = substitute(self.prefix, ENV)
```

### Comparing `kpops-1.1.4/kpops/components/streams_bootstrap/producer/model.py` & `kpops-1.1.5/kpops/components/streams_bootstrap/producer/model.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.4/kpops/components/streams_bootstrap/producer/producer_app.py` & `kpops-1.1.5/kpops/components/streams_bootstrap/producer/producer_app.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.4/kpops/components/streams_bootstrap/streams/model.py` & `kpops-1.1.5/kpops/components/streams_bootstrap/streams/model.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.4/kpops/components/streams_bootstrap/streams/streams_app.py` & `kpops-1.1.5/kpops/components/streams_bootstrap/streams/streams_app.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.4/kpops/pipeline_generator/pipeline.py` & `kpops-1.1.5/kpops/pipeline_generator/pipeline.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from __future__ import annotations
 
 import json
 import logging
-import os
 from collections.abc import Iterator
 from contextlib import suppress
 from pathlib import Path
 
 import yaml
 from pydantic import BaseModel
 from rich.console import Console
 from rich.syntax import Syntax
 
 from kpops.cli.pipeline_config import PipelineConfig
 from kpops.cli.registry import Registry
 from kpops.component_handlers import ComponentHandlers
 from kpops.components.base_components.base_defaults_component import update_nested_pair
 from kpops.components.base_components.pipeline_component import PipelineComponent
+from kpops.utils.environment import ENV
 from kpops.utils.yaml_loading import load_yaml_file, substitute
 
 log = logging.getLogger("PipelineGenerator")
 
 
 class ParsingException(Exception):
     pass
@@ -72,15 +72,15 @@
     for component in environment_components:
         if "type" not in component or "name" not in component:
             raise ValueError(
                 "To override components per environment, every component should at least have a type and a name."
             )
         index[
             PipelineComponent.substitute_component_names(
-                component["name"], component["type"], **os.environ
+                component["name"], component["type"], **ENV
             )
         ] = component
     return index
 
 
 class Pipeline:
     def __init__(
@@ -105,23 +105,23 @@
         path: Path,
         registry: Registry,
         config: PipelineConfig,
         handlers: ComponentHandlers,
     ) -> Pipeline:
         Pipeline.set_pipeline_name_env_vars(base_dir, path)
 
-        main_content = load_yaml_file(path, substitution=dict(os.environ))
+        main_content = load_yaml_file(path, substitution=ENV)
         if not isinstance(main_content, list):
             raise TypeError(
                 f"The pipeline definition {path} should contain a list of components"
             )
 
         env_content = []
         if (env_file := Pipeline.pipeline_filename_environment(path, config)).exists():
-            env_content = load_yaml_file(env_file, substitution=dict(os.environ))
+            env_content = load_yaml_file(env_file, substitution=ENV)
             if not isinstance(env_content, list):
                 raise TypeError(
                     f"The pipeline definition {env_file} should contain a list of components"
                 )
 
         pipeline = cls(main_content, env_content, registry, config, handlers)
         return pipeline
@@ -269,10 +269,10 @@
         :param base_dir: Base directory to the pipeline files
         :param path: Path to pipeline.yaml file
         """
         path_without_file = path.resolve().relative_to(base_dir.resolve()).parts[:-1]
         if not path_without_file:
             raise ValueError("The pipeline-base-dir should not equal the pipeline-path")
         pipeline_name = "-".join(path_without_file)
-        os.environ["pipeline_name"] = pipeline_name
+        ENV["pipeline_name"] = pipeline_name
         for level, parent in enumerate(path_without_file):
-            os.environ[f"pipeline_name_{level}"] = parent
+            ENV[f"pipeline_name_{level}"] = parent
```

### Comparing `kpops-1.1.4/kpops/utils/dict_differ.py` & `kpops-1.1.5/kpops/utils/dict_differ.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.4/kpops/utils/docstring.py` & `kpops-1.1.5/kpops/utils/docstring.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.4/kpops/utils/gen_schema.py` & `kpops-1.1.5/kpops/utils/gen_schema.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.4/kpops/utils/pydantic.py` & `kpops-1.1.5/kpops/utils/pydantic.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.4/kpops/utils/yaml_loading.py` & `kpops-1.1.5/kpops/utils/yaml_loading.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,23 +4,25 @@
 from typing import Any
 
 import yaml
 from cachetools import cached
 from cachetools.keys import hashkey
 
 
-def generate_hashkey(file_path: Path, substitution: dict | None = None) -> tuple:
+def generate_hashkey(
+    file_path: Path, substitution: Mapping[str, Any] | None = None
+) -> tuple:
     if substitution is None:
         substitution = {}
     return hashkey(str(file_path) + str(sorted(substitution.items())))
 
 
 @cached(cache={}, key=generate_hashkey)
 def load_yaml_file(
-    file_path: Path, *, substitution: dict | None = None
+    file_path: Path, *, substitution: Mapping[str, Any] | None = None
 ) -> dict | list[dict]:
     with open(file_path) as yaml_file:
         return yaml.load(substitute(yaml_file.read(), substitution), Loader=yaml.Loader)
 
 
 def substitute(input: str, substitution: Mapping[str, Any] | None = None) -> str:
     """Substitute $-placeholders in input using template string.
```

### Comparing `kpops-1.1.4/pyproject.toml` & `kpops-1.1.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 [tool.poetry]
 name = "kpops"
-version = "1.1.4"
+version = "1.1.5"
 description = "KPOps is a tool to deploy Kafka pipelines to Kubernetes"
 authors = ["bakdata <opensource@bakdata.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bakdata/kpops"
 documentation = "https://bakdata.github.io/kpops/latest"
 keywords = ["kafka", "kubernetes", "stream-processing", "pipelines"]
 classifiers = [
-    "Environment :: Console",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.10",
-    "Topic :: Software Development :: Libraries :: Python Modules",
-    "Topic :: Software Development :: Libraries",
-    "Topic :: Software Development",
-    "Intended Audience :: Developers",
-    "Typing :: Typed",
+  "Environment :: Console",
+  "License :: OSI Approved :: MIT License",
+  "Operating System :: OS Independent",
+  "Programming Language :: Python",
+  "Programming Language :: Python :: 3",
+  "Programming Language :: Python :: 3 :: Only",
+  "Programming Language :: Python :: 3.10",
+  "Topic :: Software Development :: Libraries :: Python Modules",
+  "Topic :: Software Development :: Libraries",
+  "Topic :: Software Development",
+  "Intended Audience :: Developers",
+  "Typing :: Typed",
 ]
 
 [tool.poetry.scripts]
 kpops = "kpops.cli.main:app"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-pydantic = { extras = ["dotenv"], version = "^1.9.1" }
+pydantic = {extras = ["dotenv"], version = "^1.10.8"}
 rich = "^12.4.4"
 PyYAML = "^6.0"
 requests = "^2.28.0"
 typer = { extras = ["all"], version = "^0.6.1" }
 pyhumps = "^3.7.3"
 cachetools = "^5.2.0"
 dictdiffer = "^0.9.0"
```

### Comparing `kpops-1.1.4/setup.py` & `kpops-1.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,27 +22,27 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['PyYAML>=6.0,<7.0',
  'cachetools>=5.2.0,<6.0.0',
  'dictdiffer>=0.9.0,<0.10.0',
- 'pydantic[dotenv]>=1.9.1,<2.0.0',
+ 'pydantic[dotenv]>=1.10.8,<2.0.0',
  'pyhumps>=3.7.3,<4.0.0',
  'python-schema-registry-client>=2.4.1,<3.0.0',
  'requests>=2.28.0,<3.0.0',
  'rich>=12.4.4,<13.0.0',
  'typer[all]>=0.6.1,<0.7.0']
 
 entry_points = \
 {'console_scripts': ['kpops = kpops.cli.main:app']}
 
 setup_kwargs = {
     'name': 'kpops',
-    'version': '1.1.4',
+    'version': '1.1.5',
     'description': 'KPOps is a tool to deploy Kafka pipelines to Kubernetes',
     'long_description': '# KPOps\n\n[![Build status](https://github.com/bakdata/kpops/actions/workflows/ci.yaml/badge.svg)](https://github.com/bakdata/kpops/actions/workflows/ci.yaml)\n[![pypi](https://img.shields.io/pypi/v/kpops.svg)](https://pypi.org/project/kpops)\n[![versions](https://img.shields.io/pypi/pyversions/kpops.svg)](https://github.com/bakdata/kpops)\n[![license](https://img.shields.io/github/license/bakdata/kpops.svg)](https://github.com/bakdata/kpops/blob/main/LICENSE)\n\n## Key features\n\n- **Deploy Kafka apps to Kubernetes**: KPOps allows to deploy consecutive Kafka Streams applications and producers using an easy-to-read and -write pipeline definition.\n- **Manage Kafka Connectors**: KPOps connects with your Kafka Connect cluster and deploys, validates, and deletes your connectors.\n- **Configure multiple pipelines and steps**: KPOps has various abstractions that simplify configuring multiple pipelines and steps within pipelines by sharing common configuration between different components, such as producers or streaming applications.\n- **Handle your topics and schemas**: KPOps not only creates and deletes your topics but also registers and deletes your schemas.\n- **Clean termination of Kafka components**: KPOps removes your pipeline components (i.e., Kafka Streams applications) from the Kubernetes cluster _and_ cleans up the component-related states (i.e., removing/resetting offset of Kafka consumer groups).\n- **Preview your pipeline changes**: With the KPOps dry-run, you can ensure your pipeline definition is set up correctly. This helps to minimize downtime and prevent potential errors or issues that could impact your production environment.\n\n## Documentation\n\nFor detailed usage and installation instructions, check out\nthe [documentation](https://bakdata.github.io/kpops/latest/user/what-is-kpops/).\n\n## Install KPOps\n\nKPOps comes as a [PyPI package](https://pypi.org/project/kpops/). \nYou can install it with [pip](https://github.com/pypa/pip):\n\n```shell\npip install kpops\n```\n\n## Contributing\n\nWe are happy if you want to contribute to this project.\nIf you find any bugs or have suggestions for improvements, please open an issue.\nWe are also happy to accept your PRs.\nJust open an issue beforehand and let us know what you want to do and why.\n\n## License\n\nKPOps is licensed under the [MIT License](https://github.com/bakdata/kpops/blob/main/LICENSE).\n',
     'author': 'bakdata',
     'author_email': 'opensource@bakdata.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/bakdata/kpops',
```

### Comparing `kpops-1.1.4/PKG-INFO` & `kpops-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kpops
-Version: 1.1.4
+Version: 1.1.5
 Summary: KPOps is a tool to deploy Kafka pipelines to Kubernetes
 Home-page: https://github.com/bakdata/kpops
 License: MIT
 Keywords: kafka,kubernetes,stream-processing,pipelines
 Author: bakdata
 Author-email: opensource@bakdata.com
 Requires-Python: >=3.10,<4.0
@@ -22,15 +22,15 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: cachetools (>=5.2.0,<6.0.0)
 Requires-Dist: dictdiffer (>=0.9.0,<0.10.0)
-Requires-Dist: pydantic[dotenv] (>=1.9.1,<2.0.0)
+Requires-Dist: pydantic[dotenv] (>=1.10.8,<2.0.0)
 Requires-Dist: pyhumps (>=3.7.3,<4.0.0)
 Requires-Dist: python-schema-registry-client (>=2.4.1,<3.0.0)
 Requires-Dist: requests (>=2.28.0,<3.0.0)
 Requires-Dist: rich (>=12.4.4,<13.0.0)
 Requires-Dist: typer[all] (>=0.6.1,<0.7.0)
 Project-URL: Documentation, https://bakdata.github.io/kpops/latest
 Project-URL: Repository, https://github.com/bakdata/kpops
```

