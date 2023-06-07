# Comparing `tmp/bulma_sphinx_theme-0.0.9.tar.gz` & `tmp/bulma_sphinx_theme-0.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bulma_sphinx_theme-0.0.9.tar", last modified: Mon Jun  5 15:13:36 2023, max compression
+gzip compressed data, was "bulma_sphinx_theme-0.1.0rc1.tar", last modified: Wed Jun  7 05:08:57 2023, max compression
```

## Comparing `bulma_sphinx_theme-0.0.9.tar` & `bulma_sphinx_theme-0.1.0rc1.tar`

### file list

```diff
@@ -1,203 +1,202 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:36.541664 bulma_sphinx_theme-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    21234 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/_static/favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/_static/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/admonitions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/blocks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/generic.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/images.rst
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/lists.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/really-long.md
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/sphinx-design.md
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/tables.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/typography.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/mult_headers.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/reference/admonitions.md
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/reference/api.md
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/reference/code-blocks.md
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/reference/hyperlinks.md
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/reference/images.md
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/reference/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/reference/lists.md
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/reference/tables.md
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/reference/tabs.md
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/reference/text-formatting.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/subpages/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/subpages/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/subpages/subpage1.rst
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/subpages/subpage2.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/subpages/subsubpages/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/subpages/subsubpages/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/subpages/subsubpages/subsubpage1.rst
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/subpages/subsubpages/subsubpage2.rst
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/subpages/subsubpages/subsubpage3.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/subpages/subsubpages/subsubsubpages/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/examples/subpages/subsubpages/subsubsubpages/subsubsubpage1.rst
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/user_guide/develop.md
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/user_guide/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/user_guide/navbar.md
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/user_guide/search.md
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/user_guide/sidenav.md
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/user_guide/source.md
--rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/user_guide/theme-elements.md
--rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/docs/user_guide/web-components.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-05 15:13:19.625455 bulma_sphinx_theme-0.0.9/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)   130410 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/package.json
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/postcss.config.js
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.633455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/
--rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)    11169 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/scripts/bulma-sphinx-theme.js
--rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/scripts/gumshoe-patched.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/abstracts/
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/abstracts/_mixins.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/base/
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/base/_icons.scss
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/base/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/base/_typography.scss
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/bulma-sphinx-theme.sass
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/components/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/components/_article-bottom.scss
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/components/_article-top.scss
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/components/_back-to-top.scss
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/components/_brand-logo.scss
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/components/_breadcrumbs.scss
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/components/_edit-page.scss
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/components/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/components/_info-panel.scss
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/components/_last-updated.scss
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/components/_prev-next.scss
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/components/_search-button.scss
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/components/_search-field.sass
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/components/_search-icon.scss
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/components/_search-results.scss
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/components/_search-wrapper.scss
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/components/_search.sass
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/components/_sidenav-brand.scss
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/components/_switcher-theme.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/
--rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_admonitions.scss
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_api.scss
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_blocks.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_code.scss
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_footnotes.sass
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_gui-labels.scss
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_images.sass
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_indexes.sass
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_lists.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_math.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_misc.sass
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_rubrics.sass
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_sidebar.sass
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_tables.sass
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_target.sass
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/extensions/_ablog.scss
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/extensions/_bulma.scss
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/extensions/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/extensions/_leaflet.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/extensions/_notebooks.scss
--rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/extensions/_sphinx-design.scss
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/extensions/_togglebutton.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/sections/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/sections/_bulma-content.scss
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/sections/_bulma-main.scss
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/sections/_bulma-sidenav.scss
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/sections/_bulma-tocnav.scss
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/sections/_footer.scss
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/sections/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/sections/_navbar.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/variables/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/variables/_admonitions.scss
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/variables/_color.scss
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/variables/_definition.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/variables/_fonts.scss
--rw-r--r--   0 runner    (1001) docker     (123)     6907 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/variables/_icons.scss
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/variables/_index.sass
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/variables/_layout.scss
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/variables/_spacing.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/translations/
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/translations/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/translations/jsons/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/translations/jsons/Back to top.json
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/translations/jsons/Edit this page.json
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/translations/jsons/On this page.json
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/translations/jsons/last update.json
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/translations/jsons/with.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/demo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/demo/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/demo/sphinxext.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/pygment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.633455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/back-to-top.html
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/brand-logo.html
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/copyright.html
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/edit-this-page.html
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/icon-links.html
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/info-panel.html
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/last-updated.html
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/navbar-nav.html
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/prev-next.html
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-button.html
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-field.html
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-icon.html
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-wrapper.html
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/searchbox.html
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sidenav-nav.html
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sourcelink.html
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sphinx-version.html
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/theme-swither.html
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/toggle-sidenav.html
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/domainindex.html
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/genindex.html
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/globaltoc.html
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/localtoc.html
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/page.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_css_variables_define.html
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-05 15:13:19.629455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_icon_links_declare.html
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-06-05 15:13:19.633455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/icons.html
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-05 15:13:19.633455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/search.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.633455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-05 15:13:19.633455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-bottom.html
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-05 15:13:19.633455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-top.html
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-05 15:13:19.633455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-05 15:13:19.633455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/headnav.html
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-05 15:13:19.633455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/sidenav.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:13:19.633455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/static/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-05 15:13:19.633455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-05 15:13:19.633455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/theme.conf
--rw-r--r--   0 runner    (1001) docker     (123)    17845 2023-06-05 15:13:19.633455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/toctree.py
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-06-05 15:13:19.633455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-06-05 15:13:19.633455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/translations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-06-05 15:13:19.633455 bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-06-05 15:13:19.633455 bulma_sphinx_theme-0.0.9/webpack.config.js
--rw-r--r--   0        0        0     4450 1970-01-01 00:00:00.000000 bulma_sphinx_theme-0.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:57.788139 bulma_sphinx_theme-0.1.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-07 05:08:39.760347 bulma_sphinx_theme-0.1.0rc1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-07 05:08:39.760347 bulma_sphinx_theme-0.1.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-07 05:08:39.760347 bulma_sphinx_theme-0.1.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-07 05:08:39.760347 bulma_sphinx_theme-0.1.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.760347 bulma_sphinx_theme-0.1.0rc1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    21234 2023-06-07 05:08:39.760347 bulma_sphinx_theme-0.1.0rc1/docs/_static/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-07 05:08:39.760347 bulma_sphinx_theme-0.1.0rc1/docs/_static/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-06-07 05:08:39.760347 bulma_sphinx_theme-0.1.0rc1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-07 05:08:39.760347 bulma_sphinx_theme-0.1.0rc1/docs/examples/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-07 05:08:39.760347 bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/admonitions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/blocks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/generic.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/images.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/lists.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/really-long.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/sphinx-design.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/tables.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/typography.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/mult_headers.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/reference/admonitions.md
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/reference/api.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/reference/code-blocks.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/reference/hyperlinks.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/reference/images.md
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/reference/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/reference/lists.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/reference/tables.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/reference/tabs.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/reference/text-formatting.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/subpages/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/subpages/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/subpages/subpage1.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/subpages/subpage2.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/subpages/subsubpages/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/subpages/subsubpages/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/subpages/subsubpages/subsubpage1.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/subpages/subsubpages/subsubpage2.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/subpages/subsubpages/subsubpage3.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/subpages/subsubpages/subsubsubpages/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/examples/subpages/subsubpages/subsubsubpages/subsubsubpage1.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/user_guide/develop.md
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/user_guide/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/user_guide/navbar.md
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/user_guide/search.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/user_guide/sidenav.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/user_guide/source.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/user_guide/theme-elements.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5423 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/docs/user_guide/web-components.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)   130410 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/postcss.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/
+-rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)    11169 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/scripts/bulma-sphinx-theme.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/scripts/gumshoe-patched.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/abstracts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/abstracts/_mixins.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/base/_icons.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/base/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/base/_typography.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/bulma-sphinx-theme.sass
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/components/_article-bottom.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/components/_article-top.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/components/_back-to-top.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/components/_brand-logo.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/components/_breadcrumbs.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/components/_edit-page.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/components/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/components/_info-panel.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/components/_last-updated.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/components/_prev-next.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/components/_search-button.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/components/_search-field.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/components/_search-icon.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/components/_search-results.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/components/_search-wrapper.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/components/_search.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/components/_sidenav-brand.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/components/_switcher-theme.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/
+-rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_admonitions.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_api.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_blocks.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_code.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_footnotes.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_gui-labels.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_images.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_indexes.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_lists.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_math.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_misc.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_rubrics.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_sidebar.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_tables.sass
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_target.sass
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/extensions/_ablog.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/extensions/_bulma.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/extensions/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/extensions/_leaflet.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/extensions/_notebooks.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/extensions/_sphinx-design.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/extensions/_togglebutton.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/sections/_bulma-content.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-07 05:08:39.764347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/sections/_bulma-main.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/sections/_bulma-sidenav.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/sections/_bulma-tocnav.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/sections/_footer.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/sections/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/sections/_navbar.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/variables/_admonitions.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/variables/_color.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/variables/_fonts.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/variables/_icons.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/variables/_index.sass
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/variables/_layout.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/variables/_spacing.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/translations/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/translations/jsons/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/translations/jsons/Back to top.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/translations/jsons/Edit this page.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/translations/jsons/On this page.json
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/translations/jsons/last update.json
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/translations/jsons/with.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/demo/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/demo/sphinxext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/pygment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/back-to-top.html
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/brand-logo.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/copyright.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/edit-this-page.html
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/icon-links.html
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/info-panel.html
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/last-updated.html
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/navbar-nav.html
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/prev-next.html
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-button.html
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-field.html
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-icon.html
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-wrapper.html
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/searchbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sidenav-nav.html
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sourcelink.html
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/sphinx-version.html
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/theme-swither.html
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/toggle-sidenav.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/domainindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/genindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/globaltoc.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/localtoc.html
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/page.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_css_variables_define.html
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_icon_links_declare.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/icons.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/search.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-bottom.html
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-top.html
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/headnav.html
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/sidenav.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/static/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/theme.conf
+-rw-r--r--   0 runner    (1001) docker     (123)    17845 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/toctree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/translations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-06-07 05:08:39.768347 bulma_sphinx_theme-0.1.0rc1/webpack.config.js
+-rw-r--r--   0        0        0     4453 1970-01-01 00:00:00.000000 bulma_sphinx_theme-0.1.0rc1/PKG-INFO
```

### Comparing `bulma_sphinx_theme-0.0.9/LICENSE` & `bulma_sphinx_theme-0.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/README.md` & `bulma_sphinx_theme-0.1.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/docs/_static/favicon.png` & `bulma_sphinx_theme-0.1.0rc1/docs/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/docs/_static/logo.svg` & `bulma_sphinx_theme-0.1.0rc1/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/docs/conf.py` & `bulma_sphinx_theme-0.1.0rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/docs/examples/index.md` & `bulma_sphinx_theme-0.1.0rc1/docs/examples/index.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/admonitions.rst` & `bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/admonitions.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/api.rst` & `bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/api.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/blocks.rst` & `bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/blocks.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/generic.rst` & `bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/generic.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/images.rst` & `bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/images.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/index.md` & `bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/index.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/lists.rst` & `bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/lists.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/really-long.md` & `bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/really-long.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/sphinx-design.md` & `bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/sphinx-design.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/structure.rst` & `bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/structure.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/tables.rst` & `bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/tables.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/docs/examples/kitchen-sink/typography.rst` & `bulma_sphinx_theme-0.1.0rc1/docs/examples/kitchen-sink/typography.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/docs/examples/mult_headers.rst` & `bulma_sphinx_theme-0.1.0rc1/docs/examples/mult_headers.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/docs/examples/reference/admonitions.md` & `bulma_sphinx_theme-0.1.0rc1/docs/examples/reference/admonitions.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/docs/examples/reference/api.md` & `bulma_sphinx_theme-0.1.0rc1/docs/examples/reference/api.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/docs/examples/reference/code-blocks.md` & `bulma_sphinx_theme-0.1.0rc1/docs/examples/reference/code-blocks.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/docs/examples/reference/hyperlinks.md` & `bulma_sphinx_theme-0.1.0rc1/docs/examples/reference/hyperlinks.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/docs/examples/reference/images.md` & `bulma_sphinx_theme-0.1.0rc1/docs/examples/reference/images.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/docs/examples/reference/index.md` & `bulma_sphinx_theme-0.1.0rc1/docs/examples/reference/index.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/docs/examples/reference/lists.md` & `bulma_sphinx_theme-0.1.0rc1/docs/examples/reference/lists.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/docs/examples/reference/tables.md` & `bulma_sphinx_theme-0.1.0rc1/docs/examples/reference/tables.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/docs/examples/reference/tabs.md` & `bulma_sphinx_theme-0.1.0rc1/docs/examples/reference/tabs.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/docs/examples/reference/text-formatting.md` & `bulma_sphinx_theme-0.1.0rc1/docs/examples/reference/text-formatting.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/docs/examples/subpages/subpage1.rst` & `bulma_sphinx_theme-0.1.0rc1/docs/examples/subpages/subpage1.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/docs/examples/subpages/subpage2.rst` & `bulma_sphinx_theme-0.1.0rc1/docs/examples/subpages/subpage2.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/docs/examples/subpages/subsubpages/subsubpage1.rst` & `bulma_sphinx_theme-0.1.0rc1/docs/examples/subpages/subsubpages/subsubpage1.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/docs/examples/subpages/subsubpages/subsubpage2.rst` & `bulma_sphinx_theme-0.1.0rc1/docs/examples/subpages/subsubpages/subsubpage2.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/docs/examples/subpages/subsubpages/subsubpage3.rst` & `bulma_sphinx_theme-0.1.0rc1/docs/examples/subpages/subsubpages/subsubpage3.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/docs/user_guide/develop.md` & `bulma_sphinx_theme-0.1.0rc1/docs/user_guide/develop.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/docs/user_guide/navbar.md` & `bulma_sphinx_theme-0.1.0rc1/docs/user_guide/navbar.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/docs/user_guide/search.md` & `bulma_sphinx_theme-0.1.0rc1/docs/user_guide/search.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/docs/user_guide/sidenav.md` & `bulma_sphinx_theme-0.1.0rc1/docs/user_guide/sidenav.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/docs/user_guide/source.md` & `bulma_sphinx_theme-0.1.0rc1/docs/user_guide/source.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/docs/user_guide/theme-elements.md` & `bulma_sphinx_theme-0.1.0rc1/docs/user_guide/theme-elements.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/docs/user_guide/web-components.rst` & `bulma_sphinx_theme-0.1.0rc1/docs/user_guide/web-components.rst`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/noxfile.py` & `bulma_sphinx_theme-0.1.0rc1/noxfile.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/package-lock.json` & `bulma_sphinx_theme-0.1.0rc1/package-lock.json`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/package.json` & `bulma_sphinx_theme-0.1.0rc1/package.json`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/pyproject.toml` & `bulma_sphinx_theme-0.1.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/__init__.py` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from functools import lru_cache
 from pathlib import Path
 from typing import Any, Dict, List
 from sphinx.builders.html import StandaloneHTMLBuilder
 from sphinx.locale import get_translation
 from . import pygment, toctree, transforms, utils
 
-__version__ = "0.0.9"
+__version__ = "0.1.0rc1"
 logger = logging.getLogger(__name__)
 MESSAGE_CATALOG_NAME = "bulmasphinxtheme"
 
 
 def _get_html_theme_path():
     """Return list of HTML theme paths."""
     parent = Path(__file__).parent.resolve()
@@ -68,25 +68,33 @@
 def _builder_inited(app: sphinx.application.Sphinx) -> None:
     theme_options = utils.get_theme_options(app)
 
     have_navbar = theme_options.get("have_top_navbar", True)
     if not (have_navbar):
         theme_options["fix_navbar"] = False
 
-    info_include_directly = theme_options.get(
-        "information_panel_include_directly", None
-    )
-    if info_include_directly and isinstance(info_include_directly, list):
-        theme_options["information_panel_include_directly"].extend(
-            info_include_directly
-        )
+    # define navbar style
+    default_navbar_directly = ["navbar-nav.html", "icon-links.html"]
+    navbar_directly = theme_options.get("navbar_include_directly", None)
+    if navbar_directly and isinstance(navbar_directly, list):
+        default_navbar_directly.extend(navbar_directly)
+
+    theme_options["navbar_include_directly"] = default_navbar_directly
+
+    # define information panel
+    default_panel_items = ["search-button.html"]
+    info_panel = theme_options.get("information_panel", {})
+    if info_panel.get("items"):
+        info_panel["items"] = info_panel.get("items")
+    else:
+        info_panel["items"] = default_panel_items
+    if info_panel.get("level_items"):
+        info_panel["level_items"] = info_panel.get("level_items")
 
-    navbar_include_directly = theme_options.get("navbar_include_directly", None)
-    if navbar_include_directly and isinstance(navbar_include_directly, list):
-        theme_options["navbar_include_directly"].extend(navbar_include_directly)
+    theme_options["information_panel"] = info_panel
 
     # Add an analytics ID to the site if provided
     analytics = theme_options.get("analytics", {})
     if analytics:
         # Google Analytics
         gid = analytics.get("google_analytics_id")
 
@@ -118,16 +126,14 @@
         "theme_article_top_left",
         "theme_article_top_right",
         "theme_article_bottom_left",
         "theme_article_bottom_right",
         "theme_navbar_start",
         "theme_navbar_end",
         "theme_navbar_include_directly",
-        "theme_information_panel",
-        "theme_information_panel_include_directly",
         "sidebars",
     ]
 
     for section in template_sections:
         if context.get(section):
             # Break apart `,` separated strings so we can use , in the defaults
             if isinstance(context.get(section), str):
```

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/scripts/bulma-sphinx-theme.js` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/scripts/bulma-sphinx-theme.js`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/scripts/gumshoe-patched.js` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/scripts/gumshoe-patched.js`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/abstracts/_mixins.scss` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/abstracts/_mixins.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/base/_typography.scss` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/base/_typography.scss`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 @use "sass:math";
 
-html,
-body {
+html {
   height: 100%;
+}
+
+body {
+  display: flex;
+  min-height: 100%;
+  flex-direction: column;
   background-color: var(--bst-color-background);
   color: var(--bst-color-text-base);
 }
 
 body,
 button,
 input,
```

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/components/_back-to-top.scss` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/components/_back-to-top.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/components/_prev-next.scss` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/components/_prev-next.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/components/_search-wrapper.scss` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/components/_search-wrapper.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/components/_switcher-theme.scss` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/components/_switcher-theme.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_admonitions.scss` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_admonitions.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_api.scss` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_api.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_code.scss` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_code.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_footnotes.sass` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_footnotes.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_images.sass` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_images.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_lists.scss` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_lists.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_math.scss` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_math.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_misc.sass` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_misc.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_sidebar.sass` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_sidebar.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_tables.sass` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_tables.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/content/_target.sass` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/content/_target.sass`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/extensions/_ablog.scss` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/extensions/_ablog.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/extensions/_notebooks.scss` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/extensions/_notebooks.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/extensions/_sphinx-design.scss` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/extensions/_sphinx-design.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/sections/_bulma-sidenav.scss` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/sections/_bulma-sidenav.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/sections/_bulma-tocnav.scss` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/sections/_bulma-tocnav.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/sections/_navbar.scss` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/sections/_navbar.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/variables/_admonitions.scss` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/variables/_admonitions.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/variables/_color.scss` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/variables/_color.scss`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/styles/variables/_icons.scss` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/styles/variables/_icons.scss`

 * *Files 4% similar despite different names*

```diff
@@ -41,8 +41,10 @@
   @each $name, $glyph in $icons {
     --icon-#{$name}: #{$glyph};
   }
 }
 
 html {
   @include icons;
+  --bst-icon-angle-left: "\f104";
+  --bst-icon-angle-right: "\f105";
 }
```

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/translations/README.md` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/translations/README.md`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/translations/jsons/Edit this page.json` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/translations/jsons/Edit this page.json`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/assets/translations/jsons/On this page.json` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/assets/translations/jsons/On this page.json`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/demo/module.py` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/demo/module.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/demo/sphinxext.py` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/demo/sphinxext.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/pygment.py` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/pygment.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/base.html` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/base.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/breadcrumbs.html` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/edit-this-page.html` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/edit-this-page.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/prev-next.html` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/prev-next.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-button.html` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-button.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-field.html` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/search-field.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/theme-swither.html` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/components/theme-swither.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-<button class="button theme-switch-button icon" title="{{ _('light/dark') }}" aria-label="{{ _('light/dark') }}">
+<button class="button theme-switch-button icon level-item" title="{{ _('light/dark') }}"
+    aria-label="{{ _('light/dark') }}">
     <span class="theme-switch nav-link" data-mode="light">
         <svg class="svg-sun">
             <use href="#svg-sun"></use>
         </svg>
     </span>
     <span class="theme-switch nav-link" data-mode="dark">
         <svg class="svg-moon">
```

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/domainindex.html` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/domainindex.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/genindex.html` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/genindex.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/layout.html` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/layout.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_css_variables_define.html` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_css_variables_define.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_icon_links_declare.html` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/_icon_links_declare.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/icons.html` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/partials/icons.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/search.html` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/search.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-bottom.html` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-bottom.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-top.html` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/article-top.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/headnav.html` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/sections/headnav.html`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/theme.conf` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/theme/bulma_sphinx_theme/theme.conf`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 pygment_light_style = manni
 pygment_dark_style = material
 
 # see https://bulma.io/documentation/components/navbar/#colors for more navbar color styles
 navbar_color_style = is-white
 navbar_start = navbar-nav.html
 navbar_end = theme-swither.html, icon-links.html
-navbar_include_directly = navbar-nav.html, icon-links.html
+navbar_include_directly =
 analytics =
 footer = copyright.html, sphinx-version.html
 toc_title = On this page
 dropdown_label_name = More
 dropdown_label_target_url =
 navigation_with_keys = True
 search_bar_text = Search the docs ...
@@ -39,13 +39,12 @@
 article_bottom_right = sourcelink.html, edit-this-page.html
 use_edit_page_button =
 source_repository =
 source_branch =
 source_directory =
 source_edit_link =
 show_prev_next = True
-information_panel = search-button.html
-information_panel_include_directly = search-button.html, theme-swither.html
+information_panel =
 # define css variables
 light_colors =
 dark_colors =
 css_variables =
```

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/toctree.py` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/toctree.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/transforms.py` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/transforms.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/translations.py` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/translations.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/src/bulma_sphinx_theme/utils.py` & `bulma_sphinx_theme-0.1.0rc1/src/bulma_sphinx_theme/utils.py`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/webpack.config.js` & `bulma_sphinx_theme-0.1.0rc1/webpack.config.js`

 * *Files identical despite different names*

### Comparing `bulma_sphinx_theme-0.0.9/PKG-INFO` & `bulma_sphinx_theme-0.1.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bulma-sphinx-theme
-Version: 0.0.9
+Version: 0.1.0rc1
 Summary: A sphinx theme based on bulma.
 Author-Email: zclab <syfhub@hotmail.com>
 License: MIT License
         
         Copyright (c) 2023 zc
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: bulma-sphinx-theme Version: 0.0.9 Summary: A sphinx
-theme based on bulma. Author-Email: zclab
+Metadata-Version: 2.1 Name: bulma-sphinx-theme Version: 0.1.0rc1 Summary: A
+sphinx theme based on bulma. Author-Email: zclab
 hotmail.com> License: MIT License Copyright (c) 2023 zc Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions: The above copyright notice and this
```

