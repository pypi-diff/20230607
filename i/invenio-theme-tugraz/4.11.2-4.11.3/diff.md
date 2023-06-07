# Comparing `tmp/invenio-theme-tugraz-4.11.2.tar.gz` & `tmp/invenio-theme-tugraz-4.11.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-theme-tugraz-4.11.2.tar", last modified: Thu Jun  1 10:46:22 2023, max compression
+gzip compressed data, was "dist/invenio-theme-tugraz-4.11.3.tar", last modified: Wed Jun  7 21:37:16 2023, max compression
```

## Comparing `invenio-theme-tugraz-4.11.2.tar` & `invenio-theme-tugraz-4.11.3.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/.github/workflows/tests.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/.tx/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/.tx/config
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/scss/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/footer.scss
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/header.scss
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/overrides.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/search/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/search/footer.scss
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/search/theme.scss
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/search/variables.scss
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/theme.scss
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/variables.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/js/invenio_theme_tugraz/
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/js/invenio_theme_tugraz/theme.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/accounts.less
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/communities.less
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/deposit.less
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/
--rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/OFL.txt
--rw-r--r--   0 runner    (1001) docker     (123)    94816 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/SourceSansPro-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   269108 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/SourceSansPro-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/footer.less
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/frontpage.less
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/header.less
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/login.less
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/macros.less
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/overrides.less
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/record.less
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/search.less
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/theme.less
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/variables.less
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/extra/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/extra/orcid.png
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)    18533 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/Fair_Data_Austria_orangerot.png
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/Icon_1_v2.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/TU_Austria_Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)   225210 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/footer.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/icon_use.png
--rw-r--r--   0 runner    (1001) docker     (123)    18643 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/inveniordm-tail.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/library_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    23820 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/login_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    97455 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    16480 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/oea.svg
--rw-r--r--   0 runner    (1001) docker     (123)    38212 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/re3data.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/tug_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/
--rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/accounts_base.html
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/header_login.html
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/login_user.html
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/register_user.html
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/benefits.html
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/comingsoon.html
--rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/header.html
--rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/macros/
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/macros/authors.html
--rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/navbar.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/translations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/translations/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-06-01 10:46:21.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (123)    16921 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/translations/de/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)    12938 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/translations/messages.pot
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/invenio_theme_tugraz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      660 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:46:22.000000 invenio-theme-tugraz-4.11.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-01 10:46:13.000000 invenio-theme-tugraz-4.11.2/tests/test_invenio_theme_tugraz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:37:16.000000 invenio-theme-tugraz-4.11.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:37:16.000000 invenio-theme-tugraz-4.11.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:37:16.000000 invenio-theme-tugraz-4.11.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/.github/workflows/tests.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:37:16.000000 invenio-theme-tugraz-4.11.3/.tx/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/.tx/config
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7791 2023-06-07 21:37:16.000000 invenio-theme-tugraz-4.11.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:37:16.000000 invenio-theme-tugraz-4.11.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:37:16.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:37:16.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:37:16.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/scss/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:37:16.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/footer.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/header.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/overrides.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:37:16.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/search/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/search/footer.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/search/theme.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/search/variables.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/theme.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/variables.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:37:16.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:37:16.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:37:16.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/semantic-ui/js/invenio_theme_tugraz/
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/semantic-ui/js/invenio_theme_tugraz/theme.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:37:16.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/semantic-ui/less/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:37:16.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/accounts.less
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/communities.less
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/deposit.less
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:37:16.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:37:16.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/
+-rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/OFL.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    94816 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/SourceSansPro-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   269108 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/SourceSansPro-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/footer.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/frontpage.less
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/header.less
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/login.less
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/macros.less
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/overrides.less
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/record.less
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/search.less
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/theme.less
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/variables.less
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:37:16.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:37:16.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/static/extra/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/static/extra/orcid.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:37:16.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    18533 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/static/images/Fair_Data_Austria_orangerot.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/static/images/Icon_1_v2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/static/images/TU_Austria_Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   225210 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/static/images/footer.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/static/images/icon_use.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18643 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/static/images/inveniordm-tail.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/static/images/library_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23820 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/static/images/login_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    97455 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/static/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16480 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/static/images/oea.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    38212 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/static/images/re3data.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/static/images/tug_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:37:16.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:37:16.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/templates/invenio_theme_tugraz/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:37:16.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/accounts_base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/header_login.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/login_user.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/register_user.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/templates/invenio_theme_tugraz/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/templates/invenio_theme_tugraz/benefits.html
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/templates/invenio_theme_tugraz/comingsoon.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/templates/invenio_theme_tugraz/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/templates/invenio_theme_tugraz/header.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:37:16.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/templates/invenio_theme_tugraz/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/templates/invenio_theme_tugraz/macros/authors.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6530 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/templates/invenio_theme_tugraz/navbar.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:37:16.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/translations/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:37:16.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:37:16.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-06-07 21:37:15.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    16921 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/translations/de/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)    12938 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/translations/messages.pot
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:37:16.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7791 2023-06-07 21:37:15.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-06-07 21:37:16.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 21:37:15.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-07 21:37:15.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 21:37:15.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-07 21:37:15.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-07 21:37:15.000000 invenio-theme-tugraz-4.11.3/invenio_theme_tugraz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      660 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-06-07 21:37:16.000000 invenio-theme-tugraz-4.11.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:37:16.000000 invenio-theme-tugraz-4.11.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-07 21:37:09.000000 invenio-theme-tugraz-4.11.3/tests/test_invenio_theme_tugraz.py
```

### Comparing `invenio-theme-tugraz-4.11.2/.editorconfig` & `invenio-theme-tugraz-4.11.3/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/.github/workflows/pypi-publish.yml` & `invenio-theme-tugraz-4.11.3/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/.github/workflows/tests.yml` & `invenio-theme-tugraz-4.11.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/.tx/config` & `invenio-theme-tugraz-4.11.3/.tx/config`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/CHANGES.rst` & `invenio-theme-tugraz-4.11.3/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,19 @@
     invenio-theme-tugraz is free software; you can redistribute it and/or
     modify it under the terms of the MIT License; see LICENSE file for more
     details.
 
 Changes
 =======
 
+Version v4.11.3 (release 2023-06-07)
+
+- fix: frontpage upload buttons small monitor
+
+
 Version v4.11.2 (release 2023-06-01)
 
 - frontpage: layout changes
 - translation: add oer frontpage translation
 - WIP: oer upload button on frontpage
```

### Comparing `invenio-theme-tugraz-4.11.2/CONTRIBUTING.rst` & `invenio-theme-tugraz-4.11.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/LICENSE` & `invenio-theme-tugraz-4.11.3/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/MANIFEST.in` & `invenio-theme-tugraz-4.11.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/PKG-INFO` & `invenio-theme-tugraz-4.11.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-theme-tugraz
-Version: 4.11.2
+Version: 4.11.3
 Summary: "Invenio module for TUGRAZ theme."
 Home-page: https://github.com/tu-graz-library/invenio-theme-tugraz
 Author: "Graz University of Technology"
 Author-email: mojib.wali@tugraz.at
 License: MIT
 Description: ..
             Copyright (C) 2020-2021 Graz University of Technology.
@@ -58,14 +58,19 @@
             invenio-theme-tugraz is free software; you can redistribute it and/or
             modify it under the terms of the MIT License; see LICENSE file for more
             details.
         
         Changes
         =======
         
+        Version v4.11.3 (release 2023-06-07)
+        
+        - fix: frontpage upload buttons small monitor
+        
+        
         Version v4.11.2 (release 2023-06-01)
         
         - frontpage: layout changes
         - translation: add oer frontpage translation
         - WIP: oer upload button on frontpage
```

### Comparing `invenio-theme-tugraz-4.11.2/README.rst` & `invenio-theme-tugraz-4.11.3/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/docs/Makefile` & `invenio-theme-tugraz-4.11.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/docs/conf.py` & `invenio-theme-tugraz-4.11.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/docs/index.rst` & `invenio-theme-tugraz-4.11.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/docs/make.bat` & `invenio-theme-tugraz-4.11.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/footer.scss` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/footer.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/header.scss` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/header.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/overrides.scss` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/overrides.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/search/footer.scss` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/scss/invenio_theme_tugraz/search/footer.scss`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/js/invenio_theme_tugraz/theme.js` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/semantic-ui/js/invenio_theme_tugraz/theme.js`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/accounts.less` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/accounts.less`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/OFL.txt` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/OFL.txt`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/SourceSansPro-Italic.ttf` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/SourceSansPro-Italic.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/SourceSansPro-Regular.ttf` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/fonts/SourceSansPro/SourceSansPro-Regular.ttf`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/footer.less` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/footer.less`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/frontpage.less` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/frontpage.less`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/header.less` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/header.less`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/overrides.less` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/overrides.less`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/search.less` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/search.less`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/theme.less` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/theme.less`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/variables.less` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/assets/semantic-ui/less/invenio_theme_tugraz/variables.less`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/config.py` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/config.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/ext.py` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/search.py` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/search.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/extra/orcid.png` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/static/extra/orcid.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/favicon.ico` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/Fair_Data_Austria_orangerot.png` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/static/images/Fair_Data_Austria_orangerot.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/Icon_1_v2.svg` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/static/images/Icon_1_v2.svg`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/TU_Austria_Logo.png` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/static/images/TU_Austria_Logo.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/footer.jpg` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/static/images/footer.jpg`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/icon_use.png` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/static/images/icon_use.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/inveniordm-tail.svg` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/static/images/inveniordm-tail.svg`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/library_logo.png` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/static/images/library_logo.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/login_logo.png` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/static/images/login_logo.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/logo.svg` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/oea.svg` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/static/images/oea.svg`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/re3data.svg` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/static/images/re3data.svg`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/static/images/tug_logo.png` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/static/images/tug_logo.png`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/accounts_base.html` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/accounts_base.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/header_login.html` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/header_login.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/login_user.html` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/login_user.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/register_user.html` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/templates/invenio_theme_tugraz/accounts/register_user.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/base.html` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/templates/invenio_theme_tugraz/base.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/benefits.html` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/templates/invenio_theme_tugraz/benefits.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/footer.html` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/templates/invenio_theme_tugraz/footer.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/header.html` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/templates/invenio_theme_tugraz/header.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/templates/invenio_theme_tugraz/index.html`

 * *Files 20% similar despite different names*

```diff
@@ -105,33 +105,38 @@
 
 
     <!---segments-->
     <div class="six wide column">
       <div class="ui segment" style="padding-bottom: 10px;">
         <h4>{{ _("You can upload different types of records:") }}</h4>
 
-        <p style="margin: 14px">
-          <span class="ui left floated" style="text-align: justify; width:260px; display:inline-block;">
-            {{ _("Visibility of uploaded content is maximized through synchronization with data hubs (DataCite).") }}
-          </span>
-          <a class="ui positive right floated button" style="width:250px; display:inline-block;" href="me/uploads" title="Research Data">
-            <i aria-hidden="true" class="upload icon"></i>
-            {{ _("Upload Research Output") }}
-          </a>
-        </p>
-        <p style="margin: 14px;">
-          <span class="ui left floated" style="text-align: justify; width:260px; display:inline-block;">
-            {{ _("Open Educational Resources (OER) will be visible on various discovery tools like the OERhub.") }}
-          </span>
-
-          <a class="ui positive right floated button" style="width:250px; display:inline-block;" href="lom/uploads" title="Open Educational Resources">
-            <i aria-hidden="true" class="upload icon"></i>
-            {{ _("Upload OER") }}
-          </a>
-        </p>
+        <div class="ui grid">
+          <div class="sixteen wide mobile eight wide computer column">
+            <span>
+              {{ _("Visibility of uploaded content is maximized through synchronization with data hubs (DataCite).") }}
+            </span>
+          </div>
+          <div class="sixteen wide mobile eight wide computer column">
+            <a class="ui fluid positive button" href="me/uploads" title="Research Data">
+              <i aria-hidden="true" class="upload icon"></i>
+              {{ _("Upload Research Output") }}
+            </a>
+          </div>
+          <div class="sixteen wide mobile eight wide computer column">
+            <span>
+              {{ _("Open Educational Resources (OER) will be visible on various discovery tools like the OERhub.") }}
+            </span>
+          </div>
+          <div class="sixteen wide mobile eight wide computer column">
+            <a class="ui fluid positive button" href="lom/uploads" title="Open Educational Resources">
+              <i aria-hidden="true" class="upload icon"></i>
+              {{ _("Upload OER") }}
+            </a>
+          </div>
+        </div>
       </div>
 
       <!--contact us-->
       <div class="ui segment">
         <h4>{{ _("Need help?") }}</h4>
         {%- if config.THEME_TUGRAZ_CONTACT_FORM %}
         <div style="padding-bottom: 10px;">
```

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/macros/authors.html` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/templates/invenio_theme_tugraz/macros/authors.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/templates/invenio_theme_tugraz/navbar.html` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/templates/invenio_theme_tugraz/navbar.html`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/translations/de/LC_MESSAGES/messages.mo` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/translations/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/translations/de/LC_MESSAGES/messages.po` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/translations/messages.pot` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/views.py` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/views.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz/webpack.py` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz/webpack.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz.egg-info/PKG-INFO` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-theme-tugraz
-Version: 4.11.2
+Version: 4.11.3
 Summary: "Invenio module for TUGRAZ theme."
 Home-page: https://github.com/tu-graz-library/invenio-theme-tugraz
 Author: "Graz University of Technology"
 Author-email: mojib.wali@tugraz.at
 License: MIT
 Description: ..
             Copyright (C) 2020-2021 Graz University of Technology.
@@ -58,14 +58,19 @@
             invenio-theme-tugraz is free software; you can redistribute it and/or
             modify it under the terms of the MIT License; see LICENSE file for more
             details.
         
         Changes
         =======
         
+        Version v4.11.3 (release 2023-06-07)
+        
+        - fix: frontpage upload buttons small monitor
+        
+        
         Version v4.11.2 (release 2023-06-01)
         
         - frontpage: layout changes
         - translation: add oer frontpage translation
         - WIP: oer upload button on frontpage
```

### Comparing `invenio-theme-tugraz-4.11.2/invenio_theme_tugraz.egg-info/SOURCES.txt` & `invenio-theme-tugraz-4.11.3/invenio_theme_tugraz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/requirements-devel.txt` & `invenio-theme-tugraz-4.11.3/requirements-devel.txt`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/run-tests.sh` & `invenio-theme-tugraz-4.11.3/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/setup.cfg` & `invenio-theme-tugraz-4.11.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/tests/conftest.py` & `invenio-theme-tugraz-4.11.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-theme-tugraz-4.11.2/tests/test_invenio_theme_tugraz.py` & `invenio-theme-tugraz-4.11.3/tests/test_invenio_theme_tugraz.py`

 * *Files identical despite different names*

