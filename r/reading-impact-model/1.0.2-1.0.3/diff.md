# Comparing `tmp/reading_impact_model-1.0.2.tar.gz` & `tmp/reading_impact_model-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reading_impact_model-1.0.2.tar", max compression
+gzip compressed data, was "reading_impact_model-1.0.3.tar", max compression
```

## Comparing `reading_impact_model-1.0.2.tar` & `reading_impact_model-1.0.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     6941 2023-03-25 09:51:54.164506 reading_impact_model-1.0.2/README.md
--rw-r--r--   0        0        0     1185 2023-06-07 14:13:11.195598 reading_impact_model-1.0.2/pyproject.toml
--rw-r--r--   0        0        0       21 2023-06-07 14:13:11.195810 reading_impact_model-1.0.2/reading_impact_model/__init__.py
--rw-r--r--   0        0        0    21445 2023-03-25 09:23:34.833907 reading_impact_model-1.0.2/reading_impact_model/impact_model.py
--rw-r--r--   0        0        0        0 2023-03-21 06:20:35.500337 reading_impact_model-1.0.2/reading_impact_model/matchers/__init__.py
--rw-r--r--   0        0        0      203 2023-03-21 06:50:01.001599 reading_impact_model-1.0.2/reading_impact_model/matchers/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     5284 2023-03-22 13:46:51.249891 reading_impact_model-1.0.2/reading_impact_model/matchers/__pycache__/alpino_matcher.cpython-310.pyc
--rw-r--r--   0        0        0    14677 2023-06-07 14:11:05.000971 reading_impact_model-1.0.2/reading_impact_model/matchers/__pycache__/matcher.cpython-310.pyc
--rw-r--r--   0        0        0     1892 2023-06-07 14:03:03.744638 reading_impact_model-1.0.2/reading_impact_model/matchers/__pycache__/spacy_matcher.cpython-310.pyc
--rw-r--r--   0        0        0     4736 2023-03-22 13:16:07.552479 reading_impact_model-1.0.2/reading_impact_model/matchers/alpino_matcher.py
--rw-r--r--   0        0        0    11246 2023-03-21 06:24:13.469150 reading_impact_model-1.0.2/reading_impact_model/matchers/alpinor_matcher_old.py
--rw-r--r--   0        0        0    22038 2023-06-07 14:11:00.909291 reading_impact_model-1.0.2/reading_impact_model/matchers/matcher.py
--rw-r--r--   0        0        0      775 2023-03-21 06:27:57.741456 reading_impact_model-1.0.2/reading_impact_model/matchers/nltk_matcher.py
--rw-r--r--   0        0        0     1532 2023-06-07 13:49:21.112807 reading_impact_model-1.0.2/reading_impact_model/matchers/spacy_matcher.py
--rw-r--r--   0        0        0     1240 2023-03-22 13:17:03.674991 reading_impact_model-1.0.2/reading_impact_model/matchers/stanza_matcher.py
--rw-r--r--   0        0        0     1186 2023-03-22 13:17:03.671968 reading_impact_model-1.0.2/reading_impact_model/matchers/trankit_matcher.py
--rw-r--r--   0        0        0        0 2023-03-20 14:46:41.117875 reading_impact_model-1.0.2/reading_impact_model/model/__init__.py
--rw-r--r--   0        0        0     5589 2023-03-20 14:34:36.075954 reading_impact_model-1.0.2/reading_impact_model/model/phrase.py
--rw-r--r--   0        0        0        0 2023-03-20 14:46:41.124577 reading_impact_model-1.0.2/reading_impact_model/models/__init__.py
--rw-r--r--   0        0        0      201 2023-03-20 14:55:07.896122 reading_impact_model-1.0.2/reading_impact_model/models/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0   619876 2023-03-20 14:55:07.939597 reading_impact_model-1.0.2/reading_impact_model/models/__pycache__/impact_model_en.cpython-310.pyc
--rw-r--r--   0        0        0   160274 2023-03-20 14:55:07.905894 reading_impact_model-1.0.2/reading_impact_model/models/__pycache__/impact_model_nl.cpython-310.pyc
--rw-r--r--   0        0        0   356666 2020-06-19 22:04:56.168319 reading_impact_model-1.0.2/reading_impact_model/models/impact_model-en-0.1.pcl
--rw-r--r--   0        0        0   209835 2021-04-20 14:51:48.208246 reading_impact_model-1.0.2/reading_impact_model/models/impact_model-en-0.2.pcl
--rw-r--r--   0        0        0   230737 2021-07-02 13:07:05.214976 reading_impact_model-1.0.2/reading_impact_model/models/impact_model-en-0.3.pcl
--rw-r--r--   0        0        0   230678 2021-07-05 10:41:51.476919 reading_impact_model-1.0.2/reading_impact_model/models/impact_model-en-0.4.pcl
--rw-r--r--   0        0        0   230690 2021-07-06 11:33:29.799021 reading_impact_model-1.0.2/reading_impact_model/models/impact_model-en-0.5.pcl
--rw-r--r--   0        0        0   692078 2021-10-25 11:59:27.603446 reading_impact_model-1.0.2/reading_impact_model/models/impact_model-en-0.6.json
--rw-r--r--   0        0        0   579958 2021-10-25 11:59:27.554350 reading_impact_model-1.0.2/reading_impact_model/models/impact_model-en-0.6.pcl
--rw-r--r--   0        0        0   691857 2023-03-21 09:49:00.251013 reading_impact_model-1.0.2/reading_impact_model/models/impact_model-en-0.7.json
--rw-r--r--   0        0        0   621720 2023-03-21 09:49:00.228629 reading_impact_model-1.0.2/reading_impact_model/models/impact_model-en-0.7.pcl
--rw-r--r--   0        0        0   691857 2023-03-21 09:49:00.264532 reading_impact_model-1.0.2/reading_impact_model/models/impact_model-en.json
--rw-r--r--   0        0        0   621720 2023-03-21 09:49:00.234743 reading_impact_model-1.0.2/reading_impact_model/models/impact_model-en.pcl
--rw-r--r--   0        0        0   244747 2021-10-25 11:40:57.657433 reading_impact_model-1.0.2/reading_impact_model/models/impact_model-nl-1.0.json
--rw-r--r--   0        0        0   244747 2021-10-25 11:40:57.645116 reading_impact_model-1.0.2/reading_impact_model/models/impact_model-nl.json
--rw-r--r--   0        0        0   176064 2020-05-19 14:38:46.549523 reading_impact_model-1.0.2/reading_impact_model/models/impact_model-nl.pcl
--rw-r--r--   0        0        0   692090 2021-10-25 11:59:46.390314 reading_impact_model-1.0.2/reading_impact_model/models/impact_model_en.py
--rw-r--r--   0        0        0   244764 2023-03-20 14:34:33.867788 reading_impact_model-1.0.2/reading_impact_model/models/impact_model_nl.py
--rw-r--r--   0        0        0      903 2023-03-21 06:24:13.480622 reading_impact_model-1.0.2/reading_impact_model/reading_impact.py
--rw-r--r--   0        0        0     7806 1970-01-01 00:00:00.000000 reading_impact_model-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     6941 2023-03-25 09:51:54.164506 reading_impact_model-1.0.3/README.md
+-rw-r--r--   0        0        0     1185 2023-06-07 14:21:48.669047 reading_impact_model-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-06-07 14:21:48.669253 reading_impact_model-1.0.3/reading_impact_model/__init__.py
+-rw-r--r--   0        0        0    21445 2023-03-25 09:23:34.833907 reading_impact_model-1.0.3/reading_impact_model/impact_model.py
+-rw-r--r--   0        0        0        0 2023-03-21 06:20:35.500337 reading_impact_model-1.0.3/reading_impact_model/matchers/__init__.py
+-rw-r--r--   0        0        0      203 2023-03-21 06:50:01.001599 reading_impact_model-1.0.3/reading_impact_model/matchers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     5284 2023-03-22 13:46:51.249891 reading_impact_model-1.0.3/reading_impact_model/matchers/__pycache__/alpino_matcher.cpython-310.pyc
+-rw-r--r--   0        0        0    14687 2023-06-07 14:21:00.015137 reading_impact_model-1.0.3/reading_impact_model/matchers/__pycache__/matcher.cpython-310.pyc
+-rw-r--r--   0        0        0     1892 2023-06-07 14:03:03.744638 reading_impact_model-1.0.3/reading_impact_model/matchers/__pycache__/spacy_matcher.cpython-310.pyc
+-rw-r--r--   0        0        0     4736 2023-03-22 13:16:07.552479 reading_impact_model-1.0.3/reading_impact_model/matchers/alpino_matcher.py
+-rw-r--r--   0        0        0    11246 2023-03-21 06:24:13.469150 reading_impact_model-1.0.3/reading_impact_model/matchers/alpinor_matcher_old.py
+-rw-r--r--   0        0        0    22105 2023-06-07 14:19:20.706865 reading_impact_model-1.0.3/reading_impact_model/matchers/matcher.py
+-rw-r--r--   0        0        0      775 2023-03-21 06:27:57.741456 reading_impact_model-1.0.3/reading_impact_model/matchers/nltk_matcher.py
+-rw-r--r--   0        0        0     1532 2023-06-07 13:49:21.112807 reading_impact_model-1.0.3/reading_impact_model/matchers/spacy_matcher.py
+-rw-r--r--   0        0        0     1240 2023-03-22 13:17:03.674991 reading_impact_model-1.0.3/reading_impact_model/matchers/stanza_matcher.py
+-rw-r--r--   0        0        0     1186 2023-03-22 13:17:03.671968 reading_impact_model-1.0.3/reading_impact_model/matchers/trankit_matcher.py
+-rw-r--r--   0        0        0        0 2023-03-20 14:46:41.117875 reading_impact_model-1.0.3/reading_impact_model/model/__init__.py
+-rw-r--r--   0        0        0     5589 2023-03-20 14:34:36.075954 reading_impact_model-1.0.3/reading_impact_model/model/phrase.py
+-rw-r--r--   0        0        0        0 2023-03-20 14:46:41.124577 reading_impact_model-1.0.3/reading_impact_model/models/__init__.py
+-rw-r--r--   0        0        0      201 2023-03-20 14:55:07.896122 reading_impact_model-1.0.3/reading_impact_model/models/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0   619876 2023-03-20 14:55:07.939597 reading_impact_model-1.0.3/reading_impact_model/models/__pycache__/impact_model_en.cpython-310.pyc
+-rw-r--r--   0        0        0   160274 2023-03-20 14:55:07.905894 reading_impact_model-1.0.3/reading_impact_model/models/__pycache__/impact_model_nl.cpython-310.pyc
+-rw-r--r--   0        0        0   356666 2020-06-19 22:04:56.168319 reading_impact_model-1.0.3/reading_impact_model/models/impact_model-en-0.1.pcl
+-rw-r--r--   0        0        0   209835 2021-04-20 14:51:48.208246 reading_impact_model-1.0.3/reading_impact_model/models/impact_model-en-0.2.pcl
+-rw-r--r--   0        0        0   230737 2021-07-02 13:07:05.214976 reading_impact_model-1.0.3/reading_impact_model/models/impact_model-en-0.3.pcl
+-rw-r--r--   0        0        0   230678 2021-07-05 10:41:51.476919 reading_impact_model-1.0.3/reading_impact_model/models/impact_model-en-0.4.pcl
+-rw-r--r--   0        0        0   230690 2021-07-06 11:33:29.799021 reading_impact_model-1.0.3/reading_impact_model/models/impact_model-en-0.5.pcl
+-rw-r--r--   0        0        0   692078 2021-10-25 11:59:27.603446 reading_impact_model-1.0.3/reading_impact_model/models/impact_model-en-0.6.json
+-rw-r--r--   0        0        0   579958 2021-10-25 11:59:27.554350 reading_impact_model-1.0.3/reading_impact_model/models/impact_model-en-0.6.pcl
+-rw-r--r--   0        0        0   691857 2023-03-21 09:49:00.251013 reading_impact_model-1.0.3/reading_impact_model/models/impact_model-en-0.7.json
+-rw-r--r--   0        0        0   621720 2023-03-21 09:49:00.228629 reading_impact_model-1.0.3/reading_impact_model/models/impact_model-en-0.7.pcl
+-rw-r--r--   0        0        0   691857 2023-03-21 09:49:00.264532 reading_impact_model-1.0.3/reading_impact_model/models/impact_model-en.json
+-rw-r--r--   0        0        0   621720 2023-03-21 09:49:00.234743 reading_impact_model-1.0.3/reading_impact_model/models/impact_model-en.pcl
+-rw-r--r--   0        0        0   244747 2021-10-25 11:40:57.657433 reading_impact_model-1.0.3/reading_impact_model/models/impact_model-nl-1.0.json
+-rw-r--r--   0        0        0   244747 2021-10-25 11:40:57.645116 reading_impact_model-1.0.3/reading_impact_model/models/impact_model-nl.json
+-rw-r--r--   0        0        0   176064 2020-05-19 14:38:46.549523 reading_impact_model-1.0.3/reading_impact_model/models/impact_model-nl.pcl
+-rw-r--r--   0        0        0   692090 2021-10-25 11:59:46.390314 reading_impact_model-1.0.3/reading_impact_model/models/impact_model_en.py
+-rw-r--r--   0        0        0   244764 2023-03-20 14:34:33.867788 reading_impact_model-1.0.3/reading_impact_model/models/impact_model_nl.py
+-rw-r--r--   0        0        0      903 2023-03-21 06:24:13.480622 reading_impact_model-1.0.3/reading_impact_model/reading_impact.py
+-rw-r--r--   0        0        0     7806 1970-01-01 00:00:00.000000 reading_impact_model-1.0.3/PKG-INFO
```

### Comparing `reading_impact_model-1.0.2/README.md` & `reading_impact_model-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.2/pyproject.toml` & `reading_impact_model-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reading-impact-model"
-version = "1.0.2"
+version = "1.0.3"
 description = ""
 authors = ["Marijn Koolen <marijn.koolen@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/marijnkoolen/reading-impact-model"
 repository = "https://github.com/marijnkoolen/reading-impact-model"
 classifiers = [
@@ -26,15 +26,15 @@
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.bumpver]
-current_version = "1.0.2"
+current_version = "1.0.3"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `reading_impact_model-1.0.2/reading_impact_model/impact_model.py` & `reading_impact_model-1.0.3/reading_impact_model/impact_model.py`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.2/reading_impact_model/matchers/__pycache__/alpino_matcher.cpython-310.pyc` & `reading_impact_model-1.0.3/reading_impact_model/matchers/__pycache__/alpino_matcher.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.2/reading_impact_model/matchers/__pycache__/matcher.cpython-310.pyc` & `reading_impact_model-1.0.3/reading_impact_model/matchers/__pycache__/matcher.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Jun  7 14:11:00 2023 UTC, .py size: 22038 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 f48f 8064 1656 0000  o..........d.V..
+00000000: 6f0d 0d0a 0000 0000 e891 8064 5956 0000  o..........dYV..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 b200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 6d05 5a05  ..d.d.l.m.Z.m.Z.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c09 6d0a 5a0a 6d0b 5a0b  ..d.d.l.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 0100 6400  m.Z.m.Z.m.Z...d.
@@ -120,15 +120,15 @@
 00000770: 6417 6503 6418 6515 651d 1900 6608 6436  d.e.d.e.e...f.d6
 00000780: 6437 8405 5a1e 6418 6515 651d 1900 6602  d7..Z.d.e.e...f.
 00000790: 6438 6439 8404 5a1f 6435 6507 6602 643a  d8d9..Z.d5e.f.d:
 000007a0: 643b 8404 5a20 6435 6507 643c 651d 6604  d;..Z d5e.d<e.f.
 000007b0: 643d 643e 8404 5a21 6435 6507 643c 651d  d=d>..Z!d5e.d<e.
 000007c0: 6418 6505 6606 643f 6440 8404 5a22 6435  d.e.f.d?d@..Z"d5
 000007d0: 6507 643c 651d 6418 6505 6606 6441 6442  e.d<e.d.e.f.dAdB
-000007e0: 8404 5a23 6443 651d 6418 650d 6503 650f  ..Z#dCe.d.e.e.e.
+000007e0: 8404 5a23 6443 651d 6418 650d 6503 650e  ..Z#dCe.d.e.e.e.
 000007f0: 6602 1900 6604 6444 6445 8404 5a24 0903  f...f.dDdE..Z$..
 00000800: 6450 6446 6515 651d 1900 6424 6505 6418  dPdFe.e...d$e.d.
 00000810: 6515 650d 6503 650e 6602 1900 1900 6606  e.e.e.e.f.....f.
 00000820: 6447 6448 8405 5a25 6402 5300 2951 da0d  dGdH..Z%d.S.)Q..
 00000830: 496d 7061 6374 4d61 7463 6865 72da 0265  ImpactMatcher..e
 00000840: 6e4e 46da 046c 616e 67da 0c69 6d70 6163  nNF..lang..impac
 00000850: 745f 6d6f 6465 6cda 0564 6562 7567 6304  t_model..debugc.
@@ -830,89 +830,89 @@
 000033d0: 0000 00da 1269 6e69 745f 696d 7061 6374  .....init_impact
 000033e0: 5f73 636f 7265 739f 0100 0073 1c00 0000  _scores....s....
 000033f0: 0402 0401 0401 06fd 0e05 0a01 0801 1001  ................
 00003400: 0801 0e01 1801 1401 0280 0401 7a20 496d  ............z Im
 00003410: 7061 6374 4d61 7463 6865 722e 696e 6974  pactMatcher.init
 00003420: 5f69 6d70 6163 745f 7363 6f72 6573 7296  _impact_scoresr.
 00003430: 0000 0063 0300 0000 0000 0000 0000 0000  ...c............
-00003440: 0c00 0000 0500 0000 4300 0000 7334 0100  ........C...s4..
+00003440: 0c00 0000 0500 0000 4300 0000 733e 0100  ........C...s>..
 00003450: 0068 0064 01a3 017d 0367 007d 0474 0083  .h.d...}.g.}.t..
-00003460: 007d 057c 0144 005d 8c7d 067c 00a0 017c  .}.|.D.].}.|...|
+00003460: 007d 057c 0144 005d 917d 067c 00a0 017c  .}.|.D.].}.|...|
 00003470: 06a1 017d 077c 0264 0275 0072 1c7c 066a  ...}.|.d.u.r.|.j
 00003480: 0264 036b 0272 1c71 0b7c 066a 037d 0674  .d.k.r.q.|.j.}.t
 00003490: 0444 005d 087d 087c 067c 0819 007c 077c  .D.].}.|.|...|.|
-000034a0: 083c 0071 2174 0544 005d 247d 0964 047c  .<.q!t.D.]$}.d.|
-000034b0: 0676 0072 5074 067c 0664 0419 0083 0164  .v.rPt.|.d.....d
-000034c0: 056b 0472 507c 09a0 0764 06a1 0172 417c  .k.rP|...d...rA|
-000034d0: 096e 0464 077c 099b 009d 027d 0a7c 0664  .n.d.|.....}.|.d
-000034e0: 0419 0064 0519 007c 0919 007c 077c 0a3c  ...d...|...|.|.<
-000034f0: 0071 2c7c 0664 0819 0064 036b 0272 5871  .q,|.d...d.k.rXq
-00003500: 0b74 087c 0683 017d 0b7c 0664 0919 007c  .t.|...}.|.d...|
-00003510: 0b66 027c 0576 0172 757c 077c 0b05 0019  .f.|.v.ru|.|....
-00003520: 0064 0a37 0003 003c 007c 05a0 097c 0664  .d.7...<.|...|.d
-00003530: 0919 007c 0b66 02a1 0101 007c 0b7c 0376  ...|.f.....|.|.v
-00003540: 0072 927c 0664 0919 0064 0b66 027c 0576  .r.|.d...d.f.|.v
-00003550: 0172 927c 0764 0b05 0019 0064 0a37 0003  .r.|.d.....d.7..
-00003560: 003c 007c 05a0 097c 0664 0919 0064 0b66  .<.|...|.d...d.f
-00003570: 02a1 0101 007c 04a0 0a7c 07a1 0101 0071  .....|...|.....q
-00003580: 0b7c 0453 0029 0c4e 3e03 0000 00da 0573  .|.S.).N>......s
-00003590: 7479 6c65 da09 6e61 7272 6174 6976 65da  tyle..narrative.
-000035a0: 0568 756d 6f72 46da 074e 6575 7472 616c  .humorF..Neutral
-000035b0: 72a1 0000 0072 0100 0000 72a2 0000 0072  r....r....r....r
-000035c0: a300 0000 7212 0000 00da 0b6d 6174 6368  ....r......match
-000035d0: 5f69 6e64 6578 7245 0000 0072 1400 0000  _indexrE...r....
-000035e0: 290b 7234 0000 0072 aa00 0000 7212 0000  ).r4...r....r...
-000035f0: 00da 046a 736f 6e72 0d00 0000 720e 0000  ...jsonr....r...
-00003600: 0072 9f00 0000 72a5 0000 0072 1900 0000  .r....r....r....
-00003610: 7253 0000 0072 4f00 0000 290c 723b 0000  rS...rO...).r;..
-00003620: 0072 9600 0000 726a 0000 005a 1070 6f73  .r....rj...Z.pos
-00003630: 6974 6976 655f 7375 625f 6361 7472 6f00  itive_sub_catro.
-00003640: 0000 5a07 636f 756e 7465 6472 1600 0000  ..Z.countedr....
-00003650: 72a6 0000 0072 a700 0000 72a8 0000 0072  r....r....r....r
-00003660: a900 0000 7212 0000 0072 1700 0000 7217  ....r....r....r.
-00003670: 0000 0072 1800 0000 726d 0000 00af 0100  ...r....rm......
-00003680: 0073 3600 0000 0802 0401 0601 0801 0a01  .s6.............
-00003690: 1201 0201 0601 0801 0e01 0801 1801 1801  ................
-000036a0: 1401 0280 0c01 0201 0801 1001 1001 1201  ................
-000036b0: 0801 1001 1001 1201 0c01 0401 7a23 496d  ............z#Im
-000036c0: 7061 6374 4d61 7463 6865 722e 636f 6d70  pactMatcher.comp
-000036d0: 7574 655f 7265 7669 6577 5f69 6d70 6163  ute_review_impac
-000036e0: 7429 0372 2900 0000 4e46 2902 4e4e 7249  t).r)...NF).NNrI
-000036f0: 0000 0029 024e 4629 0154 2902 727b 0000  ...).NF).T).r{..
-00003700: 0054 2903 4e4e 4e29 0146 2926 da08 5f5f  .T).NNN).F)&..__
-00003710: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-00003720: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-00003730: 7252 0000 0072 0700 0000 da04 626f 6f6c  rR...r......bool
-00003740: 723c 0000 0072 0800 0000 7248 0000 0072  r<...r....rH...r
-00003750: 3a00 0000 724e 0000 0072 0b00 0000 7256  :...rN...r....rV
-00003760: 0000 0072 0300 0000 da03 616e 7972 3600  ...r......anyr6.
-00003770: 0000 725f 0000 0072 6100 0000 7263 0000  ..r_...ra...rc..
-00003780: 0072 6600 0000 7269 0000 0072 0400 0000  .rf...ri...r....
-00003790: 7270 0000 0072 7300 0000 7277 0000 0072  rp...rs...rw...r
-000037a0: 7a00 0000 7285 0000 0072 8600 0000 726b  z...r....r....rk
-000037b0: 0000 0072 0900 0000 7287 0000 0072 8b00  ...r....r....r..
-000037c0: 0000 728c 0000 0072 9200 0000 729b 0000  ..r....r....r...
-000037d0: 0072 9c00 0000 72aa 0000 0072 6d00 0000  .r....r....rm...
-000037e0: 7217 0000 0072 1700 0000 7217 0000 0072  r....r....r....r
-000037f0: 1800 0000 7228 0000 0037 0000 0073 5600  ....r(...7...sV.
-00003800: 0000 0800 1802 161e 0812 0807 0e0b 2211  ..............".
-00003810: 1a09 080c 1c07 140b 0208 0201 0cff 0201  ................
-00003820: 02ff 0e01 0aff 0a0a 0a0b 0a0b 0a1c 0818  ................
-00003830: 0805 0206 0201 0cff 0201 02ff 0601 0aff  ................
-00003840: 120e 0e13 1217 161e 161b 1a14 0211 0cff  ................
-00003850: 0201 02ff 0e01 0eff 7228 0000 0029 1a72  ........r(...).r
-00003860: 2400 0000 da0b 636f 6c6c 6563 7469 6f6e  $.....collection
-00003870: 7372 0200 0000 da06 7479 7069 6e67 7203  sr......typingr.
-00003880: 0000 0072 0400 0000 7205 0000 005a 0d6e  ...r....r....Z.n
-00003890: 6c74 6b2e 746f 6b65 6e69 7a65 7206 0000  ltk.tokenizer...
-000038a0: 005a 2172 6561 6469 6e67 5f69 6d70 6163  .Z!reading_impac
-000038b0: 745f 6d6f 6465 6c2e 696d 7061 6374 5f6d  t_model.impact_m
-000038c0: 6f64 656c 7207 0000 0072 0800 0000 7209  odelr....r....r.
-000038d0: 0000 0072 0a00 0000 720b 0000 0072 0c00  ...r....r....r..
-000038e0: 0000 720d 0000 0072 0e00 0000 720f 0000  ..r....r....r...
-000038f0: 0072 1000 0000 7211 0000 0072 1900 0000  .r....r....r....
-00003900: 721f 0000 0072 2300 0000 7227 0000 0072  r....r#...r'...r
-00003910: 2800 0000 7217 0000 0072 1700 0000 7217  (...r....r....r.
-00003920: 0000 0072 1800 0000 da08 3c6d 6f64 756c  ...r......<modul
-00003930: 653e 0100 0000 731a 0000 0008 000c 0114  e>....s.........
-00003940: 010c 021c 0214 010c 0110 0108 0308 0708  ................
-00003950: 0f08 0f12 05                             .....
+000034a0: 083c 0071 2174 0544 005d 297d 097c 09a0  .<.q!t.D.])}.|..
+000034b0: 0664 04a1 0172 357c 096e 0464 057c 099b  .d...r5|.n.d.|..
+000034c0: 009d 027d 0a64 067c 0676 0072 5174 077c  ...}.d.|.v.rQt.|
+000034d0: 0664 0619 0083 0164 076b 0472 517c 0664  .d.....d.k.rQ|.d
+000034e0: 0619 0064 0719 007c 0919 007c 077c 0a3c  ...d...|...|.|.<
+000034f0: 0071 2c64 007c 077c 0a3c 0071 2c7c 0664  .q,d.|.|.<.q,|.d
+00003500: 0819 0064 036b 0272 5d71 0b74 087c 0683  ...d.k.r]q.t.|..
+00003510: 017d 0b7c 0664 0919 007c 0b66 027c 0576  .}.|.d...|.f.|.v
+00003520: 0172 7a7c 077c 0b05 0019 0064 0a37 0003  .rz|.|.....d.7..
+00003530: 003c 007c 05a0 097c 0664 0919 007c 0b66  .<.|...|.d...|.f
+00003540: 02a1 0101 007c 0b7c 0376 0072 977c 0664  .....|.|.v.r.|.d
+00003550: 0919 0064 0b66 027c 0576 0172 977c 0764  ...d.f.|.v.r.|.d
+00003560: 0b05 0019 0064 0a37 0003 003c 007c 05a0  .....d.7...<.|..
+00003570: 097c 0664 0919 0064 0b66 02a1 0101 007c  .|.d...d.f.....|
+00003580: 04a0 0a7c 07a1 0101 0071 0b7c 0453 0029  ...|.....q.|.S.)
+00003590: 0c4e 3e03 0000 00da 096e 6172 7261 7469  .N>......narrati
+000035a0: 7665 da05 6875 6d6f 72da 0573 7479 6c65  ve..humor..style
+000035b0: 46da 074e 6575 7472 616c 72a2 0000 0072  F..Neutralr....r
+000035c0: a300 0000 72a1 0000 0072 0100 0000 7212  ....r....r....r.
+000035d0: 0000 00da 0b6d 6174 6368 5f69 6e64 6578  .....match_index
+000035e0: 7245 0000 0072 1400 0000 290b 7234 0000  rE...r....).r4..
+000035f0: 0072 aa00 0000 7212 0000 00da 046a 736f  .r....r......jso
+00003600: 6e72 0d00 0000 720e 0000 0072 a500 0000  nr....r....r....
+00003610: 729f 0000 0072 1900 0000 7253 0000 0072  r....r....rS...r
+00003620: 4f00 0000 290c 723b 0000 0072 9600 0000  O...).r;...r....
+00003630: 726a 0000 005a 1070 6f73 6974 6976 655f  rj...Z.positive_
+00003640: 7375 625f 6361 7472 6f00 0000 5a07 636f  sub_catro...Z.co
+00003650: 756e 7465 6472 1600 0000 72a6 0000 0072  untedr....r....r
+00003660: a700 0000 72a8 0000 0072 a900 0000 7212  ....r....r....r.
+00003670: 0000 0072 1700 0000 7217 0000 0072 1800  ...r....r....r..
+00003680: 0000 726d 0000 00af 0100 0073 3600 0000  ..rm.......s6...
+00003690: 0802 0401 0601 0801 0a01 1201 0201 0601  ................
+000036a0: 0801 0e01 0801 1801 1801 1601 0a02 0c01  ................
+000036b0: 0201 0801 1001 1001 1201 0801 1001 1001  ................
+000036c0: 1201 0c01 0401 7a23 496d 7061 6374 4d61  ......z#ImpactMa
+000036d0: 7463 6865 722e 636f 6d70 7574 655f 7265  tcher.compute_re
+000036e0: 7669 6577 5f69 6d70 6163 7429 0372 2900  view_impact).r).
+000036f0: 0000 4e46 2902 4e4e 7249 0000 0029 024e  ..NF).NNrI...).N
+00003700: 4629 0154 2902 727b 0000 0054 2903 4e4e  F).T).r{...T).NN
+00003710: 4e29 0146 2926 da08 5f5f 6e61 6d65 5f5f  N).F)&..__name__
+00003720: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+00003730: 7175 616c 6e61 6d65 5f5f 7252 0000 0072  qualname__rR...r
+00003740: 0700 0000 da04 626f 6f6c 723c 0000 0072  ......boolr<...r
+00003750: 0800 0000 7248 0000 0072 3a00 0000 724e  ....rH...r:...rN
+00003760: 0000 0072 0b00 0000 7256 0000 0072 0300  ...r....rV...r..
+00003770: 0000 da03 616e 7972 3600 0000 725f 0000  ....anyr6...r_..
+00003780: 0072 6100 0000 7263 0000 0072 6600 0000  .ra...rc...rf...
+00003790: 7269 0000 0072 0400 0000 7270 0000 0072  ri...r....rp...r
+000037a0: 7300 0000 7277 0000 0072 7a00 0000 7285  s...rw...rz...r.
+000037b0: 0000 0072 8600 0000 726b 0000 0072 0900  ...r....rk...r..
+000037c0: 0000 7287 0000 0072 8b00 0000 728c 0000  ..r....r....r...
+000037d0: 0072 9200 0000 729b 0000 0072 9c00 0000  .r....r....r....
+000037e0: 72aa 0000 0072 6d00 0000 7217 0000 0072  r....rm...r....r
+000037f0: 1700 0000 7217 0000 0072 1800 0000 7228  ....r....r....r(
+00003800: 0000 0037 0000 0073 5600 0000 0800 1802  ...7...sV.......
+00003810: 161e 0812 0807 0e0b 2211 1a09 080c 1c07  ........".......
+00003820: 140b 0208 0201 0cff 0201 02ff 0e01 0aff  ................
+00003830: 0a0a 0a0b 0a0b 0a1c 0818 0805 0206 0201  ................
+00003840: 0cff 0201 02ff 0601 0aff 120e 0e13 1217  ................
+00003850: 161e 161b 1a14 0211 0cff 0201 02ff 0e01  ................
+00003860: 0eff 7228 0000 0029 1a72 2400 0000 da0b  ..r(...).r$.....
+00003870: 636f 6c6c 6563 7469 6f6e 7372 0200 0000  collectionsr....
+00003880: da06 7479 7069 6e67 7203 0000 0072 0400  ..typingr....r..
+00003890: 0000 7205 0000 005a 0d6e 6c74 6b2e 746f  ..r....Z.nltk.to
+000038a0: 6b65 6e69 7a65 7206 0000 00da 2172 6561  kenizer.....!rea
+000038b0: 6469 6e67 5f69 6d70 6163 745f 6d6f 6465  ding_impact_mode
+000038c0: 6c2e 696d 7061 6374 5f6d 6f64 656c 7207  l.impact_modelr.
+000038d0: 0000 0072 0800 0000 7209 0000 0072 0a00  ...r....r....r..
+000038e0: 0000 720b 0000 0072 0c00 0000 720d 0000  ..r....r....r...
+000038f0: 0072 0e00 0000 720f 0000 0072 1000 0000  .r....r....r....
+00003900: 7211 0000 0072 1900 0000 721f 0000 0072  r....r....r....r
+00003910: 2300 0000 7227 0000 0072 2800 0000 7217  #...r'...r(...r.
+00003920: 0000 0072 1700 0000 7217 0000 0072 1800  ...r....r....r..
+00003930: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00003940: 731a 0000 0008 000c 0114 010c 021c 0214  s...............
+00003950: 010c 0110 0108 0308 0708 0f08 0f12 05    ...............
```

### Comparing `reading_impact_model-1.0.2/reading_impact_model/matchers/__pycache__/spacy_matcher.cpython-310.pyc` & `reading_impact_model-1.0.3/reading_impact_model/matchers/__pycache__/spacy_matcher.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.2/reading_impact_model/matchers/alpino_matcher.py` & `reading_impact_model-1.0.3/reading_impact_model/matchers/alpino_matcher.py`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.2/reading_impact_model/matchers/alpinor_matcher_old.py` & `reading_impact_model-1.0.3/reading_impact_model/matchers/alpinor_matcher_old.py`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.2/reading_impact_model/matchers/matcher.py` & `reading_impact_model-1.0.3/reading_impact_model/matchers/matcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -408,15 +408,15 @@
             condition_matches.append(condition_match)
         if len(condition_matches) > 0:
             impact_match.condition_matches = condition_matches
             return True
         else:
             return False
 
-    def init_impact_scores(self, match: ImpactMatch) -> Dict[str, int]:
+    def init_impact_scores(self, match: ImpactMatch) -> Dict[str, any]:
         impact = {
             "doc_id": match.doc_id,
             "sentence_index": match.sentence_index,
             "sentence": match.sentence,
         }
         for impact_type in IMPACT_TYPES[self.lang]:
             impact[impact_type] = 0
@@ -437,17 +437,19 @@
             impact = self.init_impact_scores(match)
             if include_neutral is False and match.impact_type == 'Neutral':
                 continue
             match = match.json
             for field in IMPACT_MATCH_FIELDS:
                 impact[field] = match[field]
             for cond_field in CONDITION_MATCH_FIELDS:
+                display_field = cond_field if cond_field.startswith('cond') else f'condition_{cond_field}'
                 if 'condition_match' in match and len(match['condition_match']) > 0:
-                    display_field = cond_field if cond_field.startswith('cond') else f'condition_{cond_field}'
                     impact[display_field] = match['condition_match'][0][cond_field]
+                else:
+                    impact[display_field] = None
             if match['impact_type'] == 'Neutral':
                 continue
             impact_type = map_review_impact(match)
             if (match['match_index'], impact_type) not in counted:
                 impact[impact_type] += 1
                 counted.add((match['match_index'], impact_type))
             if impact_type in positive_sub_cat:
```

### Comparing `reading_impact_model-1.0.2/reading_impact_model/matchers/nltk_matcher.py` & `reading_impact_model-1.0.3/reading_impact_model/matchers/nltk_matcher.py`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.2/reading_impact_model/matchers/spacy_matcher.py` & `reading_impact_model-1.0.3/reading_impact_model/matchers/spacy_matcher.py`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.2/reading_impact_model/matchers/stanza_matcher.py` & `reading_impact_model-1.0.3/reading_impact_model/matchers/stanza_matcher.py`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.2/reading_impact_model/matchers/trankit_matcher.py` & `reading_impact_model-1.0.3/reading_impact_model/matchers/trankit_matcher.py`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.2/reading_impact_model/model/phrase.py` & `reading_impact_model-1.0.3/reading_impact_model/model/phrase.py`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.2/reading_impact_model/models/__pycache__/impact_model_en.cpython-310.pyc` & `reading_impact_model-1.0.3/reading_impact_model/models/__pycache__/impact_model_en.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.2/reading_impact_model/models/__pycache__/impact_model_nl.cpython-310.pyc` & `reading_impact_model-1.0.3/reading_impact_model/models/__pycache__/impact_model_nl.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.2/reading_impact_model/models/impact_model-en-0.1.pcl` & `reading_impact_model-1.0.3/reading_impact_model/models/impact_model-en-0.1.pcl`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.2/reading_impact_model/models/impact_model-en-0.2.pcl` & `reading_impact_model-1.0.3/reading_impact_model/models/impact_model-en-0.2.pcl`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.2/reading_impact_model/models/impact_model-en-0.3.pcl` & `reading_impact_model-1.0.3/reading_impact_model/models/impact_model-en-0.3.pcl`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.2/reading_impact_model/models/impact_model-en-0.4.pcl` & `reading_impact_model-1.0.3/reading_impact_model/models/impact_model-en-0.4.pcl`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.2/reading_impact_model/models/impact_model-en-0.5.pcl` & `reading_impact_model-1.0.3/reading_impact_model/models/impact_model-en-0.5.pcl`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.2/reading_impact_model/models/impact_model-en-0.6.json` & `reading_impact_model-1.0.3/reading_impact_model/models/impact_model-en-0.6.json`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.2/reading_impact_model/models/impact_model-en-0.6.pcl` & `reading_impact_model-1.0.3/reading_impact_model/models/impact_model-en-0.6.pcl`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.2/reading_impact_model/models/impact_model-en-0.7.json` & `reading_impact_model-1.0.3/reading_impact_model/models/impact_model-en-0.7.json`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.2/reading_impact_model/models/impact_model-en-0.7.pcl` & `reading_impact_model-1.0.3/reading_impact_model/models/impact_model-en-0.7.pcl`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.2/reading_impact_model/models/impact_model-en.json` & `reading_impact_model-1.0.3/reading_impact_model/models/impact_model-en.json`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.2/reading_impact_model/models/impact_model-en.pcl` & `reading_impact_model-1.0.3/reading_impact_model/models/impact_model-en.pcl`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.2/reading_impact_model/models/impact_model-nl-1.0.json` & `reading_impact_model-1.0.3/reading_impact_model/models/impact_model-nl-1.0.json`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.2/reading_impact_model/models/impact_model-nl.json` & `reading_impact_model-1.0.3/reading_impact_model/models/impact_model-nl.json`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.2/reading_impact_model/models/impact_model-nl.pcl` & `reading_impact_model-1.0.3/reading_impact_model/models/impact_model-nl.pcl`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.2/reading_impact_model/models/impact_model_en.py` & `reading_impact_model-1.0.3/reading_impact_model/models/impact_model_en.py`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.2/reading_impact_model/models/impact_model_nl.py` & `reading_impact_model-1.0.3/reading_impact_model/models/impact_model_nl.py`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.2/reading_impact_model/reading_impact.py` & `reading_impact_model-1.0.3/reading_impact_model/reading_impact.py`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.2/PKG-INFO` & `reading_impact_model-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reading-impact-model
-Version: 1.0.2
+Version: 1.0.3
 Summary: 
 Home-page: https://github.com/marijnkoolen/reading-impact-model
 License: MIT
 Author: Marijn Koolen
 Author-email: marijn.koolen@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: reading-impact-model Version: 1.0.2 Summary: Home-
+Metadata-Version: 2.1 Name: reading-impact-model Version: 1.0.3 Summary: Home-
 page: https://github.com/marijnkoolen/reading-impact-model License: MIT Author:
 Marijn Koolen Author-email: marijn.koolen@gmail.com Requires-Python:
 >=3.10,<4.0 Classifier: Development Status :: 4 - Beta Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Topic :: Scientific/
```

