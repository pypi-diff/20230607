# Comparing `tmp/karp-backend-5-5.26.4.tar.gz` & `tmp/karp-backend-5-5.27.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/karp-backend-5-5.26.4.tar", last modified: Wed Jan 12 08:10:22 2022, max compression
+gzip compressed data, was "karp-backend-5-5.27.5.tar", last modified: Wed Jun  7 08:14:57 2023, max compression
```

## Comparing `karp-backend-5-5.26.4.tar` & `karp-backend-5-5.27.5.tar`

### file list

```diff
@@ -1,241 +1,248 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/
--rw-r--r--   0 runner    (1001) docker     (121)    17930 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (121)    17864 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/data/panacea/
--rw-r--r--   0 runner    (1001) docker     (121)      167 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/data/panacea/PAN_metadata_Glossary DE-EN_prob-Authors.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2067 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/data/panacea/convert_panacea.py
--rw-r--r--   0 runner    (1001) docker     (121)  1823097 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/data/panacea/WP52-LtXfr-ProbLex-deen.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1117 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/data/panacea/readme_bilingual_glossary_prob_DE-EN.txt
--rw-r--r--   0 runner    (1001) docker     (121)   172184 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/data/panacea/Creative Commons — Attri....0 Unported — CC BY 3.pdf
--rw-r--r--   0 runner    (1001) docker     (121)    10468 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/data/panacea/PAN_metadata_Glossary DE-EN_prob.html
--rw-r--r--   0 runner    (1001) docker     (121)  6830756 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/data/panacea/panacea.json
--rw-r--r--   0 runner    (1001) docker     (121)      597 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)     1408 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1545 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/export_bugg.md
--rw-r--r--   0 runner    (1001) docker     (121)      728 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/backend.wsgi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2365 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (121)     3874 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/.github/workflows/build-publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2056 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/config/
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/config/lexiconconf.json.example
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/config/lexiconconf.json.panacea
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/config/mappings/
--rw-r--r--   0 runner    (1001) docker     (121)      355 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/config/mappings/fieldmappings_default.json
--rw-r--r--   0 runner    (1001) docker     (121)     1259 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/config/mappings/mappingconf_panacea.json.panacea
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/config/mappings/README
--rw-r--r--   0 runner    (1001) docker     (121)      310 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/config/mappings/fieldmappings_panacea.json.panacea
--rw-r--r--   0 runner    (1001) docker     (121)      696 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/config/config.json.example
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1376 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/config/modes.json.example
--rw-r--r--   0 runner    (1001) docker     (121)      758 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/config/modes.json.panacea
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp_backend_5.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp_backend_5.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp_backend_5.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp_backend_5.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5376 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp_backend_5.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp_backend_5.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6286 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp_backend_5.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5376 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/doc/
--rw-r--r--   0 runner    (1001) docker     (121)     1164 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/doc/HowToMoveAResource.md
--rw-r--r--   0 runner    (1001) docker     (121)     7546 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/doc/advanced_setup.md
--rw-r--r--   0 runner    (1001) docker     (121)     1544 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/doc/wsauth_manual.md
--rw-r--r--   0 runner    (1001) docker     (121)    22428 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/doc/manual.md
--rw-r--r--   0 runner    (1001) docker     (121)     3062 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/doc/structure.tex
--rw-r--r--   0 runner    (1001) docker     (121)    44172 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/doc/about.tex
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)      507 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/run.py
--rw-r--r--   0 runner    (1001) docker     (121)     2925 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/pyrightconfig.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/
--rw-r--r--   0 runner    (1001) docker     (121)    10043 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/server/
--rw-r--r--   0 runner    (1001) docker     (121)    14100 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/server/update.py
--rw-r--r--   0 runner    (1001) docker     (121)    32868 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/server/searching.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/server/translator/
--rw-r--r--   0 runner    (1001) docker     (121)     2433 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/server/translator/bulkify.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/server/translator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11987 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/server/translator/elasticObjects.py
--rw-r--r--   0 runner    (1001) docker     (121)     3318 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/server/translator/validatejson.py
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/server/translator/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)    30602 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/server/translator/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2179 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/server/idgenerator.py
--rw-r--r--   0 runner    (1001) docker     (121)     3535 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/server/checkdbhistory.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/server/helper/
--rw-r--r--   0 runner    (1001) docker     (121)      575 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/server/helper/jsonwalk.py
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/server/helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6140 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/server/helper/flaskhelper.py
--rw-r--r--   0 runner    (1001) docker     (121)     2083 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/server/helper/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     6250 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/server/suggestions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/document/
--rw-r--r--   0 runner    (1001) docker     (121)     1269 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/document/autoupdates.py
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/document/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2377 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/document/doc_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/context/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/context/auth/
--rw-r--r--   0 runner    (1001) docker     (121)     3137 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/context/auth/std_auth.py
--rw-r--r--   0 runner    (1001) docker     (121)     1270 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/context/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3211 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/context/auth/dummy_auth.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/context/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/application/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/application/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/application/actions/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/application/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      353 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/application/actions/mode_actions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3667 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/html/
--rw-r--r--   0 runner    (1001) docker     (121)    35024 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/html/api.md
--rw-r--r--   0 runner    (1001) docker     (121)    38531 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/html/index_dokumentation.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/config/
--rw-r--r--   0 runner    (1001) docker     (121)    18140 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/config/configmanager.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/config/ext/
--rw-r--r--   0 runner    (1001) docker     (121)      400 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/config/ext/ext_src.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/config/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2106 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/config/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      232 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      340 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/config/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/static/
--rw-r--r--   0 runner    (1001) docker     (121)    37335 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/static/karp.png
--rw-r--r--   0 runner    (1001) docker     (121)     2741 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/static/api.css
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     3760 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)      425 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/instance_info.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/cli/
--rw-r--r--   0 runner    (1001) docker     (121)     2015 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/cli/getmapping.py
--rw-r--r--   0 runner    (1001) docker     (121)     1607 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/cli/create_metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)     8234 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    25017 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/cli/upload_offline.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/util/
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1825 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/util/text.py
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/util/debug.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       97 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/test_index.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/tests/data/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/tests/data/data/large_lex/
--rw-r--r--   0 runner    (1001) docker     (121)  1288892 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/data/data/large_lex/large_lex.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/tests/data/data/panacea/
--rw-r--r--   0 runner    (1001) docker     (121)  6830756 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/data/data/panacea/panacea.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/tests/data/data/foo/
--rw-r--r--   0 runner    (1001) docker     (121)      470 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/data/data/foo/foo.json
--rw-r--r--   0 runner    (1001) docker     (121)      287 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/data/data/foo/bar.json
--rw-r--r--   0 runner    (1001) docker     (121)      194 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/data/data/custom_path_bar.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/tests/data/config/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/tests/data/config/mappings/
--rw-r--r--   0 runner    (1001) docker     (121)      604 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/data/config/mappings/mappingconf_foo.json
--rw-r--r--   0 runner    (1001) docker     (121)     1259 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/data/config/mappings/mappingconf_panacea.json
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/data/config/mappings/fieldmappings_foo.json
--rw-r--r--   0 runner    (1001) docker     (121)      355 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/data/config/mappings/fieldmappings_default.json
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/data/config/mappings/README
--rw-r--r--   0 runner    (1001) docker     (121)      421 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/data/config/mappings/mappingconf_large_lex.json
--rw-r--r--   0 runner    (1001) docker     (121)      310 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/data/config/mappings/fieldmappings_panacea.json
--rw-r--r--   0 runner    (1001) docker     (121)      310 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/data/config/mappings/fieldmappings_panacea_links.json
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/data/config/mappings/fieldmappings_large_lex.json
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/data/config/mappings/fieldmappings_bar.json
--rw-r--r--   0 runner    (1001) docker     (121)     1259 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/data/config/mappings/mappingconf_panacea_links.json
--rw-r--r--   0 runner    (1001) docker     (121)      698 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/data/config/config.json
--rw-r--r--   0 runner    (1001) docker     (121)     2485 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/data/config/modes.json
--rw-r--r--   0 runner    (1001) docker     (121)      762 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/data/config/lexiconconf.json
--rw-r--r--   0 runner    (1001) docker     (121)     1171 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (121)     1639 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/auth_server.py
--rw-r--r--   0 runner    (1001) docker     (121)     1097 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/test_update_index.py
--rw-r--r--   0 runner    (1001) docker     (121)     2978 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/common_fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/tests/api/
--rw-r--r--   0 runner    (1001) docker     (121)      140 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/api/test_logout.py
--rw-r--r--   0 runner    (1001) docker     (121)      718 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/api/test_autocomplete.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/tests/api/search/
--rw-r--r--   0 runner    (1001) docker     (121)     1638 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/api/search/test_search.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/api/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2056 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/api/search/test_pagination.py
--rw-r--r--   0 runner    (1001) docker     (121)     2109 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/api/search/test_stats.py
--rw-r--r--   0 runner    (1001) docker     (121)     1106 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/api/test_explain.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/tests/api/config/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/api/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      383 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/api/config/test_routes.py
--rw-r--r--   0 runner    (1001) docker     (121)     4689 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/api/test_history.py
--rw-r--r--   0 runner    (1001) docker     (121)      800 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/api/test_export.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/api/test_suggestion.py
--rw-r--r--   0 runner    (1001) docker     (121)      551 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/_test_config.py
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/test_modes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (121)     2804 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/cli/test_es.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      286 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/cli/test_recover.py
--rw-r--r--   0 runner    (1001) docker     (121)     7768 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/cli/test_upload.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/tests/integration_tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/tests/integration_tests/server/
--rw-r--r--   0 runner    (1001) docker     (121)     9519 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/integration_tests/server/test_searching_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/tests/integration_tests/server/translator/
--rw-r--r--   0 runner    (1001) docker     (121)     1087 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/integration_tests/server/translator/test_validatejson_on_panacea.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/integration_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/tests/integration_tests/domain/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/tests/integration_tests/domain/services/
--rw-r--r--   0 runner    (1001) docker     (121)      887 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/integration_tests/domain/services/test_search_service_it.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/tests/parser/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/parser/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     2917 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/tests/unit_tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/tests/unit_tests/server/
--rw-r--r--   0 runner    (1001) docker     (121)     7216 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/unit_tests/server/test_searching.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/tests/unit_tests/server/translator/
--rw-r--r--   0 runner    (1001) docker     (121)     6358 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/unit_tests/server/translator/test_parser_statistics.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/unit_tests/server/translator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2149 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/unit_tests/server/translator/test_parser_freetext.py
--rw-r--r--   0 runner    (1001) docker     (121)     1780 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/unit_tests/server/translator/test_validatejson.py
--rw-r--r--   0 runner    (1001) docker     (121)    11021 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/unit_tests/server/translator/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     5254 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/unit_tests/server/translator/test_parser_search.py
--rw-r--r--   0 runner    (1001) docker     (121)     1218 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/unit_tests/server/test_statlist.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/tests/unit_tests/context/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/tests/unit_tests/context/auth/
--rw-r--r--   0 runner    (1001) docker     (121)     3880 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/unit_tests/context/auth/test_std_auth.py
--rw-r--r--   0 runner    (1001) docker     (121)     4004 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/unit_tests/context/auth/test_dummy_auth.py
--rw-r--r--   0 runner    (1001) docker     (121)     1165 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/unit_tests/context/auth/test_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/tests/unit_tests/application/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/tests/unit_tests/application/actions/
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/unit_tests/application/actions/test_mode_actions.py
--rw-r--r--   0 runner    (1001) docker     (121)      268 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/unit_tests/test_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/tests/unit_tests/config/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/unit_tests/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2694 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/unit_tests/config/test_configmanager.py
--rw-r--r--   0 runner    (1001) docker     (121)      860 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/unit_tests/config/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     2283 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/unit_tests/test_errors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/tests/unit_tests/domain/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/tests/unit_tests/domain/services/
--rw-r--r--   0 runner    (1001) docker     (121)     2502 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/unit_tests/domain/services/test_search_service.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/unit_tests/domain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/tests/unit_tests/domain/model/
--rw-r--r--   0 runner    (1001) docker     (121)      230 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/unit_tests/domain/model/test_user.py
--rw-r--r--   0 runner    (1001) docker     (121)     5770 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/unit_tests/domain/model/test_mode.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/unit_tests/domain/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/tests/unit_tests/dbhandler/
--rw-r--r--   0 runner    (1001) docker     (121)     1353 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/unit_tests/dbhandler/test_dbhandler.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/tests/unit_tests/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (121)      425 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/tests/unit_tests/infrastructure/test_json_file_mode_respository.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/domain/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/domain/services/
--rw-r--r--   0 runner    (1001) docker     (121)     1867 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/domain/services/search_service.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/domain/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/domain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/domain/model/
--rw-r--r--   0 runner    (1001) docker     (121)      290 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/domain/model/user.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/domain/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1902 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/domain/model/mode.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/dbhandler/
--rw-r--r--   0 runner    (1001) docker     (121)     1676 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/dbhandler/emailsender.py
--rw-r--r--   0 runner    (1001) docker     (121)    16708 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/dbhandler/dbhandler.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/dbhandler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 08:10:22.000000 karp-backend-5-5.26.4/karp5/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (121)      924 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/karp5/infrastructure/json_file_mode_repository.py
--rw-r--r--   0 runner    (1001) docker     (121)      349 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/create_large_lex.py
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      201 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4215 2022-01-12 08:10:11.000000 karp-backend-5-5.26.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.926145 karp-backend-5-5.27.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.890144 karp-backend-5-5.27.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.890144 karp-backend-5-5.27.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/.github/workflows/build-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    17864 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-07 08:14:57.000000 karp-backend-5-5.27.5/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-07 08:14:57.000000 karp-backend-5-5.27.5/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-06-07 08:14:57.926145 karp-backend-5-5.27.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/backend.wsgi
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.890144 karp-backend-5-5.27.5/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/config/config.json.example
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/config/lexiconconf.json.example
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/config/lexiconconf.json.panacea
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.890144 karp-backend-5-5.27.5/config/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/config/mappings/README
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/config/mappings/fieldmappings_default.json
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/config/mappings/fieldmappings_panacea.json.panacea
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/config/mappings/mappingconf_panacea.json.panacea
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/config/modes.json.example
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/config/modes.json.panacea
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/create_large_lex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.882144 karp-backend-5-5.27.5/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.902145 karp-backend-5-5.27.5/data/panacea/
+-rw-r--r--   0 runner    (1001) docker     (123)   172184 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/data/panacea/Creative Commons — Attri....0 Unported — CC BY 3.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/data/panacea/PAN_metadata_Glossary DE-EN_prob-Authors.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10468 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/data/panacea/PAN_metadata_Glossary DE-EN_prob.html
+-rw-r--r--   0 runner    (1001) docker     (123)  1823097 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/data/panacea/WP52-LtXfr-ProbLex-deen.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/data/panacea/convert_panacea.py
+-rw-r--r--   0 runner    (1001) docker     (123)  6830756 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/data/panacea/panacea.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/data/panacea/readme_bilingual_glossary_prob_DE-EN.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.902145 karp-backend-5-5.27.5/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/doc/HowToMoveAResource.md
+-rw-r--r--   0 runner    (1001) docker     (123)    44172 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/doc/about.tex
+-rw-r--r--   0 runner    (1001) docker     (123)     7546 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/doc/advanced_setup.md
+-rw-r--r--   0 runner    (1001) docker     (123)    22428 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/doc/manual.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/doc/structure.tex
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/doc/wsauth_manual.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/export_bugg.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.902145 karp-backend-5-5.27.5/karp5/
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.902145 karp-backend-5-5.27.5/karp5/application/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/application/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.902145 karp-backend-5-5.27.5/karp5/application/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/application/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/application/actions/mode_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10043 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.902145 karp-backend-5-5.27.5/karp5/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     8234 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/cli/create_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/cli/getmapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25017 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/cli/upload_offline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.902145 karp-backend-5-5.27.5/karp5/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18140 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/config/configmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/config/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.906144 karp-backend-5-5.27.5/karp5/config/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/config/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/config/ext/ext_src.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.906144 karp-backend-5-5.27.5/karp5/context/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/context/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.906144 karp-backend-5-5.27.5/karp5/context/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/context/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/context/auth/dummy_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/context/auth/std_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.906144 karp-backend-5-5.27.5/karp5/dbhandler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/dbhandler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16708 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/dbhandler/dbhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/dbhandler/emailsender.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.906144 karp-backend-5-5.27.5/karp5/document/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/document/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/document/autoupdates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/document/doc_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.906144 karp-backend-5-5.27.5/karp5/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/domain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.906144 karp-backend-5-5.27.5/karp5/domain/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/domain/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/domain/model/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/domain/model/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.906144 karp-backend-5-5.27.5/karp5/domain/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/domain/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/domain/services/search_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.906144 karp-backend-5-5.27.5/karp5/html/
+-rw-r--r--   0 runner    (1001) docker     (123)    35024 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/html/api.md
+-rw-r--r--   0 runner    (1001) docker     (123)    38531 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/html/index_dokumentation.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.906144 karp-backend-5-5.27.5/karp5/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/infrastructure/json_file_mode_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/instance_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.906144 karp-backend-5-5.27.5/karp5/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/server/checkdbhistory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/server/extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.906144 karp-backend-5-5.27.5/karp5/server/helper/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/server/helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/server/helper/flaskhelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/server/helper/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/server/helper/jsonwalk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/server/idgenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32868 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/server/searching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/server/suggestions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.910145 karp-backend-5-5.27.5/karp5/server/translator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/server/translator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/server/translator/bulkify.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11987 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/server/translator/elasticObjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/server/translator/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30602 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/server/translator/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/server/translator/validatejson.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14100 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/server/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.910145 karp-backend-5-5.27.5/karp5/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/static/api.css
+-rw-r--r--   0 runner    (1001) docker     (123)    37335 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/static/karp.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.910145 karp-backend-5-5.27.5/karp5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/_test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.910145 karp-backend-5-5.27.5/karp5/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.910145 karp-backend-5-5.27.5/karp5/tests/api/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/api/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/api/config/test_routes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.910145 karp-backend-5-5.27.5/karp5/tests/api/search/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/api/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/api/search/test_pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/api/search/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/api/search/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/api/test_autocomplete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/api/test_explain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/api/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/api/test_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/api/test_logout.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/api/test_suggestion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/auth_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.914145 karp-backend-5-5.27.5/karp5/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/cli/test_es.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/cli/test_recover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/cli/test_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/common_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.886144 karp-backend-5-5.27.5/karp5/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.914145 karp-backend-5-5.27.5/karp5/tests/data/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/data/config/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/data/config/lexiconconf.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.914145 karp-backend-5-5.27.5/karp5/tests/data/config/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/data/config/mappings/README
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/data/config/mappings/fieldmappings_bar.json
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/data/config/mappings/fieldmappings_default.json
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/data/config/mappings/fieldmappings_foo.json
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/data/config/mappings/fieldmappings_large_lex.json
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/data/config/mappings/fieldmappings_panacea.json
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/data/config/mappings/fieldmappings_panacea_links.json
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/data/config/mappings/mappingconf_foo.json
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/data/config/mappings/mappingconf_large_lex.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/data/config/mappings/mappingconf_panacea.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/data/config/mappings/mappingconf_panacea_links.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/data/config/modes.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.914145 karp-backend-5-5.27.5/karp5/tests/data/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/data/data/custom_path_bar.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.914145 karp-backend-5-5.27.5/karp5/tests/data/data/foo/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/data/data/foo/bar.json
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/data/data/foo/foo.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.914145 karp-backend-5-5.27.5/karp5/tests/data/data/large_lex/
+-rw-r--r--   0 runner    (1001) docker     (123)  1288892 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/data/data/large_lex/large_lex.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.914145 karp-backend-5-5.27.5/karp5/tests/data/data/panacea/
+-rw-r--r--   0 runner    (1001) docker     (123)  6830756 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/data/data/panacea/panacea.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.922145 karp-backend-5-5.27.5/karp5/tests/integration_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/integration_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.886144 karp-backend-5-5.27.5/karp5/tests/integration_tests/domain/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.922145 karp-backend-5-5.27.5/karp5/tests/integration_tests/domain/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/integration_tests/domain/services/test_search_service_it.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.922145 karp-backend-5-5.27.5/karp5/tests/integration_tests/server/
+-rw-r--r--   0 runner    (1001) docker     (123)     9519 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/integration_tests/server/test_searching_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.922145 karp-backend-5-5.27.5/karp5/tests/integration_tests/server/translator/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/integration_tests/server/translator/test_validatejson_on_panacea.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.922145 karp-backend-5-5.27.5/karp5/tests/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/parser/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/test_modes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/test_update_index.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.922145 karp-backend-5-5.27.5/karp5/tests/unit_tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.886144 karp-backend-5-5.27.5/karp5/tests/unit_tests/application/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.922145 karp-backend-5-5.27.5/karp5/tests/unit_tests/application/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/unit_tests/application/actions/test_mode_actions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.922145 karp-backend-5-5.27.5/karp5/tests/unit_tests/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/unit_tests/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/unit_tests/config/test_configmanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/unit_tests/config/test_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.886144 karp-backend-5-5.27.5/karp5/tests/unit_tests/context/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.926145 karp-backend-5-5.27.5/karp5/tests/unit_tests/context/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/unit_tests/context/auth/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/unit_tests/context/auth/test_dummy_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/unit_tests/context/auth/test_std_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.926145 karp-backend-5-5.27.5/karp5/tests/unit_tests/dbhandler/
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/unit_tests/dbhandler/test_dbhandler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.926145 karp-backend-5-5.27.5/karp5/tests/unit_tests/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/unit_tests/domain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.926145 karp-backend-5-5.27.5/karp5/tests/unit_tests/domain/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/unit_tests/domain/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5770 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/unit_tests/domain/model/test_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/unit_tests/domain/model/test_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.926145 karp-backend-5-5.27.5/karp5/tests/unit_tests/domain/services/
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/unit_tests/domain/services/test_search_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.926145 karp-backend-5-5.27.5/karp5/tests/unit_tests/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/unit_tests/infrastructure/test_json_file_mode_respository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.926145 karp-backend-5-5.27.5/karp5/tests/unit_tests/server/
+-rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/unit_tests/server/test_searching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/unit_tests/server/test_statlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.926145 karp-backend-5-5.27.5/karp5/tests/unit_tests/server/translator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/unit_tests/server/translator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11021 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/unit_tests/server/translator/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/unit_tests/server/translator/test_parser_freetext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/unit_tests/server/translator/test_parser_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/unit_tests/server/translator/test_parser_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/unit_tests/server/translator/test_validatejson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/unit_tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/unit_tests/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/tests/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.926145 karp-backend-5-5.27.5/karp5/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/util/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/karp5/util/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 08:14:57.926145 karp-backend-5-5.27.5/karp_backend_5.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-06-07 08:14:57.000000 karp-backend-5-5.27.5/karp_backend_5.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-06-07 08:14:57.000000 karp-backend-5-5.27.5/karp_backend_5.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 08:14:57.000000 karp-backend-5-5.27.5/karp_backend_5.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 08:14:57.000000 karp-backend-5-5.27.5/karp_backend_5.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-07 08:14:57.000000 karp-backend-5-5.27.5/karp_backend_5.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-07 08:14:57.000000 karp-backend-5-5.27.5/karp_backend_5.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-07 08:14:57.000000 karp-backend-5-5.27.5/karp_backend_5.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/pyrightconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-07 08:14:57.930145 karp-backend-5-5.27.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-07 08:14:49.000000 karp-backend-5-5.27.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `karp-backend-5-5.26.4/.pylintrc` & `karp-backend-5-5.27.5/.pylintrc`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/data/panacea/convert_panacea.py` & `karp-backend-5-5.27.5/data/panacea/convert_panacea.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/data/panacea/WP52-LtXfr-ProbLex-deen.txt` & `karp-backend-5-5.27.5/data/panacea/WP52-LtXfr-ProbLex-deen.txt`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/data/panacea/readme_bilingual_glossary_prob_DE-EN.txt` & `karp-backend-5-5.27.5/data/panacea/readme_bilingual_glossary_prob_DE-EN.txt`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/data/panacea/Creative Commons — Attri....0 Unported — CC BY 3.pdf` & `karp-backend-5-5.27.5/data/panacea/Creative Commons — Attri....0 Unported — CC BY 3.pdf`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/data/panacea/PAN_metadata_Glossary DE-EN_prob.html` & `karp-backend-5-5.27.5/data/panacea/PAN_metadata_Glossary DE-EN_prob.html`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/data/panacea/panacea.json` & `karp-backend-5-5.27.5/data/panacea/panacea.json`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/setup.cfg` & `karp-backend-5-5.27.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/export_bugg.md` & `karp-backend-5-5.27.5/export_bugg.md`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/backend.wsgi` & `karp-backend-5-5.27.5/backend.wsgi`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/.github/workflows/codeql-analysis.yml` & `karp-backend-5-5.27.5/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/.github/workflows/build-publish.yml` & `karp-backend-5-5.27.5/.github/workflows/build-publish.yml`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
           MYSQL_PASSWORD: testing
           MYSQL_USER: karp
         options: --health-cmd "mysqladmin ping" --health-interval 10s --health-timeout 5s --health-retries 10
 
     strategy:
       max-parallel: 4
       matrix:
-        python-version: [3.6, 3.7, 3.8]
+        python-version: [ "3.8"]
         es-version: ["6.8.6"]
         # es-version: ["6.2.4", "6.5.4", "6.8.6"]
     steps:
       - uses: actions/checkout@v1
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v1
         with:
@@ -72,40 +72,45 @@
       - name: Test with pytest
         run: |
           echo "KARP5_DBPASS=${KARP5_DBPASS}"
           make test-w-coverage
           docker logs "${{ job.services.mysql.id }}"
         env:
           KARP5_DBPASS: karp:testing@127.0.0.1:${{ job.services.mysql.ports['3306'] }}
+      - name: Upload coverage to Codecov
+        uses: codecov/codecov-action@v2
+        with:
+          fail_ci_if_error: true
+          verbose: true
       # - name: Coveralls
       #   uses: coverallsapp/github-action@master
       #   with:
       #     github-token: ${{ secrets.github_token }}
   publish:
     needs: build
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v1
-      - name: Set up Python 3.6
+      - name: Set up Python 3.8
         uses: actions/setup-python@v1
         with:
-          python-version: 3.6
+          python-version: 3.8
       - name: Build distribution
         run: |
           pip install --upgrade setuptools twine wheel pbr
           python setup.py sdist bdist_wheel
           echo "github.ref = ${{ github.ref }}"
       - name: Check distributions
         run: twine check dist/*
-      - name: Publish package to TestPyPI
-        uses: pypa/gh-action-pypi-publish@master
-        if: github.repository == 'spraakbanken/karp-backend-v5' && !startsWith(github.ref, 'refs/tags/')
-        with:
-          user: __token__
-          password: ${{ secrets.test_pypi_password }}
-          repository_url: https://test.pypi.org/legacy/
-      - name: Publish package to PyPI
-        uses: pypa/gh-action-pypi-publish@master
-        if: github.repository == 'spraakbanken/karp-backend-v5' && startsWith(github.ref, 'refs/tags/')
-        with:
-          user: __token__
-          password: ${{ secrets.pypi_password }}
+      # - name: Publish package to TestPyPI
+      #   uses: pypa/gh-action-pypi-publish@master
+      #   if: github.repository == 'spraakbanken/karp-backend-v5' && !startsWith(github.ref, 'refs/tags/')
+      #   with:
+      #     user: __token__
+      #     password: ${{ secrets.test_pypi_password }}
+      #     repository_url: https://test.pypi.org/legacy/
+      # - name: Publish package to PyPI
+      #   uses: pypa/gh-action-pypi-publish@master
+      #   if: github.repository == 'spraakbanken/karp-backend-v5' && startsWith(github.ref, 'refs/tags/')
+      #   with:
+      #     user: __token__
+      #     password: ${{ secrets.pypi_password }}
```

### Comparing `karp-backend-5-5.26.4/.github/workflows/build.yml` & `karp-backend-5-5.27.5/.github/workflows/build.yml`

 * *Files 7% similar despite different names*

```diff
@@ -21,16 +21,17 @@
           MYSQL_DATABASE: karp
           MYSQL_PASSWORD: testing
           MYSQL_USER: karp
         options: --health-cmd "mysqladmin ping" --health-interval 10s --health-timeout 5s --health-retries 10
 
     strategy:
       max-parallel: 4
+      fail-fast: false
       matrix:
-        python-version: [3.6, 3.7, 3.8]
+        python-version: [3.8]
         es-version: ["6.8.6"]
     steps:
       - uses: actions/checkout@v1
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v1
         with:
           python-version: ${{ matrix.python-version }}
@@ -53,15 +54,20 @@
         run: make lint-no-fail
       # - name: Typecheck with pytype
       #   if: matrix.python-version != '3.8'
       #   run: make type-check
       - name: Test with pytest
         run: |
           echo "KARP5_DBPASS=${KARP5_DBPASS}"
-          make test-w-coverage
+          make test-w-coverage cov_report=xml
           docker logs "${{ job.services.mysql.id }}"
         env:
           KARP5_DBPASS: karp:testing@127.0.0.1:${{ job.services.mysql.ports['3306'] }}
+      - name: Upload coverage to Codecov
+        uses: codecov/codecov-action@v3
+        with:
+          fail_ci_if_error: false
+          verbose: true
       # - name: Coveralls
       #   uses: coverallsapp/github-action@master
       #   with:
       #     github-token: ${{ secrets.github_token }}
```

### Comparing `karp-backend-5-5.26.4/LICENSE` & `karp-backend-5-5.27.5/LICENSE`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/config/mappings/mappingconf_panacea.json.panacea` & `karp-backend-5-5.27.5/config/mappings/mappingconf_panacea.json.panacea`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/config/config.json.example` & `karp-backend-5-5.27.5/config/config.json.example`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/config/modes.json.example` & `karp-backend-5-5.27.5/config/modes.json.example`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/config/modes.json.panacea` & `karp-backend-5-5.27.5/config/modes.json.panacea`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp_backend_5.egg-info/PKG-INFO` & `karp-backend-5-5.27.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: karp-backend-5
-Version: 5.26.4
+Version: 5.27.5
 Summary: Backend for Karp
 Home-page: https://github.com/spraakbanken/karp-backend-v5
 Author: Språkbanken at the University of Gothenburg
 Author-email: sb-info@svenska.gu.se
 Maintainer: Språkbanken
 Maintainer-email: sb-info@svenska.gu.se
 License: MIT
 Project-URL: Bug Tracker, https://github.com/spraakbanken/karp-backend-v5/issues
 Project-URL: Source Code, https://github.com/spraakbanken/karp-backend-v5
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -33,16 +32,14 @@
 **This package is the legacy version of Karp, [go here for the current version(https://github.com/spraakbanken/karp-backend)]**
 
 ## master
 
 [![codecov](https://codecov.io/gh/spraakbanken/karp-backend-v5/branch/master/graph/badge.svg)](https://codecov.io/gh/spraakbanken/karp-backend-v5)
 [![](https://github.com/spraakbanken/karp-backend-v5/workflows/Build/badge.svg)](https://github.com/spraakbanken/karp-backend-v5/actions)
 
-**This package - code and documentation - is still under construction.**
-
 Karp is the lexical platform of Språkbanken.
 Now migrated to Python 3.6+.
 
 # Karp in Docker
 
 For easy testing, use [Docker](https://docs.docker.com/engine/installation/) to run Karp-b.
 
@@ -117,9 +114,7 @@
 
 - Check if any index is locked: `curl <host>:<port>/_all/_settings/index.blocks*`
   - If all is open, Elasticsearch answers with `{}`
   - else it answers with `{<index>: { "settings": { "index": { "blocks": {"read_only_allow_delete": "true"} } } }, ... }`
 - To unlock all locked indices on a `host` and `port`:
   - `curl -X PUT <host>:<port>/_all/_settings -H 'Content-Type: application' -d '{"index.blocks.read_only_allow_delete": null}'`
 
-
-
```

### Comparing `karp-backend-5-5.26.4/karp_backend_5.egg-info/SOURCES.txt` & `karp-backend-5-5.27.5/karp_backend_5.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 .bumpversion.cfg
+.coveragerc
 .pylintrc
 AUTHORS
 ChangeLog
 LICENSE
 Makefile
 README.md
 backend.wsgi
 cli.py
+codecov.yml
 create_large_lex.py
 export_bugg.md
+pyproject.toml
 pyrightconfig.json
 requirements.txt
 run.py
 setup.cfg
 setup.py
+.github/dependabot.yml
 .github/workflows/build-publish.yml
 .github/workflows/build.yml
+.github/workflows/ci.yml
 .github/workflows/codeql-analysis.yml
 config/__init__.py
 config/config.json.example
 config/lexiconconf.json.example
 config/lexiconconf.json.panacea
 config/modes.json.example
 config/modes.json.panacea
@@ -75,14 +80,15 @@
 karp5/domain/services/__init__.py
 karp5/domain/services/search_service.py
 karp5/html/api.md
 karp5/html/index_dokumentation.html
 karp5/infrastructure/json_file_mode_repository.py
 karp5/server/__init__.py
 karp5/server/checkdbhistory.py
+karp5/server/extensions.py
 karp5/server/idgenerator.py
 karp5/server/searching.py
 karp5/server/suggestions.py
 karp5/server/update.py
 karp5/server/helper/__init__.py
 karp5/server/helper/flaskhelper.py
 karp5/server/helper/helpers.py
@@ -172,9 +178,10 @@
 karp5/util/__init__.py
 karp5/util/debug.py
 karp5/util/text.py
 karp_backend_5.egg-info/PKG-INFO
 karp_backend_5.egg-info/SOURCES.txt
 karp_backend_5.egg-info/dependency_links.txt
 karp_backend_5.egg-info/not-zip-safe
+karp_backend_5.egg-info/pbr.json
 karp_backend_5.egg-info/requires.txt
 karp_backend_5.egg-info/top_level.txt
```

### Comparing `karp-backend-5-5.26.4/PKG-INFO` & `karp-backend-5-5.27.5/karp_backend_5.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: karp-backend-5
-Version: 5.26.4
+Version: 5.27.5
 Summary: Backend for Karp
 Home-page: https://github.com/spraakbanken/karp-backend-v5
 Author: Språkbanken at the University of Gothenburg
 Author-email: sb-info@svenska.gu.se
 Maintainer: Språkbanken
 Maintainer-email: sb-info@svenska.gu.se
 License: MIT
 Project-URL: Bug Tracker, https://github.com/spraakbanken/karp-backend-v5/issues
 Project-URL: Source Code, https://github.com/spraakbanken/karp-backend-v5
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -33,16 +32,14 @@
 **This package is the legacy version of Karp, [go here for the current version(https://github.com/spraakbanken/karp-backend)]**
 
 ## master
 
 [![codecov](https://codecov.io/gh/spraakbanken/karp-backend-v5/branch/master/graph/badge.svg)](https://codecov.io/gh/spraakbanken/karp-backend-v5)
 [![](https://github.com/spraakbanken/karp-backend-v5/workflows/Build/badge.svg)](https://github.com/spraakbanken/karp-backend-v5/actions)
 
-**This package - code and documentation - is still under construction.**
-
 Karp is the lexical platform of Språkbanken.
 Now migrated to Python 3.6+.
 
 # Karp in Docker
 
 For easy testing, use [Docker](https://docs.docker.com/engine/installation/) to run Karp-b.
 
@@ -117,9 +114,7 @@
 
 - Check if any index is locked: `curl <host>:<port>/_all/_settings/index.blocks*`
   - If all is open, Elasticsearch answers with `{}`
   - else it answers with `{<index>: { "settings": { "index": { "blocks": {"read_only_allow_delete": "true"} } } }, ... }`
 - To unlock all locked indices on a `host` and `port`:
   - `curl -X PUT <host>:<port>/_all/_settings -H 'Content-Type: application' -d '{"index.blocks.read_only_allow_delete": null}'`
 
-
-
```

### Comparing `karp-backend-5-5.26.4/doc/HowToMoveAResource.md` & `karp-backend-5-5.27.5/doc/HowToMoveAResource.md`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/doc/advanced_setup.md` & `karp-backend-5-5.27.5/doc/advanced_setup.md`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/doc/wsauth_manual.md` & `karp-backend-5-5.27.5/doc/wsauth_manual.md`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/doc/manual.md` & `karp-backend-5-5.27.5/doc/manual.md`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/doc/structure.tex` & `karp-backend-5-5.27.5/doc/structure.tex`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/doc/about.tex` & `karp-backend-5-5.27.5/doc/about.tex`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/Makefile` & `karp-backend-5-5.27.5/Makefile`

 * *Files 7% similar despite different names*

```diff
@@ -66,21 +66,25 @@
 
 lint-syntax-errors: install-test
 	${INVENV} flake8 karp5 setup.py run.py cli.py --count --select=E9,F63,F7,F82 --show-source --statistics ${FLAKE8_FLAGS}
 
 test: install-test clean-pyc
 	${INVENV} pytest -vv karp5/tests/unit_tests
 
+cov_report := "term-missing"
 test-w-coverage: install-test clean-pyc
-	${INVENV} pytest -vv --cov-config=setup.cfg --cov=karp5 --cov-report=term-missing karp5/tests
+	${INVENV} pytest -vv --cov-config=setup.cfg --cov=karp5 --cov-report=${cov_report} karp5/tests
 
 test-log: install-test clean-pyc
 	${INVENV} pytest --cov=karp5 --cov-report=term-missing karp5/tests > pytest.log
 
-lint: install
+lint:
+	${INVENV} pylint --rcfile .pylintrc --disable=all --enable=E,W karp5 setup.py cli.py run.py
+
+lint-all:
 	${INVENV} pylint --rcfile .pylintrc karp5 setup.py cli.py run.py
 
 lint-no-fail: install
 	${INVENV} pylint --rcfile .pylintrc --exit-zero karp5 setup.py cli.py run.py
 
 type-check: install-test install-typecheck
 	${INVENV} pytype karp5
```

### Comparing `karp-backend-5-5.26.4/karp5/backend.py` & `karp-backend-5-5.27.5/karp5/backend.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/server/update.py` & `karp-backend-5-5.27.5/karp5/server/update.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/server/searching.py` & `karp-backend-5-5.27.5/karp5/server/searching.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/server/translator/bulkify.py` & `karp-backend-5-5.27.5/karp5/server/translator/bulkify.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/server/translator/elasticObjects.py` & `karp-backend-5-5.27.5/karp5/server/translator/elasticObjects.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/server/translator/validatejson.py` & `karp-backend-5-5.27.5/karp5/server/translator/validatejson.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/server/translator/errors.py` & `karp-backend-5-5.27.5/karp5/server/translator/errors.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/server/translator/parser.py` & `karp-backend-5-5.27.5/karp5/server/translator/parser.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/server/idgenerator.py` & `karp-backend-5-5.27.5/karp5/server/idgenerator.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/server/checkdbhistory.py` & `karp-backend-5-5.27.5/karp5/server/checkdbhistory.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/server/helper/jsonwalk.py` & `karp-backend-5-5.27.5/karp5/server/helper/jsonwalk.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/server/helper/flaskhelper.py` & `karp-backend-5-5.27.5/karp5/server/helper/flaskhelper.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/server/helper/helpers.py` & `karp-backend-5-5.27.5/karp5/server/helper/helpers.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/server/suggestions.py` & `karp-backend-5-5.27.5/karp5/server/suggestions.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/document/autoupdates.py` & `karp-backend-5-5.27.5/karp5/document/autoupdates.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/document/doc_converter.py` & `karp-backend-5-5.27.5/karp5/document/doc_converter.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/context/auth/std_auth.py` & `karp-backend-5-5.27.5/karp5/context/auth/std_auth.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/context/auth/__init__.py` & `karp-backend-5-5.27.5/karp5/context/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/context/auth/dummy_auth.py` & `karp-backend-5-5.27.5/karp5/context/auth/dummy_auth.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/__init__.py` & `karp-backend-5-5.27.5/karp5/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-__version__ = "5.26.4"
+__version__ = "5.27.5"
 
 import pkg_resources
 import logging
 import logging.handlers
 import os
 
 import six
 
 from .instance_info import get_instance_path
 
 from flask import Flask, request
 
 from karp5.config import Config, conf_mgr
+from karp5.server.extensions import matomo
 
 
 __name = "karp5"
 
 
 class RequestFormatter(logging.Formatter):
     def __init__(self, fmt=None, datefmt=None):
@@ -46,26 +47,30 @@
     else:
         auth.init("std")
 
     from karp5.server.helper import flaskhelper
 
     flaskhelper.init_errorhandler(app)
 
+    configure_extensions(app)
+
     from karp5 import backend
 
     flaskhelper.register(app, backend.init)
 
     print("app.debug = {}".format(app.debug))
     print("app.testing = {}".format(app.testing))
     print("Setting up loggers")
     logger = logging.getLogger("karp5")
     logger.setLevel(app.config["LOG_LEVEL"])
     print("log_fmt = {}".format(app.config["LOG_FMT"]))
     print("log_datefmt = {}".format(app.config["LOG_DATEFMT"]))
-    formatter = logging.Formatter(fmt=app.config["LOG_FMT"], datefmt=app.config["LOG_DATEFMT"])
+    formatter = logging.Formatter(
+        fmt=app.config["LOG_FMT"], datefmt=app.config["LOG_DATEFMT"]
+    )
 
     request_logger = logging.getLogger("karp5.requests")
     request_logger.setLevel(logging.INFO)
     request_formatter = RequestFormatter(
         fmt="[%(asctime)s] %(req_remote_addr)s %(req_method)s %(req_url)s %(message)s",
         datefmt=app.config["LOG_DATEFMT"],
     )
@@ -87,22 +92,25 @@
             os.path.join(log_dir, "karp5.log"), when="d", interval=1, backupCount=0
         )
         file_handler.setLevel(app.config["LOG_LEVEL"])
         file_handler.setFormatter(formatter)
         logger.addHandler(file_handler)
 
         request_file_handler = logging.handlers.TimedRotatingFileHandler(
-            os.path.join(log_dir, "karp5.requests.log"), when="d", interval=1, backupCount=0,
+            os.path.join(log_dir, "karp5.requests.log"),
+            when="d",
+            interval=1,
+            backupCount=0,
         )
         request_file_handler.setFormatter(request_formatter)
         request_logger.addHandler(request_file_handler)
 
     @app.after_request
     def after_request(response):
-        """ Logging after every request. """
+        """Logging after every request."""
         request_logger.info(response.status)
         return response
 
     return app
 
 
 def get_version():
@@ -115,7 +123,12 @@
 
 def get_pkg_resource(filename):
     assert pkg_resources.resource_exists(__name__, filename)
     result = pkg_resources.resource_string(__name__, filename)
     if isinstance(result, six.binary_type):
         result = result.decode("utf-8")
     return result
+
+
+def configure_extensions(app: Flask) -> None:
+    if matomo.matomo_url != "NOT_USED":
+        matomo.init_app(app)
```

### Comparing `karp-backend-5-5.26.4/karp5/html/api.md` & `karp-backend-5-5.27.5/karp5/html/api.md`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/html/index_dokumentation.html` & `karp-backend-5-5.27.5/karp5/html/index_dokumentation.html`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/config/configmanager.py` & `karp-backend-5-5.27.5/karp5/config/configmanager.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/config/config.py` & `karp-backend-5-5.27.5/karp5/config/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,40 +20,54 @@
 
 
 class Config:
     """[summary]"""
 
     DEBUG = False
     TESTING = False
-    LOG_LEVEL = getattr(logging, _CONFIG["DEBUG"]["DEBUGLEVEL"].upper(), logging.WARNING)
+    LOG_LEVEL = getattr(
+        logging, _CONFIG["DEBUG"]["DEBUGLEVEL"].upper(), logging.WARNING
+    )
     # LOG_LEVEL = debug_str_to_int(_CONFIG['DEBUG']['DEBUGLEVEL'])
     LOG_FMT = _CONFIG["DEBUG"].get("LOGFMT")
     LOG_DIR = _CONFIG["DEBUG"].get("LOGDIR")
     LOG_DATEFMT = _CONFIG["DEBUG"].get("DATEFMT")
     LOG_TO_STDERR = _CONFIG["DEBUG"].get("DEBUG_TO_STDERR")
     SECRET_KEY = ENV_SETUP_SECRET_KEY or _CONFIG["SETUP"]["SECRET_KEY"]
     ABSOLUTE_PATH = _CONFIG["SETUP"]["ABSOLUTE_PATH"]
-    BACKEND_URL = _CONFIG["SETUP"].get("BACKEND_URL") or "https://ws.spraakbanken.gu.se/ws/karp/v5"
+    BACKEND_URL = (
+        _CONFIG["SETUP"].get("BACKEND_URL")
+        or "https://ws.spraakbanken.gu.se/ws/karp/v5"
+    )
     SCRIPT_PATH = _CONFIG["SETUP"]["SCRIPT_PATH"]
     SENDER_EMAIL = _CONFIG["DB"]["SENDER_EMAIL"]
     SMTP_SERVER = _CONFIG["DB"].get("SMTP_SERVER")
     AUTH_RESOURCES = _CONFIG["AUTH"]["AUTH_RESOURCES"]
     AUTH_SECRET = ENV_AUTH_SECRET or _CONFIG["AUTH"]["AUTH_SECRET"]
     AUTH_SERVER = _CONFIG["AUTH"]["AUTH_SERVER"]
     ADMIN_EMAILS = _CONFIG["DB"].get("ADMIN_EMAILS")
     MAX_PAGE = _CONFIG["SETUP"]["MAX_PAGE"]
     MINIENTRY_PAGE = _CONFIG["SETUP"]["MINIENTRY_PAGE"]
     SCAN_LIMIT = _CONFIG["SETUP"]["SCAN_LIMIT"]
-    ELASTICSEARCH_URL = os.environ.get("KARP5_ELASTICSEARCH_URL", "http://localhost:9200").split(
-        ","
-    )
+    ELASTICSEARCH_URL = os.environ.get(
+        "KARP5_ELASTICSEARCH_URL", "http://localhost:9200"
+    ).split(",")
     OVERRIDE_ELASTICSEARCH_URL = strtobool(
         os.environ.get("KARP5_ELASTICSEARCH_URL_OVERRIDE", "false")
     )
     TESTING = False
     DEBUG = False
     DATABASE_BASEURL = (
         f"mysql+pymysql://{ENV_DBPASS}/" + "{}?charset=utf8"
         if ENV_DBPASS
         else f"mysql+pymysql://{_CONFIG['DB']['DBPASS']}/" + "{}?charset=utf8"
     )
     STANDARDMODE = _CONFIG["SETUP"]["STANDARDMODE"]
+    TRACKING_MATOMO_URL = _CONFIG["SETUP"].get("MATOMO_URL") or os.environ.get(
+        "KARP5_TRACKING_URL"
+    )
+    TRACKING_SITE_ID = _CONFIG["SETUP"].get("SITE_ID") or os.environ.get(
+        "KARP5_TRACKING_SITE_ID"
+    )
+    TRACKING_AUTH_TOKEN = _CONFIG["SETUP"].get("AUTH_TOKEN") or os.environ.get(
+        "KARP5_TRACKING_AUTH_TOKEN"
+    )
```

### Comparing `karp-backend-5-5.26.4/karp5/static/karp.png` & `karp-backend-5-5.27.5/karp5/static/karp.png`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/static/api.css` & `karp-backend-5-5.27.5/karp5/static/api.css`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/errors.py` & `karp-backend-5-5.27.5/karp5/errors.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/cli/getmapping.py` & `karp-backend-5-5.27.5/karp5/cli/getmapping.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/cli/create_metadata.py` & `karp-backend-5-5.27.5/karp5/cli/create_metadata.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/cli/__init__.py` & `karp-backend-5-5.27.5/karp5/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/cli/upload_offline.py` & `karp-backend-5-5.27.5/karp5/cli/upload_offline.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/util/text.py` & `karp-backend-5-5.27.5/karp5/util/text.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/tests/data/data/large_lex/large_lex.json` & `karp-backend-5-5.27.5/karp5/tests/data/data/large_lex/large_lex.json`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/tests/data/data/panacea/panacea.json` & `karp-backend-5-5.27.5/karp5/tests/data/data/panacea/panacea.json`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/tests/data/config/mappings/mappingconf_foo.json` & `karp-backend-5-5.27.5/karp5/tests/data/config/mappings/mappingconf_foo.json`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/tests/data/config/mappings/mappingconf_panacea.json` & `karp-backend-5-5.27.5/karp5/tests/data/config/mappings/mappingconf_panacea.json`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/tests/data/config/mappings/mappingconf_panacea_links.json` & `karp-backend-5-5.27.5/karp5/tests/data/config/mappings/mappingconf_panacea_links.json`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/tests/data/config/config.json` & `karp-backend-5-5.27.5/karp5/tests/data/config/config.json`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/tests/data/config/modes.json` & `karp-backend-5-5.27.5/karp5/tests/data/config/modes.json`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/tests/data/config/lexiconconf.json` & `karp-backend-5-5.27.5/karp5/tests/data/config/lexiconconf.json`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/tests/util.py` & `karp-backend-5-5.27.5/karp5/tests/util.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/tests/auth_server.py` & `karp-backend-5-5.27.5/karp5/tests/auth_server.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/tests/test_update_index.py` & `karp-backend-5-5.27.5/karp5/tests/test_update_index.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/tests/common_fixtures.py` & `karp-backend-5-5.27.5/karp5/tests/common_fixtures.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/tests/api/test_autocomplete.py` & `karp-backend-5-5.27.5/karp5/tests/api/test_autocomplete.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/tests/api/search/test_search.py` & `karp-backend-5-5.27.5/karp5/tests/api/search/test_search.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/tests/api/search/test_pagination.py` & `karp-backend-5-5.27.5/karp5/tests/api/search/test_pagination.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/tests/api/search/test_stats.py` & `karp-backend-5-5.27.5/karp5/tests/api/search/test_stats.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/tests/api/test_explain.py` & `karp-backend-5-5.27.5/karp5/tests/api/test_explain.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/tests/api/test_history.py` & `karp-backend-5-5.27.5/karp5/tests/api/test_history.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/tests/api/test_export.py` & `karp-backend-5-5.27.5/karp5/tests/api/test_export.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/tests/_test_config.py` & `karp-backend-5-5.27.5/karp5/tests/_test_config.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/tests/cli/test_es.py` & `karp-backend-5-5.27.5/karp5/tests/cli/test_es.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/tests/cli/test_upload.py` & `karp-backend-5-5.27.5/karp5/tests/cli/test_upload.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/tests/integration_tests/server/test_searching_integration.py` & `karp-backend-5-5.27.5/karp5/tests/integration_tests/server/test_searching_integration.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/tests/integration_tests/server/translator/test_validatejson_on_panacea.py` & `karp-backend-5-5.27.5/karp5/tests/integration_tests/server/translator/test_validatejson_on_panacea.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/tests/integration_tests/domain/services/test_search_service_it.py` & `karp-backend-5-5.27.5/karp5/tests/integration_tests/domain/services/test_search_service_it.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/tests/conftest.py` & `karp-backend-5-5.27.5/karp5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/tests/unit_tests/server/test_searching.py` & `karp-backend-5-5.27.5/karp5/tests/unit_tests/server/test_searching.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/tests/unit_tests/server/translator/test_parser_statistics.py` & `karp-backend-5-5.27.5/karp5/tests/unit_tests/server/translator/test_parser_statistics.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/tests/unit_tests/server/translator/test_parser_freetext.py` & `karp-backend-5-5.27.5/karp5/tests/unit_tests/server/translator/test_parser_freetext.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/tests/unit_tests/server/translator/test_validatejson.py` & `karp-backend-5-5.27.5/karp5/tests/unit_tests/server/translator/test_validatejson.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/tests/unit_tests/server/translator/test_parser.py` & `karp-backend-5-5.27.5/karp5/tests/unit_tests/server/translator/test_parser.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/tests/unit_tests/server/translator/test_parser_search.py` & `karp-backend-5-5.27.5/karp5/tests/unit_tests/server/translator/test_parser_search.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/tests/unit_tests/server/test_statlist.py` & `karp-backend-5-5.27.5/karp5/tests/unit_tests/server/test_statlist.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/tests/unit_tests/context/auth/test_std_auth.py` & `karp-backend-5-5.27.5/karp5/tests/unit_tests/context/auth/test_std_auth.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/tests/unit_tests/context/auth/test_dummy_auth.py` & `karp-backend-5-5.27.5/karp5/tests/unit_tests/context/auth/test_dummy_auth.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/tests/unit_tests/context/auth/test_auth.py` & `karp-backend-5-5.27.5/karp5/tests/unit_tests/context/auth/test_auth.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/tests/unit_tests/config/test_configmanager.py` & `karp-backend-5-5.27.5/karp5/tests/unit_tests/config/test_configmanager.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/tests/unit_tests/config/test_errors.py` & `karp-backend-5-5.27.5/karp5/tests/unit_tests/config/test_errors.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/tests/unit_tests/test_errors.py` & `karp-backend-5-5.27.5/karp5/tests/unit_tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/tests/unit_tests/domain/services/test_search_service.py` & `karp-backend-5-5.27.5/karp5/tests/unit_tests/domain/services/test_search_service.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/tests/unit_tests/domain/model/test_mode.py` & `karp-backend-5-5.27.5/karp5/tests/unit_tests/domain/model/test_mode.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/tests/unit_tests/dbhandler/test_dbhandler.py` & `karp-backend-5-5.27.5/karp5/tests/unit_tests/dbhandler/test_dbhandler.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/domain/services/search_service.py` & `karp-backend-5-5.27.5/karp5/domain/services/search_service.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/domain/model/mode.py` & `karp-backend-5-5.27.5/karp5/domain/model/mode.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/dbhandler/emailsender.py` & `karp-backend-5-5.27.5/karp5/dbhandler/emailsender.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/dbhandler/dbhandler.py` & `karp-backend-5-5.27.5/karp5/dbhandler/dbhandler.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/karp5/infrastructure/json_file_mode_repository.py` & `karp-backend-5-5.27.5/karp5/infrastructure/json_file_mode_repository.py`

 * *Files identical despite different names*

### Comparing `karp-backend-5-5.26.4/README.md` & `karp-backend-5-5.27.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 **This package is the legacy version of Karp, [go here for the current version(https://github.com/spraakbanken/karp-backend)]**
 
 ## master
 
 [![codecov](https://codecov.io/gh/spraakbanken/karp-backend-v5/branch/master/graph/badge.svg)](https://codecov.io/gh/spraakbanken/karp-backend-v5)
 [![](https://github.com/spraakbanken/karp-backend-v5/workflows/Build/badge.svg)](https://github.com/spraakbanken/karp-backend-v5/actions)
 
-**This package - code and documentation - is still under construction.**
-
 Karp is the lexical platform of Språkbanken.
 Now migrated to Python 3.6+.
 
 # Karp in Docker
 
 For easy testing, use [Docker](https://docs.docker.com/engine/installation/) to run Karp-b.
```

