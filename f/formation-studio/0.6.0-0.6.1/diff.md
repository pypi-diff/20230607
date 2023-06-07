# Comparing `tmp/formation-studio-0.6.0.tar.gz` & `tmp/formation-studio-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formation-studio-0.6.0.tar", last modified: Sat Jun  3 20:00:53 2023, max compression
+gzip compressed data, was "formation-studio-0.6.1.tar", last modified: Wed Jun  7 11:04:15 2023, max compression
```

## Comparing `formation-studio-0.6.0.tar` & `formation-studio-0.6.1.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:00:53.417703 formation-studio-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-03 20:00:31.000000 formation-studio-0.6.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-03 20:00:31.000000 formation-studio-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8796 2023-06-03 20:00:53.417703 formation-studio-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7534 2023-06-03 20:00:31.000000 formation-studio-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:00:53.397703 formation-studio-0.6.0/formation/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-03 20:00:31.000000 formation-studio-0.6.0/formation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:00:53.397703 formation-studio-0.6.0/formation/formats/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-03 20:00:31.000000 formation-studio-0.6.0/formation/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-06-03 20:00:31.000000 formation-studio-0.6.0/formation/formats/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-03 20:00:31.000000 formation-studio-0.6.0/formation/formats/_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-03 20:00:31.000000 formation-studio-0.6.0/formation/formats/_xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:00:53.397703 formation-studio-0.6.0/formation/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-03 20:00:31.000000 formation-studio-0.6.0/formation/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-03 20:00:31.000000 formation-studio-0.6.0/formation/handlers/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-03 20:00:31.000000 formation-studio-0.6.0/formation/handlers/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-06-03 20:00:31.000000 formation-studio-0.6.0/formation/handlers/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-03 20:00:31.000000 formation-studio-0.6.0/formation/handlers/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    18018 2023-06-03 20:00:31.000000 formation-studio-0.6.0/formation/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-03 20:00:31.000000 formation-studio-0.6.0/formation/meth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-03 20:00:31.000000 formation-studio-0.6.0/formation/preprocessors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-06-03 20:00:31.000000 formation-studio-0.6.0/formation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:00:53.397703 formation-studio-0.6.0/formation_studio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8796 2023-06-03 20:00:53.000000 formation-studio-0.6.0/formation_studio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-06-03 20:00:53.000000 formation-studio-0.6.0/formation_studio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 20:00:53.000000 formation-studio-0.6.0/formation_studio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-03 20:00:53.000000 formation-studio-0.6.0/formation_studio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-03 20:00:53.000000 formation-studio-0.6.0/formation_studio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-03 20:00:53.000000 formation-studio-0.6.0/formation_studio.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:00:53.397703 formation-studio-0.6.0/hoverset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 20:00:31.000000 formation-studio-0.6.0/hoverset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:00:53.405703 formation-studio-0.6.0/hoverset/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 20:00:31.000000 formation-studio-0.6.0/hoverset/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-06-03 20:00:31.000000 formation-studio-0.6.0/hoverset/data/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-06-03 20:00:31.000000 formation-studio-0.6.0/hoverset/data/image.bak
--rw-r--r--   0 runner    (1001) docker     (123)  6268365 2023-06-03 20:00:31.000000 formation-studio-0.6.0/hoverset/data/image.dat
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-06-03 20:00:31.000000 formation-studio-0.6.0/hoverset/data/image.dir
--rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-06-03 20:00:31.000000 formation-studio-0.6.0/hoverset/data/images.py
--rw-r--r--   0 runner    (1001) docker     (123)    16776 2023-06-03 20:00:31.000000 formation-studio-0.6.0/hoverset/data/keymap.py
--rw-r--r--   0 runner    (1001) docker     (123)    22989 2023-06-03 20:00:31.000000 formation-studio-0.6.0/hoverset/data/preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-03 20:00:31.000000 formation-studio-0.6.0/hoverset/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:00:53.405703 formation-studio-0.6.0/hoverset/platform/
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-03 20:00:31.000000 formation-studio-0.6.0/hoverset/platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-03 20:00:31.000000 formation-studio-0.6.0/hoverset/platform/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:00:53.409703 formation-studio-0.6.0/hoverset/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 20:00:31.000000 formation-studio-0.6.0/hoverset/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-06-03 20:00:31.000000 formation-studio-0.6.0/hoverset/ui/animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-06-03 20:00:31.000000 formation-studio-0.6.0/hoverset/ui/color.tcl
--rw-r--r--   0 runner    (1001) docker     (123)    18314 2023-06-03 20:00:31.000000 formation-studio-0.6.0/hoverset/ui/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-03 20:00:31.000000 formation-studio-0.6.0/hoverset/ui/icons.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-03 20:00:31.000000 formation-studio-0.6.0/hoverset/ui/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     9587 2023-06-03 20:00:31.000000 formation-studio-0.6.0/hoverset/ui/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)    21046 2023-06-03 20:00:31.000000 formation-studio-0.6.0/hoverset/ui/panels.py
--rw-r--r--   0 runner    (1001) docker     (123)    11644 2023-06-03 20:00:31.000000 formation-studio-0.6.0/hoverset/ui/pickers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-06-03 20:00:31.000000 formation-studio-0.6.0/hoverset/ui/styles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:00:53.409703 formation-studio-0.6.0/hoverset/ui/themes/
--rw-r--r--   0 runner    (1001) docker     (123)     5167 2023-06-03 20:00:31.000000 formation-studio-0.6.0/hoverset/ui/themes/default.css
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-06-03 20:00:31.000000 formation-studio-0.6.0/hoverset/ui/themes/light.css
--rw-r--r--   0 runner    (1001) docker     (123)   117202 2023-06-03 20:00:31.000000 formation-studio-0.6.0/hoverset/ui/widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-03 20:00:31.000000 formation-studio-0.6.0/hoverset/ui/windows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:00:53.409703 formation-studio-0.6.0/hoverset/util/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-03 20:00:31.000000 formation-studio-0.6.0/hoverset/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10307 2023-06-03 20:00:31.000000 formation-studio-0.6.0/hoverset/util/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     7436 2023-06-03 20:00:31.000000 formation-studio-0.6.0/hoverset/util/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-06-03 20:00:31.000000 formation-studio-0.6.0/hoverset/util/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-03 20:00:31.000000 formation-studio-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-03 20:00:31.000000 formation-studio-0.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 20:00:53.417703 formation-studio-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:00:53.409703 formation-studio-0.6.0/studio/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:00:53.409703 formation-studio-0.6.0/studio/debugtools/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/debugtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/debugtools/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/debugtools/debugger.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/debugtools/defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7965 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/debugtools/element_pane.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/debugtools/layouts.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/debugtools/preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/debugtools/style_pane.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:00:53.413703 formation-studio-0.6.0/studio/feature/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/feature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13215 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/feature/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/feature/component_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    18112 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/feature/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    35484 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/feature/design.py
--rw-r--r--   0 runner    (1001) docker     (123)     8748 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/feature/eventspane.py
--rw-r--r--   0 runner    (1001) docker     (123)    24252 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/feature/stylepane.py
--rw-r--r--   0 runner    (1001) docker     (123)     9008 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/feature/variablepane.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:00:53.413703 formation-studio-0.6.0/studio/lib/
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14083 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/lib/canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/lib/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    35873 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/lib/layouts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/lib/legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/lib/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/lib/native.py
--rw-r--r--   0 runner    (1001) docker     (123)    16822 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/lib/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    17395 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/lib/pseudo.py
--rw-r--r--   0 runner    (1001) docker     (123)    14563 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/lib/toplevel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/lib/variables.py
--rw-r--r--   0 runner    (1001) docker     (123)    38284 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:00:53.413703 formation-studio-0.6.0/studio/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16038 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/parsers/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    11616 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/resource_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:00:53.393703 formation-studio-0.6.0/studio/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:00:53.413703 formation-studio-0.6.0/studio/resources/images/
--rw-r--r--   0 runner    (1001) docker     (123)   225382 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/resources/images/formation.ico
--rw-r--r--   0 runner    (1001) docker     (123)    12275 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/resources/images/formation.png
--rw-r--r--   0 runner    (1001) docker     (123)   218818 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/resources/images/formation_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/resources/images/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:00:53.417703 formation-studio-0.6.0/studio/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/tools/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    45136 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/tools/canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)    17111 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/tools/menus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 20:00:53.417703 formation-studio-0.6.0/studio/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/ui/about.py
--rw-r--r--   0 runner    (1001) docker     (123)    28888 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/ui/editors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/ui/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    16601 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/ui/highlight.py
--rw-r--r--   0 runner    (1001) docker     (123)    16315 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/ui/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    12956 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/ui/widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-06-03 20:00:31.000000 formation-studio-0.6.0/studio/updates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:04:15.677651 formation-studio-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-07 11:03:54.000000 formation-studio-0.6.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-07 11:03:54.000000 formation-studio-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8796 2023-06-07 11:04:15.677651 formation-studio-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7534 2023-06-07 11:03:54.000000 formation-studio-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:04:15.645650 formation-studio-0.6.1/formation/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-07 11:03:54.000000 formation-studio-0.6.1/formation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:04:15.645650 formation-studio-0.6.1/formation/formats/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-07 11:03:54.000000 formation-studio-0.6.1/formation/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-06-07 11:03:54.000000 formation-studio-0.6.1/formation/formats/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-07 11:03:54.000000 formation-studio-0.6.1/formation/formats/_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-06-07 11:03:54.000000 formation-studio-0.6.1/formation/formats/_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:04:15.645650 formation-studio-0.6.1/formation/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-07 11:03:54.000000 formation-studio-0.6.1/formation/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-07 11:03:54.000000 formation-studio-0.6.1/formation/handlers/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-07 11:03:54.000000 formation-studio-0.6.1/formation/handlers/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-06-07 11:03:54.000000 formation-studio-0.6.1/formation/handlers/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-07 11:03:54.000000 formation-studio-0.6.1/formation/handlers/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18018 2023-06-07 11:03:54.000000 formation-studio-0.6.1/formation/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-07 11:03:54.000000 formation-studio-0.6.1/formation/meth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-07 11:03:54.000000 formation-studio-0.6.1/formation/preprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-06-07 11:03:54.000000 formation-studio-0.6.1/formation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:04:15.649651 formation-studio-0.6.1/formation_studio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8796 2023-06-07 11:04:15.000000 formation-studio-0.6.1/formation_studio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-06-07 11:04:15.000000 formation-studio-0.6.1/formation_studio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 11:04:15.000000 formation-studio-0.6.1/formation_studio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-07 11:04:15.000000 formation-studio-0.6.1/formation_studio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-07 11:04:15.000000 formation-studio-0.6.1/formation_studio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-07 11:04:15.000000 formation-studio-0.6.1/formation_studio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:04:15.649651 formation-studio-0.6.1/hoverset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:04:15.657651 formation-studio-0.6.1/hoverset/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/data/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/data/image.bak
+-rw-r--r--   0 runner    (1001) docker     (123)  6268365 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/data/image.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/data/image.dir
+-rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/data/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16776 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/data/keymap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22989 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/data/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:04:15.657651 formation-studio-0.6.1/hoverset/platform/
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/platform/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:04:15.661651 formation-studio-0.6.1/hoverset/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/ui/animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/ui/color.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)    18314 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/ui/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/ui/icons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/ui/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9587 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/ui/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21046 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/ui/panels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11644 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/ui/pickers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/ui/styles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:04:15.661651 formation-studio-0.6.1/hoverset/ui/themes/
+-rw-r--r--   0 runner    (1001) docker     (123)     5167 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/ui/themes/default.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/ui/themes/light.css
+-rw-r--r--   0 runner    (1001) docker     (123)   117202 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/ui/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/ui/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:04:15.661651 formation-studio-0.6.1/hoverset/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10307 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/util/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7436 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/util/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4770 2023-06-07 11:03:54.000000 formation-studio-0.6.1/hoverset/util/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-07 11:03:54.000000 formation-studio-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-07 11:03:54.000000 formation-studio-0.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 11:04:15.677651 formation-studio-0.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:04:15.665651 formation-studio-0.6.1/studio/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:04:15.665651 formation-studio-0.6.1/studio/debugtools/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/debugtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/debugtools/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/debugtools/debugger.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/debugtools/defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7965 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/debugtools/element_pane.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/debugtools/layouts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/debugtools/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/debugtools/style_pane.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:04:15.669651 formation-studio-0.6.1/studio/feature/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/feature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13215 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/feature/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/feature/component_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18112 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/feature/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35484 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/feature/design.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8748 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/feature/eventspane.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24252 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/feature/stylepane.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9008 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/feature/variablepane.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:04:15.673651 formation-studio-0.6.1/studio/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14083 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/lib/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/lib/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35873 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/lib/layouts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/lib/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/lib/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/lib/native.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16822 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/lib/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17395 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/lib/pseudo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14563 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/lib/toplevel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/lib/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38284 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:04:15.673651 formation-studio-0.6.1/studio/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16056 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/parsers/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11719 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/resource_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:04:15.641651 formation-studio-0.6.1/studio/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:04:15.673651 formation-studio-0.6.1/studio/resources/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   225382 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/resources/images/formation.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    12275 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/resources/images/formation.png
+-rw-r--r--   0 runner    (1001) docker     (123)   218818 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/resources/images/formation_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/resources/images/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:04:15.673651 formation-studio-0.6.1/studio/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/tools/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45136 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/tools/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17111 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/tools/menus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 11:04:15.677651 formation-studio-0.6.1/studio/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/ui/about.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28888 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/ui/editors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7830 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/ui/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16601 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/ui/highlight.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16315 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/ui/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12956 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/ui/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-06-07 11:03:54.000000 formation-studio-0.6.1/studio/updates.py
```

### Comparing `formation-studio-0.6.0/LICENSE.txt` & `formation-studio-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/PKG-INFO` & `formation-studio-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formation-studio
-Version: 0.6.0
+Version: 0.6.1
 Summary: Simplify GUI development in python
 Author-email: Emmanuel Obara <emmanuelobarany@gmail.com>
 License: MIT
 Project-URL: Documentation, https://formation-studio.readthedocs.io/en/latest/
 Project-URL: Issues, https://github.com/ObaraEmmanuel/Formation/issues
 Project-URL: Source, https://github.com/ObaraEmmanuel/Formation
 Keywords: formation,gui,graphical-user-interface,drag drop,tkinter,hoverset,python
```

### Comparing `formation-studio-0.6.0/README.md` & `formation-studio-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/formation/formats/__init__.py` & `formation-studio-0.6.1/formation/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/formation/formats/_base.py` & `formation-studio-0.6.1/formation/formats/_base.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/formation/formats/_json.py` & `formation-studio-0.6.1/formation/formats/_json.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/formation/formats/_xml.py` & `formation-studio-0.6.1/formation/formats/_xml.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 
 import re
 from collections import defaultdict
 
 try:
     from lxml import etree
     element_class = etree._Element
+    _using_lxml = True
 except ModuleNotFoundError:
     # use default xml library; features may be limited
     import xml.etree.ElementTree as etree
     element_class = etree.Element
+    _using_lxml = False
 
 from formation.formats._base import BaseFormat, Node
 
 namespaces = {
     "layout": "http://www.hoversetformationstudio.com/layouts/",
     "attr": "http://www.hoversetformationstudio.com/styles/",
     "menu": "http://www.hoversetformationstudio.com/menu",
@@ -83,17 +85,22 @@
         else:
             x_node = etree.fromstring(self.data)
         self.root = self._load_node(None, x_node)
         return self.root
 
     def generate(self, **kw):
         x_node = self._generate_node(None, self.root)
-        etree.cleanup_namespaces(x_node, top_nsmap=namespaces)
+        if _using_lxml:
+            etree.cleanup_namespaces(x_node, top_nsmap=namespaces)
+            return etree.tostring(
+                x_node, pretty_print=kw.get("pretty_print", True),
+                encoding="utf-8", xml_declaration=kw.get("xml_declaration", True)
+            ).decode('utf-8')
+
         return etree.tostring(
-            x_node, pretty_print=kw.get("pretty_print", True),
-            encoding="utf-8", xml_declaration=kw.get("xml_declaration", True)
-        ).decode('utf-8')
+            x_node, encoding="utf-8", xml_declaration=kw.get("xml_declaration", True)
+        ).decode("utf-8")
 
 
 if __name__ == "__main__":
     x = XMLFormat(path="formation/tests/samples/all_legacy.xml")
     x.load()
```

### Comparing `formation-studio-0.6.0/formation/handlers/__init__.py` & `formation-studio-0.6.1/formation/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/formation/handlers/command.py` & `formation-studio-0.6.1/formation/handlers/command.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/formation/handlers/image.py` & `formation-studio-0.6.1/formation/handlers/image.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/formation/handlers/layout.py` & `formation-studio-0.6.1/formation/handlers/layout.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/formation/handlers/misc.py` & `formation-studio-0.6.1/formation/handlers/misc.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/formation/loader.py` & `formation-studio-0.6.1/formation/loader.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/formation/meth.py` & `formation-studio-0.6.1/formation/meth.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/formation/preprocessors.py` & `formation-studio-0.6.1/formation/preprocessors.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/formation/utils.py` & `formation-studio-0.6.1/formation/utils.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/formation_studio.egg-info/PKG-INFO` & `formation-studio-0.6.1/formation_studio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formation-studio
-Version: 0.6.0
+Version: 0.6.1
 Summary: Simplify GUI development in python
 Author-email: Emmanuel Obara <emmanuelobarany@gmail.com>
 License: MIT
 Project-URL: Documentation, https://formation-studio.readthedocs.io/en/latest/
 Project-URL: Issues, https://github.com/ObaraEmmanuel/Formation/issues
 Project-URL: Source, https://github.com/ObaraEmmanuel/Formation
 Keywords: formation,gui,graphical-user-interface,drag drop,tkinter,hoverset,python
```

### Comparing `formation-studio-0.6.0/formation_studio.egg-info/SOURCES.txt` & `formation-studio-0.6.1/formation_studio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/hoverset/data/actions.py` & `formation-studio-0.6.1/hoverset/data/actions.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/hoverset/data/image.bak` & `formation-studio-0.6.1/hoverset/data/image.bak`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/hoverset/data/image.dat` & `formation-studio-0.6.1/hoverset/data/image.dat`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/hoverset/data/image.dir` & `formation-studio-0.6.1/hoverset/data/image.dir`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/hoverset/data/images.py` & `formation-studio-0.6.1/hoverset/data/images.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/hoverset/data/keymap.py` & `formation-studio-0.6.1/hoverset/data/keymap.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/hoverset/data/preferences.py` & `formation-studio-0.6.1/hoverset/data/preferences.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/hoverset/data/utils.py` & `formation-studio-0.6.1/hoverset/data/utils.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/hoverset/platform/__init__.py` & `formation-studio-0.6.1/hoverset/platform/__init__.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/hoverset/platform/functions.py` & `formation-studio-0.6.1/hoverset/platform/functions.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/hoverset/ui/animation.py` & `formation-studio-0.6.1/hoverset/ui/animation.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/hoverset/ui/color.tcl` & `formation-studio-0.6.1/hoverset/ui/color.tcl`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/hoverset/ui/dialogs.py` & `formation-studio-0.6.1/hoverset/ui/dialogs.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/hoverset/ui/loaders.py` & `formation-studio-0.6.1/hoverset/ui/loaders.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/hoverset/ui/menu.py` & `formation-studio-0.6.1/hoverset/ui/menu.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/hoverset/ui/panels.py` & `formation-studio-0.6.1/hoverset/ui/panels.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/hoverset/ui/pickers.py` & `formation-studio-0.6.1/hoverset/ui/pickers.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/hoverset/ui/styles.py` & `formation-studio-0.6.1/hoverset/ui/styles.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/hoverset/ui/themes/default.css` & `formation-studio-0.6.1/hoverset/ui/themes/default.css`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/hoverset/ui/themes/light.css` & `formation-studio-0.6.1/hoverset/ui/themes/light.css`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/hoverset/ui/widgets.py` & `formation-studio-0.6.1/hoverset/ui/widgets.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/hoverset/ui/windows.py` & `formation-studio-0.6.1/hoverset/ui/windows.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/hoverset/util/__init__.py` & `formation-studio-0.6.1/hoverset/util/__init__.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/hoverset/util/color.py` & `formation-studio-0.6.1/hoverset/util/color.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/hoverset/util/execution.py` & `formation-studio-0.6.1/hoverset/util/execution.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/hoverset/util/validators.py` & `formation-studio-0.6.1/hoverset/util/validators.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/pyproject.toml` & `formation-studio-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/studio/cli.py` & `formation-studio-0.6.1/studio/cli.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/studio/context.py` & `formation-studio-0.6.1/studio/context.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/studio/debugtools/common.py` & `formation-studio-0.6.1/studio/debugtools/common.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/studio/debugtools/debugger.py` & `formation-studio-0.6.1/studio/debugtools/debugger.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/studio/debugtools/element_pane.py` & `formation-studio-0.6.1/studio/debugtools/element_pane.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/studio/debugtools/layouts.py` & `formation-studio-0.6.1/studio/debugtools/layouts.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/studio/debugtools/style_pane.py` & `formation-studio-0.6.1/studio/debugtools/style_pane.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/studio/feature/_base.py` & `formation-studio-0.6.1/studio/feature/_base.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/studio/feature/component_tree.py` & `formation-studio-0.6.1/studio/feature/component_tree.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/studio/feature/components.py` & `formation-studio-0.6.1/studio/feature/components.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/studio/feature/design.py` & `formation-studio-0.6.1/studio/feature/design.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/studio/feature/eventspane.py` & `formation-studio-0.6.1/studio/feature/eventspane.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/studio/feature/stylepane.py` & `formation-studio-0.6.1/studio/feature/stylepane.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/studio/feature/variablepane.py` & `formation-studio-0.6.1/studio/feature/variablepane.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/studio/lib/__init__.py` & `formation-studio-0.6.1/studio/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/studio/lib/canvas.py` & `formation-studio-0.6.1/studio/lib/canvas.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/studio/lib/layouts.py` & `formation-studio-0.6.1/studio/lib/layouts.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/studio/lib/legacy.py` & `formation-studio-0.6.1/studio/lib/legacy.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/studio/lib/menu.py` & `formation-studio-0.6.1/studio/lib/menu.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/studio/lib/native.py` & `formation-studio-0.6.1/studio/lib/native.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/studio/lib/properties.py` & `formation-studio-0.6.1/studio/lib/properties.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/studio/lib/pseudo.py` & `formation-studio-0.6.1/studio/lib/pseudo.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/studio/lib/toplevel.py` & `formation-studio-0.6.1/studio/lib/toplevel.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/studio/lib/variables.py` & `formation-studio-0.6.1/studio/lib/variables.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/studio/main.py` & `formation-studio-0.6.1/studio/main.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/studio/parsers/loader.py` & `formation-studio-0.6.1/studio/parsers/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -385,18 +385,19 @@
         :param path: Path to file to be written to
         :return: String
         """
         file_loader = infer_format(path)
         pref = Preferences.acquire()
         pref_path = f"designer::{file_loader.name.lower()}"
         pref.set_default(pref_path, {})
+        # generate an upto-date tree first
+        self.generate()
+        content = file_loader(node=self.root).generate(**pref.get(pref_path))
         with open(path, 'w') as dump:
-            # generate an upto-date tree first
-            self.generate()
-            dump.write(file_loader(node=self.root).generate(**pref.get(pref_path)))
+            dump.write(content)
 
     def __eq__(self, other):
         if isinstance(other, DesignBuilder):
             return self.root == other.root
         return False
 
     def __ne__(self, other):
```

### Comparing `formation-studio-0.6.0/studio/preferences.py` & `formation-studio-0.6.1/studio/preferences.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,14 +191,18 @@
         ),
         "Xml options": (
             {
                 "desc": "Pretty print output xml",
                 "path": "designer::xml::pretty_print",
                 "element": Check,
             },
+            {
+                "element": Note,
+                "desc": "(Requires lxml)"
+            }
         ),
         "JSON options": (
             {
                 "desc": "Compact output",
                 "path": "designer::json::compact",
                 "element": Check
             },
```

### Comparing `formation-studio-0.6.0/studio/resource_loader.py` & `formation-studio-0.6.1/studio/resource_loader.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/studio/resources/images/formation.ico` & `formation-studio-0.6.1/studio/resources/images/formation.ico`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/studio/resources/images/formation.png` & `formation-studio-0.6.1/studio/resources/images/formation.png`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/studio/resources/images/formation_icon.png` & `formation-studio-0.6.1/studio/resources/images/formation_icon.png`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/studio/resources/images/logo.png` & `formation-studio-0.6.1/studio/resources/images/logo.png`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/studio/tools/__init__.py` & `formation-studio-0.6.1/studio/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/studio/tools/_base.py` & `formation-studio-0.6.1/studio/tools/_base.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/studio/tools/canvas.py` & `formation-studio-0.6.1/studio/tools/canvas.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/studio/tools/menus.py` & `formation-studio-0.6.1/studio/tools/menus.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/studio/ui/about.py` & `formation-studio-0.6.1/studio/ui/about.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/studio/ui/editors.py` & `formation-studio-0.6.1/studio/ui/editors.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/studio/ui/geometry.py` & `formation-studio-0.6.1/studio/ui/geometry.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/studio/ui/highlight.py` & `formation-studio-0.6.1/studio/ui/highlight.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/studio/ui/tree.py` & `formation-studio-0.6.1/studio/ui/tree.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/studio/ui/widgets.py` & `formation-studio-0.6.1/studio/ui/widgets.py`

 * *Files identical despite different names*

### Comparing `formation-studio-0.6.0/studio/updates.py` & `formation-studio-0.6.1/studio/updates.py`

 * *Files identical despite different names*

