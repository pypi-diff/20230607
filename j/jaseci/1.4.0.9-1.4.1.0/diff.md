# Comparing `tmp/jaseci-1.4.0.9.tar.gz` & `tmp/jaseci-1.4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaseci-1.4.0.9.tar", last modified: Tue Feb 14 17:26:22 2023, max compression
+gzip compressed data, was "jaseci-1.4.1.0.tar", last modified: Wed Jun  7 18:24:54 2023, max compression
```

## Comparing `jaseci-1.4.0.9.tar` & `jaseci-1.4.1.0.tar`

### file list

```diff
@@ -1,231 +1,207 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:22.104182 jaseci-1.4.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-02-14 17:26:22.104182 jaseci-1.4.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:22.080181 jaseci-1.4.0.9/jaseci/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:22.080181 jaseci-1.4.0.9/jaseci/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9361 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/actions/live_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/actions/remote_actions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:22.084181 jaseci-1.4.0.9/jaseci/actions/standard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/actions/standard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/actions/standard/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/actions/standard/elastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/actions/standard/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/actions/standard/internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/actions/standard/jaseci.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/actions/standard/mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/actions/standard/net.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/actions/standard/rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/actions/standard/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/actions/standard/std.py
--rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/actions/standard/stripe.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/actions/standard/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:22.084181 jaseci-1.4.0.9/jaseci/actions/standard/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/actions/standard/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/actions/standard/tests/test_file_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/actions/standard/tests/test_mail_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/actions/standard/tests/test_net_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/actions/standard/tests/test_std_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/actions/standard/tests/test_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/actions/standard/tests/test_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/actions/standard/tests/test_webtool.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/actions/standard/tests/test_zlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/actions/standard/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/actions/standard/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/actions/standard/webtool.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/actions/standard/zlib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:22.084181 jaseci-1.4.0.9/jaseci/actions/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/actions/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/actions/tests/std_test_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/actions/tests/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/actions/tests/test_std.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:22.084181 jaseci-1.4.0.9/jaseci/actor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/actor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/actor/architype.py
--rw-r--r--   0 runner    (1001) docker     (123)     9304 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/actor/sentinel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8299 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/actor/walker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:22.088181 jaseci-1.4.0.9/jaseci/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/api/actions_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/api/alias_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/api/architype_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/api/config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/api/global_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/api/graph_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9591 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/api/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/api/jac_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10609 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/api/jsorc_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/api/logger_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/api/master_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/api/object_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/api/prometheus_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/api/queue_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9626 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/api/sentinel_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/api/super_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:22.088181 jaseci-1.4.0.9/jaseci/api/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/api/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/api/tests/test_architype_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/api/tests/test_global_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/api/tests/test_graph_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/api/tests/test_logger_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/api/tests/test_sentinel_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/api/tests/test_user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11782 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/api/tests/test_walker_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/api/user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8732 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/api/walker_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/api/webhook_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:22.088181 jaseci-1.4.0.9/jaseci/attr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/attr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/attr/action.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/attr/item.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:22.092181 jaseci-1.4.0.9/jaseci/element/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/element/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/element/element.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/element/master.py
--rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/element/obj_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/element/super_master.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:22.092181 jaseci-1.4.0.9/jaseci/graph/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/graph/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    17719 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/graph/node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:22.092181 jaseci-1.4.0.9/jaseci/hook/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/hook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/hook/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/hook/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:22.092181 jaseci-1.4.0.9/jaseci/jac/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/jac/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:22.092181 jaseci-1.4.0.9/jaseci/jac/interpreter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/jac/interpreter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/jac/interpreter/architype_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)    70340 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/jac/interpreter/interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/jac/interpreter/sentinel_interp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:22.092181 jaseci-1.4.0.9/jaseci/jac/interpreter/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/jac/interpreter/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/jac/interpreter/tests/test_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/jac/interpreter/walker_interp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:22.092181 jaseci-1.4.0.9/jaseci/jac/ir/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/jac/ir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/jac/ir/ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/jac/ir/ast_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/jac/ir/jac_code.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:22.092181 jaseci-1.4.0.9/jaseci/jac/ir/passes/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/jac/ir/passes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/jac/ir/passes/ast_prune_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/jac/ir/passes/codegen_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/jac/ir/passes/ir_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/jac/ir/passes/printer_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/jac/ir/passes/pt_prune_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/jac/ir/passes/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/jac/ir/passes/stats_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)     8925 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/jac/jac.g4
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:22.096181 jaseci-1.4.0.9/jaseci/jac/jac_parse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/jac/jac_parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34691 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/jac/jac_parse/jacLexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    29061 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/jac/jac_parse/jacListener.py
--rw-r--r--   0 runner    (1001) docker     (123)   333597 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/jac/jac_parse/jacParser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/jac/jac_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:22.096181 jaseci-1.4.0.9/jaseci/jac/jsci_vm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/jac/jsci_vm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/jac/jsci_vm/disasm.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/jac/jsci_vm/inst_ptr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/jac/jsci_vm/machine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/jac/jsci_vm/op_codes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:22.096181 jaseci-1.4.0.9/jaseci/jac/jsci_vm/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/jac/jsci_vm/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/jac/jsci_vm/tests/test_codegen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:22.096181 jaseci-1.4.0.9/jaseci/jac/machine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/jac/machine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/jac/machine/jac_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/jac/machine/jac_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     9171 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/jac/machine/machine_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:22.096181 jaseci-1.4.0.9/jaseci/jac/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/jac/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13323 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/jac/tests/book_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    13884 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/jac/tests/test_book.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/jac/tests/test_lang_14.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:22.096181 jaseci-1.4.0.9/jaseci/jsctl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/jsctl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16114 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/jsctl/book_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    12246 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/jsctl/jsctl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:22.096181 jaseci-1.4.0.9/jaseci/jsctl/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/jsctl/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20339 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/jsctl/tests/test_jsctl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:22.096181 jaseci-1.4.0.9/jaseci/svc/
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/svc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:22.100181 jaseci-1.4.0.9/jaseci/svc/actions_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/svc/actions_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21169 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/svc/actions_optimizer/actions_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/svc/actions_optimizer/actions_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    27118 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/svc/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/svc/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:22.100181 jaseci-1.4.0.9/jaseci/svc/elastic/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/svc/elastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/svc/elastic/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/svc/elastic/elastic.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/svc/elastic/manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:22.100181 jaseci-1.4.0.9/jaseci/svc/jsorc-backup/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/svc/jsorc-backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/svc/jsorc-backup/jaseci-redis.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/svc/jsorc-backup/jsorc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:22.100181 jaseci-1.4.0.9/jaseci/svc/jsorc-backup/promon/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/svc/jsorc-backup/promon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/svc/jsorc-backup/promon/promon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:22.100181 jaseci-1.4.0.9/jaseci/svc/mail/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/svc/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/svc/mail/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/svc/mail/mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/svc/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:22.100181 jaseci-1.4.0.9/jaseci/svc/postgres/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/svc/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/svc/postgres/manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:22.100181 jaseci-1.4.0.9/jaseci/svc/prometheus/
--rwxr-xr-x   0 runner    (1001) docker     (123)       82 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/svc/prometheus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/svc/prometheus/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    53949 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/svc/prometheus/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9888 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/svc/prometheus/prometheus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:22.100181 jaseci-1.4.0.9/jaseci/svc/redis/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/svc/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/svc/redis/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/svc/redis/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/svc/redis/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/svc/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:22.100181 jaseci-1.4.0.9/jaseci/svc/stripe/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/svc/stripe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/svc/stripe/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/svc/stripe/stripe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:22.100181 jaseci-1.4.0.9/jaseci/svc/task/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/svc/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/svc/task/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/svc/task/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/svc/task/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:22.104182 jaseci-1.4.0.9/jaseci/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/tests/infer.py
--rw-r--r--   0 runner    (1001) docker     (123)    25194 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/tests/jac_test_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    13249 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/tests/jac_test_progs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    32292 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/tests/test_jac.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/tests/test_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    22073 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/tests/test_progs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/tests/test_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/tests/test_stripe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:22.104182 jaseci-1.4.0.9/jaseci/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/utils/id_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/utils/json_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/utils/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/jaseci/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:22.080181 jaseci-1.4.0.9/jaseci.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-02-14 17:26:22.000000 jaseci-1.4.0.9/jaseci.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-02-14 17:26:22.000000 jaseci-1.4.0.9/jaseci.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-14 17:26:22.000000 jaseci-1.4.0.9/jaseci.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-02-14 17:26:22.000000 jaseci-1.4.0.9/jaseci.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-02-14 17:26:22.000000 jaseci-1.4.0.9/jaseci.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-14 17:26:22.000000 jaseci-1.4.0.9/jaseci.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-14 17:26:22.104182 jaseci-1.4.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-02-14 17:25:56.000000 jaseci-1.4.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.739014 jaseci-1.4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-07 18:24:54.739014 jaseci-1.4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.719014 jaseci-1.4.1.0/jaseci/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.719014 jaseci-1.4.1.0/jaseci/cli_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/cli_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16103 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/cli_tools/book_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14384 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/cli_tools/jsctl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.719014 jaseci-1.4.1.0/jaseci/cli_tools/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/cli_tools/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21217 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/cli_tools/tests/test_jsctl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.719014 jaseci-1.4.1.0/jaseci/extens/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.723014 jaseci-1.4.1.0/jaseci/extens/act_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/elastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/jaseci.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7162 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/std.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/stripe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.723014 jaseci-1.4.1.0/jaseci/extens/act_lib/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/tests/std_test_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/tests/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/tests/test_elastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/tests/test_file_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/tests/test_mail_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/tests/test_net_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/tests/test_regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/tests/test_std.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/tests/test_std_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/tests/test_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/tests/test_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/tests/test_webtool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/tests/test_zlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/webtool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/act_lib/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.727014 jaseci-1.4.1.0/jaseci/extens/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6923 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/actions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/alias_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7237 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/architype_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/global_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/graph_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9587 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5816 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/jac_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9991 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/jsorc_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/logger_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/master_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/object_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/prometheus_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/queue_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9632 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/sentinel_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/super_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.727014 jaseci-1.4.1.0/jaseci/extens/api/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/tests/test_architype_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/tests/test_global_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/tests/test_graph_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/tests/test_logger_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/tests/test_object_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/tests/test_sentinel_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/tests/test_user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12622 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/tests/test_walker_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9556 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/walker_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/api/webhook_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.727014 jaseci-1.4.1.0/jaseci/extens/svc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/svc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12501 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/svc/elastic_svc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15612 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/svc/kube_svc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/svc/mail_svc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/svc/prome_svc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/svc/redis_svc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/svc/stripe_svc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/svc/task_svc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10351 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/extens/svc/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.727014 jaseci-1.4.1.0/jaseci/jac/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.731014 jaseci-1.4.1.0/jaseci/jac/interpreter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/interpreter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/interpreter/architype_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66659 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/interpreter/interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/interpreter/sentinel_interp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.731014 jaseci-1.4.1.0/jaseci/jac/interpreter/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/interpreter/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/interpreter/tests/test_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8503 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/interpreter/walker_interp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.731014 jaseci-1.4.1.0/jaseci/jac/ir/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/ir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/ir/ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/ir/ast_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/ir/jac_code.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.731014 jaseci-1.4.1.0/jaseci/jac/ir/passes/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/ir/passes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/ir/passes/ast_prune_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/ir/passes/codegen_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/ir/passes/ir_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/ir/passes/printer_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/ir/passes/pt_prune_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/ir/passes/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/ir/passes/stats_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8916 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/jac.g4
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.731014 jaseci-1.4.1.0/jaseci/jac/jac_parse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/jac_parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34691 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/jac_parse/jacLexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29031 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/jac_parse/jacListener.py
+-rw-r--r--   0 runner    (1001) docker     (123)   334026 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/jac_parse/jacParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/jac_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.731014 jaseci-1.4.1.0/jaseci/jac/jsci_vm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/jsci_vm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/jsci_vm/disasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/jsci_vm/inst_ptr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/jsci_vm/machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/jsci_vm/op_codes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.731014 jaseci-1.4.1.0/jaseci/jac/jsci_vm/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/jsci_vm/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/jsci_vm/tests/test_codegen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.731014 jaseci-1.4.1.0/jaseci/jac/machine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/machine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/machine/jac_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/machine/jac_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/machine/machine_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.735014 jaseci-1.4.1.0/jaseci/jac/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13323 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/tests/book_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13870 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/tests/test_book.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jac/tests/test_lang_14.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.735014 jaseci-1.4.1.0/jaseci/jsorc/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jsorc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21601 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jsorc/jsorc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jsorc/jsorc_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8945 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jsorc/jsorc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jsorc/live_actions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.735014 jaseci-1.4.1.0/jaseci/jsorc/manifests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jsorc/manifests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jsorc/manifests/database.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   484138 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jsorc/manifests/elastic.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    37855 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jsorc/manifests/prometheus.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jsorc/manifests/redis.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jsorc/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jsorc/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jsorc/remote_actions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.735014 jaseci-1.4.1.0/jaseci/jsorc/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jsorc/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jsorc/tests/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/jsorc/tests/test_jsorc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.735014 jaseci-1.4.1.0/jaseci/prim/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/prim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/prim/ability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/prim/architype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/prim/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/prim/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/prim/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/prim/master.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17712 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/prim/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/prim/obj_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/prim/sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/prim/super_master.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/prim/walker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.739014 jaseci-1.4.1.0/jaseci/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/tests/infer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25194 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/tests/jac_test_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14396 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/tests/jac_test_progs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31674 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/tests/test_jac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/tests/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24345 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/tests/test_progs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/tests/test_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8096 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/tests/test_stripe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.739014 jaseci-1.4.1.0/jaseci/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.739014 jaseci-1.4.1.0/jaseci/utils/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/utils/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/utils/actions/actions_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21564 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/utils/actions/actions_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/utils/actions/actions_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)   119142 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/utils/gprof2dot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/utils/id_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/utils/json_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/utils/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10234 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/jaseci/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:54.719014 jaseci-1.4.1.0/jaseci.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-07 18:24:54.000000 jaseci-1.4.1.0/jaseci.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-06-07 18:24:54.000000 jaseci-1.4.1.0/jaseci.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 18:24:54.000000 jaseci-1.4.1.0/jaseci.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-07 18:24:54.000000 jaseci-1.4.1.0/jaseci.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-07 18:24:54.000000 jaseci-1.4.1.0/jaseci.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-07 18:24:54.000000 jaseci-1.4.1.0/jaseci.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 18:24:54.739014 jaseci-1.4.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-07 18:24:38.000000 jaseci-1.4.1.0/setup.py
```

### Comparing `jaseci-1.4.0.9/LICENSE` & `jaseci-1.4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.0.9/jaseci/actions/live_actions.py` & `jaseci-1.4.1.0/jaseci/jsorc/live_actions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 """
 General action base class with automation for hot loading
 """
 from importlib.util import spec_from_file_location, module_from_spec
 from jaseci.utils.utils import logger
-from jaseci.actions.remote_actions import ACTIONS_SPEC_LOC
-from jaseci.actions.remote_actions import serv_actions, mark_as_remote, mark_as_endpoint
+from jaseci.jsorc.remote_actions import ACTIONS_SPEC_LOC
+from jaseci.jsorc.remote_actions import serv_actions, mark_as_remote, mark_as_endpoint
 import requests
 import os
 import sys
 import inspect
 import importlib
 import gc
 
 live_actions = {}  # {"act.func": func_obj, ...}
 live_action_modules = {}  # {__module__: ["act.func1", "act.func2", ...], ...}
 action_configs = {}  # {"module_name": {}, ...}
 
+glob_act_group = {}  # {"group_name": {"act_name": action, ...}, ...}
+glob_act_hook = None
+
 
 def jaseci_action(act_group=None, aliases=list(), allow_remote=False):
     """Decorator for Jaseci Action interface"""
     caller_globals = dict(inspect.getmembers(inspect.currentframe().f_back))[
         "f_globals"
     ]
     if allow_remote and "serv_actions" not in caller_globals:
@@ -66,15 +69,15 @@
                     f"{'.'.join(act_group+[i])}"
                 )
             else:
                 live_action_modules[func.__module__] = [f"{'.'.join(act_group+[i])}"]
     return func
 
 
-def load_local_actions(file: str):
+def load_local_actions(file: str, ctx: dict = {}):
     """Load all jaseci actions from python file"""
     try:
         name = file.rstrip(".py")
         name = ".".join(name.split("/")[-2:])
         # Assumes parent folder of py file is a package for internal relative
         # imports, name is package.module and package path is added to sys path
         spec = spec_from_file_location(name, str(file))
@@ -83,21 +86,29 @@
             return False
         else:
             module_dir = os.path.dirname(os.path.dirname(os.path.realpath(file)))
             if module_dir not in sys.path:
                 sys.path.append(module_dir)
             mod = module_from_spec(spec)
             spec.loader.exec_module(mod)
+            try:
+                if hasattr(mod, "setup"):
+                    mod.setup(**ctx)
+            except Exception as e:
+                logger.error(
+                    f"Cannot run set up for module {mod}. This could be because the module doesn't have a setup procedure for initialization, or wrong setup parameters are provided."
+                )
+                logger.error(e)
             return True
-    except Exception:
-        logger.error(f"Cannot hot load local actions from {file}.")
+    except Exception as e:
+        logger.error(f"Cannot hot load local actions from {file}: {e}")
         return False
 
 
-def load_module_actions(mod, loaded_module=None):
+def load_module_actions(mod, loaded_module=None, ctx: dict = {}):
     """Load all jaseci actions from python module"""
     try:
         if mod in sys.modules:
             del sys.modules[mod]
         if loaded_module and loaded_module in sys.modules:
             del sys.modules[loaded_module]
         if mod in live_action_modules:
@@ -106,18 +117,26 @@
                     del live_actions[i]
         if loaded_module in live_action_modules:
             for i in live_action_modules[loaded_module]:
                 if i in live_actions:
                     del live_actions[i]
 
         mod = importlib.import_module(mod)
+        try:
+            if hasattr(mod, "setup"):
+                mod.setup(**ctx)
+        except Exception as e:
+            logger.error(
+                f"Cannot run set up for module {mod}. This could be because the module doesn't have a setup procedure for initialization, or wrong setup parameters are provided."
+            )
+            logger.error(e)
         if mod:
             return True
-    except Exception:
-        logger.error(f"Cannot hot load module actions from {mod}.")
+    except Exception as e:
+        logger.error(f"Cannot hot load module actions from {mod}: {e}")
 
     return False
 
 
 def load_action_config(config, module_name):
     """
     Load the action config of a jaseci action module
@@ -195,45 +214,48 @@
 
 
 def get_global_actions():
     """
     Loads all global action hooks for use by Jac programs
     Attaches globals to mem_hook
     """
-    from jaseci.attr.action import Action
-    from jaseci.hook.memory import MemoryHook
+    from jaseci.prim.ability import Ability
+    from jaseci.jsorc.memory import MemoryHook
 
-    global_action_list = []
-    hook = MemoryHook()
-    for i in live_actions.keys():
-        if (
-            i.startswith("std.")
-            or i.startswith("file.")
-            or i.startswith("net.")
-            or i.startswith("rand.")
-            or i.startswith("vector.")
-            or i.startswith("request.")
-            or i.startswith("date.")
-            or i.startswith("jaseci.")
-            or i.startswith("internal.")
-            or i.startswith("zlib.")
-            or i.startswith("webtool.")
-            or i.startswith("url.")
-        ):
-            global_action_list.append(
-                Action(
+    if not glob_act_group:
+        glob_act_hook = MemoryHook()
+        for i in live_actions.keys():
+            name = i.split(".")
+            if name[0] in [
+                "std",
+                "file",
+                "net",
+                "rand",
+                "vector",
+                "request",
+                "date",
+                "jaseci",
+                "internal",
+                "zip",
+                "webtool",
+                "url",
+                "regex",
+            ]:
+                if name[0] not in glob_act_group:
+                    glob_act_group[name[0]] = {}
+                glob_act_group[name[0]][name[1]] = Ability(
                     m_id=0,
-                    h=hook,
+                    h=glob_act_hook,
                     mode="public",
                     name=i,
+                    kind="ability",
                     value=i,
                     persist=False,
                 )
-            )
-    return global_action_list
+    return glob_act_group
 
 
 def unload_remote_actions(url):
     """
     Get the list of actions from the given URL and then unload them.
     """
     headers = {"content-type": "application/json"}
@@ -243,22 +265,30 @@
         for i in spec.keys():
             unload_action(i)
         return True
     except Exception as e:
         logger.error(f"Cannot unload remote action from {url}: {e}")
 
 
-def load_remote_actions(url):
+def load_remote_actions(url, ctx: dict = {}):
     """Load all jaseci actions from live pod"""
     headers = {"content-type": "application/json"}
     try:
         spec = requests.get(url.rstrip("/") + ACTIONS_SPEC_LOC, headers=headers)
         spec = spec.json()
         for i in spec.keys():
             live_actions[i] = gen_remote_func_hook(url, i, spec[i])
+            if i.endswith(".setup") and ctx:
+                try:
+                    live_actions[i](**ctx)
+                except Exception as e:
+                    logger.error(
+                        f"Cannot run set up for remote action {i}. This could be because the module doesn't have a setup procedure for initialization, or wrong setup parameters are provided."
+                    )
+                    logger.error(e)
         return True
 
     except Exception as e:
         logger.error(f"Cannot hot load remote actions at {url}: {e}")
         return False
 
 
@@ -271,16 +301,34 @@
             if i < len(args):
                 params[param_names[i]] = args[i]
             else:
                 params[param_names[i]] = None
         for i in kwargs.keys():
             if i in param_names:
                 params[i] = kwargs[i]
+        # Remove any None-valued parameters to use the default value of the action def
+        params = dict([(k, v) for k, v in params.items() if v is not None])
         act_url = f"{url.rstrip('/')}/{act_name.split('.')[-1]}"
         res = requests.post(
             act_url, headers={"content-type": "application/json"}, json=params
         )
         return res.json()
 
     func.__module__ = "js_remote_hook"
 
     return func
+
+
+def call_action(action_name: str, ctx: dict = {}) -> None:
+    """
+    Call an action by name
+    """
+    try:
+        action_name = action_name.strip()
+        if action_name in live_actions.keys():
+            res = live_actions[action_name](**ctx)
+            return res, True
+        else:
+            raise Exception(f"Action {action_name} not found")
+    except Exception as e:
+        logger.error(f"Error calling action {action_name}: {e}")
+        return None, False
```

### Comparing `jaseci-1.4.0.9/jaseci/actions/remote_actions.py` & `jaseci-1.4.1.0/jaseci/jsorc/remote_actions.py`

 * *Files 7% similar despite different names*

```diff
@@ -58,38 +58,40 @@
         else act_group
     )
     remote_actions[f"{'.'.join(act_group+[func.__name__])}"] = varnames
 
     # Need to get pydatic model for func signature for fastAPI post
     model = validate_arguments(func).model
 
-    # Keep only feilds present in param list in base model
+    # Keep only fields present in param list in base model
     keep_fields = {}
     for i in model.__fields__.keys():
         if i in varnames:
             keep_fields[i] = model.__fields__[i]
     model.__fields__ = keep_fields
 
     # Create duplicate funtion for api endpoint and inject in call site globals
     @app.post(f"/{func.__name__}/")
-    def new_func(params: model):
+    def new_func(params: model = model.construct()):
         pl_peek = str(dict(params.__dict__))[:128]
         logger.info(str(f"Incoming call to {func.__name__} with {pl_peek}"))
         start_time = time()
 
         ret = validate_arguments(func)(**(params.__dict__))
         tot_time = time() - start_time
         logger.info(
             str(
                 f"API call to {Cc.TG}{func.__name__}{Cc.EC}"
                 f" completed in {Cc.TY}{tot_time:.3f} seconds{Cc.EC}"
             )
         )
         return ret
 
+    if func.__name__ == "setup":
+        new_func = app.on_event("startup")(new_func)
     for i in aliases:
         new_func = app.post(f"/{i}/")(new_func)
         remote_actions[f"{'.'.join(act_group+[i])}"] = varnames
     caller_globals[f"{JS_ACTION_PREAMBLE}{func.__name__}"] = new_func
 
 
 def gen_endpoint(app, func, endpoint, mount, caller_globals):
```

### Comparing `jaseci-1.4.0.9/jaseci/actions/standard/date.py` & `jaseci-1.4.1.0/jaseci/extens/act_lib/date.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Built in actions for Jaseci"""
-from datetime import datetime
-from datetime import timedelta
-from jaseci.actions.live_actions import jaseci_action
+from datetime import datetime, timedelta
+from jaseci.jsorc.live_actions import jaseci_action
+from dateutil.relativedelta import relativedelta
 
 
 @jaseci_action()
 def quantize_to_year(date: str):
     date = datetime.fromisoformat(date)
     date = date.replace(month=1, day=1, hour=0, minute=0, second=0, microsecond=0)
     return date.isoformat()
@@ -31,31 +31,80 @@
     date = datetime.fromisoformat(date)
     date = date.replace(hour=0, minute=0, second=0, microsecond=0)
     return date.isoformat()
 
 
 @jaseci_action()
 def datetime_now():
-    """Get utc date time for now in iso format"""
+    """Get utc date time now in iso format"""
     return datetime.utcnow().isoformat()
 
 
 @jaseci_action()
 def date_now():
-    """Get utc date time for now in iso format"""
+    """Get utc date now in iso format"""
     return datetime.utcnow().date().isoformat()
 
 
 @jaseci_action()
 def timestamp_now():
     """Get utc date time for now in iso format"""
     return int(datetime.utcnow().timestamp())
 
 
 @jaseci_action()
+def datetime_obj(date: str = None):
+    """Get utc date time now or parse one to dict format"""
+    if date:
+        date = datetime.fromisoformat(date)
+    else:
+        date = datetime.utcnow()
+
+    return {
+        "year": date.year,
+        "month": date.month,
+        "weekday": date.isoweekday(),
+        "day": date.day,
+        "hour": date.hour,
+        "minute": date.minute,
+        "second": date.second,
+        "microsecond": date.microsecond,
+        "iso": date.isoformat(),
+    }
+
+
+@jaseci_action()
+def datetime_add(date: str = None, **kwargs):
+    """
+    Get utc date time now or parse one then add timedelta
+    kwargs: this should be valid timedelta arguments
+    """
+    if date:
+        date = datetime.fromisoformat(date)
+    else:
+        date = datetime.utcnow()
+
+    return (date + relativedelta(**kwargs)).isoformat()
+
+
+@jaseci_action()
+def datetime_sub(date: str = None, **kwargs):
+    """
+    Get utc date time now or parse one then subtract timedelta
+    kwargs: this should be valid timedelta arguments
+    """
+    if date:
+        date = datetime.fromisoformat(date)
+    else:
+        date = datetime.utcnow()
+
+    return (date - relativedelta(**kwargs)).isoformat()
+
+
+@jaseci_action()
 def date_day_diff(start_date: str, end_date: str = None):
     # Try to deal with some incompatible date in old nodes
     # Due date has not been saving in isoformat so this doesn't work
     # for example,'2021-03-31T04:00:00.000Z'
     start_date = datetime.fromisoformat(start_date.split("T")[0])
 
     if end_date is None:
```

### Comparing `jaseci-1.4.0.9/jaseci/actions/standard/elastic.py` & `jaseci-1.4.1.0/jaseci/extens/act_lib/elastic.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,24 @@
-from jaseci.actions.live_actions import jaseci_action
-from jaseci.svc import MetaService
+from jaseci.jsorc.live_actions import jaseci_action
+from jaseci.jsorc.jsorc import JsOrc
+from jaseci.extens.svc.elastic_svc import ElasticService, Elastic
 
 
 def elastic():
-    return MetaService().get_service("elastic").poke()
+    return JsOrc.svc("elastic", ElasticService).poke(Elastic)
+
+
+@jaseci_action()
+def _post(url: str, json: dict = {}):
+    return elastic()._post(url, json)
+
+
+@jaseci_action()
+def _get(url: str, json: dict = None):
+    return elastic()._get(url, json)
 
 
 @jaseci_action()
 def post(url: str, body: dict, index: str = "", suffix: str = ""):
     return elastic().post(url, body, index, suffix)
 
 
@@ -53,14 +64,24 @@
 
 @jaseci_action()
 def mapping_activity(query: str = "", suffix: str = ""):
     return elastic().mapping_activity(query, suffix)
 
 
 @jaseci_action()
+def refresh(index: str = "", suffix: str = ""):
+    return elastic().refresh(index, suffix)
+
+
+@jaseci_action()
+def refresh_activity(suffix: str = ""):
+    return elastic().refresh_activity(suffix)
+
+
+@jaseci_action()
 def aliases(query: str = "pretty=true"):
     return elastic().aliases(query)
 
 
 @jaseci_action()
 def reindex(body: dict, query: str = "pretty"):
     return elastic().reindex(body, query)
```

### Comparing `jaseci-1.4.0.9/jaseci/actions/standard/file.py` & `jaseci-1.4.1.0/jaseci/extens/act_lib/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Built in actions for Jaseci"""
-from jaseci.actions.live_actions import jaseci_action
+from jaseci.jsorc.live_actions import jaseci_action
 import os
 import json
 import base64
 
 
 @jaseci_action()
 def load_str(fn: str, max_chars: int = None):
```

### Comparing `jaseci-1.4.0.9/jaseci/actions/standard/jaseci.py` & `jaseci-1.4.1.0/jaseci/extens/act_lib/jaseci.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Built in actions for Jaseci"""
-from jaseci.actions.live_actions import jaseci_action
+from jaseci.jsorc.live_actions import jaseci_action
 from jaseci.utils.utils import master_from_meta, copy_func
-from jaseci.element.super_master import SuperMaster
+from jaseci.prim.super_master import SuperMaster
 import functools
 
 
 def interface_api(api_name, is_public, p_spec, *args, meta):
     """
     Interfaces Master apis after processing arguments/parameters
     from cli
```

### Comparing `jaseci-1.4.0.9/jaseci/actions/standard/net.py` & `jaseci-1.4.1.0/jaseci/extens/act_lib/net.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 
 This library of actions cover the standard operations that can be
 run on graph elements (nodes and edges). A number of these actions
 accept lists that are exclusively composed of instances of defined
 architype node and/or edges. Keep in mind that a \\lstinline{jac_set}
 is simply a list that only contains such elements.
 """
-from jaseci.actions.live_actions import jaseci_action
+from jaseci.jsorc.live_actions import jaseci_action
 from jaseci.utils.utils import master_from_meta
 from jaseci.jac.jac_set import JacSet
-from jaseci.graph.node import Node
-from jaseci.graph.edge import Edge
+from jaseci.prim.node import Node
+from jaseci.prim.edge import Edge
 import uuid
 
 
 @jaseci_action()
 def max(item_set: JacSet):
     """
     Max based on anchor value
```

### Comparing `jaseci-1.4.0.9/jaseci/actions/standard/rand.py` & `jaseci-1.4.1.0/jaseci/extens/act_lib/rand.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Built in actions for Jaseci"""
 import random
 
 # import faker
 from datetime import datetime
 from datetime import timedelta
-from jaseci.actions.live_actions import jaseci_action
+from jaseci.jsorc.live_actions import jaseci_action
 
 lorem_words = (
     "adipisci aliquam amet consectetur dolor dolore dolorem eius "
     "est et incidunt ipsum labore magnam modi neque non numquam "
     "porro quaerat qui quia quisquam sed sit tempora ut velit "
     "voluptatem"
 ).split()
```

### Comparing `jaseci-1.4.0.9/jaseci/actions/standard/request.py` & `jaseci-1.4.1.0/jaseci/extens/act_lib/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Built in actions for Jaseci"""
 import requests
-from jaseci.actions.live_actions import jaseci_action
+from jaseci.jsorc.live_actions import jaseci_action
 from base64 import b64decode, b64encode
 from io import BytesIO
 
 
 @jaseci_action()
 def get(url: str, data: dict, header: dict):
     """
```

### Comparing `jaseci-1.4.0.9/jaseci/actions/standard/std.py` & `jaseci-1.4.1.0/jaseci/extens/act_lib/std.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """Built in actions for Jaseci"""
 from operator import itemgetter
 from jaseci.utils.utils import app_logger, json_out
 from datetime import datetime
 from jaseci.jac.machine.jac_value import jac_wrap_value as jwv
-from jaseci.actions.live_actions import jaseci_action
+from jaseci.jsorc.live_actions import jaseci_action
 from jaseci.utils.utils import master_from_meta
-from jaseci.element.element import Element
-from jaseci.svc import MetaService
+from jaseci.prim.element import Element
+from jaseci.jsorc.jsorc import JsOrc
+from jaseci.extens.svc.elastic_svc import Elastic
 
 import sys
 import json
+import time
 
 
 @jaseci_action()
 def log(*args):
     """Standard built in for printing output to log"""
     result = ""
     for i in args:
@@ -45,14 +47,20 @@
 def err(*args):
     """Standard built in for printing to stderr"""
     args = [json_out(jwv(x)) for x in args]
     print(*args, file=sys.stderr)
 
 
 @jaseci_action()
+def sleep(secs: float):
+    """Standard built in for sleep"""
+    return time.sleep(secs)
+
+
+@jaseci_action()
 def sort_by_col(lst: list, col_num: int, reverse: bool = False):
     """
     Sorts in place list of lists by column
     Param 1 - list
     Param 2 - col number
     Param 3 - boolean as to whether things should be reversed
 
@@ -208,13 +216,13 @@
     meta["interp"].report = []
     if hasattr(meta["interp"], "save"):
         meta["interp"].save()
 
 
 @jaseci_action()
 def log_activity(
-    log: dict, action: str = "", query: str = "", suffix: str = "", meta: dict = {}
+    log: dict = {}, action: str = "", query: str = "", suffix: str = "", meta: dict = {}
 ):
-    elastic = MetaService().get_service("elastic").poke()
-    activity = elastic.generate_from_meta(meta, log)
+    elastic = JsOrc.svc("elastic").poke(Elastic)
+    activity = elastic.generate_from_meta(meta, log, action)
 
     return elastic.doc_activity(activity, query, suffix)
```

### Comparing `jaseci-1.4.0.9/jaseci/actions/standard/stripe.py` & `jaseci-1.4.1.0/jaseci/extens/act_lib/stripe.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Built in actions for Jaseci"""
 import stripe as s
 
-from jaseci.svc import MetaService
+from jaseci.jsorc.jsorc import JsOrc
+from jaseci.extens.svc.stripe_svc import StripeService
 from datetime import datetime
-from jaseci.actions.live_actions import jaseci_action
+from jaseci.jsorc.live_actions import jaseci_action
 
 
 def stripe() -> s:
-    return MetaService().get_service("stripe").poke()
+    return JsOrc.svc("stripe", StripeService).poke()
 
 
 @jaseci_action()
 def create_product(name: str, description: str, **kwargs):
     """create product"""
 
     return stripe().Product.create(name=name, description=description, **kwargs)
```

### Comparing `jaseci-1.4.0.9/jaseci/actions/standard/tests/test_file_lib.py` & `jaseci-1.4.1.0/jaseci/extens/act_lib/tests/test_file_lib.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.0.9/jaseci/actions/standard/tests/test_net_lib.py` & `jaseci-1.4.1.0/jaseci/extens/act_lib/tests/test_net_lib.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.0.9/jaseci/actions/standard/tests/test_std_lib.py` & `jaseci-1.4.1.0/jaseci/extens/act_lib/tests/test_std_lib.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,17 @@
         ret = self.call(
             self.mast,
             ["sentinel_register", {"code": self.load_jac("general.jac")}],
         )
         ret = self.call(self.mast, ["walker_run", {"name": "internal_lib"}])
         self.assertEqual(len(ret["report"]), 1)
         self.assertTrue(
-            ret["report"][0].startswith("ncalls,tottime,percall,cumtime,percall,")
+            ret["report"][0]["calls"].startswith(
+                "ncalls,tottime,percall,cumtime,percall,"
+            )
         )
 
     def test_rand_float_round(self):
         ret = self.call(
             self.mast,
             ["sentinel_register", {"code": self.load_jac("general.jac")}],
         )
```

### Comparing `jaseci-1.4.0.9/jaseci/actions/standard/tests/test_url.py` & `jaseci-1.4.1.0/jaseci/extens/act_lib/tests/test_url.py`

 * *Files 27% similar despite different names*

```diff
@@ -16,19 +16,16 @@
         self.assertEqual(
             ret["report"],
             [True, False, False, False],
         )
 
     @jac_testcase("url.jac", "download_text_test")
     def test_download_text(self, ret):
-        # Jaseci home page is 170,193 bytes in html
-        # HTML pages change, so we'll allow a 1% tolerance
-        diff = abs(len(ret["report"][0]) - 170193)
-        diff_percentange = diff / 170193
-        self.assertTrue(diff_percentange <= 0.01)
+        # Download the jaseci homepage as a test
+        self.assertGreater(abs(len(ret["report"][0])), 0)
 
     @jac_testcase("url.jac", "download_b64_test")
     def test_download_b64(self, ret):
         # Jaseci white paper is 2,034,680 bytes in base64
         self.assertEqual(
             len(ret["report"][0]),
             2034680,
```

### Comparing `jaseci-1.4.0.9/jaseci/actions/standard/tests/test_vector.py` & `jaseci-1.4.1.0/jaseci/extens/act_lib/tests/test_vector.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.0.9/jaseci/actions/standard/tests/test_webtool.py` & `jaseci-1.4.1.0/jaseci/extens/act_lib/tests/test_webtool.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,23 +5,40 @@
     """UnitTest for Webtool"""
 
     fixture_src = __file__
 
     @jac_testcase("webtool.jac", "get_meta_valid")
     def test_get_meta_valid(self, ret):
         self.assertTrue(ret["success"])
-        self.assertTrue("og" in ret["report"][0])
-        self.assertTrue("meta" in ret["report"][0])
-        self.assertTrue("dc" in ret["report"][0])
-        self.assertTrue("page" in ret["report"][0])
+        expected_tags = set(["og:image", "og:type", "og:title"])
+        tags = set(
+            [
+                meta["property"] if "property" in meta else ""
+                for meta in ret["report"][0]
+            ]
+        )
+        self.assertTrue(tags.issuperset(expected_tags))
 
-    @jac_testcase("webtool.jac", "get_meta_403_response")
-    def test_get_meta_403_response(self, ret):
+    @jac_testcase("webtool.jac", "get_meta_need_auth")
+    def test_get_meta_need_auth(self, ret):
         self.assertTrue(ret["success"])
-        self.assertTrue("og" in ret["report"][0])
-        self.assertTrue("meta" in ret["report"][0])
-        self.assertTrue("dc" in ret["report"][0])
-        self.assertTrue("page" in ret["report"][0])
+        self.assertTrue(len(ret["report"][0]) > 0)
 
     @jac_testcase("webtool.jac", "get_meta_invalid")
     def test_get_meta_invalid(self, ret):
-        self.assertFalse(ret["success"])
+        self.assertTrue("Failed at getting metadata" in ret["report"][0])
+
+    @jac_testcase("webtool.jac", "get_meta_timeout")
+    def test_get_meta_timeout(self, ret):
+        self.assertTrue("Failed at getting metadata" in ret["report"][0])
+
+    @jac_testcase("webtool.jac", "get_meta_need_header")
+    def test_get_meta_need_header(self, ret):
+        self.assertTrue(ret["success"])
+        expected_tags = set(["og:image", "og:type", "og:title"])
+        tags = set(
+            [
+                meta["property"] if "property" in meta else ""
+                for meta in ret["report"][0]
+            ]
+        )
+        self.assertTrue(tags.issuperset(expected_tags))
```

### Comparing `jaseci-1.4.0.9/jaseci/actions/standard/tests/test_zlib.py` & `jaseci-1.4.1.0/jaseci/extens/act_lib/tests/test_zlib.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 class ZlibTest(CoreTest):
     fixture_src = __file__
 
     data_uncompressed = "iVBORw0KGgoAAAANSUhEUgAAAAgAAAAIAQMAAAD+wSzIAAAABlBMVEX///+/v7+jQ3Y5AAAADklEQVQI12P4AIX8EAgALgAD/aNpbtEAAAAASUVORK5CYII="
     data_compressed = "eJzrDPBz5+WS4mJgYOD19HAJAtIcIMzIDCT/HdQ5AaTYAnxCXP///79///7FzmWWQBE+TxfHEI7ryT8YWv8IcDDoMTD/XZyZdxEow+Dp6ueyzimhCQDLCRkd"
 
-    @jac_testcase("zlib.jac", "compress_test")
+    @jac_testcase("zlib.jac", "compress_test", True)
     def test_compress(self, ret):
         print(ret["report"])
         self.assertEqual(
             ret["report"][0],
             self.data_compressed,
         )
```

### Comparing `jaseci-1.4.0.9/jaseci/actions/standard/url.py` & `jaseci-1.4.1.0/jaseci/extens/act_lib/url.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Built in actions for Jaseci"""
-from jaseci.actions.live_actions import jaseci_action
+from jaseci.jsorc.live_actions import jaseci_action
 from fastapi import HTTPException
 import base64
 import requests
 import urllib
 import validators
```

### Comparing `jaseci-1.4.0.9/jaseci/actions/standard/vector.py` & `jaseci-1.4.1.0/jaseci/extens/act_lib/vector.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Built in actions for Jaseci"""
 import numpy as np
 from operator import itemgetter
 import pickle, base64
 
-from jaseci.actions.live_actions import jaseci_action
+from jaseci.jsorc.live_actions import jaseci_action
 
 
 def check_nested_list(lst):
     return all(isinstance(el, list) for el in lst)
 
 
 @jaseci_action(aliases=["cos_sim"])
```

### Comparing `jaseci-1.4.0.9/jaseci/actions/standard/zlib.py` & `jaseci-1.4.1.0/jaseci/extens/act_lib/zip.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Built in actions for Jaseci"""
-from jaseci.actions.live_actions import jaseci_action
+from jaseci.jsorc.live_actions import jaseci_action
+from jaseci.utils.utils import print_stack_to_log
 from base64 import b64decode, b64encode
 import zlib
 
 
 @jaseci_action()
 def compress(data_b64: str = ""):
     """
```

### Comparing `jaseci-1.4.0.9/jaseci/actions/tests/std_test_code.py` & `jaseci-1.4.1.0/jaseci/extens/act_lib/tests/std_test_code.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.0.9/jaseci/actions/tests/test_actions.py` & `jaseci-1.4.1.0/jaseci/jsorc/tests/test_actions.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from unittest import TestCase
+from unittest.mock import patch
 from jaseci.utils.utils import TestCaseHelper
-import jaseci.actions.live_actions as jla
-import jaseci.actions.remote_actions as jra
+import jaseci.jsorc.live_actions as jla
+import jaseci.jsorc.remote_actions as jra
+from jaseci.jsorc.live_actions import gen_remote_func_hook
 
 
 class JacActionsTests(TestCaseHelper, TestCase):
     """Unit tests for Jac language"""
 
     def setUp(self):
         super().setUp()
@@ -48,7 +50,31 @@
                 "use.qa_score": ["q_emb", "a_emb"],
                 "use.question_encode": ["question"],
             },
         )
 
     def test_live_action_globals(self):
         self.assertGreater(len(jla.live_actions), 25)
+
+    @patch("requests.post")
+    def test_remote_action_kwargs(self, mock_post):
+        remote_action = gen_remote_func_hook(
+            url="https://example.com/api/v1/endpoint",
+            act_name="example.action",
+            param_names=["param1", "param2"],
+        )
+        payload = {"param1": "value1"}
+        remote_action(**payload)
+
+        mock_post.assert_called_once()
+
+        _, kwargs = mock_post.call_args
+
+        assert kwargs["json"] == payload
+
+    def test_setup_decorated_as_startup(self):
+        @jla.jaseci_action(act_group=["ex"], allow_remote=True)
+        def setup(param: str = ""):
+            pass
+
+        app = jra.serv_actions()
+        assert len(app.__dict__["router"].__dict__["on_startup"]) == 1
```

### Comparing `jaseci-1.4.0.9/jaseci/actions/tests/test_std.py` & `jaseci-1.4.1.0/jaseci/extens/act_lib/tests/test_std.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,50 @@
 from unittest import TestCase
 
-import jaseci.actions.tests.std_test_code as stc
-from jaseci.actor.sentinel import Sentinel
-from jaseci.graph.graph import Graph
-from jaseci.svc import MetaService
+import jaseci.extens.act_lib.tests.std_test_code as stc
+from jaseci.prim.sentinel import Sentinel
+from jaseci.prim.graph import Graph
+from jaseci.jsorc.jsorc import JsOrc
 from jaseci.utils.utils import TestCaseHelper
 
 
 class JacTests(TestCaseHelper, TestCase):
     """Unit tests for STD library language"""
 
     def setUp(self):
         super().setUp()
-        self.meta = MetaService()
 
     def tearDown(self):
         super().tearDown()
 
     def test_rand_std(self):
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(stc.rand_std)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         report = test_walker.report
         self.assertEqual(len(report), 4)
         self.assertGreater(len(report[1]), len(report[0]))
         self.assertGreater(len(report[2]), len(report[1]))
         self.assertGreater(len(report[3]), len(report[2]))
 
     def test_file_io(self):
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(stc.file_io)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         report = test_walker.report
         self.assertEqual(report, ['{"a": 10}{"a": 10}'])
 
     def test_std_used_in_node_has_var(self):
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(stc.std_used_in_node_has_var)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         report = test_walker.report
         self.assertGreater(len(report[0]), 10)
```

### Comparing `jaseci-1.4.0.9/jaseci/actor/architype.py` & `jaseci-1.4.1.0/jaseci/prim/architype.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,71 +1,89 @@
 """
 Architype class for Jaseci
 
 Each architype is a registered templatized version of instances of any Jaseci
 abstractions or collections of instances (e.g., subgraphs, etc)
 """
-from jaseci.element.element import Element
+from jaseci.prim.element import Element
 from jaseci.jac.interpreter.architype_interp import ArchitypeInterp
 from jaseci.jac.ir.jac_code import JacCode
 from jaseci.utils.id_list import IdList
 
 
 class Architype(Element, JacCode, ArchitypeInterp):
     """Architype class for Jaseci"""
 
     def __init__(self, code_ir=None, is_async=False, *args, **kwargs):
         self.super_archs = list()
         self.anchor_var = None
         self.private_vars = []
         self.has_vars = []
-        self.entry_action_ids = IdList(self)
-        self.activity_action_ids = IdList(self)
-        self.exit_action_ids = IdList(self)
+        self.entry_ability_ids = IdList(self)
+        self.activity_ability_ids = IdList(self)
+        self.exit_ability_ids = IdList(self)
 
         # async handling for walker
         self.is_async = is_async
 
         Element.__init__(self, *args, **kwargs)
         JacCode.__init__(self, code_ir)
         ArchitypeInterp.__init__(self)
 
     def run(self):
         """
         Create set of new object instances from architype if needed
         """
         return self.run_architype(jac_ast=self.get_jac_ast())
 
-    def get_all_actions(self):
+    def get_actions(self, action_types: list):
         actions = IdList(self, auto_save=False)
         for i in self.arch_with_supers():
-            actions += i.entry_action_ids + i.activity_action_ids + i.exit_action_ids
+            for j in action_types:
+                actions += getattr(i, j)
         return actions
 
+    def get_entry_abilities(self):
+        return self.get_actions(["entry_ability_ids"])
+
+    def get_activity_abilities(self):
+        return self.get_actions(["activity_ability_ids"])
+
+    def get_exit_abilities(self):
+        return self.get_actions(["exit_ability_ids"])
+
+    def get_all_abilities(self):
+        return self.get_actions(
+            ["entry_ability_ids", "activity_ability_ids", "exit_ability_ids"]
+        )
+
     def arch_with_supers(self):
         archs = [self]
         for i in self.super_archs:
             obj = self.parent().arch_ids.get_obj_by_name(name=i, kind=self.kind)
             archs += obj.arch_with_supers()
         return archs
 
     def derived_types(self):
         names = []
         for i in self.arch_with_supers():
             names += i.super_archs + [i.name]
         return names
 
+    def get_architype(self):
+        return self
+
     def is_instance(self, name):
         return name in self.derived_types()
 
     def destroy(self):
         """
         Destroys self from memory and persistent storage
         """
         des = (
-            self.activity_action_ids.obj_list()
-            + self.entry_action_ids.obj_list()
-            + self.exit_action_ids.obj_list()
+            self.activity_ability_ids.obj_list()
+            + self.entry_ability_ids.obj_list()
+            + self.exit_ability_ids.obj_list()
         )
         for i in des:
             i.destroy()
         super().destroy()
```

### Comparing `jaseci-1.4.0.9/jaseci/actor/sentinel.py` & `jaseci-1.4.1.0/jaseci/prim/sentinel.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """
 Sentinel class for Jaseci
 
 Each sentinel has an id, name, timestamp and it's set of walkers.
 """
-from jaseci.element.element import Element
-from jaseci.element.obj_mixins import Anchored
+from jaseci.prim.element import Element
+from jaseci.prim.obj_mixins import Anchored
 from jaseci.utils.utils import (
     logger,
     ColCodes as Cc,
     is_true,
     perf_test_start,
     perf_test_stop,
 )
 from jaseci.utils.id_list import IdList
 from jaseci.jac.ir.jac_code import JacCode, jac_ir_to_ast
 from jaseci.jac.interpreter.sentinel_interp import SentinelInterp
-from jaseci.actor.walker import Walker
-from jaseci.actor.architype import Architype
+from jaseci.prim.walker import Walker
+from jaseci.prim.architype import Architype
 
 
 class Sentinel(Element, JacCode, SentinelInterp):
     """
     Sentinel class for Jaseci
 
     is_active is used to signify whether sentinel is ready to run walkers, i.e,
@@ -215,15 +215,17 @@
                     print(f"Testing {title}: ", end="")
                 sys.stdout, sys.stderr = buff_out[0], buff_out[1]
                 wlk.run()
                 sys.stdout, sys.stderr = screen_out[0], screen_out[1]
                 if i["assert_block"]:
                     wlk._loop_ctrl = None
                     wlk.scope_and_run(
-                        jac_ir_to_ast(i["assert_block"]), run_func=wlk.run_code_block
+                        jac_ir_to_ast(i["assert_block"]),
+                        run_func=wlk.run_code_block,
+                        scope_name="assert_block",
                     )
                 i["passed"] = True
                 if not silent:
                     print(
                         f"[{Cc.TG}PASSED{Cc.EC} in {Cc.TY}{time()-stime:.2f}s{Cc.EC}]"
                     )
                 if detailed and not silent:
```

### Comparing `jaseci-1.4.0.9/jaseci/actor/walker.py` & `jaseci-1.4.1.0/jaseci/prim/walker.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,24 +6,27 @@
 default hooks to save db read/writes
 """
 
 from jaseci.utils.utils import (
     logger,
     perf_test_start,
     perf_test_stop,
-    perf_test_to_b64,
     exc_stack_as_str_list,
 )
-from jaseci.element.element import Element
-from jaseci.element.obj_mixins import Anchored
+from jaseci.prim.element import Element
+from jaseci.prim.obj_mixins import Anchored
 from jaseci.utils.id_list import IdList
 from jaseci.jac.interpreter.walker_interp import WalkerInterp
 import uuid
 import hashlib
 
+from jaseci.jsorc.jsorc import JsOrc
+from jaseci.extens.svc.task_svc import TaskService
+from jaseci.utils.utils import format_jac_profile
+
 
 class Walker(Element, WalkerInterp, Anchored):
     """Walker class for Jaseci"""
 
     def __init__(self, is_async=False, **kwargs):
         self.yielded = False
         self.namespaces = []
@@ -33,14 +36,16 @@
         self.next_node_ids = IdList(self)
         self.destroy_node_ids = IdList(self)
         self.current_step = 0
         self.in_entry_exit = False
         self.step_limit = 10000
         self.is_async = is_async
         self._to_await = False
+        if "persist" not in kwargs:  # Default walker persistence to is_async
+            kwargs["persist"] = is_async
         Element.__init__(self, **kwargs)
         WalkerInterp.__init__(self)
         Anchored.__init__(self)
 
     @property
     def current_node(self):
         if not self.current_node_id:
@@ -113,41 +118,39 @@
                     self.current_node_id = None
                 i.destroy()
                 self.destroy_node_ids.remove_obj(i)
             return True
 
     def prime(self, start_node, prime_ctx=None, request_ctx=None):
         """Place walker on node and get ready to step step"""
-        if not self.yielded:
-            self.clear_state()
         if not self.yielded or not len(self.next_node_ids):  # modus ponens
             self.next_node_ids.add_obj(start_node, push_front=True)
         if prime_ctx:
             for i in prime_ctx.keys():
                 self.context[str(i)] = prime_ctx[i]
         self.request_context = request_ctx
         self.profile["steps"] = self.current_step
         logger.debug(str(f"Walker {self.name} primed - {start_node}"))
 
     def run(self, start_node=None, prime_ctx=None, request_ctx=None, profiling=False):
         """Executes Walker to completion"""
-        if self.for_queue() and self._h.task.is_running():
+        if self.for_queue() and JsOrc.svc("task").is_running():
             start_node = (
                 start_node
                 if not (start_node is None)
                 else (
                     self.next_node_ids.pop_first_obj() if self.next_node_ids else None
                 )
             )
 
             self._h.commit_all_cache_sync()
 
             return {
                 "is_queued": True,
-                "result": self._h.task.add_queue(
+                "result": JsOrc.svc("task", TaskService).add_queue(
                     self,
                     start_node,
                     prime_ctx or self.context,
                     request_ctx or self.request_context,
                     profiling,
                 ),
             }
@@ -184,16 +187,18 @@
             report_ret["status_code"] = self.report_status
         if self.report_custom:
             report_ret["report_custom"] = self.report_custom
         if len(self.runtime_errors):
             report_ret["errors"] = self.runtime_errors
             report_ret["success"] = False
         if profiling:
-            self.profile["perf"] = perf_test_stop(pr)
-            self.profile["graph"] = perf_test_to_b64(pr)
+            self.profile["jac"] = format_jac_profile(self.get_master()._jac_profile)
+            calls, graph = perf_test_stop(pr)
+            self.profile["perf"] = calls
+            self.profile["graph"] = graph
             report_ret["profile"] = self.profile
 
         if self.for_queue():
             return {"is_queued": False, "result": report_ret}
 
         return report_ret
 
@@ -224,15 +229,15 @@
         self.context = {}
         WalkerInterp.reset(self)
 
     def destroy(self):
         """
         Destroys self from memory and persistent storage
         """
-        if not self.for_queue() or not self._h.task.is_running():
+        if not self.for_queue() or not JsOrc.svc("task").is_running():
             WalkerInterp.destroy(self)
             super().destroy()
 
     def register_yield_or_destroy(self, yield_ids):
         """Helper for auto destroying walkers"""
         if not self.yielded:
             if self.jid in yield_ids:
```

### Comparing `jaseci-1.4.0.9/jaseci/api/actions_api.py` & `jaseci-1.4.1.0/jaseci/extens/api/actions_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Admin Global api functions as a mixin
 """
-from jaseci.api.interface import Interface
-import jaseci.actions.live_actions as lact
+from jaseci.extens.api.interface import Interface
+import jaseci.jsorc.live_actions as lact
 import json
 
 
 class ActionsApi:
     """
     APIs to manage actions
 
@@ -15,29 +15,29 @@
     the python program, or as a remote container linked action library. In this mode,
     action libraries operate as micro-services. Jaseci will be able to dynamically
     and automatically make this decision for the user based on online monitoring and
     performance profiling.
     """
 
     @Interface.admin_api(cli_args=["file"])
-    def actions_load_local(self, file: str):
+    def actions_load_local(self, file: str, ctx: dict = {}):
         """
         Hot load a python module and assimilate any Jaseci Actions
 
         This API will dynamically load a module based on a python file. The module
         is loaded directly into the running Jaseci python instance. This API also
         makes an attempt to auto detect and hot load any python package dependencies
         the file may reference via python's relative imports. This file is assumed to
         have the necessary annotations and decorations required by Jaseci to recognize
         its actions.
 
         :param file: The python file with full to load actions from.
             (i.e., ~/local/myact.py)
         """
-        success = lact.load_local_actions(file)
+        success = lact.load_local_actions(file, ctx=ctx)
         if success:
             cur_config = self.config_get("ACTION_SETS")
             if cur_config and (not isinstance(cur_config, list)):
                 config = json.loads(cur_config)
                 if file not in config["local"]:
                     config["local"].append(file)
                     self.config_set("ACTION_SETS", json.dumps(config))
@@ -45,29 +45,29 @@
                 self.config_set(
                     "ACTION_SETS",
                     json.dumps({"local": [file], "remote": [], "module": []}),
                 )
         return {"success": success}
 
     @Interface.admin_api(cli_args=["url"])
-    def actions_load_remote(self, url: str):
+    def actions_load_remote(self, url: str, ctx: dict = {}):
         """
         Hot link to a container linked action library
 
         This API will dynamically load a set of actions that are present on a remote
         server/micro-service. This server must be configured to interact with Jaseci
         properly. This is easily achieved using the same decorators used for local
         action libraries. Remote actions allow for higher flexibility in the languages
         supported for action libraries. If an  library writer would like to use another
         language, the main hook REST api simply needs to be implemented. Please
         refer to documentation on creating action libraries for more details.
 
         :param url: The url of the API server supporting Jaseci actions.
         """
-        success = lact.load_remote_actions(url)
+        success = lact.load_remote_actions(url, ctx=ctx)
         if success:
             cur_config = self.config_get("ACTION_SETS")
             if cur_config and (not isinstance(cur_config, list)):
                 config = json.loads(cur_config)
                 if url not in config["remote"]:
                     config["remote"].append(url)
                     self.config_set("ACTION_SETS", json.dumps(config))
@@ -75,28 +75,28 @@
                 self.config_set(
                     "ACTION_SETS",
                     json.dumps({"local": [], "remote": [url], "module": []}),
                 )
         return {"success": success}
 
     @Interface.admin_api(cli_args=["mod"])
-    def actions_load_module(self, mod: str):
+    def actions_load_module(self, mod: str, ctx: dict = {}):
         """
         Hot load a python module and assimilate any Jaseci Actions
 
         This API will dynamically load a module using python's module import format.
         This is particularly useful for pip installed action libraries as the developer
         can directly reference the module using the same format as a regular python
         import. As with load local, the module will be loaded directly into the running
         Jaseci python instance.
 
         :param mod: The import style module to load actions from.
             (i.e., jaseci_ai_kit.bi_enc)
         """
-        success = lact.load_module_actions(mod)
+        success = lact.load_module_actions(mod, ctx=ctx)
         if success:
             cur_config = self.config_get("ACTION_SETS")
             if cur_config and (not isinstance(cur_config, list)):
                 config = json.loads(cur_config)
                 if mod not in config["module"]:
                     config["module"].append(mod)
                     self.config_set("ACTION_SETS", json.dumps(config))
@@ -156,7 +156,15 @@
 
     @Interface.admin_api(cli_args=["name"])
     def actions_unload_actionset(self, name: str):
         """
         Unload modules loaded for actions
         """
         return {"success": lact.unload_actionset(name)}
+
+    @Interface.admin_api(cli_args=["name"])
+    def actions_call(self, name: str, ctx: dict = {}):
+        """
+        Call an action by name
+        """
+        ret, sucess = lact.call_action(name, ctx=ctx)
+        return {"success": sucess, "result": ret}
```

### Comparing `jaseci-1.4.0.9/jaseci/api/alias_api.py` & `jaseci-1.4.1.0/jaseci/extens/api/alias_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Alias api as a mixin
 """
-from jaseci.api.interface import Interface
+from jaseci.extens.api.interface import Interface
 
 
 class AliasAPI:
     """
     Alias APIs for creating nicknames for UUIDs and other long strings
 
     The alias set of APIs provide a set of `alias' management functions for
```

### Comparing `jaseci-1.4.0.9/jaseci/api/architype_api.py` & `jaseci-1.4.1.0/jaseci/extens/api/architype_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Architype api functions as a mixin
 """
-from jaseci.api.interface import Interface
-from jaseci.actor.architype import Architype
-from jaseci.actor.sentinel import Sentinel
+from jaseci.extens.api.interface import Interface
+from jaseci.prim.architype import Architype
+from jaseci.prim.sentinel import Sentinel
 from jaseci.utils.utils import b64decode_str
 
 
 class ArchitypeApi:
     """Architype APIs for creating and managing Jaseci architypes
 
     The architype set of APIs allow for the addition and removing of
```

### Comparing `jaseci-1.4.0.9/jaseci/api/global_api.py` & `jaseci-1.4.1.0/jaseci/extens/api/global_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Admin Global api functions as a mixin
 """
-from jaseci.api.interface import Interface
-from jaseci.actor.sentinel import Sentinel
+from jaseci.extens.api.interface import Interface
+from jaseci.prim.sentinel import Sentinel
 import uuid
 
 
 class GlobalApi:
     """
     Admin global APIs
     """
```

### Comparing `jaseci-1.4.0.9/jaseci/api/graph_api.py` & `jaseci-1.4.1.0/jaseci/extens/api/graph_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Graph api functions as a mixin
 """
-from jaseci.api.interface import Interface
+from jaseci.extens.api.interface import Interface
 from jaseci.utils.id_list import IdList
-from jaseci.graph.graph import Graph
-from jaseci.graph.node import Node
+from jaseci.prim.graph import Graph
+from jaseci.prim.node import Node
 import uuid
 
 
 class GraphApi:
     """
     Graph APIs
     """
```

### Comparing `jaseci-1.4.0.9/jaseci/api/interface.py` & `jaseci-1.4.1.0/jaseci/extens/api/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 General master interface engine for client interfaces as mixin
 """
 from inspect import signature, getdoc
 from jaseci.utils.utils import logger, is_jsonable, is_true, exc_stack_as_str_list
-from jaseci.element.element import Element
-from jaseci.actor.walker import Walker
+from jaseci.prim.element import Element
+from jaseci.prim.walker import Walker
 import json
 
 
 class Interface:
     """
     General master interface engine
     """
```

### Comparing `jaseci-1.4.0.9/jaseci/api/jac_api.py` & `jaseci-1.4.1.0/jaseci/extens/api/jac_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 Jac tools api functions as a mixin
 """
 from copy import deepcopy
 import json
 import os
 
-from jaseci.api.interface import Interface
-from jaseci.svc import MetaService
+from jaseci.extens.api.interface import Interface
+from jaseci.jsorc.jsorc import JsOrc
 
 
 class JacApi:
     """
     Jac tool APIs
     """
 
@@ -154,15 +154,15 @@
             nd=faux.active_gph(),
             ctx=ctx,
             profiling=False,
         )
         return faux.graph_get(nd=faux.active_gph(), mode="dot", detailed=detailed)
 
     def faux_master(self):
-        faux = MetaService(run_svcs=False).build_super_master()
+        faux = JsOrc.super_master()
         faux._h.mem["global"] = deepcopy(self._h.mem["global"])
         return faux
 
     def check_for_file(self, file):
         if not os.path.isfile(file):
             ret = "File does not exsist!"
             return ret, ret
```

### Comparing `jaseci-1.4.0.9/jaseci/api/logger_api.py` & `jaseci-1.4.1.0/jaseci/extens/api/logger_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Logger api as a mixin
 """
 import re
-from jaseci.api.interface import Interface
+from jaseci.extens.api.interface import Interface
 from jaseci.utils.log_utils import parse_logs
 from jaseci.utils.utils import logger, app_logger, logs
 from jaseci.utils.utils import connect_logger_handler
 from logging.handlers import HTTPHandler
 
 
 class LoggerApi:
```

### Comparing `jaseci-1.4.0.9/jaseci/api/master_api.py` & `jaseci-1.4.1.0/jaseci/extens/api/master_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Master api as a mixin
 """
-from jaseci.api.interface import Interface
+from jaseci.extens.api.interface import Interface
 from jaseci.utils.id_list import IdList
 import uuid
 
 
 class MasterApi:
     """
     Master APIs for users creating and managing groups of sub users
```

### Comparing `jaseci-1.4.0.9/jaseci/api/object_api.py` & `jaseci-1.4.1.0/jaseci/extens/api/object_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Object api as a mixin
 """
-from jaseci.api.interface import Interface
-from jaseci.element.element import Element
+from jaseci.extens.api.interface import Interface
+from jaseci.prim.element import Element
 
 
 class ObjectApi:
     """Object APIs for generalized operations on Jaseci objects
 
     ...
     """
@@ -25,14 +25,26 @@
     @Interface.private_api(cli_args=["obj"])
     def object_get(self, obj: Element, depth: int = 0, detailed: bool = False):
         """Returns object details for any Jaseci object."""
         ret = obj.serialize(deep=depth, detailed=detailed)
         return ret
 
     @Interface.private_api(cli_args=["obj"])
+    def object_set(
+        self, obj: Element, ctx: dict, depth: int = 0, detailed: bool = False
+    ):
+        """Update a field in an object."""
+        if "jid" in ctx:
+            del ctx["jid"]
+        for i in ctx.keys():
+            if i in dir(obj) and not callable(getattr(obj, i)):
+                setattr(obj, i, ctx[i])
+        return obj.serialize(deep=depth, detailed=detailed)
+
+    @Interface.private_api(cli_args=["obj"])
     def object_perms_get(self, obj: Element):
         """Returns object access mode for any Jaseci object."""
         return {"access": obj.j_access}
 
     @Interface.private_api(cli_args=["obj"])
     def object_perms_set(self, obj: Element, mode: str):
         """Sets object access mode for any Jaseci object."""
```

### Comparing `jaseci-1.4.0.9/jaseci/api/prometheus_api.py` & `jaseci-1.4.1.0/jaseci/extens/api/prometheus_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,74 @@
 """
 Prometheus APIs
 """
-from jaseci.api.interface import Interface
+from jaseci.extens.api.interface import Interface
+from jaseci.jsorc.jsorc import JsOrc
+from jaseci.extens.svc.prome_svc import PrometheusService
+
+
+def prome():
+    return JsOrc.svc("prome").poke(PrometheusService)
 
 
 class PrometheusApi:
     """
     Prometheus APIs
     """
 
     @Interface.admin_api()
     def prometheus_metrics_list(self):
         """
         Return list of availabel metrics
         """
-        hook = self._h
-        if hook.meta.run_svcs:
-            return hook.promon.all_metrics()
-        else:
-            return {"success": False, "message": "No runnning Prometheus service."}
+        return prome().all_metrics()
 
     @Interface.admin_api()
     def prometheus_pod_list(self, namespace: str = "", exclude_prom: bool = False):
         """
         Return list of pods. If exclude_prom,
         """
-        hook = self._h
-        if hook.meta.run_svcs:
-            return hook.promon.pods(namespace=namespace, exclude_prom=exclude_prom)
-        else:
-            return {"success": False, "message": "No runnning Prometheus service."}
+        return prome().pods(namespace=namespace, exclude_prom=exclude_prom)
 
     @Interface.admin_api()
     def prometheus_pod_info(
         self,
         namespace: str = "",
         exclude_prom: bool = False,
         timestamp: int = 0,
         duration: int = 0,
     ):
         """
         Return pods info and metrics
         """
-        hook = self._h
-        if hook.meta.run_svcs:
-            return hook.promon.info(
+        return (
+            prome()
+            .info(
+                namespace=namespace,
+                exclude_prom=exclude_prom,
+                timestamp=timestamp,
+                duration=duration,
+            )
+            .pod
+        )
+
+    @Interface.admin_api()
+    def prometheus_node_info(
+        self,
+        namespace: str = "",
+        exclude_prom: bool = False,
+        timestamp: int = 0,
+        duration: int = 0,
+    ):
+        """
+        Return pods info and metrics
+        """
+        return (
+            prome()
+            .info(
                 namespace=namespace,
                 exclude_prom=exclude_prom,
                 timestamp=timestamp,
                 duration=duration,
             )
-        else:
-            return {"success": False, "message": "No runnning Prometheus service."}
+            .node
+        )
```

### Comparing `jaseci-1.4.0.9/jaseci/api/sentinel_api.py` & `jaseci-1.4.1.0/jaseci/extens/api/sentinel_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Sentinel api functions as a mixin
 """
-from jaseci.api.interface import Interface
+from jaseci.extens.api.interface import Interface
 from jaseci.utils.id_list import IdList
-from jaseci.actor.sentinel import Sentinel
+from jaseci.prim.sentinel import Sentinel
 from jaseci.utils.utils import b64decode_str
 import uuid
 
 
 class SentinelApi:
     """
     Sentinel APIs
```

### Comparing `jaseci-1.4.0.9/jaseci/api/super_api.py` & `jaseci-1.4.1.0/jaseci/extens/api/super_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Super (master) api as a mixin
 """
-from jaseci.api.interface import Interface
-from jaseci.element.master import Master
+from jaseci.extens.api.interface import Interface
+from jaseci.prim.master import Master
 
 
 class SuperApi:
     """Super APIs for creating nicknames for UUIDs and other long strings"""
 
     @Interface.admin_api(cli_args=["name"])
     def master_createsuper(
```

### Comparing `jaseci-1.4.0.9/jaseci/api/tests/test_architype_api.py` & `jaseci-1.4.1.0/jaseci/extens/api/tests/test_architype_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.0.9/jaseci/api/tests/test_global_api.py` & `jaseci-1.4.1.0/jaseci/extens/api/tests/test_global_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from jaseci.utils.test_core import CoreTest
+from jaseci.jsorc.jsorc import JsOrc
 import jaseci.tests.jac_test_code as jtc
 
 
 class GlobalApiTest(CoreTest):
     """Unit tests for Jac Global APIs"""
 
     fixture_src = __file__
 
     def setUp(self):
         super().setUp()
 
-        self.smast2 = self.meta.build_super_master(h=self.smast._h)
+        self.smast2 = JsOrc.super_master(h=self.smast._h)
         self.smast.sentinel_register(name="test", code=jtc.basic)
 
-        self.mast = self.meta.build_master()
-        self.mast2 = self.meta.build_super_master(h=self.mast._h)
+        self.mast2 = JsOrc.master(h=self.mast._h)
         self.mast.sentinel_register(name="test", code=jtc.basic)
 
     def tearDown(self):
         super().tearDown()
 
     def test_sent_global_active(self):
         """Test setting global sentinel"""
```

### Comparing `jaseci-1.4.0.9/jaseci/api/tests/test_graph_api.py` & `jaseci-1.4.1.0/jaseci/extens/api/tests/test_graph_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.0.9/jaseci/api/tests/test_logger_api.py` & `jaseci-1.4.1.0/jaseci/extens/api/tests/test_logger_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import logging
 from jaseci.utils.log_utils import LimitedSlidingBuffer, parse_logs
 from jaseci.utils.test_core import CoreTest
 
 
 class LoggerApiTest(CoreTest):
     fixture_src = __file__
 
@@ -27,17 +26,16 @@
         self.call(
             self.mast,
             ["sentinel_register", {"code": self.load_jac("test_logging.jac")}],
         )
         self.logger_off()
 
         ret = self.call(self.smast, ["logger_get", {}])
-
-        self.assertEqual(len(ret), 1)
-        self.assertTrue(ret[0]["log"].endswith("Hello world!"))
+        self.assertGreaterEqual(len(ret), 1)
+        self.assertTrue(ret[-1]["log"].endswith("Hello world!"))
 
     def test_limited_sliding_buffer(self):
         buffer = LimitedSlidingBuffer(max_size=25)
         buffer.write("Hello world!")
         buffer.write("Hi there!")
         buffer.write("Hello world!")
         buffer.write("Hi there!")
```

### Comparing `jaseci-1.4.0.9/jaseci/api/tests/test_sentinel_api.py` & `jaseci-1.4.1.0/jaseci/extens/api/tests/test_sentinel_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.0.9/jaseci/api/tests/test_user_api.py` & `jaseci-1.4.1.0/jaseci/extens/api/tests/test_user_api.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.0.9/jaseci/api/tests/test_walker_api.py` & `jaseci-1.4.1.0/jaseci/extens/api/tests/test_walker_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from jaseci.graph.edge import Edge
-from jaseci.graph.node import Node
+from jaseci.prim.edge import Edge
+from jaseci.prim.node import Node
 from jaseci.utils.test_core import CoreTest
 
 
 class WalkerApiTest(CoreTest):
     """Unit tests for Jac Walker APIs"""
 
     fixture_src = __file__
@@ -292,7 +292,25 @@
             self.mast,
             ["sentinel_register", {"code": self.load_jac("walker_yield.jac")}],
         )
         ret = []
         self.call(self.mast, ["walker_run", {"name": "error_walker_action"}])
         ret = self.call(self.mast, ["walker_run", {"name": "error_walker_action"}])
         self.assertIn('cannot execute the statement "disengage ; "', ret["errors"][0])
+
+    def test_walker_stepping(self):
+        self.call(
+            self.mast,
+            ["sentinel_register", {"code": self.load_jac("fam.jac")}],
+        )
+        ret = self.call(self.mast, ["walker_spawn_create", {"name": "create_fam"}])
+        jid = ret["jid"]
+        ret = self.call(self.mast, ["walker_prime", {"wlk": jid}])
+        ret = self.call(self.mast, ["walker_step", {"wlk": jid}])
+        self.log(ret)
+        self.assertEqual(len(ret["next_node_ids"]), 2)
+        ret = self.call(self.mast, ["walker_step", {"wlk": jid}])
+        self.assertEqual(len(ret["next_node_ids"]), 1)
+        ret = self.call(self.mast, ["walker_step", {"wlk": jid}])
+        self.assertEqual(len(ret["next_node_ids"]), 0)
+        ret = self.call(self.mast, ["walker_step", {"wlk": jid}])
+        self.assertEqual(len(ret["next_node_ids"]), 0)
```

### Comparing `jaseci-1.4.0.9/jaseci/api/user_api.py` & `jaseci-1.4.1.0/jaseci/extens/api/user_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 User API
 """
-from jaseci.api.interface import Interface
-from jaseci.svc.meta import MetaService
+from jaseci.extens.api.interface import Interface
+from jaseci.jsorc.jsorc import JsOrc
 
 
 class UserApi:
     """
     User APIs for creating users (some functions should be override downstream)
 
     These User APIs enable the creation and management of users on a Jaseci machine.
@@ -103,22 +103,22 @@
         return ret
 
     def user_creator(self, name, password: str = "", other_fields: dict = {}):
         """
         Abstraction for user creation for elegant overriding
         """
 
-        return MetaService().build_master(h=self._h, name=name)
+        return JsOrc.master(h=self._h, name=name)
 
     def superuser_creator(self, name, password: str = "", other_fields: dict = {}):
         """
         Abstraction for super user creation for elegant overriding
         """
 
-        return MetaService().build_super_master(h=self._h, name=name)
+        return JsOrc.super_master(h=self._h, name=name)
 
     def user_global_init(
         self,
         mast,
         global_init: str = "",
         global_init_ctx: dict = {},
     ):
```

### Comparing `jaseci-1.4.0.9/jaseci/api/walker_api.py` & `jaseci-1.4.1.0/jaseci/extens/api/walker_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Walker api functions as a mixin
 """
-from jaseci.api.interface import Interface
-from jaseci.actor.walker import Walker
-from jaseci.graph.node import Node
-from jaseci.actor.sentinel import Sentinel
+from jaseci.extens.api.interface import Interface
+from jaseci.prim.walker import Walker
+from jaseci.prim.node import Node
+from jaseci.prim.sentinel import Sentinel
 from jaseci.utils.id_list import IdList
 
 
 class WalkerApi:
     """
     Walker APIs
 
@@ -18,14 +18,19 @@
     variations on this API that enable the invocation of walkers with various
     semantics.
     """
 
     def __init__(self):
         self.spawned_walker_ids = IdList(self)
         self.yielded_walkers_ids = IdList(self)
+        self.reset_profiling(False)
+
+    def reset_profiling(self, profiling):
+        self._profiling = profiling
+        self._jac_profile = {}
 
     @Interface.private_api(cli_args=["wlk"])
     def walker_get(self, wlk: Walker, mode: str = "default", detailed: bool = False):
         """
         Get a walker rendered with specific mode
         Valid modes: {default, code, ir, keys, }
         """
@@ -60,14 +65,15 @@
 
     @Interface.private_api(cli_args=["name"])
     def walker_spawn_create(self, name: str, snt: Sentinel = None):
         """
         Creates new instance of walker and returns new walker object
         """
         wlk = snt.run_architype(name=name, kind="walker", caller=self, is_async=False)
+        wlk.make_persistent()
         if wlk:
             if self.spawned_walker_ids.has_obj_by_name(name):
                 self.spawned_walker_ids.destroy_obj_by_name(name)
             self.spawned_walker_ids.add_obj(wlk)
             self.alias_register(f"spawned:walker:{name}", wlk.jid)
             return wlk.serialize()
         else:
@@ -161,18 +167,34 @@
         ctx: dict = {},
         _req_ctx: dict = {},
         profiling: bool = False,
     ):
         """
         Executes walker (assumes walker is primed)
         """
+        self.reset_profiling(profiling)
         return wlk.run(
             start_node=prime, prime_ctx=ctx, request_ctx=_req_ctx, profiling=profiling
         )
 
+    @Interface.private_api(cli_args=["wlk"])
+    def walker_step(self, wlk: Walker, detailed: bool = False):
+        """
+        Executes walker (assumes walker is primed)
+        """
+        wlk.step()
+        ret = {
+            "current_node": wlk.current_node.serialize(detailed=detailed),
+            "next_node_ids": wlk.next_node_ids,
+            "walker_context": wlk.serialize(detailed=detailed)["context"],
+            "walker_report": wlk.report,
+            "profile": wlk.profile,
+        }
+        return ret
+
     @Interface.private_api(cli_args=["name"])
     def walker_run(
         self,
         name: str,
         nd: Node = None,
         ctx: dict = {},
         _req_ctx: dict = {},
@@ -180,14 +202,15 @@
         profiling: bool = False,
         is_async: bool = None,
     ):
         """
         Creates walker instance, primes walker on node, executes walker,
         reports results, and cleans up walker instance.
         """
+        self.reset_profiling(profiling)
         wlk = self.yielded_walkers_ids.get_obj_by_name(name, silent=True)
         if wlk is None:
             wlk = snt.run_architype(
                 name=name, kind="walker", caller=self, is_async=is_async
             )
         if wlk is None:
             return self.bad_walk_response([f"Walker {name} not found!"])
@@ -206,14 +229,15 @@
         _req_ctx: dict = {},
         snt: Sentinel = None,
         profiling: bool = False,
     ):
         """
         Walker individual APIs
         """
+        self.reset_profiling(profiling)
         return self.walker_run(name, nd, ctx, _req_ctx, snt, profiling)
 
     @Interface.public_api(cli_args=["wlk"])
     def walker_summon(
         self,
         key: str,
         wlk: Walker,
```

### Comparing `jaseci-1.4.0.9/jaseci/api/webhook_api.py` & `jaseci-1.4.1.0/jaseci/extens/api/webhook_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 """
 Webhook API
 """
-from jaseci.api.interface import Interface
+from jaseci.extens.api.interface import Interface
 from fastapi import HTTPException
-from json import loads
-from jaseci.svc import MetaService
+from jaseci.jsorc.jsorc import JsOrc
+from jaseci.extens.svc.stripe_svc import StripeService
+
+import stripe as _stripe
 
 
 class WebhookApi:
     """
     Webhook API
     """
 
     @Interface.public_api(url_args=["provider"], allowed_methods=["post"])
     def webhook(self, provider: str, _req_ctx: dict = {}, _raw_req_ctx: str = None):
         """Handle webhook logic"""
         req_body = _req_ctx["body"]
 
         if provider == "stripe":
-            stripe_service = MetaService().get_service("stripe")
-            stripe = stripe_service.poke()
+            stripe_service = JsOrc.svc("stripe", StripeService)
+            stripe = stripe_service.poke(_stripe)
 
             # to be updated
             stripe_service.get_event(_raw_req_ctx, _req_ctx["headers"])
 
             payload_obj = req_body.get("data").get("object")
             customer_id = payload_obj.get("customer")
```

### Comparing `jaseci-1.4.0.9/jaseci/element/element.py` & `jaseci-1.4.1.0/jaseci/prim/element.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 """
 
 import copy
 import json
 import uuid
 from datetime import datetime
 
-from jaseci.element.obj_mixins import Hookable
-from jaseci.hook import MemoryHook
+from jaseci.prim.obj_mixins import Hookable
+from jaseci.jsorc.memory import MemoryHook
 from jaseci.utils.id_list import IdList
 from jaseci.utils.json_handler import JaseciJsonEncoder, json_str_to_jsci_dict
 from jaseci.utils.utils import log_var_out, logger, camel_to_snake
 
 __version__ = "1.0.0"
 element_fields = None
```

### Comparing `jaseci-1.4.0.9/jaseci/element/master.py` & `jaseci-1.4.1.0/jaseci/prim/master.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 """
 Main master handler for each user of Jaseci, serves as main interface between
 between user and Jaseci
 """
 
-from jaseci.element.element import Element
-from jaseci.api.alias_api import AliasAPI
-from jaseci.api.object_api import ObjectApi
-from jaseci.api.graph_api import GraphApi
-from jaseci.api.sentinel_api import SentinelApi
-from jaseci.api.walker_api import WalkerApi
-from jaseci.api.architype_api import ArchitypeApi
-from jaseci.api.config_api import ConfigApi
-from jaseci.api.interface import Interface
-from jaseci.api.master_api import MasterApi
-from jaseci.api.jac_api import JacApi
-from jaseci.api.user_api import UserApi
-from jaseci.api.queue_api import QueueApi
-from jaseci.api.webhook_api import WebhookApi
+from jaseci.prim.element import Element
+from jaseci.extens.api.alias_api import AliasAPI
+from jaseci.extens.api.object_api import ObjectApi
+from jaseci.extens.api.graph_api import GraphApi
+from jaseci.extens.api.sentinel_api import SentinelApi
+from jaseci.extens.api.walker_api import WalkerApi
+from jaseci.extens.api.architype_api import ArchitypeApi
+from jaseci.extens.api.config_api import ConfigApi
+from jaseci.extens.api.interface import Interface
+from jaseci.extens.api.master_api import MasterApi
+from jaseci.extens.api.jac_api import JacApi
+from jaseci.extens.api.user_api import UserApi
+from jaseci.extens.api.queue_api import QueueApi
+from jaseci.extens.api.webhook_api import WebhookApi
+from jaseci.jsorc.jsorc import JsOrc
 
 
+@JsOrc.context(name="master")
 class Master(
     Element,
     Interface,
     MasterApi,
     AliasAPI,
     GraphApi,
     ObjectApi,
```

### Comparing `jaseci-1.4.0.9/jaseci/element/obj_mixins.py` & `jaseci-1.4.1.0/jaseci/prim/obj_mixins.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,14 +203,19 @@
                     "Hook for {} does not match {}, {} != {}".format(
                         target, self, target._h, self._h
                     )
                 )
             )
         return target._h == self._h
 
+    def make_persistent(self):
+        """Make element persistent"""
+        self._persist = True
+        self.save()
+
     def save(self):
         """
         Write self through hook to persistent storage
         """
         self._h.save_obj(self._m_id, self)
 
     def destroy(self):
```

### Comparing `jaseci-1.4.0.9/jaseci/graph/edge.py` & `jaseci-1.4.1.0/jaseci/prim/edge.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Edge class for Jaseci
 
 Each edge has an id, name, timestamp, the from node at the element of the edge
 and the to node it is pointing to.
 """
-from jaseci.element.element import Element
-from jaseci.element.obj_mixins import Anchored
+from jaseci.prim.element import Element
+from jaseci.prim.obj_mixins import Anchored
 from jaseci.utils.utils import logger
 import uuid
 import sys
 
 
 class Edge(Element, Anchored):
     """Edge class for Jaseci"""
```

### Comparing `jaseci-1.4.0.9/jaseci/graph/graph.py` & `jaseci-1.4.1.0/jaseci/prim/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Graph  class for Jaseci
 
 """
-from jaseci.graph.node import Node
+from jaseci.prim.node import Node
 from jaseci.utils.id_list import IdList
 
 
 class Graph(Node):
     """Graph class for Jaseci"""
 
     def __init__(self, **kwargs):
```

### Comparing `jaseci-1.4.0.9/jaseci/graph/node.py` & `jaseci-1.4.1.0/jaseci/prim/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 Node class for Jaseci
 
 Each node has an id, name, timestamp and it's set of edges.
 First node in list of 'member_node_ids' is designated root node
 """
 from collections import OrderedDict
-from jaseci.element.element import Element
-from jaseci.element.obj_mixins import Anchored
-from jaseci.graph.edge import Edge
+from jaseci.prim.element import Element
+from jaseci.prim.obj_mixins import Anchored
+from jaseci.prim.edge import Edge
 from jaseci.utils.id_list import IdList
 from jaseci.utils.utils import logger
 
 import uuid
 
 TO = 0
 FROM = 1
```

### Comparing `jaseci-1.4.0.9/jaseci/hook/memory.py` & `jaseci-1.4.1.0/jaseci/jsorc/memory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from json import dumps, loads
 import sys
 from jaseci.utils.utils import find_class_and_import
+from jaseci.jsorc.jsorc import JsOrc
 
 
+@JsOrc.repository(name="hook")
 class MemoryHook:
     """
     Set of virtual functions to be used as hooks to allow access to
     the complete set of items across jaseci object types. This class contains
     a number of blank function calls to be bound extrenally and passed
     to the objects. They return jaseci core types.
     """
 
     def __init__(self):
-        from jaseci.actions.live_actions import get_global_actions
+        from jaseci.jsorc.live_actions import get_global_actions
 
         self.mem = {"global": {}}
         self._machine = None
         self.save_obj_list = set()
         self.save_glob_dict = {}
 
     ####################################################
@@ -93,15 +95,15 @@
         self.decommit_glob_from_cache(name)
 
         if persist:
             self.destroy_glob_from_store(name)
 
     # ----------------- SERVICE GLOB ----------------- #
 
-    def service_glob(self, name, val):
+    def get_or_create_glob(self, name, val):
         if not self.has_glob(name):
             self.save_glob(name, dumps(val))
             self.commit()
         return loads(self.get_glob(name))
 
     ####################################################
     #        DATASOURCE METHOD (TO BE OVERRIDE)        #
@@ -155,24 +157,25 @@
         """Get list of global config to externally hooked general store"""
         return list(self.mem["global"].keys())
 
     ####################################################
     # ------------------ COMMITTER ------------------- #
     ####################################################
 
-    def commit(self):
-        for i in self.save_obj_list:
-            self.commit_obj_to_cache(i)
+    def commit(self, skip_cache=False):
+        if not skip_cache:
+            for i in self.save_obj_list:
+                self.commit_obj_to_cache(i)
 
-        self.save_obj_list = set()
+            self.save_obj_list = set()
 
-        for i in self.save_glob_dict.keys():
-            self.commit_glob_to_cache(name=i, value=self.save_glob_dict[i])
+            for i in self.save_glob_dict.keys():
+                self.commit_glob_to_cache(name=i, value=self.save_glob_dict[i])
 
-        self.save_glob_dict = {}
+            self.save_glob_dict = {}
 
     ###################################################
     #   CACHE CONTROL (SHOULD NOT OVERRIDEN ON ORM)   #
     ###################################################
 
     # -------------------- GLOBS -------------------- #
 
@@ -215,15 +218,15 @@
         return sys.getsizeof(self.mem) / 1024
 
     ###################################################
     #                  CLASS CONTROL                  #
     ###################################################
 
     def find_class_and_import(self, j_type, mod):
-        cls = self.meta.get_context(j_type)
+        cls = JsOrc.ctx_cls(j_type)
 
         if not cls:
             cls = find_class_and_import(j_type, mod)
 
         return cls
 
     def clear_cache(self):
```

### Comparing `jaseci-1.4.0.9/jaseci/hook/redis.py` & `jaseci-1.4.1.0/jaseci/jsorc/redis.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 """
 This module includes code related to hooking Jaseci's Redis to the
 core engine.
 """
 import json
 
 import jaseci as core_mod
-from jaseci.svc import ProxyService
-from jaseci.utils.json_handler import JaseciJsonDecoder
-from .memory import MemoryHook
+from jaseci.utils.json_handler import JaseciJsonDecoder, jsci_dict_normalize
+from jaseci.jsorc.memory import MemoryHook
+from jaseci.jsorc.jsorc import JsOrc
+from jaseci.extens.svc.redis_svc import RedisService
 
 
 #################################################
 #                  REDIS HOOK                   #
 #################################################
 
 
+@JsOrc.repository(name="hook", priority=1)
 class RedisHook(MemoryHook):
-    def __init__(self):
-        # proxy redis, to be overriden by build_apps
-        self.redis = ProxyService()
+    def __init__(self, redis: RedisService = None):
+        self.redis = JsOrc.svc("redis", RedisService)
         self.red_touch_count = 0
 
         super().__init__()
 
     ####################################################
     #        DATASOURCE METHOD (TO BE OVERRIDE)        #
     ####################################################
@@ -40,19 +41,21 @@
             if loaded_obj:
                 self.red_touch_count += 1
                 jdict = json.loads(loaded_obj, cls=JaseciJsonDecoder)
                 j_type = jdict["j_type"]
                 j_master = jdict["j_master"]
                 class_for_type = self.find_class_and_import(j_type, core_mod)
                 ret_obj = class_for_type(h=self, m_id=j_master, auto_save=False)
-                ret_obj.json_load(loaded_obj)
+                jsci_dict_normalize(jdict, parent_obj=ret_obj)
+                ret_obj.dict_load(jdict)
 
                 super().commit_obj_to_cache(ret_obj)
-                return ret_obj
-
+                obj = ret_obj
+        if obj:
+            obj._persist = True
         return obj
 
     def has_obj_in_store(self, item_id):
         """
         Checks for object existance in store
         """
         return super().has_obj_in_store(item_id) or (
@@ -117,15 +120,15 @@
 
         if all_caches and item._persist and self.redis.is_running():
             self.redis.set(item.jid, item.json(detailed=True))
 
     def decommit_obj_from_cache(self, item):
         super().decommit_obj_from_cache(item)
 
-        if self.redis.is_running():
+        if item._persist and self.redis.is_running():
             self.redis.delete(item.jid)
 
     ###################################################
     #                     CLEANER                     #
     ###################################################
 
     def clear_cache(self):
```

### Comparing `jaseci-1.4.0.9/jaseci/jac/interpreter/architype_interp.py` & `jaseci-1.4.1.0/jaseci/jac/interpreter/architype_interp.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """
 Sentinel interpreter for jac code in AST form
 
 This interpreter should be inhereted from the class that manages state
 referenced through self.
 """
-from jaseci.graph.node import Node
-from jaseci.graph.edge import Edge
-from jaseci.actor.walker import Walker
+from jaseci.prim.node import Node
+from jaseci.prim.edge import Edge
+from jaseci.prim.walker import Walker
 from jaseci.jac.interpreter.interp import Interp
 from jaseci.jac.machine.jac_scope import JacScope
+from jaseci.jac.machine.jac_value import JacValue
 
 
 class ArchitypeInterp(Interp):
     """Jac interpreter mixin for objects that will execute Jac code"""
 
     def run_architype(self, jac_ast):
         """
@@ -39,15 +40,15 @@
                     kind=self.kind,
                     name=self.name,
                     parent=self.parent(),
                 )
 
         kid = self.set_cur_ast(jac_ast)
 
-        self.push_scope(JacScope(parent=self, has_obj=self, action_sets=[]))
+        self.push_scope(JacScope(parent=self, name=f"spawn:{jac_ast.loc_str()}"))
         if kid[0].name == "KW_NODE":
             item = Node(
                 m_id=self._m_id,
                 h=self._h,
                 kind=kid[0].token_text(),
                 name=kid[1].token_text(),
                 parent=self.parent(),
@@ -74,83 +75,113 @@
                 name=kid[1].token_text(),
                 kind=kid[0].token_text(),
                 parent=self.parent(),
                 is_async=self.is_async,
             )
             if kid[2].name == "namespaces":
                 item.namespaces = self.run_namespaces(jac_ast.kid[2])
+            self.build_object_with_supers(item, kid[-1])
         elif jac_ast.name == "graph_block":  # usedi n jac tests
             item = self.run_graph_block(jac_ast)
         self.pop_scope()
         return item
 
     def run_namespaces(self, jac_ast):
         """
         namespaces: COLON name_list;
         """
         return self.run_name_list(jac_ast.kid[1])
 
+    def run_walker_block(self, jac_ast, obj):
+        """
+        walker_block:
+            LBRACE attr_stmt* walk_entry_block? (
+                statement
+                | walk_activity_block
+            )* walk_exit_block? RBRACE;
+        """
+        kid = self.set_cur_ast(jac_ast)
+        for i in kid:
+            if i.name == "attr_stmt":
+                self.run_attr_stmt(jac_ast=i, obj=obj)
+
     def run_attr_block(self, jac_ast, obj):
         """
         attr_block:
             LBRACE (attr_stmt)* RBRACE
             | COLON (attr_stmt)* SEMI
             | SEMI;
         """
         kid = self.set_cur_ast(jac_ast)
         for i in kid:
             if i.name == "attr_stmt":
                 self.run_attr_stmt(i, obj)
 
-    def run_struct_block(self, jac_ast):
+    def run_attr_stmt(self, jac_ast, obj):
         """
-        struct_block: LBRACE (has_stmt)* RBRACE | COLON has_stmt | SEMI;
+        attr_stmt: has_stmt | can_stmt;
         """
         kid = self.set_cur_ast(jac_ast)
-        ret = {}
-        for i in kid:
-            if i.name == "has_stmt":
-                self.run_has_stmt(i, ret)
-        return ret
+        if kid[0].name == "has_stmt":
+            self.run_has_stmt(kid[0], obj)
+        #  Can statements in architype handled in architype load
 
-    def run_can_block(self, jac_ast):
+    def run_has_stmt(self, jac_ast, obj):
         """
-        can_block: (can_stmt)*;
+        has_stmt: KW_HAS has_assign (COMMA has_assign)* SEMI;
         """
         kid = self.set_cur_ast(jac_ast)
         for i in kid:
-            if i.name == "can_stmt":
-                self.run_can_stmt(i, self)
+            if i.name == "has_assign":
+                self.run_has_assign(i, obj)
 
-    def run_graph_block(self, jac_ast):
+    def run_has_assign(self, jac_ast, obj):
         """
-        graph_block: graph_block_spawn;
+        has_assign: KW_PRIVATE? KW_ANCHOR? (NAME | NAME EQ expression);
         """
         kid = self.set_cur_ast(jac_ast)
-        return getattr(self, f"run_{kid[0].name}")(kid[0])
+        while kid[0].name in ["KW_PRIVATE", "KW_ANCHOR"]:
+            kid = kid[1:]
+        var_name = kid[0].token_text()
+        var_val = None  # jac's null
+        if len(kid) > 1:
+            self.run_expression(kid[2])
+            var_val = self.pop().value
+        if isinstance(obj, dict):
+            obj[var_name] = var_val
+        # Runs only once for walkers
+        elif var_name not in obj.context.keys() or obj.j_type != "walker":
+            JacValue(
+                self, ctx=obj, name=var_name, value=var_val, create_mode=True
+            ).write(kid[0], force=True)
 
-    def run_graph_block_spawn(self, jac_ast):
+    def run_struct_block(self, jac_ast):
+        """
+        struct_block: LBRACE (has_stmt)* RBRACE | COLON has_stmt | SEMI;
+        """
+        kid = self.set_cur_ast(jac_ast)
+        ret = {}
+        for i in kid:
+            if i.name == "has_stmt":
+                self.run_has_stmt(i, ret)
+        return ret
+
+    def run_graph_block(self, jac_ast):
         """
-        graph_block_spawn:
+        graph_block:
             LBRACE has_root can_block KW_SPAWN code_block RBRACE
             | COLON has_root can_block KW_SPAWN code_block SEMI;
         """
         kid = self.set_cur_ast(jac_ast)
         root_name = self.run_has_root(kid[1])
-        self.run_can_block(kid[2])
-        m = Interp(parent_override=self.parent(), caller=self)
-        m.push_scope(
-            JacScope(parent=self, has_obj=None, action_sets=[self.activity_action_ids])
-        )
         try:
-            m.run_code_block(kid[4])
+            self.run_code_block(kid[4])
         except Exception as e:
-            self.rt_error(f"Internal Exception: {e}", m._cur_jac_ast)
-        local_state = m._jac_scope.local_scope
-        self.report = self.report + m.report
+            self.rt_error(f"Internal Exception: {e}", self._cur_jac_ast)
+        local_state = self._jac_scope.local_scope
         if root_name in local_state.keys():
             obj = local_state[root_name]
             if not isinstance(obj, Node):
                 self.rt_error(f"{root_name} is {type(obj)} not node!", kid[3])
             return obj
         else:
             self.rt_error("Graph didn't produce root node!", kid[3])
@@ -169,9 +200,13 @@
         for i in self.super_archs:
             super_jac_ast = (
                 self.parent()
                 .arch_ids.get_obj_by_name(name=i, kind=item.kind)
                 .get_jac_ast()
                 .kid[-1]
             )
-            self.run_attr_block(super_jac_ast, item)
-        self.run_attr_block(jac_ast, item)
+            self.run_attr_block(super_jac_ast, item) if not isinstance(
+                item, Walker
+            ) else self.run_walker_block(super_jac_ast, item)
+        self.run_attr_block(jac_ast, item) if not isinstance(
+            item, Walker
+        ) else self.run_walker_block(jac_ast, item)
```

### Comparing `jaseci-1.4.0.9/jaseci/jac/interpreter/interp.py` & `jaseci-1.4.1.0/jaseci/jac/interpreter/interp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,144 +1,39 @@
 """
 Interpreter for jac code in AST form
 
 This interpreter should be inhereted from the class that manages state
 referenced through self.
 """
+from jaseci.jsorc.jsorc import JsOrc
+from jaseci.extens.svc.task_svc import TaskService
 from jaseci.utils.utils import is_jsonable, parse_str_token, uuid_re
-from jaseci.element.element import Element
-from jaseci.graph.node import Node
-from jaseci.graph.edge import Edge
-from jaseci.attr.action import Action
+from jaseci.prim.element import Element
+from jaseci.prim.node import Node
+from jaseci.prim.edge import Edge
 from jaseci.jac.jac_set import JacSet
 from jaseci.jac.ir.jac_code import jac_ast_to_ir, jac_ir_to_ast
 from jaseci.jac.machine.jac_scope import JacScope
 from jaseci.jac.jsci_vm.machine import VirtualMachine
 from jaseci.jac.machine.machine_state import TryException
 
 from jaseci.jac.machine.jac_value import JacValue
 from jaseci.jac.machine.jac_value import jac_elem_unwrap as jeu
 from jaseci.jac.machine.jac_value import jac_wrap_value as jwv
+from json import dumps, loads
 from copy import copy, deepcopy
 from base64 import b64decode
+from itertools import pairwise
 
 from jaseci.jac.jsci_vm.op_codes import JsCmp
 
 
 class Interp(VirtualMachine):
     """Shared interpreter class across both sentinels and walkers"""
 
-    def run_attr_stmt(self, jac_ast, obj):
-        """
-        attr_stmt: has_stmt | can_stmt;
-        """
-        kid = self.set_cur_ast(jac_ast)
-        if kid[0].name == "has_stmt":
-            self.run_has_stmt(kid[0], obj)
-        #  Can statements in architype handled in architype load
-
-    def run_has_stmt(self, jac_ast, obj):
-        """
-        has_stmt: KW_HAS has_assign (COMMA has_assign)* SEMI;
-        """
-        kid = self.set_cur_ast(jac_ast)
-        for i in kid:
-            if i.name == "has_assign":
-                self.run_has_assign(i, obj)
-
-    def run_has_assign(self, jac_ast, obj):
-        """
-        has_assign: KW_PRIVATE? KW_ANCHOR? (NAME | NAME EQ expression);
-        """
-        kid = self.set_cur_ast(jac_ast)
-        while kid[0].name in ["KW_PRIVATE", "KW_ANCHOR"]:
-            kid = kid[1:]
-        var_name = kid[0].token_text()
-        var_val = None  # jac's null
-        if len(kid) > 1:
-            self.run_expression(kid[2])
-            var_val = self.pop().value
-        if isinstance(obj, dict):
-            obj[var_name] = var_val
-        # Runs only once for walkers
-        elif var_name not in obj.context.keys() or obj.j_type != "walker":
-            JacValue(
-                self, ctx=obj, name=var_name, value=var_val, create_mode=True
-            ).write(kid[0], force=True)
-
-    def run_can_stmt(self, jac_ast, obj):
-        """
-        can_stmt:
-            KW_CAN dotted_name (preset_in_out event_clause)? (
-                COMMA dotted_name (preset_in_out event_clause)?
-            )* SEMI
-            | KW_CAN NAME event_clause? code_block;
-        """
-        kid = self.set_cur_ast(jac_ast)
-        kid = kid[1:]
-        while True:
-            action_type = "activity"
-            access_list = None
-            preset_in_out = None
-            if kid[0].name == "NAME":
-                action_name = kid[0].token_text()
-            else:
-                action_name = self.run_dotted_name(kid[0])
-            kid = kid[1:]
-            if len(kid) > 0 and kid[0].name == "preset_in_out":
-                preset_in_out = jac_ast_to_ir(kid[0])
-                kid = kid[1:]
-            if len(kid) > 0 and kid[0].name == "event_clause":
-                action_type, access_list = self.run_event_clause(kid[0])
-                kid = kid[1:]
-            # if (not isinstance(obj, node) and action_type != 'activity'):
-            #     self.rt_warn(
-            #         "Only nodes has on entry/exit, treating as activity",
-            #         kid[0])
-            #     action_type = 'activity'
-            if kid[0].name == "code_block":
-                act = Action(
-                    m_id=self._m_id,
-                    h=self._h,
-                    name=action_name,
-                    value=jac_ast_to_ir(kid[0]),
-                    preset_in_out=preset_in_out,
-                    access_list=access_list,
-                )
-                getattr(obj, f"{action_type}_action_ids").add_obj(act)
-                self._jac_scope.add_action(act)
-                break
-            else:
-                self.check_builtin_action(action_name, jac_ast)
-                act = Action(
-                    m_id=self._m_id,
-                    h=self._h,
-                    name=action_name,
-                    value=action_name,
-                    preset_in_out=preset_in_out,
-                    access_list=access_list,
-                )
-                getattr(obj, f"{action_type}_action_ids").add_obj(act)
-                self._jac_scope.add_action(act)
-            if not len(kid) or kid[0].name != "COMMA":
-                break
-            else:
-                kid = kid[1:]
-
-    def run_event_clause(self, jac_ast):
-        """
-        event_clause:
-                KW_WITH name_list? (KW_ENTRY | KW_EXIT | KW_ACTIVITY);
-        """
-        kid = self.set_cur_ast(jac_ast)
-        nl = []
-        if kid[1].name == "name_list":
-            nl = self.run_name_list(kid[1])
-        return kid[-1].token_text(), nl
-
     def run_dotted_name(self, jac_ast):
         """
         dotted_name: NAME (DOT NAME)*;
         """
         kid = self.set_cur_ast(jac_ast)
         ret = ""
         for i in kid:
@@ -754,15 +649,15 @@
             | NAME
             | global_ref
             | node_edge_ref
             | list_val
             | dict_val
             | LPAREN expression RPAREN
             | ability_op NAME spawn_ctx?
-            | atom atom_trailer+
+            | atom atom_trailer
             | KW_SYNC atom
             | spawn
             | ref
             | deref
             | any_type;
         """
         try:
@@ -780,51 +675,54 @@
             elif kid[0].name == "NULL":
                 self.push(JacValue(self, value=None))
             elif kid[0].name == "NAME":
                 self.load_variable(kid[0].token_text(), kid[0])
             elif kid[0].name == "LPAREN":
                 self.run_expression(kid[1])
             elif kid[0].name == "ability_op":
-                self.push(self.run_atom_trailer(jac_ast, None))
+                self.push(
+                    self.run_ability_call(
+                        jac_ast, atom_res=JacValue(self, value=self._jac_scope.has_obj)
+                    )
+                )
             elif kid[0].name == "atom":
                 self.run_atom(kid[0])
                 ret = self.pop()
                 for i in kid[1:]:
                     ret = self.run_atom_trailer(i, ret)
                 self.push(ret)
             elif kid[0].name == "KW_SYNC":
                 self.run_atom(kid[1])
                 val = self.pop()
-                task_func = self._h.task
-                if not task_func.is_running():
-                    raise Exception("Task hook is not yet initialized!")
                 self.push(
                     JacValue(
-                        self, value=task_func.get_by_task_id(val.value["result"], True)
+                        self,
+                        value=(
+                            JsOrc.svc("task")
+                            .poke(TaskService)
+                            .get_by_task_id(val.value["result"], True)
+                        ),
                     )
                 )
             else:
                 self.push(self.run_rule(kid[0]))
 
         except Exception as e:
             self.jac_try_exception(e, jac_ast)
 
     def run_atom_trailer(self, jac_ast, atom_res):
         """
         atom_trailer:
             DOT built_in
             | DOT NAME
             | index_slice
-            | LPAREN param_list? RPAREN
-            | ability_op NAME spawn_ctx?;
+            | ability_call;
         """
         try:
             kid = self.set_cur_ast(jac_ast)
-            if atom_res is None:
-                atom_res = JacValue(self, value=self._jac_scope.has_obj)
             if isinstance(atom_res.value, Element):
                 self._write_candidate = atom_res.value
             if kid[0].name == "DOT":
                 if kid[1].name == "built_in":
                     return self.run_built_in(kid[1], atom_res)
                 elif kid[1].name == "NAME":
                     d = atom_res.value
@@ -848,36 +746,48 @@
                         return ret
                     else:
                         self.rt_error(f"Invalid variable {n}", kid[0])
             elif kid[0].name == "index_slice":
                 if not self.rt_check_type(atom_res.value, [list, str, dict], kid[0]):
                     return atom_res
                 return self.run_index_slice(kid[0], atom_res)
-            elif kid[0].name == "LPAREN":
-                param_list = {"args": [], "kwargs": {}}
-                if kid[1].name == "param_list":
-                    param_list = self.run_param_list(kid[1]).value
-                if isinstance(atom_res.value, Action):
-                    ret = atom_res.value.trigger(param_list, self._jac_scope, self)
-                    return JacValue(self, value=ret)
-                else:
-                    self.rt_error("Unable to execute ability", kid[0])
-            elif kid[0].name == "ability_op":
-                arch = self.run_ability_op(kid[0], atom_res)
-                if len(kid) > 2:
-                    self.run_spawn_ctx(kid[2], atom_res.value)
-                self.call_ability(
-                    nd=atom_res.value,
-                    name=kid[1].token_text(),
-                    act_list=arch.get_all_actions(),
-                )
-                return atom_res
+            elif kid[0].name == "ability_call":
+                return self.run_ability_call(kid[0], atom_res)
         except Exception as e:
             self.jac_try_exception(e, jac_ast)
 
+    def run_ability_call(self, jac_ast, atom_res):
+        """
+        ability_call:
+            LPAREN param_list? RPAREN
+            | ability_op NAME spawn_ctx?;
+        """
+        from jaseci.prim.ability import Ability
+
+        kid = self.set_cur_ast(jac_ast)
+        if kid[0].name == "LPAREN":
+            param_list = {"args": [], "kwargs": {}}
+            if kid[1].name == "param_list":
+                param_list = self.run_param_list(kid[1]).value
+            if isinstance(atom_res.value, Ability):
+                ret = atom_res.value.run_action(param_list, self._jac_scope, self)
+                return JacValue(self, value=ret)
+            else:
+                self.rt_error("Unable to execute ability", kid[0])
+        elif kid[0].name == "ability_op":
+            arch = self.run_ability_op(kid[0], atom_res)
+            if len(kid) > 2:
+                self.run_spawn_ctx(kid[2], atom_res.value)
+            self.call_ability(
+                nd=atom_res.value,
+                name=kid[1].token_text(),
+                act_list=arch.get_all_abilities(),
+            )
+            return atom_res
+
     def run_ability_op(self, jac_ast, atom_res):
         """
         ability_op: DBL_COLON | DBL_COLON NAME COLON;
         """
         kid = self.set_cur_ast(jac_ast)
         base_arch = atom_res.value.get_architype()
         if len(kid) > 1:
@@ -943,29 +853,21 @@
         self.run_any_type(kid[0])
         typ = self.pop()
         if typ.value == Edge:
             if isinstance(atom_res.value, Node):
                 return JacValue(
                     self,
                     value=self.obj_set_to_jac_set(
-                        self.current_node.attached_edges(atom_res.value)
+                        self.here().attached_edges(atom_res.value)
                     ),
                 )
             elif isinstance(atom_res.value, Edge):
                 return atom_res
             elif isinstance(atom_res.value, JacSet):
                 return JacValue(self, value=self._relevant_edges)
-                # res = jac_set()
-                # for i in atom_res.value.obj_list():
-                #     if(isinstance(i, edge)):
-                #         res.add_obj(i)
-                #     elif(isinstance(i, node)):
-                #         res += self.obj_set_to_jac_set(
-                #             self.current_node.attached_edges(i))
-                # return jac_value(self, value=res)
             else:
                 self.rt_error(
                     f"Cannot get edges from {atom_res.value}. "
                     f"Type {atom_res.jac_type()} invalid",
                     kid[0],
                 )
         # may want to remove 'here" node from return below
@@ -987,15 +889,20 @@
                 self.rt_error(
                     f"Cannot get nodes from {atom_res}. "
                     f"Type {atom_res.jac_type()} invalid",
                     kid[0],
                 )
         else:
             try:
-                atom_res.value = typ.value(atom_res.value)
+                if isinstance(atom_res.value, str) and typ.value == dict:
+                    atom_res.value = loads(atom_res.value)
+                elif isinstance(atom_res.value, dict) and typ.value == str:
+                    atom_res.value = dumps(atom_res.value)
+                else:
+                    atom_res.value = typ.value(atom_res.value)
             except Exception as e:
                 self.rt_error(
                     f"Invalid cast of {atom_res.jac_type()} "
                     f"to {jwv(typ.value)}: {e}",
                     kid[0],
                 )
             return atom_res
@@ -1003,15 +910,15 @@
         return atom_res
 
     def run_obj_built_in(self, jac_ast, atom_res):
         """
         obj_built_in: KW_CONTEXT | KW_INFO | KW_DETAILS;
         """
         kid = self.set_cur_ast(jac_ast)
-        from jaseci.actor.walker import Walker
+        from jaseci.prim.walker import Walker
 
         if kid[0].name == "KW_CONTEXT":
             if self.rt_check_type(atom_res.value, [Node, Edge, Walker], kid[0]):
                 return JacValue(self, ctx=atom_res.value, value=atom_res.value.context)
         elif kid[0].name == "KW_INFO":
             if self.rt_check_type(atom_res.value, [Node, Edge, Walker], kid[0]):
                 return JacValue(
@@ -1150,14 +1057,21 @@
                     result = JacValue(
                         self, value=atom_res.value.index(max(atom_res.value))
                     )
                 elif op == "idx_of_min":
                     result = JacValue(
                         self, value=atom_res.value.index(min(atom_res.value))
                     )
+                elif op == "pairwise":
+                    result = JacValue(
+                        self, value=[list(s) for s in pairwise(atom_res.value)]
+                    )
+                elif op == "unique":
+                    result = JacValue(self, value=list(set(atom_res.value)))
+
                 elif len(kid) < 2 and op == "pop":
                     result = JacValue(self, value=atom_res.value.pop())
                     self.candidate_writethrough()
                 if result:
                     if len(kid) > 1:
                         self.rt_warn(f"{op} does not take parameters, ignoring", kid[2])
                     return result
@@ -1340,15 +1254,16 @@
         kid = self.set_cur_ast(jac_ast)
         name = kid[-1].token_text()
         wlk = self.yielded_walkers_ids.get_obj_by_name(name, silent=True)
         if wlk is None:
             wlk = self.parent().run_architype(name=name, kind="walker", caller=self)
         if wlk is None:
             self.rt_error(f"No walker {name} exists!", kid[-1])
-        wlk._to_await = to_await
+        else:
+            wlk._to_await = to_await
         return wlk
 
     def run_graph_ref(self, jac_ast):
         """
         graph_ref: GRAPH_DBL_COLON NAME;
         """
         kid = self.set_cur_ast(jac_ast)
@@ -1378,15 +1293,15 @@
         """
         edge_to:
             '-->'
             | '-' ('[' NAME (spawn_ctx | filter_ctx)? ']')? '->';
         """
         kid = self.set_cur_ast(jac_ast)
         if not location:
-            location = self.current_node
+            location = self.here()
         result = JacSet()
         for i in location.outbound_edges() + location.bidirected_edges():
             if len(kid) > 2 and not i.get_architype().is_instance(kid[2].token_text()):
                 continue
             result.add_obj(i)
         if len(kid) > 2 and kid[3].name == "filter_ctx":
             result = self.run_filter_ctx(kid[3], result)
@@ -1398,15 +1313,15 @@
         """
         edge_from:
             '<--'
             | '<-' ('[' NAME (spawn_ctx | filter_ctx)? ']')? '-';
         """
         kid = self.set_cur_ast(jac_ast)
         if not location:
-            location = self.current_node
+            location = self.here()
         result = JacSet()
         for i in location.inbound_edges() + location.bidirected_edges():
             if len(kid) > 2 and not i.get_architype().is_instance(kid[2].token_text()):
                 continue
             result.add_obj(i)
         if len(kid) > 2 and kid[3].name == "filter_ctx":
             result = self.run_filter_ctx(kid[3], result)
@@ -1419,15 +1334,15 @@
         edge_any:
             '<-->'
             | '<-' ('[' NAME (spawn_ctx | filter_ctx)? ']')? '->';
         NOTE: these do not use strict bidirected semantic but any edge
         """
         kid = self.set_cur_ast(jac_ast)
         if not location:
-            location = self.current_node
+            location = self.here()
         result = JacSet()
         for i in location.attached_edges():
             if len(kid) > 2 and not i.get_architype().is_instance(kid[2].token_text()):
                 continue
             result.add_obj(i)
         if len(kid) > 2 and kid[3].name == "filter_ctx":
             result = self.run_filter_ctx(kid[3], result)
@@ -1798,32 +1713,26 @@
     def attempt_bytecode(self, jac_ast):
         if hasattr(jac_ast, "bytecode") and jac_ast.bytecode:
             self.run_bytecode(b64decode(jac_ast.bytecode.encode()))
             return True
         return False
 
     def call_ability(self, nd, name, act_list):
-        m = Interp(parent_override=self.parent(), caller=self)
-        m.current_node = nd
-        arch = nd.get_architype()
-        m.push_scope(
-            JacScope(parent=self, has_obj=nd, action_sets=[arch.get_all_actions()])
-        )
-        m._jac_scope.inherit_agent_refs(self._jac_scope, nd)
+        ability = act_list.get_obj_by_name(name)
         try:
-            m.run_code_block(jac_ir_to_ast(act_list.get_obj_by_name(name).value))
+            ability.run_ability(here=nd, visitor=self._jac_scope.visitor())
         except Exception as e:
-            self.rt_error(f"Internal Exception: {e}", m._cur_jac_ast)
-        self.inherit_runtime_state(m)
+            self.rt_error(f"Internal Exception: {e}", ability._cur_jac_ast)
+        self.inherit_runtime_state(ability)
 
     def visibility_prune(self, node_set=None):
         """Returns all nodes that shouldnt be ignored"""
         ret = JacSet()
         if node_set is None:
-            node_set = self.current_node.attached_nodes()
+            node_set = self.here().attached_nodes()
         for i in node_set:
             if i not in self.ignore_node_ids.obj_list():
                 ret.add_obj(i)
         return ret
 
     def run_rule(self, jac_ast, *args):
         """Helper to run rule if exists in execution context"""
```

### Comparing `jaseci-1.4.0.9/jaseci/jac/interpreter/sentinel_interp.py` & `jaseci-1.4.1.0/jaseci/jac/interpreter/sentinel_interp.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """
 Sentinel interpreter for jac code in AST form
 
 This interpreter should be inhereted from the class that manages state
 referenced through self.
 """
-from jaseci.actor.architype import Architype
+from jaseci.prim.architype import Architype
 from jaseci.jac.interpreter.interp import Interp
 from jaseci.utils.utils import parse_str_token
 from jaseci.jac.ir.jac_code import jac_ast_to_ir
 from jaseci.jac.machine.jac_scope import JacScope
+from jaseci.prim.ability import Ability
 
 
 class SentinelInterp(Interp):
     """Jac interpreter mixin for objects that will execute Jac code"""
 
     def run_start(self, jac_ast):
         """
@@ -120,25 +121,92 @@
                                 arch.anchor_var = var_name
                             arch.has_vars.append(var_name)
         arch.save()
 
     def arch_can_compile(self, jac_ast, arch):
         """Helper function to statically compile can stmts for arch"""
         kid = self.set_cur_ast(jac_ast)
-        self.push_scope(JacScope(parent=self, has_obj=self, action_sets=[]))
+        self.push_scope(
+            JacScope(parent=self, name=f"a_cgen:{jac_ast.loc_str()}", has_obj=None)
+        )
         if jac_ast.name in ["attr_block", "walker_block"]:
             for i in kid:
                 if i.name == "attr_stmt" and i.kid[0].name == "can_stmt":
                     self.run_can_stmt(i.kid[0], arch)
-        elif kid[0].name == "graph_block_spawn":
-            kid = kid[0].kid[2].kid
-            for i in kid:
-                self.run_can_stmt(i, arch)
+        elif jac_ast.name == "graph_block":
+            self.run_can_block(jac_ast.kid[2], arch)
         self.pop_scope()
 
+    def run_can_block(self, jac_ast, arch):
+        """
+        can_block: (can_stmt)*;
+        """
+        kid = self.set_cur_ast(jac_ast)
+        for i in kid:
+            if i.name == "can_stmt":
+                self.run_can_stmt(i, arch)
+
+    def run_can_stmt(self, jac_ast, obj):
+        """
+        can_stmt:
+            KW_CAN dotted_name (preset_in_out event_clause)? (
+                COMMA dotted_name (preset_in_out event_clause)?
+            )* SEMI
+            | KW_CAN NAME event_clause? code_block;
+        """
+        kid = self.set_cur_ast(jac_ast)
+        kid = kid[1:]
+        ir = None
+        while True:
+            action_type = "activity"
+            access_list = None
+            preset_in_out = None
+            if kid[0].name == "NAME":
+                action_name = kid[0].token_text()
+            else:
+                action_name = self.run_dotted_name(kid[0])
+            kid = kid[1:]
+            if len(kid) > 0 and kid[0].name == "preset_in_out":
+                preset_in_out = jac_ast_to_ir(kid[0])
+                kid = kid[1:]
+            if len(kid) > 0 and kid[0].name == "event_clause":
+                action_type, access_list = self.run_event_clause(kid[0])
+                kid = kid[1:]
+            if kid[0].name != "code_block":
+                self.check_builtin_action(action_name, jac_ast)
+            else:
+                ir = kid[0]
+            getattr(obj, f"{action_type}_ability_ids").add_obj(
+                Ability(
+                    m_id=self._m_id,
+                    h=self._h,
+                    name=action_name,
+                    kind="ability",
+                    code_ir=ir,
+                    preset_in_out=preset_in_out,
+                    access_list=access_list,
+                    parent=self,
+                )
+            )
+            if not len(kid) or kid[0].name != "COMMA":
+                break
+            else:
+                kid = kid[1:]
+
+    def run_event_clause(self, jac_ast):
+        """
+        event_clause:
+                KW_WITH name_list? (KW_ENTRY | KW_EXIT | KW_ACTIVITY);
+        """
+        kid = self.set_cur_ast(jac_ast)
+        nl = []
+        if kid[1].name == "name_list":
+            nl = self.run_name_list(kid[1])
+        return kid[-1].token_text(), nl
+
     def load_test(self, jac_ast):
         """
         test:
             KW_TEST NAME? multistring KW_WITH (
                 graph_ref
                 | KW_GRAPH graph_block
             ) KW_BY (
```

### Comparing `jaseci-1.4.0.9/jaseci/jac/interpreter/tests/test_interp.py` & `jaseci-1.4.1.0/jaseci/jac/interpreter/tests/test_interp.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.0.9/jaseci/jac/interpreter/walker_interp.py` & `jaseci-1.4.1.0/jaseci/jac/interpreter/walker_interp.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """
 Walker interpreter for jac code in AST form
 
 This interpreter should be inhereted from the class that manages state
 referenced through self.
 """
-from jaseci.graph.node import Node
+from jaseci.prim.node import Node
 from jaseci.jac.interpreter.interp import Interp
 from jaseci.jac.jac_set import JacSet
 from jaseci.jac.machine.jac_scope import JacScope
 from jaseci.jac.ir.jac_code import jac_ir_to_ast
-from jaseci.utils.id_list import IdList
 
 
 class WalkerInterp(Interp):
     """Jac interpreter mixin for objects that will execute Jac code"""
 
     # Walker only executes statements, sentinels handle attr_stmts
 
@@ -21,49 +20,39 @@
         """
         walker: KW_ASYNC? KW_WALKER NAME namespaces? walker_block;
         """
         kid = self.set_cur_ast(jac_ast)
         self.scope_and_run(
             jac_ast if jac_ast.name == "walker_block" else kid[-1],
             self.run_walker_block,
+            scope_name=f"w_run:{jac_ast.loc_str()}",
         )
 
     def run_walker_block(self, jac_ast):
         """
         walker_block:
             LBRACE attr_stmt* walk_entry_block? (
                 statement
                 | walk_activity_block
             )* walk_exit_block? RBRACE;
         """
         kid = self.set_cur_ast(jac_ast)
-        if self.current_step == 0:
-            for i in kid:
-                if i.name == "attr_stmt":
-                    self.run_attr_stmt(jac_ast=i, obj=self)
-        archs = self.current_node.get_architype().arch_with_supers()
-        act_list = IdList(self)
-        for i in archs:
-            act_list += i.entry_action_ids
-        self.auto_trigger_node_actions(nd=self.current_node, act_list=act_list)
+        act_list = self.current_node.get_architype().get_entry_abilities()
+        self.auto_trigger_node_actions(act_list=act_list)
 
         for i in kid:
             if i.name == "walk_entry_block":
                 self.run_walk_entry_block(i)
             if i.name == "statement":
                 self.run_statement(i)
             if i.name == "walk_activity_block":
                 self.run_walk_activity_block(i)
 
-        # self.trigger_activity_actions()
-        archs = self.current_node.get_architype().arch_with_supers()
-        act_list = IdList(self)
-        for i in archs:
-            act_list += i.exit_action_ids
-        self.auto_trigger_node_actions(nd=self.current_node, act_list=act_list)
+        act_list = self.current_node.get_architype().get_exit_abilities()
+        self.auto_trigger_node_actions(act_list=act_list)
 
         if not self.yielded and kid[-2].name == "walk_exit_block":
             self.run_walk_exit_block(kid[-2])
 
     def run_node_ctx_block(self, jac_ast):
         """
         node_ctx_block: name_list code_block;
@@ -186,75 +175,75 @@
         """
         kid = self.set_cur_ast(jac_ast)
         if len(kid) and kid[1].name != "SEMI":
             expr_func = getattr(self, f"run_{kid[1].name}")
             expr_func(kid[1])
         self.yield_walk()
 
-    def run_preset_in_out(self, jac_ast, obj, act):
+    def run_preset_in_out(self, jac_ast, act):
         """
         preset_in_out:
             DBL_COLON param_list? (DBL_COLON | COLON_OUT expression);
 
         obj: The node or edge with preset
         act: The action associated with preset
         """
         kid = self.set_cur_ast(jac_ast)
         param_list = {"args": [], "kwargs": []}
-        m = Interp(parent_override=self.parent(), caller=self)
-        arch = obj.get_architype()
-        m.push_scope(
-            JacScope(parent=self, has_obj=obj, action_sets=[arch.activity_action_ids])
+        self.push_scope(
+            JacScope(
+                parent=self,
+                name=f"p_in_out:{jac_ast.loc_str()}",
+                has_obj=self.current_node,
+                here=self.current_node,
+                visitor=self,
+            )
         )
-        m._jac_scope.set_agent_refs(cur_node=self.current_node, cur_walker=self)
 
         if kid[1].name == "param_list":
-            param_list = m.run_param_list(kid[1]).value
+            param_list = self.run_param_list(kid[1]).value
         try:
-            result = act.trigger(param_list, self._jac_scope, self)
+            result = act.run_action(param_list, self._jac_scope, self)
         except Exception as e:
-            self.rt_error(f"Internal Exception: {e}", m._cur_jac_ast)
+            self.rt_error(f"Internal Exception: {e}", self._cur_jac_ast)
             result = None
         if kid[-1].name == "expression":
-            m.run_expression(kid[-1])
-            dest = m.pop()
+            self.run_expression(kid[-1])
+            dest = self.pop()
             dest.value = result
             dest.write(kid[-1])
+        self.pop_scope()
 
     # Helper Functions ##################
-    def auto_trigger_node_actions(self, nd, act_list):
+    def auto_trigger_node_actions(self, act_list):
         already_executed = []  # handles inhereted duplicates, (overriding)
+        nd = self.current_node
         for i in act_list.obj_list():
             if (
                 i.access_list
                 and self.name not in i.access_list
                 or i.name in already_executed
             ):
                 continue
             if i.preset_in_out:
-                self.run_preset_in_out(jac_ir_to_ast(i.preset_in_out), nd, i)
+                self.run_preset_in_out(jac_ir_to_ast(i.preset_in_out), i)
             else:
                 self.call_ability(nd=nd, name=i.name, act_list=act_list)
             if not i.preset_in_out:  # All preset in and outs get executed
                 already_executed.append(i.name)
 
-    def scope_and_run(self, jac_ast, run_func):
+    def scope_and_run(self, jac_ast, run_func, scope_name):
         """
         Helper to run ast elements with execution scope added
         (Useful for running arbitrary code blocks as one-offs)
         """
-        node_arch = self.current_node.get_architype()
-        walk_arch = self.get_architype()
         self.push_scope(
             JacScope(
                 parent=self,
+                name=scope_name,
                 has_obj=self,
-                action_sets=[
-                    walk_arch.activity_action_ids,
-                    node_arch.activity_action_ids,
-                ],
+                here=self.current_node,
+                visitor=self,
             )
         )
-        self._jac_scope.set_agent_refs(cur_node=self.current_node, cur_walker=self)
-
         run_func(jac_ast)
         self.pop_scope()
```

### Comparing `jaseci-1.4.0.9/jaseci/jac/ir/ast.py` & `jaseci-1.4.1.0/jaseci/jac/ir/ast.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,20 @@
 
     def __init__(
         self,
         mod_name,
     ):
         self.name = "unparsed"
         self.kid = []
-        self.loc = [0, 0, mod_name if mod_name is not None else "@default", {}]
+        self.loc = [
+            0,
+            0,
+            mod_name if mod_name is not None else "@default",
+            {},
+        ]  # line, col, module, tokens
 
     def is_terminal(self):
         """Returns true if node is a terminal"""
         return len(self.loc[3].keys())
 
     def token(self):
         if not self.is_terminal():
@@ -33,14 +38,17 @@
         if self.is_terminal():
             return self.token()["text"]
 
     def token_symbol(self):
         if self.is_terminal():
             return self.token()["symbol"]
 
+    def loc_str(self):
+        return f"{self.loc[2]}:{self.loc[0]}"
+
     def __str__(self):
         res = f"{self.name}:{self.loc[2]}:{self.loc[0]}:{self.loc[1]}:"
         if self.is_terminal():
             res += f':{self.loc[3]["token"]["text"]}'
         return res
 
     def __repr__(self):
```

### Comparing `jaseci-1.4.0.9/jaseci/jac/ir/ast_builder.py` & `jaseci-1.4.1.0/jaseci/jac/ir/ast_builder.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.0.9/jaseci/jac/ir/jac_code.py` & `jaseci-1.4.1.0/jaseci/jac/ir/jac_code.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.0.9/jaseci/jac/ir/passes/codegen_pass.py` & `jaseci-1.4.1.0/jaseci/jac/ir/passes/codegen_pass.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.0.9/jaseci/jac/ir/passes/ir_pass.py` & `jaseci-1.4.1.0/jaseci/jac/ir/passes/ir_pass.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.0.9/jaseci/jac/ir/passes/printer_pass.py` & `jaseci-1.4.1.0/jaseci/jac/ir/passes/printer_pass.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.0.9/jaseci/jac/ir/passes/pt_prune_pass.py` & `jaseci-1.4.1.0/jaseci/jac/ir/passes/pt_prune_pass.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.0.9/jaseci/jac/ir/passes/schedule.py` & `jaseci-1.4.1.0/jaseci/jac/ir/passes/schedule.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.0.9/jaseci/jac/jac.g4` & `jaseci-1.4.1.0/jaseci/jac/jac.g4`

 * *Files 2% similar despite different names*

```diff
@@ -68,17 +68,15 @@
 
 attr_stmt: has_stmt | can_stmt;
 
 struct_block: LBRACE (has_stmt)* RBRACE | COLON has_stmt | SEMI;
 
 can_block: (can_stmt)*;
 
-graph_block: graph_block_spawn;
-
-graph_block_spawn:
+graph_block:
 	LBRACE has_root can_block KW_SPAWN code_block RBRACE
 	| COLON has_root can_block KW_SPAWN code_block SEMI;
 
 has_root: KW_HAS KW_ANCHOR NAME SEMI;
 
 has_stmt: KW_HAS has_assign (COMMA has_assign)* SEMI;
 
@@ -224,15 +222,18 @@
 	| deref
 	| any_type;
 
 atom_trailer:
 	DOT built_in
 	| DOT NAME
 	| index_slice
-	| LPAREN param_list? RPAREN
+	| ability_call;
+
+ability_call:
+	LPAREN param_list? RPAREN
 	| ability_op NAME spawn_ctx?;
 
 ability_op: DBL_COLON | DBL_COLON NAME COLON;
 
 ref: KW_REF atom;
 
 deref: STAR_MUL atom;
```

### Comparing `jaseci-1.4.0.9/jaseci/jac/jac_parse/jacLexer.py` & `jaseci-1.4.1.0/jaseci/jac/jac_parse/jacLexer.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.0.9/jaseci/jac/jac_parse/jacListener.py` & `jaseci-1.4.1.0/jaseci/jac/jac_parse/jacListener.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,22 +157,14 @@
     def enterGraph_block(self, ctx: jacParser.Graph_blockContext):
         pass
 
     # Exit a parse tree produced by jacParser#graph_block.
     def exitGraph_block(self, ctx: jacParser.Graph_blockContext):
         pass
 
-    # Enter a parse tree produced by jacParser#graph_block_spawn.
-    def enterGraph_block_spawn(self, ctx: jacParser.Graph_block_spawnContext):
-        pass
-
-    # Exit a parse tree produced by jacParser#graph_block_spawn.
-    def exitGraph_block_spawn(self, ctx: jacParser.Graph_block_spawnContext):
-        pass
-
     # Enter a parse tree produced by jacParser#has_root.
     def enterHas_root(self, ctx: jacParser.Has_rootContext):
         pass
 
     # Exit a parse tree produced by jacParser#has_root.
     def exitHas_root(self, ctx: jacParser.Has_rootContext):
         pass
@@ -533,14 +525,22 @@
     def enterAtom_trailer(self, ctx: jacParser.Atom_trailerContext):
         pass
 
     # Exit a parse tree produced by jacParser#atom_trailer.
     def exitAtom_trailer(self, ctx: jacParser.Atom_trailerContext):
         pass
 
+    # Enter a parse tree produced by jacParser#ability_call.
+    def enterAbility_call(self, ctx: jacParser.Ability_callContext):
+        pass
+
+    # Exit a parse tree produced by jacParser#ability_call.
+    def exitAbility_call(self, ctx: jacParser.Ability_callContext):
+        pass
+
     # Enter a parse tree produced by jacParser#ability_op.
     def enterAbility_op(self, ctx: jacParser.Ability_opContext):
         pass
 
     # Exit a parse tree produced by jacParser#ability_op.
     def exitAbility_op(self, ctx: jacParser.Ability_opContext):
         pass
```

### Comparing `jaseci-1.4.0.9/jaseci/jac/jac_parse/jacParser.py` & `jaseci-1.4.1.0/jaseci/jac/jac_parse/jacParser.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 else:
     from typing.io import TextIO
 
 
 def serializedATN():
     with StringIO() as buf:
         buf.write("\3\u608b\ua72a\u8133\ub9ed\u417c\u3be7\u7786\u5964\3s")
-        buf.write("\u04a4\4\2\t\2\4\3\t\3\4\4\t\4\4\5\t\5\4\6\t\6\4\7\t\7")
+        buf.write("\u04a5\4\2\t\2\4\3\t\3\4\4\t\4\4\5\t\5\4\6\t\6\4\7\t\7")
         buf.write("\4\b\t\b\4\t\t\t\4\n\t\n\4\13\t\13\4\f\t\f\4\r\t\r\4\16")
         buf.write("\t\16\4\17\t\17\4\20\t\20\4\21\t\21\4\22\t\22\4\23\t\23")
         buf.write("\4\24\t\24\4\25\t\25\4\26\t\26\4\27\t\27\4\30\t\30\4\31")
         buf.write("\t\31\4\32\t\32\4\33\t\33\4\34\t\34\4\35\t\35\4\36\t\36")
         buf.write('\4\37\t\37\4 \t \4!\t!\4"\t"\4#\t#\4$\t$\4%\t%\4&\t')
         buf.write("&\4'\t'\4(\t(\4)\t)\4*\t*\4+\t+\4,\t,\4-\t-\4.\t.\4")
         buf.write("/\t/\4\60\t\60\4\61\t\61\4\62\t\62\4\63\t\63\4\64\t\64")
@@ -49,116 +49,117 @@
         buf.write("\13\u0194\n\13\3\13\3\13\5\13\u0198\n\13\3\13\3\13\5\13")
         buf.write("\u019c\n\13\3\f\3\f\3\f\3\r\3\r\3\r\3\r\3\16\3\16\3\16")
         buf.write("\3\16\3\17\3\17\3\17\3\17\3\20\3\20\7\20\u01af\n\20\f")
         buf.write("\20\16\20\u01b2\13\20\3\20\3\20\3\20\3\20\5\20\u01b8\n")
         buf.write("\20\3\21\3\21\5\21\u01bc\n\21\3\22\3\22\7\22\u01c0\n\22")
         buf.write("\f\22\16\22\u01c3\13\22\3\22\3\22\3\22\3\22\5\22\u01c9")
         buf.write("\n\22\3\23\7\23\u01cc\n\23\f\23\16\23\u01cf\13\23\3\24")
-        buf.write("\3\24\3\25\3\25\3\25\3\25\3\25\3\25\3\25\3\25\3\25\3\25")
-        buf.write("\3\25\3\25\3\25\3\25\5\25\u01e1\n\25\3\26\3\26\3\26\3")
-        buf.write("\26\3\26\3\27\3\27\3\27\3\27\7\27\u01ec\n\27\f\27\16\27")
-        buf.write("\u01ef\13\27\3\27\3\27\3\30\5\30\u01f4\n\30\3\30\5\30")
-        buf.write("\u01f7\n\30\3\30\3\30\3\30\3\30\5\30\u01fd\n\30\3\31\3")
-        buf.write("\31\3\31\3\31\3\31\5\31\u0204\n\31\3\31\3\31\3\31\3\31")
-        buf.write("\3\31\5\31\u020b\n\31\7\31\u020d\n\31\f\31\16\31\u0210")
-        buf.write("\13\31\3\31\3\31\3\31\3\31\3\31\5\31\u0217\n\31\3\31\5")
-        buf.write("\31\u021a\n\31\3\32\3\32\5\32\u021e\n\32\3\32\3\32\3\33")
-        buf.write("\3\33\5\33\u0224\n\33\3\33\3\33\3\33\5\33\u0229\n\33\3")
-        buf.write("\34\3\34\3\34\3\34\3\35\3\35\3\35\7\35\u0232\n\35\f\35")
-        buf.write("\16\35\u0235\13\35\3\36\3\36\3\36\3\36\3\36\3\36\5\36")
-        buf.write("\u023d\n\36\3\37\3\37\3\37\7\37\u0242\n\37\f\37\16\37")
-        buf.write("\u0245\13\37\3 \3 \3 \3 \3 \3 \3 \7 \u024e\n \f \16 \u0251")
-        buf.write("\13 \3!\3!\7!\u0255\n!\f!\16!\u0258\13!\3!\3!\3!\5!\u025d")
-        buf.write('\n!\3"\3"\3"\3#\3#\3#\3#\3#\3#\3#\3#\3#\3#\3#\3#\3')
-        buf.write("#\3#\3#\3#\3#\3#\5#\u0274\n#\3$\3$\3$\3$\7$\u027a\n$\f")
-        buf.write("$\16$\u027d\13$\3$\5$\u0280\n$\3%\3%\3%\5%\u0285\n%\3")
-        buf.write("&\3&\3&\3&\5&\u028b\n&\3&\3&\3&\3&\5&\u0291\n&\3&\5&\u0294")
-        buf.write("\n&\3'\3'\3'\3'\3(\3(\3(\3)\3)\3)\3)\3)\3)\3)\3)\3")
-        buf.write(")\3)\3)\3)\5)\u02a9\n)\3)\3)\3)\3)\5)\u02af\n)\3*\3*\3")
-        buf.write("*\3*\3+\3+\3,\3,\3,\3-\3-\3-\3-\3.\3.\3.\3.\3.\3.\3.\3")
-        buf.write(".\3.\3.\3.\5.\u02c9\n.\3/\3/\3/\3/\5/\u02cf\n/\3\60\3")
-        buf.write("\60\3\60\3\60\3\61\3\61\3\61\5\61\u02d8\n\61\3\61\3\61")
-        buf.write("\3\61\5\61\u02dd\n\61\3\62\3\62\3\62\5\62\u02e2\n\62\3")
-        buf.write("\63\3\63\3\63\3\63\3\63\5\63\u02e9\n\63\3\64\3\64\3\64")
-        buf.write("\3\64\5\64\u02ef\n\64\3\65\3\65\3\65\3\66\3\66\3\66\3")
-        buf.write("\67\3\67\3\67\38\38\38\38\58\u02fe\n8\38\38\58\u0302\n")
-        buf.write("8\39\39\39\79\u0307\n9\f9\169\u030a\139\3:\3:\3:\3:\3")
-        buf.write(":\3:\7:\u0312\n:\f:\16:\u0315\13:\5:\u0317\n:\3;\3;\3")
-        buf.write(";\3;\3;\3;\3;\3;\5;\u0321\n;\3<\3<\3<\3=\3=\3=\7=\u0329")
-        buf.write("\n=\f=\16=\u032c\13=\3>\3>\3>\7>\u0331\n>\f>\16>\u0334")
-        buf.write("\13>\3?\3?\3?\5?\u0339\n?\3@\3@\3@\7@\u033e\n@\f@\16@")
-        buf.write("\u0341\13@\3A\3A\3A\3A\5A\u0347\nA\3B\3B\3B\3B\3B\3B\3")
-        buf.write("B\3B\3B\3B\3B\3B\3B\3B\3B\3B\3B\3B\5B\u035b\nB\3B\3B\3")
-        buf.write("B\3B\3B\3B\5B\u0363\nB\3B\3B\7B\u0367\nB\fB\16B\u036a")
-        buf.write("\13B\3C\3C\3C\3C\3C\3C\3C\5C\u0373\nC\3C\3C\3C\3C\5C\u0379")
-        buf.write("\nC\5C\u037b\nC\3D\3D\3D\3D\5D\u0381\nD\3E\3E\3E\3F\3")
-        buf.write("F\3F\3G\3G\3G\3G\3G\3G\5G\u038f\nG\3H\3H\3I\3I\3J\3J\3")
-        buf.write("J\3J\3J\3J\3J\3J\5J\u039d\nJ\3J\3J\3J\3J\3J\5J\u03a4\n")
-        buf.write("J\5J\u03a6\nJ\3K\3K\3K\3K\5K\u03ac\nK\3K\3K\3K\3K\3K\5")
-        buf.write("K\u03b3\nK\5K\u03b5\nK\3L\3L\3L\5L\u03ba\nL\3L\3L\3L\3")
-        buf.write("L\3L\5L\u03c1\nL\3M\3M\5M\u03c5\nM\3M\5M\u03c8\nM\3M\3")
-        buf.write("M\5M\u03cc\nM\5M\u03ce\nM\3N\3N\3N\3O\3O\3O\3P\3P\3P\3")
-        buf.write("Q\3Q\3Q\3R\3R\3R\5R\u03df\nR\3S\3S\3S\3S\3S\5S\u03e6\n")
-        buf.write("S\3S\5S\u03e9\nS\3S\5S\u03ec\nS\3T\3T\3T\3T\3T\5T\u03f3")
-        buf.write("\nT\3T\5T\u03f6\nT\3T\5T\u03f9\nT\3U\3U\3U\3U\3U\5U\u0400")
-        buf.write("\nU\3U\5U\u0403\nU\3U\5U\u0406\nU\3V\3V\3V\5V\u040b\n")
-        buf.write("V\3W\3W\3W\3W\3W\5W\u0412\nW\3W\5W\u0415\nW\3W\5W\u0418")
-        buf.write("\nW\3X\3X\3X\3X\3X\5X\u041f\nX\3X\5X\u0422\nX\3X\5X\u0425")
-        buf.write("\nX\3Y\3Y\3Y\3Y\3Y\5Y\u042c\nY\3Y\5Y\u042f\nY\3Y\5Y\u0432")
-        buf.write("\nY\3Z\3Z\5Z\u0436\nZ\3Z\3Z\3[\3[\3[\3[\3[\3[\3[\3[\3")
-        buf.write("[\3[\5[\u0444\n[\3\\\3\\\3\\\3\\\7\\\u044a\n\\\f\\\16")
-        buf.write("\\\u044d\13\\\5\\\u044f\n\\\3\\\3\\\3]\3]\3]\3]\3^\3^")
-        buf.write("\3^\3_\3_\3_\3_\5_\u045e\n_\3`\3`\3`\3a\5a\u0464\na\3")
-        buf.write("a\3a\5a\u0468\na\3b\5b\u046b\nb\3b\3b\3c\3c\5c\u0471\n")
-        buf.write("c\3c\3c\5c\u0475\nc\3d\3d\5d\u0479\nd\3e\3e\3e\3e\7e\u047f")
-        buf.write("\ne\fe\16e\u0482\13e\5e\u0484\ne\3e\3e\3f\3f\3f\3f\7f")
-        buf.write("\u048c\nf\ff\16f\u048f\13f\5f\u0491\nf\3f\3f\3g\3g\3g")
-        buf.write("\3g\3h\3h\3h\3h\3i\3i\3j\6j\u04a0\nj\rj\16j\u04a1\3j\2")
-        buf.write('\3\u0082k\2\4\6\b\n\f\16\20\22\24\26\30\32\34\36 "$&')
+        buf.write("\3\24\3\24\3\24\3\24\3\24\3\24\3\24\3\24\3\24\3\24\3\24")
+        buf.write("\3\24\3\24\5\24\u01df\n\24\3\25\3\25\3\25\3\25\3\25\3")
+        buf.write("\26\3\26\3\26\3\26\7\26\u01ea\n\26\f\26\16\26\u01ed\13")
+        buf.write("\26\3\26\3\26\3\27\5\27\u01f2\n\27\3\27\5\27\u01f5\n\27")
+        buf.write("\3\27\3\27\3\27\3\27\5\27\u01fb\n\27\3\30\3\30\3\30\3")
+        buf.write("\30\3\30\5\30\u0202\n\30\3\30\3\30\3\30\3\30\3\30\5\30")
+        buf.write("\u0209\n\30\7\30\u020b\n\30\f\30\16\30\u020e\13\30\3\30")
+        buf.write("\3\30\3\30\3\30\3\30\5\30\u0215\n\30\3\30\5\30\u0218\n")
+        buf.write("\30\3\31\3\31\5\31\u021c\n\31\3\31\3\31\3\32\3\32\5\32")
+        buf.write("\u0222\n\32\3\32\3\32\3\32\5\32\u0227\n\32\3\33\3\33\3")
+        buf.write("\33\3\33\3\34\3\34\3\34\7\34\u0230\n\34\f\34\16\34\u0233")
+        buf.write("\13\34\3\35\3\35\3\35\3\35\3\35\3\35\5\35\u023b\n\35\3")
+        buf.write("\36\3\36\3\36\7\36\u0240\n\36\f\36\16\36\u0243\13\36\3")
+        buf.write("\37\3\37\3\37\3\37\3\37\3\37\3\37\7\37\u024c\n\37\f\37")
+        buf.write("\16\37\u024f\13\37\3 \3 \7 \u0253\n \f \16 \u0256\13 ")
+        buf.write('\3 \3 \3 \5 \u025b\n \3!\3!\3!\3"\3"\3"\3"\3"\3"')
+        buf.write('\3"\3"\3"\3"\3"\3"\3"\3"\3"\3"\3"\3"\5"\u0272')
+        buf.write('\n"\3#\3#\3#\3#\7#\u0278\n#\f#\16#\u027b\13#\3#\5#\u027e')
+        buf.write("\n#\3$\3$\3$\5$\u0283\n$\3%\3%\3%\3%\5%\u0289\n%\3%\3")
+        buf.write("%\3%\3%\5%\u028f\n%\3%\5%\u0292\n%\3&\3&\3&\3&\3'\3'")
+        buf.write("\3'\3(\3(\3(\3(\3(\3(\3(\3(\3(\3(\3(\3(\5(\u02a7\n(\3")
+        buf.write("(\3(\3(\3(\5(\u02ad\n(\3)\3)\3)\3)\3*\3*\3+\3+\3+\3,\3")
+        buf.write(",\3,\3,\3-\3-\3-\3-\3-\3-\3-\3-\3-\3-\3-\5-\u02c7\n-\3")
+        buf.write(".\3.\3.\3.\5.\u02cd\n.\3/\3/\3/\3/\3\60\3\60\3\60\5\60")
+        buf.write("\u02d6\n\60\3\60\3\60\3\60\5\60\u02db\n\60\3\61\3\61\3")
+        buf.write("\61\5\61\u02e0\n\61\3\62\3\62\3\62\3\62\3\62\5\62\u02e7")
+        buf.write("\n\62\3\63\3\63\3\63\3\63\5\63\u02ed\n\63\3\64\3\64\3")
+        buf.write("\64\3\65\3\65\3\65\3\66\3\66\3\66\3\67\3\67\3\67\3\67")
+        buf.write("\5\67\u02fc\n\67\3\67\3\67\5\67\u0300\n\67\38\38\38\7")
+        buf.write("8\u0305\n8\f8\168\u0308\138\39\39\39\39\39\39\79\u0310")
+        buf.write("\n9\f9\169\u0313\139\59\u0315\n9\3:\3:\3:\3:\3:\3:\3:")
+        buf.write("\3:\5:\u031f\n:\3;\3;\3;\3<\3<\3<\7<\u0327\n<\f<\16<\u032a")
+        buf.write("\13<\3=\3=\3=\7=\u032f\n=\f=\16=\u0332\13=\3>\3>\3>\5")
+        buf.write(">\u0337\n>\3?\3?\3?\7?\u033c\n?\f?\16?\u033f\13?\3@\3")
+        buf.write("@\3@\3@\5@\u0345\n@\3A\3A\3A\3A\3A\3A\3A\3A\3A\3A\3A\3")
+        buf.write("A\3A\3A\3A\3A\3A\3A\5A\u0359\nA\3A\3A\3A\3A\3A\3A\5A\u0361")
+        buf.write("\nA\3A\3A\7A\u0365\nA\fA\16A\u0368\13A\3B\3B\3B\3B\3B")
+        buf.write("\3B\5B\u0370\nB\3C\3C\5C\u0374\nC\3C\3C\3C\3C\5C\u037a")
+        buf.write("\nC\5C\u037c\nC\3D\3D\3D\3D\5D\u0382\nD\3E\3E\3E\3F\3")
+        buf.write("F\3F\3G\3G\3G\3G\3G\3G\5G\u0390\nG\3H\3H\3I\3I\3J\3J\3")
+        buf.write("J\3J\3J\3J\3J\3J\5J\u039e\nJ\3J\3J\3J\3J\3J\5J\u03a5\n")
+        buf.write("J\5J\u03a7\nJ\3K\3K\3K\3K\5K\u03ad\nK\3K\3K\3K\3K\3K\5")
+        buf.write("K\u03b4\nK\5K\u03b6\nK\3L\3L\3L\5L\u03bb\nL\3L\3L\3L\3")
+        buf.write("L\3L\5L\u03c2\nL\3M\3M\5M\u03c6\nM\3M\5M\u03c9\nM\3M\3")
+        buf.write("M\5M\u03cd\nM\5M\u03cf\nM\3N\3N\3N\3O\3O\3O\3P\3P\3P\3")
+        buf.write("Q\3Q\3Q\3R\3R\3R\5R\u03e0\nR\3S\3S\3S\3S\3S\5S\u03e7\n")
+        buf.write("S\3S\5S\u03ea\nS\3S\5S\u03ed\nS\3T\3T\3T\3T\3T\5T\u03f4")
+        buf.write("\nT\3T\5T\u03f7\nT\3T\5T\u03fa\nT\3U\3U\3U\3U\3U\5U\u0401")
+        buf.write("\nU\3U\5U\u0404\nU\3U\5U\u0407\nU\3V\3V\3V\5V\u040c\n")
+        buf.write("V\3W\3W\3W\3W\3W\5W\u0413\nW\3W\5W\u0416\nW\3W\5W\u0419")
+        buf.write("\nW\3X\3X\3X\3X\3X\5X\u0420\nX\3X\5X\u0423\nX\3X\5X\u0426")
+        buf.write("\nX\3Y\3Y\3Y\3Y\3Y\5Y\u042d\nY\3Y\5Y\u0430\nY\3Y\5Y\u0433")
+        buf.write("\nY\3Z\3Z\5Z\u0437\nZ\3Z\3Z\3[\3[\3[\3[\3[\3[\3[\3[\3")
+        buf.write("[\3[\5[\u0445\n[\3\\\3\\\3\\\3\\\7\\\u044b\n\\\f\\\16")
+        buf.write("\\\u044e\13\\\5\\\u0450\n\\\3\\\3\\\3]\3]\3]\3]\3^\3^")
+        buf.write("\3^\3_\3_\3_\3_\5_\u045f\n_\3`\3`\3`\3a\5a\u0465\na\3")
+        buf.write("a\3a\5a\u0469\na\3b\5b\u046c\nb\3b\3b\3c\3c\5c\u0472\n")
+        buf.write("c\3c\3c\5c\u0476\nc\3d\3d\5d\u047a\nd\3e\3e\3e\3e\7e\u0480")
+        buf.write("\ne\fe\16e\u0483\13e\5e\u0485\ne\3e\3e\3f\3f\3f\3f\7f")
+        buf.write("\u048d\nf\ff\16f\u0490\13f\5f\u0492\nf\3f\3f\3g\3g\3g")
+        buf.write("\3g\3h\3h\3h\3h\3i\3i\3j\6j\u04a1\nj\rj\16j\u04a2\3j\2")
+        buf.write('\3\u0080k\2\4\6\b\n\f\16\20\22\24\26\30\32\34\36 "$&')
         buf.write("(*,.\60\62\64\668:<>@BDFHJLNPRTVXZ\\^`bdfhjlnprtvxz|~")
         buf.write("\u0080\u0082\u0084\u0086\u0088\u008a\u008c\u008e\u0090")
         buf.write("\u0092\u0094\u0096\u0098\u009a\u009c\u009e\u00a0\u00a2")
         buf.write("\u00a4\u00a6\u00a8\u00aa\u00ac\u00ae\u00b0\u00b2\u00b4")
         buf.write("\u00b6\u00b8\u00ba\u00bc\u00be\u00c0\u00c2\u00c4\u00c6")
         buf.write('\u00c8\u00ca\u00cc\u00ce\u00d0\u00d2\2\13\4\2\33\34"')
         buf.write('"\4\2GHKK\3\29<\3\2>?\3\2_`\3\2ac\3\2\37!\4\2\36\36n')
-        buf.write("n\5\2\16\24\26\26\61\61\2\u0506\2\u00d5\3\2\2\2\4\u00e5")
+        buf.write("n\5\2\16\24\26\26\61\61\2\u0507\2\u00d5\3\2\2\2\4\u00e5")
         buf.write("\3\2\2\2\6\u00eb\3\2\2\2\b\u012d\3\2\2\2\n\u0134\3\2\2")
         buf.write("\2\f\u0139\3\2\2\2\16\u013b\3\2\2\2\20\u016d\3\2\2\2\22")
         buf.write("\u016f\3\2\2\2\24\u0185\3\2\2\2\26\u019d\3\2\2\2\30\u01a0")
         buf.write("\3\2\2\2\32\u01a4\3\2\2\2\34\u01a8\3\2\2\2\36\u01b7\3")
         buf.write('\2\2\2 \u01bb\3\2\2\2"\u01c8\3\2\2\2$\u01cd\3\2\2\2&')
-        buf.write("\u01d0\3\2\2\2(\u01e0\3\2\2\2*\u01e2\3\2\2\2,\u01e7\3")
-        buf.write("\2\2\2.\u01f3\3\2\2\2\60\u0219\3\2\2\2\62\u021b\3\2\2")
-        buf.write("\2\64\u0221\3\2\2\2\66\u022a\3\2\2\28\u022e\3\2\2\2:\u023c")
-        buf.write("\3\2\2\2<\u023e\3\2\2\2>\u0246\3\2\2\2@\u025c\3\2\2\2")
-        buf.write("B\u025e\3\2\2\2D\u0273\3\2\2\2F\u0275\3\2\2\2H\u0281\3")
-        buf.write("\2\2\2J\u0293\3\2\2\2L\u0295\3\2\2\2N\u0299\3\2\2\2P\u02ae")
-        buf.write("\3\2\2\2R\u02b0\3\2\2\2T\u02b4\3\2\2\2V\u02b6\3\2\2\2")
-        buf.write("X\u02b9\3\2\2\2Z\u02c8\3\2\2\2\\\u02ce\3\2\2\2^\u02d0")
-        buf.write("\3\2\2\2`\u02d4\3\2\2\2b\u02de\3\2\2\2d\u02e3\3\2\2\2")
-        buf.write("f\u02ea\3\2\2\2h\u02f0\3\2\2\2j\u02f3\3\2\2\2l\u02f6\3")
-        buf.write("\2\2\2n\u02f9\3\2\2\2p\u0303\3\2\2\2r\u0316\3\2\2\2t\u0320")
-        buf.write("\3\2\2\2v\u0322\3\2\2\2x\u0325\3\2\2\2z\u032d\3\2\2\2")
-        buf.write("|\u0338\3\2\2\2~\u033a\3\2\2\2\u0080\u0342\3\2\2\2\u0082")
-        buf.write("\u0362\3\2\2\2\u0084\u037a\3\2\2\2\u0086\u0380\3\2\2\2")
-        buf.write("\u0088\u0382\3\2\2\2\u008a\u0385\3\2\2\2\u008c\u038e\3")
-        buf.write("\2\2\2\u008e\u0390\3\2\2\2\u0090\u0392\3\2\2\2\u0092\u03a5")
-        buf.write("\3\2\2\2\u0094\u03b4\3\2\2\2\u0096\u03b9\3\2\2\2\u0098")
-        buf.write("\u03cd\3\2\2\2\u009a\u03cf\3\2\2\2\u009c\u03d2\3\2\2\2")
-        buf.write("\u009e\u03d5\3\2\2\2\u00a0\u03d8\3\2\2\2\u00a2\u03de\3")
-        buf.write("\2\2\2\u00a4\u03eb\3\2\2\2\u00a6\u03f8\3\2\2\2\u00a8\u0405")
-        buf.write("\3\2\2\2\u00aa\u040a\3\2\2\2\u00ac\u0417\3\2\2\2\u00ae")
-        buf.write("\u0424\3\2\2\2\u00b0\u0431\3\2\2\2\u00b2\u0433\3\2\2\2")
-        buf.write("\u00b4\u0443\3\2\2\2\u00b6\u0445\3\2\2\2\u00b8\u0452\3")
-        buf.write("\2\2\2\u00ba\u0456\3\2\2\2\u00bc\u045d\3\2\2\2\u00be\u045f")
-        buf.write("\3\2\2\2\u00c0\u0463\3\2\2\2\u00c2\u046a\3\2\2\2\u00c4")
-        buf.write("\u046e\3\2\2\2\u00c6\u0476\3\2\2\2\u00c8\u047a\3\2\2\2")
-        buf.write("\u00ca\u0487\3\2\2\2\u00cc\u0494\3\2\2\2\u00ce\u0498\3")
-        buf.write("\2\2\2\u00d0\u049c\3\2\2\2\u00d2\u049f\3\2\2\2\u00d4\u00d6")
+        buf.write("\u01de\3\2\2\2(\u01e0\3\2\2\2*\u01e5\3\2\2\2,\u01f1\3")
+        buf.write("\2\2\2.\u0217\3\2\2\2\60\u0219\3\2\2\2\62\u021f\3\2\2")
+        buf.write("\2\64\u0228\3\2\2\2\66\u022c\3\2\2\28\u023a\3\2\2\2:\u023c")
+        buf.write("\3\2\2\2<\u0244\3\2\2\2>\u025a\3\2\2\2@\u025c\3\2\2\2")
+        buf.write("B\u0271\3\2\2\2D\u0273\3\2\2\2F\u027f\3\2\2\2H\u0291\3")
+        buf.write("\2\2\2J\u0293\3\2\2\2L\u0297\3\2\2\2N\u02ac\3\2\2\2P\u02ae")
+        buf.write("\3\2\2\2R\u02b2\3\2\2\2T\u02b4\3\2\2\2V\u02b7\3\2\2\2")
+        buf.write("X\u02c6\3\2\2\2Z\u02cc\3\2\2\2\\\u02ce\3\2\2\2^\u02d2")
+        buf.write("\3\2\2\2`\u02dc\3\2\2\2b\u02e1\3\2\2\2d\u02e8\3\2\2\2")
+        buf.write("f\u02ee\3\2\2\2h\u02f1\3\2\2\2j\u02f4\3\2\2\2l\u02f7\3")
+        buf.write("\2\2\2n\u0301\3\2\2\2p\u0314\3\2\2\2r\u031e\3\2\2\2t\u0320")
+        buf.write("\3\2\2\2v\u0323\3\2\2\2x\u032b\3\2\2\2z\u0336\3\2\2\2")
+        buf.write("|\u0338\3\2\2\2~\u0340\3\2\2\2\u0080\u0360\3\2\2\2\u0082")
+        buf.write("\u036f\3\2\2\2\u0084\u037b\3\2\2\2\u0086\u0381\3\2\2\2")
+        buf.write("\u0088\u0383\3\2\2\2\u008a\u0386\3\2\2\2\u008c\u038f\3")
+        buf.write("\2\2\2\u008e\u0391\3\2\2\2\u0090\u0393\3\2\2\2\u0092\u03a6")
+        buf.write("\3\2\2\2\u0094\u03b5\3\2\2\2\u0096\u03ba\3\2\2\2\u0098")
+        buf.write("\u03ce\3\2\2\2\u009a\u03d0\3\2\2\2\u009c\u03d3\3\2\2\2")
+        buf.write("\u009e\u03d6\3\2\2\2\u00a0\u03d9\3\2\2\2\u00a2\u03df\3")
+        buf.write("\2\2\2\u00a4\u03ec\3\2\2\2\u00a6\u03f9\3\2\2\2\u00a8\u0406")
+        buf.write("\3\2\2\2\u00aa\u040b\3\2\2\2\u00ac\u0418\3\2\2\2\u00ae")
+        buf.write("\u0425\3\2\2\2\u00b0\u0432\3\2\2\2\u00b2\u0434\3\2\2\2")
+        buf.write("\u00b4\u0444\3\2\2\2\u00b6\u0446\3\2\2\2\u00b8\u0453\3")
+        buf.write("\2\2\2\u00ba\u0457\3\2\2\2\u00bc\u045e\3\2\2\2\u00be\u0460")
+        buf.write("\3\2\2\2\u00c0\u0464\3\2\2\2\u00c2\u046b\3\2\2\2\u00c4")
+        buf.write("\u046f\3\2\2\2\u00c6\u0477\3\2\2\2\u00c8\u047b\3\2\2\2")
+        buf.write("\u00ca\u0488\3\2\2\2\u00cc\u0495\3\2\2\2\u00ce\u0499\3")
+        buf.write("\2\2\2\u00d0\u049d\3\2\2\2\u00d2\u04a0\3\2\2\2\u00d4\u00d6")
         buf.write("\5\4\3\2\u00d5\u00d4\3\2\2\2\u00d5\u00d6\3\2\2\2\u00d6")
         buf.write("\u00da\3\2\2\2\u00d7\u00d9\5\6\4\2\u00d8\u00d7\3\2\2\2")
         buf.write("\u00d9\u00dc\3\2\2\2\u00da\u00d8\3\2\2\2\u00da\u00db\3")
         buf.write("\2\2\2\u00db\u00e0\3\2\2\2\u00dc\u00da\3\2\2\2\u00dd\u00df")
         buf.write("\5\f\7\2\u00de\u00dd\3\2\2\2\u00df\u00e2\3\2\2\2\u00e0")
         buf.write("\u00de\3\2\2\2\u00e0\u00e1\3\2\2\2\u00e1\u00e3\3\2\2\2")
         buf.write("\u00e2\u00e0\3\2\2\2\u00e3\u00e4\7\2\2\3\u00e4\3\3\2\2")
@@ -192,22 +193,22 @@
         buf.write("\2\2\2\u0124\u0127\7-\2\2\u0125\u0128\7a\2\2\u0126\u0128")
         buf.write("\5\n\6\2\u0127\u0125\3\2\2\2\u0127\u0126\3\2\2\2\u0128")
         buf.write("\u012b\3\2\2\2\u0129\u012a\7]\2\2\u012a\u012c\5\b\5\2")
         buf.write("\u012b\u0129\3\2\2\2\u012b\u012c\3\2\2\2\u012c\u012e\3")
         buf.write("\2\2\2\u012d\u00f6\3\2\2\2\u012d\u00ff\3\2\2\2\u012d\u0108")
         buf.write("\3\2\2\2\u012d\u0111\3\2\2\2\u012d\u011a\3\2\2\2\u012d")
         buf.write("\u0124\3\2\2\2\u012e\t\3\2\2\2\u012f\u0135\7n\2\2\u0130")
-        buf.write("\u0131\7/\2\2\u0131\u0132\58\35\2\u0132\u0133\7\60\2\2")
-        buf.write("\u0133\u0135\3\2\2\2\u0134\u012f\3\2\2\2\u0134\u0130\3")
-        buf.write("\2\2\2\u0135\13\3\2\2\2\u0136\u013a\5\16\b\2\u0137\u013a")
+        buf.write("\u0131\7/\2\2\u0131\u0132\5\66\34\2\u0132\u0133\7\60\2")
+        buf.write("\2\u0133\u0135\3\2\2\2\u0134\u012f\3\2\2\2\u0134\u0130")
+        buf.write("\3\2\2\2\u0135\13\3\2\2\2\u0136\u013a\5\16\b\2\u0137\u013a")
         buf.write("\5\20\t\2\u0138\u013a\5\24\13\2\u0139\u0136\3\2\2\2\u0139")
         buf.write("\u0137\3\2\2\2\u0139\u0138\3\2\2\2\u013a\r\3\2\2\2\u013b")
         buf.write("\u013c\7[\2\2\u013c\u013d\7n\2\2\u013d\u013e\78\2\2\u013e")
-        buf.write("\u0145\5f\64\2\u013f\u0140\7]\2\2\u0140\u0141\7n\2\2\u0141")
-        buf.write("\u0142\78\2\2\u0142\u0144\5f\64\2\u0143\u013f\3\2\2\2")
+        buf.write("\u0145\5d\63\2\u013f\u0140\7]\2\2\u0140\u0141\7n\2\2\u0141")
+        buf.write("\u0142\78\2\2\u0142\u0144\5d\63\2\u0143\u013f\3\2\2\2")
         buf.write("\u0144\u0147\3\2\2\2\u0145\u0143\3\2\2\2\u0145\u0146\3")
         buf.write("\2\2\2\u0146\u0148\3\2\2\2\u0147\u0145\3\2\2\2\u0148\u0149")
         buf.write("\7\67\2\2\u0149\17\3\2\2\2\u014a\u014b\7\26\2\2\u014b")
         buf.write("\u0150\7n\2\2\u014c\u014d\7$\2\2\u014d\u014f\7n\2\2\u014e")
         buf.write("\u014c\3\2\2\2\u014f\u0152\3\2\2\2\u0150\u014e\3\2\2\2")
         buf.write("\u0150\u0151\3\2\2\2\u0151\u0153\3\2\2\2\u0152\u0150\3")
         buf.write("\2\2\2\u0153\u016e\5\36\20\2\u0154\u0155\7\61\2\2\u0155")
@@ -223,383 +224,385 @@
         buf.write("\3\2\2\2\u016b\u016c\3\2\2\2\u016c\u016e\5\22\n\2\u016d")
         buf.write("\u014a\3\2\2\2\u016d\u0154\3\2\2\2\u016d\u015e\3\2\2\2")
         buf.write("\u016d\u0161\3\2\2\2\u016d\u0165\3\2\2\2\u016e\21\3\2")
         buf.write("\2\2\u016f\u0173\7/\2\2\u0170\u0172\5 \21\2\u0171\u0170")
         buf.write("\3\2\2\2\u0172\u0175\3\2\2\2\u0173\u0171\3\2\2\2\u0173")
         buf.write("\u0174\3\2\2\2\u0174\u0177\3\2\2\2\u0175\u0173\3\2\2\2")
         buf.write("\u0176\u0178\5\30\r\2\u0177\u0176\3\2\2\2\u0177\u0178")
-        buf.write("\3\2\2\2\u0178\u017d\3\2\2\2\u0179\u017c\5D#\2\u017a\u017c")
-        buf.write("\5\34\17\2\u017b\u0179\3\2\2\2\u017b\u017a\3\2\2\2\u017c")
-        buf.write("\u017f\3\2\2\2\u017d\u017b\3\2\2\2\u017d\u017e\3\2\2\2")
-        buf.write("\u017e\u0181\3\2\2\2\u017f\u017d\3\2\2\2\u0180\u0182\5")
-        buf.write("\32\16\2\u0181\u0180\3\2\2\2\u0181\u0182\3\2\2\2\u0182")
-        buf.write("\u0183\3\2\2\2\u0183\u0184\7\60\2\2\u0184\23\3\2\2\2\u0185")
-        buf.write("\u0187\7\65\2\2\u0186\u0188\7n\2\2\u0187\u0186\3\2\2\2")
-        buf.write("\u0187\u0188\3\2\2\2\u0188\u0189\3\2\2\2\u0189\u018a\5")
-        buf.write("\u00d2j\2\u018a\u018e\7\32\2\2\u018b\u018f\5\u009eP\2")
-        buf.write("\u018c\u018d\7\25\2\2\u018d\u018f\5&\24\2\u018e\u018b")
+        buf.write('\3\2\2\2\u0178\u017d\3\2\2\2\u0179\u017c\5B"\2\u017a')
+        buf.write("\u017c\5\34\17\2\u017b\u0179\3\2\2\2\u017b\u017a\3\2\2")
+        buf.write("\2\u017c\u017f\3\2\2\2\u017d\u017b\3\2\2\2\u017d\u017e")
+        buf.write("\3\2\2\2\u017e\u0181\3\2\2\2\u017f\u017d\3\2\2\2\u0180")
+        buf.write("\u0182\5\32\16\2\u0181\u0180\3\2\2\2\u0181\u0182\3\2\2")
+        buf.write("\2\u0182\u0183\3\2\2\2\u0183\u0184\7\60\2\2\u0184\23\3")
+        buf.write("\2\2\2\u0185\u0187\7\65\2\2\u0186\u0188\7n\2\2\u0187\u0186")
+        buf.write("\3\2\2\2\u0187\u0188\3\2\2\2\u0188\u0189\3\2\2\2\u0189")
+        buf.write("\u018a\5\u00d2j\2\u018a\u018e\7\32\2\2\u018b\u018f\5\u009e")
+        buf.write("P\2\u018c\u018d\7\25\2\2\u018d\u018f\5&\24\2\u018e\u018b")
         buf.write("\3\2\2\2\u018e\u018c\3\2\2\2\u018f\u0190\3\2\2\2\u0190")
         buf.write("\u019b\7E\2\2\u0191\u0193\5\u009cO\2\u0192\u0194\5\u00c8")
         buf.write("e\2\u0193\u0192\3\2\2\2\u0193\u0194\3\2\2\2\u0194\u0197")
-        buf.write("\3\2\2\2\u0195\u0198\5@!\2\u0196\u0198\7\67\2\2\u0197")
+        buf.write("\3\2\2\2\u0195\u0198\5> \2\u0196\u0198\7\67\2\2\u0197")
         buf.write("\u0195\3\2\2\2\u0197\u0196\3\2\2\2\u0198\u019c\3\2\2\2")
         buf.write("\u0199\u019a\7\62\2\2\u019a\u019c\5\22\n\2\u019b\u0191")
         buf.write("\3\2\2\2\u019b\u0199\3\2\2\2\u019c\25\3\2\2\2\u019d\u019e")
-        buf.write("\7$\2\2\u019e\u019f\58\35\2\u019f\27\3\2\2\2\u01a0\u01a1")
-        buf.write("\7\32\2\2\u01a1\u01a2\7\33\2\2\u01a2\u01a3\5@!\2\u01a3")
+        buf.write("\7$\2\2\u019e\u019f\5\66\34\2\u019f\27\3\2\2\2\u01a0\u01a1")
+        buf.write("\7\32\2\2\u01a1\u01a2\7\33\2\2\u01a2\u01a3\5> \2\u01a3")
         buf.write("\31\3\2\2\2\u01a4\u01a5\7\32\2\2\u01a5\u01a6\7\34\2\2")
-        buf.write("\u01a6\u01a7\5@!\2\u01a7\33\3\2\2\2\u01a8\u01a9\7\32\2")
-        buf.write('\2\u01a9\u01aa\7"\2\2\u01aa\u01ab\5@!\2\u01ab\35\3\2')
+        buf.write("\u01a6\u01a7\5> \2\u01a7\33\3\2\2\2\u01a8\u01a9\7\32\2")
+        buf.write('\2\u01a9\u01aa\7"\2\2\u01aa\u01ab\5> \2\u01ab\35\3\2')
         buf.write("\2\2\u01ac\u01b0\7/\2\2\u01ad\u01af\5 \21\2\u01ae\u01ad")
         buf.write("\3\2\2\2\u01af\u01b2\3\2\2\2\u01b0\u01ae\3\2\2\2\u01b0")
         buf.write("\u01b1\3\2\2\2\u01b1\u01b3\3\2\2\2\u01b2\u01b0\3\2\2\2")
         buf.write("\u01b3\u01b8\7\60\2\2\u01b4\u01b5\7$\2\2\u01b5\u01b8\5")
         buf.write(" \21\2\u01b6\u01b8\7\67\2\2\u01b7\u01ac\3\2\2\2\u01b7")
         buf.write("\u01b4\3\2\2\2\u01b7\u01b6\3\2\2\2\u01b8\37\3\2\2\2\u01b9")
-        buf.write("\u01bc\5,\27\2\u01ba\u01bc\5\60\31\2\u01bb\u01b9\3\2\2")
-        buf.write("\2\u01bb\u01ba\3\2\2\2\u01bc!\3\2\2\2\u01bd\u01c1\7/\2")
-        buf.write("\2\u01be\u01c0\5,\27\2\u01bf\u01be\3\2\2\2\u01c0\u01c3")
-        buf.write("\3\2\2\2\u01c1\u01bf\3\2\2\2\u01c1\u01c2\3\2\2\2\u01c2")
-        buf.write("\u01c4\3\2\2\2\u01c3\u01c1\3\2\2\2\u01c4\u01c9\7\60\2")
-        buf.write("\2\u01c5\u01c6\7$\2\2\u01c6\u01c9\5,\27\2\u01c7\u01c9")
-        buf.write("\7\67\2\2\u01c8\u01bd\3\2\2\2\u01c8\u01c5\3\2\2\2\u01c8")
-        buf.write("\u01c7\3\2\2\2\u01c9#\3\2\2\2\u01ca\u01cc\5\60\31\2\u01cb")
-        buf.write("\u01ca\3\2\2\2\u01cc\u01cf\3\2\2\2\u01cd\u01cb\3\2\2\2")
-        buf.write("\u01cd\u01ce\3\2\2\2\u01ce%\3\2\2\2\u01cf\u01cd\3\2\2")
-        buf.write("\2\u01d0\u01d1\5(\25\2\u01d1'\3\2\2\2\u01d2\u01d3\7/")
-        buf.write("\2\2\u01d3\u01d4\5*\26\2\u01d4\u01d5\5$\23\2\u01d5\u01d6")
-        buf.write("\7\31\2\2\u01d6\u01d7\5@!\2\u01d7\u01d8\7\60\2\2\u01d8")
-        buf.write("\u01e1\3\2\2\2\u01d9\u01da\7$\2\2\u01da\u01db\5*\26\2")
-        buf.write("\u01db\u01dc\5$\23\2\u01dc\u01dd\7\31\2\2\u01dd\u01de")
-        buf.write("\5@!\2\u01de\u01df\7\67\2\2\u01df\u01e1\3\2\2\2\u01e0")
-        buf.write("\u01d2\3\2\2\2\u01e0\u01d9\3\2\2\2\u01e1)\3\2\2\2\u01e2")
-        buf.write("\u01e3\7Z\2\2\u01e3\u01e4\7Y\2\2\u01e4\u01e5\7n\2\2\u01e5")
-        buf.write("\u01e6\7\67\2\2\u01e6+\3\2\2\2\u01e7\u01e8\7Z\2\2\u01e8")
-        buf.write("\u01ed\5.\30\2\u01e9\u01ea\7]\2\2\u01ea\u01ec\5.\30\2")
-        buf.write("\u01eb\u01e9\3\2\2\2\u01ec\u01ef\3\2\2\2\u01ed\u01eb\3")
-        buf.write("\2\2\2\u01ed\u01ee\3\2\2\2\u01ee\u01f0\3\2\2\2\u01ef\u01ed")
-        buf.write("\3\2\2\2\u01f0\u01f1\7\67\2\2\u01f1-\3\2\2\2\u01f2\u01f4")
-        buf.write("\7\\\2\2\u01f3\u01f2\3\2\2\2\u01f3\u01f4\3\2\2\2\u01f4")
-        buf.write("\u01f6\3\2\2\2\u01f5\u01f7\7Y\2\2\u01f6\u01f5\3\2\2\2")
-        buf.write("\u01f6\u01f7\3\2\2\2\u01f7\u01fc\3\2\2\2\u01f8\u01fd\7")
-        buf.write("n\2\2\u01f9\u01fa\7n\2\2\u01fa\u01fb\78\2\2\u01fb\u01fd")
-        buf.write("\5f\64\2\u01fc\u01f8\3\2\2\2\u01fc\u01f9\3\2\2\2\u01fd")
-        buf.write("/\3\2\2\2\u01fe\u01ff\7^\2\2\u01ff\u0203\5\66\34\2\u0200")
-        buf.write("\u0201\5\64\33\2\u0201\u0202\5\62\32\2\u0202\u0204\3\2")
-        buf.write("\2\2\u0203\u0200\3\2\2\2\u0203\u0204\3\2\2\2\u0204\u020e")
-        buf.write("\3\2\2\2\u0205\u0206\7]\2\2\u0206\u020a\5\66\34\2\u0207")
-        buf.write("\u0208\5\64\33\2\u0208\u0209\5\62\32\2\u0209\u020b\3\2")
-        buf.write("\2\2\u020a\u0207\3\2\2\2\u020a\u020b\3\2\2\2\u020b\u020d")
-        buf.write("\3\2\2\2\u020c\u0205\3\2\2\2\u020d\u0210\3\2\2\2\u020e")
-        buf.write("\u020c\3\2\2\2\u020e\u020f\3\2\2\2\u020f\u0211\3\2\2\2")
-        buf.write("\u0210\u020e\3\2\2\2\u0211\u0212\7\67\2\2\u0212\u021a")
-        buf.write("\3\2\2\2\u0213\u0214\7^\2\2\u0214\u0216\7n\2\2\u0215\u0217")
-        buf.write("\5\62\32\2\u0216\u0215\3\2\2\2\u0216\u0217\3\2\2\2\u0217")
-        buf.write("\u0218\3\2\2\2\u0218\u021a\5@!\2\u0219\u01fe\3\2\2\2\u0219")
-        buf.write("\u0213\3\2\2\2\u021a\61\3\2\2\2\u021b\u021d\7\32\2\2\u021c")
-        buf.write("\u021e\58\35\2\u021d\u021c\3\2\2\2\u021d\u021e\3\2\2\2")
-        buf.write("\u021e\u021f\3\2\2\2\u021f\u0220\t\2\2\2\u0220\63\3\2")
-        buf.write("\2\2\u0221\u0223\7%\2\2\u0222\u0224\5:\36\2\u0223\u0222")
-        buf.write("\3\2\2\2\u0223\u0224\3\2\2\2\u0224\u0228\3\2\2\2\u0225")
-        buf.write("\u0229\7%\2\2\u0226\u0227\7.\2\2\u0227\u0229\5f\64\2\u0228")
-        buf.write("\u0225\3\2\2\2\u0228\u0226\3\2\2\2\u0229\65\3\2\2\2\u022a")
-        buf.write("\u022b\7n\2\2\u022b\u022c\7P\2\2\u022c\u022d\7n\2\2\u022d")
-        buf.write("\67\3\2\2\2\u022e\u0233\7n\2\2\u022f\u0230\7]\2\2\u0230")
-        buf.write("\u0232\7n\2\2\u0231\u022f\3\2\2\2\u0232\u0235\3\2\2\2")
-        buf.write("\u0233\u0231\3\2\2\2\u0233\u0234\3\2\2\2\u02349\3\2\2")
-        buf.write("\2\u0235\u0233\3\2\2\2\u0236\u023d\5<\37\2\u0237\u023d")
-        buf.write("\5> \2\u0238\u0239\5<\37\2\u0239\u023a\7]\2\2\u023a\u023b")
-        buf.write("\5> \2\u023b\u023d\3\2\2\2\u023c\u0236\3\2\2\2\u023c\u0237")
-        buf.write("\3\2\2\2\u023c\u0238\3\2\2\2\u023d;\3\2\2\2\u023e\u0243")
-        buf.write("\5n8\2\u023f\u0240\7]\2\2\u0240\u0242\5n8\2\u0241\u023f")
-        buf.write("\3\2\2\2\u0242\u0245\3\2\2\2\u0243\u0241\3\2\2\2\u0243")
-        buf.write("\u0244\3\2\2\2\u0244=\3\2\2\2\u0245\u0243\3\2\2\2\u0246")
-        buf.write("\u0247\7n\2\2\u0247\u0248\78\2\2\u0248\u024f\5n8\2\u0249")
-        buf.write("\u024a\7]\2\2\u024a\u024b\7n\2\2\u024b\u024c\78\2\2\u024c")
-        buf.write("\u024e\5n8\2\u024d\u0249\3\2\2\2\u024e\u0251\3\2\2\2\u024f")
-        buf.write("\u024d\3\2\2\2\u024f\u0250\3\2\2\2\u0250?\3\2\2\2\u0251")
-        buf.write("\u024f\3\2\2\2\u0252\u0256\7/\2\2\u0253\u0255\5D#\2\u0254")
-        buf.write("\u0253\3\2\2\2\u0255\u0258\3\2\2\2\u0256\u0254\3\2\2\2")
-        buf.write("\u0256\u0257\3\2\2\2\u0257\u0259\3\2\2\2\u0258\u0256\3")
-        buf.write("\2\2\2\u0259\u025d\7\60\2\2\u025a\u025b\7$\2\2\u025b\u025d")
-        buf.write("\5D#\2\u025c\u0252\3\2\2\2\u025c\u025a\3\2\2\2\u025dA")
-        buf.write("\3\2\2\2\u025e\u025f\58\35\2\u025f\u0260\5@!\2\u0260C")
-        buf.write('\3\2\2\2\u0261\u0274\5@!\2\u0262\u0274\5B"\2\u0263\u0264')
-        buf.write("\5f\64\2\u0264\u0265\7\67\2\2\u0265\u0274\3\2\2\2\u0266")
-        buf.write("\u0274\5F$\2\u0267\u0274\5H%\2\u0268\u0274\5P)\2\u0269")
-        buf.write("\u0274\5R*\2\u026a\u026b\5V,\2\u026b\u026c\7\67\2\2\u026c")
-        buf.write("\u0274\3\2\2\2\u026d\u026e\5T+\2\u026e\u026f\7\67\2\2")
-        buf.write("\u026f\u0274\3\2\2\2\u0270\u0274\5X-\2\u0271\u0274\5Z")
-        buf.write(".\2\u0272\u0274\5\\/\2\u0273\u0261\3\2\2\2\u0273\u0262")
-        buf.write("\3\2\2\2\u0273\u0263\3\2\2\2\u0273\u0266\3\2\2\2\u0273")
-        buf.write("\u0267\3\2\2\2\u0273\u0268\3\2\2\2\u0273\u0269\3\2\2\2")
-        buf.write("\u0273\u026a\3\2\2\2\u0273\u026d\3\2\2\2\u0273\u0270\3")
-        buf.write("\2\2\2\u0273\u0271\3\2\2\2\u0273\u0272\3\2\2\2\u0274E")
-        buf.write("\3\2\2\2\u0275\u0276\7@\2\2\u0276\u0277\5f\64\2\u0277")
-        buf.write("\u027b\5@!\2\u0278\u027a\5L'\2\u0279\u0278\3\2\2\2\u027a")
-        buf.write("\u027d\3\2\2\2\u027b\u0279\3\2\2\2\u027b\u027c\3\2\2\2")
-        buf.write("\u027c\u027f\3\2\2\2\u027d\u027b\3\2\2\2\u027e\u0280\5")
-        buf.write("N(\2\u027f\u027e\3\2\2\2\u027f\u0280\3\2\2\2\u0280G\3")
-        buf.write("\2\2\2\u0281\u0282\7N\2\2\u0282\u0284\5@!\2\u0283\u0285")
-        buf.write("\5J&\2\u0284\u0283\3\2\2\2\u0284\u0285\3\2\2\2\u0285I")
-        buf.write("\3\2\2\2\u0286\u028a\7B\2\2\u0287\u0288\7e\2\2\u0288\u0289")
-        buf.write("\7n\2\2\u0289\u028b\7f\2\2\u028a\u0287\3\2\2\2\u028a\u028b")
-        buf.write("\3\2\2\2\u028b\u028c\3\2\2\2\u028c\u0294\5@!\2\u028d\u0290")
-        buf.write("\7B\2\2\u028e\u028f\7\32\2\2\u028f\u0291\7n\2\2\u0290")
-        buf.write("\u028e\3\2\2\2\u0290\u0291\3\2\2\2\u0291\u0292\3\2\2\2")
-        buf.write("\u0292\u0294\5@!\2\u0293\u0286\3\2\2\2\u0293\u028d\3\2")
-        buf.write("\2\2\u0294K\3\2\2\2\u0295\u0296\7A\2\2\u0296\u0297\5f")
-        buf.write("\64\2\u0297\u0298\5@!\2\u0298M\3\2\2\2\u0299\u029a\7B")
-        buf.write("\2\2\u029a\u029b\5@!\2\u029bO\3\2\2\2\u029c\u029d\7C\2")
-        buf.write("\2\u029d\u029e\5f\64\2\u029e\u029f\7D\2\2\u029f\u02a0")
-        buf.write("\5f\64\2\u02a0\u02a1\7E\2\2\u02a1\u02a2\5f\64\2\u02a2")
-        buf.write("\u02a3\5@!\2\u02a3\u02af\3\2\2\2\u02a4\u02a5\7C\2\2\u02a5")
-        buf.write("\u02a8\7n\2\2\u02a6\u02a7\7]\2\2\u02a7\u02a9\7n\2\2\u02a8")
-        buf.write("\u02a6\3\2\2\2\u02a8\u02a9\3\2\2\2\u02a9\u02aa\3\2\2\2")
-        buf.write("\u02aa\u02ab\7X\2\2\u02ab\u02ac\5f\64\2\u02ac\u02ad\5")
-        buf.write("@!\2\u02ad\u02af\3\2\2\2\u02ae\u029c\3\2\2\2\u02ae\u02a4")
-        buf.write("\3\2\2\2\u02afQ\3\2\2\2\u02b0\u02b1\7F\2\2\u02b1\u02b2")
-        buf.write("\5f\64\2\u02b2\u02b3\5@!\2\u02b3S\3\2\2\2\u02b4\u02b5")
-        buf.write("\t\3\2\2\u02b5U\3\2\2\2\u02b6\u02b7\7\66\2\2\u02b7\u02b8")
-        buf.write("\5f\64\2\u02b8W\3\2\2\2\u02b9\u02ba\7M\2\2\u02ba\u02bb")
-        buf.write("\5f\64\2\u02bb\u02bc\7\67\2\2\u02bcY\3\2\2\2\u02bd\u02be")
-        buf.write("\7L\2\2\u02be\u02bf\5f\64\2\u02bf\u02c0\7\67\2\2\u02c0")
-        buf.write("\u02c9\3\2\2\2\u02c1\u02c2\7L\2\2\u02c2\u02c3\7$\2\2\u02c3")
-        buf.write("\u02c4\7n\2\2\u02c4\u02c5\78\2\2\u02c5\u02c6\5f\64\2\u02c6")
-        buf.write("\u02c7\7\67\2\2\u02c7\u02c9\3\2\2\2\u02c8\u02bd\3\2\2")
-        buf.write("\2\u02c8\u02c1\3\2\2\2\u02c9[\3\2\2\2\u02ca\u02cf\5^\60")
-        buf.write("\2\u02cb\u02cf\5`\61\2\u02cc\u02cf\5b\62\2\u02cd\u02cf")
-        buf.write("\5d\63\2\u02ce\u02ca\3\2\2\2\u02ce\u02cb\3\2\2\2\u02ce")
-        buf.write("\u02cc\3\2\2\2\u02ce\u02cd\3\2\2\2\u02cf]\3\2\2\2\u02d0")
-        buf.write("\u02d1\7\27\2\2\u02d1\u02d2\5f\64\2\u02d2\u02d3\7\67\2")
-        buf.write("\2\u02d3_\3\2\2\2\u02d4\u02d7\7\30\2\2\u02d5\u02d6\7$")
-        buf.write("\2\2\u02d6\u02d8\7n\2\2\u02d7\u02d5\3\2\2\2\u02d7\u02d8")
-        buf.write("\3\2\2\2\u02d8\u02d9\3\2\2\2\u02d9\u02dc\5f\64\2\u02da")
-        buf.write("\u02dd\7\67\2\2\u02db\u02dd\5N(\2\u02dc\u02da\3\2\2\2")
-        buf.write("\u02dc\u02db\3\2\2\2\u02dda\3\2\2\2\u02de\u02e1\7I\2\2")
-        buf.write("\u02df\u02e2\5Z.\2\u02e0\u02e2\7\67\2\2\u02e1\u02df\3")
-        buf.write("\2\2\2\u02e1\u02e0\3\2\2\2\u02e2c\3\2\2\2\u02e3\u02e8")
-        buf.write("\7J\2\2\u02e4\u02e9\5Z.\2\u02e5\u02e9\5b\62\2\u02e6\u02e9")
-        buf.write("\5`\61\2\u02e7\u02e9\7\67\2\2\u02e8\u02e4\3\2\2\2\u02e8")
-        buf.write("\u02e5\3\2\2\2\u02e8\u02e6\3\2\2\2\u02e8\u02e7\3\2\2\2")
-        buf.write("\u02e9e\3\2\2\2\u02ea\u02ee\5n8\2\u02eb\u02ef\5h\65\2")
-        buf.write("\u02ec\u02ef\5j\66\2\u02ed\u02ef\5l\67\2\u02ee\u02eb\3")
-        buf.write("\2\2\2\u02ee\u02ec\3\2\2\2\u02ee\u02ed\3\2\2\2\u02ee\u02ef")
-        buf.write("\3\2\2\2\u02efg\3\2\2\2\u02f0\u02f1\78\2\2\u02f1\u02f2")
-        buf.write("\5f\64\2\u02f2i\3\2\2\2\u02f3\u02f4\7=\2\2\u02f4\u02f5")
-        buf.write("\5f\64\2\u02f5k\3\2\2\2\u02f6\u02f7\t\4\2\2\u02f7\u02f8")
-        buf.write("\5f\64\2\u02f8m\3\2\2\2\u02f9\u0301\5p9\2\u02fa\u02fb")
-        buf.write("\7Q\2\2\u02fb\u02fe\5\u00a2R\2\u02fc\u02fe\5\u00aaV\2")
-        buf.write("\u02fd\u02fa\3\2\2\2\u02fd\u02fc\3\2\2\2\u02fe\u02ff\3")
-        buf.write("\2\2\2\u02ff\u0300\5f\64\2\u0300\u0302\3\2\2\2\u0301\u02fd")
-        buf.write("\3\2\2\2\u0301\u0302\3\2\2\2\u0302o\3\2\2\2\u0303\u0308")
-        buf.write("\5r:\2\u0304\u0305\t\5\2\2\u0305\u0307\5r:\2\u0306\u0304")
-        buf.write("\3\2\2\2\u0307\u030a\3\2\2\2\u0308\u0306\3\2\2\2\u0308")
-        buf.write("\u0309\3\2\2\2\u0309q\3\2\2\2\u030a\u0308\3\2\2\2\u030b")
-        buf.write("\u030c\7Q\2\2\u030c\u0317\5r:\2\u030d\u0313\5x=\2\u030e")
-        buf.write("\u030f\5t;\2\u030f\u0310\5x=\2\u0310\u0312\3\2\2\2\u0311")
-        buf.write("\u030e\3\2\2\2\u0312\u0315\3\2\2\2\u0313\u0311\3\2\2\2")
-        buf.write("\u0313\u0314\3\2\2\2\u0314\u0317\3\2\2\2\u0315\u0313\3")
-        buf.write("\2\2\2\u0316\u030b\3\2\2\2\u0316\u030d\3\2\2\2\u0317s")
-        buf.write("\3\2\2\2\u0318\u0321\7R\2\2\u0319\u0321\7S\2\2\u031a\u0321")
-        buf.write("\7T\2\2\u031b\u0321\7U\2\2\u031c\u0321\7V\2\2\u031d\u0321")
-        buf.write("\7W\2\2\u031e\u0321\7X\2\2\u031f\u0321\5v<\2\u0320\u0318")
-        buf.write("\3\2\2\2\u0320\u0319\3\2\2\2\u0320\u031a\3\2\2\2\u0320")
-        buf.write("\u031b\3\2\2\2\u0320\u031c\3\2\2\2\u0320\u031d\3\2\2\2")
-        buf.write("\u0320\u031e\3\2\2\2\u0320\u031f\3\2\2\2\u0321u\3\2\2")
-        buf.write("\2\u0322\u0323\7Q\2\2\u0323\u0324\7X\2\2\u0324w\3\2\2")
-        buf.write("\2\u0325\u032a\5z>\2\u0326\u0327\t\6\2\2\u0327\u0329\5")
-        buf.write("z>\2\u0328\u0326\3\2\2\2\u0329\u032c\3\2\2\2\u032a\u0328")
-        buf.write("\3\2\2\2\u032a\u032b\3\2\2\2\u032by\3\2\2\2\u032c\u032a")
-        buf.write("\3\2\2\2\u032d\u0332\5|?\2\u032e\u032f\t\7\2\2\u032f\u0331")
-        buf.write("\5|?\2\u0330\u032e\3\2\2\2\u0331\u0334\3\2\2\2\u0332\u0330")
-        buf.write("\3\2\2\2\u0332\u0333\3\2\2\2\u0333{\3\2\2\2\u0334\u0332")
-        buf.write("\3\2\2\2\u0335\u0336\t\6\2\2\u0336\u0339\5|?\2\u0337\u0339")
-        buf.write("\5~@\2\u0338\u0335\3\2\2\2\u0338\u0337\3\2\2\2\u0339}")
-        buf.write("\3\2\2\2\u033a\u033f\5\u0082B\2\u033b\u033c\7d\2\2\u033c")
-        buf.write("\u033e\5|?\2\u033d\u033b\3\2\2\2\u033e\u0341\3\2\2\2\u033f")
-        buf.write("\u033d\3\2\2\2\u033f\u0340\3\2\2\2\u0340\177\3\2\2\2\u0341")
-        buf.write("\u033f\3\2\2\2\u0342\u0343\7[\2\2\u0343\u0346\7P\2\2\u0344")
-        buf.write("\u0347\5\u0090I\2\u0345\u0347\7n\2\2\u0346\u0344\3\2\2")
-        buf.write("\2\u0346\u0345\3\2\2\2\u0347\u0081\3\2\2\2\u0348\u0349")
-        buf.write("\bB\1\2\u0349\u0363\7l\2\2\u034a\u0363\7i\2\2\u034b\u0363")
-        buf.write("\5\u00d2j\2\u034c\u0363\7k\2\2\u034d\u0363\7m\2\2\u034e")
-        buf.write("\u0363\7n\2\2\u034f\u0363\5\u0080A\2\u0350\u0363\5\u0098")
-        buf.write("M\2\u0351\u0363\5\u00b2Z\2\u0352\u0363\5\u00b6\\\2\u0353")
-        buf.write("\u0354\7e\2\2\u0354\u0355\5f\64\2\u0355\u0356\7f\2\2\u0356")
-        buf.write("\u0363\3\2\2\2\u0357\u0358\5\u0086D\2\u0358\u035a\7n\2")
-        buf.write("\2\u0359\u035b\5\u00c8e\2\u035a\u0359\3\2\2\2\u035a\u035b")
-        buf.write("\3\2\2\2\u035b\u0363\3\2\2\2\u035c\u035d\7\64\2\2\u035d")
-        buf.write("\u0363\5\u0082B\7\u035e\u0363\5\u00ba^\2\u035f\u0363\5")
-        buf.write("\u0088E\2\u0360\u0363\5\u008aF\2\u0361\u0363\5\u00d0i")
-        buf.write("\2\u0362\u0348\3\2\2\2\u0362\u034a\3\2\2\2\u0362\u034b")
-        buf.write("\3\2\2\2\u0362\u034c\3\2\2\2\u0362\u034d\3\2\2\2\u0362")
-        buf.write("\u034e\3\2\2\2\u0362\u034f\3\2\2\2\u0362\u0350\3\2\2\2")
-        buf.write("\u0362\u0351\3\2\2\2\u0362\u0352\3\2\2\2\u0362\u0353\3")
-        buf.write("\2\2\2\u0362\u0357\3\2\2\2\u0362\u035c\3\2\2\2\u0362\u035e")
-        buf.write("\3\2\2\2\u0362\u035f\3\2\2\2\u0362\u0360\3\2\2\2\u0362")
-        buf.write("\u0361\3\2\2\2\u0363\u0368\3\2\2\2\u0364\u0365\f\b\2\2")
-        buf.write("\u0365\u0367\5\u0084C\2\u0366\u0364\3\2\2\2\u0367\u036a")
-        buf.write("\3\2\2\2\u0368\u0366\3\2\2\2\u0368\u0369\3\2\2\2\u0369")
-        buf.write("\u0083\3\2\2\2\u036a\u0368\3\2\2\2\u036b\u036c\7P\2\2")
-        buf.write("\u036c\u037b\5\u008cG\2\u036d\u036e\7P\2\2\u036e\u037b")
-        buf.write("\7n\2\2\u036f\u037b\5\u00b4[\2\u0370\u0372\7e\2\2\u0371")
-        buf.write("\u0373\5:\36\2\u0372\u0371\3\2\2\2\u0372\u0373\3\2\2\2")
-        buf.write("\u0373\u0374\3\2\2\2\u0374\u037b\7f\2\2\u0375\u0376\5")
-        buf.write("\u0086D\2\u0376\u0378\7n\2\2\u0377\u0379\5\u00c8e\2\u0378")
-        buf.write("\u0377\3\2\2\2\u0378\u0379\3\2\2\2\u0379\u037b\3\2\2\2")
-        buf.write("\u037a\u036b\3\2\2\2\u037a\u036d\3\2\2\2\u037a\u036f\3")
-        buf.write("\2\2\2\u037a\u0370\3\2\2\2\u037a\u0375\3\2\2\2\u037b\u0085")
-        buf.write("\3\2\2\2\u037c\u0381\7%\2\2\u037d\u037e\7%\2\2\u037e\u037f")
-        buf.write("\7n\2\2\u037f\u0381\7$\2\2\u0380\u037c\3\2\2\2\u0380\u037d")
-        buf.write("\3\2\2\2\u0381\u0087\3\2\2\2\u0382\u0383\7O\2\2\u0383")
-        buf.write("\u0384\5\u0082B\2\u0384\u0089\3\2\2\2\u0385\u0386\7a\2")
-        buf.write("\2\u0386\u0387\5\u0082B\2\u0387\u008b\3\2\2\2\u0388\u038f")
-        buf.write("\3\2\2\2\u0389\u038f\5\u0096L\2\u038a\u038f\5\u0092J\2")
-        buf.write("\u038b\u038f\5\u0094K\2\u038c\u038f\5\u0090I\2\u038d\u038f")
-        buf.write("\5\u008eH\2\u038e\u0388\3\2\2\2\u038e\u0389\3\2\2\2\u038e")
-        buf.write("\u038a\3\2\2\2\u038e\u038b\3\2\2\2\u038e\u038c\3\2\2\2")
-        buf.write("\u038e\u038d\3\2\2\2\u038f\u008d\3\2\2\2\u0390\u0391\5")
-        buf.write("\u00d0i\2\u0391\u008f\3\2\2\2\u0392\u0393\t\b\2\2\u0393")
-        buf.write("\u0091\3\2\2\2\u0394\u03a6\7\36\2\2\u0395\u0396\7/\2\2")
-        buf.write("\u0396\u0397\58\35\2\u0397\u0398\7\60\2\2\u0398\u03a6")
-        buf.write("\3\2\2\2\u0399\u039a\7\22\2\2\u039a\u039d\7%\2\2\u039b")
-        buf.write("\u039d\7(\2\2\u039c\u0399\3\2\2\2\u039c\u039b\3\2\2\2")
-        buf.write("\u039d\u039e\3\2\2\2\u039e\u03a3\t\t\2\2\u039f\u03a0\7")
-        buf.write("e\2\2\u03a0\u03a1\5<\37\2\u03a1\u03a2\7f\2\2\u03a2\u03a4")
-        buf.write("\3\2\2\2\u03a3\u039f\3\2\2\2\u03a3\u03a4\3\2\2\2\u03a4")
-        buf.write("\u03a6\3\2\2\2\u03a5\u0394\3\2\2\2\u03a5\u0395\3\2\2\2")
-        buf.write("\u03a5\u039c\3\2\2\2\u03a6\u0093\3\2\2\2\u03a7\u03b5\7")
-        buf.write("\35\2\2\u03a8\u03a9\7\21\2\2\u03a9\u03ac\7%\2\2\u03aa")
-        buf.write("\u03ac\7'\2\2\u03ab\u03a8\3\2\2\2\u03ab\u03aa\3\2\2\2")
-        buf.write("\u03ac\u03ad\3\2\2\2\u03ad\u03b2\7n\2\2\u03ae\u03af\7")
-        buf.write("e\2\2\u03af\u03b0\5<\37\2\u03b0\u03b1\7f\2\2\u03b1\u03b3")
-        buf.write("\3\2\2\2\u03b2\u03ae\3\2\2\2\u03b2\u03b3\3\2\2\2\u03b3")
-        buf.write("\u03b5\3\2\2\2\u03b4\u03a7\3\2\2\2\u03b4\u03ab\3\2\2\2")
-        buf.write("\u03b5\u0095\3\2\2\2\u03b6\u03b7\7\16\2\2\u03b7\u03ba")
-        buf.write("\7%\2\2\u03b8\u03ba\7&\2\2\u03b9\u03b6\3\2\2\2\u03b9\u03b8")
-        buf.write("\3\2\2\2\u03ba\u03bb\3\2\2\2\u03bb\u03c0\7n\2\2\u03bc")
-        buf.write("\u03bd\7e\2\2\u03bd\u03be\5<\37\2\u03be\u03bf\7f\2\2\u03bf")
-        buf.write("\u03c1\3\2\2\2\u03c0\u03bc\3\2\2\2\u03c0\u03c1\3\2\2\2")
-        buf.write("\u03c1\u0097\3\2\2\2\u03c2\u03c4\5\u009aN\2\u03c3\u03c5")
-        buf.write("\5\u00caf\2\u03c4\u03c3\3\2\2\2\u03c4\u03c5\3\2\2\2\u03c5")
-        buf.write("\u03c7\3\2\2\2\u03c6\u03c8\5\u0098M\2\u03c7\u03c6\3\2")
-        buf.write("\2\2\u03c7\u03c8\3\2\2\2\u03c8\u03ce\3\2\2\2\u03c9\u03cb")
-        buf.write("\5\u00a2R\2\u03ca\u03cc\5\u0098M\2\u03cb\u03ca\3\2\2\2")
-        buf.write("\u03cb\u03cc\3\2\2\2\u03cc\u03ce\3\2\2\2\u03cd\u03c2\3")
-        buf.write("\2\2\2\u03cd\u03c9\3\2\2\2\u03ce\u0099\3\2\2\2\u03cf\u03d0")
-        buf.write("\7)\2\2\u03d0\u03d1\7n\2\2\u03d1\u009b\3\2\2\2\u03d2\u03d3")
-        buf.write("\7+\2\2\u03d3\u03d4\7n\2\2\u03d4\u009d\3\2\2\2\u03d5\u03d6")
-        buf.write("\7,\2\2\u03d6\u03d7\7n\2\2\u03d7\u009f\3\2\2\2\u03d8\u03d9")
-        buf.write("\7-\2\2\u03d9\u03da\7n\2\2\u03da\u00a1\3\2\2\2\u03db\u03df")
-        buf.write("\5\u00a4S\2\u03dc\u03df\5\u00a6T\2\u03dd\u03df\5\u00a8")
-        buf.write("U\2\u03de\u03db\3\2\2\2\u03de\u03dc\3\2\2\2\u03de\u03dd")
-        buf.write("\3\2\2\2\u03df\u00a3\3\2\2\2\u03e0\u03ec\7\4\2\2\u03e1")
-        buf.write("\u03e8\7`\2\2\u03e2\u03e3\7g\2\2\u03e3\u03e5\7n\2\2\u03e4")
-        buf.write("\u03e6\5\u00caf\2\u03e5\u03e4\3\2\2\2\u03e5\u03e6\3\2")
-        buf.write("\2\2\u03e6\u03e7\3\2\2\2\u03e7\u03e9\7h\2\2\u03e8\u03e2")
-        buf.write("\3\2\2\2\u03e8\u03e9\3\2\2\2\u03e9\u03ea\3\2\2\2\u03ea")
-        buf.write("\u03ec\7\5\2\2\u03eb\u03e0\3\2\2\2\u03eb\u03e1\3\2\2\2")
-        buf.write("\u03ec\u00a5\3\2\2\2\u03ed\u03f9\7\6\2\2\u03ee\u03f5\7")
-        buf.write("\7\2\2\u03ef\u03f0\7g\2\2\u03f0\u03f2\7n\2\2\u03f1\u03f3")
-        buf.write("\5\u00caf\2\u03f2\u03f1\3\2\2\2\u03f2\u03f3\3\2\2\2\u03f3")
-        buf.write("\u03f4\3\2\2\2\u03f4\u03f6\7h\2\2\u03f5\u03ef\3\2\2\2")
-        buf.write("\u03f5\u03f6\3\2\2\2\u03f6\u03f7\3\2\2\2\u03f7\u03f9\7")
-        buf.write("`\2\2\u03f8\u03ed\3\2\2\2\u03f8\u03ee\3\2\2\2\u03f9\u00a7")
-        buf.write("\3\2\2\2\u03fa\u0406\7\b\2\2\u03fb\u0402\7\7\2\2\u03fc")
-        buf.write("\u03fd\7g\2\2\u03fd\u03ff\7n\2\2\u03fe\u0400\5\u00caf")
-        buf.write("\2\u03ff\u03fe\3\2\2\2\u03ff\u0400\3\2\2\2\u0400\u0401")
-        buf.write("\3\2\2\2\u0401\u0403\7h\2\2\u0402\u03fc\3\2\2\2\u0402")
-        buf.write("\u0403\3\2\2\2\u0403\u0404\3\2\2\2\u0404\u0406\7\5\2\2")
-        buf.write("\u0405\u03fa\3\2\2\2\u0405\u03fb\3\2\2\2\u0406\u00a9\3")
-        buf.write("\2\2\2\u0407\u040b\5\u00acW\2\u0408\u040b\5\u00aeX\2\u0409")
-        buf.write("\u040b\5\u00b0Y\2\u040a\u0407\3\2\2\2\u040a\u0408\3\2")
-        buf.write("\2\2\u040a\u0409\3\2\2\2\u040b\u00ab\3\2\2\2\u040c\u0418")
-        buf.write("\7\t\2\2\u040d\u0414\7_\2\2\u040e\u040f\7g\2\2\u040f\u0411")
-        buf.write("\7n\2\2\u0410\u0412\5\u00c8e\2\u0411\u0410\3\2\2\2\u0411")
-        buf.write("\u0412\3\2\2\2\u0412\u0413\3\2\2\2\u0413\u0415\7h\2\2")
-        buf.write("\u0414\u040e\3\2\2\2\u0414\u0415\3\2\2\2\u0415\u0416\3")
-        buf.write("\2\2\2\u0416\u0418\7\n\2\2\u0417\u040c\3\2\2\2\u0417\u040d")
-        buf.write("\3\2\2\2\u0418\u00ad\3\2\2\2\u0419\u0425\7\13\2\2\u041a")
-        buf.write("\u0421\7\f\2\2\u041b\u041c\7g\2\2\u041c\u041e\7n\2\2\u041d")
-        buf.write("\u041f\5\u00c8e\2\u041e\u041d\3\2\2\2\u041e\u041f\3\2")
-        buf.write("\2\2\u041f\u0420\3\2\2\2\u0420\u0422\7h\2\2\u0421\u041b")
-        buf.write("\3\2\2\2\u0421\u0422\3\2\2\2\u0422\u0423\3\2\2\2\u0423")
-        buf.write("\u0425\7_\2\2\u0424\u0419\3\2\2\2\u0424\u041a\3\2\2\2")
-        buf.write("\u0425\u00af\3\2\2\2\u0426\u0432\7\r\2\2\u0427\u042e\7")
-        buf.write("\f\2\2\u0428\u0429\7g\2\2\u0429\u042b\7n\2\2\u042a\u042c")
-        buf.write("\5\u00c8e\2\u042b\u042a\3\2\2\2\u042b\u042c\3\2\2\2\u042c")
-        buf.write("\u042d\3\2\2\2\u042d\u042f\7h\2\2\u042e\u0428\3\2\2\2")
-        buf.write("\u042e\u042f\3\2\2\2\u042f\u0430\3\2\2\2\u0430\u0432\7")
-        buf.write("\n\2\2\u0431\u0426\3\2\2\2\u0431\u0427\3\2\2\2\u0432\u00b1")
-        buf.write("\3\2\2\2\u0433\u0435\7g\2\2\u0434\u0436\5<\37\2\u0435")
-        buf.write("\u0434\3\2\2\2\u0435\u0436\3\2\2\2\u0436\u0437\3\2\2\2")
-        buf.write("\u0437\u0438\7h\2\2\u0438\u00b3\3\2\2\2\u0439\u043a\7")
-        buf.write("g\2\2\u043a\u043b\5f\64\2\u043b\u043c\7h\2\2\u043c\u0444")
-        buf.write("\3\2\2\2\u043d\u043e\7g\2\2\u043e\u043f\5f\64\2\u043f")
-        buf.write("\u0440\7$\2\2\u0440\u0441\5f\64\2\u0441\u0442\7h\2\2\u0442")
-        buf.write("\u0444\3\2\2\2\u0443\u0439\3\2\2\2\u0443\u043d\3\2\2\2")
-        buf.write("\u0444\u00b5\3\2\2\2\u0445\u044e\7/\2\2\u0446\u044b\5")
-        buf.write("\u00b8]\2\u0447\u0448\7]\2\2\u0448\u044a\5\u00b8]\2\u0449")
-        buf.write("\u0447\3\2\2\2\u044a\u044d\3\2\2\2\u044b\u0449\3\2\2\2")
-        buf.write("\u044b\u044c\3\2\2\2\u044c\u044f\3\2\2\2\u044d\u044b\3")
-        buf.write("\2\2\2\u044e\u0446\3\2\2\2\u044e\u044f\3\2\2\2\u044f\u0450")
-        buf.write("\3\2\2\2\u0450\u0451\7\60\2\2\u0451\u00b7\3\2\2\2\u0452")
-        buf.write("\u0453\5f\64\2\u0453\u0454\7$\2\2\u0454\u0455\5f\64\2")
-        buf.write("\u0455\u00b9\3\2\2\2\u0456\u0457\7\31\2\2\u0457\u0458")
-        buf.write("\5\u00bc_\2\u0458\u00bb\3\2\2\2\u0459\u045e\5\u00c0a\2")
-        buf.write("\u045a\u045e\5\u00c4c\2\u045b\u045e\5\u00c2b\2\u045c\u045e")
-        buf.write("\5\u00c6d\2\u045d\u0459\3\2\2\2\u045d\u045a\3\2\2\2\u045d")
-        buf.write("\u045b\3\2\2\2\u045d\u045c\3\2\2\2\u045e\u00bd\3\2\2\2")
-        buf.write("\u045f\u0460\5f\64\2\u0460\u0461\5\u00aaV\2\u0461\u00bf")
-        buf.write("\3\2\2\2\u0462\u0464\5\u00be`\2\u0463\u0462\3\2\2\2\u0463")
-        buf.write("\u0464\3\2\2\2\u0464\u0465\3\2\2\2\u0465\u0467\5\u009a")
-        buf.write("N\2\u0466\u0468\5\u00c8e\2\u0467\u0466\3\2\2\2\u0467\u0468")
-        buf.write("\3\2\2\2\u0468\u00c1\3\2\2\2\u0469\u046b\5\u00be`\2\u046a")
-        buf.write("\u0469\3\2\2\2\u046a\u046b\3\2\2\2\u046b\u046c\3\2\2\2")
-        buf.write("\u046c\u046d\5\u009eP\2\u046d\u00c3\3\2\2\2\u046e\u0470")
-        buf.write("\5f\64\2\u046f\u0471\7\64\2\2\u0470\u046f\3\2\2\2\u0470")
-        buf.write("\u0471\3\2\2\2\u0471\u0472\3\2\2\2\u0472\u0474\5\u009c")
-        buf.write("O\2\u0473\u0475\5\u00c8e\2\u0474\u0473\3\2\2\2\u0474\u0475")
-        buf.write("\3\2\2\2\u0475\u00c5\3\2\2\2\u0476\u0478\5\u00a0Q\2\u0477")
-        buf.write("\u0479\5\u00c8e\2\u0478\u0477\3\2\2\2\u0478\u0479\3\2")
-        buf.write("\2\2\u0479\u00c7\3\2\2\2\u047a\u0483\7e\2\2\u047b\u0480")
-        buf.write("\5\u00ccg\2\u047c\u047d\7]\2\2\u047d\u047f\5\u00ccg\2")
-        buf.write("\u047e\u047c\3\2\2\2\u047f\u0482\3\2\2\2\u0480\u047e\3")
-        buf.write("\2\2\2\u0480\u0481\3\2\2\2\u0481\u0484\3\2\2\2\u0482\u0480")
-        buf.write("\3\2\2\2\u0483\u047b\3\2\2\2\u0483\u0484\3\2\2\2\u0484")
-        buf.write("\u0485\3\2\2\2\u0485\u0486\7f\2\2\u0486\u00c9\3\2\2\2")
-        buf.write("\u0487\u0490\7e\2\2\u0488\u048d\5\u00ceh\2\u0489\u048a")
-        buf.write("\7]\2\2\u048a\u048c\5\u00ceh\2\u048b\u0489\3\2\2\2\u048c")
-        buf.write("\u048f\3\2\2\2\u048d\u048b\3\2\2\2\u048d\u048e\3\2\2\2")
-        buf.write("\u048e\u0491\3\2\2\2\u048f\u048d\3\2\2\2\u0490\u0488\3")
-        buf.write("\2\2\2\u0490\u0491\3\2\2\2\u0491\u0492\3\2\2\2\u0492\u0493")
-        buf.write("\7f\2\2\u0493\u00cb\3\2\2\2\u0494\u0495\7n\2\2\u0495\u0496")
-        buf.write("\78\2\2\u0496\u0497\5f\64\2\u0497\u00cd\3\2\2\2\u0498")
-        buf.write("\u0499\7n\2\2\u0499\u049a\5t;\2\u049a\u049b\5f\64\2\u049b")
-        buf.write("\u00cf\3\2\2\2\u049c\u049d\t\n\2\2\u049d\u00d1\3\2\2\2")
-        buf.write("\u049e\u04a0\7j\2\2\u049f\u049e\3\2\2\2\u04a0\u04a1\3")
-        buf.write("\2\2\2\u04a1\u049f\3\2\2\2\u04a1\u04a2\3\2\2\2\u04a2\u00d3")
-        buf.write("\3\2\2\2\u0092\u00d5\u00da\u00e0\u00e9\u00ef\u00f9\u00fd")
+        buf.write("\u01bc\5*\26\2\u01ba\u01bc\5.\30\2\u01bb\u01b9\3\2\2\2")
+        buf.write("\u01bb\u01ba\3\2\2\2\u01bc!\3\2\2\2\u01bd\u01c1\7/\2\2")
+        buf.write("\u01be\u01c0\5*\26\2\u01bf\u01be\3\2\2\2\u01c0\u01c3\3")
+        buf.write("\2\2\2\u01c1\u01bf\3\2\2\2\u01c1\u01c2\3\2\2\2\u01c2\u01c4")
+        buf.write("\3\2\2\2\u01c3\u01c1\3\2\2\2\u01c4\u01c9\7\60\2\2\u01c5")
+        buf.write("\u01c6\7$\2\2\u01c6\u01c9\5*\26\2\u01c7\u01c9\7\67\2\2")
+        buf.write("\u01c8\u01bd\3\2\2\2\u01c8\u01c5\3\2\2\2\u01c8\u01c7\3")
+        buf.write("\2\2\2\u01c9#\3\2\2\2\u01ca\u01cc\5.\30\2\u01cb\u01ca")
+        buf.write("\3\2\2\2\u01cc\u01cf\3\2\2\2\u01cd\u01cb\3\2\2\2\u01cd")
+        buf.write("\u01ce\3\2\2\2\u01ce%\3\2\2\2\u01cf\u01cd\3\2\2\2\u01d0")
+        buf.write("\u01d1\7/\2\2\u01d1\u01d2\5(\25\2\u01d2\u01d3\5$\23\2")
+        buf.write("\u01d3\u01d4\7\31\2\2\u01d4\u01d5\5> \2\u01d5\u01d6\7")
+        buf.write("\60\2\2\u01d6\u01df\3\2\2\2\u01d7\u01d8\7$\2\2\u01d8\u01d9")
+        buf.write("\5(\25\2\u01d9\u01da\5$\23\2\u01da\u01db\7\31\2\2\u01db")
+        buf.write("\u01dc\5> \2\u01dc\u01dd\7\67\2\2\u01dd\u01df\3\2\2\2")
+        buf.write("\u01de\u01d0\3\2\2\2\u01de\u01d7\3\2\2\2\u01df'\3\2\2")
+        buf.write("\2\u01e0\u01e1\7Z\2\2\u01e1\u01e2\7Y\2\2\u01e2\u01e3\7")
+        buf.write("n\2\2\u01e3\u01e4\7\67\2\2\u01e4)\3\2\2\2\u01e5\u01e6")
+        buf.write("\7Z\2\2\u01e6\u01eb\5,\27\2\u01e7\u01e8\7]\2\2\u01e8\u01ea")
+        buf.write("\5,\27\2\u01e9\u01e7\3\2\2\2\u01ea\u01ed\3\2\2\2\u01eb")
+        buf.write("\u01e9\3\2\2\2\u01eb\u01ec\3\2\2\2\u01ec\u01ee\3\2\2\2")
+        buf.write("\u01ed\u01eb\3\2\2\2\u01ee\u01ef\7\67\2\2\u01ef+\3\2\2")
+        buf.write("\2\u01f0\u01f2\7\\\2\2\u01f1\u01f0\3\2\2\2\u01f1\u01f2")
+        buf.write("\3\2\2\2\u01f2\u01f4\3\2\2\2\u01f3\u01f5\7Y\2\2\u01f4")
+        buf.write("\u01f3\3\2\2\2\u01f4\u01f5\3\2\2\2\u01f5\u01fa\3\2\2\2")
+        buf.write("\u01f6\u01fb\7n\2\2\u01f7\u01f8\7n\2\2\u01f8\u01f9\78")
+        buf.write("\2\2\u01f9\u01fb\5d\63\2\u01fa\u01f6\3\2\2\2\u01fa\u01f7")
+        buf.write("\3\2\2\2\u01fb-\3\2\2\2\u01fc\u01fd\7^\2\2\u01fd\u0201")
+        buf.write("\5\64\33\2\u01fe\u01ff\5\62\32\2\u01ff\u0200\5\60\31\2")
+        buf.write("\u0200\u0202\3\2\2\2\u0201\u01fe\3\2\2\2\u0201\u0202\3")
+        buf.write("\2\2\2\u0202\u020c\3\2\2\2\u0203\u0204\7]\2\2\u0204\u0208")
+        buf.write("\5\64\33\2\u0205\u0206\5\62\32\2\u0206\u0207\5\60\31\2")
+        buf.write("\u0207\u0209\3\2\2\2\u0208\u0205\3\2\2\2\u0208\u0209\3")
+        buf.write("\2\2\2\u0209\u020b\3\2\2\2\u020a\u0203\3\2\2\2\u020b\u020e")
+        buf.write("\3\2\2\2\u020c\u020a\3\2\2\2\u020c\u020d\3\2\2\2\u020d")
+        buf.write("\u020f\3\2\2\2\u020e\u020c\3\2\2\2\u020f\u0210\7\67\2")
+        buf.write("\2\u0210\u0218\3\2\2\2\u0211\u0212\7^\2\2\u0212\u0214")
+        buf.write("\7n\2\2\u0213\u0215\5\60\31\2\u0214\u0213\3\2\2\2\u0214")
+        buf.write("\u0215\3\2\2\2\u0215\u0216\3\2\2\2\u0216\u0218\5> \2\u0217")
+        buf.write("\u01fc\3\2\2\2\u0217\u0211\3\2\2\2\u0218/\3\2\2\2\u0219")
+        buf.write("\u021b\7\32\2\2\u021a\u021c\5\66\34\2\u021b\u021a\3\2")
+        buf.write("\2\2\u021b\u021c\3\2\2\2\u021c\u021d\3\2\2\2\u021d\u021e")
+        buf.write("\t\2\2\2\u021e\61\3\2\2\2\u021f\u0221\7%\2\2\u0220\u0222")
+        buf.write("\58\35\2\u0221\u0220\3\2\2\2\u0221\u0222\3\2\2\2\u0222")
+        buf.write("\u0226\3\2\2\2\u0223\u0227\7%\2\2\u0224\u0225\7.\2\2\u0225")
+        buf.write("\u0227\5d\63\2\u0226\u0223\3\2\2\2\u0226\u0224\3\2\2\2")
+        buf.write("\u0227\63\3\2\2\2\u0228\u0229\7n\2\2\u0229\u022a\7P\2")
+        buf.write("\2\u022a\u022b\7n\2\2\u022b\65\3\2\2\2\u022c\u0231\7n")
+        buf.write("\2\2\u022d\u022e\7]\2\2\u022e\u0230\7n\2\2\u022f\u022d")
+        buf.write("\3\2\2\2\u0230\u0233\3\2\2\2\u0231\u022f\3\2\2\2\u0231")
+        buf.write("\u0232\3\2\2\2\u0232\67\3\2\2\2\u0233\u0231\3\2\2\2\u0234")
+        buf.write("\u023b\5:\36\2\u0235\u023b\5<\37\2\u0236\u0237\5:\36\2")
+        buf.write("\u0237\u0238\7]\2\2\u0238\u0239\5<\37\2\u0239\u023b\3")
+        buf.write("\2\2\2\u023a\u0234\3\2\2\2\u023a\u0235\3\2\2\2\u023a\u0236")
+        buf.write("\3\2\2\2\u023b9\3\2\2\2\u023c\u0241\5l\67\2\u023d\u023e")
+        buf.write("\7]\2\2\u023e\u0240\5l\67\2\u023f\u023d\3\2\2\2\u0240")
+        buf.write("\u0243\3\2\2\2\u0241\u023f\3\2\2\2\u0241\u0242\3\2\2\2")
+        buf.write("\u0242;\3\2\2\2\u0243\u0241\3\2\2\2\u0244\u0245\7n\2\2")
+        buf.write("\u0245\u0246\78\2\2\u0246\u024d\5l\67\2\u0247\u0248\7")
+        buf.write("]\2\2\u0248\u0249\7n\2\2\u0249\u024a\78\2\2\u024a\u024c")
+        buf.write("\5l\67\2\u024b\u0247\3\2\2\2\u024c\u024f\3\2\2\2\u024d")
+        buf.write("\u024b\3\2\2\2\u024d\u024e\3\2\2\2\u024e=\3\2\2\2\u024f")
+        buf.write('\u024d\3\2\2\2\u0250\u0254\7/\2\2\u0251\u0253\5B"\2\u0252')
+        buf.write("\u0251\3\2\2\2\u0253\u0256\3\2\2\2\u0254\u0252\3\2\2\2")
+        buf.write("\u0254\u0255\3\2\2\2\u0255\u0257\3\2\2\2\u0256\u0254\3")
+        buf.write("\2\2\2\u0257\u025b\7\60\2\2\u0258\u0259\7$\2\2\u0259\u025b")
+        buf.write('\5B"\2\u025a\u0250\3\2\2\2\u025a\u0258\3\2\2\2\u025b')
+        buf.write("?\3\2\2\2\u025c\u025d\5\66\34\2\u025d\u025e\5> \2\u025e")
+        buf.write("A\3\2\2\2\u025f\u0272\5> \2\u0260\u0272\5@!\2\u0261\u0262")
+        buf.write("\5d\63\2\u0262\u0263\7\67\2\2\u0263\u0272\3\2\2\2\u0264")
+        buf.write("\u0272\5D#\2\u0265\u0272\5F$\2\u0266\u0272\5N(\2\u0267")
+        buf.write("\u0272\5P)\2\u0268\u0269\5T+\2\u0269\u026a\7\67\2\2\u026a")
+        buf.write("\u0272\3\2\2\2\u026b\u026c\5R*\2\u026c\u026d\7\67\2\2")
+        buf.write("\u026d\u0272\3\2\2\2\u026e\u0272\5V,\2\u026f\u0272\5X")
+        buf.write("-\2\u0270\u0272\5Z.\2\u0271\u025f\3\2\2\2\u0271\u0260")
+        buf.write("\3\2\2\2\u0271\u0261\3\2\2\2\u0271\u0264\3\2\2\2\u0271")
+        buf.write("\u0265\3\2\2\2\u0271\u0266\3\2\2\2\u0271\u0267\3\2\2\2")
+        buf.write("\u0271\u0268\3\2\2\2\u0271\u026b\3\2\2\2\u0271\u026e\3")
+        buf.write("\2\2\2\u0271\u026f\3\2\2\2\u0271\u0270\3\2\2\2\u0272C")
+        buf.write("\3\2\2\2\u0273\u0274\7@\2\2\u0274\u0275\5d\63\2\u0275")
+        buf.write("\u0279\5> \2\u0276\u0278\5J&\2\u0277\u0276\3\2\2\2\u0278")
+        buf.write("\u027b\3\2\2\2\u0279\u0277\3\2\2\2\u0279\u027a\3\2\2\2")
+        buf.write("\u027a\u027d\3\2\2\2\u027b\u0279\3\2\2\2\u027c\u027e\5")
+        buf.write("L'\2\u027d\u027c\3\2\2\2\u027d\u027e\3\2\2\2\u027eE\3")
+        buf.write("\2\2\2\u027f\u0280\7N\2\2\u0280\u0282\5> \2\u0281\u0283")
+        buf.write("\5H%\2\u0282\u0281\3\2\2\2\u0282\u0283\3\2\2\2\u0283G")
+        buf.write("\3\2\2\2\u0284\u0288\7B\2\2\u0285\u0286\7e\2\2\u0286\u0287")
+        buf.write("\7n\2\2\u0287\u0289\7f\2\2\u0288\u0285\3\2\2\2\u0288\u0289")
+        buf.write("\3\2\2\2\u0289\u028a\3\2\2\2\u028a\u0292\5> \2\u028b\u028e")
+        buf.write("\7B\2\2\u028c\u028d\7\32\2\2\u028d\u028f\7n\2\2\u028e")
+        buf.write("\u028c\3\2\2\2\u028e\u028f\3\2\2\2\u028f\u0290\3\2\2\2")
+        buf.write("\u0290\u0292\5> \2\u0291\u0284\3\2\2\2\u0291\u028b\3\2")
+        buf.write("\2\2\u0292I\3\2\2\2\u0293\u0294\7A\2\2\u0294\u0295\5d")
+        buf.write("\63\2\u0295\u0296\5> \2\u0296K\3\2\2\2\u0297\u0298\7B")
+        buf.write("\2\2\u0298\u0299\5> \2\u0299M\3\2\2\2\u029a\u029b\7C\2")
+        buf.write("\2\u029b\u029c\5d\63\2\u029c\u029d\7D\2\2\u029d\u029e")
+        buf.write("\5d\63\2\u029e\u029f\7E\2\2\u029f\u02a0\5d\63\2\u02a0")
+        buf.write("\u02a1\5> \2\u02a1\u02ad\3\2\2\2\u02a2\u02a3\7C\2\2\u02a3")
+        buf.write("\u02a6\7n\2\2\u02a4\u02a5\7]\2\2\u02a5\u02a7\7n\2\2\u02a6")
+        buf.write("\u02a4\3\2\2\2\u02a6\u02a7\3\2\2\2\u02a7\u02a8\3\2\2\2")
+        buf.write("\u02a8\u02a9\7X\2\2\u02a9\u02aa\5d\63\2\u02aa\u02ab\5")
+        buf.write("> \2\u02ab\u02ad\3\2\2\2\u02ac\u029a\3\2\2\2\u02ac\u02a2")
+        buf.write("\3\2\2\2\u02adO\3\2\2\2\u02ae\u02af\7F\2\2\u02af\u02b0")
+        buf.write("\5d\63\2\u02b0\u02b1\5> \2\u02b1Q\3\2\2\2\u02b2\u02b3")
+        buf.write("\t\3\2\2\u02b3S\3\2\2\2\u02b4\u02b5\7\66\2\2\u02b5\u02b6")
+        buf.write("\5d\63\2\u02b6U\3\2\2\2\u02b7\u02b8\7M\2\2\u02b8\u02b9")
+        buf.write("\5d\63\2\u02b9\u02ba\7\67\2\2\u02baW\3\2\2\2\u02bb\u02bc")
+        buf.write("\7L\2\2\u02bc\u02bd\5d\63\2\u02bd\u02be\7\67\2\2\u02be")
+        buf.write("\u02c7\3\2\2\2\u02bf\u02c0\7L\2\2\u02c0\u02c1\7$\2\2\u02c1")
+        buf.write("\u02c2\7n\2\2\u02c2\u02c3\78\2\2\u02c3\u02c4\5d\63\2\u02c4")
+        buf.write("\u02c5\7\67\2\2\u02c5\u02c7\3\2\2\2\u02c6\u02bb\3\2\2")
+        buf.write("\2\u02c6\u02bf\3\2\2\2\u02c7Y\3\2\2\2\u02c8\u02cd\5\\")
+        buf.write("/\2\u02c9\u02cd\5^\60\2\u02ca\u02cd\5`\61\2\u02cb\u02cd")
+        buf.write("\5b\62\2\u02cc\u02c8\3\2\2\2\u02cc\u02c9\3\2\2\2\u02cc")
+        buf.write("\u02ca\3\2\2\2\u02cc\u02cb\3\2\2\2\u02cd[\3\2\2\2\u02ce")
+        buf.write("\u02cf\7\27\2\2\u02cf\u02d0\5d\63\2\u02d0\u02d1\7\67\2")
+        buf.write("\2\u02d1]\3\2\2\2\u02d2\u02d5\7\30\2\2\u02d3\u02d4\7$")
+        buf.write("\2\2\u02d4\u02d6\7n\2\2\u02d5\u02d3\3\2\2\2\u02d5\u02d6")
+        buf.write("\3\2\2\2\u02d6\u02d7\3\2\2\2\u02d7\u02da\5d\63\2\u02d8")
+        buf.write("\u02db\7\67\2\2\u02d9\u02db\5L'\2\u02da\u02d8\3\2\2\2")
+        buf.write("\u02da\u02d9\3\2\2\2\u02db_\3\2\2\2\u02dc\u02df\7I\2\2")
+        buf.write("\u02dd\u02e0\5X-\2\u02de\u02e0\7\67\2\2\u02df\u02dd\3")
+        buf.write("\2\2\2\u02df\u02de\3\2\2\2\u02e0a\3\2\2\2\u02e1\u02e6")
+        buf.write("\7J\2\2\u02e2\u02e7\5X-\2\u02e3\u02e7\5`\61\2\u02e4\u02e7")
+        buf.write("\5^\60\2\u02e5\u02e7\7\67\2\2\u02e6\u02e2\3\2\2\2\u02e6")
+        buf.write("\u02e3\3\2\2\2\u02e6\u02e4\3\2\2\2\u02e6\u02e5\3\2\2\2")
+        buf.write("\u02e7c\3\2\2\2\u02e8\u02ec\5l\67\2\u02e9\u02ed\5f\64")
+        buf.write("\2\u02ea\u02ed\5h\65\2\u02eb\u02ed\5j\66\2\u02ec\u02e9")
+        buf.write("\3\2\2\2\u02ec\u02ea\3\2\2\2\u02ec\u02eb\3\2\2\2\u02ec")
+        buf.write("\u02ed\3\2\2\2\u02ede\3\2\2\2\u02ee\u02ef\78\2\2\u02ef")
+        buf.write("\u02f0\5d\63\2\u02f0g\3\2\2\2\u02f1\u02f2\7=\2\2\u02f2")
+        buf.write("\u02f3\5d\63\2\u02f3i\3\2\2\2\u02f4\u02f5\t\4\2\2\u02f5")
+        buf.write("\u02f6\5d\63\2\u02f6k\3\2\2\2\u02f7\u02ff\5n8\2\u02f8")
+        buf.write("\u02f9\7Q\2\2\u02f9\u02fc\5\u00a2R\2\u02fa\u02fc\5\u00aa")
+        buf.write("V\2\u02fb\u02f8\3\2\2\2\u02fb\u02fa\3\2\2\2\u02fc\u02fd")
+        buf.write("\3\2\2\2\u02fd\u02fe\5d\63\2\u02fe\u0300\3\2\2\2\u02ff")
+        buf.write("\u02fb\3\2\2\2\u02ff\u0300\3\2\2\2\u0300m\3\2\2\2\u0301")
+        buf.write("\u0306\5p9\2\u0302\u0303\t\5\2\2\u0303\u0305\5p9\2\u0304")
+        buf.write("\u0302\3\2\2\2\u0305\u0308\3\2\2\2\u0306\u0304\3\2\2\2")
+        buf.write("\u0306\u0307\3\2\2\2\u0307o\3\2\2\2\u0308\u0306\3\2\2")
+        buf.write("\2\u0309\u030a\7Q\2\2\u030a\u0315\5p9\2\u030b\u0311\5")
+        buf.write("v<\2\u030c\u030d\5r:\2\u030d\u030e\5v<\2\u030e\u0310\3")
+        buf.write("\2\2\2\u030f\u030c\3\2\2\2\u0310\u0313\3\2\2\2\u0311\u030f")
+        buf.write("\3\2\2\2\u0311\u0312\3\2\2\2\u0312\u0315\3\2\2\2\u0313")
+        buf.write("\u0311\3\2\2\2\u0314\u0309\3\2\2\2\u0314\u030b\3\2\2\2")
+        buf.write("\u0315q\3\2\2\2\u0316\u031f\7R\2\2\u0317\u031f\7S\2\2")
+        buf.write("\u0318\u031f\7T\2\2\u0319\u031f\7U\2\2\u031a\u031f\7V")
+        buf.write("\2\2\u031b\u031f\7W\2\2\u031c\u031f\7X\2\2\u031d\u031f")
+        buf.write("\5t;\2\u031e\u0316\3\2\2\2\u031e\u0317\3\2\2\2\u031e\u0318")
+        buf.write("\3\2\2\2\u031e\u0319\3\2\2\2\u031e\u031a\3\2\2\2\u031e")
+        buf.write("\u031b\3\2\2\2\u031e\u031c\3\2\2\2\u031e\u031d\3\2\2\2")
+        buf.write("\u031fs\3\2\2\2\u0320\u0321\7Q\2\2\u0321\u0322\7X\2\2")
+        buf.write("\u0322u\3\2\2\2\u0323\u0328\5x=\2\u0324\u0325\t\6\2\2")
+        buf.write("\u0325\u0327\5x=\2\u0326\u0324\3\2\2\2\u0327\u032a\3\2")
+        buf.write("\2\2\u0328\u0326\3\2\2\2\u0328\u0329\3\2\2\2\u0329w\3")
+        buf.write("\2\2\2\u032a\u0328\3\2\2\2\u032b\u0330\5z>\2\u032c\u032d")
+        buf.write("\t\7\2\2\u032d\u032f\5z>\2\u032e\u032c\3\2\2\2\u032f\u0332")
+        buf.write("\3\2\2\2\u0330\u032e\3\2\2\2\u0330\u0331\3\2\2\2\u0331")
+        buf.write("y\3\2\2\2\u0332\u0330\3\2\2\2\u0333\u0334\t\6\2\2\u0334")
+        buf.write("\u0337\5z>\2\u0335\u0337\5|?\2\u0336\u0333\3\2\2\2\u0336")
+        buf.write("\u0335\3\2\2\2\u0337{\3\2\2\2\u0338\u033d\5\u0080A\2\u0339")
+        buf.write("\u033a\7d\2\2\u033a\u033c\5z>\2\u033b\u0339\3\2\2\2\u033c")
+        buf.write("\u033f\3\2\2\2\u033d\u033b\3\2\2\2\u033d\u033e\3\2\2\2")
+        buf.write("\u033e}\3\2\2\2\u033f\u033d\3\2\2\2\u0340\u0341\7[\2\2")
+        buf.write("\u0341\u0344\7P\2\2\u0342\u0345\5\u0090I\2\u0343\u0345")
+        buf.write("\7n\2\2\u0344\u0342\3\2\2\2\u0344\u0343\3\2\2\2\u0345")
+        buf.write("\177\3\2\2\2\u0346\u0347\bA\1\2\u0347\u0361\7l\2\2\u0348")
+        buf.write("\u0361\7i\2\2\u0349\u0361\5\u00d2j\2\u034a\u0361\7k\2")
+        buf.write("\2\u034b\u0361\7m\2\2\u034c\u0361\7n\2\2\u034d\u0361\5")
+        buf.write("~@\2\u034e\u0361\5\u0098M\2\u034f\u0361\5\u00b2Z\2\u0350")
+        buf.write("\u0361\5\u00b6\\\2\u0351\u0352\7e\2\2\u0352\u0353\5d\63")
+        buf.write("\2\u0353\u0354\7f\2\2\u0354\u0361\3\2\2\2\u0355\u0356")
+        buf.write("\5\u0086D\2\u0356\u0358\7n\2\2\u0357\u0359\5\u00c8e\2")
+        buf.write("\u0358\u0357\3\2\2\2\u0358\u0359\3\2\2\2\u0359\u0361\3")
+        buf.write("\2\2\2\u035a\u035b\7\64\2\2\u035b\u0361\5\u0080A\7\u035c")
+        buf.write("\u0361\5\u00ba^\2\u035d\u0361\5\u0088E\2\u035e\u0361\5")
+        buf.write("\u008aF\2\u035f\u0361\5\u00d0i\2\u0360\u0346\3\2\2\2\u0360")
+        buf.write("\u0348\3\2\2\2\u0360\u0349\3\2\2\2\u0360\u034a\3\2\2\2")
+        buf.write("\u0360\u034b\3\2\2\2\u0360\u034c\3\2\2\2\u0360\u034d\3")
+        buf.write("\2\2\2\u0360\u034e\3\2\2\2\u0360\u034f\3\2\2\2\u0360\u0350")
+        buf.write("\3\2\2\2\u0360\u0351\3\2\2\2\u0360\u0355\3\2\2\2\u0360")
+        buf.write("\u035a\3\2\2\2\u0360\u035c\3\2\2\2\u0360\u035d\3\2\2\2")
+        buf.write("\u0360\u035e\3\2\2\2\u0360\u035f\3\2\2\2\u0361\u0366\3")
+        buf.write("\2\2\2\u0362\u0363\f\b\2\2\u0363\u0365\5\u0082B\2\u0364")
+        buf.write("\u0362\3\2\2\2\u0365\u0368\3\2\2\2\u0366\u0364\3\2\2\2")
+        buf.write("\u0366\u0367\3\2\2\2\u0367\u0081\3\2\2\2\u0368\u0366\3")
+        buf.write("\2\2\2\u0369\u036a\7P\2\2\u036a\u0370\5\u008cG\2\u036b")
+        buf.write("\u036c\7P\2\2\u036c\u0370\7n\2\2\u036d\u0370\5\u00b4[")
+        buf.write("\2\u036e\u0370\5\u0084C\2\u036f\u0369\3\2\2\2\u036f\u036b")
+        buf.write("\3\2\2\2\u036f\u036d\3\2\2\2\u036f\u036e\3\2\2\2\u0370")
+        buf.write("\u0083\3\2\2\2\u0371\u0373\7e\2\2\u0372\u0374\58\35\2")
+        buf.write("\u0373\u0372\3\2\2\2\u0373\u0374\3\2\2\2\u0374\u0375\3")
+        buf.write("\2\2\2\u0375\u037c\7f\2\2\u0376\u0377\5\u0086D\2\u0377")
+        buf.write("\u0379\7n\2\2\u0378\u037a\5\u00c8e\2\u0379\u0378\3\2\2")
+        buf.write("\2\u0379\u037a\3\2\2\2\u037a\u037c\3\2\2\2\u037b\u0371")
+        buf.write("\3\2\2\2\u037b\u0376\3\2\2\2\u037c\u0085\3\2\2\2\u037d")
+        buf.write("\u0382\7%\2\2\u037e\u037f\7%\2\2\u037f\u0380\7n\2\2\u0380")
+        buf.write("\u0382\7$\2\2\u0381\u037d\3\2\2\2\u0381\u037e\3\2\2\2")
+        buf.write("\u0382\u0087\3\2\2\2\u0383\u0384\7O\2\2\u0384\u0385\5")
+        buf.write("\u0080A\2\u0385\u0089\3\2\2\2\u0386\u0387\7a\2\2\u0387")
+        buf.write("\u0388\5\u0080A\2\u0388\u008b\3\2\2\2\u0389\u0390\3\2")
+        buf.write("\2\2\u038a\u0390\5\u0096L\2\u038b\u0390\5\u0092J\2\u038c")
+        buf.write("\u0390\5\u0094K\2\u038d\u0390\5\u0090I\2\u038e\u0390\5")
+        buf.write("\u008eH\2\u038f\u0389\3\2\2\2\u038f\u038a\3\2\2\2\u038f")
+        buf.write("\u038b\3\2\2\2\u038f\u038c\3\2\2\2\u038f\u038d\3\2\2\2")
+        buf.write("\u038f\u038e\3\2\2\2\u0390\u008d\3\2\2\2\u0391\u0392\5")
+        buf.write("\u00d0i\2\u0392\u008f\3\2\2\2\u0393\u0394\t\b\2\2\u0394")
+        buf.write("\u0091\3\2\2\2\u0395\u03a7\7\36\2\2\u0396\u0397\7/\2\2")
+        buf.write("\u0397\u0398\5\66\34\2\u0398\u0399\7\60\2\2\u0399\u03a7")
+        buf.write("\3\2\2\2\u039a\u039b\7\22\2\2\u039b\u039e\7%\2\2\u039c")
+        buf.write("\u039e\7(\2\2\u039d\u039a\3\2\2\2\u039d\u039c\3\2\2\2")
+        buf.write("\u039e\u039f\3\2\2\2\u039f\u03a4\t\t\2\2\u03a0\u03a1\7")
+        buf.write("e\2\2\u03a1\u03a2\5:\36\2\u03a2\u03a3\7f\2\2\u03a3\u03a5")
+        buf.write("\3\2\2\2\u03a4\u03a0\3\2\2\2\u03a4\u03a5\3\2\2\2\u03a5")
+        buf.write("\u03a7\3\2\2\2\u03a6\u0395\3\2\2\2\u03a6\u0396\3\2\2\2")
+        buf.write("\u03a6\u039d\3\2\2\2\u03a7\u0093\3\2\2\2\u03a8\u03b6\7")
+        buf.write("\35\2\2\u03a9\u03aa\7\21\2\2\u03aa\u03ad\7%\2\2\u03ab")
+        buf.write("\u03ad\7'\2\2\u03ac\u03a9\3\2\2\2\u03ac\u03ab\3\2\2\2")
+        buf.write("\u03ad\u03ae\3\2\2\2\u03ae\u03b3\7n\2\2\u03af\u03b0\7")
+        buf.write("e\2\2\u03b0\u03b1\5:\36\2\u03b1\u03b2\7f\2\2\u03b2\u03b4")
+        buf.write("\3\2\2\2\u03b3\u03af\3\2\2\2\u03b3\u03b4\3\2\2\2\u03b4")
+        buf.write("\u03b6\3\2\2\2\u03b5\u03a8\3\2\2\2\u03b5\u03ac\3\2\2\2")
+        buf.write("\u03b6\u0095\3\2\2\2\u03b7\u03b8\7\16\2\2\u03b8\u03bb")
+        buf.write("\7%\2\2\u03b9\u03bb\7&\2\2\u03ba\u03b7\3\2\2\2\u03ba\u03b9")
+        buf.write("\3\2\2\2\u03bb\u03bc\3\2\2\2\u03bc\u03c1\7n\2\2\u03bd")
+        buf.write("\u03be\7e\2\2\u03be\u03bf\5:\36\2\u03bf\u03c0\7f\2\2\u03c0")
+        buf.write("\u03c2\3\2\2\2\u03c1\u03bd\3\2\2\2\u03c1\u03c2\3\2\2\2")
+        buf.write("\u03c2\u0097\3\2\2\2\u03c3\u03c5\5\u009aN\2\u03c4\u03c6")
+        buf.write("\5\u00caf\2\u03c5\u03c4\3\2\2\2\u03c5\u03c6\3\2\2\2\u03c6")
+        buf.write("\u03c8\3\2\2\2\u03c7\u03c9\5\u0098M\2\u03c8\u03c7\3\2")
+        buf.write("\2\2\u03c8\u03c9\3\2\2\2\u03c9\u03cf\3\2\2\2\u03ca\u03cc")
+        buf.write("\5\u00a2R\2\u03cb\u03cd\5\u0098M\2\u03cc\u03cb\3\2\2\2")
+        buf.write("\u03cc\u03cd\3\2\2\2\u03cd\u03cf\3\2\2\2\u03ce\u03c3\3")
+        buf.write("\2\2\2\u03ce\u03ca\3\2\2\2\u03cf\u0099\3\2\2\2\u03d0\u03d1")
+        buf.write("\7)\2\2\u03d1\u03d2\7n\2\2\u03d2\u009b\3\2\2\2\u03d3\u03d4")
+        buf.write("\7+\2\2\u03d4\u03d5\7n\2\2\u03d5\u009d\3\2\2\2\u03d6\u03d7")
+        buf.write("\7,\2\2\u03d7\u03d8\7n\2\2\u03d8\u009f\3\2\2\2\u03d9\u03da")
+        buf.write("\7-\2\2\u03da\u03db\7n\2\2\u03db\u00a1\3\2\2\2\u03dc\u03e0")
+        buf.write("\5\u00a4S\2\u03dd\u03e0\5\u00a6T\2\u03de\u03e0\5\u00a8")
+        buf.write("U\2\u03df\u03dc\3\2\2\2\u03df\u03dd\3\2\2\2\u03df\u03de")
+        buf.write("\3\2\2\2\u03e0\u00a3\3\2\2\2\u03e1\u03ed\7\4\2\2\u03e2")
+        buf.write("\u03e9\7`\2\2\u03e3\u03e4\7g\2\2\u03e4\u03e6\7n\2\2\u03e5")
+        buf.write("\u03e7\5\u00caf\2\u03e6\u03e5\3\2\2\2\u03e6\u03e7\3\2")
+        buf.write("\2\2\u03e7\u03e8\3\2\2\2\u03e8\u03ea\7h\2\2\u03e9\u03e3")
+        buf.write("\3\2\2\2\u03e9\u03ea\3\2\2\2\u03ea\u03eb\3\2\2\2\u03eb")
+        buf.write("\u03ed\7\5\2\2\u03ec\u03e1\3\2\2\2\u03ec\u03e2\3\2\2\2")
+        buf.write("\u03ed\u00a5\3\2\2\2\u03ee\u03fa\7\6\2\2\u03ef\u03f6\7")
+        buf.write("\7\2\2\u03f0\u03f1\7g\2\2\u03f1\u03f3\7n\2\2\u03f2\u03f4")
+        buf.write("\5\u00caf\2\u03f3\u03f2\3\2\2\2\u03f3\u03f4\3\2\2\2\u03f4")
+        buf.write("\u03f5\3\2\2\2\u03f5\u03f7\7h\2\2\u03f6\u03f0\3\2\2\2")
+        buf.write("\u03f6\u03f7\3\2\2\2\u03f7\u03f8\3\2\2\2\u03f8\u03fa\7")
+        buf.write("`\2\2\u03f9\u03ee\3\2\2\2\u03f9\u03ef\3\2\2\2\u03fa\u00a7")
+        buf.write("\3\2\2\2\u03fb\u0407\7\b\2\2\u03fc\u0403\7\7\2\2\u03fd")
+        buf.write("\u03fe\7g\2\2\u03fe\u0400\7n\2\2\u03ff\u0401\5\u00caf")
+        buf.write("\2\u0400\u03ff\3\2\2\2\u0400\u0401\3\2\2\2\u0401\u0402")
+        buf.write("\3\2\2\2\u0402\u0404\7h\2\2\u0403\u03fd\3\2\2\2\u0403")
+        buf.write("\u0404\3\2\2\2\u0404\u0405\3\2\2\2\u0405\u0407\7\5\2\2")
+        buf.write("\u0406\u03fb\3\2\2\2\u0406\u03fc\3\2\2\2\u0407\u00a9\3")
+        buf.write("\2\2\2\u0408\u040c\5\u00acW\2\u0409\u040c\5\u00aeX\2\u040a")
+        buf.write("\u040c\5\u00b0Y\2\u040b\u0408\3\2\2\2\u040b\u0409\3\2")
+        buf.write("\2\2\u040b\u040a\3\2\2\2\u040c\u00ab\3\2\2\2\u040d\u0419")
+        buf.write("\7\t\2\2\u040e\u0415\7_\2\2\u040f\u0410\7g\2\2\u0410\u0412")
+        buf.write("\7n\2\2\u0411\u0413\5\u00c8e\2\u0412\u0411\3\2\2\2\u0412")
+        buf.write("\u0413\3\2\2\2\u0413\u0414\3\2\2\2\u0414\u0416\7h\2\2")
+        buf.write("\u0415\u040f\3\2\2\2\u0415\u0416\3\2\2\2\u0416\u0417\3")
+        buf.write("\2\2\2\u0417\u0419\7\n\2\2\u0418\u040d\3\2\2\2\u0418\u040e")
+        buf.write("\3\2\2\2\u0419\u00ad\3\2\2\2\u041a\u0426\7\13\2\2\u041b")
+        buf.write("\u0422\7\f\2\2\u041c\u041d\7g\2\2\u041d\u041f\7n\2\2\u041e")
+        buf.write("\u0420\5\u00c8e\2\u041f\u041e\3\2\2\2\u041f\u0420\3\2")
+        buf.write("\2\2\u0420\u0421\3\2\2\2\u0421\u0423\7h\2\2\u0422\u041c")
+        buf.write("\3\2\2\2\u0422\u0423\3\2\2\2\u0423\u0424\3\2\2\2\u0424")
+        buf.write("\u0426\7_\2\2\u0425\u041a\3\2\2\2\u0425\u041b\3\2\2\2")
+        buf.write("\u0426\u00af\3\2\2\2\u0427\u0433\7\r\2\2\u0428\u042f\7")
+        buf.write("\f\2\2\u0429\u042a\7g\2\2\u042a\u042c\7n\2\2\u042b\u042d")
+        buf.write("\5\u00c8e\2\u042c\u042b\3\2\2\2\u042c\u042d\3\2\2\2\u042d")
+        buf.write("\u042e\3\2\2\2\u042e\u0430\7h\2\2\u042f\u0429\3\2\2\2")
+        buf.write("\u042f\u0430\3\2\2\2\u0430\u0431\3\2\2\2\u0431\u0433\7")
+        buf.write("\n\2\2\u0432\u0427\3\2\2\2\u0432\u0428\3\2\2\2\u0433\u00b1")
+        buf.write("\3\2\2\2\u0434\u0436\7g\2\2\u0435\u0437\5:\36\2\u0436")
+        buf.write("\u0435\3\2\2\2\u0436\u0437\3\2\2\2\u0437\u0438\3\2\2\2")
+        buf.write("\u0438\u0439\7h\2\2\u0439\u00b3\3\2\2\2\u043a\u043b\7")
+        buf.write("g\2\2\u043b\u043c\5d\63\2\u043c\u043d\7h\2\2\u043d\u0445")
+        buf.write("\3\2\2\2\u043e\u043f\7g\2\2\u043f\u0440\5d\63\2\u0440")
+        buf.write("\u0441\7$\2\2\u0441\u0442\5d\63\2\u0442\u0443\7h\2\2\u0443")
+        buf.write("\u0445\3\2\2\2\u0444\u043a\3\2\2\2\u0444\u043e\3\2\2\2")
+        buf.write("\u0445\u00b5\3\2\2\2\u0446\u044f\7/\2\2\u0447\u044c\5")
+        buf.write("\u00b8]\2\u0448\u0449\7]\2\2\u0449\u044b\5\u00b8]\2\u044a")
+        buf.write("\u0448\3\2\2\2\u044b\u044e\3\2\2\2\u044c\u044a\3\2\2\2")
+        buf.write("\u044c\u044d\3\2\2\2\u044d\u0450\3\2\2\2\u044e\u044c\3")
+        buf.write("\2\2\2\u044f\u0447\3\2\2\2\u044f\u0450\3\2\2\2\u0450\u0451")
+        buf.write("\3\2\2\2\u0451\u0452\7\60\2\2\u0452\u00b7\3\2\2\2\u0453")
+        buf.write("\u0454\5d\63\2\u0454\u0455\7$\2\2\u0455\u0456\5d\63\2")
+        buf.write("\u0456\u00b9\3\2\2\2\u0457\u0458\7\31\2\2\u0458\u0459")
+        buf.write("\5\u00bc_\2\u0459\u00bb\3\2\2\2\u045a\u045f\5\u00c0a\2")
+        buf.write("\u045b\u045f\5\u00c4c\2\u045c\u045f\5\u00c2b\2\u045d\u045f")
+        buf.write("\5\u00c6d\2\u045e\u045a\3\2\2\2\u045e\u045b\3\2\2\2\u045e")
+        buf.write("\u045c\3\2\2\2\u045e\u045d\3\2\2\2\u045f\u00bd\3\2\2\2")
+        buf.write("\u0460\u0461\5d\63\2\u0461\u0462\5\u00aaV\2\u0462\u00bf")
+        buf.write("\3\2\2\2\u0463\u0465\5\u00be`\2\u0464\u0463\3\2\2\2\u0464")
+        buf.write("\u0465\3\2\2\2\u0465\u0466\3\2\2\2\u0466\u0468\5\u009a")
+        buf.write("N\2\u0467\u0469\5\u00c8e\2\u0468\u0467\3\2\2\2\u0468\u0469")
+        buf.write("\3\2\2\2\u0469\u00c1\3\2\2\2\u046a\u046c\5\u00be`\2\u046b")
+        buf.write("\u046a\3\2\2\2\u046b\u046c\3\2\2\2\u046c\u046d\3\2\2\2")
+        buf.write("\u046d\u046e\5\u009eP\2\u046e\u00c3\3\2\2\2\u046f\u0471")
+        buf.write("\5d\63\2\u0470\u0472\7\64\2\2\u0471\u0470\3\2\2\2\u0471")
+        buf.write("\u0472\3\2\2\2\u0472\u0473\3\2\2\2\u0473\u0475\5\u009c")
+        buf.write("O\2\u0474\u0476\5\u00c8e\2\u0475\u0474\3\2\2\2\u0475\u0476")
+        buf.write("\3\2\2\2\u0476\u00c5\3\2\2\2\u0477\u0479\5\u00a0Q\2\u0478")
+        buf.write("\u047a\5\u00c8e\2\u0479\u0478\3\2\2\2\u0479\u047a\3\2")
+        buf.write("\2\2\u047a\u00c7\3\2\2\2\u047b\u0484\7e\2\2\u047c\u0481")
+        buf.write("\5\u00ccg\2\u047d\u047e\7]\2\2\u047e\u0480\5\u00ccg\2")
+        buf.write("\u047f\u047d\3\2\2\2\u0480\u0483\3\2\2\2\u0481\u047f\3")
+        buf.write("\2\2\2\u0481\u0482\3\2\2\2\u0482\u0485\3\2\2\2\u0483\u0481")
+        buf.write("\3\2\2\2\u0484\u047c\3\2\2\2\u0484\u0485\3\2\2\2\u0485")
+        buf.write("\u0486\3\2\2\2\u0486\u0487\7f\2\2\u0487\u00c9\3\2\2\2")
+        buf.write("\u0488\u0491\7e\2\2\u0489\u048e\5\u00ceh\2\u048a\u048b")
+        buf.write("\7]\2\2\u048b\u048d\5\u00ceh\2\u048c\u048a\3\2\2\2\u048d")
+        buf.write("\u0490\3\2\2\2\u048e\u048c\3\2\2\2\u048e\u048f\3\2\2\2")
+        buf.write("\u048f\u0492\3\2\2\2\u0490\u048e\3\2\2\2\u0491\u0489\3")
+        buf.write("\2\2\2\u0491\u0492\3\2\2\2\u0492\u0493\3\2\2\2\u0493\u0494")
+        buf.write("\7f\2\2\u0494\u00cb\3\2\2\2\u0495\u0496\7n\2\2\u0496\u0497")
+        buf.write("\78\2\2\u0497\u0498\5d\63\2\u0498\u00cd\3\2\2\2\u0499")
+        buf.write("\u049a\7n\2\2\u049a\u049b\5r:\2\u049b\u049c\5d\63\2\u049c")
+        buf.write("\u00cf\3\2\2\2\u049d\u049e\t\n\2\2\u049e\u00d1\3\2\2\2")
+        buf.write("\u049f\u04a1\7j\2\2\u04a0\u049f\3\2\2\2\u04a1\u04a2\3")
+        buf.write("\2\2\2\u04a2\u04a0\3\2\2\2\u04a2\u04a3\3\2\2\2\u04a3\u00d3")
+        buf.write("\3\2\2\2\u0093\u00d5\u00da\u00e0\u00e9\u00ef\u00f9\u00fd")
         buf.write("\u0102\u0106\u010b\u010f\u0114\u0118\u011e\u0122\u0127")
         buf.write("\u012b\u012d\u0134\u0139\u0145\u0150\u015a\u0165\u016a")
         buf.write("\u016d\u0173\u0177\u017b\u017d\u0181\u0187\u018e\u0193")
-        buf.write("\u0197\u019b\u01b0\u01b7\u01bb\u01c1\u01c8\u01cd\u01e0")
-        buf.write("\u01ed\u01f3\u01f6\u01fc\u0203\u020a\u020e\u0216\u0219")
-        buf.write("\u021d\u0223\u0228\u0233\u023c\u0243\u024f\u0256\u025c")
-        buf.write("\u0273\u027b\u027f\u0284\u028a\u0290\u0293\u02a8\u02ae")
-        buf.write("\u02c8\u02ce\u02d7\u02dc\u02e1\u02e8\u02ee\u02fd\u0301")
-        buf.write("\u0308\u0313\u0316\u0320\u032a\u0332\u0338\u033f\u0346")
-        buf.write("\u035a\u0362\u0368\u0372\u0378\u037a\u0380\u038e\u039c")
-        buf.write("\u03a3\u03a5\u03ab\u03b2\u03b4\u03b9\u03c0\u03c4\u03c7")
-        buf.write("\u03cb\u03cd\u03de\u03e5\u03e8\u03eb\u03f2\u03f5\u03f8")
-        buf.write("\u03ff\u0402\u0405\u040a\u0411\u0414\u0417\u041e\u0421")
-        buf.write("\u0424\u042b\u042e\u0431\u0435\u0443\u044b\u044e\u045d")
-        buf.write("\u0463\u0467\u046a\u0470\u0474\u0478\u0480\u0483\u048d")
-        buf.write("\u0490\u04a1")
+        buf.write("\u0197\u019b\u01b0\u01b7\u01bb\u01c1\u01c8\u01cd\u01de")
+        buf.write("\u01eb\u01f1\u01f4\u01fa\u0201\u0208\u020c\u0214\u0217")
+        buf.write("\u021b\u0221\u0226\u0231\u023a\u0241\u024d\u0254\u025a")
+        buf.write("\u0271\u0279\u027d\u0282\u0288\u028e\u0291\u02a6\u02ac")
+        buf.write("\u02c6\u02cc\u02d5\u02da\u02df\u02e6\u02ec\u02fb\u02ff")
+        buf.write("\u0306\u0311\u0314\u031e\u0328\u0330\u0336\u033d\u0344")
+        buf.write("\u0358\u0360\u0366\u036f\u0373\u0379\u037b\u0381\u038f")
+        buf.write("\u039d\u03a4\u03a6\u03ac\u03b3\u03b5\u03ba\u03c1\u03c5")
+        buf.write("\u03c8\u03cc\u03ce\u03df\u03e6\u03e9\u03ec\u03f3\u03f6")
+        buf.write("\u03f9\u0400\u0403\u0406\u040b\u0412\u0415\u0418\u041f")
+        buf.write("\u0422\u0425\u042c\u042f\u0432\u0436\u0444\u044c\u044f")
+        buf.write("\u045e\u0464\u0468\u046b\u0471\u0475\u0479\u0481\u0484")
+        buf.write("\u048e\u0491\u04a2")
         return buf.getvalue()
 
 
 class jacParser(Parser):
     grammarFileName = "jac.g4"
 
     atn = ATNDeserializer().deserialize(serializedATN())
@@ -851,61 +854,61 @@
     RULE_walk_exit_block = 12
     RULE_walk_activity_block = 13
     RULE_attr_block = 14
     RULE_attr_stmt = 15
     RULE_struct_block = 16
     RULE_can_block = 17
     RULE_graph_block = 18
-    RULE_graph_block_spawn = 19
-    RULE_has_root = 20
-    RULE_has_stmt = 21
-    RULE_has_assign = 22
-    RULE_can_stmt = 23
-    RULE_event_clause = 24
-    RULE_preset_in_out = 25
-    RULE_dotted_name = 26
-    RULE_name_list = 27
-    RULE_param_list = 28
-    RULE_expr_list = 29
-    RULE_kw_expr_list = 30
-    RULE_code_block = 31
-    RULE_node_ctx_block = 32
-    RULE_statement = 33
-    RULE_if_stmt = 34
-    RULE_try_stmt = 35
-    RULE_else_from_try = 36
-    RULE_elif_stmt = 37
-    RULE_else_stmt = 38
-    RULE_for_stmt = 39
-    RULE_while_stmt = 40
-    RULE_ctrl_stmt = 41
-    RULE_assert_stmt = 42
-    RULE_destroy_action = 43
-    RULE_report_action = 44
-    RULE_walker_action = 45
-    RULE_ignore_action = 46
-    RULE_take_action = 47
-    RULE_disengage_action = 48
-    RULE_yield_action = 49
-    RULE_expression = 50
-    RULE_assignment = 51
-    RULE_copy_assign = 52
-    RULE_inc_assign = 53
-    RULE_connect = 54
-    RULE_logical = 55
-    RULE_compare = 56
-    RULE_cmp_op = 57
-    RULE_nin = 58
-    RULE_arithmetic = 59
-    RULE_term = 60
-    RULE_factor = 61
-    RULE_power = 62
-    RULE_global_ref = 63
-    RULE_atom = 64
-    RULE_atom_trailer = 65
+    RULE_has_root = 19
+    RULE_has_stmt = 20
+    RULE_has_assign = 21
+    RULE_can_stmt = 22
+    RULE_event_clause = 23
+    RULE_preset_in_out = 24
+    RULE_dotted_name = 25
+    RULE_name_list = 26
+    RULE_param_list = 27
+    RULE_expr_list = 28
+    RULE_kw_expr_list = 29
+    RULE_code_block = 30
+    RULE_node_ctx_block = 31
+    RULE_statement = 32
+    RULE_if_stmt = 33
+    RULE_try_stmt = 34
+    RULE_else_from_try = 35
+    RULE_elif_stmt = 36
+    RULE_else_stmt = 37
+    RULE_for_stmt = 38
+    RULE_while_stmt = 39
+    RULE_ctrl_stmt = 40
+    RULE_assert_stmt = 41
+    RULE_destroy_action = 42
+    RULE_report_action = 43
+    RULE_walker_action = 44
+    RULE_ignore_action = 45
+    RULE_take_action = 46
+    RULE_disengage_action = 47
+    RULE_yield_action = 48
+    RULE_expression = 49
+    RULE_assignment = 50
+    RULE_copy_assign = 51
+    RULE_inc_assign = 52
+    RULE_connect = 53
+    RULE_logical = 54
+    RULE_compare = 55
+    RULE_cmp_op = 56
+    RULE_nin = 57
+    RULE_arithmetic = 58
+    RULE_term = 59
+    RULE_factor = 60
+    RULE_power = 61
+    RULE_global_ref = 62
+    RULE_atom = 63
+    RULE_atom_trailer = 64
+    RULE_ability_call = 65
     RULE_ability_op = 66
     RULE_ref = 67
     RULE_deref = 68
     RULE_built_in = 69
     RULE_cast_built_in = 70
     RULE_obj_built_in = 71
     RULE_dict_built_in = 72
@@ -958,15 +961,14 @@
         "walk_exit_block",
         "walk_activity_block",
         "attr_block",
         "attr_stmt",
         "struct_block",
         "can_block",
         "graph_block",
-        "graph_block_spawn",
         "has_root",
         "has_stmt",
         "has_assign",
         "can_stmt",
         "event_clause",
         "preset_in_out",
         "dotted_name",
@@ -1005,14 +1007,15 @@
         "arithmetic",
         "term",
         "factor",
         "power",
         "global_ref",
         "atom",
         "atom_trailer",
+        "ability_call",
         "ability_op",
         "ref",
         "deref",
         "built_in",
         "cast_built_in",
         "obj_built_in",
         "dict_built_in",
@@ -2824,52 +2827,14 @@
 
         def __init__(
             self, parser, parent: ParserRuleContext = None, invokingState: int = -1
         ):
             super().__init__(parent, invokingState)
             self.parser = parser
 
-        def graph_block_spawn(self):
-            return self.getTypedRuleContext(jacParser.Graph_block_spawnContext, 0)
-
-        def getRuleIndex(self):
-            return jacParser.RULE_graph_block
-
-        def enterRule(self, listener: ParseTreeListener):
-            if hasattr(listener, "enterGraph_block"):
-                listener.enterGraph_block(self)
-
-        def exitRule(self, listener: ParseTreeListener):
-            if hasattr(listener, "exitGraph_block"):
-                listener.exitGraph_block(self)
-
-    def graph_block(self):
-        localctx = jacParser.Graph_blockContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 36, self.RULE_graph_block)
-        try:
-            self.enterOuterAlt(localctx, 1)
-            self.state = 462
-            self.graph_block_spawn()
-        except RecognitionException as re:
-            localctx.exception = re
-            self._errHandler.reportError(self, re)
-            self._errHandler.recover(self, re)
-        finally:
-            self.exitRule()
-        return localctx
-
-    class Graph_block_spawnContext(ParserRuleContext):
-        __slots__ = "parser"
-
-        def __init__(
-            self, parser, parent: ParserRuleContext = None, invokingState: int = -1
-        ):
-            super().__init__(parent, invokingState)
-            self.parser = parser
-
         def LBRACE(self):
             return self.getToken(jacParser.LBRACE, 0)
 
         def has_root(self):
             return self.getTypedRuleContext(jacParser.Has_rootContext, 0)
 
         def can_block(self):
@@ -2887,59 +2852,59 @@
         def COLON(self):
             return self.getToken(jacParser.COLON, 0)
 
         def SEMI(self):
             return self.getToken(jacParser.SEMI, 0)
 
         def getRuleIndex(self):
-            return jacParser.RULE_graph_block_spawn
+            return jacParser.RULE_graph_block
 
         def enterRule(self, listener: ParseTreeListener):
-            if hasattr(listener, "enterGraph_block_spawn"):
-                listener.enterGraph_block_spawn(self)
+            if hasattr(listener, "enterGraph_block"):
+                listener.enterGraph_block(self)
 
         def exitRule(self, listener: ParseTreeListener):
-            if hasattr(listener, "exitGraph_block_spawn"):
-                listener.exitGraph_block_spawn(self)
+            if hasattr(listener, "exitGraph_block"):
+                listener.exitGraph_block(self)
 
-    def graph_block_spawn(self):
-        localctx = jacParser.Graph_block_spawnContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 38, self.RULE_graph_block_spawn)
+    def graph_block(self):
+        localctx = jacParser.Graph_blockContext(self, self._ctx, self.state)
+        self.enterRule(localctx, 36, self.RULE_graph_block)
         try:
-            self.state = 478
+            self.state = 476
             self._errHandler.sync(self)
             token = self._input.LA(1)
             if token in [jacParser.LBRACE]:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 464
+                self.state = 462
                 self.match(jacParser.LBRACE)
-                self.state = 465
+                self.state = 463
                 self.has_root()
-                self.state = 466
+                self.state = 464
                 self.can_block()
-                self.state = 467
+                self.state = 465
                 self.match(jacParser.KW_SPAWN)
-                self.state = 468
+                self.state = 466
                 self.code_block()
-                self.state = 469
+                self.state = 467
                 self.match(jacParser.RBRACE)
                 pass
             elif token in [jacParser.COLON]:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 471
+                self.state = 469
                 self.match(jacParser.COLON)
-                self.state = 472
+                self.state = 470
                 self.has_root()
-                self.state = 473
+                self.state = 471
                 self.can_block()
-                self.state = 474
+                self.state = 472
                 self.match(jacParser.KW_SPAWN)
-                self.state = 475
+                self.state = 473
                 self.code_block()
-                self.state = 476
+                self.state = 474
                 self.match(jacParser.SEMI)
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -2979,24 +2944,24 @@
 
         def exitRule(self, listener: ParseTreeListener):
             if hasattr(listener, "exitHas_root"):
                 listener.exitHas_root(self)
 
     def has_root(self):
         localctx = jacParser.Has_rootContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 40, self.RULE_has_root)
+        self.enterRule(localctx, 38, self.RULE_has_root)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 480
+            self.state = 478
             self.match(jacParser.KW_HAS)
-            self.state = 481
+            self.state = 479
             self.match(jacParser.KW_ANCHOR)
-            self.state = 482
+            self.state = 480
             self.match(jacParser.NAME)
-            self.state = 483
+            self.state = 481
             self.match(jacParser.SEMI)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -3038,35 +3003,35 @@
 
         def exitRule(self, listener: ParseTreeListener):
             if hasattr(listener, "exitHas_stmt"):
                 listener.exitHas_stmt(self)
 
     def has_stmt(self):
         localctx = jacParser.Has_stmtContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 42, self.RULE_has_stmt)
+        self.enterRule(localctx, 40, self.RULE_has_stmt)
         self._la = 0  # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 485
+            self.state = 483
             self.match(jacParser.KW_HAS)
-            self.state = 486
+            self.state = 484
             self.has_assign()
-            self.state = 491
+            self.state = 489
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             while _la == jacParser.COMMA:
-                self.state = 487
+                self.state = 485
                 self.match(jacParser.COMMA)
-                self.state = 488
+                self.state = 486
                 self.has_assign()
-                self.state = 493
+                self.state = 491
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
 
-            self.state = 494
+            self.state = 492
             self.match(jacParser.SEMI)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -3105,46 +3070,46 @@
 
         def exitRule(self, listener: ParseTreeListener):
             if hasattr(listener, "exitHas_assign"):
                 listener.exitHas_assign(self)
 
     def has_assign(self):
         localctx = jacParser.Has_assignContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 44, self.RULE_has_assign)
+        self.enterRule(localctx, 42, self.RULE_has_assign)
         self._la = 0  # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 497
+            self.state = 495
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             if _la == jacParser.KW_PRIVATE:
-                self.state = 496
+                self.state = 494
                 self.match(jacParser.KW_PRIVATE)
 
-            self.state = 500
+            self.state = 498
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             if _la == jacParser.KW_ANCHOR:
-                self.state = 499
+                self.state = 497
                 self.match(jacParser.KW_ANCHOR)
 
-            self.state = 506
+            self.state = 504
             self._errHandler.sync(self)
             la_ = self._interp.adaptivePredict(self._input, 46, self._ctx)
             if la_ == 1:
-                self.state = 502
+                self.state = 500
                 self.match(jacParser.NAME)
                 pass
 
             elif la_ == 2:
-                self.state = 503
+                self.state = 501
                 self.match(jacParser.NAME)
-                self.state = 504
+                self.state = 502
                 self.match(jacParser.EQ)
-                self.state = 505
+                self.state = 503
                 self.expression()
                 pass
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -3206,74 +3171,74 @@
 
         def exitRule(self, listener: ParseTreeListener):
             if hasattr(listener, "exitCan_stmt"):
                 listener.exitCan_stmt(self)
 
     def can_stmt(self):
         localctx = jacParser.Can_stmtContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 46, self.RULE_can_stmt)
+        self.enterRule(localctx, 44, self.RULE_can_stmt)
         self._la = 0  # Token type
         try:
-            self.state = 535
+            self.state = 533
             self._errHandler.sync(self)
             la_ = self._interp.adaptivePredict(self._input, 51, self._ctx)
             if la_ == 1:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 508
+                self.state = 506
                 self.match(jacParser.KW_CAN)
-                self.state = 509
+                self.state = 507
                 self.dotted_name()
-                self.state = 513
+                self.state = 511
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
                 if _la == jacParser.DBL_COLON:
-                    self.state = 510
+                    self.state = 508
                     self.preset_in_out()
-                    self.state = 511
+                    self.state = 509
                     self.event_clause()
 
-                self.state = 524
+                self.state = 522
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
                 while _la == jacParser.COMMA:
-                    self.state = 515
+                    self.state = 513
                     self.match(jacParser.COMMA)
-                    self.state = 516
+                    self.state = 514
                     self.dotted_name()
-                    self.state = 520
+                    self.state = 518
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
                     if _la == jacParser.DBL_COLON:
-                        self.state = 517
+                        self.state = 515
                         self.preset_in_out()
-                        self.state = 518
+                        self.state = 516
                         self.event_clause()
 
-                    self.state = 526
+                    self.state = 524
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
 
-                self.state = 527
+                self.state = 525
                 self.match(jacParser.SEMI)
                 pass
 
             elif la_ == 2:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 529
+                self.state = 527
                 self.match(jacParser.KW_CAN)
-                self.state = 530
+                self.state = 528
                 self.match(jacParser.NAME)
-                self.state = 532
+                self.state = 530
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
                 if _la == jacParser.KW_WITH:
-                    self.state = 531
+                    self.state = 529
                     self.event_clause()
 
-                self.state = 534
+                self.state = 532
                 self.code_block()
                 pass
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -3314,28 +3279,28 @@
 
         def exitRule(self, listener: ParseTreeListener):
             if hasattr(listener, "exitEvent_clause"):
                 listener.exitEvent_clause(self)
 
     def event_clause(self):
         localctx = jacParser.Event_clauseContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 48, self.RULE_event_clause)
+        self.enterRule(localctx, 46, self.RULE_event_clause)
         self._la = 0  # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 537
+            self.state = 535
             self.match(jacParser.KW_WITH)
-            self.state = 539
+            self.state = 537
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             if _la == jacParser.NAME:
-                self.state = 538
+                self.state = 536
                 self.name_list()
 
-            self.state = 541
+            self.state = 539
             _la = self._input.LA(1)
             if not (
                 (
                     ((_la) & ~0x3F) == 0
                     and (
                         (1 << _la)
                         & (
@@ -3392,37 +3357,37 @@
 
         def exitRule(self, listener: ParseTreeListener):
             if hasattr(listener, "exitPreset_in_out"):
                 listener.exitPreset_in_out(self)
 
     def preset_in_out(self):
         localctx = jacParser.Preset_in_outContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 50, self.RULE_preset_in_out)
+        self.enterRule(localctx, 48, self.RULE_preset_in_out)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 543
+            self.state = 541
             self.match(jacParser.DBL_COLON)
-            self.state = 545
+            self.state = 543
             self._errHandler.sync(self)
             la_ = self._interp.adaptivePredict(self._input, 53, self._ctx)
             if la_ == 1:
-                self.state = 544
+                self.state = 542
                 self.param_list()
 
-            self.state = 550
+            self.state = 548
             self._errHandler.sync(self)
             token = self._input.LA(1)
             if token in [jacParser.DBL_COLON]:
-                self.state = 547
+                self.state = 545
                 self.match(jacParser.DBL_COLON)
                 pass
             elif token in [jacParser.COLON_OUT]:
-                self.state = 548
+                self.state = 546
                 self.match(jacParser.COLON_OUT)
-                self.state = 549
+                self.state = 547
                 self.expression()
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -3459,22 +3424,22 @@
 
         def exitRule(self, listener: ParseTreeListener):
             if hasattr(listener, "exitDotted_name"):
                 listener.exitDotted_name(self)
 
     def dotted_name(self):
         localctx = jacParser.Dotted_nameContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 52, self.RULE_dotted_name)
+        self.enterRule(localctx, 50, self.RULE_dotted_name)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 552
+            self.state = 550
             self.match(jacParser.NAME)
-            self.state = 553
+            self.state = 551
             self.match(jacParser.DOT)
-            self.state = 554
+            self.state = 552
             self.match(jacParser.NAME)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -3510,29 +3475,29 @@
 
         def exitRule(self, listener: ParseTreeListener):
             if hasattr(listener, "exitName_list"):
                 listener.exitName_list(self)
 
     def name_list(self):
         localctx = jacParser.Name_listContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 54, self.RULE_name_list)
+        self.enterRule(localctx, 52, self.RULE_name_list)
         self._la = 0  # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 556
+            self.state = 554
             self.match(jacParser.NAME)
-            self.state = 561
+            self.state = 559
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             while _la == jacParser.COMMA:
-                self.state = 557
+                self.state = 555
                 self.match(jacParser.COMMA)
-                self.state = 558
+                self.state = 556
                 self.match(jacParser.NAME)
-                self.state = 563
+                self.state = 561
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -3567,38 +3532,38 @@
 
         def exitRule(self, listener: ParseTreeListener):
             if hasattr(listener, "exitParam_list"):
                 listener.exitParam_list(self)
 
     def param_list(self):
         localctx = jacParser.Param_listContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 56, self.RULE_param_list)
+        self.enterRule(localctx, 54, self.RULE_param_list)
         try:
-            self.state = 570
+            self.state = 568
             self._errHandler.sync(self)
             la_ = self._interp.adaptivePredict(self._input, 56, self._ctx)
             if la_ == 1:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 564
+                self.state = 562
                 self.expr_list()
                 pass
 
             elif la_ == 2:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 565
+                self.state = 563
                 self.kw_expr_list()
                 pass
 
             elif la_ == 3:
                 self.enterOuterAlt(localctx, 3)
-                self.state = 566
+                self.state = 564
                 self.expr_list()
-                self.state = 567
+                self.state = 565
                 self.match(jacParser.COMMA)
-                self.state = 568
+                self.state = 566
                 self.kw_expr_list()
                 pass
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -3636,29 +3601,29 @@
 
         def exitRule(self, listener: ParseTreeListener):
             if hasattr(listener, "exitExpr_list"):
                 listener.exitExpr_list(self)
 
     def expr_list(self):
         localctx = jacParser.Expr_listContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 58, self.RULE_expr_list)
+        self.enterRule(localctx, 56, self.RULE_expr_list)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 572
+            self.state = 570
             self.connect()
-            self.state = 577
+            self.state = 575
             self._errHandler.sync(self)
             _alt = self._interp.adaptivePredict(self._input, 57, self._ctx)
             while _alt != 2 and _alt != ATN.INVALID_ALT_NUMBER:
                 if _alt == 1:
-                    self.state = 573
+                    self.state = 571
                     self.match(jacParser.COMMA)
-                    self.state = 574
+                    self.state = 572
                     self.connect()
-                self.state = 579
+                self.state = 577
                 self._errHandler.sync(self)
                 _alt = self._interp.adaptivePredict(self._input, 57, self._ctx)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -3708,37 +3673,37 @@
 
         def exitRule(self, listener: ParseTreeListener):
             if hasattr(listener, "exitKw_expr_list"):
                 listener.exitKw_expr_list(self)
 
     def kw_expr_list(self):
         localctx = jacParser.Kw_expr_listContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 60, self.RULE_kw_expr_list)
+        self.enterRule(localctx, 58, self.RULE_kw_expr_list)
         self._la = 0  # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 580
+            self.state = 578
             self.match(jacParser.NAME)
-            self.state = 581
+            self.state = 579
             self.match(jacParser.EQ)
-            self.state = 582
+            self.state = 580
             self.connect()
-            self.state = 589
+            self.state = 587
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             while _la == jacParser.COMMA:
-                self.state = 583
+                self.state = 581
                 self.match(jacParser.COMMA)
-                self.state = 584
+                self.state = 582
                 self.match(jacParser.NAME)
-                self.state = 585
+                self.state = 583
                 self.match(jacParser.EQ)
-                self.state = 586
+                self.state = 584
                 self.connect()
-                self.state = 591
+                self.state = 589
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -3779,25 +3744,25 @@
 
         def exitRule(self, listener: ParseTreeListener):
             if hasattr(listener, "exitCode_block"):
                 listener.exitCode_block(self)
 
     def code_block(self):
         localctx = jacParser.Code_blockContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 62, self.RULE_code_block)
+        self.enterRule(localctx, 60, self.RULE_code_block)
         self._la = 0  # Token type
         try:
-            self.state = 602
+            self.state = 600
             self._errHandler.sync(self)
             token = self._input.LA(1)
             if token in [jacParser.LBRACE]:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 592
+                self.state = 590
                 self.match(jacParser.LBRACE)
-                self.state = 596
+                self.state = 594
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
                 while (
                     ((_la) & ~0x3F) == 0
                     and (
                         (1 << _la)
                         & (
@@ -3856,28 +3821,28 @@
                             | (1 << (jacParser.INT - 65))
                             | (1 << (jacParser.NULL - 65))
                             | (1 << (jacParser.NAME - 65))
                         )
                     )
                     != 0
                 ):
-                    self.state = 593
+                    self.state = 591
                     self.statement()
-                    self.state = 598
+                    self.state = 596
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
 
-                self.state = 599
+                self.state = 597
                 self.match(jacParser.RBRACE)
                 pass
             elif token in [jacParser.COLON]:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 600
+                self.state = 598
                 self.match(jacParser.COLON)
-                self.state = 601
+                self.state = 599
                 self.statement()
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -3911,20 +3876,20 @@
 
         def exitRule(self, listener: ParseTreeListener):
             if hasattr(listener, "exitNode_ctx_block"):
                 listener.exitNode_ctx_block(self)
 
     def node_ctx_block(self):
         localctx = jacParser.Node_ctx_blockContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 64, self.RULE_node_ctx_block)
+        self.enterRule(localctx, 62, self.RULE_node_ctx_block)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 604
+            self.state = 602
             self.name_list()
-            self.state = 605
+            self.state = 603
             self.code_block()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -3987,94 +3952,94 @@
 
         def exitRule(self, listener: ParseTreeListener):
             if hasattr(listener, "exitStatement"):
                 listener.exitStatement(self)
 
     def statement(self):
         localctx = jacParser.StatementContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 66, self.RULE_statement)
+        self.enterRule(localctx, 64, self.RULE_statement)
         try:
-            self.state = 625
+            self.state = 623
             self._errHandler.sync(self)
             la_ = self._interp.adaptivePredict(self._input, 61, self._ctx)
             if la_ == 1:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 607
+                self.state = 605
                 self.code_block()
                 pass
 
             elif la_ == 2:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 608
+                self.state = 606
                 self.node_ctx_block()
                 pass
 
             elif la_ == 3:
                 self.enterOuterAlt(localctx, 3)
-                self.state = 609
+                self.state = 607
                 self.expression()
-                self.state = 610
+                self.state = 608
                 self.match(jacParser.SEMI)
                 pass
 
             elif la_ == 4:
                 self.enterOuterAlt(localctx, 4)
-                self.state = 612
+                self.state = 610
                 self.if_stmt()
                 pass
 
             elif la_ == 5:
                 self.enterOuterAlt(localctx, 5)
-                self.state = 613
+                self.state = 611
                 self.try_stmt()
                 pass
 
             elif la_ == 6:
                 self.enterOuterAlt(localctx, 6)
-                self.state = 614
+                self.state = 612
                 self.for_stmt()
                 pass
 
             elif la_ == 7:
                 self.enterOuterAlt(localctx, 7)
-                self.state = 615
+                self.state = 613
                 self.while_stmt()
                 pass
 
             elif la_ == 8:
                 self.enterOuterAlt(localctx, 8)
-                self.state = 616
+                self.state = 614
                 self.assert_stmt()
-                self.state = 617
+                self.state = 615
                 self.match(jacParser.SEMI)
                 pass
 
             elif la_ == 9:
                 self.enterOuterAlt(localctx, 9)
-                self.state = 619
+                self.state = 617
                 self.ctrl_stmt()
-                self.state = 620
+                self.state = 618
                 self.match(jacParser.SEMI)
                 pass
 
             elif la_ == 10:
                 self.enterOuterAlt(localctx, 10)
-                self.state = 622
+                self.state = 620
                 self.destroy_action()
                 pass
 
             elif la_ == 11:
                 self.enterOuterAlt(localctx, 11)
-                self.state = 623
+                self.state = 621
                 self.report_action()
                 pass
 
             elif la_ == 12:
                 self.enterOuterAlt(localctx, 12)
-                self.state = 624
+                self.state = 622
                 self.walker_action()
                 pass
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -4118,39 +4083,39 @@
 
         def exitRule(self, listener: ParseTreeListener):
             if hasattr(listener, "exitIf_stmt"):
                 listener.exitIf_stmt(self)
 
     def if_stmt(self):
         localctx = jacParser.If_stmtContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 68, self.RULE_if_stmt)
+        self.enterRule(localctx, 66, self.RULE_if_stmt)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 627
+            self.state = 625
             self.match(jacParser.KW_IF)
-            self.state = 628
+            self.state = 626
             self.expression()
-            self.state = 629
+            self.state = 627
             self.code_block()
-            self.state = 633
+            self.state = 631
             self._errHandler.sync(self)
             _alt = self._interp.adaptivePredict(self._input, 62, self._ctx)
             while _alt != 2 and _alt != ATN.INVALID_ALT_NUMBER:
                 if _alt == 1:
-                    self.state = 630
+                    self.state = 628
                     self.elif_stmt()
-                self.state = 635
+                self.state = 633
                 self._errHandler.sync(self)
                 _alt = self._interp.adaptivePredict(self._input, 62, self._ctx)
 
-            self.state = 637
+            self.state = 635
             self._errHandler.sync(self)
             la_ = self._interp.adaptivePredict(self._input, 63, self._ctx)
             if la_ == 1:
-                self.state = 636
+                self.state = 634
                 self.else_stmt()
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
@@ -4184,26 +4149,26 @@
 
         def exitRule(self, listener: ParseTreeListener):
             if hasattr(listener, "exitTry_stmt"):
                 listener.exitTry_stmt(self)
 
     def try_stmt(self):
         localctx = jacParser.Try_stmtContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 70, self.RULE_try_stmt)
+        self.enterRule(localctx, 68, self.RULE_try_stmt)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 639
+            self.state = 637
             self.match(jacParser.KW_TRY)
-            self.state = 640
+            self.state = 638
             self.code_block()
-            self.state = 642
+            self.state = 640
             self._errHandler.sync(self)
             la_ = self._interp.adaptivePredict(self._input, 64, self._ctx)
             if la_ == 1:
-                self.state = 641
+                self.state = 639
                 self.else_from_try()
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
@@ -4246,53 +4211,53 @@
 
         def exitRule(self, listener: ParseTreeListener):
             if hasattr(listener, "exitElse_from_try"):
                 listener.exitElse_from_try(self)
 
     def else_from_try(self):
         localctx = jacParser.Else_from_tryContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 72, self.RULE_else_from_try)
+        self.enterRule(localctx, 70, self.RULE_else_from_try)
         self._la = 0  # Token type
         try:
-            self.state = 657
+            self.state = 655
             self._errHandler.sync(self)
             la_ = self._interp.adaptivePredict(self._input, 67, self._ctx)
             if la_ == 1:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 644
+                self.state = 642
                 self.match(jacParser.KW_ELSE)
-                self.state = 648
+                self.state = 646
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
                 if _la == jacParser.LPAREN:
-                    self.state = 645
+                    self.state = 643
                     self.match(jacParser.LPAREN)
-                    self.state = 646
+                    self.state = 644
                     self.match(jacParser.NAME)
-                    self.state = 647
+                    self.state = 645
                     self.match(jacParser.RPAREN)
 
-                self.state = 650
+                self.state = 648
                 self.code_block()
                 pass
 
             elif la_ == 2:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 651
+                self.state = 649
                 self.match(jacParser.KW_ELSE)
-                self.state = 654
+                self.state = 652
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
                 if _la == jacParser.KW_WITH:
-                    self.state = 652
+                    self.state = 650
                     self.match(jacParser.KW_WITH)
-                    self.state = 653
+                    self.state = 651
                     self.match(jacParser.NAME)
 
-                self.state = 656
+                self.state = 654
                 self.code_block()
                 pass
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -4327,22 +4292,22 @@
 
         def exitRule(self, listener: ParseTreeListener):
             if hasattr(listener, "exitElif_stmt"):
                 listener.exitElif_stmt(self)
 
     def elif_stmt(self):
         localctx = jacParser.Elif_stmtContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 74, self.RULE_elif_stmt)
+        self.enterRule(localctx, 72, self.RULE_elif_stmt)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 659
+            self.state = 657
             self.match(jacParser.KW_ELIF)
-            self.state = 660
+            self.state = 658
             self.expression()
-            self.state = 661
+            self.state = 659
             self.code_block()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -4372,20 +4337,20 @@
 
         def exitRule(self, listener: ParseTreeListener):
             if hasattr(listener, "exitElse_stmt"):
                 listener.exitElse_stmt(self)
 
     def else_stmt(self):
         localctx = jacParser.Else_stmtContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 76, self.RULE_else_stmt)
+        self.enterRule(localctx, 74, self.RULE_else_stmt)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 663
+            self.state = 661
             self.match(jacParser.KW_ELSE)
-            self.state = 664
+            self.state = 662
             self.code_block()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -4439,58 +4404,58 @@
 
         def exitRule(self, listener: ParseTreeListener):
             if hasattr(listener, "exitFor_stmt"):
                 listener.exitFor_stmt(self)
 
     def for_stmt(self):
         localctx = jacParser.For_stmtContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 78, self.RULE_for_stmt)
+        self.enterRule(localctx, 76, self.RULE_for_stmt)
         self._la = 0  # Token type
         try:
-            self.state = 684
+            self.state = 682
             self._errHandler.sync(self)
             la_ = self._interp.adaptivePredict(self._input, 69, self._ctx)
             if la_ == 1:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 666
+                self.state = 664
                 self.match(jacParser.KW_FOR)
+                self.state = 665
+                self.expression()
+                self.state = 666
+                self.match(jacParser.KW_TO)
                 self.state = 667
                 self.expression()
                 self.state = 668
-                self.match(jacParser.KW_TO)
+                self.match(jacParser.KW_BY)
                 self.state = 669
                 self.expression()
                 self.state = 670
-                self.match(jacParser.KW_BY)
-                self.state = 671
-                self.expression()
-                self.state = 672
                 self.code_block()
                 pass
 
             elif la_ == 2:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 674
+                self.state = 672
                 self.match(jacParser.KW_FOR)
-                self.state = 675
+                self.state = 673
                 self.match(jacParser.NAME)
-                self.state = 678
+                self.state = 676
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
                 if _la == jacParser.COMMA:
-                    self.state = 676
+                    self.state = 674
                     self.match(jacParser.COMMA)
-                    self.state = 677
+                    self.state = 675
                     self.match(jacParser.NAME)
 
-                self.state = 680
+                self.state = 678
                 self.match(jacParser.KW_IN)
-                self.state = 681
+                self.state = 679
                 self.expression()
-                self.state = 682
+                self.state = 680
                 self.code_block()
                 pass
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -4525,22 +4490,22 @@
 
         def exitRule(self, listener: ParseTreeListener):
             if hasattr(listener, "exitWhile_stmt"):
                 listener.exitWhile_stmt(self)
 
     def while_stmt(self):
         localctx = jacParser.While_stmtContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 80, self.RULE_while_stmt)
+        self.enterRule(localctx, 78, self.RULE_while_stmt)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 686
+            self.state = 684
             self.match(jacParser.KW_WHILE)
-            self.state = 687
+            self.state = 685
             self.expression()
-            self.state = 688
+            self.state = 686
             self.code_block()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -4573,19 +4538,19 @@
 
         def exitRule(self, listener: ParseTreeListener):
             if hasattr(listener, "exitCtrl_stmt"):
                 listener.exitCtrl_stmt(self)
 
     def ctrl_stmt(self):
         localctx = jacParser.Ctrl_stmtContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 82, self.RULE_ctrl_stmt)
+        self.enterRule(localctx, 80, self.RULE_ctrl_stmt)
         self._la = 0  # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 690
+            self.state = 688
             _la = self._input.LA(1)
             if not (
                 (
                     (((_la - 69)) & ~0x3F) == 0
                     and (
                         (1 << (_la - 69))
                         & (
@@ -4633,20 +4598,20 @@
 
         def exitRule(self, listener: ParseTreeListener):
             if hasattr(listener, "exitAssert_stmt"):
                 listener.exitAssert_stmt(self)
 
     def assert_stmt(self):
         localctx = jacParser.Assert_stmtContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 84, self.RULE_assert_stmt)
+        self.enterRule(localctx, 82, self.RULE_assert_stmt)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 692
+            self.state = 690
             self.match(jacParser.KW_ASSERT)
-            self.state = 693
+            self.state = 691
             self.expression()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -4679,22 +4644,22 @@
 
         def exitRule(self, listener: ParseTreeListener):
             if hasattr(listener, "exitDestroy_action"):
                 listener.exitDestroy_action(self)
 
     def destroy_action(self):
         localctx = jacParser.Destroy_actionContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 86, self.RULE_destroy_action)
+        self.enterRule(localctx, 84, self.RULE_destroy_action)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 695
+            self.state = 693
             self.match(jacParser.KW_DESTROY)
-            self.state = 696
+            self.state = 694
             self.expression()
-            self.state = 697
+            self.state = 695
             self.match(jacParser.SEMI)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -4736,42 +4701,42 @@
 
         def exitRule(self, listener: ParseTreeListener):
             if hasattr(listener, "exitReport_action"):
                 listener.exitReport_action(self)
 
     def report_action(self):
         localctx = jacParser.Report_actionContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 88, self.RULE_report_action)
+        self.enterRule(localctx, 86, self.RULE_report_action)
         try:
-            self.state = 710
+            self.state = 708
             self._errHandler.sync(self)
             la_ = self._interp.adaptivePredict(self._input, 70, self._ctx)
             if la_ == 1:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 699
+                self.state = 697
                 self.match(jacParser.KW_REPORT)
-                self.state = 700
+                self.state = 698
                 self.expression()
-                self.state = 701
+                self.state = 699
                 self.match(jacParser.SEMI)
                 pass
 
             elif la_ == 2:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 703
+                self.state = 701
                 self.match(jacParser.KW_REPORT)
-                self.state = 704
+                self.state = 702
                 self.match(jacParser.COLON)
-                self.state = 705
+                self.state = 703
                 self.match(jacParser.NAME)
-                self.state = 706
+                self.state = 704
                 self.match(jacParser.EQ)
-                self.state = 707
+                self.state = 705
                 self.expression()
-                self.state = 708
+                self.state = 706
                 self.match(jacParser.SEMI)
                 pass
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -4809,37 +4774,37 @@
 
         def exitRule(self, listener: ParseTreeListener):
             if hasattr(listener, "exitWalker_action"):
                 listener.exitWalker_action(self)
 
     def walker_action(self):
         localctx = jacParser.Walker_actionContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 90, self.RULE_walker_action)
+        self.enterRule(localctx, 88, self.RULE_walker_action)
         try:
-            self.state = 716
+            self.state = 714
             self._errHandler.sync(self)
             token = self._input.LA(1)
             if token in [jacParser.KW_IGNORE]:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 712
+                self.state = 710
                 self.ignore_action()
                 pass
             elif token in [jacParser.KW_TAKE]:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 713
+                self.state = 711
                 self.take_action()
                 pass
             elif token in [jacParser.KW_DISENGAGE]:
                 self.enterOuterAlt(localctx, 3)
-                self.state = 714
+                self.state = 712
                 self.disengage_action()
                 pass
             elif token in [jacParser.KW_YIELD]:
                 self.enterOuterAlt(localctx, 4)
-                self.state = 715
+                self.state = 713
                 self.yield_action()
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -4876,22 +4841,22 @@
 
         def exitRule(self, listener: ParseTreeListener):
             if hasattr(listener, "exitIgnore_action"):
                 listener.exitIgnore_action(self)
 
     def ignore_action(self):
         localctx = jacParser.Ignore_actionContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 92, self.RULE_ignore_action)
+        self.enterRule(localctx, 90, self.RULE_ignore_action)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 718
+            self.state = 716
             self.match(jacParser.KW_IGNORE)
-            self.state = 719
+            self.state = 717
             self.expression()
-            self.state = 720
+            self.state = 718
             self.match(jacParser.SEMI)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -4933,40 +4898,40 @@
 
         def exitRule(self, listener: ParseTreeListener):
             if hasattr(listener, "exitTake_action"):
                 listener.exitTake_action(self)
 
     def take_action(self):
         localctx = jacParser.Take_actionContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 94, self.RULE_take_action)
+        self.enterRule(localctx, 92, self.RULE_take_action)
         self._la = 0  # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 722
+            self.state = 720
             self.match(jacParser.KW_TAKE)
-            self.state = 725
+            self.state = 723
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             if _la == jacParser.COLON:
-                self.state = 723
+                self.state = 721
                 self.match(jacParser.COLON)
-                self.state = 724
+                self.state = 722
                 self.match(jacParser.NAME)
 
-            self.state = 727
+            self.state = 725
             self.expression()
-            self.state = 730
+            self.state = 728
             self._errHandler.sync(self)
             token = self._input.LA(1)
             if token in [jacParser.SEMI]:
-                self.state = 728
+                self.state = 726
                 self.match(jacParser.SEMI)
                 pass
             elif token in [jacParser.KW_ELSE]:
-                self.state = 729
+                self.state = 727
                 self.else_stmt()
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -5003,28 +4968,28 @@
 
         def exitRule(self, listener: ParseTreeListener):
             if hasattr(listener, "exitDisengage_action"):
                 listener.exitDisengage_action(self)
 
     def disengage_action(self):
         localctx = jacParser.Disengage_actionContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 96, self.RULE_disengage_action)
+        self.enterRule(localctx, 94, self.RULE_disengage_action)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 732
+            self.state = 730
             self.match(jacParser.KW_DISENGAGE)
-            self.state = 735
+            self.state = 733
             self._errHandler.sync(self)
             token = self._input.LA(1)
             if token in [jacParser.KW_REPORT]:
-                self.state = 733
+                self.state = 731
                 self.report_action()
                 pass
             elif token in [jacParser.SEMI]:
-                self.state = 734
+                self.state = 732
                 self.match(jacParser.SEMI)
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -5067,36 +5032,36 @@
 
         def exitRule(self, listener: ParseTreeListener):
             if hasattr(listener, "exitYield_action"):
                 listener.exitYield_action(self)
 
     def yield_action(self):
         localctx = jacParser.Yield_actionContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 98, self.RULE_yield_action)
+        self.enterRule(localctx, 96, self.RULE_yield_action)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 737
+            self.state = 735
             self.match(jacParser.KW_YIELD)
-            self.state = 742
+            self.state = 740
             self._errHandler.sync(self)
             token = self._input.LA(1)
             if token in [jacParser.KW_REPORT]:
-                self.state = 738
+                self.state = 736
                 self.report_action()
                 pass
             elif token in [jacParser.KW_DISENGAGE]:
-                self.state = 739
+                self.state = 737
                 self.disengage_action()
                 pass
             elif token in [jacParser.KW_TAKE]:
-                self.state = 740
+                self.state = 738
                 self.take_action()
                 pass
             elif token in [jacParser.SEMI]:
-                self.state = 741
+                self.state = 739
                 self.match(jacParser.SEMI)
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -5136,32 +5101,32 @@
 
         def exitRule(self, listener: ParseTreeListener):
             if hasattr(listener, "exitExpression"):
                 listener.exitExpression(self)
 
     def expression(self):
         localctx = jacParser.ExpressionContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 100, self.RULE_expression)
+        self.enterRule(localctx, 98, self.RULE_expression)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 744
+            self.state = 742
             self.connect()
-            self.state = 748
+            self.state = 746
             self._errHandler.sync(self)
             la_ = self._interp.adaptivePredict(self._input, 76, self._ctx)
             if la_ == 1:
-                self.state = 745
+                self.state = 743
                 self.assignment()
 
             elif la_ == 2:
-                self.state = 746
+                self.state = 744
                 self.copy_assign()
 
             elif la_ == 3:
-                self.state = 747
+                self.state = 745
                 self.inc_assign()
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
@@ -5192,20 +5157,20 @@
 
         def exitRule(self, listener: ParseTreeListener):
             if hasattr(listener, "exitAssignment"):
                 listener.exitAssignment(self)
 
     def assignment(self):
         localctx = jacParser.AssignmentContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 102, self.RULE_assignment)
+        self.enterRule(localctx, 100, self.RULE_assignment)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 750
+            self.state = 748
             self.match(jacParser.EQ)
-            self.state = 751
+            self.state = 749
             self.expression()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -5235,20 +5200,20 @@
 
         def exitRule(self, listener: ParseTreeListener):
             if hasattr(listener, "exitCopy_assign"):
                 listener.exitCopy_assign(self)
 
     def copy_assign(self):
         localctx = jacParser.Copy_assignContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 104, self.RULE_copy_assign)
+        self.enterRule(localctx, 102, self.RULE_copy_assign)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 753
+            self.state = 751
             self.match(jacParser.CPY_EQ)
-            self.state = 754
+            self.state = 752
             self.expression()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -5287,19 +5252,19 @@
 
         def exitRule(self, listener: ParseTreeListener):
             if hasattr(listener, "exitInc_assign"):
                 listener.exitInc_assign(self)
 
     def inc_assign(self):
         localctx = jacParser.Inc_assignContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 106, self.RULE_inc_assign)
+        self.enterRule(localctx, 104, self.RULE_inc_assign)
         self._la = 0  # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 756
+            self.state = 754
             _la = self._input.LA(1)
             if not (
                 (
                     ((_la) & ~0x3F) == 0
                     and (
                         (1 << _la)
                         & (
@@ -5312,15 +5277,15 @@
                     != 0
                 )
             ):
                 self._errHandler.recoverInline(self)
             else:
                 self._errHandler.reportMatch(self)
                 self.consume()
-            self.state = 757
+            self.state = 755
             self.expression()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -5359,46 +5324,46 @@
 
         def exitRule(self, listener: ParseTreeListener):
             if hasattr(listener, "exitConnect"):
                 listener.exitConnect(self)
 
     def connect(self):
         localctx = jacParser.ConnectContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 108, self.RULE_connect)
+        self.enterRule(localctx, 106, self.RULE_connect)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 759
+            self.state = 757
             self.logical()
-            self.state = 767
+            self.state = 765
             self._errHandler.sync(self)
             la_ = self._interp.adaptivePredict(self._input, 78, self._ctx)
             if la_ == 1:
-                self.state = 763
+                self.state = 761
                 self._errHandler.sync(self)
                 token = self._input.LA(1)
                 if token in [jacParser.NOT]:
-                    self.state = 760
+                    self.state = 758
                     self.match(jacParser.NOT)
-                    self.state = 761
+                    self.state = 759
                     self.edge_ref()
                     pass
                 elif token in [
                     jacParser.T__6,
                     jacParser.T__8,
                     jacParser.T__9,
                     jacParser.T__10,
                     jacParser.PLUS,
                 ]:
-                    self.state = 762
+                    self.state = 760
                     self.connect_op()
                     pass
                 else:
                     raise NoViableAltException(self)
 
-                self.state = 765
+                self.state = 763
                 self.expression()
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
@@ -5441,34 +5406,34 @@
 
         def exitRule(self, listener: ParseTreeListener):
             if hasattr(listener, "exitLogical"):
                 listener.exitLogical(self)
 
     def logical(self):
         localctx = jacParser.LogicalContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 110, self.RULE_logical)
+        self.enterRule(localctx, 108, self.RULE_logical)
         self._la = 0  # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 769
+            self.state = 767
             self.compare()
-            self.state = 774
+            self.state = 772
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             while _la == jacParser.KW_AND or _la == jacParser.KW_OR:
-                self.state = 770
+                self.state = 768
                 _la = self._input.LA(1)
                 if not (_la == jacParser.KW_AND or _la == jacParser.KW_OR):
                     self._errHandler.recoverInline(self)
                 else:
                     self._errHandler.reportMatch(self)
                     self.consume()
-                self.state = 771
+                self.state = 769
                 self.compare()
-                self.state = 776
+                self.state = 774
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -5512,24 +5477,24 @@
 
         def exitRule(self, listener: ParseTreeListener):
             if hasattr(listener, "exitCompare"):
                 listener.exitCompare(self)
 
     def compare(self):
         localctx = jacParser.CompareContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 112, self.RULE_compare)
+        self.enterRule(localctx, 110, self.RULE_compare)
         try:
-            self.state = 788
+            self.state = 786
             self._errHandler.sync(self)
             token = self._input.LA(1)
             if token in [jacParser.NOT]:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 777
+                self.state = 775
                 self.match(jacParser.NOT)
-                self.state = 778
+                self.state = 776
                 self.compare()
                 pass
             elif token in [
                 jacParser.T__1,
                 jacParser.T__3,
                 jacParser.T__4,
                 jacParser.T__5,
@@ -5558,26 +5523,26 @@
                 jacParser.STRING,
                 jacParser.BOOL,
                 jacParser.INT,
                 jacParser.NULL,
                 jacParser.NAME,
             ]:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 779
+                self.state = 777
                 self.arithmetic()
-                self.state = 785
+                self.state = 783
                 self._errHandler.sync(self)
                 _alt = self._interp.adaptivePredict(self._input, 80, self._ctx)
                 while _alt != 2 and _alt != ATN.INVALID_ALT_NUMBER:
                     if _alt == 1:
-                        self.state = 780
+                        self.state = 778
                         self.cmp_op()
-                        self.state = 781
+                        self.state = 779
                         self.arithmetic()
-                    self.state = 787
+                    self.state = 785
                     self._errHandler.sync(self)
                     _alt = self._interp.adaptivePredict(self._input, 80, self._ctx)
 
                 pass
             else:
                 raise NoViableAltException(self)
 
@@ -5631,57 +5596,57 @@
 
         def exitRule(self, listener: ParseTreeListener):
             if hasattr(listener, "exitCmp_op"):
                 listener.exitCmp_op(self)
 
     def cmp_op(self):
         localctx = jacParser.Cmp_opContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 114, self.RULE_cmp_op)
+        self.enterRule(localctx, 112, self.RULE_cmp_op)
         try:
-            self.state = 798
+            self.state = 796
             self._errHandler.sync(self)
             token = self._input.LA(1)
             if token in [jacParser.EE]:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 790
+                self.state = 788
                 self.match(jacParser.EE)
                 pass
             elif token in [jacParser.LT]:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 791
+                self.state = 789
                 self.match(jacParser.LT)
                 pass
             elif token in [jacParser.GT]:
                 self.enterOuterAlt(localctx, 3)
-                self.state = 792
+                self.state = 790
                 self.match(jacParser.GT)
                 pass
             elif token in [jacParser.LTE]:
                 self.enterOuterAlt(localctx, 4)
-                self.state = 793
+                self.state = 791
                 self.match(jacParser.LTE)
                 pass
             elif token in [jacParser.GTE]:
                 self.enterOuterAlt(localctx, 5)
-                self.state = 794
+                self.state = 792
                 self.match(jacParser.GTE)
                 pass
             elif token in [jacParser.NE]:
                 self.enterOuterAlt(localctx, 6)
-                self.state = 795
+                self.state = 793
                 self.match(jacParser.NE)
                 pass
             elif token in [jacParser.KW_IN]:
                 self.enterOuterAlt(localctx, 7)
-                self.state = 796
+                self.state = 794
                 self.match(jacParser.KW_IN)
                 pass
             elif token in [jacParser.NOT]:
                 self.enterOuterAlt(localctx, 8)
-                self.state = 797
+                self.state = 795
                 self.nin()
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -5715,20 +5680,20 @@
 
         def exitRule(self, listener: ParseTreeListener):
             if hasattr(listener, "exitNin"):
                 listener.exitNin(self)
 
     def nin(self):
         localctx = jacParser.NinContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 116, self.RULE_nin)
+        self.enterRule(localctx, 114, self.RULE_nin)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 800
+            self.state = 798
             self.match(jacParser.NOT)
-            self.state = 801
+            self.state = 799
             self.match(jacParser.KW_IN)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -5770,35 +5735,35 @@
 
         def exitRule(self, listener: ParseTreeListener):
             if hasattr(listener, "exitArithmetic"):
                 listener.exitArithmetic(self)
 
     def arithmetic(self):
         localctx = jacParser.ArithmeticContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 118, self.RULE_arithmetic)
+        self.enterRule(localctx, 116, self.RULE_arithmetic)
         self._la = 0  # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 803
+            self.state = 801
             self.term()
-            self.state = 808
+            self.state = 806
             self._errHandler.sync(self)
             _alt = self._interp.adaptivePredict(self._input, 83, self._ctx)
             while _alt != 2 and _alt != ATN.INVALID_ALT_NUMBER:
                 if _alt == 1:
-                    self.state = 804
+                    self.state = 802
                     _la = self._input.LA(1)
                     if not (_la == jacParser.PLUS or _la == jacParser.MINUS):
                         self._errHandler.recoverInline(self)
                     else:
                         self._errHandler.reportMatch(self)
                         self.consume()
-                    self.state = 805
+                    self.state = 803
                     self.term()
-                self.state = 810
+                self.state = 808
                 self._errHandler.sync(self)
                 _alt = self._interp.adaptivePredict(self._input, 83, self._ctx)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -5848,32 +5813,32 @@
 
         def exitRule(self, listener: ParseTreeListener):
             if hasattr(listener, "exitTerm"):
                 listener.exitTerm(self)
 
     def term(self):
         localctx = jacParser.TermContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 120, self.RULE_term)
+        self.enterRule(localctx, 118, self.RULE_term)
         self._la = 0  # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 811
+            self.state = 809
             self.factor()
-            self.state = 816
+            self.state = 814
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             while (((_la - 95)) & ~0x3F) == 0 and (
                 (1 << (_la - 95))
                 & (
                     (1 << (jacParser.STAR_MUL - 95))
                     | (1 << (jacParser.DIV - 95))
                     | (1 << (jacParser.MOD - 95))
                 )
             ) != 0:
-                self.state = 812
+                self.state = 810
                 _la = self._input.LA(1)
                 if not (
                     (
                         (((_la - 95)) & ~0x3F) == 0
                         and (
                             (1 << (_la - 95))
                             & (
@@ -5885,17 +5850,17 @@
                         != 0
                     )
                 ):
                     self._errHandler.recoverInline(self)
                 else:
                     self._errHandler.reportMatch(self)
                     self.consume()
-                self.state = 813
+                self.state = 811
                 self.factor()
-                self.state = 818
+                self.state = 816
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -5933,36 +5898,36 @@
 
         def exitRule(self, listener: ParseTreeListener):
             if hasattr(listener, "exitFactor"):
                 listener.exitFactor(self)
 
     def factor(self):
         localctx = jacParser.FactorContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 122, self.RULE_factor)
+        self.enterRule(localctx, 120, self.RULE_factor)
         self._la = 0  # Token type
         try:
-            self.state = 822
+            self.state = 820
             self._errHandler.sync(self)
             la_ = self._interp.adaptivePredict(self._input, 85, self._ctx)
             if la_ == 1:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 819
+                self.state = 817
                 _la = self._input.LA(1)
                 if not (_la == jacParser.PLUS or _la == jacParser.MINUS):
                     self._errHandler.recoverInline(self)
                 else:
                     self._errHandler.reportMatch(self)
                     self.consume()
-                self.state = 820
+                self.state = 818
                 self.factor()
                 pass
 
             elif la_ == 2:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 821
+                self.state = 819
                 self.power()
                 pass
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -6003,29 +5968,29 @@
 
         def exitRule(self, listener: ParseTreeListener):
             if hasattr(listener, "exitPower"):
                 listener.exitPower(self)
 
     def power(self):
         localctx = jacParser.PowerContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 124, self.RULE_power)
+        self.enterRule(localctx, 122, self.RULE_power)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 824
+            self.state = 822
             self.atom(0)
-            self.state = 829
+            self.state = 827
             self._errHandler.sync(self)
             _alt = self._interp.adaptivePredict(self._input, 86, self._ctx)
             while _alt != 2 and _alt != ATN.INVALID_ALT_NUMBER:
                 if _alt == 1:
-                    self.state = 825
+                    self.state = 823
                     self.match(jacParser.POW)
-                    self.state = 826
+                    self.state = 824
                     self.factor()
-                self.state = 831
+                self.state = 829
                 self._errHandler.sync(self)
                 _alt = self._interp.adaptivePredict(self._input, 86, self._ctx)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -6063,30 +6028,30 @@
 
         def exitRule(self, listener: ParseTreeListener):
             if hasattr(listener, "exitGlobal_ref"):
                 listener.exitGlobal_ref(self)
 
     def global_ref(self):
         localctx = jacParser.Global_refContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 126, self.RULE_global_ref)
+        self.enterRule(localctx, 124, self.RULE_global_ref)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 832
+            self.state = 830
             self.match(jacParser.KW_GLOBAL)
-            self.state = 833
+            self.state = 831
             self.match(jacParser.DOT)
-            self.state = 836
+            self.state = 834
             self._errHandler.sync(self)
             token = self._input.LA(1)
             if token in [jacParser.KW_CONTEXT, jacParser.KW_INFO, jacParser.KW_DETAILS]:
-                self.state = 834
+                self.state = 832
                 self.obj_built_in()
                 pass
             elif token in [jacParser.NAME]:
-                self.state = 835
+                self.state = 833
                 self.match(jacParser.NAME)
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -6183,145 +6148,145 @@
                 listener.exitAtom(self)
 
     def atom(self, _p: int = 0):
         _parentctx = self._ctx
         _parentState = self.state
         localctx = jacParser.AtomContext(self, self._ctx, _parentState)
         _prevctx = localctx
-        _startState = 128
-        self.enterRecursionRule(localctx, 128, self.RULE_atom, _p)
+        _startState = 126
+        self.enterRecursionRule(localctx, 126, self.RULE_atom, _p)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 864
+            self.state = 862
             self._errHandler.sync(self)
             token = self._input.LA(1)
             if token in [jacParser.INT]:
-                self.state = 839
+                self.state = 837
                 self.match(jacParser.INT)
                 pass
             elif token in [jacParser.FLOAT]:
-                self.state = 840
+                self.state = 838
                 self.match(jacParser.FLOAT)
                 pass
             elif token in [jacParser.STRING]:
-                self.state = 841
+                self.state = 839
                 self.multistring()
                 pass
             elif token in [jacParser.BOOL]:
-                self.state = 842
+                self.state = 840
                 self.match(jacParser.BOOL)
                 pass
             elif token in [jacParser.NULL]:
-                self.state = 843
+                self.state = 841
                 self.match(jacParser.NULL)
                 pass
             elif token in [jacParser.NAME]:
-                self.state = 844
+                self.state = 842
                 self.match(jacParser.NAME)
                 pass
             elif token in [jacParser.KW_GLOBAL]:
-                self.state = 845
+                self.state = 843
                 self.global_ref()
                 pass
             elif token in [
                 jacParser.T__1,
                 jacParser.T__3,
                 jacParser.T__4,
                 jacParser.T__5,
                 jacParser.NODE_DBL_COLON,
                 jacParser.MINUS,
             ]:
-                self.state = 846
+                self.state = 844
                 self.node_edge_ref()
                 pass
             elif token in [jacParser.LSQUARE]:
-                self.state = 847
+                self.state = 845
                 self.list_val()
                 pass
             elif token in [jacParser.LBRACE]:
-                self.state = 848
+                self.state = 846
                 self.dict_val()
                 pass
             elif token in [jacParser.LPAREN]:
-                self.state = 849
+                self.state = 847
                 self.match(jacParser.LPAREN)
-                self.state = 850
+                self.state = 848
                 self.expression()
-                self.state = 851
+                self.state = 849
                 self.match(jacParser.RPAREN)
                 pass
             elif token in [jacParser.DBL_COLON]:
-                self.state = 853
+                self.state = 851
                 self.ability_op()
-                self.state = 854
+                self.state = 852
                 self.match(jacParser.NAME)
-                self.state = 856
+                self.state = 854
                 self._errHandler.sync(self)
                 la_ = self._interp.adaptivePredict(self._input, 88, self._ctx)
                 if la_ == 1:
-                    self.state = 855
+                    self.state = 853
                     self.spawn_ctx()
 
                 pass
             elif token in [jacParser.KW_SYNC]:
-                self.state = 858
+                self.state = 856
                 self.match(jacParser.KW_SYNC)
-                self.state = 859
+                self.state = 857
                 self.atom(5)
                 pass
             elif token in [jacParser.KW_SPAWN]:
-                self.state = 860
+                self.state = 858
                 self.spawn()
                 pass
             elif token in [jacParser.KW_REF]:
-                self.state = 861
+                self.state = 859
                 self.ref()
                 pass
             elif token in [jacParser.STAR_MUL]:
-                self.state = 862
+                self.state = 860
                 self.deref()
                 pass
             elif token in [
                 jacParser.TYP_STRING,
                 jacParser.TYP_INT,
                 jacParser.TYP_FLOAT,
                 jacParser.TYP_LIST,
                 jacParser.TYP_DICT,
                 jacParser.TYP_BOOL,
                 jacParser.KW_TYPE,
                 jacParser.KW_NODE,
                 jacParser.KW_EDGE,
             ]:
-                self.state = 863
+                self.state = 861
                 self.any_type()
                 pass
             else:
                 raise NoViableAltException(self)
 
             self._ctx.stop = self._input.LT(-1)
-            self.state = 870
+            self.state = 868
             self._errHandler.sync(self)
             _alt = self._interp.adaptivePredict(self._input, 90, self._ctx)
             while _alt != 2 and _alt != ATN.INVALID_ALT_NUMBER:
                 if _alt == 1:
                     if self._parseListeners is not None:
                         self.triggerExitRuleEvent()
                     _prevctx = localctx
                     localctx = jacParser.AtomContext(self, _parentctx, _parentState)
                     self.pushNewRecursionContext(localctx, _startState, self.RULE_atom)
-                    self.state = 866
+                    self.state = 864
                     if not self.precpred(self._ctx, 6):
                         from antlr4.error.Errors import FailedPredicateException
 
                         raise FailedPredicateException(
                             self, "self.precpred(self._ctx, 6)"
                         )
-                    self.state = 867
+                    self.state = 865
                     self.atom_trailer()
-                self.state = 872
+                self.state = 870
                 self._errHandler.sync(self)
                 _alt = self._interp.adaptivePredict(self._input, 90, self._ctx)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -6346,75 +6311,122 @@
 
         def NAME(self):
             return self.getToken(jacParser.NAME, 0)
 
         def index_slice(self):
             return self.getTypedRuleContext(jacParser.Index_sliceContext, 0)
 
-        def LPAREN(self):
-            return self.getToken(jacParser.LPAREN, 0)
-
-        def RPAREN(self):
-            return self.getToken(jacParser.RPAREN, 0)
-
-        def param_list(self):
-            return self.getTypedRuleContext(jacParser.Param_listContext, 0)
-
-        def ability_op(self):
-            return self.getTypedRuleContext(jacParser.Ability_opContext, 0)
-
-        def spawn_ctx(self):
-            return self.getTypedRuleContext(jacParser.Spawn_ctxContext, 0)
+        def ability_call(self):
+            return self.getTypedRuleContext(jacParser.Ability_callContext, 0)
 
         def getRuleIndex(self):
             return jacParser.RULE_atom_trailer
 
         def enterRule(self, listener: ParseTreeListener):
             if hasattr(listener, "enterAtom_trailer"):
                 listener.enterAtom_trailer(self)
 
         def exitRule(self, listener: ParseTreeListener):
             if hasattr(listener, "exitAtom_trailer"):
                 listener.exitAtom_trailer(self)
 
     def atom_trailer(self):
         localctx = jacParser.Atom_trailerContext(self, self._ctx, self.state)
-        self.enterRule(localctx, 130, self.RULE_atom_trailer)
-        self._la = 0  # Token type
+        self.enterRule(localctx, 128, self.RULE_atom_trailer)
         try:
-            self.state = 888
+            self.state = 877
             self._errHandler.sync(self)
-            la_ = self._interp.adaptivePredict(self._input, 93, self._ctx)
+            la_ = self._interp.adaptivePredict(self._input, 91, self._ctx)
             if la_ == 1:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 873
+                self.state = 871
                 self.match(jacParser.DOT)
-                self.state = 874
+                self.state = 872
                 self.built_in()
                 pass
 
             elif la_ == 2:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 875
+                self.state = 873
                 self.match(jacParser.DOT)
-                self.state = 876
+                self.state = 874
                 self.match(jacParser.NAME)
                 pass
 
             elif la_ == 3:
                 self.enterOuterAlt(localctx, 3)
-                self.state = 877
+                self.state = 875
                 self.index_slice()
                 pass
 
             elif la_ == 4:
                 self.enterOuterAlt(localctx, 4)
-                self.state = 878
+                self.state = 876
+                self.ability_call()
+                pass
+
+        except RecognitionException as re:
+            localctx.exception = re
+            self._errHandler.reportError(self, re)
+            self._errHandler.recover(self, re)
+        finally:
+            self.exitRule()
+        return localctx
+
+    class Ability_callContext(ParserRuleContext):
+        __slots__ = "parser"
+
+        def __init__(
+            self, parser, parent: ParserRuleContext = None, invokingState: int = -1
+        ):
+            super().__init__(parent, invokingState)
+            self.parser = parser
+
+        def LPAREN(self):
+            return self.getToken(jacParser.LPAREN, 0)
+
+        def RPAREN(self):
+            return self.getToken(jacParser.RPAREN, 0)
+
+        def param_list(self):
+            return self.getTypedRuleContext(jacParser.Param_listContext, 0)
+
+        def ability_op(self):
+            return self.getTypedRuleContext(jacParser.Ability_opContext, 0)
+
+        def NAME(self):
+            return self.getToken(jacParser.NAME, 0)
+
+        def spawn_ctx(self):
+            return self.getTypedRuleContext(jacParser.Spawn_ctxContext, 0)
+
+        def getRuleIndex(self):
+            return jacParser.RULE_ability_call
+
+        def enterRule(self, listener: ParseTreeListener):
+            if hasattr(listener, "enterAbility_call"):
+                listener.enterAbility_call(self)
+
+        def exitRule(self, listener: ParseTreeListener):
+            if hasattr(listener, "exitAbility_call"):
+                listener.exitAbility_call(self)
+
+    def ability_call(self):
+        localctx = jacParser.Ability_callContext(self, self._ctx, self.state)
+        self.enterRule(localctx, 130, self.RULE_ability_call)
+        self._la = 0  # Token type
+        try:
+            self.state = 889
+            self._errHandler.sync(self)
+            token = self._input.LA(1)
+            if token in [jacParser.LPAREN]:
+                self.enterOuterAlt(localctx, 1)
+                self.state = 879
                 self.match(jacParser.LPAREN)
-                self.state = 880
+                self.state = 881
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
                 if (
                     ((_la) & ~0x3F) == 0
                     and (
                         (1 << _la)
                         & (
@@ -6458,35 +6470,36 @@
                             | (1 << (jacParser.INT - 77))
                             | (1 << (jacParser.NULL - 77))
                             | (1 << (jacParser.NAME - 77))
                         )
                     )
                     != 0
                 ):
-                    self.state = 879
+                    self.state = 880
                     self.param_list()
 
-                self.state = 882
+                self.state = 883
                 self.match(jacParser.RPAREN)
                 pass
-
-            elif la_ == 5:
-                self.enterOuterAlt(localctx, 5)
-                self.state = 883
-                self.ability_op()
+            elif token in [jacParser.DBL_COLON]:
+                self.enterOuterAlt(localctx, 2)
                 self.state = 884
+                self.ability_op()
+                self.state = 885
                 self.match(jacParser.NAME)
-                self.state = 886
+                self.state = 887
                 self._errHandler.sync(self)
-                la_ = self._interp.adaptivePredict(self._input, 92, self._ctx)
+                la_ = self._interp.adaptivePredict(self._input, 93, self._ctx)
                 if la_ == 1:
-                    self.state = 885
+                    self.state = 886
                     self.spawn_ctx()
 
                 pass
+            else:
+                raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -6521,30 +6534,30 @@
             if hasattr(listener, "exitAbility_op"):
                 listener.exitAbility_op(self)
 
     def ability_op(self):
         localctx = jacParser.Ability_opContext(self, self._ctx, self.state)
         self.enterRule(localctx, 132, self.RULE_ability_op)
         try:
-            self.state = 894
+            self.state = 895
             self._errHandler.sync(self)
-            la_ = self._interp.adaptivePredict(self._input, 94, self._ctx)
+            la_ = self._interp.adaptivePredict(self._input, 95, self._ctx)
             if la_ == 1:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 890
+                self.state = 891
                 self.match(jacParser.DBL_COLON)
                 pass
 
             elif la_ == 2:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 891
-                self.match(jacParser.DBL_COLON)
                 self.state = 892
-                self.match(jacParser.NAME)
+                self.match(jacParser.DBL_COLON)
                 self.state = 893
+                self.match(jacParser.NAME)
+                self.state = 894
                 self.match(jacParser.COLON)
                 pass
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -6579,17 +6592,17 @@
                 listener.exitRef(self)
 
     def ref(self):
         localctx = jacParser.RefContext(self, self._ctx, self.state)
         self.enterRule(localctx, 134, self.RULE_ref)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 896
-            self.match(jacParser.KW_REF)
             self.state = 897
+            self.match(jacParser.KW_REF)
+            self.state = 898
             self.atom(0)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -6622,17 +6635,17 @@
                 listener.exitDeref(self)
 
     def deref(self):
         localctx = jacParser.DerefContext(self, self._ctx, self.state)
         self.enterRule(localctx, 136, self.RULE_deref)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 899
-            self.match(jacParser.STAR_MUL)
             self.state = 900
+            self.match(jacParser.STAR_MUL)
+            self.state = 901
             self.atom(0)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -6673,49 +6686,49 @@
             if hasattr(listener, "exitBuilt_in"):
                 listener.exitBuilt_in(self)
 
     def built_in(self):
         localctx = jacParser.Built_inContext(self, self._ctx, self.state)
         self.enterRule(localctx, 138, self.RULE_built_in)
         try:
-            self.state = 908
+            self.state = 909
             self._errHandler.sync(self)
-            la_ = self._interp.adaptivePredict(self._input, 95, self._ctx)
+            la_ = self._interp.adaptivePredict(self._input, 96, self._ctx)
             if la_ == 1:
                 self.enterOuterAlt(localctx, 1)
 
                 pass
 
             elif la_ == 2:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 903
+                self.state = 904
                 self.string_built_in()
                 pass
 
             elif la_ == 3:
                 self.enterOuterAlt(localctx, 3)
-                self.state = 904
+                self.state = 905
                 self.dict_built_in()
                 pass
 
             elif la_ == 4:
                 self.enterOuterAlt(localctx, 4)
-                self.state = 905
+                self.state = 906
                 self.list_built_in()
                 pass
 
             elif la_ == 5:
                 self.enterOuterAlt(localctx, 5)
-                self.state = 906
+                self.state = 907
                 self.obj_built_in()
                 pass
 
             elif la_ == 6:
                 self.enterOuterAlt(localctx, 6)
-                self.state = 907
+                self.state = 908
                 self.cast_built_in()
                 pass
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -6747,15 +6760,15 @@
                 listener.exitCast_built_in(self)
 
     def cast_built_in(self):
         localctx = jacParser.Cast_built_inContext(self, self._ctx, self.state)
         self.enterRule(localctx, 140, self.RULE_cast_built_in)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 910
+            self.state = 911
             self.any_type()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -6792,15 +6805,15 @@
 
     def obj_built_in(self):
         localctx = jacParser.Obj_built_inContext(self, self._ctx, self.state)
         self.enterRule(localctx, 142, self.RULE_obj_built_in)
         self._la = 0  # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 912
+            self.state = 913
             _la = self._input.LA(1)
             if not (
                 (
                     ((_la) & ~0x3F) == 0
                     and (
                         (1 << _la)
                         & (
@@ -6878,65 +6891,65 @@
                 listener.exitDict_built_in(self)
 
     def dict_built_in(self):
         localctx = jacParser.Dict_built_inContext(self, self._ctx, self.state)
         self.enterRule(localctx, 144, self.RULE_dict_built_in)
         self._la = 0  # Token type
         try:
-            self.state = 931
+            self.state = 932
             self._errHandler.sync(self)
             token = self._input.LA(1)
             if token in [jacParser.KW_KEYS]:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 914
+                self.state = 915
                 self.match(jacParser.KW_KEYS)
                 pass
             elif token in [jacParser.LBRACE]:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 915
-                self.match(jacParser.LBRACE)
                 self.state = 916
-                self.name_list()
+                self.match(jacParser.LBRACE)
                 self.state = 917
+                self.name_list()
+                self.state = 918
                 self.match(jacParser.RBRACE)
                 pass
             elif token in [jacParser.TYP_DICT, jacParser.DICT_DBL_COLON]:
                 self.enterOuterAlt(localctx, 3)
-                self.state = 922
+                self.state = 923
                 self._errHandler.sync(self)
                 token = self._input.LA(1)
                 if token in [jacParser.TYP_DICT]:
-                    self.state = 919
-                    self.match(jacParser.TYP_DICT)
                     self.state = 920
+                    self.match(jacParser.TYP_DICT)
+                    self.state = 921
                     self.match(jacParser.DBL_COLON)
                     pass
                 elif token in [jacParser.DICT_DBL_COLON]:
-                    self.state = 921
+                    self.state = 922
                     self.match(jacParser.DICT_DBL_COLON)
                     pass
                 else:
                     raise NoViableAltException(self)
 
-                self.state = 924
+                self.state = 925
                 _la = self._input.LA(1)
                 if not (_la == jacParser.KW_KEYS or _la == jacParser.NAME):
                     self._errHandler.recoverInline(self)
                 else:
                     self._errHandler.reportMatch(self)
                     self.consume()
-                self.state = 929
+                self.state = 930
                 self._errHandler.sync(self)
-                la_ = self._interp.adaptivePredict(self._input, 97, self._ctx)
+                la_ = self._interp.adaptivePredict(self._input, 98, self._ctx)
                 if la_ == 1:
-                    self.state = 925
-                    self.match(jacParser.LPAREN)
                     self.state = 926
-                    self.expr_list()
+                    self.match(jacParser.LPAREN)
                     self.state = 927
+                    self.expr_list()
+                    self.state = 928
                     self.match(jacParser.RPAREN)
 
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
@@ -6991,51 +7004,51 @@
             if hasattr(listener, "exitList_built_in"):
                 listener.exitList_built_in(self)
 
     def list_built_in(self):
         localctx = jacParser.List_built_inContext(self, self._ctx, self.state)
         self.enterRule(localctx, 146, self.RULE_list_built_in)
         try:
-            self.state = 946
+            self.state = 947
             self._errHandler.sync(self)
             token = self._input.LA(1)
             if token in [jacParser.KW_LENGTH]:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 933
+                self.state = 934
                 self.match(jacParser.KW_LENGTH)
                 pass
             elif token in [jacParser.TYP_LIST, jacParser.LIST_DBL_COLON]:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 937
+                self.state = 938
                 self._errHandler.sync(self)
                 token = self._input.LA(1)
                 if token in [jacParser.TYP_LIST]:
-                    self.state = 934
-                    self.match(jacParser.TYP_LIST)
                     self.state = 935
+                    self.match(jacParser.TYP_LIST)
+                    self.state = 936
                     self.match(jacParser.DBL_COLON)
                     pass
                 elif token in [jacParser.LIST_DBL_COLON]:
-                    self.state = 936
+                    self.state = 937
                     self.match(jacParser.LIST_DBL_COLON)
                     pass
                 else:
                     raise NoViableAltException(self)
 
-                self.state = 939
+                self.state = 940
                 self.match(jacParser.NAME)
-                self.state = 944
+                self.state = 945
                 self._errHandler.sync(self)
-                la_ = self._interp.adaptivePredict(self._input, 100, self._ctx)
+                la_ = self._interp.adaptivePredict(self._input, 101, self._ctx)
                 if la_ == 1:
-                    self.state = 940
-                    self.match(jacParser.LPAREN)
                     self.state = 941
-                    self.expr_list()
+                    self.match(jacParser.LPAREN)
                     self.state = 942
+                    self.expr_list()
+                    self.state = 943
                     self.match(jacParser.RPAREN)
 
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
@@ -7088,41 +7101,41 @@
                 listener.exitString_built_in(self)
 
     def string_built_in(self):
         localctx = jacParser.String_built_inContext(self, self._ctx, self.state)
         self.enterRule(localctx, 148, self.RULE_string_built_in)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 951
+            self.state = 952
             self._errHandler.sync(self)
             token = self._input.LA(1)
             if token in [jacParser.TYP_STRING]:
-                self.state = 948
-                self.match(jacParser.TYP_STRING)
                 self.state = 949
+                self.match(jacParser.TYP_STRING)
+                self.state = 950
                 self.match(jacParser.DBL_COLON)
                 pass
             elif token in [jacParser.STR_DBL_COLON]:
-                self.state = 950
+                self.state = 951
                 self.match(jacParser.STR_DBL_COLON)
                 pass
             else:
                 raise NoViableAltException(self)
 
-            self.state = 953
+            self.state = 954
             self.match(jacParser.NAME)
-            self.state = 958
+            self.state = 959
             self._errHandler.sync(self)
-            la_ = self._interp.adaptivePredict(self._input, 103, self._ctx)
+            la_ = self._interp.adaptivePredict(self._input, 104, self._ctx)
             if la_ == 1:
-                self.state = 954
-                self.match(jacParser.LPAREN)
                 self.state = 955
-                self.expr_list()
+                self.match(jacParser.LPAREN)
                 self.state = 956
+                self.expr_list()
+                self.state = 957
                 self.match(jacParser.RPAREN)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
@@ -7161,51 +7174,51 @@
             if hasattr(listener, "exitNode_edge_ref"):
                 listener.exitNode_edge_ref(self)
 
     def node_edge_ref(self):
         localctx = jacParser.Node_edge_refContext(self, self._ctx, self.state)
         self.enterRule(localctx, 150, self.RULE_node_edge_ref)
         try:
-            self.state = 971
+            self.state = 972
             self._errHandler.sync(self)
             token = self._input.LA(1)
             if token in [jacParser.NODE_DBL_COLON]:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 960
+                self.state = 961
                 self.node_ref()
-                self.state = 962
+                self.state = 963
                 self._errHandler.sync(self)
-                la_ = self._interp.adaptivePredict(self._input, 104, self._ctx)
+                la_ = self._interp.adaptivePredict(self._input, 105, self._ctx)
                 if la_ == 1:
-                    self.state = 961
+                    self.state = 962
                     self.filter_ctx()
 
-                self.state = 965
+                self.state = 966
                 self._errHandler.sync(self)
-                la_ = self._interp.adaptivePredict(self._input, 105, self._ctx)
+                la_ = self._interp.adaptivePredict(self._input, 106, self._ctx)
                 if la_ == 1:
-                    self.state = 964
+                    self.state = 965
                     self.node_edge_ref()
 
                 pass
             elif token in [
                 jacParser.T__1,
                 jacParser.T__3,
                 jacParser.T__4,
                 jacParser.T__5,
                 jacParser.MINUS,
             ]:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 967
+                self.state = 968
                 self.edge_ref()
-                self.state = 969
+                self.state = 970
                 self._errHandler.sync(self)
-                la_ = self._interp.adaptivePredict(self._input, 106, self._ctx)
+                la_ = self._interp.adaptivePredict(self._input, 107, self._ctx)
                 if la_ == 1:
-                    self.state = 968
+                    self.state = 969
                     self.node_edge_ref()
 
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
@@ -7243,17 +7256,17 @@
                 listener.exitNode_ref(self)
 
     def node_ref(self):
         localctx = jacParser.Node_refContext(self, self._ctx, self.state)
         self.enterRule(localctx, 152, self.RULE_node_ref)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 973
-            self.match(jacParser.NODE_DBL_COLON)
             self.state = 974
+            self.match(jacParser.NODE_DBL_COLON)
+            self.state = 975
             self.match(jacParser.NAME)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -7286,17 +7299,17 @@
                 listener.exitWalker_ref(self)
 
     def walker_ref(self):
         localctx = jacParser.Walker_refContext(self, self._ctx, self.state)
         self.enterRule(localctx, 154, self.RULE_walker_ref)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 976
-            self.match(jacParser.WALKER_DBL_COLON)
             self.state = 977
+            self.match(jacParser.WALKER_DBL_COLON)
+            self.state = 978
             self.match(jacParser.NAME)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -7329,17 +7342,17 @@
                 listener.exitGraph_ref(self)
 
     def graph_ref(self):
         localctx = jacParser.Graph_refContext(self, self._ctx, self.state)
         self.enterRule(localctx, 156, self.RULE_graph_ref)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 979
-            self.match(jacParser.GRAPH_DBL_COLON)
             self.state = 980
+            self.match(jacParser.GRAPH_DBL_COLON)
+            self.state = 981
             self.match(jacParser.NAME)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -7372,17 +7385,17 @@
                 listener.exitType_ref(self)
 
     def type_ref(self):
         localctx = jacParser.Type_refContext(self, self._ctx, self.state)
         self.enterRule(localctx, 158, self.RULE_type_ref)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 982
-            self.match(jacParser.TYPE_DBL_COLON)
             self.state = 983
+            self.match(jacParser.TYPE_DBL_COLON)
+            self.state = 984
             self.match(jacParser.NAME)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -7417,32 +7430,32 @@
             if hasattr(listener, "exitEdge_ref"):
                 listener.exitEdge_ref(self)
 
     def edge_ref(self):
         localctx = jacParser.Edge_refContext(self, self._ctx, self.state)
         self.enterRule(localctx, 160, self.RULE_edge_ref)
         try:
-            self.state = 988
+            self.state = 989
             self._errHandler.sync(self)
-            la_ = self._interp.adaptivePredict(self._input, 108, self._ctx)
+            la_ = self._interp.adaptivePredict(self._input, 109, self._ctx)
             if la_ == 1:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 985
+                self.state = 986
                 self.edge_to()
                 pass
 
             elif la_ == 2:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 986
+                self.state = 987
                 self.edge_from()
                 pass
 
             elif la_ == 3:
                 self.enterOuterAlt(localctx, 3)
-                self.state = 987
+                self.state = 988
                 self.edge_any()
                 pass
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -7486,45 +7499,45 @@
                 listener.exitEdge_to(self)
 
     def edge_to(self):
         localctx = jacParser.Edge_toContext(self, self._ctx, self.state)
         self.enterRule(localctx, 162, self.RULE_edge_to)
         self._la = 0  # Token type
         try:
-            self.state = 1001
+            self.state = 1002
             self._errHandler.sync(self)
             token = self._input.LA(1)
             if token in [jacParser.T__1]:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 990
+                self.state = 991
                 self.match(jacParser.T__1)
                 pass
             elif token in [jacParser.MINUS]:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 991
+                self.state = 992
                 self.match(jacParser.MINUS)
-                self.state = 998
+                self.state = 999
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
                 if _la == jacParser.LSQUARE:
-                    self.state = 992
-                    self.match(jacParser.LSQUARE)
                     self.state = 993
+                    self.match(jacParser.LSQUARE)
+                    self.state = 994
                     self.match(jacParser.NAME)
-                    self.state = 995
+                    self.state = 996
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
                     if _la == jacParser.LPAREN:
-                        self.state = 994
+                        self.state = 995
                         self.filter_ctx()
 
-                    self.state = 997
+                    self.state = 998
                     self.match(jacParser.RSQUARE)
 
-                self.state = 1000
+                self.state = 1001
                 self.match(jacParser.T__2)
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -7570,45 +7583,45 @@
                 listener.exitEdge_from(self)
 
     def edge_from(self):
         localctx = jacParser.Edge_fromContext(self, self._ctx, self.state)
         self.enterRule(localctx, 164, self.RULE_edge_from)
         self._la = 0  # Token type
         try:
-            self.state = 1014
+            self.state = 1015
             self._errHandler.sync(self)
             token = self._input.LA(1)
             if token in [jacParser.T__3]:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 1003
+                self.state = 1004
                 self.match(jacParser.T__3)
                 pass
             elif token in [jacParser.T__4]:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 1004
+                self.state = 1005
                 self.match(jacParser.T__4)
-                self.state = 1011
+                self.state = 1012
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
                 if _la == jacParser.LSQUARE:
-                    self.state = 1005
-                    self.match(jacParser.LSQUARE)
                     self.state = 1006
+                    self.match(jacParser.LSQUARE)
+                    self.state = 1007
                     self.match(jacParser.NAME)
-                    self.state = 1008
+                    self.state = 1009
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
                     if _la == jacParser.LPAREN:
-                        self.state = 1007
+                        self.state = 1008
                         self.filter_ctx()
 
-                    self.state = 1010
+                    self.state = 1011
                     self.match(jacParser.RSQUARE)
 
-                self.state = 1013
+                self.state = 1014
                 self.match(jacParser.MINUS)
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -7651,45 +7664,45 @@
                 listener.exitEdge_any(self)
 
     def edge_any(self):
         localctx = jacParser.Edge_anyContext(self, self._ctx, self.state)
         self.enterRule(localctx, 166, self.RULE_edge_any)
         self._la = 0  # Token type
         try:
-            self.state = 1027
+            self.state = 1028
             self._errHandler.sync(self)
             token = self._input.LA(1)
             if token in [jacParser.T__5]:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 1016
+                self.state = 1017
                 self.match(jacParser.T__5)
                 pass
             elif token in [jacParser.T__4]:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 1017
+                self.state = 1018
                 self.match(jacParser.T__4)
-                self.state = 1024
+                self.state = 1025
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
                 if _la == jacParser.LSQUARE:
-                    self.state = 1018
-                    self.match(jacParser.LSQUARE)
                     self.state = 1019
+                    self.match(jacParser.LSQUARE)
+                    self.state = 1020
                     self.match(jacParser.NAME)
-                    self.state = 1021
+                    self.state = 1022
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
                     if _la == jacParser.LPAREN:
-                        self.state = 1020
+                        self.state = 1021
                         self.filter_ctx()
 
-                    self.state = 1023
+                    self.state = 1024
                     self.match(jacParser.RSQUARE)
 
-                self.state = 1026
+                self.state = 1027
                 self.match(jacParser.T__2)
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -7728,32 +7741,32 @@
             if hasattr(listener, "exitConnect_op"):
                 listener.exitConnect_op(self)
 
     def connect_op(self):
         localctx = jacParser.Connect_opContext(self, self._ctx, self.state)
         self.enterRule(localctx, 168, self.RULE_connect_op)
         try:
-            self.state = 1032
+            self.state = 1033
             self._errHandler.sync(self)
-            la_ = self._interp.adaptivePredict(self._input, 118, self._ctx)
+            la_ = self._interp.adaptivePredict(self._input, 119, self._ctx)
             if la_ == 1:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 1029
+                self.state = 1030
                 self.connect_to()
                 pass
 
             elif la_ == 2:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 1030
+                self.state = 1031
                 self.connect_from()
                 pass
 
             elif la_ == 3:
                 self.enterOuterAlt(localctx, 3)
-                self.state = 1031
+                self.state = 1032
                 self.connect_any()
                 pass
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -7797,45 +7810,45 @@
                 listener.exitConnect_to(self)
 
     def connect_to(self):
         localctx = jacParser.Connect_toContext(self, self._ctx, self.state)
         self.enterRule(localctx, 170, self.RULE_connect_to)
         self._la = 0  # Token type
         try:
-            self.state = 1045
+            self.state = 1046
             self._errHandler.sync(self)
             token = self._input.LA(1)
             if token in [jacParser.T__6]:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 1034
+                self.state = 1035
                 self.match(jacParser.T__6)
                 pass
             elif token in [jacParser.PLUS]:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 1035
+                self.state = 1036
                 self.match(jacParser.PLUS)
-                self.state = 1042
+                self.state = 1043
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
                 if _la == jacParser.LSQUARE:
-                    self.state = 1036
-                    self.match(jacParser.LSQUARE)
                     self.state = 1037
+                    self.match(jacParser.LSQUARE)
+                    self.state = 1038
                     self.match(jacParser.NAME)
-                    self.state = 1039
+                    self.state = 1040
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
                     if _la == jacParser.LPAREN:
-                        self.state = 1038
+                        self.state = 1039
                         self.spawn_ctx()
 
-                    self.state = 1041
+                    self.state = 1042
                     self.match(jacParser.RSQUARE)
 
-                self.state = 1044
+                self.state = 1045
                 self.match(jacParser.T__7)
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -7881,45 +7894,45 @@
                 listener.exitConnect_from(self)
 
     def connect_from(self):
         localctx = jacParser.Connect_fromContext(self, self._ctx, self.state)
         self.enterRule(localctx, 172, self.RULE_connect_from)
         self._la = 0  # Token type
         try:
-            self.state = 1058
+            self.state = 1059
             self._errHandler.sync(self)
             token = self._input.LA(1)
             if token in [jacParser.T__8]:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 1047
+                self.state = 1048
                 self.match(jacParser.T__8)
                 pass
             elif token in [jacParser.T__9]:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 1048
+                self.state = 1049
                 self.match(jacParser.T__9)
-                self.state = 1055
+                self.state = 1056
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
                 if _la == jacParser.LSQUARE:
-                    self.state = 1049
-                    self.match(jacParser.LSQUARE)
                     self.state = 1050
+                    self.match(jacParser.LSQUARE)
+                    self.state = 1051
                     self.match(jacParser.NAME)
-                    self.state = 1052
+                    self.state = 1053
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
                     if _la == jacParser.LPAREN:
-                        self.state = 1051
+                        self.state = 1052
                         self.spawn_ctx()
 
-                    self.state = 1054
+                    self.state = 1055
                     self.match(jacParser.RSQUARE)
 
-                self.state = 1057
+                self.state = 1058
                 self.match(jacParser.PLUS)
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -7962,45 +7975,45 @@
                 listener.exitConnect_any(self)
 
     def connect_any(self):
         localctx = jacParser.Connect_anyContext(self, self._ctx, self.state)
         self.enterRule(localctx, 174, self.RULE_connect_any)
         self._la = 0  # Token type
         try:
-            self.state = 1071
+            self.state = 1072
             self._errHandler.sync(self)
             token = self._input.LA(1)
             if token in [jacParser.T__10]:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 1060
+                self.state = 1061
                 self.match(jacParser.T__10)
                 pass
             elif token in [jacParser.T__9]:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 1061
+                self.state = 1062
                 self.match(jacParser.T__9)
-                self.state = 1068
+                self.state = 1069
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
                 if _la == jacParser.LSQUARE:
-                    self.state = 1062
-                    self.match(jacParser.LSQUARE)
                     self.state = 1063
+                    self.match(jacParser.LSQUARE)
+                    self.state = 1064
                     self.match(jacParser.NAME)
-                    self.state = 1065
+                    self.state = 1066
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
                     if _la == jacParser.LPAREN:
-                        self.state = 1064
+                        self.state = 1065
                         self.spawn_ctx()
 
-                    self.state = 1067
+                    self.state = 1068
                     self.match(jacParser.RSQUARE)
 
-                self.state = 1070
+                self.state = 1071
                 self.match(jacParser.T__7)
                 pass
             else:
                 raise NoViableAltException(self)
 
         except RecognitionException as re:
             localctx.exception = re
@@ -8041,17 +8054,17 @@
 
     def list_val(self):
         localctx = jacParser.List_valContext(self, self._ctx, self.state)
         self.enterRule(localctx, 176, self.RULE_list_val)
         self._la = 0  # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 1073
+            self.state = 1074
             self.match(jacParser.LSQUARE)
-            self.state = 1075
+            self.state = 1076
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             if (
                 ((_la) & ~0x3F) == 0
                 and (
                     (1 << _la)
                     & (
@@ -8095,18 +8108,18 @@
                         | (1 << (jacParser.INT - 77))
                         | (1 << (jacParser.NULL - 77))
                         | (1 << (jacParser.NAME - 77))
                     )
                 )
                 != 0
             ):
-                self.state = 1074
+                self.state = 1075
                 self.expr_list()
 
-            self.state = 1077
+            self.state = 1078
             self.match(jacParser.RSQUARE)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -8147,38 +8160,38 @@
             if hasattr(listener, "exitIndex_slice"):
                 listener.exitIndex_slice(self)
 
     def index_slice(self):
         localctx = jacParser.Index_sliceContext(self, self._ctx, self.state)
         self.enterRule(localctx, 178, self.RULE_index_slice)
         try:
-            self.state = 1089
+            self.state = 1090
             self._errHandler.sync(self)
-            la_ = self._interp.adaptivePredict(self._input, 129, self._ctx)
+            la_ = self._interp.adaptivePredict(self._input, 130, self._ctx)
             if la_ == 1:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 1079
-                self.match(jacParser.LSQUARE)
                 self.state = 1080
-                self.expression()
+                self.match(jacParser.LSQUARE)
                 self.state = 1081
+                self.expression()
+                self.state = 1082
                 self.match(jacParser.RSQUARE)
                 pass
 
             elif la_ == 2:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 1083
-                self.match(jacParser.LSQUARE)
                 self.state = 1084
-                self.expression()
+                self.match(jacParser.LSQUARE)
                 self.state = 1085
-                self.match(jacParser.COLON)
-                self.state = 1086
                 self.expression()
+                self.state = 1086
+                self.match(jacParser.COLON)
                 self.state = 1087
+                self.expression()
+                self.state = 1088
                 self.match(jacParser.RSQUARE)
                 pass
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -8226,17 +8239,17 @@
 
     def dict_val(self):
         localctx = jacParser.Dict_valContext(self, self._ctx, self.state)
         self.enterRule(localctx, 180, self.RULE_dict_val)
         self._la = 0  # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 1091
+            self.state = 1092
             self.match(jacParser.LBRACE)
-            self.state = 1100
+            self.state = 1101
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             if (
                 ((_la) & ~0x3F) == 0
                 and (
                     (1 << _la)
                     & (
@@ -8280,29 +8293,29 @@
                         | (1 << (jacParser.INT - 77))
                         | (1 << (jacParser.NULL - 77))
                         | (1 << (jacParser.NAME - 77))
                     )
                 )
                 != 0
             ):
-                self.state = 1092
+                self.state = 1093
                 self.kv_pair()
-                self.state = 1097
+                self.state = 1098
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
                 while _la == jacParser.COMMA:
-                    self.state = 1093
-                    self.match(jacParser.COMMA)
                     self.state = 1094
+                    self.match(jacParser.COMMA)
+                    self.state = 1095
                     self.kv_pair()
-                    self.state = 1099
+                    self.state = 1100
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
 
-            self.state = 1102
+            self.state = 1103
             self.match(jacParser.RBRACE)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -8338,19 +8351,19 @@
                 listener.exitKv_pair(self)
 
     def kv_pair(self):
         localctx = jacParser.Kv_pairContext(self, self._ctx, self.state)
         self.enterRule(localctx, 182, self.RULE_kv_pair)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 1104
-            self.expression()
             self.state = 1105
-            self.match(jacParser.COLON)
+            self.expression()
             self.state = 1106
+            self.match(jacParser.COLON)
+            self.state = 1107
             self.expression()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -8383,17 +8396,17 @@
                 listener.exitSpawn(self)
 
     def spawn(self):
         localctx = jacParser.SpawnContext(self, self._ctx, self.state)
         self.enterRule(localctx, 184, self.RULE_spawn)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 1108
-            self.match(jacParser.KW_SPAWN)
             self.state = 1109
+            self.match(jacParser.KW_SPAWN)
+            self.state = 1110
             self.spawn_object()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -8431,38 +8444,38 @@
             if hasattr(listener, "exitSpawn_object"):
                 listener.exitSpawn_object(self)
 
     def spawn_object(self):
         localctx = jacParser.Spawn_objectContext(self, self._ctx, self.state)
         self.enterRule(localctx, 186, self.RULE_spawn_object)
         try:
-            self.state = 1115
+            self.state = 1116
             self._errHandler.sync(self)
-            la_ = self._interp.adaptivePredict(self._input, 132, self._ctx)
+            la_ = self._interp.adaptivePredict(self._input, 133, self._ctx)
             if la_ == 1:
                 self.enterOuterAlt(localctx, 1)
-                self.state = 1111
+                self.state = 1112
                 self.node_spawn()
                 pass
 
             elif la_ == 2:
                 self.enterOuterAlt(localctx, 2)
-                self.state = 1112
+                self.state = 1113
                 self.walker_spawn()
                 pass
 
             elif la_ == 3:
                 self.enterOuterAlt(localctx, 3)
-                self.state = 1113
+                self.state = 1114
                 self.graph_spawn()
                 pass
 
             elif la_ == 4:
                 self.enterOuterAlt(localctx, 4)
-                self.state = 1114
+                self.state = 1115
                 self.type_spawn()
                 pass
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
@@ -8497,17 +8510,17 @@
                 listener.exitSpawn_edge(self)
 
     def spawn_edge(self):
         localctx = jacParser.Spawn_edgeContext(self, self._ctx, self.state)
         self.enterRule(localctx, 188, self.RULE_spawn_edge)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 1117
-            self.expression()
             self.state = 1118
+            self.expression()
+            self.state = 1119
             self.connect_op()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -8543,28 +8556,28 @@
                 listener.exitNode_spawn(self)
 
     def node_spawn(self):
         localctx = jacParser.Node_spawnContext(self, self._ctx, self.state)
         self.enterRule(localctx, 190, self.RULE_node_spawn)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 1121
+            self.state = 1122
             self._errHandler.sync(self)
-            la_ = self._interp.adaptivePredict(self._input, 133, self._ctx)
+            la_ = self._interp.adaptivePredict(self._input, 134, self._ctx)
             if la_ == 1:
-                self.state = 1120
+                self.state = 1121
                 self.spawn_edge()
 
-            self.state = 1123
+            self.state = 1124
             self.node_ref()
-            self.state = 1125
+            self.state = 1126
             self._errHandler.sync(self)
-            la_ = self._interp.adaptivePredict(self._input, 134, self._ctx)
+            la_ = self._interp.adaptivePredict(self._input, 135, self._ctx)
             if la_ == 1:
-                self.state = 1124
+                self.state = 1125
                 self.spawn_ctx()
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
@@ -8599,15 +8612,15 @@
 
     def graph_spawn(self):
         localctx = jacParser.Graph_spawnContext(self, self._ctx, self.state)
         self.enterRule(localctx, 192, self.RULE_graph_spawn)
         self._la = 0  # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 1128
+            self.state = 1129
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             if (
                 ((_la) & ~0x3F) == 0
                 and (
                     (1 << _la)
                     & (
@@ -8651,18 +8664,18 @@
                         | (1 << (jacParser.INT - 77))
                         | (1 << (jacParser.NULL - 77))
                         | (1 << (jacParser.NAME - 77))
                     )
                 )
                 != 0
             ):
-                self.state = 1127
+                self.state = 1128
                 self.spawn_edge()
 
-            self.state = 1130
+            self.state = 1131
             self.graph_ref()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -8702,30 +8715,30 @@
 
     def walker_spawn(self):
         localctx = jacParser.Walker_spawnContext(self, self._ctx, self.state)
         self.enterRule(localctx, 194, self.RULE_walker_spawn)
         self._la = 0  # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 1132
+            self.state = 1133
             self.expression()
-            self.state = 1134
+            self.state = 1135
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             if _la == jacParser.KW_SYNC:
-                self.state = 1133
+                self.state = 1134
                 self.match(jacParser.KW_SYNC)
 
-            self.state = 1136
+            self.state = 1137
             self.walker_ref()
-            self.state = 1138
+            self.state = 1139
             self._errHandler.sync(self)
-            la_ = self._interp.adaptivePredict(self._input, 137, self._ctx)
+            la_ = self._interp.adaptivePredict(self._input, 138, self._ctx)
             if la_ == 1:
-                self.state = 1137
+                self.state = 1138
                 self.spawn_ctx()
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
@@ -8759,21 +8772,21 @@
                 listener.exitType_spawn(self)
 
     def type_spawn(self):
         localctx = jacParser.Type_spawnContext(self, self._ctx, self.state)
         self.enterRule(localctx, 196, self.RULE_type_spawn)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 1140
+            self.state = 1141
             self.type_ref()
-            self.state = 1142
+            self.state = 1143
             self._errHandler.sync(self)
-            la_ = self._interp.adaptivePredict(self._input, 138, self._ctx)
+            la_ = self._interp.adaptivePredict(self._input, 139, self._ctx)
             if la_ == 1:
-                self.state = 1141
+                self.state = 1142
                 self.spawn_ctx()
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
@@ -8820,35 +8833,35 @@
 
     def spawn_ctx(self):
         localctx = jacParser.Spawn_ctxContext(self, self._ctx, self.state)
         self.enterRule(localctx, 198, self.RULE_spawn_ctx)
         self._la = 0  # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 1144
+            self.state = 1145
             self.match(jacParser.LPAREN)
-            self.state = 1153
+            self.state = 1154
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             if _la == jacParser.NAME:
-                self.state = 1145
+                self.state = 1146
                 self.spawn_assign()
-                self.state = 1150
+                self.state = 1151
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
                 while _la == jacParser.COMMA:
-                    self.state = 1146
-                    self.match(jacParser.COMMA)
                     self.state = 1147
+                    self.match(jacParser.COMMA)
+                    self.state = 1148
                     self.spawn_assign()
-                    self.state = 1152
+                    self.state = 1153
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
 
-            self.state = 1155
+            self.state = 1156
             self.match(jacParser.RPAREN)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -8894,35 +8907,35 @@
 
     def filter_ctx(self):
         localctx = jacParser.Filter_ctxContext(self, self._ctx, self.state)
         self.enterRule(localctx, 200, self.RULE_filter_ctx)
         self._la = 0  # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 1157
+            self.state = 1158
             self.match(jacParser.LPAREN)
-            self.state = 1166
+            self.state = 1167
             self._errHandler.sync(self)
             _la = self._input.LA(1)
             if _la == jacParser.NAME:
-                self.state = 1158
+                self.state = 1159
                 self.filter_compare()
-                self.state = 1163
+                self.state = 1164
                 self._errHandler.sync(self)
                 _la = self._input.LA(1)
                 while _la == jacParser.COMMA:
-                    self.state = 1159
-                    self.match(jacParser.COMMA)
                     self.state = 1160
+                    self.match(jacParser.COMMA)
+                    self.state = 1161
                     self.filter_compare()
-                    self.state = 1165
+                    self.state = 1166
                     self._errHandler.sync(self)
                     _la = self._input.LA(1)
 
-            self.state = 1168
+            self.state = 1169
             self.match(jacParser.RPAREN)
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -8958,19 +8971,19 @@
                 listener.exitSpawn_assign(self)
 
     def spawn_assign(self):
         localctx = jacParser.Spawn_assignContext(self, self._ctx, self.state)
         self.enterRule(localctx, 202, self.RULE_spawn_assign)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 1170
-            self.match(jacParser.NAME)
             self.state = 1171
-            self.match(jacParser.EQ)
+            self.match(jacParser.NAME)
             self.state = 1172
+            self.match(jacParser.EQ)
+            self.state = 1173
             self.expression()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -9006,19 +9019,19 @@
                 listener.exitFilter_compare(self)
 
     def filter_compare(self):
         localctx = jacParser.Filter_compareContext(self, self._ctx, self.state)
         self.enterRule(localctx, 204, self.RULE_filter_compare)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 1174
-            self.match(jacParser.NAME)
             self.state = 1175
-            self.cmp_op()
+            self.match(jacParser.NAME)
             self.state = 1176
+            self.cmp_op()
+            self.state = 1177
             self.expression()
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
@@ -9073,15 +9086,15 @@
 
     def any_type(self):
         localctx = jacParser.Any_typeContext(self, self._ctx, self.state)
         self.enterRule(localctx, 206, self.RULE_any_type)
         self._la = 0  # Token type
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 1178
+            self.state = 1179
             _la = self._input.LA(1)
             if not (
                 (
                     ((_la) & ~0x3F) == 0
                     and (
                         (1 << _la)
                         & (
@@ -9138,40 +9151,40 @@
                 listener.exitMultistring(self)
 
     def multistring(self):
         localctx = jacParser.MultistringContext(self, self._ctx, self.state)
         self.enterRule(localctx, 208, self.RULE_multistring)
         try:
             self.enterOuterAlt(localctx, 1)
-            self.state = 1181
+            self.state = 1182
             self._errHandler.sync(self)
             _alt = 1
             while _alt != 2 and _alt != ATN.INVALID_ALT_NUMBER:
                 if _alt == 1:
-                    self.state = 1180
+                    self.state = 1181
                     self.match(jacParser.STRING)
 
                 else:
                     raise NoViableAltException(self)
-                self.state = 1183
+                self.state = 1184
                 self._errHandler.sync(self)
-                _alt = self._interp.adaptivePredict(self._input, 143, self._ctx)
+                _alt = self._interp.adaptivePredict(self._input, 144, self._ctx)
 
         except RecognitionException as re:
             localctx.exception = re
             self._errHandler.reportError(self, re)
             self._errHandler.recover(self, re)
         finally:
             self.exitRule()
         return localctx
 
     def sempred(self, localctx: RuleContext, ruleIndex: int, predIndex: int):
         if self._predicates == None:
             self._predicates = dict()
-        self._predicates[64] = self.atom_sempred
+        self._predicates[63] = self.atom_sempred
         pred = self._predicates.get(ruleIndex, None)
         if pred is None:
             raise Exception("No predicate with index:" + str(ruleIndex))
         else:
             return pred(localctx, predIndex)
 
     def atom_sempred(self, localctx: AtomContext, predIndex: int):
```

### Comparing `jaseci-1.4.0.9/jaseci/jac/jac_set.py` & `jaseci-1.4.1.0/jaseci/jac/jac_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Jac's set class for Jaseci
 
 Adds relevant operators to id_list for operations on sets of nodes and edges
 """
 # from jaseci.utils.id_list import id_list
 from jaseci.utils.utils import logger
-from jaseci.element.element import Element
+from jaseci.prim.element import Element
 
 
 class JacSet(list):
     """
     Jac set class for operations in Jac lang
     (keeps append ordering and no dups)
     """
```

### Comparing `jaseci-1.4.0.9/jaseci/jac/jsci_vm/disasm.py` & `jaseci-1.4.1.0/jaseci/jac/jsci_vm/disasm.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.0.9/jaseci/jac/jsci_vm/inst_ptr.py` & `jaseci-1.4.1.0/jaseci/jac/jsci_vm/inst_ptr.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.0.9/jaseci/jac/jsci_vm/machine.py` & `jaseci-1.4.1.0/jaseci/jac/jsci_vm/machine.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.0.9/jaseci/jac/jsci_vm/op_codes.py` & `jaseci-1.4.1.0/jaseci/jac/jsci_vm/op_codes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from enum import IntEnum, auto
-from jaseci.graph.edge import Edge
-from jaseci.graph.node import Node
+from jaseci.prim.edge import Edge
+from jaseci.prim.node import Node
 
 
 class JsOp(IntEnum):
     PUSH_SCOPE = auto()
     POP_SCOPE = auto()
     ADD = auto()
     SUBTRACT = auto()
```

### Comparing `jaseci-1.4.0.9/jaseci/jac/jsci_vm/tests/test_codegen.py` & `jaseci-1.4.1.0/jaseci/jac/jsci_vm/tests/test_codegen.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.0.9/jaseci/jac/machine/jac_scope.py` & `jaseci-1.4.1.0/jaseci/jac/machine/jac_scope.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,76 +1,69 @@
 """
 Variable scope manager for Jac
 
 Utility for all runtime interaction with variables in different scopes
 """
-from jaseci.utils.id_list import IdList
 from jaseci.jac.machine.jac_value import JacValue
-from jaseci.actions.live_actions import get_global_actions
-
-global_action_sets = None
+from jaseci.jsorc.live_actions import get_global_actions
 
 
 class JacScope:
-    def __init__(self, parent, has_obj, action_sets):
+    def __init__(self, parent, name, has_obj=None, here=None, visitor=None):
         self.parent = parent
+        self.name = name
         self.local_scope = {}
         self.has_obj = has_obj if has_obj else self
         self.context = {}
-        self.action_sets = action_sets
+        self.action_sets = []
+        self._start_time = 0  # For profiling
+        self._total_time = 0  # For profiling
+        self._cum_start_time = None
+        self.set_refs(here, visitor)
         self.setup_actions()
 
     def setup_actions(self):
-        global global_action_sets
-        if global_action_sets is None:
-            global_action_sets = self.group_actions(get_global_actions())
         allactions = []
         for i in self.action_sets:
             allactions += i.obj_list()
-        self.action_sets = global_action_sets
+        self.action_sets = get_global_actions()
         for i in allactions:
             self.add_action(i)
 
     def add_action(self, act):
         group = act.name.split(".")[0]
         if "." in act.name:
             if group not in self.action_sets.keys():
                 self.action_sets[group] = {}
             action = act.name.split(".")[1]
             self.action_sets[group][action] = act
         else:
             self.action_sets[group] = act
 
-    def group_actions(self, act_list):
-        action_sets = {}
-        for act in act_list:
-            group = act.name.split(".")[0]
-            if "." in act.name:
-                if group not in action_sets.keys():
-                    action_sets[group] = {}
-                action = act.name.split(".")[1]
-                action_sets[group][action] = act
-            else:
-                action_sets[group] = act
-        return action_sets
-
-    def set_agent_refs(self, cur_node, cur_walker):
-        self.local_scope["here"] = cur_node
-        self.local_scope["visitor"] = cur_walker
-
-    def inherit_agent_refs(self, src_scope, src_node):  # used for calls of abilities
-        self.local_scope["here"] = src_node
-        self.local_scope["visitor"] = src_scope.local_scope["visitor"]
+    def set_refs(self, here, visitor):
+        self.local_scope["here"] = here
+        self.local_scope["visitor"] = visitor
+        self.action_sets = []
+        if here:
+            self.action_sets += [here.get_architype().get_all_abilities()]
+        if visitor:
+            self.action_sets += [visitor.get_architype().get_all_abilities()]
 
-    def get_aganet_refs(self):
+    def get_refs(self):
         return {
             "here": self.local_scope["here"],
             "visitor": self.local_scope["visitor"],
         }
 
+    def here(self):
+        return self.local_scope["here"]
+
+    def visitor(self):
+        return self.local_scope["visitor"]
+
     def find_live_attr(self, name, allow_read_only=True):
         """Finds binding for variable if not in standard scope"""
         # check if var is in walker's context
         if "context" in self.has_obj.__dict__ and name in self.has_obj.context.keys():
             return JacValue(self.parent, ctx=self.has_obj, name=name)
         elif name in self.action_sets.keys():
             return JacValue(self.parent, ctx=self.action_sets, name=name)
```

### Comparing `jaseci-1.4.0.9/jaseci/jac/machine/jac_value.py` & `jaseci-1.4.1.0/jaseci/jac/machine/jac_value.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 Variable manager for Jac
 
 Representations for all jac runtime variables
 """
-from jaseci.element.element import Element
-from jaseci.element.obj_mixins import Anchored
-from jaseci.graph.node import Node
-from jaseci.graph.edge import Edge
-from jaseci.graph.graph import Graph
+from jaseci.prim.element import Element
+from jaseci.prim.obj_mixins import Anchored
+from jaseci.prim.node import Node
+from jaseci.prim.edge import Edge
+from jaseci.prim.graph import Graph
 from jaseci.jac.jac_set import JacSet
 import uuid
 
 NoneType = type(None)
 
 
 class JacType:
@@ -156,15 +156,22 @@
         if value is not None:
             return value
         elif self.ctx is not None and self.name is not None:
             if self.end is not None:
                 return self.ctx[self.name : self.end]
             elif type(self.name) == int or self.name in self.ctx.keys():
                 return self.ctx[self.name]
-            elif not self.parent._assign_mode and not create_mode:
+            elif (
+                not self.parent._assign_mode
+                and not create_mode
+                and (
+                    not self.is_element
+                    or self.name not in self.is_element.get_architype().has_vars
+                )
+            ):
                 self.parent.rt_error(f"Key {self.name} not found in object/dict.")
         else:
             return None
 
     def write(self, jac_ast, force=False):
         if (
             not force
```

### Comparing `jaseci-1.4.0.9/jaseci/jac/machine/machine_state.py` & `jaseci-1.4.1.0/jaseci/jac/machine/machine_state.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,83 +2,147 @@
 Interpreter for jac code in AST form
 
 This interpreter should be inhereted from the class that manages state
 referenced through self.
 """
 from copy import copy
 from jaseci.utils.utils import logger
-from jaseci.actions.live_actions import live_actions, load_preconfig_actions
+from jaseci.jsorc.live_actions import live_actions, load_preconfig_actions
 
 # from jaseci.actions.find_action import find_action
-from jaseci.element.element import Element
+from jaseci.prim.element import Element
 
 from jaseci.jac.jac_set import JacSet
 from jaseci.jac.machine.jac_scope import JacScope
 from jaseci.utils.id_list import IdList
 from jaseci.jac.ir.ast import Ast
-from jaseci.graph.edge import Edge
-from jaseci.graph.node import Node
+from jaseci.prim.edge import Edge
+from jaseci.prim.node import Node
 from jaseci.jac.machine.jac_value import JacValue
 from jaseci.jac.jsci_vm.op_codes import JsCmp
+import time
 
 
 class MachineState:
     """Shared interpreter class across both sentinels and walkers"""
 
-    def __init__(self, parent_override=None, caller=None):
+    recur_detect_set = []
+    profile_stack = [None]
+
+    def __init__(self):
         self.report = []
         self.report_status = None
         self.report_custom = None
         self.request_context = None
         self.runtime_errors = []
         self.yielded_walkers_ids = IdList(self)
         self.ignore_node_ids = IdList(self)
-        self._parent_override = parent_override
-        if not isinstance(self, Element) and caller:
-            self._m_id = caller._m_id
-            self._h = caller._h
         self._scope_stack = [None]
         self._jac_scope = None
         self._relevant_edges = []
         self._loop_ctrl = None
         self._stopped = None
         self._assign_mode = False
         self._jac_try_mode = 0  # 0 is false, +=1 for each nested try
         self._loop_limit = 10000
         self._cur_jac_ast = Ast("none")
         self._write_candidate = None
+        self._mast = self.get_master()
+
         self.inform_hook()
 
     def inform_hook(self):
         if hasattr(self, "_h"):
             self._h._machine = self
 
-    def parent(self):  # parent here is always a sentinel
-        if self._parent_override:
-            return self._parent_override
-        else:
-            return Element.parent(self)
-
     def reset(self):
         self.report = []
         self.report_status = None
         self.report_custom = None
         self.runtime_errors = []
         self._scope_stack = [None]
         self._jac_scope = None
         self._loop_ctrl = None
         self._stopped = None
 
     def push_scope(self, scope: JacScope):
+        self.profile_pause()
         self._scope_stack.append(scope)
         self._jac_scope = scope
+        MachineState.profile_stack.append(self._jac_scope)
+        self.profile_in()
+        MachineState.recur_detect_set.append(self.call_name())
 
     def pop_scope(self):
+        MachineState.recur_detect_set.remove(self.call_name())
+        self.profile_out()
         self._scope_stack.pop()
         self._jac_scope = self._scope_stack[-1]
+        MachineState.profile_stack.pop()
+        self.profile_unpause()
+
+    def profile_in(self):
+        if self._mast and self._mast._profiling:
+            self._jac_scope._start_time = time.time()
+            self._jac_scope._cum_start_time = time.time()
+
+    def profile_out(self):
+        # profile_jac_scope = MachineState.profile_stack[-1]  # refactor and clean
+        if self._mast and self._mast._profiling:
+            name = self.call_name()
+            if name not in self._mast._jac_profile:
+                self._mast._jac_profile[name] = {
+                    "calls": 1,
+                    "u_calls": 0 if name in MachineState.recur_detect_set else 1,
+                    "tot_time": self._jac_scope._total_time
+                    + (time.time() - self._jac_scope._start_time),
+                    "cum_time": 0
+                    if name in MachineState.recur_detect_set
+                    else time.time() - self._jac_scope._cum_start_time,
+                }
+            else:
+                c = self._mast._jac_profile[name]["calls"]
+                u = self._mast._jac_profile[name]["u_calls"]
+                t = self._mast._jac_profile[name]["tot_time"]
+                p = self._mast._jac_profile[name]["cum_time"]
+                self._mast._jac_profile[name]["calls"] = c + 1
+                self._mast._jac_profile[name]["u_calls"] = (
+                    u if name in MachineState.recur_detect_set else u + 1
+                )
+                self._mast._jac_profile[name][
+                    "tot_time"
+                ] += self._jac_scope._total_time + (
+                    time.time() - self._jac_scope._start_time
+                )
+
+                self._mast._jac_profile[name]["cum_time"] = (
+                    p
+                    if name in MachineState.recur_detect_set
+                    else (p + time.time() - self._jac_scope._cum_start_time)
+                )
+
+    def call_name(self):
+        return f"{self.kind}::{self.name}:{self._jac_scope.name}"
+
+    def profile_pause(self):
+        _jac_scope = MachineState.profile_stack[-1]  # refactor and clean
+        if self._mast and self._mast._profiling and _jac_scope:
+            _jac_scope._total_time += time.time() - _jac_scope._start_time
+            _jac_scope._start_time = 0
+
+    def profile_unpause(self):
+        _jac_scope = MachineState.profile_stack[-1]  # refactor and clean
+        if self._mast and self._mast._profiling and _jac_scope:
+            _jac_scope._start_time = time.time()
+
+    def here(self):
+        return self._scope_stack[-1].here() if self._scope_stack[-1] else None
+
+    def visitor(self):
+        return self._scope_stack[-1].visitor() if self._scope_stack[-1] else None
 
     def set_cur_ast(self, jac_ast):
         self._cur_jac_ast = jac_ast
         return jac_ast.kid
 
     def destroy(self):
         """
@@ -160,15 +224,15 @@
 
     def edge_to_node_jac_set(self, edge_set, location=None):
         """
         Returns nodes jac_set from edge jac_set from current node
         """
         ret = JacSet()
         if not location:
-            location = self.current_node
+            location = self.here()
         for i in edge_set.obj_list():
             ret.add_obj(i.opposing_node(location))
         return ret
 
     def edges_filter_on_nodes(self, edge_set, node_set):
         """
         Returns nodes jac_set from edge jac_set from current node
```

### Comparing `jaseci-1.4.0.9/jaseci/jac/tests/book_code.py` & `jaseci-1.4.1.0/jaseci/jac/tests/book_code.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.0.9/jaseci/jac/tests/test_book.py` & `jaseci-1.4.1.0/jaseci/jac/tests/test_book.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import io
 import sys
 from unittest import TestCase
 
 import jaseci.jac.tests.book_code as jtc
-from jaseci.actor.sentinel import Sentinel
-from jaseci.graph.graph import Graph
-from jaseci.svc import MetaService
+from jaseci.prim.sentinel import Sentinel
+from jaseci.prim.graph import Graph
+from jaseci.jsorc.jsorc import JsOrc
 from jaseci.utils.utils import TestCaseHelper
 
 
 class JacBookTests(TestCaseHelper, TestCase):
     """Unit tests for Jac language"""
 
     def setUp(self):
         super().setUp()
-        self.sent = Sentinel(m_id=0, h=MetaService().build_hook())
+        self.sent = Sentinel(m_id=0, h=JsOrc.hook())
         self.gph = Graph(m_id=0, h=self.sent._h)
         self.old_stdout = sys.stdout
         self.new_stdout = io.StringIO()
         sys.stdout = self.new_stdout
 
     def tearDown(self):
         sys.stdout = self.old_stdout
```

### Comparing `jaseci-1.4.0.9/jaseci/jac/tests/test_lang_14.py` & `jaseci-1.4.1.0/jaseci/jac/tests/test_lang_14.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,18 +22,28 @@
 
     def test_kwargs(self):
         ret = self.call(
             self.mast,
             ["sentinel_register", {"code": self.load_jac("general.jac")}],
         )
         ret = self.call(self.mast, ["walker_run", {"name": "test_kwargs"}])
-        self.assertEqual(ret["report"][0].count("."), 4)
+        self.assertGreater(ret["report"][0].count("."), 2)
+        self.assertLess(ret["report"][0].count("."), 6)
         self.assertEqual(ret["report"][1], ret["report"][2])
         self.assertNotEqual(ret["report"][3], ret["report"][2])
 
     def test_multistring(self):
         ret = self.call(
             self.mast,
             ["sentinel_register", {"code": self.load_jac("general.jac")}],
         )
         ret = self.call(self.mast, ["walker_run", {"name": "multistring"}])
         self.assertEqual(ret["report"][0], "This is a multistring")
+
+    def test_free_ref_ifs(self):
+        ret = self.call(
+            self.mast,
+            ["sentinel_register", {"code": self.load_jac("free_refs.jac")}],
+        )
+        ret = self.call(self.mast, ["walker_run", {"name": "init"}])
+        self.assertEqual(ret["report"], [True, True])
+        self.assertEqual(ret["success"], True)
```

### Comparing `jaseci-1.4.0.9/jaseci/jsctl/book_tools.py` & `jaseci-1.4.1.0/jaseci/cli_tools/book_tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from jaseci.utils.utils import obj_class_cache, build_class_dict
-from jaseci.element.super_master import SuperMaster as Sm
+from jaseci.prim.super_master import SuperMaster as Sm
 from docstring_parser import parse
 from os.path import exists
 
 # from pprint import pformat
 from inspect import getdoc, signature
 import jaseci
 
@@ -67,18 +67,18 @@
             + " Actions in Jac}\\label{tab:"
             + act
             + "std}\\end{longtable}"
         )
         return clip
 
     def get_global_actions(self):
-        import jaseci.actions.standard as stdact
+        import jaseci.extens.act_lib as stdact
         import pkgutil
         from importlib.machinery import SourceFileLoader
-        from jaseci.actions.live_actions import live_actions
+        from jaseci.jsorc.live_actions import live_actions
 
         all_action_sets = []
         for importer, modname, ispkg in pkgutil.iter_modules(stdact.__path__):
             if not exists(stdact.__path__[0] + "/" + modname + ".py"):
                 continue
             mod = SourceFileLoader(
                 modname, stdact.__path__[0] + "/" + modname + ".py"
@@ -297,18 +297,18 @@
             + " Actions in Jac}\\label{tab:"
             + act
             + "std}\\end{longtable}"
         )
         return clip
 
     def get_global_actions(self):
-        import jaseci.actions.standard as stdact
+        import jaseci.extens.act_lib as stdact
         import pkgutil
         from importlib.machinery import SourceFileLoader
-        from jaseci.actions.live_actions import live_actions
+        from jaseci.jsorc.live_actions import live_actions
 
         all_action_sets = []
         for importer, modname, ispkg in pkgutil.iter_modules(stdact.__path__):
             if not exists(stdact.__path__[0] + "/" + modname + ".py"):
                 continue
             mod = SourceFileLoader(
                 modname, stdact.__path__[0] + "/" + modname + ".py"
```

### Comparing `jaseci-1.4.0.9/jaseci/jsctl/jsctl.py` & `jaseci-1.4.1.0/jaseci/cli_tools/jsctl.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,34 +2,35 @@
 Command line tool for Jaseci
 """
 
 import functools
 import json
 import os
 import pickle
-
+import webbrowser
 import click
 import requests
 from click_shell import shell
 from click.testing import CliRunner
 from jaseci import __version__
-from jaseci.element.super_master import SuperMaster
-from jaseci.svc import MetaService
+from jaseci.prim.super_master import SuperMaster
 from jaseci.utils.utils import copy_func
 from .book_tools import Book, modifiedBook
-from jaseci.utils.utils import logger, perf_test_start, perf_test_stop
+from jaseci.utils.utils import logger, perf_test_start, perf_test_stop, find_first_api
+from jaseci.jsorc.jsorc import JsOrc
+from prettytable import PrettyTable
 
 session = None
 
 
 def reset_state():
     global session
     session = {
         "filename": "js.session",
-        "user": [MetaService(run_svcs=False).build_super_master(name="admin")],
+        "user": [JsOrc.super_master(name="admin")],
         "mem-only": session["mem-only"] if session is not None else False,
         "connection": {"url": None, "token": None, "headers": None},
     }
     session["master"] = session["user"][0]
 
 
 reset_state()
@@ -79,25 +80,27 @@
 
 
 def remote_api_call(payload, api_name):
     """
     Constructs and issues call to remote server
     NOTE: Untested
     """
-    for i in SuperMaster.all_apis(None):
-        if api_name == "_".join(i["groups"]):
-            if i in SuperMaster._private_api:
-                path = "/js/" + api_name
-            elif i in SuperMaster._admin_api:
-                path = "/js_admin/" + api_name
-            elif i in SuperMaster._public_api:
-                path = "/js_public/" + api_name
-            break
-    ret = requests.post(
-        session["connection"]["url"] + path,
+    path, api = find_first_api(
+        api_name,
+        js_public=SuperMaster._public_api,
+        js=SuperMaster._private_api,
+        js_admin=SuperMaster._admin_api,
+    )
+
+    method = requests.post
+    if api["allowed_methods"] != None and "post" not in api["allowed_methods"]:
+        method = requests.get
+
+    ret = method(
+        session["connection"]["url"] + f"/{path}/{api_name}",
         json=payload,
         headers=session["connection"]["headers"],
     )
     if ret.status_code > 205:
         ret = f"Status Code Error {ret.status_code}\n{ret.json()}"
     else:
         ret = ret.json()
@@ -106,14 +109,47 @@
 
 def resolve_none_type(kwargs):
     for i in kwargs.keys():
         if kwargs[i] == "None":
             kwargs[i] = None
 
 
+def has_profile(output):
+    if isinstance(output, dict):
+        if "profile" in output.keys():
+            if "jac" in output["profile"].keys() and "perf" in output["profile"].keys():
+                return True
+    return False
+
+
+def gen_pretty_table(csv_str):
+    rows = csv_str.split("\n")
+    row_width = len(rows[0].split(","))
+    first_row = rows[0].split(",")
+    if first_row[2] == "percall":
+        first_row[2] = "percall_tot"
+    try:
+        table = PrettyTable(first_row)
+        for i in rows[1:]:
+            row = i.split(",")
+            if len(row) != row_width:
+                continue
+            table.add_row(row)
+        return table
+    except Exception as e:
+        click.echo(f"Something went wrong pretty printing profile: {e}")
+
+
+def pretty_profile(output):
+    click.echo("Jac Code Profile:")
+    click.echo(gen_pretty_table(output["profile"]["jac"]))
+    click.echo("\nInternal Jaseci Profile:")
+    click.echo(gen_pretty_table(output["profile"]["perf"]))
+
+
 def interface_api(api_name, is_public, is_cli_only, **kwargs):
     """
     Interfaces Master apis after processing arguments/parameters
     from cli
     """
     if "code" in kwargs and kwargs["code"]:
         if os.path.isfile(kwargs["code"]):
@@ -131,14 +167,15 @@
     resolve_none_type(kwargs)
     if not is_cli_only and is_connected():
         out = remote_api_call(kwargs, api_name)
     elif is_public:
         out = session["master"].public_interface_to_api(kwargs, api_name)
     else:
         out = session["master"].general_interface_to_api(kwargs, api_name)
+    d_out = out
     if (
         isinstance(out, dict)
         and "report_custom" in out.keys()
         and out["report_custom"] is not None
     ):
         out = out["report_custom"]
     if isinstance(out, dict) or isinstance(out, list):
@@ -147,14 +184,16 @@
     if "output" in kwargs and kwargs["output"]:
         with open(kwargs["output"], "w") as f:
             f.write(out)
         click.echo(f'[saved to {kwargs["output"]}]')
     if not session["mem-only"]:
         with open(session["filename"], "wb") as f:
             pickle.dump(session, f)
+    if has_profile(d_out):
+        pretty_profile(d_out)
 
 
 def extract_api_tree():
     """
     Generates a tree of command group names and function
     signatures in leaves from API function names in Master
     """
@@ -266,14 +305,44 @@
     else:
         click.echo("Login failed!\n")
     if not session["mem-only"]:
         with open(session["filename"], "wb") as f:
             pickle.dump(session, f)
 
 
+@click.command(help="Launch Jaseci Studio")
+def studio():
+    token = session["connection"]["token"]
+
+    if not token:
+        click.echo(
+            click.style(
+                "It doesn't look like you're logged in to a Jaseci instance. Please log in to a Jaseci instance to use this command.\n",
+                fg="red",
+            )
+        )
+    else:
+        url = session["connection"]["url"] + "/studio/"
+
+        if token == "PUBLIC":
+            click.echo(
+                click.style(
+                    "You are logged in as a public user. Please log in to a Jaseci instance to use this command.\n",
+                    fg="red",
+                )
+            )
+
+            webbrowser.open(url)
+        else:
+            click.echo(click.style("Launching Jaseci Studio...", fg="green"))
+            click.echo(click.style("URL: ", fg="green", bold=True) + url)
+            click.echo(click.style(f"Token: {token}", fg="green"))
+            webbrowser.open(url + "?token=" + token)
+
+
 @click.command(help="Command for unauthenticated log into live Jaseci server")
 @click.argument("url", type=str, required=True)
 def publogin(url):
     url = url[:-1] if url[-1] == "/" else url
     if requests.get(url).status_code <= 205:
         session["connection"]["token"] = "PUBLIC"
         session["connection"]["url"] = url
@@ -348,28 +417,30 @@
         return
     with open(filename) as file:
         cmds = [line.rstrip() for line in file]
     if output:
         with open(output, "w") as f:
             f.write("Multi Command Script Output:\n")
     for i in cmds:
-        res = CliRunner(mix_stderr=False).invoke(jsctl, i.split())
+        res = CliRunner(mix_stderr=False).invoke(jsctl, i)
         click.echo(res.stdout)
         if output:
             with open(output, "a") as f:
                 f.write(f"Output for {i}:\n")
                 f.write(res.stdout)
     if profile:
-        perf = perf_test_stop(prof)
+        perf, graph = perf_test_stop(prof)
         click.echo(perf)
+        click.echo(graph)
     if output:
         with open(output, "a") as f:
             if profile:
                 f.write(f"\nProfile:\n")
                 f.write(perf)
+                f.write(graph)
         click.echo(f"[saved to {output}]")
 
 
 @click.command(help="Internal book generation tools")
 @click.argument("op", type=str, default="cheatsheet", required=True)
 @click.option(
     "--output",
@@ -404,14 +475,15 @@
 jsctl.add_command(publogin)
 jsctl.add_command(logout)
 jsctl.add_command(edit)
 jsctl.add_command(ls)
 jsctl.add_command(clear)
 jsctl.add_command(reset)
 jsctl.add_command(script)
+jsctl.add_command(studio)
 jsctl.add_command(booktool)
 cmd_tree_builder(extract_api_tree())
 cmd_tree_builder(extract_api_tree()["jac"], group_func=jac)
 
 
 def main():
     jsctl()
```

### Comparing `jaseci-1.4.0.9/jaseci/jsctl/tests/test_jsctl.py` & `jaseci-1.4.1.0/jaseci/cli_tools/tests/test_jsctl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 from unittest import TestCase
 from jaseci.utils.utils import TestCaseHelper
-from jaseci.jsctl import jsctl
+from jaseci.cli_tools import jsctl
 from click.testing import CliRunner
 import json
 import os
 
+from jaseci.jsorc.jsorc import JsOrc
+from jaseci.extens.svc.redis_svc import RedisService
+
 
 class JsctlTest(TestCaseHelper, TestCase):
     """Unit tests for Jac language"""
 
     infer_loc = (
         os.path.dirname(os.path.dirname(os.path.dirname(__file__))) + "/tests/infer.py"
     )
 
     def setUp(self):
         super().setUp()
+        JsOrc.svc("redis", RedisService).clear()
 
     def call(self, cmd: str):
         res = CliRunner(mix_stderr=False).invoke(jsctl.jsctl, ["-m"] + cmd.split())
         # self.log(res.stdout)
         # self.log(res.stderr)
         # self.log(res.exception)
         return res.stdout
@@ -150,14 +154,15 @@
         self.call("config set APPLE -value Grape2 -do_check False")
         self.call("config set APPLE_JSON -value '{\"test\":true}' -do_check False")
         self.call('config set "Banana" -value "Grape" -do_check False')
         self.call('config set "Pear" -value "Banana" -do_check False')
         r = self.call("config get APPLE -do_check False")
         self.assertEqual(r.strip(), "Grape2")
         r = self.call_cast("config list")
+
         self.assertEqual(len(r), 1)
 
     def test_jsctl_default_snt_setting(self):
         """Tests that alias mapping api works"""
         self.call(
             f"sentinel register {os.path.dirname(__file__)}/teststest.jac -name zsb "
             "-set_active true"
@@ -412,14 +417,23 @@
         r = self.call(
             f"sentinel register "
             f"{os.path.dirname(__file__)}/graph_can.jac -name gc -set_active true"
         )
         r = self.call("walker run go")
         self.assertEqual(r.split()[0], "2020-01-01T00:00:00")
 
+    def test_jsctl_action_call(self):
+        self.call(f"actions load local {self.infer_loc}")
+        r = self.call(f"actions call infer.date_now")
+        r = json.loads(r)
+        import datetime
+
+        date_now = datetime.datetime.utcnow().date().isoformat()
+        self.assertEqual(r["result"], date_now)
+
     def test_jsctl_custom_report(self):
         self.call(
             f"sentinel register {os.path.dirname(__file__)}/glob_imp.jac -set_active true"
         )
         r = self.call_cast("walker run cust_report")
         self.assertEqual(r, {"a": "b"})
 
@@ -488,14 +502,25 @@
                 "Output for graph list:",
                 "[]",
                 "Output for alias list:",
                 "{}",
             ],
         )
 
+    def test_jsctl_pretty_profiles(self):
+        self.call(f"actions load local {self.infer_loc}")
+        r = self.call(
+            f"sentinel register "
+            f"{os.path.dirname(__file__)}/graph_can.jac -name gc -set_active true"
+        )
+        r = self.call("walker run go -profiling true")
+        self.assertIn("walker::go", r)
+        self.assertIn("cumtime", r)
+        self.assertIn("cum_time", r)
+
 
 class JsctlTestWithSession(TestCaseHelper, TestCase):
     """Unit tests for Jac language"""
 
     def setUp(self):
         super().setUp()
```

### Comparing `jaseci-1.4.0.9/jaseci/svc/actions_optimizer/actions_optimizer.py` & `jaseci-1.4.1.0/jaseci/utils/actions/actions_optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,73 +1,66 @@
 """
 Module that manage and optimizes the actions configuration of Jaseci
 """
-
-from jaseci.actions.remote_actions import ACTIONS_SPEC_LOC
+from jaseci.jsorc.jsorc import JsOrc
+from jaseci.extens.svc.kube_svc import KubeService
+from jaseci.jsorc.remote_actions import ACTIONS_SPEC_LOC
 from jaseci.utils.utils import logger
-from jaseci.svc.actions_optimizer.actions_state import ActionsState
-from jaseci.actions.live_actions import (
+from jaseci.jsorc.live_actions import (
     load_module_actions,
     unload_module,
     unload_remote_actions,
     load_remote_actions,
     live_actions,
     action_configs,
 )
+
 import requests
 import copy
 import time
-from kubernetes.client.rest import ApiException
+
+from .actions_state import ActionsState
 
 POLICIES = ["Default", "Evaluation"]
+THRESHOLD = 0.2
+NODE_MEM_THRESHOLD = 0.8
 
 
 class ActionsOptimizer:
     def __init__(
         self,
-        kube=None,
         namespace: str = "default",
         policy: str = "Default",
         benchmark: dict = {},
         actions_history: dict = {},
         actions_calls: dict = {},
     ) -> None:
-        self.kube = kube
         self.actions_state = ActionsState()
         self.actions_change = {}
         self.jsorc_interval = 0
         self.namespace = namespace
         self.policy = policy
         self.benchmark = benchmark
         self.actions_history = actions_history
         self.actions_calls = actions_calls
         self.policy_params = {}
         self.policy_state = {}
+        self.last_eval_configs = []
 
     def kube_create(self, config):
+        kube = JsOrc.svc("kube").poke(cast=KubeService)
         for kind, conf in config.items():
             name = conf["metadata"]["name"]
-            try:
-                self.kube.create(kind, self.namespace, conf)
-            except ApiException:
-                logger.error(f"Error creating {kind} for {name}")
+            kube.create(kind, name, conf, kube.namespace, "ActionsOptimzer:")
 
     def kube_delete(self, config):
+        kube = JsOrc.svc("kube").poke(cast=KubeService)
         for kind, conf in config.items():
             name = conf["metadata"]["name"]
-            try:
-                logger.info(
-                    f"ActionsOptimzer: deleting {kind} for {name} for namespace {self.namespace}"
-                )
-                self.kube.delete(kind, name, self.namespace)
-            except ApiException as e:
-                logger.error(
-                    f"Error deleting {kind} for {name} for namespace {self.namespace}"
-                )
-                logger.error(str(e))
+            kube.delete(kind, name, kube.namespace, "ActionsOptimzer:")
 
     def get_actions_status(self, name=""):
         """
         Return the state of action
         """
         if name == "":
             return self.actions_state.get_all_state()
@@ -103,15 +96,16 @@
         Any action preparation that needs to be called right after action is loaded
         """
         pass
 
     def load_action_remote(self, name, unload_existing=False):
         """
         Load a remote action.
-        JSORC will get the URL of the remote microservice and stand up a microservice if there isn't currently one in the cluster.
+        JSORC will get the URL of the remote microservice
+        and stand up a microservice if there isn't currently one in the cluster.
         Return True if the remote action is loaded successfully,
         False otherwise
         """
         cur_state = self.actions_state.get_state(name)
         if cur_state is None:
             cur_state = self.actions_state.init_state(name)
 
@@ -143,18 +137,20 @@
         return False
 
     def load_action_module(self, name, unload_existing=False):
         """
         Load an action module
         """
         cur_state = self.actions_state.get_state(name)
+        logger.info(cur_state)
         if cur_state is None:
             cur_state = self.actions_state.init_state(name)
 
         if cur_state["mode"] == "module":
+            logger.info("ALREADY A MODULE LOADED")
             # Check if there is already a local action loaded
             return
 
         if name not in action_configs:
             return
 
         module = action_configs[name]["module"]
@@ -263,15 +259,14 @@
         """
         self.jsorc_interval = jsorc_interval
         if self.policy == "Default":
             # Default policy does not manage action automatically
             return
         elif self.policy == "Evaluation":
             self._actionpolicy_evaluation()
-
         if len(self.actions_change) > 0:
             self.apply_actions_change()
 
     def _init_evalution_policy(self, policy_state):
         # 999 is just really large memory size so everything can fits in local
         node_mem = self.policy_params.get("node_mem", 999 * 1024)
         jaseci_runtime_mem = self.policy_params.get("jaseci_runtime_mem", 300)
@@ -282,17 +277,24 @@
         for act in actions:
             new_configs = []
             for con in all_configs:
                 for m in ["local", "remote"]:
                     c = copy.deepcopy(con)
                     c[act] = m
                     if m == "local":
-                        c["local_mem"] += action_configs[act].get("remote_memory", 0)
-                        if c["local_mem"] < node_mem:
+                        local_mem_requirement = action_configs[act][
+                            "local_mem_requirement"
+                        ]
+                        c["local_mem"] = c["local_mem"] + local_mem_requirement
+                        if c["local_mem"] < (node_mem * NODE_MEM_THRESHOLD):
                             new_configs.append(dict(c))
+                        else:
+                            logger.info(
+                                f"config dropped for memory constraint: {c},\n\tcurrent node memory: {node_mem}\n\tavailable memory: {(node_mem * NODE_MEM_THRESHOLD)-c['local_mem'] }"
+                            )
                     else:
                         new_configs.append(dict(c))
             all_configs = list(new_configs)
         policy_state["remain_configs"] = all_configs
 
     def _actionpolicy_evaluation(self):
         """
@@ -306,16 +308,20 @@
         if len(policy_state) == 0:
             # Initialize policy tracking state
             policy_state = {
                 "phase": "eval",  # current phase of policy: eval|perf
                 "cur_config": None,  # current active configuration
                 "remain_configs": [],  # remaining configurations that need to be evaluated
                 "past_configs": [],  # configurations already evaluated
-                "eval_phase": 10,  # how long is evaluatin period (in seconds)
-                "perf_phase": 100,  # how long is the performance period (in seconds)
+                "eval_phase": self.policy_params.get(
+                    "eval_phase", 10
+                ),  # how long is evaluatin period (in seconds)
+                "perf_phase": self.policy_params.get(
+                    "perf_phase", 100
+                ),  # how long is the performance period (in seconds)
                 "cur_phase": 0,  # how long the current period has been running
                 "prev_best_config": self.actions_state.get_all_state(),
             }
         policy_state["cur_phase"] += self.jsorc_interval
 
         # check if we should go into evaluation phase
         if (
@@ -440,15 +446,14 @@
                 logger.info(
                     f"===Evaluation Policy=== All actions change have been applied. Start evaluation phase."
                 )
                 policy_state["phase"] = "eval"
                 policy_state["cur_phase"] = 0
                 self.benchmark["active"] = True
                 self.benchmark["requests"] = {}
-
         self.policy_state["Evaluation"] = policy_state
 
     def _get_action_change(self, new_action_state):
         """
         Given a new desired action state and the current action_state tracking, return the change set
         """
         change_state = {}
@@ -472,15 +477,15 @@
         Apply any action configuration changes
         """
         actions_change = dict(self.actions_change)
         # For now, to_* and *_to_* are the same logic
         # But this might change down the line
         for name, change_type in actions_change.items():
             logger.info(f"==Actions Optimizer== Changing {name} {change_type}")
-            if change_type == "to_local" or change_type == "to_module":
+            if change_type in ["to_local", "_to_local", "_to_module", "to_module"]:
                 # Switching from no action loaded to local
                 self.load_action_module(name)
                 del self.actions_change[name]
             elif change_type == "to_remote":
                 loaded = self.load_action_remote(name)
                 if loaded:
                     del self.actions_change[name]
```

### Comparing `jaseci-1.4.0.9/jaseci/svc/actions_optimizer/actions_state.py` & `jaseci-1.4.1.0/jaseci/utils/actions/actions_state.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.0.9/jaseci/svc/jsorc-backup/jaseci-redis.yaml` & `jaseci-1.4.1.0/jaseci/jsorc/manifests/redis.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,25 @@
+apiVersion: v1
+kind: Service
+metadata:
+  name: jaseci-redis
+  namespace: redis
+spec:
+  selector:
+    pod: jaseci-redis
+  ports:
+    - protocol: TCP
+      port: 6379
+      targetPort: 6379
 ---
 apiVersion: apps/v1
 kind: Deployment
 metadata:
   name: jaseci-redis
+  namespace: redis
 spec:
   replicas: 1
   selector:
     matchLabels:
       pod: jaseci-redis
   template:
     metadata:
@@ -35,7 +48,17 @@
           emptyDir: {}
         - name: config
           configMap:
             name: jaseci-redis-config
             items:
               - key: redis-config
                 path: redis.conf
+---
+apiVersion: v1
+kind: ConfigMap
+metadata:
+  name: jaseci-redis-config
+  namespace: redis
+data:
+  redis-config: |
+    maxmemory 1000mb
+    maxmemory-policy allkeys-lru
```

### Comparing `jaseci-1.4.0.9/jaseci/svc/mail/mail.py` & `jaseci-1.4.1.0/jaseci/extens/svc/mail_svc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import ssl
+from json import dumps
 from email.mime.multipart import MIMEMultipart
 from email.mime.text import MIMEText
-from json import dumps
 from smtplib import SMTP, SMTP_SSL
 
-from jaseci.svc import CommonService
-from .config import MAIL_CONFIG
+from jaseci.jsorc.jsorc import JsOrc
 
 
 #################################################
-#                  EMAIL APP                   #
+#                   EMAIL APP                   #
 #################################################
 
 
-class MailService(CommonService):
+@JsOrc.service(name="mail", config="MAIL_CONFIG")
+class MailService(JsOrc.CommonService):
     ###################################################
     #                     BUILDER                     #
     ###################################################
 
-    def run(self, hook=None):
-        self.__convert_config(hook)
+    def run(self):
+        self.__convert_config()
         self.app = self.connect()
 
     # ----------- BACKWARD COMPATIBILITY ------------ #
     # ---------------- TO BE REMOVED ---------------- #
 
     def __convert(self, hook, holder, mapping: dict):
         for k, v in mapping.items():
@@ -32,15 +32,16 @@
                 if not (conf is None):
                     if v == "tls":
                         holder[v] = conf.lower() == "true"
                     else:
                         holder[v] = conf
         return holder
 
-    def __convert_config(self, hook):
+    def __convert_config(self):
+        hook = JsOrc.hook()
         version = self.config.get("version", 2)
         migrate = self.config.get("migrate", False)
         if version == 1 or migrate:
             self.__convert(
                 hook,
                 self.config,
                 {
@@ -67,27 +68,40 @@
                     "EMAIL_RESETPASS_SUBJ": "resetpass_subj",
                     "EMAIL_RESETPASS_BODY": "resetpass_body",
                     "EMAIL_RESETPASS_HTML_BODY": "resetpass_html_body",
                 },
             )
 
             if migrate:
-                self.config["migrate"] = False
-                hook.save_glob("MAIL_CONFIG", dumps(self.config))
+                hook.save_glob(
+                    "MAIL_CONFIG",
+                    dumps(
+                        {
+                            **{
+                                "enabled": self.enabled,
+                                "quiet": self.quiet,
+                                "automated": self.automated,
+                            },
+                            **self.config,
+                            "migrate": False,
+                        }
+                    ),
+                )
+                hook.commit()
 
     ###################################################
     #                     CLEANER                     #
     ###################################################
 
-    def reset(self, hook, start=True):
+    # ---------------- PROXY EVENTS ----------------- #
+
+    def on_delete(self):
         if self.is_running():
             self.app.terminate()
 
-        super().reset(hook, start)
-
     ####################################################
     #                    OVERRIDDEN                    #
     ####################################################
 
     def connect(self):
         host = self.config.get("host")
         port = self.config.get("port")
@@ -105,28 +119,24 @@
         else:
             server = SMTP_SSL(host, port, context=context)
 
         server.login(user, _pass)
 
         return Mailer(server, sender)
 
-    def build_config(self, hook) -> dict:
-        return hook.service_glob("MAIL_CONFIG", MAIL_CONFIG)
-
 
 # ----------------------------------------------- #
 
-
 ####################################################
-#                   EMAIL CONFIG                   #
+#                      MAILER                      #
 ####################################################
 
 
 class Mailer:
-    def __init__(self, server, sender):
+    def __init__(self, server: SMTP, sender):
         self.server = server
         self.sender = sender
 
     def send_custom_email(
         self,
         sender: str = None,
         recipients: list = [],
```

### Comparing `jaseci-1.4.0.9/jaseci/svc/prometheus/prometheus.py` & `jaseci-1.4.1.0/jaseci/extens/svc/prome_svc.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,28 @@
-from prometheus_api_client import PrometheusConnect
-from jaseci.svc import CommonService
-from .config import PROMON_CONFIG
-from .manifest import PROMON_MANIFEST
 import time
+from prometheus_api_client import PrometheusConnect
+from jaseci.jsorc.jsorc import JsOrc
+
+
+class MetricValue:
+    node = None
+    pod = None
+
+    def __init__(self, _node: dict, _pod: dict):
+        self.node = _node
+        self.pod = _pod
 
 
-class PrometheusService(CommonService):
+@JsOrc.service(name="prome", config="PROME_CONFIG", manifest="PROME_MANIFEST")
+class PrometheusService(JsOrc.CommonService):
     ###################################################
     #                     BUILDER                     #
     ###################################################
 
-    def run(self, hook=None):
+    def run(self):
         self.app = PrometheusConnect(url=self.config.get("url"), disable_ssl=True)
         self.ping()
         self.cpu = Cpu(self.app)
         self.memory = Memory(self.app)
         self.network = Network(self.app)
         self.disk = Disk(self.app)
 
@@ -50,28 +58,66 @@
             if exclude_prom and "prometheus" in pod:
                 continue
             if res.get(node) is None:
                 res[node] = []
             res[node].append(pod)
         return res
 
-    def info(
+    def node_info(
+        self,
+        namespace: str = "",
+        exclude_prom: bool = False,
+        timestamp: int = 0,
+        duration: int = 0,
+    ) -> dict:
+        if namespace == "":
+            util = self.app.get_current_metric_value("kube_node_info")
+        else:
+            util = self.app.get_current_metric_value(
+                f"kube_node_info{{namespace='{namespace}'}}"
+            )
+
+        res = {}
+        disk_read = self.disk.read()
+        disk_write = self.disk.write()
+
+        node_names = [nodes["metric"]["node"] for nodes in util]
+
+        for node_name in node_names:
+            res[node_name] = {}
+
+        for node_name in node_names:
+            res[node_name]["disk_read_bytes"] = disk_read.get(node_name, 0)
+
+        for node_name in node_names:
+            res[node_name]["disk_write_bytes"] = disk_write.get(node_name, 0)
+
+        return res
+
+    def pod_info(
         self,
         namespace: str = "",
         exclude_prom: bool = False,
         timestamp: int = 0,
         duration: int = 0,
     ) -> dict:
         if namespace == "":
             util = self.app.get_current_metric_value("kube_pod_info")
         else:
             util = self.app.get_current_metric_value(
                 f"kube_pod_info{{namespace='{namespace}'}}"
             )
+
         res = {}
+
+        for pod in util:
+            pod_name = pod["metric"]["pod"]
+            if exclude_prom and "prometheus" in pod_name:
+                continue
+
         for pod in util:
             pod_name = pod["metric"]["pod"]
             if exclude_prom and "prometheus" in pod_name:
                 continue
             # res[pod_name] = pod["metric"]
             res[pod_name] = {}
 
@@ -82,14 +128,25 @@
         for pod in util:
             pod_name = pod["metric"]["pod"]
             if exclude_prom and "prometheus" in pod_name:
                 continue
             pod_cpu = cpu.get(pod_name, 0)
 
             res[pod_name]["cpu_utilization_cores"] = pod_cpu
+        if timestamp != 0 and duration != 0:
+            cpu = self.cpu.utilization_per_pod_cores(ts=timestamp, duration=duration)
+        else:
+            cpu = self.cpu.utilization_per_pod_cores()
+        for pod in util:
+            pod_name = pod["metric"]["pod"]
+            if exclude_prom and "prometheus" in pod_name:
+                continue
+            pod_cpu = cpu.get(pod_name, 0)
+
+            res[pod_name]["cpu_utilization_cores"] = pod_cpu
 
         mem = self.memory.utilization_per_pod_bytes()
         for pod in util:
             pod_name = pod["metric"]["pod"]
             pod_mem = mem.get(pod_name, 0)
             res[pod_name]["mem_utilization_bytes"] = pod_mem
 
@@ -113,23 +170,34 @@
             if exclude_prom and "prometheus" in pod_name:
                 continue
             pod_tran = tran.get(pod_name, 0)
             res[pod_name]["network_tran_bytes"] = pod_tran
 
         return res
 
-    ####################################################
-    #                    OVERRIDDEN                    #
-    ####################################################
-
-    def build_config(self, hook) -> dict:
-        return hook.service_glob("PROMON_CONFIG", PROMON_CONFIG)
-
-    def build_manifest(self, hook) -> dict:
-        return hook.service_glob("PROMON_MANIFEST", PROMON_MANIFEST)
+    def info(
+        self,
+        namespace: str = "",
+        exclude_prom: bool = False,
+        timestamp: int = 0,
+        duration: int = 0,
+    ) -> MetricValue:
+        node_value = self.node_info(
+            namespace=namespace,
+            exclude_prom=exclude_prom,
+            timestamp=timestamp,
+            duration=duration,
+        )
+        pod_value = self.pod_info(
+            namespace=namespace,
+            exclude_prom=exclude_prom,
+            timestamp=timestamp,
+            duration=duration,
+        )
+        return MetricValue(_node=node_value, _pod=pod_value)
 
 
 class Info:
     def __init__(self, app):
         self.app = app
 
 
@@ -282,7 +350,29 @@
         )
         res = {}
         for node in util:
             node_name = node["metric"]["node"]
             node_util = float(node["value"][1])
             res[node_name] = node_util
         return res
+
+    def read(self) -> dict:
+        util = self.app.get_current_metric_value(
+            "sum (rate (node_disk_read_bytes_total{}[10m])) by (node)"
+        )
+        res = {}
+        for node in util:
+            node_name = node["metric"]["node"]
+            node_util = float(node["value"][1])
+            res[node_name] = node_util
+        return res
+
+    def write(self) -> dict:
+        util = self.app.get_current_metric_value(
+            "sum (rate (node_disk_written_bytes_total{}[10m])) by (node)"
+        )
+        res = {}
+        for node in util:
+            node_name = node["metric"]["node"]
+            node_util = float(node["value"][1])
+            res[node_name] = node_util
+        return res
```

### Comparing `jaseci-1.4.0.9/jaseci/svc/redis/redis.py` & `jaseci-1.4.1.0/jaseci/extens/svc/redis_svc.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,20 @@
+from jaseci.jsorc.jsorc import JsOrc
 from redis import Redis
 
-from jaseci.svc import CommonService
-from .config import REDIS_CONFIG
-from .manifest import REDIS_MANIFEST
 
-
-#################################################
-#                  REDIS HOOK                   #
-#################################################
-
-
-class RedisService(CommonService):
-    ###################################################
-    #                     BUILDER                     #
-    ###################################################
-
-    def run(self, hook=None):
+@JsOrc.service(
+    name="redis",
+    config="REDIS_CONFIG",
+    manifest="REDIS_MANIFEST",
+    priority=0,
+    proxy=True,
+)
+class RedisService(JsOrc.CommonService):
+    def run(self):
         self.app = Redis(**self.config, decode_responses=True)
         self.app.ping()
 
     ###################################################
     #                     COMMONS                     #
     ###################################################
 
@@ -54,19 +49,12 @@
     #                     CLEANER                     #
     ###################################################
 
     def clear(self):
         if self.is_running():
             self.app.flushdb()
 
-    ###################################################
-    #                     CONFIG                      #
-    ###################################################
-
-    def build_config(self, hook) -> dict:
-        return hook.service_glob("REDIS_CONFIG", REDIS_CONFIG)
+    # ---------------- PROXY EVENTS ----------------- #
 
-    def build_manifest(self, hook) -> dict:
-        return hook.service_glob("REDIS_MANIFEST", REDIS_MANIFEST)
-
-
-# ----------------------------------------------- #
+    def on_delete(self):
+        if self.is_running():
+            self.app.close()
```

### Comparing `jaseci-1.4.0.9/jaseci/svc/stripe/stripe.py` & `jaseci-1.4.1.0/jaseci/extens/svc/stripe_svc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import stripe
-from jaseci.svc import CommonService
-from .config import STRIPE_CONFIG
+from jaseci.jsorc.jsorc import JsOrc
 
 #################################################
 #                  STRIPE APP                   #
 #################################################
 
 
-class StripeService(CommonService):
+@JsOrc.service("stripe", config="STRIPE_CONFIG")
+class StripeService(JsOrc.CommonService):
     ###################################################
     #                     BUILDER                     #
     ###################################################
 
-    def run(self, hook=None):
+    def run(self):
         self.app = stripe
         if not self.config.get("api_key"):
             raise Exception("api_key is required!")
         self.app.api_key = self.config.get("api_key")
 
         if not self.config.get("webhook_key"):
             raise Exception("webhook_key is required!")
@@ -45,10 +45,7 @@
     ####################################################
     #                    OVERRIDDEN                    #
     ####################################################
 
     def reset(self, hook, start=True):
         stripe.api_key = None
         super().reset(hook, start)
-
-    def build_config(self, hook) -> dict:
-        return hook.service_glob("STRIPE_CONFIG", STRIPE_CONFIG)
```

### Comparing `jaseci-1.4.0.9/jaseci/svc/task/common.py` & `jaseci-1.4.1.0/jaseci/extens/svc/tasks.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,293 +1,293 @@
-import re
-from copy import deepcopy
-from typing import Tuple
-from uuid import UUID
-
-from celery import Task
-from jaseci.svc.task.config import DEFAULT_MSG
-from requests import get, post
-from requests.exceptions import HTTPError
-
-
-class Queue(Task):
-    def run(self, wlk, nd, args):
-        from jaseci.svc import MetaService
-
-        hook = MetaService().build_hook()
-
-        wlk = hook.get_obj_from_store(wlk)
-        wlk._to_await = True
-
-        nd = hook.get_obj_from_store(nd)
-        resp = wlk.run(nd, *args)
-        wlk.destroy()
-
-        return {"anchor": wlk.anchor_value(), "response": resp}
-
-
-class ScheduledWalker(Task):
-    def get_obj(self, jid):
-        return self.hook.get_obj_from_store(jid)
-
-    def run(self, name, ctx, nd=None, snt=None, mst=None):
-        from jaseci.svc import MetaService
-
-        self.hook = MetaService().build_hook()
-
-        if mst:
-            mst = self.get_obj(mst)
-        else:
-            return f"{DEFAULT_MSG} mst (Master) is required!"
-
-        if mst is None:
-            return f"{DEFAULT_MSG} Invalid Master!"
-
-        try:
-            if not snt:
-                if mst.active_snt_id == "global":
-                    global_snt_id = self.hook.get_glob("GLOB_SENTINEL")
-                    snt = self.get_obj(global_snt_id)
-                elif mst.active_snt_id:
-                    snt = self.get_obj(mst.active_snt_id)
-            elif snt in mst.alias_map:
-                snt = self.get_obj(mst.alias_map[snt])
-            else:
-                snt = self.get_obj(snt)
-
-            if not snt:
-                return f"{DEFAULT_MSG} Invalid Sentinel!"
-
-            if not nd:
-                if mst.active_gph_id:
-                    nd = self.get_obj(mst.active_gph_id)
-            elif nd in mst.alias_map:
-                nd = self.get_obj(mst.alias_map[nd])
-            else:
-                nd = self.get_obj(nd)
-
-            if not nd:
-                return f"{DEFAULT_MSG} Invalid Node!"
-
-            return mst.walker_run(name, nd, ctx, ctx, snt, False, False)
-        except Exception as e:
-            return f"{DEFAULT_MSG} Error occured: {e}"
-
-
-class ScheduledSequence(Task):
-    json_escape = re.compile(r"[^a-zA-Z0-9_]")
-    internal = re.compile(r"\(([a-zA-Z0-9_\.\[\]\$\#\@\!]*?)\)")
-    full = re.compile(r"^\{\{([a-zA-Z0-9_\.\[\]\$\#\(\)\@\!]*?)\}\}$")
-    partial = re.compile(r"\{\{([a-zA-Z0-9_\.\[\]\$\#\(\)\@\!]*?)\}\}")
-
-    def get_deep_value(self, data, keys, default):
-        if len(keys) == 0:
-            return data
-
-        key = keys.pop(0)
-        t = type(data)
-
-        if t is dict and key in data:
-            return self.get_deep_value(data[key], keys, default)
-        elif t is list and key.isnumeric():
-            return self.get_deep_value(data[int(key)], keys, default)
-        else:
-            return default
-
-    def get_value(self, holder: Tuple, keys: str, default=None):
-        while self.internal.search(keys):
-            for intern in self.internal.findall(keys):
-                keys = keys.replace(
-                    "(" + intern + ")", self.get_value(holder, intern, "")
-                )
-
-        if keys:
-            keys = keys.split(".")
-            key = keys.pop(0)
-            if key == "#":
-                return self.get_deep_value(holder[0], keys, default)
-            elif key == "$":
-                t = type(holder[1])
-                if t is dict or t is list:
-                    return self.get_deep_value(holder[1], keys, default)
-                else:
-                    return holder[1]
-            elif key == "@":
-                t = type(holder[2])
-                if t is dict or t is list:
-                    return self.get_deep_value(holder[2], keys, default)
-                else:
-                    return holder[2]
-            elif key == "!":
-                return holder[3]
-        return default
-
-    def compare(self, condition, expected, actual):
-        if condition == "eq":
-            return actual == expected
-        elif condition == "ne":
-            return actual != expected
-        elif condition == "gt":
-            return actual > expected
-        elif condition == "gte":
-            return actual >= expected
-        elif condition == "lt":
-            return actual < expected
-        elif condition == "lte":
-            return actual <= expected
-        elif condition == "regex":
-            return re.compile(expected).match(actual)
-
-    def condition(self, holder: Tuple, filter):
-        for cons in filter["condition"].keys():
-            if not (filter["condition"][cons] is None) and not self.compare(
-                cons, filter["condition"][cons], self.get_value(holder, filter["by"])
-            ):
-                return False
-        return True
-
-    def or_condition(self, holder: Tuple, filter):
-        for filt in filter:
-            if "condition" in filt and self.condition(holder, filt):
-                return True
-            elif "or" in filt and self.or_condition(holder, filt["or"]):
-                return True
-            elif "and" in filt and self.and_condition(holder, filt["and"]):
-                return True
-        return False
-
-    def and_condition(self, holder: Tuple, filter):
-        for filt in filter:
-            if "condition" in filt and not self.condition(holder, filt):
-                return False
-            elif "or" in filt and not self.or_condition(holder, filt["or"]):
-                return False
-            elif "and" in filt and not self.and_condition(holder, filt["and"]):
-                return False
-        return True
-
-    def deep_replace_str(self, holder: Tuple, data, key):
-        matcher = self.full.match(data[key])
-        if matcher:
-            data[key] = self.get_value(holder, matcher.group(1))
-        else:
-            for rep in self.partial.findall(data[key]):
-                data[key] = data[key].replace(
-                    "{{" + rep + "}}", self.get_value(holder, rep, "")
-                )
-
-    def deep_replace_dict(self, holder: Tuple, data):
-        for key in data.keys():
-            if key != "__def_loop__":
-                t = type(data[key])
-                if t is str:
-                    self.deep_replace_str(holder, data, key)
-                elif t is dict:
-                    self.deep_replace_dict(holder, data[key])
-
-    def save(self, holder: Tuple, req, params):
-        if params in req:
-            holder[0][self.json_escape.sub("_", req[params])] = holder[1]
-
-    def trigger_interface(self, req: dict):
-        from jaseci.svc import MetaService
-
-        master = req.get("master")
-        app = MetaService()
-        if master is None:
-            caller = app.build_master()
-            trigger_type = "public"
-        else:
-            caller = app.build_hook().get_obj_from_store(master)
-            trigger_type = "general"
-
-        api = req.get("api")
-        body = req.get("body", {})
-
-        return getattr(caller, f"{trigger_type}_interface_to_api")(body, api)
-
-    def run(self, *args, **kwargs):
-        requests = kwargs.get("requests")
-        persistence = kwargs.get("persistence", {})
-        container = kwargs.get("container", {"current": persistence})
-        index = container.get("index", "0")
-
-        if "parent_current" in container:
-            container["current"] = container["parent_current"]
-
-        for req in requests:
-            try:
-                self.deep_replace_dict(
-                    (
-                        persistence,
-                        container["current"],
-                        container.get("parent_current", {}),
-                        index,
-                    ),
-                    req,
-                )
-                self.save((persistence, req), req, "save_req_to")
-
-                method = req["method"].upper()
-
-                if method == "JAC":
-                    container["current"] = self.trigger_interface(req)
-                else:
-                    if method == "POST":
-                        response = post(
-                            req["api"],
-                            json=req.get("body", {}),
-                            headers=req.get("header", {}),
-                        )
-                    elif method == "GET":
-                        response = get(req["api"], headers=req.get("header", {}))
-                    response.raise_for_status()
-                    if "application/json" in response.headers.get("Content-Type"):
-                        container["current"] = response.json()
-                    else:
-                        container["current"] = response.text
-
-                if "__def_loop__" in req:
-                    def_loop = req["__def_loop__"]
-                    for idx, loop in enumerate(
-                        self.get_value(
-                            (persistence, container["current"]), def_loop["by"], []
-                        )
-                    ):
-                        if "filter" in def_loop and not self.and_condition(
-                            (persistence, loop), def_loop["filter"]
-                        ):
-                            continue
-                        loop_container = {"parent_current": loop, "index": str(idx)}
-                        self.run(
-                            requests=deepcopy(def_loop["requests"]),
-                            persistence=persistence,
-                            container=loop_container,
-                        )
-
-                self.save((persistence, container["current"]), req, "save_to")
-
-            except Exception as err:
-                container["current"] = (
-                    {
-                        "status": err.response.status_code,
-                        "message": err.response.reason,
-                    }
-                    if isinstance(err, HTTPError)
-                    else {
-                        "worker_error": str(err),
-                    }
-                )
-
-                self.save((persistence, container["current"]), req, "save_to")
-
-                if "ignore_error" not in req or not req["ignore_error"]:
-                    if "parent_current" in container:
-                        raise err
-                    break
-
-            if "break" in req and self.and_condition(
-                (persistence, container["current"]), req["break"]
-            ):
-                break
-
-        return persistence
+import re
+from copy import deepcopy
+from typing import Tuple
+
+from celery import Task
+from requests import get, post
+from requests.exceptions import HTTPError
+from jaseci.jsorc.jsorc import JsOrc
+
+DEFAULT_MSG = "Skipping scheduled walker!"
+
+
+class Queue(Task):
+    def run(self, wlk, nd, args):
+        hook = JsOrc.hook()
+
+        wlk = hook.get_obj_from_store(wlk)
+        wlk._to_await = True
+
+        nd = hook.get_obj_from_store(nd)
+        resp = wlk.run(nd, *args)
+
+        # commit to cache first then db instead of `commit()` only
+        # this is to support both jsctl and jsserv
+        wlk._h.commit_all_cache_sync()
+        wlk._h.commit(True)
+
+        wlk.destroy()
+
+        return {"anchor": wlk.anchor_value(), "response": resp}
+
+
+class ScheduledWalker(Task):
+    def get_obj(self, jid):
+        return self.hook.get_obj_from_store(jid)
+
+    def run(self, mst, wlk, ctx, nd=None, snt=None):
+        self.hook = JsOrc.hook()
+
+        if mst:
+            mst = self.get_obj(mst)
+        else:
+            return f"{DEFAULT_MSG} mst (Master) is required!"
+
+        if mst is None:
+            return f"{DEFAULT_MSG} Invalid Master!"
+
+        try:
+            if not snt:
+                if mst.active_snt_id == "global":
+                    global_snt_id = self.hook.get_glob("GLOB_SENTINEL")
+                    snt = self.get_obj(global_snt_id)
+                elif mst.active_snt_id:
+                    snt = self.get_obj(mst.active_snt_id)
+            elif snt in mst.alias_map:
+                snt = self.get_obj(mst.alias_map[snt])
+            else:
+                snt = self.get_obj(snt)
+
+            if not snt:
+                return f"{DEFAULT_MSG} Invalid Sentinel!"
+
+            if not nd:
+                if mst.active_gph_id:
+                    nd = self.get_obj(mst.active_gph_id)
+            elif nd in mst.alias_map:
+                nd = self.get_obj(mst.alias_map[nd])
+            else:
+                nd = self.get_obj(nd)
+
+            if not nd:
+                return f"{DEFAULT_MSG} Invalid Node!"
+
+            return mst.walker_run(wlk, nd, ctx, ctx, snt, False, False)
+        except Exception as e:
+            return f"{DEFAULT_MSG} Error occured: {e}"
+
+
+class ScheduledSequence(Task):
+    json_escape = re.compile(r"[^a-zA-Z0-9_]")
+    internal = re.compile(r"\(([a-zA-Z0-9_\.\[\]\$\#\@\!]*?)\)")
+    full = re.compile(r"^\{\{([a-zA-Z0-9_\.\[\]\$\#\(\)\@\!]*?)\}\}$")
+    partial = re.compile(r"\{\{([a-zA-Z0-9_\.\[\]\$\#\(\)\@\!]*?)\}\}")
+
+    def get_deep_value(self, data, keys, default):
+        if len(keys) == 0:
+            return data
+
+        key = keys.pop(0)
+        t = type(data)
+
+        if t is dict and key in data:
+            return self.get_deep_value(data[key], keys, default)
+        elif t is list and key.isnumeric():
+            return self.get_deep_value(data[int(key)], keys, default)
+        else:
+            return default
+
+    def get_value(self, holder: Tuple, keys: str, default=None):
+        while self.internal.search(keys):
+            for intern in self.internal.findall(keys):
+                keys = keys.replace(
+                    "(" + intern + ")", self.get_value(holder, intern, "")
+                )
+
+        if keys:
+            keys = keys.split(".")
+            key = keys.pop(0)
+            if key == "#":
+                return self.get_deep_value(holder[0], keys, default)
+            elif key == "$":
+                t = type(holder[1])
+                if t is dict or t is list:
+                    return self.get_deep_value(holder[1], keys, default)
+                else:
+                    return holder[1]
+            elif key == "@":
+                t = type(holder[2])
+                if t is dict or t is list:
+                    return self.get_deep_value(holder[2], keys, default)
+                else:
+                    return holder[2]
+            elif key == "!":
+                return holder[3]
+        return default
+
+    def compare(self, condition, expected, actual):
+        if condition == "eq":
+            return actual == expected
+        elif condition == "ne":
+            return actual != expected
+        elif condition == "gt":
+            return actual > expected
+        elif condition == "gte":
+            return actual >= expected
+        elif condition == "lt":
+            return actual < expected
+        elif condition == "lte":
+            return actual <= expected
+        elif condition == "regex":
+            return re.compile(expected).match(actual)
+
+    def condition(self, holder: Tuple, filter):
+        for cons in filter["condition"].keys():
+            if not (filter["condition"][cons] is None) and not self.compare(
+                cons, filter["condition"][cons], self.get_value(holder, filter["by"])
+            ):
+                return False
+        return True
+
+    def or_condition(self, holder: Tuple, filter):
+        for filt in filter:
+            if "condition" in filt and self.condition(holder, filt):
+                return True
+            elif "or" in filt and self.or_condition(holder, filt["or"]):
+                return True
+            elif "and" in filt and self.and_condition(holder, filt["and"]):
+                return True
+        return False
+
+    def and_condition(self, holder: Tuple, filter):
+        for filt in filter:
+            if "condition" in filt and not self.condition(holder, filt):
+                return False
+            elif "or" in filt and not self.or_condition(holder, filt["or"]):
+                return False
+            elif "and" in filt and not self.and_condition(holder, filt["and"]):
+                return False
+        return True
+
+    def deep_replace_str(self, holder: Tuple, data, key):
+        matcher = self.full.match(data[key])
+        if matcher:
+            data[key] = self.get_value(holder, matcher.group(1))
+        else:
+            for rep in self.partial.findall(data[key]):
+                data[key] = data[key].replace(
+                    "{{" + rep + "}}", self.get_value(holder, rep, "")
+                )
+
+    def deep_replace_dict(self, holder: Tuple, data):
+        for key in data.keys():
+            if key != "__def_loop__":
+                t = type(data[key])
+                if t is str:
+                    self.deep_replace_str(holder, data, key)
+                elif t is dict:
+                    self.deep_replace_dict(holder, data[key])
+
+    def save(self, holder: Tuple, req, params):
+        if params in req:
+            holder[0][self.json_escape.sub("_", req[params])] = holder[1]
+
+    def trigger_interface(self, req: dict):
+        master = req.get("master")
+        if master is None:
+            caller = JsOrc.master()
+            trigger_type = "public"
+        else:
+            caller = JsOrc.hook().get_obj_from_store(master)
+            trigger_type = "general"
+
+        api = req.get("api")
+        body = req.get("body", {})
+
+        return getattr(caller, f"{trigger_type}_interface_to_api")(body, api)
+
+    def run(self, **kwargs):
+        requests = kwargs.get("requests")
+        persistence = kwargs.get("persistence", {})
+        container = kwargs.get("container", {"current": persistence})
+        index = container.get("index", "0")
+
+        if "parent_current" in container:
+            container["current"] = container["parent_current"]
+
+        for req in requests:
+            try:
+                self.deep_replace_dict(
+                    (
+                        persistence,
+                        container["current"],
+                        container.get("parent_current", {}),
+                        index,
+                    ),
+                    req,
+                )
+                self.save((persistence, req), req, "save_req_to")
+
+                method = req["method"].upper()
+
+                if method == "JAC":
+                    container["current"] = self.trigger_interface(req)
+                else:
+                    if method == "POST":
+                        response = post(
+                            req["api"],
+                            json=req.get("body", {}),
+                            headers=req.get("header", {}),
+                        )
+                    elif method == "GET":
+                        response = get(req["api"], headers=req.get("header", {}))
+                    response.raise_for_status()
+                    if "application/json" in response.headers.get("Content-Type"):
+                        container["current"] = response.json()
+                    else:
+                        container["current"] = response.text
+
+                if "__def_loop__" in req:
+                    def_loop = req["__def_loop__"]
+                    for idx, loop in enumerate(
+                        self.get_value(
+                            (persistence, container["current"]), def_loop["by"], []
+                        )
+                    ):
+                        if "filter" in def_loop and not self.and_condition(
+                            (persistence, loop), def_loop["filter"]
+                        ):
+                            continue
+                        loop_container = {"parent_current": loop, "index": str(idx)}
+                        self.run(
+                            requests=deepcopy(def_loop["requests"]),
+                            persistence=persistence,
+                            container=loop_container,
+                        )
+
+                self.save((persistence, container["current"]), req, "save_to")
+
+            except Exception as err:
+                container["current"] = (
+                    {
+                        "status": err.response.status_code,
+                        "message": err.response.reason,
+                    }
+                    if isinstance(err, HTTPError)
+                    else {
+                        "worker_error": str(err),
+                    }
+                )
+
+                self.save((persistence, container["current"]), req, "save_to")
+
+                if "ignore_error" not in req or not req["ignore_error"]:
+                    if "parent_current" in container:
+                        raise err
+                    break
+
+            if "break" in req and self.and_condition(
+                (persistence, container["current"]), req["break"]
+            ):
+                break
+
+        return persistence
```

### Comparing `jaseci-1.4.0.9/jaseci/svc/task/task.py` & `jaseci-1.4.1.0/jaseci/extens/svc/task_svc.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,58 +1,75 @@
 from celery import Celery
+from celery.app.trace import build_tracer
 from celery.app.control import Inspect
 from celery.backends.base import DisabledBackend
 
-from jaseci.svc import CommonService
-from .common import Queue, ScheduledWalker, ScheduledSequence
-from .config import TASK_CONFIG
+from jaseci.jsorc.jsorc import JsOrc
+from jaseci.jsorc.jsorc_utils import ManifestType
+from .tasks import Queue, ScheduledWalker, ScheduledSequence
 
 #################################################
 #                   TASK APP                   #
 #################################################
 
 
-class TaskService(CommonService):
+@JsOrc.service(name="task", config="TASK_CONFIG")
+class TaskService(JsOrc.CommonService):
     ###################################################
     #                   INITIALIZER                   #
     ###################################################
 
-    def __init__(self, hook=None):
+    def __init__(
+        self,
+        config: dict,
+        manifest: dict,
+        manifest_type: ManifestType = ManifestType.DEDICATED,
+        source: dict = {},
+    ):
         self.inspect: Inspect = None
         self.queue: Queue = None
         self.scheduled_walker: ScheduledWalker = None
         self.scheduled_sequence: ScheduledSequence = None
 
-        super().__init__(hook)
+        super().__init__(config, manifest, manifest_type, source)
 
     ###################################################
     #                     BUILDER                     #
     ###################################################
 
-    def run(self, hook=None):
+    def run(self):
         self.app = Celery("celery")
         self.app.conf.update(**self.config)
 
         # -------------------- TASKS -------------------- #
-
-        self.queue = self.app.register_task(Queue())
-        self.scheduled_walker = self.app.register_task(ScheduledWalker())
-        self.scheduled_sequence = self.app.register_task(ScheduledSequence())
+        (
+            self.queue,
+            self.scheduled_walker,
+            self.scheduled_sequence,
+        ) = self.register_tasks(Queue, ScheduledWalker, ScheduledSequence)
 
         # ------------------ INSPECTOR ------------------ #
 
         self.inspect = self.app.control.inspect()
         self.ping()
 
-    def post_run(self, hook=None):
+    def post_run(self):
         self.spawn_daemon(
             worker=self.app.Worker(quiet=self.quiet).start,
             scheduler=self.app.Beat(socket_timeout=None, quiet=self.quiet).run,
         )
 
+    def register_tasks(self, *tasks) -> tuple:
+        registered = []
+        for task in tasks:
+            task = self.app.register_task(task())
+            task.__trace__ = build_tracer(task.name, task, app=self.app)
+            registered.append(task)
+        return tuple(registered)
+
     ###################################################
     #              COMMON GETTER/SETTER               #
     ###################################################
 
     def get_by_task_id(self, task_id, wait=False, timeout=30):
         task = self.app.AsyncResult(task_id)
 
@@ -89,22 +106,15 @@
     def add_queue(self, wlk, nd, *args):
         return self.queue.delay(wlk.jid, nd.jid, args).task_id
 
     ###################################################
     #                     CLEANER                     #
     ###################################################
 
-    def reset(self, hook, start=True):
+    def failed(self, error):
+        super().failed(error)
         self.terminate_daemon("worker", "scheduler")
-        self.inspect = None
-        super().reset(hook, start)
 
-    def failed(self):
-        super().failed()
-        self.terminate_daemon("worker", "scheduler")
+    # ---------------- PROXY EVENTS ----------------- #
 
-    ####################################################
-    #                    OVERRIDDEN                    #
-    ####################################################
-
-    def build_config(self, hook) -> dict:
-        return hook.service_glob("TASK_CONFIG", TASK_CONFIG)
+    def on_delete(self):
+        self.terminate_daemon("worker", "scheduler")
```

### Comparing `jaseci-1.4.0.9/jaseci/tests/infer.py` & `jaseci-1.4.1.0/jaseci/tests/infer.py`

 * *Files 3% similar despite different names*

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
 
@@ -27,7 +27,13 @@
     return jsdate.quantize_to_day(date)
 
 
 @jaseci_action()
 def date_day_diff(start_date: str, end_date: str):
     logger.warning("Deprecated! Use date...")
     return jsdate.date_day_diff(start_date, end_date)
+
+
+@jaseci_action()
+def date_now():
+    logger.warning("Deprecated! Use date...")
+    return jsdate.date_now()
```

### Comparing `jaseci-1.4.0.9/jaseci/tests/jac_test_code.py` & `jaseci-1.4.1.0/jaseci/tests/jac_test_code.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.0.9/jaseci/tests/jac_test_progs.py` & `jaseci-1.4.1.0/jaseci/tests/jac_test_progs.py`

 * *Files 6% similar despite different names*

```diff
@@ -553,14 +553,34 @@
             };
 
             report testing;
         }
     }
 """
 
+list_pairwise = """
+walker init{
+    with entry{
+        _list = [1,2,3,4];
+        p = _list.list::pairwise;
+        report p;
+    }
+    }
+"""
+
+list_unique = """
+walker init{
+    with entry{
+        _list = [1,2,3,4,2,3,4,5];
+        p = _list.list::unique;
+        report p;
+    }
+    }
+"""
+
 check_new_builtin = """
     walker init {
         with entry {
             a = {"test":"test"};
 
             // dict get with default if not existing
             b = a.dict::get("t", 1);
@@ -574,14 +594,15 @@
             report b;
             report c;
             report d;
         }
     }
 """
 
+
 continue_issue = """
     walker init {
         root {
             for i=0 to i<10 by i+=1 {
                 if(i==9):
                     continue;
                 if(i):
@@ -625,14 +646,44 @@
         report task2;
 
         report sync task2;
     }
 }
 """
 
+async_syntax_with_update = """
+node a {
+    has value = false;
+}
+walker init {
+    root {
+        spawn here ++> node::a;
+    }
+}
+
+async walker update_value {
+    root {
+        take --> node::a;
+    }
+    a {
+        here.value = true;
+        report here.context;
+    }
+}
+
+walker get_value {
+    root {
+        take --> node::a;
+    }
+    a {
+        report here.context;
+    }
+}
+"""
+
 block_scope_check = """
     walker init {
         i=5;
         for i=0 to i<10 by i+=1 {
             report i;
         }
         report i;
@@ -667,7 +718,40 @@
     can sim1.tester, sim2.tester;
     with entry {
         report sim1.tester();
         report sim2.tester();
     }
 }
 """
+
+walker_null_args = """
+node c {
+    has c1, c2;
+}
+
+walker b {
+    has anchor b1, b2;
+    with entry {
+        report b1;
+        report b2;
+    }
+}
+
+walker a {
+    has a1;
+
+    with entry {
+        a2 = null;
+        te = spawn here walker::b(b1 = a1, b2 = a2);
+        te = spawn here ++> node::c(c1=a1, c2=a2);
+    }
+}
+"""
+
+json_casting = """
+walker json_casting {
+    with entry {
+        report {"test": 1}.str;
+        report '{"test2": 2}'.dict;
+    }
+}
+"""
```

### Comparing `jaseci-1.4.0.9/jaseci/tests/test_core.py` & `jaseci-1.4.1.0/jaseci/tests/test_core.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 import uuid
 from unittest import TestCase
 
 import jaseci.tests.jac_test_code as jtc
-from jaseci.actor.sentinel import Sentinel
-from jaseci.element.element import Element
-from jaseci.graph.graph import Graph
-from jaseci.graph.node import Node
-from jaseci.svc import MetaService
+from jaseci.prim.sentinel import Sentinel
+from jaseci.prim.element import Element
+from jaseci.prim.graph import Graph
+from jaseci.prim.node import Node
+from jaseci.jsorc.jsorc import JsOrc
 from jaseci.utils.utils import TestCaseHelper, get_all_subclasses
-from jaseci.actor.architype import Architype
+from jaseci.prim.architype import Architype
 
 
 class ArchitypeTests(TestCaseHelper, TestCase):
     def setUp(self):
         super().setUp()
-        self.meta = MetaService(run_svcs=False)
 
     def tearDown(self):
         super().tearDown()
 
     def test_object_creation_basic_no_side_creation(self):
         """ """
-        mast = self.meta.build_master()
+        mast = JsOrc.master()
         num_objs = len(mast._h.mem.keys())
         node1 = Node(m_id=mast._m_id, h=mast._h)
         node2 = Node(m_id=mast._m_id, h=mast._h, parent=node1)
         num_new = len(mast._h.mem.keys())
         self.assertEqual(num_new, num_objs + 2)
 
         new_graph = Graph(m_id=mast._m_id, h=mast._h)
@@ -36,30 +35,30 @@
         new_graph.attach_outbound(node1)
         new_graph.attach_outbound(node2)
         num_new = len(mast._h.mem.keys())
         self.assertEqual(num_new, num_objs + 5)
 
     def test_edge_removal_updates_nodes_edgelist(self):
         """ """
-        mast = self.meta.build_master()
+        mast = JsOrc.master()
         node1 = Node(m_id=mast._m_id, h=mast._h)
         node2 = Node(m_id=mast._m_id, h=mast._h)
         edge = node1.attach_outbound(node2)
         self.assertEqual(len(node1.smart_edge_list), 1)
         self.assertEqual(len(node2.smart_edge_list), 1)
         self.assertEqual(len(edge), 1)
         edge[0].destroy()
         self.assertEqual(len(node1.smart_edge_list), 0)
         self.assertEqual(len(node2.smart_edge_list), 0)
 
     def test_object_creation_by_sentinel_no_leaks(self):
         """
         Test that the destroy of sentinels clears owned objects
         """
-        mast = self.meta.build_master()
+        mast = JsOrc.master()
         num_objs = len(mast._h.mem.keys())
         self.assertEqual(num_objs, 2)
         new_graph = Graph(m_id=mast._m_id, h=mast._h)
         sent = Sentinel(m_id=mast._m_id, h=mast._h)
         code = jtc.prog1
         mast.sentinel_ids.add_obj(sent)
         mast.graph_ids.add_obj(new_graph)
@@ -73,66 +72,64 @@
         self.assertEqual(num_objs, new_num)
 
     def test_json_blob_of_objects(self):
         """
         Test saving object to json and back to python dict
         """
         for i in get_all_subclasses(Element):
-            kwargs = {"m_id": 0, "h": self.meta.build_hook()}
+            kwargs = {"m_id": 0, "h": JsOrc.hook()}
             orig = i(**kwargs)
             blob1 = orig.json(detailed=True)
             new = i(**kwargs)
             self.assertNotEqual(orig.id, new.id)
             new.json_load(blob1)
             self.assertEqual(orig.id, new.id)
             self.assertTrue(orig.is_equivalent(new))
 
     def test_supermaster_can_touch_all_data(self):
-        mh = self.meta.build_hook()
-        mast = self.meta.build_master(h=mh)
-        mast2 = self.meta.build_master(h=mh)
+        mh = JsOrc.hook()
+        mast = JsOrc.master(h=mh)
+        mast2 = JsOrc.master(h=mh)
         node12 = Node(m_id=mast2._m_id, h=mast2._h)
-        supmast = self.meta.build_super_master(h=mh)
+        supmast = JsOrc.super_master(h=mh)
         bad = mh.get_obj(mast._m_id, node12.jid)
         good = mh.get_obj(supmast._m_id, node12.jid)
         self.assertEqual(good, node12)
         self.assertNotEqual(bad, node12)
         self.assertIsNone(bad)
 
     def test_id_list_smart_name_error(self):
-        self.logger_on()
-        mast = self.meta.build_master()
+        mast = JsOrc.master()
         sent = Sentinel(m_id=mast._m_id, h=mast._h)
         self.assertIn("arch_ids", sent.arch_ids.obj_for_id_not_exist_error(0))
 
     def test_dont_store_invalid_feilds_in_blob(self):
-        self.logger_on()
-        mast = self.meta.build_master()
+        mast = JsOrc.master()
         sent = Sentinel(m_id=mast._m_id, h=mast._h)
         sent.fake_data = 5
         stored = sent.jsci_payload()
         sent2 = Sentinel(m_id=mast._m_id, h=mast._h)
         sent2.json_load(stored)
         self.assertNotIn("fake_data", vars(sent2).keys())
 
     def test_sentinel_default_archs_dont_grow(self):
-        mast = self.meta.build_master()
+        mast = JsOrc.master()
         sent = Sentinel(m_id=mast._m_id, h=mast._h)
         sent.register_code(text="node simple; walker init {}")
         before = sent._h.get_object_distribution()[Architype]
         stored = sent.jsci_payload()
         sent2 = Sentinel(m_id=mast._m_id, h=mast._h)
         sent2.json_load(stored)
         sent2 = Sentinel(m_id=mast._m_id, h=mast._h)
         sent2.json_load(stored)
         after = sent2._h.get_object_distribution()[Architype]
         self.assertEqual(before, after)
 
     def test_sentinel_default_archs_dont_grow_multi_compile(self):
-        mast = self.meta.build_master()
+        mast = JsOrc.master()
         sent = Sentinel(m_id=mast._m_id, h=mast._h)
         sent.register_code(text="node simple; walker init {}")
         before = sent._h.get_object_distribution()[Architype]
         stored = sent.jsci_payload()
         sent2 = Sentinel(m_id=mast._m_id, h=mast._h)
         sent2.json_load(stored)
         sent2.register_code(text="node simple; walker init {}")
@@ -141,15 +138,15 @@
         sent2.register_code(text="node simple; walker init {}")
         after_id = sent2.arch_ids[0]
         after = sent2._h.get_object_distribution()[Architype]
         self.assertEqual(before, after)
         self.assertNotEqual(before_id, after_id)
 
     def test_id_list_heals(self):
-        mast = self.meta.build_master()
+        mast = JsOrc.master()
         sent = Sentinel(m_id=mast._m_id, h=mast._h)
         sent.register_code(text="node simple; walker init {}")
         before = len(sent.arch_ids)
         sent._h.get_obj(mast._m_id, sent.arch_ids[1]).destroy()
         sent._h.get_obj(mast._m_id, sent.arch_ids[3]).destroy()
         sent.arch_ids.obj_list()
         after = len(sent.arch_ids)
```

### Comparing `jaseci-1.4.0.9/jaseci/tests/test_jac.py` & `jaseci-1.4.1.0/jaseci/tests/test_jac.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import os
 from unittest import TestCase
 
 from antlr4 import CommonTokenStream, InputStream
 
-import jaseci.actions.live_actions as lact
+import jaseci.jsorc.live_actions as lact
 import jaseci.tests.jac_test_code as jtc
-from jaseci.actor.sentinel import Sentinel
-from jaseci.graph.graph import Graph
+from jaseci.prim.sentinel import Sentinel
+from jaseci.prim.graph import Graph
 from jaseci.jac.jac_parse.jacLexer import jacLexer
 from jaseci.jac.jac_parse.jacParser import jacParser
-from jaseci.svc import MetaService
+from jaseci.jsorc.jsorc import JsOrc
 from jaseci.utils.utils import TestCaseHelper
 
 
 class JacTests(TestCaseHelper, TestCase):
     """Unit tests for Jac language"""
 
     def setUp(self):
         super().setUp()
-        self.meta = MetaService()
 
     def tearDown(self):
         super().tearDown()
 
     def test_antlr4_parsing_lifelogify(self):
         """Basic test of jac grammar with lifelogify program"""
         input_stream = InputStream(jtc.prog1)
@@ -30,32 +29,32 @@
         stream = CommonTokenStream(lexer)
         parser = jacParser(stream)
         parser.start()
         self.assertEqual(parser.getNumberOfSyntaxErrors(), 0)
 
     def test_sentinel_loading_jac_code(self):
         """Test the generation of jaseci trees for programs in grammar"""
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         sent.register_code(jtc.prog1)
         self.assertIsNotNone(sent.run_architype("get_gen_day"))
         self.assertIsNotNone(sent.arch_ids.get_obj_by_name("week", kind="node"))
 
     def test_sentinel_loading_jac_code_multiple_times(self):
         """Test registering resets correctly for multiple attempts"""
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         sent.register_code(jtc.prog0)
         num_arch = len(sent.arch_ids)
         sent.register_code(jtc.prog0)
         self.assertEqual(len(sent.arch_ids), num_arch)
         sent.register_code(jtc.prog0)
         self.assertEqual(len(sent.arch_ids), num_arch)
 
     def test_sentinel_register_dep_on_static_errors(self):
         """Test Jac registering is dependant on correct static/dynamic code"""
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         correct = "node b { has anchor a; }"
         wrong1 = "adfdsf"
         sent.register_code(correct)
         self.assertTrue(sent.is_active)
         sent.register_code(wrong1)
         self.assertFalse(sent.is_active)
         sent.register_code(correct)
@@ -63,23 +62,23 @@
         sent.register_code(wrong1)
         self.assertFalse(sent.is_active)
         sent.register_code(correct)
         self.assertTrue(sent.is_active)
 
     def test_sentinel_loading_arhitype(self):
         """Test the generation of jaseci trees for programs in grammar"""
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         sent.register_code(jtc.prog1)
         self.assertGreater(
             len(sent.arch_ids.get_obj_by_name("month", kind="node").code_ir), 5
         )
 
     def test_sentinel_running_basic_walker(self):
         """Test the execution of a basic walker building graph"""
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         sent.register_code(jtc.prog1)
         test_node = sent.arch_ids.get_obj_by_name("life", kind="node").run()
         test_walker = sent.run_architype("get_gen_day")
         test_walker.prime(test_node)
         test_walker.context["date"] = "2010-08-03T03:00:00.000000"
         test_walker.run()
         self.assertEqual(len(test_node.outbound_nodes()), 1)
@@ -87,15 +86,15 @@
         self.assertEqual(
             test_node.outbound_nodes()[0].outbound_nodes()[0].outbound_nodes()[0].name,
             "week",
         )
 
     def test_sentinel_setp_running_walker(self):
         """Test the execution of a basic walker building graph"""
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         sent.register_code(jtc.prog1)
         test_node = sent.arch_ids.get_obj_by_name("life", kind="node").run()
         test_walker = sent.run_architype("get_gen_day")
         test_walker.prime(test_node)
         test_walker.context["date"] = "2010-08-03T03:00:00.000000"
         self.assertEqual(len(test_node.outbound_nodes()), 0)
         next = test_walker.step()
@@ -110,15 +109,15 @@
         next = test_walker.step()
         self.assertFalse(next)
 
     def test_walker_writes_through_no_data_gain_loss_on_contexts(self):
         """
         Test that  no loss or gain of data on second trak on second trek
         """
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.prog1)
         test_node = sent.arch_ids.get_obj_by_name("life", kind="node").run()
         test_walker = sent.run_architype("get_gen_day")
         test_walker.prime(test_node)
         test_walker.context["date"] = "2010-08-03T03:00:00.000000"
         self.assertEqual(test_walker.context["date"], "2010-08-03T03:00:00.000000")
@@ -133,15 +132,15 @@
 
     def test_arch_ids_generate_node_bound_objects_scalably(self):
         """
         Test that arch_ids in sents bind contents to actual nodes
         scalably (node contexts dont get deleted when arch_ids deleted)
         """
         lact.load_local_actions(os.path.dirname(__file__) + "/infer.py")
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         sent.register_code(jtc.prog1)
         test_node = sent.arch_ids.get_obj_by_name("life", kind="node").run()
         test_walker = sent.run_architype("get_gen_day")
         test_walker.prime(test_node)
         test_walker.context["date"] = "2010-08-03T03:00:00.000000"
         self.assertEqual(test_walker.context["date"], "2010-08-03T03:00:00.000000")
         test_walker.run()
@@ -150,137 +149,137 @@
         before_del = year_node.context["year"]
         sent.register_code(jtc.prog1)
         after_del = year_node.context["year"]
         self.assertEqual(before_del, after_del)
 
     def test_sent_loads_complex_walker_and_arch(self):
         """Test loading attributes of arch and walkers"""
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         sent.register_code(jtc.prog1)
         test_node = sent.arch_ids.get_obj_by_name("testnode", kind="node").run()
         test_walker = sent.run_architype("testwalk")
         test_walker.prime(test_node)
         test_walker.run()
         self.assertEqual(test_node.context["c"], '43Yeah \n"fools"!')
 
     def test_availabilty_of_global_functions(self):
         """Test preset function loading"""
         from jaseci.jac.machine.jac_scope import JacScope
 
-        JacScope(None, None, [])
-        from jaseci.jac.machine.jac_scope import global_action_sets
+        JacScope(None, None)
+        from jaseci.jac.machine.jac_scope import get_global_actions
 
-        self.assertGreater(len(global_action_sets), 5)
+        self.assertGreater(len(get_global_actions()), 5)
 
     def test_multiple_edged_between_nodes_work(self):
         """Test that multiple edges between the same two nodes are allowed"""
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.edgey)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         edges = list(gph.get_all_architypes()[1].values())
         self.assertEqual(len(edges), 3)
         edge_names = [edges[0].name, edges[1].name, edges[2].name]
         self.assertIn("generic", edge_names)
         self.assertIn("apple", edge_names)
         self.assertIn("banana", edge_names)
 
     def test_multiple_edged_between_nodes_delete_all(self):
         """Test that multiple edges deleted correctly if delete all"""
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.edgey2)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         edges = gph.get_all_architypes()[1].values()
         self.assertEqual(len(edges), 0)
 
     def test_multiple_edged_between_nodes_delete_all_specific(self):
         """Test that multiple edges deleted correctly if delete all"""
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.edgey2b)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         edges = gph.get_all_architypes()[1].values()
         self.assertEqual(len(edges), 1)
 
     def test_multiple_edged_between_nodes_delete_all_labeled(self):
         """Test that multiple edges deleted correctly if delete all"""
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.edgey2c)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         edges = gph.get_all_architypes()[1].values()
         self.assertEqual(len(edges), 3)
 
     def test_multiple_edged_between_nodes_delete_filtered(self):
         """Test that multiple edges deleted correctly if delete filtered"""
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.edgey3)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         edges = gph.get_all_architypes()[1].values()
         self.assertEqual(len(edges), 5)
 
     def test_generic_can_be_used_to_specify_generic_edges(self):
         """Test that generic edge tag works"""
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.edgey4)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         edges = gph.get_all_architypes()[1].values()
         self.assertEqual(len(edges), 2)
 
     def test_can_disconnect_multi_nodes_simultaneously(self):
         """Test disconnecting mutilpe nodes"""
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.edgey5)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         edges = gph.get_all_architypes()[1].values()
         self.assertEqual(len(edges), 2)
 
     def test_can_connect_multi_nodes_simultaneously(self):
         """Test connecting mutilpe nodes"""
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.edgey6)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         edges = gph.get_all_architypes()[1].values()
         self.assertEqual(len(edges), 4)
 
     def test_can_disconnect_multi_nodes_advanced(self):
         """Test disconnecting mutilpe nodes advanced"""
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.edgey7)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         edges = gph.get_all_architypes()[1].values()
         self.assertEqual(len(edges), 3)
 
     def test_accessing_edges_basic(self):
         """Test accessing Edges"""
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.edge_access)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         edges = list(gph.get_all_architypes()[1].values())
         if edges[0].name == "apple":
@@ -288,15 +287,15 @@
             self.assertEqual(edges[1].context["x1"], 8)
         else:
             self.assertEqual(edges[1].context["v1"], 7)
             self.assertEqual(edges[0].context["x1"], 8)
 
     def test_has_assign(self):
         """Test assignment on definition"""
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.has_assign)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         nodes = gph.get_all_architypes()[0].values()
         self.assertEqual(len(nodes), 3)
@@ -305,146 +304,146 @@
             if i.name == "testnode":
                 self.assertEqual(i.context["a"], 8)
                 num += 1
         self.assertEqual(num, 2)
 
     def test_global_get_set(self):
         """Test assignment on definition"""
-        mast = self.meta.build_super_master()
+        mast = JsOrc.super_master()
         sent = Sentinel(m_id=mast.jid, h=mast._h)
         gph = Graph(m_id=mast.jid, h=mast._h)
         sent.register_code(jtc.set_get_global)
         test_walker = sent.run_architype("setter")
         test_walker.prime(gph)
         test_walker.run()
         test_walker2 = sent.run_architype("getter")
         test_walker2.prime(gph)
         test_walker2.run()
         self.assertEqual(test_walker2.context["a"], 59)
 
     def test_global_set_requires_admin(self):
         """Test assignment on definition"""
-        mast = self.meta.build_master()
+        mast = JsOrc.master()
         sent = Sentinel(m_id=mast.jid, h=mast._h)
         gph = Graph(m_id=mast.jid, h=mast._h)
         sent.register_code(jtc.set_get_global2)
         test_walker = sent.run_architype("setter")
         test_walker.prime(gph)
         test_walker.run()
         test_walker2 = sent.run_architype("getter")
         test_walker2.prime(gph)
         test_walker2.run()
         self.assertEqual(test_walker2.context["a"], None)
 
     def test_sentinel_version_label(self):
         """Test sentinel version labeling"""
-        mast = self.meta.build_master()
+        mast = JsOrc.master()
         sent = Sentinel(m_id=mast.jid, h=mast._h)
         sent.register_code(jtc.version_label)
         self.assertEqual(sent.version, "alpha-1.0")
 
     def test_visibility_builtins(self):
         """Test builtins to see into nodes and edges"""
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.visibility_builtins)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         self.assertEqual(2, len(test_walker.report[0][0].keys()))
         self.assertGreaterEqual(len(test_walker.report[0][1].keys()), 6)
         self.assertLess(len(test_walker.report[0][1].keys()), 14)
         self.assertGreaterEqual(len(test_walker.report[0][2].keys()), 13)
 
     def test_spawn_ctx_for_edges_nodes(self):
         """Test builtins to see into nodes and edges"""
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.spawn_ctx_edge_node)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         self.assertEqual(test_walker.report[0]["age"], 32)
         self.assertEqual(test_walker.report[1]["meeting_place"], "college")
         self.assertEqual(test_walker.report[2]["name"], "Jane")
         self.assertEqual(test_walker.report[3]["kind"], "sister")
 
     def test_filter_ctx_for_edges_nodes(self):
         """Test builtins to see into nodes and edges"""
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.filter_ctx_edge_node)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         self.assertEqual(test_walker.report[0]["age"], 30)
         self.assertEqual(len(test_walker.report[1]), 0)
 
     def test_null_handling(self):
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.null_handleing)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         self.assertEqual(test_walker.report[0], True)
         self.assertEqual(test_walker.report[1], False)
         self.assertEqual(test_walker.report[2], True)
         self.assertEqual(test_walker.report[3], False)
 
     def test_bool_type_convert(self):
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.bool_type_convert)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         self.assertEqual(test_walker.report[0], True)
         self.assertEqual(True, test_walker.report[1]["name"])
 
     def test_typecasts(self):
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.typecasts)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         self.assertEqual(test_walker.report[0], 7.6)
         self.assertEqual(test_walker.report[1], 7)
         self.assertEqual(test_walker.report[2], "7.6")
         self.assertEqual(test_walker.report[3], True)
         self.assertEqual(test_walker.report[4], 7.0)
         self.assertEqual(test_walker.report[5], "Types comes back correct")
 
     def test_typecast_error(self):
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.typecasts_error)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         self.assertIn("Cannot get edges from 7.6", test_walker.runtime_errors[0])
         self.assertIn(
             "Invalid cast of JAC_TYPE.STR to JAC_TYPE.INT",
             test_walker.runtime_errors[1],
         )
 
     def test_filter_on_context(self):
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.filter_on_context)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         self.assertEqual({"yo": "Yeah i said"}, test_walker.report[0][0])
         self.assertNotIn("name", test_walker.report[0][1].keys())
         self.assertIn("name", test_walker.report[0][2].keys())
 
     def test_string_manipulation(self):
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.string_manipulation)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         rep = test_walker.report
         self.assertEqual(rep[0], "t")
@@ -475,15 +474,15 @@
         self.assertEqual(rep[25], "tEsting me  ")
         self.assertEqual(rep[26], "sting me  ")
         self.assertEqual(rep[27], " tEsting me")
         self.assertEqual(rep[28], " tEsting m")
         self.assertEqual(rep[29], True)
 
     def test_list_manipulation(self):
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.list_manipulation)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         rep = test_walker.report
         self.assertEqual(rep[0], [4])
@@ -495,26 +494,26 @@
         self.assertEqual(rep[6], [5, 5, 4, 2])
         self.assertEqual(rep[7], [5, "apple", 4, 2])
         self.assertEqual(rep[8], 1)
         self.assertEqual(rep[9], [5, "apple", 4])
         self.assertEqual(rep[10], [])
 
     def test_list_reversed(self):
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.list_reversed)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         rep = test_walker.report
         self.assertEqual(rep[0], [7, 2, 4])
         self.assertEqual(rep[1], [4, 2, 7])
 
     def test_dict_manipulation(self):
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.dict_manipulation)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         rep = test_walker.report
         self.assertEqual(rep[0], {"four": 4, "five": 5})
@@ -523,37 +522,37 @@
         self.assertEqual(rep[3], ["four", "five"])
         self.assertEqual(rep[4], {"four": 4})
         self.assertEqual(rep[5], [4])
         self.assertEqual(rep[6], {"four": 7})
         self.assertEqual(rep[7], {})
 
     def test_string_join(self):
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.string_join)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         rep = test_walker.report
         self.assertEqual(rep[0], "test_me_now")
 
     def test_sub_list(self):
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.sub_list)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         rep = test_walker.report
         self.assertEqual(rep[0][0], 5)
         self.assertEqual(rep[0][1], 6)
         self.assertEqual(rep[0][2], 7)
 
     def test_destroy_and_misc(self):
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.destroy_and_misc)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         rep = test_walker.report
         self.assertEqual(rep[0], "Josh")
@@ -570,27 +569,27 @@
         self.assertEqual(rep[7], None)
         self.assertEqual(
             rep[8], {"age": 32, "birthday": None, "name": "pete", "profession": None}
         )
         self.assertEqual(rep[9], True)
 
     def test_arbitrary_assign_on_element(self):
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.arbitrary_assign_on_element)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         rep = test_walker.report
         self.assertEqual(
             rep[0], {"name": None, "age": None, "birthday": None, "profession": None}
         )
 
     def test_try_else_stmts(self):
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.try_else_stmts)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         rep = test_walker.report
         self.assertEqual(
@@ -607,189 +606,189 @@
             },
         )
         self.assertEqual(rep[1], "dont need err")
         self.assertEqual(rep[2], None)
         self.assertEqual(rep[3], 2)
 
     def test_node_edge_same_name(self):
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.node_edge_same_name)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         rep = test_walker.report
         self.assertEqual(rep[0], {"meeting_place": "college"})
         self.assertEqual(
             rep[1], {"age": 32, "birthday": None, "name": "Josh", "profession": None}
         )
 
     def test_testcases(self):
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         sent.register_code(jtc.testcases)
         sent.run_tests(silent=True)
         self.assertEqual(len(sent.testcases), 4)
         for i in sent.testcases:
             self.assertEqual(i["passed"], True)
 
     def test_testcase_asserts(self):
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         sent.register_code(jtc.testcase_asserts)
         sent.run_tests(silent=True)
         self.assertEqual(len(sent.testcases), 3)
         self.assertEqual(sent.testcases[0]["passed"], True)
         self.assertEqual(sent.testcases[1]["passed"], False)
         self.assertEqual(sent.testcases[2]["passed"], False)
 
     def test_report_not_to_jacset(self):
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.report_not_to_jacset)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         rep = test_walker.report
         self.assertIn("context", rep[0][0].keys())
         self.assertIn("j_type", rep[0][0].keys())
 
     def test_walker_spawn_unwrap_check(self):
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.walker_spawn_unwrap_check)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         rep = test_walker.report
         self.assertTrue(rep[0].startswith("urn:uuid"))
 
     def test_std_get_report(self):
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.std_get_report)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         rep = test_walker.report
         self.assertEqual(rep, [3, 5, 6, 7, [3, 5, 6, 7], 8])
 
     def test_func_with_array_index(self):
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.func_with_array_index)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         rep = test_walker.report
         self.assertEqual(rep, [3, 5, 3])
 
     def test_rt_error_test1(self):
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.rt_error_test1)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         self.assertIn("List index out of range", test_walker.runtime_errors[0])
         self.assertIn(" line ", test_walker.runtime_errors[0])
         self.assertIn(" col ", test_walker.runtime_errors[0])
 
     def test_root_type_nodes(self):
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.root_type_nodes)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         report = test_walker.report
         self.assertEqual(report, ["root", "root"])
 
     def test_invalid_key_error(self):
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.invalid_key_error)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         errors = test_walker.runtime_errors
         self.assertGreater(len(errors), 0)
 
     def test_auto_cast(self):
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.auto_cast)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         report = test_walker.report
         self.assertEqual(report, [True, True])
 
     def test_no_error_on_dict_key_assign(self):
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.no_error_on_dict_key_assign)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         report = test_walker.report
         self.assertEqual(report, [{"b": 4}])
         self.assertEqual(len(test_walker.runtime_errors), 0)
 
     def test_report_status(self):
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.report_status)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         report = test_walker.report
         self.assertEqual(report, ["hello"])
         self.assertEqual(test_walker.report_status, 302)
 
     def test_graph_in_graph(self):
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.graph_in_graph)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         report = test_walker.report
         self.assertEqual(len(report), 3)
 
     def test_min_max_on_list(self):
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.min_max_on_list)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         report = test_walker.report
         self.assertEqual(report, [531.1, 3, 5, 1])
 
     def test_edge_bug(self):
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.edge_bug)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         report = test_walker.report
         self.assertEqual(len(report[0]), 4)
 
     def test_rand_choice(self):
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.rand_choice)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         report = test_walker.report
         self.assertIn(report[1], report[0])
 
     def test_struct_types(self):
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtc.struct_types)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         report = test_walker.report
         self.assertEqual(report[0], [43, 33])
```

### Comparing `jaseci-1.4.0.9/jaseci/tests/test_node.py` & `jaseci-1.4.1.0/jaseci/tests/test_node.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,23 @@
 from unittest import TestCase
 
-from jaseci.actor.architype import Architype
-from jaseci.attr import action
-from jaseci.graph.edge import Edge
-from jaseci.graph.node import Node
-from jaseci.svc import MetaService
+from jaseci.prim.architype import Architype
+from jaseci.prim import ability
+from jaseci.prim.edge import Edge
+from jaseci.prim.node import Node
+from jaseci.jsorc.jsorc import JsOrc
 from jaseci.utils.utils import TestCaseHelper
 
 
 class NodeTests(TestCaseHelper, TestCase):
     """Tests for the funcationality of Jaseci node class"""
 
-    def setUp(self):
-        super().setUp()
-        self.meta = MetaService()
-
-    def tearDown(self):
-        super().tearDown()
-
     def test_node_connections(self):
         """Test connecting and disconnecting etc of nodes"""
-        node1 = Node(m_id=0, h=self.meta.build_hook())
+        node1 = Node(m_id=0, h=JsOrc.hook())
         node2 = Node(m_id=0, h=node1._h)
         node3 = Node(m_id=0, h=node1._h)
         node4 = Node(m_id=0, h=node1._h)
         node1.attach_outbound(node2)
         node3.attach_outbound(node2)
         node1.attach_inbound(node2)
         node3.attach_inbound(node2)
@@ -45,55 +38,52 @@
         self.assertEqual(len(node1.inbound_nodes()), 0)
         self.assertEqual(len(node2.inbound_nodes()), 0)
         self.assertEqual(len(node3.inbound_nodes()), 0)
         self.assertEqual(len(node4.inbound_nodes()), 0)
 
     def test_add_context_to_node_and_destroy(self):
         """Test adding and removing contexts nodes"""
-        node1 = Node(m_id=0, h=self.meta.build_hook())
+        node1 = Node(m_id=0, h=JsOrc.hook())
         node1.context["yeah dude"] = "SUP"
         self.assertEqual(node1.context["yeah dude"], "SUP")
         self.assertEqual(len(node1.context.keys()), 1)
         self.assertTrue("yeah dude" in node1.context.keys())
         self.assertFalse("yeah  dude" in node1.context.keys())
 
     def test_add_entry_action_to_node_and_destroy(self):
         """Test connecting and disconnecting etc of nodes"""
-        node1 = Architype(m_id=0, h=self.meta.build_hook())
-        act = action.Action(m_id=0, h=node1._h, name="yeah dude", value="SUP")
-        node1.entry_action_ids.add_obj(act)
-        self.assertEqual(
-            node1.entry_action_ids.get_obj_by_name("yeah dude").value, "SUP"
-        )
-        self.assertEqual(len(node1.entry_action_ids), 1)
-        self.assertTrue(node1.entry_action_ids.has_obj_by_name("yeah dude"))
-        self.assertFalse(node1.entry_action_ids.has_obj_by_name("yeah  dude"))
-
-        node1.entry_action_ids.destroy_obj_by_name(name="yeah dude")
-        self.assertEqual(len(node1.entry_action_ids), 0)
-        self.assertFalse(node1.entry_action_ids.has_obj_by_name("yeah dude"))
+        node1 = Architype(m_id=0, h=JsOrc.hook())
+        act = ability.Ability(m_id=0, h=node1._h, name="yeah dude")
+        node1.entry_ability_ids.add_obj(act)
+        self.assertEqual(len(node1.entry_ability_ids), 1)
+        self.assertTrue(node1.entry_ability_ids.has_obj_by_name("yeah dude"))
+        self.assertFalse(node1.entry_ability_ids.has_obj_by_name("yeah  dude"))
+
+        node1.entry_ability_ids.destroy_obj_by_name(name="yeah dude")
+        self.assertEqual(len(node1.entry_ability_ids), 0)
+        self.assertFalse(node1.entry_ability_ids.has_obj_by_name("yeah dude"))
 
     def test_adding_and_removing_from_hdnodes(self):
         """Test adding nodes and removing them from HDGDs"""
-        node1 = Node(m_id=0, h=self.meta.build_hook())
+        node1 = Node(m_id=0, h=JsOrc.hook())
         hdgd1 = Node(m_id=0, h=node1._h, name="yeah dude", dimension=1)
         node1.make_member_of(hdgd1)
         self.assertEqual(node1.parent_node_ids.obj_list()[0], hdgd1)
         self.assertEqual(hdgd1.member_node_ids.obj_list()[0], node1)
 
         hdgd2 = Node(m_id=0, h=node1._h, dimension=2)
         node1.make_member_of(hdgd2)
         self.assertNotIn(hdgd2.id, node1.parent_node_ids)
 
         node1.leave_memebership_of(hdgd1)
         self.assertEqual(len(hdgd1.member_node_ids), 0)
 
     def test_inherit_from_element_edge(self):
         """Test that inheriting params with kwargs works"""
-        hook = self.meta.build_hook()
+        hook = JsOrc.hook()
         a = Edge(
             name="my edge",
             m_id=0,
             h=hook,
         )
         a.connect(Node(m_id=0, h=hook), Node(m_id=0, h=hook)),
         self.assertEqual(a.name, "my edge")
```

### Comparing `jaseci-1.4.0.9/jaseci/tests/test_progs.py` & `jaseci-1.4.1.0/jaseci/tests/test_progs.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,99 +1,97 @@
 import os
 import pytest
 from unittest import TestCase
-from jaseci.svc import ServiceState
 
 import jaseci.tests.jac_test_progs as jtp
-from jaseci.actor.sentinel import Sentinel
-from jaseci.graph.graph import Graph
-from jaseci.graph.node import Node
-from jaseci.svc import MetaService
+from jaseci.prim.sentinel import Sentinel
+from jaseci.prim.graph import Graph
+from jaseci.prim.node import Node
 from jaseci.utils.utils import TestCaseHelper
+from jaseci.jsorc.jsorc import JsOrc
+from jaseci.jsorc.jsorc_utils import State
 
 
-class JacTests(TestCaseHelper, TestCase):
+class ProgTests(TestCaseHelper, TestCase):
     """Unit tests for Jac language"""
 
     def setUp(self):
         super().setUp()
 
-        self.meta = MetaService()
-
     def tearDown(self):
         super().tearDown()
 
     def test_bug_check1(self):
         self.logger_on()
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtp.bug_check1)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         report = test_walker.report
         self.assertEqual(report[0][0], "THIS IS AN INTENT_LABEL")
 
     def test_action_load_std_lib(self):
-        mast = self.meta.build_super_master()
+        mast = JsOrc.super_master()
         mast.sentinel_register(name="test", code=jtp.action_load_std_lib)
         report = mast.general_interface_to_api(
             api_name="walker_run", params={"name": "aload"}
         )["report"]
         self.assertEqual(report[0], True)
 
     def test_action_load_std_lib_only_super(self):
-        mast = self.meta.build_master()
+        mast = JsOrc.master()
         mast.sentinel_register(name="test", code=jtp.action_load_std_lib)
         report = mast.general_interface_to_api(
             api_name="walker_run", params={"name": "aload"}
         )
         report = report["report"]
         self.assertEqual(report[0], False)
 
     def test_globals(self):
-        sent = Sentinel(m_id=0, h=self.meta.build_hook())
+        sent = Sentinel(m_id=0, h=JsOrc.hook())
         gph = Graph(m_id=0, h=sent._h)
         sent.register_code(jtp.globals)
         test_walker = sent.run_architype("init")
         test_walker.prime(gph)
         test_walker.run()
         report = test_walker.report
         self.assertEqual(report, ["testing", 56])
 
     def test_net_root_std_lib(self):
-        mast = self.meta.build_master()
+        mast = JsOrc.master()
         mast.sentinel_register(name="test", code=jtp.net_root_std_lib)
         report = mast.general_interface_to_api(
             api_name="walker_run", params={"name": "init"}
         )["report"]
         self.assertEqual(report[0][0], report[0][1])
         self.assertEqual(report[0][1], report[1][1])
         self.assertNotEqual(report[1][0], report[1][1])
 
     def test_or_stmt(self):
-        mast = self.meta.build_master()
+        mast = JsOrc.master()
         mast.sentinel_register(name="test", code=jtp.or_stmt)
         report = mast.general_interface_to_api(
             api_name="walker_run", params={"name": "init"}
         )["report"]
         self.assertEqual(report, [[3.4, "Hello"]])
 
     def test_nd_equals(self):
-        mast = self.meta.build_master()
+        mast = JsOrc.master()
         mast.sentinel_register(name="test", code=jtp.nd_equals_error_correct_line)
         report = mast.general_interface_to_api(
             api_name="walker_run", params={"name": "init"}
         )
         self.assertIn("line 3", report["errors"][0])
 
     def test_strange_ability_bug(self):
         import json
 
-        mast = self.meta.build_master()
+        mast = JsOrc.master()
         mast.sentinel_register(name="test", code=jtp.strange_ability_bug)
         report = mast.general_interface_to_api(
             api_name="walker_run", params={"name": "travel"}
         )["report"]
         mast.sentinel_register(name="test", code=jtp.strange_ability_bug, auto_run="")
         report += mast.general_interface_to_api(
             api_name="walker_run", params={"name": "travel"}
@@ -105,15 +103,15 @@
         )["report"]
         report += mast.general_interface_to_api(
             api_name="walker_run", params={"name": "travel"}
         )["report"]
         self.assertEqual(report, ["Showing", "Showing", "Showing", "Showing"])
 
     def test_node_inheritance(self):
-        mast = self.meta.build_master()
+        mast = JsOrc.master()
         mast.sentinel_register(name="test", code=jtp.node_inheritance, auto_run="")
         report = mast.general_interface_to_api(
             api_name="walker_run", params={"name": "init"}
         )
         del report["final_node"]
         self.assertEqual(
             report,
@@ -127,163 +125,163 @@
                 ],
                 "success": True,
                 "yielded": False,
             },
         )
 
     def test_inherited_ref(self):
-        mast = self.meta.build_master()
+        mast = JsOrc.master()
         mast.sentinel_register(name="test", code=jtp.inherited_ref, auto_run="")
         report = mast.general_interface_to_api(
             api_name="walker_run", params={"name": "init"}
         )
         self.assertEqual(len(report["report"]), 12)
 
     def test_node_inheritance_chain_check(self):
-        mast = self.meta.build_master()
+        mast = JsOrc.master()
         mast.sentinel_register(
             name="test", code=jtp.node_inheritance_chain_check, auto_run=""
         )
         report = mast.general_interface_to_api(
             api_name="walker_run", params={"name": "init"}
         )
         self.assertEqual(report["success"], False)
 
     def test_global_reregistering(self):
-        mast = self.meta.build_master()
+        mast = JsOrc.master()
         mast.sentinel_register(name="test", code=jtp.global_reregistering)
         self.assertTrue(mast.active_snt().is_active)
         mast.sentinel_set(snt=mast.active_snt(), code=jtp.global_reregistering)
         self.assertTrue(mast.active_snt().is_active)
         mast.sentinel_register(name="test", code=jtp.global_reregistering)
         self.assertTrue(mast.active_snt().is_active)
 
     def test_vector_cos_sim_check(self):
-        mast = self.meta.build_master()
+        mast = JsOrc.master()
         mast.sentinel_register(name="test", code=jtp.vector_cos_sim_check, auto_run="")
         report = mast.general_interface_to_api(
             api_name="walker_run", params={"name": "init"}
         )["report"]
         self.assertEqual(len(report), 1)
         self.assertEqual(type(report[0]), float)
 
     def test_multi_breaks(self):
-        mast = self.meta.build_master()
+        mast = JsOrc.master()
         mast.sentinel_register(name="test", code=jtp.multi_breaks, auto_run="")
         report = mast.general_interface_to_api(
             api_name="walker_run", params={"name": "init"}
         )["report"]
         self.assertEqual(len(report), 15)
         self.assertEqual(report[14], 180)
 
     def test_reffy_deref_check(self):
-        mast = self.meta.build_master()
+        mast = JsOrc.master()
         mast.sentinel_register(name="test", code=jtp.reffy_deref_check, auto_run="")
         report = mast.general_interface_to_api(
             api_name="walker_run", params={"name": "init"}
         )["report"]
         self.assertFalse(report[0])
         self.assertTrue(report[1])
 
     def test_vanishing_can_check(self):
-        mast = self.meta.build_super_master()
+        mast = JsOrc.super_master()
         mast.actions_load_local("jaseci/tests/infer.py")
         mast.sentinel_register(name="test", code=jtp.vanishing_can_check, auto_run="")
         mast.general_interface_to_api(api_name="walker_run", params={"name": "init"})
         report = mast.general_interface_to_api(
             api_name="walker_run", params={"name": "init"}
         )["report"]
         self.assertEqual(report, ["2022-01-01T00:00:00"])
         mast.propagate_access("public")
-        mast2 = self.meta.build_super_master(h=mast._h)
+        mast2 = JsOrc.super_master(h=mast._h)
         mast.active_snt().run_architype(name="plain", kind="node", caller=mast2)
         report = mast.general_interface_to_api(
             api_name="walker_run", params={"name": "init"}
         )["report"]
         self.assertEqual(report, ["2022-01-01T00:00:00"])
 
     def test_jasecilib_alias_list(self):
-        mast = self.meta.build_master()
+        mast = JsOrc.master()
         mast.sentinel_register(name="test", code=jtp.jasecilib_alias_list, auto_run="")
         report = mast.general_interface_to_api(
             api_name="walker_run", params={"name": "init"}
         )["report"]
         self.assertGreater(len(report[0].keys()), 3)
 
     def test_jasecilib_params(self):
-        mast = self.meta.build_master()
+        mast = JsOrc.master()
         mast.sentinel_register(name="test", code=jtp.jasecilib_params, auto_run="")
         report = mast.general_interface_to_api(
             api_name="walker_run", params={"name": "init"}
         )["report"]
         self.assertIn("j_r_acc_ids", report[0][0].keys())
 
     def test_jasecilib_create_user(self):
-        mast = self.meta.build_master()
+        mast = JsOrc.master()
         mast.sentinel_register(name="test", code=jtp.jasecilib_create_user, auto_run="")
         report = mast.general_interface_to_api(
             api_name="walker_run", params={"name": "init"}
         )["report"]
         self.assertEqual(report[0]["user"]["name"], "daman@gmail.com")
 
     def test_root_is_node_type(self):
-        mast = self.meta.build_master()
+        mast = JsOrc.master()
         mast.sentinel_register(name="test", code=jtp.root_is_node_type, auto_run="")
         report = mast.general_interface_to_api(
             api_name="walker_run", params={"name": "init"}
         )
         self.assertEqual(report["report"][0], "JAC_TYPE.NODE")
 
     def test_walker_with_exit_after_node(self):
-        mast = self.meta.build_master()
+        mast = JsOrc.master()
         mast.sentinel_register(
             name="test", code=jtp.walker_with_exit_after_node, auto_run=""
         )
         report = mast.general_interface_to_api(
             api_name="walker_run", params={"name": "init"}
         )
         self.assertEqual(report["report"], [1, 1, 3, 1, 3, 1, 3, 1, 3, 43])
 
     def test_depth_first_take(self):
-        mast = self.meta.build_master()
+        mast = JsOrc.master()
         mast.sentinel_register(name="test", code=jtp.depth_first_take, auto_run="")
         report = mast.general_interface_to_api(
             api_name="walker_run", params={"name": "init"}
         )
         self.assertEqual(report["report"], [1, 2, 3, 4, 5, 6, 7])
 
     def test_breadth_first_take(self):
-        mast = self.meta.build_master()
+        mast = JsOrc.master()
         mast.sentinel_register(name="test", code=jtp.breadth_first_take, auto_run="")
         report = mast.general_interface_to_api(
             api_name="walker_run", params={"name": "init"}
         )
         self.assertEqual(report["report"], [1, 2, 5, 3, 4, 6, 7])
 
     def test_inheritance_override_here_check(self):
-        mast = self.meta.build_master()
+        mast = JsOrc.master()
         mast.sentinel_register(
             name="test", code=jtp.inheritance_override_here_check, auto_run=""
         )
         report = mast.general_interface_to_api(
             api_name="walker_run", params={"name": "init"}
         )
         self.assertEqual(report["report"], [9, 9, 10])
 
     def test_dot_private_hidden(self):
-        mast = self.meta.build_master()
+        mast = JsOrc.master()
         mast.sentinel_register(name="test", code=jtp.dot_private_hidden, auto_run="")
         mast.general_interface_to_api(api_name="walker_run", params={"name": "init"})
         report = mast.general_interface_to_api(
             api_name="graph_get", params={"mode": "dot", "detailed": True}
         )
         self.assertNotIn("j=", report)
 
     def test_check_destroy_node_has_var(self):
-        mast = self.meta.build_master()
+        mast = JsOrc.master()
         mast.sentinel_register(
             name="test", code=jtp.check_destroy_node_has_var, auto_run=""
         )
         report = mast.general_interface_to_api(
             api_name="walker_run", params={"name": "create"}
         )
         self.assertEqual(mast._h.get_object_distribution()[Node], 2)
@@ -291,15 +289,15 @@
         report = mast.general_interface_to_api(
             api_name="walker_run", params={"name": "remove"}
         )
         self.assertEqual(mast._h.get_object_distribution()[Node], 1)
         self.assertEqual(report["report"][0], "JAC_TYPE.NULL")
 
     def test_for_loop_dict(self):
-        mast = self.meta.build_master()
+        mast = JsOrc.master()
         mast.sentinel_register(
             name="test", code=jtp.check_dict_for_in_loop, auto_run=""
         )
         res = mast.general_interface_to_api(
             api_name="walker_run", params={"name": "for_loop_dict"}
         )
 
@@ -318,60 +316,87 @@
                 "0 : 5",
                 "1 : 6",
                 "2 : 7",
             ],
         )
 
     def test_var_as_key_for_dict(self):
-        mast = self.meta.build_master()
+        mast = JsOrc.master()
         mast.sentinel_register(
             name="test", code=jtp.check_dict_for_in_loop, auto_run=""
         )
         res = mast.general_interface_to_api(
             api_name="walker_run", params={"name": "var_as_key_for_dict"}
         )
 
         self.assertEqual(res["report"], [{"key1": "key1", "key2": 2}])
         self.assertIn("Key is not str type : <class 'int'>!", res["errors"][0])
 
+    def test_list_pairwise(self):
+        mast = JsOrc.master()
+        mast.sentinel_register(name="test", code=jtp.list_pairwise, auto_run="")
+
+        res = mast.general_interface_to_api(
+            api_name="walker_run", params={"name": "init"}
+        )
+
+        self.assertEqual(
+            res["report"],
+            [[[1, 2], [2, 3], [3, 4]]],
+        )
+
+    def test_list_unique(self):
+        mast = JsOrc.master()
+        mast.sentinel_register(name="test", code=jtp.list_unique, auto_run="")
+
+        res = mast.general_interface_to_api(
+            api_name="walker_run", params={"name": "init"}
+        )
+
+        self.assertEqual(
+            res["report"],
+            [[1, 2, 3, 4, 5]],
+        )
+
     def test_new_additional_builtin(self):
-        mast = self.meta.build_master()
+        mast = JsOrc.master()
         mast.sentinel_register(name="test", code=jtp.check_new_builtin, auto_run="")
 
         res = mast.general_interface_to_api(
             api_name="walker_run", params={"name": "init"}
         )
 
         self.assertEqual(
             res["report"],
             [{"test": "test"}, 1, "1 2 3 4", "1 2 3 4"],
         )
 
     def test_continue_issue(self):
-        mast = self.meta.build_master()
+        mast = JsOrc.master()
         mast.sentinel_register(name="test", code=jtp.continue_issue, auto_run="")
         res = mast.general_interface_to_api(
             api_name="walker_run", params={"name": "init"}
         )
         self.assertEqual(res["report"], [1, 2, 3, 4, 5, 6, 7, 8, "apple"])
 
     def test_registering_dict_as_ir(self):
-        mast = self.meta.build_master()
+        mast = JsOrc.master()
         mast.sentinel_register(name="test", code=jtp.continue_issue, auto_run="")
         code_dict = mast.sentinel_get(snt=mast.active_snt(), mode="ir")
         self.assertEqual(type(code_dict), dict)
         mast.sentinel_register(name="test", code=code_dict, mode="ir", auto_run="")
         res = mast.general_interface_to_api(
             api_name="walker_run", params={"name": "init"}
         )
         self.assertEqual(res["report"], [1, 2, 3, 4, 5, 6, 7, 8, "apple"])
 
+    @pytest.mark.order(2)
     def test_async_syntax_with_celery(self):
-        mast = self.meta.build_master()
-        if not mast._h.task.is_running():
+        mast = JsOrc.master()
+        if not JsOrc.svc("task").is_running():
             self.skip_test("Celery not running")
         mast.sentinel_register(name="test", code=jtp.async_syntax, auto_run="")
         res = mast.general_interface_to_api(
             api_name="walker_run",
             params={"name": "simple_async", "ctx": {"sample": "name"}},
         )
 
@@ -404,17 +429,50 @@
             params={"task_id": res["result"]},
         )
 
         self.assertEqual(report4, res)
         self.assertEqual(2, res["result"]["anchor"])
         self.assertEqual([2, 2], res["result"]["response"]["report"])
 
+    @pytest.mark.order(3)
+    def test_async_syntax_with_update_and_celery(self):
+        mast = JsOrc.master()
+        if not JsOrc.svc("task").is_running():
+            self.skip_test("Celery not running")
+        mast.sentinel_register(
+            name="test", code=jtp.async_syntax_with_update, auto_run="init"
+        )
+        res = mast.general_interface_to_api(
+            api_name="walker_run",
+            params={"name": "update_value", "ctx": {}},
+        )
+
+        self.assertTrue(res["is_queued"])
+
+        res = mast.general_interface_to_api(
+            api_name="walker_queue_wait",
+            params={"task_id": res["result"], "timeout": 15},
+        )
+
+        self.assertEqual("SUCCESS", res["status"])
+        self.assertTrue(res["result"]["response"]["report"][0]["value"])
+
+        # remove the node on current _h.mem and let the redis repopulate it
+        mast._h.mem.pop(res["result"]["response"]["final_node"], None)
+
+        res = mast.general_interface_to_api(
+            api_name="walker_run",
+            params={"name": "get_value", "ctx": {}},
+        )
+
+        self.assertTrue(res["report"][0]["value"])
+
     def test_async_syntax_without_celery(self):
-        mast = self.meta.build_master()
-        mast._h.task.state = ServiceState.NOT_STARTED
+        mast = JsOrc.master()
+        JsOrc.svc("task").state = State.NOT_STARTED
         mast.sentinel_register(name="test", code=jtp.async_syntax, auto_run="")
         res = mast.general_interface_to_api(
             api_name="walker_run",
             params={"name": "simple_async", "ctx": {"sample": "name"}},
         )
 
         # no celery running
@@ -433,19 +491,19 @@
 
         res = res["result"]["report"][5]
 
         # no celery running
         self.assertFalse(res["is_queued"])
         self.assertEqual(2, res["result"])
 
-        mast._h.task.state = ServiceState.RUNNING
+        JsOrc.svc("task").state = State.RUNNING
 
     def test_async_sync_syntax_with_celery(self):
-        mast = self.meta.build_master()
-        if not mast._h.task.is_running():
+        mast = JsOrc.master()
+        if not JsOrc.svc("task").is_running():
             self.skip_test("Celery not running")
         mast.sentinel_register(name="test", code=jtp.async_syntax, auto_run="")
         res = mast.general_interface_to_api(
             api_name="walker_run",
             params={"name": "simple_async_with_sync", "ctx": {"sample": "name"}},
         )
 
@@ -479,16 +537,16 @@
         )
 
         self.assertEqual(report4, res)
         self.assertEqual(2, res["result"]["anchor"])
         self.assertEqual([2, 2], res["result"]["response"]["report"])
 
     def test_async_sync_syntax_without_celery(self):
-        mast = self.meta.build_master()
-        mast._h.task.state = ServiceState.NOT_STARTED
+        mast = JsOrc.master()
+        JsOrc.svc("task").state = State.NOT_STARTED
         mast.sentinel_register(name="test", code=jtp.async_syntax, auto_run="")
         res = mast.general_interface_to_api(
             api_name="walker_run",
             params={"name": "simple_async_with_sync", "ctx": {"sample": "name"}},
         )
 
         # no celery running
@@ -507,43 +565,41 @@
 
         res = res["result"]["report"][5]
 
         # no celery running
         self.assertFalse(res["is_queued"])
         self.assertEqual(2, res["result"])
 
-        mast._h.task.state = ServiceState.RUNNING
+        JsOrc.svc("task").state = State.RUNNING
 
     def test_block_scope_check(self):
-        mast = self.meta.build_master()
-        mast._h.task.state = ServiceState.NOT_STARTED
+        mast = JsOrc.master()
         mast.sentinel_register(name="test", code=jtp.block_scope_check, auto_run="")
         res = mast.general_interface_to_api(
             api_name="walker_run", params={"name": "init"}
         )
         self.assertEqual(res["report"][-1], 10)
 
     def test_ignore_check(self):
-        mast = self.meta.build_master()
-        mast._h.task.state = ServiceState.NOT_STARTED
+        mast = JsOrc.master()
         res = mast.sentinel_register(name="test", code=jtp.ignore_check, auto_run="")
         res = mast.general_interface_to_api(
             api_name="walker_run", params={"name": "init"}
         )
         self.assertEqual(len(res["report"]), 9)
 
     @pytest.mark.order(1)
     def test_module_on_async(self):
-        mast = self.meta.build_super_master()
-        if not mast._h.task.is_running():
+        mast = JsOrc.super_master()
+        if not JsOrc.svc("task").is_running():
             self.skip_test("Celery not running")
 
         with open("jaseci/tests/fixtures/non_existing_action.py", "w") as file:
             file.write(
-                "from jaseci.actions.live_actions import jaseci_action\n@jaseci_action(act_group=['sim1'])\ndef tester():\n\treturn 1"
+                "from jaseci.jsorc.live_actions import jaseci_action\n@jaseci_action(act_group=['sim1'])\ndef tester():\n\treturn 1"
             )
 
         mast.sentinel_register(name="test", code=jtp.async_module, auto_run="")
 
         # sequence is relevant
         mast.actions_load_local("jaseci/tests/fixtures/non_existing_action.py")
         mast.actions_load_local("jaseci/tests/fixtures/existing_action.py")
@@ -581,7 +637,35 @@
         # return would be [None, None] if not yet fixed
         self.assertEqual([None, 2], res["result"]["response"]["report"])
 
         self.assertIn(
             "Cannot execute sim1.tester - Not Found",
             res["result"]["response"]["errors"][0],
         )
+
+    def test_walker_run_with_null_arguments(self):
+        mast = JsOrc.master()
+        res = mast.sentinel_register(
+            name="test", code=jtp.walker_null_args, auto_run=""
+        )
+        res = mast.general_interface_to_api(
+            api_name="walker_run",
+            params={"name": "a", "ctx": {}},
+        )
+        self.assertTrue(res["success"])
+        self.assertTrue(res["report"], [None, None])
+        self.assertIsNone(res.get("errors"))
+
+    def test_json_casting(self):
+        mast = JsOrc.master()
+        mast.sentinel_register(name="test", code=jtp.json_casting, auto_run="")
+
+        res = mast.general_interface_to_api(
+            api_name="walker_run",
+            params={"name": "json_casting", "ctx": {}},
+        )
+
+        self.assertTrue(res["success"])
+        self.assertEqual(
+            res["report"],
+            ['{"test": 1}', {"test2": 2}],
+        )
```

### Comparing `jaseci-1.4.0.9/jaseci/tests/test_stack.py` & `jaseci-1.4.1.0/jaseci/tests/test_stack.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,81 +30,81 @@
         life_node = self.mast._h.get_obj(self.mast._m_id, ret["final_node"])
         life_node.context.pop("note")
         ret = self.call(self.mast, ["walker_run", {"name": "print_life_note"}])
         self.assertTrue(ret["success"])
 
     def test_action_module_list(self):
         ret = self.call(self.smast, ["actions_module_list", {}])
-        self.assertIn("jaseci.actions.standard.rand", ret)
-        self.assertIn("jaseci.actions.standard.std", ret)
-        self.assertIn("jaseci.actions.standard.file", ret)
+        self.assertIn("jaseci.extens.act_lib.rand", ret)
+        self.assertIn("jaseci.extens.act_lib.std", ret)
+        self.assertIn("jaseci.extens.act_lib.file", ret)
 
     def test_action_module_unload_reload(self):
         ret = self.call(self.smast, ["actions_module_list", {}])
         before = len(ret)
         ret = self.call(
             self.smast,
-            ["actions_unload_module", {"name": "jaseci.actions.standard.rand"}],
+            ["actions_unload_module", {"name": "jaseci.extens.act_lib.rand"}],
         )
         ret = self.call(
             self.smast,
-            ["actions_unload_module", {"name": "jaseci.actions.standard.file"}],
+            ["actions_unload_module", {"name": "jaseci.extens.act_lib.file"}],
         )
         ret = self.call(self.smast, ["actions_module_list", {}])
         self.assertEqual(len(ret), before - 2)
         ret = self.call(
             self.smast,
-            ["actions_load_module", {"mod": "jaseci.actions.standard.rand"}],
+            ["actions_load_module", {"mod": "jaseci.extens.act_lib.rand"}],
         )
         ret = self.call(
             self.smast,
-            ["actions_load_module", {"mod": "jaseci.actions.standard.file"}],
+            ["actions_load_module", {"mod": "jaseci.extens.act_lib.file"}],
         )
         ret = self.call(self.smast, ["actions_module_list", {}])
         self.assertEqual(len(ret), before)
 
     def test_action_module_unload_reload_aliased(self):
         ret = self.call(self.smast, ["actions_module_list", {}])
         before = len(ret)
         ret = self.call(
             self.smast,
-            ["actions_unload_module", {"name": "jaseci.actions.standard.vector"}],
+            ["actions_unload_module", {"name": "jaseci.extens.act_lib.vector"}],
         )
         ret = self.call(self.smast, ["actions_module_list", {}])
         self.assertEqual(len(ret), before - 1)
         self.assertNotIn("vector.cos_sim", self.call(self.smast, ["actions_list", {}]))
         ret = self.call(
             self.smast,
-            ["actions_load_module", {"mod": "jaseci.actions.standard.vector"}],
+            ["actions_load_module", {"mod": "jaseci.extens.act_lib.vector"}],
         )
         ret = self.call(self.smast, ["actions_module_list", {}])
         self.assertEqual(len(ret), before)
 
     def test_action_unload(self):
         ret = self.call(self.smast, ["actions_module_list", {}])
         before = len(ret)
         ret = self.call(self.smast, ["actions_list", {"name": "rand"}])
         for i in ret:
             self.call(self.smast, ["actions_unload_action", {"name": i}])
         ret = self.call(self.smast, ["actions_module_list", {}])
         self.assertEqual(len(ret), before - 1)
         ret = self.call(
             self.smast,
-            ["actions_load_module", {"mod": "jaseci.actions.standard.rand"}],
+            ["actions_load_module", {"mod": "jaseci.extens.act_lib.rand"}],
         )
 
     def test_action_set_unload(self):
         ret = self.call(self.smast, ["actions_module_list", {}])
         before = len(ret)
         ret = self.call(self.smast, ["actions_unload_actionset", {"name": "rand"}])
         ret = self.call(self.smast, ["actions_module_list", {}])
         self.assertEqual(len(ret), before - 1)
         ret = self.call(
             self.smast,
-            ["actions_load_module", {"mod": "jaseci.actions.standard.rand"}],
+            ["actions_load_module", {"mod": "jaseci.extens.act_lib.rand"}],
         )
 
     def test_sentinel_missing_architype(self):
         """
         Test when the original sentinel is missing the corresponding architype for a
         node
         """
@@ -192,7 +192,29 @@
                 {"auto_run": "", "code": self.load_jac("simple.jac")},
             ],
         )
 
         ret = self.call(self.smast, ["walker_run", {"name": "deep_except"}])
         self.assertTrue(ret["success"])
         self.assertIn("xxxx.xxxx", ret["report"][2]["msg"])
+
+    def test_dot_profiling_in_walker(self):
+        ret = self.call(
+            self.mast,
+            ["sentinel_register", {"code": self.load_jac("simple.jac")}],
+        )
+        ret = self.call(self.mast, ["walker_run", {"name": "init", "profiling": True}])
+        self.assertIn("digraph", ret["profile"]["graph"])
+        self.assertIn("jaseci", ret["profile"]["graph"])
+        self.assertGreater(len(ret["profile"]["graph"]), 1000)
+
+    def test_jac_profiling_in_walker(self):
+        ret = self.call(
+            self.mast,
+            ["sentinel_register", {"code": self.load_jac("simple.jac")}],
+        )
+        ret = self.call(
+            self.mast, ["walker_run", {"name": "complex", "profiling": True}]
+        )
+        print(ret["profile"]["jac"])
+        self.assertIn("cum_time", ret["profile"]["jac"])
+        self.assertIn("run_walker", ret["profile"]["graph"])
```

### Comparing `jaseci-1.4.0.9/jaseci/tests/test_stripe.py` & `jaseci-1.4.1.0/jaseci/tests/test_stripe.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 import stripe
 from unittest.mock import Mock
-from unittest import mock
 from jaseci.utils.test_core import CoreTest, jac_testcase
-from jaseci.svc.stripe.config import STRIPE_CONFIG
-from jaseci.svc.meta import MetaService
+from jaseci.jsorc.jsorc import JsOrc
 
 
 class StripeTests(CoreTest):
     """Unit tests for Stripe actions"""
 
     fixture_src = __file__
 
     @classmethod
     def setUpClass(cls):
-        STRIPE_CONFIG["enabled"] = True
-        STRIPE_CONFIG[
+        config = JsOrc.settings("STRIPE_CONFIG")
+        config["enabled"] = True
+        config[
             "api_key"
         ] = "sk_test_51JWUIeCZO78n7fsZnPvualWhmJg1DcCI332kKnWF3q2sKGwnPADjEmNblfFWi4pWAWPuJwHxpeSoJGc0J5ButHN900Q2xBz1se"
-        STRIPE_CONFIG["webhook_key"] = "test_webhook_key"
+        config["webhook_key"] = "test_webhook_key"
 
-        meta = MetaService()
-        hook = meta.build_hook()
-
-        meta.get_service("stripe").reset(hook)
+        JsOrc.svc_reset("stripe")
 
         super(StripeTests, cls).setUpClass()
         stripe.Product.create = Mock()
         stripe.Price.create = Mock()
         stripe.Product.list = Mock()
         stripe.Customer.create = Mock()
         stripe.Customer.retrieve = Mock()
```

### Comparing `jaseci-1.4.0.9/jaseci/utils/id_list.py` & `jaseci-1.4.1.0/jaseci/utils/id_list.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.0.9/jaseci/utils/json_handler.py` & `jaseci-1.4.1.0/jaseci/utils/json_handler.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import json
 from json import JSONDecoder, JSONEncoder
-from uuid import UUID
 
-from jaseci.svc import MetaService
+from jaseci.jsorc.jsorc import JsOrc
 from jaseci.utils.id_list import IdList
 from jaseci.utils.utils import logger
 
 
 class JaseciJsonEncoder(JSONEncoder):
     def default(self, obj):
-        from jaseci.element.element import Element
+        from jaseci.prim.element import Element
 
         if isinstance(obj, Element):
             return {"__mem_id__": obj.jid}
         else:
             return super().default(obj)
 
 
@@ -41,27 +40,31 @@
                 for k in obj[key]:
                     self.transform(obj[key], k)
         elif isinstance(obj[key], (list, tuple)):
             for idx, k in enumerate(obj[key]):
                 self.transform(obj[key], idx)
 
     def convert(self, urn):
-        return MetaService().build_hook().get_obj_from_store(urn)
+        return JsOrc.hook().get_obj_from_store(urn)
 
 
 def json_str_to_jsci_dict(input_str, parent_obj=None):
     """
     Helper function to convert JSON strings to dictionarys with _ids list
     conversions from hex to UUID
 
     ret_obj is the owning object for id_list objects
     """
 
     try:
-        obj_fields = json.loads(input_str)
+        obj_fields = json.loads(input_str, cls=JaseciJsonDecoder)
     except ValueError:
         logger.error(str(f"Invalid jsci_obj string {input_str} on {parent_obj.jid}"))
         obj_fields = {}
+    jsci_dict_normalize(obj_fields, parent_obj)
+    return obj_fields
+
+
+def jsci_dict_normalize(obj_fields, parent_obj):
     for i in obj_fields.keys():
         if str(i).endswith("_ids") and isinstance(obj_fields[i], list):
             obj_fields[i] = IdList(parent_obj=parent_obj, in_list=obj_fields[i])
-    return obj_fields
```

### Comparing `jaseci-1.4.0.9/jaseci/utils/log_utils.py` & `jaseci-1.4.1.0/jaseci/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `jaseci-1.4.0.9/jaseci/utils/test_core.py` & `jaseci-1.4.1.0/jaseci/utils/test_core.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,62 @@
 import os
+import unittest
 from unittest import TestCase
 
-from jaseci.svc import MetaService
+from jaseci.jsorc.jsorc import JsOrc
 from jaseci.utils.utils import TestCaseHelper
 
 
 class CoreTest(TestCaseHelper, TestCase):
     """Unit tests for Jac Core APIs"""
 
     fixture_src = __file__
 
-    def setUp(self, run_svcs=False):
+    def setUp(self):
         super().setUp()
-        self.meta = MetaService(run_svcs=run_svcs)
-        self.smast = self.meta.build_super_master()
-        self.mast = self.meta.build_master(h=self.smast._h)
+        self.smast = JsOrc.super_master()
+        self.mast = JsOrc.master(h=self.smast._h)
 
     def tearDown(self):
         super().tearDown()
 
     def call(self, mast, pl):
         ret = mast.general_interface_to_api(api_name=pl[0], params=pl[1])
         return ret
 
     def load_jac(self, fn):
         with open(os.path.dirname(self.fixture_src) + "/fixtures/" + fn) as f:
             return f.read()
 
 
-def jac_testcase(jac_file: str, test_name: str):
+def jac_testcase(jac_file: str, test_name: str, log_out: bool = False):
     """decorator for test cases"""
 
     def decorator(func):
         def wrapper(self):
+            if log_out:
+                self.logger_on()
             self.call(
                 self.mast,
                 ["sentinel_register", {"code": self.load_jac(jac_file)}],
             )
             ret = self.call(self.mast, ["walker_run", {"name": test_name}])
             func(self, ret)
+            if log_out:
+                self.logger_off()
 
         return wrapper
 
     return decorator
+
+
+def skip_without_redis(test):
+    """
+    Skip test if expected not to work without redis.
+    """
+
+    def skipper(*args, **kwargs):
+        if not JsOrc.svc("redis").is_running():
+            raise unittest.SkipTest("No Redis!")
+        test(*args, **kwargs)
+
+    return skipper
```

### Comparing `jaseci-1.4.0.9/jaseci.egg-info/SOURCES.txt` & `jaseci-1.4.1.0/jaseci.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -5,94 +5,90 @@
 jaseci/__init__.py
 jaseci.egg-info/PKG-INFO
 jaseci.egg-info/SOURCES.txt
 jaseci.egg-info/dependency_links.txt
 jaseci.egg-info/entry_points.txt
 jaseci.egg-info/requires.txt
 jaseci.egg-info/top_level.txt
-jaseci/actions/__init__.py
-jaseci/actions/live_actions.py
-jaseci/actions/remote_actions.py
-jaseci/actions/standard/__init__.py
-jaseci/actions/standard/date.py
-jaseci/actions/standard/elastic.py
-jaseci/actions/standard/file.py
-jaseci/actions/standard/internal.py
-jaseci/actions/standard/jaseci.py
-jaseci/actions/standard/mail.py
-jaseci/actions/standard/net.py
-jaseci/actions/standard/rand.py
-jaseci/actions/standard/request.py
-jaseci/actions/standard/std.py
-jaseci/actions/standard/stripe.py
-jaseci/actions/standard/task.py
-jaseci/actions/standard/url.py
-jaseci/actions/standard/vector.py
-jaseci/actions/standard/webtool.py
-jaseci/actions/standard/zlib.py
-jaseci/actions/standard/tests/__init__.py
-jaseci/actions/standard/tests/test_file_lib.py
-jaseci/actions/standard/tests/test_mail_lib.py
-jaseci/actions/standard/tests/test_net_lib.py
-jaseci/actions/standard/tests/test_std_lib.py
-jaseci/actions/standard/tests/test_url.py
-jaseci/actions/standard/tests/test_vector.py
-jaseci/actions/standard/tests/test_webtool.py
-jaseci/actions/standard/tests/test_zlib.py
-jaseci/actions/tests/__init__.py
-jaseci/actions/tests/std_test_code.py
-jaseci/actions/tests/test_actions.py
-jaseci/actions/tests/test_std.py
-jaseci/actor/__init__.py
-jaseci/actor/architype.py
-jaseci/actor/sentinel.py
-jaseci/actor/walker.py
-jaseci/api/__init__.py
-jaseci/api/actions_api.py
-jaseci/api/alias_api.py
-jaseci/api/architype_api.py
-jaseci/api/config_api.py
-jaseci/api/global_api.py
-jaseci/api/graph_api.py
-jaseci/api/interface.py
-jaseci/api/jac_api.py
-jaseci/api/jsorc_api.py
-jaseci/api/logger_api.py
-jaseci/api/master_api.py
-jaseci/api/object_api.py
-jaseci/api/prometheus_api.py
-jaseci/api/queue_api.py
-jaseci/api/sentinel_api.py
-jaseci/api/super_api.py
-jaseci/api/user_api.py
-jaseci/api/walker_api.py
-jaseci/api/webhook_api.py
-jaseci/api/tests/__init__.py
-jaseci/api/tests/test_architype_api.py
-jaseci/api/tests/test_global_api.py
-jaseci/api/tests/test_graph_api.py
-jaseci/api/tests/test_logger_api.py
-jaseci/api/tests/test_sentinel_api.py
-jaseci/api/tests/test_user_api.py
-jaseci/api/tests/test_walker_api.py
-jaseci/attr/__init__.py
-jaseci/attr/action.py
-jaseci/attr/item.py
-jaseci/element/__init__.py
-jaseci/element/element.py
-jaseci/element/master.py
-jaseci/element/obj_mixins.py
-jaseci/element/super_master.py
-jaseci/graph/__init__.py
-jaseci/graph/edge.py
-jaseci/graph/graph.py
-jaseci/graph/node.py
-jaseci/hook/__init__.py
-jaseci/hook/memory.py
-jaseci/hook/redis.py
+jaseci/cli_tools/__init__.py
+jaseci/cli_tools/book_tools.py
+jaseci/cli_tools/jsctl.py
+jaseci/cli_tools/tests/__init__.py
+jaseci/cli_tools/tests/test_jsctl.py
+jaseci/extens/__init__.py
+jaseci/extens/act_lib/__init__.py
+jaseci/extens/act_lib/date.py
+jaseci/extens/act_lib/elastic.py
+jaseci/extens/act_lib/file.py
+jaseci/extens/act_lib/internal.py
+jaseci/extens/act_lib/jaseci.py
+jaseci/extens/act_lib/mail.py
+jaseci/extens/act_lib/net.py
+jaseci/extens/act_lib/rand.py
+jaseci/extens/act_lib/regex.py
+jaseci/extens/act_lib/request.py
+jaseci/extens/act_lib/std.py
+jaseci/extens/act_lib/stripe.py
+jaseci/extens/act_lib/task.py
+jaseci/extens/act_lib/url.py
+jaseci/extens/act_lib/vector.py
+jaseci/extens/act_lib/webtool.py
+jaseci/extens/act_lib/zip.py
+jaseci/extens/act_lib/tests/__init__.py
+jaseci/extens/act_lib/tests/std_test_code.py
+jaseci/extens/act_lib/tests/test_date.py
+jaseci/extens/act_lib/tests/test_elastic.py
+jaseci/extens/act_lib/tests/test_file_lib.py
+jaseci/extens/act_lib/tests/test_mail_lib.py
+jaseci/extens/act_lib/tests/test_net_lib.py
+jaseci/extens/act_lib/tests/test_regex.py
+jaseci/extens/act_lib/tests/test_std.py
+jaseci/extens/act_lib/tests/test_std_lib.py
+jaseci/extens/act_lib/tests/test_url.py
+jaseci/extens/act_lib/tests/test_vector.py
+jaseci/extens/act_lib/tests/test_webtool.py
+jaseci/extens/act_lib/tests/test_zlib.py
+jaseci/extens/api/__init__.py
+jaseci/extens/api/actions_api.py
+jaseci/extens/api/alias_api.py
+jaseci/extens/api/architype_api.py
+jaseci/extens/api/config_api.py
+jaseci/extens/api/global_api.py
+jaseci/extens/api/graph_api.py
+jaseci/extens/api/interface.py
+jaseci/extens/api/jac_api.py
+jaseci/extens/api/jsorc_api.py
+jaseci/extens/api/logger_api.py
+jaseci/extens/api/master_api.py
+jaseci/extens/api/object_api.py
+jaseci/extens/api/prometheus_api.py
+jaseci/extens/api/queue_api.py
+jaseci/extens/api/sentinel_api.py
+jaseci/extens/api/super_api.py
+jaseci/extens/api/user_api.py
+jaseci/extens/api/walker_api.py
+jaseci/extens/api/webhook_api.py
+jaseci/extens/api/tests/__init__.py
+jaseci/extens/api/tests/test_architype_api.py
+jaseci/extens/api/tests/test_global_api.py
+jaseci/extens/api/tests/test_graph_api.py
+jaseci/extens/api/tests/test_logger_api.py
+jaseci/extens/api/tests/test_object_api.py
+jaseci/extens/api/tests/test_sentinel_api.py
+jaseci/extens/api/tests/test_user_api.py
+jaseci/extens/api/tests/test_walker_api.py
+jaseci/extens/svc/__init__.py
+jaseci/extens/svc/elastic_svc.py
+jaseci/extens/svc/kube_svc.py
+jaseci/extens/svc/mail_svc.py
+jaseci/extens/svc/prome_svc.py
+jaseci/extens/svc/redis_svc.py
+jaseci/extens/svc/stripe_svc.py
+jaseci/extens/svc/task_svc.py
+jaseci/extens/svc/tasks.py
 jaseci/jac/__init__.py
 jaseci/jac/jac.g4
 jaseci/jac/jac_set.py
 jaseci/jac/interpreter/__init__.py
 jaseci/jac/interpreter/architype_interp.py
 jaseci/jac/interpreter/interp.py
 jaseci/jac/interpreter/sentinel_interp.py
@@ -126,65 +122,56 @@
 jaseci/jac/machine/jac_scope.py
 jaseci/jac/machine/jac_value.py
 jaseci/jac/machine/machine_state.py
 jaseci/jac/tests/__init__.py
 jaseci/jac/tests/book_code.py
 jaseci/jac/tests/test_book.py
 jaseci/jac/tests/test_lang_14.py
-jaseci/jsctl/__init__.py
-jaseci/jsctl/book_tools.py
-jaseci/jsctl/jsctl.py
-jaseci/jsctl/tests/__init__.py
-jaseci/jsctl/tests/test_jsctl.py
-jaseci/svc/__init__.py
-jaseci/svc/common.py
-jaseci/svc/config.py
-jaseci/svc/meta.py
-jaseci/svc/state.py
-jaseci/svc/actions_optimizer/__init__.py
-jaseci/svc/actions_optimizer/actions_optimizer.py
-jaseci/svc/actions_optimizer/actions_state.py
-jaseci/svc/elastic/__init__.py
-jaseci/svc/elastic/config.py
-jaseci/svc/elastic/elastic.py
-jaseci/svc/elastic/manifest.py
-jaseci/svc/jsorc-backup/__init__.py
-jaseci/svc/jsorc-backup/jaseci-redis.yaml
-jaseci/svc/jsorc-backup/jsorc.py
-jaseci/svc/jsorc-backup/promon/__init__.py
-jaseci/svc/jsorc-backup/promon/promon.py
-jaseci/svc/mail/__init__.py
-jaseci/svc/mail/config.py
-jaseci/svc/mail/mail.py
-jaseci/svc/postgres/__init__.py
-jaseci/svc/postgres/manifest.py
-jaseci/svc/prometheus/__init__.py
-jaseci/svc/prometheus/config.py
-jaseci/svc/prometheus/manifest.py
-jaseci/svc/prometheus/prometheus.py
-jaseci/svc/redis/__init__.py
-jaseci/svc/redis/config.py
-jaseci/svc/redis/manifest.py
-jaseci/svc/redis/redis.py
-jaseci/svc/stripe/__init__.py
-jaseci/svc/stripe/config.py
-jaseci/svc/stripe/stripe.py
-jaseci/svc/task/__init__.py
-jaseci/svc/task/common.py
-jaseci/svc/task/config.py
-jaseci/svc/task/task.py
+jaseci/jsorc/__init__.py
+jaseci/jsorc/jsorc.py
+jaseci/jsorc/jsorc_settings.py
+jaseci/jsorc/jsorc_utils.py
+jaseci/jsorc/live_actions.py
+jaseci/jsorc/memory.py
+jaseci/jsorc/redis.py
+jaseci/jsorc/remote_actions.py
+jaseci/jsorc/manifests/__init__.py
+jaseci/jsorc/manifests/database.yaml
+jaseci/jsorc/manifests/elastic.yaml
+jaseci/jsorc/manifests/prometheus.yaml
+jaseci/jsorc/manifests/redis.yaml
+jaseci/jsorc/tests/__init__.py
+jaseci/jsorc/tests/test_actions.py
+jaseci/jsorc/tests/test_jsorc.py
+jaseci/prim/__init__.py
+jaseci/prim/ability.py
+jaseci/prim/architype.py
+jaseci/prim/edge.py
+jaseci/prim/element.py
+jaseci/prim/graph.py
+jaseci/prim/master.py
+jaseci/prim/node.py
+jaseci/prim/obj_mixins.py
+jaseci/prim/sentinel.py
+jaseci/prim/super_master.py
+jaseci/prim/walker.py
 jaseci/tests/__init__.py
 jaseci/tests/infer.py
 jaseci/tests/jac_test_code.py
 jaseci/tests/jac_test_progs.py
 jaseci/tests/test_core.py
 jaseci/tests/test_jac.py
 jaseci/tests/test_node.py
 jaseci/tests/test_progs.py
 jaseci/tests/test_stack.py
 jaseci/tests/test_stripe.py
 jaseci/utils/__init__.py
+jaseci/utils/gprof2dot.py
 jaseci/utils/id_list.py
 jaseci/utils/json_handler.py
 jaseci/utils/log_utils.py
 jaseci/utils/test_core.py
-jaseci/utils/utils.py
+jaseci/utils/utils.py
+jaseci/utils/actions/__init__.py
+jaseci/utils/actions/actions_manager.py
+jaseci/utils/actions/actions_optimizer.py
+jaseci/utils/actions/actions_state.py
```

### Comparing `jaseci-1.4.0.9/setup.py` & `jaseci-1.4.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,24 +27,29 @@
         "docstring-parser",
         "prometheus_api_client==0.5.1",
         "prometheus-client==0.14.1",
         "kubernetes==23.6.0",
         "pytest",
         "pytest-xdist",
         "pytest-cov",
-        "gprof2dot",
-        "metadata_parser",
         "validators",
+        "psycopg2-binary==2.9.5",
+        "pygls",
+        "mock",
+        "beautifulsoup4>=4.12.2, <4.13.0",
+        "lxml>=4.9.2, <4.10.0",
+        "html5lib>=1.1, <1.2",
+        "prettytable>=3.7.0, <3.8.0",
     ],
     package_data={
         "": ["*.ini", "*.yaml", "jac.g4", "VERSION"],
     },
     entry_points={
         "console_scripts": [
-            "jsctl = jaseci.jsctl.jsctl:jsctl",
-            "jac = jaseci.jsctl.jsctl:jac",
+            "jsctl = jaseci.cli_tools.jsctl:jsctl",
+            "jac = jaseci.cli_tools.jsctl:jac",
         ]
     },
     author="Jason Mars",
     author_email="jason@jaseci.org",
     url="https://github.com/Jaseci-Labs/jaseci",
 )
```

