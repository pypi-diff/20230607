# Comparing `tmp/dexterity.membrane-3.0.1.tar.gz` & `tmp/dexterity.membrane-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dexterity.membrane-3.0.1.tar", last modified: Fri Mar 24 07:38:32 2023, max compression
+gzip compressed data, was "dexterity.membrane-3.0.2.tar", last modified: Wed Jun  7 06:32:30 2023, max compression
```

## Comparing `dexterity.membrane-3.0.1.tar` & `dexterity.membrane-3.0.2.tar`

### file list

```diff
@@ -1,111 +1,102 @@
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-03-24 07:38:32.483569 dexterity.membrane-3.0.1/
--rw-r--r--   0 peterm     (501) staff       (20)       39 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/.coveragerc
--rw-r--r--   0 peterm     (501) staff       (20)     5327 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/CHANGES.rst
--rw-r--r--   0 peterm     (501) staff       (20)      119 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/MANIFEST.in
--rw-r--r--   0 peterm     (501) staff       (20)    10763 2023-03-24 07:38:32.483641 dexterity.membrane-3.0.1/PKG-INFO
--rw-r--r--   0 peterm     (501) staff       (20)     4222 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/README.rst
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-03-24 07:38:32.474339 dexterity.membrane-3.0.1/dexterity/
--rw-r--r--   0 peterm     (501) staff       (20)       80 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/__init__.py
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-03-24 07:38:32.476052 dexterity.membrane-3.0.1/dexterity/membrane/
--rw-r--r--   0 peterm     (501) staff       (20)      201 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/__init__.py
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-03-24 07:38:32.477060 dexterity.membrane-3.0.1/dexterity/membrane/behavior/
--rw-r--r--   0 peterm     (501) staff       (20)       24 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/behavior/__init__.py
--rw-r--r--   0 peterm     (501) staff       (20)     2373 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/behavior/configure.zcml
--rw-r--r--   0 peterm     (501) staff       (20)     1265 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/behavior/group.py
--rw-r--r--   0 peterm     (501) staff       (20)      186 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/behavior/membranegroup.py
--rw-r--r--   0 peterm     (501) staff       (20)      402 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/behavior/membranepassword.py
--rw-r--r--   0 peterm     (501) staff       (20)      181 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/behavior/membraneuser.py
--rw-r--r--   0 peterm     (501) staff       (20)     6376 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/behavior/password.py
--rw-r--r--   0 peterm     (501) staff       (20)     1627 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/behavior/settings.py
--rw-r--r--   0 peterm     (501) staff       (20)     7593 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/behavior/user.py
--rw-r--r--   0 peterm     (501) staff       (20)     1377 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/configure.zcml
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-03-24 07:38:32.477395 dexterity.membrane-3.0.1/dexterity/membrane/content/
--rw-r--r--   0 peterm     (501) staff       (20)       24 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/content/__init__.py
--rw-r--r--   0 peterm     (501) staff       (20)      899 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/content/configure.zcml
--rw-r--r--   0 peterm     (501) staff       (20)     3956 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/content/member.py
--rw-r--r--   0 peterm     (501) staff       (20)      731 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/deprecation.py
--rw-r--r--   0 peterm     (501) staff       (20)      350 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/indexers.py
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-03-24 07:38:32.477733 dexterity.membrane-3.0.1/dexterity/membrane/locales/
--rw-r--r--   0 peterm     (501) staff       (20)     1562 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/locales/dexterity.membrane.pot
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-03-24 07:38:32.472064 dexterity.membrane-3.0.1/dexterity/membrane/locales/en/
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-03-24 07:38:32.478205 dexterity.membrane-3.0.1/dexterity/membrane/locales/en/LC_MESSAGES/
--rw-r--r--   0 peterm     (501) staff       (20)      470 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/locales/en/LC_MESSAGES/dexterity.membrane.mo
--rw-r--r--   0 peterm     (501) staff       (20)     1562 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/locales/en/LC_MESSAGES/dexterity.membrane.po
--rw-r--r--   0 peterm     (501) staff       (20)      458 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/locales/en/LC_MESSAGES/plone.mo
--rw-r--r--   0 peterm     (501) staff       (20)      484 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/locales/en/LC_MESSAGES/plone.po
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-03-24 07:38:32.472181 dexterity.membrane-3.0.1/dexterity/membrane/locales/es/
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-03-24 07:38:32.478937 dexterity.membrane-3.0.1/dexterity/membrane/locales/es/LC_MESSAGES/
--rw-r--r--   0 peterm     (501) staff       (20)     1228 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/locales/es/LC_MESSAGES/dexterity.membrane.mo
--rw-r--r--   0 peterm     (501) staff       (20)     1872 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/locales/es/LC_MESSAGES/dexterity.membrane.po
--rw-r--r--   0 peterm     (501) staff       (20)      473 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/locales/es/LC_MESSAGES/plone.mo
--rw-r--r--   0 peterm     (501) staff       (20)      611 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/locales/es/LC_MESSAGES/plone.po
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-03-24 07:38:32.472312 dexterity.membrane-3.0.1/dexterity/membrane/locales/fr/
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-03-24 07:38:32.479236 dexterity.membrane-3.0.1/dexterity/membrane/locales/fr/LC_MESSAGES/
--rw-r--r--   0 peterm     (501) staff       (20)     1267 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/locales/fr/LC_MESSAGES/dexterity.membrane.mo
--rw-r--r--   0 peterm     (501) staff       (20)     1892 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/locales/fr/LC_MESSAGES/dexterity.membrane.po
--rw-r--r--   0 peterm     (501) staff       (20)      610 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/locales/manual.pot
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-03-24 07:38:32.472432 dexterity.membrane-3.0.1/dexterity/membrane/locales/nl/
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-03-24 07:38:32.479847 dexterity.membrane-3.0.1/dexterity/membrane/locales/nl/LC_MESSAGES/
--rw-r--r--   0 peterm     (501) staff       (20)     1060 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/locales/nl/LC_MESSAGES/dexterity.membrane.mo
--rw-r--r--   0 peterm     (501) staff       (20)     1694 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/locales/nl/LC_MESSAGES/dexterity.membrane.po
--rw-r--r--   0 peterm     (501) staff       (20)      458 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/locales/nl/LC_MESSAGES/plone.mo
--rw-r--r--   0 peterm     (501) staff       (20)      484 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/locales/nl/LC_MESSAGES/plone.po
--rw-r--r--   0 peterm     (501) staff       (20)      610 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/locales/plone.pot
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-03-24 07:38:32.472556 dexterity.membrane-3.0.1/dexterity/membrane/locales/pt_BR/
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-03-24 07:38:32.480414 dexterity.membrane-3.0.1/dexterity/membrane/locales/pt_BR/LC_MESSAGES/
--rw-r--r--   0 peterm     (501) staff       (20)     1257 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/locales/pt_BR/LC_MESSAGES/dexterity.membrane.mo
--rw-r--r--   0 peterm     (501) staff       (20)     1905 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/locales/pt_BR/LC_MESSAGES/dexterity.membrane.po
--rw-r--r--   0 peterm     (501) staff       (20)      473 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/locales/pt_BR/LC_MESSAGES/plone.mo
--rw-r--r--   0 peterm     (501) staff       (20)      611 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/locales/pt_BR/LC_MESSAGES/plone.po
--rw-r--r--   0 peterm     (501) staff       (20)     3274 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/membrane_helpers.py
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-03-24 07:38:32.473068 dexterity.membrane-3.0.1/dexterity/membrane/profiles/
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-03-24 07:38:32.480959 dexterity.membrane-3.0.1/dexterity/membrane/profiles/content/
--rw-r--r--   0 peterm     (501) staff       (20)      138 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/profiles/content/membrane_tool.xml
--rw-r--r--   0 peterm     (501) staff       (20)      292 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/profiles/content/metadata.xml
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-03-24 07:38:32.481102 dexterity.membrane-3.0.1/dexterity/membrane/profiles/content/types/
--rw-r--r--   0 peterm     (501) staff       (20)     2818 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/profiles/content/types/dexterity.membrane.member.xml
--rw-r--r--   0 peterm     (501) staff       (20)      133 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/profiles/content/types.xml
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-03-24 07:38:32.472873 dexterity.membrane-3.0.1/dexterity/membrane/profiles/content/workflows/
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-03-24 07:38:32.481240 dexterity.membrane-3.0.1/dexterity/membrane/profiles/content/workflows/dexterity_membrane_workflow/
--rw-r--r--   0 peterm     (501) staff       (20)     6790 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/profiles/content/workflows/dexterity_membrane_workflow/definition.xml
--rw-r--r--   0 peterm     (501) staff       (20)      285 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/profiles/content/workflows.xml
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-03-24 07:38:32.481611 dexterity.membrane-3.0.1/dexterity/membrane/profiles/default/
--rw-r--r--   0 peterm     (501) staff       (20)      577 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/profiles/default/controlpanel.xml
--rw-r--r--   0 peterm     (501) staff       (20)      154 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/profiles/default/metadata.xml
--rw-r--r--   0 peterm     (501) staff       (20)      877 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/profiles/default/registry.xml
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-03-24 07:38:32.481956 dexterity.membrane-3.0.1/dexterity/membrane/profiles/uninstall/
--rw-r--r--   0 peterm     (501) staff       (20)      362 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/profiles/uninstall/controlpanel.xml
--rw-r--r--   0 peterm     (501) staff       (20)       49 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/profiles/uninstall/metadata.xml
--rw-r--r--   0 peterm     (501) staff       (20)      391 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/profiles/uninstall/registry.xml
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-03-24 07:38:32.482324 dexterity.membrane-3.0.1/dexterity/membrane/profiles/uninstall_content/
--rw-r--r--   0 peterm     (501) staff       (20)       49 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/profiles/uninstall_content/metadata.xml
--rw-r--r--   0 peterm     (501) staff       (20)      147 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/profiles/uninstall_content/types.xml
--rw-r--r--   0 peterm     (501) staff       (20)      237 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/profiles/uninstall_content/workflows.xml
--rwxr-xr-x   0 peterm     (501) staff       (20)      238 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/rebuild_i18n.sh
--rw-r--r--   0 peterm     (501) staff       (20)     1892 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/testing.py
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-03-24 07:38:32.482798 dexterity.membrane-3.0.1/dexterity/membrane/tests/
--rw-r--r--   0 peterm     (501) staff       (20)       24 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/tests/__init__.py
--rw-r--r--   0 peterm     (501) staff       (20)      688 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/tests/test_doctest.py
--rw-r--r--   0 peterm     (501) staff       (20)    21339 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/tests/test_member.py
--rw-r--r--   0 peterm     (501) staff       (20)     2392 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/tests/test_settings.py
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-03-24 07:38:32.483118 dexterity.membrane-3.0.1/dexterity/membrane/upgrades/
--rw-r--r--   0 peterm     (501) staff       (20)        0 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/upgrades/__init__.py
--rw-r--r--   0 peterm     (501) staff       (20)      444 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/upgrades/configure.zcml
--rw-r--r--   0 peterm     (501) staff       (20)     1277 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity/membrane/upgrades/to_1002.py
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-03-24 07:38:32.475245 dexterity.membrane-3.0.1/dexterity.membrane.egg-info/
--rw-r--r--   0 peterm     (501) staff       (20)    10763 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity.membrane.egg-info/PKG-INFO
--rw-r--r--   0 peterm     (501) staff       (20)     3561 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity.membrane.egg-info/SOURCES.txt
--rw-r--r--   0 peterm     (501) staff       (20)        1 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity.membrane.egg-info/dependency_links.txt
--rw-r--r--   0 peterm     (501) staff       (20)       40 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity.membrane.egg-info/entry_points.txt
--rw-r--r--   0 peterm     (501) staff       (20)       10 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity.membrane.egg-info/namespace_packages.txt
--rw-r--r--   0 peterm     (501) staff       (20)        1 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity.membrane.egg-info/not-zip-safe
--rw-r--r--   0 peterm     (501) staff       (20)      204 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity.membrane.egg-info/requires.txt
--rw-r--r--   0 peterm     (501) staff       (20)       10 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/dexterity.membrane.egg-info/top_level.txt
-drwxr-xr-x   0 peterm     (501) staff       (20)        0 2023-03-24 07:38:32.483464 dexterity.membrane-3.0.1/docs/
--rw-r--r--   0 peterm     (501) staff       (20)      494 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/docs/INSTALL.rst
--rw-r--r--   0 peterm     (501) staff       (20)    17987 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/docs/LICENSE.GPL
--rw-r--r--   0 peterm     (501) staff       (20)      735 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/docs/LICENSE.txt
--rw-r--r--   0 peterm     (501) staff       (20)       62 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/requirements-5.2.txt
--rw-r--r--   0 peterm     (501) staff       (20)       62 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/requirements-6.0.txt
--rw-r--r--   0 peterm     (501) staff       (20)      105 2023-03-24 07:38:32.483868 dexterity.membrane-3.0.1/setup.cfg
--rw-r--r--   0 peterm     (501) staff       (20)     2097 2023-03-24 07:38:32.000000 dexterity.membrane-3.0.1/setup.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-07 06:32:30.510095 dexterity.membrane-3.0.2/
+-rw-rw-r--   0 ale       (1000) ale       (1000)       39 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/.coveragerc
+-rw-rw-r--   0 ale       (1000) ale       (1000)     5410 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/CHANGES.rst
+-rw-rw-r--   0 ale       (1000) ale       (1000)      119 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/MANIFEST.in
+-rw-rw-r--   0 ale       (1000) ale       (1000)    10846 2023-06-07 06:32:30.510095 dexterity.membrane-3.0.2/PKG-INFO
+-rw-rw-r--   0 ale       (1000) ale       (1000)     4222 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/README.rst
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-07 06:32:30.506095 dexterity.membrane-3.0.2/dexterity/
+-rw-rw-r--   0 ale       (1000) ale       (1000)       80 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/__init__.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-07 06:32:30.506095 dexterity.membrane-3.0.2/dexterity/membrane/
+-rw-rw-r--   0 ale       (1000) ale       (1000)      201 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/__init__.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-07 06:32:30.510095 dexterity.membrane-3.0.2/dexterity/membrane/behavior/
+-rw-rw-r--   0 ale       (1000) ale       (1000)       24 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/behavior/__init__.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2373 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/behavior/configure.zcml
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1265 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/behavior/group.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      186 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/behavior/membranegroup.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      402 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/behavior/membranepassword.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      181 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/behavior/membraneuser.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     6375 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/behavior/password.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1627 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/behavior/settings.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     7593 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/behavior/user.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1377 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/configure.zcml
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-07 06:32:30.510095 dexterity.membrane-3.0.2/dexterity/membrane/content/
+-rw-rw-r--   0 ale       (1000) ale       (1000)       24 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/content/__init__.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      899 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/content/configure.zcml
+-rw-rw-r--   0 ale       (1000) ale       (1000)     3956 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/content/member.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      731 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/deprecation.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      350 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/indexers.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-07 06:32:30.510095 dexterity.membrane-3.0.2/dexterity/membrane/locales/
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1562 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/locales/dexterity.membrane.pot
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-07 06:32:30.506095 dexterity.membrane-3.0.2/dexterity/membrane/locales/en/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-07 06:32:30.510095 dexterity.membrane-3.0.2/dexterity/membrane/locales/en/LC_MESSAGES/
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1562 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/locales/en/LC_MESSAGES/dexterity.membrane.po
+-rw-rw-r--   0 ale       (1000) ale       (1000)      484 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/locales/en/LC_MESSAGES/plone.po
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-07 06:32:30.506095 dexterity.membrane-3.0.2/dexterity/membrane/locales/es/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-07 06:32:30.510095 dexterity.membrane-3.0.2/dexterity/membrane/locales/es/LC_MESSAGES/
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1872 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/locales/es/LC_MESSAGES/dexterity.membrane.po
+-rw-rw-r--   0 ale       (1000) ale       (1000)      611 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/locales/es/LC_MESSAGES/plone.po
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-07 06:32:30.506095 dexterity.membrane-3.0.2/dexterity/membrane/locales/fr/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-07 06:32:30.510095 dexterity.membrane-3.0.2/dexterity/membrane/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1892 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/locales/fr/LC_MESSAGES/dexterity.membrane.po
+-rw-rw-r--   0 ale       (1000) ale       (1000)      610 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/locales/manual.pot
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-07 06:32:30.506095 dexterity.membrane-3.0.2/dexterity/membrane/locales/nl/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-07 06:32:30.510095 dexterity.membrane-3.0.2/dexterity/membrane/locales/nl/LC_MESSAGES/
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1694 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/locales/nl/LC_MESSAGES/dexterity.membrane.po
+-rw-rw-r--   0 ale       (1000) ale       (1000)      484 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/locales/nl/LC_MESSAGES/plone.po
+-rw-rw-r--   0 ale       (1000) ale       (1000)      610 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/locales/plone.pot
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-07 06:32:30.506095 dexterity.membrane-3.0.2/dexterity/membrane/locales/pt_BR/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-07 06:32:30.510095 dexterity.membrane-3.0.2/dexterity/membrane/locales/pt_BR/LC_MESSAGES/
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1905 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/locales/pt_BR/LC_MESSAGES/dexterity.membrane.po
+-rw-rw-r--   0 ale       (1000) ale       (1000)      611 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/locales/pt_BR/LC_MESSAGES/plone.po
+-rw-rw-r--   0 ale       (1000) ale       (1000)     3274 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/membrane_helpers.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-07 06:32:30.506095 dexterity.membrane-3.0.2/dexterity/membrane/profiles/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-07 06:32:30.510095 dexterity.membrane-3.0.2/dexterity/membrane/profiles/content/
+-rw-rw-r--   0 ale       (1000) ale       (1000)      138 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/profiles/content/membrane_tool.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)      292 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/profiles/content/metadata.xml
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-07 06:32:30.510095 dexterity.membrane-3.0.2/dexterity/membrane/profiles/content/types/
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2818 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/profiles/content/types/dexterity.membrane.member.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)      133 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/profiles/content/types.xml
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-07 06:32:30.506095 dexterity.membrane-3.0.2/dexterity/membrane/profiles/content/workflows/
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-07 06:32:30.510095 dexterity.membrane-3.0.2/dexterity/membrane/profiles/content/workflows/dexterity_membrane_workflow/
+-rw-rw-r--   0 ale       (1000) ale       (1000)     6790 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/profiles/content/workflows/dexterity_membrane_workflow/definition.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)      285 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/profiles/content/workflows.xml
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-07 06:32:30.510095 dexterity.membrane-3.0.2/dexterity/membrane/profiles/default/
+-rw-rw-r--   0 ale       (1000) ale       (1000)      577 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/profiles/default/controlpanel.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)      154 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/profiles/default/metadata.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)      877 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/profiles/default/registry.xml
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-07 06:32:30.510095 dexterity.membrane-3.0.2/dexterity/membrane/profiles/uninstall/
+-rw-rw-r--   0 ale       (1000) ale       (1000)      362 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/profiles/uninstall/controlpanel.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)       49 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/profiles/uninstall/metadata.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)      391 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/profiles/uninstall/registry.xml
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-07 06:32:30.510095 dexterity.membrane-3.0.2/dexterity/membrane/profiles/uninstall_content/
+-rw-rw-r--   0 ale       (1000) ale       (1000)       49 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/profiles/uninstall_content/metadata.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)      147 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/profiles/uninstall_content/types.xml
+-rw-rw-r--   0 ale       (1000) ale       (1000)      237 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/profiles/uninstall_content/workflows.xml
+-rwxrwxr-x   0 ale       (1000) ale       (1000)      238 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/rebuild_i18n.sh
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1892 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/testing.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-07 06:32:30.510095 dexterity.membrane-3.0.2/dexterity/membrane/tests/
+-rw-rw-r--   0 ale       (1000) ale       (1000)       24 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/tests/__init__.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      688 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/tests/test_doctest.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)    21336 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/tests/test_member.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2392 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/tests/test_settings.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-07 06:32:30.510095 dexterity.membrane-3.0.2/dexterity/membrane/upgrades/
+-rw-rw-r--   0 ale       (1000) ale       (1000)        0 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/upgrades/__init__.py
+-rw-rw-r--   0 ale       (1000) ale       (1000)      444 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/upgrades/configure.zcml
+-rw-rw-r--   0 ale       (1000) ale       (1000)     1277 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity/membrane/upgrades/to_1002.py
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-07 06:32:30.506095 dexterity.membrane-3.0.2/dexterity.membrane.egg-info/
+-rw-rw-r--   0 ale       (1000) ale       (1000)    10846 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity.membrane.egg-info/PKG-INFO
+-rw-rw-r--   0 ale       (1000) ale       (1000)     3031 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity.membrane.egg-info/SOURCES.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        1 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity.membrane.egg-info/dependency_links.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)       40 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity.membrane.egg-info/entry_points.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)       10 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity.membrane.egg-info/namespace_packages.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)        1 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity.membrane.egg-info/not-zip-safe
+-rw-rw-r--   0 ale       (1000) ale       (1000)      204 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity.membrane.egg-info/requires.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)       10 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/dexterity.membrane.egg-info/top_level.txt
+drwxrwxr-x   0 ale       (1000) ale       (1000)        0 2023-06-07 06:32:30.510095 dexterity.membrane-3.0.2/docs/
+-rw-rw-r--   0 ale       (1000) ale       (1000)      494 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/docs/INSTALL.rst
+-rw-rw-r--   0 ale       (1000) ale       (1000)    17987 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/docs/LICENSE.GPL
+-rw-rw-r--   0 ale       (1000) ale       (1000)      735 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/docs/LICENSE.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)       62 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/requirements-5.2.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)       62 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/requirements-6.0.txt
+-rw-rw-r--   0 ale       (1000) ale       (1000)      105 2023-06-07 06:32:30.510095 dexterity.membrane-3.0.2/setup.cfg
+-rw-rw-r--   0 ale       (1000) ale       (1000)     2097 2023-06-07 06:32:30.000000 dexterity.membrane-3.0.2/setup.py
```

### Comparing `dexterity.membrane-3.0.1/CHANGES.rst` & `dexterity.membrane-3.0.2/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 Changelog
 =========
 
 
+3.0.2 (2023-06-07)
+------------------
+
+- Remove deprecation warnings.
+  [ale-rt]
+
+
 3.0.1 (2023-03-24)
 ------------------
 
 - Fix for `AuthEncoding >= 5.0`.
   [petschki]
 
 - Rename profile `dexterity.membrane: example` -> `dexterity.membrane: content`
```

### Comparing `dexterity.membrane-3.0.1/PKG-INFO` & `dexterity.membrane-3.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dexterity.membrane
-Version: 3.0.1
+Version: 3.0.2
 Summary: Dexterity content and behaviors to integrate with membrane.
 Home-page: https://github.com/collective/dexterity.membrane
 Author: Maurits van Rees
 Author-email: maurits@vanrees.org
 License: GPL
 Keywords: plone dexterity membrane
 Classifier: Development Status :: 5 - Production/Stable
@@ -146,14 +146,21 @@
 
 .. _bcrypt: https://en.wikipedia.org/wiki/Bcrypt
 
 Changelog
 =========
 
 
+3.0.2 (2023-06-07)
+------------------
+
+- Remove deprecation warnings.
+  [ale-rt]
+
+
 3.0.1 (2023-03-24)
 ------------------
 
 - Fix for `AuthEncoding >= 5.0`.
   [petschki]
 
 - Rename profile `dexterity.membrane: example` -> `dexterity.membrane: content`
```

### Comparing `dexterity.membrane-3.0.1/README.rst` & `dexterity.membrane-3.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `dexterity.membrane-3.0.1/dexterity/membrane/behavior/configure.zcml` & `dexterity.membrane-3.0.2/dexterity/membrane/behavior/configure.zcml`

 * *Files identical despite different names*

### Comparing `dexterity.membrane-3.0.1/dexterity/membrane/behavior/group.py` & `dexterity.membrane-3.0.2/dexterity/membrane/behavior/group.py`

 * *Files identical despite different names*

### Comparing `dexterity.membrane-3.0.1/dexterity/membrane/behavior/password.py` & `dexterity.membrane-3.0.2/dexterity/membrane/behavior/password.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-from AccessControl import AuthEncoding
+from AuthEncoding import AuthEncoding
 from dexterity.membrane import _
 from dexterity.membrane.behavior.user import IMembraneUser
 from dexterity.membrane.behavior.user import IMembraneUserWorkflow
 from plone.autoform import directives
 from plone.autoform.interfaces import IFormFieldProvider
 from plone.memoize import ram
 from plone.supermodel import model
```

### Comparing `dexterity.membrane-3.0.1/dexterity/membrane/behavior/settings.py` & `dexterity.membrane-3.0.2/dexterity/membrane/behavior/settings.py`

 * *Files identical despite different names*

### Comparing `dexterity.membrane-3.0.1/dexterity/membrane/behavior/user.py` & `dexterity.membrane-3.0.2/dexterity/membrane/behavior/user.py`

 * *Files identical despite different names*

### Comparing `dexterity.membrane-3.0.1/dexterity/membrane/configure.zcml` & `dexterity.membrane-3.0.2/dexterity/membrane/configure.zcml`

 * *Files identical despite different names*

### Comparing `dexterity.membrane-3.0.1/dexterity/membrane/content/configure.zcml` & `dexterity.membrane-3.0.2/dexterity/membrane/content/configure.zcml`

 * *Files identical despite different names*

### Comparing `dexterity.membrane-3.0.1/dexterity/membrane/content/member.py` & `dexterity.membrane-3.0.2/dexterity/membrane/content/member.py`

 * *Files identical despite different names*

### Comparing `dexterity.membrane-3.0.1/dexterity/membrane/deprecation.py` & `dexterity.membrane-3.0.2/dexterity/membrane/deprecation.py`

 * *Files identical despite different names*

### Comparing `dexterity.membrane-3.0.1/dexterity/membrane/locales/dexterity.membrane.pot` & `dexterity.membrane-3.0.2/dexterity/membrane/locales/dexterity.membrane.pot`

 * *Files identical despite different names*

### Comparing `dexterity.membrane-3.0.1/dexterity/membrane/locales/en/LC_MESSAGES/dexterity.membrane.po` & `dexterity.membrane-3.0.2/dexterity/membrane/locales/en/LC_MESSAGES/dexterity.membrane.po`

 * *Files identical despite different names*

### Comparing `dexterity.membrane-3.0.1/dexterity/membrane/locales/es/LC_MESSAGES/dexterity.membrane.po` & `dexterity.membrane-3.0.2/dexterity/membrane/locales/es/LC_MESSAGES/dexterity.membrane.po`

 * *Files identical despite different names*

### Comparing `dexterity.membrane-3.0.1/dexterity/membrane/locales/es/LC_MESSAGES/plone.po` & `dexterity.membrane-3.0.2/dexterity/membrane/locales/es/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `dexterity.membrane-3.0.1/dexterity/membrane/locales/fr/LC_MESSAGES/dexterity.membrane.po` & `dexterity.membrane-3.0.2/dexterity/membrane/locales/fr/LC_MESSAGES/dexterity.membrane.po`

 * *Files identical despite different names*

### Comparing `dexterity.membrane-3.0.1/dexterity/membrane/locales/manual.pot` & `dexterity.membrane-3.0.2/dexterity/membrane/locales/manual.pot`

 * *Files identical despite different names*

### Comparing `dexterity.membrane-3.0.1/dexterity/membrane/locales/nl/LC_MESSAGES/dexterity.membrane.po` & `dexterity.membrane-3.0.2/dexterity/membrane/locales/nl/LC_MESSAGES/dexterity.membrane.po`

 * *Files identical despite different names*

### Comparing `dexterity.membrane-3.0.1/dexterity/membrane/locales/plone.pot` & `dexterity.membrane-3.0.2/dexterity/membrane/locales/plone.pot`

 * *Files identical despite different names*

### Comparing `dexterity.membrane-3.0.1/dexterity/membrane/locales/pt_BR/LC_MESSAGES/dexterity.membrane.po` & `dexterity.membrane-3.0.2/dexterity/membrane/locales/pt_BR/LC_MESSAGES/dexterity.membrane.po`

 * *Files identical despite different names*

### Comparing `dexterity.membrane-3.0.1/dexterity/membrane/locales/pt_BR/LC_MESSAGES/plone.po` & `dexterity.membrane-3.0.2/dexterity/membrane/locales/pt_BR/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `dexterity.membrane-3.0.1/dexterity/membrane/membrane_helpers.py` & `dexterity.membrane-3.0.2/dexterity/membrane/membrane_helpers.py`

 * *Files identical despite different names*

### Comparing `dexterity.membrane-3.0.1/dexterity/membrane/profiles/content/types/dexterity.membrane.member.xml` & `dexterity.membrane-3.0.2/dexterity/membrane/profiles/content/types/dexterity.membrane.member.xml`

 * *Files identical despite different names*

### Comparing `dexterity.membrane-3.0.1/dexterity/membrane/profiles/content/workflows/dexterity_membrane_workflow/definition.xml` & `dexterity.membrane-3.0.2/dexterity/membrane/profiles/content/workflows/dexterity_membrane_workflow/definition.xml`

 * *Files identical despite different names*

### Comparing `dexterity.membrane-3.0.1/dexterity/membrane/profiles/default/controlpanel.xml` & `dexterity.membrane-3.0.2/dexterity/membrane/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `dexterity.membrane-3.0.1/dexterity/membrane/profiles/default/registry.xml` & `dexterity.membrane-3.0.2/dexterity/membrane/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `dexterity.membrane-3.0.1/dexterity/membrane/testing.py` & `dexterity.membrane-3.0.2/dexterity/membrane/testing.py`

 * *Files identical despite different names*

### Comparing `dexterity.membrane-3.0.1/dexterity/membrane/tests/test_doctest.py` & `dexterity.membrane-3.0.2/dexterity/membrane/tests/test_doctest.py`

 * *Files identical despite different names*

### Comparing `dexterity.membrane-3.0.1/dexterity/membrane/tests/test_member.py` & `dexterity.membrane-3.0.2/dexterity/membrane/tests/test_member.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,15 +212,15 @@
                 membrane.unrestrictedSearchResults(
                     exact_getUserName='joe@example.org'),
             ),
             0
         )
 
     def _legacy_set_password(self, member, password):
-        from AccessControl import AuthEncoding
+        from AuthEncoding import AuthEncoding
         # Default AuthEncoding 'encryption' uses SSHA
         member.password = AuthEncoding.pw_encrypt(password)
         self.layer['portal'].membrane_tool.reindexObject(member)
 
     def test_legacy_password_authentication(self):
         from Products.membrane.interfaces import IMembraneUserAuth
         member = self._createType(
@@ -234,26 +234,26 @@
         self.assertTrue(
             pw_auth.verifyCredentials(dict(login=u'joe@example.com',
                                            password='foobar',
                                            confirm_password='foobar',))
         )
 
     def test_legacy_password_validates(self):
-        from AccessControl import AuthEncoding
+        from AuthEncoding import AuthEncoding
         member = self._createType(
             self.layer['portal'],
             'dexterity.membrane.member',
             'joe',
         )
         member.email = 'joe@example.org'
         self._legacy_set_password(member, b'foobar')
         self.assertTrue(AuthEncoding.pw_validate(member.password, b'foobar'))
 
     def test_reset_password(self):
-        from AccessControl import AuthEncoding
+        from AuthEncoding import AuthEncoding
         member = self._createType(
             self.layer['portal'],
             'dexterity.membrane.member',
             'joe',
         )
         member.email = 'joe@example.org'
         self.layer['portal'].membrane_tool.reindexObject(member)
```

### Comparing `dexterity.membrane-3.0.1/dexterity/membrane/tests/test_settings.py` & `dexterity.membrane-3.0.2/dexterity/membrane/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `dexterity.membrane-3.0.1/dexterity/membrane/upgrades/to_1002.py` & `dexterity.membrane-3.0.2/dexterity/membrane/upgrades/to_1002.py`

 * *Files identical despite different names*

### Comparing `dexterity.membrane-3.0.1/dexterity.membrane.egg-info/PKG-INFO` & `dexterity.membrane-3.0.2/dexterity.membrane.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dexterity.membrane
-Version: 3.0.1
+Version: 3.0.2
 Summary: Dexterity content and behaviors to integrate with membrane.
 Home-page: https://github.com/collective/dexterity.membrane
 Author: Maurits van Rees
 Author-email: maurits@vanrees.org
 License: GPL
 Keywords: plone dexterity membrane
 Classifier: Development Status :: 5 - Production/Stable
@@ -146,14 +146,21 @@
 
 .. _bcrypt: https://en.wikipedia.org/wiki/Bcrypt
 
 Changelog
 =========
 
 
+3.0.2 (2023-06-07)
+------------------
+
+- Remove deprecation warnings.
+  [ale-rt]
+
+
 3.0.1 (2023-03-24)
 ------------------
 
 - Fix for `AuthEncoding >= 5.0`.
   [petschki]
 
 - Rename profile `dexterity.membrane: example` -> `dexterity.membrane: content`
```

### Comparing `dexterity.membrane-3.0.1/dexterity.membrane.egg-info/SOURCES.txt` & `dexterity.membrane-3.0.2/dexterity.membrane.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -33,31 +33,22 @@
 dexterity/membrane/behavior/user.py
 dexterity/membrane/content/__init__.py
 dexterity/membrane/content/configure.zcml
 dexterity/membrane/content/member.py
 dexterity/membrane/locales/dexterity.membrane.pot
 dexterity/membrane/locales/manual.pot
 dexterity/membrane/locales/plone.pot
-dexterity/membrane/locales/en/LC_MESSAGES/dexterity.membrane.mo
 dexterity/membrane/locales/en/LC_MESSAGES/dexterity.membrane.po
-dexterity/membrane/locales/en/LC_MESSAGES/plone.mo
 dexterity/membrane/locales/en/LC_MESSAGES/plone.po
-dexterity/membrane/locales/es/LC_MESSAGES/dexterity.membrane.mo
 dexterity/membrane/locales/es/LC_MESSAGES/dexterity.membrane.po
-dexterity/membrane/locales/es/LC_MESSAGES/plone.mo
 dexterity/membrane/locales/es/LC_MESSAGES/plone.po
-dexterity/membrane/locales/fr/LC_MESSAGES/dexterity.membrane.mo
 dexterity/membrane/locales/fr/LC_MESSAGES/dexterity.membrane.po
-dexterity/membrane/locales/nl/LC_MESSAGES/dexterity.membrane.mo
 dexterity/membrane/locales/nl/LC_MESSAGES/dexterity.membrane.po
-dexterity/membrane/locales/nl/LC_MESSAGES/plone.mo
 dexterity/membrane/locales/nl/LC_MESSAGES/plone.po
-dexterity/membrane/locales/pt_BR/LC_MESSAGES/dexterity.membrane.mo
 dexterity/membrane/locales/pt_BR/LC_MESSAGES/dexterity.membrane.po
-dexterity/membrane/locales/pt_BR/LC_MESSAGES/plone.mo
 dexterity/membrane/locales/pt_BR/LC_MESSAGES/plone.po
 dexterity/membrane/profiles/content/membrane_tool.xml
 dexterity/membrane/profiles/content/metadata.xml
 dexterity/membrane/profiles/content/types.xml
 dexterity/membrane/profiles/content/workflows.xml
 dexterity/membrane/profiles/content/types/dexterity.membrane.member.xml
 dexterity/membrane/profiles/content/workflows/dexterity_membrane_workflow/definition.xml
```

### Comparing `dexterity.membrane-3.0.1/docs/LICENSE.GPL` & `dexterity.membrane-3.0.2/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `dexterity.membrane-3.0.1/docs/LICENSE.txt` & `dexterity.membrane-3.0.2/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dexterity.membrane-3.0.1/setup.py` & `dexterity.membrane-3.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = '3.0.1'
+version = '3.0.2'
 
 setup(
     name='dexterity.membrane',
     version=version,
     description='Dexterity content and behaviors to integrate with membrane.',
     long_description=(
         open('README.rst').read() + '\n' +
```

