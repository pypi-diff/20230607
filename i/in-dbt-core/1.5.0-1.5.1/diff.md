# Comparing `tmp/in-dbt-core-1.5.0.tar.gz` & `tmp/in-dbt-core-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "in-dbt-core-1.5.0.tar", last modified: Thu Jun  1 18:21:06 2023, max compression
+gzip compressed data, was "in-dbt-core-1.5.1.tar", last modified: Wed Jun  7 11:50:36 2023, max compression
```

## Comparing `in-dbt-core-1.5.0.tar` & `in-dbt-core-1.5.1.tar`

### file list

```diff
@@ -1,312 +1,312 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.045342 in-dbt-core-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-06-01 18:21:06.045342 in-dbt-core-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.013342 in-dbt-core-1.5.0/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.013342 in-dbt-core-1.5.0/dbt/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.013342 in-dbt-core-1.5.0/dbt/adapters/base/
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/adapters/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/adapters/base/column.py
--rw-r--r--   0 runner    (1001) docker     (123)    15908 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/adapters/base/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)    55030 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/adapters/base/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/adapters/base/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/adapters/base/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/adapters/base/query_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14913 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/adapters/base/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19958 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/adapters/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/adapters/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/adapters/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/adapters/reference_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.017342 in-dbt-core-1.5.0/dbt/adapters/sql/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/adapters/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/adapters/sql/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/adapters/sql/impl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.017342 in-dbt-core-1.5.0/dbt/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/cli/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12739 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/cli/flags.py
--rw-r--r--   0 runner    (1001) docker     (123)    16615 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/cli/option_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    16863 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/cli/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     8568 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/cli/requires.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/cli/resolvers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.017342 in-dbt-core-1.5.0/dbt/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12364 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/clients/_jinja_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/clients/agate_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/clients/git.py
--rw-r--r--   0 runner    (1001) docker     (123)    21425 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/clients/jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/clients/jinja_static.py
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/clients/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    19144 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/clients/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/clients/yaml_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    19815 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/compilation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.017342 in-dbt-core-1.5.0/dbt/config/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16817 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/config/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    24994 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/config/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     7204 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/config/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)    16144 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/config/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/config/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/config/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.021342 in-dbt-core-1.5.0/dbt/context/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22970 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/context/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/context/configured.py
--rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/context/context_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/context/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/context/exceptions_jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/context/macro_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/context/macros.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/context/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)    58069 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/context/providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/context/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/context/target.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.021342 in-dbt-core-1.5.0/dbt/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/contracts/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    10372 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/contracts/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.025342 in-dbt-core-1.5.0/dbt/contracts/graph/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:20:52.000000 in-dbt-core-1.5.0/dbt/contracts/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47351 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/contracts/graph/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/contracts/graph/manifest_upgrade.py
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/contracts/graph/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    20939 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/contracts/graph/model_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    45470 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/contracts/graph/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/contracts/graph/searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    20236 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/contracts/graph/unparsed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/contracts/graph/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/contracts/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/contracts/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)    13381 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/contracts/results.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/contracts/selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/contracts/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/contracts/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/contracts/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/dataclass_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/deprecations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.025342 in-dbt-core-1.5.0/dbt/deps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/deps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/deps/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/deps/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/deps/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/deps/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/deps/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/deps/tarball.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.005341 in-dbt-core-1.5.0/dbt/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.025342 in-dbt-core-1.5.0/dbt/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.025342 in-dbt-core-1.5.0/dbt/docs/source/_ext/
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/docs/source/_ext/dbt_click.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.025342 in-dbt-core-1.5.0/dbt/events/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/events/adapter_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/events/base_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/events/contextvars.py
--rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/events/eventmgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/events/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     9522 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/events/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/events/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    59505 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/events/types.py
--rw-r--r--   0 runner    (1001) docker     (123)   102151 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/events/types_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    74918 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/flags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.025342 in-dbt-core-1.5.0/dbt/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/graph/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/graph/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    13206 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/graph/selector.py
--rw-r--r--   0 runner    (1001) docker     (123)    27989 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/graph/selector_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/graph/selector_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/helper_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.029342 in-dbt-core-1.5.0/dbt/include/
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.029342 in-dbt-core-1.5.0/dbt/include/global_project/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.029342 in-dbt-core-1.5.0/dbt/include/global_project/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/docs/overview.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.009342 in-dbt-core-1.5.0/dbt/include/global_project/macros/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.029342 in-dbt-core-1.5.0/dbt/include/global_project/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/adapters/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/adapters/columns.sql
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/adapters/freshness.sql
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/adapters/indexes.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/adapters/metadata.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/adapters/persist_docs.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/adapters/relation.sql
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/adapters/schema.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/adapters/timestamps.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.029342 in-dbt-core-1.5.0/dbt/include/global_project/macros/etc/
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/etc/datetime.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/etc/statement.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.029342 in-dbt-core-1.5.0/dbt/include/global_project/macros/generic_test_sql/
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/generic_test_sql/not_null.sql
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/generic_test_sql/relationships.sql
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/generic_test_sql/unique.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.033342 in-dbt-core-1.5.0/dbt/include/global_project/macros/get_custom_name/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.033342 in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/configs.sql
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/hooks.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.009342 in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.033342 in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/models/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/models/incremental/is_incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/models/incremental/merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.033342 in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/models/table/
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/models/table/columns_spec_ddl.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/models/table/create_table_as.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/models/table/table.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.033342 in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/models/view/
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/models/view/create_or_replace_view.sql
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/models/view/create_view_as.sql
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/models/view/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/models/view/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.033342 in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/seeds/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/seeds/seed.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.033342 in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/snapshots/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/snapshots/strategies.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.033342 in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/tests/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/tests/test.sql
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/tests/where_subquery.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.033342 in-dbt-core-1.5.0/dbt/include/global_project/macros/python_model/
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/python_model/python.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.037342 in-dbt-core-1.5.0/dbt/include/global_project/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/utils/cast_bool_to_text.sql
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/utils/concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/utils/data_types.sql
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/utils/date_trunc.sql
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/utils/except.sql
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/utils/hash.sql
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/utils/intersect.sql
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/utils/last_day.sql
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/utils/length.sql
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/utils/literal.sql
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/utils/position.sql
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/utils/replace.sql
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/utils/right.sql
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/macros/utils/split_part.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.009342 in-dbt-core-1.5.0/dbt/include/global_project/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.037342 in-dbt-core-1.5.0/dbt/include/global_project/tests/generic/
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/global_project/tests/generic/builtin.sql
--rw-r--r--   0 runner    (1001) docker     (123)  1497701 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.037342 in-dbt-core-1.5.0/dbt/include/starter_project/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/starter_project/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/starter_project/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/starter_project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.037342 in-dbt-core-1.5.0/dbt/include/starter_project/analyses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/starter_project/analyses/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/starter_project/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.037342 in-dbt-core-1.5.0/dbt/include/starter_project/macros/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/starter_project/macros/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.009342 in-dbt-core-1.5.0/dbt/include/starter_project/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.037342 in-dbt-core-1.5.0/dbt/include/starter_project/models/example/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/starter_project/models/example/my_first_dbt_model.sql
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/starter_project/models/example/my_second_dbt_model.sql
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/starter_project/models/example/schema.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.037342 in-dbt-core-1.5.0/dbt/include/starter_project/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/starter_project/seeds/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.037342 in-dbt-core-1.5.0/dbt/include/starter_project/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/starter_project/snapshots/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.037342 in-dbt-core-1.5.0/dbt/include/starter_project/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/include/starter_project/tests/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/internal_deprecations.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/links.py
--rw-r--r--   0 runner    (1001) docker     (123)    19932 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/node_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.041342 in-dbt-core-1.5.0/dbt/parser/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/parser/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    16910 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/parser/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/parser/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/parser/generic_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16770 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/parser/generic_test_builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/parser/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/parser/macros.py
--rw-r--r--   0 runner    (1001) docker     (123)    62438 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/parser/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)    25716 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/parser/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    51437 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/parser/partial.py
--rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/parser/read_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/parser/schema_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)    59386 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/parser/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/parser/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/parser/seeds.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/parser/singular_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/parser/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)    14106 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/parser/sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/parser/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/selected_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    13885 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/semver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.045342 in-dbt-core-1.5.0/dbt/task/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16571 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/task/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/task/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/task/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/task/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)    14097 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/task/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/task/deps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/task/freshness.py
--rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/task/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)    13795 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/task/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/task/list.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/task/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/task/printer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17788 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/task/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/task/run_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)    21143 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/task/runnable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/task/seed.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/task/serve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/task/show.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/task/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/task/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     7043 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/task/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.045342 in-dbt-core-1.5.0/dbt/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.045342 in-dbt-core-1.5.0/dbt/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18424 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/tests/fixtures/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    18179 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    14471 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/tracking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    20505 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7395 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/dbt/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:21:06.045342 in-dbt-core-1.5.0/in_dbt_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-06-01 18:21:05.000000 in-dbt-core-1.5.0/in_dbt_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-06-01 18:21:05.000000 in-dbt-core-1.5.0/in_dbt_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 18:21:05.000000 in-dbt-core-1.5.0/in_dbt_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-01 18:21:05.000000 in-dbt-core-1.5.0/in_dbt_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 18:21:05.000000 in-dbt-core-1.5.0/in_dbt_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-01 18:21:05.000000 in-dbt-core-1.5.0/in_dbt_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-01 18:21:05.000000 in-dbt-core-1.5.0/in_dbt_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 18:21:06.045342 in-dbt-core-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-06-01 18:20:53.000000 in-dbt-core-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.931499 in-dbt-core-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-06-07 11:50:36.931499 in-dbt-core-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.899499 in-dbt-core-1.5.1/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.899499 in-dbt-core-1.5.1/dbt/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.899499 in-dbt-core-1.5.1/dbt/adapters/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/adapters/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/adapters/base/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15908 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/adapters/base/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55030 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/adapters/base/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/adapters/base/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/adapters/base/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/adapters/base/query_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14913 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/adapters/base/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19958 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/adapters/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/adapters/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/adapters/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/adapters/reference_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.903499 in-dbt-core-1.5.1/dbt/adapters/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/adapters/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/adapters/sql/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/adapters/sql/impl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.903499 in-dbt-core-1.5.1/dbt/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/cli/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12739 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/cli/flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16615 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/cli/option_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16863 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/cli/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8568 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/cli/requires.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/cli/resolvers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.903499 in-dbt-core-1.5.1/dbt/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12364 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/clients/_jinja_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/clients/agate_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/clients/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21425 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/clients/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/clients/jinja_static.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/clients/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19144 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/clients/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/clients/yaml_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19815 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/compilation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.903499 in-dbt-core-1.5.1/dbt/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16817 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/config/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24994 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/config/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7204 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/config/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16144 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/config/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/config/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/config/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.907499 in-dbt-core-1.5.1/dbt/context/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22970 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/context/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/context/configured.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/context/context_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/context/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/context/exceptions_jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/context/macro_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/context/macros.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/context/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58069 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/context/providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/context/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/context/target.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.907499 in-dbt-core-1.5.1/dbt/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/contracts/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10372 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/contracts/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.911499 in-dbt-core-1.5.1/dbt/contracts/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/contracts/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47351 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/contracts/graph/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/contracts/graph/manifest_upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/contracts/graph/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20939 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/contracts/graph/model_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45470 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/contracts/graph/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/contracts/graph/searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20236 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/contracts/graph/unparsed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/contracts/graph/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/contracts/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/contracts/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13381 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/contracts/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/contracts/selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/contracts/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/contracts/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/contracts/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/dataclass_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/deprecations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.911499 in-dbt-core-1.5.1/dbt/deps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/deps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/deps/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/deps/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/deps/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/deps/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/deps/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/deps/tarball.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.891499 in-dbt-core-1.5.1/dbt/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.911499 in-dbt-core-1.5.1/dbt/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.911499 in-dbt-core-1.5.1/dbt/docs/source/_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/docs/source/_ext/dbt_click.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.911499 in-dbt-core-1.5.1/dbt/events/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/events/adapter_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/events/base_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/events/contextvars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/events/eventmgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/events/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9522 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/events/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/events/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59505 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/events/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)   104535 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/events/types_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74918 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/flags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.911499 in-dbt-core-1.5.1/dbt/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/graph/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/graph/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13206 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/graph/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27989 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/graph/selector_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/graph/selector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/helper_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.911499 in-dbt-core-1.5.1/dbt/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.915499 in-dbt-core-1.5.1/dbt/include/global_project/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.915499 in-dbt-core-1.5.1/dbt/include/global_project/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/docs/overview.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.895499 in-dbt-core-1.5.1/dbt/include/global_project/macros/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.915499 in-dbt-core-1.5.1/dbt/include/global_project/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/adapters/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/adapters/columns.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/adapters/freshness.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/adapters/indexes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/adapters/metadata.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/adapters/persist_docs.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/adapters/relation.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/adapters/schema.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/adapters/timestamps.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.915499 in-dbt-core-1.5.1/dbt/include/global_project/macros/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/etc/datetime.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/etc/statement.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.915499 in-dbt-core-1.5.1/dbt/include/global_project/macros/generic_test_sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/generic_test_sql/not_null.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/generic_test_sql/relationships.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/generic_test_sql/unique.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.915499 in-dbt-core-1.5.1/dbt/include/global_project/macros/get_custom_name/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.915499 in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/configs.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/hooks.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.895499 in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.919499 in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/models/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/models/incremental/is_incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/models/incremental/merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.919499 in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/models/table/
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/models/table/columns_spec_ddl.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/models/table/create_table_as.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/models/table/table.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.919499 in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/models/view/
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/models/view/create_or_replace_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/models/view/create_view_as.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/models/view/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/models/view/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.919499 in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/seeds/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/seeds/seed.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.919499 in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/snapshots/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/snapshots/strategies.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.919499 in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/tests/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/tests/test.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/tests/where_subquery.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.919499 in-dbt-core-1.5.1/dbt/include/global_project/macros/python_model/
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/python_model/python.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.923499 in-dbt-core-1.5.1/dbt/include/global_project/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/utils/concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/utils/data_types.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/utils/date_trunc.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/utils/except.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/utils/hash.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/utils/intersect.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/utils/last_day.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/utils/length.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/utils/literal.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/utils/position.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/utils/replace.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/utils/right.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/macros/utils/split_part.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.895499 in-dbt-core-1.5.1/dbt/include/global_project/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.923499 in-dbt-core-1.5.1/dbt/include/global_project/tests/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/global_project/tests/generic/builtin.sql
+-rw-r--r--   0 runner    (1001) docker     (123)  1497701 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.923499 in-dbt-core-1.5.1/dbt/include/starter_project/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/starter_project/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/starter_project/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/starter_project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.923499 in-dbt-core-1.5.1/dbt/include/starter_project/analyses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/starter_project/analyses/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/starter_project/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.923499 in-dbt-core-1.5.1/dbt/include/starter_project/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/starter_project/macros/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.895499 in-dbt-core-1.5.1/dbt/include/starter_project/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.923499 in-dbt-core-1.5.1/dbt/include/starter_project/models/example/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/starter_project/models/example/my_first_dbt_model.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/starter_project/models/example/my_second_dbt_model.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/starter_project/models/example/schema.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.923499 in-dbt-core-1.5.1/dbt/include/starter_project/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/starter_project/seeds/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.923499 in-dbt-core-1.5.1/dbt/include/starter_project/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/starter_project/snapshots/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.923499 in-dbt-core-1.5.1/dbt/include/starter_project/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/include/starter_project/tests/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/internal_deprecations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19932 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/node_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.927499 in-dbt-core-1.5.1/dbt/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/parser/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16910 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/parser/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/parser/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/parser/generic_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16770 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/parser/generic_test_builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/parser/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/parser/macros.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62438 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/parser/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25716 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/parser/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51437 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/parser/partial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/parser/read_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/parser/schema_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59386 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/parser/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/parser/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/parser/seeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/parser/singular_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/parser/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14106 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/parser/sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/parser/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/selected_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13885 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/semver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.931499 in-dbt-core-1.5.1/dbt/task/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16571 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/task/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/task/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/task/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/task/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14097 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/task/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/task/deps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/task/freshness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/task/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13795 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/task/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/task/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/task/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/task/printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17788 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/task/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/task/run_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21143 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/task/runnable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/task/seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/task/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/task/show.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/task/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/task/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7043 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/task/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.931499 in-dbt-core-1.5.1/dbt/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.931499 in-dbt-core-1.5.1/dbt/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18424 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/tests/fixtures/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18179 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14471 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20505 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7395 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/dbt/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:50:36.931499 in-dbt-core-1.5.1/in_dbt_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-06-07 11:50:36.000000 in-dbt-core-1.5.1/in_dbt_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-06-07 11:50:36.000000 in-dbt-core-1.5.1/in_dbt_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 11:50:36.000000 in-dbt-core-1.5.1/in_dbt_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-07 11:50:36.000000 in-dbt-core-1.5.1/in_dbt_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 11:50:36.000000 in-dbt-core-1.5.1/in_dbt_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-07 11:50:36.000000 in-dbt-core-1.5.1/in_dbt_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-07 11:50:36.000000 in-dbt-core-1.5.1/in_dbt_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 11:50:36.931499 in-dbt-core-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-06-07 11:50:24.000000 in-dbt-core-1.5.1/setup.py
```

### Comparing `in-dbt-core-1.5.0/PKG-INFO` & `in-dbt-core-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: in-dbt-core
-Version: 1.5.0
+Version: 1.5.1
 Summary: Release for LinkedIn's changes to dbt-core.
 Home-page: https://github.com/linkedin/in-dbt-core
 Author: LinkedIn DBT Team
 Author-email: dbt-eng@linkedin.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: in-dbt-core Version: 1.5.0 Summary: Release for
+Metadata-Version: 2.1 Name: in-dbt-core Version: 1.5.1 Summary: Release for
 LinkedIn's changes to dbt-core. Home-page: https://github.com/linkedin/in-dbt-
 core Author: LinkedIn DBT Team Author-email: dbt-eng@linkedin.com Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `in-dbt-core-1.5.0/README.md` & `in-dbt-core-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/adapters/base/__init__.py` & `in-dbt-core-1.5.1/dbt/adapters/base/__init__.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/adapters/base/column.py` & `in-dbt-core-1.5.1/dbt/adapters/base/column.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/adapters/base/connections.py` & `in-dbt-core-1.5.1/dbt/adapters/base/connections.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/adapters/base/impl.py` & `in-dbt-core-1.5.1/dbt/adapters/base/impl.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/adapters/base/meta.py` & `in-dbt-core-1.5.1/dbt/adapters/base/meta.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/adapters/base/plugin.py` & `in-dbt-core-1.5.1/dbt/adapters/base/plugin.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/adapters/base/query_headers.py` & `in-dbt-core-1.5.1/dbt/adapters/base/query_headers.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/adapters/base/relation.py` & `in-dbt-core-1.5.1/dbt/adapters/base/relation.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/adapters/cache.py` & `in-dbt-core-1.5.1/dbt/adapters/cache.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/adapters/factory.py` & `in-dbt-core-1.5.1/dbt/adapters/factory.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/adapters/protocol.py` & `in-dbt-core-1.5.1/dbt/adapters/protocol.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/adapters/reference_keys.py` & `in-dbt-core-1.5.1/dbt/adapters/reference_keys.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/adapters/sql/connections.py` & `in-dbt-core-1.5.1/dbt/adapters/sql/connections.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/adapters/sql/impl.py` & `in-dbt-core-1.5.1/dbt/adapters/sql/impl.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/cli/exceptions.py` & `in-dbt-core-1.5.1/dbt/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/cli/flags.py` & `in-dbt-core-1.5.1/dbt/cli/flags.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/cli/main.py` & `in-dbt-core-1.5.1/dbt/cli/main.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/cli/option_types.py` & `in-dbt-core-1.5.1/dbt/cli/option_types.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/cli/options.py` & `in-dbt-core-1.5.1/dbt/cli/options.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/cli/params.py` & `in-dbt-core-1.5.1/dbt/cli/params.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/cli/requires.py` & `in-dbt-core-1.5.1/dbt/cli/requires.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/cli/resolvers.py` & `in-dbt-core-1.5.1/dbt/cli/resolvers.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/clients/_jinja_blocks.py` & `in-dbt-core-1.5.1/dbt/clients/_jinja_blocks.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/clients/agate_helper.py` & `in-dbt-core-1.5.1/dbt/clients/agate_helper.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/clients/git.py` & `in-dbt-core-1.5.1/dbt/clients/git.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/clients/jinja.py` & `in-dbt-core-1.5.1/dbt/clients/jinja.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/clients/jinja_static.py` & `in-dbt-core-1.5.1/dbt/clients/jinja_static.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/clients/registry.py` & `in-dbt-core-1.5.1/dbt/clients/registry.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/clients/system.py` & `in-dbt-core-1.5.1/dbt/clients/system.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/clients/yaml_helper.py` & `in-dbt-core-1.5.1/dbt/clients/yaml_helper.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/compilation.py` & `in-dbt-core-1.5.1/dbt/compilation.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/config/profile.py` & `in-dbt-core-1.5.1/dbt/config/profile.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/config/project.py` & `in-dbt-core-1.5.1/dbt/config/project.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/config/renderer.py` & `in-dbt-core-1.5.1/dbt/config/renderer.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/config/runtime.py` & `in-dbt-core-1.5.1/dbt/config/runtime.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/config/selectors.py` & `in-dbt-core-1.5.1/dbt/config/selectors.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/config/utils.py` & `in-dbt-core-1.5.1/dbt/config/utils.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/context/base.py` & `in-dbt-core-1.5.1/dbt/context/base.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/context/configured.py` & `in-dbt-core-1.5.1/dbt/context/configured.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/context/context_config.py` & `in-dbt-core-1.5.1/dbt/context/context_config.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/context/docs.py` & `in-dbt-core-1.5.1/dbt/context/docs.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/context/exceptions_jinja.py` & `in-dbt-core-1.5.1/dbt/context/exceptions_jinja.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/context/macro_resolver.py` & `in-dbt-core-1.5.1/dbt/context/macro_resolver.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/context/macros.py` & `in-dbt-core-1.5.1/dbt/context/macros.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/context/manifest.py` & `in-dbt-core-1.5.1/dbt/context/manifest.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/context/providers.py` & `in-dbt-core-1.5.1/dbt/context/providers.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/context/secret.py` & `in-dbt-core-1.5.1/dbt/context/secret.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/context/target.py` & `in-dbt-core-1.5.1/dbt/context/target.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/contracts/connection.py` & `in-dbt-core-1.5.1/dbt/contracts/connection.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/contracts/files.py` & `in-dbt-core-1.5.1/dbt/contracts/files.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/contracts/graph/manifest.py` & `in-dbt-core-1.5.1/dbt/contracts/graph/manifest.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/contracts/graph/manifest_upgrade.py` & `in-dbt-core-1.5.1/dbt/contracts/graph/manifest_upgrade.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/contracts/graph/metrics.py` & `in-dbt-core-1.5.1/dbt/contracts/graph/metrics.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/contracts/graph/model_config.py` & `in-dbt-core-1.5.1/dbt/contracts/graph/model_config.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/contracts/graph/nodes.py` & `in-dbt-core-1.5.1/dbt/contracts/graph/nodes.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/contracts/graph/unparsed.py` & `in-dbt-core-1.5.1/dbt/contracts/graph/unparsed.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/contracts/graph/utils.py` & `in-dbt-core-1.5.1/dbt/contracts/graph/utils.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/contracts/project.py` & `in-dbt-core-1.5.1/dbt/contracts/project.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/contracts/relation.py` & `in-dbt-core-1.5.1/dbt/contracts/relation.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/contracts/results.py` & `in-dbt-core-1.5.1/dbt/contracts/results.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/contracts/selection.py` & `in-dbt-core-1.5.1/dbt/contracts/selection.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/contracts/sql.py` & `in-dbt-core-1.5.1/dbt/contracts/sql.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/contracts/state.py` & `in-dbt-core-1.5.1/dbt/contracts/state.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/contracts/util.py` & `in-dbt-core-1.5.1/dbt/contracts/util.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/dataclass_schema.py` & `in-dbt-core-1.5.1/dbt/dataclass_schema.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/deprecations.py` & `in-dbt-core-1.5.1/dbt/deprecations.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/deps/base.py` & `in-dbt-core-1.5.1/dbt/deps/base.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/deps/git.py` & `in-dbt-core-1.5.1/dbt/deps/git.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/deps/local.py` & `in-dbt-core-1.5.1/dbt/deps/local.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/deps/registry.py` & `in-dbt-core-1.5.1/dbt/deps/registry.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/deps/resolver.py` & `in-dbt-core-1.5.1/dbt/deps/resolver.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/deps/tarball.py` & `in-dbt-core-1.5.1/dbt/deps/tarball.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/docs/source/_ext/dbt_click.py` & `in-dbt-core-1.5.1/dbt/docs/source/_ext/dbt_click.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/docs/source/conf.py` & `in-dbt-core-1.5.1/dbt/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/events/adapter_endpoint.py` & `in-dbt-core-1.5.1/dbt/events/adapter_endpoint.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/events/base_types.py` & `in-dbt-core-1.5.1/dbt/events/base_types.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/events/contextvars.py` & `in-dbt-core-1.5.1/dbt/events/contextvars.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/events/eventmgr.py` & `in-dbt-core-1.5.1/dbt/events/eventmgr.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/events/format.py` & `in-dbt-core-1.5.1/dbt/events/format.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/events/functions.py` & `in-dbt-core-1.5.1/dbt/events/functions.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/events/helpers.py` & `in-dbt-core-1.5.1/dbt/events/helpers.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/events/types.py` & `in-dbt-core-1.5.1/dbt/events/types.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/events/types_pb2.py` & `in-dbt-core-1.5.1/dbt/events/types_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0btypes.proto\x12\x0bproto_types\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1cgoogle/protobuf/struct.proto\"\x91\x02\n\tEventInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x0b\n\x03msg\x18\x03 \x01(\t\x12\r\n\x05level\x18\x04 \x01(\t\x12\x15\n\rinvocation_id\x18\x05 \x01(\t\x12\x0b\n\x03pid\x18\x06 \x01(\x05\x12\x0e\n\x06thread\x18\x07 \x01(\t\x12&\n\x02ts\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x05\x65xtra\x18\t \x03(\x0b\x32!.proto_types.EventInfo.ExtraEntry\x12\x10\n\x08\x63\x61tegory\x18\n \x01(\t\x1a,\n\nExtraEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x7f\n\rTimingInfoMsg\x12\x0c\n\x04name\x18\x01 \x01(\t\x12.\n\nstarted_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0c\x63ompleted_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"V\n\x0cNodeRelation\x12\x10\n\x08\x64\x61tabase\x18\n \x01(\t\x12\x0e\n\x06schema\x18\x0b \x01(\t\x12\r\n\x05\x61lias\x18\x0c \x01(\t\x12\x15\n\rrelation_name\x18\r \x01(\t\"\x91\x02\n\x08NodeInfo\x12\x11\n\tnode_path\x18\x01 \x01(\t\x12\x11\n\tnode_name\x18\x02 \x01(\t\x12\x11\n\tunique_id\x18\x03 \x01(\t\x12\x15\n\rresource_type\x18\x04 \x01(\t\x12\x14\n\x0cmaterialized\x18\x05 \x01(\t\x12\x13\n\x0bnode_status\x18\x06 \x01(\t\x12\x17\n\x0fnode_started_at\x18\x07 \x01(\t\x12\x18\n\x10node_finished_at\x18\x08 \x01(\t\x12%\n\x04meta\x18\t \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x30\n\rnode_relation\x18\n \x01(\x0b\x32\x19.proto_types.NodeRelation\"\xd1\x01\n\x0cRunResultMsg\x12\x0e\n\x06status\x18\x01 \x01(\t\x12\x0f\n\x07message\x18\x02 \x01(\t\x12/\n\x0btiming_info\x18\x03 \x03(\x0b\x32\x1a.proto_types.TimingInfoMsg\x12\x0e\n\x06thread\x18\x04 \x01(\t\x12\x16\n\x0e\x65xecution_time\x18\x05 \x01(\x02\x12\x31\n\x10\x61\x64\x61pter_response\x18\x06 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x14\n\x0cnum_failures\x18\x07 \x01(\x05\"G\n\x0fReferenceKeyMsg\x12\x10\n\x08\x64\x61tabase\x18\x01 \x01(\t\x12\x0e\n\x06schema\x18\x02 \x01(\t\x12\x12\n\nidentifier\x18\x03 \x01(\t\"6\n\x0eGenericMessage\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\"9\n\x11MainReportVersion\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x13\n\x0blog_version\x18\x02 \x01(\x05\"j\n\x14MainReportVersionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.MainReportVersion\"r\n\x0eMainReportArgs\x12\x33\n\x04\x61rgs\x18\x01 \x03(\x0b\x32%.proto_types.MainReportArgs.ArgsEntry\x1a+\n\tArgsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"d\n\x11MainReportArgsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.MainReportArgs\"+\n\x15MainTrackingUserState\x12\x12\n\nuser_state\x18\x01 \x01(\t\"r\n\x18MainTrackingUserStateMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.MainTrackingUserState\"5\n\x0fMergedFromState\x12\x12\n\nnum_merged\x18\x01 \x01(\x05\x12\x0e\n\x06sample\x18\x02 \x03(\t\"f\n\x12MergedFromStateMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.MergedFromState\"A\n\x14MissingProfileTarget\x12\x14\n\x0cprofile_name\x18\x01 \x01(\t\x12\x13\n\x0btarget_name\x18\x02 \x01(\t\"p\n\x17MissingProfileTargetMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.MissingProfileTarget\"(\n\x11InvalidOptionYAML\x12\x13\n\x0boption_name\x18\x01 \x01(\t\"j\n\x14InvalidOptionYAMLMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.InvalidOptionYAML\"!\n\x12LogDbtProjectError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"l\n\x15LogDbtProjectErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogDbtProjectError\"3\n\x12LogDbtProfileError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\x12\x10\n\x08profiles\x18\x02 \x03(\t\"l\n\x15LogDbtProfileErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogDbtProfileError\"!\n\x12StarterProjectPath\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"l\n\x15StarterProjectPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.StarterProjectPath\"$\n\x15\x43onfigFolderDirectory\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"r\n\x18\x43onfigFolderDirectoryMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.ConfigFolderDirectory\"\'\n\x14NoSampleProfileFound\x12\x0f\n\x07\x61\x64\x61pter\x18\x01 \x01(\t\"p\n\x17NoSampleProfileFoundMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.NoSampleProfileFound\"6\n\x18ProfileWrittenWithSample\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"x\n\x1bProfileWrittenWithSampleMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.ProfileWrittenWithSample\"B\n$ProfileWrittenWithTargetTemplateYAML\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"\x90\x01\n\'ProfileWrittenWithTargetTemplateYAMLMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12?\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x31.proto_types.ProfileWrittenWithTargetTemplateYAML\"C\n%ProfileWrittenWithProjectTemplateYAML\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"\x92\x01\n(ProfileWrittenWithProjectTemplateYAMLMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12@\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x32.proto_types.ProfileWrittenWithProjectTemplateYAML\"\x12\n\x10SettingUpProfile\"h\n\x13SettingUpProfileMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.SettingUpProfile\"\x1c\n\x1aInvalidProfileTemplateYAML\"|\n\x1dInvalidProfileTemplateYAMLMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.InvalidProfileTemplateYAML\"(\n\x18ProjectNameAlreadyExists\x12\x0c\n\x04name\x18\x01 \x01(\t\"x\n\x1bProjectNameAlreadyExistsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.ProjectNameAlreadyExists\"K\n\x0eProjectCreated\x12\x14\n\x0cproject_name\x18\x01 \x01(\t\x12\x10\n\x08\x64ocs_url\x18\x02 \x01(\t\x12\x11\n\tslack_url\x18\x03 \x01(\t\"d\n\x11ProjectCreatedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.ProjectCreated\"@\n\x1aPackageRedirectDeprecation\x12\x10\n\x08old_name\x18\x01 \x01(\t\x12\x10\n\x08new_name\x18\x02 \x01(\t\"|\n\x1dPackageRedirectDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.PackageRedirectDeprecation\"\x1f\n\x1dPackageInstallPathDeprecation\"\x82\x01\n PackageInstallPathDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.PackageInstallPathDeprecation\"H\n\x1b\x43onfigSourcePathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\x12\x10\n\x08\x65xp_path\x18\x02 \x01(\t\"~\n\x1e\x43onfigSourcePathDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.ConfigSourcePathDeprecation\"F\n\x19\x43onfigDataPathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\x12\x10\n\x08\x65xp_path\x18\x02 \x01(\t\"z\n\x1c\x43onfigDataPathDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.ConfigDataPathDeprecation\"?\n\x19\x41\x64\x61pterDeprecationWarning\x12\x10\n\x08old_name\x18\x01 \x01(\t\x12\x10\n\x08new_name\x18\x02 \x01(\t\"z\n\x1c\x41\x64\x61pterDeprecationWarningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.AdapterDeprecationWarning\".\n\x17MetricAttributesRenamed\x12\x13\n\x0bmetric_name\x18\x01 \x01(\t\"v\n\x1aMetricAttributesRenamedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.MetricAttributesRenamed\"+\n\x17\x45xposureNameDeprecation\x12\x10\n\x08\x65xposure\x18\x01 \x01(\t\"v\n\x1a\x45xposureNameDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.ExposureNameDeprecation\"^\n\x13InternalDeprecation\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x18\n\x10suggested_action\x18\x03 \x01(\t\x12\x0f\n\x07version\x18\x04 \x01(\t\"n\n\x16InternalDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.InternalDeprecation\"@\n\x1a\x45nvironmentVariableRenamed\x12\x10\n\x08old_name\x18\x01 \x01(\t\x12\x10\n\x08new_name\x18\x02 \x01(\t\"|\n\x1d\x45nvironmentVariableRenamedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.EnvironmentVariableRenamed\"3\n\x18\x43onfigLogPathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\"x\n\x1b\x43onfigLogPathDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.ConfigLogPathDeprecation\"6\n\x1b\x43onfigTargetPathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\"~\n\x1e\x43onfigTargetPathDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.ConfigTargetPathDeprecation\"\x87\x01\n\x11\x41\x64\x61pterEventDebug\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61se_msg\x18\x03 \x01(\t\x12(\n\x04\x61rgs\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.ListValue\"j\n\x14\x41\x64\x61pterEventDebugMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.AdapterEventDebug\"\x86\x01\n\x10\x41\x64\x61pterEventInfo\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61se_msg\x18\x03 \x01(\t\x12(\n\x04\x61rgs\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.ListValue\"h\n\x13\x41\x64\x61pterEventInfoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.AdapterEventInfo\"\x89\x01\n\x13\x41\x64\x61pterEventWarning\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61se_msg\x18\x03 \x01(\t\x12(\n\x04\x61rgs\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.ListValue\"n\n\x16\x41\x64\x61pterEventWarningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.AdapterEventWarning\"\x99\x01\n\x11\x41\x64\x61pterEventError\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61se_msg\x18\x03 \x01(\t\x12(\n\x04\x61rgs\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12\x10\n\x08\x65xc_info\x18\x05 \x01(\t\"j\n\x14\x41\x64\x61pterEventErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.AdapterEventError\"_\n\rNewConnection\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_type\x18\x02 \x01(\t\x12\x11\n\tconn_name\x18\x03 \x01(\t\"b\n\x10NewConnectionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.NewConnection\"=\n\x10\x43onnectionReused\x12\x11\n\tconn_name\x18\x01 \x01(\t\x12\x16\n\x0eorig_conn_name\x18\x02 \x01(\t\"h\n\x13\x43onnectionReusedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.ConnectionReused\"0\n\x1b\x43onnectionLeftOpenInCleanup\x12\x11\n\tconn_name\x18\x01 \x01(\t\"~\n\x1e\x43onnectionLeftOpenInCleanupMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.ConnectionLeftOpenInCleanup\".\n\x19\x43onnectionClosedInCleanup\x12\x11\n\tconn_name\x18\x01 \x01(\t\"z\n\x1c\x43onnectionClosedInCleanupMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.ConnectionClosedInCleanup\"_\n\x0eRollbackFailed\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"d\n\x11RollbackFailedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.RollbackFailed\"O\n\x10\x43onnectionClosed\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\"h\n\x13\x43onnectionClosedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.ConnectionClosed\"Q\n\x12\x43onnectionLeftOpen\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\"l\n\x15\x43onnectionLeftOpenMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.ConnectionLeftOpen\"G\n\x08Rollback\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\"X\n\x0bRollbackMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12#\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x15.proto_types.Rollback\"@\n\tCacheMiss\x12\x11\n\tconn_name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tabase\x18\x02 \x01(\t\x12\x0e\n\x06schema\x18\x03 \x01(\t\"Z\n\x0c\x43\x61\x63heMissMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12$\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.proto_types.CacheMiss\"b\n\rListRelations\x12\x10\n\x08\x64\x61tabase\x18\x01 \x01(\t\x12\x0e\n\x06schema\x18\x02 \x01(\t\x12/\n\trelations\x18\x03 \x03(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"b\n\x10ListRelationsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.ListRelations\"`\n\x0e\x43onnectionUsed\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_type\x18\x02 \x01(\t\x12\x11\n\tconn_name\x18\x03 \x01(\t\"d\n\x11\x43onnectionUsedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.ConnectionUsed\"T\n\x08SQLQuery\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\x12\x0b\n\x03sql\x18\x03 \x01(\t\"X\n\x0bSQLQueryMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12#\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x15.proto_types.SQLQuery\"[\n\x0eSQLQueryStatus\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x0f\n\x07\x65lapsed\x18\x03 \x01(\x02\"d\n\x11SQLQueryStatusMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.SQLQueryStatus\"H\n\tSQLCommit\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\"Z\n\x0cSQLCommitMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12$\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.proto_types.SQLCommit\"a\n\rColTypeChange\x12\x11\n\torig_type\x18\x01 \x01(\t\x12\x10\n\x08new_type\x18\x02 \x01(\t\x12+\n\x05table\x18\x03 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"b\n\x10\x43olTypeChangeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.ColTypeChange\"@\n\x0eSchemaCreation\x12.\n\x08relation\x18\x01 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"d\n\x11SchemaCreationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.SchemaCreation\"<\n\nSchemaDrop\x12.\n\x08relation\x18\x01 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"\\\n\rSchemaDropMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.SchemaDrop\"\xde\x01\n\x0b\x43\x61\x63heAction\x12\x0e\n\x06\x61\x63tion\x18\x01 \x01(\t\x12-\n\x07ref_key\x18\x02 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\x12/\n\tref_key_2\x18\x03 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\x12/\n\tref_key_3\x18\x04 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\x12.\n\x08ref_list\x18\x05 \x03(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"^\n\x0e\x43\x61\x63heActionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.CacheAction\"\x98\x01\n\x0e\x43\x61\x63heDumpGraph\x12\x33\n\x04\x64ump\x18\x01 \x03(\x0b\x32%.proto_types.CacheDumpGraph.DumpEntry\x12\x14\n\x0c\x62\x65\x66ore_after\x18\x02 \x01(\t\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\x1a+\n\tDumpEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"d\n\x11\x43\x61\x63heDumpGraphMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.CacheDumpGraph\"!\n\x12\x41\x64\x61pterImportError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"l\n\x15\x41\x64\x61pterImportErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.AdapterImportError\"#\n\x0fPluginLoadError\x12\x10\n\x08\x65xc_info\x18\x01 \x01(\t\"f\n\x12PluginLoadErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.PluginLoadError\"Z\n\x14NewConnectionOpening\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x18\n\x10\x63onnection_state\x18\x02 \x01(\t\"p\n\x17NewConnectionOpeningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.NewConnectionOpening\"8\n\rCodeExecution\x12\x11\n\tconn_name\x18\x01 \x01(\t\x12\x14\n\x0c\x63ode_content\x18\x02 \x01(\t\"b\n\x10\x43odeExecutionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.CodeExecution\"6\n\x13\x43odeExecutionStatus\x12\x0e\n\x06status\x18\x01 \x01(\t\x12\x0f\n\x07\x65lapsed\x18\x02 \x01(\x02\"n\n\x16\x43odeExecutionStatusMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.CodeExecutionStatus\"%\n\x16\x43\x61talogGenerationError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"t\n\x19\x43\x61talogGenerationErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.CatalogGenerationError\"-\n\x13WriteCatalogFailure\x12\x16\n\x0enum_exceptions\x18\x01 \x01(\x05\"n\n\x16WriteCatalogFailureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.WriteCatalogFailure\"\x1e\n\x0e\x43\x61talogWritten\x12\x0c\n\x04path\x18\x01 \x01(\t\"d\n\x11\x43\x61talogWrittenMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.CatalogWritten\"\x14\n\x12\x43\x61nnotGenerateDocs\"l\n\x15\x43\x61nnotGenerateDocsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.CannotGenerateDocs\"\x11\n\x0f\x42uildingCatalog\"f\n\x12\x42uildingCatalogMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.BuildingCatalog\"-\n\x18\x44\x61tabaseErrorRunningHook\x12\x11\n\thook_type\x18\x01 \x01(\t\"x\n\x1b\x44\x61tabaseErrorRunningHookMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.DatabaseErrorRunningHook\"4\n\x0cHooksRunning\x12\x11\n\tnum_hooks\x18\x01 \x01(\x05\x12\x11\n\thook_type\x18\x02 \x01(\t\"`\n\x0fHooksRunningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.HooksRunning\"T\n\x14\x46inishedRunningStats\x12\x11\n\tstat_line\x18\x01 \x01(\t\x12\x11\n\texecution\x18\x02 \x01(\t\x12\x16\n\x0e\x65xecution_time\x18\x03 \x01(\x02\"p\n\x17\x46inishedRunningStatsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.FinishedRunningStats\"<\n\x15\x43onstraintNotEnforced\x12\x12\n\nconstraint\x18\x01 \x01(\t\x12\x0f\n\x07\x61\x64\x61pter\x18\x02 \x01(\t\"r\n\x18\x43onstraintNotEnforcedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.ConstraintNotEnforced\"=\n\x16\x43onstraintNotSupported\x12\x12\n\nconstraint\x18\x01 \x01(\t\x12\x0f\n\x07\x61\x64\x61pter\x18\x02 \x01(\t\"t\n\x19\x43onstraintNotSupportedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.ConstraintNotSupported\"7\n\x12InputFileDiffError\x12\x10\n\x08\x63\x61tegory\x18\x01 \x01(\t\x12\x0f\n\x07\x66ile_id\x18\x02 \x01(\t\"l\n\x15InputFileDiffErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.InputFileDiffError\"?\n\x14InvalidValueForField\x12\x12\n\nfield_name\x18\x01 \x01(\t\x12\x13\n\x0b\x66ield_value\x18\x02 \x01(\t\"p\n\x17InvalidValueForFieldMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.InvalidValueForField\"Q\n\x11ValidationWarning\x12\x15\n\rresource_type\x18\x01 \x01(\t\x12\x12\n\nfield_name\x18\x02 \x01(\t\x12\x11\n\tnode_name\x18\x03 \x01(\t\"j\n\x14ValidationWarningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.ValidationWarning\"!\n\x11ParsePerfInfoPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"j\n\x14ParsePerfInfoPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.ParsePerfInfoPath\"$\n\x14GenericTestFileParse\x12\x0c\n\x04path\x18\x01 \x01(\t\"p\n\x17GenericTestFileParseMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.GenericTestFileParse\"\x1e\n\x0eMacroFileParse\x12\x0c\n\x04path\x18\x01 \x01(\t\"d\n\x11MacroFileParseMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.MacroFileParse\"1\n!PartialParsingErrorProcessingFile\x12\x0c\n\x04\x66ile\x18\x01 \x01(\t\"\x8a\x01\n$PartialParsingErrorProcessingFileMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12<\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32..proto_types.PartialParsingErrorProcessingFile\"\x86\x01\n\x13PartialParsingError\x12?\n\x08\x65xc_info\x18\x01 \x03(\x0b\x32-.proto_types.PartialParsingError.ExcInfoEntry\x1a.\n\x0c\x45xcInfoEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"n\n\x16PartialParsingErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.PartialParsingError\"\x1b\n\x19PartialParsingSkipParsing\"z\n\x1cPartialParsingSkipParsingMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.PartialParsingSkipParsing\"&\n\x14UnableToPartialParse\x12\x0e\n\x06reason\x18\x01 \x01(\t\"p\n\x17UnableToPartialParseMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.UnableToPartialParse\"f\n\x12StateCheckVarsHash\x12\x10\n\x08\x63hecksum\x18\x01 \x01(\t\x12\x0c\n\x04vars\x18\x02 \x01(\t\x12\x0f\n\x07profile\x18\x03 \x01(\t\x12\x0e\n\x06target\x18\x04 \x01(\t\x12\x0f\n\x07version\x18\x05 \x01(\t\"l\n\x15StateCheckVarsHashMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.StateCheckVarsHash\"\x1a\n\x18PartialParsingNotEnabled\"x\n\x1bPartialParsingNotEnabledMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.PartialParsingNotEnabled\"C\n\x14ParsedFileLoadFailed\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"p\n\x17ParsedFileLoadFailedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.ParsedFileLoadFailed\"H\n\x15PartialParsingEnabled\x12\x0f\n\x07\x64\x65leted\x18\x01 \x01(\x05\x12\r\n\x05\x61\x64\x64\x65\x64\x18\x02 \x01(\x05\x12\x0f\n\x07\x63hanged\x18\x03 \x01(\x05\"r\n\x18PartialParsingEnabledMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.PartialParsingEnabled\"8\n\x12PartialParsingFile\x12\x0f\n\x07\x66ile_id\x18\x01 \x01(\t\x12\x11\n\toperation\x18\x02 \x01(\t\"l\n\x15PartialParsingFileMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.PartialParsingFile\"\xaf\x01\n\x1fInvalidDisabledTargetInTestNode\x12\x1b\n\x13resource_type_title\x18\x01 \x01(\t\x12\x11\n\tunique_id\x18\x02 \x01(\t\x12\x1a\n\x12original_file_path\x18\x03 \x01(\t\x12\x13\n\x0btarget_kind\x18\x04 \x01(\t\x12\x13\n\x0btarget_name\x18\x05 \x01(\t\x12\x16\n\x0etarget_package\x18\x06 \x01(\t\"\x86\x01\n\"InvalidDisabledTargetInTestNodeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.InvalidDisabledTargetInTestNode\"7\n\x18UnusedResourceConfigPath\x12\x1b\n\x13unused_config_paths\x18\x01 \x03(\t\"x\n\x1bUnusedResourceConfigPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.UnusedResourceConfigPath\"3\n\rSeedIncreased\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"b\n\x10SeedIncreasedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.SeedIncreased\">\n\x18SeedExceedsLimitSamePath\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"x\n\x1bSeedExceedsLimitSamePathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.SeedExceedsLimitSamePath\"D\n\x1eSeedExceedsLimitAndPathChanged\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x84\x01\n!SeedExceedsLimitAndPathChangedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.SeedExceedsLimitAndPathChanged\"\\\n\x1fSeedExceedsLimitChecksumChanged\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x15\n\rchecksum_name\x18\x03 \x01(\t\"\x86\x01\n\"SeedExceedsLimitChecksumChangedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.SeedExceedsLimitChecksumChanged\"%\n\x0cUnusedTables\x12\x15\n\runused_tables\x18\x01 \x03(\t\"`\n\x0fUnusedTablesMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.UnusedTables\"\x87\x01\n\x17WrongResourceSchemaFile\x12\x12\n\npatch_name\x18\x01 \x01(\t\x12\x15\n\rresource_type\x18\x02 \x01(\t\x12\x1c\n\x14plural_resource_type\x18\x03 \x01(\t\x12\x10\n\x08yaml_key\x18\x04 \x01(\t\x12\x11\n\tfile_path\x18\x05 \x01(\t\"v\n\x1aWrongResourceSchemaFileMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.WrongResourceSchemaFile\"K\n\x10NoNodeForYamlKey\x12\x12\n\npatch_name\x18\x01 \x01(\t\x12\x10\n\x08yaml_key\x18\x02 \x01(\t\x12\x11\n\tfile_path\x18\x03 \x01(\t\"h\n\x13NoNodeForYamlKeyMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.NoNodeForYamlKey\"+\n\x15MacroNotFoundForPatch\x12\x12\n\npatch_name\x18\x01 \x01(\t\"r\n\x18MacroNotFoundForPatchMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.MacroNotFoundForPatch\"\xb8\x01\n\x16NodeNotFoundOrDisabled\x12\x1a\n\x12original_file_path\x18\x01 \x01(\t\x12\x11\n\tunique_id\x18\x02 \x01(\t\x12\x1b\n\x13resource_type_title\x18\x03 \x01(\t\x12\x13\n\x0btarget_name\x18\x04 \x01(\t\x12\x13\n\x0btarget_kind\x18\x05 \x01(\t\x12\x16\n\x0etarget_package\x18\x06 \x01(\t\x12\x10\n\x08\x64isabled\x18\x07 \x01(\t\"t\n\x19NodeNotFoundOrDisabledMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.NodeNotFoundOrDisabled\"H\n\x0fJinjaLogWarning\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03msg\x18\x02 \x01(\t\"f\n\x12JinjaLogWarningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.JinjaLogWarning\"E\n\x0cJinjaLogInfo\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03msg\x18\x02 \x01(\t\"`\n\x0fJinjaLogInfoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.JinjaLogInfo\"F\n\rJinjaLogDebug\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03msg\x18\x02 \x01(\t\"b\n\x10JinjaLogDebugMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.JinjaLogDebug\"\xae\x01\n\x1eUnpinnedRefNewVersionAvailable\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x15\n\rref_node_name\x18\x02 \x01(\t\x12\x18\n\x10ref_node_package\x18\x03 \x01(\t\x12\x18\n\x10ref_node_version\x18\x04 \x01(\t\x12\x17\n\x0fref_max_version\x18\x05 \x01(\t\"\x84\x01\n!UnpinnedRefNewVersionAvailableMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.UnpinnedRefNewVersionAvailable\"/\n\x1dGitSparseCheckoutSubdirectory\x12\x0e\n\x06subdir\x18\x01 \x01(\t\"\x82\x01\n GitSparseCheckoutSubdirectoryMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.GitSparseCheckoutSubdirectory\"/\n\x1bGitProgressCheckoutRevision\x12\x10\n\x08revision\x18\x01 \x01(\t\"~\n\x1eGitProgressCheckoutRevisionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.GitProgressCheckoutRevision\"4\n%GitProgressUpdatingExistingDependency\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"\x92\x01\n(GitProgressUpdatingExistingDependencyMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12@\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x32.proto_types.GitProgressUpdatingExistingDependency\".\n\x1fGitProgressPullingNewDependency\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"\x86\x01\n\"GitProgressPullingNewDependencyMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.GitProgressPullingNewDependency\"\x1d\n\x0eGitNothingToDo\x12\x0b\n\x03sha\x18\x01 \x01(\t\"d\n\x11GitNothingToDoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.GitNothingToDo\"E\n\x1fGitProgressUpdatedCheckoutRange\x12\x11\n\tstart_sha\x18\x01 \x01(\t\x12\x0f\n\x07\x65nd_sha\x18\x02 \x01(\t\"\x86\x01\n\"GitProgressUpdatedCheckoutRangeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.GitProgressUpdatedCheckoutRange\"*\n\x17GitProgressCheckedOutAt\x12\x0f\n\x07\x65nd_sha\x18\x01 \x01(\t\"v\n\x1aGitProgressCheckedOutAtMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.GitProgressCheckedOutAt\")\n\x1aRegistryProgressGETRequest\x12\x0b\n\x03url\x18\x01 \x01(\t\"|\n\x1dRegistryProgressGETRequestMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.RegistryProgressGETRequest\"=\n\x1bRegistryProgressGETResponse\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x11\n\tresp_code\x18\x02 \x01(\x05\"~\n\x1eRegistryProgressGETResponseMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.RegistryProgressGETResponse\"_\n\x1dSelectorReportInvalidSelector\x12\x17\n\x0fvalid_selectors\x18\x01 \x01(\t\x12\x13\n\x0bspec_method\x18\x02 \x01(\t\x12\x10\n\x08raw_spec\x18\x03 \x01(\t\"\x82\x01\n SelectorReportInvalidSelectorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.SelectorReportInvalidSelector\"\x15\n\x13\x44\x65psNoPackagesFound\"n\n\x16\x44\x65psNoPackagesFoundMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.DepsNoPackagesFound\"/\n\x17\x44\x65psStartPackageInstall\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\"v\n\x1a\x44\x65psStartPackageInstallMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.DepsStartPackageInstall\"\'\n\x0f\x44\x65psInstallInfo\x12\x14\n\x0cversion_name\x18\x01 \x01(\t\"f\n\x12\x44\x65psInstallInfoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DepsInstallInfo\"-\n\x13\x44\x65psUpdateAvailable\x12\x16\n\x0eversion_latest\x18\x01 \x01(\t\"n\n\x16\x44\x65psUpdateAvailableMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.DepsUpdateAvailable\"\x0e\n\x0c\x44\x65psUpToDate\"`\n\x0f\x44\x65psUpToDateMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.DepsUpToDate\",\n\x14\x44\x65psListSubdirectory\x12\x14\n\x0csubdirectory\x18\x01 \x01(\t\"p\n\x17\x44\x65psListSubdirectoryMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.DepsListSubdirectory\".\n\x1a\x44\x65psNotifyUpdatesAvailable\x12\x10\n\x08packages\x18\x01 \x03(\t\"|\n\x1d\x44\x65psNotifyUpdatesAvailableMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.DepsNotifyUpdatesAvailable\"1\n\x11RetryExternalCall\x12\x0f\n\x07\x61ttempt\x18\x01 \x01(\x05\x12\x0b\n\x03max\x18\x02 \x01(\x05\"j\n\x14RetryExternalCallMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.RetryExternalCall\"#\n\x14RecordRetryException\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"p\n\x17RecordRetryExceptionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.RecordRetryException\".\n\x1fRegistryIndexProgressGETRequest\x12\x0b\n\x03url\x18\x01 \x01(\t\"\x86\x01\n\"RegistryIndexProgressGETRequestMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.RegistryIndexProgressGETRequest\"B\n RegistryIndexProgressGETResponse\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x11\n\tresp_code\x18\x02 \x01(\x05\"\x88\x01\n#RegistryIndexProgressGETResponseMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12;\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32-.proto_types.RegistryIndexProgressGETResponse\"2\n\x1eRegistryResponseUnexpectedType\x12\x10\n\x08response\x18\x01 \x01(\t\"\x84\x01\n!RegistryResponseUnexpectedTypeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.RegistryResponseUnexpectedType\"2\n\x1eRegistryResponseMissingTopKeys\x12\x10\n\x08response\x18\x01 \x01(\t\"\x84\x01\n!RegistryResponseMissingTopKeysMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.RegistryResponseMissingTopKeys\"5\n!RegistryResponseMissingNestedKeys\x12\x10\n\x08response\x18\x01 \x01(\t\"\x8a\x01\n$RegistryResponseMissingNestedKeysMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12<\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32..proto_types.RegistryResponseMissingNestedKeys\"3\n\x1fRegistryResponseExtraNestedKeys\x12\x10\n\x08response\x18\x01 \x01(\t\"\x86\x01\n\"RegistryResponseExtraNestedKeysMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.RegistryResponseExtraNestedKeys\"(\n\x18\x44\x65psSetDownloadDirectory\x12\x0c\n\x04path\x18\x01 \x01(\t\"x\n\x1b\x44\x65psSetDownloadDirectoryMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.DepsSetDownloadDirectory\"-\n\x0c\x44\x65psUnpinned\x12\x10\n\x08revision\x18\x01 \x01(\t\x12\x0b\n\x03git\x18\x02 \x01(\t\"`\n\x0f\x44\x65psUnpinnedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.DepsUnpinned\"/\n\x1bNoNodesForSelectionCriteria\x12\x10\n\x08spec_raw\x18\x01 \x01(\t\"~\n\x1eNoNodesForSelectionCriteriaMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.NoNodesForSelectionCriteria\"*\n\x1bRunningOperationCaughtError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"~\n\x1eRunningOperationCaughtErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.RunningOperationCaughtError\"\x11\n\x0f\x43ompileComplete\"f\n\x12\x43ompileCompleteMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.CompileComplete\"\x18\n\x16\x46reshnessCheckComplete\"t\n\x19\x46reshnessCheckCompleteMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.FreshnessCheckComplete\"\x1c\n\nSeedHeader\x12\x0e\n\x06header\x18\x01 \x01(\t\"\\\n\rSeedHeaderMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.SeedHeader\"3\n\x12SQLRunnerException\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x02 \x01(\t\"l\n\x15SQLRunnerExceptionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.SQLRunnerException\"\xa8\x01\n\rLogTestResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\x12\n\nnum_models\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\x12\x14\n\x0cnum_failures\x18\x07 \x01(\x05\"b\n\x10LogTestResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.LogTestResult\"k\n\x0cLogStartLine\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"`\n\x0fLogStartLineMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.LogStartLine\"\x95\x01\n\x0eLogModelResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\"d\n\x11LogModelResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.LogModelResult\"\xfa\x01\n\x11LogSnapshotResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\x12\x34\n\x03\x63\x66g\x18\x07 \x03(\x0b\x32\'.proto_types.LogSnapshotResult.CfgEntry\x1a*\n\x08\x43\x66gEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"j\n\x14LogSnapshotResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.LogSnapshotResult\"\xb9\x01\n\rLogSeedResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x16\n\x0eresult_message\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\x12\x0e\n\x06schema\x18\x07 \x01(\t\x12\x10\n\x08relation\x18\x08 \x01(\t\"b\n\x10LogSeedResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.LogSeedResult\"\xad\x01\n\x12LogFreshnessResult\x12\x0e\n\x06status\x18\x01 \x01(\t\x12(\n\tnode_info\x18\x02 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x05 \x01(\x02\x12\x13\n\x0bsource_name\x18\x06 \x01(\t\x12\x12\n\ntable_name\x18\x07 \x01(\t\"l\n\x15LogFreshnessResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogFreshnessResult\"\"\n\rLogCancelLine\x12\x11\n\tconn_name\x18\x01 \x01(\t\"b\n\x10LogCancelLineMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.LogCancelLine\"\x1f\n\x0f\x44\x65\x66\x61ultSelector\x12\x0c\n\x04name\x18\x01 \x01(\t\"f\n\x12\x44\x65\x66\x61ultSelectorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DefaultSelector\"5\n\tNodeStart\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"Z\n\x0cNodeStartMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12$\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.proto_types.NodeStart\"g\n\x0cNodeFinished\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12-\n\nrun_result\x18\x02 \x01(\x0b\x32\x19.proto_types.RunResultMsg\"`\n\x0fNodeFinishedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.NodeFinished\"+\n\x1bQueryCancelationUnsupported\x12\x0c\n\x04type\x18\x01 \x01(\t\"~\n\x1eQueryCancelationUnsupportedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.QueryCancelationUnsupported\"O\n\x0f\x43oncurrencyLine\x12\x13\n\x0bnum_threads\x18\x01 \x01(\x05\x12\x13\n\x0btarget_name\x18\x02 \x01(\t\x12\x12\n\nnode_count\x18\x03 \x01(\x05\"f\n\x12\x43oncurrencyLineMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.ConcurrencyLine\"E\n\x19WritingInjectedSQLForNode\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"z\n\x1cWritingInjectedSQLForNodeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.WritingInjectedSQLForNode\"9\n\rNodeCompiling\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"b\n\x10NodeCompilingMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.NodeCompiling\"9\n\rNodeExecuting\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"b\n\x10NodeExecutingMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.NodeExecuting\"m\n\x10LogHookStartLine\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tstatement\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"h\n\x13LogHookStartLineMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.LogHookStartLine\"\x93\x01\n\x0eLogHookEndLine\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tstatement\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\"d\n\x11LogHookEndLineMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.LogHookEndLine\"\x93\x01\n\x0fSkippingDetails\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x15\n\rresource_type\x18\x02 \x01(\t\x12\x0e\n\x06schema\x18\x03 \x01(\t\x12\x11\n\tnode_name\x18\x04 \x01(\t\x12\r\n\x05index\x18\x05 \x01(\x05\x12\r\n\x05total\x18\x06 \x01(\x05\"f\n\x12SkippingDetailsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.SkippingDetails\"\r\n\x0bNothingToDo\"^\n\x0eNothingToDoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.NothingToDo\",\n\x1dRunningOperationUncaughtError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"\x82\x01\n RunningOperationUncaughtErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.RunningOperationUncaughtError\"\x93\x01\n\x0c\x45ndRunResult\x12*\n\x07results\x18\x01 \x03(\x0b\x32\x19.proto_types.RunResultMsg\x12\x14\n\x0c\x65lapsed_time\x18\x02 \x01(\x02\x12\x30\n\x0cgenerated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07success\x18\x04 \x01(\x08\"`\n\x0f\x45ndRunResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.EndRunResult\"\x11\n\x0fNoNodesSelected\"f\n\x12NoNodesSelectedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.NoNodesSelected\"w\n\x10\x43ommandCompleted\x12\x0f\n\x07\x63ommand\x18\x01 \x01(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x30\n\x0c\x63ompleted_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07\x65lapsed\x18\x04 \x01(\x02\"h\n\x13\x43ommandCompletedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.CommandCompleted\"k\n\x08ShowNode\x12\x11\n\tnode_name\x18\x01 \x01(\t\x12\x0f\n\x07preview\x18\x02 \x01(\t\x12\x11\n\tis_inline\x18\x03 \x01(\x08\x12\x15\n\routput_format\x18\x04 \x01(\t\x12\x11\n\tunique_id\x18\x05 \x01(\t\"X\n\x0bShowNodeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12#\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x15.proto_types.ShowNode\"p\n\x0c\x43ompiledNode\x12\x11\n\tnode_name\x18\x01 \x01(\t\x12\x10\n\x08\x63ompiled\x18\x02 \x01(\t\x12\x11\n\tis_inline\x18\x03 \x01(\x08\x12\x15\n\routput_format\x18\x04 \x01(\t\x12\x11\n\tunique_id\x18\x05 \x01(\t\"`\n\x0f\x43ompiledNodeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.CompiledNode\"b\n\x17\x43\x61tchableExceptionOnRun\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"v\n\x1a\x43\x61tchableExceptionOnRunMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.CatchableExceptionOnRun\"5\n\x12InternalErrorOnRun\x12\x12\n\nbuild_path\x18\x01 \x01(\t\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\"l\n\x15InternalErrorOnRunMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.InternalErrorOnRun\"K\n\x15GenericExceptionOnRun\x12\x12\n\nbuild_path\x18\x01 \x01(\t\x12\x11\n\tunique_id\x18\x02 \x01(\t\x12\x0b\n\x03\x65xc\x18\x03 \x01(\t\"r\n\x18GenericExceptionOnRunMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.GenericExceptionOnRun\"N\n\x1aNodeConnectionReleaseError\x12\x11\n\tnode_name\x18\x01 \x01(\t\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"|\n\x1dNodeConnectionReleaseErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.NodeConnectionReleaseError\"\x1f\n\nFoundStats\x12\x11\n\tstat_line\x18\x01 \x01(\t\"\\\n\rFoundStatsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.FoundStats\"\x17\n\x15MainKeyboardInterrupt\"r\n\x18MainKeyboardInterruptMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.MainKeyboardInterrupt\"#\n\x14MainEncounteredError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"p\n\x17MainEncounteredErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.MainEncounteredError\"%\n\x0eMainStackTrace\x12\x13\n\x0bstack_trace\x18\x01 \x01(\t\"d\n\x11MainStackTraceMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.MainStackTrace\"@\n\x13SystemCouldNotWrite\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x0b\n\x03\x65xc\x18\x03 \x01(\t\"n\n\x16SystemCouldNotWriteMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.SystemCouldNotWrite\"!\n\x12SystemExecutingCmd\x12\x0b\n\x03\x63md\x18\x01 \x03(\t\"l\n\x15SystemExecutingCmdMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.SystemExecutingCmd\"\x1c\n\x0cSystemStdOut\x12\x0c\n\x04\x62msg\x18\x01 \x01(\t\"`\n\x0fSystemStdOutMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.SystemStdOut\"\x1c\n\x0cSystemStdErr\x12\x0c\n\x04\x62msg\x18\x01 \x01(\t\"`\n\x0fSystemStdErrMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.SystemStdErr\",\n\x16SystemReportReturnCode\x12\x12\n\nreturncode\x18\x01 \x01(\x05\"t\n\x19SystemReportReturnCodeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.SystemReportReturnCode\"p\n\x13TimingInfoCollected\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12/\n\x0btiming_info\x18\x02 \x01(\x0b\x32\x1a.proto_types.TimingInfoMsg\"n\n\x16TimingInfoCollectedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.TimingInfoCollected\"&\n\x12LogDebugStackTrace\x12\x10\n\x08\x65xc_info\x18\x01 \x01(\t\"l\n\x15LogDebugStackTraceMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogDebugStackTrace\"\x1e\n\x0e\x43heckCleanPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"d\n\x11\x43heckCleanPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.CheckCleanPath\" \n\x10\x43onfirmCleanPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"h\n\x13\x43onfirmCleanPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.ConfirmCleanPath\"\"\n\x12ProtectedCleanPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"l\n\x15ProtectedCleanPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.ProtectedCleanPath\"\x14\n\x12\x46inishedCleanPaths\"l\n\x15\x46inishedCleanPathsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.FinishedCleanPaths\"5\n\x0bOpenCommand\x12\x10\n\x08open_cmd\x18\x01 \x01(\t\x12\x14\n\x0cprofiles_dir\x18\x02 \x01(\t\"^\n\x0eOpenCommandMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.OpenCommand\"\x19\n\nFormatting\x12\x0b\n\x03msg\x18\x01 \x01(\t\"\\\n\rFormattingMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.Formatting\"0\n\x0fServingDocsPort\x12\x0f\n\x07\x61\x64\x64ress\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\"f\n\x12ServingDocsPortMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.ServingDocsPort\"%\n\x15ServingDocsAccessInfo\x12\x0c\n\x04port\x18\x01 \x01(\t\"r\n\x18ServingDocsAccessInfoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.ServingDocsAccessInfo\"\x15\n\x13ServingDocsExitInfo\"n\n\x16ServingDocsExitInfoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.ServingDocsExitInfo\"J\n\x10RunResultWarning\x12\x15\n\rresource_type\x18\x01 \x01(\t\x12\x11\n\tnode_name\x18\x02 \x01(\t\x12\x0c\n\x04path\x18\x03 \x01(\t\"h\n\x13RunResultWarningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.RunResultWarning\"J\n\x10RunResultFailure\x12\x15\n\rresource_type\x18\x01 \x01(\t\x12\x11\n\tnode_name\x18\x02 \x01(\t\x12\x0c\n\x04path\x18\x03 \x01(\t\"h\n\x13RunResultFailureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.RunResultFailure\"k\n\tStatsLine\x12\x30\n\x05stats\x18\x01 \x03(\x0b\x32!.proto_types.StatsLine.StatsEntry\x1a,\n\nStatsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\"Z\n\x0cStatsLineMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12$\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.proto_types.StatsLine\"\x1d\n\x0eRunResultError\x12\x0b\n\x03msg\x18\x01 \x01(\t\"d\n\x11RunResultErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.RunResultError\")\n\x17RunResultErrorNoMessage\x12\x0e\n\x06status\x18\x01 \x01(\t\"v\n\x1aRunResultErrorNoMessageMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.RunResultErrorNoMessage\"\x1f\n\x0fSQLCompiledPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"f\n\x12SQLCompiledPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.SQLCompiledPath\"-\n\x14\x43heckNodeTestFailure\x12\x15\n\rrelation_name\x18\x01 \x01(\t\"p\n\x17\x43heckNodeTestFailureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.CheckNodeTestFailure\"\"\n\x13\x46irstRunResultError\x12\x0b\n\x03msg\x18\x01 \x01(\t\"n\n\x16\x46irstRunResultErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.FirstRunResultError\"\'\n\x18\x41\x66terFirstRunResultError\x12\x0b\n\x03msg\x18\x01 \x01(\t\"x\n\x1b\x41\x66terFirstRunResultErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.AfterFirstRunResultError\"W\n\x0f\x45ndOfRunSummary\x12\x12\n\nnum_errors\x18\x01 \x01(\x05\x12\x14\n\x0cnum_warnings\x18\x02 \x01(\x05\x12\x1a\n\x12keyboard_interrupt\x18\x03 \x01(\x08\"f\n\x12\x45ndOfRunSummaryMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.EndOfRunSummary\"U\n\x13LogSkipBecauseError\x12\x0e\n\x06schema\x18\x01 \x01(\t\x12\x10\n\x08relation\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"n\n\x16LogSkipBecauseErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.LogSkipBecauseError\"\x14\n\x12\x45nsureGitInstalled\"l\n\x15\x45nsureGitInstalledMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.EnsureGitInstalled\"\x1a\n\x18\x44\x65psCreatingLocalSymlink\"x\n\x1b\x44\x65psCreatingLocalSymlinkMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.DepsCreatingLocalSymlink\"\x19\n\x17\x44\x65psSymlinkNotAvailable\"v\n\x1a\x44\x65psSymlinkNotAvailableMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.DepsSymlinkNotAvailable\"\x11\n\x0f\x44isableTracking\"f\n\x12\x44isableTrackingMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DisableTracking\"\x1e\n\x0cSendingEvent\x12\x0e\n\x06kwargs\x18\x01 \x01(\t\"`\n\x0fSendingEventMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.SendingEvent\"\x12\n\x10SendEventFailure\"h\n\x13SendEventFailureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.SendEventFailure\"\r\n\x0b\x46lushEvents\"^\n\x0e\x46lushEventsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.FlushEvents\"\x14\n\x12\x46lushEventsFailure\"l\n\x15\x46lushEventsFailureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.FlushEventsFailure\"-\n\x19TrackingInitializeFailure\x12\x10\n\x08\x65xc_info\x18\x01 \x01(\t\"z\n\x1cTrackingInitializeFailureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.TrackingInitializeFailure\"&\n\x17RunResultWarningMessage\x12\x0b\n\x03msg\x18\x01 \x01(\t\"v\n\x1aRunResultWarningMessageMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.RunResultWarningMessage\"\x1a\n\x0b\x44\x65\x62ugCmdOut\x12\x0b\n\x03msg\x18\x01 \x01(\t\"^\n\x0e\x44\x65\x62ugCmdOutMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.DebugCmdOut\"\x1d\n\x0e\x44\x65\x62ugCmdResult\x12\x0b\n\x03msg\x18\x01 \x01(\t\"d\n\x11\x44\x65\x62ugCmdResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.DebugCmdResult\"\x19\n\nListCmdOut\x12\x0b\n\x03msg\x18\x01 \x01(\t\"\\\n\rListCmdOutMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.ListCmdOut\"\x13\n\x04Note\x12\x0b\n\x03msg\x18\x01 \x01(\t\"P\n\x07NoteMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x1f\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x11.proto_types.Noteb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0btypes.proto\x12\x0bproto_types\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1cgoogle/protobuf/struct.proto\"\x91\x02\n\tEventInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x0b\n\x03msg\x18\x03 \x01(\t\x12\r\n\x05level\x18\x04 \x01(\t\x12\x15\n\rinvocation_id\x18\x05 \x01(\t\x12\x0b\n\x03pid\x18\x06 \x01(\x05\x12\x0e\n\x06thread\x18\x07 \x01(\t\x12&\n\x02ts\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x05\x65xtra\x18\t \x03(\x0b\x32!.proto_types.EventInfo.ExtraEntry\x12\x10\n\x08\x63\x61tegory\x18\n \x01(\t\x1a,\n\nExtraEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x7f\n\rTimingInfoMsg\x12\x0c\n\x04name\x18\x01 \x01(\t\x12.\n\nstarted_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0c\x63ompleted_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"V\n\x0cNodeRelation\x12\x10\n\x08\x64\x61tabase\x18\n \x01(\t\x12\x0e\n\x06schema\x18\x0b \x01(\t\x12\r\n\x05\x61lias\x18\x0c \x01(\t\x12\x15\n\rrelation_name\x18\r \x01(\t\"\x91\x02\n\x08NodeInfo\x12\x11\n\tnode_path\x18\x01 \x01(\t\x12\x11\n\tnode_name\x18\x02 \x01(\t\x12\x11\n\tunique_id\x18\x03 \x01(\t\x12\x15\n\rresource_type\x18\x04 \x01(\t\x12\x14\n\x0cmaterialized\x18\x05 \x01(\t\x12\x13\n\x0bnode_status\x18\x06 \x01(\t\x12\x17\n\x0fnode_started_at\x18\x07 \x01(\t\x12\x18\n\x10node_finished_at\x18\x08 \x01(\t\x12%\n\x04meta\x18\t \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x30\n\rnode_relation\x18\n \x01(\x0b\x32\x19.proto_types.NodeRelation\"\xd1\x01\n\x0cRunResultMsg\x12\x0e\n\x06status\x18\x01 \x01(\t\x12\x0f\n\x07message\x18\x02 \x01(\t\x12/\n\x0btiming_info\x18\x03 \x03(\x0b\x32\x1a.proto_types.TimingInfoMsg\x12\x0e\n\x06thread\x18\x04 \x01(\t\x12\x16\n\x0e\x65xecution_time\x18\x05 \x01(\x02\x12\x31\n\x10\x61\x64\x61pter_response\x18\x06 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x14\n\x0cnum_failures\x18\x07 \x01(\x05\"G\n\x0fReferenceKeyMsg\x12\x10\n\x08\x64\x61tabase\x18\x01 \x01(\t\x12\x0e\n\x06schema\x18\x02 \x01(\t\x12\x12\n\nidentifier\x18\x03 \x01(\t\"6\n\x0eGenericMessage\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\"9\n\x11MainReportVersion\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x13\n\x0blog_version\x18\x02 \x01(\x05\"j\n\x14MainReportVersionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.MainReportVersion\"r\n\x0eMainReportArgs\x12\x33\n\x04\x61rgs\x18\x01 \x03(\x0b\x32%.proto_types.MainReportArgs.ArgsEntry\x1a+\n\tArgsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"d\n\x11MainReportArgsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.MainReportArgs\"+\n\x15MainTrackingUserState\x12\x12\n\nuser_state\x18\x01 \x01(\t\"r\n\x18MainTrackingUserStateMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.MainTrackingUserState\"5\n\x0fMergedFromState\x12\x12\n\nnum_merged\x18\x01 \x01(\x05\x12\x0e\n\x06sample\x18\x02 \x03(\t\"f\n\x12MergedFromStateMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.MergedFromState\"A\n\x14MissingProfileTarget\x12\x14\n\x0cprofile_name\x18\x01 \x01(\t\x12\x13\n\x0btarget_name\x18\x02 \x01(\t\"p\n\x17MissingProfileTargetMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.MissingProfileTarget\"(\n\x11InvalidOptionYAML\x12\x13\n\x0boption_name\x18\x01 \x01(\t\"j\n\x14InvalidOptionYAMLMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.InvalidOptionYAML\"!\n\x12LogDbtProjectError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"l\n\x15LogDbtProjectErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogDbtProjectError\"3\n\x12LogDbtProfileError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\x12\x10\n\x08profiles\x18\x02 \x03(\t\"l\n\x15LogDbtProfileErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogDbtProfileError\"!\n\x12StarterProjectPath\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"l\n\x15StarterProjectPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.StarterProjectPath\"$\n\x15\x43onfigFolderDirectory\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"r\n\x18\x43onfigFolderDirectoryMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.ConfigFolderDirectory\"\'\n\x14NoSampleProfileFound\x12\x0f\n\x07\x61\x64\x61pter\x18\x01 \x01(\t\"p\n\x17NoSampleProfileFoundMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.NoSampleProfileFound\"6\n\x18ProfileWrittenWithSample\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"x\n\x1bProfileWrittenWithSampleMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.ProfileWrittenWithSample\"B\n$ProfileWrittenWithTargetTemplateYAML\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"\x90\x01\n\'ProfileWrittenWithTargetTemplateYAMLMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12?\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x31.proto_types.ProfileWrittenWithTargetTemplateYAML\"C\n%ProfileWrittenWithProjectTemplateYAML\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"\x92\x01\n(ProfileWrittenWithProjectTemplateYAMLMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12@\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x32.proto_types.ProfileWrittenWithProjectTemplateYAML\"\x12\n\x10SettingUpProfile\"h\n\x13SettingUpProfileMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.SettingUpProfile\"\x1c\n\x1aInvalidProfileTemplateYAML\"|\n\x1dInvalidProfileTemplateYAMLMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.InvalidProfileTemplateYAML\"(\n\x18ProjectNameAlreadyExists\x12\x0c\n\x04name\x18\x01 \x01(\t\"x\n\x1bProjectNameAlreadyExistsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.ProjectNameAlreadyExists\"K\n\x0eProjectCreated\x12\x14\n\x0cproject_name\x18\x01 \x01(\t\x12\x10\n\x08\x64ocs_url\x18\x02 \x01(\t\x12\x11\n\tslack_url\x18\x03 \x01(\t\"d\n\x11ProjectCreatedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.ProjectCreated\"@\n\x1aPackageRedirectDeprecation\x12\x10\n\x08old_name\x18\x01 \x01(\t\x12\x10\n\x08new_name\x18\x02 \x01(\t\"|\n\x1dPackageRedirectDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.PackageRedirectDeprecation\"\x1f\n\x1dPackageInstallPathDeprecation\"\x82\x01\n PackageInstallPathDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.PackageInstallPathDeprecation\"H\n\x1b\x43onfigSourcePathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\x12\x10\n\x08\x65xp_path\x18\x02 \x01(\t\"~\n\x1e\x43onfigSourcePathDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.ConfigSourcePathDeprecation\"F\n\x19\x43onfigDataPathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\x12\x10\n\x08\x65xp_path\x18\x02 \x01(\t\"z\n\x1c\x43onfigDataPathDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.ConfigDataPathDeprecation\"?\n\x19\x41\x64\x61pterDeprecationWarning\x12\x10\n\x08old_name\x18\x01 \x01(\t\x12\x10\n\x08new_name\x18\x02 \x01(\t\"z\n\x1c\x41\x64\x61pterDeprecationWarningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.AdapterDeprecationWarning\".\n\x17MetricAttributesRenamed\x12\x13\n\x0bmetric_name\x18\x01 \x01(\t\"v\n\x1aMetricAttributesRenamedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.MetricAttributesRenamed\"+\n\x17\x45xposureNameDeprecation\x12\x10\n\x08\x65xposure\x18\x01 \x01(\t\"v\n\x1a\x45xposureNameDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.ExposureNameDeprecation\"^\n\x13InternalDeprecation\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x18\n\x10suggested_action\x18\x03 \x01(\t\x12\x0f\n\x07version\x18\x04 \x01(\t\"n\n\x16InternalDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.InternalDeprecation\"@\n\x1a\x45nvironmentVariableRenamed\x12\x10\n\x08old_name\x18\x01 \x01(\t\x12\x10\n\x08new_name\x18\x02 \x01(\t\"|\n\x1d\x45nvironmentVariableRenamedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.EnvironmentVariableRenamed\"3\n\x18\x43onfigLogPathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\"x\n\x1b\x43onfigLogPathDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.ConfigLogPathDeprecation\"6\n\x1b\x43onfigTargetPathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\"~\n\x1e\x43onfigTargetPathDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.ConfigTargetPathDeprecation\"\x87\x01\n\x11\x41\x64\x61pterEventDebug\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61se_msg\x18\x03 \x01(\t\x12(\n\x04\x61rgs\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.ListValue\"j\n\x14\x41\x64\x61pterEventDebugMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.AdapterEventDebug\"\x86\x01\n\x10\x41\x64\x61pterEventInfo\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61se_msg\x18\x03 \x01(\t\x12(\n\x04\x61rgs\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.ListValue\"h\n\x13\x41\x64\x61pterEventInfoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.AdapterEventInfo\"\x89\x01\n\x13\x41\x64\x61pterEventWarning\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61se_msg\x18\x03 \x01(\t\x12(\n\x04\x61rgs\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.ListValue\"n\n\x16\x41\x64\x61pterEventWarningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.AdapterEventWarning\"\x99\x01\n\x11\x41\x64\x61pterEventError\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61se_msg\x18\x03 \x01(\t\x12(\n\x04\x61rgs\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12\x10\n\x08\x65xc_info\x18\x05 \x01(\t\"j\n\x14\x41\x64\x61pterEventErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.AdapterEventError\"_\n\rNewConnection\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_type\x18\x02 \x01(\t\x12\x11\n\tconn_name\x18\x03 \x01(\t\"b\n\x10NewConnectionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.NewConnection\"=\n\x10\x43onnectionReused\x12\x11\n\tconn_name\x18\x01 \x01(\t\x12\x16\n\x0eorig_conn_name\x18\x02 \x01(\t\"h\n\x13\x43onnectionReusedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.ConnectionReused\"0\n\x1b\x43onnectionLeftOpenInCleanup\x12\x11\n\tconn_name\x18\x01 \x01(\t\"~\n\x1e\x43onnectionLeftOpenInCleanupMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.ConnectionLeftOpenInCleanup\".\n\x19\x43onnectionClosedInCleanup\x12\x11\n\tconn_name\x18\x01 \x01(\t\"z\n\x1c\x43onnectionClosedInCleanupMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.ConnectionClosedInCleanup\"_\n\x0eRollbackFailed\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"d\n\x11RollbackFailedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.RollbackFailed\"O\n\x10\x43onnectionClosed\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\"h\n\x13\x43onnectionClosedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.ConnectionClosed\"\x85\x01\n\x0fInDBTEventDebug\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61se_msg\x18\x03 \x01(\t\x12(\n\x04\x61rgs\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.ListValue\"f\n\x12InDBTEventDebugMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.InDBTEventDebug\"\x84\x01\n\x0eInDBTEventInfo\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61se_msg\x18\x03 \x01(\t\x12(\n\x04\x61rgs\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.ListValue\"d\n\x11InDBTEventInfoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.InDBTEventInfo\"\x87\x01\n\x11InDBTEventWarning\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61se_msg\x18\x03 \x01(\t\x12(\n\x04\x61rgs\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.ListValue\"j\n\x14InDBTEventWarningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.InDBTEventWarning\"\x97\x01\n\x0fInDBTEventError\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61se_msg\x18\x03 \x01(\t\x12(\n\x04\x61rgs\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12\x10\n\x08\x65xc_info\x18\x05 \x01(\t\"f\n\x12InDBTEventErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.InDBTEventError\"Q\n\x12\x43onnectionLeftOpen\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\"l\n\x15\x43onnectionLeftOpenMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.ConnectionLeftOpen\"G\n\x08Rollback\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\"X\n\x0bRollbackMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12#\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x15.proto_types.Rollback\"@\n\tCacheMiss\x12\x11\n\tconn_name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tabase\x18\x02 \x01(\t\x12\x0e\n\x06schema\x18\x03 \x01(\t\"Z\n\x0c\x43\x61\x63heMissMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12$\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.proto_types.CacheMiss\"b\n\rListRelations\x12\x10\n\x08\x64\x61tabase\x18\x01 \x01(\t\x12\x0e\n\x06schema\x18\x02 \x01(\t\x12/\n\trelations\x18\x03 \x03(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"b\n\x10ListRelationsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.ListRelations\"`\n\x0e\x43onnectionUsed\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_type\x18\x02 \x01(\t\x12\x11\n\tconn_name\x18\x03 \x01(\t\"d\n\x11\x43onnectionUsedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.ConnectionUsed\"T\n\x08SQLQuery\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\x12\x0b\n\x03sql\x18\x03 \x01(\t\"X\n\x0bSQLQueryMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12#\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x15.proto_types.SQLQuery\"[\n\x0eSQLQueryStatus\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x0f\n\x07\x65lapsed\x18\x03 \x01(\x02\"d\n\x11SQLQueryStatusMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.SQLQueryStatus\"H\n\tSQLCommit\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\"Z\n\x0cSQLCommitMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12$\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.proto_types.SQLCommit\"a\n\rColTypeChange\x12\x11\n\torig_type\x18\x01 \x01(\t\x12\x10\n\x08new_type\x18\x02 \x01(\t\x12+\n\x05table\x18\x03 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"b\n\x10\x43olTypeChangeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.ColTypeChange\"@\n\x0eSchemaCreation\x12.\n\x08relation\x18\x01 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"d\n\x11SchemaCreationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.SchemaCreation\"<\n\nSchemaDrop\x12.\n\x08relation\x18\x01 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"\\\n\rSchemaDropMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.SchemaDrop\"\xde\x01\n\x0b\x43\x61\x63heAction\x12\x0e\n\x06\x61\x63tion\x18\x01 \x01(\t\x12-\n\x07ref_key\x18\x02 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\x12/\n\tref_key_2\x18\x03 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\x12/\n\tref_key_3\x18\x04 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\x12.\n\x08ref_list\x18\x05 \x03(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"^\n\x0e\x43\x61\x63heActionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.CacheAction\"\x98\x01\n\x0e\x43\x61\x63heDumpGraph\x12\x33\n\x04\x64ump\x18\x01 \x03(\x0b\x32%.proto_types.CacheDumpGraph.DumpEntry\x12\x14\n\x0c\x62\x65\x66ore_after\x18\x02 \x01(\t\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\x1a+\n\tDumpEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"d\n\x11\x43\x61\x63heDumpGraphMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.CacheDumpGraph\"!\n\x12\x41\x64\x61pterImportError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"l\n\x15\x41\x64\x61pterImportErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.AdapterImportError\"#\n\x0fPluginLoadError\x12\x10\n\x08\x65xc_info\x18\x01 \x01(\t\"f\n\x12PluginLoadErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.PluginLoadError\"Z\n\x14NewConnectionOpening\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x18\n\x10\x63onnection_state\x18\x02 \x01(\t\"p\n\x17NewConnectionOpeningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.NewConnectionOpening\"8\n\rCodeExecution\x12\x11\n\tconn_name\x18\x01 \x01(\t\x12\x14\n\x0c\x63ode_content\x18\x02 \x01(\t\"b\n\x10\x43odeExecutionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.CodeExecution\"6\n\x13\x43odeExecutionStatus\x12\x0e\n\x06status\x18\x01 \x01(\t\x12\x0f\n\x07\x65lapsed\x18\x02 \x01(\x02\"n\n\x16\x43odeExecutionStatusMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.CodeExecutionStatus\"%\n\x16\x43\x61talogGenerationError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"t\n\x19\x43\x61talogGenerationErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.CatalogGenerationError\"-\n\x13WriteCatalogFailure\x12\x16\n\x0enum_exceptions\x18\x01 \x01(\x05\"n\n\x16WriteCatalogFailureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.WriteCatalogFailure\"\x1e\n\x0e\x43\x61talogWritten\x12\x0c\n\x04path\x18\x01 \x01(\t\"d\n\x11\x43\x61talogWrittenMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.CatalogWritten\"\x14\n\x12\x43\x61nnotGenerateDocs\"l\n\x15\x43\x61nnotGenerateDocsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.CannotGenerateDocs\"\x11\n\x0f\x42uildingCatalog\"f\n\x12\x42uildingCatalogMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.BuildingCatalog\"-\n\x18\x44\x61tabaseErrorRunningHook\x12\x11\n\thook_type\x18\x01 \x01(\t\"x\n\x1b\x44\x61tabaseErrorRunningHookMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.DatabaseErrorRunningHook\"4\n\x0cHooksRunning\x12\x11\n\tnum_hooks\x18\x01 \x01(\x05\x12\x11\n\thook_type\x18\x02 \x01(\t\"`\n\x0fHooksRunningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.HooksRunning\"T\n\x14\x46inishedRunningStats\x12\x11\n\tstat_line\x18\x01 \x01(\t\x12\x11\n\texecution\x18\x02 \x01(\t\x12\x16\n\x0e\x65xecution_time\x18\x03 \x01(\x02\"p\n\x17\x46inishedRunningStatsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.FinishedRunningStats\"<\n\x15\x43onstraintNotEnforced\x12\x12\n\nconstraint\x18\x01 \x01(\t\x12\x0f\n\x07\x61\x64\x61pter\x18\x02 \x01(\t\"r\n\x18\x43onstraintNotEnforcedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.ConstraintNotEnforced\"=\n\x16\x43onstraintNotSupported\x12\x12\n\nconstraint\x18\x01 \x01(\t\x12\x0f\n\x07\x61\x64\x61pter\x18\x02 \x01(\t\"t\n\x19\x43onstraintNotSupportedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.ConstraintNotSupported\"7\n\x12InputFileDiffError\x12\x10\n\x08\x63\x61tegory\x18\x01 \x01(\t\x12\x0f\n\x07\x66ile_id\x18\x02 \x01(\t\"l\n\x15InputFileDiffErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.InputFileDiffError\"?\n\x14InvalidValueForField\x12\x12\n\nfield_name\x18\x01 \x01(\t\x12\x13\n\x0b\x66ield_value\x18\x02 \x01(\t\"p\n\x17InvalidValueForFieldMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.InvalidValueForField\"Q\n\x11ValidationWarning\x12\x15\n\rresource_type\x18\x01 \x01(\t\x12\x12\n\nfield_name\x18\x02 \x01(\t\x12\x11\n\tnode_name\x18\x03 \x01(\t\"j\n\x14ValidationWarningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.ValidationWarning\"!\n\x11ParsePerfInfoPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"j\n\x14ParsePerfInfoPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.ParsePerfInfoPath\"$\n\x14GenericTestFileParse\x12\x0c\n\x04path\x18\x01 \x01(\t\"p\n\x17GenericTestFileParseMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.GenericTestFileParse\"\x1e\n\x0eMacroFileParse\x12\x0c\n\x04path\x18\x01 \x01(\t\"d\n\x11MacroFileParseMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.MacroFileParse\"1\n!PartialParsingErrorProcessingFile\x12\x0c\n\x04\x66ile\x18\x01 \x01(\t\"\x8a\x01\n$PartialParsingErrorProcessingFileMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12<\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32..proto_types.PartialParsingErrorProcessingFile\"\x86\x01\n\x13PartialParsingError\x12?\n\x08\x65xc_info\x18\x01 \x03(\x0b\x32-.proto_types.PartialParsingError.ExcInfoEntry\x1a.\n\x0c\x45xcInfoEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"n\n\x16PartialParsingErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.PartialParsingError\"\x1b\n\x19PartialParsingSkipParsing\"z\n\x1cPartialParsingSkipParsingMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.PartialParsingSkipParsing\"&\n\x14UnableToPartialParse\x12\x0e\n\x06reason\x18\x01 \x01(\t\"p\n\x17UnableToPartialParseMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.UnableToPartialParse\"f\n\x12StateCheckVarsHash\x12\x10\n\x08\x63hecksum\x18\x01 \x01(\t\x12\x0c\n\x04vars\x18\x02 \x01(\t\x12\x0f\n\x07profile\x18\x03 \x01(\t\x12\x0e\n\x06target\x18\x04 \x01(\t\x12\x0f\n\x07version\x18\x05 \x01(\t\"l\n\x15StateCheckVarsHashMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.StateCheckVarsHash\"\x1a\n\x18PartialParsingNotEnabled\"x\n\x1bPartialParsingNotEnabledMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.PartialParsingNotEnabled\"C\n\x14ParsedFileLoadFailed\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"p\n\x17ParsedFileLoadFailedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.ParsedFileLoadFailed\"H\n\x15PartialParsingEnabled\x12\x0f\n\x07\x64\x65leted\x18\x01 \x01(\x05\x12\r\n\x05\x61\x64\x64\x65\x64\x18\x02 \x01(\x05\x12\x0f\n\x07\x63hanged\x18\x03 \x01(\x05\"r\n\x18PartialParsingEnabledMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.PartialParsingEnabled\"8\n\x12PartialParsingFile\x12\x0f\n\x07\x66ile_id\x18\x01 \x01(\t\x12\x11\n\toperation\x18\x02 \x01(\t\"l\n\x15PartialParsingFileMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.PartialParsingFile\"\xaf\x01\n\x1fInvalidDisabledTargetInTestNode\x12\x1b\n\x13resource_type_title\x18\x01 \x01(\t\x12\x11\n\tunique_id\x18\x02 \x01(\t\x12\x1a\n\x12original_file_path\x18\x03 \x01(\t\x12\x13\n\x0btarget_kind\x18\x04 \x01(\t\x12\x13\n\x0btarget_name\x18\x05 \x01(\t\x12\x16\n\x0etarget_package\x18\x06 \x01(\t\"\x86\x01\n\"InvalidDisabledTargetInTestNodeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.InvalidDisabledTargetInTestNode\"7\n\x18UnusedResourceConfigPath\x12\x1b\n\x13unused_config_paths\x18\x01 \x03(\t\"x\n\x1bUnusedResourceConfigPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.UnusedResourceConfigPath\"3\n\rSeedIncreased\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"b\n\x10SeedIncreasedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.SeedIncreased\">\n\x18SeedExceedsLimitSamePath\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"x\n\x1bSeedExceedsLimitSamePathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.SeedExceedsLimitSamePath\"D\n\x1eSeedExceedsLimitAndPathChanged\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x84\x01\n!SeedExceedsLimitAndPathChangedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.SeedExceedsLimitAndPathChanged\"\\\n\x1fSeedExceedsLimitChecksumChanged\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x15\n\rchecksum_name\x18\x03 \x01(\t\"\x86\x01\n\"SeedExceedsLimitChecksumChangedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.SeedExceedsLimitChecksumChanged\"%\n\x0cUnusedTables\x12\x15\n\runused_tables\x18\x01 \x03(\t\"`\n\x0fUnusedTablesMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.UnusedTables\"\x87\x01\n\x17WrongResourceSchemaFile\x12\x12\n\npatch_name\x18\x01 \x01(\t\x12\x15\n\rresource_type\x18\x02 \x01(\t\x12\x1c\n\x14plural_resource_type\x18\x03 \x01(\t\x12\x10\n\x08yaml_key\x18\x04 \x01(\t\x12\x11\n\tfile_path\x18\x05 \x01(\t\"v\n\x1aWrongResourceSchemaFileMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.WrongResourceSchemaFile\"K\n\x10NoNodeForYamlKey\x12\x12\n\npatch_name\x18\x01 \x01(\t\x12\x10\n\x08yaml_key\x18\x02 \x01(\t\x12\x11\n\tfile_path\x18\x03 \x01(\t\"h\n\x13NoNodeForYamlKeyMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.NoNodeForYamlKey\"+\n\x15MacroNotFoundForPatch\x12\x12\n\npatch_name\x18\x01 \x01(\t\"r\n\x18MacroNotFoundForPatchMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.MacroNotFoundForPatch\"\xb8\x01\n\x16NodeNotFoundOrDisabled\x12\x1a\n\x12original_file_path\x18\x01 \x01(\t\x12\x11\n\tunique_id\x18\x02 \x01(\t\x12\x1b\n\x13resource_type_title\x18\x03 \x01(\t\x12\x13\n\x0btarget_name\x18\x04 \x01(\t\x12\x13\n\x0btarget_kind\x18\x05 \x01(\t\x12\x16\n\x0etarget_package\x18\x06 \x01(\t\x12\x10\n\x08\x64isabled\x18\x07 \x01(\t\"t\n\x19NodeNotFoundOrDisabledMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.NodeNotFoundOrDisabled\"H\n\x0fJinjaLogWarning\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03msg\x18\x02 \x01(\t\"f\n\x12JinjaLogWarningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.JinjaLogWarning\"E\n\x0cJinjaLogInfo\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03msg\x18\x02 \x01(\t\"`\n\x0fJinjaLogInfoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.JinjaLogInfo\"F\n\rJinjaLogDebug\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03msg\x18\x02 \x01(\t\"b\n\x10JinjaLogDebugMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.JinjaLogDebug\"\xae\x01\n\x1eUnpinnedRefNewVersionAvailable\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x15\n\rref_node_name\x18\x02 \x01(\t\x12\x18\n\x10ref_node_package\x18\x03 \x01(\t\x12\x18\n\x10ref_node_version\x18\x04 \x01(\t\x12\x17\n\x0fref_max_version\x18\x05 \x01(\t\"\x84\x01\n!UnpinnedRefNewVersionAvailableMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.UnpinnedRefNewVersionAvailable\"/\n\x1dGitSparseCheckoutSubdirectory\x12\x0e\n\x06subdir\x18\x01 \x01(\t\"\x82\x01\n GitSparseCheckoutSubdirectoryMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.GitSparseCheckoutSubdirectory\"/\n\x1bGitProgressCheckoutRevision\x12\x10\n\x08revision\x18\x01 \x01(\t\"~\n\x1eGitProgressCheckoutRevisionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.GitProgressCheckoutRevision\"4\n%GitProgressUpdatingExistingDependency\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"\x92\x01\n(GitProgressUpdatingExistingDependencyMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12@\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x32.proto_types.GitProgressUpdatingExistingDependency\".\n\x1fGitProgressPullingNewDependency\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"\x86\x01\n\"GitProgressPullingNewDependencyMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.GitProgressPullingNewDependency\"\x1d\n\x0eGitNothingToDo\x12\x0b\n\x03sha\x18\x01 \x01(\t\"d\n\x11GitNothingToDoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.GitNothingToDo\"E\n\x1fGitProgressUpdatedCheckoutRange\x12\x11\n\tstart_sha\x18\x01 \x01(\t\x12\x0f\n\x07\x65nd_sha\x18\x02 \x01(\t\"\x86\x01\n\"GitProgressUpdatedCheckoutRangeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.GitProgressUpdatedCheckoutRange\"*\n\x17GitProgressCheckedOutAt\x12\x0f\n\x07\x65nd_sha\x18\x01 \x01(\t\"v\n\x1aGitProgressCheckedOutAtMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.GitProgressCheckedOutAt\")\n\x1aRegistryProgressGETRequest\x12\x0b\n\x03url\x18\x01 \x01(\t\"|\n\x1dRegistryProgressGETRequestMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.RegistryProgressGETRequest\"=\n\x1bRegistryProgressGETResponse\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x11\n\tresp_code\x18\x02 \x01(\x05\"~\n\x1eRegistryProgressGETResponseMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.RegistryProgressGETResponse\"_\n\x1dSelectorReportInvalidSelector\x12\x17\n\x0fvalid_selectors\x18\x01 \x01(\t\x12\x13\n\x0bspec_method\x18\x02 \x01(\t\x12\x10\n\x08raw_spec\x18\x03 \x01(\t\"\x82\x01\n SelectorReportInvalidSelectorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.SelectorReportInvalidSelector\"\x15\n\x13\x44\x65psNoPackagesFound\"n\n\x16\x44\x65psNoPackagesFoundMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.DepsNoPackagesFound\"/\n\x17\x44\x65psStartPackageInstall\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\"v\n\x1a\x44\x65psStartPackageInstallMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.DepsStartPackageInstall\"\'\n\x0f\x44\x65psInstallInfo\x12\x14\n\x0cversion_name\x18\x01 \x01(\t\"f\n\x12\x44\x65psInstallInfoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DepsInstallInfo\"-\n\x13\x44\x65psUpdateAvailable\x12\x16\n\x0eversion_latest\x18\x01 \x01(\t\"n\n\x16\x44\x65psUpdateAvailableMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.DepsUpdateAvailable\"\x0e\n\x0c\x44\x65psUpToDate\"`\n\x0f\x44\x65psUpToDateMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.DepsUpToDate\",\n\x14\x44\x65psListSubdirectory\x12\x14\n\x0csubdirectory\x18\x01 \x01(\t\"p\n\x17\x44\x65psListSubdirectoryMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.DepsListSubdirectory\".\n\x1a\x44\x65psNotifyUpdatesAvailable\x12\x10\n\x08packages\x18\x01 \x03(\t\"|\n\x1d\x44\x65psNotifyUpdatesAvailableMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.DepsNotifyUpdatesAvailable\"1\n\x11RetryExternalCall\x12\x0f\n\x07\x61ttempt\x18\x01 \x01(\x05\x12\x0b\n\x03max\x18\x02 \x01(\x05\"j\n\x14RetryExternalCallMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.RetryExternalCall\"#\n\x14RecordRetryException\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"p\n\x17RecordRetryExceptionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.RecordRetryException\".\n\x1fRegistryIndexProgressGETRequest\x12\x0b\n\x03url\x18\x01 \x01(\t\"\x86\x01\n\"RegistryIndexProgressGETRequestMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.RegistryIndexProgressGETRequest\"B\n RegistryIndexProgressGETResponse\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x11\n\tresp_code\x18\x02 \x01(\x05\"\x88\x01\n#RegistryIndexProgressGETResponseMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12;\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32-.proto_types.RegistryIndexProgressGETResponse\"2\n\x1eRegistryResponseUnexpectedType\x12\x10\n\x08response\x18\x01 \x01(\t\"\x84\x01\n!RegistryResponseUnexpectedTypeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.RegistryResponseUnexpectedType\"2\n\x1eRegistryResponseMissingTopKeys\x12\x10\n\x08response\x18\x01 \x01(\t\"\x84\x01\n!RegistryResponseMissingTopKeysMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.RegistryResponseMissingTopKeys\"5\n!RegistryResponseMissingNestedKeys\x12\x10\n\x08response\x18\x01 \x01(\t\"\x8a\x01\n$RegistryResponseMissingNestedKeysMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12<\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32..proto_types.RegistryResponseMissingNestedKeys\"3\n\x1fRegistryResponseExtraNestedKeys\x12\x10\n\x08response\x18\x01 \x01(\t\"\x86\x01\n\"RegistryResponseExtraNestedKeysMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.RegistryResponseExtraNestedKeys\"(\n\x18\x44\x65psSetDownloadDirectory\x12\x0c\n\x04path\x18\x01 \x01(\t\"x\n\x1b\x44\x65psSetDownloadDirectoryMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.DepsSetDownloadDirectory\"-\n\x0c\x44\x65psUnpinned\x12\x10\n\x08revision\x18\x01 \x01(\t\x12\x0b\n\x03git\x18\x02 \x01(\t\"`\n\x0f\x44\x65psUnpinnedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.DepsUnpinned\"/\n\x1bNoNodesForSelectionCriteria\x12\x10\n\x08spec_raw\x18\x01 \x01(\t\"~\n\x1eNoNodesForSelectionCriteriaMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.NoNodesForSelectionCriteria\"*\n\x1bRunningOperationCaughtError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"~\n\x1eRunningOperationCaughtErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.RunningOperationCaughtError\"\x11\n\x0f\x43ompileComplete\"f\n\x12\x43ompileCompleteMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.CompileComplete\"\x18\n\x16\x46reshnessCheckComplete\"t\n\x19\x46reshnessCheckCompleteMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.FreshnessCheckComplete\"\x1c\n\nSeedHeader\x12\x0e\n\x06header\x18\x01 \x01(\t\"\\\n\rSeedHeaderMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.SeedHeader\"3\n\x12SQLRunnerException\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x02 \x01(\t\"l\n\x15SQLRunnerExceptionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.SQLRunnerException\"\xa8\x01\n\rLogTestResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\x12\n\nnum_models\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\x12\x14\n\x0cnum_failures\x18\x07 \x01(\x05\"b\n\x10LogTestResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.LogTestResult\"k\n\x0cLogStartLine\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"`\n\x0fLogStartLineMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.LogStartLine\"\x95\x01\n\x0eLogModelResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\"d\n\x11LogModelResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.LogModelResult\"\xfa\x01\n\x11LogSnapshotResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\x12\x34\n\x03\x63\x66g\x18\x07 \x03(\x0b\x32\'.proto_types.LogSnapshotResult.CfgEntry\x1a*\n\x08\x43\x66gEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"j\n\x14LogSnapshotResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.LogSnapshotResult\"\xb9\x01\n\rLogSeedResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x16\n\x0eresult_message\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\x12\x0e\n\x06schema\x18\x07 \x01(\t\x12\x10\n\x08relation\x18\x08 \x01(\t\"b\n\x10LogSeedResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.LogSeedResult\"\xad\x01\n\x12LogFreshnessResult\x12\x0e\n\x06status\x18\x01 \x01(\t\x12(\n\tnode_info\x18\x02 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x05 \x01(\x02\x12\x13\n\x0bsource_name\x18\x06 \x01(\t\x12\x12\n\ntable_name\x18\x07 \x01(\t\"l\n\x15LogFreshnessResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogFreshnessResult\"\"\n\rLogCancelLine\x12\x11\n\tconn_name\x18\x01 \x01(\t\"b\n\x10LogCancelLineMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.LogCancelLine\"\x1f\n\x0f\x44\x65\x66\x61ultSelector\x12\x0c\n\x04name\x18\x01 \x01(\t\"f\n\x12\x44\x65\x66\x61ultSelectorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DefaultSelector\"5\n\tNodeStart\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"Z\n\x0cNodeStartMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12$\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.proto_types.NodeStart\"g\n\x0cNodeFinished\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12-\n\nrun_result\x18\x02 \x01(\x0b\x32\x19.proto_types.RunResultMsg\"`\n\x0fNodeFinishedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.NodeFinished\"+\n\x1bQueryCancelationUnsupported\x12\x0c\n\x04type\x18\x01 \x01(\t\"~\n\x1eQueryCancelationUnsupportedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.QueryCancelationUnsupported\"O\n\x0f\x43oncurrencyLine\x12\x13\n\x0bnum_threads\x18\x01 \x01(\x05\x12\x13\n\x0btarget_name\x18\x02 \x01(\t\x12\x12\n\nnode_count\x18\x03 \x01(\x05\"f\n\x12\x43oncurrencyLineMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.ConcurrencyLine\"E\n\x19WritingInjectedSQLForNode\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"z\n\x1cWritingInjectedSQLForNodeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.WritingInjectedSQLForNode\"9\n\rNodeCompiling\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"b\n\x10NodeCompilingMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.NodeCompiling\"9\n\rNodeExecuting\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"b\n\x10NodeExecutingMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.NodeExecuting\"m\n\x10LogHookStartLine\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tstatement\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"h\n\x13LogHookStartLineMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.LogHookStartLine\"\x93\x01\n\x0eLogHookEndLine\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tstatement\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\"d\n\x11LogHookEndLineMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.LogHookEndLine\"\x93\x01\n\x0fSkippingDetails\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x15\n\rresource_type\x18\x02 \x01(\t\x12\x0e\n\x06schema\x18\x03 \x01(\t\x12\x11\n\tnode_name\x18\x04 \x01(\t\x12\r\n\x05index\x18\x05 \x01(\x05\x12\r\n\x05total\x18\x06 \x01(\x05\"f\n\x12SkippingDetailsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.SkippingDetails\"\r\n\x0bNothingToDo\"^\n\x0eNothingToDoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.NothingToDo\",\n\x1dRunningOperationUncaughtError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"\x82\x01\n RunningOperationUncaughtErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.RunningOperationUncaughtError\"\x93\x01\n\x0c\x45ndRunResult\x12*\n\x07results\x18\x01 \x03(\x0b\x32\x19.proto_types.RunResultMsg\x12\x14\n\x0c\x65lapsed_time\x18\x02 \x01(\x02\x12\x30\n\x0cgenerated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07success\x18\x04 \x01(\x08\"`\n\x0f\x45ndRunResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.EndRunResult\"\x11\n\x0fNoNodesSelected\"f\n\x12NoNodesSelectedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.NoNodesSelected\"w\n\x10\x43ommandCompleted\x12\x0f\n\x07\x63ommand\x18\x01 \x01(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x30\n\x0c\x63ompleted_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07\x65lapsed\x18\x04 \x01(\x02\"h\n\x13\x43ommandCompletedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.CommandCompleted\"k\n\x08ShowNode\x12\x11\n\tnode_name\x18\x01 \x01(\t\x12\x0f\n\x07preview\x18\x02 \x01(\t\x12\x11\n\tis_inline\x18\x03 \x01(\x08\x12\x15\n\routput_format\x18\x04 \x01(\t\x12\x11\n\tunique_id\x18\x05 \x01(\t\"X\n\x0bShowNodeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12#\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x15.proto_types.ShowNode\"p\n\x0c\x43ompiledNode\x12\x11\n\tnode_name\x18\x01 \x01(\t\x12\x10\n\x08\x63ompiled\x18\x02 \x01(\t\x12\x11\n\tis_inline\x18\x03 \x01(\x08\x12\x15\n\routput_format\x18\x04 \x01(\t\x12\x11\n\tunique_id\x18\x05 \x01(\t\"`\n\x0f\x43ompiledNodeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.CompiledNode\"b\n\x17\x43\x61tchableExceptionOnRun\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"v\n\x1a\x43\x61tchableExceptionOnRunMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.CatchableExceptionOnRun\"5\n\x12InternalErrorOnRun\x12\x12\n\nbuild_path\x18\x01 \x01(\t\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\"l\n\x15InternalErrorOnRunMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.InternalErrorOnRun\"K\n\x15GenericExceptionOnRun\x12\x12\n\nbuild_path\x18\x01 \x01(\t\x12\x11\n\tunique_id\x18\x02 \x01(\t\x12\x0b\n\x03\x65xc\x18\x03 \x01(\t\"r\n\x18GenericExceptionOnRunMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.GenericExceptionOnRun\"N\n\x1aNodeConnectionReleaseError\x12\x11\n\tnode_name\x18\x01 \x01(\t\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"|\n\x1dNodeConnectionReleaseErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.NodeConnectionReleaseError\"\x1f\n\nFoundStats\x12\x11\n\tstat_line\x18\x01 \x01(\t\"\\\n\rFoundStatsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.FoundStats\"\x17\n\x15MainKeyboardInterrupt\"r\n\x18MainKeyboardInterruptMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.MainKeyboardInterrupt\"#\n\x14MainEncounteredError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"p\n\x17MainEncounteredErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.MainEncounteredError\"%\n\x0eMainStackTrace\x12\x13\n\x0bstack_trace\x18\x01 \x01(\t\"d\n\x11MainStackTraceMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.MainStackTrace\"@\n\x13SystemCouldNotWrite\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x0b\n\x03\x65xc\x18\x03 \x01(\t\"n\n\x16SystemCouldNotWriteMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.SystemCouldNotWrite\"!\n\x12SystemExecutingCmd\x12\x0b\n\x03\x63md\x18\x01 \x03(\t\"l\n\x15SystemExecutingCmdMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.SystemExecutingCmd\"\x1c\n\x0cSystemStdOut\x12\x0c\n\x04\x62msg\x18\x01 \x01(\t\"`\n\x0fSystemStdOutMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.SystemStdOut\"\x1c\n\x0cSystemStdErr\x12\x0c\n\x04\x62msg\x18\x01 \x01(\t\"`\n\x0fSystemStdErrMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.SystemStdErr\",\n\x16SystemReportReturnCode\x12\x12\n\nreturncode\x18\x01 \x01(\x05\"t\n\x19SystemReportReturnCodeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.SystemReportReturnCode\"p\n\x13TimingInfoCollected\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12/\n\x0btiming_info\x18\x02 \x01(\x0b\x32\x1a.proto_types.TimingInfoMsg\"n\n\x16TimingInfoCollectedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.TimingInfoCollected\"&\n\x12LogDebugStackTrace\x12\x10\n\x08\x65xc_info\x18\x01 \x01(\t\"l\n\x15LogDebugStackTraceMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogDebugStackTrace\"\x1e\n\x0e\x43heckCleanPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"d\n\x11\x43heckCleanPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.CheckCleanPath\" \n\x10\x43onfirmCleanPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"h\n\x13\x43onfirmCleanPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.ConfirmCleanPath\"\"\n\x12ProtectedCleanPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"l\n\x15ProtectedCleanPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.ProtectedCleanPath\"\x14\n\x12\x46inishedCleanPaths\"l\n\x15\x46inishedCleanPathsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.FinishedCleanPaths\"5\n\x0bOpenCommand\x12\x10\n\x08open_cmd\x18\x01 \x01(\t\x12\x14\n\x0cprofiles_dir\x18\x02 \x01(\t\"^\n\x0eOpenCommandMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.OpenCommand\"\x19\n\nFormatting\x12\x0b\n\x03msg\x18\x01 \x01(\t\"\\\n\rFormattingMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.Formatting\"0\n\x0fServingDocsPort\x12\x0f\n\x07\x61\x64\x64ress\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\"f\n\x12ServingDocsPortMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.ServingDocsPort\"%\n\x15ServingDocsAccessInfo\x12\x0c\n\x04port\x18\x01 \x01(\t\"r\n\x18ServingDocsAccessInfoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.ServingDocsAccessInfo\"\x15\n\x13ServingDocsExitInfo\"n\n\x16ServingDocsExitInfoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.ServingDocsExitInfo\"J\n\x10RunResultWarning\x12\x15\n\rresource_type\x18\x01 \x01(\t\x12\x11\n\tnode_name\x18\x02 \x01(\t\x12\x0c\n\x04path\x18\x03 \x01(\t\"h\n\x13RunResultWarningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.RunResultWarning\"J\n\x10RunResultFailure\x12\x15\n\rresource_type\x18\x01 \x01(\t\x12\x11\n\tnode_name\x18\x02 \x01(\t\x12\x0c\n\x04path\x18\x03 \x01(\t\"h\n\x13RunResultFailureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.RunResultFailure\"k\n\tStatsLine\x12\x30\n\x05stats\x18\x01 \x03(\x0b\x32!.proto_types.StatsLine.StatsEntry\x1a,\n\nStatsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\"Z\n\x0cStatsLineMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12$\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.proto_types.StatsLine\"\x1d\n\x0eRunResultError\x12\x0b\n\x03msg\x18\x01 \x01(\t\"d\n\x11RunResultErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.RunResultError\")\n\x17RunResultErrorNoMessage\x12\x0e\n\x06status\x18\x01 \x01(\t\"v\n\x1aRunResultErrorNoMessageMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.RunResultErrorNoMessage\"\x1f\n\x0fSQLCompiledPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"f\n\x12SQLCompiledPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.SQLCompiledPath\"-\n\x14\x43heckNodeTestFailure\x12\x15\n\rrelation_name\x18\x01 \x01(\t\"p\n\x17\x43heckNodeTestFailureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.CheckNodeTestFailure\"\"\n\x13\x46irstRunResultError\x12\x0b\n\x03msg\x18\x01 \x01(\t\"n\n\x16\x46irstRunResultErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.FirstRunResultError\"\'\n\x18\x41\x66terFirstRunResultError\x12\x0b\n\x03msg\x18\x01 \x01(\t\"x\n\x1b\x41\x66terFirstRunResultErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.AfterFirstRunResultError\"W\n\x0f\x45ndOfRunSummary\x12\x12\n\nnum_errors\x18\x01 \x01(\x05\x12\x14\n\x0cnum_warnings\x18\x02 \x01(\x05\x12\x1a\n\x12keyboard_interrupt\x18\x03 \x01(\x08\"f\n\x12\x45ndOfRunSummaryMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.EndOfRunSummary\"U\n\x13LogSkipBecauseError\x12\x0e\n\x06schema\x18\x01 \x01(\t\x12\x10\n\x08relation\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"n\n\x16LogSkipBecauseErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.LogSkipBecauseError\"\x14\n\x12\x45nsureGitInstalled\"l\n\x15\x45nsureGitInstalledMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.EnsureGitInstalled\"\x1a\n\x18\x44\x65psCreatingLocalSymlink\"x\n\x1b\x44\x65psCreatingLocalSymlinkMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.DepsCreatingLocalSymlink\"\x19\n\x17\x44\x65psSymlinkNotAvailable\"v\n\x1a\x44\x65psSymlinkNotAvailableMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.DepsSymlinkNotAvailable\"\x11\n\x0f\x44isableTracking\"f\n\x12\x44isableTrackingMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DisableTracking\"\x1e\n\x0cSendingEvent\x12\x0e\n\x06kwargs\x18\x01 \x01(\t\"`\n\x0fSendingEventMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.SendingEvent\"\x12\n\x10SendEventFailure\"h\n\x13SendEventFailureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.SendEventFailure\"\r\n\x0b\x46lushEvents\"^\n\x0e\x46lushEventsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.FlushEvents\"\x14\n\x12\x46lushEventsFailure\"l\n\x15\x46lushEventsFailureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.FlushEventsFailure\"-\n\x19TrackingInitializeFailure\x12\x10\n\x08\x65xc_info\x18\x01 \x01(\t\"z\n\x1cTrackingInitializeFailureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.TrackingInitializeFailure\"&\n\x17RunResultWarningMessage\x12\x0b\n\x03msg\x18\x01 \x01(\t\"v\n\x1aRunResultWarningMessageMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.RunResultWarningMessage\"\x1a\n\x0b\x44\x65\x62ugCmdOut\x12\x0b\n\x03msg\x18\x01 \x01(\t\"^\n\x0e\x44\x65\x62ugCmdOutMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.DebugCmdOut\"\x1d\n\x0e\x44\x65\x62ugCmdResult\x12\x0b\n\x03msg\x18\x01 \x01(\t\"d\n\x11\x44\x65\x62ugCmdResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.DebugCmdResult\"\x19\n\nListCmdOut\x12\x0b\n\x03msg\x18\x01 \x01(\t\"\\\n\rListCmdOutMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.ListCmdOut\"\x13\n\x04Note\x12\x0b\n\x03msg\x18\x01 \x01(\t\"P\n\x07NoteMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x1f\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x11.proto_types.Noteb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'types_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _EVENTINFO_EXTRAENTRY._options = None
@@ -204,676 +204,692 @@
   _ROLLBACKFAILED._serialized_end=8088
   _ROLLBACKFAILEDMSG._serialized_start=8090
   _ROLLBACKFAILEDMSG._serialized_end=8190
   _CONNECTIONCLOSED._serialized_start=8192
   _CONNECTIONCLOSED._serialized_end=8271
   _CONNECTIONCLOSEDMSG._serialized_start=8273
   _CONNECTIONCLOSEDMSG._serialized_end=8377
-  _CONNECTIONLEFTOPEN._serialized_start=8379
-  _CONNECTIONLEFTOPEN._serialized_end=8460
-  _CONNECTIONLEFTOPENMSG._serialized_start=8462
-  _CONNECTIONLEFTOPENMSG._serialized_end=8570
-  _ROLLBACK._serialized_start=8572
-  _ROLLBACK._serialized_end=8643
-  _ROLLBACKMSG._serialized_start=8645
-  _ROLLBACKMSG._serialized_end=8733
-  _CACHEMISS._serialized_start=8735
-  _CACHEMISS._serialized_end=8799
-  _CACHEMISSMSG._serialized_start=8801
-  _CACHEMISSMSG._serialized_end=8891
-  _LISTRELATIONS._serialized_start=8893
-  _LISTRELATIONS._serialized_end=8991
-  _LISTRELATIONSMSG._serialized_start=8993
-  _LISTRELATIONSMSG._serialized_end=9091
-  _CONNECTIONUSED._serialized_start=9093
-  _CONNECTIONUSED._serialized_end=9189
-  _CONNECTIONUSEDMSG._serialized_start=9191
-  _CONNECTIONUSEDMSG._serialized_end=9291
-  _SQLQUERY._serialized_start=9293
-  _SQLQUERY._serialized_end=9377
-  _SQLQUERYMSG._serialized_start=9379
-  _SQLQUERYMSG._serialized_end=9467
-  _SQLQUERYSTATUS._serialized_start=9469
-  _SQLQUERYSTATUS._serialized_end=9560
-  _SQLQUERYSTATUSMSG._serialized_start=9562
-  _SQLQUERYSTATUSMSG._serialized_end=9662
-  _SQLCOMMIT._serialized_start=9664
-  _SQLCOMMIT._serialized_end=9736
-  _SQLCOMMITMSG._serialized_start=9738
-  _SQLCOMMITMSG._serialized_end=9828
-  _COLTYPECHANGE._serialized_start=9830
-  _COLTYPECHANGE._serialized_end=9927
-  _COLTYPECHANGEMSG._serialized_start=9929
-  _COLTYPECHANGEMSG._serialized_end=10027
-  _SCHEMACREATION._serialized_start=10029
-  _SCHEMACREATION._serialized_end=10093
-  _SCHEMACREATIONMSG._serialized_start=10095
-  _SCHEMACREATIONMSG._serialized_end=10195
-  _SCHEMADROP._serialized_start=10197
-  _SCHEMADROP._serialized_end=10257
-  _SCHEMADROPMSG._serialized_start=10259
-  _SCHEMADROPMSG._serialized_end=10351
-  _CACHEACTION._serialized_start=10354
-  _CACHEACTION._serialized_end=10576
-  _CACHEACTIONMSG._serialized_start=10578
-  _CACHEACTIONMSG._serialized_end=10672
-  _CACHEDUMPGRAPH._serialized_start=10675
-  _CACHEDUMPGRAPH._serialized_end=10827
-  _CACHEDUMPGRAPH_DUMPENTRY._serialized_start=10784
-  _CACHEDUMPGRAPH_DUMPENTRY._serialized_end=10827
-  _CACHEDUMPGRAPHMSG._serialized_start=10829
-  _CACHEDUMPGRAPHMSG._serialized_end=10929
-  _ADAPTERIMPORTERROR._serialized_start=10931
-  _ADAPTERIMPORTERROR._serialized_end=10964
-  _ADAPTERIMPORTERRORMSG._serialized_start=10966
-  _ADAPTERIMPORTERRORMSG._serialized_end=11074
-  _PLUGINLOADERROR._serialized_start=11076
-  _PLUGINLOADERROR._serialized_end=11111
-  _PLUGINLOADERRORMSG._serialized_start=11113
-  _PLUGINLOADERRORMSG._serialized_end=11215
-  _NEWCONNECTIONOPENING._serialized_start=11217
-  _NEWCONNECTIONOPENING._serialized_end=11307
-  _NEWCONNECTIONOPENINGMSG._serialized_start=11309
-  _NEWCONNECTIONOPENINGMSG._serialized_end=11421
-  _CODEEXECUTION._serialized_start=11423
-  _CODEEXECUTION._serialized_end=11479
-  _CODEEXECUTIONMSG._serialized_start=11481
-  _CODEEXECUTIONMSG._serialized_end=11579
-  _CODEEXECUTIONSTATUS._serialized_start=11581
-  _CODEEXECUTIONSTATUS._serialized_end=11635
-  _CODEEXECUTIONSTATUSMSG._serialized_start=11637
-  _CODEEXECUTIONSTATUSMSG._serialized_end=11747
-  _CATALOGGENERATIONERROR._serialized_start=11749
-  _CATALOGGENERATIONERROR._serialized_end=11786
-  _CATALOGGENERATIONERRORMSG._serialized_start=11788
-  _CATALOGGENERATIONERRORMSG._serialized_end=11904
-  _WRITECATALOGFAILURE._serialized_start=11906
-  _WRITECATALOGFAILURE._serialized_end=11951
-  _WRITECATALOGFAILUREMSG._serialized_start=11953
-  _WRITECATALOGFAILUREMSG._serialized_end=12063
-  _CATALOGWRITTEN._serialized_start=12065
-  _CATALOGWRITTEN._serialized_end=12095
-  _CATALOGWRITTENMSG._serialized_start=12097
-  _CATALOGWRITTENMSG._serialized_end=12197
-  _CANNOTGENERATEDOCS._serialized_start=12199
-  _CANNOTGENERATEDOCS._serialized_end=12219
-  _CANNOTGENERATEDOCSMSG._serialized_start=12221
-  _CANNOTGENERATEDOCSMSG._serialized_end=12329
-  _BUILDINGCATALOG._serialized_start=12331
-  _BUILDINGCATALOG._serialized_end=12348
-  _BUILDINGCATALOGMSG._serialized_start=12350
-  _BUILDINGCATALOGMSG._serialized_end=12452
-  _DATABASEERRORRUNNINGHOOK._serialized_start=12454
-  _DATABASEERRORRUNNINGHOOK._serialized_end=12499
-  _DATABASEERRORRUNNINGHOOKMSG._serialized_start=12501
-  _DATABASEERRORRUNNINGHOOKMSG._serialized_end=12621
-  _HOOKSRUNNING._serialized_start=12623
-  _HOOKSRUNNING._serialized_end=12675
-  _HOOKSRUNNINGMSG._serialized_start=12677
-  _HOOKSRUNNINGMSG._serialized_end=12773
-  _FINISHEDRUNNINGSTATS._serialized_start=12775
-  _FINISHEDRUNNINGSTATS._serialized_end=12859
-  _FINISHEDRUNNINGSTATSMSG._serialized_start=12861
-  _FINISHEDRUNNINGSTATSMSG._serialized_end=12973
-  _CONSTRAINTNOTENFORCED._serialized_start=12975
-  _CONSTRAINTNOTENFORCED._serialized_end=13035
-  _CONSTRAINTNOTENFORCEDMSG._serialized_start=13037
-  _CONSTRAINTNOTENFORCEDMSG._serialized_end=13151
-  _CONSTRAINTNOTSUPPORTED._serialized_start=13153
-  _CONSTRAINTNOTSUPPORTED._serialized_end=13214
-  _CONSTRAINTNOTSUPPORTEDMSG._serialized_start=13216
-  _CONSTRAINTNOTSUPPORTEDMSG._serialized_end=13332
-  _INPUTFILEDIFFERROR._serialized_start=13334
-  _INPUTFILEDIFFERROR._serialized_end=13389
-  _INPUTFILEDIFFERRORMSG._serialized_start=13391
-  _INPUTFILEDIFFERRORMSG._serialized_end=13499
-  _INVALIDVALUEFORFIELD._serialized_start=13501
-  _INVALIDVALUEFORFIELD._serialized_end=13564
-  _INVALIDVALUEFORFIELDMSG._serialized_start=13566
-  _INVALIDVALUEFORFIELDMSG._serialized_end=13678
-  _VALIDATIONWARNING._serialized_start=13680
-  _VALIDATIONWARNING._serialized_end=13761
-  _VALIDATIONWARNINGMSG._serialized_start=13763
-  _VALIDATIONWARNINGMSG._serialized_end=13869
-  _PARSEPERFINFOPATH._serialized_start=13871
-  _PARSEPERFINFOPATH._serialized_end=13904
-  _PARSEPERFINFOPATHMSG._serialized_start=13906
-  _PARSEPERFINFOPATHMSG._serialized_end=14012
-  _GENERICTESTFILEPARSE._serialized_start=14014
-  _GENERICTESTFILEPARSE._serialized_end=14050
-  _GENERICTESTFILEPARSEMSG._serialized_start=14052
-  _GENERICTESTFILEPARSEMSG._serialized_end=14164
-  _MACROFILEPARSE._serialized_start=14166
-  _MACROFILEPARSE._serialized_end=14196
-  _MACROFILEPARSEMSG._serialized_start=14198
-  _MACROFILEPARSEMSG._serialized_end=14298
-  _PARTIALPARSINGERRORPROCESSINGFILE._serialized_start=14300
-  _PARTIALPARSINGERRORPROCESSINGFILE._serialized_end=14349
-  _PARTIALPARSINGERRORPROCESSINGFILEMSG._serialized_start=14352
-  _PARTIALPARSINGERRORPROCESSINGFILEMSG._serialized_end=14490
-  _PARTIALPARSINGERROR._serialized_start=14493
-  _PARTIALPARSINGERROR._serialized_end=14627
-  _PARTIALPARSINGERROR_EXCINFOENTRY._serialized_start=14581
-  _PARTIALPARSINGERROR_EXCINFOENTRY._serialized_end=14627
-  _PARTIALPARSINGERRORMSG._serialized_start=14629
-  _PARTIALPARSINGERRORMSG._serialized_end=14739
-  _PARTIALPARSINGSKIPPARSING._serialized_start=14741
-  _PARTIALPARSINGSKIPPARSING._serialized_end=14768
-  _PARTIALPARSINGSKIPPARSINGMSG._serialized_start=14770
-  _PARTIALPARSINGSKIPPARSINGMSG._serialized_end=14892
-  _UNABLETOPARTIALPARSE._serialized_start=14894
-  _UNABLETOPARTIALPARSE._serialized_end=14932
-  _UNABLETOPARTIALPARSEMSG._serialized_start=14934
-  _UNABLETOPARTIALPARSEMSG._serialized_end=15046
-  _STATECHECKVARSHASH._serialized_start=15048
-  _STATECHECKVARSHASH._serialized_end=15150
-  _STATECHECKVARSHASHMSG._serialized_start=15152
-  _STATECHECKVARSHASHMSG._serialized_end=15260
-  _PARTIALPARSINGNOTENABLED._serialized_start=15262
-  _PARTIALPARSINGNOTENABLED._serialized_end=15288
-  _PARTIALPARSINGNOTENABLEDMSG._serialized_start=15290
-  _PARTIALPARSINGNOTENABLEDMSG._serialized_end=15410
-  _PARSEDFILELOADFAILED._serialized_start=15412
-  _PARSEDFILELOADFAILED._serialized_end=15479
-  _PARSEDFILELOADFAILEDMSG._serialized_start=15481
-  _PARSEDFILELOADFAILEDMSG._serialized_end=15593
-  _PARTIALPARSINGENABLED._serialized_start=15595
-  _PARTIALPARSINGENABLED._serialized_end=15667
-  _PARTIALPARSINGENABLEDMSG._serialized_start=15669
-  _PARTIALPARSINGENABLEDMSG._serialized_end=15783
-  _PARTIALPARSINGFILE._serialized_start=15785
-  _PARTIALPARSINGFILE._serialized_end=15841
-  _PARTIALPARSINGFILEMSG._serialized_start=15843
-  _PARTIALPARSINGFILEMSG._serialized_end=15951
-  _INVALIDDISABLEDTARGETINTESTNODE._serialized_start=15954
-  _INVALIDDISABLEDTARGETINTESTNODE._serialized_end=16129
-  _INVALIDDISABLEDTARGETINTESTNODEMSG._serialized_start=16132
-  _INVALIDDISABLEDTARGETINTESTNODEMSG._serialized_end=16266
-  _UNUSEDRESOURCECONFIGPATH._serialized_start=16268
-  _UNUSEDRESOURCECONFIGPATH._serialized_end=16323
-  _UNUSEDRESOURCECONFIGPATHMSG._serialized_start=16325
-  _UNUSEDRESOURCECONFIGPATHMSG._serialized_end=16445
-  _SEEDINCREASED._serialized_start=16447
-  _SEEDINCREASED._serialized_end=16498
-  _SEEDINCREASEDMSG._serialized_start=16500
-  _SEEDINCREASEDMSG._serialized_end=16598
-  _SEEDEXCEEDSLIMITSAMEPATH._serialized_start=16600
-  _SEEDEXCEEDSLIMITSAMEPATH._serialized_end=16662
-  _SEEDEXCEEDSLIMITSAMEPATHMSG._serialized_start=16664
-  _SEEDEXCEEDSLIMITSAMEPATHMSG._serialized_end=16784
-  _SEEDEXCEEDSLIMITANDPATHCHANGED._serialized_start=16786
-  _SEEDEXCEEDSLIMITANDPATHCHANGED._serialized_end=16854
-  _SEEDEXCEEDSLIMITANDPATHCHANGEDMSG._serialized_start=16857
-  _SEEDEXCEEDSLIMITANDPATHCHANGEDMSG._serialized_end=16989
-  _SEEDEXCEEDSLIMITCHECKSUMCHANGED._serialized_start=16991
-  _SEEDEXCEEDSLIMITCHECKSUMCHANGED._serialized_end=17083
-  _SEEDEXCEEDSLIMITCHECKSUMCHANGEDMSG._serialized_start=17086
-  _SEEDEXCEEDSLIMITCHECKSUMCHANGEDMSG._serialized_end=17220
-  _UNUSEDTABLES._serialized_start=17222
-  _UNUSEDTABLES._serialized_end=17259
-  _UNUSEDTABLESMSG._serialized_start=17261
-  _UNUSEDTABLESMSG._serialized_end=17357
-  _WRONGRESOURCESCHEMAFILE._serialized_start=17360
-  _WRONGRESOURCESCHEMAFILE._serialized_end=17495
-  _WRONGRESOURCESCHEMAFILEMSG._serialized_start=17497
-  _WRONGRESOURCESCHEMAFILEMSG._serialized_end=17615
-  _NONODEFORYAMLKEY._serialized_start=17617
-  _NONODEFORYAMLKEY._serialized_end=17692
-  _NONODEFORYAMLKEYMSG._serialized_start=17694
-  _NONODEFORYAMLKEYMSG._serialized_end=17798
-  _MACRONOTFOUNDFORPATCH._serialized_start=17800
-  _MACRONOTFOUNDFORPATCH._serialized_end=17843
-  _MACRONOTFOUNDFORPATCHMSG._serialized_start=17845
-  _MACRONOTFOUNDFORPATCHMSG._serialized_end=17959
-  _NODENOTFOUNDORDISABLED._serialized_start=17962
-  _NODENOTFOUNDORDISABLED._serialized_end=18146
-  _NODENOTFOUNDORDISABLEDMSG._serialized_start=18148
-  _NODENOTFOUNDORDISABLEDMSG._serialized_end=18264
-  _JINJALOGWARNING._serialized_start=18266
-  _JINJALOGWARNING._serialized_end=18338
-  _JINJALOGWARNINGMSG._serialized_start=18340
-  _JINJALOGWARNINGMSG._serialized_end=18442
-  _JINJALOGINFO._serialized_start=18444
-  _JINJALOGINFO._serialized_end=18513
-  _JINJALOGINFOMSG._serialized_start=18515
-  _JINJALOGINFOMSG._serialized_end=18611
-  _JINJALOGDEBUG._serialized_start=18613
-  _JINJALOGDEBUG._serialized_end=18683
-  _JINJALOGDEBUGMSG._serialized_start=18685
-  _JINJALOGDEBUGMSG._serialized_end=18783
-  _UNPINNEDREFNEWVERSIONAVAILABLE._serialized_start=18786
-  _UNPINNEDREFNEWVERSIONAVAILABLE._serialized_end=18960
-  _UNPINNEDREFNEWVERSIONAVAILABLEMSG._serialized_start=18963
-  _UNPINNEDREFNEWVERSIONAVAILABLEMSG._serialized_end=19095
-  _GITSPARSECHECKOUTSUBDIRECTORY._serialized_start=19097
-  _GITSPARSECHECKOUTSUBDIRECTORY._serialized_end=19144
-  _GITSPARSECHECKOUTSUBDIRECTORYMSG._serialized_start=19147
-  _GITSPARSECHECKOUTSUBDIRECTORYMSG._serialized_end=19277
-  _GITPROGRESSCHECKOUTREVISION._serialized_start=19279
-  _GITPROGRESSCHECKOUTREVISION._serialized_end=19326
-  _GITPROGRESSCHECKOUTREVISIONMSG._serialized_start=19328
-  _GITPROGRESSCHECKOUTREVISIONMSG._serialized_end=19454
-  _GITPROGRESSUPDATINGEXISTINGDEPENDENCY._serialized_start=19456
-  _GITPROGRESSUPDATINGEXISTINGDEPENDENCY._serialized_end=19508
-  _GITPROGRESSUPDATINGEXISTINGDEPENDENCYMSG._serialized_start=19511
-  _GITPROGRESSUPDATINGEXISTINGDEPENDENCYMSG._serialized_end=19657
-  _GITPROGRESSPULLINGNEWDEPENDENCY._serialized_start=19659
-  _GITPROGRESSPULLINGNEWDEPENDENCY._serialized_end=19705
-  _GITPROGRESSPULLINGNEWDEPENDENCYMSG._serialized_start=19708
-  _GITPROGRESSPULLINGNEWDEPENDENCYMSG._serialized_end=19842
-  _GITNOTHINGTODO._serialized_start=19844
-  _GITNOTHINGTODO._serialized_end=19873
-  _GITNOTHINGTODOMSG._serialized_start=19875
-  _GITNOTHINGTODOMSG._serialized_end=19975
-  _GITPROGRESSUPDATEDCHECKOUTRANGE._serialized_start=19977
-  _GITPROGRESSUPDATEDCHECKOUTRANGE._serialized_end=20046
-  _GITPROGRESSUPDATEDCHECKOUTRANGEMSG._serialized_start=20049
-  _GITPROGRESSUPDATEDCHECKOUTRANGEMSG._serialized_end=20183
-  _GITPROGRESSCHECKEDOUTAT._serialized_start=20185
-  _GITPROGRESSCHECKEDOUTAT._serialized_end=20227
-  _GITPROGRESSCHECKEDOUTATMSG._serialized_start=20229
-  _GITPROGRESSCHECKEDOUTATMSG._serialized_end=20347
-  _REGISTRYPROGRESSGETREQUEST._serialized_start=20349
-  _REGISTRYPROGRESSGETREQUEST._serialized_end=20390
-  _REGISTRYPROGRESSGETREQUESTMSG._serialized_start=20392
-  _REGISTRYPROGRESSGETREQUESTMSG._serialized_end=20516
-  _REGISTRYPROGRESSGETRESPONSE._serialized_start=20518
-  _REGISTRYPROGRESSGETRESPONSE._serialized_end=20579
-  _REGISTRYPROGRESSGETRESPONSEMSG._serialized_start=20581
-  _REGISTRYPROGRESSGETRESPONSEMSG._serialized_end=20707
-  _SELECTORREPORTINVALIDSELECTOR._serialized_start=20709
-  _SELECTORREPORTINVALIDSELECTOR._serialized_end=20804
-  _SELECTORREPORTINVALIDSELECTORMSG._serialized_start=20807
-  _SELECTORREPORTINVALIDSELECTORMSG._serialized_end=20937
-  _DEPSNOPACKAGESFOUND._serialized_start=20939
-  _DEPSNOPACKAGESFOUND._serialized_end=20960
-  _DEPSNOPACKAGESFOUNDMSG._serialized_start=20962
-  _DEPSNOPACKAGESFOUNDMSG._serialized_end=21072
-  _DEPSSTARTPACKAGEINSTALL._serialized_start=21074
-  _DEPSSTARTPACKAGEINSTALL._serialized_end=21121
-  _DEPSSTARTPACKAGEINSTALLMSG._serialized_start=21123
-  _DEPSSTARTPACKAGEINSTALLMSG._serialized_end=21241
-  _DEPSINSTALLINFO._serialized_start=21243
-  _DEPSINSTALLINFO._serialized_end=21282
-  _DEPSINSTALLINFOMSG._serialized_start=21284
-  _DEPSINSTALLINFOMSG._serialized_end=21386
-  _DEPSUPDATEAVAILABLE._serialized_start=21388
-  _DEPSUPDATEAVAILABLE._serialized_end=21433
-  _DEPSUPDATEAVAILABLEMSG._serialized_start=21435
-  _DEPSUPDATEAVAILABLEMSG._serialized_end=21545
-  _DEPSUPTODATE._serialized_start=21547
-  _DEPSUPTODATE._serialized_end=21561
-  _DEPSUPTODATEMSG._serialized_start=21563
-  _DEPSUPTODATEMSG._serialized_end=21659
-  _DEPSLISTSUBDIRECTORY._serialized_start=21661
-  _DEPSLISTSUBDIRECTORY._serialized_end=21705
-  _DEPSLISTSUBDIRECTORYMSG._serialized_start=21707
-  _DEPSLISTSUBDIRECTORYMSG._serialized_end=21819
-  _DEPSNOTIFYUPDATESAVAILABLE._serialized_start=21821
-  _DEPSNOTIFYUPDATESAVAILABLE._serialized_end=21867
-  _DEPSNOTIFYUPDATESAVAILABLEMSG._serialized_start=21869
-  _DEPSNOTIFYUPDATESAVAILABLEMSG._serialized_end=21993
-  _RETRYEXTERNALCALL._serialized_start=21995
-  _RETRYEXTERNALCALL._serialized_end=22044
-  _RETRYEXTERNALCALLMSG._serialized_start=22046
-  _RETRYEXTERNALCALLMSG._serialized_end=22152
-  _RECORDRETRYEXCEPTION._serialized_start=22154
-  _RECORDRETRYEXCEPTION._serialized_end=22189
-  _RECORDRETRYEXCEPTIONMSG._serialized_start=22191
-  _RECORDRETRYEXCEPTIONMSG._serialized_end=22303
-  _REGISTRYINDEXPROGRESSGETREQUEST._serialized_start=22305
-  _REGISTRYINDEXPROGRESSGETREQUEST._serialized_end=22351
-  _REGISTRYINDEXPROGRESSGETREQUESTMSG._serialized_start=22354
-  _REGISTRYINDEXPROGRESSGETREQUESTMSG._serialized_end=22488
-  _REGISTRYINDEXPROGRESSGETRESPONSE._serialized_start=22490
-  _REGISTRYINDEXPROGRESSGETRESPONSE._serialized_end=22556
-  _REGISTRYINDEXPROGRESSGETRESPONSEMSG._serialized_start=22559
-  _REGISTRYINDEXPROGRESSGETRESPONSEMSG._serialized_end=22695
-  _REGISTRYRESPONSEUNEXPECTEDTYPE._serialized_start=22697
-  _REGISTRYRESPONSEUNEXPECTEDTYPE._serialized_end=22747
-  _REGISTRYRESPONSEUNEXPECTEDTYPEMSG._serialized_start=22750
-  _REGISTRYRESPONSEUNEXPECTEDTYPEMSG._serialized_end=22882
-  _REGISTRYRESPONSEMISSINGTOPKEYS._serialized_start=22884
-  _REGISTRYRESPONSEMISSINGTOPKEYS._serialized_end=22934
-  _REGISTRYRESPONSEMISSINGTOPKEYSMSG._serialized_start=22937
-  _REGISTRYRESPONSEMISSINGTOPKEYSMSG._serialized_end=23069
-  _REGISTRYRESPONSEMISSINGNESTEDKEYS._serialized_start=23071
-  _REGISTRYRESPONSEMISSINGNESTEDKEYS._serialized_end=23124
-  _REGISTRYRESPONSEMISSINGNESTEDKEYSMSG._serialized_start=23127
-  _REGISTRYRESPONSEMISSINGNESTEDKEYSMSG._serialized_end=23265
-  _REGISTRYRESPONSEEXTRANESTEDKEYS._serialized_start=23267
-  _REGISTRYRESPONSEEXTRANESTEDKEYS._serialized_end=23318
-  _REGISTRYRESPONSEEXTRANESTEDKEYSMSG._serialized_start=23321
-  _REGISTRYRESPONSEEXTRANESTEDKEYSMSG._serialized_end=23455
-  _DEPSSETDOWNLOADDIRECTORY._serialized_start=23457
-  _DEPSSETDOWNLOADDIRECTORY._serialized_end=23497
-  _DEPSSETDOWNLOADDIRECTORYMSG._serialized_start=23499
-  _DEPSSETDOWNLOADDIRECTORYMSG._serialized_end=23619
-  _DEPSUNPINNED._serialized_start=23621
-  _DEPSUNPINNED._serialized_end=23666
-  _DEPSUNPINNEDMSG._serialized_start=23668
-  _DEPSUNPINNEDMSG._serialized_end=23764
-  _NONODESFORSELECTIONCRITERIA._serialized_start=23766
-  _NONODESFORSELECTIONCRITERIA._serialized_end=23813
-  _NONODESFORSELECTIONCRITERIAMSG._serialized_start=23815
-  _NONODESFORSELECTIONCRITERIAMSG._serialized_end=23941
-  _RUNNINGOPERATIONCAUGHTERROR._serialized_start=23943
-  _RUNNINGOPERATIONCAUGHTERROR._serialized_end=23985
-  _RUNNINGOPERATIONCAUGHTERRORMSG._serialized_start=23987
-  _RUNNINGOPERATIONCAUGHTERRORMSG._serialized_end=24113
-  _COMPILECOMPLETE._serialized_start=24115
-  _COMPILECOMPLETE._serialized_end=24132
-  _COMPILECOMPLETEMSG._serialized_start=24134
-  _COMPILECOMPLETEMSG._serialized_end=24236
-  _FRESHNESSCHECKCOMPLETE._serialized_start=24238
-  _FRESHNESSCHECKCOMPLETE._serialized_end=24262
-  _FRESHNESSCHECKCOMPLETEMSG._serialized_start=24264
-  _FRESHNESSCHECKCOMPLETEMSG._serialized_end=24380
-  _SEEDHEADER._serialized_start=24382
-  _SEEDHEADER._serialized_end=24410
-  _SEEDHEADERMSG._serialized_start=24412
-  _SEEDHEADERMSG._serialized_end=24504
-  _SQLRUNNEREXCEPTION._serialized_start=24506
-  _SQLRUNNEREXCEPTION._serialized_end=24557
-  _SQLRUNNEREXCEPTIONMSG._serialized_start=24559
-  _SQLRUNNEREXCEPTIONMSG._serialized_end=24667
-  _LOGTESTRESULT._serialized_start=24670
-  _LOGTESTRESULT._serialized_end=24838
-  _LOGTESTRESULTMSG._serialized_start=24840
-  _LOGTESTRESULTMSG._serialized_end=24938
-  _LOGSTARTLINE._serialized_start=24940
-  _LOGSTARTLINE._serialized_end=25047
-  _LOGSTARTLINEMSG._serialized_start=25049
-  _LOGSTARTLINEMSG._serialized_end=25145
-  _LOGMODELRESULT._serialized_start=25148
-  _LOGMODELRESULT._serialized_end=25297
-  _LOGMODELRESULTMSG._serialized_start=25299
-  _LOGMODELRESULTMSG._serialized_end=25399
-  _LOGSNAPSHOTRESULT._serialized_start=25402
-  _LOGSNAPSHOTRESULT._serialized_end=25652
-  _LOGSNAPSHOTRESULT_CFGENTRY._serialized_start=25610
-  _LOGSNAPSHOTRESULT_CFGENTRY._serialized_end=25652
-  _LOGSNAPSHOTRESULTMSG._serialized_start=25654
-  _LOGSNAPSHOTRESULTMSG._serialized_end=25760
-  _LOGSEEDRESULT._serialized_start=25763
-  _LOGSEEDRESULT._serialized_end=25948
-  _LOGSEEDRESULTMSG._serialized_start=25950
-  _LOGSEEDRESULTMSG._serialized_end=26048
-  _LOGFRESHNESSRESULT._serialized_start=26051
-  _LOGFRESHNESSRESULT._serialized_end=26224
-  _LOGFRESHNESSRESULTMSG._serialized_start=26226
-  _LOGFRESHNESSRESULTMSG._serialized_end=26334
-  _LOGCANCELLINE._serialized_start=26336
-  _LOGCANCELLINE._serialized_end=26370
-  _LOGCANCELLINEMSG._serialized_start=26372
-  _LOGCANCELLINEMSG._serialized_end=26470
-  _DEFAULTSELECTOR._serialized_start=26472
-  _DEFAULTSELECTOR._serialized_end=26503
-  _DEFAULTSELECTORMSG._serialized_start=26505
-  _DEFAULTSELECTORMSG._serialized_end=26607
-  _NODESTART._serialized_start=26609
-  _NODESTART._serialized_end=26662
-  _NODESTARTMSG._serialized_start=26664
-  _NODESTARTMSG._serialized_end=26754
-  _NODEFINISHED._serialized_start=26756
-  _NODEFINISHED._serialized_end=26859
-  _NODEFINISHEDMSG._serialized_start=26861
-  _NODEFINISHEDMSG._serialized_end=26957
-  _QUERYCANCELATIONUNSUPPORTED._serialized_start=26959
-  _QUERYCANCELATIONUNSUPPORTED._serialized_end=27002
-  _QUERYCANCELATIONUNSUPPORTEDMSG._serialized_start=27004
-  _QUERYCANCELATIONUNSUPPORTEDMSG._serialized_end=27130
-  _CONCURRENCYLINE._serialized_start=27132
-  _CONCURRENCYLINE._serialized_end=27211
-  _CONCURRENCYLINEMSG._serialized_start=27213
-  _CONCURRENCYLINEMSG._serialized_end=27315
-  _WRITINGINJECTEDSQLFORNODE._serialized_start=27317
-  _WRITINGINJECTEDSQLFORNODE._serialized_end=27386
-  _WRITINGINJECTEDSQLFORNODEMSG._serialized_start=27388
-  _WRITINGINJECTEDSQLFORNODEMSG._serialized_end=27510
-  _NODECOMPILING._serialized_start=27512
-  _NODECOMPILING._serialized_end=27569
-  _NODECOMPILINGMSG._serialized_start=27571
-  _NODECOMPILINGMSG._serialized_end=27669
-  _NODEEXECUTING._serialized_start=27671
-  _NODEEXECUTING._serialized_end=27728
-  _NODEEXECUTINGMSG._serialized_start=27730
-  _NODEEXECUTINGMSG._serialized_end=27828
-  _LOGHOOKSTARTLINE._serialized_start=27830
-  _LOGHOOKSTARTLINE._serialized_end=27939
-  _LOGHOOKSTARTLINEMSG._serialized_start=27941
-  _LOGHOOKSTARTLINEMSG._serialized_end=28045
-  _LOGHOOKENDLINE._serialized_start=28048
-  _LOGHOOKENDLINE._serialized_end=28195
-  _LOGHOOKENDLINEMSG._serialized_start=28197
-  _LOGHOOKENDLINEMSG._serialized_end=28297
-  _SKIPPINGDETAILS._serialized_start=28300
-  _SKIPPINGDETAILS._serialized_end=28447
-  _SKIPPINGDETAILSMSG._serialized_start=28449
-  _SKIPPINGDETAILSMSG._serialized_end=28551
-  _NOTHINGTODO._serialized_start=28553
-  _NOTHINGTODO._serialized_end=28566
-  _NOTHINGTODOMSG._serialized_start=28568
-  _NOTHINGTODOMSG._serialized_end=28662
-  _RUNNINGOPERATIONUNCAUGHTERROR._serialized_start=28664
-  _RUNNINGOPERATIONUNCAUGHTERROR._serialized_end=28708
-  _RUNNINGOPERATIONUNCAUGHTERRORMSG._serialized_start=28711
-  _RUNNINGOPERATIONUNCAUGHTERRORMSG._serialized_end=28841
-  _ENDRUNRESULT._serialized_start=28844
-  _ENDRUNRESULT._serialized_end=28991
-  _ENDRUNRESULTMSG._serialized_start=28993
-  _ENDRUNRESULTMSG._serialized_end=29089
-  _NONODESSELECTED._serialized_start=29091
-  _NONODESSELECTED._serialized_end=29108
-  _NONODESSELECTEDMSG._serialized_start=29110
-  _NONODESSELECTEDMSG._serialized_end=29212
-  _COMMANDCOMPLETED._serialized_start=29214
-  _COMMANDCOMPLETED._serialized_end=29333
-  _COMMANDCOMPLETEDMSG._serialized_start=29335
-  _COMMANDCOMPLETEDMSG._serialized_end=29439
-  _SHOWNODE._serialized_start=29441
-  _SHOWNODE._serialized_end=29548
-  _SHOWNODEMSG._serialized_start=29550
-  _SHOWNODEMSG._serialized_end=29638
-  _COMPILEDNODE._serialized_start=29640
-  _COMPILEDNODE._serialized_end=29752
-  _COMPILEDNODEMSG._serialized_start=29754
-  _COMPILEDNODEMSG._serialized_end=29850
-  _CATCHABLEEXCEPTIONONRUN._serialized_start=29852
-  _CATCHABLEEXCEPTIONONRUN._serialized_end=29950
-  _CATCHABLEEXCEPTIONONRUNMSG._serialized_start=29952
-  _CATCHABLEEXCEPTIONONRUNMSG._serialized_end=30070
-  _INTERNALERRORONRUN._serialized_start=30072
-  _INTERNALERRORONRUN._serialized_end=30125
-  _INTERNALERRORONRUNMSG._serialized_start=30127
-  _INTERNALERRORONRUNMSG._serialized_end=30235
-  _GENERICEXCEPTIONONRUN._serialized_start=30237
-  _GENERICEXCEPTIONONRUN._serialized_end=30312
-  _GENERICEXCEPTIONONRUNMSG._serialized_start=30314
-  _GENERICEXCEPTIONONRUNMSG._serialized_end=30428
-  _NODECONNECTIONRELEASEERROR._serialized_start=30430
-  _NODECONNECTIONRELEASEERROR._serialized_end=30508
-  _NODECONNECTIONRELEASEERRORMSG._serialized_start=30510
-  _NODECONNECTIONRELEASEERRORMSG._serialized_end=30634
-  _FOUNDSTATS._serialized_start=30636
-  _FOUNDSTATS._serialized_end=30667
-  _FOUNDSTATSMSG._serialized_start=30669
-  _FOUNDSTATSMSG._serialized_end=30761
-  _MAINKEYBOARDINTERRUPT._serialized_start=30763
-  _MAINKEYBOARDINTERRUPT._serialized_end=30786
-  _MAINKEYBOARDINTERRUPTMSG._serialized_start=30788
-  _MAINKEYBOARDINTERRUPTMSG._serialized_end=30902
-  _MAINENCOUNTEREDERROR._serialized_start=30904
-  _MAINENCOUNTEREDERROR._serialized_end=30939
-  _MAINENCOUNTEREDERRORMSG._serialized_start=30941
-  _MAINENCOUNTEREDERRORMSG._serialized_end=31053
-  _MAINSTACKTRACE._serialized_start=31055
-  _MAINSTACKTRACE._serialized_end=31092
-  _MAINSTACKTRACEMSG._serialized_start=31094
-  _MAINSTACKTRACEMSG._serialized_end=31194
-  _SYSTEMCOULDNOTWRITE._serialized_start=31196
-  _SYSTEMCOULDNOTWRITE._serialized_end=31260
-  _SYSTEMCOULDNOTWRITEMSG._serialized_start=31262
-  _SYSTEMCOULDNOTWRITEMSG._serialized_end=31372
-  _SYSTEMEXECUTINGCMD._serialized_start=31374
-  _SYSTEMEXECUTINGCMD._serialized_end=31407
-  _SYSTEMEXECUTINGCMDMSG._serialized_start=31409
-  _SYSTEMEXECUTINGCMDMSG._serialized_end=31517
-  _SYSTEMSTDOUT._serialized_start=31519
-  _SYSTEMSTDOUT._serialized_end=31547
-  _SYSTEMSTDOUTMSG._serialized_start=31549
-  _SYSTEMSTDOUTMSG._serialized_end=31645
-  _SYSTEMSTDERR._serialized_start=31647
-  _SYSTEMSTDERR._serialized_end=31675
-  _SYSTEMSTDERRMSG._serialized_start=31677
-  _SYSTEMSTDERRMSG._serialized_end=31773
-  _SYSTEMREPORTRETURNCODE._serialized_start=31775
-  _SYSTEMREPORTRETURNCODE._serialized_end=31819
-  _SYSTEMREPORTRETURNCODEMSG._serialized_start=31821
-  _SYSTEMREPORTRETURNCODEMSG._serialized_end=31937
-  _TIMINGINFOCOLLECTED._serialized_start=31939
-  _TIMINGINFOCOLLECTED._serialized_end=32051
-  _TIMINGINFOCOLLECTEDMSG._serialized_start=32053
-  _TIMINGINFOCOLLECTEDMSG._serialized_end=32163
-  _LOGDEBUGSTACKTRACE._serialized_start=32165
-  _LOGDEBUGSTACKTRACE._serialized_end=32203
-  _LOGDEBUGSTACKTRACEMSG._serialized_start=32205
-  _LOGDEBUGSTACKTRACEMSG._serialized_end=32313
-  _CHECKCLEANPATH._serialized_start=32315
-  _CHECKCLEANPATH._serialized_end=32345
-  _CHECKCLEANPATHMSG._serialized_start=32347
-  _CHECKCLEANPATHMSG._serialized_end=32447
-  _CONFIRMCLEANPATH._serialized_start=32449
-  _CONFIRMCLEANPATH._serialized_end=32481
-  _CONFIRMCLEANPATHMSG._serialized_start=32483
-  _CONFIRMCLEANPATHMSG._serialized_end=32587
-  _PROTECTEDCLEANPATH._serialized_start=32589
-  _PROTECTEDCLEANPATH._serialized_end=32623
-  _PROTECTEDCLEANPATHMSG._serialized_start=32625
-  _PROTECTEDCLEANPATHMSG._serialized_end=32733
-  _FINISHEDCLEANPATHS._serialized_start=32735
-  _FINISHEDCLEANPATHS._serialized_end=32755
-  _FINISHEDCLEANPATHSMSG._serialized_start=32757
-  _FINISHEDCLEANPATHSMSG._serialized_end=32865
-  _OPENCOMMAND._serialized_start=32867
-  _OPENCOMMAND._serialized_end=32920
-  _OPENCOMMANDMSG._serialized_start=32922
-  _OPENCOMMANDMSG._serialized_end=33016
-  _FORMATTING._serialized_start=33018
-  _FORMATTING._serialized_end=33043
-  _FORMATTINGMSG._serialized_start=33045
-  _FORMATTINGMSG._serialized_end=33137
-  _SERVINGDOCSPORT._serialized_start=33139
-  _SERVINGDOCSPORT._serialized_end=33187
-  _SERVINGDOCSPORTMSG._serialized_start=33189
-  _SERVINGDOCSPORTMSG._serialized_end=33291
-  _SERVINGDOCSACCESSINFO._serialized_start=33293
-  _SERVINGDOCSACCESSINFO._serialized_end=33330
-  _SERVINGDOCSACCESSINFOMSG._serialized_start=33332
-  _SERVINGDOCSACCESSINFOMSG._serialized_end=33446
-  _SERVINGDOCSEXITINFO._serialized_start=33448
-  _SERVINGDOCSEXITINFO._serialized_end=33469
-  _SERVINGDOCSEXITINFOMSG._serialized_start=33471
-  _SERVINGDOCSEXITINFOMSG._serialized_end=33581
-  _RUNRESULTWARNING._serialized_start=33583
-  _RUNRESULTWARNING._serialized_end=33657
-  _RUNRESULTWARNINGMSG._serialized_start=33659
-  _RUNRESULTWARNINGMSG._serialized_end=33763
-  _RUNRESULTFAILURE._serialized_start=33765
-  _RUNRESULTFAILURE._serialized_end=33839
-  _RUNRESULTFAILUREMSG._serialized_start=33841
-  _RUNRESULTFAILUREMSG._serialized_end=33945
-  _STATSLINE._serialized_start=33947
-  _STATSLINE._serialized_end=34054
-  _STATSLINE_STATSENTRY._serialized_start=34010
-  _STATSLINE_STATSENTRY._serialized_end=34054
-  _STATSLINEMSG._serialized_start=34056
-  _STATSLINEMSG._serialized_end=34146
-  _RUNRESULTERROR._serialized_start=34148
-  _RUNRESULTERROR._serialized_end=34177
-  _RUNRESULTERRORMSG._serialized_start=34179
-  _RUNRESULTERRORMSG._serialized_end=34279
-  _RUNRESULTERRORNOMESSAGE._serialized_start=34281
-  _RUNRESULTERRORNOMESSAGE._serialized_end=34322
-  _RUNRESULTERRORNOMESSAGEMSG._serialized_start=34324
-  _RUNRESULTERRORNOMESSAGEMSG._serialized_end=34442
-  _SQLCOMPILEDPATH._serialized_start=34444
-  _SQLCOMPILEDPATH._serialized_end=34475
-  _SQLCOMPILEDPATHMSG._serialized_start=34477
-  _SQLCOMPILEDPATHMSG._serialized_end=34579
-  _CHECKNODETESTFAILURE._serialized_start=34581
-  _CHECKNODETESTFAILURE._serialized_end=34626
-  _CHECKNODETESTFAILUREMSG._serialized_start=34628
-  _CHECKNODETESTFAILUREMSG._serialized_end=34740
-  _FIRSTRUNRESULTERROR._serialized_start=34742
-  _FIRSTRUNRESULTERROR._serialized_end=34776
-  _FIRSTRUNRESULTERRORMSG._serialized_start=34778
-  _FIRSTRUNRESULTERRORMSG._serialized_end=34888
-  _AFTERFIRSTRUNRESULTERROR._serialized_start=34890
-  _AFTERFIRSTRUNRESULTERROR._serialized_end=34929
-  _AFTERFIRSTRUNRESULTERRORMSG._serialized_start=34931
-  _AFTERFIRSTRUNRESULTERRORMSG._serialized_end=35051
-  _ENDOFRUNSUMMARY._serialized_start=35053
-  _ENDOFRUNSUMMARY._serialized_end=35140
-  _ENDOFRUNSUMMARYMSG._serialized_start=35142
-  _ENDOFRUNSUMMARYMSG._serialized_end=35244
-  _LOGSKIPBECAUSEERROR._serialized_start=35246
-  _LOGSKIPBECAUSEERROR._serialized_end=35331
-  _LOGSKIPBECAUSEERRORMSG._serialized_start=35333
-  _LOGSKIPBECAUSEERRORMSG._serialized_end=35443
-  _ENSUREGITINSTALLED._serialized_start=35445
-  _ENSUREGITINSTALLED._serialized_end=35465
-  _ENSUREGITINSTALLEDMSG._serialized_start=35467
-  _ENSUREGITINSTALLEDMSG._serialized_end=35575
-  _DEPSCREATINGLOCALSYMLINK._serialized_start=35577
-  _DEPSCREATINGLOCALSYMLINK._serialized_end=35603
-  _DEPSCREATINGLOCALSYMLINKMSG._serialized_start=35605
-  _DEPSCREATINGLOCALSYMLINKMSG._serialized_end=35725
-  _DEPSSYMLINKNOTAVAILABLE._serialized_start=35727
-  _DEPSSYMLINKNOTAVAILABLE._serialized_end=35752
-  _DEPSSYMLINKNOTAVAILABLEMSG._serialized_start=35754
-  _DEPSSYMLINKNOTAVAILABLEMSG._serialized_end=35872
-  _DISABLETRACKING._serialized_start=35874
-  _DISABLETRACKING._serialized_end=35891
-  _DISABLETRACKINGMSG._serialized_start=35893
-  _DISABLETRACKINGMSG._serialized_end=35995
-  _SENDINGEVENT._serialized_start=35997
-  _SENDINGEVENT._serialized_end=36027
-  _SENDINGEVENTMSG._serialized_start=36029
-  _SENDINGEVENTMSG._serialized_end=36125
-  _SENDEVENTFAILURE._serialized_start=36127
-  _SENDEVENTFAILURE._serialized_end=36145
-  _SENDEVENTFAILUREMSG._serialized_start=36147
-  _SENDEVENTFAILUREMSG._serialized_end=36251
-  _FLUSHEVENTS._serialized_start=36253
-  _FLUSHEVENTS._serialized_end=36266
-  _FLUSHEVENTSMSG._serialized_start=36268
-  _FLUSHEVENTSMSG._serialized_end=36362
-  _FLUSHEVENTSFAILURE._serialized_start=36364
-  _FLUSHEVENTSFAILURE._serialized_end=36384
-  _FLUSHEVENTSFAILUREMSG._serialized_start=36386
-  _FLUSHEVENTSFAILUREMSG._serialized_end=36494
-  _TRACKINGINITIALIZEFAILURE._serialized_start=36496
-  _TRACKINGINITIALIZEFAILURE._serialized_end=36541
-  _TRACKINGINITIALIZEFAILUREMSG._serialized_start=36543
-  _TRACKINGINITIALIZEFAILUREMSG._serialized_end=36665
-  _RUNRESULTWARNINGMESSAGE._serialized_start=36667
-  _RUNRESULTWARNINGMESSAGE._serialized_end=36705
-  _RUNRESULTWARNINGMESSAGEMSG._serialized_start=36707
-  _RUNRESULTWARNINGMESSAGEMSG._serialized_end=36825
-  _DEBUGCMDOUT._serialized_start=36827
-  _DEBUGCMDOUT._serialized_end=36853
-  _DEBUGCMDOUTMSG._serialized_start=36855
-  _DEBUGCMDOUTMSG._serialized_end=36949
-  _DEBUGCMDRESULT._serialized_start=36951
-  _DEBUGCMDRESULT._serialized_end=36980
-  _DEBUGCMDRESULTMSG._serialized_start=36982
-  _DEBUGCMDRESULTMSG._serialized_end=37082
-  _LISTCMDOUT._serialized_start=37084
-  _LISTCMDOUT._serialized_end=37109
-  _LISTCMDOUTMSG._serialized_start=37111
-  _LISTCMDOUTMSG._serialized_end=37203
-  _NOTE._serialized_start=37205
-  _NOTE._serialized_end=37224
-  _NOTEMSG._serialized_start=37226
-  _NOTEMSG._serialized_end=37306
+  _INDBTEVENTDEBUG._serialized_start=8380
+  _INDBTEVENTDEBUG._serialized_end=8513
+  _INDBTEVENTDEBUGMSG._serialized_start=8515
+  _INDBTEVENTDEBUGMSG._serialized_end=8617
+  _INDBTEVENTINFO._serialized_start=8620
+  _INDBTEVENTINFO._serialized_end=8752
+  _INDBTEVENTINFOMSG._serialized_start=8754
+  _INDBTEVENTINFOMSG._serialized_end=8854
+  _INDBTEVENTWARNING._serialized_start=8857
+  _INDBTEVENTWARNING._serialized_end=8992
+  _INDBTEVENTWARNINGMSG._serialized_start=8994
+  _INDBTEVENTWARNINGMSG._serialized_end=9100
+  _INDBTEVENTERROR._serialized_start=9103
+  _INDBTEVENTERROR._serialized_end=9254
+  _INDBTEVENTERRORMSG._serialized_start=9256
+  _INDBTEVENTERRORMSG._serialized_end=9358
+  _CONNECTIONLEFTOPEN._serialized_start=9360
+  _CONNECTIONLEFTOPEN._serialized_end=9441
+  _CONNECTIONLEFTOPENMSG._serialized_start=9443
+  _CONNECTIONLEFTOPENMSG._serialized_end=9551
+  _ROLLBACK._serialized_start=9553
+  _ROLLBACK._serialized_end=9624
+  _ROLLBACKMSG._serialized_start=9626
+  _ROLLBACKMSG._serialized_end=9714
+  _CACHEMISS._serialized_start=9716
+  _CACHEMISS._serialized_end=9780
+  _CACHEMISSMSG._serialized_start=9782
+  _CACHEMISSMSG._serialized_end=9872
+  _LISTRELATIONS._serialized_start=9874
+  _LISTRELATIONS._serialized_end=9972
+  _LISTRELATIONSMSG._serialized_start=9974
+  _LISTRELATIONSMSG._serialized_end=10072
+  _CONNECTIONUSED._serialized_start=10074
+  _CONNECTIONUSED._serialized_end=10170
+  _CONNECTIONUSEDMSG._serialized_start=10172
+  _CONNECTIONUSEDMSG._serialized_end=10272
+  _SQLQUERY._serialized_start=10274
+  _SQLQUERY._serialized_end=10358
+  _SQLQUERYMSG._serialized_start=10360
+  _SQLQUERYMSG._serialized_end=10448
+  _SQLQUERYSTATUS._serialized_start=10450
+  _SQLQUERYSTATUS._serialized_end=10541
+  _SQLQUERYSTATUSMSG._serialized_start=10543
+  _SQLQUERYSTATUSMSG._serialized_end=10643
+  _SQLCOMMIT._serialized_start=10645
+  _SQLCOMMIT._serialized_end=10717
+  _SQLCOMMITMSG._serialized_start=10719
+  _SQLCOMMITMSG._serialized_end=10809
+  _COLTYPECHANGE._serialized_start=10811
+  _COLTYPECHANGE._serialized_end=10908
+  _COLTYPECHANGEMSG._serialized_start=10910
+  _COLTYPECHANGEMSG._serialized_end=11008
+  _SCHEMACREATION._serialized_start=11010
+  _SCHEMACREATION._serialized_end=11074
+  _SCHEMACREATIONMSG._serialized_start=11076
+  _SCHEMACREATIONMSG._serialized_end=11176
+  _SCHEMADROP._serialized_start=11178
+  _SCHEMADROP._serialized_end=11238
+  _SCHEMADROPMSG._serialized_start=11240
+  _SCHEMADROPMSG._serialized_end=11332
+  _CACHEACTION._serialized_start=11335
+  _CACHEACTION._serialized_end=11557
+  _CACHEACTIONMSG._serialized_start=11559
+  _CACHEACTIONMSG._serialized_end=11653
+  _CACHEDUMPGRAPH._serialized_start=11656
+  _CACHEDUMPGRAPH._serialized_end=11808
+  _CACHEDUMPGRAPH_DUMPENTRY._serialized_start=11765
+  _CACHEDUMPGRAPH_DUMPENTRY._serialized_end=11808
+  _CACHEDUMPGRAPHMSG._serialized_start=11810
+  _CACHEDUMPGRAPHMSG._serialized_end=11910
+  _ADAPTERIMPORTERROR._serialized_start=11912
+  _ADAPTERIMPORTERROR._serialized_end=11945
+  _ADAPTERIMPORTERRORMSG._serialized_start=11947
+  _ADAPTERIMPORTERRORMSG._serialized_end=12055
+  _PLUGINLOADERROR._serialized_start=12057
+  _PLUGINLOADERROR._serialized_end=12092
+  _PLUGINLOADERRORMSG._serialized_start=12094
+  _PLUGINLOADERRORMSG._serialized_end=12196
+  _NEWCONNECTIONOPENING._serialized_start=12198
+  _NEWCONNECTIONOPENING._serialized_end=12288
+  _NEWCONNECTIONOPENINGMSG._serialized_start=12290
+  _NEWCONNECTIONOPENINGMSG._serialized_end=12402
+  _CODEEXECUTION._serialized_start=12404
+  _CODEEXECUTION._serialized_end=12460
+  _CODEEXECUTIONMSG._serialized_start=12462
+  _CODEEXECUTIONMSG._serialized_end=12560
+  _CODEEXECUTIONSTATUS._serialized_start=12562
+  _CODEEXECUTIONSTATUS._serialized_end=12616
+  _CODEEXECUTIONSTATUSMSG._serialized_start=12618
+  _CODEEXECUTIONSTATUSMSG._serialized_end=12728
+  _CATALOGGENERATIONERROR._serialized_start=12730
+  _CATALOGGENERATIONERROR._serialized_end=12767
+  _CATALOGGENERATIONERRORMSG._serialized_start=12769
+  _CATALOGGENERATIONERRORMSG._serialized_end=12885
+  _WRITECATALOGFAILURE._serialized_start=12887
+  _WRITECATALOGFAILURE._serialized_end=12932
+  _WRITECATALOGFAILUREMSG._serialized_start=12934
+  _WRITECATALOGFAILUREMSG._serialized_end=13044
+  _CATALOGWRITTEN._serialized_start=13046
+  _CATALOGWRITTEN._serialized_end=13076
+  _CATALOGWRITTENMSG._serialized_start=13078
+  _CATALOGWRITTENMSG._serialized_end=13178
+  _CANNOTGENERATEDOCS._serialized_start=13180
+  _CANNOTGENERATEDOCS._serialized_end=13200
+  _CANNOTGENERATEDOCSMSG._serialized_start=13202
+  _CANNOTGENERATEDOCSMSG._serialized_end=13310
+  _BUILDINGCATALOG._serialized_start=13312
+  _BUILDINGCATALOG._serialized_end=13329
+  _BUILDINGCATALOGMSG._serialized_start=13331
+  _BUILDINGCATALOGMSG._serialized_end=13433
+  _DATABASEERRORRUNNINGHOOK._serialized_start=13435
+  _DATABASEERRORRUNNINGHOOK._serialized_end=13480
+  _DATABASEERRORRUNNINGHOOKMSG._serialized_start=13482
+  _DATABASEERRORRUNNINGHOOKMSG._serialized_end=13602
+  _HOOKSRUNNING._serialized_start=13604
+  _HOOKSRUNNING._serialized_end=13656
+  _HOOKSRUNNINGMSG._serialized_start=13658
+  _HOOKSRUNNINGMSG._serialized_end=13754
+  _FINISHEDRUNNINGSTATS._serialized_start=13756
+  _FINISHEDRUNNINGSTATS._serialized_end=13840
+  _FINISHEDRUNNINGSTATSMSG._serialized_start=13842
+  _FINISHEDRUNNINGSTATSMSG._serialized_end=13954
+  _CONSTRAINTNOTENFORCED._serialized_start=13956
+  _CONSTRAINTNOTENFORCED._serialized_end=14016
+  _CONSTRAINTNOTENFORCEDMSG._serialized_start=14018
+  _CONSTRAINTNOTENFORCEDMSG._serialized_end=14132
+  _CONSTRAINTNOTSUPPORTED._serialized_start=14134
+  _CONSTRAINTNOTSUPPORTED._serialized_end=14195
+  _CONSTRAINTNOTSUPPORTEDMSG._serialized_start=14197
+  _CONSTRAINTNOTSUPPORTEDMSG._serialized_end=14313
+  _INPUTFILEDIFFERROR._serialized_start=14315
+  _INPUTFILEDIFFERROR._serialized_end=14370
+  _INPUTFILEDIFFERRORMSG._serialized_start=14372
+  _INPUTFILEDIFFERRORMSG._serialized_end=14480
+  _INVALIDVALUEFORFIELD._serialized_start=14482
+  _INVALIDVALUEFORFIELD._serialized_end=14545
+  _INVALIDVALUEFORFIELDMSG._serialized_start=14547
+  _INVALIDVALUEFORFIELDMSG._serialized_end=14659
+  _VALIDATIONWARNING._serialized_start=14661
+  _VALIDATIONWARNING._serialized_end=14742
+  _VALIDATIONWARNINGMSG._serialized_start=14744
+  _VALIDATIONWARNINGMSG._serialized_end=14850
+  _PARSEPERFINFOPATH._serialized_start=14852
+  _PARSEPERFINFOPATH._serialized_end=14885
+  _PARSEPERFINFOPATHMSG._serialized_start=14887
+  _PARSEPERFINFOPATHMSG._serialized_end=14993
+  _GENERICTESTFILEPARSE._serialized_start=14995
+  _GENERICTESTFILEPARSE._serialized_end=15031
+  _GENERICTESTFILEPARSEMSG._serialized_start=15033
+  _GENERICTESTFILEPARSEMSG._serialized_end=15145
+  _MACROFILEPARSE._serialized_start=15147
+  _MACROFILEPARSE._serialized_end=15177
+  _MACROFILEPARSEMSG._serialized_start=15179
+  _MACROFILEPARSEMSG._serialized_end=15279
+  _PARTIALPARSINGERRORPROCESSINGFILE._serialized_start=15281
+  _PARTIALPARSINGERRORPROCESSINGFILE._serialized_end=15330
+  _PARTIALPARSINGERRORPROCESSINGFILEMSG._serialized_start=15333
+  _PARTIALPARSINGERRORPROCESSINGFILEMSG._serialized_end=15471
+  _PARTIALPARSINGERROR._serialized_start=15474
+  _PARTIALPARSINGERROR._serialized_end=15608
+  _PARTIALPARSINGERROR_EXCINFOENTRY._serialized_start=15562
+  _PARTIALPARSINGERROR_EXCINFOENTRY._serialized_end=15608
+  _PARTIALPARSINGERRORMSG._serialized_start=15610
+  _PARTIALPARSINGERRORMSG._serialized_end=15720
+  _PARTIALPARSINGSKIPPARSING._serialized_start=15722
+  _PARTIALPARSINGSKIPPARSING._serialized_end=15749
+  _PARTIALPARSINGSKIPPARSINGMSG._serialized_start=15751
+  _PARTIALPARSINGSKIPPARSINGMSG._serialized_end=15873
+  _UNABLETOPARTIALPARSE._serialized_start=15875
+  _UNABLETOPARTIALPARSE._serialized_end=15913
+  _UNABLETOPARTIALPARSEMSG._serialized_start=15915
+  _UNABLETOPARTIALPARSEMSG._serialized_end=16027
+  _STATECHECKVARSHASH._serialized_start=16029
+  _STATECHECKVARSHASH._serialized_end=16131
+  _STATECHECKVARSHASHMSG._serialized_start=16133
+  _STATECHECKVARSHASHMSG._serialized_end=16241
+  _PARTIALPARSINGNOTENABLED._serialized_start=16243
+  _PARTIALPARSINGNOTENABLED._serialized_end=16269
+  _PARTIALPARSINGNOTENABLEDMSG._serialized_start=16271
+  _PARTIALPARSINGNOTENABLEDMSG._serialized_end=16391
+  _PARSEDFILELOADFAILED._serialized_start=16393
+  _PARSEDFILELOADFAILED._serialized_end=16460
+  _PARSEDFILELOADFAILEDMSG._serialized_start=16462
+  _PARSEDFILELOADFAILEDMSG._serialized_end=16574
+  _PARTIALPARSINGENABLED._serialized_start=16576
+  _PARTIALPARSINGENABLED._serialized_end=16648
+  _PARTIALPARSINGENABLEDMSG._serialized_start=16650
+  _PARTIALPARSINGENABLEDMSG._serialized_end=16764
+  _PARTIALPARSINGFILE._serialized_start=16766
+  _PARTIALPARSINGFILE._serialized_end=16822
+  _PARTIALPARSINGFILEMSG._serialized_start=16824
+  _PARTIALPARSINGFILEMSG._serialized_end=16932
+  _INVALIDDISABLEDTARGETINTESTNODE._serialized_start=16935
+  _INVALIDDISABLEDTARGETINTESTNODE._serialized_end=17110
+  _INVALIDDISABLEDTARGETINTESTNODEMSG._serialized_start=17113
+  _INVALIDDISABLEDTARGETINTESTNODEMSG._serialized_end=17247
+  _UNUSEDRESOURCECONFIGPATH._serialized_start=17249
+  _UNUSEDRESOURCECONFIGPATH._serialized_end=17304
+  _UNUSEDRESOURCECONFIGPATHMSG._serialized_start=17306
+  _UNUSEDRESOURCECONFIGPATHMSG._serialized_end=17426
+  _SEEDINCREASED._serialized_start=17428
+  _SEEDINCREASED._serialized_end=17479
+  _SEEDINCREASEDMSG._serialized_start=17481
+  _SEEDINCREASEDMSG._serialized_end=17579
+  _SEEDEXCEEDSLIMITSAMEPATH._serialized_start=17581
+  _SEEDEXCEEDSLIMITSAMEPATH._serialized_end=17643
+  _SEEDEXCEEDSLIMITSAMEPATHMSG._serialized_start=17645
+  _SEEDEXCEEDSLIMITSAMEPATHMSG._serialized_end=17765
+  _SEEDEXCEEDSLIMITANDPATHCHANGED._serialized_start=17767
+  _SEEDEXCEEDSLIMITANDPATHCHANGED._serialized_end=17835
+  _SEEDEXCEEDSLIMITANDPATHCHANGEDMSG._serialized_start=17838
+  _SEEDEXCEEDSLIMITANDPATHCHANGEDMSG._serialized_end=17970
+  _SEEDEXCEEDSLIMITCHECKSUMCHANGED._serialized_start=17972
+  _SEEDEXCEEDSLIMITCHECKSUMCHANGED._serialized_end=18064
+  _SEEDEXCEEDSLIMITCHECKSUMCHANGEDMSG._serialized_start=18067
+  _SEEDEXCEEDSLIMITCHECKSUMCHANGEDMSG._serialized_end=18201
+  _UNUSEDTABLES._serialized_start=18203
+  _UNUSEDTABLES._serialized_end=18240
+  _UNUSEDTABLESMSG._serialized_start=18242
+  _UNUSEDTABLESMSG._serialized_end=18338
+  _WRONGRESOURCESCHEMAFILE._serialized_start=18341
+  _WRONGRESOURCESCHEMAFILE._serialized_end=18476
+  _WRONGRESOURCESCHEMAFILEMSG._serialized_start=18478
+  _WRONGRESOURCESCHEMAFILEMSG._serialized_end=18596
+  _NONODEFORYAMLKEY._serialized_start=18598
+  _NONODEFORYAMLKEY._serialized_end=18673
+  _NONODEFORYAMLKEYMSG._serialized_start=18675
+  _NONODEFORYAMLKEYMSG._serialized_end=18779
+  _MACRONOTFOUNDFORPATCH._serialized_start=18781
+  _MACRONOTFOUNDFORPATCH._serialized_end=18824
+  _MACRONOTFOUNDFORPATCHMSG._serialized_start=18826
+  _MACRONOTFOUNDFORPATCHMSG._serialized_end=18940
+  _NODENOTFOUNDORDISABLED._serialized_start=18943
+  _NODENOTFOUNDORDISABLED._serialized_end=19127
+  _NODENOTFOUNDORDISABLEDMSG._serialized_start=19129
+  _NODENOTFOUNDORDISABLEDMSG._serialized_end=19245
+  _JINJALOGWARNING._serialized_start=19247
+  _JINJALOGWARNING._serialized_end=19319
+  _JINJALOGWARNINGMSG._serialized_start=19321
+  _JINJALOGWARNINGMSG._serialized_end=19423
+  _JINJALOGINFO._serialized_start=19425
+  _JINJALOGINFO._serialized_end=19494
+  _JINJALOGINFOMSG._serialized_start=19496
+  _JINJALOGINFOMSG._serialized_end=19592
+  _JINJALOGDEBUG._serialized_start=19594
+  _JINJALOGDEBUG._serialized_end=19664
+  _JINJALOGDEBUGMSG._serialized_start=19666
+  _JINJALOGDEBUGMSG._serialized_end=19764
+  _UNPINNEDREFNEWVERSIONAVAILABLE._serialized_start=19767
+  _UNPINNEDREFNEWVERSIONAVAILABLE._serialized_end=19941
+  _UNPINNEDREFNEWVERSIONAVAILABLEMSG._serialized_start=19944
+  _UNPINNEDREFNEWVERSIONAVAILABLEMSG._serialized_end=20076
+  _GITSPARSECHECKOUTSUBDIRECTORY._serialized_start=20078
+  _GITSPARSECHECKOUTSUBDIRECTORY._serialized_end=20125
+  _GITSPARSECHECKOUTSUBDIRECTORYMSG._serialized_start=20128
+  _GITSPARSECHECKOUTSUBDIRECTORYMSG._serialized_end=20258
+  _GITPROGRESSCHECKOUTREVISION._serialized_start=20260
+  _GITPROGRESSCHECKOUTREVISION._serialized_end=20307
+  _GITPROGRESSCHECKOUTREVISIONMSG._serialized_start=20309
+  _GITPROGRESSCHECKOUTREVISIONMSG._serialized_end=20435
+  _GITPROGRESSUPDATINGEXISTINGDEPENDENCY._serialized_start=20437
+  _GITPROGRESSUPDATINGEXISTINGDEPENDENCY._serialized_end=20489
+  _GITPROGRESSUPDATINGEXISTINGDEPENDENCYMSG._serialized_start=20492
+  _GITPROGRESSUPDATINGEXISTINGDEPENDENCYMSG._serialized_end=20638
+  _GITPROGRESSPULLINGNEWDEPENDENCY._serialized_start=20640
+  _GITPROGRESSPULLINGNEWDEPENDENCY._serialized_end=20686
+  _GITPROGRESSPULLINGNEWDEPENDENCYMSG._serialized_start=20689
+  _GITPROGRESSPULLINGNEWDEPENDENCYMSG._serialized_end=20823
+  _GITNOTHINGTODO._serialized_start=20825
+  _GITNOTHINGTODO._serialized_end=20854
+  _GITNOTHINGTODOMSG._serialized_start=20856
+  _GITNOTHINGTODOMSG._serialized_end=20956
+  _GITPROGRESSUPDATEDCHECKOUTRANGE._serialized_start=20958
+  _GITPROGRESSUPDATEDCHECKOUTRANGE._serialized_end=21027
+  _GITPROGRESSUPDATEDCHECKOUTRANGEMSG._serialized_start=21030
+  _GITPROGRESSUPDATEDCHECKOUTRANGEMSG._serialized_end=21164
+  _GITPROGRESSCHECKEDOUTAT._serialized_start=21166
+  _GITPROGRESSCHECKEDOUTAT._serialized_end=21208
+  _GITPROGRESSCHECKEDOUTATMSG._serialized_start=21210
+  _GITPROGRESSCHECKEDOUTATMSG._serialized_end=21328
+  _REGISTRYPROGRESSGETREQUEST._serialized_start=21330
+  _REGISTRYPROGRESSGETREQUEST._serialized_end=21371
+  _REGISTRYPROGRESSGETREQUESTMSG._serialized_start=21373
+  _REGISTRYPROGRESSGETREQUESTMSG._serialized_end=21497
+  _REGISTRYPROGRESSGETRESPONSE._serialized_start=21499
+  _REGISTRYPROGRESSGETRESPONSE._serialized_end=21560
+  _REGISTRYPROGRESSGETRESPONSEMSG._serialized_start=21562
+  _REGISTRYPROGRESSGETRESPONSEMSG._serialized_end=21688
+  _SELECTORREPORTINVALIDSELECTOR._serialized_start=21690
+  _SELECTORREPORTINVALIDSELECTOR._serialized_end=21785
+  _SELECTORREPORTINVALIDSELECTORMSG._serialized_start=21788
+  _SELECTORREPORTINVALIDSELECTORMSG._serialized_end=21918
+  _DEPSNOPACKAGESFOUND._serialized_start=21920
+  _DEPSNOPACKAGESFOUND._serialized_end=21941
+  _DEPSNOPACKAGESFOUNDMSG._serialized_start=21943
+  _DEPSNOPACKAGESFOUNDMSG._serialized_end=22053
+  _DEPSSTARTPACKAGEINSTALL._serialized_start=22055
+  _DEPSSTARTPACKAGEINSTALL._serialized_end=22102
+  _DEPSSTARTPACKAGEINSTALLMSG._serialized_start=22104
+  _DEPSSTARTPACKAGEINSTALLMSG._serialized_end=22222
+  _DEPSINSTALLINFO._serialized_start=22224
+  _DEPSINSTALLINFO._serialized_end=22263
+  _DEPSINSTALLINFOMSG._serialized_start=22265
+  _DEPSINSTALLINFOMSG._serialized_end=22367
+  _DEPSUPDATEAVAILABLE._serialized_start=22369
+  _DEPSUPDATEAVAILABLE._serialized_end=22414
+  _DEPSUPDATEAVAILABLEMSG._serialized_start=22416
+  _DEPSUPDATEAVAILABLEMSG._serialized_end=22526
+  _DEPSUPTODATE._serialized_start=22528
+  _DEPSUPTODATE._serialized_end=22542
+  _DEPSUPTODATEMSG._serialized_start=22544
+  _DEPSUPTODATEMSG._serialized_end=22640
+  _DEPSLISTSUBDIRECTORY._serialized_start=22642
+  _DEPSLISTSUBDIRECTORY._serialized_end=22686
+  _DEPSLISTSUBDIRECTORYMSG._serialized_start=22688
+  _DEPSLISTSUBDIRECTORYMSG._serialized_end=22800
+  _DEPSNOTIFYUPDATESAVAILABLE._serialized_start=22802
+  _DEPSNOTIFYUPDATESAVAILABLE._serialized_end=22848
+  _DEPSNOTIFYUPDATESAVAILABLEMSG._serialized_start=22850
+  _DEPSNOTIFYUPDATESAVAILABLEMSG._serialized_end=22974
+  _RETRYEXTERNALCALL._serialized_start=22976
+  _RETRYEXTERNALCALL._serialized_end=23025
+  _RETRYEXTERNALCALLMSG._serialized_start=23027
+  _RETRYEXTERNALCALLMSG._serialized_end=23133
+  _RECORDRETRYEXCEPTION._serialized_start=23135
+  _RECORDRETRYEXCEPTION._serialized_end=23170
+  _RECORDRETRYEXCEPTIONMSG._serialized_start=23172
+  _RECORDRETRYEXCEPTIONMSG._serialized_end=23284
+  _REGISTRYINDEXPROGRESSGETREQUEST._serialized_start=23286
+  _REGISTRYINDEXPROGRESSGETREQUEST._serialized_end=23332
+  _REGISTRYINDEXPROGRESSGETREQUESTMSG._serialized_start=23335
+  _REGISTRYINDEXPROGRESSGETREQUESTMSG._serialized_end=23469
+  _REGISTRYINDEXPROGRESSGETRESPONSE._serialized_start=23471
+  _REGISTRYINDEXPROGRESSGETRESPONSE._serialized_end=23537
+  _REGISTRYINDEXPROGRESSGETRESPONSEMSG._serialized_start=23540
+  _REGISTRYINDEXPROGRESSGETRESPONSEMSG._serialized_end=23676
+  _REGISTRYRESPONSEUNEXPECTEDTYPE._serialized_start=23678
+  _REGISTRYRESPONSEUNEXPECTEDTYPE._serialized_end=23728
+  _REGISTRYRESPONSEUNEXPECTEDTYPEMSG._serialized_start=23731
+  _REGISTRYRESPONSEUNEXPECTEDTYPEMSG._serialized_end=23863
+  _REGISTRYRESPONSEMISSINGTOPKEYS._serialized_start=23865
+  _REGISTRYRESPONSEMISSINGTOPKEYS._serialized_end=23915
+  _REGISTRYRESPONSEMISSINGTOPKEYSMSG._serialized_start=23918
+  _REGISTRYRESPONSEMISSINGTOPKEYSMSG._serialized_end=24050
+  _REGISTRYRESPONSEMISSINGNESTEDKEYS._serialized_start=24052
+  _REGISTRYRESPONSEMISSINGNESTEDKEYS._serialized_end=24105
+  _REGISTRYRESPONSEMISSINGNESTEDKEYSMSG._serialized_start=24108
+  _REGISTRYRESPONSEMISSINGNESTEDKEYSMSG._serialized_end=24246
+  _REGISTRYRESPONSEEXTRANESTEDKEYS._serialized_start=24248
+  _REGISTRYRESPONSEEXTRANESTEDKEYS._serialized_end=24299
+  _REGISTRYRESPONSEEXTRANESTEDKEYSMSG._serialized_start=24302
+  _REGISTRYRESPONSEEXTRANESTEDKEYSMSG._serialized_end=24436
+  _DEPSSETDOWNLOADDIRECTORY._serialized_start=24438
+  _DEPSSETDOWNLOADDIRECTORY._serialized_end=24478
+  _DEPSSETDOWNLOADDIRECTORYMSG._serialized_start=24480
+  _DEPSSETDOWNLOADDIRECTORYMSG._serialized_end=24600
+  _DEPSUNPINNED._serialized_start=24602
+  _DEPSUNPINNED._serialized_end=24647
+  _DEPSUNPINNEDMSG._serialized_start=24649
+  _DEPSUNPINNEDMSG._serialized_end=24745
+  _NONODESFORSELECTIONCRITERIA._serialized_start=24747
+  _NONODESFORSELECTIONCRITERIA._serialized_end=24794
+  _NONODESFORSELECTIONCRITERIAMSG._serialized_start=24796
+  _NONODESFORSELECTIONCRITERIAMSG._serialized_end=24922
+  _RUNNINGOPERATIONCAUGHTERROR._serialized_start=24924
+  _RUNNINGOPERATIONCAUGHTERROR._serialized_end=24966
+  _RUNNINGOPERATIONCAUGHTERRORMSG._serialized_start=24968
+  _RUNNINGOPERATIONCAUGHTERRORMSG._serialized_end=25094
+  _COMPILECOMPLETE._serialized_start=25096
+  _COMPILECOMPLETE._serialized_end=25113
+  _COMPILECOMPLETEMSG._serialized_start=25115
+  _COMPILECOMPLETEMSG._serialized_end=25217
+  _FRESHNESSCHECKCOMPLETE._serialized_start=25219
+  _FRESHNESSCHECKCOMPLETE._serialized_end=25243
+  _FRESHNESSCHECKCOMPLETEMSG._serialized_start=25245
+  _FRESHNESSCHECKCOMPLETEMSG._serialized_end=25361
+  _SEEDHEADER._serialized_start=25363
+  _SEEDHEADER._serialized_end=25391
+  _SEEDHEADERMSG._serialized_start=25393
+  _SEEDHEADERMSG._serialized_end=25485
+  _SQLRUNNEREXCEPTION._serialized_start=25487
+  _SQLRUNNEREXCEPTION._serialized_end=25538
+  _SQLRUNNEREXCEPTIONMSG._serialized_start=25540
+  _SQLRUNNEREXCEPTIONMSG._serialized_end=25648
+  _LOGTESTRESULT._serialized_start=25651
+  _LOGTESTRESULT._serialized_end=25819
+  _LOGTESTRESULTMSG._serialized_start=25821
+  _LOGTESTRESULTMSG._serialized_end=25919
+  _LOGSTARTLINE._serialized_start=25921
+  _LOGSTARTLINE._serialized_end=26028
+  _LOGSTARTLINEMSG._serialized_start=26030
+  _LOGSTARTLINEMSG._serialized_end=26126
+  _LOGMODELRESULT._serialized_start=26129
+  _LOGMODELRESULT._serialized_end=26278
+  _LOGMODELRESULTMSG._serialized_start=26280
+  _LOGMODELRESULTMSG._serialized_end=26380
+  _LOGSNAPSHOTRESULT._serialized_start=26383
+  _LOGSNAPSHOTRESULT._serialized_end=26633
+  _LOGSNAPSHOTRESULT_CFGENTRY._serialized_start=26591
+  _LOGSNAPSHOTRESULT_CFGENTRY._serialized_end=26633
+  _LOGSNAPSHOTRESULTMSG._serialized_start=26635
+  _LOGSNAPSHOTRESULTMSG._serialized_end=26741
+  _LOGSEEDRESULT._serialized_start=26744
+  _LOGSEEDRESULT._serialized_end=26929
+  _LOGSEEDRESULTMSG._serialized_start=26931
+  _LOGSEEDRESULTMSG._serialized_end=27029
+  _LOGFRESHNESSRESULT._serialized_start=27032
+  _LOGFRESHNESSRESULT._serialized_end=27205
+  _LOGFRESHNESSRESULTMSG._serialized_start=27207
+  _LOGFRESHNESSRESULTMSG._serialized_end=27315
+  _LOGCANCELLINE._serialized_start=27317
+  _LOGCANCELLINE._serialized_end=27351
+  _LOGCANCELLINEMSG._serialized_start=27353
+  _LOGCANCELLINEMSG._serialized_end=27451
+  _DEFAULTSELECTOR._serialized_start=27453
+  _DEFAULTSELECTOR._serialized_end=27484
+  _DEFAULTSELECTORMSG._serialized_start=27486
+  _DEFAULTSELECTORMSG._serialized_end=27588
+  _NODESTART._serialized_start=27590
+  _NODESTART._serialized_end=27643
+  _NODESTARTMSG._serialized_start=27645
+  _NODESTARTMSG._serialized_end=27735
+  _NODEFINISHED._serialized_start=27737
+  _NODEFINISHED._serialized_end=27840
+  _NODEFINISHEDMSG._serialized_start=27842
+  _NODEFINISHEDMSG._serialized_end=27938
+  _QUERYCANCELATIONUNSUPPORTED._serialized_start=27940
+  _QUERYCANCELATIONUNSUPPORTED._serialized_end=27983
+  _QUERYCANCELATIONUNSUPPORTEDMSG._serialized_start=27985
+  _QUERYCANCELATIONUNSUPPORTEDMSG._serialized_end=28111
+  _CONCURRENCYLINE._serialized_start=28113
+  _CONCURRENCYLINE._serialized_end=28192
+  _CONCURRENCYLINEMSG._serialized_start=28194
+  _CONCURRENCYLINEMSG._serialized_end=28296
+  _WRITINGINJECTEDSQLFORNODE._serialized_start=28298
+  _WRITINGINJECTEDSQLFORNODE._serialized_end=28367
+  _WRITINGINJECTEDSQLFORNODEMSG._serialized_start=28369
+  _WRITINGINJECTEDSQLFORNODEMSG._serialized_end=28491
+  _NODECOMPILING._serialized_start=28493
+  _NODECOMPILING._serialized_end=28550
+  _NODECOMPILINGMSG._serialized_start=28552
+  _NODECOMPILINGMSG._serialized_end=28650
+  _NODEEXECUTING._serialized_start=28652
+  _NODEEXECUTING._serialized_end=28709
+  _NODEEXECUTINGMSG._serialized_start=28711
+  _NODEEXECUTINGMSG._serialized_end=28809
+  _LOGHOOKSTARTLINE._serialized_start=28811
+  _LOGHOOKSTARTLINE._serialized_end=28920
+  _LOGHOOKSTARTLINEMSG._serialized_start=28922
+  _LOGHOOKSTARTLINEMSG._serialized_end=29026
+  _LOGHOOKENDLINE._serialized_start=29029
+  _LOGHOOKENDLINE._serialized_end=29176
+  _LOGHOOKENDLINEMSG._serialized_start=29178
+  _LOGHOOKENDLINEMSG._serialized_end=29278
+  _SKIPPINGDETAILS._serialized_start=29281
+  _SKIPPINGDETAILS._serialized_end=29428
+  _SKIPPINGDETAILSMSG._serialized_start=29430
+  _SKIPPINGDETAILSMSG._serialized_end=29532
+  _NOTHINGTODO._serialized_start=29534
+  _NOTHINGTODO._serialized_end=29547
+  _NOTHINGTODOMSG._serialized_start=29549
+  _NOTHINGTODOMSG._serialized_end=29643
+  _RUNNINGOPERATIONUNCAUGHTERROR._serialized_start=29645
+  _RUNNINGOPERATIONUNCAUGHTERROR._serialized_end=29689
+  _RUNNINGOPERATIONUNCAUGHTERRORMSG._serialized_start=29692
+  _RUNNINGOPERATIONUNCAUGHTERRORMSG._serialized_end=29822
+  _ENDRUNRESULT._serialized_start=29825
+  _ENDRUNRESULT._serialized_end=29972
+  _ENDRUNRESULTMSG._serialized_start=29974
+  _ENDRUNRESULTMSG._serialized_end=30070
+  _NONODESSELECTED._serialized_start=30072
+  _NONODESSELECTED._serialized_end=30089
+  _NONODESSELECTEDMSG._serialized_start=30091
+  _NONODESSELECTEDMSG._serialized_end=30193
+  _COMMANDCOMPLETED._serialized_start=30195
+  _COMMANDCOMPLETED._serialized_end=30314
+  _COMMANDCOMPLETEDMSG._serialized_start=30316
+  _COMMANDCOMPLETEDMSG._serialized_end=30420
+  _SHOWNODE._serialized_start=30422
+  _SHOWNODE._serialized_end=30529
+  _SHOWNODEMSG._serialized_start=30531
+  _SHOWNODEMSG._serialized_end=30619
+  _COMPILEDNODE._serialized_start=30621
+  _COMPILEDNODE._serialized_end=30733
+  _COMPILEDNODEMSG._serialized_start=30735
+  _COMPILEDNODEMSG._serialized_end=30831
+  _CATCHABLEEXCEPTIONONRUN._serialized_start=30833
+  _CATCHABLEEXCEPTIONONRUN._serialized_end=30931
+  _CATCHABLEEXCEPTIONONRUNMSG._serialized_start=30933
+  _CATCHABLEEXCEPTIONONRUNMSG._serialized_end=31051
+  _INTERNALERRORONRUN._serialized_start=31053
+  _INTERNALERRORONRUN._serialized_end=31106
+  _INTERNALERRORONRUNMSG._serialized_start=31108
+  _INTERNALERRORONRUNMSG._serialized_end=31216
+  _GENERICEXCEPTIONONRUN._serialized_start=31218
+  _GENERICEXCEPTIONONRUN._serialized_end=31293
+  _GENERICEXCEPTIONONRUNMSG._serialized_start=31295
+  _GENERICEXCEPTIONONRUNMSG._serialized_end=31409
+  _NODECONNECTIONRELEASEERROR._serialized_start=31411
+  _NODECONNECTIONRELEASEERROR._serialized_end=31489
+  _NODECONNECTIONRELEASEERRORMSG._serialized_start=31491
+  _NODECONNECTIONRELEASEERRORMSG._serialized_end=31615
+  _FOUNDSTATS._serialized_start=31617
+  _FOUNDSTATS._serialized_end=31648
+  _FOUNDSTATSMSG._serialized_start=31650
+  _FOUNDSTATSMSG._serialized_end=31742
+  _MAINKEYBOARDINTERRUPT._serialized_start=31744
+  _MAINKEYBOARDINTERRUPT._serialized_end=31767
+  _MAINKEYBOARDINTERRUPTMSG._serialized_start=31769
+  _MAINKEYBOARDINTERRUPTMSG._serialized_end=31883
+  _MAINENCOUNTEREDERROR._serialized_start=31885
+  _MAINENCOUNTEREDERROR._serialized_end=31920
+  _MAINENCOUNTEREDERRORMSG._serialized_start=31922
+  _MAINENCOUNTEREDERRORMSG._serialized_end=32034
+  _MAINSTACKTRACE._serialized_start=32036
+  _MAINSTACKTRACE._serialized_end=32073
+  _MAINSTACKTRACEMSG._serialized_start=32075
+  _MAINSTACKTRACEMSG._serialized_end=32175
+  _SYSTEMCOULDNOTWRITE._serialized_start=32177
+  _SYSTEMCOULDNOTWRITE._serialized_end=32241
+  _SYSTEMCOULDNOTWRITEMSG._serialized_start=32243
+  _SYSTEMCOULDNOTWRITEMSG._serialized_end=32353
+  _SYSTEMEXECUTINGCMD._serialized_start=32355
+  _SYSTEMEXECUTINGCMD._serialized_end=32388
+  _SYSTEMEXECUTINGCMDMSG._serialized_start=32390
+  _SYSTEMEXECUTINGCMDMSG._serialized_end=32498
+  _SYSTEMSTDOUT._serialized_start=32500
+  _SYSTEMSTDOUT._serialized_end=32528
+  _SYSTEMSTDOUTMSG._serialized_start=32530
+  _SYSTEMSTDOUTMSG._serialized_end=32626
+  _SYSTEMSTDERR._serialized_start=32628
+  _SYSTEMSTDERR._serialized_end=32656
+  _SYSTEMSTDERRMSG._serialized_start=32658
+  _SYSTEMSTDERRMSG._serialized_end=32754
+  _SYSTEMREPORTRETURNCODE._serialized_start=32756
+  _SYSTEMREPORTRETURNCODE._serialized_end=32800
+  _SYSTEMREPORTRETURNCODEMSG._serialized_start=32802
+  _SYSTEMREPORTRETURNCODEMSG._serialized_end=32918
+  _TIMINGINFOCOLLECTED._serialized_start=32920
+  _TIMINGINFOCOLLECTED._serialized_end=33032
+  _TIMINGINFOCOLLECTEDMSG._serialized_start=33034
+  _TIMINGINFOCOLLECTEDMSG._serialized_end=33144
+  _LOGDEBUGSTACKTRACE._serialized_start=33146
+  _LOGDEBUGSTACKTRACE._serialized_end=33184
+  _LOGDEBUGSTACKTRACEMSG._serialized_start=33186
+  _LOGDEBUGSTACKTRACEMSG._serialized_end=33294
+  _CHECKCLEANPATH._serialized_start=33296
+  _CHECKCLEANPATH._serialized_end=33326
+  _CHECKCLEANPATHMSG._serialized_start=33328
+  _CHECKCLEANPATHMSG._serialized_end=33428
+  _CONFIRMCLEANPATH._serialized_start=33430
+  _CONFIRMCLEANPATH._serialized_end=33462
+  _CONFIRMCLEANPATHMSG._serialized_start=33464
+  _CONFIRMCLEANPATHMSG._serialized_end=33568
+  _PROTECTEDCLEANPATH._serialized_start=33570
+  _PROTECTEDCLEANPATH._serialized_end=33604
+  _PROTECTEDCLEANPATHMSG._serialized_start=33606
+  _PROTECTEDCLEANPATHMSG._serialized_end=33714
+  _FINISHEDCLEANPATHS._serialized_start=33716
+  _FINISHEDCLEANPATHS._serialized_end=33736
+  _FINISHEDCLEANPATHSMSG._serialized_start=33738
+  _FINISHEDCLEANPATHSMSG._serialized_end=33846
+  _OPENCOMMAND._serialized_start=33848
+  _OPENCOMMAND._serialized_end=33901
+  _OPENCOMMANDMSG._serialized_start=33903
+  _OPENCOMMANDMSG._serialized_end=33997
+  _FORMATTING._serialized_start=33999
+  _FORMATTING._serialized_end=34024
+  _FORMATTINGMSG._serialized_start=34026
+  _FORMATTINGMSG._serialized_end=34118
+  _SERVINGDOCSPORT._serialized_start=34120
+  _SERVINGDOCSPORT._serialized_end=34168
+  _SERVINGDOCSPORTMSG._serialized_start=34170
+  _SERVINGDOCSPORTMSG._serialized_end=34272
+  _SERVINGDOCSACCESSINFO._serialized_start=34274
+  _SERVINGDOCSACCESSINFO._serialized_end=34311
+  _SERVINGDOCSACCESSINFOMSG._serialized_start=34313
+  _SERVINGDOCSACCESSINFOMSG._serialized_end=34427
+  _SERVINGDOCSEXITINFO._serialized_start=34429
+  _SERVINGDOCSEXITINFO._serialized_end=34450
+  _SERVINGDOCSEXITINFOMSG._serialized_start=34452
+  _SERVINGDOCSEXITINFOMSG._serialized_end=34562
+  _RUNRESULTWARNING._serialized_start=34564
+  _RUNRESULTWARNING._serialized_end=34638
+  _RUNRESULTWARNINGMSG._serialized_start=34640
+  _RUNRESULTWARNINGMSG._serialized_end=34744
+  _RUNRESULTFAILURE._serialized_start=34746
+  _RUNRESULTFAILURE._serialized_end=34820
+  _RUNRESULTFAILUREMSG._serialized_start=34822
+  _RUNRESULTFAILUREMSG._serialized_end=34926
+  _STATSLINE._serialized_start=34928
+  _STATSLINE._serialized_end=35035
+  _STATSLINE_STATSENTRY._serialized_start=34991
+  _STATSLINE_STATSENTRY._serialized_end=35035
+  _STATSLINEMSG._serialized_start=35037
+  _STATSLINEMSG._serialized_end=35127
+  _RUNRESULTERROR._serialized_start=35129
+  _RUNRESULTERROR._serialized_end=35158
+  _RUNRESULTERRORMSG._serialized_start=35160
+  _RUNRESULTERRORMSG._serialized_end=35260
+  _RUNRESULTERRORNOMESSAGE._serialized_start=35262
+  _RUNRESULTERRORNOMESSAGE._serialized_end=35303
+  _RUNRESULTERRORNOMESSAGEMSG._serialized_start=35305
+  _RUNRESULTERRORNOMESSAGEMSG._serialized_end=35423
+  _SQLCOMPILEDPATH._serialized_start=35425
+  _SQLCOMPILEDPATH._serialized_end=35456
+  _SQLCOMPILEDPATHMSG._serialized_start=35458
+  _SQLCOMPILEDPATHMSG._serialized_end=35560
+  _CHECKNODETESTFAILURE._serialized_start=35562
+  _CHECKNODETESTFAILURE._serialized_end=35607
+  _CHECKNODETESTFAILUREMSG._serialized_start=35609
+  _CHECKNODETESTFAILUREMSG._serialized_end=35721
+  _FIRSTRUNRESULTERROR._serialized_start=35723
+  _FIRSTRUNRESULTERROR._serialized_end=35757
+  _FIRSTRUNRESULTERRORMSG._serialized_start=35759
+  _FIRSTRUNRESULTERRORMSG._serialized_end=35869
+  _AFTERFIRSTRUNRESULTERROR._serialized_start=35871
+  _AFTERFIRSTRUNRESULTERROR._serialized_end=35910
+  _AFTERFIRSTRUNRESULTERRORMSG._serialized_start=35912
+  _AFTERFIRSTRUNRESULTERRORMSG._serialized_end=36032
+  _ENDOFRUNSUMMARY._serialized_start=36034
+  _ENDOFRUNSUMMARY._serialized_end=36121
+  _ENDOFRUNSUMMARYMSG._serialized_start=36123
+  _ENDOFRUNSUMMARYMSG._serialized_end=36225
+  _LOGSKIPBECAUSEERROR._serialized_start=36227
+  _LOGSKIPBECAUSEERROR._serialized_end=36312
+  _LOGSKIPBECAUSEERRORMSG._serialized_start=36314
+  _LOGSKIPBECAUSEERRORMSG._serialized_end=36424
+  _ENSUREGITINSTALLED._serialized_start=36426
+  _ENSUREGITINSTALLED._serialized_end=36446
+  _ENSUREGITINSTALLEDMSG._serialized_start=36448
+  _ENSUREGITINSTALLEDMSG._serialized_end=36556
+  _DEPSCREATINGLOCALSYMLINK._serialized_start=36558
+  _DEPSCREATINGLOCALSYMLINK._serialized_end=36584
+  _DEPSCREATINGLOCALSYMLINKMSG._serialized_start=36586
+  _DEPSCREATINGLOCALSYMLINKMSG._serialized_end=36706
+  _DEPSSYMLINKNOTAVAILABLE._serialized_start=36708
+  _DEPSSYMLINKNOTAVAILABLE._serialized_end=36733
+  _DEPSSYMLINKNOTAVAILABLEMSG._serialized_start=36735
+  _DEPSSYMLINKNOTAVAILABLEMSG._serialized_end=36853
+  _DISABLETRACKING._serialized_start=36855
+  _DISABLETRACKING._serialized_end=36872
+  _DISABLETRACKINGMSG._serialized_start=36874
+  _DISABLETRACKINGMSG._serialized_end=36976
+  _SENDINGEVENT._serialized_start=36978
+  _SENDINGEVENT._serialized_end=37008
+  _SENDINGEVENTMSG._serialized_start=37010
+  _SENDINGEVENTMSG._serialized_end=37106
+  _SENDEVENTFAILURE._serialized_start=37108
+  _SENDEVENTFAILURE._serialized_end=37126
+  _SENDEVENTFAILUREMSG._serialized_start=37128
+  _SENDEVENTFAILUREMSG._serialized_end=37232
+  _FLUSHEVENTS._serialized_start=37234
+  _FLUSHEVENTS._serialized_end=37247
+  _FLUSHEVENTSMSG._serialized_start=37249
+  _FLUSHEVENTSMSG._serialized_end=37343
+  _FLUSHEVENTSFAILURE._serialized_start=37345
+  _FLUSHEVENTSFAILURE._serialized_end=37365
+  _FLUSHEVENTSFAILUREMSG._serialized_start=37367
+  _FLUSHEVENTSFAILUREMSG._serialized_end=37475
+  _TRACKINGINITIALIZEFAILURE._serialized_start=37477
+  _TRACKINGINITIALIZEFAILURE._serialized_end=37522
+  _TRACKINGINITIALIZEFAILUREMSG._serialized_start=37524
+  _TRACKINGINITIALIZEFAILUREMSG._serialized_end=37646
+  _RUNRESULTWARNINGMESSAGE._serialized_start=37648
+  _RUNRESULTWARNINGMESSAGE._serialized_end=37686
+  _RUNRESULTWARNINGMESSAGEMSG._serialized_start=37688
+  _RUNRESULTWARNINGMESSAGEMSG._serialized_end=37806
+  _DEBUGCMDOUT._serialized_start=37808
+  _DEBUGCMDOUT._serialized_end=37834
+  _DEBUGCMDOUTMSG._serialized_start=37836
+  _DEBUGCMDOUTMSG._serialized_end=37930
+  _DEBUGCMDRESULT._serialized_start=37932
+  _DEBUGCMDRESULT._serialized_end=37961
+  _DEBUGCMDRESULTMSG._serialized_start=37963
+  _DEBUGCMDRESULTMSG._serialized_end=38063
+  _LISTCMDOUT._serialized_start=38065
+  _LISTCMDOUT._serialized_end=38090
+  _LISTCMDOUTMSG._serialized_start=38092
+  _LISTCMDOUTMSG._serialized_end=38184
+  _NOTE._serialized_start=38186
+  _NOTE._serialized_end=38205
+  _NOTEMSG._serialized_start=38207
+  _NOTEMSG._serialized_end=38287
 # @@protoc_insertion_point(module_scope)
```

### Comparing `in-dbt-core-1.5.0/dbt/exceptions.py` & `in-dbt-core-1.5.1/dbt/exceptions.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/flags.py` & `in-dbt-core-1.5.1/dbt/flags.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/graph/cli.py` & `in-dbt-core-1.5.1/dbt/graph/cli.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/graph/graph.py` & `in-dbt-core-1.5.1/dbt/graph/graph.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/graph/queue.py` & `in-dbt-core-1.5.1/dbt/graph/queue.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/graph/selector.py` & `in-dbt-core-1.5.1/dbt/graph/selector.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/graph/selector_methods.py` & `in-dbt-core-1.5.1/dbt/graph/selector_methods.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/graph/selector_spec.py` & `in-dbt-core-1.5.1/dbt/graph/selector_spec.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/helper_types.py` & `in-dbt-core-1.5.1/dbt/helper_types.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/include/README.md` & `in-dbt-core-1.5.1/dbt/include/README.md`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/include/global_project/docs/overview.md` & `in-dbt-core-1.5.1/dbt/include/global_project/docs/overview.md`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/include/global_project/macros/adapters/apply_grants.sql` & `in-dbt-core-1.5.1/dbt/include/global_project/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/include/global_project/macros/adapters/columns.sql` & `in-dbt-core-1.5.1/dbt/include/global_project/macros/adapters/columns.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/include/global_project/macros/adapters/freshness.sql` & `in-dbt-core-1.5.1/dbt/include/global_project/macros/adapters/freshness.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/include/global_project/macros/adapters/indexes.sql` & `in-dbt-core-1.5.1/dbt/include/global_project/macros/adapters/indexes.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/include/global_project/macros/adapters/metadata.sql` & `in-dbt-core-1.5.1/dbt/include/global_project/macros/adapters/metadata.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/include/global_project/macros/adapters/persist_docs.sql` & `in-dbt-core-1.5.1/dbt/include/global_project/macros/adapters/persist_docs.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/include/global_project/macros/adapters/relation.sql` & `in-dbt-core-1.5.1/dbt/include/global_project/macros/adapters/relation.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/include/global_project/macros/adapters/schema.sql` & `in-dbt-core-1.5.1/dbt/include/global_project/macros/adapters/schema.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/include/global_project/macros/adapters/timestamps.sql` & `in-dbt-core-1.5.1/dbt/include/global_project/macros/adapters/timestamps.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/include/global_project/macros/etc/datetime.sql` & `in-dbt-core-1.5.1/dbt/include/global_project/macros/etc/datetime.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/include/global_project/macros/etc/statement.sql` & `in-dbt-core-1.5.1/dbt/include/global_project/macros/etc/statement.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql` & `in-dbt-core-1.5.1/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql` & `in-dbt-core-1.5.1/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql` & `in-dbt-core-1.5.1/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql` & `in-dbt-core-1.5.1/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/configs.sql` & `in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/configs.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/hooks.sql` & `in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/hooks.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql` & `in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql` & `in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/models/incremental/merge.sql` & `in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/models/incremental/merge.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql` & `in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql` & `in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/models/table/columns_spec_ddl.sql` & `in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/models/table/columns_spec_ddl.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/models/table/create_table_as.sql` & `in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/models/table/create_table_as.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/models/table/table.sql` & `in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/models/table/table.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/models/view/create_or_replace_view.sql` & `in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/models/view/create_or_replace_view.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/models/view/create_view_as.sql` & `in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/models/view/create_view_as.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/models/view/view.sql` & `in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/models/view/view.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/seeds/helpers.sql` & `in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/seeds/helpers.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/seeds/seed.sql` & `in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/seeds/seed.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/snapshots/helpers.sql` & `in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/snapshots/helpers.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql` & `in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql` & `in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/snapshots/strategies.sql` & `in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/snapshots/strategies.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/tests/helpers.sql` & `in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/tests/helpers.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/include/global_project/macros/materializations/tests/test.sql` & `in-dbt-core-1.5.1/dbt/include/global_project/macros/materializations/tests/test.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/include/global_project/macros/python_model/python.sql` & `in-dbt-core-1.5.1/dbt/include/global_project/macros/python_model/python.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/include/global_project/macros/utils/data_types.sql` & `in-dbt-core-1.5.1/dbt/include/global_project/macros/utils/data_types.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/include/global_project/macros/utils/listagg.sql` & `in-dbt-core-1.5.1/dbt/include/global_project/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/include/global_project/macros/utils/split_part.sql` & `in-dbt-core-1.5.1/dbt/include/global_project/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/include/global_project/tests/generic/builtin.sql` & `in-dbt-core-1.5.1/dbt/include/global_project/tests/generic/builtin.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/include/index.html` & `in-dbt-core-1.5.1/dbt/include/index.html`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/include/starter_project/README.md` & `in-dbt-core-1.5.1/dbt/include/starter_project/README.md`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/include/starter_project/dbt_project.yml` & `in-dbt-core-1.5.1/dbt/include/starter_project/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/internal_deprecations.py` & `in-dbt-core-1.5.1/dbt/internal_deprecations.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/logger.py` & `in-dbt-core-1.5.1/dbt/logger.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/node_types.py` & `in-dbt-core-1.5.1/dbt/node_types.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/parser/__init__.py` & `in-dbt-core-1.5.1/dbt/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/parser/analysis.py` & `in-dbt-core-1.5.1/dbt/parser/analysis.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/parser/base.py` & `in-dbt-core-1.5.1/dbt/parser/base.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/parser/docs.py` & `in-dbt-core-1.5.1/dbt/parser/docs.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/parser/generic_test.py` & `in-dbt-core-1.5.1/dbt/parser/generic_test.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/parser/generic_test_builders.py` & `in-dbt-core-1.5.1/dbt/parser/generic_test_builders.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/parser/hooks.py` & `in-dbt-core-1.5.1/dbt/parser/hooks.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/parser/macros.py` & `in-dbt-core-1.5.1/dbt/parser/macros.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/parser/manifest.py` & `in-dbt-core-1.5.1/dbt/parser/manifest.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/parser/models.py` & `in-dbt-core-1.5.1/dbt/parser/models.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/parser/partial.py` & `in-dbt-core-1.5.1/dbt/parser/partial.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/parser/read_files.py` & `in-dbt-core-1.5.1/dbt/parser/read_files.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/parser/schema_renderer.py` & `in-dbt-core-1.5.1/dbt/parser/schema_renderer.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/parser/schemas.py` & `in-dbt-core-1.5.1/dbt/parser/schemas.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/parser/search.py` & `in-dbt-core-1.5.1/dbt/parser/search.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/parser/seeds.py` & `in-dbt-core-1.5.1/dbt/parser/seeds.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/parser/singular_test.py` & `in-dbt-core-1.5.1/dbt/parser/singular_test.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/parser/snapshots.py` & `in-dbt-core-1.5.1/dbt/parser/snapshots.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/parser/sources.py` & `in-dbt-core-1.5.1/dbt/parser/sources.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/parser/sql.py` & `in-dbt-core-1.5.1/dbt/parser/sql.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/semver.py` & `in-dbt-core-1.5.1/dbt/semver.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/task/base.py` & `in-dbt-core-1.5.1/dbt/task/base.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/task/build.py` & `in-dbt-core-1.5.1/dbt/task/build.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/task/clean.py` & `in-dbt-core-1.5.1/dbt/task/clean.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/task/compile.py` & `in-dbt-core-1.5.1/dbt/task/compile.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/task/debug.py` & `in-dbt-core-1.5.1/dbt/task/debug.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/task/deps.py` & `in-dbt-core-1.5.1/dbt/task/deps.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/task/freshness.py` & `in-dbt-core-1.5.1/dbt/task/freshness.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/task/generate.py` & `in-dbt-core-1.5.1/dbt/task/generate.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/task/init.py` & `in-dbt-core-1.5.1/dbt/task/init.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/task/list.py` & `in-dbt-core-1.5.1/dbt/task/list.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/task/printer.py` & `in-dbt-core-1.5.1/dbt/task/printer.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/task/run.py` & `in-dbt-core-1.5.1/dbt/task/run.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/task/run_operation.py` & `in-dbt-core-1.5.1/dbt/task/run_operation.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/task/runnable.py` & `in-dbt-core-1.5.1/dbt/task/runnable.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/task/seed.py` & `in-dbt-core-1.5.1/dbt/task/seed.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/task/serve.py` & `in-dbt-core-1.5.1/dbt/task/serve.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/task/show.py` & `in-dbt-core-1.5.1/dbt/task/show.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/task/snapshot.py` & `in-dbt-core-1.5.1/dbt/task/snapshot.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/task/sql.py` & `in-dbt-core-1.5.1/dbt/task/sql.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/task/test.py` & `in-dbt-core-1.5.1/dbt/task/test.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/tests/fixtures/project.py` & `in-dbt-core-1.5.1/dbt/tests/fixtures/project.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/tests/util.py` & `in-dbt-core-1.5.1/dbt/tests/util.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/tracking.py` & `in-dbt-core-1.5.1/dbt/tracking.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/ui.py` & `in-dbt-core-1.5.1/dbt/ui.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/utils.py` & `in-dbt-core-1.5.1/dbt/utils.py`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/dbt/version.py` & `in-dbt-core-1.5.1/dbt/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,9 +228,9 @@
             # the path is like .../dbt/adapters/{plugin_name}/__version__.py
             # except it could be \\ on windows!
             plugin_root, _ = os.path.split(version_path)
             _, plugin_name = os.path.split(plugin_root)
             yield plugin_name
 
 
-__version__ = "1.5.0"
+__version__ = "1.5.1"
 installed = get_installed_version()
```

### Comparing `in-dbt-core-1.5.0/in_dbt_core.egg-info/PKG-INFO` & `in-dbt-core-1.5.1/in_dbt_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: in-dbt-core
-Version: 1.5.0
+Version: 1.5.1
 Summary: Release for LinkedIn's changes to dbt-core.
 Home-page: https://github.com/linkedin/in-dbt-core
 Author: LinkedIn DBT Team
 Author-email: dbt-eng@linkedin.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: in-dbt-core Version: 1.5.0 Summary: Release for
+Metadata-Version: 2.1 Name: in-dbt-core Version: 1.5.1 Summary: Release for
 LinkedIn's changes to dbt-core. Home-page: https://github.com/linkedin/in-dbt-
 core Author: LinkedIn DBT Team Author-email: dbt-eng@linkedin.com Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `in-dbt-core-1.5.0/in_dbt_core.egg-info/SOURCES.txt` & `in-dbt-core-1.5.1/in_dbt_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `in-dbt-core-1.5.0/setup.py` & `in-dbt-core-1.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md")) as f:
     long_description = f.read()
 
 
 package_name = "in-dbt-core"
-package_version = "1.5.0"
+package_version = "1.5.1"
 description = """Release for LinkedIn's changes to dbt-core."""
 
 
 setup(
     name=package_name,
     version=package_version,
     description=description,
```

