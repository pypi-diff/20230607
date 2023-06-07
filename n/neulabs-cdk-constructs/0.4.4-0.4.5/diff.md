# Comparing `tmp/neulabs-cdk-constructs-0.4.4.tar.gz` & `tmp/neulabs-cdk-constructs-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neulabs-cdk-constructs-0.4.4.tar", last modified: Mon May 29 10:06:04 2023, max compression
+gzip compressed data, was "neulabs-cdk-constructs-0.4.5.tar", last modified: Wed Jun  7 14:53:31 2023, max compression
```

## Comparing `neulabs-cdk-constructs-0.4.4.tar` & `neulabs-cdk-constructs-0.4.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:06:04.826568 neulabs-cdk-constructs-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-29 10:05:49.000000 neulabs-cdk-constructs-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-29 10:05:49.000000 neulabs-cdk-constructs-0.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-05-29 10:06:04.826568 neulabs-cdk-constructs-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-05-29 10:05:49.000000 neulabs-cdk-constructs-0.4.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-29 10:05:49.000000 neulabs-cdk-constructs-0.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 10:06:04.830568 neulabs-cdk-constructs-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-29 10:05:49.000000 neulabs-cdk-constructs-0.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:06:04.822569 neulabs-cdk-constructs-0.4.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:06:04.826568 neulabs-cdk-constructs-0.4.4/src/neulabs_cdk_constructs/
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-05-29 10:05:49.000000 neulabs-cdk-constructs-0.4.4/src/neulabs_cdk_constructs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:06:04.826568 neulabs-cdk-constructs-0.4.4/src/neulabs_cdk_constructs/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-29 10:05:49.000000 neulabs-cdk-constructs-0.4.4/src/neulabs_cdk_constructs/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   100993 2023-05-29 10:05:49.000000 neulabs-cdk-constructs-0.4.4/src/neulabs_cdk_constructs/_jsii/neulabs-cdk-constructs@0.4.4.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:06:04.826568 neulabs-cdk-constructs-0.4.4/src/neulabs_cdk_constructs/aws_lambda/
--rw-r--r--   0 runner    (1001) docker     (123)   221164 2023-05-29 10:05:49.000000 neulabs-cdk-constructs-0.4.4/src/neulabs_cdk_constructs/aws_lambda/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:06:04.826568 neulabs-cdk-constructs-0.4.4/src/neulabs_cdk_constructs/newrelic/
--rw-r--r--   0 runner    (1001) docker     (123)    40572 2023-05-29 10:05:49.000000 neulabs-cdk-constructs-0.4.4/src/neulabs_cdk_constructs/newrelic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:06:04.826568 neulabs-cdk-constructs-0.4.4/src/neulabs_cdk_constructs/oidc/
--rw-r--r--   0 runner    (1001) docker     (123)    45448 2023-05-29 10:05:49.000000 neulabs-cdk-constructs-0.4.4/src/neulabs_cdk_constructs/oidc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 10:05:49.000000 neulabs-cdk-constructs-0.4.4/src/neulabs_cdk_constructs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:06:04.826568 neulabs-cdk-constructs-0.4.4/src/neulabs_cdk_constructs/stack/
--rw-r--r--   0 runner    (1001) docker     (123)    24368 2023-05-29 10:05:49.000000 neulabs-cdk-constructs-0.4.4/src/neulabs_cdk_constructs/stack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:06:04.826568 neulabs-cdk-constructs-0.4.4/src/neulabs_cdk_constructs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-05-29 10:05:49.000000 neulabs-cdk-constructs-0.4.4/src/neulabs_cdk_constructs/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:06:04.826568 neulabs-cdk-constructs-0.4.4/src/neulabs_cdk_constructs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-05-29 10:06:04.000000 neulabs-cdk-constructs-0.4.4/src/neulabs_cdk_constructs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-29 10:06:04.000000 neulabs-cdk-constructs-0.4.4/src/neulabs_cdk_constructs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 10:06:04.000000 neulabs-cdk-constructs-0.4.4/src/neulabs_cdk_constructs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-29 10:06:04.000000 neulabs-cdk-constructs-0.4.4/src/neulabs_cdk_constructs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-29 10:06:04.000000 neulabs-cdk-constructs-0.4.4/src/neulabs_cdk_constructs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:53:31.246003 neulabs-cdk-constructs-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-07 14:53:18.000000 neulabs-cdk-constructs-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-07 14:53:18.000000 neulabs-cdk-constructs-0.4.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-06-07 14:53:31.246003 neulabs-cdk-constructs-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-06-07 14:53:18.000000 neulabs-cdk-constructs-0.4.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-07 14:53:18.000000 neulabs-cdk-constructs-0.4.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 14:53:31.246003 neulabs-cdk-constructs-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-07 14:53:18.000000 neulabs-cdk-constructs-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:53:31.242003 neulabs-cdk-constructs-0.4.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:53:31.242003 neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-06-07 14:53:18.000000 neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:53:31.242003 neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-07 14:53:18.000000 neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115223 2023-06-07 14:53:18.000000 neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs/_jsii/neulabs-cdk-constructs@0.4.5.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:53:31.242003 neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs/aws_lambda/
+-rw-r--r--   0 runner    (1001) docker     (123)   299578 2023-06-07 14:53:18.000000 neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs/aws_lambda/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:53:31.242003 neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs/newrelic/
+-rw-r--r--   0 runner    (1001) docker     (123)    40572 2023-06-07 14:53:18.000000 neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs/newrelic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:53:31.242003 neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs/oidc/
+-rw-r--r--   0 runner    (1001) docker     (123)    45448 2023-06-07 14:53:18.000000 neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs/oidc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 14:53:18.000000 neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:53:31.242003 neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs/stack/
+-rw-r--r--   0 runner    (1001) docker     (123)    24368 2023-06-07 14:53:18.000000 neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs/stack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:53:31.242003 neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-06-07 14:53:18.000000 neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:53:31.242003 neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-06-07 14:53:31.000000 neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-07 14:53:31.000000 neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 14:53:31.000000 neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-07 14:53:31.000000 neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-07 14:53:31.000000 neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs.egg-info/top_level.txt
```

### Comparing `neulabs-cdk-constructs-0.4.4/LICENSE` & `neulabs-cdk-constructs-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.4.4/PKG-INFO` & `neulabs-cdk-constructs-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neulabs-cdk-constructs
-Version: 0.4.4
+Version: 0.4.5
 Summary: neulabs-cdk-constructs
 Home-page: https://github.com/neulabscom/neulabs-cdk-constructs.git
 Author: Neulabs<tech@neulabs.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/neulabscom/neulabs-cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `neulabs-cdk-constructs-0.4.4/README.md` & `neulabs-cdk-constructs-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.4.4/setup.py` & `neulabs-cdk-constructs-0.4.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "neulabs-cdk-constructs",
-    "version": "0.4.4",
+    "version": "0.4.5",
     "description": "neulabs-cdk-constructs",
     "license": "Apache-2.0",
     "url": "https://github.com/neulabscom/neulabs-cdk-constructs.git",
     "long_description_content_type": "text/markdown",
     "author": "Neulabs<tech@neulabs.com>",
     "bdist_wheel": {
         "universal": true
@@ -27,25 +27,25 @@
         "neulabs_cdk_constructs.newrelic",
         "neulabs_cdk_constructs.oidc",
         "neulabs_cdk_constructs.stack",
         "neulabs_cdk_constructs.utils"
     ],
     "package_data": {
         "neulabs_cdk_constructs._jsii": [
-            "neulabs-cdk-constructs@0.4.4.jsii.tgz"
+            "neulabs-cdk-constructs@0.4.5.jsii.tgz"
         ],
         "neulabs_cdk_constructs": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "aws-cdk-lib==2.78.0",
-        "aws-cdk.aws-apigatewayv2-alpha==2.78.0.a0",
-        "aws-cdk.aws-apigatewayv2-integrations-alpha==2.78.0.a0",
+        "aws-cdk-lib==2.82.0",
+        "aws-cdk.aws-apigatewayv2-alpha==2.82.0.a0",
+        "aws-cdk.aws-apigatewayv2-integrations-alpha==2.82.0.a0",
         "constructs>=10.0.0, <11.0.0",
         "jsii>=1.82.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
```

### Comparing `neulabs-cdk-constructs-0.4.4/src/neulabs_cdk_constructs/__init__.py` & `neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.4.4/src/neulabs_cdk_constructs/_jsii/__init__.py` & `neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs/_jsii/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 import aws_cdk._jsii
 import aws_cdk.aws_apigatewayv2_alpha._jsii
 import aws_cdk.aws_apigatewayv2_integrations_alpha._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "neulabs-cdk-constructs",
-    "0.4.4",
+    "0.4.5",
     __name__[0:-6],
-    "neulabs-cdk-constructs@0.4.4.jsii.tgz",
+    "neulabs-cdk-constructs@0.4.5.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `neulabs-cdk-constructs-0.4.4/src/neulabs_cdk_constructs/aws_lambda/__init__.py` & `neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs/aws_lambda/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -2210,14 +2210,192 @@
             on_success=on_success,
             retry_attempts=retry_attempts,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
 
+class NewRelicFunctionNode(
+    FunctionNode,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="neulabs-cdk-constructs.aws_lambda.NewRelicFunctionNode",
+):
+    def __init__(
+        self,
+        scope: _constructs_77d1e7e8.Construct,
+        id: builtins.str,
+        *,
+        new_relic_account_id: builtins.str,
+        new_relic_layer_name: builtins.str,
+        new_relic_layer_version: jsii.Number,
+        new_relicwith_extension_send_logs: typing.Optional[builtins.bool] = None,
+        stage: builtins.str,
+        with_base_environment: typing.Optional[builtins.bool] = None,
+        with_base_tags: typing.Optional[builtins.bool] = None,
+        aws_sdk_connection_reuse: typing.Optional[builtins.bool] = None,
+        bundling: typing.Optional[typing.Union[_aws_cdk_aws_lambda_nodejs_ceddda9d.BundlingOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+        deps_lock_file_path: typing.Optional[builtins.str] = None,
+        entry: typing.Optional[builtins.str] = None,
+        handler: typing.Optional[builtins.str] = None,
+        project_root: typing.Optional[builtins.str] = None,
+        runtime: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.Runtime] = None,
+        adot_instrumentation: typing.Optional[typing.Union[_aws_cdk_aws_lambda_ceddda9d.AdotInstrumentationConfig, typing.Dict[builtins.str, typing.Any]]] = None,
+        allow_all_outbound: typing.Optional[builtins.bool] = None,
+        allow_public_subnet: typing.Optional[builtins.bool] = None,
+        architecture: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.Architecture] = None,
+        code_signing_config: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.ICodeSigningConfig] = None,
+        current_version_options: typing.Optional[typing.Union[_aws_cdk_aws_lambda_ceddda9d.VersionOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+        dead_letter_queue: typing.Optional[_aws_cdk_aws_sqs_ceddda9d.IQueue] = None,
+        dead_letter_queue_enabled: typing.Optional[builtins.bool] = None,
+        dead_letter_topic: typing.Optional[_aws_cdk_aws_sns_ceddda9d.ITopic] = None,
+        description: typing.Optional[builtins.str] = None,
+        environment: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+        environment_encryption: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
+        ephemeral_storage_size: typing.Optional[_aws_cdk_ceddda9d.Size] = None,
+        events: typing.Optional[typing.Sequence[_aws_cdk_aws_lambda_ceddda9d.IEventSource]] = None,
+        filesystem: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.FileSystem] = None,
+        function_name: typing.Optional[builtins.str] = None,
+        initial_policy: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
+        insights_version: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.LambdaInsightsVersion] = None,
+        layers: typing.Optional[typing.Sequence[_aws_cdk_aws_lambda_ceddda9d.ILayerVersion]] = None,
+        log_retention: typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays] = None,
+        log_retention_retry_options: typing.Optional[typing.Union[_aws_cdk_aws_lambda_ceddda9d.LogRetentionRetryOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+        log_retention_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
+        memory_size: typing.Optional[jsii.Number] = None,
+        profiling: typing.Optional[builtins.bool] = None,
+        profiling_group: typing.Optional[_aws_cdk_aws_codeguruprofiler_ceddda9d.IProfilingGroup] = None,
+        reserved_concurrent_executions: typing.Optional[jsii.Number] = None,
+        role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
+        runtime_management_mode: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.RuntimeManagementMode] = None,
+        security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
+        timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
+        tracing: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.Tracing] = None,
+        vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
+        vpc_subnets: typing.Optional[typing.Union[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection, typing.Dict[builtins.str, typing.Any]]] = None,
+        max_event_age: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
+        on_failure: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.IDestination] = None,
+        on_success: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.IDestination] = None,
+        retry_attempts: typing.Optional[jsii.Number] = None,
+    ) -> None:
+        '''
+        :param scope: -
+        :param id: -
+        :param new_relic_account_id: 
+        :param new_relic_layer_name: 
+        :param new_relic_layer_version: 
+        :param new_relicwith_extension_send_logs: 
+        :param stage: 
+        :param with_base_environment: 
+        :param with_base_tags: 
+        :param aws_sdk_connection_reuse: Whether to automatically reuse TCP connections when working with the AWS SDK for JavaScript. This sets the ``AWS_NODEJS_CONNECTION_REUSE_ENABLED`` environment variable to ``1``. Default: true
+        :param bundling: Bundling options. Default: - use default bundling options: no minify, no sourcemap, all modules are bundled.
+        :param deps_lock_file_path: The path to the dependencies lock file (``yarn.lock``, ``pnpm-lock.yaml`` or ``package-lock.json``). This will be used as the source for the volume mounted in the Docker container. Modules specified in ``nodeModules`` will be installed using the right installer (``yarn``, ``pnpm`` or ``npm``) along with this lock file. Default: - the path is found by walking up parent directories searching for a ``yarn.lock``, ``pnpm-lock.yaml`` or ``package-lock.json`` file
+        :param entry: Path to the entry file (JavaScript or TypeScript). Default: - Derived from the name of the defining file and the construct's id. If the ``NodejsFunction`` is defined in ``stack.ts`` with ``my-handler`` as id (``new NodejsFunction(this, 'my-handler')``), the construct will look at ``stack.my-handler.ts`` and ``stack.my-handler.js``.
+        :param handler: The name of the exported handler in the entry file. The handler is prefixed with ``index.`` unless the specified handler value contains a ``.``, in which case it is used as-is. Default: handler
+        :param project_root: The path to the directory containing project config files (``package.json`` or ``tsconfig.json``). Default: - the directory containing the ``depsLockFilePath``
+        :param runtime: The runtime environment. Only runtimes of the Node.js family are supported. Default: Runtime.NODEJS_14_X
+        :param adot_instrumentation: Specify the configuration of AWS Distro for OpenTelemetry (ADOT) instrumentation. Default: - No ADOT instrumentation
+        :param allow_all_outbound: Whether to allow the Lambda to send all network traffic. If set to false, you must individually add traffic rules to allow the Lambda to connect to network targets. Default: true
+        :param allow_public_subnet: Lambda Functions in a public subnet can NOT access the internet. Use this property to acknowledge this limitation and still place the function in a public subnet. Default: false
+        :param architecture: The system architectures compatible with this lambda function. Default: Architecture.X86_64
+        :param code_signing_config: Code signing config associated with this function. Default: - Not Sign the Code
+        :param current_version_options: Options for the ``lambda.Version`` resource automatically created by the ``fn.currentVersion`` method. Default: - default options as described in ``VersionOptions``
+        :param dead_letter_queue: The SQS queue to use if DLQ is enabled. If SNS topic is desired, specify ``deadLetterTopic`` property instead. Default: - SQS queue with 14 day retention period if ``deadLetterQueueEnabled`` is ``true``
+        :param dead_letter_queue_enabled: Enabled DLQ. If ``deadLetterQueue`` is undefined, an SQS queue with default options will be defined for your Function. Default: - false unless ``deadLetterQueue`` is set, which implies DLQ is enabled.
+        :param dead_letter_topic: The SNS topic to use as a DLQ. Note that if ``deadLetterQueueEnabled`` is set to ``true``, an SQS queue will be created rather than an SNS topic. Using an SNS topic as a DLQ requires this property to be set explicitly. Default: - no SNS topic
+        :param description: A description of the function. Default: - No description.
+        :param environment: Key-value pairs that Lambda caches and makes available for your Lambda functions. Use environment variables to apply configuration changes, such as test and production environment configurations, without changing your Lambda function source code. Default: - No environment variables.
+        :param environment_encryption: The AWS KMS key that's used to encrypt your function's environment variables. Default: - AWS Lambda creates and uses an AWS managed customer master key (CMK).
+        :param ephemeral_storage_size: The size of the function’s /tmp directory in MiB. Default: 512 MiB
+        :param events: Event sources for this function. You can also add event sources using ``addEventSource``. Default: - No event sources.
+        :param filesystem: The filesystem configuration for the lambda function. Default: - will not mount any filesystem
+        :param function_name: A name for the function. Default: - AWS CloudFormation generates a unique physical ID and uses that ID for the function's name. For more information, see Name Type.
+        :param initial_policy: Initial policy statements to add to the created Lambda Role. You can call ``addToRolePolicy`` to the created lambda to add statements post creation. Default: - No policy statements are added to the created Lambda role.
+        :param insights_version: Specify the version of CloudWatch Lambda insights to use for monitoring. Default: - No Lambda Insights
+        :param layers: A list of layers to add to the function's execution environment. You can configure your Lambda function to pull in additional code during initialization in the form of layers. Layers are packages of libraries or other dependencies that can be used by multiple functions. Default: - No layers.
+        :param log_retention: The number of days log events are kept in CloudWatch Logs. When updating this property, unsetting it doesn't remove the log retention policy. To remove the retention policy, set the value to ``INFINITE``. Default: logs.RetentionDays.INFINITE
+        :param log_retention_retry_options: When log retention is specified, a custom resource attempts to create the CloudWatch log group. These options control the retry policy when interacting with CloudWatch APIs. Default: - Default AWS SDK retry options.
+        :param log_retention_role: The IAM role for the Lambda function associated with the custom resource that sets the retention policy. Default: - A new role is created.
+        :param memory_size: The amount of memory, in MB, that is allocated to your Lambda function. Lambda uses this value to proportionally allocate the amount of CPU power. For more information, see Resource Model in the AWS Lambda Developer Guide. Default: 128
+        :param profiling: Enable profiling. Default: - No profiling.
+        :param profiling_group: Profiling Group. Default: - A new profiling group will be created if ``profiling`` is set.
+        :param reserved_concurrent_executions: The maximum of concurrent executions you want to reserve for the function. Default: - No specific limit - account limit.
+        :param role: Lambda execution role. This is the role that will be assumed by the function upon execution. It controls the permissions that the function will have. The Role must be assumable by the 'lambda.amazonaws.com' service principal. The default Role automatically has permissions granted for Lambda execution. If you provide a Role, you must add the relevant AWS managed policies yourself. The relevant managed policies are "service-role/AWSLambdaBasicExecutionRole" and "service-role/AWSLambdaVPCAccessExecutionRole". Default: - A unique role will be generated for this lambda function. Both supplied and generated roles can always be changed by calling ``addToRolePolicy``.
+        :param runtime_management_mode: Sets the runtime management configuration for a function's version. Default: Auto
+        :param security_groups: The list of security groups to associate with the Lambda's network interfaces. Only used if 'vpc' is supplied. Default: - If the function is placed within a VPC and a security group is not specified, either by this or securityGroup prop, a dedicated security group will be created for this function.
+        :param timeout: The function execution time (in seconds) after which Lambda terminates the function. Because the execution time affects cost, set this value based on the function's expected execution time. Default: Duration.seconds(3)
+        :param tracing: Enable AWS X-Ray Tracing for Lambda Function. Default: Tracing.Disabled
+        :param vpc: VPC network to place Lambda network interfaces. Specify this if the Lambda function needs to access resources in a VPC. This is required when ``vpcSubnets`` is specified. Default: - Function is not placed within a VPC.
+        :param vpc_subnets: Where to place the network interfaces within the VPC. This requires ``vpc`` to be specified in order for interfaces to actually be placed in the subnets. If ``vpc`` is not specify, this will raise an error. Note: Internet access for Lambda Functions requires a NAT Gateway, so picking public subnets is not allowed (unless ``allowPublicSubnet`` is set to ``true``). Default: - the Vpc default strategy if not specified
+        :param max_event_age: The maximum age of a request that Lambda sends to a function for processing. Minimum: 60 seconds Maximum: 6 hours Default: Duration.hours(6)
+        :param on_failure: The destination for failed invocations. Default: - no destination
+        :param on_success: The destination for successful invocations. Default: - no destination
+        :param retry_attempts: The maximum number of times to retry when the function returns an error. Minimum: 0 Maximum: 2 Default: 2
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__b0d58974e5f5a337faa6fb1a15de86db2d61e9b089cfd2d4a2af9eff7761b643)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+        props = FunctionNodeNewRelicProps(
+            new_relic_account_id=new_relic_account_id,
+            new_relic_layer_name=new_relic_layer_name,
+            new_relic_layer_version=new_relic_layer_version,
+            new_relicwith_extension_send_logs=new_relicwith_extension_send_logs,
+            stage=stage,
+            with_base_environment=with_base_environment,
+            with_base_tags=with_base_tags,
+            aws_sdk_connection_reuse=aws_sdk_connection_reuse,
+            bundling=bundling,
+            deps_lock_file_path=deps_lock_file_path,
+            entry=entry,
+            handler=handler,
+            project_root=project_root,
+            runtime=runtime,
+            adot_instrumentation=adot_instrumentation,
+            allow_all_outbound=allow_all_outbound,
+            allow_public_subnet=allow_public_subnet,
+            architecture=architecture,
+            code_signing_config=code_signing_config,
+            current_version_options=current_version_options,
+            dead_letter_queue=dead_letter_queue,
+            dead_letter_queue_enabled=dead_letter_queue_enabled,
+            dead_letter_topic=dead_letter_topic,
+            description=description,
+            environment=environment,
+            environment_encryption=environment_encryption,
+            ephemeral_storage_size=ephemeral_storage_size,
+            events=events,
+            filesystem=filesystem,
+            function_name=function_name,
+            initial_policy=initial_policy,
+            insights_version=insights_version,
+            layers=layers,
+            log_retention=log_retention,
+            log_retention_retry_options=log_retention_retry_options,
+            log_retention_role=log_retention_role,
+            memory_size=memory_size,
+            profiling=profiling,
+            profiling_group=profiling_group,
+            reserved_concurrent_executions=reserved_concurrent_executions,
+            role=role,
+            runtime_management_mode=runtime_management_mode,
+            security_groups=security_groups,
+            timeout=timeout,
+            tracing=tracing,
+            vpc=vpc,
+            vpc_subnets=vpc_subnets,
+            max_event_age=max_event_age,
+            on_failure=on_failure,
+            on_success=on_success,
+            retry_attempts=retry_attempts,
+        )
+
+        jsii.create(self.__class__, self, [scope, id, props])
+
+
 @jsii.data_type(
     jsii_type="neulabs-cdk-constructs.aws_lambda.NewRelicProps",
     jsii_struct_bases=[],
     name_mapping={
         "handler": "handler",
         "new_relic_account_id": "newRelicAccountId",
         "new_relic_layer_name": "newRelicLayerName",
@@ -3138,21 +3316,945 @@
 
     def __repr__(self) -> str:
         return "FunctionNewRelicProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
+@jsii.data_type(
+    jsii_type="neulabs-cdk-constructs.aws_lambda.FunctionNodeNewRelicProps",
+    jsii_struct_bases=[FunctionNodeProps],
+    name_mapping={
+        "max_event_age": "maxEventAge",
+        "on_failure": "onFailure",
+        "on_success": "onSuccess",
+        "retry_attempts": "retryAttempts",
+        "adot_instrumentation": "adotInstrumentation",
+        "allow_all_outbound": "allowAllOutbound",
+        "allow_public_subnet": "allowPublicSubnet",
+        "architecture": "architecture",
+        "code_signing_config": "codeSigningConfig",
+        "current_version_options": "currentVersionOptions",
+        "dead_letter_queue": "deadLetterQueue",
+        "dead_letter_queue_enabled": "deadLetterQueueEnabled",
+        "dead_letter_topic": "deadLetterTopic",
+        "description": "description",
+        "environment": "environment",
+        "environment_encryption": "environmentEncryption",
+        "ephemeral_storage_size": "ephemeralStorageSize",
+        "events": "events",
+        "filesystem": "filesystem",
+        "function_name": "functionName",
+        "initial_policy": "initialPolicy",
+        "insights_version": "insightsVersion",
+        "layers": "layers",
+        "log_retention": "logRetention",
+        "log_retention_retry_options": "logRetentionRetryOptions",
+        "log_retention_role": "logRetentionRole",
+        "memory_size": "memorySize",
+        "profiling": "profiling",
+        "profiling_group": "profilingGroup",
+        "reserved_concurrent_executions": "reservedConcurrentExecutions",
+        "role": "role",
+        "runtime_management_mode": "runtimeManagementMode",
+        "security_groups": "securityGroups",
+        "timeout": "timeout",
+        "tracing": "tracing",
+        "vpc": "vpc",
+        "vpc_subnets": "vpcSubnets",
+        "aws_sdk_connection_reuse": "awsSdkConnectionReuse",
+        "bundling": "bundling",
+        "deps_lock_file_path": "depsLockFilePath",
+        "entry": "entry",
+        "handler": "handler",
+        "project_root": "projectRoot",
+        "runtime": "runtime",
+        "stage": "stage",
+        "with_base_environment": "withBaseEnvironment",
+        "with_base_tags": "withBaseTags",
+        "new_relic_account_id": "newRelicAccountId",
+        "new_relic_layer_name": "newRelicLayerName",
+        "new_relic_layer_version": "newRelicLayerVersion",
+        "new_relicwith_extension_send_logs": "newRelicwithExtensionSendLogs",
+    },
+)
+class FunctionNodeNewRelicProps(FunctionNodeProps):
+    def __init__(
+        self,
+        *,
+        max_event_age: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
+        on_failure: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.IDestination] = None,
+        on_success: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.IDestination] = None,
+        retry_attempts: typing.Optional[jsii.Number] = None,
+        adot_instrumentation: typing.Optional[typing.Union[_aws_cdk_aws_lambda_ceddda9d.AdotInstrumentationConfig, typing.Dict[builtins.str, typing.Any]]] = None,
+        allow_all_outbound: typing.Optional[builtins.bool] = None,
+        allow_public_subnet: typing.Optional[builtins.bool] = None,
+        architecture: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.Architecture] = None,
+        code_signing_config: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.ICodeSigningConfig] = None,
+        current_version_options: typing.Optional[typing.Union[_aws_cdk_aws_lambda_ceddda9d.VersionOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+        dead_letter_queue: typing.Optional[_aws_cdk_aws_sqs_ceddda9d.IQueue] = None,
+        dead_letter_queue_enabled: typing.Optional[builtins.bool] = None,
+        dead_letter_topic: typing.Optional[_aws_cdk_aws_sns_ceddda9d.ITopic] = None,
+        description: typing.Optional[builtins.str] = None,
+        environment: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+        environment_encryption: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
+        ephemeral_storage_size: typing.Optional[_aws_cdk_ceddda9d.Size] = None,
+        events: typing.Optional[typing.Sequence[_aws_cdk_aws_lambda_ceddda9d.IEventSource]] = None,
+        filesystem: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.FileSystem] = None,
+        function_name: typing.Optional[builtins.str] = None,
+        initial_policy: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
+        insights_version: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.LambdaInsightsVersion] = None,
+        layers: typing.Optional[typing.Sequence[_aws_cdk_aws_lambda_ceddda9d.ILayerVersion]] = None,
+        log_retention: typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays] = None,
+        log_retention_retry_options: typing.Optional[typing.Union[_aws_cdk_aws_lambda_ceddda9d.LogRetentionRetryOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+        log_retention_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
+        memory_size: typing.Optional[jsii.Number] = None,
+        profiling: typing.Optional[builtins.bool] = None,
+        profiling_group: typing.Optional[_aws_cdk_aws_codeguruprofiler_ceddda9d.IProfilingGroup] = None,
+        reserved_concurrent_executions: typing.Optional[jsii.Number] = None,
+        role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
+        runtime_management_mode: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.RuntimeManagementMode] = None,
+        security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
+        timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
+        tracing: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.Tracing] = None,
+        vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
+        vpc_subnets: typing.Optional[typing.Union[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection, typing.Dict[builtins.str, typing.Any]]] = None,
+        aws_sdk_connection_reuse: typing.Optional[builtins.bool] = None,
+        bundling: typing.Optional[typing.Union[_aws_cdk_aws_lambda_nodejs_ceddda9d.BundlingOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+        deps_lock_file_path: typing.Optional[builtins.str] = None,
+        entry: typing.Optional[builtins.str] = None,
+        handler: typing.Optional[builtins.str] = None,
+        project_root: typing.Optional[builtins.str] = None,
+        runtime: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.Runtime] = None,
+        stage: builtins.str,
+        with_base_environment: typing.Optional[builtins.bool] = None,
+        with_base_tags: typing.Optional[builtins.bool] = None,
+        new_relic_account_id: builtins.str,
+        new_relic_layer_name: builtins.str,
+        new_relic_layer_version: jsii.Number,
+        new_relicwith_extension_send_logs: typing.Optional[builtins.bool] = None,
+    ) -> None:
+        '''
+        :param max_event_age: The maximum age of a request that Lambda sends to a function for processing. Minimum: 60 seconds Maximum: 6 hours Default: Duration.hours(6)
+        :param on_failure: The destination for failed invocations. Default: - no destination
+        :param on_success: The destination for successful invocations. Default: - no destination
+        :param retry_attempts: The maximum number of times to retry when the function returns an error. Minimum: 0 Maximum: 2 Default: 2
+        :param adot_instrumentation: Specify the configuration of AWS Distro for OpenTelemetry (ADOT) instrumentation. Default: - No ADOT instrumentation
+        :param allow_all_outbound: Whether to allow the Lambda to send all network traffic. If set to false, you must individually add traffic rules to allow the Lambda to connect to network targets. Default: true
+        :param allow_public_subnet: Lambda Functions in a public subnet can NOT access the internet. Use this property to acknowledge this limitation and still place the function in a public subnet. Default: false
+        :param architecture: The system architectures compatible with this lambda function. Default: Architecture.X86_64
+        :param code_signing_config: Code signing config associated with this function. Default: - Not Sign the Code
+        :param current_version_options: Options for the ``lambda.Version`` resource automatically created by the ``fn.currentVersion`` method. Default: - default options as described in ``VersionOptions``
+        :param dead_letter_queue: The SQS queue to use if DLQ is enabled. If SNS topic is desired, specify ``deadLetterTopic`` property instead. Default: - SQS queue with 14 day retention period if ``deadLetterQueueEnabled`` is ``true``
+        :param dead_letter_queue_enabled: Enabled DLQ. If ``deadLetterQueue`` is undefined, an SQS queue with default options will be defined for your Function. Default: - false unless ``deadLetterQueue`` is set, which implies DLQ is enabled.
+        :param dead_letter_topic: The SNS topic to use as a DLQ. Note that if ``deadLetterQueueEnabled`` is set to ``true``, an SQS queue will be created rather than an SNS topic. Using an SNS topic as a DLQ requires this property to be set explicitly. Default: - no SNS topic
+        :param description: A description of the function. Default: - No description.
+        :param environment: Key-value pairs that Lambda caches and makes available for your Lambda functions. Use environment variables to apply configuration changes, such as test and production environment configurations, without changing your Lambda function source code. Default: - No environment variables.
+        :param environment_encryption: The AWS KMS key that's used to encrypt your function's environment variables. Default: - AWS Lambda creates and uses an AWS managed customer master key (CMK).
+        :param ephemeral_storage_size: The size of the function’s /tmp directory in MiB. Default: 512 MiB
+        :param events: Event sources for this function. You can also add event sources using ``addEventSource``. Default: - No event sources.
+        :param filesystem: The filesystem configuration for the lambda function. Default: - will not mount any filesystem
+        :param function_name: A name for the function. Default: - AWS CloudFormation generates a unique physical ID and uses that ID for the function's name. For more information, see Name Type.
+        :param initial_policy: Initial policy statements to add to the created Lambda Role. You can call ``addToRolePolicy`` to the created lambda to add statements post creation. Default: - No policy statements are added to the created Lambda role.
+        :param insights_version: Specify the version of CloudWatch Lambda insights to use for monitoring. Default: - No Lambda Insights
+        :param layers: A list of layers to add to the function's execution environment. You can configure your Lambda function to pull in additional code during initialization in the form of layers. Layers are packages of libraries or other dependencies that can be used by multiple functions. Default: - No layers.
+        :param log_retention: The number of days log events are kept in CloudWatch Logs. When updating this property, unsetting it doesn't remove the log retention policy. To remove the retention policy, set the value to ``INFINITE``. Default: logs.RetentionDays.INFINITE
+        :param log_retention_retry_options: When log retention is specified, a custom resource attempts to create the CloudWatch log group. These options control the retry policy when interacting with CloudWatch APIs. Default: - Default AWS SDK retry options.
+        :param log_retention_role: The IAM role for the Lambda function associated with the custom resource that sets the retention policy. Default: - A new role is created.
+        :param memory_size: The amount of memory, in MB, that is allocated to your Lambda function. Lambda uses this value to proportionally allocate the amount of CPU power. For more information, see Resource Model in the AWS Lambda Developer Guide. Default: 128
+        :param profiling: Enable profiling. Default: - No profiling.
+        :param profiling_group: Profiling Group. Default: - A new profiling group will be created if ``profiling`` is set.
+        :param reserved_concurrent_executions: The maximum of concurrent executions you want to reserve for the function. Default: - No specific limit - account limit.
+        :param role: Lambda execution role. This is the role that will be assumed by the function upon execution. It controls the permissions that the function will have. The Role must be assumable by the 'lambda.amazonaws.com' service principal. The default Role automatically has permissions granted for Lambda execution. If you provide a Role, you must add the relevant AWS managed policies yourself. The relevant managed policies are "service-role/AWSLambdaBasicExecutionRole" and "service-role/AWSLambdaVPCAccessExecutionRole". Default: - A unique role will be generated for this lambda function. Both supplied and generated roles can always be changed by calling ``addToRolePolicy``.
+        :param runtime_management_mode: Sets the runtime management configuration for a function's version. Default: Auto
+        :param security_groups: The list of security groups to associate with the Lambda's network interfaces. Only used if 'vpc' is supplied. Default: - If the function is placed within a VPC and a security group is not specified, either by this or securityGroup prop, a dedicated security group will be created for this function.
+        :param timeout: The function execution time (in seconds) after which Lambda terminates the function. Because the execution time affects cost, set this value based on the function's expected execution time. Default: Duration.seconds(3)
+        :param tracing: Enable AWS X-Ray Tracing for Lambda Function. Default: Tracing.Disabled
+        :param vpc: VPC network to place Lambda network interfaces. Specify this if the Lambda function needs to access resources in a VPC. This is required when ``vpcSubnets`` is specified. Default: - Function is not placed within a VPC.
+        :param vpc_subnets: Where to place the network interfaces within the VPC. This requires ``vpc`` to be specified in order for interfaces to actually be placed in the subnets. If ``vpc`` is not specify, this will raise an error. Note: Internet access for Lambda Functions requires a NAT Gateway, so picking public subnets is not allowed (unless ``allowPublicSubnet`` is set to ``true``). Default: - the Vpc default strategy if not specified
+        :param aws_sdk_connection_reuse: Whether to automatically reuse TCP connections when working with the AWS SDK for JavaScript. This sets the ``AWS_NODEJS_CONNECTION_REUSE_ENABLED`` environment variable to ``1``. Default: true
+        :param bundling: Bundling options. Default: - use default bundling options: no minify, no sourcemap, all modules are bundled.
+        :param deps_lock_file_path: The path to the dependencies lock file (``yarn.lock``, ``pnpm-lock.yaml`` or ``package-lock.json``). This will be used as the source for the volume mounted in the Docker container. Modules specified in ``nodeModules`` will be installed using the right installer (``yarn``, ``pnpm`` or ``npm``) along with this lock file. Default: - the path is found by walking up parent directories searching for a ``yarn.lock``, ``pnpm-lock.yaml`` or ``package-lock.json`` file
+        :param entry: Path to the entry file (JavaScript or TypeScript). Default: - Derived from the name of the defining file and the construct's id. If the ``NodejsFunction`` is defined in ``stack.ts`` with ``my-handler`` as id (``new NodejsFunction(this, 'my-handler')``), the construct will look at ``stack.my-handler.ts`` and ``stack.my-handler.js``.
+        :param handler: The name of the exported handler in the entry file. The handler is prefixed with ``index.`` unless the specified handler value contains a ``.``, in which case it is used as-is. Default: handler
+        :param project_root: The path to the directory containing project config files (``package.json`` or ``tsconfig.json``). Default: - the directory containing the ``depsLockFilePath``
+        :param runtime: The runtime environment. Only runtimes of the Node.js family are supported. Default: Runtime.NODEJS_14_X
+        :param stage: 
+        :param with_base_environment: 
+        :param with_base_tags: 
+        :param new_relic_account_id: 
+        :param new_relic_layer_name: 
+        :param new_relic_layer_version: 
+        :param new_relicwith_extension_send_logs: 
+        '''
+        if isinstance(adot_instrumentation, dict):
+            adot_instrumentation = _aws_cdk_aws_lambda_ceddda9d.AdotInstrumentationConfig(**adot_instrumentation)
+        if isinstance(current_version_options, dict):
+            current_version_options = _aws_cdk_aws_lambda_ceddda9d.VersionOptions(**current_version_options)
+        if isinstance(log_retention_retry_options, dict):
+            log_retention_retry_options = _aws_cdk_aws_lambda_ceddda9d.LogRetentionRetryOptions(**log_retention_retry_options)
+        if isinstance(vpc_subnets, dict):
+            vpc_subnets = _aws_cdk_aws_ec2_ceddda9d.SubnetSelection(**vpc_subnets)
+        if isinstance(bundling, dict):
+            bundling = _aws_cdk_aws_lambda_nodejs_ceddda9d.BundlingOptions(**bundling)
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__8213adbac9e19e0b3d755ffb9f07652b9bfc13f0ae2e707f94b0a29dac983629)
+            check_type(argname="argument max_event_age", value=max_event_age, expected_type=type_hints["max_event_age"])
+            check_type(argname="argument on_failure", value=on_failure, expected_type=type_hints["on_failure"])
+            check_type(argname="argument on_success", value=on_success, expected_type=type_hints["on_success"])
+            check_type(argname="argument retry_attempts", value=retry_attempts, expected_type=type_hints["retry_attempts"])
+            check_type(argname="argument adot_instrumentation", value=adot_instrumentation, expected_type=type_hints["adot_instrumentation"])
+            check_type(argname="argument allow_all_outbound", value=allow_all_outbound, expected_type=type_hints["allow_all_outbound"])
+            check_type(argname="argument allow_public_subnet", value=allow_public_subnet, expected_type=type_hints["allow_public_subnet"])
+            check_type(argname="argument architecture", value=architecture, expected_type=type_hints["architecture"])
+            check_type(argname="argument code_signing_config", value=code_signing_config, expected_type=type_hints["code_signing_config"])
+            check_type(argname="argument current_version_options", value=current_version_options, expected_type=type_hints["current_version_options"])
+            check_type(argname="argument dead_letter_queue", value=dead_letter_queue, expected_type=type_hints["dead_letter_queue"])
+            check_type(argname="argument dead_letter_queue_enabled", value=dead_letter_queue_enabled, expected_type=type_hints["dead_letter_queue_enabled"])
+            check_type(argname="argument dead_letter_topic", value=dead_letter_topic, expected_type=type_hints["dead_letter_topic"])
+            check_type(argname="argument description", value=description, expected_type=type_hints["description"])
+            check_type(argname="argument environment", value=environment, expected_type=type_hints["environment"])
+            check_type(argname="argument environment_encryption", value=environment_encryption, expected_type=type_hints["environment_encryption"])
+            check_type(argname="argument ephemeral_storage_size", value=ephemeral_storage_size, expected_type=type_hints["ephemeral_storage_size"])
+            check_type(argname="argument events", value=events, expected_type=type_hints["events"])
+            check_type(argname="argument filesystem", value=filesystem, expected_type=type_hints["filesystem"])
+            check_type(argname="argument function_name", value=function_name, expected_type=type_hints["function_name"])
+            check_type(argname="argument initial_policy", value=initial_policy, expected_type=type_hints["initial_policy"])
+            check_type(argname="argument insights_version", value=insights_version, expected_type=type_hints["insights_version"])
+            check_type(argname="argument layers", value=layers, expected_type=type_hints["layers"])
+            check_type(argname="argument log_retention", value=log_retention, expected_type=type_hints["log_retention"])
+            check_type(argname="argument log_retention_retry_options", value=log_retention_retry_options, expected_type=type_hints["log_retention_retry_options"])
+            check_type(argname="argument log_retention_role", value=log_retention_role, expected_type=type_hints["log_retention_role"])
+            check_type(argname="argument memory_size", value=memory_size, expected_type=type_hints["memory_size"])
+            check_type(argname="argument profiling", value=profiling, expected_type=type_hints["profiling"])
+            check_type(argname="argument profiling_group", value=profiling_group, expected_type=type_hints["profiling_group"])
+            check_type(argname="argument reserved_concurrent_executions", value=reserved_concurrent_executions, expected_type=type_hints["reserved_concurrent_executions"])
+            check_type(argname="argument role", value=role, expected_type=type_hints["role"])
+            check_type(argname="argument runtime_management_mode", value=runtime_management_mode, expected_type=type_hints["runtime_management_mode"])
+            check_type(argname="argument security_groups", value=security_groups, expected_type=type_hints["security_groups"])
+            check_type(argname="argument timeout", value=timeout, expected_type=type_hints["timeout"])
+            check_type(argname="argument tracing", value=tracing, expected_type=type_hints["tracing"])
+            check_type(argname="argument vpc", value=vpc, expected_type=type_hints["vpc"])
+            check_type(argname="argument vpc_subnets", value=vpc_subnets, expected_type=type_hints["vpc_subnets"])
+            check_type(argname="argument aws_sdk_connection_reuse", value=aws_sdk_connection_reuse, expected_type=type_hints["aws_sdk_connection_reuse"])
+            check_type(argname="argument bundling", value=bundling, expected_type=type_hints["bundling"])
+            check_type(argname="argument deps_lock_file_path", value=deps_lock_file_path, expected_type=type_hints["deps_lock_file_path"])
+            check_type(argname="argument entry", value=entry, expected_type=type_hints["entry"])
+            check_type(argname="argument handler", value=handler, expected_type=type_hints["handler"])
+            check_type(argname="argument project_root", value=project_root, expected_type=type_hints["project_root"])
+            check_type(argname="argument runtime", value=runtime, expected_type=type_hints["runtime"])
+            check_type(argname="argument stage", value=stage, expected_type=type_hints["stage"])
+            check_type(argname="argument with_base_environment", value=with_base_environment, expected_type=type_hints["with_base_environment"])
+            check_type(argname="argument with_base_tags", value=with_base_tags, expected_type=type_hints["with_base_tags"])
+            check_type(argname="argument new_relic_account_id", value=new_relic_account_id, expected_type=type_hints["new_relic_account_id"])
+            check_type(argname="argument new_relic_layer_name", value=new_relic_layer_name, expected_type=type_hints["new_relic_layer_name"])
+            check_type(argname="argument new_relic_layer_version", value=new_relic_layer_version, expected_type=type_hints["new_relic_layer_version"])
+            check_type(argname="argument new_relicwith_extension_send_logs", value=new_relicwith_extension_send_logs, expected_type=type_hints["new_relicwith_extension_send_logs"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "stage": stage,
+            "new_relic_account_id": new_relic_account_id,
+            "new_relic_layer_name": new_relic_layer_name,
+            "new_relic_layer_version": new_relic_layer_version,
+        }
+        if max_event_age is not None:
+            self._values["max_event_age"] = max_event_age
+        if on_failure is not None:
+            self._values["on_failure"] = on_failure
+        if on_success is not None:
+            self._values["on_success"] = on_success
+        if retry_attempts is not None:
+            self._values["retry_attempts"] = retry_attempts
+        if adot_instrumentation is not None:
+            self._values["adot_instrumentation"] = adot_instrumentation
+        if allow_all_outbound is not None:
+            self._values["allow_all_outbound"] = allow_all_outbound
+        if allow_public_subnet is not None:
+            self._values["allow_public_subnet"] = allow_public_subnet
+        if architecture is not None:
+            self._values["architecture"] = architecture
+        if code_signing_config is not None:
+            self._values["code_signing_config"] = code_signing_config
+        if current_version_options is not None:
+            self._values["current_version_options"] = current_version_options
+        if dead_letter_queue is not None:
+            self._values["dead_letter_queue"] = dead_letter_queue
+        if dead_letter_queue_enabled is not None:
+            self._values["dead_letter_queue_enabled"] = dead_letter_queue_enabled
+        if dead_letter_topic is not None:
+            self._values["dead_letter_topic"] = dead_letter_topic
+        if description is not None:
+            self._values["description"] = description
+        if environment is not None:
+            self._values["environment"] = environment
+        if environment_encryption is not None:
+            self._values["environment_encryption"] = environment_encryption
+        if ephemeral_storage_size is not None:
+            self._values["ephemeral_storage_size"] = ephemeral_storage_size
+        if events is not None:
+            self._values["events"] = events
+        if filesystem is not None:
+            self._values["filesystem"] = filesystem
+        if function_name is not None:
+            self._values["function_name"] = function_name
+        if initial_policy is not None:
+            self._values["initial_policy"] = initial_policy
+        if insights_version is not None:
+            self._values["insights_version"] = insights_version
+        if layers is not None:
+            self._values["layers"] = layers
+        if log_retention is not None:
+            self._values["log_retention"] = log_retention
+        if log_retention_retry_options is not None:
+            self._values["log_retention_retry_options"] = log_retention_retry_options
+        if log_retention_role is not None:
+            self._values["log_retention_role"] = log_retention_role
+        if memory_size is not None:
+            self._values["memory_size"] = memory_size
+        if profiling is not None:
+            self._values["profiling"] = profiling
+        if profiling_group is not None:
+            self._values["profiling_group"] = profiling_group
+        if reserved_concurrent_executions is not None:
+            self._values["reserved_concurrent_executions"] = reserved_concurrent_executions
+        if role is not None:
+            self._values["role"] = role
+        if runtime_management_mode is not None:
+            self._values["runtime_management_mode"] = runtime_management_mode
+        if security_groups is not None:
+            self._values["security_groups"] = security_groups
+        if timeout is not None:
+            self._values["timeout"] = timeout
+        if tracing is not None:
+            self._values["tracing"] = tracing
+        if vpc is not None:
+            self._values["vpc"] = vpc
+        if vpc_subnets is not None:
+            self._values["vpc_subnets"] = vpc_subnets
+        if aws_sdk_connection_reuse is not None:
+            self._values["aws_sdk_connection_reuse"] = aws_sdk_connection_reuse
+        if bundling is not None:
+            self._values["bundling"] = bundling
+        if deps_lock_file_path is not None:
+            self._values["deps_lock_file_path"] = deps_lock_file_path
+        if entry is not None:
+            self._values["entry"] = entry
+        if handler is not None:
+            self._values["handler"] = handler
+        if project_root is not None:
+            self._values["project_root"] = project_root
+        if runtime is not None:
+            self._values["runtime"] = runtime
+        if with_base_environment is not None:
+            self._values["with_base_environment"] = with_base_environment
+        if with_base_tags is not None:
+            self._values["with_base_tags"] = with_base_tags
+        if new_relicwith_extension_send_logs is not None:
+            self._values["new_relicwith_extension_send_logs"] = new_relicwith_extension_send_logs
+
+    @builtins.property
+    def max_event_age(self) -> typing.Optional[_aws_cdk_ceddda9d.Duration]:
+        '''The maximum age of a request that Lambda sends to a function for processing.
+
+        Minimum: 60 seconds
+        Maximum: 6 hours
+
+        :default: Duration.hours(6)
+        '''
+        result = self._values.get("max_event_age")
+        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.Duration], result)
+
+    @builtins.property
+    def on_failure(self) -> typing.Optional[_aws_cdk_aws_lambda_ceddda9d.IDestination]:
+        '''The destination for failed invocations.
+
+        :default: - no destination
+        '''
+        result = self._values.get("on_failure")
+        return typing.cast(typing.Optional[_aws_cdk_aws_lambda_ceddda9d.IDestination], result)
+
+    @builtins.property
+    def on_success(self) -> typing.Optional[_aws_cdk_aws_lambda_ceddda9d.IDestination]:
+        '''The destination for successful invocations.
+
+        :default: - no destination
+        '''
+        result = self._values.get("on_success")
+        return typing.cast(typing.Optional[_aws_cdk_aws_lambda_ceddda9d.IDestination], result)
+
+    @builtins.property
+    def retry_attempts(self) -> typing.Optional[jsii.Number]:
+        '''The maximum number of times to retry when the function returns an error.
+
+        Minimum: 0
+        Maximum: 2
+
+        :default: 2
+        '''
+        result = self._values.get("retry_attempts")
+        return typing.cast(typing.Optional[jsii.Number], result)
+
+    @builtins.property
+    def adot_instrumentation(
+        self,
+    ) -> typing.Optional[_aws_cdk_aws_lambda_ceddda9d.AdotInstrumentationConfig]:
+        '''Specify the configuration of AWS Distro for OpenTelemetry (ADOT) instrumentation.
+
+        :default: - No ADOT instrumentation
+
+        :see: https://aws-otel.github.io/docs/getting-started/lambda
+        '''
+        result = self._values.get("adot_instrumentation")
+        return typing.cast(typing.Optional[_aws_cdk_aws_lambda_ceddda9d.AdotInstrumentationConfig], result)
+
+    @builtins.property
+    def allow_all_outbound(self) -> typing.Optional[builtins.bool]:
+        '''Whether to allow the Lambda to send all network traffic.
+
+        If set to false, you must individually add traffic rules to allow the
+        Lambda to connect to network targets.
+
+        :default: true
+        '''
+        result = self._values.get("allow_all_outbound")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def allow_public_subnet(self) -> typing.Optional[builtins.bool]:
+        '''Lambda Functions in a public subnet can NOT access the internet.
+
+        Use this property to acknowledge this limitation and still place the function in a public subnet.
+
+        :default: false
+
+        :see: https://stackoverflow.com/questions/52992085/why-cant-an-aws-lambda-function-inside-a-public-subnet-in-a-vpc-connect-to-the/52994841#52994841
+        '''
+        result = self._values.get("allow_public_subnet")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def architecture(
+        self,
+    ) -> typing.Optional[_aws_cdk_aws_lambda_ceddda9d.Architecture]:
+        '''The system architectures compatible with this lambda function.
+
+        :default: Architecture.X86_64
+        '''
+        result = self._values.get("architecture")
+        return typing.cast(typing.Optional[_aws_cdk_aws_lambda_ceddda9d.Architecture], result)
+
+    @builtins.property
+    def code_signing_config(
+        self,
+    ) -> typing.Optional[_aws_cdk_aws_lambda_ceddda9d.ICodeSigningConfig]:
+        '''Code signing config associated with this function.
+
+        :default: - Not Sign the Code
+        '''
+        result = self._values.get("code_signing_config")
+        return typing.cast(typing.Optional[_aws_cdk_aws_lambda_ceddda9d.ICodeSigningConfig], result)
+
+    @builtins.property
+    def current_version_options(
+        self,
+    ) -> typing.Optional[_aws_cdk_aws_lambda_ceddda9d.VersionOptions]:
+        '''Options for the ``lambda.Version`` resource automatically created by the ``fn.currentVersion`` method.
+
+        :default: - default options as described in ``VersionOptions``
+        '''
+        result = self._values.get("current_version_options")
+        return typing.cast(typing.Optional[_aws_cdk_aws_lambda_ceddda9d.VersionOptions], result)
+
+    @builtins.property
+    def dead_letter_queue(self) -> typing.Optional[_aws_cdk_aws_sqs_ceddda9d.IQueue]:
+        '''The SQS queue to use if DLQ is enabled.
+
+        If SNS topic is desired, specify ``deadLetterTopic`` property instead.
+
+        :default: - SQS queue with 14 day retention period if ``deadLetterQueueEnabled`` is ``true``
+        '''
+        result = self._values.get("dead_letter_queue")
+        return typing.cast(typing.Optional[_aws_cdk_aws_sqs_ceddda9d.IQueue], result)
+
+    @builtins.property
+    def dead_letter_queue_enabled(self) -> typing.Optional[builtins.bool]:
+        '''Enabled DLQ.
+
+        If ``deadLetterQueue`` is undefined,
+        an SQS queue with default options will be defined for your Function.
+
+        :default: - false unless ``deadLetterQueue`` is set, which implies DLQ is enabled.
+        '''
+        result = self._values.get("dead_letter_queue_enabled")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def dead_letter_topic(self) -> typing.Optional[_aws_cdk_aws_sns_ceddda9d.ITopic]:
+        '''The SNS topic to use as a DLQ.
+
+        Note that if ``deadLetterQueueEnabled`` is set to ``true``, an SQS queue will be created
+        rather than an SNS topic. Using an SNS topic as a DLQ requires this property to be set explicitly.
+
+        :default: - no SNS topic
+        '''
+        result = self._values.get("dead_letter_topic")
+        return typing.cast(typing.Optional[_aws_cdk_aws_sns_ceddda9d.ITopic], result)
+
+    @builtins.property
+    def description(self) -> typing.Optional[builtins.str]:
+        '''A description of the function.
+
+        :default: - No description.
+        '''
+        result = self._values.get("description")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def environment(
+        self,
+    ) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
+        '''Key-value pairs that Lambda caches and makes available for your Lambda functions.
+
+        Use environment variables to apply configuration changes, such
+        as test and production environment configurations, without changing your
+        Lambda function source code.
+
+        :default: - No environment variables.
+        '''
+        result = self._values.get("environment")
+        return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
+
+    @builtins.property
+    def environment_encryption(self) -> typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey]:
+        '''The AWS KMS key that's used to encrypt your function's environment variables.
+
+        :default: - AWS Lambda creates and uses an AWS managed customer master key (CMK).
+        '''
+        result = self._values.get("environment_encryption")
+        return typing.cast(typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey], result)
+
+    @builtins.property
+    def ephemeral_storage_size(self) -> typing.Optional[_aws_cdk_ceddda9d.Size]:
+        '''The size of the function’s /tmp directory in MiB.
+
+        :default: 512 MiB
+        '''
+        result = self._values.get("ephemeral_storage_size")
+        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.Size], result)
+
+    @builtins.property
+    def events(
+        self,
+    ) -> typing.Optional[typing.List[_aws_cdk_aws_lambda_ceddda9d.IEventSource]]:
+        '''Event sources for this function.
+
+        You can also add event sources using ``addEventSource``.
+
+        :default: - No event sources.
+        '''
+        result = self._values.get("events")
+        return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_lambda_ceddda9d.IEventSource]], result)
+
+    @builtins.property
+    def filesystem(self) -> typing.Optional[_aws_cdk_aws_lambda_ceddda9d.FileSystem]:
+        '''The filesystem configuration for the lambda function.
+
+        :default: - will not mount any filesystem
+        '''
+        result = self._values.get("filesystem")
+        return typing.cast(typing.Optional[_aws_cdk_aws_lambda_ceddda9d.FileSystem], result)
+
+    @builtins.property
+    def function_name(self) -> typing.Optional[builtins.str]:
+        '''A name for the function.
+
+        :default:
+
+        - AWS CloudFormation generates a unique physical ID and uses that
+        ID for the function's name. For more information, see Name Type.
+        '''
+        result = self._values.get("function_name")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def initial_policy(
+        self,
+    ) -> typing.Optional[typing.List[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]]:
+        '''Initial policy statements to add to the created Lambda Role.
+
+        You can call ``addToRolePolicy`` to the created lambda to add statements post creation.
+
+        :default: - No policy statements are added to the created Lambda role.
+        '''
+        result = self._values.get("initial_policy")
+        return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]], result)
+
+    @builtins.property
+    def insights_version(
+        self,
+    ) -> typing.Optional[_aws_cdk_aws_lambda_ceddda9d.LambdaInsightsVersion]:
+        '''Specify the version of CloudWatch Lambda insights to use for monitoring.
+
+        :default: - No Lambda Insights
+
+        :see: https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/Lambda-Insights-Getting-Started-docker.html
+        '''
+        result = self._values.get("insights_version")
+        return typing.cast(typing.Optional[_aws_cdk_aws_lambda_ceddda9d.LambdaInsightsVersion], result)
+
+    @builtins.property
+    def layers(
+        self,
+    ) -> typing.Optional[typing.List[_aws_cdk_aws_lambda_ceddda9d.ILayerVersion]]:
+        '''A list of layers to add to the function's execution environment.
+
+        You can configure your Lambda function to pull in
+        additional code during initialization in the form of layers. Layers are packages of libraries or other dependencies
+        that can be used by multiple functions.
+
+        :default: - No layers.
+        '''
+        result = self._values.get("layers")
+        return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_lambda_ceddda9d.ILayerVersion]], result)
+
+    @builtins.property
+    def log_retention(
+        self,
+    ) -> typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays]:
+        '''The number of days log events are kept in CloudWatch Logs.
+
+        When updating
+        this property, unsetting it doesn't remove the log retention policy. To
+        remove the retention policy, set the value to ``INFINITE``.
+
+        :default: logs.RetentionDays.INFINITE
+        '''
+        result = self._values.get("log_retention")
+        return typing.cast(typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays], result)
+
+    @builtins.property
+    def log_retention_retry_options(
+        self,
+    ) -> typing.Optional[_aws_cdk_aws_lambda_ceddda9d.LogRetentionRetryOptions]:
+        '''When log retention is specified, a custom resource attempts to create the CloudWatch log group.
+
+        These options control the retry policy when interacting with CloudWatch APIs.
+
+        :default: - Default AWS SDK retry options.
+        '''
+        result = self._values.get("log_retention_retry_options")
+        return typing.cast(typing.Optional[_aws_cdk_aws_lambda_ceddda9d.LogRetentionRetryOptions], result)
+
+    @builtins.property
+    def log_retention_role(self) -> typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole]:
+        '''The IAM role for the Lambda function associated with the custom resource that sets the retention policy.
+
+        :default: - A new role is created.
+        '''
+        result = self._values.get("log_retention_role")
+        return typing.cast(typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole], result)
+
+    @builtins.property
+    def memory_size(self) -> typing.Optional[jsii.Number]:
+        '''The amount of memory, in MB, that is allocated to your Lambda function.
+
+        Lambda uses this value to proportionally allocate the amount of CPU
+        power. For more information, see Resource Model in the AWS Lambda
+        Developer Guide.
+
+        :default: 128
+        '''
+        result = self._values.get("memory_size")
+        return typing.cast(typing.Optional[jsii.Number], result)
+
+    @builtins.property
+    def profiling(self) -> typing.Optional[builtins.bool]:
+        '''Enable profiling.
+
+        :default: - No profiling.
+
+        :see: https://docs.aws.amazon.com/codeguru/latest/profiler-ug/setting-up-lambda.html
+        '''
+        result = self._values.get("profiling")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def profiling_group(
+        self,
+    ) -> typing.Optional[_aws_cdk_aws_codeguruprofiler_ceddda9d.IProfilingGroup]:
+        '''Profiling Group.
+
+        :default: - A new profiling group will be created if ``profiling`` is set.
+
+        :see: https://docs.aws.amazon.com/codeguru/latest/profiler-ug/setting-up-lambda.html
+        '''
+        result = self._values.get("profiling_group")
+        return typing.cast(typing.Optional[_aws_cdk_aws_codeguruprofiler_ceddda9d.IProfilingGroup], result)
+
+    @builtins.property
+    def reserved_concurrent_executions(self) -> typing.Optional[jsii.Number]:
+        '''The maximum of concurrent executions you want to reserve for the function.
+
+        :default: - No specific limit - account limit.
+
+        :see: https://docs.aws.amazon.com/lambda/latest/dg/concurrent-executions.html
+        '''
+        result = self._values.get("reserved_concurrent_executions")
+        return typing.cast(typing.Optional[jsii.Number], result)
+
+    @builtins.property
+    def role(self) -> typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole]:
+        '''Lambda execution role.
+
+        This is the role that will be assumed by the function upon execution.
+        It controls the permissions that the function will have. The Role must
+        be assumable by the 'lambda.amazonaws.com' service principal.
+
+        The default Role automatically has permissions granted for Lambda execution. If you
+        provide a Role, you must add the relevant AWS managed policies yourself.
+
+        The relevant managed policies are "service-role/AWSLambdaBasicExecutionRole" and
+        "service-role/AWSLambdaVPCAccessExecutionRole".
+
+        :default:
+
+        - A unique role will be generated for this lambda function.
+        Both supplied and generated roles can always be changed by calling ``addToRolePolicy``.
+        '''
+        result = self._values.get("role")
+        return typing.cast(typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole], result)
+
+    @builtins.property
+    def runtime_management_mode(
+        self,
+    ) -> typing.Optional[_aws_cdk_aws_lambda_ceddda9d.RuntimeManagementMode]:
+        '''Sets the runtime management configuration for a function's version.
+
+        :default: Auto
+        '''
+        result = self._values.get("runtime_management_mode")
+        return typing.cast(typing.Optional[_aws_cdk_aws_lambda_ceddda9d.RuntimeManagementMode], result)
+
+    @builtins.property
+    def security_groups(
+        self,
+    ) -> typing.Optional[typing.List[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]]:
+        '''The list of security groups to associate with the Lambda's network interfaces.
+
+        Only used if 'vpc' is supplied.
+
+        :default:
+
+        - If the function is placed within a VPC and a security group is
+        not specified, either by this or securityGroup prop, a dedicated security
+        group will be created for this function.
+        '''
+        result = self._values.get("security_groups")
+        return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]], result)
+
+    @builtins.property
+    def timeout(self) -> typing.Optional[_aws_cdk_ceddda9d.Duration]:
+        '''The function execution time (in seconds) after which Lambda terminates the function.
+
+        Because the execution time affects cost, set this value
+        based on the function's expected execution time.
+
+        :default: Duration.seconds(3)
+        '''
+        result = self._values.get("timeout")
+        return typing.cast(typing.Optional[_aws_cdk_ceddda9d.Duration], result)
+
+    @builtins.property
+    def tracing(self) -> typing.Optional[_aws_cdk_aws_lambda_ceddda9d.Tracing]:
+        '''Enable AWS X-Ray Tracing for Lambda Function.
+
+        :default: Tracing.Disabled
+        '''
+        result = self._values.get("tracing")
+        return typing.cast(typing.Optional[_aws_cdk_aws_lambda_ceddda9d.Tracing], result)
+
+    @builtins.property
+    def vpc(self) -> typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc]:
+        '''VPC network to place Lambda network interfaces.
+
+        Specify this if the Lambda function needs to access resources in a VPC.
+        This is required when ``vpcSubnets`` is specified.
+
+        :default: - Function is not placed within a VPC.
+        '''
+        result = self._values.get("vpc")
+        return typing.cast(typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc], result)
+
+    @builtins.property
+    def vpc_subnets(self) -> typing.Optional[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection]:
+        '''Where to place the network interfaces within the VPC.
+
+        This requires ``vpc`` to be specified in order for interfaces to actually be
+        placed in the subnets. If ``vpc`` is not specify, this will raise an error.
+
+        Note: Internet access for Lambda Functions requires a NAT Gateway, so picking
+        public subnets is not allowed (unless ``allowPublicSubnet`` is set to ``true``).
+
+        :default: - the Vpc default strategy if not specified
+        '''
+        result = self._values.get("vpc_subnets")
+        return typing.cast(typing.Optional[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection], result)
+
+    @builtins.property
+    def aws_sdk_connection_reuse(self) -> typing.Optional[builtins.bool]:
+        '''Whether to automatically reuse TCP connections when working with the AWS SDK for JavaScript.
+
+        This sets the ``AWS_NODEJS_CONNECTION_REUSE_ENABLED`` environment variable
+        to ``1``.
+
+        :default: true
+
+        :see: https://docs.aws.amazon.com/sdk-for-javascript/v2/developer-guide/node-reusing-connections.html
+        '''
+        result = self._values.get("aws_sdk_connection_reuse")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def bundling(
+        self,
+    ) -> typing.Optional[_aws_cdk_aws_lambda_nodejs_ceddda9d.BundlingOptions]:
+        '''Bundling options.
+
+        :default:
+
+        - use default bundling options: no minify, no sourcemap, all
+        modules are bundled.
+        '''
+        result = self._values.get("bundling")
+        return typing.cast(typing.Optional[_aws_cdk_aws_lambda_nodejs_ceddda9d.BundlingOptions], result)
+
+    @builtins.property
+    def deps_lock_file_path(self) -> typing.Optional[builtins.str]:
+        '''The path to the dependencies lock file (``yarn.lock``, ``pnpm-lock.yaml`` or ``package-lock.json``).
+
+        This will be used as the source for the volume mounted in the Docker
+        container.
+
+        Modules specified in ``nodeModules`` will be installed using the right
+        installer (``yarn``, ``pnpm`` or ``npm``) along with this lock file.
+
+        :default:
+
+        - the path is found by walking up parent directories searching for
+        a ``yarn.lock``, ``pnpm-lock.yaml`` or ``package-lock.json`` file
+        '''
+        result = self._values.get("deps_lock_file_path")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def entry(self) -> typing.Optional[builtins.str]:
+        '''Path to the entry file (JavaScript or TypeScript).
+
+        :default:
+
+        - Derived from the name of the defining file and the construct's id.
+        If the ``NodejsFunction`` is defined in ``stack.ts`` with ``my-handler`` as id
+        (``new NodejsFunction(this, 'my-handler')``), the construct will look at ``stack.my-handler.ts``
+        and ``stack.my-handler.js``.
+        '''
+        result = self._values.get("entry")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def handler(self) -> typing.Optional[builtins.str]:
+        '''The name of the exported handler in the entry file.
+
+        The handler is prefixed with ``index.`` unless the specified handler value contains a ``.``,
+        in which case it is used as-is.
+
+        :default: handler
+        '''
+        result = self._values.get("handler")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def project_root(self) -> typing.Optional[builtins.str]:
+        '''The path to the directory containing project config files (``package.json`` or ``tsconfig.json``).
+
+        :default: - the directory containing the ``depsLockFilePath``
+        '''
+        result = self._values.get("project_root")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def runtime(self) -> typing.Optional[_aws_cdk_aws_lambda_ceddda9d.Runtime]:
+        '''The runtime environment.
+
+        Only runtimes of the Node.js family are
+        supported.
+
+        :default: Runtime.NODEJS_14_X
+        '''
+        result = self._values.get("runtime")
+        return typing.cast(typing.Optional[_aws_cdk_aws_lambda_ceddda9d.Runtime], result)
+
+    @builtins.property
+    def stage(self) -> builtins.str:
+        result = self._values.get("stage")
+        assert result is not None, "Required property 'stage' is missing"
+        return typing.cast(builtins.str, result)
+
+    @builtins.property
+    def with_base_environment(self) -> typing.Optional[builtins.bool]:
+        result = self._values.get("with_base_environment")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def with_base_tags(self) -> typing.Optional[builtins.bool]:
+        result = self._values.get("with_base_tags")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
+    def new_relic_account_id(self) -> builtins.str:
+        result = self._values.get("new_relic_account_id")
+        assert result is not None, "Required property 'new_relic_account_id' is missing"
+        return typing.cast(builtins.str, result)
+
+    @builtins.property
+    def new_relic_layer_name(self) -> builtins.str:
+        result = self._values.get("new_relic_layer_name")
+        assert result is not None, "Required property 'new_relic_layer_name' is missing"
+        return typing.cast(builtins.str, result)
+
+    @builtins.property
+    def new_relic_layer_version(self) -> jsii.Number:
+        result = self._values.get("new_relic_layer_version")
+        assert result is not None, "Required property 'new_relic_layer_version' is missing"
+        return typing.cast(jsii.Number, result)
+
+    @builtins.property
+    def new_relicwith_extension_send_logs(self) -> typing.Optional[builtins.bool]:
+        result = self._values.get("new_relicwith_extension_send_logs")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "FunctionNodeNewRelicProps(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
 __all__ = [
     "Function",
     "FunctionNewRelicProps",
     "FunctionNode",
+    "FunctionNodeNewRelicProps",
     "FunctionNodeProps",
     "FunctionProps",
     "NewRelicFunction",
+    "NewRelicFunctionNode",
     "NewRelicProps",
 ]
 
 publication.publish()
 
 def _typecheckingstub__b9727f7ce5c71748cdd3f6195fddab6280bd7bd81c56cc7ce47431c08c8e1c15(
     scope: _constructs_77d1e7e8.Construct,
@@ -3413,14 +4515,73 @@
     on_failure: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.IDestination] = None,
     on_success: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.IDestination] = None,
     retry_attempts: typing.Optional[jsii.Number] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__b0d58974e5f5a337faa6fb1a15de86db2d61e9b089cfd2d4a2af9eff7761b643(
+    scope: _constructs_77d1e7e8.Construct,
+    id: builtins.str,
+    *,
+    new_relic_account_id: builtins.str,
+    new_relic_layer_name: builtins.str,
+    new_relic_layer_version: jsii.Number,
+    new_relicwith_extension_send_logs: typing.Optional[builtins.bool] = None,
+    stage: builtins.str,
+    with_base_environment: typing.Optional[builtins.bool] = None,
+    with_base_tags: typing.Optional[builtins.bool] = None,
+    aws_sdk_connection_reuse: typing.Optional[builtins.bool] = None,
+    bundling: typing.Optional[typing.Union[_aws_cdk_aws_lambda_nodejs_ceddda9d.BundlingOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+    deps_lock_file_path: typing.Optional[builtins.str] = None,
+    entry: typing.Optional[builtins.str] = None,
+    handler: typing.Optional[builtins.str] = None,
+    project_root: typing.Optional[builtins.str] = None,
+    runtime: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.Runtime] = None,
+    adot_instrumentation: typing.Optional[typing.Union[_aws_cdk_aws_lambda_ceddda9d.AdotInstrumentationConfig, typing.Dict[builtins.str, typing.Any]]] = None,
+    allow_all_outbound: typing.Optional[builtins.bool] = None,
+    allow_public_subnet: typing.Optional[builtins.bool] = None,
+    architecture: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.Architecture] = None,
+    code_signing_config: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.ICodeSigningConfig] = None,
+    current_version_options: typing.Optional[typing.Union[_aws_cdk_aws_lambda_ceddda9d.VersionOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+    dead_letter_queue: typing.Optional[_aws_cdk_aws_sqs_ceddda9d.IQueue] = None,
+    dead_letter_queue_enabled: typing.Optional[builtins.bool] = None,
+    dead_letter_topic: typing.Optional[_aws_cdk_aws_sns_ceddda9d.ITopic] = None,
+    description: typing.Optional[builtins.str] = None,
+    environment: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+    environment_encryption: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
+    ephemeral_storage_size: typing.Optional[_aws_cdk_ceddda9d.Size] = None,
+    events: typing.Optional[typing.Sequence[_aws_cdk_aws_lambda_ceddda9d.IEventSource]] = None,
+    filesystem: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.FileSystem] = None,
+    function_name: typing.Optional[builtins.str] = None,
+    initial_policy: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
+    insights_version: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.LambdaInsightsVersion] = None,
+    layers: typing.Optional[typing.Sequence[_aws_cdk_aws_lambda_ceddda9d.ILayerVersion]] = None,
+    log_retention: typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays] = None,
+    log_retention_retry_options: typing.Optional[typing.Union[_aws_cdk_aws_lambda_ceddda9d.LogRetentionRetryOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+    log_retention_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
+    memory_size: typing.Optional[jsii.Number] = None,
+    profiling: typing.Optional[builtins.bool] = None,
+    profiling_group: typing.Optional[_aws_cdk_aws_codeguruprofiler_ceddda9d.IProfilingGroup] = None,
+    reserved_concurrent_executions: typing.Optional[jsii.Number] = None,
+    role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
+    runtime_management_mode: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.RuntimeManagementMode] = None,
+    security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
+    timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
+    tracing: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.Tracing] = None,
+    vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
+    vpc_subnets: typing.Optional[typing.Union[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection, typing.Dict[builtins.str, typing.Any]]] = None,
+    max_event_age: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
+    on_failure: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.IDestination] = None,
+    on_success: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.IDestination] = None,
+    retry_attempts: typing.Optional[jsii.Number] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__b7814149e68cf909ed05655748a5db5ef1654ca712712f23b88372e6aea61cca(
     *,
     handler: builtins.str,
     new_relic_account_id: builtins.str,
     new_relic_layer_name: builtins.str,
     new_relic_layer_version: jsii.Number,
     new_relicwith_extension_send_logs: typing.Optional[builtins.bool] = None,
@@ -3473,10 +4634,67 @@
     stage: builtins.str,
     with_base_environment: typing.Optional[builtins.bool] = None,
     with_base_tags: typing.Optional[builtins.bool] = None,
     new_relic_account_id: builtins.str,
     new_relic_layer_name: builtins.str,
     new_relic_layer_version: jsii.Number,
     new_relicwith_extension_send_logs: typing.Optional[builtins.bool] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__8213adbac9e19e0b3d755ffb9f07652b9bfc13f0ae2e707f94b0a29dac983629(
+    *,
+    max_event_age: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
+    on_failure: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.IDestination] = None,
+    on_success: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.IDestination] = None,
+    retry_attempts: typing.Optional[jsii.Number] = None,
+    adot_instrumentation: typing.Optional[typing.Union[_aws_cdk_aws_lambda_ceddda9d.AdotInstrumentationConfig, typing.Dict[builtins.str, typing.Any]]] = None,
+    allow_all_outbound: typing.Optional[builtins.bool] = None,
+    allow_public_subnet: typing.Optional[builtins.bool] = None,
+    architecture: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.Architecture] = None,
+    code_signing_config: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.ICodeSigningConfig] = None,
+    current_version_options: typing.Optional[typing.Union[_aws_cdk_aws_lambda_ceddda9d.VersionOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+    dead_letter_queue: typing.Optional[_aws_cdk_aws_sqs_ceddda9d.IQueue] = None,
+    dead_letter_queue_enabled: typing.Optional[builtins.bool] = None,
+    dead_letter_topic: typing.Optional[_aws_cdk_aws_sns_ceddda9d.ITopic] = None,
+    description: typing.Optional[builtins.str] = None,
+    environment: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+    environment_encryption: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
+    ephemeral_storage_size: typing.Optional[_aws_cdk_ceddda9d.Size] = None,
+    events: typing.Optional[typing.Sequence[_aws_cdk_aws_lambda_ceddda9d.IEventSource]] = None,
+    filesystem: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.FileSystem] = None,
+    function_name: typing.Optional[builtins.str] = None,
+    initial_policy: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
+    insights_version: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.LambdaInsightsVersion] = None,
+    layers: typing.Optional[typing.Sequence[_aws_cdk_aws_lambda_ceddda9d.ILayerVersion]] = None,
+    log_retention: typing.Optional[_aws_cdk_aws_logs_ceddda9d.RetentionDays] = None,
+    log_retention_retry_options: typing.Optional[typing.Union[_aws_cdk_aws_lambda_ceddda9d.LogRetentionRetryOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+    log_retention_role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
+    memory_size: typing.Optional[jsii.Number] = None,
+    profiling: typing.Optional[builtins.bool] = None,
+    profiling_group: typing.Optional[_aws_cdk_aws_codeguruprofiler_ceddda9d.IProfilingGroup] = None,
+    reserved_concurrent_executions: typing.Optional[jsii.Number] = None,
+    role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
+    runtime_management_mode: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.RuntimeManagementMode] = None,
+    security_groups: typing.Optional[typing.Sequence[_aws_cdk_aws_ec2_ceddda9d.ISecurityGroup]] = None,
+    timeout: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
+    tracing: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.Tracing] = None,
+    vpc: typing.Optional[_aws_cdk_aws_ec2_ceddda9d.IVpc] = None,
+    vpc_subnets: typing.Optional[typing.Union[_aws_cdk_aws_ec2_ceddda9d.SubnetSelection, typing.Dict[builtins.str, typing.Any]]] = None,
+    aws_sdk_connection_reuse: typing.Optional[builtins.bool] = None,
+    bundling: typing.Optional[typing.Union[_aws_cdk_aws_lambda_nodejs_ceddda9d.BundlingOptions, typing.Dict[builtins.str, typing.Any]]] = None,
+    deps_lock_file_path: typing.Optional[builtins.str] = None,
+    entry: typing.Optional[builtins.str] = None,
+    handler: typing.Optional[builtins.str] = None,
+    project_root: typing.Optional[builtins.str] = None,
+    runtime: typing.Optional[_aws_cdk_aws_lambda_ceddda9d.Runtime] = None,
+    stage: builtins.str,
+    with_base_environment: typing.Optional[builtins.bool] = None,
+    with_base_tags: typing.Optional[builtins.bool] = None,
+    new_relic_account_id: builtins.str,
+    new_relic_layer_name: builtins.str,
+    new_relic_layer_version: jsii.Number,
+    new_relicwith_extension_send_logs: typing.Optional[builtins.bool] = None,
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `neulabs-cdk-constructs-0.4.4/src/neulabs_cdk_constructs/newrelic/__init__.py` & `neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs/newrelic/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.4.4/src/neulabs_cdk_constructs/oidc/__init__.py` & `neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs/oidc/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.4.4/src/neulabs_cdk_constructs/stack/__init__.py` & `neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs/stack/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.4.4/src/neulabs_cdk_constructs/utils/__init__.py` & `neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neulabs-cdk-constructs-0.4.4/src/neulabs_cdk_constructs.egg-info/PKG-INFO` & `neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neulabs-cdk-constructs
-Version: 0.4.4
+Version: 0.4.5
 Summary: neulabs-cdk-constructs
 Home-page: https://github.com/neulabscom/neulabs-cdk-constructs.git
 Author: Neulabs<tech@neulabs.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/neulabscom/neulabs-cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `neulabs-cdk-constructs-0.4.4/src/neulabs_cdk_constructs.egg-info/SOURCES.txt` & `neulabs-cdk-constructs-0.4.5/src/neulabs_cdk_constructs.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,13 +7,13 @@
 src/neulabs_cdk_constructs/py.typed
 src/neulabs_cdk_constructs.egg-info/PKG-INFO
 src/neulabs_cdk_constructs.egg-info/SOURCES.txt
 src/neulabs_cdk_constructs.egg-info/dependency_links.txt
 src/neulabs_cdk_constructs.egg-info/requires.txt
 src/neulabs_cdk_constructs.egg-info/top_level.txt
 src/neulabs_cdk_constructs/_jsii/__init__.py
-src/neulabs_cdk_constructs/_jsii/neulabs-cdk-constructs@0.4.4.jsii.tgz
+src/neulabs_cdk_constructs/_jsii/neulabs-cdk-constructs@0.4.5.jsii.tgz
 src/neulabs_cdk_constructs/aws_lambda/__init__.py
 src/neulabs_cdk_constructs/newrelic/__init__.py
 src/neulabs_cdk_constructs/oidc/__init__.py
 src/neulabs_cdk_constructs/stack/__init__.py
 src/neulabs_cdk_constructs/utils/__init__.py
```

