# Comparing `tmp/erpbrasil.assinatura-1.6.0.tar.gz` & `tmp/erpbrasil.assinatura-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erpbrasil.assinatura-1.6.0.tar", last modified: Wed Jan  4 14:16:11 2023, max compression
+gzip compressed data, was "/home/renato/git/erpbrasil.assinatura/dist/.tmp-339fn7d7/erpbrasil.assinatura-1.7.0.tar", last modified: Wed Jun  7 13:27:39 2023, max compression
```

## Comparing `erpbrasil.assinatura-1.6.0.tar` & `erpbrasil.assinatura-1.7.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 renatolima   (501) staff       (20)        0 2023-01-04 14:16:11.954089 erpbrasil.assinatura-1.6.0/
--rw-r--r--   0 renatolima   (501) staff       (20)     1424 2021-07-22 15:29:10.000000 erpbrasil.assinatura-1.6.0/.appveyor.yml
--rw-r--r--   0 renatolima   (501) staff       (20)      497 2023-01-04 13:28:23.000000 erpbrasil.assinatura-1.6.0/.bumpversion.cfg
--rw-r--r--   0 renatolima   (501) staff       (20)     2268 2019-11-15 19:34:04.000000 erpbrasil.assinatura-1.6.0/.cookiecutterrc
--rw-r--r--   0 renatolima   (501) staff       (20)      188 2019-11-15 19:34:04.000000 erpbrasil.assinatura-1.6.0/.coveragerc
--rw-r--r--   0 renatolima   (501) staff       (20)      215 2019-11-15 19:34:04.000000 erpbrasil.assinatura-1.6.0/.editorconfig
--rw-r--r--   0 renatolima   (501) staff       (20)      915 2021-07-22 15:31:45.000000 erpbrasil.assinatura-1.6.0/.travis.yml
--rw-r--r--   0 renatolima   (501) staff       (20)       64 2019-11-15 19:34:04.000000 erpbrasil.assinatura-1.6.0/AUTHORS.rst
--rw-r--r--   0 renatolima   (501) staff       (20)      900 2021-07-22 15:31:45.000000 erpbrasil.assinatura-1.6.0/CHANGELOG.rst
--rw-r--r--   0 renatolima   (501) staff       (20)     2812 2019-11-15 19:34:04.000000 erpbrasil.assinatura-1.6.0/CONTRIBUTING.rst
--rw-r--r--   0 renatolima   (501) staff       (20)     1074 2019-11-15 19:34:04.000000 erpbrasil.assinatura-1.6.0/LICENSE
--rw-r--r--   0 renatolima   (501) staff       (20)      408 2021-07-22 15:29:10.000000 erpbrasil.assinatura-1.6.0/MANIFEST.in
--rw-r--r--   0 renatolima   (501) staff       (20)     3568 2023-01-04 14:16:11.954269 erpbrasil.assinatura-1.6.0/PKG-INFO
--rw-r--r--   0 renatolima   (501) staff       (20)     3694 2023-01-04 13:28:23.000000 erpbrasil.assinatura-1.6.0/README.rst
-drwxr-xr-x   0 renatolima   (501) staff       (20)        0 2023-01-04 14:16:11.911531 erpbrasil.assinatura-1.6.0/ci/
--rw-r--r--   0 renatolima   (501) staff       (20)     3995 2019-11-15 19:34:04.000000 erpbrasil.assinatura-1.6.0/ci/appveyor-bootstrap.py
--rwxr-xr-x   0 renatolima   (501) staff       (20)     3827 2019-11-15 19:34:04.000000 erpbrasil.assinatura-1.6.0/ci/appveyor-download.py
--rw-r--r--   0 renatolima   (501) staff       (20)      763 2019-11-15 19:34:04.000000 erpbrasil.assinatura-1.6.0/ci/appveyor-with-compiler.cmd
--rwxr-xr-x   0 renatolima   (501) staff       (20)     2097 2021-07-22 15:29:10.000000 erpbrasil.assinatura-1.6.0/ci/bootstrap.py
--rw-r--r--   0 renatolima   (501) staff       (20)       50 2021-07-22 15:29:10.000000 erpbrasil.assinatura-1.6.0/ci/requirements.txt
-drwxr-xr-x   0 renatolima   (501) staff       (20)        0 2023-01-04 14:16:11.913686 erpbrasil.assinatura-1.6.0/ci/templates/
--rw-r--r--   0 renatolima   (501) staff       (20)     1756 2021-07-22 15:29:10.000000 erpbrasil.assinatura-1.6.0/ci/templates/.appveyor.yml
--rw-r--r--   0 renatolima   (501) staff       (20)      956 2021-07-22 15:29:10.000000 erpbrasil.assinatura-1.6.0/ci/templates/.travis.yml
--rw-r--r--   0 renatolima   (501) staff       (20)     1816 2021-07-22 15:29:10.000000 erpbrasil.assinatura-1.6.0/ci/templates/appveyor.yml
-drwxr-xr-x   0 renatolima   (501) staff       (20)        0 2023-01-04 14:16:11.920773 erpbrasil.assinatura-1.6.0/docs/
--rw-r--r--   0 renatolima   (501) staff       (20)       28 2019-11-15 19:34:04.000000 erpbrasil.assinatura-1.6.0/docs/authors.rst
--rw-r--r--   0 renatolima   (501) staff       (20)       30 2019-11-15 19:34:04.000000 erpbrasil.assinatura-1.6.0/docs/changelog.rst
--rw-r--r--   0 renatolima   (501) staff       (20)     1401 2023-01-04 13:28:23.000000 erpbrasil.assinatura-1.6.0/docs/conf.py
--rw-r--r--   0 renatolima   (501) staff       (20)       33 2019-11-15 19:34:04.000000 erpbrasil.assinatura-1.6.0/docs/contributing.rst
--rw-r--r--   0 renatolima   (501) staff       (20)      245 2019-11-15 19:34:04.000000 erpbrasil.assinatura-1.6.0/docs/index.rst
--rw-r--r--   0 renatolima   (501) staff       (20)      100 2019-11-15 19:34:04.000000 erpbrasil.assinatura-1.6.0/docs/installation.rst
--rw-r--r--   0 renatolima   (501) staff       (20)       27 2019-11-15 19:34:04.000000 erpbrasil.assinatura-1.6.0/docs/readme.rst
-drwxr-xr-x   0 renatolima   (501) staff       (20)        0 2023-01-04 14:16:11.922623 erpbrasil.assinatura-1.6.0/docs/reference/
--rw-r--r--   0 renatolima   (501) staff       (20)      140 2019-11-15 19:34:04.000000 erpbrasil.assinatura-1.6.0/docs/reference/edoc_assinatura.rst
--rw-r--r--   0 renatolima   (501) staff       (20)       72 2019-11-15 19:34:04.000000 erpbrasil.assinatura-1.6.0/docs/reference/index.rst
--rw-r--r--   0 renatolima   (501) staff       (20)       34 2019-11-15 19:34:04.000000 erpbrasil.assinatura-1.6.0/docs/requirements.txt
--rw-r--r--   0 renatolima   (501) staff       (20)      109 2019-11-15 19:34:04.000000 erpbrasil.assinatura-1.6.0/docs/spelling_wordlist.txt
--rw-r--r--   0 renatolima   (501) staff       (20)       92 2019-11-15 19:34:04.000000 erpbrasil.assinatura-1.6.0/docs/usage.rst
--rw-r--r--   0 renatolima   (501) staff       (20)       63 2022-09-07 16:42:03.000000 erpbrasil.assinatura-1.6.0/requirements.txt
--rw-r--r--   0 renatolima   (501) staff       (20)      528 2023-01-04 14:16:11.955408 erpbrasil.assinatura-1.6.0/setup.cfg
--rw-r--r--   0 renatolima   (501) staff       (20)     3255 2023-01-04 13:28:23.000000 erpbrasil.assinatura-1.6.0/setup.py
-drwxr-xr-x   0 renatolima   (501) staff       (20)        0 2023-01-04 14:16:11.894969 erpbrasil.assinatura-1.6.0/src/
-drwxr-xr-x   0 renatolima   (501) staff       (20)        0 2023-01-04 14:16:11.923412 erpbrasil.assinatura-1.6.0/src/erpbrasil/
--rw-r--r--   0 renatolima   (501) staff       (20)      271 2021-07-22 15:29:10.000000 erpbrasil.assinatura-1.6.0/src/erpbrasil/__init__.py
-drwxr-xr-x   0 renatolima   (501) staff       (20)        0 2023-01-04 14:16:11.938161 erpbrasil.assinatura-1.6.0/src/erpbrasil/assinatura/
--rw-r--r--   0 renatolima   (501) staff       (20)      222 2023-01-04 13:28:23.000000 erpbrasil.assinatura-1.6.0/src/erpbrasil/assinatura/__init__.py
--rw-r--r--   0 renatolima   (501) staff       (20)      404 2019-11-15 19:34:04.000000 erpbrasil.assinatura-1.6.0/src/erpbrasil/assinatura/__main__.py
--rw-r--r--   0 renatolima   (501) staff       (20)     4899 2023-01-04 13:27:49.000000 erpbrasil.assinatura-1.6.0/src/erpbrasil/assinatura/assinatura.py
--rw-r--r--   0 renatolima   (501) staff       (20)     4850 2022-09-07 16:42:03.000000 erpbrasil.assinatura-1.6.0/src/erpbrasil/assinatura/certificado.py
--rw-r--r--   0 renatolima   (501) staff       (20)      834 2019-11-15 19:34:04.000000 erpbrasil.assinatura-1.6.0/src/erpbrasil/assinatura/cli.py
--rw-r--r--   0 renatolima   (501) staff       (20)      333 2022-04-30 23:27:08.000000 erpbrasil.assinatura-1.6.0/src/erpbrasil/assinatura/excecoes.py
--rw-r--r--   0 renatolima   (501) staff       (20)     2400 2023-01-04 13:27:49.000000 erpbrasil.assinatura-1.6.0/src/erpbrasil/assinatura/misc.py
-drwxr-xr-x   0 renatolima   (501) staff       (20)        0 2023-01-04 14:16:11.930534 erpbrasil.assinatura-1.6.0/src/erpbrasil.assinatura.egg-info/
--rw-r--r--   0 renatolima   (501) staff       (20)     3568 2023-01-04 14:16:11.000000 erpbrasil.assinatura-1.6.0/src/erpbrasil.assinatura.egg-info/PKG-INFO
--rw-r--r--   0 renatolima   (501) staff       (20)     1639 2023-01-04 14:16:11.000000 erpbrasil.assinatura-1.6.0/src/erpbrasil.assinatura.egg-info/SOURCES.txt
--rw-r--r--   0 renatolima   (501) staff       (20)        1 2023-01-04 14:16:11.000000 erpbrasil.assinatura-1.6.0/src/erpbrasil.assinatura.egg-info/dependency_links.txt
--rw-r--r--   0 renatolima   (501) staff       (20)       71 2023-01-04 14:16:11.000000 erpbrasil.assinatura-1.6.0/src/erpbrasil.assinatura.egg-info/entry_points.txt
--rw-r--r--   0 renatolima   (501) staff       (20)       10 2023-01-04 14:16:11.000000 erpbrasil.assinatura-1.6.0/src/erpbrasil.assinatura.egg-info/namespace_packages.txt
--rw-r--r--   0 renatolima   (501) staff       (20)        1 2021-08-24 20:50:48.000000 erpbrasil.assinatura-1.6.0/src/erpbrasil.assinatura.egg-info/not-zip-safe
--rw-r--r--   0 renatolima   (501) staff       (20)       63 2023-01-04 14:16:11.000000 erpbrasil.assinatura-1.6.0/src/erpbrasil.assinatura.egg-info/requires.txt
--rw-r--r--   0 renatolima   (501) staff       (20)       10 2023-01-04 14:16:11.000000 erpbrasil.assinatura-1.6.0/src/erpbrasil.assinatura.egg-info/top_level.txt
-drwxr-xr-x   0 renatolima   (501) staff       (20)        0 2023-01-04 14:16:11.944336 erpbrasil.assinatura-1.6.0/tests/
-drwxr-xr-x   0 renatolima   (501) staff       (20)        0 2023-01-04 14:16:11.947636 erpbrasil.assinatura-1.6.0/tests/files/
--rw-r--r--   0 renatolima   (501) staff       (20)    60278 2019-11-15 19:34:04.000000 erpbrasil.assinatura-1.6.0/tests/files/google.pdf
--rw-r--r--   0 renatolima   (501) staff       (20)     6015 2019-11-15 19:34:04.000000 erpbrasil.assinatura-1.6.0/tests/files/nfe-400.xml
-drwxr-xr-x   0 renatolima   (501) staff       (20)        0 2023-01-04 14:16:11.949789 erpbrasil.assinatura-1.6.0/tests/fixtures/
--rw-r--r--   0 renatolima   (501) staff       (20)     2597 2021-07-22 15:29:10.000000 erpbrasil.assinatura-1.6.0/tests/fixtures/dummy_cert.pfx
--rw-r--r--   0 renatolima   (501) staff       (20)     3748 2022-04-30 23:27:08.000000 erpbrasil.assinatura-1.6.0/tests/test_erpbrasil_assinatura_pdf.py
--rw-r--r--   0 renatolima   (501) staff       (20)     1512 2021-07-22 15:29:10.000000 erpbrasil.assinatura-1.6.0/tests/test_erpbrasil_assinatura_string.py
--rw-r--r--   0 renatolima   (501) staff       (20)     1122 2021-08-31 14:00:28.000000 erpbrasil.assinatura-1.6.0/tests/test_erpbrasil_assinatura_xml.py
--rw-r--r--   0 renatolima   (501) staff       (20)     1729 2022-03-11 12:09:04.000000 erpbrasil.assinatura-1.6.0/tests/test_erpbrasil_certificado.py
--rw-r--r--   0 renatolima   (501) staff       (20)     2053 2022-09-07 16:42:03.000000 erpbrasil.assinatura-1.6.0/tests/test_erpbrasil_fake_certificate.py
--rw-r--r--   0 renatolima   (501) staff       (20)     2621 2019-11-15 19:34:04.000000 erpbrasil.assinatura-1.6.0/tests/teste.pfx
-drwxr-xr-x   0 renatolima   (501) staff       (20)        0 2023-01-04 14:16:11.952607 erpbrasil.assinatura-1.6.0/tests/xml/
--rw-r--r--   0 renatolima   (501) staff       (20)    10896 2019-11-15 19:34:04.000000 erpbrasil.assinatura-1.6.0/tests/xml/nfe-400-assinado.xml
--rw-r--r--   0 renatolima   (501) staff       (20)     1976 2021-07-22 15:29:10.000000 erpbrasil.assinatura-1.6.0/tox.ini
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-06-07 13:27:39.000000 erpbrasil.assinatura-1.7.0/
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1424 2023-06-07 13:11:10.000000 erpbrasil.assinatura-1.7.0/.appveyor.yml
+-rw-rw-r--   0 renato    (1000) renato    (1000)      497 2023-06-07 13:16:46.000000 erpbrasil.assinatura-1.7.0/.bumpversion.cfg
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2268 2023-06-07 13:11:10.000000 erpbrasil.assinatura-1.7.0/.cookiecutterrc
+-rw-rw-r--   0 renato    (1000) renato    (1000)      188 2023-06-07 13:11:10.000000 erpbrasil.assinatura-1.7.0/.coveragerc
+-rw-rw-r--   0 renato    (1000) renato    (1000)      215 2023-06-07 13:11:10.000000 erpbrasil.assinatura-1.7.0/.editorconfig
+-rw-rw-r--   0 renato    (1000) renato    (1000)      915 2023-06-07 13:11:10.000000 erpbrasil.assinatura-1.7.0/.travis.yml
+-rw-rw-r--   0 renato    (1000) renato    (1000)       64 2023-06-07 13:11:10.000000 erpbrasil.assinatura-1.7.0/AUTHORS.rst
+-rw-rw-r--   0 renato    (1000) renato    (1000)      900 2023-06-07 13:11:10.000000 erpbrasil.assinatura-1.7.0/CHANGELOG.rst
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2812 2023-06-07 13:11:10.000000 erpbrasil.assinatura-1.7.0/CONTRIBUTING.rst
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1074 2023-06-07 13:11:10.000000 erpbrasil.assinatura-1.7.0/LICENSE
+-rw-rw-r--   0 renato    (1000) renato    (1000)      408 2023-06-07 13:11:10.000000 erpbrasil.assinatura-1.7.0/MANIFEST.in
+-rw-rw-r--   0 renato    (1000) renato    (1000)     3568 2023-06-07 13:27:39.000000 erpbrasil.assinatura-1.7.0/PKG-INFO
+-rw-rw-r--   0 renato    (1000) renato    (1000)     3694 2023-06-07 13:16:46.000000 erpbrasil.assinatura-1.7.0/README.rst
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-06-07 13:27:39.000000 erpbrasil.assinatura-1.7.0/ci/
+-rw-rw-r--   0 renato    (1000) renato    (1000)     3995 2023-06-07 13:11:10.000000 erpbrasil.assinatura-1.7.0/ci/appveyor-bootstrap.py
+-rwxrwxr-x   0 renato    (1000) renato    (1000)     3827 2023-06-07 13:11:10.000000 erpbrasil.assinatura-1.7.0/ci/appveyor-download.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)      763 2023-06-07 13:11:10.000000 erpbrasil.assinatura-1.7.0/ci/appveyor-with-compiler.cmd
+-rwxrwxr-x   0 renato    (1000) renato    (1000)     2097 2023-06-07 13:11:10.000000 erpbrasil.assinatura-1.7.0/ci/bootstrap.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)       50 2023-06-07 13:11:10.000000 erpbrasil.assinatura-1.7.0/ci/requirements.txt
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-06-07 13:27:39.000000 erpbrasil.assinatura-1.7.0/ci/templates/
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1756 2023-06-07 13:11:10.000000 erpbrasil.assinatura-1.7.0/ci/templates/.appveyor.yml
+-rw-rw-r--   0 renato    (1000) renato    (1000)      956 2023-06-07 13:11:10.000000 erpbrasil.assinatura-1.7.0/ci/templates/.travis.yml
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1816 2023-06-07 13:11:10.000000 erpbrasil.assinatura-1.7.0/ci/templates/appveyor.yml
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-06-07 13:27:39.000000 erpbrasil.assinatura-1.7.0/docs/
+-rw-rw-r--   0 renato    (1000) renato    (1000)       28 2023-06-07 13:11:10.000000 erpbrasil.assinatura-1.7.0/docs/authors.rst
+-rw-rw-r--   0 renato    (1000) renato    (1000)       30 2023-06-07 13:11:10.000000 erpbrasil.assinatura-1.7.0/docs/changelog.rst
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1401 2023-06-07 13:16:46.000000 erpbrasil.assinatura-1.7.0/docs/conf.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)       33 2023-06-07 13:11:10.000000 erpbrasil.assinatura-1.7.0/docs/contributing.rst
+-rw-rw-r--   0 renato    (1000) renato    (1000)      245 2023-06-07 13:11:10.000000 erpbrasil.assinatura-1.7.0/docs/index.rst
+-rw-rw-r--   0 renato    (1000) renato    (1000)      100 2023-06-07 13:11:10.000000 erpbrasil.assinatura-1.7.0/docs/installation.rst
+-rw-rw-r--   0 renato    (1000) renato    (1000)       27 2023-06-07 13:11:10.000000 erpbrasil.assinatura-1.7.0/docs/readme.rst
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-06-07 13:27:39.000000 erpbrasil.assinatura-1.7.0/docs/reference/
+-rw-rw-r--   0 renato    (1000) renato    (1000)      140 2023-06-07 13:11:10.000000 erpbrasil.assinatura-1.7.0/docs/reference/edoc_assinatura.rst
+-rw-rw-r--   0 renato    (1000) renato    (1000)       72 2023-06-07 13:11:10.000000 erpbrasil.assinatura-1.7.0/docs/reference/index.rst
+-rw-rw-r--   0 renato    (1000) renato    (1000)       34 2023-06-07 13:11:10.000000 erpbrasil.assinatura-1.7.0/docs/requirements.txt
+-rw-rw-r--   0 renato    (1000) renato    (1000)      109 2023-06-07 13:11:10.000000 erpbrasil.assinatura-1.7.0/docs/spelling_wordlist.txt
+-rw-rw-r--   0 renato    (1000) renato    (1000)       92 2023-06-07 13:11:10.000000 erpbrasil.assinatura-1.7.0/docs/usage.rst
+-rw-rw-r--   0 renato    (1000) renato    (1000)       63 2023-06-07 13:11:10.000000 erpbrasil.assinatura-1.7.0/requirements.txt
+-rw-rw-r--   0 renato    (1000) renato    (1000)      528 2023-06-07 13:27:39.000000 erpbrasil.assinatura-1.7.0/setup.cfg
+-rw-rw-r--   0 renato    (1000) renato    (1000)     3255 2023-06-07 13:16:46.000000 erpbrasil.assinatura-1.7.0/setup.py
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-06-07 13:27:39.000000 erpbrasil.assinatura-1.7.0/src/
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-06-07 13:27:39.000000 erpbrasil.assinatura-1.7.0/src/erpbrasil/
+-rw-rw-r--   0 renato    (1000) renato    (1000)      271 2023-06-07 13:11:10.000000 erpbrasil.assinatura-1.7.0/src/erpbrasil/__init__.py
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-06-07 13:27:39.000000 erpbrasil.assinatura-1.7.0/src/erpbrasil/assinatura/
+-rw-rw-r--   0 renato    (1000) renato    (1000)      222 2023-06-07 13:16:46.000000 erpbrasil.assinatura-1.7.0/src/erpbrasil/assinatura/__init__.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)      404 2023-06-07 13:11:10.000000 erpbrasil.assinatura-1.7.0/src/erpbrasil/assinatura/__main__.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     5883 2023-06-07 13:11:10.000000 erpbrasil.assinatura-1.7.0/src/erpbrasil/assinatura/assinatura.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     4850 2023-06-07 13:11:10.000000 erpbrasil.assinatura-1.7.0/src/erpbrasil/assinatura/certificado.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)      834 2023-06-07 13:11:10.000000 erpbrasil.assinatura-1.7.0/src/erpbrasil/assinatura/cli.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)      333 2023-06-07 13:11:10.000000 erpbrasil.assinatura-1.7.0/src/erpbrasil/assinatura/excecoes.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2400 2023-06-07 13:11:10.000000 erpbrasil.assinatura-1.7.0/src/erpbrasil/assinatura/misc.py
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-06-07 13:27:39.000000 erpbrasil.assinatura-1.7.0/src/erpbrasil.assinatura.egg-info/
+-rw-rw-r--   0 renato    (1000) renato    (1000)     3568 2023-06-07 13:27:39.000000 erpbrasil.assinatura-1.7.0/src/erpbrasil.assinatura.egg-info/PKG-INFO
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1639 2023-06-07 13:27:39.000000 erpbrasil.assinatura-1.7.0/src/erpbrasil.assinatura.egg-info/SOURCES.txt
+-rw-rw-r--   0 renato    (1000) renato    (1000)        1 2023-06-07 13:27:39.000000 erpbrasil.assinatura-1.7.0/src/erpbrasil.assinatura.egg-info/dependency_links.txt
+-rw-rw-r--   0 renato    (1000) renato    (1000)       71 2023-06-07 13:27:39.000000 erpbrasil.assinatura-1.7.0/src/erpbrasil.assinatura.egg-info/entry_points.txt
+-rw-rw-r--   0 renato    (1000) renato    (1000)       10 2023-06-07 13:27:39.000000 erpbrasil.assinatura-1.7.0/src/erpbrasil.assinatura.egg-info/namespace_packages.txt
+-rw-rw-r--   0 renato    (1000) renato    (1000)        1 2023-06-07 13:27:39.000000 erpbrasil.assinatura-1.7.0/src/erpbrasil.assinatura.egg-info/not-zip-safe
+-rw-rw-r--   0 renato    (1000) renato    (1000)       63 2023-06-07 13:27:39.000000 erpbrasil.assinatura-1.7.0/src/erpbrasil.assinatura.egg-info/requires.txt
+-rw-rw-r--   0 renato    (1000) renato    (1000)       10 2023-06-07 13:27:39.000000 erpbrasil.assinatura-1.7.0/src/erpbrasil.assinatura.egg-info/top_level.txt
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-06-07 13:27:39.000000 erpbrasil.assinatura-1.7.0/tests/
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-06-07 13:27:39.000000 erpbrasil.assinatura-1.7.0/tests/files/
+-rw-rw-r--   0 renato    (1000) renato    (1000)    60278 2023-06-07 13:11:10.000000 erpbrasil.assinatura-1.7.0/tests/files/google.pdf
+-rw-rw-r--   0 renato    (1000) renato    (1000)     6015 2023-06-07 13:11:10.000000 erpbrasil.assinatura-1.7.0/tests/files/nfe-400.xml
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-06-07 13:27:39.000000 erpbrasil.assinatura-1.7.0/tests/fixtures/
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2597 2023-06-07 13:11:10.000000 erpbrasil.assinatura-1.7.0/tests/fixtures/dummy_cert.pfx
+-rw-rw-r--   0 renato    (1000) renato    (1000)     3748 2023-06-07 13:11:10.000000 erpbrasil.assinatura-1.7.0/tests/test_erpbrasil_assinatura_pdf.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1512 2023-06-07 13:11:10.000000 erpbrasil.assinatura-1.7.0/tests/test_erpbrasil_assinatura_string.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1122 2023-06-07 13:11:10.000000 erpbrasil.assinatura-1.7.0/tests/test_erpbrasil_assinatura_xml.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1729 2023-06-07 13:11:10.000000 erpbrasil.assinatura-1.7.0/tests/test_erpbrasil_certificado.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2053 2023-06-07 13:11:10.000000 erpbrasil.assinatura-1.7.0/tests/test_erpbrasil_fake_certificate.py
+-rw-rw-r--   0 renato    (1000) renato    (1000)     2621 2023-06-07 13:11:10.000000 erpbrasil.assinatura-1.7.0/tests/teste.pfx
+drwxrwxr-x   0 renato    (1000) renato    (1000)        0 2023-06-07 13:27:39.000000 erpbrasil.assinatura-1.7.0/tests/xml/
+-rw-rw-r--   0 renato    (1000) renato    (1000)    10896 2023-06-07 13:11:10.000000 erpbrasil.assinatura-1.7.0/tests/xml/nfe-400-assinado.xml
+-rw-rw-r--   0 renato    (1000) renato    (1000)     1976 2023-06-07 13:11:10.000000 erpbrasil.assinatura-1.7.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `erpbrasil.assinatura-1.6.0/.appveyor.yml` & `erpbrasil.assinatura-1.7.0/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `erpbrasil.assinatura-1.6.0/.cookiecutterrc` & `erpbrasil.assinatura-1.7.0/.cookiecutterrc`

 * *Files identical despite different names*

### Comparing `erpbrasil.assinatura-1.6.0/.travis.yml` & `erpbrasil.assinatura-1.7.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `erpbrasil.assinatura-1.6.0/CHANGELOG.rst` & `erpbrasil.assinatura-1.7.0/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `erpbrasil.assinatura-1.6.0/CONTRIBUTING.rst` & `erpbrasil.assinatura-1.7.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `erpbrasil.assinatura-1.6.0/LICENSE` & `erpbrasil.assinatura-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `erpbrasil.assinatura-1.6.0/PKG-INFO` & `erpbrasil.assinatura-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erpbrasil.assinatura
-Version: 1.6.0
+Version: 1.7.0
 Summary: Assinatura de documentos com certificados digitais A1 e A3
 Home-page: https://github.com/erpbrasil/erpbrasil.assinatura
 Author: Luis Felipe Mileo
 Author-email: mileo@kmee.com.br
 License: MIT license
 Project-URL: Documentation, https://erpbrasilassinatura.readthedocs.io/en/latest/
 Project-URL: Changelog, https://erpbrasilassinatura.readthedocs.io/en/latest/changelog.html
```

### Comparing `erpbrasil.assinatura-1.6.0/README.rst` & `erpbrasil.assinatura-1.7.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -36,17 +36,17 @@
     :alt: Coverage Status
     :target: https://codecov.io/github/erpbrasil/erpbrasil.assinatura
 
 .. |version| image:: https://img.shields.io/pypi/v/erpbrasil.assinatura.svg
     :alt: PyPI Package latest release
     :target: https://erpbrasilassinatura.readthedocs.io/en/latest/
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/erpbrasil/erpbrasil.assinatura/v1.6.0...svg
+.. |commits-since| image:: https://img.shields.io/github/commits-since/erpbrasil/erpbrasil.assinatura/v1.7.0...svg
     :alt: Commits since latest release
-    :target: https://github.com/erpbrasil/erpbrasil.assinatura/compare/v1.6.0...master
+    :target: https://github.com/erpbrasil/erpbrasil.assinatura/compare/v1.7.0...master
 
 .. |wheel| image:: https://img.shields.io/pypi/wheel/erpbrasil.assinatura.svg
     :alt: PyPI Wheel
     :target: https://pypi.org/project/erpbrasil.assinatura
 
 .. |supported-versions| image:: https://img.shields.io/pypi/pyversions/erpbrasil.assinatura.svg
     :alt: Supported versions
```

### Comparing `erpbrasil.assinatura-1.6.0/ci/appveyor-bootstrap.py` & `erpbrasil.assinatura-1.7.0/ci/appveyor-bootstrap.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.assinatura-1.6.0/ci/appveyor-download.py` & `erpbrasil.assinatura-1.7.0/ci/appveyor-download.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.assinatura-1.6.0/ci/appveyor-with-compiler.cmd` & `erpbrasil.assinatura-1.7.0/ci/appveyor-with-compiler.cmd`

 * *Files identical despite different names*

### Comparing `erpbrasil.assinatura-1.6.0/ci/bootstrap.py` & `erpbrasil.assinatura-1.7.0/ci/bootstrap.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.assinatura-1.6.0/ci/templates/.appveyor.yml` & `erpbrasil.assinatura-1.7.0/ci/templates/.appveyor.yml`

 * *Files identical despite different names*

### Comparing `erpbrasil.assinatura-1.6.0/ci/templates/.travis.yml` & `erpbrasil.assinatura-1.7.0/ci/templates/.travis.yml`

 * *Files identical despite different names*

### Comparing `erpbrasil.assinatura-1.6.0/ci/templates/appveyor.yml` & `erpbrasil.assinatura-1.7.0/ci/templates/appveyor.yml`

 * *Files identical despite different names*

### Comparing `erpbrasil.assinatura-1.6.0/docs/conf.py` & `erpbrasil.assinatura-1.7.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 source_suffix = '.rst'
 master_doc = 'index'
 project = 'erpbrasil.assinatura'
 year = '2019'
 author = 'Luis Felipe Mileo'
 copyright = '{0}, {1}'.format(year, author)
-version = release = '1.6.0'
+version = release = '1.7.0'
 
 pygments_style = 'trac'
 templates_path = ['.']
 extlinks = {
     'issue': ('https://github.com/erpbrasil/erpbrasil.assinatura/issues/%s', '#'),
     'pr': ('https://github.com/erpbrasil/erpbrasil.assinatura/pull/%s', 'PR #'),
 }
```

### Comparing `erpbrasil.assinatura-1.6.0/setup.cfg` & `erpbrasil.assinatura-1.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `erpbrasil.assinatura-1.6.0/setup.py` & `erpbrasil.assinatura-1.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         encoding=kwargs.get('encoding', 'utf8')
     ) as fh:
         return fh.read()
 
 
 setup(
     name='erpbrasil.assinatura',
-    version='1.6.0',
+    version='1.7.0',
     license='MIT license',
     description='Assinatura de documentos com certificados digitais A1 e A3',
     long_description='%s\n%s' % (
         re.compile('^.. start-badges.*^.. end-badges', re.M | re.S).sub('',
                                                                         read(
                                                                             'README.rst')),
         re.sub(':[a-z]+:`~?(.*?)`', r'``\1``', read('CHANGELOG.rst'))
```

### Comparing `erpbrasil.assinatura-1.6.0/src/erpbrasil/assinatura/assinatura.py` & `erpbrasil.assinatura-1.7.0/src/erpbrasil/assinatura/assinatura.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,14 +6,27 @@
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.asymmetric import padding
 from lxml import etree
 
 _logger = logging.getLogger(__name__)
 
 
+class XMLSignerWithSHA1(signxml.XMLSigner):
+    """
+    Extension of the `XMLSigner` class that adds support for the SHA1 hash algorithm
+    to the XML signature process.
+    Note:
+        SHA1-based algorithms are not supported in the default configuration because
+        they are not secure, but in the NF-e project, other more modern algorithms
+        are still not accepted.
+    """
+    def check_deprecated_methods(self):
+        "Override to disable deprecated Check"
+
+
 class Assinatura(object):
 
     def __init__(self, certificado):
         self.certificado = certificado
         self.cert = certificado._cert
         self.chave_privada = certificado._chave
         self.senha = certificado._senha
@@ -44,22 +57,23 @@
         return etree.tostring(signed_root)
 
     def assina_xml2(self, xml_element, reference, getchildren=False):
         for element in xml_element.iter("*"):
             if element.text is not None and not element.text.strip():
                 element.text = None
 
-        signer = signxml.XMLSigner(
+        signer = XMLSignerWithSHA1(
             method=signxml.methods.enveloped,
             signature_algorithm="rsa-sha1",
             digest_algorithm='sha1',
             c14n_algorithm='http://www.w3.org/TR/2001/REC-xml-c14n-20010315'
         )
 
-        signer.namespaces = {"ds": "http://www.w3.org/2000/09/xmldsig#"}
+        signer.excise_empty_xmlns_declarations = True
+        signer.namespaces = {None: signxml.namespaces.ds}
 
         ref_uri = ('#%s' % reference) if reference else None
 
         signed_root = False
         try:
             signed_root = signer.sign(
                 xml_element,
@@ -87,45 +101,63 @@
             elif element_signed is not None and signature is not None:
                 parent = element_signed.getparent()
                 parent.append(signature)
         return etree.tostring(signed_root, encoding=str)
 
     def assina_nfse(self, xml_etree):
 
-        signer = signxml.XMLSigner(
+        signer = XMLSignerWithSHA1(
             method=signxml.methods.enveloped,
             signature_algorithm="rsa-sha1",
             digest_algorithm='sha1',
             c14n_algorithm='http://www.w3.org/TR/2001/REC-xml-c14n-20010315'
         )
 
         signed_root = signer.sign(
             xml_etree,
             key=self.chave_privada,
             cert=self.cert,
         )
-
         signed_root = etree.tostring(signed_root, encoding=str)
 
-        signed_root = signed_root.replace('\r', '').replace('\n', '')
-
         return signed_root
 
     def assina_string(self, message):
         private_key = self.certificado.key
         signature = private_key.sign(
             message,
             padding.PSS(
                 mgf=padding.MGF1(hashes.SHA1()),
                 salt_length=padding.PSS.MAX_LENGTH
             ),
             hashes.SHA1()
         )
         return signature
 
+      
+    def sign_pkcs1v15_sha1(self, data):
+        """
+        Sign data using PKCS1v15 padding and SHA1 hash algorithm.
+
+        This method is specifically tailored for the NFSe Paulistana RPS signing process.
+
+        Args:
+            data (bytes): Data to be signed.
+
+        Returns:
+            bytes: Generated signature.
+        """
+        private_key = self.certificado.key
+        signature = private_key.sign(
+            data,
+            padding.PKCS1v15(),
+            hashes.SHA1()
+        )
+        return signature
+
     def assina_pdf(self, arquivo, dados_assinatura, algoritmo='sha256'):
         try:
             from endesive import pdf
         except ImportError:
             _logger.info(
                 "assina_pdf requires the https://github.com/m32/endesive"
                 "package but it is not bundled by default"
```

### Comparing `erpbrasil.assinatura-1.6.0/src/erpbrasil/assinatura/certificado.py` & `erpbrasil.assinatura-1.7.0/src/erpbrasil/assinatura/certificado.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.assinatura-1.6.0/src/erpbrasil/assinatura/cli.py` & `erpbrasil.assinatura-1.7.0/src/erpbrasil/assinatura/cli.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.assinatura-1.6.0/src/erpbrasil/assinatura/misc.py` & `erpbrasil.assinatura-1.7.0/src/erpbrasil/assinatura/misc.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.assinatura-1.6.0/src/erpbrasil.assinatura.egg-info/PKG-INFO` & `erpbrasil.assinatura-1.7.0/src/erpbrasil.assinatura.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erpbrasil.assinatura
-Version: 1.6.0
+Version: 1.7.0
 Summary: Assinatura de documentos com certificados digitais A1 e A3
 Home-page: https://github.com/erpbrasil/erpbrasil.assinatura
 Author: Luis Felipe Mileo
 Author-email: mileo@kmee.com.br
 License: MIT license
 Project-URL: Documentation, https://erpbrasilassinatura.readthedocs.io/en/latest/
 Project-URL: Changelog, https://erpbrasilassinatura.readthedocs.io/en/latest/changelog.html
```

### Comparing `erpbrasil.assinatura-1.6.0/src/erpbrasil.assinatura.egg-info/SOURCES.txt` & `erpbrasil.assinatura-1.7.0/src/erpbrasil.assinatura.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `erpbrasil.assinatura-1.6.0/tests/files/google.pdf` & `erpbrasil.assinatura-1.7.0/tests/files/google.pdf`

 * *Files identical despite different names*

### Comparing `erpbrasil.assinatura-1.6.0/tests/files/nfe-400.xml` & `erpbrasil.assinatura-1.7.0/tests/files/nfe-400.xml`

 * *Files identical despite different names*

### Comparing `erpbrasil.assinatura-1.6.0/tests/fixtures/dummy_cert.pfx` & `erpbrasil.assinatura-1.7.0/tests/fixtures/dummy_cert.pfx`

 * *Files identical despite different names*

### Comparing `erpbrasil.assinatura-1.6.0/tests/test_erpbrasil_assinatura_pdf.py` & `erpbrasil.assinatura-1.7.0/tests/test_erpbrasil_assinatura_pdf.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.assinatura-1.6.0/tests/test_erpbrasil_assinatura_string.py` & `erpbrasil.assinatura-1.7.0/tests/test_erpbrasil_assinatura_string.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.assinatura-1.6.0/tests/test_erpbrasil_assinatura_xml.py` & `erpbrasil.assinatura-1.7.0/tests/test_erpbrasil_assinatura_xml.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.assinatura-1.6.0/tests/test_erpbrasil_certificado.py` & `erpbrasil.assinatura-1.7.0/tests/test_erpbrasil_certificado.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.assinatura-1.6.0/tests/test_erpbrasil_fake_certificate.py` & `erpbrasil.assinatura-1.7.0/tests/test_erpbrasil_fake_certificate.py`

 * *Files identical despite different names*

### Comparing `erpbrasil.assinatura-1.6.0/tests/teste.pfx` & `erpbrasil.assinatura-1.7.0/tests/teste.pfx`

 * *Files identical despite different names*

### Comparing `erpbrasil.assinatura-1.6.0/tests/xml/nfe-400-assinado.xml` & `erpbrasil.assinatura-1.7.0/tests/xml/nfe-400-assinado.xml`

 * *Files identical despite different names*

### Comparing `erpbrasil.assinatura-1.6.0/tox.ini` & `erpbrasil.assinatura-1.7.0/tox.ini`

 * *Files identical despite different names*

