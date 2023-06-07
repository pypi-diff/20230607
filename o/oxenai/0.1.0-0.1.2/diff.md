# Comparing `tmp/oxenai-0.1.0.tar.gz` & `tmp/oxenai-0.1.2.tar.gz`

## Comparing `oxenai-0.1.0.tar` & `oxenai-0.1.2.tar`

### file list

```diff
@@ -1,86 +1,239 @@
--rw-r--r--   0        0        0      434 1970-01-01 00:00:00.000000 oxenai-0.1.0/Cargo.toml
--rw-r--r--   0      501       20     2809 2023-04-24 18:10:45.000000 oxenai-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0      501       20      685 2023-04-24 18:10:45.000000 oxenai-0.1.0/.gitignore
--rw-r--r--   0      501       20      984 2023-05-11 16:11:21.000000 oxenai-0.1.0/README.md
--rw-r--r--   0      501       20      638 2023-05-16 20:02:04.000000 oxenai-0.1.0/docs/Makefile
--rw-r--r--   0      501       20      804 2023-05-16 20:02:04.000000 oxenai-0.1.0/docs/make.bat
--rw-r--r--   0      501       20     1348 2023-05-18 04:48:44.000000 oxenai-0.1.0/docs/source/conf.py
--rw-r--r--   0      501       20      435 2023-05-17 22:27:30.000000 oxenai-0.1.0/docs/source/getting_started/commands.md
--rw-r--r--   0      501       20     2148 2023-05-18 04:14:06.000000 oxenai-0.1.0/docs/source/getting_started/installation.md
--rw-r--r--   0      501       20     1041 2023-05-18 03:41:56.000000 oxenai-0.1.0/docs/source/getting_started/python.md
--rw-r--r--   0      501       20       18 2023-05-17 00:07:17.000000 oxenai-0.1.0/docs/source/getting_started/tutorials.md
--rw-r--r--   0      501       20      753 2023-05-18 04:21:40.000000 oxenai-0.1.0/docs/source/index.rst
--rw-r--r--   0      501       20       69 2023-05-18 03:59:38.000000 oxenai-0.1.0/docs/source/references/python/local_repo.rst
--rw-r--r--   0      501       20       68 2023-05-18 04:14:40.000000 oxenai-0.1.0/docs/source/references/python/remote_repo.rst
--rw-r--r--   0      501       20      235 2023-05-18 04:22:39.000000 oxenai-0.1.0/docs/source/references/rust.md
--rw-r--r--   0      501       20      451 2023-05-18 05:03:17.000000 oxenai-0.1.0/pyproject.toml
--rw-r--r--   0      501       20      560 2023-05-18 04:28:27.000000 oxenai-0.1.0/python/oxen/__init__.py
--rw-r--r--   0      501       20      656 2023-05-12 22:34:40.000000 oxenai-0.1.0/python/oxen/dag.py
--rw-r--r--   0      501       20     5995 2023-05-12 22:03:31.000000 oxenai-0.1.0/python/oxen/dataset.py
--rw-r--r--   0      501       20     1378 2023-05-11 01:03:21.000000 oxenai-0.1.0/python/oxen/features.py
--rw-r--r--   0      501       20      181 2023-05-12 22:50:15.000000 oxenai-0.1.0/python/oxen/loaders/__init__.py
--rw-r--r--   0      501       20     1057 2023-05-12 22:37:03.000000 oxenai-0.1.0/python/oxen/loaders/chat.py
--rw-r--r--   0      501       20        0 2023-05-12 02:11:27.000000 oxenai-0.1.0/python/oxen/loaders/image_classification.py
--rw-r--r--   0      501       20      802 2023-05-12 22:56:45.000000 oxenai-0.1.0/python/oxen/loaders/regression.py
--rw-r--r--   0      501       20     3732 2023-05-18 04:48:44.000000 oxenai-0.1.0/python/oxen/local_repo.py
--rw-r--r--   0      501       20     1498 2023-05-12 22:34:23.000000 oxenai-0.1.0/python/oxen/op.py
--rw-r--r--   0      501       20      390 2023-05-12 21:46:13.000000 oxenai-0.1.0/python/oxen/ops/__init__.py
--rw-r--r--   0      501       20      207 2023-05-12 21:46:13.000000 oxenai-0.1.0/python/oxen/ops/concat_series.py
--rw-r--r--   0      501       20      203 2023-05-12 21:46:13.000000 oxenai-0.1.0/python/oxen/ops/extract_col.py
--rw-r--r--   0      501       20      214 2023-05-12 22:34:50.000000 oxenai-0.1.0/python/oxen/ops/identity.py
--rw-r--r--   0      501       20      224 2023-05-12 22:35:42.000000 oxenai-0.1.0/python/oxen/ops/read_df.py
--rw-r--r--   0      501       20      235 2023-05-12 22:35:42.000000 oxenai-0.1.0/python/oxen/ops/read_text.py
--rw-r--r--   0      501       20      354 2023-05-12 22:33:21.000000 oxenai-0.1.0/python/oxen/ops/str_col_template.py
--rw-r--r--   0      501       20     5494 2023-05-18 04:48:44.000000 oxenai-0.1.0/python/oxen/remote_repo.py
--rw-r--r--   0      501       20        0 2023-04-27 17:45:52.000000 oxenai-0.1.0/python/oxen/util/__init__.py
--rw-r--r--   0      501       20     1500 2023-05-18 04:26:23.000000 oxenai-0.1.0/python/oxen/util/fs.py
--rw-r--r--   0      501       20      144 2023-05-18 04:12:52.000000 oxenai-0.1.0/requirements.txt
--rw-r--r--   0      501       20      370 2023-04-26 18:47:19.000000 oxenai-0.1.0/src/error.rs
--rw-r--r--   0      501       20     1726 2023-05-18 04:50:52.000000 oxenai-0.1.0/src/lib.rs
--rw-r--r--   0      501       20      718 2023-05-18 04:53:34.000000 oxenai-0.1.0/src/py_branch.rs
--rw-r--r--   0      501       20      291 2023-04-26 18:47:19.000000 oxenai-0.1.0/src/py_commit.rs
--rw-r--r--   0      501       20      474 2023-05-05 03:46:35.000000 oxenai-0.1.0/src/py_dataset.rs
--rw-r--r--   0      501       20     3875 2023-05-18 04:51:00.000000 oxenai-0.1.0/src/py_local_repo.rs
--rw-r--r--   0      501       20     8111 2023-05-18 04:50:52.000000 oxenai-0.1.0/src/py_remote_repo.rs
--rw-r--r--   0      501       20     1572 2023-05-17 00:12:30.000000 oxenai-0.1.0/src/py_staged_data.rs
--rw-r--r--   0      501       20      538 2023-05-17 00:12:30.000000 oxenai-0.1.0/src/util.rs
--rw-r--r--   0      501       20      345 2023-05-18 02:53:28.000000 oxenai-0.1.0/test.py
--rw-r--r--   0      501       20        0 2023-04-26 19:43:28.000000 oxenai-0.1.0/tests/__init__.py
--rw-r--r--   0      501       20     3474 2023-05-18 04:26:36.000000 oxenai-0.1.0/tests/conftest.py
--rw-r--r--   0      501       20      114 2023-04-25 22:04:20.000000 oxenai-0.1.0/tests/data/CelebA/annotations/test.csv
--rw-r--r--   0      501       20      139 2023-04-25 22:04:25.000000 oxenai-0.1.0/tests/data/CelebA/annotations/train.csv
--rw-r--r--   0      501       20    11440 2023-04-25 21:59:53.000000 oxenai-0.1.0/tests/data/CelebA/images/1.jpg
--rw-r--r--   0      501       20     7448 2023-04-25 21:59:53.000000 oxenai-0.1.0/tests/data/CelebA/images/2.jpg
--rw-r--r--   0      501       20     4253 2023-04-25 21:59:53.000000 oxenai-0.1.0/tests/data/CelebA/images/3.jpg
--rw-r--r--   0      501       20    10747 2023-04-25 21:59:53.000000 oxenai-0.1.0/tests/data/CelebA/images/4.jpg
--rw-r--r--   0      501       20     6351 2023-04-25 21:59:53.000000 oxenai-0.1.0/tests/data/CelebA/images/5.jpg
--rw-r--r--   0      501       20     8073 2023-04-25 21:59:53.000000 oxenai-0.1.0/tests/data/CelebA/images/6.jpg
--rw-r--r--   0      501       20     8203 2023-04-25 21:59:53.000000 oxenai-0.1.0/tests/data/CelebA/images/7.jpg
--rw-r--r--   0      501       20     7725 2023-04-25 21:59:53.000000 oxenai-0.1.0/tests/data/CelebA/images/8.jpg
--rw-r--r--   0      501       20     8641 2023-04-25 21:59:53.000000 oxenai-0.1.0/tests/data/CelebA/images/9.jpg
--rw-r--r--   0      501       20      337 2023-05-12 22:23:52.000000 oxenai-0.1.0/tests/data/ChatBot/examples.tsv
--rw-r--r--   0      501       20       88 2023-05-12 22:31:17.000000 oxenai-0.1.0/tests/data/ChatBot/prompt.txt
--rw-r--r--   0      501       20      148 2023-05-12 22:42:34.000000 oxenai-0.1.0/tests/data/HousePrices/prices.csv
--rw-r--r--   0      501       20      477 2023-05-18 04:26:41.000000 oxenai-0.1.0/tests/test_add.py
--rw-r--r--   0      501       20      363 2023-05-12 22:35:42.000000 oxenai-0.1.0/tests/test_chat_loader.py
--rw-r--r--   0      501       20     1299 2023-05-18 04:46:14.000000 oxenai-0.1.0/tests/test_checkout.py
--rw-r--r--   0      501       20      716 2023-05-18 04:26:46.000000 oxenai-0.1.0/tests/test_clone.py
--rw-r--r--   0      501       20      850 2023-04-29 18:40:43.000000 oxenai-0.1.0/tests/test_commit.py
--rw-r--r--   0      501       20     2444 2023-05-18 04:50:44.000000 oxenai-0.1.0/tests/test_dataloader_pytorch.py
--rw-r--r--   0      501       20     1506 2023-05-18 04:48:44.000000 oxenai-0.1.0/tests/test_dataset.py
--rw-r--r--   0      501       20      338 2023-05-18 04:26:51.000000 oxenai-0.1.0/tests/test_init.py
--rw-r--r--   0      501       20      440 2023-04-29 22:00:54.000000 oxenai-0.1.0/tests/test_push.py
--rw-r--r--   0      501       20      916 2023-05-18 04:26:56.000000 oxenai-0.1.0/tests/test_push_pull.py
--rw-r--r--   0      501       20      488 2023-05-12 22:56:45.000000 oxenai-0.1.0/tests/test_regression_loader.py
--rw-r--r--   0      501       20      828 2023-05-17 00:12:30.000000 oxenai-0.1.0/tests/test_remote_add.py
--rw-r--r--   0      501       20      560 2023-05-17 00:12:30.000000 oxenai-0.1.0/tests/test_remote_branch.py
--rw-r--r--   0      501       20      538 2023-05-18 04:50:44.000000 oxenai-0.1.0/tests/test_remote_checkout.py
--rw-r--r--   0      501       20      685 2023-05-17 00:12:30.000000 oxenai-0.1.0/tests/test_remote_commit.py
--rw-r--r--   0      501       20     1473 2023-05-18 04:50:44.000000 oxenai-0.1.0/tests/test_remote_df_add.py
--rw-r--r--   0      501       20      530 2023-05-17 00:12:30.000000 oxenai-0.1.0/tests/test_remote_list.py
--rw-r--r--   0      501       20      657 2023-05-17 00:12:30.000000 oxenai-0.1.0/tests/test_remote_remove.py
--rw-r--r--   0      501       20      114 2023-04-27 16:40:57.000000 oxenai-0.1.0/tests/test_remote_repo.py
--rw-r--r--   0      501       20      636 2023-05-17 00:12:30.000000 oxenai-0.1.0/tests/test_remote_status.py
--rw-r--r--   0      501       20      259 2023-05-18 04:27:00.000000 oxenai-0.1.0/tests/test_status.py
--rw-r--r--   0      501       20   109486 2023-05-17 21:25:52.000000 oxenai-0.1.0/Cargo.lock
--rw-r--r--   0        0        0     1360 1970-01-01 00:00:00.000000 oxenai-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      432 1970-01-01 00:00:00.000000 oxenai-0.1.2/Cargo.toml
+-rw-r--r--   0      501       20     2809 2023-05-18 05:25:22.000000 oxenai-0.1.2/.github/workflows/CI.yml
+-rw-r--r--   0      501       20      687 2023-05-18 16:10:10.000000 oxenai-0.1.2/.gitignore
+-rw-r--r--   0      501       20     1255 2023-06-07 15:31:28.000000 oxenai-0.1.2/Develop.md
+-rw-r--r--   0      501       20     1840 2023-06-07 15:31:28.000000 oxenai-0.1.2/README.md
+-rw-r--r--   0      501       20      638 2023-05-18 05:25:22.000000 oxenai-0.1.2/docs/Makefile
+-rw-r--r--   0      501       20   111104 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/doctrees/concepts/data_frames.doctree
+-rw-r--r--   0      501       20     2426 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/doctrees/concepts/embedding_search.doctree
+-rw-r--r--   0      501       20    33060 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/doctrees/concepts/remote_staging.doctree
+-rw-r--r--   0      501       20     4832 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/doctrees/contributing/documentation.doctree
+-rw-r--r--   0      501       20     3114 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/doctrees/contributing/python.doctree
+-rw-r--r--   0      501       20     3041 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/doctrees/contributing/rust.doctree
+-rw-r--r--   0      501       20   521114 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/doctrees/environment.pickle
+-rw-r--r--   0      501       20     4632 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/doctrees/getting_started/commands.doctree
+-rw-r--r--   0      501       20    13327 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/doctrees/getting_started/installation.doctree
+-rw-r--r--   0      501       20     8868 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/doctrees/getting_started/python.doctree
+-rw-r--r--   0      501       20     2515 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/doctrees/getting_started/tutorials.doctree
+-rw-r--r--   0      501       20    92642 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/doctrees/index.doctree
+-rw-r--r--   0      501       20    41036 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/doctrees/references/python/local_repo.doctree
+-rw-r--r--   0      501       20    54552 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/doctrees/references/python/remote_repo.doctree
+-rw-r--r--   0      501       20     3870 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/doctrees/references/rust.doctree
+-rw-r--r--   0      501       20      230 2023-05-30 22:47:04.000000 oxenai-0.1.2/docs/build/html/.buildinfo
+-rw-r--r--   0      501       20    45695 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/html/_sources/concepts/data_frames.md
+-rw-r--r--   0      501       20       18 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/html/_sources/concepts/embedding_search.md
+-rw-r--r--   0      501       20    10491 2023-05-30 22:47:04.000000 oxenai-0.1.2/docs/build/html/_sources/concepts/remote_staging.md
+-rw-r--r--   0      501       20      435 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/html/_sources/contributing/documentation.md
+-rw-r--r--   0      501       20      165 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/html/_sources/contributing/python.md
+-rw-r--r--   0      501       20      135 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/html/_sources/contributing/rust.md
+-rw-r--r--   0      501       20      435 2023-05-17 22:27:30.000000 oxenai-0.1.2/docs/build/html/_sources/getting_started/commands.md
+-rw-r--r--   0      501       20     2148 2023-05-18 04:14:06.000000 oxenai-0.1.2/docs/build/html/_sources/getting_started/installation.md
+-rw-r--r--   0      501       20     1816 2023-05-30 22:47:04.000000 oxenai-0.1.2/docs/build/html/_sources/getting_started/python.md
+-rw-r--r--   0      501       20       18 2023-05-17 00:07:17.000000 oxenai-0.1.2/docs/build/html/_sources/getting_started/tutorials.md
+-rw-r--r--   0      501       20     1130 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/html/_sources/index.rst
+-rw-r--r--   0      501       20       69 2023-05-18 03:59:38.000000 oxenai-0.1.2/docs/build/html/_sources/references/python/local_repo.rst
+-rw-r--r--   0      501       20       68 2023-05-18 04:14:40.000000 oxenai-0.1.2/docs/build/html/_sources/references/python/remote_repo.rst
+-rw-r--r--   0      501       20      235 2023-05-18 04:22:39.000000 oxenai-0.1.2/docs/build/html/_sources/references/rust.md
+-rw-r--r--   0      501       20    14813 2023-05-24 22:24:23.000000 oxenai-0.1.2/docs/build/html/_static/basic.css
+-rw-r--r--   0      501       20      313 2023-05-16 23:41:23.000000 oxenai-0.1.2/docs/build/html/_static/check-solid.svg
+-rw-r--r--   0      501       20     9031 2023-05-16 23:41:23.000000 oxenai-0.1.2/docs/build/html/_static/clipboard.min.js
+-rw-r--r--   0      501       20      411 2023-05-16 23:41:23.000000 oxenai-0.1.2/docs/build/html/_static/copy-button.svg
+-rw-r--r--   0      501       20     2060 2023-05-16 23:41:23.000000 oxenai-0.1.2/docs/build/html/_static/copybutton.css
+-rw-r--r--   0      501       20     8469 2023-05-30 22:47:04.000000 oxenai-0.1.2/docs/build/html/_static/copybutton.js
+-rw-r--r--   0      501       20     2698 2023-05-16 23:41:23.000000 oxenai-0.1.2/docs/build/html/_static/copybutton_funcs.js
+-rw-r--r--   0      501       20     4472 2023-05-16 20:00:40.000000 oxenai-0.1.2/docs/build/html/_static/doctools.js
+-rw-r--r--   0      501       20      415 2023-05-24 22:24:23.000000 oxenai-0.1.2/docs/build/html/_static/documentation_options.js
+-rw-r--r--   0      501       20      286 2023-05-16 20:00:40.000000 oxenai-0.1.2/docs/build/html/_static/file.png
+-rw-r--r--   0      501       20     1186 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/images/logo_binder.svg
+-rw-r--r--   0      501       20     7601 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/images/logo_colab.png
+-rw-r--r--   0      501       20      681 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/images/logo_deepnote.svg
+-rw-r--r--   0      501       20     1758 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/images/logo_jupyterhub.svg
+-rw-r--r--   0      501       20     4758 2023-05-24 22:24:23.000000 oxenai-0.1.2/docs/build/html/_static/language_data.js
+-rw-r--r--   0      501       20     1459 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/ar/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1626 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/bg/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1564 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/bn/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1166 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/ca/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1323 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/cs/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1222 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/da/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1306 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/de/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1640 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/el/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1255 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/eo/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1314 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/es/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1259 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/et/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1286 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/fi/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1330 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/fr/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1320 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/hr/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1241 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/id/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1321 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/it/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1363 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/iw/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1389 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/ja/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1293 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/ko/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1331 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/lt/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1322 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/lv/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1803 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/ml/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1594 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/mr/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1133 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/ms/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1274 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/nl/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1235 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/no/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1289 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/pl/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1282 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/pt/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1308 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/ro/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1640 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/ru/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1311 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/sk/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1292 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/sl/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1597 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/sr/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1267 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/sv/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1848 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/ta/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1726 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/te/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1546 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/tg/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1684 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/th/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1193 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/tl/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1291 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/tr/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1601 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/uk/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1382 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/ur/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1349 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/vi/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1228 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1259 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20       90 2023-05-16 20:00:40.000000 oxenai-0.1.2/docs/build/html/_static/minus.png
+-rw-r--r--   0      501       20       90 2023-05-16 20:00:40.000000 oxenai-0.1.2/docs/build/html/_static/plus.png
+-rw-r--r--   0      501       20    12757 2023-05-24 22:24:23.000000 oxenai-0.1.2/docs/build/html/_static/pygments.css
+-rw-r--r--   0      501       20      419 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/sbt-webpack-macros.html
+-rw-r--r--   0      501       20    80813 2023-05-16 20:04:17.000000 oxenai-0.1.2/docs/build/html/_static/scripts/bootstrap.js
+-rw-r--r--   0      501       20      237 2023-05-16 20:04:17.000000 oxenai-0.1.2/docs/build/html/_static/scripts/bootstrap.js.LICENSE.txt
+-rw-r--r--   0      501       20   335757 2023-05-16 20:04:17.000000 oxenai-0.1.2/docs/build/html/_static/scripts/bootstrap.js.map
+-rw-r--r--   0      501       20     4456 2023-05-16 20:04:17.000000 oxenai-0.1.2/docs/build/html/_static/scripts/pydata-sphinx-theme.js
+-rw-r--r--   0      501       20    19648 2023-05-16 20:04:17.000000 oxenai-0.1.2/docs/build/html/_static/scripts/pydata-sphinx-theme.js.map
+-rw-r--r--   0      501       20     3075 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/scripts/sphinx-book-theme.js
+-rw-r--r--   0      501       20    13066 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/scripts/sphinx-book-theme.js.map
+-rw-r--r--   0      501       20    18215 2023-05-16 20:00:40.000000 oxenai-0.1.2/docs/build/html/_static/searchtools.js
+-rw-r--r--   0      501       20     4712 2023-05-16 20:00:40.000000 oxenai-0.1.2/docs/build/html/_static/sphinx_highlight.js
+-rw-r--r--   0      501       20   176654 2023-05-16 20:04:17.000000 oxenai-0.1.2/docs/build/html/_static/styles/bootstrap.css
+-rw-r--r--   0      501       20    63341 2023-05-16 20:04:17.000000 oxenai-0.1.2/docs/build/html/_static/styles/pydata-sphinx-theme.css
+-rw-r--r--   0      501       20    13841 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/styles/sphinx-book-theme.css
+-rw-r--r--   0      501       20      106 2023-05-16 20:04:17.000000 oxenai-0.1.2/docs/build/html/_static/styles/theme.css
+-rw-r--r--   0      501       20     7427 2023-05-16 20:04:17.000000 oxenai-0.1.2/docs/build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt
+-rw-r--r--   0      501       20   101691 2023-05-16 20:04:17.000000 oxenai-0.1.2/docs/build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css
+-rw-r--r--   0      501       20   181264 2023-05-16 20:04:17.000000 oxenai-0.1.2/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf
+-rw-r--r--   0      501       20   105112 2023-05-16 20:04:17.000000 oxenai-0.1.2/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2
+-rw-r--r--   0      501       20    60236 2023-05-16 20:04:17.000000 oxenai-0.1.2/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf
+-rw-r--r--   0      501       20    24028 2023-05-16 20:04:17.000000 oxenai-0.1.2/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2
+-rw-r--r--   0      501       20   389948 2023-05-16 20:04:17.000000 oxenai-0.1.2/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf
+-rw-r--r--   0      501       20   154840 2023-05-16 20:04:17.000000 oxenai-0.1.2/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2
+-rw-r--r--   0      501       20    10084 2023-05-16 20:04:17.000000 oxenai-0.1.2/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0      501       20     4776 2023-05-16 20:04:17.000000 oxenai-0.1.2/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2
+-rw-r--r--   0      501       20     1863 2023-05-16 20:04:17.000000 oxenai-0.1.2/docs/build/html/_static/webpack-macros.html
+-rw-r--r--   0      501       20    94792 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/html/concepts/data_frames.html
+-rw-r--r--   0      501       20    12188 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/html/concepts/embedding_search.html
+-rw-r--r--   0      501       20    41523 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/html/concepts/remote_staging.html
+-rw-r--r--   0      501       20    13736 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/html/contributing/documentation.html
+-rw-r--r--   0      501       20    14226 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/html/contributing/python.html
+-rw-r--r--   0      501       20    13585 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/html/contributing/rust.html
+-rw-r--r--   0      501       20    17490 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/html/genindex.html
+-rw-r--r--   0      501       20    14743 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/html/getting_started/commands.html
+-rw-r--r--   0      501       20    21507 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/html/getting_started/installation.html
+-rw-r--r--   0      501       20    18772 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/html/getting_started/python.html
+-rw-r--r--   0      501       20    12068 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/html/getting_started/tutorials.html
+-rw-r--r--   0      501       20    72087 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/html/index.html
+-rw-r--r--   0      501       20      888 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/html/objects.inv
+-rw-r--r--   0      501       20    29798 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/html/references/python/local_repo.html
+-rw-r--r--   0      501       20    36459 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/html/references/python/remote_repo.html
+-rw-r--r--   0      501       20    13229 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/html/references/rust.html
+-rw-r--r--   0      501       20    11383 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/html/search.html
+-rw-r--r--   0      501       20    23670 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/html/searchindex.js
+-rw-r--r--   0      501       20       99 2023-05-30 22:47:04.000000 oxenai-0.1.2/docs/docsenv/pyvenv.cfg
+-rw-r--r--   0      501       20      804 2023-05-18 05:25:22.000000 oxenai-0.1.2/docs/make.bat
+-rw-r--r--   0      501       20      131 2023-06-07 15:47:27.000000 oxenai-0.1.2/docs/requirements.txt
+-rw-r--r--   0      501       20    45695 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/source/concepts/data_frames.md
+-rw-r--r--   0      501       20       24 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/source/concepts/embedding_search.md
+-rw-r--r--   0      501       20    10491 2023-05-30 22:47:04.000000 oxenai-0.1.2/docs/source/concepts/remote_staging.md
+-rw-r--r--   0      501       20     1395 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/source/conf.py
+-rw-r--r--   0      501       20      435 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/source/contributing/documentation.md
+-rw-r--r--   0      501       20      165 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/source/contributing/python.md
+-rw-r--r--   0      501       20      135 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/source/contributing/rust.md
+-rw-r--r--   0      501       20      435 2023-05-18 05:25:22.000000 oxenai-0.1.2/docs/source/getting_started/commands.md
+-rw-r--r--   0      501       20     2148 2023-05-18 05:25:22.000000 oxenai-0.1.2/docs/source/getting_started/installation.md
+-rw-r--r--   0      501       20     1816 2023-05-30 22:47:04.000000 oxenai-0.1.2/docs/source/getting_started/python.md
+-rw-r--r--   0      501       20       18 2023-05-18 05:25:22.000000 oxenai-0.1.2/docs/source/getting_started/tutorials.md
+-rw-r--r--   0      501       20     1130 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/source/index.rst
+-rw-r--r--   0      501       20       69 2023-05-18 05:25:22.000000 oxenai-0.1.2/docs/source/references/python/local_repo.rst
+-rw-r--r--   0      501       20       68 2023-05-18 05:25:22.000000 oxenai-0.1.2/docs/source/references/python/remote_repo.rst
+-rw-r--r--   0      501       20      235 2023-05-18 05:25:22.000000 oxenai-0.1.2/docs/source/references/rust.md
+-rw-r--r--   0      501       20      451 2023-05-18 05:25:22.000000 oxenai-0.1.2/pyproject.toml
+-rw-r--r--   0      501       20      593 2023-06-07 15:31:28.000000 oxenai-0.1.2/python/oxen/__init__.py
+-rw-r--r--   0      501       20      597 2023-06-07 15:31:28.000000 oxenai-0.1.2/python/oxen/auth.py
+-rw-r--r--   0      501       20      746 2023-06-07 15:31:28.000000 oxenai-0.1.2/python/oxen/dag.py
+-rw-r--r--   0      501       20     5995 2023-05-18 05:25:22.000000 oxenai-0.1.2/python/oxen/dataset.py
+-rw-r--r--   0      501       20     1378 2023-05-18 05:25:22.000000 oxenai-0.1.2/python/oxen/features.py
+-rw-r--r--   0      501       20     1500 2023-06-07 15:31:28.000000 oxenai-0.1.2/python/oxen/fs.py
+-rw-r--r--   0      501       20      259 2023-06-07 15:31:28.000000 oxenai-0.1.2/python/oxen/loaders/__init__.py
+-rw-r--r--   0      501       20     1057 2023-05-18 05:25:22.000000 oxenai-0.1.2/python/oxen/loaders/chat.py
+-rw-r--r--   0      501       20     1159 2023-06-07 15:31:28.000000 oxenai-0.1.2/python/oxen/loaders/image_classification.py
+-rw-r--r--   0      501       20      802 2023-05-18 05:25:22.000000 oxenai-0.1.2/python/oxen/loaders/regression.py
+-rw-r--r--   0      501       20     3732 2023-05-18 05:25:22.000000 oxenai-0.1.2/python/oxen/local_repo.py
+-rw-r--r--   0      501       20     1543 2023-06-07 15:31:28.000000 oxenai-0.1.2/python/oxen/op.py
+-rw-r--r--   0      501       20      578 2023-06-07 15:31:28.000000 oxenai-0.1.2/python/oxen/ops/__init__.py
+-rw-r--r--   0      501       20      207 2023-05-18 05:25:22.000000 oxenai-0.1.2/python/oxen/ops/concat_series.py
+-rw-r--r--   0      501       20      876 2023-06-07 15:31:28.000000 oxenai-0.1.2/python/oxen/ops/create_label_map.py
+-rw-r--r--   0      501       20      493 2023-06-07 15:31:28.000000 oxenai-0.1.2/python/oxen/ops/encode_labels.py
+-rw-r--r--   0      501       20      440 2023-06-07 15:31:28.000000 oxenai-0.1.2/python/oxen/ops/extract_col.py
+-rw-r--r--   0      501       20      214 2023-05-18 05:25:22.000000 oxenai-0.1.2/python/oxen/ops/identity.py
+-rw-r--r--   0      501       20      361 2023-06-07 15:31:28.000000 oxenai-0.1.2/python/oxen/ops/read_df.py
+-rw-r--r--   0      501       20      710 2023-06-07 15:31:28.000000 oxenai-0.1.2/python/oxen/ops/read_image_dir.py
+-rw-r--r--   0      501       20      347 2023-06-07 15:31:28.000000 oxenai-0.1.2/python/oxen/ops/read_text.py
+-rw-r--r--   0      501       20      354 2023-05-18 05:25:22.000000 oxenai-0.1.2/python/oxen/ops/str_col_template.py
+-rw-r--r--   0      501       20     5494 2023-05-18 05:25:22.000000 oxenai-0.1.2/python/oxen/remote_repo.py
+-rw-r--r--   0      501       20        0 2023-05-18 05:25:22.000000 oxenai-0.1.2/python/oxen/util/__init__.py
+-rw-r--r--   0      501       20      195 2023-06-07 15:31:28.000000 oxenai-0.1.2/requirements.txt
+-rw-r--r--   0      501       20      908 2023-06-07 15:31:28.000000 oxenai-0.1.2/src/auth.rs
+-rw-r--r--   0      501       20      370 2023-05-18 05:25:22.000000 oxenai-0.1.2/src/error.rs
+-rw-r--r--   0      501       20     2105 2023-06-07 15:31:28.000000 oxenai-0.1.2/src/lib.rs
+-rw-r--r--   0      501       20      718 2023-05-18 05:25:22.000000 oxenai-0.1.2/src/py_branch.rs
+-rw-r--r--   0      501       20      291 2023-05-18 05:25:22.000000 oxenai-0.1.2/src/py_commit.rs
+-rw-r--r--   0      501       20      474 2023-05-18 05:25:22.000000 oxenai-0.1.2/src/py_dataset.rs
+-rw-r--r--   0      501       20     3875 2023-05-18 05:25:22.000000 oxenai-0.1.2/src/py_local_repo.rs
+-rw-r--r--   0      501       20     8111 2023-05-18 05:25:22.000000 oxenai-0.1.2/src/py_remote_repo.rs
+-rw-r--r--   0      501       20     1572 2023-05-18 05:25:22.000000 oxenai-0.1.2/src/py_staged_data.rs
+-rw-r--r--   0      501       20      538 2023-05-18 05:25:22.000000 oxenai-0.1.2/src/util.rs
+-rw-r--r--   0      501       20      345 2023-05-18 05:25:22.000000 oxenai-0.1.2/test.py
+-rw-r--r--   0      501       20        0 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/__init__.py
+-rw-r--r--   0      501       20     3474 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/conftest.py
+-rw-r--r--   0      501       20       18 2023-06-07 15:31:28.000000 oxenai-0.1.2/tests/data/CelebA/annotations/labels.txt
+-rw-r--r--   0      501       20       94 2023-06-07 15:31:28.000000 oxenai-0.1.2/tests/data/CelebA/annotations/test.csv
+-rw-r--r--   0      501       20      114 2023-06-07 15:31:28.000000 oxenai-0.1.2/tests/data/CelebA/annotations/train.csv
+-rw-r--r--   0      501       20    11440 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/data/CelebA/images/1.jpg
+-rw-r--r--   0      501       20     7448 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/data/CelebA/images/2.jpg
+-rw-r--r--   0      501       20     4253 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/data/CelebA/images/3.jpg
+-rw-r--r--   0      501       20    10747 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/data/CelebA/images/4.jpg
+-rw-r--r--   0      501       20     6351 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/data/CelebA/images/5.jpg
+-rw-r--r--   0      501       20     8073 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/data/CelebA/images/6.jpg
+-rw-r--r--   0      501       20     8203 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/data/CelebA/images/7.jpg
+-rw-r--r--   0      501       20     7725 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/data/CelebA/images/8.jpg
+-rw-r--r--   0      501       20     8641 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/data/CelebA/images/9.jpg
+-rw-r--r--   0      501       20      337 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/data/ChatBot/examples.tsv
+-rw-r--r--   0      501       20       88 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/data/ChatBot/prompt.txt
+-rw-r--r--   0      501       20      148 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/data/HousePrices/prices.csv
+-rw-r--r--   0      501       20      519 2023-06-07 15:31:28.000000 oxenai-0.1.2/tests/test_add.py
+-rw-r--r--   0      501       20     1706 2023-06-07 15:31:28.000000 oxenai-0.1.2/tests/test_auth.py
+-rw-r--r--   0      501       20      363 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/test_chat_loader.py
+-rw-r--r--   0      501       20     1299 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/test_checkout.py
+-rw-r--r--   0      501       20      723 2023-06-07 15:31:28.000000 oxenai-0.1.2/tests/test_clone.py
+-rw-r--r--   0      501       20      850 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/test_commit.py
+-rw-r--r--   0      501       20     2444 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/test_dataloader_pytorch.py
+-rw-r--r--   0      501       20     1506 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/test_dataset.py
+-rw-r--r--   0      501       20     2022 2023-06-07 15:31:28.000000 oxenai-0.1.2/tests/test_image_classification_loader.py
+-rw-r--r--   0      501       20      338 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/test_init.py
+-rw-r--r--   0      501       20      440 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/test_push.py
+-rw-r--r--   0      501       20      911 2023-06-07 15:31:28.000000 oxenai-0.1.2/tests/test_push_pull.py
+-rw-r--r--   0      501       20      488 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/test_regression_loader.py
+-rw-r--r--   0      501       20      828 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/test_remote_add.py
+-rw-r--r--   0      501       20      560 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/test_remote_branch.py
+-rw-r--r--   0      501       20      538 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/test_remote_checkout.py
+-rw-r--r--   0      501       20      685 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/test_remote_commit.py
+-rw-r--r--   0      501       20     1473 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/test_remote_df_add.py
+-rw-r--r--   0      501       20      530 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/test_remote_list.py
+-rw-r--r--   0      501       20      657 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/test_remote_remove.py
+-rw-r--r--   0      501       20      114 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/test_remote_repo.py
+-rw-r--r--   0      501       20      636 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/test_remote_status.py
+-rw-r--r--   0      501       20      259 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/test_status.py
+-rw-r--r--   0      501       20   109484 2023-06-07 15:47:32.000000 oxenai-0.1.2/Cargo.lock
+-rw-r--r--   0        0        0     2216 1970-01-01 00:00:00.000000 oxenai-0.1.2/PKG-INFO
```

### Comparing `oxenai-0.1.0/.github/workflows/CI.yml` & `oxenai-0.1.2/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/.gitignore` & `oxenai-0.1.2/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 *.so
 
 # Distribution / packaging
 .Python
 .venv/
 env/
 bin/
-build/
+# build/
 develop-eggs/
 dist/
 eggs/
 lib/
 lib64/
 parts/
 sdist/
```

### Comparing `oxenai-0.1.0/docs/Makefile` & `oxenai-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/docs/make.bat` & `oxenai-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/docs/source/conf.py` & `oxenai-0.1.2/docs/source/conf.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # For the full list of built-in configuration values, see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 import toml
+import sys, os
 
 with open("../../Cargo.toml") as f:
     data = toml.load(f)
 
 version = data["package"]["version"]
 
 project = "🐂 🌾 Oxen"
@@ -32,17 +33,18 @@
     "sphinx.ext.autosummary",
     "sphinx.ext.napoleon",
 ]
 
 templates_path = ["_templates"]
 exclude_patterns = []
 
+copybutton_prompt_text = "$ "
 
 source_suffix = [".md", ".rst"]
 
 m2r_parse_relative_links = True
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
 html_theme = "sphinx_book_theme"
-html_static_path = ["_static"]
+# html_static_path = ["_static"]
```

### Comparing `oxenai-0.1.0/docs/source/getting_started/installation.md` & `oxenai-0.1.2/docs/build/html/_sources/getting_started/installation.md`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/docs/source/getting_started/python.md` & `oxenai-0.1.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-# Python
+# 🐂 🐍 Oxen Python Interface 
 
 The Oxen python interface makes it easy to integrate Oxen datasets directly into machine learning dataloaders or other data pipelines.
 
 ## Repositories
 
 There are two types of repositories one can interact with, a `LocalRepo` and a `RemoteRepo`.
 
 
-### Local Repo
+## Local Repo
 
 To fully clone all the data to your local machine, you can use the `LocalRepo` class.
 
 ```python
 import oxen
 
 repo = LocalRepo("path/to/repository")
@@ -30,8 +30,35 @@
 
 ```python
 import oxen
 
 repo = LocalRepo("path/to/repository")
 repo.clone("https://hub.oxen.ai/ox/CatDogBBox")
 repo.checkout()
-```
+```
+
+## Remote Repo
+
+If you don't want to download the data locally, you can use the `RemoteRepo` class to interact with a remote repository on OxenHub.
+
+```python
+import oxen 
+
+repo = RemoteRepo("https://hub.oxen.ai/ox/CatDogBBox")
+```
+
+To stage and commit files to a specific version of the data, you can `checkout` an existing branch or create a new one.
+
+```python
+repo.create_branch("dev")
+repo.checkout("dev")
+```
+
+You can then stage files to the remote repository by specifying the file path and destination directory.
+
+```python
+repo.add("new-cat.png", "images") # Stage to images/new-cat.png on remote
+repo.commit("Adding another training image")
+```
+
+Note that no "push" command is required here, since the above code creates a commit directly on the remote branch.
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `oxenai-0.1.0/python/oxen/__init__.py` & `oxenai-0.1.2/python/oxen/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,22 +6,24 @@
 
 # Python classes
 from oxen.dataset import Dataset
 from oxen.local_repo import LocalRepo
 from oxen.remote_repo import RemoteRepo
 from oxen.dag import DAG
 from oxen.op import Op
+from oxen import auth
 
 # Names of public modules we want to expose
 __all__ = [
     "Dataset",
     "DAG",
     "PyCommit",
     "PyDataset",
     "PyRemoteRepo",
     "PyLocalRepo",
     "PyStagedData",
     "Op",
     "RemoteRepo",
     "LocalRepo",
     "util",
+    "auth"
 ]
```

### Comparing `oxenai-0.1.0/python/oxen/dataset.py` & `oxenai-0.1.2/python/oxen/dataset.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/python/oxen/features.py` & `oxenai-0.1.2/python/oxen/features.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/python/oxen/loaders/chat.py` & `oxenai-0.1.2/python/oxen/loaders/chat.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/python/oxen/loaders/regression.py` & `oxenai-0.1.2/python/oxen/loaders/regression.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/python/oxen/local_repo.py` & `oxenai-0.1.2/python/oxen/local_repo.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/python/oxen/op.py` & `oxenai-0.1.2/python/oxen/op.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,15 @@
+import uuid
+
+
 class Op:
     def __init__(self, *args, **kwargs):
         self.args = args
         self.kwargs = kwargs
+        self.id = uuid.uuid4()
         self.input = None
         self.name = self.__class__.__name__
 
         if "name" in kwargs:
             self.name = kwargs["name"]
 
         if "input" in kwargs:
```

### Comparing `oxenai-0.1.0/python/oxen/remote_repo.py` & `oxenai-0.1.2/python/oxen/remote_repo.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/python/oxen/util/fs.py` & `oxenai-0.1.2/python/oxen/fs.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/src/lib.rs` & `oxenai-0.1.2/src/lib.rs`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 use pyo3::prelude::*;
 
 pub mod error;
 pub mod py_branch;
 
+pub mod auth;
 pub mod py_commit;
 pub mod py_dataset;
 pub mod py_local_repo;
 pub mod py_remote_repo;
 pub mod py_staged_data;
 pub mod util;
 
@@ -41,9 +42,15 @@
 
     // Util Module
     let util_module = PyModule::new(py, "util")?;
     util_module.add_function(wrap_pyfunction!(util::is_tabular, util_module)?)?;
     util_module.add_function(wrap_pyfunction!(util::read_df, util_module)?)?;
     m.add_submodule(util_module)?;
 
+    // Auth Module
+    let auth_module = PyModule::new(py, "auth")?;
+    auth_module.add_function(wrap_pyfunction!(auth::get_oxen_home_dir, auth_module)?)?;
+    auth_module.add_function(wrap_pyfunction!(auth::add_host_auth, auth_module)?)?;
+    auth_module.add_function(wrap_pyfunction!(auth::create_user_config, auth_module)?)?;
+    m.add_submodule(auth_module)?;
     Ok(())
 }
```

### Comparing `oxenai-0.1.0/src/py_branch.rs` & `oxenai-0.1.2/src/py_branch.rs`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/src/py_local_repo.rs` & `oxenai-0.1.2/src/py_local_repo.rs`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/src/py_remote_repo.rs` & `oxenai-0.1.2/src/py_remote_repo.rs`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/src/py_staged_data.rs` & `oxenai-0.1.2/src/py_staged_data.rs`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/src/util.rs` & `oxenai-0.1.2/src/util.rs`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/tests/conftest.py` & `oxenai-0.1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/tests/data/CelebA/images/1.jpg` & `oxenai-0.1.2/tests/data/CelebA/images/1.jpg`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/tests/data/CelebA/images/2.jpg` & `oxenai-0.1.2/tests/data/CelebA/images/2.jpg`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/tests/data/CelebA/images/3.jpg` & `oxenai-0.1.2/tests/data/CelebA/images/3.jpg`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/tests/data/CelebA/images/4.jpg` & `oxenai-0.1.2/tests/data/CelebA/images/4.jpg`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/tests/data/CelebA/images/5.jpg` & `oxenai-0.1.2/tests/data/CelebA/images/5.jpg`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/tests/data/CelebA/images/6.jpg` & `oxenai-0.1.2/tests/data/CelebA/images/6.jpg`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/tests/data/CelebA/images/7.jpg` & `oxenai-0.1.2/tests/data/CelebA/images/7.jpg`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/tests/data/CelebA/images/8.jpg` & `oxenai-0.1.2/tests/data/CelebA/images/8.jpg`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/tests/data/CelebA/images/9.jpg` & `oxenai-0.1.2/tests/data/CelebA/images/9.jpg`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/tests/test_checkout.py` & `oxenai-0.1.2/tests/test_checkout.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/tests/test_clone.py` & `oxenai-0.1.2/tests/test_clone.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from oxen import LocalRepo
-from oxen.util.fs import rcount_files_in_repo
+import oxen
+from oxen.fs import rcount_files_in_repo
 
 
 def test_repo_clone(celeba_remote_repo_fully_pushed, empty_local_dir):
     # og_local_repo is the original local repo
     # then we pushed to the remote repo
     og_local_repo, remote_repo = celeba_remote_repo_fully_pushed
```

### Comparing `oxenai-0.1.0/tests/test_commit.py` & `oxenai-0.1.2/tests/test_commit.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/tests/test_dataloader_pytorch.py` & `oxenai-0.1.2/tests/test_dataloader_pytorch.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/tests/test_dataset.py` & `oxenai-0.1.2/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/tests/test_push_pull.py` & `oxenai-0.1.2/tests/test_push_pull.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pytest
 
 from oxen import LocalRepo
-from oxen.util.fs import rcount_files_in_repo_dir
+from oxen.fs import rcount_files_in_repo_dir
 
 # Alias the fixtures just to make it a little easier to read
 @pytest.fixture
 def local_repo(celeba_local_repo_one_image_committed):
     yield celeba_local_repo_one_image_committed
```

### Comparing `oxenai-0.1.0/tests/test_remote_add.py` & `oxenai-0.1.2/tests/test_remote_add.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/tests/test_remote_branch.py` & `oxenai-0.1.2/tests/test_remote_branch.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/tests/test_remote_checkout.py` & `oxenai-0.1.2/tests/test_remote_checkout.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/tests/test_remote_commit.py` & `oxenai-0.1.2/tests/test_remote_commit.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/tests/test_remote_df_add.py` & `oxenai-0.1.2/tests/test_remote_df_add.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/tests/test_remote_list.py` & `oxenai-0.1.2/tests/test_remote_list.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/tests/test_remote_remove.py` & `oxenai-0.1.2/tests/test_remote_remove.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/tests/test_remote_status.py` & `oxenai-0.1.2/tests/test_remote_status.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.0/Cargo.lock` & `oxenai-0.1.2/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -381,17 +381,17 @@
 dependencies = [
  "planus",
  "serde",
 ]
 
 [[package]]
 name = "arrow2"
-version = "0.17.0"
+version = "0.17.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c3c63cf31f1416ed2fab8f91e8488e10129f47bd89c553ec354a06751d5697f3"
+checksum = "15ae0428d69ab31d7b2adad22a752d6f11fef2e901d2262d0cad4f5cb08b7093"
 dependencies = [
  "ahash 0.8.3",
  "arrow-format",
  "base64",
  "bytemuck",
  "chrono",
  "dyn-clone",
@@ -1618,17 +1618,17 @@
  "tokio",
  "tokio-util",
  "tracing",
 ]
 
 [[package]]
 name = "halfbrown"
-version = "0.2.1"
+version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6d9ab7d9233262d3b74ae4c4a7a090fc4379b07c6eb9b02ecab7cbb12ad67a58"
+checksum = "f985624e90f861184145c13b736873a0f83cdb998a292dbb0653598ab03aecbf"
 dependencies = [
  "hashbrown 0.13.2",
  "rustc-hash",
  "serde",
 ]
 
 [[package]]
@@ -2064,17 +2064,17 @@
 name = "libm"
 version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "348108ab3fba42ec82ff6e9564fc4ca0247bdccdc68dd8af9764bbc79c3c8ffb"
 
 [[package]]
 name = "liboxen"
-version = "0.6.0+2"
+version = "0.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99a8965fe6a2f1fe992daba715602de64fddb7062b7a9c60bad80573e297219d"
+checksum = "287c6c8c83b21baaed2f81d33674db345e29ed9bde621759f1fa6b675aee81a4"
 dependencies = [
  "actix-files",
  "actix-web",
  "async-compression 0.4.0",
  "async-recursion",
  "async-std",
  "async-tar",
@@ -2461,15 +2461,15 @@
 name = "option-ext"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "04744f49eae99ab78e0d5c0b603ab218f515ea8cfe5a456d7629ad883a3b6e7d"
 
 [[package]]
 name = "oxen"
-version = "0.1.0"
+version = "0.1.2"
 dependencies = [
  "liboxen",
  "log",
  "pyo3",
  "pyo3-asyncio",
  "pyo3-log",
  "pyo3-polars",
@@ -4046,17 +4046,17 @@
 dependencies = [
  "ctor",
  "version_check",
 ]
 
 [[package]]
 name = "value-trait"
-version = "0.6.0"
+version = "0.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "733e1909354ceff16f7e1f7ddebc063455b8fda4968d91760a7c6115b96647a5"
+checksum = "09a5b6c8ceb01263b969cac48d4a6705134d490ded13d889e52c0cfc80c6945e"
 dependencies = [
  "float-cmp",
  "halfbrown",
  "itoa",
  "ryu",
 ]
```

