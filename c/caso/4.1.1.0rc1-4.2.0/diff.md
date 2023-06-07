# Comparing `tmp/caso-4.1.1.0rc1.tar.gz` & `tmp/caso-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caso-4.1.1.0rc1.tar", last modified: Mon Apr 10 20:41:03 2023, max compression
+gzip compressed data, was "caso-4.2.0.tar", last modified: Wed Jun  7 09:54:27 2023, max compression
```

## Comparing `caso-4.1.1.0rc1.tar` & `caso-4.2.0.tar`

### file list

```diff
@@ -1,125 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:41:03.258921 caso-4.1.1.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:41:03.246920 caso-4.1.1.0rc1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:41:03.246920 caso-4.1.1.0rc1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/.github/workflows/packaging.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/.github/workflows/python-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/.mailmap
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/.stestr.conf
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/.testr.conf
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-10 20:41:03.000000 caso-4.1.1.0rc1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-10 20:41:03.000000 caso-4.1.1.0rc1/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-10 20:41:03.258921 caso-4.1.1.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:41:03.246920 caso-4.1.1.0rc1/caso/
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:41:03.250921 caso-4.1.1.0rc1/caso/_cmd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/_cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/_cmd/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/_cmd/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:41:03.250921 caso-4.1.1.0rc1/caso/extract/
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/extract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/extract/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11174 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/extract/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:41:03.250921 caso-4.1.1.0rc1/caso/extract/openstack/
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/extract/openstack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/extract/openstack/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/extract/openstack/cinder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/extract/openstack/neutron.py
--rw-r--r--   0 runner    (1001) docker     (123)    19575 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/extract/openstack/nova.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/keystone_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:41:03.250921 caso-4.1.1.0rc1/caso/messenger/
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/messenger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/messenger/logstash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/messenger/noop.py
--rw-r--r--   0 runner    (1001) docker     (123)     8099 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/messenger/ssm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/opts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10056 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/record.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:41:03.250921 caso-4.1.1.0rc1/caso/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:41:03.250921 caso-4.1.1.0rc1/caso/tests/extract/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/tests/extract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/tests/extract/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/tests/extract/test_nova.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/tests/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/caso/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:41:03.250921 caso-4.1.1.0rc1/caso.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-10 20:41:03.000000 caso-4.1.1.0rc1/caso.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-10 20:41:03.000000 caso-4.1.1.0rc1/caso.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 20:41:03.000000 caso-4.1.1.0rc1/caso.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-10 20:41:03.000000 caso-4.1.1.0rc1/caso.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 20:41:03.000000 caso-4.1.1.0rc1/caso.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-10 20:41:03.000000 caso-4.1.1.0rc1/caso.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-10 20:41:03.000000 caso-4.1.1.0rc1/caso.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-10 20:41:03.000000 caso-4.1.1.0rc1/caso.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:41:03.250921 caso-4.1.1.0rc1/doc/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/doc/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:41:03.254921 caso-4.1.1.0rc1/doc/source/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2980 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/doc/source/configuration-file.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13983 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/doc/source/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/doc/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/doc/source/multi-region.rst
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/doc/source/release-notes.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:41:03.254921 caso-4.1.1.0rc1/doc/source/static/
--rw-r--r--   0 runner    (1001) docker     (123)    58956 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/doc/source/static/caso-diagram.drawio
--rw-r--r--   0 runner    (1001) docker     (123)   111404 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/doc/source/static/caso-diagram.png
--rw-r--r--   0 runner    (1001) docker     (123)    15375 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/doc/source/static/caso.conf.sample
--rw-r--r--   0 runner    (1001) docker     (123)    15964 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/doc/source/static/caso.png
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/doc/source/troubleshooting.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/doc/source/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:41:03.242920 caso-4.1.1.0rc1/etc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:41:03.254921 caso-4.1.1.0rc1/etc/caso/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/etc/caso/caso-config-generator.conf
--rw-r--r--   0 runner    (1001) docker     (123)    15605 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/etc/caso/caso.conf.sample
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/etc/caso/voms.json.sample
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:41:03.242920 caso-4.1.1.0rc1/packaging/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:41:03.254921 caso-4.1.1.0rc1/packaging/debian/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/packaging/debian/README.Debian
--rw-r--r--   0 runner    (1001) docker     (123)    10681 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/packaging/debian/changelog
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/packaging/debian/clean
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/packaging/debian/compat
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/packaging/debian/control
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/packaging/debian/copyright
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/packaging/debian/cron.hourly
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/packaging/debian/gbp.conf
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/packaging/debian/postinst
--rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/packaging/debian/rules
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:41:03.254921 caso-4.1.1.0rc1/packaging/debian/source/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/packaging/debian/source/format
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:41:03.254921 caso-4.1.1.0rc1/packaging/redhat/
--rw-r--r--   0 runner    (1001) docker     (123)     8740 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/packaging/redhat/caso.spec
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:41:03.242920 caso-4.1.1.0rc1/releasenotes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 20:41:03.258921 caso-4.1.1.0rc1/releasenotes/notes/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/releasenotes/notes/allow-to-load-an-extractor-list-fd1f6905d0d01383.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/releasenotes/notes/default-to-all-extractors-0da9448a00091bc1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/releasenotes/notes/deprecate-voms-mapping-80cfda2246ec43e9.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/releasenotes/notes/gpu-accounting-082a62b7254d29bd.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/releasenotes/notes/multi-region-support-4395450dfbc4e8a3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/releasenotes/notes/new-release-notes-b79c3d7a778fc946.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/releasenotes/notes/new-ussuri-configuration-03b764a39f461eda.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/releasenotes/notes/option-deprecation-a4eba5fa1a362815.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/releasenotes/notes/refactor-extractor-e826c64087e17065.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/releasenotes/notes/require-system-scope-67d0d11681beea27.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/releasenotes/notes/support-for-storage-34675eff431608d1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/releasenotes/notes/tags-for-projects-3b9b6b5a92bcc6df.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-10 20:41:03.258921 caso-4.1.1.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-04-10 20:40:53.000000 caso-4.1.1.0rc1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:54:27.410450 caso-4.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-07 09:54:09.000000 caso-4.2.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:54:27.394449 caso-4.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-07 09:54:09.000000 caso-4.2.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-07 09:54:09.000000 caso-4.2.0/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:54:27.398449 caso-4.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-07 09:54:09.000000 caso-4.2.0/.github/workflows/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-06-07 09:54:09.000000 caso-4.2.0/.github/workflows/packaging.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-07 09:54:09.000000 caso-4.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-07 09:54:09.000000 caso-4.2.0/.github/workflows/python-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-07 09:54:09.000000 caso-4.2.0/.mailmap
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-07 09:54:09.000000 caso-4.2.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-07 09:54:09.000000 caso-4.2.0/.stestr.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-07 09:54:09.000000 caso-4.2.0/.testr.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-07 09:54:09.000000 caso-4.2.0/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-07 09:54:27.000000 caso-4.2.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-07 09:54:09.000000 caso-4.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-06-07 09:54:09.000000 caso-4.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-07 09:54:27.000000 caso-4.2.0/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-06-07 09:54:09.000000 caso-4.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-07 09:54:09.000000 caso-4.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-06-07 09:54:27.410450 caso-4.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-07 09:54:09.000000 caso-4.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:54:27.398449 caso-4.2.0/caso/
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-07 09:54:09.000000 caso-4.2.0/caso/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:54:27.398449 caso-4.2.0/caso/_cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 09:54:09.000000 caso-4.2.0/caso/_cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-07 09:54:09.000000 caso-4.2.0/caso/_cmd/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-06-07 09:54:09.000000 caso-4.2.0/caso/_cmd/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-06-07 09:54:09.000000 caso-4.2.0/caso/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-07 09:54:09.000000 caso-4.2.0/caso/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:54:27.398449 caso-4.2.0/caso/extract/
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-07 09:54:09.000000 caso-4.2.0/caso/extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-07 09:54:09.000000 caso-4.2.0/caso/extract/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-06-07 09:54:09.000000 caso-4.2.0/caso/extract/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:54:27.398449 caso-4.2.0/caso/extract/openstack/
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-07 09:54:09.000000 caso-4.2.0/caso/extract/openstack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-06-07 09:54:09.000000 caso-4.2.0/caso/extract/openstack/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-06-07 09:54:09.000000 caso-4.2.0/caso/extract/openstack/cinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-06-07 09:54:09.000000 caso-4.2.0/caso/extract/openstack/neutron.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19575 2023-06-07 09:54:09.000000 caso-4.2.0/caso/extract/openstack/nova.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-07 09:54:09.000000 caso-4.2.0/caso/keystone_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-06-07 09:54:09.000000 caso-4.2.0/caso/loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-06-07 09:54:09.000000 caso-4.2.0/caso/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:54:27.402449 caso-4.2.0/caso/messenger/
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-07 09:54:09.000000 caso-4.2.0/caso/messenger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-07 09:54:09.000000 caso-4.2.0/caso/messenger/logstash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-07 09:54:09.000000 caso-4.2.0/caso/messenger/noop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-06-07 09:54:09.000000 caso-4.2.0/caso/messenger/ssm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-07 09:54:09.000000 caso-4.2.0/caso/opts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13496 2023-06-07 09:54:09.000000 caso-4.2.0/caso/record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:54:27.402449 caso-4.2.0/caso/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-07 09:54:09.000000 caso-4.2.0/caso/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-07 09:54:09.000000 caso-4.2.0/caso/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26533 2023-06-07 09:54:09.000000 caso-4.2.0/caso/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:54:27.402449 caso-4.2.0/caso/tests/extract/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-07 09:54:09.000000 caso-4.2.0/caso/tests/extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-06-07 09:54:09.000000 caso-4.2.0/caso/tests/extract/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-06-07 09:54:09.000000 caso-4.2.0/caso/tests/extract/test_nova.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-07 09:54:09.000000 caso-4.2.0/caso/tests/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-06-07 09:54:09.000000 caso-4.2.0/caso/tests/test_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6966 2023-06-07 09:54:09.000000 caso-4.2.0/caso/tests/test_ssm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-07 09:54:09.000000 caso-4.2.0/caso/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:54:27.398449 caso-4.2.0/caso.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-06-07 09:54:27.000000 caso-4.2.0/caso.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-06-07 09:54:27.000000 caso-4.2.0/caso.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 09:54:27.000000 caso-4.2.0/caso.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-07 09:54:27.000000 caso-4.2.0/caso.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 09:54:27.000000 caso-4.2.0/caso.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-07 09:54:27.000000 caso-4.2.0/caso.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-07 09:54:27.000000 caso-4.2.0/caso.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-07 09:54:27.000000 caso-4.2.0/caso.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:54:27.402449 caso-4.2.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-07 09:54:09.000000 caso-4.2.0/doc/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:54:27.406449 caso-4.2.0/doc/source/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2980 2023-06-07 09:54:09.000000 caso-4.2.0/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-07 09:54:09.000000 caso-4.2.0/doc/source/configuration-file.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13983 2023-06-07 09:54:09.000000 caso-4.2.0/doc/source/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-07 09:54:09.000000 caso-4.2.0/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-07 09:54:09.000000 caso-4.2.0/doc/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-07 09:54:09.000000 caso-4.2.0/doc/source/multi-region.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-07 09:54:09.000000 caso-4.2.0/doc/source/release-notes.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:54:27.406449 caso-4.2.0/doc/source/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    58956 2023-06-07 09:54:09.000000 caso-4.2.0/doc/source/static/caso-diagram.drawio
+-rw-r--r--   0 runner    (1001) docker     (123)   111404 2023-06-07 09:54:09.000000 caso-4.2.0/doc/source/static/caso-diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15375 2023-06-07 09:54:09.000000 caso-4.2.0/doc/source/static/caso.conf.sample
+-rw-r--r--   0 runner    (1001) docker     (123)    15964 2023-06-07 09:54:09.000000 caso-4.2.0/doc/source/static/caso.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-07 09:54:09.000000 caso-4.2.0/doc/source/troubleshooting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-06-07 09:54:09.000000 caso-4.2.0/doc/source/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:54:27.394449 caso-4.2.0/etc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:54:27.406449 caso-4.2.0/etc/caso/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-07 09:54:09.000000 caso-4.2.0/etc/caso/caso-config-generator.conf
+-rw-r--r--   0 runner    (1001) docker     (123)    15605 2023-06-07 09:54:09.000000 caso-4.2.0/etc/caso/caso.conf.sample
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-07 09:54:09.000000 caso-4.2.0/etc/caso/voms.json.sample
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-07 09:54:09.000000 caso-4.2.0/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:54:27.394449 caso-4.2.0/packaging/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:54:27.406449 caso-4.2.0/packaging/debian/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-07 09:54:09.000000 caso-4.2.0/packaging/debian/README.Debian
+-rw-r--r--   0 runner    (1001) docker     (123)    11260 2023-06-07 09:54:09.000000 caso-4.2.0/packaging/debian/changelog
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-07 09:54:09.000000 caso-4.2.0/packaging/debian/clean
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-07 09:54:09.000000 caso-4.2.0/packaging/debian/compat
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-07 09:54:09.000000 caso-4.2.0/packaging/debian/control
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-06-07 09:54:09.000000 caso-4.2.0/packaging/debian/copyright
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-07 09:54:09.000000 caso-4.2.0/packaging/debian/cron.hourly
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-07 09:54:09.000000 caso-4.2.0/packaging/debian/gbp.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-07 09:54:09.000000 caso-4.2.0/packaging/debian/postinst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      157 2023-06-07 09:54:09.000000 caso-4.2.0/packaging/debian/rules
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:54:27.406449 caso-4.2.0/packaging/debian/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 09:54:09.000000 caso-4.2.0/packaging/debian/source/format
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:54:27.406449 caso-4.2.0/packaging/redhat/
+-rw-r--r--   0 runner    (1001) docker     (123)     9046 2023-06-07 09:54:09.000000 caso-4.2.0/packaging/redhat/caso.spec
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:54:27.394449 caso-4.2.0/releasenotes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:54:27.410450 caso-4.2.0/releasenotes/notes/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-07 09:54:09.000000 caso-4.2.0/releasenotes/notes/allow-to-load-an-extractor-list-fd1f6905d0d01383.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-07 09:54:09.000000 caso-4.2.0/releasenotes/notes/default-to-all-extractors-0da9448a00091bc1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-07 09:54:09.000000 caso-4.2.0/releasenotes/notes/deprecate-voms-mapping-80cfda2246ec43e9.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-07 09:54:09.000000 caso-4.2.0/releasenotes/notes/fix-timestamps-84cd81de7d26e164.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-07 09:54:09.000000 caso-4.2.0/releasenotes/notes/gpu-accounting-082a62b7254d29bd.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-07 09:54:09.000000 caso-4.2.0/releasenotes/notes/multi-region-support-4395450dfbc4e8a3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-07 09:54:09.000000 caso-4.2.0/releasenotes/notes/new-release-notes-b79c3d7a778fc946.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-07 09:54:09.000000 caso-4.2.0/releasenotes/notes/new-ussuri-configuration-03b764a39f461eda.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-07 09:54:09.000000 caso-4.2.0/releasenotes/notes/option-deprecation-a4eba5fa1a362815.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-07 09:54:09.000000 caso-4.2.0/releasenotes/notes/refactor-extractor-e826c64087e17065.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-07 09:54:09.000000 caso-4.2.0/releasenotes/notes/require-system-scope-67d0d11681beea27.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-07 09:54:09.000000 caso-4.2.0/releasenotes/notes/support-for-storage-34675eff431608d1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-07 09:54:09.000000 caso-4.2.0/releasenotes/notes/tags-for-projects-3b9b6b5a92bcc6df.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-07 09:54:09.000000 caso-4.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-06-07 09:54:27.410450 caso-4.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-07 09:54:09.000000 caso-4.2.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-06-07 09:54:09.000000 caso-4.2.0/tox.ini
```

### Comparing `caso-4.1.1.0rc1/.github/PULL_REQUEST_TEMPLATE.md` & `caso-4.2.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/.github/workflows/python-publish.yml` & `caso-4.2.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/.github/workflows/python-test.yml` & `caso-4.2.0/.github/workflows/python-test.yml`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/.readthedocs.yml` & `caso-4.2.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/CODE_OF_CONDUCT.md` & `caso-4.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/CONTRIBUTING.md` & `caso-4.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/LICENSE` & `caso-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/PKG-INFO` & `caso-4.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caso
-Version: 4.1.1.0rc1
+Version: 4.2.0
 Summary: cASO is an OpenStack Accounting extractor.
 Home-page: http://github.com/IFCA/caso
 Author: Alvaro Lopez Garcia
 Author-email: aloga@ifca.unican.es
 License: Apache-2
 Project-URL: Bug Tracker, https://github.com/IFCA/caso/issues
 Project-URL: Documentation, https://caso.readthedocs.io/
```

### Comparing `caso-4.1.1.0rc1/README.md` & `caso-4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/caso/__init__.py` & `caso-4.2.0/caso/__init__.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/caso/_cmd/extract.py` & `caso-4.2.0/caso/_cmd/extract.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/caso/_cmd/projects.py` & `caso-4.2.0/caso/_cmd/projects.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/caso/config.py` & `caso-4.2.0/caso/config.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/caso/exception.py` & `caso-4.2.0/caso/exception.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/caso/extract/__init__.py` & `caso-4.2.0/caso/extract/__init__.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/caso/extract/base.py` & `caso-4.2.0/caso/extract/base.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/caso/extract/manager.py` & `caso-4.2.0/caso/extract/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     cfg.StrOpt(
         "caso_tag",
         default="caso",
         help="Tag used to mark a project in Keystone to be extracted by cASO",
     ),
     cfg.StrOpt(
         "vo_property",
-        default="accounting:VO",
+        default="VO",
         help="Property key used to get the VO name from the project properties. ",
     ),
     cfg.StrOpt(
         "mapping_file",
         default="/etc/caso/voms.json",
         deprecated_group="extractor",
         deprecated_for_removal=True,
```

### Comparing `caso-4.1.1.0rc1/caso/extract/openstack/__init__.py` & `caso-4.2.0/caso/extract/openstack/__init__.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/caso/extract/openstack/base.py` & `caso-4.2.0/caso/extract/openstack/base.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/caso/extract/openstack/cinder.py` & `caso-4.2.0/caso/extract/openstack/cinder.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/caso/extract/openstack/neutron.py` & `caso-4.2.0/caso/extract/openstack/neutron.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
                 continue
             else:
                 if ip_version == 4:
                     ip_counts_v4[user] += 1
                 elif ip_version == 6:
                     ip_counts_v6[user] += 1
 
-        for (ip_version, ip_counts) in [(4, ip_counts_v4), (6, ip_counts_v6)]:
+        for ip_version, ip_counts in [(4, ip_counts_v4), (6, ip_counts_v6)]:
             for user_id, count in ip_counts.items():
                 if count == 0:
                     continue
 
                 self.ip_records[user_id] = self._build_ip_record(
                     user_id, count, ip_version
                 )
```

### Comparing `caso-4.1.1.0rc1/caso/extract/openstack/nova.py` & `caso-4.2.0/caso/extract/openstack/nova.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/caso/keystone_client.py` & `caso-4.2.0/caso/keystone_client.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/caso/loading.py` & `caso-4.2.0/caso/loading.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/caso/manager.py` & `caso-4.2.0/caso/manager.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/caso/messenger/__init__.py` & `caso-4.2.0/caso/messenger/__init__.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/caso/messenger/logstash.py` & `caso-4.2.0/caso/messenger/logstash.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/caso/messenger/noop.py` & `caso-4.2.0/caso/messenger/noop.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/caso/messenger/ssm.py` & `caso-4.2.0/caso/messenger/ssm.py`

 * *Files 22% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 
 # We are not parsing XML so this is safe
 import xml.etree.ElementTree as ETree  # nosec
 
 import dirq.QueueSimple
 from oslo_config import cfg
 from oslo_log import log
-import six
 
 import caso.exception
 import caso.messenger
 import caso.record
 from caso import utils
 
 LOG = log.getLogger(__name__)
@@ -65,107 +64,80 @@
     def __init__(self):
         """Initialize the SSM messenger with configured values."""
         try:
             utils.makedirs(CONF.ssm.output_path)
         except Exception as err:
             LOG.error(f"Failed to create path {CONF.ssm.output_path} because {err}")
             raise err
+        self.queue = dirq.QueueSimple.QueueSimple(CONF.ssm.output_path)
 
-    def _push_message_cloud(
-        self, queue: dirq.QueueSimple.QueueSimple, entries: typing.List[str]
-    ):
+    def _push_message_cloud(self, entries: typing.List[str]):
         """Push a compute message, formatted following the CloudRecord."""
         message = f"APEL-cloud-message: v{self.version_cloud}\n"
-        aux = "%%\n".join(entries)
+        aux = "\n%%\n".join(entries)
         message += f"{aux}\n"
-        queue.add(message.encode("utf-8"))
+        self.queue.add(message.encode("utf-8"))
 
     def _push_message_json(
         self,
-        queue: dirq.QueueSimple.QueueSimple,
         entries: typing.List[str],
         msg_type: str,
         version: str,
     ):
         """Push a JSON message with a UsageRecords list."""
         message = {
             "Type": msg_type,
             "Version": version,
             "UsageRecords": [json.loads(r) for r in entries],
         }
-        queue.add(json.dumps(message))
+        self.queue.add(json.dumps(message))
 
-    def _push_message_ip(
-        self, queue: dirq.QueueSimple.QueueSimple, entries: typing.List[str]
-    ):
+    def _push_message_ip(self, entries: typing.List[str]):
         """Push an IP message."""
-        self._push_message_json(
-            queue, entries, "APEL Public IP message", self.version_ip
-        )
+        self._push_message_json(entries, "APEL Public IP message", self.version_ip)
 
-    def _push_message_accelerator(
-        self, queue: dirq.QueueSimple.QueueSimple, entries: typing.List[str]
-    ):
+    def _push_message_accelerator(self, entries: typing.List[str]):
         """Push an accelerator message."""
         self._push_message_json(
-            queue, entries, "APEL-accelerator-message", self.version_accelerator
+            entries, "APEL-accelerator-message", self.version_accelerator
         )
 
-    def _push_message_storage(self, queue, entries):
+    def _push_message_storage(self, entries):
         """Push a storage message."""
-        ns = {"xmlns:sr": "http://eu-emi.eu/namespaces/2011/02/storagerecord"}
-        root = ETree.Element("sr:StorageUsageRecords", attrib=ns)
+        ETree.register_namespace(
+            "sr", "http://eu-emi.eu/namespaces/2011/02/storagerecord"
+        )
+        root = ETree.Element("sr:StorageUsageRecords")
         for record in entries:
-            sr = ETree.SubElement(root, "sr:StorageUsageRecord")
-            ETree.SubElement(
-                sr,
-                "sr:RecordIdentity",
-                attrib={
-                    "sr:createTime": record.measure_time.isoformat(),
-                    "sr:recordId": str(record.uuid),
-                },
-            )
-            ETree.SubElement(sr, "sr:StorageSystem").text = record.compute_service
-            ETree.SubElement(sr, "sr:Site").text = record.site_name
-            subject = ETree.SubElement(sr, "sr:SubjectIdentity")
-            ETree.SubElement(subject, "sr:LocalUser").text = record.user_id
-            ETree.SubElement(subject, "sr:LocalGroup").text = record.group_id
-            if record.user_dn:
-                ETree.SubElement(subject, "sr:UserIdentity").text = record.user_dn
-            if record.fqan:
-                ETree.SubElement(subject, "sr:Group").text = record.fqan
-            ETree.SubElement(sr, "sr:StartTime").text = record.start_time.isoformat()
-            ETree.SubElement(sr, "sr:EndTime").text = record.measure_time.isoformat()
-            capacity = str(int(record.capacity * 1073741824))  # 1 GiB = 2^30
-            ETree.SubElement(sr, "sr:ResourceCapacityUsed").text = capacity
-        queue.add(ETree.tostring(root))
+            # We are not parsing XML so this is safe
+            sr = ETree.fromstring(record)  # nosec
+            root.append(sr)
+        self.queue.add(ETree.tostring(root))
 
     def _push(self, entries_cloud, entries_ip, entries_accelerator, entries_storage):
         """Push all messages, dividing them into smaller chunks.
 
         This method gets lists of messages to be pushed in smaller chucks as per GGUS
         ticket 143436: https://ggus.eu/index.php?mode=ticket_info&ticket_id=143436
         """
-        queue = dirq.QueueSimple.QueueSimple(CONF.ssm.output_path)
-
         for i in range(0, len(entries_cloud), CONF.ssm.max_size):
             entries = entries_cloud[i : i + CONF.ssm.max_size]  # noqa(E203)
-            self._push_message_cloud(queue, entries)
+            self._push_message_cloud(entries)
 
         for i in range(0, len(entries_ip), CONF.ssm.max_size):
             entries = entries_ip[i : i + CONF.ssm.max_size]  # noqa(E203)
-            self._push_message_ip(queue, entries)
+            self._push_message_ip(entries)
 
         for i in range(0, len(entries_accelerator), CONF.ssm.max_size):
             entries = entries_accelerator[i : i + CONF.ssm.max_size]  # noqa(E203)
-            self._push_message_accelerator(queue, entries)
+            self._push_message_accelerator(entries)
 
         for i in range(0, len(entries_storage), CONF.ssm.max_size):
             entries = entries_storage[i : i + CONF.ssm.max_size]  # noqa(E203)
-            self._push_message_storage(queue, entries)
+            self._push_message_storage(entries)
 
     def push(self, records):
         """Push all records to SSM.
 
         This includes pushing the following records:
             - Cloud records
             - IP records
@@ -178,32 +150,23 @@
         if not records:
             return
 
         entries_cloud = []
         entries_ip = []
         entries_accelerator = []
         entries_storage = []
-        opts = {
-            "by_alias": True,
-            "exclude_unset": True,
-            "exclude_none": True,
-        }
         for record in records:
             if isinstance(record, caso.record.CloudRecord):
-                aux = ""
-                for k, v in six.iteritems(record.dict(**opts)):
-                    if v is not None:
-                        aux += f"{k}: {v}\n"
-                entries_cloud.append(aux)
+                entries_cloud.append(record.ssm_message())
             elif isinstance(record, caso.record.IPRecord):
-                entries_ip.append(record.json(**opts))
+                entries_ip.append(record.ssm_message())
             elif isinstance(record, caso.record.AcceleratorRecord):
-                entries_accelerator.append(record.json(**opts))
+                entries_accelerator.append(record.ssm_message())
             elif isinstance(record, caso.record.StorageRecord):
-                entries_storage.append(record)
+                entries_storage.append(record.ssm_message())
             else:
                 raise caso.exception.CasoError("Unexpected record format!")
 
         self._push(entries_cloud, entries_ip, entries_accelerator, entries_storage)
 
 
 class SSMMessengerV04(SSMMessenger):
```

### Comparing `caso-4.1.1.0rc1/caso/opts.py` & `caso-4.2.0/caso/opts.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/caso/record.py` & `caso-4.2.0/caso/record.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,52 +14,72 @@
 # License for the specific language governing permissions and limitations
 # under the License.
 
 """Module containing all the cloud accounting records."""
 
 import abc
 import datetime
+import enum
+import json
 import typing
 import uuid as m_uuid
 
+# We are not parsing XML so this is safe
+import xml.etree.ElementTree as ETree  # nosec
+
 import pydantic
 
 import caso
 from oslo_log import log
 
 LOG = log.getLogger(__name__)
 
 
 class _BaseRecord(pydantic.BaseModel, abc.ABC):
     """This is the base cASO record object."""
 
-    version: str
+    version: str = pydantic.Field(..., exclude=True)
 
     site_name: str
-    cloud_type = caso.user_agent
+    cloud_type: str = caso.user_agent
     compute_service: str
 
+    @abc.abstractmethod
+    def ssm_message(self):
+        """Render record as the expected SSM message."""
+        raise NotImplementedError("Method not implemented")
+
+
+class _ValidCloudStatus(str, enum.Enum):
+    started = "started"
+    completed = "completed"
+    error = "error"
+    paused = "paused"
+    suspended = "suspended"
+    stopped = "stopped"
+    unknown = "unknown"
+
 
 class CloudRecord(_BaseRecord):
     """The CloudRecord class holds information for each of the records.
 
     This class is versioned, following the Cloud Accounting Record versions.
     """
 
-    version: str = "0.4"
+    version: str = pydantic.Field("0.4", exclude=True)
 
     uuid: m_uuid.UUID
     name: str
 
     user_id: str
     user_dn: typing.Optional[str]
     group_id: str
     fqan: str
 
-    status: str
+    status: _ValidCloudStatus
 
     image_id: typing.Optional[str]
 
     public_ip_count = 0
     cpu_count: int
     memory: int
     disk: int
@@ -103,14 +123,29 @@
             duration = int(duration)
         return duration
 
     def set_cpu_duration(self, value: int):
         """Set the CPU duration for the record."""
         self._cpu_duration = value
 
+    def ssm_message(self):
+        """Render record as the expected SSM message."""
+        opts = {
+            "by_alias": True,
+            "exclude_none": True,
+        }
+        # NOTE(aloga): do not iter over the dictionary returned by record.dict() as this
+        # is just a dictionary representation of the object, where no serialization is
+        # done. In order to get objects correctly serialized we need to convert to JSON,
+        # then reload the model
+        serialized_record = json.loads(self.json(**opts))
+        aux = [f"{k}: {v}" for k, v in serialized_record.items()]
+        aux.sort()
+        return "\n".join(aux)
+
     class Config:
         """Config class for Pydantic."""
 
         @staticmethod
         def map_fields(value: str) -> str:
             """Map object fields to Cloud Accounting Record fields."""
             d = {
@@ -139,40 +174,49 @@
                 "public_ip_count": "PublicIPCount",
                 "benchmark_value": "Benchmark",
                 "benchmark_type": "BenchmarkType",
                 "compute_service": "CloudComputeService",
             }
             return d.get(value, value)
 
+        json_encoders = {datetime.datetime: lambda v: int(v.timestamp())}
         alias_generator = map_fields
         allow_population_by_field_name = True
         underscore_attrs_are_private = True
         extra = "forbid"
 
 
 class IPRecord(_BaseRecord):
     """The IPRecord class holds information for each of the records.
 
     This class is versioned, following the Public IP Usage Record versions.
     """
 
-    version = "0.2"
+    version: str = pydantic.Field("0.2", exclude=True)
 
     uuid: m_uuid.UUID
 
     user_id: typing.Optional[str]
     user_dn: typing.Optional[str]
     group_id: str
     fqan: str
 
     measure_time: datetime.datetime
 
     ip_version: int
     public_ip_count: int
 
+    def ssm_message(self):
+        """Render record as the expected SSM message."""
+        opts = {
+            "by_alias": True,
+            "exclude_none": True,
+        }
+        return self.json(**opts)
+
     class Config:
         """Config class for Pydantic."""
 
         @staticmethod
         def map_fields(field: str) -> str:
             """Map object fields to accounting Public IP Usage record fields."""
             d = {
@@ -185,28 +229,29 @@
                 "user_dn": "GlobalUserName",
                 "ip_version": "IPVersion",
                 "public_ip_count": "IPCount",
                 "compute_service": "CloudComputeService",
             }
             return d.get(field, field)
 
+        json_encoders = {datetime.datetime: lambda v: int(v.timestamp())}
         alias_generator = map_fields
         allow_population_by_field_name = True
         underscore_attrs_are_private = True
         extra = "forbid"
 
 
 class AcceleratorRecord(_BaseRecord):
     """The AcceleratorRecord class holds information for each of the records.
 
     This class is versioned, following the Accelerator Usage Record versions
 
     """
 
-    version = "0.1"
+    version: str = pydantic.Field("0.1", exclude=True)
 
     uuid: m_uuid.UUID
 
     user_dn: typing.Optional[str]
     fqan: str
 
     count: int
@@ -232,14 +277,22 @@
             return self._active_duration
         return self.available_duration
 
     def set_active_duration(self, value: int):
         """Set the active duration for the record."""
         self._active_duration = value
 
+    def ssm_message(self):
+        """Render record as the expected SSM message."""
+        opts = {
+            "by_alias": True,
+            "exclude_none": True,
+        }
+        return self.json(**opts)
+
     class Config:
         """Config class for Pydantic."""
 
         @staticmethod
         def map_fields(field: str) -> str:
             """Map object fields to accounting Accelerator Usage Record fields."""
             d = {
@@ -254,31 +307,34 @@
                 "cores": "Cores",
                 "active_duration": "ActiveDuration",
                 "available_duration": "AvailableDuration",
                 "benchmark_type": "BenchmarkType",
                 "benchmark": "Benchmark",
                 "accelerator_type": "Type",
                 "model": "Model",
+                "cloud_type": "CloudType",
+                "compute_service": "CloudComputeService",
             }
             return d.get(field, field)
 
+        json_encoders = {datetime.datetime: lambda v: int(v.timestamp())}
         alias_generator = map_fields
         allow_population_by_field_name = True
         underscore_attrs_are_private = True
         extra = "forbid"
 
 
 class StorageRecord(_BaseRecord):
     """The StorageRecord class holds information for each of the records.
 
     This class is versioned, following the Storage Accounting Definition on
     EMI StAR
     """
 
-    version: str = "0.1"
+    version: str = pydantic.Field("0.1", exclude=True)
 
     uuid: m_uuid.UUID
     name: str
 
     user_id: str
     user_dn: typing.Optional[str]
     group_id: str
@@ -299,14 +355,41 @@
     @classmethod
     @pydantic.validator("attached_duration", always=True)
     def _validate_attached_duration(cls, value):
         if value is not None:
             return value
         return 0
 
+    def ssm_message(self):
+        """Render record as the expected SSM message."""
+        ns = {"xmlns:sr": "http://eu-emi.eu/namespaces/2011/02/storagerecord"}
+        sr = ETree.Element("sr:StorageUsageRecord", attrib=ns)
+        ETree.SubElement(
+            sr,
+            "sr:RecordIdentity",
+            attrib={
+                "sr:createTime": self.measure_time.isoformat(),
+                "sr:recordId": str(self.uuid),
+            },
+        )
+        ETree.SubElement(sr, "sr:StorageSystem").text = self.compute_service
+        ETree.SubElement(sr, "sr:Site").text = self.site_name
+        subject = ETree.SubElement(sr, "sr:SubjectIdentity")
+        ETree.SubElement(subject, "sr:LocalUser").text = self.user_id
+        ETree.SubElement(subject, "sr:LocalGroup").text = self.group_id
+        if self.user_dn:
+            ETree.SubElement(subject, "sr:UserIdentity").text = self.user_dn
+        if self.fqan:
+            ETree.SubElement(subject, "sr:Group").text = self.fqan
+        ETree.SubElement(sr, "sr:StartTime").text = self.start_time.isoformat()
+        ETree.SubElement(sr, "sr:EndTime").text = self.measure_time.isoformat()
+        capacity = str(int(self.capacity * 1073741824))  # 1 GiB = 2^30
+        ETree.SubElement(sr, "sr:ResourceCapacityUsed").text = capacity
+        return ETree.tostring(sr)
+
     class Config:
         """Config class for Pydantic."""
 
         @staticmethod
         def map_fields(field: str) -> str:
             """Map object fields to accounting EMI StAR record values."""
             d = {
@@ -321,14 +404,15 @@
                 "capacity": "Capacity",
                 "active_duration": "ActiveDuration",
                 "start_time": "StartTime",
                 "storage_type": "Type",
                 "status": "Status",
                 "attached_to": "AttachedTo",
                 "attached_duration": "AttachedDuration",
+                "cloud_type": "CloudType",
                 "compute_service": "CloudComputeService",
             }
             return d.get(field, field)
 
         alias_generator = map_fields
         allow_population_by_field_name = True
         underscore_attrs_are_private = True
```

### Comparing `caso-4.1.1.0rc1/caso/tests/base.py` & `caso-4.2.0/caso/tests/base.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/caso/tests/extract/test_manager.py` & `caso-4.2.0/caso/tests/extract/test_manager.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/caso/tests/extract/test_nova.py` & `caso-4.2.0/caso/tests/extract/test_nova.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/caso/tests/test_manager.py` & `caso-4.2.0/caso/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/caso/utils.py` & `caso-4.2.0/caso/utils.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/caso.egg-info/PKG-INFO` & `caso-4.2.0/caso.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caso
-Version: 4.1.1.0rc1
+Version: 4.2.0
 Summary: cASO is an OpenStack Accounting extractor.
 Home-page: http://github.com/IFCA/caso
 Author: Alvaro Lopez Garcia
 Author-email: aloga@ifca.unican.es
 License: Apache-2
 Project-URL: Bug Tracker, https://github.com/IFCA/caso/issues
 Project-URL: Documentation, https://caso.readthedocs.io/
```

### Comparing `caso-4.1.1.0rc1/caso.egg-info/SOURCES.txt` & `caso-4.2.0/caso.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 mypy.ini
 requirements.txt
 setup.cfg
 setup.py
 tox.ini
 .github/ISSUE_TEMPLATE.md
 .github/PULL_REQUEST_TEMPLATE.md
+.github/workflows/codecov.yml
 .github/workflows/packaging.yml
 .github/workflows/python-publish.yml
 .github/workflows/python-test.yml
 caso/__init__.py
 caso/config.py
 caso/exception.py
 caso/keystone_client.py
@@ -51,15 +52,18 @@
 caso/extract/openstack/nova.py
 caso/messenger/__init__.py
 caso/messenger/logstash.py
 caso/messenger/noop.py
 caso/messenger/ssm.py
 caso/tests/__init__.py
 caso/tests/base.py
+caso/tests/conftest.py
 caso/tests/test_manager.py
+caso/tests/test_record.py
+caso/tests/test_ssm.py
 caso/tests/extract/__init__.py
 caso/tests/extract/test_manager.py
 caso/tests/extract/test_nova.py
 doc/requirements.txt
 doc/source/conf.py
 doc/source/configuration-file.rst
 doc/source/configuration.rst
@@ -87,14 +91,15 @@
 packaging/debian/postinst
 packaging/debian/rules
 packaging/debian/source/format
 packaging/redhat/caso.spec
 releasenotes/notes/allow-to-load-an-extractor-list-fd1f6905d0d01383.yaml
 releasenotes/notes/default-to-all-extractors-0da9448a00091bc1.yaml
 releasenotes/notes/deprecate-voms-mapping-80cfda2246ec43e9.yaml
+releasenotes/notes/fix-timestamps-84cd81de7d26e164.yaml
 releasenotes/notes/gpu-accounting-082a62b7254d29bd.yaml
 releasenotes/notes/multi-region-support-4395450dfbc4e8a3.yaml
 releasenotes/notes/new-release-notes-b79c3d7a778fc946.yaml
 releasenotes/notes/new-ussuri-configuration-03b764a39f461eda.yaml
 releasenotes/notes/option-deprecation-a4eba5fa1a362815.yaml
 releasenotes/notes/refactor-extractor-e826c64087e17065.yaml
 releasenotes/notes/require-system-scope-67d0d11681beea27.yaml
```

### Comparing `caso-4.1.1.0rc1/caso.egg-info/entry_points.txt` & `caso-4.2.0/caso.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/doc/source/conf.py` & `caso-4.2.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/doc/source/configuration.rst` & `caso-4.2.0/doc/source/configuration.rst`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/doc/source/index.rst` & `caso-4.2.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/doc/source/installation.rst` & `caso-4.2.0/doc/source/installation.rst`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/doc/source/multi-region.rst` & `caso-4.2.0/doc/source/multi-region.rst`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/doc/source/static/caso-diagram.drawio` & `caso-4.2.0/doc/source/static/caso-diagram.drawio`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/doc/source/static/caso-diagram.png` & `caso-4.2.0/doc/source/static/caso-diagram.png`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/doc/source/static/caso.conf.sample` & `caso-4.2.0/doc/source/static/caso.conf.sample`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/doc/source/static/caso.png` & `caso-4.2.0/doc/source/static/caso.png`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/doc/source/troubleshooting.rst` & `caso-4.2.0/doc/source/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/doc/source/usage.rst` & `caso-4.2.0/doc/source/usage.rst`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/etc/caso/caso.conf.sample` & `caso-4.2.0/etc/caso/caso.conf.sample`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/packaging/debian/changelog` & `caso-4.2.0/packaging/debian/changelog`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,22 @@
-python3-caso (4.1.0-0rc2) stable; urgency=medium
+python3-caso (4.2.0-1) stable; urgency=medium
+
+  [ Enol Fernandez ]
+  * [c1df014] fix: use POSIX timestamps for SSM cloud records
+
+  [ Alvaro Lopez Garcia ]
+  * [0135a74] Render JSON dates as timestamp integers
+  * [40eba2b] Do not render records using .dict() but usin JSON
+  * [d2f2b45] Include type annotations on fixtures
+  * [9667bfc] Records must implement an SSM rendering by themselves
+  * Add unit testing for SSM messenger and records
+
+ -- Alvaro Lopez Garcia <aloga@ifca.unican.es>  Wed, 07 Jun 2023 10:09:11 +0200
+
+python3-caso (4.1.1-1) stable; urgency=medium
 
   * [a74fb28] Remove duplicated option
   * [1142758] Let operators mark projects directly on keystone
   * [ce9e416] Use Keystone properties to load VO mapping.
   * [fc039e2] Move VM status method to Nova extractor
   * [3982e48] nova: move accelerator and benchmark options to correct place
   * [416d2f7] extractors: move projects options to correct place
@@ -15,14 +29,15 @@
   * [4bda67d] Fix noop messenger
   * [bb8ffee] Include project names in project listing
   * [93b9df3] Update documentation
   * [b014846] Include caso-projects in usage commands
   * [6aaad9d] Remove deprecated option
   * [42789db] Update configuration file
   * [0206294] Default to all OpenStack extractors
+  * [8d0ea78] Use system_scope for Keystone operations
 
  -- Alvaro Lopez Garcia <aloga@ifca.unican.es>  Mon, 10 Apr 2023 14:29:16 +0200
 
 python3-caso (4.0.0-1) stable; urgency=medium
 
   [ Alvaro Lopez Garcia ]
   * [2dc5334] Remove deprecated extractor base class
```

### Comparing `caso-4.1.1.0rc1/packaging/debian/control` & `caso-4.2.0/packaging/debian/control`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/packaging/debian/copyright` & `caso-4.2.0/packaging/debian/copyright`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/packaging/debian/postinst` & `caso-4.2.0/packaging/debian/postinst`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/packaging/redhat/caso.spec` & `caso-4.2.0/packaging/redhat/caso.spec`

 * *Files 3% similar despite different names*

```diff
@@ -56,14 +56,20 @@
 %{python3_sitelib}/caso/
 %{python3_sitelib}/caso-%{version}*
 %config /etc/caso/caso.conf.sample
 %config /etc/caso/voms.json.sample
 %exclude /etc/caso/caso-config-generator.conf
 
 %changelog
+* Wed Jun 06 2023 Alvaro Lopez Garcia <aloga@ifca.unican.es> 4.2.0
+- fix: use POSIX timestamps for SSM cloud records
+- Render JSON dates as timestamp integers
+- Do not render records using .dict() but usin JSON
+- Include type annotations on fixtures
+- Records must implement an SSM rendering by themselves
 * Mon Apr 10 2023 Alvaro Lopez Garcia <aloga@ifca.unican.es> 4.1.0
 - Remove duplicated option
 - Let operators mark projects directly on keystone
 - Use Keystone properties to load VO mapping.
 - Move VM status method to Nova extractor
 - nova: move accelerator and benchmark options to correct place
 - extractors: move projects options to correct place
```

### Comparing `caso-4.1.1.0rc1/releasenotes/notes/deprecate-voms-mapping-80cfda2246ec43e9.yaml` & `caso-4.2.0/releasenotes/notes/deprecate-voms-mapping-80cfda2246ec43e9.yaml`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/releasenotes/notes/new-release-notes-b79c3d7a778fc946.yaml` & `caso-4.2.0/releasenotes/notes/new-release-notes-b79c3d7a778fc946.yaml`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/releasenotes/notes/new-ussuri-configuration-03b764a39f461eda.yaml` & `caso-4.2.0/releasenotes/notes/new-ussuri-configuration-03b764a39f461eda.yaml`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/requirements.txt` & `caso-4.2.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/setup.cfg` & `caso-4.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/setup.py` & `caso-4.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `caso-4.1.1.0rc1/tox.ini` & `caso-4.2.0/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -63,14 +63,22 @@
 basepython = python3.10
 commands =
     find . -type f -name "*.pyc" -delete
     pytest {posargs} --cov={[base]package} \
            --cov-report term \
            --cov-report=xml
 
+[testenv:covhtml]
+basepython = python3.10
+commands =
+    find . -type f -name "*.pyc" -delete
+    pytest {posargs} --cov={[base]package} \
+           --cov-report term \
+           --cov-report=html
+
 [flake8]
 # Black default line length is 88
 max-line-length = 88
 show-source = True
 builtins = _
 ignore = E123,E125,H803,H405,W504
 exclude =
```

