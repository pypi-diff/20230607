# Comparing `tmp/eth-typing-3.3.0.tar.gz` & `tmp/eth-typing-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eth-typing-3.3.0.tar", last modified: Wed Mar  8 18:06:46 2023, max compression
+gzip compressed data, was "eth-typing-3.4.0.tar", last modified: Wed Jun  7 21:41:25 2023, max compression
```

## Comparing `eth-typing-3.3.0.tar` & `eth-typing-3.4.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-03-08 18:06:46.577755 eth-typing-3.3.0/
--rw-r--r--   0 eve        (501) staff       (20)     1090 2021-11-05 21:32:29.000000 eth-typing-3.3.0/LICENSE
--rw-r--r--   0 eve        (501) staff       (20)      137 2021-11-05 21:32:29.000000 eth-typing-3.3.0/MANIFEST.in
--rw-r--r--   0 eve        (501) staff       (20)     4215 2023-03-08 18:06:46.577629 eth-typing-3.3.0/PKG-INFO
--rw-r--r--   0 eve        (501) staff       (20)     3198 2021-11-05 21:32:29.000000 eth-typing-3.3.0/README.md
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-03-08 18:06:46.576900 eth-typing-3.3.0/eth_typing/
--rw-r--r--   0 eve        (501) staff       (20)      803 2022-06-22 17:47:19.000000 eth-typing-3.3.0/eth_typing/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)       85 2021-11-05 21:32:29.000000 eth-typing-3.3.0/eth_typing/abi.py
--rw-r--r--   0 eve        (501) staff       (20)      191 2022-06-22 17:47:19.000000 eth-typing-3.3.0/eth_typing/bls.py
--rw-r--r--   0 eve        (501) staff       (20)       71 2022-01-21 20:17:43.000000 eth-typing-3.3.0/eth_typing/discovery.py
--rw-r--r--   0 eve        (501) staff       (20)      117 2021-11-05 21:32:29.000000 eth-typing-3.3.0/eth_typing/encoding.py
--rw-r--r--   0 eve        (501) staff       (20)      436 2023-03-08 17:58:11.000000 eth-typing-3.3.0/eth_typing/enums.py
--rw-r--r--   0 eve        (501) staff       (20)      173 2021-11-05 21:32:29.000000 eth-typing-3.3.0/eth_typing/ethpm.py
--rw-r--r--   0 eve        (501) staff       (20)      431 2021-11-05 21:32:29.000000 eth-typing-3.3.0/eth_typing/evm.py
--rw-r--r--   0 eve        (501) staff       (20)        0 2021-11-05 21:32:29.000000 eth-typing-3.3.0/eth_typing/py.typed
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-03-08 18:06:46.577461 eth-typing-3.3.0/eth_typing.egg-info/
--rw-r--r--   0 eve        (501) staff       (20)     4215 2023-03-08 18:06:46.000000 eth-typing-3.3.0/eth_typing.egg-info/PKG-INFO
--rw-r--r--   0 eve        (501) staff       (20)      439 2023-03-08 18:06:46.000000 eth-typing-3.3.0/eth_typing.egg-info/SOURCES.txt
--rw-r--r--   0 eve        (501) staff       (20)        1 2023-03-08 18:06:46.000000 eth-typing-3.3.0/eth_typing.egg-info/dependency_links.txt
--rw-r--r--   0 eve        (501) staff       (20)        1 2023-03-08 18:06:46.000000 eth-typing-3.3.0/eth_typing.egg-info/not-zip-safe
--rw-r--r--   0 eve        (501) staff       (20)      429 2023-03-08 18:06:46.000000 eth-typing-3.3.0/eth_typing.egg-info/requires.txt
--rw-r--r--   0 eve        (501) staff       (20)       11 2023-03-08 18:06:46.000000 eth-typing-3.3.0/eth_typing.egg-info/top_level.txt
--rw-r--r--   0 eve        (501) staff       (20)     1127 2023-03-08 17:58:11.000000 eth-typing-3.3.0/pyproject.toml
--rw-r--r--   0 eve        (501) staff       (20)       38 2023-03-08 18:06:46.577787 eth-typing-3.3.0/setup.cfg
--rw-r--r--   0 eve        (501) staff       (20)     2204 2023-03-08 18:05:13.000000 eth-typing-3.3.0/setup.py
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-07 21:41:25.408229 eth-typing-3.4.0/
+-rw-r--r--   0 eve        (501) staff       (20)     1095 2023-06-07 21:32:24.000000 eth-typing-3.4.0/LICENSE
+-rw-r--r--   0 eve        (501) staff       (20)      141 2023-06-07 21:32:24.000000 eth-typing-3.4.0/MANIFEST.in
+-rw-r--r--   0 eve        (501) staff       (20)     3230 2023-06-07 21:41:25.408103 eth-typing-3.4.0/PKG-INFO
+-rw-r--r--   0 eve        (501) staff       (20)     2282 2023-06-07 21:32:24.000000 eth-typing-3.4.0/README.md
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-07 21:41:25.407352 eth-typing-3.4.0/eth_typing/
+-rw-r--r--   0 eve        (501) staff       (20)      797 2023-06-07 21:32:24.000000 eth-typing-3.4.0/eth_typing/__init__.py
+-rw-r--r--   0 eve        (501) staff       (20)       85 2021-11-05 21:32:29.000000 eth-typing-3.4.0/eth_typing/abi.py
+-rw-r--r--   0 eve        (501) staff       (20)      191 2023-06-07 21:32:24.000000 eth-typing-3.4.0/eth_typing/bls.py
+-rw-r--r--   0 eve        (501) staff       (20)       71 2022-01-21 20:17:43.000000 eth-typing-3.4.0/eth_typing/discovery.py
+-rw-r--r--   0 eve        (501) staff       (20)      117 2023-06-07 21:32:24.000000 eth-typing-3.4.0/eth_typing/encoding.py
+-rw-r--r--   0 eve        (501) staff       (20)      458 2023-06-07 21:32:24.000000 eth-typing-3.4.0/eth_typing/enums.py
+-rw-r--r--   0 eve        (501) staff       (20)      173 2023-06-07 21:32:24.000000 eth-typing-3.4.0/eth_typing/ethpm.py
+-rw-r--r--   0 eve        (501) staff       (20)      431 2023-06-07 21:32:24.000000 eth-typing-3.4.0/eth_typing/evm.py
+-rw-r--r--   0 eve        (501) staff       (20)        0 2021-11-05 21:32:29.000000 eth-typing-3.4.0/eth_typing/py.typed
+drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-06-07 21:41:25.407937 eth-typing-3.4.0/eth_typing.egg-info/
+-rw-r--r--   0 eve        (501) staff       (20)     3230 2023-06-07 21:41:24.000000 eth-typing-3.4.0/eth_typing.egg-info/PKG-INFO
+-rw-r--r--   0 eve        (501) staff       (20)      439 2023-06-07 21:41:25.000000 eth-typing-3.4.0/eth_typing.egg-info/SOURCES.txt
+-rw-r--r--   0 eve        (501) staff       (20)        1 2023-06-07 21:41:24.000000 eth-typing-3.4.0/eth_typing.egg-info/dependency_links.txt
+-rw-r--r--   0 eve        (501) staff       (20)        1 2023-06-07 21:41:24.000000 eth-typing-3.4.0/eth_typing.egg-info/not-zip-safe
+-rw-r--r--   0 eve        (501) staff       (20)      477 2023-06-07 21:41:24.000000 eth-typing-3.4.0/eth_typing.egg-info/requires.txt
+-rw-r--r--   0 eve        (501) staff       (20)       11 2023-06-07 21:41:24.000000 eth-typing-3.4.0/eth_typing.egg-info/top_level.txt
+-rw-r--r--   0 eve        (501) staff       (20)     1226 2023-06-07 21:32:24.000000 eth-typing-3.4.0/pyproject.toml
+-rw-r--r--   0 eve        (501) staff       (20)       38 2023-06-07 21:41:25.408260 eth-typing-3.4.0/setup.cfg
+-rw-r--r--   0 eve        (501) staff       (20)     2350 2023-06-07 21:40:11.000000 eth-typing-3.4.0/setup.py
```

### Comparing `eth-typing-3.3.0/LICENSE` & `eth-typing-3.4.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2019 The Ethereum Foundation
+Copyright (c) 2018-2023 The Ethereum Foundation
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `eth-typing-3.3.0/PKG-INFO` & `eth-typing-3.4.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-typing
-Version: 3.3.0
+Version: 3.4.0
 Summary: eth-typing: Common type annotations for ethereum python packages
 Home-page: https://github.com/ethereum/eth-typing
 Author: The Ethereum Foundation
 Author-email: snakecharmers@ethereum.org
 License: MIT
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,35 +13,34 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7.2, <4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: dev
 License-File: LICENSE
 
 # eth-typing
 
-[![Join the chat at https://gitter.im/ethereum/eth-typing](https://badges.gitter.im/ethereum/eth-typing.svg)](https://gitter.im/ethereum/eth-typing?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
+[![Join the conversation on Discord](https://img.shields.io/discord/809793915578089484?color=blue&label=chat&logo=discord&logoColor=white)](https://discord.gg/GHryRvPB84)
 [![Build Status](https://circleci.com/gh/ethereum/eth-typing.svg?style=shield)](https://circleci.com/gh/ethereum/eth-typing)
 [![PyPI version](https://badge.fury.io/py/eth-typing.svg)](https://badge.fury.io/py/eth-typing)
 [![Python versions](https://img.shields.io/pypi/pyversions/eth-typing.svg)](https://pypi.python.org/pypi/eth-typing)
-[![Docs build](https://readthedocs.org/projects/eth-typing/badge/?version=latest)](http://eth-typing.readthedocs.io/en/latest/?badge=latest)
+[![Docs build](https://readthedocs.org/projects/eth-typing/badge/?version=latest)](https://eth-typing.readthedocs.io/en/latest/?badge=latest)
    
 
 Common type annotations for ethereum python packages.
 
-Read more in the [documentation on ReadTheDocs](https://eth-typing.readthedocs.io/). [View the change log](https://eth-typing.readthedocs.io/en/latest/releases.html).
+Read more in the [documentation on ReadTheDocs](https://eth-typing.readthedocs.io/). [View the change log](https://eth-typing.readthedocs.io/en/latest/release_notes.html).
 
 ## Quickstart
 
 ```sh
 pip install eth-typing
 ```
 
@@ -61,66 +60,32 @@
 You can set up your dev environment with:
 
 ```sh
 git clone git@github.com:ethereum/eth-typing.git
 cd eth-typing
 virtualenv -p python3 venv
 . venv/bin/activate
-pip install -e .[dev]
-```
-
-### Testing Setup
-
-During development, you might like to have tests run on every file save.
-
-Show flake8 errors on file change:
-
-```sh
-# Test flake8
-when-changed -v -s -r -1 eth_typing/ tests/ -c "clear; flake8 eth_typing tests && echo 'flake8 success' || echo 'error'"
-```
-
-Run multi-process tests in one command, but without color:
-
-```sh
-# in the project root:
-pytest --numprocesses=4 --looponfail --maxfail=1
-# the same thing, succinctly:
-pytest -n 4 -f --maxfail=1
-```
-
-Run in one thread, with color and desktop notifications:
-
-```sh
-cd venv
-ptw --onfail "notify-send -t 5000 'Test failure ⚠⚠⚠⚠⚠' 'python 3 test on eth-typing failed'" ../tests ../eth_typing
+pip install -e ".[dev]"
 ```
 
 ### Release setup
 
-For Debian-like systems:
-```
-apt install pandoc
-```
-
 To release a new version:
 
 ```sh
 make release bump=$$VERSION_PART_TO_BUMP$$
 ```
 
 #### How to bumpversion
 
 The version format for this repo is `{major}.{minor}.{patch}` for stable, and
 `{major}.{minor}.{patch}-{stage}.{devnum}` for unstable (`stage` can be alpha or beta).
 
 To issue the next version in line, specify which part to bump,
 like `make release bump=minor` or `make release bump=devnum`. This is typically done from the
 master branch, except when releasing a beta (in which case the beta is released from master,
-and the previous stable branch is released from said branch). To include changes made with each
-release, update "docs/releases.rst" with the changes, and apply commit directly to master 
-before release.
+and the previous stable branch is released from said branch).
 
 If you are in a beta version, `make release bump=stage` will switch to a stable.
 
 To issue an unstable version when the current version is stable, specify the
 new version explicitly, like `make release bump="--new-version 4.0.0-alpha.1 devnum"`
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `eth-typing-3.3.0/README.md` & `eth-typing-3.4.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # eth-typing
 
-[![Join the chat at https://gitter.im/ethereum/eth-typing](https://badges.gitter.im/ethereum/eth-typing.svg)](https://gitter.im/ethereum/eth-typing?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
+[![Join the conversation on Discord](https://img.shields.io/discord/809793915578089484?color=blue&label=chat&logo=discord&logoColor=white)](https://discord.gg/GHryRvPB84)
 [![Build Status](https://circleci.com/gh/ethereum/eth-typing.svg?style=shield)](https://circleci.com/gh/ethereum/eth-typing)
 [![PyPI version](https://badge.fury.io/py/eth-typing.svg)](https://badge.fury.io/py/eth-typing)
 [![Python versions](https://img.shields.io/pypi/pyversions/eth-typing.svg)](https://pypi.python.org/pypi/eth-typing)
-[![Docs build](https://readthedocs.org/projects/eth-typing/badge/?version=latest)](http://eth-typing.readthedocs.io/en/latest/?badge=latest)
+[![Docs build](https://readthedocs.org/projects/eth-typing/badge/?version=latest)](https://eth-typing.readthedocs.io/en/latest/?badge=latest)
    
 
 Common type annotations for ethereum python packages.
 
-Read more in the [documentation on ReadTheDocs](https://eth-typing.readthedocs.io/). [View the change log](https://eth-typing.readthedocs.io/en/latest/releases.html).
+Read more in the [documentation on ReadTheDocs](https://eth-typing.readthedocs.io/). [View the change log](https://eth-typing.readthedocs.io/en/latest/release_notes.html).
 
 ## Quickstart
 
 ```sh
 pip install eth-typing
 ```
 
@@ -33,66 +33,32 @@
 You can set up your dev environment with:
 
 ```sh
 git clone git@github.com:ethereum/eth-typing.git
 cd eth-typing
 virtualenv -p python3 venv
 . venv/bin/activate
-pip install -e .[dev]
-```
-
-### Testing Setup
-
-During development, you might like to have tests run on every file save.
-
-Show flake8 errors on file change:
-
-```sh
-# Test flake8
-when-changed -v -s -r -1 eth_typing/ tests/ -c "clear; flake8 eth_typing tests && echo 'flake8 success' || echo 'error'"
-```
-
-Run multi-process tests in one command, but without color:
-
-```sh
-# in the project root:
-pytest --numprocesses=4 --looponfail --maxfail=1
-# the same thing, succinctly:
-pytest -n 4 -f --maxfail=1
-```
-
-Run in one thread, with color and desktop notifications:
-
-```sh
-cd venv
-ptw --onfail "notify-send -t 5000 'Test failure ⚠⚠⚠⚠⚠' 'python 3 test on eth-typing failed'" ../tests ../eth_typing
+pip install -e ".[dev]"
 ```
 
 ### Release setup
 
-For Debian-like systems:
-```
-apt install pandoc
-```
-
 To release a new version:
 
 ```sh
 make release bump=$$VERSION_PART_TO_BUMP$$
 ```
 
 #### How to bumpversion
 
 The version format for this repo is `{major}.{minor}.{patch}` for stable, and
 `{major}.{minor}.{patch}-{stage}.{devnum}` for unstable (`stage` can be alpha or beta).
 
 To issue the next version in line, specify which part to bump,
 like `make release bump=minor` or `make release bump=devnum`. This is typically done from the
 master branch, except when releasing a beta (in which case the beta is released from master,
-and the previous stable branch is released from said branch). To include changes made with each
-release, update "docs/releases.rst" with the changes, and apply commit directly to master 
-before release.
+and the previous stable branch is released from said branch).
 
 If you are in a beta version, `make release bump=stage` will switch to a stable.
 
 To issue an unstable version when the current version is stable, specify the
 new version explicitly, like `make release bump="--new-version 4.0.0-alpha.1 devnum"`
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `eth-typing-3.3.0/eth_typing/__init__.py` & `eth-typing-3.4.0/eth_typing/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,30 +31,24 @@
     Hash32,
     HexAddress,
 )
 
 __all__ = (
     "Decodable",
     "TypeStr",
-
     "BLSPrivateKey",
     "BLSPubkey",
     "BLSSignature",
-
     "NodeID",
-
     "HexStr",
     "Primitives",
-
     "ForkName",
-
     "URI",
     "ContractName",
     "Manifest",
-
     "Address",
     "AnyAddress",
     "BlockIdentifier",
     "BlockNumber",
     "ChecksumAddress",
     "Hash32",
     "HexAddress",
```

### Comparing `eth-typing-3.3.0/eth_typing.egg-info/PKG-INFO` & `eth-typing-3.4.0/eth_typing.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-typing
-Version: 3.3.0
+Version: 3.4.0
 Summary: eth-typing: Common type annotations for ethereum python packages
 Home-page: https://github.com/ethereum/eth-typing
 Author: The Ethereum Foundation
 Author-email: snakecharmers@ethereum.org
 License: MIT
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,35 +13,34 @@
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7.2, <4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: dev
 License-File: LICENSE
 
 # eth-typing
 
-[![Join the chat at https://gitter.im/ethereum/eth-typing](https://badges.gitter.im/ethereum/eth-typing.svg)](https://gitter.im/ethereum/eth-typing?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
+[![Join the conversation on Discord](https://img.shields.io/discord/809793915578089484?color=blue&label=chat&logo=discord&logoColor=white)](https://discord.gg/GHryRvPB84)
 [![Build Status](https://circleci.com/gh/ethereum/eth-typing.svg?style=shield)](https://circleci.com/gh/ethereum/eth-typing)
 [![PyPI version](https://badge.fury.io/py/eth-typing.svg)](https://badge.fury.io/py/eth-typing)
 [![Python versions](https://img.shields.io/pypi/pyversions/eth-typing.svg)](https://pypi.python.org/pypi/eth-typing)
-[![Docs build](https://readthedocs.org/projects/eth-typing/badge/?version=latest)](http://eth-typing.readthedocs.io/en/latest/?badge=latest)
+[![Docs build](https://readthedocs.org/projects/eth-typing/badge/?version=latest)](https://eth-typing.readthedocs.io/en/latest/?badge=latest)
    
 
 Common type annotations for ethereum python packages.
 
-Read more in the [documentation on ReadTheDocs](https://eth-typing.readthedocs.io/). [View the change log](https://eth-typing.readthedocs.io/en/latest/releases.html).
+Read more in the [documentation on ReadTheDocs](https://eth-typing.readthedocs.io/). [View the change log](https://eth-typing.readthedocs.io/en/latest/release_notes.html).
 
 ## Quickstart
 
 ```sh
 pip install eth-typing
 ```
 
@@ -61,66 +60,32 @@
 You can set up your dev environment with:
 
 ```sh
 git clone git@github.com:ethereum/eth-typing.git
 cd eth-typing
 virtualenv -p python3 venv
 . venv/bin/activate
-pip install -e .[dev]
-```
-
-### Testing Setup
-
-During development, you might like to have tests run on every file save.
-
-Show flake8 errors on file change:
-
-```sh
-# Test flake8
-when-changed -v -s -r -1 eth_typing/ tests/ -c "clear; flake8 eth_typing tests && echo 'flake8 success' || echo 'error'"
-```
-
-Run multi-process tests in one command, but without color:
-
-```sh
-# in the project root:
-pytest --numprocesses=4 --looponfail --maxfail=1
-# the same thing, succinctly:
-pytest -n 4 -f --maxfail=1
-```
-
-Run in one thread, with color and desktop notifications:
-
-```sh
-cd venv
-ptw --onfail "notify-send -t 5000 'Test failure ⚠⚠⚠⚠⚠' 'python 3 test on eth-typing failed'" ../tests ../eth_typing
+pip install -e ".[dev]"
 ```
 
 ### Release setup
 
-For Debian-like systems:
-```
-apt install pandoc
-```
-
 To release a new version:
 
 ```sh
 make release bump=$$VERSION_PART_TO_BUMP$$
 ```
 
 #### How to bumpversion
 
 The version format for this repo is `{major}.{minor}.{patch}` for stable, and
 `{major}.{minor}.{patch}-{stage}.{devnum}` for unstable (`stage` can be alpha or beta).
 
 To issue the next version in line, specify which part to bump,
 like `make release bump=minor` or `make release bump=devnum`. This is typically done from the
 master branch, except when releasing a beta (in which case the beta is released from master,
-and the previous stable branch is released from said branch). To include changes made with each
-release, update "docs/releases.rst" with the changes, and apply commit directly to master 
-before release.
+and the previous stable branch is released from said branch).
 
 If you are in a beta version, `make release bump=stage` will switch to a stable.
 
 To issue an unstable version when the current version is stable, specify the
 new version explicitly, like `make release bump="--new-version 4.0.0-alpha.1 devnum"`
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `eth-typing-3.3.0/pyproject.toml` & `eth-typing-3.4.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,48 +1,53 @@
 [tool.towncrier]
-# Read https://github.com/ethereum/eth-typing/newsfragments/README.md for instructions
+# Read https://github.com/ethereum/eth-typing/blob/master/newsfragments/README.md for instructions
 package = "eth_typing"
 filename = "docs/release_notes.rst"
 directory = "newsfragments"
 underlines = ["-", "~", "^"]
-title_format = "v{version} ({project_date})"
+title_format = "eth-typing v{version} ({project_date})"
 issue_format = "`#{issue} <https://github.com/ethereum/eth-typing/issues/{issue}>`__"
 
 [[tool.towncrier.type]]
-directory = "feature"
-name = "Features"
+directory = "breaking"
+name = "Breaking changes"
 showcontent = true
 
 [[tool.towncrier.type]]
 directory = "bugfix"
 name = "Bugfixes"
 showcontent = true
 
 [[tool.towncrier.type]]
-directory = "performance"
-name = "Performance improvements"
+directory = "deprecation"
+name = "Deprecations"
 showcontent = true
 
 [[tool.towncrier.type]]
 directory = "doc"
 name = "Improved Documentation"
 showcontent = true
 
 [[tool.towncrier.type]]
-directory = "removal"
-name = "Deprecations and Removals"
+directory = "feature"
+name = "Features"
 showcontent = true
 
 [[tool.towncrier.type]]
 directory = "internal"
 name = "Internal Changes - for eth-typing Contributors"
 showcontent = true
 
 [[tool.towncrier.type]]
 directory = "misc"
 name = "Miscellaneous changes"
 showcontent = false
 
 [[tool.towncrier.type]]
-directory = "breaking"
-name = "Breaking changes"
-showcontent = true
+directory = "performance"
+name = "Performance improvements"
+showcontent = true
+
+[[tool.towncrier.type]]
+directory = "removal"
+name = "Removals"
+showcontent = true
```

