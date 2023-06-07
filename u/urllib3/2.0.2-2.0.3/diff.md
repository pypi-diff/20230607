# Comparing `tmp/urllib3-2.0.2.tar.gz` & `tmp/urllib3-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Wed May  3 22:26:56 2023, max compression
+gzip compressed data, last modified: Wed Jun  7 10:13:12 2023, max compression
```

## Comparing `urllib3-2.0.2.tar` & `urllib3-2.0.3.tar`

### file list

```diff
@@ -1,119 +1,119 @@
--rw-r--r--   0        0        0    58603 2023-05-03 22:26:56.000000 urllib3-2.0.2/CHANGES.rst
--rw-r--r--   0        0        0      328 2023-05-03 22:26:56.000000 urllib3-2.0.2/dev-requirements.txt
--rw-r--r--   0        0        0     4602 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/Makefile
--rw-r--r--   0        0        0    21359 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/advanced-usage.rst
--rw-r--r--   0        0        0       59 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/changelog.rst
--rw-r--r--   0        0        0     3795 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/conf.py
--rw-r--r--   0        0        0     9500 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/contributing.rst
--rw-r--r--   0        0        0     3836 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/index.rst
--rw-r--r--   0        0        0     4513 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/make.bat
--rw-r--r--   0        0        0       72 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/requirements.txt
--rw-r--r--   0        0        0     1818 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/sponsors.rst
--rw-r--r--   0        0        0    16385 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/user-guide.rst
--rw-r--r--   0        0        0    12502 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/v2-migration-guide.rst
--rw-r--r--   0        0        0     1770 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/_static/banner.svg
--rw-r--r--   0        0        0     3999 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/_static/banner_github.svg
--rw-r--r--   0        0        0     1818 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/_static/dark-logo.svg
--rw-r--r--   0        0        0     7872 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/images/demo-button.png
--rw-r--r--   0        0        0      714 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/images/favicon.png
--rw-r--r--   0        0        0     6226 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/images/learn-more-button.png
--rw-r--r--   0        0        0     2165 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/images/logo.png
--rw-r--r--   0        0        0      516 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/images/logo.svg
--rw-r--r--   0        0        0      226 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/reference/index.rst
--rw-r--r--   0        0        0      316 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/reference/urllib3.connection.rst
--rw-r--r--   0        0        0      408 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/reference/urllib3.connectionpool.rst
--rw-r--r--   0        0        0      185 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/reference/urllib3.exceptions.rst
--rw-r--r--   0        0        0      350 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/reference/urllib3.fields.rst
--rw-r--r--   0        0        0      338 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/reference/urllib3.poolmanager.rst
--rw-r--r--   0        0        0       71 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/reference/urllib3.request.rst
--rw-r--r--   0        0        0      788 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/reference/urllib3.response.rst
--rw-r--r--   0        0        0      555 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/reference/urllib3.util.rst
--rw-r--r--   0        0        0      233 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/reference/contrib/index.rst
--rw-r--r--   0        0        0      295 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/reference/contrib/pyopenssl.rst
--rw-r--r--   0        0        0     1431 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/reference/contrib/securetransport.rst
--rw-r--r--   0        0        0      124 2023-05-03 22:26:56.000000 urllib3-2.0.2/docs/reference/contrib/socks.rst
--rw-r--r--   0        0        0        0 2023-05-03 22:26:56.000000 urllib3-2.0.2/dummyserver/__init__.py
--rw-r--r--   0        0        0    13109 2023-05-03 22:26:56.000000 urllib3-2.0.2/dummyserver/handlers.py
--rwxr-xr-x   0        0        0     1198 2023-05-03 22:26:56.000000 urllib3-2.0.2/dummyserver/https_proxy.py
--rwxr-xr-x   0        0        0     5420 2023-05-03 22:26:56.000000 urllib3-2.0.2/dummyserver/proxy.py
--rwxr-xr-x   0        0        0     9839 2023-05-03 22:26:56.000000 urllib3-2.0.2/dummyserver/server.py
--rw-r--r--   0        0        0    11171 2023-05-03 22:26:56.000000 urllib3-2.0.2/dummyserver/testcase.py
--rw-r--r--   0        0        0      511 2023-05-03 22:26:56.000000 urllib3-2.0.2/dummyserver/certs/README.rst
--rw-r--r--   0        0        0     1679 2023-05-03 22:26:56.000000 urllib3-2.0.2/dummyserver/certs/cacert.key
--rw-r--r--   0        0        0     1273 2023-05-03 22:26:56.000000 urllib3-2.0.2/dummyserver/certs/cacert.pem
--rw-r--r--   0        0        0     1265 2023-05-03 22:26:56.000000 urllib3-2.0.2/dummyserver/certs/server.crt
--rw-r--r--   0        0        0     1679 2023-05-03 22:26:56.000000 urllib3-2.0.2/dummyserver/certs/server.key
--rw-r--r--   0        0        0     5028 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/__init__.py
--rw-r--r--   0        0        0     5651 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/_base_connection.py
--rw-r--r--   0        0        0    15561 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/_collections.py
--rw-r--r--   0        0        0     7756 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/_request_methods.py
--rw-r--r--   0        0        0       98 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/_version.py
--rw-r--r--   0        0        0    33511 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/connection.py
--rw-r--r--   0        0        0    42961 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/connectionpool.py
--rw-r--r--   0        0        0     9289 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/exceptions.py
--rw-r--r--   0        0        0    11026 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/fields.py
--rw-r--r--   0        0        0     2395 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/filepost.py
--rw-r--r--   0        0        0    22160 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/poolmanager.py
--rw-r--r--   0        0        0       93 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/py.typed
--rw-r--r--   0        0        0    39802 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/response.py
--rw-r--r--   0        0        0        0 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/contrib/__init__.py
--rw-r--r--   0        0        0    19437 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/contrib/pyopenssl.py
--rw-r--r--   0        0        0    34121 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/contrib/securetransport.py
--rw-r--r--   0        0        0     7715 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/contrib/socks.py
--rw-r--r--   0        0        0        0 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--   0        0        0    14452 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--   0        0        0    16220 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--   0        0        0     1051 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/util/__init__.py
--rw-r--r--   0        0        0     4462 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/util/connection.py
--rw-r--r--   0        0        0     1148 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/util/proxy.py
--rw-r--r--   0        0        0     8111 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/util/request.py
--rw-r--r--   0        0        0     3374 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/util/response.py
--rw-r--r--   0        0        0    18375 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/util/retry.py
--rw-r--r--   0        0        0    18540 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/util/ssl_.py
--rw-r--r--   0        0        0     5812 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/util/ssl_match_hostname.py
--rw-r--r--   0        0        0     9045 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/util/ssltransport.py
--rw-r--r--   0        0        0    10529 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/util/timeout.py
--rw-r--r--   0        0        0    15213 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/util/url.py
--rw-r--r--   0        0        0     1146 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/util/util.py
--rw-r--r--   0        0        0     4423 2023-05-03 22:26:56.000000 urllib3-2.0.2/src/urllib3/util/wait.py
--rw-r--r--   0        0        0    10763 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/__init__.py
--rw-r--r--   0        0        0    11211 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/conftest.py
--rw-r--r--   0        0        0     6222 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/port_helpers.py
--rw-r--r--   0        0        0    13035 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/test_collections.py
--rw-r--r--   0        0        0      692 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/test_compatibility.py
--rw-r--r--   0        0        0    10737 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/test_connection.py
--rw-r--r--   0        0        0    22772 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/test_connectionpool.py
--rw-r--r--   0        0        0     2164 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/test_exceptions.py
--rw-r--r--   0        0        0     4438 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/test_fields.py
--rw-r--r--   0        0        0     3751 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/test_filepost.py
--rw-r--r--   0        0        0      978 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/test_no_ssl.py
--rw-r--r--   0        0        0    17765 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/test_poolmanager.py
--rw-r--r--   0        0        0     3657 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/test_proxymanager.py
--rw-r--r--   0        0        0      761 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/test_queue_monkeypatch.py
--rw-r--r--   0        0        0    44819 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/test_response.py
--rw-r--r--   0        0        0    16568 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/test_retry.py
--rw-r--r--   0        0        0     7281 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/test_ssl.py
--rw-r--r--   0        0        0    20750 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/test_ssltransport.py
--rw-r--r--   0        0        0    43233 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/test_util.py
--rw-r--r--   0        0        0     5999 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/test_wait.py
--rw-r--r--   0        0        0     1211 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/tz_stub.py
--rw-r--r--   0        0        0        0 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/contrib/__init__.py
--rw-r--r--   0        0        0     1257 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/contrib/duplicate_san.pem
--rw-r--r--   0        0        0     3007 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/contrib/test_pyopenssl.py
--rw-r--r--   0        0        0     1988 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/contrib/test_pyopenssl_dependencies.py
--rw-r--r--   0        0        0     1690 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/contrib/test_securetransport.py
--rw-r--r--   0        0        0    25908 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/contrib/test_socks.py
--rw-r--r--   0        0        0        0 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/with_dummyserver/__init__.py
--rw-r--r--   0        0        0    10678 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/with_dummyserver/test_chunked_transfer.py
--rw-r--r--   0        0        0     3827 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/with_dummyserver/test_connection.py
--rw-r--r--   0        0        0    56860 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/with_dummyserver/test_connectionpool.py
--rw-r--r--   0        0        0    43609 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/with_dummyserver/test_https.py
--rw-r--r--   0        0        0     1104 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/with_dummyserver/test_no_ssl.py
--rw-r--r--   0        0        0    22082 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/with_dummyserver/test_poolmanager.py
--rw-r--r--   0        0        0    33489 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/with_dummyserver/test_proxy_poolmanager.py
--rw-r--r--   0        0        0    85953 2023-05-03 22:26:56.000000 urllib3-2.0.2/test/with_dummyserver/test_socketlevel.py
--rw-r--r--   0        0        0       85 2023-05-03 22:26:56.000000 urllib3-2.0.2/.gitignore
--rw-r--r--   0        0        0     1115 2023-05-03 22:26:56.000000 urllib3-2.0.2/LICENSE.txt
--rw-r--r--   0        0        0     4363 2023-05-03 22:26:56.000000 urllib3-2.0.2/README.md
--rw-r--r--   0        0        0     4069 2023-05-03 22:26:56.000000 urllib3-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     6591 2023-05-03 22:26:56.000000 urllib3-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0    59525 2023-06-07 10:13:12.000000 urllib3-2.0.3/CHANGES.rst
+-rw-r--r--   0        0        0      328 2023-06-07 10:13:12.000000 urllib3-2.0.3/dev-requirements.txt
+-rw-r--r--   0        0        0     4602 2023-06-07 10:13:12.000000 urllib3-2.0.3/docs/Makefile
+-rw-r--r--   0        0        0    21359 2023-06-07 10:13:12.000000 urllib3-2.0.3/docs/advanced-usage.rst
+-rw-r--r--   0        0        0       59 2023-06-07 10:13:12.000000 urllib3-2.0.3/docs/changelog.rst
+-rw-r--r--   0        0        0     4118 2023-06-07 10:13:12.000000 urllib3-2.0.3/docs/conf.py
+-rw-r--r--   0        0        0     9500 2023-06-07 10:13:12.000000 urllib3-2.0.3/docs/contributing.rst
+-rw-r--r--   0        0        0     3836 2023-06-07 10:13:12.000000 urllib3-2.0.3/docs/index.rst
+-rw-r--r--   0        0        0     4513 2023-06-07 10:13:12.000000 urllib3-2.0.3/docs/make.bat
+-rw-r--r--   0        0        0       91 2023-06-07 10:13:12.000000 urllib3-2.0.3/docs/requirements.txt
+-rw-r--r--   0        0        0     1818 2023-06-07 10:13:12.000000 urllib3-2.0.3/docs/sponsors.rst
+-rw-r--r--   0        0        0    16385 2023-06-07 10:13:12.000000 urllib3-2.0.3/docs/user-guide.rst
+-rw-r--r--   0        0        0    17159 2023-06-07 10:13:12.000000 urllib3-2.0.3/docs/v2-migration-guide.rst
+-rw-r--r--   0        0        0     1770 2023-06-07 10:13:12.000000 urllib3-2.0.3/docs/_static/banner.svg
+-rw-r--r--   0        0        0     3999 2023-06-07 10:13:12.000000 urllib3-2.0.3/docs/_static/banner_github.svg
+-rw-r--r--   0        0        0     1818 2023-06-07 10:13:12.000000 urllib3-2.0.3/docs/_static/dark-logo.svg
+-rw-r--r--   0        0        0     7872 2023-06-07 10:13:12.000000 urllib3-2.0.3/docs/images/demo-button.png
+-rw-r--r--   0        0        0      714 2023-06-07 10:13:12.000000 urllib3-2.0.3/docs/images/favicon.png
+-rw-r--r--   0        0        0     6226 2023-06-07 10:13:12.000000 urllib3-2.0.3/docs/images/learn-more-button.png
+-rw-r--r--   0        0        0     2165 2023-06-07 10:13:12.000000 urllib3-2.0.3/docs/images/logo.png
+-rw-r--r--   0        0        0      516 2023-06-07 10:13:12.000000 urllib3-2.0.3/docs/images/logo.svg
+-rw-r--r--   0        0        0      226 2023-06-07 10:13:12.000000 urllib3-2.0.3/docs/reference/index.rst
+-rw-r--r--   0        0        0      352 2023-06-07 10:13:12.000000 urllib3-2.0.3/docs/reference/urllib3.connection.rst
+-rw-r--r--   0        0        0      448 2023-06-07 10:13:12.000000 urllib3-2.0.3/docs/reference/urllib3.connectionpool.rst
+-rw-r--r--   0        0        0      185 2023-06-07 10:13:12.000000 urllib3-2.0.3/docs/reference/urllib3.exceptions.rst
+-rw-r--r--   0        0        0      350 2023-06-07 10:13:12.000000 urllib3-2.0.3/docs/reference/urllib3.fields.rst
+-rw-r--r--   0        0        0      338 2023-06-07 10:13:12.000000 urllib3-2.0.3/docs/reference/urllib3.poolmanager.rst
+-rw-r--r--   0        0        0       71 2023-06-07 10:13:12.000000 urllib3-2.0.3/docs/reference/urllib3.request.rst
+-rw-r--r--   0        0        0      788 2023-06-07 10:13:12.000000 urllib3-2.0.3/docs/reference/urllib3.response.rst
+-rw-r--r--   0        0        0      555 2023-06-07 10:13:12.000000 urllib3-2.0.3/docs/reference/urllib3.util.rst
+-rw-r--r--   0        0        0      233 2023-06-07 10:13:12.000000 urllib3-2.0.3/docs/reference/contrib/index.rst
+-rw-r--r--   0        0        0      295 2023-06-07 10:13:12.000000 urllib3-2.0.3/docs/reference/contrib/pyopenssl.rst
+-rw-r--r--   0        0        0     1431 2023-06-07 10:13:12.000000 urllib3-2.0.3/docs/reference/contrib/securetransport.rst
+-rw-r--r--   0        0        0      124 2023-06-07 10:13:12.000000 urllib3-2.0.3/docs/reference/contrib/socks.rst
+-rw-r--r--   0        0        0        0 2023-06-07 10:13:12.000000 urllib3-2.0.3/dummyserver/__init__.py
+-rw-r--r--   0        0        0    13171 2023-06-07 10:13:12.000000 urllib3-2.0.3/dummyserver/handlers.py
+-rwxr-xr-x   0        0        0     1198 2023-06-07 10:13:12.000000 urllib3-2.0.3/dummyserver/https_proxy.py
+-rwxr-xr-x   0        0        0     4582 2023-06-07 10:13:12.000000 urllib3-2.0.3/dummyserver/proxy.py
+-rwxr-xr-x   0        0        0     9839 2023-06-07 10:13:12.000000 urllib3-2.0.3/dummyserver/server.py
+-rw-r--r--   0        0        0    11171 2023-06-07 10:13:12.000000 urllib3-2.0.3/dummyserver/testcase.py
+-rw-r--r--   0        0        0      511 2023-06-07 10:13:12.000000 urllib3-2.0.3/dummyserver/certs/README.rst
+-rw-r--r--   0        0        0     1679 2023-06-07 10:13:12.000000 urllib3-2.0.3/dummyserver/certs/cacert.key
+-rw-r--r--   0        0        0     1273 2023-06-07 10:13:12.000000 urllib3-2.0.3/dummyserver/certs/cacert.pem
+-rw-r--r--   0        0        0     1265 2023-06-07 10:13:12.000000 urllib3-2.0.3/dummyserver/certs/server.crt
+-rw-r--r--   0        0        0     1679 2023-06-07 10:13:12.000000 urllib3-2.0.3/dummyserver/certs/server.key
+-rw-r--r--   0        0        0     5283 2023-06-07 10:13:12.000000 urllib3-2.0.3/src/urllib3/__init__.py
+-rw-r--r--   0        0        0     5651 2023-06-07 10:13:12.000000 urllib3-2.0.3/src/urllib3/_base_connection.py
+-rw-r--r--   0        0        0    15561 2023-06-07 10:13:12.000000 urllib3-2.0.3/src/urllib3/_collections.py
+-rw-r--r--   0        0        0     7756 2023-06-07 10:13:12.000000 urllib3-2.0.3/src/urllib3/_request_methods.py
+-rw-r--r--   0        0        0       98 2023-06-07 10:13:12.000000 urllib3-2.0.3/src/urllib3/_version.py
+-rw-r--r--   0        0        0    33622 2023-06-07 10:13:12.000000 urllib3-2.0.3/src/urllib3/connection.py
+-rw-r--r--   0        0        0    42961 2023-06-07 10:13:12.000000 urllib3-2.0.3/src/urllib3/connectionpool.py
+-rw-r--r--   0        0        0     9385 2023-06-07 10:13:12.000000 urllib3-2.0.3/src/urllib3/exceptions.py
+-rw-r--r--   0        0        0    11026 2023-06-07 10:13:12.000000 urllib3-2.0.3/src/urllib3/fields.py
+-rw-r--r--   0        0        0     2395 2023-06-07 10:13:12.000000 urllib3-2.0.3/src/urllib3/filepost.py
+-rw-r--r--   0        0        0    22648 2023-06-07 10:13:12.000000 urllib3-2.0.3/src/urllib3/poolmanager.py
+-rw-r--r--   0        0        0       93 2023-06-07 10:13:12.000000 urllib3-2.0.3/src/urllib3/py.typed
+-rw-r--r--   0        0        0    40092 2023-06-07 10:13:12.000000 urllib3-2.0.3/src/urllib3/response.py
+-rw-r--r--   0        0        0        0 2023-06-07 10:13:12.000000 urllib3-2.0.3/src/urllib3/contrib/__init__.py
+-rw-r--r--   0        0        0    19437 2023-06-07 10:13:12.000000 urllib3-2.0.3/src/urllib3/contrib/pyopenssl.py
+-rw-r--r--   0        0        0    34121 2023-06-07 10:13:12.000000 urllib3-2.0.3/src/urllib3/contrib/securetransport.py
+-rw-r--r--   0        0        0     7715 2023-06-07 10:13:12.000000 urllib3-2.0.3/src/urllib3/contrib/socks.py
+-rw-r--r--   0        0        0        0 2023-06-07 10:13:12.000000 urllib3-2.0.3/src/urllib3/contrib/_securetransport/__init__.py
+-rw-r--r--   0        0        0    14452 2023-06-07 10:13:12.000000 urllib3-2.0.3/src/urllib3/contrib/_securetransport/bindings.py
+-rw-r--r--   0        0        0    16220 2023-06-07 10:13:12.000000 urllib3-2.0.3/src/urllib3/contrib/_securetransport/low_level.py
+-rw-r--r--   0        0        0     1051 2023-06-07 10:13:12.000000 urllib3-2.0.3/src/urllib3/util/__init__.py
+-rw-r--r--   0        0        0     4462 2023-06-07 10:13:12.000000 urllib3-2.0.3/src/urllib3/util/connection.py
+-rw-r--r--   0        0        0     1148 2023-06-07 10:13:12.000000 urllib3-2.0.3/src/urllib3/util/proxy.py
+-rw-r--r--   0        0        0     8111 2023-06-07 10:13:12.000000 urllib3-2.0.3/src/urllib3/util/request.py
+-rw-r--r--   0        0        0     3374 2023-06-07 10:13:12.000000 urllib3-2.0.3/src/urllib3/util/response.py
+-rw-r--r--   0        0        0    18374 2023-06-07 10:13:12.000000 urllib3-2.0.3/src/urllib3/util/retry.py
+-rw-r--r--   0        0        0    18860 2023-06-07 10:13:12.000000 urllib3-2.0.3/src/urllib3/util/ssl_.py
+-rw-r--r--   0        0        0     5812 2023-06-07 10:13:12.000000 urllib3-2.0.3/src/urllib3/util/ssl_match_hostname.py
+-rw-r--r--   0        0        0     9045 2023-06-07 10:13:12.000000 urllib3-2.0.3/src/urllib3/util/ssltransport.py
+-rw-r--r--   0        0        0    10529 2023-06-07 10:13:12.000000 urllib3-2.0.3/src/urllib3/util/timeout.py
+-rw-r--r--   0        0        0    15213 2023-06-07 10:13:12.000000 urllib3-2.0.3/src/urllib3/util/url.py
+-rw-r--r--   0        0        0     1146 2023-06-07 10:13:12.000000 urllib3-2.0.3/src/urllib3/util/util.py
+-rw-r--r--   0        0        0     4423 2023-06-07 10:13:12.000000 urllib3-2.0.3/src/urllib3/util/wait.py
+-rw-r--r--   0        0        0    10763 2023-06-07 10:13:12.000000 urllib3-2.0.3/test/__init__.py
+-rw-r--r--   0        0        0    11211 2023-06-07 10:13:12.000000 urllib3-2.0.3/test/conftest.py
+-rw-r--r--   0        0        0     6222 2023-06-07 10:13:12.000000 urllib3-2.0.3/test/port_helpers.py
+-rw-r--r--   0        0        0    13035 2023-06-07 10:13:12.000000 urllib3-2.0.3/test/test_collections.py
+-rw-r--r--   0        0        0      692 2023-06-07 10:13:12.000000 urllib3-2.0.3/test/test_compatibility.py
+-rw-r--r--   0        0        0    10737 2023-06-07 10:13:12.000000 urllib3-2.0.3/test/test_connection.py
+-rw-r--r--   0        0        0    22772 2023-06-07 10:13:12.000000 urllib3-2.0.3/test/test_connectionpool.py
+-rw-r--r--   0        0        0     2164 2023-06-07 10:13:12.000000 urllib3-2.0.3/test/test_exceptions.py
+-rw-r--r--   0        0        0     4438 2023-06-07 10:13:12.000000 urllib3-2.0.3/test/test_fields.py
+-rw-r--r--   0        0        0     3751 2023-06-07 10:13:12.000000 urllib3-2.0.3/test/test_filepost.py
+-rw-r--r--   0        0        0      978 2023-06-07 10:13:12.000000 urllib3-2.0.3/test/test_no_ssl.py
+-rw-r--r--   0        0        0    18464 2023-06-07 10:13:12.000000 urllib3-2.0.3/test/test_poolmanager.py
+-rw-r--r--   0        0        0     3657 2023-06-07 10:13:12.000000 urllib3-2.0.3/test/test_proxymanager.py
+-rw-r--r--   0        0        0      761 2023-06-07 10:13:12.000000 urllib3-2.0.3/test/test_queue_monkeypatch.py
+-rw-r--r--   0        0        0    45439 2023-06-07 10:13:12.000000 urllib3-2.0.3/test/test_response.py
+-rw-r--r--   0        0        0    16568 2023-06-07 10:13:12.000000 urllib3-2.0.3/test/test_retry.py
+-rw-r--r--   0        0        0     7281 2023-06-07 10:13:12.000000 urllib3-2.0.3/test/test_ssl.py
+-rw-r--r--   0        0        0    20750 2023-06-07 10:13:12.000000 urllib3-2.0.3/test/test_ssltransport.py
+-rw-r--r--   0        0        0    43541 2023-06-07 10:13:12.000000 urllib3-2.0.3/test/test_util.py
+-rw-r--r--   0        0        0     5999 2023-06-07 10:13:12.000000 urllib3-2.0.3/test/test_wait.py
+-rw-r--r--   0        0        0     1211 2023-06-07 10:13:12.000000 urllib3-2.0.3/test/tz_stub.py
+-rw-r--r--   0        0        0        0 2023-06-07 10:13:12.000000 urllib3-2.0.3/test/contrib/__init__.py
+-rw-r--r--   0        0        0     1257 2023-06-07 10:13:12.000000 urllib3-2.0.3/test/contrib/duplicate_san.pem
+-rw-r--r--   0        0        0     3007 2023-06-07 10:13:12.000000 urllib3-2.0.3/test/contrib/test_pyopenssl.py
+-rw-r--r--   0        0        0     1988 2023-06-07 10:13:12.000000 urllib3-2.0.3/test/contrib/test_pyopenssl_dependencies.py
+-rw-r--r--   0        0        0     1690 2023-06-07 10:13:12.000000 urllib3-2.0.3/test/contrib/test_securetransport.py
+-rw-r--r--   0        0        0    25908 2023-06-07 10:13:12.000000 urllib3-2.0.3/test/contrib/test_socks.py
+-rw-r--r--   0        0        0        0 2023-06-07 10:13:12.000000 urllib3-2.0.3/test/with_dummyserver/__init__.py
+-rw-r--r--   0        0        0    10678 2023-06-07 10:13:12.000000 urllib3-2.0.3/test/with_dummyserver/test_chunked_transfer.py
+-rw-r--r--   0        0        0     3827 2023-06-07 10:13:12.000000 urllib3-2.0.3/test/with_dummyserver/test_connection.py
+-rw-r--r--   0        0        0    57173 2023-06-07 10:13:12.000000 urllib3-2.0.3/test/with_dummyserver/test_connectionpool.py
+-rw-r--r--   0        0        0    44685 2023-06-07 10:13:12.000000 urllib3-2.0.3/test/with_dummyserver/test_https.py
+-rw-r--r--   0        0        0     1104 2023-06-07 10:13:12.000000 urllib3-2.0.3/test/with_dummyserver/test_no_ssl.py
+-rw-r--r--   0        0        0    22082 2023-06-07 10:13:12.000000 urllib3-2.0.3/test/with_dummyserver/test_poolmanager.py
+-rw-r--r--   0        0        0    33489 2023-06-07 10:13:12.000000 urllib3-2.0.3/test/with_dummyserver/test_proxy_poolmanager.py
+-rw-r--r--   0        0        0    85953 2023-06-07 10:13:12.000000 urllib3-2.0.3/test/with_dummyserver/test_socketlevel.py
+-rw-r--r--   0        0        0       85 2023-06-07 10:13:12.000000 urllib3-2.0.3/.gitignore
+-rw-r--r--   0        0        0     1093 2023-06-07 10:13:12.000000 urllib3-2.0.3/LICENSE.txt
+-rw-r--r--   0        0        0     4363 2023-06-07 10:13:12.000000 urllib3-2.0.3/README.md
+-rw-r--r--   0        0        0     4662 2023-06-07 10:13:12.000000 urllib3-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6591 2023-06-07 10:13:12.000000 urllib3-2.0.3/PKG-INFO
```

### Comparing `urllib3-2.0.2/CHANGES.rst` & `urllib3-2.0.3/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+2.0.3 (2023-06-07)
+==================
+
+- Allowed alternative SSL libraries such as LibreSSL, while still issuing a warning as we cannot help users facing issues with implementations other than OpenSSL. (`#3020 <https://github.com/urllib3/urllib3/issues/3020>`__)
+- Deprecated URLs which don't have an explicit scheme (`#2950 <https://github.com/urllib3/urllib3/pull/2950>`_)
+- Fixed response decoding with Zstandard when compressed data is made of several frames. (`#3008 <https://github.com/urllib3/urllib3/issues/3008>`__)
+- Fixed ``assert_hostname=False`` to correctly skip hostname check. (`#3051 <https://github.com/urllib3/urllib3/issues/3051>`__)
+
+
 2.0.2 (2023-05-03)
 ==================
 
 - Fixed ``HTTPResponse.stream()`` to continue yielding bytes if buffered decompressed data
   was still available to be read even if the underlying socket is closed. This prevents
   a compressed response from being truncated. (`#3009 <https://github.com/urllib3/urllib3/issues/3009>`__)
 
@@ -133,14 +142,20 @@
 * Fixed ``socket.error.errno`` when raised from pyOpenSSL's ``OpenSSL.SSL.SysCallError`` (`#2118 <https://github.com/urllib3/urllib3/issues/2118>`__).
 * Fixed the default value of ``HTTPSConnection.socket_options`` to match ``HTTPConnection`` (`#2213 <https://github.com/urllib3/urllib3/issues/2213>`__).
 * Fixed a bug where ``headers`` would be modified by the ``remove_headers_on_redirect`` feature (`#2272 <https://github.com/urllib3/urllib3/issues/2272>`__).
 * Fixed a reference cycle bug in ``urllib3.util.connection.create_connection()`` (`#2277 <https://github.com/urllib3/urllib3/issues/2277>`__).
 * Fixed a socket leak if ``HTTPConnection.connect()`` fails (`#2571 <https://github.com/urllib3/urllib3/pull/2571>`__).
 * Fixed ``urllib3.contrib.pyopenssl.WrappedSocket`` and ``urllib3.contrib.securetransport.WrappedSocket`` close methods (`#2970 <https://github.com/urllib3/urllib3/issues/2970>`__)
 
+1.26.16 (2023-05-23)
+====================
+
+* Fixed thread-safety issue where accessing a ``PoolManager`` with many distinct origins
+  would cause connection pools to be closed while requests are in progress (`#2954 <https://github.com/urllib3/urllib3/pull/2954>`_)
+
 1.26.15 (2023-03-10)
 ====================
 
 * Fix socket timeout value when ``HTTPConnection`` is reused (`#2645 <https://github.com/urllib3/urllib3/issues/2645>`__)
 * Remove "!" character from the unreserved characters in IPv6 Zone ID parsing
   (`#2899 <https://github.com/urllib3/urllib3/issues/2899>`__)
 * Fix IDNA handling of '\x80' byte (`#2901 <https://github.com/urllib3/urllib3/issues/2901>`__)
```

### Comparing `urllib3-2.0.2/docs/Makefile` & `urllib3-2.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/docs/advanced-usage.rst` & `urllib3-2.0.3/docs/advanced-usage.rst`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/docs/conf.py` & `urllib3-2.0.3/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,16 +31,24 @@
 # Add any Sphinx extension module names here, as strings. They can be extensions
 # coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx_copybutton",
     "sphinx.ext.doctest",
     "sphinx.ext.intersphinx",
+    "sphinxext.opengraph",
 ]
 
+# Open Graph metadata
+ogp_title = "urllib3 documentation"
+ogp_site_url = "https://urllib3.readthedocs.io"
+ogp_type = "website"
+ogp_image = "https://github.com/urllib3/urllib3/raw/main/docs/_static/banner_github.svg"
+ogp_description = "urllib3 is a user-friendly HTTP client library for Python."
+
 # Test code blocks only when explicitly specified
 doctest_test_doctest_blocks = ""
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # The suffix of source filenames.
```

### Comparing `urllib3-2.0.2/docs/contributing.rst` & `urllib3-2.0.3/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/docs/index.rst` & `urllib3-2.0.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/docs/make.bat` & `urllib3-2.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/docs/sponsors.rst` & `urllib3-2.0.3/docs/sponsors.rst`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/docs/user-guide.rst` & `urllib3-2.0.3/docs/user-guide.rst`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/docs/v2-migration-guide.rst` & `urllib3-2.0.3/docs/v2-migration-guide.rst`

 * *Files 15% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 - Removed support for OpenSSL versions older than 1.1.1.
 - Removed support for Python implementations that aren't CPython or PyPy3 (previously supported Google App Engine, Jython).
 - Removed the ``urllib3.contrib.ntlmpool`` module.
 - Deprecated the ``urllib3.contrib.pyopenssl``, ``urllib3.contrib.securetransport`` modules, will be removed in v2.1.0.
 - Deprecated the ``urllib3[secure]`` extra, will be removed in v2.1.0.
 - Deprecated the ``HTTPResponse.getheaders()`` method in favor of ``HTTPResponse.headers``, will be removed in v2.1.0.
 - Deprecated the ``HTTPResponse.getheader(name, default)`` method in favor of ``HTTPResponse.headers.get(name, default)``, will be removed in v2.1.0.
+- Deprecated URLs without a scheme (ie 'https://') and will be raising an error in a future version of urllib3.
 - Changed the default minimum TLS version to TLS 1.2 (previously was TLS 1.0).
 - Removed support for verifying certificate hostnames via ``commonName``, now only ``subjectAltName`` is used.
 - Removed the default set of TLS ciphers, instead now urllib3 uses the list of ciphers configured by the system.
 
 For a full list of changes you can look at `the changelog <https://github.com/urllib3/urllib3/blob/main/CHANGES.rst>`_.
 
 
@@ -148,19 +149,19 @@
 .. code-block:: bash
 
   # From inside your Python environment:
   $ python -m pip install pipdeptree
   # We only care about packages requiring urllib3
   $ pipdeptree --reverse | grep "requires: urllib3"
 
-  - botocore==1.29.8 [requires: urllib3>=1.25.4,<1.27]
-  - requests==2.28.1 [requires: urllib3>=1.21.1,<1.27]
+  - botocore==1.29.8 [requires: urllib3>=1.25.4,<2]
+  - requests==2.28.1 [requires: urllib3>=1.21.1,<2]
 
 Reading the output from above, there are two packages which depend on urllib3: ``botocore`` and ``requests``.
-The versions of these two packages both require urllib3 that is less than v2.0 (ie ``<1.27``).
+The versions of these two packages both require urllib3 that is less than v2.0 (ie ``<2``).
 
 Because both of these packages require urllib3 before v2.0 the new version of urllib3 can't be installed
 by default. There are ways to force installing the newer version of urllib3 v2.0 (ie pinning to ``urllib3==2.0.0``)
 which you can do to test your application.
 
 It's important to know that even if you don't upgrade all of your services to 2.x
 immediately you will `receive security fixes on the 1.26.x release stream <#security-fixes-for-urllib3-v1-26-x>` for some time.
@@ -175,14 +176,97 @@
 
 However, upgrading is still recommended as **no new feature developments or non-critical
 bug fixes will be shipped to the 1.26.x release stream**.
 
 If your organization relies on urllib3 and is interested in continuing support you can learn
 more about the `Tidelift Subscription for Enterprise <https://tidelift.com/subscription/pkg/pypi-urllib3?utm_source=pypi-urllib3&utm_medium=referral&utm_campaign=docs>`_.
 
+**🤔 Common upgrading issues**
+-------------------------------
+
+ssl module is compiled with OpenSSL 1.0.2.k-fips
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. code-block:: text
+
+  ImportError: urllib3 v2.0 only supports OpenSSL 1.1.1+, currently the 'ssl' module is compiled with 'OpenSSL 1.0.2k-fips  26 Jan 2017'.
+  See: https://github.com/urllib3/urllib3/issues/2168
+
+Remediation depends on your system:
+
+- **AWS Lambda**: Upgrade to the Python3.10 runtime as it uses OpenSSL 1.1.1. Alternatively, you can
+  use a `custom Docker image
+  <https://aws.amazon.com/blogs/aws/new-for-aws-lambda-container-image-support/>`_ and ensure you
+  use a Python build that uses OpenSSL 1.1.1 or later.
+- **Amazon Linux 2**: Upgrade to `Amazon Linux 2023
+  <https://aws.amazon.com/linux/amazon-linux-2023/>`_. Alternatively, you can install OpenSSL 1.1.1
+  on Amazon Linux 2 using ``yum install openssl11 openssl11-devel`` and then install Python with a
+  tool like pyenv.
+- **Red Hat Enterpritse Linux 7 (RHEL 7)**: Upgrade to RHEL 8 or RHEL 9.
+- **Read the Docs**: Upgrade your `configuration file to use Ubuntu 22.04
+  <https://docs.readthedocs.io/en/stable/config-file/v2.html>`_ by using ``os: ubuntu-22.04`` in the
+  ``build`` section. Feel free to use the `urllib3 configuration
+  <https://github.com/urllib3/urllib3/blob/2.0.0/.readthedocs.yml>`_ as an inspiration.
+
+docker.errors.dockerexception: error while fetching server api version: request() got an unexpected keyword argument 'chunked'
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Upgrade to ``docker==6.1.0`` that is compatible with urllib3 2.0.
+
+ImportError: cannot import name 'gaecontrib' from 'requests_toolbelt._compat'
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+To be compatible with urllib3 2.0, Requests Toolbelt released version 1.0.0 without Google App
+Engine Standard Python 2.7 support. Most users that reported this issue were using the `Pyrebase
+<https://github.com/thisbejim/Pyrebase>`_ library that provides an API for the Firebase API. This
+library is unmaintained, but `replacements exist
+<https://github.com/thisbejim/Pyrebase/issues/435>`_.
+
+``ImportError: cannot import name 'DEFAULT_CIPHERS' from 'urllib3.util.ssl_'``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+This likely happens because you're using botocore which `does not support urllib3 2.0 yet
+<https://github.com/boto/botocore/issues/2921>`_. The good news is that botocore explicitly declares
+in its dependencies that it only supports ``urllib3<2``. Make sure to use a recent pip. That way, pip
+will install urllib3 1.26.x until botocore starts supporting urllib3 2.0.
+
+If you're deploying to an AWS environment such as Lambda or a host using Amazon Linux 2,
+you'll need to explicitly pin to ``urllib3<2`` in your project to ensure urllib3 2.0 isn't
+brought into your environment. Otherwise, this may result in unintended side effects with
+the default boto3 installation.
+
+AttributeError: module 'urllib3.connectionpool' has no attribute 'VerifiedHTTPSConnection'
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+The ``VerifiedHTTPSConnection`` class has always been documented to be in the
+:mod:`~urllib3.connection` module. It used to be possible to import it from
+:mod:`~urllib3.connectionpool` but that was acccidental and is no longer possible due to a
+refactoring in urllib3 2.0.
+
+Note that the new name of this class is :class:`~urllib3.connection.HTTPSConnection`. It can be used
+starting from urllib3 1.25.9.
+
+AttributeError: 'HTTPResponse' object has no attribute 'strict'
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+The ``strict`` parameter is unneeded with Python 3 and should be removed.
+
+Pinning urllib3<2
+~~~~~~~~~~~~~~~~~
+
+If the advice from the above sections did not help, you can pin urllib3 to 1.26.x by installing
+``urllib3<2``. Please do **not** specify ``urllib3==1.26.15`` to make sure you continue getting
+1.26.x updates!
+
+While urllib3 1.26.x is still supported, it won't get new features or bug fixes, just security
+updates. Consider opening a tracking issue to unpin urllib3 in the future to not stay on 1.26.x
+indefinitely.  For more details on the recommended way to handle your dependencies in general, see
+`Semantic Versioning Will Not Save You <https://hynek.me/articles/semver-will-not-save-you/>`_. The
+second half even uses urllib3 2.0 as an example!
+
 
 **💪 User-friendly features**
 -----------------------------
 
 urllib3 has always billed itself as a **user-friendly HTTP client library**.
 In the spirit of being even more user-friendly we've added two features
 which should make using urllib3 for tinkering sessions, throw-away scripts,
```

### Comparing `urllib3-2.0.2/docs/_static/banner.svg` & `urllib3-2.0.3/docs/_static/banner.svg`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/docs/_static/banner_github.svg` & `urllib3-2.0.3/docs/_static/banner_github.svg`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/docs/_static/dark-logo.svg` & `urllib3-2.0.3/docs/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/docs/images/demo-button.png` & `urllib3-2.0.3/docs/images/demo-button.png`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/docs/images/favicon.png` & `urllib3-2.0.3/docs/images/favicon.png`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/docs/images/learn-more-button.png` & `urllib3-2.0.3/docs/images/learn-more-button.png`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/docs/images/logo.png` & `urllib3-2.0.3/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/docs/images/logo.svg` & `urllib3-2.0.3/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/docs/reference/urllib3.response.rst` & `urllib3-2.0.3/docs/reference/urllib3.response.rst`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/docs/reference/urllib3.util.rst` & `urllib3-2.0.3/docs/reference/urllib3.util.rst`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/docs/reference/contrib/securetransport.rst` & `urllib3-2.0.3/docs/reference/contrib/securetransport.rst`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/dummyserver/handlers.py` & `urllib3-2.0.3/dummyserver/handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import contextlib
 import gzip
 import json
 import logging
 import sys
 import typing
 import zlib
-from datetime import datetime, timedelta
+from datetime import datetime, timedelta, timezone
 from http.client import responses
 from io import BytesIO
 from urllib.parse import urlsplit
 
 from tornado import httputil
 from tornado.web import RequestHandler
 
@@ -340,15 +340,17 @@
 
     def redirect_after(self, request: httputil.HTTPServerRequest) -> Response:
         "Perform a redirect to ``target``"
         params = request_params(request)
         date = params.get("date")
         if date:
             retry_after = str(
-                httputil.format_timestamp(datetime.utcfromtimestamp(float(date)))
+                httputil.format_timestamp(
+                    datetime.fromtimestamp(float(date), tz=timezone.utc)
+                )
             )
         else:
             retry_after = "1"
         target = params.get("target", "/")
         headers = [("Location", target), ("Retry-After", retry_after)]
         return Response(status="303 See Other", headers=headers)
```

### Comparing `urllib3-2.0.2/dummyserver/https_proxy.py` & `urllib3-2.0.3/dummyserver/https_proxy.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/dummyserver/proxy.py` & `urllib3-2.0.3/dummyserver/proxy.py`

 * *Files 12% similar despite different names*

```diff
@@ -41,37 +41,14 @@
 __all__ = ["ProxyHandler", "run_proxy"]
 
 
 class ProxyHandler(tornado.web.RequestHandler):
     SUPPORTED_METHODS = ["GET", "POST", "CONNECT"]  # type: ignore[assignment]
 
     async def get(self) -> None:
-        async def handle_response(response: tornado.httpclient.HTTPResponse) -> None:
-            if response.error and not isinstance(
-                response.error, tornado.httpclient.HTTPError
-            ):
-                self.set_status(500)
-                self.write("Internal server error:\n" + str(response.error))
-                await self.finish()
-            else:
-                self.set_status(response.code)
-                for header in (
-                    "Date",
-                    "Cache-Control",
-                    "Server",
-                    "Content-Type",
-                    "Location",
-                ):
-                    v = response.headers.get(header)
-                    if v:
-                        self.set_header(header, v)
-                if response.body:
-                    self.write(response.body)
-                await self.finish()
-
         upstream_ca_certs = self.application.settings.get("upstream_ca_certs", None)
         ssl_options = None
 
         if upstream_ca_certs:
             ssl_options = ssl.create_default_context(cafile=upstream_ca_certs)
 
         assert self.request.uri is not None
@@ -83,24 +60,29 @@
             headers=self.request.headers,
             follow_redirects=False,
             allow_nonstandard_methods=True,
             ssl_options=ssl_options,
         )
 
         client = tornado.httpclient.AsyncHTTPClient()
-        try:
-            response = await client.fetch(req)
-            await handle_response(response)
-        except tornado.httpclient.HTTPError as e:
-            if hasattr(e, "response") and e.response:
-                await handle_response(e.response)
-            else:
-                self.set_status(500)
-                self.write("Internal server error:\n" + str(e))
-                self.finish()
+        response = await client.fetch(req, raise_error=False)
+        self.set_status(response.code)
+        for header in (
+            "Date",
+            "Cache-Control",
+            "Server",
+            "Content-Type",
+            "Location",
+        ):
+            v = response.headers.get(header)
+            if v:
+                self.set_header(header, v)
+        if response.body:
+            self.write(response.body)
+        await self.finish()
 
     async def post(self) -> None:
         await self.get()
 
     async def connect(self) -> None:
         assert self.request.uri is not None
         host, port = self.request.uri.split(":")
```

### Comparing `urllib3-2.0.2/dummyserver/server.py` & `urllib3-2.0.3/dummyserver/server.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/dummyserver/testcase.py` & `urllib3-2.0.3/dummyserver/testcase.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/dummyserver/certs/cacert.key` & `urllib3-2.0.3/dummyserver/certs/cacert.key`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/dummyserver/certs/cacert.pem` & `urllib3-2.0.3/dummyserver/certs/cacert.pem`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/dummyserver/certs/server.crt` & `urllib3-2.0.3/dummyserver/certs/server.crt`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/dummyserver/certs/server.key` & `urllib3-2.0.3/dummyserver/certs/server.key`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/src/urllib3/__init__.py` & `urllib3-2.0.3/src/urllib3/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,25 +26,27 @@
 # If the 'ssl' module isn't available at all that's
 # fine, we only care if the module is available.
 try:
     import ssl
 except ImportError:
     pass
 else:
-    # fmt: off
-    if (
-        not ssl.OPENSSL_VERSION.startswith("OpenSSL ")
-        or ssl.OPENSSL_VERSION_INFO < (1, 1, 1)
-    ):  # Defensive:
+    if not ssl.OPENSSL_VERSION.startswith("OpenSSL "):  # Defensive:
+        warnings.warn(
+            "urllib3 v2.0 only supports OpenSSL 1.1.1+, currently "
+            f"the 'ssl' module is compiled with {ssl.OPENSSL_VERSION!r}. "
+            "See: https://github.com/urllib3/urllib3/issues/3020",
+            exceptions.NotOpenSSLWarning,
+        )
+    elif ssl.OPENSSL_VERSION_INFO < (1, 1, 1):  # Defensive:
         raise ImportError(
             "urllib3 v2.0 only supports OpenSSL 1.1.1+, currently "
-            f"the 'ssl' module is compiled with {ssl.OPENSSL_VERSION}. "
+            f"the 'ssl' module is compiled with {ssl.OPENSSL_VERSION!r}. "
             "See: https://github.com/urllib3/urllib3/issues/2168"
         )
-    # fmt: on
 
 # === NOTE TO REPACKAGERS AND VENDORS ===
 # Please delete this block, this logic is only
 # for urllib3 being distributed via PyPI.
 # See: https://github.com/urllib3/urllib3/issues/2680
 try:
     import urllib3_secure_extra  # type: ignore # noqa: F401
```

### Comparing `urllib3-2.0.2/src/urllib3/_base_connection.py` & `urllib3-2.0.3/src/urllib3/_base_connection.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/src/urllib3/_collections.py` & `urllib3-2.0.3/src/urllib3/_collections.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/src/urllib3/_request_methods.py` & `urllib3-2.0.3/src/urllib3/_request_methods.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/src/urllib3/connection.py` & `urllib3-2.0.3/src/urllib3/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -737,14 +737,16 @@
     context.verify_mode = resolve_cert_reqs(cert_reqs)
 
     # In some cases, we want to verify hostnames ourselves
     if (
         # `ssl` can't verify fingerprints or alternate hostnames
         assert_fingerprint
         or assert_hostname
+        # assert_hostname can be set to False to disable hostname checking
+        or assert_hostname is False
         # We still support OpenSSL 1.0.2, which prevents us from verifying
         # hostnames easily: https://github.com/pyca/pyopenssl/pull/933
         or ssl_.IS_PYOPENSSL
         or not ssl_.HAS_NEVER_CHECK_COMMON_NAME
     ):
         context.check_hostname = False
```

### Comparing `urllib3-2.0.2/src/urllib3/connectionpool.py` & `urllib3-2.0.3/src/urllib3/connectionpool.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/src/urllib3/exceptions.py` & `urllib3-2.0.3/src/urllib3/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,14 +210,18 @@
     """Warned when performing security reducing actions"""
 
 
 class InsecureRequestWarning(SecurityWarning):
     """Warned when making an unverified HTTPS request."""
 
 
+class NotOpenSSLWarning(SecurityWarning):
+    """Warned when using unsupported SSL library"""
+
+
 class SystemTimeWarning(SecurityWarning):
     """Warned when system time is suspected to be wrong"""
 
 
 class InsecurePlatformWarning(SecurityWarning):
     """Warned when certain TLS/SSL configuration is not available on a platform."""
```

### Comparing `urllib3-2.0.2/src/urllib3/fields.py` & `urllib3-2.0.3/src/urllib3/fields.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/src/urllib3/filepost.py` & `urllib3-2.0.3/src/urllib3/filepost.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/src/urllib3/poolmanager.py` & `urllib3-2.0.3/src/urllib3/poolmanager.py`

 * *Files 2% similar despite different names*

```diff
@@ -415,14 +415,24 @@
         portion of the ``url``.
 
         The given ``url`` parameter must be absolute, such that an appropriate
         :class:`urllib3.connectionpool.ConnectionPool` can be chosen for it.
         """
         u = parse_url(url)
 
+        if u.scheme is None:
+            warnings.warn(
+                "URLs without a scheme (ie 'https://') are deprecated and will raise an error "
+                "in a future version of urllib3. To avoid this DeprecationWarning ensure all URLs "
+                "start with 'https://' or 'http://'. Read more in this issue: "
+                "https://github.com/urllib3/urllib3/issues/2920",
+                category=DeprecationWarning,
+                stacklevel=2,
+            )
+
         conn = self.connection_from_host(u.host, port=u.port, scheme=u.scheme)
 
         kw["assert_same_host"] = False
         kw["redirect"] = False
 
         if "headers" not in kw:
             kw["headers"] = self.headers
```

### Comparing `urllib3-2.0.2/src/urllib3/response.py` & `urllib3-2.0.3/src/urllib3/response.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,18 +165,23 @@
     class ZstdDecoder(ContentDecoder):
         def __init__(self) -> None:
             self._obj = zstd.ZstdDecompressor().decompressobj()
 
         def decompress(self, data: bytes) -> bytes:
             if not data:
                 return b""
-            return self._obj.decompress(data)  # type: ignore[no-any-return]
+            data_parts = [self._obj.decompress(data)]
+            while self._obj.eof and self._obj.unused_data:
+                unused_data = self._obj.unused_data
+                self._obj = zstd.ZstdDecompressor().decompressobj()
+                data_parts.append(self._obj.decompress(unused_data))
+            return b"".join(data_parts)
 
         def flush(self) -> bytes:
-            ret = self._obj.flush()
+            ret = self._obj.flush()  # note: this is a no-op
             if not self._obj.eof:
                 raise DecodeError("Zstandard data is incomplete")
             return ret  # type: ignore[no-any-return]
 
 
 class MultiDecoder(ContentDecoder):
     """
```

### Comparing `urllib3-2.0.2/src/urllib3/contrib/pyopenssl.py` & `urllib3-2.0.3/src/urllib3/contrib/pyopenssl.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/src/urllib3/contrib/securetransport.py` & `urllib3-2.0.3/src/urllib3/contrib/securetransport.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/src/urllib3/contrib/socks.py` & `urllib3-2.0.3/src/urllib3/contrib/socks.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/src/urllib3/contrib/_securetransport/bindings.py` & `urllib3-2.0.3/src/urllib3/contrib/_securetransport/bindings.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/src/urllib3/contrib/_securetransport/low_level.py` & `urllib3-2.0.3/src/urllib3/contrib/_securetransport/low_level.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/src/urllib3/util/__init__.py` & `urllib3-2.0.3/src/urllib3/util/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/src/urllib3/util/connection.py` & `urllib3-2.0.3/src/urllib3/util/connection.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/src/urllib3/util/proxy.py` & `urllib3-2.0.3/src/urllib3/util/proxy.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/src/urllib3/util/request.py` & `urllib3-2.0.3/src/urllib3/util/request.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/src/urllib3/util/response.py` & `urllib3-2.0.3/src/urllib3/util/response.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/src/urllib3/util/retry.py` & `urllib3-2.0.3/src/urllib3/util/retry.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,15 @@
         By default, this is disabled with ``None``.
 
     :param float backoff_factor:
         A backoff factor to apply between attempts after the second try
         (most errors are resolved immediately by a second try without a
         delay). urllib3 will sleep for::
 
-            {backoff factor} * (2 ** ({number of total retries} - 1))
+            {backoff factor} * (2 ** ({number of previous retries}))
 
         seconds. If `backoff_jitter` is non-zero, this sleep is extended by::
 
             random.uniform(0, {backoff jitter})
 
         seconds. For example, if the backoff_factor is 0.1, then :func:`Retry.sleep` will
         sleep for [0.0s, 0.2s, 0.4s, 0.8s, ...] between retries. No backoff will ever
```

### Comparing `urllib3-2.0.2/src/urllib3/util/ssl_.py` & `urllib3-2.0.3/src/urllib3/util/ssl_.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,26 +51,31 @@
         (major_minor == (3, 8) and micro >= 9)
         or (major_minor == (3, 9) and micro >= 3)
         or major_minor >= (3, 10)
     )
 
 
 def _is_has_never_check_common_name_reliable(
+    openssl_version: str,
     openssl_version_number: int,
     implementation_name: str,
     version_info: _TYPE_VERSION_INFO,
 ) -> bool:
+    # As of May 2023, all released versions of LibreSSL fail to reject certificates with
+    # only common names, see https://github.com/urllib3/urllib3/pull/3024
+    is_openssl = openssl_version.startswith("OpenSSL ")
     # Before fixing OpenSSL issue #14579, the SSL_new() API was not copying hostflags
     # like X509_CHECK_FLAG_NEVER_CHECK_SUBJECT, which tripped up CPython.
     # https://github.com/openssl/openssl/issues/14579
     # This was released in OpenSSL 1.1.1l+ (>=0x101010cf)
     is_openssl_issue_14579_fixed = openssl_version_number >= 0x101010CF
 
-    return is_openssl_issue_14579_fixed or _is_bpo_43522_fixed(
-        implementation_name, version_info
+    return is_openssl and (
+        is_openssl_issue_14579_fixed
+        or _is_bpo_43522_fixed(implementation_name, version_info)
     )
 
 
 if typing.TYPE_CHECKING:
     from ssl import VerifyMode
 
     from typing_extensions import Literal, TypedDict
@@ -89,28 +94,30 @@
 try:  # Do we have ssl at all?
     import ssl
     from ssl import (  # type: ignore[assignment]
         CERT_REQUIRED,
         HAS_NEVER_CHECK_COMMON_NAME,
         OP_NO_COMPRESSION,
         OP_NO_TICKET,
+        OPENSSL_VERSION,
         OPENSSL_VERSION_NUMBER,
         PROTOCOL_TLS,
         PROTOCOL_TLS_CLIENT,
         OP_NO_SSLv2,
         OP_NO_SSLv3,
         SSLContext,
         TLSVersion,
     )
 
     PROTOCOL_SSLv23 = PROTOCOL_TLS
 
     # Setting SSLContext.hostname_checks_common_name = False didn't work before CPython
     # 3.8.9, 3.9.3, and 3.10 (but OK on PyPy) or OpenSSL 1.1.1l+
     if HAS_NEVER_CHECK_COMMON_NAME and not _is_has_never_check_common_name_reliable(
+        OPENSSL_VERSION,
         OPENSSL_VERSION_NUMBER,
         sys.implementation.name,
         sys.version_info,
     ):
         HAS_NEVER_CHECK_COMMON_NAME = False
 
     # Need to be careful here in case old TLS versions get
```

### Comparing `urllib3-2.0.2/src/urllib3/util/ssl_match_hostname.py` & `urllib3-2.0.3/src/urllib3/util/ssl_match_hostname.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/src/urllib3/util/ssltransport.py` & `urllib3-2.0.3/src/urllib3/util/ssltransport.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/src/urllib3/util/timeout.py` & `urllib3-2.0.3/src/urllib3/util/timeout.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/src/urllib3/util/url.py` & `urllib3-2.0.3/src/urllib3/util/url.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/src/urllib3/util/util.py` & `urllib3-2.0.3/src/urllib3/util/util.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/src/urllib3/util/wait.py` & `urllib3-2.0.3/src/urllib3/util/wait.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/test/__init__.py` & `urllib3-2.0.3/test/__init__.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/test/conftest.py` & `urllib3-2.0.3/test/conftest.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/test/port_helpers.py` & `urllib3-2.0.3/test/port_helpers.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/test/test_collections.py` & `urllib3-2.0.3/test/test_collections.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/test/test_compatibility.py` & `urllib3-2.0.3/test/test_compatibility.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/test/test_connection.py` & `urllib3-2.0.3/test/test_connection.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/test/test_connectionpool.py` & `urllib3-2.0.3/test/test_connectionpool.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/test/test_exceptions.py` & `urllib3-2.0.3/test/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/test/test_fields.py` & `urllib3-2.0.3/test/test_fields.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/test/test_filepost.py` & `urllib3-2.0.3/test/test_filepost.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/test/test_no_ssl.py` & `urllib3-2.0.3/test/test_no_ssl.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/test/test_poolmanager.py` & `urllib3-2.0.3/test/test_poolmanager.py`

 * *Files 5% similar despite different names*

```diff
@@ -255,14 +255,31 @@
         pool = p.connection_from_context(context)
         other_pool = p.connection_from_context(other_context)
 
         assert 1 == len(p.pools)
         assert pool is other_pool
         assert all(isinstance(key, PoolKey) for key in p.pools.keys())
 
+    def test_deprecated_no_scheme(self) -> None:
+        p = PoolManager()
+
+        with pytest.warns(DeprecationWarning) as records:
+            p.request(method="GET", url="evil.com://good.com")
+
+        msg = (
+            "URLs without a scheme (ie 'https://') are deprecated and will raise an error "
+            "in a future version of urllib3. To avoid this DeprecationWarning ensure all URLs "
+            "start with 'https://' or 'http://'. Read more in this issue: "
+            "https://github.com/urllib3/urllib3/issues/2920"
+        )
+
+        assert len(records) == 1
+        assert isinstance(records[0].message, DeprecationWarning)
+        assert records[0].message.args[0] == msg
+
     @patch("urllib3.poolmanager.PoolManager.connection_from_pool_key")
     def test_connection_from_context_strict_param(
         self, connection_from_pool_key: mock.MagicMock
     ) -> None:
         p = PoolManager()
         context = {
             "scheme": "http",
```

### Comparing `urllib3-2.0.2/test/test_proxymanager.py` & `urllib3-2.0.3/test/test_proxymanager.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/test/test_queue_monkeypatch.py` & `urllib3-2.0.3/test/test_queue_monkeypatch.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/test/test_response.py` & `urllib3-2.0.3/test/test_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -329,14 +329,33 @@
         data = zstd.compress(b"foo")
 
         fp = BytesIO(data)
         r = HTTPResponse(fp, headers={"content-encoding": "zstd"})
         assert r.data == b"foo"
 
     @onlyZstd()
+    def test_decode_multiframe_zstd(self) -> None:
+        data = (
+            # Zstandard frame
+            zstd.compress(b"foo")
+            # skippable frame (must be ignored)
+            + bytes.fromhex(
+                "50 2A 4D 18"  # Magic_Number (little-endian)
+                "07 00 00 00"  # Frame_Size (little-endian)
+                "00 00 00 00 00 00 00"  # User_Data
+            )
+            # Zstandard frame
+            + zstd.compress(b"bar")
+        )
+
+        fp = BytesIO(data)
+        r = HTTPResponse(fp, headers={"content-encoding": "zstd"})
+        assert r.data == b"foobar"
+
+    @onlyZstd()
     def test_chunked_decoding_zstd(self) -> None:
         data = zstd.compress(b"foobarbaz")
 
         fp = BytesIO(data)
         r = HTTPResponse(
             fp, headers={"content-encoding": "zstd"}, preload_content=False
         )
```

### Comparing `urllib3-2.0.2/test/test_retry.py` & `urllib3-2.0.3/test/test_retry.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/test/test_ssl.py` & `urllib3-2.0.3/test/test_ssl.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/test/test_ssltransport.py` & `urllib3-2.0.3/test/test_ssltransport.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/test/test_util.py` & `urllib3-2.0.3/test/test_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1064,36 +1064,40 @@
         """Test that a warning is not made if server_hostname is not given."""
         sock = Mock()
         context, warn = self._wrap_socket_and_mock_warn(sock, None)
         context.wrap_socket.assert_called_once_with(sock, server_hostname=None)
         warn.assert_not_called()
 
     @pytest.mark.parametrize(
-        "openssl_version_number, implementation_name, version_info, reliable",
+        "openssl_version, openssl_version_number, implementation_name, version_info, reliable",
         [
             # OpenSSL and Python OK -> reliable
-            (0x101010CF, "cpython", (3, 9, 3), True),
+            ("OpenSSL 1.1.1", 0x101010CF, "cpython", (3, 9, 3), True),
             # Python OK -> reliable
-            (0x10101000, "cpython", (3, 9, 3), True),
-            (0x10101000, "pypy", (3, 6, 9), False),
+            ("OpenSSL 1.1.1", 0x10101000, "cpython", (3, 9, 3), True),
+            ("OpenSSL 1.1.1", 0x10101000, "pypy", (3, 6, 9), False),
             # OpenSSL OK -> reliable
-            (0x101010CF, "cpython", (3, 9, 2), True),
-            # unreliable
-            (0x10101000, "cpython", (3, 9, 2), False),
+            ("OpenSSL 1.1.1", 0x101010CF, "cpython", (3, 9, 2), True),
+            # not OpenSSSL -> unreliable
+            ("LibreSSL 2.8.3", 0x101010CF, "cpython", (3, 10, 0), False),
+            # old OpenSSL and old Python, unreliable
+            ("OpenSSL 1.1.0", 0x10101000, "cpython", (3, 9, 2), False),
         ],
     )
     def test_is_has_never_check_common_name_reliable(
         self,
+        openssl_version: str,
         openssl_version_number: int,
         implementation_name: str,
         version_info: _TYPE_VERSION_INFO,
         reliable: bool,
     ) -> None:
         assert (
             _is_has_never_check_common_name_reliable(
+                openssl_version,
                 openssl_version_number,
                 implementation_name,
                 version_info,
             )
             == reliable
         )
```

### Comparing `urllib3-2.0.2/test/test_wait.py` & `urllib3-2.0.3/test/test_wait.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/test/tz_stub.py` & `urllib3-2.0.3/test/tz_stub.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/test/contrib/duplicate_san.pem` & `urllib3-2.0.3/test/contrib/duplicate_san.pem`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/test/contrib/test_pyopenssl.py` & `urllib3-2.0.3/test/contrib/test_pyopenssl.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/test/contrib/test_pyopenssl_dependencies.py` & `urllib3-2.0.3/test/contrib/test_pyopenssl_dependencies.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/test/contrib/test_securetransport.py` & `urllib3-2.0.3/test/contrib/test_securetransport.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/test/contrib/test_socks.py` & `urllib3-2.0.3/test/contrib/test_socks.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/test/with_dummyserver/test_chunked_transfer.py` & `urllib3-2.0.3/test/with_dummyserver/test_chunked_transfer.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/test/with_dummyserver/test_connection.py` & `urllib3-2.0.3/test/with_dummyserver/test_connection.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/test/with_dummyserver/test_connectionpool.py` & `urllib3-2.0.3/test/with_dummyserver/test_connectionpool.py`

 * *Files 0% similar despite different names*

```diff
@@ -461,14 +461,20 @@
                     conn, "_tunnel", create=True, return_value=None
                 ) as conn_tunnel:
                     pool._make_request(conn, "GET", "/")
                 assert not conn_tunnel.called
             finally:
                 conn.close()
 
+    def test_redirect_relative_url_no_deprecation(self) -> None:
+        with HTTPConnectionPool(self.host, self.port) as pool:
+            with warnings.catch_warnings():
+                warnings.simplefilter("error", DeprecationWarning)
+                pool.request("GET", "/redirect", fields={"target": "/"})
+
     def test_redirect(self) -> None:
         with HTTPConnectionPool(self.host, self.port) as pool:
             r = pool.request("GET", "/redirect", fields={"target": "/"}, redirect=False)
             assert r.status == 303
 
             r = pool.request("GET", "/redirect", fields={"target": "/"})
             assert r.status == 200
```

### Comparing `urllib3-2.0.2/test/with_dummyserver/test_https.py` & `urllib3-2.0.3/test/with_dummyserver/test_https.py`

 * *Files 1% similar despite different names*

```diff
@@ -1113,14 +1113,40 @@
         else:
             assert err is not None
             assert type(err.reason) == SSLError
             assert isinstance(
                 err.reason.args[0], (ssl.SSLCertVerificationError, CertificateError)
             )
 
+    def test_assert_hostname_invalid_san(
+        self, no_localhost_san_server: ServerConfig
+    ) -> None:
+        """Ensure SAN errors are not raised while assert_hostname is false"""
+        with HTTPSConnectionPool(
+            no_localhost_san_server.host,
+            no_localhost_san_server.port,
+            cert_reqs="CERT_REQUIRED",
+            ca_certs=no_localhost_san_server.ca_certs,
+            assert_hostname=False,
+        ) as https_pool:
+            https_pool.request("GET", "/")
+
+    def test_assert_hostname_invalid_cn(
+        self, no_san_server_with_different_commmon_name: ServerConfig
+    ) -> None:
+        """Ensure CN errors are not raised while assert_hostname is false"""
+        with HTTPSConnectionPool(
+            no_san_server_with_different_commmon_name.host,
+            no_san_server_with_different_commmon_name.port,
+            cert_reqs="CERT_REQUIRED",
+            ca_certs=no_san_server_with_different_commmon_name.ca_certs,
+            assert_hostname=False,
+        ) as https_pool:
+            https_pool.request("GET", "/")
+
 
 class TestHTTPS_IPV4SAN:
     def test_can_validate_ip_san(self, ipv4_san_server: ServerConfig) -> None:
         """Ensure that urllib3 can validate SANs with IP addresses in them."""
         with HTTPSConnectionPool(
             ipv4_san_server.host,
             ipv4_san_server.port,
```

### Comparing `urllib3-2.0.2/test/with_dummyserver/test_no_ssl.py` & `urllib3-2.0.3/test/with_dummyserver/test_no_ssl.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/test/with_dummyserver/test_poolmanager.py` & `urllib3-2.0.3/test/with_dummyserver/test_poolmanager.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/test/with_dummyserver/test_proxy_poolmanager.py` & `urllib3-2.0.3/test/with_dummyserver/test_proxy_poolmanager.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/test/with_dummyserver/test_socketlevel.py` & `urllib3-2.0.3/test/with_dummyserver/test_socketlevel.py`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/LICENSE.txt` & `urllib3-2.0.3/LICENSE.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2008-2020 Andrey Petrov and contributors (see CONTRIBUTORS.txt)
+Copyright (c) 2008-2020 Andrey Petrov and contributors.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `urllib3-2.0.2/README.md` & `urllib3-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `urllib3-2.0.2/pyproject.toml` & `urllib3-2.0.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -81,27 +81,33 @@
 [tool.pytest.ini_options]
 xfail_strict = true
 python_classes = ["Test", "*TestCase"]
 markers = ["limit_memory"]
 log_level = "DEBUG"
 filterwarnings = [
     "error",
+    '''default:urllib3 v2.0 only supports OpenSSL 1.1.1+.*''',
     '''default:'urllib3\[secure\]' extra is deprecated and will be removed in urllib3 v2\.1\.0.*:DeprecationWarning''',
     '''default:'urllib3\.contrib\.pyopenssl' module is deprecated and will be removed in urllib3 v2\.1\.0.*:DeprecationWarning''',
     '''default:'urllib3\.contrib\.securetransport' module is deprecated and will be removed in urllib3 v2\.1\.0.*:DeprecationWarning''',
     '''default:No IPv6 support. Falling back to IPv4:urllib3.exceptions.HTTPWarning''',
     '''default:No IPv6 support. skipping:urllib3.exceptions.HTTPWarning''',
     '''default:ssl\.TLSVersion\.TLSv1 is deprecated:DeprecationWarning''',
     '''default:ssl\.PROTOCOL_TLS is deprecated:DeprecationWarning''',
     '''default:ssl\.PROTOCOL_TLSv1 is deprecated:DeprecationWarning''',
     '''default:ssl\.TLSVersion\.TLSv1_1 is deprecated:DeprecationWarning''',
     '''default:ssl\.PROTOCOL_TLSv1_1 is deprecated:DeprecationWarning''',
     '''default:ssl\.PROTOCOL_TLSv1_2 is deprecated:DeprecationWarning''',
     '''default:unclosed .*:ResourceWarning''',
     '''default:ssl NPN is deprecated, use ALPN instead:DeprecationWarning''',
+    # https://github.com/pytest-dev/pytest/issues/10977
+    '''default:ast\.(Num|NameConstant|Str) is deprecated and will be removed in Python 3\.14; use ast\.Constant instead:DeprecationWarning:_pytest''',
+    '''default:Attribute s is deprecated and will be removed in Python 3\.14; use value instead:DeprecationWarning:_pytest''',
+    # https://github.com/dateutil/dateutil/issues/1284
+    '''default:datetime\.utcfromtimestamp\(\) is deprecated and scheduled for removal in a future version\.*:DeprecationWarning:dateutil''',
 ]
 
 [tool.isort]
 profile = "black"
 add_imports = "from __future__ import annotations"
 
 [tool.mypy]
```

### Comparing `urllib3-2.0.2/PKG-INFO` & `urllib3-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urllib3
-Version: 2.0.2
+Version: 2.0.3
 Summary: HTTP library with thread-safe connection pooling, file post, and more.
 Project-URL: Changelog, https://github.com/urllib3/urllib3/blob/main/CHANGES.rst
 Project-URL: Documentation, https://urllib3.readthedocs.io
 Project-URL: Code, https://github.com/urllib3/urllib3
 Project-URL: Issue tracker, https://github.com/urllib3/urllib3/issues
 Author-email: Andrey Petrov <andrey.petrov@shazow.net>
 Maintainer-email: Seth Michael Larson <sethmichaellarson@gmail.com>, Quentin Pradet <quentin@pradet.me>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: urllib3 Version: 2.0.2 Summary: HTTP library with
+Metadata-Version: 2.1 Name: urllib3 Version: 2.0.3 Summary: HTTP library with
 thread-safe connection pooling, file post, and more. Project-URL: Changelog,
 https://github.com/urllib3/urllib3/blob/main/CHANGES.rst Project-URL:
 Documentation, https://urllib3.readthedocs.io Project-URL: Code, https://
 github.com/urllib3/urllib3 Project-URL: Issue tracker, https://github.com/
 urllib3/urllib3/issues Author-email: Andrey Petrov
 petrov@shazow.net> Maintainer-email: Seth Michael Larson
 gmail.com>, Quentin Pradet
```

