# Comparing `tmp/xklb-1.30.3.tar.gz` & `tmp/xklb-1.30.5.tar.gz`

## Comparing `xklb-1.30.3.tar` & `xklb-1.30.5.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.30.3/.gitattributes
--rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 xklb-1.30.3/TODO
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.30.3/Windows.md
--rw-r--r--   0        0        0   489912 2020-02-02 00:00:00.000000 xklb-1.30.3/pdm.lock
--rw-r--r--   0        0        0    19066 2020-02-02 00:00:00.000000 xklb-1.30.3/readme.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.30.3/.github/FUNDING.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.30.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.30.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 xklb-1.30.3/.github/workflows/push.yaml
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xklb-1.30.3/sql/transfer.sql
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/__init__.py
--rw-r--r--   0        0        0     8237 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/av.py
--rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/books.py
--rw-r--r--   0        0        0     7790 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/consts.py
--rw-r--r--   0        0        0     8737 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/db.py
--rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/dl_config.py
--rw-r--r--   0        0        0     9808 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/dl_extract.py
--rw-r--r--   0        0        0    14237 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/fs_extract.py
--rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/gui.py
--rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/hn_extract.py
--rw-r--r--   0        0        0    11152 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/lb.py
--rw-r--r--   0        0        0    25158 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/play_actions.py
--rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/playback.py
--rw-r--r--   0        0        0    35093 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/player.py
--rw-r--r--   0        0        0    13992 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/praw_extract.py
--rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/search.py
--rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/subtitle.py
--rw-r--r--   0        0        0     6029 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/tabs_actions.py
--rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/tabs_extract.py
--rw-r--r--   0        0        0    22847 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/tube_backend.py
--rw-r--r--   0        0        0     5463 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/tube_extract.py
--rw-r--r--   0        0        0    77169 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/usage.py
--rw-r--r--   0        0        0    37021 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     5389 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/scripts/bigdirs.py
--rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/scripts/block.py
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/scripts/christen.py
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/scripts/cluster_sort.py
--rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/scripts/copy_play_counts.py
--rw-r--r--   0        0        0     8150 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/scripts/dedupe.py
--rw-r--r--   0        0        0     5090 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/scripts/download_status.py
--rw-r--r--   0        0        0     4930 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/scripts/history.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/scripts/move_list.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     5957 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/scripts/playlists.py
--rw-r--r--   0        0        0     5986 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/scripts/relmv.py
--rw-r--r--   0        0        0     8696 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/scripts/mining/data.py
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/scripts/mining/extract_links.py
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/scripts/mining/reddit_selftext.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.30.3/xklb/assets/kotobago.png
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.30.3/.gitignore
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.30.3/LICENSE
--rw-r--r--   0        0        0    99455 2020-02-02 00:00:00.000000 xklb-1.30.3/README.md
--rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 xklb-1.30.3/pyproject.toml
--rw-r--r--   0        0        0   103051 2020-02-02 00:00:00.000000 xklb-1.30.3/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.30.5/.gitattributes
+-rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 xklb-1.30.5/TODO
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.30.5/Windows.md
+-rw-r--r--   0        0        0   490403 2020-02-02 00:00:00.000000 xklb-1.30.5/pdm.lock
+-rw-r--r--   0        0        0    19130 2020-02-02 00:00:00.000000 xklb-1.30.5/readme.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.30.5/.github/FUNDING.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.30.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.30.5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 xklb-1.30.5/.github/workflows/push.yaml
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xklb-1.30.5/sql/transfer.sql
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/__init__.py
+-rw-r--r--   0        0        0     8237 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/av.py
+-rw-r--r--   0        0        0     6921 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/books.py
+-rw-r--r--   0        0        0     7790 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/consts.py
+-rw-r--r--   0        0        0     8737 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/db.py
+-rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/dl_config.py
+-rw-r--r--   0        0        0     9808 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/dl_extract.py
+-rw-r--r--   0        0        0    14237 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/fs_extract.py
+-rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/gui.py
+-rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/hn_extract.py
+-rw-r--r--   0        0        0    11152 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/lb.py
+-rw-r--r--   0        0        0    25158 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/play_actions.py
+-rw-r--r--   0        0        0     4564 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/playback.py
+-rw-r--r--   0        0        0    35093 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/player.py
+-rw-r--r--   0        0        0    13992 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/praw_extract.py
+-rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/search.py
+-rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/subtitle.py
+-rw-r--r--   0        0        0     6029 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    22847 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/tube_backend.py
+-rw-r--r--   0        0        0     4877 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/tube_extract.py
+-rw-r--r--   0        0        0    77219 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/usage.py
+-rw-r--r--   0        0        0    37021 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     5389 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/scripts/bigdirs.py
+-rw-r--r--   0        0        0     7253 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/scripts/block.py
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/scripts/christen.py
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/scripts/cluster_sort.py
+-rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/scripts/copy_play_counts.py
+-rw-r--r--   0        0        0     8150 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/scripts/dedupe.py
+-rw-r--r--   0        0        0     5090 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/scripts/download_status.py
+-rw-r--r--   0        0        0     4930 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/scripts/history.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     5957 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/scripts/playlists.py
+-rw-r--r--   0        0        0     5986 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/scripts/relmv.py
+-rw-r--r--   0        0        0     8696 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/scripts/mining/data.py
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/scripts/mining/extract_links.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/scripts/mining/reddit_selftext.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.30.5/xklb/assets/kotobago.png
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.30.5/.gitignore
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.30.5/LICENSE
+-rw-r--r--   0        0        0    99569 2020-02-02 00:00:00.000000 xklb-1.30.5/README.md
+-rw-r--r--   0        0        0     2635 2020-02-02 00:00:00.000000 xklb-1.30.5/pyproject.toml
+-rw-r--r--   0        0        0   103165 2020-02-02 00:00:00.000000 xklb-1.30.5/PKG-INFO
```

### Comparing `xklb-1.30.3/TODO` & `xklb-1.30.5/TODO`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/Windows.md` & `xklb-1.30.5/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/pdm.lock` & `xklb-1.30.5/pdm.lock`

 * *Files 0% similar despite different names*

```diff
@@ -769,25 +769,25 @@
 name = "pynvml"
 version = "11.5.0"
 requires_python = ">=3.6"
 summary = "Python Bindings for the NVIDIA Management Library"
 
 [[package]]
 name = "pyobjc-core"
-version = "9.1.1"
+version = "9.2"
 requires_python = ">=3.7"
 summary = "Python<->ObjC Interoperability Module"
 
 [[package]]
 name = "pyobjc-framework-cocoa"
-version = "9.1.1"
+version = "9.2"
 requires_python = ">=3.7"
 summary = "Wrappers for the Cocoa frameworks on macOS"
 dependencies = [
-    "pyobjc-core>=9.1.1",
+    "pyobjc-core>=9.2",
 ]
 
 [[package]]
 name = "pysrt"
 version = "1.1.2"
 summary = "SubRip (.srt) subtitle parser and writer"
 dependencies = [
@@ -1180,15 +1180,15 @@
 name = "urllib3"
 version = "1.25.11"
 requires_python = ">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, <4"
 summary = "HTTP library with thread-safe connection pooling, file post, and more."
 
 [[package]]
 name = "wasabi"
-version = "1.1.1"
+version = "1.1.2"
 requires_python = ">=3.6"
 summary = "A lightweight console printing and formatting toolkit"
 dependencies = [
     "colorama>=0.4.6; sys_platform == \"win32\" and python_version >= \"3.7\"",
 ]
 
 [[package]]
@@ -2748,31 +2748,33 @@
     {url = "https://files.pythonhosted.org/packages/34/a7/37c8d68532ba71549db4212cb036dbd6161b40e463aba336770e80c72f84/Pygments-2.15.1-py3-none-any.whl", hash = "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"},
     {url = "https://files.pythonhosted.org/packages/89/6b/2114e54b290824197006e41be3f9bbe1a26e9c39d1f5fa20a6d62945a0b3/Pygments-2.15.1.tar.gz", hash = "sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c"},
 ]
 "pynvml 11.5.0" = [
     {url = "https://files.pythonhosted.org/packages/5b/9c/adb8070059caaa15d5a572b66bccd95900d8c1b9fa54d6ecea6ae97448d1/pynvml-11.5.0-py3-none-any.whl", hash = "sha256:5cce014ac01b098d08f06178f86c37be409b80b2e903a5a03ce15eed60f55e25"},
     {url = "https://files.pythonhosted.org/packages/77/1b/dbc48e97c0c005a5ac4574dbea98465211e918dd79e6bdbde21ee77cccb9/pynvml-11.5.0.tar.gz", hash = "sha256:d027b21b95b1088b9fc278117f9f61b7c67f8e33a787e9f83f735f0f71ac32d0"},
 ]
-"pyobjc-core 9.1.1" = [
-    {url = "https://files.pythonhosted.org/packages/0b/0b/f13a4ff6bc4ef8eacd4a487e2892041f71fbd7abfbc6791c78a458e314a7/pyobjc_core-9.1.1-cp38-cp38-macosx_11_0_universal2.whl", hash = "sha256:1626909916603a3b04c07c721cf1af0e0b892cec85bb3db98d05ba024f1786fc"},
-    {url = "https://files.pythonhosted.org/packages/10/49/63fca6412f4a0fcd3c73f333165222064f0a84fc9ef4d285cc1a4a009df7/pyobjc_core-9.1.1-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:d61e9517d451bc062a7fae8b3648f4deba4fa54a24926fa1cf581b90ef4ced5a"},
-    {url = "https://files.pythonhosted.org/packages/89/33/78a6350f83d071c502b778762564720dd6ab681a6c6104f7607aa83fe3c2/pyobjc_core-9.1.1-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:083004d28b92ccb483a41195c600728854843b0486566aba2d6e63eef51f80e6"},
-    {url = "https://files.pythonhosted.org/packages/9e/43/da6deaad1611502c4a05e3d4e669c9279c65a801a8317b912725bae72844/pyobjc_core-9.1.1-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:2dde96462b52e952515d142e2afbb6913624a02c13582047e06211e6c3993728"},
-    {url = "https://files.pythonhosted.org/packages/b5/a6/22b65cabf1c05b388a5b48046d51b71b2478b0fc5b12c300375425fbdd2e/pyobjc_core-9.1.1-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:4bd07049fd9fe5b40e4b7c468af9cf942508387faf383a5acb043d20627bad2c"},
-    {url = "https://files.pythonhosted.org/packages/d2/b4/cb2a22c509c8ce435ac0617e3354a1f94411f0023d3c2feb350b007b8da0/pyobjc-core-9.1.1.tar.gz", hash = "sha256:4b6cb9053b5fcd3c0e76b8c8105a8110786b20f3403c5643a688c5ec51c55c6b"},
-    {url = "https://files.pythonhosted.org/packages/df/b0/fc43adf71907d1d9ae8ab0751426f1577e24588854e83e927c76c86b2cfa/pyobjc_core-9.1.1-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:1a8307527621729ff2ab67860e7ed84f76ad0da881b248c2ef31e0da0088e4ba"},
-]
-"pyobjc-framework-cocoa 9.1.1" = [
-    {url = "https://files.pythonhosted.org/packages/1d/79/af7bd8fdc61a1210f679c1cff689b86894473a7e81ab355e2d0cb59dc131/pyobjc_framework_Cocoa-9.1.1-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:5e1e96fb3461f46ff951413515f2029e21be268b0e033db6abee7b64ec8e93d3"},
-    {url = "https://files.pythonhosted.org/packages/4e/d9/fc63476d44b2b1c6acbe6704eda28ddc8beb5aa9c1bb14833f9660e51389/pyobjc_framework_Cocoa-9.1.1-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:083b195c496d30c6b9dd86126a6093c4b95e0138e9b052b13e54103fcc0b4872"},
-    {url = "https://files.pythonhosted.org/packages/61/fd/df2e56a3e5962a0413014859225c663e3071c51a3d1e7837bbaebca9d72a/pyobjc_framework_Cocoa-9.1.1-cp38-cp38-macosx_11_0_universal2.whl", hash = "sha256:54c017354671f0d955432986c42218e452ca69906a101c8e7acde8510432303a"},
-    {url = "https://files.pythonhosted.org/packages/7d/b4/f9d0bde8f0da5857a857ffbbddb96fb549bc68365a0a35f126e7fd72cb5c/pyobjc_framework_Cocoa-9.1.1-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:9176a4276f3b4b4758e9b9ca10698be5341ceffaeaa4fa055133417179e6bc37"},
-    {url = "https://files.pythonhosted.org/packages/90/70/7ec76e482a49cdb4dd5c4371c52775d237fcbf4fc1932bd60889b8006f1a/pyobjc-framework-Cocoa-9.1.1.tar.gz", hash = "sha256:345c32b6d1f3db45f635e400f2d0d6c0f0f7349d45ec823f76fc1df43d13caeb"},
-    {url = "https://files.pythonhosted.org/packages/ab/04/ab93732b4aa8381790a9b7e43e2d73ccdf79a02570070b5c5f8ee433adc1/pyobjc_framework_Cocoa-9.1.1-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:a1b3333b1aa045608848bd68bbab4c31171f36aeeaa2fabeb4527c6f6f1e33cd"},
-    {url = "https://files.pythonhosted.org/packages/f4/f4/5837b90164d987ed14bb726b7deb3670c7d66471ba9f214bf38bdd2e6217/pyobjc_framework_Cocoa-9.1.1-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:10c0075688ce95b92caf59e368585fffdcc98c919bc345067af070222f5d01d2"},
+"pyobjc-core 9.2" = [
+    {url = "https://files.pythonhosted.org/packages/04/8f/e005f4863a7257285d5c98365e2d6e2dd717298d829453fc6eb25ac74a11/pyobjc_core-9.2-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:fa674a39949f5cde8e5c7bbcd24496446bfc67592b028aedbec7f81dc5fc4daa"},
+    {url = "https://files.pythonhosted.org/packages/04/f5/f750f72af0fe30c3e30b92f514701fb724db28b860838bc3b83584af01ff/pyobjc_core-9.2-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:41189c2c680931c0395a55691763c481fc681f454f21bb4f1644f98c24a45954"},
+    {url = "https://files.pythonhosted.org/packages/08/45/b993d9ac2ea48f020ae6f295c61695818eebf3921d0959a000b8fcb2895e/pyobjc_core-9.2-cp312-cp312-macosx_10_9_universal2.whl", hash = "sha256:0fa950f092673883b8bd28bc18397415cabb457bf410920762109b411789ade9"},
+    {url = "https://files.pythonhosted.org/packages/35/5e/6d130b175bb4d4635a0e434e7d05be019841ac11c63e9be7eb3c25029346/pyobjc_core-9.2-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:b9809cf96678797acb72a758f34932fe8e2602d5ab7abec15c5ac68ddb481720"},
+    {url = "https://files.pythonhosted.org/packages/48/d9/a13566ce8914746557b9e8637a5abe1caae86ed202b0fb072029626b8bb1/pyobjc-core-9.2.tar.gz", hash = "sha256:d734b9291fec91ff4e3ae38b9c6839debf02b79c07314476e87da8e90b2c68c3"},
+    {url = "https://files.pythonhosted.org/packages/81/49/766832436ba1f992328d6048145a1aaec11f677f1e53e0de658a2b627562/pyobjc_core-9.2-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:bbc8de304ee322a1ee530b4d2daca135a49b4a49aa3cedc6b2c26c43885f4842"},
+    {url = "https://files.pythonhosted.org/packages/b9/75/7750c084871975ead4fdfc4938315709d48ea7952e8a1a2c6247436e0478/pyobjc_core-9.2-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:586e4cae966282eaa61b21cae66ccdcee9d69c036979def26eebdc08ddebe20f"},
+    {url = "https://files.pythonhosted.org/packages/b9/bd/3d85098a8f2cfd725391abf145c37a638717968efa52bfc0568e155a628e/pyobjc_core-9.2-cp38-cp38-macosx_11_0_universal2.whl", hash = "sha256:2d23ee539f2ba5e9f5653d75a13f575c7e36586fc0086792739e69e4c2617eda"},
+]
+"pyobjc-framework-cocoa 9.2" = [
+    {url = "https://files.pythonhosted.org/packages/04/0a/1bb7500d725593fa035b44c5d16b95c0b80d501db3ce1c2e97f47be23c69/pyobjc_framework_Cocoa-9.2-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:3b1e6287b3149e4c6679cdbccd8e9ef6557a4e492a892e80a77df143f40026d2"},
+    {url = "https://files.pythonhosted.org/packages/15/10/0d46760671b5fce9e494db4dca3a976cb0ea4feba1ad8ef489082a09b253/pyobjc_framework_Cocoa-9.2-cp38-cp38-macosx_11_0_universal2.whl", hash = "sha256:32d9ac1033fac1b821ddee8c68f972a7074ad8c50bec0bea9a719034c1c2fb94"},
+    {url = "https://files.pythonhosted.org/packages/38/91/c54fdffda6d7cfad67ff617f19001163658d50bc72376d1584e691cf4895/pyobjc-framework-Cocoa-9.2.tar.gz", hash = "sha256:efd78080872d8c8de6c2b97e0e4eac99d6203a5d1637aa135d071d464eb2db53"},
+    {url = "https://files.pythonhosted.org/packages/64/09/d0eb252549b3009f008c8415c9739a9c726ddfec9adc1aa92b6a8dec0efe/pyobjc_framework_Cocoa-9.2-cp39-cp39-macosx_10_9_universal2.whl", hash = "sha256:b236bb965e41aeb2e215d4e98a5a230d4b63252c6d26e00924ea2e69540a59d6"},
+    {url = "https://files.pythonhosted.org/packages/9b/e2/49ea296127184f8b578838ba0d3d170abb75c23760d940f952df0fe0e132/pyobjc_framework_Cocoa-9.2-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:739a421e14382a46cbeb9a883f192dceff368ad28ec34d895c48c0ad34cf2c1d"},
+    {url = "https://files.pythonhosted.org/packages/d7/b3/e9c6d3e8d53453567805ca461cf52a08807ca2c860c1364c27dc10cdc67e/pyobjc_framework_Cocoa-9.2-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:9e02d8a7cc4eb7685377c50ba4f17345701acf4c05b1e7480d421bff9e2f62a4"},
+    {url = "https://files.pythonhosted.org/packages/e0/f6/ecbc6323aa12df79acdaf8a75f7bb93d273b6dcd0c5b65658c2505bbc977/pyobjc_framework_Cocoa-9.2-cp312-cp312-macosx_10_9_universal2.whl", hash = "sha256:312977ce2e3989073c6b324c69ba24283de206fe7acd6dbbbaf3e29238a22537"},
+    {url = "https://files.pythonhosted.org/packages/fa/f1/d3d3528d1d62d3e21211bcb8bd6bfe1b8c2815d700eb986fdb1f37de9c7d/pyobjc_framework_Cocoa-9.2-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:aae7841cf40c26dd915f4dd828f91c6616e6b7998630b72e704750c09e00f334"},
 ]
 "pysrt 1.1.2" = [
     {url = "https://files.pythonhosted.org/packages/31/1a/0d858da1c6622dcf16011235a2639b0a01a49cecf812f8ab03308ab4de37/pysrt-1.1.2.tar.gz", hash = "sha256:b4f844ba33e4e7743e9db746492f3a193dc0bc112b153914698e7c1cdeb9b0b9"},
 ]
 "pysubs2 1.6.1" = [
     {url = "https://files.pythonhosted.org/packages/22/3e/fb1b08a06144ba63f19cc4758dd72e2eb8c7fc95c6c8364faccfc570c7bf/pysubs2-1.6.1.tar.gz", hash = "sha256:0261611e71735ff7763972c519c72593c8063efcb9039c54af65f31b81cec116"},
     {url = "https://files.pythonhosted.org/packages/4f/dc/dc1763a3abab92af2253b1abb3dd48e07b2a3613d7ae64a3ab5c27da3019/pysubs2-1.6.1-py3-none-any.whl", hash = "sha256:1f96d9dfb5f859a54a00e04621beb20ff21ea1d788821b2f4935c5c0ef8dc68e"},
@@ -3133,17 +3135,17 @@
     {url = "https://files.pythonhosted.org/packages/0c/ba/8dd7fa5f0b1c6a8ac62f8f57f7e794160c1f86f31c6d0fb00f582372a3e4/update_checker-0.18.0-py3-none-any.whl", hash = "sha256:cbba64760a36fe2640d80d85306e8fe82b6816659190993b7bdabadee4d4bbfd"},
     {url = "https://files.pythonhosted.org/packages/5c/0b/1bec4a6cc60d33ce93d11a7bcf1aeffc7ad0aa114986073411be31395c6f/update_checker-0.18.0.tar.gz", hash = "sha256:6a2d45bb4ac585884a6b03f9eade9161cedd9e8111545141e9aa9058932acb13"},
 ]
 "urllib3 1.25.11" = [
     {url = "https://files.pythonhosted.org/packages/56/aa/4ef5aa67a9a62505db124a5cb5262332d1d4153462eb8fd89c9fa41e5d92/urllib3-1.25.11-py2.py3-none-any.whl", hash = "sha256:f5321fbe4bf3fefa0efd0bfe7fb14e90909eb62a48ccda331726b4319897dd5e"},
     {url = "https://files.pythonhosted.org/packages/76/d9/bbbafc76b18da706451fa91bc2ebe21c0daf8868ef3c30b869ac7cb7f01d/urllib3-1.25.11.tar.gz", hash = "sha256:8d7eaa5a82a1cac232164990f04874c594c9453ec55eef02eab885aa02fc17a2"},
 ]
-"wasabi 1.1.1" = [
-    {url = "https://files.pythonhosted.org/packages/58/5f/1f2833d59abf53e24dbadc21b0565fe10c64545da8705faed8eff3b14745/wasabi-1.1.1-py3-none-any.whl", hash = "sha256:32e44649d99a64e08e40c1c96cddb69fad460bd0cc33802a53cab6714dfb73f8"},
-    {url = "https://files.pythonhosted.org/packages/8d/d3/abe7d7d745657e43af711bdc58d4c9016f63546795ec9b5b62b2d9b89fa6/wasabi-1.1.1.tar.gz", hash = "sha256:f5ee7c609027811bd16e620f2fd7a7319466005848e41b051a62053ab8fd70d6"},
+"wasabi 1.1.2" = [
+    {url = "https://files.pythonhosted.org/packages/3e/09/bbd7e880b56e825d5859a58adb1bd1feb45b604218706057ca1e3278fa62/wasabi-1.1.2.tar.gz", hash = "sha256:1aaef3aceaa32edb9c91330d29d3936c0c39fdb965743549c173cb54b16c30b5"},
+    {url = "https://files.pythonhosted.org/packages/8f/69/26cbf0bad11703241cb84d5324d868097f7a8faf2f1888354dac8883f3fc/wasabi-1.1.2-py3-none-any.whl", hash = "sha256:0a3f933c4bf0ed3f93071132c1b87549733256d6c8de6473c5f7ed2e171b5cf9"},
 ]
 "wcwidth 0.2.6" = [
     {url = "https://files.pythonhosted.org/packages/20/f4/c0584a25144ce20bfcf1aecd041768b8c762c1eb0aa77502a3f0baa83f11/wcwidth-0.2.6-py2.py3-none-any.whl", hash = "sha256:795b138f6875577cd91bba52baf9e445cd5118fd32723b460e30a0af30ea230e"},
     {url = "https://files.pythonhosted.org/packages/5e/5f/1e4bd82a9cc1f17b2c2361a2d876d4c38973a997003ba5eb400e8a932b6c/wcwidth-0.2.6.tar.gz", hash = "sha256:a5220780a404dbe3353789870978e472cfe477761f06ee55077256e509b156d0"},
 ]
 "websocket-client 1.5.2" = [
     {url = "https://files.pythonhosted.org/packages/3f/f2/2624e12ef854ee667d92ac5dc7815932095e0852e5ff2b2bf57feda8a11b/websocket-client-1.5.2.tar.gz", hash = "sha256:c7d67c13b928645f259d9b847ab5b57fd2d127213ca41ebd880de1f553b7c23b"},
```

### Comparing `xklb-1.30.3/readme.py` & `xklb-1.30.5/readme.py`

 * *Files 1% similar despite different names*

```diff
@@ -429,15 +429,15 @@
         end
     end | parallel -j8
 
     for subreddit in $subreddits
         sqlite-utils upsert --pk path --alter --csv --detect-types $reddit_db media $subreddit.csv
     end
 
-    library tubeadd --safe -i $reddit_db --playlist-db media
+    library tubeadd --safe --ignore-errors --force $reddit_db (sqlite-utils --raw-lines $reddit_db 'select path from media')
 end
 ```
 
 </details>
 
 ### Datasette
```

### Comparing `xklb-1.30.3/.github/ISSUE_TEMPLATE/bug_report.md` & `xklb-1.30.5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/.github/ISSUE_TEMPLATE/feature_request.md` & `xklb-1.30.5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/.github/workflows/push.yaml` & `xklb-1.30.5/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/sql/transfer.sql` & `xklb-1.30.5/sql/transfer.sql`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/xklb/av.py` & `xklb-1.30.5/xklb/av.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/xklb/books.py` & `xklb-1.30.5/xklb/books.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/xklb/consts.py` & `xklb-1.30.5/xklb/consts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/xklb/db.py` & `xklb-1.30.5/xklb/db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/xklb/dl_config.py` & `xklb-1.30.5/xklb/dl_config.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/xklb/dl_extract.py` & `xklb-1.30.5/xklb/dl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/xklb/fs_extract.py` & `xklb-1.30.5/xklb/fs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/xklb/gui.py` & `xklb-1.30.5/xklb/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/xklb/hn_extract.py` & `xklb-1.30.5/xklb/hn_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/xklb/lb.py` & `xklb-1.30.5/xklb/lb.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/xklb/play_actions.py` & `xklb-1.30.5/xklb/play_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/xklb/playback.py` & `xklb-1.30.5/xklb/playback.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/xklb/player.py` & `xklb-1.30.5/xklb/player.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/xklb/praw_extract.py` & `xklb-1.30.5/xklb/praw_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/xklb/search.py` & `xklb-1.30.5/xklb/search.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/xklb/subtitle.py` & `xklb-1.30.5/xklb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/xklb/tabs_actions.py` & `xklb-1.30.5/xklb/tabs_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/xklb/tabs_extract.py` & `xklb-1.30.5/xklb/tabs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/xklb/tube_backend.py` & `xklb-1.30.5/xklb/tube_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/xklb/tube_extract.py` & `xklb-1.30.5/xklb/scripts/bigdirs.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,141 +1,173 @@
-import argparse, sys
+import argparse
 from pathlib import Path
+from typing import Dict, List
 
-from xklb import db, tube_backend, usage, utils
-from xklb.consts import SC
+from tabulate import tabulate
+
+from xklb import db, usage, utils
 from xklb.utils import log
 
 
-def parse_args(action, usage) -> argparse.Namespace:
+def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
-        prog="library " + action,
-        usage=usage,
+        prog="library bigdirs",
+        usage=usage.bigdirs,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
-
+    parser.add_argument("--sort-by")
+    parser.add_argument("--limit", "-L", "-l", "-queue", "--queue", default="4000")
+    parser.add_argument("--depth", "-d", default=0, type=int, help="Depth of folders")
+    parser.add_argument("--lower", type=int, help="Number of files per folder lower limit")
+    parser.add_argument("--upper", type=int, help="Number of files per folder upper limit")
     parser.add_argument(
-        "--dl-config",
-        "-dl-config",
-        nargs=1,
-        action=utils.ArgparseDict,
-        default={},
-        metavar="KEY=VALUE",
-        help="Add key/value pairs to override or extend default downloader configuration",
+        "--size",
+        "-S",
+        action="append",
+        help="Only include files of specific sizes (uses the same syntax as fd-find)",
     )
-    parser.add_argument("--download-archive", default="~/.local/share/yt_archive.txt")
-    parser.add_argument("--safe", "-safe", action="store_true", help="Skip generic URLs")
-    parser.add_argument("--no-sanitize", "-s", action="store_true", help="Don't sanitize some common URL parameters")
-    parser.add_argument("--extra", "-extra", action="store_true", help="Get full metadata (takes a lot longer)")
-    parser.add_argument("--playlist-files", action="store_true", help="Read playlists from text files")
-    parser.add_argument("--playlist-db", action="store_true", help="Fetch metadata for paths in a table")
-    parser.add_argument("--subs", action="store_true")
-    parser.add_argument("--auto-subs", "--autosubs", action="store_true")
-    parser.add_argument("--subtitle-languages", "--subtitle-language", "--sl", action=utils.ArgparseList)
-    parser.add_argument("--extra-media-data", default={})
-    parser.add_argument("--extra-playlist-data", default={})
-    parser.add_argument("--ignore-errors", "--ignoreerrors", "-i", "-f", action="store_true", help=argparse.SUPPRESS)
-
-    if action in (SC.tubeadd, SC.tubeupdate):
-        parser.add_argument("--category", "-c", help=argparse.SUPPRESS)
-
-    parser.add_argument("--timeout", "-T", help="Quit after x minutes")
+    parser.add_argument("--include", "-s", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
+    parser.add_argument("--exclude", "-E", "-e", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
     parser.add_argument("--verbose", "-v", action="count", default=0)
-    parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
 
     parser.add_argument("database")
-    if action == SC.tubeadd:
-        parser.add_argument("playlists", nargs="+", help=argparse.SUPPRESS)
-
-    args = parser.parse_args()
-    args.action = action
-
-    if args.db:
-        args.database = args.db
-    if action == SC.tubeadd:
-        Path(args.database).touch()
+    parser.add_argument("search", nargs="*")
+    args = parser.parse_intermixed_args()
     args.db = db.connect(args)
 
-    if hasattr(args, "playlists"):
-        args.playlists = list(set(args.playlists))
-        if not args.no_sanitize:
-            args.playlists = [utils.sanitize_url(args, p) for p in args.playlists]
-        args.playlists = utils.conform(args.playlists)
+    args.include += args.search
+    if args.include == ["."]:
+        args.include = [str(Path().cwd().resolve())]
 
-    utils.timeout(args.timeout)
+    if args.size:
+        args.size = utils.parse_human_to_sql(utils.human_to_bytes, "size", args.size)
 
     log.info(utils.dict_filter_bool(args.__dict__))
     return args
 
 
-def tube_add(args=None) -> None:
-    if args:
-        sys.argv = ["tubeadd", *args]
-
-    args = parse_args(SC.tubeadd, usage=usage.tubeadd)
-    if args.playlist_files:
-        args.playlists = list(utils.flatten([Path(p).read_text().splitlines() for p in args.playlists]))
-    elif args.playlist_db:
-        args.playlists = list(
-            utils.flatten(
-                [
-                    d["path"]
-                    for d in args.db.query(
-                        f"""
-                    select path from {table}
-                    where 1=1
-                    and COALESCE(time_deleted,0) = 0
-                    and COALESCE(time_modified,0) = 0
-                    and COALESCE(time_downloaded,0) = 0
-                    {'and width is null' if 'width' in args.db[table].columns_dict else ''}
-                    {'and title is null' if 'title' in args.db[table].columns_dict else ''}
-                    {'and duration is null' if 'duration' in args.db[table].columns_dict else ''}
-                    {'and size is null' if 'size' in args.db[table].columns_dict else ''}
-                    ORDER by random()
-                    """,
-                    )
-                ]
-                for table in args.playlists
-            ),
-        )
-
-    tables = args.db.table_names()
-
-    for path in args.playlists:
-        if args.safe and not tube_backend.is_supported(path):
-            log.info("[%s]: Skipping unsupported playlist (safe_mode)", path)
+def group_files_by_folder(args, media) -> List[Dict]:
+    d = {}
+    for m in media:
+        p = m["path"].split("/")
+        while len(p) >= 2:
+            p.pop()
+            parent = "/".join(p) + "/"
+
+            file_deleted = bool(m.get("time_deleted", 0))
+            file_played = bool(m.get("time_played", 0))
+            if parent not in d:
+                d[parent] = {"size": 0, "count": 0, "deleted": 0, "played": 0}
+            if not file_deleted:
+                d[parent]["size"] += m.get("size", 0)
+                d[parent]["count"] += 1
+            else:
+                d[parent]["deleted"] += 1
+            if file_played:
+                d[parent]["played"] += 1
+
+    for path, pdict in list(d.items()):
+        if pdict["count"] == 0:
+            d.pop(path)
+        elif not args.depth:
+            if pdict["count"] < (args.lower or 4):
+                d.pop(path)
+            elif pdict["count"] > (args.upper or 4000):
+                d.pop(path)
+
+    return [{**v, "path": k} for k, v in d.items()]
+
+
+def group_folders(args, folders) -> List[Dict]:
+    d = {}
+    for f in folders:
+        p = f["path"].split("/")
+        p.pop()
+
+        depth = 1 + args.depth
+        parent = "/".join(p[:depth]) + "/"
+        if len(p) < depth:
             continue
 
-        if "media" in tables and not args.playlist_db:
-            m_columns = args.db["media"].columns_dict
-            playlist_already_added = list(
-                args.db.query(
-                    f"""
-                    SELECT path from media
-                    WHERE 1=1
-                    AND (path=? or {'web' if 'webpath' in m_columns else ''}path=?)
-                    """,
-                    [path, path],
-                ),
-            )
-            if playlist_already_added:
-                log.info("[%s]: Already added. Skipping!", path)
-                continue
-
-        tube_backend.process_playlist(args, path, tube_backend.tube_opts(args))
-
-        if args.extra:
-            log.warning("[%s]: Getting extra metadata", path)
-            tube_backend.get_extra_metadata(args, path)
-
-    LARGE_NUMBER = 100_000
-    if not args.db["media"].detect_fts() or tube_backend.added_media_count > LARGE_NUMBER:
-        db.optimize(args)
-
-
-def tube_update(args=None) -> None:
-    if args:
-        sys.argv = ["tubeupdate", *args]
-
-    args = parse_args(SC.tubeupdate, usage=usage.tubeupdate)
-    playlists = db.get_playlists(args, constrain=True)
-    tube_backend.update_playlists(args, playlists)
+        if d.get(parent):
+            d[parent]["size"] += f["size"]
+            d[parent]["count"] += f["count"]
+            d[parent]["deleted"] += f["deleted"]
+            d[parent]["played"] += f["played"]
+        else:
+            d[parent] = f
+
+    for path, pdict in list(d.items()):
+        if args.lower is not None and pdict["count"] < args.lower:
+            d.pop(path)
+        elif args.upper is not None and pdict["count"] > args.upper:
+            d.pop(path)
+
+    return [{**v, "path": k} for k, v in d.items()]
+
+
+def get_table(args) -> List[dict]:
+    m_columns = args.db["media"].columns_dict
+    args.filter_sql = []
+    args.filter_bindings = {}
+
+    if args.size:
+        args.filter_sql.append(" and size IS NOT NULL " + args.size)
+    db.construct_search_bindings(args, m_columns)
+
+    media = list(
+        args.db.query(
+            f"""
+        select
+            path
+            , size
+            {', time_deleted' if 'time_deleted' in m_columns else ''}
+            {', time_played' if 'time_played' in m_columns else ''}
+        from media m
+        where 1=1
+            {'and time_downloaded > 0' if 'time_downloaded' in m_columns else ''}
+            {" ".join(args.filter_sql)}
+        order by path
+        """,
+            args.filter_bindings,
+        ),
+    )
+    return media
+
+
+def sort_by(args):
+    if args.sort_by:
+        if args.sort_by == "played_ratio":
+            return lambda x: x["played"] / x["deleted"] if x["deleted"] else 0
+        elif args.sort_by == "deleted_ratio":
+            return lambda x: x["deleted"] / x["played"] if x["played"] else 0
+        else:
+            return lambda x: x[args.sort_by]
+
+    return lambda x: x["size"] / x["count"]
+
+
+def process_bigdirs(args, media) -> List[Dict]:
+    folders = group_files_by_folder(args, media)
+    if args.depth:
+        folders = group_folders(args, folders)
+    return sorted(folders, key=sort_by(args))
+
+
+def bigdirs() -> None:
+    args = parse_args()
+    tbl = get_table(args)
+    tbl = process_bigdirs(args, tbl)
+
+    if args.limit:
+        tbl = tbl[-int(args.limit) :]
+
+    tbl = utils.list_dict_filter_bool(tbl, keep_0=False)
+    tbl = utils.col_resize(tbl, "path", 50)
+    tbl = utils.col_naturalsize(tbl, "size")
+    print(tabulate(tbl, tablefmt="fancy_grid", headers="keys", showindex=False))
+    if not args.limit:
+        print(f"{len(tbl)} folders found")
+
+
+if __name__ == "__main__":
+    bigdirs()
```

### Comparing `xklb-1.30.3/xklb/usage.py` & `xklb-1.30.5/xklb/usage.py`

 * *Files 0% similar despite different names*

```diff
@@ -710,15 +710,15 @@
 
     Add links from a line-delimited file
 
         library tubeadd reddit.db --playlist-file ./my_yt_subscriptions.txt
 
     Add metadata to links already in a database table
 
-        library tubeadd reddit.db --playlist-db media
+        library tubeadd --force reddit.db (sqlite-utils --raw-lines reddit.db 'select path from media')
 
     You can also include a category for file organization
 
         library tubeadd -c Mealtime dl.db (cat ~/.jobs/todo/71_Mealtime_Videos)
 
     Files will be saved to <download prefix>/<tubeadd category>/
```

### Comparing `xklb-1.30.3/xklb/utils.py` & `xklb-1.30.5/xklb/utils.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/xklb/scripts/bigdirs.py` & `xklb-1.30.5/xklb/scripts/playlists.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,173 +1,155 @@
-import argparse
-from pathlib import Path
-from typing import Dict, List
+import argparse, json
+from copy import deepcopy
+from typing import Tuple
 
 from tabulate import tabulate
 
-from xklb import db, usage, utils
+from xklb import consts, db, usage, utils
+from xklb.player import delete_playlists
 from xklb.utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(
-        prog="library bigdirs",
-        usage=usage.bigdirs,
+        "library playlists",
+        usage.playlists,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
-    parser.add_argument("--sort-by")
-    parser.add_argument("--limit", "-L", "-l", "-queue", "--queue", default="4000")
-    parser.add_argument("--depth", "-d", default=0, type=int, help="Depth of folders")
-    parser.add_argument("--lower", type=int, help="Number of files per folder lower limit")
-    parser.add_argument("--upper", type=int, help="Number of files per folder upper limit")
-    parser.add_argument(
-        "--size",
-        "-S",
-        action="append",
-        help="Only include files of specific sizes (uses the same syntax as fd-find)",
-    )
-    parser.add_argument("--include", "-s", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
+    parser.add_argument("--aggregate", "-a", action="store_true", help=argparse.SUPPRESS)
+    parser.add_argument("--json", "-j", action="store_true", help=argparse.SUPPRESS)
+    parser.add_argument("--sort", "-u", nargs="+", help=argparse.SUPPRESS)
+    parser.add_argument("--where", "-w", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
+    parser.add_argument("--include", "-s", "--search", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
     parser.add_argument("--exclude", "-E", "-e", nargs="+", action="extend", default=[], help=argparse.SUPPRESS)
-    parser.add_argument("--verbose", "-v", action="count", default=0)
+    parser.add_argument("--duration", "-d", action="append", help=argparse.SUPPRESS)
+    parser.add_argument("--limit", "-L", "-l", "-queue", "--queue", help=argparse.SUPPRESS)
+    parser.add_argument("--safe", "-safe", action="store_true", help="Skip generic URLs")
+    parser.add_argument("--errors", "-errors", "--error", action="store_true", help="Show only rows with errors")
+    parser.add_argument("--delete", "--remove", "--erase", "--rm", "-rm", nargs="+", help=argparse.SUPPRESS)
+    parser.add_argument("--print", "-p", default=False, const="p", nargs="?", help=argparse.SUPPRESS)
+
+    parser.add_argument("-v", "--verbose", action="count", default=0)
+    parser.add_argument("--db", "-db", help=argparse.SUPPRESS)
 
     parser.add_argument("database")
-    parser.add_argument("search", nargs="*")
-    args = parser.parse_intermixed_args()
+    args = parser.parse_args()
+    if args.db:
+        args.database = args.db
     args.db = db.connect(args)
-
-    args.include += args.search
-    if args.include == ["."]:
-        args.include = [str(Path().cwd().resolve())]
-
-    if args.size:
-        args.size = utils.parse_human_to_sql(utils.human_to_bytes, "size", args.size)
-
     log.info(utils.dict_filter_bool(args.__dict__))
-    return args
 
-
-def group_files_by_folder(args, media) -> List[Dict]:
-    d = {}
-    for m in media:
-        p = m["path"].split("/")
-        while len(p) >= 2:
-            p.pop()
-            parent = "/".join(p) + "/"
-
-            file_deleted = bool(m.get("time_deleted", 0))
-            file_played = bool(m.get("time_played", 0))
-            if parent not in d:
-                d[parent] = {"size": 0, "count": 0, "deleted": 0, "played": 0}
-            if not file_deleted:
-                d[parent]["size"] += m.get("size", 0)
-                d[parent]["count"] += 1
-            else:
-                d[parent]["deleted"] += 1
-            if file_played:
-                d[parent]["played"] += 1
-
-    for path, pdict in list(d.items()):
-        if pdict["count"] == 0:
-            d.pop(path)
-        elif not args.depth:
-            if pdict["count"] < (args.lower or 4):
-                d.pop(path)
-            elif pdict["count"] > (args.upper or 4000):
-                d.pop(path)
-
-    return [{**v, "path": k} for k, v in d.items()]
-
-
-def group_folders(args, folders) -> List[Dict]:
-    d = {}
-    for f in folders:
-        p = f["path"].split("/")
-        p.pop()
-
-        depth = 1 + args.depth
-        parent = "/".join(p[:depth]) + "/"
-        if len(p) < depth:
-            continue
-
-        if d.get(parent):
-            d[parent]["size"] += f["size"]
-            d[parent]["count"] += f["count"]
-            d[parent]["deleted"] += f["deleted"]
-            d[parent]["played"] += f["played"]
-        else:
-            d[parent] = f
-
-    for path, pdict in list(d.items()):
-        if args.lower is not None and pdict["count"] < args.lower:
-            d.pop(path)
-        elif args.upper is not None and pdict["count"] > args.upper:
-            d.pop(path)
-
-    return [{**v, "path": k} for k, v in d.items()]
+    args.action = consts.SC.stats
+    return args
 
 
-def get_table(args) -> List[dict]:
-    m_columns = args.db["media"].columns_dict
+def construct_query(args) -> Tuple[str, dict]:
+    utils.ensure_playlists_exists(args)
+    pl_columns = args.db["playlists"].columns_dict
     args.filter_sql = []
     args.filter_bindings = {}
 
-    if args.size:
-        args.filter_sql.append(" and size IS NOT NULL " + args.size)
-    db.construct_search_bindings(args, m_columns)
-
-    media = list(
-        args.db.query(
-            f"""
-        select
-            path
-            , size
-            {', time_deleted' if 'time_deleted' in m_columns else ''}
-            {', time_played' if 'time_played' in m_columns else ''}
-        from media m
-        where 1=1
-            {'and time_downloaded > 0' if 'time_downloaded' in m_columns else ''}
-            {" ".join(args.filter_sql)}
-        order by path
-        """,
-            args.filter_bindings,
-        ),
-    )
-    return media
-
-
-def sort_by(args):
-    if args.sort_by:
-        if args.sort_by == "played_ratio":
-            return lambda x: x["played"] / x["deleted"] if x["deleted"] else 0
-        elif args.sort_by == "deleted_ratio":
-            return lambda x: x["deleted"] / x["played"] if x["played"] else 0
-        else:
-            return lambda x: x[args.sort_by]
-
-    return lambda x: x["size"] / x["count"]
-
+    args.filter_sql.extend([" and " + w for w in args.where])
 
-def process_bigdirs(args, media) -> List[Dict]:
-    folders = group_files_by_folder(args, media)
-    if args.depth:
-        folders = group_folders(args, folders)
-    return sorted(folders, key=sort_by(args))
+    args.table = "playlists"
+    if args.db["playlists"].detect_fts():
+        if args.include:
+            args.table = db.fts_flexible_search(args)
+        elif args.exclude:
+            db.construct_search_bindings(args, pl_columns)
+    else:
+        db.construct_search_bindings(args, pl_columns)
+
+    LIMIT = "LIMIT " + str(args.limit) if args.limit else ""
+    query = f"""SELECT
+        *
+    FROM {args.table}
+    WHERE 1=1
+        and COALESCE(time_deleted,0) = 0
+        {" ".join(args.filter_sql)}
+    ORDER BY 1=1
+        {', ' + args.sort if args.sort else ''}
+        , path
+        , random()
+    {LIMIT}
+    """
+
+    return query, args.filter_bindings
+
+
+def printer(args, query, bindings) -> None:
+    media = list(args.db.query(query, bindings))
+    media = utils.list_dict_filter_bool(media)
+    if not media:
+        utils.no_media_found()
+
+    tbl = deepcopy(media)
+    utils.col_naturaldate(tbl, "avg_time_since_download")
+    utils.col_naturalsize(tbl, "size")
+    utils.col_duration(tbl, "duration")
+    utils.col_duration(tbl, "avg_playlist_duration")
+
+    if args.print and "f" in args.print:
+        utils.pipe_print("\n".join([d["path"] for d in media]))
+        return
+    elif args.json or consts.TERMINAL_SIZE.columns < 80:
+        print(json.dumps(tbl, indent=3))
+    else:
+        tbl = utils.col_resize(tbl, "path", 30)
+        tbl = utils.col_resize(tbl, "title", 20)
+        tbl = utils.col_resize(tbl, "uploader_url")
+
+        tbl = utils.list_dict_filter_bool(tbl)
+
+        print(tabulate(tbl, tablefmt="fancy_grid", headers="keys", showindex=False))
+
+    print(f"{len(media)} playlists" if len(media) > 1 else "1 playlist")
+    duration = sum(m.get("duration") or 0 for m in media)
+    if duration > 0:
+        duration = utils.human_time(duration)
+        if not args.aggregate:
+            print("Total duration:", duration)
 
 
-def bigdirs() -> None:
+def playlists() -> None:
     args = parse_args()
-    tbl = get_table(args)
-    tbl = process_bigdirs(args, tbl)
 
-    if args.limit:
-        tbl = tbl[-int(args.limit) :]
+    if args.delete:
+        return delete_playlists(args, args.delete)
 
-    tbl = utils.list_dict_filter_bool(tbl, keep_0=False)
-    tbl = utils.col_resize(tbl, "path", 50)
-    tbl = utils.col_naturalsize(tbl, "size")
-    print(tabulate(tbl, tablefmt="fancy_grid", headers="keys", showindex=False))
-    if not args.limit:
-        print(f"{len(tbl)} folders found")
+    pl_columns = args.db["playlists"].columns_dict
+    m_columns = args.db["media"].columns_dict
+    query, bindings = construct_query(args)
 
+    if "playlist_path" in m_columns:
+        query = f"""
+        select
+            coalesce(p.path, "Playlist-less media") path
+            {', p.ie_key' if 'ie_key' in pl_columns else ''}
+            {', p.title' if 'title' in pl_columns else ''}
+            {', p.time_deleted' if 'time_deleted' in pl_columns else ''}
+            {', count(*) FILTER(WHERE play_count>0) play_count' if 'play_count' in m_columns else ''}
+            {', sum(m.duration) duration' if 'duration' in m_columns else ''}
+            {', sum(m.size) size' if 'size' in m_columns else ''}
+            , count(*) count
+        from media m
+        left join ({query}) p on (p.path = m.playlist_path {"and p.ie_key = m.ie_key and m.ie_key != 'Local'" if 'ie_key' in m_columns else ''})
+        group by coalesce(p.path, "Playlist-less media")
+        order by count, p.category nulls last, p.path
+        """
+
+    if args.aggregate:
+        query = f"""
+        select
+            'Aggregate of playlists' path
+            {', count(*) FILTER(WHERE time_deleted>0) deleted_count' if 'time_deleted' in query else ''}
+            {', sum(play_count) play_count' if 'play_count' in query else ''}
+            {', sum(duration) duration' if 'duration' in query else ''}
+            {', avg(duration) avg_playlist_duration' if 'duration' in query else ''}
+            {', sum(size) size' if 'size' in query else ''}
+            , count(*) playlists_count
+            {', sum(count) videos_count' if 'count' in query else ''}
+        from ({query})
+        """
 
-if __name__ == "__main__":
-    bigdirs()
+    printer(args, query, bindings)
+    return None
```

### Comparing `xklb-1.30.3/xklb/scripts/block.py` & `xklb-1.30.5/xklb/scripts/block.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/xklb/scripts/christen.py` & `xklb-1.30.5/xklb/scripts/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/xklb/scripts/cluster_sort.py` & `xklb-1.30.5/xklb/scripts/cluster_sort.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/xklb/scripts/copy_play_counts.py` & `xklb-1.30.5/xklb/scripts/copy_play_counts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/xklb/scripts/dedupe.py` & `xklb-1.30.5/xklb/scripts/dedupe.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/xklb/scripts/download_status.py` & `xklb-1.30.5/xklb/scripts/download_status.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/xklb/scripts/history.py` & `xklb-1.30.5/xklb/scripts/history.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/xklb/scripts/merge_dbs.py` & `xklb-1.30.5/xklb/scripts/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/xklb/scripts/merge_online_local.py` & `xklb-1.30.5/xklb/scripts/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/xklb/scripts/move_list.py` & `xklb-1.30.5/xklb/scripts/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/xklb/scripts/optimize_db.py` & `xklb-1.30.5/xklb/scripts/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/xklb/scripts/redownload.py` & `xklb-1.30.5/xklb/scripts/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/xklb/scripts/relmv.py` & `xklb-1.30.5/xklb/scripts/relmv.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/xklb/scripts/scatter.py` & `xklb-1.30.5/xklb/scripts/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/xklb/scripts/streaming_tab_loader.py` & `xklb-1.30.5/xklb/scripts/streaming_tab_loader.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/xklb/scripts/mining/data.py` & `xklb-1.30.5/xklb/scripts/mining/data.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/xklb/scripts/mining/extract_links.py` & `xklb-1.30.5/xklb/scripts/mining/extract_links.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/xklb/scripts/mining/nouns.py` & `xklb-1.30.5/xklb/scripts/mining/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/xklb/scripts/mining/pushshift.py` & `xklb-1.30.5/xklb/scripts/mining/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/xklb/scripts/mining/reddit_selftext.py` & `xklb-1.30.5/xklb/scripts/mining/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/xklb/assets/kotobago.png` & `xklb-1.30.5/xklb/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/.gitignore` & `xklb-1.30.5/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/LICENSE` & `xklb-1.30.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/README.md` & `xklb-1.30.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 Incremental surfing. 📈🏄 totally rad!
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.30.003)
+    xk media library subcommands (v1.30.005)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
@@ -499,15 +499,15 @@
         end
     end | parallel -j8
 
     for subreddit in $subreddits
         sqlite-utils upsert --pk path --alter --csv --detect-types $reddit_db media $subreddit.csv
     end
 
-    library tubeadd --safe -i $reddit_db --playlist-db media
+    library tubeadd --safe --ignore-errors --force $reddit_db (sqlite-utils --raw-lines $reddit_db 'select path from media')
 end
 ```
 
 </details>
 
 ### Datasette
 
@@ -582,15 +582,15 @@
 
     Add links from a line-delimited file
 
         library tubeadd reddit.db --playlist-file ./my_yt_subscriptions.txt
 
     Add metadata to links already in a database table
 
-        library tubeadd reddit.db --playlist-db media
+        library tubeadd --force reddit.db (sqlite-utils --raw-lines reddit.db 'select path from media')
 
     You can also include a category for file organization
 
         library tubeadd -c Mealtime dl.db (cat ~/.jobs/todo/71_Mealtime_Videos)
 
     Files will be saved to <download prefix>/<tubeadd category>/
```

### Comparing `xklb-1.30.3/pyproject.toml` & `xklb-1.30.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xklb-1.30.3/PKG-INFO` & `xklb-1.30.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xklb
-Version: 1.30.3
+Version: 1.30.5
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
-    xk media library subcommands (v1.30.003)
+    xk media library subcommands (v1.30.005)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
@@ -583,15 +583,15 @@
         end
     end | parallel -j8
 
     for subreddit in $subreddits
         sqlite-utils upsert --pk path --alter --csv --detect-types $reddit_db media $subreddit.csv
     end
 
-    library tubeadd --safe -i $reddit_db --playlist-db media
+    library tubeadd --safe --ignore-errors --force $reddit_db (sqlite-utils --raw-lines $reddit_db 'select path from media')
 end
 ```
 
 </details>
 
 ### Datasette
 
@@ -666,15 +666,15 @@
 
     Add links from a line-delimited file
 
         library tubeadd reddit.db --playlist-file ./my_yt_subscriptions.txt
 
     Add metadata to links already in a database table
 
-        library tubeadd reddit.db --playlist-db media
+        library tubeadd --force reddit.db (sqlite-utils --raw-lines reddit.db 'select path from media')
 
     You can also include a category for file organization
 
         library tubeadd -c Mealtime dl.db (cat ~/.jobs/todo/71_Mealtime_Videos)
 
     Files will be saved to <download prefix>/<tubeadd category>/
```

