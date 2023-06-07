# Comparing `tmp/atatus-1.5.0.tar.gz` & `tmp/atatus-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atatus-1.5.0.tar", last modified: Tue May  2 09:37:59 2023, max compression
+gzip compressed data, was "atatus-1.5.1.tar", last modified: Wed Jun  7 12:21:31 2023, max compression
```

## Comparing `atatus-1.5.0.tar` & `atatus-1.5.1.tar`

### file list

```diff
@@ -1,204 +1,204 @@
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.430778 atatus-1.5.0/
--rw-r--r--   0 apple      (501) staff       (20)     3356 2023-01-04 09:02:24.000000 atatus-1.5.0/LICENSE
--rw-r--r--   0 apple      (501) staff       (20)      110 2019-11-18 06:31:28.000000 atatus-1.5.0/MANIFEST.in
--rw-r--r--   0 apple      (501) staff       (20)     2489 2023-05-02 09:37:59.430956 atatus-1.5.0/PKG-INFO
--rw-r--r--   0 apple      (501) staff       (20)      991 2023-01-04 09:26:05.000000 atatus-1.5.0/README.rst
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.402470 atatus-1.5.0/atatus/
--rw-r--r--   0 apple      (501) staff       (20)     2826 2022-12-16 06:48:10.000000 atatus-1.5.0/atatus/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)    30577 2023-01-03 09:24:18.000000 atatus-1.5.0/atatus/base.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.404796 atatus-1.5.0/atatus/collector/
--rw-r--r--   0 apple      (501) staff       (20)        0 2022-12-16 06:48:10.000000 atatus-1.5.0/atatus/collector/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)    25451 2023-04-26 05:49:01.000000 atatus-1.5.0/atatus/collector/base.py
--rw-r--r--   0 apple      (501) staff       (20)    20628 2023-01-03 09:24:18.000000 atatus-1.5.0/atatus/collector/builder.py
--rw-r--r--   0 apple      (501) staff       (20)     1211 2022-12-16 06:48:10.000000 atatus-1.5.0/atatus/collector/hist.py
--rw-r--r--   0 apple      (501) staff       (20)     1195 2022-12-16 06:48:10.000000 atatus-1.5.0/atatus/collector/layer.py
--rw-r--r--   0 apple      (501) staff       (20)     6418 2023-04-29 10:18:47.000000 atatus-1.5.0/atatus/collector/transport.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.405555 atatus-1.5.0/atatus/conf/
--rw-r--r--   0 apple      (501) staff       (20)    35250 2023-04-26 05:49:01.000000 atatus-1.5.0/atatus/conf/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     3840 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/conf/constants.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.406246 atatus-1.5.0/atatus/context/
--rw-r--r--   0 apple      (501) staff       (20)     2619 2019-11-18 10:56:33.000000 atatus-1.5.0/atatus/context/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     2757 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/context/base.py
--rw-r--r--   0 apple      (501) staff       (20)     3638 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/context/contextvars.py
--rw-r--r--   0 apple      (501) staff       (20)     3617 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/context/threadlocal.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.406506 atatus-1.5.0/atatus/contrib/
--rw-r--r--   0 apple      (501) staff       (20)     1591 2019-11-18 06:31:28.000000 atatus-1.5.0/atatus/contrib/__init__.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.407072 atatus-1.5.0/atatus/contrib/aiohttp/
--rw-r--r--   0 apple      (501) staff       (20)     2321 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/aiohttp/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     5835 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/aiohttp/middleware.py
--rw-r--r--   0 apple      (501) staff       (20)     2639 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/aiohttp/utils.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.407476 atatus-1.5.0/atatus/contrib/asyncio/
--rw-r--r--   0 apple      (501) staff       (20)     1591 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/asyncio/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     3322 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/asyncio/traces.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.407619 atatus-1.5.0/atatus/contrib/celery/
--rw-r--r--   0 apple      (501) staff       (20)     5694 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/celery/__init__.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.409134 atatus-1.5.0/atatus/contrib/django/
--rw-r--r--   0 apple      (501) staff       (20)     1789 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/django/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     7863 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/django/apps.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.409411 atatus-1.5.0/atatus/contrib/django/celery/
--rw-r--r--   0 apple      (501) staff       (20)     1588 2019-11-18 06:31:28.000000 atatus-1.5.0/atatus/contrib/django/celery/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     1862 2019-11-18 06:31:28.000000 atatus-1.5.0/atatus/contrib/django/celery/models.py
--rw-r--r--   0 apple      (501) staff       (20)    14034 2023-04-26 05:49:01.000000 atatus-1.5.0/atatus/contrib/django/client.py
--rw-r--r--   0 apple      (501) staff       (20)     2240 2019-11-18 10:56:34.000000 atatus-1.5.0/atatus/contrib/django/context_processors.py
--rw-r--r--   0 apple      (501) staff       (20)     3384 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/django/handlers.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.409549 atatus-1.5.0/atatus/contrib/django/management/
--rw-r--r--   0 apple      (501) staff       (20)     1591 2019-11-18 06:31:28.000000 atatus-1.5.0/atatus/contrib/django/management/__init__.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.409841 atatus-1.5.0/atatus/contrib/django/management/commands/
--rw-r--r--   0 apple      (501) staff       (20)     1519 2019-11-18 06:31:28.000000 atatus-1.5.0/atatus/contrib/django/management/commands/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)    13737 2023-01-03 09:24:18.000000 atatus-1.5.0/atatus/contrib/django/management/commands/atatus.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.410341 atatus-1.5.0/atatus/contrib/django/middleware/
--rw-r--r--   0 apple      (501) staff       (20)     9184 2023-01-03 09:24:18.000000 atatus-1.5.0/atatus/contrib/django/middleware/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     2262 2019-11-18 11:24:33.000000 atatus-1.5.0/atatus/contrib/django/middleware/wsgi.py
--rw-r--r--   0 apple      (501) staff       (20)     4446 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/django/utils.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.410751 atatus-1.5.0/atatus/contrib/flask/
--rw-r--r--   0 apple      (501) staff       (20)     8515 2022-12-16 06:48:10.000000 atatus-1.5.0/atatus/contrib/flask/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     3602 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/flask/utils.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.411627 atatus-1.5.0/atatus/contrib/opentelemetry/
--rw-r--r--   0 apple      (501) staff       (20)     1644 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/opentelemetry/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     5592 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/opentelemetry/context.py
--rw-r--r--   0 apple      (501) staff       (20)    12843 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/opentelemetry/span.py
--rw-r--r--   0 apple      (501) staff       (20)    13216 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/opentelemetry/trace.py
--rw-r--r--   0 apple      (501) staff       (20)     3035 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/opentelemetry/utils.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.412007 atatus-1.5.0/atatus/contrib/opentracing/
--rw-r--r--   0 apple      (501) staff       (20)     1886 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/opentracing/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     5778 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/opentracing/span.py
--rw-r--r--   0 apple      (501) staff       (20)     6210 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/opentracing/tracer.py
--rw-r--r--   0 apple      (501) staff       (20)     1818 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/paste.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.412289 atatus-1.5.0/atatus/contrib/pylons/
--rw-r--r--   0 apple      (501) staff       (20)     2134 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/pylons/__init__.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.412433 atatus-1.5.0/atatus/contrib/rq/
--rw-r--r--   0 apple      (501) staff       (20)     2378 2019-11-18 11:25:11.000000 atatus-1.5.0/atatus/contrib/rq/__init__.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.412964 atatus-1.5.0/atatus/contrib/sanic/
--rw-r--r--   0 apple      (501) staff       (20)    15842 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/sanic/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     4270 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/sanic/patch.py
--rw-r--r--   0 apple      (501) staff       (20)     2745 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/sanic/sanic_types.py
--rw-r--r--   0 apple      (501) staff       (20)     6081 2022-12-16 06:48:10.000000 atatus-1.5.0/atatus/contrib/sanic/utils.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.413442 atatus-1.5.0/atatus/contrib/serverless/
--rw-r--r--   0 apple      (501) staff       (20)     1975 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/serverless/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)    20636 2023-01-03 09:24:18.000000 atatus-1.5.0/atatus/contrib/serverless/aws.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.413868 atatus-1.5.0/atatus/contrib/starlette/
--rw-r--r--   0 apple      (501) staff       (20)    10726 2022-12-22 14:08:57.000000 atatus-1.5.0/atatus/contrib/starlette/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     4863 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/starlette/utils.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.414230 atatus-1.5.0/atatus/contrib/tornado/
--rw-r--r--   0 apple      (501) staff       (20)     3049 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/tornado/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     3371 2022-12-16 06:48:10.000000 atatus-1.5.0/atatus/contrib/tornado/utils.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.414350 atatus-1.5.0/atatus/contrib/twisted/
--rw-r--r--   0 apple      (501) staff       (20)     2449 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/contrib/twisted/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     8231 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/events.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.415094 atatus-1.5.0/atatus/handlers/
--rw-r--r--   0 apple      (501) staff       (20)     1588 2019-11-18 06:31:28.000000 atatus-1.5.0/atatus/handlers/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     4247 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/handlers/logbook.py
--rw-r--r--   0 apple      (501) staff       (20)    10219 2023-01-03 09:24:18.000000 atatus-1.5.0/atatus/handlers/logging.py
--rw-r--r--   0 apple      (501) staff       (20)     2582 2023-01-03 09:24:18.000000 atatus-1.5.0/atatus/handlers/structlog.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.415481 atatus-1.5.0/atatus/instrumentation/
--rw-r--r--   0 apple      (501) staff       (20)     1591 2019-11-18 06:31:28.000000 atatus-1.5.0/atatus/instrumentation/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     2119 2019-11-18 10:56:35.000000 atatus-1.5.0/atatus/instrumentation/control.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.420640 atatus-1.5.0/atatus/instrumentation/packages/
--rw-r--r--   0 apple      (501) staff       (20)     1591 2019-11-18 06:31:28.000000 atatus-1.5.0/atatus/instrumentation/packages/__init__.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.422640 atatus-1.5.0/atatus/instrumentation/packages/asyncio/
--rw-r--r--   0 apple      (501) staff       (20)     1591 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/asyncio/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     2699 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/asyncio/aiobotocore.py
--rw-r--r--   0 apple      (501) staff       (20)     4496 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/asyncio/aiohttp_client.py
--rw-r--r--   0 apple      (501) staff       (20)     3031 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/asyncio/aiomysql.py
--rw-r--r--   0 apple      (501) staff       (20)     3189 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/asyncio/aiopg.py
--rw-r--r--   0 apple      (501) staff       (20)     4624 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/asyncio/aioredis.py
--rw-r--r--   0 apple      (501) staff       (20)     3755 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/asyncio/asyncpg.py
--rw-r--r--   0 apple      (501) staff       (20)     1848 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/asyncio/base.py
--rw-r--r--   0 apple      (501) staff       (20)     4330 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/asyncio/elasticsearch.py
--rw-r--r--   0 apple      (501) staff       (20)     2124 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/asyncio/sleep.py
--rw-r--r--   0 apple      (501) staff       (20)    18215 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/azure.py
--rw-r--r--   0 apple      (501) staff       (20)    11063 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/base.py
--rw-r--r--   0 apple      (501) staff       (20)    10984 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/botocore.py
--rw-r--r--   0 apple      (501) staff       (20)     4167 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/cassandra.py
--rw-r--r--   0 apple      (501) staff       (20)    10031 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/dbapi2.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.422943 atatus-1.5.0/atatus/instrumentation/packages/django/
--rw-r--r--   0 apple      (501) staff       (20)     1591 2019-11-18 06:31:28.000000 atatus-1.5.0/atatus/instrumentation/packages/django/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     2918 2019-11-18 10:56:35.000000 atatus-1.5.0/atatus/instrumentation/packages/django/template.py
--rw-r--r--   0 apple      (501) staff       (20)     7414 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/elasticsearch.py
--rw-r--r--   0 apple      (501) staff       (20)     4443 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/graphql.py
--rw-r--r--   0 apple      (501) staff       (20)     5496 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/httplib2.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.423271 atatus-1.5.0/atatus/instrumentation/packages/httpx/
--rw-r--r--   0 apple      (501) staff       (20)     1591 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/httpx/__init__.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.423739 atatus-1.5.0/atatus/instrumentation/packages/httpx/async/
--rw-r--r--   0 apple      (501) staff       (20)     1591 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/httpx/async/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     5028 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/httpx/async/httpcore.py
--rw-r--r--   0 apple      (501) staff       (20)     2823 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/httpx/async/httpx.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.424166 atatus-1.5.0/atatus/instrumentation/packages/httpx/sync/
--rw-r--r--   0 apple      (501) staff       (20)     1591 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/httpx/sync/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     4586 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/httpx/sync/httpcore.py
--rw-r--r--   0 apple      (501) staff       (20)     2749 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/httpx/sync/httpx.py
--rw-r--r--   0 apple      (501) staff       (20)     3674 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/httpx/utils.py
--rw-r--r--   0 apple      (501) staff       (20)     2115 2019-11-18 10:56:35.000000 atatus-1.5.0/atatus/instrumentation/packages/jinja2.py
--rw-r--r--   0 apple      (501) staff       (20)     8759 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/kafka.py
--rw-r--r--   0 apple      (501) staff       (20)     2758 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/mysql.py
--rw-r--r--   0 apple      (501) staff       (20)     2822 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/mysql_connector.py
--rw-r--r--   0 apple      (501) staff       (20)     6121 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/psycopg2.py
--rw-r--r--   0 apple      (501) staff       (20)     3499 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/pylibmc.py
--rw-r--r--   0 apple      (501) staff       (20)     4126 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/pymemcache.py
--rw-r--r--   0 apple      (501) staff       (20)     6227 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/pymongo.py
--rw-r--r--   0 apple      (501) staff       (20)     3154 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/pymssql.py
--rw-r--r--   0 apple      (501) staff       (20)     2368 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/pymysql.py
--rw-r--r--   0 apple      (501) staff       (20)     2359 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/pyodbc.py
--rw-r--r--   0 apple      (501) staff       (20)     3235 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/python_memcached.py
--rw-r--r--   0 apple      (501) staff       (20)     4626 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/redis.py
--rw-r--r--   0 apple      (501) staff       (20)     7001 2023-04-26 05:49:01.000000 atatus-1.5.0/atatus/instrumentation/packages/requests.py
--rw-r--r--   0 apple      (501) staff       (20)     3438 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/sqlite.py
--rw-r--r--   0 apple      (501) staff       (20)     6342 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/tornado.py
--rw-r--r--   0 apple      (501) staff       (20)     5309 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/urllib.py
--rw-r--r--   0 apple      (501) staff       (20)     6363 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/packages/urllib3.py
--rw-r--r--   0 apple      (501) staff       (20)     2097 2019-11-18 10:56:36.000000 atatus-1.5.0/atatus/instrumentation/packages/zlib.py
--rw-r--r--   0 apple      (501) staff       (20)     6211 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/instrumentation/register.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.424431 atatus-1.5.0/atatus/metrics/
--rw-r--r--   0 apple      (501) staff       (20)     1591 2019-11-18 06:31:28.000000 atatus-1.5.0/atatus/metrics/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)    18424 2022-12-22 14:08:57.000000 atatus-1.5.0/atatus/metrics/base_metrics.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.425285 atatus-1.5.0/atatus/metrics/sets/
--rw-r--r--   0 apple      (501) staff       (20)     1591 2019-11-18 06:31:28.000000 atatus-1.5.0/atatus/metrics/sets/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     1748 2019-11-18 10:56:36.000000 atatus-1.5.0/atatus/metrics/sets/breakdown.py
--rw-r--r--   0 apple      (501) staff       (20)     1857 2019-11-18 11:11:54.000000 atatus-1.5.0/atatus/metrics/sets/cpu.py
--rw-r--r--   0 apple      (501) staff       (20)    11809 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/metrics/sets/cpu_linux.py
--rw-r--r--   0 apple      (501) staff       (20)     2898 2019-11-18 10:56:36.000000 atatus-1.5.0/atatus/metrics/sets/cpu_psutil.py
--rw-r--r--   0 apple      (501) staff       (20)     5450 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/metrics/sets/prometheus.py
--rw-r--r--   0 apple      (501) staff       (20)     2920 2019-11-18 11:25:40.000000 atatus-1.5.0/atatus/middleware.py
--rw-r--r--   0 apple      (501) staff       (20)    14144 2022-12-16 06:48:10.000000 atatus-1.5.0/atatus/processors.py
--rw-r--r--   0 apple      (501) staff       (20)    51580 2022-12-22 05:27:27.000000 atatus-1.5.0/atatus/traces.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.426456 atatus-1.5.0/atatus/transport/
--rw-r--r--   0 apple      (501) staff       (20)     1615 2019-11-18 06:31:28.000000 atatus-1.5.0/atatus/transport/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)    17353 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/transport/base.py
--rw-r--r--   0 apple      (501) staff       (20)     1840 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/transport/exceptions.py
--rw-r--r--   0 apple      (501) staff       (20)    10167 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/transport/http.py
--rw-r--r--   0 apple      (501) staff       (20)     3906 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/transport/http_base.py
--rw-r--r--   0 apple      (501) staff       (20)     1900 2019-11-18 10:56:37.000000 atatus-1.5.0/atatus/transport/http_urllib3.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.428973 atatus-1.5.0/atatus/utils/
--rw-r--r--   0 apple      (501) staff       (20)     7689 2023-04-26 05:49:01.000000 atatus-1.5.0/atatus/utils/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     4432 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/utils/cgroup.py
--rw-r--r--   0 apple      (501) staff       (20)     7562 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/utils/cloud.py
--rw-r--r--   0 apple      (501) staff       (20)     3705 2023-04-29 11:08:46.000000 atatus-1.5.0/atatus/utils/compat.py
--rw-r--r--   0 apple      (501) staff       (20)     2536 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/utils/deprecation.py
--rw-r--r--   0 apple      (501) staff       (20)    12347 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/utils/disttracing.py
--rw-r--r--   0 apple      (501) staff       (20)    10629 2023-01-03 09:24:18.000000 atatus-1.5.0/atatus/utils/encoding.py
--rw-r--r--   0 apple      (501) staff       (20)     4207 2022-12-16 06:48:10.000000 atatus-1.5.0/atatus/utils/hw_info.py
--rw-r--r--   0 apple      (501) staff       (20)     2520 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/utils/json_encoder.py
--rw-r--r--   0 apple      (501) staff       (20)     2024 2019-11-18 11:12:02.000000 atatus-1.5.0/atatus/utils/logging.py
--rw-r--r--   0 apple      (501) staff       (20)     2348 2019-11-18 06:31:28.000000 atatus-1.5.0/atatus/utils/module_import.py
--rw-r--r--   0 apple      (501) staff       (20)    13225 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/utils/stacks.py
--rw-r--r--   0 apple      (501) staff       (20)     4476 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/utils/threading.py
--rw-r--r--   0 apple      (501) staff       (20)     3756 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/utils/time.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.430556 atatus-1.5.0/atatus/utils/wrapt/
--rw-r--r--   0 apple      (501) staff       (20)      699 2019-11-18 06:31:28.000000 atatus-1.5.0/atatus/utils/wrapt/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)    81870 2019-11-18 06:31:28.000000 atatus-1.5.0/atatus/utils/wrapt/_wrappers.c
--rw-r--r--   0 apple      (501) staff       (20)     4059 2019-11-18 06:31:28.000000 atatus-1.5.0/atatus/utils/wrapt/arguments.py
--rw-r--r--   0 apple      (501) staff       (20)    20127 2019-11-18 06:31:28.000000 atatus-1.5.0/atatus/utils/wrapt/decorators.py
--rw-r--r--   0 apple      (501) staff       (20)     7726 2019-11-18 06:31:28.000000 atatus-1.5.0/atatus/utils/wrapt/importer.py
--rw-r--r--   0 apple      (501) staff       (20)    32389 2019-11-18 06:31:28.000000 atatus-1.5.0/atatus/utils/wrapt/wrappers.py
--rw-r--r--   0 apple      (501) staff       (20)     4927 2022-12-15 12:32:13.000000 atatus-1.5.0/atatus/utils/wsgi.py
--rw-r--r--   0 apple      (501) staff       (20)     1658 2023-04-26 05:50:12.000000 atatus-1.5.0/atatus/version.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-05-02 09:37:59.403534 atatus-1.5.0/atatus.egg-info/
--rw-r--r--   0 apple      (501) staff       (20)     2489 2023-05-02 09:37:59.000000 atatus-1.5.0/atatus.egg-info/PKG-INFO
--rw-r--r--   0 apple      (501) staff       (20)     5743 2023-05-02 09:37:59.000000 atatus-1.5.0/atatus.egg-info/SOURCES.txt
--rw-r--r--   0 apple      (501) staff       (20)        1 2023-05-02 09:37:59.000000 atatus-1.5.0/atatus.egg-info/dependency_links.txt
--rw-r--r--   0 apple      (501) staff       (20)        1 2019-11-18 11:35:56.000000 atatus-1.5.0/atatus.egg-info/not-zip-safe
--rw-r--r--   0 apple      (501) staff       (20)      205 2023-05-02 09:37:59.000000 atatus-1.5.0/atatus.egg-info/requires.txt
--rw-r--r--   0 apple      (501) staff       (20)        7 2023-05-02 09:37:59.000000 atatus-1.5.0/atatus.egg-info/top_level.txt
--rw-r--r--   0 apple      (501) staff       (20)      239 2019-11-18 10:56:32.000000 atatus-1.5.0/pyproject.toml
--rw-r--r--   0 apple      (501) staff       (20)     3524 2023-05-02 09:37:59.431549 atatus-1.5.0/setup.cfg
--rw-r--r--   0 apple      (501) staff       (20)     5656 2023-01-04 09:02:24.000000 atatus-1.5.0/setup.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 12:21:31.624058 atatus-1.5.1/
+-rw-r--r--   0 apple      (501) staff       (20)     3356 2023-01-04 09:02:24.000000 atatus-1.5.1/LICENSE
+-rw-r--r--   0 apple      (501) staff       (20)      110 2019-11-18 06:31:28.000000 atatus-1.5.1/MANIFEST.in
+-rw-r--r--   0 apple      (501) staff       (20)     2489 2023-06-07 12:21:31.624160 atatus-1.5.1/PKG-INFO
+-rw-r--r--   0 apple      (501) staff       (20)      991 2023-01-04 09:26:05.000000 atatus-1.5.1/README.rst
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 12:21:31.608430 atatus-1.5.1/atatus/
+-rw-r--r--   0 apple      (501) staff       (20)     2826 2022-12-16 06:48:10.000000 atatus-1.5.1/atatus/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)    30577 2023-01-03 09:24:18.000000 atatus-1.5.1/atatus/base.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 12:21:31.609648 atatus-1.5.1/atatus/collector/
+-rw-r--r--   0 apple      (501) staff       (20)        0 2022-12-16 06:48:10.000000 atatus-1.5.1/atatus/collector/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)    27411 2023-06-07 09:35:43.000000 atatus-1.5.1/atatus/collector/base.py
+-rw-r--r--   0 apple      (501) staff       (20)    20628 2023-01-03 09:24:18.000000 atatus-1.5.1/atatus/collector/builder.py
+-rw-r--r--   0 apple      (501) staff       (20)     1211 2022-12-16 06:48:10.000000 atatus-1.5.1/atatus/collector/hist.py
+-rw-r--r--   0 apple      (501) staff       (20)     1195 2022-12-16 06:48:10.000000 atatus-1.5.1/atatus/collector/layer.py
+-rw-r--r--   0 apple      (501) staff       (20)     6418 2023-04-29 10:18:47.000000 atatus-1.5.1/atatus/collector/transport.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 12:21:31.609871 atatus-1.5.1/atatus/conf/
+-rw-r--r--   0 apple      (501) staff       (20)    35440 2023-06-07 07:23:32.000000 atatus-1.5.1/atatus/conf/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     3840 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/conf/constants.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 12:21:31.610258 atatus-1.5.1/atatus/context/
+-rw-r--r--   0 apple      (501) staff       (20)     2619 2019-11-18 10:56:33.000000 atatus-1.5.1/atatus/context/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     2757 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/context/base.py
+-rw-r--r--   0 apple      (501) staff       (20)     3638 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/context/contextvars.py
+-rw-r--r--   0 apple      (501) staff       (20)     3617 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/context/threadlocal.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 12:21:31.610459 atatus-1.5.1/atatus/contrib/
+-rw-r--r--   0 apple      (501) staff       (20)     1591 2019-11-18 06:31:28.000000 atatus-1.5.1/atatus/contrib/__init__.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 12:21:31.610779 atatus-1.5.1/atatus/contrib/aiohttp/
+-rw-r--r--   0 apple      (501) staff       (20)     2321 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/contrib/aiohttp/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     5835 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/contrib/aiohttp/middleware.py
+-rw-r--r--   0 apple      (501) staff       (20)     2639 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/contrib/aiohttp/utils.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 12:21:31.611141 atatus-1.5.1/atatus/contrib/asyncio/
+-rw-r--r--   0 apple      (501) staff       (20)     1591 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/contrib/asyncio/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     3322 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/contrib/asyncio/traces.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 12:21:31.611239 atatus-1.5.1/atatus/contrib/celery/
+-rw-r--r--   0 apple      (501) staff       (20)     5694 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/contrib/celery/__init__.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 12:21:31.611822 atatus-1.5.1/atatus/contrib/django/
+-rw-r--r--   0 apple      (501) staff       (20)     1789 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/contrib/django/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     7863 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/contrib/django/apps.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 12:21:31.612026 atatus-1.5.1/atatus/contrib/django/celery/
+-rw-r--r--   0 apple      (501) staff       (20)     1588 2019-11-18 06:31:28.000000 atatus-1.5.1/atatus/contrib/django/celery/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     1862 2019-11-18 06:31:28.000000 atatus-1.5.1/atatus/contrib/django/celery/models.py
+-rw-r--r--   0 apple      (501) staff       (20)    13285 2023-06-07 07:23:32.000000 atatus-1.5.1/atatus/contrib/django/client.py
+-rw-r--r--   0 apple      (501) staff       (20)     2240 2019-11-18 10:56:34.000000 atatus-1.5.1/atatus/contrib/django/context_processors.py
+-rw-r--r--   0 apple      (501) staff       (20)     3384 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/contrib/django/handlers.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 12:21:31.612127 atatus-1.5.1/atatus/contrib/django/management/
+-rw-r--r--   0 apple      (501) staff       (20)     1591 2019-11-18 06:31:28.000000 atatus-1.5.1/atatus/contrib/django/management/__init__.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 12:21:31.612335 atatus-1.5.1/atatus/contrib/django/management/commands/
+-rw-r--r--   0 apple      (501) staff       (20)     1519 2019-11-18 06:31:28.000000 atatus-1.5.1/atatus/contrib/django/management/commands/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)    13737 2023-01-03 09:24:18.000000 atatus-1.5.1/atatus/contrib/django/management/commands/atatus.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 12:21:31.612538 atatus-1.5.1/atatus/contrib/django/middleware/
+-rw-r--r--   0 apple      (501) staff       (20)     9342 2023-06-07 07:23:32.000000 atatus-1.5.1/atatus/contrib/django/middleware/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     2262 2019-11-18 11:24:33.000000 atatus-1.5.1/atatus/contrib/django/middleware/wsgi.py
+-rw-r--r--   0 apple      (501) staff       (20)     4446 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/contrib/django/utils.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 12:21:31.612730 atatus-1.5.1/atatus/contrib/flask/
+-rw-r--r--   0 apple      (501) staff       (20)     8515 2022-12-16 06:48:10.000000 atatus-1.5.1/atatus/contrib/flask/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     4998 2023-06-07 07:23:32.000000 atatus-1.5.1/atatus/contrib/flask/utils.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 12:21:31.613224 atatus-1.5.1/atatus/contrib/opentelemetry/
+-rw-r--r--   0 apple      (501) staff       (20)     1644 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/contrib/opentelemetry/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     5592 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/contrib/opentelemetry/context.py
+-rw-r--r--   0 apple      (501) staff       (20)    12843 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/contrib/opentelemetry/span.py
+-rw-r--r--   0 apple      (501) staff       (20)    13216 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/contrib/opentelemetry/trace.py
+-rw-r--r--   0 apple      (501) staff       (20)     3035 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/contrib/opentelemetry/utils.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 12:21:31.613537 atatus-1.5.1/atatus/contrib/opentracing/
+-rw-r--r--   0 apple      (501) staff       (20)     1886 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/contrib/opentracing/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     5778 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/contrib/opentracing/span.py
+-rw-r--r--   0 apple      (501) staff       (20)     6210 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/contrib/opentracing/tracer.py
+-rw-r--r--   0 apple      (501) staff       (20)     1818 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/contrib/paste.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 12:21:31.613633 atatus-1.5.1/atatus/contrib/pylons/
+-rw-r--r--   0 apple      (501) staff       (20)     2134 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/contrib/pylons/__init__.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 12:21:31.613734 atatus-1.5.1/atatus/contrib/rq/
+-rw-r--r--   0 apple      (501) staff       (20)     2378 2019-11-18 11:25:11.000000 atatus-1.5.1/atatus/contrib/rq/__init__.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 12:21:31.614163 atatus-1.5.1/atatus/contrib/sanic/
+-rw-r--r--   0 apple      (501) staff       (20)    15842 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/contrib/sanic/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     4270 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/contrib/sanic/patch.py
+-rw-r--r--   0 apple      (501) staff       (20)     2745 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/contrib/sanic/sanic_types.py
+-rw-r--r--   0 apple      (501) staff       (20)     6081 2022-12-16 06:48:10.000000 atatus-1.5.1/atatus/contrib/sanic/utils.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 12:21:31.614392 atatus-1.5.1/atatus/contrib/serverless/
+-rw-r--r--   0 apple      (501) staff       (20)     1975 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/contrib/serverless/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)    20636 2023-01-03 09:24:18.000000 atatus-1.5.1/atatus/contrib/serverless/aws.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 12:21:31.614625 atatus-1.5.1/atatus/contrib/starlette/
+-rw-r--r--   0 apple      (501) staff       (20)    10726 2022-12-22 14:08:57.000000 atatus-1.5.1/atatus/contrib/starlette/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     4863 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/contrib/starlette/utils.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 12:21:31.614811 atatus-1.5.1/atatus/contrib/tornado/
+-rw-r--r--   0 apple      (501) staff       (20)     3049 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/contrib/tornado/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     3371 2022-12-16 06:48:10.000000 atatus-1.5.1/atatus/contrib/tornado/utils.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 12:21:31.614910 atatus-1.5.1/atatus/contrib/twisted/
+-rw-r--r--   0 apple      (501) staff       (20)     2449 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/contrib/twisted/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     8231 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/events.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 12:21:31.615291 atatus-1.5.1/atatus/handlers/
+-rw-r--r--   0 apple      (501) staff       (20)     1588 2019-11-18 06:31:28.000000 atatus-1.5.1/atatus/handlers/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     4247 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/handlers/logbook.py
+-rw-r--r--   0 apple      (501) staff       (20)    10219 2023-01-03 09:24:18.000000 atatus-1.5.1/atatus/handlers/logging.py
+-rw-r--r--   0 apple      (501) staff       (20)     2582 2023-01-03 09:24:18.000000 atatus-1.5.1/atatus/handlers/structlog.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 12:21:31.615615 atatus-1.5.1/atatus/instrumentation/
+-rw-r--r--   0 apple      (501) staff       (20)     1591 2019-11-18 06:31:28.000000 atatus-1.5.1/atatus/instrumentation/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     2119 2019-11-18 10:56:35.000000 atatus-1.5.1/atatus/instrumentation/control.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 12:21:31.618402 atatus-1.5.1/atatus/instrumentation/packages/
+-rw-r--r--   0 apple      (501) staff       (20)     1591 2019-11-18 06:31:28.000000 atatus-1.5.1/atatus/instrumentation/packages/__init__.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 12:21:31.619403 atatus-1.5.1/atatus/instrumentation/packages/asyncio/
+-rw-r--r--   0 apple      (501) staff       (20)     1591 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/instrumentation/packages/asyncio/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     2699 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/instrumentation/packages/asyncio/aiobotocore.py
+-rw-r--r--   0 apple      (501) staff       (20)     4496 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/instrumentation/packages/asyncio/aiohttp_client.py
+-rw-r--r--   0 apple      (501) staff       (20)     3031 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/instrumentation/packages/asyncio/aiomysql.py
+-rw-r--r--   0 apple      (501) staff       (20)     3189 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/instrumentation/packages/asyncio/aiopg.py
+-rw-r--r--   0 apple      (501) staff       (20)     4624 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/instrumentation/packages/asyncio/aioredis.py
+-rw-r--r--   0 apple      (501) staff       (20)     3755 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/instrumentation/packages/asyncio/asyncpg.py
+-rw-r--r--   0 apple      (501) staff       (20)     1848 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/instrumentation/packages/asyncio/base.py
+-rw-r--r--   0 apple      (501) staff       (20)     4330 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/instrumentation/packages/asyncio/elasticsearch.py
+-rw-r--r--   0 apple      (501) staff       (20)     2124 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/instrumentation/packages/asyncio/sleep.py
+-rw-r--r--   0 apple      (501) staff       (20)    18215 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/instrumentation/packages/azure.py
+-rw-r--r--   0 apple      (501) staff       (20)    11063 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/instrumentation/packages/base.py
+-rw-r--r--   0 apple      (501) staff       (20)    10984 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/instrumentation/packages/botocore.py
+-rw-r--r--   0 apple      (501) staff       (20)     4167 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/instrumentation/packages/cassandra.py
+-rw-r--r--   0 apple      (501) staff       (20)    10031 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/instrumentation/packages/dbapi2.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 12:21:31.619614 atatus-1.5.1/atatus/instrumentation/packages/django/
+-rw-r--r--   0 apple      (501) staff       (20)     1591 2019-11-18 06:31:28.000000 atatus-1.5.1/atatus/instrumentation/packages/django/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     2918 2019-11-18 10:56:35.000000 atatus-1.5.1/atatus/instrumentation/packages/django/template.py
+-rw-r--r--   0 apple      (501) staff       (20)     7414 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/instrumentation/packages/elasticsearch.py
+-rw-r--r--   0 apple      (501) staff       (20)     4443 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/instrumentation/packages/graphql.py
+-rw-r--r--   0 apple      (501) staff       (20)     5496 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/instrumentation/packages/httplib2.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 12:21:31.619810 atatus-1.5.1/atatus/instrumentation/packages/httpx/
+-rw-r--r--   0 apple      (501) staff       (20)     1591 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/instrumentation/packages/httpx/__init__.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 12:21:31.620116 atatus-1.5.1/atatus/instrumentation/packages/httpx/async/
+-rw-r--r--   0 apple      (501) staff       (20)     1591 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/instrumentation/packages/httpx/async/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     5028 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/instrumentation/packages/httpx/async/httpcore.py
+-rw-r--r--   0 apple      (501) staff       (20)     2823 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/instrumentation/packages/httpx/async/httpx.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 12:21:31.620404 atatus-1.5.1/atatus/instrumentation/packages/httpx/sync/
+-rw-r--r--   0 apple      (501) staff       (20)     1591 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/instrumentation/packages/httpx/sync/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     4586 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/instrumentation/packages/httpx/sync/httpcore.py
+-rw-r--r--   0 apple      (501) staff       (20)     2749 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/instrumentation/packages/httpx/sync/httpx.py
+-rw-r--r--   0 apple      (501) staff       (20)     3674 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/instrumentation/packages/httpx/utils.py
+-rw-r--r--   0 apple      (501) staff       (20)     2115 2019-11-18 10:56:35.000000 atatus-1.5.1/atatus/instrumentation/packages/jinja2.py
+-rw-r--r--   0 apple      (501) staff       (20)     8759 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/instrumentation/packages/kafka.py
+-rw-r--r--   0 apple      (501) staff       (20)     2758 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/instrumentation/packages/mysql.py
+-rw-r--r--   0 apple      (501) staff       (20)     2822 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/instrumentation/packages/mysql_connector.py
+-rw-r--r--   0 apple      (501) staff       (20)     6121 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/instrumentation/packages/psycopg2.py
+-rw-r--r--   0 apple      (501) staff       (20)     3499 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/instrumentation/packages/pylibmc.py
+-rw-r--r--   0 apple      (501) staff       (20)     4126 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/instrumentation/packages/pymemcache.py
+-rw-r--r--   0 apple      (501) staff       (20)     6227 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/instrumentation/packages/pymongo.py
+-rw-r--r--   0 apple      (501) staff       (20)     3154 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/instrumentation/packages/pymssql.py
+-rw-r--r--   0 apple      (501) staff       (20)     2368 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/instrumentation/packages/pymysql.py
+-rw-r--r--   0 apple      (501) staff       (20)     2359 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/instrumentation/packages/pyodbc.py
+-rw-r--r--   0 apple      (501) staff       (20)     3235 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/instrumentation/packages/python_memcached.py
+-rw-r--r--   0 apple      (501) staff       (20)     4626 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/instrumentation/packages/redis.py
+-rw-r--r--   0 apple      (501) staff       (20)     7001 2023-04-26 05:49:01.000000 atatus-1.5.1/atatus/instrumentation/packages/requests.py
+-rw-r--r--   0 apple      (501) staff       (20)     3438 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/instrumentation/packages/sqlite.py
+-rw-r--r--   0 apple      (501) staff       (20)     6342 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/instrumentation/packages/tornado.py
+-rw-r--r--   0 apple      (501) staff       (20)     5309 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/instrumentation/packages/urllib.py
+-rw-r--r--   0 apple      (501) staff       (20)     6363 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/instrumentation/packages/urllib3.py
+-rw-r--r--   0 apple      (501) staff       (20)     2097 2019-11-18 10:56:36.000000 atatus-1.5.1/atatus/instrumentation/packages/zlib.py
+-rw-r--r--   0 apple      (501) staff       (20)     6211 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/instrumentation/register.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 12:21:31.620599 atatus-1.5.1/atatus/metrics/
+-rw-r--r--   0 apple      (501) staff       (20)     1591 2019-11-18 06:31:28.000000 atatus-1.5.1/atatus/metrics/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)    18424 2022-12-22 14:08:57.000000 atatus-1.5.1/atatus/metrics/base_metrics.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 12:21:31.621202 atatus-1.5.1/atatus/metrics/sets/
+-rw-r--r--   0 apple      (501) staff       (20)     1591 2019-11-18 06:31:28.000000 atatus-1.5.1/atatus/metrics/sets/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     1748 2019-11-18 10:56:36.000000 atatus-1.5.1/atatus/metrics/sets/breakdown.py
+-rw-r--r--   0 apple      (501) staff       (20)     1857 2019-11-18 11:11:54.000000 atatus-1.5.1/atatus/metrics/sets/cpu.py
+-rw-r--r--   0 apple      (501) staff       (20)    11809 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/metrics/sets/cpu_linux.py
+-rw-r--r--   0 apple      (501) staff       (20)     2898 2019-11-18 10:56:36.000000 atatus-1.5.1/atatus/metrics/sets/cpu_psutil.py
+-rw-r--r--   0 apple      (501) staff       (20)     5450 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/metrics/sets/prometheus.py
+-rw-r--r--   0 apple      (501) staff       (20)     2920 2019-11-18 11:25:40.000000 atatus-1.5.1/atatus/middleware.py
+-rw-r--r--   0 apple      (501) staff       (20)    14144 2022-12-16 06:48:10.000000 atatus-1.5.1/atatus/processors.py
+-rw-r--r--   0 apple      (501) staff       (20)    51580 2022-12-22 05:27:27.000000 atatus-1.5.1/atatus/traces.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 12:21:31.621799 atatus-1.5.1/atatus/transport/
+-rw-r--r--   0 apple      (501) staff       (20)     1615 2019-11-18 06:31:28.000000 atatus-1.5.1/atatus/transport/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)    17353 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/transport/base.py
+-rw-r--r--   0 apple      (501) staff       (20)     1840 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/transport/exceptions.py
+-rw-r--r--   0 apple      (501) staff       (20)    10167 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/transport/http.py
+-rw-r--r--   0 apple      (501) staff       (20)     3906 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/transport/http_base.py
+-rw-r--r--   0 apple      (501) staff       (20)     1900 2019-11-18 10:56:37.000000 atatus-1.5.1/atatus/transport/http_urllib3.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 12:21:31.623264 atatus-1.5.1/atatus/utils/
+-rw-r--r--   0 apple      (501) staff       (20)     7689 2023-04-26 05:49:01.000000 atatus-1.5.1/atatus/utils/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     4432 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/utils/cgroup.py
+-rw-r--r--   0 apple      (501) staff       (20)     7562 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/utils/cloud.py
+-rw-r--r--   0 apple      (501) staff       (20)     3705 2023-04-29 11:08:46.000000 atatus-1.5.1/atatus/utils/compat.py
+-rw-r--r--   0 apple      (501) staff       (20)     2536 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/utils/deprecation.py
+-rw-r--r--   0 apple      (501) staff       (20)    12347 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/utils/disttracing.py
+-rw-r--r--   0 apple      (501) staff       (20)    11290 2023-06-07 07:23:32.000000 atatus-1.5.1/atatus/utils/encoding.py
+-rw-r--r--   0 apple      (501) staff       (20)     4207 2022-12-16 06:48:10.000000 atatus-1.5.1/atatus/utils/hw_info.py
+-rw-r--r--   0 apple      (501) staff       (20)     2520 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/utils/json_encoder.py
+-rw-r--r--   0 apple      (501) staff       (20)     2024 2019-11-18 11:12:02.000000 atatus-1.5.1/atatus/utils/logging.py
+-rw-r--r--   0 apple      (501) staff       (20)     2348 2019-11-18 06:31:28.000000 atatus-1.5.1/atatus/utils/module_import.py
+-rw-r--r--   0 apple      (501) staff       (20)    13225 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/utils/stacks.py
+-rw-r--r--   0 apple      (501) staff       (20)     4476 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/utils/threading.py
+-rw-r--r--   0 apple      (501) staff       (20)     3756 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/utils/time.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 12:21:31.623937 atatus-1.5.1/atatus/utils/wrapt/
+-rw-r--r--   0 apple      (501) staff       (20)      699 2019-11-18 06:31:28.000000 atatus-1.5.1/atatus/utils/wrapt/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)    81870 2019-11-18 06:31:28.000000 atatus-1.5.1/atatus/utils/wrapt/_wrappers.c
+-rw-r--r--   0 apple      (501) staff       (20)     4059 2019-11-18 06:31:28.000000 atatus-1.5.1/atatus/utils/wrapt/arguments.py
+-rw-r--r--   0 apple      (501) staff       (20)    20127 2019-11-18 06:31:28.000000 atatus-1.5.1/atatus/utils/wrapt/decorators.py
+-rw-r--r--   0 apple      (501) staff       (20)     7726 2019-11-18 06:31:28.000000 atatus-1.5.1/atatus/utils/wrapt/importer.py
+-rw-r--r--   0 apple      (501) staff       (20)    32389 2019-11-18 06:31:28.000000 atatus-1.5.1/atatus/utils/wrapt/wrappers.py
+-rw-r--r--   0 apple      (501) staff       (20)     4927 2022-12-15 12:32:13.000000 atatus-1.5.1/atatus/utils/wsgi.py
+-rw-r--r--   0 apple      (501) staff       (20)     1658 2023-06-07 07:24:00.000000 atatus-1.5.1/atatus/version.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 12:21:31.609034 atatus-1.5.1/atatus.egg-info/
+-rw-r--r--   0 apple      (501) staff       (20)     2489 2023-06-07 12:21:31.000000 atatus-1.5.1/atatus.egg-info/PKG-INFO
+-rw-r--r--   0 apple      (501) staff       (20)     5743 2023-06-07 12:21:31.000000 atatus-1.5.1/atatus.egg-info/SOURCES.txt
+-rw-r--r--   0 apple      (501) staff       (20)        1 2023-06-07 12:21:31.000000 atatus-1.5.1/atatus.egg-info/dependency_links.txt
+-rw-r--r--   0 apple      (501) staff       (20)        1 2019-11-18 11:35:56.000000 atatus-1.5.1/atatus.egg-info/not-zip-safe
+-rw-r--r--   0 apple      (501) staff       (20)      205 2023-06-07 12:21:31.000000 atatus-1.5.1/atatus.egg-info/requires.txt
+-rw-r--r--   0 apple      (501) staff       (20)        7 2023-06-07 12:21:31.000000 atatus-1.5.1/atatus.egg-info/top_level.txt
+-rw-r--r--   0 apple      (501) staff       (20)      239 2019-11-18 10:56:32.000000 atatus-1.5.1/pyproject.toml
+-rw-r--r--   0 apple      (501) staff       (20)     3524 2023-06-07 12:21:31.624680 atatus-1.5.1/setup.cfg
+-rw-r--r--   0 apple      (501) staff       (20)     5656 2023-01-04 09:02:24.000000 atatus-1.5.1/setup.py
```

### Comparing `atatus-1.5.0/LICENSE` & `atatus-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/PKG-INFO` & `atatus-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atatus
-Version: 1.5.0
+Version: 1.5.1
 Summary: Atatus Python Agent
 Home-page: https://www.atatus.com/for/python
 Author: Atatus
 License: Atatus License
 Project-URL: Documentation, https://docs.atatus.com/docs/application-monitoring/python-agent/overview.html
 Project-URL: Release notes, https://docs.atatus.com/docs/release-notes/python.html
 Description: Atatus APM agent for Python
```

### Comparing `atatus-1.5.0/README.rst` & `atatus-1.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/__init__.py` & `atatus-1.5.1/atatus/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/base.py` & `atatus-1.5.1/atatus/base.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/collector/base.py` & `atatus-1.5.1/atatus/collector/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -357,17 +357,37 @@
         if "context" in txn and \
             "company" in txn["context"]:
 
             if "id" in txn["context"]["company"]:
                 analytics_txn["companyId"] = str(txn["context"]["company"]["id"])
 
         analytics_txn["body_len"] = requestBodyLen + responseBodyLen
+        analytics_txn["direction"] = "incoming"
         with self._analytics_lock:
-             if len(self._analytics_agg) < 10000:
-                self._analytics_agg.append(analytics_txn)
+            if len(self._analytics_agg) < 10000:
+                skip_event = False
+
+                if self._config.skip_event_processor is not None:
+                    try:
+                        skip_event = self._config.skip_event_processor(analytics_txn)
+                    except Exception as e:
+                        self._error_logger.debug("skip function failed with exception: %r" % e)
+                        pass
+
+                if skip_event == False:
+                    if self._config.mask_event_processor is not None:
+                        try:
+                            self._config.mask_event_processor(analytics_txn)
+                        except Exception as e:
+                            self._error_logger.debug("mask function failed with exception: %r" % e)
+                            pass
+                    self._analytics_agg.append(analytics_txn)
+                else:
+                    if "name" in analytics_txn:
+                        self._error_logger.debug("skipping analytics event: %r" % analytics_txn["name"])
 
     def add_analytics_outgoing(self, txn, span):
         analytics_txn = {}
 
         if not all(k in txn for k in ("name", "id", "timestamp", "duration")):
             return
 
@@ -454,15 +474,33 @@
             if "id" in txn["context"]["company"]:
                 analytics_txn["companyId"] = str(txn["context"]["company"]["id"])
 
         analytics_txn["body_len"] = requestBodyLen + responseBodyLen
         analytics_txn["direction"] = "outgoing"
         with self._analytics_lock:
              if len(self._analytics_agg) < 10000:
-                self._analytics_agg.append(analytics_txn)
+                skip_event = False
+                if self._config.skip_event_processor is not None:
+                    try:
+                        skip_event = self._config.skip_event_processor(analytics_txn)
+                    except Exception as e:
+                        self._error_logger.debug("skip function failed with exception: %r" % e)
+                        pass
+
+                if skip_event == False:
+                    if self._config.mask_event_processor is not None:
+                        try:
+                            self._config.mask_event_processor(analytics_txn)
+                        except Exception as e:
+                            self._error_logger.debug("mask function failed with exception: %r" % e)
+                            pass
+                    self._analytics_agg.append(analytics_txn)
+                else:
+                    if "name" in analytics_txn:
+                        self._error_logger.debug("skipping analytics event: %r" % analytics_txn["name"])
 
     def add_span(self, span):
 
         if not all(k in span for k in ("transaction_id", "name", "type", "subtype", "duration")):
             return
 
         span_id = span["transaction_id"]
```

### Comparing `atatus-1.5.0/atatus/collector/builder.py` & `atatus-1.5.1/atatus/collector/builder.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/collector/hist.py` & `atatus-1.5.1/atatus/collector/hist.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/collector/layer.py` & `atatus-1.5.1/atatus/collector/layer.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/collector/transport.py` & `atatus-1.5.1/atatus/collector/transport.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/conf/__init__.py` & `atatus-1.5.1/atatus/conf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -596,14 +596,16 @@
         default=[
             "atatus.processors.sanitize_http_request_cookies_analytics",
             "atatus.processors.sanitize_http_response_cookies_analytics",
             "atatus.processors.sanitize_http_headers_analytics",
             "atatus.processors.sanitize_http_request_body_analytics",
         ],
     )
+    skip_event_processor = _ConfigValue("SKIP_EVENT", type=None, default=None, required=False)
+    mask_event_processor = _ConfigValue("MASK_EVENT", type=None, default=None, required=False)
     sanitize_field_names = _ListConfigValue(
         "SANITIZE_FIELD_NAMES", type=starmatch_to_regex, default=BASE_SANITIZE_FIELD_NAMES
     )
     metrics_sets = _ListConfigValue(
         "METRICS_SETS",
         default=[
             "atatus.metrics.sets.cpu.CPUMetricSet",
```

### Comparing `atatus-1.5.0/atatus/conf/constants.py` & `atatus-1.5.1/atatus/conf/constants.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/context/__init__.py` & `atatus-1.5.1/atatus/context/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/context/base.py` & `atatus-1.5.1/atatus/context/base.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/context/contextvars.py` & `atatus-1.5.1/atatus/context/contextvars.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/context/threadlocal.py` & `atatus-1.5.1/atatus/context/threadlocal.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/contrib/__init__.py` & `atatus-1.5.1/atatus/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/contrib/aiohttp/__init__.py` & `atatus-1.5.1/atatus/contrib/aiohttp/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/contrib/aiohttp/middleware.py` & `atatus-1.5.1/atatus/contrib/aiohttp/middleware.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/contrib/aiohttp/utils.py` & `atatus-1.5.1/atatus/contrib/aiohttp/utils.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/contrib/asyncio/__init__.py` & `atatus-1.5.1/atatus/contrib/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/contrib/asyncio/traces.py` & `atatus-1.5.1/atatus/contrib/asyncio/traces.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/contrib/celery/__init__.py` & `atatus-1.5.1/atatus/contrib/celery/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/contrib/django/__init__.py` & `atatus-1.5.1/atatus/contrib/django/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/contrib/django/apps.py` & `atatus-1.5.1/atatus/contrib/django/apps.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/contrib/django/celery/__init__.py` & `atatus-1.5.1/atatus/contrib/django/celery/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/contrib/django/celery/models.py` & `atatus-1.5.1/atatus/contrib/django/celery/models.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/contrib/django/client.py` & `atatus-1.5.1/atatus/contrib/django/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,17 +47,14 @@
 from atatus.contrib.django.utils import get_raw_uri, iterate_with_template_sources
 from atatus.utils import compat, encoding, get_url_dict
 from atatus.utils.encoding import long_field
 from atatus.utils.logging import get_logger
 from atatus.utils.module_import import import_string
 from atatus.utils.wsgi import get_environ, get_headers
 
-import gzip
-import base64
-
 __all__ = ("DjangoClient",)
 
 
 default_client_class = "atatus.contrib.django.DjangoClient"
 
 
 def get_client():
@@ -142,18 +139,18 @@
                 content_type = request.META.get("CONTENT_TYPE")
                 if content_type and content_type.startswith("multipart/form-data"):
                     data = compat.multidict_to_dict(request.POST)
                     if request.FILES:
                         data["_files"] = {field: file.name for field, file in request.FILES.items()}
                 else:
                     try:
-                        if isinstance(request.body, bytes):
-                            data = self.body_decode(request.body)
+                        if isinstance(request._atatus_body, bytes):
+                            data = encoding.body_decode(request._atatus_body)
                         else:
-                            data = request.body
+                            data = request._atatus_body
                     except Exception as e:
                         self.logger.debug("Can't capture request body: %s", str(e))
                         data = "<unavailable>"
                 if data is not None:
                     # Can we apply this as a processor instead?
                     # https://github.com/elastic/apm-agent-python/issues/305
                     result["body"] = long_field(data)
@@ -161,40 +158,15 @@
         url = get_raw_uri(request)
         try:
             result["url"] = get_url_dict(url)
         except ValueError as exc:
             self.logger.warning(f"URL parsing failed: {exc}")
         return result
 
-    def body_decode(self, body):
-        if isinstance(body, bytes):
-            try:
-                string_data = body.decode('UTF-8')
-                return string_data
-            except:
-                pass
-        return body
-
-    def body_bytes(self, body, content_encoding):
-        try:
-            if content_encoding == "gzip":
-                parsed_body = gzip.decompress(body)
-                return parsed_body
-        except:
-            pass
-        return body
 
-    def body_string(self, body, content_encoding):
-        try:
-            if content_encoding == "gzip":
-                decompressed_body = gzip.GzipFile(fileobj=StringIO(body)).read()
-                return decompressed_body
-        except:
-            pass
-        return body
 
     def get_data_from_response(self, response, event_type):
         result = {"status_code": response.status_code}
 
         if self.config.capture_headers and hasattr(response, "items"):
             response_headers = dict(response.items())
 
@@ -217,19 +189,19 @@
             if captureContent is True:
                 content_encoding = ""
                 if "headers" in result and "Content-Encoding" in result["headers"] and result["headers"]["Content-Encoding"] is not None and "gzip" in (result["headers"]["Content-Encoding"]).lower():
                     content_encoding = "gzip"
 
                 body = None
                 if isinstance(response.content, str):
-                    body = self.body_string(response.content, content_encoding)
+                    body = encoding.body_string(response.content, content_encoding)
                 else:
-                    body = self.body_bytes(response.content, content_encoding)
+                    body = encoding.body_bytes(response.content, content_encoding)
                 if body is not None:
-                    decoded_body = self.body_decode(body)
+                    decoded_body = encoding.body_decode(body)
                     result["body"] = encoding.body_field(str(decoded_body))
 
 
         return result
 
     def capture(self, event_type, request=None, **kwargs):
         if "context" not in kwargs:
```

### Comparing `atatus-1.5.0/atatus/contrib/django/context_processors.py` & `atatus-1.5.1/atatus/contrib/django/context_processors.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/contrib/django/handlers.py` & `atatus-1.5.1/atatus/contrib/django/handlers.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/contrib/django/management/__init__.py` & `atatus-1.5.1/atatus/contrib/django/management/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/contrib/django/management/commands/__init__.py` & `atatus-1.5.1/atatus/contrib/django/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/contrib/django/management/commands/atatus.py` & `atatus-1.5.1/atatus/contrib/django/management/commands/atatus.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/contrib/django/middleware/__init__.py` & `atatus-1.5.1/atatus/contrib/django/middleware/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,14 +158,20 @@
                     if hasattr(middleware_class, "process_request"):
                         wrapt.wrap_function_wrapper(middleware_class, "process_request", process_request_wrapper)
                     if hasattr(middleware_class, "process_response"):
                         wrapt.wrap_function_wrapper(middleware_class, "process_response", process_response_wrapper)
                 except ImportError:
                     client.logger.warning("Can't instrument middleware %s", middleware_path)
 
+    def process_request(self, request):
+        try:
+            request._atatus_body = request.body
+        except:
+            request._atatus_body = None
+
     def process_view(self, request: HttpRequest, view_func: FunctionType, view_args: list, view_kwargs: dict):
         atatus.set_transaction_name(self.get_transaction_name(request, view_func), override=False)
         request._atatus_name_set = True
 
     def process_response(self, request: HttpRequest, response: HttpResponse):
         if django_settings.DEBUG and not self.client.config.debug:
             return response
```

### Comparing `atatus-1.5.0/atatus/contrib/django/middleware/wsgi.py` & `atatus-1.5.1/atatus/contrib/django/middleware/wsgi.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/contrib/django/utils.py` & `atatus-1.5.1/atatus/contrib/django/utils.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/contrib/flask/__init__.py` & `atatus-1.5.1/atatus/contrib/flask/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/contrib/flask/utils.py` & `atatus-1.5.1/atatus/contrib/tornado/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -23,62 +23,58 @@
 #  DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 #  FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 #  DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 #  SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 #  CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 #  OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 #  OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
-
-from werkzeug.exceptions import ClientDisconnected
-
+import atatus
 from atatus.conf import constants
-from atatus.utils import compat, get_url_dict
-from atatus.utils.wsgi import get_environ, get_headers
+
+try:
+    import tornado
+except ImportError:
+    pass
 
 
-def get_data_from_request(request, config, event_type):
+def get_data_from_request(request_handler, request, config, event_type):
+    """
+    Capture relevant data from a tornado.httputil.HTTPServerRequest
+    """
     result = {
-        "env": dict(get_environ(request.environ)),
         "method": request.method,
-        "socket": {"remote_address": request.environ.get("REMOTE_ADDR")},
+        "socket": {"remote_address": request.remote_ip},
         "cookies": request.cookies,
+        "http_version": request.version,
     }
     if config.capture_headers:
-        result["headers"] = dict(get_headers(request.environ))
+        result["headers"] = dict(request.headers)
     if request.method in constants.HTTP_WITH_BODY:
-        if config.capture_body not in ("all", event_type):
-            result["body"] = "[REDACTED]"
+        if tornado.web._has_stream_request_body(request_handler.__class__):
+            # Body is a future and streaming is expected to be handled by
+            # the user in the RequestHandler.data_received function.
+            # Currently not sure of a safe way to get the body in this case.
+            result["body"] = "[STREAMING]" if config.capture_body in ("all", "request") else "[REDACTED]"
         else:
             body = None
-            if request.content_type == "application/x-www-form-urlencoded":
-                body = compat.multidict_to_dict(request.form)
-            elif request.content_type and request.content_type.startswith("multipart/form-data"):
-                body = compat.multidict_to_dict(request.form)
-                if request.files:
-                    body["_files"] = {
-                        field: val[0].filename if len(val) == 1 else [f.filename for f in val]
-                        for field, val in request.files.lists()
-                    }
-            else:
-                try:
-                    body = request.get_data(as_text=True)
-                except ClientDisconnected:
-                    pass
+            try:
+                body = tornado.escape.json_decode(request.body)
+            except Exception:
+                body = str(request.body, errors="ignore")
 
             if body is not None:
-                result["body"] = body
+                result["body"] = body if config.capture_body in ("all", "request") else "[REDACTED]"
 
-    result["url"] = get_url_dict(request.url)
+    result["url"] = atatus.utils.get_url_dict(request.full_url())
     return result
 
 
-def get_data_from_response(response, config, event_type):
+def get_data_from_response(request_handler, config, event_type):
     result = {}
 
-    if isinstance(getattr(response, "status_code", None), int):
-        result["status_code"] = response.status_code
+    result["status_code"] = request_handler.get_status()
 
-    if config.capture_headers and getattr(response, "headers", None):
-        headers = response.headers
-        result["headers"] = {key: ";".join(headers.getlist(key)) for key in headers.keys()}
+    if config.capture_headers and request_handler._headers:
+        headers = request_handler._headers
+        result["headers"] = {key: ";".join(headers.get_list(key)) for key in headers.keys()}
+        pass
     return result
```

### Comparing `atatus-1.5.0/atatus/contrib/opentelemetry/__init__.py` & `atatus-1.5.1/atatus/contrib/opentelemetry/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/contrib/opentelemetry/context.py` & `atatus-1.5.1/atatus/contrib/opentelemetry/context.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/contrib/opentelemetry/span.py` & `atatus-1.5.1/atatus/contrib/opentelemetry/span.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/contrib/opentelemetry/trace.py` & `atatus-1.5.1/atatus/contrib/opentelemetry/trace.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/contrib/opentelemetry/utils.py` & `atatus-1.5.1/atatus/contrib/opentelemetry/utils.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/contrib/opentracing/__init__.py` & `atatus-1.5.1/atatus/contrib/opentracing/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/contrib/opentracing/span.py` & `atatus-1.5.1/atatus/contrib/opentracing/span.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/contrib/opentracing/tracer.py` & `atatus-1.5.1/atatus/contrib/opentracing/tracer.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/contrib/paste.py` & `atatus-1.5.1/atatus/contrib/paste.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/contrib/pylons/__init__.py` & `atatus-1.5.1/atatus/contrib/pylons/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/contrib/rq/__init__.py` & `atatus-1.5.1/atatus/contrib/rq/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/contrib/sanic/__init__.py` & `atatus-1.5.1/atatus/contrib/sanic/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/contrib/sanic/patch.py` & `atatus-1.5.1/atatus/contrib/sanic/patch.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/contrib/sanic/sanic_types.py` & `atatus-1.5.1/atatus/contrib/sanic/sanic_types.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/contrib/sanic/utils.py` & `atatus-1.5.1/atatus/contrib/sanic/utils.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/contrib/serverless/__init__.py` & `atatus-1.5.1/atatus/contrib/serverless/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/contrib/serverless/aws.py` & `atatus-1.5.1/atatus/contrib/serverless/aws.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/contrib/starlette/__init__.py` & `atatus-1.5.1/atatus/contrib/starlette/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/contrib/starlette/utils.py` & `atatus-1.5.1/atatus/contrib/starlette/utils.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/contrib/tornado/__init__.py` & `atatus-1.5.1/atatus/contrib/tornado/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/contrib/tornado/utils.py` & `atatus-1.5.1/atatus/instrumentation/packages/httpx/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #  BSD 3-Clause License
 #
-#  Copyright (c) 2019, Elasticsearch BV
+#  Copyright (c) 2021, Elasticsearch BV
 #  All rights reserved.
 #
 #  Redistribution and use in source and binary forms, with or without
 #  modification, are permitted provided that the following conditions are met:
 #
 #  * Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
@@ -23,58 +23,64 @@
 #  DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 #  FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 #  DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 #  SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 #  CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 #  OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 #  OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-import atatus
-from atatus.conf import constants
-
-try:
-    import tornado
-except ImportError:
-    pass
-
-
-def get_data_from_request(request_handler, request, config, event_type):
-    """
-    Capture relevant data from a tornado.httputil.HTTPServerRequest
-    """
-    result = {
-        "method": request.method,
-        "socket": {"remote_address": request.remote_ip},
-        "cookies": request.cookies,
-        "http_version": request.version,
-    }
-    if config.capture_headers:
-        result["headers"] = dict(request.headers)
-    if request.method in constants.HTTP_WITH_BODY:
-        if tornado.web._has_stream_request_body(request_handler.__class__):
-            # Body is a future and streaming is expected to be handled by
-            # the user in the RequestHandler.data_received function.
-            # Currently not sure of a safe way to get the body in this case.
-            result["body"] = "[STREAMING]" if config.capture_body in ("all", "request") else "[REDACTED]"
-        else:
-            body = None
-            try:
-                body = tornado.escape.json_decode(request.body)
-            except Exception:
-                body = str(request.body, errors="ignore")
+from typing import Tuple
 
-            if body is not None:
-                result["body"] = body if config.capture_body in ("all", "request") else "[REDACTED]"
+from atatus.conf import constants
 
-    result["url"] = atatus.utils.get_url_dict(request.full_url())
-    return result
 
+def get_request_data(args, kwargs) -> Tuple[Tuple[str, str, int, str], str, list]:
+    if len(args) == 1 and hasattr(args[0], "method"):
+        # httpcore >= 0.14
+        request = args[0]
+        method = request.method.decode("utf-8")
+        headers = request.headers
+        url = (
+            request.url.scheme.decode("utf-8"),
+            request.url.host.decode("utf-8"),
+            request.url.port,
+            request.url.target.decode("utf-8"),
+        )
+    else:
+        if "method" in kwargs:
+            method = kwargs["method"].decode("utf-8")
+        else:
+            method = args[0].decode("utf-8")
 
-def get_data_from_response(request_handler, config, event_type):
-    result = {}
+        # URL is a tuple of (scheme, host, port, path)
+        if "url" in kwargs:
+            url = kwargs["url"]
+        else:
+            url = args[1]
+        url = (url[0].decode("utf-8"), url[1].decode("utf-8"), url[2], url[3].decode("utf-8"))
+        if "headers" in kwargs:
+            headers = kwargs["headers"]
+        else:
+            headers = []
+    return url, method, headers
 
-    result["status_code"] = request_handler.get_status()
 
-    if config.capture_headers and request_handler._headers:
-        headers = request_handler._headers
-        result["headers"] = {key: ";".join(headers.get_list(key)) for key in headers.keys()}
-        pass
-    return result
+def get_status(response) -> int:
+    if hasattr(response, "status"):  # httpcore >= 0.14
+        status_code = response.status
+    elif len(response) > 4:
+        # httpcore < 0.11.0
+        # response = (http_version, status_code, reason_phrase, headers, stream)
+        status_code = response[1]
+    else:
+        # httpcore >= 0.11.0
+        # response = (status_code, headers, stream, ext)
+        status_code = response[0]
+    return status_code
+
+
+def set_disttracing_headers(headers, trace_parent, transaction):
+    trace_parent_str = trace_parent.to_string()
+    headers.append((bytes(constants.TRACEPARENT_HEADER_NAME, "utf-8"), bytes(trace_parent_str, "utf-8")))
+    if transaction.tracer.config.use_atatus_traceparent_header:
+        headers.append((bytes(constants.TRACEPARENT_LEGACY_HEADER_NAME, "utf-8"), bytes(trace_parent_str, "utf-8")))
+    if trace_parent.tracestate:
+        headers.append((bytes(constants.TRACESTATE_HEADER_NAME, "utf-8"), bytes(trace_parent.tracestate, "utf-8")))
```

### Comparing `atatus-1.5.0/atatus/contrib/twisted/__init__.py` & `atatus-1.5.1/atatus/contrib/twisted/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/events.py` & `atatus-1.5.1/atatus/events.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/handlers/__init__.py` & `atatus-1.5.1/atatus/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/handlers/logbook.py` & `atatus-1.5.1/atatus/handlers/logbook.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/handlers/logging.py` & `atatus-1.5.1/atatus/handlers/logging.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/handlers/structlog.py` & `atatus-1.5.1/atatus/handlers/structlog.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/__init__.py` & `atatus-1.5.1/atatus/instrumentation/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/control.py` & `atatus-1.5.1/atatus/instrumentation/control.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/packages/__init__.py` & `atatus-1.5.1/atatus/instrumentation/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/packages/asyncio/__init__.py` & `atatus-1.5.1/atatus/instrumentation/packages/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/packages/asyncio/aiobotocore.py` & `atatus-1.5.1/atatus/instrumentation/packages/asyncio/aiobotocore.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/packages/asyncio/aiohttp_client.py` & `atatus-1.5.1/atatus/instrumentation/packages/asyncio/aiohttp_client.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/packages/asyncio/aiomysql.py` & `atatus-1.5.1/atatus/instrumentation/packages/asyncio/aiomysql.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/packages/asyncio/aiopg.py` & `atatus-1.5.1/atatus/instrumentation/packages/asyncio/aiopg.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/packages/asyncio/aioredis.py` & `atatus-1.5.1/atatus/instrumentation/packages/asyncio/aioredis.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/packages/asyncio/asyncpg.py` & `atatus-1.5.1/atatus/instrumentation/packages/asyncio/asyncpg.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/packages/asyncio/base.py` & `atatus-1.5.1/atatus/instrumentation/packages/asyncio/base.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/packages/asyncio/elasticsearch.py` & `atatus-1.5.1/atatus/instrumentation/packages/asyncio/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/packages/asyncio/sleep.py` & `atatus-1.5.1/atatus/instrumentation/packages/asyncio/sleep.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/packages/azure.py` & `atatus-1.5.1/atatus/instrumentation/packages/azure.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/packages/base.py` & `atatus-1.5.1/atatus/instrumentation/packages/base.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/packages/botocore.py` & `atatus-1.5.1/atatus/instrumentation/packages/botocore.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/packages/cassandra.py` & `atatus-1.5.1/atatus/instrumentation/packages/cassandra.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/packages/dbapi2.py` & `atatus-1.5.1/atatus/instrumentation/packages/dbapi2.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/packages/django/__init__.py` & `atatus-1.5.1/atatus/instrumentation/packages/django/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/packages/django/template.py` & `atatus-1.5.1/atatus/instrumentation/packages/django/template.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/packages/elasticsearch.py` & `atatus-1.5.1/atatus/instrumentation/packages/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/packages/graphql.py` & `atatus-1.5.1/atatus/instrumentation/packages/graphql.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/packages/httplib2.py` & `atatus-1.5.1/atatus/instrumentation/packages/httplib2.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/packages/httpx/__init__.py` & `atatus-1.5.1/atatus/instrumentation/packages/httpx/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/packages/httpx/async/__init__.py` & `atatus-1.5.1/atatus/instrumentation/packages/httpx/async/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/packages/httpx/async/httpcore.py` & `atatus-1.5.1/atatus/instrumentation/packages/httpx/async/httpcore.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/packages/httpx/async/httpx.py` & `atatus-1.5.1/atatus/instrumentation/packages/httpx/async/httpx.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/packages/httpx/sync/__init__.py` & `atatus-1.5.1/atatus/instrumentation/packages/httpx/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/packages/httpx/sync/httpcore.py` & `atatus-1.5.1/atatus/instrumentation/packages/httpx/sync/httpcore.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/packages/httpx/sync/httpx.py` & `atatus-1.5.1/atatus/instrumentation/packages/httpx/sync/httpx.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/packages/httpx/utils.py` & `atatus-1.5.1/atatus/utils/compat.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+# -*- coding: utf-8 -*-
+
 #  BSD 3-Clause License
 #
-#  Copyright (c) 2021, Elasticsearch BV
+#  Copyright (c) 2019, Elasticsearch BV
 #  All rights reserved.
 #
 #  Redistribution and use in source and binary forms, with or without
 #  modification, are permitted provided that the following conditions are met:
 #
 #  * Redistributions of source code must retain the above copyright notice, this
 #    list of conditions and the following disclaimer.
@@ -23,64 +25,92 @@
 #  DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
 #  FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 #  DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 #  SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 #  CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 #  OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 #  OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-from typing import Tuple
 
-from atatus.conf import constants
+import sys
+import atexit
+import functools
+import platform
 
 
-def get_request_data(args, kwargs) -> Tuple[Tuple[str, str, int, str], str, list]:
-    if len(args) == 1 and hasattr(args[0], "method"):
-        # httpcore >= 0.14
-        request = args[0]
-        method = request.method.decode("utf-8")
-        headers = request.headers
-        url = (
-            request.url.scheme.decode("utf-8"),
-            request.url.host.decode("utf-8"),
-            request.url.port,
-            request.url.target.decode("utf-8"),
-        )
-    else:
-        if "method" in kwargs:
-            method = kwargs["method"].decode("utf-8")
-        else:
-            method = args[0].decode("utf-8")
+PY3 = sys.version_info[0] == 3
 
-        # URL is a tuple of (scheme, host, port, path)
-        if "url" in kwargs:
-            url = kwargs["url"]
-        else:
-            url = args[1]
-        url = (url[0].decode("utf-8"), url[1].decode("utf-8"), url[2], url[3].decode("utf-8"))
-        if "headers" in kwargs:
-            headers = kwargs["headers"]
-        else:
-            headers = []
-    return url, method, headers
+def noop_decorator(func):
+    @functools.wraps(func)
+    def wrapped(*args, **kwargs):
+        return func(*args, **kwargs)
+
+    return wrapped
+
+
+def atexit_register(func):
+    """
+    Uses either uwsgi's atexit mechanism, or atexit from the stdlib.
 
+    When running under uwsgi, using their atexit handler is more reliable,
+    especially when using gevent
+    :param func: the function to call at exit
+    """
+    try:
+        import uwsgi
 
-def get_status(response) -> int:
-    if hasattr(response, "status"):  # httpcore >= 0.14
-        status_code = response.status
-    elif len(response) > 4:
-        # httpcore < 0.11.0
-        # response = (http_version, status_code, reason_phrase, headers, stream)
-        status_code = response[1]
+        orig = getattr(uwsgi, "atexit", None)
+
+        def uwsgi_atexit():
+            if callable(orig):
+                orig()
+            func()
+
+        uwsgi.atexit = uwsgi_atexit
+    except ImportError:
+        atexit.register(func)
+
+
+def get_default_library_patters():
+    """
+    Returns library paths depending on the used platform.
+
+    :return: a list of glob paths
+    """
+    python_version = platform.python_version_tuple()
+    python_implementation = platform.python_implementation()
+    system = platform.system()
+    if python_implementation == "PyPy":
+        if python_version[0] == "2":
+            return ["*/lib-python/%s.%s/*" % python_version[:2], "*/site-packages/*"]
+        else:
+            return ["*/lib-python/%s/*" % python_version[0], "*/site-packages/*"]
     else:
-        # httpcore >= 0.11.0
-        # response = (status_code, headers, stream, ext)
-        status_code = response[0]
-    return status_code
+        if system == "Windows":
+            return [r"*\lib\*"]
+        return ["*/lib/python%s.%s/*" % python_version[:2], "*/lib64/python%s.%s/*" % python_version[:2]]
+
+
+def multidict_to_dict(d):
+    """
+    Turns a werkzeug.MultiDict or django.MultiValueDict into a dict with
+    list values
+    :param d: a MultiDict or MultiValueDict instance
+    :return: a dict instance
+    """
+    return dict((k, v[0] if len(v) == 1 else v) for k, v in d.lists())
+
+
+try:
+    import uwsgi
+
+    # check if a master is running before importing postfork
+    if uwsgi.masterpid() != 0:
+        from uwsgidecorators import postfork
+    else:
+
+        def postfork(f):
+            return f
 
+except (ImportError, AttributeError):
 
-def set_disttracing_headers(headers, trace_parent, transaction):
-    trace_parent_str = trace_parent.to_string()
-    headers.append((bytes(constants.TRACEPARENT_HEADER_NAME, "utf-8"), bytes(trace_parent_str, "utf-8")))
-    if transaction.tracer.config.use_atatus_traceparent_header:
-        headers.append((bytes(constants.TRACEPARENT_LEGACY_HEADER_NAME, "utf-8"), bytes(trace_parent_str, "utf-8")))
-    if trace_parent.tracestate:
-        headers.append((bytes(constants.TRACESTATE_HEADER_NAME, "utf-8"), bytes(trace_parent.tracestate, "utf-8")))
+    def postfork(f):
+        return f
```

### Comparing `atatus-1.5.0/atatus/instrumentation/packages/jinja2.py` & `atatus-1.5.1/atatus/instrumentation/packages/jinja2.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/packages/kafka.py` & `atatus-1.5.1/atatus/instrumentation/packages/kafka.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/packages/mysql.py` & `atatus-1.5.1/atatus/instrumentation/packages/mysql.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/packages/mysql_connector.py` & `atatus-1.5.1/atatus/instrumentation/packages/mysql_connector.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/packages/psycopg2.py` & `atatus-1.5.1/atatus/instrumentation/packages/psycopg2.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/packages/pylibmc.py` & `atatus-1.5.1/atatus/instrumentation/packages/pylibmc.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/packages/pymemcache.py` & `atatus-1.5.1/atatus/instrumentation/packages/pymemcache.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/packages/pymongo.py` & `atatus-1.5.1/atatus/instrumentation/packages/pymongo.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/packages/pymssql.py` & `atatus-1.5.1/atatus/instrumentation/packages/pymssql.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/packages/pymysql.py` & `atatus-1.5.1/atatus/instrumentation/packages/pymysql.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/packages/pyodbc.py` & `atatus-1.5.1/atatus/instrumentation/packages/pyodbc.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/packages/python_memcached.py` & `atatus-1.5.1/atatus/instrumentation/packages/python_memcached.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/packages/redis.py` & `atatus-1.5.1/atatus/instrumentation/packages/redis.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/packages/requests.py` & `atatus-1.5.1/atatus/instrumentation/packages/requests.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/packages/sqlite.py` & `atatus-1.5.1/atatus/instrumentation/packages/sqlite.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/packages/tornado.py` & `atatus-1.5.1/atatus/instrumentation/packages/tornado.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/packages/urllib.py` & `atatus-1.5.1/atatus/instrumentation/packages/urllib.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/packages/urllib3.py` & `atatus-1.5.1/atatus/instrumentation/packages/urllib3.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/packages/zlib.py` & `atatus-1.5.1/atatus/instrumentation/packages/zlib.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/instrumentation/register.py` & `atatus-1.5.1/atatus/instrumentation/register.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/metrics/__init__.py` & `atatus-1.5.1/atatus/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/metrics/base_metrics.py` & `atatus-1.5.1/atatus/metrics/base_metrics.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/metrics/sets/__init__.py` & `atatus-1.5.1/atatus/metrics/sets/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/metrics/sets/breakdown.py` & `atatus-1.5.1/atatus/metrics/sets/breakdown.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/metrics/sets/cpu.py` & `atatus-1.5.1/atatus/metrics/sets/cpu.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/metrics/sets/cpu_linux.py` & `atatus-1.5.1/atatus/metrics/sets/cpu_linux.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/metrics/sets/cpu_psutil.py` & `atatus-1.5.1/atatus/metrics/sets/cpu_psutil.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/metrics/sets/prometheus.py` & `atatus-1.5.1/atatus/metrics/sets/prometheus.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/middleware.py` & `atatus-1.5.1/atatus/middleware.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/processors.py` & `atatus-1.5.1/atatus/processors.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/traces.py` & `atatus-1.5.1/atatus/traces.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/transport/__init__.py` & `atatus-1.5.1/atatus/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/transport/base.py` & `atatus-1.5.1/atatus/transport/base.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/transport/exceptions.py` & `atatus-1.5.1/atatus/transport/exceptions.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/transport/http.py` & `atatus-1.5.1/atatus/transport/http.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/transport/http_base.py` & `atatus-1.5.1/atatus/transport/http_base.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/transport/http_urllib3.py` & `atatus-1.5.1/atatus/transport/http_urllib3.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/utils/__init__.py` & `atatus-1.5.1/atatus/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/utils/cgroup.py` & `atatus-1.5.1/atatus/utils/cgroup.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/utils/cloud.py` & `atatus-1.5.1/atatus/utils/cloud.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/utils/deprecation.py` & `atatus-1.5.1/atatus/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/utils/disttracing.py` & `atatus-1.5.1/atatus/utils/disttracing.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/utils/encoding.py` & `atatus-1.5.1/atatus/utils/encoding.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 #  OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 
 
 import datetime
 import itertools
 import uuid
 from decimal import Decimal
+import gzip
 
 from atatus.conf.constants import KEYWORD_MAX_LENGTH, LABEL_RE, LABEL_TYPES, LONG_FIELD_MAX_LENGTH
 
 PROTECTED_TYPES = (int, type(None), float, Decimal, datetime.datetime, datetime.date, datetime.time)
 
 
 def is_protected_type(obj):
@@ -209,14 +210,40 @@
     elif isinstance(var, dict) and len(var) > dict_length:
         trimmed_tuples = [(k, v) for (k, v) in itertools.islice(var.items(), dict_length)]
         if "<truncated>" not in var:
             trimmed_tuples += [("<truncated>", "(%d more elements)" % (len(var) - dict_length))]
         var = dict(trimmed_tuples)
     return var
 
+def body_decode(body):
+    if isinstance(body, bytes):
+        try:
+            string_data = body.decode('UTF-8')
+            return string_data
+        except:
+            pass
+    return body
+
+def body_bytes(body, content_encoding):
+    try:
+        if content_encoding == "gzip":
+            parsed_body = gzip.decompress(body)
+            return parsed_body
+    except:
+        pass
+    return body
+
+def body_string(body, content_encoding):
+    try:
+        if content_encoding == "gzip":
+            decompressed_body = gzip.GzipFile(fileobj=StringIO(body)).read()
+            return decompressed_body
+    except:
+        pass
+    return body
 
 def keyword_field(string):
     """
     If the given string is longer than KEYWORD_MAX_LENGTH, truncate it to
     KEYWORD_MAX_LENGTH-1, adding the "…" character at the end.
     """
     if not isinstance(string, str) or len(string) <= KEYWORD_MAX_LENGTH:
```

### Comparing `atatus-1.5.0/atatus/utils/hw_info.py` & `atatus-1.5.1/atatus/utils/hw_info.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/utils/json_encoder.py` & `atatus-1.5.1/atatus/utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/utils/logging.py` & `atatus-1.5.1/atatus/utils/logging.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/utils/module_import.py` & `atatus-1.5.1/atatus/utils/module_import.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/utils/stacks.py` & `atatus-1.5.1/atatus/utils/stacks.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/utils/threading.py` & `atatus-1.5.1/atatus/utils/threading.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/utils/time.py` & `atatus-1.5.1/atatus/utils/time.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/utils/wrapt/__init__.py` & `atatus-1.5.1/atatus/utils/wrapt/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/utils/wrapt/_wrappers.c` & `atatus-1.5.1/atatus/utils/wrapt/_wrappers.c`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/utils/wrapt/arguments.py` & `atatus-1.5.1/atatus/utils/wrapt/arguments.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/utils/wrapt/decorators.py` & `atatus-1.5.1/atatus/utils/wrapt/decorators.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/utils/wrapt/importer.py` & `atatus-1.5.1/atatus/utils/wrapt/importer.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/utils/wrapt/wrappers.py` & `atatus-1.5.1/atatus/utils/wrapt/wrappers.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/utils/wsgi.py` & `atatus-1.5.1/atatus/utils/wsgi.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/atatus/version.py` & `atatus-1.5.1/atatus/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,9 +24,9 @@
 #  FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 #  DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 #  SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 #  CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 #  OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 #  OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = (1, 5, 0)
+__version__ = (1, 5, 1)
 VERSION = ".".join(map(str, __version__))
```

### Comparing `atatus-1.5.0/atatus.egg-info/PKG-INFO` & `atatus-1.5.1/atatus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atatus
-Version: 1.5.0
+Version: 1.5.1
 Summary: Atatus Python Agent
 Home-page: https://www.atatus.com/for/python
 Author: Atatus
 License: Atatus License
 Project-URL: Documentation, https://docs.atatus.com/docs/application-monitoring/python-agent/overview.html
 Project-URL: Release notes, https://docs.atatus.com/docs/release-notes/python.html
 Description: Atatus APM agent for Python
```

### Comparing `atatus-1.5.0/atatus.egg-info/SOURCES.txt` & `atatus-1.5.1/atatus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/setup.cfg` & `atatus-1.5.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `atatus-1.5.0/setup.py` & `atatus-1.5.1/setup.py`

 * *Files identical despite different names*

