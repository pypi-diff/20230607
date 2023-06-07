# Comparing `tmp/certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3.tar.gz` & `tmp/certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3.tar", last modified: Wed Jun  7 18:11:52 2023, max compression
+gzip compressed data, was "certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4.tar", last modified: Wed Jun  7 18:12:24 2023, max compression
```

## Comparing `certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3.tar` & `certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 shelly     (501) staff       (20)        0 2023-06-07 18:11:52.949690 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/
--rw-r--r--   0 shelly     (501) staff       (20)     1065 2023-06-07 18:11:52.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/LICENSE
--rw-r--r--   0 shelly     (501) staff       (20)       44 2023-06-07 18:11:52.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/MANIFEST.in
--rw-r--r--   0 shelly     (501) staff       (20)      624 2023-06-07 18:11:52.949519 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/PKG-INFO
--rw-r--r--   0 shelly     (501) staff       (20)       99 2023-06-07 18:11:52.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/README.md
-drwxr-xr-x   0 shelly     (501) staff       (20)        0 2023-06-07 18:11:52.941407 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli/
-drwxr-xr-x   0 shelly     (501) staff       (20)        0 2023-06-07 18:11:52.945203 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli/EVMVerifier/
-drwxr-xr-x   0 shelly     (501) staff       (20)        0 2023-06-07 18:11:52.946532 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli/EVMVerifier/Compiler/
--rw-r--r--   0 shelly     (501) staff       (20)     3620 2023-06-07 17:50:01.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli/EVMVerifier/Compiler/CompilerCollector.py
--rw-r--r--   0 shelly     (501) staff       (20)     6506 2023-06-07 17:50:01.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli/EVMVerifier/Compiler/CompilerCollectorFactory.py
--rw-r--r--   0 shelly     (501) staff       (20)     3313 2023-06-07 17:50:01.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli/EVMVerifier/Compiler/CompilerCollectorSol.py
--rw-r--r--   0 shelly     (501) staff       (20)    20524 2023-06-07 17:50:01.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli/EVMVerifier/Compiler/CompilerCollectorVy.py
--rw-r--r--   0 shelly     (501) staff       (20)       99 2023-04-19 19:52:39.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli/EVMVerifier/Compiler/__init__.py
--rw-r--r--   0 shelly     (501) staff       (20)      159 2023-04-19 19:52:39.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli/EVMVerifier/__init__.py
--rw-r--r--   0 shelly     (501) staff       (20)   184988 2023-06-07 17:50:01.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli/EVMVerifier/certoraBuild.py
--rw-r--r--   0 shelly     (501) staff       (20)    40099 2023-06-07 17:50:01.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli/EVMVerifier/certoraCloudIO.py
--rw-r--r--   0 shelly     (501) staff       (20)     8192 2023-06-07 17:50:01.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli/EVMVerifier/certoraCollectRunMetadata.py
--rw-r--r--   0 shelly     (501) staff       (20)     3741 2023-06-07 17:50:01.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli/EVMVerifier/certoraConfigIO.py
--rwxr-xr-x   0 shelly     (501) staff       (20)    32616 2023-06-07 17:50:01.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli/EVMVerifier/certoraContext.py
--rw-r--r--   0 shelly     (501) staff       (20)    29555 2023-06-07 17:50:01.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli/EVMVerifier/certoraContextAttribute.py
--rw-r--r--   0 shelly     (501) staff       (20)       84 2023-06-07 17:50:01.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli/EVMVerifier/certoraContextClass.py
--rw-r--r--   0 shelly     (501) staff       (20)    44746 2023-06-07 17:50:01.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli/EVMVerifier/certoraContextValidator.py
--rw-r--r--   0 shelly     (501) staff       (20)    10932 2023-05-04 09:01:41.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli/EVMVerifier/certoraJobList.py
--rw-r--r--   0 shelly     (501) staff       (20)     1415 2023-06-07 17:50:01.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli/EVMVerifier/certoraNodeFilters.py
--rw-r--r--   0 shelly     (501) staff       (20)    12774 2023-06-07 17:50:01.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli/EVMVerifier/certoraType.py
--rw-r--r--   0 shelly     (501) staff       (20)    27191 2023-06-07 17:50:01.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli/EVMVerifier/certoraValidateFuncs.py
-drwxr-xr-x   0 shelly     (501) staff       (20)        0 2023-06-07 18:11:52.947521 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli/Shared/
--rw-r--r--   0 shelly     (501) staff       (20)      333 2023-04-19 19:52:39.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli/Shared/__init__.py
--rw-r--r--   0 shelly     (501) staff       (20)    13275 2023-05-04 11:23:56.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli/Shared/certoraLogging.py
--rw-r--r--   0 shelly     (501) staff       (20)     5575 2023-06-07 17:50:01.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli/Shared/certoraTester.py
--rw-r--r--   0 shelly     (501) staff       (20)    40311 2023-06-07 17:50:01.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli/Shared/certoraUtils.py
--rw-r--r--   0 shelly     (501) staff       (20)        0 2023-06-07 18:11:52.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli/__init__.py
-drwxr-xr-x   0 shelly     (501) staff       (20)        0 2023-06-07 18:11:52.949050 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli_alpha_shelly_whenwillitbeoverinternalfunctions.egg-info/
--rw-r--r--   0 shelly     (501) staff       (20)      624 2023-06-07 18:11:52.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli_alpha_shelly_whenwillitbeoverinternalfunctions.egg-info/PKG-INFO
--rw-r--r--   0 shelly     (501) staff       (20)     1573 2023-06-07 18:11:52.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli_alpha_shelly_whenwillitbeoverinternalfunctions.egg-info/SOURCES.txt
--rw-r--r--   0 shelly     (501) staff       (20)        1 2023-06-07 18:11:52.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli_alpha_shelly_whenwillitbeoverinternalfunctions.egg-info/dependency_links.txt
--rw-r--r--   0 shelly     (501) staff       (20)      131 2023-06-07 18:11:52.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli_alpha_shelly_whenwillitbeoverinternalfunctions.egg-info/entry_points.txt
--rw-r--r--   0 shelly     (501) staff       (20)       58 2023-06-07 18:11:52.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli_alpha_shelly_whenwillitbeoverinternalfunctions.egg-info/requires.txt
--rw-r--r--   0 shelly     (501) staff       (20)       25 2023-06-07 18:11:52.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli_alpha_shelly_whenwillitbeoverinternalfunctions.egg-info/top_level.txt
-drwxr-xr-x   0 shelly     (501) staff       (20)        0 2023-06-07 18:11:52.949276 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_jars/
--rw-r--r--   0 shelly     (501) staff       (20)        0 2023-06-07 18:11:52.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_jars/__init__.py
--rw-r--r--   0 shelly     (501) staff       (20)       38 2023-06-07 18:11:52.949731 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/setup.cfg
--rw-r--r--   0 shelly     (501) staff       (20)     1228 2023-06-07 18:11:52.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/setup.py
+drwxr-xr-x   0 shelly     (501) staff       (20)        0 2023-06-07 18:12:24.601275 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/
+-rw-r--r--   0 shelly     (501) staff       (20)     1065 2023-06-07 18:12:24.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/LICENSE
+-rw-r--r--   0 shelly     (501) staff       (20)       44 2023-06-07 18:12:24.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/MANIFEST.in
+-rw-r--r--   0 shelly     (501) staff       (20)      624 2023-06-07 18:12:24.601139 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/PKG-INFO
+-rw-r--r--   0 shelly     (501) staff       (20)       99 2023-06-07 18:12:24.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/README.md
+drwxr-xr-x   0 shelly     (501) staff       (20)        0 2023-06-07 18:12:24.594161 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli/
+drwxr-xr-x   0 shelly     (501) staff       (20)        0 2023-06-07 18:12:24.597394 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli/EVMVerifier/
+drwxr-xr-x   0 shelly     (501) staff       (20)        0 2023-06-07 18:12:24.598665 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli/EVMVerifier/Compiler/
+-rw-r--r--   0 shelly     (501) staff       (20)     3620 2023-06-07 17:50:01.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli/EVMVerifier/Compiler/CompilerCollector.py
+-rw-r--r--   0 shelly     (501) staff       (20)     6506 2023-06-07 17:50:01.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli/EVMVerifier/Compiler/CompilerCollectorFactory.py
+-rw-r--r--   0 shelly     (501) staff       (20)     3313 2023-06-07 17:50:01.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli/EVMVerifier/Compiler/CompilerCollectorSol.py
+-rw-r--r--   0 shelly     (501) staff       (20)    20524 2023-06-07 17:50:01.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli/EVMVerifier/Compiler/CompilerCollectorVy.py
+-rw-r--r--   0 shelly     (501) staff       (20)       99 2023-04-19 19:52:39.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli/EVMVerifier/Compiler/__init__.py
+-rw-r--r--   0 shelly     (501) staff       (20)      159 2023-04-19 19:52:39.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli/EVMVerifier/__init__.py
+-rw-r--r--   0 shelly     (501) staff       (20)   184988 2023-06-07 17:50:01.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli/EVMVerifier/certoraBuild.py
+-rw-r--r--   0 shelly     (501) staff       (20)    40099 2023-06-07 17:50:01.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli/EVMVerifier/certoraCloudIO.py
+-rw-r--r--   0 shelly     (501) staff       (20)     8192 2023-06-07 17:50:01.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli/EVMVerifier/certoraCollectRunMetadata.py
+-rw-r--r--   0 shelly     (501) staff       (20)     3741 2023-06-07 17:50:01.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli/EVMVerifier/certoraConfigIO.py
+-rwxr-xr-x   0 shelly     (501) staff       (20)    32616 2023-06-07 17:50:01.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli/EVMVerifier/certoraContext.py
+-rw-r--r--   0 shelly     (501) staff       (20)    29555 2023-06-07 17:50:01.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli/EVMVerifier/certoraContextAttribute.py
+-rw-r--r--   0 shelly     (501) staff       (20)       84 2023-06-07 17:50:01.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli/EVMVerifier/certoraContextClass.py
+-rw-r--r--   0 shelly     (501) staff       (20)    44746 2023-06-07 17:50:01.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli/EVMVerifier/certoraContextValidator.py
+-rw-r--r--   0 shelly     (501) staff       (20)    10932 2023-05-04 09:01:41.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli/EVMVerifier/certoraJobList.py
+-rw-r--r--   0 shelly     (501) staff       (20)     1415 2023-06-07 17:50:01.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli/EVMVerifier/certoraNodeFilters.py
+-rw-r--r--   0 shelly     (501) staff       (20)    12774 2023-06-07 17:50:01.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli/EVMVerifier/certoraType.py
+-rw-r--r--   0 shelly     (501) staff       (20)    27191 2023-06-07 17:50:01.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli/EVMVerifier/certoraValidateFuncs.py
+drwxr-xr-x   0 shelly     (501) staff       (20)        0 2023-06-07 18:12:24.599464 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli/Shared/
+-rw-r--r--   0 shelly     (501) staff       (20)      333 2023-04-19 19:52:39.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli/Shared/__init__.py
+-rw-r--r--   0 shelly     (501) staff       (20)    13275 2023-05-04 11:23:56.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli/Shared/certoraLogging.py
+-rw-r--r--   0 shelly     (501) staff       (20)     5575 2023-06-07 17:50:01.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli/Shared/certoraTester.py
+-rw-r--r--   0 shelly     (501) staff       (20)    40311 2023-06-07 17:50:01.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli/Shared/certoraUtils.py
+-rw-r--r--   0 shelly     (501) staff       (20)        0 2023-06-07 18:12:24.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli/__init__.py
+drwxr-xr-x   0 shelly     (501) staff       (20)        0 2023-06-07 18:12:24.600742 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli_alpha_shelly_whenwillitbeoverinternalfunctions.egg-info/
+-rw-r--r--   0 shelly     (501) staff       (20)      624 2023-06-07 18:12:24.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli_alpha_shelly_whenwillitbeoverinternalfunctions.egg-info/PKG-INFO
+-rw-r--r--   0 shelly     (501) staff       (20)     1573 2023-06-07 18:12:24.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli_alpha_shelly_whenwillitbeoverinternalfunctions.egg-info/SOURCES.txt
+-rw-r--r--   0 shelly     (501) staff       (20)        1 2023-06-07 18:12:24.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli_alpha_shelly_whenwillitbeoverinternalfunctions.egg-info/dependency_links.txt
+-rw-r--r--   0 shelly     (501) staff       (20)      131 2023-06-07 18:12:24.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli_alpha_shelly_whenwillitbeoverinternalfunctions.egg-info/entry_points.txt
+-rw-r--r--   0 shelly     (501) staff       (20)       58 2023-06-07 18:12:24.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli_alpha_shelly_whenwillitbeoverinternalfunctions.egg-info/requires.txt
+-rw-r--r--   0 shelly     (501) staff       (20)       25 2023-06-07 18:12:24.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli_alpha_shelly_whenwillitbeoverinternalfunctions.egg-info/top_level.txt
+drwxr-xr-x   0 shelly     (501) staff       (20)        0 2023-06-07 18:12:24.600924 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_jars/
+-rw-r--r--   0 shelly     (501) staff       (20)        0 2023-06-07 18:12:24.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_jars/__init__.py
+-rw-r--r--   0 shelly     (501) staff       (20)       38 2023-06-07 18:12:24.601308 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/setup.cfg
+-rw-r--r--   0 shelly     (501) staff       (20)     1228 2023-06-07 18:12:24.000000 certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/setup.py
```

### Comparing `certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/LICENSE` & `certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/LICENSE`

 * *Files identical despite different names*

### Comparing `certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/PKG-INFO` & `certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions
-Version: 3.6.8.post3
+Version: 3.6.8.post4
 Summary: Runner for the Certora Prover
 Home-page: https://pypi.org/project/certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions
 Author: Certora
 Author-email: support@certora.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli/EVMVerifier/Compiler/CompilerCollector.py` & `certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli/EVMVerifier/Compiler/CompilerCollector.py`

 * *Files identical despite different names*

### Comparing `certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli/EVMVerifier/Compiler/CompilerCollectorFactory.py` & `certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli/EVMVerifier/Compiler/CompilerCollectorFactory.py`

 * *Files identical despite different names*

### Comparing `certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli/EVMVerifier/Compiler/CompilerCollectorSol.py` & `certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli/EVMVerifier/Compiler/CompilerCollectorSol.py`

 * *Files identical despite different names*

### Comparing `certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli/EVMVerifier/Compiler/CompilerCollectorVy.py` & `certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli/EVMVerifier/Compiler/CompilerCollectorVy.py`

 * *Files identical despite different names*

### Comparing `certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli/EVMVerifier/certoraBuild.py` & `certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli/EVMVerifier/certoraBuild.py`

 * *Files identical despite different names*

### Comparing `certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli/EVMVerifier/certoraCloudIO.py` & `certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli/EVMVerifier/certoraCloudIO.py`

 * *Files identical despite different names*

### Comparing `certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli/EVMVerifier/certoraCollectRunMetadata.py` & `certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli/EVMVerifier/certoraCollectRunMetadata.py`

 * *Files identical despite different names*

### Comparing `certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli/EVMVerifier/certoraConfigIO.py` & `certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli/EVMVerifier/certoraConfigIO.py`

 * *Files identical despite different names*

### Comparing `certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli/EVMVerifier/certoraContext.py` & `certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli/EVMVerifier/certoraContext.py`

 * *Files identical despite different names*

### Comparing `certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli/EVMVerifier/certoraContextAttribute.py` & `certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli/EVMVerifier/certoraContextAttribute.py`

 * *Files identical despite different names*

### Comparing `certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli/EVMVerifier/certoraContextValidator.py` & `certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli/EVMVerifier/certoraContextValidator.py`

 * *Files identical despite different names*

### Comparing `certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli/EVMVerifier/certoraJobList.py` & `certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli/EVMVerifier/certoraJobList.py`

 * *Files identical despite different names*

### Comparing `certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli/EVMVerifier/certoraNodeFilters.py` & `certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli/EVMVerifier/certoraNodeFilters.py`

 * *Files identical despite different names*

### Comparing `certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli/EVMVerifier/certoraType.py` & `certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli/EVMVerifier/certoraType.py`

 * *Files identical despite different names*

### Comparing `certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli/EVMVerifier/certoraValidateFuncs.py` & `certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli/EVMVerifier/certoraValidateFuncs.py`

 * *Files identical despite different names*

### Comparing `certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli/Shared/certoraLogging.py` & `certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli/Shared/certoraLogging.py`

 * *Files identical despite different names*

### Comparing `certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli/Shared/certoraTester.py` & `certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli/Shared/certoraTester.py`

 * *Files identical despite different names*

### Comparing `certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli/Shared/certoraUtils.py` & `certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli/Shared/certoraUtils.py`

 * *Files identical despite different names*

### Comparing `certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli_alpha_shelly_whenwillitbeoverinternalfunctions.egg-info/PKG-INFO` & `certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli_alpha_shelly_whenwillitbeoverinternalfunctions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions
-Version: 3.6.8.post3
+Version: 3.6.8.post4
 Summary: Runner for the Certora Prover
 Home-page: https://pypi.org/project/certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions
 Author: Certora
 Author-email: support@certora.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/certora_cli_alpha_shelly_whenwillitbeoverinternalfunctions.egg-info/SOURCES.txt` & `certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/certora_cli_alpha_shelly_whenwillitbeoverinternalfunctions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post3/setup.py` & `certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions-3.6.8.post4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 import setuptools
 
 if __name__ == "__main__":
     setuptools.setup(
         name="certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions",
-        version="3.6.8-3",
+        version="3.6.8-4",
         author="Certora",
         author_email="support@certora.com",
         description="Runner for the Certora Prover",
         long_description="Commit 97e72b6. Build and Run scripts for executing the Certora Prover on Solidity smart contracts.",
         long_description_content_type="text/markdown",
         url="https://pypi.org/project/certora-cli-alpha-shelly-whenwillitbeoverinternalfunctions",
         packages=setuptools.find_packages(),
```

