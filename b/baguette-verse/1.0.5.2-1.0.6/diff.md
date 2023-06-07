# Comparing `tmp/baguette_verse-1.0.5.2.tar.gz` & `tmp/baguette_verse-1.0.6.tar.gz`

## Comparing `baguette_verse-1.0.5.2.tar` & `baguette_verse-1.0.6.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/__init__.py
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/baguette.py
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/logger.py
--rw-r--r--   0        0        0    24429 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/rack.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/__init__.py
--rw-r--r--   0        0        0    23863 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/bake.py
--rw-r--r--   0        0        0     5124 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/compiler.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/__init__.py
--rw-r--r--   0        0        0    13119 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/build.py
--rw-r--r--   0        0        0    17960 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/colors.py
--rw-r--r--   0        0        0     7862 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/config.py
--rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/event.py
--rw-r--r--   0        0        0     9262 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/filters.py
--rw-r--r--   0        0        0    34141 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/graph.py
--rw-r--r--   0        0        0     4633 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/record.py
--rw-r--r--   0        0        0     7635 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/utils.py
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/__init__.py
--rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/utils.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/data/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/data/__proc__.py
--rw-r--r--   0        0        0    13656 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/data/entities.py
--rw-r--r--   0        0        0     7833 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/data/integration.py
--rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/data/relations.py
--rw-r--r--   0        0        0     9533 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/data/utils.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/execution/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/execution/__proc__.py
--rw-r--r--   0        0        0    10104 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/execution/entities.py
--rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/execution/integration.py
--rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/execution/relations.py
--rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/execution/utils.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/filesystem/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/filesystem/__proc__.py
--rw-r--r--   0        0        0     6524 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/filesystem/entities.py
--rw-r--r--   0        0        0    13702 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/filesystem/integration.py
--rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/filesystem/relations.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/imports/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/imports/__proc__.py
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/imports/entities.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/imports/integration.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/imports/relations.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/network/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/network/__proc__.py
--rw-r--r--   0        0        0    10482 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/network/entities.py
--rw-r--r--   0        0        0     9931 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/network/integration.py
--rw-r--r--   0        0        0     5164 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/network/relations.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/registry/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/registry/__proc__.py
--rw-r--r--   0        0        0    11045 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/registry/entities.py
--rw-r--r--   0        0        0    16630 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/registry/integration.py
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/bakery/source/types/registry/relations.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/croutons/__init__.py
--rw-r--r--   0        0        0     5081 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/croutons/extractor.py
--rw-r--r--   0        0        0    20653 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/croutons/toast.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/croutons/metalib/__init__.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/croutons/metalib/interact.py
--rw-r--r--   0        0        0     4784 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/croutons/metalib/utils.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/croutons/source/__init__.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/croutons/source/evaluator.py
--rw-r--r--   0        0        0    35062 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/croutons/source/metagraph.py
--rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/croutons/source/utils.py
--rw-r--r--   0        0        0  9439185 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/tutorial/data.zip
--rw-r--r--   0        0        0    16890 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/tutorial/scripts.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/tutorial/state.txt
--rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/baguette/tutorial/utils.py
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/.gitignore
--rw-r--r--   0        0        0    35123 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/LICENSE
--rw-r--r--   0        0        0     8419 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/README.md
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/pyproject.toml
--rw-r--r--   0        0        0    48797 2020-02-02 00:00:00.000000 baguette_verse-1.0.5.2/PKG-INFO
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/__init__.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/baguette.py
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/logger.py
+-rw-r--r--   0        0        0    16694 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/rack.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/__init__.py
+-rw-r--r--   0        0        0    23828 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/bake.py
+-rw-r--r--   0        0        0     6109 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/compiler.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/__init__.py
+-rw-r--r--   0        0        0    13119 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/build.py
+-rw-r--r--   0        0        0    17960 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/colors.py
+-rw-r--r--   0        0        0     7862 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/config.py
+-rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/event.py
+-rw-r--r--   0        0        0     9262 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/filters.py
+-rw-r--r--   0        0        0    34141 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/graph.py
+-rw-r--r--   0        0        0     4633 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/record.py
+-rw-r--r--   0        0        0     7635 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/utils.py
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/__init__.py
+-rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/utils.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/data/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/data/__proc__.py
+-rw-r--r--   0        0        0    13656 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/data/entities.py
+-rw-r--r--   0        0        0     7833 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/data/integration.py
+-rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/data/relations.py
+-rw-r--r--   0        0        0     9533 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/data/utils.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/execution/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/execution/__proc__.py
+-rw-r--r--   0        0        0    10104 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/execution/entities.py
+-rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/execution/integration.py
+-rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/execution/relations.py
+-rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/execution/utils.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/filesystem/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/filesystem/__proc__.py
+-rw-r--r--   0        0        0     6524 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/filesystem/entities.py
+-rw-r--r--   0        0        0    13702 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/filesystem/integration.py
+-rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/filesystem/relations.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/imports/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/imports/__proc__.py
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/imports/entities.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/imports/integration.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/imports/relations.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/network/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/network/__proc__.py
+-rw-r--r--   0        0        0    10482 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/network/entities.py
+-rw-r--r--   0        0        0     9931 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/network/integration.py
+-rw-r--r--   0        0        0     5164 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/network/relations.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/registry/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/registry/__proc__.py
+-rw-r--r--   0        0        0    11045 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/registry/entities.py
+-rw-r--r--   0        0        0    16630 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/registry/integration.py
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/bakery/source/types/registry/relations.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/croutons/__init__.py
+-rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/croutons/extractor.py
+-rw-r--r--   0        0        0    20675 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/croutons/toast.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/croutons/metalib/__init__.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/croutons/metalib/interact.py
+-rw-r--r--   0        0        0     4784 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/croutons/metalib/utils.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/croutons/source/__init__.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/croutons/source/evaluator.py
+-rw-r--r--   0        0        0    35062 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/croutons/source/metagraph.py
+-rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/croutons/source/utils.py
+-rw-r--r--   0        0        0  9439185 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/tutorial/data.zip
+-rw-r--r--   0        0        0    16890 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/tutorial/scripts.py
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/tutorial/state.txt
+-rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/baguette/tutorial/utils.py
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/.gitignore
+-rw-r--r--   0        0        0    35123 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/LICENSE
+-rw-r--r--   0        0        0     8419 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/README.md
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0    48795 2020-02-02 00:00:00.000000 baguette_verse-1.0.6/PKG-INFO
```

### Comparing `baguette_verse-1.0.5.2/baguette/baguette.py` & `baguette_verse-1.0.6/baguette/baguette.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.2/baguette/logger.py` & `baguette_verse-1.0.6/baguette/logger.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.2/baguette/bakery/bake.py` & `baguette_verse-1.0.6/baguette/bakery/bake.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,16 +153,16 @@
                 r, g, b = int(r, 16), int(g, 16), int(b, 16)
             else:
                 parser.error(f"could not understand color format : '{c}'")
 
             return Color(r, g, b)
 
     parser.add_argument("reports", type=PathSorter(reports, "report"), default=None, nargs="*" if "BAGUETTE_REPORTS" in environ else "+", help="Cuckoo report files (.json) to bake baguettes from. Can also be folders containing reports. Defaults to environment variable 'BAGUETTE_REPORTS' if set.")
-    parser.add_argument("--baguettes", type=PathSorter(baguettes, "baguette"), default=None, action="extend", nargs="*", help="the path(s) to the output baguette files (.pyt). Use '-' to leave it to the automatic destination. Defaults to environment variable 'BAGUETTE_BAGUETTES' or '-' if not set.")
-    parser.add_argument("--visuals", type=PathSorter(visuals, "visual"), default=None, action="extend", nargs="*", help="the path(s) to the output visual (Gephi) files (.gexf). Use '-' to leave it to the automatic destination. Defaults to environment variable 'BAGUETTE_VISUALS' or '-' if not set.")
+    parser.add_argument("--baguettes", type=PathSorter(baguettes, "baguette"), default=None, action="extend", nargs="*", help="the path(s) to the output (copy) baguette files (.pyt). Use '-' to leave it to the automatic destination. Defaults to environment variable 'BAGUETTE_BAGUETTES' or '-' if not set.")
+    parser.add_argument("--visuals", type=PathSorter(visuals, "visual"), default=None, action="extend", nargs="*", help="the path(s) to the output (copy) visual (Gephi) files (.gexf). Use '-' to leave it to the automatic destination. Defaults to environment variable 'BAGUETTE_VISUALS' or '-' if not set.")
     parser.add_argument("-o", "--outputs", type=PathSorter(outputs, "output"), default=None, action="extend", nargs="*", help="the path to the result index folders (which end in .bag). They contain the index file (.pyt) which stores all the information about a given baguette. Use '-' to leave it to the automatic destination. Defaults to environment variable 'BAGUETTE_OUTPUTS' or '.' if not set.")
     parser.add_argument("--pool", type=pool_size, default=pool_size("0.5"), help="the size of the process pool to use to bake in parallel.")
     parser.add_argument("--maxtime", type=time, default=time("inf"), help="the maximum amount of time spent baking a single baguette. No maxtime by default.")
     parser.add_argument("-f", "--filters", type=str, default=[], choices=[name for name in dir(filters) if isinstance(getattr(filters, name), filters.Filter)], nargs="*", help="a list of filters that can be used when exporting the baguette to the visual file (.gexf).")
     parser.add_argument("--perf", action="store_true", default=False, help="if this is enabled, a performance report will be printed at the end of the baking process.")
     parser.add_argument("-v", "--verbosity", action="count", default=0, help="increases the verbosity of the output.")
     parser.add_argument("--skip_data_comparison", action="store_true", default=False, help="if enabled, the computation of the Levenshtein similarity between all Data nodes will be skipped.")
@@ -403,15 +403,15 @@
         if isinstance(b, list) and len(b) != n:
             parser.error("got a work group with different numbers of inputs and outputs.")
         if isinstance(v, list) and len(v) != n:
             parser.error("got a work group with different numbers of inputs and outputs.")
         if isinstance(o, list) and len(o) != n:
             parser.error("got a work group with different numbers of inputs and outputs.")
 
-    work : list[BaguetteRack] = []
+    work : list[tuple[BaguetteRack, pathlib.Path, pathlib.Path | None, pathlib.Path | None]] = []
 
     def stripname(p : pathlib.Path) -> str:
         """
         Returns the name of the path without the exetension if it has one.
         """
         ext = p.suffix
         if ext:
@@ -438,25 +438,22 @@
         if vgroup == "-":                           # Magic destination:
             vgroup = [None for _ in rgroup]         # To be determined later
         elif isinstance(vgroup, pathlib.Path):      # Folder visual destination
             vgroup = [create_name(pathlib.Path(vgroup, stripname(r) + ".gexf")) for r in rgroup]       # Pre-compute the visual paths with report names
         
         for r, b, v, o in zip(rgroup, bgroup, vgroup, ogroup):
             bg = BaguetteRack(o)
-            bg.report = r
-            bg.baguette = b if b is not None else (bg.working_directory / "baguette.pyt")
-            bg.visual = v if v is not None else (bg.working_directory / "visual.gexf")
             bg.verbosity = verbosity
             bg.skip_data_comparison = args.skip_data_comparison
             bg.skip_diff_comparison = args.skip_diff_comparison
             bg.filter_names = args.filters
             bg.maxtime = args.maxtime
             bg.perf = args.perf
             bg.background_color = args.background
-            work.append(bg)
+            work.append((bg, r, b, v))
     
     
     # Compile now...
 
     from multiprocessing.pool import Pool
     from threading import Lock, Thread
 
@@ -465,28 +462,31 @@
     lock = Lock()
     failed, timed_out, total = 0, 0, len(work)
     def execute_single_job(P : Pool) -> bool:
         nonlocal failed, timed_out
         with lock:
             if not work: 
                 return False
-            br = work.pop()
+            br, r, b, v = work.pop()
         try:
-            br = P.apply(compile, (br, ))
+            br.export()
+            P.apply(compile, (br.index, r, b, v))
+            br = BaguetteRack.import_from(br.index)
         except KeyboardInterrupt as e:
             from traceback import TracebackException
             br.exception = TracebackException.from_exception(e)
-        if br.exception is None or not br.suppressed:
             br.export()
+        if br.suppressed:
+            br.clean()
         if br.exception is not None and issubclass(br.exception.exc_type, KeyboardInterrupt):
             return False
         elif br.exception is not None and not issubclass(br.exception.exc_type, TimeoutExit):
             with lock:
                 failed += 1
-            logger.error("Got a '{}' error during the baking of '{}'.".format(br.exception.exc_type.__name__, br.report.name))
+            logger.error("Got a '{}' error during the baking of '{}'.".format(br.exception.exc_type.__name__, r.name))
         elif br.exception is not None and issubclass(br.exception.exc_type, TimeoutExit):
             with lock:
                 timed_out += 1
         return True
 
     def executor(P : Pool):
         while execute_single_job(P):
```

### Comparing `baguette_verse-1.0.5.2/baguette/bakery/compiler.py` & `baguette_verse-1.0.6/baguette/bakery/compiler.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 """
 This module contains the compile function which is used to bake baguettes.
 """
 
-from ..rack import BaguetteRack
+from pathlib import Path
 
 __all__ = ["compile"]
 
 
 
 
 
-def compile(rack : BaguetteRack) -> BaguetteRack:
+def compile(rack_path : Path, report_path : Path, cp_baguette : Path | None = None, cp_visual : Path | None = None):
 
     """
     Compiles a baguette using the data written in the given BaguetteRack object.
     Returns a BaguetteRack (the same) containing the results (and exceptions on failure).
     """
 
     from ..rack import BaguetteRack, TimeoutExit
+    from pickle import dump
+
+    rack = BaguetteRack.import_from(rack_path)
 
     try:
 
         if rack.baked:
-            return rack
+            return
         
         import logging
         levels = {
             0 : logging.ERROR,
             1 : logging.WARNING,
             2 : logging.INFO,
             3 : logging.DEBUG
@@ -34,36 +37,41 @@
         
         from ..logger import set_level, logger
         set_level(levels[rack.verbosity])
 
         logger.debug("Just change worker's verbosity level.")
 
         import os
-        from pickle import dump
         from .source.build import Builder
         from .source.config import CompilationParameters, ajust_for_background_color
         from .source import types
         from Viper.better_threading import Future, DaemonThread
 
         if rack.perf:
             from .source.utils import chrono
             chrono.enabled = True
             chrono.auto_report = True
 
-        if not os.path.exists(rack.report):
+        if not os.path.exists(report_path):
             rack.suppressed = True
-            raise FileNotFoundError("Could not find report file: {}".format(rack.report))
-        if not os.path.isfile(rack.report):
+            raise FileNotFoundError("Could not find report file: {}".format(report_path))
+        if not os.path.isfile(report_path):
             rack.suppressed = True
             raise FileExistsError("Given path to report file is not a file.")
         if os.path.exists(rack.baguette) and not os.path.isfile(rack.baguette):
             rack.suppressed = True
+            raise FileExistsError("Baguette output file exists and is not a file.")
+        if cp_baguette is not None and os.path.exists(cp_baguette) and not os.path.isfile(cp_baguette):
+            rack.suppressed = True
             raise FileExistsError("Given baguette output file exists and is not a file.")
         if os.path.exists(rack.visual) and not os.path.isfile(rack.visual):
             rack.suppressed = True
+            raise FileExistsError("Visual output file exists and is not a file.")
+        if cp_visual is not None and os.path.exists(cp_visual) and not os.path.isfile(cp_visual):
+            rack.suppressed = True
             raise FileExistsError("Given visual output file exists and is not a file.")
 
         if rack.skip_data_comparison:
             CompilationParameters.SkipLevenshteinForDataNodes = True
         if rack.skip_diff_comparison:
             CompilationParameters.SkipLevenshteinForDiffNodes = True
 
@@ -71,15 +79,15 @@
 
         def compile_main():
             
             try:
                 logger.info("Loading file...")
                 from json import JSONDecodeError
                 try:
-                    with rack.report.open("r") as file:
+                    with report_path.open("r") as file:
                         b = Builder(file)
                 except JSONDecodeError:
                     rack.suppressed = True
                     raise
                 logger.info("Checking color settings...")
                 ajust_for_background_color(rack.background_color)
                 logger.info("Building graph...")
@@ -87,22 +95,30 @@
                 G = b.graph
                 logger.info("Analyzing graph...")
                 logger.info("Got {} vertices and {} edges.".format(G.n, G.m))
                 logger.info("Saving with pickle")
                 rack.baguette.parent.mkdir(parents = True, exist_ok = True)
                 with rack.baguette.open("wb") as file:
                     dump(G, file)
+                if cp_baguette is not None:
+                    from shutil import copyfile
+                    cp_baguette.parent.mkdir(parents=True, exist_ok=True)
+                    copyfile(rack.baguette, cp_baguette)
                 filters = rack.filters
                 if filters:
                     for i, (f, name) in enumerate(zip(filters, rack.filter_names)):
                         logger.info("Applying filters {}/{} : {}".format(i + 1, len(filters), name))
                         f.apply(G)
                 logger.info("Exporting to .gexf")
                 rack.visual.parent.mkdir(parents = True, exist_ok = True)
                 G.export(str(rack.visual))
+                if cp_visual is not None:
+                    from shutil import copyfile
+                    cp_visual.parent.mkdir(parents=True, exist_ok=True)
+                    copyfile(rack.visual, cp_visual)
                 result.set(True)
                 logger.info("Done !")
             except BaseException as e:
                 result.set_exception(e)
 
         def death_timer():
             from time import sleep
@@ -129,14 +145,14 @@
         from traceback import print_exc, TracebackException
         rack.exception = TracebackException.from_exception(e)
         if not isinstance(e, (KeyboardInterrupt, TimeoutExit)):
             print_exc()
     finally:
         if rack.exception is None or not issubclass(rack.exception.exc_type, (KeyboardInterrupt, TimeoutExit)):
             rack.baked = True
-        return rack
+        rack.export()
 
 
 
 
 
-del BaguetteRack
+del Path
```

### Comparing `baguette_verse-1.0.5.2/baguette/bakery/source/build.py` & `baguette_verse-1.0.6/baguette/bakery/source/build.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.2/baguette/bakery/source/colors.py` & `baguette_verse-1.0.6/baguette/bakery/source/colors.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.2/baguette/bakery/source/config.py` & `baguette_verse-1.0.6/baguette/bakery/source/config.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.2/baguette/bakery/source/event.py` & `baguette_verse-1.0.6/baguette/bakery/source/event.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.2/baguette/bakery/source/filters.py` & `baguette_verse-1.0.6/baguette/bakery/source/filters.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.2/baguette/bakery/source/graph.py` & `baguette_verse-1.0.6/baguette/bakery/source/graph.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.2/baguette/bakery/source/record.py` & `baguette_verse-1.0.6/baguette/bakery/source/record.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.2/baguette/bakery/source/utils.py` & `baguette_verse-1.0.6/baguette/bakery/source/utils.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.2/baguette/bakery/source/types/__init__.py` & `baguette_verse-1.0.6/baguette/bakery/source/types/__init__.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.2/baguette/bakery/source/types/utils.py` & `baguette_verse-1.0.6/baguette/bakery/source/types/utils.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.2/baguette/bakery/source/types/data/entities.py` & `baguette_verse-1.0.6/baguette/bakery/source/types/data/entities.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.2/baguette/bakery/source/types/data/integration.py` & `baguette_verse-1.0.6/baguette/bakery/source/types/data/integration.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.2/baguette/bakery/source/types/data/relations.py` & `baguette_verse-1.0.6/baguette/bakery/source/types/data/relations.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.2/baguette/bakery/source/types/data/utils.py` & `baguette_verse-1.0.6/baguette/bakery/source/types/data/utils.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.2/baguette/bakery/source/types/execution/entities.py` & `baguette_verse-1.0.6/baguette/bakery/source/types/execution/entities.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.2/baguette/bakery/source/types/execution/integration.py` & `baguette_verse-1.0.6/baguette/bakery/source/types/execution/integration.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.2/baguette/bakery/source/types/execution/relations.py` & `baguette_verse-1.0.6/baguette/bakery/source/types/execution/relations.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.2/baguette/bakery/source/types/execution/utils.py` & `baguette_verse-1.0.6/baguette/bakery/source/types/execution/utils.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.2/baguette/bakery/source/types/filesystem/entities.py` & `baguette_verse-1.0.6/baguette/bakery/source/types/filesystem/entities.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.2/baguette/bakery/source/types/filesystem/integration.py` & `baguette_verse-1.0.6/baguette/bakery/source/types/filesystem/integration.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.2/baguette/bakery/source/types/filesystem/relations.py` & `baguette_verse-1.0.6/baguette/bakery/source/types/filesystem/relations.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.2/baguette/bakery/source/types/imports/entities.py` & `baguette_verse-1.0.6/baguette/bakery/source/types/imports/entities.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.2/baguette/bakery/source/types/imports/integration.py` & `baguette_verse-1.0.6/baguette/bakery/source/types/imports/integration.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.2/baguette/bakery/source/types/imports/relations.py` & `baguette_verse-1.0.6/baguette/bakery/source/types/imports/relations.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.2/baguette/bakery/source/types/network/entities.py` & `baguette_verse-1.0.6/baguette/bakery/source/types/network/entities.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.2/baguette/bakery/source/types/network/integration.py` & `baguette_verse-1.0.6/baguette/bakery/source/types/network/integration.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.2/baguette/bakery/source/types/network/relations.py` & `baguette_verse-1.0.6/baguette/bakery/source/types/network/relations.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.2/baguette/bakery/source/types/registry/entities.py` & `baguette_verse-1.0.6/baguette/bakery/source/types/registry/entities.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.2/baguette/bakery/source/types/registry/integration.py` & `baguette_verse-1.0.6/baguette/bakery/source/types/registry/integration.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.2/baguette/bakery/source/types/registry/relations.py` & `baguette_verse-1.0.6/baguette/bakery/source/types/registry/relations.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.2/baguette/croutons/extractor.py` & `baguette_verse-1.0.6/baguette/croutons/extractor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 """
 This module contains the extract function which is used to toast baguettes.
 """
 
-from ..rack import BaguetteRack
+from pathlib import Path
 
 __all__ = ["extract"]
 
 
 
 
 
-def extract(rack : BaguetteRack) -> BaguetteRack:
+def extract(rack_path : Path, cp_extracted : Path | None = None):
 
     """
     Extracts patterns in a baguette using the data written in the given BaguetteRack object.
     Returns a BaguetteRack (the same) containing the results (and exceptions on failure).
     """
 
     from ..rack import BaguetteRack, TimeoutExit
 
+    rack = BaguetteRack.import_from(rack_path)
+
     try:
 
         if rack.toasted:
-            return rack
+            return
         
         import logging
         levels = {
             0 : logging.ERROR,
             1 : logging.WARNING,
             2 : logging.INFO,
             3 : logging.DEBUG
@@ -44,19 +46,21 @@
 
         if rack.perf:
             from ..bakery.source.utils import chrono
             chrono.enabled = True
             chrono.auto_report = True
 
         if not os.path.exists(rack.baguette):
-            raise FileNotFoundError("Could not find baguette file: {}".format(rack.report))
+            raise FileNotFoundError("Could not find baguette file: {}".format(rack.baguette))
         if not os.path.isfile(rack.baguette):
             raise FileExistsError("Given path to baguette file is not a file.")
-        if os.path.exists(rack.extracted) and not os.path.isfile(rack.extracted):
+        if cp_extracted is not None and os.path.exists(cp_extracted) and not os.path.isfile(cp_extracted):
             raise FileExistsError("Given baguette extraction file exists and is not a file.")
+        if os.path.exists(rack.extracted) and not os.path.isfile(rack.extracted):
+            raise FileExistsError("Baguette extraction file exists and is not a file.")
 
         result : Future[bool] = Future()
 
         def extract_main():
             
             try:
                 logger.info("Loading baguette...")
@@ -85,14 +89,18 @@
                     if l:
                         matches[name] = l
 
                 logger.info("Exporting {} matches to file '{}'...".format(sum(len(l) for l in matches.values()), rack.extracted))
                 rack.extracted.parent.mkdir(parents = True, exist_ok = True)
                 with open(rack.extracted, "wb") as file:
                     dump(matches, file)
+                if cp_extracted is not None:
+                    from shutil import copyfile
+                    cp_extracted.parent.mkdir(parents=True, exist_ok=True)
+                    copyfile(rack.extracted, cp_extracted)
 
                 if matches and rack.paint_color:
                     logger.info("Exporting visual with colors")
                     for i, (f, name) in enumerate(zip(rack.filters, rack.filter_names)):
                         logger.info("Applying filters {}/{} : {}".format(i + 1, len(rack.filters), name))
                         f.apply(b)
                     logger.info("Exporting to .gexf")
@@ -129,14 +137,14 @@
         from traceback import print_exc, TracebackException
         rack.exception = TracebackException.from_exception(e)
         if not isinstance(e, (KeyboardInterrupt, TimeoutExit)):
             print_exc()
     finally:
         if rack.exception is None or not issubclass(rack.exception.exc_type, (KeyboardInterrupt, TimeoutExit)):
             rack.toasted = True
-        return rack
+        rack.export()
 
 
 
 
 
-del BaguetteRack
+del Path
```

### Comparing `baguette_verse-1.0.5.2/baguette/croutons/toast.py` & `baguette_verse-1.0.6/baguette/croutons/toast.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
                 r, g, b = int(r, 16), int(g, 16), int(b, 16)
             else:
                 parser.error(f"could not understand color format : '{c}'")
 
             return Color(r, g, b)
 
     parser.add_argument("inputs", type=PathSorter(inputs, "input"), default=None, nargs="*" if ("BAGUETTE_INPUTS" in environ or "BAGUETTE_OUTPUTS" in environ) else "+", help="Baguette folders. These should contain the index file resulting from the baking. Can also be folders baguette folders. Defaults to environment variable 'BAGUETTE_INPUTS' (or 'BAGUETTE_OUTPUTS') if set.")
-    parser.add_argument("--extracted", type=PathSorter(extracted, "extracted"), default=None, action="extend", nargs="*", help="the path(s) to the output extracted match files (.pyt). Use '-' to leave it to the automatic destination. Defaults to environment variable 'BAGUETTE_EXTRACTED' or '-' if not set.")
+    parser.add_argument("--extracted", type=PathSorter(extracted, "extracted"), default=None, action="extend", nargs="*", help="the path(s) to the output (copy) extracted match files (.pyt). Use '-' to leave it to the automatic destination. Defaults to environment variable 'BAGUETTE_EXTRACTED' or '-' if not set.")
     parser.add_argument("--pool", type=pool_size, default=pool_size("0.5"), help="the size of the process pool to use to bake in parallel.")
     parser.add_argument("--maxtime", type=time, default=time("inf"), help="the maximum amount of time spent baking a single baguette. No maxtime by default.")
     parser.add_argument("-p", "--pattern", type=str, action="extend", choices=["-"] + entries(), nargs="+", help="The metapath names (as in the source.metalib module) to search for. Leave empty or use '-' to search for all defined metagraphs.")
     parser.add_argument("--perf", action="store_true", default=False, help="if this is enabled, a performance report will be printed at the end of the baking process.")
     parser.add_argument("--paint", type=paint_color, nargs="+", default=[], help="If a color is given for painting, the matches found will be painted in the visual.gexf file. Must be a valid color name or RGB values.")
     parser.add_argument("-v", "--verbosity", action="count", default=0, help="increases the verbosity of the output.")
 
@@ -369,15 +369,15 @@
     for i, e in zip(input_groups, extracted_groups):
         if not isinstance(i, list):
             raise RuntimeError("How did we get here?")
         n = len(i)
         if isinstance(e, list) and len(e) != n:
             parser.error("got a work group with different numbers of inputs and outputs.")
 
-    work : list[BaguetteRack] = []
+    work : list[tuple[BaguetteRack, pathlib.Path | None]] = []
 
     def stripname(p : pathlib.Path) -> str:
         """
         Returns the name of the path without the exetension if it has one.
         """
         ext = p.suffix
         if ext:
@@ -399,20 +399,19 @@
         for i, e in zip(igroup, egroup):
             if not (i / "index.pyt").exists():
                 parser.error("baguette folder does not have the appropriate index file : '{}' not found.".format(i / "index.pyt"))
             if not (i / "index.pyt").is_file():
                 parser.error("baguette folder does not have the appropriate index file : '{}' is not a file.".format(i / "index.pyt"))
             bg = BaguetteRack.import_from(i / "index.pyt")
             bg.verbosity = args.verbosity
-            bg.extracted = e if e is not None else bg.working_directory / "extracted.pyt"
             bg.pattern_names = args.pattern
             bg.maxtime = args.maxtime
             bg.perf = args.perf
             bg.paint_color = args.paint
-            work.append(bg)
+            work.append((bg, e))
     
     
     # Extract now...
 
     from multiprocessing.pool import Pool
     from threading import Lock, Thread
 
@@ -421,22 +420,25 @@
     lock = Lock()
     failed, timed_out, total = 0, 0, len(work)
     def execute_single_job(P : Pool) -> bool:
         nonlocal failed, timed_out
         with lock:
             if not work: 
                 return False
-            br = work.pop()
+            br, e = work.pop()
         try:
-            br = P.apply(extract, (br, ))
-        except KeyboardInterrupt as e:
+            br.export()
+            P.apply(extract, (br.index, e))
+            br = br.import_from(br.index)
+        except KeyboardInterrupt as exc:
             from traceback import TracebackException
-            br.exception = TracebackException.from_exception(e)
-        if br.exception is None or not br.suppressed:
+            br.exception = TracebackException.from_exception(exc)
             br.export()
+        if br.suppressed:
+            br.clean()
         if br.exception is not None and issubclass(br.exception.exc_type, KeyboardInterrupt):
             return False
         elif br.exception is not None and not issubclass(br.exception.exc_type, TimeoutExit):
             with lock:
                 failed += 1
             logger.error("Got a '{}' error during the toasting of '{}'.".format(br.exception.exc_type.__name__, br.working_directory.name))
         elif br.exception is not None and issubclass(br.exception.exc_type, TimeoutExit):
```

### Comparing `baguette_verse-1.0.5.2/baguette/croutons/metalib/__init__.py` & `baguette_verse-1.0.6/baguette/croutons/metalib/__init__.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.2/baguette/croutons/metalib/interact.py` & `baguette_verse-1.0.6/baguette/croutons/metalib/interact.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.2/baguette/croutons/metalib/utils.py` & `baguette_verse-1.0.6/baguette/croutons/metalib/utils.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.2/baguette/croutons/source/evaluator.py` & `baguette_verse-1.0.6/baguette/croutons/source/evaluator.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.2/baguette/croutons/source/metagraph.py` & `baguette_verse-1.0.6/baguette/croutons/source/metagraph.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.2/baguette/croutons/source/utils.py` & `baguette_verse-1.0.6/baguette/croutons/source/utils.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.2/baguette/tutorial/data.zip` & `baguette_verse-1.0.6/baguette/tutorial/data.zip`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.2/baguette/tutorial/scripts.py` & `baguette_verse-1.0.6/baguette/tutorial/scripts.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.2/baguette/tutorial/utils.py` & `baguette_verse-1.0.6/baguette/tutorial/utils.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.2/.gitignore` & `baguette_verse-1.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.2/LICENSE` & `baguette_verse-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.2/README.md` & `baguette_verse-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.5.2/pyproject.toml` & `baguette_verse-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "baguette-verse"
-version = "1.0.5.2"
+version = "1.0.6"
 authors = [
   { name="Vincent Raulin", email="vincent.raulin@inria.fr" },
 ]
 description = "A malware behavioral analysis framework centered around BAGUETTE!"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.10"
```

### Comparing `baguette_verse-1.0.5.2/PKG-INFO` & `baguette_verse-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baguette-verse
-Version: 1.0.5.2
+Version: 1.0.6
 Summary: A malware behavioral analysis framework centered around BAGUETTE!
 Project-URL: Repository, https://gitlab.inria.fr/vraulin/baguette-verse
 Project-URL: Bug Tracker, https://gitlab.inria.fr/vraulin/baguette-verse/-/issues
 Author-email: Vincent Raulin <vincent.raulin@inria.fr>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
```

