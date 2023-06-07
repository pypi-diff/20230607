# Comparing `tmp/board_automate-0.3.0.tar.gz` & `tmp/board_automate-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "board_automate-0.3.0.tar", max compression
+gzip compressed data, was "board_automate-0.4.0.tar", max compression
```

## Comparing `board_automate-0.3.0.tar` & `board_automate-0.4.0.tar`

### file list

```diff
@@ -1,73 +1,73 @@
--rw-r--r--   0        0        0     1083 2022-12-12 19:32:40.802366 board_automate-0.3.0/LICENSE
--rw-r--r--   0        0        0      348 2021-08-17 13:08:10.908459 board_automate-0.3.0/automate/__init__.py
--rw-r--r--   0        0        0        0 2023-03-05 17:24:23.234629 board_automate-0.3.0/automate/_vendor/__init__.py
--rw-r--r--   0        0        0        0 2023-03-05 17:24:24.082632 board_automate-0.3.0/automate/_vendor/patchwork/__init__.py
--rw-r--r--   0        0        0       80 2023-03-05 17:24:24.086632 board_automate-0.3.0/automate/_vendor/patchwork/_version.py
--rw-r--r--   0        0        0      265 2023-03-05 17:24:24.078632 board_automate-0.3.0/automate/_vendor/patchwork/environment.py
--rw-r--r--   0        0        0     3611 2023-03-05 17:27:36.575414 board_automate-0.3.0/automate/_vendor/patchwork/files.py
--rw-r--r--   0        0        0     1469 2023-03-05 17:24:24.078632 board_automate-0.3.0/automate/_vendor/patchwork/info.py
--rw-r--r--   0        0        0      990 2023-03-05 17:24:24.082632 board_automate-0.3.0/automate/_vendor/patchwork/packages/__init__.py
--rw-r--r--   0        0        0     5778 2023-03-05 17:24:24.082632 board_automate-0.3.0/automate/_vendor/patchwork/transfers.py
--rw-r--r--   0        0        0     5260 2023-03-05 17:24:24.082632 board_automate-0.3.0/automate/_vendor/patchwork/util.py
--rw-r--r--   0        0        0     1198 2023-03-05 17:24:23.918631 board_automate-0.3.0/automate/_vendor/patchwork-1.0.1.dist-info/DESCRIPTION.rst
--rw-r--r--   0        0        0        4 2023-03-05 17:24:23.922632 board_automate-0.3.0/automate/_vendor/patchwork-1.0.1.dist-info/INSTALLER
--rw-r--r--   0        0        0     1314 2023-03-05 17:24:23.918631 board_automate-0.3.0/automate/_vendor/patchwork-1.0.1.dist-info/LICENSE.txt
--rw-r--r--   0        0        0     2574 2023-03-05 17:24:23.918631 board_automate-0.3.0/automate/_vendor/patchwork-1.0.1.dist-info/METADATA
--rw-r--r--   0        0        0     1811 2023-03-05 17:24:23.958632 board_automate-0.3.0/automate/_vendor/patchwork-1.0.1.dist-info/RECORD
--rw-r--r--   0        0        0        0 2023-03-05 17:24:23.958632 board_automate-0.3.0/automate/_vendor/patchwork-1.0.1.dist-info/REQUESTED
--rw-r--r--   0        0        0      110 2023-03-05 17:24:23.918631 board_automate-0.3.0/automate/_vendor/patchwork-1.0.1.dist-info/WHEEL
--rw-r--r--   0        0        0     1443 2023-03-05 17:24:23.918631 board_automate-0.3.0/automate/_vendor/patchwork-1.0.1.dist-info/metadata.json
--rw-r--r--   0        0        0       10 2023-03-05 17:24:23.918631 board_automate-0.3.0/automate/_vendor/patchwork-1.0.1.dist-info/top_level.txt
--rw-r--r--   0        0        0       80 2023-03-05 17:30:56.276227 board_automate-0.3.0/automate/_version.py
--rw-r--r--   0        0        0    15650 2021-08-17 13:08:10.908459 board_automate-0.3.0/automate/board.py
--rw-r--r--   0        0        0      133 2021-08-17 13:08:10.908459 board_automate-0.3.0/automate/builder/__init__.py
--rw-r--r--   0        0        0     4794 2023-03-05 16:28:13.337031 board_automate-0.3.0/automate/builder/builder.py
--rw-r--r--   0        0        0     6252 2021-08-17 13:08:10.908459 board_automate-0.3.0/automate/builder/cmake.py
--rw-r--r--   0        0        0     8666 2021-08-17 13:08:10.908459 board_automate-0.3.0/automate/builder/kernel.py
--rw-r--r--   0        0        0     3629 2021-08-17 13:08:10.908459 board_automate-0.3.0/automate/builder/make.py
--rw-r--r--   0        0        0    13943 2021-08-17 13:08:10.908459 board_automate-0.3.0/automate/compiler.py
--rw-r--r--   0        0        0      990 2023-03-05 16:18:07.702511 board_automate-0.3.0/automate/config.py
--rw-r--r--   0        0        0    15168 2022-12-12 18:48:35.316190 board_automate-0.3.0/automate/context.py
--rw-r--r--   0        0        0       49 2021-08-17 13:08:10.908459 board_automate-0.3.0/automate/database/__init__.py
--rw-r--r--   0        0        0    17481 2022-05-05 13:11:49.893064 board_automate-0.3.0/automate/database/database.py
--rw-r--r--   0        0        0      109 2021-08-17 13:08:10.908459 board_automate-0.3.0/automate/database/queries/delete_lock_for_board.sql
--rw-r--r--   0        0        0    17186 2021-08-17 13:08:10.908459 board_automate-0.3.0/automate/database/queries/init_database.sql
--rw-r--r--   0        0        0    11009 2021-08-17 13:08:10.908459 board_automate-0.3.0/automate/database/queries/insert_board.sql
--rw-r--r--   0        0        0      202 2021-08-17 13:08:10.908459 board_automate-0.3.0/automate/database/queries/insert_lock.sql
--rw-r--r--   0        0        0      185 2021-08-17 13:08:10.908459 board_automate-0.3.0/automate/database/queries/select_all_boards.sql
--rw-r--r--   0        0        0     1027 2021-08-17 13:08:10.908459 board_automate-0.3.0/automate/database/queries/select_all_cpu_cores_for_board.sql
--rw-r--r--   0        0        0      155 2021-08-17 13:08:10.908459 board_automate-0.3.0/automate/database/queries/select_all_docs_for_board.sql
--rw-r--r--   0        0        0      584 2021-08-17 13:08:10.908459 board_automate-0.3.0/automate/database/queries/select_all_kernels_for_os.sql
--rw-r--r--   0        0        0      121 2021-08-17 13:08:10.908459 board_automate-0.3.0/automate/database/queries/select_lock_for_board.sql
--rw-r--r--   0        0        0      629 2021-08-17 13:08:10.908459 board_automate-0.3.0/automate/database/queries/select_os_for_board.sql
--rw-r--r--   0        0        0      174 2021-08-17 13:08:10.908459 board_automate-0.3.0/automate/database/queries/transfer_lock_for_board.sql
--rw-r--r--   0        0        0      133 2021-08-17 13:08:10.908459 board_automate-0.3.0/automate/database/queries/update_lock_lease_for_board.sql
--rw-r--r--   0        0        0      469 2021-08-17 13:08:10.908459 board_automate-0.3.0/automate/executor.py
--rw-r--r--   0        0        0     7125 2022-05-05 13:11:49.901064 board_automate-0.3.0/automate/loader.py
--rw-r--r--   0        0        0    12819 2022-05-05 13:11:49.905064 board_automate-0.3.0/automate/locks.py
--rw-r--r--   0        0        0     1884 2021-08-17 13:08:10.908459 board_automate-0.3.0/automate/main.py
--rw-r--r--   0        0        0      111 2021-08-17 13:08:10.908459 board_automate-0.3.0/automate/model/__init__.py
--rw-r--r--   0        0        0     3109 2021-08-17 13:08:10.908459 board_automate-0.3.0/automate/model/board.py
--rw-r--r--   0        0        0     2167 2021-08-17 13:08:10.908459 board_automate-0.3.0/automate/model/common.py
--rw-r--r--   0        0        0      956 2021-08-17 13:08:10.908459 board_automate-0.3.0/automate/model/compiler.py
--rw-r--r--   0        0        0      284 2021-08-17 13:08:10.908459 board_automate-0.3.0/automate/model/metadata.py
--rw-r--r--   0        0        0      794 2021-08-17 13:08:10.908459 board_automate-0.3.0/automate/model/model_base.py
--rw-r--r--   0        0        0      254 2021-08-17 13:08:10.908459 board_automate-0.3.0/automate/model/user.py
--rw-r--r--   0        0        0      836 2021-08-17 13:08:10.908459 board_automate-0.3.0/automate/tasks/__init__.py
--rw-r--r--   0        0        0    18494 2023-03-05 17:26:47.179213 board_automate-0.3.0/automate/tasks/admin.py
--rw-r--r--   0        0        0     7164 2021-08-17 13:08:10.908459 board_automate-0.3.0/automate/tasks/board.py
--rw-r--r--   0        0        0     3703 2021-08-17 13:08:10.908459 board_automate-0.3.0/automate/tasks/cmake.py
--rw-r--r--   0        0        0     2738 2021-08-17 13:08:10.908459 board_automate-0.3.0/automate/tasks/common.py
--rw-r--r--   0        0        0     2143 2021-08-17 13:08:10.908459 board_automate-0.3.0/automate/tasks/compiler.py
--rw-r--r--   0        0        0     1335 2021-08-17 13:08:10.908459 board_automate-0.3.0/automate/tasks/database.py
--rw-r--r--   0        0        0     2524 2021-08-17 13:08:10.908459 board_automate-0.3.0/automate/tasks/kernel.py
--rw-r--r--   0        0        0     1582 2021-08-17 13:08:10.908459 board_automate-0.3.0/automate/tasks/make.py
--rw-r--r--   0        0        0     2155 2021-08-17 13:08:10.908459 board_automate-0.3.0/automate/utils/__init__.py
--rw-r--r--   0        0        0      303 2021-08-17 13:08:10.908459 board_automate-0.3.0/automate/utils/appdirs.py
--rw-r--r--   0        0        0     3087 2021-08-17 13:08:10.908459 board_automate-0.3.0/automate/utils/cpuinfo.py
--rw-r--r--   0        0        0     3950 2021-08-17 13:08:10.908459 board_automate-0.3.0/automate/utils/cpuinfo_arm.py
--rw-r--r--   0        0        0     5871 2021-08-17 13:08:10.908459 board_automate-0.3.0/automate/utils/kernel.py
--rw-r--r--   0        0        0     8286 2023-03-05 17:20:34.477703 board_automate-0.3.0/automate/utils/network.py
--rw-r--r--   0        0        0     3205 2021-08-17 13:08:10.908459 board_automate-0.3.0/automate/utils/uboot.py
--rw-r--r--   0        0        0     1800 2023-03-05 17:30:36.188145 board_automate-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1350 1970-01-01 00:00:00.000000 board_automate-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2022-12-12 19:32:40.802366 board_automate-0.4.0/LICENSE
+-rw-r--r--   0        0        0      348 2021-08-17 13:08:10.908459 board_automate-0.4.0/automate/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-05 17:24:23.234629 board_automate-0.4.0/automate/_vendor/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-07 16:33:28.920276 board_automate-0.4.0/automate/_vendor/patchwork/__init__.py
+-rw-r--r--   0        0        0       80 2023-06-07 16:33:28.924276 board_automate-0.4.0/automate/_vendor/patchwork/_version.py
+-rw-r--r--   0        0        0      265 2023-06-07 16:33:28.920276 board_automate-0.4.0/automate/_vendor/patchwork/environment.py
+-rw-r--r--   0        0        0     3611 2023-06-07 16:33:28.924276 board_automate-0.4.0/automate/_vendor/patchwork/files.py
+-rw-r--r--   0        0        0     1469 2023-06-07 16:33:28.920276 board_automate-0.4.0/automate/_vendor/patchwork/info.py
+-rw-r--r--   0        0        0      990 2023-06-07 16:33:28.924276 board_automate-0.4.0/automate/_vendor/patchwork/packages/__init__.py
+-rw-r--r--   0        0        0     5759 2023-06-07 16:44:21.167031 board_automate-0.4.0/automate/_vendor/patchwork/transfers.py
+-rw-r--r--   0        0        0     5260 2023-06-07 16:33:28.920276 board_automate-0.4.0/automate/_vendor/patchwork/util.py
+-rw-r--r--   0        0        0     1198 2023-03-05 17:24:23.918631 board_automate-0.4.0/automate/_vendor/patchwork-1.0.1.dist-info/DESCRIPTION.rst
+-rw-r--r--   0        0        0        4 2023-03-05 17:24:23.922632 board_automate-0.4.0/automate/_vendor/patchwork-1.0.1.dist-info/INSTALLER
+-rw-r--r--   0        0        0     1314 2023-03-05 17:24:23.918631 board_automate-0.4.0/automate/_vendor/patchwork-1.0.1.dist-info/LICENSE.txt
+-rw-r--r--   0        0        0     2574 2023-03-05 17:24:23.918631 board_automate-0.4.0/automate/_vendor/patchwork-1.0.1.dist-info/METADATA
+-rw-r--r--   0        0        0     1811 2023-03-05 17:24:23.958632 board_automate-0.4.0/automate/_vendor/patchwork-1.0.1.dist-info/RECORD
+-rw-r--r--   0        0        0        0 2023-03-05 17:24:23.958632 board_automate-0.4.0/automate/_vendor/patchwork-1.0.1.dist-info/REQUESTED
+-rw-r--r--   0        0        0      110 2023-03-05 17:24:23.918631 board_automate-0.4.0/automate/_vendor/patchwork-1.0.1.dist-info/WHEEL
+-rw-r--r--   0        0        0     1443 2023-03-05 17:24:23.918631 board_automate-0.4.0/automate/_vendor/patchwork-1.0.1.dist-info/metadata.json
+-rw-r--r--   0        0        0       10 2023-03-05 17:24:23.918631 board_automate-0.4.0/automate/_vendor/patchwork-1.0.1.dist-info/top_level.txt
+-rw-r--r--   0        0        0       80 2023-06-07 16:44:21.167031 board_automate-0.4.0/automate/_version.py
+-rw-r--r--   0        0        0    15650 2021-08-17 13:08:10.908459 board_automate-0.4.0/automate/board.py
+-rw-r--r--   0        0        0      133 2021-08-17 13:08:10.908459 board_automate-0.4.0/automate/builder/__init__.py
+-rw-r--r--   0        0        0     4794 2023-03-05 16:28:13.337031 board_automate-0.4.0/automate/builder/builder.py
+-rw-r--r--   0        0        0     6252 2021-08-17 13:08:10.908459 board_automate-0.4.0/automate/builder/cmake.py
+-rw-r--r--   0        0        0     8666 2021-08-17 13:08:10.908459 board_automate-0.4.0/automate/builder/kernel.py
+-rw-r--r--   0        0        0     3629 2021-08-17 13:08:10.908459 board_automate-0.4.0/automate/builder/make.py
+-rw-r--r--   0        0        0    13943 2021-08-17 13:08:10.908459 board_automate-0.4.0/automate/compiler.py
+-rw-r--r--   0        0        0     1020 2023-06-07 16:44:21.167031 board_automate-0.4.0/automate/config.py
+-rw-r--r--   0        0        0    15324 2023-06-07 16:44:21.167031 board_automate-0.4.0/automate/context.py
+-rw-r--r--   0        0        0       49 2021-08-17 13:08:10.908459 board_automate-0.4.0/automate/database/__init__.py
+-rw-r--r--   0        0        0    17481 2022-05-05 13:11:49.893064 board_automate-0.4.0/automate/database/database.py
+-rw-r--r--   0        0        0      109 2021-08-17 13:08:10.908459 board_automate-0.4.0/automate/database/queries/delete_lock_for_board.sql
+-rw-r--r--   0        0        0    17186 2021-08-17 13:08:10.908459 board_automate-0.4.0/automate/database/queries/init_database.sql
+-rw-r--r--   0        0        0    11009 2021-08-17 13:08:10.908459 board_automate-0.4.0/automate/database/queries/insert_board.sql
+-rw-r--r--   0        0        0      202 2021-08-17 13:08:10.908459 board_automate-0.4.0/automate/database/queries/insert_lock.sql
+-rw-r--r--   0        0        0      185 2021-08-17 13:08:10.908459 board_automate-0.4.0/automate/database/queries/select_all_boards.sql
+-rw-r--r--   0        0        0     1027 2021-08-17 13:08:10.908459 board_automate-0.4.0/automate/database/queries/select_all_cpu_cores_for_board.sql
+-rw-r--r--   0        0        0      155 2021-08-17 13:08:10.908459 board_automate-0.4.0/automate/database/queries/select_all_docs_for_board.sql
+-rw-r--r--   0        0        0      584 2021-08-17 13:08:10.908459 board_automate-0.4.0/automate/database/queries/select_all_kernels_for_os.sql
+-rw-r--r--   0        0        0      121 2021-08-17 13:08:10.908459 board_automate-0.4.0/automate/database/queries/select_lock_for_board.sql
+-rw-r--r--   0        0        0      629 2021-08-17 13:08:10.908459 board_automate-0.4.0/automate/database/queries/select_os_for_board.sql
+-rw-r--r--   0        0        0      174 2021-08-17 13:08:10.908459 board_automate-0.4.0/automate/database/queries/transfer_lock_for_board.sql
+-rw-r--r--   0        0        0      133 2021-08-17 13:08:10.908459 board_automate-0.4.0/automate/database/queries/update_lock_lease_for_board.sql
+-rw-r--r--   0        0        0      469 2021-08-17 13:08:10.908459 board_automate-0.4.0/automate/executor.py
+-rw-r--r--   0        0        0     7125 2022-05-05 13:11:49.901064 board_automate-0.4.0/automate/loader.py
+-rw-r--r--   0        0        0    12819 2022-05-05 13:11:49.905064 board_automate-0.4.0/automate/locks.py
+-rw-r--r--   0        0        0     1884 2021-08-17 13:08:10.908459 board_automate-0.4.0/automate/main.py
+-rw-r--r--   0        0        0      111 2021-08-17 13:08:10.908459 board_automate-0.4.0/automate/model/__init__.py
+-rw-r--r--   0        0        0     3614 2023-06-07 16:44:21.167031 board_automate-0.4.0/automate/model/board.py
+-rw-r--r--   0        0        0     2167 2021-08-17 13:08:10.908459 board_automate-0.4.0/automate/model/common.py
+-rw-r--r--   0        0        0      956 2021-08-17 13:08:10.908459 board_automate-0.4.0/automate/model/compiler.py
+-rw-r--r--   0        0        0      284 2021-08-17 13:08:10.908459 board_automate-0.4.0/automate/model/metadata.py
+-rw-r--r--   0        0        0      794 2021-08-17 13:08:10.908459 board_automate-0.4.0/automate/model/model_base.py
+-rw-r--r--   0        0        0      254 2021-08-17 13:08:10.908459 board_automate-0.4.0/automate/model/user.py
+-rw-r--r--   0        0        0      836 2021-08-17 13:08:10.908459 board_automate-0.4.0/automate/tasks/__init__.py
+-rw-r--r--   0        0        0    18514 2023-06-07 16:44:21.167031 board_automate-0.4.0/automate/tasks/admin.py
+-rw-r--r--   0        0        0     7164 2021-08-17 13:08:10.908459 board_automate-0.4.0/automate/tasks/board.py
+-rw-r--r--   0        0        0     3703 2021-08-17 13:08:10.908459 board_automate-0.4.0/automate/tasks/cmake.py
+-rw-r--r--   0        0        0     2878 2023-06-07 16:44:21.167031 board_automate-0.4.0/automate/tasks/common.py
+-rw-r--r--   0        0        0     2143 2021-08-17 13:08:10.908459 board_automate-0.4.0/automate/tasks/compiler.py
+-rw-r--r--   0        0        0     1335 2021-08-17 13:08:10.908459 board_automate-0.4.0/automate/tasks/database.py
+-rw-r--r--   0        0        0     2524 2021-08-17 13:08:10.908459 board_automate-0.4.0/automate/tasks/kernel.py
+-rw-r--r--   0        0        0     1582 2021-08-17 13:08:10.908459 board_automate-0.4.0/automate/tasks/make.py
+-rw-r--r--   0        0        0     2155 2021-08-17 13:08:10.908459 board_automate-0.4.0/automate/utils/__init__.py
+-rw-r--r--   0        0        0      303 2021-08-17 13:08:10.908459 board_automate-0.4.0/automate/utils/appdirs.py
+-rw-r--r--   0        0        0     3087 2021-08-17 13:08:10.908459 board_automate-0.4.0/automate/utils/cpuinfo.py
+-rw-r--r--   0        0        0     3950 2021-08-17 13:08:10.908459 board_automate-0.4.0/automate/utils/cpuinfo_arm.py
+-rw-r--r--   0        0        0     5871 2021-08-17 13:08:10.908459 board_automate-0.4.0/automate/utils/kernel.py
+-rw-r--r--   0        0        0     8304 2023-06-07 16:44:21.167031 board_automate-0.4.0/automate/utils/network.py
+-rw-r--r--   0        0        0     3205 2021-08-17 13:08:10.908459 board_automate-0.4.0/automate/utils/uboot.py
+-rw-r--r--   0        0        0     1911 2023-06-07 16:44:21.167031 board_automate-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1334 1970-01-01 00:00:00.000000 board_automate-0.4.0/PKG-INFO
```

### Comparing `board_automate-0.3.0/LICENSE` & `board_automate-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `board_automate-0.3.0/automate/_vendor/patchwork/files.py` & `board_automate-0.4.0/automate/_vendor/patchwork/files.py`

 * *Files identical despite different names*

### Comparing `board_automate-0.3.0/automate/_vendor/patchwork/info.py` & `board_automate-0.4.0/automate/_vendor/patchwork/info.py`

 * *Files identical despite different names*

### Comparing `board_automate-0.3.0/automate/_vendor/patchwork/packages/__init__.py` & `board_automate-0.4.0/automate/_vendor/patchwork/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `board_automate-0.3.0/automate/_vendor/patchwork/transfers.py` & `board_automate-0.4.0/automate/_vendor/patchwork/transfers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 File transfer functionality above and beyond basic ``put``/``get``.
 """
 
-from invoke.vendor import six
+import six
 
 
 def rsync(
     c,
     source,
     target,
     exclude=(),
```

### Comparing `board_automate-0.3.0/automate/_vendor/patchwork/util.py` & `board_automate-0.4.0/automate/_vendor/patchwork/util.py`

 * *Files identical despite different names*

### Comparing `board_automate-0.3.0/automate/_vendor/patchwork-1.0.1.dist-info/DESCRIPTION.rst` & `board_automate-0.4.0/automate/_vendor/patchwork-1.0.1.dist-info/DESCRIPTION.rst`

 * *Files identical despite different names*

### Comparing `board_automate-0.3.0/automate/_vendor/patchwork-1.0.1.dist-info/LICENSE.txt` & `board_automate-0.4.0/automate/_vendor/patchwork-1.0.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `board_automate-0.3.0/automate/_vendor/patchwork-1.0.1.dist-info/METADATA` & `board_automate-0.4.0/automate/_vendor/patchwork-1.0.1.dist-info/METADATA`

 * *Files identical despite different names*

### Comparing `board_automate-0.3.0/automate/_vendor/patchwork-1.0.1.dist-info/RECORD` & `board_automate-0.4.0/automate/_vendor/patchwork-1.0.1.dist-info/RECORD`

 * *Files identical despite different names*

### Comparing `board_automate-0.3.0/automate/_vendor/patchwork-1.0.1.dist-info/metadata.json` & `board_automate-0.4.0/automate/_vendor/patchwork-1.0.1.dist-info/metadata.json`

 * *Files identical despite different names*

### Comparing `board_automate-0.3.0/automate/board.py` & `board_automate-0.4.0/automate/board.py`

 * *Files identical despite different names*

### Comparing `board_automate-0.3.0/automate/builder/builder.py` & `board_automate-0.4.0/automate/builder/builder.py`

 * *Files identical despite different names*

### Comparing `board_automate-0.3.0/automate/builder/cmake.py` & `board_automate-0.4.0/automate/builder/cmake.py`

 * *Files identical despite different names*

### Comparing `board_automate-0.3.0/automate/builder/kernel.py` & `board_automate-0.4.0/automate/builder/kernel.py`

 * *Files identical despite different names*

### Comparing `board_automate-0.3.0/automate/builder/make.py` & `board_automate-0.4.0/automate/builder/make.py`

 * *Files identical despite different names*

### Comparing `board_automate-0.3.0/automate/compiler.py` & `board_automate-0.4.0/automate/compiler.py`

 * *Files identical despite different names*

### Comparing `board_automate-0.3.0/automate/config.py` & `board_automate-0.4.0/automate/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 from invoke.config import Config, merge_dicts
 
 
 class AutomateConfig(Config):
     """Encapsulates ~/.automate.yml"""
 
-    prefix = "automate"
-    env_prefix = "AUTOMATE"
+    prefix = "automate" # type: ignore
+    env_prefix = "AUTOMATE" # type: ignore
 
     @staticmethod
     def global_defaults() -> Any:
         their_defaults = Config.global_defaults()
 
         my_defaults = {
             "automate": {
```

### Comparing `board_automate-0.3.0/automate/context.py` & `board_automate-0.4.0/automate/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -327,17 +327,22 @@
                     finally:
                         sock.close()
 
                 time.sleep(0.1)
 
         logging.debug("Setup forwards finished")
 
-    def boards(self) -> Generator[Board, None, None]:
+    def boards(self, all=False) -> Generator[Board, None, None]:
         """Return iterator over Boards"""
         for board in sorted(self.metadata.boards, key=lambda b: b.name):
+            if not board.available and not all:
+                continue
+            if board.maintenance and not all:
+                continue
+
             yield Board(
                 self,
                 board,
                 self.metadata.compilers,
                 os.path.expanduser(self.config.automate.identity),
             )
```

### Comparing `board_automate-0.3.0/automate/database/database.py` & `board_automate-0.4.0/automate/database/database.py`

 * *Files identical despite different names*

### Comparing `board_automate-0.3.0/automate/database/queries/init_database.sql` & `board_automate-0.4.0/automate/database/queries/init_database.sql`

 * *Files identical despite different names*

### Comparing `board_automate-0.3.0/automate/database/queries/insert_board.sql` & `board_automate-0.4.0/automate/database/queries/insert_board.sql`

 * *Files identical despite different names*

### Comparing `board_automate-0.3.0/automate/database/queries/select_all_cpu_cores_for_board.sql` & `board_automate-0.4.0/automate/database/queries/select_all_cpu_cores_for_board.sql`

 * *Files identical despite different names*

### Comparing `board_automate-0.3.0/automate/database/queries/select_all_kernels_for_os.sql` & `board_automate-0.4.0/automate/database/queries/select_all_kernels_for_os.sql`

 * *Files identical despite different names*

### Comparing `board_automate-0.3.0/automate/database/queries/select_os_for_board.sql` & `board_automate-0.4.0/automate/database/queries/select_os_for_board.sql`

 * *Files identical despite different names*

### Comparing `board_automate-0.3.0/automate/loader.py` & `board_automate-0.4.0/automate/loader.py`

 * *Files identical despite different names*

### Comparing `board_automate-0.3.0/automate/locks.py` & `board_automate-0.4.0/automate/locks.py`

 * *Files identical despite different names*

### Comparing `board_automate-0.3.0/automate/main.py` & `board_automate-0.4.0/automate/main.py`

 * *Files identical despite different names*

### Comparing `board_automate-0.3.0/automate/model/board.py` & `board_automate-0.4.0/automate/model/board.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from enum import Enum
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Dict, List, Optional, Union, Literal
 
 from pydantic import BaseModel, Field, HttpUrl
 
+
 from .common import *
 from .compiler import TripleModel
 from .model_base import *
 
 
 class DocumentationLinkModel(DataModelBase):
     title: str
@@ -20,14 +21,24 @@
     port: int = 22
 
 
 class SSHConnectionModel(DataModelBase):
     host: str
     username: str
     port: int = 22
+    
+class XilinxHWServerConnectionModel(DataModelBase):
+    host: str
+    protocol: Literal["xilinx_hw"] = "xilinx_hw"
+    port: int = 3121 
+    
+class XilinxCSServerConnectionModel(DataModelBase):
+    host: str
+    protocol: Literal["xilinx_cs"] = "xilinx_cs"
+    port: int = 3121
 
 
 class UARTConnectionModel(DataModelBase):
     device: Path
     baudrate: int = 11520
 
 
@@ -98,21 +109,23 @@
     board: str
     hostname: str = ""  # FIXME use pydantic datatypes
     mac_address: str = ""  # FIXME use pydantic datatypes
     description: str
     rundir: Path
     doc: List[DocumentationLinkModel] = []
     gateway: Optional[GatewayModel] = None
-    connections: List[Union[SSHConnectionModel, UARTConnectionModel]]
-    cores: List[CoreModel]
-    os: OSModel
+    connections: List[Union[SSHConnectionModel, UARTConnectionModel, XilinxHWServerConnectionModel, XilinxCSServerConnectionModel]]
+    cores: List[CoreModel] = []
+    os: Optional[OSModel] = None
 
     soc: Optional[SOCModel] = None
     power_supply: Optional[PowerSupplyModel] = None
     reset: List[str] = []
+    available: bool =  True    # Board is theoretically available
+    maintenance: bool = False  # Board is in maintenance mode
 
     def _get_env_dict(self) -> Dict[str, str]:
         default_dict = dict(super(BoardModel, self)._get_env_dict())
 
         d = {"board": self.board, "board_name": self.name}
 
         default_dict.update(d)
```

### Comparing `board_automate-0.3.0/automate/model/common.py` & `board_automate-0.4.0/automate/model/common.py`

 * *Files identical despite different names*

### Comparing `board_automate-0.3.0/automate/model/compiler.py` & `board_automate-0.4.0/automate/model/compiler.py`

 * *Files identical despite different names*

### Comparing `board_automate-0.3.0/automate/model/model_base.py` & `board_automate-0.4.0/automate/model/model_base.py`

 * *Files identical despite different names*

### Comparing `board_automate-0.3.0/automate/tasks/__init__.py` & `board_automate-0.4.0/automate/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `board_automate-0.3.0/automate/tasks/admin.py` & `board_automate-0.4.0/automate/tasks/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import shutil
 import subprocess
 import tempfile
 from collections import namedtuple
 from enum import Enum
 from pathlib import Path
 
-import automate._vendor.patchwork.files
+import automate._vendor.patchwork.files as patchwork_files 
 from fabric import Connection, task
 from paramiko.ssh_exception import AuthenticationException
 from prompt_toolkit import prompt
 from ruamel.yaml import YAML  # type: ignore
 
 from ..loader import ModelLoader
 from ..model import (
@@ -33,15 +33,15 @@
 def add_users(c):  # pragma: no cover
     """Add users ssh keys to all boards and gateways
     """
     loader = ModelLoader(c.config)
     users = loader.load_users()
 
     def copy_keys(sftp, users, homedir):
-        patchwork.files.directory(con, "~/.ssh", mode="700")
+        patchwork_files.directory(con, "~/.ssh", mode="700")
 
         authorized_keys = homedir / ".ssh" / "authorized_keys"
         with sftp.open(str(authorized_keys), "w") as authorized_keys_file:
             for user_id, user in users.users.items():
                 authorized_keys_file.write("# {}\n".format(user_id))
                 for ssh_key in user.public_keys:
                     ssh_key = ssh_key.strip()
@@ -378,16 +378,16 @@
             default=str(identity) + ".pub",
             is_password=False,
         )
 
         with open(keyfile) as f:
             key = f.read()
 
-            patchwork.files.directory(con, "~/.ssh", mode="700")
-            patchwork.files.append(con, "~/.ssh/authorized_keys", key)
+            patchwork_files.directory(con, "~/.ssh", mode="700")
+            patchwork_files.append(con, "~/.ssh/authorized_keys", key)
 
             con.close()
 
             con = connect(
                 host,
                 user,
                 port,
```

### Comparing `board_automate-0.3.0/automate/tasks/board.py` & `board_automate-0.4.0/automate/tasks/board.py`

 * *Files identical despite different names*

### Comparing `board_automate-0.3.0/automate/tasks/cmake.py` & `board_automate-0.4.0/automate/tasks/cmake.py`

 * *Files identical despite different names*

### Comparing `board_automate-0.3.0/automate/tasks/common.py` & `board_automate-0.4.0/automate/tasks/common.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,57 +19,63 @@
 
       -b/--boards: only list boards
       -c/--compilers: only list compilers
     """
 
     if not boards and not compilers:
         boards = True
-        compilers = True
+        compilers = False
 
     if boards:
         board_table = []
         board_header = [
             "Name",
             "Machine",
             "Cores",
             "OS",
             "Connections",
             "Default Compiler",
-            "Lock Status",
+            "Status",
         ]
-        for board in c.boards():
+        for board in c.boards(all=True):
             os = getattr(board.os, "distribution", "unknown")
 
             connections = []
             for connection in board.connections:
                 s = connection_to_string(connection)
                 connections.append(s)
 
             default_compiler_name = ""
             try:
                 default_compiler_name = board.compiler().name
             except:
                 pass
 
-            lock_status = "unlocked"
+            status = "unlocked"
             if board.is_locked() or board.has_lock():
                 lock_user = board.lock_holder()
                 lock_lease_time_end = datetime.now() + board.lock_lease_time()
-                lock_status = (
+                status = (
                     f"locked by {lock_user} until {lock_lease_time_end}"
                 )
 
+            if board.maintenance: 
+                status = "maintenance"
+
+            if not board.available:
+                status = "unavailable"
+
             board_line = [
                 board.name,
                 board.board,
                 len(board.cores),
                 os,
                 ",".join(connections),
                 default_compiler_name,
-                lock_status,
+                status,
             ]
 
             board_table.append(board_line)
 
         print("Boards:")
         print(tabulate.tabulate(board_table, headers=board_header))
         print("")
```

### Comparing `board_automate-0.3.0/automate/tasks/compiler.py` & `board_automate-0.4.0/automate/tasks/compiler.py`

 * *Files identical despite different names*

### Comparing `board_automate-0.3.0/automate/tasks/database.py` & `board_automate-0.4.0/automate/tasks/database.py`

 * *Files identical despite different names*

### Comparing `board_automate-0.3.0/automate/tasks/kernel.py` & `board_automate-0.4.0/automate/tasks/kernel.py`

 * *Files identical despite different names*

### Comparing `board_automate-0.3.0/automate/tasks/make.py` & `board_automate-0.4.0/automate/tasks/make.py`

 * *Files identical despite different names*

### Comparing `board_automate-0.3.0/automate/utils/__init__.py` & `board_automate-0.4.0/automate/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `board_automate-0.3.0/automate/utils/cpuinfo.py` & `board_automate-0.4.0/automate/utils/cpuinfo.py`

 * *Files identical despite different names*

### Comparing `board_automate-0.3.0/automate/utils/cpuinfo_arm.py` & `board_automate-0.4.0/automate/utils/cpuinfo_arm.py`

 * *Files identical despite different names*

### Comparing `board_automate-0.3.0/automate/utils/kernel.py` & `board_automate-0.4.0/automate/utils/kernel.py`

 * *Files identical despite different names*

### Comparing `board_automate-0.3.0/automate/utils/network.py` & `board_automate-0.4.0/automate/utils/network.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,19 +44,20 @@
         return super().__enter__(*args, **kwargs)
 
     def __exit__(self, *args, **kwargs):
         self.close()
         return super().__exit__(*args, **kwargs)
 
     def close(self):
+        ret = super().close()
         if self.gateway is not None:
             self.gateway.close()
             self.gateway = None
 
-        return super().close()
+        return ret
 
     def __del__(self):
         self.close()
 
 
 def connect(
     host: str,
```

### Comparing `board_automate-0.3.0/automate/utils/uboot.py` & `board_automate-0.4.0/automate/utils/uboot.py`

 * *Files identical despite different names*

### Comparing `board_automate-0.3.0/pyproject.toml` & `board_automate-0.4.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 [tool.poetry]
 name = "board-automate"
-version = "0.3.0"
+version = "0.4.0"
 description = "Automate remote exection on linux based embedded boards"
 authors = ["Christoph Gerum <christoph.gerum@uni-tuebingen.de>"]
 packages = [
     { include = "automate"}
 ]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">3.7.1,<4.0"
 pydantic = "^1.10.5"
 coloredlogs = "^10.0"
 tabulate = "^0.8.6"
-invoke = "^2.0.0"
-fabric = "^3.0.0"
+fabric = "^3.1.0"
 prompt_toolkit = "^3.0"
 requests = "^2.22"
 python-dotenv = {version = "^0.10.5", optional = true}
 pydot = {version = "^1.4.1", optional = true}
 jinjasql = {version = ">0.1.7", optional = true}
 jinja2 = {version = ">3.0,<3.1", optional = true}
 keyring = "^21.1.0"
 setproctitle = "^1.1.10"
 psycopg2-binary = {version = "^2.8.6", optional = true}
 GitPython = "^3.1.27"
 ruamel-yaml = "^0.17.21"
 six = "^1.16.0"
 
+# Optional dependencies for xilinx boards
+
 [tool.poetry.extras]
 postgres = ["python-dotenv", "pydot", "psycopg2-binary", "jinjasql", "jinja"]
+xilinx = ["chipscopy"]
 
 [tool.poetry.dev-dependencies]
 mypy = ">0.740.0"
 pre-commit = ">2.0.1"
 pydoc-markdown = {version="<4.0", python=">=3.7.0,<4.0.0"}
 pytest = ">5.3"
 pytest-cov = ">2.8"
@@ -51,14 +53,17 @@
 types-tabulate = "^0.8.7"
 
 
 [tool.poetry.scripts]
 automate = 'automate.main:program.run'
 automate-run = 'automate.main:program_run.run'
 
+[tool.poetry.group.dev.dependencies]
+types-six = "^1.16.21.6"
+
 [tool.isort]
 multi_line_output=3
 include_trailing_comma=true
 force_grid_wrap=0
 use_parentheses=true
 line_length=80
```

### Comparing `board_automate-0.3.0/PKG-INFO` & `board_automate-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: board-automate
-Version: 0.3.0
+Version: 0.4.0
 Summary: Automate remote exection on linux based embedded boards
 License: MIT
 Author: Christoph Gerum
 Author-email: christoph.gerum@uni-tuebingen.de
 Requires-Python: >3.7.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: postgres
+Provides-Extra: xilinx
 Requires-Dist: GitPython (>=3.1.27,<4.0.0)
 Requires-Dist: coloredlogs (>=10.0,<11.0)
-Requires-Dist: fabric (>=3.0.0,<4.0.0)
-Requires-Dist: invoke (>=2.0.0,<3.0.0)
+Requires-Dist: fabric (>=3.1.0,<4.0.0)
 Requires-Dist: jinja2 (>3.0,<3.1)
 Requires-Dist: jinjasql (>0.1.7) ; extra == "postgres"
 Requires-Dist: keyring (>=21.1.0,<22.0.0)
 Requires-Dist: prompt_toolkit (>=3.0,<4.0)
 Requires-Dist: psycopg2-binary (>=2.8.6,<3.0.0) ; extra == "postgres"
 Requires-Dist: pydantic (>=1.10.5,<2.0.0)
 Requires-Dist: pydot (>=1.4.1,<2.0.0) ; extra == "postgres"
```

