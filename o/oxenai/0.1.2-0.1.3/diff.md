# Comparing `tmp/oxenai-0.1.2.tar.gz` & `tmp/oxenai-0.1.3.tar.gz`

## Comparing `oxenai-0.1.2.tar` & `oxenai-0.1.3.tar`

### file list

```diff
@@ -1,239 +1,239 @@
--rw-r--r--   0        0        0      432 1970-01-01 00:00:00.000000 oxenai-0.1.2/Cargo.toml
--rw-r--r--   0      501       20     2809 2023-05-18 05:25:22.000000 oxenai-0.1.2/.github/workflows/CI.yml
--rw-r--r--   0      501       20      687 2023-05-18 16:10:10.000000 oxenai-0.1.2/.gitignore
--rw-r--r--   0      501       20     1255 2023-06-07 15:31:28.000000 oxenai-0.1.2/Develop.md
--rw-r--r--   0      501       20     1840 2023-06-07 15:31:28.000000 oxenai-0.1.2/README.md
--rw-r--r--   0      501       20      638 2023-05-18 05:25:22.000000 oxenai-0.1.2/docs/Makefile
--rw-r--r--   0      501       20   111104 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/doctrees/concepts/data_frames.doctree
--rw-r--r--   0      501       20     2426 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/doctrees/concepts/embedding_search.doctree
--rw-r--r--   0      501       20    33060 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/doctrees/concepts/remote_staging.doctree
--rw-r--r--   0      501       20     4832 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/doctrees/contributing/documentation.doctree
--rw-r--r--   0      501       20     3114 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/doctrees/contributing/python.doctree
--rw-r--r--   0      501       20     3041 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/doctrees/contributing/rust.doctree
--rw-r--r--   0      501       20   521114 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/doctrees/environment.pickle
--rw-r--r--   0      501       20     4632 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/doctrees/getting_started/commands.doctree
--rw-r--r--   0      501       20    13327 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/doctrees/getting_started/installation.doctree
--rw-r--r--   0      501       20     8868 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/doctrees/getting_started/python.doctree
--rw-r--r--   0      501       20     2515 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/doctrees/getting_started/tutorials.doctree
--rw-r--r--   0      501       20    92642 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/doctrees/index.doctree
--rw-r--r--   0      501       20    41036 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/doctrees/references/python/local_repo.doctree
--rw-r--r--   0      501       20    54552 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/doctrees/references/python/remote_repo.doctree
--rw-r--r--   0      501       20     3870 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/doctrees/references/rust.doctree
--rw-r--r--   0      501       20      230 2023-05-30 22:47:04.000000 oxenai-0.1.2/docs/build/html/.buildinfo
--rw-r--r--   0      501       20    45695 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/html/_sources/concepts/data_frames.md
--rw-r--r--   0      501       20       18 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/html/_sources/concepts/embedding_search.md
--rw-r--r--   0      501       20    10491 2023-05-30 22:47:04.000000 oxenai-0.1.2/docs/build/html/_sources/concepts/remote_staging.md
--rw-r--r--   0      501       20      435 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/html/_sources/contributing/documentation.md
--rw-r--r--   0      501       20      165 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/html/_sources/contributing/python.md
--rw-r--r--   0      501       20      135 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/html/_sources/contributing/rust.md
--rw-r--r--   0      501       20      435 2023-05-17 22:27:30.000000 oxenai-0.1.2/docs/build/html/_sources/getting_started/commands.md
--rw-r--r--   0      501       20     2148 2023-05-18 04:14:06.000000 oxenai-0.1.2/docs/build/html/_sources/getting_started/installation.md
--rw-r--r--   0      501       20     1816 2023-05-30 22:47:04.000000 oxenai-0.1.2/docs/build/html/_sources/getting_started/python.md
--rw-r--r--   0      501       20       18 2023-05-17 00:07:17.000000 oxenai-0.1.2/docs/build/html/_sources/getting_started/tutorials.md
--rw-r--r--   0      501       20     1130 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/html/_sources/index.rst
--rw-r--r--   0      501       20       69 2023-05-18 03:59:38.000000 oxenai-0.1.2/docs/build/html/_sources/references/python/local_repo.rst
--rw-r--r--   0      501       20       68 2023-05-18 04:14:40.000000 oxenai-0.1.2/docs/build/html/_sources/references/python/remote_repo.rst
--rw-r--r--   0      501       20      235 2023-05-18 04:22:39.000000 oxenai-0.1.2/docs/build/html/_sources/references/rust.md
--rw-r--r--   0      501       20    14813 2023-05-24 22:24:23.000000 oxenai-0.1.2/docs/build/html/_static/basic.css
--rw-r--r--   0      501       20      313 2023-05-16 23:41:23.000000 oxenai-0.1.2/docs/build/html/_static/check-solid.svg
--rw-r--r--   0      501       20     9031 2023-05-16 23:41:23.000000 oxenai-0.1.2/docs/build/html/_static/clipboard.min.js
--rw-r--r--   0      501       20      411 2023-05-16 23:41:23.000000 oxenai-0.1.2/docs/build/html/_static/copy-button.svg
--rw-r--r--   0      501       20     2060 2023-05-16 23:41:23.000000 oxenai-0.1.2/docs/build/html/_static/copybutton.css
--rw-r--r--   0      501       20     8469 2023-05-30 22:47:04.000000 oxenai-0.1.2/docs/build/html/_static/copybutton.js
--rw-r--r--   0      501       20     2698 2023-05-16 23:41:23.000000 oxenai-0.1.2/docs/build/html/_static/copybutton_funcs.js
--rw-r--r--   0      501       20     4472 2023-05-16 20:00:40.000000 oxenai-0.1.2/docs/build/html/_static/doctools.js
--rw-r--r--   0      501       20      415 2023-05-24 22:24:23.000000 oxenai-0.1.2/docs/build/html/_static/documentation_options.js
--rw-r--r--   0      501       20      286 2023-05-16 20:00:40.000000 oxenai-0.1.2/docs/build/html/_static/file.png
--rw-r--r--   0      501       20     1186 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/images/logo_binder.svg
--rw-r--r--   0      501       20     7601 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/images/logo_colab.png
--rw-r--r--   0      501       20      681 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/images/logo_deepnote.svg
--rw-r--r--   0      501       20     1758 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/images/logo_jupyterhub.svg
--rw-r--r--   0      501       20     4758 2023-05-24 22:24:23.000000 oxenai-0.1.2/docs/build/html/_static/language_data.js
--rw-r--r--   0      501       20     1459 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/ar/LC_MESSAGES/booktheme.po
--rw-r--r--   0      501       20     1626 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/bg/LC_MESSAGES/booktheme.po
--rw-r--r--   0      501       20     1564 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/bn/LC_MESSAGES/booktheme.po
--rw-r--r--   0      501       20     1166 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/ca/LC_MESSAGES/booktheme.po
--rw-r--r--   0      501       20     1323 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/cs/LC_MESSAGES/booktheme.po
--rw-r--r--   0      501       20     1222 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/da/LC_MESSAGES/booktheme.po
--rw-r--r--   0      501       20     1306 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/de/LC_MESSAGES/booktheme.po
--rw-r--r--   0      501       20     1640 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/el/LC_MESSAGES/booktheme.po
--rw-r--r--   0      501       20     1255 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/eo/LC_MESSAGES/booktheme.po
--rw-r--r--   0      501       20     1314 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/es/LC_MESSAGES/booktheme.po
--rw-r--r--   0      501       20     1259 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/et/LC_MESSAGES/booktheme.po
--rw-r--r--   0      501       20     1286 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/fi/LC_MESSAGES/booktheme.po
--rw-r--r--   0      501       20     1330 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/fr/LC_MESSAGES/booktheme.po
--rw-r--r--   0      501       20     1320 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/hr/LC_MESSAGES/booktheme.po
--rw-r--r--   0      501       20     1241 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/id/LC_MESSAGES/booktheme.po
--rw-r--r--   0      501       20     1321 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/it/LC_MESSAGES/booktheme.po
--rw-r--r--   0      501       20     1363 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/iw/LC_MESSAGES/booktheme.po
--rw-r--r--   0      501       20     1389 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/ja/LC_MESSAGES/booktheme.po
--rw-r--r--   0      501       20     1293 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/ko/LC_MESSAGES/booktheme.po
--rw-r--r--   0      501       20     1331 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/lt/LC_MESSAGES/booktheme.po
--rw-r--r--   0      501       20     1322 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/lv/LC_MESSAGES/booktheme.po
--rw-r--r--   0      501       20     1803 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/ml/LC_MESSAGES/booktheme.po
--rw-r--r--   0      501       20     1594 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/mr/LC_MESSAGES/booktheme.po
--rw-r--r--   0      501       20     1133 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/ms/LC_MESSAGES/booktheme.po
--rw-r--r--   0      501       20     1274 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/nl/LC_MESSAGES/booktheme.po
--rw-r--r--   0      501       20     1235 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/no/LC_MESSAGES/booktheme.po
--rw-r--r--   0      501       20     1289 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/pl/LC_MESSAGES/booktheme.po
--rw-r--r--   0      501       20     1282 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/pt/LC_MESSAGES/booktheme.po
--rw-r--r--   0      501       20     1308 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/ro/LC_MESSAGES/booktheme.po
--rw-r--r--   0      501       20     1640 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/ru/LC_MESSAGES/booktheme.po
--rw-r--r--   0      501       20     1311 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/sk/LC_MESSAGES/booktheme.po
--rw-r--r--   0      501       20     1292 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/sl/LC_MESSAGES/booktheme.po
--rw-r--r--   0      501       20     1597 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/sr/LC_MESSAGES/booktheme.po
--rw-r--r--   0      501       20     1267 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/sv/LC_MESSAGES/booktheme.po
--rw-r--r--   0      501       20     1848 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/ta/LC_MESSAGES/booktheme.po
--rw-r--r--   0      501       20     1726 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/te/LC_MESSAGES/booktheme.po
--rw-r--r--   0      501       20     1546 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/tg/LC_MESSAGES/booktheme.po
--rw-r--r--   0      501       20     1684 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/th/LC_MESSAGES/booktheme.po
--rw-r--r--   0      501       20     1193 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/tl/LC_MESSAGES/booktheme.po
--rw-r--r--   0      501       20     1291 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/tr/LC_MESSAGES/booktheme.po
--rw-r--r--   0      501       20     1601 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/uk/LC_MESSAGES/booktheme.po
--rw-r--r--   0      501       20     1382 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/ur/LC_MESSAGES/booktheme.po
--rw-r--r--   0      501       20     1349 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/vi/LC_MESSAGES/booktheme.po
--rw-r--r--   0      501       20     1228 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po
--rw-r--r--   0      501       20     1259 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po
--rw-r--r--   0      501       20       90 2023-05-16 20:00:40.000000 oxenai-0.1.2/docs/build/html/_static/minus.png
--rw-r--r--   0      501       20       90 2023-05-16 20:00:40.000000 oxenai-0.1.2/docs/build/html/_static/plus.png
--rw-r--r--   0      501       20    12757 2023-05-24 22:24:23.000000 oxenai-0.1.2/docs/build/html/_static/pygments.css
--rw-r--r--   0      501       20      419 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/sbt-webpack-macros.html
--rw-r--r--   0      501       20    80813 2023-05-16 20:04:17.000000 oxenai-0.1.2/docs/build/html/_static/scripts/bootstrap.js
--rw-r--r--   0      501       20      237 2023-05-16 20:04:17.000000 oxenai-0.1.2/docs/build/html/_static/scripts/bootstrap.js.LICENSE.txt
--rw-r--r--   0      501       20   335757 2023-05-16 20:04:17.000000 oxenai-0.1.2/docs/build/html/_static/scripts/bootstrap.js.map
--rw-r--r--   0      501       20     4456 2023-05-16 20:04:17.000000 oxenai-0.1.2/docs/build/html/_static/scripts/pydata-sphinx-theme.js
--rw-r--r--   0      501       20    19648 2023-05-16 20:04:17.000000 oxenai-0.1.2/docs/build/html/_static/scripts/pydata-sphinx-theme.js.map
--rw-r--r--   0      501       20     3075 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/scripts/sphinx-book-theme.js
--rw-r--r--   0      501       20    13066 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/scripts/sphinx-book-theme.js.map
--rw-r--r--   0      501       20    18215 2023-05-16 20:00:40.000000 oxenai-0.1.2/docs/build/html/_static/searchtools.js
--rw-r--r--   0      501       20     4712 2023-05-16 20:00:40.000000 oxenai-0.1.2/docs/build/html/_static/sphinx_highlight.js
--rw-r--r--   0      501       20   176654 2023-05-16 20:04:17.000000 oxenai-0.1.2/docs/build/html/_static/styles/bootstrap.css
--rw-r--r--   0      501       20    63341 2023-05-16 20:04:17.000000 oxenai-0.1.2/docs/build/html/_static/styles/pydata-sphinx-theme.css
--rw-r--r--   0      501       20    13841 2023-05-17 00:03:57.000000 oxenai-0.1.2/docs/build/html/_static/styles/sphinx-book-theme.css
--rw-r--r--   0      501       20      106 2023-05-16 20:04:17.000000 oxenai-0.1.2/docs/build/html/_static/styles/theme.css
--rw-r--r--   0      501       20     7427 2023-05-16 20:04:17.000000 oxenai-0.1.2/docs/build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt
--rw-r--r--   0      501       20   101691 2023-05-16 20:04:17.000000 oxenai-0.1.2/docs/build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css
--rw-r--r--   0      501       20   181264 2023-05-16 20:04:17.000000 oxenai-0.1.2/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf
--rw-r--r--   0      501       20   105112 2023-05-16 20:04:17.000000 oxenai-0.1.2/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2
--rw-r--r--   0      501       20    60236 2023-05-16 20:04:17.000000 oxenai-0.1.2/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf
--rw-r--r--   0      501       20    24028 2023-05-16 20:04:17.000000 oxenai-0.1.2/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2
--rw-r--r--   0      501       20   389948 2023-05-16 20:04:17.000000 oxenai-0.1.2/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf
--rw-r--r--   0      501       20   154840 2023-05-16 20:04:17.000000 oxenai-0.1.2/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2
--rw-r--r--   0      501       20    10084 2023-05-16 20:04:17.000000 oxenai-0.1.2/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0      501       20     4776 2023-05-16 20:04:17.000000 oxenai-0.1.2/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2
--rw-r--r--   0      501       20     1863 2023-05-16 20:04:17.000000 oxenai-0.1.2/docs/build/html/_static/webpack-macros.html
--rw-r--r--   0      501       20    94792 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/html/concepts/data_frames.html
--rw-r--r--   0      501       20    12188 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/html/concepts/embedding_search.html
--rw-r--r--   0      501       20    41523 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/html/concepts/remote_staging.html
--rw-r--r--   0      501       20    13736 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/html/contributing/documentation.html
--rw-r--r--   0      501       20    14226 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/html/contributing/python.html
--rw-r--r--   0      501       20    13585 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/html/contributing/rust.html
--rw-r--r--   0      501       20    17490 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/html/genindex.html
--rw-r--r--   0      501       20    14743 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/html/getting_started/commands.html
--rw-r--r--   0      501       20    21507 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/html/getting_started/installation.html
--rw-r--r--   0      501       20    18772 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/html/getting_started/python.html
--rw-r--r--   0      501       20    12068 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/html/getting_started/tutorials.html
--rw-r--r--   0      501       20    72087 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/html/index.html
--rw-r--r--   0      501       20      888 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/html/objects.inv
--rw-r--r--   0      501       20    29798 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/html/references/python/local_repo.html
--rw-r--r--   0      501       20    36459 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/html/references/python/remote_repo.html
--rw-r--r--   0      501       20    13229 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/html/references/rust.html
--rw-r--r--   0      501       20    11383 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/html/search.html
--rw-r--r--   0      501       20    23670 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/build/html/searchindex.js
--rw-r--r--   0      501       20       99 2023-05-30 22:47:04.000000 oxenai-0.1.2/docs/docsenv/pyvenv.cfg
--rw-r--r--   0      501       20      804 2023-05-18 05:25:22.000000 oxenai-0.1.2/docs/make.bat
--rw-r--r--   0      501       20      131 2023-06-07 15:47:27.000000 oxenai-0.1.2/docs/requirements.txt
--rw-r--r--   0      501       20    45695 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/source/concepts/data_frames.md
--rw-r--r--   0      501       20       24 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/source/concepts/embedding_search.md
--rw-r--r--   0      501       20    10491 2023-05-30 22:47:04.000000 oxenai-0.1.2/docs/source/concepts/remote_staging.md
--rw-r--r--   0      501       20     1395 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/source/conf.py
--rw-r--r--   0      501       20      435 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/source/contributing/documentation.md
--rw-r--r--   0      501       20      165 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/source/contributing/python.md
--rw-r--r--   0      501       20      135 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/source/contributing/rust.md
--rw-r--r--   0      501       20      435 2023-05-18 05:25:22.000000 oxenai-0.1.2/docs/source/getting_started/commands.md
--rw-r--r--   0      501       20     2148 2023-05-18 05:25:22.000000 oxenai-0.1.2/docs/source/getting_started/installation.md
--rw-r--r--   0      501       20     1816 2023-05-30 22:47:04.000000 oxenai-0.1.2/docs/source/getting_started/python.md
--rw-r--r--   0      501       20       18 2023-05-18 05:25:22.000000 oxenai-0.1.2/docs/source/getting_started/tutorials.md
--rw-r--r--   0      501       20     1130 2023-06-07 15:31:28.000000 oxenai-0.1.2/docs/source/index.rst
--rw-r--r--   0      501       20       69 2023-05-18 05:25:22.000000 oxenai-0.1.2/docs/source/references/python/local_repo.rst
--rw-r--r--   0      501       20       68 2023-05-18 05:25:22.000000 oxenai-0.1.2/docs/source/references/python/remote_repo.rst
--rw-r--r--   0      501       20      235 2023-05-18 05:25:22.000000 oxenai-0.1.2/docs/source/references/rust.md
--rw-r--r--   0      501       20      451 2023-05-18 05:25:22.000000 oxenai-0.1.2/pyproject.toml
--rw-r--r--   0      501       20      593 2023-06-07 15:31:28.000000 oxenai-0.1.2/python/oxen/__init__.py
--rw-r--r--   0      501       20      597 2023-06-07 15:31:28.000000 oxenai-0.1.2/python/oxen/auth.py
--rw-r--r--   0      501       20      746 2023-06-07 15:31:28.000000 oxenai-0.1.2/python/oxen/dag.py
--rw-r--r--   0      501       20     5995 2023-05-18 05:25:22.000000 oxenai-0.1.2/python/oxen/dataset.py
--rw-r--r--   0      501       20     1378 2023-05-18 05:25:22.000000 oxenai-0.1.2/python/oxen/features.py
--rw-r--r--   0      501       20     1500 2023-06-07 15:31:28.000000 oxenai-0.1.2/python/oxen/fs.py
--rw-r--r--   0      501       20      259 2023-06-07 15:31:28.000000 oxenai-0.1.2/python/oxen/loaders/__init__.py
--rw-r--r--   0      501       20     1057 2023-05-18 05:25:22.000000 oxenai-0.1.2/python/oxen/loaders/chat.py
--rw-r--r--   0      501       20     1159 2023-06-07 15:31:28.000000 oxenai-0.1.2/python/oxen/loaders/image_classification.py
--rw-r--r--   0      501       20      802 2023-05-18 05:25:22.000000 oxenai-0.1.2/python/oxen/loaders/regression.py
--rw-r--r--   0      501       20     3732 2023-05-18 05:25:22.000000 oxenai-0.1.2/python/oxen/local_repo.py
--rw-r--r--   0      501       20     1543 2023-06-07 15:31:28.000000 oxenai-0.1.2/python/oxen/op.py
--rw-r--r--   0      501       20      578 2023-06-07 15:31:28.000000 oxenai-0.1.2/python/oxen/ops/__init__.py
--rw-r--r--   0      501       20      207 2023-05-18 05:25:22.000000 oxenai-0.1.2/python/oxen/ops/concat_series.py
--rw-r--r--   0      501       20      876 2023-06-07 15:31:28.000000 oxenai-0.1.2/python/oxen/ops/create_label_map.py
--rw-r--r--   0      501       20      493 2023-06-07 15:31:28.000000 oxenai-0.1.2/python/oxen/ops/encode_labels.py
--rw-r--r--   0      501       20      440 2023-06-07 15:31:28.000000 oxenai-0.1.2/python/oxen/ops/extract_col.py
--rw-r--r--   0      501       20      214 2023-05-18 05:25:22.000000 oxenai-0.1.2/python/oxen/ops/identity.py
--rw-r--r--   0      501       20      361 2023-06-07 15:31:28.000000 oxenai-0.1.2/python/oxen/ops/read_df.py
--rw-r--r--   0      501       20      710 2023-06-07 15:31:28.000000 oxenai-0.1.2/python/oxen/ops/read_image_dir.py
--rw-r--r--   0      501       20      347 2023-06-07 15:31:28.000000 oxenai-0.1.2/python/oxen/ops/read_text.py
--rw-r--r--   0      501       20      354 2023-05-18 05:25:22.000000 oxenai-0.1.2/python/oxen/ops/str_col_template.py
--rw-r--r--   0      501       20     5494 2023-05-18 05:25:22.000000 oxenai-0.1.2/python/oxen/remote_repo.py
--rw-r--r--   0      501       20        0 2023-05-18 05:25:22.000000 oxenai-0.1.2/python/oxen/util/__init__.py
--rw-r--r--   0      501       20      195 2023-06-07 15:31:28.000000 oxenai-0.1.2/requirements.txt
--rw-r--r--   0      501       20      908 2023-06-07 15:31:28.000000 oxenai-0.1.2/src/auth.rs
--rw-r--r--   0      501       20      370 2023-05-18 05:25:22.000000 oxenai-0.1.2/src/error.rs
--rw-r--r--   0      501       20     2105 2023-06-07 15:31:28.000000 oxenai-0.1.2/src/lib.rs
--rw-r--r--   0      501       20      718 2023-05-18 05:25:22.000000 oxenai-0.1.2/src/py_branch.rs
--rw-r--r--   0      501       20      291 2023-05-18 05:25:22.000000 oxenai-0.1.2/src/py_commit.rs
--rw-r--r--   0      501       20      474 2023-05-18 05:25:22.000000 oxenai-0.1.2/src/py_dataset.rs
--rw-r--r--   0      501       20     3875 2023-05-18 05:25:22.000000 oxenai-0.1.2/src/py_local_repo.rs
--rw-r--r--   0      501       20     8111 2023-05-18 05:25:22.000000 oxenai-0.1.2/src/py_remote_repo.rs
--rw-r--r--   0      501       20     1572 2023-05-18 05:25:22.000000 oxenai-0.1.2/src/py_staged_data.rs
--rw-r--r--   0      501       20      538 2023-05-18 05:25:22.000000 oxenai-0.1.2/src/util.rs
--rw-r--r--   0      501       20      345 2023-05-18 05:25:22.000000 oxenai-0.1.2/test.py
--rw-r--r--   0      501       20        0 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/__init__.py
--rw-r--r--   0      501       20     3474 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/conftest.py
--rw-r--r--   0      501       20       18 2023-06-07 15:31:28.000000 oxenai-0.1.2/tests/data/CelebA/annotations/labels.txt
--rw-r--r--   0      501       20       94 2023-06-07 15:31:28.000000 oxenai-0.1.2/tests/data/CelebA/annotations/test.csv
--rw-r--r--   0      501       20      114 2023-06-07 15:31:28.000000 oxenai-0.1.2/tests/data/CelebA/annotations/train.csv
--rw-r--r--   0      501       20    11440 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/data/CelebA/images/1.jpg
--rw-r--r--   0      501       20     7448 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/data/CelebA/images/2.jpg
--rw-r--r--   0      501       20     4253 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/data/CelebA/images/3.jpg
--rw-r--r--   0      501       20    10747 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/data/CelebA/images/4.jpg
--rw-r--r--   0      501       20     6351 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/data/CelebA/images/5.jpg
--rw-r--r--   0      501       20     8073 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/data/CelebA/images/6.jpg
--rw-r--r--   0      501       20     8203 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/data/CelebA/images/7.jpg
--rw-r--r--   0      501       20     7725 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/data/CelebA/images/8.jpg
--rw-r--r--   0      501       20     8641 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/data/CelebA/images/9.jpg
--rw-r--r--   0      501       20      337 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/data/ChatBot/examples.tsv
--rw-r--r--   0      501       20       88 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/data/ChatBot/prompt.txt
--rw-r--r--   0      501       20      148 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/data/HousePrices/prices.csv
--rw-r--r--   0      501       20      519 2023-06-07 15:31:28.000000 oxenai-0.1.2/tests/test_add.py
--rw-r--r--   0      501       20     1706 2023-06-07 15:31:28.000000 oxenai-0.1.2/tests/test_auth.py
--rw-r--r--   0      501       20      363 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/test_chat_loader.py
--rw-r--r--   0      501       20     1299 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/test_checkout.py
--rw-r--r--   0      501       20      723 2023-06-07 15:31:28.000000 oxenai-0.1.2/tests/test_clone.py
--rw-r--r--   0      501       20      850 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/test_commit.py
--rw-r--r--   0      501       20     2444 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/test_dataloader_pytorch.py
--rw-r--r--   0      501       20     1506 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/test_dataset.py
--rw-r--r--   0      501       20     2022 2023-06-07 15:31:28.000000 oxenai-0.1.2/tests/test_image_classification_loader.py
--rw-r--r--   0      501       20      338 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/test_init.py
--rw-r--r--   0      501       20      440 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/test_push.py
--rw-r--r--   0      501       20      911 2023-06-07 15:31:28.000000 oxenai-0.1.2/tests/test_push_pull.py
--rw-r--r--   0      501       20      488 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/test_regression_loader.py
--rw-r--r--   0      501       20      828 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/test_remote_add.py
--rw-r--r--   0      501       20      560 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/test_remote_branch.py
--rw-r--r--   0      501       20      538 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/test_remote_checkout.py
--rw-r--r--   0      501       20      685 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/test_remote_commit.py
--rw-r--r--   0      501       20     1473 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/test_remote_df_add.py
--rw-r--r--   0      501       20      530 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/test_remote_list.py
--rw-r--r--   0      501       20      657 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/test_remote_remove.py
--rw-r--r--   0      501       20      114 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/test_remote_repo.py
--rw-r--r--   0      501       20      636 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/test_remote_status.py
--rw-r--r--   0      501       20      259 2023-05-18 05:25:22.000000 oxenai-0.1.2/tests/test_status.py
--rw-r--r--   0      501       20   109484 2023-06-07 15:47:32.000000 oxenai-0.1.2/Cargo.lock
--rw-r--r--   0        0        0     2216 1970-01-01 00:00:00.000000 oxenai-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      432 1970-01-01 00:00:00.000000 oxenai-0.1.3/Cargo.toml
+-rw-r--r--   0      501       20     2809 2023-05-18 05:25:22.000000 oxenai-0.1.3/.github/workflows/CI.yml
+-rw-r--r--   0      501       20      687 2023-05-18 16:10:10.000000 oxenai-0.1.3/.gitignore
+-rw-r--r--   0      501       20     1255 2023-06-07 15:31:28.000000 oxenai-0.1.3/Develop.md
+-rw-r--r--   0      501       20     1840 2023-06-07 15:31:28.000000 oxenai-0.1.3/README.md
+-rw-r--r--   0      501       20      638 2023-05-18 05:25:22.000000 oxenai-0.1.3/docs/Makefile
+-rw-r--r--   0      501       20   111104 2023-06-07 15:31:28.000000 oxenai-0.1.3/docs/build/doctrees/concepts/data_frames.doctree
+-rw-r--r--   0      501       20     2426 2023-06-07 15:31:28.000000 oxenai-0.1.3/docs/build/doctrees/concepts/embedding_search.doctree
+-rw-r--r--   0      501       20    33060 2023-06-07 15:31:28.000000 oxenai-0.1.3/docs/build/doctrees/concepts/remote_staging.doctree
+-rw-r--r--   0      501       20     4832 2023-06-07 15:31:28.000000 oxenai-0.1.3/docs/build/doctrees/contributing/documentation.doctree
+-rw-r--r--   0      501       20     3114 2023-06-07 15:31:28.000000 oxenai-0.1.3/docs/build/doctrees/contributing/python.doctree
+-rw-r--r--   0      501       20     3041 2023-06-07 15:31:28.000000 oxenai-0.1.3/docs/build/doctrees/contributing/rust.doctree
+-rw-r--r--   0      501       20   521114 2023-06-07 15:31:28.000000 oxenai-0.1.3/docs/build/doctrees/environment.pickle
+-rw-r--r--   0      501       20     4632 2023-06-07 15:31:28.000000 oxenai-0.1.3/docs/build/doctrees/getting_started/commands.doctree
+-rw-r--r--   0      501       20    13327 2023-06-07 15:31:28.000000 oxenai-0.1.3/docs/build/doctrees/getting_started/installation.doctree
+-rw-r--r--   0      501       20     8868 2023-06-07 15:31:28.000000 oxenai-0.1.3/docs/build/doctrees/getting_started/python.doctree
+-rw-r--r--   0      501       20     2515 2023-06-07 15:31:28.000000 oxenai-0.1.3/docs/build/doctrees/getting_started/tutorials.doctree
+-rw-r--r--   0      501       20    92642 2023-06-07 15:31:28.000000 oxenai-0.1.3/docs/build/doctrees/index.doctree
+-rw-r--r--   0      501       20    41036 2023-06-07 15:31:28.000000 oxenai-0.1.3/docs/build/doctrees/references/python/local_repo.doctree
+-rw-r--r--   0      501       20    54552 2023-06-07 15:31:28.000000 oxenai-0.1.3/docs/build/doctrees/references/python/remote_repo.doctree
+-rw-r--r--   0      501       20     3870 2023-06-07 15:31:28.000000 oxenai-0.1.3/docs/build/doctrees/references/rust.doctree
+-rw-r--r--   0      501       20      230 2023-05-30 22:47:04.000000 oxenai-0.1.3/docs/build/html/.buildinfo
+-rw-r--r--   0      501       20    45695 2023-06-07 15:31:28.000000 oxenai-0.1.3/docs/build/html/_sources/concepts/data_frames.md
+-rw-r--r--   0      501       20       18 2023-06-07 15:31:28.000000 oxenai-0.1.3/docs/build/html/_sources/concepts/embedding_search.md
+-rw-r--r--   0      501       20    10491 2023-05-30 22:47:04.000000 oxenai-0.1.3/docs/build/html/_sources/concepts/remote_staging.md
+-rw-r--r--   0      501       20      435 2023-06-07 15:31:28.000000 oxenai-0.1.3/docs/build/html/_sources/contributing/documentation.md
+-rw-r--r--   0      501       20      165 2023-06-07 15:31:28.000000 oxenai-0.1.3/docs/build/html/_sources/contributing/python.md
+-rw-r--r--   0      501       20      135 2023-06-07 15:31:28.000000 oxenai-0.1.3/docs/build/html/_sources/contributing/rust.md
+-rw-r--r--   0      501       20      435 2023-05-17 22:27:30.000000 oxenai-0.1.3/docs/build/html/_sources/getting_started/commands.md
+-rw-r--r--   0      501       20     2148 2023-05-18 04:14:06.000000 oxenai-0.1.3/docs/build/html/_sources/getting_started/installation.md
+-rw-r--r--   0      501       20     1816 2023-05-30 22:47:04.000000 oxenai-0.1.3/docs/build/html/_sources/getting_started/python.md
+-rw-r--r--   0      501       20       18 2023-05-17 00:07:17.000000 oxenai-0.1.3/docs/build/html/_sources/getting_started/tutorials.md
+-rw-r--r--   0      501       20     1130 2023-06-07 15:31:28.000000 oxenai-0.1.3/docs/build/html/_sources/index.rst
+-rw-r--r--   0      501       20       69 2023-05-18 03:59:38.000000 oxenai-0.1.3/docs/build/html/_sources/references/python/local_repo.rst
+-rw-r--r--   0      501       20       68 2023-05-18 04:14:40.000000 oxenai-0.1.3/docs/build/html/_sources/references/python/remote_repo.rst
+-rw-r--r--   0      501       20      235 2023-05-18 04:22:39.000000 oxenai-0.1.3/docs/build/html/_sources/references/rust.md
+-rw-r--r--   0      501       20    14813 2023-05-24 22:24:23.000000 oxenai-0.1.3/docs/build/html/_static/basic.css
+-rw-r--r--   0      501       20      313 2023-05-16 23:41:23.000000 oxenai-0.1.3/docs/build/html/_static/check-solid.svg
+-rw-r--r--   0      501       20     9031 2023-05-16 23:41:23.000000 oxenai-0.1.3/docs/build/html/_static/clipboard.min.js
+-rw-r--r--   0      501       20      411 2023-05-16 23:41:23.000000 oxenai-0.1.3/docs/build/html/_static/copy-button.svg
+-rw-r--r--   0      501       20     2060 2023-05-16 23:41:23.000000 oxenai-0.1.3/docs/build/html/_static/copybutton.css
+-rw-r--r--   0      501       20     8469 2023-05-30 22:47:04.000000 oxenai-0.1.3/docs/build/html/_static/copybutton.js
+-rw-r--r--   0      501       20     2698 2023-05-16 23:41:23.000000 oxenai-0.1.3/docs/build/html/_static/copybutton_funcs.js
+-rw-r--r--   0      501       20     4472 2023-05-16 20:00:40.000000 oxenai-0.1.3/docs/build/html/_static/doctools.js
+-rw-r--r--   0      501       20      415 2023-05-24 22:24:23.000000 oxenai-0.1.3/docs/build/html/_static/documentation_options.js
+-rw-r--r--   0      501       20      286 2023-05-16 20:00:40.000000 oxenai-0.1.3/docs/build/html/_static/file.png
+-rw-r--r--   0      501       20     1186 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/images/logo_binder.svg
+-rw-r--r--   0      501       20     7601 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/images/logo_colab.png
+-rw-r--r--   0      501       20      681 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/images/logo_deepnote.svg
+-rw-r--r--   0      501       20     1758 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/images/logo_jupyterhub.svg
+-rw-r--r--   0      501       20     4758 2023-05-24 22:24:23.000000 oxenai-0.1.3/docs/build/html/_static/language_data.js
+-rw-r--r--   0      501       20     1459 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/locales/ar/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1626 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/locales/bg/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1564 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/locales/bn/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1166 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/locales/ca/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1323 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/locales/cs/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1222 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/locales/da/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1306 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/locales/de/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1640 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/locales/el/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1255 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/locales/eo/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1314 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/locales/es/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1259 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/locales/et/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1286 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/locales/fi/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1330 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/locales/fr/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1320 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/locales/hr/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1241 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/locales/id/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1321 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/locales/it/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1363 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/locales/iw/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1389 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/locales/ja/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1293 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/locales/ko/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1331 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/locales/lt/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1322 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/locales/lv/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1803 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/locales/ml/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1594 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/locales/mr/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1133 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/locales/ms/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1274 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/locales/nl/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1235 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/locales/no/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1289 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/locales/pl/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1282 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/locales/pt/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1308 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/locales/ro/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1640 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/locales/ru/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1311 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/locales/sk/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1292 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/locales/sl/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1597 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/locales/sr/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1267 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/locales/sv/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1848 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/locales/ta/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1726 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/locales/te/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1546 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/locales/tg/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1684 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/locales/th/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1193 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/locales/tl/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1291 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/locales/tr/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1601 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/locales/uk/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1382 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/locales/ur/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1349 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/locales/vi/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1228 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20     1259 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po
+-rw-r--r--   0      501       20       90 2023-05-16 20:00:40.000000 oxenai-0.1.3/docs/build/html/_static/minus.png
+-rw-r--r--   0      501       20       90 2023-05-16 20:00:40.000000 oxenai-0.1.3/docs/build/html/_static/plus.png
+-rw-r--r--   0      501       20    12757 2023-05-24 22:24:23.000000 oxenai-0.1.3/docs/build/html/_static/pygments.css
+-rw-r--r--   0      501       20      419 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/sbt-webpack-macros.html
+-rw-r--r--   0      501       20    80813 2023-05-16 20:04:17.000000 oxenai-0.1.3/docs/build/html/_static/scripts/bootstrap.js
+-rw-r--r--   0      501       20      237 2023-05-16 20:04:17.000000 oxenai-0.1.3/docs/build/html/_static/scripts/bootstrap.js.LICENSE.txt
+-rw-r--r--   0      501       20   335757 2023-05-16 20:04:17.000000 oxenai-0.1.3/docs/build/html/_static/scripts/bootstrap.js.map
+-rw-r--r--   0      501       20     4456 2023-05-16 20:04:17.000000 oxenai-0.1.3/docs/build/html/_static/scripts/pydata-sphinx-theme.js
+-rw-r--r--   0      501       20    19648 2023-05-16 20:04:17.000000 oxenai-0.1.3/docs/build/html/_static/scripts/pydata-sphinx-theme.js.map
+-rw-r--r--   0      501       20     3075 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/scripts/sphinx-book-theme.js
+-rw-r--r--   0      501       20    13066 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/scripts/sphinx-book-theme.js.map
+-rw-r--r--   0      501       20    18215 2023-05-16 20:00:40.000000 oxenai-0.1.3/docs/build/html/_static/searchtools.js
+-rw-r--r--   0      501       20     4712 2023-05-16 20:00:40.000000 oxenai-0.1.3/docs/build/html/_static/sphinx_highlight.js
+-rw-r--r--   0      501       20   176654 2023-05-16 20:04:17.000000 oxenai-0.1.3/docs/build/html/_static/styles/bootstrap.css
+-rw-r--r--   0      501       20    63341 2023-05-16 20:04:17.000000 oxenai-0.1.3/docs/build/html/_static/styles/pydata-sphinx-theme.css
+-rw-r--r--   0      501       20    13841 2023-05-17 00:03:57.000000 oxenai-0.1.3/docs/build/html/_static/styles/sphinx-book-theme.css
+-rw-r--r--   0      501       20      106 2023-05-16 20:04:17.000000 oxenai-0.1.3/docs/build/html/_static/styles/theme.css
+-rw-r--r--   0      501       20     7427 2023-05-16 20:04:17.000000 oxenai-0.1.3/docs/build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt
+-rw-r--r--   0      501       20   101691 2023-05-16 20:04:17.000000 oxenai-0.1.3/docs/build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css
+-rw-r--r--   0      501       20   181264 2023-05-16 20:04:17.000000 oxenai-0.1.3/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf
+-rw-r--r--   0      501       20   105112 2023-05-16 20:04:17.000000 oxenai-0.1.3/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2
+-rw-r--r--   0      501       20    60236 2023-05-16 20:04:17.000000 oxenai-0.1.3/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf
+-rw-r--r--   0      501       20    24028 2023-05-16 20:04:17.000000 oxenai-0.1.3/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2
+-rw-r--r--   0      501       20   389948 2023-05-16 20:04:17.000000 oxenai-0.1.3/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf
+-rw-r--r--   0      501       20   154840 2023-05-16 20:04:17.000000 oxenai-0.1.3/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2
+-rw-r--r--   0      501       20    10084 2023-05-16 20:04:17.000000 oxenai-0.1.3/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0      501       20     4776 2023-05-16 20:04:17.000000 oxenai-0.1.3/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2
+-rw-r--r--   0      501       20     1863 2023-05-16 20:04:17.000000 oxenai-0.1.3/docs/build/html/_static/webpack-macros.html
+-rw-r--r--   0      501       20    94792 2023-06-07 15:31:28.000000 oxenai-0.1.3/docs/build/html/concepts/data_frames.html
+-rw-r--r--   0      501       20    12188 2023-06-07 15:31:28.000000 oxenai-0.1.3/docs/build/html/concepts/embedding_search.html
+-rw-r--r--   0      501       20    41523 2023-06-07 15:31:28.000000 oxenai-0.1.3/docs/build/html/concepts/remote_staging.html
+-rw-r--r--   0      501       20    13736 2023-06-07 15:31:28.000000 oxenai-0.1.3/docs/build/html/contributing/documentation.html
+-rw-r--r--   0      501       20    14226 2023-06-07 15:31:28.000000 oxenai-0.1.3/docs/build/html/contributing/python.html
+-rw-r--r--   0      501       20    13585 2023-06-07 15:31:28.000000 oxenai-0.1.3/docs/build/html/contributing/rust.html
+-rw-r--r--   0      501       20    17490 2023-06-07 15:31:28.000000 oxenai-0.1.3/docs/build/html/genindex.html
+-rw-r--r--   0      501       20    14743 2023-06-07 15:31:28.000000 oxenai-0.1.3/docs/build/html/getting_started/commands.html
+-rw-r--r--   0      501       20    21507 2023-06-07 15:31:28.000000 oxenai-0.1.3/docs/build/html/getting_started/installation.html
+-rw-r--r--   0      501       20    18772 2023-06-07 15:31:28.000000 oxenai-0.1.3/docs/build/html/getting_started/python.html
+-rw-r--r--   0      501       20    12068 2023-06-07 15:31:28.000000 oxenai-0.1.3/docs/build/html/getting_started/tutorials.html
+-rw-r--r--   0      501       20    72087 2023-06-07 15:31:28.000000 oxenai-0.1.3/docs/build/html/index.html
+-rw-r--r--   0      501       20      888 2023-06-07 15:31:28.000000 oxenai-0.1.3/docs/build/html/objects.inv
+-rw-r--r--   0      501       20    29798 2023-06-07 15:31:28.000000 oxenai-0.1.3/docs/build/html/references/python/local_repo.html
+-rw-r--r--   0      501       20    36459 2023-06-07 15:31:28.000000 oxenai-0.1.3/docs/build/html/references/python/remote_repo.html
+-rw-r--r--   0      501       20    13229 2023-06-07 15:31:28.000000 oxenai-0.1.3/docs/build/html/references/rust.html
+-rw-r--r--   0      501       20    11383 2023-06-07 15:31:28.000000 oxenai-0.1.3/docs/build/html/search.html
+-rw-r--r--   0      501       20    23670 2023-06-07 15:31:28.000000 oxenai-0.1.3/docs/build/html/searchindex.js
+-rw-r--r--   0      501       20       99 2023-05-30 22:47:04.000000 oxenai-0.1.3/docs/docsenv/pyvenv.cfg
+-rw-r--r--   0      501       20      804 2023-05-18 05:25:22.000000 oxenai-0.1.3/docs/make.bat
+-rw-r--r--   0      501       20      131 2023-06-07 20:59:12.000000 oxenai-0.1.3/docs/requirements.txt
+-rw-r--r--   0      501       20    45695 2023-06-07 15:31:28.000000 oxenai-0.1.3/docs/source/concepts/data_frames.md
+-rw-r--r--   0      501       20       24 2023-06-07 15:31:28.000000 oxenai-0.1.3/docs/source/concepts/embedding_search.md
+-rw-r--r--   0      501       20    10491 2023-05-30 22:47:04.000000 oxenai-0.1.3/docs/source/concepts/remote_staging.md
+-rw-r--r--   0      501       20     1395 2023-06-07 15:31:28.000000 oxenai-0.1.3/docs/source/conf.py
+-rw-r--r--   0      501       20      435 2023-06-07 15:31:28.000000 oxenai-0.1.3/docs/source/contributing/documentation.md
+-rw-r--r--   0      501       20      165 2023-06-07 15:31:28.000000 oxenai-0.1.3/docs/source/contributing/python.md
+-rw-r--r--   0      501       20      135 2023-06-07 15:31:28.000000 oxenai-0.1.3/docs/source/contributing/rust.md
+-rw-r--r--   0      501       20      435 2023-05-18 05:25:22.000000 oxenai-0.1.3/docs/source/getting_started/commands.md
+-rw-r--r--   0      501       20     2148 2023-05-18 05:25:22.000000 oxenai-0.1.3/docs/source/getting_started/installation.md
+-rw-r--r--   0      501       20     1816 2023-05-30 22:47:04.000000 oxenai-0.1.3/docs/source/getting_started/python.md
+-rw-r--r--   0      501       20       18 2023-05-18 05:25:22.000000 oxenai-0.1.3/docs/source/getting_started/tutorials.md
+-rw-r--r--   0      501       20     1130 2023-06-07 15:31:28.000000 oxenai-0.1.3/docs/source/index.rst
+-rw-r--r--   0      501       20       69 2023-05-18 05:25:22.000000 oxenai-0.1.3/docs/source/references/python/local_repo.rst
+-rw-r--r--   0      501       20       68 2023-05-18 05:25:22.000000 oxenai-0.1.3/docs/source/references/python/remote_repo.rst
+-rw-r--r--   0      501       20      235 2023-05-18 05:25:22.000000 oxenai-0.1.3/docs/source/references/rust.md
+-rw-r--r--   0      501       20      451 2023-05-18 05:25:22.000000 oxenai-0.1.3/pyproject.toml
+-rw-r--r--   0      501       20      593 2023-06-07 15:31:28.000000 oxenai-0.1.3/python/oxen/__init__.py
+-rw-r--r--   0      501       20      597 2023-06-07 20:58:40.000000 oxenai-0.1.3/python/oxen/auth.py
+-rw-r--r--   0      501       20      746 2023-06-07 15:31:28.000000 oxenai-0.1.3/python/oxen/dag.py
+-rw-r--r--   0      501       20     5995 2023-05-18 05:25:22.000000 oxenai-0.1.3/python/oxen/dataset.py
+-rw-r--r--   0      501       20     1378 2023-05-18 05:25:22.000000 oxenai-0.1.3/python/oxen/features.py
+-rw-r--r--   0      501       20     1500 2023-06-07 15:31:28.000000 oxenai-0.1.3/python/oxen/fs.py
+-rw-r--r--   0      501       20      259 2023-06-07 15:31:28.000000 oxenai-0.1.3/python/oxen/loaders/__init__.py
+-rw-r--r--   0      501       20     1057 2023-05-18 05:25:22.000000 oxenai-0.1.3/python/oxen/loaders/chat.py
+-rw-r--r--   0      501       20     1159 2023-06-07 15:31:28.000000 oxenai-0.1.3/python/oxen/loaders/image_classification.py
+-rw-r--r--   0      501       20      802 2023-05-18 05:25:22.000000 oxenai-0.1.3/python/oxen/loaders/regression.py
+-rw-r--r--   0      501       20     3732 2023-05-18 05:25:22.000000 oxenai-0.1.3/python/oxen/local_repo.py
+-rw-r--r--   0      501       20     1543 2023-06-07 15:31:28.000000 oxenai-0.1.3/python/oxen/op.py
+-rw-r--r--   0      501       20      578 2023-06-07 15:31:28.000000 oxenai-0.1.3/python/oxen/ops/__init__.py
+-rw-r--r--   0      501       20      207 2023-05-18 05:25:22.000000 oxenai-0.1.3/python/oxen/ops/concat_series.py
+-rw-r--r--   0      501       20      876 2023-06-07 15:31:28.000000 oxenai-0.1.3/python/oxen/ops/create_label_map.py
+-rw-r--r--   0      501       20      493 2023-06-07 15:31:28.000000 oxenai-0.1.3/python/oxen/ops/encode_labels.py
+-rw-r--r--   0      501       20      440 2023-06-07 15:31:28.000000 oxenai-0.1.3/python/oxen/ops/extract_col.py
+-rw-r--r--   0      501       20      214 2023-05-18 05:25:22.000000 oxenai-0.1.3/python/oxen/ops/identity.py
+-rw-r--r--   0      501       20      361 2023-06-07 15:31:28.000000 oxenai-0.1.3/python/oxen/ops/read_df.py
+-rw-r--r--   0      501       20      732 2023-06-07 20:58:40.000000 oxenai-0.1.3/python/oxen/ops/read_image_dir.py
+-rw-r--r--   0      501       20      347 2023-06-07 15:31:28.000000 oxenai-0.1.3/python/oxen/ops/read_text.py
+-rw-r--r--   0      501       20      354 2023-05-18 05:25:22.000000 oxenai-0.1.3/python/oxen/ops/str_col_template.py
+-rw-r--r--   0      501       20     5494 2023-05-18 05:25:22.000000 oxenai-0.1.3/python/oxen/remote_repo.py
+-rw-r--r--   0      501       20        0 2023-05-18 05:25:22.000000 oxenai-0.1.3/python/oxen/util/__init__.py
+-rw-r--r--   0      501       20      195 2023-06-07 15:31:28.000000 oxenai-0.1.3/requirements.txt
+-rw-r--r--   0      501       20      908 2023-06-07 15:31:28.000000 oxenai-0.1.3/src/auth.rs
+-rw-r--r--   0      501       20      370 2023-05-18 05:25:22.000000 oxenai-0.1.3/src/error.rs
+-rw-r--r--   0      501       20     2105 2023-06-07 15:31:28.000000 oxenai-0.1.3/src/lib.rs
+-rw-r--r--   0      501       20      718 2023-05-18 05:25:22.000000 oxenai-0.1.3/src/py_branch.rs
+-rw-r--r--   0      501       20      291 2023-05-18 05:25:22.000000 oxenai-0.1.3/src/py_commit.rs
+-rw-r--r--   0      501       20      474 2023-05-18 05:25:22.000000 oxenai-0.1.3/src/py_dataset.rs
+-rw-r--r--   0      501       20     3875 2023-05-18 05:25:22.000000 oxenai-0.1.3/src/py_local_repo.rs
+-rw-r--r--   0      501       20     8111 2023-05-18 05:25:22.000000 oxenai-0.1.3/src/py_remote_repo.rs
+-rw-r--r--   0      501       20     1572 2023-05-18 05:25:22.000000 oxenai-0.1.3/src/py_staged_data.rs
+-rw-r--r--   0      501       20      538 2023-05-18 05:25:22.000000 oxenai-0.1.3/src/util.rs
+-rw-r--r--   0      501       20      345 2023-05-18 05:25:22.000000 oxenai-0.1.3/test.py
+-rw-r--r--   0      501       20        0 2023-05-18 05:25:22.000000 oxenai-0.1.3/tests/__init__.py
+-rw-r--r--   0      501       20     3474 2023-05-18 05:25:22.000000 oxenai-0.1.3/tests/conftest.py
+-rw-r--r--   0      501       20       18 2023-06-07 15:31:28.000000 oxenai-0.1.3/tests/data/CelebA/annotations/labels.txt
+-rw-r--r--   0      501       20       94 2023-06-07 15:31:28.000000 oxenai-0.1.3/tests/data/CelebA/annotations/test.csv
+-rw-r--r--   0      501       20      114 2023-06-07 15:31:28.000000 oxenai-0.1.3/tests/data/CelebA/annotations/train.csv
+-rw-r--r--   0      501       20    11440 2023-05-18 05:25:22.000000 oxenai-0.1.3/tests/data/CelebA/images/1.jpg
+-rw-r--r--   0      501       20     7448 2023-05-18 05:25:22.000000 oxenai-0.1.3/tests/data/CelebA/images/2.jpg
+-rw-r--r--   0      501       20     4253 2023-05-18 05:25:22.000000 oxenai-0.1.3/tests/data/CelebA/images/3.jpg
+-rw-r--r--   0      501       20    10747 2023-05-18 05:25:22.000000 oxenai-0.1.3/tests/data/CelebA/images/4.jpg
+-rw-r--r--   0      501       20     6351 2023-05-18 05:25:22.000000 oxenai-0.1.3/tests/data/CelebA/images/5.jpg
+-rw-r--r--   0      501       20     8073 2023-05-18 05:25:22.000000 oxenai-0.1.3/tests/data/CelebA/images/6.jpg
+-rw-r--r--   0      501       20     8203 2023-05-18 05:25:22.000000 oxenai-0.1.3/tests/data/CelebA/images/7.jpg
+-rw-r--r--   0      501       20     7725 2023-05-18 05:25:22.000000 oxenai-0.1.3/tests/data/CelebA/images/8.jpg
+-rw-r--r--   0      501       20     8641 2023-05-18 05:25:22.000000 oxenai-0.1.3/tests/data/CelebA/images/9.jpg
+-rw-r--r--   0      501       20      337 2023-05-18 05:25:22.000000 oxenai-0.1.3/tests/data/ChatBot/examples.tsv
+-rw-r--r--   0      501       20       88 2023-05-18 05:25:22.000000 oxenai-0.1.3/tests/data/ChatBot/prompt.txt
+-rw-r--r--   0      501       20      148 2023-05-18 05:25:22.000000 oxenai-0.1.3/tests/data/HousePrices/prices.csv
+-rw-r--r--   0      501       20      520 2023-06-07 20:58:40.000000 oxenai-0.1.3/tests/test_add.py
+-rw-r--r--   0      501       20     1706 2023-06-07 15:31:28.000000 oxenai-0.1.3/tests/test_auth.py
+-rw-r--r--   0      501       20      363 2023-05-18 05:25:22.000000 oxenai-0.1.3/tests/test_chat_loader.py
+-rw-r--r--   0      501       20     1299 2023-05-18 05:25:22.000000 oxenai-0.1.3/tests/test_checkout.py
+-rw-r--r--   0      501       20      723 2023-06-07 15:31:28.000000 oxenai-0.1.3/tests/test_clone.py
+-rw-r--r--   0      501       20      850 2023-05-18 05:25:22.000000 oxenai-0.1.3/tests/test_commit.py
+-rw-r--r--   0      501       20     2444 2023-05-18 05:25:22.000000 oxenai-0.1.3/tests/test_dataloader_pytorch.py
+-rw-r--r--   0      501       20     1506 2023-05-18 05:25:22.000000 oxenai-0.1.3/tests/test_dataset.py
+-rw-r--r--   0      501       20     2022 2023-06-07 15:31:28.000000 oxenai-0.1.3/tests/test_image_classification_loader.py
+-rw-r--r--   0      501       20      338 2023-05-18 05:25:22.000000 oxenai-0.1.3/tests/test_init.py
+-rw-r--r--   0      501       20      440 2023-05-18 05:25:22.000000 oxenai-0.1.3/tests/test_push.py
+-rw-r--r--   0      501       20      911 2023-06-07 15:31:28.000000 oxenai-0.1.3/tests/test_push_pull.py
+-rw-r--r--   0      501       20      488 2023-05-18 05:25:22.000000 oxenai-0.1.3/tests/test_regression_loader.py
+-rw-r--r--   0      501       20      828 2023-05-18 05:25:22.000000 oxenai-0.1.3/tests/test_remote_add.py
+-rw-r--r--   0      501       20      560 2023-05-18 05:25:22.000000 oxenai-0.1.3/tests/test_remote_branch.py
+-rw-r--r--   0      501       20      538 2023-05-18 05:25:22.000000 oxenai-0.1.3/tests/test_remote_checkout.py
+-rw-r--r--   0      501       20      685 2023-05-18 05:25:22.000000 oxenai-0.1.3/tests/test_remote_commit.py
+-rw-r--r--   0      501       20     1473 2023-05-18 05:25:22.000000 oxenai-0.1.3/tests/test_remote_df_add.py
+-rw-r--r--   0      501       20      530 2023-05-18 05:25:22.000000 oxenai-0.1.3/tests/test_remote_list.py
+-rw-r--r--   0      501       20      657 2023-05-18 05:25:22.000000 oxenai-0.1.3/tests/test_remote_remove.py
+-rw-r--r--   0      501       20      114 2023-05-18 05:25:22.000000 oxenai-0.1.3/tests/test_remote_repo.py
+-rw-r--r--   0      501       20      636 2023-05-18 05:25:22.000000 oxenai-0.1.3/tests/test_remote_status.py
+-rw-r--r--   0      501       20      259 2023-05-18 05:25:22.000000 oxenai-0.1.3/tests/test_status.py
+-rw-r--r--   0      501       20   109484 2023-06-07 20:59:10.000000 oxenai-0.1.3/Cargo.lock
+-rw-r--r--   0        0        0     2216 1970-01-01 00:00:00.000000 oxenai-0.1.3/PKG-INFO
```

### Comparing `oxenai-0.1.2/.github/workflows/CI.yml` & `oxenai-0.1.3/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/.gitignore` & `oxenai-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/Develop.md` & `oxenai-0.1.3/Develop.md`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/README.md` & `oxenai-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/Makefile` & `oxenai-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/doctrees/concepts/data_frames.doctree` & `oxenai-0.1.3/docs/build/doctrees/concepts/data_frames.doctree`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/doctrees/concepts/embedding_search.doctree` & `oxenai-0.1.3/docs/build/doctrees/concepts/embedding_search.doctree`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/doctrees/concepts/remote_staging.doctree` & `oxenai-0.1.3/docs/build/doctrees/concepts/remote_staging.doctree`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/doctrees/contributing/documentation.doctree` & `oxenai-0.1.3/docs/build/doctrees/contributing/documentation.doctree`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/doctrees/contributing/python.doctree` & `oxenai-0.1.3/docs/build/doctrees/contributing/python.doctree`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/doctrees/contributing/rust.doctree` & `oxenai-0.1.3/docs/build/doctrees/contributing/rust.doctree`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/doctrees/environment.pickle` & `oxenai-0.1.3/docs/build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/doctrees/getting_started/commands.doctree` & `oxenai-0.1.3/docs/build/doctrees/getting_started/commands.doctree`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/doctrees/getting_started/installation.doctree` & `oxenai-0.1.3/docs/build/doctrees/getting_started/installation.doctree`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/doctrees/getting_started/python.doctree` & `oxenai-0.1.3/docs/build/doctrees/getting_started/python.doctree`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/doctrees/getting_started/tutorials.doctree` & `oxenai-0.1.3/docs/build/doctrees/getting_started/tutorials.doctree`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/doctrees/index.doctree` & `oxenai-0.1.3/docs/build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/doctrees/references/python/local_repo.doctree` & `oxenai-0.1.3/docs/build/doctrees/references/python/local_repo.doctree`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/doctrees/references/python/remote_repo.doctree` & `oxenai-0.1.3/docs/build/doctrees/references/python/remote_repo.doctree`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/doctrees/references/rust.doctree` & `oxenai-0.1.3/docs/build/doctrees/references/rust.doctree`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_sources/concepts/data_frames.md` & `oxenai-0.1.3/docs/build/html/_sources/concepts/data_frames.md`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_sources/concepts/remote_staging.md` & `oxenai-0.1.3/docs/build/html/_sources/concepts/remote_staging.md`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_sources/getting_started/installation.md` & `oxenai-0.1.3/docs/build/html/_sources/getting_started/installation.md`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_sources/getting_started/python.md` & `oxenai-0.1.3/docs/build/html/_sources/getting_started/python.md`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_sources/index.rst` & `oxenai-0.1.3/docs/build/html/_sources/index.rst`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/basic.css` & `oxenai-0.1.3/docs/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/clipboard.min.js` & `oxenai-0.1.3/docs/build/html/_static/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/copybutton.css` & `oxenai-0.1.3/docs/build/html/_static/copybutton.css`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/copybutton.js` & `oxenai-0.1.3/docs/build/html/_static/copybutton.js`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/copybutton_funcs.js` & `oxenai-0.1.3/docs/build/html/_static/copybutton_funcs.js`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/doctools.js` & `oxenai-0.1.3/docs/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/images/logo_binder.svg` & `oxenai-0.1.3/docs/build/html/_static/images/logo_binder.svg`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/images/logo_colab.png` & `oxenai-0.1.3/docs/build/html/_static/images/logo_colab.png`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/images/logo_deepnote.svg` & `oxenai-0.1.3/docs/build/html/_static/images/logo_deepnote.svg`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/images/logo_jupyterhub.svg` & `oxenai-0.1.3/docs/build/html/_static/images/logo_jupyterhub.svg`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/language_data.js` & `oxenai-0.1.3/docs/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/locales/ar/LC_MESSAGES/booktheme.po` & `oxenai-0.1.3/docs/build/html/_static/locales/ar/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/locales/bg/LC_MESSAGES/booktheme.po` & `oxenai-0.1.3/docs/build/html/_static/locales/bg/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/locales/bn/LC_MESSAGES/booktheme.po` & `oxenai-0.1.3/docs/build/html/_static/locales/bn/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/locales/ca/LC_MESSAGES/booktheme.po` & `oxenai-0.1.3/docs/build/html/_static/locales/ca/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/locales/cs/LC_MESSAGES/booktheme.po` & `oxenai-0.1.3/docs/build/html/_static/locales/cs/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/locales/da/LC_MESSAGES/booktheme.po` & `oxenai-0.1.3/docs/build/html/_static/locales/da/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/locales/de/LC_MESSAGES/booktheme.po` & `oxenai-0.1.3/docs/build/html/_static/locales/de/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/locales/el/LC_MESSAGES/booktheme.po` & `oxenai-0.1.3/docs/build/html/_static/locales/el/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/locales/eo/LC_MESSAGES/booktheme.po` & `oxenai-0.1.3/docs/build/html/_static/locales/eo/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/locales/es/LC_MESSAGES/booktheme.po` & `oxenai-0.1.3/docs/build/html/_static/locales/es/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/locales/et/LC_MESSAGES/booktheme.po` & `oxenai-0.1.3/docs/build/html/_static/locales/et/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/locales/fi/LC_MESSAGES/booktheme.po` & `oxenai-0.1.3/docs/build/html/_static/locales/fi/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/locales/fr/LC_MESSAGES/booktheme.po` & `oxenai-0.1.3/docs/build/html/_static/locales/fr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/locales/hr/LC_MESSAGES/booktheme.po` & `oxenai-0.1.3/docs/build/html/_static/locales/hr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/locales/id/LC_MESSAGES/booktheme.po` & `oxenai-0.1.3/docs/build/html/_static/locales/id/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/locales/it/LC_MESSAGES/booktheme.po` & `oxenai-0.1.3/docs/build/html/_static/locales/it/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/locales/iw/LC_MESSAGES/booktheme.po` & `oxenai-0.1.3/docs/build/html/_static/locales/iw/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/locales/ja/LC_MESSAGES/booktheme.po` & `oxenai-0.1.3/docs/build/html/_static/locales/ja/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/locales/ko/LC_MESSAGES/booktheme.po` & `oxenai-0.1.3/docs/build/html/_static/locales/ko/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/locales/lt/LC_MESSAGES/booktheme.po` & `oxenai-0.1.3/docs/build/html/_static/locales/lt/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/locales/lv/LC_MESSAGES/booktheme.po` & `oxenai-0.1.3/docs/build/html/_static/locales/lv/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/locales/ml/LC_MESSAGES/booktheme.po` & `oxenai-0.1.3/docs/build/html/_static/locales/ml/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/locales/mr/LC_MESSAGES/booktheme.po` & `oxenai-0.1.3/docs/build/html/_static/locales/mr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/locales/ms/LC_MESSAGES/booktheme.po` & `oxenai-0.1.3/docs/build/html/_static/locales/ms/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/locales/nl/LC_MESSAGES/booktheme.po` & `oxenai-0.1.3/docs/build/html/_static/locales/nl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/locales/no/LC_MESSAGES/booktheme.po` & `oxenai-0.1.3/docs/build/html/_static/locales/no/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/locales/pl/LC_MESSAGES/booktheme.po` & `oxenai-0.1.3/docs/build/html/_static/locales/pl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/locales/pt/LC_MESSAGES/booktheme.po` & `oxenai-0.1.3/docs/build/html/_static/locales/pt/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/locales/ro/LC_MESSAGES/booktheme.po` & `oxenai-0.1.3/docs/build/html/_static/locales/ro/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/locales/ru/LC_MESSAGES/booktheme.po` & `oxenai-0.1.3/docs/build/html/_static/locales/ru/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/locales/sk/LC_MESSAGES/booktheme.po` & `oxenai-0.1.3/docs/build/html/_static/locales/sk/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/locales/sl/LC_MESSAGES/booktheme.po` & `oxenai-0.1.3/docs/build/html/_static/locales/sl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/locales/sr/LC_MESSAGES/booktheme.po` & `oxenai-0.1.3/docs/build/html/_static/locales/sr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/locales/sv/LC_MESSAGES/booktheme.po` & `oxenai-0.1.3/docs/build/html/_static/locales/sv/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/locales/ta/LC_MESSAGES/booktheme.po` & `oxenai-0.1.3/docs/build/html/_static/locales/ta/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/locales/te/LC_MESSAGES/booktheme.po` & `oxenai-0.1.3/docs/build/html/_static/locales/te/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/locales/tg/LC_MESSAGES/booktheme.po` & `oxenai-0.1.3/docs/build/html/_static/locales/tg/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/locales/th/LC_MESSAGES/booktheme.po` & `oxenai-0.1.3/docs/build/html/_static/locales/th/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/locales/tl/LC_MESSAGES/booktheme.po` & `oxenai-0.1.3/docs/build/html/_static/locales/tl/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/locales/tr/LC_MESSAGES/booktheme.po` & `oxenai-0.1.3/docs/build/html/_static/locales/tr/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/locales/uk/LC_MESSAGES/booktheme.po` & `oxenai-0.1.3/docs/build/html/_static/locales/uk/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/locales/ur/LC_MESSAGES/booktheme.po` & `oxenai-0.1.3/docs/build/html/_static/locales/ur/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/locales/vi/LC_MESSAGES/booktheme.po` & `oxenai-0.1.3/docs/build/html/_static/locales/vi/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po` & `oxenai-0.1.3/docs/build/html/_static/locales/zh_CN/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po` & `oxenai-0.1.3/docs/build/html/_static/locales/zh_TW/LC_MESSAGES/booktheme.po`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/pygments.css` & `oxenai-0.1.3/docs/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/scripts/bootstrap.js` & `oxenai-0.1.3/docs/build/html/_static/scripts/bootstrap.js`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/scripts/bootstrap.js.map` & `oxenai-0.1.3/docs/build/html/_static/scripts/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/scripts/pydata-sphinx-theme.js` & `oxenai-0.1.3/docs/build/html/_static/scripts/pydata-sphinx-theme.js`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/scripts/pydata-sphinx-theme.js.map` & `oxenai-0.1.3/docs/build/html/_static/scripts/pydata-sphinx-theme.js.map`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/scripts/sphinx-book-theme.js` & `oxenai-0.1.3/docs/build/html/_static/scripts/sphinx-book-theme.js`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/scripts/sphinx-book-theme.js.map` & `oxenai-0.1.3/docs/build/html/_static/scripts/sphinx-book-theme.js.map`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/searchtools.js` & `oxenai-0.1.3/docs/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/sphinx_highlight.js` & `oxenai-0.1.3/docs/build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/styles/bootstrap.css` & `oxenai-0.1.3/docs/build/html/_static/styles/bootstrap.css`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/styles/pydata-sphinx-theme.css` & `oxenai-0.1.3/docs/build/html/_static/styles/pydata-sphinx-theme.css`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/styles/sphinx-book-theme.css` & `oxenai-0.1.3/docs/build/html/_static/styles/sphinx-book-theme.css`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt` & `oxenai-0.1.3/docs/build/html/_static/vendor/fontawesome/6.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css` & `oxenai-0.1.3/docs/build/html/_static/vendor/fontawesome/6.1.2/css/all.min.css`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf` & `oxenai-0.1.3/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2` & `oxenai-0.1.3/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf` & `oxenai-0.1.3/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2` & `oxenai-0.1.3/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf` & `oxenai-0.1.3/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2` & `oxenai-0.1.3/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf` & `oxenai-0.1.3/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2` & `oxenai-0.1.3/docs/build/html/_static/vendor/fontawesome/6.1.2/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/_static/webpack-macros.html` & `oxenai-0.1.3/docs/build/html/_static/webpack-macros.html`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/concepts/data_frames.html` & `oxenai-0.1.3/docs/build/html/concepts/data_frames.html`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/concepts/embedding_search.html` & `oxenai-0.1.3/docs/build/html/concepts/embedding_search.html`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/concepts/remote_staging.html` & `oxenai-0.1.3/docs/build/html/concepts/remote_staging.html`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/contributing/documentation.html` & `oxenai-0.1.3/docs/build/html/contributing/documentation.html`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/contributing/python.html` & `oxenai-0.1.3/docs/build/html/contributing/python.html`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/contributing/rust.html` & `oxenai-0.1.3/docs/build/html/contributing/rust.html`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/genindex.html` & `oxenai-0.1.3/docs/build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/getting_started/commands.html` & `oxenai-0.1.3/docs/build/html/getting_started/commands.html`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/getting_started/installation.html` & `oxenai-0.1.3/docs/build/html/getting_started/installation.html`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/getting_started/python.html` & `oxenai-0.1.3/docs/build/html/getting_started/python.html`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/getting_started/tutorials.html` & `oxenai-0.1.3/docs/build/html/getting_started/tutorials.html`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/index.html` & `oxenai-0.1.3/docs/build/html/index.html`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/objects.inv` & `oxenai-0.1.3/docs/build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/references/python/local_repo.html` & `oxenai-0.1.3/docs/build/html/references/python/local_repo.html`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/references/python/remote_repo.html` & `oxenai-0.1.3/docs/build/html/references/python/remote_repo.html`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/references/rust.html` & `oxenai-0.1.3/docs/build/html/references/rust.html`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/search.html` & `oxenai-0.1.3/docs/build/html/search.html`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/build/html/searchindex.js` & `oxenai-0.1.3/docs/build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/make.bat` & `oxenai-0.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/source/concepts/data_frames.md` & `oxenai-0.1.3/docs/source/concepts/data_frames.md`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/source/concepts/remote_staging.md` & `oxenai-0.1.3/docs/source/concepts/remote_staging.md`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/source/conf.py` & `oxenai-0.1.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/source/getting_started/installation.md` & `oxenai-0.1.3/docs/source/getting_started/installation.md`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/source/getting_started/python.md` & `oxenai-0.1.3/docs/source/getting_started/python.md`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/docs/source/index.rst` & `oxenai-0.1.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/python/oxen/__init__.py` & `oxenai-0.1.3/python/oxen/__init__.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/python/oxen/auth.py` & `oxenai-0.1.3/python/oxen/auth.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,13 +5,13 @@
     if path is None:
         path = f"{auth.get_oxen_home_dir()}/user_config.toml"
     if not path.endswith(".toml"):
         raise ValueError("Path must end with .toml")
     auth.create_user_config(name, email, path)
 
 
-def add_host_auth(name: str, email: str, path: str | None = None):
+def add_host_auth(host: str, token: str, path: str | None = None):
     if path is None:
         path = f"{auth.get_oxen_home_dir()}/user_config.toml"
     if not path.endswith(".toml"):
         raise ValueError("Path must end with .toml")
-    auth.add_host_auth(name, email, path)
+    auth.add_host_auth(host, token, path)
```

### Comparing `oxenai-0.1.2/python/oxen/dag.py` & `oxenai-0.1.3/python/oxen/dag.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/python/oxen/dataset.py` & `oxenai-0.1.3/python/oxen/dataset.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/python/oxen/features.py` & `oxenai-0.1.3/python/oxen/features.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/python/oxen/fs.py` & `oxenai-0.1.3/python/oxen/fs.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/python/oxen/loaders/chat.py` & `oxenai-0.1.3/python/oxen/loaders/chat.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/python/oxen/loaders/image_classification.py` & `oxenai-0.1.3/python/oxen/loaders/image_classification.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/python/oxen/loaders/regression.py` & `oxenai-0.1.3/python/oxen/loaders/regression.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/python/oxen/local_repo.py` & `oxenai-0.1.3/python/oxen/local_repo.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/python/oxen/op.py` & `oxenai-0.1.3/python/oxen/op.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/python/oxen/ops/__init__.py` & `oxenai-0.1.3/python/oxen/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/python/oxen/ops/create_label_map.py` & `oxenai-0.1.3/python/oxen/ops/create_label_map.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/python/oxen/ops/read_image_dir.py` & `oxenai-0.1.3/python/oxen/ops/read_image_dir.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,11 +17,11 @@
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def call(self, args):
         image_data = []
         prefix = args[0]
         for path in tqdm(args[1]):
-            img = cv2.imread(f"{prefix}/{path}")
+            img = cv2.imread(f"{prefix}/{path}", cv2.IMREAD_UNCHANGED)
             image_data.append(img)
         return np.array(image_data)
```

### Comparing `oxenai-0.1.2/python/oxen/remote_repo.py` & `oxenai-0.1.3/python/oxen/remote_repo.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/src/auth.rs` & `oxenai-0.1.3/src/auth.rs`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/src/lib.rs` & `oxenai-0.1.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/src/py_branch.rs` & `oxenai-0.1.3/src/py_branch.rs`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/src/py_local_repo.rs` & `oxenai-0.1.3/src/py_local_repo.rs`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/src/py_remote_repo.rs` & `oxenai-0.1.3/src/py_remote_repo.rs`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/src/py_staged_data.rs` & `oxenai-0.1.3/src/py_staged_data.rs`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/src/util.rs` & `oxenai-0.1.3/src/util.rs`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/tests/conftest.py` & `oxenai-0.1.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/tests/data/CelebA/images/1.jpg` & `oxenai-0.1.3/tests/data/CelebA/images/1.jpg`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/tests/data/CelebA/images/2.jpg` & `oxenai-0.1.3/tests/data/CelebA/images/2.jpg`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/tests/data/CelebA/images/3.jpg` & `oxenai-0.1.3/tests/data/CelebA/images/3.jpg`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/tests/data/CelebA/images/4.jpg` & `oxenai-0.1.3/tests/data/CelebA/images/4.jpg`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/tests/data/CelebA/images/5.jpg` & `oxenai-0.1.3/tests/data/CelebA/images/5.jpg`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/tests/data/CelebA/images/6.jpg` & `oxenai-0.1.3/tests/data/CelebA/images/6.jpg`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/tests/data/CelebA/images/7.jpg` & `oxenai-0.1.3/tests/data/CelebA/images/7.jpg`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/tests/data/CelebA/images/8.jpg` & `oxenai-0.1.3/tests/data/CelebA/images/8.jpg`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/tests/data/CelebA/images/9.jpg` & `oxenai-0.1.3/tests/data/CelebA/images/9.jpg`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/tests/test_add.py` & `oxenai-0.1.3/tests/test_add.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,13 +11,13 @@
     full_path = os.path.join(repo_dir, image_file)
     repo.add(full_path)
     staged_data = repo.status()
 
     added_files = staged_data.added_files()
     added_files.sort()
 
-    assert set(added_file) == {
+    assert set(added_files) == {
         "annotations/test.csv",
         "annotations/train.csv",
         "annotations/labels.txt"
     }
```

### Comparing `oxenai-0.1.2/tests/test_auth.py` & `oxenai-0.1.3/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/tests/test_checkout.py` & `oxenai-0.1.3/tests/test_checkout.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/tests/test_clone.py` & `oxenai-0.1.3/tests/test_clone.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/tests/test_commit.py` & `oxenai-0.1.3/tests/test_commit.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/tests/test_dataloader_pytorch.py` & `oxenai-0.1.3/tests/test_dataloader_pytorch.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/tests/test_dataset.py` & `oxenai-0.1.3/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/tests/test_image_classification_loader.py` & `oxenai-0.1.3/tests/test_image_classification_loader.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/tests/test_push_pull.py` & `oxenai-0.1.3/tests/test_push_pull.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/tests/test_remote_add.py` & `oxenai-0.1.3/tests/test_remote_add.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/tests/test_remote_branch.py` & `oxenai-0.1.3/tests/test_remote_branch.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/tests/test_remote_checkout.py` & `oxenai-0.1.3/tests/test_remote_checkout.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/tests/test_remote_commit.py` & `oxenai-0.1.3/tests/test_remote_commit.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/tests/test_remote_df_add.py` & `oxenai-0.1.3/tests/test_remote_df_add.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/tests/test_remote_list.py` & `oxenai-0.1.3/tests/test_remote_list.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/tests/test_remote_remove.py` & `oxenai-0.1.3/tests/test_remote_remove.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/tests/test_remote_status.py` & `oxenai-0.1.3/tests/test_remote_status.py`

 * *Files identical despite different names*

### Comparing `oxenai-0.1.2/Cargo.lock` & `oxenai-0.1.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -2461,15 +2461,15 @@
 name = "option-ext"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "04744f49eae99ab78e0d5c0b603ab218f515ea8cfe5a456d7629ad883a3b6e7d"
 
 [[package]]
 name = "oxen"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
  "liboxen",
  "log",
  "pyo3",
  "pyo3-asyncio",
  "pyo3-log",
  "pyo3-polars",
```

### Comparing `oxenai-0.1.2/PKG-INFO` & `oxenai-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oxenai
-Version: 0.1.2
+Version: 0.1.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Data version control for machine learning
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

