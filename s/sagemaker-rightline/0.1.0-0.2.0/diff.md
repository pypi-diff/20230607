# Comparing `tmp/sagemaker-rightline-0.1.0.tar.gz` & `tmp/sagemaker-rightline-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sagemaker-rightline-0.1.0.tar", last modified: Wed Jun  7 08:42:20 2023, max compression
+gzip compressed data, was "sagemaker-rightline-0.2.0.tar", last modified: Wed Jun  7 19:56:22 2023, max compression
```

## Comparing `sagemaker-rightline-0.1.0.tar` & `sagemaker-rightline-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:42:20.956539 sagemaker-rightline-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-07 08:42:04.000000 sagemaker-rightline-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7467 2023-06-07 08:42:20.956539 sagemaker-rightline-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-06-07 08:42:04.000000 sagemaker-rightline-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-07 08:42:04.000000 sagemaker-rightline-0.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:42:20.956539 sagemaker-rightline-0.1.0/sagemaker_rightline/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 08:42:12.000000 sagemaker-rightline-0.1.0/sagemaker_rightline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10562 2023-06-07 08:42:04.000000 sagemaker-rightline-0.1.0/sagemaker_rightline/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-06-07 08:42:04.000000 sagemaker-rightline-0.1.0/sagemaker_rightline/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    17709 2023-06-07 08:42:04.000000 sagemaker-rightline-0.1.0/sagemaker_rightline/validations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:42:20.956539 sagemaker-rightline-0.1.0/sagemaker_rightline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7467 2023-06-07 08:42:20.000000 sagemaker-rightline-0.1.0/sagemaker_rightline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-07 08:42:20.000000 sagemaker-rightline-0.1.0/sagemaker_rightline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 08:42:20.000000 sagemaker-rightline-0.1.0/sagemaker_rightline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-07 08:42:20.000000 sagemaker-rightline-0.1.0/sagemaker_rightline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-07 08:42:20.000000 sagemaker-rightline-0.1.0/sagemaker_rightline.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 08:42:20.956539 sagemaker-rightline-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:42:20.956539 sagemaker-rightline-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-06-07 08:42:04.000000 sagemaker-rightline-0.1.0/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-06-07 08:42:04.000000 sagemaker-rightline-0.1.0/tests/test_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-06-07 08:42:04.000000 sagemaker-rightline-0.1.0/tests/test_validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:56:22.748468 sagemaker-rightline-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-07 19:56:09.000000 sagemaker-rightline-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7814 2023-06-07 19:56:22.748468 sagemaker-rightline-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-06-07 19:56:09.000000 sagemaker-rightline-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-07 19:56:09.000000 sagemaker-rightline-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:56:22.748468 sagemaker-rightline-0.2.0/sagemaker_rightline/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 19:56:15.000000 sagemaker-rightline-0.2.0/sagemaker_rightline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10562 2023-06-07 19:56:09.000000 sagemaker-rightline-0.2.0/sagemaker_rightline/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-06-07 19:56:09.000000 sagemaker-rightline-0.2.0/sagemaker_rightline/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19742 2023-06-07 19:56:09.000000 sagemaker-rightline-0.2.0/sagemaker_rightline/validations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:56:22.748468 sagemaker-rightline-0.2.0/sagemaker_rightline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7814 2023-06-07 19:56:22.000000 sagemaker-rightline-0.2.0/sagemaker_rightline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-07 19:56:22.000000 sagemaker-rightline-0.2.0/sagemaker_rightline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 19:56:22.000000 sagemaker-rightline-0.2.0/sagemaker_rightline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-07 19:56:22.000000 sagemaker-rightline-0.2.0/sagemaker_rightline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-07 19:56:22.000000 sagemaker-rightline-0.2.0/sagemaker_rightline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 19:56:22.748468 sagemaker-rightline-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:56:22.748468 sagemaker-rightline-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-06-07 19:56:09.000000 sagemaker-rightline-0.2.0/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-06-07 19:56:09.000000 sagemaker-rightline-0.2.0/tests/test_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15133 2023-06-07 19:56:09.000000 sagemaker-rightline-0.2.0/tests/test_validations.py
```

### Comparing `sagemaker-rightline-0.1.0/LICENSE` & `sagemaker-rightline-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sagemaker-rightline-0.1.0/PKG-INFO` & `sagemaker-rightline-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemaker-rightline
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python package to easily validate properties of a SageMaker Pipeline.
 Author-email: stiebels <stiebels@github.com>, dipanjank <dipanjank@github.com>
 License: MIT License
         
         Copyright (c) 2023 stiebels
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -70,99 +70,110 @@
 
 ### ✔️ Validations
 A `Validation` is a class that inherits from the `Validation` base class.
 It is responsible for validating a single property of the `Pipeline` object.
 We differentiate between `Validations` that check the `Pipeline` object itself (class names beginning with "Pipeline") and `Validations` that check the `Pipeline` object's `Step` objects (class name starting with "Step").
 Depending on the specific `Validation`, a different set of `StepTypEnums` may be supported.
 
-For example, the `StepImagesExistOnEcr` supports `Processing` and `Training` steps. It's a validation checks that all ImageURI that
+For example, the `StepImagesExist` supports `Processing` and `Training` steps. It's a validation checks that all ImageURI that
 Steps of the named types of the `Pipeline` object reference indeed exist on the target ECR.
 
 The following `Validations` are currently implemented:
-  - `PipelineParameters`
-  - `StepImagesExistOnEcr`
-  - `StepKmsKeyId`
-  - `StepNetworkConfig`
+  - `PipelineParametersAsExpected`
+  - `StepImagesExist`
+  - `StepKmsKeyIdAsExpected`
+  - `StepNetworkConfigAsExpected`
   - `StepLambdaFunctionExists`
   - `StepRoleNameExists`
   - `StepRoleNameAsExpected`
+  - `StepTagsAsExpected`
 
 In most cases, a `Validation` subclass requires passing a `Rule` object to its constructor.
 
 ### 📜 Rules
 A `Rule` is a class that inherits from the `Rule` base class.
 It is responsible for defining the rule that a `Validation` checks for.
-For example, passing the list of expected KMSKeyIDs and the `Rule` `Equals` to `StepKmsKeyId` will check that
+For example, passing the list of expected KMSKeyIDs and the `Rule` `Equals` to `StepKmsKeyIdAsExpected` will check that
 all `Step` objects of the `Pipeline` object have a `KmsKeyId` property that matches the passed KMSKeyIDs.
 
-Note that not all `Validations` require a `Rule` object, e.g. `StepImagesExistOnEcr`.
+Note that not all `Validations` require a `Rule` object, e.g. `StepImagesExist`.
 
 The following `Rules` are currently implemented:
   - `Equals`
   - `Contains`
 
 All rules support the `negative` parameter (default: `False`), which allows for inverting the rule.
 
 ### 📝 Report
 A `Report` is a class whose instance is returned by the `Configuration` class (optionally a pandas.DataFrame instead).
 It contains the results of the `Validations` that were run against the `Pipeline` object as well as additional information
 to allow for further analysis.
 
 ## Usage
+
 ```python
 from sagemaker.processing import NetworkConfig
 from sagemaker.workflow.parameters import ParameterString
 from sagemaker_rightline.model import Configuration
 from sagemaker_rightline.rules import Contains, Equals
 from sagemaker_rightline.validations import (
-    PipelineParameters,
-    StepImagesExistOnEcr,
-    StepKmsKeyId,
-    StepNetworkConfig,
+    PipelineParametersAsExpected,
+    StepImagesExist,
+    StepKmsKeyIdAsExpected,
+    StepNetworkConfigAsExpected,
     StepLambdaFunctionExists,
     StepRoleNameExists,
     StepRoleNameAsExpected,
+    StepTagsAsExpected,
 )
 
 # Import a dummy pipeline
 from tests.fixtures.pipeline import get_sagemaker_pipeline
+
 sm_pipeline = get_sagemaker_pipeline()
 
 # Define Validations
 validations = [
-    StepImagesExistOnEcr(),
-    PipelineParameters(
+    StepImagesExist(),
+    PipelineParametersAsExpected(
         parameters_expected=[
             ParameterString(
                 name="parameter-1",
                 default_value="some-value",
             ),
         ],
         rule=Contains(),
     ),
-    StepKmsKeyId(
+    StepKmsKeyIdAsExpected(
         kms_key_id_expected="some/kms-key-alias",
         step_name="sm_training_step_sklearn",  # optional: if not set, will check all steps
         rule=Equals(),
     ),
-    StepNetworkConfig(
+    StepNetworkConfigAsExpected(
         network_config_expected=NetworkConfig(
             enable_network_isolation=False,
             security_group_ids=["sg-1234567890"],
             subnets=["subnet-1234567890"],
         ),
         rule=Equals(negative=True),
     ),
     StepLambdaFunctionExists(),
     StepRoleNameExists(),
     StepRoleNameAsExpected(
         role_name_expected="some-role-name",
         step_name="sm_training_step_sklearn",  # optional: if not set, will check all steps
         rule=Equals(),
     ),
+    StepTagsAsExpected(
+        tags_expected=[{
+            "some-key": "some-value",
+        }],
+        step_name="sm_training_step_sklearn",  # optional: if not set, will check all steps
+        rule=Equals(),
+    ),
 ]
 
 # Add Validations and SageMaker Pipeline to Configuration
 cm = Configuration(
     validations=validations,
     sagemaker_pipeline=sm_pipeline,
 )
```

### Comparing `sagemaker-rightline-0.1.0/README.md` & `sagemaker-rightline-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -25,99 +25,110 @@
 
 ### ✔️ Validations
 A `Validation` is a class that inherits from the `Validation` base class.
 It is responsible for validating a single property of the `Pipeline` object.
 We differentiate between `Validations` that check the `Pipeline` object itself (class names beginning with "Pipeline") and `Validations` that check the `Pipeline` object's `Step` objects (class name starting with "Step").
 Depending on the specific `Validation`, a different set of `StepTypEnums` may be supported.
 
-For example, the `StepImagesExistOnEcr` supports `Processing` and `Training` steps. It's a validation checks that all ImageURI that
+For example, the `StepImagesExist` supports `Processing` and `Training` steps. It's a validation checks that all ImageURI that
 Steps of the named types of the `Pipeline` object reference indeed exist on the target ECR.
 
 The following `Validations` are currently implemented:
-  - `PipelineParameters`
-  - `StepImagesExistOnEcr`
-  - `StepKmsKeyId`
-  - `StepNetworkConfig`
+  - `PipelineParametersAsExpected`
+  - `StepImagesExist`
+  - `StepKmsKeyIdAsExpected`
+  - `StepNetworkConfigAsExpected`
   - `StepLambdaFunctionExists`
   - `StepRoleNameExists`
   - `StepRoleNameAsExpected`
+  - `StepTagsAsExpected`
 
 In most cases, a `Validation` subclass requires passing a `Rule` object to its constructor.
 
 ### 📜 Rules
 A `Rule` is a class that inherits from the `Rule` base class.
 It is responsible for defining the rule that a `Validation` checks for.
-For example, passing the list of expected KMSKeyIDs and the `Rule` `Equals` to `StepKmsKeyId` will check that
+For example, passing the list of expected KMSKeyIDs and the `Rule` `Equals` to `StepKmsKeyIdAsExpected` will check that
 all `Step` objects of the `Pipeline` object have a `KmsKeyId` property that matches the passed KMSKeyIDs.
 
-Note that not all `Validations` require a `Rule` object, e.g. `StepImagesExistOnEcr`.
+Note that not all `Validations` require a `Rule` object, e.g. `StepImagesExist`.
 
 The following `Rules` are currently implemented:
   - `Equals`
   - `Contains`
 
 All rules support the `negative` parameter (default: `False`), which allows for inverting the rule.
 
 ### 📝 Report
 A `Report` is a class whose instance is returned by the `Configuration` class (optionally a pandas.DataFrame instead).
 It contains the results of the `Validations` that were run against the `Pipeline` object as well as additional information
 to allow for further analysis.
 
 ## Usage
+
 ```python
 from sagemaker.processing import NetworkConfig
 from sagemaker.workflow.parameters import ParameterString
 from sagemaker_rightline.model import Configuration
 from sagemaker_rightline.rules import Contains, Equals
 from sagemaker_rightline.validations import (
-    PipelineParameters,
-    StepImagesExistOnEcr,
-    StepKmsKeyId,
-    StepNetworkConfig,
+    PipelineParametersAsExpected,
+    StepImagesExist,
+    StepKmsKeyIdAsExpected,
+    StepNetworkConfigAsExpected,
     StepLambdaFunctionExists,
     StepRoleNameExists,
     StepRoleNameAsExpected,
+    StepTagsAsExpected,
 )
 
 # Import a dummy pipeline
 from tests.fixtures.pipeline import get_sagemaker_pipeline
+
 sm_pipeline = get_sagemaker_pipeline()
 
 # Define Validations
 validations = [
-    StepImagesExistOnEcr(),
-    PipelineParameters(
+    StepImagesExist(),
+    PipelineParametersAsExpected(
         parameters_expected=[
             ParameterString(
                 name="parameter-1",
                 default_value="some-value",
             ),
         ],
         rule=Contains(),
     ),
-    StepKmsKeyId(
+    StepKmsKeyIdAsExpected(
         kms_key_id_expected="some/kms-key-alias",
         step_name="sm_training_step_sklearn",  # optional: if not set, will check all steps
         rule=Equals(),
     ),
-    StepNetworkConfig(
+    StepNetworkConfigAsExpected(
         network_config_expected=NetworkConfig(
             enable_network_isolation=False,
             security_group_ids=["sg-1234567890"],
             subnets=["subnet-1234567890"],
         ),
         rule=Equals(negative=True),
     ),
     StepLambdaFunctionExists(),
     StepRoleNameExists(),
     StepRoleNameAsExpected(
         role_name_expected="some-role-name",
         step_name="sm_training_step_sklearn",  # optional: if not set, will check all steps
         rule=Equals(),
     ),
+    StepTagsAsExpected(
+        tags_expected=[{
+            "some-key": "some-value",
+        }],
+        step_name="sm_training_step_sklearn",  # optional: if not set, will check all steps
+        rule=Equals(),
+    ),
 ]
 
 # Add Validations and SageMaker Pipeline to Configuration
 cm = Configuration(
     validations=validations,
     sagemaker_pipeline=sm_pipeline,
 )
```

### Comparing `sagemaker-rightline-0.1.0/pyproject.toml` & `sagemaker-rightline-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sagemaker-rightline-0.1.0/sagemaker_rightline/model.py` & `sagemaker-rightline-0.2.0/sagemaker_rightline/model.py`

 * *Files identical despite different names*

### Comparing `sagemaker-rightline-0.1.0/sagemaker_rightline/rules.py` & `sagemaker-rightline-0.2.0/sagemaker_rightline/rules.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         :param expected: expected list
         :type expected: List[Any]
         :param validation_name: name of the validation
         :type validation_name: str
         :return: validation result
         :rtype: ValidationResult
         """
-        is_contained = set(expected).issubset(set(observed))
+        is_contained = all(item in observed for item in expected)
         is_contained = is_contained if not self.negative else not is_contained
         return ValidationResult(
             validation_name=validation_name,
             success=is_contained,
             negative=self.negative,
             message=f"{str(observed)} does {'not ' if not is_contained else ''}contain "
             f"{str(expected)}",
```

### Comparing `sagemaker-rightline-0.1.0/sagemaker_rightline/validations.py` & `sagemaker-rightline-0.2.0/sagemaker_rightline/validations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 import re
 from dataclasses import dataclass
-from typing import List, Optional, Union
+from typing import Dict, List, Optional, Union
 
 import boto3
 from botocore.exceptions import ClientError
 from sagemaker.estimator import Estimator
 from sagemaker.processing import NetworkConfig
+from sagemaker.workflow.entities import PipelineVariable
 from sagemaker.workflow.parameters import Parameter
 from sagemaker.workflow.pipeline import Pipeline
 
 from sagemaker_rightline.model import Rule, Validation, ValidationResult
 
 
-class PipelineParameters(Validation):
+class PipelineParametersAsExpected(Validation):
     """Validate Pipeline Parameters.
 
     This validation will check if the parameters in the pipeline are as
     expected.
     """
 
     def __init__(
         self, parameters_expected: List[Parameter], rule: Rule, ignore_default_value: bool = False
     ) -> None:
         """Validate Pipeline Parameters."""
-        super().__init__(name="PipelineParameters", paths=[".parameters[]"], rule=rule)
+        super().__init__(name="PipelineParametersAsExpected", paths=[".parameters[]"], rule=rule)
         if not parameters_expected:
             raise ValueError("parameters_expected cannot be empty.")
         self.parameters_expected: List[Parameter] = parameters_expected
         self.ignore_default_value: bool = ignore_default_value
 
     def run(self, sagemaker_pipeline: Pipeline) -> ValidationResult:
         """Runs validation of Parameters on Pipeline.
@@ -41,29 +42,29 @@
         if self.ignore_default_value:
             for ix, parameter in enumerate(parameters_observed):
                 parameters_observed[ix].default_value = None
         result = self.rule.run(parameters_observed, self.parameters_expected, self.name)
         return result
 
 
-class StepKmsKeyId(Validation):
+class StepKmsKeyIdAsExpected(Validation):
     """Validate KmsKeyId or output_kms_key in Step.
 
     Supported only for ProcessingStep and TrainingStep (output_kms_key).
     This validation is useful when you want to ensure that the KmsKeyId
     or output_kms_key of a Pipeline Step is as expected.
     """
 
     def __init__(
         self, kms_key_id_expected: str, rule: Rule, step_name: Optional[str] = None
     ) -> None:
-        """Initialize StepKmsKeyId validation."""
+        """Initialize StepKmsKeyIdAsExpected validation."""
         self.step_filter: str = f"name=={step_name}" if step_name else ""
         super().__init__(
-            name="StepKmsKeyId",
+            name="StepKmsKeyIdAsExpected",
             paths=[
                 f".steps[{self.step_filter} && step_type/value==Processing].kms_key",
                 f".steps[{self.step_filter} && step_type/value==Training].estimator.output_kms_key",
             ],
             rule=rule,
         )
         self.kms_key_id_expected: str = kms_key_id_expected
@@ -94,15 +95,15 @@
         """Decompose ImageUri into its components."""
         self.account_id = self.uri.split(".")[0]
         self.repository = re.search("/(.*):", self.uri).group(1)
         self.region = self.uri.split(".")[3]
         self.tag = self.uri.split(":")[1]
 
 
-class StepImagesExistOnEcr(Validation):
+class StepImagesExist(Validation):
     """Check if container images exist in ECR.
 
     Supported only for ProcessingStep and TrainingStep.
     """
 
     def __init__(
         self,
@@ -116,15 +117,15 @@
         :param step_name: Step name to filter on, defaults to None
         :type step_name: Optional[str], optional
         :return: None
         :rtype: None
         """
         self.step_filter: str = f"name=={step_name}" if step_name else ""
         super().__init__(
-            name="StepImagesExistOnEcr",
+            name="StepImagesExist",
             paths=[
                 f".steps[{self.step_filter} && step_type/value==Processing].processor.image_uri",
                 f".steps[{self.step_filter} && step_type/value==Training].estimator.image_uri",
             ],
         )
         if isinstance(boto3_client, str) and boto3_client != "ecr":
             raise ValueError(f"boto3_client must be 'ecr', not {boto3_client}.")
@@ -177,39 +178,39 @@
             success=True,
             negative=False,
             message=f"Images {exist} exist.",
             subject=str(exist),
         )
 
 
-class StepNetworkConfig(Validation):
+class StepNetworkConfigAsExpected(Validation):
     """Validate NetworkConfig in Step.
 
     This Validation currently supports only ProcessingStep. This
     validation is useful when you want to ensure that the NetworkConfig
     of a Pipeline Step's Processor is as expected.
     """
 
     def __init__(
         self, network_config_expected: NetworkConfig, rule: Rule, step_name: Optional[str] = None
     ) -> None:
-        """Initialize StepNetworkConfig validation.
+        """Initialize StepNetworkConfigAsExpected validation.
 
         :param network_config_expected: Expected NetworkConfig
         :type network_config_expected: NetworkConfig
         :param rule: Rule to apply
         :type rule: Rule
         :param step_name: Name of Step to validate, defaults to None
         :type step_name: Optional[str], optional
         :return: None
         :rtype: None
         """
         self.step_filter: str = f"name=={step_name}" if step_name else ""
         super().__init__(
-            name="StepNetworkConfig",
+            name="StepNetworkConfigAsExpected",
             paths=[
                 f".steps[{self.step_filter}].processor.network_config",
             ],
             rule=rule,
         )
         self.network_config_expected: NetworkConfig = network_config_expected
 
@@ -258,16 +259,18 @@
         training_step_estimators = [
             step.estimator
             for step in sagemaker_pipeline.steps
             if step.step_type.value == "Training"
             and step.name == self.step_filter.replace("name==", "")
         ]
         if training_step_estimators:
-            network_configs_observed += StepNetworkConfig.get_training_step_network_config(
-                training_step_estimators
+            network_configs_observed += (
+                StepNetworkConfigAsExpected.get_training_step_network_config(
+                    training_step_estimators
+                )
             )
 
         network_configs_observed_dict = []
         for nwc in network_configs_observed:
             if nwc:
                 network_configs_observed_dict.append(nwc.__dict__)
             else:
@@ -481,7 +484,60 @@
             return ValidationResult(
                 success=True,
                 negative=False,
                 message=f"Role {exist} exists.",
                 subject=str(role_name_observed),
                 validation_name=self.name,
             )
+
+
+class StepTagsAsExpected(Validation):
+    """Validate Tags of Pipeline Step.
+
+    Supported only for ProcessingStep and TrainingStep. This validation
+    is useful when you want to ensure that the Tags of a Pipeline Step
+    are as expected.
+    """
+
+    def __init__(
+        self,
+        tags_expected: List[Dict[str, Union[str, PipelineVariable]]],
+        rule: Rule,
+        step_name: Optional[str] = None,
+    ) -> None:
+        """Initialize StepTagsAsExpected validation.
+
+        :param tags_expected: Expected Tags
+        :type tags_expected: List[Dict[str, Union[str, PipelineVariable]]]
+        :param rule: Rule to use for validation
+        :type rule: Rule
+        :param step_name: Name of Step to validate, defaults to None
+        :type step_name: Optional[str], optional
+        :return: None
+        :rtype: None
+        """
+        self.step_filter: str = f"name=={step_name}" if step_name else ""
+
+        super().__init__(
+            name="StepTagsAsExpected",
+            paths=[
+                f".steps[{self.step_filter} && step_type/value==Processing].processor.tags",
+                f".steps[{self.step_filter} && step_type/value==Training].estimator.tags",
+            ],
+            rule=rule,
+        )
+        self.tags_expected: List[Dict[str, Union[str, PipelineVariable]]] = tags_expected
+
+    def run(
+        self,
+        sagemaker_pipeline: Pipeline,
+    ) -> ValidationResult:
+        """Runs validation of Parameters on Pipeline.
+
+        :param sagemaker_pipeline: SageMaker Pipeline
+        :type sagemaker_pipeline: sagemaker.workflow.pipeline.Pipeline
+        :return: validation result
+        :rtype: ValidationResult
+        """
+        tags_observed = self.get_attribute(sagemaker_pipeline)
+        result = self.rule.run(tags_observed[0], self.tags_expected, self.name)
+        return result
```

### Comparing `sagemaker-rightline-0.1.0/sagemaker_rightline.egg-info/PKG-INFO` & `sagemaker-rightline-0.2.0/sagemaker_rightline.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemaker-rightline
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python package to easily validate properties of a SageMaker Pipeline.
 Author-email: stiebels <stiebels@github.com>, dipanjank <dipanjank@github.com>
 License: MIT License
         
         Copyright (c) 2023 stiebels
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -70,99 +70,110 @@
 
 ### ✔️ Validations
 A `Validation` is a class that inherits from the `Validation` base class.
 It is responsible for validating a single property of the `Pipeline` object.
 We differentiate between `Validations` that check the `Pipeline` object itself (class names beginning with "Pipeline") and `Validations` that check the `Pipeline` object's `Step` objects (class name starting with "Step").
 Depending on the specific `Validation`, a different set of `StepTypEnums` may be supported.
 
-For example, the `StepImagesExistOnEcr` supports `Processing` and `Training` steps. It's a validation checks that all ImageURI that
+For example, the `StepImagesExist` supports `Processing` and `Training` steps. It's a validation checks that all ImageURI that
 Steps of the named types of the `Pipeline` object reference indeed exist on the target ECR.
 
 The following `Validations` are currently implemented:
-  - `PipelineParameters`
-  - `StepImagesExistOnEcr`
-  - `StepKmsKeyId`
-  - `StepNetworkConfig`
+  - `PipelineParametersAsExpected`
+  - `StepImagesExist`
+  - `StepKmsKeyIdAsExpected`
+  - `StepNetworkConfigAsExpected`
   - `StepLambdaFunctionExists`
   - `StepRoleNameExists`
   - `StepRoleNameAsExpected`
+  - `StepTagsAsExpected`
 
 In most cases, a `Validation` subclass requires passing a `Rule` object to its constructor.
 
 ### 📜 Rules
 A `Rule` is a class that inherits from the `Rule` base class.
 It is responsible for defining the rule that a `Validation` checks for.
-For example, passing the list of expected KMSKeyIDs and the `Rule` `Equals` to `StepKmsKeyId` will check that
+For example, passing the list of expected KMSKeyIDs and the `Rule` `Equals` to `StepKmsKeyIdAsExpected` will check that
 all `Step` objects of the `Pipeline` object have a `KmsKeyId` property that matches the passed KMSKeyIDs.
 
-Note that not all `Validations` require a `Rule` object, e.g. `StepImagesExistOnEcr`.
+Note that not all `Validations` require a `Rule` object, e.g. `StepImagesExist`.
 
 The following `Rules` are currently implemented:
   - `Equals`
   - `Contains`
 
 All rules support the `negative` parameter (default: `False`), which allows for inverting the rule.
 
 ### 📝 Report
 A `Report` is a class whose instance is returned by the `Configuration` class (optionally a pandas.DataFrame instead).
 It contains the results of the `Validations` that were run against the `Pipeline` object as well as additional information
 to allow for further analysis.
 
 ## Usage
+
 ```python
 from sagemaker.processing import NetworkConfig
 from sagemaker.workflow.parameters import ParameterString
 from sagemaker_rightline.model import Configuration
 from sagemaker_rightline.rules import Contains, Equals
 from sagemaker_rightline.validations import (
-    PipelineParameters,
-    StepImagesExistOnEcr,
-    StepKmsKeyId,
-    StepNetworkConfig,
+    PipelineParametersAsExpected,
+    StepImagesExist,
+    StepKmsKeyIdAsExpected,
+    StepNetworkConfigAsExpected,
     StepLambdaFunctionExists,
     StepRoleNameExists,
     StepRoleNameAsExpected,
+    StepTagsAsExpected,
 )
 
 # Import a dummy pipeline
 from tests.fixtures.pipeline import get_sagemaker_pipeline
+
 sm_pipeline = get_sagemaker_pipeline()
 
 # Define Validations
 validations = [
-    StepImagesExistOnEcr(),
-    PipelineParameters(
+    StepImagesExist(),
+    PipelineParametersAsExpected(
         parameters_expected=[
             ParameterString(
                 name="parameter-1",
                 default_value="some-value",
             ),
         ],
         rule=Contains(),
     ),
-    StepKmsKeyId(
+    StepKmsKeyIdAsExpected(
         kms_key_id_expected="some/kms-key-alias",
         step_name="sm_training_step_sklearn",  # optional: if not set, will check all steps
         rule=Equals(),
     ),
-    StepNetworkConfig(
+    StepNetworkConfigAsExpected(
         network_config_expected=NetworkConfig(
             enable_network_isolation=False,
             security_group_ids=["sg-1234567890"],
             subnets=["subnet-1234567890"],
         ),
         rule=Equals(negative=True),
     ),
     StepLambdaFunctionExists(),
     StepRoleNameExists(),
     StepRoleNameAsExpected(
         role_name_expected="some-role-name",
         step_name="sm_training_step_sklearn",  # optional: if not set, will check all steps
         rule=Equals(),
     ),
+    StepTagsAsExpected(
+        tags_expected=[{
+            "some-key": "some-value",
+        }],
+        step_name="sm_training_step_sklearn",  # optional: if not set, will check all steps
+        rule=Equals(),
+    ),
 ]
 
 # Add Validations and SageMaker Pipeline to Configuration
 cm = Configuration(
     validations=validations,
     sagemaker_pipeline=sm_pipeline,
 )
```

### Comparing `sagemaker-rightline-0.1.0/tests/test_model.py` & `sagemaker-rightline-0.2.0/tests/test_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     Report,
     Validation,
     ValidationFailedError,
 )
 from sagemaker_rightline.rules import Equals, Rule
 from sagemaker_rightline.validations import (
     ContainerImage,
-    StepImagesExistOnEcr,
-    StepKmsKeyId,
+    StepImagesExist,
+    StepKmsKeyIdAsExpected,
     ValidationResult,
 )
 from tests.fixtures.image_details import IMAGE_1_URI, IMAGE_2_URI
 from tests.fixtures.pipeline import get_sagemaker_pipeline
 from tests.utils import create_image, ecr_client
 
 
@@ -27,16 +27,16 @@
 
 @pytest.mark.parametrize(
     "validations,error",
     [
         [["not_validation"], True],
         ["not_list", True],
         [[], True],
-        [[StepImagesExistOnEcr()], False],
-        [[StepImagesExistOnEcr(), StepImagesExistOnEcr()], False],
+        [[StepImagesExist()], False],
+        [[StepImagesExist(), StepImagesExist()], False],
     ],
 )
 def test_configuration_validate_input_validations(validations, error: bool) -> None:
     if error:
         with pytest.raises((ValueError, TypeError)):
             Configuration._validate_input_validations(validations=validations)
     else:
@@ -81,16 +81,16 @@
     assert isinstance(report.results[0], ValidationResult)
 
 
 @mock_ecr
 @pytest.mark.parametrize(
     "expected_report_length,validations, return_df",
     [
-        [1, [StepImagesExistOnEcr()], False],
-        [2, [StepImagesExistOnEcr(), StepImagesExistOnEcr()], True],
+        [1, [StepImagesExist()], False],
+        [2, [StepImagesExist(), StepImagesExist()], True],
     ],
 )
 def test_configuration_run(
     sagemaker_pipeline, ecr_client, expected_report_length, validations, return_df
 ) -> None:
     """Test run method of Configuration class."""
     container_images = [
@@ -108,15 +108,15 @@
         assert isinstance(report, Report)
         observed_report_len = len(report.results)
     assert observed_report_len == expected_report_length
 
 
 def test_configuration_handle_empty_results(sagemaker_pipeline) -> None:
     """Test run method of Configuration class."""
-    validation = StepKmsKeyId(
+    validation = StepKmsKeyIdAsExpected(
         step_name="sm_processing_step_sklearn",
         rule=Equals(),
         kms_key_id_expected="some/kms-key-alias",
     )
     cf = Configuration(validations=[validation], sagemaker_pipeline=sagemaker_pipeline)
     validation_result = cf._handle_empty_results(
         result=None,
@@ -127,16 +127,16 @@
     assert not validation_result.success
 
 
 @mock_ecr
 @pytest.mark.parametrize(
     "raises_error,validations",
     [
-        [False, [StepImagesExistOnEcr()]],
-        [True, [StepImagesExistOnEcr(), StepImagesExistOnEcr()]],
+        [False, [StepImagesExist()]],
+        [True, [StepImagesExist(), StepImagesExist()]],
     ],
 )
 def test_configuration_run_fail_fast(sagemaker_pipeline, raises_error, validations) -> None:
     """Test run method of Configuration class."""
     cf = Configuration(validations=validations, sagemaker_pipeline=sagemaker_pipeline)
     if raises_error:
         with pytest.raises(ValidationFailedError):
@@ -144,15 +144,15 @@
     else:
         report = cf.run(fail_fast=True)
         assert len(report.results) == 1
 
 
 def test_report_to_df() -> None:
     """Test to_df method of Report class."""
-    validation_name = "StepImagesExistOnEcr"
+    validation_name = "StepImagesExist"
     report = Report(
         results=[
             ValidationResult(
                 success=True,
                 negative=False,
                 message="test-message-0",
                 subject="test-subject-0",
@@ -168,36 +168,36 @@
     assert df["message"].tolist() == ["test-message-0"]
     assert df["validation_name"].tolist() == [validation_name]
 
 
 def test_validation_get_attribute_filter(sagemaker_pipeline) -> None:
     """Test get_attribute method of Validation class."""
     kms_key_alias_expected = "some/kms-key-alias"
-    validation = StepKmsKeyId(
+    validation = StepKmsKeyIdAsExpected(
         step_name="sm_processing_step_sklearn",
         rule=Equals(),
         kms_key_id_expected=kms_key_alias_expected,
     )
     assert validation.get_attribute(sagemaker_pipeline) == [kms_key_alias_expected]
 
 
 def test_validation_get_attribute_no_filter(sagemaker_pipeline) -> None:
     """Test get_attribute method of Validation class."""
     kms_key_alias_expected = "some/kms-key-alias"
-    validation = StepKmsKeyId(
+    validation = StepKmsKeyIdAsExpected(
         rule=Equals(),
         kms_key_id_expected=kms_key_alias_expected,
     )
     assert validation.get_attribute(sagemaker_pipeline) == [
         kms_key_alias_expected,
         kms_key_alias_expected,
         kms_key_alias_expected,
     ]
 
-    validation = StepImagesExistOnEcr()
+    validation = StepImagesExist()
     assert validation.get_attribute(sagemaker_pipeline) == [IMAGE_1_URI, IMAGE_2_URI, IMAGE_1_URI]
 
 
 def test_validation_failed_error():
     """Test ValidationFailedError class."""
     validation_result = ValidationResult(
         success=False,
```

### Comparing `sagemaker-rightline-0.1.0/tests/test_rules.py` & `sagemaker-rightline-0.2.0/tests/test_rules.py`

 * *Files identical despite different names*

### Comparing `sagemaker-rightline-0.1.0/tests/test_validations.py` & `sagemaker-rightline-0.2.0/tests/test_validations.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import pytest
 from moto import mock_ecr, mock_iam, mock_lambda
 from sagemaker.processing import NetworkConfig
 from sagemaker.workflow.parameters import ParameterString
 
 from sagemaker_rightline.model import Validation, ValidationResult
-from sagemaker_rightline.rules import Equals
+from sagemaker_rightline.rules import Contains, Equals
 from sagemaker_rightline.validations import (
     ContainerImage,
-    PipelineParameters,
-    StepImagesExistOnEcr,
-    StepKmsKeyId,
+    PipelineParametersAsExpected,
+    StepImagesExist,
+    StepKmsKeyIdAsExpected,
     StepLambdaFunctionExists,
-    StepNetworkConfig,
+    StepNetworkConfigAsExpected,
     StepRoleNameAsExpected,
     StepRoleNameExists,
+    StepTagsAsExpected,
 )
 from tests.fixtures.constants import (
     TEST_ACCOUNT_ID,
     TEST_LAMBDA_FUNC_NAME,
     TEST_REGION_NAME,
     TEST_ROLE_NAME,
 )
@@ -75,34 +76,34 @@
 @mock_ecr
 def test_step_image_exists_run_positive(ecr_client, sagemaker_pipeline) -> None:
     container_images = [
         ContainerImage(uri=IMAGE_1_URI),
         ContainerImage(uri=IMAGE_2_URI),
     ]
     with create_image(ecr_client, container_images):
-        image_exists = StepImagesExistOnEcr()
+        image_exists = StepImagesExist()
         result = image_exists.run(sagemaker_pipeline)
 
     assert result.success
     assert not result.negative
     assert result.message.endswith(" exist.")
 
 
 @mock_ecr
 def test_step_image_exists_run_negative(sagemaker_pipeline) -> None:
-    image_exists = StepImagesExistOnEcr()
+    image_exists = StepImagesExist()
     result = image_exists.run(sagemaker_pipeline)
 
     assert not result.success
     assert result.message.endswith(" not exist.")
 
 
 def test_step_image_exists_wrong_client() -> None:
     with pytest.raises(ValueError):
-        _ = StepImagesExistOnEcr(boto3_client="not-a-boto3-client")
+        _ = StepImagesExist(boto3_client="not-a-boto3-client")
 
 
 def test_step_lambda_function_exists_wrong_client() -> None:
     with pytest.raises(ValueError):
         _ = StepLambdaFunctionExists(boto3_client="not-a-boto3-client")
 
 
@@ -135,15 +136,15 @@
                 ParameterString(name="parameter-2", default_value="some-value-2"),
             ],
             False,
         ],
     ],
 )
 def test_pipeline_parameters_equals(parameters_expected, success, sagemaker_pipeline) -> None:
-    pipeline_parameters = PipelineParameters(
+    pipeline_parameters = PipelineParametersAsExpected(
         parameters_expected=parameters_expected,
         rule=Equals(),
     )
     result = pipeline_parameters.run(sagemaker_pipeline)
     assert result.success == success
 
 
@@ -167,37 +168,37 @@
             False,
         ],
     ],
 )
 def test_pipeline_parameters_ignore_default_value(
     parameters_expected, ignore_default_value, success, sagemaker_pipeline
 ) -> None:
-    pipeline_parameters = PipelineParameters(
+    pipeline_parameters = PipelineParametersAsExpected(
         parameters_expected=parameters_expected,
         ignore_default_value=ignore_default_value,
         rule=Equals(),
     )
     result = pipeline_parameters.run(sagemaker_pipeline)
     assert result.success == success
 
 
 def test_has_parameters_raise() -> None:
     with pytest.raises(ValueError):
-        _ = PipelineParameters(parameters_expected=[], rule=Equals())
+        _ = PipelineParametersAsExpected(parameters_expected=[], rule=Equals())
 
 
 @pytest.mark.parametrize(
     "kms_key_id_expected,success",
     [
         ["some/kms-key-alias", True],
         ["does-not-exist", False],
     ],
 )
 def test_step_kms_key_id(kms_key_id_expected, success, sagemaker_pipeline) -> None:
-    has_kms_key_id_in_processing_output = StepKmsKeyId(
+    has_kms_key_id_in_processing_output = StepKmsKeyIdAsExpected(
         kms_key_id_expected=kms_key_id_expected,
         rule=Equals(),
     )
     result = has_kms_key_id_in_processing_output.run(sagemaker_pipeline)
     assert result.success == success
 
 
@@ -205,15 +206,15 @@
     "kms_key_id_expected,success",
     [
         ["some/kms-key-alias", True],
         ["does-not-exist", False],
     ],
 )
 def test_step_kms_key_id_filter(kms_key_id_expected, success, sagemaker_pipeline) -> None:
-    has_kms_key_id_in_processing_output = StepKmsKeyId(
+    has_kms_key_id_in_processing_output = StepKmsKeyIdAsExpected(
         kms_key_id_expected=kms_key_id_expected,
         step_name="sm_processing_step_sklearn",
         rule=Equals(),
     )
     result = has_kms_key_id_in_processing_output.run(sagemaker_pipeline)
     assert result.success == success
 
@@ -222,15 +223,15 @@
     "kms_key_id_expected,success",
     [
         ["some/kms-key-alias", True],
         ["does-not-exist", False],
     ],
 )
 def test_step_kms_key_id_no_filter(kms_key_id_expected, success, sagemaker_pipeline) -> None:
-    has_kms_key_id_in_processing_output = StepKmsKeyId(
+    has_kms_key_id_in_processing_output = StepKmsKeyIdAsExpected(
         kms_key_id_expected=kms_key_id_expected,
         rule=Equals(),
     )
     result = has_kms_key_id_in_processing_output.run(sagemaker_pipeline)
     assert result.success == success
 
 
@@ -248,15 +249,15 @@
 ) -> None:
     network_config_expected = NetworkConfig(
         enable_network_isolation=True,
         security_group_ids=["sg-12345"],
         subnets=["subnet-12345"],
         encrypt_inter_container_traffic=True,
     )
-    step_network_config = StepNetworkConfig(
+    step_network_config = StepNetworkConfigAsExpected(
         network_config_expected=network_config_expected,
         rule=Equals(),
     )
     result = step_network_config.run(sagemaker_pipeline)
     assert not result.success
 
 
@@ -265,15 +266,15 @@
 ) -> None:
     network_config_expected = NetworkConfig(
         enable_network_isolation=True,
         security_group_ids=["sg-12345"],
         subnets=["subnet-12345"],
         encrypt_inter_container_traffic=True,
     )
-    step_network_config = StepNetworkConfig(
+    step_network_config = StepNetworkConfigAsExpected(
         network_config_expected=network_config_expected,
         rule=Equals(),
     )
     result = step_network_config.rule.run([None], network_config_expected, step_network_config.name)
     assert not result.success
 
 
@@ -314,15 +315,15 @@
             "sm_training_step_sklearn",
         ],
     ],
 )
 def test_step_network_config_filter(
     network_config_expected, success, step_name, sagemaker_pipeline
 ) -> None:
-    step_network_config = StepNetworkConfig(
+    step_network_config = StepNetworkConfigAsExpected(
         network_config_expected=network_config_expected,
         rule=Equals(),
         step_name=step_name,
     )
     result = step_network_config.run(sagemaker_pipeline)
     assert result.success == success
 
@@ -361,15 +362,15 @@
 @pytest.mark.parametrize(
     "role_name_expected,success",
     [
         [TEST_ROLE_NAME, True],
         ["nonexistent-role-name", False],
     ],
 )
-def test_step_role_filter(role_name_expected, success, sagemaker_pipeline) -> None:
+def test_step_role_name_as_expected_filter(role_name_expected, success, sagemaker_pipeline) -> None:
     step_role_validation = StepRoleNameAsExpected(
         role_name_expected=role_name_expected,
         step_name="sm_processing_step_sklearn",
         rule=Equals(),
     )
     result = step_role_validation.run(sagemaker_pipeline)
     assert result.success == success
@@ -378,14 +379,113 @@
 @pytest.mark.parametrize(
     "role_name_expected,success",
     [
         [TEST_ROLE_NAME, True],
         ["nonexistent-role-name", False],
     ],
 )
-def test_step_role_no_filter(role_name_expected, success, sagemaker_pipeline) -> None:
+def test_step_role_name_as_expected_no_filter(
+    role_name_expected, success, sagemaker_pipeline
+) -> None:
     step_role_validation = StepRoleNameAsExpected(
         role_name_expected=role_name_expected,
         rule=Equals(),
     )
     result = step_role_validation.run(sagemaker_pipeline)
     assert result.success == success
+
+
+@pytest.mark.parametrize(
+    "rule,tags_expected,step_name,success",
+    [
+        [Equals, [{"Key": "some-key", "Value": "some-value"}], "sm_processing_step_spark", True],
+        [Contains, [{"Key": "some-key", "Value": "some-value"}], "sm_processing_step_spark", True],
+        [
+            Contains,
+            [{"Key": "some-key", "Value": "some-value"}],
+            "sm_processing_step_sklearn",
+            True,
+        ],
+        [
+            Equals,
+            [
+                {
+                    "Key": "some-key",
+                    "Value": ParameterString(name="parameter-1", default_value="some-value-1"),
+                }
+            ],
+            "sm_training_step_sklearn",
+            False,
+        ],
+        [
+            Equals,
+            [
+                {"Key": "some-key", "Value": "some-value"},
+                {
+                    "Key": "some-key",
+                    "Value": ParameterString(name="parameter-1", default_value="some-value-1"),
+                },
+            ],
+            "sm_training_step_sklearn",
+            True,
+        ],
+        [
+            Equals,
+            [
+                {"Key": "some-key", "Value": "some-value"},
+                {"Key": "some-non-existent-key", "Value": "some-non-existent-value"},
+            ],
+            "sm_processing_step_spark",
+            False,
+        ],
+        [
+            Equals,
+            [{"Key": "some-key", "Value": "some-non-existent-value"}],
+            "sm_processing_step_spark",
+            False,
+        ],
+        [
+            Equals,
+            [{"Key": "some-non-existent-key", "Value": "some-value"}],
+            "sm_processing_step_spark",
+            False,
+        ],
+        [Equals, [], "sm_processing_step_spark", False],
+    ],
+)
+def test_step_tags_as_expected_filter(
+    rule, tags_expected, step_name, success, sagemaker_pipeline
+) -> None:
+    step_role_validation = StepTagsAsExpected(
+        tags_expected=tags_expected,
+        step_name=step_name,
+        rule=rule(),
+    )
+    result = step_role_validation.run(sagemaker_pipeline)
+    assert result.success == success
+
+
+@pytest.mark.parametrize(
+    "rule,tags_expected,success",
+    [
+        [Equals, [{"Key": "some-key", "Value": "some-value"}], False],
+        [Equals, [{"Key": "some-non-existent-key", "Value": "some-non-existent-value"}], False],
+        [
+            Contains,
+            [
+                {
+                    "Key": "some-key",
+                    "Value": ParameterString(name="parameter-1", default_value="some-value-1"),
+                }
+            ],
+            False,
+        ],
+        [Contains, [{"Key": "some-key", "Value": "some-value"}], True],
+    ],
+)
+def test_step_tags_as_expected_no_filter(rule, tags_expected, success, sagemaker_pipeline) -> None:
+    step_role_validation = StepTagsAsExpected(
+        tags_expected=tags_expected,
+        rule=rule(),
+    )
+    result = step_role_validation.run(sagemaker_pipeline)
+    assert result.success == success
```

