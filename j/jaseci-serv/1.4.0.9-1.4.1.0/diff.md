# Comparing `tmp/jaseci_serv-1.4.0.9.tar.gz` & `tmp/jaseci_serv-1.4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaseci_serv-1.4.0.9.tar", last modified: Tue Feb 14 17:26:34 2023, max compression
+gzip compressed data, was "jaseci_serv-1.4.1.0.tar", last modified: Wed Jun  7 18:27:58 2023, max compression
```

## Comparing `jaseci_serv-1.4.0.9.tar` & `jaseci_serv-1.4.1.0.tar`

### file list

```diff
@@ -1,128 +1,178 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:34.855676 jaseci_serv-1.4.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-02-14 17:26:34.855676 jaseci_serv-1.4.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:34.835675 jaseci_serv-1.4.0.9/jaseci_serv/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/asgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:34.839675 jaseci_serv-1.4.0.9/jaseci_serv/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/base/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/base/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/base/jsorc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9317 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/base/jsorc_loadtest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:34.839675 jaseci_serv-1.4.0.9/jaseci_serv/base/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/base/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:34.839675 jaseci_serv-1.4.0.9/jaseci_serv/base/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/base/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/base/management/commands/createdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/base/management/commands/dropdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/base/management/commands/wait_for_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/base/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:34.839675 jaseci_serv-1.4.0.9/jaseci_serv/base/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/base/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/base/tests/aitest_ai_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/base/tests/mock_redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/base/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/base/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/base/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    11675 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/base/tests/test_orm_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/base/tests/test_orm_hooks_cfg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:34.839675 jaseci_serv-1.4.0.9/jaseci_serv/hook/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/hook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/hook/orm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:34.843675 jaseci_serv-1.4.0.9/jaseci_serv/jac_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/jac_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/jac_api/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/jac_api/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:34.843675 jaseci_serv-1.4.0.9/jaseci_serv/jac_api/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/jac_api/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/jac_api/tests/general.jac
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/jac_api/tests/infer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14915 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/jac_api/tests/ll.jac
--rw-r--r--   0 runner    (1001) docker     (123)    21775 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/jac_api/tests/ll_wall.jac
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/jac_api/tests/public.jac
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/jac_api/tests/public_updated.jac
--rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/jac_api/tests/test_jac_admin_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    70873 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/jac_api/tests/test_jac_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/jac_api/tests/test_jac_general.py
--rw-r--r--   0 runner    (1001) docker     (123)    11101 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/jac_api/tests/test_ll.py
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/jac_api/tests/test_ll_wall.py
--rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/jac_api/tests/test_pub_walker.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/jac_api/tests/try-syntax.jac
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/jac_api/tests/various.jac
--rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/jac_api/tests/zsb.jac
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/jac_api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/jac_api/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:34.847675 jaseci_serv-1.4.0.9/jaseci_serv/jsx_oauth/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/jsx_oauth/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/jsx_oauth/admin.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      103 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/jsx_oauth/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/jsx_oauth/config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2286 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/jsx_oauth/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/jsx_oauth/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/jsx_oauth/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:34.847675 jaseci_serv-1.4.0.9/jaseci_serv/jsx_oauth/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/jsx_oauth/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/jsx_oauth/tests/test_social_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/jsx_oauth/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/jsx_oauth/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/jsx_oauth/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:34.847675 jaseci_serv-1.4.0.9/jaseci_serv/obj_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/obj_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/obj_api/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:34.847675 jaseci_serv-1.4.0.9/jaseci_serv/obj_api/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/obj_api/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/obj_api/tests/test_obj_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/obj_api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/obj_api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:34.847675 jaseci_serv-1.4.0.9/jaseci_serv/svc/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/svc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/svc/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:34.851675 jaseci_serv-1.4.0.9/jaseci_serv/svc/elastic/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/svc/elastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/svc/elastic/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/svc/elastic/elastic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:34.851675 jaseci_serv-1.4.0.9/jaseci_serv/svc/mail/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/svc/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/svc/mail/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/svc/mail/mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/svc/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:34.851675 jaseci_serv-1.4.0.9/jaseci_serv/svc/prometheus/
--rwxr-xr-x   0 runner    (1001) docker     (123)       82 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/svc/prometheus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/svc/prometheus/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/svc/prometheus/prometheus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:34.851675 jaseci_serv-1.4.0.9/jaseci_serv/svc/redis/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/svc/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/svc/redis/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/svc/redis/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:34.851675 jaseci_serv-1.4.0.9/jaseci_serv/svc/stripe/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/svc/stripe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/svc/stripe/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/svc/stripe/stripe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:34.851675 jaseci_serv-1.4.0.9/jaseci_serv/svc/task/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/svc/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/svc/task/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/svc/task/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:34.855676 jaseci_serv-1.4.0.9/jaseci_serv/user_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/user_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/user_api/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/user_api/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:34.855676 jaseci_serv-1.4.0.9/jaseci_serv/user_api/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/user_api/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15768 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/user_api/tests/test_user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/user_api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/user_api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jaseci_serv/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:34.835675 jaseci_serv-1.4.0.9/jaseci_serv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-02-14 17:26:34.000000 jaseci_serv-1.4.0.9/jaseci_serv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-02-14 17:26:34.000000 jaseci_serv-1.4.0.9/jaseci_serv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-14 17:26:34.000000 jaseci_serv-1.4.0.9/jaseci_serv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-02-14 17:26:34.000000 jaseci_serv-1.4.0.9/jaseci_serv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-14 17:26:34.000000 jaseci_serv-1.4.0.9/jaseci_serv.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      628 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/jsserv
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-14 17:26:34.855676 jaseci_serv-1.4.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-02-14 17:25:59.000000 jaseci_serv-1.4.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:27:58.552198 jaseci_serv-1.4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-07 18:27:58.552198 jaseci_serv-1.4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:27:58.524197 jaseci_serv-1.4.1.0/jaseci_serv/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/asgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:27:58.536198 jaseci_serv-1.4.1.0/jaseci_serv/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/base/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/base/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:27:58.536198 jaseci_serv-1.4.1.0/jaseci_serv/base/example_jac/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/base/example_jac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/base/example_jac/discussion_analysis.jac
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/base/example_jac/flight_chatbot.jac
+-rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/base/example_jac/flow_analysis.jac
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/base/example_jac/restaurant_chatbot.jac
+-rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/base/example_jac/sentence_pairing.jac
+-rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/base/example_jac/virtual_assistant.jac
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/base/example_jac/zeroshot_faq_bot.jac
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/base/jsorc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11183 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/base/jsorc_loadtest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:27:58.536198 jaseci_serv-1.4.1.0/jaseci_serv/base/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/base/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:27:58.536198 jaseci_serv-1.4.1.0/jaseci_serv/base/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/base/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/base/management/commands/createdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/base/management/commands/dropdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/base/management/commands/wait_for_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/base/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:27:58.540198 jaseci_serv-1.4.1.0/jaseci_serv/base/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/base/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/base/tests/aitest_ai_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/base/tests/mock_redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/base/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/base/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/base/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11781 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/base/tests/test_orm_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/base/tests/test_orm_hooks_cfg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:27:58.540198 jaseci_serv-1.4.1.0/jaseci_serv/hook/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/hook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/hook/orm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:27:58.540198 jaseci_serv-1.4.1.0/jaseci_serv/jac_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/jac_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/jac_api/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/jac_api/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:27:58.544198 jaseci_serv-1.4.1.0/jaseci_serv/jac_api/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/jac_api/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/jac_api/tests/async_update.jac
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/jac_api/tests/general.jac
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/jac_api/tests/infer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14915 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/jac_api/tests/ll.jac
+-rw-r--r--   0 runner    (1001) docker     (123)    21775 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/jac_api/tests/ll_wall.jac
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/jac_api/tests/object_bug.jac
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/jac_api/tests/public.jac
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/jac_api/tests/public_updated.jac
+-rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/jac_api/tests/test_jac_admin_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74281 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/jac_api/tests/test_jac_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/jac_api/tests/test_jac_general.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11098 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/jac_api/tests/test_ll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/jac_api/tests/test_ll_wall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/jac_api/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/jac_api/tests/test_pub_walker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/jac_api/tests/try-syntax.jac
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/jac_api/tests/various.jac
+-rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/jac_api/tests/zsb.jac
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/jac_api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/jac_api/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:27:58.544198 jaseci_serv-1.4.1.0/jaseci_serv/jsx_oauth/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/jsx_oauth/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      626 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/jsx_oauth/admin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      103 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/jsx_oauth/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/jsx_oauth/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3514 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/jsx_oauth/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/jsx_oauth/permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:27:58.548198 jaseci_serv-1.4.1.0/jaseci_serv/jsx_oauth/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/jsx_oauth/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/jsx_oauth/tests/test_social_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/jsx_oauth/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/jsx_oauth/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/jsx_oauth/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:27:58.548198 jaseci_serv-1.4.1.0/jaseci_serv/obj_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/obj_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/obj_api/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:27:58.548198 jaseci_serv-1.4.1.0/jaseci_serv/obj_api/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/obj_api/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/obj_api/tests/test_obj_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/obj_api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/obj_api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:27:58.548198 jaseci_serv-1.4.1.0/jaseci_serv/studio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/studio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:27:58.548198 jaseci_serv-1.4.1.0/jaseci_serv/studio/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/studio/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/studio/tests/test_studio_routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/studio/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/studio/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:27:58.548198 jaseci_serv-1.4.1.0/jaseci_serv/svc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/svc/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      230 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/svc/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/svc/mail_svc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:27:58.552198 jaseci_serv-1.4.1.0/jaseci_serv/user_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/user_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/user_api/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/user_api/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:27:58.552198 jaseci_serv-1.4.1.0/jaseci_serv/user_api/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/user_api/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15642 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/user_api/tests/test_user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/user_api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/user_api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jaseci_serv/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:27:58.528198 jaseci_serv-1.4.1.0/jaseci_serv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-07 18:27:58.000000 jaseci_serv-1.4.1.0/jaseci_serv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-06-07 18:27:58.000000 jaseci_serv-1.4.1.0/jaseci_serv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 18:27:58.000000 jaseci_serv-1.4.1.0/jaseci_serv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-07 18:27:58.000000 jaseci_serv-1.4.1.0/jaseci_serv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 18:27:58.000000 jaseci_serv-1.4.1.0/jaseci_serv.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      628 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/jsserv
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 18:27:58.552198 jaseci_serv-1.4.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:27:58.520197 jaseci_serv-1.4.1.0/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:27:58.528198 jaseci_serv-1.4.1.0/static/studio/
+-rw-r--r--   0 runner    (1001) docker     (123)   217364 2023-06-07 18:27:36.000000 jaseci_serv-1.4.1.0/static/studio/Jaseci-Submark.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:27:58.520197 jaseci_serv-1.4.1.0/static/studio/_next/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:27:58.520197 jaseci_serv-1.4.1.0/static/studio/_next/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:27:58.528198 jaseci_serv-1.4.1.0/static/studio/_next/static/chunks/
+-rw-r--r--   0 runner    (1001) docker     (123)    78281 2023-06-07 18:27:36.000000 jaseci_serv-1.4.1.0/static/studio/_next/static/chunks/113-f20cf828040267fc.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15560 2023-06-07 18:27:36.000000 jaseci_serv-1.4.1.0/static/studio/_next/static/chunks/289-4a13cf748d6cfb17.js
+-rw-r--r--   0 runner    (1001) docker     (123)    29311 2023-06-07 18:27:36.000000 jaseci_serv-1.4.1.0/static/studio/_next/static/chunks/3-d801e16fe6466f20.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19722 2023-06-07 18:27:36.000000 jaseci_serv-1.4.1.0/static/studio/_next/static/chunks/30-825cca92eb40c60a.js
+-rw-r--r--   0 runner    (1001) docker     (123)    53501 2023-06-07 18:27:36.000000 jaseci_serv-1.4.1.0/static/studio/_next/static/chunks/358-5eea73ebeed3f5bf.js
+-rw-r--r--   0 runner    (1001) docker     (123)   151456 2023-06-07 18:27:36.000000 jaseci_serv-1.4.1.0/static/studio/_next/static/chunks/707-69e1edf708a55a15.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-06-07 18:27:36.000000 jaseci_serv-1.4.1.0/static/studio/_next/static/chunks/76-3f26e2d93951e5cd.js
+-rw-r--r--   0 runner    (1001) docker     (123)   141058 2023-06-07 18:27:36.000000 jaseci_serv-1.4.1.0/static/studio/_next/static/chunks/framework-3b5a00d5d7e8d93b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    85384 2023-06-07 18:27:36.000000 jaseci_serv-1.4.1.0/static/studio/_next/static/chunks/main-1844b67c68085ff6.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:27:58.532198 jaseci_serv-1.4.1.0/static/studio/_next/static/chunks/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)   287285 2023-06-07 18:27:36.000000 jaseci_serv-1.4.1.0/static/studio/_next/static/chunks/pages/_app-3023bf5945430c06.js
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-07 18:27:36.000000 jaseci_serv-1.4.1.0/static/studio/_next/static/chunks/pages/_error-8353112a01355ec2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-06-07 18:27:36.000000 jaseci_serv-1.4.1.0/static/studio/_next/static/chunks/pages/actions-23d0ce4e5128707c.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11815 2023-06-07 18:27:36.000000 jaseci_serv-1.4.1.0/static/studio/_next/static/chunks/pages/architype-d880a2d3a649d424.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11389 2023-06-07 18:27:36.000000 jaseci_serv-1.4.1.0/static/studio/_next/static/chunks/pages/dashboard-1f7803986fd8e669.js
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-07 18:27:36.000000 jaseci_serv-1.4.1.0/static/studio/_next/static/chunks/pages/emotion-5c2381ec5367a041.js
+-rw-r--r--   0 runner    (1001) docker     (123)    27709 2023-06-07 18:27:36.000000 jaseci_serv-1.4.1.0/static/studio/_next/static/chunks/pages/graph-viewer-11af1303610b16aa.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-06-07 18:27:36.000000 jaseci_serv-1.4.1.0/static/studio/_next/static/chunks/pages/index-9873ec26aff4396d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-07 18:27:36.000000 jaseci_serv-1.4.1.0/static/studio/_next/static/chunks/pages/layout-8121c21658da9a00.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-06-07 18:27:36.000000 jaseci_serv-1.4.1.0/static/studio/_next/static/chunks/pages/logs-a311b718d668cc55.js
+-rw-r--r--   0 runner    (1001) docker     (123)    91460 2023-06-07 18:27:36.000000 jaseci_serv-1.4.1.0/static/studio/_next/static/chunks/polyfills-c67a75d1b6f99dc8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-06-07 18:27:36.000000 jaseci_serv-1.4.1.0/static/studio/_next/static/chunks/webpack-620c68345e03c539.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:27:58.532198 jaseci_serv-1.4.1.0/static/studio/_next/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-07 18:27:36.000000 jaseci_serv-1.4.1.0/static/studio/_next/static/css/cc49d8d41e055bcd.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:27:58.532198 jaseci_serv-1.4.1.0/static/studio/_next/static/l_z_Xkf-xtxbUILJVFoom/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-07 18:27:36.000000 jaseci_serv-1.4.1.0/static/studio/_next/static/l_z_Xkf-xtxbUILJVFoom/_buildManifest.js
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-07 18:27:36.000000 jaseci_serv-1.4.1.0/static/studio/_next/static/l_z_Xkf-xtxbUILJVFoom/_ssgManifest.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:27:58.532198 jaseci_serv-1.4.1.0/static/studio/_next/static/media/
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-06-07 18:27:36.000000 jaseci_serv-1.4.1.0/static/studio/_next/static/media/2e1b830192b7974a.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    10088 2023-06-07 18:27:36.000000 jaseci_serv-1.4.1.0/static/studio/_next/static/media/3478b6abef19b3b3.p.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     8760 2023-06-07 18:27:36.000000 jaseci_serv-1.4.1.0/static/studio/_next/static/media/3aa27b2eb5f698f7.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-06-07 18:27:36.000000 jaseci_serv-1.4.1.0/static/studio/_next/static/media/d607327a37a507c7.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-06-07 18:27:36.000000 jaseci_serv-1.4.1.0/static/studio/_next/static/media/ebec2867f40f78ec.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-06-07 18:27:36.000000 jaseci_serv-1.4.1.0/static/studio/react.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-07 18:27:36.000000 jaseci_serv-1.4.1.0/static/studio/test.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:27:58.552198 jaseci_serv-1.4.1.0/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:27:58.552198 jaseci_serv-1.4.1.0/templates/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/templates/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-06-07 18:24:54.000000 jaseci_serv-1.4.1.0/templates/examples/social_auth.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:27:58.536198 jaseci_serv-1.4.1.0/templates/studio/
+-rw-r--r--   0 runner    (1001) docker     (123)    17468 2023-06-07 18:27:37.000000 jaseci_serv-1.4.1.0/templates/studio/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14419 2023-06-07 18:27:37.000000 jaseci_serv-1.4.1.0/templates/studio/actions.html
+-rw-r--r--   0 runner    (1001) docker     (123)    58019 2023-06-07 18:27:37.000000 jaseci_serv-1.4.1.0/templates/studio/architype.html
+-rw-r--r--   0 runner    (1001) docker     (123)    25538 2023-06-07 18:27:37.000000 jaseci_serv-1.4.1.0/templates/studio/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (123)    16059 2023-06-07 18:27:37.000000 jaseci_serv-1.4.1.0/templates/studio/emotion.html
+-rw-r--r--   0 runner    (1001) docker     (123)    19582 2023-06-07 18:27:37.000000 jaseci_serv-1.4.1.0/templates/studio/graph-viewer.html
+-rw-r--r--   0 runner    (1001) docker     (123)    33279 2023-06-07 18:27:37.000000 jaseci_serv-1.4.1.0/templates/studio/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    21974 2023-06-07 18:27:37.000000 jaseci_serv-1.4.1.0/templates/studio/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)    38884 2023-06-07 18:27:37.000000 jaseci_serv-1.4.1.0/templates/studio/logs.html
```

### Comparing `jaseci_serv-1.4.0.9/LICENSE` & `jaseci_serv-1.4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.0.9/jaseci_serv/base/admin.py` & `jaseci_serv-1.4.1.0/jaseci_serv/base/admin.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.0.9/jaseci_serv/base/management/commands/createdb.py` & `jaseci_serv-1.4.1.0/jaseci_serv/base/management/commands/createdb.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.0.9/jaseci_serv/base/management/commands/dropdb.py` & `jaseci_serv-1.4.1.0/jaseci_serv/base/management/commands/dropdb.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.0.9/jaseci_serv/base/management/commands/wait_for_db.py` & `jaseci_serv-1.4.1.0/jaseci_serv/base/management/commands/wait_for_db.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.0.9/jaseci_serv/base/models.py` & `jaseci_serv-1.4.1.0/jaseci_serv/base/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,23 @@
     AbstractBaseUser,
     BaseUserManager,
     PermissionsMixin,
 )
 from django.db import models
 from django.db.models import Q
 
-from jaseci.api.interface import Interface
-from jaseci.element.master import Master as CoreMaster
-from jaseci.element.super_master import SuperMaster as CoreSuper
+from jaseci.extens.api.interface import Interface
+from jaseci.prim.master import Master as CoreMaster
+from jaseci.prim.super_master import SuperMaster as CoreSuper
 from jaseci_serv.settings import JASECI_CONFIGS
-from jaseci_serv.svc import MetaService
+from jaseci.jsorc.jsorc import JsOrc
 from jaseci_serv.base.jsorc import JsOrcApi
 
 
+@JsOrc.context(name="master", priority=1)
 class Master(CoreMaster):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._valid_configs += JASECI_CONFIGS
 
     def user_creator(self, name, password, other_fields: dict = {}):
         """
@@ -73,15 +74,35 @@
         """
         try:
             get_user_model().objects.get(email=name).delete()
             return True
         except Exception:
             return False
 
+    @Interface.private_api()
+    def master_self(self, detailed: bool = False):
+        """
+        Returns the masters object
+        """
+        info = self.serialize(detailed=detailed)
+        if detailed:
+            for user in get_user_model().objects.filter(email=info["name"])[0:1]:
+                info["__meta__"] = {
+                    "id": user.id,
+                    "jid": user.master.urn,
+                    "email": user.email,
+                    "name": user.name,
+                    "created_date": user.time_created.isoformat(),
+                    "is_activated": user.is_activated,
+                    "is_superuser": user.is_superuser,
+                }
+        return info
+
 
+@JsOrc.context(name="super_master", priority=1)
 class SuperMaster(Master, JsOrcApi, CoreSuper):
     @Interface.admin_api()
     def master_allusers(
         self, limit: int = 10, offset: int = 0, asc: bool = False, search: str = None
     ):
         """
         Returns info on a set of users, limit specifies the number of users to
@@ -109,14 +130,17 @@
                     "id": i.id,
                     "user": i.email,
                     "jid": i.master.urn,
                     "name": i.name,
                     "created_date": i.time_created.isoformat(),
                     "is_activated": i.is_activated,
                     "is_superuser": i.is_superuser,
+                    "last_login": i.last_login.isoformat()
+                    if i.last_login is not None
+                    else "",
                 }
             )
         ret = {"total": total, "data": filtered_users}
 
         return ret
 
 
@@ -135,15 +159,15 @@
             return self.create_superuser(email, password, **extra_fields)
         email = self.normalize_email(email).lower()
         user = self.model(email=email, **extra_fields)
         user.set_password(password)
         user.save(using=self._db)
 
         # Create user's root node
-        user.master = MetaService().build_master(h=user._h, name=email).id
+        user.master = JsOrc.master(h=user._h, name=email).id
         user._h.commit()
 
         user.save(using=self._db)
         return user
 
     def create_superuser(self, email, password=None, **extra_fields):
         """Creates and saves a new super user"""
@@ -153,15 +177,15 @@
         user.is_staff = True
         user.is_activated = True
         user.is_admin = True
         user.is_superuser = True
         user.save(using=self._db)
 
         # Create user's root node
-        user.master = MetaService().build_super_master(h=user._h, name=email).id
+        user.master = JsOrc.super_master(h=user._h, name=email).id
         user._h.commit()
 
         user.save(using=self._db)
         return user
 
 
 class User(AbstractBaseUser, PermissionsMixin):
@@ -180,15 +204,15 @@
     is_staff = models.BooleanField(default=False)
     is_admin = models.BooleanField(default=False)
     is_superuser = models.BooleanField(default=False)
     master = models.UUIDField(default=uuid.uuid4)
     objects = UserManager()
 
     def __init__(self, *args, **kwargs):
-        self._h = MetaService().build_hook()
+        self._h = JsOrc.hook(use_proxy=True)
         AbstractBaseUser.__init__(self, *args, **kwargs)
         PermissionsMixin.__init__(self, *args, **kwargs)
 
     USERNAME_FIELD = "email"
 
     def get_master(self):
         """Returns main user Jaseci node"""
```

### Comparing `jaseci_serv-1.4.0.9/jaseci_serv/base/tests/aitest_ai_models.py` & `jaseci_serv-1.4.1.0/jaseci_serv/base/tests/aitest_ai_models.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,25 @@
 from django.test import TestCase
 
-import jaseci.actions.live_actions as lact
+import jaseci.jsorc.live_actions as lact
 import jaseci.tests.jac_test_code as jtc
-from jaseci.actor.sentinel import sentinel
-from jaseci.graph.graph import Graph
+from jaseci.prim.sentinel import sentinel
+from jaseci.prim.graph import Graph
 from jaseci.utils.utils import TestCaseHelper
-from jaseci_serv.svc import MetaService
+from jaseci.jsorc.jsorc import JsOrc
 
 
 class JacTests(TestCaseHelper, TestCase):
     """Unit tests for Jac language"""
 
-    def setUp(self):
-        super().setUp()
-        self.meta = MetaService()
-
-    def tearDown(self):
-        super().tearDown()
-
     def test_basic_use_calls_from_jac(self):
         """Test the execution of a basic walker building graph"""
         if not lact.load_remote_actions("http://js-use-qa"):
             self.skipTest("external resource not available")
-        gph = Graph(m_id=0, h=self.meta.build_hook())
+        gph = Graph(m_id=0, h=JsOrc.hook())
         sent = sentinel(m_id=gph._m_id, h=gph._h)
         sent.register_code(jtc.prog1)
         test_node = sent.arch_ids.get_obj_by_name("life", kind="node").run()
         test_walker = sent.run_architype("use_test")
         test_walker.prime(test_node)
         report = test_walker.run()
         test_walker.save()
@@ -34,15 +27,15 @@
         self.assertEqual(len(report["report"][0]), 2)
         self.assertEqual(len(report["report"][0][1]), 2)
 
     def test_basic_use_single_string_calls_from_jac(self):
         """Test the execution of a basic walker building Graph"""
         if not lact.load_remote_actions("http://js-use-qa"):
             self.skipTest("external resource not available")
-        gph = Graph(m_id=0, h=self.meta.build_hook())
+        gph = Graph(m_id=0, h=JsOrc.hook())
         sent = sentinel(m_id=gph._m_id, h=gph._h)
         sent.register_code(jtc.prog1)
         test_node = sent.arch_ids.get_obj_by_name("life", kind="node").run()
         test_walker = sent.run_architype("use_test_single")
         test_walker.prime(test_node)
         report = test_walker.run()
         test_walker.save()
@@ -50,15 +43,15 @@
         self.assertEqual(len(report["report"][0]), 1)
         self.assertEqual(len(report["report"][0][0]), 1)
 
     def test_use_qa_with_ctx(self):
         """Test the execution of a basic walker building Graph"""
         if not lact.load_remote_actions("http://js-use-qa"):
             self.skipTest("external resource not available")
-        gph = Graph(m_id=0, h=self.meta.build_hook())
+        gph = Graph(m_id=0, h=JsOrc.hook())
         sent = sentinel(m_id=gph._m_id, h=gph._h)
         sent.register_code(jtc.prog1)
         test_node = sent.arch_ids.get_obj_by_name("life", kind="node").run()
         test_walker = sent.run_architype("use_test_with_ctx")
         test_walker.prime(test_node)
         report = test_walker.run()
         test_walker.save()
@@ -66,15 +59,15 @@
         self.assertEqual(len(report["report"][0]), 1)
         self.assertEqual(len(report["report"][0][0]), 1)
 
     def test_use_qa_with_ctx_clean(self):
         """Test the execution of a basic walker building Graph"""
         if not lact.load_remote_actions("http://js-use-qa"):
             self.skipTest("external resource not available")
-        gph = Graph(m_id=0, h=self.meta.build_hook())
+        gph = Graph(m_id=0, h=JsOrc.hook())
         sent = sentinel(m_id=gph._m_id, h=gph._h)
         sent.register_code(jtc.prog1)
         test_node = sent.arch_ids.get_obj_by_name("life", kind="node").run()
         test_walker = sent.run_architype("use_test_with_ctx2")
         test_walker.prime(test_node)
         report = test_walker.run()
         test_walker.save()
```

### Comparing `jaseci_serv-1.4.0.9/jaseci_serv/base/tests/mock_redis.py` & `jaseci_serv-1.4.1.0/jaseci_serv/base/tests/mock_redis.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.0.9/jaseci_serv/base/tests/test_admin.py` & `jaseci_serv-1.4.1.0/jaseci_serv/base/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.0.9/jaseci_serv/base/tests/test_commands.py` & `jaseci_serv-1.4.1.0/jaseci_serv/base/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.0.9/jaseci_serv/base/tests/test_models.py` & `jaseci_serv-1.4.1.0/jaseci_serv/base/tests/test_models.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,26 @@
 from django.contrib.auth import get_user_model
 from django.test import TestCase
 
-from jaseci.element import element
-from jaseci.element.super_master import SuperMaster
+from jaseci.prim import element
+from jaseci.prim.super_master import SuperMaster
 from jaseci.utils.utils import TestCaseHelper
 from jaseci_serv.base import models
 from jaseci_serv.obj_api.views import JaseciObjectSerializer
-from jaseci_serv.svc import MetaService
+from jaseci.jsorc.jsorc import JsOrc
 
 
 def sample_user(email="JSCITEST_user@jaseci.com", password="whatever"):
     """Create a sample user for testing"""
     if get_user_model().objects.filter(email=email).exists():
         return get_user_model().objects.get(email=email)
     return get_user_model().objects.create_user(email, password)
 
 
 class ModelTests(TestCaseHelper, TestCase):
-    def setUp(self):
-        super().setUp()
-        self.meta = MetaService()
-
-    def tearDown(self):
-        super().tearDown()
-
     def test_users_creation_and_deletion(self):
         """
         Tests that users are created based on valid emails and
         objects are deleted with user
         """
         email = "JSCITEST_blah@BlaB.com"
         password = "passW123"
@@ -50,23 +43,23 @@
 
         self.assertIsInstance(user.get_master(), SuperMaster)
         user.delete()
         self.assertFalse(get_user_model().objects.filter(id=user.id).exists())
 
     def test_jaseci_obj_accessl_has_relevant_fields(self):
         """Test that Jaseci ORM models has all element class fields"""
-        element_obj = element.Element(m_id=0, h=self.meta.build_hook())
+        element_obj = element.Element(m_id=0, h=JsOrc.hook())
         orm_obj = models.JaseciObject()
         for a in vars(element_obj).keys():
             if not a.startswith("_") and not callable(getattr(element_obj, a)):
                 self.assertIn(a, dir(orm_obj))
 
     def test_jaseci_json_has_relevant_fields(self):
         """Test that Jaseci ORM models has all element class fields"""
-        element_obj = element.Element(m_id=0, h=self.meta.build_hook())
+        element_obj = element.Element(m_id=0, h=JsOrc.hook())
         for a in vars(element_obj).keys():
             if not a.startswith("_") and not callable(getattr(element_obj, a)):
                 self.assertIn(a, JaseciObjectSerializer.Meta.fields)
 
     def test_jaseci_obj_accessl_create_delete(self):
         """Test that we can create and delete jaseci object models"""
         orm_obj = models.JaseciObject.objects.create(name="test Obj")
```

### Comparing `jaseci_serv-1.4.0.9/jaseci_serv/base/tests/test_orm_hooks.py` & `jaseci_serv-1.4.1.0/jaseci_serv/base/tests/test_orm_hooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from django.contrib.auth import get_user_model
 
 from jaseci.utils.utils import TestCaseHelper
 from jaseci.utils.id_list import IdList
 from django.test import TestCase
 
+from jaseci.jsorc.jsorc import JsOrc
 from jaseci_serv.base.models import JaseciObject
-from jaseci.graph import node
-from jaseci.graph import edge
-from jaseci.graph.graph import Graph
-from jaseci.actor.sentinel import Sentinel
+from jaseci.prim import node
+from jaseci.prim import edge
+from jaseci.prim.graph import Graph
+from jaseci.prim.sentinel import Sentinel
 import jaseci.tests.jac_test_code as jtc
-from jaseci_serv.utils.test_utils import skip_without_redis
+from jaseci.utils.test_core import skip_without_redis
 import uuid
 
 # Alias for create user
 create_user = get_user_model().objects.create_user
 get_user = get_user_model().objects.get
 
 
@@ -132,16 +133,18 @@
         self.assertEqual(node2.id, new_node.jid)
         self.assertEqual(node1.id, new_jsci_node.parent().id)
 
     @skip_without_redis
     def test_redis_connection(self):
         """Test redis connection"""
 
-        redis = self.user._h.redis
+        redis = JsOrc.svc("redis")
+        self.assertTrue(redis.is_running())
 
+        redis = JsOrc.hook().redis
         self.assertTrue(redis.is_running())
 
         redis.set("test", "this is a test")
         self.assertEqual(redis.get("test"), "this is a test")
 
     def test_redis_saving(self):
         """Test that redis hooks are set up correctly for saving"""
```

### Comparing `jaseci_serv-1.4.0.9/jaseci_serv/base/tests/test_orm_hooks_cfg.py` & `jaseci_serv-1.4.1.0/jaseci_serv/base/tests/test_orm_hooks_cfg.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.0.9/jaseci_serv/jac_api/api.py` & `jaseci_serv-1.4.1.0/jaseci_serv/jac_api/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from django.urls import path
 from .views import AbstractJacAPIView
 from .views import AbstractAdminJacAPIView, AbstractPublicJacAPIView
-from jaseci.element.element import Element
+from jaseci.prim.element import Element
 from jaseci_serv.base.models import SuperMaster
 from jaseci.utils.utils import copy_func
 from inspect import signature
 import uuid
 import json
```

### Comparing `jaseci_serv-1.4.0.9/jaseci_serv/jac_api/tests/infer.py` & `jaseci_serv-1.4.1.0/jaseci_serv/jac_api/tests/infer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from jaseci.utils.utils import logger
-import jaseci.actions.standard.date as jsdate
-from jaseci.actions.live_actions import jaseci_action
+import jaseci.extens.act_lib.date as jsdate
+from jaseci.jsorc.live_actions import jaseci_action
 
 
 @jaseci_action()
 def year_from_date(date: str):
     logger.warning("Deprecated! Use date.quantlize_...")
     return jsdate.quantize_to_year(date)
```

### Comparing `jaseci_serv-1.4.0.9/jaseci_serv/jac_api/tests/ll.jac` & `jaseci_serv-1.4.1.0/jaseci_serv/jac_api/tests/ll.jac`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.0.9/jaseci_serv/jac_api/tests/ll_wall.jac` & `jaseci_serv-1.4.1.0/jaseci_serv/jac_api/tests/ll_wall.jac`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.0.9/jaseci_serv/jac_api/tests/test_jac_admin_api.py` & `jaseci_serv-1.4.1.0/jaseci_serv/jac_api/tests/test_jac_admin_api.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.0.9/jaseci_serv/jac_api/tests/test_jac_api.py` & `jaseci_serv-1.4.1.0/jaseci_serv/jac_api/tests/test_jac_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import base64
 import json
 
 from django.contrib.auth import get_user_model
 from django.urls import reverse
-from jaseci_serv.utils.test_utils import skip_without_redis
+from jaseci.utils.test_core import skip_without_redis
 
 from rest_framework.test import APIClient
 from rest_framework import status
 
 from jaseci.utils.utils import TestCaseHelper
 from django.test import TestCase
 
@@ -26,15 +26,15 @@
         )
         self.user = get_user_model().objects.create_user(
             "JSCITfdfdEST_test@jaseci.com", "password"
         )
         self.auth_client = APIClient()
         self.auth_client.force_authenticate(self.user)
         self.suser = get_user_model().objects.create_superuser(
-            "JSCITfdfdEST_test2@jaseci.com", "password"
+            "JSCITfdfdEST_test2@jaseci.com", "password", name="Administrator"
         )
         self.sauth_client = APIClient()
         self.sauth_client.force_authenticate(self.suser)
 
     def tearDown(self):
         super().tearDown()
 
@@ -244,14 +244,33 @@
             reverse("jac_api:walker_queue_check") + f"?task_id={task_id}"
         )
 
         self.assertEqual("SUCCESS", res.data["status"])
         self.assertIsNone(res.data["result"]["anchor"])
         self.assertTrue(res.data["result"]["response"]["success"])
 
+    def test_master_self_detailed(self):
+        """Test public API for walker callback"""
+        zsb_file = open(os.path.dirname(__file__) + "/zsb.jac").read()
+        payload = {"op": "sentinel_register", "name": "zsb", "code": zsb_file}
+        res = self.sauth_client.post(
+            reverse(f'jac_api:{payload["op"]}'), payload, format="json"
+        )
+        self.assertEqual(len(res.data), 2)
+        payload = {"op": "walker_run", "name": "master_self"}
+        res = self.sauth_client.post(
+            reverse(f'jac_api:{payload["op"]}'), payload, format="json"
+        ).data
+        self.assertIn("__meta__", res["report"][0].keys())
+        meta = res["report"][0]["__meta__"]
+        self.assertEqual(meta["email"], "jscitfdfdest_test2@jaseci.com")
+        self.assertEqual(meta["name"], "Administrator")
+        self.assertTrue(meta["is_activated"])
+        self.assertTrue(meta["is_superuser"])
+
 
 class PrivateJacApiTests(TestCaseHelper, TestCase):
     """Test the authorized user node API"""
 
     def setUp(self):
         super().setUp()
         get_user_model().objects.create_user(
@@ -1260,21 +1279,50 @@
         res = self.client.post(reverse("jac_api:walker_list"), payload)
         self.assertEqual(len(res.data), 1)
         res = self.client.post(reverse("jac_api:wapi", args=["ss"]), payload)
         self.assertEqual(res.status_code, 302)
         self.assertTrue(res.data["success"])
 
     def test_jac_admin_master_allusers(self):
-        """Test API for creating a graph"""
+        """Test API for getting all users information"""
         payload = {}
         res = self.sclient.post(
             reverse("jac_api:master_allusers"), payload, format="json"
         )
         self.assertEqual(res.status_code, status.HTTP_200_OK)
 
+    def test_jac_admin_master_allusers_last_login(self):
+        """Test API for getting user information include last login time"""
+        payload = {
+            "op": "master_create",
+            "name": "test@gmail.com",
+            "other_fields": {
+                "password": "abcd1234@#$%",
+                "name": "",
+                "is_activated": True,
+            },
+        }
+        res = self.client.post(
+            reverse(f'jac_api:{payload["op"]}'), payload, format="json"
+        )
+        login_client = APIClient()
+        payload = {"email": "test@gmail.com", "password": "abcd1234@#$%"}
+        res = login_client.post(reverse("user_api:token"), payload)
+
+        res = self.sclient.post(
+            reverse("jac_api:master_allusers"), payload, format="json"
+        )
+        self.assertEqual(res.status_code, status.HTTP_200_OK)
+
+        for i in res.json()["data"]:
+            if i["user"] == "test@gmail.com":
+                self.assertIsNotNone(i["last_login"])
+                return
+            self.fail("Test user does not exist in master_allusers response.")
+
     def test_jac_admin_master_allusers_search(self):
         """Test API for searching users"""
         public_client = APIClient()
         payload = {
             "op": "user_create",
             "name": "john.doe@gmail.com",
             "global_init": "init",
@@ -1555,14 +1603,48 @@
         self.assertEqual(1, res["result"]["anchor"])
         self.assertEqual(1, res["result"]["response"]["report"][0])
         self.assertEqual(2, res["result"]["response"]["report"][1])
         self.assertEqual(
             {"sample": "sample"}, res["result"]["response"]["report"][2]["ctx"]
         )
 
+    @skip_without_redis
+    def test_async_with_update(self):
+        """Test async with attribute update"""
+        zsb_file = open(os.path.dirname(__file__) + "/async_update.jac").read()
+        payload = {"op": "sentinel_register", "name": "zsb", "code": zsb_file}
+        self.client.post(reverse(f'jac_api:{payload["op"]}'), payload, format="json")
+
+        payload = {"op": "walker_run", "name": "update_value"}
+        res = self.client.post(
+            reverse(f'jac_api:{payload["op"]}'), payload, format="json"
+        ).data
+
+        self.assertTrue(res["is_queued"])
+        task_id = res["result"]
+
+        res = self.client.get(
+            reverse("jac_api:walker_queue_wait") + f"?task_id={task_id}"
+        ).data
+
+        self.assertEqual("SUCCESS", res["status"])
+        self.assertIsNone(res["result"]["anchor"])
+        self.assertTrue(res["result"]["response"]["report"][0]["value"])
+
+        # clear current cache since it will still use the outdated _h.mem
+        # _h.mem will always be updated on actual because it will always renew on request
+        self.client.handler._force_user._h.clear_cache()
+
+        payload = {"op": "walker_run", "name": "get_value"}
+        res = self.client.post(
+            reverse(f'jac_api:{payload["op"]}'), payload, format="json"
+        ).data
+
+        self.assertTrue(res["report"][0]["value"])
+
     def test_multipart_json_string(self):
         """Test multipart using json string as ctx parameter"""
         zsb_file = open(os.path.dirname(__file__) + "/zsb.jac").read()
         payload = {"op": "sentinel_register", "name": "zsb", "code": zsb_file}
         self.client.post(reverse(f'jac_api:{payload["op"]}'), payload, format="json")
 
         form = {
```

### Comparing `jaseci_serv-1.4.0.9/jaseci_serv/jac_api/tests/test_ll.py` & `jaseci_serv-1.4.1.0/jaseci_serv/jac_api/tests/test_ll.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from django.contrib.auth import get_user_model
 from django.urls import reverse
 from rest_framework.test import APIClient
 from jaseci.utils.utils import TestCaseHelper
-import jaseci.actions.live_actions as lact
-from jaseci.graph.edge import Edge
+import jaseci.jsorc.live_actions as lact
+from jaseci.prim.edge import Edge
 from django.test import TestCase
 import uuid
 import base64
 import datetime
 import random
 import os
```

### Comparing `jaseci_serv-1.4.0.9/jaseci_serv/jac_api/tests/test_ll_wall.py` & `jaseci_serv-1.4.1.0/jaseci_serv/jac_api/tests/test_ll_wall.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from django.contrib.auth import get_user_model
 from django.urls import reverse
 
 from rest_framework.test import APIClient
 from jaseci.utils.utils import TestCaseHelper
-import jaseci.actions.live_actions as lact
+import jaseci.jsorc.live_actions as lact
 from django.test import TestCase
 import uuid
 import base64
 import os
 
 
 class TestLLWall(TestCaseHelper, TestCase):
```

### Comparing `jaseci_serv-1.4.0.9/jaseci_serv/jac_api/tests/test_pub_walker.py` & `jaseci_serv-1.4.1.0/jaseci_serv/jac_api/tests/test_pub_walker.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.0.9/jaseci_serv/jac_api/tests/try-syntax.jac` & `jaseci_serv-1.4.1.0/jaseci_serv/jac_api/tests/try-syntax.jac`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.0.9/jaseci_serv/jac_api/tests/various.jac` & `jaseci_serv-1.4.1.0/jaseci_serv/jac_api/tests/various.jac`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.0.9/jaseci_serv/jac_api/tests/zsb.jac` & `jaseci_serv-1.4.1.0/jaseci_serv/jac_api/tests/zsb.jac`

 * *Files 2% similar despite different names*

```diff
@@ -294,8 +294,14 @@
 
         if not(global.info['request_context']["body"]["ctx"]) {
             report true;
         }
 
         report global.info['request_context']["body"]["fileTypeField"];
     }
+}
+
+walker master_self {
+    with entry {
+        report jaseci.master_self(true);
+    }
 }
```

### Comparing `jaseci_serv-1.4.0.9/jaseci_serv/jac_api/views.py` & `jaseci_serv-1.4.1.0/jaseci_serv/jac_api/views.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,20 +5,25 @@
 from time import time
 
 from knox.auth import TokenAuthentication
 from rest_framework.permissions import AllowAny, IsAdminUser, IsAuthenticated
 from rest_framework.response import Response
 from rest_framework.views import APIView
 
-from jaseci.element.element import Element
+from jaseci.jsorc.jsorc import JsOrc
+from jaseci.prim.element import Element
 from jaseci.utils.utils import logger, ColCodes as Cc
+from jaseci.utils.actions.actions_manager import ActionManager
 from jaseci_serv.base.models import Master as ServMaster
-from jaseci_serv.svc import MetaService
 from jaseci_serv.user_api import serializers as user_slzr
 
+# The limit for logging an object (request payload and response): 5MB
+# Will truncate in the logs if the object exceeds this limit
+OBJECT_LOG_LIMIT = 5 * 1024 * 1024
+
 
 class JResponse(Response):
     def __init__(self, master, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.hook = master._h
         self.hook.commit_all_cache_sync()
 
@@ -41,57 +46,82 @@
         """
         General GET function that parses api signature to load parms
         SuperSmart GET - can read signatures of master and process
         bodies accordingly
         """
         self.proc_request(request, **kwargs)
         api_result = self.caller.general_interface_to_api(self.cmd, type(self).__name__)
-        self.log_request_stats(request)
+        self.log_request_stats(request, api_result)
         return self.issue_response(api_result)
 
     def post(self, request, **kwargs):
         """
         General post function that parses api signature to load parms
         SuperSmart Post - can read signatures of master and process
         bodies accordingly
         """
         self.proc_request(request, **kwargs)
         api_result = self.caller.general_interface_to_api(self.cmd, type(self).__name__)
-        self.log_request_stats(request)
+        self.log_request_stats(request, api_result)
         return self.issue_response(api_result)
 
-    def log_request_stats(self, request):
+    def log_request_stats(self, request, api_result):
         """Api call preamble"""
         tot_time = time() - self.start_time
         save_count = 0
         touch_count = 0
         db_touches = 0
         touch_kb = 0
         if isinstance(self.caller, Element):
             save_count = len(self.caller._h.save_obj_list)
             touch_count = len(self.caller._h.mem.keys())
             db_touches = self.caller._h.db_touch_count
             red_touches = self.caller._h.red_touch_count
             touch_kb = self.caller._h.mem_size()
-        logger.info(
-            str(
-                f"API call to {Cc.TG}{type(self).__name__}{Cc.EC}"
-                f" completed in {Cc.TY}{tot_time:.3f} seconds{Cc.EC}"
-                f" touched {Cc.TY}{touch_count}{Cc.EC} mem /"
-                f" {Cc.TY}{red_touches}{Cc.EC} redis /"
-                f" {Cc.TY}{db_touches}{Cc.EC} db "
-                f" ({Cc.TY}{touch_kb:.1f}kb{Cc.EC}) and"
-                f" saving {Cc.TY}{save_count}{Cc.EC} objects."
-            )
+
+        res_peek = str(api_result)[:256]
+        log_str = str(
+            f"API call from {Cc.TG}{self.caller.name}{Cc.EC}:{self.caller.jid}"
+            f" to {Cc.TG}{type(self).__name__}{Cc.EC}"
+            f" completed in {Cc.TY}{tot_time:.3f} seconds{Cc.EC}"
+            f" touched {Cc.TY}{touch_count}{Cc.EC} mem /"
+            f" {Cc.TY}{red_touches}{Cc.EC} redis /"
+            f" {Cc.TY}{db_touches}{Cc.EC} db "
+            f" ({Cc.TY}{touch_kb:.1f}kb{Cc.EC}) and"
+            f" saving {Cc.TY}{save_count}{Cc.EC} objects."
+            f" Response: {res_peek}."
         )
 
-        hook = self.caller._h
-        hook.meta.app.post_request_hook(type(self).__name__, request, tot_time) if (
-            hook.meta.run_svcs and hook.meta.app != None
-        ) else None
+        log_dict = {
+            "api_name": type(self).__name__,
+            "request_latency": tot_time,
+            "objects_touched": touch_count,
+            "redis_touches": red_touches,
+            "db_touches": db_touches,
+            "objects_touched_size": touch_kb,
+            "objects_saved": save_count,
+            "caller_name": self.caller.name,
+            "caller_jid": self.caller.jid,
+        }
+        # Add custom fields depending on the type of API
+        if log_dict["api_name"] == "walker_run":
+            log_dict["walker_name"] = self.cmd.get("name", "")
+            log_dict["success"] = (api_result.get("success", True),)
+        try:
+            api_result_str = json.dumps(api_result)[:OBJECT_LOG_LIMIT]
+        except TypeError:
+            api_result_str = str(api_result)[:OBJECT_LOG_LIMIT]
+        log_dict["api_response"] = api_result_str
+
+        log_dict["extra_fields"] = list(log_dict.keys())
+
+        logger.info(log_str, extra=log_dict)
+        JsOrc.get("action_manager", ActionManager).post_request_hook(
+            type(self).__name__, request, tot_time
+        )
 
     def proc_prime_ctx(self, request, req_data):
         try:
             if "ctx" in request.FILES:
                 ctx = request.FILES.pop("ctx")[0]
                 if ctx.content_type == "application/json":
                     req_data["ctx"] = json.loads(ctx.read().decode("utf-8"))
@@ -142,29 +172,50 @@
         )
         req_data.update(req_query)
 
     def proc_request(self, request, **kwargs):
         """Parse request to field set"""
         raw_req_data = request.body
         pl_peek = str(dict(request.data))[:256]
-        logger.info(str(f"Incoming call to {type(self).__name__} with {pl_peek}"))
+        user_agent = request.META.get("HTTP_USER_AGENT", "")
+        self.set_caller(request)
+        log_str = str(
+            f"Incoming call from {Cc.TG}{self.caller.name}{Cc.EC}:{self.caller.jid} to {Cc.TG}{type(self).__name__}{Cc.EC} with {pl_peek} via {user_agent}"
+        )
+        log_dict = {
+            "api_name": type(self).__name__,
+            "caller_name": self.caller.name,
+            "caller_jid": self.caller.jid,
+            "request_user_agent": user_agent,
+        }
+        # Add custom field based on type of API
+        if log_dict["api_name"] == "walker_run":
+            log_dict["walker_name"] = request.data.get("name", "")
+        try:
+            request_payload_str = json.dumps(dict(request.data))[:OBJECT_LOG_LIMIT]
+        except TypeError:
+            request_payload_str = str(dict(request.data))[:OBJECT_LOG_LIMIT]
+        log_dict["request_payload"] = request_payload_str
+        log_dict["extra_fields"] = list(log_dict.keys())
+
+        logger.info(log_str, extra=log_dict)
+
         self.start_time = time()
 
         req_data = (
             request.data.dict() if type(request.data) is not dict else request.data
         )
 
         self.proc_prime_ctx(request, req_data)
         self.proc_file_ctx(request, req_data)
         self.proc_request_ctx(request, req_data, raw_req_data)
 
         req_data.update(kwargs)
 
         self.cmd = req_data
-        self.set_caller(request)
         self.res = "Not valid interaction!"
 
     def set_caller(self, request):
         """Assigns the calling api interface obj"""
         self.caller = request.user.get_master()
 
     def pluck_status_code(self, api_result):
@@ -212,33 +263,33 @@
         Public GET function that parses api signature to load parms
         SuperSmart GET - can read signatures of master and process
         bodies accordingly
         """
         self.proc_request(request, **kwargs)
 
         api_result = self.caller.public_interface_to_api(self.cmd, type(self).__name__)
-        self.log_request_stats(request)
+        self.log_request_stats(request, api_result)
         return self.issue_response(api_result)
 
     def post(self, request, **kwargs):
         """
         Public post function that parses api signature to load parms
         SuperSmart Post - can read signatures of master and process
         bodies accordingly
         """
         self.proc_request(request, **kwargs)
 
         api_result = self.caller.public_interface_to_api(self.cmd, type(self).__name__)
-        self.log_request_stats(request)
+        self.log_request_stats(request, api_result)
         return self.issue_response(api_result)
 
     def set_caller(self, request):
         """Assigns the calling api interface obj"""
         self.caller = ServMaster(
-            h=MetaService().build_hook(),
+            h=JsOrc.hook(),
             persist=False,
         )
 
     def issue_response(self, api_result):
         """Issue response from call"""
         # If committer set, results should be saved back
         status = self.pluck_status_code(api_result)
```

### Comparing `jaseci_serv-1.4.0.9/jaseci_serv/jsx_oauth/utils.py` & `jaseci_serv-1.4.1.0/jaseci_serv/jsx_oauth/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,102 @@
-from jaseci_serv.svc import MetaService
-from jaseci_serv.jsx_oauth.models import PROVIDERS_MAPPING
+from jaseci.jsorc.jsorc import JsOrc
+from jaseci_serv.jsx_oauth.models import PROVIDERS_MAPPING, SocialLoginProvider
 from allauth.socialaccount.providers.oauth2.client import OAuth2Client
 from dj_rest_auth.registration.views import SocialLoginView
 from dj_rest_auth.registration.serializers import SocialLoginSerializer
 from jaseci_serv.base.models import lookup_global_config
+from django.core.exceptions import ObjectDoesNotExist
 from django.conf import settings
 from django.utils.translation import gettext_lazy as _
 from knox.settings import knox_settings
 from knox.models import AuthToken
 from django.contrib.auth import authenticate, get_user_model
 from datetime import timedelta
 from rest_framework.response import Response
 from rest_framework.exceptions import APIException
 from rest_framework import serializers
 from allauth.socialaccount.helpers import complete_social_login
-from allauth.account import app_settings as allauth_settings
 from requests.exceptions import HTTPError
+from enum import Enum
 
+from .models import SocialApp
 
-class RegistrationConflict(APIException):
-    status_code = 409
-    default_detail = "User is already registered with this e-mail address!"
-    default_code = "Registration failed!"
+
+class LoginType(Enum):
+    REGISTRATION = "New account"
+    EXISTING = "Existing account"
+    ACTIVATION = "Existing account but just got activated"
+    BINDING = "Existing account but just got binded with different login type"
+
+
+class AppIdFieldNotExists(APIException):
+    status_code = 400
+    default_detail = "app_id is required!"
+    default_code = "Request failed!"
+
+
+class GetExampleUrlSerializer(serializers.Serializer):
+    provider = serializers.ChoiceField(choices=SocialLoginProvider.choices)
 
 
 class JSXSocialLoginSerializer(SocialLoginSerializer):
+    app_id = serializers.CharField(required=False, allow_blank=True)
+
+    # deprecated
+    internal_client_id = serializers.CharField(required=False, allow_blank=True)
+
     def validate(self, attrs):
         view = self.context.get("view")
         request = self._get_request()
 
         if not view:
             raise serializers.ValidationError(
                 _("View is not defined, pass it as a context variable"),
             )
 
         adapter_class = getattr(view, "adapter_class", None)
         if not adapter_class:
             raise serializers.ValidationError(_("Define adapter_class in view"))
 
         adapter = adapter_class(request)
-        app = adapter.get_provider().get_app(request)
 
-        access_token = attrs.get("access_token")
+        # internal_client_id is deprecated
+        app_id = attrs.get("app_id") or attrs.get("internal_client_id")
+
+        if app_id:
+            try:
+                app = SocialApp.objects.get(id=app_id).legacy()
+            except SocialApp.DoesNotExist:
+                raise serializers.ValidationError(
+                    _(f"app_id is not yet associated on any Social App!"),
+                )
+        else:
+            social_apps = SocialApp.objects.filter(provider=adapter.provider_id)
+            social_apps_count = len(social_apps)
+
+            if social_apps_count > 1:
+                raise serializers.ValidationError(
+                    _(
+                        f"You have multiple {adapter.provider_id} Social App. app_id is required to associated it on one of those apps!"
+                    ),
+                )
+            elif social_apps_count < 1:
+                raise serializers.ValidationError(
+                    _(
+                        f"You don't have any Social App for this provider [{adapter.provider_id}]"
+                    ),
+                )
+            else:
+                # backward compatibility
+                app = social_apps[0].legacy()
+
+        request.app = app
         code = attrs.get("code")
-        # Case 1: We received the access_token
-        if access_token:
-            tokens_to_parse = {"access_token": access_token}
-            token = access_token
-            # For sign in with apple
-            id_token = attrs.get("id_token")
-            if id_token:
-                tokens_to_parse["id_token"] = id_token
 
-        # Case 2: We received the authorization code
-        elif code:
+        if code:
             self.set_callback_url(view=view, adapter_class=adapter_class)
             self.client_class = getattr(view, "client_class", None)
 
             if not self.client_class:
                 raise serializers.ValidationError(
                     _("Define client_class in view"),
                 )
@@ -71,109 +110,110 @@
                 adapter.access_token_url,
                 self.callback_url,
                 scope,
                 scope_delimiter=adapter.scope_delimiter,
                 headers=adapter.headers,
                 basic_auth=adapter.basic_auth,
             )
-            token = client.get_access_token(code)
-            access_token = token["access_token"]
-            tokens_to_parse = {"access_token": access_token}
-
-            # If available we add additional data to the dictionary
-            for key in ["refresh_token", "id_token", adapter.expires_in_key]:
-                if key in token:
-                    tokens_to_parse[key] = token[key]
-        else:
-            raise serializers.ValidationError(
-                _("Incorrect input. access_token or code is required."),
-            )
+            attrs = client.get_access_token(code)
+
+        if not attrs.get("access_token") and attrs.get("id_token"):
+            attrs["access_token"] = attrs["id_token"]
 
-        social_token = adapter.parse_token(tokens_to_parse)
+        social_token = adapter.parse_token(attrs)
         social_token.app = app
 
         try:
-            login = self.get_social_login(adapter, app, social_token, token)
+            login = self.get_social_login(adapter, app, social_token, attrs)
             complete_social_login(request, login)
         except HTTPError:
             raise serializers.ValidationError(_("Incorrect value"))
-        if not login.is_existing:
-            if allauth_settings.UNIQUE_EMAIL:
-                # Do we have an account already with this email address?
-                account_exists = (
-                    get_user_model()
-                    .objects.filter(
-                        email=login.user.email,
-                    )
-                    .exists()
-                )
-                if account_exists:
-                    raise RegistrationConflict()
 
+        attrs["type"] = LoginType.EXISTING
+
+        if not login.is_existing:
             login.lookup()
+            try:
+                user = get_user_model().objects.get(
+                    email=login.user.email,
+                )
+                login.user = user
+                attrs["type"] = LoginType.BINDING
+            except ObjectDoesNotExist:
+                pass
             login.save(request, connect=True)
-        attrs["user"] = login.account.user
-        if "name" in login.account.extra_data.keys():
-            attrs["name"] = login.account.extra_data.get("name", "")
+
+        user = login.account.user
+        attrs["user"] = user
+
+        if not user.is_activated:
+            user.is_activated = True
+            if user.has_usable_password():
+                attrs["type"] = LoginType.ACTIVATION
+            else:
+                if "name" in login.account.extra_data.keys():
+                    user.name = login.account.extra_data.get("name", "")
+                user.master = JsOrc.master(h=user._h, name=user.email).id
+                attrs["type"] = LoginType.REGISTRATION
+
+            user._h.commit()
+            user.save()
+
         return attrs
 
 
 class JSXSocialLoginView(SocialLoginView):
     adapter_class = None
     provider = None
     client_class = OAuth2Client
     serializer_class = JSXSocialLoginSerializer
     # permission_classes = [IsValidateLicense, AllowAny]
 
     def get_callback_url(self, request):
-        callback_url = request.POST.get("callback_url")
+        callback_url = request.data.get("callback_url")
         if callback_url:
             return callback_url
 
         if self.provider:
             prov = PROVIDERS_MAPPING[self.provider]
             return lookup_global_config(
                 name=prov["URL_KEY"],
                 default=f'{request.build_absolute_uri("/")[:-1]}{prov["DEFAULT_REDIRECT_URI"]}',
             )
         raise RuntimeError(
             "Provider name cannot be empty or None. "
             'Please provide a valid provider name e.g. "GOOGLE"'
         )
 
-    def dispatch(self, request, *args, **kwargs):
-        self.callback_url = self.get_callback_url(request)
-        return super().dispatch(request, *args, **kwargs)
-
     def post(self, request, *args, **kwargs):
         self.request = request
+        self.callback_url = self.get_callback_url(request)
         self.serializer = self.get_serializer(data=self.request.data)
         self.serializer.is_valid(raise_exception=True)
-        self.user = self.serializer.validated_data.get("user")
-        # self.login()
-        self.user.is_activated = True
-        self.user.name = self.serializer.validated_data.get("name")
-        self.user.master = (
-            MetaService().build_master(h=self.user._h, name=self.user.email).id
-        )
-        self.user._h.commit()
-        self.user.save()
-        auth_token = AuthToken.objects.filter(user_id=self.user.id)
-        if auth_token:
-            AuthToken.objects.filter(user_id=self.user.id).delete()
-        instance, token = AuthToken.objects.create(
-            self.user,
+        data = self.serializer.validated_data
+        self.user = data.get("user")
+
+        expiry = (
             knox_settings.TOKEN_TTL
             if knox_settings.TOKEN_TTL
-            else timedelta(hours=settings.KNOX_TOKEN_EXPIRY),
+            else timedelta(hours=settings.KNOX_TOKEN_EXPIRY)
         )
+        expires_in: str = self.request.query_params.get("expires_in")
+
+        if expires_in and expires_in.isnumeric():
+            expiry = None if expires_in == "0" else timedelta(hours=int(expires_in))
+
+        instance, token = AuthToken.objects.create(self.user, expiry)
 
         auth_user = authenticate(
             request=self.request, username=self.user.email, password=self.user.password
         )
+        login_type = data.get("type")
         return Response(
             {
                 "email": auth_user.email if auth_user else self.user.email,
                 "token": token,
                 "exp": instance.expiry,
+                "type": login_type.name,
+                "details": login_type.value,
             }
         )
```

### Comparing `jaseci_serv-1.4.0.9/jaseci_serv/jsx_oauth/views.py` & `jaseci_serv-1.4.1.0/jaseci_serv/jsx_oauth/views.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,43 +2,87 @@
 import string
 from allauth.socialaccount.providers.google.views import GoogleOAuth2Adapter
 from allauth.socialaccount.providers.facebook.views import FacebookOAuth2Adapter
 from allauth.socialaccount.providers.github.views import GitHubOAuth2Adapter
 from allauth.socialaccount.providers.microsoft.views import MicrosoftGraphOAuth2Adapter
 from allauth.socialaccount.providers.okta.views import OktaOAuth2Adapter
 from allauth.socialaccount.providers.oauth2.client import OAuth2Client
+from allauth.socialaccount.providers.apple.views import (
+    AppleOAuth2Adapter as LegacyAppleOAuth2Adapter,
+    AppleOAuth2Client,
+)
+from allauth.socialaccount.adapter import DefaultSocialAccountAdapter, get_adapter
 from rest_framework.generics import GenericAPIView
 from rest_framework.response import Response
-from jaseci_serv.jsx_oauth import serializers
-from django.conf import settings
+from jaseci_serv.jsx_oauth.utils import GetExampleUrlSerializer
 from django.views import View
 from django.shortcuts import render
 from django.utils.translation import gettext_lazy as _
+from django.utils.decorators import method_decorator
+from django.views.decorators.csrf import csrf_exempt
 from rest_framework import status
 from rest_framework.generics import GenericAPIView
 from rest_framework.response import Response
-from jaseci_serv.jsx_oauth.models import SocialLoginProvider, PROVIDERS_MAPPING
-from allauth.socialaccount.models import SocialApp
+from jaseci_serv.jsx_oauth.models import (
+    SocialLoginProvider,
+    PROVIDERS_MAPPING,
+    SocialApp,
+)
 from jaseci_serv.jsx_oauth.utils import JSXSocialLoginView
 
+#################################################
+#     OVERRIDING DEFAULTS FOR APPLE SIGN IN     #
+#################################################
+
+main_get_app = DefaultSocialAccountAdapter.get_app
+
+
+def custom_get_app(self, request, provider, config=None):
+    if hasattr(request, "app") and request.app:
+        return request.app
+    return main_get_app(self, request, provider, config)
+
+
+DefaultSocialAccountAdapter.get_app = custom_get_app
+
+
+class AppleOAuth2Adapter(LegacyAppleOAuth2Adapter):
+    def get_client_id(self, provider):
+        app = get_adapter().get_app(self.request, provider)
+        return [aud.strip() for aud in app.client_id.split(",")]
+
+
+# --------------------------------------------- #
+
+
+def generate_state():
+    return "".join(
+        random.choices(
+            string.ascii_uppercase + string.ascii_lowercase + string.digits, k=64
+        )
+    )
+
 
 class ExampleUrlView(GenericAPIView):
-    serializer_class = serializers.GetExampleUrlSerializer
+    serializer_class = GetExampleUrlSerializer
 
     def post(self, request):
         serializer_data = self.serializer_class(data=request.data)
         serializer_data.is_valid(raise_exception=True)
         provider = serializer_data.validated_data.get("provider")
-        callback_url = f"{request.build_absolute_uri('/')[:-1]}{settings.DEFAULT_CALLBACK_URL_FOR_SSO}"
+        provider_map = PROVIDERS_MAPPING[provider]
+        callback_url = f'{request.build_absolute_uri("/")[:-1]}{provider_map["DEFAULT_REDIRECT_URI"]}'
         social_app = SocialApp.objects.filter(provider=provider.lower()).first()
         if social_app:
             return Response(
                 {
-                    "url": PROVIDERS_MAPPING[provider]["LOGIN_URL"].format(
-                        callback_url=callback_url, client_id=social_app.client_id
+                    "url": provider_map["LOGIN_URL"].format(
+                        callback_url=callback_url,
+                        client_id=social_app.client_id,
+                        state=generate_state(),
                     )
                 }
             )
         else:
             return Response(
                 {
                     "error": f"Social login applications for the {provider} not configured properly"
@@ -79,30 +123,42 @@
 
 class OpenIdLogin(JSXSocialLoginView):
     adapter_class = GitHubOAuth2Adapter  # TODO: create custom adaptor for OpenID
     provider = SocialLoginProvider.OPENID
     client_class = OAuth2Client
 
 
+class AppleLogin(JSXSocialLoginView):
+    adapter_class = AppleOAuth2Adapter
+    provider = SocialLoginProvider.APPLE
+    client_class = AppleOAuth2Client
+
+
+@method_decorator(csrf_exempt, name="dispatch")
 class ExampleLiveView(View):
     template_name = "examples/social_auth.html"
 
     def get(self, request, provider):
         code = request.GET.get("code")
         social_app = SocialApp.objects.filter(provider=provider).first()
         return render(
             request,
             self.template_name,
             {
                 "provider": provider,
                 "code": code,
                 "client_id": social_app.client_id,
-                "state": self.generate_state(),
+                "state": generate_state(),
             },
         )
 
-    def generate_state(self):
-        return "".join(
-            random.choices(
-                string.ascii_uppercase + string.ascii_lowercase + string.digits, k=64
-            )
+    def post(self, request, provider):
+        data = request.POST.dict()
+        return render(
+            request,
+            self.template_name,
+            {
+                "provider": provider,
+                "id_token": data["id_token"],
+                "state": data["state"],
+            },
         )
```

### Comparing `jaseci_serv-1.4.0.9/jaseci_serv/obj_api/tests/test_obj_api.py` & `jaseci_serv-1.4.1.0/jaseci_serv/obj_api/tests/test_obj_api.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.0.9/jaseci_serv/obj_api/views.py` & `jaseci_serv-1.4.1.0/jaseci_serv/obj_api/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from knox.auth import TokenAuthentication
 from rest_framework.permissions import IsAdminUser, IsAuthenticated
 from rest_framework import serializers as slzrs
 from rest_framework.serializers import HyperlinkedIdentityField
 from django.contrib.auth.models import AnonymousUser
 
 from jaseci_serv.base import models
-from jaseci_serv.hook.orm import json_str_to_jsci_dict
+from jaseci.utils.json_handler import json_str_to_jsci_dict
 
 
 class JaseciObjectSerializer(slzrs.HyperlinkedModelSerializer):
     """Serializer for Jaseci object model"""
 
     url = HyperlinkedIdentityField(view_name="obj_api:jaseciobject-detail")
```

### Comparing `jaseci_serv-1.4.0.9/jaseci_serv/settings.py` & `jaseci_serv-1.4.1.0/jaseci_serv/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 """
 
 import os
 import sys
 
 from .jsx_oauth.config import *
 
+# Increase data upload max size for requests
+DATA_UPLOAD_MAX_MEMORY_SIZE = 10485760
+
 # Build paths inside the project like this: os.path.join(BASE_DIR, ...)
 BASE_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 
 TEMPLATE_DIR = os.path.join(BASE_DIR, "ui/templates")
 
 # Quick-start development settings - unsuitable for production
 # See https://docs.djangoproject.com/en/3.0/howto/deployment/checklist/
@@ -37,26 +40,34 @@
     "django.contrib.admin",
     "django.contrib.auth",
     "django.contrib.contenttypes",
     "django.contrib.sessions",
     "django.contrib.messages",
     "django.contrib.staticfiles",
     "rest_framework",
+    "rest_framework.authtoken",
     "knox",
     "django_rest_passwordreset",
     "drf_yasg",
+    "allauth",
+    "allauth.account",
+    "allauth.socialaccount",
+    "dj_rest_auth",
+    "dj_rest_auth.registration",
     "jaseci_serv.base",
     "jaseci_serv.user_api",
     "jaseci_serv.obj_api",
     "jaseci_serv.jac_api",
     "corsheaders",
     "django_celery_results",
     "django_celery_beat",
     "jaseci_serv.jsx_oauth",
-]
+    # this MUST always be the last app
+    "jaseci_serv.svc",
+] + OAUTH_APPS
 
 MIDDLEWARE = [
     "corsheaders.middleware.CorsMiddleware",
     "django.middleware.security.SecurityMiddleware",
     "django.contrib.sessions.middleware.SessionMiddleware",
     "django.middleware.common.CommonMiddleware",
     "django.middleware.csrf.CsrfViewMiddleware",
@@ -68,15 +79,15 @@
 CORS_ORIGIN_ALLOW_ALL = True
 
 ROOT_URLCONF = "jaseci_serv.urls"
 
 TEMPLATES = [
     {
         "BACKEND": "django.template.backends.django.DjangoTemplates",
-        "DIRS": [TEMPLATE_DIR],
+        "DIRS": [TEMPLATE_DIR, os.path.join(BASE_DIR, "templates")],
         "APP_DIRS": True,
         "OPTIONS": {
             "context_processors": [
                 "django.template.context_processors.debug",
                 "django.template.context_processors.request",
                 "django.contrib.auth.context_processors.auth",
                 "django.contrib.messages.context_processors.messages",
@@ -204,18 +215,7 @@
     "EMAIL_RESETPASS_BODY",
     "EMAIL_RESETPASS_HTML_BODY",
     "LOGIN_TOKEN_TTL_HOURS",
 ]
 
 DJANGO_CELERY_BEAT_TZ_AWARE = False
 DEFAULT_AUTO_FIELD = "django.db.models.AutoField"
-
-
-#################################################
-#                    ADDONS                     #
-#################################################
-
-# ------------------- OAUTH ------------------- #
-
-INSTALLED_APPS += OAUTH_APPS
-JSX_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
-TEMPLATES[0]["DIRS"] += [os.path.join(JSX_DIR, "templates")]
```

### Comparing `jaseci_serv-1.4.0.9/jaseci_serv/svc/mail/mail.py` & `jaseci_serv-1.4.1.0/jaseci_serv/svc/mail_svc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from django.core import mail
-
-from jaseci.svc import MailService as Ms
-from jaseci.svc.mail import Mailer as Em
-from .config import MAIL_CONFIG
+from jaseci.jsorc.jsorc import JsOrc
+from jaseci.extens.svc.mail_svc import MailService as Ms, Mailer as Em
 
 #################################################
 #                 EMAIL APP ORM                 #
 #################################################
 
 
+@JsOrc.service(name="mail", config="MAIL_CONFIG", priority=1)
 class MailService(Ms):
     def connect(self):
         user = self.config.get("user")
         backend = self.config.get("backend", "smtp")
         sender = self.config.get("sender", user)
 
         server = mail.get_connection(
@@ -28,23 +27,19 @@
         server.open()
 
         # closing will now let the actual email sending open their own connecion
         server.close()
 
         return Mailer(server, sender, self.config["templates"])
 
-    def build_config(self, hook) -> dict:
-        return hook.service_glob("MAIL_CONFIG", MAIL_CONFIG)
-
 
 # ----------------------------------------------- #
 
-
 ####################################################
-#                   EMAIL CONFIG                   #
+#                      MAILER                      #
 ####################################################
 
 
 class Mailer(Em):
     def __init__(self, server, sender, templates):
         super().__init__(server, sender)
```

### Comparing `jaseci_serv-1.4.0.9/jaseci_serv/urls.py` & `jaseci_serv-1.4.1.0/jaseci_serv/urls.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,11 +38,12 @@
         "docs/",
         schema_view.with_ui("swagger", cache_timeout=0),
         name="schema-swagger-ui",
     ),
     path("redocs/", schema_view.with_ui("redoc", cache_timeout=0), name="schema-redoc"),
     path("admin/", admin.site.urls),
     path("user/", include("jaseci_serv.user_api.urls")),
+    path("studio/", include("jaseci_serv.studio.urls")),
     path("", include("jaseci_serv.jac_api.urls")),
     path("", include("jaseci_serv.obj_api.urls")),
     path("", include("jaseci_serv.jsx_oauth.urls")),
 ]
```

### Comparing `jaseci_serv-1.4.0.9/jaseci_serv/user_api/serializers.py` & `jaseci_serv-1.4.1.0/jaseci_serv/user_api/serializers.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,38 +3,37 @@
 from django.contrib.auth import authenticate, get_user_model
 from django.dispatch import receiver
 from django.urls import reverse
 from django.utils.translation import ugettext_lazy as _
 from django_rest_passwordreset.signals import reset_password_token_created
 from rest_framework import serializers
 
-from jaseci.utils.utils import logger
-from jaseci_serv.svc import MetaService
+from jaseci.jsorc.jsorc import JsOrc
+from jaseci_serv.svc.mail_svc import Mailer
 
 requests_for_emails = None
 
 
 def send_activation_email(email):
     """Construct activation email body"""
     code = base64.b64encode(email.encode()).decode()
     if requests_for_emails is not None:
         link = requests_for_emails.build_absolute_uri(
             reverse("user_api:activate", kwargs={"code": code})
         )
     else:
         link = "invalid"
-
-    MetaService().get_service("mail").poke().send_activation_email(email, code, link)
+    JsOrc.svc("mail").poke(Mailer).send_activation_email(email, code, link)
 
 
 @receiver(reset_password_token_created)
 def password_reset_token_created(
     sender, instance, reset_password_token, *args, **kwargs
 ):
-    MetaService().get_service("mail").poke().send_reset_email(
+    JsOrc.svc("mail").poke(Mailer).send_reset_email(
         reset_password_token.user.email, reset_password_token.key
     )
 
 
 class UserSerializer(serializers.ModelSerializer):
     """Serializer for users object"""
```

### Comparing `jaseci_serv-1.4.0.9/jaseci_serv/user_api/tests/test_user_api.py` & `jaseci_serv-1.4.1.0/jaseci_serv/user_api/tests/test_user_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from rest_framework import status
 
 from jaseci.utils.utils import TestCaseHelper
 from django.test import TestCase
 
 from unittest.mock import MagicMock, Mock
 
-from jaseci_serv.svc import MetaService, MailService
-from jaseci_serv.svc.mail import MAIL_CONFIG
+from jaseci_serv.svc.mail_svc import MailService
+from jaseci.jsorc.jsorc import JsOrc
 
 
 # Consts for url
 CREATE_USER_URL = reverse("user_api:create")
 TOKEN_URL = reverse("user_api:token")
 MANAGE_URL = reverse("user_api:manage")
 LOGOUT_EVERYONE_URL = reverse("user_api:logout_everyone")
@@ -26,23 +26,20 @@
 get_user = get_user_model().objects.get
 
 
 class UserApiPublicTests(TestCaseHelper, TestCase):
     """Tests for user API (public)"""
 
     def __init__(self, *args, **kwargs):
-        MAIL_CONFIG["enabled"] = True
+        JsOrc.settings("MAIL_CONFIG")["enabled"] = True
         MailService.connect = MagicMock(return_value=Mock())
         super(UserApiPublicTests, self).__init__(*args, **kwargs)
 
     def setUp(self):
         super().setUp()
-        self.meta = MetaService()
-        self.hook = self.meta.build_hook()
-        self.meta.get_service("mail").reset(self.hook)
         self.client = APIClient()
 
     def tearDown(self):
         super().tearDown()
 
     def test_create_valid_user_success(self):
         """Test creating user with valid payload is successful"""
```

### Comparing `jaseci_serv-1.4.0.9/jaseci_serv/user_api/urls.py` & `jaseci_serv-1.4.1.0/jaseci_serv/user_api/urls.py`

 * *Files identical despite different names*

### Comparing `jaseci_serv-1.4.0.9/jaseci_serv/user_api/views.py` & `jaseci_serv-1.4.1.0/jaseci_serv/user_api/views.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 from django.contrib.auth import login, get_user_model
 from django.contrib.auth.signals import user_logged_out
 from knox.auth import TokenAuthentication
 
 from jaseci_serv.user_api.serializers import UserSerializer
 from jaseci_serv.user_api.serializers import SuperUserSerializer
 from jaseci_serv.user_api.serializers import AuthTokenSerializer
-from jaseci_serv.user_api.serializers import send_activation_email
 from jaseci_serv.base.models import lookup_global_config
 from datetime import timedelta
 
 from rest_framework.response import Response
 import base64
 
-from jaseci_serv.svc import MetaService
+from jaseci.jsorc.jsorc import JsOrc
+from jaseci.utils.utils import logger, ColCodes as Cc
 
 
 class CreateUserView(generics.CreateAPIView):
     """Create a new user in the system"""
 
     serializer_class = UserSerializer
 
@@ -62,16 +62,36 @@
 
     def post(self, request, format=None):
         serializer = AuthTokenSerializer(
             data=request.data, context={"request": request}
         )
         serializer.is_valid(raise_exception=True)
         user = serializer.validated_data["user"]
+        user_agent = request.META.get("HTTP_USER_AGENT", "")
+        log_str = f"Login request from {Cc.TG}{user}{Cc.EC} via {user_agent}"
+        log_dict = {
+            "api_name": "login",
+            "caller_name": str(user),
+            "request_user_agent": user_agent,
+        }
+        log_dict["extra_fields"] = list(log_dict.keys())
+        logger.info(log_str, extra=log_dict)
+
         login(request, user)
-        return super(CreateTokenView, self).post(request, format=None)
+        res = super(CreateTokenView, self).post(request, format=None)
+
+        log_str = f"Login success for {Cc.TG}{user}{Cc.EC} via {user_agent}"
+        log_dict = {
+            "api_name": "login",
+            "caller_name": str(user),
+            "request_user_agent": user_agent,
+        }
+        log_dict["extra_fields"] = list(log_dict.keys())
+        logger.info(log_str, extra=log_dict)
+        return res
 
 
 class ManageUserView(generics.RetrieveUpdateAPIView):
     """Manage the authenticated user"""
 
     # TODO: re-activate when user changes email address or disable email change
     serializer_class = UserSerializer
@@ -90,15 +110,15 @@
             "name": user.name,
             "is_activated": user.is_activated,
             "is_superuser": user.is_superuser,
         }
 
         response = self.update(request, *args, **kwargs)
 
-        elastic = MetaService().get_service("elastic")
+        elastic = JsOrc.svc("elastic")
         if elastic.is_running():
             activity = elastic.app.generate_from_request(request)
 
             user = response.data
 
             activity["misc"] = {
                 "old": current_user,
@@ -175,15 +195,15 @@
             return Response(status=status.HTTP_400_BAD_REQUEST)
 
         if self.update_field(
             user, request.data, {"is_activated": bool, "is_superuser": bool}
         ):
             user.save()
 
-            elastic = MetaService().get_service("elastic")
+            elastic = JsOrc.svc("elastic")
             if elastic.is_running():
                 activity = elastic.app.generate_from_request(request)
 
                 activity["misc"] = {
                     "old": current_user,
                     "new": {
                         "id": user.id,
```

### Comparing `jaseci_serv-1.4.0.9/jsserv` & `jaseci_serv-1.4.1.0/jsserv`

 * *Files identical despite different names*

