# Comparing `tmp/acids-msprior-1.1.0.tar.gz` & `tmp/acids-msprior-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acids-msprior-1.1.0.tar", last modified: Mon May 22 12:04:36 2023, max compression
+gzip compressed data, was "acids-msprior-1.1.1.tar", last modified: Wed Jun  7 12:55:12 2023, max compression
```

## Comparing `acids-msprior-1.1.0.tar` & `acids-msprior-1.1.1.tar`

### file list

```diff
@@ -1,39 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:04:36.407917 acids-msprior-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-05-22 12:04:36.407917 acids-msprior-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:04:36.399917 acids-msprior-1.1.0/acids_msprior.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-05-22 12:04:36.000000 acids-msprior-1.1.0/acids_msprior.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-22 12:04:36.000000 acids-msprior-1.1.0/acids_msprior.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 12:04:36.000000 acids-msprior-1.1.0/acids_msprior.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-22 12:04:36.000000 acids-msprior-1.1.0/acids_msprior.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-22 12:04:36.000000 acids-msprior-1.1.0/acids_msprior.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-22 12:04:36.000000 acids-msprior-1.1.0/acids_msprior.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:04:36.403917 acids-msprior-1.1.0/msprior/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/msprior/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19972 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/msprior/attention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:04:36.403917 acids-msprior-1.1.0/msprior/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/msprior/configs/decoder_only.gin
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/msprior/configs/encoder_decoder.gin
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/msprior/configs/encoder_decoder_continuous.gin
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/msprior/configs/recurrent.gin
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/msprior/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/msprior/preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/msprior/scripted.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/msprior/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/msprior/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:04:36.407917 acids-msprior-1.1.0/msprior_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/msprior_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/msprior_scripts/compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/msprior_scripts/export.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/msprior_scripts/main_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/msprior_scripts/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/msprior_scripts/train.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 12:04:36.407917 acids-msprior-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:04:36.407917 acids-msprior-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/tests/test_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-22 12:01:21.000000 acids-msprior-1.1.0/tests/test_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:55:12.887970 acids-msprior-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-06-07 12:55:12.887970 acids-msprior-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:55:12.879970 acids-msprior-1.1.1/acids_msprior.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-06-07 12:55:12.000000 acids-msprior-1.1.1/acids_msprior.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-07 12:55:12.000000 acids-msprior-1.1.1/acids_msprior.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 12:55:12.000000 acids-msprior-1.1.1/acids_msprior.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-07 12:55:12.000000 acids-msprior-1.1.1/acids_msprior.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-07 12:55:12.000000 acids-msprior-1.1.1/acids_msprior.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-07 12:55:12.000000 acids-msprior-1.1.1/acids_msprior.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:55:12.879970 acids-msprior-1.1.1/msprior/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/msprior/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20823 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/msprior/attention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:55:12.883970 acids-msprior-1.1.1/msprior/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/msprior/configs/decoder_only.gin
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/msprior/configs/encoder_decoder.gin
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/msprior/configs/encoder_decoder_continuous.gin
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/msprior/configs/flattened.gin
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/msprior/configs/recurrent.gin
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/msprior/configs/rwkv.gin
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/msprior/configs/rwkv_semantic.gin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:55:12.883970 acids-msprior-1.1.1/msprior/cuda/
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/msprior/cuda/wkv_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/msprior/cuda/wkv_op.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/msprior/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/msprior/preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12734 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/msprior/rwkv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11112 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/msprior/scripted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/msprior/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/msprior/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:55:12.883970 acids-msprior-1.1.1/msprior_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/msprior_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/msprior_scripts/combine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/msprior_scripts/compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/msprior_scripts/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/msprior_scripts/main_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/msprior_scripts/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/msprior_scripts/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 12:55:12.887970 acids-msprior-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:55:12.887970 acids-msprior-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/tests/test_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/tests/test_configs.py
```

### Comparing `acids-msprior-1.1.0/PKG-INFO` & `acids-msprior-1.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acids-msprior
-Version: 1.1.0
+Version: 1.1.1
 Summary: MSPRIOR: A multiscale prior model for realtime temporal learning
 Author: Antoine CAILLON
 Author-email: caillon@ircam.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
@@ -101,7 +101,13 @@
 ### 4. Realtime usage
 
 Once exported, you can load the model inside MaxMSP following the image below.
 
 ![Max Msp usage](docs/maxmsp_usage.png)
 
 Note that additional inputs (e.g. semantic) are only available when using seq2seq models. The last output yields the perplexity of the model.
+
+## Funding
+
+This work is funded by the DAFNE+ N° 101061548 project, and is led at IRCAM in the STMS lab.
+
+<img src="https://ec.europa.eu/regional_policy/images/information-sources/logo-download-center/eu_co_funded_en.jpg" width=200px/>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: acids-msprior Version: 1.1.0 Summary: MSPRIOR: A
+Metadata-Version: 2.1 Name: acids-msprior Version: 1.1.1 Summary: MSPRIOR: A
 multiscale prior model for realtime temporal learning Author: Antoine CAILLON
 Author-email: caillon@ircam.fr Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.9 Description-Content-Type: text/
 markdown # MSPrior ### A multi(scale/stream) prior model for realtime temporal
 learning ## Disclaimer This is an experimental project that *will* be subject
 to lots of changes. ## Installation ```bash pip install acids-msprior ``` ##
@@ -39,8 +39,11 @@
 github.com/acids-ircam/nn_tilde). ```bash msprior export --run /path/to/your/
 run ``` **WARNING** If you are training on top of a *continuous* rave (i.e.
 anything but the `discrete` configuration), you shoud pass the `--continuous`
 flag during export ```bash msprior export --run /path/to/your/run --continuous
 ``` ### 4. Realtime usage Once exported, you can load the model inside MaxMSP
 following the image below. ![Max Msp usage](docs/maxmsp_usage.png) Note that
 additional inputs (e.g. semantic) are only available when using seq2seq models.
-The last output yields the perplexity of the model.
+The last output yields the perplexity of the model. ## Funding This work is
+funded by the DAFNE+ NÂ° 101061548 project, and is led at IRCAM in the STMS
+lab. [https://ec.europa.eu/regional_policy/images/information-sources/logo-
+download-center/eu_co_funded_en.jpg]
```

### Comparing `acids-msprior-1.1.0/README.md` & `acids-msprior-1.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -88,8 +88,14 @@
 
 ### 4. Realtime usage
 
 Once exported, you can load the model inside MaxMSP following the image below.
 
 ![Max Msp usage](docs/maxmsp_usage.png)
 
-Note that additional inputs (e.g. semantic) are only available when using seq2seq models. The last output yields the perplexity of the model.
+Note that additional inputs (e.g. semantic) are only available when using seq2seq models. The last output yields the perplexity of the model.
+
+## Funding
+
+This work is funded by the DAFNE+ N° 101061548 project, and is led at IRCAM in the STMS lab.
+
+<img src="https://ec.europa.eu/regional_policy/images/information-sources/logo-download-center/eu_co_funded_en.jpg" width=200px/>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -34,8 +34,11 @@
 github.com/acids-ircam/nn_tilde). ```bash msprior export --run /path/to/your/
 run ``` **WARNING** If you are training on top of a *continuous* rave (i.e.
 anything but the `discrete` configuration), you shoud pass the `--continuous`
 flag during export ```bash msprior export --run /path/to/your/run --continuous
 ``` ### 4. Realtime usage Once exported, you can load the model inside MaxMSP
 following the image below. ![Max Msp usage](docs/maxmsp_usage.png) Note that
 additional inputs (e.g. semantic) are only available when using seq2seq models.
-The last output yields the perplexity of the model.
+The last output yields the perplexity of the model. ## Funding This work is
+funded by the DAFNE+ NÂ° 101061548 project, and is led at IRCAM in the STMS
+lab. [https://ec.europa.eu/regional_policy/images/information-sources/logo-
+download-center/eu_co_funded_en.jpg]
```

### Comparing `acids-msprior-1.1.0/acids_msprior.egg-info/PKG-INFO` & `acids-msprior-1.1.1/acids_msprior.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acids-msprior
-Version: 1.1.0
+Version: 1.1.1
 Summary: MSPRIOR: A multiscale prior model for realtime temporal learning
 Author: Antoine CAILLON
 Author-email: caillon@ircam.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
@@ -101,7 +101,13 @@
 ### 4. Realtime usage
 
 Once exported, you can load the model inside MaxMSP following the image below.
 
 ![Max Msp usage](docs/maxmsp_usage.png)
 
 Note that additional inputs (e.g. semantic) are only available when using seq2seq models. The last output yields the perplexity of the model.
+
+## Funding
+
+This work is funded by the DAFNE+ N° 101061548 project, and is led at IRCAM in the STMS lab.
+
+<img src="https://ec.europa.eu/regional_policy/images/information-sources/logo-download-center/eu_co_funded_en.jpg" width=200px/>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: acids-msprior Version: 1.1.0 Summary: MSPRIOR: A
+Metadata-Version: 2.1 Name: acids-msprior Version: 1.1.1 Summary: MSPRIOR: A
 multiscale prior model for realtime temporal learning Author: Antoine CAILLON
 Author-email: caillon@ircam.fr Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.9 Description-Content-Type: text/
 markdown # MSPrior ### A multi(scale/stream) prior model for realtime temporal
 learning ## Disclaimer This is an experimental project that *will* be subject
 to lots of changes. ## Installation ```bash pip install acids-msprior ``` ##
@@ -39,8 +39,11 @@
 github.com/acids-ircam/nn_tilde). ```bash msprior export --run /path/to/your/
 run ``` **WARNING** If you are training on top of a *continuous* rave (i.e.
 anything but the `discrete` configuration), you shoud pass the `--continuous`
 flag during export ```bash msprior export --run /path/to/your/run --continuous
 ``` ### 4. Realtime usage Once exported, you can load the model inside MaxMSP
 following the image below. ![Max Msp usage](docs/maxmsp_usage.png) Note that
 additional inputs (e.g. semantic) are only available when using seq2seq models.
-The last output yields the perplexity of the model.
+The last output yields the perplexity of the model. ## Funding This work is
+funded by the DAFNE+ NÂ° 101061548 project, and is led at IRCAM in the STMS
+lab. [https://ec.europa.eu/regional_policy/images/information-sources/logo-
+download-center/eu_co_funded_en.jpg]
```

### Comparing `acids-msprior-1.1.0/acids_msprior.egg-info/SOURCES.txt` & `acids-msprior-1.1.1/acids_msprior.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -8,22 +8,29 @@
 acids_msprior.egg-info/entry_points.txt
 acids_msprior.egg-info/requires.txt
 acids_msprior.egg-info/top_level.txt
 msprior/__init__.py
 msprior/attention.py
 msprior/dataset.py
 msprior/preprocessor.py
+msprior/rwkv.py
 msprior/scripted.py
 msprior/task.py
 msprior/utils.py
 msprior/configs/decoder_only.gin
 msprior/configs/encoder_decoder.gin
 msprior/configs/encoder_decoder_continuous.gin
+msprior/configs/flattened.gin
 msprior/configs/recurrent.gin
+msprior/configs/rwkv.gin
+msprior/configs/rwkv_semantic.gin
+msprior/cuda/wkv_cuda.cu
+msprior/cuda/wkv_op.cpp
 msprior_scripts/__init__.py
+msprior_scripts/combine.py
 msprior_scripts/compact.py
 msprior_scripts/export.py
 msprior_scripts/main_cli.py
 msprior_scripts/preprocess.py
 msprior_scripts/train.py
 tests/__init__.py
 tests/test_attention.py
```

### Comparing `acids-msprior-1.1.0/msprior/attention.py` & `acids-msprior-1.1.1/msprior/attention.py`

 * *Files 2% similar despite different names*

```diff
@@ -331,28 +331,43 @@
             x = self.proj(x)
 
         return x
 
 
 class Embedding(nn.Embedding):
 
-    def forward(self, input: torch.Tensor) -> torch.Tensor:
+    def forward(self,
+                input: torch.Tensor,
+                sum_over_quantizers: Optional[bool] = None) -> torch.Tensor:
         input = input.long()
 
         return nn.functional.embedding(input, self.weight, self.padding_idx,
                                        self.max_norm, self.norm_type,
                                        self.scale_grad_by_freq, self.sparse)
 
 
+class LogitsProjection(nn.Module):
+
+    def __init__(self, dim: int, num_tokens: int, **kwargs) -> None:
+        super().__init__()
+        self.net = nn.Sequential(nn.GELU(), nn.Linear(dim, num_tokens))
+
+    def forward(self, inputs: torch.Tensor, *args, **kwargs) -> torch.Tensor:
+        return self.net(inputs)
+
+
 class FeatureEmbedding(nn.Module):
 
     def __init__(self, in_features: int, out_features: int) -> None:
         super().__init__()
         self.norm = nn.BatchNorm1d(in_features)
-        self.net = nn.Linear(in_features, out_features)
+        self.net = nn.Sequential(
+            nn.Linear(in_features, out_features),
+            nn.LayerNorm(out_features),
+        )
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         x = self.norm(x.permute(0, 2, 1))
         return self.net(x.permute(0, 2, 1))
 
 
 class IndividualPredictor(nn.Module):
@@ -360,15 +375,16 @@
     def __init__(self, dim: int, num_tokens: int, first_quantizer: bool,
                  dropout: float) -> None:
         super().__init__()
         self.predictor = nn.Sequential(nn.GELU(), nn.Linear(dim, num_tokens))
         self.dropout = nn.Dropout(dropout)
 
         if not first_quantizer:
-            self.film = nn.Linear(dim, 2 * dim)
+            self.film = nn.Sequential(nn.Linear(dim, dim), nn.GELU(),
+                                      nn.Linear(dim, 2 * dim))
         else:
             self.film = None
 
     def forward(self,
                 context: torch.Tensor,
                 previous_embedding: Optional[torch.Tensor] = None):
 
@@ -519,22 +535,26 @@
 @gin.configurable
 class Prior(pl.LightningModule):
 
     def __init__(
         self,
         decoder_factory: Callable[[], Decoder],
         encoder_factory: Optional[Callable[[], Encoder]] = None,
+        inputs_preprocessing: Optional[Callable[[TensorDict],
+                                                TensorDict]] = None,
     ) -> None:
         super().__init__()
 
         self.encoder = None
         if encoder_factory is not None:
             self.encoder = encoder_factory()
         self.decoder = decoder_factory()
 
+        self.inputs_preprocessing = inputs_preprocessing
+
     def forward(
         self,
         x: torch.Tensor,
         y: Optional[torch.Tensor] = None,
         targets: Optional[torch.Tensor] = None,
     ) -> torch.Tensor:
         if self.encoder is not None:
@@ -555,14 +575,17 @@
         return self.decoder.sample(
             x,
             encoder_out,
             temperature=temperature,
         )
 
     def loss(self, inputs: TensorDict) -> torch.Tensor:
+        if self.inputs_preprocessing is not None:
+            inputs = self.inputs_preprocessing(inputs)
+
         logits = self.forward(
             inputs["decoder_inputs"],
             inputs["encoder_inputs"],
             inputs["decoder_targets"],
         )
 
         targets_one_hot = nn.functional.one_hot(
```

### Comparing `acids-msprior-1.1.0/msprior/configs/decoder_only.gin` & `acids-msprior-1.1.1/msprior/configs/decoder_only.gin`

 * *Files 11% similar despite different names*

```diff
@@ -69,8 +69,9 @@
     betas = (.9, .99)
 
 dataset.SequenceDataset:
     task_fn = @task.decoder_only_rave
 
 task.decoder_only_rave:
     seq_len = %SEQ_LEN
-    decoder_key = "rave"
+    decoder_key = "rave"
+    quantizer_crop = %NUM_QUANTIZERS
```

### Comparing `acids-msprior-1.1.0/msprior/configs/encoder_decoder.gin` & `acids-msprior-1.1.1/msprior/configs/encoder_decoder.gin`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.1.0/msprior/configs/encoder_decoder_continuous.gin` & `acids-msprior-1.1.1/msprior/configs/encoder_decoder_continuous.gin`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.1.0/msprior/dataset.py` & `acids-msprior-1.1.1/msprior/dataset.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.1.0/msprior/preprocessor.py` & `acids-msprior-1.1.1/msprior/preprocessor.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.1.0/msprior/scripted.py` & `acids-msprior-1.1.1/msprior/scripted.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import cached_conv as cc
 import gin
 import nn_tilde
 import torch
 
 from .attention import Embedding, FeatureEmbedding, Prior
+from .rwkv import RWKV
 
 
 class ScriptedPrior(nn_tilde.Module):
 
     def __init__(
         self,
         run: Optional[str] = None,
@@ -36,15 +37,19 @@
 
         if run is not None:
             ckpts = pathlib.Path(run).rglob("*.ckpt")
             ckpts = map(str, ckpts)
             ckpts = sorted(ckpts, key=lambda x: "last" in x, reverse=True)
             ckpt = next(iter(ckpts))
             ckpt = torch.load(ckpt, map_location="cpu")["state_dict"]
-            model.load_state_dict(ckpt)
+            if isinstance(model.decoder.net[0], RWKV):
+                for k, v in ckpt.items():
+                    if ".time" in k:
+                        ckpt[k] = v.reshape(-1)
+            model.load_state_dict(ckpt, strict=False)
 
         model.eval()
 
         self.encoder = model.encoder
         self.decoder = model.decoder
 
         # RETRIEVE INPUT/OUTPUT DETAILS
@@ -59,16 +64,22 @@
         num_inputs = self.num_rave_quantizers
         self.encoder_input_type = "none"
         self.encoder_num_tokens = 0
         self.feature_vae = None
         self.from_continuous = from_continuous
 
         if self.has_encoder:
-            encoder_embedder = gin.get_bindings(
-                "attention.Encoder")["embedder"]
+            encoder_ratio = 1
+            try:
+                encoder_embedder = gin.get_bindings(
+                    "attention.Encoder")["embedder"]
+            except ValueError:
+                encoder_embedder = gin.get_bindings(
+                    "attention.Prior")["encoder_factory"]
+
             if isinstance(encoder_embedder(), Embedding):
                 num_inputs += 1
                 self.encoder_num_tokens = gin.get_bindings(
                     "encoder/attention.Embedding")["num_embeddings"]
                 self.encoder_input_type = "discrete"
             elif isinstance(encoder_embedder(), FeatureEmbedding):
                 if vae_path is not None:
@@ -80,16 +91,21 @@
                         "attention.FeatureEmbedding")["in_features"]
                     num_inputs += feature_dim
                     self.encoder_input_type = "full"
             else:
                 raise ValueError(
                     f"Unknown encoder embedder {encoder_embedder}")
 
-            self.encoder_ratio = gin.get_bindings(
-                "decoder/attention.TransformerLayer")["encoder_out_ratio"]
+            try:
+                encoder_ratio = gin.get_bindings(
+                    "decoder/attention.TransformerLayer")["encoder_out_ratio"]
+            except KeyError:
+                pass
+
+            self.encoder_ratio = encoder_ratio
 
         input_labels = [
             f"rave latent {i+1}" for i in range(self.num_rave_quantizers)
         ]
 
         if self.encoder_input_type == "none":
             pass
@@ -145,15 +161,15 @@
                 self.encoder_ratio * temporal_ratio,
                 1,
                 self.encoder_ratio * temporal_ratio,
             )
 
     def apply_full_reset(self):
         for n, b in self.named_buffers():
-            if "_cache_length" in n or "_relative_index" in n or "_state" in n:
+            if "_cache_length" in n or "_relative_index" in n or "_state" in n or "last_" in n:
                 b.zero_()
         self.set_reset(False)
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
         batch_size = x.shape[0]
         input_rave = x[:, :self.num_rave_quantizers]
```

### Comparing `acids-msprior-1.1.0/msprior/utils.py` & `acids-msprior-1.1.1/msprior/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 import gin
 import numpy as np
 import torch
 import torch.nn as nn
 
 # GIN UTILS
 
+TensorDict = Dict[str, torch.Tensor]
+
 
 def get_feed_forward_size(model_dim):
     return 4 * model_dim
 
 
 @gin.configurable
 def build_warmed_exponential_lr_scheduler(
@@ -225,24 +227,54 @@
             f(inputs)
 
     return composed_function
 
 
 # OTHERS
 
-# def sample_from_logits(logits: torch.Tensor,
-#                        temperature: float = 0.) -> torch.Tensor:
-#     assert temperature >= 0
-#     dist = torch.softmax(logits / (temperature + 1e-15), -1)
-#     dist = dist.reshape(-1, dist.shape[-1])
-#     samples = torch.multinomial(dist, 1).reshape_as(logits[..., 0])
-#     return samples
-
 
 def sample_from_logits(logits: torch.Tensor,
                        temperature: float = 0.) -> torch.Tensor:
     if temperature != 0:
         logits = torch.log_softmax(logits / temperature, -1)
         logits -= torch.empty_like(logits).exponential_().log()
 
     samples = torch.argmax(logits, -1)
     return samples
+
+
+# CONTINUOUS FEATURE RECONSTRUCTION
+
+
+def semantic_vae_processing(
+        vae_path: Optional[str] = None
+) -> Callable[[torch.Tensor], torch.Tensor]:
+
+    if vae_path is None:
+        return lambda x: x
+
+    vae = torch.jit.load(vae_path).eval()
+    state = list(
+        map(lambda nv: nv[1],
+            filter(
+                lambda nv: "_state" in nv[0],
+                vae.named_buffers(),
+            )))
+
+    def reset():
+        for elm in state:
+            elm.zero_()
+
+    @torch.no_grad()
+    def vae_processing(inputs: TensorDict) -> TensorDict:
+        reset()
+        vae.to(inputs["encoder_inputs"].device)
+        reconstruction = vae.forward(
+            inputs["encoder_inputs"],
+            context=inputs["decoder_inputs"],
+        )
+
+        inputs["encoder_inputs"] = reconstruction
+
+        return inputs
+
+    return vae_processing
```

### Comparing `acids-msprior-1.1.0/msprior_scripts/compact.py` & `acids-msprior-1.1.1/msprior_scripts/compact.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.1.0/msprior_scripts/export.py` & `acids-msprior-1.1.1/msprior_scripts/export.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 
 from msprior.scripted import ScriptedPrior
 
 torch.set_grad_enabled(False)
 
 
 def main(argv):
-    # DUE TO THE COMPUTATIONAL COMPLEXITY OF THE MODEL, RESTRICTING TO A BATCH_SIZE OF 1
-    cc.MAX_BATCH_SIZE = 1
+    cc.MAX_BATCH_SIZE = FLAGS.batch_size
     cc.use_cached_conv(True)
 
     model = ScriptedPrior(
         run=FLAGS.run,
         temporal_ratio=FLAGS.temporal_ratio,
         from_continuous=FLAGS.continuous,
         vae_path=FLAGS.vae_path,
@@ -26,14 +25,15 @@
     model.export_to_ts(export_path)
     print(f'model exported to {export_path}')
 
 
 FLAGS = flags.FLAGS
 flags.DEFINE_string('run', default=None, required=True, help='Run to export')
 flags.DEFINE_string('vae_path', default=None, help='Pretrained semantic VAE')
+flags.DEFINE_integer('batch_size', default=1, help='Maximum batch size')
 flags.DEFINE_integer(
     'temporal_ratio',
     default=1024,
     help='Sequence temporal ratio',
 )
 flags.DEFINE_bool(
     'continuous',
```

### Comparing `acids-msprior-1.1.0/msprior_scripts/main_cli.py` & `acids-msprior-1.1.1/msprior_scripts/main_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import importlib
 import sys
 
 from absl import app
 
-AVAILABLE_SCRIPTS = ['preprocess', 'train', 'export', 'compact']
+AVAILABLE_SCRIPTS = ['preprocess', 'train', 'export', 'compact', 'combine']
 
 
 def help():
     print(f"""usage: msprior [ {' | '.join(AVAILABLE_SCRIPTS)} ]
 
 positional arguments:
   command     Command to launch with msprior.
```

### Comparing `acids-msprior-1.1.0/msprior_scripts/preprocess.py` & `acids-msprior-1.1.1/msprior_scripts/preprocess.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.1.0/msprior_scripts/train.py` & `acids-msprior-1.1.1/msprior_scripts/train.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from torch.utils import data
 
 from msprior.attention import Prior
 from msprior.dataset import SequenceDataset
 
 FLAGS = flags.FLAGS
 flags.DEFINE_multi_string("config",
-                          default="msprior/configs/decoder_only.gin",
+                          default="decoder_only",
                           help="config to parse.")
 flags.DEFINE_string("db_path",
                     default=None,
                     required=True,
                     help="path to dataset.")
 flags.DEFINE_integer("val_size",
                      default=8192,
@@ -64,19 +64,19 @@
     logging.info("loading dataset")
     dataset = SequenceDataset(db_path=FLAGS.db_path)
     train, val = data.random_split(
         dataset,
         (len(dataset) - FLAGS.val_size, FLAGS.val_size),
         generator=torch.Generator().manual_seed(42),
     )
-
-    logging.info("quantizer number retrieval")
-    with gin.unlock_config():
-        gin.parse_config(
-            f"NUM_QUANTIZERS={train[0]['decoder_inputs'].shape[-1]}")
+    if not any(map(lambda x: "flattened" in x, FLAGS.config)):
+        logging.info("quantizer number retrieval")
+        with gin.unlock_config():
+            gin.parse_config(
+                f"NUM_QUANTIZERS={train[0]['decoder_inputs'].shape[-1]}")
 
     logging.info("building model")
     model = Prior()
 
     train_loader = data.DataLoader(
         train,
         batch_size=FLAGS.batch_size,
@@ -88,15 +88,15 @@
         val,
         batch_size=FLAGS.batch_size,
         shuffle=False,
         drop_last=False,
         num_workers=FLAGS.workers,
     )
 
-    os.makedirs(os.path.join("runs", FLAGS.name), exist_ok=False)
+    os.makedirs(os.path.join("runs", FLAGS.name), exist_ok=True)
     with open(os.path.join("runs", FLAGS.name, "config.gin"),
               "w") as config_out:
         config_out.write(gin.config_str())
 
     val_check = {}
     if len(train_loader) >= FLAGS.val_every:
         val_check["val_check_interval"] = FLAGS.val_every
@@ -112,15 +112,15 @@
         callbacks=[
             callbacks.LearningRateMonitor(logging_interval='step'),
             callbacks.ModelCheckpoint(monitor="val_cross_entropy",
                                       filename='best'),
             callbacks.ModelCheckpoint(filename='last'),
             callbacks.EarlyStopping(
                 "val_cross_entropy",
-                patience=10,
+                patience=20,
             )
         ],
         log_every_n_steps=10,
         **val_check,
     )
 
     torch.backends.cudnn.benchmark = True
```

### Comparing `acids-msprior-1.1.0/setup.py` & `acids-msprior-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.1.0/tests/test_attention.py` & `acids-msprior-1.1.1/tests/test_attention.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.1.0/tests/test_cache.py` & `acids-msprior-1.1.1/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.1.0/tests/test_configs.py` & `acids-msprior-1.1.1/tests/test_configs.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 import torch
 
 from msprior.scripted import ScriptedPrior
 
 torch.set_grad_enabled(False)
 
 configs = map(str, pathlib.Path("msprior/configs").glob("*.gin"))
+configs = filter(lambda x:"flattened" not in x, configs)
+configs = filter(lambda x:"rwkv" not in x, configs)
 configs = list(configs)
 
 names = map(os.path.basename, configs)
 names = map(lambda x: os.path.splitext(x)[0], names)
 
 names = itertools.product(names, ["continuous", "discrete"],
                           ["listen", "generate"])
```

