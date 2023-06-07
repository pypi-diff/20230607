# Comparing `tmp/torchrec_nightly-2023.6.5-py39-none-any.whl.zip` & `tmp/torchrec_nightly-2023.6.6-py39-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,144 +1,145 @@
-Zip file size: 349142 bytes, number of entries: 142
--rw-r--r--  2.0 unx      811 b- defN 23-Jun-05 11:18 torchrec/__init__.py
--rw-r--r--  2.0 unx     1638 b- defN 23-Jun-05 11:18 torchrec/streamable.py
--rw-r--r--  2.0 unx      854 b- defN 23-Jun-05 11:18 torchrec/types.py
--rw-r--r--  2.0 unx     1153 b- defN 23-Jun-05 11:18 torchrec/datasets/__init__.py
--rw-r--r--  2.0 unx    41469 b- defN 23-Jun-05 11:18 torchrec/datasets/criteo.py
--rw-r--r--  2.0 unx     4548 b- defN 23-Jun-05 11:18 torchrec/datasets/movielens.py
--rw-r--r--  2.0 unx     6539 b- defN 23-Jun-05 11:18 torchrec/datasets/random.py
--rw-r--r--  2.0 unx    10909 b- defN 23-Jun-05 11:18 torchrec/datasets/utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-05 11:18 torchrec/datasets/scripts/__init__.py
--rw-r--r--  2.0 unx     2448 b- defN 23-Jun-05 11:18 torchrec/datasets/scripts/contiguous_preproc_criteo.py
--rw-r--r--  2.0 unx     2847 b- defN 23-Jun-05 11:18 torchrec/datasets/scripts/npy_preproc_criteo.py
--rw-r--r--  2.0 unx     3077 b- defN 23-Jun-05 11:18 torchrec/datasets/scripts/shuffle_preproc_criteo.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-05 11:18 torchrec/datasets/test_utils/__init__.py
--rw-r--r--  2.0 unx     5308 b- defN 23-Jun-05 11:18 torchrec/datasets/test_utils/criteo_test_utils.py
--rw-r--r--  2.0 unx     1912 b- defN 23-Jun-05 11:18 torchrec/distributed/__init__.py
--rw-r--r--  2.0 unx    37053 b- defN 23-Jun-05 11:18 torchrec/distributed/batched_embedding_kernel.py
--rw-r--r--  2.0 unx     2069 b- defN 23-Jun-05 11:18 torchrec/distributed/collective_utils.py
--rw-r--r--  2.0 unx     4988 b- defN 23-Jun-05 11:18 torchrec/distributed/comm.py
--rw-r--r--  2.0 unx    55918 b- defN 23-Jun-05 11:18 torchrec/distributed/comm_ops.py
--rw-r--r--  2.0 unx    35580 b- defN 23-Jun-05 11:18 torchrec/distributed/dist_data.py
--rw-r--r--  2.0 unx    30257 b- defN 23-Jun-05 11:18 torchrec/distributed/embedding.py
--rw-r--r--  2.0 unx     3872 b- defN 23-Jun-05 11:18 torchrec/distributed/embedding_kernel.py
--rw-r--r--  2.0 unx    28994 b- defN 23-Jun-05 11:18 torchrec/distributed/embedding_lookup.py
--rw-r--r--  2.0 unx    18564 b- defN 23-Jun-05 11:18 torchrec/distributed/embedding_sharding.py
--rw-r--r--  2.0 unx    37089 b- defN 23-Jun-05 11:18 torchrec/distributed/embedding_tower_sharding.py
--rw-r--r--  2.0 unx    15030 b- defN 23-Jun-05 11:18 torchrec/distributed/embedding_types.py
--rw-r--r--  2.0 unx    35078 b- defN 23-Jun-05 11:18 torchrec/distributed/embeddingbag.py
--rw-r--r--  2.0 unx     7373 b- defN 23-Jun-05 11:18 torchrec/distributed/fbgemm_qcomm_codec.py
--rw-r--r--  2.0 unx     5542 b- defN 23-Jun-05 11:18 torchrec/distributed/fp_embeddingbag.py
--rw-r--r--  2.0 unx     5273 b- defN 23-Jun-05 11:18 torchrec/distributed/fused_embedding.py
--rw-r--r--  2.0 unx     5110 b- defN 23-Jun-05 11:18 torchrec/distributed/fused_embeddingbag.py
--rw-r--r--  2.0 unx     1709 b- defN 23-Jun-05 11:18 torchrec/distributed/fused_params.py
--rw-r--r--  2.0 unx     3807 b- defN 23-Jun-05 11:18 torchrec/distributed/grouped_position_weighted.py
--rw-r--r--  2.0 unx    19520 b- defN 23-Jun-05 11:18 torchrec/distributed/model_parallel.py
--rw-r--r--  2.0 unx    13729 b- defN 23-Jun-05 11:18 torchrec/distributed/quant_embedding.py
--rw-r--r--  2.0 unx    13343 b- defN 23-Jun-05 11:18 torchrec/distributed/quant_embedding_kernel.py
--rw-r--r--  2.0 unx    10931 b- defN 23-Jun-05 11:18 torchrec/distributed/quant_embeddingbag.py
--rw-r--r--  2.0 unx     9261 b- defN 23-Jun-05 11:18 torchrec/distributed/shard.py
--rw-r--r--  2.0 unx    19411 b- defN 23-Jun-05 11:18 torchrec/distributed/sharding_plan.py
--rw-r--r--  2.0 unx    34059 b- defN 23-Jun-05 11:18 torchrec/distributed/train_pipeline.py
--rw-r--r--  2.0 unx    24927 b- defN 23-Jun-05 11:18 torchrec/distributed/types.py
--rw-r--r--  2.0 unx    11373 b- defN 23-Jun-05 11:18 torchrec/distributed/utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-05 11:18 torchrec/distributed/composable/__init__.py
--rw-r--r--  2.0 unx     3207 b- defN 23-Jun-05 11:18 torchrec/distributed/composable/table_batched_embedding_slice.py
--rw-r--r--  2.0 unx     1025 b- defN 23-Jun-05 11:18 torchrec/distributed/planner/__init__.py
--rw-r--r--  2.0 unx     3135 b- defN 23-Jun-05 11:18 torchrec/distributed/planner/constants.py
--rw-r--r--  2.0 unx    10318 b- defN 23-Jun-05 11:18 torchrec/distributed/planner/enumerators.py
--rw-r--r--  2.0 unx    12642 b- defN 23-Jun-05 11:18 torchrec/distributed/planner/partitioners.py
--rw-r--r--  2.0 unx      835 b- defN 23-Jun-05 11:18 torchrec/distributed/planner/perf_models.py
--rw-r--r--  2.0 unx    13288 b- defN 23-Jun-05 11:18 torchrec/distributed/planner/planners.py
--rw-r--r--  2.0 unx    11134 b- defN 23-Jun-05 11:18 torchrec/distributed/planner/proposers.py
--rw-r--r--  2.0 unx    40395 b- defN 23-Jun-05 11:18 torchrec/distributed/planner/shard_estimators.py
--rw-r--r--  2.0 unx    23617 b- defN 23-Jun-05 11:18 torchrec/distributed/planner/stats.py
--rw-r--r--  2.0 unx     9125 b- defN 23-Jun-05 11:18 torchrec/distributed/planner/storage_reservations.py
--rw-r--r--  2.0 unx    13899 b- defN 23-Jun-05 11:18 torchrec/distributed/planner/types.py
--rw-r--r--  2.0 unx     1119 b- defN 23-Jun-05 11:18 torchrec/distributed/planner/utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-05 11:18 torchrec/distributed/sharding/__init__.py
--rw-r--r--  2.0 unx     2539 b- defN 23-Jun-05 11:18 torchrec/distributed/sharding/cw_sequence_sharding.py
--rw-r--r--  2.0 unx     9519 b- defN 23-Jun-05 11:18 torchrec/distributed/sharding/cw_sharding.py
--rw-r--r--  2.0 unx     2802 b- defN 23-Jun-05 11:18 torchrec/distributed/sharding/dp_sequence_sharding.py
--rw-r--r--  2.0 unx     7681 b- defN 23-Jun-05 11:18 torchrec/distributed/sharding/dp_sharding.py
--rw-r--r--  2.0 unx     5041 b- defN 23-Jun-05 11:18 torchrec/distributed/sharding/rw_sequence_sharding.py
--rw-r--r--  2.0 unx    12850 b- defN 23-Jun-05 11:18 torchrec/distributed/sharding/rw_sharding.py
--rw-r--r--  2.0 unx     3114 b- defN 23-Jun-05 11:18 torchrec/distributed/sharding/sequence_sharding.py
--rw-r--r--  2.0 unx     7692 b- defN 23-Jun-05 11:18 torchrec/distributed/sharding/tw_sequence_sharding.py
--rw-r--r--  2.0 unx    16315 b- defN 23-Jun-05 11:18 torchrec/distributed/sharding/tw_sharding.py
--rw-r--r--  2.0 unx     1284 b- defN 23-Jun-05 11:18 torchrec/distributed/sharding/twcw_sharding.py
--rw-r--r--  2.0 unx    19898 b- defN 23-Jun-05 11:18 torchrec/distributed/sharding/twrw_sharding.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-05 11:18 torchrec/distributed/test_utils/__init__.py
--rw-r--r--  2.0 unx    10213 b- defN 23-Jun-05 11:18 torchrec/distributed/test_utils/infer_utils.py
--rw-r--r--  2.0 unx     4868 b- defN 23-Jun-05 11:18 torchrec/distributed/test_utils/multi_process.py
--rw-r--r--  2.0 unx    34114 b- defN 23-Jun-05 11:18 torchrec/distributed/test_utils/test_model.py
--rw-r--r--  2.0 unx    11193 b- defN 23-Jun-05 11:18 torchrec/distributed/test_utils/test_model_parallel.py
--rw-r--r--  2.0 unx    25075 b- defN 23-Jun-05 11:18 torchrec/distributed/test_utils/test_model_parallel_base.py
--rw-r--r--  2.0 unx    15367 b- defN 23-Jun-05 11:18 torchrec/distributed/test_utils/test_sharding.py
--rw-r--r--  2.0 unx      422 b- defN 23-Jun-05 11:18 torchrec/fx/__init__.py
--rw-r--r--  2.0 unx     6477 b- defN 23-Jun-05 11:18 torchrec/fx/tracer.py
--rw-r--r--  2.0 unx     4401 b- defN 23-Jun-05 11:18 torchrec/fx/utils.py
--rw-r--r--  2.0 unx     1223 b- defN 23-Jun-05 11:18 torchrec/inference/__init__.py
--rw-r--r--  2.0 unx     3614 b- defN 23-Jun-05 11:18 torchrec/inference/client.py
--rw-r--r--  2.0 unx     3957 b- defN 23-Jun-05 11:18 torchrec/inference/model_packager.py
--rw-r--r--  2.0 unx     8068 b- defN 23-Jun-05 11:18 torchrec/inference/modules.py
--rw-r--r--  2.0 unx     3797 b- defN 23-Jun-05 11:18 torchrec/inference/state_dict_transform.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-05 11:18 torchrec/metrics/__init__.py
--rw-r--r--  2.0 unx    12549 b- defN 23-Jun-05 11:18 torchrec/metrics/auc.py
--rw-r--r--  2.0 unx     3703 b- defN 23-Jun-05 11:18 torchrec/metrics/calibration.py
--rw-r--r--  2.0 unx     3465 b- defN 23-Jun-05 11:18 torchrec/metrics/ctr.py
--rw-r--r--  2.0 unx     3836 b- defN 23-Jun-05 11:18 torchrec/metrics/mae.py
--rw-r--r--  2.0 unx    17812 b- defN 23-Jun-05 11:18 torchrec/metrics/metric_module.py
--rw-r--r--  2.0 unx     6752 b- defN 23-Jun-05 11:18 torchrec/metrics/metrics_config.py
--rw-r--r--  2.0 unx     3643 b- defN 23-Jun-05 11:18 torchrec/metrics/metrics_namespace.py
--rw-r--r--  2.0 unx     3904 b- defN 23-Jun-05 11:18 torchrec/metrics/model_utils.py
--rw-r--r--  2.0 unx     4631 b- defN 23-Jun-05 11:18 torchrec/metrics/mse.py
--rw-r--r--  2.0 unx     5605 b- defN 23-Jun-05 11:18 torchrec/metrics/multiclass_recall.py
--rw-r--r--  2.0 unx     6811 b- defN 23-Jun-05 11:18 torchrec/metrics/ne.py
--rw-r--r--  2.0 unx    31495 b- defN 23-Jun-05 11:18 torchrec/metrics/rec_metric.py
--rw-r--r--  2.0 unx    10490 b- defN 23-Jun-05 11:18 torchrec/metrics/recall_session.py
--rw-r--r--  2.0 unx     6057 b- defN 23-Jun-05 11:18 torchrec/metrics/throughput.py
--rw-r--r--  2.0 unx    10622 b- defN 23-Jun-05 11:18 torchrec/metrics/tower_qps.py
--rw-r--r--  2.0 unx     2867 b- defN 23-Jun-05 11:18 torchrec/metrics/weighted_avg.py
--rw-r--r--  2.0 unx    16441 b- defN 23-Jun-05 11:18 torchrec/metrics/test_utils/__init__.py
--rw-r--r--  2.0 unx      913 b- defN 23-Jun-05 11:18 torchrec/models/__init__.py
--rw-r--r--  2.0 unx    11410 b- defN 23-Jun-05 11:18 torchrec/models/deepfm.py
--rw-r--r--  2.0 unx    30000 b- defN 23-Jun-05 11:18 torchrec/models/dlrm.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-05 11:18 torchrec/models/experimental/__init__.py
--rw-r--r--  2.0 unx     9825 b- defN 23-Jun-05 11:18 torchrec/models/experimental/test_transformerdlrm.py
--rw-r--r--  2.0 unx     7434 b- defN 23-Jun-05 11:18 torchrec/models/experimental/transformerdlrm.py
--rw-r--r--  2.0 unx     1179 b- defN 23-Jun-05 11:18 torchrec/modules/__init__.py
--rw-r--r--  2.0 unx     1456 b- defN 23-Jun-05 11:18 torchrec/modules/activation.py
--rw-r--r--  2.0 unx    15163 b- defN 23-Jun-05 11:18 torchrec/modules/crossnet.py
--rw-r--r--  2.0 unx     8415 b- defN 23-Jun-05 11:18 torchrec/modules/deepfm.py
--rw-r--r--  2.0 unx     5537 b- defN 23-Jun-05 11:18 torchrec/modules/embedding_configs.py
--rw-r--r--  2.0 unx    14021 b- defN 23-Jun-05 11:18 torchrec/modules/embedding_modules.py
--rw-r--r--  2.0 unx     4858 b- defN 23-Jun-05 11:18 torchrec/modules/embedding_tower.py
--rw-r--r--  2.0 unx    12360 b- defN 23-Jun-05 11:18 torchrec/modules/feature_processor.py
--rw-r--r--  2.0 unx     2169 b- defN 23-Jun-05 11:18 torchrec/modules/feature_processor_.py
--rw-r--r--  2.0 unx     4028 b- defN 23-Jun-05 11:18 torchrec/modules/fp_embedding_modules.py
--rw-r--r--  2.0 unx    31193 b- defN 23-Jun-05 11:18 torchrec/modules/fused_embedding_modules.py
--rw-r--r--  2.0 unx    10696 b- defN 23-Jun-05 11:18 torchrec/modules/lazy_extension.py
--rw-r--r--  2.0 unx     6309 b- defN 23-Jun-05 11:18 torchrec/modules/mlp.py
--rw-r--r--  2.0 unx     4022 b- defN 23-Jun-05 11:18 torchrec/modules/utils.py
--rw-r--r--  2.0 unx     1639 b- defN 23-Jun-05 11:18 torchrec/optim/__init__.py
--rw-r--r--  2.0 unx     2012 b- defN 23-Jun-05 11:18 torchrec/optim/apply_optimizer_in_backward.py
--rw-r--r--  2.0 unx     1569 b- defN 23-Jun-05 11:18 torchrec/optim/clipping.py
--rw-r--r--  2.0 unx     1353 b- defN 23-Jun-05 11:18 torchrec/optim/fused.py
--rw-r--r--  2.0 unx    16069 b- defN 23-Jun-05 11:18 torchrec/optim/keyed.py
--rw-r--r--  2.0 unx     4420 b- defN 23-Jun-05 11:18 torchrec/optim/optimizers.py
--rw-r--r--  2.0 unx     7405 b- defN 23-Jun-05 11:18 torchrec/optim/rowwise_adagrad.py
--rw-r--r--  2.0 unx     4865 b- defN 23-Jun-05 11:18 torchrec/optim/warmup.py
--rw-r--r--  2.0 unx      560 b- defN 23-Jun-05 11:18 torchrec/optim/test_utils/__init__.py
--rw-r--r--  2.0 unx     1140 b- defN 23-Jun-05 11:18 torchrec/quant/__init__.py
--rw-r--r--  2.0 unx    22933 b- defN 23-Jun-05 11:18 torchrec/quant/embedding_modules.py
--rw-r--r--  2.0 unx     4100 b- defN 23-Jun-05 11:18 torchrec/quant/utils.py
--rw-r--r--  2.0 unx     1163 b- defN 23-Jun-05 11:18 torchrec/sparse/__init__.py
--rw-r--r--  2.0 unx    55649 b- defN 23-Jun-05 11:18 torchrec/sparse/jagged_tensor.py
--rw-r--r--  2.0 unx     1430 b- defN 23-Jun-05 11:18 torchrec/sparse/test_utils/__init__.py
--rw-r--r--  2.0 unx     5661 b- defN 23-Jun-05 11:18 torchrec/test_utils/__init__.py
--rw-r--r--  2.0 unx     1530 b- defN 23-Jun-05 11:22 torchrec_nightly-2023.6.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     5011 b- defN 23-Jun-05 11:22 torchrec_nightly-2023.6.5.dist-info/METADATA
--rw-r--r--  2.0 unx       93 b- defN 23-Jun-05 11:22 torchrec_nightly-2023.6.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jun-05 11:22 torchrec_nightly-2023.6.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    13262 b- defN 23-Jun-05 11:22 torchrec_nightly-2023.6.5.dist-info/RECORD
-142 files, 1422180 bytes uncompressed, 327920 bytes compressed:  76.9%
+Zip file size: 350634 bytes, number of entries: 143
+-rw-r--r--  2.0 unx      811 b- defN 23-Jun-06 11:17 torchrec/__init__.py
+-rw-r--r--  2.0 unx     1638 b- defN 23-Jun-06 11:17 torchrec/streamable.py
+-rw-r--r--  2.0 unx      854 b- defN 23-Jun-06 11:17 torchrec/types.py
+-rw-r--r--  2.0 unx     1153 b- defN 23-Jun-06 11:17 torchrec/datasets/__init__.py
+-rw-r--r--  2.0 unx    41469 b- defN 23-Jun-06 11:17 torchrec/datasets/criteo.py
+-rw-r--r--  2.0 unx     4548 b- defN 23-Jun-06 11:17 torchrec/datasets/movielens.py
+-rw-r--r--  2.0 unx     6539 b- defN 23-Jun-06 11:17 torchrec/datasets/random.py
+-rw-r--r--  2.0 unx    10909 b- defN 23-Jun-06 11:17 torchrec/datasets/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 11:17 torchrec/datasets/scripts/__init__.py
+-rw-r--r--  2.0 unx     2448 b- defN 23-Jun-06 11:17 torchrec/datasets/scripts/contiguous_preproc_criteo.py
+-rw-r--r--  2.0 unx     2847 b- defN 23-Jun-06 11:17 torchrec/datasets/scripts/npy_preproc_criteo.py
+-rw-r--r--  2.0 unx     3077 b- defN 23-Jun-06 11:17 torchrec/datasets/scripts/shuffle_preproc_criteo.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 11:17 torchrec/datasets/test_utils/__init__.py
+-rw-r--r--  2.0 unx     5308 b- defN 23-Jun-06 11:17 torchrec/datasets/test_utils/criteo_test_utils.py
+-rw-r--r--  2.0 unx     1912 b- defN 23-Jun-06 11:17 torchrec/distributed/__init__.py
+-rw-r--r--  2.0 unx    37053 b- defN 23-Jun-06 11:17 torchrec/distributed/batched_embedding_kernel.py
+-rw-r--r--  2.0 unx     2069 b- defN 23-Jun-06 11:17 torchrec/distributed/collective_utils.py
+-rw-r--r--  2.0 unx     4988 b- defN 23-Jun-06 11:17 torchrec/distributed/comm.py
+-rw-r--r--  2.0 unx    55918 b- defN 23-Jun-06 11:17 torchrec/distributed/comm_ops.py
+-rw-r--r--  2.0 unx    35580 b- defN 23-Jun-06 11:17 torchrec/distributed/dist_data.py
+-rw-r--r--  2.0 unx    30257 b- defN 23-Jun-06 11:17 torchrec/distributed/embedding.py
+-rw-r--r--  2.0 unx     3872 b- defN 23-Jun-06 11:17 torchrec/distributed/embedding_kernel.py
+-rw-r--r--  2.0 unx    28994 b- defN 23-Jun-06 11:17 torchrec/distributed/embedding_lookup.py
+-rw-r--r--  2.0 unx    18564 b- defN 23-Jun-06 11:17 torchrec/distributed/embedding_sharding.py
+-rw-r--r--  2.0 unx    37089 b- defN 23-Jun-06 11:17 torchrec/distributed/embedding_tower_sharding.py
+-rw-r--r--  2.0 unx    15030 b- defN 23-Jun-06 11:17 torchrec/distributed/embedding_types.py
+-rw-r--r--  2.0 unx    35078 b- defN 23-Jun-06 11:17 torchrec/distributed/embeddingbag.py
+-rw-r--r--  2.0 unx     7373 b- defN 23-Jun-06 11:17 torchrec/distributed/fbgemm_qcomm_codec.py
+-rw-r--r--  2.0 unx     5542 b- defN 23-Jun-06 11:17 torchrec/distributed/fp_embeddingbag.py
+-rw-r--r--  2.0 unx     5273 b- defN 23-Jun-06 11:17 torchrec/distributed/fused_embedding.py
+-rw-r--r--  2.0 unx     5110 b- defN 23-Jun-06 11:17 torchrec/distributed/fused_embeddingbag.py
+-rw-r--r--  2.0 unx     1709 b- defN 23-Jun-06 11:17 torchrec/distributed/fused_params.py
+-rw-r--r--  2.0 unx     3807 b- defN 23-Jun-06 11:17 torchrec/distributed/grouped_position_weighted.py
+-rw-r--r--  2.0 unx    19520 b- defN 23-Jun-06 11:17 torchrec/distributed/model_parallel.py
+-rw-r--r--  2.0 unx    13729 b- defN 23-Jun-06 11:17 torchrec/distributed/quant_embedding.py
+-rw-r--r--  2.0 unx    13343 b- defN 23-Jun-06 11:17 torchrec/distributed/quant_embedding_kernel.py
+-rw-r--r--  2.0 unx    10931 b- defN 23-Jun-06 11:17 torchrec/distributed/quant_embeddingbag.py
+-rw-r--r--  2.0 unx     9261 b- defN 23-Jun-06 11:17 torchrec/distributed/shard.py
+-rw-r--r--  2.0 unx    19411 b- defN 23-Jun-06 11:17 torchrec/distributed/sharding_plan.py
+-rw-r--r--  2.0 unx    34059 b- defN 23-Jun-06 11:17 torchrec/distributed/train_pipeline.py
+-rw-r--r--  2.0 unx    24927 b- defN 23-Jun-06 11:17 torchrec/distributed/types.py
+-rw-r--r--  2.0 unx    11373 b- defN 23-Jun-06 11:17 torchrec/distributed/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 11:17 torchrec/distributed/composable/__init__.py
+-rw-r--r--  2.0 unx     3207 b- defN 23-Jun-06 11:17 torchrec/distributed/composable/table_batched_embedding_slice.py
+-rw-r--r--  2.0 unx     1025 b- defN 23-Jun-06 11:17 torchrec/distributed/planner/__init__.py
+-rw-r--r--  2.0 unx     3135 b- defN 23-Jun-06 11:17 torchrec/distributed/planner/constants.py
+-rw-r--r--  2.0 unx    10318 b- defN 23-Jun-06 11:17 torchrec/distributed/planner/enumerators.py
+-rw-r--r--  2.0 unx    12642 b- defN 23-Jun-06 11:17 torchrec/distributed/planner/partitioners.py
+-rw-r--r--  2.0 unx      835 b- defN 23-Jun-06 11:17 torchrec/distributed/planner/perf_models.py
+-rw-r--r--  2.0 unx    13288 b- defN 23-Jun-06 11:17 torchrec/distributed/planner/planners.py
+-rw-r--r--  2.0 unx    11134 b- defN 23-Jun-06 11:17 torchrec/distributed/planner/proposers.py
+-rw-r--r--  2.0 unx    40395 b- defN 23-Jun-06 11:17 torchrec/distributed/planner/shard_estimators.py
+-rw-r--r--  2.0 unx    23617 b- defN 23-Jun-06 11:17 torchrec/distributed/planner/stats.py
+-rw-r--r--  2.0 unx     9125 b- defN 23-Jun-06 11:17 torchrec/distributed/planner/storage_reservations.py
+-rw-r--r--  2.0 unx    13899 b- defN 23-Jun-06 11:17 torchrec/distributed/planner/types.py
+-rw-r--r--  2.0 unx     1119 b- defN 23-Jun-06 11:17 torchrec/distributed/planner/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 11:17 torchrec/distributed/sharding/__init__.py
+-rw-r--r--  2.0 unx     2539 b- defN 23-Jun-06 11:17 torchrec/distributed/sharding/cw_sequence_sharding.py
+-rw-r--r--  2.0 unx     9519 b- defN 23-Jun-06 11:17 torchrec/distributed/sharding/cw_sharding.py
+-rw-r--r--  2.0 unx     2802 b- defN 23-Jun-06 11:17 torchrec/distributed/sharding/dp_sequence_sharding.py
+-rw-r--r--  2.0 unx     7681 b- defN 23-Jun-06 11:17 torchrec/distributed/sharding/dp_sharding.py
+-rw-r--r--  2.0 unx     5041 b- defN 23-Jun-06 11:17 torchrec/distributed/sharding/rw_sequence_sharding.py
+-rw-r--r--  2.0 unx    12850 b- defN 23-Jun-06 11:17 torchrec/distributed/sharding/rw_sharding.py
+-rw-r--r--  2.0 unx     3114 b- defN 23-Jun-06 11:17 torchrec/distributed/sharding/sequence_sharding.py
+-rw-r--r--  2.0 unx     7692 b- defN 23-Jun-06 11:17 torchrec/distributed/sharding/tw_sequence_sharding.py
+-rw-r--r--  2.0 unx    16315 b- defN 23-Jun-06 11:17 torchrec/distributed/sharding/tw_sharding.py
+-rw-r--r--  2.0 unx     1284 b- defN 23-Jun-06 11:17 torchrec/distributed/sharding/twcw_sharding.py
+-rw-r--r--  2.0 unx    19898 b- defN 23-Jun-06 11:17 torchrec/distributed/sharding/twrw_sharding.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 11:17 torchrec/distributed/test_utils/__init__.py
+-rw-r--r--  2.0 unx    10213 b- defN 23-Jun-06 11:17 torchrec/distributed/test_utils/infer_utils.py
+-rw-r--r--  2.0 unx     4868 b- defN 23-Jun-06 11:17 torchrec/distributed/test_utils/multi_process.py
+-rw-r--r--  2.0 unx    34114 b- defN 23-Jun-06 11:17 torchrec/distributed/test_utils/test_model.py
+-rw-r--r--  2.0 unx    11193 b- defN 23-Jun-06 11:17 torchrec/distributed/test_utils/test_model_parallel.py
+-rw-r--r--  2.0 unx    25075 b- defN 23-Jun-06 11:17 torchrec/distributed/test_utils/test_model_parallel_base.py
+-rw-r--r--  2.0 unx    15367 b- defN 23-Jun-06 11:17 torchrec/distributed/test_utils/test_sharding.py
+-rw-r--r--  2.0 unx      422 b- defN 23-Jun-06 11:17 torchrec/fx/__init__.py
+-rw-r--r--  2.0 unx     6477 b- defN 23-Jun-06 11:17 torchrec/fx/tracer.py
+-rw-r--r--  2.0 unx     4401 b- defN 23-Jun-06 11:17 torchrec/fx/utils.py
+-rw-r--r--  2.0 unx     1223 b- defN 23-Jun-06 11:17 torchrec/inference/__init__.py
+-rw-r--r--  2.0 unx     3614 b- defN 23-Jun-06 11:17 torchrec/inference/client.py
+-rw-r--r--  2.0 unx     3957 b- defN 23-Jun-06 11:17 torchrec/inference/model_packager.py
+-rw-r--r--  2.0 unx     8068 b- defN 23-Jun-06 11:17 torchrec/inference/modules.py
+-rw-r--r--  2.0 unx     3797 b- defN 23-Jun-06 11:17 torchrec/inference/state_dict_transform.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 11:17 torchrec/metrics/__init__.py
+-rw-r--r--  2.0 unx     4168 b- defN 23-Jun-06 11:17 torchrec/metrics/accuracy.py
+-rw-r--r--  2.0 unx    12549 b- defN 23-Jun-06 11:17 torchrec/metrics/auc.py
+-rw-r--r--  2.0 unx     3703 b- defN 23-Jun-06 11:17 torchrec/metrics/calibration.py
+-rw-r--r--  2.0 unx     3465 b- defN 23-Jun-06 11:17 torchrec/metrics/ctr.py
+-rw-r--r--  2.0 unx     3836 b- defN 23-Jun-06 11:17 torchrec/metrics/mae.py
+-rw-r--r--  2.0 unx    17909 b- defN 23-Jun-06 11:17 torchrec/metrics/metric_module.py
+-rw-r--r--  2.0 unx     6778 b- defN 23-Jun-06 11:17 torchrec/metrics/metrics_config.py
+-rw-r--r--  2.0 unx     3695 b- defN 23-Jun-06 11:17 torchrec/metrics/metrics_namespace.py
+-rw-r--r--  2.0 unx     3904 b- defN 23-Jun-06 11:17 torchrec/metrics/model_utils.py
+-rw-r--r--  2.0 unx     4631 b- defN 23-Jun-06 11:17 torchrec/metrics/mse.py
+-rw-r--r--  2.0 unx     5605 b- defN 23-Jun-06 11:17 torchrec/metrics/multiclass_recall.py
+-rw-r--r--  2.0 unx     6811 b- defN 23-Jun-06 11:17 torchrec/metrics/ne.py
+-rw-r--r--  2.0 unx    31495 b- defN 23-Jun-06 11:17 torchrec/metrics/rec_metric.py
+-rw-r--r--  2.0 unx    10490 b- defN 23-Jun-06 11:17 torchrec/metrics/recall_session.py
+-rw-r--r--  2.0 unx     6057 b- defN 23-Jun-06 11:17 torchrec/metrics/throughput.py
+-rw-r--r--  2.0 unx    10622 b- defN 23-Jun-06 11:17 torchrec/metrics/tower_qps.py
+-rw-r--r--  2.0 unx     2867 b- defN 23-Jun-06 11:17 torchrec/metrics/weighted_avg.py
+-rw-r--r--  2.0 unx    16441 b- defN 23-Jun-06 11:17 torchrec/metrics/test_utils/__init__.py
+-rw-r--r--  2.0 unx      913 b- defN 23-Jun-06 11:17 torchrec/models/__init__.py
+-rw-r--r--  2.0 unx    11410 b- defN 23-Jun-06 11:17 torchrec/models/deepfm.py
+-rw-r--r--  2.0 unx    30000 b- defN 23-Jun-06 11:17 torchrec/models/dlrm.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 11:17 torchrec/models/experimental/__init__.py
+-rw-r--r--  2.0 unx     9825 b- defN 23-Jun-06 11:17 torchrec/models/experimental/test_transformerdlrm.py
+-rw-r--r--  2.0 unx     7434 b- defN 23-Jun-06 11:17 torchrec/models/experimental/transformerdlrm.py
+-rw-r--r--  2.0 unx     1179 b- defN 23-Jun-06 11:17 torchrec/modules/__init__.py
+-rw-r--r--  2.0 unx     1456 b- defN 23-Jun-06 11:17 torchrec/modules/activation.py
+-rw-r--r--  2.0 unx    15163 b- defN 23-Jun-06 11:17 torchrec/modules/crossnet.py
+-rw-r--r--  2.0 unx     8415 b- defN 23-Jun-06 11:17 torchrec/modules/deepfm.py
+-rw-r--r--  2.0 unx     5537 b- defN 23-Jun-06 11:17 torchrec/modules/embedding_configs.py
+-rw-r--r--  2.0 unx    14021 b- defN 23-Jun-06 11:17 torchrec/modules/embedding_modules.py
+-rw-r--r--  2.0 unx     4858 b- defN 23-Jun-06 11:17 torchrec/modules/embedding_tower.py
+-rw-r--r--  2.0 unx    12360 b- defN 23-Jun-06 11:17 torchrec/modules/feature_processor.py
+-rw-r--r--  2.0 unx     2169 b- defN 23-Jun-06 11:17 torchrec/modules/feature_processor_.py
+-rw-r--r--  2.0 unx     4028 b- defN 23-Jun-06 11:17 torchrec/modules/fp_embedding_modules.py
+-rw-r--r--  2.0 unx    31193 b- defN 23-Jun-06 11:17 torchrec/modules/fused_embedding_modules.py
+-rw-r--r--  2.0 unx    10696 b- defN 23-Jun-06 11:17 torchrec/modules/lazy_extension.py
+-rw-r--r--  2.0 unx     6309 b- defN 23-Jun-06 11:17 torchrec/modules/mlp.py
+-rw-r--r--  2.0 unx     4022 b- defN 23-Jun-06 11:17 torchrec/modules/utils.py
+-rw-r--r--  2.0 unx     1639 b- defN 23-Jun-06 11:17 torchrec/optim/__init__.py
+-rw-r--r--  2.0 unx     2012 b- defN 23-Jun-06 11:17 torchrec/optim/apply_optimizer_in_backward.py
+-rw-r--r--  2.0 unx     1569 b- defN 23-Jun-06 11:17 torchrec/optim/clipping.py
+-rw-r--r--  2.0 unx     1353 b- defN 23-Jun-06 11:17 torchrec/optim/fused.py
+-rw-r--r--  2.0 unx    16069 b- defN 23-Jun-06 11:17 torchrec/optim/keyed.py
+-rw-r--r--  2.0 unx     4420 b- defN 23-Jun-06 11:17 torchrec/optim/optimizers.py
+-rw-r--r--  2.0 unx     7405 b- defN 23-Jun-06 11:17 torchrec/optim/rowwise_adagrad.py
+-rw-r--r--  2.0 unx     4865 b- defN 23-Jun-06 11:17 torchrec/optim/warmup.py
+-rw-r--r--  2.0 unx      560 b- defN 23-Jun-06 11:17 torchrec/optim/test_utils/__init__.py
+-rw-r--r--  2.0 unx     1140 b- defN 23-Jun-06 11:17 torchrec/quant/__init__.py
+-rw-r--r--  2.0 unx    22933 b- defN 23-Jun-06 11:17 torchrec/quant/embedding_modules.py
+-rw-r--r--  2.0 unx     4100 b- defN 23-Jun-06 11:17 torchrec/quant/utils.py
+-rw-r--r--  2.0 unx     1163 b- defN 23-Jun-06 11:17 torchrec/sparse/__init__.py
+-rw-r--r--  2.0 unx    55649 b- defN 23-Jun-06 11:17 torchrec/sparse/jagged_tensor.py
+-rw-r--r--  2.0 unx     1430 b- defN 23-Jun-06 11:17 torchrec/sparse/test_utils/__init__.py
+-rw-r--r--  2.0 unx     5661 b- defN 23-Jun-06 11:17 torchrec/test_utils/__init__.py
+-rw-r--r--  2.0 unx     1530 b- defN 23-Jun-06 11:22 torchrec_nightly-2023.6.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5011 b- defN 23-Jun-06 11:22 torchrec_nightly-2023.6.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       93 b- defN 23-Jun-06 11:22 torchrec_nightly-2023.6.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-06 11:22 torchrec_nightly-2023.6.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    13347 b- defN 23-Jun-06 11:22 torchrec_nightly-2023.6.6.dist-info/RECORD
+143 files, 1426608 bytes uncompressed, 329280 bytes compressed:  76.9%
```

## zipnote {}

```diff
@@ -246,14 +246,17 @@
 
 Filename: torchrec/inference/state_dict_transform.py
 Comment: 
 
 Filename: torchrec/metrics/__init__.py
 Comment: 
 
+Filename: torchrec/metrics/accuracy.py
+Comment: 
+
 Filename: torchrec/metrics/auc.py
 Comment: 
 
 Filename: torchrec/metrics/calibration.py
 Comment: 
 
 Filename: torchrec/metrics/ctr.py
@@ -405,23 +408,23 @@
 
 Filename: torchrec/sparse/test_utils/__init__.py
 Comment: 
 
 Filename: torchrec/test_utils/__init__.py
 Comment: 
 
-Filename: torchrec_nightly-2023.6.5.dist-info/LICENSE
+Filename: torchrec_nightly-2023.6.6.dist-info/LICENSE
 Comment: 
 
-Filename: torchrec_nightly-2023.6.5.dist-info/METADATA
+Filename: torchrec_nightly-2023.6.6.dist-info/METADATA
 Comment: 
 
-Filename: torchrec_nightly-2023.6.5.dist-info/WHEEL
+Filename: torchrec_nightly-2023.6.6.dist-info/WHEEL
 Comment: 
 
-Filename: torchrec_nightly-2023.6.5.dist-info/top_level.txt
+Filename: torchrec_nightly-2023.6.6.dist-info/top_level.txt
 Comment: 
 
-Filename: torchrec_nightly-2023.6.5.dist-info/RECORD
+Filename: torchrec_nightly-2023.6.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## torchrec/metrics/metric_module.py

```diff
@@ -12,14 +12,15 @@
 import time
 from typing import Any, Dict, List, Optional, Type, Union
 
 import torch
 import torch.distributed as dist
 import torch.nn as nn
 from torch.profiler import record_function
+from torchrec.metrics.accuracy import AccuracyMetric
 from torchrec.metrics.auc import AUCMetric
 from torchrec.metrics.calibration import CalibrationMetric
 from torchrec.metrics.ctr import CTRMetric
 from torchrec.metrics.mae import MAEMetric
 from torchrec.metrics.metrics_config import (
     MetricsConfig,
     RecMetricEnum,
@@ -52,14 +53,15 @@
     RecMetricEnum.AUC: AUCMetric,
     RecMetricEnum.MSE: MSEMetric,
     RecMetricEnum.MAE: MAEMetric,
     RecMetricEnum.MULTICLASS_RECALL: MulticlassRecallMetric,
     RecMetricEnum.WEIGHTED_AVG: WeightedAvgMetric,
     RecMetricEnum.TOWER_QPS: TowerQPSMetric,
     RecMetricEnum.RECALL_SESSION_LEVEL: RecallSessionMetric,
+    RecMetricEnum.ACCURACY: AccuracyMetric,
 }
 
 
 # Label used for emitting model metrics to the coresponding trainer publishers.
 MODEL_METRIC_LABEL: str = "model"
```

## torchrec/metrics/metrics_config.py

```diff
@@ -24,14 +24,15 @@
     CALIBRATION = "calibration"
     MSE = "mse"
     MAE = "mae"
     MULTICLASS_RECALL = "multiclass_recall"
     RECALL_SESSION_LEVEL = "recall_session_level"
     WEIGHTED_AVG = "weighted_avg"
     TOWER_QPS = "tower_qps"
+    ACCURACY = "accuracy"
 
 
 @dataclass(unsafe_hash=True, eq=True)
 class SessionMetricDef:
     # hyperparameters required for session level metrics
     # session_var_name: name of session tensor in the model_out
     # top_threshold: predictiones ranked in top "top_threshold" are considered as positive
```

## torchrec/metrics/metrics_namespace.py

```diff
@@ -48,14 +48,15 @@
     RMSE = "rmse"
     AUC = "auc"
     GROUPED_AUC = "grouped_auc"
     RECALL_SESSION_LEVEL = "recall_session_level"
     MULTICLASS_RECALL = "multiclass_recall"
     WEIGHTED_AVG = "weighted_avg"
     TOWER_QPS = "qps"
+    ACCURACY = "accuracy"
 
 
 class MetricNamespaceBase(StrValueMixin, Enum):
     pass
 
 
 class MetricNamespace(MetricNamespaceBase):
@@ -64,14 +65,15 @@
     NE = "ne"
     THROUGHPUT = "throughput"
     CTR = "ctr"
     CALIBRATION = "calibration"
     MSE = "mse"
     AUC = "auc"
     MAE = "mae"
+    ACCURACY = "accuracy"
 
     OPTIMIZERS = "optimizers"
     MODEL_CONFIGURATOR = "model_configurator"
 
     MULTICLASS_RECALL = "multiclass_recall"
 
     WEIGHTED_AVG = "weighted_avg"
```

## Comparing `torchrec_nightly-2023.6.5.dist-info/LICENSE` & `torchrec_nightly-2023.6.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `torchrec_nightly-2023.6.5.dist-info/METADATA` & `torchrec_nightly-2023.6.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchrec-nightly
-Version: 2023.6.5
+Version: 2023.6.6
 Summary: Pytorch domain library for recommendation systems
 Home-page: https://github.com/pytorch/torchrec
 Author: TorchRec Team
 Author-email: packages@pytorch.org
 License: BSD-3
 Keywords: pytorch,recommendation systems,sharding
 Classifier: Development Status :: 4 - Beta
```

## Comparing `torchrec_nightly-2023.6.5.dist-info/RECORD` & `torchrec_nightly-2023.6.6.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -78,21 +78,22 @@
 torchrec/fx/utils.py,sha256=N50AfwlUhyS9r1Sv21fSbqRxiOk4KRX0MX9sDjCaQcA,4401
 torchrec/inference/__init__.py,sha256=vi2C_o1Bvsp6hS3_uVZTL7kShgxw5qFZp248Svee2Og,1223
 torchrec/inference/client.py,sha256=jS6ldQxBRY3Bp_LwDLUNSlPt2VYMc-Hsd4iKKoHfDVU,3614
 torchrec/inference/model_packager.py,sha256=HxOEbnqXB2K4uUB9dBBJAL49ZYJME4xTFyVzKjpsjy4,3957
 torchrec/inference/modules.py,sha256=Cx4wYzrc7xG9CmvEb_xCL5sNJ7fqpnQo6G93G-euzw8,8068
 torchrec/inference/state_dict_transform.py,sha256=eFejfFRzU3pL7CmiJtkjq2mpz6Ue_NOUuO2g8-LnLig,3797
 torchrec/metrics/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+torchrec/metrics/accuracy.py,sha256=q5TVzSDBpXHN8YbiAanvwxloGmqmyxr9IBQ2gkQE-g0,4168
 torchrec/metrics/auc.py,sha256=vyUUEJc6Kp1R5kSHBH0t0lI1ZdZzCr0dad6v0aVxJIA,12549
 torchrec/metrics/calibration.py,sha256=hngIvPjcAHusdz1KBrPvwMZX6OkyS0nv18EAmMcyIl0,3703
 torchrec/metrics/ctr.py,sha256=2HY53CX9If6wYcOErvYCT73NH8UdY8oI0UIitoREsMs,3465
 torchrec/metrics/mae.py,sha256=QDPT7l4LCBtTgoxEeEm9vFzCEDtEIlfzs58PtH1oS_U,3836
-torchrec/metrics/metric_module.py,sha256=Zb871gbVS2ymaoslwJIaFbps0tEjDiOiCStoppMj_bA,17812
-torchrec/metrics/metrics_config.py,sha256=ASCrwplAR7ivkgJ5arUrXVjVsU5PY49bfeCvj8_yTk4,6752
-torchrec/metrics/metrics_namespace.py,sha256=nHQCcGJujWcHR8KWDRgGY2yLpKvqtNTAL42o953nPck,3643
+torchrec/metrics/metric_module.py,sha256=8XXa5DJ5eYrS1Pat34_FZ3E9OKUj--8i80nCqXqtJsg,17909
+torchrec/metrics/metrics_config.py,sha256=tL9etUu4FsA_Dr9kUKCf3zIixK6VbIgVi4UoBTZ1GnM,6778
+torchrec/metrics/metrics_namespace.py,sha256=fodij0OglzAGOWNEefuPw0UL1cYfQZAAedCjTErDV6M,3695
 torchrec/metrics/model_utils.py,sha256=WNMsAKK9b5OVPWeuRrNDZ2HjwKuAw3gjNG3OdE99EXw,3904
 torchrec/metrics/mse.py,sha256=tkK3yBV8Uu9Z8Mw_3c1k4kYAhp1jUQkFEJxc0l2LtWU,4631
 torchrec/metrics/multiclass_recall.py,sha256=7NqjkA4IUy4Db90du3hVt8cJxoWS18PBaOourHETkEs,5605
 torchrec/metrics/ne.py,sha256=wXEb9Eh5Mn3D_uuAIaUb3CvJ1eDs06ahVxaWOjR4CtU,6811
 torchrec/metrics/rec_metric.py,sha256=Oq6SRk_TVOXba3qgKbNc7X2ExsiaHNA00J_ZhhkYpHY,31495
 torchrec/metrics/recall_session.py,sha256=24aDBSi8V5XXSnwpqCR5bWcm2CWslBBZ9_a0LQ6VGeg,10490
 torchrec/metrics/throughput.py,sha256=A_WqccFNgu4XpBZzZxnGxAT84Xp2ld43qQM6R1zaqik,6057
@@ -131,12 +132,12 @@
 torchrec/quant/__init__.py,sha256=A6NIA6ztq6iP1JTLRLNzlgnCcd-LaN8efnxGub3Ii4A,1140
 torchrec/quant/embedding_modules.py,sha256=RLuYVywThBXgLEZeHrH2F1sGEA1XydzBg4S9v2rivgY,22933
 torchrec/quant/utils.py,sha256=PkgXn7wnnBIqJ5JAidJMvpAVre1YL8oiYGiPuV_gU2c,4100
 torchrec/sparse/__init__.py,sha256=dLqSye4Jo6obnNNTUKdPDxPQb9sL2U4weemSn-DjpYk,1163
 torchrec/sparse/jagged_tensor.py,sha256=t0QsLwPZ9l2M5by3FpGOPXL6KeSWQqOp7hLayDF-DAc,55649
 torchrec/sparse/test_utils/__init__.py,sha256=BLxfGKJvwjjCiQM64O5wGAA_Cea0sG-buw9lTDWuqug,1430
 torchrec/test_utils/__init__.py,sha256=JncJcXS4N3gI7-fsizQ2-qiWM6MhIrpvskF_9gDf0Go,5661
-torchrec_nightly-2023.6.5.dist-info/LICENSE,sha256=e0Eotbf_rHOYPuEUlppIbvwy4SN98CZnl_hqwvbDA4Q,1530
-torchrec_nightly-2023.6.5.dist-info/METADATA,sha256=LzbsHy4A-iDJWXqqRNSsonhN0uFHyq7RBh8VDyq6wIU,5011
-torchrec_nightly-2023.6.5.dist-info/WHEEL,sha256=ns_9KNZvwSNZtRgVV_clzMUG_fXjGc5Z8Tx4hxQ0gkw,93
-torchrec_nightly-2023.6.5.dist-info/top_level.txt,sha256=LoLcTAPLj_7x62AuyYmhEVBcx2WJ1Z1Nrknv0Jnk_gQ,9
-torchrec_nightly-2023.6.5.dist-info/RECORD,,
+torchrec_nightly-2023.6.6.dist-info/LICENSE,sha256=e0Eotbf_rHOYPuEUlppIbvwy4SN98CZnl_hqwvbDA4Q,1530
+torchrec_nightly-2023.6.6.dist-info/METADATA,sha256=j0WSpgxT6SFi9zD9rG6uFARAN2tnX4AD0xaOYHbUwH8,5011
+torchrec_nightly-2023.6.6.dist-info/WHEEL,sha256=ns_9KNZvwSNZtRgVV_clzMUG_fXjGc5Z8Tx4hxQ0gkw,93
+torchrec_nightly-2023.6.6.dist-info/top_level.txt,sha256=LoLcTAPLj_7x62AuyYmhEVBcx2WJ1Z1Nrknv0Jnk_gQ,9
+torchrec_nightly-2023.6.6.dist-info/RECORD,,
```

