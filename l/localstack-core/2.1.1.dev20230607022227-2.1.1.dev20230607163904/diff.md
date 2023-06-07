# Comparing `tmp/localstack-core-2.1.1.dev20230607022227.tar.gz` & `tmp/localstack-core-2.1.1.dev20230607163904.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localstack-core-2.1.1.dev20230607022227.tar", last modified: Wed Jun  7 02:22:34 2023, max compression
+gzip compressed data, was "localstack-core-2.1.1.dev20230607163904.tar", last modified: Wed Jun  7 16:39:11 2023, max compression
```

## Comparing `localstack-core-2.1.1.dev20230607022227.tar` & `localstack-core-2.1.1.dev20230607163904.tar`

### file list

```diff
@@ -1,849 +1,849 @@
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.398749 localstack-core-2.1.1.dev20230607022227/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/LICENSE.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      216 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/MANIFEST.in
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15152 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/Makefile
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-06-07 02:22:34.398749 localstack-core-2.1.1.dev20230607022227/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10791 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/README.md
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.278755 localstack-core-2.1.1.dev20230607022227/bin/
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)      543 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/bin/localstack
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)     5936 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/bin/localstack-supervisor
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       29 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/bin/localstack.bat
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.278755 localstack-core-2.1.1.dev20230607022227/localstack/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       40 2023-06-07 02:22:27.000000 localstack-core-2.1.1.dev20230607022227/localstack/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.278755 localstack-core-2.1.1.dev20230607022227/localstack/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/accounts.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.278755 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      371 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.278755 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/acm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17594 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/acm/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.278755 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/apigateway/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    72874 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/apigateway/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.278755 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/cloudcontrol/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10727 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/cloudcontrol/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.278755 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/cloudformation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    84791 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/cloudformation/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.278755 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    42875 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/cloudwatch/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.278755 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/config/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   125975 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/config/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6224 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/core.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.278755 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/dynamodb/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    81315 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/dynamodb/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.278755 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/dynamodbstreams/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6998 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/dynamodbstreams/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.278755 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/ec2/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   755668 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/ec2/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.282755 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/es/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    60425 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/es/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.282755 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/events/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    55327 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/events/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.282755 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/firehose/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    42200 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/firehose/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.282755 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/iam/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   102907 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/iam/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.282755 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    25818 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/kinesis/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.282755 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/kms/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    48662 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/kms/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.282755 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/lambda_/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    71916 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/lambda_/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.282755 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/logs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    35937 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/logs/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.282755 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/opensearch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    67985 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/opensearch/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.282755 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/redshift/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   129662 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/redshift/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.282755 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/resource_groups/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14546 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/resource_groups/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.282755 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/resourcegroupstaggingapi/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8578 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/resourcegroupstaggingapi/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.282755 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/route53/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    67927 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/route53/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.282755 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/route53resolver/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    52075 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/route53resolver/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.282755 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/s3/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   132536 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/s3/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.282755 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/s3control/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    65907 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/s3control/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.282755 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/secretsmanager/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21744 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/secretsmanager/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.282755 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/ses/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    54804 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/ses/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.282755 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/sns/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27429 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/sns/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.282755 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/sqs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16662 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/sqs/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.282755 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/ssm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   215900 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/ssm/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.282755 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/stepfunctions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33164 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/stepfunctions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.282755 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/sts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9713 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/sts/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.282755 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/support/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16691 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/support/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.282755 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/swf/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    59679 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/swf/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.286755 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/transcribe/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    40302 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/api/transcribe/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4447 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/app.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8455 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/chain.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8023 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    22554 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/connect.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8959 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/forwarder.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      998 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/gateway.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.286755 localstack-core-2.1.1.dev20230607022227/localstack/aws/handlers/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1665 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/handlers/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2548 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/handlers/analytics.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2137 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/handlers/auth.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/handlers/codec.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9926 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/handlers/cors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2285 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/handlers/fallback.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1320 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/handlers/internal.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      843 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/handlers/internal_requests.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6990 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/handlers/legacy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5877 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/handlers/logging.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6368 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/handlers/metric_handler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10511 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/handlers/partition_rewriter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      650 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/handlers/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      665 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/handlers/region.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      862 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/handlers/routes.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11961 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/handlers/service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2924 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/handlers/service_plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13758 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/mocking.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.286755 localstack-core-2.1.1.dev20230607022227/localstack/aws/protocol/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/protocol/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15278 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/protocol/op_router.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    49972 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/protocol/parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    75997 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/protocol/serializer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14590 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/protocol/service_router.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5316 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/protocol/validate.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1912 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20281 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/scaffold.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.286755 localstack-core-2.1.1.dev20230607022227/localstack/aws/serving/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/serving/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2377 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/serving/asgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1060 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/serving/edge.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1424 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/serving/hypercorn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      775 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/serving/werkzeug.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1446 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/serving/wsgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7908 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/skeleton.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28256 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/spec-patches.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7072 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/spec.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12624 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/aws/trace.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.286755 localstack-core-2.1.1.dev20230607022227/localstack/cli/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      176 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/cli/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/cli/console.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26867 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/cli/localstack.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4220 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/cli/lpm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      477 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/cli/main.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      879 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/cli/plugin.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3429 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/cli/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1385 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/cli/profiles.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    50308 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/config.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7855 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/constants.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.286755 localstack-core-2.1.1.dev20230607022227/localstack/contrib/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/contrib/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11774 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/deprecations.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.286755 localstack-core-2.1.1.dev20230607022227/localstack/extensions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/extensions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.290754 localstack-core-2.1.1.dev20230607022227/localstack/extensions/api/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      138 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/extensions/api/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/extensions/api/aws.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2588 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/extensions/api/extension.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      422 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/extensions/api/http.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       84 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/extensions/api/runtime.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/extensions/api/services.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.290754 localstack-core-2.1.1.dev20230607022227/localstack/http/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      213 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/http/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2933 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/http/adapters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14117 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/http/asgi.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5518 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/http/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2397 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/http/dispatcher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5116 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/http/hypercorn.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7159 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/http/proxy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11089 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/http/request.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4124 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/http/resource.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3232 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/http/response.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17344 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/http/router.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.290754 localstack-core-2.1.1.dev20230607022227/localstack/logging/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/logging/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4844 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/logging/format.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4230 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/logging/setup.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.290754 localstack-core-2.1.1.dev20230607022227/localstack/packages/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      533 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/packages/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15427 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/packages/api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6728 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/packages/core.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1296 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/packages/debugpy.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1390 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/packages/ffmpeg.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      337 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/packages/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1313 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/packages/terraform.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1174 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/plugins.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.290754 localstack-core-2.1.1.dev20230607022227/localstack/runtime/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/runtime/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2672 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/runtime/analytics.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/runtime/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      289 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/runtime/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3114 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/runtime/hooks.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6440 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/runtime/init.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      817 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/runtime/main.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1415 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/runtime/shutdown.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.290754 localstack-core-2.1.1.dev20230607022227/localstack/services/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.290754 localstack-core-2.1.1.dev20230607022227/localstack/services/acm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/acm/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6530 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/acm/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.294754 localstack-core-2.1.1.dev20230607022227/localstack/services/apigateway/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/apigateway/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6200 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/apigateway/context.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    52139 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/apigateway/helpers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    34633 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/apigateway/integration.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13880 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/apigateway/invocations.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2564 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/apigateway/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11959 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/apigateway/patches.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    74708 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/apigateway/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5657 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/apigateway/router_asf.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11189 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/apigateway/templates.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.294754 localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24219 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/api_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.294754 localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/event_source_listeners/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/event_source_listeners/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9215 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/event_source_listeners/adapters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2923 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3064 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/event_source_listeners/event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3931 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11855 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    18555 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      519 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/hooks.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.294754 localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/invocation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      202 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/invocation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17789 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/invocation/docker_runtime_executor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4894 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/invocation/executor_endpoint.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21256 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/invocation/lambda_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28306 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/invocation/lambda_service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      914 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/invocation/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      406 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/invocation/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12705 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/invocation/runtime_environment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3908 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/invocation/runtime_executor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    32558 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/invocation/version_manager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    91684 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/lambda_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    72329 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/lambda_executors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1012 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/lambda_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4273 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/lambda_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17196 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/lambda_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.294754 localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/layerfetcher/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/layerfetcher/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      603 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/layerfetcher/layer_fetcher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4843 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1504 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)   155097 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7878 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/urlrouter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      396 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/usage.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.310753 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3644 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/api_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2058 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/cfn_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6247 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/deploy.html
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8513 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/deployment_utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.310753 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/engine/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/engine/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13077 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/engine/entities.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7994 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/engine/parameters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      454 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/engine/policy_loader.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    63509 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/engine/template_deployer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7451 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/engine/template_preparer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2309 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/engine/transformers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2044 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/engine/yaml_parser.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.314753 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      428 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    32657 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/apigateway.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20947 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/awslambda.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1201 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/cdk.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2242 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/certificatemanager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7009 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/cloudformation.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2126 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/cloudwatch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5391 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/dynamodb.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    22846 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/ec2.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2585 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/ecr.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2778 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/elasticsearch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8984 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    28326 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/iam.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3062 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/kinesis.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2112 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/kinesisfirehose.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5326 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/kms.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4769 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/logs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2643 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/opensearch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1177 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/redshift.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1414 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/resourcegroups.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3449 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/route53.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13557 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/s3.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6426 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/secretsmanager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8745 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/sns.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5299 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/sqs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3812 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/ssm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5502 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/stepfunctions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      668 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      247 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    39161 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5711 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/service_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2983 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/stores.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/usage.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.314753 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudwatch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15545 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudwatch/alarm_scheduler.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16188 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/cloudwatch/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.314753 localstack-core-2.1.1.dev20230607022227/localstack/services/configservice/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/configservice/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       92 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/configservice/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.314753 localstack-core-2.1.1.dev20230607022227/localstack/services/dynamodb/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/dynamodb/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1198 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/dynamodb/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/dynamodb/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/dynamodb/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    73281 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/dynamodb/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6106 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/dynamodb/server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10712 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/dynamodb/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.314753 localstack-core-2.1.1.dev20230607022227/localstack/services/dynamodbstreams/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/dynamodbstreams/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4420 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/dynamodbstreams/dynamodbstreams_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      359 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/dynamodbstreams/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6039 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/dynamodbstreams/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.314753 localstack-core-2.1.1.dev20230607022227/localstack/services/ec2/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/ec2/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1801 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/ec2/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      553 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/ec2/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    20653 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/ec2/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19131 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/edge.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.314753 localstack-core-2.1.1.dev20230607022227/localstack/services/es/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/es/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/es/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16936 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/es/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.318753 localstack-core-2.1.1.dev20230607022227/localstack/services/events/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/events/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      306 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/events/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    22448 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/events/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2675 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/events/scheduler.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.318753 localstack-core-2.1.1.dev20230607022227/localstack/services/firehose/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/firehose/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6345 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/firehose/mappers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      620 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/firehose/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    31864 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/firehose/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24573 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/generic_proxy.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.318753 localstack-core-2.1.1.dev20230607022227/localstack/services/iam/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/iam/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19454 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/iam/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16051 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/infra.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12094 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/internal.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.318753 localstack-core-2.1.1.dev20230607022227/localstack/services/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/kinesis/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6613 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/kinesis/kinesis_mock_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       75 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/kinesis/kinesis_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      641 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/kinesis/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1719 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/kinesis/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      224 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/kinesis/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7005 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/kinesis/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.318753 localstack-core-2.1.1.dev20230607022227/localstack/services/kms/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/kms/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2688 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/kms/local_kms_provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2592 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/kms/local_kms_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    35960 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/kms/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      837 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/kms/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/kms/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    52700 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/kms/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      895 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/kms/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.318753 localstack-core-2.1.1.dev20230607022227/localstack/services/logs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/logs/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/logs/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16491 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/logs/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1411 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/messages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7244 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/moto.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1903 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/motoserver.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.322753 localstack-core-2.1.1.dev20230607022227/localstack/services/opensearch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/opensearch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24093 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/opensearch/cluster.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15264 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/opensearch/cluster_manager.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      631 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/opensearch/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13589 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/opensearch/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      222 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/opensearch/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26686 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/opensearch/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9592 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/opensearch/versions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    26188 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11565 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/providers.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.322753 localstack-core-2.1.1.dev20230607022227/localstack/services/redshift/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/redshift/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2039 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/redshift/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.322753 localstack-core-2.1.1.dev20230607022227/localstack/services/resourcegroups/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/resourcegroups/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      125 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/resourcegroups/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.322753 localstack-core-2.1.1.dev20230607022227/localstack/services/resourcegroupstaggingapi/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/resourcegroupstaggingapi/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      190 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/resourcegroupstaggingapi/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.322753 localstack-core-2.1.1.dev20230607022227/localstack/services/route53/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/route53/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      411 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/route53/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2682 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/route53/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.322753 localstack-core-2.1.1.dev20230607022227/localstack/services/route53resolver/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/route53resolver/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8323 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/route53resolver/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33479 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/route53resolver/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2223 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/route53resolver/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.326753 localstack-core-2.1.1.dev20230607022227/localstack/services/s3/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/s3/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1974 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/s3/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12543 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/s3/cors.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3411 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/s3/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3609 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/s3/multipart_content.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27704 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/s3/notifications.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    31371 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/s3/presigned_url.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    69800 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/s3/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    68303 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/s3/s3_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15062 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/s3/s3_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17709 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/s3/s3_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9488 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/s3/utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5562 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/s3/virtual_host.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    15516 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/s3/website_hosting.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.326753 localstack-core-2.1.1.dev20230607022227/localstack/services/s3control/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/s3control/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/s3control/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.326753 localstack-core-2.1.1.dev20230607022227/localstack/services/secretsmanager/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/secretsmanager/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    27770 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/secretsmanager/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.326753 localstack-core-2.1.1.dev20230607022227/localstack/services/ses/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/ses/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      441 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/ses/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    21127 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/ses/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.326753 localstack-core-2.1.1.dev20230607022227/localstack/services/sns/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/sns/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/sns/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5649 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/sns/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    43125 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/sns/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    54630 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/sns/publisher.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.326753 localstack-core-2.1.1.dev20230607022227/localstack/services/sqs/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/sqs/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1616 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/sqs/constants.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/sqs/exceptions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    36763 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/sqs/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    54820 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/sqs/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7427 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/sqs/query_api.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6878 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/sqs/utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.326753 localstack-core-2.1.1.dev20230607022227/localstack/services/ssm/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/ssm/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9298 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/ssm/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.326753 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.326753 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.326753 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/antlt4utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/antlt4utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      844 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.326753 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.334752 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.334752 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/catch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/catch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1098 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/catch/catch_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3652 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      165 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/catch/catcher_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/catch/catcher_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/cause_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      215 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/comment.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/error_decl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.334752 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/error_name/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/error_name/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      618 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2660 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      646 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1961 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.334752 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/flow/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/flow/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      299 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/flow/end.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      421 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/flow/next.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      233 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/flow/start_at.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      568 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/parameters.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.334752 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/path/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/path/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      708 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/path/input_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      719 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/path/items_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      649 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/path/output_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      685 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/path/result_path.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.334752 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/payload/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/payload/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.334752 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payload_value.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.334752 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      625 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.342752 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      643 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1037 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      803 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      961 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      699 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.342752 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      727 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.342752 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_bool.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      277 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_float.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_int.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_lit.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      264 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_null.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_str.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      659 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/result_selector.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.342752 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/retry/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/retry/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      679 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      604 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      550 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3289 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/retry/retrier_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/retry/retrier_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1434 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      105 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/retry/retry_outcome.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      180 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/component.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      890 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/eval_component.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.346752 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.346752 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/argument/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/argument/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      268 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_bool.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      269 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_float.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      661 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      265 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_int.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      623 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      647 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      266 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      175 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/component.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.350751 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.350751 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.354751 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1153 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1698 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1760 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1570 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2277 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2077 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1869 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.354751 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2006 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1988 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4499 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.354751 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3708 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.354751 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_algorithm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2837 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.354751 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3146 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1297 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1387 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.354751 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1936 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2307 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      576 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1167 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2143 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1190 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.354751 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2138 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.362751 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1176 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.362751 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/functionname/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/functionname/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      232 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/functionname/custom_function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      209 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/functionname/function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      484 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/functionname/states_function_name.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      398 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/member.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/member_access.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      221 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/program.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.362751 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/program/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/program/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3629 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/program/program.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.362751 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5973 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.362751 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_choice/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_choice/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1559 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule_stmt.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      350 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_choice/choices_decl.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.362751 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      999 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3059 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1268 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2309 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1063 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      157 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_stmt.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.362751 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1236 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.374750 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1422 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3490 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4233 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4496 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5038 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      334 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/operator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      228 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_choice/default_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2479 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      361 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_continue_with.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.374750 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_execution/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_execution/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6356 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.374750 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.374750 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3857 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      128 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor_props.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/processor_config.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/max_concurrency.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/mode.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2870 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.374750 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1550 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1445 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.374750 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.374750 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3549 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1950 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5439 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4672 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5376 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3633 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6149 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.374750 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_fail/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_fail/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1150 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.374750 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_pass/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_pass/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_pass/result.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2575 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1356 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_props.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.374750 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_succeed/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_succeed/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1416 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_type.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.374750 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_wait/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_wait/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1151 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      776 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.374750 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      600 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      762 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1352 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1041 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1702 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      278 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/states.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.378750 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/eval/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/eval/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.378750 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/eval/contextobject/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/eval/contextobject/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      983 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      498 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/eval/count_down_latch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4700 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/eval/environment.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.378750 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/eval/event/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/eval/event/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3681 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/eval/event/event_detail.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1207 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/eval/event/event_history.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1707 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/eval/program_worker.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.382750 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/eval/programstate/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/eval/programstate/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      140 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/eval/programstate/program_ended.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      347 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/eval/programstate/program_error.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      945 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/eval/programstate/program_running.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       50 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/eval/programstate/program_state.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      464 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/eval/programstate/program_stopped.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.382750 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/parse/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/parse/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      790 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/parse/asl_parser.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.382750 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/parse/intrinsic/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/parse/intrinsic/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      876 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5292 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    31040 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/parse/preprocessor.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      964 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/parse/typed_props.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.382750 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      373 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/utils/encoding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      352 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/utils/json_path.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.382750 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/backend/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/backend/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6485 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/backend/execution.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2617 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/backend/execution_worker.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      386 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/backend/execution_worker_comm.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1540 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/backend/state_machine.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/backend/store.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7014 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/packages.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      262 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/plugins.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2587 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/provider.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10366 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/provider_v2.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4342 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/stepfunctions_starter.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      645 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/stepfunctions_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11179 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/stores.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.382750 localstack-core-2.1.1.dev20230607022227/localstack/services/sts/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/sts/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      621 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/sts/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.382750 localstack-core-2.1.1.dev20230607022227/localstack/services/support/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/support/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/support/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.382750 localstack-core-2.1.1.dev20230607022227/localstack/services/swf/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/swf/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      106 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/swf/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.382750 localstack-core-2.1.1.dev20230607022227/localstack/services/transcribe/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/transcribe/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/transcribe/models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12937 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/services/transcribe/provider.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.382750 localstack-core-2.1.1.dev20230607022227/localstack/state/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      307 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/state/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3774 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/state/core.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6216 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/state/inspect.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11061 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/state/pickle.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      751 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/state/snapshot.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.382750 localstack-core-2.1.1.dev20230607022227/localstack/testing/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/testing/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.382750 localstack-core-2.1.1.dev20230607022227/localstack/testing/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/testing/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5828 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/testing/aws/asf_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1466 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/testing/aws/cloudformation_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4452 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/testing/aws/lambda_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6709 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/testing/aws/util.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.386750 localstack-core-2.1.1.dev20230607022227/localstack/testing/pytest/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/testing/pytest/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1611 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/testing/pytest/detect_thread_leakage.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1089 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/testing/pytest/filters.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/testing/pytest/find_orphaned_snapshots.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1473 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/testing/pytest/fixture_conflicts.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    69013 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/testing/pytest/fixtures.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2320 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/testing/pytest/metric_collection.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4565 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/testing/pytest/snapshot.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      941 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/testing/pytest/util.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.386750 localstack-core-2.1.1.dev20230607022227/localstack/testing/snapshots/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      158 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/testing/snapshots/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12355 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/testing/snapshots/prototype.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5012 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/testing/snapshots/report.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9496 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/testing/snapshots/transformer.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    25882 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/testing/snapshots/transformer_utility.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.390750 localstack-core-2.1.1.dev20230607022227/localstack/utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/__init__.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.394749 localstack-core-2.1.1.dev20230607022227/localstack/utils/analytics/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      290 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/analytics/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2410 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/analytics/cli.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3102 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/analytics/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/analytics/events.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1397 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/analytics/logger.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3324 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/analytics/metadata.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8421 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/analytics/publisher.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3926 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/analytics/service_request_aggregator.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3841 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/analytics/usage.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     8479 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/archives.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      282 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/async_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4396 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/asyncio.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2415 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/auth.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.398749 localstack-core-2.1.1.dev20230607022227/localstack/utils/aws/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/aws/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13624 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/aws/arns.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    14834 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/aws/aws_models.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10896 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/aws/aws_responses.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    17098 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/aws/aws_stack.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2926 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/aws/client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    13412 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/aws/client_types.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5833 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/aws/dead_letter_queue.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    11782 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/aws/message_forwarding.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3437 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/aws/queries.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7899 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/aws/request_context.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7915 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/aws/resources.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6780 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/aws/templating.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    24003 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/bootstrap.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.398749 localstack-core-2.1.1.dev20230607022227/localstack/utils/cloudwatch/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/cloudwatch/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6253 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/cloudwatch/cloudwatch_util.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16629 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/collections.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6561 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/common.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2343 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/config_listener.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5253 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/container_networking.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.398749 localstack-core-2.1.1.dev20230607022227/localstack/utils/container_utils/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/container_utils/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    45835 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/container_utils/container_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    32496 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/container_utils/docker_cmd_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    33160 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/container_utils/docker_sdk_client.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      701 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/coverage_docs.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     7181 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/crypto.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4683 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/diagnose.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9027 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/docker_utils.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9365 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/files.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2966 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/functions.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     9391 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/http.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6182 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/json.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.398749 localstack-core-2.1.1.dev20230607022227/localstack/utils/kinesis/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/kinesis/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4127 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/kinesis/kclipy_helper.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    19202 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/kinesis/kinesis_connector.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2416 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/kinesis/kinesis_util.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    10069 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/net.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      811 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/no_exit_argument_parser.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/numbers.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6176 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/objects.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4923 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/patch.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1553 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/platform.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    16617 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/run.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6547 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/scheduler.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.398749 localstack-core-2.1.1.dev20230607022227/localstack/utils/server/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/server/__init__.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    12408 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/server/http2_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      149 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/server/multiserver.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5822 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/server/proxy_server.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     6037 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/serving.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2300 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/ssl.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5724 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/strings.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3725 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/sync.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      829 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/tagging.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2952 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/tail.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    23504 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/testutil.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4851 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/threads.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1834 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/time.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1235 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/urls.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3202 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/venv.py
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1146 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/localstack/utils/xml.py
-drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 02:22:34.398749 localstack-core-2.1.1.dev20230607022227/localstack_core.egg-info/
--rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-06-07 02:22:34.000000 localstack-core-2.1.1.dev20230607022227/localstack_core.egg-info/PKG-INFO
--rw-rw-r--   0 circleci  (1001) circleci  (1002)    37703 2023-06-07 02:22:34.000000 localstack-core-2.1.1.dev20230607022227/localstack_core.egg-info/SOURCES.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-06-07 02:22:34.000000 localstack-core-2.1.1.dev20230607022227/localstack_core.egg-info/dependency_links.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     4957 2023-06-07 02:22:34.000000 localstack-core-2.1.1.dev20230607022227/localstack_core.egg-info/entry_points.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-06-07 02:22:30.000000 localstack-core-2.1.1.dev20230607022227/localstack_core.egg-info/not-zip-safe
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     5044 2023-06-07 02:22:30.000000 localstack-core-2.1.1.dev20230607022227/localstack_core.egg-info/plux.json
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     2814 2023-06-07 02:22:34.000000 localstack-core-2.1.1.dev20230607022227/localstack_core.egg-info/requires.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)       11 2023-06-07 02:22:34.000000 localstack-core-2.1.1.dev20230607022227/localstack_core.egg-info/top_level.txt
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     1450 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/pyproject.toml
--rw-rw-r--   0 circleci  (1001) circleci  (1002)     3145 2023-06-07 02:22:34.398749 localstack-core-2.1.1.dev20230607022227/setup.cfg
--rwxrwxr-x   0 circleci  (1001) circleci  (1002)       60 2023-06-07 01:28:52.000000 localstack-core-2.1.1.dev20230607022227/setup.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.973053 localstack-core-2.1.1.dev20230607163904/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/LICENSE.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      216 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/MANIFEST.in
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15152 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/Makefile
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-06-07 16:39:11.973053 localstack-core-2.1.1.dev20230607163904/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10791 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/README.md
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.877049 localstack-core-2.1.1.dev20230607163904/bin/
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)      543 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/bin/localstack
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)     5936 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/bin/localstack-supervisor
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       29 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/bin/localstack.bat
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.877049 localstack-core-2.1.1.dev20230607163904/localstack/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       40 2023-06-07 16:39:04.000000 localstack-core-2.1.1.dev20230607163904/localstack/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.877049 localstack-core-2.1.1.dev20230607163904/localstack/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/accounts.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.877049 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      371 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.877049 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/acm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17594 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/acm/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.877049 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/apigateway/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    72874 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/apigateway/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.877049 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/cloudcontrol/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10727 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/cloudcontrol/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.877049 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/cloudformation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    84791 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/cloudformation/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.877049 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    42875 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/cloudwatch/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.877049 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/config/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   125975 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/config/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6224 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/core.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.881049 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/dynamodb/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    81315 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/dynamodb/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.881049 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/dynamodbstreams/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6998 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/dynamodbstreams/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.881049 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/ec2/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   755668 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/ec2/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.881049 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/es/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    60425 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/es/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.881049 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/events/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    55327 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/events/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.881049 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/firehose/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    42200 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/firehose/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.881049 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/iam/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   102907 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/iam/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.881049 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    25818 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/kinesis/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.881049 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/kms/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    48662 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/kms/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.881049 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/lambda_/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    71916 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/lambda_/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.881049 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/logs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    35937 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/logs/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.881049 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/opensearch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    67985 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/opensearch/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.881049 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/redshift/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   129662 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/redshift/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.881049 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/resource_groups/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14546 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/resource_groups/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.881049 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/resourcegroupstaggingapi/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8578 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/resourcegroupstaggingapi/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.881049 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/route53/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    67927 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/route53/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.881049 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/route53resolver/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    52075 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/route53resolver/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.881049 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/s3/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   132536 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/s3/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.881049 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/s3control/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    65907 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/s3control/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.881049 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/secretsmanager/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21744 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/secretsmanager/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.881049 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/ses/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    54804 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/ses/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.881049 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/sns/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27429 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/sns/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.881049 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/sqs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16662 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/sqs/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.881049 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/ssm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   215900 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/ssm/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.885050 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/stepfunctions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33164 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/stepfunctions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.885050 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/sts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9713 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/sts/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.885050 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/support/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16691 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/support/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.885050 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/swf/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    59679 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/swf/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.885050 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/transcribe/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    40302 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/api/transcribe/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4447 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/app.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8455 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/chain.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8023 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    22554 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/connect.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8959 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/forwarder.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      998 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/gateway.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.885050 localstack-core-2.1.1.dev20230607163904/localstack/aws/handlers/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1665 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/handlers/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2548 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/handlers/analytics.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2137 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/handlers/auth.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/handlers/codec.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9926 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/handlers/cors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2285 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/handlers/fallback.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1320 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/handlers/internal.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      843 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/handlers/internal_requests.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6990 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/handlers/legacy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5877 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/handlers/logging.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6368 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/handlers/metric_handler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10511 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/handlers/partition_rewriter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      650 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/handlers/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      665 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/handlers/region.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      862 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/handlers/routes.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11961 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/handlers/service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2924 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/handlers/service_plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13758 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/mocking.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.885050 localstack-core-2.1.1.dev20230607163904/localstack/aws/protocol/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/protocol/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15278 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/protocol/op_router.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    49972 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/protocol/parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    75997 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/protocol/serializer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14590 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/protocol/service_router.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5316 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/protocol/validate.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1912 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20281 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/scaffold.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.885050 localstack-core-2.1.1.dev20230607163904/localstack/aws/serving/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/serving/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2377 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/serving/asgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1060 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/serving/edge.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1424 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/serving/hypercorn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      775 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/serving/werkzeug.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1446 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/serving/wsgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7908 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/skeleton.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28256 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/spec-patches.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7072 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/spec.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12624 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/aws/trace.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.889050 localstack-core-2.1.1.dev20230607163904/localstack/cli/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      176 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/cli/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/cli/console.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26867 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/cli/localstack.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4220 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/cli/lpm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      477 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/cli/main.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      879 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/cli/plugin.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3429 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/cli/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1385 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/cli/profiles.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    50308 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/config.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7855 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/constants.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.889050 localstack-core-2.1.1.dev20230607163904/localstack/contrib/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/contrib/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11774 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/deprecations.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.889050 localstack-core-2.1.1.dev20230607163904/localstack/extensions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/extensions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.889050 localstack-core-2.1.1.dev20230607163904/localstack/extensions/api/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      138 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/extensions/api/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/extensions/api/aws.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2588 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/extensions/api/extension.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      422 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/extensions/api/http.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       84 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/extensions/api/runtime.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/extensions/api/services.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.889050 localstack-core-2.1.1.dev20230607163904/localstack/http/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      213 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/http/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2933 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/http/adapters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14117 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/http/asgi.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5518 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/http/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2397 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/http/dispatcher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5116 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/http/hypercorn.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7159 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/http/proxy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11089 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/http/request.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4124 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/http/resource.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3232 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/http/response.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17344 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/http/router.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.889050 localstack-core-2.1.1.dev20230607163904/localstack/logging/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/logging/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4844 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/logging/format.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4230 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/logging/setup.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.889050 localstack-core-2.1.1.dev20230607163904/localstack/packages/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      533 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/packages/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15427 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/packages/api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6728 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/packages/core.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1296 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/packages/debugpy.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1390 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/packages/ffmpeg.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      337 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/packages/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1313 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/packages/terraform.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1174 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/plugins.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.889050 localstack-core-2.1.1.dev20230607163904/localstack/runtime/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/runtime/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2672 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/runtime/analytics.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/runtime/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      289 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/runtime/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3114 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/runtime/hooks.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6440 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/runtime/init.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      817 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/runtime/main.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1415 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/runtime/shutdown.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.893050 localstack-core-2.1.1.dev20230607163904/localstack/services/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.893050 localstack-core-2.1.1.dev20230607163904/localstack/services/acm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/acm/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6530 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/acm/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.893050 localstack-core-2.1.1.dev20230607163904/localstack/services/apigateway/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/apigateway/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6200 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/apigateway/context.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    61607 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/apigateway/helpers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    34633 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/apigateway/integration.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14059 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/apigateway/invocations.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2725 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/apigateway/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11959 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/apigateway/patches.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    74955 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/apigateway/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5657 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/apigateway/router_asf.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11189 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/apigateway/templates.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.893050 localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24219 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/api_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.897050 localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/event_source_listeners/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/event_source_listeners/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9215 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/event_source_listeners/adapters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2923 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3064 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/event_source_listeners/event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3931 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11855 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    18555 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      519 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/hooks.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.897050 localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/invocation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      202 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/invocation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17789 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/invocation/docker_runtime_executor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4894 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/invocation/executor_endpoint.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21256 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/invocation/lambda_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28306 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/invocation/lambda_service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      914 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/invocation/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      406 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/invocation/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12705 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/invocation/runtime_environment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3908 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/invocation/runtime_executor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    32558 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/invocation/version_manager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    91684 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/lambda_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    72329 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/lambda_executors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1012 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/lambda_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4273 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/lambda_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17196 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/lambda_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.897050 localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/layerfetcher/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/layerfetcher/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      603 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/layerfetcher/layer_fetcher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4843 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1504 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)   155097 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7878 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/urlrouter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      396 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/usage.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.897050 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3644 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/api_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2058 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/cfn_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6247 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/deploy.html
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8513 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/deployment_utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.897050 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/engine/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/engine/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13077 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/engine/entities.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7994 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/engine/parameters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      454 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/engine/policy_loader.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    63509 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/engine/template_deployer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7451 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/engine/template_preparer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2309 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/engine/transformers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2044 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/engine/yaml_parser.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.901050 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      428 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    32657 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/apigateway.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20947 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/awslambda.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1201 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/cdk.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2242 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/certificatemanager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7009 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/cloudformation.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2126 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/cloudwatch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5391 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/dynamodb.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    22846 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/ec2.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2585 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/ecr.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2778 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/elasticsearch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8984 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    28326 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/iam.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3062 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/kinesis.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2112 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/kinesisfirehose.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5326 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/kms.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4769 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/logs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2643 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/opensearch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1177 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/redshift.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1414 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/resourcegroups.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3449 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/route53.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13557 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/s3.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6426 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/secretsmanager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8745 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/sns.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5299 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/sqs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3812 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/ssm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5502 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/stepfunctions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      668 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      247 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    39161 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5711 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/service_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2983 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/stores.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/usage.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.901050 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudwatch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15545 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudwatch/alarm_scheduler.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16188 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/cloudwatch/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.901050 localstack-core-2.1.1.dev20230607163904/localstack/services/configservice/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/configservice/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       92 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/configservice/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.901050 localstack-core-2.1.1.dev20230607163904/localstack/services/dynamodb/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/dynamodb/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1198 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/dynamodb/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3959 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/dynamodb/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/dynamodb/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    73281 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/dynamodb/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6106 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/dynamodb/server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10712 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/dynamodb/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.901050 localstack-core-2.1.1.dev20230607163904/localstack/services/dynamodbstreams/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/dynamodbstreams/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4420 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/dynamodbstreams/dynamodbstreams_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      359 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/dynamodbstreams/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6039 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/dynamodbstreams/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.901050 localstack-core-2.1.1.dev20230607163904/localstack/services/ec2/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/ec2/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1801 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/ec2/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      553 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/ec2/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    20653 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/ec2/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19131 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/edge.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.901050 localstack-core-2.1.1.dev20230607163904/localstack/services/es/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/es/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      234 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/es/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16936 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/es/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.905050 localstack-core-2.1.1.dev20230607163904/localstack/services/events/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/events/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      306 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/events/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    22448 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/events/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2675 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/events/scheduler.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.905050 localstack-core-2.1.1.dev20230607163904/localstack/services/firehose/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/firehose/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6345 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/firehose/mappers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      620 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/firehose/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    31864 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/firehose/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24573 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/generic_proxy.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.905050 localstack-core-2.1.1.dev20230607163904/localstack/services/iam/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/iam/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19454 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/iam/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16051 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/infra.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12094 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/internal.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.905050 localstack-core-2.1.1.dev20230607163904/localstack/services/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/kinesis/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6613 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/kinesis/kinesis_mock_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       75 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/kinesis/kinesis_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      641 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/kinesis/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1719 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/kinesis/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      224 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/kinesis/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7005 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/kinesis/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.905050 localstack-core-2.1.1.dev20230607163904/localstack/services/kms/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/kms/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2688 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/kms/local_kms_provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2592 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/kms/local_kms_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    35960 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/kms/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      837 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/kms/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/kms/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    52700 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/kms/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      895 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/kms/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.905050 localstack-core-2.1.1.dev20230607163904/localstack/services/logs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/logs/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      570 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/logs/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16491 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/logs/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1411 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/messages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7244 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/moto.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1903 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/motoserver.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.905050 localstack-core-2.1.1.dev20230607163904/localstack/services/opensearch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/opensearch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24093 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/opensearch/cluster.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15264 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/opensearch/cluster_manager.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      631 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/opensearch/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13589 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/opensearch/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      222 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/opensearch/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26686 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/opensearch/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9592 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/opensearch/versions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    26188 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11565 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/providers.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.905050 localstack-core-2.1.1.dev20230607163904/localstack/services/redshift/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/redshift/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2039 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/redshift/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.905050 localstack-core-2.1.1.dev20230607163904/localstack/services/resourcegroups/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/resourcegroups/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      125 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/resourcegroups/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.905050 localstack-core-2.1.1.dev20230607163904/localstack/services/resourcegroupstaggingapi/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/resourcegroupstaggingapi/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      190 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/resourcegroupstaggingapi/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.905050 localstack-core-2.1.1.dev20230607163904/localstack/services/route53/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/route53/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      411 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/route53/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2682 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/route53/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.909050 localstack-core-2.1.1.dev20230607163904/localstack/services/route53resolver/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/route53resolver/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8323 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/route53resolver/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33479 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/route53resolver/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2223 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/route53resolver/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.909050 localstack-core-2.1.1.dev20230607163904/localstack/services/s3/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/s3/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1974 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/s3/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12543 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/s3/cors.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3411 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/s3/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3609 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/s3/multipart_content.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27704 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/s3/notifications.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    31371 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/s3/presigned_url.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    69800 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/s3/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    68303 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/s3/s3_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15062 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/s3/s3_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17709 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/s3/s3_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9488 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/s3/utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5562 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/s3/virtual_host.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    15516 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/s3/website_hosting.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.909050 localstack-core-2.1.1.dev20230607163904/localstack/services/s3control/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/s3control/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      104 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/s3control/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.909050 localstack-core-2.1.1.dev20230607163904/localstack/services/secretsmanager/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/secretsmanager/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    27770 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/secretsmanager/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.909050 localstack-core-2.1.1.dev20230607163904/localstack/services/ses/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/ses/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      441 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/ses/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    21127 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/ses/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.909050 localstack-core-2.1.1.dev20230607163904/localstack/services/sns/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/sns/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/sns/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5649 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/sns/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    43125 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/sns/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    54630 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/sns/publisher.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.909050 localstack-core-2.1.1.dev20230607163904/localstack/services/sqs/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/sqs/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1616 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/sqs/constants.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/sqs/exceptions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    36763 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/sqs/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    54820 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/sqs/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7427 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/sqs/query_api.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6878 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/sqs/utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.909050 localstack-core-2.1.1.dev20230607163904/localstack/services/ssm/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/ssm/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9298 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/ssm/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.913051 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.913051 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.913051 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/antlt4utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/antlt4utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      844 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.913051 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.913051 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.913051 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/catch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/catch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1098 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/catch/catch_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3652 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      165 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/catch/catcher_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/catch/catcher_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/cause_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      215 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/comment.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      211 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/error_decl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.913051 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/error_name/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/error_name/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      618 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2660 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      518 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      646 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      686 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1961 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.917051 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/flow/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/flow/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      299 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/flow/end.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      421 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/flow/next.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      233 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/flow/start_at.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      568 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/parameters.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.917051 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/path/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/path/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      708 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/path/input_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      719 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/path/items_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      649 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/path/output_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      685 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/path/result_path.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.917051 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/payload/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/payload/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.917051 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      155 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payload_value.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.917051 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      625 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.917051 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      643 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1037 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      803 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      961 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      699 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.917051 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      727 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.917051 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_bool.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      277 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_float.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_int.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_lit.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      264 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_null.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      271 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadvaluelit/payload_value_str.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      659 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/result_selector.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.925051 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/retry/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/retry/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      679 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      604 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      550 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3289 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       95 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/retry/retrier_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/retry/retrier_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1434 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      105 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/retry/retry_outcome.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      180 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/component.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      890 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/eval_component.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.925051 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.929051 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/argument/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/argument/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      452 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      268 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_bool.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      269 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_float.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      661 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      265 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_int.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      623 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      647 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      266 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      175 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/component.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.929051 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      606 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.929051 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.929051 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1153 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1698 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1760 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1570 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2277 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2077 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1869 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.929051 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2006 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1988 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4499 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.933051 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3708 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.933051 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_algorithm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2837 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.933051 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3146 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1297 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1387 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.933051 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1936 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2307 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      576 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1167 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2143 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1190 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.933051 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2138 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.933051 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1176 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.937051 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/functionname/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/functionname/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      232 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/functionname/custom_function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      209 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/functionname/function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1071 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      484 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/functionname/states_function_name.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      398 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/member.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      287 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/member_access.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      221 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/program.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.937051 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/program/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/program/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3629 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/program/program.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.937051 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5973 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.937051 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_choice/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_choice/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1559 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      144 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule_stmt.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      350 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_choice/choices_decl.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.945052 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      999 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3059 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1268 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2309 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1063 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      157 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_stmt.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.945052 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1236 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.945052 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1422 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3490 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4233 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4496 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5038 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      334 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/operator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      228 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_choice/default_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2479 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      361 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_continue_with.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.945052 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_execution/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_execution/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6356 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.945052 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.945052 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3857 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      128 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor_props.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      450 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/processor_config.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      263 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/max_concurrency.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      154 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/mode.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2870 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.945052 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1550 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1445 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.945052 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.945052 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3549 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1950 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5439 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4672 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5376 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3633 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6149 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.945052 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_fail/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_fail/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1150 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.953052 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_pass/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_pass/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      205 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_pass/result.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2575 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1356 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_props.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.953052 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_succeed/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_succeed/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1416 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      346 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_type.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.953052 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_wait/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_wait/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1151 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      776 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.953052 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      600 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      762 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1352 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1041 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1702 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      278 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/states.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.953052 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/eval/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/eval/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.953052 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/eval/contextobject/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/eval/contextobject/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      983 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      498 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/eval/count_down_latch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4700 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/eval/environment.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.953052 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/eval/event/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/eval/event/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3681 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/eval/event/event_detail.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1207 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/eval/event/event_history.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1707 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/eval/program_worker.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.953052 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/eval/programstate/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/eval/programstate/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      140 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/eval/programstate/program_ended.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      347 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/eval/programstate/program_error.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      945 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/eval/programstate/program_running.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       50 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/eval/programstate/program_state.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      464 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/eval/programstate/program_stopped.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.953052 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/parse/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/parse/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      790 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/parse/asl_parser.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.953052 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/parse/intrinsic/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/parse/intrinsic/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      876 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5292 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    31040 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/parse/preprocessor.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      964 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/parse/typed_props.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.953052 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      373 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/utils/encoding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      352 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/utils/json_path.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.961052 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/backend/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/backend/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6485 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/backend/execution.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2617 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/backend/execution_worker.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      386 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/backend/execution_worker_comm.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1540 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/backend/state_machine.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      778 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/backend/store.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7014 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/packages.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      262 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/plugins.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2587 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/provider.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10366 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/provider_v2.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4342 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/stepfunctions_starter.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      645 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/stepfunctions_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11179 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/stores.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.961052 localstack-core-2.1.1.dev20230607163904/localstack/services/sts/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/sts/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      621 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/sts/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.961052 localstack-core-2.1.1.dev20230607163904/localstack/services/support/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/support/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      122 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/support/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.961052 localstack-core-2.1.1.dev20230607163904/localstack/services/swf/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/swf/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      106 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/swf/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.961052 localstack-core-2.1.1.dev20230607163904/localstack/services/transcribe/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/transcribe/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      376 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/transcribe/models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12937 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/services/transcribe/provider.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.961052 localstack-core-2.1.1.dev20230607163904/localstack/state/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      307 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/state/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3774 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/state/core.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6216 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/state/inspect.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11061 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/state/pickle.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      751 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/state/snapshot.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.961052 localstack-core-2.1.1.dev20230607163904/localstack/testing/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/testing/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.961052 localstack-core-2.1.1.dev20230607163904/localstack/testing/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/testing/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5828 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/testing/aws/asf_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1466 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/testing/aws/cloudformation_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4452 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/testing/aws/lambda_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6709 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/testing/aws/util.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.965052 localstack-core-2.1.1.dev20230607163904/localstack/testing/pytest/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/testing/pytest/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1611 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/testing/pytest/detect_thread_leakage.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1089 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/testing/pytest/filters.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1337 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/testing/pytest/find_orphaned_snapshots.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1473 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/testing/pytest/fixture_conflicts.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    69013 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/testing/pytest/fixtures.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2320 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/testing/pytest/metric_collection.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4565 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/testing/pytest/snapshot.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      941 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/testing/pytest/util.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.965052 localstack-core-2.1.1.dev20230607163904/localstack/testing/snapshots/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      158 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/testing/snapshots/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12355 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/testing/snapshots/prototype.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5012 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/testing/snapshots/report.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9496 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/testing/snapshots/transformer.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    25882 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/testing/snapshots/transformer_utility.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.969052 localstack-core-2.1.1.dev20230607163904/localstack/utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/__init__.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.969052 localstack-core-2.1.1.dev20230607163904/localstack/utils/analytics/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      290 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/analytics/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2410 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/analytics/cli.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3102 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/analytics/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      582 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/analytics/events.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1397 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/analytics/logger.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3324 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/analytics/metadata.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8421 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/analytics/publisher.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3926 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/analytics/service_request_aggregator.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3841 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/analytics/usage.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     8479 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/archives.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      282 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/async_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4396 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/asyncio.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2415 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/auth.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.969052 localstack-core-2.1.1.dev20230607163904/localstack/utils/aws/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/aws/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13624 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/aws/arns.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    14834 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/aws/aws_models.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10896 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/aws/aws_responses.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    17098 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/aws/aws_stack.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2926 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/aws/client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    13412 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/aws/client_types.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5833 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/aws/dead_letter_queue.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    11782 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/aws/message_forwarding.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3437 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/aws/queries.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7899 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/aws/request_context.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7915 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/aws/resources.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6780 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/aws/templating.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    24003 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/bootstrap.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.973053 localstack-core-2.1.1.dev20230607163904/localstack/utils/cloudwatch/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/cloudwatch/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6253 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/cloudwatch/cloudwatch_util.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16629 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/collections.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6561 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/common.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2343 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/config_listener.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5253 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/container_networking.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.973053 localstack-core-2.1.1.dev20230607163904/localstack/utils/container_utils/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/container_utils/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    45835 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/container_utils/container_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    32496 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/container_utils/docker_cmd_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    33160 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/container_utils/docker_sdk_client.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      701 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/coverage_docs.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     7181 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/crypto.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4683 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/diagnose.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9027 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/docker_utils.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9365 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/files.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2966 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/functions.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     9391 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/http.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6182 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/json.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.973053 localstack-core-2.1.1.dev20230607163904/localstack/utils/kinesis/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/kinesis/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4127 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/kinesis/kclipy_helper.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    19202 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/kinesis/kinesis_connector.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2416 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/kinesis/kinesis_util.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    10069 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/net.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      811 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/no_exit_argument_parser.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1288 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/numbers.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6176 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/objects.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4923 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/patch.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1553 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/platform.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    16617 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/run.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6547 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/scheduler.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.973053 localstack-core-2.1.1.dev20230607163904/localstack/utils/server/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/server/__init__.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    12408 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/server/http2_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      149 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/server/multiserver.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5822 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/server/proxy_server.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     6037 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/serving.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2300 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/ssl.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5724 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/strings.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3725 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/sync.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      829 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/tagging.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2952 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/tail.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    23504 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/testutil.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4851 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/threads.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1834 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/time.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1235 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/urls.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3202 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/venv.py
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1146 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/localstack/utils/xml.py
+drwxrwxr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-07 16:39:11.973053 localstack-core-2.1.1.dev20230607163904/localstack_core.egg-info/
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)      652 2023-06-07 16:39:11.000000 localstack-core-2.1.1.dev20230607163904/localstack_core.egg-info/PKG-INFO
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)    37703 2023-06-07 16:39:11.000000 localstack-core-2.1.1.dev20230607163904/localstack_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-06-07 16:39:11.000000 localstack-core-2.1.1.dev20230607163904/localstack_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     4957 2023-06-07 16:39:11.000000 localstack-core-2.1.1.dev20230607163904/localstack_core.egg-info/entry_points.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)        1 2023-06-07 16:39:08.000000 localstack-core-2.1.1.dev20230607163904/localstack_core.egg-info/not-zip-safe
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     5044 2023-06-07 16:39:08.000000 localstack-core-2.1.1.dev20230607163904/localstack_core.egg-info/plux.json
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     2814 2023-06-07 16:39:11.000000 localstack-core-2.1.1.dev20230607163904/localstack_core.egg-info/requires.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)       11 2023-06-07 16:39:11.000000 localstack-core-2.1.1.dev20230607163904/localstack_core.egg-info/top_level.txt
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     1450 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/pyproject.toml
+-rw-rw-r--   0 circleci  (1001) circleci  (1002)     3145 2023-06-07 16:39:11.973053 localstack-core-2.1.1.dev20230607163904/setup.cfg
+-rwxrwxr-x   0 circleci  (1001) circleci  (1002)       60 2023-06-07 16:04:27.000000 localstack-core-2.1.1.dev20230607163904/setup.py
```

### Comparing `localstack-core-2.1.1.dev20230607022227/LICENSE.txt` & `localstack-core-2.1.1.dev20230607163904/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/Makefile` & `localstack-core-2.1.1.dev20230607163904/Makefile`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/PKG-INFO` & `localstack-core-2.1.1.dev20230607163904/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack-core
-Version: 2.1.1.dev20230607022227
+Version: 2.1.1.dev20230607163904
 Summary: The core library and runtime of LocalStack
 Home-page: https://github.com/localstack/localstack
 Author: LocalStack Contributors
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `localstack-core-2.1.1.dev20230607022227/README.md` & `localstack-core-2.1.1.dev20230607163904/README.md`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/bin/localstack` & `localstack-core-2.1.1.dev20230607163904/bin/localstack`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/bin/localstack-supervisor` & `localstack-core-2.1.1.dev20230607163904/bin/localstack-supervisor`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/accounts.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/accounts.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/api/acm/__init__.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/api/acm/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/api/apigateway/__init__.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/api/apigateway/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/api/cloudcontrol/__init__.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/api/cloudcontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/api/cloudformation/__init__.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/api/cloudformation/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/api/cloudwatch/__init__.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/api/cloudwatch/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/api/config/__init__.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/api/config/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/api/core.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/api/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/api/dynamodb/__init__.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/api/dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/api/dynamodbstreams/__init__.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/api/dynamodbstreams/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/api/ec2/__init__.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/api/ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/api/es/__init__.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/api/es/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/api/events/__init__.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/api/events/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/api/firehose/__init__.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/api/firehose/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/api/iam/__init__.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/api/iam/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/api/kinesis/__init__.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/api/kinesis/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/api/kms/__init__.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/api/kms/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/api/lambda_/__init__.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/api/lambda_/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/api/logs/__init__.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/api/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/api/opensearch/__init__.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/api/opensearch/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/api/redshift/__init__.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/api/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/api/resource_groups/__init__.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/api/resource_groups/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/api/resourcegroupstaggingapi/__init__.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/api/resourcegroupstaggingapi/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/api/route53/__init__.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/api/route53/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/api/route53resolver/__init__.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/api/route53resolver/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/api/s3/__init__.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/api/s3/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/api/s3control/__init__.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/api/s3control/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/api/secretsmanager/__init__.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/api/secretsmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/api/ses/__init__.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/api/ses/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/api/sns/__init__.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/api/sns/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/api/sqs/__init__.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/api/sqs/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/api/ssm/__init__.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/api/ssm/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/api/stepfunctions/__init__.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/api/stepfunctions/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/api/sts/__init__.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/api/sts/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/api/support/__init__.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/api/support/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/api/swf/__init__.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/api/swf/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/api/transcribe/__init__.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/api/transcribe/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/app.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/app.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/chain.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/chain.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/client.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/connect.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/connect.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/forwarder.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/forwarder.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/gateway.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/gateway.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/handlers/__init__.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/handlers/analytics.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/handlers/analytics.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/handlers/auth.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/handlers/auth.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/handlers/codec.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/handlers/codec.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/handlers/cors.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/handlers/cors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/handlers/fallback.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/handlers/fallback.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/handlers/internal.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/handlers/internal.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/handlers/internal_requests.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/handlers/internal_requests.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/handlers/legacy.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/handlers/legacy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/handlers/logging.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/handlers/logging.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/handlers/metric_handler.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/handlers/metric_handler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/handlers/partition_rewriter.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/handlers/partition_rewriter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/handlers/proxy.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/handlers/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/handlers/region.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/handlers/region.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/handlers/routes.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/handlers/routes.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/handlers/service.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/handlers/service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/handlers/service_plugin.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/handlers/service_plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/mocking.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/mocking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/protocol/op_router.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/protocol/op_router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/protocol/parser.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/protocol/parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/protocol/serializer.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/protocol/serializer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/protocol/service_router.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/protocol/service_router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/protocol/validate.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/protocol/validate.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/proxy.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/scaffold.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/scaffold.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/serving/asgi.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/serving/asgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/serving/edge.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/serving/edge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/serving/hypercorn.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/serving/hypercorn.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/serving/werkzeug.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/serving/werkzeug.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/serving/wsgi.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/serving/wsgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/skeleton.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/skeleton.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/spec-patches.json` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/spec-patches.json`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/spec.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/spec.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/aws/trace.py` & `localstack-core-2.1.1.dev20230607163904/localstack/aws/trace.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/cli/localstack.py` & `localstack-core-2.1.1.dev20230607163904/localstack/cli/localstack.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/cli/lpm.py` & `localstack-core-2.1.1.dev20230607163904/localstack/cli/lpm.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/cli/plugin.py` & `localstack-core-2.1.1.dev20230607163904/localstack/cli/plugin.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/cli/plugins.py` & `localstack-core-2.1.1.dev20230607163904/localstack/cli/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/cli/profiles.py` & `localstack-core-2.1.1.dev20230607163904/localstack/cli/profiles.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/config.py` & `localstack-core-2.1.1.dev20230607163904/localstack/config.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/constants.py` & `localstack-core-2.1.1.dev20230607163904/localstack/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/deprecations.py` & `localstack-core-2.1.1.dev20230607163904/localstack/deprecations.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/extensions/api/aws.py` & `localstack-core-2.1.1.dev20230607163904/localstack/extensions/api/aws.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/extensions/api/extension.py` & `localstack-core-2.1.1.dev20230607163904/localstack/extensions/api/extension.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/http/adapters.py` & `localstack-core-2.1.1.dev20230607163904/localstack/http/adapters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/http/asgi.py` & `localstack-core-2.1.1.dev20230607163904/localstack/http/asgi.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/http/client.py` & `localstack-core-2.1.1.dev20230607163904/localstack/http/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/http/dispatcher.py` & `localstack-core-2.1.1.dev20230607163904/localstack/http/dispatcher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/http/hypercorn.py` & `localstack-core-2.1.1.dev20230607163904/localstack/http/hypercorn.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/http/proxy.py` & `localstack-core-2.1.1.dev20230607163904/localstack/http/proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/http/request.py` & `localstack-core-2.1.1.dev20230607163904/localstack/http/request.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/http/resource.py` & `localstack-core-2.1.1.dev20230607163904/localstack/http/resource.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/http/response.py` & `localstack-core-2.1.1.dev20230607163904/localstack/http/response.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/http/router.py` & `localstack-core-2.1.1.dev20230607163904/localstack/http/router.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/logging/format.py` & `localstack-core-2.1.1.dev20230607163904/localstack/logging/format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/logging/setup.py` & `localstack-core-2.1.1.dev20230607163904/localstack/logging/setup.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/packages/__init__.py` & `localstack-core-2.1.1.dev20230607163904/localstack/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/packages/api.py` & `localstack-core-2.1.1.dev20230607163904/localstack/packages/api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/packages/core.py` & `localstack-core-2.1.1.dev20230607163904/localstack/packages/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/packages/debugpy.py` & `localstack-core-2.1.1.dev20230607163904/localstack/packages/debugpy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/packages/ffmpeg.py` & `localstack-core-2.1.1.dev20230607163904/localstack/packages/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/packages/terraform.py` & `localstack-core-2.1.1.dev20230607163904/localstack/packages/terraform.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/plugins.py` & `localstack-core-2.1.1.dev20230607163904/localstack/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/runtime/analytics.py` & `localstack-core-2.1.1.dev20230607163904/localstack/runtime/analytics.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/runtime/hooks.py` & `localstack-core-2.1.1.dev20230607163904/localstack/runtime/hooks.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/runtime/init.py` & `localstack-core-2.1.1.dev20230607163904/localstack/runtime/init.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/runtime/main.py` & `localstack-core-2.1.1.dev20230607163904/localstack/runtime/main.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/runtime/shutdown.py` & `localstack-core-2.1.1.dev20230607163904/localstack/runtime/shutdown.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/acm/provider.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/acm/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/apigateway/context.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/apigateway/context.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/apigateway/helpers.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/apigateway/helpers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import contextlib
+import copy
 import json
 import logging
 import re
 import time
 from datetime import datetime, timezone
 from typing import Any, Callable, Dict, List, Optional, Tuple, TypedDict, Union
 from urllib import parse as urlparse
@@ -13,32 +14,42 @@
 from jsonpointer import JsonPointerException
 from moto.apigateway.models import Integration, Resource, RestAPI, apigateway_backends
 from moto.apigateway.utils import create_id as create_resource_id
 from requests.models import Response
 
 from localstack import config
 from localstack.aws.accounts import get_aws_account_id
-from localstack.aws.api.apigateway import Authorizer, ConnectionType, IntegrationType, Model
+from localstack.aws.api.apigateway import (
+    Authorizer,
+    ConnectionType,
+    IntegrationType,
+    Model,
+    RequestValidator,
+)
 from localstack.constants import (
     APPLICATION_JSON,
     HEADER_LOCALSTACK_EDGE_URL,
     LOCALHOST_HOSTNAME,
     PATH_USER_REQUEST,
 )
 from localstack.services.apigateway.context import ApiInvocationContext
-from localstack.services.apigateway.models import ApiGatewayStore, apigateway_stores
+from localstack.services.apigateway.models import (
+    ApiGatewayStore,
+    RestApiContainer,
+    apigateway_stores,
+)
 from localstack.utils import common
 from localstack.utils.aws import aws_stack, queries
 from localstack.utils.aws import resources as resource_utils
 from localstack.utils.aws.arns import parse_arn
 from localstack.utils.aws.aws_responses import requests_error_response_json, requests_response
 from localstack.utils.aws.request_context import MARKER_APIGW_REQUEST_REGION, THREAD_LOCAL
-from localstack.utils.json import canonical_json
 from localstack.utils.strings import long_uid, short_uid
 from localstack.utils.time import TIMESTAMP_FORMAT_TZ, timestamp
+from localstack.utils.urls import localstack_host
 
 LOG = logging.getLogger(__name__)
 
 REQUEST_TIME_DATE_FORMAT = "%d/%b/%Y:%H:%M:%S %z"
 
 # regex path pattern for user requests, handles stages like $default
 PATH_REGEX_USER_REQUEST = (
@@ -103,21 +114,23 @@
 # TODO: make the CRUD operations in this file generic for the different model types (authorizes, validators, ...)
 
 
 def get_apigateway_store(account_id: str = None, region: str = None) -> ApiGatewayStore:
     return apigateway_stores[account_id or get_aws_account_id()][region or aws_stack.get_region()]
 
 
-class Resolver:
-    def __init__(self, document: dict, allow_recursive=True):
+class OpenAPISpecificationResolver:
+    def __init__(self, document: dict, rest_api_id: str, allow_recursive=True):
         self.document = document
         self.allow_recursive = allow_recursive
         # cache which maps known refs to part of the document
         self._cache = {}
         self._refpaths = ["#"]
+        host_definition = localstack_host(use_localhost_cloud=True)
+        self._base_url = f"{config.get_protocol()}://apigateway.{host_definition.host_and_port()}/restapis/{rest_api_id}/models/"
 
     def _is_ref(self, item) -> bool:
         return isinstance(item, dict) and "$ref" in item
 
     def _is_internal_ref(self, refpath) -> bool:
         return str(refpath).startswith("#/")
 
@@ -134,27 +147,45 @@
         yield
         self._refpaths.pop()
 
     def _resolve_refpath(self, refpath: str) -> dict:
         if refpath in self._refpaths and not self.allow_recursive:
             raise Exception("recursion detected with allow_recursive=False")
 
-        if refpath in self._cache:
+        # We don't resolve the Model definition, we will return a absolute reference to the model like AWS
+        # When validating the schema, we will need to resolve the $ref there
+        # Because if we resolved all $ref in schema, it can lead to circular references in complex schemas
+        if self.current_path.startswith("#/definitions") or self.current_path.startswith(
+            "#/components/schemas"
+        ):
+            return {"$ref": f"{self._base_url}{refpath.rsplit('/', maxsplit=1)[-1]}"}
+
+        # We should not resolve the Model either, because we need its name to set it to the Request/ResponseModels,
+        # it just makes our job more difficult to retrieve the Model name
+        # We still need to verify that the ref exists
+        is_schema = self.current_path.endswith("schema")
+
+        if refpath in self._cache and not is_schema:
             return self._cache.get(refpath)
 
         with self._pathctx(refpath):
             if self._is_internal_ref(self.current_path):
                 cur = self.document
             else:
                 raise NotImplementedError("External references not yet supported.")
 
             for step in self.current_path.split("/")[1:]:
                 cur = cur.get(step)
 
             self._cache[self.current_path] = cur
+
+            if is_schema:
+                # If the $ref doesn't exist in our schema, return None, otherwise return the ref
+                return {"$ref": refpath} if cur else None
+
             return cur
 
     def _namespaced_resolution(self, namespace: str, data: Union[dict, list]) -> Union[dict, list]:
         with self._pathctx(namespace):
             return self._resolve_references(data)
 
     def _resolve_references(self, data) -> Union[dict, list]:
@@ -170,14 +201,139 @@
 
         return data
 
     def resolve_references(self) -> dict:
         return self._resolve_references(self.document)
 
 
+class ModelResolver:
+    """
+    This class allows a Model to use recursive and circular references to other Models.
+    To be able to JSON dump Models, AWS will not resolve Models but will use their absolute $ref instead.
+    When validating, we need to resolve those references, using JSON schema tricks to allow recursion.
+    See: https://json-schema.org/understanding-json-schema/structuring.html#recursion
+
+    To allow a simpler structure, we're not replacing directly the reference with the schema, but instead create
+    a map of all used schema in $defs, as advised on JSON schema:
+    See: https://json-schema.org/understanding-json-schema/structuring.html#defs
+
+    This allows us to not render every sub schema/models, but instead keep a clean map of used schemas.
+    """
+
+    def __init__(self, rest_api_container: RestApiContainer, model_name: str):
+        self.rest_api_container = rest_api_container
+        self.model_name = model_name
+        self._deps = {}
+        self._current_resolving_name = None
+
+    @contextlib.contextmanager
+    def _resolving_ctx(self, current_resolving_name: str):
+        self._current_resolving_name = current_resolving_name
+        yield
+        self._current_resolving_name = None
+
+    def resolve_model(self, model: dict) -> dict | None:
+        resolved_model = copy.deepcopy(model)
+        model_names = set()
+
+        def _look_for_ref(sub_model):
+            for key, value in sub_model.items():
+                if key == "$ref":
+                    ref_name = value.rsplit("/", maxsplit=1)[-1]
+                    if ref_name == self.model_name:
+                        # if we reference our main Model, use the # for recursive access
+                        sub_model[key] = "#"
+                        continue
+                    # otherwise, this Model will be available in $defs
+                    sub_model[key] = f"#/$defs/{ref_name}"
+
+                    if ref_name != self._current_resolving_name:
+                        # add the ref to the next ref to resolve and to $deps
+                        model_names.add(ref_name)
+
+                elif isinstance(value, dict):
+                    _look_for_ref(value)
+
+        if isinstance(resolved_model, dict):
+            _look_for_ref(resolved_model)
+
+        if model_names:
+            for ref_model_name in model_names:
+                if ref_model_name in self._deps:
+                    continue
+
+                def_resolved, was_resolved = self._get_resolved_submodel(model_name=ref_model_name)
+
+                if not def_resolved:
+                    return
+                # if the ref was already resolved, we copy the result to not alter the already resolved schema
+                if was_resolved:
+                    def_resolved = copy.deepcopy(def_resolved)
+
+                self._remove_self_ref(def_resolved)
+
+                if "$deps" in def_resolved:
+                    # this will happen only if the schema was already resolved, otherwise the deps would be in _deps
+                    # remove own definition in case of recursive / circular Models
+                    def_resolved["$defs"].pop(self.model_name, None)
+                    # remove the $defs from the schema, we don't want nested $defs
+                    def_resolved_defs = def_resolved.pop("$defs")
+                    # merge the resolved sub model $defs to the main schema
+                    self._deps.update(def_resolved_defs)
+
+                # add the dependencies to the global $deps
+                self._deps[ref_model_name] = def_resolved
+
+        return resolved_model
+
+    def _remove_self_ref(self, resolved_schema: dict):
+        for key, value in resolved_schema.items():
+            if key == "$ref":
+                ref_name = value.rsplit("/", maxsplit=1)[-1]
+                if ref_name == self.model_name:
+                    resolved_schema[key] = "#"
+
+            elif isinstance(value, dict):
+                self._remove_self_ref(value)
+
+    def get_resolved_model(self) -> dict | None:
+        if not (resolved_model := self.rest_api_container.resolved_models.get(self.model_name)):
+            model = self.rest_api_container.models.get(self.model_name)
+            if not model:
+                return None
+            schema = json.loads(model["schema"])
+            resolved_model = self.resolve_model(schema)
+            if not resolved_model:
+                return None
+            # attach the resolved dependencies of the schema
+            if self._deps:
+                resolved_model["$defs"] = self._deps
+            self.rest_api_container.resolved_models[self.model_name] = resolved_model
+
+        return resolved_model
+
+    def _get_resolved_submodel(self, model_name: str) -> tuple[dict | None, bool | None]:
+        was_resolved = True
+        if not (resolved_model := self.rest_api_container.resolved_models.get(model_name)):
+            was_resolved = False
+            model = self.rest_api_container.models.get(model_name)
+            if not model:
+                LOG.warning(
+                    "Error while validating the request body, could not the find the Model: '%s'",
+                    model_name,
+                )
+                return None, was_resolved
+            schema = json.loads(model["schema"])
+
+            with self._resolving_ctx(model_name):
+                resolved_model = self.resolve_model(schema)
+
+        return resolved_model, was_resolved
+
+
 class IntegrationParameters(TypedDict):
     path: Dict[str, str]
     querystring: Dict[str, str]
     headers: Dict[str, str]
 
 
 class RequestParametersResolver:
@@ -259,16 +415,18 @@
 
         if context.data:
             params["method.request.body"] = context.data
 
         return {key.lower(): val for key, val in params.items()}
 
 
-def resolve_references(data: dict, allow_recursive=True) -> dict:
-    resolver = Resolver(data, allow_recursive=allow_recursive)
+def resolve_references(data: dict, rest_api_id, allow_recursive=True) -> dict:
+    resolver = OpenAPISpecificationResolver(
+        data, allow_recursive=allow_recursive, rest_api_id=rest_api_id
+    )
     return resolver.resolve_references()
 
 
 def make_json_response(message):
     return requests_response(json.dumps(message), headers={"Content-Type": APPLICATION_JSON})
 
 
@@ -556,15 +714,15 @@
 
 
 def import_api_from_openapi_spec(
     rest_api: RestAPI, body: Dict, query_params: Dict, account_id: str = None, region: str = None
 ) -> Optional[RestAPI]:
     """Import an API from an OpenAPI spec document"""
 
-    resolved_schema = resolve_references(body)
+    resolved_schema = resolve_references(copy.deepcopy(body), rest_api_id=rest_api.id)
 
     # TODO:
     # 1. validate the "mode" property of the spec document, "merge" or "overwrite"
     # 2. validate the document type, "swagger" or "openapi"
 
     rest_api.version = str(resolved_schema.get("info", {}).get("version")) or None
     # XXX for some reason this makes cf tests fail that's why is commented.
@@ -586,17 +744,17 @@
         if not (security_schemes := path_payload.get("security")):
             return False
 
         for security_scheme in security_schemes:
             for security_scheme_name in security_scheme.keys():
                 # $.securityDefinitions is Swagger 2.0
                 # $.components.SecuritySchemes is OpenAPI 3.0
-                security_definitions = body.get("securityDefinitions") or body.get(
-                    "components", {}
-                ).get("securitySchemes", {})
+                security_definitions = resolved_schema.get(
+                    "securityDefinitions"
+                ) or resolved_schema.get("components", {}).get("securitySchemes", {})
                 if security_scheme_name in security_definitions:
                     security_config = security_definitions.get(security_scheme_name)
                     if (
                         OpenAPIExt.AUTHORIZER not in security_config
                         and security_config.get("type") == "apiKey"
                         and security_config.get("name", "").lower() == "x-api-key"
                     ):
@@ -607,17 +765,17 @@
         if not (security_schemes := path_payload.get("security")):
             return None
 
         for security_scheme in security_schemes:
             for security_scheme_name in security_scheme.keys():
                 # $.securityDefinitions is Swagger 2.0
                 # $.components.SecuritySchemes is OpenAPI 3.0
-                security_definitions = body.get("securityDefinitions") or body.get(
-                    "components", {}
-                ).get("securitySchemes", {})
+                security_definitions = resolved_schema.get(
+                    "securityDefinitions"
+                ) or resolved_schema.get("components", {}).get("securitySchemes", {})
                 if security_scheme_name in security_definitions:
                     security_config = security_definitions.get(security_scheme_name)
                     aws_apigateway_authorizer = security_config.get(OpenAPIExt.AUTHORIZER, {})
                     if not aws_apigateway_authorizer:
                         continue
 
                     if authorizer := authorizers.get(security_scheme_name):
@@ -714,19 +872,20 @@
 
             # Create the `Method` resource for each method path
             method_resource = create_method_resource(resource, method_name, field_schema)
 
             # Get the `Method` requestParameters and requestModels
             request_parameters_schema = field_schema.get("parameters", [])
             request_parameters = {}
+            request_models = {}
             if request_parameters_schema:
-                request_models = {}
                 for req_param_data in request_parameters_schema:
-                    # TODO: does `required` attribute maps to a RequestValidator? check with AWS
-                    # Possible values for `in` from the specs are "query", "header", "path", "formData" or "body".
+                    # For Swagger 2.0, possible values for `in` from the specs are "query", "header", "path",
+                    # "formData" or "body".
+                    # For OpenAPI 3.0, values are "query", "header", "path" or "cookie".
                     # Only "path", "header" and "query" are supported in API Gateway for requestParameters
                     # "body" is mapped to a requestModel
                     param_location = req_param_data.get("in")
                     param_name = req_param_data.get("name")
                     param_required = req_param_data.get("required", False)
                     if param_location in ("query", "header", "path"):
                         if param_location == "query":
@@ -742,52 +901,86 @@
                     else:
                         LOG.warning(
                             "Ignoring unsupported requestParameters/requestModels location value for %s: %s",
                             param_name,
                             param_location,
                         )
                         continue
-                method_resource.request_models = request_models or None
+
+            # this replaces 'body' in Parameters for OpenAPI 3.0, a requestBody Object
+            # https://swagger.io/specification/v3/#request-body-object
+            if request_models_schema := field_schema.get("requestBody"):
+                model_ref = None
+                for content_type, media_type in request_models_schema.get("content", {}).items():
+                    # we're iterating over the Media Type object:
+                    # https://swagger.io/specification/v3/#media-type-object
+                    if content_type == APPLICATION_JSON:
+                        model_ref = media_type.get("schema", {}).get("$ref")
+                        continue
+                    LOG.warning(
+                        "Found '%s' content-type for the MethodResponse model for path '%s' and method '', not adding the model as currently not supported",
+                        content_type,
+                        rel_path,
+                        method_name,
+                    )
+                if model_ref:
+                    model_schema = model_ref.rsplit("/", maxsplit=1)[-1]
+                    request_models = {APPLICATION_JSON: model_schema}
+
+            method_resource.request_models = request_models or None
+
+            # check if there's a request validator set in the method
+            request_validator_name = field_schema.get(
+                OpenAPIExt.REQUEST_VALIDATOR, default_req_validator_name
+            )
+            if request_validator_name:
+                if not (
+                    req_validator_id := request_validator_name_id_map.get(request_validator_name)
+                ):
+                    # Might raise an exception here if we properly validate the template
+                    LOG.warning(
+                        "A validator ('%s') was referenced for %s.(%s), but is not defined",
+                        request_validator_name,
+                        rel_path,
+                        method_name,
+                    )
+                method_resource.request_validator_id = req_validator_id
 
             # we check if there's a path parameter, AWS adds the requestParameter automatically
             resource_path_part = parts[-1].strip("/")
             if is_variable_path(resource_path_part) and not is_greedy_path(resource_path_part):
                 path_parameter = resource_path_part[1:-1]  # remove the curly braces
                 request_parameters[f"method.request.path.{path_parameter}"] = True
 
             method_resource.request_parameters = request_parameters or None
 
             # Create the `MethodResponse` for the previously created `Method`
             method_responses = field_schema.get("responses", {})
             for method_status_code, method_response in method_responses.items():
                 method_response_model = None
-                model_schema = None
-
+                model_ref = None
                 # separating the two different versions, Swagger (2.0) and OpenAPI 3.0
                 if "schema" in method_response:  # this is Swagger
-                    model_schema = method_response["schema"]
+                    model_ref = method_response["schema"].get("$ref")
                 elif "content" in method_response:  # this is OpenAPI 3.0
                     for content_type, media_type in method_response["content"].items():
                         # we're iterating over the Media Type object:
                         # https://swagger.io/specification/v3/#media-type-object
                         if content_type == APPLICATION_JSON:
-                            model_schema = media_type.get("schema")
+                            model_ref = media_type.get("schema", {}).get("$ref")
                             continue
                         LOG.warning(
                             "Found '%s' content-type for the MethodResponse model for path '%s' and method '', not adding the model as currently not supported",
                             content_type,
                             rel_path,
                             method_name,
                         )
 
-                if model_schema:
-                    if isinstance(model_schema, dict):
-                        # this means the model schema was resolved directly from the schema, instead of its name
-                        # we dump the model to canonical JSON to be able to retrieve its name
-                        model_schema = schema_map.get(canonical_json(model_schema))
+                if model_ref:
+                    model_schema = model_ref.rsplit("/", maxsplit=1)[-1]
 
                     method_response_model = {APPLICATION_JSON: model_schema}
 
                 method_response_parameters = {}
                 if response_param_headers := method_response.get("headers"):
                     for header, header_info in response_param_headers.items():
                         # TODO: make use of `header_info`
@@ -880,29 +1073,44 @@
             operation_name=method_schema.get("operationId"),
             **kwargs,
         )
 
     models = resolved_schema.get("definitions") or resolved_schema.get("components", {}).get(
         "schemas", {}
     )
-    schema_map = {}
-    for name, model in models.items():
-        # keep a map of the schema to retrieve the schema name for responseModels resolved $ref
-        schema_map[canonical_json(model)] = name
-
+    for name, model_data in models.items():
         model_id = short_uid()[:6]  # length 6 to make TF tests pass
         model = Model(
             id=model_id,
             name=name,
             contentType=APPLICATION_JSON,
-            description=None,
-            schema=json.dumps(model),
+            description=model_data.get("description"),
+            schema=json.dumps(model_data),
         )
         store.rest_apis[rest_api.id].models[name] = model
 
+    # create the RequestValidators defined at the top-level field `x-amazon-apigateway-request-validators`
+    request_validators = resolved_schema.get(OpenAPIExt.REQUEST_VALIDATORS, {})
+    request_validator_name_id_map = {}
+    for validator_name, validator_schema in request_validators.items():
+        validator_id = short_uid()[:6]
+
+        validator = RequestValidator(
+            id=validator_id,
+            name=validator_name,
+            validateRequestBody=validator_schema.get("validateRequestBody") or False,
+            validateRequestParameters=validator_schema.get("validateRequestParameters") or False,
+        )
+
+        store.rest_apis[rest_api.id].validators[validator_id] = validator
+        request_validator_name_id_map[validator_name] = validator_id
+
+    # get default requestValidator if present
+    default_req_validator_name = resolved_schema.get(OpenAPIExt.REQUEST_VALIDATOR)
+
     # create default authorizer if present
     default_authorizer = create_authorizer(resolved_schema)
 
     # determine base path
     # default basepath mode is "ignore"
     # see https://docs.aws.amazon.com/apigateway/latest/developerguide/api-gateway-import-api-basePath.html
     basepath_mode = query_params.get("basepath") or "ignore"
```

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/apigateway/integration.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/apigateway/integration.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/apigateway/invocations.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/apigateway/invocations.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import json
 import logging
 from typing import Dict
 
-from botocore.exceptions import ClientError
 from jsonschema import ValidationError, validate
 from requests.models import Response
+from werkzeug.exceptions import NotFound
 
 from localstack.aws.connect import connect_to
 from localstack.constants import APPLICATION_JSON
 from localstack.services.apigateway import helpers
 from localstack.services.apigateway.context import ApiInvocationContext
 from localstack.services.apigateway.helpers import (
     EMPTY_MODEL,
+    ModelResolver,
     extract_path_params,
     extract_query_string_params,
+    get_apigateway_store,
     get_cors_response,
     make_error_response,
 )
 from localstack.services.apigateway.integration import (
     DynamoDBIntegration,
     HTTPIntegration,
     KinesisIntegration,
@@ -25,29 +27,36 @@
     LambdaProxyIntegration,
     MockIntegration,
     S3Integration,
     SNSIntegration,
     SQSIntegration,
     StepFunctionIntegration,
 )
+from localstack.services.apigateway.models import ApiGatewayStore
 from localstack.utils.aws import aws_stack
 
 LOG = logging.getLogger(__name__)
 
 
 class AuthorizationError(Exception):
     pass
 
 
 class RequestValidator:
-    __slots__ = ["context", "apigateway_client"]
+    __slots__ = ["context", "rest_api_container"]
 
-    def __init__(self, context: ApiInvocationContext, apigateway_client):
+    def __init__(self, context: ApiInvocationContext, store: ApiGatewayStore = None):
         self.context = context
-        self.apigateway_client = apigateway_client
+        store = store or get_apigateway_store(
+            account_id=context.account_id, region=context.region_name
+        )
+        if not (container := store.rest_apis.get(context.api_id)):
+            # TODO: find the right exception
+            raise NotFound()
+        self.rest_api_container = container
 
     def is_request_valid(self) -> bool:
         # make all the positive checks first
         if self.context.resource is None or "resourceMethods" not in self.context.resource:
             return True
 
         resource_methods = self.context.resource["resourceMethods"]
@@ -56,23 +65,17 @@
 
         # check if there is validator for the resource
         resource = resource_methods[self.context.method]
         if not (resource.get("requestValidatorId") or "").strip():
             return True
 
         # check if there is a validator for this request
-        try:
-            validator = self.apigateway_client.get_request_validator(
-                restApiId=self.context.api_id, requestValidatorId=resource["requestValidatorId"]
-            )
-        except ClientError as e:
-            if "NotFoundException" in e:
-                return True
-
-            raise
+        validator = self.rest_api_container.validators.get(resource["requestValidatorId"])
+        if not validator:
+            return True
 
         # are we validating the body?
         if self.should_validate_body(validator):
             is_body_valid = self.validate_body(resource)
             if not is_body_valid:
                 return is_body_valid
 
@@ -83,38 +86,42 @@
 
         return True
 
     def validate_body(self, resource):
         # if there's no model to validate the body, use the Empty model
         # https://docs.aws.amazon.com/cdk/api/v1/docs/@aws-cdk_aws-apigateway.EmptyModel.html
         if not (request_models := resource.get("requestModels")):
-            schema_name = EMPTY_MODEL
+            model_name = EMPTY_MODEL
         else:
-            schema_name = request_models.get(APPLICATION_JSON, EMPTY_MODEL)
+            model_name = request_models.get(APPLICATION_JSON, EMPTY_MODEL)
 
-        try:
-            model = self.apigateway_client.get_model(
-                restApiId=self.context.api_id,
-                modelName=schema_name,
+        model_resolver = ModelResolver(
+            rest_api_container=self.rest_api_container,
+            model_name=model_name,
+        )
+
+        # try to get the resolved model first
+        resolved_schema = model_resolver.get_resolved_model()
+        if not resolved_schema:
+            LOG.exception(
+                "An exception occurred while trying to validate the request: could not find the model"
             )
-        except ClientError as e:
-            LOG.exception("An exception occurred while trying to validate the request: %s", e)
             return False
 
         try:
             # if the body is empty, replace it with an empty JSON body
             validate(
-                instance=json.loads(self.context.data or "{}"), schema=json.loads(model["schema"])
+                instance=json.loads(self.context.data or "{}"),
+                schema=resolved_schema,
             )
             return True
         except ValidationError as e:
             LOG.warning("failed to validate request body %s", e)
             return False
         except json.JSONDecodeError as e:
-            # TODO: for now, it could also be the loading of the schema failing but it will be validated at some point
             LOG.warning("failed to validate request body, request data is not valid JSON %s", e)
             return False
 
     # TODO implement parameters and headers
     def validate_parameters_and_headers(self, resource):
         return True
 
@@ -243,15 +250,15 @@
     authorize_invocation(invocation_context)
 
     extracted_path, resource = helpers.get_target_resource_details(invocation_context)
     if not resource:
         return make_error_response("Unable to find path %s" % invocation_context.path, 404)
 
     # validate request
-    validator = RequestValidator(invocation_context, aws_stack.connect_to_service("apigateway"))
+    validator = RequestValidator(invocation_context)
     if not validator.is_request_valid():
         return make_error_response("Invalid request body", 400)
 
     api_key_required = resource.get("resourceMethods", {}).get(method, {}).get("apiKeyRequired")
     if api_key_required and not is_api_key_valid(invocation_context):
         return make_error_response("Access denied - invalid API key", 403)
```

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/apigateway/models.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/apigateway/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,24 +28,27 @@
     validators: Dict[str, RequestValidator]
     # map DocumentationPartId -> DocumentationPart
     documentation_parts: Dict[str, DocumentationPart]
     # not used yet, still in moto
     gateway_responses: Dict[str, GatewayResponse]
     # maps Model name -> Model
     models: Dict[str, Model]
+    # maps Model name -> resolved dict Model, so we don't need to load the JSON everytime
+    resolved_models: Dict[str, dict]
     # maps ResourceId of a Resource to its children ResourceIds
     resource_children: Dict[str, List[str]]
 
     def __init__(self, rest_api: RestApi):
         self.rest_api = rest_api
         self.authorizers = {}
         self.validators = {}
         self.documentation_parts = {}
         self.gateway_responses = {}
         self.models = {}
+        self.resolved_models = {}
         self.resource_children = {}
 
 
 class ApiGatewayStore(BaseStore):
     # maps (API id) -> RestApiContainer
     # TODO: remove CaseInsensitiveDict, and lower the value of the ID when getting it from the tags
     rest_apis: Dict[str, RestApiContainer] = LocalAttribute(default=CaseInsensitiveDict)
```

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/apigateway/patches.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/apigateway/patches.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/apigateway/provider.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/apigateway/provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1578,18 +1578,21 @@
             if path not in ("/schema", "/description"):
                 raise BadRequestException(
                     f"Invalid patch path  '{path}' specified for op 'replace'. Must be one of: [/description, /schema]"
                 )
 
             key = path[1:]  # remove the leading slash
             value = operation.get("value")
-            if key == "schema" and not value:
-                raise BadRequestException(
-                    "Model schema must have at least 1 property or array items defined"
-                )
+            if key == "schema":
+                if not value:
+                    raise BadRequestException(
+                        "Model schema must have at least 1 property or array items defined"
+                    )
+                # delete the resolved model to invalidate it
+                store.rest_apis[rest_api_id].resolved_models.pop(model_name, None)
             model[key] = value
         remove_empty_attributes_from_model(model)
         return model
 
     def delete_model(
         self, context: RequestContext, rest_api_id: String, model_name: String
     ) -> None:
@@ -1601,14 +1604,15 @@
         ):
             raise NotFoundException(f"Invalid model name specified: {model_name}")
 
         moto_rest_api = get_moto_rest_api(context, rest_api_id)
         validate_model_in_use(moto_rest_api, model_name)
 
         store.rest_apis[rest_api_id].models.pop(model_name, None)
+        store.rest_apis[rest_api_id].resolved_models.pop(model_name, None)
 
 
 # ---------------
 # UTIL FUNCTIONS
 # ---------------
```

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/apigateway/router_asf.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/apigateway/router_asf.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/apigateway/templates.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/apigateway/templates.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/api_utils.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/api_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/event_source_listeners/adapters.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/event_source_listeners/adapters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/event_source_listeners/dynamodb_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/event_source_listeners/event_source_listener.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/event_source_listeners/event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/event_source_listeners/kinesis_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/event_source_listeners/sqs_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/event_source_listeners/stream_event_source_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/hooks.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/hooks.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/invocation/docker_runtime_executor.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/invocation/docker_runtime_executor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/invocation/executor_endpoint.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/invocation/executor_endpoint.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/invocation/lambda_models.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/invocation/lambda_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/invocation/lambda_service.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/invocation/lambda_service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/invocation/models.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/invocation/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/invocation/runtime_environment.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/invocation/runtime_environment.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/invocation/runtime_executor.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/invocation/runtime_executor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/invocation/version_manager.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/invocation/version_manager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/lambda_api.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/lambda_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/lambda_executors.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/lambda_executors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/lambda_models.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/lambda_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/lambda_starter.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/lambda_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/lambda_utils.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/layerfetcher/layer_fetcher.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/layerfetcher/layer_fetcher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/packages.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/plugins.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/provider.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/awslambda/urlrouter.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/awslambda/urlrouter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/api_utils.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/api_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/cfn_utils.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/cfn_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/deploy.html` & `localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/deploy.html`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/deployment_utils.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/engine/entities.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/engine/entities.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/engine/parameters.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/engine/parameters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/engine/template_deployer.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/engine/template_deployer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/engine/template_preparer.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/engine/template_preparer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/engine/transformers.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/engine/transformers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/engine/yaml_parser.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/engine/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/apigateway.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/apigateway.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/awslambda.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/awslambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/cdk.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/cdk.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/certificatemanager.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/certificatemanager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/cloudformation.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/cloudformation.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/cloudwatch.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/dynamodb.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/dynamodb.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/ec2.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/ec2.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/ecr.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/ecr.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/elasticsearch.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/events.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/events.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/iam.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/iam.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/kinesis.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/kinesis.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/kinesisfirehose.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/kinesisfirehose.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/kms.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/kms.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/logs.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/logs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/opensearch.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/opensearch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/redshift.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/redshift.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/resourcegroups.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/resourcegroups.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/route53.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/route53.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/s3.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/s3.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/secretsmanager.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/secretsmanager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/sns.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/sns.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/sqs.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/sqs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/ssm.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/ssm.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/models/stepfunctions.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/models/stepfunctions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/packages.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/provider.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/service_models.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/service_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/cloudformation/stores.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/cloudformation/stores.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/cloudwatch/alarm_scheduler.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/cloudwatch/alarm_scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/cloudwatch/provider.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/cloudwatch/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/dynamodb/models.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/dynamodb/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/dynamodb/packages.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/dynamodb/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/dynamodb/provider.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/dynamodb/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/dynamodb/server.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/dynamodb/server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/dynamodb/utils.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/dynamodb/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/dynamodbstreams/dynamodbstreams_api.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/dynamodbstreams/dynamodbstreams_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/dynamodbstreams/provider.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/dynamodbstreams/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/ec2/exceptions.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/ec2/exceptions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/ec2/models.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/ec2/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/ec2/provider.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/ec2/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/edge.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/edge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/es/provider.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/es/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/events/provider.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/events/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/events/scheduler.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/events/scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/firehose/mappers.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/firehose/mappers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/firehose/models.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/firehose/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/firehose/provider.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/firehose/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/generic_proxy.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/generic_proxy.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/iam/provider.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/iam/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/infra.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/infra.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/internal.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/internal.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/kinesis/kinesis_mock_server.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/kinesis/kinesis_mock_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/kinesis/models.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/kinesis/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/kinesis/packages.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/kinesis/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/kinesis/provider.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/kinesis/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/kms/local_kms_provider.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/kms/local_kms_provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/kms/local_kms_server.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/kms/local_kms_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/kms/models.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/kms/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/kms/packages.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/kms/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/kms/provider.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/kms/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/kms/utils.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/kms/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/logs/models.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/logs/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/logs/provider.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/logs/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/messages.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/messages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/moto.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/moto.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/motoserver.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/motoserver.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/opensearch/cluster.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/opensearch/cluster.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/opensearch/cluster_manager.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/opensearch/cluster_manager.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/opensearch/models.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/opensearch/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/opensearch/packages.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/opensearch/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/opensearch/provider.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/opensearch/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/opensearch/versions.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/opensearch/versions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/plugins.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/plugins.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/providers.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/providers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/redshift/provider.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/redshift/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/route53/provider.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/route53/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/route53resolver/models.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/route53resolver/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/route53resolver/provider.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/route53resolver/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/route53resolver/utils.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/route53resolver/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/s3/constants.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/s3/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/s3/cors.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/s3/cors.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/s3/models.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/s3/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/s3/multipart_content.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/s3/multipart_content.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/s3/notifications.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/s3/notifications.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/s3/presigned_url.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/s3/presigned_url.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/s3/provider.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/s3/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/s3/s3_listener.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/s3/s3_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/s3/s3_starter.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/s3/s3_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/s3/s3_utils.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/s3/s3_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/s3/utils.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/s3/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/s3/virtual_host.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/s3/virtual_host.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/s3/website_hosting.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/s3/website_hosting.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/secretsmanager/provider.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/secretsmanager/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/ses/provider.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/ses/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/sns/constants.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/sns/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/sns/models.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/sns/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/sns/provider.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/sns/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/sns/publisher.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/sns/publisher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/sqs/constants.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/sqs/constants.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/sqs/exceptions.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/sqs/exceptions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/sqs/models.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/sqs/models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/sqs/provider.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/sqs/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/sqs/query_api.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/sqs/query_api.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/sqs/utils.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/sqs/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/ssm/provider.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/ssm/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/antlt4utils/antlr4utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/catch/catch_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/catch/catcher_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/error_name/custom_error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/error_name/error_equals_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/error_name/error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/error_name/failure_event.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/error_name/states_error_name_type.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/parameters.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/parameters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/path/input_path.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/path/input_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/path/items_path.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/path/items_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/path/output_path.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/path/output_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/path/result_path.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/path/result_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadarr/payload_arr.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_intrinsic_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_path_context_obj.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadbinding/payload_binding_value.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/payload/payloadvalue/payloadtmpl/payload_tmpl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/result_selector.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/result_selector.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/retry/backoff_rate_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/retry/interval_seconds_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/retry/max_attempts_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/retry/retrier_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/common/retry/retry_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/eval_component.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/eval_component.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_json_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/argument/function_argument_list.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_contains.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_get_item.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_length.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_partition.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_range.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/array/array_unique.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_decode.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/encoding_decoding/base_64_encode.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/factory.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/generic/string_format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/hash_calculations/hash_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_merge.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/json_to_string.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/json_manipulation/string_to_json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_add.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/math_operations/math_random.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_array.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_format.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_json_to_string.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_string_to_json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/states_function_uuid.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/string_operations/string_split.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/function/statesfunction/unique_id_generation/uuid.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_fuinction_name_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/intrinsic/functionname/state_function_name_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/program/program.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/program/program.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_choice/choice_rule.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_composite.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_func.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_operator_type.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/comparison_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/factory.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/boolean_equals.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/is_operator.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/numeric.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/string_operators.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_choice/comparison/operator/implementations/timestamp_operators.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_choice/state_choice.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_execution/execute_state.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/itemprocessor/item_processor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_execution/state_map/state_map.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/branches_decl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_execution/state_parallel/state_parallel.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/resource.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_aws_sdk.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_lambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/service/state_task_service_sqs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_execution/state_task/state_task_lambda.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_fail/state_fail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_pass/state_pass.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_props.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_succeed/state_succeed.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_wait/state_wait.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_wait/variable.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/seconds_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/timestamp_path.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/component/state/state_wait/wait_function/wait_function.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/eval/contextobject/contex_object.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/eval/environment.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/eval/environment.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/eval/event/event_detail.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/eval/event/event_detail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/eval/event/event_history.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/eval/event/event_history.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/eval/program_worker.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/eval/program_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/eval/programstate/program_running.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/eval/programstate/program_running.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/parse/asl_parser.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/parse/asl_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/parse/intrinsic/intrinsic_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/parse/intrinsic/preprocessor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/parse/preprocessor.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/parse/preprocessor.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/asl/parse/typed_props.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/asl/parse/typed_props.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/backend/execution.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/backend/execution.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/backend/execution_worker.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/backend/execution_worker.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/backend/state_machine.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/backend/state_machine.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/backend/store.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/backend/store.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/packages.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/packages.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/provider.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/provider_v2.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/provider_v2.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/stepfunctions_starter.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/stepfunctions_starter.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stepfunctions/stepfunctions_utils.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stepfunctions/stepfunctions_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/stores.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/stores.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/sts/provider.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/sts/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/services/transcribe/provider.py` & `localstack-core-2.1.1.dev20230607163904/localstack/services/transcribe/provider.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/state/core.py` & `localstack-core-2.1.1.dev20230607163904/localstack/state/core.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/state/inspect.py` & `localstack-core-2.1.1.dev20230607163904/localstack/state/inspect.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/state/pickle.py` & `localstack-core-2.1.1.dev20230607163904/localstack/state/pickle.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/state/snapshot.py` & `localstack-core-2.1.1.dev20230607163904/localstack/state/snapshot.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/testing/aws/asf_utils.py` & `localstack-core-2.1.1.dev20230607163904/localstack/testing/aws/asf_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/testing/aws/cloudformation_utils.py` & `localstack-core-2.1.1.dev20230607163904/localstack/testing/aws/cloudformation_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/testing/aws/lambda_utils.py` & `localstack-core-2.1.1.dev20230607163904/localstack/testing/aws/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/testing/aws/util.py` & `localstack-core-2.1.1.dev20230607163904/localstack/testing/aws/util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/testing/pytest/detect_thread_leakage.py` & `localstack-core-2.1.1.dev20230607163904/localstack/testing/pytest/detect_thread_leakage.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/testing/pytest/filters.py` & `localstack-core-2.1.1.dev20230607163904/localstack/testing/pytest/filters.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/testing/pytest/find_orphaned_snapshots.py` & `localstack-core-2.1.1.dev20230607163904/localstack/testing/pytest/find_orphaned_snapshots.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/testing/pytest/fixture_conflicts.py` & `localstack-core-2.1.1.dev20230607163904/localstack/testing/pytest/fixture_conflicts.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/testing/pytest/fixtures.py` & `localstack-core-2.1.1.dev20230607163904/localstack/testing/pytest/fixtures.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/testing/pytest/metric_collection.py` & `localstack-core-2.1.1.dev20230607163904/localstack/testing/pytest/metric_collection.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/testing/pytest/snapshot.py` & `localstack-core-2.1.1.dev20230607163904/localstack/testing/pytest/snapshot.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/testing/pytest/util.py` & `localstack-core-2.1.1.dev20230607163904/localstack/testing/pytest/util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/testing/snapshots/prototype.py` & `localstack-core-2.1.1.dev20230607163904/localstack/testing/snapshots/prototype.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/testing/snapshots/report.py` & `localstack-core-2.1.1.dev20230607163904/localstack/testing/snapshots/report.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/testing/snapshots/transformer.py` & `localstack-core-2.1.1.dev20230607163904/localstack/testing/snapshots/transformer.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/testing/snapshots/transformer_utility.py` & `localstack-core-2.1.1.dev20230607163904/localstack/testing/snapshots/transformer_utility.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/analytics/cli.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/analytics/cli.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/analytics/client.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/analytics/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/analytics/events.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/analytics/events.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/analytics/logger.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/analytics/logger.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/analytics/metadata.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/analytics/metadata.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/analytics/publisher.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/analytics/publisher.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/analytics/service_request_aggregator.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/analytics/service_request_aggregator.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/analytics/usage.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/analytics/usage.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/archives.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/archives.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/asyncio.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/auth.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/auth.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/aws/arns.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/aws/arns.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/aws/aws_models.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/aws/aws_models.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/aws/aws_responses.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/aws/aws_responses.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/aws/aws_stack.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/aws/aws_stack.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/aws/client.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/aws/client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/aws/client_types.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/aws/client_types.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/aws/dead_letter_queue.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/aws/dead_letter_queue.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/aws/message_forwarding.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/aws/message_forwarding.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/aws/queries.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/aws/queries.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/aws/request_context.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/aws/request_context.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/aws/resources.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/aws/resources.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/aws/templating.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/aws/templating.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/bootstrap.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/bootstrap.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/cloudwatch/cloudwatch_util.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/cloudwatch/cloudwatch_util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/collections.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/collections.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/common.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/common.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/config_listener.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/config_listener.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/container_networking.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/container_networking.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/container_utils/container_client.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/container_utils/container_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/container_utils/docker_cmd_client.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/container_utils/docker_cmd_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/container_utils/docker_sdk_client.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/container_utils/docker_sdk_client.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/coverage_docs.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/coverage_docs.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/crypto.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/diagnose.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/diagnose.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/docker_utils.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/files.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/files.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/functions.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/functions.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/http.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/http.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/json.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/json.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/kinesis/kclipy_helper.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/kinesis/kclipy_helper.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/kinesis/kinesis_connector.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/kinesis/kinesis_connector.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/kinesis/kinesis_util.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/kinesis/kinesis_util.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/net.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/net.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/no_exit_argument_parser.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/no_exit_argument_parser.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/numbers.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/numbers.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/objects.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/objects.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/patch.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/patch.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/platform.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/platform.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/run.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/run.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/scheduler.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/server/http2_server.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/server/http2_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/server/proxy_server.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/server/proxy_server.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/serving.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/serving.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/ssl.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/ssl.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/strings.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/strings.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/sync.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/sync.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/tagging.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/tagging.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/tail.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/tail.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/testutil.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/testutil.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/threads.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/threads.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/time.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/time.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/urls.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/urls.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/venv.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/venv.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack/utils/xml.py` & `localstack-core-2.1.1.dev20230607163904/localstack/utils/xml.py`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack_core.egg-info/PKG-INFO` & `localstack-core-2.1.1.dev20230607163904/localstack_core.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack-core
-Version: 2.1.1.dev20230607022227
+Version: 2.1.1.dev20230607163904
 Summary: The core library and runtime of LocalStack
 Home-page: https://github.com/localstack/localstack
 Author: LocalStack Contributors
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack_core.egg-info/SOURCES.txt` & `localstack-core-2.1.1.dev20230607163904/localstack_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack_core.egg-info/entry_points.txt` & `localstack-core-2.1.1.dev20230607163904/localstack_core.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack_core.egg-info/plux.json` & `localstack-core-2.1.1.dev20230607163904/localstack_core.egg-info/plux.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8805555555555555%*

 * *Differences: {"'localstack.hooks.on_infra_ready'": '{insert: [(1, '*

 * *                                      "'register_virtual_host_routes=localstack.services.s3.virtual_host:register_virtual_host_routes')], "*

 * *                                      'delete: [0]}',*

 * * "'localstack.hooks.on_infra_start'": '{insert: [(0, '*

 * *                                      "'validate_configuration=localstack.services.awslambda.plugins:validate_configuration'), "*

 * *                                      '(1, '*

 * *                                   […]*

```diff
@@ -45,44 +45,44 @@
         "swf:default=localstack.services.providers:swf",
         "transcribe:default=localstack.services.providers:transcribe"
     ],
     "localstack.hooks.configure_localstack_container": [
         "configure_edge_port=localstack.plugins:configure_edge_port"
     ],
     "localstack.hooks.on_infra_ready": [
-        "register_virtual_host_routes=localstack.services.s3.virtual_host:register_virtual_host_routes",
-        "_run_init_scripts_on_ready=localstack.runtime.init:_run_init_scripts_on_ready"
+        "_run_init_scripts_on_ready=localstack.runtime.init:_run_init_scripts_on_ready",
+        "register_virtual_host_routes=localstack.services.s3.virtual_host:register_virtual_host_routes"
     ],
     "localstack.hooks.on_infra_shutdown": [
         "_run_init_scripts_on_shutdown=localstack.runtime.init:_run_init_scripts_on_shutdown",
         "run_shutdown_handlers=localstack.runtime.shutdown:run_shutdown_handlers"
     ],
     "localstack.hooks.on_infra_start": [
+        "validate_configuration=localstack.services.awslambda.plugins:validate_configuration",
+        "_run_init_scripts_on_start=localstack.runtime.init:_run_init_scripts_on_start",
         "deprecation_warnings=localstack.plugins:deprecation_warnings",
         "register_partition_adjusting_proxy_listener=localstack.plugins:register_partition_adjusting_proxy_listener",
         "_patch_botocore_json_parser=localstack.aws.client:_patch_botocore_json_parser",
         "_publish_config_as_analytics_event=localstack.runtime.analytics:_publish_config_as_analytics_event",
-        "_publish_container_info=localstack.runtime.analytics:_publish_container_info",
-        "_run_init_scripts_on_start=localstack.runtime.init:_run_init_scripts_on_start",
-        "validate_configuration=localstack.services.awslambda.plugins:validate_configuration"
+        "_publish_container_info=localstack.runtime.analytics:_publish_container_info"
     ],
     "localstack.hooks.prepare_host": [
         "prepare_host_machine_id=localstack.utils.analytics.metadata:prepare_host_machine_id"
     ],
     "localstack.lambda.runtime_executor": [
         "docker=localstack.services.awslambda.invocation.plugins:DockerRuntimeExecutorPlugin"
     ],
     "localstack.packages": [
-        "stepfunctions-local/community=localstack.services.stepfunctions.plugins:stepfunctions_local_packages",
-        "kinesis-mock/community=localstack.services.kinesis.plugins:kinesismock_package",
+        "awslambda-go-runtime/community=localstack.services.awslambda.plugins:awslambda_go_runtime_package",
+        "awslambda-runtime/community=localstack.services.awslambda.plugins:awslambda_runtime_package",
+        "lambda-java-libs/community=localstack.services.awslambda.plugins:lambda_java_libs",
+        "cloudformation-libs/community=localstack.services.cloudformation.plugins:cloudformation_package",
         "ffmpeg/community=localstack.packages.plugins:ffmpeg_package",
         "terraform/community=localstack.packages.plugins:terraform_package",
-        "local-kms/community=localstack.services.kms.plugins:local_kms_package",
-        "cloudformation-libs/community=localstack.services.cloudformation.plugins:cloudformation_package",
-        "elasticsearch/community=localstack.services.es.plugins:elasticsearch_package",
         "opensearch/community=localstack.services.opensearch.plugins:opensearch_package",
         "dynamodb-local/community=localstack.services.dynamodb.plugins:dynamodb_local_package",
-        "awslambda-go-runtime/community=localstack.services.awslambda.plugins:awslambda_go_runtime_package",
-        "awslambda-runtime/community=localstack.services.awslambda.plugins:awslambda_runtime_package",
-        "lambda-java-libs/community=localstack.services.awslambda.plugins:lambda_java_libs"
+        "elasticsearch/community=localstack.services.es.plugins:elasticsearch_package",
+        "kinesis-mock/community=localstack.services.kinesis.plugins:kinesismock_package",
+        "local-kms/community=localstack.services.kms.plugins:local_kms_package",
+        "stepfunctions-local/community=localstack.services.stepfunctions.plugins:stepfunctions_local_packages"
     ]
 }
```

### Comparing `localstack-core-2.1.1.dev20230607022227/localstack_core.egg-info/requires.txt` & `localstack-core-2.1.1.dev20230607163904/localstack_core.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/pyproject.toml` & `localstack-core-2.1.1.dev20230607163904/pyproject.toml`

 * *Files identical despite different names*

### Comparing `localstack-core-2.1.1.dev20230607022227/setup.cfg` & `localstack-core-2.1.1.dev20230607163904/setup.cfg`

 * *Files identical despite different names*

