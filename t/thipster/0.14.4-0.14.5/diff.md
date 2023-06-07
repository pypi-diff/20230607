# Comparing `tmp/thipster-0.14.4.tar.gz` & `tmp/thipster-0.14.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thipster-0.14.4.tar", last modified: Wed Jun  7 07:40:06 2023, max compression
+gzip compressed data, was "thipster-0.14.5.tar", last modified: Wed Jun  7 12:44:36 2023, max compression
```

## Comparing `thipster-0.14.4.tar` & `thipster-0.14.5.tar`

### file list

```diff
@@ -1,71 +1,77 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 07:40:06.962073 thipster-0.14.4/
--rw-r--r--   0 root         (0) root         (0)     1051 2023-06-07 07:40:03.000000 thipster-0.14.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       80 2023-06-07 07:40:03.000000 thipster-0.14.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4003 2023-06-07 07:40:06.962073 thipster-0.14.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3390 2023-06-07 07:40:03.000000 thipster-0.14.4/README.md
--rw-r--r--   0 root         (0) root         (0)      905 2023-06-07 07:40:03.000000 thipster-0.14.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      137 2023-06-07 07:40:03.000000 thipster-0.14.4/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-07 07:40:06.962073 thipster-0.14.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1372 2023-06-07 07:40:03.000000 thipster-0.14.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 07:40:06.946073 thipster-0.14.4/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 07:40:03.000000 thipster-0.14.4/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 07:40:06.950073 thipster-0.14.4/tests/engine/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 07:40:03.000000 thipster-0.14.4/tests/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3222 2023-06-07 07:40:03.000000 thipster-0.14.4/tests/engine/test_engine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 07:40:06.950073 thipster-0.14.4/tests/parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 07:40:03.000000 thipster-0.14.4/tests/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 07:40:06.950073 thipster-0.14.4/tests/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 07:40:03.000000 thipster-0.14.4/tests/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15549 2023-06-07 07:40:03.000000 thipster-0.14.4/tests/parser/dsl_parser/test_DSLparser.py
--rw-r--r--   0 root         (0) root         (0)     1358 2023-06-07 07:40:03.000000 thipster-0.14.4/tests/parser/dsl_parser/test_ast.py
--rw-r--r--   0 root         (0) root         (0)    13297 2023-06-07 07:40:03.000000 thipster-0.14.4/tests/parser/dsl_parser/test_lexer.py
--rw-r--r--   0 root         (0) root         (0)      862 2023-06-07 07:40:03.000000 thipster-0.14.4/tests/parser/dsl_parser/test_token.py
--rw-r--r--   0 root         (0) root         (0)     3524 2023-06-07 07:40:03.000000 thipster-0.14.4/tests/parser/dsl_parser/test_tokenparser.py
--rw-r--r--   0 root         (0) root         (0)     3010 2023-06-07 07:40:03.000000 thipster-0.14.4/tests/parser/test_ParserFactory.py
--rw-r--r--   0 root         (0) root         (0)     4956 2023-06-07 07:40:03.000000 thipster-0.14.4/tests/parser/test_YAMLParser.py
--rw-r--r--   0 root         (0) root         (0)     4683 2023-06-07 07:40:03.000000 thipster-0.14.4/tests/parser/test_parsedfile.py
--rw-r--r--   0 root         (0) root         (0)     6934 2023-06-07 07:40:03.000000 thipster-0.14.4/tests/test_e2e.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 07:40:06.950073 thipster-0.14.4/thipster/
--rw-r--r--   0 root         (0) root         (0)      171 2023-06-07 07:40:03.000000 thipster-0.14.4/thipster/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 07:40:06.954073 thipster-0.14.4/thipster/auth/
--rw-r--r--   0 root         (0) root         (0)      215 2023-06-07 07:40:03.000000 thipster-0.14.4/thipster/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)      683 2023-06-07 07:40:03.000000 thipster-0.14.4/thipster/auth/google.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 07:40:06.954073 thipster-0.14.4/thipster/engine/
--rw-r--r--   0 root         (0) root         (0)      369 2023-06-07 07:40:03.000000 thipster-0.14.4/thipster/engine/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4178 2023-06-07 07:40:03.000000 thipster-0.14.4/thipster/engine/engine.py
--rw-r--r--   0 root         (0) root         (0)      464 2023-06-07 07:40:03.000000 thipster-0.14.4/thipster/engine/i_auth.py
--rw-r--r--   0 root         (0) root         (0)      726 2023-06-07 07:40:03.000000 thipster-0.14.4/thipster/engine/i_parser.py
--rw-r--r--   0 root         (0) root         (0)      597 2023-06-07 07:40:03.000000 thipster-0.14.4/thipster/engine/i_repository.py
--rw-r--r--   0 root         (0) root         (0)     1420 2023-06-07 07:40:03.000000 thipster-0.14.4/thipster/engine/i_terraform.py
--rw-r--r--   0 root         (0) root         (0)     6023 2023-06-07 07:40:03.000000 thipster-0.14.4/thipster/engine/parsed_file.py
--rw-r--r--   0 root         (0) root         (0)     4124 2023-06-07 07:40:03.000000 thipster-0.14.4/thipster/engine/resource_model.py
--rw-r--r--   0 root         (0) root         (0)      129 2023-06-07 07:40:03.000000 thipster-0.14.4/thipster/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 07:40:06.958073 thipster-0.14.4/thipster/parser/
--rw-r--r--   0 root         (0) root         (0)      365 2023-06-07 07:40:03.000000 thipster-0.14.4/thipster/parser/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 07:40:06.958073 thipster-0.14.4/thipster/parser/dsl_parser/
--rw-r--r--   0 root         (0) root         (0)       30 2023-06-07 07:40:03.000000 thipster-0.14.4/thipster/parser/dsl_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10326 2023-06-07 07:40:03.000000 thipster-0.14.4/thipster/parser/dsl_parser/ast.py
--rw-r--r--   0 root         (0) root         (0)     1811 2023-06-07 07:40:03.000000 thipster-0.14.4/thipster/parser/dsl_parser/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    13710 2023-06-07 07:40:03.000000 thipster-0.14.4/thipster/parser/dsl_parser/interpreter.py
--rw-r--r--   0 root         (0) root         (0)    17262 2023-06-07 07:40:03.000000 thipster-0.14.4/thipster/parser/dsl_parser/lexer.py
--rw-r--r--   0 root         (0) root         (0)     4771 2023-06-07 07:40:03.000000 thipster-0.14.4/thipster/parser/dsl_parser/lexer_position.py
--rw-r--r--   0 root         (0) root         (0)     1944 2023-06-07 07:40:03.000000 thipster-0.14.4/thipster/parser/dsl_parser/parser.py
--rw-r--r--   0 root         (0) root         (0)     2290 2023-06-07 07:40:03.000000 thipster-0.14.4/thipster/parser/dsl_parser/token.py
--rw-r--r--   0 root         (0) root         (0)    19125 2023-06-07 07:40:03.000000 thipster-0.14.4/thipster/parser/dsl_parser/token_parser.py
--rw-r--r--   0 root         (0) root         (0)     2255 2023-06-07 07:40:03.000000 thipster-0.14.4/thipster/parser/parser_factory.py
--rw-r--r--   0 root         (0) root         (0)     6276 2023-06-07 07:40:03.000000 thipster-0.14.4/thipster/parser/yaml_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 07:40:06.958073 thipster-0.14.4/thipster/repository/
--rw-r--r--   0 root         (0) root         (0)      333 2023-06-07 07:40:03.000000 thipster-0.14.4/thipster/repository/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1139 2023-06-07 07:40:03.000000 thipster-0.14.4/thipster/repository/github.py
--rw-r--r--   0 root         (0) root         (0)     4652 2023-06-07 07:40:03.000000 thipster-0.14.4/thipster/repository/json.py
--rw-r--r--   0 root         (0) root         (0)      347 2023-06-07 07:40:03.000000 thipster-0.14.4/thipster/repository/local.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 07:40:06.962073 thipster-0.14.4/thipster/terraform/
--rw-r--r--   0 root         (0) root         (0)      327 2023-06-07 07:40:03.000000 thipster-0.14.4/thipster/terraform/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15624 2023-06-07 07:40:03.000000 thipster-0.14.4/thipster/terraform/cdk.py
--rw-r--r--   0 root         (0) root         (0)     1119 2023-06-07 07:40:03.000000 thipster-0.14.4/thipster/terraform/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 07:40:06.954073 thipster-0.14.4/thipster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4003 2023-06-07 07:40:06.000000 thipster-0.14.4/thipster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1658 2023-06-07 07:40:06.000000 thipster-0.14.4/thipster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 07:40:06.000000 thipster-0.14.4/thipster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      237 2023-06-07 07:40:06.000000 thipster-0.14.4/thipster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-07 07:40:06.000000 thipster-0.14.4/thipster.egg-info/top_level.txt
+drwxr-xr-x   0 rcattin   (1000) rcattin   (1000)        0 2023-06-07 12:44:36.213512 thipster-0.14.5/
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)     1052 2023-06-07 09:14:11.000000 thipster-0.14.5/LICENSE
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)       81 2023-06-07 09:14:11.000000 thipster-0.14.5/MANIFEST.in
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)     4003 2023-06-07 12:44:36.213512 thipster-0.14.5/PKG-INFO
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)     3390 2023-06-06 10:08:32.000000 thipster-0.14.5/README.md
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)      916 2023-06-07 12:43:52.000000 thipster-0.14.5/pyproject.toml
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)      137 2023-06-07 09:14:11.000000 thipster-0.14.5/requirements.txt
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)       38 2023-06-07 12:44:36.213512 thipster-0.14.5/setup.cfg
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)     1372 2023-06-07 12:43:57.000000 thipster-0.14.5/setup.py
+drwxr-xr-x   0 rcattin   (1000) rcattin   (1000)        0 2023-06-07 12:44:36.173512 thipster-0.14.5/tests/
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)        0 2023-04-26 14:12:09.000000 thipster-0.14.5/tests/__init__.py
+drwxr-xr-x   0 rcattin   (1000) rcattin   (1000)        0 2023-06-07 12:44:36.173512 thipster-0.14.5/tests/engine/
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)        0 2023-04-20 08:57:48.000000 thipster-0.14.5/tests/engine/__init__.py
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)     3222 2023-06-06 14:38:25.000000 thipster-0.14.5/tests/engine/test_engine.py
+drwxr-xr-x   0 rcattin   (1000) rcattin   (1000)        0 2023-06-07 12:44:36.173512 thipster-0.14.5/tests/parser/
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)        0 2023-04-20 08:57:48.000000 thipster-0.14.5/tests/parser/__init__.py
+drwxr-xr-x   0 rcattin   (1000) rcattin   (1000)        0 2023-06-07 12:44:36.173512 thipster-0.14.5/tests/parser/dsl_parser/
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)        0 2023-04-21 13:59:54.000000 thipster-0.14.5/tests/parser/dsl_parser/__init__.py
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)    15548 2023-06-07 09:14:11.000000 thipster-0.14.5/tests/parser/dsl_parser/test_DSLparser.py
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)     1358 2023-06-06 14:38:25.000000 thipster-0.14.5/tests/parser/dsl_parser/test_ast.py
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)    13297 2023-06-06 14:38:25.000000 thipster-0.14.5/tests/parser/dsl_parser/test_lexer.py
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)      862 2023-06-06 14:38:25.000000 thipster-0.14.5/tests/parser/dsl_parser/test_token.py
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)     3524 2023-06-06 14:38:25.000000 thipster-0.14.5/tests/parser/dsl_parser/test_tokenparser.py
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)     3010 2023-06-06 14:38:25.000000 thipster-0.14.5/tests/parser/test_ParserFactory.py
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)     4956 2023-06-06 14:38:25.000000 thipster-0.14.5/tests/parser/test_YAMLParser.py
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)     4683 2023-06-06 14:38:25.000000 thipster-0.14.5/tests/parser/test_parsedfile.py
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)     6934 2023-06-07 12:43:52.000000 thipster-0.14.5/tests/test_e2e.py
+drwxr-xr-x   0 rcattin   (1000) rcattin   (1000)        0 2023-06-07 12:44:36.173512 thipster-0.14.5/thipster/
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)      171 2023-06-06 14:38:25.000000 thipster-0.14.5/thipster/__init__.py
+drwxr-xr-x   0 rcattin   (1000) rcattin   (1000)        0 2023-06-07 12:44:36.183512 thipster-0.14.5/thipster/auth/
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)      215 2023-06-06 14:38:25.000000 thipster-0.14.5/thipster/auth/__init__.py
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)      941 2023-06-07 12:43:57.000000 thipster-0.14.5/thipster/auth/google.py
+drwxr-xr-x   0 rcattin   (1000) rcattin   (1000)        0 2023-06-07 12:44:36.183512 thipster-0.14.5/thipster/engine/
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)      369 2023-06-06 14:38:25.000000 thipster-0.14.5/thipster/engine/__init__.py
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)     4949 2023-06-07 12:43:57.000000 thipster-0.14.5/thipster/engine/engine.py
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)      410 2023-06-07 12:43:57.000000 thipster-0.14.5/thipster/engine/i_auth.py
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)      726 2023-06-06 14:38:25.000000 thipster-0.14.5/thipster/engine/i_parser.py
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)      597 2023-06-06 14:38:25.000000 thipster-0.14.5/thipster/engine/i_repository.py
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)     1815 2023-06-07 12:43:57.000000 thipster-0.14.5/thipster/engine/i_terraform.py
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)     6023 2023-06-06 14:38:25.000000 thipster-0.14.5/thipster/engine/parsed_file.py
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)     4125 2023-06-07 09:00:27.000000 thipster-0.14.5/thipster/engine/resource_model.py
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)      654 2023-06-07 12:43:57.000000 thipster-0.14.5/thipster/helpers.py
+drwxr-xr-x   0 rcattin   (1000) rcattin   (1000)        0 2023-06-07 12:44:36.183512 thipster-0.14.5/thipster/parser/
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)      364 2023-06-07 09:14:11.000000 thipster-0.14.5/thipster/parser/__init__.py
+drwxr-xr-x   0 rcattin   (1000) rcattin   (1000)        0 2023-06-07 12:44:36.183512 thipster-0.14.5/thipster/parser/dsl_parser/
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)       30 2023-06-06 14:38:25.000000 thipster-0.14.5/thipster/parser/dsl_parser/__init__.py
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)    10326 2023-06-07 09:14:11.000000 thipster-0.14.5/thipster/parser/dsl_parser/ast.py
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)     1811 2023-06-06 14:38:25.000000 thipster-0.14.5/thipster/parser/dsl_parser/exceptions.py
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)    13708 2023-06-07 09:14:11.000000 thipster-0.14.5/thipster/parser/dsl_parser/interpreter.py
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)    17264 2023-06-07 12:43:57.000000 thipster-0.14.5/thipster/parser/dsl_parser/lexer.py
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)     4771 2023-06-06 14:38:25.000000 thipster-0.14.5/thipster/parser/dsl_parser/lexer_position.py
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)     1944 2023-06-06 14:38:25.000000 thipster-0.14.5/thipster/parser/dsl_parser/parser.py
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)     2290 2023-06-06 14:38:25.000000 thipster-0.14.5/thipster/parser/dsl_parser/token.py
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)    19125 2023-06-07 09:14:11.000000 thipster-0.14.5/thipster/parser/dsl_parser/token_parser.py
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)     2254 2023-06-07 09:14:11.000000 thipster-0.14.5/thipster/parser/parser_factory.py
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)     6275 2023-06-07 09:14:11.000000 thipster-0.14.5/thipster/parser/yaml_parser.py
+drwxr-xr-x   0 rcattin   (1000) rcattin   (1000)        0 2023-06-07 12:44:36.183512 thipster-0.14.5/thipster/repository/
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)      332 2023-06-07 09:14:11.000000 thipster-0.14.5/thipster/repository/__init__.py
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)     1284 2023-06-07 12:43:57.000000 thipster-0.14.5/thipster/repository/github.py
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)     4652 2023-06-06 14:38:25.000000 thipster-0.14.5/thipster/repository/json.py
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)      347 2023-06-06 14:38:25.000000 thipster-0.14.5/thipster/repository/local.py
+drwxr-xr-x   0 rcattin   (1000) rcattin   (1000)        0 2023-06-07 12:44:36.183512 thipster-0.14.5/thipster/terraform/
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)      327 2023-06-06 14:38:25.000000 thipster-0.14.5/thipster/terraform/__init__.py
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)    19903 2023-06-07 12:43:57.000000 thipster-0.14.5/thipster/terraform/cdk.py
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)     1119 2023-06-06 14:38:25.000000 thipster-0.14.5/thipster/terraform/exceptions.py
+drwxr-xr-x   0 rcattin   (1000) rcattin   (1000)        0 2023-06-07 12:44:36.203512 thipster-0.14.5/thipster/thipster.egg-info/
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)     1265 2023-05-30 13:56:10.000000 thipster-0.14.5/thipster/thipster.egg-info/SOURCES.txt
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)        1 2023-05-30 13:56:10.000000 thipster-0.14.5/thipster/thipster.egg-info/dependency_links.txt
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)       44 2023-05-30 13:56:10.000000 thipster-0.14.5/thipster/thipster.egg-info/entry_points.txt
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)      205 2023-05-30 13:56:10.000000 thipster-0.14.5/thipster/thipster.egg-info/requires.txt
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)       57 2023-05-30 13:56:10.000000 thipster-0.14.5/thipster/thipster.egg-info/top_level.txt
+drwxr-xr-x   0 rcattin   (1000) rcattin   (1000)        0 2023-06-07 12:44:36.183512 thipster-0.14.5/thipster.egg-info/
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)     4003 2023-06-07 12:44:36.000000 thipster-0.14.5/thipster.egg-info/PKG-INFO
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)     1870 2023-06-07 12:44:36.000000 thipster-0.14.5/thipster.egg-info/SOURCES.txt
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)        1 2023-06-07 12:44:36.000000 thipster-0.14.5/thipster.egg-info/dependency_links.txt
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)      237 2023-06-07 12:44:36.000000 thipster-0.14.5/thipster.egg-info/requires.txt
+-rw-r--r--   0 rcattin   (1000) rcattin   (1000)       15 2023-06-07 12:44:36.000000 thipster-0.14.5/thipster.egg-info/top_level.txt
```

### Comparing `thipster-0.14.4/LICENSE` & `thipster-0.14.5/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
 EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
 MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
 NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
 LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
 OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
-WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `thipster-0.14.4/PKG-INFO` & `thipster-0.14.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.14.4
+Version: 0.14.5
 Summary: THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files. It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `thipster-0.14.4/README.md` & `thipster-0.14.5/README.md`

 * *Files identical despite different names*

### Comparing `thipster-0.14.4/pyproject.toml` & `thipster-0.14.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 major_emoji = ":boom:"
 minor_emoji = ":sparkles:"
 patch_emoji = ":ambulance:,:bug:,:adhesive_bandage:,:lock:,:arrow_up:,:arrow_down:,:heavy_plus_sign:,:heavy_minus_sign:,:rotating_light:,:zap:,:recycle:,:wrench:,:loud_sound:,:mute:,:goal_net:,:wastebasket:,:coffin:,:chart_with_upwards_trend:,:globe_with_meridians:,:alien:,:wheelchair:,:children_crossing:,:bricks:"
 
 repository_url = "https://upload.pypi.org/legacy/"
 
-commit_subject = ":bookmark: {version}"
+commit_subject = ":bookmark: {version} [skip ci]"
 major_on_zero = false
 
 [pytest]
 mock_use_standalone_module = true
 
 [tool.ruff]
-exclude = ["__init__.py"]
+exclude = ["__init__.py"]
```

### Comparing `thipster-0.14.4/setup.py` & `thipster-0.14.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 from setuptools import setup, find_packages
 
-__version__ = '0.14.4'
+__version__ = '0.14.5'
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
-with open("README.md") as rm:
+with open('README.md') as rm:
     readme = rm.read()
 
 setup(
-    name="thipster",
+    name='thipster',
     authors=[
-        {"name": "rcattin", "email": "rafa.cattin+thipster@gmail.com"},
-        {"name": "gsuquet", "email": "gsuquet@ippon.fr"},
+        {'name': 'rcattin', 'email': 'rafa.cattin+thipster@gmail.com'},
+        {'name': 'gsuquet', 'email': 'gsuquet@ippon.fr'},
     ],
-    description="THipster is a tool dedicated to simplifying the difficulty associated \
+    description='THipster is a tool dedicated to simplifying the difficulty associated \
 with writing Terraform files. It allows users to write infrastructure as code in a \
-simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.",
+simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.',
     long_description=readme,
-    long_description_content_type="text/markdown",
+    long_description_content_type='text/markdown',
     classifiers=[
-        "Development Status :: 1 - Planning",
-        "Programming Language :: Python",
+        'Development Status :: 1 - Planning',
+        'Programming Language :: Python',
     ],
 
-    download_url="https://github.com/THipster/THipster.git",
-    url="https://github.com/THipster/THipster",
+    download_url='https://github.com/THipster/THipster.git',
+    url='https://github.com/THipster/THipster',
 
     version=__version__,
     install_requires=required,
     packages=find_packages(
         exclude=['pipelines'],
     ),
     extras_require={
```

### Comparing `thipster-0.14.4/tests/engine/test_engine.py` & `thipster-0.14.5/tests/engine/test_engine.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.4/tests/parser/dsl_parser/test_DSLparser.py` & `thipster-0.14.5/tests/parser/dsl_parser/test_DSLparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,15 @@
         assert region.name == 'region'
         assert region.value == 'euw'
 
 
 def test_parse_list():
     out = __test_file(
         file="""bucket my-bucket:
-\tregion: 
+\tregion:
 \t\t- toto
 \t\t- titi
 \t\t- tata
 """,
     )
 
     assert len(out.resources) == 1
```

### Comparing `thipster-0.14.4/tests/parser/dsl_parser/test_ast.py` & `thipster-0.14.5/tests/parser/dsl_parser/test_ast.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.4/tests/parser/dsl_parser/test_lexer.py` & `thipster-0.14.5/tests/parser/dsl_parser/test_lexer.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.4/tests/parser/dsl_parser/test_token.py` & `thipster-0.14.5/tests/parser/dsl_parser/test_token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.4/tests/parser/dsl_parser/test_tokenparser.py` & `thipster-0.14.5/tests/parser/dsl_parser/test_tokenparser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.4/tests/parser/test_ParserFactory.py` & `thipster-0.14.5/tests/parser/test_ParserFactory.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.4/tests/parser/test_YAMLParser.py` & `thipster-0.14.5/tests/parser/test_YAMLParser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.4/tests/parser/test_parsedfile.py` & `thipster-0.14.5/tests/parser/test_parsedfile.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.4/tests/test_e2e.py` & `thipster-0.14.5/tests/test_e2e.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 LOCAL_REPO = 'tests/resources/e2e/models'
 REMOTE_REPO = 'THipster/models'
 
 
 class MockAuth(I_Auth):
     def authenticate(app):
         GoogleProvider(
-            app, "default_google",
-            project="project_id",
-            credentials="credentials.token",
+            app, 'default_google',
+            project='project_id',
+            credentials='credentials.token',
         )
 
 
 def create_dir(dirname: str, files: dict[str, str]):
     if not os.path.isdir(dirname):
         os.mkdir(dirname)
 
@@ -79,57 +79,57 @@
         if os.path.exists('cdktf.out'):
             shutil.rmtree('cdktf.out')
 
     return output
 
 
 def get_output():
-    with open("thipster.tf.json") as f:
+    with open('thipster.tf.json') as f:
         file_contents = json.load(f)
         f.close()
     return file_contents
 
 
 def get_resource(resource_data: tuple):
     output = get_output()
 
-    resources_of_type = output.get("resource").get(resource_data[0])
+    resources_of_type = output.get('resource').get(resource_data[0])
     resource = None
     for r in resources_of_type.values():
-        if r.get("name") == resource_data[1]:
+        if r.get('name') == resource_data[1]:
             resource = r
 
     assert resource is not None
 
     return resource
 
 
 def assert_resource_created(
     resource_type: str,
     resource_name: str,
 ):
     output = get_output()
-    assert output.get("resource") is not None
-    resources = output.get("resource")
+    assert output.get('resource') is not None
+    resources = output.get('resource')
 
     assert resources.get(resource_type) is not None
 
-    names = [x.get("name") for _, x in resources.get(resource_type).items()]
+    names = [x.get('name') for _, x in resources.get(resource_type).items()]
     assert resource_name in names
 
     return (resource_type, resource_name)
 
 
 def assert_number_of_resource_type_is(
     resource_type: str,
     amount: str,
 ):
     output = get_output()
-    assert output.get("resource") is not None
-    resources = output.get("resource")
+    assert output.get('resource') is not None
+    resources = output.get('resource')
 
     assert resources.get(resource_type) is not None
     assert len(resources.get(resource_type)) == amount
 
 
 def assert_resource_parameters_are(resource_data: tuple, parameters: list[str]):
     resource = get_resource(resource_data)
@@ -149,42 +149,42 @@
     __test_file(
         file="""
 bucket my-bucket:
 \tregion : euw
     """,
     )
 
-    assert_number_of_resource_type_is("google_storage_bucket", 1)
-    bucket = assert_resource_created("google_storage_bucket", "my-bucket")
-    assert_resource_parameters_are(bucket, ["location"])
+    assert_number_of_resource_type_is('google_storage_bucket', 1)
+    bucket = assert_resource_created('google_storage_bucket', 'my-bucket')
+    assert_resource_parameters_are(bucket, ['location'])
 
 
 def test_empty_bucket():
     __test_file(
         file="""
 bucket dzvhvzarbazkhr:
 
     """,
     )
 
-    assert_number_of_resource_type_is("google_storage_bucket", 1)
-    assert_resource_created("google_storage_bucket", "dzvhvzarbazkhr")
+    assert_number_of_resource_type_is('google_storage_bucket', 1)
+    assert_resource_created('google_storage_bucket', 'dzvhvzarbazkhr')
 
     __test_file(
         file="""
 bucket dzvhvzarbazkhr:
 
 bucket ezezeaz:
     region: europe
     """,
     )
 
-    assert_number_of_resource_type_is("google_storage_bucket", 2)
-    assert_resource_created("google_storage_bucket", "dzvhvzarbazkhr")
-    assert_resource_created("google_storage_bucket", "ezezeaz")
+    assert_number_of_resource_type_is('google_storage_bucket', 2)
+    assert_resource_created('google_storage_bucket', 'dzvhvzarbazkhr')
+    assert_resource_created('google_storage_bucket', 'ezezeaz')
 
 
 def test_dep_with_no_options():
     with pytest.raises(CDKMissingAttributeInDependency):
         __test_file(
             file="""
 bucket_bad_dep_parent my-bucket:
@@ -214,19 +214,19 @@
 \tip_range: 10.0.1.0/24
 
 loadbalancer my-lb:
 \tload_balancing_scheme: EXTERNAL
     """,
     )
 
-    assert_number_of_resource_type_is("google_compute_network", 3)
-    assert_resource_created("google_compute_network", "lb-net")
+    assert_number_of_resource_type_is('google_compute_network', 3)
+    assert_resource_created('google_compute_network', 'lb-net')
 
-    assert_number_of_resource_type_is("google_compute_subnetwork", 1)
-    assert_resource_created("google_compute_subnetwork", "lb-subnet")
+    assert_number_of_resource_type_is('google_compute_subnetwork', 1)
+    assert_resource_created('google_compute_subnetwork', 'lb-subnet')
 
 
 def test_internal_object():
     __test_file(
         file="""
 firewall testParent:
 \tdirection: EGRESS
@@ -280,16 +280,16 @@
             - "*"
         responseHeader:
             - "*"
         maxAge: 400
         """,
     )
 
-    assert_number_of_resource_type_is("google_storage_bucket", 1)
-    assert_resource_created("google_storage_bucket", "corsBucket")
+    assert_number_of_resource_type_is('google_storage_bucket', 1)
+    assert_resource_created('google_storage_bucket', 'corsBucket')
 
 
 def test_bucket_two_cors():
     __test_file(
         file="""
 bucket:
   name: corsBucket
@@ -308,12 +308,12 @@
       responseHeader:
       - "*"
       maxAge: 600
 """,
         file_type='yaml',
     )
 
-    assert_number_of_resource_type_is("google_storage_bucket", 1)
-    bucket = assert_resource_created("google_storage_bucket", "corsBucket")
-    cors_block = get_resource_parameter(bucket, "cors")
+    assert_number_of_resource_type_is('google_storage_bucket', 1)
+    bucket = assert_resource_created('google_storage_bucket', 'corsBucket')
+    cors_block = get_resource_parameter(bucket, 'cors')
 
     assert len(cors_block) == 2
```

### Comparing `thipster-0.14.4/thipster/engine/engine.py` & `thipster-0.14.5/thipster/engine/engine.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """_Engine.py module.
 """
-import time
 
 import thipster.engine.parsed_file as pf
 
 from .i_auth import I_Auth
 from .i_parser import I_Parser
 from .i_repository import I_Repository
 from .i_terraform import I_Terraform
@@ -14,16 +13,14 @@
 class Engine():
     """The engine of thipster
 
     The core of the application, it is used to call and link all
     interfaces together.
     """
 
-    importedPackages = []
-
     def __init__(
             self, parser: I_Parser,
             repository: I_Repository,
             auth: I_Auth,
             terraform:  I_Terraform,
     ):
         """
@@ -99,65 +96,99 @@
         ----------
         path : str
             The path of the files to be processed
 
         Returns
         -------
         tuple[list[str], str]
-            A tuple made up of the list of directories containing the Terraform json 
+            A tuple made up of the list of directories containing the Terraform json
             files and a string with the results of the Terraform plan
         """
         # Parse file or directory
-        file = self._parse_files(path)[0]
+        parsed_file = self._parse_files(path)
 
         # Get needed models
-        models = self._get_models(file)[0]
+        models = self._get_models(parsed_file)
 
         # Generate Terraform files
-        dirs = self.__terraform.generate(file, models, self.__auth)
+        dirs = self._generate_tf_files(parsed_file, models)
 
         self.__terraform.init()
 
         return dirs, self.__terraform.plan()
 
-    def _parse_files(self, path: str) -> tuple[pf.ParsedFile, float]:
+    def _parse_files(self, path: str) -> pf.ParsedFile:
         """Parse the input file or directory
 
         Parameters
         ----------
         path : str
             The path of the files to be processed
 
         Returns
         -------
-        tuple[pf.ParsedFile, float]
-            A tuple made up of the ParsedFile object and the time it took to parse it
+        pf.ParsedFile
+            The ParsedFile object containing the resources defined in the input file
         """
-        start = time.time()
-
-        file = self.__parser.run(path)
-        assert type(file) == pf.ParsedFile
+        parsed_file = self.__parser.run(path)
+        assert type(parsed_file) == pf.ParsedFile
 
-        end = time.time()
-        return file, end - start
+        return parsed_file
 
     def _get_models(
         self, file: pf.ParsedFile,
-    ) -> tuple[dict[str, ResourceModel], float]:
+    ) -> dict[str, ResourceModel]:
         """Get the models from the repository
 
         Parameters
         ----------
         file : pf.ParsedFile
             The ParsedFile object containing the resources defined in the input file
 
         Returns
         -------
-        tuple[dict[str, ResourceModel], float]
-            A tuple made up of the dictionary of models and the time it took to get them
+        dict[str, ResourceModel]
+            The dictionary of models
         """
-        start = time.time()
         types = [r.type for r in file.resources]
         models = self.__repository.get(types)
-        end = time.time()
 
-        return models, end - start
+        return models
+
+    def _generate_tf_files(
+        self, file: pf.ParsedFile, models: dict[str, ResourceModel],
+    ) -> list[str]:
+        """Generate Terraform files
+
+        Parameters
+        ----------
+        file : pf.ParsedFile
+            The ParsedFile object containing the resources defined in the input file
+        models : dict[str, ResourceModel]
+            The dictionary of models
+
+        Returns
+        -------
+        list[str]
+            A list of directories containing the Terraform json files
+        """
+        dirs = self.__terraform.generate(file, models, self.__auth)
+
+        return dirs
+
+    def _init_terraform(self) -> None:
+        """Initialize Terraform
+        """
+        self.__terraform.init()
+
+    def _plan_terraform(self) -> str:
+        """Plan Terraform
+
+        Returns
+        -------
+        tuple[str, float]
+            A tuple made up of the results of the Terraform plan and the time it took
+            to run it
+        """
+        results = self.__terraform.plan()
+
+        return results
```

### Comparing `thipster-0.14.4/thipster/engine/i_parser.py` & `thipster-0.14.5/thipster/engine/i_parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.4/thipster/engine/i_repository.py` & `thipster-0.14.5/thipster/engine/i_repository.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.4/thipster/engine/i_terraform.py` & `thipster-0.14.5/thipster/engine/i_terraform.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,29 +4,41 @@
 import thipster.engine.resource_model as rm
 
 
 class I_Terraform(ABC):
     """Terraform module interface
     """
     @abstractmethod
-    def apply(self):
+    def apply(self, plan_file_path: str | None = None):
         """Apply generated terraform code
 
+        Parameters
+        ----------
+        plan_file_path : str, optional
+            Path to plan file, by default None
+
         Raises
         ------
         NotImplementedError
             If method is not implemented in inheriting classes
 
         """
         raise NotImplementedError('Should implement apply()')
 
     @abstractmethod
     def generate(self, file: pf.ParsedFile, models: dict[str, rm.ResourceModel]):
         """Generates Terraform code from parsed file and models
 
+        Parameters
+        ----------
+        file : pf.ParsedFile
+            The ParsedFile object containing the resources defined in the input file
+        models : dict[str, rm.ResourceModel]
+            The dictionary of models
+
         Raises
         ------
         NotImplementedError
             If method is not implemented in inheriting classes
 
         """
         raise NotImplementedError('Should implement generate()')
```

### Comparing `thipster-0.14.4/thipster/engine/parsed_file.py` & `thipster-0.14.5/thipster/engine/parsed_file.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.4/thipster/engine/resource_model.py` & `thipster-0.14.5/thipster/engine/resource_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
         return self.__attributes
 
     @property
     def dependencies(self):
         return self.__dependencies
 
     @property
-    def internalObjects(self):
+    def internal_objects(self):
         return self.__internal_objects
 
     @property
     def name_key(self):
         return self.__name_key
 
     @property
```

### Comparing `thipster-0.14.4/thipster/parser/dsl_parser/ast.py` & `thipster-0.14.5/thipster/parser/dsl_parser/ast.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 class StringNode(Node):
     def __init__(self, value: Token) -> None:
         super().__init__()
         self.__value = value
 
     def __str__(self) -> str:
-        return f"<STRING {self.__value}>"
+        return f'<STRING {self.__value}>'
 
     @property
     def value(self) -> Token:
         return self.__value
 
     def accept(self, visitor):
         return visitor.visitString(self)
```

### Comparing `thipster-0.14.4/thipster/parser/dsl_parser/exceptions.py` & `thipster-0.14.5/thipster/parser/dsl_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.4/thipster/parser/dsl_parser/interpreter.py` & `thipster-0.14.5/thipster/parser/dsl_parser/interpreter.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,15 +214,15 @@
             The visited node
 
         Returns
         -------
         str
             The string value of the node
         """
-        ret = ""
+        ret = ''
         for value in element.values:
             ret += str(value.accept(self))
 
         return pf.ParsedLiteral(ret)
 
     def visitVariableDefinition(self, element: ast.VariableDefinitionNode) -> str:
         """Visitor for a VariableDefinitionNode
@@ -372,15 +372,15 @@
         ----------
         element: AmountNode
             The visited node
 
         Returns
         -------
         list[object]
-            A list with the required number of object (resource, list item, ...) 
+            A list with the required number of object (resource, list item, ...)
         """
         var = element.variable.accept(self) if element.variable else None
         res = []
         amount = element.amount.accept(self).value
         if not isinstance(amount, int):
             raise DSLSyntaxException(amount.value.position)
 
@@ -417,15 +417,15 @@
         ----------
         element: DictNode
             The visited node
 
         Returns
         -------
         ParsedDict
-            A ParsedDict object based on the node attributes 
+            A ParsedDict object based on the node attributes
         """
         return pf.ParsedDict([v.accept(self) for v in element.value])
 
     def visitLiteral(self, element: ast.LiteralNode) -> pf.ParsedLiteral:
         """Visitor for an LiteralNode
 
         Parameters
```

### Comparing `thipster-0.14.4/thipster/parser/dsl_parser/lexer.py` & `thipster-0.14.5/thipster/parser/dsl_parser/lexer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from thipster.engine.parsed_file import Position
-from thipster.helpers import createLogger
+from thipster.helpers import create_logger
 
 from .exceptions import DSLParserNoEndingQuotes
 from .lexer_position import LexerPosition
 from .token import TOKENTYPES as TT
 from .token import Token
 
 
@@ -14,15 +14,15 @@
     def __init__(self, files: dict[str, str]):
         """
         Parameters
         ----------
         files : dict[str, str]
             Dictionnary of files to tokenize, fileName : fileContent
         """
-        self.__logger = createLogger(__name__)
+        self.__logger = create_logger(__name__)
         self.__files = files
         self.__tokenList = []
         self.__lexerPosition = LexerPosition()
         self.__currentChar = ''
 
     @property
     def files(self):
```

### Comparing `thipster-0.14.4/thipster/parser/dsl_parser/lexer_position.py` & `thipster-0.14.5/thipster/parser/dsl_parser/lexer_position.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.4/thipster/parser/dsl_parser/parser.py` & `thipster-0.14.5/thipster/parser/dsl_parser/parser.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.4/thipster/parser/dsl_parser/token.py` & `thipster-0.14.5/thipster/parser/dsl_parser/token.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.4/thipster/parser/dsl_parser/token_parser.py` & `thipster-0.14.5/thipster/parser/dsl_parser/token_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -578,22 +578,22 @@
                 case TT.VAR:
                     values.append(ast.VariableNode(self.__next(TT.VAR)))
 
                 case TT.INT:
                     values.append(ast.IntNode(self.__next(TT.INT)))
 
                 case TT.DIV:
-                    token = Token(self.__next(TT.DIV).position, TT.STRING, "/")
+                    token = Token(self.__next(TT.DIV).position, TT.STRING, '/')
                     values.append(ast.StringNode(token))
 
                 case TT.MINUS:
                     token = Token(
                         self.__next(
                             TT.MINUS,
-                        ).position, TT.STRING, "-",
+                        ).position, TT.STRING, '-',
                     )
                     values.append(ast.StringNode(token))
             nextType = self.__get_next_type()
 
         return ast.StringExprNode(values)
 
     def __get_type(self):
@@ -603,20 +603,20 @@
         nextType = self.__get_next_type()
         while nextType in [TT.STRING, TT.MINUS, TT.DIV]:
             match nextType:
                 case TT.STRING:
                     values.append(ast.StringNode(self.__next(TT.STRING)))
 
                 case TT.DIV:
-                    token = Token(self.__next(TT.DIV).position, TT.STRING, "/")
+                    token = Token(self.__next(TT.DIV).position, TT.STRING, '/')
                     values.append(ast.StringNode(token))
 
                 case TT.MINUS:
                     token = Token(
                         self.__next(
                             TT.MINUS,
-                        ).position, TT.STRING, "-",
+                        ).position, TT.STRING, '-',
                     )
                     values.append(ast.StringNode(token))
             nextType = self.__get_next_type()
 
         return ast.StringExprNode(values)
```

### Comparing `thipster-0.14.4/thipster/parser/parser_factory.py` & `thipster-0.14.5/thipster/parser/parser_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         ----------
         path: str
             Path to run this function into
 
         Returns
         -------
         list[str]
-            A list of all the filenames 
+            A list of all the filenames
         """
 
         path = os.path.abspath(path)
 
         if not os.path.exists(path):
             raise ParserPathNotFound(path)
```

### Comparing `thipster-0.14.4/thipster/parser/yaml_parser.py` & `thipster-0.14.5/thipster/parser/yaml_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         ----------
         path: str
             Path to run this function into
 
         Returns
         -------
         list[str]
-            A list of all the filenames 
+            A list of all the filenames
         """
         path = os.path.abspath(path)
 
         if not os.path.exists(path):
             raise YAMLParserPathNotFound(path)
 
         files = []
```

### Comparing `thipster-0.14.4/thipster/repository/github.py` & `thipster-0.14.5/thipster/repository/github.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,23 +10,26 @@
     """Class representing a GitHub resources Repository
 
     JSON Models of resources and services offered by supported cloud providers are
     stored in a repository.
     This class is used to access those models if they are located in a GitHub repo.
     """
 
-    def __init__(self, repo: str) -> None:
+    def __init__(self, repo: str, branch: str = 'main') -> None:
         """
         Parameters
         ----------
         repo : str
             Name of the repository, for example : 'THipster/models'
+        branch : str, optional
+            Name of the branch, by default 'main'
         """
         super().__init__()
         self.__repo = repo
+        self.__branch = branch
 
     def get_json(self, name: str) -> str | bytes | bytearray:
         """Method to get the json file from the GitHub repository
 
         Parameters
         ----------
         name : str
@@ -34,11 +37,11 @@
 
         Returns
         -------
         str | bytes | bytearray
             Content of the JSON file defining the desired resource
         """
         response = requests.get(
-            f'https://raw.githubusercontent.com/{self.__repo}/main/{name}.json',
+            f'https://raw.githubusercontent.com/{self.__repo}/{self.__branch}/{name}.json',
         )
 
         return response.content
```

### Comparing `thipster-0.14.4/thipster/repository/json.py` & `thipster-0.14.5/thipster/repository/json.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.4/thipster/terraform/exceptions.py` & `thipster-0.14.5/thipster/terraform/exceptions.py`

 * *Files identical despite different names*

### Comparing `thipster-0.14.4/thipster.egg-info/PKG-INFO` & `thipster-0.14.5/thipster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thipster
-Version: 0.14.4
+Version: 0.14.5
 Summary: THipster is a tool dedicated to simplifying the difficulty associated with writing Terraform files. It allows users to write infrastructure as code in a simplified format, using either YAML (with JINJA) or the dedicated Thipster DSL.
 Home-page: https://github.com/THipster/THipster
 Download-URL: https://github.com/THipster/THipster.git
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `thipster-0.14.4/thipster.egg-info/SOURCES.txt` & `thipster-0.14.5/thipster.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -49,8 +49,13 @@
 thipster/parser/dsl_parser/token_parser.py
 thipster/repository/__init__.py
 thipster/repository/github.py
 thipster/repository/json.py
 thipster/repository/local.py
 thipster/terraform/__init__.py
 thipster/terraform/cdk.py
-thipster/terraform/exceptions.py
+thipster/terraform/exceptions.py
+thipster/thipster.egg-info/SOURCES.txt
+thipster/thipster.egg-info/dependency_links.txt
+thipster/thipster.egg-info/entry_points.txt
+thipster/thipster.egg-info/requires.txt
+thipster/thipster.egg-info/top_level.txt
```

