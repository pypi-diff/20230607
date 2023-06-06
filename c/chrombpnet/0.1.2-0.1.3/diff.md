# Comparing `tmp/chrombpnet-0.1.2.tar.gz` & `tmp/chrombpnet-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chrombpnet-0.1.2.tar", last modified: Fri Mar 24 22:45:11 2023, max compression
+gzip compressed data, was "chrombpnet-0.1.3.tar", last modified: Tue Jun  6 23:33:55 2023, max compression
```

## Comparing `chrombpnet-0.1.2.tar` & `chrombpnet-0.1.3.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-03-24 22:45:11.623572 chrombpnet-0.1.2/
--rwxrwxr-x   0 anusri    (1005) anusri    (1006)     1068 2022-12-15 07:53:05.000000 chrombpnet-0.1.2/LICENSE
--rwxrwxr-x   0 anusri    (1005) anusri    (1006)       87 2023-01-28 21:08:16.000000 chrombpnet-0.1.2/MANIFEST.in
--rw-rw-r--   0 anusri    (1005) anusri    (1006)      270 2023-03-24 22:45:11.623572 chrombpnet-0.1.2/PKG-INFO
--rw-rw-r--   0 anusri    (1005) anusri    (1006)    13980 2023-03-24 21:17:48.000000 chrombpnet-0.1.2/README.md
-drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-03-24 22:45:11.615571 chrombpnet-0.1.2/chrombpnet/
--rw-rw-r--   0 anusri    (1005) anusri    (1006)     7165 2023-03-24 21:17:48.000000 chrombpnet-0.1.2/chrombpnet/CHROMBPNET.py
--rw-rw-r--   0 anusri    (1005) anusri    (1006)        0 2023-01-28 21:08:16.000000 chrombpnet-0.1.2/chrombpnet/__init__.py
-drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-03-24 22:45:11.615571 chrombpnet-0.1.2/chrombpnet/data/
--rw-rw-r--   0 anusri    (1005) anusri    (1006)     3525 2023-01-28 21:08:16.000000 chrombpnet-0.1.2/chrombpnet/data/ATAC.ref.motifs.txt
--rw-rw-r--   0 anusri    (1005) anusri    (1006)     7013 2023-01-28 21:08:16.000000 chrombpnet-0.1.2/chrombpnet/data/DNASE.ref.motifs.txt
--rw-rw-r--   0 anusri    (1005) anusri    (1006)      702 2023-01-28 21:08:16.000000 chrombpnet-0.1.2/chrombpnet/data/__init__.py
--rw-rw-r--   0 anusri    (1005) anusri    (1006)      139 2023-01-28 21:08:16.000000 chrombpnet-0.1.2/chrombpnet/data/motif_to_pwm.ATAC.tsv
--rw-rw-r--   0 anusri    (1005) anusri    (1006)       44 2023-01-28 21:08:16.000000 chrombpnet-0.1.2/chrombpnet/data/motif_to_pwm.DNASE.tsv
--rw-rw-r--   0 anusri    (1005) anusri    (1006)      342 2023-01-28 21:08:16.000000 chrombpnet-0.1.2/chrombpnet/data/motif_to_pwm.TF.tsv
--rw-rw-r--   0 anusri    (1005) anusri    (1006)  1108122 2023-01-28 21:08:16.000000 chrombpnet-0.1.2/chrombpnet/data/motifs.meme.txt
-drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-03-24 22:45:11.615571 chrombpnet-0.1.2/chrombpnet/evaluation/
--rw-rw-r--   0 anusri    (1005) anusri    (1006)        0 2022-12-15 07:53:05.000000 chrombpnet-0.1.2/chrombpnet/evaluation/__init__.py
-drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-03-24 22:45:11.615571 chrombpnet-0.1.2/chrombpnet/evaluation/interpret/
--rw-rw-r--   0 anusri    (1005) anusri    (1006)        0 2022-12-15 07:53:05.000000 chrombpnet-0.1.2/chrombpnet/evaluation/interpret/__init__.py
--rw-rw-r--   0 anusri    (1005) anusri    (1006)     1101 2022-12-15 07:53:05.000000 chrombpnet-0.1.2/chrombpnet/evaluation/interpret/input_utils.py
--rw-rw-r--   0 anusri    (1005) anusri    (1006)     5578 2023-03-24 22:02:17.000000 chrombpnet-0.1.2/chrombpnet/evaluation/interpret/interpret.py
--rw-rw-r--   0 anusri    (1005) anusri    (1006)     3845 2022-12-15 07:53:05.000000 chrombpnet-0.1.2/chrombpnet/evaluation/interpret/shap_utils.py
-drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-03-24 22:45:11.615571 chrombpnet-0.1.2/chrombpnet/evaluation/invivo_footprints/
--rw-rw-r--   0 anusri    (1005) anusri    (1006)        0 2022-12-15 07:53:05.000000 chrombpnet-0.1.2/chrombpnet/evaluation/invivo_footprints/__init__.py
--rw-rw-r--   0 anusri    (1005) anusri    (1006)     9973 2022-12-15 07:53:05.000000 chrombpnet-0.1.2/chrombpnet/evaluation/invivo_footprints/run_tfmodisco.py
--rw-rw-r--   0 anusri    (1005) anusri    (1006)    13499 2022-12-15 07:53:05.000000 chrombpnet-0.1.2/chrombpnet/evaluation/invivo_footprints/tf_modiscohits.py
-drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-03-24 22:45:11.619572 chrombpnet-0.1.2/chrombpnet/evaluation/make_bigwigs/
--rw-rw-r--   0 anusri    (1005) anusri    (1006)        0 2022-12-15 07:53:05.000000 chrombpnet-0.1.2/chrombpnet/evaluation/make_bigwigs/__init__.py
--rw-rw-r--   0 anusri    (1005) anusri    (1006)     3553 2023-01-28 21:08:16.000000 chrombpnet-0.1.2/chrombpnet/evaluation/make_bigwigs/bigwig_helper.py
--rw-rw-r--   0 anusri    (1005) anusri    (1006)     2384 2023-01-28 21:08:16.000000 chrombpnet-0.1.2/chrombpnet/evaluation/make_bigwigs/importance_hdf5_to_bigwig.py
--rw-rw-r--   0 anusri    (1005) anusri    (1006)    11378 2023-01-28 21:08:16.000000 chrombpnet-0.1.2/chrombpnet/evaluation/make_bigwigs/predict_to_bigwig.py
-drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-03-24 22:45:11.619572 chrombpnet-0.1.2/chrombpnet/evaluation/marginal_footprints/
--rw-rw-r--   0 anusri    (1005) anusri    (1006)        0 2022-12-15 07:53:05.000000 chrombpnet-0.1.2/chrombpnet/evaluation/marginal_footprints/__init__.py
--rw-rw-r--   0 anusri    (1005) anusri    (1006)     6997 2023-03-24 21:17:48.000000 chrombpnet-0.1.2/chrombpnet/evaluation/marginal_footprints/marginal_footprinting.py
-drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-03-24 22:45:11.619572 chrombpnet-0.1.2/chrombpnet/evaluation/modisco/
--rw-rw-r--   0 anusri    (1005) anusri    (1006)        0 2022-12-15 07:53:05.000000 chrombpnet-0.1.2/chrombpnet/evaluation/modisco/__init__.py
--rw-rw-r--   0 anusri    (1005) anusri    (1006)      610 2023-01-28 21:08:16.000000 chrombpnet-0.1.2/chrombpnet/evaluation/modisco/convert_html_to_pdf.py
--rw-rw-r--   0 anusri    (1005) anusri    (1006)     6274 2022-12-15 07:53:05.000000 chrombpnet-0.1.2/chrombpnet/evaluation/modisco/fetch_tomtom.py
--rw-rw-r--   0 anusri    (1005) anusri    (1006)     6349 2022-12-15 07:53:05.000000 chrombpnet-0.1.2/chrombpnet/evaluation/modisco/run_modisco.py
--rw-rw-r--   0 anusri    (1005) anusri    (1006)     8232 2022-12-15 07:53:05.000000 chrombpnet-0.1.2/chrombpnet/evaluation/modisco/visualize_motif_matches.py
-drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-03-24 22:45:11.619572 chrombpnet-0.1.2/chrombpnet/evaluation/variant_effect_prediction/
--rw-rw-r--   0 anusri    (1005) anusri    (1006)        0 2022-12-15 07:53:05.000000 chrombpnet-0.1.2/chrombpnet/evaluation/variant_effect_prediction/__init__.py
--rw-rw-r--   0 anusri    (1005) anusri    (1006)     2748 2022-12-15 07:53:05.000000 chrombpnet-0.1.2/chrombpnet/evaluation/variant_effect_prediction/snp_generator.py
--rw-rw-r--   0 anusri    (1005) anusri    (1006)     8338 2023-01-28 21:08:16.000000 chrombpnet-0.1.2/chrombpnet/evaluation/variant_effect_prediction/snp_scoring.py
--rw-rw-r--   0 anusri    (1005) anusri    (1006)      699 2022-12-15 07:53:05.000000 chrombpnet-0.1.2/chrombpnet/evaluation/variant_effect_prediction/testing.py
-drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-03-24 22:45:11.619572 chrombpnet-0.1.2/chrombpnet/helpers/
--rw-rw-r--   0 anusri    (1005) anusri    (1006)        0 2022-12-15 07:53:05.000000 chrombpnet-0.1.2/chrombpnet/helpers/__init__.py
-drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-03-24 22:45:11.619572 chrombpnet-0.1.2/chrombpnet/helpers/generate_reports/
--rw-rw-r--   0 anusri    (1005) anusri    (1006)        0 2023-01-28 21:08:16.000000 chrombpnet-0.1.2/chrombpnet/helpers/generate_reports/__init__.py
--rw-rw-r--   0 anusri    (1005) anusri    (1006)    18002 2023-03-24 21:17:48.000000 chrombpnet-0.1.2/chrombpnet/helpers/generate_reports/make_html.py
--rw-rw-r--   0 anusri    (1005) anusri    (1006)    14314 2023-01-28 21:08:16.000000 chrombpnet-0.1.2/chrombpnet/helpers/generate_reports/make_html_bias.py
-drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-03-24 22:45:11.619572 chrombpnet-0.1.2/chrombpnet/helpers/hyperparameters/
--rw-rw-r--   0 anusri    (1005) anusri    (1006)        0 2022-12-15 07:53:05.000000 chrombpnet-0.1.2/chrombpnet/helpers/hyperparameters/__init__.py
--rw-rw-r--   0 anusri    (1005) anusri    (1006)     8205 2023-03-24 21:17:48.000000 chrombpnet-0.1.2/chrombpnet/helpers/hyperparameters/find_bias_hyperparams.py
--rw-rw-r--   0 anusri    (1005) anusri    (1006)    10566 2023-03-24 21:17:48.000000 chrombpnet-0.1.2/chrombpnet/helpers/hyperparameters/find_chrombpnet_hyperparams.py
--rw-rw-r--   0 anusri    (1005) anusri    (1006)     2587 2022-12-15 07:53:05.000000 chrombpnet-0.1.2/chrombpnet/helpers/hyperparameters/param_utils.py
-drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-03-24 22:45:11.619572 chrombpnet-0.1.2/chrombpnet/helpers/make_chr_splits/
--rw-rw-r--   0 anusri    (1005) anusri    (1006)        0 2022-12-15 07:53:05.000000 chrombpnet-0.1.2/chrombpnet/helpers/make_chr_splits/__init__.py
--rw-rw-r--   0 anusri    (1005) anusri    (1006)     1591 2023-01-28 21:08:16.000000 chrombpnet-0.1.2/chrombpnet/helpers/make_chr_splits/splits.py
-drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-03-24 22:45:11.619572 chrombpnet-0.1.2/chrombpnet/helpers/make_gc_matched_negatives/
--rw-rw-r--   0 anusri    (1005) anusri    (1006)        0 2022-12-15 07:53:05.000000 chrombpnet-0.1.2/chrombpnet/helpers/make_gc_matched_negatives/__init__.py
--rwxrwxr-x   0 anusri    (1005) anusri    (1006)     2464 2023-01-28 21:08:16.000000 chrombpnet-0.1.2/chrombpnet/helpers/make_gc_matched_negatives/get_gc_content.py
--rwxrwxr-x   0 anusri    (1005) anusri    (1006)     7035 2023-01-28 21:08:16.000000 chrombpnet-0.1.2/chrombpnet/helpers/make_gc_matched_negatives/get_gc_matched_negatives.py
-drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-03-24 22:45:11.619572 chrombpnet-0.1.2/chrombpnet/helpers/make_gc_matched_negatives/get_genomewide_gc_buckets/
--rw-rw-r--   0 anusri    (1005) anusri    (1006)        0 2022-12-15 07:53:05.000000 chrombpnet-0.1.2/chrombpnet/helpers/make_gc_matched_negatives/get_genomewide_gc_buckets/__init__.py
--rw-rw-r--   0 anusri    (1005) anusri    (1006)     2928 2023-01-28 21:08:16.000000 chrombpnet-0.1.2/chrombpnet/helpers/make_gc_matched_negatives/get_genomewide_gc_buckets/get_genomewide_gc_bins.py
-drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-03-24 22:45:11.619572 chrombpnet-0.1.2/chrombpnet/helpers/preprocessing/
--rw-rw-r--   0 anusri    (1005) anusri    (1006)        0 2022-12-15 07:53:05.000000 chrombpnet-0.1.2/chrombpnet/helpers/preprocessing/__init__.py
-drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-03-24 22:45:11.623572 chrombpnet-0.1.2/chrombpnet/helpers/preprocessing/analysis/
--rw-rw-r--   0 anusri    (1005) anusri    (1006)        0 2022-12-15 07:53:05.000000 chrombpnet-0.1.2/chrombpnet/helpers/preprocessing/analysis/__init__.py
--rw-rw-r--   0 anusri    (1005) anusri    (1006)     2950 2023-01-28 21:08:16.000000 chrombpnet-0.1.2/chrombpnet/helpers/preprocessing/analysis/build_pwm_from_bigwig.py
--rw-rw-r--   0 anusri    (1005) anusri    (1006)    11082 2023-03-24 21:18:52.000000 chrombpnet-0.1.2/chrombpnet/helpers/preprocessing/auto_shift_detect.py
--rw-rw-r--   0 anusri    (1005) anusri    (1006)     5103 2023-03-24 21:18:52.000000 chrombpnet-0.1.2/chrombpnet/helpers/preprocessing/reads_to_bigwig.py
--rw-rw-r--   0 anusri    (1005) anusri    (1006)    27194 2023-01-28 21:08:16.000000 chrombpnet-0.1.2/chrombpnet/parsers.py
--rw-rw-r--   0 anusri    (1005) anusri    (1006)    24932 2023-01-28 21:08:16.000000 chrombpnet-0.1.2/chrombpnet/pipelines.py
-drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-03-24 22:45:11.623572 chrombpnet-0.1.2/chrombpnet/training/
--rw-rw-r--   0 anusri    (1005) anusri    (1006)        0 2022-12-15 07:53:05.000000 chrombpnet-0.1.2/chrombpnet/training/__init__.py
-drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-03-24 22:45:11.623572 chrombpnet-0.1.2/chrombpnet/training/data_generators/
--rw-rw-r--   0 anusri    (1005) anusri    (1006)        0 2022-12-15 07:53:05.000000 chrombpnet-0.1.2/chrombpnet/training/data_generators/__init__.py
--rw-rw-r--   0 anusri    (1005) anusri    (1006)     5518 2022-12-15 07:53:05.000000 chrombpnet-0.1.2/chrombpnet/training/data_generators/batchgen_generator.py
--rw-rw-r--   0 anusri    (1005) anusri    (1006)     4418 2022-12-15 07:53:05.000000 chrombpnet-0.1.2/chrombpnet/training/data_generators/initializers.py
--rw-rw-r--   0 anusri    (1005) anusri    (1006)     4755 2023-01-28 21:08:16.000000 chrombpnet-0.1.2/chrombpnet/training/metrics.py
-drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-03-24 22:45:11.623572 chrombpnet-0.1.2/chrombpnet/training/models/
--rw-rw-r--   0 anusri    (1005) anusri    (1006)        0 2022-12-15 07:53:05.000000 chrombpnet-0.1.2/chrombpnet/training/models/__init__.py
--rw-rw-r--   0 anusri    (1005) anusri    (1006)     4048 2022-12-15 07:53:05.000000 chrombpnet-0.1.2/chrombpnet/training/models/bpnet_model.py
--rw-rw-r--   0 anusri    (1005) anusri    (1006)     6167 2023-01-28 21:08:16.000000 chrombpnet-0.1.2/chrombpnet/training/models/chrombpnet_with_bias_model.py
--rw-rw-r--   0 anusri    (1005) anusri    (1006)     7727 2023-01-28 21:08:16.000000 chrombpnet-0.1.2/chrombpnet/training/predict.py
--rw-rw-r--   0 anusri    (1005) anusri    (1006)     4817 2023-01-28 21:08:16.000000 chrombpnet-0.1.2/chrombpnet/training/train.py
-drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-03-24 22:45:11.623572 chrombpnet-0.1.2/chrombpnet/training/utils/
--rw-rw-r--   0 anusri    (1005) anusri    (1006)        0 2022-12-15 07:53:05.000000 chrombpnet-0.1.2/chrombpnet/training/utils/__init__.py
--rw-rw-r--   0 anusri    (1005) anusri    (1006)     3781 2023-01-28 21:08:16.000000 chrombpnet-0.1.2/chrombpnet/training/utils/argmanager.py
--rw-rw-r--   0 anusri    (1005) anusri    (1006)     3060 2022-12-15 07:53:05.000000 chrombpnet-0.1.2/chrombpnet/training/utils/augment.py
--rw-rw-r--   0 anusri    (1005) anusri    (1006)     1538 2022-12-15 07:53:05.000000 chrombpnet-0.1.2/chrombpnet/training/utils/callbacks.py
--rw-rw-r--   0 anusri    (1005) anusri    (1006)     3553 2022-12-15 07:53:05.000000 chrombpnet-0.1.2/chrombpnet/training/utils/data_utils.py
--rw-rw-r--   0 anusri    (1005) anusri    (1006)      687 2022-12-15 07:53:05.000000 chrombpnet-0.1.2/chrombpnet/training/utils/losses.py
--rw-rw-r--   0 anusri    (1005) anusri    (1006)     6434 2023-01-28 21:08:16.000000 chrombpnet-0.1.2/chrombpnet/training/utils/metrics_utils.py
--rw-rw-r--   0 anusri    (1005) anusri    (1006)     2565 2022-12-15 07:53:05.000000 chrombpnet-0.1.2/chrombpnet/training/utils/one_hot.py
-drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-03-24 22:45:11.615571 chrombpnet-0.1.2/chrombpnet.egg-info/
--rw-rw-r--   0 anusri    (1005) anusri    (1006)      270 2023-03-24 22:45:11.000000 chrombpnet-0.1.2/chrombpnet.egg-info/PKG-INFO
--rw-rw-r--   0 anusri    (1005) anusri    (1006)     3868 2023-03-24 22:45:11.000000 chrombpnet-0.1.2/chrombpnet.egg-info/SOURCES.txt
--rw-rw-r--   0 anusri    (1005) anusri    (1006)        1 2023-03-24 22:45:11.000000 chrombpnet-0.1.2/chrombpnet.egg-info/dependency_links.txt
--rw-rw-r--   0 anusri    (1005) anusri    (1006)      129 2023-03-24 22:45:11.000000 chrombpnet-0.1.2/chrombpnet.egg-info/entry_points.txt
--rw-rw-r--   0 anusri    (1005) anusri    (1006)        1 2023-03-24 22:45:11.000000 chrombpnet-0.1.2/chrombpnet.egg-info/not-zip-safe
--rw-rw-r--   0 anusri    (1005) anusri    (1006)      347 2023-03-24 22:45:11.000000 chrombpnet-0.1.2/chrombpnet.egg-info/requires.txt
--rw-rw-r--   0 anusri    (1005) anusri    (1006)       11 2023-03-24 22:45:11.000000 chrombpnet-0.1.2/chrombpnet.egg-info/top_level.txt
--rw-rw-r--   0 anusri    (1005) anusri    (1006)      413 2023-03-24 22:40:34.000000 chrombpnet-0.1.2/requirements.txt
--rw-rw-r--   0 anusri    (1005) anusri    (1006)       38 2023-03-24 22:45:11.623572 chrombpnet-0.1.2/setup.cfg
--rwxrwxr-x   0 anusri    (1005) anusri    (1006)     1038 2023-03-24 22:43:32.000000 chrombpnet-0.1.2/setup.py
-drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-03-24 22:45:11.623572 chrombpnet-0.1.2/tests/
--rwxrwxr-x   0 anusri    (1005) anusri    (1006)     3028 2023-01-28 21:08:16.000000 chrombpnet-0.1.2/tests/full_workflow.sh
--rwxrwxr-x   0 anusri    (1005) anusri    (1006)     1496 2022-12-15 07:53:05.000000 chrombpnet-0.1.2/tests/genomewide_gc_bin_test.sh
--rwxrwxr-x   0 anusri    (1005) anusri    (1006)      349 2022-12-15 07:53:05.000000 chrombpnet-0.1.2/tests/test_pred_to_bigwig.sh
-drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-03-24 22:45:11.623572 chrombpnet-0.1.2/workflows/
--rw-rw-r--   0 anusri    (1005) anusri    (1006)    12178 2023-01-28 21:08:16.000000 chrombpnet-0.1.2/workflows/train_bias_model.sh
--rw-rw-r--   0 anusri    (1005) anusri    (1006)    17611 2023-01-28 21:08:16.000000 chrombpnet-0.1.2/workflows/train_chrombpnet_model.sh
+drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-06-06 23:33:55.135674 chrombpnet-0.1.3/
+-rwxrwxr-x   0 anusri    (1005) anusri    (1006)     1068 2022-12-15 07:53:05.000000 chrombpnet-0.1.3/LICENSE
+-rwxrwxr-x   0 anusri    (1005) anusri    (1006)       87 2023-01-28 21:08:16.000000 chrombpnet-0.1.3/MANIFEST.in
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)      270 2023-06-06 23:33:55.131674 chrombpnet-0.1.3/PKG-INFO
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)    14038 2023-06-06 23:16:27.000000 chrombpnet-0.1.3/README.md
+drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-06-06 23:33:55.083670 chrombpnet-0.1.3/chrombpnet/
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)     7177 2023-04-17 01:25:44.000000 chrombpnet-0.1.3/chrombpnet/CHROMBPNET.py
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)        0 2023-01-28 21:08:16.000000 chrombpnet-0.1.3/chrombpnet/__init__.py
+drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-06-06 23:33:55.087671 chrombpnet-0.1.3/chrombpnet/data/
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)     3525 2023-01-28 21:08:16.000000 chrombpnet-0.1.3/chrombpnet/data/ATAC.ref.motifs.txt
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)     7013 2023-01-28 21:08:16.000000 chrombpnet-0.1.3/chrombpnet/data/DNASE.ref.motifs.txt
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)      702 2023-01-28 21:08:16.000000 chrombpnet-0.1.3/chrombpnet/data/__init__.py
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)      139 2023-01-28 21:08:16.000000 chrombpnet-0.1.3/chrombpnet/data/motif_to_pwm.ATAC.tsv
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)       44 2023-01-28 21:08:16.000000 chrombpnet-0.1.3/chrombpnet/data/motif_to_pwm.DNASE.tsv
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)      342 2023-01-28 21:08:16.000000 chrombpnet-0.1.3/chrombpnet/data/motif_to_pwm.TF.tsv
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)  1108122 2023-01-28 21:08:16.000000 chrombpnet-0.1.3/chrombpnet/data/motifs.meme.txt
+drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-06-06 23:33:55.095671 chrombpnet-0.1.3/chrombpnet/evaluation/
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)        0 2022-12-15 07:53:05.000000 chrombpnet-0.1.3/chrombpnet/evaluation/__init__.py
+drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-06-06 23:33:55.099671 chrombpnet-0.1.3/chrombpnet/evaluation/interpret/
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)        0 2022-12-15 07:53:05.000000 chrombpnet-0.1.3/chrombpnet/evaluation/interpret/__init__.py
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)     1115 2023-04-11 00:43:00.000000 chrombpnet-0.1.3/chrombpnet/evaluation/interpret/input_utils.py
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)     5578 2023-03-24 22:02:17.000000 chrombpnet-0.1.3/chrombpnet/evaluation/interpret/interpret.py
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)     3845 2022-12-15 07:53:05.000000 chrombpnet-0.1.3/chrombpnet/evaluation/interpret/shap_utils.py
+drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-06-06 23:33:55.099671 chrombpnet-0.1.3/chrombpnet/evaluation/invivo_footprints/
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)        0 2022-12-15 07:53:05.000000 chrombpnet-0.1.3/chrombpnet/evaluation/invivo_footprints/__init__.py
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)     9973 2022-12-15 07:53:05.000000 chrombpnet-0.1.3/chrombpnet/evaluation/invivo_footprints/run_tfmodisco.py
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)    13499 2022-12-15 07:53:05.000000 chrombpnet-0.1.3/chrombpnet/evaluation/invivo_footprints/tf_modiscohits.py
+drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-06-06 23:33:55.103672 chrombpnet-0.1.3/chrombpnet/evaluation/make_bigwigs/
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)        0 2022-12-15 07:53:05.000000 chrombpnet-0.1.3/chrombpnet/evaluation/make_bigwigs/__init__.py
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)     3553 2023-01-28 21:08:16.000000 chrombpnet-0.1.3/chrombpnet/evaluation/make_bigwigs/bigwig_helper.py
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)     2384 2023-01-28 21:08:16.000000 chrombpnet-0.1.3/chrombpnet/evaluation/make_bigwigs/importance_hdf5_to_bigwig.py
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)    11393 2023-04-11 00:48:48.000000 chrombpnet-0.1.3/chrombpnet/evaluation/make_bigwigs/predict_to_bigwig.py
+drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-06-06 23:33:55.103672 chrombpnet-0.1.3/chrombpnet/evaluation/marginal_footprints/
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)        0 2022-12-15 07:53:05.000000 chrombpnet-0.1.3/chrombpnet/evaluation/marginal_footprints/__init__.py
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)     7014 2023-06-06 23:16:27.000000 chrombpnet-0.1.3/chrombpnet/evaluation/marginal_footprints/marginal_footprinting.py
+drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-06-06 23:33:55.107672 chrombpnet-0.1.3/chrombpnet/evaluation/modisco/
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)        0 2022-12-15 07:53:05.000000 chrombpnet-0.1.3/chrombpnet/evaluation/modisco/__init__.py
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)      610 2023-01-28 21:08:16.000000 chrombpnet-0.1.3/chrombpnet/evaluation/modisco/convert_html_to_pdf.py
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)     6274 2022-12-15 07:53:05.000000 chrombpnet-0.1.3/chrombpnet/evaluation/modisco/fetch_tomtom.py
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)     6349 2022-12-15 07:53:05.000000 chrombpnet-0.1.3/chrombpnet/evaluation/modisco/run_modisco.py
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)     8232 2022-12-15 07:53:05.000000 chrombpnet-0.1.3/chrombpnet/evaluation/modisco/visualize_motif_matches.py
+drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-06-06 23:33:55.111672 chrombpnet-0.1.3/chrombpnet/evaluation/variant_effect_prediction/
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)        0 2022-12-15 07:53:05.000000 chrombpnet-0.1.3/chrombpnet/evaluation/variant_effect_prediction/__init__.py
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)     2748 2022-12-15 07:53:05.000000 chrombpnet-0.1.3/chrombpnet/evaluation/variant_effect_prediction/snp_generator.py
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)     8353 2023-04-11 00:52:07.000000 chrombpnet-0.1.3/chrombpnet/evaluation/variant_effect_prediction/snp_scoring.py
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)      699 2022-12-15 07:53:05.000000 chrombpnet-0.1.3/chrombpnet/evaluation/variant_effect_prediction/testing.py
+drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-06-06 23:33:55.111672 chrombpnet-0.1.3/chrombpnet/helpers/
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)        0 2022-12-15 07:53:05.000000 chrombpnet-0.1.3/chrombpnet/helpers/__init__.py
+drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-06-06 23:33:55.111672 chrombpnet-0.1.3/chrombpnet/helpers/generate_reports/
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)        0 2023-01-28 21:08:16.000000 chrombpnet-0.1.3/chrombpnet/helpers/generate_reports/__init__.py
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)    18003 2023-06-06 23:16:27.000000 chrombpnet-0.1.3/chrombpnet/helpers/generate_reports/make_html.py
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)    14314 2023-01-28 21:08:16.000000 chrombpnet-0.1.3/chrombpnet/helpers/generate_reports/make_html_bias.py
+drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-06-06 23:33:55.115673 chrombpnet-0.1.3/chrombpnet/helpers/hyperparameters/
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)        0 2022-12-15 07:53:05.000000 chrombpnet-0.1.3/chrombpnet/helpers/hyperparameters/__init__.py
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)     8205 2023-03-24 21:17:48.000000 chrombpnet-0.1.3/chrombpnet/helpers/hyperparameters/find_bias_hyperparams.py
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)    10566 2023-03-24 21:17:48.000000 chrombpnet-0.1.3/chrombpnet/helpers/hyperparameters/find_chrombpnet_hyperparams.py
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)     2587 2022-12-15 07:53:05.000000 chrombpnet-0.1.3/chrombpnet/helpers/hyperparameters/param_utils.py
+drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-06-06 23:33:55.115673 chrombpnet-0.1.3/chrombpnet/helpers/make_chr_splits/
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)        0 2022-12-15 07:53:05.000000 chrombpnet-0.1.3/chrombpnet/helpers/make_chr_splits/__init__.py
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)     1591 2023-01-28 21:08:16.000000 chrombpnet-0.1.3/chrombpnet/helpers/make_chr_splits/splits.py
+drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-06-06 23:33:55.115673 chrombpnet-0.1.3/chrombpnet/helpers/make_gc_matched_negatives/
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)        0 2022-12-15 07:53:05.000000 chrombpnet-0.1.3/chrombpnet/helpers/make_gc_matched_negatives/__init__.py
+-rwxrwxr-x   0 anusri    (1005) anusri    (1006)     2464 2023-01-28 21:08:16.000000 chrombpnet-0.1.3/chrombpnet/helpers/make_gc_matched_negatives/get_gc_content.py
+-rwxrwxr-x   0 anusri    (1005) anusri    (1006)     7035 2023-01-28 21:08:16.000000 chrombpnet-0.1.3/chrombpnet/helpers/make_gc_matched_negatives/get_gc_matched_negatives.py
+drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-06-06 23:33:55.115673 chrombpnet-0.1.3/chrombpnet/helpers/make_gc_matched_negatives/get_genomewide_gc_buckets/
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)        0 2022-12-15 07:53:05.000000 chrombpnet-0.1.3/chrombpnet/helpers/make_gc_matched_negatives/get_genomewide_gc_buckets/__init__.py
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)     2928 2023-01-28 21:08:16.000000 chrombpnet-0.1.3/chrombpnet/helpers/make_gc_matched_negatives/get_genomewide_gc_buckets/get_genomewide_gc_bins.py
+drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-06-06 23:33:55.119673 chrombpnet-0.1.3/chrombpnet/helpers/preprocessing/
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)        0 2022-12-15 07:53:05.000000 chrombpnet-0.1.3/chrombpnet/helpers/preprocessing/__init__.py
+drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-06-06 23:33:55.119673 chrombpnet-0.1.3/chrombpnet/helpers/preprocessing/analysis/
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)        0 2022-12-15 07:53:05.000000 chrombpnet-0.1.3/chrombpnet/helpers/preprocessing/analysis/__init__.py
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)     2950 2023-01-28 21:08:16.000000 chrombpnet-0.1.3/chrombpnet/helpers/preprocessing/analysis/build_pwm_from_bigwig.py
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)    11082 2023-03-24 21:18:52.000000 chrombpnet-0.1.3/chrombpnet/helpers/preprocessing/auto_shift_detect.py
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)     5103 2023-03-24 21:18:52.000000 chrombpnet-0.1.3/chrombpnet/helpers/preprocessing/reads_to_bigwig.py
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)    27194 2023-01-28 21:08:16.000000 chrombpnet-0.1.3/chrombpnet/parsers.py
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)    24932 2023-01-28 21:08:16.000000 chrombpnet-0.1.3/chrombpnet/pipelines.py
+drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-06-06 23:33:55.119673 chrombpnet-0.1.3/chrombpnet/training/
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)        0 2022-12-15 07:53:05.000000 chrombpnet-0.1.3/chrombpnet/training/__init__.py
+drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-06-06 23:33:55.123673 chrombpnet-0.1.3/chrombpnet/training/data_generators/
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)        0 2022-12-15 07:53:05.000000 chrombpnet-0.1.3/chrombpnet/training/data_generators/__init__.py
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)     5518 2022-12-15 07:53:05.000000 chrombpnet-0.1.3/chrombpnet/training/data_generators/batchgen_generator.py
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)     4418 2022-12-15 07:53:05.000000 chrombpnet-0.1.3/chrombpnet/training/data_generators/initializers.py
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)     4755 2023-01-28 21:08:16.000000 chrombpnet-0.1.3/chrombpnet/training/metrics.py
+drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-06-06 23:33:55.123673 chrombpnet-0.1.3/chrombpnet/training/models/
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)        0 2022-12-15 07:53:05.000000 chrombpnet-0.1.3/chrombpnet/training/models/__init__.py
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)     4048 2022-12-15 07:53:05.000000 chrombpnet-0.1.3/chrombpnet/training/models/bpnet_model.py
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)     6167 2023-01-28 21:08:16.000000 chrombpnet-0.1.3/chrombpnet/training/models/chrombpnet_with_bias_model.py
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)     7742 2023-04-11 00:50:14.000000 chrombpnet-0.1.3/chrombpnet/training/predict.py
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)     4817 2023-01-28 21:08:16.000000 chrombpnet-0.1.3/chrombpnet/training/train.py
+drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-06-06 23:33:55.131674 chrombpnet-0.1.3/chrombpnet/training/utils/
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)        0 2022-12-15 07:53:05.000000 chrombpnet-0.1.3/chrombpnet/training/utils/__init__.py
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)     3781 2023-01-28 21:08:16.000000 chrombpnet-0.1.3/chrombpnet/training/utils/argmanager.py
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)     3060 2022-12-15 07:53:05.000000 chrombpnet-0.1.3/chrombpnet/training/utils/augment.py
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)     1538 2022-12-15 07:53:05.000000 chrombpnet-0.1.3/chrombpnet/training/utils/callbacks.py
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)     3553 2022-12-15 07:53:05.000000 chrombpnet-0.1.3/chrombpnet/training/utils/data_utils.py
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)      687 2022-12-15 07:53:05.000000 chrombpnet-0.1.3/chrombpnet/training/utils/losses.py
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)     6434 2023-01-28 21:08:16.000000 chrombpnet-0.1.3/chrombpnet/training/utils/metrics_utils.py
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)     2565 2022-12-15 07:53:05.000000 chrombpnet-0.1.3/chrombpnet/training/utils/one_hot.py
+drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-06-06 23:33:55.083670 chrombpnet-0.1.3/chrombpnet.egg-info/
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)      270 2023-06-06 23:33:55.000000 chrombpnet-0.1.3/chrombpnet.egg-info/PKG-INFO
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)     3868 2023-06-06 23:33:55.000000 chrombpnet-0.1.3/chrombpnet.egg-info/SOURCES.txt
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)        1 2023-06-06 23:33:55.000000 chrombpnet-0.1.3/chrombpnet.egg-info/dependency_links.txt
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)      129 2023-06-06 23:33:55.000000 chrombpnet-0.1.3/chrombpnet.egg-info/entry_points.txt
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)        1 2023-03-24 22:45:11.000000 chrombpnet-0.1.3/chrombpnet.egg-info/not-zip-safe
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)      345 2023-06-06 23:33:55.000000 chrombpnet-0.1.3/chrombpnet.egg-info/requires.txt
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)       11 2023-06-06 23:33:55.000000 chrombpnet-0.1.3/chrombpnet.egg-info/top_level.txt
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)      411 2023-06-06 23:17:02.000000 chrombpnet-0.1.3/requirements.txt
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)       38 2023-06-06 23:33:55.135674 chrombpnet-0.1.3/setup.cfg
+-rwxrwxr-x   0 anusri    (1005) anusri    (1006)     1038 2023-06-06 23:20:52.000000 chrombpnet-0.1.3/setup.py
+drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-06-06 23:33:55.131674 chrombpnet-0.1.3/tests/
+-rwxrwxr-x   0 anusri    (1005) anusri    (1006)     3028 2023-01-28 21:08:16.000000 chrombpnet-0.1.3/tests/full_workflow.sh
+-rwxrwxr-x   0 anusri    (1005) anusri    (1006)     1496 2022-12-15 07:53:05.000000 chrombpnet-0.1.3/tests/genomewide_gc_bin_test.sh
+-rwxrwxr-x   0 anusri    (1005) anusri    (1006)      349 2022-12-15 07:53:05.000000 chrombpnet-0.1.3/tests/test_pred_to_bigwig.sh
+drwxrwxr-x   0 anusri    (1005) anusri    (1006)        0 2023-06-06 23:33:55.131674 chrombpnet-0.1.3/workflows/
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)    12178 2023-01-28 21:08:16.000000 chrombpnet-0.1.3/workflows/train_bias_model.sh
+-rw-rw-r--   0 anusri    (1005) anusri    (1006)    17611 2023-01-28 21:08:16.000000 chrombpnet-0.1.3/workflows/train_chrombpnet_model.sh
```

### Comparing `chrombpnet-0.1.2/LICENSE` & `chrombpnet-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chrombpnet-0.1.2/README.md` & `chrombpnet-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Bias factorized, base-resolution deep learning models of chromatin accessibility reveal cis-regulatory sequence syntax, transcription factor footprints and regulatory variants
 
 - This repo contains code for the paper `Bias factorized, base-resolution deep learning models of chromatin accessibility reveal cis-regulatory sequence syntax, transcription factor footprints and regulatory variants` (techincal report coming soon) by  Anusri Pampari*, Anna Shcherbina*, Anshul Kundaje. (*authors contributed equally)  
 - Please contact [Anusri Pampari] (\<first-name\>@stanford.edu) for suggestions and comments. 
-- Here is a link to the [slides](https://docs.google.com/presentation/d/1Ow6K8TYN40u7T3ODdo-JRCLuv5fUUacA/edit?usp=sharing&ouid=104820480456877027097&rtpof=true&sd=true) and a comprehensive [tutorial](https://github.com/kundajelab/chrombpnet/wiki). Please see the [FAQ](https://github.com/kundajelab/chrombpnet/wiki/FAQ) and file a github [issue](https://github.com/kundajelab/chrombpnet/issues) if you have questions.
+- Here is a link to the [slides](https://docs.google.com/presentation/d/1Ow6K8TYN40u7T3ODdo-JRCLuv5fUUacA/edit?usp=sharing&ouid=104820480456877027097&rtpof=true&sd=true), [ISMB talk](https://www.youtube.com/watch?v=3W3JeJvvjLc) and a comprehensive [tutorial](https://github.com/kundajelab/chrombpnet/wiki). Please see the [FAQ](https://github.com/kundajelab/chrombpnet/wiki/FAQ) and file a github [issue](https://github.com/kundajelab/chrombpnet/issues) if you have questions.
 
 Chromatin profiles (DNASE-seq and ATAC-seq) exhibit multi-resolution shapes and spans regulated by co-operative binding of transcription factors (TFs). This complexity is further difficult to mine because of confounding bias from enzymes (DNASE-I/Tn5) used in these assays. Existing methods do not account for this complexity at base-resolution and do not account for enzyme bias correctly, thus missing the high-resolution architecture of these profile. Here we introduce ChromBPNet to address both these aspects.
 
 ChromBPNet (shown in the image as `Bias-Factorized ChromBPNet`) is a fully convolutional neural network that uses dilated convolutions with residual connections to enable large receptive fields with efficient parameterization. It also performs automatic assay bias correction in two steps, first by learning simple model on chromatin background that captures the enzyme effect (called `Frozen Bias Model` in the image). Then we use this model to regress out the effect of the enzyme from the ATAC-seq/DNASE-seq profiles. This two step process ensures that the sequence component of the ChromBPNet model (called `TF Model`) does not learn enzymatic bias. 
 
 <p align="center">
 <img src="images/chrombpnet_arch.png" alt="ChromBPNet" align="center" style="width: 400px;"/>
```

#### html2text {}

```diff
@@ -4,34 +4,35 @@
 `Bias factorized, base-resolution deep learning models of chromatin
 accessibility reveal cis-regulatory sequence syntax, transcription factor
 footprints and regulatory variants` (techincal report coming soon) by Anusri
 Pampari*, Anna Shcherbina*, Anshul Kundaje. (*authors contributed equally) -
 Please contact [Anusri Pampari] (\
 >@stanford.edu) for suggestions and comments. - Here is a link to the [slides]
 (https://docs.google.com/presentation/d/1Ow6K8TYN40u7T3ODdo-JRCLuv5fUUacA/
-edit?usp=sharing&ouid=104820480456877027097&rtpof=true&sd=true) and a
-comprehensive [tutorial](https://github.com/kundajelab/chrombpnet/wiki). Please
-see the [FAQ](https://github.com/kundajelab/chrombpnet/wiki/FAQ) and file a
-github [issue](https://github.com/kundajelab/chrombpnet/issues) if you have
-questions. Chromatin profiles (DNASE-seq and ATAC-seq) exhibit multi-resolution
-shapes and spans regulated by co-operative binding of transcription factors
-(TFs). This complexity is further difficult to mine because of confounding bias
-from enzymes (DNASE-I/Tn5) used in these assays. Existing methods do not
-account for this complexity at base-resolution and do not account for enzyme
-bias correctly, thus missing the high-resolution architecture of these profile.
-Here we introduce ChromBPNet to address both these aspects. ChromBPNet (shown
-in the image as `Bias-Factorized ChromBPNet`) is a fully convolutional neural
-network that uses dilated convolutions with residual connections to enable
-large receptive fields with efficient parameterization. It also performs
-automatic assay bias correction in two steps, first by learning simple model on
-chromatin background that captures the enzyme effect (called `Frozen Bias
-Model` in the image). Then we use this model to regress out the effect of the
-enzyme from the ATAC-seq/DNASE-seq profiles. This two step process ensures that
-the sequence component of the ChromBPNet model (called `TF Model`) does not
-learn enzymatic bias.
+edit?usp=sharing&ouid=104820480456877027097&rtpof=true&sd=true), [ISMB talk]
+(https://www.youtube.com/watch?v=3W3JeJvvjLc) and a comprehensive [tutorial]
+(https://github.com/kundajelab/chrombpnet/wiki). Please see the [FAQ](https://
+github.com/kundajelab/chrombpnet/wiki/FAQ) and file a github [issue](https://
+github.com/kundajelab/chrombpnet/issues) if you have questions. Chromatin
+profiles (DNASE-seq and ATAC-seq) exhibit multi-resolution shapes and spans
+regulated by co-operative binding of transcription factors (TFs). This
+complexity is further difficult to mine because of confounding bias from
+enzymes (DNASE-I/Tn5) used in these assays. Existing methods do not account for
+this complexity at base-resolution and do not account for enzyme bias
+correctly, thus missing the high-resolution architecture of these profile. Here
+we introduce ChromBPNet to address both these aspects. ChromBPNet (shown in the
+image as `Bias-Factorized ChromBPNet`) is a fully convolutional neural network
+that uses dilated convolutions with residual connections to enable large
+receptive fields with efficient parameterization. It also performs automatic
+assay bias correction in two steps, first by learning simple model on chromatin
+background that captures the enzyme effect (called `Frozen Bias Model` in the
+image). Then we use this model to regress out the effect of the enzyme from the
+ATAC-seq/DNASE-seq profiles. This two step process ensures that the sequence
+component of the ChromBPNet model (called `TF Model`) does not learn enzymatic
+bias.
                                  [ChromBPNet]
 ## Table of contents - [Installation](#installation) - [QuickStart]
 (#quickstart) - [How-to-cite](#how-to-cite) ## Installation This section will
 discuss the packages needed to train a ChromBPNet model. Firstly, it is
 recommended that you use a GPU for model training and have the necessary NVIDIA
 drivers and CUDA already installed. You can verify that your machine is set up
 to use GPU's properly by executing the `nvidia-smi` command and ensuring that
```

### Comparing `chrombpnet-0.1.2/chrombpnet/CHROMBPNET.py` & `chrombpnet-0.1.3/chrombpnet/CHROMBPNET.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
 			negatives = pd.read_csv(args.output_prefix+"_auxiliary/negatives.bed", sep="\t", header=None)
 			negatives[3]="."
 			negatives[4]="."
 			negatives[5]="."
 			negatives[6]="."
 			negatives[7]="."
 			negatives[8]="."
-			negatives[9]=1057
+			negatives[9]=args.inputlen//2
 			negatives.to_csv(args.output_prefix+"_negatives.bed", sep="\t", header=False, index=False)
 
 		elif args.cmd_prep == "splits":
 			import chrombpnet.helpers.make_chr_splits.splits as splits
 			splits.main(args)
 			
 		else:
```

### Comparing `chrombpnet-0.1.2/chrombpnet/data/ATAC.ref.motifs.txt` & `chrombpnet-0.1.3/chrombpnet/data/ATAC.ref.motifs.txt`

 * *Files identical despite different names*

### Comparing `chrombpnet-0.1.2/chrombpnet/data/DNASE.ref.motifs.txt` & `chrombpnet-0.1.3/chrombpnet/data/DNASE.ref.motifs.txt`

 * *Files identical despite different names*

### Comparing `chrombpnet-0.1.2/chrombpnet/data/__init__.py` & `chrombpnet-0.1.3/chrombpnet/data/__init__.py`

 * *Files identical despite different names*

### Comparing `chrombpnet-0.1.2/chrombpnet/data/motifs.meme.txt` & `chrombpnet-0.1.3/chrombpnet/data/motifs.meme.txt`

 * *Files identical despite different names*

### Comparing `chrombpnet-0.1.2/chrombpnet/evaluation/interpret/input_utils.py` & `chrombpnet-0.1.3/chrombpnet/evaluation/interpret/input_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,12 +27,12 @@
     return one_hot.dna_to_one_hot(vals), np.array(peaks_used)
 
 
 def load_model_wrapper(args):
     # read .h5 model
     custom_objects={"multinomial_nll": losses.multinomial_nll, "tf": tf}    
     get_custom_objects().update(custom_objects)    
-    model=load_model(args.model_h5)
+    model=load_model(args.model_h5,compile=False)
     print("got the model")
     model.summary()
     return model
```

### Comparing `chrombpnet-0.1.2/chrombpnet/evaluation/interpret/interpret.py` & `chrombpnet-0.1.3/chrombpnet/evaluation/interpret/interpret.py`

 * *Files identical despite different names*

### Comparing `chrombpnet-0.1.2/chrombpnet/evaluation/interpret/shap_utils.py` & `chrombpnet-0.1.3/chrombpnet/evaluation/interpret/shap_utils.py`

 * *Files identical despite different names*

### Comparing `chrombpnet-0.1.2/chrombpnet/evaluation/invivo_footprints/run_tfmodisco.py` & `chrombpnet-0.1.3/chrombpnet/evaluation/invivo_footprints/run_tfmodisco.py`

 * *Files identical despite different names*

### Comparing `chrombpnet-0.1.2/chrombpnet/evaluation/invivo_footprints/tf_modiscohits.py` & `chrombpnet-0.1.3/chrombpnet/evaluation/invivo_footprints/tf_modiscohits.py`

 * *Files identical despite different names*

### Comparing `chrombpnet-0.1.2/chrombpnet/evaluation/make_bigwigs/bigwig_helper.py` & `chrombpnet-0.1.3/chrombpnet/evaluation/make_bigwigs/bigwig_helper.py`

 * *Files identical despite different names*

### Comparing `chrombpnet-0.1.2/chrombpnet/evaluation/make_bigwigs/importance_hdf5_to_bigwig.py` & `chrombpnet-0.1.3/chrombpnet/evaluation/make_bigwigs/importance_hdf5_to_bigwig.py`

 * *Files identical despite different names*

### Comparing `chrombpnet-0.1.2/chrombpnet/evaluation/make_bigwigs/predict_to_bigwig.py` & `chrombpnet-0.1.3/chrombpnet/evaluation/make_bigwigs/predict_to_bigwig.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
     norm_x = x - np.mean(x,axis=1, keepdims=True)
     return np.exp(temp*norm_x)/np.sum(np.exp(temp*norm_x), axis=1, keepdims=True)
 
 def load_model_wrapper(model_hdf5):
     # read .h5 model
     custom_objects={"multinomial_nll":losses.multinomial_nll, "tf": tf}    
     get_custom_objects().update(custom_objects)    
-    model=load_model(model_hdf5)
+    model=load_model(model_hdf5, compile=False)
     print("got the model")
     model.summary()
     return model
 
 def main(args):
```

### Comparing `chrombpnet-0.1.2/chrombpnet/evaluation/marginal_footprints/marginal_footprinting.py` & `chrombpnet-0.1.3/chrombpnet/evaluation/marginal_footprints/marginal_footprinting.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 NARROWPEAK_SCHEMA = ["chr", "start", "end", "1", "2", "3", "4", "5", "6", "summit"]
 PWM_SCHEMA = ["MOTIF_NAME", "MOTIF_PWM_FWD"]
 
 def load_model_wrapper(args):
     # read .h5 model
     custom_objects={"multinomial_nll":losses.multinomial_nll, "tf": tf}    
     get_custom_objects().update(custom_objects)    
-    model=load_model(args.model_h5)
+    model=load_model(args.model_h5, compile=False)
     print("got the model")
     model.summary()
     return model
 
 
 def fetch_footprinting_args():
     parser=argparse.ArgumentParser(description="get marginal footprinting for given model and given motifs")
@@ -138,19 +138,19 @@
 		plt.ylabel("Probability", fontsize=11)
 		plt.xticks(ticks=[0,100,200], labels=[-100,0,100])
 		plt.tight_layout()
 		plt.savefig(args.output_prefix+".{}.footprint.png".format(motif))
 
 	if len(avg_response_at_tn5) > 0:
 		if np.all(np.array(avg_response_at_tn5) < 0.003):
-			ofile = open("{}_max_bias_resonse.txt".format(args.output_prefix), "w")
+			ofile = open("{}_max_bias_response.txt".format(args.output_prefix), "w")
 			ofile.write("corrected_"+str(round(np.mean(avg_response_at_tn5),3))+"_"+"/".join(list(map(str,avg_response_at_tn5))))
 			ofile.close()
 		else:
-			ofile = open("{}_max_bias_resonse.txt".format(args.output_prefix), "w")
+			ofile = open("{}_max_bias_response.txt".format(args.output_prefix), "w")
 			ofile.write("uncorrected_"+str(round(np.mean(avg_response_at_tn5),3))+"_"+"/".join(list(map(str,avg_response_at_tn5))))
 			ofile.close()
 
 	print("Saving marginal footprints")
 	dd.io.save("{}_footprints.h5".format(args.output_prefix),
 		footprints_at_motifs,
 		compression='blosc')
```

### Comparing `chrombpnet-0.1.2/chrombpnet/evaluation/modisco/convert_html_to_pdf.py` & `chrombpnet-0.1.3/chrombpnet/evaluation/modisco/convert_html_to_pdf.py`

 * *Files identical despite different names*

### Comparing `chrombpnet-0.1.2/chrombpnet/evaluation/modisco/fetch_tomtom.py` & `chrombpnet-0.1.3/chrombpnet/evaluation/modisco/fetch_tomtom.py`

 * *Files identical despite different names*

### Comparing `chrombpnet-0.1.2/chrombpnet/evaluation/modisco/run_modisco.py` & `chrombpnet-0.1.3/chrombpnet/evaluation/modisco/run_modisco.py`

 * *Files identical despite different names*

### Comparing `chrombpnet-0.1.2/chrombpnet/evaluation/modisco/visualize_motif_matches.py` & `chrombpnet-0.1.3/chrombpnet/evaluation/modisco/visualize_motif_matches.py`

 * *Files identical despite different names*

### Comparing `chrombpnet-0.1.2/chrombpnet/evaluation/variant_effect_prediction/snp_generator.py` & `chrombpnet-0.1.3/chrombpnet/evaluation/variant_effect_prediction/snp_generator.py`

 * *Files identical despite different names*

### Comparing `chrombpnet-0.1.2/chrombpnet/evaluation/variant_effect_prediction/snp_scoring.py` & `chrombpnet-0.1.3/chrombpnet/evaluation/variant_effect_prediction/snp_scoring.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     norm_x = x - np.mean(x,axis=1, keepdims=True)
     return np.exp(temp*norm_x)/np.sum(np.exp(temp*norm_x), axis=1, keepdims=True)
 
 def load_model_wrapper(args):
     # read .h5 model
     custom_objects={"tf": tf, "multinomial_nll":losses.multinomial_nll}    
     get_custom_objects().update(custom_objects)    
-    model=load_model(args.model_h5)
+    model=load_model(args.model_h5, compile=False)
     print("model loaded succesfully")
     return model
 
 def fetch_snp_predictions(model, snp_regions, inputlen, genome_fasta, batch_size, debug_mode_on=False):
     '''
     Returns model predictions (counts and profile probability predictions) at the given reference and alternate snp alleles.
     Please note that if the SNP location is at the edge - i.e we are unable to form a given inputlen of sequence - we skip predictions at this SNP
```

### Comparing `chrombpnet-0.1.2/chrombpnet/evaluation/variant_effect_prediction/testing.py` & `chrombpnet-0.1.3/chrombpnet/evaluation/variant_effect_prediction/testing.py`

 * *Files identical despite different names*

### Comparing `chrombpnet-0.1.2/chrombpnet/helpers/generate_reports/make_html.py` & `chrombpnet-0.1.3/chrombpnet/helpers/generate_reports/make_html.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 		
 	## Marginal footprinting on enzyme bias
 	
 	marg_hed = 'ChromBPNet marginal footprints on tn5 motifs'
 	marg_text = 'The marginal footprints are the response of the ChromBPNet no bias model to the hetergenous bias motifs. \
 	If the bias correction is complete the max of the profiles below should be below 0.003 on all the \
 	bias motifs. '
-	data = open(os.path.join(prefix,"evaluation/{}chrombpnet_nobias_max_bias_resonse.txt".format(fpx))).read()
+	data = open(os.path.join(prefix,"evaluation/{}chrombpnet_nobias_max_bias_response.txt".format(fpx))).read()
 	vals = data.split("_")
 	marg_text1 = "For your convenience we calculate here the average of the max of the profiles: "+vals[1]+" And the model according to this is <b>"+vals[0]+"</b> \
 	<br> \
 	<br> \
 	<b> What to do if your model looks uncorrected (i.e max of profiles is greater than 0.003)? </b> <br> \
 	Look at the motifs below captured by TFModisco and you should be able to see motifs that closely look like the bias motifs showing incomplete bias correction. \
 	This indicates that your bias model was not completely capturing the response of the bias. We recommend that you \
```

### Comparing `chrombpnet-0.1.2/chrombpnet/helpers/generate_reports/make_html_bias.py` & `chrombpnet-0.1.3/chrombpnet/helpers/generate_reports/make_html_bias.py`

 * *Files identical despite different names*

### Comparing `chrombpnet-0.1.2/chrombpnet/helpers/hyperparameters/find_bias_hyperparams.py` & `chrombpnet-0.1.3/chrombpnet/helpers/hyperparameters/find_bias_hyperparams.py`

 * *Files identical despite different names*

### Comparing `chrombpnet-0.1.2/chrombpnet/helpers/hyperparameters/find_chrombpnet_hyperparams.py` & `chrombpnet-0.1.3/chrombpnet/helpers/hyperparameters/find_chrombpnet_hyperparams.py`

 * *Files identical despite different names*

### Comparing `chrombpnet-0.1.2/chrombpnet/helpers/hyperparameters/param_utils.py` & `chrombpnet-0.1.3/chrombpnet/helpers/hyperparameters/param_utils.py`

 * *Files identical despite different names*

### Comparing `chrombpnet-0.1.2/chrombpnet/helpers/make_chr_splits/splits.py` & `chrombpnet-0.1.3/chrombpnet/helpers/make_chr_splits/splits.py`

 * *Files identical despite different names*

### Comparing `chrombpnet-0.1.2/chrombpnet/helpers/make_gc_matched_negatives/get_gc_content.py` & `chrombpnet-0.1.3/chrombpnet/helpers/make_gc_matched_negatives/get_gc_content.py`

 * *Files identical despite different names*

### Comparing `chrombpnet-0.1.2/chrombpnet/helpers/make_gc_matched_negatives/get_gc_matched_negatives.py` & `chrombpnet-0.1.3/chrombpnet/helpers/make_gc_matched_negatives/get_gc_matched_negatives.py`

 * *Files identical despite different names*

### Comparing `chrombpnet-0.1.2/chrombpnet/helpers/make_gc_matched_negatives/get_genomewide_gc_buckets/get_genomewide_gc_bins.py` & `chrombpnet-0.1.3/chrombpnet/helpers/make_gc_matched_negatives/get_genomewide_gc_buckets/get_genomewide_gc_bins.py`

 * *Files identical despite different names*

### Comparing `chrombpnet-0.1.2/chrombpnet/helpers/preprocessing/analysis/build_pwm_from_bigwig.py` & `chrombpnet-0.1.3/chrombpnet/helpers/preprocessing/analysis/build_pwm_from_bigwig.py`

 * *Files identical despite different names*

### Comparing `chrombpnet-0.1.2/chrombpnet/helpers/preprocessing/auto_shift_detect.py` & `chrombpnet-0.1.3/chrombpnet/helpers/preprocessing/auto_shift_detect.py`

 * *Files identical despite different names*

### Comparing `chrombpnet-0.1.2/chrombpnet/helpers/preprocessing/reads_to_bigwig.py` & `chrombpnet-0.1.3/chrombpnet/helpers/preprocessing/reads_to_bigwig.py`

 * *Files identical despite different names*

### Comparing `chrombpnet-0.1.2/chrombpnet/parsers.py` & `chrombpnet-0.1.3/chrombpnet/parsers.py`

 * *Files identical despite different names*

### Comparing `chrombpnet-0.1.2/chrombpnet/pipelines.py` & `chrombpnet-0.1.3/chrombpnet/pipelines.py`

 * *Files identical despite different names*

### Comparing `chrombpnet-0.1.2/chrombpnet/training/data_generators/batchgen_generator.py` & `chrombpnet-0.1.3/chrombpnet/training/data_generators/batchgen_generator.py`

 * *Files identical despite different names*

### Comparing `chrombpnet-0.1.2/chrombpnet/training/data_generators/initializers.py` & `chrombpnet-0.1.3/chrombpnet/training/data_generators/initializers.py`

 * *Files identical despite different names*

### Comparing `chrombpnet-0.1.2/chrombpnet/training/metrics.py` & `chrombpnet-0.1.3/chrombpnet/training/metrics.py`

 * *Files identical despite different names*

### Comparing `chrombpnet-0.1.2/chrombpnet/training/models/bpnet_model.py` & `chrombpnet-0.1.3/chrombpnet/training/models/bpnet_model.py`

 * *Files identical despite different names*

### Comparing `chrombpnet-0.1.2/chrombpnet/training/models/chrombpnet_with_bias_model.py` & `chrombpnet-0.1.3/chrombpnet/training/models/chrombpnet_with_bias_model.py`

 * *Files identical despite different names*

### Comparing `chrombpnet-0.1.2/chrombpnet/training/predict.py` & `chrombpnet-0.1.3/chrombpnet/training/predict.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     h5_file.close()
 
 
 def load_model_wrapper(args):
     # read .h5 model
     custom_objects={"tf": tf, "multinomial_nll":losses.multinomial_nll}    
     get_custom_objects().update(custom_objects)    
-    model=load_model(args.model_h5)
+    model=load_model(args.model_h5, compile=False)
     print("got the model")
     #model.summary()
     return model
 
 def softmax(x, temp=1):
     norm_x = x - np.mean(x,axis=1, keepdims=True)
     return np.exp(temp*norm_x)/np.sum(np.exp(temp*norm_x), axis=1, keepdims=True)
```

### Comparing `chrombpnet-0.1.2/chrombpnet/training/train.py` & `chrombpnet-0.1.3/chrombpnet/training/train.py`

 * *Files identical despite different names*

### Comparing `chrombpnet-0.1.2/chrombpnet/training/utils/argmanager.py` & `chrombpnet-0.1.3/chrombpnet/training/utils/argmanager.py`

 * *Files identical despite different names*

### Comparing `chrombpnet-0.1.2/chrombpnet/training/utils/augment.py` & `chrombpnet-0.1.3/chrombpnet/training/utils/augment.py`

 * *Files identical despite different names*

### Comparing `chrombpnet-0.1.2/chrombpnet/training/utils/callbacks.py` & `chrombpnet-0.1.3/chrombpnet/training/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `chrombpnet-0.1.2/chrombpnet/training/utils/data_utils.py` & `chrombpnet-0.1.3/chrombpnet/training/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `chrombpnet-0.1.2/chrombpnet/training/utils/losses.py` & `chrombpnet-0.1.3/chrombpnet/training/utils/losses.py`

 * *Files identical despite different names*

### Comparing `chrombpnet-0.1.2/chrombpnet/training/utils/metrics_utils.py` & `chrombpnet-0.1.3/chrombpnet/training/utils/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `chrombpnet-0.1.2/chrombpnet/training/utils/one_hot.py` & `chrombpnet-0.1.3/chrombpnet/training/utils/one_hot.py`

 * *Files identical despite different names*

### Comparing `chrombpnet-0.1.2/chrombpnet.egg-info/SOURCES.txt` & `chrombpnet-0.1.3/chrombpnet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chrombpnet-0.1.2/setup.py` & `chrombpnet-0.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 config = {
     'name': 'chrombpnet',
     'author_email': 'anusri @ stanford.edu',
     'license': 'MIT',
     'include_package_data': True,
     'description': 'chrombpnet predicts chromatin accessibility from sequence',
     'download_url': 'https://github.com/kundajelab/chrombpnet',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'packages': find_packages(),
     'python_requires': '>=3.8',
     'install_requires': install_requires,
     'zip_safe': False,
     'scripts':[
                'chrombpnet/training/models/bpnet_model.py',
                'chrombpnet/training/models/chrombpnet_with_bias_model.py'
```

### Comparing `chrombpnet-0.1.2/tests/full_workflow.sh` & `chrombpnet-0.1.3/tests/full_workflow.sh`

 * *Files identical despite different names*

### Comparing `chrombpnet-0.1.2/tests/genomewide_gc_bin_test.sh` & `chrombpnet-0.1.3/tests/genomewide_gc_bin_test.sh`

 * *Files identical despite different names*

### Comparing `chrombpnet-0.1.2/workflows/train_bias_model.sh` & `chrombpnet-0.1.3/workflows/train_bias_model.sh`

 * *Files identical despite different names*

### Comparing `chrombpnet-0.1.2/workflows/train_chrombpnet_model.sh` & `chrombpnet-0.1.3/workflows/train_chrombpnet_model.sh`

 * *Files identical despite different names*

