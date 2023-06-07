# Comparing `tmp/singularity-hpc-0.1.22.tar.gz` & `tmp/singularity-hpc-0.1.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "singularity-hpc-0.1.22.tar", last modified: Thu May  4 22:27:12 2023, max compression
+gzip compressed data, was "singularity-hpc-0.1.23.tar", last modified: Wed Jun  7 13:47:44 2023, max compression
```

## Comparing `singularity-hpc-0.1.22.tar` & `singularity-hpc-0.1.23.tar`

### file list

```diff
@@ -1,159 +1,159 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:27:12.471106 singularity-hpc-0.1.22/
--rw-r--r--   0 runner    (1001) docker     (122)    15830 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      346 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     7729 2023-05-04 22:27:12.471106 singularity-hpc-0.1.22/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     6870 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:27:12.455106 singularity-hpc-0.1.22/example/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:27:12.455106 singularity-hpc-0.1.22/example/google-cloud-storage/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:27:12.455106 singularity-hpc-0.1.22/example/google-cloud-storage/img/
--rw-r--r--   0 runner    (1001) docker     (122)    47310 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/example/google-cloud-storage/img/storage.png
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      241 2023-05-04 22:27:12.471106 singularity-hpc-0.1.22/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3305 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:27:12.459106 singularity-hpc-0.1.22/shpc/
--rw-r--r--   0 runner    (1001) docker     (122)       57 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:27:12.459106 singularity-hpc-0.1.22/shpc/client/
--rw-r--r--   0 runner    (1001) docker     (122)    15917 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      770 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/client/add.py
--rw-r--r--   0 runner    (1001) docker     (122)      548 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/client/check.py
--rw-r--r--   0 runner    (1001) docker     (122)     1491 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/client/config.py
--rw-r--r--   0 runner    (1001) docker     (122)      696 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/client/docgen.py
--rw-r--r--   0 runner    (1001) docker     (122)      607 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/client/get.py
--rw-r--r--   0 runner    (1001) docker     (122)     6864 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/client/help.py
--rw-r--r--   0 runner    (1001) docker     (122)     2364 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/client/inspect.py
--rw-r--r--   0 runner    (1001) docker     (122)     1043 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/client/install.py
--rw-r--r--   0 runner    (1001) docker     (122)      520 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/client/listing.py
--rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/client/namespace.py
--rw-r--r--   0 runner    (1001) docker     (122)      557 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/client/pull.py
--rw-r--r--   0 runner    (1001) docker     (122)      724 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/client/remove.py
--rw-r--r--   0 runner    (1001) docker     (122)     1821 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/client/shell.py
--rw-r--r--   0 runner    (1001) docker     (122)      697 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/client/show.py
--rw-r--r--   0 runner    (1001) docker     (122)      858 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/client/sync.py
--rw-r--r--   0 runner    (1001) docker     (122)      729 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/client/test.py
--rw-r--r--   0 runner    (1001) docker     (122)      990 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/client/uninstall.py
--rw-r--r--   0 runner    (1001) docker     (122)      396 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/client/update.py
--rw-r--r--   0 runner    (1001) docker     (122)     5366 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/client/view.py
--rw-r--r--   0 runner    (1001) docker     (122)      813 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/defaults.py
--rw-r--r--   0 runner    (1001) docker     (122)     6116 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:27:12.459106 singularity-hpc-0.1.22/shpc/main/
--rw-r--r--   0 runner    (1001) docker     (122)     2152 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8078 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/client.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:27:12.459106 singularity-hpc-0.1.22/shpc/main/container/
--rw-r--r--   0 runner    (1001) docker     (122)      154 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6050 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/container/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     9472 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/container/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     7819 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/container/docker.py
--rw-r--r--   0 runner    (1001) docker     (122)      541 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/container/podman.py
--rw-r--r--   0 runner    (1001) docker     (122)    14004 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/container/singularity.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:27:12.459106 singularity-hpc-0.1.22/shpc/main/container/templates/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/container/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      487 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/container/templates/container.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:27:12.459106 singularity-hpc-0.1.22/shpc/main/container/update/
--rw-r--r--   0 runner    (1001) docker     (122)     3929 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/container/update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1994 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/container/update/diff.py
--rw-r--r--   0 runner    (1001) docker     (122)     1864 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/container/update/docker.py
--rw-r--r--   0 runner    (1001) docker     (122)     5287 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/container/update/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:27:12.463106 singularity-hpc-0.1.22/shpc/main/modules/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    17548 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/modules/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      473 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/modules/lmod.py
--rw-r--r--   0 runner    (1001) docker     (122)     5779 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/modules/module.py
--rw-r--r--   0 runner    (1001) docker     (122)      559 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/modules/tcl.py
--rw-r--r--   0 runner    (1001) docker     (122)     1522 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/modules/template.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:27:12.463106 singularity-hpc-0.1.22/shpc/main/modules/templates/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/modules/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/modules/templates/default_version
--rw-r--r--   0 runner    (1001) docker     (122)     6887 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/modules/templates/docker.lua
--rw-r--r--   0 runner    (1001) docker     (122)     8289 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/modules/templates/docker.tcl
--rw-r--r--   0 runner    (1001) docker     (122)     5200 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/modules/templates/docs.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:27:12.463106 singularity-hpc-0.1.22/shpc/main/modules/templates/includes/
--rw-r--r--   0 runner    (1001) docker     (122)      336 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/modules/templates/includes/default_version.lua
--rw-r--r--   0 runner    (1001) docker     (122)      285 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/modules/templates/includes/load_view.lua
--rw-r--r--   0 runner    (1001) docker     (122)      267 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/modules/templates/includes/load_view.tcl
--rw-r--r--   0 runner    (1001) docker     (122)     7855 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/modules/templates/singularity.lua
--rw-r--r--   0 runner    (1001) docker     (122)     9602 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/modules/templates/singularity.tcl
--rwxr-xr-x   0 runner    (1001) docker     (122)      405 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/modules/templates/test.sh
--rw-r--r--   0 runner    (1001) docker     (122)      256 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/modules/templates/view_module.lua
--rw-r--r--   0 runner    (1001) docker     (122)      307 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/modules/templates/view_module.tcl
--rw-r--r--   0 runner    (1001) docker     (122)     2847 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/modules/versions.py
--rw-r--r--   0 runner    (1001) docker     (122)    18795 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/modules/views.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:27:12.463106 singularity-hpc-0.1.22/shpc/main/registry/
--rw-r--r--   0 runner    (1001) docker     (122)     6939 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3925 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/registry/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (122)     1693 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/registry/provider.py
--rw-r--r--   0 runner    (1001) docker     (122)     6072 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/registry/remote.py
--rw-r--r--   0 runner    (1001) docker     (122)     5786 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/schemas.py
--rw-r--r--   0 runner    (1001) docker     (122)    13562 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/settings.py
--rw-r--r--   0 runner    (1001) docker     (122)      488 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/templates.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:27:12.463106 singularity-hpc-0.1.22/shpc/main/wrappers/
--rw-r--r--   0 runner    (1001) docker     (122)     1995 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5150 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/wrappers/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     4018 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/wrappers/generators.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:27:12.463106 singularity-hpc-0.1.22/shpc/main/wrappers/templates/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/wrappers/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:27:12.463106 singularity-hpc-0.1.22/shpc/main/wrappers/templates/bases/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/wrappers/templates/bases/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      319 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/wrappers/templates/bases/shell-script-base.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:27:12.467106 singularity-hpc-0.1.22/shpc/main/wrappers/templates/docker/
--rw-r--r--   0 runner    (1001) docker     (122)       96 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/wrappers/templates/docker/container.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      625 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/wrappers/templates/docker/exec.sh
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/wrappers/templates/docker/inspect.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      625 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/wrappers/templates/docker/run.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      650 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/wrappers/templates/docker/shell.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      730 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/wrappers/templates/docker.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:27:12.467106 singularity-hpc-0.1.22/shpc/main/wrappers/templates/singularity/
--rw-r--r--   0 runner    (1001) docker     (122)       96 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/wrappers/templates/singularity/container.sh
--rw-r--r--   0 runner    (1001) docker     (122)      774 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/wrappers/templates/singularity/exec.sh
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/wrappers/templates/singularity/inspect-deffile.sh
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/wrappers/templates/singularity/inspect-runscript.sh
--rw-r--r--   0 runner    (1001) docker     (122)      773 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/wrappers/templates/singularity/run.sh
--rw-r--r--   0 runner    (1001) docker     (122)      585 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/wrappers/templates/singularity/shell.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      794 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/wrappers/templates/singularity.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:27:12.467106 singularity-hpc-0.1.22/shpc/main/wrappers/templates/snippets/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/main/wrappers/templates/snippets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3896 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/settings.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:27:12.467106 singularity-hpc-0.1.22/shpc/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1717 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (122)      569 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/tests/helpers.sh
--rwxr-xr-x   0 runner    (1001) docker     (122)      474 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/tests/test-registry-module.sh
--rw-r--r--   0 runner    (1001) docker     (122)    13070 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/tests/test_client.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3757 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/tests/test_client.sh
--rw-r--r--   0 runner    (1001) docker     (122)     3846 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (122)     1777 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/tests/test_container.py
--rw-r--r--   0 runner    (1001) docker     (122)     3533 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/tests/test_container_config.py
--rw-r--r--   0 runner    (1001) docker     (122)     1828 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (122)     4150 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/tests/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (122)     4671 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     6646 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (122)     6826 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/tests/test_wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:27:12.467106 singularity-hpc-0.1.22/shpc/tests/testdata/
--rw-r--r--   0 runner    (1001) docker     (122)      839 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/tests/testdata/alias-container.yaml
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/tests/testdata/empty_singularity.sh
--rw-r--r--   0 runner    (1001) docker     (122)      108 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/tests/testdata/hashtest.txt
--rw-r--r--   0 runner    (1001) docker     (122)       45 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/tests/testdata/overrides-invalid.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/tests/testdata/overrides.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      755 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/tests/testdata/python-container.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      410 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/tests/testdata/quay-container.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:27:12.455106 singularity-hpc-0.1.22/shpc/tests/testdata/registry/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:27:12.455106 singularity-hpc-0.1.22/shpc/tests/testdata/registry/dinosaur/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:27:12.467106 singularity-hpc-0.1.22/shpc/tests/testdata/registry/dinosaur/salad/
--rw-r--r--   0 runner    (1001) docker     (122)      636 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/tests/testdata/registry/dinosaur/salad/container.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:27:12.467106 singularity-hpc-0.1.22/shpc/tests/testdata/samtools/
--rw-r--r--   0 runner    (1001) docker     (122)     1173 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/tests/testdata/samtools/1.14--hb421002_0.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       47 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/tests/testdata/samtools/1.15--h3843a85_0.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1530 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/tests/testdata/samtools/container.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      114 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/tests/testdata/view.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:27:12.471106 singularity-hpc-0.1.22/shpc/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      460 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5824 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/utils/fileio.py
--rw-r--r--   0 runner    (1001) docker     (122)     3575 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/utils/terminal.py
--rw-r--r--   0 runner    (1001) docker     (122)     1151 2023-05-04 22:26:40.000000 singularity-hpc-0.1.22/shpc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:27:12.471106 singularity-hpc-0.1.22/singularity_hpc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7729 2023-05-04 22:27:12.000000 singularity-hpc-0.1.22/singularity_hpc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4212 2023-05-04 22:27:12.000000 singularity-hpc-0.1.22/singularity_hpc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-04 22:27:12.000000 singularity-hpc-0.1.22/singularity_hpc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-05-04 22:27:12.000000 singularity-hpc-0.1.22/singularity_hpc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-04 22:27:12.000000 singularity-hpc-0.1.22/singularity_hpc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      129 2023-05-04 22:27:12.000000 singularity-hpc-0.1.22/singularity_hpc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-04 22:27:12.000000 singularity-hpc-0.1.22/singularity_hpc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 13:47:44.942203 singularity-hpc-0.1.23/
+-rw-r--r--   0 runner    (1001) docker     (122)    15830 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      346 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     7729 2023-06-07 13:47:44.942203 singularity-hpc-0.1.23/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6870 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 13:47:44.926202 singularity-hpc-0.1.23/example/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 13:47:44.926202 singularity-hpc-0.1.23/example/google-cloud-storage/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 13:47:44.926202 singularity-hpc-0.1.23/example/google-cloud-storage/img/
+-rw-r--r--   0 runner    (1001) docker     (122)    47310 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/example/google-cloud-storage/img/storage.png
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      241 2023-06-07 13:47:44.942203 singularity-hpc-0.1.23/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3305 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 13:47:44.930203 singularity-hpc-0.1.23/shpc/
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 13:47:44.930203 singularity-hpc-0.1.23/shpc/client/
+-rw-r--r--   0 runner    (1001) docker     (122)    15917 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      770 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/client/add.py
+-rw-r--r--   0 runner    (1001) docker     (122)      548 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/client/check.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1491 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/client/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      696 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/client/docgen.py
+-rw-r--r--   0 runner    (1001) docker     (122)      607 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/client/get.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6864 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/client/help.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2364 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/client/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1043 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/client/install.py
+-rw-r--r--   0 runner    (1001) docker     (122)      520 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/client/listing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1181 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/client/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (122)      557 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/client/pull.py
+-rw-r--r--   0 runner    (1001) docker     (122)      724 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/client/remove.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1821 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/client/shell.py
+-rw-r--r--   0 runner    (1001) docker     (122)      697 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/client/show.py
+-rw-r--r--   0 runner    (1001) docker     (122)      858 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/client/sync.py
+-rw-r--r--   0 runner    (1001) docker     (122)      729 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/client/test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      990 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/client/uninstall.py
+-rw-r--r--   0 runner    (1001) docker     (122)      396 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/client/update.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5366 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/client/view.py
+-rw-r--r--   0 runner    (1001) docker     (122)      813 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6116 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 13:47:44.930203 singularity-hpc-0.1.23/shpc/main/
+-rw-r--r--   0 runner    (1001) docker     (122)     2152 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8078 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 13:47:44.930203 singularity-hpc-0.1.23/shpc/main/container/
+-rw-r--r--   0 runner    (1001) docker     (122)      154 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6379 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/container/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9533 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/container/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7864 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/container/docker.py
+-rw-r--r--   0 runner    (1001) docker     (122)      541 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/container/podman.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14124 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/container/singularity.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 13:47:44.930203 singularity-hpc-0.1.23/shpc/main/container/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/container/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      487 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/container/templates/container.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 13:47:44.934203 singularity-hpc-0.1.23/shpc/main/container/update/
+-rw-r--r--   0 runner    (1001) docker     (122)     3929 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/container/update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1994 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/container/update/diff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1864 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/container/update/docker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5287 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/container/update/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 13:47:44.934203 singularity-hpc-0.1.23/shpc/main/modules/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17548 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/modules/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      473 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/modules/lmod.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5779 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/modules/module.py
+-rw-r--r--   0 runner    (1001) docker     (122)      559 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/modules/tcl.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1522 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/modules/template.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 13:47:44.934203 singularity-hpc-0.1.23/shpc/main/modules/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/modules/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/modules/templates/default_version
+-rw-r--r--   0 runner    (1001) docker     (122)     6887 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/modules/templates/docker.lua
+-rw-r--r--   0 runner    (1001) docker     (122)     8289 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/modules/templates/docker.tcl
+-rw-r--r--   0 runner    (1001) docker     (122)     5200 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/modules/templates/docs.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 13:47:44.934203 singularity-hpc-0.1.23/shpc/main/modules/templates/includes/
+-rw-r--r--   0 runner    (1001) docker     (122)      336 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/modules/templates/includes/default_version.lua
+-rw-r--r--   0 runner    (1001) docker     (122)      285 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/modules/templates/includes/load_view.lua
+-rw-r--r--   0 runner    (1001) docker     (122)      267 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/modules/templates/includes/load_view.tcl
+-rw-r--r--   0 runner    (1001) docker     (122)     7855 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/modules/templates/singularity.lua
+-rw-r--r--   0 runner    (1001) docker     (122)     9602 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/modules/templates/singularity.tcl
+-rwxr-xr-x   0 runner    (1001) docker     (122)      405 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/modules/templates/test.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      256 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/modules/templates/view_module.lua
+-rw-r--r--   0 runner    (1001) docker     (122)      307 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/modules/templates/view_module.tcl
+-rw-r--r--   0 runner    (1001) docker     (122)     2847 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/modules/versions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18795 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/modules/views.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 13:47:44.934203 singularity-hpc-0.1.23/shpc/main/registry/
+-rw-r--r--   0 runner    (1001) docker     (122)     6939 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3925 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/registry/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1693 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/registry/provider.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6072 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/registry/remote.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5829 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13562 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)      488 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/templates.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 13:47:44.934203 singularity-hpc-0.1.23/shpc/main/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (122)     1995 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5150 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/wrappers/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4018 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/wrappers/generators.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 13:47:44.934203 singularity-hpc-0.1.23/shpc/main/wrappers/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/wrappers/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 13:47:44.934203 singularity-hpc-0.1.23/shpc/main/wrappers/templates/bases/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/wrappers/templates/bases/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)      319 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/wrappers/templates/bases/shell-script-base.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 13:47:44.934203 singularity-hpc-0.1.23/shpc/main/wrappers/templates/docker/
+-rw-r--r--   0 runner    (1001) docker     (122)       96 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/wrappers/templates/docker/container.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      625 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/wrappers/templates/docker/exec.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/wrappers/templates/docker/inspect.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      625 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/wrappers/templates/docker/run.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      650 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/wrappers/templates/docker/shell.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      730 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/wrappers/templates/docker.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 13:47:44.938203 singularity-hpc-0.1.23/shpc/main/wrappers/templates/singularity/
+-rw-r--r--   0 runner    (1001) docker     (122)       96 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/wrappers/templates/singularity/container.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      774 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/wrappers/templates/singularity/exec.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/wrappers/templates/singularity/inspect-deffile.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/wrappers/templates/singularity/inspect-runscript.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      773 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/wrappers/templates/singularity/run.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      585 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/wrappers/templates/singularity/shell.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      794 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/wrappers/templates/singularity.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 13:47:44.938203 singularity-hpc-0.1.23/shpc/main/wrappers/templates/snippets/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/main/wrappers/templates/snippets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3976 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/settings.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 13:47:44.938203 singularity-hpc-0.1.23/shpc/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1717 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      569 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/tests/helpers.sh
+-rwxr-xr-x   0 runner    (1001) docker     (122)      474 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/tests/test-registry-module.sh
+-rw-r--r--   0 runner    (1001) docker     (122)    13070 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/tests/test_client.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3757 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/tests/test_client.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     3846 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1777 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/tests/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3533 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/tests/test_container_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1828 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4150 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/tests/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4671 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6646 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6826 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/tests/test_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 13:47:44.938203 singularity-hpc-0.1.23/shpc/tests/testdata/
+-rw-r--r--   0 runner    (1001) docker     (122)      839 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/tests/testdata/alias-container.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/tests/testdata/empty_singularity.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      108 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/tests/testdata/hashtest.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/tests/testdata/overrides-invalid.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/tests/testdata/overrides.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      755 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/tests/testdata/python-container.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      410 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/tests/testdata/quay-container.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 13:47:44.926202 singularity-hpc-0.1.23/shpc/tests/testdata/registry/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 13:47:44.926202 singularity-hpc-0.1.23/shpc/tests/testdata/registry/dinosaur/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 13:47:44.938203 singularity-hpc-0.1.23/shpc/tests/testdata/registry/dinosaur/salad/
+-rw-r--r--   0 runner    (1001) docker     (122)      636 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/tests/testdata/registry/dinosaur/salad/container.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 13:47:44.938203 singularity-hpc-0.1.23/shpc/tests/testdata/samtools/
+-rw-r--r--   0 runner    (1001) docker     (122)     1173 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/tests/testdata/samtools/1.14--hb421002_0.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/tests/testdata/samtools/1.15--h3843a85_0.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1530 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/tests/testdata/samtools/container.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      114 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/tests/testdata/view.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 13:47:44.938203 singularity-hpc-0.1.23/shpc/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      460 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5824 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/utils/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3575 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/utils/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1151 2023-06-07 13:47:01.000000 singularity-hpc-0.1.23/shpc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 13:47:44.942203 singularity-hpc-0.1.23/singularity_hpc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7729 2023-06-07 13:47:44.000000 singularity-hpc-0.1.23/singularity_hpc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4212 2023-06-07 13:47:44.000000 singularity-hpc-0.1.23/singularity_hpc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-07 13:47:44.000000 singularity-hpc-0.1.23/singularity_hpc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-06-07 13:47:44.000000 singularity-hpc-0.1.23/singularity_hpc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-07 13:47:44.000000 singularity-hpc-0.1.23/singularity_hpc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      129 2023-06-07 13:47:44.000000 singularity-hpc-0.1.23/singularity_hpc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-07 13:47:44.000000 singularity-hpc-0.1.23/singularity_hpc.egg-info/top_level.txt
```

### Comparing `singularity-hpc-0.1.22/LICENSE` & `singularity-hpc-0.1.23/LICENSE`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/PKG-INFO` & `singularity-hpc-0.1.23/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: singularity-hpc
-Version: 0.1.22
+Version: 0.1.23
 Summary: Local registry intended for HPC using containers and system modules.
 Home-page: https://github.com/singularityhub/singularity-hpc
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: singularity,containers,hpc,lmd
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: singularity-hpc Version: 0.1.22 Summary: Local
+Metadata-Version: 2.1 Name: singularity-hpc Version: 0.1.23 Summary: Local
 registry intended for HPC using containers and system modules. Home-page:
 https://github.com/singularityhub/singularity-hpc Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com Maintainer: Vanessa Sochat
 License: LICENSE Keywords: singularity,containers,hpc,lmd Classifier: Intended
 Audience :: Science/Research Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: C Classifier: Programming Language ::
```

### Comparing `singularity-hpc-0.1.22/README.md` & `singularity-hpc-0.1.23/README.md`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/example/google-cloud-storage/img/storage.png` & `singularity-hpc-0.1.23/example/google-cloud-storage/img/storage.png`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/setup.py` & `singularity-hpc-0.1.23/setup.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/client/__init__.py` & `singularity-hpc-0.1.23/shpc/client/__init__.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/client/add.py` & `singularity-hpc-0.1.23/shpc/client/add.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/client/check.py` & `singularity-hpc-0.1.23/shpc/client/check.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/client/config.py` & `singularity-hpc-0.1.23/shpc/client/config.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/client/docgen.py` & `singularity-hpc-0.1.23/shpc/client/docgen.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/client/get.py` & `singularity-hpc-0.1.23/shpc/client/get.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/client/help.py` & `singularity-hpc-0.1.23/shpc/client/help.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/client/inspect.py` & `singularity-hpc-0.1.23/shpc/client/inspect.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/client/install.py` & `singularity-hpc-0.1.23/shpc/client/install.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/client/listing.py` & `singularity-hpc-0.1.23/shpc/client/listing.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/client/namespace.py` & `singularity-hpc-0.1.23/shpc/client/namespace.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/client/pull.py` & `singularity-hpc-0.1.23/shpc/client/pull.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/client/remove.py` & `singularity-hpc-0.1.23/shpc/client/remove.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/client/shell.py` & `singularity-hpc-0.1.23/shpc/client/shell.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/client/show.py` & `singularity-hpc-0.1.23/shpc/client/show.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/client/sync.py` & `singularity-hpc-0.1.23/shpc/client/sync.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/client/test.py` & `singularity-hpc-0.1.23/shpc/client/test.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/client/uninstall.py` & `singularity-hpc-0.1.23/shpc/client/uninstall.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/client/view.py` & `singularity-hpc-0.1.23/shpc/client/view.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/defaults.py` & `singularity-hpc-0.1.23/shpc/defaults.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/logger.py` & `singularity-hpc-0.1.23/shpc/logger.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/main/__init__.py` & `singularity-hpc-0.1.23/shpc/main/__init__.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/main/client.py` & `singularity-hpc-0.1.23/shpc/main/client.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/main/container/base.py` & `singularity-hpc-0.1.23/shpc/main/container/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -98,14 +98,23 @@
         if ":" in name:
             name = name.replace(":", os.sep)
 
         if not self.settings.container_base:
             return os.path.join(self.settings.module_base, name)
         return os.path.join(self.settings.container_base, name)
 
+    def clean_labels(self, labels):
+        """
+        Clean labels, meaning removing newlines and replacing with label separator
+        """
+        updated_labels = {}
+        for key, value in labels.items():
+            updated_labels[key] = value.replace("\n", self.settings.label_separator)
+        return updated_labels
+
     def guess_tag(self, module_name, allow_fail=False):
         """
         If a user asks for a name without a tag, try to figure it out.
         """
         if ":" in module_name:
             return module_name
         tags = self.installed_tags(module_name)
```

### Comparing `singularity-hpc-0.1.22/shpc/main/container/config.py` & `singularity-hpc-0.1.23/shpc/main/container/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,14 +250,17 @@
         ):
             logger.exit(
                 "A docker, gh, or path field is currently required in the config."
             )
         return self.get("docker") or self.get("gh") or self.get("path")
 
     def get(self, key, default=None):
+        """
+        Get a value from the config.
+        """
         return self.entry._config.get(key, default)
 
     def get_pull_type(self):
         if self.oras:
             return "oras"
         if self.gh:
             return "gh"
```

### Comparing `singularity-hpc-0.1.22/shpc/main/container/docker.py` & `singularity-hpc-0.1.23/shpc/main/container/docker.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,15 +203,16 @@
         # Do we want to clean up other versions here too?
         manifest = self.inspect(module.container_path)
         if not manifest:
             sys.exit(
                 "Container %s was not found. Was it pulled?" % module.container_path
             )
 
-        labels = manifest[0].get("Labels", {})
+        labels = manifest[0].get("Labels") or {}
+        labels = self.clean_labels(labels)
 
         # Option to create wrapper scripts for commands
         aliases = module.config.get_aliases()
         wrapper_scripts = []
 
         # Wrapper scripts can be global (for aliases) or container specific
         if self.settings.wrapper_scripts["enabled"] is True:
```

### Comparing `singularity-hpc-0.1.22/shpc/main/container/podman.py` & `singularity-hpc-0.1.23/shpc/main/container/podman.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/main/container/singularity.py` & `singularity-hpc-0.1.23/shpc/main/container/singularity.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,26 +187,29 @@
             os.remove(older)
 
         # Get inspect metadata from the container (only if singularity installed
         try:
             metadata = self.inspect(module.container_path)
 
             # Add labels, and deffile
-            labels = metadata.get("attributes", {}).get("labels")
+            labels = metadata.get("attributes", {}).get("labels") or {}
             deffile = (
                 metadata.get("attributes", {}).get("deffile", "").replace("\n", "\\n")
             )
         except Exception:
             metadata = None
             deffile = None
             labels = {}
 
         # Option to create wrapper scripts for commands
         aliases = module.config.get_aliases()
 
+        # Labels with newlines need to be handled, replace with comma
+        labels = self.clean_labels(labels)
+
         # Wrapper scripts can be global (for aliases) or container specific
         wrapper_scripts = []
         if self.settings.wrapper_scripts["enabled"] is True:
             wrapper_scripts = shpc.main.wrappers.generate(
                 aliases=aliases,
                 module_dir=module.module_dir,
                 features=features,
```

### Comparing `singularity-hpc-0.1.22/shpc/main/container/update/__init__.py` & `singularity-hpc-0.1.23/shpc/main/container/update/__init__.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/main/container/update/diff.py` & `singularity-hpc-0.1.23/shpc/main/container/update/diff.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/main/container/update/docker.py` & `singularity-hpc-0.1.23/shpc/main/container/update/docker.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/main/container/update/versions.py` & `singularity-hpc-0.1.23/shpc/main/container/update/versions.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/main/modules/base.py` & `singularity-hpc-0.1.23/shpc/main/modules/base.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/main/modules/module.py` & `singularity-hpc-0.1.23/shpc/main/modules/module.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/main/modules/tcl.py` & `singularity-hpc-0.1.23/shpc/main/modules/tcl.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/main/modules/template.py` & `singularity-hpc-0.1.23/shpc/main/modules/template.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/main/modules/templates/docker.lua` & `singularity-hpc-0.1.23/shpc/main/modules/templates/docker.lua`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/main/modules/templates/docker.tcl` & `singularity-hpc-0.1.23/shpc/main/modules/templates/docker.tcl`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/main/modules/templates/docs.md` & `singularity-hpc-0.1.23/shpc/main/modules/templates/docs.md`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/main/modules/templates/singularity.lua` & `singularity-hpc-0.1.23/shpc/main/modules/templates/singularity.lua`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/main/modules/templates/singularity.tcl` & `singularity-hpc-0.1.23/shpc/main/modules/templates/singularity.tcl`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/main/modules/versions.py` & `singularity-hpc-0.1.23/shpc/main/modules/versions.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/main/modules/views.py` & `singularity-hpc-0.1.23/shpc/main/modules/views.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/main/registry/__init__.py` & `singularity-hpc-0.1.23/shpc/main/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/main/registry/filesystem.py` & `singularity-hpc-0.1.23/shpc/main/registry/filesystem.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/main/registry/provider.py` & `singularity-hpc-0.1.23/shpc/main/registry/provider.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/main/registry/remote.py` & `singularity-hpc-0.1.23/shpc/main/registry/remote.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/main/schemas.py` & `singularity-hpc-0.1.23/shpc/main/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,14 +153,15 @@
             {
                 "type": "string",
                 "enum": ["module_sys", "last_installed", "first_installed"],
             },
         ]
     },
     "enable_tty": {"type": "boolean"},
+    "label_separator": {"type": "string"},
     "views_base": {"type": ["string", "null"]},
     "default_view": {"type": ["string", "null"]},
     "wrapper_scripts": wrapper_scripts,
     "container_tech": {"type": "string", "enum": ["singularity", "podman", "docker"]},
     "singularity_shell": {"type": "string", "enum": shells},
     "podman_shell": {"type": "string", "enum": shells},
     "docker_shell": {"type": "string", "enum": shells},
```

### Comparing `singularity-hpc-0.1.22/shpc/main/settings.py` & `singularity-hpc-0.1.23/shpc/main/settings.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/main/wrappers/__init__.py` & `singularity-hpc-0.1.23/shpc/main/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/main/wrappers/base.py` & `singularity-hpc-0.1.23/shpc/main/wrappers/base.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/main/wrappers/generators.py` & `singularity-hpc-0.1.23/shpc/main/wrappers/generators.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/main/wrappers/templates/docker/exec.sh` & `singularity-hpc-0.1.23/shpc/main/wrappers/templates/docker/exec.sh`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/main/wrappers/templates/docker/run.sh` & `singularity-hpc-0.1.23/shpc/main/wrappers/templates/docker/run.sh`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/main/wrappers/templates/docker/shell.sh` & `singularity-hpc-0.1.23/shpc/main/wrappers/templates/docker/shell.sh`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/main/wrappers/templates/docker.sh` & `singularity-hpc-0.1.23/shpc/main/wrappers/templates/docker.sh`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/main/wrappers/templates/singularity/exec.sh` & `singularity-hpc-0.1.23/shpc/main/wrappers/templates/singularity/exec.sh`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/main/wrappers/templates/singularity/run.sh` & `singularity-hpc-0.1.23/shpc/main/wrappers/templates/singularity/run.sh`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/main/wrappers/templates/singularity/shell.sh` & `singularity-hpc-0.1.23/shpc/main/wrappers/templates/singularity/shell.sh`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/main/wrappers/templates/singularity.sh` & `singularity-hpc-0.1.23/shpc/main/wrappers/templates/singularity.sh`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/settings.yml` & `singularity-hpc-0.1.23/shpc/settings.yml`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,17 @@
 # first_installed: use the first installed
 default_version: module_sys
 
 # store containers separately from module files
 # It's recommended to do this for faster loading
 container_base: $root_dir/containers
 
+# When parsing labels, replace newlines with this string
+label_separator: ', '
+
 # Default root directory to create views
 views_base: $root_dir/views
 
 # Always install to a default "active" view (null means we don't)
 default_view:
 
 # if defined, add to lmod script to load this Singularity module first
```

### Comparing `singularity-hpc-0.1.22/shpc/tests/helpers.py` & `singularity-hpc-0.1.23/shpc/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/tests/helpers.sh` & `singularity-hpc-0.1.23/shpc/tests/helpers.sh`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/tests/test_client.py` & `singularity-hpc-0.1.23/shpc/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/tests/test_client.sh` & `singularity-hpc-0.1.23/shpc/tests/test_client.sh`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/tests/test_config.py` & `singularity-hpc-0.1.23/shpc/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/tests/test_container.py` & `singularity-hpc-0.1.23/shpc/tests/test_container.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/tests/test_container_config.py` & `singularity-hpc-0.1.23/shpc/tests/test_container_config.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/tests/test_settings.py` & `singularity-hpc-0.1.23/shpc/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/tests/test_sync.py` & `singularity-hpc-0.1.23/shpc/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/tests/test_utils.py` & `singularity-hpc-0.1.23/shpc/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/tests/test_views.py` & `singularity-hpc-0.1.23/shpc/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/tests/test_wrappers.py` & `singularity-hpc-0.1.23/shpc/tests/test_wrappers.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/tests/testdata/alias-container.yaml` & `singularity-hpc-0.1.23/shpc/tests/testdata/alias-container.yaml`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/tests/testdata/python-container.yaml` & `singularity-hpc-0.1.23/shpc/tests/testdata/python-container.yaml`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/tests/testdata/registry/dinosaur/salad/container.yaml` & `singularity-hpc-0.1.23/shpc/tests/testdata/registry/dinosaur/salad/container.yaml`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/tests/testdata/samtools/1.14--hb421002_0.yaml` & `singularity-hpc-0.1.23/shpc/tests/testdata/samtools/1.14--hb421002_0.yaml`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/tests/testdata/samtools/container.yaml` & `singularity-hpc-0.1.23/shpc/tests/testdata/samtools/container.yaml`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/utils/fileio.py` & `singularity-hpc-0.1.23/shpc/utils/fileio.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/utils/terminal.py` & `singularity-hpc-0.1.23/shpc/utils/terminal.py`

 * *Files identical despite different names*

### Comparing `singularity-hpc-0.1.22/shpc/version.py` & `singularity-hpc-0.1.23/shpc/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __author__ = "Vanessa Sochat"
 __copyright__ = "Copyright 2021-2023, Vanessa Sochat"
 __license__ = "MPL 2.0"
 
-__version__ = "0.1.22"
+__version__ = "0.1.23"
 AUTHOR = "Vanessa Sochat"
 EMAIL = "vsoch@users.noreply.github.com"
 NAME = "singularity-hpc"
 PACKAGE_URL = "https://github.com/singularityhub/singularity-hpc"
 KEYWORDS = "singularity, containers, hpc, lmd"
 DESCRIPTION = "Local registry intended for HPC using containers and system modules."
 LICENSE = "LICENSE"
```

### Comparing `singularity-hpc-0.1.22/singularity_hpc.egg-info/PKG-INFO` & `singularity-hpc-0.1.23/singularity_hpc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: singularity-hpc
-Version: 0.1.22
+Version: 0.1.23
 Summary: Local registry intended for HPC using containers and system modules.
 Home-page: https://github.com/singularityhub/singularity-hpc
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: singularity,containers,hpc,lmd
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: singularity-hpc Version: 0.1.22 Summary: Local
+Metadata-Version: 2.1 Name: singularity-hpc Version: 0.1.23 Summary: Local
 registry intended for HPC using containers and system modules. Home-page:
 https://github.com/singularityhub/singularity-hpc Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com Maintainer: Vanessa Sochat
 License: LICENSE Keywords: singularity,containers,hpc,lmd Classifier: Intended
 Audience :: Science/Research Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: C Classifier: Programming Language ::
```

### Comparing `singularity-hpc-0.1.22/singularity_hpc.egg-info/SOURCES.txt` & `singularity-hpc-0.1.23/singularity_hpc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

