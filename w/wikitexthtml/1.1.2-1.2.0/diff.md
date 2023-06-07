# Comparing `tmp/wikitexthtml-1.1.2.tar.gz` & `tmp/wikitexthtml-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wikitexthtml-1.1.2.tar", last modified: Thu Jul 14 06:13:19 2022, max compression
+gzip compressed data, was "wikitexthtml-1.2.0.tar", last modified: Wed Jun  7 09:49:21 2023, max compression
```

## Comparing `wikitexthtml-1.1.2.tar` & `wikitexthtml-1.2.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 06:13:19.899816 wikitexthtml-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (121)     7652 2022-07-14 06:13:11.000000 wikitexthtml-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-07-14 06:13:11.000000 wikitexthtml-1.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2912 2022-07-14 06:13:19.899816 wikitexthtml-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2039 2022-07-14 06:13:11.000000 wikitexthtml-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-07-14 06:13:19.000000 wikitexthtml-1.1.2/VERSION
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-14 06:13:19.899816 wikitexthtml-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      841 2022-07-14 06:13:11.000000 wikitexthtml-1.1.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     1618 2022-07-14 06:13:11.000000 wikitexthtml-1.1.2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 06:13:19.895815 wikitexthtml-1.1.2/wikitexthtml/
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-07-14 06:13:11.000000 wikitexthtml-1.1.2/wikitexthtml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-07-14 06:13:11.000000 wikitexthtml-1.1.2/wikitexthtml/enums.py
--rw-r--r--   0 runner    (1001) docker     (121)      241 2022-07-14 06:13:11.000000 wikitexthtml-1.1.2/wikitexthtml/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3821 2022-07-14 06:13:11.000000 wikitexthtml-1.1.2/wikitexthtml/page.py
--rw-r--r--   0 runner    (1001) docker     (121)     1521 2022-07-14 06:13:11.000000 wikitexthtml-1.1.2/wikitexthtml/prototype.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 06:13:19.895815 wikitexthtml-1.1.2/wikitexthtml/render/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 06:13:11.000000 wikitexthtml-1.1.2/wikitexthtml/render/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      371 2022-07-14 06:13:11.000000 wikitexthtml-1.1.2/wikitexthtml/render/bold_and_italic.py
--rw-r--r--   0 runner    (1001) docker     (121)      887 2022-07-14 06:13:11.000000 wikitexthtml-1.1.2/wikitexthtml/render/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1431 2022-07-14 06:13:11.000000 wikitexthtml-1.1.2/wikitexthtml/render/external_link.py
--rw-r--r--   0 runner    (1001) docker     (121)     2631 2022-07-14 06:13:11.000000 wikitexthtml-1.1.2/wikitexthtml/render/list_.py
--rw-r--r--   0 runner    (1001) docker     (121)     2156 2022-07-14 06:13:11.000000 wikitexthtml-1.1.2/wikitexthtml/render/parameter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1150 2022-07-14 06:13:11.000000 wikitexthtml-1.1.2/wikitexthtml/render/parser_function.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 06:13:19.895815 wikitexthtml-1.1.2/wikitexthtml/render/parser_functions/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 06:13:11.000000 wikitexthtml-1.1.2/wikitexthtml/render/parser_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-07-14 06:13:11.000000 wikitexthtml-1.1.2/wikitexthtml/render/parser_functions/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)      599 2022-07-14 06:13:11.000000 wikitexthtml-1.1.2/wikitexthtml/render/parser_functions/expr.py
--rw-r--r--   0 runner    (1001) docker     (121)     4688 2022-07-14 06:13:11.000000 wikitexthtml-1.1.2/wikitexthtml/render/parser_functions/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)      544 2022-07-14 06:13:11.000000 wikitexthtml-1.1.2/wikitexthtml/render/parser_functions/if_.py
--rw-r--r--   0 runner    (1001) docker     (121)      608 2022-07-14 06:13:11.000000 wikitexthtml-1.1.2/wikitexthtml/render/parser_functions/ifeq.py
--rw-r--r--   0 runner    (1001) docker     (121)      594 2022-07-14 06:13:11.000000 wikitexthtml-1.1.2/wikitexthtml/render/parser_functions/ifexist.py
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-07-14 06:13:11.000000 wikitexthtml-1.1.2/wikitexthtml/render/parser_functions/ifexpr.py
--rw-r--r--   0 runner    (1001) docker     (121)    22550 2022-07-14 06:13:11.000000 wikitexthtml-1.1.2/wikitexthtml/render/parser_functions/parsetab.py
--rw-r--r--   0 runner    (1001) docker     (121)     1240 2022-07-14 06:13:11.000000 wikitexthtml-1.1.2/wikitexthtml/render/parser_functions/string.py
--rw-r--r--   0 runner    (1001) docker     (121)     1675 2022-07-14 06:13:11.000000 wikitexthtml-1.1.2/wikitexthtml/render/parser_functions/switch.py
--rw-r--r--   0 runner    (1001) docker     (121)      610 2022-07-14 06:13:11.000000 wikitexthtml-1.1.2/wikitexthtml/render/parser_functions/url.py
--rw-r--r--   0 runner    (1001) docker     (121)     1060 2022-07-14 06:13:11.000000 wikitexthtml-1.1.2/wikitexthtml/render/parser_functions/variables.py
--rw-r--r--   0 runner    (1001) docker     (121)      379 2022-07-14 06:13:11.000000 wikitexthtml-1.1.2/wikitexthtml/render/postprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 06:13:19.895815 wikitexthtml-1.1.2/wikitexthtml/render/postprocesses/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 06:13:11.000000 wikitexthtml-1.1.2/wikitexthtml/render/postprocesses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2136 2022-07-14 06:13:11.000000 wikitexthtml-1.1.2/wikitexthtml/render/postprocesses/add_p_blocks.py
--rw-r--r--   0 runner    (1001) docker     (121)     2722 2022-07-14 06:13:11.000000 wikitexthtml-1.1.2/wikitexthtml/render/postprocesses/clean_html.py
--rw-r--r--   0 runner    (1001) docker     (121)      854 2022-07-14 06:13:11.000000 wikitexthtml-1.1.2/wikitexthtml/render/postprocesses/fix_dangling_lt.py
--rw-r--r--   0 runner    (1001) docker     (121)     1637 2022-07-14 06:13:11.000000 wikitexthtml-1.1.2/wikitexthtml/render/postprocesses/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     9061 2022-07-14 06:13:11.000000 wikitexthtml-1.1.2/wikitexthtml/render/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (121)     5699 2022-07-14 06:13:11.000000 wikitexthtml-1.1.2/wikitexthtml/render/section.py
--rw-r--r--   0 runner    (1001) docker     (121)     3898 2022-07-14 06:13:11.000000 wikitexthtml-1.1.2/wikitexthtml/render/table.py
--rw-r--r--   0 runner    (1001) docker     (121)      481 2022-07-14 06:13:11.000000 wikitexthtml-1.1.2/wikitexthtml/render/tag.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 06:13:19.895815 wikitexthtml-1.1.2/wikitexthtml/render/tags/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 06:13:11.000000 wikitexthtml-1.1.2/wikitexthtml/render/tags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2683 2022-07-14 06:13:11.000000 wikitexthtml-1.1.2/wikitexthtml/render/tags/gallery.py
--rw-r--r--   0 runner    (1001) docker     (121)     1943 2022-07-14 06:13:11.000000 wikitexthtml-1.1.2/wikitexthtml/render/template.py
--rw-r--r--   0 runner    (1001) docker     (121)     1456 2022-07-14 06:13:11.000000 wikitexthtml-1.1.2/wikitexthtml/render/wikilink.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 06:13:19.899816 wikitexthtml-1.1.2/wikitexthtml/render/wikilinks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 06:13:11.000000 wikitexthtml-1.1.2/wikitexthtml/render/wikilinks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8554 2022-07-14 06:13:11.000000 wikitexthtml-1.1.2/wikitexthtml/render/wikilinks/file.py
--rw-r--r--   0 runner    (1001) docker     (121)     1480 2022-07-14 06:13:11.000000 wikitexthtml-1.1.2/wikitexthtml/render/wikilinks/internal.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 06:13:19.895815 wikitexthtml-1.1.2/wikitexthtml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2912 2022-07-14 06:13:19.000000 wikitexthtml-1.1.2/wikitexthtml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1866 2022-07-14 06:13:19.000000 wikitexthtml-1.1.2/wikitexthtml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-14 06:13:19.000000 wikitexthtml-1.1.2/wikitexthtml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-07-14 06:13:19.000000 wikitexthtml-1.1.2/wikitexthtml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-07-14 06:13:19.000000 wikitexthtml-1.1.2/wikitexthtml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:49:21.757419 wikitexthtml-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-07 09:49:10.000000 wikitexthtml-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-07 09:49:10.000000 wikitexthtml-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-06-07 09:49:21.757419 wikitexthtml-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-07 09:49:10.000000 wikitexthtml-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-07 09:49:21.000000 wikitexthtml-1.2.0/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 09:49:21.757419 wikitexthtml-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-07 09:49:10.000000 wikitexthtml-1.2.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-07 09:49:10.000000 wikitexthtml-1.2.0/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:49:21.749420 wikitexthtml-1.2.0/wikitexthtml/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-07 09:49:10.000000 wikitexthtml-1.2.0/wikitexthtml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-07 09:49:10.000000 wikitexthtml-1.2.0/wikitexthtml/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-07 09:49:10.000000 wikitexthtml-1.2.0/wikitexthtml/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-06-07 09:49:10.000000 wikitexthtml-1.2.0/wikitexthtml/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-07 09:49:10.000000 wikitexthtml-1.2.0/wikitexthtml/prototype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:49:21.753419 wikitexthtml-1.2.0/wikitexthtml/render/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 09:49:10.000000 wikitexthtml-1.2.0/wikitexthtml/render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-07 09:49:10.000000 wikitexthtml-1.2.0/wikitexthtml/render/bold_and_italic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-07 09:49:10.000000 wikitexthtml-1.2.0/wikitexthtml/render/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-07 09:49:10.000000 wikitexthtml-1.2.0/wikitexthtml/render/external_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-07 09:49:10.000000 wikitexthtml-1.2.0/wikitexthtml/render/list_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-07 09:49:10.000000 wikitexthtml-1.2.0/wikitexthtml/render/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-07 09:49:10.000000 wikitexthtml-1.2.0/wikitexthtml/render/parser_function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:49:21.753419 wikitexthtml-1.2.0/wikitexthtml/render/parser_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 09:49:10.000000 wikitexthtml-1.2.0/wikitexthtml/render/parser_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-07 09:49:10.000000 wikitexthtml-1.2.0/wikitexthtml/render/parser_functions/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-07 09:49:10.000000 wikitexthtml-1.2.0/wikitexthtml/render/parser_functions/expr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4688 2023-06-07 09:49:10.000000 wikitexthtml-1.2.0/wikitexthtml/render/parser_functions/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-07 09:49:10.000000 wikitexthtml-1.2.0/wikitexthtml/render/parser_functions/if_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-07 09:49:10.000000 wikitexthtml-1.2.0/wikitexthtml/render/parser_functions/ifeq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-07 09:49:10.000000 wikitexthtml-1.2.0/wikitexthtml/render/parser_functions/ifexist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-07 09:49:10.000000 wikitexthtml-1.2.0/wikitexthtml/render/parser_functions/ifexpr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22550 2023-06-07 09:49:10.000000 wikitexthtml-1.2.0/wikitexthtml/render/parser_functions/parsetab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-07 09:49:10.000000 wikitexthtml-1.2.0/wikitexthtml/render/parser_functions/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-07 09:49:10.000000 wikitexthtml-1.2.0/wikitexthtml/render/parser_functions/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-07 09:49:10.000000 wikitexthtml-1.2.0/wikitexthtml/render/parser_functions/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-07 09:49:10.000000 wikitexthtml-1.2.0/wikitexthtml/render/parser_functions/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-07 09:49:10.000000 wikitexthtml-1.2.0/wikitexthtml/render/postprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:49:21.753419 wikitexthtml-1.2.0/wikitexthtml/render/postprocesses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 09:49:10.000000 wikitexthtml-1.2.0/wikitexthtml/render/postprocesses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-06-07 09:49:10.000000 wikitexthtml-1.2.0/wikitexthtml/render/postprocesses/add_p_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-06-07 09:49:10.000000 wikitexthtml-1.2.0/wikitexthtml/render/postprocesses/clean_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-07 09:49:10.000000 wikitexthtml-1.2.0/wikitexthtml/render/postprocesses/fix_dangling_lt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-06-07 09:49:10.000000 wikitexthtml-1.2.0/wikitexthtml/render/postprocesses/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-06-07 09:49:10.000000 wikitexthtml-1.2.0/wikitexthtml/render/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-06-07 09:49:10.000000 wikitexthtml-1.2.0/wikitexthtml/render/section.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-06-07 09:49:10.000000 wikitexthtml-1.2.0/wikitexthtml/render/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-07 09:49:10.000000 wikitexthtml-1.2.0/wikitexthtml/render/tag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:49:21.753419 wikitexthtml-1.2.0/wikitexthtml/render/tags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 09:49:10.000000 wikitexthtml-1.2.0/wikitexthtml/render/tags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-06-07 09:49:10.000000 wikitexthtml-1.2.0/wikitexthtml/render/tags/gallery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-07 09:49:10.000000 wikitexthtml-1.2.0/wikitexthtml/render/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-07 09:49:10.000000 wikitexthtml-1.2.0/wikitexthtml/render/wikilink.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:49:21.757419 wikitexthtml-1.2.0/wikitexthtml/render/wikilinks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 09:49:10.000000 wikitexthtml-1.2.0/wikitexthtml/render/wikilinks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8554 2023-06-07 09:49:10.000000 wikitexthtml-1.2.0/wikitexthtml/render/wikilinks/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-07 09:49:10.000000 wikitexthtml-1.2.0/wikitexthtml/render/wikilinks/internal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 09:49:21.753419 wikitexthtml-1.2.0/wikitexthtml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-06-07 09:49:21.000000 wikitexthtml-1.2.0/wikitexthtml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-07 09:49:21.000000 wikitexthtml-1.2.0/wikitexthtml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 09:49:21.000000 wikitexthtml-1.2.0/wikitexthtml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-07 09:49:21.000000 wikitexthtml-1.2.0/wikitexthtml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-07 09:49:21.000000 wikitexthtml-1.2.0/wikitexthtml.egg-info/top_level.txt
```

### Comparing `wikitexthtml-1.1.2/LICENSE` & `wikitexthtml-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wikitexthtml-1.1.2/PKG-INFO` & `wikitexthtml-1.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: wikitexthtml
-Version: 1.1.2
+Version: 1.2.0
 Summary: Convert wikitext to HTML
 Home-page: https://github.com/TrueBrain/wikitexthtml
 Author: Patric 'TrueBrain' Stout
 Author-email: truebrain@truebrain.nl
 License: UNKNOWN
 Description: # wikitexthtml
         
         [![GitHub License](https://img.shields.io/github/license/TrueBrain/wikitexthtml)](https://github.com/TrueBrain/wikitexthtml/blob/main/LICENSE)
         [![GitHub Tag](https://img.shields.io/github/v/tag/TrueBrain/wikitexthtml?include_prereleases&label=stable)](https://github.com/TrueBrain/wikitexthtml/releases)
         [![GitHub commits since latest release](https://img.shields.io/github/commits-since/TrueBrain/wikitexthtml/latest/main)](https://github.com/TrueBrain/wikitexthtml/commits/main)
         
-        [![GitHub Workflow Status (Testing)](https://img.shields.io/github/workflow/status/TrueBrain/wikitexthtml/Testing/main?label=main)](https://github.com/TrueBrain/wikitexthtml/actions?query=workflow%3ATesting)
-        [![GitHub Workflow Status (Release)](https://img.shields.io/github/workflow/status/TrueBrain/wikitexthtml/Release?label=release)](https://github.com/TrueBrain/wikitexthtml/actions?query=workflow%3A%22Release%22)
+        [![GitHub Workflow Status (Testing)](https://img.shields.io/github/actions/workflow/status/TrueBrain/wikitexthtml/testing.yml?branch=main&label=main)](https://github.com/TrueBrain/wikitexthtml/actions/workflows/testing.yml)
+        [![GitHub Workflow Status (Release)](https://img.shields.io/github/actions/workflow/status/TrueBrain/wikitexthtml/release.yml?label=release)](https://github.com/TrueBrain/wikitexthtml/actions/workflows/release.yml)
         
         wikitexthtml is a library that renders HTML from WikiText.
         
         ## Dependencies
         
         - Python3.8 or higher.
         - `python-slugify` (via `setup.py`), for slugs in anchors
```

### Comparing `wikitexthtml-1.1.2/README.md` & `wikitexthtml-1.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # wikitexthtml
 
 [![GitHub License](https://img.shields.io/github/license/TrueBrain/wikitexthtml)](https://github.com/TrueBrain/wikitexthtml/blob/main/LICENSE)
 [![GitHub Tag](https://img.shields.io/github/v/tag/TrueBrain/wikitexthtml?include_prereleases&label=stable)](https://github.com/TrueBrain/wikitexthtml/releases)
 [![GitHub commits since latest release](https://img.shields.io/github/commits-since/TrueBrain/wikitexthtml/latest/main)](https://github.com/TrueBrain/wikitexthtml/commits/main)
 
-[![GitHub Workflow Status (Testing)](https://img.shields.io/github/workflow/status/TrueBrain/wikitexthtml/Testing/main?label=main)](https://github.com/TrueBrain/wikitexthtml/actions?query=workflow%3ATesting)
-[![GitHub Workflow Status (Release)](https://img.shields.io/github/workflow/status/TrueBrain/wikitexthtml/Release?label=release)](https://github.com/TrueBrain/wikitexthtml/actions?query=workflow%3A%22Release%22)
+[![GitHub Workflow Status (Testing)](https://img.shields.io/github/actions/workflow/status/TrueBrain/wikitexthtml/testing.yml?branch=main&label=main)](https://github.com/TrueBrain/wikitexthtml/actions/workflows/testing.yml)
+[![GitHub Workflow Status (Release)](https://img.shields.io/github/actions/workflow/status/TrueBrain/wikitexthtml/release.yml?label=release)](https://github.com/TrueBrain/wikitexthtml/actions/workflows/release.yml)
 
 wikitexthtml is a library that renders HTML from WikiText.
 
 ## Dependencies
 
 - Python3.8 or higher.
 - `python-slugify` (via `setup.py`), for slugs in anchors
```

### Comparing `wikitexthtml-1.1.2/setup.py` & `wikitexthtml-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `wikitexthtml-1.1.2/version.py` & `wikitexthtml-1.2.0/version.py`

 * *Files identical despite different names*

### Comparing `wikitexthtml-1.1.2/wikitexthtml/page.py` & `wikitexthtml-1.2.0/wikitexthtml/page.py`

 * *Files identical despite different names*

### Comparing `wikitexthtml-1.1.2/wikitexthtml/prototype.py` & `wikitexthtml-1.2.0/wikitexthtml/prototype.py`

 * *Files identical despite different names*

### Comparing `wikitexthtml-1.1.2/wikitexthtml/render/config.py` & `wikitexthtml-1.2.0/wikitexthtml/render/config.py`

 * *Files identical despite different names*

### Comparing `wikitexthtml-1.1.2/wikitexthtml/render/external_link.py` & `wikitexthtml-1.2.0/wikitexthtml/render/external_link.py`

 * *Files identical despite different names*

### Comparing `wikitexthtml-1.1.2/wikitexthtml/render/list_.py` & `wikitexthtml-1.2.0/wikitexthtml/render/list_.py`

 * *Files identical despite different names*

### Comparing `wikitexthtml-1.1.2/wikitexthtml/render/parameter.py` & `wikitexthtml-1.2.0/wikitexthtml/render/parameter.py`

 * *Files identical despite different names*

### Comparing `wikitexthtml-1.1.2/wikitexthtml/render/parser_function.py` & `wikitexthtml-1.2.0/wikitexthtml/render/parser_function.py`

 * *Files identical despite different names*

### Comparing `wikitexthtml-1.1.2/wikitexthtml/render/parser_functions/expr.py` & `wikitexthtml-1.2.0/wikitexthtml/render/parser_functions/expr.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import wikitextparser
 
-from .exceptions import (
-    EvaluationError,
-    ParserFunctionWrongArgumentCount,
-)
+from .exceptions import EvaluationError
 from .helpers import (
     evaluate,
     get_argument,
 )
 from ...prototype import WikiTextHtml
 
 
 def expr(instance: WikiTextHtml, parser_function: wikitextparser.ParserFunction):
     if len(parser_function.arguments) < 1:
-        raise ParserFunctionWrongArgumentCount
+        instance.add_error(
+            f'Parser function "{parser_function.name}" expects at least argument, '
+            f"but {len(parser_function.arguments)} given."
+        )
+        return
 
     expr = get_argument(parser_function, 0)
 
     try:
         result = evaluate(expr, as_str=True)
     except EvaluationError as e:
         result = f"Expression error: {e.args[0]}"
```

### Comparing `wikitexthtml-1.1.2/wikitexthtml/render/parser_functions/helpers.py` & `wikitexthtml-1.2.0/wikitexthtml/render/parser_functions/helpers.py`

 * *Files identical despite different names*

### Comparing `wikitexthtml-1.1.2/wikitexthtml/render/parser_functions/if_.py` & `wikitexthtml-1.2.0/wikitexthtml/render/parser_functions/url.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,23 @@
+import html
+import urllib
 import wikitextparser
 
-from .exceptions import ParserFunctionWrongArgumentCount
 from .helpers import get_argument
 from ...prototype import WikiTextHtml
 
 
-def if_(instance: WikiTextHtml, parser_function: wikitextparser.ParserFunction):
-    if len(parser_function.arguments) < 1:
-        raise ParserFunctionWrongArgumentCount
-
-    condition = get_argument(parser_function, 0)
-
-    if condition.strip():
-        parser_function.string = get_argument(parser_function, 1)
-    else:
-        parser_function.string = get_argument(parser_function, 2)
+def encode(instance: WikiTextHtml, parser_function: wikitextparser.ParserFunction):
+    if len(parser_function.arguments) != 1:
+        instance.add_error(
+            f'Parser function "{parser_function.name}" expects 1 argument, '
+            f"but {len(parser_function.arguments)} given."
+        )
+        return
+
+    url = get_argument(parser_function, 0).strip()
+
+    # All variables should already be HTML escaped, so unescape first,
+    # as otherwise we are double encoding them.
+    url = urllib.parse.quote(html.unescape(url))
+
+    parser_function.string = url
```

### Comparing `wikitexthtml-1.1.2/wikitexthtml/render/parser_functions/ifeq.py` & `wikitexthtml-1.2.0/wikitexthtml/render/parser_functions/ifeq.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import wikitextparser
 
-from .exceptions import ParserFunctionWrongArgumentCount
 from .helpers import get_argument
 from ...prototype import WikiTextHtml
 
 
 def ifeq(
     instance: WikiTextHtml,
     parser_function: wikitextparser.ParserFunction,
 ):
     if len(parser_function.arguments) < 2:
-        raise ParserFunctionWrongArgumentCount
+        instance.add_error(
+            f'Parser function "{parser_function.name}" expects at least 2 arguments, '
+            f"but {len(parser_function.arguments)} given."
+        )
+        return
 
     left = get_argument(parser_function, 0)
     right = get_argument(parser_function, 1)
 
     if left.strip() == right.strip():
         parser_function.string = get_argument(parser_function, 2)
     else:
```

### Comparing `wikitexthtml-1.1.2/wikitexthtml/render/parser_functions/ifexist.py` & `wikitexthtml-1.2.0/wikitexthtml/render/parser_functions/if_.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import wikitextparser
 
-from .exceptions import ParserFunctionWrongArgumentCount
 from .helpers import get_argument
 from ...prototype import WikiTextHtml
 
 
-def ifexist(instance: WikiTextHtml, parser_function: wikitextparser.ParserFunction):
+def if_(instance: WikiTextHtml, parser_function: wikitextparser.ParserFunction):
     if len(parser_function.arguments) < 1:
-        raise ParserFunctionWrongArgumentCount
+        instance.add_error(
+            f'Parser function "{parser_function.name}" expects at least 1 argument, '
+            f"but {len(parser_function.arguments)} given."
+        )
+        return
 
-    page_title = get_argument(parser_function, 0)
-    page_exists = instance.page_exists(page_title)
+    condition = get_argument(parser_function, 0)
 
-    if page_exists:
+    if condition.strip():
         parser_function.string = get_argument(parser_function, 1)
     else:
         parser_function.string = get_argument(parser_function, 2)
```

### Comparing `wikitexthtml-1.1.2/wikitexthtml/render/parser_functions/ifexpr.py` & `wikitexthtml-1.2.0/wikitexthtml/render/parser_functions/ifexpr.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import wikitextparser
 
-from .exceptions import (
-    EvaluationError,
-    ParserFunctionWrongArgumentCount,
-)
+from .exceptions import EvaluationError
 from .helpers import (
     evaluate,
     get_argument,
 )
 from ...prototype import WikiTextHtml
 
 
 def ifexpr(instance: WikiTextHtml, parser_function: wikitextparser.ParserFunction):
     if len(parser_function.arguments) < 1:
-        raise ParserFunctionWrongArgumentCount
+        instance.add_error(
+            f'Parser function "{parser_function.name}" expects at least 1 argument, '
+            f"but {len(parser_function.arguments)} given."
+        )
+        return
 
     expr = get_argument(parser_function, 0)
 
     try:
         result = evaluate(expr)
     except EvaluationError as e:
         parser_function.string = f"Expression error: {e.args[0]}"
```

### Comparing `wikitexthtml-1.1.2/wikitexthtml/render/parser_functions/parsetab.py` & `wikitexthtml-1.2.0/wikitexthtml/render/parser_functions/parsetab.py`

 * *Files identical despite different names*

### Comparing `wikitexthtml-1.1.2/wikitexthtml/render/parser_functions/string.py` & `wikitexthtml-1.2.0/wikitexthtml/render/parser_functions/variables.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,30 @@
+import datetime
+import html
 import wikitextparser
 
-from .exceptions import ParserFunctionWrongArgumentCount
-from .helpers import get_argument
+from ...exceptions import InvalidWikiLink
 from ...prototype import WikiTextHtml
 
 
-def lc(instance: WikiTextHtml, parser_function: wikitextparser.ParserFunction):
-    if len(parser_function.arguments) != 1:
-        raise ParserFunctionWrongArgumentCount
-
-    value = get_argument(parser_function, 0).lower()
-    parser_function.string = value
-
-
-def uc(instance: WikiTextHtml, parser_function: wikitextparser.ParserFunction):
-    if len(parser_function.arguments) != 1:
-        raise ParserFunctionWrongArgumentCount
-
-    value = get_argument(parser_function, 0).upper()
-    parser_function.string = value
-
-
-def lcfirst(instance: WikiTextHtml, parser_function: wikitextparser.ParserFunction):
-    if len(parser_function.arguments) != 1:
-        raise ParserFunctionWrongArgumentCount
-
-    value = get_argument(parser_function, 0)
-    parser_function.string = value[0].lower() + value[1:]
-
-
-def ucfirst(instance: WikiTextHtml, parser_function: wikitextparser.ParserFunction):
-    if len(parser_function.arguments) != 1:
-        raise ParserFunctionWrongArgumentCount
-
-    value = get_argument(parser_function, 0)
-    parser_function.string = value[0].upper() + value[1:]
+def variable(instance: WikiTextHtml, parser_function: wikitextparser.ParserFunction):
+    if len(parser_function.arguments) != 0:
+        instance.add_error(
+            f'Parser function "{parser_function.name}" expects no arguments, '
+            f"but {len(parser_function.arguments)} given."
+        )
+        return
+
+    name = parser_function.name.lower()
+    if name == "currentyear":
+        parser_function.string = str(datetime.datetime.now().year)
+    elif name in ("pagename", "fullpagename", "basepagename"):
+        parser_function.string = html.escape(instance.page)
+    elif name == "subpagename":
+        try:
+            parser_function.string = html.escape(instance.clean_title(instance.page))
+        except InvalidWikiLink as e:
+            # Errors always end with a dot, hence the [:-1].
+            instance.add_error(f'{e.args[0][:-1]} (parserfunction "{parser_function.string}").')
+            parser_function.string = ""
+    elif name == "namespace":
+        parser_function.string = ""
```

### Comparing `wikitexthtml-1.1.2/wikitexthtml/render/parser_functions/switch.py` & `wikitexthtml-1.2.0/wikitexthtml/render/parser_functions/switch.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import wikitextparser
 
-from .exceptions import ParserFunctionWrongArgumentCount
 from .helpers import get_argument
 from ...prototype import WikiTextHtml
 
 
 def switch(instance: WikiTextHtml, parser_function: wikitextparser.ParserFunction):
     if len(parser_function.arguments) < 1:
-        raise ParserFunctionWrongArgumentCount
+        instance.add_error(
+            f'Parser function "{parser_function.name}" expects at least 1 argument, '
+            f"but {len(parser_function.arguments)} given."
+        )
+        return
 
     branch = get_argument(parser_function, 0).strip()
 
     explicit_default = None
     positional_default = None
     fallthrough = False
```

### Comparing `wikitexthtml-1.1.2/wikitexthtml/render/postprocesses/add_p_blocks.py` & `wikitexthtml-1.2.0/wikitexthtml/render/postprocesses/add_p_blocks.py`

 * *Files identical despite different names*

### Comparing `wikitexthtml-1.1.2/wikitexthtml/render/postprocesses/clean_html.py` & `wikitexthtml-1.2.0/wikitexthtml/render/postprocesses/clean_html.py`

 * *Files identical despite different names*

### Comparing `wikitexthtml-1.1.2/wikitexthtml/render/postprocesses/fix_dangling_lt.py` & `wikitexthtml-1.2.0/wikitexthtml/render/postprocesses/fix_dangling_lt.py`

 * *Files identical despite different names*

### Comparing `wikitexthtml-1.1.2/wikitexthtml/render/postprocesses/helper.py` & `wikitexthtml-1.2.0/wikitexthtml/render/postprocesses/helper.py`

 * *Files identical despite different names*

### Comparing `wikitexthtml-1.1.2/wikitexthtml/render/preprocess.py` & `wikitexthtml-1.2.0/wikitexthtml/render/preprocess.py`

 * *Files identical despite different names*

### Comparing `wikitexthtml-1.1.2/wikitexthtml/render/section.py` & `wikitexthtml-1.2.0/wikitexthtml/render/section.py`

 * *Files identical despite different names*

### Comparing `wikitexthtml-1.1.2/wikitexthtml/render/table.py` & `wikitexthtml-1.2.0/wikitexthtml/render/table.py`

 * *Files identical despite different names*

### Comparing `wikitexthtml-1.1.2/wikitexthtml/render/tags/gallery.py` & `wikitexthtml-1.2.0/wikitexthtml/render/tags/gallery.py`

 * *Files identical despite different names*

### Comparing `wikitexthtml-1.1.2/wikitexthtml/render/template.py` & `wikitexthtml-1.2.0/wikitexthtml/render/template.py`

 * *Files identical despite different names*

### Comparing `wikitexthtml-1.1.2/wikitexthtml/render/wikilink.py` & `wikitexthtml-1.2.0/wikitexthtml/render/wikilink.py`

 * *Files identical despite different names*

### Comparing `wikitexthtml-1.1.2/wikitexthtml/render/wikilinks/file.py` & `wikitexthtml-1.2.0/wikitexthtml/render/wikilinks/file.py`

 * *Files identical despite different names*

### Comparing `wikitexthtml-1.1.2/wikitexthtml/render/wikilinks/internal.py` & `wikitexthtml-1.2.0/wikitexthtml/render/wikilinks/internal.py`

 * *Files identical despite different names*

### Comparing `wikitexthtml-1.1.2/wikitexthtml.egg-info/PKG-INFO` & `wikitexthtml-1.2.0/wikitexthtml.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: wikitexthtml
-Version: 1.1.2
+Version: 1.2.0
 Summary: Convert wikitext to HTML
 Home-page: https://github.com/TrueBrain/wikitexthtml
 Author: Patric 'TrueBrain' Stout
 Author-email: truebrain@truebrain.nl
 License: UNKNOWN
 Description: # wikitexthtml
         
         [![GitHub License](https://img.shields.io/github/license/TrueBrain/wikitexthtml)](https://github.com/TrueBrain/wikitexthtml/blob/main/LICENSE)
         [![GitHub Tag](https://img.shields.io/github/v/tag/TrueBrain/wikitexthtml?include_prereleases&label=stable)](https://github.com/TrueBrain/wikitexthtml/releases)
         [![GitHub commits since latest release](https://img.shields.io/github/commits-since/TrueBrain/wikitexthtml/latest/main)](https://github.com/TrueBrain/wikitexthtml/commits/main)
         
-        [![GitHub Workflow Status (Testing)](https://img.shields.io/github/workflow/status/TrueBrain/wikitexthtml/Testing/main?label=main)](https://github.com/TrueBrain/wikitexthtml/actions?query=workflow%3ATesting)
-        [![GitHub Workflow Status (Release)](https://img.shields.io/github/workflow/status/TrueBrain/wikitexthtml/Release?label=release)](https://github.com/TrueBrain/wikitexthtml/actions?query=workflow%3A%22Release%22)
+        [![GitHub Workflow Status (Testing)](https://img.shields.io/github/actions/workflow/status/TrueBrain/wikitexthtml/testing.yml?branch=main&label=main)](https://github.com/TrueBrain/wikitexthtml/actions/workflows/testing.yml)
+        [![GitHub Workflow Status (Release)](https://img.shields.io/github/actions/workflow/status/TrueBrain/wikitexthtml/release.yml?label=release)](https://github.com/TrueBrain/wikitexthtml/actions/workflows/release.yml)
         
         wikitexthtml is a library that renders HTML from WikiText.
         
         ## Dependencies
         
         - Python3.8 or higher.
         - `python-slugify` (via `setup.py`), for slugs in anchors
```

### Comparing `wikitexthtml-1.1.2/wikitexthtml.egg-info/SOURCES.txt` & `wikitexthtml-1.2.0/wikitexthtml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

