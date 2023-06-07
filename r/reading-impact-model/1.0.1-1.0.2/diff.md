# Comparing `tmp/reading_impact_model-1.0.1.tar.gz` & `tmp/reading_impact_model-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reading_impact_model-1.0.1.tar", max compression
+gzip compressed data, was "reading_impact_model-1.0.2.tar", max compression
```

## Comparing `reading_impact_model-1.0.1.tar` & `reading_impact_model-1.0.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     6941 2023-03-25 09:51:54.164506 reading_impact_model-1.0.1/README.md
--rw-r--r--   0        0        0     1185 2023-06-07 13:55:29.913779 reading_impact_model-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       21 2023-06-07 13:55:29.913977 reading_impact_model-1.0.1/reading_impact_model/__init__.py
--rw-r--r--   0        0        0    21445 2023-03-25 09:23:34.833907 reading_impact_model-1.0.1/reading_impact_model/impact_model.py
--rw-r--r--   0        0        0        0 2023-03-21 06:20:35.500337 reading_impact_model-1.0.1/reading_impact_model/matchers/__init__.py
--rw-r--r--   0        0        0      203 2023-03-21 06:50:01.001599 reading_impact_model-1.0.1/reading_impact_model/matchers/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     5284 2023-03-22 13:46:51.249891 reading_impact_model-1.0.1/reading_impact_model/matchers/__pycache__/alpino_matcher.cpython-310.pyc
--rw-r--r--   0        0        0    14361 2023-03-25 09:36:41.648917 reading_impact_model-1.0.1/reading_impact_model/matchers/__pycache__/matcher.cpython-310.pyc
--rw-r--r--   0        0        0     1866 2023-03-24 12:38:36.508590 reading_impact_model-1.0.1/reading_impact_model/matchers/__pycache__/spacy_matcher.cpython-310.pyc
--rw-r--r--   0        0        0     4736 2023-03-22 13:16:07.552479 reading_impact_model-1.0.1/reading_impact_model/matchers/alpino_matcher.py
--rw-r--r--   0        0        0    11246 2023-03-21 06:24:13.469150 reading_impact_model-1.0.1/reading_impact_model/matchers/alpinor_matcher_old.py
--rw-r--r--   0        0        0    21568 2023-06-07 13:48:46.145196 reading_impact_model-1.0.1/reading_impact_model/matchers/matcher.py
--rw-r--r--   0        0        0      775 2023-03-21 06:27:57.741456 reading_impact_model-1.0.1/reading_impact_model/matchers/nltk_matcher.py
--rw-r--r--   0        0        0     1532 2023-06-07 13:49:21.112807 reading_impact_model-1.0.1/reading_impact_model/matchers/spacy_matcher.py
--rw-r--r--   0        0        0     1240 2023-03-22 13:17:03.674991 reading_impact_model-1.0.1/reading_impact_model/matchers/stanza_matcher.py
--rw-r--r--   0        0        0     1186 2023-03-22 13:17:03.671968 reading_impact_model-1.0.1/reading_impact_model/matchers/trankit_matcher.py
--rw-r--r--   0        0        0        0 2023-03-20 14:46:41.117875 reading_impact_model-1.0.1/reading_impact_model/model/__init__.py
--rw-r--r--   0        0        0     5589 2023-03-20 14:34:36.075954 reading_impact_model-1.0.1/reading_impact_model/model/phrase.py
--rw-r--r--   0        0        0        0 2023-03-20 14:46:41.124577 reading_impact_model-1.0.1/reading_impact_model/models/__init__.py
--rw-r--r--   0        0        0      201 2023-03-20 14:55:07.896122 reading_impact_model-1.0.1/reading_impact_model/models/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0   619876 2023-03-20 14:55:07.939597 reading_impact_model-1.0.1/reading_impact_model/models/__pycache__/impact_model_en.cpython-310.pyc
--rw-r--r--   0        0        0   160274 2023-03-20 14:55:07.905894 reading_impact_model-1.0.1/reading_impact_model/models/__pycache__/impact_model_nl.cpython-310.pyc
--rw-r--r--   0        0        0   356666 2020-06-19 22:04:56.168319 reading_impact_model-1.0.1/reading_impact_model/models/impact_model-en-0.1.pcl
--rw-r--r--   0        0        0   209835 2021-04-20 14:51:48.208246 reading_impact_model-1.0.1/reading_impact_model/models/impact_model-en-0.2.pcl
--rw-r--r--   0        0        0   230737 2021-07-02 13:07:05.214976 reading_impact_model-1.0.1/reading_impact_model/models/impact_model-en-0.3.pcl
--rw-r--r--   0        0        0   230678 2021-07-05 10:41:51.476919 reading_impact_model-1.0.1/reading_impact_model/models/impact_model-en-0.4.pcl
--rw-r--r--   0        0        0   230690 2021-07-06 11:33:29.799021 reading_impact_model-1.0.1/reading_impact_model/models/impact_model-en-0.5.pcl
--rw-r--r--   0        0        0   692078 2021-10-25 11:59:27.603446 reading_impact_model-1.0.1/reading_impact_model/models/impact_model-en-0.6.json
--rw-r--r--   0        0        0   579958 2021-10-25 11:59:27.554350 reading_impact_model-1.0.1/reading_impact_model/models/impact_model-en-0.6.pcl
--rw-r--r--   0        0        0   691857 2023-03-21 09:49:00.251013 reading_impact_model-1.0.1/reading_impact_model/models/impact_model-en-0.7.json
--rw-r--r--   0        0        0   621720 2023-03-21 09:49:00.228629 reading_impact_model-1.0.1/reading_impact_model/models/impact_model-en-0.7.pcl
--rw-r--r--   0        0        0   691857 2023-03-21 09:49:00.264532 reading_impact_model-1.0.1/reading_impact_model/models/impact_model-en.json
--rw-r--r--   0        0        0   621720 2023-03-21 09:49:00.234743 reading_impact_model-1.0.1/reading_impact_model/models/impact_model-en.pcl
--rw-r--r--   0        0        0   244747 2021-10-25 11:40:57.657433 reading_impact_model-1.0.1/reading_impact_model/models/impact_model-nl-1.0.json
--rw-r--r--   0        0        0   244747 2021-10-25 11:40:57.645116 reading_impact_model-1.0.1/reading_impact_model/models/impact_model-nl.json
--rw-r--r--   0        0        0   176064 2020-05-19 14:38:46.549523 reading_impact_model-1.0.1/reading_impact_model/models/impact_model-nl.pcl
--rw-r--r--   0        0        0   692090 2021-10-25 11:59:46.390314 reading_impact_model-1.0.1/reading_impact_model/models/impact_model_en.py
--rw-r--r--   0        0        0   244764 2023-03-20 14:34:33.867788 reading_impact_model-1.0.1/reading_impact_model/models/impact_model_nl.py
--rw-r--r--   0        0        0      903 2023-03-21 06:24:13.480622 reading_impact_model-1.0.1/reading_impact_model/reading_impact.py
--rw-r--r--   0        0        0     7806 1970-01-01 00:00:00.000000 reading_impact_model-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     6941 2023-03-25 09:51:54.164506 reading_impact_model-1.0.2/README.md
+-rw-r--r--   0        0        0     1185 2023-06-07 14:13:11.195598 reading_impact_model-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-06-07 14:13:11.195810 reading_impact_model-1.0.2/reading_impact_model/__init__.py
+-rw-r--r--   0        0        0    21445 2023-03-25 09:23:34.833907 reading_impact_model-1.0.2/reading_impact_model/impact_model.py
+-rw-r--r--   0        0        0        0 2023-03-21 06:20:35.500337 reading_impact_model-1.0.2/reading_impact_model/matchers/__init__.py
+-rw-r--r--   0        0        0      203 2023-03-21 06:50:01.001599 reading_impact_model-1.0.2/reading_impact_model/matchers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     5284 2023-03-22 13:46:51.249891 reading_impact_model-1.0.2/reading_impact_model/matchers/__pycache__/alpino_matcher.cpython-310.pyc
+-rw-r--r--   0        0        0    14677 2023-06-07 14:11:05.000971 reading_impact_model-1.0.2/reading_impact_model/matchers/__pycache__/matcher.cpython-310.pyc
+-rw-r--r--   0        0        0     1892 2023-06-07 14:03:03.744638 reading_impact_model-1.0.2/reading_impact_model/matchers/__pycache__/spacy_matcher.cpython-310.pyc
+-rw-r--r--   0        0        0     4736 2023-03-22 13:16:07.552479 reading_impact_model-1.0.2/reading_impact_model/matchers/alpino_matcher.py
+-rw-r--r--   0        0        0    11246 2023-03-21 06:24:13.469150 reading_impact_model-1.0.2/reading_impact_model/matchers/alpinor_matcher_old.py
+-rw-r--r--   0        0        0    22038 2023-06-07 14:11:00.909291 reading_impact_model-1.0.2/reading_impact_model/matchers/matcher.py
+-rw-r--r--   0        0        0      775 2023-03-21 06:27:57.741456 reading_impact_model-1.0.2/reading_impact_model/matchers/nltk_matcher.py
+-rw-r--r--   0        0        0     1532 2023-06-07 13:49:21.112807 reading_impact_model-1.0.2/reading_impact_model/matchers/spacy_matcher.py
+-rw-r--r--   0        0        0     1240 2023-03-22 13:17:03.674991 reading_impact_model-1.0.2/reading_impact_model/matchers/stanza_matcher.py
+-rw-r--r--   0        0        0     1186 2023-03-22 13:17:03.671968 reading_impact_model-1.0.2/reading_impact_model/matchers/trankit_matcher.py
+-rw-r--r--   0        0        0        0 2023-03-20 14:46:41.117875 reading_impact_model-1.0.2/reading_impact_model/model/__init__.py
+-rw-r--r--   0        0        0     5589 2023-03-20 14:34:36.075954 reading_impact_model-1.0.2/reading_impact_model/model/phrase.py
+-rw-r--r--   0        0        0        0 2023-03-20 14:46:41.124577 reading_impact_model-1.0.2/reading_impact_model/models/__init__.py
+-rw-r--r--   0        0        0      201 2023-03-20 14:55:07.896122 reading_impact_model-1.0.2/reading_impact_model/models/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0   619876 2023-03-20 14:55:07.939597 reading_impact_model-1.0.2/reading_impact_model/models/__pycache__/impact_model_en.cpython-310.pyc
+-rw-r--r--   0        0        0   160274 2023-03-20 14:55:07.905894 reading_impact_model-1.0.2/reading_impact_model/models/__pycache__/impact_model_nl.cpython-310.pyc
+-rw-r--r--   0        0        0   356666 2020-06-19 22:04:56.168319 reading_impact_model-1.0.2/reading_impact_model/models/impact_model-en-0.1.pcl
+-rw-r--r--   0        0        0   209835 2021-04-20 14:51:48.208246 reading_impact_model-1.0.2/reading_impact_model/models/impact_model-en-0.2.pcl
+-rw-r--r--   0        0        0   230737 2021-07-02 13:07:05.214976 reading_impact_model-1.0.2/reading_impact_model/models/impact_model-en-0.3.pcl
+-rw-r--r--   0        0        0   230678 2021-07-05 10:41:51.476919 reading_impact_model-1.0.2/reading_impact_model/models/impact_model-en-0.4.pcl
+-rw-r--r--   0        0        0   230690 2021-07-06 11:33:29.799021 reading_impact_model-1.0.2/reading_impact_model/models/impact_model-en-0.5.pcl
+-rw-r--r--   0        0        0   692078 2021-10-25 11:59:27.603446 reading_impact_model-1.0.2/reading_impact_model/models/impact_model-en-0.6.json
+-rw-r--r--   0        0        0   579958 2021-10-25 11:59:27.554350 reading_impact_model-1.0.2/reading_impact_model/models/impact_model-en-0.6.pcl
+-rw-r--r--   0        0        0   691857 2023-03-21 09:49:00.251013 reading_impact_model-1.0.2/reading_impact_model/models/impact_model-en-0.7.json
+-rw-r--r--   0        0        0   621720 2023-03-21 09:49:00.228629 reading_impact_model-1.0.2/reading_impact_model/models/impact_model-en-0.7.pcl
+-rw-r--r--   0        0        0   691857 2023-03-21 09:49:00.264532 reading_impact_model-1.0.2/reading_impact_model/models/impact_model-en.json
+-rw-r--r--   0        0        0   621720 2023-03-21 09:49:00.234743 reading_impact_model-1.0.2/reading_impact_model/models/impact_model-en.pcl
+-rw-r--r--   0        0        0   244747 2021-10-25 11:40:57.657433 reading_impact_model-1.0.2/reading_impact_model/models/impact_model-nl-1.0.json
+-rw-r--r--   0        0        0   244747 2021-10-25 11:40:57.645116 reading_impact_model-1.0.2/reading_impact_model/models/impact_model-nl.json
+-rw-r--r--   0        0        0   176064 2020-05-19 14:38:46.549523 reading_impact_model-1.0.2/reading_impact_model/models/impact_model-nl.pcl
+-rw-r--r--   0        0        0   692090 2021-10-25 11:59:46.390314 reading_impact_model-1.0.2/reading_impact_model/models/impact_model_en.py
+-rw-r--r--   0        0        0   244764 2023-03-20 14:34:33.867788 reading_impact_model-1.0.2/reading_impact_model/models/impact_model_nl.py
+-rw-r--r--   0        0        0      903 2023-03-21 06:24:13.480622 reading_impact_model-1.0.2/reading_impact_model/reading_impact.py
+-rw-r--r--   0        0        0     7806 1970-01-01 00:00:00.000000 reading_impact_model-1.0.2/PKG-INFO
```

### Comparing `reading_impact_model-1.0.1/README.md` & `reading_impact_model-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.1/pyproject.toml` & `reading_impact_model-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reading-impact-model"
-version = "1.0.1"
+version = "1.0.2"
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
-current_version = "1.0.1"
+current_version = "1.0.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `reading_impact_model-1.0.1/reading_impact_model/impact_model.py` & `reading_impact_model-1.0.2/reading_impact_model/impact_model.py`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.1/reading_impact_model/matchers/__pycache__/alpino_matcher.cpython-310.pyc` & `reading_impact_model-1.0.2/reading_impact_model/matchers/__pycache__/alpino_matcher.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.1/reading_impact_model/matchers/__pycache__/matcher.cpython-310.pyc` & `reading_impact_model-1.0.2/reading_impact_model/matchers/__pycache__/matcher.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Mar 25 09:36:36 2023 UTC, .py size: 21410 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a4c0 1e64 a253 0000  o..........d.S..
+00000000: 6f0d 0d0a 0000 0000 f48f 8064 1656 0000  o..........d.V..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 b200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 6d05 5a05  ..d.d.l.m.Z.m.Z.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c09 6d0a 5a0a 6d0b 5a0b  ..d.d.l.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 0100 6400  m.Z.m.Z.m.Z...d.
@@ -27,27 +27,27 @@
 000001a0: 645f 6d6f 6465 6c29 02da 1069 735f 7769  d_model)...is_wi
 000001b0: 6c64 6361 7264 5f74 6572 6dda 1377 696c  ldcard_term..wil
 000001c0: 6463 6172 645f 7465 726d 5f6d 6174 6368  dcard_term_match
 000001d0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
 000001e0: 0002 0000 0043 0000 0073 1c00 0000 7c00  .....C...s....|.
 000001f0: 6401 1900 6402 6b02 7208 6403 5300 7c00  d...d.k.r.d.S.|.
 00000200: 6401 1900 a000 a100 5300 2904 4eda 0b69  d.......S.).N..i
-00000210: 6d70 6163 745f 7479 7065 5a06 4166 6665  mpact_typeZ.Affe
+00000210: 6d70 6163 745f 7479 7065 da06 4166 6665  mpact_type..Affe
 00000220: 6374 da08 706f 7369 7469 7665 2901 da05  ct..positive)...
 00000230: 6c6f 7765 7229 01da 056d 6174 6368 a900  lower)...match..
-00000240: 7216 0000 00fa 6d2f 5573 6572 732f 6d61  r.....m/Users/ma
+00000240: 7217 0000 00fa 6d2f 5573 6572 732f 6d61  r.....m/Users/ma
 00000250: 7269 6a6e 6b6f 6f6c 656e 2f44 6174 612f  rijnkoolen/Data/
 00000260: 5072 6f6a 6563 7473 2f54 2d52 6563 732f  Projects/T-Recs/
 00000270: 4170 7065 616c 2f72 6561 6469 6e67 2d69  Appeal/reading-i
 00000280: 6d70 6163 742d 6d6f 6465 6c2f 7265 6164  mpact-model/read
 00000290: 696e 675f 696d 7061 6374 5f6d 6f64 656c  ing_impact_model
 000002a0: 2f6d 6174 6368 6572 732f 6d61 7463 6865  /matchers/matche
 000002b0: 722e 7079 da11 6d61 705f 7265 7669 6577  r.py..map_review
 000002c0: 5f69 6d70 6163 740d 0000 0073 0600 0000  _impact....s....
-000002d0: 0c01 0401 0c02 7218 0000 0063 0200 0000  ......r....c....
+000002d0: 0c01 0401 0c02 7219 0000 0063 0200 0000  ......r....c....
 000002e0: 0000 0000 0000 0000 0200 0000 0800 0000  ................
 000002f0: 4300 0000 f340 0000 0074 007c 0183 0172  C....@...t.|...r
 00000300: 187a 0674 017c 007c 0183 0257 0053 0004  .z.t.|.|...W.S..
 00000310: 0074 0279 1701 0001 0001 0074 0364 017c  .t.y.......t.d.|
 00000320: 0183 0201 0082 0077 007c 007c 016b 0272  .......w.|.|.k.r
 00000330: 1e64 0253 0064 0353 0029 047a 6e74 6869  .d.S.d.S.).znthi
 00000340: 7320 6675 6e63 7469 6f6e 206d 6174 6368  s function match
@@ -56,843 +56,863 @@
 00000370: 6365 2074 6572 6d2c 0a20 2020 2075 7365  ce term,.    use
 00000380: 7320 7769 6c64 6361 7264 7320 6966 2067  s wildcards if g
 00000390: 6976 656e 2c20 6f74 6865 7277 6973 6520  iven, otherwise 
 000003a0: 6578 6163 7420 6d61 7463 687a 1349 6e76  exact matchz.Inv
 000003b0: 616c 6964 206d 6f64 656c 5f74 6572 6d3a  alid model_term:
 000003c0: 5446 a904 7210 0000 0072 1100 0000 da0a  TF..r....r......
 000003d0: 496e 6465 7845 7272 6f72 da05 7072 696e  IndexError..prin
-000003e0: 7429 025a 0d73 656e 7465 6e63 655f 7465  t).Z.sentence_te
-000003f0: 726d 5a0a 6d6f 6465 6c5f 7465 726d 7216  rmZ.model_termr.
-00000400: 0000 0072 1600 0000 7217 0000 00da 0a74  ...r....r......t
+000003e0: 7429 02da 0d73 656e 7465 6e63 655f 7465  t)...sentence_te
+000003f0: 726d 5a0a 6d6f 6465 6c5f 7465 726d 7217  rmZ.model_termr.
+00000400: 0000 0072 1700 0000 7218 0000 00da 0a74  ...r....r......t
 00000410: 6572 6d5f 6d61 7463 6814 0000 00f3 1400  erm_match.......
 00000420: 0000 0803 0201 0c01 0c01 0a01 0201 02fe  ................
-00000430: 0803 0401 0402 721d 0000 0063 0200 0000  ......r....c....
+00000430: 0803 0401 0402 721f 0000 0063 0200 0000  ......r....c....
 00000440: 0000 0000 0000 0000 0200 0000 0800 0000  ................
-00000450: 4300 0000 7219 0000 0029 047a 7674 6869  C...r....).zvthi
+00000450: 4300 0000 721a 0000 0029 047a 7674 6869  C...r....).zvthi
 00000460: 7320 6675 6e63 7469 6f6e 206d 6174 6368  s function match
 00000470: 6573 2061 206d 6f64 656c 2074 6572 6d20  es a model term 
 00000480: 6167 6169 6e73 7420 6120 6c65 6d6d 6120  against a lemma 
 00000490: 6672 6f6d 2061 2073 656e 7465 6e63 652c  from a sentence,
 000004a0: 0a20 2020 2075 7365 7320 7769 6c64 6361  .    uses wildca
 000004b0: 7264 7320 6966 2067 6976 656e 2c20 6f74  rds if given, ot
 000004c0: 6865 7277 6973 6520 6578 6163 7420 6d61  herwise exact ma
 000004d0: 7463 687a 1349 6e76 616c 6964 206d 6174  tchz.Invalid mat
-000004e0: 6368 5f74 6572 6d3a 5446 721a 0000 0029  ch_term:TFr....)
-000004f0: 02da 056c 656d 6d61 da04 7465 726d 7216  ...lemma..termr.
-00000500: 0000 0072 1600 0000 7217 0000 00da 106c  ...r....r......l
+000004e0: 6368 5f74 6572 6d3a 5446 721b 0000 0029  ch_term:TFr....)
+000004f0: 02da 056c 656d 6d61 da04 7465 726d 7217  ...lemma..termr.
+00000500: 0000 0072 1700 0000 7218 0000 00da 106c  ...r....r......l
 00000510: 656d 6d61 5f74 6572 6d5f 6d61 7463 6823  emma_term_match#
-00000520: 0000 0072 1e00 0000 7221 0000 0063 0100  ...r....r!...c..
+00000520: 0000 0072 2000 0000 7223 0000 0063 0100  ...r ...r#...c..
 00000530: 0000 0000 0000 0000 0000 0100 0000 0500  ................
 00000540: 0000 4300 0000 730e 0000 0074 00a0 0164  ..C...s....t...d
 00000550: 0164 027c 00a1 0353 0029 037a 5472 656d  .d.|...S.).zTrem
 00000560: 6f76 6573 206c 6561 6469 6e67 2061 6e64  oves leading and
 00000570: 2074 7261 696c 696e 6720 7075 6e63 7475   trailing punctu
 00000580: 6174 696f 6e20 6672 6f6d 2061 2073 7472  ation from a str
 00000590: 696e 672e 204e 6565 6465 6420 666f 7220  ing. Needed for 
 000005a0: 416c 7069 6e6f 2077 6f72 6420 6e6f 6465  Alpino word node
 000005b0: 737a 105e 5c57 2a5c 6228 2e2a 295c 625c  sz.^\W*\b(.*)\b\
 000005c0: 572a 247a 025c 3129 02da 0272 65da 0373  W*$z.\1)...re..s
-000005d0: 7562 2901 da06 7374 7269 6e67 7216 0000  ub)...stringr...
-000005e0: 0072 1600 0000 7217 0000 00da 1b72 656d  .r....r......rem
+000005d0: 7562 2901 da06 7374 7269 6e67 7217 0000  ub)...stringr...
+000005e0: 0072 1700 0000 7218 0000 00da 1b72 656d  .r....r......rem
 000005f0: 6f76 655f 7472 6169 6c69 6e67 5f70 756e  ove_trailing_pun
 00000600: 6374 7561 7469 6f6e 3200 0000 7302 0000  ctuation2...s...
-00000610: 000e 0272 2500 0000 6300 0000 0000 0000  ...r%...c.......
+00000610: 000e 0272 2700 0000 6300 0000 0000 0000  ...r'...c.......
 00000620: 0000 0000 0000 0000 000c 0000 0040 0000  .............@..
-00000630: 0073 e801 0000 6500 5a01 6400 5a02 6449  .s....e.Z.d.Z.dI
+00000630: 0073 f601 0000 6500 5a01 6400 5a02 6449  .s....e.Z.d.Z.dI
 00000640: 6404 6503 6405 6504 6406 6505 6606 6407  d.e.d.e.d.e.f.d.
 00000650: 6408 8405 5a06 6409 6503 640a 6507 640b  d...Z.d.e.d.e.d.
 00000660: 6503 6606 640c 640d 8404 5a08 640e 640f  e.f.d.d...Z.d.d.
 00000670: 8400 5a09 6410 6411 8400 5a0a 6412 650b  ..Z.d.d...Z.d.e.
-00000680: 6602 6413 6414 8404 5a0c 6415 650d 6416  f.d.d...Z.d.e.d.
-00000690: 650e 6503 650f 6602 1900 6417 6503 6418  e.e.e.f...d.e.d.
-000006a0: 6402 6608 6419 641a 8404 5a10 6415 650d  d.f.d.d...Z.d.e.
-000006b0: 6416 6503 6417 6503 6418 6402 6608 641b  d.e.d.e.d.d.f.d.
-000006c0: 641c 8404 5a11 641d 641e 8400 5a12 6415  d...Z.d.d...Z.d.
-000006d0: 650d 6416 6503 6417 6503 6418 6402 6608  e.d.e.d.e.d.d.f.
-000006e0: 641f 6420 8404 5a13 644a 6421 6503 6417  d.d ..Z.dJd!e.d.
-000006f0: 6503 6604 6422 6423 8405 5a14 0902 0903  e.f.d"d#..Z.....
-00000700: 644b 6421 6503 6417 6503 6424 6505 6418  dKd!e.d.e.d$e.d.
-00000710: 6515 650e 6503 650f 6602 1900 1900 6608  e.e.e.e.f.....f.
-00000720: 6425 6426 8405 5a16 644c 6428 6429 8401  d%d&..Z.dLd(d)..
-00000730: 5a17 644c 642a 642b 8401 5a18 644c 642c  Z.dLd*d+..Z.dLd,
-00000740: 642d 8401 5a19 644d 642f 6430 8401 5a1a  d-..Z.dMd/d0..Z.
-00000750: 6431 6432 8400 5a1b 6433 6434 8400 5a1c  d1d2..Z.d3d4..Z.
-00000760: 644a 6435 6507 6418 6515 651d 1900 6604  dJd5e.d.e.e...f.
-00000770: 6436 6437 8405 5a1e 6418 6515 651d 1900  d6d7..Z.d.e.e...
-00000780: 6602 6438 6439 8404 5a1f 6435 6507 6602  f.d8d9..Z.d5e.f.
-00000790: 643a 643b 8404 5a20 6435 6507 643c 651d  d:d;..Z d5e.d<e.
-000007a0: 6604 643d 643e 8404 5a21 6435 6507 643c  f.d=d>..Z!d5e.d<
-000007b0: 651d 6418 6505 6606 643f 6440 8404 5a22  e.d.e.f.d?d@..Z"
-000007c0: 6435 6507 643c 651d 6418 6505 6606 6441  d5e.d<e.d.e.f.dA
-000007d0: 6442 8404 5a23 6443 651d 6418 650e 6503  dB..Z#dCe.d.e.e.
-000007e0: 650d 6602 1900 6604 6444 6445 8404 5a24  e.f...f.dDdE..Z$
-000007f0: 0903 644e 6446 6515 651d 1900 6424 6505  ..dNdFe.e...d$e.
-00000800: 6418 6515 650e 6503 650f 6602 1900 1900  d.e.e.e.e.f.....
-00000810: 6606 6447 6448 8405 5a25 6402 5300 294f  f.dGdH..Z%d.S.)O
-00000820: da0d 496d 7061 6374 4d61 7463 6865 72da  ..ImpactMatcher.
-00000830: 0265 6e4e 46da 046c 616e 67da 0c69 6d70  .enNF..lang..imp
-00000840: 6163 745f 6d6f 6465 6cda 0564 6562 7567  act_model..debug
-00000850: 6304 0000 0000 0000 0000 0000 0004 0000  c...............
-00000860: 0003 0000 0043 0000 0073 8e00 0000 7c01  .....C...s....|.
-00000870: 7c00 5f00 7c01 6401 7501 720e 7401 7c01  |._.|.d.u.r.t.|.
-00000880: 6402 8d01 7c00 5f02 6e0d 7403 7c02 7404  d...|._.n.t.|.t.
-00000890: 8302 7217 7c02 7c00 5f02 6e04 7405 6403  ..r.|.|._.n.t.d.
-000008a0: 8301 8201 7c03 7c00 5f06 6404 7c00 5f07  ....|.|._.d.|._.
-000008b0: 6700 7c00 5f08 6401 7c00 5f09 6401 7c00  g.|._.d.|._.d.|.
-000008c0: 5f0a 740b 740c 8301 7c00 5f0d 740c 8300  _.t.t...|._.t...
-000008d0: 7c00 5f0e 740c 8300 7c00 5f0f 740b 7410  |._.t...|._.t.t.
-000008e0: 8301 7c00 5f11 740b 7412 8301 7c00 5f13  ..|._.t.t...|._.
-000008f0: 7c00 a014 a100 0100 6401 5300 2905 61ee  |.......d.S.).a.
-00000900: 0100 0043 7265 6174 6520 6120 7265 6164  ...Create a read
-00000910: 696e 6720 696d 7061 6374 206d 6174 6368  ing impact match
-00000920: 6572 206f 626a 6563 7420 666f 7220 6120  er object for a 
-00000930: 6769 7665 6e20 7265 6164 696e 6720 696d  given reading im
-00000940: 7061 6374 206d 6f64 656c 206f 7220 6c61  pact model or la
-00000950: 6e67 7561 6765 2e0a 0a20 2020 2020 2020  nguage...       
-00000960: 2049 6620 6f6e 6c79 2061 206c 616e 6775   If only a langu
-00000970: 6167 6520 6964 656e 7469 6669 6572 2028  age identifier (
-00000980: 2765 6e27 206f 7220 276e 6c27 2920 6973  'en' or 'nl') is
-00000990: 2070 6173 7365 642c 2074 6865 2064 6566   passed, the def
-000009a0: 6175 6c74 206d 6f64 656c 2066 6f72 2074  ault model for t
-000009b0: 6861 740a 2020 2020 2020 2020 6c61 6e67  hat.        lang
-000009c0: 7561 6765 2077 696c 6c20 6265 2075 7365  uage will be use
-000009d0: 642e 0a0a 2020 2020 2020 2020 3a70 6172  d...        :par
-000009e0: 616d 206c 616e 673a 2074 6865 206c 616e  am lang: the lan
-000009f0: 6775 6167 6520 666f 7220 7768 6963 6820  guage for which 
-00000a00: 6120 7265 6164 696e 6720 696d 7061 6374  a reading impact
-00000a10: 206d 6f64 656c 2073 686f 756c 6420 6265   model should be
-00000a20: 2075 7365 6420 2864 6566 6175 6c74 2027   used (default '
-00000a30: 656e 272c 2077 6869 6368 2069 7320 456e  en', which is En
-00000a40: 676c 6973 6829 2e0a 2020 2020 2020 2020  glish)..        
-00000a50: 3a74 7970 6520 6c61 6e67 3a20 7374 720a  :type lang: str.
-00000a60: 2020 2020 2020 2020 3a70 6172 616d 2069          :param i
-00000a70: 6d70 6163 745f 6d6f 6465 6c3a 2061 2073  mpact_model: a s
-00000a80: 7065 6369 6669 6320 696d 7061 6374 206d  pecific impact m
-00000a90: 6f64 656c 2c20 6966 2079 6f75 2077 616e  odel, if you wan
-00000aa0: 7420 746f 206f 7665 7272 6964 6520 7468  t to override th
-00000ab0: 6520 6465 6661 756c 7420 6d6f 6465 6c2e  e default model.
-00000ac0: 0a20 2020 2020 2020 203a 7479 7065 2069  .        :type i
-00000ad0: 6d70 6163 745f 6d6f 6465 6c3a 2049 6d70  mpact_model: Imp
-00000ae0: 6163 744d 6f64 656c 0a20 2020 2020 2020  actModel.       
-00000af0: 204e 2901 7228 0000 007a 374d 6174 6368   N).r(...z7Match
-00000b00: 6572 206d 7573 7420 6265 2069 6e73 7461  er must be insta
-00000b10: 6e74 6961 7465 6420 7769 7468 2061 6e20  ntiated with an 
-00000b20: 496d 7061 6374 4d6f 6465 6c20 6f62 6a65  ImpactModel obje
-00000b30: 6374 da00 2915 7228 0000 0072 0f00 0000  ct..).r(...r....
-00000b40: 7229 0000 00da 0a69 7369 6e73 7461 6e63  r).....isinstanc
-00000b50: 6572 0700 0000 da09 5479 7065 4572 726f  er......TypeErro
-00000b60: 7272 2a00 0000 da0f 7365 6e74 656e 6365  rr*.....sentence
-00000b70: 5f73 7472 696e 67da 0f73 656e 7465 6e63  _string..sentenc
-00000b80: 655f 746f 6b65 6e73 da06 646f 635f 6964  e_tokens..doc_id
-00000b90: da0e 7365 6e74 656e 6365 5f69 6e64 6578  ..sentence_index
-00000ba0: 7202 0000 00da 0373 6574 da14 7365 6e74  r......set..sent
-00000bb0: 656e 6365 5f76 6f63 6162 5f74 6572 6d73  ence_vocab_terms
-00000bc0: 5a15 7365 6e74 656e 6365 5f69 6d70 6163  Z.sentence_impac
-00000bd0: 745f 7465 726d 735a 1573 656e 7465 6e63  t_termsZ.sentenc
-00000be0: 655f 6173 7065 6374 5f74 6572 6d73 da03  e_aspect_terms..
-00000bf0: 696e 74da 0f63 616e 6469 6461 7465 5f72  int..candidate_r
-00000c00: 756c 6573 da04 6c69 7374 da16 696d 7061  ules..list..impa
-00000c10: 6374 5f72 756c 655f 7465 726d 5f69 6e64  ct_rule_term_ind
-00000c20: 6578 da18 5f69 6e64 6578 5f69 6d70 6163  ex.._index_impac
-00000c30: 745f 7275 6c65 5f77 6f72 6473 2904 da04  t_rule_words)...
-00000c40: 7365 6c66 7228 0000 0072 2900 0000 722a  selfr(...r)...r*
-00000c50: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
-00000c60: 0000 da08 5f5f 696e 6974 5f5f 3900 0000  ....__init__9...
-00000c70: 7322 0000 0006 0b08 010e 010a 0108 0108  s"..............
-00000c80: 0206 0106 0106 0106 0106 010a 0108 0108  ................
-00000c90: 010a 010a 010c 017a 1649 6d70 6163 744d  .......z.ImpactM
-00000ca0: 6174 6368 6572 2e5f 5f69 6e69 745f 5f72  atcher.__init__r
-00000cb0: 2400 0000 da04 7275 6c65 da09 7465 726d  $.....rule..term
-00000cc0: 5f74 7970 6563 0400 0000 0000 0000 0000  _typec..........
-00000cd0: 0000 0700 0000 0800 0000 4300 0000 73d6  ..........C...s.
-00000ce0: 0000 007c 0364 016b 0272 107c 006a 007c  ...|.d.k.r.|.j.|
-00000cf0: 0105 0019 007c 0267 0137 0003 003c 0064  .....|.g.7...<.d
-00000d00: 0053 007c 0364 026b 0273 187c 0364 036b  .S.|.d.k.s.|.d.k
-00000d10: 0272 697a 3d7c 01a0 01a1 00a0 0264 04a1  .riz=|.......d..
-00000d20: 0144 005d 327d 047c 0464 0519 0064 066b  .D.]2}.|.d...d.k
-00000d30: 0272 487c 0464 0719 0064 086b 0272 4874  .rH|.d...d.k.rHt
-00000d40: 03a0 0264 097c 0464 0a64 0785 0219 00a1  ...d.|.d.d......
-00000d50: 027d 057c 0544 005d 0c7d 067c 006a 007c  .}.|.D.].}.|.j.|
-00000d60: 0605 0019 007c 0267 0137 0003 003c 0071  .....|.g.7...<.q
-00000d70: 3a71 207c 006a 007c 0405 0019 007c 0267  :q |.j.|.....|.g
-00000d80: 0137 0003 003c 0071 2057 0064 0053 0004  .7...<.q W.d.S..
-00000d90: 0074 0479 6801 0001 0001 0074 057c 0183  .t.yh......t.|..
-00000da0: 0101 0074 057c 01a0 0264 04a1 0183 0101  ...t.|...d......
-00000db0: 0082 0077 0064 0053 0029 0b4e 7220 0000  ...w.d.S.).Nr ..
-00000dc0: 00da 0670 6872 6173 65da 0572 6567 6578  ...phrase..regex
-00000dd0: fa01 2072 0100 0000 fa01 28e9 ffff ffff  .. r......(.....
-00000de0: fa01 297a 045b 207c 5de9 0100 0000 2906  ..)z.[ |].....).
-00000df0: 7237 0000 00da 0573 7472 6970 da05 7370  r7.....strip..sp
-00000e00: 6c69 7472 2200 0000 721b 0000 0072 1c00  litr"...r....r..
-00000e10: 0000 2907 7239 0000 0072 2400 0000 723b  ..).r9...r$...r;
-00000e20: 0000 0072 3c00 0000 5a0b 7068 7261 7365  ...r<...Z.phrase
-00000e30: 5f70 6172 745a 1170 6872 6173 655f 7061  _partZ.phrase_pa
-00000e40: 7274 5f74 6572 6d73 7220 0000 0072 1600  rt_termsr ...r..
-00000e50: 0000 7216 0000 0072 1700 0000 da19 5f69  ..r....r......_i
-00000e60: 6e64 6578 5f69 6d70 6163 745f 7275 6c65  ndex_impact_rule
-00000e70: 5f73 7472 696e 6757 0000 0073 2400 0000  _stringW...s$...
-00000e80: 0801 1801 1001 0201 1201 1801 1401 0802  ................
-00000e90: 1601 02ff 1603 06f9 0c08 0801 0e01 0201  ................
-00000ea0: 02fd 04f6 7a27 496d 7061 6374 4d61 7463  ....z'ImpactMatc
-00000eb0: 6865 722e 5f69 6e64 6578 5f69 6d70 6163  her._index_impac
-00000ec0: 745f 7275 6c65 5f73 7472 696e 6763 0100  t_rule_stringc..
-00000ed0: 0000 0000 0000 0000 0000 0200 0000 0600  ................
-00000ee0: 0000 4300 0000 7328 0000 007c 006a 006a  ..C...s(...|.j.j
-00000ef0: 0144 005d 0d7d 017c 00a0 027c 016a 036a  .D.].}.|...|.j.j
-00000f00: 047c 017c 016a 036a 05a1 0301 0071 0464  .|.|.j.j.....q.d
-00000f10: 0053 00a9 014e 2906 7229 0000 005a 0c69  .S...N).r)...Z.i
-00000f20: 6d70 6163 745f 7275 6c65 7372 4600 0000  mpact_rulesrF...
-00000f30: da0b 696d 7061 6374 5f74 6572 6d72 2400  ..impact_termr$.
-00000f40: 0000 da04 7479 7065 2902 7239 0000 0072  ....type).r9...r
-00000f50: 3b00 0000 7216 0000 0072 1600 0000 7217  ;...r....r....r.
-00000f60: 0000 0072 3800 0000 6900 0000 7306 0000  ...r8...i...s...
-00000f70: 000c 0118 0104 ff7a 2649 6d70 6163 744d  .......z&ImpactM
-00000f80: 6174 6368 6572 2e5f 696e 6465 785f 696d  atcher._index_im
-00000f90: 7061 6374 5f72 756c 655f 776f 7264 7363  pact_rule_wordsc
-00000fa0: 0300 0000 0000 0000 0000 0000 0400 0000  ................
-00000fb0: 0500 0000 4300 0000 736c 0000 007c 017c  ....C...sl...|.|
-00000fc0: 006a 0076 0072 167c 006a 007c 0119 0044  .j.v.r.|.j.|...D
-00000fd0: 005d 0b7d 037c 006a 017c 0305 0019 0064  .].}.|.j.|.....d
-00000fe0: 0137 0003 003c 0071 0a7c 027c 016b 0372  .7...<.q.|.|.k.r
-00000ff0: 307c 027c 006a 0076 0072 327c 006a 007c  0|.|.j.v.r2|.j.|
-00001000: 0219 0044 005d 0f7d 037c 006a 017c 0305  ...D.].}.|.j.|..
-00001010: 0019 0064 0137 0003 003c 0071 2464 0053  ...d.7...<.q$d.S
-00001020: 0064 0053 0064 0053 0029 024e 7243 0000  .d.S.d.S.).NrC..
-00001030: 0029 0272 3700 0000 7235 0000 0029 0472  .).r7...r5...).r
-00001040: 3900 0000 da05 746f 6b65 6e72 1f00 0000  9.....tokenr....
-00001050: 723b 0000 0072 1600 0000 7216 0000 0072  r;...r....r....r
-00001060: 1700 0000 da13 6164 645f 6361 6e64 6964  ......add_candid
-00001070: 6174 655f 7275 6c65 7370 0000 0073 1000  ate_rulesp...s..
-00001080: 0000 0a02 0e02 1402 1201 0e01 1401 08fe  ................
-00001090: 0401 7a21 496d 7061 6374 4d61 7463 6865  ..z!ImpactMatche
-000010a0: 722e 6164 645f 6361 6e64 6964 6174 655f  r.add_candidate_
-000010b0: 7275 6c65 7372 4a00 0000 6302 0000 0000  rulesrJ...c.....
-000010c0: 0000 0000 0000 0004 0000 0004 0000 0043  ...............C
-000010d0: 0000 0073 c200 0000 7c00 6a00 a001 7c01  ...s....|.j...|.
-000010e0: a101 0100 7c00 6a02 a003 7c01 6a04 a101  ....|.j...|.j...
-000010f0: 7d02 7405 7c02 7406 8302 721b 7c00 6a07  }.t.|.t...r.|.j.
-00001100: 7c02 1900 a008 7c01 a101 0100 6e12 7405  |.....|.....n.t.
-00001110: 7c02 7409 8302 722d 7c02 4400 5d0a 7d03  |.t...r-|.D.].}.
-00001120: 7c00 6a07 7c03 1900 a008 7c01 a101 0100  |.j.|.....|.....
-00001130: 7122 7c01 6a0a 7c01 6a04 6b02 7235 6400  q"|.j.|.j.k.r5d.
-00001140: 5300 7c00 6a02 a003 7c01 6a0a a101 7d02  S.|.j...|.j...}.
-00001150: 7405 7c02 7406 8302 724b 7c00 6a07 7c02  t.|.t...rK|.j.|.
-00001160: 1900 a008 7c01 a101 0100 6400 5300 7405  ....|.....d.S.t.
-00001170: 7c02 7409 8302 725d 7c02 4400 5d0c 7d03  |.t...r]|.D.].}.
-00001180: 7c00 6a07 7c03 1900 a008 7c01 a101 0100  |.j.|.....|.....
-00001190: 7152 6400 5300 6400 5300 7247 0000 0029  qRd.S.d.S.rG...)
-000011a0: 0b72 2f00 0000 da06 6170 7065 6e64 7229  .r/.....appendr)
-000011b0: 0000 005a 1767 6574 5f6d 6174 6368 696e  ...Z.get_matchin
-000011c0: 675f 766f 6361 625f 7465 726d da04 776f  g_vocab_term..wo
-000011d0: 7264 722c 0000 00da 0373 7472 7233 0000  rdr,.....strr3..
-000011e0: 00da 0361 6464 7232 0000 0072 1f00 0000  ...addr2...r....
-000011f0: 2904 7239 0000 0072 4a00 0000 5a0b 766f  ).r9...rJ...Z.vo
-00001200: 6361 625f 7465 726d 735a 0a76 6f63 6162  cab_termsZ.vocab
-00001210: 5f74 6572 6d72 1600 0000 7216 0000 0072  _termr....r....r
-00001220: 1700 0000 da13 5f61 6464 5f73 656e 7465  ......_add_sente
-00001230: 6e63 655f 746f 6b65 6e7b 0000 0073 2200  nce_token{...s".
-00001240: 0000 0c01 0e01 0a01 1201 0a01 0801 1201  ................
-00001250: 0c01 0401 0e01 0a01 1401 0a01 0801 1201  ................
-00001260: 04fe 0401 7a21 496d 7061 6374 4d61 7463  ....z!ImpactMatc
-00001270: 6865 722e 5f61 6464 5f73 656e 7465 6e63  her._add_sentenc
-00001280: 655f 746f 6b65 6e72 3100 0000 da08 7365  e_tokenr1.....se
-00001290: 6e74 656e 6365 7230 0000 00da 0672 6574  ntencer0.....ret
-000012a0: 7572 6e63 0400 0000 0000 0000 0000 0000  urnc............
-000012b0: 0600 0000 0700 0000 4300 0000 736a 0000  ........C...sj..
-000012c0: 007c 0264 0119 007c 005f 007c 017c 0366  .|.d...|._.|.|.f
-000012d0: 027c 005f 0174 027c 0264 0219 0083 0144  .|._.t.|.d.....D
-000012e0: 005d 225c 027d 047d 0574 037c 056a 047c  .]"\.}.}.t.|.j.|
-000012f0: 047c 056a 0564 037c 0576 0072 217c 056a  .|.j.d.|.v.r!|.j
-00001300: 066e 0164 0064 048d 047d 057c 00a0 077c  .n.d.d...}.|...|
-00001310: 05a1 0101 007c 00a0 087c 056a 047c 056a  .....|...|.j.|.j
-00001320: 05a1 0201 0071 1064 0053 0029 054e da04  .....q.d.S.).N..
-00001330: 7465 7874 da06 746f 6b65 6e73 da03 706f  text..tokens..po
-00001340: 7329 0472 4d00 0000 da05 696e 6465 7872  s).rM.....indexr
-00001350: 1f00 0000 7255 0000 0029 0972 2e00 0000  ....rU...).r....
-00001360: da0b 7365 6e74 656e 6365 5f69 64da 0965  ..sentence_id..e
-00001370: 6e75 6d65 7261 7465 720b 0000 0072 4d00  numerater....rM.
-00001380: 0000 721f 0000 0072 5500 0000 7250 0000  ..r....rU...rP..
-00001390: 0072 4b00 0000 2906 7239 0000 0072 3100  .rK...).r9...r1.
-000013a0: 0000 7251 0000 0072 3000 0000 da02 7469  ..rQ...r0.....ti
-000013b0: 724a 0000 0072 1600 0000 7216 0000 0072  rJ...r....r....r
-000013c0: 1700 0000 da12 5f73 6574 5f64 6963 745f  ......_set_dict_
-000013d0: 7365 6e74 656e 6365 8c00 0000 730e 0000  sentence....s...
-000013e0: 000a 010a 0114 0122 010a 0112 0104 fd7a  .......".......z
-000013f0: 2049 6d70 6163 744d 6174 6368 6572 2e5f   ImpactMatcher._
-00001400: 7365 745f 6469 6374 5f73 656e 7465 6e63  set_dict_sentenc
-00001410: 6563 0400 0000 0000 0000 0000 0000 0800  ec..............
-00001420: 0000 0600 0000 4300 0000 7356 0000 007c  ......C...sV...|
-00001430: 027c 005f 007c 017c 0366 027c 005f 0174  .|._.|.|.f.|._.t
-00001440: 02a0 0364 017c 02a1 027d 0474 047c 0483  ...d.|...}.t.|..
-00001450: 0144 005d 165c 027d 057d 0674 057c 067c  .D.].\.}.}.t.|.|
-00001460: 057c 0664 028d 037d 077c 00a0 067c 07a1  .|.d...}.|...|..
-00001470: 0101 007c 00a0 077c 067c 06a1 0201 0071  ...|...|.|.....q
-00001480: 1264 0053 0029 034e 7a03 5c57 2b29 0172  .d.S.).Nz.\W+).r
-00001490: 1f00 0000 2908 722e 0000 0072 5700 0000  ....).r....rW...
-000014a0: 7222 0000 0072 4500 0000 7258 0000 0072  r"...rE...rX...r
-000014b0: 0b00 0000 7250 0000 0072 4b00 0000 2908  ....rP...rK...).
-000014c0: 7239 0000 0072 3100 0000 7251 0000 0072  r9...r1...rQ...r
-000014d0: 3000 0000 da05 776f 7264 735a 0277 6972  0.....wordsZ.wir
-000014e0: 4d00 0000 724a 0000 0072 1600 0000 7216  M...rJ...r....r.
-000014f0: 0000 0072 1700 0000 da14 5f73 6574 5f73  ...r......_set_s
-00001500: 7472 696e 675f 7365 6e74 656e 6365 9400  tring_sentence..
-00001510: 0000 7310 0000 0006 010a 010c 0110 010e  ..s.............
-00001520: 010a 010e 0104 fd7a 2249 6d70 6163 744d  .......z"ImpactM
-00001530: 6174 6368 6572 2e5f 7365 745f 7374 7269  atcher._set_stri
-00001540: 6e67 5f73 656e 7465 6e63 6563 0100 0000  ng_sentencec....
-00001550: 0000 0000 0000 0000 0100 0000 0200 0000  ................
-00001560: 4300 0000 732a 0000 0064 017c 005f 0067  C...s*...d.|._.g
-00001570: 007c 005f 0174 0274 0383 017c 005f 0474  .|._.t.t...|._.t
-00001580: 0274 0583 017c 005f 0664 007c 005f 0764  .t...|._.d.|._.d
-00001590: 0053 0029 024e 722b 0000 0029 0872 2e00  .S.).Nr+...).r..
-000015a0: 0000 722f 0000 0072 0200 0000 7232 0000  ..r/...r....r2..
-000015b0: 0072 3300 0000 7234 0000 0072 3500 0000  .r3...r4...r5...
-000015c0: 5a07 7365 6e74 5f69 64a9 0172 3900 0000  Z.sent_id..r9...
-000015d0: 7216 0000 0072 1600 0000 7217 0000 00da  r....r....r.....
-000015e0: 0f5f 7265 7365 745f 7365 6e74 656e 6365  ._reset_sentence
-000015f0: 9f00 0000 730a 0000 0006 0106 010a 010a  ....s...........
-00001600: 010a 017a 1d49 6d70 6163 744d 6174 6368  ...z.ImpactMatch
-00001610: 6572 2e5f 7265 7365 745f 7365 6e74 656e  er._reset_senten
-00001620: 6365 6304 0000 0000 0000 0000 0000 0004  cec.............
-00001630: 0000 0005 0000 0043 0000 0073 5e00 0000  .......C...s^...
-00001640: 7c00 a000 a100 0100 7c03 7c00 5f01 7402  |.......|.|._.t.
-00001650: 7c02 7403 8302 721d 6401 7c02 7600 721d  |.t...r.d.|.v.r.
-00001660: 6402 7c02 7600 721d 7c00 a004 7c01 7c02  d.|.v.r.|...|.|.
-00001670: 7c03 a103 0100 6400 5300 7402 7c02 7405  |.....d.S.t.|.t.
-00001680: 8302 722b 7c00 a006 7c01 7c02 7c03 a103  ..r+|...|.|.|...
-00001690: 0100 6400 5300 7407 6403 8301 8201 2904  ..d.S.t.d.....).
-000016a0: 4e72 5300 0000 7254 0000 007a 5273 656e  NrS...rT...zRsen
-000016b0: 7465 6e63 6520 6d75 7374 2062 6520 6569  tence must be ei
-000016c0: 7468 6572 2061 2073 7472 696e 672c 2061  ther a string, a
-000016d0: 6e20 5365 6e74 656e 6365 206f 626a 6563  n Sentence objec
-000016e0: 7420 6672 6f6d 2041 6c70 696e 6f2c 2053  t from Alpino, S
-000016f0: 7061 6379 206f 7220 5374 616e 7a61 2e29  pacy or Stanza.)
-00001700: 0872 5e00 0000 7230 0000 0072 2c00 0000  .r^...r0...r,...
-00001710: da04 6469 6374 725a 0000 0072 4e00 0000  ..dictrZ...rN...
-00001720: 725c 0000 0072 2d00 0000 2904 7239 0000  r\...r-...).r9..
-00001730: 0072 3100 0000 7251 0000 0072 3000 0000  .r1...rQ...r0...
-00001740: 7216 0000 0072 1600 0000 7217 0000 00da  r....r....r.....
-00001750: 0d5f 7365 745f 7365 6e74 656e 6365 a600  ._set_sentence..
-00001760: 0000 7312 0000 0008 0106 011a 0112 010a  ..s.............
-00001770: 0112 0102 0202 0104 ff7a 1b49 6d70 6163  .........z.Impac
-00001780: 744d 6174 6368 6572 2e5f 7365 745f 7365  tMatcher._set_se
-00001790: 6e74 656e 6365 7253 0000 0063 0300 0000  ntencerS...c....
-000017a0: 0000 0000 0000 0000 0500 0000 0600 0000  ................
-000017b0: 6300 0000 7330 0000 0081 0074 0074 017c  c...s0.....t.t.|
-000017c0: 0183 0183 0144 005d 0e5c 027d 037d 047c  .....D.].\.}.}.|
-000017d0: 00a0 027c 037c 047c 02a1 0301 007c 0356  ...|.|.|.....|.V
-000017e0: 0001 0071 0764 0053 0072 4700 0000 2903  ...q.d.S.rG...).
-000017f0: 7258 0000 0072 0600 0000 7260 0000 0029  rX...r....r`...)
-00001800: 0572 3900 0000 7253 0000 0072 3000 0000  .r9...rS...r0...
-00001810: da02 7369 da04 7365 6e74 7216 0000 0072  ..si..sentr....r
-00001820: 1600 0000 7217 0000 00da 145f 6974 6572  ....r......_iter
-00001830: 5f74 6578 745f 7365 6e74 656e 6365 73b1  _text_sentences.
-00001840: 0000 0073 0a00 0000 0280 1401 0e01 0801  ...s............
-00001850: 04fe 7a22 496d 7061 6374 4d61 7463 6865  ..z"ImpactMatche
-00001860: 722e 5f69 7465 725f 7465 7874 5f73 656e  r._iter_text_sen
-00001870: 7465 6e63 6573 da0f 696e 636c 7564 655f  tences..include_
-00001880: 6e65 7574 7261 6c63 0400 0000 0000 0000  neutralc........
-00001890: 0000 0000 0800 0000 0400 0000 4300 0000  ............C...
-000018a0: 733a 0000 0067 007d 047c 00a0 007c 017c  s:...g.}.|...|.|
-000018b0: 02a1 0244 005d 0b7d 057c 00a0 01a1 007d  ...D.].}.|.....}
-000018c0: 067c 04a0 027c 06a1 0101 0071 087c 006a  .|...|.....q.|.j
-000018d0: 037c 047c 0364 018d 027d 077c 0753 0029  .|.|.d...}.|.S.)
-000018e0: 024e 2901 7264 0000 0029 0472 6300 0000  .N).rd...).rc...
-000018f0: da0c 5f6d 6174 6368 5f72 756c 6573 da06  .._match_rules..
-00001900: 6578 7465 6e64 da15 636f 6d70 7574 655f  extend..compute_
-00001910: 7265 7669 6577 5f69 6d70 6163 7429 0872  review_impact).r
-00001920: 3900 0000 7253 0000 0072 3000 0000 7264  9...rS...r0...rd
-00001930: 0000 005a 0b61 6c6c 5f6d 6174 6368 6573  ...Z.all_matches
-00001940: da01 5f5a 1073 656e 7465 6e63 655f 6d61  .._Z.sentence_ma
-00001950: 7463 6865 73da 0d72 6576 6965 775f 696d  tches..review_im
-00001960: 7061 6374 7216 0000 0072 1600 0000 7217  pactr....r....r.
-00001970: 0000 00da 0c61 6e61 6c79 7365 5f74 6578  .....analyse_tex
-00001980: 74b6 0000 0073 1000 0000 0402 1001 0801  t....s..........
-00001990: 0c01 0601 0201 06ff 0402 7a1a 496d 7061  ..........z.Impa
-000019a0: 6374 4d61 7463 6865 722e 616e 616c 7973  ctMatcher.analys
-000019b0: 655f 7465 7874 5463 0300 0000 0000 0000  e_textTc........
-000019c0: 0000 0000 0300 0000 0400 0000 4300 0000  ............C...
-000019d0: 7324 0000 007c 0272 0d74 00a0 0164 017c  s$...|.r.t...d.|
-000019e0: 0117 0064 0117 007c 006a 02a1 0253 007c  ...d...|.j...S.|
-000019f0: 017c 006a 0276 0053 0029 027a a50a 2020  .|.j.v.S.).z..  
-00001a00: 2020 2020 2020 6368 6563 6b20 6966 2074        check if t
-00001a10: 6572 6d20 6f63 6375 7273 2069 6e20 7365  erm occurs in se
-00001a20: 6e74 656e 6365 2073 7472 696e 672e 0a20  ntence string.. 
-00001a30: 2020 2020 2020 2041 7373 756d 6573 2077         Assumes w
-00001a40: 6f72 6420 626f 756e 6461 7269 6573 2008  ord boundaries .
-00001a50: 7465 726d 0820 6279 2064 6566 6175 6c74  term. by default
-00001a60: 2e0a 2020 2020 2020 2020 5573 6520 776f  ..        Use wo
-00001a70: 7264 5f62 6f75 6e64 6172 6965 733d 4661  rd_boundaries=Fa
-00001a80: 6c73 6520 666f 7220 7075 7265 2073 7472  lse for pure str
-00001a90: 696e 6720 6d61 7463 680a 2020 2020 2020  ing match.      
-00001aa0: 2020 fa02 5c62 2903 7222 0000 00da 0673    ..\b).r".....s
-00001ab0: 6561 7263 6872 2e00 0000 2903 7239 0000  earchr....).r9..
-00001ac0: 0072 2000 0000 5a0f 776f 7264 5f62 6f75  .r ...Z.word_bou
-00001ad0: 6e64 6172 6965 7372 1600 0000 7216 0000  ndariesr....r...
-00001ae0: 0072 1700 0000 da13 7465 726d 5f73 656e  .r......term_sen
-00001af0: 7465 6e63 655f 6d61 7463 68c0 0000 0073  tence_match....s
-00001b00: 0600 0000 0406 1601 0a02 7a21 496d 7061  ..........z!Impa
-00001b10: 6374 4d61 7463 6865 722e 7465 726d 5f73  ctMatcher.term_s
-00001b20: 656e 7465 6e63 655f 6d61 7463 6863 0300  entence_matchc..
-00001b30: 0000 0000 0000 0000 0000 0600 0000 0400  ................
-00001b40: 0000 6300 0000 7356 0000 0081 007c 017c  ..c...sV.....|.|
-00001b50: 006a 0076 0072 0b7c 006a 007c 0119 006e  .j.v.r.|.j.|...n
-00001b60: 0167 007d 037c 0344 005d 197d 047c 0272  .g.}.|.D.].}.|.r
-00001b70: 1d7c 046a 01a0 02a1 007d 057c 01a0 02a1  .|.j.....}.|....
-00001b80: 007d 016e 037c 046a 017d 0574 037c 057c  .}.n.|.j.}.t.|.|
-00001b90: 0183 0272 287c 0456 0001 0071 0f64 0053  ...r(|.V...q.d.S
-00001ba0: 0072 4700 0000 2904 7233 0000 0072 4d00  .rG...).r3...rM.
-00001bb0: 0000 7214 0000 0072 1d00 0000 2906 7239  ..r....r....).r9
-00001bc0: 0000 00da 0a6d 6174 6368 5f74 6572 6dda  .....match_term.
-00001bd0: 0a69 676e 6f72 6563 6173 65da 0c6d 6174  .ignorecase..mat
-00001be0: 6368 5f74 6f6b 656e 7372 4a00 0000 724d  ch_tokensrJ...rM
-00001bf0: 0000 0072 1600 0000 7216 0000 0072 1700  ...r....r....r..
-00001c00: 0000 da20 6765 745f 7365 6e74 656e 6365  ... get_sentence
-00001c10: 5f77 6f72 6473 5f6d 6174 6368 696e 675f  _words_matching_
-00001c20: 7465 726d cb00 0000 7316 0000 0002 8018  term....s.......
-00001c30: 0108 0104 010a 010a 0106 020a 0106 0102  ................
-00001c40: 8004 f97a 2e49 6d70 6163 744d 6174 6368  ...z.ImpactMatch
-00001c50: 6572 2e67 6574 5f73 656e 7465 6e63 655f  er.get_sentence_
-00001c60: 776f 7264 735f 6d61 7463 6869 6e67 5f74  words_matching_t
-00001c70: 6572 6d63 0400 0000 0000 0000 0000 0000  ermc............
-00001c80: 0800 0000 0600 0000 6300 0000 73fc 0000  ........c...s...
-00001c90: 0081 007c 006a 0072 1674 0164 017c 017c  ...|.j.r.t.d.|.|
-00001ca0: 0283 0301 0074 017c 006a 0283 0101 0074  .....t.|.j.....t
-00001cb0: 017c 017c 006a 0276 0083 0101 007c 017c  .|.|.j.v.....|.|
-00001cc0: 006a 0276 0072 207c 006a 027c 0119 006e  .j.v.r |.j.|...n
-00001cd0: 0167 007d 047c 0444 005d 577d 057c 0372  .g.}.|.D.]W}.|.r
-00001ce0: 377c 056a 03a0 04a1 007d 067c 056a 05a0  7|.j.....}.|.j..
-00001cf0: 04a1 007d 077c 01a0 04a1 007d 016e 067c  ...}.|.....}.n.|
-00001d00: 056a 037d 067c 056a 057d 077c 006a 0072  .j.}.|.j.}.|.j.r
-00001d10: 4974 0164 027c 056a 0364 037c 056a 0683  It.d.|.j.d.|.j..
-00001d20: 0401 0074 077c 067c 0183 0273 5474 077c  ...t.|.|...sTt.|
-00001d30: 077c 0183 0273 5471 247c 0272 637c 056a  .|...sTq$|.rc|.j
-00001d40: 0672 637c 056a 067c 026b 0273 637c 056a  .rc|.j.|.k.sc|.j
-00001d50: 0664 046b 0272 6e7c 006a 0072 6a74 0164  .d.k.rn|.j.rjt.d
-00001d60: 0583 0101 007c 0556 0001 0071 247c 006a  .....|.V...q$|.j
-00001d70: 0072 7b74 0164 0683 0101 0074 017c 0564  .r{t.d.....t.|.d
-00001d80: 0719 0083 0101 0071 2464 0053 0029 084e  .......q$d.S.).N
-00001d90: 7a21 6c6f 6f6b 696e 6720 666f 7220 6c65  z!looking for le
-00001da0: 6d6d 6173 206d 6174 6368 696e 6720 7465  mmas matching te
-00001db0: 726d 3a7a 0709 6c65 6d6d 613a 7a04 706f  rm:z..lemma:z.po
-00001dc0: 733a da04 6e61 6d65 7a17 4d41 5443 4820  s:..namez.MATCH 
-00001dd0: 4f46 204c 454d 4d41 2041 4e44 2050 4f53  OF LEMMA AND POS
-00001de0: 217a 1e4d 4154 4348 204f 4620 4c45 4d4d  !z.MATCH OF LEMM
-00001df0: 4120 4255 5420 4e4f 5420 4f46 2050 4f53  A BUT NOT OF POS
-00001e00: 2172 5500 0000 2908 722a 0000 0072 1c00  !rU...).r*...r..
-00001e10: 0000 7233 0000 0072 1f00 0000 7214 0000  ..r3...r....r...
-00001e20: 0072 4d00 0000 7255 0000 0072 1d00 0000  .rM...rU...r....
-00001e30: 2908 7239 0000 0072 6e00 0000 da09 6d61  ).r9...rn.....ma
-00001e40: 7463 685f 706f 7372 6f00 0000 7270 0000  tch_posro...rp..
-00001e50: 0072 4a00 0000 721f 0000 0072 4d00 0000  .rJ...r....rM...
-00001e60: 7216 0000 0072 1600 0000 7217 0000 00da  r....r....r.....
-00001e70: 2167 6574 5f73 656e 7465 6e63 655f 6c65  !get_sentence_le
-00001e80: 6d6d 6173 5f6d 6174 6368 696e 675f 7465  mmas_matching_te
-00001e90: 726d d600 0000 7334 0000 0002 8006 010c  rm....s4........
-00001ea0: 010a 010e 0118 0108 0104 010a 010a 010a  ................
-00001eb0: 0106 0206 0106 0112 0114 0302 011e 0106  ................
-00001ec0: 0108 0108 0106 0108 010c 0102 8004 ec7a  ...............z
-00001ed0: 2f49 6d70 6163 744d 6174 6368 6572 2e67  /ImpactMatcher.g
-00001ee0: 6574 5f73 656e 7465 6e63 655f 6c65 6d6d  et_sentence_lemm
-00001ef0: 6173 5f6d 6174 6368 696e 675f 7465 726d  as_matching_term
-00001f00: da0d 6e65 6967 6862 6f75 7268 6f6f 6463  ..neighbourhoodc
-00001f10: 0400 0000 0000 0000 0000 0000 0700 0000  ................
-00001f20: 0800 0000 6300 0000 73c4 0000 0081 007c  ....c...s......|
-00001f30: 006a 0072 0b74 0164 017c 0164 027c 0283  .j.r.t.d.|.d.|..
-00001f40: 0401 007c 006a 027d 047c 0372 187c 04a0  ...|.j.}.|.r.|..
-00001f50: 03a1 007d 047c 01a0 03a1 007d 017c 006a  ...}.|.....}.|.j
-00001f60: 0072 2074 0164 037c 0483 0201 0064 047c  .r t.d.|.....d.|
-00001f70: 0117 0064 0417 007d 057c 0264 056b 0272  ...d...}.|.d.k.r
-00001f80: 3764 067c 0517 007d 057c 006a 0072 3674  7d.|...}.|.j.r6t
-00001f90: 0164 077c 0583 0201 006e 087c 0264 086b  .d.|.....n.|.d.k
-00001fa0: 0272 3f7c 0564 0917 007d 057a 0f74 04a0  .r?|.d...}.z.t..
-00001fb0: 057c 057c 04a1 0244 005d 057d 067c 0656  .|.|...D.].}.|.V
-00001fc0: 0001 0071 4657 0064 0053 0004 0074 046a  ...qFW.d.S...t.j
-00001fd0: 0679 6101 0001 0001 0074 0164 0a7c 0583  .ya......t.d.|..
-00001fe0: 0201 0074 0164 037c 0483 0201 0082 0077  ...t.d.|.......w
-00001ff0: 0029 0b4e 7a2c 6c6f 6f6b 696e 6720 666f  .).Nz,looking fo
-00002000: 7220 7365 6e74 656e 6365 2073 7472 696e  r sentence strin
-00002010: 6720 6d61 7463 6869 6e67 2070 6872 6173  g matching phras
-00002020: 653a 7a0c 616e 6420 6c6f 6361 7469 6f6e  e:z.and location
-00002030: fa09 7365 6e74 656e 6365 3a72 6b00 0000  ..sentence:rk...
-00002040: da0e 7365 6e74 656e 6365 5f73 7461 7274  ..sentence_start
-00002050: fa01 5eda 0c6d 6174 6368 5f73 7472 696e  ..^..match_strin
-00002060: 675a 0c73 656e 7465 6e63 655f 656e 64fa  gZ.sentence_end.
-00002070: 0124 7a0d 6d61 7463 685f 7374 7269 6e67  .$z.match_string
-00002080: 3a29 0772 2a00 0000 721c 0000 0072 2e00  :).r*...r....r..
-00002090: 0000 7214 0000 0072 2200 0000 da08 6669  ..r....r".....fi
-000020a0: 6e64 6974 6572 da05 6572 726f 7229 0772  nditer..error).r
-000020b0: 3900 0000 726e 0000 00da 086c 6f63 6174  9...rn.....locat
-000020c0: 696f 6e72 6f00 0000 7251 0000 0072 7900  ionro...rQ...ry.
-000020d0: 0000 7215 0000 0072 1600 0000 7216 0000  ..r....r....r...
-000020e0: 0072 1700 0000 da21 6765 745f 7365 6e74  .r.....!get_sent
-000020f0: 656e 6365 5f73 7472 696e 675f 6d61 7463  ence_string_matc
-00002100: 6869 6e67 5f74 6572 6df2 0000 0073 3400  hing_term....s4.
-00002110: 0000 0280 0601 0e01 0601 0401 0801 0801  ................
-00002120: 0601 0a01 0c01 0801 0801 0601 0a01 0280  ................
-00002130: 0801 0801 0201 1001 0801 06ff 0e02 0a01  ................
-00002140: 0a01 0201 02fd 7a2f 496d 7061 6374 4d61  ......z/ImpactMa
-00002150: 7463 6865 722e 6765 745f 7365 6e74 656e  tcher.get_senten
-00002160: 6365 5f73 7472 696e 675f 6d61 7463 6869  ce_string_matchi
-00002170: 6e67 5f74 6572 6d63 0200 0000 0000 0000  ng_termc........
-00002180: 0000 0000 0200 0000 0300 0000 4300 0000  ............C...
-00002190: 7312 0000 007c 00a0 007c 01a1 0101 007c  s....|...|.....|
-000021a0: 00a0 01a1 0053 0029 017a 3652 6574 7572  .....S.).z6Retur
-000021b0: 6e20 616c 6c20 6d61 7463 6869 6e67 2069  n all matching i
-000021c0: 6d70 6163 7420 7275 6c65 7320 666f 7220  mpact rules for 
-000021d0: 6120 6769 7665 6e20 7365 6e74 656e 6365  a given sentence
-000021e0: 2e29 0272 6000 0000 7265 0000 0029 0272  .).r`...re...).r
-000021f0: 3900 0000 7251 0000 0072 1600 0000 7216  9...rQ...r....r.
-00002200: 0000 0072 1700 0000 da13 6669 6e64 5f69  ...r......find_i
-00002210: 6d70 6163 745f 6d61 7463 6865 730a 0100  mpact_matches...
-00002220: 0073 0400 0000 0a02 0801 7a21 496d 7061  .s........z!Impa
-00002230: 6374 4d61 7463 6865 722e 6669 6e64 5f69  ctMatcher.find_i
-00002240: 6d70 6163 745f 6d61 7463 6865 7363 0100  mpact_matchesc..
-00002250: 0000 0000 0000 0000 0000 0100 0000 0300  ................
-00002260: 0000 0300 0000 7314 0000 0087 0066 0164  ......s......f.d
-00002270: 0164 0284 0888 006a 0044 0083 0153 0029  .d.....j.D...S.)
-00002280: 037a 3c4d 6174 6368 2073 656e 7465 6e63  .z<Match sentenc
-00002290: 6520 6167 6169 6e73 7420 616c 6c20 696d  e against all im
-000022a0: 7061 6374 2072 756c 6573 206f 6620 7468  pact rules of th
-000022b0: 6520 696d 7061 6374 206d 6f64 656c 2e63  e impact model.c
-000022c0: 0100 0000 0000 0000 0000 0000 0300 0000  ................
-000022d0: 0500 0000 1300 0000 7320 0000 0067 007c  ........s ...g.|
-000022e0: 005d 0c7d 0188 00a0 007c 01a1 0144 005d  .].}.....|...D.]
-000022f0: 047d 027c 0291 0371 0971 0253 0072 1600  .}.|...q.q.S.r..
-00002300: 0000 2901 da0a 6d61 7463 685f 7275 6c65  ..)...match_rule
-00002310: 2903 da02 2e30 da0b 696d 7061 6374 5f72  )....0..impact_r
-00002320: 756c 6572 1500 0000 725d 0000 0072 1600  uler....r]...r..
-00002330: 0000 7217 0000 00da 0a3c 6c69 7374 636f  ..r......<listco
-00002340: 6d70 3e11 0100 0073 0200 0000 2000 7a2e  mp>....s.... .z.
-00002350: 496d 7061 6374 4d61 7463 6865 722e 5f6d  ImpactMatcher._m
-00002360: 6174 6368 5f72 756c 6573 2e3c 6c6f 6361  atch_rules.<loca
-00002370: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 2901  ls>.<listcomp>).
-00002380: 7235 0000 0072 5d00 0000 7216 0000 0072  r5...r]...r....r
-00002390: 5d00 0000 7217 0000 0072 6500 0000 0f01  ]...r....re.....
-000023a0: 0000 7302 0000 0014 027a 1a49 6d70 6163  ..s......z.Impac
-000023b0: 744d 6174 6368 6572 2e5f 6d61 7463 685f  tMatcher._match_
-000023c0: 7275 6c65 7372 8200 0000 6303 0000 0000  rulesr....c.....
-000023d0: 0000 0000 0000 0003 0000 0003 0000 0043  ...............C
-000023e0: 0000 0073 5200 0000 7c02 720e 7c00 6a00  ...sR...|.r.|.j.
-000023f0: 7209 7401 6401 8301 0100 7c00 a002 7c02  r.t.d.....|...|.
-00002400: a101 0100 7c01 6a03 6a04 6402 6b02 7219  ....|.j.j.d.k.r.
-00002410: 7c00 a005 7c01 a101 5300 7c01 6a03 6a04  |...|...S.|.j.j.
-00002420: 6403 6b02 7224 7c00 a005 7c01 a101 5300  d.k.r$|...|...S.
-00002430: 7c00 a006 7c01 a101 5300 2904 7a2e 4d61  |...|...S.).z.Ma
-00002440: 7463 6820 7365 6e74 656e 6365 2061 6761  tch sentence aga
-00002450: 696e 7374 2061 2073 7065 6369 6669 6320  inst a specific 
-00002460: 696d 7061 6374 2072 756c 652e 7a26 7365  impact rule.z&se
-00002470: 7474 696e 6720 7365 6e74 656e 6365 2066  tting sentence f
-00002480: 6f72 2073 696e 676c 6520 7275 6c65 206d  or single rule m
-00002490: 6174 6368 723d 0000 0072 3e00 0000 2907  atchr=...r>...).
-000024a0: 722a 0000 0072 1c00 0000 7260 0000 0072  r*...r....r`...r
-000024b0: 4800 0000 7249 0000 00da 136d 6174 6368  H...rI.....match
-000024c0: 5f69 6d70 6163 745f 7068 7261 7365 da11  _impact_phrase..
-000024d0: 6d61 7463 685f 696d 7061 6374 5f74 6572  match_impact_ter
-000024e0: 6d29 0372 3900 0000 7282 0000 0072 5100  m).r9...r....rQ.
-000024f0: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
-00002500: 0072 8000 0000 1301 0000 7312 0000 0004  .r........s.....
-00002510: 0206 0108 010a 010c 010a 010c 010a 010a  ................
-00002520: 027a 1849 6d70 6163 744d 6174 6368 6572  .z.ImpactMatcher
-00002530: 2e6d 6174 6368 5f72 756c 6563 0200 0000  .match_rulec....
-00002540: 0000 0000 0000 0000 0500 0000 0c00 0000  ................
-00002550: 4300 0000 73ac 0000 0067 007d 027c 006a  C...s....g.}.|.j
-00002560: 0072 1874 0164 017c 016a 026a 0383 0201  .r.t.d.|.j.j....
-00002570: 0074 0164 027c 016a 0283 0201 0074 0164  .t.d.|.j.....t.d
-00002580: 037c 006a 0483 0201 007c 006a 057c 016a  .|.j.....|.j.|.j
-00002590: 026a 037c 016a 0664 048d 0244 005d 317d  .j.|.j.d...D.]1}
-000025a0: 0374 077c 03a0 0864 05a1 0164 067c 03a0  .t.|...d...d.|..
-000025b0: 09a1 007c 016a 026a 037c 016a 026a 0a7c  ...|.j.j.|.j.j.|
-000025c0: 016a 0b7c 006a 0c7c 006a 0d7c 006a 0464  .j.|.j.|.j.|.j.d
-000025d0: 078d 097d 047c 00a0 0e7c 017c 04a1 0272  ...}.|...|.|...r
-000025e0: 4a7c 02a0 0f7c 04a1 0101 0071 227c 006a  J|...|.....q"|.j
-000025f0: 0072 5374 0164 087c 016a 1083 0201 0071  .rSt.d.|.j.....q
-00002600: 227c 0253 0029 097a 2843 6865 636b 2069  "|.S.).z(Check i
-00002610: 6620 7365 6e74 656e 6365 206d 6174 6368  f sentence match
-00002620: 6573 2069 6d70 6163 7420 7068 7261 7365  es impact phrase
-00002630: 2e7a 0d6d 6174 6368 5f70 6872 6173 653a  .z.match_phrase:
-00002640: 7a0c 696d 7061 6374 5f74 6572 6d3a 7276  z.impact_term:rv
-00002650: 0000 00a9 0172 6f00 0000 7201 0000 004e  .....ro...r....N
-00002660: a903 7230 0000 0072 3100 0000 7251 0000  ..r0...r1...rQ..
-00002670: 00fa 1950 4852 4153 4520 434f 4e44 4954  ...PHRASE CONDIT
-00002680: 494f 4e20 4e4f 5420 4d45 543a 2911 722a  ION NOT MET:).r*
-00002690: 0000 0072 1c00 0000 7248 0000 0072 2400  ...r....rH...r$.
-000026a0: 0000 722e 0000 0072 7e00 0000 726f 0000  ..r....r~...ro..
-000026b0: 0072 0900 0000 da05 6772 6f75 70da 0573  .r......group..s
-000026c0: 7461 7274 7249 0000 0072 1200 0000 7230  tartrI...r....r0
-000026d0: 0000 0072 3100 0000 da0f 6d61 7463 685f  ...r1.....match_
-000026e0: 636f 6e64 6974 696f 6e72 4c00 0000 da09  conditionrL.....
-000026f0: 636f 6e64 6974 696f 6e29 0572 3900 0000  condition).r9...
-00002700: 7282 0000 00da 076d 6174 6368 6573 7215  r......matchesr.
-00002710: 0000 00da 0c69 6d70 6163 745f 6d61 7463  .....impact_matc
-00002720: 6872 1600 0000 7216 0000 0072 1700 0000  hr....r....r....
-00002730: 7284 0000 0020 0100 0073 2600 0000 0402  r.... ...s&.....
-00002740: 0601 0e01 0c01 0c01 0a01 0401 0aff 1802  ................
-00002750: 0a01 0801 0401 06fd 0c04 0c01 0601 0c01  ................
-00002760: 0280 0401 7a21 496d 7061 6374 4d61 7463  ....z!ImpactMatc
-00002770: 6865 722e 6d61 7463 685f 696d 7061 6374  her.match_impact
-00002780: 5f70 6872 6173 6563 0200 0000 0000 0000  _phrasec........
-00002790: 0000 0000 0700 0000 0c00 0000 4300 0000  ............C...
-000027a0: 73bc 0000 0067 007d 027c 016a 006a 017d  s....g.}.|.j.j.}
-000027b0: 037c 016a 006a 027d 047c 006a 0372 1a74  .|.j.j.}.|.j.r.t
-000027c0: 0464 017c 0364 027c 0483 0401 0074 0464  .d.|.d.|.....t.d
-000027d0: 037c 006a 0583 0201 007c 006a 067c 037c  .|.j.....|.j.|.|
-000027e0: 047c 016a 0764 048d 0344 005d 387d 0574  .|.j.d...D.]8}.t
-000027f0: 087c 056a 097c 056a 0a7c 056a 0b7c 016a  .|.j.|.j.|.j.|.j
-00002800: 006a 017c 016a 006a 0c7c 016a 0d7c 006a  .j.|.j.j.|.j.|.j
-00002810: 0e7c 006a 0f7c 006a 0564 058d 097d 067c  .|.j.|.j.d...}.|
-00002820: 006a 0372 4674 0464 067c 056a 0983 0201  .j.rFt.d.|.j....
-00002830: 007c 00a0 107c 017c 06a1 0272 527c 02a0  .|...|.|...rR|..
-00002840: 117c 06a1 0101 0071 237c 006a 0372 5b74  .|.....q#|.j.r[t
-00002850: 0464 077c 016a 1283 0201 0071 237c 0253  .d.|.j.....q#|.S
-00002860: 0029 087a 2643 6865 636b 2069 6620 7365  .).z&Check if se
-00002870: 6e74 656e 6365 206d 6174 6368 6573 2069  ntence matches i
-00002880: 6d70 6163 7420 7465 726d 2e7a 0b6d 6174  mpact term.z.mat
-00002890: 6368 5f74 6572 6d3a 7a0a 6d61 7463 685f  ch_term:z.match_
-000028a0: 706f 733a 7276 0000 0072 8600 0000 7287  pos:rv...r....r.
-000028b0: 0000 007a 0b6d 6174 6368 2074 6572 6d3a  ...z.match term:
-000028c0: 7288 0000 0029 1372 4800 0000 7224 0000  r....).rH...r$..
-000028d0: 0072 5500 0000 722a 0000 0072 1c00 0000  .rU...r*...r....
-000028e0: 722e 0000 0072 7400 0000 726f 0000 0072  r....rt...ro...r
-000028f0: 0900 0000 724d 0000 0072 1f00 0000 7256  ....rM...r....rV
-00002900: 0000 0072 4900 0000 7212 0000 0072 3000  ...rI...r....r0.
-00002910: 0000 7231 0000 0072 8b00 0000 724c 0000  ..r1...r....rL..
-00002920: 0072 8c00 0000 2907 7239 0000 0072 8200  .r....).r9...r..
-00002930: 0000 da0e 696d 7061 6374 5f6d 6174 6368  ....impact_match
-00002940: 6573 726e 0000 0072 7300 0000 5a0c 696d  esrn...rs...Z.im
-00002950: 7061 6374 5f74 6f6b 656e 728e 0000 0072  pact_tokenr....r
-00002960: 1600 0000 7216 0000 0072 1700 0000 7285  ....r....r....r.
-00002970: 0000 0033 0100 0073 2e00 0000 0402 0801  ...3...s........
-00002980: 0801 0601 0e01 0c01 0801 0401 0aff 0e02  ................
-00002990: 0c01 0401 0801 0401 06fc 0605 0c01 0c01  ................
-000029a0: 0c01 0601 0c01 0280 0401 7a1f 496d 7061  ..........z.Impa
-000029b0: 6374 4d61 7463 6865 722e 6d61 7463 685f  ctMatcher.match_
-000029c0: 696d 7061 6374 5f74 6572 6d72 8e00 0000  impact_termr....
-000029d0: 6303 0000 0000 0000 0000 0000 0004 0000  c...............
-000029e0: 0004 0000 0043 0000 0073 de00 0000 7c01  .....C...s....|.
-000029f0: 6a00 7305 6401 5300 7c00 6a01 7216 7402  j.s.d.S.|.j.r.t.
-00002a00: 6402 7c01 6a00 6403 1900 8302 0100 7402  d.|.j.d.......t.
-00002a10: 6404 7c01 6a00 8302 0100 7c01 6a00 6403  d.|.j.....|.j.d.
-00002a20: 1900 6405 6b02 7224 7c00 a003 7c01 7c02  ..d.k.r$|...|.|.
-00002a30: a102 7d03 6e19 7c01 6a00 6403 1900 6406  ..}.n.|.j.d...d.
-00002a40: 6b02 7232 7c00 a004 7c01 7c02 a102 7d03  k.r2|...|.|...}.
-00002a50: 6e0b 7c00 6a01 723b 7402 6407 7c01 6a00  n.|.j.r;t.d.|.j.
-00002a60: 8302 0100 6408 5300 7c01 6a05 724a 7c00  ....d.S.|.j.rJ|.
-00002a70: 6a01 7247 7402 6409 8301 0100 7c03 0c00  j.rGt.d.....|...
-00002a80: 7d03 7c00 6a01 726d 7c03 725f 7402 640a  }.|.j.rm|.r_t.d.
-00002a90: 7c01 6a00 8302 0100 7402 640b 7c02 8302  |.j.....t.d.|...
-00002aa0: 0100 7402 8300 0100 7c03 5300 7402 640c  ..t.....|.S.t.d.
-00002ab0: 7c01 6a00 8302 0100 7402 640b 7c02 8302  |.j.....t.d.|...
-00002ac0: 0100 7402 8300 0100 7c03 5300 290d fa49  ..t.....|.S.)..I
-00002ad0: 4368 6563 6b20 6966 2073 656e 7465 6e63  Check if sentenc
-00002ae0: 6520 7769 7468 2069 6d70 6163 7420 7465  e with impact te
-00002af0: 726d 206d 6174 6368 2061 6c73 6f20 6d61  rm match also ma
-00002b00: 7463 6865 7320 636f 6e74 6578 7420 636f  tches context co
-00002b10: 6e64 6974 696f 6e73 2e54 7a0f 636f 6e64  nditions.Tz.cond
-00002b20: 6974 696f 6e20 7479 7065 3a5a 0e63 6f6e  ition type:Z.con
-00002b30: 6469 7469 6f6e 5f74 7970 657a 0a63 6f6e  dition_typez.con
-00002b40: 6469 7469 6f6e 3ada 0b61 7370 6563 745f  dition:..aspect_
-00002b50: 7465 726d da0c 636f 6e74 6578 745f 7465  term..context_te
-00002b60: 726d 7a10 4f54 4845 5220 434f 4e44 4954  rmz.OTHER CONDIT
-00002b70: 494f 4e3a 467a 0f49 4e56 4552 5449 4e47  ION:Fz.INVERTING
-00002b80: 204d 4154 4348 7a13 4d41 5443 4849 4e47   MATCHz.MATCHING
-00002b90: 2043 4f4e 4449 5449 4f4e 3a7a 0d49 4d50   CONDITION:z.IMP
-00002ba0: 4143 545f 4d41 5443 483a 7a16 4e4f 204d  ACT_MATCH:z.NO M
-00002bb0: 4154 4348 494e 4720 434f 4e44 4954 494f  ATCHING CONDITIO
-00002bc0: 4e3a 2906 728c 0000 0072 2a00 0000 721c  N:).r....r*...r.
-00002bd0: 0000 00da 166d 6174 6368 5f61 7370 6563  .....match_aspec
-00002be0: 745f 636f 6e64 6974 696f 6eda 176d 6174  t_condition..mat
-00002bf0: 6368 5f63 6f6e 7465 7874 5f63 6f6e 6469  ch_context_condi
-00002c00: 7469 6f6e da06 6669 6c74 6572 2904 7239  tion..filter).r9
-00002c10: 0000 0072 8200 0000 728e 0000 0072 1500  ...r....r....r..
-00002c20: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
-00002c30: 0072 8b00 0000 4a01 0000 7334 0000 0006  .r....J...s4....
-00002c40: 0204 0106 0110 010c 010e 010e 010e 010e  ................
-00002c50: 0106 020c 0104 0106 0106 0108 0106 0106  ................
-00002c60: 0104 010c 010a 0106 0104 050c fd0a 0106  ................
-00002c70: 0104 017a 1d49 6d70 6163 744d 6174 6368  ...z.ImpactMatch
-00002c80: 6572 2e6d 6174 6368 5f63 6f6e 6469 7469  er.match_conditi
-00002c90: 6f6e 6303 0000 0000 0000 0000 0000 000a  onc.............
-00002ca0: 0000 0008 0000 0043 0000 0073 dc00 0000  .......C...s....
-00002cb0: 7c01 6a00 6401 1900 7d03 7c00 6a01 a002  |.j.d...}.|.j...
-00002cc0: 7c03 a101 7d04 7c04 7314 7403 6402 7c03  |...}.|.s.t.d.|.
-00002cd0: 8302 0100 6403 5300 7c04 6404 1900 4400  ....d.S.|.d...D.
-00002ce0: 5d53 7d05 6700 7d06 7c00 6a04 7c05 7c01  ]S}.g.}.|.j.|.|.
-00002cf0: 6a05 6405 8d02 4400 5d12 7d07 7406 7c07  j.d...D.].}.t.|.
-00002d00: 6a07 7c07 6a08 7c07 6a09 7c05 7c03 8305  j.|.j.|.j.|.|...
-00002d10: 7d08 7c06 a00a 7c08 a101 0100 7124 740b  }.|...|.....q$t.
-00002d20: 7c06 8301 6406 6b04 7243 7c06 7c02 5f0c  |...d.k.rC|.|._.
-00002d30: 0100 6407 5300 7c00 6a0d 7c05 6408 7c01  ..d.S.|.j.|.d.|.
-00002d40: 6a05 6405 8d03 4400 5d12 7d09 7406 7c09  j.d...D.].}.t.|.
-00002d50: 6a07 7c09 6a08 7c09 6a09 7c05 7c03 8305  j.|.j.|.j.|.|...
-00002d60: 7d08 7c06 a00a 7c08 a101 0100 714c 740b  }.|...|.....qLt.
-00002d70: 7c06 8301 6406 6b04 726b 7c06 7c02 5f0c  |...d.k.rk|.|._.
-00002d80: 0100 6407 5300 7118 6403 5300 2909 7a48  ..d.S.q.d.S.).zH
-00002d90: 4368 6563 6b20 6966 2073 656e 7465 6e63  Check if sentenc
-00002da0: 6520 7769 7468 2069 6d70 6163 7420 7465  e with impact te
-00002db0: 726d 206d 6174 6368 2061 6c73 6f20 6d61  rm match also ma
-00002dc0: 7463 6865 7320 6173 7065 6374 2063 6f6e  tches aspect con
-00002dd0: 6469 7469 6f6e 732e da0c 6173 7065 6374  ditions...aspect
-00002de0: 5f67 726f 7570 7a2e 4572 726f 7220 2d20  _groupz.Error - 
-00002df0: 6e6f 2061 7370 6563 7420 6772 6f75 7020  no aspect group 
-00002e00: 696e 666f 2066 6f72 2061 7370 6563 7420  info for aspect 
-00002e10: 6772 6f75 703a 4672 9100 0000 7286 0000  group:Fr....r...
-00002e20: 0072 0100 0000 544e 290e 728c 0000 0072  .r....TN).r....r
-00002e30: 2900 0000 7296 0000 0072 1c00 0000 7271  )...r....r....rq
-00002e40: 0000 0072 6f00 0000 720a 0000 0072 4d00  ...ro...r....rM.
-00002e50: 0000 721f 0000 0072 5600 0000 724c 0000  ..r....rV...rL..
-00002e60: 00da 036c 656e da11 636f 6e64 6974 696f  ...len..conditio
-00002e70: 6e5f 6d61 7463 6865 7372 7400 0000 290a  n_matchesrt...).
-00002e80: 7239 0000 0072 8200 0000 728e 0000 0072  r9...r....r....r
-00002e90: 9600 0000 5a0b 6173 7065 6374 5f69 6e66  ....Z.aspect_inf
-00002ea0: 6f72 9100 0000 7298 0000 005a 0c61 7370  or....r....Z.asp
-00002eb0: 6563 745f 6d61 7463 68da 0f63 6f6e 6469  ect_match..condi
-00002ec0: 7469 6f6e 5f6d 6174 6368 5a0c 6173 7065  tion_matchZ.aspe
-00002ed0: 6374 5f74 6f6b 656e 7216 0000 0072 1600  ct_tokenr....r..
-00002ee0: 0000 7217 0000 0072 9300 0000 6801 0000  ..r....r....h...
-00002ef0: 733a 0000 000a 020c 0104 010a 0104 010c  s:..............
-00002f00: 0104 0106 0104 010a ff0e 0204 0104 ff0c  ................
-00002f10: 020c 0106 0106 0108 0104 010a ff0e 0204  ................
-00002f20: 0104 ff0c 020c 0106 0106 0102 fe04 037a  ...............z
-00002f30: 2449 6d70 6163 744d 6174 6368 6572 2e6d  $ImpactMatcher.m
-00002f40: 6174 6368 5f61 7370 6563 745f 636f 6e64  atch_aspect_cond
-00002f50: 6974 696f 6e63 0300 0000 0000 0000 0000  itionc..........
-00002f60: 0000 0700 0000 0800 0000 4300 0000 73a2  ..........C...s.
-00002f70: 0000 007c 016a 0064 0119 007d 0367 007d  ...|.j.d...}.g.}
-00002f80: 047c 016a 0064 0219 0064 036b 0272 197c  .|.j.d...d.k.r.|
-00002f90: 006a 0172 1974 0264 047c 0364 057c 016a  .j.r.t.d.|.d.|.j
-00002fa0: 0083 0401 007c 006a 037c 037c 016a 0064  .....|.j.|.|.j.d
-00002fb0: 0219 007c 016a 0464 068d 0344 005d 1e7d  ...|.j.d...D.].}
-00002fc0: 0574 057c 05a0 0664 07a1 0164 087c 05a0  .t.|...d...d.|..
-00002fd0: 07a1 007c 037c 016a 0064 0919 0083 057d  ...|.|.j.d.....}
-00002fe0: 067c 006a 0172 3e74 0264 0a83 0101 007c  .|.j.r>t.d.....|
-00002ff0: 04a0 087c 06a1 0101 0071 2574 097c 0483  ...|.....q%t.|..
-00003000: 0164 076b 0472 4f7c 047c 025f 0a64 0b53  .d.k.rO|.|._.d.S
-00003010: 0064 0c53 0029 0d72 9000 0000 7292 0000  .d.S.).r....r...
-00003020: 0072 7d00 0000 7277 0000 007a 106c 6f6f  .r}...rw...z.loo
-00003030: 6b69 6e67 2066 6f72 2074 6572 6d7a 0f20  king for termz. 
-00003040: 7769 7468 2063 6f6e 6469 7469 6f6e 7286  with conditionr.
-00003050: 0000 0072 0100 0000 4e72 3c00 0000 7a17  ...r....Nr<...z.
-00003060: 434f 4e54 4558 5420 434f 4e44 4954 494f  CONTEXT CONDITIO
-00003070: 4e20 4d41 5443 4854 4629 0b72 8c00 0000  N MATCHTF).r....
-00003080: 722a 0000 0072 1c00 0000 727e 0000 0072  r*...r....r~...r
-00003090: 6f00 0000 720a 0000 0072 8900 0000 728a  o...r....r....r.
-000030a0: 0000 0072 4c00 0000 7297 0000 0072 9800  ...rL...r....r..
-000030b0: 0000 2907 7239 0000 0072 8200 0000 728e  ..).r9...r....r.
-000030c0: 0000 0072 9200 0000 7298 0000 005a 0d63  ...r....r....Z.c
-000030d0: 6f6e 7465 7874 5f6d 6174 6368 7299 0000  ontext_matchr...
-000030e0: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
-000030f0: 7294 0000 0083 0100 0073 2400 0000 0a02  r........s$.....
-00003100: 0401 0e01 0601 1001 0e01 0401 0aff 1202  ................
-00003110: 0a01 04ff 0602 0801 0c01 0c01 0601 0401  ................
-00003120: 0402 7a25 496d 7061 6374 4d61 7463 6865  ..z%ImpactMatche
-00003130: 722e 6d61 7463 685f 636f 6e74 6578 745f  r.match_context_
-00003140: 636f 6e64 6974 696f 6e72 1500 0000 6302  conditionr....c.
-00003150: 0000 0000 0000 0000 0000 0007 0000 0004  ................
-00003160: 0000 0043 0000 0073 8a00 0000 7c01 6a00  ...C...s....|.j.
-00003170: 7c01 6a01 7c01 6a02 6401 9c03 7d02 7403  |.j.|.j.d...}.t.
-00003180: 7c00 6a04 1900 4400 5d06 7d03 6402 7c02  |.j...D.].}.d.|.
-00003190: 7c03 3c00 710e 7405 4400 5d09 7d04 7c01  |.<.q.t.D.].}.|.
-000031a0: a006 7c04 a101 7c02 7c04 3c00 7117 7407  ..|...|.|.<.q.t.
-000031b0: 4400 5d1f 7d05 7408 7c01 6a09 8301 6402  D.].}.t.|.j...d.
-000031c0: 6b04 7242 7c05 a00a 6403 a101 7233 7c05  k.rB|...d...r3|.
-000031d0: 6e04 6404 7c05 9b00 9d02 7d06 7c01 6a09  n.d.|.....}.|.j.
-000031e0: 6402 1900 a006 7c05 a101 7c02 7c06 3c00  d.....|...|.|.<.
-000031f0: 7123 7c02 5300 2905 4e72 8700 0000 7201  q#|.S.).Nr....r.
-00003200: 0000 00da 0463 6f6e 64da 0a63 6f6e 6469  .....cond..condi
-00003210: 7469 6f6e 5f29 0b72 3000 0000 7231 0000  tion_).r0...r1..
-00003220: 0072 5100 0000 720c 0000 0072 2800 0000  .rQ...r....r(...
-00003230: 720d 0000 00da 105f 5f67 6574 6174 7472  r......__getattr
-00003240: 6962 7574 655f 5f72 0e00 0000 7297 0000  ibute__r....r...
-00003250: 0072 9800 0000 da0a 7374 6172 7473 7769  .r......startswi
-00003260: 7468 2907 7239 0000 0072 1500 0000 da06  th).r9...r......
-00003270: 696d 7061 6374 7212 0000 00da 0566 6965  impactr......fie
-00003280: 6c64 da0a 636f 6e64 5f66 6965 6c64 da0d  ld..cond_field..
-00003290: 6469 7370 6c61 795f 6669 656c 6472 1600  display_fieldr..
-000032a0: 0000 7216 0000 0072 1700 0000 da12 696e  ..r....r......in
-000032b0: 6974 5f69 6d70 6163 745f 7363 6f72 6573  it_impact_scores
-000032c0: 9701 0000 731c 0000 0004 0204 0104 0106  ....s...........
-000032d0: fd0e 050a 0108 0110 0108 010e 0118 0114  ................
-000032e0: 0102 8004 017a 2049 6d70 6163 744d 6174  .....z ImpactMat
-000032f0: 6368 6572 2e69 6e69 745f 696d 7061 6374  cher.init_impact
-00003300: 5f73 636f 7265 7372 8f00 0000 6303 0000  _scoresr....c...
-00003310: 0000 0000 0000 0000 000c 0000 0005 0000  ................
-00003320: 0043 0000 0073 3401 0000 6800 6401 a301  .C...s4...h.d...
-00003330: 7d03 6700 7d04 7400 8300 7d05 7c01 4400  }.g.}.t...}.|.D.
-00003340: 5d8c 7d06 7c00 a001 7c06 a101 7d07 7c02  ].}.|...|...}.|.
-00003350: 6402 7500 721c 7c06 6a02 6403 6b02 721c  d.u.r.|.j.d.k.r.
-00003360: 710b 7c06 6a03 7d06 7404 4400 5d08 7d08  q.|.j.}.t.D.].}.
-00003370: 7c06 7c08 1900 7c07 7c08 3c00 7121 7405  |.|...|.|.<.q!t.
-00003380: 4400 5d24 7d09 6404 7c06 7600 7250 7406  D.]$}.d.|.v.rPt.
-00003390: 7c06 6404 1900 8301 6405 6b04 7250 7c09  |.d.....d.k.rP|.
-000033a0: a007 6406 a101 7241 7c09 6e04 6407 7c09  ..d...rA|.n.d.|.
-000033b0: 9b00 9d02 7d0a 7c06 6404 1900 6405 1900  ....}.|.d...d...
-000033c0: 7c09 1900 7c07 7c0a 3c00 712c 7c06 6408  |...|.|.<.q,|.d.
-000033d0: 1900 6403 6b02 7258 710b 7408 7c06 8301  ..d.k.rXq.t.|...
-000033e0: 7d0b 7c06 6409 1900 7c0b 6602 7c05 7601  }.|.d...|.f.|.v.
-000033f0: 7275 7c07 7c0b 0500 1900 640a 3700 0300  ru|.|.....d.7...
-00003400: 3c00 7c05 a009 7c06 6409 1900 7c0b 6602  <.|...|.d...|.f.
-00003410: a101 0100 7c0b 7c03 7600 7292 7c06 6409  ....|.|.v.r.|.d.
-00003420: 1900 640b 6602 7c05 7601 7292 7c07 640b  ..d.f.|.v.r.|.d.
-00003430: 0500 1900 640a 3700 0300 3c00 7c05 a009  ....d.7...<.|...
-00003440: 7c06 6409 1900 640b 6602 a101 0100 7c04  |.d...d.f.....|.
-00003450: a00a 7c07 a101 0100 710b 7c04 5300 290c  ..|.....q.|.S.).
-00003460: 4e3e 0300 0000 da05 7374 796c 655a 096e  N>......styleZ.n
-00003470: 6172 7261 7469 7665 5a05 6875 6d6f 7246  arrativeZ.humorF
-00003480: da07 4e65 7574 7261 6c72 9900 0000 7201  ..Neutralr....r.
-00003490: 0000 0072 9a00 0000 729b 0000 0072 1200  ...r....r....r..
-000034a0: 0000 da0b 6d61 7463 685f 696e 6465 7872  ....match_indexr
-000034b0: 4300 0000 7213 0000 0029 0b72 3200 0000  C...r....).r2...
-000034c0: 72a2 0000 0072 1200 0000 da04 6a73 6f6e  r....r......json
-000034d0: 720d 0000 0072 0e00 0000 7297 0000 0072  r....r....r....r
-000034e0: 9d00 0000 7218 0000 0072 4f00 0000 724c  ....r....rO...rL
-000034f0: 0000 0029 0c72 3900 0000 728f 0000 0072  ...).r9...r....r
-00003500: 6400 0000 5a10 706f 7369 7469 7665 5f73  d...Z.positive_s
-00003510: 7562 5f63 6174 7269 0000 005a 0763 6f75  ub_catri...Z.cou
-00003520: 6e74 6564 7215 0000 0072 9e00 0000 729f  ntedr....r....r.
-00003530: 0000 0072 a000 0000 72a1 0000 0072 1200  ...r....r....r..
-00003540: 0000 7216 0000 0072 1600 0000 7217 0000  ..r....r....r...
-00003550: 0072 6700 0000 a701 0000 7336 0000 0008  .rg.......s6....
-00003560: 0204 0106 0108 010a 0112 0102 0106 0108  ................
-00003570: 010e 0108 0118 0118 0114 0102 800c 0102  ................
-00003580: 0108 0110 0110 0112 0108 0110 0110 0112  ................
-00003590: 010c 0104 017a 2349 6d70 6163 744d 6174  .....z#ImpactMat
-000035a0: 6368 6572 2e63 6f6d 7075 7465 5f72 6576  cher.compute_rev
-000035b0: 6965 775f 696d 7061 6374 2903 7227 0000  iew_impact).r'..
-000035c0: 004e 4672 4700 0000 2902 4e46 2901 5429  .NFrG...).NF).T)
-000035d0: 0272 7500 0000 5429 0146 2926 da08 5f5f  .ru...T).F)&..__
-000035e0: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-000035f0: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-00003600: 724e 0000 0072 0700 0000 da04 626f 6f6c  rN...r......bool
-00003610: 723a 0000 0072 0800 0000 7246 0000 0072  r:...r....rF...r
-00003620: 3800 0000 724b 0000 0072 0b00 0000 7250  8...rK...r....rP
-00003630: 0000 0072 3400 0000 7203 0000 00da 0361  ...r4...r......a
-00003640: 6e79 725a 0000 0072 5c00 0000 725e 0000  nyrZ...r\...r^..
-00003650: 0072 6000 0000 7263 0000 0072 0400 0000  .r`...rc...r....
-00003660: 726a 0000 0072 6d00 0000 7271 0000 0072  rj...rm...rq...r
-00003670: 7400 0000 727e 0000 0072 7f00 0000 7265  t...r~...r....re
-00003680: 0000 0072 0900 0000 7280 0000 0072 8400  ...r....r....r..
-00003690: 0000 7285 0000 0072 8b00 0000 7293 0000  ..r....r....r...
-000036a0: 0072 9400 0000 72a2 0000 0072 6700 0000  .r....r....rg...
-000036b0: 7216 0000 0072 1600 0000 7216 0000 0072  r....r....r....r
-000036c0: 1700 0000 7226 0000 0037 0000 0073 4a00  ....r&...7...sJ.
-000036d0: 0000 0800 1802 161e 0812 0807 0e0b 2211  ..............".
-000036e0: 1a08 080b 1a07 140b 0205 0201 0cff 0201  ................
-000036f0: 02ff 0e01 0aff 0a0a 0a0b 0a0b 0a1c 0818  ................
-00003700: 0805 1804 120d 0e13 1217 161e 161b 1a14  ................
-00003710: 0211 0cff 0201 02ff 0e01 0eff 7226 0000  ............r&..
-00003720: 0029 1a72 2200 0000 da0b 636f 6c6c 6563  .).r".....collec
-00003730: 7469 6f6e 7372 0200 0000 da06 7479 7069  tionsr......typi
-00003740: 6e67 7203 0000 0072 0400 0000 7205 0000  ngr....r....r...
-00003750: 005a 0d6e 6c74 6b2e 746f 6b65 6e69 7a65  .Z.nltk.tokenize
-00003760: 7206 0000 005a 2172 6561 6469 6e67 5f69  r....Z!reading_i
-00003770: 6d70 6163 745f 6d6f 6465 6c2e 696d 7061  mpact_model.impa
-00003780: 6374 5f6d 6f64 656c 7207 0000 0072 0800  ct_modelr....r..
-00003790: 0000 7209 0000 0072 0a00 0000 720b 0000  ..r....r....r...
-000037a0: 0072 0c00 0000 720d 0000 0072 0e00 0000  .r....r....r....
-000037b0: 720f 0000 0072 1000 0000 7211 0000 0072  r....r....r....r
-000037c0: 1800 0000 721d 0000 0072 2100 0000 7225  ....r....r!...r%
-000037d0: 0000 0072 2600 0000 7216 0000 0072 1600  ...r&...r....r..
-000037e0: 0000 7216 0000 0072 1700 0000 da08 3c6d  ..r....r......<m
-000037f0: 6f64 756c 653e 0100 0000 731a 0000 0008  odule>....s.....
-00003800: 000c 0114 010c 021c 0214 010c 0110 0108  ................
-00003810: 0308 0708 0f08 0f12 05                   .........
+00000680: 6602 6413 6414 8404 5a0c 6415 650d 6503  f.d.d...Z.d.e.e.
+00000690: 650e 6602 1900 6416 650f 6417 6503 6418  e.f...d.e.d.e.d.
+000006a0: 6402 6608 6419 641a 8404 5a10 6415 6503  d.f.d.d...Z.d.e.
+000006b0: 6416 650f 6417 6503 6418 6402 6608 641b  d.e.d.e.d.d.f.d.
+000006c0: 641c 8404 5a11 641d 641e 8400 5a12 644a  d...Z.d.d...Z.dJ
+000006d0: 6415 6503 6416 650f 6417 6503 6418 6402  d.e.d.e.d.e.d.d.
+000006e0: 6608 641f 6420 8405 5a13 644b 6421 6503  f.d.d ..Z.dKd!e.
+000006f0: 6417 6503 6604 6422 6423 8405 5a14 0902  d.e.f.d"d#..Z...
+00000700: 0903 644c 6421 6503 6417 6503 6424 6505  ..dLd!e.d.e.d$e.
+00000710: 6418 6515 650d 6503 650e 6602 1900 1900  d.e.e.e.e.f.....
+00000720: 6608 6425 6426 8405 5a16 644d 6428 6429  f.d%d&..Z.dMd(d)
+00000730: 8401 5a17 644d 642a 642b 8401 5a18 644d  ..Z.dMd*d+..Z.dM
+00000740: 642c 642d 8401 5a19 644e 642f 6430 8401  d,d-..Z.dNd/d0..
+00000750: 5a1a 6431 6432 8400 5a1b 6433 6434 8400  Z.d1d2..Z.d3d4..
+00000760: 5a1c 0902 0902 644f 6435 6507 6416 650f  Z.....dOd5e.d.e.
+00000770: 6417 6503 6418 6515 651d 1900 6608 6436  d.e.d.e.e...f.d6
+00000780: 6437 8405 5a1e 6418 6515 651d 1900 6602  d7..Z.d.e.e...f.
+00000790: 6438 6439 8404 5a1f 6435 6507 6602 643a  d8d9..Z.d5e.f.d:
+000007a0: 643b 8404 5a20 6435 6507 643c 651d 6604  d;..Z d5e.d<e.f.
+000007b0: 643d 643e 8404 5a21 6435 6507 643c 651d  d=d>..Z!d5e.d<e.
+000007c0: 6418 6505 6606 643f 6440 8404 5a22 6435  d.e.f.d?d@..Z"d5
+000007d0: 6507 643c 651d 6418 6505 6606 6441 6442  e.d<e.d.e.f.dAdB
+000007e0: 8404 5a23 6443 651d 6418 650d 6503 650f  ..Z#dCe.d.e.e.e.
+000007f0: 6602 1900 6604 6444 6445 8404 5a24 0903  f...f.dDdE..Z$..
+00000800: 6450 6446 6515 651d 1900 6424 6505 6418  dPdFe.e...d$e.d.
+00000810: 6515 650d 6503 650e 6602 1900 1900 6606  e.e.e.e.f.....f.
+00000820: 6447 6448 8405 5a25 6402 5300 2951 da0d  dGdH..Z%d.S.)Q..
+00000830: 496d 7061 6374 4d61 7463 6865 72da 0265  ImpactMatcher..e
+00000840: 6e4e 46da 046c 616e 67da 0c69 6d70 6163  nNF..lang..impac
+00000850: 745f 6d6f 6465 6cda 0564 6562 7567 6304  t_model..debugc.
+00000860: 0000 0000 0000 0000 0000 0004 0000 0003  ................
+00000870: 0000 0043 0000 0073 8e00 0000 7c01 7c00  ...C...s....|.|.
+00000880: 5f00 7c01 6401 7501 720e 7401 7c01 6402  _.|.d.u.r.t.|.d.
+00000890: 8d01 7c00 5f02 6e0d 7403 7c02 7404 8302  ..|._.n.t.|.t...
+000008a0: 7217 7c02 7c00 5f02 6e04 7405 6403 8301  r.|.|._.n.t.d...
+000008b0: 8201 7c03 7c00 5f06 6404 7c00 5f07 6700  ..|.|._.d.|._.g.
+000008c0: 7c00 5f08 6401 7c00 5f09 6401 7c00 5f0a  |._.d.|._.d.|._.
+000008d0: 740b 740c 8301 7c00 5f0d 740c 8300 7c00  t.t...|._.t...|.
+000008e0: 5f0e 740c 8300 7c00 5f0f 740b 7410 8301  _.t...|._.t.t...
+000008f0: 7c00 5f11 740b 7412 8301 7c00 5f13 7c00  |._.t.t...|._.|.
+00000900: a014 a100 0100 6401 5300 2905 61ee 0100  ......d.S.).a...
+00000910: 0043 7265 6174 6520 6120 7265 6164 696e  .Create a readin
+00000920: 6720 696d 7061 6374 206d 6174 6368 6572  g impact matcher
+00000930: 206f 626a 6563 7420 666f 7220 6120 6769   object for a gi
+00000940: 7665 6e20 7265 6164 696e 6720 696d 7061  ven reading impa
+00000950: 6374 206d 6f64 656c 206f 7220 6c61 6e67  ct model or lang
+00000960: 7561 6765 2e0a 0a20 2020 2020 2020 2049  uage...        I
+00000970: 6620 6f6e 6c79 2061 206c 616e 6775 6167  f only a languag
+00000980: 6520 6964 656e 7469 6669 6572 2028 2765  e identifier ('e
+00000990: 6e27 206f 7220 276e 6c27 2920 6973 2070  n' or 'nl') is p
+000009a0: 6173 7365 642c 2074 6865 2064 6566 6175  assed, the defau
+000009b0: 6c74 206d 6f64 656c 2066 6f72 2074 6861  lt model for tha
+000009c0: 740a 2020 2020 2020 2020 6c61 6e67 7561  t.        langua
+000009d0: 6765 2077 696c 6c20 6265 2075 7365 642e  ge will be used.
+000009e0: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+000009f0: 206c 616e 673a 2074 6865 206c 616e 6775   lang: the langu
+00000a00: 6167 6520 666f 7220 7768 6963 6820 6120  age for which a 
+00000a10: 7265 6164 696e 6720 696d 7061 6374 206d  reading impact m
+00000a20: 6f64 656c 2073 686f 756c 6420 6265 2075  odel should be u
+00000a30: 7365 6420 2864 6566 6175 6c74 2027 656e  sed (default 'en
+00000a40: 272c 2077 6869 6368 2069 7320 456e 676c  ', which is Engl
+00000a50: 6973 6829 2e0a 2020 2020 2020 2020 3a74  ish)..        :t
+00000a60: 7970 6520 6c61 6e67 3a20 7374 720a 2020  ype lang: str.  
+00000a70: 2020 2020 2020 3a70 6172 616d 2069 6d70        :param imp
+00000a80: 6163 745f 6d6f 6465 6c3a 2061 2073 7065  act_model: a spe
+00000a90: 6369 6669 6320 696d 7061 6374 206d 6f64  cific impact mod
+00000aa0: 656c 2c20 6966 2079 6f75 2077 616e 7420  el, if you want 
+00000ab0: 746f 206f 7665 7272 6964 6520 7468 6520  to override the 
+00000ac0: 6465 6661 756c 7420 6d6f 6465 6c2e 0a20  default model.. 
+00000ad0: 2020 2020 2020 203a 7479 7065 2069 6d70         :type imp
+00000ae0: 6163 745f 6d6f 6465 6c3a 2049 6d70 6163  act_model: Impac
+00000af0: 744d 6f64 656c 0a20 2020 2020 2020 204e  tModel.        N
+00000b00: 2901 722a 0000 007a 374d 6174 6368 6572  ).r*...z7Matcher
+00000b10: 206d 7573 7420 6265 2069 6e73 7461 6e74   must be instant
+00000b20: 6961 7465 6420 7769 7468 2061 6e20 496d  iated with an Im
+00000b30: 7061 6374 4d6f 6465 6c20 6f62 6a65 6374  pactModel object
+00000b40: da00 2915 722a 0000 0072 0f00 0000 722b  ..).r*...r....r+
+00000b50: 0000 00da 0a69 7369 6e73 7461 6e63 6572  .....isinstancer
+00000b60: 0700 0000 da09 5479 7065 4572 726f 7272  ......TypeErrorr
+00000b70: 2c00 0000 da0f 7365 6e74 656e 6365 5f73  ,.....sentence_s
+00000b80: 7472 696e 67da 0f73 656e 7465 6e63 655f  tring..sentence_
+00000b90: 746f 6b65 6e73 da06 646f 635f 6964 da0e  tokens..doc_id..
+00000ba0: 7365 6e74 656e 6365 5f69 6e64 6578 7202  sentence_indexr.
+00000bb0: 0000 00da 0373 6574 da14 7365 6e74 656e  .....set..senten
+00000bc0: 6365 5f76 6f63 6162 5f74 6572 6d73 5a15  ce_vocab_termsZ.
+00000bd0: 7365 6e74 656e 6365 5f69 6d70 6163 745f  sentence_impact_
+00000be0: 7465 726d 735a 1573 656e 7465 6e63 655f  termsZ.sentence_
+00000bf0: 6173 7065 6374 5f74 6572 6d73 da03 696e  aspect_terms..in
+00000c00: 74da 0f63 616e 6469 6461 7465 5f72 756c  t..candidate_rul
+00000c10: 6573 da04 6c69 7374 da16 696d 7061 6374  es..list..impact
+00000c20: 5f72 756c 655f 7465 726d 5f69 6e64 6578  _rule_term_index
+00000c30: da18 5f69 6e64 6578 5f69 6d70 6163 745f  .._index_impact_
+00000c40: 7275 6c65 5f77 6f72 6473 2904 da04 7365  rule_words)...se
+00000c50: 6c66 722a 0000 0072 2b00 0000 722c 0000  lfr*...r+...r,..
+00000c60: 0072 1700 0000 7217 0000 0072 1800 0000  .r....r....r....
+00000c70: da08 5f5f 696e 6974 5f5f 3900 0000 7322  ..__init__9...s"
+00000c80: 0000 0006 0b08 010e 010a 0108 0108 0206  ................
+00000c90: 0106 0106 0106 0106 010a 0108 0108 010a  ................
+00000ca0: 010a 010c 017a 1649 6d70 6163 744d 6174  .....z.ImpactMat
+00000cb0: 6368 6572 2e5f 5f69 6e69 745f 5f72 2600  cher.__init__r&.
+00000cc0: 0000 da04 7275 6c65 da09 7465 726d 5f74  ....rule..term_t
+00000cd0: 7970 6563 0400 0000 0000 0000 0000 0000  ypec............
+00000ce0: 0700 0000 0800 0000 4300 0000 73d6 0000  ........C...s...
+00000cf0: 007c 0364 016b 0272 107c 006a 007c 0105  .|.d.k.r.|.j.|..
+00000d00: 0019 007c 0267 0137 0003 003c 0064 0053  ...|.g.7...<.d.S
+00000d10: 007c 0364 026b 0273 187c 0364 036b 0272  .|.d.k.s.|.d.k.r
+00000d20: 697a 3d7c 01a0 01a1 00a0 0264 04a1 0144  iz=|.......d...D
+00000d30: 005d 327d 047c 0464 0519 0064 066b 0272  .]2}.|.d...d.k.r
+00000d40: 487c 0464 0719 0064 086b 0272 4874 03a0  H|.d...d.k.rHt..
+00000d50: 0264 097c 0464 0a64 0785 0219 00a1 027d  .d.|.d.d.......}
+00000d60: 057c 0544 005d 0c7d 067c 006a 007c 0605  .|.D.].}.|.j.|..
+00000d70: 0019 007c 0267 0137 0003 003c 0071 3a71  ...|.g.7...<.q:q
+00000d80: 207c 006a 007c 0405 0019 007c 0267 0137   |.j.|.....|.g.7
+00000d90: 0003 003c 0071 2057 0064 0053 0004 0074  ...<.q W.d.S...t
+00000da0: 0479 6801 0001 0001 0074 057c 0183 0101  .yh......t.|....
+00000db0: 0074 057c 01a0 0264 04a1 0183 0101 0082  .t.|...d........
+00000dc0: 0077 0064 0053 0029 0b4e 7222 0000 00da  .w.d.S.).Nr"....
+00000dd0: 0670 6872 6173 65da 0572 6567 6578 fa01  .phrase..regex..
+00000de0: 2072 0100 0000 fa01 28e9 ffff ffff fa01   r......(.......
+00000df0: 297a 045b 207c 5de9 0100 0000 2906 7239  )z.[ |].....).r9
+00000e00: 0000 00da 0573 7472 6970 da05 7370 6c69  .....strip..spli
+00000e10: 7472 2400 0000 721c 0000 0072 1d00 0000  tr$...r....r....
+00000e20: 2907 723b 0000 0072 2600 0000 723d 0000  ).r;...r&...r=..
+00000e30: 0072 3e00 0000 5a0b 7068 7261 7365 5f70  .r>...Z.phrase_p
+00000e40: 6172 745a 1170 6872 6173 655f 7061 7274  artZ.phrase_part
+00000e50: 5f74 6572 6d73 7222 0000 0072 1700 0000  _termsr"...r....
+00000e60: 7217 0000 0072 1800 0000 da19 5f69 6e64  r....r......_ind
+00000e70: 6578 5f69 6d70 6163 745f 7275 6c65 5f73  ex_impact_rule_s
+00000e80: 7472 696e 6757 0000 0073 2400 0000 0801  tringW...s$.....
+00000e90: 1801 1001 0201 1201 1801 1401 0802 1601  ................
+00000ea0: 02ff 1603 06f9 0c08 0801 0e01 0201 02fd  ................
+00000eb0: 04f6 7a27 496d 7061 6374 4d61 7463 6865  ..z'ImpactMatche
+00000ec0: 722e 5f69 6e64 6578 5f69 6d70 6163 745f  r._index_impact_
+00000ed0: 7275 6c65 5f73 7472 696e 6763 0100 0000  rule_stringc....
+00000ee0: 0000 0000 0000 0000 0200 0000 0600 0000  ................
+00000ef0: 4300 0000 7328 0000 007c 006a 006a 0144  C...s(...|.j.j.D
+00000f00: 005d 0d7d 017c 00a0 027c 016a 036a 047c  .].}.|...|.j.j.|
+00000f10: 017c 016a 036a 05a1 0301 0071 0464 0053  .|.j.j.....q.d.S
+00000f20: 00a9 014e 2906 722b 0000 00da 0c69 6d70  ...N).r+.....imp
+00000f30: 6163 745f 7275 6c65 7372 4800 0000 da0b  act_rulesrH.....
+00000f40: 696d 7061 6374 5f74 6572 6d72 2600 0000  impact_termr&...
+00000f50: da04 7479 7065 2902 723b 0000 0072 3d00  ..type).r;...r=.
+00000f60: 0000 7217 0000 0072 1700 0000 7218 0000  ..r....r....r...
+00000f70: 0072 3a00 0000 6900 0000 7306 0000 000c  .r:...i...s.....
+00000f80: 0118 0104 ff7a 2649 6d70 6163 744d 6174  .....z&ImpactMat
+00000f90: 6368 6572 2e5f 696e 6465 785f 696d 7061  cher._index_impa
+00000fa0: 6374 5f72 756c 655f 776f 7264 7363 0300  ct_rule_wordsc..
+00000fb0: 0000 0000 0000 0000 0000 0400 0000 0500  ................
+00000fc0: 0000 4300 0000 736c 0000 007c 017c 006a  ..C...sl...|.|.j
+00000fd0: 0076 0072 167c 006a 007c 0119 0044 005d  .v.r.|.j.|...D.]
+00000fe0: 0b7d 037c 006a 017c 0305 0019 0064 0137  .}.|.j.|.....d.7
+00000ff0: 0003 003c 0071 0a7c 027c 016b 0372 307c  ...<.q.|.|.k.r0|
+00001000: 027c 006a 0076 0072 327c 006a 007c 0219  .|.j.v.r2|.j.|..
+00001010: 0044 005d 0f7d 037c 006a 017c 0305 0019  .D.].}.|.j.|....
+00001020: 0064 0137 0003 003c 0071 2464 0053 0064  .d.7...<.q$d.S.d
+00001030: 0053 0064 0053 0029 024e 7245 0000 0029  .S.d.S.).NrE...)
+00001040: 0272 3900 0000 7237 0000 0029 0472 3b00  .r9...r7...).r;.
+00001050: 0000 da05 746f 6b65 6e72 2100 0000 723d  ....tokenr!...r=
+00001060: 0000 0072 1700 0000 7217 0000 0072 1800  ...r....r....r..
+00001070: 0000 da13 6164 645f 6361 6e64 6964 6174  ....add_candidat
+00001080: 655f 7275 6c65 7370 0000 0073 1000 0000  e_rulesp...s....
+00001090: 0a02 0e02 1402 1201 0e01 1401 08fe 0401  ................
+000010a0: 7a21 496d 7061 6374 4d61 7463 6865 722e  z!ImpactMatcher.
+000010b0: 6164 645f 6361 6e64 6964 6174 655f 7275  add_candidate_ru
+000010c0: 6c65 7372 4d00 0000 6302 0000 0000 0000  lesrM...c.......
+000010d0: 0000 0000 0004 0000 0004 0000 0043 0000  .............C..
+000010e0: 0073 c200 0000 7c00 6a00 a001 7c01 a101  .s....|.j...|...
+000010f0: 0100 7c00 6a02 a003 7c01 6a04 a101 7d02  ..|.j...|.j...}.
+00001100: 7405 7c02 7406 8302 721b 7c00 6a07 7c02  t.|.t...r.|.j.|.
+00001110: 1900 a008 7c01 a101 0100 6e12 7405 7c02  ....|.....n.t.|.
+00001120: 7409 8302 722d 7c02 4400 5d0a 7d03 7c00  t...r-|.D.].}.|.
+00001130: 6a07 7c03 1900 a008 7c01 a101 0100 7122  j.|.....|.....q"
+00001140: 7c01 6a0a 7c01 6a04 6b02 7235 6400 5300  |.j.|.j.k.r5d.S.
+00001150: 7c00 6a02 a003 7c01 6a0a a101 7d02 7405  |.j...|.j...}.t.
+00001160: 7c02 7406 8302 724b 7c00 6a07 7c02 1900  |.t...rK|.j.|...
+00001170: a008 7c01 a101 0100 6400 5300 7405 7c02  ..|.....d.S.t.|.
+00001180: 7409 8302 725d 7c02 4400 5d0c 7d03 7c00  t...r]|.D.].}.|.
+00001190: 6a07 7c03 1900 a008 7c01 a101 0100 7152  j.|.....|.....qR
+000011a0: 6400 5300 6400 5300 7249 0000 0029 0b72  d.S.d.S.rI...).r
+000011b0: 3100 0000 da06 6170 7065 6e64 722b 0000  1.....appendr+..
+000011c0: 00da 1767 6574 5f6d 6174 6368 696e 675f  ...get_matching_
+000011d0: 766f 6361 625f 7465 726d da04 776f 7264  vocab_term..word
+000011e0: 722e 0000 00da 0373 7472 7235 0000 00da  r......strr5....
+000011f0: 0361 6464 7234 0000 0072 2100 0000 2904  .addr4...r!...).
+00001200: 723b 0000 0072 4d00 0000 da0b 766f 6361  r;...rM.....voca
+00001210: 625f 7465 726d 73da 0a76 6f63 6162 5f74  b_terms..vocab_t
+00001220: 6572 6d72 1700 0000 7217 0000 0072 1800  ermr....r....r..
+00001230: 0000 da13 5f61 6464 5f73 656e 7465 6e63  ...._add_sentenc
+00001240: 655f 746f 6b65 6e7b 0000 0073 2200 0000  e_token{...s"...
+00001250: 0c01 0e01 0a01 1201 0a01 0801 1201 0c01  ................
+00001260: 0401 0e01 0a01 1401 0a01 0801 1201 04fe  ................
+00001270: 0401 7a21 496d 7061 6374 4d61 7463 6865  ..z!ImpactMatche
+00001280: 722e 5f61 6464 5f73 656e 7465 6e63 655f  r._add_sentence_
+00001290: 746f 6b65 6eda 0873 656e 7465 6e63 6572  token..sentencer
+000012a0: 3300 0000 7232 0000 00da 0672 6574 7572  3...r2.....retur
+000012b0: 6e63 0400 0000 0000 0000 0000 0000 0600  nc..............
+000012c0: 0000 0700 0000 4300 0000 737c 0000 007c  ......C...s|...|
+000012d0: 0164 0119 007c 005f 007c 027c 005f 017c  .d...|._.|.|._.|
+000012e0: 0272 107c 0372 107c 027c 0366 026e 0164  .r.|.r.|.|.f.n.d
+000012f0: 007c 005f 0274 037c 0164 0219 0083 0144  .|._.t.|.d.....D
+00001300: 005d 225c 027d 047d 0574 047c 056a 057c  .]"\.}.}.t.|.j.|
+00001310: 047c 056a 0664 037c 0576 0072 2a7c 056a  .|.j.d.|.v.r*|.j
+00001320: 076e 0164 0064 048d 047d 057c 00a0 087c  .n.d.d...}.|...|
+00001330: 05a1 0101 007c 00a0 097c 056a 057c 056a  .....|...|.j.|.j
+00001340: 06a1 0201 0071 1964 0053 0029 054e da04  .....q.d.S.).N..
+00001350: 7465 7874 da06 746f 6b65 6e73 da03 706f  text..tokens..po
+00001360: 7329 0472 5100 0000 da05 696e 6465 7872  s).rQ.....indexr
+00001370: 2100 0000 725b 0000 0029 0a72 3000 0000  !...r[...).r0...
+00001380: 7233 0000 00da 0b73 656e 7465 6e63 655f  r3.....sentence_
+00001390: 6964 da09 656e 756d 6572 6174 6572 0b00  id..enumerater..
+000013a0: 0000 7251 0000 0072 2100 0000 725b 0000  ..rQ...r!...r[..
+000013b0: 0072 5600 0000 724e 0000 0029 0672 3b00  .rV...rN...).r;.
+000013c0: 0000 7257 0000 0072 3300 0000 7232 0000  ..rW...r3...r2..
+000013d0: 005a 0274 6972 4d00 0000 7217 0000 0072  .Z.tirM...r....r
+000013e0: 1700 0000 7218 0000 00da 125f 7365 745f  ....r......_set_
+000013f0: 6469 6374 5f73 656e 7465 6e63 658c 0000  dict_sentence...
+00001400: 0073 1000 0000 0a01 0601 1601 1401 2201  .s............".
+00001410: 0a01 1201 04fd 7a20 496d 7061 6374 4d61  ......z ImpactMa
+00001420: 7463 6865 722e 5f73 6574 5f64 6963 745f  tcher._set_dict_
+00001430: 7365 6e74 656e 6365 6304 0000 0000 0000  sentencec.......
+00001440: 0000 0000 0008 0000 0006 0000 0043 0000  .............C..
+00001450: 0073 6800 0000 7c01 7c00 5f00 7c02 7c00  .sh...|.|._.|.|.
+00001460: 5f01 7c02 720e 7c03 720e 7c02 7c03 6602  _.|.r.|.r.|.|.f.
+00001470: 6e01 6400 7c00 5f02 7403 a004 6401 7c01  n.d.|._.t...d.|.
+00001480: a102 7d04 7405 7c04 8301 4400 5d16 5c02  ..}.t.|...D.].\.
+00001490: 7d05 7d06 7406 7c06 7c05 7c06 6402 8d03  }.}.t.|.|.|.d...
+000014a0: 7d07 7c00 a007 7c07 a101 0100 7c00 a008  }.|...|.....|...
+000014b0: 7c06 7c06 a102 0100 711b 6400 5300 2903  |.|.....q.d.S.).
+000014c0: 4e7a 035c 572b 2901 7221 0000 0029 0972  Nz.\W+).r!...).r
+000014d0: 3000 0000 7233 0000 0072 5d00 0000 7224  0...r3...r]...r$
+000014e0: 0000 0072 4700 0000 725e 0000 0072 0b00  ...rG...r^...r..
+000014f0: 0000 7256 0000 0072 4e00 0000 2908 723b  ..rV...rN...).r;
+00001500: 0000 0072 5700 0000 7233 0000 0072 3200  ...rW...r3...r2.
+00001510: 0000 da05 776f 7264 735a 0277 6972 5100  ....wordsZ.wirQ.
+00001520: 0000 724d 0000 0072 1700 0000 7217 0000  ..rM...r....r...
+00001530: 0072 1800 0000 da14 5f73 6574 5f73 7472  .r......_set_str
+00001540: 696e 675f 7365 6e74 656e 6365 9500 0000  ing_sentence....
+00001550: 7312 0000 0006 0106 0116 010c 0110 010e  s...............
+00001560: 010a 010e 0104 fd7a 2249 6d70 6163 744d  .......z"ImpactM
+00001570: 6174 6368 6572 2e5f 7365 745f 7374 7269  atcher._set_stri
+00001580: 6e67 5f73 656e 7465 6e63 6563 0100 0000  ng_sentencec....
+00001590: 0000 0000 0000 0000 0100 0000 0200 0000  ................
+000015a0: 4300 0000 732a 0000 0064 017c 005f 0067  C...s*...d.|._.g
+000015b0: 007c 005f 0174 0274 0383 017c 005f 0474  .|._.t.t...|._.t
+000015c0: 0274 0583 017c 005f 0664 007c 005f 0764  .t...|._.d.|._.d
+000015d0: 0053 0029 024e 722d 0000 0029 0872 3000  .S.).Nr-...).r0.
+000015e0: 0000 7231 0000 0072 0200 0000 7234 0000  ..r1...r....r4..
+000015f0: 0072 3500 0000 7236 0000 0072 3700 0000  .r5...r6...r7...
+00001600: 5a07 7365 6e74 5f69 64a9 0172 3b00 0000  Z.sent_id..r;...
+00001610: 7217 0000 0072 1700 0000 7218 0000 00da  r....r....r.....
+00001620: 0f5f 7265 7365 745f 7365 6e74 656e 6365  ._reset_sentence
+00001630: a100 0000 730a 0000 0006 0106 010a 010a  ....s...........
+00001640: 010a 017a 1d49 6d70 6163 744d 6174 6368  ...z.ImpactMatch
+00001650: 6572 2e5f 7265 7365 745f 7365 6e74 656e  er._reset_senten
+00001660: 6365 6304 0000 0000 0000 0000 0000 0004  cec.............
+00001670: 0000 0005 0000 0043 0000 0073 6200 0000  .......C...sb...
+00001680: 7c00 a000 a100 0100 7c03 7c00 5f01 7402  |.......|.|._.t.
+00001690: 7c01 7403 8302 721e 6401 7c01 7600 721e  |.t...r.d.|.v.r.
+000016a0: 6402 7c01 7600 721e 7c00 6a04 7c01 7c02  d.|.v.r.|.j.|.|.
+000016b0: 7c03 6403 8d03 0100 6400 5300 7402 7c01  |.d.....d.S.t.|.
+000016c0: 7405 8302 722d 7c00 6a06 7c01 7c02 7c03  t...r-|.j.|.|.|.
+000016d0: 6403 8d03 0100 6400 5300 7407 6404 8301  d.....d.S.t.d...
+000016e0: 8201 2905 4e72 5900 0000 725a 0000 00a9  ..).NrY...rZ....
+000016f0: 0272 3300 0000 7232 0000 007a 5273 656e  .r3...r2...zRsen
+00001700: 7465 6e63 6520 6d75 7374 2062 6520 6569  tence must be ei
+00001710: 7468 6572 2061 2073 7472 696e 672c 2061  ther a string, a
+00001720: 6e20 5365 6e74 656e 6365 206f 626a 6563  n Sentence objec
+00001730: 7420 6672 6f6d 2041 6c70 696e 6f2c 2053  t from Alpino, S
+00001740: 7061 6379 206f 7220 5374 616e 7a61 2e29  pacy or Stanza.)
+00001750: 0872 6300 0000 7232 0000 0072 2e00 0000  .rc...r2...r....
+00001760: da04 6469 6374 725f 0000 0072 5200 0000  ..dictr_...rR...
+00001770: 7261 0000 0072 2f00 0000 2904 723b 0000  ra...r/...).r;..
+00001780: 0072 5700 0000 7233 0000 0072 3200 0000  .rW...r3...r2...
+00001790: 7217 0000 0072 1700 0000 7218 0000 00da  r....r....r.....
+000017a0: 0d5f 7365 745f 7365 6e74 656e 6365 a800  ._set_sentence..
+000017b0: 0000 7312 0000 0008 0106 011a 0114 010a  ..s.............
+000017c0: 0114 0102 0202 0104 ff7a 1b49 6d70 6163  .........z.Impac
+000017d0: 744d 6174 6368 6572 2e5f 7365 745f 7365  tMatcher._set_se
+000017e0: 6e74 656e 6365 7259 0000 0063 0300 0000  ntencerY...c....
+000017f0: 0000 0000 0000 0000 0500 0000 0600 0000  ................
+00001800: 6300 0000 734e 0000 0081 0074 0074 017c  c...sN.....t.t.|
+00001810: 0183 0183 0144 005d 1d5c 027d 037d 047c  .....D.].\.}.}.|
+00001820: 006a 027c 047c 037c 0264 018d 0301 007c  .j.|.|.|.d.....|
+00001830: 006a 0372 2174 0464 027c 0383 0201 0074  .j.r!t.d.|.....t
+00001840: 0464 037c 006a 0583 0201 007c 0356 0001  .d.|.j.....|.V..
+00001850: 0071 0764 0053 0029 044e 7264 0000 007a  .q.d.S.).Nrd...z
+00001860: 195f 6974 6572 5f74 6578 745f 7365 6e74  ._iter_text_sent
+00001870: 656e 6365 202d 2073 693a 7a2a 5f69 7465  ence - si:z*_ite
+00001880: 725f 7465 7874 5f73 656e 7465 6e63 6520  r_text_sentence 
+00001890: 2d20 7365 6c66 2e73 656e 7465 6e63 655f  - self.sentence_
+000018a0: 696e 6465 783a 2906 725e 0000 0072 0600  index:).r^...r..
+000018b0: 0000 7266 0000 0072 2c00 0000 721d 0000  ..rf...r,...r...
+000018c0: 0072 3300 0000 2905 723b 0000 0072 5900  .r3...).r;...rY.
+000018d0: 0000 7232 0000 00da 0273 69da 0473 656e  ..r2.....si..sen
+000018e0: 7472 1700 0000 7217 0000 0072 1800 0000  tr....r....r....
+000018f0: da14 5f69 7465 725f 7465 7874 5f73 656e  .._iter_text_sen
+00001900: 7465 6e63 6573 b300 0000 7310 0000 0002  tences....s.....
+00001910: 8014 0110 0106 010a 010c 0108 0104 fb7a  ...............z
+00001920: 2249 6d70 6163 744d 6174 6368 6572 2e5f  "ImpactMatcher._
+00001930: 6974 6572 5f74 6578 745f 7365 6e74 656e  iter_text_senten
+00001940: 6365 73da 0f69 6e63 6c75 6465 5f6e 6575  ces..include_neu
+00001950: 7472 616c 6304 0000 0000 0000 0000 0000  tralc...........
+00001960: 0008 0000 0004 0000 0043 0000 0073 3a00  .........C...s:.
+00001970: 0000 6700 7d04 7c00 a000 7c01 7c02 a102  ..g.}.|...|.|...
+00001980: 4400 5d0b 7d05 7c00 a001 a100 7d06 7c04  D.].}.|.....}.|.
+00001990: a002 7c06 a101 0100 7108 7c00 6a03 7c04  ..|.....q.|.j.|.
+000019a0: 7c03 6401 8d02 7d07 7c07 5300 2902 4e29  |.d...}.|.S.).N)
+000019b0: 0172 6a00 0000 2904 7269 0000 00da 0c5f  .rj...).ri....._
+000019c0: 6d61 7463 685f 7275 6c65 73da 0665 7874  match_rules..ext
+000019d0: 656e 64da 1563 6f6d 7075 7465 5f72 6576  end..compute_rev
+000019e0: 6965 775f 696d 7061 6374 2908 723b 0000  iew_impact).r;..
+000019f0: 0072 5900 0000 7232 0000 0072 6a00 0000  .rY...r2...rj...
+00001a00: 5a0b 616c 6c5f 6d61 7463 6865 73da 015f  Z.all_matches.._
+00001a10: 5a10 7365 6e74 656e 6365 5f6d 6174 6368  Z.sentence_match
+00001a20: 6573 da0d 7265 7669 6577 5f69 6d70 6163  es..review_impac
+00001a30: 7472 1700 0000 7217 0000 0072 1800 0000  tr....r....r....
+00001a40: da0c 616e 616c 7973 655f 7465 7874 bb00  ..analyse_text..
+00001a50: 0000 7310 0000 0004 0210 0108 010c 0106  ..s.............
+00001a60: 0102 0106 ff04 027a 1a49 6d70 6163 744d  .......z.ImpactM
+00001a70: 6174 6368 6572 2e61 6e61 6c79 7365 5f74  atcher.analyse_t
+00001a80: 6578 7454 6303 0000 0000 0000 0000 0000  extTc...........
+00001a90: 0003 0000 0004 0000 0043 0000 0073 2400  .........C...s$.
+00001aa0: 0000 7c02 720d 7400 a001 6401 7c01 1700  ..|.r.t...d.|...
+00001ab0: 6401 1700 7c00 6a02 a102 5300 7c01 7c00  d...|.j...S.|.|.
+00001ac0: 6a02 7600 5300 2902 7aa5 0a20 2020 2020  j.v.S.).z..     
+00001ad0: 2020 2063 6865 636b 2069 6620 7465 726d     check if term
+00001ae0: 206f 6363 7572 7320 696e 2073 656e 7465   occurs in sente
+00001af0: 6e63 6520 7374 7269 6e67 2e0a 2020 2020  nce string..    
+00001b00: 2020 2020 4173 7375 6d65 7320 776f 7264      Assumes word
+00001b10: 2062 6f75 6e64 6172 6965 7320 0874 6572   boundaries .ter
+00001b20: 6d08 2062 7920 6465 6661 756c 742e 0a20  m. by default.. 
+00001b30: 2020 2020 2020 2055 7365 2077 6f72 645f         Use word_
+00001b40: 626f 756e 6461 7269 6573 3d46 616c 7365  boundaries=False
+00001b50: 2066 6f72 2070 7572 6520 7374 7269 6e67   for pure string
+00001b60: 206d 6174 6368 0a20 2020 2020 2020 20fa   match.        .
+00001b70: 025c 6229 0372 2400 0000 da06 7365 6172  .\b).r$.....sear
+00001b80: 6368 7230 0000 0029 0372 3b00 0000 7222  chr0...).r;...r"
+00001b90: 0000 005a 0f77 6f72 645f 626f 756e 6461  ...Z.word_bounda
+00001ba0: 7269 6573 7217 0000 0072 1700 0000 7218  riesr....r....r.
+00001bb0: 0000 00da 1374 6572 6d5f 7365 6e74 656e  .....term_senten
+00001bc0: 6365 5f6d 6174 6368 c500 0000 7306 0000  ce_match....s...
+00001bd0: 0004 0616 010a 027a 2149 6d70 6163 744d  .......z!ImpactM
+00001be0: 6174 6368 6572 2e74 6572 6d5f 7365 6e74  atcher.term_sent
+00001bf0: 656e 6365 5f6d 6174 6368 6303 0000 0000  ence_matchc.....
+00001c00: 0000 0000 0000 0006 0000 0004 0000 0063  ...............c
+00001c10: 0000 0073 5600 0000 8100 7c01 7c00 6a00  ...sV.....|.|.j.
+00001c20: 7600 720b 7c00 6a00 7c01 1900 6e01 6700  v.r.|.j.|...n.g.
+00001c30: 7d03 7c03 4400 5d19 7d04 7c02 721d 7c04  }.|.D.].}.|.r.|.
+00001c40: 6a01 a002 a100 7d05 7c01 a002 a100 7d01  j.....}.|.....}.
+00001c50: 6e03 7c04 6a01 7d05 7403 7c05 7c01 8302  n.|.j.}.t.|.|...
+00001c60: 7228 7c04 5600 0100 710f 6400 5300 7249  r(|.V...q.d.S.rI
+00001c70: 0000 0029 0472 3500 0000 7251 0000 0072  ...).r5...rQ...r
+00001c80: 1500 0000 721f 0000 0029 0672 3b00 0000  ....r....).r;...
+00001c90: da0a 6d61 7463 685f 7465 726d da0a 6967  ..match_term..ig
+00001ca0: 6e6f 7265 6361 7365 da0c 6d61 7463 685f  norecase..match_
+00001cb0: 746f 6b65 6e73 724d 0000 0072 5100 0000  tokensrM...rQ...
+00001cc0: 7217 0000 0072 1700 0000 7218 0000 00da  r....r....r.....
+00001cd0: 2067 6574 5f73 656e 7465 6e63 655f 776f   get_sentence_wo
+00001ce0: 7264 735f 6d61 7463 6869 6e67 5f74 6572  rds_matching_ter
+00001cf0: 6dd0 0000 0073 1600 0000 0280 1801 0801  m....s..........
+00001d00: 0401 0a01 0a01 0602 0a01 0601 0280 04f9  ................
+00001d10: 7a2e 496d 7061 6374 4d61 7463 6865 722e  z.ImpactMatcher.
+00001d20: 6765 745f 7365 6e74 656e 6365 5f77 6f72  get_sentence_wor
+00001d30: 6473 5f6d 6174 6368 696e 675f 7465 726d  ds_matching_term
+00001d40: 6304 0000 0000 0000 0000 0000 0008 0000  c...............
+00001d50: 0006 0000 0063 0000 0073 fc00 0000 8100  .....c...s......
+00001d60: 7c00 6a00 7216 7401 6401 7c01 7c02 8303  |.j.r.t.d.|.|...
+00001d70: 0100 7401 7c00 6a02 8301 0100 7401 7c01  ..t.|.j.....t.|.
+00001d80: 7c00 6a02 7600 8301 0100 7c01 7c00 6a02  |.j.v.....|.|.j.
+00001d90: 7600 7220 7c00 6a02 7c01 1900 6e01 6700  v.r |.j.|...n.g.
+00001da0: 7d04 7c04 4400 5d57 7d05 7c03 7237 7c05  }.|.D.]W}.|.r7|.
+00001db0: 6a03 a004 a100 7d06 7c05 6a05 a004 a100  j.....}.|.j.....
+00001dc0: 7d07 7c01 a004 a100 7d01 6e06 7c05 6a03  }.|.....}.n.|.j.
+00001dd0: 7d06 7c05 6a05 7d07 7c00 6a00 7249 7401  }.|.j.}.|.j.rIt.
+00001de0: 6402 7c05 6a03 6403 7c05 6a06 8304 0100  d.|.j.d.|.j.....
+00001df0: 7407 7c06 7c01 8302 7354 7407 7c07 7c01  t.|.|...sTt.|.|.
+00001e00: 8302 7354 7124 7c02 7263 7c05 6a06 7263  ..sTq$|.rc|.j.rc
+00001e10: 7c05 6a06 7c02 6b02 7363 7c05 6a06 6404  |.j.|.k.sc|.j.d.
+00001e20: 6b02 726e 7c00 6a00 726a 7401 6405 8301  k.rn|.j.rjt.d...
+00001e30: 0100 7c05 5600 0100 7124 7c00 6a00 727b  ..|.V...q$|.j.r{
+00001e40: 7401 6406 8301 0100 7401 7c05 6407 1900  t.d.....t.|.d...
+00001e50: 8301 0100 7124 6400 5300 2908 4e7a 216c  ....q$d.S.).Nz!l
+00001e60: 6f6f 6b69 6e67 2066 6f72 206c 656d 6d61  ooking for lemma
+00001e70: 7320 6d61 7463 6869 6e67 2074 6572 6d3a  s matching term:
+00001e80: 7a07 096c 656d 6d61 3a7a 0470 6f73 3ada  z..lemma:z.pos:.
+00001e90: 046e 616d 657a 174d 4154 4348 204f 4620  .namez.MATCH OF 
+00001ea0: 4c45 4d4d 4120 414e 4420 504f 5321 7a1e  LEMMA AND POS!z.
+00001eb0: 4d41 5443 4820 4f46 204c 454d 4d41 2042  MATCH OF LEMMA B
+00001ec0: 5554 204e 4f54 204f 4620 504f 5321 725b  UT NOT OF POS!r[
+00001ed0: 0000 0029 0872 2c00 0000 721d 0000 0072  ...).r,...r....r
+00001ee0: 3500 0000 7221 0000 0072 1500 0000 7251  5...r!...r....rQ
+00001ef0: 0000 0072 5b00 0000 721f 0000 0029 0872  ...r[...r....).r
+00001f00: 3b00 0000 7274 0000 00da 096d 6174 6368  ;...rt.....match
+00001f10: 5f70 6f73 7275 0000 0072 7600 0000 724d  _posru...rv...rM
+00001f20: 0000 0072 2100 0000 7251 0000 0072 1700  ...r!...rQ...r..
+00001f30: 0000 7217 0000 0072 1800 0000 da21 6765  ..r....r.....!ge
+00001f40: 745f 7365 6e74 656e 6365 5f6c 656d 6d61  t_sentence_lemma
+00001f50: 735f 6d61 7463 6869 6e67 5f74 6572 6ddb  s_matching_term.
+00001f60: 0000 0073 3400 0000 0280 0601 0c01 0a01  ...s4...........
+00001f70: 0e01 1801 0801 0401 0a01 0a01 0a01 0602  ................
+00001f80: 0601 0601 1201 1403 0201 1e01 0601 0801  ................
+00001f90: 0801 0601 0801 0c01 0280 04ec 7a2f 496d  ............z/Im
+00001fa0: 7061 6374 4d61 7463 6865 722e 6765 745f  pactMatcher.get_
+00001fb0: 7365 6e74 656e 6365 5f6c 656d 6d61 735f  sentence_lemmas_
+00001fc0: 6d61 7463 6869 6e67 5f74 6572 6dda 0d6e  matching_term..n
+00001fd0: 6569 6768 626f 7572 686f 6f64 6304 0000  eighbourhoodc...
+00001fe0: 0000 0000 0000 0000 0007 0000 0008 0000  ................
+00001ff0: 0063 0000 0073 c400 0000 8100 7c00 6a00  .c...s......|.j.
+00002000: 720b 7401 6401 7c01 6402 7c02 8304 0100  r.t.d.|.d.|.....
+00002010: 7c00 6a02 7d04 7c03 7218 7c04 a003 a100  |.j.}.|.r.|.....
+00002020: 7d04 7c01 a003 a100 7d01 7c00 6a00 7220  }.|.....}.|.j.r 
+00002030: 7401 6403 7c04 8302 0100 6404 7c01 1700  t.d.|.....d.|...
+00002040: 6404 1700 7d05 7c02 6405 6b02 7237 6406  d...}.|.d.k.r7d.
+00002050: 7c05 1700 7d05 7c00 6a00 7236 7401 6407  |...}.|.j.r6t.d.
+00002060: 7c05 8302 0100 6e08 7c02 6408 6b02 723f  |.....n.|.d.k.r?
+00002070: 7c05 6409 1700 7d05 7a0f 7404 a005 7c05  |.d...}.z.t...|.
+00002080: 7c04 a102 4400 5d05 7d06 7c06 5600 0100  |...D.].}.|.V...
+00002090: 7146 5700 6400 5300 0400 7404 6a06 7961  qFW.d.S...t.j.ya
+000020a0: 0100 0100 0100 7401 640a 7c05 8302 0100  ......t.d.|.....
+000020b0: 7401 6403 7c04 8302 0100 8200 7700 290b  t.d.|.......w.).
+000020c0: 4e7a 2c6c 6f6f 6b69 6e67 2066 6f72 2073  Nz,looking for s
+000020d0: 656e 7465 6e63 6520 7374 7269 6e67 206d  entence string m
+000020e0: 6174 6368 696e 6720 7068 7261 7365 3a7a  atching phrase:z
+000020f0: 0c61 6e64 206c 6f63 6174 696f 6efa 0973  .and location..s
+00002100: 656e 7465 6e63 653a 7271 0000 00da 0e73  entence:rq.....s
+00002110: 656e 7465 6e63 655f 7374 6172 74fa 015e  entence_start..^
+00002120: da0c 6d61 7463 685f 7374 7269 6e67 da0c  ..match_string..
+00002130: 7365 6e74 656e 6365 5f65 6e64 fa01 247a  sentence_end..$z
+00002140: 0d6d 6174 6368 5f73 7472 696e 673a 2907  .match_string:).
+00002150: 722c 0000 0072 1d00 0000 7230 0000 0072  r,...r....r0...r
+00002160: 1500 0000 7224 0000 00da 0866 696e 6469  ....r$.....findi
+00002170: 7465 72da 0565 7272 6f72 2907 723b 0000  ter..error).r;..
+00002180: 0072 7400 0000 da08 6c6f 6361 7469 6f6e  .rt.....location
+00002190: 7275 0000 0072 5700 0000 727f 0000 0072  ru...rW...r....r
+000021a0: 1600 0000 7217 0000 0072 1700 0000 7218  ....r....r....r.
+000021b0: 0000 00da 2167 6574 5f73 656e 7465 6e63  ....!get_sentenc
+000021c0: 655f 7374 7269 6e67 5f6d 6174 6368 696e  e_string_matchin
+000021d0: 675f 7465 726d f700 0000 7334 0000 0002  g_term....s4....
+000021e0: 8006 010e 0106 0104 0108 0108 0106 010a  ................
+000021f0: 010c 0108 0108 0106 010a 0102 8008 0108  ................
+00002200: 0102 0110 0108 0106 ff0e 020a 010a 0102  ................
+00002210: 0102 fd7a 2f49 6d70 6163 744d 6174 6368  ...z/ImpactMatch
+00002220: 6572 2e67 6574 5f73 656e 7465 6e63 655f  er.get_sentence_
+00002230: 7374 7269 6e67 5f6d 6174 6368 696e 675f  string_matching_
+00002240: 7465 726d 6302 0000 0000 0000 0000 0000  termc...........
+00002250: 0002 0000 0003 0000 0043 0000 0073 1200  .........C...s..
+00002260: 0000 7c00 a000 7c01 a101 0100 7c00 a001  ..|...|.....|...
+00002270: a100 5300 2901 7a36 5265 7475 726e 2061  ..S.).z6Return a
+00002280: 6c6c 206d 6174 6368 696e 6720 696d 7061  ll matching impa
+00002290: 6374 2072 756c 6573 2066 6f72 2061 2067  ct rules for a g
+000022a0: 6976 656e 2073 656e 7465 6e63 652e 2902  iven sentence.).
+000022b0: 7266 0000 0072 6b00 0000 2902 723b 0000  rf...rk...).r;..
+000022c0: 0072 5700 0000 7217 0000 0072 1700 0000  .rW...r....r....
+000022d0: 7218 0000 00da 1366 696e 645f 696d 7061  r......find_impa
+000022e0: 6374 5f6d 6174 6368 6573 0f01 0000 7304  ct_matches....s.
+000022f0: 0000 000a 0208 017a 2149 6d70 6163 744d  .......z!ImpactM
+00002300: 6174 6368 6572 2e66 696e 645f 696d 7061  atcher.find_impa
+00002310: 6374 5f6d 6174 6368 6573 6301 0000 0000  ct_matchesc.....
+00002320: 0000 0000 0000 0001 0000 0003 0000 0003  ................
+00002330: 0000 0073 2600 0000 8800 6a00 7209 7401  ...s&.....j.r.t.
+00002340: 6401 8800 6a02 8302 0100 8700 6601 6402  d...j.......f.d.
+00002350: 6403 8408 8800 6a03 4400 8301 5300 2904  d.....j.D...S.).
+00002360: 7a3c 4d61 7463 6820 7365 6e74 656e 6365  z<Match sentence
+00002370: 2061 6761 696e 7374 2061 6c6c 2069 6d70   against all imp
+00002380: 6163 7420 7275 6c65 7320 6f66 2074 6865  act rules of the
+00002390: 2069 6d70 6163 7420 6d6f 6465 6c2e 7a1e   impact model.z.
+000023a0: 5f6d 6174 6368 5f72 756c 6573 202d 2073  _match_rules - s
+000023b0: 656e 7465 6e63 655f 696e 6465 783a 6301  entence_index:c.
+000023c0: 0000 0000 0000 0000 0000 0003 0000 0005  ................
+000023d0: 0000 0013 0000 0073 2000 0000 6700 7c00  .......s ...g.|.
+000023e0: 5d0c 7d01 8800 a000 7c01 a101 4400 5d04  ].}.....|...D.].
+000023f0: 7d02 7c02 9103 7109 7102 5300 7217 0000  }.|...q.q.S.r...
+00002400: 0029 01da 0a6d 6174 6368 5f72 756c 6529  .)...match_rule)
+00002410: 03da 022e 30da 0b69 6d70 6163 745f 7275  ....0..impact_ru
+00002420: 6c65 7216 0000 0072 6200 0000 7217 0000  ler....rb...r...
+00002430: 0072 1800 0000 da0a 3c6c 6973 7463 6f6d  .r......<listcom
+00002440: 703e 1801 0000 7302 0000 0020 007a 2e49  p>....s.... .z.I
+00002450: 6d70 6163 744d 6174 6368 6572 2e5f 6d61  mpactMatcher._ma
+00002460: 7463 685f 7275 6c65 732e 3c6c 6f63 616c  tch_rules.<local
+00002470: 733e 2e3c 6c69 7374 636f 6d70 3e29 0472  s>.<listcomp>).r
+00002480: 2c00 0000 721d 0000 0072 3300 0000 7237  ,...r....r3...r7
+00002490: 0000 0072 6200 0000 7217 0000 0072 6200  ...rb...r....rb.
+000024a0: 0000 7218 0000 0072 6b00 0000 1401 0000  ..r....rk.......
+000024b0: 7306 0000 0006 020c 0114 017a 1a49 6d70  s..........z.Imp
+000024c0: 6163 744d 6174 6368 6572 2e5f 6d61 7463  actMatcher._matc
+000024d0: 685f 7275 6c65 7372 8900 0000 6305 0000  h_rulesr....c...
+000024e0: 0000 0000 0000 0000 0005 0000 0005 0000  ................
+000024f0: 0043 0000 0073 5800 0000 7c02 7211 7c00  .C...sX...|.r.|.
+00002500: 6a00 7209 7401 6401 8301 0100 7c00 6a02  j.r.t.d.....|.j.
+00002510: 7c02 7c03 7c04 6402 8d03 0100 7c01 6a03  |.|.|.d.....|.j.
+00002520: 6a04 6403 6b02 721c 7c00 a005 7c01 a101  j.d.k.r.|...|...
+00002530: 5300 7c01 6a03 6a04 6404 6b02 7227 7c00  S.|.j.j.d.k.r'|.
+00002540: a005 7c01 a101 5300 7c00 a006 7c01 a101  ..|...S.|...|...
+00002550: 5300 2905 7a2e 4d61 7463 6820 7365 6e74  S.).z.Match sent
+00002560: 656e 6365 2061 6761 696e 7374 2061 2073  ence against a s
+00002570: 7065 6369 6669 6320 696d 7061 6374 2072  pecific impact r
+00002580: 756c 652e 7a26 7365 7474 696e 6720 7365  ule.z&setting se
+00002590: 6e74 656e 6365 2066 6f72 2073 696e 676c  ntence for singl
+000025a0: 6520 7275 6c65 206d 6174 6368 7264 0000  e rule matchrd..
+000025b0: 0072 3f00 0000 7240 0000 0029 0772 2c00  .r?...r@...).r,.
+000025c0: 0000 721d 0000 0072 6600 0000 724b 0000  ..r....rf...rK..
+000025d0: 0072 4c00 0000 da13 6d61 7463 685f 696d  .rL.....match_im
+000025e0: 7061 6374 5f70 6872 6173 65da 116d 6174  pact_phrase..mat
+000025f0: 6368 5f69 6d70 6163 745f 7465 726d 2905  ch_impact_term).
+00002600: 723b 0000 0072 8900 0000 7257 0000 0072  r;...r....rW...r
+00002610: 3300 0000 7232 0000 0072 1700 0000 7217  3...r2...r....r.
+00002620: 0000 0072 1800 0000 7287 0000 001a 0100  ...r....r.......
+00002630: 0073 1200 0000 0403 0601 0801 1001 0c01  .s..............
+00002640: 0a01 0c01 0a01 0a02 7a18 496d 7061 6374  ........z.Impact
+00002650: 4d61 7463 6865 722e 6d61 7463 685f 7275  Matcher.match_ru
+00002660: 6c65 6302 0000 0000 0000 0000 0000 0005  lec.............
+00002670: 0000 000c 0000 0043 0000 0073 ac00 0000  .......C...s....
+00002680: 6700 7d02 7c00 6a00 7218 7401 6401 7c01  g.}.|.j.r.t.d.|.
+00002690: 6a02 6a03 8302 0100 7401 6402 7c01 6a02  j.j.....t.d.|.j.
+000026a0: 8302 0100 7401 6403 7c00 6a04 8302 0100  ....t.d.|.j.....
+000026b0: 7c00 6a05 7c01 6a02 6a03 7c01 6a06 6404  |.j.|.j.j.|.j.d.
+000026c0: 8d02 4400 5d31 7d03 7407 7c03 a008 6405  ..D.]1}.t.|...d.
+000026d0: a101 6406 7c03 a009 a100 7c01 6a02 6a03  ..d.|.....|.j.j.
+000026e0: 7c01 6a02 6a0a 7c01 6a0b 7c00 6a0c 7c00  |.j.j.|.j.|.j.|.
+000026f0: 6a0d 7c00 6a04 6407 8d09 7d04 7c00 a00e  j.|.j.d...}.|...
+00002700: 7c01 7c04 a102 724a 7c02 a00f 7c04 a101  |.|...rJ|...|...
+00002710: 0100 7122 7c00 6a00 7253 7401 6408 7c01  ..q"|.j.rSt.d.|.
+00002720: 6a10 8302 0100 7122 7c02 5300 2909 7a28  j.....q"|.S.).z(
+00002730: 4368 6563 6b20 6966 2073 656e 7465 6e63  Check if sentenc
+00002740: 6520 6d61 7463 6865 7320 696d 7061 6374  e matches impact
+00002750: 2070 6872 6173 652e 7a0d 6d61 7463 685f   phrase.z.match_
+00002760: 7068 7261 7365 3a7a 0c69 6d70 6163 745f  phrase:z.impact_
+00002770: 7465 726d 3a72 7c00 0000 a901 7275 0000  term:r|.....ru..
+00002780: 0072 0100 0000 4ea9 0372 3200 0000 7233  .r....N..r2...r3
+00002790: 0000 0072 5700 0000 fa19 5048 5241 5345  ...rW.....PHRASE
+000027a0: 2043 4f4e 4449 5449 4f4e 204e 4f54 204d   CONDITION NOT M
+000027b0: 4554 3a29 1172 2c00 0000 721d 0000 0072  ET:).r,...r....r
+000027c0: 4b00 0000 7226 0000 0072 3000 0000 7285  K...r&...r0...r.
+000027d0: 0000 0072 7500 0000 7209 0000 00da 0567  ...ru...r......g
+000027e0: 726f 7570 da05 7374 6172 7472 4c00 0000  roup..startrL...
+000027f0: 7212 0000 0072 3200 0000 7233 0000 00da  r....r2...r3....
+00002800: 0f6d 6174 6368 5f63 6f6e 6469 7469 6f6e  .match_condition
+00002810: 724f 0000 00da 0963 6f6e 6469 7469 6f6e  rO.....condition
+00002820: 2905 723b 0000 0072 8900 0000 da07 6d61  ).r;...r......ma
+00002830: 7463 6865 7372 1600 0000 da0c 696d 7061  tchesr......impa
+00002840: 6374 5f6d 6174 6368 7217 0000 0072 1700  ct_matchr....r..
+00002850: 0000 7218 0000 0072 8b00 0000 2801 0000  ..r....r....(...
+00002860: 7326 0000 0004 0206 010e 010c 010c 010a  s&..............
+00002870: 0104 010a ff18 020a 0108 0104 0106 fd0c  ................
+00002880: 040c 0106 010c 0102 8004 017a 2149 6d70  ...........z!Imp
+00002890: 6163 744d 6174 6368 6572 2e6d 6174 6368  actMatcher.match
+000028a0: 5f69 6d70 6163 745f 7068 7261 7365 6302  _impact_phrasec.
+000028b0: 0000 0000 0000 0000 0000 0007 0000 000c  ................
+000028c0: 0000 0043 0000 0073 bc00 0000 6700 7d02  ...C...s....g.}.
+000028d0: 7c01 6a00 6a01 7d03 7c01 6a00 6a02 7d04  |.j.j.}.|.j.j.}.
+000028e0: 7c00 6a03 721a 7404 6401 7c03 6402 7c04  |.j.r.t.d.|.d.|.
+000028f0: 8304 0100 7404 6403 7c00 6a05 8302 0100  ....t.d.|.j.....
+00002900: 7c00 6a06 7c03 7c04 7c01 6a07 6404 8d03  |.j.|.|.|.j.d...
+00002910: 4400 5d38 7d05 7408 7c05 6a09 7c05 6a0a  D.]8}.t.|.j.|.j.
+00002920: 7c05 6a0b 7c01 6a00 6a01 7c01 6a00 6a0c  |.j.|.j.j.|.j.j.
+00002930: 7c01 6a0d 7c00 6a0e 7c00 6a0f 7c00 6a05  |.j.|.j.|.j.|.j.
+00002940: 6405 8d09 7d06 7c00 6a03 7246 7404 6406  d...}.|.j.rFt.d.
+00002950: 7c05 6a09 8302 0100 7c00 a010 7c01 7c06  |.j.....|...|.|.
+00002960: a102 7252 7c02 a011 7c06 a101 0100 7123  ..rR|...|.....q#
+00002970: 7c00 6a03 725b 7404 6407 7c01 6a12 8302  |.j.r[t.d.|.j...
+00002980: 0100 7123 7c02 5300 2908 7a26 4368 6563  ..q#|.S.).z&Chec
+00002990: 6b20 6966 2073 656e 7465 6e63 6520 6d61  k if sentence ma
+000029a0: 7463 6865 7320 696d 7061 6374 2074 6572  tches impact ter
+000029b0: 6d2e 7a0b 6d61 7463 685f 7465 726d 3a7a  m.z.match_term:z
+000029c0: 0a6d 6174 6368 5f70 6f73 3a72 7c00 0000  .match_pos:r|...
+000029d0: 728d 0000 0072 8e00 0000 7a0b 6d61 7463  r....r....z.matc
+000029e0: 6820 7465 726d 3a72 8f00 0000 2913 724b  h term:r....).rK
+000029f0: 0000 0072 2600 0000 725b 0000 0072 2c00  ...r&...r[...r,.
+00002a00: 0000 721d 0000 0072 3000 0000 727a 0000  ..r....r0...rz..
+00002a10: 0072 7500 0000 7209 0000 0072 5100 0000  .ru...r....rQ...
+00002a20: 7221 0000 0072 5c00 0000 724c 0000 0072  r!...r\...rL...r
+00002a30: 1200 0000 7232 0000 0072 3300 0000 7292  ....r2...r3...r.
+00002a40: 0000 0072 4f00 0000 7293 0000 0029 0772  ...rO...r....).r
+00002a50: 3b00 0000 7289 0000 00da 0e69 6d70 6163  ;...r......impac
+00002a60: 745f 6d61 7463 6865 7372 7400 0000 7279  t_matchesrt...ry
+00002a70: 0000 005a 0c69 6d70 6163 745f 746f 6b65  ...Z.impact_toke
+00002a80: 6e72 9500 0000 7217 0000 0072 1700 0000  nr....r....r....
+00002a90: 7218 0000 0072 8c00 0000 3b01 0000 732e  r....r....;...s.
+00002aa0: 0000 0004 0208 0108 0106 010e 010c 0108  ................
+00002ab0: 0104 010a ff0e 020c 0104 0108 0104 0106  ................
+00002ac0: fc06 050c 010c 010c 0106 010c 0102 8004  ................
+00002ad0: 017a 1f49 6d70 6163 744d 6174 6368 6572  .z.ImpactMatcher
+00002ae0: 2e6d 6174 6368 5f69 6d70 6163 745f 7465  .match_impact_te
+00002af0: 726d 7295 0000 0063 0300 0000 0000 0000  rmr....c........
+00002b00: 0000 0000 0400 0000 0400 0000 4300 0000  ............C...
+00002b10: 73de 0000 007c 016a 0073 0564 0153 007c  s....|.j.s.d.S.|
+00002b20: 006a 0172 1674 0264 027c 016a 0064 0319  .j.r.t.d.|.j.d..
+00002b30: 0083 0201 0074 0264 047c 016a 0083 0201  .....t.d.|.j....
+00002b40: 007c 016a 0064 0319 0064 056b 0272 247c  .|.j.d...d.k.r$|
+00002b50: 00a0 037c 017c 02a1 027d 036e 197c 016a  ...|.|...}.n.|.j
+00002b60: 0064 0319 0064 066b 0272 327c 00a0 047c  .d...d.k.r2|...|
+00002b70: 017c 02a1 027d 036e 0b7c 006a 0172 3b74  .|...}.n.|.j.r;t
+00002b80: 0264 077c 016a 0083 0201 0064 0853 007c  .d.|.j.....d.S.|
+00002b90: 016a 0572 4a7c 006a 0172 4774 0264 0983  .j.rJ|.j.rGt.d..
+00002ba0: 0101 007c 030c 007d 037c 006a 0172 6d7c  ...|...}.|.j.rm|
+00002bb0: 0372 5f74 0264 0a7c 016a 0083 0201 0074  .r_t.d.|.j.....t
+00002bc0: 0264 0b7c 0283 0201 0074 0283 0001 007c  .d.|.....t.....|
+00002bd0: 0353 0074 0264 0c7c 016a 0083 0201 0074  .S.t.d.|.j.....t
+00002be0: 0264 0b7c 0283 0201 0074 0283 0001 007c  .d.|.....t.....|
+00002bf0: 0353 0029 0dfa 4943 6865 636b 2069 6620  .S.)..ICheck if 
+00002c00: 7365 6e74 656e 6365 2077 6974 6820 696d  sentence with im
+00002c10: 7061 6374 2074 6572 6d20 6d61 7463 6820  pact term match 
+00002c20: 616c 736f 206d 6174 6368 6573 2063 6f6e  also matches con
+00002c30: 7465 7874 2063 6f6e 6469 7469 6f6e 732e  text conditions.
+00002c40: 547a 0f63 6f6e 6469 7469 6f6e 2074 7970  Tz.condition typ
+00002c50: 653a da0e 636f 6e64 6974 696f 6e5f 7479  e:..condition_ty
+00002c60: 7065 7a0a 636f 6e64 6974 696f 6e3a da0b  pez.condition:..
+00002c70: 6173 7065 6374 5f74 6572 6dda 0c63 6f6e  aspect_term..con
+00002c80: 7465 7874 5f74 6572 6d7a 104f 5448 4552  text_termz.OTHER
+00002c90: 2043 4f4e 4449 5449 4f4e 3a46 7a0f 494e   CONDITION:Fz.IN
+00002ca0: 5645 5254 494e 4720 4d41 5443 487a 134d  VERTING MATCHz.M
+00002cb0: 4154 4348 494e 4720 434f 4e44 4954 494f  ATCHING CONDITIO
+00002cc0: 4e3a 7a0d 494d 5041 4354 5f4d 4154 4348  N:z.IMPACT_MATCH
+00002cd0: 3a7a 164e 4f20 4d41 5443 4849 4e47 2043  :z.NO MATCHING C
+00002ce0: 4f4e 4449 5449 4f4e 3a29 0672 9300 0000  ONDITION:).r....
+00002cf0: 722c 0000 0072 1d00 0000 da16 6d61 7463  r,...r......matc
+00002d00: 685f 6173 7065 6374 5f63 6f6e 6469 7469  h_aspect_conditi
+00002d10: 6f6e da17 6d61 7463 685f 636f 6e74 6578  on..match_contex
+00002d20: 745f 636f 6e64 6974 696f 6eda 0666 696c  t_condition..fil
+00002d30: 7465 7229 0472 3b00 0000 7289 0000 0072  ter).r;...r....r
+00002d40: 9500 0000 7216 0000 0072 1700 0000 7217  ....r....r....r.
+00002d50: 0000 0072 1800 0000 7292 0000 0052 0100  ...r....r....R..
+00002d60: 0073 3400 0000 0602 0401 0601 1001 0c01  .s4.............
+00002d70: 0e01 0e01 0e01 0e01 0602 0c01 0401 0601  ................
+00002d80: 0601 0801 0601 0601 0401 0c01 0a01 0601  ................
+00002d90: 0405 0cfd 0a01 0601 0401 7a1d 496d 7061  ..........z.Impa
+00002da0: 6374 4d61 7463 6865 722e 6d61 7463 685f  ctMatcher.match_
+00002db0: 636f 6e64 6974 696f 6e63 0300 0000 0000  conditionc......
+00002dc0: 0000 0000 0000 0a00 0000 0800 0000 4300  ..............C.
+00002dd0: 0000 73dc 0000 007c 016a 0064 0119 007d  ..s....|.j.d...}
+00002de0: 037c 006a 01a0 027c 03a1 017d 047c 0473  .|.j...|...}.|.s
+00002df0: 1474 0364 027c 0383 0201 0064 0353 007c  .t.d.|.....d.S.|
+00002e00: 0464 0419 0044 005d 537d 0567 007d 067c  .d...D.]S}.g.}.|
+00002e10: 006a 047c 057c 016a 0564 058d 0244 005d  .j.|.|.j.d...D.]
+00002e20: 127d 0774 067c 076a 077c 076a 087c 076a  .}.t.|.j.|.j.|.j
+00002e30: 097c 057c 0383 057d 087c 06a0 0a7c 08a1  .|.|...}.|...|..
+00002e40: 0101 0071 2474 0b7c 0683 0164 066b 0472  ...q$t.|...d.k.r
+00002e50: 437c 067c 025f 0c01 0064 0753 007c 006a  C|.|._...d.S.|.j
+00002e60: 0d7c 0564 087c 016a 0564 058d 0344 005d  .|.d.|.j.d...D.]
+00002e70: 127d 0974 067c 096a 077c 096a 087c 096a  .}.t.|.j.|.j.|.j
+00002e80: 097c 057c 0383 057d 087c 06a0 0a7c 08a1  .|.|...}.|...|..
+00002e90: 0101 0071 4c74 0b7c 0683 0164 066b 0472  ...qLt.|...d.k.r
+00002ea0: 6b7c 067c 025f 0c01 0064 0753 0071 1864  k|.|._...d.S.q.d
+00002eb0: 0353 0029 097a 4843 6865 636b 2069 6620  .S.).zHCheck if 
+00002ec0: 7365 6e74 656e 6365 2077 6974 6820 696d  sentence with im
+00002ed0: 7061 6374 2074 6572 6d20 6d61 7463 6820  pact term match 
+00002ee0: 616c 736f 206d 6174 6368 6573 2061 7370  also matches asp
+00002ef0: 6563 7420 636f 6e64 6974 696f 6e73 2eda  ect conditions..
+00002f00: 0c61 7370 6563 745f 6772 6f75 707a 2e45  .aspect_groupz.E
+00002f10: 7272 6f72 202d 206e 6f20 6173 7065 6374  rror - no aspect
+00002f20: 2067 726f 7570 2069 6e66 6f20 666f 7220   group info for 
+00002f30: 6173 7065 6374 2067 726f 7570 3a46 7299  aspect group:Fr.
+00002f40: 0000 0072 8d00 0000 7201 0000 0054 4e29  ...r....r....TN)
+00002f50: 0e72 9300 0000 722b 0000 0072 9e00 0000  .r....r+...r....
+00002f60: 721d 0000 0072 7700 0000 7275 0000 0072  r....rw...ru...r
+00002f70: 0a00 0000 7251 0000 0072 2100 0000 725c  ....rQ...r!...r\
+00002f80: 0000 0072 4f00 0000 da03 6c65 6eda 1163  ...rO.....len..c
+00002f90: 6f6e 6469 7469 6f6e 5f6d 6174 6368 6573  ondition_matches
+00002fa0: 727a 0000 0029 0a72 3b00 0000 7289 0000  rz...).r;...r...
+00002fb0: 0072 9500 0000 729e 0000 005a 0b61 7370  .r....r....Z.asp
+00002fc0: 6563 745f 696e 666f 7299 0000 0072 a000  ect_infor....r..
+00002fd0: 0000 5a0c 6173 7065 6374 5f6d 6174 6368  ..Z.aspect_match
+00002fe0: da0f 636f 6e64 6974 696f 6e5f 6d61 7463  ..condition_matc
+00002ff0: 685a 0c61 7370 6563 745f 746f 6b65 6e72  hZ.aspect_tokenr
+00003000: 1700 0000 7217 0000 0072 1800 0000 729b  ....r....r....r.
+00003010: 0000 0070 0100 0073 3a00 0000 0a02 0c01  ...p...s:.......
+00003020: 0401 0a01 0401 0c01 0401 0601 0401 0aff  ................
+00003030: 0e02 0401 04ff 0c02 0c01 0601 0601 0801  ................
+00003040: 0401 0aff 0e02 0401 04ff 0c02 0c01 0601  ................
+00003050: 0601 02fe 0403 7a24 496d 7061 6374 4d61  ......z$ImpactMa
+00003060: 7463 6865 722e 6d61 7463 685f 6173 7065  tcher.match_aspe
+00003070: 6374 5f63 6f6e 6469 7469 6f6e 6303 0000  ct_conditionc...
+00003080: 0000 0000 0000 0000 0007 0000 0008 0000  ................
+00003090: 0043 0000 0073 a200 0000 7c01 6a00 6401  .C...s....|.j.d.
+000030a0: 1900 7d03 6700 7d04 7c01 6a00 6402 1900  ..}.g.}.|.j.d...
+000030b0: 6403 6b02 7219 7c00 6a01 7219 7402 6404  d.k.r.|.j.r.t.d.
+000030c0: 7c03 6405 7c01 6a00 8304 0100 7c00 6a03  |.d.|.j.....|.j.
+000030d0: 7c03 7c01 6a00 6402 1900 7c01 6a04 6406  |.|.j.d...|.j.d.
+000030e0: 8d03 4400 5d1e 7d05 7405 7c05 a006 6407  ..D.].}.t.|...d.
+000030f0: a101 6408 7c05 a007 a100 7c03 7c01 6a00  ..d.|.....|.|.j.
+00003100: 6409 1900 8305 7d06 7c00 6a01 723e 7402  d.....}.|.j.r>t.
+00003110: 640a 8301 0100 7c04 a008 7c06 a101 0100  d.....|...|.....
+00003120: 7125 7409 7c04 8301 6407 6b04 724f 7c04  q%t.|...d.k.rO|.
+00003130: 7c02 5f0a 640b 5300 640c 5300 290d 7297  |._.d.S.d.S.).r.
+00003140: 0000 0072 9a00 0000 7284 0000 0072 7d00  ...r....r....r}.
+00003150: 0000 7a10 6c6f 6f6b 696e 6720 666f 7220  ..z.looking for 
+00003160: 7465 726d 7a0f 2077 6974 6820 636f 6e64  termz. with cond
+00003170: 6974 696f 6e72 8d00 0000 7201 0000 004e  itionr....r....N
+00003180: 723e 0000 007a 1743 4f4e 5445 5854 2043  r>...z.CONTEXT C
+00003190: 4f4e 4449 5449 4f4e 204d 4154 4348 5446  ONDITION MATCHTF
+000031a0: 290b 7293 0000 0072 2c00 0000 721d 0000  ).r....r,...r...
+000031b0: 0072 8500 0000 7275 0000 0072 0a00 0000  .r....ru...r....
+000031c0: 7290 0000 0072 9100 0000 724f 0000 0072  r....r....rO...r
+000031d0: 9f00 0000 72a0 0000 0029 0772 3b00 0000  ....r....).r;...
+000031e0: 7289 0000 0072 9500 0000 729a 0000 0072  r....r....r....r
+000031f0: a000 0000 5a0d 636f 6e74 6578 745f 6d61  ....Z.context_ma
+00003200: 7463 6872 a100 0000 7217 0000 0072 1700  tchr....r....r..
+00003210: 0000 7218 0000 0072 9c00 0000 8b01 0000  ..r....r........
+00003220: 7324 0000 000a 0204 010e 0106 0110 010e  s$..............
+00003230: 0104 010a ff12 020a 0104 ff06 0208 010c  ................
+00003240: 010c 0106 0104 0104 027a 2549 6d70 6163  .........z%Impac
+00003250: 744d 6174 6368 6572 2e6d 6174 6368 5f63  tMatcher.match_c
+00003260: 6f6e 7465 7874 5f63 6f6e 6469 7469 6f6e  ontext_condition
+00003270: 7216 0000 0063 0200 0000 0000 0000 0000  r....c..........
+00003280: 0000 0700 0000 0400 0000 4300 0000 738a  ..........C...s.
+00003290: 0000 007c 016a 007c 016a 017c 016a 0264  ...|.j.|.j.|.j.d
+000032a0: 019c 037d 0274 037c 006a 0419 0044 005d  ...}.t.|.j...D.]
+000032b0: 067d 0364 027c 027c 033c 0071 0e74 0544  .}.d.|.|.<.q.t.D
+000032c0: 005d 097d 047c 01a0 067c 04a1 017c 027c  .].}.|...|...|.|
+000032d0: 043c 0071 1774 0744 005d 1f7d 0574 087c  .<.q.t.D.].}.t.|
+000032e0: 016a 0983 0164 026b 0472 427c 05a0 0a64  .j...d.k.rB|...d
+000032f0: 03a1 0172 337c 056e 0464 047c 059b 009d  ...r3|.n.d.|....
+00003300: 027d 067c 016a 0964 0219 00a0 067c 05a1  .}.|.j.d.....|..
+00003310: 017c 027c 063c 0071 237c 0253 0029 054e  .|.|.<.q#|.S.).N
+00003320: 728e 0000 0072 0100 0000 da04 636f 6e64  r....r......cond
+00003330: da0a 636f 6e64 6974 696f 6e5f 290b 7232  ..condition_).r2
+00003340: 0000 0072 3300 0000 7257 0000 0072 0c00  ...r3...rW...r..
+00003350: 0000 722a 0000 0072 0d00 0000 da10 5f5f  ..r*...r......__
+00003360: 6765 7461 7474 7269 6275 7465 5f5f 720e  getattribute__r.
+00003370: 0000 0072 9f00 0000 72a0 0000 00da 0a73  ...r....r......s
+00003380: 7461 7274 7377 6974 6829 0772 3b00 0000  tartswith).r;...
+00003390: 7216 0000 00da 0669 6d70 6163 7472 1200  r......impactr..
+000033a0: 0000 da05 6669 656c 64da 0a63 6f6e 645f  ....field..cond_
+000033b0: 6669 656c 64da 0d64 6973 706c 6179 5f66  field..display_f
+000033c0: 6965 6c64 7217 0000 0072 1700 0000 7218  ieldr....r....r.
+000033d0: 0000 00da 1269 6e69 745f 696d 7061 6374  .....init_impact
+000033e0: 5f73 636f 7265 739f 0100 0073 1c00 0000  _scores....s....
+000033f0: 0402 0401 0401 06fd 0e05 0a01 0801 1001  ................
+00003400: 0801 0e01 1801 1401 0280 0401 7a20 496d  ............z Im
+00003410: 7061 6374 4d61 7463 6865 722e 696e 6974  pactMatcher.init
+00003420: 5f69 6d70 6163 745f 7363 6f72 6573 7296  _impact_scoresr.
+00003430: 0000 0063 0300 0000 0000 0000 0000 0000  ...c............
+00003440: 0c00 0000 0500 0000 4300 0000 7334 0100  ........C...s4..
+00003450: 0068 0064 01a3 017d 0367 007d 0474 0083  .h.d...}.g.}.t..
+00003460: 007d 057c 0144 005d 8c7d 067c 00a0 017c  .}.|.D.].}.|...|
+00003470: 06a1 017d 077c 0264 0275 0072 1c7c 066a  ...}.|.d.u.r.|.j
+00003480: 0264 036b 0272 1c71 0b7c 066a 037d 0674  .d.k.r.q.|.j.}.t
+00003490: 0444 005d 087d 087c 067c 0819 007c 077c  .D.].}.|.|...|.|
+000034a0: 083c 0071 2174 0544 005d 247d 0964 047c  .<.q!t.D.]$}.d.|
+000034b0: 0676 0072 5074 067c 0664 0419 0083 0164  .v.rPt.|.d.....d
+000034c0: 056b 0472 507c 09a0 0764 06a1 0172 417c  .k.rP|...d...rA|
+000034d0: 096e 0464 077c 099b 009d 027d 0a7c 0664  .n.d.|.....}.|.d
+000034e0: 0419 0064 0519 007c 0919 007c 077c 0a3c  ...d...|...|.|.<
+000034f0: 0071 2c7c 0664 0819 0064 036b 0272 5871  .q,|.d...d.k.rXq
+00003500: 0b74 087c 0683 017d 0b7c 0664 0919 007c  .t.|...}.|.d...|
+00003510: 0b66 027c 0576 0172 757c 077c 0b05 0019  .f.|.v.ru|.|....
+00003520: 0064 0a37 0003 003c 007c 05a0 097c 0664  .d.7...<.|...|.d
+00003530: 0919 007c 0b66 02a1 0101 007c 0b7c 0376  ...|.f.....|.|.v
+00003540: 0072 927c 0664 0919 0064 0b66 027c 0576  .r.|.d...d.f.|.v
+00003550: 0172 927c 0764 0b05 0019 0064 0a37 0003  .r.|.d.....d.7..
+00003560: 003c 007c 05a0 097c 0664 0919 0064 0b66  .<.|...|.d...d.f
+00003570: 02a1 0101 007c 04a0 0a7c 07a1 0101 0071  .....|...|.....q
+00003580: 0b7c 0453 0029 0c4e 3e03 0000 00da 0573  .|.S.).N>......s
+00003590: 7479 6c65 da09 6e61 7272 6174 6976 65da  tyle..narrative.
+000035a0: 0568 756d 6f72 46da 074e 6575 7472 616c  .humorF..Neutral
+000035b0: 72a1 0000 0072 0100 0000 72a2 0000 0072  r....r....r....r
+000035c0: a300 0000 7212 0000 00da 0b6d 6174 6368  ....r......match
+000035d0: 5f69 6e64 6578 7245 0000 0072 1400 0000  _indexrE...r....
+000035e0: 290b 7234 0000 0072 aa00 0000 7212 0000  ).r4...r....r...
+000035f0: 00da 046a 736f 6e72 0d00 0000 720e 0000  ...jsonr....r...
+00003600: 0072 9f00 0000 72a5 0000 0072 1900 0000  .r....r....r....
+00003610: 7253 0000 0072 4f00 0000 290c 723b 0000  rS...rO...).r;..
+00003620: 0072 9600 0000 726a 0000 005a 1070 6f73  .r....rj...Z.pos
+00003630: 6974 6976 655f 7375 625f 6361 7472 6f00  itive_sub_catro.
+00003640: 0000 5a07 636f 756e 7465 6472 1600 0000  ..Z.countedr....
+00003650: 72a6 0000 0072 a700 0000 72a8 0000 0072  r....r....r....r
+00003660: a900 0000 7212 0000 0072 1700 0000 7217  ....r....r....r.
+00003670: 0000 0072 1800 0000 726d 0000 00af 0100  ...r....rm......
+00003680: 0073 3600 0000 0802 0401 0601 0801 0a01  .s6.............
+00003690: 1201 0201 0601 0801 0e01 0801 1801 1801  ................
+000036a0: 1401 0280 0c01 0201 0801 1001 1001 1201  ................
+000036b0: 0801 1001 1001 1201 0c01 0401 7a23 496d  ............z#Im
+000036c0: 7061 6374 4d61 7463 6865 722e 636f 6d70  pactMatcher.comp
+000036d0: 7574 655f 7265 7669 6577 5f69 6d70 6163  ute_review_impac
+000036e0: 7429 0372 2900 0000 4e46 2902 4e4e 7249  t).r)...NF).NNrI
+000036f0: 0000 0029 024e 4629 0154 2902 727b 0000  ...).NF).T).r{..
+00003700: 0054 2903 4e4e 4e29 0146 2926 da08 5f5f  .T).NNN).F)&..__
+00003710: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
+00003720: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
+00003730: 7252 0000 0072 0700 0000 da04 626f 6f6c  rR...r......bool
+00003740: 723c 0000 0072 0800 0000 7248 0000 0072  r<...r....rH...r
+00003750: 3a00 0000 724e 0000 0072 0b00 0000 7256  :...rN...r....rV
+00003760: 0000 0072 0300 0000 da03 616e 7972 3600  ...r......anyr6.
+00003770: 0000 725f 0000 0072 6100 0000 7263 0000  ..r_...ra...rc..
+00003780: 0072 6600 0000 7269 0000 0072 0400 0000  .rf...ri...r....
+00003790: 7270 0000 0072 7300 0000 7277 0000 0072  rp...rs...rw...r
+000037a0: 7a00 0000 7285 0000 0072 8600 0000 726b  z...r....r....rk
+000037b0: 0000 0072 0900 0000 7287 0000 0072 8b00  ...r....r....r..
+000037c0: 0000 728c 0000 0072 9200 0000 729b 0000  ..r....r....r...
+000037d0: 0072 9c00 0000 72aa 0000 0072 6d00 0000  .r....r....rm...
+000037e0: 7217 0000 0072 1700 0000 7217 0000 0072  r....r....r....r
+000037f0: 1800 0000 7228 0000 0037 0000 0073 5600  ....r(...7...sV.
+00003800: 0000 0800 1802 161e 0812 0807 0e0b 2211  ..............".
+00003810: 1a09 080c 1c07 140b 0208 0201 0cff 0201  ................
+00003820: 02ff 0e01 0aff 0a0a 0a0b 0a0b 0a1c 0818  ................
+00003830: 0805 0206 0201 0cff 0201 02ff 0601 0aff  ................
+00003840: 120e 0e13 1217 161e 161b 1a14 0211 0cff  ................
+00003850: 0201 02ff 0e01 0eff 7228 0000 0029 1a72  ........r(...).r
+00003860: 2400 0000 da0b 636f 6c6c 6563 7469 6f6e  $.....collection
+00003870: 7372 0200 0000 da06 7479 7069 6e67 7203  sr......typingr.
+00003880: 0000 0072 0400 0000 7205 0000 005a 0d6e  ...r....r....Z.n
+00003890: 6c74 6b2e 746f 6b65 6e69 7a65 7206 0000  ltk.tokenizer...
+000038a0: 005a 2172 6561 6469 6e67 5f69 6d70 6163  .Z!reading_impac
+000038b0: 745f 6d6f 6465 6c2e 696d 7061 6374 5f6d  t_model.impact_m
+000038c0: 6f64 656c 7207 0000 0072 0800 0000 7209  odelr....r....r.
+000038d0: 0000 0072 0a00 0000 720b 0000 0072 0c00  ...r....r....r..
+000038e0: 0000 720d 0000 0072 0e00 0000 720f 0000  ..r....r....r...
+000038f0: 0072 1000 0000 7211 0000 0072 1900 0000  .r....r....r....
+00003900: 721f 0000 0072 2300 0000 7227 0000 0072  r....r#...r'...r
+00003910: 2800 0000 7217 0000 0072 1700 0000 7217  (...r....r....r.
+00003920: 0000 0072 1800 0000 da08 3c6d 6f64 756c  ...r......<modul
+00003930: 653e 0100 0000 731a 0000 0008 000c 0114  e>....s.........
+00003940: 010c 021c 0214 010c 0110 0108 0308 0708  ................
+00003950: 0f08 0f12 05                             .....
```

### Comparing `reading_impact_model-1.0.1/reading_impact_model/matchers/__pycache__/spacy_matcher.cpython-310.pyc` & `reading_impact_model-1.0.2/reading_impact_model/matchers/__pycache__/spacy_matcher.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Mar 24 12:38:28 2023 UTC, .py size: 1474 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,117 +1,119 @@
-00000000: 6f0d 0d0a 0000 0000 c499 1d64 c205 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 e18a 8064 fc05 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5600 0000 6400  .....@...sV...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 5a03 6400 6403 6c04 6d05 5a06  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6404 6c07 6d08 5a08 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c09 6d0a 5a0a 6d0b 5a0b 0100 4700  d.l.m.Z.m.Z...G.
 00000070: 6406 6407 8400 6407 6508 6a0c 8303 5a0d  d.d...d.e.j...Z.
 00000080: 6402 5300 2908 e900 0000 0029 02da 0444  d.S.)......)...D
 00000090: 6963 74da 0555 6e69 6f6e 4e29 01da 0453  ict..UnionN)...S
 000000a0: 7061 6e29 01da 076d 6174 6368 6572 2902  pan)...matcher).
 000000b0: da0b 496d 7061 6374 4d6f 6465 6cda 0554  ..ImpactModel..T
 000000c0: 6f6b 656e 6300 0000 0000 0000 0000 0000  okenc...........
-000000d0: 0000 0000 0008 0000 0000 0000 0073 6400  .............sd.
+000000d0: 0000 0000 0009 0000 0000 0000 0073 6a00  .............sj.
 000000e0: 0000 6500 5a01 6400 5a02 6411 6403 6503  ..e.Z.d.Z.d.d.e.
 000000f0: 6a04 6404 6505 6405 6506 6606 8700 6601  j.d.e.d.e.f...f.
 00000100: 6406 6407 840d 5a07 6412 6408 6505 6409  d.d...Z.d.d.e.d.
-00000110: 6505 6604 640a 640b 8405 5a08 640c 6509  e.f.d.d...Z.d.e.
-00000120: 640d 650a 6505 650b 6602 1900 6409 6505  d.e.e.e.f...d.e.
-00000130: 640e 6402 6608 640f 6410 8404 5a0c 8700  d.d.f.d.d...Z...
-00000140: 0400 5a0d 5300 2913 da0c 5370 6163 794d  ..Z.S.)...SpacyM
-00000150: 6174 6368 6572 da02 656e 4eda 0670 6172  atcher..enN..par
-00000160: 7365 72da 046c 616e 67da 0c69 6d70 6163  ser..lang..impac
-00000170: 745f 6d6f 6465 6c63 0400 0000 0000 0000  t_modelc........
-00000180: 0000 0000 0500 0000 0500 0000 0b00 0000  ................
-00000190: 7328 0000 0074 0083 006a 0164 027c 027c  s(...t...j.d.|.|
-000001a0: 0364 019c 027c 04a4 018e 0101 007c 017c  .d...|.......|.|
-000001b0: 005f 027c 027c 005f 0364 0053 0029 034e  ._.|.|._.d.S.).N
-000001c0: 2902 720b 0000 0072 0c00 0000 a900 2904  ).r....r......).
-000001d0: da05 7375 7065 72da 085f 5f69 6e69 745f  ..super..__init_
-000001e0: 5f72 0a00 0000 720b 0000 0029 05da 0473  _r....r....)...s
-000001f0: 656c 6672 0a00 0000 720b 0000 0072 0c00  elfr....r....r..
-00000200: 0000 da06 6b77 6172 6773 a901 da09 5f5f  ....kwargs....__
-00000210: 636c 6173 735f 5f72 0d00 0000 fa73 2f55  class__r.....s/U
-00000220: 7365 7273 2f6d 6172 696a 6e6b 6f6f 6c65  sers/marijnkoole
-00000230: 6e2f 4461 7461 2f50 726f 6a65 6374 732f  n/Data/Projects/
-00000240: 542d 5265 6373 2f41 7070 6561 6c2f 7265  T-Recs/Appeal/re
-00000250: 6164 696e 672d 696d 7061 6374 2d6d 6f64  ading-impact-mod
-00000260: 656c 2f72 6561 6469 6e67 5f69 6d70 6163  el/reading_impac
-00000270: 745f 6d6f 6465 6c2f 6d61 7463 6865 7273  t_model/matchers
-00000280: 2f73 7061 6379 5f6d 6174 6368 6572 2e70  /spacy_matcher.p
-00000290: 7972 0f00 0000 0c00 0000 7306 0000 0018  yr........s.....
-000002a0: 0206 010a 017a 1553 7061 6379 4d61 7463  .....z.SpacyMatc
-000002b0: 6865 722e 5f5f 696e 6974 5f5f da04 7465  her.__init__..te
-000002c0: 7874 da06 646f 635f 6964 6303 0000 0000  xt..doc_idc.....
-000002d0: 0000 0000 0000 0006 0000 0006 0000 0063  ...............c
-000002e0: 0000 0073 3800 0000 8100 7c00 a000 7c01  ...s8.....|...|.
-000002f0: a101 7d03 7401 7c03 6a02 8301 4400 5d0e  ..}.t.|.j...D.].
-00000300: 5c02 7d04 7d05 7c00 a003 7c04 7c05 7c02  \.}.}.|...|.|.|.
-00000310: a103 0100 7c04 5600 0100 710b 6400 5300  ....|.V...q.d.S.
-00000320: a901 4e29 0472 0a00 0000 da09 656e 756d  ..N).r......enum
-00000330: 6572 6174 65da 0573 656e 7473 da0d 5f73  erate..sents.._s
-00000340: 6574 5f73 656e 7465 6e63 6529 0672 1000  et_sentence).r..
-00000350: 0000 7215 0000 0072 1600 0000 da03 646f  ..r....r......do
-00000360: 63da 0273 69da 0473 656e 7472 0d00 0000  c..si..sentr....
-00000370: 720d 0000 0072 1400 0000 da14 5f69 7465  r....r......_ite
-00000380: 725f 7465 7874 5f73 656e 7465 6e63 6573  r_text_sentences
-00000390: 1200 0000 730c 0000 0002 800a 0112 010e  ....s...........
-000003a0: 0108 0104 fe7a 2153 7061 6379 4d61 7463  .....z!SpacyMatc
-000003b0: 6865 722e 5f69 7465 725f 7465 7874 5f73  her._iter_text_s
-000003c0: 656e 7465 6e63 6573 da0e 7365 6e74 656e  entences..senten
-000003d0: 6365 5f69 6e64 6578 da08 7365 6e74 656e  ce_index..senten
-000003e0: 6365 da06 7265 7475 726e 6304 0000 0000  ce..returnc.....
-000003f0: 0000 0000 0000 0007 0000 0007 0000 0043  ...............C
-00000400: 0000 0073 8000 0000 7c00 a000 a100 0100  ...s....|.......
-00000410: 7401 7c02 7402 8302 720e 7c00 a003 7c02  t.|.t...r.|...|.
-00000420: a101 7d02 7c02 6a04 7c00 5f05 7c01 7c00  ..}.|.j.|._.|.|.
-00000430: 5f06 7c03 7c00 5f07 7408 7c02 8301 4400  _.|.|._.t.|...D.
-00000440: 5d21 5c02 7d04 7d05 7409 7c05 6a04 7c04  ]!\.}.}.t.|.j.|.
-00000450: 7c05 6a0a 7c05 6a0b a00c a100 6401 8d04  |.j.|.j.....d...
-00000460: 7d06 7c00 a00d 7c06 a101 0100 7c05 6a0e  }.|...|.....|.j.
-00000470: 733d 7c00 a00f 7c05 6a04 7c05 6a0a a102  s=|...|.j.|.j...
-00000480: 0100 711c 6400 5300 2902 4e29 04da 0477  ..q.d.S.).N)...w
-00000490: 6f72 64da 0569 6e64 6578 da05 6c65 6d6d  ord..index..lemm
-000004a0: 61da 0370 6f73 2910 da0f 5f72 6573 6574  a..pos)..._reset
-000004b0: 5f73 656e 7465 6e63 65da 0a69 7369 6e73  _sentence..isins
-000004c0: 7461 6e63 65da 0373 7472 720a 0000 0072  tance..strr....r
-000004d0: 1500 0000 da0f 7365 6e74 656e 6365 5f73  ......sentence_s
-000004e0: 7472 696e 6772 1f00 0000 7216 0000 0072  tringr....r....r
-000004f0: 1800 0000 7207 0000 00da 066c 656d 6d61  ....r......lemma
-00000500: 5fda 0470 6f73 5fda 056c 6f77 6572 da13  _..pos_..lower..
-00000510: 5f61 6464 5f73 656e 7465 6e63 655f 746f  _add_sentence_to
-00000520: 6b65 6eda 0769 735f 7374 6f70 da13 6164  ken..is_stop..ad
-00000530: 645f 6361 6e64 6964 6174 655f 7275 6c65  d_candidate_rule
-00000540: 7329 0772 1000 0000 721f 0000 0072 2000  s).r....r....r .
-00000550: 0000 7216 0000 0072 1c00 0000 da0b 7370  ..r....r......sp
-00000560: 6163 795f 746f 6b65 6eda 0574 6f6b 656e  acy_token..token
-00000570: 720d 0000 0072 0d00 0000 7214 0000 0072  r....r....r....r
-00000580: 1a00 0000 1800 0000 7324 0000 0008 010a  ........s$......
-00000590: 010a 0108 0106 0106 0110 0102 0104 0102  ................
-000005a0: 0104 0108 0106 fc0a 0606 0110 0102 8004  ................
-000005b0: f77a 1a53 7061 6379 4d61 7463 6865 722e  .z.SpacyMatcher.
-000005c0: 5f73 6574 5f73 656e 7465 6e63 6529 0272  _set_sentence).r
-000005d0: 0900 0000 4e72 1700 0000 290e da08 5f5f  ....Nr....)...__
-000005e0: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
-000005f0: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
-00000600: da05 7370 6163 79da 086c 616e 6775 6167  ..spacy..languag
-00000610: 6572 2800 0000 7206 0000 0072 0f00 0000  er(...r....r....
-00000620: 721e 0000 00da 0369 6e74 7203 0000 00da  r......intr.....
-00000630: 0d53 7061 6379 5365 6e74 656e 6365 721a  .SpacySentencer.
-00000640: 0000 00da 0d5f 5f63 6c61 7373 6365 6c6c  .....__classcell
-00000650: 5f5f 720d 0000 0072 0d00 0000 7212 0000  __r....r....r...
-00000660: 0072 1400 0000 7208 0000 000a 0000 0073  .r....r........s
-00000670: 0800 0000 0800 1e02 1406 2a06 7208 0000  ..........*.r...
-00000680: 0029 0eda 0674 7970 696e 6772 0200 0000  .)...typingr....
-00000690: 7203 0000 0072 3500 0000 5a0c 7370 6163  r....r5...Z.spac
-000006a0: 792e 746f 6b65 6e73 7204 0000 0072 3800  y.tokensr....r8.
-000006b0: 0000 5a1d 7265 6164 696e 675f 696d 7061  ..Z.reading_impa
-000006c0: 6374 5f6d 6f64 656c 2e6d 6174 6368 6572  ct_model.matcher
-000006d0: 7372 0500 0000 da21 7265 6164 696e 675f  sr.....!reading_
-000006e0: 696d 7061 6374 5f6d 6f64 656c 2e69 6d70  impact_model.imp
-000006f0: 6163 745f 6d6f 6465 6c72 0600 0000 7207  act_modelr....r.
-00000700: 0000 00da 0d49 6d70 6163 744d 6174 6368  .....ImpactMatch
-00000710: 6572 7208 0000 0072 0d00 0000 720d 0000  err....r....r...
-00000720: 0072 0d00 0000 7214 0000 00da 083c 6d6f  .r....r......<mo
-00000730: 6475 6c65 3e01 0000 0073 0c00 0000 1000  dule>....s......
-00000740: 0802 0c01 0c02 1001 1603                 ..........
+00000110: 6505 6604 640a 640b 8405 5a08 0902 0902  e.f.d.d...Z.....
+00000120: 6413 640c 6509 6505 650a 6602 1900 640d  d.d.e.e.e.f...d.
+00000130: 650b 6409 6505 640e 6402 6608 640f 6410  e.d.e.d.d.f.d.d.
+00000140: 8405 5a0c 8700 0400 5a0d 5300 2914 da0c  ..Z.....Z.S.)...
+00000150: 5370 6163 794d 6174 6368 6572 da02 656e  SpacyMatcher..en
+00000160: 4eda 0670 6172 7365 72da 046c 616e 67da  N..parser..lang.
+00000170: 0c69 6d70 6163 745f 6d6f 6465 6c63 0400  .impact_modelc..
+00000180: 0000 0000 0000 0000 0000 0500 0000 0500  ................
+00000190: 0000 0b00 0000 7328 0000 0074 0083 006a  ......s(...t...j
+000001a0: 0164 027c 027c 0364 019c 027c 04a4 018e  .d.|.|.d...|....
+000001b0: 0101 007c 017c 005f 027c 027c 005f 0364  ...|.|._.|.|._.d
+000001c0: 0053 0029 034e 2902 720b 0000 0072 0c00  .S.).N).r....r..
+000001d0: 0000 a900 2904 da05 7375 7065 72da 085f  ....)...super.._
+000001e0: 5f69 6e69 745f 5f72 0a00 0000 720b 0000  _init__r....r...
+000001f0: 0029 05da 0473 656c 6672 0a00 0000 720b  .)...selfr....r.
+00000200: 0000 0072 0c00 0000 da06 6b77 6172 6773  ...r......kwargs
+00000210: a901 da09 5f5f 636c 6173 735f 5f72 0d00  ....__class__r..
+00000220: 0000 fa73 2f55 7365 7273 2f6d 6172 696a  ...s/Users/marij
+00000230: 6e6b 6f6f 6c65 6e2f 4461 7461 2f50 726f  nkoolen/Data/Pro
+00000240: 6a65 6374 732f 542d 5265 6373 2f41 7070  jects/T-Recs/App
+00000250: 6561 6c2f 7265 6164 696e 672d 696d 7061  eal/reading-impa
+00000260: 6374 2d6d 6f64 656c 2f72 6561 6469 6e67  ct-model/reading
+00000270: 5f69 6d70 6163 745f 6d6f 6465 6c2f 6d61  _impact_model/ma
+00000280: 7463 6865 7273 2f73 7061 6379 5f6d 6174  tchers/spacy_mat
+00000290: 6368 6572 2e70 7972 0f00 0000 0c00 0000  cher.pyr........
+000002a0: 7306 0000 0018 0206 010a 017a 1553 7061  s..........z.Spa
+000002b0: 6379 4d61 7463 6865 722e 5f5f 696e 6974  cyMatcher.__init
+000002c0: 5f5f da04 7465 7874 da06 646f 635f 6964  __..text..doc_id
+000002d0: 6303 0000 0000 0000 0000 0000 0006 0000  c...............
+000002e0: 0006 0000 0063 0000 0073 3800 0000 8100  .....c...s8.....
+000002f0: 7c00 a000 7c01 a101 7d03 7401 7c03 6a02  |...|...}.t.|.j.
+00000300: 8301 4400 5d0e 5c02 7d04 7d05 7c00 a003  ..D.].\.}.}.|...
+00000310: 7c05 7c04 7c02 a103 0100 7c04 5600 0100  |.|.|.....|.V...
+00000320: 710b 6400 5300 a901 4e29 0472 0a00 0000  q.d.S...N).r....
+00000330: da09 656e 756d 6572 6174 65da 0573 656e  ..enumerate..sen
+00000340: 7473 da0d 5f73 6574 5f73 656e 7465 6e63  ts.._set_sentenc
+00000350: 6529 0672 1000 0000 7215 0000 0072 1600  e).r....r....r..
+00000360: 0000 da03 646f 63da 0273 69da 0473 656e  ....doc..si..sen
+00000370: 7472 0d00 0000 720d 0000 0072 1400 0000  tr....r....r....
+00000380: da14 5f69 7465 725f 7465 7874 5f73 656e  .._iter_text_sen
+00000390: 7465 6e63 6573 1200 0000 730c 0000 0002  tences....s.....
+000003a0: 800a 0112 010e 0108 0104 fe7a 2153 7061  ...........z!Spa
+000003b0: 6379 4d61 7463 6865 722e 5f69 7465 725f  cyMatcher._iter_
+000003c0: 7465 7874 5f73 656e 7465 6e63 6573 da08  text_sentences..
+000003d0: 7365 6e74 656e 6365 da0e 7365 6e74 656e  sentence..senten
+000003e0: 6365 5f69 6e64 6578 da06 7265 7475 726e  ce_index..return
+000003f0: 6304 0000 0000 0000 0000 0000 0007 0000  c...............
+00000400: 0007 0000 0043 0000 0073 8000 0000 7c00  .....C...s....|.
+00000410: a000 a100 0100 7401 7c01 7402 8302 720e  ......t.|.t...r.
+00000420: 7c00 a003 7c01 a101 7d01 7c01 6a04 7c00  |...|...}.|.j.|.
+00000430: 5f05 7c02 7c00 5f06 7c03 7c00 5f07 7408  _.|.|._.|.|._.t.
+00000440: 7c01 8301 4400 5d21 5c02 7d04 7d05 7409  |...D.]!\.}.}.t.
+00000450: 7c05 6a04 7c04 7c05 6a0a 7c05 6a0b a00c  |.j.|.|.j.|.j...
+00000460: a100 6401 8d04 7d06 7c00 a00d 7c06 a101  ..d...}.|...|...
+00000470: 0100 7c05 6a0e 733d 7c00 a00f 7c05 6a04  ..|.j.s=|...|.j.
+00000480: 7c05 6a0a a102 0100 711c 6400 5300 2902  |.j.....q.d.S.).
+00000490: 4e29 04da 0477 6f72 64da 0569 6e64 6578  N)...word..index
+000004a0: da05 6c65 6d6d 61da 0370 6f73 2910 da0f  ..lemma..pos)...
+000004b0: 5f72 6573 6574 5f73 656e 7465 6e63 65da  _reset_sentence.
+000004c0: 0a69 7369 6e73 7461 6e63 65da 0373 7472  .isinstance..str
+000004d0: 720a 0000 0072 1500 0000 da0f 7365 6e74  r....r......sent
+000004e0: 656e 6365 5f73 7472 696e 6772 2000 0000  ence_stringr ...
+000004f0: 7216 0000 0072 1800 0000 7207 0000 00da  r....r....r.....
+00000500: 066c 656d 6d61 5fda 0470 6f73 5fda 056c  .lemma_..pos_..l
+00000510: 6f77 6572 da13 5f61 6464 5f73 656e 7465  ower.._add_sente
+00000520: 6e63 655f 746f 6b65 6eda 0769 735f 7374  nce_token..is_st
+00000530: 6f70 da13 6164 645f 6361 6e64 6964 6174  op..add_candidat
+00000540: 655f 7275 6c65 7329 0772 1000 0000 721f  e_rules).r....r.
+00000550: 0000 0072 2000 0000 7216 0000 0072 1c00  ...r ...r....r..
+00000560: 0000 5a0b 7370 6163 795f 746f 6b65 6eda  ..Z.spacy_token.
+00000570: 0574 6f6b 656e 720d 0000 0072 0d00 0000  .tokenr....r....
+00000580: 7214 0000 0072 1a00 0000 1800 0000 7324  r....r........s$
+00000590: 0000 0008 030a 010a 0108 0106 0106 0110  ................
+000005a0: 0102 0104 0102 0104 0108 0106 fc0a 0606  ................
+000005b0: 0110 0102 8004 f77a 1a53 7061 6379 4d61  .......z.SpacyMa
+000005c0: 7463 6865 722e 5f73 6574 5f73 656e 7465  tcher._set_sente
+000005d0: 6e63 6529 0272 0900 0000 4e72 1700 0000  nce).r....Nr....
+000005e0: 2902 4e4e 290e da08 5f5f 6e61 6d65 5f5f  ).NN)...__name__
+000005f0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+00000600: 7175 616c 6e61 6d65 5f5f da05 7370 6163  qualname__..spac
+00000610: 79da 086c 616e 6775 6167 6572 2800 0000  y..languager(...
+00000620: 7206 0000 0072 0f00 0000 721e 0000 0072  r....r....r....r
+00000630: 0300 0000 da0d 5370 6163 7953 656e 7465  ......SpacySente
+00000640: 6e63 65da 0369 6e74 721a 0000 00da 0d5f  nce..intr......_
+00000650: 5f63 6c61 7373 6365 6c6c 5f5f 720d 0000  _classcell__r...
+00000660: 0072 0d00 0000 7212 0000 0072 1400 0000  .r....r....r....
+00000670: 7208 0000 000a 0000 0073 1800 0000 0800  r........s......
+00000680: 1e02 1406 0207 0201 10fe 0201 02ff 0202  ................
+00000690: 02fe 0202 12fe 7208 0000 0029 0eda 0674  ......r....)...t
+000006a0: 7970 696e 6772 0200 0000 7203 0000 0072  ypingr....r....r
+000006b0: 3400 0000 5a0c 7370 6163 792e 746f 6b65  4...Z.spacy.toke
+000006c0: 6e73 7204 0000 0072 3600 0000 da1d 7265  nsr....r6.....re
+000006d0: 6164 696e 675f 696d 7061 6374 5f6d 6f64  ading_impact_mod
+000006e0: 656c 2e6d 6174 6368 6572 7372 0500 0000  el.matchersr....
+000006f0: da21 7265 6164 696e 675f 696d 7061 6374  .!reading_impact
+00000700: 5f6d 6f64 656c 2e69 6d70 6163 745f 6d6f  _model.impact_mo
+00000710: 6465 6c72 0600 0000 7207 0000 00da 0d49  delr....r......I
+00000720: 6d70 6163 744d 6174 6368 6572 7208 0000  mpactMatcherr...
+00000730: 0072 0d00 0000 720d 0000 0072 0d00 0000  .r....r....r....
+00000740: 7214 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00000750: 0000 0073 0c00 0000 1000 0802 0c01 0c02  ...s............
+00000760: 1001 1603                                ....
```

### Comparing `reading_impact_model-1.0.1/reading_impact_model/matchers/alpino_matcher.py` & `reading_impact_model-1.0.2/reading_impact_model/matchers/alpino_matcher.py`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.1/reading_impact_model/matchers/alpinor_matcher_old.py` & `reading_impact_model-1.0.2/reading_impact_model/matchers/alpinor_matcher_old.py`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.1/reading_impact_model/matchers/matcher.py` & `reading_impact_model-1.0.2/reading_impact_model/matchers/matcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,22 +135,24 @@
             self.sentence_vocab_terms[vocab_terms].add(token)
         elif isinstance(vocab_terms, set):
             for vocab_term in vocab_terms:
                 self.sentence_vocab_terms[vocab_term].add(token)
 
     def _set_dict_sentence(self, sentence: Dict[str, any], sentence_index: int, doc_id: str) -> None:
         self.sentence_string = sentence['text']
+        self.sentence_index = sentence_index
         self.sentence_id = (sentence_index, doc_id) if sentence_index and doc_id else None
         for ti, token in enumerate(sentence['tokens']):
             token = Token(word=token.word, index=ti, lemma=token.lemma, pos=token.pos if 'pos' in token else None)
             self._add_sentence_token(token)
             self.add_candidate_rules(token.word, token.lemma)
 
     def _set_string_sentence(self, sentence: str, sentence_index: int, doc_id: str) -> None:
         self.sentence_string = sentence
+        self.sentence_index = sentence_index
         self.sentence_id = (sentence_index, doc_id) if sentence_index and doc_id else None
         words = re.split(r'\W+', sentence)
         for wi, word in enumerate(words):
             token = Token(word, wi, lemma=word)
             self._add_sentence_token(token)
             self.add_candidate_rules(word, word)
         # print('sentence_string:', self.sentence_string)
@@ -173,14 +175,17 @@
         else:
             raise TypeError(
                 "sentence must be either a string, an Sentence object from Alpino, Spacy or Stanza.")
 
     def _iter_text_sentences(self, text: str, doc_id: str = None):
         for si, sent in enumerate(sent_tokenize(text)):
             self._set_sentence(sent, sentence_index=si, doc_id=doc_id)
+            if self.debug:
+                print('_iter_text_sentence - si:', si)
+                print('_iter_text_sentence - self.sentence_index:', self.sentence_index)
             yield si
 
     def analyse_text(self, text: str, doc_id: str = None,
                      include_neutral: bool = False) -> List[Dict[str, any]]:
         all_matches = []
         for _ in self._iter_text_sentences(text, doc_id):
             sentence_matches = self._match_rules()
@@ -266,22 +271,25 @@
     def find_impact_matches(self, sentence):
         """Return all matching impact rules for a given sentence."""
         self._set_sentence(sentence)
         return self._match_rules()
 
     def _match_rules(self):
         """Match sentence against all impact rules of the impact model."""
+        if self.debug:
+            print('_match_rules - sentence_index:', self.sentence_index)
         return [match for impact_rule in self.candidate_rules for match in self.match_rule(impact_rule)]
 
-    def match_rule(self, impact_rule: ImpactRule, sentence=None) -> List[ImpactMatch]:
+    def match_rule(self, impact_rule: ImpactRule, sentence=None, sentence_index: int = None,
+                   doc_id: str = None) -> List[ImpactMatch]:
         """Match sentence against a specific impact rule."""
         if sentence:
             if self.debug:
                 print('setting sentence for single rule match')
-            self._set_sentence(sentence)
+            self._set_sentence(sentence, sentence_index=sentence_index, doc_id=doc_id)
         if impact_rule.impact_term.type == "phrase":
             return self.match_impact_phrase(impact_rule)
         if impact_rule.impact_term.type == "regex":
             return self.match_impact_phrase(impact_rule)
         else:
             return self.match_impact_term(impact_rule)
```

### Comparing `reading_impact_model-1.0.1/reading_impact_model/matchers/nltk_matcher.py` & `reading_impact_model-1.0.2/reading_impact_model/matchers/nltk_matcher.py`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.1/reading_impact_model/matchers/spacy_matcher.py` & `reading_impact_model-1.0.2/reading_impact_model/matchers/spacy_matcher.py`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.1/reading_impact_model/matchers/stanza_matcher.py` & `reading_impact_model-1.0.2/reading_impact_model/matchers/stanza_matcher.py`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.1/reading_impact_model/matchers/trankit_matcher.py` & `reading_impact_model-1.0.2/reading_impact_model/matchers/trankit_matcher.py`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.1/reading_impact_model/model/phrase.py` & `reading_impact_model-1.0.2/reading_impact_model/model/phrase.py`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.1/reading_impact_model/models/__pycache__/impact_model_en.cpython-310.pyc` & `reading_impact_model-1.0.2/reading_impact_model/models/__pycache__/impact_model_en.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.1/reading_impact_model/models/__pycache__/impact_model_nl.cpython-310.pyc` & `reading_impact_model-1.0.2/reading_impact_model/models/__pycache__/impact_model_nl.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.1/reading_impact_model/models/impact_model-en-0.1.pcl` & `reading_impact_model-1.0.2/reading_impact_model/models/impact_model-en-0.1.pcl`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.1/reading_impact_model/models/impact_model-en-0.2.pcl` & `reading_impact_model-1.0.2/reading_impact_model/models/impact_model-en-0.2.pcl`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.1/reading_impact_model/models/impact_model-en-0.3.pcl` & `reading_impact_model-1.0.2/reading_impact_model/models/impact_model-en-0.3.pcl`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.1/reading_impact_model/models/impact_model-en-0.4.pcl` & `reading_impact_model-1.0.2/reading_impact_model/models/impact_model-en-0.4.pcl`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.1/reading_impact_model/models/impact_model-en-0.5.pcl` & `reading_impact_model-1.0.2/reading_impact_model/models/impact_model-en-0.5.pcl`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.1/reading_impact_model/models/impact_model-en-0.6.json` & `reading_impact_model-1.0.2/reading_impact_model/models/impact_model-en-0.6.json`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.1/reading_impact_model/models/impact_model-en-0.6.pcl` & `reading_impact_model-1.0.2/reading_impact_model/models/impact_model-en-0.6.pcl`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.1/reading_impact_model/models/impact_model-en-0.7.json` & `reading_impact_model-1.0.2/reading_impact_model/models/impact_model-en-0.7.json`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.1/reading_impact_model/models/impact_model-en-0.7.pcl` & `reading_impact_model-1.0.2/reading_impact_model/models/impact_model-en-0.7.pcl`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.1/reading_impact_model/models/impact_model-en.json` & `reading_impact_model-1.0.2/reading_impact_model/models/impact_model-en.json`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.1/reading_impact_model/models/impact_model-en.pcl` & `reading_impact_model-1.0.2/reading_impact_model/models/impact_model-en.pcl`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.1/reading_impact_model/models/impact_model-nl-1.0.json` & `reading_impact_model-1.0.2/reading_impact_model/models/impact_model-nl-1.0.json`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.1/reading_impact_model/models/impact_model-nl.json` & `reading_impact_model-1.0.2/reading_impact_model/models/impact_model-nl.json`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.1/reading_impact_model/models/impact_model-nl.pcl` & `reading_impact_model-1.0.2/reading_impact_model/models/impact_model-nl.pcl`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.1/reading_impact_model/models/impact_model_en.py` & `reading_impact_model-1.0.2/reading_impact_model/models/impact_model_en.py`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.1/reading_impact_model/models/impact_model_nl.py` & `reading_impact_model-1.0.2/reading_impact_model/models/impact_model_nl.py`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.1/reading_impact_model/reading_impact.py` & `reading_impact_model-1.0.2/reading_impact_model/reading_impact.py`

 * *Files identical despite different names*

### Comparing `reading_impact_model-1.0.1/PKG-INFO` & `reading_impact_model-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reading-impact-model
-Version: 1.0.1
+Version: 1.0.2
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
-Metadata-Version: 2.1 Name: reading-impact-model Version: 1.0.1 Summary: Home-
+Metadata-Version: 2.1 Name: reading-impact-model Version: 1.0.2 Summary: Home-
 page: https://github.com/marijnkoolen/reading-impact-model License: MIT Author:
 Marijn Koolen Author-email: marijn.koolen@gmail.com Requires-Python:
 >=3.10,<4.0 Classifier: Development Status :: 4 - Beta Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Topic :: Scientific/
```

