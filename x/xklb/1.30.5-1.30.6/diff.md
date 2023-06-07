# Comparing `tmp/xklb-1.30.5.tar.gz` & `tmp/xklb-1.30.6.tar.gz`

## Comparing `xklb-1.30.5.tar` & `xklb-1.30.6.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.30.5/.gitattributes
--rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 xklb-1.30.5/TODO
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.30.5/Windows.md
--rw-r--r--   0        0        0   490403 2020-02-02 00:00:00.000000 xklb-1.30.5/pdm.lock
--rw-r--r--   0        0        0    19130 2020-02-02 00:00:00.000000 xklb-1.30.5/readme.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.30.5/.github/FUNDING.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.30.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.30.5/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 xklb-1.30.5/.github/workflows/push.yaml
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xklb-1.30.5/sql/transfer.sql
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/__init__.py
--rw-r--r--   0        0        0     8237 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/av.py
--rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/books.py
--rw-r--r--   0        0        0     7790 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/consts.py
--rw-r--r--   0        0        0     8737 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/db.py
--rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/dl_config.py
--rw-r--r--   0        0        0     9808 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/dl_extract.py
--rw-r--r--   0        0        0    14237 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/fs_extract.py
--rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/gui.py
--rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/hn_extract.py
--rw-r--r--   0        0        0    11152 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/lb.py
--rw-r--r--   0        0        0    25158 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/play_actions.py
--rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/playback.py
--rw-r--r--   0        0        0    35093 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/player.py
--rw-r--r--   0        0        0    13992 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/praw_extract.py
--rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/search.py
--rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/subtitle.py
--rw-r--r--   0        0        0     6029 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/tabs_actions.py
--rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/tabs_extract.py
--rw-r--r--   0        0        0    22847 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/tube_backend.py
--rw-r--r--   0        0        0     4877 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/tube_extract.py
--rw-r--r--   0        0        0    77219 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/usage.py
--rw-r--r--   0        0        0    37021 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     5389 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/scripts/bigdirs.py
--rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/scripts/block.py
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/scripts/christen.py
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/scripts/cluster_sort.py
--rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/scripts/copy_play_counts.py
--rw-r--r--   0        0        0     8150 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/scripts/dedupe.py
--rw-r--r--   0        0        0     5090 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/scripts/download_status.py
--rw-r--r--   0        0        0     4930 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/scripts/history.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/scripts/move_list.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     5957 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/scripts/playlists.py
--rw-r--r--   0        0        0     5986 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/scripts/relmv.py
--rw-r--r--   0        0        0     8696 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/scripts/mining/data.py
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/scripts/mining/extract_links.py
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/scripts/mining/reddit_selftext.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/assets/kotobago.png
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.30.5/.gitignore
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.30.5/LICENSE
--rw-r--r--   0        0        0    99569 2020-02-02 00:00:00.000000 xklb-1.30.5/README.md
--rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 xklb-1.30.5/pyproject.toml
--rw-r--r--   0        0        0   103165 2020-02-02 00:00:00.000000 xklb-1.30.5/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.30.6/.gitattributes
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 xklb-1.30.6/TODO
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.30.6/Windows.md
+-rw-r--r--   0        0        0   490403 2020-02-02 00:00:00.000000 xklb-1.30.6/pdm.lock
+-rw-r--r--   0        0        0    19130 2020-02-02 00:00:00.000000 xklb-1.30.6/readme.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.30.6/.github/FUNDING.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.30.6/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.30.6/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 xklb-1.30.6/.github/workflows/push.yaml
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xklb-1.30.6/sql/transfer.sql
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/__init__.py
+-rw-r--r--   0        0        0     8237 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/av.py
+-rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/books.py
+-rw-r--r--   0        0        0     7790 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/consts.py
+-rw-r--r--   0        0        0     8737 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/db.py
+-rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/dl_config.py
+-rw-r--r--   0        0        0     9808 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/dl_extract.py
+-rw-r--r--   0        0        0    14237 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/fs_extract.py
+-rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/gui.py
+-rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/hn_extract.py
+-rw-r--r--   0        0        0    11152 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/lb.py
+-rw-r--r--   0        0        0    25158 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/play_actions.py
+-rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/playback.py
+-rw-r--r--   0        0        0    35093 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/player.py
+-rw-r--r--   0        0        0    13992 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/praw_extract.py
+-rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/search.py
+-rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/subtitle.py
+-rw-r--r--   0        0        0     6029 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    22847 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/tube_backend.py
+-rw-r--r--   0        0        0     4877 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/tube_extract.py
+-rw-r--r--   0        0        0    77219 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/usage.py
+-rw-r--r--   0        0        0    37021 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     5389 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/scripts/bigdirs.py
+-rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/scripts/block.py
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/scripts/christen.py
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/scripts/cluster_sort.py
+-rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/scripts/copy_play_counts.py
+-rw-r--r--   0        0        0     8150 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/scripts/dedupe.py
+-rw-r--r--   0        0        0     5090 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/scripts/download_status.py
+-rw-r--r--   0        0        0     4930 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/scripts/history.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     5957 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/scripts/playlists.py
+-rw-r--r--   0        0        0     5986 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/scripts/relmv.py
+-rw-r--r--   0        0        0     8696 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/scripts/mining/data.py
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/scripts/mining/extract_links.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/scripts/mining/reddit_selftext.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.30.6/xklb/assets/kotobago.png
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.30.6/.gitignore
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.30.6/LICENSE
+-rw-r--r--   0        0        0    99569 2020-02-02 00:00:00.000000 xklb-1.30.6/README.md
+-rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 xklb-1.30.6/pyproject.toml
+-rw-r--r--   0        0        0   103165 2020-02-02 00:00:00.000000 xklb-1.30.6/PKG-INFO
```

### Comparing `xklb-1.30.5/TODO` & `xklb-1.30.6/TODO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 - use rowid alias instead of string pks: playlists table: switch playlist_path fk to integer id
 
-- search: get title from media table
-
 - wt/lt/search join and use fts on both tables, threading ?
 
 - POIs CLI -- save your trip plans and see places to go with automated day trip itineraries, geopandas buffer
 
 - upscale command -- download higher quality videos; use webpath, PURL, comment to get URL
 
 - move time_played, playhead, and other ephemeral data to its own table
```

### Comparing `xklb-1.30.5/Windows.md` & `xklb-1.30.6/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/pdm.lock` & `xklb-1.30.6/pdm.lock`

 * *Files 1% similar despite different names*

```diff
@@ -742,15 +742,15 @@
 name = "pycryptodomex"
 version = "3.18.0"
 requires_python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*"
 summary = "Cryptographic library for Python"
 
 [[package]]
 name = "pydantic"
-version = "1.10.8"
+version = "1.10.9"
 requires_python = ">=3.7"
 summary = "Data validation and settings management using python type hints"
 dependencies = [
     "typing-extensions>=4.2.0",
 ]
 
 [[package]]
@@ -2698,51 +2698,51 @@
     {url = "https://files.pythonhosted.org/packages/a7/c0/8ecbd1cecc470a4aed2e5b69db367de5f87692d6d40e604b5dae58b77ed6/pycryptodomex-3.18.0-cp35-abi3-macosx_10_9_x86_64.whl", hash = "sha256:302a8f37c224e7b5d72017d462a2be058e28f7be627bdd854066e16722d0fc0c"},
     {url = "https://files.pythonhosted.org/packages/b5/48/0dcad9903dc331169f4ba8bf60e5a81c41d3725ae5ccca20f590269641f5/pycryptodomex-3.18.0-cp27-cp27mu-musllinux_1_1_aarch64.whl", hash = "sha256:f237278836dda412a325e9340ba2e6a84cb0f56b9244781e5b61f10b3905de88"},
     {url = "https://files.pythonhosted.org/packages/b9/76/dae6bec36fa6a36d2579d99fc64f67038aa112598eed1fe35315332474f5/pycryptodomex-3.18.0-pp39-pypy39_pp73-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:58fc0aceb9c961b9897facec9da24c6a94c5db04597ec832060f53d4d6a07196"},
     {url = "https://files.pythonhosted.org/packages/bd/29/e1145ac172a3cc0ec70d2857ea919f87430d3f2b0727022b8f4329527faa/pycryptodomex-3.18.0-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:bbdcce0a226d9205560a5936b05208c709b01d493ed8307792075dedfaaffa5f"},
     {url = "https://files.pythonhosted.org/packages/ef/1a/1ce7e65be28111cf6115a968516074f486edf7daa5d351cb2e7269698f84/pycryptodomex-3.18.0-cp27-cp27mu-manylinux2010_x86_64.whl", hash = "sha256:8ff129a5a0eb5ff16e45ca4fa70a6051da7f3de303c33b259063c19be0c43d35"},
     {url = "https://files.pythonhosted.org/packages/f6/9f/ab0bf98fbbf4f1ee8751566b8fc6e1613c856c81f1a887736e6f2959db8e/pycryptodomex-3.18.0-cp27-cp27m-win_amd64.whl", hash = "sha256:4d9379c684efea80fdab02a3eb0169372bca7db13f9332cb67483b8dc8b67c37"},
 ]
-"pydantic 1.10.8" = [
-    {url = "https://files.pythonhosted.org/packages/05/43/e39c6bf32695f2d568ebb2f6a3dd843c8e2edb57c77a4a911d517b5675b2/pydantic-1.10.8-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:35db5301b82e8661fa9c505c800d0990bc14e9f36f98932bb1d248c0ac5cada5"},
-    {url = "https://files.pythonhosted.org/packages/0b/39/afbca0ea8e766ccf04f224520b95ca29d5a18b680c0780609a2c39293f8b/pydantic-1.10.8-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:1243d28e9b05003a89d72e7915fdb26ffd1d39bdd39b00b7dbe4afae4b557f9d"},
-    {url = "https://files.pythonhosted.org/packages/13/dc/54ceed364e733f81596a4f113de2098221b3d39b4eb7abbffa64e681f243/pydantic-1.10.8-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:666bdf6066bf6dbc107b30d034615d2627e2121506c555f73f90b54a463d1f33"},
-    {url = "https://files.pythonhosted.org/packages/15/27/c35f6fefc782aebcff9991b28728f3855b1253ff757e6dee8e3ac3815cd0/pydantic-1.10.8-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:191ba419b605f897ede9892f6c56fb182f40a15d309ef0142212200a10af4c18"},
-    {url = "https://files.pythonhosted.org/packages/23/65/2aa13873e9e0084ecaec00fbe6c6096b65e1ab99ba66bdbf7e4e7c4cc915/pydantic-1.10.8.tar.gz", hash = "sha256:1410275520dfa70effadf4c21811d755e7ef9bb1f1d077a21958153a92c8d9ca"},
-    {url = "https://files.pythonhosted.org/packages/2d/a2/e3ac01dd929485a6280518d280d8cf313558c878c91d86b3a95b1702938b/pydantic-1.10.8-cp310-cp310-win_amd64.whl", hash = "sha256:ab523c31e22943713d80d8d342d23b6f6ac4b792a1e54064a8d0cf78fd64e800"},
-    {url = "https://files.pythonhosted.org/packages/36/60/b24bd42bdd385fee681cc1231ef1d423566d4e33e867df4d2bd08b531466/pydantic-1.10.8-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:6f2e754d5566f050954727c77f094e01793bcb5725b663bf628fa6743a5a9108"},
-    {url = "https://files.pythonhosted.org/packages/56/b5/903cd28ab9a3bf8cbfbe0a6a87d9463ceac7610193cd1d72bb1bdb276d01/pydantic-1.10.8-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f90c1e29f447557e9e26afb1c4dbf8768a10cc676e3781b6a577841ade126b85"},
-    {url = "https://files.pythonhosted.org/packages/57/ce/b3de85c397a03f1c8dadebe33fa81b195b6090c840a0333769fba00693fd/pydantic-1.10.8-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:1952526ba40b220b912cdc43c1c32bcf4a58e3f192fa313ee665916b26befb68"},
-    {url = "https://files.pythonhosted.org/packages/59/ab/1de0d5386a464ef527338d320216a2f41de416e204780e00baa0e5e3b807/pydantic-1.10.8-cp38-cp38-win_amd64.whl", hash = "sha256:6a82d6cda82258efca32b40040228ecf43a548671cb174a1e81477195ed3ed56"},
-    {url = "https://files.pythonhosted.org/packages/6b/15/3504de0fcb90336680916ea3fde845d01fa846c95ab4342c28d985c0d29d/pydantic-1.10.8-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:93e766b4a8226e0708ef243e843105bf124e21331694367f95f4e3b4a92bbb3f"},
-    {url = "https://files.pythonhosted.org/packages/6c/32/0755046e707a468fe276fd40df11d492a72d1cbcfa344091e3a46120131c/pydantic-1.10.8-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:c0ab53b609c11dfc0c060d94335993cc2b95b2150e25583bec37a49b2d6c6c3f"},
-    {url = "https://files.pythonhosted.org/packages/6c/f9/5edecae1914fc7dc6a566809a5242c97d63acfb92253b0bb885d890eb953/pydantic-1.10.8-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:42aa0c4b5c3025483240a25b09f3c09a189481ddda2ea3a831a9d25f444e03c1"},
-    {url = "https://files.pythonhosted.org/packages/6f/4d/7647a5f98fbcbb9bdb1e5a77eca931a1f83255c9aa14448794a0596b5a42/pydantic-1.10.8-cp37-cp37m-win_amd64.whl", hash = "sha256:16f8c3e33af1e9bb16c7a91fc7d5fa9fe27298e9f299cff6cb744d89d573d62c"},
-    {url = "https://files.pythonhosted.org/packages/77/ea/2b96534811f867bb53edaf2a3ca5037d8bcbceb05d5930bac5caa1fba573/pydantic-1.10.8-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:1ced8375969673929809d7f36ad322934c35de4af3b5e5b09ec967c21f9f7887"},
-    {url = "https://files.pythonhosted.org/packages/7a/ba/439e2bc693d3f464946159a76724efc570cef9f4e27303fa3b360b2f3ef7/pydantic-1.10.8-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:ceb6a23bf1ba4b837d0cfe378329ad3f351b5897c8d4914ce95b85fba96da5a1"},
-    {url = "https://files.pythonhosted.org/packages/98/20/52707fc7dc91b6e580dbd30c4a6b88e426f61af9f2547bb52e880f09e67d/pydantic-1.10.8-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:12f7b0bf8553e310e530e9f3a2f5734c68699f42218bf3568ef49cd9b0e44df4"},
-    {url = "https://files.pythonhosted.org/packages/a7/27/80672dfb14e47293cca421580141ec923a1e5fe7283f775079e006b0be28/pydantic-1.10.8-cp311-cp311-win_amd64.whl", hash = "sha256:d532bf00f381bd6bc62cabc7d1372096b75a33bc197a312b03f5838b4fb84edd"},
-    {url = "https://files.pythonhosted.org/packages/b2/43/8eca9ebbfd861209365c5b9f982b113275eccd892e53ab7bde60a21439e8/pydantic-1.10.8-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:34d327c81e68a1ecb52fe9c8d50c8a9b3e90d3c8ad991bfc8f953fb477d42fb4"},
-    {url = "https://files.pythonhosted.org/packages/b8/45/538d65960c489a1aa9cbf1f54d4b911e1e838d557d2d2ccd1b6c8fa10f3b/pydantic-1.10.8-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:17aef11cc1b997f9d574b91909fed40761e13fac438d72b81f902226a69dac01"},
-    {url = "https://files.pythonhosted.org/packages/c1/37/d136df986c0a2d20f940d360fe472ae410fba46f55a73e872fd3168f4289/pydantic-1.10.8-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:0c6fafa0965b539d7aab0a673a046466d23b86e4b0e8019d25fd53f4df62c277"},
-    {url = "https://files.pythonhosted.org/packages/c4/f3/c5dc9f49783a6407487d20c9a32bca878ebf2df155b8d2858838d79b6d46/pydantic-1.10.8-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:bb14388ec45a7a0dc429e87def6396f9e73c8c77818c927b6a60706603d5f2ea"},
-    {url = "https://files.pythonhosted.org/packages/c5/58/71d48d4154e5845192f4ccc6c6ebcf6fa5286fa3bcb3c595aa18a5bf599d/pydantic-1.10.8-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:e82d4566fcd527eae8b244fa952d99f2ca3172b7e97add0b43e2d97ee77f81ab"},
-    {url = "https://files.pythonhosted.org/packages/ca/5b/8b2c49589c826bf2796fc523d77d46fed2e82585c87c812f289ce244c88b/pydantic-1.10.8-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:2e4148e635994d57d834be1182a44bdb07dd867fa3c2d1b37002000646cc5459"},
-    {url = "https://files.pythonhosted.org/packages/cc/a4/354a73bb8a06df0df0bc74b5fbf3b9510ed4900185f86a00861dcfbe60c7/pydantic-1.10.8-py3-none-any.whl", hash = "sha256:7456eb22ed9aaa24ff3e7b4757da20d9e5ce2a81018c1b3ebd81a0b88a18f3b2"},
-    {url = "https://files.pythonhosted.org/packages/d8/7b/ca035af1833c6d047eeb328438a2ae402d03929be2055cd66294542a814d/pydantic-1.10.8-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:052d8654cb65174d6f9490cc9b9a200083a82cf5c3c5d3985db765757eb3b375"},
-    {url = "https://files.pythonhosted.org/packages/dc/92/3a09ec18592ca6fc96223b42ad20c8711847a8d2e1800779f9206c2fa6a2/pydantic-1.10.8-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:df7800cb1984d8f6e249351139667a8c50a379009271ee6236138a22a0c0f319"},
-    {url = "https://files.pythonhosted.org/packages/e2/21/e6f68631ec2f0470e28722d1ca352bac4f25aef6eb18b8e65ba3cd9ae8a2/pydantic-1.10.8-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:7b1f6cb446470b7ddf86c2e57cd119a24959af2b01e552f60705910663af09a4"},
-    {url = "https://files.pythonhosted.org/packages/e6/dd/6f9ef794df128746581bd5886c6382a19f1729ff39f3d65e66e3b6751c7a/pydantic-1.10.8-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:c33b60054b2136aef8cf190cd4c52a3daa20b2263917c49adad20eaf381e823b"},
-    {url = "https://files.pythonhosted.org/packages/e7/a3/329824b0e46edcb2c51f0fa73678f24aba083289697a0db3036f4f30e1ed/pydantic-1.10.8-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:3e59417ba8a17265e632af99cc5f35ec309de5980c440c255ab1ca3ae96a3e0e"},
-    {url = "https://files.pythonhosted.org/packages/e8/b3/b748afd5f4fd8f640e08cf4828fa5c9da865353eade18b9c789726b1a0ce/pydantic-1.10.8-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f9613fadad06b4f3bc5db2653ce2f22e0de84a7c6c293909b48f6ed37b83c61f"},
-    {url = "https://files.pythonhosted.org/packages/e9/17/a840d0631a288a4400e23a9ec96d131bd07be820fe2c1d070995de6dfb61/pydantic-1.10.8-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:93e6bcfccbd831894a6a434b0aeb1947f9e70b7468f274154d03d71fabb1d7c6"},
-    {url = "https://files.pythonhosted.org/packages/fa/3b/279a13153350b688fb5eb557acf980059a21ffede20d9b6fbc5368778bf4/pydantic-1.10.8-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:84d80219c3f8d4cad44575e18404099c76851bc924ce5ab1c4c8bb5e2a2227d0"},
-    {url = "https://files.pythonhosted.org/packages/fb/46/723587abb4aecf82edcfaa213a827d61854ebcbf76b4818cbf59c8868f4e/pydantic-1.10.8-cp39-cp39-win_amd64.whl", hash = "sha256:66a703d1983c675a6e0fed8953b0971c44dba48a929a2000a493c3772eb61a5a"},
-    {url = "https://files.pythonhosted.org/packages/fe/26/66c9ac1e21a3bda4f5c10785b3ff199e12e2d1e984780a8bfa796bb4e2f0/pydantic-1.10.8-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:7d5b8641c24886d764a74ec541d2fc2c7fb19f6da2a4001e6d580ba4a38f7878"},
-    {url = "https://files.pythonhosted.org/packages/ff/b4/b56bd5f591969df63a260555a891bf953536eefcbe66b711b80f86acc3a4/pydantic-1.10.8-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:88f195f582851e8db960b4a94c3e3ad25692c1c1539e2552f3df7a9e972ef60e"},
+"pydantic 1.10.9" = [
+    {url = "https://files.pythonhosted.org/packages/02/05/1c505fd7cc174ddecd5aa956057638ba6039b584af6fa9687f11a074fca7/pydantic-1.10.9-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:83fcff3c7df7adff880622a98022626f4f6dbce6639a88a15a3ce0f96466cb60"},
+    {url = "https://files.pythonhosted.org/packages/0a/53/5dbbfac34a8040d9af562287d7604d001170b88aa0df6789ce670aa77718/pydantic-1.10.9-cp37-cp37m-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:2196c06484da2b3fded1ab6dbe182bdabeb09f6318b7fdc412609ee2b564c49a"},
+    {url = "https://files.pythonhosted.org/packages/0e/7a/6d5d0cd7155a9625a78860698b2efe992eb9539eeddbeca099e34b0b0bb5/pydantic-1.10.9-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:67195274fd27780f15c4c372f4ba9a5c02dad6d50647b917b6a92bf00b3d301a"},
+    {url = "https://files.pythonhosted.org/packages/0f/2e/e22c5765f342d8250edf706c6852c241d1c0696387464343026e47f92399/pydantic-1.10.9-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:f50e1764ce9353be67267e7fd0da08349397c7db17a562ad036aa7c8f4adfdb6"},
+    {url = "https://files.pythonhosted.org/packages/1b/36/d0699cae7a41eb741175321ec338095d9981d05661a543b1705b35fcf7fa/pydantic-1.10.9-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:3283b574b01e8dbc982080d8287c968489d25329a463b29a90d4157de4f2baaf"},
+    {url = "https://files.pythonhosted.org/packages/1c/09/2395aebb2363026f23599df9c79353111ba0921d9b5fa188fc63065d605f/pydantic-1.10.9-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:e692dec4a40bfb40ca530e07805b1208c1de071a18d26af4a2a0d79015b352ca"},
+    {url = "https://files.pythonhosted.org/packages/1d/ac/d9b98a37670d755f2488dba7e2b3a91e1f4123fe32c726827a03a24af7b1/pydantic-1.10.9-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:939328fd539b8d0edf244327398a667b6b140afd3bf7e347cf9813c736211896"},
+    {url = "https://files.pythonhosted.org/packages/25/7d/b15e5da706957af6a570a2155ad80db47a82f1fe343beb9903b38adbb6a3/pydantic-1.10.9-cp311-cp311-win_amd64.whl", hash = "sha256:7845b31959468bc5b78d7b95ec52fe5be32b55d0d09983a877cca6aedc51068f"},
+    {url = "https://files.pythonhosted.org/packages/26/8f/8d93aae2517f702858b16d11bb3b740fa57cf00d2f986026ff852e1d6993/pydantic-1.10.9-cp39-cp39-win_amd64.whl", hash = "sha256:e7c9900b43ac14110efa977be3da28931ffc74c27e96ee89fbcaaf0b0fe338e1"},
+    {url = "https://files.pythonhosted.org/packages/2d/8b/00fa25d377e804bb78e2d9c0cf75363d16e92bb7b6359aec825175520b12/pydantic-1.10.9-cp39-cp39-musllinux_1_1_i686.whl", hash = "sha256:0a2aabdc73c2a5960e87c3ffebca6ccde88665616d1fd6d3db3178ef427b267a"},
+    {url = "https://files.pythonhosted.org/packages/2d/ba/7d8c23a4c80bf33c3bffc66e98818087d1662eeaa44bdadb58bfbfcbd10f/pydantic-1.10.9-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:d111a21bbbfd85c17248130deac02bbd9b5e20b303338e0dbe0faa78330e37e0"},
+    {url = "https://files.pythonhosted.org/packages/35/2c/eadcfc255b5ba09113ba2cef4910355656116591947e8251ef03e14ac2b4/pydantic-1.10.9-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:b48d3d634bca23b172f47f2335c617d3fcb4b3ba18481c96b7943a4c634f5c8d"},
+    {url = "https://files.pythonhosted.org/packages/3d/dc/e6c3abd1e486c32ace48c0a5f545865f54c934ce809192aaa56e10989ed6/pydantic-1.10.9-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:7847ca62e581e6088d9000f3c497267868ca2fa89432714e21a4fb33a04d52e8"},
+    {url = "https://files.pythonhosted.org/packages/45/3c/23b1d0ca338ee91ad45057a4ef1130282bf155a3b45c9e82d2adf89ddceb/pydantic-1.10.9-cp39-cp39-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:0da48717dc9495d3a8f215e0d012599db6b8092db02acac5e0d58a65248ec5bc"},
+    {url = "https://files.pythonhosted.org/packages/46/a2/8b29ba7ff9666ad96e23258d317fbf63f66c397801a274e352fc532ab901/pydantic-1.10.9-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:9863b9420d99dfa9c064042304868e8ba08e89081428a1c471858aa2af6f57c4"},
+    {url = "https://files.pythonhosted.org/packages/5b/31/e773155df3b875f5c7af23a5a8db5f8b9f06526cc08bc20a02c07d24f263/pydantic-1.10.9-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:f0b7628fb8efe60fe66fd4adadd7ad2304014770cdc1f4934db41fe46cc8825f"},
+    {url = "https://files.pythonhosted.org/packages/63/c3/a79f780b1e52b2e836f489f09710451e110114be5eede5dcaa57535d7a7d/pydantic-1.10.9-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:b9cd67fb763248cbe38f0593cd8611bfe4b8ad82acb3bdf2b0898c23415a1f82"},
+    {url = "https://files.pythonhosted.org/packages/66/a8/85ce916a7be8f601782b5a4162ddfedafccbb7ab61b1b409507aab7f9913/pydantic-1.10.9-cp310-cp310-win_amd64.whl", hash = "sha256:eec39224b2b2e861259d6f3c8b6290d4e0fbdce147adb797484a42278a1a486f"},
+    {url = "https://files.pythonhosted.org/packages/6a/88/4979f837c8ec013761610ea7c27f0fc99bcc7e06ece6c239fafff1b282f5/pydantic-1.10.9-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:3c52eb595db83e189419bf337b59154bdcca642ee4b2a09e5d7797e41ace783f"},
+    {url = "https://files.pythonhosted.org/packages/7b/54/6843930a0a0632e8431a3d2071e253e1bddd1ac41ea32ae40897497cd14f/pydantic-1.10.9-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:2e9aec8627a1a6823fc62fb96480abe3eb10168fd0d859ee3d3b395105ae19a7"},
+    {url = "https://files.pythonhosted.org/packages/8b/7b/41b331751b75cc215724c49646bef438fb23f4d1e3938e07fd5a10178b67/pydantic-1.10.9-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:7e1d5290044f620f80cf1c969c542a5468f3656de47b41aa78100c5baa2b8276"},
+    {url = "https://files.pythonhosted.org/packages/8c/ea/1483d76e4048af279fe7f49f35ea0fce6ec34d6b0276c775618204121cd0/pydantic-1.10.9-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:4b466a23009ff5cdd7076eb56aca537c745ca491293cc38e72bf1e0e00de5b91"},
+    {url = "https://files.pythonhosted.org/packages/a5/2a/dbc7a80b6192cc49efb27dc9c29965911ce7aef95c11466989ffcf0b0784/pydantic-1.10.9-cp38-cp38-win_amd64.whl", hash = "sha256:963671eda0b6ba6926d8fc759e3e10335e1dc1b71ff2a43ed2efd6996634dafb"},
+    {url = "https://files.pythonhosted.org/packages/b5/e9/5ffcdbe8ceb1ac23184b16bbd90fb5f20cdf1022e658d864c7782a32bc40/pydantic-1.10.9-cp38-cp38-musllinux_1_1_i686.whl", hash = "sha256:ad428e92ab68798d9326bb3e5515bc927444a3d71a93b4a2ca02a8a5d795c572"},
+    {url = "https://files.pythonhosted.org/packages/b8/38/d956a7a25c962a0b231a33fc4323c31177920cd6f0cdea69e0225369dad0/pydantic-1.10.9-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:970b1bdc6243ef663ba5c7e36ac9ab1f2bfecb8ad297c9824b542d41a750b298"},
+    {url = "https://files.pythonhosted.org/packages/bd/d2/703bfdc4a17f4c20d0d76fd447266a8e5e58208b4a75aaa2aa3534f9000b/pydantic-1.10.9-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:fab81a92f42d6d525dd47ced310b0c3e10c416bbfae5d59523e63ea22f82b31e"},
+    {url = "https://files.pythonhosted.org/packages/c0/82/a14d25985fbfe7be8ba871db8d6a972c1bd9af8a904425b335ce37830b80/pydantic-1.10.9-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:7ee829b86ce984261d99ff2fd6e88f2230068d96c2a582f29583ed602ef3fc2c"},
+    {url = "https://files.pythonhosted.org/packages/c7/5e/d2f760680276a015b7b9a3ccd66e4ab7924d3ee425fcf59daa949dc2ae79/pydantic-1.10.9-cp37-cp37m-win_amd64.whl", hash = "sha256:5f8bbaf4013b9a50e8100333cc4e3fa2f81214033e05ac5aa44fa24a98670a29"},
+    {url = "https://files.pythonhosted.org/packages/ca/1a/78c25abfc36fd22ae79042dc26692cfead3fc03eeb5dbaae50536f1bc9c1/pydantic-1.10.9-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:e1aa5c2410769ca28aa9a7841b80d9d9a1c5f223928ca8bec7e7c9a34d26b1d4"},
+    {url = "https://files.pythonhosted.org/packages/ce/4c/56283ddccc9cf5f4fabad21b0fec0f28867225c0cedd9ef3432872bf9456/pydantic-1.10.9-cp38-cp38-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:128d9453d92e6e81e881dd7e2484e08d8b164da5507f62d06ceecf84bf2e21d3"},
+    {url = "https://files.pythonhosted.org/packages/ce/80/92bdb68e1fda29be502adfd0b95c4cdef41f498a35125d0d540d4696c091/pydantic-1.10.9-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:07293ab08e7b4d3c9d7de4949a0ea571f11e4557d19ea24dd3ae0c524c0c334d"},
+    {url = "https://files.pythonhosted.org/packages/cf/6b/19bc450d7d51ed7e5eddfe2e09f10bd054b8e766526fbf1e6735d185039e/pydantic-1.10.9-cp37-cp37m-musllinux_1_1_i686.whl", hash = "sha256:6257bb45ad78abacda13f15bde5886efd6bf549dd71085e64b8dcf9919c38b60"},
+    {url = "https://files.pythonhosted.org/packages/d5/27/29f43b7148eb3d6e5fdd14935e88f03b6b501baddf88fb6913da7f3f7661/pydantic-1.10.9-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:73ef93e5e1d3c8e83f1ff2e7fdd026d9e063c7e089394869a6e2985696693766"},
+    {url = "https://files.pythonhosted.org/packages/e1/36/9d92178cba055627c891f3a57b660d2d4e6fe84419a520d16a677050b4e1/pydantic-1.10.9-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:517a681919bf880ce1dac7e5bc0c3af1e58ba118fd774da2ffcd93c5f96eaece"},
+    {url = "https://files.pythonhosted.org/packages/ec/0a/cf955f8bb3b9498d554522cfe7cb9b019ba9f8b86e2879009f604207b72c/pydantic-1.10.9.tar.gz", hash = "sha256:95c70da2cd3b6ddf3b9645ecaa8d98f3d80c606624b6d245558d202cd23ea3be"},
+    {url = "https://files.pythonhosted.org/packages/ed/8c/278ece6217c6dc15ab588e2b68d3d9953b426648f70444eed93eb61f8d30/pydantic-1.10.9-py3-none-any.whl", hash = "sha256:6cafde02f6699ce4ff643417d1a9223716ec25e228ddc3b436fe7e2d25a1f305"},
 ]
 "pyexiftool 0.5.5" = [
     {url = "https://files.pythonhosted.org/packages/78/04/10ac8e25bfbfd6297194e1fefdeaba1cc981ae2f5a36dd03ba30db3bbee0/PyExifTool-0.5.5.tar.gz", hash = "sha256:9dce4638c1d4d1b3414eb4e720647582f2ec14e940f97e42d4ba202580e04a66"},
     {url = "https://files.pythonhosted.org/packages/bd/fb/ffb698a0e3d8e1f45a051be009b6dd4494bd665b165ec28c594bb535cec7/PyExifTool-0.5.5-py3-none-any.whl", hash = "sha256:7048aab1cb83726d7bf0113a5acb9d9d52f9e16817e39595fa59c8ea0563bf5a"},
 ]
 "pygments 2.15.1" = [
     {url = "https://files.pythonhosted.org/packages/34/a7/37c8d68532ba71549db4212cb036dbd6161b40e463aba336770e80c72f84/Pygments-2.15.1-py3-none-any.whl", hash = "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"},
```

### Comparing `xklb-1.30.5/readme.py` & `xklb-1.30.6/readme.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/.github/ISSUE_TEMPLATE/bug_report.md` & `xklb-1.30.6/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/.github/ISSUE_TEMPLATE/feature_request.md` & `xklb-1.30.6/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/.github/workflows/push.yaml` & `xklb-1.30.6/.github/workflows/push.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 name: PyTest and Publish
 
 on:
   push:
     tags: ['v[0-9].[0-9]+.[0-9]+']
-    paths-ignore:
-      - 'README.md'
-      - 'examples/**'
 
 jobs:
   test:
     strategy:
       fail-fast: false
       max-parallel: 8
       matrix:
```

### Comparing `xklb-1.30.5/sql/transfer.sql` & `xklb-1.30.6/sql/transfer.sql`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/xklb/av.py` & `xklb-1.30.6/xklb/av.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/xklb/books.py` & `xklb-1.30.6/xklb/books.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/xklb/consts.py` & `xklb-1.30.6/xklb/consts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/xklb/db.py` & `xklb-1.30.6/xklb/db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/xklb/dl_config.py` & `xklb-1.30.6/xklb/dl_config.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/xklb/dl_extract.py` & `xklb-1.30.6/xklb/dl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/xklb/fs_extract.py` & `xklb-1.30.6/xklb/fs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/xklb/gui.py` & `xklb-1.30.6/xklb/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/xklb/hn_extract.py` & `xklb-1.30.6/xklb/hn_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/xklb/lb.py` & `xklb-1.30.6/xklb/lb.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/xklb/play_actions.py` & `xklb-1.30.6/xklb/play_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/xklb/playback.py` & `xklb-1.30.6/xklb/playback.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/xklb/player.py` & `xklb-1.30.6/xklb/player.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/xklb/praw_extract.py` & `xklb-1.30.6/xklb/praw_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/xklb/search.py` & `xklb-1.30.6/xklb/search.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/xklb/subtitle.py` & `xklb-1.30.6/xklb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/xklb/tabs_actions.py` & `xklb-1.30.6/xklb/tabs_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/xklb/tabs_extract.py` & `xklb-1.30.6/xklb/tabs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/xklb/tube_backend.py` & `xklb-1.30.6/xklb/tube_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/xklb/tube_extract.py` & `xklb-1.30.6/xklb/tube_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/xklb/usage.py` & `xklb-1.30.6/xklb/usage.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/xklb/utils.py` & `xklb-1.30.6/xklb/utils.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/xklb/scripts/bigdirs.py` & `xklb-1.30.6/xklb/scripts/bigdirs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/xklb/scripts/block.py` & `xklb-1.30.6/xklb/scripts/block.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/xklb/scripts/christen.py` & `xklb-1.30.6/xklb/scripts/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/xklb/scripts/cluster_sort.py` & `xklb-1.30.6/xklb/scripts/cluster_sort.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/xklb/scripts/copy_play_counts.py` & `xklb-1.30.6/xklb/scripts/copy_play_counts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/xklb/scripts/dedupe.py` & `xklb-1.30.6/xklb/scripts/dedupe.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/xklb/scripts/download_status.py` & `xklb-1.30.6/xklb/scripts/download_status.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/xklb/scripts/history.py` & `xklb-1.30.6/xklb/scripts/history.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/xklb/scripts/merge_dbs.py` & `xklb-1.30.6/xklb/scripts/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/xklb/scripts/merge_online_local.py` & `xklb-1.30.6/xklb/scripts/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/xklb/scripts/move_list.py` & `xklb-1.30.6/xklb/scripts/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/xklb/scripts/optimize_db.py` & `xklb-1.30.6/xklb/scripts/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/xklb/scripts/playlists.py` & `xklb-1.30.6/xklb/scripts/playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/xklb/scripts/redownload.py` & `xklb-1.30.6/xklb/scripts/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/xklb/scripts/relmv.py` & `xklb-1.30.6/xklb/scripts/relmv.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/xklb/scripts/scatter.py` & `xklb-1.30.6/xklb/scripts/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/xklb/scripts/streaming_tab_loader.py` & `xklb-1.30.6/xklb/scripts/streaming_tab_loader.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/xklb/scripts/mining/data.py` & `xklb-1.30.6/xklb/scripts/mining/data.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/xklb/scripts/mining/extract_links.py` & `xklb-1.30.6/xklb/scripts/mining/extract_links.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/xklb/scripts/mining/nouns.py` & `xklb-1.30.6/xklb/scripts/mining/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/xklb/scripts/mining/pushshift.py` & `xklb-1.30.6/xklb/scripts/mining/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/xklb/scripts/mining/reddit_selftext.py` & `xklb-1.30.6/xklb/scripts/mining/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/xklb/assets/kotobago.png` & `xklb-1.30.6/xklb/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/.gitignore` & `xklb-1.30.6/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/LICENSE` & `xklb-1.30.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/README.md` & `xklb-1.30.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 Incremental surfing. 📈🏄 totally rad!
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.30.005)
+    xk media library subcommands (v1.30.006)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

### Comparing `xklb-1.30.5/pyproject.toml` & `xklb-1.30.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xklb-1.30.5/PKG-INFO` & `xklb-1.30.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xklb
-Version: 1.30.5
+Version: 1.30.6
 Summary: xk library
 Project-URL: documentation, https://github.com/chapmanjacobd/library/wiki/Usage
 Project-URL: homepage, https://github.com/chapmanjacobd/library/
 Project-URL: repository, https://github.com/chapmanjacobd/library/
 Author-email: Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>
 License: BSD 3-Clause No Nuclear License
         
@@ -223,15 +223,15 @@
 Incremental surfing. 📈🏄 totally rad!
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.30.005)
+    xk media library subcommands (v1.30.006)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

