# Comparing `tmp/shibuya-2023.3.7.tar.gz` & `tmp/shibuya-2023.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shibuya-2023.3.7.tar", last modified: Tue Mar  7 11:43:57 2023, max compression
+gzip compressed data, was "shibuya-2023.6.7.tar", last modified: Wed Jun  7 08:34:53 2023, max compression
```

## Comparing `shibuya-2023.3.7.tar` & `shibuya-2023.6.7.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 11:43:57.496791 shibuya-2023.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-03-07 11:43:43.000000 shibuya-2023.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-03-07 11:43:43.000000 shibuya-2023.3.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-03-07 11:43:57.496791 shibuya-2023.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-03-07 11:43:43.000000 shibuya-2023.3.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-03-07 11:43:43.000000 shibuya-2023.3.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-07 11:43:57.496791 shibuya-2023.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-07 11:43:43.000000 shibuya-2023.3.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 11:43:57.488790 shibuya-2023.3.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 11:43:57.492791 shibuya-2023.3.7/src/shibuya/
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-03-07 11:43:43.000000 shibuya-2023.3.7/src/shibuya/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-03-07 11:43:43.000000 shibuya-2023.3.7/src/shibuya/_sphinx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-03-07 11:43:43.000000 shibuya-2023.3.7/src/shibuya/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 11:43:57.492791 shibuya-2023.3.7/src/shibuya/css/
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-03-07 11:43:43.000000 shibuya-2023.3.7/src/shibuya/css/base.css
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-03-07 11:43:43.000000 shibuya-2023.3.7/src/shibuya/css/dark.css
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-03-07 11:43:43.000000 shibuya-2023.3.7/src/shibuya/css/light.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 11:43:57.488790 shibuya-2023.3.7/src/shibuya/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 11:43:57.492791 shibuya-2023.3.7/src/shibuya/theme/shibuya/
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-03-07 11:43:43.000000 shibuya-2023.3.7/src/shibuya/theme/shibuya/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 11:43:57.492791 shibuya-2023.3.7/src/shibuya/theme/shibuya/components/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-03-07 11:43:43.000000 shibuya-2023.3.7/src/shibuya/theme/shibuya/components/nav-links.html
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-03-07 11:43:43.000000 shibuya-2023.3.7/src/shibuya/theme/shibuya/components/nav-versions.html
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-03-07 11:43:43.000000 shibuya-2023.3.7/src/shibuya/theme/shibuya/components/navigation.html
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-03-07 11:43:43.000000 shibuya-2023.3.7/src/shibuya/theme/shibuya/components/searchbox.html
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-03-07 11:43:43.000000 shibuya-2023.3.7/src/shibuya/theme/shibuya/components/searchbox2.html
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-03-07 11:43:43.000000 shibuya-2023.3.7/src/shibuya/theme/shibuya/components/site-foot.html
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-03-07 11:43:43.000000 shibuya-2023.3.7/src/shibuya/theme/shibuya/components/site-head.html
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-03-07 11:43:43.000000 shibuya-2023.3.7/src/shibuya/theme/shibuya/components/variables.html
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-03-07 11:43:43.000000 shibuya-2023.3.7/src/shibuya/theme/shibuya/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-03-07 11:43:43.000000 shibuya-2023.3.7/src/shibuya/theme/shibuya/page.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 11:43:57.496791 shibuya-2023.3.7/src/shibuya/theme/shibuya/partials/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 11:43:43.000000 shibuya-2023.3.7/src/shibuya/theme/shibuya/partials/article-bottom.html
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-03-07 11:43:43.000000 shibuya-2023.3.7/src/shibuya/theme/shibuya/partials/banner.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 11:43:43.000000 shibuya-2023.3.7/src/shibuya/theme/shibuya/partials/extra-head.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 11:43:43.000000 shibuya-2023.3.7/src/shibuya/theme/shibuya/partials/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-03-07 11:43:43.000000 shibuya-2023.3.7/src/shibuya/theme/shibuya/partials/opengraph.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 11:43:43.000000 shibuya-2023.3.7/src/shibuya/theme/shibuya/partials/page-bottom.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 11:43:43.000000 shibuya-2023.3.7/src/shibuya/theme/shibuya/partials/sidebar-links.html
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-03-07 11:43:43.000000 shibuya-2023.3.7/src/shibuya/theme/shibuya/partials/webfonts.html
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-03-07 11:43:43.000000 shibuya-2023.3.7/src/shibuya/theme/shibuya/search.html
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-03-07 11:43:43.000000 shibuya-2023.3.7/src/shibuya/theme/shibuya/searchbox.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 11:43:57.496791 shibuya-2023.3.7/src/shibuya/theme/shibuya/sidebars/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-03-07 11:43:43.000000 shibuya-2023.3.7/src/shibuya/theme/shibuya/sidebars/edit-this-page.html
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-07 11:43:43.000000 shibuya-2023.3.7/src/shibuya/theme/shibuya/sidebars/ethical-ads.html
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-03-07 11:43:43.000000 shibuya-2023.3.7/src/shibuya/theme/shibuya/sidebars/localtoc.html
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-03-07 11:43:43.000000 shibuya-2023.3.7/src/shibuya/theme/shibuya/sidebars/repo-stats.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 11:43:57.496791 shibuya-2023.3.7/src/shibuya/theme/shibuya/static/
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-03-07 11:43:43.000000 shibuya-2023.3.7/src/shibuya/theme/shibuya/static/print.css
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-03-07 11:43:43.000000 shibuya-2023.3.7/src/shibuya/theme/shibuya/static/pygments.css
--rw-r--r--   0 runner    (1001) docker     (123)    48437 2023-03-07 11:43:48.000000 shibuya-2023.3.7/src/shibuya/theme/shibuya/static/shibuya.css
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-03-07 11:43:46.000000 shibuya-2023.3.7/src/shibuya/theme/shibuya/static/shibuya.js
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-03-07 11:43:43.000000 shibuya-2023.3.7/src/shibuya/theme/shibuya/theme.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 11:43:57.492791 shibuya-2023.3.7/src/shibuya.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-03-07 11:43:57.000000 shibuya-2023.3.7/src/shibuya.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-03-07 11:43:57.000000 shibuya-2023.3.7/src/shibuya.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 11:43:57.000000 shibuya-2023.3.7/src/shibuya.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-07 11:43:57.000000 shibuya-2023.3.7/src/shibuya.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-07 11:43:57.000000 shibuya-2023.3.7/src/shibuya.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-07 11:43:57.000000 shibuya-2023.3.7/src/shibuya.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:34:53.863526 shibuya-2023.6.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-07 08:34:30.000000 shibuya-2023.6.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-07 08:34:30.000000 shibuya-2023.6.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-06-07 08:34:53.863526 shibuya-2023.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-07 08:34:30.000000 shibuya-2023.6.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-07 08:34:30.000000 shibuya-2023.6.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 08:34:53.863526 shibuya-2023.6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-07 08:34:30.000000 shibuya-2023.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:34:53.851526 shibuya-2023.6.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:34:53.855526 shibuya-2023.6.7/src/shibuya/
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-06-07 08:34:30.000000 shibuya-2023.6.7/src/shibuya/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-07 08:34:30.000000 shibuya-2023.6.7/src/shibuya/_sphinx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-06-07 08:34:30.000000 shibuya-2023.6.7/src/shibuya/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:34:53.855526 shibuya-2023.6.7/src/shibuya/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-07 08:34:30.000000 shibuya-2023.6.7/src/shibuya/css/base.css
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-07 08:34:30.000000 shibuya-2023.6.7/src/shibuya/css/dark.css
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-07 08:34:30.000000 shibuya-2023.6.7/src/shibuya/css/light.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:34:53.851526 shibuya-2023.6.7/src/shibuya/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:34:53.855526 shibuya-2023.6.7/src/shibuya/theme/shibuya/
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-06-07 08:34:30.000000 shibuya-2023.6.7/src/shibuya/theme/shibuya/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:34:53.859526 shibuya-2023.6.7/src/shibuya/theme/shibuya/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-07 08:34:30.000000 shibuya-2023.6.7/src/shibuya/theme/shibuya/components/nav-links.html
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-07 08:34:30.000000 shibuya-2023.6.7/src/shibuya/theme/shibuya/components/nav-versions.html
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-07 08:34:30.000000 shibuya-2023.6.7/src/shibuya/theme/shibuya/components/navigation.html
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-07 08:34:30.000000 shibuya-2023.6.7/src/shibuya/theme/shibuya/components/page-searchbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-07 08:34:30.000000 shibuya-2023.6.7/src/shibuya/theme/shibuya/components/searchbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-07 08:34:30.000000 shibuya-2023.6.7/src/shibuya/theme/shibuya/components/site-foot.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-06-07 08:34:30.000000 shibuya-2023.6.7/src/shibuya/theme/shibuya/components/site-head.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-07 08:34:30.000000 shibuya-2023.6.7/src/shibuya/theme/shibuya/components/variables.html
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-07 08:34:30.000000 shibuya-2023.6.7/src/shibuya/theme/shibuya/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-07 08:34:30.000000 shibuya-2023.6.7/src/shibuya/theme/shibuya/page.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:34:53.859526 shibuya-2023.6.7/src/shibuya/theme/shibuya/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:34:30.000000 shibuya-2023.6.7/src/shibuya/theme/shibuya/partials/article-bottom.html
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-07 08:34:30.000000 shibuya-2023.6.7/src/shibuya/theme/shibuya/partials/banner.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:34:30.000000 shibuya-2023.6.7/src/shibuya/theme/shibuya/partials/extra-head.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:34:30.000000 shibuya-2023.6.7/src/shibuya/theme/shibuya/partials/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-07 08:34:30.000000 shibuya-2023.6.7/src/shibuya/theme/shibuya/partials/opengraph.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:34:30.000000 shibuya-2023.6.7/src/shibuya/theme/shibuya/partials/page-bottom.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:34:30.000000 shibuya-2023.6.7/src/shibuya/theme/shibuya/partials/sidebar-links.html
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-07 08:34:30.000000 shibuya-2023.6.7/src/shibuya/theme/shibuya/partials/webfonts.html
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-07 08:34:30.000000 shibuya-2023.6.7/src/shibuya/theme/shibuya/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-07 08:34:30.000000 shibuya-2023.6.7/src/shibuya/theme/shibuya/searchbox.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:34:53.859526 shibuya-2023.6.7/src/shibuya/theme/shibuya/sidebars/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-07 08:34:30.000000 shibuya-2023.6.7/src/shibuya/theme/shibuya/sidebars/edit-this-page.html
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-07 08:34:30.000000 shibuya-2023.6.7/src/shibuya/theme/shibuya/sidebars/ethical-ads.html
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-07 08:34:30.000000 shibuya-2023.6.7/src/shibuya/theme/shibuya/sidebars/localtoc.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-07 08:34:30.000000 shibuya-2023.6.7/src/shibuya/theme/shibuya/sidebars/repo-stats.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:34:53.863526 shibuya-2023.6.7/src/shibuya/theme/shibuya/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-07 08:34:30.000000 shibuya-2023.6.7/src/shibuya/theme/shibuya/static/print.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-06-07 08:34:30.000000 shibuya-2023.6.7/src/shibuya/theme/shibuya/static/pygments.css
+-rw-r--r--   0 runner    (1001) docker     (123)    51450 2023-06-07 08:34:38.000000 shibuya-2023.6.7/src/shibuya/theme/shibuya/static/shibuya.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-06-07 08:34:35.000000 shibuya-2023.6.7/src/shibuya/theme/shibuya/static/shibuya.js
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-07 08:34:30.000000 shibuya-2023.6.7/src/shibuya/theme/shibuya/theme.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:34:53.855526 shibuya-2023.6.7/src/shibuya.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-06-07 08:34:53.000000 shibuya-2023.6.7/src/shibuya.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-07 08:34:53.000000 shibuya-2023.6.7/src/shibuya.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 08:34:53.000000 shibuya-2023.6.7/src/shibuya.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-07 08:34:53.000000 shibuya-2023.6.7/src/shibuya.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-07 08:34:53.000000 shibuya-2023.6.7/src/shibuya.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-07 08:34:53.000000 shibuya-2023.6.7/src/shibuya.egg-info/top_level.txt
```

### Comparing `shibuya-2023.3.7/LICENSE` & `shibuya-2023.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `shibuya-2023.3.7/README.md` & `shibuya-2023.6.7/README.md`

 * *Files identical despite different names*

### Comparing `shibuya-2023.3.7/pyproject.toml` & `shibuya-2023.6.7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 readme = "README.md"
 
 requires-python = ">=3.7"
 dependencies = [
     "Sphinx"
 ]
 
-license = { file = "LICENSE"}
+license = {text = "BSD-3-Clause"}
 authors = [
     {name = "Hsiaoming Yang", email = "me@lepture.com"},
 ]
 classifiers = [
     "Framework :: Sphinx",
     "Framework :: Sphinx :: Theme",
     "Development Status :: 5 - Production/Stable",
```

### Comparing `shibuya-2023.3.7/src/shibuya/__init__.py` & `shibuya-2023.6.7/src/shibuya/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     create_edit_source_link,
 )
 from ._sphinx import (
     WrapperPostTransform,
     WrapLineFormatter,
 )
 
-__version__ = "2023.3.7"
+__version__ = "2023.6.7"
 
 shibuya_version = __version__
 
 THEME_PATH = (Path(__file__).parent / "theme" / "shibuya").resolve()
 
 
 def _add_version(name: str):
```

### Comparing `shibuya-2023.3.7/src/shibuya/_sphinx.py` & `shibuya-2023.6.7/src/shibuya/_sphinx.py`

 * *Files identical despite different names*

### Comparing `shibuya-2023.3.7/src/shibuya/context.py` & `shibuya-2023.6.7/src/shibuya/context.py`

 * *Files 21% similar despite different names*

```diff
@@ -31,52 +31,47 @@
     toc = re.sub(r'^<ul>\n<li>.*?</a>', '', toc)
     toc = re.sub(r'</li>\n</ul>$', '', toc)
     return toc
 
 
 def create_edit_source_link(context: Dict[str, Any]):
     source_type = context.get("source_type")
+    if not source_type:
+        source_type = _normalize_readthedocs_context(context)
+
     source_user = context.get("source_user")
     source_repo = context.get("source_repo")
     source_docs_path = context.get("source_docs_path", "docs")
     source_edit_template = context.get("source_edit_template")
 
-    # extract context from readthe docs
-    if not source_type and "readthedocs" in context:
-        readthedocs = context["readthedocs"]
-        source = _get_readthedocs_vcs(readthedocs)
-        if source:
-            source_type = source.get("type")
-            source_user = source.get("user")
-            source_repo = source.get("repo")
-            source_docs_path = source.get("conf_py_path")
-
-            # add source context
-            context["source_type"] = source_type
-            context["source_user"] = source_user
-            context["source_repo"] = source_repo
-            context["source_docs_path"] = source_docs_path
-
     def edit_source_link(filename: str) -> str:
         if source_edit_template:
             return source_edit_template.format(filename)
 
         if not source_user or not source_repo:
             return
 
         if source_type == "github":
-            return f"https://github.com/{source_user}/{source_repo}/edit/master/{source_docs_path}/{filename}"
+            return f"https://github.com/{source_user}/{source_repo}/blob/master/{source_docs_path}/{filename}"
         elif source_type == "gitlab":
             return f"https://gitlab.com/{source_user}/{source_repo}/-/blob/master/{source_docs_path}/{filename}"
         elif source_type == "bitbucket":
             return  f"https://bitbucket.org/{source_user}/{source_repo}/src/master/{source_docs_path}/{filename}"
 
     return edit_source_link
 
 
-def _get_readthedocs_vcs(data: Dict[str, Any]):
-    if isinstance(readthedocs, dict) and "v1" in readthedocs:
-        readthedocs = readthedocs["v1"]
-        if isinstance(readthedocs, dict) and "vcs" in readthedocs:
-            source = readthedocs["vcs"]
-            if isinstance(source, dict):
-                return source
+def _normalize_readthedocs_context(context: Dict[str, Any]):
+    if context.get("display_github"):
+        source_type = "github"
+    elif context.get("display_gitlab"):
+        source_type = "gitlab"
+    elif context.get("display_bitbucket"):
+        source_type = "bitbucket"
+    else:
+        return
+
+    context["source_type"] = source_type
+    context["source_user"] = context.get(f"{source_type}_user")
+    context["source_repo"] = context.get(f"{source_type}_repo")
+    context["source_docs_path"] = context.get("conf_py_path")
+    return source_type
```

### Comparing `shibuya-2023.3.7/src/shibuya/css/base.css` & `shibuya-2023.6.7/src/shibuya/css/base.css`

 * *Files identical despite different names*

### Comparing `shibuya-2023.3.7/src/shibuya/theme/shibuya/base.html` & `shibuya-2023.6.7/src/shibuya/theme/shibuya/base.html`

 * *Files 14% similar despite different names*

```diff
@@ -38,14 +38,23 @@
       <link rel="prev" title="{{ prev.title|striptags|e }}" href="{{ prev.link|e }}" />
     {%- endif -%}
 
     {%- if pageurl %}
     <link rel="canonical" href="{{ pageurl|e }}" />
     {%- endif %}
   {%- endblock linktags %}
+  <script>
+    const isDarkTheme = window.matchMedia && window.matchMedia('(prefers-color-scheme: dark)').matches;
+    const sessionTheme = sessionStorage['_theme']
+    if (sessionTheme) {
+      document.documentElement.classList.add(sessionTheme)
+    } else if (isDarkTheme) {
+      document.documentElement.classList.add('dark')
+    }
+  </script>
 
   {%- if favicon_url -%}
     <link rel="shortcut icon" href="{{ favicon_url|e }}"/>
   {%- endif %}
 
   {%- block styles -%}
     {%- for css in css_files -%}
```

#### html2text {}

```diff
@@ -7,15 +7,16 @@
 {% endif %} {%- endblock -%} {%- block linktags %} {%- if hasdoc('about') -%}
  {%- endif -%} {%- if hasdoc('genindex') -%}
  {%- endif -%} {%- if hasdoc('search') -%}
  {%- endif -%} {%- if hasdoc('copyright') -%}
  {%- endif -%} {%- if next -%}
  {%- endif -%} {%- if prev -%}
  {%- endif -%} {%- if pageurl %}
- {%- endif %} {%- endblock linktags %} {%- if favicon_url -%}
+ {%- endif %} {%- endblock linktags %}
+ {%- if favicon_url -%}
  {%- endif %} {%- block styles -%} {%- for css in css_files -%} {% if css|attr
 ("filename") -%} {{ css_tag(css) }} {%- else -%}
  {%- endif %} {% endfor -%} {% include "components/variables.html" with context
 %} {% include "partials/webfonts.html" %} {% block theme_styles %}{% endblock
 %} {%- endblock -%} {%- block extrahead %}{% endblock -%} {%- include
 "partials/extra-head.html" -%}
 {%- block document -%}
```

### Comparing `shibuya-2023.3.7/src/shibuya/theme/shibuya/components/navigation.html` & `shibuya-2023.6.7/src/shibuya/theme/shibuya/components/navigation.html`

 * *Files identical despite different names*

### Comparing `shibuya-2023.3.7/src/shibuya/theme/shibuya/components/site-foot.html` & `shibuya-2023.6.7/src/shibuya/theme/shibuya/components/site-foot.html`

 * *Files identical despite different names*

### Comparing `shibuya-2023.3.7/src/shibuya/theme/shibuya/components/site-head.html` & `shibuya-2023.6.7/src/shibuya/theme/shibuya/components/site-head.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,144 +1,154 @@
-00000000: 7b25 2d20 6d61 6372 6f20 7265 6e64 6572  {%- macro render
-00000010: 5f6c 6f67 6f28 7372 632c 2063 6c61 7373  _logo(src, class
-00000020: 6e61 6d65 2920 2d25 7d0a 2020 7b25 2d20  name) -%}.  {%- 
-00000030: 6966 2073 7263 2061 6e64 2073 7263 2e73  if src and src.s
-00000040: 7461 7274 7377 6974 6828 2827 6874 7470  tartswith(('http
-00000050: 733a 2f2f 272c 2027 6874 7470 3a2f 2f27  s://', 'http://'
-00000060: 2929 202d 257d 0a20 2020 203c 696d 6720  )) -%}.    <img 
-00000070: 636c 6173 733d 227b 7b20 636c 6173 736e  class="{{ classn
-00000080: 616d 6520 7d7d 2220 7372 633d 227b 7b20  ame }}" src="{{ 
-00000090: 7372 6320 7d7d 2220 616c 743d 227b 7b20  src }}" alt="{{ 
-000000a0: 7072 6f6a 6563 7420 7d7d 2220 6865 6967  project }}" heig
-000000b0: 6874 3d22 3238 2220 2f3e 0a20 207b 252d  ht="28" />.  {%-
-000000c0: 2065 6c69 6620 7372 6320 2d25 7d0a 2020   elif src -%}.  
-000000d0: 2020 3c69 6d67 2063 6c61 7373 3d22 7b7b    <img class="{{
-000000e0: 2063 6c61 7373 6e61 6d65 207d 7d22 2073   classname }}" s
-000000f0: 7263 3d22 7b7b 2070 6174 6874 6f28 7372  rc="{{ pathto(sr
-00000100: 632c 2031 2920 7d7d 2220 616c 743d 227b  c, 1) }}" alt="{
-00000110: 7b20 7072 6f6a 6563 7420 7d7d 2220 6865  { project }}" he
-00000120: 6967 6874 3d22 3238 2220 2f3e 0a20 207b  ight="28" />.  {
-00000130: 252d 2065 6c69 6620 6c6f 676f 5f75 726c  %- elif logo_url
-00000140: 202d 257d 0a20 2020 203c 696d 6720 636c   -%}.    <img cl
-00000150: 6173 733d 227b 7b20 636c 6173 736e 616d  ass="{{ classnam
-00000160: 6520 7d7d 2220 7372 633d 227b 7b20 6c6f  e }}" src="{{ lo
-00000170: 676f 5f75 726c 207d 7d22 2061 6c74 3d22  go_url }}" alt="
-00000180: 7b7b 2070 726f 6a65 6374 207d 7d22 2068  {{ project }}" h
-00000190: 6569 6768 743d 2232 3822 202f 3e0a 2020  eight="28" />.  
-000001a0: 7b25 2d20 656e 6469 6620 2d25 7d0a 7b25  {%- endif -%}.{%
-000001b0: 2d20 656e 646d 6163 726f 202d 257d 0a0a  - endmacro -%}..
-000001c0: 3c64 6976 2063 6c61 7373 3d22 7379 2d68  <div class="sy-h
-000001d0: 6561 6422 3e0a 2020 3c64 6976 2063 6c61  ead">.  <div cla
-000001e0: 7373 3d22 7379 2d68 6561 642d 626c 7572  ss="sy-head-blur
-000001f0: 223e 3c2f 6469 763e 0a20 203c 6469 7620  "></div>.  <div 
-00000200: 636c 6173 733d 2273 792d 6865 6164 2d69  class="sy-head-i
-00000210: 6e6e 6572 2073 792d 636f 6e74 6169 6e65  nner sy-containe
-00000220: 7220 6d78 2d61 7574 6f22 3e0a 2020 2020  r mx-auto">.    
-00000230: 3c64 6976 2063 6c61 7373 3d22 7379 2d68  <div class="sy-h
-00000240: 6561 642d 6272 616e 6420 666c 6578 2069  ead-brand flex i
-00000250: 7465 6d73 2d63 656e 7465 7222 3e0a 2020  tems-center">.  
-00000260: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-00000270: 6d64 3a68 6964 6465 6e20 666c 6578 2069  md:hidden flex i
-00000280: 7465 6d73 2d63 656e 7465 7222 3e0a 2020  tems-center">.  
-00000290: 2020 2020 2020 3c62 7574 746f 6e20 636c        <button cl
-000002a0: 6173 733d 2268 616d 6275 7267 6572 206a  ass="hamburger j
-000002b0: 732d 6d65 6e75 206d 722d 3322 2061 7269  s-menu mr-3" ari
-000002c0: 612d 6c61 6265 6c3d 224d 656e 7522 2074  a-label="Menu" t
-000002d0: 7970 653d 2262 7574 746f 6e22 2061 7269  ype="button" ari
-000002e0: 612d 636f 6e74 726f 6c73 3d22 6c73 6964  a-controls="lsid
-000002f0: 6522 2061 7269 612d 6578 7061 6e64 6564  e" aria-expanded
-00000300: 3d22 6661 6c73 6522 3e0a 2020 2020 2020  ="false">.      
-00000310: 2020 2020 3c73 7061 6e20 636c 6173 733d      <span class=
-00000320: 2268 616d 6275 7267 6572 5f31 223e 3c2f  "hamburger_1"></
-00000330: 7370 616e 3e0a 2020 2020 2020 2020 2020  span>.          
-00000340: 3c73 7061 6e20 636c 6173 733d 2268 616d  <span class="ham
-00000350: 6275 7267 6572 5f32 202d 7472 616e 736c  burger_2 -transl
-00000360: 6174 652d 782d 3222 3e3c 2f73 7061 6e3e  ate-x-2"></span>
-00000370: 0a20 2020 2020 2020 2020 203c 7370 616e  .          <span
-00000380: 2063 6c61 7373 3d22 6861 6d62 7572 6765   class="hamburge
-00000390: 725f 3320 2d74 7261 6e73 6c61 7465 2d78  r_3 -translate-x
-000003a0: 2d31 223e 3c2f 7370 616e 3e0a 2020 2020  -1"></span>.    
-000003b0: 2020 2020 3c2f 6275 7474 6f6e 3e0a 2020      </button>.  
-000003c0: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
-000003d0: 203c 6120 6872 6566 3d22 7b25 2069 6620   <a href="{% if 
-000003e0: 7468 656d 655f 6c6f 676f 5f74 6172 6765  theme_logo_targe
-000003f0: 7420 257d 7b7b 2074 6865 6d65 5f6c 6f67  t %}{{ theme_log
-00000400: 6f5f 7461 7267 6574 207d 7d7b 2520 656c  o_target }}{% el
-00000410: 7365 2025 7d7b 7b20 7061 7468 746f 2872  se %}{{ pathto(r
-00000420: 6f6f 745f 646f 6329 207d 7d7b 2520 656e  oot_doc) }}{% en
-00000430: 6469 6620 257d 223e 0a20 2020 2020 2020  dif %}">.       
-00000440: 207b 7b20 7265 6e64 6572 5f6c 6f67 6f28   {{ render_logo(
-00000450: 7468 656d 655f 6c69 6768 745f 6c6f 676f  theme_light_logo
-00000460: 2c20 276c 6967 6874 2d6c 6f67 6f27 2920  , 'light-logo') 
-00000470: 7d7d 0a20 2020 2020 2020 207b 7b20 7265  }}.        {{ re
-00000480: 6e64 6572 5f6c 6f67 6f28 7468 656d 655f  nder_logo(theme_
-00000490: 6461 726b 5f6c 6f67 6f2c 2027 6461 726b  dark_logo, 'dark
-000004a0: 2d6c 6f67 6f27 2920 7d7d 0a20 2020 2020  -logo') }}.     
-000004b0: 2020 203c 7374 726f 6e67 3e7b 7b20 7072     <strong>{{ pr
-000004c0: 6f6a 6563 7420 7d7d 3c2f 7374 726f 6e67  oject }}</strong
-000004d0: 3e0a 2020 2020 2020 3c2f 613e 0a20 2020  >.      </a>.   
-000004e0: 2020 207b 2520 696e 636c 7564 6520 2263     {% include "c
-000004f0: 6f6d 706f 6e65 6e74 732f 6e61 762d 7665  omponents/nav-ve
-00000500: 7273 696f 6e73 2e68 746d 6c22 2025 7d0a  rsions.html" %}.
-00000510: 2020 2020 3c2f 6469 763e 0a20 2020 203c      </div>.    <
-00000520: 6469 7620 636c 6173 733d 2273 792d 6865  div class="sy-he
-00000530: 6164 2d61 6374 696f 6e73 2066 6c65 7820  ad-actions flex 
-00000540: 6761 702d 3220 6974 656d 732d 6365 6e74  gap-2 items-cent
-00000550: 6572 2070 7269 6e74 3a68 6964 6465 6e22  er print:hidden"
-00000560: 3e0a 2020 2020 2020 3c6e 6176 2063 6c61  >.      <nav cla
-00000570: 7373 3d22 7379 2d68 6561 642d 6e61 7620  ss="sy-head-nav 
-00000580: 6869 6464 656e 206d 643a 626c 6f63 6b22  hidden md:block"
-00000590: 3e0a 2020 2020 2020 2020 7b25 2d20 696e  >.        {%- in
-000005a0: 636c 7564 6520 2263 6f6d 706f 6e65 6e74  clude "component
-000005b0: 732f 6e61 762d 6c69 6e6b 732e 6874 6d6c  s/nav-links.html
-000005c0: 2220 257d 0a20 2020 2020 203c 2f6e 6176  " %}.      </nav
-000005d0: 3e0a 2020 2020 2020 3c64 6976 2063 6c61  >.      <div cla
-000005e0: 7373 3d22 6869 6464 656e 206d 643a 626c  ss="hidden md:bl
-000005f0: 6f63 6b22 3e0a 2020 2020 2020 2020 7b25  ock">.        {%
-00000600: 2d20 696e 636c 7564 6520 2263 6f6d 706f  - include "compo
-00000610: 6e65 6e74 732f 7365 6172 6368 626f 782e  nents/searchbox.
-00000620: 6874 6d6c 2220 257d 0a20 2020 2020 203c  html" %}.      <
-00000630: 2f64 6976 3e0a 2020 2020 2020 7b25 2d20  /div>.      {%- 
-00000640: 6966 2074 6865 6d65 5f67 6974 6875 625f  if theme_github_
-00000650: 7572 6c20 257d 0a20 2020 2020 2020 203c  url %}.        <
-00000660: 6120 636c 6173 733d 2266 6c65 7820 6974  a class="flex it
-00000670: 656d 732d 6365 6e74 6572 206d 6c2d 3122  ems-center ml-1"
-00000680: 2068 7265 663d 227b 7b20 7468 656d 655f   href="{{ theme_
-00000690: 6769 7468 7562 5f75 726c 207d 7d22 2061  github_url }}" a
-000006a0: 7269 612d 6c61 6265 6c3d 2247 6974 4875  ria-label="GitHu
-000006b0: 6222 3e0a 2020 2020 2020 2020 2020 3c69  b">.          <i
-000006c0: 2063 6c61 7373 3d22 692d 6963 6f6e 2067   class="i-icon g
-000006d0: 6974 6875 6222 3e3c 2f69 3e0a 2020 2020  ithub"></i>.    
-000006e0: 2020 2020 3c2f 613e 0a20 2020 2020 207b      </a>.      {
-000006f0: 252d 2065 6e64 6966 2025 7d0a 2020 2020  %- endif %}.    
-00000700: 2020 3c62 7574 746f 6e20 636c 6173 733d    <button class=
-00000710: 226a 732d 7468 656d 6520 7468 656d 652d  "js-theme theme-
-00000720: 7377 6974 6368 2066 6c65 7820 6974 656d  switch flex item
-00000730: 732d 6365 6e74 6572 206d 6c2d 3122 2064  s-center ml-1" d
-00000740: 6174 612d 6172 6961 2d6c 6967 6874 3d22  ata-aria-light="
-00000750: 7b7b 205f 2827 5377 6974 6368 2074 6f20  {{ _('Switch to 
-00000760: 6461 726b 206d 6f64 6527 2920 7d7d 2220  dark mode') }}" 
-00000770: 6461 7461 2d61 7269 612d 6461 726b 3d22  data-aria-dark="
-00000780: 7b7b 205f 2827 5377 6974 6368 2074 6f20  {{ _('Switch to 
-00000790: 6c69 6768 7420 6d6f 6465 2729 207d 7d22  light mode') }}"
-000007a0: 3e0a 2020 2020 2020 2020 3c69 2063 6c61  >.        <i cla
-000007b0: 7373 3d22 692d 6963 6f6e 2074 6865 6d65  ss="i-icon theme
-000007c0: 2d69 636f 6e22 3e3c 2f69 3e0a 2020 2020  -icon"></i>.    
-000007d0: 2020 3c2f 6275 7474 6f6e 3e0a 2020 2020    </button>.    
-000007e0: 2020 7b25 2069 6620 6469 7370 6c61 795f    {% if display_
-000007f0: 746f 6320 257d 0a20 2020 2020 2020 203c  toc %}.        <
-00000800: 6275 7474 6f6e 2063 6c61 7373 3d22 6a73  button class="js
-00000810: 2d6d 656e 7520 786c 3a68 6964 6465 6e20  -menu xl:hidden 
-00000820: 666c 6578 2069 7465 6d73 2d63 656e 7465  flex items-cente
-00000830: 7220 6d6c 2d31 2220 6172 6961 2d6c 6162  r ml-1" aria-lab
-00000840: 656c 3d22 5368 6f77 2074 6162 6c65 206f  el="Show table o
-00000850: 6620 636f 6e74 656e 7473 2220 7479 7065  f contents" type
-00000860: 3d22 6275 7474 6f6e 2220 6172 6961 2d63  ="button" aria-c
-00000870: 6f6e 7472 6f6c 733d 2272 7369 6465 2220  ontrols="rside" 
-00000880: 6172 6961 2d65 7870 616e 6465 643d 2266  aria-expanded="f
-00000890: 616c 7365 223e 0a20 2020 2020 2020 2020  alse">.         
-000008a0: 203c 6920 636c 6173 733d 2269 2d69 636f   <i class="i-ico
-000008b0: 6e20 6f75 7464 656e 7422 3e3c 2f69 3e0a  n outdent"></i>.
-000008c0: 2020 2020 2020 2020 3c2f 6275 7474 6f6e          </button
-000008d0: 3e0a 2020 2020 2020 7b25 2d20 656e 6469  >.      {%- endi
-000008e0: 6620 257d 0a20 2020 203c 2f64 6976 3e0a  f %}.    </div>.
-000008f0: 2020 3c2f 6469 763e 0a3c 2f64 6976 3e0a    </div>.</div>.
+00000000: 7b25 2d20 6672 6f6d 2022 636f 6d70 6f6e  {%- from "compon
+00000010: 656e 7473 2f6e 6176 2d6c 696e 6b73 2e68  ents/nav-links.h
+00000020: 746d 6c22 2069 6d70 6f72 7420 7265 6e64  tml" import rend
+00000030: 6572 4e61 764c 696e 6b73 2077 6974 6820  erNavLinks with 
+00000040: 636f 6e74 6578 7420 2d25 7d0a 0a7b 252d  context -%}..{%-
+00000050: 206d 6163 726f 2072 656e 6465 725f 6c6f   macro render_lo
+00000060: 676f 2873 7263 2c20 636c 6173 736e 616d  go(src, classnam
+00000070: 6529 202d 257d 0a20 207b 252d 2069 6620  e) -%}.  {%- if 
+00000080: 7372 6320 616e 6420 7372 632e 7374 6172  src and src.star
+00000090: 7473 7769 7468 2828 2768 7474 7073 3a2f  tswith(('https:/
+000000a0: 2f27 2c20 2768 7474 703a 2f2f 2729 2920  /', 'http://')) 
+000000b0: 2d25 7d0a 2020 2020 3c69 6d67 2063 6c61  -%}.    <img cla
+000000c0: 7373 3d22 7b7b 2063 6c61 7373 6e61 6d65  ss="{{ classname
+000000d0: 207d 7d22 2073 7263 3d22 7b7b 2073 7263   }}" src="{{ src
+000000e0: 207d 7d22 2061 6c74 3d22 7b7b 2070 726f   }}" alt="{{ pro
+000000f0: 6a65 6374 207d 7d22 2068 6569 6768 743d  ject }}" height=
+00000100: 2232 3822 202f 3e0a 2020 7b25 2d20 656c  "28" />.  {%- el
+00000110: 6966 2073 7263 202d 257d 0a20 2020 203c  if src -%}.    <
+00000120: 696d 6720 636c 6173 733d 227b 7b20 636c  img class="{{ cl
+00000130: 6173 736e 616d 6520 7d7d 2220 7372 633d  assname }}" src=
+00000140: 227b 7b20 7061 7468 746f 2873 7263 2c20  "{{ pathto(src, 
+00000150: 3129 207d 7d22 2061 6c74 3d22 7b7b 2070  1) }}" alt="{{ p
+00000160: 726f 6a65 6374 207d 7d22 2068 6569 6768  roject }}" heigh
+00000170: 743d 2232 3822 202f 3e0a 2020 7b25 2d20  t="28" />.  {%- 
+00000180: 656c 6966 206c 6f67 6f5f 7572 6c20 2d25  elif logo_url -%
+00000190: 7d0a 2020 2020 3c69 6d67 2063 6c61 7373  }.    <img class
+000001a0: 3d22 7b7b 2063 6c61 7373 6e61 6d65 207d  ="{{ classname }
+000001b0: 7d22 2073 7263 3d22 7b7b 206c 6f67 6f5f  }" src="{{ logo_
+000001c0: 7572 6c20 7d7d 2220 616c 743d 227b 7b20  url }}" alt="{{ 
+000001d0: 7072 6f6a 6563 7420 7d7d 2220 6865 6967  project }}" heig
+000001e0: 6874 3d22 3238 2220 2f3e 0a20 207b 252d  ht="28" />.  {%-
+000001f0: 2065 6e64 6966 202d 257d 0a7b 252d 2065   endif -%}.{%- e
+00000200: 6e64 6d61 6372 6f20 2d25 7d0a 0a3c 6469  ndmacro -%}..<di
+00000210: 7620 636c 6173 733d 2273 792d 6865 6164  v class="sy-head
+00000220: 223e 0a20 203c 6469 7620 636c 6173 733d  ">.  <div class=
+00000230: 2273 792d 6865 6164 2d62 6c75 7222 3e3c  "sy-head-blur"><
+00000240: 2f64 6976 3e0a 2020 3c64 6976 2063 6c61  /div>.  <div cla
+00000250: 7373 3d22 7379 2d68 6561 642d 696e 6e65  ss="sy-head-inne
+00000260: 7220 7379 2d63 6f6e 7461 696e 6572 206d  r sy-container m
+00000270: 782d 6175 746f 223e 0a20 2020 203c 6469  x-auto">.    <di
+00000280: 7620 636c 6173 733d 2273 792d 6865 6164  v class="sy-head
+00000290: 2d6c 696e 6b73 2066 6c65 7820 6974 656d  -links flex item
+000002a0: 732d 6365 6e74 6572 223e 0a20 2020 2020  s-center">.     
+000002b0: 203c 6469 7620 636c 6173 733d 226d 643a   <div class="md:
+000002c0: 6869 6464 656e 2066 6c65 7820 6974 656d  hidden flex item
+000002d0: 732d 6365 6e74 6572 223e 0a20 2020 2020  s-center">.     
+000002e0: 2020 203c 6275 7474 6f6e 2063 6c61 7373     <button class
+000002f0: 3d22 6861 6d62 7572 6765 7220 6a73 2d6d  ="hamburger js-m
+00000300: 656e 7520 6d72 2d33 2220 6172 6961 2d6c  enu mr-3" aria-l
+00000310: 6162 656c 3d22 4d65 6e75 2220 7479 7065  abel="Menu" type
+00000320: 3d22 6275 7474 6f6e 2220 6172 6961 2d63  ="button" aria-c
+00000330: 6f6e 7472 6f6c 733d 226c 7369 6465 2220  ontrols="lside" 
+00000340: 6172 6961 2d65 7870 616e 6465 643d 2266  aria-expanded="f
+00000350: 616c 7365 223e 0a20 2020 2020 2020 2020  alse">.         
+00000360: 203c 7370 616e 2063 6c61 7373 3d22 6861   <span class="ha
+00000370: 6d62 7572 6765 725f 3122 3e3c 2f73 7061  mburger_1"></spa
+00000380: 6e3e 0a20 2020 2020 2020 2020 203c 7370  n>.          <sp
+00000390: 616e 2063 6c61 7373 3d22 6861 6d62 7572  an class="hambur
+000003a0: 6765 725f 3220 2d74 7261 6e73 6c61 7465  ger_2 -translate
+000003b0: 2d78 2d32 223e 3c2f 7370 616e 3e0a 2020  -x-2"></span>.  
+000003c0: 2020 2020 2020 2020 3c73 7061 6e20 636c          <span cl
+000003d0: 6173 733d 2268 616d 6275 7267 6572 5f33  ass="hamburger_3
+000003e0: 202d 7472 616e 736c 6174 652d 782d 3122   -translate-x-1"
+000003f0: 3e3c 2f73 7061 6e3e 0a20 2020 2020 2020  ></span>.       
+00000400: 203c 2f62 7574 746f 6e3e 0a20 2020 2020   </button>.     
+00000410: 203c 2f64 6976 3e0a 2020 2020 2020 3c61   </div>.      <a
+00000420: 2063 6c61 7373 3d22 7379 2d68 6561 642d   class="sy-head-
+00000430: 6272 616e 6422 2068 7265 663d 227b 2520  brand" href="{% 
+00000440: 6966 2074 6865 6d65 5f6c 6f67 6f5f 7461  if theme_logo_ta
+00000450: 7267 6574 2025 7d7b 7b20 7468 656d 655f  rget %}{{ theme_
+00000460: 6c6f 676f 5f74 6172 6765 7420 7d7d 7b25  logo_target }}{%
+00000470: 2065 6c73 6520 257d 7b7b 2070 6174 6874   else %}{{ patht
+00000480: 6f28 726f 6f74 5f64 6f63 2920 7d7d 7b25  o(root_doc) }}{%
+00000490: 2065 6e64 6966 2025 7d22 3e0a 2020 2020   endif %}">.    
+000004a0: 2020 2020 7b7b 2072 656e 6465 725f 6c6f      {{ render_lo
+000004b0: 676f 2874 6865 6d65 5f6c 6967 6874 5f6c  go(theme_light_l
+000004c0: 6f67 6f2c 2027 6c69 6768 742d 6c6f 676f  ogo, 'light-logo
+000004d0: 2729 207d 7d0a 2020 2020 2020 2020 7b7b  ') }}.        {{
+000004e0: 2072 656e 6465 725f 6c6f 676f 2874 6865   render_logo(the
+000004f0: 6d65 5f64 6172 6b5f 6c6f 676f 2c20 2764  me_dark_logo, 'd
+00000500: 6172 6b2d 6c6f 676f 2729 207d 7d0a 2020  ark-logo') }}.  
+00000510: 2020 2020 2020 3c73 7472 6f6e 673e 7b7b        <strong>{{
+00000520: 2070 726f 6a65 6374 207d 7d3c 2f73 7472   project }}</str
+00000530: 6f6e 673e 0a20 2020 2020 203c 2f61 3e0a  ong>.      </a>.
+00000540: 2020 2020 2020 7b25 2d20 6966 2074 6865        {%- if the
+00000550: 6d65 5f6e 6176 5f6c 696e 6b73 202d 257d  me_nav_links -%}
+00000560: 0a20 2020 2020 203c 6e61 7620 636c 6173  .      <nav clas
+00000570: 733d 2273 792d 6865 6164 2d6e 6176 206d  s="sy-head-nav m
+00000580: 6c2d 3420 6869 6464 656e 206d 643a 626c  l-4 hidden md:bl
+00000590: 6f63 6b22 3e0a 2020 2020 2020 2020 7b7b  ock">.        {{
+000005a0: 2072 656e 6465 724e 6176 4c69 6e6b 7328   renderNavLinks(
+000005b0: 7468 656d 655f 6e61 765f 6c69 6e6b 732c  theme_nav_links,
+000005c0: 2054 7275 6529 207d 7d0a 2020 2020 2020   True) }}.      
+000005d0: 3c2f 6e61 763e 0a20 2020 2020 207b 252d  </nav>.      {%-
+000005e0: 2065 6e64 6966 202d 257d 0a20 2020 203c   endif -%}.    <
+000005f0: 2f64 6976 3e0a 2020 2020 3c64 6976 2063  /div>.    <div c
+00000600: 6c61 7373 3d22 7379 2d68 6561 642d 6163  lass="sy-head-ac
+00000610: 7469 6f6e 7320 666c 6578 2067 6170 2d32  tions flex gap-2
+00000620: 2069 7465 6d73 2d63 656e 7465 7220 7072   items-center pr
+00000630: 696e 743a 6869 6464 656e 223e 0a20 2020  int:hidden">.   
+00000640: 2020 207b 2520 696e 636c 7564 6520 2263     {% include "c
+00000650: 6f6d 706f 6e65 6e74 732f 6e61 762d 7665  omponents/nav-ve
+00000660: 7273 696f 6e73 2e68 746d 6c22 2025 7d0a  rsions.html" %}.
+00000670: 2020 2020 2020 3c64 6976 2063 6c61 7373        <div class
+00000680: 3d22 6869 6464 656e 206d 643a 626c 6f63  ="hidden md:bloc
+00000690: 6b22 3e0a 2020 2020 2020 2020 7b25 2d20  k">.        {%- 
+000006a0: 696e 636c 7564 6520 2263 6f6d 706f 6e65  include "compone
+000006b0: 6e74 732f 7365 6172 6368 626f 782e 6874  nts/searchbox.ht
+000006c0: 6d6c 2220 257d 0a20 2020 2020 203c 2f64  ml" %}.      </d
+000006d0: 6976 3e0a 2020 2020 2020 7b25 2d20 6966  iv>.      {%- if
+000006e0: 2074 6865 6d65 5f67 6974 6875 625f 7572   theme_github_ur
+000006f0: 6c20 257d 0a20 2020 2020 2020 203c 6120  l %}.        <a 
+00000700: 636c 6173 733d 2266 6c65 7820 6974 656d  class="flex item
+00000710: 732d 6365 6e74 6572 206d 6c2d 3122 2068  s-center ml-1" h
+00000720: 7265 663d 227b 7b20 7468 656d 655f 6769  ref="{{ theme_gi
+00000730: 7468 7562 5f75 726c 207d 7d22 2061 7269  thub_url }}" ari
+00000740: 612d 6c61 6265 6c3d 2247 6974 4875 6222  a-label="GitHub"
+00000750: 3e0a 2020 2020 2020 2020 2020 3c69 2063  >.          <i c
+00000760: 6c61 7373 3d22 692d 6963 6f6e 2067 6974  lass="i-icon git
+00000770: 6875 6222 3e3c 2f69 3e0a 2020 2020 2020  hub"></i>.      
+00000780: 2020 3c2f 613e 0a20 2020 2020 207b 252d    </a>.      {%-
+00000790: 2065 6e64 6966 2025 7d0a 2020 2020 2020   endif %}.      
+000007a0: 3c62 7574 746f 6e20 636c 6173 733d 226a  <button class="j
+000007b0: 732d 7468 656d 6520 7468 656d 652d 7377  s-theme theme-sw
+000007c0: 6974 6368 2066 6c65 7820 6974 656d 732d  itch flex items-
+000007d0: 6365 6e74 6572 206d 6c2d 3122 2064 6174  center ml-1" dat
+000007e0: 612d 6172 6961 2d6c 6967 6874 3d22 7b7b  a-aria-light="{{
+000007f0: 205f 2827 5377 6974 6368 2074 6f20 6461   _('Switch to da
+00000800: 726b 206d 6f64 6527 2920 7d7d 2220 6461  rk mode') }}" da
+00000810: 7461 2d61 7269 612d 6461 726b 3d22 7b7b  ta-aria-dark="{{
+00000820: 205f 2827 5377 6974 6368 2074 6f20 6c69   _('Switch to li
+00000830: 6768 7420 6d6f 6465 2729 207d 7d22 3e0a  ght mode') }}">.
+00000840: 2020 2020 2020 2020 3c69 2063 6c61 7373          <i class
+00000850: 3d22 692d 6963 6f6e 2074 6865 6d65 2d69  ="i-icon theme-i
+00000860: 636f 6e22 3e3c 2f69 3e0a 2020 2020 2020  con"></i>.      
+00000870: 3c2f 6275 7474 6f6e 3e0a 2020 2020 2020  </button>.      
+00000880: 7b25 2069 6620 6469 7370 6c61 795f 746f  {% if display_to
+00000890: 6320 257d 0a20 2020 2020 2020 203c 6275  c %}.        <bu
+000008a0: 7474 6f6e 2063 6c61 7373 3d22 6a73 2d6d  tton class="js-m
+000008b0: 656e 7520 786c 3a68 6964 6465 6e20 666c  enu xl:hidden fl
+000008c0: 6578 2069 7465 6d73 2d63 656e 7465 7220  ex items-center 
+000008d0: 6d6c 2d31 2220 6172 6961 2d6c 6162 656c  ml-1" aria-label
+000008e0: 3d22 5368 6f77 2074 6162 6c65 206f 6620  ="Show table of 
+000008f0: 636f 6e74 656e 7473 2220 7479 7065 3d22  contents" type="
+00000900: 6275 7474 6f6e 2220 6172 6961 2d63 6f6e  button" aria-con
+00000910: 7472 6f6c 733d 2272 7369 6465 2220 6172  trols="rside" ar
+00000920: 6961 2d65 7870 616e 6465 643d 2266 616c  ia-expanded="fal
+00000930: 7365 223e 0a20 2020 2020 2020 2020 203c  se">.          <
+00000940: 6920 636c 6173 733d 2269 2d69 636f 6e20  i class="i-icon 
+00000950: 6f75 7464 656e 7422 3e3c 2f69 3e0a 2020  outdent"></i>.  
+00000960: 2020 2020 2020 3c2f 6275 7474 6f6e 3e0a        </button>.
+00000970: 2020 2020 2020 7b25 2d20 656e 6469 6620        {%- endif 
+00000980: 257d 0a20 2020 203c 2f64 6976 3e0a 2020  %}.    </div>.  
+00000990: 3c2f 6469 763e 0a3c 2f64 6976 3e0a       </div>.</div>.
```

### Comparing `shibuya-2023.3.7/src/shibuya/theme/shibuya/components/variables.html` & `shibuya-2023.6.7/src/shibuya/theme/shibuya/components/variables.html`

 * *Files 26% similar despite different names*

```diff
@@ -15,16 +15,24 @@
 {%- endmacro -%}
 
 <style>
 :root {
   {{ declare_css_vars(shibuya_base_css_variables, theme_base_css_variables) }}
   {{ declare_css_vars(shibuya_light_css_variables, theme_light_css_variables) }}
 }
-@media not print {
-  html.light {
+@media (prefers-color-scheme: light) {
+  :root {
     {{ declare_css_vars(shibuya_light_css_variables, theme_light_css_variables) }}
   }
-  html.dark {
+}
+@media (prefers-color-scheme: dark) {
+  :root {
     {{ declare_css_vars(shibuya_dark_css_variables, theme_light_css_variables) }}
   }
 }
+html.light {
+  {{ declare_css_vars(shibuya_light_css_variables, theme_light_css_variables) }}
+}
+html.dark {
+  {{ declare_css_vars(shibuya_dark_css_variables, theme_light_css_variables) }}
+}
 </style>
```

### Comparing `shibuya-2023.3.7/src/shibuya/theme/shibuya/layout.html` & `shibuya-2023.6.7/src/shibuya/theme/shibuya/layout.html`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 {%- extends "base.html" -%}
+{%- from "components/nav-links.html" import renderNavLinks with context -%}
 
 {%- block document -%}
 <div class="document">
   {%- include "partials/banner.html" -%}
   {%- block header -%}
     {% include "components/site-head.html" with context %}
   {%- endblock -%}
 
   <aside id="lside" class="md:hidden">
     {%- block mobile_navbar -%}
       <div class="pt-6 px-6">
         {%- include "components/searchbox.html" %}
       </div>
+      {%- if theme_nav_links -%}
       <div class="pt-3 px-6">
-        {%- include "components/nav-links.html" %}
+        {{ renderNavLinks(theme_nav_links) }}
       </div>
+      {%- endif -%}
     {%- endblock %}
   </aside>
 
   <div class="sy-container mx-auto">
     <main class="sy-content mx-auto pt-12 px-6 xl:px-12 break-words">
       <article class="yue" role="main">
         {% block body %}{% endblock %}
```

### Comparing `shibuya-2023.3.7/src/shibuya/theme/shibuya/page.html` & `shibuya-2023.6.7/src/shibuya/theme/shibuya/page.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 {% extends "base.html" %}
+{%- from "components/nav-links.html" import renderNavLinks with context -%}
 
 {%- block extrahead -%}
   {% include "partials/opengraph.html" %}
 {%- endblock -%}
 
 {%- if meta and meta.dark_code == "true" -%}
   {% set dark_code = True %}
@@ -11,20 +12,24 @@
 {%- else -%}
   {% set dark_code = False %}
 {%- endif -%}
 
 {% block body %}
 <div class="sy-page sy-container flex mx-auto">
   <aside id="lside" class="sy-lside md:w-64 md:shrink-0 print:hidden">
-    <div class="sy-lside-inner md:sticky md:top-16">
-      <div class="md:hidden pt-6 px-6">
-        {%- include "components/searchbox2.html" %}
-      </div>
-      <div class="md:hidden pt-3 px-6">
-        {%- include "components/nav-links.html" %}
+    <div class="sy-lside-inner md:sticky">
+      <div class="sy-lside-top md:hidden pt-3 pb-3 px-6">
+        <div class="pt-3">
+          {%- include "components/page-searchbox.html" %}
+        </div>
+        {%- if theme_nav_links -%}
+        <div class="pt-3">
+          {{ renderNavLinks(theme_nav_links) }}
+        </div>
+        {%- endif -%}
       </div>
       <div class="sy-scrollbar p-6">
         {%- include "partials/sidebar-links.html" %}
         <div class="globaltoc">
           {{ toctree(collapse=False, titles_only=True, includehidden=True) }}
         </div>
       </div>
```

### Comparing `shibuya-2023.3.7/src/shibuya/theme/shibuya/partials/opengraph.html` & `shibuya-2023.6.7/src/shibuya/theme/shibuya/partials/opengraph.html`

 * *Files identical despite different names*

### Comparing `shibuya-2023.3.7/src/shibuya/theme/shibuya/sidebars/repo-stats.html` & `shibuya-2023.6.7/src/shibuya/theme/shibuya/sidebars/repo-stats.html`

 * *Files identical despite different names*

### Comparing `shibuya-2023.3.7/src/shibuya/theme/shibuya/static/pygments.css` & `shibuya-2023.6.7/src/shibuya/theme/shibuya/static/pygments.css`

 * *Files identical despite different names*

### Comparing `shibuya-2023.3.7/src/shibuya/theme/shibuya/static/shibuya.css` & `shibuya-2023.6.7/src/shibuya/theme/shibuya/static/shibuya.css`

 * *Files 4% similar despite different names*

```diff
@@ -1 +1 @@
-/*! tailwindcss v3.2.7 | MIT License | https://tailwindcss.com*/*,:after,:before{box-sizing:border-box;border:0 solid #e5e7eb}:after,:before{--tw-content:""}html{line-height:1.5;-webkit-text-size-adjust:100%;-moz-tab-size:4;-o-tab-size:4;tab-size:4;font-family:ui-sans-serif,system-ui,-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica Neue,Arial,Noto Sans,sans-serif,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji;font-feature-settings:normal}body{margin:0;line-height:inherit}hr{height:0;color:inherit;border-top-width:1px}abbr:where([title]){-webkit-text-decoration:underline dotted;text-decoration:underline dotted}h1,h2,h3,h4,h5,h6{font-size:inherit;font-weight:inherit}a{color:inherit;text-decoration:inherit}b,strong{font-weight:bolder}code,kbd,pre,samp{font-family:ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;font-size:1em}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:initial}sub{bottom:-.25em}sup{top:-.5em}table{text-indent:0;border-color:inherit;border-collapse:collapse}button,input,optgroup,select,textarea{font-family:inherit;font-size:100%;font-weight:inherit;line-height:inherit;color:inherit;margin:0;padding:0}button,select{text-transform:none}[type=button],[type=reset],[type=submit],button{-webkit-appearance:button;background-color:initial;background-image:none}:-moz-focusring{outline:auto}:-moz-ui-invalid{box-shadow:none}progress{vertical-align:initial}::-webkit-inner-spin-button,::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}summary{display:list-item}blockquote,dd,dl,figure,h1,h2,h3,h4,h5,h6,hr,p,pre{margin:0}fieldset{margin:0}fieldset,legend{padding:0}menu,ol,ul{list-style:none;margin:0;padding:0}textarea{resize:vertical}input::-moz-placeholder,textarea::-moz-placeholder{opacity:1;color:#9ca3af}input::placeholder,textarea::placeholder{opacity:1;color:#9ca3af}[role=button],button{cursor:pointer}:disabled{cursor:default}audio,canvas,embed,iframe,img,object,svg,video{display:block;vertical-align:middle}img,video{max-width:100%;height:auto}[hidden]{display:none}*,::backdrop,:after,:before{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:#3b82f680;--tw-ring-offset-shadow:0 0 #0000;--tw-ring-shadow:0 0 #0000;--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: }.collapse{visibility:collapse}.order-last{order:9999}.mx-auto{margin-left:auto;margin-right:auto}.ml-1{margin-left:.25rem}.mr-3{margin-right:.75rem}.block{display:block}.flex{display:flex}.table{display:table}.contents{display:contents}.hidden{display:none}.w-64{width:16rem}.w-8{width:2rem}.w-full{width:100%}.min-w-0{min-width:0}.max-w-6xl{max-width:72rem}.shrink-0{flex-shrink:0}.flex-grow{flex-grow:1}.-translate-x-1{--tw-translate-x:-0.25rem}.-translate-x-1,.-translate-x-2{transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.-translate-x-2{--tw-translate-x:-0.5rem}.flex-col{flex-direction:column}.items-center{align-items:center}.justify-between{justify-content:space-between}.justify-around{justify-content:space-around}.gap-2{gap:.5rem}.break-words{overflow-wrap:break-word}.p-6{padding:1.5rem}.px-2{padding-left:.5rem;padding-right:.5rem}.px-6{padding-left:1.5rem;padding-right:1.5rem}.pb-3{padding-bottom:.75rem}.pb-4{padding-bottom:1rem}.pb-6{padding-bottom:1.5rem}.pr-3{padding-right:.75rem}.pt-12{padding-top:3rem}.pt-3{padding-top:.75rem}.pt-6{padding-top:1.5rem}.text-2xl{font-size:1.5rem;line-height:2rem}.text-sm{font-size:.875rem;line-height:1.25rem}html.light{color-scheme:light}html.dark{color-scheme:dark}::-moz-selection{color:rgba(var(--sy-rc-theme),1);background-color:rgba(var(--sy-rc-theme),.2)}::selection{color:rgba(var(--sy-rc-theme),1);background-color:rgba(var(--sy-rc-theme),.2)}body{font-family:var(--sy-f-text);color:var(--sy-c-text)}h1,h2,h3,h4,h5{color:var(--sy-c-heading);font-family:var(--sy-f-heading)}em,strong{color:var(--sy-c-bold)}.sy-container{max-width:90rem}.sy-deprecated{padding:.8rem;font-size:.85rem;background-color:#ffdd001a;border-radius:6px}.sy-scrollbar{overflow-y:auto;scrollbar-gutter:stable}.sy-scrollbar::-webkit-scrollbar{height:.75rem;width:.75rem}.sy-scrollbar::-webkit-scrollbar-thumb{border-radius:10px}.sy-scrollbar::-webkit-scrollbar-track{background-color:initial}.sy-scrollbar:hover::-webkit-scrollbar-thumb{background-color:#9b9b9b33;background-clip:content-box;border:3px solid #0000}.i-icon{-webkit-mask:var(--icon-url) no-repeat;mask:var(--icon-url) no-repeat;-webkit-mask-size:100% 100%;mask-size:100% 100%;width:1em;height:1em;display:inline-block;vertical-align:middle;font-style:normal;background-color:currentColor}.theme-switch .theme-icon{--icon-url:var(--i-sun-url)}html.dark .theme-switch .theme-icon{--icon-url:var(--i-moon-url)}html.dark .dark-hidden,html.light .light-hidden{display:none}:root{--i-alert-url:url("data:image/svg+xml;utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath d='m21.73 18-8-14a2 2 0 0 0-3.48 0l-8 14A2 2 0 0 0 4 21h16a2 2 0 0 0 1.73-3zM12 9v4m0 4h.01'/%3E%3C/svg%3E");--i-arrows-url:url("data:image/svg+xml;utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath d='m7 15 5 5 5-5M7 9l5-5 5 5'/%3E%3C/svg%3E");--i-award-url:url("data:image/svg+xml;utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Ccircle cx='12' cy='8' r='6'/%3E%3Cpath d='M15.477 12.89 17 22l-5-3-5 3 1.523-9.11'/%3E%3C/svg%3E");--i-bell-url:url("data:image/svg+xml;utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath d='M18 8A6 6 0 0 0 6 8c0 7-3 9-3 9h18s-3-2-3-9m-4.27 13a2 2 0 0 1-3.46 0'/%3E%3C/svg%3E");--i-bookmark-url:url("data:image/svg+xml;utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath d='m19 21-7-4-7 4V5a2 2 0 0 1 2-2h10a2 2 0 0 1 2 2v16z'/%3E%3C/svg%3E");--i-calendar-url:url("data:image/svg+xml;utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Crect x='3' y='4' width='18' height='18' rx='2' ry='2'/%3E%3Cpath d='M16 2v4M8 2v4M3 10h18'/%3E%3C/svg%3E");--i-check-url:url("data:image/svg+xml;utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath d='M20 6 9 17l-5-5'/%3E%3C/svg%3E");--i-chevron-url:url("data:image/svg+xml;utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath d='m9 18 6-6-6-6'/%3E%3C/svg%3E");--i-close-url:url("data:image/svg+xml;utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath d='M18 6 6 18M6 6l12 12'/%3E%3C/svg%3E");--i-discord-url:url("data:image/svg+xml;utf8,%3Csvg viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M20.317 4.37a19.791 19.791 0 0 0-4.885-1.515.074.074 0 0 0-.079.037c-.21.375-.444.864-.608 1.25a18.27 18.27 0 0 0-5.487 0 12.64 12.64 0 0 0-.617-1.25.077.077 0 0 0-.079-.037A19.736 19.736 0 0 0 3.677 4.37a.07.07 0 0 0-.032.027C.533 9.046-.32 13.58.099 18.057a.082.082 0 0 0 .031.057 19.9 19.9 0 0 0 5.993 3.03.078.078 0 0 0 .084-.028 14.09 14.09 0 0 0 1.226-1.994.076.076 0 0 0-.041-.106 13.107 13.107 0 0 1-1.872-.892.077.077 0 0 1-.008-.128 10.2 10.2 0 0 0 .372-.292.074.074 0 0 1 .077-.01c3.928 1.793 8.18 1.793 12.062 0a.074.074 0 0 1 .078.01c.12.098.246.198.373.292a.077.077 0 0 1-.006.127 12.299 12.299 0 0 1-1.873.892.077.077 0 0 0-.041.107c.36.698.772 1.362 1.225 1.993a.076.076 0 0 0 .084.028 19.839 19.839 0 0 0 6.002-3.03.077.077 0 0 0 .032-.054c.5-5.177-.838-9.674-3.549-13.66a.061.061 0 0 0-.031-.03zM8.02 15.33c-1.183 0-2.157-1.085-2.157-2.419 0-1.333.956-2.419 2.157-2.419 1.21 0 2.176 1.096 2.157 2.42 0 1.333-.956 2.418-2.157 2.418zm7.975 0c-1.183 0-2.157-1.085-2.157-2.419 0-1.333.955-2.419 2.157-2.419 1.21 0 2.176 1.096 2.157 2.42 0 1.333-.946 2.418-2.157 2.418z'/%3E%3C/svg%3E");--i-flame-url:url("data:image/svg+xml;utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath d='M8.5 14.5A2.5 2.5 0 0 0 11 12c0-1.38-.5-2-1-3-1.072-2.143-.224-4.054 2-6 .5 2.5 2 4.9 4 6.5 2 1.6 3 3.5 3 5.5a7 7 0 1 1-14 0c0-1.153.433-2.294 1-3a2.5 2.5 0 0 0 2.5 2.5z'/%3E%3C/svg%3E");--i-git-fork-url:url("data:image/svg+xml;utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Ccircle cx='12' cy='18' r='3'/%3E%3Ccircle cx='6' cy='6' r='3'/%3E%3Ccircle cx='18' cy='6' r='3'/%3E%3Cpath d='M18 9v1a2 2 0 0 1-2 2H8a2 2 0 0 1-2-2V9M12 12v3'/%3E%3C/svg%3E");--i-github-url:url("data:image/svg+xml;utf8,%3Csvg viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M12 .297c-6.63 0-12 5.373-12 12 0 5.303 3.438 9.8 8.205 11.385.6.113.82-.258.82-.577 0-.285-.01-1.04-.015-2.04-3.338.724-4.042-1.61-4.042-1.61C4.422 18.07 3.633 17.7 3.633 17.7c-1.087-.744.084-.729.084-.729 1.205.084 1.838 1.236 1.838 1.236 1.07 1.835 2.809 1.305 3.495.998.108-.776.417-1.305.76-1.605-2.665-.3-5.466-1.332-5.466-5.93 0-1.31.465-2.38 1.235-3.22-.135-.303-.54-1.523.105-3.176 0 0 1.005-.322 3.3 1.23.96-.267 1.98-.399 3-.405 1.02.006 2.04.138 3 .405 2.28-1.552 3.285-1.23 3.285-1.23.645 1.653.24 2.873.12 3.176.765.84 1.23 1.91 1.23 3.22 0 4.61-2.805 5.625-5.475 5.92.42.36.81 1.096.81 2.22 0 1.606-.015 2.896-.015 3.286 0 .315.21.69.825.57C20.565 22.092 24 17.592 24 12.297c0-6.627-5.373-12-12-12'/%3E%3C/svg%3E");--i-gitlab-url:url("data:image/svg+xml;utf8,%3Csvg viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='m23.6 9.593-.033-.086L20.3.98a.851.851 0 0 0-.336-.405.875.875 0 0 0-1 .054.875.875 0 0 0-.29.44L16.47 7.818H7.537L5.332 1.07a.857.857 0 0 0-.29-.441.875.875 0 0 0-1-.054.859.859 0 0 0-.336.405L.433 9.502l-.032.086a6.066 6.066 0 0 0 2.012 7.01l.01.009.03.021 4.977 3.727 2.462 1.863 1.5 1.132a1.008 1.008 0 0 0 1.22 0l1.499-1.132 2.461-1.863 5.006-3.75.013-.01a6.068 6.068 0 0 0 2.01-7.002z'/%3E%3C/svg%3E");--i-help-url:url("data:image/svg+xml;utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Ccircle cx='12' cy='12' r='10'/%3E%3Cpath d='M9.09 9a3 3 0 0 1 5.83 1c0 2-3 3-3 3m.08 4h.01'/%3E%3C/svg%3E");--i-laptop-url:url("data:image/svg+xml;utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Crect x='3' y='4' width='18' height='12' rx='2' ry='2'/%3E%3Cpath d='M2 20h20'/%3E%3C/svg%3E");--i-link-url:url("data:image/svg+xml;utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath d='M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71'/%3E%3Cpath d='M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71'/%3E%3C/svg%3E");--i-mastodon-url:url("data:image/svg+xml;utf8,%3Csvg viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M23.268 5.313c-.35-2.578-2.617-4.61-5.304-5.004C17.51.242 15.792 0 11.813 0h-.03c-3.98 0-4.835.242-5.288.309C3.882.692 1.496 2.518.917 5.127.64 6.412.61 7.837.661 9.143c.074 1.874.088 3.745.26 5.611.118 1.24.325 2.47.62 3.68.55 2.237 2.777 4.098 4.96 4.857 2.336.792 4.849.923 7.256.38.265-.061.527-.132.786-.213.585-.184 1.27-.39 1.774-.753a.057.057 0 0 0 .023-.043v-1.809a.052.052 0 0 0-.02-.041.053.053 0 0 0-.046-.01 20.282 20.282 0 0 1-4.709.545c-2.73 0-3.463-1.284-3.674-1.818a5.593 5.593 0 0 1-.319-1.433.053.053 0 0 1 .066-.054c1.517.363 3.072.546 4.632.546.376 0 .75 0 1.125-.01 1.57-.044 3.224-.124 4.768-.422.038-.008.077-.015.11-.024 2.435-.464 4.753-1.92 4.989-5.604.008-.145.03-1.52.03-1.67.002-.512.167-3.63-.024-5.545zm-3.748 9.195h-2.561V8.29c0-1.309-.55-1.976-1.67-1.976-1.23 0-1.846.79-1.846 2.35v3.403h-2.546V8.663c0-1.56-.617-2.35-1.848-2.35-1.112 0-1.668.668-1.67 1.977v6.218H4.822V8.102c0-1.31.337-2.35 1.011-3.12.696-.77 1.608-1.164 2.74-1.164 1.311 0 2.302.5 2.962 1.498l.638 1.06.638-1.06c.66-.999 1.65-1.498 2.96-1.498 1.13 0 2.043.395 2.74 1.164.675.77 1.012 1.81 1.012 3.12z'/%3E%3C/svg%3E");--i-milestone-url:url("data:image/svg+xml;utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath d='M18 6H5a2 2 0 0 0-2 2v3a2 2 0 0 0 2 2h13l4-3.5L18 6zM12 13v8M12 3v3'/%3E%3C/svg%3E");--i-moon-url:url("data:image/svg+xml;utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath d='M12 3a6.364 6.364 0 0 0 9 9 9 9 0 1 1-9-9z'/%3E%3C/svg%3E");--i-outdent-url:url("data:image/svg+xml;utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath d='m7 8-4 4 4 4M21 12H11M21 6H11M21 18H11'/%3E%3C/svg%3E");--i-rocket-url:url("data:image/svg+xml;utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath d='M4.5 16.5c-1.5 1.26-2 5-2 5s3.74-.5 5-2c.71-.84.7-2.13-.09-2.91a2.18 2.18 0 0 0-2.91-.09zM12 15l-3-3a22 22 0 0 1 2-3.95A12.88 12.88 0 0 1 22 2c0 2.72-.78 7.5-6 11a22.35 22.35 0 0 1-4 2z'/%3E%3Cpath d='M9 12H4s.55-3.03 2-4c1.62-1.08 5 0 5 0M12 15v5s3.03-.55 4-2c1.08-1.62 0-5 0-5'/%3E%3C/svg%3E");--i-skull-url:url("data:image/svg+xml;utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Ccircle cx='9' cy='12' r='1'/%3E%3Ccircle cx='15' cy='12' r='1'/%3E%3Cpath d='M8 20v2h8v-2m-3.5-3-.5-1-.5 1h1z'/%3E%3Cpath d='M16 20a2 2 0 0 0 1.56-3.25 8 8 0 1 0-11.12 0A2 2 0 0 0 8 20'/%3E%3C/svg%3E");--i-star-url:url("data:image/svg+xml;utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath d='m12 2 3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01L12 2z'/%3E%3C/svg%3E");--i-sun-url:url("data:image/svg+xml;utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Ccircle cx='12' cy='12' r='4'/%3E%3Cpath d='M12 2v2m0 16v2M4.93 4.93l1.41 1.41m11.32 11.32 1.41 1.41M2 12h2m16 0h2M6.34 17.66l-1.41 1.41M19.07 4.93l-1.41 1.41'/%3E%3C/svg%3E");--i-twitter-url:url("data:image/svg+xml;utf8,%3Csvg viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M23.953 4.57a10 10 0 0 1-2.825.775 4.958 4.958 0 0 0 2.163-2.723c-.951.555-2.005.959-3.127 1.184a4.92 4.92 0 0 0-8.384 4.482C7.69 8.095 4.067 6.13 1.64 3.162a4.822 4.822 0 0 0-.666 2.475c0 1.71.87 3.213 2.188 4.096a4.904 4.904 0 0 1-2.228-.616v.06a4.923 4.923 0 0 0 3.946 4.827 4.996 4.996 0 0 1-2.212.085 4.936 4.936 0 0 0 4.604 3.417 9.867 9.867 0 0 1-6.102 2.105c-.39 0-.779-.023-1.17-.067a13.995 13.995 0 0 0 7.557 2.209c9.053 0 13.998-7.496 13.998-13.985 0-.21 0-.42-.015-.63A9.935 9.935 0 0 0 24 4.59z'/%3E%3C/svg%3E");--i-zap-url:url("data:image/svg+xml;utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath d='M13 2 3 14h9l-1 8 10-12h-9l1-8z'/%3E%3C/svg%3E")}.i-icon.alert{--icon-url:var(--i-alert-url)}.i-icon.arrows{--icon-url:var(--i-arrows-url)}.i-icon.award{--icon-url:var(--i-award-url)}.i-icon.bell{--icon-url:var(--i-bell-url)}.i-icon.bookmark{--icon-url:var(--i-bookmark-url)}.i-icon.calendar{--icon-url:var(--i-calendar-url)}.i-icon.check{--icon-url:var(--i-check-url)}.i-icon.chevron{--icon-url:var(--i-chevron-url)}.i-icon.close{--icon-url:var(--i-close-url)}.i-icon.discord{--icon-url:var(--i-discord-url)}.i-icon.flame{--icon-url:var(--i-flame-url)}.i-icon.git-fork{--icon-url:var(--i-git-fork-url)}.i-icon.github{--icon-url:var(--i-github-url)}.i-icon.gitlab{--icon-url:var(--i-gitlab-url)}.i-icon.help{--icon-url:var(--i-help-url)}.i-icon.laptop{--icon-url:var(--i-laptop-url)}.i-icon.link{--icon-url:var(--i-link-url)}.i-icon.mastodon{--icon-url:var(--i-mastodon-url)}.i-icon.milestone{--icon-url:var(--i-milestone-url)}.i-icon.moon{--icon-url:var(--i-moon-url)}.i-icon.outdent{--icon-url:var(--i-outdent-url)}.i-icon.rocket{--icon-url:var(--i-rocket-url)}.i-icon.skull{--icon-url:var(--i-skull-url)}.i-icon.star{--icon-url:var(--i-star-url)}.i-icon.sun{--icon-url:var(--i-sun-url)}.i-icon.twitter{--icon-url:var(--i-twitter-url)}.i-icon.zap{--icon-url:var(--i-zap-url)}.hamburger{position:relative;display:inline-block;width:16px;height:14px;overflow:hidden;cursor:pointer}.hamburger>span{position:absolute;width:16px;height:2px;left:0;background-color:var(--sy-c-text);transition:top .25s,transform .25s}.hamburger_1{top:0}.hamburger_2{top:6px}.hamburger_3{top:12px}button.hamburger[aria-expanded=true] .hamburger_1{top:6px;transform:translate(0) rotate(225deg)}button.hamburger[aria-expanded=true] .hamburger_2{top:6px;transform:translate(18px)}button.hamburger[aria-expanded=true] .hamburger_3{top:6px;transform:translate(0) rotate(135deg)}.globaltoc .caption{font-size:.86rem;font-weight:500;font-family:var(--sy-f-heading);color:var(--sy-c-text-weak);text-transform:uppercase;letter-spacing:.4px;padding:.8rem 0 .4rem;border-top:1px solid var(--sy-c-divider)}.globaltoc>p.caption:first-of-type{padding-top:0;border-top:none}.globaltoc .caption+ul{margin-bottom:1.5rem}.globaltoc ul+.caption{margin-top:3rem}.globaltoc li{margin:.6rem 0}.globaltoc>ul>li>ul{margin-left:.2rem;border-left:1px solid var(--sy-c-divider-weak);font-size:.96rem}.globaltoc li.toctree-l2{padding-left:.9rem;margin-left:-1px;border-left:1px solid #0000}.globaltoc li.toctree-l2.current{border-color:var(--sy-c-link)}.globaltoc>ul a.current{font-weight:500;color:var(--sy-c-link)}.globaltoc>ul a:hover{color:var(--sy-c-text-strong)}.localtoc>h3{font-size:.8rem;font-weight:500;letter-spacing:.4px;text-transform:uppercase;margin-bottom:1rem}.localtoc>ul li{margin-top:.36rem;margin-bottom:.36rem}.localtoc>ul li>a:hover{color:var(--sy-c-text-strong)}.localtoc>ul li.active>a{font-weight:500;color:var(--sy-c-link)}.localtoc>ul>li>ul{padding-left:.8rem}.searchbox{position:relative}.searchbox input{-webkit-appearance:none;-moz-appearance:none;appearance:none;width:100%;padding:6px 12px;font-size:.92rem;font-family:var(--sy-f-text);border-radius:6px;outline:0;background:var(--sy-c-bg-weak)}.searchbox button,.searchbox kbd{position:absolute;font-size:.68rem;font-weight:600;font-family:var(--sy-f-mono);padding:2px 6px;margin:6px;right:0;border-radius:3px;border:1px solid var(--sy-c-border);background-color:var(--sy-c-bg);opacity:1;transition:opacity .2s ease}.searchbox input:focus+kbd{opacity:0}.searchform{display:flex;position:relative;align-items:center}.searchform input[name=q]{-webkit-appearance:none;-moz-appearance:none;appearance:none;width:100%;padding:6px 12px;font-size:.92rem;font-family:var(--sy-f-text);border-radius:6px;outline:0;background:var(--sy-c-bg-weak)}.searchform input[name=q]+button{position:absolute;font-size:.68rem;font-weight:600;font-family:var(--sy-f-text);padding:2px 6px;margin:6px;right:0;border-radius:3px;border:1px solid var(--sy-c-divider);background-color:var(--sy-c-bg);opacity:1;transition:opacity .2s ease}.navigation{gap:2rem;padding-top:1rem;border-top:1px solid var(--sy-c-divider)}.navigation>div{width:100%}.navigation a{display:inline-flex;align-items:center}.navigation a:hover{color:rgba(var(--sy-rc-invert),1)}.navigation-prev i.chevron{transform:rotate(180deg)}.navigation-next{text-align:right}.navigation-next a{justify-content:end}.navigation .page-info{padding:0 8px}.navigation .page-info>span{font-size:.8rem;color:var(--sy-c-text-weak)}.demo{border:1px solid var(--sy-c-border);border-radius:6px}.demo-code .highlight>pre{border-bottom-left-radius:0;border-bottom-right-radius:0}.demo-result{padding:1rem}.yue button.copybtn{align-items:center;justify-content:center;background-color:initial;border:none;color:var(--sy-c-text)}.yue button.copybtn>svg{width:1.4rem;height:1.4rem}.yue .highlight button.copybtn:hover{background-color:initial;color:var(--sy-c-text-weak)}.yue .o-tooltip--left:after{background-color:initial;color:var(--sy-c-text)}#ethical-ad-placement .ethical-sidebar{position:relative;background-color:var(--sy-c-bg-weak);border:none;padding:.8rem}#ethical-ad-placement .ethical-text a{color:var(--sy-c-text)!important}.sy-main #ethical-ad-placement .ethical-sidebar{margin-left:0;max-width:380px}.sy-main #ethical-ad-placement .ethical-image-link{flex-shrink:0;margin-right:.4rem}.sy-main #ethical-ad-placement .ethical-content{display:flex}.sy-main #ethical-ad-placement .ethical-text{margin-top:0}.sy-main #ethical-ad-placement .ethical-callout{position:absolute;right:.4rem;bottom:.4rem}#carbonads{margin:1rem 0;position:relative;display:block;background-color:var(--sy-c-bg-weak);border:none;border-radius:8px;padding:.8rem .8rem 1.6rem}.carbon-wrap{display:flex;align-items:center;justify-content:space-between;flex-direction:column}.carbon-text{display:block;margin:.5rem 0;line-height:1.42;font-size:.78rem;text-align:center}.carbon-text:hover{color:var(--sy-c-link)}.carbon-poweredby{position:absolute;right:.8rem;bottom:.5rem;font-size:.68rem;text-transform:uppercase}.carbon-poweredby:hover{text-decoration:underline}.sy-main #carbonads{max-width:380px;padding:1rem}.sy-main .carbon-wrap{flex-direction:row}.sy-main .carbon-text{text-align:left;margin-left:1rem}.yue{--yue-c-text:var(--sy-c-text);--yue-c-heading:var(--sy-c-heading);--yue-c-bold:var(--sy-c-bold);--yue-c-link-1:var(--sy-c-text);--yue-c-link-2:#111827;--yue-c-link-border-1:rgba(var(--sy-rc-theme),0.8);--yue-c-link-border-2:var(--sy-c-link);--yue-c-ol-marker:#6b7280;--yue-c-ul-marker:#d1d5db;--yue-c-hr:#e5e7eb;--yue-c-quote:#111827;--yue-c-quote-border:#cfd3db;--yue-c-quote-symbol:rgba(var(--sy-rc-theme),1);--yue-c-caption:#6b7280;--yue-c-code:#111827;--yue-c-code-bg:#fff4d4;--yue-c-th-bg:#eff3f8;--yue-c-th-border:#d1d5db;--yue-c-td-border:#e5e7eb}html.dark .yue{--yue-c-link-1:var(--sy-c-text);--yue-c-link-2:#fff;--yue-c-ol-marker:#9ca3af;--yue-c-ul-marker:#4b5563;--yue-c-hr:#374151;--yue-c-quote:#f3f4f6;--yue-c-quote-border:#374151;--yue-c-caption:#9ca3af;--yue-c-code:#fff;--yue-c-code-bg:#312f29;--yue-c-th-bg:#24282e;--yue-c-th-border:#4b5563;--yue-c-td-border:#374151}.yue{font-size:1rem;line-height:1.75;color:var(--yue-c-text)}.yue p{margin-top:1rem;margin-bottom:1.25rem}.yue a{color:var(--yue-c-link-1);text-decoration:underline;font-weight:500;text-decoration:none;border-bottom:1px solid var(--yue-c-link-border-1)}.yue a:hover{color:var(--yue-c-link-2);border-bottom:2px solid var(--yue-c-link-border-2)}.yue strong{color:var(--yue-c-bold);font-weight:600}.yue a strong,.yue blockquote strong,.yue thead th strong{color:inherit}.yue ol{margin-top:1.25em;margin-bottom:1.25em;padding-left:1.625em}.yue ol,.yue ol[type="1"]{list-style-type:decimal}.yue ol.upperalpha,.yue ol[type=A]{list-style-type:upper-alpha}.yue ol.loweralpha,.yue ol[type=a]{list-style-type:lower-alpha}.yue ol.upperroman,.yue ol[type=I]{list-style-type:upper-roman}.yue ol.lowerroman,.yue ol[type=i]{list-style-type:lower-roman}.yue ul{list-style-type:disc;margin-top:1.25em;margin-bottom:1.25em;padding-left:1.625em}.yue ol>li::marker{font-weight:400;color:var(--yue-c-ol-marker)}.yue ul>li::marker{color:var(--yue-c-ul-marker)}.yue dl{margin-top:1.5rem;margin-bottom:1.5rem}.yue dt{color:var(--yue-c-bold);font-weight:600}.yue dd{margin-left:1.5rem}.yue hr{border-color:var(--yue-c-hr);border-top-width:1px;margin-top:3em;margin-bottom:3em}.yue blockquote{color:var(--yue-c-quote);border-left-width:.25rem;border-left-color:var(--yue-c-quote-border);margin-top:1.2rem;margin-bottom:1.2rem;padding-left:1rem}.yue blockquote .attribution{font-size:.85em;font-style:italic}[lang=ja] .yue blockquote .attribution,[lang=ko] .yue blockquote .attribution,[lang^=zh] .yue blockquote .attribution{font-style:normal}.yue h1{color:var(--yue-c-heading);font-weight:800;font-size:2.25em;margin-top:0;margin-bottom:.8888889em;line-height:1.1111111}.yue h1 strong{font-weight:900;color:inherit}.yue h2{color:var(--yue-c-heading);font-weight:700;font-size:1.5em;margin-top:2em;margin-bottom:1em;line-height:1.3333333}.yue h2 strong{font-weight:800;color:inherit}.yue h3{color:var(--yue-c-heading);font-weight:600;font-size:1.25em;margin-top:1.6em;margin-bottom:.6em;line-height:1.6}.yue h3 strong{font-weight:700;color:inherit}.yue h4{color:var(--yue-c-heading);font-weight:600;margin-top:1.5em;margin-bottom:.5em;line-height:1.5}.yue h4 strong{font-weight:700;color:inherit}.yue img{margin-top:2em;margin-bottom:2em}.yue figure>*{margin-top:0;margin-bottom:0}.yue figcaption{color:var(--yue-c-caption);font-size:.875em;line-height:1.4285714;margin-top:.8571429em}.yue code{color:var(--yue-c-code);font-weight:600;font-size:.875em}.yue a code,.yue blockquote code,.yue h1 code,.yue h2 code,.yue h3 code,.yue h4 code,.yue th code{color:inherit}.yue h2 code{font-size:.875em}.yue li>code,.yue p>code{padding-left:4px;padding-right:4px;border-radius:3px;font-weight:500;background-color:var(--yue-c-code-bg)}.yue h3 code{font-size:.9em}.yue figure,.yue video{margin-top:2em;margin-bottom:2em}.yue li{margin-top:.5em;margin-bottom:.5em}.yue ol>li,.yue ul>li{padding-left:.375em}.yue ol ol,.yue ol ul,.yue ul ol,.yue ul ul{margin-top:.75em;margin-bottom:.75em}.yue h2+*,.yue h3+*,.yue h4+*,.yue hr+*{margin-top:0}.yue table{width:100%;table-layout:auto;text-align:left;margin-top:2em;margin-bottom:2em;font-size:.86em;line-height:1.7}.yue table>caption{margin-bottom:.4rem;color:var(--yue-c-caption)}.yue thead tr{border-bottom-width:1px;border-bottom-color:var(--yue-c-th-border)}.yue thead th{color:var(--yue-c-heading);font-weight:600;vertical-align:middle;text-align:center}.yue tbody tr{border-bottom-width:1px;border-bottom-color:var(--yue-c-td-border)}.yue tbody tr:last-child{border-bottom-width:0}.yue tbody td{vertical-align:middle}.yue tfoot{border-top-width:1px;border-top-color:var(--yue-c-th-border)}.yue tfoot td{vertical-align:top}.yue td>p{margin:.25rem 0}.yue thead th>p{margin:0}.yue tbody td,.yue tfoot td,.yue thead th{padding:.5rem}.yue section>div{margin-bottom:2rem}.yue dd>p:first-child{margin-top:0}.yue dl.simple>dd>p,.yue ul.simple>li>p{margin:0}.yue a.headerlink{visibility:hidden;margin-left:6px;color:rgba(var(--sy-rc-text),.6);font-weight:300;font-family:var(--sy-f-mono)}.yue .math a.headerlink,h2:hover a.headerlink,h3:hover a.headerlink,h4:hover a.headerlink,h5:hover a.headerlink,h6:hover a.headerlink{visibility:visible}.yue .toctree-wrapper a{border-bottom:none}.yue .toctree-wrapper p.caption{font-size:.86rem;font-weight:500;font-family:var(--sy-f-heading);color:var(--sy-c-text-weak);text-transform:uppercase;letter-spacing:.4px;padding:.8rem 0 .4rem;border-bottom:1px solid var(--sy-c-divider)}.yue .align-center{display:block;text-align:center}.yue .align-center,.yue figure.align-center img{margin-left:auto;margin-right:auto}a.footnote-reference{font-size:.65rem;vertical-align:top}aside.footnote>span,div.citation>span{float:left;font-weight:500;padding-right:.25rem}aside.footnote>p,div.citation>p{margin-bottom:.5rem;margin-top:.5rem;margin-left:2rem}.yue kbd.kbd:not(.compound){font-size:.86rem;padding:2px 5px;border-radius:3px;margin-right:.25rem}.yue kbd.compound>kbd{margin-left:.25rem}.light .yue kbd.kbd:not(.compound){background:linear-gradient(-225deg,#e6e6e6,#f8f8f8);box-shadow:inset 0 -2px #dbdbdb,inset 0 0 1px 1px #fff,0 1px 2px 1px #50505066}.dark .yue kbd.kbd:not(.compound){background:linear-gradient(-225deg,#353434,#141414);box-shadow:inset 0 -2px #373737,inset 0 0 1px 1px #222,0 1px 2px 1px #000}.hlist td{vertical-align:top}p.centered{text-align:center}:root,html.light{--admonition-bg-opacity:0.03;--admonition-head-opacity:0.08;--admonition-border-opacity:1}html.dark{--admonition-bg-opacity:0.08;--admonition-head-opacity:0.15;--admonition-border-opacity:0.8}:root{--attention-icon:var(--i-alert-url);--attention-color:247,89,171;--caution-icon:var(--i-zap-url);--caution-color:247,186,42;--danger-icon:var(--i-skull-url);--danger-color:255,92,47;--error-icon:var(--i-close-url);--error-color:255,92,47;--hint-icon:var(--i-bell-url);--hint-color:0,200,80;--important-icon:var(--i-flame-url);--important-color:179,127,235;--note-icon:var(--i-calendar-url);--note-color:3,169,244;--tip-icon:var(--i-rocket-url);--tip-color:0,200,80;--warning-icon:var(--i-zap-url);--warning-color:255,145,0;--seealso-icon:var(--i-link-url);--seealso-color:60,140,255;--todo-icon:var(--i-bookmark-url);--todo-color:220,150,0;--versionadded-color:0,200,80;--versionchanged-color:247,186,42;--deprecated-color:255,92,47}.admonition{--color-rgb:var(--sy-rc-theme);--icon-url:var(--i-bell-url);position:relative;padding:0 16px .8rem;margin-top:1rem;margin-bottom:1rem;border-left:4px solid rgba(var(--color-rgb),var(--admonition-border-opacity));background-color:rgba(var(--color-rgb),var(--admonition-bg-opacity))}.admonition:before{position:absolute;content:"";top:6px;left:-12px;width:20px;height:20px;border-radius:100%;background-color:rgb(var(--color-rgb))}.admonition p.admonition-title{position:relative;margin:0 -16px .8rem -19px;padding:4px 18px;font-size:.85rem;font-weight:600;line-height:1.72;color:rgb(var(--color-rgb));background-color:rgba(var(--color-rgb),var(--admonition-head-opacity))}.admonition-title:before{position:absolute;content:"";top:10px;left:-5px;-webkit-mask:var(--icon-url) no-repeat;mask:var(--icon-url) no-repeat;-webkit-mask-size:100% 100%;mask-size:100% 100%;font-style:normal;width:12px;height:12px;background-color:#fff}.admonition.attention{--icon-url:var(--attention-icon);--color-rgb:var(--attention-color)}.admonition.caution{--icon-url:var(--caution-icon);--color-rgb:var(--caution-color)}.admonition.danger{--icon-url:var(--danger-icon);--color-rgb:var(--danger-color)}.admonition.error{--icon-url:var(--error-icon);--color-rgb:var(--error-color)}.admonition.hint{--icon-url:var(--hint-icon);--color-rgb:var(--hint-color)}.admonition.important{--icon-url:var(--important-icon);--color-rgb:var(--important-color)}.admonition.note{--icon-url:var(--note-icon);--color-rgb:var(--note-color)}.admonition.tip{--icon-url:var(--tip-icon);--color-rgb:var(--tip-color)}.admonition.warning{--icon-url:var(--warning-icon);--color-rgb:var(--warning-color)}.admonition.seealso{--icon-url:var(--seealso-icon);--color-rgb:var(--seealso-color)}.admonition.admonition-todo{--icon-url:var(--todo-icon);--color-rgb:var(--todo-color)}.admonition p.admonition-title+p{margin-top:0}.admonition>:last-child{margin-bottom:0}span.versionmodified{color:var(--sy-c-bold);font-weight:600}div.deprecated,div.versionadded,div.versionchanged{--version-color:var(--sy-rc-theme);position:relative;padding:6px 1rem;margin:1rem 0;border-left:4px solid rgba(var(--version-color),1);background-color:rgba(var(--version-color),.08);line-height:1.72}div.deprecated:before,div.versionadded:before,div.versionchanged:before{position:absolute;content:var(--version-icon);top:10px;left:-12px;color:#fff;width:20px;height:20px;border-radius:100%;background-color:rgba(var(--version-color),1);text-align:center;font:normal 700 14px/20px var(--sy-f-mono)}div.versionadded{--version-color:var(--versionadded-color);--version-icon:"#"}div.versionchanged{--version-color:var(--versionchanged-color);--version-icon:"%"}div.deprecated{--version-color:var(--deprecated-color);--version-icon:"!"}div.deprecated>p,div.versionadded>p,div.versionchanged>p{margin:0}.yue blockquote.epigraph{padding:1rem 2.4rem;border-left:0;text-align:center}.yue blockquote.highlights{border-left-width:4px;padding-top:.2rem;padding-bottom:.2rem;background-color:var(--sy-c-bg-weak)}.yue blockquote.pull-quote{position:relative;font-size:1.24rem;padding:2.4rem 3.6rem 1.2rem;border-left:0}.yue blockquote.pull-quote:before{content:"\201c";position:absolute;top:0;left:.5rem;color:var(--yue-c-quote-symbol);font:700 4rem/1 Times New Roman,Georgia,Palatino,Times,serif}.yue blockquote.pull-quote .attribution{text-align:right}pre.literal-block{line-height:1.48;padding:1rem;font-size:.96rem;background-color:var(--syntax-pre-bg);border-radius:6px;overflow:auto}.highlight,.literal-block-wrapper{--margin:1rem;--radius:6px}.highlight>pre{display:grid;line-height:1.48;padding:var(--margin);font-size:.96rem;background-color:var(--syntax-pre-bg);border-radius:var(--radius);overflow:auto}.highlight .linenos{display:inline-block;box-shadow:-.05rem 0 rgba(var(--sy-rc-invert),.2) inset;-webkit-user-select:none;-moz-user-select:none;user-select:none;margin-right:.8rem;padding-right:.8rem;opacity:.6}.highlight .hll{margin-left:calc(0rem - var(--margin));margin-right:calc(0rem - var(--margin));padding:0 var(--margin)}.code-block-caption{font-size:.84rem;font-weight:600;color:var(--syntax-text);background-color:var(--syntax-cap-bg);padding:.4rem var(--margin);border-radius:var(--radius) var(--radius) 0 0}.code-block-caption+div>.highlight>pre{border-top-left-radius:0;border-top-right-radius:0}.yue .table-wrapper{width:100%;overflow-x:auto;margin-top:2rem;margin-bottom:2rem}.yue .table-wrapper>table{margin:0}.yue .table-wrapper thead tr{border-top:1px solid var(--yue-c-td-border)}.yue .table-wrapper th{background-color:var(--yue-c-th-bg);border-left:1px solid var(--yue-c-td-border)}.yue .table-wrapper td,.yue .table-wrapper th:last-child{border-right:1px solid var(--yue-c-td-border)}.yue .table-wrapper td{border-left:1px solid var(--yue-c-td-border)}.yue .table-wrapper tbody tr:first-child{border-top:1px solid var(--yue-c-td-border)}.yue .table-wrapper tbody tr:last-child{border-bottom-width:1px}.yue .table-wrapper thead+tbody tr:first-child{border-top-width:0}.yue table.hlist td{vertical-align:top}.table-wrapper{overflow-x:auto;scrollbar-gutter:stable}.table-wrapper::-webkit-scrollbar{height:.75rem;width:.75rem}.table-wrapper::-webkit-scrollbar-thumb{border-radius:10px}.table-wrapper::-webkit-scrollbar-track{background-color:initial}.table-wrapper:hover::-webkit-scrollbar-thumb{background-color:#9b9b9b33;background-clip:content-box;border:3px solid #0000}dt.sig{position:relative;font-size:.92rem;padding:.25rem .5rem .25rem 3rem;text-indent:-2.4rem;border-radius:6px}dt.sig:after{content:"";display:table;clear:both}dt.sig:hover{background:var(--sy-c-bg-weak)}dt.sig+dd{font-size:.92rem;margin-left:2rem}dt.sig>em.property:first-child{color:var(--syntax-keyword)}dl.field-list a{font-weight:400}dt.sig+dd>div{margin-bottom:1rem}dt.sig+dd>dl.field-list>dt{text-transform:uppercase;font-size:.76rem}em.property,em.sig-param{font-style:normal}em.sig-param{color:var(--sy-c-text-weak)}span.sig-name,span.sig-prename{color:var(--syntax-property)}span.sig-name{font-weight:600}span.sig-return-icon{color:var(--sy-c-text-weak)}span.sig-return-typehint,span.sig-return-typehint>a{color:var(--syntax-constant)}span.pre,span.sig-paren{font-family:var(--sy-f-mono)}dt.sig>a.internal{font-size:.82rem;border:0;color:var(--sy-c-text-weak)}dt.sig>a.internal:before{content:"\a";white-space:pre}.viewcode-block{position:relative}.viewcode-back{position:absolute;top:-1.5rem;font-size:.8rem}:root,html.light{--syntax-pre-bg:#f3f1fa;--syntax-cap-bg:#eae7f7;--syntax-text:#24292f;--syntax-meta:#a6a2ae;--syntax-comment:#6e7781;--syntax-constant:#0550ae;--syntax-entity:#268bd2;--syntax-property:#8250df;--syntax-definition:#24292f;--syntax-tag:#085;--syntax-builtin:#b58900;--syntax-keyword:#cf222e;--syntax-exception:#e6212e;--syntax-string:#0a3069;--syntax-regexp:#e40;--syntax-variable:#a4480f;--syntax-invalid-illegal-text:#f6f8fa;--syntax-invalid-illegal-bg:#82071e;--syntax-markup-heading:#0550ae;--syntax-markup-italic:#24292f;--syntax-markup-bold:#24292f;--syntax-markup-deleted-text:#82071e;--syntax-markup-deleted-bg:#ffebe9;--syntax-markup-inserted-text:#116329;--syntax-markup-inserted-bg:#dafbe1;--syntax-markup-changed-text:#953800;--syntax-markup-changed-bg:#ffd8b5;--syntax-markup-ignored-text:#eaeef2;--syntax-markup-ignored-bg:#0550ae;--syntax-meta-diff-range:#8250df;--syntax-highlight-bg:#eee4ff;--syntax-special-bg:#dccafa}.dark-code,html.dark{--syntax-pre-bg:#2c283b;--syntax-cap-bg:#342f47;--syntax-text:#c9d1d9;--syntax-meta:#6e7781;--syntax-comment:#8b949e;--syntax-constant:#79c0ff;--syntax-entity:#47b0fa;--syntax-property:#d2a8ff;--syntax-definition:#c9d1d9;--syntax-tag:#7ee787;--syntax-builtin:#ffd34c;--syntax-keyword:#ff7b72;--syntax-exception:#da473c;--syntax-string:#a5d6ff;--syntax-regexp:#ef954e;--syntax-variable:#ffa657;--syntax-invalid-illegal-text:#f0f6fc;--syntax-invalid-illegal-bg:#8e1519;--syntax-markup-heading:#1f6feb;--syntax-markup-italic:#c9d1d9;--syntax-markup-bold:#c9d1d9;--syntax-markup-deleted-text:#ffdcd7;--syntax-markup-deleted-bg:#67060c;--syntax-markup-inserted-text:#aff5b4;--syntax-markup-inserted-bg:#033a16;--syntax-markup-changed-text:#ffdfb6;--syntax-markup-changed-bg:#5a1e02;--syntax-markup-ignored-text:#c9d1d9;--syntax-markup-ignored-bg:#1158c7;--syntax-meta-diff-range:#d2a8ff;--syntax-highlight-bg:#423551;--syntax-special-bg:#4f425d}.yue{--sd-color-primary:rgb(var(--sy-rc-theme));--sd-color-success:#00c850;--sd-color-warning:#ff9100;--sd-color-danger:#ff5c2f;--sd-color-card-border-hover:var(--sy-c-border);--sd-color-card-border:var(--sy-c-divider);--sd-color-tabs-label-inactive:var(--sy-c-bold);--sd-color-tabs-label-active:var(--sd-color-primary);--sd-color-tabs-underline-active:var(--sd-color-primary)}.light .yue{--sd-color-shadow:#f3f4f6}.dark .yue{--sd-color-shadow:#010409}.yue .sd-container-fluid{margin-top:2rem;padding:.5rem}.yue .sd-row{--sd-gutter-x:1rem;--sd-gutter-y:1rem}.yue .sd-row-cols-1{display:grid;grid-template-columns:1fr;grid-gap:1rem}.yue .sd-row-cols-2{display:grid;grid-template-columns:1fr 1fr;grid-gap:1rem}.yue .sd-row-cols-1>.sd-col,.yue .sd-row-cols-2>.sd-col{width:100%;padding:0;margin:0}.yue .sd-card-hover:hover{transform:scale(1)}.yue .sd-card-hover:hover .sd-card-title{color:var(--sy-c-link)}.yue .sd-card a,.yue .sd-card a:hover{border-bottom:0}@media (max-width:880px){.yue .sd-row-cols-2{grid-template-columns:1fr}}.yue .sd-tab-set>label{padding:1rem .25rem .5rem;font-size:.84rem;font-weight:500}.yue .sd-tab-set>label~label{margin-left:1rem}.yue .sd-tab-content{padding:0;box-shadow:0 -.0625rem var(--sy-c-divider)}.yue .sd-tab-content .highlight pre{border-radius:0}@media (print){.yue .sd-card{page-break-inside:avoid}}.sphinx-tabs [role=tablist]{border-color:var(--sy-c-divider)}.yue .sphinx-tabs-tab{color:var(--sy-c-text);line-height:inherit;padding:1rem .25rem .5rem;font-size:.84rem;font-weight:500;border:none;border-bottom:.125rem solid #0000}.yue .sphinx-tabs-tab:hover{color:var(--sd-color-tabs-label-hover);border-color:var(--sd-color-tabs-underline-hover)}.yue .sphinx-tabs-tab[aria-selected=true]{border:none;border-bottom:.125rem solid var(--sd-color-tabs-underline-active);color:var(--sd-color-tabs-label-active);background-color:initial}.yue .sphinx-tabs-tab+.sphinx-tabs-tab{margin-left:1rem}.yue .sphinx-tabs-panel{border:none;padding:0;margin:0;border-radius:0;background-color:initial}.yue .sphinx-tabs-panel.code-tab{padding:0}.yue .sphinx-tabs-panel.code-tab .highlight pre{border-radius:0}.banner{position:fixed;top:0;left:0;width:100%;height:var(--sy-s-banner-height);display:flex;align-items:center;color:var(--sy-c-banner,#fff);background-color:var(--sy-c-banner-bg,rgba(var(--sy-rc-theme),1));z-index:20}.banner-inner{width:100%;text-align:center}.banner-close{position:absolute;top:1rem;right:1rem}.sy-head{position:sticky;top:var(--sy-s-banner-height);height:var(--sy-s-navbar-height);background-color:initial;z-index:20}.sy-head-blur{position:absolute;top:0;left:0;width:100%;height:100%;-webkit-backdrop-filter:blur(12px);backdrop-filter:blur(12px);background-color:rgba(var(--sy-rc-bg),.85);z-index:-1;--tw-shadow:0 2px 4px rgba(var(--sy-rc-invert),.02),0 1px 0 rgba(var(--sy-rc-invert),.06);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow)}.sy-head-inner{display:flex;padding-left:max(env(safe-area-inset-right),1.5rem);padding-right:max(env(safe-area-inset-right),1.5rem);justify-content:space-between;align-items:center;height:var(--sy-s-navbar-height)}.sy-head-brand img{height:28px}.sy-head-brand img+strong{display:none}.sy-head-brand>.rst-versions{position:relative;margin-left:1rem;width:auto;background:#0000;color:var(--sy-c-text)}.sy-head-brand>.rst-versions>label{display:inline-block;cursor:pointer;font-size:.86rem;font-weight:500;background-color:var(--sy-c-bg-weak);border-radius:2rem;color:var(--sy-c-text-weak);padding:.24rem 1rem}.sy-head-brand>.rst-versions>label:hover{background-color:rgba(var(--sy-rc-invert),.08)}.sy-head-brand>.rst-versions>label .i-icon{transform:rotate(90deg)}.sy-head-brand input+.rst-other-versions{position:absolute;display:none;padding:0;top:2rem;width:300px;background-color:var(--sy-c-bg);border-radius:6px;box-shadow:0 0 3px rgba(var(--sy-rc-invert),.1),0 0 2px rgba(var(--sy-rc-invert),.2) inset}.sy-head-brand input:checked+.rst-other-versions{display:block}.sy-head-brand .injected .rst-versions{position:static;color:var(--sy-c-text);background-color:initial}.sy-head-brand .injected .rst-versions a{color:var(--sy-c-text)!important}.sy-head-brand .injected .rst-versions a:hover{color:var(--sy-c-link)!important}.sy-head-brand .injected .rst-current-version{display:none!important;border-radius:6px}.sy-head-brand .injected .rst-other-versions{display:block}.sy-head-brand .injected .rst-other-versions dt{font-size:.72rem;letter-spacing:.2px;color:var(--sy-c-text-weak)}.sy-head-brand .injected .rst-other-versions hr{border-color:var(--sy-c-divider)}.sy-head-brand .injected form.wy-form input{-webkit-appearance:none;-moz-appearance:none;appearance:none;width:100%;padding:6px 12px;font-size:.92rem;font-family:var(--sy-f-text);border-radius:6px;outline:0;background:var(--sy-c-bg-weak)}.sy-head-nav>ul>li{display:inline-block}.sy-head-nav a{padding:.5rem;font-size:.95rem;font-weight:500;white-space:nowrap}.sy-head-nav a:hover{color:rgba(var(--sy-rc-invert),1)}.sy-head-actions .i-icon{font-size:1.25rem}.sy-head-brand .dark-logo{display:none}.dark .sy-head-brand .dark-logo{display:inline}.dark .sy-head-brand .light-logo{display:none}.light .sy-head-brand .light-logo{display:inline}.light .sy-head-brand .dark-logo{display:none}.sy-foot{border-top:1px solid var(--sy-c-foot-divider);padding-top:1.5rem;padding-bottom:1rem;color:var(--sy-c-foot-text);background-color:var(--sy-c-foot-bg)}.sy-foot-inner{padding-left:max(env(safe-area-inset-right),1.5rem);padding-right:max(env(safe-area-inset-right),1.5rem)}.sy-foot-copyright{font-size:.84rem}.sy-foot-copyright a{font-weight:500}.sy-foot-socials a{font-size:1.4rem;color:var(--sy-c-foot-text)}.sy-foot-socials a+a{margin-left:.5rem}@media (max-width:767px){#lside{position:fixed;z-index:15;top:calc(var(--sy-s-offset-top) - 1px);bottom:0;width:100%;height:calc(100vh - var(---sy-s-offset-top));overflow:auto;background:rgba(var(--sy-rc-bg),.98);transform:translateY(-100%);transition:transform .2s ease}body[data-expanded-lside=true]{overflow:hidden}#lside._expanded{transform:translateY(0)}}@media (max-width:1279px){.sy-rside{position:fixed;z-index:25;top:0;right:0;bottom:0;width:20rem;max-width:100%;padding-top:2rem;padding-bottom:1rem;overflow:auto;background:var(--sy-c-bg);transform:translateX(110%);transition:transform .2s ease;--tw-shadow:-12px 0 16px rgba(var(--sy-rc-bg),0.16);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow)}#rside._expanded{transform:translateX(0)}.rside-close{position:absolute;top:1rem;right:1rem;border:1px solid var(--sy-c-divider);width:1.5rem;height:1.5rem;display:flex;align-items:center;justify-content:center;border-radius:100%}.rside-overlay{position:fixed;top:0;left:0;width:0;height:0;background-color:rgba(var(--sy-rc-invert),.24);opacity:0;transition:width 0 .25s,height 0 .25s,opacity .25s}#rside._expanded+.rside-overlay{width:100%;height:100%;opacity:1;z-index:22}}@media (min-width:768px){.sy-main{width:calc(100% - 16rem);max-width:52rem}}@media (min-width:1280px){.sy-main{width:calc(100% - 32rem)}.sy-rside .sy-scrollbar{max-height:calc(100vh - var(--sy-s-offset-top) - env(safe-area-inset-bottom))}}.yue .viewcode-block,.yue section{scroll-margin-top:calc(var(--sy-s-offset-top) + 80px)}@media (min-width:1280px){.yue .viewcode-block,.yue section{scroll-margin-top:calc(var(--sy-s-offset-top) + 20px)}}.sy-content{max-width:64rem;min-height:calc(100vh - var(--sy-s-offset-top))}.sy-lside li{margin:.6rem 0}.sy-lside .sidebar-links{margin-bottom:2rem}.sy-lside .sidebar-links span{display:inline-block;vertical-align:middle}.sy-lside .sidebar-links .icon{padding:.1rem;border-radius:6px;border:1px solid var(--sy-c-border);margin-right:.4rem;opacity:.8}.sy-lside .sidebar-links svg{width:1.5rem;height:1.5rem}.sy-lside .sidebar-links a:hover .icon{opacity:1}.repo-stats{margin:1rem 0;padding:.5rem 0;border-top:1px solid var(--sy-c-divider);border-bottom:1px solid var(--sy-c-divider)}.repo-stats-count{color:var(--sy-c-text-weak)}.repo-stats:hover .repo-stats-count{color:var(--sy-c-text)}.repo-stats strong{font-weight:500;font-family:var(--sy-f-mono);color:inherit}.edit-this-page{border-top:1px solid var(--sy-c-divider);margin:1rem 0;padding:.5rem 0;font-size:.8rem;font-weight:600}.repo-stats+.edit-this-page{border-top:0;margin-top:0;padding-top:0}.edit-this-page a{color:var(--sy-c-text-weak)}.edit-this-page a:hover{color:var(--sy-c-text)}.edit-this-page a:after{content:" →"}@media (min-width:768px){.sy-lside .sy-scrollbar{height:calc(100vh - var(--sy-s-offset-top));overflow-x:hidden}}@media print{.print\:hidden{display:none}.print\:pt-6{padding-top:1.5rem}}@media not all and (min-width:640px){.max-sm\:max-w-full{max-width:100%}}@media (min-width:768px){.md\:sticky{position:sticky}.md\:top-16{top:4rem}.md\:block{display:block}.md\:flex{display:flex}.md\:hidden{display:none}.md\:w-64{width:16rem}.md\:shrink-0{flex-shrink:0}}@media (min-width:1280px){.xl\:sticky{position:sticky}.xl\:top-16{top:4rem}.xl\:hidden{display:none}.xl\:px-12{padding-left:3rem;padding-right:3rem}.xl\:pl-0{padding-left:0}.xl\:pt-6{padding-top:1.5rem}}
+/*! tailwindcss v3.3.2 | MIT License | https://tailwindcss.com*/*,:after,:before{box-sizing:border-box;border:0 solid #e5e7eb}:after,:before{--tw-content:""}html{line-height:1.5;-webkit-text-size-adjust:100%;-moz-tab-size:4;-o-tab-size:4;tab-size:4;font-family:ui-sans-serif,system-ui,-apple-system,BlinkMacSystemFont,Segoe UI,Roboto,Helvetica Neue,Arial,Noto Sans,sans-serif,Apple Color Emoji,Segoe UI Emoji,Segoe UI Symbol,Noto Color Emoji;font-feature-settings:normal;font-variation-settings:normal}body{margin:0;line-height:inherit}hr{height:0;color:inherit;border-top-width:1px}abbr:where([title]){-webkit-text-decoration:underline dotted;text-decoration:underline dotted}h1,h2,h3,h4,h5,h6{font-size:inherit;font-weight:inherit}a{color:inherit;text-decoration:inherit}b,strong{font-weight:bolder}code,kbd,pre,samp{font-family:ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;font-size:1em}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:initial}sub{bottom:-.25em}sup{top:-.5em}table{text-indent:0;border-color:inherit;border-collapse:collapse}button,input,optgroup,select,textarea{font-family:inherit;font-size:100%;font-weight:inherit;line-height:inherit;color:inherit;margin:0;padding:0}button,select{text-transform:none}[type=button],[type=reset],[type=submit],button{-webkit-appearance:button;background-color:initial;background-image:none}:-moz-focusring{outline:auto}:-moz-ui-invalid{box-shadow:none}progress{vertical-align:initial}::-webkit-inner-spin-button,::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}summary{display:list-item}blockquote,dd,dl,figure,h1,h2,h3,h4,h5,h6,hr,p,pre{margin:0}fieldset{margin:0}fieldset,legend{padding:0}menu,ol,ul{list-style:none;margin:0;padding:0}textarea{resize:vertical}input::-moz-placeholder,textarea::-moz-placeholder{opacity:1;color:#9ca3af}input::placeholder,textarea::placeholder{opacity:1;color:#9ca3af}[role=button],button{cursor:pointer}:disabled{cursor:default}audio,canvas,embed,iframe,img,object,svg,video{display:block;vertical-align:middle}img,video{max-width:100%;height:auto}[hidden]{display:none}*,::backdrop,:after,:before{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:#3b82f680;--tw-ring-offset-shadow:0 0 #0000;--tw-ring-shadow:0 0 #0000;--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: }.collapse{visibility:collapse}.order-last{order:9999}.mx-auto{margin-left:auto;margin-right:auto}.ml-1{margin-left:.25rem}.ml-4{margin-left:1rem}.mr-3{margin-right:.75rem}.block{display:block}.flex{display:flex}.table{display:table}.contents{display:contents}.hidden{display:none}.w-64{width:16rem}.w-8{width:2rem}.w-full{width:100%}.min-w-0{min-width:0}.max-w-6xl{max-width:72rem}.shrink-0{flex-shrink:0}.flex-grow{flex-grow:1}.-translate-x-1{--tw-translate-x:-0.25rem}.-translate-x-1,.-translate-x-2{transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.-translate-x-2{--tw-translate-x:-0.5rem}.flex-col{flex-direction:column}.items-center{align-items:center}.justify-between{justify-content:space-between}.justify-around{justify-content:space-around}.gap-2{gap:.5rem}.break-words{overflow-wrap:break-word}.p-6{padding:1.5rem}.px-2{padding-left:.5rem;padding-right:.5rem}.px-6{padding-left:1.5rem;padding-right:1.5rem}.pb-3{padding-bottom:.75rem}.pb-4{padding-bottom:1rem}.pb-6{padding-bottom:1.5rem}.pr-3{padding-right:.75rem}.pt-12{padding-top:3rem}.pt-3{padding-top:.75rem}.pt-6{padding-top:1.5rem}.text-2xl{font-size:1.5rem;line-height:2rem}.text-sm{font-size:.875rem;line-height:1.25rem}html.light{color-scheme:light}html.dark{color-scheme:dark}::-moz-selection{color:rgba(var(--sy-rc-theme),1);background-color:rgba(var(--sy-rc-theme),.2)}::selection{color:rgba(var(--sy-rc-theme),1);background-color:rgba(var(--sy-rc-theme),.2)}body{font-family:var(--sy-f-text);color:var(--sy-c-text)}h1,h2,h3,h4,h5{color:var(--sy-c-heading);font-family:var(--sy-f-heading)}em,strong{color:var(--sy-c-bold)}.sy-container{max-width:90rem}.sy-deprecated{padding:.8rem;font-size:.85rem;background-color:#ffdd001a;border-radius:6px}.sy-scrollbar{overflow-y:auto;scrollbar-gutter:stable}.sy-scrollbar::-webkit-scrollbar{height:.75rem;width:.75rem}.sy-scrollbar::-webkit-scrollbar-thumb{border-radius:10px}.sy-scrollbar::-webkit-scrollbar-track{background-color:initial}.sy-scrollbar:hover::-webkit-scrollbar-thumb{background-color:#9b9b9b33;background-clip:content-box;border:3px solid #0000}.i-icon{-webkit-mask:var(--icon-url) no-repeat;mask:var(--icon-url) no-repeat;-webkit-mask-size:100% 100%;mask-size:100% 100%;width:1em;height:1em;display:inline-block;vertical-align:middle;font-style:normal;background-color:currentColor}.theme-switch .theme-icon{--icon-url:var(--i-sun-url)}html.dark .theme-switch .theme-icon{--icon-url:var(--i-moon-url)}html.dark .dark-hidden,html.light .light-hidden{display:none}:root{--i-alert-url:url("data:image/svg+xml;utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath d='m21.73 18-8-14a2 2 0 0 0-3.48 0l-8 14A2 2 0 0 0 4 21h16a2 2 0 0 0 1.73-3zM12 9v4m0 4h.01'/%3E%3C/svg%3E");--i-arrows-url:url("data:image/svg+xml;utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath d='m7 15 5 5 5-5M7 9l5-5 5 5'/%3E%3C/svg%3E");--i-award-url:url("data:image/svg+xml;utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Ccircle cx='12' cy='8' r='6'/%3E%3Cpath d='M15.477 12.89 17 22l-5-3-5 3 1.523-9.11'/%3E%3C/svg%3E");--i-bell-url:url("data:image/svg+xml;utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath d='M18 8A6 6 0 0 0 6 8c0 7-3 9-3 9h18s-3-2-3-9m-4.27 13a2 2 0 0 1-3.46 0'/%3E%3C/svg%3E");--i-bookmark-url:url("data:image/svg+xml;utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath d='m19 21-7-4-7 4V5a2 2 0 0 1 2-2h10a2 2 0 0 1 2 2v16z'/%3E%3C/svg%3E");--i-calendar-url:url("data:image/svg+xml;utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Crect x='3' y='4' width='18' height='18' rx='2' ry='2'/%3E%3Cpath d='M16 2v4M8 2v4M3 10h18'/%3E%3C/svg%3E");--i-check-url:url("data:image/svg+xml;utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath d='M20 6 9 17l-5-5'/%3E%3C/svg%3E");--i-chevron-url:url("data:image/svg+xml;utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath d='m9 18 6-6-6-6'/%3E%3C/svg%3E");--i-close-url:url("data:image/svg+xml;utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath d='M18 6 6 18M6 6l12 12'/%3E%3C/svg%3E");--i-discord-url:url("data:image/svg+xml;utf8,%3Csvg viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M20.317 4.37a19.791 19.791 0 0 0-4.885-1.515.074.074 0 0 0-.079.037c-.21.375-.444.864-.608 1.25a18.27 18.27 0 0 0-5.487 0 12.64 12.64 0 0 0-.617-1.25.077.077 0 0 0-.079-.037A19.736 19.736 0 0 0 3.677 4.37a.07.07 0 0 0-.032.027C.533 9.046-.32 13.58.099 18.057a.082.082 0 0 0 .031.057 19.9 19.9 0 0 0 5.993 3.03.078.078 0 0 0 .084-.028 14.09 14.09 0 0 0 1.226-1.994.076.076 0 0 0-.041-.106 13.107 13.107 0 0 1-1.872-.892.077.077 0 0 1-.008-.128 10.2 10.2 0 0 0 .372-.292.074.074 0 0 1 .077-.01c3.928 1.793 8.18 1.793 12.062 0a.074.074 0 0 1 .078.01c.12.098.246.198.373.292a.077.077 0 0 1-.006.127 12.299 12.299 0 0 1-1.873.892.077.077 0 0 0-.041.107c.36.698.772 1.362 1.225 1.993a.076.076 0 0 0 .084.028 19.839 19.839 0 0 0 6.002-3.03.077.077 0 0 0 .032-.054c.5-5.177-.838-9.674-3.549-13.66a.061.061 0 0 0-.031-.03zM8.02 15.33c-1.183 0-2.157-1.085-2.157-2.419 0-1.333.956-2.419 2.157-2.419 1.21 0 2.176 1.096 2.157 2.42 0 1.333-.956 2.418-2.157 2.418zm7.975 0c-1.183 0-2.157-1.085-2.157-2.419 0-1.333.955-2.419 2.157-2.419 1.21 0 2.176 1.096 2.157 2.42 0 1.333-.946 2.418-2.157 2.418z'/%3E%3C/svg%3E");--i-flame-url:url("data:image/svg+xml;utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath d='M8.5 14.5A2.5 2.5 0 0 0 11 12c0-1.38-.5-2-1-3-1.072-2.143-.224-4.054 2-6 .5 2.5 2 4.9 4 6.5 2 1.6 3 3.5 3 5.5a7 7 0 1 1-14 0c0-1.153.433-2.294 1-3a2.5 2.5 0 0 0 2.5 2.5z'/%3E%3C/svg%3E");--i-git-fork-url:url("data:image/svg+xml;utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Ccircle cx='12' cy='18' r='3'/%3E%3Ccircle cx='6' cy='6' r='3'/%3E%3Ccircle cx='18' cy='6' r='3'/%3E%3Cpath d='M18 9v1a2 2 0 0 1-2 2H8a2 2 0 0 1-2-2V9M12 12v3'/%3E%3C/svg%3E");--i-github-url:url("data:image/svg+xml;utf8,%3Csvg viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M12 .297c-6.63 0-12 5.373-12 12 0 5.303 3.438 9.8 8.205 11.385.6.113.82-.258.82-.577 0-.285-.01-1.04-.015-2.04-3.338.724-4.042-1.61-4.042-1.61C4.422 18.07 3.633 17.7 3.633 17.7c-1.087-.744.084-.729.084-.729 1.205.084 1.838 1.236 1.838 1.236 1.07 1.835 2.809 1.305 3.495.998.108-.776.417-1.305.76-1.605-2.665-.3-5.466-1.332-5.466-5.93 0-1.31.465-2.38 1.235-3.22-.135-.303-.54-1.523.105-3.176 0 0 1.005-.322 3.3 1.23.96-.267 1.98-.399 3-.405 1.02.006 2.04.138 3 .405 2.28-1.552 3.285-1.23 3.285-1.23.645 1.653.24 2.873.12 3.176.765.84 1.23 1.91 1.23 3.22 0 4.61-2.805 5.625-5.475 5.92.42.36.81 1.096.81 2.22 0 1.606-.015 2.896-.015 3.286 0 .315.21.69.825.57C20.565 22.092 24 17.592 24 12.297c0-6.627-5.373-12-12-12'/%3E%3C/svg%3E");--i-gitlab-url:url("data:image/svg+xml;utf8,%3Csvg viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='m23.6 9.593-.033-.086L20.3.98a.851.851 0 0 0-.336-.405.875.875 0 0 0-1 .054.875.875 0 0 0-.29.44L16.47 7.818H7.537L5.332 1.07a.857.857 0 0 0-.29-.441.875.875 0 0 0-1-.054.859.859 0 0 0-.336.405L.433 9.502l-.032.086a6.066 6.066 0 0 0 2.012 7.01l.01.009.03.021 4.977 3.727 2.462 1.863 1.5 1.132a1.008 1.008 0 0 0 1.22 0l1.499-1.132 2.461-1.863 5.006-3.75.013-.01a6.068 6.068 0 0 0 2.01-7.002z'/%3E%3C/svg%3E");--i-help-url:url("data:image/svg+xml;utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Ccircle cx='12' cy='12' r='10'/%3E%3Cpath d='M9.09 9a3 3 0 0 1 5.83 1c0 2-3 3-3 3m.08 4h.01'/%3E%3C/svg%3E");--i-laptop-url:url("data:image/svg+xml;utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Crect x='3' y='4' width='18' height='12' rx='2' ry='2'/%3E%3Cpath d='M2 20h20'/%3E%3C/svg%3E");--i-link-url:url("data:image/svg+xml;utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath d='M10 13a5 5 0 0 0 7.54.54l3-3a5 5 0 0 0-7.07-7.07l-1.72 1.71'/%3E%3Cpath d='M14 11a5 5 0 0 0-7.54-.54l-3 3a5 5 0 0 0 7.07 7.07l1.71-1.71'/%3E%3C/svg%3E");--i-mastodon-url:url("data:image/svg+xml;utf8,%3Csvg viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M23.268 5.313c-.35-2.578-2.617-4.61-5.304-5.004C17.51.242 15.792 0 11.813 0h-.03c-3.98 0-4.835.242-5.288.309C3.882.692 1.496 2.518.917 5.127.64 6.412.61 7.837.661 9.143c.074 1.874.088 3.745.26 5.611.118 1.24.325 2.47.62 3.68.55 2.237 2.777 4.098 4.96 4.857 2.336.792 4.849.923 7.256.38.265-.061.527-.132.786-.213.585-.184 1.27-.39 1.774-.753a.057.057 0 0 0 .023-.043v-1.809a.052.052 0 0 0-.02-.041.053.053 0 0 0-.046-.01 20.282 20.282 0 0 1-4.709.545c-2.73 0-3.463-1.284-3.674-1.818a5.593 5.593 0 0 1-.319-1.433.053.053 0 0 1 .066-.054c1.517.363 3.072.546 4.632.546.376 0 .75 0 1.125-.01 1.57-.044 3.224-.124 4.768-.422.038-.008.077-.015.11-.024 2.435-.464 4.753-1.92 4.989-5.604.008-.145.03-1.52.03-1.67.002-.512.167-3.63-.024-5.545zm-3.748 9.195h-2.561V8.29c0-1.309-.55-1.976-1.67-1.976-1.23 0-1.846.79-1.846 2.35v3.403h-2.546V8.663c0-1.56-.617-2.35-1.848-2.35-1.112 0-1.668.668-1.67 1.977v6.218H4.822V8.102c0-1.31.337-2.35 1.011-3.12.696-.77 1.608-1.164 2.74-1.164 1.311 0 2.302.5 2.962 1.498l.638 1.06.638-1.06c.66-.999 1.65-1.498 2.96-1.498 1.13 0 2.043.395 2.74 1.164.675.77 1.012 1.81 1.012 3.12z'/%3E%3C/svg%3E");--i-milestone-url:url("data:image/svg+xml;utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath d='M18 6H5a2 2 0 0 0-2 2v3a2 2 0 0 0 2 2h13l4-3.5L18 6zM12 13v8M12 3v3'/%3E%3C/svg%3E");--i-moon-url:url("data:image/svg+xml;utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath d='M12 3a6.364 6.364 0 0 0 9 9 9 9 0 1 1-9-9z'/%3E%3C/svg%3E");--i-outdent-url:url("data:image/svg+xml;utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath d='m7 8-4 4 4 4M21 12H11M21 6H11M21 18H11'/%3E%3C/svg%3E");--i-rocket-url:url("data:image/svg+xml;utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath d='M4.5 16.5c-1.5 1.26-2 5-2 5s3.74-.5 5-2c.71-.84.7-2.13-.09-2.91a2.18 2.18 0 0 0-2.91-.09zM12 15l-3-3a22 22 0 0 1 2-3.95A12.88 12.88 0 0 1 22 2c0 2.72-.78 7.5-6 11a22.35 22.35 0 0 1-4 2z'/%3E%3Cpath d='M9 12H4s.55-3.03 2-4c1.62-1.08 5 0 5 0M12 15v5s3.03-.55 4-2c1.08-1.62 0-5 0-5'/%3E%3C/svg%3E");--i-skull-url:url("data:image/svg+xml;utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Ccircle cx='9' cy='12' r='1'/%3E%3Ccircle cx='15' cy='12' r='1'/%3E%3Cpath d='M8 20v2h8v-2m-3.5-3-.5-1-.5 1h1z'/%3E%3Cpath d='M16 20a2 2 0 0 0 1.56-3.25 8 8 0 1 0-11.12 0A2 2 0 0 0 8 20'/%3E%3C/svg%3E");--i-star-url:url("data:image/svg+xml;utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath d='m12 2 3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01L12 2z'/%3E%3C/svg%3E");--i-sun-url:url("data:image/svg+xml;utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Ccircle cx='12' cy='12' r='4'/%3E%3Cpath d='M12 2v2m0 16v2M4.93 4.93l1.41 1.41m11.32 11.32 1.41 1.41M2 12h2m16 0h2M6.34 17.66l-1.41 1.41M19.07 4.93l-1.41 1.41'/%3E%3C/svg%3E");--i-twitter-url:url("data:image/svg+xml;utf8,%3Csvg viewBox='0 0 24 24' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M23.953 4.57a10 10 0 0 1-2.825.775 4.958 4.958 0 0 0 2.163-2.723c-.951.555-2.005.959-3.127 1.184a4.92 4.92 0 0 0-8.384 4.482C7.69 8.095 4.067 6.13 1.64 3.162a4.822 4.822 0 0 0-.666 2.475c0 1.71.87 3.213 2.188 4.096a4.904 4.904 0 0 1-2.228-.616v.06a4.923 4.923 0 0 0 3.946 4.827 4.996 4.996 0 0 1-2.212.085 4.936 4.936 0 0 0 4.604 3.417 9.867 9.867 0 0 1-6.102 2.105c-.39 0-.779-.023-1.17-.067a13.995 13.995 0 0 0 7.557 2.209c9.053 0 13.998-7.496 13.998-13.985 0-.21 0-.42-.015-.63A9.935 9.935 0 0 0 24 4.59z'/%3E%3C/svg%3E");--i-zap-url:url("data:image/svg+xml;utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' fill='none' stroke='currentColor' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath d='M13 2 3 14h9l-1 8 10-12h-9l1-8z'/%3E%3C/svg%3E")}.i-icon.alert{--icon-url:var(--i-alert-url)}.i-icon.arrows{--icon-url:var(--i-arrows-url)}.i-icon.award{--icon-url:var(--i-award-url)}.i-icon.bell{--icon-url:var(--i-bell-url)}.i-icon.bookmark{--icon-url:var(--i-bookmark-url)}.i-icon.calendar{--icon-url:var(--i-calendar-url)}.i-icon.check{--icon-url:var(--i-check-url)}.i-icon.chevron{--icon-url:var(--i-chevron-url)}.i-icon.close{--icon-url:var(--i-close-url)}.i-icon.discord{--icon-url:var(--i-discord-url)}.i-icon.flame{--icon-url:var(--i-flame-url)}.i-icon.git-fork{--icon-url:var(--i-git-fork-url)}.i-icon.github{--icon-url:var(--i-github-url)}.i-icon.gitlab{--icon-url:var(--i-gitlab-url)}.i-icon.help{--icon-url:var(--i-help-url)}.i-icon.laptop{--icon-url:var(--i-laptop-url)}.i-icon.link{--icon-url:var(--i-link-url)}.i-icon.mastodon{--icon-url:var(--i-mastodon-url)}.i-icon.milestone{--icon-url:var(--i-milestone-url)}.i-icon.moon{--icon-url:var(--i-moon-url)}.i-icon.outdent{--icon-url:var(--i-outdent-url)}.i-icon.rocket{--icon-url:var(--i-rocket-url)}.i-icon.skull{--icon-url:var(--i-skull-url)}.i-icon.star{--icon-url:var(--i-star-url)}.i-icon.sun{--icon-url:var(--i-sun-url)}.i-icon.twitter{--icon-url:var(--i-twitter-url)}.i-icon.zap{--icon-url:var(--i-zap-url)}.hamburger{position:relative;display:inline-block;width:16px;height:14px;overflow:hidden;cursor:pointer}.hamburger>span{position:absolute;width:16px;height:2px;left:0;background-color:var(--sy-c-text);transition:top .25s,transform .25s}.hamburger_1{top:0}.hamburger_2{top:6px}.hamburger_3{top:12px}button.hamburger[aria-expanded=true] .hamburger_1{top:6px;transform:translate(0) rotate(225deg)}button.hamburger[aria-expanded=true] .hamburger_2{top:6px;transform:translate(18px)}button.hamburger[aria-expanded=true] .hamburger_3{top:6px;transform:translate(0) rotate(135deg)}.globaltoc .caption{font-size:.86rem;font-weight:500;font-family:var(--sy-f-heading);color:var(--sy-c-text-weak);text-transform:uppercase;letter-spacing:.4px;padding:.8rem 0 .4rem;border-top:1px solid var(--sy-c-divider)}.globaltoc>p.caption:first-of-type{padding-top:0;border-top:none}.globaltoc .caption+ul{margin-bottom:1.5rem}.globaltoc ul+.caption{margin-top:3rem}.globaltoc li{margin:.6rem 0}.globaltoc>ul>li>ul{margin-left:.2rem;border-left:1px solid var(--sy-c-divider-weak);font-size:.96rem}.globaltoc li.toctree-l2{padding-left:.9rem;margin-left:-1px;border-left:1px solid #0000}.globaltoc li.toctree-l2.current{border-color:var(--sy-c-link)}.globaltoc>ul a.current{font-weight:500;color:var(--sy-c-link)}.globaltoc>ul a:hover{color:var(--sy-c-bold)}.localtoc>h3{font-size:.8rem;font-weight:500;letter-spacing:.4px;text-transform:uppercase;margin-bottom:1rem}.localtoc>ul li{margin-top:.36rem;margin-bottom:.36rem}.localtoc>ul li>a:hover{color:var(--sy-c-bold)}.localtoc>ul li.active>a{font-weight:500;color:var(--sy-c-link)}.localtoc>ul>li>ul{padding-left:.8rem}.searchbox{position:relative}.searchbox input{-webkit-appearance:none;-moz-appearance:none;appearance:none;width:100%;padding:6px 12px;font-size:.92rem;font-family:var(--sy-f-text);border-radius:6px;outline:0;background:var(--sy-c-bg-weak)}.searchbox button,.searchbox kbd{position:absolute;font-size:.68rem;font-weight:600;font-family:var(--sy-f-mono);padding:2px 6px;margin:6px;right:0;border-radius:3px;border:1px solid var(--sy-c-border);background-color:var(--sy-c-bg);opacity:1;transition:opacity .2s ease}.searchbox input:focus+kbd{opacity:0}.searchform{display:flex;position:relative;align-items:center}.searchform input[name=q]{-webkit-appearance:none;-moz-appearance:none;appearance:none;width:100%;padding:6px 12px;font-size:.92rem;font-family:var(--sy-f-text);border-radius:6px;outline:0;background:var(--sy-c-bg-weak)}.searchform input[name=q]+button{position:absolute;font-size:.68rem;font-weight:600;font-family:var(--sy-f-text);padding:2px 6px;margin:6px;right:0;border-radius:3px;border:1px solid var(--sy-c-divider);background-color:var(--sy-c-bg);opacity:1;transition:opacity .2s ease}.navigation{gap:2rem;padding-top:1rem;border-top:1px solid var(--sy-c-divider)}.navigation>div{width:100%}.navigation a{display:inline-flex;align-items:center}.navigation a:hover{color:rgba(var(--sy-rc-invert),1)}.navigation-prev i.chevron{transform:rotate(180deg)}.navigation-next{text-align:right}.navigation-next a{justify-content:end}.navigation .page-info{padding:0 8px}.navigation .page-info>span{font-size:.8rem;color:var(--sy-c-text-weak)}.demo{border:1px solid var(--sy-c-border);border-radius:6px}.demo-code .highlight>pre{border-bottom-left-radius:0;border-bottom-right-radius:0}.demo-result{padding:1rem}.yue button.copybtn{align-items:center;justify-content:center;background-color:initial;border:none;color:var(--sy-c-text)}.yue button.copybtn>svg{width:1.4rem;height:1.4rem}.yue .highlight button.copybtn:hover{background-color:initial;color:var(--sy-c-text-weak)}.yue .o-tooltip--left:after{background-color:initial;color:var(--sy-c-text)}#ethical-ad-placement .ethical-sidebar{position:relative;background-color:var(--sy-c-bg-weak);border:none;padding:.8rem}#ethical-ad-placement .ethical-text a{color:var(--sy-c-text)!important}.sy-main #ethical-ad-placement .ethical-sidebar{margin-left:0;max-width:380px}.sy-main #ethical-ad-placement .ethical-image-link{flex-shrink:0;margin-right:.4rem}.sy-main #ethical-ad-placement .ethical-content{display:flex}.sy-main #ethical-ad-placement .ethical-text{margin-top:0}.sy-main #ethical-ad-placement .ethical-callout{position:absolute;right:.4rem;bottom:.4rem}#carbonads{margin:1rem 0;position:relative;display:block;background-color:var(--sy-c-bg-weak);border:none;border-radius:8px;padding:.8rem .8rem 1.6rem}.carbon-wrap{display:flex;align-items:center;justify-content:space-between;flex-direction:column}.carbon-text{display:block;margin:.5rem 0;line-height:1.42;font-size:.78rem;text-align:center}.carbon-text:hover{color:var(--sy-c-link)}.carbon-poweredby{position:absolute;right:.8rem;bottom:.5rem;font-size:.68rem;text-transform:uppercase}.carbon-poweredby:hover{text-decoration:underline}.sy-main #carbonads{max-width:380px;padding:1rem}.sy-main .carbon-wrap{flex-direction:row}.sy-main .carbon-text{text-align:left;margin-left:1rem}.yue{--yue-c-text:var(--sy-c-text);--yue-c-heading:var(--sy-c-heading);--yue-c-bold:var(--sy-c-bold);--yue-c-link-1:var(--sy-c-text);--yue-c-link-2:#111827;--yue-c-link-border-1:rgba(var(--sy-rc-theme),0.8);--yue-c-link-border-2:var(--sy-c-link);--yue-c-ol-marker:#6b7280;--yue-c-ul-marker:#d1d5db;--yue-c-hr:#e5e7eb;--yue-c-quote:#111827;--yue-c-quote-border:#cfd3db;--yue-c-quote-symbol:rgba(var(--sy-rc-theme),1);--yue-c-caption:#6b7280;--yue-c-code:#111827;--yue-c-code-bg:#fff4d4;--yue-c-th-bg:#eff3f8;--yue-c-th-border:#d1d5db;--yue-c-td-border:#e5e7eb}html.dark .yue{--yue-c-link-1:var(--sy-c-text);--yue-c-link-2:#fff;--yue-c-ol-marker:#9ca3af;--yue-c-ul-marker:#4b5563;--yue-c-hr:#374151;--yue-c-quote:#f3f4f6;--yue-c-quote-border:#374151;--yue-c-caption:#9ca3af;--yue-c-code:#fff;--yue-c-code-bg:#312f29;--yue-c-th-bg:#24282e;--yue-c-th-border:#4b5563;--yue-c-td-border:#374151}.yue{font-size:1rem;line-height:1.75;color:var(--yue-c-text)}.yue p{margin-top:1rem;margin-bottom:1.25rem}.yue a{color:var(--yue-c-link-1);text-decoration:underline;font-weight:500;text-decoration:none;border-bottom:1px solid var(--yue-c-link-border-1)}.yue a:hover{color:var(--yue-c-link-2);border-bottom:2px solid var(--yue-c-link-border-2)}.yue strong{color:var(--yue-c-bold);font-weight:600}.yue a strong,.yue blockquote strong,.yue thead th strong{color:inherit}.yue ol{margin-top:1.25em;margin-bottom:1.25em;padding-left:1.625em}.yue ol,.yue ol[type="1"]{list-style-type:decimal}.yue ol.upperalpha,.yue ol[type=A]{list-style-type:upper-alpha}.yue ol.loweralpha,.yue ol[type=a]{list-style-type:lower-alpha}.yue ol.upperroman,.yue ol[type=I]{list-style-type:upper-roman}.yue ol.lowerroman,.yue ol[type=i]{list-style-type:lower-roman}.yue ul{list-style-type:disc;margin-top:1.25em;margin-bottom:1.25em;padding-left:1.625em}.yue ol>li::marker{font-weight:400;color:var(--yue-c-ol-marker)}.yue ul>li::marker{color:var(--yue-c-ul-marker)}.yue dl{margin-top:1.5rem;margin-bottom:1.5rem}.yue dt{color:var(--yue-c-bold);font-weight:600}.yue dd{margin-left:1.5rem}.yue hr{border-color:var(--yue-c-hr);border-top-width:1px;margin-top:3em;margin-bottom:3em}.yue blockquote{color:var(--yue-c-quote);border-left-width:.25rem;border-left-color:var(--yue-c-quote-border);margin-top:1.2rem;margin-bottom:1.2rem;padding-left:1rem}.yue blockquote .attribution{font-size:.85em;font-style:italic}[lang=ja] .yue blockquote .attribution,[lang=ko] .yue blockquote .attribution,[lang^=zh] .yue blockquote .attribution{font-style:normal}.yue h1{color:var(--yue-c-heading);font-weight:800;font-size:2.25em;margin-top:0;margin-bottom:.8888889em;line-height:1.1111111}.yue h1 strong{font-weight:900;color:inherit}.yue h2{color:var(--yue-c-heading);font-weight:700;font-size:1.5em;margin-top:2em;margin-bottom:1em;line-height:1.3333333}.yue h2 strong{font-weight:800;color:inherit}.yue h3{color:var(--yue-c-heading);font-weight:600;font-size:1.25em;margin-top:1.6em;margin-bottom:.6em;line-height:1.6}.yue h3 strong{font-weight:700;color:inherit}.yue h4{color:var(--yue-c-heading);font-weight:600;margin-top:1.5em;margin-bottom:.5em;line-height:1.5}.yue h4 strong{font-weight:700;color:inherit}.yue img{margin-top:2em;margin-bottom:2em}.yue figure>*{margin-top:0;margin-bottom:0}.yue figcaption{color:var(--yue-c-caption);font-size:.875em;line-height:1.4285714;margin-top:.8571429em}.yue code{color:var(--yue-c-code);font-weight:600;font-size:.875em}.yue a code,.yue blockquote code,.yue h1 code,.yue h2 code,.yue h3 code,.yue h4 code,.yue th code{color:inherit}.yue h2 code{font-size:.875em}.yue li>code,.yue p>code{padding-left:4px;padding-right:4px;border-radius:3px;font-weight:500;background-color:var(--yue-c-code-bg)}.yue h3 code{font-size:.9em}.yue figure,.yue video{margin-top:2em;margin-bottom:2em}.yue li{margin-top:.5em;margin-bottom:.5em}.yue ol>li,.yue ul>li{padding-left:.375em}.yue ol ol,.yue ol ul,.yue ul ol,.yue ul ul{margin-top:.75em;margin-bottom:.75em}.yue h2+*,.yue h3+*,.yue h4+*,.yue hr+*{margin-top:0}.yue table{width:100%;table-layout:auto;text-align:left;margin-top:2em;margin-bottom:2em;font-size:.86em;line-height:1.7}.yue table>caption{margin-bottom:.4rem;color:var(--yue-c-caption)}.yue thead tr{border-bottom-width:1px;border-bottom-color:var(--yue-c-th-border)}.yue thead th{color:var(--yue-c-heading);font-weight:600;vertical-align:middle;text-align:center}.yue tbody tr{border-bottom-width:1px;border-bottom-color:var(--yue-c-td-border)}.yue tbody tr:last-child{border-bottom-width:0}.yue tbody td{vertical-align:middle}.yue tfoot{border-top-width:1px;border-top-color:var(--yue-c-th-border)}.yue tfoot td{vertical-align:top}.yue td>p{margin:.25rem 0}.yue thead th>p{margin:0}.yue tbody td,.yue tfoot td,.yue thead th{padding:.5rem}.yue section>div{margin-bottom:2rem}.yue dd>p:first-child{margin-top:0}.yue dl.simple>dd>p,.yue ul.simple>li>p{margin:0}.yue a.headerlink{visibility:hidden;margin-left:6px;color:rgba(var(--sy-rc-text),.6);font-weight:300;font-family:var(--sy-f-mono)}.yue .math a.headerlink,h2:hover a.headerlink,h3:hover a.headerlink,h4:hover a.headerlink,h5:hover a.headerlink,h6:hover a.headerlink{visibility:visible}.yue .toctree-wrapper a{border-bottom:none}.yue .toctree-wrapper p.caption{font-size:.86rem;font-weight:500;font-family:var(--sy-f-heading);color:var(--sy-c-text-weak);text-transform:uppercase;letter-spacing:.4px;padding:.8rem 0 .4rem;border-bottom:1px solid var(--sy-c-divider)}.yue .align-center{display:block;text-align:center}.yue .align-center,.yue figure.align-center img{margin-left:auto;margin-right:auto}a.footnote-reference{font-size:.65rem;vertical-align:top}aside.footnote>span,div.citation>span{float:left;font-weight:500;padding-right:.25rem}aside.footnote>p,div.citation>p{margin-bottom:.5rem;margin-top:.5rem;margin-left:2rem}.yue kbd.kbd:not(.compound){font-size:.86rem;padding:2px 5px;border-radius:3px;margin-right:.25rem}.yue kbd.compound>kbd{margin-left:.25rem}.light .yue kbd.kbd:not(.compound){background:linear-gradient(-225deg,#e6e6e6,#f8f8f8);box-shadow:inset 0 -2px #dbdbdb,inset 0 0 1px 1px #fff,0 1px 2px 1px #50505066}.dark .yue kbd.kbd:not(.compound){background:linear-gradient(-225deg,#353434,#141414);box-shadow:inset 0 -2px #373737,inset 0 0 1px 1px #222,0 1px 2px 1px #000}.hlist td{vertical-align:top}p.centered{text-align:center}:root,html.light{--admonition-bg-opacity:0.03;--admonition-head-opacity:0.08;--admonition-border-opacity:1}@media (prefers-color-scheme:dark){:root{--admonition-bg-opacity:0.08;--admonition-head-opacity:0.15;--admonition-border-opacity:0.8}}html.dark{--admonition-bg-opacity:0.08;--admonition-head-opacity:0.15;--admonition-border-opacity:0.8}:root{--attention-icon:var(--i-alert-url);--attention-color:247,89,171;--caution-icon:var(--i-zap-url);--caution-color:247,186,42;--danger-icon:var(--i-skull-url);--danger-color:255,92,47;--error-icon:var(--i-close-url);--error-color:255,92,47;--hint-icon:var(--i-bell-url);--hint-color:0,200,80;--important-icon:var(--i-flame-url);--important-color:179,127,235;--note-icon:var(--i-calendar-url);--note-color:3,169,244;--tip-icon:var(--i-rocket-url);--tip-color:0,200,80;--warning-icon:var(--i-zap-url);--warning-color:255,145,0;--seealso-icon:var(--i-link-url);--seealso-color:60,140,255;--todo-icon:var(--i-bookmark-url);--todo-color:220,150,0;--versionadded-color:0,200,80;--versionchanged-color:247,186,42;--deprecated-color:255,92,47}.admonition{--color-rgb:var(--sy-rc-theme);--icon-url:var(--i-bell-url);position:relative;padding:0 16px .8rem;margin-top:1rem;margin-bottom:1rem;border-left:4px solid rgba(var(--color-rgb),var(--admonition-border-opacity));background-color:rgba(var(--color-rgb),var(--admonition-bg-opacity))}.admonition:before{position:absolute;content:"";top:6px;left:-12px;width:20px;height:20px;border-radius:100%;background-color:rgb(var(--color-rgb))}.admonition p.admonition-title{position:relative;margin:0 -16px .8rem -19px;padding:4px 18px;font-size:.85rem;font-weight:600;line-height:1.72;color:rgb(var(--color-rgb));background-color:rgba(var(--color-rgb),var(--admonition-head-opacity))}.admonition-title:before{position:absolute;content:"";top:10px;left:-5px;-webkit-mask:var(--icon-url) no-repeat;mask:var(--icon-url) no-repeat;-webkit-mask-size:100% 100%;mask-size:100% 100%;font-style:normal;width:12px;height:12px;background-color:#fff}.admonition.attention{--icon-url:var(--attention-icon);--color-rgb:var(--attention-color)}.admonition.caution{--icon-url:var(--caution-icon);--color-rgb:var(--caution-color)}.admonition.danger{--icon-url:var(--danger-icon);--color-rgb:var(--danger-color)}.admonition.error{--icon-url:var(--error-icon);--color-rgb:var(--error-color)}.admonition.hint{--icon-url:var(--hint-icon);--color-rgb:var(--hint-color)}.admonition.important{--icon-url:var(--important-icon);--color-rgb:var(--important-color)}.admonition.note{--icon-url:var(--note-icon);--color-rgb:var(--note-color)}.admonition.tip{--icon-url:var(--tip-icon);--color-rgb:var(--tip-color)}.admonition.warning{--icon-url:var(--warning-icon);--color-rgb:var(--warning-color)}.admonition.seealso{--icon-url:var(--seealso-icon);--color-rgb:var(--seealso-color)}.admonition.admonition-todo{--icon-url:var(--todo-icon);--color-rgb:var(--todo-color)}.admonition p.admonition-title+p{margin-top:0}.admonition>:last-child{margin-bottom:0}span.versionmodified{color:var(--sy-c-bold);font-weight:600}div.deprecated,div.versionadded,div.versionchanged{--version-color:var(--sy-rc-theme);position:relative;padding:6px 1rem;margin:1rem 0;border-left:4px solid rgba(var(--version-color),1);background-color:rgba(var(--version-color),.08);line-height:1.72}div.deprecated:before,div.versionadded:before,div.versionchanged:before{position:absolute;content:var(--version-icon);top:10px;left:-12px;color:#fff;width:20px;height:20px;border-radius:100%;background-color:rgba(var(--version-color),1);text-align:center;font:normal 700 14px/20px var(--sy-f-mono)}div.versionadded{--version-color:var(--versionadded-color);--version-icon:"#"}div.versionchanged{--version-color:var(--versionchanged-color);--version-icon:"%"}div.deprecated{--version-color:var(--deprecated-color);--version-icon:"!"}div.deprecated>p,div.versionadded>p,div.versionchanged>p{margin:0}.yue blockquote.epigraph{padding:1rem 2.4rem;border-left:0;text-align:center}.yue blockquote.highlights{border-left-width:4px;padding-top:.2rem;padding-bottom:.2rem;background-color:var(--sy-c-bg-weak)}.yue blockquote.pull-quote{position:relative;font-size:1.24rem;padding:2.4rem 3.6rem 1.2rem;border-left:0}.yue blockquote.pull-quote:before{content:"\201c";position:absolute;top:0;left:.5rem;color:var(--yue-c-quote-symbol);font:700 4rem/1 Times New Roman,Georgia,Palatino,Times,serif}.yue blockquote.pull-quote .attribution{text-align:right}pre.literal-block{line-height:1.48;padding:1rem;font-size:.96rem;background-color:var(--syntax-pre-bg);border-radius:6px;overflow:auto}.highlight,.literal-block-wrapper{--margin:1rem;--radius:6px}.highlight>pre{display:grid;line-height:1.48;padding:var(--margin);font-size:.96rem;background-color:var(--syntax-pre-bg);border-radius:var(--radius);overflow:auto}.highlight .linenos{display:inline-block;box-shadow:-.05rem 0 rgba(var(--sy-rc-invert),.2) inset;-webkit-user-select:none;-moz-user-select:none;user-select:none;margin-right:.8rem;padding-right:.8rem;opacity:.6}.highlight .hll{margin-left:calc(0rem - var(--margin));margin-right:calc(0rem - var(--margin));padding:0 var(--margin)}.code-block-caption{font-size:.84rem;font-weight:600;color:var(--syntax-text);background-color:var(--syntax-cap-bg);padding:.4rem var(--margin);border-radius:var(--radius) var(--radius) 0 0}.code-block-caption+div>.highlight>pre{border-top-left-radius:0;border-top-right-radius:0}.yue .table-wrapper{width:100%;overflow-x:auto;margin-top:2rem;margin-bottom:2rem}.yue .table-wrapper>table{margin:0}.yue .table-wrapper thead tr{border-top:1px solid var(--yue-c-td-border)}.yue .table-wrapper th{background-color:var(--yue-c-th-bg);border-left:1px solid var(--yue-c-td-border)}.yue .table-wrapper td,.yue .table-wrapper th:last-child{border-right:1px solid var(--yue-c-td-border)}.yue .table-wrapper td{border-left:1px solid var(--yue-c-td-border)}.yue .table-wrapper tbody tr:first-child{border-top:1px solid var(--yue-c-td-border)}.yue .table-wrapper tbody tr:last-child{border-bottom-width:1px}.yue .table-wrapper thead+tbody tr:first-child{border-top-width:0}.yue table.hlist td{vertical-align:top}.table-wrapper{overflow-x:auto;scrollbar-gutter:stable}.table-wrapper::-webkit-scrollbar{height:.75rem;width:.75rem}.table-wrapper::-webkit-scrollbar-thumb{border-radius:10px}.table-wrapper::-webkit-scrollbar-track{background-color:initial}.table-wrapper:hover::-webkit-scrollbar-thumb{background-color:#9b9b9b33;background-clip:content-box;border:3px solid #0000}dt.sig{position:relative;font-size:.92rem;padding:.25rem .5rem .25rem 3rem;text-indent:-2.4rem;border-radius:6px}dt.sig:after{content:"";display:table;clear:both}dt.sig:hover{background:var(--sy-c-bg-weak)}dt.sig+dd{font-size:.92rem;margin-left:2rem}dt.sig>em.property:first-child{color:var(--syntax-keyword)}dl.field-list a{font-weight:400}dt.sig+dd>div{margin-bottom:1rem}dt.sig+dd>dl.field-list>dt{text-transform:uppercase;font-size:.76rem}em.property,em.sig-param{font-style:normal}em.sig-param{color:var(--sy-c-text-weak)}span.sig-name,span.sig-prename{color:var(--syntax-property)}span.sig-name{font-weight:600}span.sig-return-icon{color:var(--sy-c-text-weak)}span.sig-return-typehint,span.sig-return-typehint>a{color:var(--syntax-constant)}span.pre,span.sig-paren{font-family:var(--sy-f-mono)}dt.sig>a.internal{font-size:.82rem;border:0;color:var(--sy-c-text-weak)}dt.sig>a.internal:before{content:"\a";white-space:pre}.viewcode-block{position:relative}.viewcode-back{position:absolute;top:-1.5rem;font-size:.8rem}:root,html.light{--syntax-pre-bg:#f3f1fa;--syntax-cap-bg:#eae7f7;--syntax-text:#24292f;--syntax-meta:#a6a2ae;--syntax-comment:#6e7781;--syntax-constant:#0550ae;--syntax-entity:#268bd2;--syntax-property:#8250df;--syntax-definition:#24292f;--syntax-tag:#085;--syntax-builtin:#b58900;--syntax-keyword:#cf222e;--syntax-exception:#e6212e;--syntax-string:#0a3069;--syntax-regexp:#e40;--syntax-variable:#a4480f;--syntax-invalid-illegal-text:#f6f8fa;--syntax-invalid-illegal-bg:#82071e;--syntax-markup-heading:#0550ae;--syntax-markup-italic:#24292f;--syntax-markup-bold:#24292f;--syntax-markup-deleted-text:#82071e;--syntax-markup-deleted-bg:#ffebe9;--syntax-markup-inserted-text:#116329;--syntax-markup-inserted-bg:#dafbe1;--syntax-markup-changed-text:#953800;--syntax-markup-changed-bg:#ffd8b5;--syntax-markup-ignored-text:#eaeef2;--syntax-markup-ignored-bg:#0550ae;--syntax-meta-diff-range:#8250df;--syntax-highlight-bg:#eee4ff;--syntax-special-bg:#dccafa}@media (prefers-color-scheme:dark){:root{--syntax-pre-bg:#2c283b;--syntax-cap-bg:#342f47;--syntax-text:#c9d1d9;--syntax-meta:#6e7781;--syntax-comment:#8b949e;--syntax-constant:#79c0ff;--syntax-entity:#47b0fa;--syntax-property:#d2a8ff;--syntax-definition:#c9d1d9;--syntax-tag:#7ee787;--syntax-builtin:#ffd34c;--syntax-keyword:#ff7b72;--syntax-exception:#da473c;--syntax-string:#a5d6ff;--syntax-regexp:#ef954e;--syntax-variable:#ffa657;--syntax-invalid-illegal-text:#f0f6fc;--syntax-invalid-illegal-bg:#8e1519;--syntax-markup-heading:#1f6feb;--syntax-markup-italic:#c9d1d9;--syntax-markup-bold:#c9d1d9;--syntax-markup-deleted-text:#ffdcd7;--syntax-markup-deleted-bg:#67060c;--syntax-markup-inserted-text:#aff5b4;--syntax-markup-inserted-bg:#033a16;--syntax-markup-changed-text:#ffdfb6;--syntax-markup-changed-bg:#5a1e02;--syntax-markup-ignored-text:#c9d1d9;--syntax-markup-ignored-bg:#1158c7;--syntax-meta-diff-range:#d2a8ff;--syntax-highlight-bg:#423551;--syntax-special-bg:#4f425d}}.dark-code,html.dark{--syntax-pre-bg:#2c283b;--syntax-cap-bg:#342f47;--syntax-text:#c9d1d9;--syntax-meta:#6e7781;--syntax-comment:#8b949e;--syntax-constant:#79c0ff;--syntax-entity:#47b0fa;--syntax-property:#d2a8ff;--syntax-definition:#c9d1d9;--syntax-tag:#7ee787;--syntax-builtin:#ffd34c;--syntax-keyword:#ff7b72;--syntax-exception:#da473c;--syntax-string:#a5d6ff;--syntax-regexp:#ef954e;--syntax-variable:#ffa657;--syntax-invalid-illegal-text:#f0f6fc;--syntax-invalid-illegal-bg:#8e1519;--syntax-markup-heading:#1f6feb;--syntax-markup-italic:#c9d1d9;--syntax-markup-bold:#c9d1d9;--syntax-markup-deleted-text:#ffdcd7;--syntax-markup-deleted-bg:#67060c;--syntax-markup-inserted-text:#aff5b4;--syntax-markup-inserted-bg:#033a16;--syntax-markup-changed-text:#ffdfb6;--syntax-markup-changed-bg:#5a1e02;--syntax-markup-ignored-text:#c9d1d9;--syntax-markup-ignored-bg:#1158c7;--syntax-meta-diff-range:#d2a8ff;--syntax-highlight-bg:#423551;--syntax-special-bg:#4f425d}.yue{--sd-color-primary:rgb(var(--sy-rc-theme));--sd-color-success:#00c850;--sd-color-warning:#ff9100;--sd-color-danger:#ff5c2f;--sd-color-card-border-hover:var(--sy-c-border);--sd-color-card-border:var(--sy-c-divider);--sd-color-tabs-label-inactive:var(--sy-c-bold);--sd-color-tabs-label-active:var(--sd-color-primary);--sd-color-tabs-underline-active:var(--sd-color-primary)}.light .yue{--sd-color-shadow:#f3f4f6}.dark .yue{--sd-color-shadow:#010409}.yue .sd-container-fluid{margin-top:2rem;padding:.5rem}.yue .sd-row{--sd-gutter-x:1rem;--sd-gutter-y:1rem}.yue .sd-row-cols-1{display:grid;grid-template-columns:1fr;grid-gap:1rem}.yue .sd-row-cols-2{display:grid;grid-template-columns:1fr 1fr;grid-gap:1rem}.yue .sd-row-cols-1>.sd-col,.yue .sd-row-cols-2>.sd-col{width:100%;padding:0;margin:0}.yue .sd-card-hover:hover{transform:scale(1)}.yue .sd-card-hover:hover .sd-card-title{color:var(--sy-c-link)}.yue .sd-card a,.yue .sd-card a:hover{border-bottom:0}@media (max-width:880px){.yue .sd-row-cols-2{grid-template-columns:1fr}}.yue .sd-tab-set>label{padding:1rem .25rem .5rem;font-size:.84rem;font-weight:500}.yue .sd-tab-set>label~label{margin-left:1rem}.yue .sd-tab-content{padding:0;box-shadow:0 -.0625rem var(--sy-c-divider)}.yue .sd-tab-content .highlight pre{border-radius:0}@media (print){.yue .sd-card{page-break-inside:avoid}}.yue a.sd-text-wrap{border-bottom:0}.sphinx-tabs [role=tablist]{border-color:var(--sy-c-divider)}.yue .sphinx-tabs-tab{color:var(--sy-c-text);line-height:inherit;padding:1rem .25rem .5rem;font-size:.84rem;font-weight:500;border:none;border-bottom:.125rem solid #0000}.yue .sphinx-tabs-tab:hover{color:var(--sd-color-tabs-label-hover);border-color:var(--sd-color-tabs-underline-hover)}.yue .sphinx-tabs-tab[aria-selected=true]{border:none;border-bottom:.125rem solid var(--sd-color-tabs-underline-active);color:var(--sd-color-tabs-label-active);background-color:initial}.yue .sphinx-tabs-tab+.sphinx-tabs-tab{margin-left:1rem}.yue .sphinx-tabs-panel{border:none;padding:0;margin:0;border-radius:0;background-color:initial}.yue .sphinx-tabs-panel.code-tab{padding:0}.yue .sphinx-tabs-panel.code-tab .highlight pre{border-radius:0}.announcement{position:sticky;top:0;left:0;width:100%;padding:.8rem 2rem;display:flex;align-items:center;color:var(--sy-c-banner,#fff);background-color:var(--sy-c-banner-bg,rgba(var(--sy-rc-theme),1));z-index:20}.announcement a{text-decoration:underline}.announcement ::-moz-selection{color:var(--sy-c-banner,#fff)}.announcement ::selection{color:var(--sy-c-banner,#fff)}.announcement-inner{width:100%;text-align:center}.announcement-close{position:absolute;top:.8rem;right:1rem}.sy-head{position:sticky;top:var(--sy-s-banner-height);height:var(--sy-s-navbar-height);background-color:initial;z-index:20}.sy-head-blur{position:absolute;top:0;left:0;width:100%;height:100%;-webkit-backdrop-filter:blur(12px);backdrop-filter:blur(12px);background-color:rgba(var(--sy-rc-bg),.85);z-index:-1;--tw-shadow:0 2px 4px rgba(var(--sy-rc-invert),.02),0 1px 0 rgba(var(--sy-rc-invert),.06);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow)}.sy-head-inner{display:flex;padding-left:max(env(safe-area-inset-right),1.5rem);padding-right:max(env(safe-area-inset-right),1.5rem);justify-content:space-between;align-items:center;height:var(--sy-s-navbar-height)}.sy-head-actions>.rst-versions{position:relative;width:auto;background:#0000;color:var(--sy-c-text)}.sy-head-actions>.rst-versions>label{display:inline-block;cursor:pointer;font-size:.86rem;font-weight:500;background-color:var(--sy-c-bg-weak);border-radius:2rem;color:var(--sy-c-text-weak);padding:.24rem 1rem}.sy-head-actions>.rst-versions>label:hover{background-color:rgba(var(--sy-rc-invert),.08)}.sy-head-actions>.rst-versions>label .i-icon{transform:rotate(90deg)}.sy-head-actions input+.rst-other-versions{position:absolute;display:none;padding:0;top:2.4rem;width:300px;background-color:var(--sy-c-bg);border-radius:6px;box-shadow:0 0 3px rgba(var(--sy-rc-invert),.1),0 0 2px rgba(var(--sy-rc-invert),.2) inset}@media (max-width:767px){.sy-head-actions input+.rst-other-versions{right:-4rem}}.sy-head-actions input:checked+.rst-other-versions{display:block}.sy-head-actions .rst-other-versions>ul>li+li{border-top:1px solid var(--sy-c-divider)}.sy-head-actions .rst-other-versions>ul>li>a{display:block;padding:.5rem 1rem;color:var(--sy-c-text)}.sy-head-actions .rst-other-versions>ul>li>a:hover{color:var(--sy-c-link);background:var(--sy-c-bg-weak)}.sy-head-actions .injected .rst-versions{position:static;color:var(--sy-c-text);background-color:initial}.sy-head-actions .injected .rst-versions a{color:var(--sy-c-text)!important}.sy-head-actions .injected .rst-versions a:hover{color:var(--sy-c-link)!important}.sy-head-actions .injected .rst-current-version{display:none!important;border-radius:6px}.sy-head-actions .injected .rst-other-versions{display:block}.sy-head-actions .injected .rst-other-versions dt{font-size:.68rem;font-weight:500;text-transform:uppercase;letter-spacing:.2px;color:var(--sy-c-text-weak)}.sy-head-actions .injected .rst-other-versions hr{border-color:var(--sy-c-divider)}.sy-head-actions .injected form.wy-form input{-webkit-appearance:none;-moz-appearance:none;appearance:none;width:100%;padding:6px 12px;font-size:.92rem;font-family:var(--sy-f-text);border-radius:6px;outline:0;background:var(--sy-c-bg-weak)}.sy-head-actions .i-icon{font-size:1.25rem}.sy-head-brand img{height:28px}.sy-head-brand .dark-logo,.sy-head-brand img+strong{display:none}.dark .sy-head-brand .dark-logo{display:inline}.dark .sy-head-brand .light-logo{display:none}.light .sy-head-brand .light-logo{display:inline}.light .sy-head-brand .dark-logo{display:none}.sy-head-nav .link{display:inline-flex;align-items:center;height:var(--sy-s-navbar-height)}.sy-head-nav a{padding:.5rem;font-size:.95rem;font-weight:500;white-space:nowrap}.sy-head-nav a:hover{color:rgba(var(--sy-rc-invert),1)}.sy-head-nav .link:hover>a{background-color:var(--sy-c-bg-weak);border-radius:6px}.sy-head-nav .link i.chevron{transform:rotate(90deg)}.sy-head-nav .link>ul{position:absolute;height:0;visibility:hidden;background-color:var(--sy-c-bg);top:var(--sy-s-offset-top);margin-top:-10px;padding:15px;border-radius:6px;border:1px solid var(--sy-c-divider);box-shadow:0 12px 32px rgba(var(--sy-rc-invert),.1),0 2px 6px rgba(var(--sy-rc-invert),.08);z-index:9}.sy-head-nav .link:hover>ul{height:auto;visibility:visible}.sy-head-nav .link>ul>li{padding:.2rem 0}.sy-head-nav .link>ul a{display:block}.sy-head-nav .link>ul a:hover{background:var(--sy-c-bg-weak);border-radius:6px}.sy-head-nav .link>ul small{display:block;color:var(--sy-c-text-weak);font-weight:400}.sy-foot{border-top:1px solid var(--sy-c-foot-divider);padding-top:1.5rem;padding-bottom:1rem;color:var(--sy-c-foot-text);background-color:var(--sy-c-foot-bg)}.sy-foot-inner{padding-left:max(env(safe-area-inset-right),1.5rem);padding-right:max(env(safe-area-inset-right),1.5rem)}.sy-foot-copyright{font-size:.84rem}.sy-foot-copyright a{font-weight:500}.sy-foot-socials a{font-size:1.4rem;color:var(--sy-c-foot-text)}.sy-foot-socials a+a{margin-left:.5rem}@media (max-width:767px){#lside{position:fixed;z-index:15;top:calc(var(--sy-s-offset-top) - 1px);bottom:0;width:100%;height:calc(100vh - var(---sy-s-offset-top));overflow:auto;background:rgba(var(--sy-rc-bg),.98);transform:translateY(-100%);transition:transform .2s ease}body[data-expanded-lside=true]{overflow:hidden}#lside._expanded{transform:translateY(0)}}@media (max-width:1279px){.sy-rside{position:fixed;z-index:25;top:0;right:0;bottom:0;width:20rem;max-width:100%;padding-top:2rem;padding-bottom:1rem;overflow:auto;background:var(--sy-c-bg);transform:translateX(110%);transition:transform .2s ease;--tw-shadow:-12px 0 16px rgba(var(--sy-rc-bg),0.16);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow)}#rside._expanded{transform:translateX(0)}.rside-close{position:absolute;top:1rem;right:1rem;border:1px solid var(--sy-c-divider);width:1.5rem;height:1.5rem;display:flex;align-items:center;justify-content:center;border-radius:100%}.rside-overlay{position:fixed;top:0;left:0;width:0;height:0;background-color:rgba(var(--sy-rc-invert),.24);opacity:0;transition:width 0 .25s,height 0 .25s,opacity .25s}#rside._expanded+.rside-overlay{width:100%;height:100%;opacity:1;z-index:22}}@media (min-width:768px){.sy-main{width:calc(100% - 16rem);max-width:52rem}}@media (min-width:1280px){.sy-main{width:calc(100% - 32rem)}.sy-rside .sy-scrollbar{max-height:calc(100vh - var(--sy-s-offset-top) - env(safe-area-inset-bottom))}}.yue .viewcode-block,.yue section{scroll-margin-top:calc(var(--sy-s-offset-top) + 24px)}.sy-content{max-width:64rem;min-height:calc(100vh - var(--sy-s-offset-top))}.sy-lside-top{background:var(--sy-c-bg-weak);border-bottom:1px solid var(--sy-c-divider)}.sy-lside-top .searchbox input{border:1px solid var(--sy-c-divider)}.sy-lside li{margin:.6rem 0}.sy-lside li.link>span{font-size:.86rem;font-weight:500;font-family:var(--sy-f-heading);color:var(--sy-c-text-weak);text-transform:uppercase;letter-spacing:.4px}.sy-lside li.link .i-icon{display:none}.sy-lside li.link>ul{margin-left:1rem}.sy-lside li.link>ul small{display:none}.sy-lside .sidebar-links{margin-bottom:2rem}.sy-lside .sidebar-links span{display:inline-block;vertical-align:middle}.sy-lside .sidebar-links .icon{padding:.1rem;border-radius:6px;border:1px solid var(--sy-c-border);margin-right:.4rem;opacity:.8}.sy-lside .sidebar-links svg{width:1.5rem;height:1.5rem}.sy-lside .sidebar-links a:hover .icon{opacity:1}.repo-stats{margin:1rem 0;padding:.5rem 0;border-top:1px solid var(--sy-c-divider);border-bottom:1px solid var(--sy-c-divider)}.repo-stats-count{color:var(--sy-c-text-weak)}.repo-stats:hover .repo-stats-count{color:var(--sy-c-text)}.repo-stats strong{font-weight:500;font-family:var(--sy-f-mono);color:inherit}.edit-this-page{border-top:1px solid var(--sy-c-divider);margin:1rem 0;padding:.5rem 0;font-size:.8rem;font-weight:600}.repo-stats+.edit-this-page{border-top:0;margin-top:0;padding-top:0}.edit-this-page a{color:var(--sy-c-text-weak)}.edit-this-page a:hover{color:var(--sy-c-text)}.edit-this-page a:after{content:" →"}@media (min-width:768px){.sy-lside .sy-lside-inner{top:var(--sy-s-offset-top)}.sy-lside .sy-scrollbar{height:calc(100vh - var(--sy-s-offset-top));overflow-x:hidden}}@media print{.print\:hidden{display:none}.print\:pt-6{padding-top:1.5rem}}@media not all and (min-width:640px){.max-sm\:max-w-full{max-width:100%}}@media (min-width:768px){.md\:sticky{position:sticky}.md\:block{display:block}.md\:flex{display:flex}.md\:hidden{display:none}.md\:w-64{width:16rem}.md\:shrink-0{flex-shrink:0}}@media (min-width:1280px){.xl\:sticky{position:sticky}.xl\:top-16{top:4rem}.xl\:hidden{display:none}.xl\:px-12{padding-left:3rem;padding-right:3rem}.xl\:pl-0{padding-left:0}.xl\:pt-6{padding-top:1.5rem}}
```

### Comparing `shibuya-2023.3.7/src/shibuya/theme/shibuya/static/shibuya.js` & `shibuya-2023.6.7/src/shibuya/theme/shibuya/static/shibuya.js`

 * *Files 27% similar despite different names*

#### js-beautify {}

```diff
@@ -1,94 +1,102 @@
 (() => {
     function p(t) {
         let e = t.getAttribute("aria-controls"),
-            s = document.getElementById(e),
-            o = "data-expanded-" + e;
+            o = document.getElementById(e),
+            s = "data-expanded-" + e;
         t.addEventListener("click", function() {
-            document.body.hasAttribute(o) ? (document.body.removeAttribute(o), s.classList.remove("_expanded"), d(e, "false")) : (document.body.setAttribute(o, "true"), s.classList.add("_expanded"), d(e, "true"))
+            document.body.hasAttribute(s) ? (document.body.removeAttribute(s), o.classList.remove("_expanded"), u(e, "false")) : (document.body.setAttribute(s, "true"), o.classList.add("_expanded"), u(e, "true"))
         })
     }
 
-    function d(t, e) {
-        let s = document.querySelectorAll('[aria-controls="' + t + '"]');
-        for (el of s) el.setAttribute("aria-expanded", e)
-    }
-    var u = document.querySelectorAll(".js-menu");
-    for (let t = 0; t < u.length; t++) p(u[t]);
-    var m = document.querySelector(".banner-close");
-    m && m.addEventListener("click", () => {
-        let t = document.querySelector(".banner");
-        t.parentNode.removeChild(t)
-    });
-    var g = window.matchMedia && window.matchMedia("(prefers-color-scheme: dark)").matches,
-        i = document.documentElement;
+    function u(t, e) {
+        let o = document.querySelectorAll('[aria-controls="' + t + '"]');
+        for (el of o) el.setAttribute("aria-expanded", e)
+    }
+    var m = document.querySelectorAll(".js-menu");
+    for (let t = 0; t < m.length; t++) p(m[t]);
+    var a = document.querySelector(".announcement"),
+        g = document.querySelector(".announcement-close");
+    if (a) {
+        let e = function() {
+            t.textContent = `:root{--sy-s-banner-height:${a.clientHeight}px}`
+        };
+        k = e;
+        let t = document.createElement("style");
+        document.head.appendChild(t), g.addEventListener("click", () => {
+            a.parentNode.removeChild(a), document.head.removeChild(t)
+        }), e(), window.addEventListener("resize", e)
+    }
+    var k;
+    var y = window.matchMedia && window.matchMedia("(prefers-color-scheme: dark)").matches,
+        d = document.documentElement;
 
-    function b() {
-        let t = i.classList.contains("dark"),
+    function S() {
+        let t = d.classList.contains("dark"),
             e = t ? "dark" : "light";
-        i.classList.remove(e);
-        let s = t ? "light" : "dark";
-        f(s), sessionStorage._theme = s
-    }
-    var c = document.querySelector(".js-theme");
-
-    function f(t) {
-        i.classList.add(t);
-        let e = c.getAttribute("data-aria-" + t);
-        c.setAttribute("aria-label", e)
+        d.classList.remove(e);
+        let o = t ? "light" : "dark";
+        h(o), sessionStorage._theme = o
+    }
+    var r = document.querySelector(".js-theme");
+
+    function h(t) {
+        d.classList.add(t);
+        let e = r.getAttribute("data-aria-" + t);
+        r.setAttribute("aria-label", e)
     }
-    if (c) {
-        let t = g ? "dark" : "light",
+    if (r) {
+        let t = y ? "dark" : "light",
             e = sessionStorage._theme || t;
-        f(e), c.addEventListener("click", b)
+        h(e), r.addEventListener("click", S)
     }
 
-    function h() {
+    function f() {
         let t = '.localtoc a[href="' + location.hash + '"]',
             e = document.querySelector(t);
-        e && (document.querySelectorAll(".localtoc li").forEach(o => {
-            o.classList.remove("active")
+        e && (document.querySelectorAll(".localtoc li").forEach(s => {
+            s.classList.remove("active")
         }), e.parentNode.classList.add("active"))
     }
-    h();
+    f();
     window.addEventListener("hashchange", () => {
-        h()
+        f()
     }, !1);
-    var r = document.querySelector(".js-repo-stats");
-    async function y(t, e) {
-        let s = `https://api.github.com/repos/${t}/${e}`,
-            n = await (await fetch(s)).json(),
-            a = {
+    var i = document.querySelector(".js-repo-stats");
+    async function b(t, e) {
+        let o = `https://api.github.com/repos/${t}/${e}`,
+            n = await (await fetch(o)).json(),
+            c = {
                 stars: n.watchers,
                 forks: n.forks
             };
-        l(a), sessionStorage.setItem("_sy/repo/stats", JSON.stringify(a))
+        l(c), sessionStorage.setItem("_sy/repo/stats", JSON.stringify(c))
     }
-    async function S(t, e) {
-        let s = "https://gitlab.com/api/v4/projects/" + encodeURIComponent(t + "/" + e),
-            n = await (await fetch(s)).json(),
-            a = {
+    async function v(t, e) {
+        let o = "https://gitlab.com/api/v4/projects/" + encodeURIComponent(t + "/" + e),
+            n = await (await fetch(o)).json(),
+            c = {
                 stars: n.star_count,
                 forks: n.forks_count
             };
-        l(a), sessionStorage.setItem("_sy/repo/stats", JSON.stringify(a))
+        l(c), sessionStorage.setItem("_sy/repo/stats", JSON.stringify(c))
     }
 
     function l({
         stars: t,
         forks: e
     }) {
         t && (document.querySelector(".js-repo-stars").textContent = t), e && (document.querySelector(".js-repo-forks").textContent = e)
     }
 
-    function k() {
+    function w() {
         let t = sessionStorage.getItem("_sy/repo/stats");
         if (t) l(JSON.parse(t));
         else {
-            let e = r.getAttribute("data-user"),
-                s = r.getAttribute("data-repo"),
-                o = r.getAttribute("data-type");
-            o === "github" ? y(e, s) : o === "gitlab" && S(e, s)
+            let e = i.getAttribute("data-user"),
+                o = i.getAttribute("data-repo"),
+                s = i.getAttribute("data-type");
+            s === "github" ? b(e, o) : s === "gitlab" && v(e, o)
         }
     }
-    r && k();
+    i && w();
 })();
```

### Comparing `shibuya-2023.3.7/src/shibuya.egg-info/SOURCES.txt` & `shibuya-2023.6.7/src/shibuya.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 src/shibuya/theme/shibuya/page.html
 src/shibuya/theme/shibuya/search.html
 src/shibuya/theme/shibuya/searchbox.html
 src/shibuya/theme/shibuya/theme.conf
 src/shibuya/theme/shibuya/components/nav-links.html
 src/shibuya/theme/shibuya/components/nav-versions.html
 src/shibuya/theme/shibuya/components/navigation.html
+src/shibuya/theme/shibuya/components/page-searchbox.html
 src/shibuya/theme/shibuya/components/searchbox.html
-src/shibuya/theme/shibuya/components/searchbox2.html
 src/shibuya/theme/shibuya/components/site-foot.html
 src/shibuya/theme/shibuya/components/site-head.html
 src/shibuya/theme/shibuya/components/variables.html
 src/shibuya/theme/shibuya/partials/article-bottom.html
 src/shibuya/theme/shibuya/partials/banner.html
 src/shibuya/theme/shibuya/partials/extra-head.html
 src/shibuya/theme/shibuya/partials/footer.html
```

