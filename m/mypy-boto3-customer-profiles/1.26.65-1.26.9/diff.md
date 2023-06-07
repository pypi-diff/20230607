# Comparing `tmp/mypy-boto3-customer-profiles-1.26.65.tar.gz` & `tmp/mypy-boto3-customer-profiles-1.26.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-customer-profiles-1.26.65.tar", last modified: Mon Feb  6 20:47:28 2023, max compression
+gzip compressed data, was "mypy-boto3-customer-profiles-1.26.9.tar", last modified: Mon Nov 14 20:49:29 2022, max compression
```

## Comparing `mypy-boto3-customer-profiles-1.26.65.tar` & `mypy-boto3-customer-profiles-1.26.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 20:47:28.153984 mypy-boto3-customer-profiles-1.26.65/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-06 20:47:04.000000 mypy-boto3-customer-profiles-1.26.65/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17482 2023-02-06 20:47:28.153984 mypy-boto3-customer-profiles-1.26.65/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15956 2023-02-06 20:47:04.000000 mypy-boto3-customer-profiles-1.26.65/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 20:47:28.149984 mypy-boto3-customer-profiles-1.26.65/mypy_boto3_customer_profiles/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-02-06 20:47:04.000000 mypy-boto3-customer-profiles-1.26.65/mypy_boto3_customer_profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-02-06 20:47:04.000000 mypy-boto3-customer-profiles-1.26.65/mypy_boto3_customer_profiles/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-02-06 20:47:04.000000 mypy-boto3-customer-profiles-1.26.65/mypy_boto3_customer_profiles/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30531 2023-02-06 20:47:04.000000 mypy-boto3-customer-profiles-1.26.65/mypy_boto3_customer_profiles/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    30486 2023-02-06 20:47:04.000000 mypy-boto3-customer-profiles-1.26.65/mypy_boto3_customer_profiles/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-02-06 20:47:05.000000 mypy-boto3-customer-profiles-1.26.65/mypy_boto3_customer_profiles/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-02-06 20:47:04.000000 mypy-boto3-customer-profiles-1.26.65/mypy_boto3_customer_profiles/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-06 20:47:04.000000 mypy-boto3-customer-profiles-1.26.65/mypy_boto3_customer_profiles/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    49323 2023-02-06 20:47:06.000000 mypy-boto3-customer-profiles-1.26.65/mypy_boto3_customer_profiles/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    49255 2023-02-06 20:47:05.000000 mypy-boto3-customer-profiles-1.26.65/mypy_boto3_customer_profiles/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-06 20:47:04.000000 mypy-boto3-customer-profiles-1.26.65/mypy_boto3_customer_profiles/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 20:47:28.153984 mypy-boto3-customer-profiles-1.26.65/mypy_boto3_customer_profiles.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17482 2023-02-06 20:47:28.000000 mypy-boto3-customer-profiles-1.26.65/mypy_boto3_customer_profiles.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-02-06 20:47:28.000000 mypy-boto3-customer-profiles-1.26.65/mypy_boto3_customer_profiles.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-06 20:47:28.000000 mypy-boto3-customer-profiles-1.26.65/mypy_boto3_customer_profiles.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-06 20:47:28.000000 mypy-boto3-customer-profiles-1.26.65/mypy_boto3_customer_profiles.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-06 20:47:28.000000 mypy-boto3-customer-profiles-1.26.65/mypy_boto3_customer_profiles.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-02-06 20:47:28.000000 mypy-boto3-customer-profiles-1.26.65/mypy_boto3_customer_profiles.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-06 20:47:28.153984 mypy-boto3-customer-profiles-1.26.65/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-02-06 20:47:04.000000 mypy-boto3-customer-profiles-1.26.65/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 20:49:29.644561 mypy-boto3-customer-profiles-1.26.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-14 20:48:51.000000 mypy-boto3-customer-profiles-1.26.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    17430 2022-11-14 20:49:29.644561 mypy-boto3-customer-profiles-1.26.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    15956 2022-11-14 20:48:51.000000 mypy-boto3-customer-profiles-1.26.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 20:49:29.636561 mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles/
+-rw-r--r--   0 runner    (1001) docker     (121)      448 2022-11-14 20:48:51.000000 mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      447 2022-11-14 20:48:51.000000 mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      943 2022-11-14 20:48:51.000000 mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30393 2022-11-14 20:48:51.000000 mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30348 2022-11-14 20:48:51.000000 mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)    11330 2022-11-14 20:48:51.000000 mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles/literals.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11328 2022-11-14 20:48:51.000000 mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-14 20:48:51.000000 mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)    49140 2022-11-14 20:48:53.000000 mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    49072 2022-11-14 20:48:52.000000 mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-14 20:48:51.000000 mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 20:49:29.640561 mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    17430 2022-11-14 20:49:29.000000 mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      785 2022-11-14 20:49:29.000000 mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-14 20:49:29.000000 mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-14 20:49:29.000000 mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-14 20:49:29.000000 mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2022-11-14 20:49:29.000000 mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-14 20:49:29.648561 mypy-boto3-customer-profiles-1.26.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2031 2022-11-14 20:48:50.000000 mypy-boto3-customer-profiles-1.26.9/setup.py
```

### Comparing `mypy-boto3-customer-profiles-1.26.65/LICENSE` & `mypy-boto3-customer-profiles-1.26.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-customer-profiles-1.26.65/PKG-INFO` & `mypy-boto3-customer-profiles-1.26.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-customer-profiles
-Version: 1.26.65
-Summary: Type annotations for boto3.CustomerProfiles 1.26.65 service generated with mypy-boto3-builder 7.12.3
+Version: 1.26.9
+Summary: Type annotations for boto3.CustomerProfiles 1.26.9 service generated with mypy-boto3-builder 7.11.10
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,15 +18,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -38,24 +37,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-customer-profiles.svg?color=blue)](https://pypi.org/project/mypy-boto3-customer-profiles)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-customer-profiles?color=blue)](https://pypistats.org/packages/mypy-boto3-customer-profiles)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CustomerProfiles 1.26.65](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
+[boto3.CustomerProfiles 1.26.9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-customer-profiles docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-customer-profiles-1.26.65/README.md` & `mypy-boto3-customer-profiles-1.26.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-customer-profiles.svg?color=blue)](https://pypi.org/project/mypy-boto3-customer-profiles)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-customer-profiles?color=blue)](https://pypistats.org/packages/mypy-boto3-customer-profiles)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CustomerProfiles 1.26.65](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
+[boto3.CustomerProfiles 1.26.9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-customer-profiles docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-customer-profiles-1.26.65/mypy_boto3_customer_profiles/__main__.py` & `mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CustomerProfiles 1.26.65\nVersion:         1.26.65\nBuilder"
-        " version: 7.12.3\nDocs:           "
+        "Type annotations for boto3.CustomerProfiles 1.26.9\nVersion:         1.26.9\nBuilder"
+        " version: 7.11.10\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.65")
+    print("1.26.9")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-customer-profiles-1.26.65/mypy_boto3_customer_profiles/client.py` & `mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,17 +195,15 @@
         EmailAddress: str = ...,
         PersonalEmailAddress: str = ...,
         BusinessEmailAddress: str = ...,
         Address: AddressTypeDef = ...,
         ShippingAddress: AddressTypeDef = ...,
         MailingAddress: AddressTypeDef = ...,
         BillingAddress: AddressTypeDef = ...,
-        Attributes: Mapping[str, str] = ...,
-        PartyTypeString: str = ...,
-        GenderString: str = ...
+        Attributes: Mapping[str, str] = ...
     ) -> CreateProfileResponseTypeDef:
         """
         Creates a standard profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.create_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#create_profile)
         """
@@ -634,17 +632,15 @@
         EmailAddress: str = ...,
         PersonalEmailAddress: str = ...,
         BusinessEmailAddress: str = ...,
         Address: UpdateAddressTypeDef = ...,
         ShippingAddress: UpdateAddressTypeDef = ...,
         MailingAddress: UpdateAddressTypeDef = ...,
         BillingAddress: UpdateAddressTypeDef = ...,
-        Attributes: Mapping[str, str] = ...,
-        PartyTypeString: str = ...,
-        GenderString: str = ...
+        Attributes: Mapping[str, str] = ...
     ) -> UpdateProfileResponseTypeDef:
         """
         Updates the properties of a profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.update_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#update_profile)
         """
```

### Comparing `mypy-boto3-customer-profiles-1.26.65/mypy_boto3_customer_profiles/client.pyi` & `mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -185,17 +185,15 @@
         EmailAddress: str = ...,
         PersonalEmailAddress: str = ...,
         BusinessEmailAddress: str = ...,
         Address: AddressTypeDef = ...,
         ShippingAddress: AddressTypeDef = ...,
         MailingAddress: AddressTypeDef = ...,
         BillingAddress: AddressTypeDef = ...,
-        Attributes: Mapping[str, str] = ...,
-        PartyTypeString: str = ...,
-        GenderString: str = ...
+        Attributes: Mapping[str, str] = ...
     ) -> CreateProfileResponseTypeDef:
         """
         Creates a standard profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.create_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#create_profile)
         """
@@ -589,17 +587,15 @@
         EmailAddress: str = ...,
         PersonalEmailAddress: str = ...,
         BusinessEmailAddress: str = ...,
         Address: UpdateAddressTypeDef = ...,
         ShippingAddress: UpdateAddressTypeDef = ...,
         MailingAddress: UpdateAddressTypeDef = ...,
         BillingAddress: UpdateAddressTypeDef = ...,
-        Attributes: Mapping[str, str] = ...,
-        PartyTypeString: str = ...,
-        GenderString: str = ...
+        Attributes: Mapping[str, str] = ...
     ) -> UpdateProfileResponseTypeDef:
         """
         Updates the properties of a profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles.Client.update_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/client/#update_profile)
         """
```

### Comparing `mypy-boto3-customer-profiles-1.26.65/mypy_boto3_customer_profiles/literals.py` & `mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -208,15 +208,14 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
-    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -226,31 +225,27 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
-    "chime-sdk-voice",
-    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
-    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
-    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -279,15 +274,14 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
-    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -335,15 +329,14 @@
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -354,33 +347,30 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
-    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
-    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
-    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -412,32 +402,28 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
-    "oam",
-    "omics",
     "opensearch",
-    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
-    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -465,44 +451,39 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
-    "sagemaker-geospatial",
-    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
-    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
-    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
-    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
```

### Comparing `mypy-boto3-customer-profiles-1.26.65/mypy_boto3_customer_profiles/literals.pyi` & `mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles/literals.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -206,15 +206,14 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
-    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -224,31 +223,27 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
-    "chime-sdk-voice",
-    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
-    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
-    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -277,15 +272,14 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
-    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -333,15 +327,14 @@
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -352,33 +345,30 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
-    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
-    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
-    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -410,32 +400,28 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
-    "oam",
-    "omics",
     "opensearch",
-    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
-    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -463,44 +449,39 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
-    "sagemaker-geospatial",
-    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
-    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
-    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
-    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
```

### Comparing `mypy-boto3-customer-profiles-1.26.65/mypy_boto3_customer_profiles/type_defs.py` & `mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1189,16 +1189,14 @@
         "PersonalEmailAddress": str,
         "BusinessEmailAddress": str,
         "Address": AddressTypeDef,
         "ShippingAddress": AddressTypeDef,
         "MailingAddress": AddressTypeDef,
         "BillingAddress": AddressTypeDef,
         "Attributes": Mapping[str, str],
-        "PartyTypeString": str,
-        "GenderString": str,
     },
     total=False,
 )
 
 
 class CreateProfileRequestRequestTypeDef(
     _RequiredCreateProfileRequestRequestTypeDef, _OptionalCreateProfileRequestRequestTypeDef
@@ -1358,16 +1356,14 @@
         "BusinessEmailAddress": str,
         "Address": AddressTypeDef,
         "ShippingAddress": AddressTypeDef,
         "MailingAddress": AddressTypeDef,
         "BillingAddress": AddressTypeDef,
         "Attributes": Dict[str, str],
         "FoundByItems": List[FoundByKeyValueTypeDef],
-        "PartyTypeString": str,
-        "GenderString": str,
     },
     total=False,
 )
 
 GetMatchesResponseTypeDef = TypedDict(
     "GetMatchesResponseTypeDef",
     {
@@ -1598,16 +1594,14 @@
         "PersonalEmailAddress": str,
         "BusinessEmailAddress": str,
         "Address": UpdateAddressTypeDef,
         "ShippingAddress": UpdateAddressTypeDef,
         "MailingAddress": UpdateAddressTypeDef,
         "BillingAddress": UpdateAddressTypeDef,
         "Attributes": Mapping[str, str],
-        "PartyTypeString": str,
-        "GenderString": str,
     },
     total=False,
 )
 
 
 class UpdateProfileRequestRequestTypeDef(
     _RequiredUpdateProfileRequestRequestTypeDef, _OptionalUpdateProfileRequestRequestTypeDef
```

### Comparing `mypy-boto3-customer-profiles-1.26.65/mypy_boto3_customer_profiles/type_defs.pyi` & `mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1154,16 +1154,14 @@
         "PersonalEmailAddress": str,
         "BusinessEmailAddress": str,
         "Address": AddressTypeDef,
         "ShippingAddress": AddressTypeDef,
         "MailingAddress": AddressTypeDef,
         "BillingAddress": AddressTypeDef,
         "Attributes": Mapping[str, str],
-        "PartyTypeString": str,
-        "GenderString": str,
     },
     total=False,
 )
 
 class CreateProfileRequestRequestTypeDef(
     _RequiredCreateProfileRequestRequestTypeDef, _OptionalCreateProfileRequestRequestTypeDef
 ):
@@ -1313,16 +1311,14 @@
         "BusinessEmailAddress": str,
         "Address": AddressTypeDef,
         "ShippingAddress": AddressTypeDef,
         "MailingAddress": AddressTypeDef,
         "BillingAddress": AddressTypeDef,
         "Attributes": Dict[str, str],
         "FoundByItems": List[FoundByKeyValueTypeDef],
-        "PartyTypeString": str,
-        "GenderString": str,
     },
     total=False,
 )
 
 GetMatchesResponseTypeDef = TypedDict(
     "GetMatchesResponseTypeDef",
     {
@@ -1549,16 +1545,14 @@
         "PersonalEmailAddress": str,
         "BusinessEmailAddress": str,
         "Address": UpdateAddressTypeDef,
         "ShippingAddress": UpdateAddressTypeDef,
         "MailingAddress": UpdateAddressTypeDef,
         "BillingAddress": UpdateAddressTypeDef,
         "Attributes": Mapping[str, str],
-        "PartyTypeString": str,
-        "GenderString": str,
     },
     total=False,
 )
 
 class UpdateProfileRequestRequestTypeDef(
     _RequiredUpdateProfileRequestRequestTypeDef, _OptionalUpdateProfileRequestRequestTypeDef
 ):
```

### Comparing `mypy-boto3-customer-profiles-1.26.65/mypy_boto3_customer_profiles.egg-info/PKG-INFO` & `mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-customer-profiles
-Version: 1.26.65
-Summary: Type annotations for boto3.CustomerProfiles 1.26.65 service generated with mypy-boto3-builder 7.12.3
+Version: 1.26.9
+Summary: Type annotations for boto3.CustomerProfiles 1.26.9 service generated with mypy-boto3-builder 7.11.10
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,15 +18,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -38,24 +37,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-customer-profiles.svg?color=blue)](https://pypi.org/project/mypy-boto3-customer-profiles)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-customer-profiles?color=blue)](https://pypistats.org/packages/mypy-boto3-customer-profiles)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CustomerProfiles 1.26.65](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
+[boto3.CustomerProfiles 1.26.9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#CustomerProfiles)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-customer-profiles docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-customer-profiles-1.26.65/mypy_boto3_customer_profiles.egg-info/SOURCES.txt` & `mypy-boto3-customer-profiles-1.26.9/mypy_boto3_customer_profiles.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-customer-profiles-1.26.65/setup.py` & `mypy-boto3-customer-profiles-1.26.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,46 +6,45 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-customer-profiles",
-    version="1.26.65",
+    version="1.26.9",
     packages=["mypy_boto3_customer_profiles"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CustomerProfiles 1.26.65 service generated with"
-        " mypy-boto3-builder 7.12.3"
+        "Type annotations for boto3.CustomerProfiles 1.26.9 service generated with"
+        " mypy-boto3-builder 7.11.10"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
-        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords="boto3 customer-profiles type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"mypy_boto3_customer_profiles": ["py.typed", "*.pyi"]},
+    package_data={"": ["LICENSE"], "mypy_boto3_customer_profiles": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_customer_profiles/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
```

