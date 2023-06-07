# Comparing `tmp/xklb-1.30.2.tar.gz` & `tmp/xklb-1.30.3.tar.gz`

## Comparing `xklb-1.30.2.tar` & `xklb-1.30.3.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.30.2/.gitattributes
--rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 xklb-1.30.2/TODO
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.30.2/Windows.md
--rw-r--r--   0        0        0   489912 2020-02-02 00:00:00.000000 xklb-1.30.2/pdm.lock
--rw-r--r--   0        0        0    19066 2020-02-02 00:00:00.000000 xklb-1.30.2/readme.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.30.2/.github/FUNDING.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.30.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.30.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 xklb-1.30.2/.github/workflows/push.yaml
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xklb-1.30.2/sql/transfer.sql
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/__init__.py
--rw-r--r--   0        0        0     8237 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/av.py
--rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/books.py
--rw-r--r--   0        0        0     7847 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/consts.py
--rw-r--r--   0        0        0     8737 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/db.py
--rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/dl_config.py
--rw-r--r--   0        0        0     9808 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/dl_extract.py
--rw-r--r--   0        0        0    14237 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/fs_extract.py
--rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/gui.py
--rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/hn_extract.py
--rw-r--r--   0        0        0    11152 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/lb.py
--rw-r--r--   0        0        0    25158 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/play_actions.py
--rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/playback.py
--rw-r--r--   0        0        0    35093 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/player.py
--rw-r--r--   0        0        0    13992 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/praw_extract.py
--rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/search.py
--rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/subtitle.py
--rw-r--r--   0        0        0     6029 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/tabs_actions.py
--rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/tabs_extract.py
--rw-r--r--   0        0        0    22742 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/tube_backend.py
--rw-r--r--   0        0        0     4845 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/tube_extract.py
--rw-r--r--   0        0        0    77169 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/usage.py
--rw-r--r--   0        0        0    37021 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     5389 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/scripts/bigdirs.py
--rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/scripts/block.py
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/scripts/christen.py
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/scripts/cluster_sort.py
--rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/scripts/copy_play_counts.py
--rw-r--r--   0        0        0     8150 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/scripts/dedupe.py
--rw-r--r--   0        0        0     5090 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/scripts/download_status.py
--rw-r--r--   0        0        0     4930 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/scripts/history.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/scripts/move_list.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     5957 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/scripts/playlists.py
--rw-r--r--   0        0        0     5986 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/scripts/relmv.py
--rw-r--r--   0        0        0     8696 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/scripts/mining/data.py
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/scripts/mining/extract_links.py
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/scripts/mining/reddit_selftext.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.30.2/xklb/assets/kotobago.png
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.30.2/.gitignore
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.30.2/LICENSE
--rw-r--r--   0        0        0    99455 2020-02-02 00:00:00.000000 xklb-1.30.2/README.md
--rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 xklb-1.30.2/pyproject.toml
--rw-r--r--   0        0        0   103051 2020-02-02 00:00:00.000000 xklb-1.30.2/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.30.3/.gitattributes
+-rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 xklb-1.30.3/TODO
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.30.3/Windows.md
+-rw-r--r--   0        0        0   489912 2020-02-02 00:00:00.000000 xklb-1.30.3/pdm.lock
+-rw-r--r--   0        0        0    19066 2020-02-02 00:00:00.000000 xklb-1.30.3/readme.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.30.3/.github/FUNDING.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.30.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.30.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 xklb-1.30.3/.github/workflows/push.yaml
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xklb-1.30.3/sql/transfer.sql
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/__init__.py
+-rw-r--r--   0        0        0     8237 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/av.py
+-rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/books.py
+-rw-r--r--   0        0        0     7790 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/consts.py
+-rw-r--r--   0        0        0     8737 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/db.py
+-rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/dl_config.py
+-rw-r--r--   0        0        0     9808 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/dl_extract.py
+-rw-r--r--   0        0        0    14237 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/fs_extract.py
+-rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/gui.py
+-rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/hn_extract.py
+-rw-r--r--   0        0        0    11152 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/lb.py
+-rw-r--r--   0        0        0    25158 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/play_actions.py
+-rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/playback.py
+-rw-r--r--   0        0        0    35093 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/player.py
+-rw-r--r--   0        0        0    13992 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/praw_extract.py
+-rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/search.py
+-rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/subtitle.py
+-rw-r--r--   0        0        0     6029 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    22847 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/tube_backend.py
+-rw-r--r--   0        0        0     5463 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/tube_extract.py
+-rw-r--r--   0        0        0    77169 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/usage.py
+-rw-r--r--   0        0        0    37021 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     5389 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/scripts/bigdirs.py
+-rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/scripts/block.py
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/scripts/christen.py
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/scripts/cluster_sort.py
+-rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/scripts/copy_play_counts.py
+-rw-r--r--   0        0        0     8150 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/scripts/dedupe.py
+-rw-r--r--   0        0        0     5090 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/scripts/download_status.py
+-rw-r--r--   0        0        0     4930 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/scripts/history.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     5957 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/scripts/playlists.py
+-rw-r--r--   0        0        0     5986 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/scripts/relmv.py
+-rw-r--r--   0        0        0     8696 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/scripts/mining/data.py
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/scripts/mining/extract_links.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/scripts/mining/reddit_selftext.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/assets/kotobago.png
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.30.3/.gitignore
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.30.3/LICENSE
+-rw-r--r--   0        0        0    99455 2020-02-02 00:00:00.000000 xklb-1.30.3/README.md
+-rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 xklb-1.30.3/pyproject.toml
+-rw-r--r--   0        0        0   103051 2020-02-02 00:00:00.000000 xklb-1.30.3/PKG-INFO
```

### Comparing `xklb-1.30.2/TODO` & `xklb-1.30.3/TODO`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/Windows.md` & `xklb-1.30.3/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/pdm.lock` & `xklb-1.30.3/pdm.lock`

 * *Files 0% similar despite different names*

```diff
@@ -881,15 +881,15 @@
     "markdown-it-py<3.0.0,>=2.2.0",
     "pygments<3.0.0,>=2.13.0",
     "typing-extensions<5.0,>=4.0.0; python_version < \"3.9\"",
 ]
 
 [[package]]
 name = "ruff"
-version = "0.0.270"
+version = "0.0.271"
 requires_python = ">=3.7"
 summary = "An extremely fast Python linter, written in Rust."
 
 [[package]]
 name = "scalene"
 version = "1.5.19"
 requires_python = ">=3.8"
@@ -2898,32 +2898,32 @@
     {url = "https://files.pythonhosted.org/packages/45/1e/0c169c6a5381e241ba7404532c16a21d86ab872c9bed8bdcd4c423954103/requests-2.24.0-py2.py3-none-any.whl", hash = "sha256:fe75cc94a9443b9246fc7049224f75604b113c36acb93f87b80ed42c44cbb898"},
     {url = "https://files.pythonhosted.org/packages/da/67/672b422d9daf07365259958912ba533a0ecab839d4084c487a5fe9a5405f/requests-2.24.0.tar.gz", hash = "sha256:b3559a131db72c33ee969480840fff4bb6dd111de7dd27c8ee1f820f4f00231b"},
 ]
 "rich 13.4.1" = [
     {url = "https://files.pythonhosted.org/packages/02/97/0046b5e3c6a5057b5817e5e6c51a776d410b953e6a9c67ae249dafdd2999/rich-13.4.1.tar.gz", hash = "sha256:76f6b65ea7e5c5d924ba80e322231d7cb5b5981aa60bfc1e694f1bc097fe6fe1"},
     {url = "https://files.pythonhosted.org/packages/ea/93/c68645c689d10a035010e3ae314b6b2855d040ce0d11fdfdfbb8be416581/rich-13.4.1-py3-none-any.whl", hash = "sha256:d204aadb50b936bf6b1a695385429d192bc1fdaf3e8b907e8e26f4c4e4b5bf75"},
 ]
-"ruff 0.0.270" = [
-    {url = "https://files.pythonhosted.org/packages/02/d1/77f9425bea1e5a929ecbeb3fd9e2e0931e30751b4d75bbe8b46e14408ada/ruff-0.0.270-py3-none-macosx_10_9_x86_64.macosx_11_0_arm64.macosx_10_9_universal2.whl", hash = "sha256:643de865fd35cb76c4f0739aea5afe7b8e4d40d623df7e9e6ea99054e5cead0a"},
-    {url = "https://files.pythonhosted.org/packages/06/56/39079c40dc7e995f26f630d28dec11b1b63f498bfb56409adda27300bf2f/ruff-0.0.270-py3-none-win_amd64.whl", hash = "sha256:0012f9b7dc137ab7f1f0355e3c4ca49b562baf6c9fa1180948deeb6648c52957"},
-    {url = "https://files.pythonhosted.org/packages/36/21/aa8e1d22756e1d3bcdb43f4d25451f8978cacd9d6896e365bb7c1f9037fa/ruff-0.0.270-py3-none-manylinux_2_17_ppc64.manylinux2014_ppc64.whl", hash = "sha256:08188f8351f4c0b6216e8463df0a76eb57894ca59a3da65e4ed205db980fd3ae"},
-    {url = "https://files.pythonhosted.org/packages/36/ab/ff2870e22556c780d6b0b2934152e824ca0d3d40d9e3dedb44a158a979dc/ruff-0.0.270-py3-none-musllinux_1_2_i686.whl", hash = "sha256:0bbfbf6fd2436165566ca85f6e57be03ed2f0a994faf40180cfbb3604c9232ef"},
-    {url = "https://files.pythonhosted.org/packages/40/82/c393794c4cd462ffbd0afe45b8e77c174c7f3d5df4340ecead9a42d1fa53/ruff-0.0.270-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:0827b074635d37984fc98d99316bfab5c8b1231bb83e60dacc83bd92883eedb4"},
-    {url = "https://files.pythonhosted.org/packages/57/2f/3f964a1d0208248f3c51441a9e59690c8ac6f33422a0f0918521743c9f16/ruff-0.0.270-py3-none-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:0d61ae4841313f6eeb8292dc349bef27b4ce426e62c36e80ceedc3824e408734"},
-    {url = "https://files.pythonhosted.org/packages/5a/22/e4e4d9219993e3b7f34ba16b9b14176d19bc77232daf70d176ee86687d51/ruff-0.0.270-py3-none-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:739495d2dbde87cf4e3110c8d27bc20febf93112539a968a4e02c26f0deccd1d"},
-    {url = "https://files.pythonhosted.org/packages/7f/2c/3989a9296e058720b65106bcb4756781ddada2c258fb2f54be0e702602cf/ruff-0.0.270-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:eca02e709b3308eb7255b5f74e779be23b5980fca3862eae28bb23069cd61ae4"},
-    {url = "https://files.pythonhosted.org/packages/9a/fb/625f83b6e19ef8d78f68cc43afdcb26f0e59ed83c3c569f7cdfa09afd276/ruff-0.0.270-py3-none-musllinux_1_2_armv7l.whl", hash = "sha256:21f00e47ab2308617c44435c8dfd9e2e03897461c9e647ec942deb2a235b4cfd"},
-    {url = "https://files.pythonhosted.org/packages/a6/fc/fd90a58b09ec004f773617a92e0844e30830791e9c6e39582fae414966c2/ruff-0.0.270-py3-none-win_arm64.whl", hash = "sha256:9613456b0b375766244c25045e353bc8890c856431cd97893c97b10cc93bd28d"},
-    {url = "https://files.pythonhosted.org/packages/af/a0/2b773726f2b534acc32ea60b51a3e2f0b130b68a67a32baa099536c153a4/ruff-0.0.270-py3-none-win32.whl", hash = "sha256:b4c037fe2f75bcd9aed0c89c7c507cb7fa59abae2bd4c8b6fc331a28178655a4"},
-    {url = "https://files.pythonhosted.org/packages/b0/6f/d875381e8ca1070b6065aad1095b5b7dff0a2b2198962f72166efd6bbf24/ruff-0.0.270.tar.gz", hash = "sha256:95db07b7850b30ebf32b27fe98bc39e0ab99db3985edbbf0754d399eb2f0e690"},
-    {url = "https://files.pythonhosted.org/packages/b2/4d/c74c7223aa96e2168aa55042a9123a41daddb585e1d492b10de45bcf4db9/ruff-0.0.270-py3-none-musllinux_1_2_aarch64.whl", hash = "sha256:b775e2c5fc869359daf8c8b8aa0fd67240201ab2e8d536d14a0edf279af18786"},
-    {url = "https://files.pythonhosted.org/packages/c0/90/cdbb101b1864aba6a785ef5a91c426abd4d76a3863054496c7c32a20ace8/ruff-0.0.270-py3-none-macosx_10_7_x86_64.whl", hash = "sha256:f74c4d550f7b8e808455ac77bbce38daafc458434815ba0bc21ae4bdb276509b"},
-    {url = "https://files.pythonhosted.org/packages/cb/1e/c6aa0c7e443bae068fe151c592d07078dbb75efcc4c8d73fbf8a7f872e85/ruff-0.0.270-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:0eb412f20e77529a01fb94d578b19dcb8331b56f93632aa0cce4a2ea27b7aeba"},
-    {url = "https://files.pythonhosted.org/packages/dc/59/4f1e078ddf622e42096a45e3e3e3dd524499557044847261e40817f56d2e/ruff-0.0.270-py3-none-musllinux_1_2_x86_64.whl", hash = "sha256:8af391ef81f7be960be10886a3c1aac0b298bde7cb9a86ec2b05faeb2081ce6b"},
-    {url = "https://files.pythonhosted.org/packages/f0/48/a56cdeec0277aff92d68c39c282c9f7c01f38db37c5832605ee8c1ed8097/ruff-0.0.270-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:3ed3b198768d2b3a2300fb18f730cd39948a5cc36ba29ae9d4639a11040880be"},
+"ruff 0.0.271" = [
+    {url = "https://files.pythonhosted.org/packages/00/6a/eb0f14b8942522797b3bcaa468528ab9492b7d200a76af222d76dd3a89ea/ruff-0.0.271-py3-none-win32.whl", hash = "sha256:403e8f9de18b2279d65015a45e0e0d98d60ad878d52f46904f502a4d09465815"},
+    {url = "https://files.pythonhosted.org/packages/05/3a/4cf1193c3fef061cf719e6e60291796ed189f251843e0b2c88479da8e596/ruff-0.0.271-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:9e5de841e09ea75a26956a2cda930d1260c9d8d94cbe57c13b3e881d96526860"},
+    {url = "https://files.pythonhosted.org/packages/09/42/4a175bfb99a1db67bd0ce2e9f18afa0b82f804b9dbc572a099931d4f86ae/ruff-0.0.271-py3-none-musllinux_1_2_x86_64.whl", hash = "sha256:cd43c1aff3eefb2193a125a12124438f65a8d1a6da0e86f8545141d48f6a39fa"},
+    {url = "https://files.pythonhosted.org/packages/0e/55/e6c1af8dc0ac3ea8e078ab7323567ff58ce02c8205b87716e156e5f48f9b/ruff-0.0.271-py3-none-musllinux_1_2_armv7l.whl", hash = "sha256:f3fd9e7c7afb7740d2734af3348e6c88226b42acba2e10a3d1e449caa67e4652"},
+    {url = "https://files.pythonhosted.org/packages/48/9a/99858a13725552d2364ba8ae7f89b35a7b974e4ad8eba7bf9965469dbe39/ruff-0.0.271-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:5a73ffda5548ea8e28e0afcfa698a8675bb17f7048299327f4c1a1287b6e36a2"},
+    {url = "https://files.pythonhosted.org/packages/5c/99/11d8d05cd4186fd6e852d46f47a27de5c6da9f0c2045e6eeb24db136bad5/ruff-0.0.271-py3-none-musllinux_1_2_i686.whl", hash = "sha256:efdfe7fea656eb2ed54f123135c04f71744ad6e4c0c6be156d46e7a2f4730d48"},
+    {url = "https://files.pythonhosted.org/packages/86/35/8a339e8740a7988bdab0adcb016ff0b4a390ee9e7801e2fa071e944e4885/ruff-0.0.271-py3-none-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:f445c56cdc8c12fc28a0b16588ba33abebb6340cb5b1b5a7d5668d4c0b31ad33"},
+    {url = "https://files.pythonhosted.org/packages/86/54/39c28366ee871c955a9beeb092aed3b632a466b8811865aaa78aa7d94cd3/ruff-0.0.271-py3-none-win_amd64.whl", hash = "sha256:140e912a18a662062b04b489861e5aebdbe1a1668bf416e5a951f2347aa65907"},
+    {url = "https://files.pythonhosted.org/packages/9b/50/cd5fec53ae4670b9d409a3f9e99c85016980fb594fb5e1ab354f3171853c/ruff-0.0.271-py3-none-macosx_10_7_x86_64.whl", hash = "sha256:1a627978df924635f7d1a169a98abb2ea488c2d409da56a3f9e44a82d30606ac"},
+    {url = "https://files.pythonhosted.org/packages/a0/e8/1f5116a0b4d6349b8682497287a22ea7b3c13c01b82aab407f213f8289fa/ruff-0.0.271-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:191cdddfc82165afd63ab29ad671419a90a5e699b026ac2d9c61232543965de6"},
+    {url = "https://files.pythonhosted.org/packages/a6/c0/359fa555e0a5ce87e66319c4b6f4035bba75626d39ae133deeff86ca5769/ruff-0.0.271-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:fca503741f4b23a7179fd7a9bc50fc2cca637e9a4da027776f38690c50ae559f"},
+    {url = "https://files.pythonhosted.org/packages/ae/e5/8d3c2a3a507ecb6b161a7838da601d623bb25f2b366f0aadd2f2ddeabfc4/ruff-0.0.271-py3-none-win_arm64.whl", hash = "sha256:45b3c3551a798d9786779c6dd7ad2224af6e06162e17f4a0e7678d3e9115ae56"},
+    {url = "https://files.pythonhosted.org/packages/b2/95/99f3884f93dbc909662362253b84d29923e379f5ad6032f7720ea69c12b0/ruff-0.0.271-py3-none-macosx_10_9_x86_64.macosx_11_0_arm64.macosx_10_9_universal2.whl", hash = "sha256:f47d8a192f6869e95896dc5bb7e825a4f9c554136b9c3bddd38389e43d4db08b"},
+    {url = "https://files.pythonhosted.org/packages/b9/6c/5353a2267cc1a4b72fba83ea4093a57a10a1bcf058f0fbf2557f5c6fff65/ruff-0.0.271-py3-none-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:7e34ca86329a542ab5d31f4fc2702f556d62748f4217e2f6951aef93176190f0"},
+    {url = "https://files.pythonhosted.org/packages/eb/d0/bc63f1baa7e6d7698a857591fe215cc3bac174b309de15bdd2e1b3fe0bd4/ruff-0.0.271-py3-none-manylinux_2_17_ppc64.manylinux2014_ppc64.whl", hash = "sha256:7543b8a32e000ed30727ca6e570a90ab26f8899ee23dffb28806dfc2618782fb"},
+    {url = "https://files.pythonhosted.org/packages/f9/39/2888b3baad15b7930c084da2a2c6f3cac669c4add9b98ac2f74c8378d64a/ruff-0.0.271.tar.gz", hash = "sha256:be4590137a31c47e7f6ef4488d60102c68102f842453355d8073193a30199aa7"},
+    {url = "https://files.pythonhosted.org/packages/fb/de/7647175d1889f29ffbfa7dcbc8a0ed3e007ecc955a01a158d562a6ad37ec/ruff-0.0.271-py3-none-musllinux_1_2_aarch64.whl", hash = "sha256:67525aa821ff0f8371eaa28c73dc467b8eea18931a8bd749775ad538fe1f35e6"},
 ]
 "scalene 1.5.19" = [
     {url = "https://files.pythonhosted.org/packages/11/19/c973ecc43b18076df6c7efff7bec280d02d48d8245f46d94b7e90cf306f2/scalene-1.5.19-cp39-cp39-win_amd64.whl", hash = "sha256:d1fd5d83f3c022ddc46049f29823351b8dbdb8590f5803358fa6034784601f24"},
     {url = "https://files.pythonhosted.org/packages/19/54/d89426ab970f1cb3850b0374967ae22d831d0091efeb2c1d8e8d02ac2a19/scalene-1.5.19-cp39-cp39-macosx_11_7_universal2.whl", hash = "sha256:6c08f3bc0b6355db3c34f0e9aea1b291e64675bb832e19758ee751918787cac0"},
     {url = "https://files.pythonhosted.org/packages/49/11/5a2fa4567eee217609e0a627534f5fb60d0c1f768b43a93145a2ea24e39b/scalene-1.5.19-cp38-cp38-manylinux_2_24_x86_64.whl", hash = "sha256:f67f39321548c06de440319bdd70c41c14b6c50d4748226a101402995677cade"},
     {url = "https://files.pythonhosted.org/packages/5e/3c/b1f159a11f0949f3f27b18af1cc68ee301088a7337efc7d961684bdd3f46/scalene-1.5.19-cp37-cp37m-macosx_10_15_universal2.whl", hash = "sha256:58fb40d031081a55e813f292b2d85b64d7558a372832d8e456f7fe2113adf182"},
     {url = "https://files.pythonhosted.org/packages/65/c3/ebaf00eef807b8da6c5b0c4eb6627f0a67538a25ac7e3858347e15c55d22/scalene-1.5.19-cp38-cp38-win_amd64.whl", hash = "sha256:7a1d452ad4d32cf8adb8b86cae4e5b9c7bff866fff1c43618f9ad114b9ecac32"},
```

### Comparing `xklb-1.30.2/readme.py` & `xklb-1.30.3/readme.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/.github/ISSUE_TEMPLATE/bug_report.md` & `xklb-1.30.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/.github/ISSUE_TEMPLATE/feature_request.md` & `xklb-1.30.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/.github/workflows/push.yaml` & `xklb-1.30.3/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/sql/transfer.sql` & `xklb-1.30.3/sql/transfer.sql`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/xklb/av.py` & `xklb-1.30.3/xklb/av.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/xklb/books.py` & `xklb-1.30.3/xklb/books.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/xklb/consts.py` & `xklb-1.30.3/xklb/consts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import os, re, secrets, string, sys
+import os, re, secrets, shutil, string, sys
 from datetime import datetime, timezone
 from pathlib import Path
 from tempfile import gettempdir
 from types import SimpleNamespace
 from typing import List
 
 
@@ -48,19 +48,15 @@
             r".*reddit\.com/user/(.*?)/.*",
             r".*redd\.it/user/(.*?)/.*",
         ],
     ),
 )
 REGEX_V_REDD_IT = re.compile("https?://v.redd.it/(?:[^/?#&]+)")
 APPLICATION_START = now()
-
-try:
-    TERMINAL_SIZE = os.get_terminal_size()
-except Exception:
-    TERMINAL_SIZE = SimpleNamespace(columns=80, lines=60)
+TERMINAL_SIZE = shutil.get_terminal_size(fallback=(80, 60))
 
 
 TIME_COLUMNS = (
     "time_scanned",
     "time_downloaded",
     "time_deleted",
     "time_modified",
```

### Comparing `xklb-1.30.2/xklb/db.py` & `xklb-1.30.3/xklb/db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/xklb/dl_config.py` & `xklb-1.30.3/xklb/dl_config.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/xklb/dl_extract.py` & `xklb-1.30.3/xklb/dl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/xklb/fs_extract.py` & `xklb-1.30.3/xklb/fs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/xklb/gui.py` & `xklb-1.30.3/xklb/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/xklb/hn_extract.py` & `xklb-1.30.3/xklb/hn_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/xklb/lb.py` & `xklb-1.30.3/xklb/lb.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/xklb/play_actions.py` & `xklb-1.30.3/xklb/play_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/xklb/playback.py` & `xklb-1.30.3/xklb/playback.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/xklb/player.py` & `xklb-1.30.3/xklb/player.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/xklb/praw_extract.py` & `xklb-1.30.3/xklb/praw_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/xklb/search.py` & `xklb-1.30.3/xklb/search.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/xklb/subtitle.py` & `xklb-1.30.3/xklb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/xklb/tabs_actions.py` & `xklb-1.30.3/xklb/tabs_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/xklb/tabs_extract.py` & `xklb-1.30.3/xklb/tabs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/xklb/tube_backend.py` & `xklb-1.30.3/xklb/tube_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -289,14 +289,16 @@
 
     with yt_dlp.YoutubeDL(ydl_opts) as ydl:
         ydl.add_post_processor(AddToArchivePP(), when="pre_process")
 
         count_before_extract = added_media_count
         try:
             pl = ydl.extract_info(playlist_path, download=False, process=True)
+        except yt_dlp.DownloadError:
+            log.error("[%s] DownloadError skipping", playlist_path)
         except ExistingPlaylistVideoReached:
             if added_media_count > count_before_extract:
                 sys.stdout.write("\n")
             log_problem(args, playlist_path)
         else:
             if added_media_count > count_before_extract:
                 sys.stdout.write("\n")
```

### Comparing `xklb-1.30.2/xklb/tube_extract.py` & `xklb-1.30.3/xklb/tube_extract.py`

 * *Files 7% similar despite different names*

```diff
@@ -51,22 +51,23 @@
 
     if args.db:
         args.database = args.db
     if action == SC.tubeadd:
         Path(args.database).touch()
     args.db = db.connect(args)
 
-    if hasattr(args, "no_sanitize") and hasattr(args, "playlists") and not args.no_sanitize:
-        args.playlists = [utils.sanitize_url(args, p) for p in args.playlists]
     if hasattr(args, "playlists"):
+        args.playlists = list(set(args.playlists))
+        if not args.no_sanitize:
+            args.playlists = [utils.sanitize_url(args, p) for p in args.playlists]
         args.playlists = utils.conform(args.playlists)
-    log.info(utils.dict_filter_bool(args.__dict__))
 
     utils.timeout(args.timeout)
 
+    log.info(utils.dict_filter_bool(args.__dict__))
     return args
 
 
 def tube_add(args=None) -> None:
     if args:
         sys.argv = ["tubeadd", *args]
 
@@ -93,19 +94,37 @@
                     """,
                     )
                 ]
                 for table in args.playlists
             ),
         )
 
+    tables = args.db.table_names()
+
     for path in args.playlists:
         if args.safe and not tube_backend.is_supported(path):
             log.info("[%s]: Skipping unsupported playlist (safe_mode)", path)
             continue
 
+        if "media" in tables and not args.playlist_db:
+            m_columns = args.db["media"].columns_dict
+            playlist_already_added = list(
+                args.db.query(
+                    f"""
+                    SELECT path from media
+                    WHERE 1=1
+                    AND (path=? or {'web' if 'webpath' in m_columns else ''}path=?)
+                    """,
+                    [path, path],
+                ),
+            )
+            if playlist_already_added:
+                log.info("[%s]: Already added. Skipping!", path)
+                continue
+
         tube_backend.process_playlist(args, path, tube_backend.tube_opts(args))
 
         if args.extra:
             log.warning("[%s]: Getting extra metadata", path)
             tube_backend.get_extra_metadata(args, path)
 
     LARGE_NUMBER = 100_000
```

### Comparing `xklb-1.30.2/xklb/usage.py` & `xklb-1.30.3/xklb/usage.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/xklb/utils.py` & `xklb-1.30.3/xklb/utils.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/xklb/scripts/bigdirs.py` & `xklb-1.30.3/xklb/scripts/bigdirs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/xklb/scripts/block.py` & `xklb-1.30.3/xklb/scripts/block.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/xklb/scripts/christen.py` & `xklb-1.30.3/xklb/scripts/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/xklb/scripts/cluster_sort.py` & `xklb-1.30.3/xklb/scripts/cluster_sort.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/xklb/scripts/copy_play_counts.py` & `xklb-1.30.3/xklb/scripts/copy_play_counts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/xklb/scripts/dedupe.py` & `xklb-1.30.3/xklb/scripts/dedupe.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/xklb/scripts/download_status.py` & `xklb-1.30.3/xklb/scripts/download_status.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/xklb/scripts/history.py` & `xklb-1.30.3/xklb/scripts/history.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/xklb/scripts/merge_dbs.py` & `xklb-1.30.3/xklb/scripts/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/xklb/scripts/merge_online_local.py` & `xklb-1.30.3/xklb/scripts/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/xklb/scripts/move_list.py` & `xklb-1.30.3/xklb/scripts/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/xklb/scripts/optimize_db.py` & `xklb-1.30.3/xklb/scripts/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/xklb/scripts/playlists.py` & `xklb-1.30.3/xklb/scripts/playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/xklb/scripts/redownload.py` & `xklb-1.30.3/xklb/scripts/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/xklb/scripts/relmv.py` & `xklb-1.30.3/xklb/scripts/relmv.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/xklb/scripts/scatter.py` & `xklb-1.30.3/xklb/scripts/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/xklb/scripts/streaming_tab_loader.py` & `xklb-1.30.3/xklb/scripts/streaming_tab_loader.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/xklb/scripts/mining/data.py` & `xklb-1.30.3/xklb/scripts/mining/data.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/xklb/scripts/mining/extract_links.py` & `xklb-1.30.3/xklb/scripts/mining/extract_links.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/xklb/scripts/mining/nouns.py` & `xklb-1.30.3/xklb/scripts/mining/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/xklb/scripts/mining/pushshift.py` & `xklb-1.30.3/xklb/scripts/mining/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/xklb/scripts/mining/reddit_selftext.py` & `xklb-1.30.3/xklb/scripts/mining/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/xklb/assets/kotobago.png` & `xklb-1.30.3/xklb/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/.gitignore` & `xklb-1.30.3/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/LICENSE` & `xklb-1.30.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/README.md` & `xklb-1.30.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 Incremental surfing. 📈🏄 totally rad!
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.30.002)
+    xk media library subcommands (v1.30.003)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

### Comparing `xklb-1.30.2/pyproject.toml` & `xklb-1.30.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xklb-1.30.2/PKG-INFO` & `xklb-1.30.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xklb
-Version: 1.30.2
+Version: 1.30.3
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
-    xk media library subcommands (v1.30.002)
+    xk media library subcommands (v1.30.003)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

