# Comparing `tmp/kalpy-kaldi-0.0.5.tar.gz` & `tmp/kalpy-kaldi-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kalpy-kaldi-0.0.5.tar", last modified: Sat Jun  3 21:44:23 2023, max compression
+gzip compressed data, was "kalpy-kaldi-0.0.6.tar", last modified: Wed Jun  7 06:48:55 2023, max compression
```

## Comparing `kalpy-kaldi-0.0.5.tar` & `kalpy-kaldi-0.0.6.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:44:23.619857 kalpy-kaldi-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:44:23.599857 kalpy-kaldi-0.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:44:23.603857 kalpy-kaldi-0.0.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:44:23.603857 kalpy-kaldi-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-03 21:44:23.619857 kalpy-kaldi-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:44:23.603857 kalpy-kaldi-0.0.5/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/extensions/_kalpy.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:44:23.603857 kalpy-kaldi-0.0.5/extensions/chain/
--rw-r--r--   0 runner    (1001) docker     (123)    10529 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/extensions/chain/chain.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/extensions/chain/pybind_chain.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:44:23.603857 kalpy-kaldi-0.0.5/extensions/cudamatrix/
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/extensions/cudamatrix/cudamatrix.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/extensions/cudamatrix/pybind_cudamatrix.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:44:23.603857 kalpy-kaldi-0.0.5/extensions/decoder/
--rw-r--r--   0 runner    (1001) docker     (123)    85592 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/extensions/decoder/decoder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/extensions/decoder/pybind_decoder.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:44:23.607858 kalpy-kaldi-0.0.5/extensions/feat/
--rw-r--r--   0 runner    (1001) docker     (123)    18729 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/extensions/feat/feat.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/extensions/feat/pybind_feat.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:44:23.607858 kalpy-kaldi-0.0.5/extensions/fstext/
--rw-r--r--   0 runner    (1001) docker     (123)    73561 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/extensions/fstext/fstext.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    12465 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/extensions/fstext/pybind_fstext.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:44:23.607858 kalpy-kaldi-0.0.5/extensions/gmm/
--rw-r--r--   0 runner    (1001) docker     (123)    53595 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/extensions/gmm/gmm.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/extensions/gmm/pybind_gmm.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:44:23.607858 kalpy-kaldi-0.0.5/extensions/hmm/
--rw-r--r--   0 runner    (1001) docker     (123)    13229 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/extensions/hmm/hmm.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/extensions/hmm/pybind_hmm.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:44:23.607858 kalpy-kaldi-0.0.5/extensions/itf/
--rw-r--r--   0 runner    (1001) docker     (123)    15497 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/extensions/itf/itf.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/extensions/itf/pybind_itf.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:44:23.607858 kalpy-kaldi-0.0.5/extensions/ivector/
--rw-r--r--   0 runner    (1001) docker     (123)    28267 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/extensions/ivector/ivector.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/extensions/ivector/pybind_ivector.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:44:23.607858 kalpy-kaldi-0.0.5/extensions/kws/
--rw-r--r--   0 runner    (1001) docker     (123)     9952 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/extensions/kws/kws.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/extensions/kws/pybind_kws.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:44:23.607858 kalpy-kaldi-0.0.5/extensions/lat/
--rw-r--r--   0 runner    (1001) docker     (123)    63329 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/extensions/lat/lat.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/extensions/lat/pybind_lat.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:44:23.611858 kalpy-kaldi-0.0.5/extensions/lm/
--rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/extensions/lm/lm.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/extensions/lm/pybind_lm.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:44:23.611858 kalpy-kaldi-0.0.5/extensions/matrix/
--rw-r--r--   0 runner    (1001) docker     (123)    13191 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/extensions/matrix/matrix.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/extensions/matrix/pybind_matrix.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:44:23.611858 kalpy-kaldi-0.0.5/extensions/nnet/
--rw-r--r--   0 runner    (1001) docker     (123)    78126 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/extensions/nnet/nnet.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/extensions/nnet/pybind_nnet.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:44:23.611858 kalpy-kaldi-0.0.5/extensions/nnet2/
--rw-r--r--   0 runner    (1001) docker     (123)   122159 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/extensions/nnet2/nnet2.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/extensions/nnet2/pybind_nnet2.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:44:23.611858 kalpy-kaldi-0.0.5/extensions/nnet3/
--rw-r--r--   0 runner    (1001) docker     (123)    12428 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/extensions/nnet3/nnet3.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/extensions/nnet3/pybind_nnet3.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:44:23.611858 kalpy-kaldi-0.0.5/extensions/online/
--rw-r--r--   0 runner    (1001) docker     (123)    20930 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/extensions/online/online.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/extensions/online/pybind_online.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:44:23.611858 kalpy-kaldi-0.0.5/extensions/online2/
--rw-r--r--   0 runner    (1001) docker     (123)    72778 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/extensions/online2/online2.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/extensions/online2/pybind_online2.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:44:23.611858 kalpy-kaldi-0.0.5/extensions/pybind/
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/extensions/pybind/kaldi_pybind.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:44:23.611858 kalpy-kaldi-0.0.5/extensions/rnnlm/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/extensions/rnnlm/pybind_rnnlm.h
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/extensions/rnnlm/rnnlm.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:44:23.611858 kalpy-kaldi-0.0.5/extensions/transform/
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/extensions/transform/pybind_transform.h
--rw-r--r--   0 runner    (1001) docker     (123)    39892 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/extensions/transform/transform.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:44:23.611858 kalpy-kaldi-0.0.5/extensions/tree/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/extensions/tree/pybind_tree.h
--rw-r--r--   0 runner    (1001) docker     (123)    52285 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/extensions/tree/tree.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:44:23.615857 kalpy-kaldi-0.0.5/extensions/util/
--rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/extensions/util/pybind_util.h
--rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/extensions/util/util.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:44:23.615857 kalpy-kaldi-0.0.5/kalpy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/kalpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-03 21:44:23.000000 kalpy-kaldi-0.0.5/kalpy/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:44:23.615857 kalpy-kaldi-0.0.5/kalpy/decoder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/kalpy/decoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/kalpy/decoder/training_graphs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:44:23.615857 kalpy-kaldi-0.0.5/kalpy/feat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/kalpy/feat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/kalpy/feat/mfcc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:44:23.615857 kalpy-kaldi-0.0.5/kalpy/fstext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/kalpy/fstext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19552 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/kalpy/fstext/lexicon.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/kalpy/fstext/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:44:23.615857 kalpy-kaldi-0.0.5/kalpy_kaldi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-03 21:44:23.000000 kalpy-kaldi-0.0.5/kalpy_kaldi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-06-03 21:44:23.000000 kalpy-kaldi-0.0.5/kalpy_kaldi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 21:44:23.000000 kalpy-kaldi-0.0.5/kalpy_kaldi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 21:44:23.000000 kalpy-kaldi-0.0.5/kalpy_kaldi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-03 21:44:23.000000 kalpy-kaldi-0.0.5/kalpy_kaldi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-03 21:44:23.000000 kalpy-kaldi-0.0.5/kalpy_kaldi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 21:44:23.619857 kalpy-kaldi-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:44:23.619857 kalpy-kaldi-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:44:23.603857 kalpy-kaldi-0.0.5/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:44:23.619857 kalpy-kaldi-0.0.5/tests/data/acoustic_models/
--rw-r--r--   0 runner    (1001) docker     (123)    55713 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/tests/data/acoustic_models/final.mdl
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/tests/data/acoustic_models/tree
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:44:23.619857 kalpy-kaldi-0.0.5/tests/data/dictionaries/
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/tests/data/dictionaries/test_basic.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:44:23.619857 kalpy-kaldi-0.0.5/tests/data/wav/
--rw-r--r--   0 runner    (1001) docker     (123)   855188 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/tests/data/wav/acoustic_corpus.wav
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/tests/test_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/tests/test_hmm.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/tests/test_mfcc.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-03 21:43:53.000000 kalpy-kaldi-0.0.5/tests/test_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:48:55.481334 kalpy-kaldi-0.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:48:55.457334 kalpy-kaldi-0.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:48:55.461334 kalpy-kaldi-0.0.6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:48:55.461334 kalpy-kaldi-0.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-07 06:48:55.481334 kalpy-kaldi-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:48:55.461334 kalpy-kaldi-0.0.6/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/extensions/_kalpy.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:48:55.461334 kalpy-kaldi-0.0.6/extensions/chain/
+-rw-r--r--   0 runner    (1001) docker     (123)    10529 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/extensions/chain/chain.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/extensions/chain/pybind_chain.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:48:55.465334 kalpy-kaldi-0.0.6/extensions/cudamatrix/
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/extensions/cudamatrix/cudamatrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/extensions/cudamatrix/pybind_cudamatrix.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:48:55.465334 kalpy-kaldi-0.0.6/extensions/decoder/
+-rw-r--r--   0 runner    (1001) docker     (123)    85592 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/extensions/decoder/decoder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/extensions/decoder/pybind_decoder.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:48:55.465334 kalpy-kaldi-0.0.6/extensions/feat/
+-rw-r--r--   0 runner    (1001) docker     (123)    18729 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/extensions/feat/feat.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/extensions/feat/pybind_feat.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:48:55.465334 kalpy-kaldi-0.0.6/extensions/fstext/
+-rw-r--r--   0 runner    (1001) docker     (123)    73561 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/extensions/fstext/fstext.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    12465 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/extensions/fstext/pybind_fstext.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:48:55.465334 kalpy-kaldi-0.0.6/extensions/gmm/
+-rw-r--r--   0 runner    (1001) docker     (123)    53595 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/extensions/gmm/gmm.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/extensions/gmm/pybind_gmm.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:48:55.465334 kalpy-kaldi-0.0.6/extensions/hmm/
+-rw-r--r--   0 runner    (1001) docker     (123)    13229 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/extensions/hmm/hmm.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/extensions/hmm/pybind_hmm.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:48:55.465334 kalpy-kaldi-0.0.6/extensions/itf/
+-rw-r--r--   0 runner    (1001) docker     (123)    15497 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/extensions/itf/itf.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/extensions/itf/pybind_itf.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:48:55.465334 kalpy-kaldi-0.0.6/extensions/ivector/
+-rw-r--r--   0 runner    (1001) docker     (123)    28267 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/extensions/ivector/ivector.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/extensions/ivector/pybind_ivector.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:48:55.465334 kalpy-kaldi-0.0.6/extensions/kws/
+-rw-r--r--   0 runner    (1001) docker     (123)     9952 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/extensions/kws/kws.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/extensions/kws/pybind_kws.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:48:55.469334 kalpy-kaldi-0.0.6/extensions/lat/
+-rw-r--r--   0 runner    (1001) docker     (123)    63329 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/extensions/lat/lat.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/extensions/lat/pybind_lat.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:48:55.469334 kalpy-kaldi-0.0.6/extensions/lm/
+-rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/extensions/lm/lm.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/extensions/lm/pybind_lm.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:48:55.469334 kalpy-kaldi-0.0.6/extensions/matrix/
+-rw-r--r--   0 runner    (1001) docker     (123)    13191 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/extensions/matrix/matrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/extensions/matrix/pybind_matrix.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:48:55.469334 kalpy-kaldi-0.0.6/extensions/nnet/
+-rw-r--r--   0 runner    (1001) docker     (123)    78126 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/extensions/nnet/nnet.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/extensions/nnet/pybind_nnet.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:48:55.469334 kalpy-kaldi-0.0.6/extensions/nnet2/
+-rw-r--r--   0 runner    (1001) docker     (123)   122159 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/extensions/nnet2/nnet2.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/extensions/nnet2/pybind_nnet2.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:48:55.469334 kalpy-kaldi-0.0.6/extensions/nnet3/
+-rw-r--r--   0 runner    (1001) docker     (123)    12428 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/extensions/nnet3/nnet3.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/extensions/nnet3/pybind_nnet3.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:48:55.469334 kalpy-kaldi-0.0.6/extensions/online/
+-rw-r--r--   0 runner    (1001) docker     (123)    20930 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/extensions/online/online.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/extensions/online/pybind_online.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:48:55.469334 kalpy-kaldi-0.0.6/extensions/online2/
+-rw-r--r--   0 runner    (1001) docker     (123)    72778 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/extensions/online2/online2.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/extensions/online2/pybind_online2.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:48:55.469334 kalpy-kaldi-0.0.6/extensions/pybind/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/extensions/pybind/kaldi_pybind.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:48:55.473334 kalpy-kaldi-0.0.6/extensions/rnnlm/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/extensions/rnnlm/pybind_rnnlm.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/extensions/rnnlm/rnnlm.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:48:55.473334 kalpy-kaldi-0.0.6/extensions/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/extensions/transform/pybind_transform.h
+-rw-r--r--   0 runner    (1001) docker     (123)    39892 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/extensions/transform/transform.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:48:55.473334 kalpy-kaldi-0.0.6/extensions/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/extensions/tree/pybind_tree.h
+-rw-r--r--   0 runner    (1001) docker     (123)    52285 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/extensions/tree/tree.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:48:55.473334 kalpy-kaldi-0.0.6/extensions/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/extensions/util/pybind_util.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/extensions/util/util.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:48:55.473334 kalpy-kaldi-0.0.6/kalpy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/kalpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-07 06:48:55.000000 kalpy-kaldi-0.0.6/kalpy/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:48:55.473334 kalpy-kaldi-0.0.6/kalpy/decoder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/kalpy/decoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/kalpy/decoder/training_graphs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:48:55.473334 kalpy-kaldi-0.0.6/kalpy/feat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/kalpy/feat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/kalpy/feat/mfcc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:48:55.473334 kalpy-kaldi-0.0.6/kalpy/fstext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/kalpy/fstext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19552 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/kalpy/fstext/lexicon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/kalpy/fstext/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:48:55.477334 kalpy-kaldi-0.0.6/kalpy_kaldi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-07 06:48:55.000000 kalpy-kaldi-0.0.6/kalpy_kaldi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-06-07 06:48:55.000000 kalpy-kaldi-0.0.6/kalpy_kaldi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 06:48:55.000000 kalpy-kaldi-0.0.6/kalpy_kaldi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 06:48:55.000000 kalpy-kaldi-0.0.6/kalpy_kaldi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-07 06:48:55.000000 kalpy-kaldi-0.0.6/kalpy_kaldi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-07 06:48:55.000000 kalpy-kaldi-0.0.6/kalpy_kaldi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 06:48:55.481334 kalpy-kaldi-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6481 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:48:55.477334 kalpy-kaldi-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:48:55.461334 kalpy-kaldi-0.0.6/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:48:55.477334 kalpy-kaldi-0.0.6/tests/data/acoustic_models/
+-rw-r--r--   0 runner    (1001) docker     (123)    55713 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/tests/data/acoustic_models/final.mdl
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/tests/data/acoustic_models/tree
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:48:55.477334 kalpy-kaldi-0.0.6/tests/data/dictionaries/
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/tests/data/dictionaries/test_basic.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:48:55.477334 kalpy-kaldi-0.0.6/tests/data/wav/
+-rw-r--r--   0 runner    (1001) docker     (123)   855188 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/tests/data/wav/acoustic_corpus.wav
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/tests/test_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/tests/test_hmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/tests/test_mfcc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-07 06:48:30.000000 kalpy-kaldi-0.0.6/tests/test_tree.py
```

### Comparing `kalpy-kaldi-0.0.5/.github/ISSUE_TEMPLATE/bug_report.md` & `kalpy-kaldi-0.0.6/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/.github/ISSUE_TEMPLATE/feature_request.md` & `kalpy-kaldi-0.0.6/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/.github/workflows/main.yml` & `kalpy-kaldi-0.0.6/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/.github/workflows/publish.yml` & `kalpy-kaldi-0.0.6/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/.gitignore` & `kalpy-kaldi-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/.pre-commit-config.yaml` & `kalpy-kaldi-0.0.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/CMakeLists.txt` & `kalpy-kaldi-0.0.6/CMakeLists.txt`

 * *Files 4% similar despite different names*

```diff
@@ -46,28 +46,16 @@
     endforeach()
  elseif(APPLE)
      set(CMAKE_INSTALL_RPATH "@loader_path")
  else()
      set(CMAKE_INSTALL_RPATH "$ORIGIN;$ORIGIN/../lib;$ORIGIN/../../tools/openfst/lib")
 endif ()
 
-#find_package(CUDAToolkit)
-#find_package(CUDA)
-#if(CUDA_FOUND)
-#    add_definitions(-DHAVE_CUDA=1)
-#else()
-#   add_definitions(-DHAVE_CUDA=0)
-#endif()
 find_package(CUDA)
 
-if(CUDA_FOUND)
-
-#add_definitions(-DHAVE_CUDA=1)
-endif()
-
 find_package(pybind11 REQUIRED)
 include_directories(extensions)
 pybind11_add_module(_kalpy extensions/_kalpy.cpp
                             extensions/chain/chain.cpp
                             extensions/cudamatrix/cudamatrix.cpp
                             extensions/decoder/decoder.cpp
                             extensions/feat/feat.cpp
@@ -106,15 +94,15 @@
                                     kaldi-tree
                                     kaldi-util
                                     fst
                                     )
 
 if(CUDA_FOUND)
 
-target_link_libraries(_kalpy PUBLIC kaldi-cudadecoder kaldi-cudafeat
+   target_link_libraries(_kalpy PUBLIC kaldi-cudadecoder kaldi-cudafeat
                                     )
 endif()
 target_compile_definitions(_kalpy
                            PRIVATE VERSION_INFO="5.5.1068")
 if(MSVC)
 set_target_properties(_kalpy PROPERTIES
     DEFINE_SYMBOL "KALDI_DLL_IMPORTS"
```

### Comparing `kalpy-kaldi-0.0.5/LICENSE` & `kalpy-kaldi-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/PKG-INFO` & `kalpy-kaldi-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: kalpy-kaldi
-Version: 0.0.5
+Version: 0.0.6
 Summary: Pybind11 bindings for Kaldi for use with the Montreal Forced Aligner
 Author: Michael McAuliffe
 Author-email: michael.e.mcauliffe@gmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # kalpy
-Pybind11 bindings for Kaldi for use in [Montreal Forced Aligner](montreal-forced-aligner.readthedocs.io/)
+Pybind11 bindings for Kaldi for use in [Montreal Forced Aligner](montreal-forced-aligner.readthedocs.io/).
 
 ## Installation
 
 Kalpy depends on Kaldi being built as shared libraries, and the easiest way to install is via conda-forge:
 
 ```
 conda install -c conda-forge kalpy
```

### Comparing `kalpy-kaldi-0.0.5/README.md` & `kalpy-kaldi-0.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # kalpy
-Pybind11 bindings for Kaldi for use in [Montreal Forced Aligner](montreal-forced-aligner.readthedocs.io/)
+Pybind11 bindings for Kaldi for use in [Montreal Forced Aligner](montreal-forced-aligner.readthedocs.io/).
 
 ## Installation
 
 Kalpy depends on Kaldi being built as shared libraries, and the easiest way to install is via conda-forge:
 
 ```
 conda install -c conda-forge kalpy
```

### Comparing `kalpy-kaldi-0.0.5/extensions/_kalpy.cpp` & `kalpy-kaldi-0.0.6/extensions/_kalpy.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/extensions/chain/chain.cpp` & `kalpy-kaldi-0.0.6/extensions/chain/chain.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/extensions/chain/pybind_chain.h` & `kalpy-kaldi-0.0.6/extensions/chain/pybind_chain.h`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/extensions/cudamatrix/cudamatrix.cpp` & `kalpy-kaldi-0.0.6/extensions/cudamatrix/cudamatrix.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/extensions/decoder/decoder.cpp` & `kalpy-kaldi-0.0.6/extensions/decoder/decoder.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/extensions/decoder/pybind_decoder.h` & `kalpy-kaldi-0.0.6/extensions/decoder/pybind_decoder.h`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/extensions/feat/feat.cpp` & `kalpy-kaldi-0.0.6/extensions/feat/feat.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/extensions/fstext/fstext.cpp` & `kalpy-kaldi-0.0.6/extensions/fstext/fstext.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/extensions/fstext/pybind_fstext.h` & `kalpy-kaldi-0.0.6/extensions/fstext/pybind_fstext.h`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/extensions/gmm/gmm.cpp` & `kalpy-kaldi-0.0.6/extensions/gmm/gmm.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/extensions/gmm/pybind_gmm.h` & `kalpy-kaldi-0.0.6/extensions/gmm/pybind_gmm.h`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/extensions/hmm/hmm.cpp` & `kalpy-kaldi-0.0.6/extensions/hmm/hmm.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/extensions/itf/itf.cpp` & `kalpy-kaldi-0.0.6/extensions/itf/itf.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/extensions/ivector/ivector.cpp` & `kalpy-kaldi-0.0.6/extensions/ivector/ivector.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/extensions/kws/kws.cpp` & `kalpy-kaldi-0.0.6/extensions/kws/kws.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/extensions/lat/lat.cpp` & `kalpy-kaldi-0.0.6/extensions/lat/lat.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/extensions/lat/pybind_lat.h` & `kalpy-kaldi-0.0.6/extensions/lat/pybind_lat.h`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/extensions/lm/lm.cpp` & `kalpy-kaldi-0.0.6/extensions/lm/lm.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/extensions/matrix/matrix.cpp` & `kalpy-kaldi-0.0.6/extensions/matrix/matrix.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/extensions/nnet/nnet.cpp` & `kalpy-kaldi-0.0.6/extensions/nnet/nnet.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/extensions/nnet/pybind_nnet.h` & `kalpy-kaldi-0.0.6/extensions/nnet/pybind_nnet.h`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/extensions/nnet2/nnet2.cpp` & `kalpy-kaldi-0.0.6/extensions/nnet2/nnet2.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/extensions/nnet2/pybind_nnet2.h` & `kalpy-kaldi-0.0.6/extensions/nnet2/pybind_nnet2.h`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/extensions/nnet3/nnet3.cpp` & `kalpy-kaldi-0.0.6/extensions/nnet3/nnet3.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/extensions/nnet3/pybind_nnet3.h` & `kalpy-kaldi-0.0.6/extensions/nnet3/pybind_nnet3.h`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/extensions/online/online.cpp` & `kalpy-kaldi-0.0.6/extensions/online/online.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/extensions/online2/online2.cpp` & `kalpy-kaldi-0.0.6/extensions/online2/online2.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/extensions/online2/pybind_online2.h` & `kalpy-kaldi-0.0.6/extensions/online2/pybind_online2.h`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/extensions/pybind/kaldi_pybind.h` & `kalpy-kaldi-0.0.6/extensions/pybind/kaldi_pybind.h`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/extensions/rnnlm/pybind_rnnlm.h` & `kalpy-kaldi-0.0.6/extensions/rnnlm/pybind_rnnlm.h`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/extensions/rnnlm/rnnlm.cpp` & `kalpy-kaldi-0.0.6/extensions/rnnlm/rnnlm.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/extensions/transform/pybind_transform.h` & `kalpy-kaldi-0.0.6/extensions/transform/pybind_transform.h`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/extensions/transform/transform.cpp` & `kalpy-kaldi-0.0.6/extensions/transform/transform.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/extensions/tree/tree.cpp` & `kalpy-kaldi-0.0.6/extensions/tree/tree.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/extensions/util/pybind_util.h` & `kalpy-kaldi-0.0.6/extensions/util/pybind_util.h`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/extensions/util/util.cpp` & `kalpy-kaldi-0.0.6/extensions/util/util.cpp`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/kalpy/decoder/training_graphs.py` & `kalpy-kaldi-0.0.6/kalpy/decoder/training_graphs.py`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/kalpy/feat/mfcc.py` & `kalpy-kaldi-0.0.6/kalpy/feat/mfcc.py`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/kalpy/fstext/lexicon.py` & `kalpy-kaldi-0.0.6/kalpy/fstext/lexicon.py`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/kalpy/fstext/utils.py` & `kalpy-kaldi-0.0.6/kalpy/fstext/utils.py`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/kalpy_kaldi.egg-info/PKG-INFO` & `kalpy-kaldi-0.0.6/kalpy_kaldi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: kalpy-kaldi
-Version: 0.0.5
+Version: 0.0.6
 Summary: Pybind11 bindings for Kaldi for use with the Montreal Forced Aligner
 Author: Michael McAuliffe
 Author-email: michael.e.mcauliffe@gmail.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # kalpy
-Pybind11 bindings for Kaldi for use in [Montreal Forced Aligner](montreal-forced-aligner.readthedocs.io/)
+Pybind11 bindings for Kaldi for use in [Montreal Forced Aligner](montreal-forced-aligner.readthedocs.io/).
 
 ## Installation
 
 Kalpy depends on Kaldi being built as shared libraries, and the easiest way to install is via conda-forge:
 
 ```
 conda install -c conda-forge kalpy
```

### Comparing `kalpy-kaldi-0.0.5/kalpy_kaldi.egg-info/SOURCES.txt` & `kalpy-kaldi-0.0.6/kalpy_kaldi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/pyproject.toml` & `kalpy-kaldi-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/setup.py` & `kalpy-kaldi-0.0.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,36 +53,37 @@
         # Adding CMake arguments set as environment variable
         # (needed e.g. to build for ARM OSx on conda-forge)
         if "CMAKE_ARGS" in os.environ:
             cmake_args += [item for item in os.environ["CMAKE_ARGS"].split(" ") if item]
 
         # In this example, we pass in the version to C++. You might not need to.
 
-        if not cmake_generator or cmake_generator == "Ninja":
-            try:
-                import ninja
-
-                ninja_executable_path = Path(ninja.BIN_DIR) / "ninja"
-                cmake_args += [
-                    "-GNinja",
-                    f"-DCMAKE_MAKE_PROGRAM:FILEPATH={ninja_executable_path}",
-                ]
-            except ImportError:
-                pass
         if self.compiler.compiler_type != "msvc":
             # Using Ninja-build since it a) is available as a wheel and b)
             # multithreads automatically. MSVC would require all variables be
             # exported for Ninja to pick it up, which is a little tricky to do.
             # Users can override the generator with CMAKE_GENERATOR in CMake
             # 3.15+.
             kaldi_root = os.environ.get("KALDI_ROOT", None)
             if kaldi_root:
                 cmake_args += [f"-DKALDI_ROOT={kaldi_root}"]
+            if not cmake_generator or cmake_generator == "Ninja":
+                try:
+                    import ninja
+
+                    ninja_executable_path = Path(ninja.BIN_DIR) / "ninja"
+                    cmake_args += [
+                        "-GNinja",
+                        f"-DCMAKE_MAKE_PROGRAM:FILEPATH={ninja_executable_path}",
+                    ]
+                except ImportError:
+                    pass
 
         else:
+            cmake_args += ["-GNinja"]
             # Single config generators are handled "normally"
             kaldi_root = os.environ.get("KALDI_ROOT", None)
             if kaldi_root:
                 kaldi_root = kaldi_root.replace("\\", "/")
                 cmake_args += [f"-DKALDI_ROOT={kaldi_root}"]
             single_config = any(x in cmake_generator for x in {"NMake", "Ninja"})
```

### Comparing `kalpy-kaldi-0.0.5/tests/conftest.py` & `kalpy-kaldi-0.0.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/tests/data/acoustic_models/final.mdl` & `kalpy-kaldi-0.0.6/tests/data/acoustic_models/final.mdl`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/tests/data/acoustic_models/tree` & `kalpy-kaldi-0.0.6/tests/data/acoustic_models/tree`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/tests/data/dictionaries/test_basic.txt` & `kalpy-kaldi-0.0.6/tests/data/dictionaries/test_basic.txt`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/tests/data/wav/acoustic_corpus.wav` & `kalpy-kaldi-0.0.6/tests/data/wav/acoustic_corpus.wav`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/tests/test_decoder.py` & `kalpy-kaldi-0.0.6/tests/test_decoder.py`

 * *Files identical despite different names*

### Comparing `kalpy-kaldi-0.0.5/tests/test_mfcc.py` & `kalpy-kaldi-0.0.6/tests/test_mfcc.py`

 * *Files identical despite different names*

