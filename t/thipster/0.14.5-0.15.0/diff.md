# Comparing `tmp/thipster-0.14.5.tar.gz` & `tmp/thipster-0.15.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thipster-0.14.5.tar", last modified: Wed Jun  7 12:44:36 2023, max compression
+gzip compressed data, was "thipster-0.15.0.tar", last modified: Wed Jun  7 15:19:35 2023, max compression
```

## Comparing `thipster-0.14.5.tar` & `thipster-0.15.0.tar`

### file list

```diff
@@ -1,77 +1,71 @@
-drwxr-xr-x   0 rcattin   (1000) rcattin   (1000)        0 2023-06-07 12:44:36.213512 thipster-0.14.5/
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)     1052 2023-06-07 09:14:11.000000 thipster-0.14.5/LICENSE
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)       81 2023-06-07 09:14:11.000000 thipster-0.14.5/MANIFEST.in
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)     4003 2023-06-07 12:44:36.213512 thipster-0.14.5/PKG-INFO
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)     3390 2023-06-06 10:08:32.000000 thipster-0.14.5/README.md
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)      916 2023-06-07 12:43:52.000000 thipster-0.14.5/pyproject.toml
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)      137 2023-06-07 09:14:11.000000 thipster-0.14.5/requirements.txt
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)       38 2023-06-07 12:44:36.213512 thipster-0.14.5/setup.cfg
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)     1372 2023-06-07 12:43:57.000000 thipster-0.14.5/setup.py
-drwxr-xr-x   0 rcattin   (1000) rcattin   (1000)        0 2023-06-07 12:44:36.173512 thipster-0.14.5/tests/
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)        0 2023-04-26 14:12:09.000000 thipster-0.14.5/tests/__init__.py
-drwxr-xr-x   0 rcattin   (1000) rcattin   (1000)        0 2023-06-07 12:44:36.173512 thipster-0.14.5/tests/engine/
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)        0 2023-04-20 08:57:48.000000 thipster-0.14.5/tests/engine/__init__.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)     3222 2023-06-06 14:38:25.000000 thipster-0.14.5/tests/engine/test_engine.py
-drwxr-xr-x   0 rcattin   (1000) rcattin   (1000)        0 2023-06-07 12:44:36.173512 thipster-0.14.5/tests/parser/
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)        0 2023-04-20 08:57:48.000000 thipster-0.14.5/tests/parser/__init__.py
-drwxr-xr-x   0 rcattin   (1000) rcattin   (1000)        0 2023-06-07 12:44:36.173512 thipster-0.14.5/tests/parser/dsl_parser/
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)        0 2023-04-21 13:59:54.000000 thipster-0.14.5/tests/parser/dsl_parser/__init__.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)    15548 2023-06-07 09:14:11.000000 thipster-0.14.5/tests/parser/dsl_parser/test_DSLparser.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)     1358 2023-06-06 14:38:25.000000 thipster-0.14.5/tests/parser/dsl_parser/test_ast.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)    13297 2023-06-06 14:38:25.000000 thipster-0.14.5/tests/parser/dsl_parser/test_lexer.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)      862 2023-06-06 14:38:25.000000 thipster-0.14.5/tests/parser/dsl_parser/test_token.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)     3524 2023-06-06 14:38:25.000000 thipster-0.14.5/tests/parser/dsl_parser/test_tokenparser.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)     3010 2023-06-06 14:38:25.000000 thipster-0.14.5/tests/parser/test_ParserFactory.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)     4956 2023-06-06 14:38:25.000000 thipster-0.14.5/tests/parser/test_YAMLParser.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)     4683 2023-06-06 14:38:25.000000 thipster-0.14.5/tests/parser/test_parsedfile.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)     6934 2023-06-07 12:43:52.000000 thipster-0.14.5/tests/test_e2e.py
-drwxr-xr-x   0 rcattin   (1000) rcattin   (1000)        0 2023-06-07 12:44:36.173512 thipster-0.14.5/thipster/
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)      171 2023-06-06 14:38:25.000000 thipster-0.14.5/thipster/__init__.py
-drwxr-xr-x   0 rcattin   (1000) rcattin   (1000)        0 2023-06-07 12:44:36.183512 thipster-0.14.5/thipster/auth/
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)      215 2023-06-06 14:38:25.000000 thipster-0.14.5/thipster/auth/__init__.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)      941 2023-06-07 12:43:57.000000 thipster-0.14.5/thipster/auth/google.py
-drwxr-xr-x   0 rcattin   (1000) rcattin   (1000)        0 2023-06-07 12:44:36.183512 thipster-0.14.5/thipster/engine/
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)      369 2023-06-06 14:38:25.000000 thipster-0.14.5/thipster/engine/__init__.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)     4949 2023-06-07 12:43:57.000000 thipster-0.14.5/thipster/engine/engine.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)      410 2023-06-07 12:43:57.000000 thipster-0.14.5/thipster/engine/i_auth.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)      726 2023-06-06 14:38:25.000000 thipster-0.14.5/thipster/engine/i_parser.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)      597 2023-06-06 14:38:25.000000 thipster-0.14.5/thipster/engine/i_repository.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)     1815 2023-06-07 12:43:57.000000 thipster-0.14.5/thipster/engine/i_terraform.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)     6023 2023-06-06 14:38:25.000000 thipster-0.14.5/thipster/engine/parsed_file.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)     4125 2023-06-07 09:00:27.000000 thipster-0.14.5/thipster/engine/resource_model.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)      654 2023-06-07 12:43:57.000000 thipster-0.14.5/thipster/helpers.py
-drwxr-xr-x   0 rcattin   (1000) rcattin   (1000)        0 2023-06-07 12:44:36.183512 thipster-0.14.5/thipster/parser/
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)      364 2023-06-07 09:14:11.000000 thipster-0.14.5/thipster/parser/__init__.py
-drwxr-xr-x   0 rcattin   (1000) rcattin   (1000)        0 2023-06-07 12:44:36.183512 thipster-0.14.5/thipster/parser/dsl_parser/
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)       30 2023-06-06 14:38:25.000000 thipster-0.14.5/thipster/parser/dsl_parser/__init__.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)    10326 2023-06-07 09:14:11.000000 thipster-0.14.5/thipster/parser/dsl_parser/ast.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)     1811 2023-06-06 14:38:25.000000 thipster-0.14.5/thipster/parser/dsl_parser/exceptions.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)    13708 2023-06-07 09:14:11.000000 thipster-0.14.5/thipster/parser/dsl_parser/interpreter.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)    17264 2023-06-07 12:43:57.000000 thipster-0.14.5/thipster/parser/dsl_parser/lexer.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)     4771 2023-06-06 14:38:25.000000 thipster-0.14.5/thipster/parser/dsl_parser/lexer_position.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)     1944 2023-06-06 14:38:25.000000 thipster-0.14.5/thipster/parser/dsl_parser/parser.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)     2290 2023-06-06 14:38:25.000000 thipster-0.14.5/thipster/parser/dsl_parser/token.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)    19125 2023-06-07 09:14:11.000000 thipster-0.14.5/thipster/parser/dsl_parser/token_parser.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)     2254 2023-06-07 09:14:11.000000 thipster-0.14.5/thipster/parser/parser_factory.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)     6275 2023-06-07 09:14:11.000000 thipster-0.14.5/thipster/parser/yaml_parser.py
-drwxr-xr-x   0 rcattin   (1000) rcattin   (1000)        0 2023-06-07 12:44:36.183512 thipster-0.14.5/thipster/repository/
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)      332 2023-06-07 09:14:11.000000 thipster-0.14.5/thipster/repository/__init__.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)     1284 2023-06-07 12:43:57.000000 thipster-0.14.5/thipster/repository/github.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)     4652 2023-06-06 14:38:25.000000 thipster-0.14.5/thipster/repository/json.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)      347 2023-06-06 14:38:25.000000 thipster-0.14.5/thipster/repository/local.py
-drwxr-xr-x   0 rcattin   (1000) rcattin   (1000)        0 2023-06-07 12:44:36.183512 thipster-0.14.5/thipster/terraform/
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)      327 2023-06-06 14:38:25.000000 thipster-0.14.5/thipster/terraform/__init__.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)    19903 2023-06-07 12:43:57.000000 thipster-0.14.5/thipster/terraform/cdk.py
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)     1119 2023-06-06 14:38:25.000000 thipster-0.14.5/thipster/terraform/exceptions.py
-drwxr-xr-x   0 rcattin   (1000) rcattin   (1000)        0 2023-06-07 12:44:36.203512 thipster-0.14.5/thipster/thipster.egg-info/
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)     1265 2023-05-30 13:56:10.000000 thipster-0.14.5/thipster/thipster.egg-info/SOURCES.txt
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)        1 2023-05-30 13:56:10.000000 thipster-0.14.5/thipster/thipster.egg-info/dependency_links.txt
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)       44 2023-05-30 13:56:10.000000 thipster-0.14.5/thipster/thipster.egg-info/entry_points.txt
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)      205 2023-05-30 13:56:10.000000 thipster-0.14.5/thipster/thipster.egg-info/requires.txt
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)       57 2023-05-30 13:56:10.000000 thipster-0.14.5/thipster/thipster.egg-info/top_level.txt
-drwxr-xr-x   0 rcattin   (1000) rcattin   (1000)        0 2023-06-07 12:44:36.183512 thipster-0.14.5/thipster.egg-info/
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)     4003 2023-06-07 12:44:36.000000 thipster-0.14.5/thipster.egg-info/PKG-INFO
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)     1870 2023-06-07 12:44:36.000000 thipster-0.14.5/thipster.egg-info/SOURCES.txt
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)        1 2023-06-07 12:44:36.000000 thipster-0.14.5/thipster.egg-info/dependency_links.txt
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)      237 2023-06-07 12:44:36.000000 thipster-0.14.5/thipster.egg-info/requires.txt
--rw-r--r--   0 rcattin   (1000) rcattin   (1000)       15 2023-06-07 12:44:36.000000 thipster-0.14.5/thipster.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 15:19:35.599076 thipster-0.15.0/
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-06-07 15:19:32.000000 thipster-0.15.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       81 2023-06-07 15:19:32.000000 thipster-0.15.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4003 2023-06-07 15:19:35.599076 thipster-0.15.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3390 2023-06-07 15:19:32.000000 thipster-0.15.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      916 2023-06-07 15:19:32.000000 thipster-0.15.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      137 2023-06-07 15:19:32.000000 thipster-0.15.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-07 15:19:35.599076 thipster-0.15.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1372 2023-06-07 15:19:32.000000 thipster-0.15.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 15:19:35.591076 thipster-0.15.0/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 15:19:32.000000 thipster-0.15.0/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 15:19:35.591076 thipster-0.15.0/tests/engine/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 15:19:32.000000 thipster-0.15.0/tests/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3222 2023-06-07 15:19:32.000000 thipster-0.15.0/tests/engine/test_engine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 15:19:35.591076 thipster-0.15.0/tests/parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 15:19:32.000000 thipster-0.15.0/tests/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 15:19:35.595076 thipster-0.15.0/tests/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 15:19:32.000000 thipster-0.15.0/tests/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15548 2023-06-07 15:19:32.000000 thipster-0.15.0/tests/parser/dsl_parser/test_DSLparser.py
+-rw-r--r--   0 root         (0) root         (0)     1358 2023-06-07 15:19:32.000000 thipster-0.15.0/tests/parser/dsl_parser/test_ast.py
+-rw-r--r--   0 root         (0) root         (0)    13297 2023-06-07 15:19:32.000000 thipster-0.15.0/tests/parser/dsl_parser/test_lexer.py
+-rw-r--r--   0 root         (0) root         (0)      862 2023-06-07 15:19:32.000000 thipster-0.15.0/tests/parser/dsl_parser/test_token.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2023-06-07 15:19:32.000000 thipster-0.15.0/tests/parser/dsl_parser/test_tokenparser.py
+-rw-r--r--   0 root         (0) root         (0)     3010 2023-06-07 15:19:32.000000 thipster-0.15.0/tests/parser/test_ParserFactory.py
+-rw-r--r--   0 root         (0) root         (0)     4956 2023-06-07 15:19:32.000000 thipster-0.15.0/tests/parser/test_YAMLParser.py
+-rw-r--r--   0 root         (0) root         (0)     4683 2023-06-07 15:19:32.000000 thipster-0.15.0/tests/parser/test_parsedfile.py
+-rw-r--r--   0 root         (0) root         (0)     6934 2023-06-07 15:19:32.000000 thipster-0.15.0/tests/test_e2e.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 15:19:35.595076 thipster-0.15.0/thipster/
+-rw-r--r--   0 root         (0) root         (0)      171 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 15:19:35.595076 thipster-0.15.0/thipster/auth/
+-rw-r--r--   0 root         (0) root         (0)      215 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      941 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/auth/google.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 15:19:35.595076 thipster-0.15.0/thipster/engine/
+-rw-r--r--   0 root         (0) root         (0)      369 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/engine/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5111 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/engine/engine.py
+-rw-r--r--   0 root         (0) root         (0)      410 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/engine/i_auth.py
+-rw-r--r--   0 root         (0) root         (0)      726 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/engine/i_parser.py
+-rw-r--r--   0 root         (0) root         (0)      597 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/engine/i_repository.py
+-rw-r--r--   0 root         (0) root         (0)     1815 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/engine/i_terraform.py
+-rw-r--r--   0 root         (0) root         (0)     6023 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/engine/parsed_file.py
+-rw-r--r--   0 root         (0) root         (0)     4125 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/engine/resource_model.py
+-rw-r--r--   0 root         (0) root         (0)      654 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 15:19:35.599076 thipster-0.15.0/thipster/parser/
+-rw-r--r--   0 root         (0) root         (0)      364 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/parser/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 15:19:35.599076 thipster-0.15.0/thipster/parser/dsl_parser/
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/parser/dsl_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10326 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/parser/dsl_parser/ast.py
+-rw-r--r--   0 root         (0) root         (0)     1811 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/parser/dsl_parser/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    13708 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/parser/dsl_parser/interpreter.py
+-rw-r--r--   0 root         (0) root         (0)    17264 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/parser/dsl_parser/lexer.py
+-rw-r--r--   0 root         (0) root         (0)     4771 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/parser/dsl_parser/lexer_position.py
+-rw-r--r--   0 root         (0) root         (0)     1944 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/parser/dsl_parser/parser.py
+-rw-r--r--   0 root         (0) root         (0)     2290 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/parser/dsl_parser/token.py
+-rw-r--r--   0 root         (0) root         (0)    19125 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/parser/dsl_parser/token_parser.py
+-rw-r--r--   0 root         (0) root         (0)     2254 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/parser/parser_factory.py
+-rw-r--r--   0 root         (0) root         (0)     6275 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/parser/yaml_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 15:19:35.599076 thipster-0.15.0/thipster/repository/
+-rw-r--r--   0 root         (0) root         (0)      332 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/repository/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1284 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/repository/github.py
+-rw-r--r--   0 root         (0) root         (0)     4652 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/repository/json.py
+-rw-r--r--   0 root         (0) root         (0)      347 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/repository/local.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 15:19:35.599076 thipster-0.15.0/thipster/terraform/
+-rw-r--r--   0 root         (0) root         (0)      327 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/terraform/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19903 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/terraform/cdk.py
+-rw-r--r--   0 root         (0) root         (0)     1119 2023-06-07 15:19:32.000000 thipster-0.15.0/thipster/terraform/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 15:19:35.595076 thipster-0.15.0/thipster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4003 2023-06-07 15:19:35.000000 thipster-0.15.0/thipster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1658 2023-06-07 15:19:35.000000 thipster-0.15.0/thipster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 15:19:35.000000 thipster-0.15.0/thipster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      237 2023-06-07 15:19:35.000000 thipster-0.15.0/thipster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-07 15:19:35.000000 thipster-0.15.0/thipster.egg-info/top_level.txt
```

### Comparing `thipster-0.14.5/LICENSE` & `thipster-0.15.0/LICENSE`

 * *Files identical despite different names*

### Comparing `thipster-0.14.5/PKG-INFO` & `thipster-0.15.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.14.5
+Version: 0.15.0
 Summary: THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files. It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `thipster-0.14.5/README.md` & `thipster-0.15.0/README.md`

 * *Files identical despite different names*

### Comparing `thipster-0.14.5/pyproject.toml` & `thipster-0.15.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `thipster-0.14.5/setup.py` & `thipster-0.15.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-__version__ = '0.14.5'
+__version__ = '0.15.0'
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 with open('README.md') as rm:
     readme = rm.read()
```

### Comparing `thipster-0.14.5/tests/engine/test_engine.py` & `thipster-0.15.0/tests/engine/test_engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.5/tests/parser/dsl_parser/test_DSLparser.py` & `thipster-0.15.0/tests/parser/dsl_parser/test_DSLparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.5/tests/parser/dsl_parser/test_ast.py` & `thipster-0.15.0/tests/parser/dsl_parser/test_ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.5/tests/parser/dsl_parser/test_lexer.py` & `thipster-0.15.0/tests/parser/dsl_parser/test_lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.5/tests/parser/dsl_parser/test_token.py` & `thipster-0.15.0/tests/parser/dsl_parser/test_token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.5/tests/parser/dsl_parser/test_tokenparser.py` & `thipster-0.15.0/tests/parser/dsl_parser/test_tokenparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.5/tests/parser/test_ParserFactory.py` & `thipster-0.15.0/tests/parser/test_ParserFactory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.5/tests/parser/test_YAMLParser.py` & `thipster-0.15.0/tests/parser/test_YAMLParser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.5/tests/parser/test_parsedfile.py` & `thipster-0.15.0/tests/parser/test_parsedfile.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.5/tests/test_e2e.py` & `thipster-0.15.0/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.5/thipster/auth/google.py` & `thipster-0.15.0/thipster/auth/google.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.5/thipster/engine/engine.py` & `thipster-0.15.0/thipster/engine/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,14 +181,25 @@
         self.__terraform.init()
 
     def _plan_terraform(self) -> str:
         """Plan Terraform
 
         Returns
         -------
-        tuple[str, float]
-            A tuple made up of the results of the Terraform plan and the time it took
-            to run it
+        str
+            The results of the Terraform plan
         """
         results = self.__terraform.plan()
 
         return results
+
+    def _apply_terraform(self) -> str:
+        """Apply Terraform
+
+        Returns
+        -------
+        str
+            The results of the Terraform apply
+        """
+        results = self.__terraform.apply()
+
+        return results
```

### Comparing `thipster-0.14.5/thipster/engine/i_parser.py` & `thipster-0.15.0/thipster/engine/i_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.5/thipster/engine/i_repository.py` & `thipster-0.15.0/thipster/engine/i_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.5/thipster/engine/i_terraform.py` & `thipster-0.15.0/thipster/engine/i_terraform.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.5/thipster/engine/parsed_file.py` & `thipster-0.15.0/thipster/engine/parsed_file.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.5/thipster/engine/resource_model.py` & `thipster-0.15.0/thipster/engine/resource_model.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.5/thipster/helpers.py` & `thipster-0.15.0/thipster/helpers.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.5/thipster/parser/dsl_parser/ast.py` & `thipster-0.15.0/thipster/parser/dsl_parser/ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.5/thipster/parser/dsl_parser/exceptions.py` & `thipster-0.15.0/thipster/parser/dsl_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.5/thipster/parser/dsl_parser/interpreter.py` & `thipster-0.15.0/thipster/parser/dsl_parser/interpreter.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.5/thipster/parser/dsl_parser/lexer.py` & `thipster-0.15.0/thipster/parser/dsl_parser/lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.5/thipster/parser/dsl_parser/lexer_position.py` & `thipster-0.15.0/thipster/parser/dsl_parser/lexer_position.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.5/thipster/parser/dsl_parser/parser.py` & `thipster-0.15.0/thipster/parser/dsl_parser/parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.5/thipster/parser/dsl_parser/token.py` & `thipster-0.15.0/thipster/parser/dsl_parser/token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.5/thipster/parser/dsl_parser/token_parser.py` & `thipster-0.15.0/thipster/parser/dsl_parser/token_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.5/thipster/parser/parser_factory.py` & `thipster-0.15.0/thipster/parser/parser_factory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.5/thipster/parser/yaml_parser.py` & `thipster-0.15.0/thipster/parser/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.5/thipster/repository/github.py` & `thipster-0.15.0/thipster/repository/github.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.5/thipster/repository/json.py` & `thipster-0.15.0/thipster/repository/json.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.5/thipster/terraform/cdk.py` & `thipster-0.15.0/thipster/terraform/cdk.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.5/thipster/terraform/exceptions.py` & `thipster-0.15.0/thipster/terraform/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.5/thipster/thipster.egg-info/SOURCES.txt` & `thipster-0.15.0/thipster.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,56 @@
+LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 requirements.txt
 setup.py
+tests/__init__.py
 tests/test_e2e.py
+tests/engine/__init__.py
+tests/engine/test_engine.py
+tests/parser/__init__.py
+tests/parser/test_ParserFactory.py
+tests/parser/test_YAMLParser.py
+tests/parser/test_parsedfile.py
+tests/parser/dsl_parser/__init__.py
+tests/parser/dsl_parser/test_DSLparser.py
+tests/parser/dsl_parser/test_ast.py
+tests/parser/dsl_parser/test_lexer.py
+tests/parser/dsl_parser/test_token.py
+tests/parser/dsl_parser/test_tokenparser.py
 thipster/__init__.py
 thipster/helpers.py
+thipster.egg-info/PKG-INFO
+thipster.egg-info/SOURCES.txt
+thipster.egg-info/dependency_links.txt
+thipster.egg-info/requires.txt
+thipster.egg-info/top_level.txt
 thipster/auth/__init__.py
-thipster/engine/Engine.py
-thipster/engine/I_Auth.py
-thipster/engine/I_Parser.py
-thipster/engine/I_Repository.py
-thipster/engine/I_Terraform.py
-thipster/engine/ParsedFile.py
-thipster/engine/ResourceModel.py
+thipster/auth/google.py
 thipster/engine/__init__.py
-thipster/parser/ParserFactory.py
-thipster/parser/YAMLParser.py
+thipster/engine/engine.py
+thipster/engine/i_auth.py
+thipster/engine/i_parser.py
+thipster/engine/i_repository.py
+thipster/engine/i_terraform.py
+thipster/engine/parsed_file.py
+thipster/engine/resource_model.py
 thipster/parser/__init__.py
-thipster/parser/dsl_parser/AST.py
-thipster/parser/dsl_parser/DSLExceptions.py
-thipster/parser/dsl_parser/DSLParser.py
-thipster/parser/dsl_parser/Interpreter.py
-thipster/parser/dsl_parser/Lexer.py
-thipster/parser/dsl_parser/LexerPosition.py
-thipster/parser/dsl_parser/Token.py
-thipster/parser/dsl_parser/TokenParser.py
+thipster/parser/parser_factory.py
+thipster/parser/yaml_parser.py
 thipster/parser/dsl_parser/__init__.py
-thipster/repository/GithubRepo.py
-thipster/repository/JSONRepo.py
-thipster/repository/LocalRepo.py
+thipster/parser/dsl_parser/ast.py
+thipster/parser/dsl_parser/exceptions.py
+thipster/parser/dsl_parser/interpreter.py
+thipster/parser/dsl_parser/lexer.py
+thipster/parser/dsl_parser/lexer_position.py
+thipster/parser/dsl_parser/parser.py
+thipster/parser/dsl_parser/token.py
+thipster/parser/dsl_parser/token_parser.py
 thipster/repository/__init__.py
-thipster/terraform/CDK.py
+thipster/repository/github.py
+thipster/repository/json.py
+thipster/repository/local.py
 thipster/terraform/__init__.py
-thipster/thipster.egg-info/PKG-INFO
-thipster/thipster.egg-info/SOURCES.txt
-thipster/thipster.egg-info/dependency_links.txt
-thipster/thipster.egg-info/entry_points.txt
-thipster/thipster.egg-info/requires.txt
-thipster/thipster.egg-info/top_level.txt
+thipster/terraform/cdk.py
+thipster/terraform/exceptions.py
```

### Comparing `thipster-0.14.5/thipster.egg-info/PKG-INFO` & `thipster-0.15.0/thipster.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.14.5
+Version: 0.15.0
 Summary: THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files. It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

