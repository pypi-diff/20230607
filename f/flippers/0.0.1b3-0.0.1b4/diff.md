# Comparing `tmp/flippers-0.0.1b3.tar.gz` & `tmp/flippers-0.0.1b4.tar.gz`

## Comparing `flippers-0.0.1b3.tar` & `flippers-0.0.1b4.tar`

### file list

```diff
@@ -1,84 +1,73 @@
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.readthedocs.yaml
--rw-r--r--   0        0        0    97312 2020-02-02 00:00:00.000000 flippers-0.0.1b3/LDA-Copy1.ipynb
--rw-r--r--   0        0        0    86117 2020-02-02 00:00:00.000000 flippers-0.0.1b3/LDA.ipynb
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/1015da5ee1d6ae09
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/101f92c76019d482
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/174575f6a8de99f9
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/222ffeab82898c23
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/24d706a41a5505e6
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/2619755b39779213
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/325fe9c721fee38b
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/32df89f30cbc04d0
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/32e73651997bc833
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/35ac780044c6113
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/3e9c803c3aed46b5
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/434179e472510be0
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/4349414af1af160b
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/46bff405bb5f9a55
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/51a86f2544beaac0
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/57c243f290383c75
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/5e121a9c5f4af371
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/61670e66e8896811
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/62b3397ef6b23cc6
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/6da9204864500947
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/6e36880ea88b0859
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/707a2630ead89062
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/71aabd6e1213d25d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/75172405e8805037
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/7680b266cdb5323d
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/7e140b818a0e35df
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/84f7eef6f0847552
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/8aa97df51a043d6b
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/905064e4094bb559
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/92432148d9c34749
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/931f99e805ef72f7
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/98a676691af497e5
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/a759e5f3179c9c3
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/a986cdd8da71d7e3
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/b11f13d1da690084
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/b4233a4bb09ad706
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/b7bcfa3cc7a39193
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/c161e876a1fa68c0
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/c60274caf2f8821
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/c8545ca9ed816bcd
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/ca78102643423a6c
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/ce06fdf2705b37fa
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/d4a51c2c60a9afbc
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/db5d9887bb35ef11
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/de69c8ba4e171810
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/e00199a4465c1154
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/e304e58799828dce
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/e32422aeb15174b7
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/e5b99527c8bf3efc
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/eb039d293b99e1a9
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/eb068414cbba1a66
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.ruff_cache/content/efb46ea7d6adfd16
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 flippers-0.0.1b3/docs/Makefile
--rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 flippers-0.0.1b3/docs/make.bat
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 flippers-0.0.1b3/docs/requirements.txt
--rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 flippers-0.0.1b3/docs/source/conf.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 flippers-0.0.1b3/docs/source/index.rst
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 flippers-0.0.1b3/docs/source/_static/custom.css
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 flippers-0.0.1b3/docs/source/_templates/autosummary/class.rst
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 flippers-0.0.1b3/docs/source/_templates/autosummary/module.rst
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 flippers-0.0.1b3/docs/source/reference/reference.rst
--rw-r--r--   0        0        0   216648 2020-02-02 00:00:00.000000 flippers-0.0.1b3/examples/ComparisonWithSnorkel.ipynb
--rw-r--r--   0        0        0   255575 2020-02-02 00:00:00.000000 flippers-0.0.1b3/examples/HyperParameterTuning.ipynb
--rw-r--r--   0        0        0    94666 2020-02-02 00:00:00.000000 flippers-0.0.1b3/examples/LabelModels.ipynb
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 flippers-0.0.1b3/flippers/__about__.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 flippers-0.0.1b3/flippers/__init__.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 flippers-0.0.1b3/flippers/_typing.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 flippers-0.0.1b3/flippers/_core/__init__.py
--rw-r--r--   0        0        0    18312 2020-02-02 00:00:00.000000 flippers-0.0.1b3/flippers/_core/_core.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 flippers-0.0.1b3/flippers/models/__init__.py
--rw-r--r--   0        0        0     9274 2020-02-02 00:00:00.000000 flippers-0.0.1b3/flippers/models/_base.py
--rw-r--r--   0        0        0     9354 2020-02-02 00:00:00.000000 flippers-0.0.1b3/flippers/models/_snorkel.py
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 flippers-0.0.1b3/scripts/download_wrench_datasets.sh
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 flippers-0.0.1b3/.gitignore
--rw-r--r--   0        0        0    11546 2020-02-02 00:00:00.000000 flippers-0.0.1b3/LICENSE
--rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 flippers-0.0.1b3/README.md
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 flippers-0.0.1b3/pyproject.toml
--rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 flippers-0.0.1b3/PKG-INFO
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 flippers-0.0.1b4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 flippers-0.0.1b4/.readthedocs.yaml
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 flippers-0.0.1b4/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 flippers-0.0.1b4/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 flippers-0.0.1b4/.ruff_cache/content/1992c7ad7f1af1bb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 flippers-0.0.1b4/.ruff_cache/content/1e0fe41073f4c89d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b4/.ruff_cache/content/2365ff43c932e747
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b4/.ruff_cache/content/26dcfcc00daa5079
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 flippers-0.0.1b4/.ruff_cache/content/29116d8dc091fd0
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b4/.ruff_cache/content/2a0a371120eb97da
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b4/.ruff_cache/content/409a65911ac5fb6a
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b4/.ruff_cache/content/4be1350c5c7451c6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 flippers-0.0.1b4/.ruff_cache/content/529edb5728be2ca
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b4/.ruff_cache/content/565ab6a6c96c264d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 flippers-0.0.1b4/.ruff_cache/content/61d7efe6bcf1a319
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 flippers-0.0.1b4/.ruff_cache/content/6b816c6ac0bb6ab5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 flippers-0.0.1b4/.ruff_cache/content/7034400682b4eb70
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b4/.ruff_cache/content/74ee63e9b5e09487
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 flippers-0.0.1b4/.ruff_cache/content/7531534a0fbce831
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 flippers-0.0.1b4/.ruff_cache/content/7dc39e403a79fbc9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 flippers-0.0.1b4/.ruff_cache/content/800dbb5b82579ae0
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b4/.ruff_cache/content/919a1e1e8025e12e
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b4/.ruff_cache/content/98e825767b91acc3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 flippers-0.0.1b4/.ruff_cache/content/9980df82df543ebd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 flippers-0.0.1b4/.ruff_cache/content/9e14e56eca58724a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 flippers-0.0.1b4/.ruff_cache/content/b0ff5b47ced6b2f6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 flippers-0.0.1b4/.ruff_cache/content/b47a8357941a7d49
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b4/.ruff_cache/content/bd63319d6f01c079
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b4/.ruff_cache/content/bf129a628123b1d6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 flippers-0.0.1b4/.ruff_cache/content/d522c4864c12f596
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 flippers-0.0.1b4/.ruff_cache/content/d5c096a6cf41bb9d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 flippers-0.0.1b4/.ruff_cache/content/dc8e0a575e1d22bd
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b4/.ruff_cache/content/f0b92f868316bf1f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 flippers-0.0.1b4/.ruff_cache/content/f2e76ccc1277e492
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b4/.ruff_cache/content/f9aac14f8ac8c5
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b4/.ruff_cache/content/faab5c703a005b2d
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 flippers-0.0.1b4/.ruff_cache/content/fd21da4df4f49628
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 flippers-0.0.1b4/docs/Makefile
+-rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 flippers-0.0.1b4/docs/make.bat
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 flippers-0.0.1b4/docs/requirements.txt
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 flippers-0.0.1b4/docs/source/conf.py
+-rw-r--r--   0        0        0    49718 2020-02-02 00:00:00.000000 flippers-0.0.1b4/docs/source/flippers.png
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 flippers-0.0.1b4/docs/source/index.rst
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 flippers-0.0.1b4/docs/source/_static/custom.css
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 flippers-0.0.1b4/docs/source/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 flippers-0.0.1b4/docs/source/_templates/autosummary/module.rst
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 flippers-0.0.1b4/docs/source/reference/reference.rst
+-rw-r--r--   0        0        0   385675 2020-02-02 00:00:00.000000 flippers-0.0.1b4/examples/ComparisonWithSnorkel.ipynb
+-rw-r--r--   0        0        0    64710 2020-02-02 00:00:00.000000 flippers-0.0.1b4/examples/GettingStarted.ipynb
+-rw-r--r--   0        0        0   410586 2020-02-02 00:00:00.000000 flippers-0.0.1b4/examples/HyperParameterTuning.ipynb
+-rw-r--r--   0        0        0   231267 2020-02-02 00:00:00.000000 flippers-0.0.1b4/examples/LabelModels.ipynb
+-rw-r--r--   0        0        0     6087 2020-02-02 00:00:00.000000 flippers-0.0.1b4/examples/utils.py
+-rw-r--r--   0        0        0    96313 2020-02-02 00:00:00.000000 flippers-0.0.1b4/examples/wrench.png
+-rw-r--r--   0        0        0   247912 2020-02-02 00:00:00.000000 flippers-0.0.1b4/examples/Experiments/HyperParameterTuningVAE.ipynb
+-rw-r--r--   0        0        0   220488 2020-02-02 00:00:00.000000 flippers-0.0.1b4/examples/Experiments/WeakLabelDataVAE.ipynb
+-rw-r--r--   0        0        0   520869 2020-02-02 00:00:00.000000 flippers-0.0.1b4/examples/Experiments/WeakLabelVAE.ipynb
+-rw-r--r--   0        0        0     8469 2020-02-02 00:00:00.000000 flippers-0.0.1b4/examples/Experiments/_vae.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 flippers-0.0.1b4/flippers/__about__.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 flippers-0.0.1b4/flippers/__init__.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 flippers-0.0.1b4/flippers/_typing.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 flippers-0.0.1b4/flippers/_core/__init__.py
+-rw-r--r--   0        0        0    17843 2020-02-02 00:00:00.000000 flippers-0.0.1b4/flippers/_core/_core.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 flippers-0.0.1b4/flippers/lfs/__init__.py
+-rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 flippers-0.0.1b4/flippers/lfs/_lfs.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 flippers-0.0.1b4/flippers/models/__init__.py
+-rw-r--r--   0        0        0     9253 2020-02-02 00:00:00.000000 flippers-0.0.1b4/flippers/models/_base.py
+-rw-r--r--   0        0        0     9722 2020-02-02 00:00:00.000000 flippers-0.0.1b4/flippers/models/_snorkel.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 flippers-0.0.1b4/scripts/download_wrench_datasets.sh
+-rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 flippers-0.0.1b4/.gitignore
+-rw-r--r--   0        0        0    11546 2020-02-02 00:00:00.000000 flippers-0.0.1b4/LICENSE
+-rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 flippers-0.0.1b4/README.md
+-rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 flippers-0.0.1b4/pyproject.toml
+-rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 flippers-0.0.1b4/PKG-INFO
```

### Comparing `flippers-0.0.1b3/docs/Makefile` & `flippers-0.0.1b4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `flippers-0.0.1b3/docs/make.bat` & `flippers-0.0.1b4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `flippers-0.0.1b3/docs/source/conf.py` & `flippers-0.0.1b4/docs/source/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 # Import the theme and set it as the default
 
 project = "flippers"
 copyright = f"2023 - {datetime.now().year}, Liam Toran"
 author = "Liam Toran"
-release = "alpha"
+release = ""
 
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     "sphinx.ext.napoleon",
```

### Comparing `flippers-0.0.1b3/docs/source/_templates/autosummary/class.rst` & `flippers-0.0.1b4/docs/source/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `flippers-0.0.1b3/docs/source/_templates/autosummary/module.rst` & `flippers-0.0.1b4/docs/source/_templates/autosummary/module.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 {{ fullname | escape | underline}}
 
 .. automodule:: {{ fullname }}
    :members:
    :undoc-members:
    :inherited-members:
    :show-inheritance:
+   :noindex:
 
 
    {% block modules %}
    {% if modules %}
    .. rubric:: Modules
 
    .. autosummary::
```

### Comparing `flippers-0.0.1b3/flippers/_core/_core.py` & `flippers-0.0.1b4/flippers/_core/_core.py`

 * *Files 3% similar despite different names*

```diff
@@ -109,16 +109,14 @@
         representing the possible polarities.
 
     Example
     -------
     Its always better to use an hand written ``polairites_mapping``.
     ``polarities_mapping`` lists possible polarities each labeling function can have.
 
-    >>> import pandas as pd
-    >>> import flippers
     >>> multipolar = pd.DataFrame([[-1, 1, 2], [0, -1, 0], [-1, -1, 2]])
     >>> polarities_mapping = {'0': [0], '1': [1], '2': [0, 2]}
     >>> L, polarities, _ = flippers.multipolar_to_monopolar(
                                                 multipolar, polarities_mapping
                                                 )
     >>> L
        0  1  2__0  2__2
@@ -199,24 +197,23 @@
 
     Returns
     -------
     Series of size n_samples indicating whether a sample is labeled or not.
 
     Example
     -------
-    >>> import pandas as pd
-    >>> import flippers
     >>> L = pd.DataFrame([[0, 1, 0], [1, 0, 1], [0, 0, 0], [1, 1, 1]])
     >>> flippers.is_labeled(L)
     0     True
     1     True
     2    False
     3     True
     dtype: bool
     """
+    L = pd.DataFrame(L)
     return L.sum(axis=1) > 0
 
 
 def total_coverage(L: pd.DataFrame) -> float:
     """Calculate the total proportion of labeled samples in the given label
     matrix.
 
@@ -229,20 +226,19 @@
     -------
     float
         Total coverage, ranging from 0 to 1, indicating the proportion of
         labeled samples in the label matrix.
 
     Example
     -------
-    >>> import pandas as pd
-    >>> import flippers
     >>> L = pd.DataFrame([[0, 1, 0], [1, 0, 1], [0, 0, 0], [1, 1, 1]])
     >>> flippers.total_coverage(L)
     0.75
     """
+    L = pd.DataFrame(L)
     return is_labeled(L).mean()
 
 
 def filter_labeled(L: pd.DataFrame) -> pd.DataFrame:
     """Filter out unlabeled samples from the given label matrix.
 
     Parameters
@@ -253,22 +249,21 @@
     Returns
     -------
     Returns a filtered label matrix of shape (n_labeled_samples, n_weak).
     Sliced on the condition that the first one is labeled.
 
     Example
     -------
-    >>> import pandas as pd
-    >>> import flippers
     >>> L = pd.DataFrame([[0, 1, 0], [1, 0, 1], [0, 0, 0], [1, 1, 1]])
     >>> flippers.filter_labeled(L)
        0  1  2
     0  0  1  0
     2  1  0  1
     """
+    L = pd.DataFrame(L)
     labeled = is_labeled(L)
     return L.loc[labeled]
 
 
 def coverage(L: pd.DataFrame) -> pd.Series:
     """Calculate the average of samples labeled per weak labeler.
 
@@ -279,23 +274,22 @@
 
     Returns
     -------
     Series of size n_weak with average of samples labeled per weak labeler.
 
     Example
     -------
-    >>> import pandas as pd
-    >>> import flippers
     >>> L = pd.DataFrame([[0, 1, 0], [1, 0, 1], [0, 0, 0], [1, 1, 1]])
     >>> flippers.coverage(L)
     0    0.5
     1    0.5
     2    0.5
     dtype: float64
     """
+    L = pd.DataFrame(L)
     return (L > 0).mean()
 
 
 def confidence(L: pd.DataFrame) -> pd.Series:
     """Calculate the average confidence level per weak labeler.
 
     Parameters
@@ -305,23 +299,22 @@
 
     Returns
     -------
     Series of size n_weak with average confidence level per weak labeler.
 
     Example
     -------
-    >>> import pandas as pd
-    >>> import flippers
     >>> L = pd.DataFrame([[0, .1, 0], [1, 0, .5], [0, 0, 0], [.7, .1, .2]])
     >>> flippers.confidence(L)
     0    0.85
     1    0.10
     2    0.35
     dtype: float64
     """
+    L = pd.DataFrame(L)
     return L[L > 0].mean()
 
 
 def _overlaps(
     L: pd.DataFrame, polarities: ListLike = [], sign: str = "overlaps"
 ) -> pd.Series:
     """Calculate the number of overlaps for each sample and weak label.
@@ -347,16 +340,14 @@
     -------
     pd.Series
         Series of length n_weak indicating the fraction of
         annotated samples with other annotations for each LF.
 
     Example
     -------
-    >>> import pandas as pd
-    >>> import flippers
     >>> L = pd.DataFrame([[0, 1, 0], [1, 0, 1], [0, 0, 0], [1, 1, 1]])
     >>> # All overlaps
     >>> flippers._overlaps(L)
     0    0.50
     1    0.25
     2    0.50
     dtype: float64
@@ -410,16 +401,14 @@
     -------
     pd.Series
         Series of length n_weak indicating the fraction of
         annotated samples with other annotations for each LF.
 
     Example
     -------
-    >>> import pandas as pd
-    >>> import flippers
     >>> L = pd.DataFrame([[0, 1, 0], [1, 0, 1], [0, 0, 0], [1, 1, 1]])
     >>> flippers.overlap(L)
     0    0.50
     1    0.25
     2    0.50
     dtype: float64
     """
@@ -447,16 +436,14 @@
     -------
     pd.Series
         Series of length n_weak indicating the fraction of
         annotated samples with conflicting annotations for each LF.
 
     Example
     -------
-    >>> import pandas as pd
-    >>> import flippers
     >>> L = pd.DataFrame([[0, 1, 0], [1, 0, 1], [0, 0, 0], [1, 1, 1]])
     >>> flippers.conflicts(L, polarities)
     0    0.50
     1    0.25
     2    0.50
     dtype: float64
     """
@@ -479,16 +466,14 @@
     -------
     pd.Series
         Series of length n_weak indicating the fraction of
         annotated samples with matching annotations for each LF.
 
     Example
     -------
-    >>> import pandas as pd
-    >>> import flippers
     >>> L = pd.DataFrame([[0, 1, 0], [1, 0, 1], [0, 0, 0], [1, 1, 1]])
     >>> flippers.matches(L, polarities)
     0    0.00
     1    0.25
     2    0.25
     dtype: float64
     """
@@ -521,16 +506,14 @@
         - "confidence": The average confidence level of the assigned weak labels.
         - "overlaps": The ratio of assigned labels that have overlapping labels.
         - "matches": The ratio of assigned labels that have other matching labels.
         - "conflicts": The ratio of assigned labels that have conflicting labels.
 
     Example
     -------
-    >>> import pandas as pd
-    >>> import flippers
     >>> L = pd.DataFrame([[0, 1, 0], [1, 0, 1], [0, 0, 0], [1, 1, 1]])
     >>> polarities = [0, 1, 1]
     >>> flippers.summary(L, polarities)
         polarity  coverage  confidence  overlaps  matches  conflicts
     0         0       0.5         1.0      0.50     0.00        0.50
     1         1       0.5         1.0      0.25     0.25        0.25
     2         1       0.5         1.0      0.50     0.25        0.50
```

### Comparing `flippers-0.0.1b3/flippers/models/_base.py` & `flippers-0.0.1b4/flippers/models/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,16 +59,15 @@
         Parameters
         ----------
         filepath : str
             Path to the file containing the saved model.
 
         Returns
         -------
-        model :
-            The loaded model object.
+        The loaded model object.
 
         Example
         -------
         >>> model = ModelClass.load("label_model.pkl")
         """
         with open(filepath, "rb") as file:
             model = pickle.load(file)
```

### Comparing `flippers-0.0.1b3/flippers/models/_snorkel.py` & `flippers-0.0.1b4/flippers/models/_snorkel.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,27 @@
     Bayes assumption.
 
     However, good results can also be observed in practice for
     correlated LFs.
 
     See the following link[] for more information on how to use this
     model and a comparison with the Snorkel library's implementation.
+
+    Example
+    -------
+
+    >>> from flippers.models import SnorkelModel
+    >>>
+    >>> # Create a SnorkelModel instance
+    >>> label_model = SnorkelModel(polarities, cardinality, class_balances)
+    >>> # Train the model
+    >>> label_model.fit(L_train)
+    >>> # Generate labels
+    >>> y_pred_proba = label_model.predict_proba(L) # shape: (len(L), n_classes)
+    >>> y_pred = label_model.predict(L) # shape: (len(L),)
     """
 
     def __init__(
         self,
         polarities: ListLike,
         cardinality: int = 0,
         class_balances: ListLike = [],
@@ -51,184 +64,182 @@
             Defaults to balanced classes prior.
 
         Example
         -------
         >>> polarities = [1, 0, 1, 1]
         >>> cardinality = 2
         >>> class_balances = [0.7, 0.3]
-        >>> snorkel_model = SnorkelModel(polarities, cardinality, class_balances)
+        >>> label_model = SnorkelModel(polarities, cardinality, class_balances)
+        >>> # Change device
+        >>> label_model.to("cuda")
         """
         nn.Module.__init__(self)
         _BaseModel.__init__(self, polarities, cardinality)
 
         self.Polarities = nn.Parameter(
             torch.Tensor(self.polarities_matrix), requires_grad=False
         )
 
         if not class_balances:
             class_balances = 1 / self.cardinality * np.ones(int(self.cardinality))
         self.class_balances = class_balances
         self.Balances = nn.Parameter(torch.Tensor(class_balances), requires_grad=False)
+        self.loss_history = []
+
+    @property
+    def device(self):
+        return next(self.parameters()).device
 
     def _convert_L(self, L: MatrixLike) -> torch.Tensor:
         """Convert input L to binary tensor."""
         L = np.array(L)
         L = L > 0.5
-        L = torch.tensor(L).to(torch.float)
+        L = torch.tensor(L).to(device=self.device, dtype=torch.float32)
         return L
 
     def fit(
         self,
         L: MatrixLike,
         learning_rate: float = 1e-3,
         num_epochs: int = 50,
-        prec_init: float = 0.7,
-        weight_decay: float = 0,
+        prec_init: float = 0.5,
         k: float = 0,
-        device: str = "cpu",
         verbose: bool = False,
-        *_,
+        **_,
     ) -> None:
         """Train the Snorkel model on the given weak label matrix L.
 
         Parameters
         ----------
         L : MatrixLike
             Weak Label matrix of shape (num_samples, n_weak)
         learning_rate : float, optional, default: 1e-3
             Learning rate for the optimizer.
         num_epochs : int, optional, default: 50
             Number of epochs to train the model
-        prec_init : float, optional, default: 0.7
+        prec_init : float, optional, default: 0.5
             Initial value for precision
 
             Can be of shape (n_weak) to set precision for each LF.
-        weight_decay : float, optional, default: 0
-            Weight decay (L2 penalty) for the optimizer
         k : float, optional, default: 0
             Weight of class blance loss term.
 
             This term penalizes the model for predicting a class on the train set
             differently to its specified balance
-        device : str, optional, default: "cpu"
-            Device to use for training, either "cpu" or "cuda"
         verbose : bool, optional, default: False
-            If True, displays training progress
+            When True, displays training progress using tqdm.
 
         Returns
         -------
         None
 
         Example
         -------
         >>> L = [
         ...     [1, 0, 1, 1],
         ...     [0, 1, 0, 1],
         ...     [1, 0, 1, 0]
         ... ]
-        >>> snorkel_model.fit(
+        >>> label_model.fit(
         ...     L,
         ...     learning_rate=1e-2,
         ...     num_epochs=10,
         ...     prec_init=0.7,
         ...     k=5e-3,
-        ...     device="cpu",
         ...     verbose=True
         ... )
         """
 
-        self.to(device)
-
-        self.num_samples = len(L)
         self.num_epochs = num_epochs
         self.learning_rate = learning_rate
-        self.weight_decay = weight_decay
-        self.loss_history = []
-
-        # Deal with multiple types
-        self.prec_init = prec_init
-        self.Prec_init = torch.ones(self.n_weak).to(device) * prec_init
+        eps = 1e-6
 
         # Convert L to binary tensor
         L = self._convert_L(L)
-        L = L.to(device)
 
         # Gram matrix of L gives overlaps
-        Overlaps = L.T @ L / self.num_samples
+        Overlaps = L.T @ L / len(L)
         Coverage = torch.diag(Overlaps)  # Overlaps with itself = coverage
-        Overlaps, Coverage = Overlaps.to(device), Coverage.to(device)
+        Overlaps, Coverage = Overlaps.to(self.device), Coverage.to(self.device)
 
         # mu(i, j) = P(L_i = 1 | Y = j)
         # Bayes theorem
-        self.mu_init = (
-            self.Polarities * (self.Prec_init * Coverage).view(-1, 1) / self.Balances
-        ).float()
-        self.mu = nn.Parameter(self.mu_init.clone())  # * np.random.random())
+        if not hasattr(self, "prec_init"):
+            self.prec_init = prec_init
+            self.Prec_init = torch.ones(self.n_weak).to(self.device) * prec_init
+            self.mu_init = (
+                self.Polarities
+                * (self.Prec_init * Coverage).view(-1, 1)
+                / self.Balances
+            ).float()
+            self.mu = nn.Parameter(self.mu_init.clone())  # * np.random.random())
 
         # This will be changed when dealing with cliques the right way
-        mask_overlap = torch.ones(self.n_weak, self.n_weak).to(device).int()
+        mask_overlap = torch.ones(self.n_weak, self.n_weak).to(self.device).int()
         mask_overlap = mask_overlap - torch.diag(torch.diag(mask_overlap))
+        mask_overlap = mask_overlap.bool()
+        Overlaps = Overlaps[mask_overlap]
 
-        optimizer = optim.SGD(
+        optimizer = optim.Adam(
             [x for x in self.parameters() if x.requires_grad],
             lr=self.learning_rate,
-            weight_decay=self.weight_decay,
-            momentum=0,
         )
 
+        def loss_fn(x, y):
+            return torch.norm(x - y) ** 2
+
         if verbose:
             epoch_range = trange(self.num_epochs)
         else:
             epoch_range = range(self.num_epochs)
 
         for epoch in epoch_range:
             # Zero the gradients
             optimizer.zero_grad()
-            self.mu.data = self.mu.clamp(1e-6, 1 - 1e-6)
+            self.mu.data = self.mu.clamp(eps, 1 - eps)
+
+            # # Forward
 
-            # Forward
-            # Calculate loss
-            loss_overlap = torch.norm(
-                (Overlaps - (self.mu * self.Balances) @ self.mu.t())[mask_overlap]
-            )
-
-            # mu * class_balance = precision * coverage
-            # so if for precision ~ 1, we want mu * class_balance - coverage ~ 0
-            # this term of the loss is trying to maximize the precision of
-            # the input weak labeler.
-            loss_coverage = torch.norm(self.mu @ self.Balances - Coverage)
+            # Overlap reconstruction loss
+            overlap_reconstructed = ((self.mu * self.Balances) @ self.mu.t())[
+                mask_overlap
+            ]
+            loss_overlap = loss_fn(overlap_reconstructed, Overlaps)
 
-            loss = loss_overlap**2 + loss_coverage**2
+            # Coverage reconstruction loss
+            # coverage = mu @ class_balance by total law of probability
+            loss_coverage = loss_fn(self.mu @ self.Balances, Coverage)
+
+            loss = loss_overlap + loss_coverage
             if k > 0:
-                loss_prediction = torch.norm(
-                    self.Balances - self._predict_proba_tensor(L).mean(0)
+                loss_prediction = loss_fn(
+                    self.Balances, self._predict_proba_tensor(L).mean(0)
                 )
-                loss = loss + k * loss_prediction**2
+
+                loss = loss + k * loss_prediction
 
             # Backward
             loss.backward()
 
-            # Log loss_history
-            self.loss_history.append(loss.item())
-
             # Optimizer Step
             optimizer.step()
 
-            # Scheduler step
-            # TODO
+            # Log loss_history
+            self.loss_history.append(loss.item())
+
+            if verbose and ((epoch % 50 == 0) or (epoch == self.num_epochs - 1)):
+                epoch_range.set_description(
+                    f"Epoch {epoch+1}/{self.num_epochs} | Loss {loss.item():.4f}"
+                )
 
         # Clamp mu
-        self.mu.data = self.mu.clamp(1e-6, 1 - 1e-6)
-
-        # Break permutation symetry in case class balance has non unique values
-        # TODO
+        self.mu.data = self.mu.clamp(eps, 1 - eps)
 
         # Eval mode so predict_proba doesnt calculate gradients
         self.eval()
-        self.to("cpu")
 
     def _predict_proba_tensor(
         self, L: torch.tensor, ignore_abstains: bool = False
     ) -> torch.tensor:
         # Computing trick :
         # exp(L @ log(mu))[i, k] = Product of mu[j, k] for j / L[i, j] = 1
         Log_likelihood = L @ self.mu.log()
@@ -248,36 +259,36 @@
         Parameters
         ----------
         L : MatrixLike
             Weak Label matrix
         ignore_abstains : bool, optional
             Whether to ignore abstains in the prior update:
 
-            - False (default), using both votes and abstains. This helps leveraging
-            information gained from knowing which labeling function abstained.
-
-            - True, updates prior only using non abstained votes
+            $ When `False` (default), uses both votes and abstains. This is recommended
+            and helps leverage information gained from
+            knowing which labeling function abstained.
 
+            $ When `True`, updates prior only using non abstained.
 
         Returns
         -------
         numpy.ndarray
             An array of predicted probabilities of shape (num_samples, num_classes).
 
         Example
         -------
         >>> L = [
         ...     [1, 0, 1, 1],
         ...     [0, 1, 0, 1],
         ...     [1, 0, 1, 0]
         ... ]
-        >>> proba = snorkel_model.predict_proba(L)
+        >>> proba = label_model.predict_proba(L)
         >>> # proba.shape = (len(L), cardinality)
         """
-        L = self._convert_L(L).float()
+        L = self._convert_L(L)
 
         with torch.no_grad():
             Proba = self._predict_proba_tensor(L, ignore_abstains)
 
         proba = Proba.detach().cpu().numpy()
 
         return proba
```

### Comparing `flippers-0.0.1b3/scripts/download_wrench_datasets.sh` & `flippers-0.0.1b4/scripts/download_wrench_datasets.sh`

 * *Files identical despite different names*

### Comparing `flippers-0.0.1b3/.gitignore` & `flippers-0.0.1b4/.gitignore`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# Training checkpoints
+*checkpoint*
+*runs*
+
 # Junk
 *Untitled*
 
 # Data
 *.json
 *.csv
 datasets*
```

### Comparing `flippers-0.0.1b3/LICENSE` & `flippers-0.0.1b4/LICENSE`

 * *Files identical despite different names*

### Comparing `flippers-0.0.1b3/README.md` & `flippers-0.0.1b4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,55 @@
-# flippers - A Weak Supervision Library 
+<img src="docs/source/flippers.png" width="255"/>
 
 ![GitHub last commit](https://img.shields.io/github/last-commit/liamtoran/flippers)
 ![PyPI](https://img.shields.io/pypi/v/flippers)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/flippers)
 ![Code Style](https://img.shields.io/badge/code%20style-black-black)
 ![Read the Docs](https://img.shields.io/readthedocs/flippers)
 ![GitHub](https://img.shields.io/github/license/liamtoran/flippers)
 
-(in construction)
-
 `flippers` is a Python library for weak supervision, which allows you to leverage your domain knowledge, heuristics and other weak supervision sources to generate high-quality labels for your training data. 
 
 # Features
 `flippers` includes a number of features for weak supervision, including:
 - Simple tools to analyse your labeling functions,
 - Multiple label models including a from-scratch implementation of the label model used in the `snorkel` library and featuring enhanced ways to predict probabilities,
-- An extensive [documentation](https://flippers.readthedocs.io/en/latest/) with [tutorials](missing_link) and an [API reference](https://flippers.readthedocs.io/en/latest/reference/flippers.html).
+- An extensive [documentation](https://flippers.readthedocs.io/en/latest/) with [tutorials](https://github.com/liamtoran/flippers/tree/main/examples) and an [API reference](https://flippers.readthedocs.io/en/latest/reference/flippers.html).
 
 # Installation
 To install the latest version of `flippers`, simply run:
 
 ```bash
 pip install flippers
 ```
 
 # Quick Start 
 ## Documentation
-To quickly get started with `flippers`, you can begin by exploring the [documentation](https://flippers.readthedocs.io/en/latest/) and running through the [examples](missing_link) provided. The examples cover a variety of use cases and techniques, which can help you to get a feel for how to apply `flippers` to your own projects. 
+To quickly get started with `flippers`, you can begin by exploring the [documentation](https://flippers.readthedocs.io/en/latest/) and running through the [examples](hhttps://github.com/liamtoran/flippers/tree/main/examples) provided. The examples cover a variety of use cases and techniques, which can help you to get a feel for how to apply `flippers` to your own projects. 
 ## Example
 - Analyzing your labeling functions:
 ```python
 analysis = flippers.analyis(L_train)
 ```
 - Training a Label Model and doing inference:
 
 ```python
-label_model = flippers.models.SnorkelModel(polarities,  class_balances)
+label_model = flippers.models.SnorkelModel(polarities, class_balances)
 
 label_model.fit(L_train)
 
 label_model.predict_proba(L)
 ```
 
 # Discussion
 ## Troubleshooting
 If you have any questions or issues with `flippers`, please consult the [documentation](https://flippers.readthedocs.io/en/latest/) or reach out in the [GitHub issues](https://github.com/liamtoran/flippers/issues) page for support.
 
 
 ## Contributing
 
-`flippers` is an open-source project, and contributions are welcome! If you would like to contribute to `flippers`, please read the `CONTRIBUTING.md` file for guidelines and instructions.
+`flippers` is an open-source project, and contributions are welcome!
 
 ## Related projects
 - [wrench](https://github.com/JieyuZ2/wrench): A weak supervision library created by for benchmarking label models and weak supervision techniques. `flippers` uses its list of datasets as benchmarks.  
 - [snorkel](https://github.com/snorkel-team/snorkel): A cornerstone weak supervision library created by Snorkel in 2016, now sadly abandonned.
```

### Comparing `flippers-0.0.1b3/pyproject.toml` & `flippers-0.0.1b4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -6,25 +6,22 @@
 name = "flippers"
 description = '`flippers` is a weak supervision library for creating high quality labels using your domain kownledge and weak supervision sources.'
 readme = "README.md"
 requires-python = ">=3.7"
 license = "Apache-2.0"
 keywords = [
   "weak supervision",
+  "labeling",
+  "annotation",
   "data labeling",
   "data science",
   "machine learning",
-  "data engineering",
-  "data analysis",
-  "data wrangling",
-  "data cleaning",
-  "data preparation",
-  "data augmentation",
   "data",
 ]
+
 authors = [{ name = "Liam Toran", email = "liam.toran@gmail.com" }]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
@@ -39,37 +36,38 @@
 Issues = "https://github.com/liamtoran/flippers/issues"
 Source = "https://github.com/liamtoran/flippers"
 
 [tool.hatch.version]
 path = "flippers/__about__.py"
 
 [tool.hatch.envs.default]
+python = "3.10"
 dependencies = [
   "pre-commit",
   "pre-commit-hooks",
   "docformatter",
   "black[jupyter]",
   "isort",
   "jupyterlab",
-  "ray[tune]",
+  "ray[air,tune]",
   "snorkel",
   "jupyterlab-code-formatter",
   "ruff",
 ]
 [tool.hatch.envs.default.scripts]
 
 
 [tool.coverage.run]
 branch = true
 parallel = true
 omit = ["flippers/__about__.py"]
 
 # Linting and ruff
-
 [tool.hatch.envs.lint]
+python = "3.10"
 description = "Check and lint the codebase."
 dependencies = [
   "pre-commit",
   "pre-commit-hooks",
   "docformatter",
   "isort",
   "black[jupyter]",
@@ -77,15 +75,14 @@
 ]
 
 [tool.hatch.envs.lint.scripts]
 run = ["black .", "isort .", "docformatter -i -r .", "ruff ."]
 
 
 # mypy checks
-
 [tool.hatch.envs.type]
 description = "Type check the codebase."
 dependencies = [
   "pytest",
   "pytest-cov",
   "mypy",
   # Dependencies
@@ -112,25 +109,27 @@
 
 [tool.hatch.envs.type.scripts]
 run = "mypy {args:--namespace-packages -p flippers}"
 
 [tool.coverage.report]
 exclude_lines = ["no cov", "if __name__ == .__main__.:", "if TYPE_CHECKING:"]
 
+# Documentation environment
 [tool.hatch.envs.docs]
 description = "Build the documentation."
+python = "3.10"
 dependencies = [
   "sphinx",
   "nbsphinx",
   "sphinx_argparse_cli",
   "sphinx_copybutton",
   "pydata_sphinx_theme",
 ]
 
 [tool.hatch.envs.docs.scripts]
-clean = "bpwd; cd docs; ./Make.bat clean"
+clean = "cd docs; ./make.bat clean"
 
 [tool.ruff]
 line-length = 88
 
 [tool.isort]
 profile = "black"
```

### Comparing `flippers-0.0.1b3/PKG-INFO` & `flippers-0.0.1b4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: flippers
-Version: 0.0.1b3
+Version: 0.0.1b4
 Summary: `flippers` is a weak supervision library for creating high quality labels using your domain kownledge and weak supervision sources.
 Project-URL: Documentation, https://github.com/liamtoran/flippers#readme
 Project-URL: Issues, https://github.com/liamtoran/flippers/issues
 Project-URL: Source, https://github.com/liamtoran/flippers
 Author-email: Liam Toran <liam.toran@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
-Keywords: data,data analysis,data augmentation,data cleaning,data engineering,data labeling,data preparation,data science,data wrangling,machine learning,weak supervision
+Keywords: annotation,data,data labeling,data science,labeling,machine learning,weak supervision
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -20,64 +20,62 @@
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scikit-learn
 Requires-Dist: tqdm
 Description-Content-Type: text/markdown
 
-# flippers - A Weak Supervision Library 
+<img src="docs/source/flippers.png" width="255"/>
 
 ![GitHub last commit](https://img.shields.io/github/last-commit/liamtoran/flippers)
 ![PyPI](https://img.shields.io/pypi/v/flippers)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/flippers)
 ![Code Style](https://img.shields.io/badge/code%20style-black-black)
 ![Read the Docs](https://img.shields.io/readthedocs/flippers)
 ![GitHub](https://img.shields.io/github/license/liamtoran/flippers)
 
-(in construction)
-
 `flippers` is a Python library for weak supervision, which allows you to leverage your domain knowledge, heuristics and other weak supervision sources to generate high-quality labels for your training data. 
 
 # Features
 `flippers` includes a number of features for weak supervision, including:
 - Simple tools to analyse your labeling functions,
 - Multiple label models including a from-scratch implementation of the label model used in the `snorkel` library and featuring enhanced ways to predict probabilities,
-- An extensive [documentation](https://flippers.readthedocs.io/en/latest/) with [tutorials](missing_link) and an [API reference](https://flippers.readthedocs.io/en/latest/reference/flippers.html).
+- An extensive [documentation](https://flippers.readthedocs.io/en/latest/) with [tutorials](https://github.com/liamtoran/flippers/tree/main/examples) and an [API reference](https://flippers.readthedocs.io/en/latest/reference/flippers.html).
 
 # Installation
 To install the latest version of `flippers`, simply run:
 
 ```bash
 pip install flippers
 ```
 
 # Quick Start 
 ## Documentation
-To quickly get started with `flippers`, you can begin by exploring the [documentation](https://flippers.readthedocs.io/en/latest/) and running through the [examples](missing_link) provided. The examples cover a variety of use cases and techniques, which can help you to get a feel for how to apply `flippers` to your own projects. 
+To quickly get started with `flippers`, you can begin by exploring the [documentation](https://flippers.readthedocs.io/en/latest/) and running through the [examples](hhttps://github.com/liamtoran/flippers/tree/main/examples) provided. The examples cover a variety of use cases and techniques, which can help you to get a feel for how to apply `flippers` to your own projects. 
 ## Example
 - Analyzing your labeling functions:
 ```python
 analysis = flippers.analyis(L_train)
 ```
 - Training a Label Model and doing inference:
 
 ```python
-label_model = flippers.models.SnorkelModel(polarities,  class_balances)
+label_model = flippers.models.SnorkelModel(polarities, class_balances)
 
 label_model.fit(L_train)
 
 label_model.predict_proba(L)
 ```
 
 # Discussion
 ## Troubleshooting
 If you have any questions or issues with `flippers`, please consult the [documentation](https://flippers.readthedocs.io/en/latest/) or reach out in the [GitHub issues](https://github.com/liamtoran/flippers/issues) page for support.
 
 
 ## Contributing
 
-`flippers` is an open-source project, and contributions are welcome! If you would like to contribute to `flippers`, please read the `CONTRIBUTING.md` file for guidelines and instructions.
+`flippers` is an open-source project, and contributions are welcome!
 
 ## Related projects
 - [wrench](https://github.com/JieyuZ2/wrench): A weak supervision library created by for benchmarking label models and weak supervision techniques. `flippers` uses its list of datasets as benchmarks.  
 - [snorkel](https://github.com/snorkel-team/snorkel): A cornerstone weak supervision library created by Snorkel in 2016, now sadly abandonned.
```

