# Comparing `tmp/pipeline_ai-0.5.0b1.tar.gz` & `tmp/pipeline_ai-0.5.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipeline_ai-0.5.0b1.tar", max compression
+gzip compressed data, was "pipeline_ai-0.5.0b2.tar", max compression
```

## Comparing `pipeline_ai-0.5.0b1.tar` & `pipeline_ai-0.5.0b2.tar`

### file list

```diff
@@ -1,65 +1,71 @@
--rw-r--r--   0        0        0    10176 2022-12-02 15:06:10.248482 pipeline_ai-0.5.0b1/LICENSE
--rw-r--r--   0        0        0     6130 2023-02-09 11:46:02.323639 pipeline_ai-0.5.0b1/README.md
--rw-r--r--   0        0        0      434 2023-05-02 10:09:14.691672 pipeline_ai-0.5.0b1/pipeline/__init__.py
--rw-r--r--   0        0        0      135 2022-12-02 15:06:10.250042 pipeline_ai-0.5.0b1/pipeline/__main__.py
--rw-r--r--   0        0        0       62 2022-12-02 15:06:10.250106 pipeline_ai-0.5.0b1/pipeline/api/__init__.py
--rw-r--r--   0        0        0       62 2022-12-02 15:06:10.250175 pipeline_ai-0.5.0b1/pipeline/api/asyncio/__init__.py
--rw-r--r--   0        0        0     8380 2023-02-09 11:46:02.326800 pipeline_ai-0.5.0b1/pipeline/api/asyncio/cloud.py
--rw-r--r--   0        0        0    29923 2023-05-02 10:09:14.691895 pipeline_ai-0.5.0b1/pipeline/api/cloud.py
--rw-r--r--   0        0        0      974 2023-04-18 09:42:30.784749 pipeline_ai-0.5.0b1/pipeline/api/environments.py
--rw-r--r--   0        0        0     3247 2023-05-02 10:09:14.692205 pipeline_ai-0.5.0b1/pipeline/configuration/__init__.py
--rw-r--r--   0        0        0    11693 2023-05-02 10:09:14.692377 pipeline_ai-0.5.0b1/pipeline/console/__init__.py
--rw-r--r--   0        0        0     8254 2023-04-18 09:42:33.713012 pipeline_ai-0.5.0b1/pipeline/console/environments.py
--rw-r--r--   0        0        0     2460 2023-05-02 10:09:14.692500 pipeline_ai-0.5.0b1/pipeline/console/remote.py
--rw-r--r--   0        0        0     2011 2023-02-09 11:46:02.327719 pipeline_ai-0.5.0b1/pipeline/console/runs.py
--rw-r--r--   0        0        0     4838 2023-02-09 11:46:02.327903 pipeline_ai-0.5.0b1/pipeline/console/tags.py
--rw-r--r--   0        0        0     4868 2022-12-02 15:06:10.250566 pipeline_ai-0.5.0b1/pipeline/docker/__init__.py
--rw-r--r--   0        0        0      276 2022-12-02 15:06:10.250643 pipeline_ai-0.5.0b1/pipeline/exceptions/InvalidSchema.py
--rw-r--r--   0        0        0      283 2022-12-02 15:06:10.250688 pipeline_ai-0.5.0b1/pipeline/exceptions/MissingActiveToken.py
--rw-r--r--   0        0        0      312 2022-12-02 15:06:10.250731 pipeline_ai-0.5.0b1/pipeline/exceptions/NonChargeableProfile.py
--rw-r--r--   0        0        0      309 2022-12-02 15:06:10.250769 pipeline_ai-0.5.0b1/pipeline/exceptions/PipelineNotDeployed.py
--rw-r--r--   0        0        0      546 2022-12-02 15:06:10.250834 pipeline_ai-0.5.0b1/pipeline/objects/__init__.py
--rw-r--r--   0        0        0     4752 2023-04-18 09:42:30.785282 pipeline_ai-0.5.0b1/pipeline/objects/decorators.py
--rw-r--r--   0        0        0     1528 2022-12-02 15:06:10.250970 pipeline_ai-0.5.0b1/pipeline/objects/environment/__init__.py
--rw-r--r--   0        0        0     2015 2023-04-18 09:42:33.713113 pipeline_ai-0.5.0b1/pipeline/objects/function.py
--rw-r--r--   0        0        0    10909 2023-04-18 09:42:33.713234 pipeline_ai-0.5.0b1/pipeline/objects/graph.py
--rw-r--r--   0        0        0      877 2022-12-02 15:06:10.251134 pipeline_ai-0.5.0b1/pipeline/objects/graph_node.py
--rw-r--r--   0        0        0     1091 2022-12-02 15:06:10.251206 pipeline_ai-0.5.0b1/pipeline/objects/huggingface/TransformersModelForCausalLM.py
--rw-r--r--   0        0        0        0 2022-12-02 15:06:10.251229 pipeline_ai-0.5.0b1/pipeline/objects/huggingface/__init__.py
--rw-r--r--   0        0        0     1161 2023-04-18 09:42:33.713361 pipeline_ai-0.5.0b1/pipeline/objects/model.py
--rw-r--r--   0        0        0     3474 2022-12-02 15:06:10.251326 pipeline_ai-0.5.0b1/pipeline/objects/pipeline.py
--rw-r--r--   0        0        0     1861 2023-04-18 09:42:33.713467 pipeline_ai-0.5.0b1/pipeline/objects/variable.py
--rw-r--r--   0        0        0     1712 2023-02-09 11:46:02.328433 pipeline_ai-0.5.0b1/pipeline/objects/wrappers.py
--rw-r--r--   0        0        0        0 2022-12-02 15:06:10.251476 pipeline_ai-0.5.0b1/pipeline/schemas/__init__.py
--rw-r--r--   0        0        0     1821 2022-12-02 15:06:10.251534 pipeline_ai-0.5.0b1/pipeline/schemas/base.py
--rw-r--r--   0        0        0      369 2022-12-02 15:06:10.251632 pipeline_ai-0.5.0b1/pipeline/schemas/compute_requirements.py
--rw-r--r--   0        0        0      558 2022-12-02 15:06:10.251680 pipeline_ai-0.5.0b1/pipeline/schemas/data.py
--rw-r--r--   0        0        0      573 2022-12-02 15:06:10.251726 pipeline_ai-0.5.0b1/pipeline/schemas/deployment.py
--rw-r--r--   0        0        0      516 2023-04-18 09:42:30.785393 pipeline_ai-0.5.0b1/pipeline/schemas/environment.py
--rw-r--r--   0        0        0      714 2023-04-18 09:42:33.713564 pipeline_ai-0.5.0b1/pipeline/schemas/file.py
--rw-r--r--   0        0        0     2426 2023-04-18 09:42:33.713663 pipeline_ai-0.5.0b1/pipeline/schemas/function.py
--rw-r--r--   0        0        0     5236 2022-12-02 15:06:10.251930 pipeline_ai-0.5.0b1/pipeline/schemas/metrics.py
--rw-r--r--   0        0        0      569 2022-12-02 15:06:10.251976 pipeline_ai-0.5.0b1/pipeline/schemas/milestones_register.py
--rw-r--r--   0        0        0     1599 2023-04-18 09:42:33.713758 pipeline_ai-0.5.0b1/pipeline/schemas/model.py
--rw-r--r--   0        0        0      739 2022-12-02 15:06:10.252069 pipeline_ai-0.5.0b1/pipeline/schemas/onboarding.py
--rw-r--r--   0        0        0      944 2022-12-02 15:06:10.252252 pipeline_ai-0.5.0b1/pipeline/schemas/pagination.py
--rw-r--r--   0        0        0     5817 2023-04-18 09:42:33.713869 pipeline_ai-0.5.0b1/pipeline/schemas/pipeline.py
--rw-r--r--   0        0        0     1261 2023-02-09 11:46:02.328929 pipeline_ai-0.5.0b1/pipeline/schemas/pipeline_file.py
--rw-r--r--   0        0        0      537 2022-12-02 15:06:10.252406 pipeline_ai-0.5.0b1/pipeline/schemas/project.py
--rw-r--r--   0        0        0        0 2022-12-02 15:06:10.252452 pipeline_ai-0.5.0b1/pipeline/schemas/redis/__init__.py
--rw-r--r--   0        0        0      234 2022-12-02 15:06:10.252503 pipeline_ai-0.5.0b1/pipeline/schemas/redis/command.py
--rw-r--r--   0        0        0      337 2022-12-02 15:06:10.252545 pipeline_ai-0.5.0b1/pipeline/schemas/request.py
--rw-r--r--   0        0        0      261 2022-12-02 15:06:10.252589 pipeline_ai-0.5.0b1/pipeline/schemas/resource.py
--rw-r--r--   0        0        0     3839 2023-02-09 11:46:02.329041 pipeline_ai-0.5.0b1/pipeline/schemas/run.py
--rw-r--r--   0        0        0     1031 2022-12-02 15:06:10.252742 pipeline_ai-0.5.0b1/pipeline/schemas/runnable.py
--rw-r--r--   0        0        0      167 2022-12-02 15:06:10.252798 pipeline_ai-0.5.0b1/pipeline/schemas/tag.py
--rw-r--r--   0        0        0     1668 2022-12-02 15:06:10.252857 pipeline_ai-0.5.0b1/pipeline/schemas/token.py
--rw-r--r--   0        0        0     3827 2023-02-09 11:46:02.329149 pipeline_ai-0.5.0b1/pipeline/schemas/user.py
--rw-r--r--   0        0        0     2493 2023-02-09 11:46:02.329255 pipeline_ai-0.5.0b1/pipeline/schemas/validators.py
--rw-r--r--   0        0        0      320 2022-12-02 15:06:10.253073 pipeline_ai-0.5.0b1/pipeline/schemas/worker.py
--rw-r--r--   0        0        0     1924 2023-04-18 09:42:33.713983 pipeline_ai-0.5.0b1/pipeline/util/__init__.py
--rw-r--r--   0        0        0     1129 2022-12-02 15:06:10.253212 pipeline_ai-0.5.0b1/pipeline/util/logging.py
--rw-r--r--   0        0        0      241 2022-12-02 15:06:10.253288 pipeline_ai-0.5.0b1/pipeline/util/torch_utils/__init__.py
--rw-r--r--   0        0        0     2265 2023-05-02 10:09:14.692860 pipeline_ai-0.5.0b1/pipeline/v3/__init__.py
--rw-r--r--   0        0        0     1272 2023-05-02 10:11:19.947144 pipeline_ai-0.5.0b1/pyproject.toml
--rw-r--r--   0        0        0     7131 1970-01-01 00:00:00.000000 pipeline_ai-0.5.0b1/PKG-INFO
+-rw-r--r--   0        0        0    10176 2023-06-07 10:41:11.051565 pipeline_ai-0.5.0b2/LICENSE
+-rw-r--r--   0        0        0     6130 2023-06-07 10:41:11.051565 pipeline_ai-0.5.0b2/README.md
+-rw-r--r--   0        0        0      434 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/__init__.py
+-rw-r--r--   0        0        0      135 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/__main__.py
+-rw-r--r--   0        0        0       62 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/api/__init__.py
+-rw-r--r--   0        0        0       62 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/api/asyncio/__init__.py
+-rw-r--r--   0        0        0     8380 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/api/asyncio/cloud.py
+-rw-r--r--   0        0        0    29923 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/api/cloud.py
+-rw-r--r--   0        0        0      974 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/api/environments.py
+-rw-r--r--   0        0        0     3247 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/configuration/__init__.py
+-rw-r--r--   0        0        0    11693 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/console/__init__.py
+-rw-r--r--   0        0        0     8254 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/console/environments.py
+-rw-r--r--   0        0        0     2587 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/console/remote.py
+-rw-r--r--   0        0        0     2011 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/console/runs.py
+-rw-r--r--   0        0        0     4838 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/console/tags.py
+-rw-r--r--   0        0        0     4868 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/docker/__init__.py
+-rw-r--r--   0        0        0      276 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/exceptions/InvalidSchema.py
+-rw-r--r--   0        0        0      283 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/exceptions/MissingActiveToken.py
+-rw-r--r--   0        0        0      312 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/exceptions/NonChargeableProfile.py
+-rw-r--r--   0        0        0      309 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/exceptions/PipelineNotDeployed.py
+-rw-r--r--   0        0        0      546 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/objects/__init__.py
+-rw-r--r--   0        0        0     4752 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/objects/decorators.py
+-rw-r--r--   0        0        0     1528 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/objects/environment/__init__.py
+-rw-r--r--   0        0        0     2015 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/objects/function.py
+-rw-r--r--   0        0        0    10909 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/objects/graph.py
+-rw-r--r--   0        0        0      877 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/objects/graph_node.py
+-rw-r--r--   0        0        0     1091 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/objects/huggingface/TransformersModelForCausalLM.py
+-rw-r--r--   0        0        0        0 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/objects/huggingface/__init__.py
+-rw-r--r--   0        0        0     1161 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/objects/model.py
+-rw-r--r--   0        0        0     3474 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/objects/pipeline.py
+-rw-r--r--   0        0        0     1861 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/objects/variable.py
+-rw-r--r--   0        0        0     1712 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/objects/wrappers.py
+-rw-r--r--   0        0        0        0 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/schemas/__init__.py
+-rw-r--r--   0        0        0     1821 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/schemas/base.py
+-rw-r--r--   0        0        0      369 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/schemas/compute_requirements.py
+-rw-r--r--   0        0        0      558 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/schemas/data.py
+-rw-r--r--   0        0        0      573 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/schemas/deployment.py
+-rw-r--r--   0        0        0      516 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/schemas/environment.py
+-rw-r--r--   0        0        0      714 2023-06-07 10:41:11.055565 pipeline_ai-0.5.0b2/pipeline/schemas/file.py
+-rw-r--r--   0        0        0     2426 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/schemas/function.py
+-rw-r--r--   0        0        0     5236 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/schemas/metrics.py
+-rw-r--r--   0        0        0      569 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/schemas/milestones_register.py
+-rw-r--r--   0        0        0     1599 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/schemas/model.py
+-rw-r--r--   0        0        0      739 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/schemas/onboarding.py
+-rw-r--r--   0        0        0      944 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/schemas/pagination.py
+-rw-r--r--   0        0        0     5817 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/schemas/pipeline.py
+-rw-r--r--   0        0        0     1261 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/schemas/pipeline_file.py
+-rw-r--r--   0        0        0      537 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/schemas/project.py
+-rw-r--r--   0        0        0        0 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/schemas/redis/__init__.py
+-rw-r--r--   0        0        0      234 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/schemas/redis/command.py
+-rw-r--r--   0        0        0      337 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/schemas/request.py
+-rw-r--r--   0        0        0      261 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/schemas/resource.py
+-rw-r--r--   0        0        0     3839 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/schemas/run.py
+-rw-r--r--   0        0        0     1031 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/schemas/runnable.py
+-rw-r--r--   0        0        0      167 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/schemas/tag.py
+-rw-r--r--   0        0        0     1668 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/schemas/token.py
+-rw-r--r--   0        0        0     3827 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/schemas/user.py
+-rw-r--r--   0        0        0     2493 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/schemas/validators.py
+-rw-r--r--   0        0        0      320 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/schemas/worker.py
+-rw-r--r--   0        0        0     1924 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/util/__init__.py
+-rw-r--r--   0        0        0     1129 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/util/logging.py
+-rw-r--r--   0        0        0      241 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/util/torch_utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/v3/__init__.py
+-rw-r--r--   0        0        0      287 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/v3/environments.py
+-rw-r--r--   0        0        0     3131 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/v3/http.py
+-rw-r--r--   0        0        0     3701 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/v3/pipelines.py
+-rw-r--r--   0        0        0        0 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/v3/schemas/__init__.py
+-rw-r--r--   0        0        0     2172 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/v3/schemas/runs.py
+-rw-r--r--   0        0        0     4571 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pipeline/v3/uploading.py
+-rw-r--r--   0        0        0     1249 2023-06-07 10:41:11.059565 pipeline_ai-0.5.0b2/pyproject.toml
+-rw-r--r--   0        0        0     7132 1970-01-01 00:00:00.000000 pipeline_ai-0.5.0b2/PKG-INFO
```

### Comparing `pipeline_ai-0.5.0b1/LICENSE` & `pipeline_ai-0.5.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b1/README.md` & `pipeline_ai-0.5.0b2/README.md`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b1/pipeline/api/asyncio/cloud.py` & `pipeline_ai-0.5.0b2/pipeline/api/asyncio/cloud.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b1/pipeline/api/cloud.py` & `pipeline_ai-0.5.0b2/pipeline/api/cloud.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b1/pipeline/api/environments.py` & `pipeline_ai-0.5.0b2/pipeline/api/environments.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b1/pipeline/configuration/__init__.py` & `pipeline_ai-0.5.0b2/pipeline/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b1/pipeline/console/__init__.py` & `pipeline_ai-0.5.0b2/pipeline/console/__init__.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b1/pipeline/console/environments.py` & `pipeline_ai-0.5.0b2/pipeline/console/environments.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b1/pipeline/console/remote.py` & `pipeline_ai-0.5.0b2/pipeline/console/remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,19 @@
 
         resource_data = [
             [
                 resource["id"],
                 str(resource["current_run"])
                 if (resource["busy"] == 1 and resource["current_run"] != -1)
                 else "-",
-                resource["pipeline_cache"]["cached_pipelines"],
+                [
+                    p_id
+                    for cached_pipelines in resource["pipeline_cache"].values()
+                    for p_id in cached_pipelines
+                ],
                 resource["run_queue"],
                 "N/A"
                 if resource["gpus"] is None
                 else [gpu["name"].strip() for gpu in resource["gpus"]],
             ]
             for resource in resource_information
         ]
```

### Comparing `pipeline_ai-0.5.0b1/pipeline/console/runs.py` & `pipeline_ai-0.5.0b2/pipeline/console/runs.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b1/pipeline/console/tags.py` & `pipeline_ai-0.5.0b2/pipeline/console/tags.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b1/pipeline/docker/__init__.py` & `pipeline_ai-0.5.0b2/pipeline/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b1/pipeline/objects/__init__.py` & `pipeline_ai-0.5.0b2/pipeline/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b1/pipeline/objects/decorators.py` & `pipeline_ai-0.5.0b2/pipeline/objects/decorators.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b1/pipeline/objects/environment/__init__.py` & `pipeline_ai-0.5.0b2/pipeline/objects/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b1/pipeline/objects/function.py` & `pipeline_ai-0.5.0b2/pipeline/objects/function.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b1/pipeline/objects/graph.py` & `pipeline_ai-0.5.0b2/pipeline/objects/graph.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b1/pipeline/objects/graph_node.py` & `pipeline_ai-0.5.0b2/pipeline/objects/graph_node.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b1/pipeline/objects/huggingface/TransformersModelForCausalLM.py` & `pipeline_ai-0.5.0b2/pipeline/objects/huggingface/TransformersModelForCausalLM.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b1/pipeline/objects/model.py` & `pipeline_ai-0.5.0b2/pipeline/objects/model.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b1/pipeline/objects/pipeline.py` & `pipeline_ai-0.5.0b2/pipeline/objects/pipeline.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b1/pipeline/objects/variable.py` & `pipeline_ai-0.5.0b2/pipeline/objects/variable.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b1/pipeline/objects/wrappers.py` & `pipeline_ai-0.5.0b2/pipeline/objects/wrappers.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b1/pipeline/schemas/base.py` & `pipeline_ai-0.5.0b2/pipeline/schemas/base.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b1/pipeline/schemas/data.py` & `pipeline_ai-0.5.0b2/pipeline/schemas/data.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b1/pipeline/schemas/deployment.py` & `pipeline_ai-0.5.0b2/pipeline/schemas/deployment.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b1/pipeline/schemas/environment.py` & `pipeline_ai-0.5.0b2/pipeline/schemas/environment.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b1/pipeline/schemas/file.py` & `pipeline_ai-0.5.0b2/pipeline/schemas/file.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b1/pipeline/schemas/function.py` & `pipeline_ai-0.5.0b2/pipeline/schemas/function.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b1/pipeline/schemas/metrics.py` & `pipeline_ai-0.5.0b2/pipeline/schemas/metrics.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b1/pipeline/schemas/milestones_register.py` & `pipeline_ai-0.5.0b2/pipeline/schemas/milestones_register.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b1/pipeline/schemas/model.py` & `pipeline_ai-0.5.0b2/pipeline/schemas/model.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b1/pipeline/schemas/onboarding.py` & `pipeline_ai-0.5.0b2/pipeline/schemas/onboarding.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b1/pipeline/schemas/pagination.py` & `pipeline_ai-0.5.0b2/pipeline/schemas/pagination.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b1/pipeline/schemas/pipeline.py` & `pipeline_ai-0.5.0b2/pipeline/schemas/pipeline.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b1/pipeline/schemas/pipeline_file.py` & `pipeline_ai-0.5.0b2/pipeline/schemas/pipeline_file.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b1/pipeline/schemas/project.py` & `pipeline_ai-0.5.0b2/pipeline/schemas/project.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b1/pipeline/schemas/run.py` & `pipeline_ai-0.5.0b2/pipeline/schemas/run.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b1/pipeline/schemas/runnable.py` & `pipeline_ai-0.5.0b2/pipeline/schemas/runnable.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b1/pipeline/schemas/token.py` & `pipeline_ai-0.5.0b2/pipeline/schemas/token.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b1/pipeline/schemas/user.py` & `pipeline_ai-0.5.0b2/pipeline/schemas/user.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b1/pipeline/schemas/validators.py` & `pipeline_ai-0.5.0b2/pipeline/schemas/validators.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b1/pipeline/util/__init__.py` & `pipeline_ai-0.5.0b2/pipeline/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b1/pipeline/util/logging.py` & `pipeline_ai-0.5.0b2/pipeline/util/logging.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b1/pyproject.toml` & `pipeline_ai-0.5.0b2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pipeline-ai"
-version = "0.5.0b1"
+version = "0.5.0b2"
 
 description = "Pipelines for machine learning workloads."
 authors = [
   "Paul Hetherington <ph@mystic.ai>",
   "Alex Pearwin <alex@mystic.ai>",
   "Neil Wang <neil@mystic.ai>",
   "Ross Gray <ross@mystic.ai>",
@@ -19,20 +19,22 @@
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pydantic = "^1.8.2"
 setuptools = "^65.4.1"
 pyhumps = "^3.0.2"
 tqdm = "^4.62.3"
-PyYAML = { version = "^6.0", optional = true }
+PyYAML = "^6.0"
 cloudpickle = "^2.2.0"
 dill = "^0.3.6"
 httpx = "^0.23.1"
 tabulate = "^0.9.0"
 packaging = ">=21.0"
+requests = "^2.30.0"
+requests-toolbelt = "^1.0.0"
 
 [tool.poetry.dev-dependencies]
 pydantic = "^1.8.2"
 pyhumps = "^3.0.2"
 pytest = "^6.2.5"
 black = "^22.10.0"
 pre-commit = "^2.16.0"
@@ -54,12 +56,9 @@
   )/
 )
 '''
 
 [tool.isort]
 profile = "black"
 
-[tool.poetry.extras]
-docker = ["PyYAML"]
-
 [tool.poetry.scripts]
 pipeline = "pipeline.console:_run"
```

### Comparing `pipeline_ai-0.5.0b1/PKG-INFO` & `pipeline_ai-0.5.0b2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: pipeline-ai
-Version: 0.5.0b1
+Version: 0.5.0b2
 Summary: Pipelines for machine learning workloads.
 License: Apache-2.0
 Author: Paul Hetherington
 Author-email: ph@mystic.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Provides-Extra: docker
-Requires-Dist: PyYAML (>=6.0,<7.0) ; extra == "docker"
+Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: cloudpickle (>=2.2.0,<3.0.0)
 Requires-Dist: dill (>=0.3.6,<0.4.0)
 Requires-Dist: httpx (>=0.23.1,<0.24.0)
 Requires-Dist: packaging (>=21.0)
 Requires-Dist: pydantic (>=1.8.2,<2.0.0)
 Requires-Dist: pyhumps (>=3.0.2,<4.0.0)
+Requires-Dist: requests (>=2.30.0,<3.0.0)
+Requires-Dist: requests-toolbelt (>=1.0.0,<2.0.0)
 Requires-Dist: setuptools (>=65.4.1,<66.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: tqdm (>=4.62.3,<5.0.0)
 Description-Content-Type: text/markdown
 
 # [Pipeline](https://pipeline.ai) [![Version](https://img.shields.io/pypi/v/pipeline-ai)](https://pypi.org/project/pipeline-ai) ![Size](https://img.shields.io/github/repo-size/neuro-ai-dev/pipeline) ![Downloads](https://img.shields.io/pypi/dm/pipeline-ai) [![License](https://img.shields.io/crates/l/ap)](https://www.apache.org/licenses/LICENSE-2.0) [![Discord](https://img.shields.io/badge/discord-join-blue)](https://discord.gg/eJQRkBdEcs)
```

