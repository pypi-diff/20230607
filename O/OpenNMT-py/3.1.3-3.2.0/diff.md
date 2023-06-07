# Comparing `tmp/OpenNMT-py-3.1.3.tar.gz` & `tmp/OpenNMT-py-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenNMT-py-3.1.3.tar", last modified: Wed May 24 10:41:35 2023, max compression
+gzip compressed data, was "OpenNMT-py-3.2.0.tar", last modified: Wed Jun  7 20:15:54 2023, max compression
```

## Comparing `OpenNMT-py-3.1.3.tar` & `OpenNMT-py-3.2.0.tar`

### file list

```diff
@@ -1,134 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:41:35.656069 OpenNMT-py-3.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/LICENSE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:41:35.644069 OpenNMT-py-3.1.3/OpenNMT_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-24 10:41:35.000000 OpenNMT-py-3.1.3/OpenNMT_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-24 10:41:35.000000 OpenNMT-py-3.1.3/OpenNMT_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 10:41:35.000000 OpenNMT-py-3.1.3/OpenNMT_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-24 10:41:35.000000 OpenNMT-py-3.1.3/OpenNMT_py.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-24 10:41:35.000000 OpenNMT-py-3.1.3/OpenNMT_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-24 10:41:35.000000 OpenNMT-py-3.1.3/OpenNMT_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-05-24 10:41:35.656069 OpenNMT-py-3.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:41:35.644069 OpenNMT-py-3.1.3/onmt/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:41:35.644069 OpenNMT-py-3.1.3/onmt/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/bin/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1651 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/bin/average_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    10498 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/bin/build_vocab.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1167 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/bin/release_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5237 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/bin/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/bin/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/bin/translate.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:41:35.648069 OpenNMT-py-3.1.3/onmt/decoders/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/decoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/decoders/cnn_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    14204 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/decoders/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/decoders/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)    26060 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/decoders/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:41:35.648069 OpenNMT-py-3.1.3/onmt/encoders/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/encoders/cnn_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/encoders/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/encoders/ggnn_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/encoders/mean_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/encoders/rnn_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/encoders/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:41:35.648069 OpenNMT-py-3.1.3/onmt/inputters/
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/inputters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14876 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/inputters/dynamic_iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6776 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/inputters/inputter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11281 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/inputters/text_corpus.py
--rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/inputters/text_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15660 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/model_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:41:35.648069 OpenNMT-py-3.1.3/onmt/models/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/models/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/models/model_saver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:41:35.652069 OpenNMT-py-3.1.3/onmt/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/modules/alibi_position_bias.py
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/modules/average_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/modules/conv_multi_step_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/modules/copy_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15550 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/modules/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/modules/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/modules/global_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    12194 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/modules/lora.py
--rw-r--r--   0 runner    (1001) docker     (123)    12143 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/modules/multi_headed_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/modules/position_ffn.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/modules/rmsnorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/modules/sparse_activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/modules/sparse_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    24449 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/modules/sru.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/modules/stacked_rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/modules/structured_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/modules/util_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/modules/weight_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)    52017 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/opts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:41:35.652069 OpenNMT-py-3.1.3/onmt/scorers/
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/scorers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/scorers/bleu.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/scorers/scorer.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/scorers/ter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:41:35.652069 OpenNMT-py-3.1.3/onmt/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/tests/test_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    30982 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/tests/test_beam_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/tests/test_copy_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/tests/test_data_prepare.py
--rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/tests/test_embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)    20167 2023-05-24 10:41:27.000000 OpenNMT-py-3.1.3/onmt/tests/test_greedy_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     7467 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/tests/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/tests/test_structured_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    12006 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/tests/test_subword_marker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/tests/test_text_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24156 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/tests/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    10008 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/tests/test_translation_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/tests/test_translator.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/tests/utils_for_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     9020 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/train_single.py
--rw-r--r--   0 runner    (1001) docker     (123)    23544 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:41:35.656069 OpenNMT-py-3.1.3/onmt/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17126 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/transforms/bart.py
--rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/transforms/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/transforms/docify.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/transforms/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     7688 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/transforms/fuzzymatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    13345 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/transforms/inlinetags.py
--rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/transforms/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10779 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/transforms/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     8200 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/transforms/sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)    24101 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/transforms/tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)    10123 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/transforms/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/transforms/uppercase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:41:35.656069 OpenNMT-py-3.1.3/onmt/translate/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/translate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19571 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/translate/beam_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    12967 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/translate/decode_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11385 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/translate/greedy_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/translate/penalties.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/translate/process_zh.py
--rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/translate/translation.py
--rw-r--r--   0 runner    (1001) docker     (123)    36570 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/translate/translation_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    41387 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/translate/translator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 10:41:35.656069 OpenNMT-py-3.1.3/onmt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/utils/alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/utils/cnn_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/utils/earlystopping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    15753 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    28025 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/utils/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14395 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/utils/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/utils/report_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/utils/rnn_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     8493 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/utils/scoring_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/onmt/utils/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-24 10:41:35.656069 OpenNMT-py-3.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-24 10:41:28.000000 OpenNMT-py-3.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:15:54.871519 OpenNMT-py-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/LICENSE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:15:54.843519 OpenNMT-py-3.2.0/OpenNMT_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-06-07 20:15:54.000000 OpenNMT-py-3.2.0/OpenNMT_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-06-07 20:15:54.000000 OpenNMT-py-3.2.0/OpenNMT_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 20:15:54.000000 OpenNMT-py-3.2.0/OpenNMT_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-07 20:15:54.000000 OpenNMT-py-3.2.0/OpenNMT_py.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-07 20:15:54.000000 OpenNMT-py-3.2.0/OpenNMT_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-07 20:15:54.000000 OpenNMT-py-3.2.0/OpenNMT_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-06-07 20:15:54.871519 OpenNMT-py-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:15:54.843519 OpenNMT-py-3.2.0/onmt/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:15:54.847519 OpenNMT-py-3.2.0/onmt/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/bin/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1651 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/bin/average_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10498 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/bin/build_vocab.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1167 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/bin/release_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5237 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/bin/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/bin/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/bin/translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:15:54.847519 OpenNMT-py-3.2.0/onmt/decoders/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/decoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/decoders/cnn_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14204 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/decoders/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/decoders/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28397 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/decoders/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:15:54.847519 OpenNMT-py-3.2.0/onmt/encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/encoders/cnn_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/encoders/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/encoders/ggnn_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/encoders/mean_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/encoders/rnn_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/encoders/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:15:54.855519 OpenNMT-py-3.2.0/onmt/inputters/
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/inputters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14876 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/inputters/dynamic_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7115 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/inputters/inputter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11281 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/inputters/text_corpus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/inputters/text_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14427 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/model_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:15:54.855519 OpenNMT-py-3.2.0/onmt/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5706 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/models/model_saver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:15:54.859519 OpenNMT-py-3.2.0/onmt/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/modules/alibi_position_bias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/modules/average_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7778 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/modules/bnb_linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/modules/conv_multi_step_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/modules/copy_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15550 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/modules/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/modules/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/modules/global_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12494 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/modules/lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13161 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/modules/multi_headed_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/modules/position_ffn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/modules/rmsnorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/modules/sparse_activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/modules/sparse_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24449 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/modules/sru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/modules/stacked_rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/modules/structured_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/modules/util_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/modules/weight_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53100 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/opts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:15:54.859519 OpenNMT-py-3.2.0/onmt/scorers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/scorers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/scorers/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/scorers/scorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/scorers/ter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:15:54.867519 OpenNMT-py-3.2.0/onmt/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/tests/test_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30982 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/tests/test_beam_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/tests/test_copy_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/tests/test_data_prepare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/tests/test_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20167 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/tests/test_greedy_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7467 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/tests/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/tests/test_structured_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12006 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/tests/test_subword_marker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/tests/test_text_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24156 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/tests/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10008 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/tests/test_translation_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/tests/test_translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/tests/utils_for_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/train_single.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23539 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:15:54.867519 OpenNMT-py-3.2.0/onmt/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17126 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/transforms/bart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/transforms/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/transforms/docify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/transforms/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7688 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/transforms/fuzzymatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13648 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/transforms/inlinetags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/transforms/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10779 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/transforms/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8200 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/transforms/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24101 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/transforms/tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10123 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/transforms/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/transforms/uppercase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:15:54.867519 OpenNMT-py-3.2.0/onmt/translate/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/translate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19571 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/translate/beam_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12967 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/translate/decode_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11385 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/translate/greedy_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/translate/penalties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/translate/process_zh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/translate/translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36570 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/translate/translation_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41387 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/translate/translator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:15:54.871519 OpenNMT-py-3.2.0/onmt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/utils/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/utils/cnn_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/utils/earlystopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15753 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29800 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/utils/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14395 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/utils/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/utils/report_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/utils/rnn_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8493 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/utils/scoring_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/utils/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-07 20:15:54.871519 OpenNMT-py-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/setup.py
```

### Comparing `OpenNMT-py-3.1.3/LICENSE.md` & `OpenNMT-py-3.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/OpenNMT_py.egg-info/PKG-INFO` & `OpenNMT-py-3.2.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,8 @@
-Metadata-Version: 2.1
-Name: OpenNMT-py
-Version: 3.1.3
-Summary: A python implementation of OpenNMT
-Project-URL: Documentation, http://opennmt.net/OpenNMT-py/
-Project-URL: Forum, http://forum.opennmt.net/
-Project-URL: Gitter, https://gitter.im/OpenNMT/OpenNMT-py
-Project-URL: Source, https://github.com/OpenNMT/OpenNMT-py/
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
-# OpenNMT-py: Open-Source Neural Machine Translation
+# OpenNMT-py: Open-Source Neural Machine Translation and (Large) Language Models
 
 [![Build Status](https://github.com/OpenNMT/OpenNMT-py/workflows/Lint%20&%20Tests/badge.svg)](https://github.com/OpenNMT/OpenNMT-py/actions)
 [![Documentation](https://img.shields.io/badge/docs-latest-blue.svg)](https://opennmt.net/OpenNMT-py/)
 [![Gitter](https://badges.gitter.im/OpenNMT/OpenNMT-py.svg)](https://gitter.im/OpenNMT/OpenNMT-py?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
 [![Forum](https://img.shields.io/discourse/status?server=https%3A%2F%2Fforum.opennmt.net%2F)](https://forum.opennmt.net/)
 
 OpenNMT-py is the [PyTorch](https://github.com/pytorch/pytorch) version of the [OpenNMT](https://opennmt.net) project, an open-source (MIT) neural machine translation (and beyond!) framework. It is designed to be research friendly to try out new ideas in translation, language modeling, summarization, and many other NLP tasks. Some companies have proven the code to be production ready.
@@ -24,28 +12,38 @@
 Before raising an issue, make sure you read the requirements and the [Full Documentation](https://opennmt.net/OpenNMT-py/) examples.
 
 Unless there is a bug, please use the [Forum](https://forum.opennmt.net) or [Gitter](https://gitter.im/OpenNMT/OpenNMT-py) to ask questions.
 
 ----
 ## For beginners:
 
-There is a new step-by-step and explained tuto (Thanks to Yasmin Moslem): [Tutorial](https://github.com/ymoslem/OpenNMT-Tutorial)
+There is a step-by-step and explained tuto (Thanks to Yasmin Moslem): [Tutorial](https://github.com/ymoslem/OpenNMT-Tutorial)
 
 Please try to read and/or follow before raising newbies issues.
 
 Otherwise you can just have a look at the [Quickstart](https://opennmt.net/OpenNMT-py/quickstart.html) steps
 
 ----
+## New:
+
+LLM support with converters for: Llama, OpenLlama, Redpajama, MPT-7B, Falcon.
+Support for 8bit and 4bit quantization along with LoRA adapters, with or without checkpointing.
+You can finetune 7B and 13B models on a single RTX 24GB with 4-bit quantization.
+Once your model is finetuned you can run inference either with OpenNMT-py or faster with CTranslate2.
+
+For all usecases including NMT, you can now use Multiquery instead of Multihead attention (faster at training and inference) and remove biases from all Linear (QKV as well as FeedForward modules).
+
 
 If you used previous versions of OpenNMT-py, you can check the [Changelog](https://github.com/OpenNMT/OpenNMT-py/blob/master/CHANGELOG.md) or the [Breaking Changes](https://github.com/OpenNMT/OpenNMT-py/blob/master/docs/source/changes.md)
 
 ----
 
 ## Tutorials:
 
+* How to replicate Vicuna with a 7B or 13B llama (or Open llama, MPT-7B, Redpajama)  Language Model: [Tuto Vicuna](https://github.com/OpenNMT/OpenNMT-py/blob/master/docs/source/examples/replicate_vicuna/ReplicateVicuna.md)
 * How to finetune NLLB-200 with your dataset: [Tuto Finetune NLLB-200](https://forum.opennmt.net/t/finetuning-and-curating-nllb-200-with-opennmt-py/5238)
 * How to create a simple OpenNMT-py REST Server: [Tuto REST](https://forum.opennmt.net/t/simple-opennmt-py-rest-server/1392)
 * How to create a simple Web Interface: [Tuto Streamlit](https://forum.opennmt.net/t/simple-web-interface/4527)
 * Replicate the WMT17 en-de experiment: [WMT17 ENDE](https://github.com/OpenNMT/OpenNMT-py/blob/master/docs/source/examples/wmt17/Translation.md)
 
 ----
```

### Comparing `OpenNMT-py-3.1.3/OpenNMT_py.egg-info/SOURCES.txt` & `OpenNMT-py-3.2.0/OpenNMT_py.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 onmt/inputters/text_utils.py
 onmt/models/__init__.py
 onmt/models/model.py
 onmt/models/model_saver.py
 onmt/modules/__init__.py
 onmt/modules/alibi_position_bias.py
 onmt/modules/average_attn.py
+onmt/modules/bnb_linear.py
 onmt/modules/conv_multi_step_attention.py
 onmt/modules/copy_generator.py
 onmt/modules/embeddings.py
 onmt/modules/gate.py
 onmt/modules/global_attention.py
 onmt/modules/lora.py
 onmt/modules/multi_headed_attn.py
```

### Comparing `OpenNMT-py-3.1.3/PKG-INFO` & `OpenNMT-py-3.2.0/OpenNMT_py.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: OpenNMT-py
-Version: 3.1.3
+Version: 3.2.0
 Summary: A python implementation of OpenNMT
 Project-URL: Documentation, http://opennmt.net/OpenNMT-py/
 Project-URL: Forum, http://forum.opennmt.net/
 Project-URL: Gitter, https://gitter.im/OpenNMT/OpenNMT-py
 Project-URL: Source, https://github.com/OpenNMT/OpenNMT-py/
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-# OpenNMT-py: Open-Source Neural Machine Translation
+# OpenNMT-py: Open-Source Neural Machine Translation and (Large) Language Models
 
 [![Build Status](https://github.com/OpenNMT/OpenNMT-py/workflows/Lint%20&%20Tests/badge.svg)](https://github.com/OpenNMT/OpenNMT-py/actions)
 [![Documentation](https://img.shields.io/badge/docs-latest-blue.svg)](https://opennmt.net/OpenNMT-py/)
 [![Gitter](https://badges.gitter.im/OpenNMT/OpenNMT-py.svg)](https://gitter.im/OpenNMT/OpenNMT-py?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
 [![Forum](https://img.shields.io/discourse/status?server=https%3A%2F%2Fforum.opennmt.net%2F)](https://forum.opennmt.net/)
 
 OpenNMT-py is the [PyTorch](https://github.com/pytorch/pytorch) version of the [OpenNMT](https://opennmt.net) project, an open-source (MIT) neural machine translation (and beyond!) framework. It is designed to be research friendly to try out new ideas in translation, language modeling, summarization, and many other NLP tasks. Some companies have proven the code to be production ready.
@@ -24,28 +24,38 @@
 Before raising an issue, make sure you read the requirements and the [Full Documentation](https://opennmt.net/OpenNMT-py/) examples.
 
 Unless there is a bug, please use the [Forum](https://forum.opennmt.net) or [Gitter](https://gitter.im/OpenNMT/OpenNMT-py) to ask questions.
 
 ----
 ## For beginners:
 
-There is a new step-by-step and explained tuto (Thanks to Yasmin Moslem): [Tutorial](https://github.com/ymoslem/OpenNMT-Tutorial)
+There is a step-by-step and explained tuto (Thanks to Yasmin Moslem): [Tutorial](https://github.com/ymoslem/OpenNMT-Tutorial)
 
 Please try to read and/or follow before raising newbies issues.
 
 Otherwise you can just have a look at the [Quickstart](https://opennmt.net/OpenNMT-py/quickstart.html) steps
 
 ----
+## New:
+
+LLM support with converters for: Llama, OpenLlama, Redpajama, MPT-7B, Falcon.
+Support for 8bit and 4bit quantization along with LoRA adapters, with or without checkpointing.
+You can finetune 7B and 13B models on a single RTX 24GB with 4-bit quantization.
+Once your model is finetuned you can run inference either with OpenNMT-py or faster with CTranslate2.
+
+For all usecases including NMT, you can now use Multiquery instead of Multihead attention (faster at training and inference) and remove biases from all Linear (QKV as well as FeedForward modules).
+
 
 If you used previous versions of OpenNMT-py, you can check the [Changelog](https://github.com/OpenNMT/OpenNMT-py/blob/master/CHANGELOG.md) or the [Breaking Changes](https://github.com/OpenNMT/OpenNMT-py/blob/master/docs/source/changes.md)
 
 ----
 
 ## Tutorials:
 
+* How to replicate Vicuna with a 7B or 13B llama (or Open llama, MPT-7B, Redpajama)  Language Model: [Tuto Vicuna](https://github.com/OpenNMT/OpenNMT-py/blob/master/docs/source/examples/replicate_vicuna/ReplicateVicuna.md)
 * How to finetune NLLB-200 with your dataset: [Tuto Finetune NLLB-200](https://forum.opennmt.net/t/finetuning-and-curating-nllb-200-with-opennmt-py/5238)
 * How to create a simple OpenNMT-py REST Server: [Tuto REST](https://forum.opennmt.net/t/simple-opennmt-py-rest-server/1392)
 * How to create a simple Web Interface: [Tuto Streamlit](https://forum.opennmt.net/t/simple-web-interface/4527)
 * Replicate the WMT17 en-de experiment: [WMT17 ENDE](https://github.com/OpenNMT/OpenNMT-py/blob/master/docs/source/examples/wmt17/Translation.md)
 
 ----
```

### Comparing `OpenNMT-py-3.1.3/README.md` & `OpenNMT-py-3.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,20 @@
-# OpenNMT-py: Open-Source Neural Machine Translation
+Metadata-Version: 2.1
+Name: OpenNMT-py
+Version: 3.2.0
+Summary: A python implementation of OpenNMT
+Project-URL: Documentation, http://opennmt.net/OpenNMT-py/
+Project-URL: Forum, http://forum.opennmt.net/
+Project-URL: Gitter, https://gitter.im/OpenNMT/OpenNMT-py
+Project-URL: Source, https://github.com/OpenNMT/OpenNMT-py/
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+# OpenNMT-py: Open-Source Neural Machine Translation and (Large) Language Models
 
 [![Build Status](https://github.com/OpenNMT/OpenNMT-py/workflows/Lint%20&%20Tests/badge.svg)](https://github.com/OpenNMT/OpenNMT-py/actions)
 [![Documentation](https://img.shields.io/badge/docs-latest-blue.svg)](https://opennmt.net/OpenNMT-py/)
 [![Gitter](https://badges.gitter.im/OpenNMT/OpenNMT-py.svg)](https://gitter.im/OpenNMT/OpenNMT-py?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
 [![Forum](https://img.shields.io/discourse/status?server=https%3A%2F%2Fforum.opennmt.net%2F)](https://forum.opennmt.net/)
 
 OpenNMT-py is the [PyTorch](https://github.com/pytorch/pytorch) version of the [OpenNMT](https://opennmt.net) project, an open-source (MIT) neural machine translation (and beyond!) framework. It is designed to be research friendly to try out new ideas in translation, language modeling, summarization, and many other NLP tasks. Some companies have proven the code to be production ready.
@@ -12,28 +24,38 @@
 Before raising an issue, make sure you read the requirements and the [Full Documentation](https://opennmt.net/OpenNMT-py/) examples.
 
 Unless there is a bug, please use the [Forum](https://forum.opennmt.net) or [Gitter](https://gitter.im/OpenNMT/OpenNMT-py) to ask questions.
 
 ----
 ## For beginners:
 
-There is a new step-by-step and explained tuto (Thanks to Yasmin Moslem): [Tutorial](https://github.com/ymoslem/OpenNMT-Tutorial)
+There is a step-by-step and explained tuto (Thanks to Yasmin Moslem): [Tutorial](https://github.com/ymoslem/OpenNMT-Tutorial)
 
 Please try to read and/or follow before raising newbies issues.
 
 Otherwise you can just have a look at the [Quickstart](https://opennmt.net/OpenNMT-py/quickstart.html) steps
 
 ----
+## New:
+
+LLM support with converters for: Llama, OpenLlama, Redpajama, MPT-7B, Falcon.
+Support for 8bit and 4bit quantization along with LoRA adapters, with or without checkpointing.
+You can finetune 7B and 13B models on a single RTX 24GB with 4-bit quantization.
+Once your model is finetuned you can run inference either with OpenNMT-py or faster with CTranslate2.
+
+For all usecases including NMT, you can now use Multiquery instead of Multihead attention (faster at training and inference) and remove biases from all Linear (QKV as well as FeedForward modules).
+
 
 If you used previous versions of OpenNMT-py, you can check the [Changelog](https://github.com/OpenNMT/OpenNMT-py/blob/master/CHANGELOG.md) or the [Breaking Changes](https://github.com/OpenNMT/OpenNMT-py/blob/master/docs/source/changes.md)
 
 ----
 
 ## Tutorials:
 
+* How to replicate Vicuna with a 7B or 13B llama (or Open llama, MPT-7B, Redpajama)  Language Model: [Tuto Vicuna](https://github.com/OpenNMT/OpenNMT-py/blob/master/docs/source/examples/replicate_vicuna/ReplicateVicuna.md)
 * How to finetune NLLB-200 with your dataset: [Tuto Finetune NLLB-200](https://forum.opennmt.net/t/finetuning-and-curating-nllb-200-with-opennmt-py/5238)
 * How to create a simple OpenNMT-py REST Server: [Tuto REST](https://forum.opennmt.net/t/simple-opennmt-py-rest-server/1392)
 * How to create a simple Web Interface: [Tuto Streamlit](https://forum.opennmt.net/t/simple-web-interface/4527)
 * Replicate the WMT17 en-de experiment: [WMT17 ENDE](https://github.com/OpenNMT/OpenNMT-py/blob/master/docs/source/examples/wmt17/Translation.md)
 
 ----
```

### Comparing `OpenNMT-py-3.1.3/onmt/bin/average_models.py` & `OpenNMT-py-3.2.0/onmt/bin/average_models.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/bin/build_vocab.py` & `OpenNMT-py-3.2.0/onmt/bin/build_vocab.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/bin/release_model.py` & `OpenNMT-py-3.2.0/onmt/bin/release_model.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/bin/server.py` & `OpenNMT-py-3.2.0/onmt/bin/server.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/bin/train.py` & `OpenNMT-py-3.2.0/onmt/bin/train.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/bin/translate.py` & `OpenNMT-py-3.2.0/onmt/bin/translate.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/constants.py` & `OpenNMT-py-3.2.0/onmt/constants.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/decoders/__init__.py` & `OpenNMT-py-3.2.0/onmt/decoders/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/decoders/cnn_decoder.py` & `OpenNMT-py-3.2.0/onmt/decoders/cnn_decoder.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/decoders/decoder.py` & `OpenNMT-py-3.2.0/onmt/decoders/decoder.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/decoders/ensemble.py` & `OpenNMT-py-3.2.0/onmt/decoders/ensemble.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/decoders/transformer.py` & `OpenNMT-py-3.2.0/onmt/decoders/transformer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 Implementation of "Attention is All You Need" and of
 subsequent transformer based architectures
 """
 
 import torch
 import torch.nn as nn
-
 from onmt.decoders.decoder import DecoderBase
 from onmt.modules import MultiHeadedAttention, AverageAttention
 from onmt.modules.position_ffn import PositionwiseFeedForward
 from onmt.modules.position_ffn import ActivationFunction
 from onmt.utils.misc import sequence_mask
 from onmt.modules.rmsnorm import RMSNorm
 
@@ -25,15 +24,19 @@
         self_attn_type="scaled-dot",
         max_relative_positions=0,
         aan_useffn=False,
         full_context_alignment=False,
         alignment_heads=0,
         pos_ffn_activation_fn=ActivationFunction.relu,
         add_qkvbias=False,
+        multiquery=False,
+        add_ffnbias=True,
+        parallel_residual=False,
         layer_norm="standard",
+        use_ckpting=[],
     ):
         """
         Args:
             d_model (int): the dimension of keys/values/queries in
                 :class:`MultiHeadedAttention`, also the input size of
                 the first-layer of the :class:`PositionwiseFeedForward`.
             heads (int): the number of heads for MultiHeadedAttention.
@@ -67,30 +70,40 @@
             self.self_attn = MultiHeadedAttention(
                 heads,
                 d_model,
                 dropout=attention_dropout,
                 max_relative_positions=max_relative_positions,
                 attn_type="self",
                 add_qkvbias=add_qkvbias,
+                multiquery=multiquery,
+                use_ckpting=use_ckpting,
             )
         elif self_attn_type == "average":
             self.self_attn = AverageAttention(
                 d_model, dropout=attention_dropout, aan_useffn=aan_useffn
             )
 
         self.feed_forward = PositionwiseFeedForward(
-            d_model, d_ff, dropout, pos_ffn_activation_fn, layer_norm
+            d_model,
+            d_ff,
+            dropout,
+            pos_ffn_activation_fn,
+            add_ffnbias,
+            parallel_residual,
+            layer_norm,
+            use_ckpting=use_ckpting,
         )
+        self.parallel_residual = parallel_residual
         if layer_norm == "standard":
             self.layer_norm_1 = nn.LayerNorm(d_model, eps=1e-6)
         elif layer_norm == "rms":
             self.layer_norm_1 = RMSNorm(d_model, eps=1e-6)
         else:
             raise ValueError(f"{layer_norm} layer norm type is not supported")
-        self.drop = nn.Dropout(dropout)
+        self.dropout = nn.Dropout(dropout)
         self.full_context_alignment = full_context_alignment
         self.alignment_heads = alignment_heads
 
     def forward(self, *args, **kwargs):
         """Extend `_forward` for (possibly) multiple decoder pass:
         Always a default (future masked) decoder forward pass,
         Possibly a second future aware decoder pass for joint learn
@@ -124,15 +137,15 @@
             # Case 3: full_context, 1 align heads -> full cte guided align
             attn_align = attns.mean(dim=1)
         return layer_out, top_attn, attn_align
 
     def update_dropout(self, dropout, attention_dropout):
         self.self_attn.update_dropout(attention_dropout)
         self.feed_forward.update_dropout(dropout)
-        self.drop.p = dropout
+        self.dropout.p = dropout
 
     def _forward(self, *args, **kwargs):
         raise NotImplementedError
 
     def _compute_dec_mask(self, tgt_pad_mask, future):
         tgt_len = tgt_pad_mask.size(-1)
         if not future:  # apply future_mask, result mask in (B, T, T)
@@ -148,21 +161,21 @@
             except AttributeError:
                 pass
             dec_mask = torch.gt(tgt_pad_mask + future_mask, 0)
         else:  # only mask padding, result mask in (B, 1, T)
             dec_mask = tgt_pad_mask
         return dec_mask
 
-    def _forward_self_attn(self, layer_in_norm, dec_mask, step):
+    def _forward_self_attn(self, norm_layer_in, dec_mask, step):
         if self.self_attn_type == "scaled-dot":
             return self.self_attn(
-                layer_in_norm, layer_in_norm, layer_in_norm, mask=dec_mask, step=step
+                norm_layer_in, norm_layer_in, norm_layer_in, mask=dec_mask, step=step
             )
         elif self.self_attn_type == "average":
-            return self.self_attn(layer_in_norm, mask=dec_mask, step=step)
+            return self.self_attn(norm_layer_in, mask=dec_mask, step=step)
         else:
             raise ValueError(f"self attention {type(self.self_attn)} not supported")
 
 
 class TransformerDecoderLayer(TransformerDecoderLayerBase):
     """Transformer Decoder layer block in Pre-Norm style.
     Pre-Norm style is an improvement w.r.t. Original paper's Post-Norm style,
@@ -182,15 +195,19 @@
         self_attn_type="scaled-dot",
         max_relative_positions=0,
         aan_useffn=False,
         full_context_alignment=False,
         alignment_heads=0,
         pos_ffn_activation_fn=ActivationFunction.relu,
         add_qkvbias=False,
+        multiquery=False,
+        add_ffnbias=True,
+        parallel_residual=False,
         layer_norm="standard",
+        use_ckpting=[],
     ):
         """
         Args:
             See TransformerDecoderLayerBase
         """
         super(TransformerDecoderLayer, self).__init__(
             d_model,
@@ -201,22 +218,28 @@
             self_attn_type,
             max_relative_positions,
             aan_useffn,
             full_context_alignment,
             alignment_heads,
             pos_ffn_activation_fn=pos_ffn_activation_fn,
             add_qkvbias=add_qkvbias,
+            multiquery=multiquery,
+            add_ffnbias=add_ffnbias,
+            parallel_residual=parallel_residual,
             layer_norm=layer_norm,
+            use_ckpting=use_ckpting,
         )
         self.context_attn = MultiHeadedAttention(
             heads,
             d_model,
             dropout=attention_dropout,
             attn_type="context",
             add_qkvbias=add_qkvbias,
+            multiquery=multiquery,
+            use_ckpting=use_ckpting,
         )
         if layer_norm == "standard":
             self.layer_norm_2 = nn.LayerNorm(d_model, eps=1e-6)
         elif layer_norm == "rms":
             self.layer_norm_2 = RMSNorm(d_model, eps=1e-6)
         else:
             raise ValueError(f"{layer_norm} layer norm type is not supported")
@@ -261,24 +284,37 @@
             dec_mask = self._compute_dec_mask(tgt_pad_mask, future)
             dec_mask = dec_mask.unsqueeze(1)
             dec_mask = dec_mask.expand(-1, -1, dec_mask.size(3), -1)
             src_pad_mask = src_pad_mask.expand(-1, -1, dec_mask.size(3), -1)
             # mask now are (batch x 1 x tlen x s or t len)
             # 1 = heads to be expanded in MHA
 
-        layer_in_norm = self.layer_norm_1(layer_in)
+        norm_layer_in = self.layer_norm_1(layer_in)
 
-        query, _ = self._forward_self_attn(layer_in_norm, dec_mask, step)
+        self_attn, _ = self._forward_self_attn(norm_layer_in, dec_mask, step)
 
-        query = self.drop(query) + layer_in
-
-        query_norm = self.layer_norm_2(query)
-
-        mid, attns = self.context_attn(enc_out, enc_out, query_norm, mask=src_pad_mask)
-        layer_out = self.feed_forward(self.drop(mid) + query)
+        if self.parallel_residual:
+            ctx_attn, attns = self.context_attn(
+                enc_out, enc_out, norm_layer_in, mask=src_pad_mask
+            )
+            # feed_forward applies residual, so we remove and apply residual with un-normed
+            layer_out = (
+                self.feed_forward(norm_layer_in)
+                - norm_layer_in
+                + layer_in
+                + self.dropout(self_attn)
+                + ctx_attn
+            )
+        else:
+            query = self.dropout(self_attn) + layer_in
+            norm_query = self.layer_norm_2(query)
+            ctx_attn, attns = self.context_attn(
+                enc_out, enc_out, norm_query, mask=src_pad_mask
+            )
+            layer_out = self.feed_forward(self.dropout(ctx_attn) + query)
 
         return layer_out, attns
 
 
 class TransformerDecoderBase(DecoderBase):
     def __init__(self, d_model, copy_attn, embeddings, alignment_layer, layer_norm):
         super(TransformerDecoderBase, self).__init__()
@@ -319,15 +355,19 @@
             opt.max_relative_positions,
             opt.aan_useffn,
             opt.full_context_alignment,
             opt.alignment_layer,
             alignment_heads=opt.alignment_heads,
             pos_ffn_activation_fn=opt.pos_ffn_activation_fn,
             add_qkvbias=opt.add_qkvbias,
+            multiquery=opt.multiquery,
+            add_ffnbias=opt.add_ffnbias,
+            parallel_residual=opt.parallel_residual,
             layer_norm=opt.layer_norm,
+            use_ckpting=opt.use_ckpting,
         )
 
     def init_state(self, src, enc_out, enc_final_hs):
         """Initialize decoder state."""
         self.state["src"] = src
 
     def map_state(self, fn):
@@ -402,15 +442,19 @@
         max_relative_positions,
         aan_useffn,
         full_context_alignment,
         alignment_layer,
         alignment_heads,
         pos_ffn_activation_fn=ActivationFunction.relu,
         add_qkvbias=False,
+        multiquery=False,
+        add_ffnbias=True,
+        parallel_residual=False,
         layer_norm="standard",
+        use_ckpting=[],
     ):
         super(TransformerDecoder, self).__init__(
             d_model, copy_attn, embeddings, alignment_layer, layer_norm
         )
 
         self.transformer_layers = nn.ModuleList(
             [
@@ -423,15 +467,19 @@
                     self_attn_type=self_attn_type,
                     max_relative_positions=max_relative_positions,
                     aan_useffn=aan_useffn,
                     full_context_alignment=full_context_alignment,
                     alignment_heads=alignment_heads,
                     pos_ffn_activation_fn=pos_ffn_activation_fn,
                     add_qkvbias=add_qkvbias,
+                    multiquery=multiquery,
+                    add_ffnbias=add_ffnbias,
+                    parallel_residual=parallel_residual,
                     layer_norm=layer_norm,
+                    use_ckpting=use_ckpting,
                 )
                 for i in range(num_layers)
             ]
         )
 
     def detach_state(self):
         self.state["src"] = self.state["src"].detach()
@@ -457,26 +505,24 @@
                         {"keys": torch.tensor([]), "values": torch.tensor([])},
                     )
                 layer.context_attn.layer_cache = (
                     False,
                     {"keys": torch.tensor([]), "values": torch.tensor([])},
                 )
 
-        tgt_words = tgt[:, :, 0]
-
         emb = self.embeddings(tgt, step=step)
         dec_out = emb
         assert emb.dim() == 3  # len x batch x embedding_dim
 
         pad_idx = self.embeddings.word_padding_idx
         src_lens = kwargs["src_len"]
         src_max_len = self.state["src"].shape[1]
         src_pad_mask = ~sequence_mask(src_lens, src_max_len)  # [B x slen]
         src_pad_mask = src_pad_mask.unsqueeze(1)  # [B x 1 x slen]
-        tgt_pad_mask = tgt_words.data.eq(pad_idx).unsqueeze(1)  # [B, 1, T_tgt]
+        tgt_pad_mask = tgt[:, :, 0].eq(pad_idx).unsqueeze(1)  # [B, 1, T_tgt]
 
         with_align = kwargs.pop("with_align", False)
         attn_aligns = []
 
         for layer in self.transformer_layers:
             dec_out, attn, attn_align = layer(
                 dec_out,
@@ -562,21 +608,29 @@
             # masking is necessary when sequence length is greater than one
             dec_mask = self._compute_dec_mask(tgt_pad_mask, future)
             dec_mask = dec_mask.unsqueeze(1)
             dec_mask = dec_mask.expand(-1, -1, dec_mask.size(3), -1)
             # mask now are (batch x 1 x tlen x tlen)
             # 1 = heads to be expanded in MHA
 
-        layer_in_norm = self.layer_norm_1(layer_in)
-
-        query, attns = self._forward_self_attn(layer_in_norm, dec_mask, step)
+        norm_layer_in = self.layer_norm_1(layer_in)
 
-        layer_out = self.drop(query) + layer_in
+        attn_output, attns = self._forward_self_attn(norm_layer_in, dec_mask, step)
 
-        layer_out = self.feed_forward(layer_out)
+        if self.parallel_residual:
+            # feed_forward applies residual, so we remove and apply residual with un-normed
+            layer_out = (
+                self.feed_forward(norm_layer_in)
+                - norm_layer_in
+                + layer_in
+                + self.dropout(attn_output)
+            )
+        else:
+            layer_out = self.dropout(attn_output) + layer_in
+            layer_out = self.feed_forward(layer_out)
 
         return layer_out, attns
 
 
 class TransformerLMDecoder(TransformerDecoderBase):
     """The Transformer decoder from GPT-2
     Args:
@@ -610,15 +664,19 @@
         max_relative_positions,
         aan_useffn,
         full_context_alignment=None,
         alignment_layer=None,
         alignment_heads=None,
         pos_ffn_activation_fn=ActivationFunction.relu,
         add_qkvbias=False,
+        multiquery=False,
+        add_ffnbias=True,
+        parallel_residual=False,
         layer_norm="standard",
+        use_ckpting=[],
     ):
         super(TransformerLMDecoder, self).__init__(
             d_model, copy_attn, embeddings, alignment_layer, layer_norm
         )
         self.transformer_layers = nn.ModuleList(
             [
                 TransformerLMDecoderLayer(
@@ -630,15 +688,19 @@
                     self_attn_type=self_attn_type,
                     max_relative_positions=max_relative_positions,
                     aan_useffn=aan_useffn,
                     full_context_alignment=None,
                     alignment_heads=None,
                     pos_ffn_activation_fn=pos_ffn_activation_fn,
                     add_qkvbias=add_qkvbias,
+                    multiquery=multiquery,
+                    add_ffnbias=add_ffnbias,
+                    parallel_residual=parallel_residual,
                     layer_norm=layer_norm,
+                    use_ckpting=use_ckpting,
                 )
                 for i in range(num_layers)
             ]
         )
 
     def init_state(self, src=None, enc_out=None, enc_final_hs=None):
         super(TransformerLMDecoder, self).init_state(None, None, None)
@@ -653,22 +715,20 @@
         elif step is None:
             for layer in self.transformer_layers:
                 layer.self_attn.layer_cache = (
                     False,
                     {"keys": torch.tensor([]), "values": torch.tensor([])},
                 )
 
-        tgt_words = tgt[:, :, 0]
-
         dec_out = self.embeddings(tgt, step=step)
 
         assert dec_out.dim() == 3  # batch x len x embedding_dim
 
         pad_idx = self.embeddings.word_padding_idx
-        tgt_pad_mask = tgt_words.data.eq(pad_idx).unsqueeze(1)  # [B, 1, T_tgt]
+        tgt_pad_mask = tgt[:, :, 0].eq(pad_idx).unsqueeze(1)  # [B, 1, T_tgt]
 
         with_align = kwargs.pop("with_align", False)
         assert not with_align, "TransformerLMDecoder does not support align"
 
         for layer in self.transformer_layers:
             dec_out, attn, _ = layer(
                 dec_out,
```

### Comparing `OpenNMT-py-3.1.3/onmt/encoders/__init__.py` & `OpenNMT-py-3.2.0/onmt/encoders/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/encoders/cnn_encoder.py` & `OpenNMT-py-3.2.0/onmt/encoders/cnn_encoder.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/encoders/encoder.py` & `OpenNMT-py-3.2.0/onmt/encoders/encoder.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/encoders/ggnn_encoder.py` & `OpenNMT-py-3.2.0/onmt/encoders/ggnn_encoder.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/encoders/mean_encoder.py` & `OpenNMT-py-3.2.0/onmt/encoders/mean_encoder.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/encoders/rnn_encoder.py` & `OpenNMT-py-3.2.0/onmt/encoders/rnn_encoder.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/encoders/transformer.py` & `OpenNMT-py-3.2.0/onmt/encoders/transformer.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import torch.nn as nn
 
 from onmt.encoders.encoder import EncoderBase
 from onmt.modules import MultiHeadedAttention
 from onmt.modules.position_ffn import PositionwiseFeedForward
 from onmt.modules.position_ffn import ActivationFunction
 from onmt.utils.misc import sequence_mask
+from onmt.modules.rmsnorm import RMSNorm
 
 
 class TransformerEncoderLayer(nn.Module):
     """
     A single layer of the transformer encoder.
 
     Args:
@@ -32,45 +33,77 @@
         heads,
         d_ff,
         dropout,
         attention_dropout,
         max_relative_positions=0,
         pos_ffn_activation_fn=ActivationFunction.relu,
         add_qkvbias=False,
+        multiquery=False,
+        add_ffnbias=True,
+        parallel_residual=False,
+        layer_norm="standard",
+        use_ckpting=[],
     ):
         super(TransformerEncoderLayer, self).__init__()
 
         self.self_attn = MultiHeadedAttention(
             heads,
             d_model,
             dropout=attention_dropout,
             max_relative_positions=max_relative_positions,
             attn_type="self",
             add_qkvbias=add_qkvbias,
+            multiquery=multiquery,
+            use_ckpting=use_ckpting,
         )
         self.feed_forward = PositionwiseFeedForward(
-            d_model, d_ff, dropout, pos_ffn_activation_fn
+            d_model,
+            d_ff,
+            dropout,
+            pos_ffn_activation_fn,
+            add_ffnbias,
+            parallel_residual,
+            layer_norm,
+            use_ckpting=use_ckpting,
         )
-        self.layer_norm = nn.LayerNorm(d_model, eps=1e-6)
+        self.parallel_residual = parallel_residual
+        if layer_norm == "standard":
+            self.layer_norm = nn.LayerNorm(d_model, eps=1e-6)
+        elif layer_norm == "rms":
+            self.layer_norm = RMSNorm(d_model, eps=1e-6)
+        else:
+            raise ValueError(f"{layer_norm} layer norm type is not supported")
         self.dropout = nn.Dropout(dropout)
 
     def forward(self, layer_in, mask):
         """
         Args:
             layer_in (FloatTensor): ``(batch_size, src_len, model_dim)``
             mask (LongTensor): ``(batch_size, 1, src_len)``
 
         Returns:
             (FloatTensor):
             * layer_out ``(batch_size, src_len, model_dim)``
         """
-        input_norm = self.layer_norm(layer_in)
-        context, _ = self.self_attn(input_norm, input_norm, input_norm, mask=mask)
-        layer_out = self.dropout(context) + layer_in
-        layer_out = self.feed_forward(layer_out)
+        norm_layer_in = self.layer_norm(layer_in)
+        context, _ = self.self_attn(
+            norm_layer_in, norm_layer_in, norm_layer_in, mask=mask
+        )
+        if self.parallel_residual:
+            # feed_forward applies residual, so we remove and apply residual with un-normed
+            layer_out = (
+                self.feed_forward(norm_layer_in)
+                - norm_layer_in
+                + layer_in
+                + self.dropout(context)
+            )
+        else:
+            layer_out = self.dropout(context) + layer_in
+            layer_out = self.feed_forward(layer_out)
+
         return layer_out
 
     def update_dropout(self, dropout, attention_dropout):
         self.self_attn.update_dropout(attention_dropout)
         self.feed_forward.update_dropout(dropout)
         self.dropout.p = dropout
 
@@ -106,14 +139,19 @@
         d_ff,
         dropout,
         attention_dropout,
         embeddings,
         max_relative_positions,
         pos_ffn_activation_fn=ActivationFunction.relu,
         add_qkvbias=False,
+        multiquery=False,
+        add_ffnbias=True,
+        parallel_residual=False,
+        layer_norm="standard",
+        use_ckpting=[],
     ):
         super(TransformerEncoder, self).__init__()
 
         self.embeddings = embeddings
         self.transformer = nn.ModuleList(
             [
                 TransformerEncoderLayer(
@@ -121,19 +159,29 @@
                     heads,
                     d_ff,
                     dropout,
                     attention_dropout,
                     max_relative_positions=max_relative_positions,
                     pos_ffn_activation_fn=pos_ffn_activation_fn,
                     add_qkvbias=add_qkvbias,
+                    multiquery=multiquery,
+                    add_ffnbias=add_ffnbias,
+                    parallel_residual=parallel_residual,
+                    layer_norm=layer_norm,
+                    use_ckpting=use_ckpting,
                 )
                 for i in range(num_layers)
             ]
         )
-        self.layer_norm = nn.LayerNorm(d_model, eps=1e-6)
+        if layer_norm == "standard":
+            self.layer_norm = nn.LayerNorm(d_model, eps=1e-6)
+        elif layer_norm == "rms":
+            self.layer_norm = RMSNorm(d_model, eps=1e-6)
+        else:
+            raise ValueError(f"{layer_norm} layer norm type is not supported")
 
     @classmethod
     def from_opt(cls, opt, embeddings):
         """Alternate constructor."""
         return cls(
             opt.enc_layers,
             opt.enc_hid_size,
@@ -143,14 +191,19 @@
             opt.attention_dropout[0]
             if type(opt.attention_dropout) is list
             else opt.attention_dropout,
             embeddings,
             opt.max_relative_positions,
             pos_ffn_activation_fn=opt.pos_ffn_activation_fn,
             add_qkvbias=opt.add_qkvbias,
+            multiquery=opt.multiquery,
+            add_ffnbias=opt.add_ffnbias,
+            parallel_residual=opt.parallel_residual,
+            layer_norm=opt.layer_norm,
+            use_ckpting=opt.use_ckpting,
         )
 
     def forward(self, src, src_len=None):
         """See :func:`EncoderBase.forward()`"""
         enc_out = self.embeddings(src)
         mask = ~sequence_mask(src_len).unsqueeze(1)
         mask = mask.unsqueeze(1)
```

### Comparing `OpenNMT-py-3.1.3/onmt/inputters/__init__.py` & `OpenNMT-py-3.2.0/onmt/inputters/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/inputters/dynamic_iterator.py` & `OpenNMT-py-3.2.0/onmt/inputters/dynamic_iterator.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/inputters/inputter.py` & `OpenNMT-py-3.2.0/onmt/inputters/inputter.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,15 +55,20 @@
     vocabs = {}
     src_vocab = _read_vocab_file(opt.src_vocab, opt.src_words_min_frequency)
 
     src_specials = [
         item for item in (default_specials + specials["src"]) if item not in src_vocab
     ]
 
-    if DefaultTokens.SEP in src_specials and "<0x0A>" in src_vocab:
+    if DefaultTokens.SEP in src_specials and (
+        "<0x0A>" in src_vocab or "Ċ" in src_vocab
+    ):
+        # this is hack: if the special separator ｟newline｠is returned because of the
+        # "docify" transform.get_specials we don't add it if the corresponding newline code
+        # is already included in the sentencepiece or BPE-with-gpt2-pretok.
         src_specials.remove(DefaultTokens.SEP)
 
     src_vocab = pyonmttok.build_vocab_from_tokens(
         src_vocab, maximum_size=opt.src_vocab_size, special_tokens=src_specials
     )
     src_vocab.default_id = src_vocab[DefaultTokens.UNK]
 
@@ -75,15 +80,17 @@
     else:
         tgt_vocab = _read_vocab_file(opt.tgt_vocab, opt.tgt_words_min_frequency)
         tgt_specials = [
             item
             for item in (default_specials + specials["tgt"])
             if item not in tgt_vocab
         ]
-        if DefaultTokens.SEP in tgt_specials and "<0x0A>" in tgt_vocab:
+        if DefaultTokens.SEP in tgt_specials and (
+            "<0x0A>" in tgt_vocab or "Ċ" in src_vocab
+        ):
             tgt_specials.remove(DefaultTokens.SEP)
         tgt_vocab = pyonmttok.build_vocab_from_tokens(
             tgt_vocab, maximum_size=opt.tgt_vocab_size, special_tokens=tgt_specials
         )
         tgt_vocab.default_id = tgt_vocab[DefaultTokens.UNK]
         if opt.vocab_size_multiple > 1:
             tgt_vocab = _pad_vocab_to_multiple(tgt_vocab, opt.vocab_size_multiple)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `OpenNMT-py-3.1.3/onmt/inputters/text_corpus.py` & `OpenNMT-py-3.2.0/onmt/inputters/text_corpus.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/inputters/text_utils.py` & `OpenNMT-py-3.2.0/onmt/inputters/text_utils.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/model_builder.py` & `OpenNMT-py-3.2.0/onmt/model_builder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,94 +1,32 @@
 """
 This file is for models creation, which consults options
 and creates each encoder and decoder accordingly.
 """
 import re
+import os
+import importlib
 import torch
 import torch.nn as nn
-from torch.nn.init import xavier_uniform_
+from torch.nn.init import xavier_uniform_, zeros_, uniform_
 import onmt.modules
 from onmt.encoders import str2enc
 from onmt.decoders import str2dec
 from onmt.inputters.inputter import dict_to_vocabs
 from onmt.modules import Embeddings, CopyGenerator
 from onmt.utils.misc import use_gpu
 from onmt.utils.logging import logger
 from onmt.utils.parse import ArgumentParser
+from onmt.models.model_saver import load_checkpoint
 from onmt.constants import DefaultTokens, ModelTask
-from onmt.modules import Linear, Embedding, mark_only_lora_as_trainable
-
-
-def replace_8bit_linear(model, threshold=6.0, module_to_convert=""):
-    try:
-        import bitsandbytes as bnb
-    except ImportError:
-        raise ImportError("Install bitsandbytes to use 8bit compression")
-    for name, module in model.named_children():
-        if len(list(module.children())) > 0:
-            replace_8bit_linear(module, threshold, module_to_convert)
-
-        if isinstance(module, nn.Linear) and name == module_to_convert:
-            model._modules[name] = bnb.nn.Linear8bitLt(
-                module.in_features,
-                module.out_features,
-                module.bias is not None,
-                has_fp16_weights=False,
-                threshold=threshold,
-            )
-    return model
-
-
-def replace_lora_linear(model, r=2, lora_alpha=1, lora_dropout=0, layer=""):
-    """
-    Function replacing layers with LoRa layers recursively.
-    Args:
-        model:
-        r: rank of matrix of the Low Rank layer
-        lora_alpha: cf paper
-        lora_dropout: cf paper
-        layer: layer name of the model to be replaced
-    """
-    for name, module in model.named_children():
-        if len(list(module.children())) > 0:
-            replace_lora_linear(module, r, lora_alpha, lora_dropout, layer)
-
-        if isinstance(module, nn.Linear) and name == layer:
-            model._modules[name] = Linear(
-                module.in_features,
-                module.out_features,
-                r=r,
-                lora_alpha=lora_alpha,
-                lora_dropout=lora_dropout,
-                bias=module.bias is not None,
-            )
-    return model
-
-
-def replace_lora_embedding(model, r=2, lora_alpha=1):
-    """
-    Function replacing Embeddings with LoRa ones recursively.
-    Args:
-        model:
-        r: rank of matrix of the Low Rank layer
-        lora_alpha: cf paper
-    """
-    for name, module in model.named_children():
-        if len(list(module.children())) > 0:
-            replace_lora_embedding(module, r, lora_alpha)
-        if isinstance(module, nn.Embedding):
-            model._modules[name] = Embedding(
-                module.num_embeddings,
-                module.embedding_dim,
-                r=r,
-                lora_alpha=lora_alpha,
-                padding_idx=module.padding_idx,
-                sparse=module.sparse,
-            )
-    return model
+from onmt.modules.lora import (
+    replace_lora_linear,
+    replace_lora_embedding,
+    mark_only_lora_as_trainable,
+)
 
 
 def build_embeddings(opt, vocabs, for_encoder=True):
     """
     Args:
         opt: the option in current environment.
         vocab.
@@ -151,26 +89,32 @@
     )
     return str2dec[dec_type].from_opt(opt, embeddings)
 
 
 def load_test_model(opt, model_path=None):
     if model_path is None:
         model_path = opt.models[0]
-    checkpoint = torch.load(model_path, map_location=lambda storage, loc: storage)
+    checkpoint = load_checkpoint(model_path)
 
     model_opt = ArgumentParser.ckpt_model_opts(checkpoint["opt"])
 
     ArgumentParser.update_model_opts(model_opt)
     ArgumentParser.validate_model_opts(model_opt)
     vocabs = dict_to_vocabs(checkpoint["vocab"])
 
     # Avoid functionality on inference
     model_opt.update_vocab = False
 
-    model = build_base_model(model_opt, vocabs, checkpoint)
+    model = build_base_model(model_opt, vocabs)
+
+    model.load_state_dict(
+        checkpoint, precision=torch.float32, device=torch.device("cpu"), strict=True
+    )
+
+    del checkpoint
 
     if opt.precision == "fp32":
         model.float()
     elif opt.precision == "fp16":
         model.half()
     elif opt.precision == "int8":
         if opt.gpu >= 0:
@@ -238,22 +182,22 @@
             model_opt, vocabs, share_embeddings=True, src_emb=src_emb
         )
         return onmt.models.LanguageModel(decoder=decoder)
     else:
         raise ValueError(f"No model defined for {model_opt.model_task} task")
 
 
-def use_embeddings_from_checkpoint(vocabs, model, generator, checkpoint):
+def use_embeddings_from_checkpoint(vocabs, model, checkpoint):
     # Update vocabulary embeddings with checkpoint embeddings
     logger.info("Updating vocabulary embeddings with checkpoint embeddings")
     # Embedding layers
     enc_emb_name = "encoder.embeddings.make_embedding.emb_luts.0.weight"
     dec_emb_name = "decoder.embeddings.make_embedding.emb_luts.0.weight"
-    model_dict = model.state_dict()
-    generator_dict = generator.state_dict()
+    model_dict = {k: v for k, v in model.state_dict().items() if "generator" not in k}
+    generator_dict = model.generator.state_dict()
     for side, emb_name in [("src", enc_emb_name), ("tgt", dec_emb_name)]:
         if emb_name not in checkpoint["model"]:
             continue
         new_tokens = []
         ckp_vocabs = dict_to_vocabs(checkpoint["vocab"])
         for i, tok in enumerate(vocabs[side].ids_to_tokens):
             if tok in ckp_vocabs[side]:
@@ -268,60 +212,82 @@
                 # Just for debugging purposes
                 new_tokens.append(tok)
         logger.info("%s: %d new tokens" % (side, len(new_tokens)))
 
         # Remove old vocabulary associated embeddings
         del checkpoint["model"][emb_name]
     del checkpoint["generator"]["weight"], checkpoint["generator"]["bias"]
-    model.load_state_dict(model_dict)
-    generator.load_state_dict(generator_dict)
+    fake_ckpt = {"model": model_dict, "generator": generator_dict}
+    model.load_state_dict(fake_ckpt)
 
 
-def build_base_model(model_opt, vocabs, checkpoint=None):
+def build_base_model(model_opt, vocabs):
     """Build a model from opts.
 
     Args:
         model_opt: the option loaded from checkpoint. It's important that
             the opts have been updated and validated. See
             :class:`onmt.utils.parse.ArgumentParser`.
         vocabs (dict[str, Vocab]):
             `Field` objects for the model.
-        checkpoint: the model generated by train phase, or a resumed snapshot
-                    model from a stopped training.
 
     Returns:
         the NMTModel.
     """
 
     # for back compat when attention_dropout was not defined
     try:
         model_opt.attention_dropout
     except AttributeError:
         model_opt.attention_dropout = model_opt.dropout
 
     # Build Model
     model = build_task_specific_model(model_opt, vocabs)
 
-    if hasattr(model_opt, "quant_layers") and len(model_opt.quant_layers) > 0:
-        for layer in model_opt.quant_layers:
-            logger.info("8bit compression of layer %s" % layer)
-            model = replace_8bit_linear(model, module_to_convert=layer)
+    nonlora_to_quant = [
+        layer
+        for layer in getattr(model_opt, "quant_layers", [])
+        if layer not in getattr(model_opt, "lora_layers", [])
+    ]
+
+    if hasattr(model_opt, "quant_layers") and len(nonlora_to_quant) > 0:
+        if model_opt.quant_type in ["bnb_8bit", "bnb_FP4", "bnb_NF4"]:
+            logger.info(
+                "%s compression of layer %s" % (model_opt.quant_type, nonlora_to_quant)
+            )
+            try:
+                os.environ["BITSANDBYTES_NOWELCOME"] = "1"
+                import bitsandbytes as bnb
+                from onmt.modules.bnb_linear import replace_bnb_linear
+            except ImportError:
+                raise ImportError("Install bitsandbytes to use 4/8bit compression")
+            model = replace_bnb_linear(
+                model, module_to_convert=nonlora_to_quant, q_type=model_opt.quant_type
+            )
+        else:
+            logger.info("compression type %s not supported." % model_opt.quant_type)
 
     mark_lora = False
     if hasattr(model_opt, "lora_layers") and len(model_opt.lora_layers) > 0:
         if model_opt.freeze_encoder or model_opt.freeze_decoder:
             raise ValueError("Cannot use LoRa with Enc/Dec-oder freezing")
         for layer in model_opt.lora_layers:
-            logger.info("Adding LoRa layers for %s" % layer)
+            if hasattr(model_opt, "quant_layers") and layer in model_opt.quant_layers:
+                quant_type = model_opt.quant_type
+            else:
+                quant_type = None
+            logger.info("Adding LoRa layers for %s quant %s" % (layer, quant_type))
             model = replace_lora_linear(
                 model,
                 r=model_opt.lora_rank,
                 lora_alpha=model_opt.lora_alpha,
                 lora_dropout=model_opt.lora_dropout,
                 layer=layer,
+                quant_type=quant_type,
+                use_ckpting=model_opt.use_ckpting,
             )
         mark_lora = True
     if hasattr(model_opt, "lora_embedding") and model_opt.lora_embedding:
         if model_opt.freeze_encoder or model_opt.freeze_decoder:
             raise ValueError("Cannot use LoRa with Enc/Dec-oder freezing")
         logger.info("Adding LoRa Embeddings")
         model = replace_lora_embedding(
@@ -340,85 +306,89 @@
     else:
         vocab_size = len(vocabs["tgt"])
         pad_idx = vocabs["tgt"][DefaultTokens.PAD]
         generator = CopyGenerator(model_opt.dec_hid_size, vocab_size, pad_idx)
         if model_opt.share_decoder_embeddings:
             generator.linear.weight = model.decoder.embeddings.word_lut.weight
 
-    # Load the model states from checkpoint or initialize them.
+    model.generator = generator
+
+    return model
+
+
+def build_model(model_opt, opt, vocabs, checkpoint):
+    logger.info("Building model...")
+
+    model = build_base_model(model_opt, vocabs)
+
+    # If new training initialize the model params
+    # If update_vocab init also but checkpoint will overwrite old weights
     if checkpoint is None or model_opt.update_vocab:
         if model_opt.param_init != 0.0:
-            for p in model.parameters():
-                p.data.uniform_(-model_opt.param_init, model_opt.param_init)
-            for p in generator.parameters():
-                p.data.uniform_(-model_opt.param_init, model_opt.param_init)
-        if model_opt.param_init_glorot:
-            for p in model.parameters():
-                if p.dim() > 1:
-                    xavier_uniform_(p)
-            for p in generator.parameters():
-                if p.dim() > 1:
-                    xavier_uniform_(p)
+            for param in model.parameters():
+                uniform_(param, -model_opt.param_init, model_opt.param_init)
+        elif model_opt.param_init_glorot:
+            for name, module in model.named_modules():
+                for param_name, param in module.named_parameters():
+                    if param_name == "weight" and param.dim() > 1:
+                        xavier_uniform_(param)
+                    elif param_name == "bias":
+                        zeros_(param)
+        else:
+            raise ValueError("You need either param_init != 0 OR init_glorot True")
 
         if hasattr(model, "encoder") and hasattr(model.encoder, "embeddings"):
             model.encoder.embeddings.load_pretrained_vectors(
                 model_opt.pre_word_vecs_enc
             )
         if hasattr(model.decoder, "embeddings"):
             model.decoder.embeddings.load_pretrained_vectors(
                 model_opt.pre_word_vecs_dec
             )
 
-    if checkpoint is not None:
-        # This preserves backward-compat for models using customed layernorm
-        def fix_key(s):
-            s = re.sub(r"(.*)\.layer_norm((_\d+)?)\.b_2", r"\1.layer_norm\2.bias", s)
-            s = re.sub(r"(.*)\.layer_norm((_\d+)?)\.a_2", r"\1.layer_norm\2.weight", s)
-            return s
-
-        checkpoint["model"] = {fix_key(k): v for k, v in checkpoint["model"].items()}
-
-        if "0.weight" in checkpoint["generator"]:
-            checkpoint["generator"]["weight"] = checkpoint["generator"].pop("0.weight")
-        if "0.bias" in checkpoint["generator"]:
-            checkpoint["generator"]["bias"] = checkpoint["generator"].pop("0.bias")
-        # end of patch for backward compatibility
+    # ONLY for legacy fusedam with amp pytorch requires NOT to half the model
+    if (
+        model_opt.model_dtype == "fp16"
+        and model_opt.apex_opt_level not in ["O0", "O1", "O2", "O3"]
+        and model_opt.optim == "fusedadam"
+    ):
+        precision = torch.float16
+        logger.info("Switching model to half() for FusedAdam legacy")
+        logger.info("Non quantized layer compute is %s", model_opt.model_dtype)
+    else:
+        precision = torch.float32
+        logger.info("Switching model to float32 for amp/apex_amp")
+        logger.info("Non quantized layer compute is %s", model_opt.model_dtype)
 
+    if use_gpu(opt):
+        device = torch.device("cuda")
+    else:
+        device = torch.device("cpu")
+
+    if checkpoint is not None:
         if model_opt.update_vocab:
             # Update model embeddings with those from the checkpoint
             # after initialization
-            use_embeddings_from_checkpoint(vocabs, model, generator, checkpoint)
+            use_embeddings_from_checkpoint(vocabs, model, checkpoint)
+            # after this checkpoint contains no embeddings
 
         # when using LoRa or updating the vocab (no more embeddings in ckpt)
         # => strict=False when loading state_dict
-        strict = (not model_opt.update_vocab) and (not mark_lora)
-        model.load_state_dict(checkpoint["model"], strict=strict)
-        generator.load_state_dict(checkpoint["generator"], strict=strict)
-
-    model.generator = generator
-
-    return model
-
+        strict = not model_opt.update_vocab
 
-def build_model(model_opt, opt, vocabs, checkpoint):
-    logger.info("Building model...")
-    model = build_base_model(model_opt, vocabs, checkpoint)
+        model.load_state_dict(
+            checkpoint, precision=precision, device=device, strict=strict
+        )
+    else:
+        model.to(precision)
+        model.to(device)
 
     if model_opt.freeze_encoder:
         model.encoder.requires_grad_(False)
         model.encoder.embeddings.requires_grad_()
 
     if model_opt.freeze_decoder:
         model.decoder.requires_grad_(False)
         model.decoder.embeddings.requires_grad_()
 
-    if (
-        model_opt.model_dtype == "fp16"
-        and model_opt.apex_opt_level not in ["O0", "O1", "O2", "O3"]
-        and model_opt.optim == "fusedadam"
-    ):
-        model.half()  # with amp pytorch requires NOT to half the model
-
-    if use_gpu(opt):
-        model.to(torch.device("cuda"))
     logger.info(model)
     return model
```

### Comparing `OpenNMT-py-3.1.3/onmt/models/model.py` & `OpenNMT-py-3.2.0/onmt/models/model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """ Onmt NMT Model base class definition """
+import torch
 import torch.nn as nn
+from itertools import chain
 
 
 class BaseModel(nn.Module):
     """Core trainable object in OpenNMT. Implements a trainable interface
     for a simple, generic encoder / decoder or decoder only model.
 
     Args:
@@ -39,14 +41,69 @@
 
     def update_dropout(self, dropout, attention_dropout):
         raise NotImplementedError
 
     def count_parameters(self, log=print):
         raise NotImplementedError
 
+    def load_state_dict(
+        self,
+        checkpoint,
+        precision=torch.float32,
+        device=torch.device("cpu"),
+        strict=True,
+    ):
+        """Custom state_dict loading to enable moving module on device as they are loaded
+
+        Args:
+            checkpoint:
+            precision:
+            device:
+            strict:
+
+        Return:
+
+            * Model"""
+
+        # bitsandbytes quantize weights when .cuda() is called
+        # for huge models we need to save Ram
+        # so we load the weights  module by module and transfer them to GPU for quantization
+        for name, module in self.named_modules():
+            for param_name, param in chain(
+                module.named_parameters(), module.named_buffers()
+            ):
+                if len(param_name.split(".")) == 1:  # only last key
+                    if name + "." + param_name in checkpoint["model"].keys():
+                        param.data = checkpoint["model"][name + "." + param_name]
+                        del checkpoint["model"][name + "." + param_name]
+                    elif (
+                        "generator" in checkpoint.keys()
+                        and name == "generator"
+                        and checkpoint["generator"] is not None
+                        and param_name in checkpoint["generator"].keys()
+                    ):
+                        param.data = checkpoint["generator"][param_name]
+                        del checkpoint["generator"][param_name]
+                    elif strict and "lora" not in param_name:
+                        raise ValueError(
+                            "Missing key in checkpoint: %s" % name + "." + param_name
+                        )
+                    module.to(precision)
+                    module.to(device)
+        if len(checkpoint["model"].keys()) > 0:
+            raise ValueError(
+                "Extra keys in model state_dict do not match the model config %s"
+                % checkpoint["model"].keys()
+            )
+        if len(checkpoint["generator"].keys()) > 0:
+            raise ValueError(
+                "Extra keys in generator state_dict do not match the model config %s"
+                % checkpoint["generator"].keys()
+            )
+
 
 class NMTModel(BaseModel):
     """NMTModel Class
     See :class:`~onmt.models.BaseModel` for options."""
 
     def __init__(self, encoder, decoder):
         super(NMTModel, self).__init__(encoder, decoder)
```

### Comparing `OpenNMT-py-3.1.3/onmt/modules/__init__.py` & `OpenNMT-py-3.2.0/onmt/modules/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """  Attention and normalization modules  """
+import importlib
+import os
 from onmt.modules.util_class import Elementwise
 from onmt.modules.gate import context_gate_factory, ContextGate
 from onmt.modules.global_attention import GlobalAttention
 from onmt.modules.conv_multi_step_attention import ConvMultiStepAttention
 from onmt.modules.copy_generator import CopyGenerator, CopyGeneratorLoss
 from onmt.modules.multi_headed_attn import MultiHeadedAttention
 from onmt.modules.embeddings import Embeddings, PositionalEncoding
 from onmt.modules.weight_norm import WeightNormConv2d
 from onmt.modules.average_attn import AverageAttention
 from onmt.modules.alibi_position_bias import AlibiPositionalBias
-from onmt.modules.lora import LoRALayer, Embedding, Linear, MergedLinear
-from onmt.modules.lora import mark_only_lora_as_trainable, lora_state_dict
 from onmt.modules.rmsnorm import RMSNorm
 
+
 __all__ = [
     "Elementwise",
     "context_gate_factory",
     "ContextGate",
     "GlobalAttention",
     "ConvMultiStepAttention",
     "CopyGenerator",
@@ -25,14 +26,8 @@
     "MultiHeadedAttention",
     "Embeddings",
     "PositionalEncoding",
     "AlibiPositionalBias",
     "WeightNormConv2d",
     "AverageAttention",
     "RMSNorm",
-    "LoRALayer",
-    "Embedding",
-    "Linear",
-    "MergedLinear",
-    "mark_only_lora_as_trainable",
-    "lora_state_dict",
 ]
```

### Comparing `OpenNMT-py-3.1.3/onmt/modules/alibi_position_bias.py` & `OpenNMT-py-3.2.0/onmt/modules/alibi_position_bias.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/modules/average_attn.py` & `OpenNMT-py-3.2.0/onmt/modules/average_attn.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/modules/conv_multi_step_attention.py` & `OpenNMT-py-3.2.0/onmt/modules/conv_multi_step_attention.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/modules/copy_generator.py` & `OpenNMT-py-3.2.0/onmt/modules/copy_generator.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/modules/embeddings.py` & `OpenNMT-py-3.2.0/onmt/modules/embeddings.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/modules/gate.py` & `OpenNMT-py-3.2.0/onmt/modules/gate.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/modules/global_attention.py` & `OpenNMT-py-3.2.0/onmt/modules/global_attention.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/modules/multi_headed_attn.py` & `OpenNMT-py-3.2.0/onmt/modules/multi_headed_attn.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """ Multi-Head Attention module """
 import math
 import torch
 from torch import Tensor
 from typing import Optional, Tuple
 import torch.nn as nn
+from torch.utils.checkpoint import checkpoint
+from torch.nn.utils import skip_init
 from .alibi_position_bias import AlibiPositionalBias
 
 
 # Help functions for Rotary Embeddings
 # https://arxiv.org/pdf/2104.09864.pdf
 # too convoluted to make maxseqlen a parameter.
 # we suppose src_seq_len at training and max_length at inference
@@ -147,26 +149,56 @@
         self,
         head_count: int,
         model_dim: int,
         dropout: float = 0.1,
         max_relative_positions: int = 0,
         attn_type: str = None,
         add_qkvbias=False,
+        multiquery=False,
+        use_ckpting=[],
     ) -> None:
         assert model_dim % head_count == 0
         self.dim_per_head = model_dim // head_count
         super(MultiHeadedAttention, self).__init__()
         self.head_count = head_count
-
-        self.linear_keys = nn.Linear(model_dim, model_dim, bias=add_qkvbias)
-        self.linear_values = nn.Linear(model_dim, model_dim, bias=add_qkvbias)
-        self.linear_query = nn.Linear(model_dim, model_dim, bias=add_qkvbias)
+        self.multiquery = multiquery
+        if not multiquery:
+            self.linear_keys = skip_init(
+                nn.Linear,
+                in_features=model_dim,
+                out_features=model_dim,
+                bias=add_qkvbias,
+            )
+            self.linear_values = skip_init(
+                nn.Linear,
+                in_features=model_dim,
+                out_features=model_dim,
+                bias=add_qkvbias,
+            )
+        else:
+            self.linear_keys = skip_init(
+                nn.Linear,
+                in_features=model_dim,
+                out_features=self.dim_per_head,
+                bias=add_qkvbias,
+            )
+            self.linear_values = skip_init(
+                nn.Linear,
+                in_features=model_dim,
+                out_features=self.dim_per_head,
+                bias=add_qkvbias,
+            )
+        self.linear_query = skip_init(
+            nn.Linear, in_features=model_dim, out_features=model_dim, bias=add_qkvbias
+        )
         self.softmax = nn.Softmax(dim=-1)
         self.dropout = nn.Dropout(dropout)
-        self.final_linear = nn.Linear(model_dim, model_dim, bias=add_qkvbias)
+        self.final_linear = skip_init(
+            nn.Linear, in_features=model_dim, out_features=model_dim, bias=add_qkvbias
+        )
 
         self.max_relative_positions = max_relative_positions
         self.attn_type = attn_type
         self.layer_cache = (
             False,
             {"keys": torch.tensor([]), "values": torch.tensor([])},
         )
@@ -185,14 +217,16 @@
 
             if max_relative_positions == -1:  # rotary embeddings
                 self.rope = rotaryembeddings(self.dim_per_head)
 
             if max_relative_positions == -2:  # alibi positional bias
                 self.alibi = AlibiPositionalBias(head_count)
 
+        self.maybe_ckpt = checkpoint if "mha" in use_ckpting else lambda f, x: f(x)
+
     def update_dropout(self, dropout: float) -> None:
         self.dropout.p = dropout
 
     # @torch.jit.script_method
     def forward(
         self,
         key: Tensor,
@@ -262,17 +296,17 @@
                     key, value = (
                         self.layer_cache[1]["keys"],
                         self.layer_cache[1]["values"],
                     )
                 self.layer_cache[1]["keys"] = key
                 self.layer_cache[1]["values"] = value
         else:
-            key = self.linear_keys(key)
-            value = self.linear_values(value)
-            query = self.linear_query(query)
+            key = self.maybe_ckpt(self.linear_keys, key)
+            value = self.maybe_ckpt(self.linear_values, value)
+            query = self.maybe_ckpt(self.linear_query, query)
             key = shape(key, self.dim_per_head)
             value = shape(value, self.dim_per_head)
             query = shape(query, self.dim_per_head)
 
             if self.max_relative_positions == -1:  # Rotary Embeddings
                 start_pos = 0
                 seqlen = query.size(2)
@@ -280,36 +314,34 @@
 
                 query = query.transpose(1, 2)
                 key = key.transpose(1, 2)
                 query, key = apply_rotary_emb(query, key, rope=rope)
                 query = query.transpose(1, 2)
                 key = key.transpose(1, 2)
         # 2) Calculate and scale scores.
-        query = query / math.sqrt(self.dim_per_head)
+        query /= math.sqrt(self.dim_per_head)
         # batch x num_heads x query_len x key_len
-        query_key = torch.matmul(query, key.transpose(2, 3))
+        scores = torch.matmul(query, key.transpose(2, 3))
 
         if self.relative_positions_embeddings is not None:
             key_len = key.size(2)
             # 1 or key_len x key_len
             relative_positions_matrix = gen_relative_positions(
                 key_len,
                 self.max_relative_positions,
                 cache=self.layer_cache[0],
                 device=key.device,
             )
             #  1 or key_len x key_len x dim_per_head
             relations_keys = self.relative_positions_embeddings(
                 relative_positions_matrix
             )
-            scores = query_key + relative_matmul(query, relations_keys, True)
-        elif self.max_relative_positions == -2:
-            scores = self.alibi(query_key)
-        else:
-            scores = query_key
+            scores.add_(relative_matmul(query, relations_keys, True))
+        elif self.max_relative_positions == -2:  # Alibi
+            scores = self.alibi(scores)
 
         scores = scores.float()
 
         if mask is not None:
             # not 100% necessary but expand to nb of heads
             mask = mask.expand(-1, self.head_count, -1, -1)
             # now mask and scores have the same shape
@@ -320,16 +352,14 @@
         drop_attn = self.dropout(attn)
 
         context_original = torch.matmul(drop_attn, value)
 
         if self.relative_positions_embeddings is not None:
             # We use the same embeddings for key and value
             relations_values = relations_keys
-            context = unshape(
-                context_original + relative_matmul(drop_attn, relations_values, False)
-            )
-        else:
-            context = unshape(context_original)
+            context_original.add_(relative_matmul(drop_attn, relations_values, False))
+
+        context = unshape(context_original)
 
-        output = self.final_linear(context)
+        attn_output = self.maybe_ckpt(self.final_linear, context)
 
-        return output, attn
+        return attn_output, attn
```

### Comparing `OpenNMT-py-3.1.3/onmt/modules/position_ffn.py` & `OpenNMT-py-3.2.0/onmt/modules/position_ffn.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """Position feed-forward network from "Attention is All You Need"."""
 
 
 import torch.nn as nn
 import torch.nn.functional as F
+from torch.utils.checkpoint import checkpoint
 from onmt.modules.rmsnorm import RMSNorm
+from torch.nn.utils import skip_init
 
 
 class ActivationFunction(object):
     relu = "relu"
     gelu = "gelu"
     silu = "silu"
 
@@ -34,48 +36,62 @@
 
     def __init__(
         self,
         d_model,
         d_ff,
         dropout=0.1,
         activation_fn=ActivationFunction.relu,
+        add_ffnbias=True,
+        parallel_residual=False,
         layer_norm="standard",
+        use_ckpting=[],
     ):
         super(PositionwiseFeedForward, self).__init__()
-        self.w_1 = nn.Linear(d_model, d_ff)
-        self.w_2 = nn.Linear(d_ff, d_model)
-        if layer_norm == "standard":
+        self.w_1 = skip_init(
+            nn.Linear, in_features=d_model, out_features=d_ff, bias=add_ffnbias
+        )
+        self.w_2 = skip_init(
+            nn.Linear, in_features=d_ff, out_features=d_model, bias=add_ffnbias
+        )
+        if layer_norm == "standard" and not parallel_residual:
             self.layer_norm = nn.LayerNorm(d_model, eps=1e-6)
-        elif layer_norm == "rms":
+        elif layer_norm == "rms" and not parallel_residual:
             self.layer_norm = RMSNorm(d_model, eps=1e-6)
-        else:
+        elif not parallel_residual:
             raise ValueError(f"{layer_norm} layer norm type is not supported")
+        self.parallel_residual = parallel_residual
         self.dropout_1 = nn.Dropout(dropout)
         self.activation = ACTIVATION_FUNCTIONS[activation_fn]
         self.dropout_2 = nn.Dropout(dropout)
         if activation_fn == "silu":
-            self.w_3 = nn.Linear(d_model, d_ff)
+            self.w_3 = skip_init(
+                nn.Linear, in_features=d_model, out_features=d_ff, bias=add_ffnbias
+            )
         else:
             self.w_3 = None
+        self.maybe_ckpt = checkpoint if "ffn" in use_ckpting else lambda f, x: f(x)
 
     def forward(self, x):
         """Layer definition.
 
         Args:
             x: ``(batch_size, input_len, model_dim)``
 
         Returns:
             (FloatTensor): Output ``(batch_size, input_len, model_dim)``.
         """
-        if self.w_3 is None:
-            inter = self.dropout_1(self.activation(self.w_1(self.layer_norm(x))))
+        if not self.parallel_residual:
+            norm_x = self.layer_norm(x)
         else:
-            inter = self.dropout_1(
-                self.activation(self.w_1(self.layer_norm(x)))
-                * self.w_3(self.layer_norm(x))
-            )
-        output = self.dropout_2(self.w_2(inter))
-        return output + x
+            norm_x = x
+        inter = self.maybe_ckpt(self.w_1, norm_x)
+        inter = self.activation(inter)
+        if self.w_3 is not None:
+            inter.mul_(self.maybe_ckpt(self.w_3, norm_x))
+        inter = self.dropout_1(inter)
+        inter = self.maybe_ckpt(self.w_2, inter)
+        inter = self.dropout_2(inter)
+        return inter + x
 
     def update_dropout(self, dropout):
         self.dropout_1.p = dropout
         self.dropout_2.p = dropout
```

### Comparing `OpenNMT-py-3.1.3/onmt/modules/rmsnorm.py` & `OpenNMT-py-3.2.0/onmt/modules/rmsnorm.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/modules/sparse_activations.py` & `OpenNMT-py-3.2.0/onmt/modules/sparse_activations.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/modules/sparse_losses.py` & `OpenNMT-py-3.2.0/onmt/modules/sparse_losses.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/modules/sru.py` & `OpenNMT-py-3.2.0/onmt/modules/sru.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/modules/stacked_rnn.py` & `OpenNMT-py-3.2.0/onmt/modules/stacked_rnn.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/modules/structured_attention.py` & `OpenNMT-py-3.2.0/onmt/modules/structured_attention.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/modules/util_class.py` & `OpenNMT-py-3.2.0/onmt/modules/util_class.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/modules/weight_norm.py` & `OpenNMT-py-3.2.0/onmt/modules/weight_norm.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/opts.py` & `OpenNMT-py-3.2.0/onmt/opts.py`

 * *Files 1% similar despite different names*

```diff
@@ -834,14 +834,33 @@
     group.add(
         "--add_qkvbias",
         "-add_qkvbias",
         action="store_true",
         help="Add bias to nn.linear of Query/Key/Value in MHA"
         "Note: this will add bias to output proj layer too",
     )
+    group.add(
+        "--multiquery",
+        "-multiquery",
+        action="store_true",
+        help="Use MultiQUery attention" "Note: https://arxiv.org/pdf/1911.02150.pdf",
+    )
+    group.add(
+        "--add_ffnbias",
+        "-add_ffnbias",
+        action="store_true",
+        help="Add bias to nn.linear of Position_wise FFN",
+    )
+    group.add(
+        "--parallel_residual",
+        "-parallel_residual",
+        action="store_true",
+        help="Use Parallel residual in Decoder Layer"
+        "Note: this is used by GPT-J / Falcon Architecture",
+    )
 
     # Alignement options
     group = parser.add_argument_group("Model - Alignement")
     group.add(
         "--lambda_align",
         "-lambda_align",
         type=float,
@@ -962,14 +981,23 @@
         "-apex_opt_level",
         type=str,
         default="",
         choices=["", "O0", "O1", "O2", "O3"],
         help="For FP16 training, the opt_level to use."
         "See https://nvidia.github.io/apex/amp.html#opt-levels.",
     )
+    group.add(
+        "--use_ckpting",
+        "-use_ckpting",
+        default=[],
+        nargs="+",
+        choices=["ffn", "mha", "lora"],
+        type=str,
+        help="use gradient checkpointing those modules",
+    )
 
 
 def _add_train_general_opts(parser):
     """General options for training"""
     group = parser.add_argument_group("General")
     group.add(
         "--data_type",
@@ -1088,15 +1116,24 @@
 
     group.add(
         "--quant_layers",
         "-quant_layers",
         default=[],
         nargs="+",
         type=str,
-        help="list of layers to be compressed in 8bit.",
+        help="list of layers to be compressed in 4/8bit.",
+    )
+
+    group.add(
+        "--quant_type",
+        "-quant_type",
+        default="bnb_8bit",
+        choices=["bnb_8bit", "bnb_FP4", "bnb_NF4"],
+        type=str,
+        help="Type of compression.",
     )
 
     _add_reproducibility_opts(parser)
 
     # Init options
     group = parser.add_argument_group("Initialization")
     group.add(
@@ -1266,14 +1303,17 @@
             "sgd",
             "adagrad",
             "adadelta",
             "adam",
             "sparseadam",
             "adafactor",
             "fusedadam",
+            "adamw8bit",
+            "pagedadamw8bit",
+            "pagedadamw32bit",
         ],
         help="Optimization method.",
     )
     group.add(
         "--adagrad_accumulator_init",
         "-adagrad_accumulator_init",
         type=float,
```

### Comparing `OpenNMT-py-3.1.3/onmt/scorers/__init__.py` & `OpenNMT-py-3.2.0/onmt/scorers/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/scorers/scorer.py` & `OpenNMT-py-3.2.0/onmt/scorers/scorer.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/tests/test_attention.py` & `OpenNMT-py-3.2.0/onmt/tests/test_attention.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/tests/test_beam_search.py` & `OpenNMT-py-3.2.0/onmt/tests/test_beam_search.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/tests/test_copy_generator.py` & `OpenNMT-py-3.2.0/onmt/tests/test_copy_generator.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/tests/test_data_prepare.py` & `OpenNMT-py-3.2.0/onmt/tests/test_data_prepare.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/tests/test_embeddings.py` & `OpenNMT-py-3.2.0/onmt/tests/test_embeddings.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/tests/test_events.py` & `OpenNMT-py-3.2.0/onmt/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/tests/test_greedy_search.py` & `OpenNMT-py-3.2.0/onmt/tests/test_greedy_search.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/tests/test_models.py` & `OpenNMT-py-3.2.0/onmt/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/tests/test_subword_marker.py` & `OpenNMT-py-3.2.0/onmt/tests/test_subword_marker.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/tests/test_text_utils.py` & `OpenNMT-py-3.2.0/onmt/tests/test_text_utils.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/tests/test_transform.py` & `OpenNMT-py-3.2.0/onmt/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/tests/test_translation_server.py` & `OpenNMT-py-3.2.0/onmt/tests/test_translation_server.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/tests/test_translator.py` & `OpenNMT-py-3.2.0/onmt/tests/test_translator.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/train_single.py` & `OpenNMT-py-3.2.0/onmt/train_single.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,15 +119,15 @@
         if opt.override_opts:
             logger.info("Over-ride model option set to true - use with care")
             args = list(opt.__dict__.keys())
             model_args = list(model_opt.__dict__.keys())
             for arg in args:
                 if arg in model_args and getattr(opt, arg) != getattr(model_opt, arg):
                     logger.info(
-                        "Option: %s , value: %s overiding model: %s"
+                        "Option: %s , value: %s overriding model: %s"
                         % (arg, getattr(opt, arg), getattr(model_opt, arg))
                     )
             model_opt = opt
         else:
             model_opt = ArgumentParser.ckpt_model_opts(checkpoint["opt"])
             ArgumentParser.update_model_opts(model_opt)
             ArgumentParser.validate_model_opts(model_opt)
@@ -174,31 +174,40 @@
 def main(opt, device_id):
     """Start training on `device_id`."""
     # NOTE: It's important that ``opt`` has been validated and updated
     # at this point.
 
     configure_process(opt, device_id)
     init_logger(opt.log_file)
-
     checkpoint, vocabs, transforms_cls = _init_train(opt)
     model_opt = _get_model_opts(opt, checkpoint=checkpoint)
 
     # Build model.
     model = build_model(model_opt, opt, vocabs, checkpoint)
 
     model.count_parameters(log=logger.info)
+    trainable, non_trainable = 0, 0
+    for n, p in model.named_parameters():
+        if p.requires_grad:
+            trainable += p.numel()
+        else:
+            non_trainable += p.numel()
+    logger.info("Trainable parameters = %d" % trainable)
+    logger.info("Non trainable parameters = %d" % non_trainable)
     logger.info(" * src vocab size = %d" % len(vocabs["src"]))
     logger.info(" * tgt vocab size = %d" % len(vocabs["tgt"]))
     if "src_feats" in vocabs:
         for i, feat_vocab in enumerate(vocabs["src_feats"]):
             logger.info(f"* src_feat {i} vocab size = {len(feat_vocab)}")
 
     # Build optimizer.
     optim = Optimizer.from_opt(model, opt, checkpoint=checkpoint)
 
+    del checkpoint
+
     # Build model saver
     model_saver = build_model_saver(model_opt, opt, model, vocabs, optim)
 
     trainer = build_trainer(
         opt, device_id, model, vocabs, optim, model_saver=model_saver
     )
```

### Comparing `OpenNMT-py-3.1.3/onmt/trainer.py` & `OpenNMT-py-3.2.0/onmt/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             opt.early_stopping, scorers=onmt.utils.scorers_from_opts(opt)
         )
         if opt.early_stopping > 0
         else None
     )
 
     report_manager = onmt.utils.build_report_manager(opt, gpu_rank)
-    trainer = onmt.Trainer(
+    trainer = Trainer(
         model,
         train_loss,
         valid_loss,
         scoring_preparator,
         train_scorers,
         valid_scorers,
         optim,
@@ -542,15 +542,14 @@
                                     metric, self.train_scorers[metric]["value"]
                                 )
                             )
                             computed_metrics[metric] = self.train_scorers[metric][
                                 "value"
                             ]
                         batch_stats.computed_metrics = computed_metrics
-
                     if loss is not None:
                         loss /= normalization
                         self.optim.backward(loss)
 
                     total_stats.update(batch_stats)
                     report_stats.update(batch_stats)
 
@@ -577,14 +576,15 @@
                 p.grad.data
                 for p in self.model.parameters()
                 if p.requires_grad and p.grad is not None
             ]
             onmt.utils.distributed.all_reduce_and_rescale_tensors(
                 grads, float(self.n_gpu)
             )
+
         self.optim.step()
 
     def _start_report_manager(self, start_time=None):
         """Simple function to start report manager (if any)"""
 
         if self.report_manager is not None:
             if start_time is None:
```

### Comparing `OpenNMT-py-3.1.3/onmt/transforms/__init__.py` & `OpenNMT-py-3.2.0/onmt/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/transforms/bart.py` & `OpenNMT-py-3.2.0/onmt/transforms/bart.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/transforms/clean.py` & `OpenNMT-py-3.2.0/onmt/transforms/clean.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/transforms/docify.py` & `OpenNMT-py-3.2.0/onmt/transforms/docify.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/transforms/features.py` & `OpenNMT-py-3.2.0/onmt/transforms/features.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/transforms/fuzzymatch.py` & `OpenNMT-py-3.2.0/onmt/transforms/fuzzymatch.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/transforms/inlinetags.py` & `OpenNMT-py-3.2.0/onmt/transforms/inlinetags.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from onmt.utils.logging import logger
 from onmt.transforms import register_transform
 from .transform import Transform
 
 import random
 import ahocorasick
 import string
+from typing import Tuple
 
 
 class InlineTagger(object):
     """Class for augmenting source and target sentences
     with inline tags (placeholders).
 
     It requires a prepared tab-delimited dictionary of source-target
@@ -43,33 +44,31 @@
         self.isolated_tag_prefix, self.isolated_tag_suffix = map(
             str, isolated_tag.split("#")
         )
 
         self.automaton = self._create_automaton()
 
     def _create_internal_dictionary(self, tags_dictionary_path):
-        logger.debug("Creating tag dictionary for tagging transform...")
         dictionary = list()
         with open(tags_dictionary_path, mode="r", encoding="utf-8") as file:
             pairs = file.readlines()
             for pair in pairs:
                 src_term, tgt_term = map(str, pair.split("\t"))
                 dictionary.append((src_term.strip(), tgt_term.strip()))
-        logger.debug(f"Created tag dictionary with {len(dictionary)} entries.")
         return dictionary
 
     def _create_automaton(self):
         automaton = ahocorasick.Automaton()
         for entry in self.internal_dictionary:
             automaton.add_word(entry[0], (entry[0], entry[1]))
 
         automaton.make_automaton()
         return automaton
 
-    def _tagged_src_tgt(self, src_example, tgt_example):
+    def _tagged_src_tgt(self, src_example, tgt_example) -> tuple:
         """Uses the dictionary to find exact source matches with corresponding
         target matches and adds both paired tags and standalone tags."""
 
         maybe_augmented = src_example.split(self.src_delimiter)
         source_only = maybe_augmented[0].strip()
 
         augmented_part = (
@@ -175,15 +174,15 @@
                     f"{self.isolated_tag_suffix}∥{tgt_term}∥"
                 )
                 tgt_paired_tags = (
                     f"{tgt_example[tgt_offset: tgt_match_start]}"
                     f"{self.paired_stag_prefix}{paired_tag_start_num}"
                     f"{self.paired_stag_suffix}∥{tgt_term}∥"
                     f"{self.paired_etag_prefix}{paired_tag_start_num}"
-                    f"{self.paired_etag_suffix}"
+                    f"{self.paired_etag_suffix}∥"
                 )
 
                 # Make a weighted choice between paired tags or single tags.
                 # We usually encounter, and thus here we favor, paired tags
                 # with a ratio 1/3.
                 choice = random.choices(
                     [src_single_tags, src_paired_tags], weights=(1, 3), k=1
@@ -211,17 +210,17 @@
                 src_with_tags.append(source_only[src_offset:])
 
             tgt_with_tags.append(tgt_example[tgt_offset:])
 
             return (
                 "".join(src_with_tags).replace("∥", " ").split(),
                 "".join(tgt_with_tags).replace("∥", " ").split(),
-            )
+            ), is_match
         else:
-            return (src_example.split(), tgt_example.split())
+            return (src_example.split(), tgt_example.split()), is_match
 
 
 @register_transform(name="inlinetags")
 class InlineTagsTransform(Transform):
     def __init__(self, opts):
         super().__init__(opts)
 
@@ -285,17 +284,14 @@
         )
 
     def _parse_opts(self):
         self.tags_dictionary_path = self.opts.tags_dictionary_path
         self.tags_corpus_ratio = self.opts.tags_corpus_ratio
         self.max_tags = self.opts.max_tags
         self.src_delimiter = self.opts.src_delimiter
-        self.paired_stag = (self.opts.paired_stag,)
-        self.paired_etag = (self.opts.paired_etag,)
-        self.isolated_tag = (self.opts.isolated_tag,)
 
     @classmethod
     def get_specials(cls, opts):
         """Add up to self.max_tags * 2 placeholders to src and tgt vocabs."""
 
         # Check if the tags include the
         # mandatory "#" number placeholder"
@@ -333,27 +329,37 @@
     def warm_up(self, vocabs=None):
         """Create the tagger."""
 
         super().warm_up(None)
         self.tagger = InlineTagger(
             self.tags_dictionary_path,
             self.max_tags,
-            self.paired_stag,
-            self.paired_etag,
-            self.isolated_tag,
+            self.opts.paired_stag,
+            self.opts.paired_etag,
+            self.opts.isolated_tag,
             self.src_delimiter,
             self.tags_corpus_ratio,
         )
 
-    def apply(self, example, is_train=False, stats=None, **kwargs):
-        """Add tags (placeholders) to source and target segments."""
+    def batch_apply(self, batch, is_train=False, stats=None, **kwargs):
+        bucket_size = len(batch)
+        examples_with_tags = 0
+
+        for (ex, _, _) in batch:
+            augmented_example, is_match = self.apply(ex, is_train, stats, **kwargs)
+            if is_match and (examples_with_tags < bucket_size * self.tags_corpus_ratio):
+                examples_with_tags += 1
+                ex["src"] = augmented_example["src"]
+                ex["tgt"] = augmented_example["tgt"]
+        logger.debug(f"Added tags to {examples_with_tags}/{bucket_size} examples")
+        return batch
 
-        if random.random() > self.tags_corpus_ratio:
-            return example
+    def apply(self, example, is_train=False, stats=None, **kwargs) -> tuple:
+        """Add tags (placeholders) to source and target segments."""
 
-        src_tgt_pair = self.tagger._tagged_src_tgt(
+        src_tgt_pair, is_match = self.tagger._tagged_src_tgt(
             " ".join(example["src"]), " ".join(example["tgt"])
         )
         example["src"] = src_tgt_pair[0]
         example["tgt"] = src_tgt_pair[1]
 
-        return example
+        return example, is_match
```

### Comparing `OpenNMT-py-3.1.3/onmt/transforms/misc.py` & `OpenNMT-py-3.2.0/onmt/transforms/misc.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/transforms/normalize.py` & `OpenNMT-py-3.2.0/onmt/transforms/normalize.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/transforms/sampling.py` & `OpenNMT-py-3.2.0/onmt/transforms/sampling.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/transforms/tokenize.py` & `OpenNMT-py-3.2.0/onmt/transforms/tokenize.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/transforms/transform.py` & `OpenNMT-py-3.2.0/onmt/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/transforms/uppercase.py` & `OpenNMT-py-3.2.0/onmt/transforms/uppercase.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/translate/__init__.py` & `OpenNMT-py-3.2.0/onmt/translate/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/translate/beam_search.py` & `OpenNMT-py-3.2.0/onmt/translate/beam_search.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/translate/decode_strategy.py` & `OpenNMT-py-3.2.0/onmt/translate/decode_strategy.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/translate/greedy_search.py` & `OpenNMT-py-3.2.0/onmt/translate/greedy_search.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/translate/penalties.py` & `OpenNMT-py-3.2.0/onmt/translate/penalties.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/translate/process_zh.py` & `OpenNMT-py-3.2.0/onmt/translate/process_zh.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/translate/translation.py` & `OpenNMT-py-3.2.0/onmt/translate/translation.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/translate/translation_server.py` & `OpenNMT-py-3.2.0/onmt/translate/translation_server.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/translate/translator.py` & `OpenNMT-py-3.2.0/onmt/translate/translator.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/utils/__init__.py` & `OpenNMT-py-3.2.0/onmt/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/utils/alignment.py` & `OpenNMT-py-3.2.0/onmt/utils/alignment.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/utils/cnn_factory.py` & `OpenNMT-py-3.2.0/onmt/utils/cnn_factory.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/utils/distributed.py` & `OpenNMT-py-3.2.0/onmt/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/utils/earlystopping.py` & `OpenNMT-py-3.2.0/onmt/utils/earlystopping.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/utils/logging.py` & `OpenNMT-py-3.2.0/onmt/utils/logging.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/utils/loss.py` & `OpenNMT-py-3.2.0/onmt/utils/loss.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/utils/misc.py` & `OpenNMT-py-3.2.0/onmt/utils/misc.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/utils/optimizers.py` & `OpenNMT-py-3.2.0/onmt/utils/optimizers.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import torch.optim as optim
 from torch.nn.utils import clip_grad_norm_
 import operator
 import functools
 from copy import copy
 from math import sqrt
 import types
+import os
 import importlib
 from onmt.utils.misc import fn_args
 
 try:
     import apex
 except ImportError:
     pass
@@ -95,14 +96,65 @@
                 static_loss_scale = opt.loss_scale
                 dynamic_loss_scale = opt.loss_scale == 0
                 optimizer = apex.contrib.optimizers.FP16_Optimizer(
                     optimizer,
                     static_loss_scale=static_loss_scale,
                     dynamic_loss_scale=dynamic_loss_scale,
                 )
+    elif opt.optim in ["adamw8bit", "pagedadamw8bit", "pagedadamw32bit"]:
+        try:
+            os.environ["BITSANDBYTES_NOWELCOME"] = "1"
+            import bitsandbytes as bnb
+        except ImportError:
+            raise ImportError("Install bitsandbytes to use bnb optimizers")
+        if opt.optim == "adamw8bit":
+            optimizer = bnb.optim.AdamW8bit(
+                params,
+                lr=opt.learning_rate,
+                betas=betas,
+                eps=1e-8,
+                weight_decay=1e-2,
+                amsgrad=False,
+                optim_bits=8,
+                args=None,
+                min_8bit_size=1024,
+                percentile_clipping=100,
+                block_wise=True,
+                is_paged=False,
+            )
+        elif opt.optim == "pagedadamw8bit":
+            optimizer = bnb.optim.PagedAdamW8bit(
+                params,
+                lr=opt.learning_rate,
+                betas=betas,
+                eps=1e-8,
+                weight_decay=1e-2,
+                amsgrad=False,
+                optim_bits=8,
+                args=None,
+                min_8bit_size=4096,
+                percentile_clipping=100,
+                block_wise=True,
+            )
+        elif opt.optim == "pagedadamw32bit":
+            optimizer = bnb.optim.PagedAdamW32bit(
+                params,
+                lr=opt.learning_rate,
+                betas=betas,
+                eps=1e-8,
+                weight_decay=1e-2,
+                amsgrad=False,
+                optim_bits=32,
+                args=None,
+                min_8bit_size=4096,
+                percentile_clipping=100,
+                block_wise=True,
+            )
+        else:
+            raise ValueError("Invalid optimizer type: " + opt.optim)
     else:
         raise ValueError("Invalid optimizer type: " + opt.optim)
 
     return optimizer
 
 
 def make_learning_rate_decay_fn(opt):
```

### Comparing `OpenNMT-py-3.1.3/onmt/utils/parse.py` & `OpenNMT-py-3.2.0/onmt/utils/parse.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/utils/report_manager.py` & `OpenNMT-py-3.2.0/onmt/utils/report_manager.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/utils/scoring_utils.py` & `OpenNMT-py-3.2.0/onmt/utils/scoring_utils.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/onmt/utils/statistics.py` & `OpenNMT-py-3.2.0/onmt/utils/statistics.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.1.3/setup.py` & `OpenNMT-py-3.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     long_description = f.read()
 
 setup(
     name="OpenNMT-py",
     description="A python implementation of OpenNMT",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="3.1.3",
+    version="3.2.0",
     packages=find_packages(),
     project_urls={
         "Documentation": "http://opennmt.net/OpenNMT-py/",
         "Forum": "http://forum.opennmt.net/",
         "Gitter": "https://gitter.im/OpenNMT/OpenNMT-py",
         "Source": "https://github.com/OpenNMT/OpenNMT-py/",
     },
```

