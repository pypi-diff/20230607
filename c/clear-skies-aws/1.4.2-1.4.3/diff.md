# Comparing `tmp/clear-skies-aws-1.4.2.tar.gz` & `tmp/clear_skies_aws-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clear-skies-aws-1.4.2.tar", last modified: Tue May 23 15:30:55 2023, max compression
+gzip compressed data, was "clear_skies_aws-1.4.3.tar", max compression
```

## Comparing `clear-skies-aws-1.4.2.tar` & `clear_skies_aws-1.4.3.tar`

### file list

```diff
@@ -1,59 +1,58 @@
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-23 15:30:55.552644 clear-skies-aws-1.4.2/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1053 2022-01-16 00:26:29.000000 clear-skies-aws-1.4.2/LICENSE
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       25 2022-01-16 00:26:29.000000 clear-skies-aws-1.4.2/MANIFEST.in
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     8371 2023-05-23 15:30:55.552644 clear-skies-aws-1.4.2/PKG-INFO
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     7780 2023-03-26 15:10:17.000000 clear-skies-aws-1.4.2/README.md
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       79 2023-05-23 15:30:55.552644 clear-skies-aws-1.4.2/setup.cfg
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1375 2023-05-23 15:30:35.000000 clear-skies-aws-1.4.2/setup.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-23 15:30:55.540645 clear-skies-aws-1.4.2/src/
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-23 15:30:55.540645 clear-skies-aws-1.4.2/src/clear_skies_aws.egg-info/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     8371 2023-05-23 15:30:55.000000 clear-skies-aws-1.4.2/src/clear_skies_aws.egg-info/PKG-INFO
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1979 2023-05-23 15:30:55.000000 clear-skies-aws-1.4.2/src/clear_skies_aws.egg-info/SOURCES.txt
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        1 2023-05-23 15:30:55.000000 clear-skies-aws-1.4.2/src/clear_skies_aws.egg-info/dependency_links.txt
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       36 2023-05-23 15:30:55.000000 clear-skies-aws-1.4.2/src/clear_skies_aws.egg-info/requires.txt
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       15 2023-05-23 15:30:55.000000 clear-skies-aws-1.4.2/src/clear_skies_aws.egg-info/top_level.txt
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-23 15:30:55.540645 clear-skies-aws-1.4.2/src/clearskies_aws/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       58 2023-05-23 15:29:15.000000 clear-skies-aws-1.4.2/src/clearskies_aws/__init__.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-23 15:30:55.540645 clear-skies-aws-1.4.2/src/clearskies_aws/actions/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      885 2023-05-14 19:32:03.000000 clear-skies-aws-1.4.2/src/clearskies_aws/actions/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2023-05-14 11:10:30.000000 clear-skies-aws-1.4.2/src/clearskies_aws/actions/assume_role.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     6738 2023-05-23 13:51:24.000000 clear-skies-aws-1.4.2/src/clearskies_aws/actions/ses.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)        0 2023-05-14 11:10:26.000000 clear-skies-aws-1.4.2/src/clearskies_aws/actions/sns.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2921 2023-05-15 10:23:42.000000 clear-skies-aws-1.4.2/src/clearskies_aws/actions/sqs.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-23 15:30:55.544644 clear-skies-aws-1.4.2/src/clearskies_aws/backends/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       83 2023-03-26 15:10:17.000000 clear-skies-aws-1.4.2/src/clearskies_aws/backends/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)    29126 2023-05-17 10:18:33.000000 clear-skies-aws-1.4.2/src/clearskies_aws/backends/dynamo_db_backend.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2726 2023-03-26 15:10:17.000000 clear-skies-aws-1.4.2/src/clearskies_aws/backends/sqs_backend.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-23 15:30:55.544644 clear-skies-aws-1.4.2/src/clearskies_aws/contexts/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      290 2023-03-26 15:10:17.000000 clear-skies-aws-1.4.2/src/clearskies_aws/contexts/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      506 2023-03-26 15:10:17.000000 clear-skies-aws-1.4.2/src/clearskies_aws/contexts/cli.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1002 2023-03-26 13:26:58.000000 clear-skies-aws-1.4.2/src/clearskies_aws/contexts/lambda_api_gateway.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      952 2023-03-26 13:26:58.000000 clear-skies-aws-1.4.2/src/clearskies_aws/contexts/lambda_elb.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1009 2023-03-26 13:26:58.000000 clear-skies-aws-1.4.2/src/clearskies_aws/contexts/lambda_http_gateway.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1183 2023-03-26 13:26:58.000000 clear-skies-aws-1.4.2/src/clearskies_aws/contexts/lambda_invocation.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1678 2023-04-04 23:13:02.000000 clear-skies-aws-1.4.2/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-23 15:30:55.544644 clear-skies-aws-1.4.2/src/clearskies_aws/di/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       56 2023-03-26 13:26:58.000000 clear-skies-aws-1.4.2/src/clearskies_aws/di/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      775 2023-03-26 15:10:17.000000 clear-skies-aws-1.4.2/src/clearskies_aws/di/standard_dependencies.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-23 15:30:55.548644 clear-skies-aws-1.4.2/src/clearskies_aws/input_outputs/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      233 2023-03-26 15:10:17.000000 clear-skies-aws-1.4.2/src/clearskies_aws/input_outputs/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2932 2023-03-26 13:26:58.000000 clear-skies-aws-1.4.2/src/clearskies_aws/input_outputs/lambda_api_gateway.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      662 2023-03-26 13:26:58.000000 clear-skies-aws-1.4.2/src/clearskies_aws/input_outputs/lambda_elb.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      692 2023-03-26 13:26:58.000000 clear-skies-aws-1.4.2/src/clearskies_aws/input_outputs/lambda_http_gateway.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      715 2023-03-26 13:26:58.000000 clear-skies-aws-1.4.2/src/clearskies_aws/input_outputs/lambda_invocation.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2047 2023-03-26 15:10:17.000000 clear-skies-aws-1.4.2/src/clearskies_aws/input_outputs/lambda_sqs_standard.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-23 15:30:55.548644 clear-skies-aws-1.4.2/src/clearskies_aws/mocks/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       22 2023-05-23 15:29:05.000000 clear-skies-aws-1.4.2/src/clearskies_aws/mocks/__init__.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-23 15:30:55.548644 clear-skies-aws-1.4.2/src/clearskies_aws/mocks/actions/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)       21 2023-05-23 15:29:05.000000 clear-skies-aws-1.4.2/src/clearskies_aws/mocks/actions/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      911 2023-05-23 15:29:05.000000 clear-skies-aws-1.4.2/src/clearskies_aws/mocks/actions/ses.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-23 15:30:55.548644 clear-skies-aws-1.4.2/src/clearskies_aws/secrets/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)      121 2023-03-26 13:26:58.000000 clear-skies-aws-1.4.2/src/clearskies_aws/secrets/__init__.py
-drwxrwxr-x   0 cmancone  (1000) cmancone  (1000)        0 2023-05-23 15:30:55.552644 clear-skies-aws-1.4.2/src/clearskies_aws/secrets/additional_configs/
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1919 2023-05-19 13:30:13.000000 clear-skies-aws-1.4.2/src/clearskies_aws/secrets/additional_configs/__init__.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1082 2023-03-26 13:26:58.000000 clear-skies-aws-1.4.2/src/clearskies_aws/secrets/additional_configs/iam_db_auth.py
--rw-r--r--   0 cmancone  (1000) cmancone  (1000)     3467 2023-05-19 13:34:03.000000 clear-skies-aws-1.4.2/src/clearskies_aws/secrets/additional_configs/iam_db_auth_with_ssm.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     3776 2023-03-26 13:26:58.000000 clear-skies-aws-1.4.2/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssh_cert_bastion.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     6444 2023-03-26 13:26:58.000000 clear-skies-aws-1.4.2/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssm_bastion.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     1655 2023-04-14 14:57:45.000000 clear-skies-aws-1.4.2/src/clearskies_aws/secrets/parameter_store.py
--rw-rw-r--   0 cmancone  (1000) cmancone  (1000)     2898 2023-04-14 14:57:45.000000 clear-skies-aws-1.4.2/src/clearskies_aws/secrets/secrets_manager.py
+-rw-r--r--   0        0        0     1053 2022-01-16 00:26:29.571128 clear_skies_aws-1.4.3/LICENSE
+-rw-r--r--   0        0        0     7780 2023-03-26 15:10:17.430380 clear_skies_aws-1.4.3/README.md
+-rw-r--r--   0        0        0      740 2023-06-07 12:06:57.283230 clear_skies_aws-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0       58 2023-05-23 15:29:15.831933 clear_skies_aws-1.4.3/src/clearskies_aws/__init__.py
+-rw-r--r--   0        0        0     2141 2023-06-07 12:04:20.019789 clear_skies_aws-1.4.3/src/clearskies_aws/actions/__init__.py
+-rw-r--r--   0        0        0     3356 2023-06-07 12:04:20.019789 clear_skies_aws-1.4.3/src/clearskies_aws/actions/action_aws.py
+-rw-r--r--   0        0        0     4085 2023-06-07 00:11:48.817084 clear_skies_aws-1.4.3/src/clearskies_aws/actions/assume_role.py
+-rw-r--r--   0        0        0     2450 2023-06-07 00:11:48.873084 clear_skies_aws-1.4.3/src/clearskies_aws/actions/assume_role_test.py
+-rw-r--r--   0        0        0     7064 2023-06-07 12:04:20.019789 clear_skies_aws-1.4.3/src/clearskies_aws/actions/ses.py
+-rw-r--r--   0        0        0     1630 2023-06-07 12:04:20.019789 clear_skies_aws-1.4.3/src/clearskies_aws/actions/ses_test.py
+-rw-r--r--   0        0        0     2284 2023-06-07 12:04:20.019789 clear_skies_aws-1.4.3/src/clearskies_aws/actions/sns.py
+-rw-r--r--   0        0        0     2180 2023-06-07 12:04:20.019789 clear_skies_aws-1.4.3/src/clearskies_aws/actions/sns_test.py
+-rw-r--r--   0        0        0     2387 2023-06-07 12:04:20.019789 clear_skies_aws-1.4.3/src/clearskies_aws/actions/sqs.py
+-rw-r--r--   0        0        0     2234 2023-06-06 22:38:31.426673 clear_skies_aws-1.4.3/src/clearskies_aws/actions/sqs_test.py
+-rw-r--r--   0        0        0       83 2023-03-26 15:10:17.430380 clear_skies_aws-1.4.3/src/clearskies_aws/backends/__init__.py
+-rw-r--r--   0        0        0    29126 2023-05-17 10:18:33.296047 clear_skies_aws-1.4.3/src/clearskies_aws/backends/dynamo_db_backend.py
+-rw-r--r--   0        0        0    13150 2023-04-27 10:33:09.319573 clear_skies_aws-1.4.3/src/clearskies_aws/backends/dynamo_db_backend_test.py
+-rw-r--r--   0        0        0     2726 2023-03-26 15:10:17.430380 clear_skies_aws-1.4.3/src/clearskies_aws/backends/sqs_backend.py
+-rw-r--r--   0        0        0     1138 2023-03-26 15:10:17.430380 clear_skies_aws-1.4.3/src/clearskies_aws/backends/sqs_backend_test.py
+-rw-r--r--   0        0        0      290 2023-03-26 15:10:17.430380 clear_skies_aws-1.4.3/src/clearskies_aws/contexts/__init__.py
+-rw-r--r--   0        0        0     1305 2023-03-26 13:26:58.707778 clear_skies_aws-1.4.3/src/clearskies_aws/contexts/__pycache__/aws_http_api_gateway.cpython-38.pyc
+-rw-r--r--   0        0        0     1276 2023-03-26 13:26:58.707778 clear_skies_aws-1.4.3/src/clearskies_aws/contexts/__pycache__/aws_lambda_api_gateway.cpython-38.pyc
+-rw-r--r--   0        0        0     1251 2023-03-26 13:26:58.707778 clear_skies_aws-1.4.3/src/clearskies_aws/contexts/__pycache__/aws_lambda_elb.cpython-38.pyc
+-rw-r--r--   0        0        0      506 2023-03-26 15:10:17.430380 clear_skies_aws-1.4.3/src/clearskies_aws/contexts/cli.py
+-rw-r--r--   0        0        0     1002 2023-03-26 13:26:58.703778 clear_skies_aws-1.4.3/src/clearskies_aws/contexts/lambda_api_gateway.py
+-rw-r--r--   0        0        0      952 2023-03-26 13:26:58.703778 clear_skies_aws-1.4.3/src/clearskies_aws/contexts/lambda_elb.py
+-rw-r--r--   0        0        0     1009 2023-03-26 13:26:58.703778 clear_skies_aws-1.4.3/src/clearskies_aws/contexts/lambda_http_gateway.py
+-rw-r--r--   0        0        0     1183 2023-03-26 13:26:58.703778 clear_skies_aws-1.4.3/src/clearskies_aws/contexts/lambda_invocation.py
+-rw-r--r--   0        0        0     1678 2023-04-04 23:13:02.122630 clear_skies_aws-1.4.3/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch.py
+-rw-r--r--   0        0        0     1999 2023-03-26 15:10:17.430380 clear_skies_aws-1.4.3/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch_test.py
+-rw-r--r--   0        0        0       56 2023-03-26 13:26:58.711778 clear_skies_aws-1.4.3/src/clearskies_aws/di/__init__.py
+-rw-r--r--   0        0        0      775 2023-03-26 15:10:17.430380 clear_skies_aws-1.4.3/src/clearskies_aws/di/standard_dependencies.py
+-rw-r--r--   0        0        0      233 2023-03-26 15:10:17.430380 clear_skies_aws-1.4.3/src/clearskies_aws/input_outputs/__init__.py
+-rw-r--r--   0        0        0      943 2023-03-26 13:26:58.715778 clear_skies_aws-1.4.3/src/clearskies_aws/input_outputs/__pycache__/aws_http_api_gateway.cpython-38.pyc
+-rw-r--r--   0        0        0     3710 2023-03-26 13:26:58.715778 clear_skies_aws-1.4.3/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_api_gateway.cpython-38.pyc
+-rw-r--r--   0        0        0     2761 2023-03-26 13:26:58.715778 clear_skies_aws-1.4.3/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_api_gateway_test.cpython-38.pyc
+-rw-r--r--   0        0        0      901 2023-03-26 13:26:58.715778 clear_skies_aws-1.4.3/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_elb.cpython-38.pyc
+-rw-r--r--   0        0        0     2932 2023-03-26 13:26:58.711778 clear_skies_aws-1.4.3/src/clearskies_aws/input_outputs/lambda_api_gateway.py
+-rw-r--r--   0        0        0     2845 2023-03-26 13:26:58.711778 clear_skies_aws-1.4.3/src/clearskies_aws/input_outputs/lambda_api_gateway_test.py
+-rw-r--r--   0        0        0      662 2023-03-26 13:26:58.711778 clear_skies_aws-1.4.3/src/clearskies_aws/input_outputs/lambda_elb.py
+-rw-r--r--   0        0        0      692 2023-03-26 13:26:58.711778 clear_skies_aws-1.4.3/src/clearskies_aws/input_outputs/lambda_http_gateway.py
+-rw-r--r--   0        0        0      715 2023-03-26 13:26:58.711778 clear_skies_aws-1.4.3/src/clearskies_aws/input_outputs/lambda_invocation.py
+-rw-r--r--   0        0        0     2047 2023-03-26 15:10:17.430380 clear_skies_aws-1.4.3/src/clearskies_aws/input_outputs/lambda_sqs_standard.py
+-rw-r--r--   0        0        0       22 2023-05-23 15:29:05.208303 clear_skies_aws-1.4.3/src/clearskies_aws/mocks/__init__.py
+-rw-r--r--   0        0        0       21 2023-05-23 15:29:05.208303 clear_skies_aws-1.4.3/src/clearskies_aws/mocks/actions/__init__.py
+-rw-r--r--   0        0        0      911 2023-05-23 15:29:05.208303 clear_skies_aws-1.4.3/src/clearskies_aws/mocks/actions/ses.py
+-rw-r--r--   0        0        0      121 2023-03-26 13:26:58.715778 clear_skies_aws-1.4.3/src/clearskies_aws/secrets/__init__.py
+-rw-r--r--   0        0        0     1919 2023-05-19 13:30:13.392139 clear_skies_aws-1.4.3/src/clearskies_aws/secrets/additional_configs/__init__.py
+-rw-r--r--   0        0        0     1082 2023-03-26 13:26:58.719778 clear_skies_aws-1.4.3/src/clearskies_aws/secrets/additional_configs/iam_db_auth.py
+-rw-r--r--   0        0        0     3467 2023-05-19 13:34:03.783513 clear_skies_aws-1.4.3/src/clearskies_aws/secrets/additional_configs/iam_db_auth_with_ssm.py
+-rw-r--r--   0        0        0     3776 2023-03-26 13:26:58.719778 clear_skies_aws-1.4.3/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssh_cert_bastion.py
+-rw-r--r--   0        0        0     6444 2023-03-26 13:26:58.719778 clear_skies_aws-1.4.3/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssm_bastion.py
+-rw-r--r--   0        0        0     1655 2023-04-14 14:57:45.726909 clear_skies_aws-1.4.3/src/clearskies_aws/secrets/parameter_store.py
+-rw-r--r--   0        0        0      761 2023-03-26 13:26:58.715778 clear_skies_aws-1.4.3/src/clearskies_aws/secrets/parameter_store_test.py
+-rw-r--r--   0        0        0     2898 2023-04-14 14:57:45.758909 clear_skies_aws-1.4.3/src/clearskies_aws/secrets/secrets_manager.py
+-rw-r--r--   0        0        0      786 2023-03-26 13:26:58.715778 clear_skies_aws-1.4.3/src/clearskies_aws/secrets/secrets_manager_test.py
+-rwxr-xr-x   0        0        0      705 2022-01-16 00:35:11.272652 clear_skies_aws-1.4.3/src/test.py
+-rw-r--r--   0        0        0     8579 1970-01-01 00:00:00.000000 clear_skies_aws-1.4.3/PKG-INFO
```

### Comparing `clear-skies-aws-1.4.2/LICENSE` & `clear_skies_aws-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.4.2/PKG-INFO` & `clear_skies_aws-1.4.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: clear-skies-aws
-Version: 1.4.2
-Summary: clearskies bindings for working in AWS
-Home-page: https://github.com/cmancone/clearskies-aws
-Author: Conor Mancone
-Author-email: cmancone@gmail.com
-License: MIT
-Keywords: setuptools development
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # clearskies-aws
 
 clearskies bindings for working in AWS, which means additional:
 
  - backends (DynamoDB, SQS)
  - Secret/environment integrations (parameter store/secret manager)
  - DB connectivity via IAM auth
```

### Comparing `clear-skies-aws-1.4.2/README.md` & `clear_skies_aws-1.4.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: clear-skies-aws
+Version: 1.4.3
+Summary: clearskies bindings for working in AWS
+Home-page: https://github.com/cmancone/clearskies-aws
+License: MIT
+Author: Conor Mancone
+Author-email: cmancone@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: akeyless
+Provides-Extra: ses
+Requires-Dist: boto3 (>=1.26.148,<2.0.0)
+Requires-Dist: clear-skies (>=1.14.4,<2.0.0)
+Project-URL: Repository, https://github.com/cmancone/clearskies-aws
+Description-Content-Type: text/markdown
+
 # clearskies-aws
 
 clearskies bindings for working in AWS, which means additional:
 
  - backends (DynamoDB, SQS)
  - Secret/environment integrations (parameter store/secret manager)
  - DB connectivity via IAM auth
@@ -169,7 +191,8 @@
 ```
 
 Of course normally you wouldn't want to interact with it directly.  Adding `IAMDBAuth` to your `additional_configs` and setting up the necessary environemnt variables will be sufficient that any models that use the `cursor_backend` will connect via IAM DB Auth, rather than using hard-coded passwords.
 
 ## IAM DB Auth with SSM Bastion
 
 Coming shortly
+
```

### Comparing `clear-skies-aws-1.4.2/src/clearskies_aws/actions/ses.py` & `clear_skies_aws-1.4.3/src/clearskies_aws/actions/ses.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,44 @@
-from typing import List
-import datetime
+import boto3
 import clearskies
+import datetime
+
 from botocore.exceptions import ClientError
+from clearskies.environment import Environment
+from clearskies.models import Models
 from collections.abc import Sequence
-class SES:
-    def __init__(self, boto3, di):
-        self.boto3 = boto3
-        self.di = di
+from mypy_boto3_ses import SESClient
+from typing import Any, Callable, List, Optional, Union
+
+from ..di import StandardDependencies
+from .assume_role import AssumeRole
+from .action_aws import ActionAws
+class SES(ActionAws):
+    def __init__(self, environment: Environment, boto3: boto3, di: StandardDependencies) -> None:
+        """Setup action."""
+        super().__init__(environment, boto3, di)
 
     def configure(
         self,
         sender,
-        to=None,
-        cc=None,
-        bcc=None,
-        subject=None,
-        message=None,
-        subject_template=None,
-        message_template=None,
-        subject_template_file=None,
-        message_template_file=None,
-        assume_role=None,
-        dependencies_for_template=None,
-        when=None,
+        to: Optional[Union[list, str]] = None,
+        cc: Optional[Union[list, str]] = None,
+        bcc: Optional[Union[list, str]] = None,
+        subject: Optional[str] = None,
+        message: Optional[str] = None,
+        subject_template: Optional[str] = None,
+        message_template: Optional[str] = None,
+        subject_template_file: Optional[str] = None,
+        message_template_file: Optional[str] = None,
+        assume_role: Optional[AssumeRole] = None,
+        dependencies_for_template: Optional[list[Any]] = None,
+        when: Optional[Callable] = None,
     ) -> None:
         """Configure the rules for this email notification."""
+        super().configure(message_callable=None, when=when, assume_role=assume_role)
         self.destinations = {
             "to": [],
             "cc": [],
             "bcc": [],
         }
         # this just moves the data from the various "to" inputs (to, cc, bcc) into the self.destinations
         # dictionary, after normalizing it so that it is always a list.
@@ -42,17 +52,14 @@
                 self.destinations[key] = destination_values
         self.subject = subject
         self.message = message
         self.sender = sender
         self.subject_template = None
         self.message_template = None
         self.dependencies_for_template = dependencies_for_template if dependencies_for_template else []
-        if when is not None and not callable(when):
-            raise ValueError("'when' must be a callable but it was something else")
-        self.when = when
 
         if not to and not cc:
             raise ValueError("You must configure at least one 'to' address or one 'cc' address")
         num_subjects = 0
         num_messages = 0
         for source in [subject, subject_template, subject_template_file]:
             if source:
@@ -81,31 +88,21 @@
             import jinja2
             with open(message_template_file, "r", encoding="utf-8") as template:
                 self.message_template = jinja2.Template(template.read())
         elif message_template:
             import jinja2
             self.message_template = jinja2.Template(message_template)
 
-        self.assume_role = assume_role
-
-    def __call__(self, model) -> None:
+    def _execute_action(self, client: SESClient, model: Models) -> None:
         """Send a notification as configured."""
         utcnow = self.di.build('utcnow')
-        if self.when and not self.di.call_function(self.when, model=model):
-            return
-
-        if self.assume_role:
-            boto3 = self.assume_role(self.boto3)
-        else:
-            boto3 = self.boto3
 
-        ses = boto3.client("ses")
         tos = self._resolve_destination("to", model)
         try:
-            response = ses.send_email(
+            response = client.send_email(
                 Destination={
                     "ToAddresses": tos,
                     "CcAddresses": self._resolve_destination("cc", model),
                     "BccAddresses": self._resolve_destination("bcc", model),
                 },
                 Message={
                     "Body": {
@@ -174,12 +171,12 @@
             return self.subject
 
         if self.subject_template:
             return str(self.subject_template.render(model=model, now=now, **self.more_template_variables()))
 
         return ""
 
-    def more_template_variables(self):
+    def more_template_variables(self) -> dict[str, Any]:
         more_variables = {}
         for dependency_name in self.dependencies_for_template:
             more_variables[dependency_name] = self.di.build(dependency_name)
         return more_variables
```

### Comparing `clear-skies-aws-1.4.2/src/clearskies_aws/actions/sqs.py` & `clear_skies_aws-1.4.3/src/clearskies_aws/actions/sqs.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,78 +1,64 @@
-from typing import List
+import boto3
+import json
 import datetime
-import clearskies
+
 from botocore.exceptions import ClientError
+from clearskies.environment import Environment
+from clearskies.models import Models
 from collections.abc import Sequence
-class SQS:
-    def __init__(self, environment, boto3, di):
-        self.environment = environment
-        self.boto3 = boto3
-        self.di = di
+from collections import OrderedDict
+from mypy_boto3_sqs import SQSClient
+from typing import List, Optional, Callable
+
+from ..di import StandardDependencies
+from . import assume_role
+from .action_aws import ActionAws
+class SQS(ActionAws):
+    def __init__(self, environment: Environment, boto3: boto3, di: StandardDependencies) -> None:
+        """Setup action."""
+        super().__init__(environment, boto3, di)
 
     def configure(
         self,
-        queue_url=None,
-        queue_url_environment_key=None,
-        queue_url_callable=None,
-        message_callable=None,
-        when=None,
+        queue_url: str = '',
+        queue_url_environment_key: str = '',
+        queue_url_callable: Optional[Callable] = None,
+        message_callable: Optional[Callable] = None,
+        when: Optional[Callable] = None,
+        assume_role: Optional[assume_role.AssumeRole] = None,
     ) -> None:
-        self.when = when
-        self.message_callable = message_callable
+        super().configure(message_callable=message_callable, when=when, assume_role=assume_role)
+
         self.queue_url = queue_url
-        self.queue_url_environment_key = self.queue_url_environment_key
-        self.queue_url_callable = self.queue_url_callable
+        self.queue_url_environment_key = queue_url_environment_key
+        self.queue_url_callable = queue_url_callable
 
-        if self.message_callable and not callable(self.message_callable):
-            raise ValueError(
-                "'message_callable' should be a callable that returns the message for the queue, but a callable was not passed."
-            )
         queue_urls = 0
         for value in [queue_url, queue_url_environment_key, queue_url_callable]:
             if value:
                 queue_urls += 1
         if queue_urls > 1:
             raise ValueError(
                 "You can only provide one of 'queue_url', 'queue_url_environment_key', or 'queue_url_callable', but more than one were provided."
             )
         if not queue_urls:
             raise ValueError(
                 "You must provide at least one of 'queue_url', 'queue_url_environment_key', or 'queue_url_callable'."
             )
-        if when and not callable(when):
-            raise ValueError("'when' must be a callable but something else was found")
 
-    def __call__(self, model) -> None:
+    def _execute_action(self, client, model) -> None:
         """Send a notification as configured."""
-        if self.when and not self.di.call_function(self.when, model=model):
-            return
-
-        if self.assume_role:
-            boto3 = self.assume_role(self.boto3)
-        else:
-            boto3 = self.boto3
-
-        boto3.client("sqs").send_message(
-            QueueUrl=self.get_queue_url(model),
-            MessageBody=self.get_message_body(model),
-        )
+        try:
+            client.send_message(
+                QueueUrl=self.get_queue_url(model),
+                MessageBody=self.get_message_body(model),
+            )
+        except ClientError as e:
+            raise e
 
-    def get_queue_url(self):
+    def get_queue_url(self, model):
         if self.queue_url:
             return self.queue_url
         if self.queue_url_environment_key:
             return self.environment.get(self.queue_url_environment_key)
         return self.di.call_function(self.queue_url_callable, model=model)
-
-    def get_message_body(self, model):
-        if self.message_callable:
-            return self.di.call_function(self.message_callable, model=model)
-        #json = OrderedDict()
-        #for (output_name, column) in self._as_json_map.items():
-        #column_data = column.to_json(model)
-        #if type(column_data) == dict:
-        #for (key, value) in column_data.items():
-        #json[self.auto_case_column_name(key, True)] = value
-        #else:
-        #json[output_name] = column_data
-        #return json
```

### Comparing `clear-skies-aws-1.4.2/src/clearskies_aws/backends/dynamo_db_backend.py` & `clear_skies_aws-1.4.3/src/clearskies_aws/backends/dynamo_db_backend.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.4.2/src/clearskies_aws/backends/sqs_backend.py` & `clear_skies_aws-1.4.3/src/clearskies_aws/backends/sqs_backend.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.4.2/src/clearskies_aws/contexts/lambda_api_gateway.py` & `clear_skies_aws-1.4.3/src/clearskies_aws/contexts/lambda_api_gateway.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.4.2/src/clearskies_aws/contexts/lambda_elb.py` & `clear_skies_aws-1.4.3/src/clearskies_aws/contexts/lambda_elb.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.4.2/src/clearskies_aws/contexts/lambda_http_gateway.py` & `clear_skies_aws-1.4.3/src/clearskies_aws/contexts/lambda_http_gateway.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.4.2/src/clearskies_aws/contexts/lambda_invocation.py` & `clear_skies_aws-1.4.3/src/clearskies_aws/contexts/lambda_invocation.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.4.2/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch.py` & `clear_skies_aws-1.4.3/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.4.2/src/clearskies_aws/di/standard_dependencies.py` & `clear_skies_aws-1.4.3/src/clearskies_aws/di/standard_dependencies.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.4.2/src/clearskies_aws/input_outputs/lambda_api_gateway.py` & `clear_skies_aws-1.4.3/src/clearskies_aws/input_outputs/lambda_api_gateway.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.4.2/src/clearskies_aws/input_outputs/lambda_elb.py` & `clear_skies_aws-1.4.3/src/clearskies_aws/input_outputs/lambda_elb.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.4.2/src/clearskies_aws/input_outputs/lambda_http_gateway.py` & `clear_skies_aws-1.4.3/src/clearskies_aws/input_outputs/lambda_http_gateway.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.4.2/src/clearskies_aws/input_outputs/lambda_invocation.py` & `clear_skies_aws-1.4.3/src/clearskies_aws/input_outputs/lambda_invocation.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.4.2/src/clearskies_aws/input_outputs/lambda_sqs_standard.py` & `clear_skies_aws-1.4.3/src/clearskies_aws/input_outputs/lambda_sqs_standard.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.4.2/src/clearskies_aws/mocks/actions/ses.py` & `clear_skies_aws-1.4.3/src/clearskies_aws/mocks/actions/ses.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.4.2/src/clearskies_aws/secrets/additional_configs/__init__.py` & `clear_skies_aws-1.4.3/src/clearskies_aws/secrets/additional_configs/__init__.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.4.2/src/clearskies_aws/secrets/additional_configs/iam_db_auth.py` & `clear_skies_aws-1.4.3/src/clearskies_aws/secrets/additional_configs/iam_db_auth.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.4.2/src/clearskies_aws/secrets/additional_configs/iam_db_auth_with_ssm.py` & `clear_skies_aws-1.4.3/src/clearskies_aws/secrets/additional_configs/iam_db_auth_with_ssm.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.4.2/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssh_cert_bastion.py` & `clear_skies_aws-1.4.3/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssh_cert_bastion.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.4.2/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssm_bastion.py` & `clear_skies_aws-1.4.3/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssm_bastion.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.4.2/src/clearskies_aws/secrets/parameter_store.py` & `clear_skies_aws-1.4.3/src/clearskies_aws/secrets/parameter_store.py`

 * *Files identical despite different names*

### Comparing `clear-skies-aws-1.4.2/src/clearskies_aws/secrets/secrets_manager.py` & `clear_skies_aws-1.4.3/src/clearskies_aws/secrets/secrets_manager.py`

 * *Files identical despite different names*

