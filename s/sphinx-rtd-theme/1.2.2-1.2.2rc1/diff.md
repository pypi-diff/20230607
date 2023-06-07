# Comparing `tmp/sphinx_rtd_theme-1.2.2.tar.gz` & `tmp/sphinx_rtd_theme-1.2.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_rtd_theme-1.2.2.tar", last modified: Wed Jun  7 13:27:19 2023, max compression
+gzip compressed data, was "sphinx_rtd_theme-1.2.2rc1.tar", last modified: Wed Jun  7 12:48:22 2023, max compression
```

## Comparing `sphinx_rtd_theme-1.2.2.tar` & `sphinx_rtd_theme-1.2.2rc1.tar`

### file list

```diff
@@ -1,154 +1,154 @@
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.383995 sphinx_rtd_theme-1.2.2/
--rw-rw-r--   0 balder    (1000) balder    (1000)    11379 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2/Apache-License-2.0.txt
--rw-rw-r--   0 balder    (1000) balder    (1000)     1119 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2/LICENSE
--rw-rw-r--   0 balder    (1000) balder    (1000)      576 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2/MANIFEST.in
--rw-rw-r--   0 balder    (1000) balder    (1000)     4438 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2/OFL-License.txt
--rw-rw-r--   0 balder    (1000) balder    (1000)     4182 2023-06-07 13:27:19.383995 sphinx_rtd_theme-1.2.2/PKG-INFO
--rw-rw-r--   0 balder    (1000) balder    (1000)     2742 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2/README.rst
--rw-rw-r--   0 balder    (1000) balder    (1000)      338 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2/babel.cfg
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.367995 sphinx_rtd_theme-1.2.2/bin/
--rwxrwxr-x   0 balder    (1000) balder    (1000)      853 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2/bin/preinstall.js
--rw-rw-r--   0 balder    (1000) balder    (1000)     2946 2023-06-07 13:27:19.383995 sphinx_rtd_theme-1.2.2/setup.cfg
--rw-rw-r--   0 balder    (1000) balder    (1000)     2108 2023-06-07 13:27:13.000000 sphinx_rtd_theme-1.2.2/setup.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.371995 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/
--rw-rw-r--   0 balder    (1000) balder    (1000)     3477 2023-06-07 13:27:13.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/__init__.py
--rw-r--r--   0 balder    (1000) balder    (1000)     4277 2023-06-07 12:45:49.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/breadcrumbs.html
--rw-r--r--   0 balder    (1000) balder    (1000)     2915 2023-06-07 12:45:49.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/footer.html
--rw-r--r--   0 balder    (1000) balder    (1000)     9716 2023-06-07 12:45:49.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/layout.html
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.371995 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.363995 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/da/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.371995 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/da/LC_MESSAGES/
--rw-r--r--   0 balder    (1000) balder    (1000)     2514 2023-06-07 12:45:49.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/da/LC_MESSAGES/sphinx.mo
--rw-r--r--   0 balder    (1000) balder    (1000)     5820 2023-06-07 12:45:49.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/da/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.363995 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/de/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.371995 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/de/LC_MESSAGES/
--rw-r--r--   0 balder    (1000) balder    (1000)     2087 2023-06-07 12:45:49.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/de/LC_MESSAGES/sphinx.mo
--rw-r--r--   0 balder    (1000) balder    (1000)     4023 2023-06-07 12:45:49.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/de/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.363995 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/en/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.371995 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/en/LC_MESSAGES/
--rw-r--r--   0 balder    (1000) balder    (1000)      457 2023-06-07 12:45:49.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/en/LC_MESSAGES/sphinx.mo
--rw-r--r--   0 balder    (1000) balder    (1000)     4912 2023-06-07 12:45:49.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/en/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.363995 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/es/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.371995 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/es/LC_MESSAGES/
--rw-r--r--   0 balder    (1000) balder    (1000)     2567 2023-06-07 12:45:49.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/es/LC_MESSAGES/sphinx.mo
--rw-r--r--   0 balder    (1000) balder    (1000)     5094 2023-06-07 12:45:49.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/es/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.363995 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/et/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.371995 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/et/LC_MESSAGES/
--rw-r--r--   0 balder    (1000) balder    (1000)     2380 2023-06-07 12:45:49.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/et/LC_MESSAGES/sphinx.mo
--rw-r--r--   0 balder    (1000) balder    (1000)     4828 2023-06-07 12:45:49.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/et/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.363995 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/fa_IR/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.371995 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/fa_IR/LC_MESSAGES/
--rw-r--r--   0 balder    (1000) balder    (1000)     2693 2023-06-07 12:45:49.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/fa_IR/LC_MESSAGES/sphinx.mo
--rw-r--r--   0 balder    (1000) balder    (1000)     5018 2023-06-07 12:45:49.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/fa_IR/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.363995 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/fr/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.371995 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/fr/LC_MESSAGES/
--rw-r--r--   0 balder    (1000) balder    (1000)     2522 2023-06-07 12:45:49.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/fr/LC_MESSAGES/sphinx.mo
--rw-r--r--   0 balder    (1000) balder    (1000)     5050 2023-06-07 12:45:49.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/fr/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.363995 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/hr/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.371995 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/hr/LC_MESSAGES/
--rw-r--r--   0 balder    (1000) balder    (1000)      575 2023-06-07 12:45:49.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/hr/LC_MESSAGES/sphinx.mo
--rw-r--r--   0 balder    (1000) balder    (1000)      842 2023-06-07 12:45:49.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/hr/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.367995 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/hu/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.371995 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/hu/LC_MESSAGES/
--rw-r--r--   0 balder    (1000) balder    (1000)      501 2023-06-07 12:45:49.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/hu/LC_MESSAGES/sphinx.mo
--rw-r--r--   0 balder    (1000) balder    (1000)      765 2023-06-07 12:45:49.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/hu/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.367995 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/it/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.371995 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/it/LC_MESSAGES/
--rw-r--r--   0 balder    (1000) balder    (1000)     2703 2023-06-07 12:45:49.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/it/LC_MESSAGES/sphinx.mo
--rw-r--r--   0 balder    (1000) balder    (1000)     5824 2023-06-07 12:45:49.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/it/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.367995 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/lt/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.371995 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/lt/LC_MESSAGES/
--rw-r--r--   0 balder    (1000) balder    (1000)     2750 2023-06-07 12:45:49.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/lt/LC_MESSAGES/sphinx.mo
--rw-r--r--   0 balder    (1000) balder    (1000)     5711 2023-06-07 12:45:49.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/lt/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.367995 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/nl/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.375995 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/nl/LC_MESSAGES/
--rw-r--r--   0 balder    (1000) balder    (1000)     2549 2023-06-07 12:45:49.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/nl/LC_MESSAGES/sphinx.mo
--rw-r--r--   0 balder    (1000) balder    (1000)     5505 2023-06-07 12:45:49.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/nl/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.367995 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/pl/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.375995 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/pl/LC_MESSAGES/
--rw-r--r--   0 balder    (1000) balder    (1000)     2339 2023-06-07 12:45:49.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/pl/LC_MESSAGES/sphinx.mo
--rw-r--r--   0 balder    (1000) balder    (1000)     4257 2023-06-07 12:45:49.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/pl/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.367995 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/pt/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.375995 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/pt/LC_MESSAGES/
--rw-r--r--   0 balder    (1000) balder    (1000)     2354 2023-06-07 12:45:49.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/pt/LC_MESSAGES/sphinx.mo
--rw-r--r--   0 balder    (1000) balder    (1000)     5038 2023-06-07 12:45:49.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/pt/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.367995 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/pt_BR/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.375995 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 balder    (1000) balder    (1000)     2780 2023-06-07 12:45:49.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/pt_BR/LC_MESSAGES/sphinx.mo
--rw-r--r--   0 balder    (1000) balder    (1000)     5830 2023-06-07 12:45:49.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/pt_BR/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.367995 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/ru/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.375995 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/ru/LC_MESSAGES/
--rw-r--r--   0 balder    (1000) balder    (1000)     3449 2023-06-07 12:45:49.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/ru/LC_MESSAGES/sphinx.mo
--rw-r--r--   0 balder    (1000) balder    (1000)     6468 2023-06-07 12:45:49.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/ru/LC_MESSAGES/sphinx.po
--rw-r--r--   0 balder    (1000) balder    (1000)     4633 2023-06-07 12:45:49.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/sphinx.pot
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.367995 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/sv/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.375995 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/sv/LC_MESSAGES/
--rw-r--r--   0 balder    (1000) balder    (1000)     2132 2023-06-07 12:45:49.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/sv/LC_MESSAGES/sphinx.mo
--rw-r--r--   0 balder    (1000) balder    (1000)     4353 2023-06-07 12:45:49.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/sv/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.367995 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/tr/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.375995 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/tr/LC_MESSAGES/
--rw-r--r--   0 balder    (1000) balder    (1000)     2117 2023-06-07 12:45:49.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/tr/LC_MESSAGES/sphinx.mo
--rw-r--r--   0 balder    (1000) balder    (1000)     4142 2023-06-07 12:45:49.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/tr/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.367995 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/zh_CN/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.375995 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 balder    (1000) balder    (1000)     2511 2023-06-07 12:45:49.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/zh_CN/LC_MESSAGES/sphinx.mo
--rw-r--r--   0 balder    (1000) balder    (1000)     5523 2023-06-07 12:45:49.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/zh_CN/LC_MESSAGES/sphinx.po
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.367995 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/zh_TW/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.375995 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/zh_TW/LC_MESSAGES/
--rw-r--r--   0 balder    (1000) balder    (1000)      506 2023-06-07 12:45:49.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/zh_TW/LC_MESSAGES/sphinx.mo
--rw-r--r--   0 balder    (1000) balder    (1000)      769 2023-06-07 12:45:49.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/zh_TW/LC_MESSAGES/sphinx.po
--rw-r--r--   0 balder    (1000) balder    (1000)     1759 2023-06-07 12:45:49.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/search.html
--rw-r--r--   0 balder    (1000) balder    (1000)      405 2023-06-07 12:45:49.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/searchbox.html
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.367995 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.375995 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/css/
--rw-r--r--   0 balder    (1000) balder    (1000)     3229 2023-06-07 12:45:53.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/css/badge_only.css
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.379995 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/css/fonts/
--rw-r--r--   0 balder    (1000) balder    (1000)    87624 2023-06-07 12:45:53.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0 balder    (1000) balder    (1000)    67312 2023-06-07 12:45:53.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0 balder    (1000) balder    (1000)    86288 2023-06-07 12:45:53.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0 balder    (1000) balder    (1000)    66444 2023-06-07 12:45:53.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0 balder    (1000) balder    (1000)   165742 2023-06-07 12:45:53.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0 balder    (1000) balder    (1000)   444379 2023-06-07 12:45:53.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0 balder    (1000) balder    (1000)   165548 2023-06-07 12:45:53.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 balder    (1000) balder    (1000)    98024 2023-06-07 12:45:53.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0 balder    (1000) balder    (1000)    77160 2023-06-07 12:45:53.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 balder    (1000) balder    (1000)   323344 2023-06-07 12:45:53.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0 balder    (1000) balder    (1000)   193308 2023-06-07 12:45:53.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0 balder    (1000) balder    (1000)   309728 2023-06-07 12:45:53.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/css/fonts/lato-bold.woff
--rw-r--r--   0 balder    (1000) balder    (1000)   184912 2023-06-07 12:45:53.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/css/fonts/lato-bold.woff2
--rw-r--r--   0 balder    (1000) balder    (1000)   328412 2023-06-07 12:45:53.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0 balder    (1000) balder    (1000)   195704 2023-06-07 12:45:53.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0 balder    (1000) balder    (1000)   309192 2023-06-07 12:45:53.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/css/fonts/lato-normal.woff
--rw-r--r--   0 balder    (1000) balder    (1000)   182708 2023-06-07 12:45:53.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/css/fonts/lato-normal.woff2
--rw-r--r--   0 balder    (1000) balder    (1000)   135314 2023-06-07 12:45:53.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/css/theme.css
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.379995 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/js/
--rw-r--r--   0 balder    (1000) balder    (1000)      934 2023-06-07 12:45:53.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/js/badge_only.js
--rw-r--r--   0 balder    (1000) balder    (1000)     4370 2023-06-07 12:45:53.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/js/html5shiv-printshiv.min.js
--rw-r--r--   0 balder    (1000) balder    (1000)     2734 2023-06-07 12:45:53.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/js/html5shiv.min.js
--rw-r--r--   0 balder    (1000) balder    (1000)     5023 2023-06-07 12:45:53.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/js/theme.js
--rw-r--r--   0 balder    (1000) balder    (1000)      407 2023-06-07 12:45:49.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/theme.conf
--rw-r--r--   0 balder    (1000) balder    (1000)     1247 2023-06-07 12:45:49.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/versions.html
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.371995 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme.egg-info/
--rw-rw-r--   0 balder    (1000) balder    (1000)     4182 2023-06-07 13:27:19.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme.egg-info/PKG-INFO
--rw-rw-r--   0 balder    (1000) balder    (1000)     4199 2023-06-07 13:27:19.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme.egg-info/SOURCES.txt
--rw-rw-r--   0 balder    (1000) balder    (1000)        1 2023-06-07 13:27:19.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme.egg-info/dependency_links.txt
--rw-rw-r--   0 balder    (1000) balder    (1000)       57 2023-06-07 13:27:19.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme.egg-info/entry_points.txt
--rw-rw-r--   0 balder    (1000) balder    (1000)        1 2023-01-13 09:47:39.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme.egg-info/not-zip-safe
--rw-rw-r--   0 balder    (1000) balder    (1000)      124 2023-06-07 13:27:19.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme.egg-info/requires.txt
--rw-rw-r--   0 balder    (1000) balder    (1000)       17 2023-06-07 13:27:19.000000 sphinx_rtd_theme-1.2.2/sphinx_rtd_theme.egg-info/top_level.txt
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.379995 sphinx_rtd_theme-1.2.2/tests/
--rw-rw-r--   0 balder    (1000) balder    (1000)        0 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2/tests/__init__.py
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.367995 sphinx_rtd_theme-1.2.2/tests/roots/
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.383995 sphinx_rtd_theme-1.2.2/tests/roots/test-basic/
--rw-rw-r--   0 balder    (1000) balder    (1000)        8 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2/tests/roots/test-basic/bar.rst
--rw-rw-r--   0 balder    (1000) balder    (1000)       76 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2/tests/roots/test-basic/conf.py
--rw-rw-r--   0 balder    (1000) balder    (1000)       31 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2/tests/roots/test-basic/foo.rst
--rw-rw-r--   0 balder    (1000) balder    (1000)       85 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2/tests/roots/test-basic/index.rst
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.383995 sphinx_rtd_theme-1.2.2/tests/roots/test-empty/
--rw-rw-r--   0 balder    (1000) balder    (1000)       76 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2/tests/roots/test-empty/conf.py
--rw-rw-r--   0 balder    (1000) balder    (1000)       76 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2/tests/roots/test-empty/index.rst
-drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 13:27:19.383995 sphinx_rtd_theme-1.2.2/tests/roots/test-missing-toctree/
--rw-rw-r--   0 balder    (1000) balder    (1000)       76 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2/tests/roots/test-missing-toctree/conf.py
--rw-rw-r--   0 balder    (1000) balder    (1000)       42 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2/tests/roots/test-missing-toctree/index.rst
--rw-rw-r--   0 balder    (1000) balder    (1000)     3159 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2/tests/test_builders.py
--rw-rw-r--   0 balder    (1000) balder    (1000)     1770 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2/tests/util.py
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.119685 sphinx_rtd_theme-1.2.2rc1/
+-rw-rw-r--   0 balder    (1000) balder    (1000)    11379 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2rc1/Apache-License-2.0.txt
+-rw-rw-r--   0 balder    (1000) balder    (1000)     1119 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2rc1/LICENSE
+-rw-rw-r--   0 balder    (1000) balder    (1000)      576 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2rc1/MANIFEST.in
+-rw-rw-r--   0 balder    (1000) balder    (1000)     4438 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2rc1/OFL-License.txt
+-rw-rw-r--   0 balder    (1000) balder    (1000)     4185 2023-06-07 12:48:22.119685 sphinx_rtd_theme-1.2.2rc1/PKG-INFO
+-rw-rw-r--   0 balder    (1000) balder    (1000)     2742 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2rc1/README.rst
+-rw-rw-r--   0 balder    (1000) balder    (1000)      338 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2rc1/babel.cfg
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.099684 sphinx_rtd_theme-1.2.2rc1/bin/
+-rwxrwxr-x   0 balder    (1000) balder    (1000)      853 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2rc1/bin/preinstall.js
+-rw-rw-r--   0 balder    (1000) balder    (1000)     2949 2023-06-07 12:48:22.119685 sphinx_rtd_theme-1.2.2rc1/setup.cfg
+-rw-rw-r--   0 balder    (1000) balder    (1000)     2111 2023-06-07 12:41:28.000000 sphinx_rtd_theme-1.2.2rc1/setup.py
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.099684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/
+-rw-r--r--   0 balder    (1000) balder    (1000)     3480 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/__init__.py
+-rw-r--r--   0 balder    (1000) balder    (1000)     4277 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/breadcrumbs.html
+-rw-r--r--   0 balder    (1000) balder    (1000)     2915 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/footer.html
+-rw-r--r--   0 balder    (1000) balder    (1000)     9716 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/layout.html
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.103684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.095684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/da/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.103684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/da/LC_MESSAGES/
+-rw-r--r--   0 balder    (1000) balder    (1000)     2514 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/da/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 balder    (1000) balder    (1000)     5820 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/da/LC_MESSAGES/sphinx.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.095684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/de/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.103684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/de/LC_MESSAGES/
+-rw-r--r--   0 balder    (1000) balder    (1000)     2087 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/de/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 balder    (1000) balder    (1000)     4023 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/de/LC_MESSAGES/sphinx.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.095684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/en/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.103684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/en/LC_MESSAGES/
+-rw-r--r--   0 balder    (1000) balder    (1000)      457 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/en/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 balder    (1000) balder    (1000)     4912 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/en/LC_MESSAGES/sphinx.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.095684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/es/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.103684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/es/LC_MESSAGES/
+-rw-r--r--   0 balder    (1000) balder    (1000)     2567 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/es/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 balder    (1000) balder    (1000)     5094 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/es/LC_MESSAGES/sphinx.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.095684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/et/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.103684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/et/LC_MESSAGES/
+-rw-r--r--   0 balder    (1000) balder    (1000)     2380 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/et/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 balder    (1000) balder    (1000)     4828 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/et/LC_MESSAGES/sphinx.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.095684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/fa_IR/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.103684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/fa_IR/LC_MESSAGES/
+-rw-r--r--   0 balder    (1000) balder    (1000)     2693 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/fa_IR/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 balder    (1000) balder    (1000)     5018 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/fa_IR/LC_MESSAGES/sphinx.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.095684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/fr/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.103684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 balder    (1000) balder    (1000)     2522 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/fr/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 balder    (1000) balder    (1000)     5050 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/fr/LC_MESSAGES/sphinx.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.095684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/hr/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.103684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/hr/LC_MESSAGES/
+-rw-r--r--   0 balder    (1000) balder    (1000)      575 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/hr/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 balder    (1000) balder    (1000)      842 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/hr/LC_MESSAGES/sphinx.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.095684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/hu/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.103684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/hu/LC_MESSAGES/
+-rw-r--r--   0 balder    (1000) balder    (1000)      501 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/hu/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 balder    (1000) balder    (1000)      765 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/hu/LC_MESSAGES/sphinx.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.095684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/it/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.103684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/it/LC_MESSAGES/
+-rw-r--r--   0 balder    (1000) balder    (1000)     2703 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/it/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 balder    (1000) balder    (1000)     5824 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/it/LC_MESSAGES/sphinx.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.095684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/lt/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.103684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 balder    (1000) balder    (1000)     2750 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/lt/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 balder    (1000) balder    (1000)     5711 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/lt/LC_MESSAGES/sphinx.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.095684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/nl/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.103684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 balder    (1000) balder    (1000)     2549 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/nl/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 balder    (1000) balder    (1000)     5505 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/nl/LC_MESSAGES/sphinx.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.095684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/pl/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.107684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 balder    (1000) balder    (1000)     2339 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/pl/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 balder    (1000) balder    (1000)     4257 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/pl/LC_MESSAGES/sphinx.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.095684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/pt/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.107684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/pt/LC_MESSAGES/
+-rw-r--r--   0 balder    (1000) balder    (1000)     2354 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/pt/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 balder    (1000) balder    (1000)     5038 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/pt/LC_MESSAGES/sphinx.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.095684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/pt_BR/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.107684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 balder    (1000) balder    (1000)     2780 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/pt_BR/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 balder    (1000) balder    (1000)     5830 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/pt_BR/LC_MESSAGES/sphinx.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.095684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/ru/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.107684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 balder    (1000) balder    (1000)     3449 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/ru/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 balder    (1000) balder    (1000)     6468 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/ru/LC_MESSAGES/sphinx.po
+-rw-r--r--   0 balder    (1000) balder    (1000)     4633 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/sphinx.pot
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.095684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/sv/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.107684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/sv/LC_MESSAGES/
+-rw-r--r--   0 balder    (1000) balder    (1000)     2132 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/sv/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 balder    (1000) balder    (1000)     4353 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/sv/LC_MESSAGES/sphinx.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.095684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/tr/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.107684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 balder    (1000) balder    (1000)     2117 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/tr/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 balder    (1000) balder    (1000)     4142 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/tr/LC_MESSAGES/sphinx.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.095684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/zh_CN/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.107684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 balder    (1000) balder    (1000)     2511 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/zh_CN/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 balder    (1000) balder    (1000)     5523 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/zh_CN/LC_MESSAGES/sphinx.po
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.095684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/zh_TW/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.107684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 balder    (1000) balder    (1000)      506 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/zh_TW/LC_MESSAGES/sphinx.mo
+-rw-r--r--   0 balder    (1000) balder    (1000)      769 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/zh_TW/LC_MESSAGES/sphinx.po
+-rw-r--r--   0 balder    (1000) balder    (1000)     1759 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/search.html
+-rw-r--r--   0 balder    (1000) balder    (1000)      405 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/searchbox.html
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.095684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.107684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/
+-rw-r--r--   0 balder    (1000) balder    (1000)     3229 2023-06-07 12:45:39.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/badge_only.css
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.111684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/
+-rw-r--r--   0 balder    (1000) balder    (1000)    87624 2023-06-07 12:45:39.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0 balder    (1000) balder    (1000)    67312 2023-06-07 12:45:39.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0 balder    (1000) balder    (1000)    86288 2023-06-07 12:45:39.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0 balder    (1000) balder    (1000)    66444 2023-06-07 12:45:39.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0 balder    (1000) balder    (1000)   165742 2023-06-07 12:45:39.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 balder    (1000) balder    (1000)   444379 2023-06-07 12:45:39.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 balder    (1000) balder    (1000)   165548 2023-06-07 12:45:39.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 balder    (1000) balder    (1000)    98024 2023-06-07 12:45:39.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 balder    (1000) balder    (1000)    77160 2023-06-07 12:45:39.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 balder    (1000) balder    (1000)   323344 2023-06-07 12:45:39.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0 balder    (1000) balder    (1000)   193308 2023-06-07 12:45:39.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0 balder    (1000) balder    (1000)   309728 2023-06-07 12:45:39.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/lato-bold.woff
+-rw-r--r--   0 balder    (1000) balder    (1000)   184912 2023-06-07 12:45:39.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/lato-bold.woff2
+-rw-r--r--   0 balder    (1000) balder    (1000)   328412 2023-06-07 12:45:39.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0 balder    (1000) balder    (1000)   195704 2023-06-07 12:45:39.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0 balder    (1000) balder    (1000)   309192 2023-06-07 12:45:39.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/lato-normal.woff
+-rw-r--r--   0 balder    (1000) balder    (1000)   182708 2023-06-07 12:45:39.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/lato-normal.woff2
+-rw-r--r--   0 balder    (1000) balder    (1000)   135314 2023-06-07 12:45:39.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/theme.css
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.111684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/js/
+-rw-r--r--   0 balder    (1000) balder    (1000)      934 2023-06-07 12:45:39.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/js/badge_only.js
+-rw-r--r--   0 balder    (1000) balder    (1000)     4370 2023-06-07 12:45:39.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/js/html5shiv-printshiv.min.js
+-rw-r--r--   0 balder    (1000) balder    (1000)     2734 2023-06-07 12:45:39.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/js/html5shiv.min.js
+-rw-r--r--   0 balder    (1000) balder    (1000)     5023 2023-06-07 12:45:39.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/js/theme.js
+-rw-r--r--   0 balder    (1000) balder    (1000)      407 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/theme.conf
+-rw-r--r--   0 balder    (1000) balder    (1000)     1247 2023-06-07 12:45:35.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/versions.html
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.103684 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme.egg-info/
+-rw-rw-r--   0 balder    (1000) balder    (1000)     4185 2023-06-07 12:48:22.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme.egg-info/PKG-INFO
+-rw-rw-r--   0 balder    (1000) balder    (1000)     4199 2023-06-07 12:48:22.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme.egg-info/SOURCES.txt
+-rw-rw-r--   0 balder    (1000) balder    (1000)        1 2023-06-07 12:48:22.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme.egg-info/dependency_links.txt
+-rw-rw-r--   0 balder    (1000) balder    (1000)       57 2023-06-07 12:48:22.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme.egg-info/entry_points.txt
+-rw-rw-r--   0 balder    (1000) balder    (1000)        1 2023-01-13 09:47:39.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme.egg-info/not-zip-safe
+-rw-rw-r--   0 balder    (1000) balder    (1000)      124 2023-06-07 12:48:22.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme.egg-info/requires.txt
+-rw-rw-r--   0 balder    (1000) balder    (1000)       17 2023-06-07 12:48:22.000000 sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme.egg-info/top_level.txt
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.115684 sphinx_rtd_theme-1.2.2rc1/tests/
+-rw-rw-r--   0 balder    (1000) balder    (1000)        0 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2rc1/tests/__init__.py
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.099684 sphinx_rtd_theme-1.2.2rc1/tests/roots/
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.115684 sphinx_rtd_theme-1.2.2rc1/tests/roots/test-basic/
+-rw-rw-r--   0 balder    (1000) balder    (1000)        8 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2rc1/tests/roots/test-basic/bar.rst
+-rw-rw-r--   0 balder    (1000) balder    (1000)       76 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2rc1/tests/roots/test-basic/conf.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)       31 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2rc1/tests/roots/test-basic/foo.rst
+-rw-rw-r--   0 balder    (1000) balder    (1000)       85 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2rc1/tests/roots/test-basic/index.rst
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.115684 sphinx_rtd_theme-1.2.2rc1/tests/roots/test-empty/
+-rw-rw-r--   0 balder    (1000) balder    (1000)       76 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2rc1/tests/roots/test-empty/conf.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)       76 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2rc1/tests/roots/test-empty/index.rst
+drwxrwxr-x   0 balder    (1000) balder    (1000)        0 2023-06-07 12:48:22.115684 sphinx_rtd_theme-1.2.2rc1/tests/roots/test-missing-toctree/
+-rw-rw-r--   0 balder    (1000) balder    (1000)       76 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2rc1/tests/roots/test-missing-toctree/conf.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)       42 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2rc1/tests/roots/test-missing-toctree/index.rst
+-rw-rw-r--   0 balder    (1000) balder    (1000)     3159 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2rc1/tests/test_builders.py
+-rw-rw-r--   0 balder    (1000) balder    (1000)     1770 2023-01-13 09:46:18.000000 sphinx_rtd_theme-1.2.2rc1/tests/util.py
```

### Comparing `sphinx_rtd_theme-1.2.2/Apache-License-2.0.txt` & `sphinx_rtd_theme-1.2.2rc1/Apache-License-2.0.txt`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/LICENSE` & `sphinx_rtd_theme-1.2.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/MANIFEST.in` & `sphinx_rtd_theme-1.2.2rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/OFL-License.txt` & `sphinx_rtd_theme-1.2.2rc1/OFL-License.txt`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/PKG-INFO` & `sphinx_rtd_theme-1.2.2rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx_rtd_theme
-Version: 1.2.2
+Version: 1.2.2rc1
 Summary: Read the Docs theme for Sphinx
 Home-page: https://github.com/readthedocs/sphinx_rtd_theme
 Author: Dave Snider, Read the Docs, Inc. & contributors
 Author-email: dev@readthedocs.org
 License: MIT
 Project-URL: Homepage, https://sphinx-rtd-theme.readthedocs.io/
 Project-URL: Source Code, https://github.com/readthedocs/sphinx_rtd_theme
```

### Comparing `sphinx_rtd_theme-1.2.2/README.rst` & `sphinx_rtd_theme-1.2.2rc1/README.rst`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/bin/preinstall.js` & `sphinx_rtd_theme-1.2.2rc1/bin/preinstall.js`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/setup.cfg` & `sphinx_rtd_theme-1.2.2rc1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.2.2
+current_version = 1.2.2rc1
 commit = false
 tag = false
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)((?P<release>[a-z]+)(?P<dev>\d+))?
 serialize = 
 	{major}.{minor}.{patch}{release}{dev}
 	{major}.{minor}.{patch}
```

### Comparing `sphinx_rtd_theme-1.2.2/setup.py` & `sphinx_rtd_theme-1.2.2rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
     def run(self):
         subprocess.run(['tx', 'push', '--source'], check=True)
         subprocess.run(['tx', 'pull', '--mode', 'onlyreviewed', '-f', '-a'], check=True)
 
 
 setup(
-    version='1.2.2',
+    version='1.2.2rc1',
     cmdclass={
         'update_translations': UpdateTranslationsCommand,
         'transifex': TransifexCommand,
         'build_assets': WebpackBuildCommand,
         'watch': WebpackDevelopCommand,
     },
 )
```

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/__init__.py` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from sys import version_info as python_version
 
 from sphinx import version_info as sphinx_version
 from sphinx.locale import _
 from sphinx.util.logging import getLogger
 
 
-__version__ = '1.2.2'
+__version__ = '1.2.2rc1'
 __version_full__ = __version__
 
 logger = getLogger(__name__)
 
 
 def get_html_theme_path():
     """Return list of HTML theme paths."""
```

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/breadcrumbs.html` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/footer.html` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/footer.html`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/layout.html` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/layout.html`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/da/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/da/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/da/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/da/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/de/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/de/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/de/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/de/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/en/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/en/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/es/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/es/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/es/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/es/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/et/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/et/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/et/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/et/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/fa_IR/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/fa_IR/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/fa_IR/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/fa_IR/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/fr/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/fr/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/fr/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/fr/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/hr/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/hr/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/hr/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/hr/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/hu/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/hu/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/it/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/it/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/it/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/it/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/lt/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/lt/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/lt/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/lt/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/nl/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/nl/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/nl/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/nl/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/pl/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/pl/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/pl/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/pl/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/pt/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/pt/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/pt/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/pt/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/pt_BR/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/pt_BR/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/pt_BR/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/pt_BR/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/ru/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/ru/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/ru/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/ru/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/sphinx.pot` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/sphinx.pot`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/sv/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/sv/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/sv/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/sv/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/tr/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/tr/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/tr/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/tr/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/zh_CN/LC_MESSAGES/sphinx.mo` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/zh_CN/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/zh_CN/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/zh_CN/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/locale/zh_TW/LC_MESSAGES/sphinx.po` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/locale/zh_TW/LC_MESSAGES/sphinx.po`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/search.html` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/search.html`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/css/badge_only.css` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/css/fonts/Roboto-Slab-Bold.woff` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/css/fonts/Roboto-Slab-Bold.woff2` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/css/fonts/Roboto-Slab-Regular.woff` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/css/fonts/Roboto-Slab-Regular.woff2` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.eot` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.svg` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.ttf` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.woff` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.woff2` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/css/fonts/lato-bold-italic.woff` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/css/fonts/lato-bold-italic.woff2` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/css/fonts/lato-bold.woff` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/css/fonts/lato-bold.woff2` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/css/fonts/lato-normal-italic.woff` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/css/fonts/lato-normal-italic.woff2` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/css/fonts/lato-normal.woff` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/css/fonts/lato-normal.woff2` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/css/theme.css` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/css/theme.css`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/js/badge_only.js` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/js/html5shiv-printshiv.min.js` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/js/html5shiv.min.js` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/static/js/theme.js` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/static/js/theme.js`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme/versions.html` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme/versions.html`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme.egg-info/PKG-INFO` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-rtd-theme
-Version: 1.2.2
+Version: 1.2.2rc1
 Summary: Read the Docs theme for Sphinx
 Home-page: https://github.com/readthedocs/sphinx_rtd_theme
 Author: Dave Snider, Read the Docs, Inc. & contributors
 Author-email: dev@readthedocs.org
 License: MIT
 Project-URL: Homepage, https://sphinx-rtd-theme.readthedocs.io/
 Project-URL: Source Code, https://github.com/readthedocs/sphinx_rtd_theme
```

### Comparing `sphinx_rtd_theme-1.2.2/sphinx_rtd_theme.egg-info/SOURCES.txt` & `sphinx_rtd_theme-1.2.2rc1/sphinx_rtd_theme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/tests/test_builders.py` & `sphinx_rtd_theme-1.2.2rc1/tests/test_builders.py`

 * *Files identical despite different names*

### Comparing `sphinx_rtd_theme-1.2.2/tests/util.py` & `sphinx_rtd_theme-1.2.2rc1/tests/util.py`

 * *Files identical despite different names*

