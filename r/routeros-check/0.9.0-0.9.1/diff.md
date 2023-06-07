# Comparing `tmp/routeros-check-0.9.0.tar.gz` & `tmp/routeros-check-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "routeros-check-0.9.0.tar", last modified: Fri Jun  2 11:14:55 2023, max compression
+gzip compressed data, was "routeros-check-0.9.1.tar", last modified: Wed Jun  7 10:54:09 2023, max compression
```

## Comparing `routeros-check-0.9.0.tar` & `routeros-check-0.9.1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:14:55.012930 routeros-check-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-02 11:14:36.000000 routeros-check-0.9.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:14:55.000930 routeros-check-0.9.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:14:55.004930 routeros-check-0.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-02 11:14:36.000000 routeros-check-0.9.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-02 11:14:36.000000 routeros-check-0.9.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-02 11:14:36.000000 routeros-check-0.9.0/.github/workflows/icinga.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-02 11:14:36.000000 routeros-check-0.9.0/.github/workflows/pages.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-02 11:14:36.000000 routeros-check-0.9.0/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-02 11:14:36.000000 routeros-check-0.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-02 11:14:36.000000 routeros-check-0.9.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-02 11:14:36.000000 routeros-check-0.9.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-02 11:14:36.000000 routeros-check-0.9.0/CHANGELOG.md.license
--rw-r--r--   0 runner    (1001) docker     (123)    34916 2023-06-02 11:14:36.000000 routeros-check-0.9.0/LICENSE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:14:55.004930 routeros-check-0.9.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-06-02 11:14:36.000000 routeros-check-0.9.0/LICENSES/CC0-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    34670 2023-06-02 11:14:36.000000 routeros-check-0.9.0/LICENSES/GPL-3.0-or-later.txt
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-02 11:14:36.000000 routeros-check-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    47174 2023-06-02 11:14:55.012930 routeros-check-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-06-02 11:14:36.000000 routeros-check-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-02 11:14:36.000000 routeros-check-0.9.0/README.md.license
--rwxr-xr-x   0 runner    (1001) docker     (123)      159 2023-06-02 11:14:36.000000 routeros-check-0.9.0/check_routeros.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:14:55.004930 routeros-check-0.9.0/config/
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-06-02 11:14:36.000000 routeros-check-0.9.0/config/check_routeros.icinga2.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:14:55.004930 routeros-check-0.9.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    34916 2023-06-02 11:14:36.000000 routeros-check-0.9.0/docs/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-02 11:14:36.000000 routeros-check-0.9.0/docs/cli.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-02 11:14:36.000000 routeros-check-0.9.0/docs/cli.md.license
--rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-06-02 11:14:36.000000 routeros-check-0.9.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-02 11:14:36.000000 routeros-check-0.9.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-02 11:14:36.000000 routeros-check-0.9.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-02 11:14:36.000000 routeros-check-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-02 11:14:36.000000 routeros-check-0.9.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:14:55.008930 routeros-check-0.9.0/routeros_check/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-02 11:14:54.000000 routeros-check-0.9.0/routeros_check/_scm_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:14:55.012930 routeros-check-0.9.0/routeros_check/check/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14759 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/check/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/check/interface_gre.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/check/interface_vrrp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/check/routing_bgp_peer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/check/routing_ospf_neighbor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/check/system_clock.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/check/system_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/check/system_fan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/check/system_license.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/check/system_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     9545 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/check/system_ntp_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/check/system_power.py
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/check/system_psu.py
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/check/system_temperature.py
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/check/system_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/check/system_uptime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/check/tool_ping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/exeption.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    16609 2023-06-02 11:14:36.000000 routeros-check-0.9.0/routeros_check/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:14:55.008930 routeros-check-0.9.0/routeros_check.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    47174 2023-06-02 11:14:54.000000 routeros-check-0.9.0/routeros_check.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-02 11:14:55.000000 routeros-check-0.9.0/routeros_check.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 11:14:54.000000 routeros-check-0.9.0/routeros_check.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-02 11:14:54.000000 routeros-check-0.9.0/routeros_check.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-02 11:14:54.000000 routeros-check-0.9.0/routeros_check.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-02 11:14:54.000000 routeros-check-0.9.0/routeros_check.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 11:14:55.012930 routeros-check-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-02 11:14:36.000000 routeros-check-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 11:14:55.012930 routeros-check-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 11:14:36.000000 routeros-check-0.9.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-02 11:14:36.000000 routeros-check-0.9.0/tests/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-06-02 11:14:36.000000 routeros-check-0.9.0/tests/helpers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-02 11:14:36.000000 routeros-check-0.9.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:54:09.801489 routeros-check-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-07 10:53:53.000000 routeros-check-0.9.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:54:09.793490 routeros-check-0.9.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:54:09.793490 routeros-check-0.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-07 10:53:53.000000 routeros-check-0.9.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-07 10:53:53.000000 routeros-check-0.9.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-07 10:53:53.000000 routeros-check-0.9.1/.github/workflows/icinga.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-07 10:53:53.000000 routeros-check-0.9.1/.github/workflows/pages.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-07 10:53:53.000000 routeros-check-0.9.1/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-07 10:53:53.000000 routeros-check-0.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-07 10:53:53.000000 routeros-check-0.9.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-07 10:53:53.000000 routeros-check-0.9.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-07 10:53:53.000000 routeros-check-0.9.1/CHANGELOG.md.license
+-rw-r--r--   0 runner    (1001) docker     (123)    34916 2023-06-07 10:53:53.000000 routeros-check-0.9.1/LICENSE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:54:09.797490 routeros-check-0.9.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-06-07 10:53:53.000000 routeros-check-0.9.1/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    34670 2023-06-07 10:53:53.000000 routeros-check-0.9.1/LICENSES/GPL-3.0-or-later.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-07 10:53:53.000000 routeros-check-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    47174 2023-06-07 10:54:09.801489 routeros-check-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-06-07 10:53:53.000000 routeros-check-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-07 10:53:53.000000 routeros-check-0.9.1/README.md.license
+-rwxr-xr-x   0 runner    (1001) docker     (123)      159 2023-06-07 10:53:53.000000 routeros-check-0.9.1/check_routeros.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:54:09.797490 routeros-check-0.9.1/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     8325 2023-06-07 10:53:53.000000 routeros-check-0.9.1/config/check_routeros.icinga2.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:54:09.797490 routeros-check-0.9.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    34916 2023-06-07 10:53:53.000000 routeros-check-0.9.1/docs/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-07 10:53:53.000000 routeros-check-0.9.1/docs/cli.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-07 10:53:53.000000 routeros-check-0.9.1/docs/cli.md.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-06-07 10:53:53.000000 routeros-check-0.9.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-07 10:53:53.000000 routeros-check-0.9.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-07 10:53:53.000000 routeros-check-0.9.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-07 10:53:53.000000 routeros-check-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-07 10:53:53.000000 routeros-check-0.9.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:54:09.797490 routeros-check-0.9.1/routeros_check/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-07 10:54:09.000000 routeros-check-0.9.1/routeros_check/_scm_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:54:09.801489 routeros-check-0.9.1/routeros_check/check/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14844 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/check/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/check/interface_gre.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/check/interface_vrrp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/check/routing_bgp_peer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/check/routing_ospf_neighbor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/check/system_clock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/check/system_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/check/system_fan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/check/system_license.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/check/system_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9545 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/check/system_ntp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/check/system_power.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/check/system_psu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/check/system_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/check/system_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/check/system_uptime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/check/tool_ping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/exeption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16609 2023-06-07 10:53:53.000000 routeros-check-0.9.1/routeros_check/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:54:09.797490 routeros-check-0.9.1/routeros_check.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    47174 2023-06-07 10:54:09.000000 routeros-check-0.9.1/routeros_check.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-07 10:54:09.000000 routeros-check-0.9.1/routeros_check.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 10:54:09.000000 routeros-check-0.9.1/routeros_check.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-07 10:54:09.000000 routeros-check-0.9.1/routeros_check.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-07 10:54:09.000000 routeros-check-0.9.1/routeros_check.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-07 10:54:09.000000 routeros-check-0.9.1/routeros_check.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 10:54:09.801489 routeros-check-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-07 10:53:53.000000 routeros-check-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:54:09.801489 routeros-check-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 10:53:53.000000 routeros-check-0.9.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-07 10:53:53.000000 routeros-check-0.9.1/tests/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-06-07 10:53:53.000000 routeros-check-0.9.1/tests/helpers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-07 10:53:53.000000 routeros-check-0.9.1/tox.ini
```

### Comparing `routeros-check-0.9.0/.github/workflows/ci.yml` & `routeros-check-0.9.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.0/.github/workflows/docs.yml` & `routeros-check-0.9.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.0/.github/workflows/icinga.yml` & `routeros-check-0.9.1/.github/workflows/icinga.yml`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.0/.github/workflows/pages.yml` & `routeros-check-0.9.1/.github/workflows/pages.yml`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.0/.github/workflows/pypi.yml` & `routeros-check-0.9.1/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.0/.gitignore` & `routeros-check-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.0/.pre-commit-config.yaml` & `routeros-check-0.9.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.0/CHANGELOG.md` & `routeros-check-0.9.1/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+0.9.1 - 2023-06-07
+------------------
+
+- Fix checks
+  - interface - Fix l2mtu issue on CHR devices
+- Update icinga2 example config
+
 0.9.0 - 2023-06-02
 ------------------
 
 - Add checks
   - system.clock
   - system.ntp.client
 - Update checks to support RouterOS 7.x
```

### Comparing `routeros-check-0.9.0/LICENSE.md` & `routeros-check-0.9.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.0/LICENSES/CC0-1.0.txt` & `routeros-check-0.9.1/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.0/LICENSES/GPL-3.0-or-later.txt` & `routeros-check-0.9.1/LICENSES/GPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.0/PKG-INFO` & `routeros-check-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routeros-check
-Version: 0.9.0
+Version: 0.9.1
 Summary: Monitoring plugin for MikroTik devices for Icinga-Nagios-... 
 Author: DinoTools
 License: ### GNU GENERAL PUBLIC LICENSE
         
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc.
```

### Comparing `routeros-check-0.9.0/README.md` & `routeros-check-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.0/config/check_routeros.icinga2.conf` & `routeros-check-0.9.1/config/check_routeros.icinga2.conf`

 * *Files 27% similar despite different names*

```diff
@@ -75,35 +75,73 @@
 			order = -1
 		}
 	}
 
 	vars.routeros_address = "$check_address$"
 }
 
+
+object CheckCommand "routeros_interface" {
+	import "routeros_command"
+
+	arguments += {
+		"--name" = {
+			value = "$routeros_interface_name$"
+		}
+		"--regex" = {
+			set_if = "$routeros_interface_regex$"
+		}
+		"--single" = {
+			set_if = "$routeros_interface_single$"
+		}
+		"--ignore-disabled" = {
+			set_if = "$routeros_interface_ignore_disabled$"
+		}
+		"--cookie-filename" = {
+			value = "$routeros_interface_cookie_filename$"
+		}
+		"--value-override" = {
+			value = "$routeros_interface_value_override$"
+      repeat_key = true
+		}
+		"--value-warning" = {
+			value = "$routeros_interface_value_warning$"
+      repeat_key = true
+		}
+		"--value-critical" = {
+			value = "$routeros_interface_value_critical$"
+      repeat_key = true
+		}
+	}
+
+	vars.routeros_command = "interface"
+}
+
+
 object CheckCommand "routeros_interface_gre" {
 	import "routeros_command"
 
 	arguments += {
 		"--name" = {
-			value = "$routeros_interface_gre_names$"
+			value = "$routeros_interface_gre_name$"
       repeat_key = true
 		}
 		"--regex" = {
 			set_if = "$routeros_interface_gre_regex$"
 		}
 		"--single" = {
 			set_if = "$routeros_interface_gre_single$"
 		}
 		"--ignore-disabled" = {
-			set_if = "$routeros_interface_ignore_disabled$"
+			set_if = "$routeros_interface_gre_ignore_disabled$"
 		}
 	}
 
 	vars.routeros_command = "interface.gre"
-	vars.routeros_interface_ignore_disabled = true
+	vars.routeros_interface_gre_ignore_disabled = true
 }
 
 object CheckCommand "routeros_interface_vrrp" {
 	import "routeros_command"
 
 	arguments += {
 		"--name" = {
@@ -114,27 +152,27 @@
 			value = "$routeros_interface_vrrp_master$"
 		}
 	}
 
 	vars.routeros_command = "interface.vrrp"
 }
 
-object CheckCommand "routeros_routing_bgp_peers" {
+object CheckCommand "routeros_routing_bgp_peer" {
 	import "routeros_command"
 
 	arguments += {
 		"--name" = {
-			value = "$routeros_routing_bgp_peers_names$"
+			value = "$routeros_routing_bgp_peer_name$"
       repeat_key = true
 		}
 		"--regex" = {
-			set_if = "$routeros_routing_bgp_peers_regex$"
+			set_if = "$routeros_routing_bgp_peer_regex$"
 		}
 		"--single" = {
-			set_if = "$routeros_routing_bgp_peers_single$"
+			set_if = "$routeros_routing_bgp_peer_single$"
 		}
 	}
 
 	vars.routeros_command = "routing.bgp.peers"
 }
 
 
@@ -151,19 +189,80 @@
 			required = true
 		}
 	}
 
 	vars.routeros_command = "routing.ospf.neighbors"
 }
 
+object CheckCommand "routeros_system_clock" {
+	import "routeros_command"
+
+	arguments += {
+		"--warning" = {
+			value = "$routeros_system_clock_warning$"
+		}
+		"--critical" = {
+			value = "$routeros_system_clock_critical$"
+		}
+	}
+
+	vars.routeros_command = "system.clock"
+}
+
+object CheckCommand "routeros_system_cpu" {
+	import "routeros_command"
+
+	arguments += {
+		"--load-warning" = {
+			value = "$routeros_system_cpu_load_warning$"
+		}
+		"--load-critical" = {
+			value = "$routeros_system_cpu_load_critical$"
+		}
+		"--value-warning" = {
+			value = "$routeros_system_cpu_value_warning$"
+      repeat_key = true
+		}
+		"--value-critical" = {
+			value = "$routeros_system_cpu_value_critical$"
+      repeat_key = true
+		}
+		"--regex" = {
+			set_if = "$routeros_system_cpu_regex$"
+		}
+	}
+
+	vars.routeros_command = "system.cpu"
+}
+
+object CheckCommand "routeros_system_fan" {
+	import "routeros_command"
+
+	arguments += {
+		"--value-warning" = {
+			value = "$routeros_system_fan_value_warning$"
+      repeat_key = true
+		}
+		"--value-critical" = {
+			value = "$routeros_system_fan_value_critical$"
+      repeat_key = true
+		}
+		"--regex" = {
+			set_if = "$routeros_system_fan_regex$"
+		}
+	}
+
+	vars.routeros_command = "system.fan"
+}
+
 object CheckCommand "routeros_system_license" {
 	import "routeros_command"
 
 	arguments += {
-		"----deadline-warning" = {
+		"--deadline-warning" = {
 			value = "$routeros_system_licsense_deadline_warning$"
 		}
 		"--deadline-critical" = {
 			value = "$routeros_system_license_deadline_critical$"
 		}
 		"--next-renewal-warning" = {
 			value = "$routeros_system_license_next_renewal_warning$"
@@ -183,26 +282,107 @@
 
 object CheckCommand "routeros_system_memory" {
 	import "routeros_command"
 
 	arguments += {
 		"--warning" = {
 			value = "$routeros_system_memory_warning$"
-			required = true
 		}
 		"--critical" = {
 			value = "$routeros_system_memory_critical$"
-			required = true
 		}
 	}
 
 	vars.routeros_command = "system.memory"
 }
 
 
+object CheckCommand "routeros_system_ntp_client" {
+	import "routeros_command"
+
+	arguments += {
+		"--last-update-before-warning" = {
+			value = "$routeros_system_ntp_client_last_update_before_warning$"
+		}
+		"--last-update-before-critical" = {
+			value = "$routeros_system_ntp_client_last_update_before_critical$"
+		}
+		"--offset-warning" = {
+			value = "$routeros_system_ntp_client_offset_warning$"
+		}
+		"--offset-critical" = {
+			value = "$routeros_system_ntp_client_offset_critical$"
+		}
+		"--stratum-warning" = {
+			value = "$routeros_system_ntp_client_stratum_warning$"
+		}
+		"--stratum-critical" = {
+			value = "$routeros_system_ntp_client_stratum_critical$"
+		}
+		"--expected-server" = {
+			value = "$routeros_system_ntp_client_expected_server$"
+			repeat_key = true
+		}
+	}
+
+	vars.routeros_command = "system.ntp.client"
+}
+
+object CheckCommand "routeros_system_power" {
+	import "routeros_command"
+
+	arguments += {
+		"--warning" = {
+			value = "$routeros_system_power_warning$"
+		}
+		"--critical" = {
+			value = "$routeros_system_power_critical$"
+		}
+	}
+
+	vars.routeros_command = "system.power"
+}
+
+object CheckCommand "routeros_system_psu" {
+	import "routeros_command"
+
+	arguments += {
+		"--value-warning" = {
+			value = "$routeros_system_psu_value_warning$"
+      repeat_key = true
+		}
+		"--value-critical" = {
+			value = "$routeros_system_psu_value_critical$"
+      repeat_key = true
+		}
+	}
+
+	vars.routeros_command = "system.psu"
+}
+
+object CheckCommand "routeros_system_temperature" {
+	import "routeros_command"
+
+	arguments += {
+		"--value-warning" = {
+			value = "$routeros_system_temperature_value_warning$"
+      repeat_key = true
+		}
+		"--value-critical" = {
+			value = "$routeros_system_temperature_value_critical$"
+      repeat_key = true
+		}
+		"--regex" = {
+			set_if = "$routeros_system_temperature_regex$"
+		}
+	}
+
+	vars.routeros_command = "system.temperature"
+}
+
 object CheckCommand "routeros_system_uptime" {
 	import "routeros_command"
 
 	arguments += {
 	}
 
 	vars.routeros_command = "system.uptime"
```

### Comparing `routeros-check-0.9.0/docs/LICENSE.md` & `routeros-check-0.9.1/docs/LICENSE.md`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.0/docs/index.md` & `routeros-check-0.9.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.0/mkdocs.yml` & `routeros-check-0.9.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.0/pyproject.toml` & `routeros-check-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.0/routeros_check/check/interface.py` & `routeros-check-0.9.1/routeros_check/check/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,14 +109,16 @@
                 "uom": "c",
                 "rate": True,
             },
             {
                 "name": "l2mtu",
                 "type": int,
                 "min": 0,
+                # CHR devices don't report l2mtu
+                "missing_ok": True,
             },
             {
                 "name": "link-downs",
                 "type": int,
                 "min": 0,
                 "uom": "c",
             },
```

### Comparing `routeros-check-0.9.0/routeros_check/check/interface_gre.py` & `routeros-check-0.9.1/routeros_check/check/interface_gre.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.0/routeros_check/check/interface_vrrp.py` & `routeros-check-0.9.1/routeros_check/check/interface_vrrp.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.0/routeros_check/check/routing_bgp_peer.py` & `routeros-check-0.9.1/routeros_check/check/routing_bgp_peer.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.0/routeros_check/check/routing_ospf_neighbor.py` & `routeros-check-0.9.1/routeros_check/check/routing_ospf_neighbor.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.0/routeros_check/check/system_clock.py` & `routeros-check-0.9.1/routeros_check/check/system_clock.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.0/routeros_check/check/system_cpu.py` & `routeros-check-0.9.1/routeros_check/check/system_cpu.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.0/routeros_check/check/system_fan.py` & `routeros-check-0.9.1/routeros_check/check/system_fan.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.0/routeros_check/check/system_license.py` & `routeros-check-0.9.1/routeros_check/check/system_license.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.0/routeros_check/check/system_memory.py` & `routeros-check-0.9.1/routeros_check/check/system_memory.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.0/routeros_check/check/system_ntp_client.py` & `routeros-check-0.9.1/routeros_check/check/system_ntp_client.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.0/routeros_check/check/system_power.py` & `routeros-check-0.9.1/routeros_check/check/system_power.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.0/routeros_check/check/system_psu.py` & `routeros-check-0.9.1/routeros_check/check/system_psu.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.0/routeros_check/check/system_temperature.py` & `routeros-check-0.9.1/routeros_check/check/system_temperature.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.0/routeros_check/check/system_update.py` & `routeros-check-0.9.1/routeros_check/check/system_update.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.0/routeros_check/check/system_uptime.py` & `routeros-check-0.9.1/routeros_check/check/system_uptime.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.0/routeros_check/check/tool_ping.py` & `routeros-check-0.9.1/routeros_check/check/tool_ping.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.0/routeros_check/cli.py` & `routeros-check-0.9.1/routeros_check/cli.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.0/routeros_check/context.py` & `routeros-check-0.9.1/routeros_check/context.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.0/routeros_check/helper.py` & `routeros-check-0.9.1/routeros_check/helper.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.0/routeros_check/resource.py` & `routeros-check-0.9.1/routeros_check/resource.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.0/routeros_check.egg-info/PKG-INFO` & `routeros-check-0.9.1/routeros_check.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: routeros-check
-Version: 0.9.0
+Version: 0.9.1
 Summary: Monitoring plugin for MikroTik devices for Icinga-Nagios-... 
 Author: DinoTools
 License: ### GNU GENERAL PUBLIC LICENSE
         
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc.
```

### Comparing `routeros-check-0.9.0/routeros_check.egg-info/SOURCES.txt` & `routeros-check-0.9.1/routeros_check.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.0/tests/base_test.py` & `routeros-check-0.9.1/tests/base_test.py`

 * *Files identical despite different names*

### Comparing `routeros-check-0.9.0/tests/helpers_test.py` & `routeros-check-0.9.1/tests/helpers_test.py`

 * *Files identical despite different names*

