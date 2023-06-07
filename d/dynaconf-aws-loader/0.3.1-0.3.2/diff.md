# Comparing `tmp/dynaconf_aws_loader-0.3.1.tar.gz` & `tmp/dynaconf_aws_loader-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynaconf_aws_loader-0.3.1.tar", max compression
+gzip compressed data, was "dynaconf_aws_loader-0.3.2.tar", max compression
```

## Comparing `dynaconf_aws_loader-0.3.1.tar` & `dynaconf_aws_loader-0.3.2.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1072 2023-06-06 19:25:26.067428 dynaconf_aws_loader-0.3.1/LICENSE
--rw-r--r--   0        0        0     6557 2023-06-06 19:25:26.067428 dynaconf_aws_loader-0.3.1/README.rst
--rw-r--r--   0        0        0      369 2023-06-06 19:25:26.067428 dynaconf_aws_loader-0.3.1/dynaconf_aws_loader/__init__.py
--rw-r--r--   0        0        0     5702 2023-06-06 19:25:26.067428 dynaconf_aws_loader-0.3.1/dynaconf_aws_loader/loader.py
--rw-r--r--   0        0        0      757 2023-06-06 19:25:26.067428 dynaconf_aws_loader-0.3.1/dynaconf_aws_loader/util.py
--rw-r--r--   0        0        0     1100 2023-06-06 19:25:26.067428 dynaconf_aws_loader-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     7512 1970-01-01 00:00:00.000000 dynaconf_aws_loader-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      282 2023-06-07 19:08:03.503127 dynaconf_aws_loader-0.3.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1072 2023-06-07 19:08:03.503127 dynaconf_aws_loader-0.3.2/LICENSE
+-rw-r--r--   0        0        0     6557 2023-06-07 19:08:03.503127 dynaconf_aws_loader-0.3.2/README.rst
+-rw-r--r--   0        0        0      369 2023-06-07 19:08:03.503127 dynaconf_aws_loader-0.3.2/dynaconf_aws_loader/__init__.py
+-rw-r--r--   0        0        0     5702 2023-06-07 19:08:03.503127 dynaconf_aws_loader-0.3.2/dynaconf_aws_loader/loader.py
+-rw-r--r--   0        0        0      757 2023-06-07 19:08:03.503127 dynaconf_aws_loader-0.3.2/dynaconf_aws_loader/util.py
+-rw-r--r--   0        0        0     1249 2023-06-07 19:08:03.503127 dynaconf_aws_loader-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     7648 1970-01-01 00:00:00.000000 dynaconf_aws_loader-0.3.2/PKG-INFO
```

### Comparing `dynaconf_aws_loader-0.3.1/LICENSE` & `dynaconf_aws_loader-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dynaconf_aws_loader-0.3.1/README.rst` & `dynaconf_aws_loader-0.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `dynaconf_aws_loader-0.3.1/dynaconf_aws_loader/loader.py` & `dynaconf_aws_loader-0.3.2/dynaconf_aws_loader/loader.py`

 * *Files identical despite different names*

### Comparing `dynaconf_aws_loader-0.3.1/dynaconf_aws_loader/util.py` & `dynaconf_aws_loader-0.3.2/dynaconf_aws_loader/util.py`

 * *Files identical despite different names*

### Comparing `dynaconf_aws_loader-0.3.1/pyproject.toml` & `dynaconf_aws_loader-0.3.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 [tool.poetry]
 name = "dynaconf-aws-loader"
-version = "0.3.1"
+version = "0.3.2"
 description = "A custom loader for Dynaconf that uses AWS Systems Manager Parameter Store as a source of truth"
+homepage = "https://github.com/fictivekin/dynaconf-aws-loader"
+repository = "https://github.com/fictivekin/dynaconf-aws-loader"
 authors = [
     "Joël Perras <joel@fictivekin.com>",
 ]
 readme = "README.rst"
 packages = [{include = "dynaconf_aws_loader"}]
 license = "MIT"
 keywords = ["dynaconf", "AWS", "SSM"]
 classifiers = [
     "Environment :: Console",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Documentation",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 include = [
-    "LICENSE"
+    "LICENSE",
+    "CHANGELOG.md"
 ]
 
+
 [tool.poetry.dependencies]
 python = "^3.8"
 boto3 = "^1.26"
 botocore = "^1.29"
 dynaconf = "^3.1"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `dynaconf_aws_loader-0.3.1/PKG-INFO` & `dynaconf_aws_loader-0.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: dynaconf-aws-loader
-Version: 0.3.1
+Version: 0.3.2
 Summary: A custom loader for Dynaconf that uses AWS Systems Manager Parameter Store as a source of truth
+Home-page: https://github.com/fictivekin/dynaconf-aws-loader
 License: MIT
 Keywords: dynaconf,AWS,SSM
 Author: Joël Perras
 Author-email: joel@fictivekin.com
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
@@ -16,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: boto3 (>=1.26,<2.0)
 Requires-Dist: botocore (>=1.29,<2.0)
 Requires-Dist: dynaconf (>=3.1,<4.0)
+Project-URL: Repository, https://github.com/fictivekin/dynaconf-aws-loader
 Description-Content-Type: text/x-rst
 
 Dynaconf AWS Systems Manager Parameter Store Loader
 ====================================================
 
 When configured, this loader will permit Dynaconf to query `AWS Systems Manager Parameter Store <https://docs.aws.amazon.com/systems-manager/latest/userguide/systems-manager-parameter-store.html>`_ for slash-delimited hierarchical configuration data.
```

