# Comparing `tmp/jac_nlp-1.4.0.9.tar.gz` & `tmp/jac_nlp-1.4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jac_nlp-1.4.0.9.tar", last modified: Tue Feb 14 17:26:33 2023, max compression
+gzip compressed data, was "jac_nlp-1.4.1.0.tar", last modified: Wed Jun  7 18:25:12 2023, max compression
```

## Comparing `jac_nlp-1.4.0.9.tar` & `jac_nlp-1.4.1.0.tar`

### file list

```diff
@@ -1,141 +1,205 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:33.744855 jac_nlp-1.4.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-02-14 17:26:33.744855 jac_nlp-1.4.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:33.720855 jac_nlp-1.4.0.9/jac_nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:33.724855 jac_nlp-1.4.0.9/jac_nlp/bart_sum/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/bart_sum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/bart_sum/bart_sum.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/bart_sum/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:33.724855 jac_nlp-1.4.0.9/jac_nlp/bi_enc/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/bi_enc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14063 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/bi_enc/bi_enc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12717 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/bi_enc/poly_enc.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/bi_enc/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/bi_enc/sent_enc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:33.724855 jac_nlp-1.4.0.9/jac_nlp/bi_enc/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/bi_enc/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/bi_enc/tests/test_bi_enc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:33.724855 jac_nlp-1.4.0.9/jac_nlp/bi_enc/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/bi_enc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/bi_enc/utils/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/bi_enc/utils/model_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     9975 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/bi_enc/utils/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8153 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/bi_enc/utils/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/bi_enc/utils/train.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/bi_enc/utils/train_config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:33.728855 jac_nlp-1.4.0.9/jac_nlp/bi_ner/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/bi_ner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/bi_ner/bi_ner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:33.728855 jac_nlp-1.4.0.9/jac_nlp/bi_ner/datamodel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/bi_ner/datamodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/bi_ner/datamodel/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/bi_ner/datamodel/example.py
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/bi_ner/datamodel/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:33.728855 jac_nlp-1.4.0.9/jac_nlp/bi_ner/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/bi_ner/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14986 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/bi_ner/model/base_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/bi_ner/model/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/bi_ner/model/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/bi_ner/model/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/bi_ner/model/tokenize_data.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/bi_ner/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:33.728855 jac_nlp-1.4.0.9/jac_nlp/bi_ner/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/bi_ner/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/bi_ner/tests/test_bi_ner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:33.728855 jac_nlp-1.4.0.9/jac_nlp/cl_summer/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/cl_summer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/cl_summer/cl_summer.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/cl_summer/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:33.732855 jac_nlp-1.4.0.9/jac_nlp/cl_summer/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/cl_summer/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/cl_summer/tests/test_cl_summer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:33.732855 jac_nlp-1.4.0.9/jac_nlp/ent_ext/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/ent_ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/ent_ext/config.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    14920 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/ent_ext/ent_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/ent_ext/entity_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/ent_ext/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:33.732855 jac_nlp-1.4.0.9/jac_nlp/ent_ext/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/ent_ext/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/ent_ext/tests/test_ent_ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:33.732855 jac_nlp-1.4.0.9/jac_nlp/fast_enc/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/fast_enc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/fast_enc/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    56442 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/fast_enc/example_training_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/fast_enc/fast_enc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/fast_enc/json_to_train.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/fast_enc/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:33.732855 jac_nlp-1.4.0.9/jac_nlp/fast_enc/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/fast_enc/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/fast_enc/tests/test_fast_enc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:33.736855 jac_nlp-1.4.0.9/jac_nlp/gpt2/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/gpt2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/gpt2/gpt2.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/gpt2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:33.736855 jac_nlp-1.4.0.9/jac_nlp/sbert_sim/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/sbert_sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/sbert_sim/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/sbert_sim/sbert_sim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:33.736855 jac_nlp-1.4.0.9/jac_nlp/sbert_sim/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/sbert_sim/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/sbert_sim/tests/test_sbert_sim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:33.736855 jac_nlp-1.4.0.9/jac_nlp/t5_sum/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/t5_sum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/t5_sum/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/t5_sum/t5_sum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:33.736855 jac_nlp-1.4.0.9/jac_nlp/t5_sum/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/t5_sum/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/t5_sum/tests/test_t5_sum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:33.740856 jac_nlp-1.4.0.9/jac_nlp/text_seg/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/text_seg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/text_seg/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/text_seg/text_seg.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:33.740856 jac_nlp-1.4.0.9/jac_nlp/tfm_ner/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/tfm_ner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/tfm_ner/entity_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/tfm_ner/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:33.740856 jac_nlp-1.4.0.9/jac_nlp/tfm_ner/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/tfm_ner/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/tfm_ner/tests/test_tfm_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/tfm_ner/tfm_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)     8895 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/tfm_ner/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:33.740856 jac_nlp-1.4.0.9/jac_nlp/tfm_ner/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/tfm_ner/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/tfm_ner/utils/data_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/tfm_ner/utils/model_config.json
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/tfm_ner/utils/train_config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:33.740856 jac_nlp-1.4.0.9/jac_nlp/topic_ext/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/topic_ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/topic_ext/action_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/topic_ext/config.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/topic_ext/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/topic_ext/topic_ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:33.744855 jac_nlp-1.4.0.9/jac_nlp/use_enc/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/use_enc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/use_enc/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:33.744855 jac_nlp-1.4.0.9/jac_nlp/use_enc/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/use_enc/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/use_enc/tests/test_use_enc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/use_enc/use_enc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:33.744855 jac_nlp-1.4.0.9/jac_nlp/use_qa/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/use_qa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/use_qa/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:33.744855 jac_nlp-1.4.0.9/jac_nlp/use_qa/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/use_qa/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/use_qa/tests/test_use_qa.py
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/use_qa/use_qa.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:33.744855 jac_nlp-1.4.0.9/jac_nlp/zs_classifier/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/zs_classifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/zs_classifier/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/jac_nlp/zs_classifier/zs_classifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-14 17:26:33.720855 jac_nlp-1.4.0.9/jac_nlp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-02-14 17:26:33.000000 jac_nlp-1.4.0.9/jac_nlp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-02-14 17:26:33.000000 jac_nlp-1.4.0.9/jac_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-14 17:26:33.000000 jac_nlp-1.4.0.9/jac_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-02-14 17:26:33.000000 jac_nlp-1.4.0.9/jac_nlp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-14 17:26:33.000000 jac_nlp-1.4.0.9/jac_nlp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-14 17:26:33.744855 jac_nlp-1.4.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-02-14 17:26:01.000000 jac_nlp-1.4.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:12.706768 jac_nlp-1.4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-07 18:25:12.706768 jac_nlp-1.4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    42252 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:12.678768 jac_nlp-1.4.1.0/jac_nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:12.682768 jac_nlp-1.4.1.0/jac_nlp/action_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/action_configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/action_configs/bart_sum_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/action_configs/bi_enc_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/action_configs/bi_ner_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/action_configs/cl_summer_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/action_configs/ent_ext_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/action_configs/fast_enc_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/action_configs/paraphraser_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/action_configs/sbert_sim_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/action_configs/sentiment_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3495 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/action_configs/t5_sum_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/action_configs/text_seg_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/action_configs/tfm_ner_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/action_configs/topic_ext_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/action_configs/use_enc_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/action_configs/use_qa_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/action_configs/zs_classifier_action_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:12.682768 jac_nlp-1.4.1.0/jac_nlp/bart_sum/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/bart_sum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/bart_sum/bart_sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/bart_sum/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:12.682768 jac_nlp-1.4.1.0/jac_nlp/bi_enc/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/bi_enc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14563 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/bi_enc/bi_enc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12713 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/bi_enc/poly_enc.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/bi_enc/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/bi_enc/sent_enc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:12.686768 jac_nlp-1.4.1.0/jac_nlp/bi_enc/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/bi_enc/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:12.686768 jac_nlp-1.4.1.0/jac_nlp/bi_enc/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/bi_enc/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/bi_enc/tests/fixtures/bi_enc.jac
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/bi_enc/tests/test_bi_enc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:12.686768 jac_nlp-1.4.1.0/jac_nlp/bi_enc/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/bi_enc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/bi_enc/utils/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/bi_enc/utils/model_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9975 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/bi_enc/utils/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8153 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/bi_enc/utils/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/bi_enc/utils/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/bi_enc/utils/train_config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:12.686768 jac_nlp-1.4.1.0/jac_nlp/bi_ner/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/bi_ner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7382 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/bi_ner/bi_ner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:12.686768 jac_nlp-1.4.1.0/jac_nlp/bi_ner/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/bi_ner/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/bi_ner/config/m_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/bi_ner/config/t_config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:12.686768 jac_nlp-1.4.1.0/jac_nlp/bi_ner/datamodel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/bi_ner/datamodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/bi_ner/datamodel/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/bi_ner/datamodel/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/bi_ner/datamodel/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:12.690768 jac_nlp-1.4.1.0/jac_nlp/bi_ner/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/bi_ner/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14986 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/bi_ner/model/base_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/bi_ner/model/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/bi_ner/model/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/bi_ner/model/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15772 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/bi_ner/model/ph_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/bi_ner/model/tokenize_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/bi_ner/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:12.690768 jac_nlp-1.4.1.0/jac_nlp/bi_ner/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/bi_ner/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:12.690768 jac_nlp-1.4.1.0/jac_nlp/bi_ner/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/bi_ner/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/bi_ner/tests/fixtures/bi_ner.jac
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/bi_ner/tests/test_bi_ner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:12.690768 jac_nlp-1.4.1.0/jac_nlp/cl_summer/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/cl_summer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/cl_summer/cl_summer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/cl_summer/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:12.690768 jac_nlp-1.4.1.0/jac_nlp/cl_summer/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/cl_summer/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:12.690768 jac_nlp-1.4.1.0/jac_nlp/cl_summer/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/cl_summer/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/cl_summer/tests/fixtures/cl_summer.jac
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/cl_summer/tests/test_cl_summer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:12.694768 jac_nlp-1.4.1.0/jac_nlp/dolly/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/dolly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/dolly/dolly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/dolly/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:12.694768 jac_nlp-1.4.1.0/jac_nlp/ent_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/ent_ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/ent_ext/config.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    15307 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/ent_ext/ent_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/ent_ext/entity_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/ent_ext/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:12.694768 jac_nlp-1.4.1.0/jac_nlp/ent_ext/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/ent_ext/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:12.694768 jac_nlp-1.4.1.0/jac_nlp/ent_ext/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/ent_ext/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/ent_ext/tests/fixtures/ent_ext.jac
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/ent_ext/tests/test_ent_ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:12.694768 jac_nlp-1.4.1.0/jac_nlp/gpt2/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/gpt2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/gpt2/gpt2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/gpt2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/gpt2/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:12.694768 jac_nlp-1.4.1.0/jac_nlp/gpt3/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/gpt3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/gpt3/gpt3.py
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/gpt3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:12.698768 jac_nlp-1.4.1.0/jac_nlp/paraphraser/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/paraphraser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/paraphraser/config.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/paraphraser/paraphraser.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/paraphraser/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:12.698768 jac_nlp-1.4.1.0/jac_nlp/paraphraser/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/paraphraser/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:12.698768 jac_nlp-1.4.1.0/jac_nlp/paraphraser/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/paraphraser/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/paraphraser/tests/fixtures/paraphraser.jac
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/paraphraser/tests/test_paraphraser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:12.698768 jac_nlp-1.4.1.0/jac_nlp/sbert_sim/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/sbert_sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/sbert_sim/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/sbert_sim/sbert_sim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:12.698768 jac_nlp-1.4.1.0/jac_nlp/sbert_sim/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/sbert_sim/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:12.698768 jac_nlp-1.4.1.0/jac_nlp/sbert_sim/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/sbert_sim/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/sbert_sim/tests/fixtures/sbert_sim.jac
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/sbert_sim/tests/test_sbert_sim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:12.698768 jac_nlp-1.4.1.0/jac_nlp/sentiment/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/sentiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/sentiment/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/sentiment/sentiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:12.698768 jac_nlp-1.4.1.0/jac_nlp/t5_sum/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/t5_sum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/t5_sum/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/t5_sum/t5_sum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:12.698768 jac_nlp-1.4.1.0/jac_nlp/t5_sum/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/t5_sum/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:12.698768 jac_nlp-1.4.1.0/jac_nlp/t5_sum/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/t5_sum/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/t5_sum/tests/fixtures/t5_sum.jac
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/t5_sum/tests/test_t5_sum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:12.702768 jac_nlp-1.4.1.0/jac_nlp/text_seg/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/text_seg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/text_seg/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/text_seg/text_seg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:12.702768 jac_nlp-1.4.1.0/jac_nlp/tfm_ner/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/tfm_ner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/tfm_ner/entity_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/tfm_ner/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:12.702768 jac_nlp-1.4.1.0/jac_nlp/tfm_ner/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/tfm_ner/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:12.702768 jac_nlp-1.4.1.0/jac_nlp/tfm_ner/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/tfm_ner/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/tfm_ner/tests/fixtures/tfm_ner.jac
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/tfm_ner/tests/test_tfm_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7412 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/tfm_ner/tfm_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/tfm_ner/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:12.702768 jac_nlp-1.4.1.0/jac_nlp/tfm_ner/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/tfm_ner/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/tfm_ner/utils/data_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/tfm_ner/utils/model_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/tfm_ner/utils/train_config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:12.702768 jac_nlp-1.4.1.0/jac_nlp/topic_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/topic_ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/topic_ext/action_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/topic_ext/config.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/topic_ext/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/topic_ext/topic_ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:12.706768 jac_nlp-1.4.1.0/jac_nlp/use_enc/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/use_enc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/use_enc/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:12.706768 jac_nlp-1.4.1.0/jac_nlp/use_enc/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/use_enc/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:12.706768 jac_nlp-1.4.1.0/jac_nlp/use_enc/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/use_enc/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/use_enc/tests/fixtures/use_enc.jac
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/use_enc/tests/test_use_enc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/use_enc/use_enc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:12.706768 jac_nlp-1.4.1.0/jac_nlp/use_qa/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/use_qa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/use_qa/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:12.706768 jac_nlp-1.4.1.0/jac_nlp/use_qa/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/use_qa/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:12.706768 jac_nlp-1.4.1.0/jac_nlp/use_qa/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/use_qa/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/use_qa/tests/fixtures/use_qa.jac
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/use_qa/tests/test_use_qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/use_qa/use_qa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:12.706768 jac_nlp-1.4.1.0/jac_nlp/zs_classifier/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/zs_classifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/zs_classifier/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/jac_nlp/zs_classifier/zs_classifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:25:12.678768 jac_nlp-1.4.1.0/jac_nlp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-07 18:25:12.000000 jac_nlp-1.4.1.0/jac_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-06-07 18:25:12.000000 jac_nlp-1.4.1.0/jac_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 18:25:12.000000 jac_nlp-1.4.1.0/jac_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-07 18:25:12.000000 jac_nlp-1.4.1.0/jac_nlp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-07 18:25:12.000000 jac_nlp-1.4.1.0/jac_nlp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 18:25:12.706768 jac_nlp-1.4.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-07 18:24:46.000000 jac_nlp-1.4.1.0/setup.py
```

### Comparing `jac_nlp-1.4.0.9/PKG-INFO` & `jac_nlp-1.4.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 Metadata-Version: 2.1
 Name: jac_nlp
-Version: 1.4.0.9
+Version: 1.4.1.0
 Home-page: https://github.com/Jaseci-Labs/jaseci
 Author: Jason Mars
 Author-email: jason@jaseci.org
 Provides-Extra: all
 Provides-Extra: bart_sum
 Provides-Extra: cl_summer
 Provides-Extra: ent_ext
-Provides-Extra: fast_enc
 Provides-Extra: sbert_sim
 Provides-Extra: t5_sum
 Provides-Extra: text_seg
 Provides-Extra: tfm_ner
 Provides-Extra: use_enc
 Provides-Extra: use_qa
 Provides-Extra: zs_classifier
 Provides-Extra: bi_enc
 Provides-Extra: topic_ext
 Provides-Extra: gpt2
+Provides-Extra: bi_ner
+Provides-Extra: gpt3
+Provides-Extra: sentiment
+Provides-Extra: paraphraser
+Provides-Extra: dolly
```

### Comparing `jac_nlp-1.4.0.9/jac_nlp/bart_sum/bart_sum.py` & `jac_nlp-1.4.1.0/jac_nlp/t5_sum/t5_sum.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,51 @@
-from transformers import BartTokenizer, BartForConditionalGeneration
 import torch
-from typing import List, Union
-from jaseci.actions.live_actions import jaseci_action
-import traceback
-from fastapi import HTTPException
-import requests
-from bs4 import BeautifulSoup
-
-
-device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
-
-bart_tokenizer = BartTokenizer.from_pretrained("facebook/bart-large-cnn")
-bart_model = BartForConditionalGeneration.from_pretrained("facebook/bart-large-cnn").to(
-    device
-)
-
-
-@jaseci_action(act_group=["bart_sum"], allow_remote=True)
-def summarize(
-    text: Union[List[str], str] = None,  # type: ignore
-    url: str = None,  # type: ignore
-    max_length: int = 100,
-    min_length: int = 10,
-    num_beams: int = 4,
-) -> List[str]:
-    try:
-        if text is not None:
-            if isinstance(text, str):
-                text = [text]
-        elif url is not None:
-            page = requests.get(url)
-            soup = BeautifulSoup(page.text, "html.parser")
-            text = [" ".join(map(lambda p: p.text, soup.find_all("p")))]
-        else:
-            raise HTTPException(status_code=400, detail="No text or url provided")
-
-        inputs = bart_tokenizer.batch_encode_plus(
-            text, max_length=1024, return_tensors="pt"
-        )
-        summary_ids = bart_model.generate(
-            inputs["input_ids"].to(device),
-            num_beams=num_beams,
-            max_length=max_length,
-            min_length=min_length,
-            early_stopping=True,
-        )
-        return bart_tokenizer.batch_decode(
-            summary_ids, skip_special_tokens=True, clean_up_tokenization_spaces=True
-        )
-    except Exception as e:
-        traceback.print_exc()
-        raise HTTPException(status_code=500, detail=str(e))
+from jaseci.jsorc.live_actions import jaseci_action
+from transformers import T5Tokenizer, T5ForConditionalGeneration  # , T5Config
+
+# from fastapi import HTTPException
+
+model = None
+tokenizer = None
+device = torch.device("cpu")
+
+
+@jaseci_action(act_group=["t5_sum"], allow_remote=True)
+def setup(model_name: str = "t5-small", tokenizer_name: str = "t5-small"):
+    global model, tokenizer
+    model = T5ForConditionalGeneration.from_pretrained(model_name)
+    tokenizer = T5Tokenizer.from_pretrained(tokenizer_name)
+
+
+# generates summary based on text
+def t5_generate_sum(text, min_length, max_length):
+    preprocess_text = text.strip().replace("\n", "")
+    t5_prepared_Text = "summarize: " + preprocess_text
+
+    tokenized_text = tokenizer.encode(t5_prepared_Text, return_tensors="pt").to(device)
+
+    summary_ids = model.generate(
+        tokenized_text,
+        num_beams=4,
+        no_repeat_ngram_size=2,
+        min_length=min_length,
+        max_length=max_length,
+        early_stopping=True,
+    )
+
+    output = tokenizer.decode(summary_ids[0], skip_special_tokens=True)
+
+    return output
+
+
+# summarize a large body of text using t5 model (small model)
+# which returns data at a fast rate.
+@jaseci_action(act_group=["t5_sum"], allow_remote=True)
+def classify_text(text: str, min_length: int = 30, max_length: int = 100):
+    output = t5_generate_sum(text, min_length, max_length)
+    return output
+
+
+if __name__ == "__main__":
+    from jaseci.jsorc.remote_actions import launch_server
+
+    launch_server(port=8000)
```

### Comparing `jac_nlp-1.4.0.9/jac_nlp/bi_enc/bi_enc.py` & `jac_nlp-1.4.1.0/jac_nlp/bi_enc/bi_enc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,54 +1,62 @@
 import os
 import torch
 from typing import Dict, List, Union
 from fastapi import HTTPException
 from transformers import AutoModel, AutoConfig, AutoTokenizer
 import traceback
 import numpy as np
-from jaseci.actions.live_actions import jaseci_action
+from jaseci.jsorc.live_actions import jaseci_action
+from jaseci.utils.utils import model_base_path
 import random
 import json
 import shutil
 
 from .utils.evaluate import get_embeddings  # noqa
 from .utils.models import BiEncoder  # noqa
 from .utils.train import train_model  # noqa
 
 
-# device = torch.device("cpu")
-# uncomment this if you wish to use GPU to train
-# this is commented out because this causes issues with
-# unittest on machines with GPU
 device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
+MODEL_BASE_PATH = model_base_path("jac_nlp/bi_enc")
 
 
 # funtion to set seed for the module
 def set_seed(seed):
     random.seed(seed)
     np.random.seed(seed)
     torch.manual_seed(seed)
 
 
-def config_setup():
+@jaseci_action(act_group=["bi_enc"], allow_remote=True)
+def setup():
     """
     Loading configurations from utils/config.cfg and
     initialize tokenizer and model
     """
     global model, tokenizer, model_config, train_config, t_config_fname, m_config_fname
     dirname = os.path.dirname(__file__)
     m_config_fname = os.path.join(dirname, "utils/model_config.json")
     t_config_fname = os.path.join(dirname, "utils/train_config.json")
     with open(m_config_fname, "r") as jsonfile:
         model_config = json.load(jsonfile)
     with open(t_config_fname, "r") as jsonfile:
         train_config = json.load(jsonfile)
-
+    os.makedirs(MODEL_BASE_PATH, exist_ok=True)
+    if all(
+        os.path.isfile(os.path.join(MODEL_BASE_PATH, file))
+        for file in ["config.json", "pytorch_model.bin"]
+    ):
+        trf_config = AutoConfig.from_pretrained(MODEL_BASE_PATH)
+    else:
+        trf_config = AutoConfig.from_pretrained(model_config["model_name"])
+        model = AutoModel.from_config(trf_config)
+        model.save_pretrained(MODEL_BASE_PATH)
+        del model
     train_config.update({"device": device.type})
-    trf_config = AutoConfig.from_pretrained(model_config["model_name"])
     tokenizer = AutoTokenizer.from_pretrained(
         model_config["model_name"], do_lower_case=True, clean_text=False
     )
     if model_config["shared"] is True:
         cont_bert = AutoModel.from_config(trf_config)
         cand_bert = cont_bert
         print("shared model created")
@@ -65,17 +73,14 @@
         loss_function=model_config["loss_function"],
     )
 
     model.to(train_config["device"])
     set_seed(train_config["seed"])
 
 
-config_setup()
-
-
 # API for getting the cosine similarity
 @jaseci_action(act_group=["bi_enc"], allow_remote=True)
 def cosine_sim(vec_a: List[float], vec_b: List[float]):
     """
     Caculate the cosine similarity score of two given vectors
     Param 1 - First vector
     Param 2 - Second vector
@@ -177,15 +182,15 @@
     """
     Take list of context, candidate, labels and trains the model
     """
     global model
     train_data = {"contexts": [], "candidates": [], "labels": []}
     if from_scratch is True:
         save_model(model_config["model_save_path"])
-        config_setup()
+        setup()
     model.train()
     try:
         if training_parameters is not None:
             with open(t_config_fname, "w+") as jsonfile:
                 train_config.update(training_parameters)
                 json.dump(train_config, jsonfile, indent=4)
         for data in dataset.keys():
@@ -285,15 +290,15 @@
     global model_config
     try:
         save_model(model_config["model_save_path"])
         with open(m_config_fname, "w+") as jsonfile:
             model_config.update(model_parameters)
             json.dump(model_config, jsonfile, indent=4)
 
-        config_setup()
+        setup()
         return "Config setup is complete."
 
     except Exception as e:
         raise HTTPException(status_code=500, detail=str(e))
 
 
 @jaseci_action(act_group=["bi_enc"], allow_remote=True)
@@ -305,16 +310,17 @@
         if not model_path.replace("_", "").isalnum():
             raise HTTPException(
                 status_code=400,
                 detail="""
                 Invalid model name. Model Name can only have Alphanumeric
                  and '_' characters.""",
             )
-        if not os.path.exists(model_path):
-            os.makedirs(model_path)
+        if not os.path.isabs(model_path):
+            model_path = os.path.join(MODEL_BASE_PATH, model_path)
+        os.makedirs(model_path, exist_ok=True)
         if model_config["shared"] is True:
             model.cont_bert.save_pretrained(model_path)
             tokenizer.save_vocabulary(model_path)
             print(f"Saving shared model to : {model_path}")
         else:
             cand_bert_path = os.path.join(model_path + "/cand_bert")
             cont_bert_path = os.path.join(model_path + "/cont_bert")
@@ -343,14 +349,16 @@
 
 @jaseci_action(act_group=["bi_enc"], allow_remote=True)
 def load_model(model_path):
     """
     loads the model from the provided model_path
     """
     global model, tokenizer
+    if not os.path.isabs(model_path):
+        model_path = os.path.join(MODEL_BASE_PATH, model_path)
     if not os.path.exists(model_path):
         raise HTTPException(status_code=404, detail="Model path is not available")
     try:
         with open(m_config_fname, "r") as jsonfile:
             model_config_data = json.load(jsonfile)
         if model_config_data["shared"] is True:
             trf_config = AutoConfig.from_pretrained(model_path, local_files_only=True)
@@ -384,10 +392,10 @@
         return f"[loaded model from] : {model_path}"
     except Exception as e:
         traceback.print_exc()
         raise HTTPException(status_code=500, detail=str(e))
 
 
 if __name__ == "__main__":
-    from jaseci.actions.remote_actions import launch_server
+    from jaseci.jsorc.remote_actions import launch_server
 
     launch_server(port=8000)
```

### Comparing `jac_nlp-1.4.0.9/jac_nlp/bi_enc/poly_enc.py` & `jac_nlp-1.4.1.0/jac_nlp/bi_enc/poly_enc.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from fastapi import HTTPException
 from transformers import AutoModel, AutoConfig, AutoTokenizer
 from utils.evaluate import get_embeddings, get_inference
 from utils.models import PolyEncoder
 import traceback
 import numpy as np
 from utils.train import train_model
-from jaseci.actions.live_actions import jaseci_action
+from jaseci.jsorc.live_actions import jaseci_action
 import random
 import json
 import shutil
 
 
 # device = torch.device("cpu")
 # uncomment this if you wish to use GPU to train
@@ -360,10 +360,10 @@
         return f"[loaded model from] : {model_path}"
     except Exception as e:
         traceback.print_exc()
         raise HTTPException(status_code=500, detail=str(e))
 
 
 if __name__ == "__main__":
-    from jaseci.actions.remote_actions import launch_server
+    from jaseci.jsorc.remote_actions import launch_server
 
     launch_server(port=8000)
```

### Comparing `jac_nlp-1.4.0.9/jac_nlp/bi_enc/sent_enc.py` & `jac_nlp-1.4.1.0/jac_nlp/bi_enc/sent_enc.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from torch.utils.data import DataLoader
 import nlpaug.augmenter.word as naw
 import torch
 import math
 from datetime import datetime
 import numpy as np
 from fastapi.responses import JSONResponse
-from jaseci.actions.live_actions import jaseci_action
+from jaseci.jsorc.live_actions import jaseci_action
 
 model_name = "bert-base-uncased"
 device = "cuda" if torch.cuda.is_available() else "cpu"
 num_epochs = 2
 model_save_path = (
     "output/sent_"
     + model_name.replace("/", "-")
```

### Comparing `jac_nlp-1.4.0.9/jac_nlp/bi_enc/tests/test_bi_enc.py` & `jac_nlp-1.4.1.0/jac_nlp/bi_enc/tests/test_bi_enc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from jaseci.utils.test_core import CoreTest, jac_testcase
-from jaseci.actions.live_actions import load_module_actions, unload_module
+from jaseci.jsorc.live_actions import load_module_actions, unload_module
 import pytest
+import shutil
+from os import path
 
 
 class BiEncTest(CoreTest):
     fixture_src = __file__
 
     @classmethod
     def setUpClass(cls):
@@ -71,7 +73,10 @@
         self.assertEqual(ret["success"], True)
 
     @classmethod
     def tearDownClass(cls):
         super(BiEncTest, cls).tearDownClass()
         ret = unload_module("jac_nlp.bi_enc.bi_enc")
         assert ret is True
+        for temp_path in ["modeloutput", "logoutput"]:
+            if path.exists(temp_path) and path.isdir(temp_path):
+                shutil.rmtree(temp_path)
```

### Comparing `jac_nlp-1.4.0.9/jac_nlp/bi_enc/utils/evaluate.py` & `jac_nlp-1.4.1.0/jac_nlp/bi_enc/utils/evaluate.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.0.9/jac_nlp/bi_enc/utils/models.py` & `jac_nlp-1.4.1.0/jac_nlp/bi_enc/utils/models.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.0.9/jac_nlp/bi_enc/utils/tokenizer.py` & `jac_nlp-1.4.1.0/jac_nlp/bi_enc/utils/tokenizer.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.0.9/jac_nlp/bi_enc/utils/train.py` & `jac_nlp-1.4.1.0/jac_nlp/bi_enc/utils/train.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.0.9/jac_nlp/bi_ner/bi_ner.py` & `jac_nlp-1.4.1.0/jac_nlp/bi_ner/bi_ner.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 import traceback
 from fastapi import HTTPException
 
 from .model.base_encoder import BI_Enc_NER
 from .model.inference import Bi_NER_Infer
 from .datamodel.utils import invert, get_category_id_mapping
 from .model.tokenize_data import get_datasets
-from jaseci.actions.live_actions import jaseci_action
+from jaseci.jsorc.live_actions import jaseci_action
 
 
-def config_setup(category_name: List[str] = None):
+@jaseci_action(act_group=["bi_ner"], allow_remote=True)
+def setup(category_name: List[str] = None):
     global model, example_encoder, category_id_mapping, device
     global model_args, m_config_fname, train_args, t_config_fname
 
     dirname = os.path.dirname(__file__)
     m_config_fname = os.path.join(dirname, "config/m_config.json")
     with open(m_config_fname, "r") as jsonfile:
         model_args = json.load(jsonfile)
@@ -33,18 +34,14 @@
         model.prepare_inputs,
         category_mapping=invert(category_id_mapping),
         no_entity_category=model_args["unk_category"],
     )
     device = model.device
 
 
-# initialize the model
-config_setup()
-
-
 @jaseci_action(act_group=["bi_ner"], allow_remote=True)
 def infer(contexts: List[str]):
     """
     Take list of context, candidate and return nearest candidate to the context
     """
     predicted_candidates = []
     try:
@@ -83,15 +80,15 @@
             json.dump(train_args, jsonfile, indent=4)
     category_name = list(
         set(ele["entity_type"] for val in dataset["annotations"] for ele in val)
     )
     def_category = list(category_id_mapping.values())
     def_category.pop(-1)
     if from_scratch or not (sorted(def_category) == sorted(category_name)):
-        config_setup(category_name=category_name)
+        setup(category_name=category_name)
     train_dataset = get_datasets(dataset, example_encoder)
 
     training_args = TrainingArguments(
         output_dir=train_args["logpath"],
         evaluation_strategy=train_args["evaluation_strategy"],
         learning_rate=train_args["learning_rate"],
         per_device_train_batch_size=train_args["train_batch_size"],
@@ -158,15 +155,15 @@
     global model_args
     try:
         model.save(train_args["logpath"])
         with open(m_config_fname, "w+") as jsonfile:
             model_args.update(model_parameters)
             json.dump(model_args, jsonfile, indent=4)
 
-        config_setup()
+        setup()
         return "Config setup is complete."
     except Exception as e:
         raise HTTPException(status_code=500, detail=str(e))
 
 
 @jaseci_action(act_group=["bi_ner"], allow_remote=True)
 def save_model(model_path: str):
@@ -202,10 +199,10 @@
         return f"[loaded model from] : {model_path}"
     except Exception as e:
         traceback.print_exc()
         raise HTTPException(status_code=500, detail=str(e))
 
 
 if __name__ == "__main__":
-    from jaseci.actions.remote_actions import launch_server
+    from jaseci.jsorc.remote_actions import launch_server
 
     launch_server(port=8000)
```

### Comparing `jac_nlp-1.4.0.9/jac_nlp/bi_ner/datamodel/example.py` & `jac_nlp-1.4.1.0/jac_nlp/bi_ner/datamodel/example.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.0.9/jac_nlp/bi_ner/datamodel/utils.py` & `jac_nlp-1.4.1.0/jac_nlp/bi_ner/datamodel/utils.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.0.9/jac_nlp/bi_ner/model/base_encoder.py` & `jac_nlp-1.4.1.0/jac_nlp/bi_ner/model/base_encoder.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.0.9/jac_nlp/bi_ner/model/inference.py` & `jac_nlp-1.4.1.0/jac_nlp/bi_ner/model/inference.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.0.9/jac_nlp/bi_ner/model/loss.py` & `jac_nlp-1.4.1.0/jac_nlp/bi_ner/model/loss.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.0.9/jac_nlp/bi_ner/model/metric.py` & `jac_nlp-1.4.1.0/jac_nlp/bi_ner/model/metric.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.0.9/jac_nlp/bi_ner/model/tokenize_data.py` & `jac_nlp-1.4.1.0/jac_nlp/bi_ner/model/tokenize_data.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.0.9/jac_nlp/bi_ner/tests/test_bi_ner.py` & `jac_nlp-1.4.1.0/jac_nlp/bi_ner/tests/test_bi_ner.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from jaseci.utils.test_core import CoreTest, jac_testcase
-from jaseci.actions.live_actions import load_module_actions, unload_module
+from jaseci.jsorc.live_actions import load_module_actions, unload_module
 import pytest
+import shutil
+from os import path
 
 
 class BiNERTest(CoreTest):
     fixture_src = __file__
 
     @classmethod
     def setUpClass(cls):
@@ -54,7 +56,10 @@
         self.assertEqual(ret["success"], True)
 
     @classmethod
     def tearDownClass(cls):
         super(BiNERTest, cls).tearDownClass()
         ret = unload_module("jac_nlp.bi_ner.bi_ner")
         assert ret is True
+        for temp_path in ["mypath", "result", "logoutput"]:
+            if path.exists(temp_path) and path.isdir(temp_path):
+                shutil.rmtree(temp_path)
```

### Comparing `jac_nlp-1.4.0.9/jac_nlp/cl_summer/cl_summer.py` & `jac_nlp-1.4.1.0/jac_nlp/cl_summer/cl_summer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from fastapi import HTTPException
 from sumy.summarizers.lex_rank import LexRankSummarizer
 from sumy.summarizers.lsa import LsaSummarizer
 from sumy.summarizers.luhn import LuhnSummarizer
 from sumy.nlp.tokenizers import Tokenizer
 from sumy.parsers.plaintext import PlaintextParser
-from jaseci.actions.live_actions import jaseci_action
+from jaseci.jsorc.live_actions import jaseci_action
 from sumy.parsers.html import HtmlParser
 from sumy.nlp.stemmers import Stemmer
 from sumy.utils import get_stop_words
 import nltk
 
 nltk.download("punkt")
 nltk.download("stopwords")
@@ -70,10 +70,10 @@
     for sentence in summarizer(parser.document, sent_count):
         sentences.append(str(sentence))
 
     return sentences
 
 
 if __name__ == "__main__":
-    from jaseci.actions.remote_actions import launch_server
+    from jaseci.jsorc.remote_actions import launch_server
 
     launch_server(port=8000)
```

### Comparing `jac_nlp-1.4.0.9/jac_nlp/cl_summer/tests/test_cl_summer.py` & `jac_nlp-1.4.1.0/jac_nlp/cl_summer/tests/test_cl_summer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from jaseci.utils.test_core import CoreTest, jac_testcase
-from jaseci.actions.live_actions import load_module_actions, unload_module
+from jaseci.jsorc.live_actions import load_module_actions, unload_module
 
 
 class ClSummerModule(CoreTest):
     fixture_src = __file__
 
     @classmethod
     def setUpClass(cls):
```

### Comparing `jac_nlp-1.4.0.9/jac_nlp/config.py` & `jac_nlp-1.4.1.0/jac_nlp/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from .action_configs.sbert_sim_action_config import SBERT_SIM_ACTION_CONFIG
 from .action_configs.text_seg_action_config import TEXT_SEG_ACTION_CONFIG
 from .action_configs.tfm_ner_action_config import TFM_NER_ACTION_CONFIG
 from .action_configs.topic_ext_action_config import TOPIC_EXT_ACTION_CONFIG
 from .action_configs.use_enc_action_config import USE_ENC_ACTION_CONFIG
 from .action_configs.use_qa_action_config import USE_QA_ACTION_CONFIG
 from .action_configs.zs_classifier_action_config import ZS_CLASSIFIER_ACTION_CONFIG
+from .action_configs.sentiment_action_config import SENTIMENT_ACTION_CONFIG
 
 ACTION_CONFIGS = {
     "bart_sum": BART_SUM_ACTION_CONFIG,
     "bi_enc": BI_ENC_ACTION_CONFIG,
     "bi_ner": BI_NER_ACTION_CONFIG,
     "cl_summer": CL_SUMMER_ACTION_CONFIG,
     "ent_ext": ENT_EXT_ACTION_CONFIG,
@@ -22,8 +23,9 @@
     "sbert_sim": SBERT_SIM_ACTION_CONFIG,
     "text_seg": TEXT_SEG_ACTION_CONFIG,
     "tfm_ner": TFM_NER_ACTION_CONFIG,
     "topic_ext": TOPIC_EXT_ACTION_CONFIG,
     "use_enc": USE_ENC_ACTION_CONFIG,
     "use_qa": USE_QA_ACTION_CONFIG,
     "zs_classifier": ZS_CLASSIFIER_ACTION_CONFIG,
+    "sentiment": SENTIMENT_ACTION_CONFIG,
 }
```

### Comparing `jac_nlp-1.4.0.9/jac_nlp/ent_ext/ent_ext.py` & `jac_nlp-1.4.1.0/jac_nlp/ent_ext/ent_ext.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 from random import random
 from typing import List, Optional, Dict
 from fastapi import HTTPException
 from flair.data import Corpus
 from flair.datasets import ColumnCorpus
 from flair.models import TARSTagger, SequenceTagger
+
 from flair.embeddings import WordEmbeddings, StackedEmbeddings, FlairEmbeddings
+from flair.file_utils import cached_path
+from flair.file_utils import cached_path
 from flair.data import Sentence
 from flair.trainers import ModelTrainer
 import pandas as pd
 from .entity_utils import create_data, create_data_new
 import configparser
-from jaseci.actions.live_actions import jaseci_action
+from jaseci.jsorc.live_actions import jaseci_action
 import torch
 import os
 from pathlib import Path
 from datetime import datetime
 import warnings
+from jaseci.utils.utils import model_base_path
+
+from jaseci.utils.utils import model_base_path
 
 warnings.filterwarnings("ignore")
 
 config = configparser.ConfigParser()
-
-
+MODEL_BASE_PATH = model_base_path("jac_nlp/ent_ext")
+TARS_NER_PATH = (
+    "https://nlp.informatik.hu-berlin.de/resources/models/tars-ner/tars-ner.pt"
+)
 # 1. initialize each embedding for LSTM
 embedding_types = [
     # GloVe embeddings
     WordEmbeddings("glove"),
     # contextual string embeddings, forward
     FlairEmbeddings("news-forward"),
     # contextual string embeddings, backward
@@ -34,36 +42,33 @@
 
 # embedding stack consists of Flair and GloVe embeddings
 embeddings = StackedEmbeddings(embeddings=embedding_types)
 
 device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
 
-def init_model(reload=False):
+@jaseci_action(act_group=["ent_ext"], allow_remote=True)
+def setup(reload=False):
     """create a tagger as per the model provided through config"""
 
     global tagger, NER_MODEL_NAME, NER_LABEL_TYPE, MODEL_TYPE, config
     if reload is False:
         config.read(os.path.join(os.path.dirname(__file__), "config.cfg"))
     NER_MODEL_NAME = config["TAGGER_MODEL"]["NER_MODEL"]
     NER_LABEL_TYPE = config["LABEL_TYPE"]["NER"]
     MODEL_TYPE = config["TAGGER_MODEL"]["MODEL_TYPE"]
     if MODEL_TYPE.lower() == "trfmodel" and NER_MODEL_NAME.lower() != "none":
         tagger = TARSTagger(embeddings=NER_MODEL_NAME)
     elif NER_MODEL_NAME.lower() != "none" and MODEL_TYPE.lower() in ["lstm", "gru"]:
-        tagger = SequenceTagger.load(NER_MODEL_NAME)
+        tagger = SequenceTagger.load(cached_path(NER_MODEL_NAME, MODEL_BASE_PATH))
     elif MODEL_TYPE.lower() in "tars" and NER_MODEL_NAME.lower() != "none":
-        tagger = TARSTagger.load(NER_MODEL_NAME)
+        tagger = TARSTagger.load(cached_path(TARS_NER_PATH, MODEL_BASE_PATH))
     print(f"loaded mode : [{NER_MODEL_NAME}]")
 
 
-# initialize the tagger
-init_model()
-
-
 def train_entity(train_params: dict):
     """
     funtion for training the model
     """
     global tagger, NER_MODEL_NAME, MODEL_TYPE
     # define columns
     columns = {0: "text", 1: "ner"}
@@ -365,15 +370,15 @@
 def load_model(model_path="default_path", default=False):
     """
     loads the model from the provided model_path
     """
     global tagger
     try:
         if default is True:
-            init_model()
+            setup()
             return f"[deafaul model loaded model from] : {config['TAGGER_MODEL']['NER_MODEL']}"  # noqa
         if type(model_path) is str:
             model_path = Path(model_path)
         if (model_path / "final-model.pt").exists():
             tagger.load_state_dict(
                 tagger.load(model_path / "final-model.pt").state_dict()
             )
@@ -399,17 +404,17 @@
 
     if ner_model or model_type:
         config["TAGGER_MODEL"]["NER_MODEL"] = ner_model
         config["TAGGER_MODEL"]["MODEL_TYPE"] = model_type
     with open("config.cfg", "w") as configfile:
         config.write(configfile)
     try:
-        init_model(reload=True)
+        setup(reload=True)
     except Exception as e:
         raise HTTPException(status_code=500, detail=str(e))
     return "Config setup is complete."
 
 
 if __name__ == "__main__":
-    from jaseci.actions.remote_actions import launch_server
+    from jaseci.jsorc.remote_actions import launch_server
 
     launch_server(port=8000)
```

### Comparing `jac_nlp-1.4.0.9/jac_nlp/ent_ext/entity_utils.py` & `jac_nlp-1.4.1.0/jac_nlp/ent_ext/entity_utils.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.0.9/jac_nlp/fast_enc/tests/test_fast_enc.py` & `jac_nlp-1.4.1.0/jac_nlp/ent_ext/tests/test_ent_ext.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,52 @@
 from jaseci.utils.test_core import CoreTest, jac_testcase
-from jaseci.actions.live_actions import load_module_actions, unload_module
+from jaseci.jsorc.live_actions import load_module_actions, unload_module
 import pytest
+import shutil
+from os import path
 
 
-class FastEncTest(CoreTest):
+class EntExtTest(CoreTest):
     fixture_src = __file__
     """
-    Test Class for Fast encoder Module to test the functionality of api's
+    Test Class for EntExt Module to test the functionality of api's
     """
 
     @classmethod
     def setUpClass(cls):
-        super(FastEncTest, cls).setUpClass()
-        ret = load_module_actions("jac_nlp.fast_enc")
+        super(EntExtTest, cls).setUpClass()
+        ret = load_module_actions("jac_nlp.ent_ext")
         assert ret is True
 
     @pytest.mark.order(1)
-    @jac_testcase("fast_enc.jac", "test_train")
-    def test_train(self, ret):
+    @jac_testcase("ent_ext.jac", "test_ent_ext_set_config")
+    def test_ent_ext_set_config(self, ret):
         self.assertEqual(ret["success"], True)
 
     @pytest.mark.order(2)
-    @jac_testcase("fast_enc.jac", "test_predict")
-    def test_predict(self, ret):
+    @jac_testcase("ent_ext.jac", "test_train_ner")
+    def test_train_ner(self, ret):
         self.assertEqual(ret["success"], True)
 
     @pytest.mark.order(3)
-    @jac_testcase("fast_enc.jac", "test_fast_enc_save_model")
-    def test_fast_enc_save_model(self, ret):
+    @jac_testcase("ent_ext.jac", "test_extract_entity")
+    def test_extract_entity(self, ret):
         self.assertEqual(ret["success"], True)
 
     @pytest.mark.order(4)
-    @jac_testcase("fast_enc.jac", "test_fast_enc_load_model")
-    def test_fast_enc_load_model(self, ret):
+    @jac_testcase("ent_ext.jac", "test_ent_ext_save_model")
+    def test_ent_ext_save_model(self, ret):
+        self.assertEqual(ret["success"], True)
+
+    @pytest.mark.order(5)
+    @jac_testcase("ent_ext.jac", "test_ent_ext_load_model")
+    def test_ent_ext_load_model(self, ret):
         self.assertEqual(ret["success"], True)
 
     @classmethod
     def tearDownClass(cls):
-        super(FastEncTest, cls).tearDownClass()
-        ret = unload_module("jac_nlp.fast_enc.fast_enc")
+        super(EntExtTest, cls).tearDownClass()
+        ret = unload_module("jac_nlp.ent_ext.ent_ext")
         assert ret is True
+        for temp_path in ["modeloutput", "train"]:
+            if path.exists(temp_path) and path.isdir(temp_path):
+                shutil.rmtree(temp_path)
```

### Comparing `jac_nlp-1.4.0.9/jac_nlp/gpt2/gpt2.py` & `jac_nlp-1.4.1.0/jac_nlp/gpt2/gpt2.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,45 +1,55 @@
-from transformers import pipeline, GPT2Tokenizer, GPT2Model
+from transformers import (
+    pipeline,
+    GPT2Tokenizer,
+    GPT2Model,
+    AutoTokenizer,
+    AutoModelWithLMHead,
+)
 import torch
-from jaseci.actions.live_actions import jaseci_action
+from jaseci.jsorc.live_actions import jaseci_action
 import traceback
 from fastapi import HTTPException
 from typing import List, Union
+import os
+from .train import prepare_data, load_dataset, get_trainer
+import shutil
 
 device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
 model = None
 tokenizer = None
 generator = None
 
 
-def setup(model_name: str = "gpt2-medium", get_embeddings: bool = False):
+@jaseci_action(act_group=["gpt2"], allow_remote=True)
+def setup(model_name: str = "gpt2", get_embeddings: bool = False):
     global model, tokenizer, generator
     if get_embeddings:
+        generator = None
         tokenizer = GPT2Tokenizer.from_pretrained(model_name)
         tokenizer.pad_token = tokenizer.eos_token
         model = GPT2Model.from_pretrained(model_name).to(device)
     else:
-        generator = pipeline("text-generation", model=model_name)
-
-
-setup(model_name="gpt2-medium", get_embeddings=False)
+        model, tokenizer = None, None
+        generator = pipeline("text-generation", model=model_name, tokenizer="gpt2")
 
 
 @jaseci_action(act_group=["gpt2"], allow_remote=True)
 def generate(
     text: Union[List[str], str],
     max_length: int = 30,
     min_length: int = 10,
     num_return_sequences: int = 3,
 ) -> List:
     global generator, model, tokenizer
     if generator is None:
         model, tokenizer = None, None
-        setup(model_name="gpt2-medium", get_embeddings=False)
+        model_name = "./gpt2-trained" if os.path.exists("gpt2-trained") else "gpt2"
+        setup(model_name=model_name, get_embeddings=False)
     try:
         if isinstance(text, str):
             text = [text]
         return generator(
             text,
             max_length=max_length,
             min_length=min_length,
@@ -51,24 +61,55 @@
 
 
 @jaseci_action(act_group=["gpt2"], allow_remote=True)
 def get_embeddings(text: Union[List[str], str]) -> List:
     global model, tokenizer, generator, device
     if model is None or tokenizer is None:
         generator = None
-        setup(model_name="gpt2-medium", get_embeddings=True)
+        setup(model_name="gpt2", get_embeddings=True)
     try:
         if isinstance(text, str):
             text = [text]
         inputs = tokenizer(text, return_tensors="pt", padding=True).to(device)
         with torch.no_grad():
             outputs = model(**inputs)
         return outputs.last_hidden_state.tolist()
     except Exception as e:
         traceback.print_exc()
         raise HTTPException(status_code=500, detail=str(e))
 
 
+@jaseci_action(act_group=["gpt2"], allow_remote=True)
+def train(
+    text: Union[List[str], str], epochs: int = 1, use_prev_trained=True, freeze=True
+):
+    if not use_prev_trained:
+        shutil.rmtree("gpt2-trained", ignore_errors=True)
+    tokenizer = AutoTokenizer.from_pretrained("gpt2")
+    train_path, test_path = prepare_data(text)
+    train_dataset, test_dataset, data_collator = load_dataset(
+        train_path, test_path, tokenizer
+    )
+    model_name = (
+        "./gpt2-trained"
+        if os.path.exists("gpt2-trained") and use_prev_trained
+        else "gpt2"
+    )
+    model = AutoModelWithLMHead.from_pretrained(model_name)
+
+    if freeze:
+        for param in model.parameters():
+            param.requires_grad = False
+        model.lm_head.weight.requires_grad = True
+
+    trainer = get_trainer(model, train_dataset, test_dataset, data_collator, epochs)
+    trainer.train()
+    trainer.save_model()
+
+    global generator
+    generator = pipeline("text-generation", model="./gpt2-trained", tokenizer="gpt2")
+
+
 if __name__ == "__main__":
-    from jaseci.actions.remote_actions import launch_server
+    from jaseci.jsorc.remote_actions import launch_server
 
     launch_server(port=8000)
```

### Comparing `jac_nlp-1.4.0.9/jac_nlp/sbert_sim/sbert_sim.py` & `jac_nlp-1.4.1.0/jac_nlp/sbert_sim/sbert_sim.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,27 +5,61 @@
 from torch import nn
 from torch.utils.data import DataLoader
 import torch
 import math
 from datetime import datetime
 import numpy as np
 from fastapi import HTTPException
-from jaseci.actions.live_actions import jaseci_action
+from jaseci.jsorc.live_actions import jaseci_action
+from jaseci.utils.utils import model_base_path
+import os
 
 """
 Declaring the training config
 """
 training_config: Dict = {
     "device": "cuda" if torch.cuda.is_available() else "cpu",
     "num_epochs": 2,
     "model_save_path": (
         "output/sent_model" + "-" + datetime.now().strftime("%Y-%m-%d_%H-%M-%S")
     ),
     "model_name": "bert-base-uncased",
 }
+MODEL_BASE_PATH = str(model_base_path("jac_nlp/sbert_sim"))
+
+
+@jaseci_action(act_group=["sbert_sim"], allow_remote=True)
+def setup(model_name="all-mpnet-base-v2"):
+    global model
+    os.makedirs(MODEL_BASE_PATH, exist_ok=True)
+    if all(
+        os.path.isfile(os.path.join(MODEL_BASE_PATH, f_name))
+        for f_name in ["pytorch_model.bin"]
+    ):
+        model = SentenceTransformer(MODEL_BASE_PATH)
+    else:
+        model = SentenceTransformer(model_name)
+        model.save(MODEL_BASE_PATH)
+
+
+SBERT_SIM_ROOT = str(model_base_path("jac_nlp/sbert_sim"))
+
+
+@jaseci_action(act_group=["sbert_sim"], allow_remote=True)
+def setup(model_name="all-mpnet-base-v2"):
+    global model
+    os.makedirs(SBERT_SIM_ROOT, exist_ok=True)
+    if all(
+        os.path.isfile(os.path.join(SBERT_SIM_ROOT, f_name))
+        for f_name in ["pytorch_model.bin"]
+    ):
+        model = SentenceTransformer(SBERT_SIM_ROOT)
+    else:
+        model = SentenceTransformer(model_name)
+        model.save(SBERT_SIM_ROOT)
 
 
 def create_model(model_name="bert-base-uncased", max_seq_length=256):
     """
     This fumctions can be used to create a custom sbert model from transformers
     model name :- valid transformer model from the hugging face hub
     max_seq_len :- the max_seq_len that it would support for tokenization
@@ -123,15 +157,15 @@
     text : contains a list of sentences to generate encodings
     Returns:  List of encoding for each text
     """
     global model
     model.eval()
     try:
         embeddings = model.encode(text)
-        return {np.squeeze(np.asarray(embeddings)).tolist()}
+        return np.squeeze(np.asarray(embeddings)).tolist()
     except Exception as e:
         print(e)
         return f"Error Occured : {str(e)}"
 
 
 @jaseci_action(act_group=["sbert_sim"], allow_remote=True)
 def get_cos_score(vec_a: list, vec_b: list):
@@ -152,15 +186,15 @@
     Param 2 - Second vector
     Return - float between 0 and 1
     """
     return np.asarray(dot_score(vec_a, vec_b)).tolist()
 
 
 @jaseci_action(act_group=["sbert_sim"], allow_remote=True)
-def load_model(model_name="all-MiniLM-L12-v2", model_type="default"):
+def load_model(model_name="all-mpnet-base-v2", model_type="default"):
     """
     Load models load in the memory for similarty scoring
     model_type : can be default or tfm_model
             default : loads model from the sbert model zoo
             tfm_model : load tranformer model from the huggingface hub
     model_name : this is name of the model to be loaded
     Returns: confirmation if the model is loaded
@@ -191,11 +225,10 @@
     try:
         return training_config
     except Exception as e:
         raise HTTPException(status_code=500, detail=str(e))
 
 
 if __name__ == "__main__":
-    from jaseci.actions.remote_actions import launch_server
+    from jaseci.jsorc.remote_actions import launch_server
 
-    load_model()
     launch_server(port=8000)
```

### Comparing `jac_nlp-1.4.0.9/jac_nlp/sbert_sim/tests/test_sbert_sim.py` & `jac_nlp-1.4.1.0/jac_nlp/sbert_sim/tests/test_sbert_sim.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from jaseci.utils.test_core import CoreTest, jac_testcase
-from jaseci.actions.live_actions import load_module_actions, unload_module
+from jaseci.jsorc.live_actions import load_module_actions, unload_module
 import pytest
+import shutil
+from os import path
 
 
 class SbertSimTest(CoreTest):
     fixture_src = __file__
 
     @classmethod
     def setUpClass(cls):
@@ -49,7 +51,10 @@
         self.assertEqual(ret["success"], True)
 
     @classmethod
     def tearDownClass(cls):
         super(SbertSimTest, cls).tearDownClass()
         ret = unload_module("jac_nlp.sbert_sim.sbert_sim")
         assert ret is True
+        for temp_path in ["output"]:
+            if path.exists(temp_path) and path.isdir(temp_path):
+                shutil.rmtree(temp_path)
```

### Comparing `jac_nlp-1.4.0.9/jac_nlp/t5_sum/tests/test_t5_sum.py` & `jac_nlp-1.4.1.0/jac_nlp/t5_sum/tests/test_t5_sum.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from jaseci.utils.test_core import CoreTest, jac_testcase
-from jaseci.actions.live_actions import load_module_actions, unload_module
+from jaseci.jsorc.live_actions import load_module_actions, unload_module
 import pytest
 
 
 class T5SumTest(CoreTest):
     fixture_src = __file__
     """
     Test Class for T5Sum Module to test the functionality of api's
```

### Comparing `jac_nlp-1.4.0.9/jac_nlp/text_seg/text_seg.py` & `jac_nlp-1.4.1.0/jac_nlp/text_seg/text_seg.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,60 @@
 import spacy
 from fastapi import HTTPException
 from transformers import AutoTokenizer, AutoModelForSequenceClassification
 import torch
-from jaseci.actions.live_actions import jaseci_action
+from jaseci.jsorc.live_actions import jaseci_action
+import os
+from jaseci.utils.utils import model_base_path
+
+
+"""
+1. Get the path to the home directory
+2. Download the model to the jaseci/models directory
+"""
+
+
+TFM_MODEL_NAME = "dennlinger/roberta-cls-consec"
+SPACY_MODEL_NAME = "en_core_web_sm"
+MODEL_BASE_PATH = model_base_path("jac_nlp/text_seg")
+os.makedirs(MODEL_BASE_PATH, exist_ok=True)
+TFM_MODEL_PATH = os.path.join(MODEL_BASE_PATH, TFM_MODEL_NAME)
+SPACY_MODEL_PATH = os.path.join(MODEL_BASE_PATH, SPACY_MODEL_NAME)
 
-# loading segmentation model from hugging face
-tokenizer = AutoTokenizer.from_pretrained("dennlinger/roberta-cls-consec")
-model = AutoModelForSequenceClassification.from_pretrained(
-    "dennlinger/roberta-cls-consec"
-)
-# Download the pretrained model pipeline
-spacy.cli.download("en_core_web_sm")
-# loading space model for sentence tokenization
-pipeline = spacy.load("en_core_web_sm")
+
+@jaseci_action(act_group=["text_seg"], allow_remote=True)
+def setup():
+    """
+    initialize tokenizer and model
+    """
+    global pipeline, tokenizer, model
+
+    try:
+        pipeline = spacy.load(SPACY_MODEL_PATH)
+    except OSError:
+        spacy.cli.download(SPACY_MODEL_NAME)
+        pipeline = spacy.load(SPACY_MODEL_NAME)
+        pipeline.to_disk(SPACY_MODEL_PATH)
+
+    if all(
+        os.path.isfile(os.path.join(TFM_MODEL_PATH, file))
+        for file in ["config.json", "pytorch_model.bin"]
+    ):
+        tokenizer = AutoTokenizer.from_pretrained(TFM_MODEL_PATH, local_files_only=True)
+        model = AutoModelForSequenceClassification.from_pretrained(
+            TFM_MODEL_PATH, local_files_only=True
+        )
+    else:
+        os.makedirs(TFM_MODEL_PATH, exist_ok=True)
+        tokenizer = AutoTokenizer.from_pretrained(
+            TFM_MODEL_NAME, cache_dir=TFM_MODEL_PATH
+        )
+        model = AutoModelForSequenceClassification.from_pretrained(
+            TFM_MODEL_NAME, cache_dir=TFM_MODEL_PATH
+        )
 
 
 def segmentation(text, threshold=0.85):
     """
     This function takes the raw text, converts them into sentence tokens.
     Tokens are then provided to the sequence classifier to predict the
     syntactical similarity.
@@ -82,11 +120,11 @@
         )
     else:
         raise HTTPException(status_code=500, detail="Invalid model name.")
     return f"[Model Loaded] : {model_name}"
 
 
 if __name__ == "__main__":
-    from jaseci.actions.remote_actions import launch_server
+    from jaseci.jsorc.remote_actions import launch_server
 
     print("Text Segmentor up and running")
     launch_server(port=8000)
```

### Comparing `jac_nlp-1.4.0.9/jac_nlp/tfm_ner/entity_utils.py` & `jac_nlp-1.4.1.0/jac_nlp/tfm_ner/entity_utils.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.0.9/jac_nlp/tfm_ner/tests/test_tfm_ner.py` & `jac_nlp-1.4.1.0/jac_nlp/tfm_ner/tests/test_tfm_ner.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from jaseci.utils.test_core import CoreTest, jac_testcase
-from jaseci.actions.live_actions import load_module_actions, unload_module
+from jaseci.jsorc.live_actions import load_module_actions, unload_module
 import pytest
 import os
+import shutil
+from os import path
 
 
 class TfmNerTest(CoreTest):
     fixture_src = __file__
     """
     Test Class for Tfm_Ner Module to test the functionality of api's
     """
@@ -59,7 +61,10 @@
         self.assertEqual(ret["success"], True)
 
     @classmethod
     def tearDownClass(cls):
         super(TfmNerTest, cls).tearDownClass()
         ret = unload_module("jac_nlp.tfm_ner.tfm_ner")
         assert ret is True
+        for temp_path in ["results", "modeloutput", "train", "test"]:
+            if path.exists(temp_path) and path.isdir(temp_path):
+                shutil.rmtree(temp_path)
```

### Comparing `jac_nlp-1.4.0.9/jac_nlp/tfm_ner/tfm_ner.py` & `jac_nlp-1.4.1.0/jac_nlp/tfm_ner/tfm_ner.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,58 @@
 import traceback
 from fastapi import HTTPException
-from jaseci.actions.live_actions import jaseci_action
+from jaseci.jsorc.live_actions import jaseci_action
 from typing import Dict, List, Optional
 import os
 import json
 import warnings
 from .train import (
     predict_text,
     load_custom_model,
     save_custom_model,
     NERDataMaker,
     train_model,
 )
 import shutil
+from pathlib import Path
+from transformers import AutoTokenizer, AutoModelForSequenceClassification
+from jaseci.utils.utils import model_base_path
+
 
 warnings.filterwarnings("ignore")
 
 
-def config_setup():
+@jaseci_action(act_group=["tfm_ner"], allow_remote=True)
+def setup():
     """
     Loading configurations from config and
     initialize tokenizer and model
     """
-    global train_config, model_config, curr_model_path
+    global train_config, model_config, MODEL_BASE_PATH
     global t_config_fname, m_config_fname
     dirname = os.path.dirname(__file__)
     m_config_fname = os.path.join(dirname, "utils/model_config.json")
     t_config_fname = os.path.join(dirname, "utils/train_config.json")
 
     with open(t_config_fname, "r") as jsonfile:
         train_config = json.load(jsonfile)
     with open(m_config_fname, "r") as jsonfile:
         model_config = json.load(jsonfile)
+    MODEL_BASE_PATH = str(model_base_path("jac_nlp/tfm_ner"))
+    os.makedirs(MODEL_BASE_PATH, exist_ok=True)
+    if not os.listdir(MODEL_BASE_PATH):
+        model = AutoModelForSequenceClassification.from_pretrained(
+            model_config["model_name"]
+        )
+        tokenizer = AutoTokenizer.from_pretrained(model_config["model_name"])
+        tokenizer.save_vocabulary(MODEL_BASE_PATH)
+        model.save_pretrained(MODEL_BASE_PATH)
+        del model, tokenizer
+    load_custom_model(MODEL_BASE_PATH)
 
-    curr_model_path = model_config["model_name"]
-
-
-config_setup()
 
 enum = {"default": 1, "append": 2, "incremental": 3}
 
 
 @jaseci_action(act_group=["tfm_ner"], allow_remote=True)
 def extract_entity(text: str = None):
     try:
@@ -52,16 +64,16 @@
     except Exception as e:
         print(traceback.format_exc())
         raise HTTPException(status_code=500, detail=str(e))
 
 
 @jaseci_action(act_group=["tfm_ner"], allow_remote=True)
 def train(
-    mode: str = train_config["MODE"],
-    epochs: int = train_config["EPOCHS"],
+    mode: str = "default",
+    epochs: int = 20,
     train_data: List = [],
     val_data: Optional[List] = [],
 ):
     """
     API for training the model
     """
     if not os.path.exists("train/logs"):
@@ -90,53 +102,57 @@
             "Error": "Please define training mode",
             "Available mode": ["default", "append", "incremental"],
         }
         raise HTTPException(status_code=400, detail=st)
 
     try:
         train_dm = NERDataMaker(train_data)
-        load_custom_model(curr_model_path, train_dm)
+        load_custom_model(MODEL_BASE_PATH, train_dm)
         train_model(train_data=train_data, val_data=val_data, train_config=train_config)
         print("model training Completed")
         return {"status": "model Training Successful!"}
     except Exception as e:
         print(e)
         traceback.print_exc()
         raise HTTPException(
             status_code=500,
             detail=str("Issue encountered during train "),
         )
 
 
 @jaseci_action(act_group=["tfm_ner"], allow_remote=True)
 def load_model(model_path: str = "default", local_file: bool = True):
-    global curr_model_path
-    curr_model_path = model_path
+    global MODEL_BASE_PATH
+    if not os.path.isabs(model_path):
+        model_path = str(MODEL_BASE_PATH / Path(model_path))
+    MODEL_BASE_PATH = model_path
     train_file_path = os.path.join(model_path, "train.json")
     if local_file is True and not os.path.exists(model_path):
         return "Model path is not available"
     try:
         print("loading latest trained model to memory...")
         if os.path.exists(train_file_path):
             with open(train_file_path, "r") as fp:
                 train_data = json.load(fp)
             train_dm = NERDataMaker(train_data)
-            load_custom_model(curr_model_path, train_dm)
+            load_custom_model(MODEL_BASE_PATH, train_dm)
             print("model successfully load to memory!")
             return {"status": "model Loaded Successfull!"}
         else:
             raise HTTPException(status_code=400, detail=str("cannot load model"))
     except Exception as e:
         print(traceback.format_exc())
         raise HTTPException(status_code=400, detail=str(e))
 
 
 @jaseci_action(act_group=["tfm_ner"], allow_remote=True)
 def save_model(model_path: str = "mymodel"):
     try:
+        if not os.path.isabs(model_path):
+            model_path = str(MODEL_BASE_PATH / Path(model_path))
         save_custom_model(model_path)
         print(f"current model {model_path} saved to disk.")
         shutil.copy("train/train.json", model_path)
         return {"status": f"model {model_path} saved Successfull!"}
     except Exception as e:
         print(traceback.format_exc())
         raise HTTPException(status_code=400, detail=str(e))
@@ -184,18 +200,18 @@
     global model_config
     try:
         save_model(model_config["model_save_path"])
         model_config.update(model_parameters)
         with open(m_config_fname, "w+") as jsonfile:
             json.dump(model_config, jsonfile, indent=4)
 
-        config_setup()
+        setup()
         return "Config setup is complete."
     except Exception as e:
         print(traceback.format_exc())
         raise HTTPException(status_code=500, detail=str(e))
 
 
 if __name__ == "__main__":
-    from jaseci.actions.remote_actions import launch_server
+    from jaseci.jsorc.remote_actions import launch_server
 
     launch_server(port=8000)
```

### Comparing `jac_nlp-1.4.0.9/jac_nlp/tfm_ner/train.py` & `jac_nlp-1.4.1.0/jac_nlp/tfm_ner/train.py`

 * *Files 3% similar despite different names*

```diff
@@ -186,58 +186,68 @@
         tokenized_ds = ds.map(tokenize_and_align_labels, batched=True)
         return tokenized_ds
 
 
 def load_custom_model(model_path, train_dm=None):
     global model, tokenizer, data_collator
     tokenizer = AutoTokenizer.from_pretrained(model_path)
-    model = AutoModelForTokenClassification.from_pretrained(
-        model_path,
-        num_labels=len(train_dm.unique_entities),
-        id2label=train_dm.id2label,
-        label2id=train_dm.label2id,
-    )
+    if train_dm is None:
+        model = AutoModelForTokenClassification.from_pretrained(model_path)
+    else:
+        num_labels = len(train_dm.unique_entities)
+        id2label = train_dm.id2label
+        label2id = train_dm.label2id
+        model = AutoModelForTokenClassification.from_pretrained(
+            model_path,
+            num_labels=num_labels,
+            id2label=id2label,
+            label2id=label2id,
+            local_files_only=True,
+            ignore_mismatched_sizes=True,
+        )
     model.to(device)
     data_collator = DataCollatorForTokenClassification(tokenizer=tokenizer)
 
 
 def train_model(train_data, val_data, train_config):
     global val_dm
     if len(train_data) != 0:
         train_dm = NERDataMaker(train_data)
         train_ds = train_dm.as_hf_dataset(tokenizer=tokenizer)
         print(f"total Train examples = {len(train_data)}")
-    if len(val_data) != 0:
-        val_dm = NERDataMaker(val_data)
-        val_ds = val_dm.as_hf_dataset(tokenizer=tokenizer)
-        print(f"total validation examples = {len(val_dm)}")
-    else:
-        val_dm = train_dm
-        val_ds = train_ds
-    training_args = TrainingArguments(
-        output_dir="./results",
-        evaluation_strategy="epoch",
-        learning_rate=train_config["LEARNING_RATE"],
-        per_device_train_batch_size=train_config["TRAIN_BATCH_SIZE"],
-        per_device_eval_batch_size=train_config["VALID_BATCH_SIZE"],
-        num_train_epochs=train_config["EPOCHS"],
-        weight_decay=0.01,
-    )
-    trainer = Trainer(
-        model=model,
-        args=training_args,
-        train_dataset=train_ds,
-        eval_dataset=val_ds,
-        tokenizer=tokenizer,
-        data_collator=data_collator,
-        compute_metrics=compute_metrics,
-        callbacks=None,
-    )
+        if len(val_data) != 0:
+            val_dm = NERDataMaker(val_data)
+            val_ds = val_dm.as_hf_dataset(tokenizer=tokenizer)
+            print(f"total validation examples = {len(val_dm)}")
+        else:
+            val_dm = train_dm
+            val_ds = train_ds
+        training_args = TrainingArguments(
+            output_dir="./results",
+            evaluation_strategy="epoch",
+            learning_rate=train_config["LEARNING_RATE"],
+            per_device_train_batch_size=train_config["TRAIN_BATCH_SIZE"],
+            per_device_eval_batch_size=train_config["VALID_BATCH_SIZE"],
+            num_train_epochs=train_config["EPOCHS"],
+            weight_decay=0.01,
+        )
+        trainer = Trainer(
+            model=model,
+            args=training_args,
+            train_dataset=train_ds,
+            eval_dataset=val_ds,
+            tokenizer=tokenizer,
+            data_collator=data_collator,
+            compute_metrics=compute_metrics,
+            callbacks=None,
+        )
 
-    trainer.train()
+        trainer.train()
+    else:
+        print("Training data not available")
 
 
 def save_custom_model(model_path):
     # saving model
     model.save_pretrained(model_path)
     tokenizer.save_pretrained(model_path)
     print(str(datetime.now()) + "   ", f"model saved successful to : {model_path}")
```

### Comparing `jac_nlp-1.4.0.9/jac_nlp/tfm_ner/utils/data_tokens.py` & `jac_nlp-1.4.1.0/jac_nlp/tfm_ner/utils/data_tokens.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.0.9/jac_nlp/topic_ext/action_utils.py` & `jac_nlp-1.4.1.0/jac_nlp/topic_ext/action_utils.py`

 * *Files identical despite different names*

### Comparing `jac_nlp-1.4.0.9/jac_nlp/topic_ext/topic_ext.py` & `jac_nlp-1.4.1.0/jac_nlp/topic_ext/topic_ext.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import warnings
 
 import pandas as pd
 
-from jaseci.actions.live_actions import jaseci_action
-from jaseci.actions.remote_actions import launch_server
+from jaseci.jsorc.live_actions import jaseci_action
+from jaseci.jsorc.remote_actions import launch_server
 from fastapi import HTTPException
 
 from .action_utils import (
     c_tf_idf,
     extract_top_n_words_per_topic,
     generate_topic_label,
     mmr,
```

### Comparing `jac_nlp-1.4.0.9/jac_nlp/use_enc/tests/test_use_enc.py` & `jac_nlp-1.4.1.0/jac_nlp/use_enc/tests/test_use_enc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from jaseci.utils.test_core import CoreTest, jac_testcase
-from jaseci.actions.live_actions import load_module_actions, unload_module
+from jaseci.jsorc.live_actions import load_module_actions, unload_module
 
 
 class UseEncModule(CoreTest):
     fixture_src = __file__
 
     @classmethod
     def setUpClass(cls):
```

### Comparing `jac_nlp-1.4.0.9/jac_nlp/use_enc/use_enc.py` & `jac_nlp-1.4.1.0/jac_nlp/use_enc/use_enc.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,34 @@
 import numpy as np
 import tensorflow_hub as hub
 import tensorflow as tf
 import tensorflow_text  # noqa
-from jaseci.actions.live_actions import jaseci_action
+from jaseci.jsorc.live_actions import jaseci_action
 from typing import Union
+import os
+from jaseci.utils.utils import model_base_path
 
 
-module = hub.load("https://tfhub.dev/google/universal-sentence-encoder/4")
+MODULE_URL = "https://tfhub.dev/google/universal-sentence-encoder/4"
+MODEL_BASE_PATH = model_base_path("jac_nlp/use_enc")
+
+
+@jaseci_action(act_group=["use"], allow_remote=True)
+def setup():
+    """
+    Load Universal Sentence Encoder model
+    """
+    global module
+    try:
+        module = tf.saved_model.load(os.path.join(MODEL_BASE_PATH, "saved_model.pb"))
+    except OSError:
+        os.makedirs(MODEL_BASE_PATH, exist_ok=True)
+        module = hub.load(MODULE_URL)
+        tf.saved_model.save(module, MODEL_BASE_PATH)
+        tf.keras.backend.clear_session()
 
 
 @jaseci_action(act_group=["use"], aliases=["get_embedding"], allow_remote=True)
 def encode(text: Union[str, list]):
     if isinstance(text, str):
         text = [text]
     return module(text).numpy().tolist()
@@ -42,10 +60,10 @@
     ret["match"] = (
         classes[top_hit] if isinstance(classes[top_hit], str) else "[embedded value]"
     )
     return ret
 
 
 if __name__ == "__main__":
-    from jaseci.actions.remote_actions import launch_server
+    from jaseci.jsorc.remote_actions import launch_server
 
     launch_server(port=8000)
```

### Comparing `jac_nlp-1.4.0.9/jac_nlp/use_qa/tests/test_use_qa.py` & `jac_nlp-1.4.1.0/jac_nlp/use_qa/tests/test_use_qa.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from jaseci.utils.test_core import CoreTest, jac_testcase
-from jaseci.actions.live_actions import load_module_actions, unload_module
+from jaseci.jsorc.live_actions import load_module_actions, unload_module
 
 
 class UseQAModule(CoreTest):
     fixture_src = __file__
 
     @classmethod
     def setUpClass(cls):
```

### Comparing `jac_nlp-1.4.0.9/jac_nlp.egg-info/PKG-INFO` & `jac_nlp-1.4.1.0/jac_nlp.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 Metadata-Version: 2.1
 Name: jac-nlp
-Version: 1.4.0.9
+Version: 1.4.1.0
 Home-page: https://github.com/Jaseci-Labs/jaseci
 Author: Jason Mars
 Author-email: jason@jaseci.org
 Provides-Extra: all
 Provides-Extra: bart_sum
 Provides-Extra: cl_summer
 Provides-Extra: ent_ext
-Provides-Extra: fast_enc
 Provides-Extra: sbert_sim
 Provides-Extra: t5_sum
 Provides-Extra: text_seg
 Provides-Extra: tfm_ner
 Provides-Extra: use_enc
 Provides-Extra: use_qa
 Provides-Extra: zs_classifier
 Provides-Extra: bi_enc
 Provides-Extra: topic_ext
 Provides-Extra: gpt2
+Provides-Extra: bi_ner
+Provides-Extra: gpt3
+Provides-Extra: sentiment
+Provides-Extra: paraphraser
+Provides-Extra: dolly
```

### Comparing `jac_nlp-1.4.0.9/jac_nlp.egg-info/requires.txt` & `jac_nlp-1.4.1.0/jac_nlp.egg-info/requires.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-jaseci
+jaseci==1.4.1.0
 pytest<7.1,>=7.0.1
 pytest-order<1.1,>=1.0.1
 
 [all]
 transformers>=4.25.1
-beautifulsoup4<4.11.0,>=4.10.0
+beautifulsoup4<4.13.0,>=4.12.2
 torch<2.0.0,>=1.10.2
 sumy==0.11.0
 flair==0.11.3
-fasttext<0.10.0,>=0.9.2
 sentence-transformers<2.3,>=2.2.0
 torch==1.13.1
 transformers==4.25.1
 sentencepiece==0.1.95
 spacy==3.3.0
 datasets==2.8.0
 evaluate<0.3,>=0.2.2
@@ -21,41 +20,71 @@
 tensorflow-text<3.0.0,>=2.7.3
 tensorflow<3.0.0,>=2.8.0
 torch
 numpy>=1.23.0
 scikit-learn>=1.2.0
 pandas==1.5.2
 sentence-transformers==2.2.2
+scikit-learn>=0.24.2
+openai>=0.26.5
+emoji==0.6.0
+protobuf<3.21.0
+transformers<5.0.0,>=4.25.1
+numpy<2.0.0,>=1.23.5
+accelerate<0.19.0,>=0.18.0
+langchain<0.1.0,>=0.0.151
 
 [bart_sum]
 transformers>=4.25.1
-beautifulsoup4<4.11.0,>=4.10.0
+beautifulsoup4<4.13.0,>=4.12.2
 torch<2.0.0,>=1.10.2
 
 [bi_enc]
 transformers==4.25.1
 torch==1.13.1
 
+[bi_ner]
+transformers==4.25.1
+torch==1.13.1
+
 [cl_summer]
 sumy==0.11.0
 
+[dolly]
+transformers<5.0.0,>=4.25.1
+numpy<2.0.0,>=1.23.5
+torch<2.0.0,>=1.10.2
+accelerate<0.19.0,>=0.18.0
+langchain<0.1.0,>=0.0.151
+
 [ent_ext]
 flair==0.11.3
 
-[fast_enc]
-fasttext<0.10.0,>=0.9.2
-
 [gpt2]
 transformers>=4.25.1
 torch<2.0.0,>=1.10.2
+scikit-learn>=0.24.2
+
+[gpt3]
+openai>=0.26.5
+
+[paraphraser]
+transformers>=4.25.1
+sentencepiece==0.1.95
+torch==1.13.1
+protobuf<3.21.0
 
 [sbert_sim]
 sentence-transformers<2.3,>=2.2.0
 torch==1.13.1
 
+[sentiment]
+transformers==4.25.1
+emoji==0.6.0
+
 [t5_sum]
 transformers==4.25.1
 torch==1.13.1
 sentencepiece==0.1.95
 
 [text_seg]
 spacy==3.3.0
```

### Comparing `jac_nlp-1.4.0.9/setup.py` & `jac_nlp-1.4.1.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 from setuptools import setup, find_packages
 from os.path import join
 
 MODULES = [
     "bart_sum",
     "cl_summer",
     "ent_ext",
-    "fast_enc",
+    # "fast_enc",
     "sbert_sim",
     "t5_sum",
     "text_seg",
     "tfm_ner",
     "use_enc",
     "use_qa",
     "zs_classifier",
     "bi_enc",
     "topic_ext",
     "gpt2",
+    "bi_ner",
+    "gpt3",
+    "sentiment",
+    "paraphraser",
+    "dolly",
 ]
 
 
 def get_ver():
     with open(join("./jac_nlp", "VERSION")) as version_file:
         return version_file.read().strip()
 
@@ -33,16 +38,20 @@
     return extras_requires
 
 
 setup(
     name="jac_nlp",
     version=get_ver(),
     packages=find_packages(include=["jac_nlp", "jac_nlp.*"]),
-    install_requires=["jaseci", "pytest>=7.0.1,<7.1", "pytest-order>=1.0.1,<1.1"],
+    install_requires=[
+        f"jaseci=={get_ver()}",
+        "pytest>=7.0.1,<7.1",
+        "pytest-order>=1.0.1,<1.1",
+    ],
     extras_require=get_extras_requires(),
     package_data={
-        "": ["*.json", "*.cfg", "VERSION", "*.yaml", "requirements.txt"],
+        "": ["*.json", "*.cfg", "VERSION", "*.yaml", "requirements.txt", "*.jac"],
     },
     author="Jason Mars",
     author_email="jason@jaseci.org",
     url="https://github.com/Jaseci-Labs/jaseci",
 )
```

