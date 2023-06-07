# Comparing `tmp/dcicutils-7.5.0.tar.gz` & `tmp/dcicutils-7.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcicutils-7.5.0.tar", max compression
+gzip compressed data, was "dcicutils-7.5.1.tar", max compression
```

## Comparing `dcicutils-7.5.0.tar` & `dcicutils-7.5.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1098 2023-05-31 13:58:40.363974 dcicutils-7.5.0/LICENSE.txt
--rw-r--r--   0        0        0     1166 2023-05-31 13:58:40.363974 dcicutils-7.5.0/README.rst
--rw-r--r--   0        0        0        0 2023-05-31 13:58:40.363974 dcicutils-7.5.0/dcicutils/__init__.py
--rw-r--r--   0        0        0     5115 2023-05-31 13:58:40.363974 dcicutils-7.5.0/dcicutils/base.py
--rwxr-xr-x   0        0        0    51434 2023-05-31 13:58:40.363974 dcicutils-7.5.0/dcicutils/beanstalk_utils.py
--rw-r--r--   0        0        0    13786 2023-05-31 13:58:40.363974 dcicutils-7.5.0/dcicutils/cloudformation_utils.py
--rw-r--r--   0        0        0     1155 2023-05-31 13:58:40.363974 dcicutils-7.5.0/dcicutils/codebuild_utils.py
--rw-r--r--   0        0        0    15285 2023-05-31 13:58:40.363974 dcicutils-7.5.0/dcicutils/command_utils.py
--rw-r--r--   0        0        0     3723 2023-05-31 13:58:40.363974 dcicutils-7.5.0/dcicutils/common.py
--rw-r--r--   0        0        0    11032 2023-05-31 13:58:40.363974 dcicutils-7.5.0/dcicutils/creds_utils.py
--rw-r--r--   0        0        0     3098 2023-05-31 13:58:40.363974 dcicutils-7.5.0/dcicutils/data_utils.py
--rw-r--r--   0        0        0    68354 2023-05-31 13:58:40.363974 dcicutils-7.5.0/dcicutils/deployment_utils.py
--rw-r--r--   0        0        0     8118 2023-05-31 13:58:40.363974 dcicutils-7.5.0/dcicutils/diff_utils.py
--rw-r--r--   0        0        0     1747 2023-05-31 13:58:40.363974 dcicutils-7.5.0/dcicutils/docker_utils.py
--rw-r--r--   0        0        0    19474 2023-05-31 13:58:40.363974 dcicutils-7.5.0/dcicutils/ecr_scripts.py
--rw-r--r--   0        0        0    13079 2023-05-31 13:58:40.363974 dcicutils-7.5.0/dcicutils/ecr_utils.py
--rw-r--r--   0        0        0     3590 2023-05-31 13:58:40.363974 dcicutils-7.5.0/dcicutils/ecs_utils.py
--rw-r--r--   0        0        0     6356 2023-05-31 13:58:40.363974 dcicutils-7.5.0/dcicutils/env_base.py
--rw-r--r--   0        0        0     9444 2023-05-31 13:58:40.367974 dcicutils-7.5.0/dcicutils/env_manager.py
--rw-r--r--   0        0        0     3909 2023-05-31 13:58:40.367974 dcicutils-7.5.0/dcicutils/env_scripts.py
--rw-r--r--   0        0        0    46739 2023-05-31 13:58:40.367974 dcicutils-7.5.0/dcicutils/env_utils.py
--rw-r--r--   0        0        0    29032 2023-05-31 13:58:40.367974 dcicutils-7.5.0/dcicutils/env_utils_legacy.py
--rw-r--r--   0        0        0     7541 2023-05-31 13:58:40.367974 dcicutils-7.5.0/dcicutils/es_utils.py
--rw-r--r--   0        0        0     9931 2023-05-31 13:58:40.367974 dcicutils-7.5.0/dcicutils/exceptions.py
--rw-r--r--   0        0        0    36918 2023-05-31 13:58:40.367974 dcicutils-7.5.0/dcicutils/ff_mocks.py
--rw-r--r--   0        0        0    66453 2023-05-31 13:58:40.367974 dcicutils-7.5.0/dcicutils/ff_utils.py
--rw-r--r--   0        0        0    10026 2023-05-31 13:58:40.367974 dcicutils-7.5.0/dcicutils/function_cache_decorator.py
--rw-r--r--   0        0        0    33704 2023-05-31 13:58:40.367974 dcicutils-7.5.0/dcicutils/glacier_utils.py
--rw-r--r--   0        0        0    11502 2023-05-31 13:58:40.367974 dcicutils-7.5.0/dcicutils/jh_utils.py
--rw-r--r--   0        0        0    16225 2023-05-31 13:58:40.367974 dcicutils-7.5.0/dcicutils/kibana/dashboards.json
--rw-r--r--   0        0        0     2164 2023-05-31 13:58:40.367974 dcicutils-7.5.0/dcicutils/kibana/readme.md
--rw-r--r--   0        0        0    27661 2023-05-31 13:58:40.367974 dcicutils-7.5.0/dcicutils/lang_utils.py
--rw-r--r--   0        0        0    10883 2023-05-31 13:58:40.367974 dcicutils-7.5.0/dcicutils/log_utils.py
--rw-r--r--   0        0        0    90749 2023-05-31 13:58:40.367974 dcicutils-7.5.0/dcicutils/misc_utils.py
--rw-r--r--   0        0        0     5963 2023-05-31 13:58:40.367974 dcicutils-7.5.0/dcicutils/obfuscation_utils.py
--rw-r--r--   0        0        0     1017 2023-05-31 13:58:40.367974 dcicutils-7.5.0/dcicutils/opensearch_utils.py
--rw-r--r--   0        0        0    30631 2023-05-31 13:58:40.367974 dcicutils-7.5.0/dcicutils/project_utils.py
--rw-r--r--   0        0        0    20234 2023-05-31 13:58:40.367974 dcicutils-7.5.0/dcicutils/qa_checkers.py
--rw-r--r--   0        0        0   156269 2023-05-31 13:58:40.371974 dcicutils-7.5.0/dcicutils/qa_utils.py
--rw-r--r--   0        0        0     6509 2023-05-31 13:58:40.371974 dcicutils-7.5.0/dcicutils/redis_tools.py
--rw-r--r--   0        0        0     6462 2023-05-31 13:58:40.371974 dcicutils-7.5.0/dcicutils/redis_utils.py
--rw-r--r--   0        0        0    28852 2023-05-31 13:58:40.371974 dcicutils-7.5.0/dcicutils/s3_utils.py
--rw-r--r--   0        0        0    12767 2023-05-31 13:58:40.371974 dcicutils-7.5.0/dcicutils/scripts/publish_to_pypi.py
--rw-r--r--   0        0        0    19745 2023-05-31 13:58:40.371974 dcicutils-7.5.0/dcicutils/secrets_utils.py
--rw-r--r--   0        0        0    22961 2023-05-31 13:58:40.371974 dcicutils-7.5.0/dcicutils/snapshot_utils.py
--rw-r--r--   0        0        0     9707 2023-05-31 13:58:40.371974 dcicutils-7.5.0/dcicutils/ssl_certificate_utils.py
--rw-r--r--   0        0        0     8082 2023-05-31 13:58:40.371974 dcicutils-7.5.0/dcicutils/task_utils.py
--rw-r--r--   0        0        0     1769 2023-05-31 13:58:40.371974 dcicutils-7.5.0/dcicutils/trace_utils.py
--rw-r--r--   0        0        0     3945 2023-05-31 13:58:40.371974 dcicutils-7.5.0/pyproject.toml
--rw-r--r--   0        0        0     2660 1970-01-01 00:00:00.000000 dcicutils-7.5.0/setup.py
--rw-r--r--   0        0        0     2998 1970-01-01 00:00:00.000000 dcicutils-7.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1098 2023-06-07 19:41:06.461298 dcicutils-7.5.1/LICENSE.txt
+-rw-r--r--   0        0        0     1166 2023-06-07 19:41:06.461298 dcicutils-7.5.1/README.rst
+-rw-r--r--   0        0        0        0 2023-06-07 19:41:06.461298 dcicutils-7.5.1/dcicutils/__init__.py
+-rw-r--r--   0        0        0     5115 2023-06-07 19:41:06.461298 dcicutils-7.5.1/dcicutils/base.py
+-rwxr-xr-x   0        0        0    51434 2023-06-07 19:41:06.461298 dcicutils-7.5.1/dcicutils/beanstalk_utils.py
+-rw-r--r--   0        0        0    13786 2023-06-07 19:41:06.461298 dcicutils-7.5.1/dcicutils/cloudformation_utils.py
+-rw-r--r--   0        0        0     1155 2023-06-07 19:41:06.461298 dcicutils-7.5.1/dcicutils/codebuild_utils.py
+-rw-r--r--   0        0        0    15285 2023-06-07 19:41:06.461298 dcicutils-7.5.1/dcicutils/command_utils.py
+-rw-r--r--   0        0        0     3723 2023-06-07 19:41:06.461298 dcicutils-7.5.1/dcicutils/common.py
+-rw-r--r--   0        0        0    11032 2023-06-07 19:41:06.461298 dcicutils-7.5.1/dcicutils/creds_utils.py
+-rw-r--r--   0        0        0     3098 2023-06-07 19:41:06.461298 dcicutils-7.5.1/dcicutils/data_utils.py
+-rw-r--r--   0        0        0    68354 2023-06-07 19:41:06.461298 dcicutils-7.5.1/dcicutils/deployment_utils.py
+-rw-r--r--   0        0        0     8118 2023-06-07 19:41:06.461298 dcicutils-7.5.1/dcicutils/diff_utils.py
+-rw-r--r--   0        0        0     1747 2023-06-07 19:41:06.461298 dcicutils-7.5.1/dcicutils/docker_utils.py
+-rw-r--r--   0        0        0    19474 2023-06-07 19:41:06.461298 dcicutils-7.5.1/dcicutils/ecr_scripts.py
+-rw-r--r--   0        0        0    13079 2023-06-07 19:41:06.461298 dcicutils-7.5.1/dcicutils/ecr_utils.py
+-rw-r--r--   0        0        0     3590 2023-06-07 19:41:06.461298 dcicutils-7.5.1/dcicutils/ecs_utils.py
+-rw-r--r--   0        0        0     6356 2023-06-07 19:41:06.461298 dcicutils-7.5.1/dcicutils/env_base.py
+-rw-r--r--   0        0        0     9444 2023-06-07 19:41:06.461298 dcicutils-7.5.1/dcicutils/env_manager.py
+-rw-r--r--   0        0        0     3909 2023-06-07 19:41:06.461298 dcicutils-7.5.1/dcicutils/env_scripts.py
+-rw-r--r--   0        0        0    46739 2023-06-07 19:41:06.461298 dcicutils-7.5.1/dcicutils/env_utils.py
+-rw-r--r--   0        0        0    29032 2023-06-07 19:41:06.461298 dcicutils-7.5.1/dcicutils/env_utils_legacy.py
+-rw-r--r--   0        0        0     7541 2023-06-07 19:41:06.461298 dcicutils-7.5.1/dcicutils/es_utils.py
+-rw-r--r--   0        0        0     9931 2023-06-07 19:41:06.461298 dcicutils-7.5.1/dcicutils/exceptions.py
+-rw-r--r--   0        0        0    36918 2023-06-07 19:41:06.461298 dcicutils-7.5.1/dcicutils/ff_mocks.py
+-rw-r--r--   0        0        0    66453 2023-06-07 19:41:06.461298 dcicutils-7.5.1/dcicutils/ff_utils.py
+-rw-r--r--   0        0        0    10026 2023-06-07 19:41:06.461298 dcicutils-7.5.1/dcicutils/function_cache_decorator.py
+-rw-r--r--   0        0        0    33704 2023-06-07 19:41:06.461298 dcicutils-7.5.1/dcicutils/glacier_utils.py
+-rw-r--r--   0        0        0    11502 2023-06-07 19:41:06.461298 dcicutils-7.5.1/dcicutils/jh_utils.py
+-rw-r--r--   0        0        0    16225 2023-06-07 19:41:06.461298 dcicutils-7.5.1/dcicutils/kibana/dashboards.json
+-rw-r--r--   0        0        0     2164 2023-06-07 19:41:06.461298 dcicutils-7.5.1/dcicutils/kibana/readme.md
+-rw-r--r--   0        0        0    27661 2023-06-07 19:41:06.461298 dcicutils-7.5.1/dcicutils/lang_utils.py
+-rw-r--r--   0        0        0    10883 2023-06-07 19:41:06.465298 dcicutils-7.5.1/dcicutils/log_utils.py
+-rw-r--r--   0        0        0    90749 2023-06-07 19:41:06.465298 dcicutils-7.5.1/dcicutils/misc_utils.py
+-rw-r--r--   0        0        0     5963 2023-06-07 19:41:06.465298 dcicutils-7.5.1/dcicutils/obfuscation_utils.py
+-rw-r--r--   0        0        0     1017 2023-06-07 19:41:06.465298 dcicutils-7.5.1/dcicutils/opensearch_utils.py
+-rw-r--r--   0        0        0    30631 2023-06-07 19:41:06.465298 dcicutils-7.5.1/dcicutils/project_utils.py
+-rw-r--r--   0        0        0    20234 2023-06-07 19:41:06.465298 dcicutils-7.5.1/dcicutils/qa_checkers.py
+-rw-r--r--   0        0        0   156269 2023-06-07 19:41:06.465298 dcicutils-7.5.1/dcicutils/qa_utils.py
+-rw-r--r--   0        0        0     6509 2023-06-07 19:41:06.465298 dcicutils-7.5.1/dcicutils/redis_tools.py
+-rw-r--r--   0        0        0     6462 2023-06-07 19:41:06.465298 dcicutils-7.5.1/dcicutils/redis_utils.py
+-rw-r--r--   0        0        0    28852 2023-06-07 19:41:06.465298 dcicutils-7.5.1/dcicutils/s3_utils.py
+-rw-r--r--   0        0        0    13576 2023-06-07 19:41:06.465298 dcicutils-7.5.1/dcicutils/scripts/publish_to_pypi.py
+-rw-r--r--   0        0        0    19745 2023-06-07 19:41:06.465298 dcicutils-7.5.1/dcicutils/secrets_utils.py
+-rw-r--r--   0        0        0    22961 2023-06-07 19:41:06.465298 dcicutils-7.5.1/dcicutils/snapshot_utils.py
+-rw-r--r--   0        0        0     9707 2023-06-07 19:41:06.465298 dcicutils-7.5.1/dcicutils/ssl_certificate_utils.py
+-rw-r--r--   0        0        0     8082 2023-06-07 19:41:06.465298 dcicutils-7.5.1/dcicutils/task_utils.py
+-rw-r--r--   0        0        0     1769 2023-06-07 19:41:06.465298 dcicutils-7.5.1/dcicutils/trace_utils.py
+-rw-r--r--   0        0        0     3944 2023-06-07 19:41:06.465298 dcicutils-7.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2660 1970-01-01 00:00:00.000000 dcicutils-7.5.1/setup.py
+-rw-r--r--   0        0        0     2998 1970-01-01 00:00:00.000000 dcicutils-7.5.1/PKG-INFO
```

### Comparing `dcicutils-7.5.0/LICENSE.txt` & `dcicutils-7.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.0/README.rst` & `dcicutils-7.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.0/dcicutils/base.py` & `dcicutils-7.5.1/dcicutils/base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.0/dcicutils/beanstalk_utils.py` & `dcicutils-7.5.1/dcicutils/beanstalk_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.0/dcicutils/cloudformation_utils.py` & `dcicutils-7.5.1/dcicutils/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.0/dcicutils/codebuild_utils.py` & `dcicutils-7.5.1/dcicutils/codebuild_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.0/dcicutils/command_utils.py` & `dcicutils-7.5.1/dcicutils/command_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.0/dcicutils/common.py` & `dcicutils-7.5.1/dcicutils/common.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.0/dcicutils/creds_utils.py` & `dcicutils-7.5.1/dcicutils/creds_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.0/dcicutils/data_utils.py` & `dcicutils-7.5.1/dcicutils/data_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.0/dcicutils/deployment_utils.py` & `dcicutils-7.5.1/dcicutils/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.0/dcicutils/diff_utils.py` & `dcicutils-7.5.1/dcicutils/diff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.0/dcicutils/docker_utils.py` & `dcicutils-7.5.1/dcicutils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.0/dcicutils/ecr_scripts.py` & `dcicutils-7.5.1/dcicutils/ecr_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.0/dcicutils/ecr_utils.py` & `dcicutils-7.5.1/dcicutils/ecr_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.0/dcicutils/ecs_utils.py` & `dcicutils-7.5.1/dcicutils/ecs_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.0/dcicutils/env_base.py` & `dcicutils-7.5.1/dcicutils/env_base.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.0/dcicutils/env_manager.py` & `dcicutils-7.5.1/dcicutils/env_manager.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.0/dcicutils/env_scripts.py` & `dcicutils-7.5.1/dcicutils/env_scripts.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.0/dcicutils/env_utils.py` & `dcicutils-7.5.1/dcicutils/env_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.0/dcicutils/env_utils_legacy.py` & `dcicutils-7.5.1/dcicutils/env_utils_legacy.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.0/dcicutils/es_utils.py` & `dcicutils-7.5.1/dcicutils/es_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.0/dcicutils/exceptions.py` & `dcicutils-7.5.1/dcicutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.0/dcicutils/ff_mocks.py` & `dcicutils-7.5.1/dcicutils/ff_mocks.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.0/dcicutils/ff_utils.py` & `dcicutils-7.5.1/dcicutils/ff_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.0/dcicutils/function_cache_decorator.py` & `dcicutils-7.5.1/dcicutils/function_cache_decorator.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.0/dcicutils/glacier_utils.py` & `dcicutils-7.5.1/dcicutils/glacier_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.0/dcicutils/jh_utils.py` & `dcicutils-7.5.1/dcicutils/jh_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.0/dcicutils/kibana/dashboards.json` & `dcicutils-7.5.1/dcicutils/kibana/dashboards.json`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.0/dcicutils/kibana/readme.md` & `dcicutils-7.5.1/dcicutils/kibana/readme.md`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.0/dcicutils/lang_utils.py` & `dcicutils-7.5.1/dcicutils/lang_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.0/dcicutils/log_utils.py` & `dcicutils-7.5.1/dcicutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.0/dcicutils/misc_utils.py` & `dcicutils-7.5.1/dcicutils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.0/dcicutils/obfuscation_utils.py` & `dcicutils-7.5.1/dcicutils/obfuscation_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.0/dcicutils/opensearch_utils.py` & `dcicutils-7.5.1/dcicutils/opensearch_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.0/dcicutils/project_utils.py` & `dcicutils-7.5.1/dcicutils/project_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.0/dcicutils/qa_checkers.py` & `dcicutils-7.5.1/dcicutils/qa_checkers.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.0/dcicutils/qa_utils.py` & `dcicutils-7.5.1/dcicutils/qa_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.0/dcicutils/redis_tools.py` & `dcicutils-7.5.1/dcicutils/redis_tools.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.0/dcicutils/redis_utils.py` & `dcicutils-7.5.1/dcicutils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.0/dcicutils/s3_utils.py` & `dcicutils-7.5.1/dcicutils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.0/dcicutils/scripts/publish_to_pypi.py` & `dcicutils-7.5.1/dcicutils/scripts/publish_to_pypi.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,27 +35,29 @@
 import subprocess
 import toml
 
 from typing import Tuple, Union
 
 
 PYPI_BASE_URL = "https://pypi.org"
+PYPI_API_TOKEN_USERNAME = "__token__"
 DEBUG = False
 
 
 def main() -> None:
 
     def is_github_actions_context():
         return "GITHUB_ACTIONS" in os.environ
 
     argp = argparse.ArgumentParser()
     argp.add_argument("--noconfirm", required=False, dest="noconfirm", action="store_true")
     argp.add_argument("--debug", required=False, dest="debug", action="store_true")
     argp.add_argument("--username", required=False, dest="username")
     argp.add_argument("--password", required=False, dest="password")
+    argp.add_argument("--force-allow-username", required=False, action="store_true")
     args = argp.parse_args()
 
     if args.debug:
         global DEBUG
         DEBUG = True
 
     if args.noconfirm and not is_github_actions_context():
@@ -88,30 +90,35 @@
 
     if not args.noconfirm:
         if not answered_yes_to_confirmation(f"Do you want to publish {package_name} {package_version} to PyPi?"):
             exit_with_no_action()
 
     PRINT(f"Publishing {package_name} {package_version} to PyPi ...")
 
-    if not publish_package(args.username, args.password):
+    if not publish_package(args.username, args.password, args.force_allow_username):
         exit_with_no_action()
 
     PRINT(f"Publishing {package_name} {package_version} to PyPi complete.")
 
 
-def publish_package(pypi_username: str = None, pypi_password: str = None) -> bool:
+def publish_package(pypi_username: str = None, pypi_password: str = None, force_allow_username: bool = False) -> bool:
     if not pypi_username:
         pypi_username = os.environ.get("PYPI_USER")
     if not pypi_password:
         pypi_password = os.environ.get("PYPI_PASSWORD")
     if not pypi_username or not pypi_password:
         ERROR_PRINT(f"No PyPi credentials; you should set the PYPI_USER and PYPI_PASSWORD environment variables.")
         return False
-    if pypi_username != "__token__":
-        WARNING_PRINT(f"Publishing with username/pasword is deprecated; should use be using API token instead.")
+    if pypi_username != PYPI_API_TOKEN_USERNAME:
+        if not force_allow_username:
+            # Just in case someone really really needs this we will allow for now: --force-allow-username
+            ERROR_PRINT(f"Publishing with username/pasword is no longer allowed; must use API token instead.")
+            return False
+        WARNING_PRINT(f"Publishing with username/pasword is NOT recommmended; use API token instead;"
+                      f"only allowing because you said: --force-allow-username")
     poetry_publish_command = [
         "poetry", "publish",
         "--no-interaction", "--build",
         f"--username={pypi_username}", f"--password={pypi_password}"
     ]
     poetry_publish_results, status_code = execute_command(poetry_publish_command)
     PRINT("\n".join(poetry_publish_results))
@@ -252,40 +259,47 @@
     return package_version
 
 
 def get_package_name() -> str:
     """
     Returns the base name of the current git repo name.
     """
-    package_name, _ = execute_command("git config --get remote.origin.url")
-    package_name = os.path.basename(package_name[0])
-    if package_name.endswith(".git"):
-        package_name = package_name[:-4]
-    return package_name
+    # No, the package name should come from pyproject.toml not from the git repo name ...
+    # package_name, _ = execute_command("git config --get remote.origin.url")
+    # package_name = os.path.basename(package_name[0])
+    # if package_name.endswith(".git"):
+    #     package_name = package_name[:-4]
+    # return package_name
+    pyproject_toml = get_pyproject_toml()
+    return pyproject_toml["tool"]["poetry"]["name"]
 
 
 def get_package_directories() -> list:
     """
     Returns a list of directories constituting the Python package of the current repo,
     according to the pyproject.toml file.
     """
     package_directories = []
-    with open("pyproject.toml", "r") as f:
-        pyproject_toml = toml.load(f)
+    pyproject_toml = get_pyproject_toml()
     pyproject_package_directories = pyproject_toml["tool"]["poetry"]["packages"]
     for pyproject_package_directory in pyproject_package_directories:
         package_directory = pyproject_package_directory.get("include")
         if package_directory:
             package_directory_from = pyproject_package_directory.get("from")
             if package_directory_from:
                 package_directory = os.path.join(package_directory_from, package_directory)
             package_directories.append(package_directory)
     return package_directories
 
 
+def get_pyproject_toml() -> list:
+    with open("pyproject.toml", "r") as f:
+        return toml.load(f)
+
+
 def execute_command(command_argv: Union[list, str], lines_containing: str = None) -> Tuple[list, int]:
     """
     Executes the given command as a command-line subprocess, and returns a tuple whose first element
     is the list of lines from the output of the command, and the second element is the exit status code.
     """
     def cleanup_funny_output(output: str) -> str:
         return output.replace("('", "").replace("',)", "").replace("\\n\\n", "\n").replace("\\n", "\n")
```

### Comparing `dcicutils-7.5.0/dcicutils/secrets_utils.py` & `dcicutils-7.5.1/dcicutils/secrets_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.0/dcicutils/snapshot_utils.py` & `dcicutils-7.5.1/dcicutils/snapshot_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.0/dcicutils/ssl_certificate_utils.py` & `dcicutils-7.5.1/dcicutils/ssl_certificate_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.0/dcicutils/task_utils.py` & `dcicutils-7.5.1/dcicutils/task_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.0/dcicutils/trace_utils.py` & `dcicutils-7.5.1/dcicutils/trace_utils.py`

 * *Files identical despite different names*

### Comparing `dcicutils-7.5.0/pyproject.toml` & `dcicutils-7.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcicutils"
-version = "7.5.0" 
+version = "7.5.1"
 description = "Utility package for interacting with the 4DN Data Portal and other 4DN resources"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/4dn-dcic/utils"
 repository = "https://github.com/4dn-dcic/utils"
 packages = [
```

### Comparing `dcicutils-7.5.0/setup.py` & `dcicutils-7.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 entry_points = \
 {'console_scripts': ['publish-to-pypi = '
                      'dcicutils.scripts.publish_to_pypi:main']}
 
 setup_kwargs = {
     'name': 'dcicutils',
-    'version': '7.5.0',
+    'version': '7.5.1',
     'description': 'Utility package for interacting with the 4DN Data Portal and other 4DN resources',
     'long_description': '=====\nutils\n=====\n\nCheck out our full documentation `here <https://dcic-utils.readthedocs.io/en/latest/>`_\n\nThis repository contains various utility modules shared amongst several projects in the 4DN-DCIC. It is meant to be used internally by the DCIC team and externally as a Python API to `Fourfront <https://data.4dnucleome.org>`_\\ , the 4DN data portal.\n\npip installable as the ``dcicutils`` package with: ``pip install dcicutils``\n\nSee `this document <https://dcic-utils.readthedocs.io/en/latest/getting_started.html>`_ for tips on getting started. `Go here <https://dcic-utils.readthedocs.io/en/latest/examples.html>`_ for examples of some of the most useful functions.\n\n\n.. image:: https://travis-ci.org/4dn-dcic/utils.svg?branch=master\n   :target: https://travis-ci.org/4dn-dcic/utils\n   :alt: Build Status\n\n\n.. image:: https://coveralls.io/repos/github/4dn-dcic/utils/badge.svg?branch=master\n   :target: https://coveralls.io/github/4dn-dcic/utils?branch=master\n   :alt: Coverage\n\n.. image:: https://readthedocs.org/projects/dcic-utils/badge/?version=latest\n   :target: https://dcic-utils.readthedocs.io/en/latest/?badge=latest\n   :alt: Documentation Status\n',
     'author': '4DN-DCIC Team',
     'author_email': 'support@4dnucleome.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/4dn-dcic/utils',
```

### Comparing `dcicutils-7.5.0/PKG-INFO` & `dcicutils-7.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcicutils
-Version: 7.5.0
+Version: 7.5.1
 Summary: Utility package for interacting with the 4DN Data Portal and other 4DN resources
 Home-page: https://github.com/4dn-dcic/utils
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7,<3.10
 Classifier: Development Status :: 4 - Beta
```

