# Comparing `tmp/Simba-UW-tf-dev-1.62.7.tar.gz` & `tmp/Simba-UW-tf-dev-1.62.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Simba-UW-tf-dev-1.62.7.tar", last modified: Mon Jun  5 19:40:44 2023, max compression
+gzip compressed data, was "dist/Simba-UW-tf-dev-1.62.8.tar", last modified: Wed Jun  7 20:12:49 2023, max compression
```

## Comparing `Simba-UW-tf-dev-1.62.7.tar` & `Simba-UW-tf-dev-1.62.8.tar`

### file list

```diff
@@ -1,519 +1,520 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/PKG-INFO
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/ui/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-30 12:37:26.000000 Simba-UW-tf-dev-1.62.7/simba/ui/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/
--rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/csv_2_parquet_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2343 2023-05-17 20:47:45.000000 Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/quick_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/batch_preprocess_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8342 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/heatmap_location_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/clf_probability_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-23 15:42:32.000000 Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/movement_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     9471 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/clf_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    15950 2023-05-20 12:10:35.000000 Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1150 2023-05-25 18:21:39.000000 Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/remove_roi_features_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4798 2023-04-29 18:54:24.000000 Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/roi_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5977 2023-05-31 12:58:14.000000 Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/outlier_settings_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/gantt_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/clf_validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7721 2023-05-24 15:18:33.000000 Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/severity_analysis_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/fsttc_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4052 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/kleinberg_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7288 2023-05-29 20:14:50.000000 Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5425 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/pose_reorganizer_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/clf_by_timebins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8673 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/heatmap_clf_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/data_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7860 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/roi_features_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/pup_retrieval_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/about_simba_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3605 2023-05-25 18:54:56.000000 Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     6353 2023-05-24 15:31:12.000000 Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    42478 2023-04-29 18:56:08.000000 Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/video_processing_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     7535 2023-05-15 13:09:04.000000 Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/validation_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/clf_by_roi_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/make_path_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/archive_files_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     4087 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/pose_bp_drop_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    10695 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/distance_plot_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     2567 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
--rw-r--r--   0 simon      (501) staff       (20)    12869 2023-05-23 12:47:59.000000 Simba-UW-tf-dev-1.62.7/simba/ui/video_info_ui.py
--rw-r--r--   0 simon      (501) staff       (20)     6019 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.62.7/simba/ui/user_defined_pose_creator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/ui/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    12602 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.62.7/simba/ui/create_project_ui.py
--rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.62.7/simba/ui/tkinter_functions.py
--rw-r--r--   0 simon      (501) staff       (20)    35432 2023-06-05 18:05:35.000000 Simba-UW-tf-dev-1.62.7/simba/ui/machine_model_settings_ui.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/blob_storage/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.62.7/simba/blob_storage/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/labelling/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 13:50:26.000000 Simba-UW-tf-dev-1.62.7/simba/labelling/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/labelling/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    20743 2023-05-14 23:21:08.000000 Simba-UW-tf-dev-1.62.7/simba/labelling/labelling_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     3568 2023-05-19 11:18:49.000000 Simba-UW-tf-dev-1.62.7/simba/labelling/extract_labelled_frames.py
--rw-r--r--   0 simon      (501) staff       (20)    26931 2023-05-24 17:01:48.000000 Simba-UW-tf-dev-1.62.7/simba/labelling/labelling_advanced_interface.py
--rw-r--r--   0 simon      (501) staff       (20)     6629 2023-05-13 17:45:08.000000 Simba-UW-tf-dev-1.62.7/simba/labelling/play_annotation_video.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)    11877 2023-05-17 14:59:39.000000 Simba-UW-tf-dev-1.62.7/simba/unsupervised/dbcv_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.62.7/simba/unsupervised/enums.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:15:51.000000 Simba-UW-tf-dev-1.62.7/simba/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     8141 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.62.7/simba/unsupervised/dataset_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     5636 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.62.7/simba/unsupervised/grid_search_visualizers.py
--rw-r--r--   0 simon      (501) staff       (20)     7310 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.62.7/simba/unsupervised/data_extractor.py
--rw-r--r--   0 simon      (501) staff       (20)     9848 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.62.7/simba/unsupervised/ui.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/unsupervised/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     9851 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.62.7/simba/unsupervised/umap_embedder.py
--rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.62.7/simba/unsupervised/pop_up_classes.py
--rw-r--r--   0 simon      (501) staff       (20)     2931 2023-05-17 14:54:38.000000 Simba-UW-tf-dev-1.62.7/simba/unsupervised/bout_aggregator.py
--rw-r--r--   0 simon      (501) staff       (20)    20846 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.62.7/simba/unsupervised/cluster_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.62.7/simba/unsupervised/data_map.yaml
--rw-r--r--   0 simon      (501) staff       (20)    10288 2023-05-17 15:07:44.000000 Simba-UW-tf-dev-1.62.7/simba/unsupervised/hdbscan_clusterer.py
--rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.62.7/simba/unsupervised/tsne.py
--rw-r--r--   0 simon      (501) staff       (20)     6656 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.62.7/simba/unsupervised/cluster_visualizer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/bounding_box_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.62.7/simba/bounding_box_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/bounding_box_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7031 2023-05-14 18:13:04.000000 Simba-UW-tf-dev-1.62.7/simba/bounding_box_tools/agg_boundary_stats.py
--rw-r--r--   0 simon      (501) staff       (20)    23566 2023-05-14 18:29:41.000000 Simba-UW-tf-dev-1.62.7/simba/bounding_box_tools/boundary_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     8497 2023-05-14 18:22:39.000000 Simba-UW-tf-dev-1.62.7/simba/bounding_box_tools/boundary_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)     6376 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.62.7/simba/bounding_box_tools/find_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    11381 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.62.7/simba/bounding_box_tools/visualize_boundaries.py
--rw-r--r--   0 simon      (501) staff       (20)    49156 2023-06-05 16:31:18.000000 Simba-UW-tf-dev-1.62.7/simba/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/
--rw-r--r--   0 simon      (501) staff       (20)    42512 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/feature_extractor_14bp.py
--rw-r--r--   0 simon      (501) staff       (20)    21482 2023-05-14 23:55:56.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/feature_extractor_7bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/
--rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/doctests.py
--rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
--rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/read_in_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/peaks.py
--rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/fish_feature_extractor_2022.py
--rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
--rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/convex_hull_scratch_1.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
--rw-r--r--   0 simon      (501) staff       (20)     7127 2023-05-28 19:41:35.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/egocentrical_aligner.py
--rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/count_values_in_range.py
--rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/graph_creator.py
--rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/termite_rois.csv
--rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/mutual_exclusive.py
--rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/video_color.py
--rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/graph_3d_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     8943 2023-06-05 18:15:28.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/shap_log_mp_2.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/video_rotator.py
--rw-r--r--   0 simon      (501) staff       (20)     8580 2023-05-31 20:02:32.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/shap_log_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/add_probability_cnt_features.py
--rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/make_splash.py
--rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:46:44.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
--rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/time_stamp_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/video_rotator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     4279 2023-06-01 12:49:14.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/read_files_mp_2.py
--rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:44:29.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
--rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/convex_hull_scratch_2.py
--rw-r--r--   0 simon      (501) staff       (20)    27995 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/feature_extractor_8bps_2_animals.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-05-19 20:03:28.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3864 2023-05-19 19:41:40.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/perimeter_jit.py
--rw-r--r--   0 simon      (501) staff       (20)    13579 2023-05-14 19:53:33.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/feature_subsets.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8244 2023-05-21 16:28:49.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/feature_extractor_user_defined.py
--rw-r--r--   0 simon      (501) staff       (20)    46461 2023-05-15 00:03:36.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/feature_extractor_16bp.py
--rw-r--r--   0 simon      (501) staff       (20)    28259 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/feature_extractor_9bp.py
--rw-r--r--   0 simon      (501) staff       (20)    23976 2023-05-15 00:01:21.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/feature_extractor_8bp.py
--rw-r--r--   0 simon      (501) staff       (20)    16880 2023-05-14 23:53:59.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/feature_extractor_4bp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/.idea/features_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/.idea/.gitignore
--rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/.idea/.name
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/feature_extractors/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    15434 2023-05-20 18:29:53.000000 Simba-UW-tf-dev-1.62.7/simba/requirements.txt
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/mixins/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.62.7/simba/mixins/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43029 2023-06-05 17:40:09.000000 Simba-UW-tf-dev-1.62.7/simba/mixins/pop_up_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    33507 2023-05-25 18:37:00.000000 Simba-UW-tf-dev-1.62.7/simba/mixins/config_reader.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/mixins/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18616 2023-05-17 19:39:33.000000 Simba-UW-tf-dev-1.62.7/simba/mixins/pose_importer_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/mixins/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-06-01 18:12:36.000000 Simba-UW-tf-dev-1.62.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.62.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)     2090 2023-06-01 14:35:51.000000 Simba-UW-tf-dev-1.62.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi
--rw-r--r--   0 simon      (501) staff       (20)    82442 2023-06-01 18:12:36.000000 Simba-UW-tf-dev-1.62.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    51809 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.62.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    14391 2023-06-01 14:35:51.000000 Simba-UW-tf-dev-1.62.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc
--rw-r--r--   0 simon      (501) staff       (20)    14188 2023-05-21 00:18:56.000000 Simba-UW-tf-dev-1.62.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc
--rw-r--r--   0 simon      (501) staff       (20)    37135 2023-06-02 12:12:15.000000 Simba-UW-tf-dev-1.62.7/simba/mixins/feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    61873 2023-05-19 21:14:46.000000 Simba-UW-tf-dev-1.62.7/simba/mixins/plotting_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     9144 2023-05-28 17:30:45.000000 Simba-UW-tf-dev-1.62.7/simba/mixins/unsupervised_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)    73513 2023-06-05 19:37:03.000000 Simba-UW-tf-dev-1.62.7/simba/mixins/train_model_mixin.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/third_party_label_appenders/
--rw-r--r--   0 simon      (501) staff       (20)     6094 2023-05-21 17:39:19.000000 Simba-UW-tf-dev-1.62.7/simba/third_party_label_appenders/deepethogram_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    10623 2023-05-21 18:42:05.000000 Simba-UW-tf-dev-1.62.7/simba/third_party_label_appenders/BORIS_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8998 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.62.7/simba/third_party_label_appenders/observer_importer.py
--rw-r--r--   0 simon      (501) staff       (20)    17954 2023-05-21 15:57:11.000000 Simba-UW-tf-dev-1.62.7/simba/third_party_label_appenders/tools.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.62.7/simba/third_party_label_appenders/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    18514 2023-05-29 20:20:16.000000 Simba-UW-tf-dev-1.62.7/simba/third_party_label_appenders/third_party_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     8181 2023-05-21 17:19:25.000000 Simba-UW-tf-dev-1.62.7/simba/third_party_label_appenders/ethovision_import.py
--rw-r--r--   0 simon      (501) staff       (20)     6988 2023-05-21 17:31:04.000000 Simba-UW-tf-dev-1.62.7/simba/third_party_label_appenders/BENTO_appender.py
--rw-r--r--   0 simon      (501) staff       (20)     5239 2023-05-21 18:07:18.000000 Simba-UW-tf-dev-1.62.7/simba/third_party_label_appenders/solomon_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/cue_light_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:06:55.000000 Simba-UW-tf-dev-1.62.7/simba/cue_light_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7652 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.62.7/simba/cue_light_tools/cue_light_clf_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)    12207 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.62.7/simba/cue_light_tools/cue_light_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    16690 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.62.7/simba/cue_light_tools/cue_light_menues.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/cue_light_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     1879 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.62.7/simba/cue_light_tools/cue_light_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    15212 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.62.7/simba/cue_light_tools/cue_light_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12650 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.62.7/simba/cue_light_tools/cue_light_movement_statistics.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/utils/
--rw-r--r--   0 simon      (501) staff       (20)    11899 2023-05-15 12:44:10.000000 Simba-UW-tf-dev-1.62.7/simba/utils/config_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    21017 2023-06-05 18:05:35.000000 Simba-UW-tf-dev-1.62.7/simba/utils/enums.py
--rw-r--r--   0 simon      (501) staff       (20)    10244 2023-06-05 17:20:50.000000 Simba-UW-tf-dev-1.62.7/simba/utils/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7396 2023-06-01 13:09:55.000000 Simba-UW-tf-dev-1.62.7/simba/utils/warnings.py
--rw-r--r--   0 simon      (501) staff       (20)     8807 2023-05-25 13:24:45.000000 Simba-UW-tf-dev-1.62.7/simba/utils/checks.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/utils/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    43061 2023-05-25 14:56:03.000000 Simba-UW-tf-dev-1.62.7/simba/utils/read_write.py
--rw-r--r--   0 simon      (501) staff       (20)     8585 2023-06-05 17:07:45.000000 Simba-UW-tf-dev-1.62.7/simba/utils/lookups.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/utils/cli/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/utils/cli/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6017 2023-05-28 13:41:20.000000 Simba-UW-tf-dev-1.62.7/simba/utils/cli/cli_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    14666 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.62.7/simba/utils/errors.py
--rw-r--r--   0 simon      (501) staff       (20)    17829 2023-05-25 17:48:38.000000 Simba-UW-tf-dev-1.62.7/simba/utils/data.py
--rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.62.7/simba/utils/printing.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/pose_processors/
--rw-r--r--   0 simon      (501) staff       (20)     8256 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.62.7/simba/pose_processors/reorganize_keypoint.py
--rw-r--r--   0 simon      (501) staff       (20)     5167 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.62.7/simba/pose_processors/remove_keypoints.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/pose_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     2656 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.62.7/simba/pose_processors/pose_reset.py
--rw-r--r--   0 simon      (501) staff       (20)     5614 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.62.7/simba/pose_processors/reverse_pose.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/plotting/
--rw-r--r--   0 simon      (501) staff       (20)     9114 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.62.7/simba/plotting/gantt_creator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/plotting/tools/
--rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.62.7/simba/plotting/tools/tkinter_tools.py
--rw-r--r--   0 simon      (501) staff       (20)    13008 2023-05-24 15:32:44.000000 Simba-UW-tf-dev-1.62.7/simba/plotting/ROI_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 23:35:57.000000 Simba-UW-tf-dev-1.62.7/simba/plotting/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    14568 2023-05-15 18:41:17.000000 Simba-UW-tf-dev-1.62.7/simba/plotting/shap_agg_stats_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    10105 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.62.7/simba/plotting/gantt_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15730 2023-05-15 17:49:01.000000 Simba-UW-tf-dev-1.62.7/simba/plotting/heat_mapper_clf_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8731 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.62.7/simba/plotting/probability_plot_creator.py
--rw-r--r--   0 simon      (501) staff       (20)    12484 2023-05-23 14:52:24.000000 Simba-UW-tf-dev-1.62.7/simba/plotting/plot_clf_results.py
--rw-r--r--   0 simon      (501) staff       (20)    14056 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.62.7/simba/plotting/plot_clf_results_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    16031 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.62.7/simba/plotting/ROI_feature_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    12770 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.62.7/simba/plotting/heat_mapper_location.py
--rw-r--r--   0 simon      (501) staff       (20)    10100 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.62.7/simba/plotting/probability_plot_creator_mp.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/plotting/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     4881 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.62.7/simba/plotting/interactive_probability_grapher.py
--rw-r--r--   0 simon      (501) staff       (20)     5812 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.62.7/simba/plotting/plot_pose_in_dir.py
--rw-r--r--   0 simon      (501) staff       (20)    14029 2023-06-04 11:55:47.000000 Simba-UW-tf-dev-1.62.7/simba/plotting/single_run_model_validation_video.py
--rw-r--r--   0 simon      (501) staff       (20)    12790 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.62.7/simba/plotting/frame_mergerer_ffmpeg.py
--rw-r--r--   0 simon      (501) staff       (20)     7891 2023-05-29 21:41:05.000000 Simba-UW-tf-dev-1.62.7/simba/plotting/Directing_animals_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11219 2023-05-17 12:58:17.000000 Simba-UW-tf-dev-1.62.7/simba/plotting/clf_validator.py
--rw-r--r--   0 simon      (501) staff       (20)    15745 2023-05-20 12:16:06.000000 Simba-UW-tf-dev-1.62.7/simba/plotting/path_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    11203 2023-05-24 15:35:24.000000 Simba-UW-tf-dev-1.62.7/simba/plotting/ROI_feature_visualizer_mp.py
--rw-r--r--   0 simon      (501) staff       (20)     8933 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.62.7/simba/plotting/data_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13471 2023-05-20 12:15:46.000000 Simba-UW-tf-dev-1.62.7/simba/plotting/path_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     6494 2023-05-17 20:55:17.000000 Simba-UW-tf-dev-1.62.7/simba/plotting/ez_lineplot.py
--rw-r--r--   0 simon      (501) staff       (20)    11519 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.62.7/simba/plotting/distance_plotter_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    15794 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.62.7/simba/plotting/ROI_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)    13163 2023-05-16 16:42:03.000000 Simba-UW-tf-dev-1.62.7/simba/plotting/heat_mapper_clf.py
--rw-r--r--   0 simon      (501) staff       (20)     9385 2023-05-31 16:46:49.000000 Simba-UW-tf-dev-1.62.7/simba/plotting/distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     9526 2023-06-04 12:03:25.000000 Simba-UW-tf-dev-1.62.7/simba/plotting/single_run_model_validation_video_mp.py
--rw-r--r--   0 simon      (501) staff       (20)    10005 2023-05-29 21:36:37.000000 Simba-UW-tf-dev-1.62.7/simba/plotting/Directing_animals_visualizer.py
--rw-r--r--   0 simon      (501) staff       (20)    16320 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.62.7/simba/plotting/heat_mapper_location_mp.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/dash_app/
--rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/dash_app/SimBA_dash_app.py
--rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/dash_app/run_dash_tkinter.py
--rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/dash_app/dash_app.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/data_processors/
--rw-r--r--   0 simon      (501) staff       (20)     7248 2023-05-25 19:01:00.000000 Simba-UW-tf-dev-1.62.7/simba/data_processors/agg_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    11196 2023-05-28 19:50:35.000000 Simba-UW-tf-dev-1.62.7/simba/data_processors/severity_bout_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16259 2023-05-24 20:39:01.000000 Simba-UW-tf-dev-1.62.7/simba/data_processors/interpolation_smoothing.py
--rw-r--r--   0 simon      (501) staff       (20)     8127 2023-05-25 13:57:19.000000 Simba-UW-tf-dev-1.62.7/simba/data_processors/timebins_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    12938 2023-05-23 20:14:45.000000 Simba-UW-tf-dev-1.62.7/simba/data_processors/fsttc_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/data_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6306 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.62.7/simba/data_processors/interpolate_pose.py
--rw-r--r--   0 simon      (501) staff       (20)     9646 2023-05-14 19:19:14.000000 Simba-UW-tf-dev-1.62.7/simba/data_processors/directing_other_animals_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8624 2023-05-25 14:07:56.000000 Simba-UW-tf-dev-1.62.7/simba/data_processors/timebins_movement_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     4799 2023-05-17 17:23:16.000000 Simba-UW-tf-dev-1.62.7/simba/data_processors/severity_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    16980 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.62.7/simba/data_processors/pup_retrieval_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-13 17:23:00.000000 Simba-UW-tf-dev-1.62.7/simba/data_processors/pybursts_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    11533 2023-05-28 19:50:34.000000 Simba-UW-tf-dev-1.62.7/simba/data_processors/severity_frame_based_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     9656 2023-05-25 13:32:25.000000 Simba-UW-tf-dev-1.62.7/simba/data_processors/kleinberg_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     8131 2023-05-25 14:37:36.000000 Simba-UW-tf-dev-1.62.7/simba/data_processors/movement_calculator.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations_archive/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations_archive/pose_configurations_archive_1/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/model/
--rw-r--r--   0 simon      (501) staff       (20)    20128 2023-06-05 18:11:07.000000 Simba-UW-tf-dev-1.62.7/simba/model/train_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:06:50.000000 Simba-UW-tf-dev-1.62.7/simba/model/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     3315 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.62.7/simba/model/inference_batch.py
--rw-r--r--   0 simon      (501) staff       (20)    20849 2023-06-05 18:44:40.000000 Simba-UW-tf-dev-1.62.7/simba/model/grid_search_rf.py
--rw-r--r--   0 simon      (501) staff       (20)     3363 2023-05-19 11:12:45.000000 Simba-UW-tf-dev-1.62.7/simba/model/inference_validation.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/roi_tools/
--rw-r--r--   0 simon      (501) staff       (20)     5858 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.62.7/simba/roi_tools/ROI_time_bin_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)     1687 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.62.7/simba/roi_tools/ROI_movement_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.62.7/simba/roi_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    43119 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.62.7/simba/roi_tools/ROI_define.py
--rw-r--r--   0 simon      (501) staff       (20)     4024 2023-05-16 13:21:43.000000 Simba-UW-tf-dev-1.62.7/simba/roi_tools/ROI_reset.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/roi_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    19901 2023-05-15 17:00:34.000000 Simba-UW-tf-dev-1.62.7/simba/roi_tools/ROI_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    11608 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.62.7/simba/roi_tools/ROI_feature_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.62.7/simba/roi_tools/ROI_multiply.py
--rw-r--r--   0 simon      (501) staff       (20)      959 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.62.7/simba/roi_tools/ROI_size_calculations.py
--rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/roi_tools/ROI_zoom.py
--rw-r--r--   0 simon      (501) staff       (20)    11556 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.62.7/simba/roi_tools/ROI_directing_analyzer.py
--rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/roi_tools/ROI_move_shape.py
--rw-r--r--   0 simon      (501) staff       (20)     5079 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.62.7/simba/roi_tools/ROI_menus.py
--rw-r--r--   0 simon      (501) staff       (20)    13742 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.62.7/simba/roi_tools/ROI_clf_calculator.py
--rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.62.7/simba/roi_tools/ROI_image.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/pose_importers/
--rw-r--r--   0 simon      (501) staff       (20)     8115 2023-05-14 18:03:14.000000 Simba-UW-tf-dev-1.62.7/simba/pose_importers/sleap_csv_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/pose_importers/misc/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.62.7/simba/pose_importers/misc/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.62.7/simba/pose_importers/misc/apt_trk_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.62.7/simba/pose_importers/read_DANNCE_mat.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:45:51.000000 Simba-UW-tf-dev-1.62.7/simba/pose_importers/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)    12549 2023-05-17 20:32:56.000000 Simba-UW-tf-dev-1.62.7/simba/pose_importers/sleap_h5_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7322 2023-05-16 16:55:05.000000 Simba-UW-tf-dev-1.62.7/simba/pose_importers/madlc_importer.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/pose_importers/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)    12141 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.62.7/simba/pose_importers/sleap_slp_importer.py
--rw-r--r--   0 simon      (501) staff       (20)     7931 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.62.7/simba/pose_importers/import_mars.py
--rw-r--r--   0 simon      (501) staff       (20)     6978 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.62.7/simba/pose_importers/dlc_importer_csv.py
--rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.62.7/simba/pose_importers/trk_importer.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations/
--rw-r--r--   0 simon      (501) staff       (20)    14340 2023-05-14 23:57:00.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations/bp_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations/bp_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations/bp_names/bp_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations/no_animals/
--rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations/no_animals/no_animals.csv
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations/no_animals/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations/configuration_names/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations/configuration_names/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations/configuration_names/pose_config_names.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations/schematics/
--rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations/schematics/8.png
--rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations/schematics/9.png
--rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations/schematics/12.png
--rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations/schematics/11.png
--rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations/schematics/10.png
--rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations/schematics/4.png
--rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations/schematics/5.png
--rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations/schematics/7.png
--rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations/schematics/6.png
--rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations/schematics/2.png
--rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations/schematics/3.png
--rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/pose_configurations/schematics/1.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/video_processors/
--rw-r--r--   0 simon      (501) staff       (20)    45564 2023-05-14 17:15:40.000000 Simba-UW-tf-dev-1.62.7/simba/video_processors/video_processing.py
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-20 18:15:51.000000 Simba-UW-tf-dev-1.62.7/simba/video_processors/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.62.7/simba/video_processors/px_to_mm.py
--rw-r--r--   0 simon      (501) staff       (20)    24648 2023-05-16 16:42:04.000000 Simba-UW-tf-dev-1.62.7/simba/video_processors/batch_process_menus.py
--rw-r--r--   0 simon      (501) staff       (20)     7333 2023-05-16 12:54:28.000000 Simba-UW-tf-dev-1.62.7/simba/video_processors/multi_cropper.py
--rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.62.7/simba/video_processors/extract_frames.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/video_processors/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.62.7/simba/video_processors/calculate_px_dist.py
--rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.62.7/simba/video_processors/extract_seqframes.py
--rw-r--r--   0 simon      (501) staff       (20)    11087 2023-05-14 16:24:59.000000 Simba-UW-tf-dev-1.62.7/simba/video_processors/batch_process_create_ffmpeg_commands.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/outlier_tools/
--rw-r--r--   0 simon      (501) staff       (20)     6535 2023-05-25 14:24:01.000000 Simba-UW-tf-dev-1.62.7/simba/outlier_tools/outlier_corrector_movement.py
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-08 20:25:20.000000 Simba-UW-tf-dev-1.62.7/simba/outlier_tools/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/outlier_tools/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     8168 2023-06-01 12:38:34.000000 Simba-UW-tf-dev-1.62.7/simba/outlier_tools/outlier_corrector_location.py
--rw-r--r--   0 simon      (501) staff       (20)     2668 2023-05-25 14:26:49.000000 Simba-UW-tf-dev-1.62.7/simba/outlier_tools/skip_outlier_correction.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/outlier_tools/.idea/
--rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/outlier_tools/.idea/outlier_scripts.iml
--rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/outlier_tools/.idea/encodings.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/outlier_tools/.idea/inspectionProfiles/
--rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/outlier_tools/.idea/libraries/
--rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/outlier_tools/.idea/libraries/R_User_Library.xml
--rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/outlier_tools/.idea/workspace.xml
--rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/outlier_tools/.idea/modules.xml
--rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/outlier_tools/.idea/misc.xml
--rw-r--r--   0 simon      (501) staff       (20)    65549 2023-05-25 18:24:18.000000 Simba-UW-tf-dev-1.62.7/simba/SimBA.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/assets/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/assets/unsupervised/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/assets/unsupervised/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/assets/unsupervised/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/assets/unsupervised/features.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/assets/shap/
--rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/assets/shap/down_arrow.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/assets/shap/intruder_shape.jpg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/assets/shap/feature_categories/
--rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
--rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/assets/shap/feature_categories/shap_feature_categories.csv
--rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.62.7/simba/assets/shap/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/assets/shap/resident_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/assets/shap/resident_intruder_shape.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/assets/shap/animal_distances.jpg
--rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/assets/shap/baseline_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/assets/shap/ubuntu.regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/assets/shap/side_scale.jpg
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/assets/shap/UbuntuMono-Regular.ttf
--rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/assets/shap/side_scale_5.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/assets/shap/intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/assets/shap/resident_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/assets/shap/color_bar.jpg
--rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/assets/shap/resident_intruder_movement.jpg
--rw-r--r--   0 simon      (501) staff       (20)    16388 2023-05-15 20:24:40.000000 Simba-UW-tf-dev-1.62.7/simba/assets/.DS_Store
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/assets/lookups/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/assets/lookups/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/assets/lookups/model_names.parquet
--rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.62.7/simba/assets/lookups/feature_extraction_headers.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/assets/lookups/features.csv
--rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/assets/lookups/unsupervised_example_x.csv
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/assets/stl/
--rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/assets/stl/operant_tray.stl
--rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/assets/stl/operant_lever.stl
--rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/assets/stl/operant_walls.stl
--rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/assets/stl/grid_floor.stl
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/assets/img/
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.62.7/simba/assets/img/.DS_Store
--rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/assets/img/about_me.png
--rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.62.7/simba/assets/img/splash.mp4
--rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.62.7/simba/assets/img/bg_2.png
--rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/assets/img/splash.pptx
--rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.62.7/simba/assets/img/bg.png
--rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/assets/UbuntuMono-Regular.ttf
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/
--rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/factory.png
--rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/cluster.png
--rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/load.png
--rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/gif.png
--rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/pose.png
--rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/features.png
--rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/.DS_Store
--rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/settings.png
--rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/stopwatch.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/link.png
--rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/dash_simba.css
--rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/documentation.png
--rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/fps.png
--rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/dimensionality_reduction.png
--rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/roi.png
--rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/superimpose.png
--rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/label.png
--rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/change.png
--rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/crop.png
--rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/rotate.png
--rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/path.png
--rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/clip.png
--rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/restart.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/calipher.png
--rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/add_on.png
--rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/create.png
--rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/SimBA_logo.ico
--rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/print.png
--rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/clf.png
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/concat_icons/
--rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/concat_icons/mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/concat_icons/vertical.png
--rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/concat_icons/horizontal.png
--rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/concat_icons/mixed_mosaic.png
--rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/merge.png
--rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/clean.png
--rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/clf_2.png
--rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/visualize.png
--rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/concat.png
--rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/boris.png
--rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/frames.png
--rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/video.png
--rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/sample.png
--rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/metrics.png
--rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/grey.png
--rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/exit.png
--rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/outlier.png
--rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/clahe.png
--rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/trash.png
--rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/about.png
--rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/convert.png
--rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/SimBA_logo.icns
--rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/reorganize.png
--rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/browse.png
--rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/SimBA_logo.png
--rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/ethovision.png
--rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.62.7/simba/assets/icons/close.png
--rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/assets/dash_simba_base.css
--rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.7/simba/assets/TheGoldenLab.PNG
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/Simba_UW_tf_dev.egg-info/
--rw-rw-r--   0 simon      (501) staff       (20)      579 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/Simba_UW_tf_dev.egg-info/PKG-INFO
--rw-rw-r--   0 simon      (501) staff       (20)    19265 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/Simba_UW_tf_dev.egg-info/SOURCES.txt
--rw-rw-r--   0 simon      (501) staff       (20)       44 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/Simba_UW_tf_dev.egg-info/entry_points.txt
--rw-rw-r--   0 simon      (501) staff       (20)      639 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/Simba_UW_tf_dev.egg-info/requires.txt
--rw-rw-r--   0 simon      (501) staff       (20)       12 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/Simba_UW_tf_dev.egg-info/top_level.txt
--rw-rw-r--   0 simon      (501) staff       (20)        1 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/Simba_UW_tf_dev.egg-info/dependency_links.txt
--rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.62.7/LICENSE.md
--rw-r--r--   0 simon      (501) staff       (20)       89 2023-05-20 17:55:56.000000 Simba-UW-tf-dev-1.62.7/pyproject.toml
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/tests/
--rw-r--r--   0 simon      (501) staff       (20)     5209 2023-05-28 14:15:24.000000 Simba-UW-tf-dev-1.62.7/tests/test_data_processors.py
--rw-r--r--   0 simon      (501) staff       (20)     5317 2023-05-31 19:40:16.000000 Simba-UW-tf-dev-1.62.7/tests/test_distance_plotter.py
--rw-r--r--   0 simon      (501) staff       (20)     3134 2023-06-04 19:21:28.000000 Simba-UW-tf-dev-1.62.7/tests/test_train_model_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.7/tests/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     6757 2023-06-02 12:11:53.000000 Simba-UW-tf-dev-1.62.7/tests/test_feature_extraction_mixin.py
--rw-r--r--   0 simon      (501) staff       (20)     1528 2023-05-25 14:26:19.000000 Simba-UW-tf-dev-1.62.7/tests/test_outlier_correctors.py
--rw-r--r--   0 simon      (501) staff       (20)     4356 2023-05-29 20:59:49.000000 Simba-UW-tf-dev-1.62.7/tests/test_visualize_directing_animals.py
--rw-r--r--   0 simon      (501) staff       (20)     1859 2023-05-21 16:40:19.000000 Simba-UW-tf-dev-1.62.7/tests/test_featurizers.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/tests/data/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.7/tests/data/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/tests/data/test_projects/
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/tests/data/test_projects/two_c57/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.7/tests/data/test_projects/two_c57/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/tests/data/test_projects/two_c57/models/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.7/tests/data/test_projects/two_c57/models/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.7/tests/data/test_projects/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/tests/data/test_projects/mouse_open_field/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.7/tests/data/test_projects/mouse_open_field/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/tests/data/test_projects/zebrafish/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.7/tests/data/test_projects/zebrafish/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/tests/data/test_projects/zebrafish/feature_file/
--rw-rw-r--   0 simon      (501) staff       (20)        0 2020-08-11 16:11:18.000000 Simba-UW-tf-dev-1.62.7/tests/data/test_projects/zebrafish/feature_file/__init__.py
--rw-rw-r--   0 simon      (501) staff       (20)    14128 2022-04-11 08:07:36.000000 Simba-UW-tf-dev-1.62.7/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py
--rw-r--r--   0 simon      (501) staff       (20)     3971 2023-05-28 17:20:18.000000 Simba-UW-tf-dev-1.62.7/tests/test_thirdparty_appenders.py
--rw-r--r--   0 simon      (501) staff       (20)     3090 2023-05-31 15:49:24.000000 Simba-UW-tf-dev-1.62.7/tests/test_validation_clips.py
--rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.62.7/MANIFEST.in
--rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.62.7/README.md
--rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-06-05 19:34:42.000000 Simba-UW-tf-dev-1.62.7/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-06-05 19:40:44.000000 Simba-UW-tf-dev-1.62.7/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/PKG-INFO
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/ui/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-30 12:37:26.000000 Simba-UW-tf-dev-1.62.8/simba/ui/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/
+-rw-r--r--   0 simon      (501) staff       (20)     3463 2023-05-04 17:49:06.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1431 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/csv_2_parquet_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2343 2023-05-17 20:47:45.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/quick_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2332 2023-04-29 18:13:54.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/batch_preprocess_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8342 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/heatmap_location_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9302 2023-05-04 15:16:51.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/clf_probability_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-23 15:42:32.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-03 16:24:11.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/movement_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3657 2023-04-29 19:37:54.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     9471 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/clf_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    15950 2023-05-20 12:10:35.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1150 2023-05-25 18:21:39.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/remove_roi_features_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3024 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/smoothing_interpolation_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4798 2023-04-29 18:54:24.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3551 2023-05-03 16:20:49.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/roi_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5977 2023-05-31 12:58:14.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/outlier_settings_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8296 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/gantt_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5726 2023-05-01 12:04:35.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/clf_validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7721 2023-05-24 15:18:33.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/severity_analysis_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2779 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/fsttc_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4052 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/kleinberg_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7288 2023-05-29 20:14:50.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5425 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/pose_reorganizer_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2411 2023-05-03 16:35:10.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/append_roi_features_animals_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3251 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/clf_by_timebins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8673 2023-05-14 15:52:16.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/heatmap_clf_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7688 2023-04-29 15:00:50.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/data_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7860 2023-05-14 16:01:44.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/roi_features_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     8363 2023-04-29 19:49:16.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/pup_retrieval_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)      579 2023-04-29 18:12:37.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/about_simba_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3605 2023-05-25 18:54:56.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     6353 2023-05-24 15:31:12.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/roi_tracking_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1468 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5318 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/clf_add_remove_print_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    42478 2023-04-29 18:56:08.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/video_processing_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     7535 2023-05-15 13:09:04.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/validation_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5255 2023-05-04 18:22:44.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/clf_by_roi_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2840 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/make_path_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     5406 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     1065 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/archive_files_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     4087 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/pose_bp_drop_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    10695 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/distance_plot_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     2567 2023-04-29 16:24:52.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/subset_feature_extractor_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3114 2023-04-29 18:36:18.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)     3193 2023-05-04 18:50:54.000000 Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py
+-rw-r--r--   0 simon      (501) staff       (20)    12869 2023-05-23 12:47:59.000000 Simba-UW-tf-dev-1.62.8/simba/ui/video_info_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)     6019 2023-05-16 16:45:46.000000 Simba-UW-tf-dev-1.62.8/simba/ui/user_defined_pose_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/ui/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    12602 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.62.8/simba/ui/create_project_ui.py
+-rw-r--r--   0 simon      (501) staff       (20)    10957 2023-05-04 14:03:25.000000 Simba-UW-tf-dev-1.62.8/simba/ui/tkinter_functions.py
+-rw-r--r--   0 simon      (501) staff       (20)    35432 2023-06-05 18:05:35.000000 Simba-UW-tf-dev-1.62.8/simba/ui/machine_model_settings_ui.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/blob_storage/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.62.8/simba/blob_storage/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/labelling/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 13:50:26.000000 Simba-UW-tf-dev-1.62.8/simba/labelling/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/labelling/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    20743 2023-05-14 23:21:08.000000 Simba-UW-tf-dev-1.62.8/simba/labelling/labelling_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     3568 2023-05-19 11:18:49.000000 Simba-UW-tf-dev-1.62.8/simba/labelling/extract_labelled_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)    26931 2023-05-24 17:01:48.000000 Simba-UW-tf-dev-1.62.8/simba/labelling/labelling_advanced_interface.py
+-rw-r--r--   0 simon      (501) staff       (20)     6629 2023-05-13 17:45:08.000000 Simba-UW-tf-dev-1.62.8/simba/labelling/play_annotation_video.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)    11877 2023-05-17 14:59:39.000000 Simba-UW-tf-dev-1.62.8/simba/unsupervised/dbcv_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3375 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.62.8/simba/unsupervised/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:15:51.000000 Simba-UW-tf-dev-1.62.8/simba/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     8141 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.62.8/simba/unsupervised/dataset_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5636 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.62.8/simba/unsupervised/grid_search_visualizers.py
+-rw-r--r--   0 simon      (501) staff       (20)     7310 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.62.8/simba/unsupervised/data_extractor.py
+-rw-r--r--   0 simon      (501) staff       (20)     9846 2023-06-06 18:27:30.000000 Simba-UW-tf-dev-1.62.8/simba/unsupervised/ui.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/unsupervised/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     9851 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.62.8/simba/unsupervised/umap_embedder.py
+-rw-r--r--   0 simon      (501) staff       (20)    41323 2023-05-02 18:14:28.000000 Simba-UW-tf-dev-1.62.8/simba/unsupervised/pop_up_classes.py
+-rw-r--r--   0 simon      (501) staff       (20)     2931 2023-05-17 14:54:38.000000 Simba-UW-tf-dev-1.62.8/simba/unsupervised/bout_aggregator.py
+-rw-r--r--   0 simon      (501) staff       (20)    20846 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.62.8/simba/unsupervised/cluster_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     2188 2023-04-18 23:25:29.000000 Simba-UW-tf-dev-1.62.8/simba/unsupervised/data_map.yaml
+-rw-r--r--   0 simon      (501) staff       (20)    10287 2023-06-06 17:50:12.000000 Simba-UW-tf-dev-1.62.8/simba/unsupervised/hdbscan_clusterer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3937 2023-04-28 19:59:05.000000 Simba-UW-tf-dev-1.62.8/simba/unsupervised/tsne.py
+-rw-r--r--   0 simon      (501) staff       (20)     6656 2023-05-17 15:03:51.000000 Simba-UW-tf-dev-1.62.8/simba/unsupervised/cluster_visualizer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/bounding_box_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:16:05.000000 Simba-UW-tf-dev-1.62.8/simba/bounding_box_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/bounding_box_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7031 2023-05-14 18:13:04.000000 Simba-UW-tf-dev-1.62.8/simba/bounding_box_tools/agg_boundary_stats.py
+-rw-r--r--   0 simon      (501) staff       (20)    23566 2023-05-14 18:29:41.000000 Simba-UW-tf-dev-1.62.8/simba/bounding_box_tools/boundary_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     8497 2023-05-14 18:22:39.000000 Simba-UW-tf-dev-1.62.8/simba/bounding_box_tools/boundary_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)     6376 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.62.8/simba/bounding_box_tools/find_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    11381 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.62.8/simba/bounding_box_tools/visualize_boundaries.py
+-rw-r--r--   0 simon      (501) staff       (20)    49156 2023-06-05 19:45:58.000000 Simba-UW-tf-dev-1.62.8/simba/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/
+-rw-r--r--   0 simon      (501) staff       (20)    42512 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/feature_extractor_14bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    21482 2023-05-14 23:55:56.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/feature_extractor_7bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     1685 2023-04-14 17:52:01.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/doctests.py
+-rw-r--r--   0 simon      (501) staff       (20)    23850 2023-04-17 18:48:40.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     2732 2023-04-04 19:46:36.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/read_in_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2460 2023-04-22 18:02:29.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/peaks.py
+-rw-r--r--   0 simon      (501) staff       (20)    14141 2023-03-15 17:20:08.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/fish_feature_extractor_2022.py
+-rw-r--r--   0 simon      (501) staff       (20)     2053 2023-04-04 03:00:41.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/convex_hull_3_scratch_3.py
+-rw-r--r--   0 simon      (501) staff       (20)     5762 2023-04-04 01:54:33.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/convex_hull_scratch_1.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-14 19:36:02.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    21398 2023-04-16 17:03:37.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     7127 2023-05-28 19:41:35.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/egocentrical_aligner.py
+-rw-r--r--   0 simon      (501) staff       (20)     1213 2023-04-11 20:12:47.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/count_values_in_range.py
+-rw-r--r--   0 simon      (501) staff       (20)     4708 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/graph_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3954 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/termite_rois.csv
+-rw-r--r--   0 simon      (501) staff       (20)      732 2023-03-20 12:13:51.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/mutual_exclusive.py
+-rw-r--r--   0 simon      (501) staff       (20)     2841 2023-04-14 15:16:23.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/video_color.py
+-rw-r--r--   0 simon      (501) staff       (20)     1862 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/graph_3d_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     8943 2023-06-05 18:15:28.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/shap_log_mp_2.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-13 14:05:29.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/video_rotator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8580 2023-05-31 20:02:32.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/shap_log_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     2692 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/add_probability_cnt_features.py
+-rw-r--r--   0 simon      (501) staff       (20)     1619 2023-04-08 20:02:08.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/make_splash.py
+-rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:46:44.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py
+-rw-r--r--   0 simon      (501) staff       (20)     1658 2023-04-22 19:16:28.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/time_stamp_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     5232 2023-04-15 19:24:18.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/video_rotator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     4279 2023-06-01 12:49:14.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/read_files_mp_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    30661 2023-05-19 20:44:29.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py
+-rw-r--r--   0 simon      (501) staff       (20)     2058 2023-04-03 23:51:37.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/convex_hull_scratch_2.py
+-rw-r--r--   0 simon      (501) staff       (20)    27995 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/feature_extractor_8bps_2_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-05-19 20:03:28.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3864 2023-05-19 19:41:40.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/perimeter_jit.py
+-rw-r--r--   0 simon      (501) staff       (20)    13579 2023-05-14 19:53:33.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/feature_subsets.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8244 2023-05-21 16:28:49.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/feature_extractor_user_defined.py
+-rw-r--r--   0 simon      (501) staff       (20)    46461 2023-05-15 00:03:36.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/feature_extractor_16bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    28259 2023-05-15 00:05:22.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/feature_extractor_9bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    23976 2023-05-15 00:01:21.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/feature_extractor_8bp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16880 2023-05-14 23:53:59.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/feature_extractor_4bp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/.idea/features_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      822 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)      273 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/.idea/.gitignore
+-rw-r--r--   0 simon      (501) staff       (20)     8081 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      291 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)       23 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/.idea/.name
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/feature_extractors/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    15434 2023-05-20 18:29:53.000000 Simba-UW-tf-dev-1.62.8/simba/requirements.txt
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/mixins/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-15 17:26:03.000000 Simba-UW-tf-dev-1.62.8/simba/mixins/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43029 2023-06-05 17:40:09.000000 Simba-UW-tf-dev-1.62.8/simba/mixins/pop_up_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    38228 2023-06-07 20:11:55.000000 Simba-UW-tf-dev-1.62.8/simba/mixins/config_reader.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/mixins/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18616 2023-05-17 19:39:33.000000 Simba-UW-tf-dev-1.62.8/simba/mixins/pose_importer_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/mixins/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-06-01 18:12:36.000000 Simba-UW-tf-dev-1.62.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     1223 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.62.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2023-06-01 14:35:51.000000 Simba-UW-tf-dev-1.62.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi
+-rw-r--r--   0 simon      (501) staff       (20)    82442 2023-06-01 18:12:36.000000 Simba-UW-tf-dev-1.62.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    51809 2023-05-21 16:37:18.000000 Simba-UW-tf-dev-1.62.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    14391 2023-06-01 14:35:51.000000 Simba-UW-tf-dev-1.62.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    14188 2023-05-21 00:18:56.000000 Simba-UW-tf-dev-1.62.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc
+-rw-r--r--   0 simon      (501) staff       (20)    37135 2023-06-02 12:12:15.000000 Simba-UW-tf-dev-1.62.8/simba/mixins/feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    61873 2023-05-19 21:14:46.000000 Simba-UW-tf-dev-1.62.8/simba/mixins/plotting_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     9144 2023-05-28 17:30:45.000000 Simba-UW-tf-dev-1.62.8/simba/mixins/unsupervised_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)    73224 2023-06-06 16:32:51.000000 Simba-UW-tf-dev-1.62.8/simba/mixins/train_model_mixin.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/third_party_label_appenders/
+-rw-r--r--   0 simon      (501) staff       (20)     6094 2023-05-21 17:39:19.000000 Simba-UW-tf-dev-1.62.8/simba/third_party_label_appenders/deepethogram_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10623 2023-05-21 18:42:05.000000 Simba-UW-tf-dev-1.62.8/simba/third_party_label_appenders/BORIS_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8998 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.62.8/simba/third_party_label_appenders/observer_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)    17954 2023-05-21 15:57:11.000000 Simba-UW-tf-dev-1.62.8/simba/third_party_label_appenders/tools.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-04-01 14:10:06.000000 Simba-UW-tf-dev-1.62.8/simba/third_party_label_appenders/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    18514 2023-05-29 20:20:16.000000 Simba-UW-tf-dev-1.62.8/simba/third_party_label_appenders/third_party_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     8181 2023-05-21 17:19:25.000000 Simba-UW-tf-dev-1.62.8/simba/third_party_label_appenders/ethovision_import.py
+-rw-r--r--   0 simon      (501) staff       (20)     6988 2023-05-21 17:31:04.000000 Simba-UW-tf-dev-1.62.8/simba/third_party_label_appenders/BENTO_appender.py
+-rw-r--r--   0 simon      (501) staff       (20)     5239 2023-05-21 18:07:18.000000 Simba-UW-tf-dev-1.62.8/simba/third_party_label_appenders/solomon_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/cue_light_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:06:55.000000 Simba-UW-tf-dev-1.62.8/simba/cue_light_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7652 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.62.8/simba/cue_light_tools/cue_light_clf_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)    12207 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.62.8/simba/cue_light_tools/cue_light_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16690 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.62.8/simba/cue_light_tools/cue_light_menues.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/cue_light_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     1879 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.62.8/simba/cue_light_tools/cue_light_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    15212 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.62.8/simba/cue_light_tools/cue_light_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12650 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.62.8/simba/cue_light_tools/cue_light_movement_statistics.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/utils/
+-rw-r--r--   0 simon      (501) staff       (20)    11899 2023-05-15 12:44:10.000000 Simba-UW-tf-dev-1.62.8/simba/utils/config_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    21017 2023-06-05 18:05:35.000000 Simba-UW-tf-dev-1.62.8/simba/utils/enums.py
+-rw-r--r--   0 simon      (501) staff       (20)    10244 2023-06-05 17:20:50.000000 Simba-UW-tf-dev-1.62.8/simba/utils/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7396 2023-06-01 13:09:55.000000 Simba-UW-tf-dev-1.62.8/simba/utils/warnings.py
+-rw-r--r--   0 simon      (501) staff       (20)     8807 2023-05-25 13:24:45.000000 Simba-UW-tf-dev-1.62.8/simba/utils/checks.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/utils/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    43061 2023-05-25 14:56:03.000000 Simba-UW-tf-dev-1.62.8/simba/utils/read_write.py
+-rw-r--r--   0 simon      (501) staff       (20)     8585 2023-06-05 17:07:45.000000 Simba-UW-tf-dev-1.62.8/simba/utils/lookups.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/utils/cli/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/utils/cli/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6017 2023-05-28 13:41:20.000000 Simba-UW-tf-dev-1.62.8/simba/utils/cli/cli_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    14666 2023-04-28 19:59:06.000000 Simba-UW-tf-dev-1.62.8/simba/utils/errors.py
+-rw-r--r--   0 simon      (501) staff       (20)    17829 2023-05-25 17:48:38.000000 Simba-UW-tf-dev-1.62.8/simba/utils/data.py
+-rw-r--r--   0 simon      (501) staff       (20)     1615 2023-05-08 18:13:22.000000 Simba-UW-tf-dev-1.62.8/simba/utils/printing.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/pose_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     8256 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.62.8/simba/pose_processors/reorganize_keypoint.py
+-rw-r--r--   0 simon      (501) staff       (20)     5167 2023-05-15 16:58:05.000000 Simba-UW-tf-dev-1.62.8/simba/pose_processors/remove_keypoints.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/pose_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     2656 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.62.8/simba/pose_processors/pose_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)     5614 2023-05-04 15:35:50.000000 Simba-UW-tf-dev-1.62.8/simba/pose_processors/reverse_pose.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/
+-rw-r--r--   0 simon      (501) staff       (20)     9114 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/gantt_creator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5388 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/tools/tkinter_tools.py
+-rw-r--r--   0 simon      (501) staff       (20)    13008 2023-05-24 15:32:44.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/ROI_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-25 23:35:57.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    14568 2023-05-15 18:41:17.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/shap_agg_stats_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10105 2023-05-15 17:45:06.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/gantt_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15730 2023-05-15 17:49:01.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/heat_mapper_clf_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8731 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/probability_plot_creator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12484 2023-05-23 14:52:24.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/plot_clf_results.py
+-rw-r--r--   0 simon      (501) staff       (20)    14056 2023-05-17 14:20:24.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/plot_clf_results_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    16031 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/ROI_feature_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    12770 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/heat_mapper_location.py
+-rw-r--r--   0 simon      (501) staff       (20)    10100 2023-05-15 18:13:11.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/probability_plot_creator_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     4881 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/interactive_probability_grapher.py
+-rw-r--r--   0 simon      (501) staff       (20)     5812 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/plot_pose_in_dir.py
+-rw-r--r--   0 simon      (501) staff       (20)    14029 2023-06-04 11:55:47.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/single_run_model_validation_video.py
+-rw-r--r--   0 simon      (501) staff       (20)    12790 2023-05-16 16:20:20.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/frame_mergerer_ffmpeg.py
+-rw-r--r--   0 simon      (501) staff       (20)     7891 2023-05-29 21:41:05.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/Directing_animals_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11219 2023-05-17 12:58:17.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/clf_validator.py
+-rw-r--r--   0 simon      (501) staff       (20)    15745 2023-05-20 12:16:06.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/path_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    11203 2023-05-24 15:35:24.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/ROI_feature_visualizer_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)     8933 2023-05-16 16:18:45.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/data_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13471 2023-05-20 12:15:46.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/path_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     6494 2023-05-17 20:55:17.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/ez_lineplot.py
+-rw-r--r--   0 simon      (501) staff       (20)    11519 2023-05-31 16:42:04.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/distance_plotter_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    15794 2023-05-17 13:58:48.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/ROI_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    13163 2023-05-16 16:42:03.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/heat_mapper_clf.py
+-rw-r--r--   0 simon      (501) staff       (20)     9385 2023-05-31 16:46:49.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)     9526 2023-06-04 12:03:25.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/single_run_model_validation_video_mp.py
+-rw-r--r--   0 simon      (501) staff       (20)    10005 2023-05-29 21:36:37.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/Directing_animals_visualizer.py
+-rw-r--r--   0 simon      (501) staff       (20)    16320 2023-05-15 18:08:47.000000 Simba-UW-tf-dev-1.62.8/simba/plotting/heat_mapper_location_mp.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/dash_app/
+-rw-r--r--   0 simon      (501) staff       (20)    49699 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/dash_app/SimBA_dash_app.py
+-rw-r--r--   0 simon      (501) staff       (20)     5029 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/dash_app/run_dash_tkinter.py
+-rw-r--r--   0 simon      (501) staff       (20)    24474 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/dash_app/dash_app.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/data_processors/
+-rw-r--r--   0 simon      (501) staff       (20)     7248 2023-05-25 19:01:00.000000 Simba-UW-tf-dev-1.62.8/simba/data_processors/agg_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    11196 2023-05-28 19:50:35.000000 Simba-UW-tf-dev-1.62.8/simba/data_processors/severity_bout_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16259 2023-05-24 20:39:01.000000 Simba-UW-tf-dev-1.62.8/simba/data_processors/interpolation_smoothing.py
+-rw-r--r--   0 simon      (501) staff       (20)     8127 2023-05-25 13:57:19.000000 Simba-UW-tf-dev-1.62.8/simba/data_processors/timebins_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    12938 2023-05-23 20:14:45.000000 Simba-UW-tf-dev-1.62.8/simba/data_processors/fsttc_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/data_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6306 2023-05-13 17:09:38.000000 Simba-UW-tf-dev-1.62.8/simba/data_processors/interpolate_pose.py
+-rw-r--r--   0 simon      (501) staff       (20)     9646 2023-05-14 19:19:14.000000 Simba-UW-tf-dev-1.62.8/simba/data_processors/directing_other_animals_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8624 2023-05-25 14:07:56.000000 Simba-UW-tf-dev-1.62.8/simba/data_processors/timebins_movement_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     4799 2023-05-17 17:23:16.000000 Simba-UW-tf-dev-1.62.8/simba/data_processors/severity_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    16980 2023-05-14 19:47:31.000000 Simba-UW-tf-dev-1.62.8/simba/data_processors/pup_retrieval_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     3143 2023-05-13 17:23:00.000000 Simba-UW-tf-dev-1.62.8/simba/data_processors/pybursts_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    11533 2023-05-28 19:50:34.000000 Simba-UW-tf-dev-1.62.8/simba/data_processors/severity_frame_based_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     9656 2023-05-25 13:32:25.000000 Simba-UW-tf-dev-1.62.8/simba/data_processors/kleinberg_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     8131 2023-05-25 14:37:36.000000 Simba-UW-tf-dev-1.62.8/simba/data_processors/movement_calculator.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-03-30 11:05:37.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1334 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       26 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      282 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-03-30 10:45:10.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    11376 2023-04-28 23:45:27.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/model/
+-rw-r--r--   0 simon      (501) staff       (20)    20086 2023-06-05 20:43:28.000000 Simba-UW-tf-dev-1.62.8/simba/model/train_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-20 18:06:50.000000 Simba-UW-tf-dev-1.62.8/simba/model/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     3315 2023-05-18 22:48:36.000000 Simba-UW-tf-dev-1.62.8/simba/model/inference_batch.py
+-rw-r--r--   0 simon      (501) staff       (20)    20849 2023-06-05 18:44:40.000000 Simba-UW-tf-dev-1.62.8/simba/model/grid_search_rf.py
+-rw-r--r--   0 simon      (501) staff       (20)     3363 2023-05-19 11:12:45.000000 Simba-UW-tf-dev-1.62.8/simba/model/inference_validation.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/roi_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     5858 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_time_bin_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)     1687 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_movement_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-20 12:47:56.000000 Simba-UW-tf-dev-1.62.8/simba/roi_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    43119 2023-05-14 16:11:59.000000 Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_define.py
+-rw-r--r--   0 simon      (501) staff       (20)     4024 2023-05-16 13:21:43.000000 Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_reset.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/roi_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    19901 2023-05-15 17:00:34.000000 Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    11608 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_feature_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)     3654 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_multiply.py
+-rw-r--r--   0 simon      (501) staff       (20)      959 2023-05-15 17:20:07.000000 Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_size_calculations.py
+-rw-r--r--   0 simon      (501) staff       (20)     3505 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_zoom.py
+-rw-r--r--   0 simon      (501) staff       (20)    11556 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_directing_analyzer.py
+-rw-r--r--   0 simon      (501) staff       (20)    10128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_move_shape.py
+-rw-r--r--   0 simon      (501) staff       (20)     5079 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)    13742 2023-05-15 17:12:32.000000 Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_clf_calculator.py
+-rw-r--r--   0 simon      (501) staff       (20)    22688 2023-04-29 19:01:32.000000 Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_image.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/pose_importers/
+-rw-r--r--   0 simon      (501) staff       (20)     8115 2023-05-14 18:03:14.000000 Simba-UW-tf-dev-1.62.8/simba/pose_importers/sleap_csv_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/pose_importers/misc/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:42:38.000000 Simba-UW-tf-dev-1.62.8/simba/pose_importers/misc/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7943 2023-05-01 19:07:14.000000 Simba-UW-tf-dev-1.62.8/simba/pose_importers/misc/apt_trk_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     2464 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.62.8/simba/pose_importers/read_DANNCE_mat.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-09 17:45:51.000000 Simba-UW-tf-dev-1.62.8/simba/pose_importers/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)    12549 2023-05-17 20:32:56.000000 Simba-UW-tf-dev-1.62.8/simba/pose_importers/sleap_h5_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7322 2023-05-16 16:55:05.000000 Simba-UW-tf-dev-1.62.8/simba/pose_importers/madlc_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/pose_importers/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)    12141 2023-05-16 18:48:44.000000 Simba-UW-tf-dev-1.62.8/simba/pose_importers/sleap_slp_importer.py
+-rw-r--r--   0 simon      (501) staff       (20)     7931 2023-05-15 16:58:04.000000 Simba-UW-tf-dev-1.62.8/simba/pose_importers/import_mars.py
+-rw-r--r--   0 simon      (501) staff       (20)     6978 2023-05-15 16:44:53.000000 Simba-UW-tf-dev-1.62.8/simba/pose_importers/dlc_importer_csv.py
+-rw-r--r--   0 simon      (501) staff       (20)     8060 2023-04-28 19:20:42.000000 Simba-UW-tf-dev-1.62.8/simba/pose_importers/trk_importer.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations/
+-rw-r--r--   0 simon      (501) staff       (20)    14340 2023-05-14 23:57:00.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations/bp_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:00.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations/bp_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1316 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations/bp_names/bp_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations/no_animals/
+-rw-r--r--   0 simon      (501) staff       (20)       24 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations/no_animals/no_animals.csv
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:19.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations/no_animals/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations/configuration_names/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-16 13:26:14.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations/configuration_names/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)      267 2023-04-29 18:20:02.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations/configuration_names/pose_config_names.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/
+-rw-r--r--   0 simon      (501) staff       (20)    39805 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/8.png
+-rw-r--r--   0 simon      (501) staff       (20)    62501 2023-03-30 10:39:05.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/9.png
+-rw-r--r--   0 simon      (501) staff       (20)     6172 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/12.png
+-rw-r--r--   0 simon      (501) staff       (20)    69501 2023-03-30 10:44:04.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/11.png
+-rw-r--r--   0 simon      (501) staff       (20)    69410 2023-03-30 10:40:01.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/10.png
+-rw-r--r--   0 simon      (501) staff       (20)    16000 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/4.png
+-rw-r--r--   0 simon      (501) staff       (20)    28150 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/5.png
+-rw-r--r--   0 simon      (501) staff       (20)    31140 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/7.png
+-rw-r--r--   0 simon      (501) staff       (20)    30634 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/6.png
+-rw-r--r--   0 simon      (501) staff       (20)    15417 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/2.png
+-rw-r--r--   0 simon      (501) staff       (20)    15786 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/3.png
+-rw-r--r--   0 simon      (501) staff       (20)    18939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/1.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/video_processors/
+-rw-r--r--   0 simon      (501) staff       (20)    45564 2023-05-14 17:15:40.000000 Simba-UW-tf-dev-1.62.8/simba/video_processors/video_processing.py
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-05-20 18:15:51.000000 Simba-UW-tf-dev-1.62.8/simba/video_processors/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     7171 2023-04-27 19:42:17.000000 Simba-UW-tf-dev-1.62.8/simba/video_processors/px_to_mm.py
+-rw-r--r--   0 simon      (501) staff       (20)    24648 2023-05-16 16:42:04.000000 Simba-UW-tf-dev-1.62.8/simba/video_processors/batch_process_menus.py
+-rw-r--r--   0 simon      (501) staff       (20)     7333 2023-05-16 12:54:28.000000 Simba-UW-tf-dev-1.62.8/simba/video_processors/multi_cropper.py
+-rw-r--r--   0 simon      (501) staff       (20)     2833 2023-04-27 20:23:35.000000 Simba-UW-tf-dev-1.62.8/simba/video_processors/extract_frames.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/video_processors/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8266 2023-05-08 18:19:00.000000 Simba-UW-tf-dev-1.62.8/simba/video_processors/calculate_px_dist.py
+-rw-r--r--   0 simon      (501) staff       (20)     4695 2023-04-26 18:17:53.000000 Simba-UW-tf-dev-1.62.8/simba/video_processors/extract_seqframes.py
+-rw-r--r--   0 simon      (501) staff       (20)    11087 2023-05-14 16:24:59.000000 Simba-UW-tf-dev-1.62.8/simba/video_processors/batch_process_create_ffmpeg_commands.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/outlier_tools/
+-rw-r--r--   0 simon      (501) staff       (20)     6535 2023-05-25 14:24:01.000000 Simba-UW-tf-dev-1.62.8/simba/outlier_tools/outlier_corrector_movement.py
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-05-08 20:25:20.000000 Simba-UW-tf-dev-1.62.8/simba/outlier_tools/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/outlier_tools/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     8168 2023-06-01 12:38:34.000000 Simba-UW-tf-dev-1.62.8/simba/outlier_tools/outlier_corrector_location.py
+-rw-r--r--   0 simon      (501) staff       (20)     2668 2023-05-25 14:26:49.000000 Simba-UW-tf-dev-1.62.8/simba/outlier_tools/skip_outlier_correction.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/outlier_tools/.idea/
+-rw-r--r--   0 simon      (501) staff       (20)      617 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/outlier_tools/.idea/outlier_scripts.iml
+-rw-r--r--   0 simon      (501) staff       (20)      138 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/outlier_tools/.idea/encodings.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/outlier_tools/.idea/inspectionProfiles/
+-rw-r--r--   0 simon      (501) staff       (20)      668 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/outlier_tools/.idea/libraries/
+-rw-r--r--   0 simon      (501) staff       (20)      128 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/outlier_tools/.idea/libraries/R_User_Library.xml
+-rw-r--r--   0 simon      (501) staff       (20)     8102 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/outlier_tools/.idea/workspace.xml
+-rw-r--r--   0 simon      (501) staff       (20)      289 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/outlier_tools/.idea/modules.xml
+-rw-r--r--   0 simon      (501) staff       (20)      294 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/outlier_tools/.idea/misc.xml
+-rw-r--r--   0 simon      (501) staff       (20)    65549 2023-05-25 18:24:18.000000 Simba-UW-tf-dev-1.62.8/simba/SimBA.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/assets/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/assets/unsupervised/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/unsupervised/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   109483 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/unsupervised/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/unsupervised/features.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/assets/shap/
+-rw-r--r--   0 simon      (501) staff       (20)     1177 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/shap/down_arrow.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1733 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/shap/intruder_shape.jpg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/assets/shap/feature_categories/
+-rw-r--r--   0 simon      (501) staff       (20)      109 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/shap/feature_categories/.~lock.shap_feature_categories.csv#
+-rw-r--r--   0 simon      (501) staff       (20)    17420 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/shap/feature_categories/shap_feature_categories.csv
+-rw-r--r--   0 simon      (501) staff       (20)     8196 2023-04-10 20:37:13.000000 Simba-UW-tf-dev-1.62.8/simba/assets/shap/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)     1665 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/shap/resident_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2415 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/shap/resident_intruder_shape.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2012 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/shap/animal_distances.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     4422 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/shap/baseline_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   353824 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/shap/ubuntu.regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     6672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/shap/side_scale.jpg
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/shap/UbuntuMono-Regular.ttf
+-rw-r--r--   0 simon      (501) staff       (20)     2737 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/shap/side_scale_5.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1785 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/shap/intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     1435 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/shap/resident_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     3134 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/shap/color_bar.jpg
+-rw-r--r--   0 simon      (501) staff       (20)     2120 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/shap/resident_intruder_movement.jpg
+-rw-r--r--   0 simon      (501) staff       (20)    16388 2023-05-15 20:24:40.000000 Simba-UW-tf-dev-1.62.8/simba/assets/.DS_Store
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/assets/lookups/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/lookups/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   270783 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/lookups/model_names.parquet
+-rw-r--r--   0 simon      (501) staff       (20)     2987 2023-04-25 20:39:03.000000 Simba-UW-tf-dev-1.62.8/simba/assets/lookups/feature_extraction_headers.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/lookups/features.csv
+-rw-r--r--   0 simon      (501) staff       (20)    14175 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/lookups/unsupervised_example_x.csv
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/assets/stl/
+-rw-r--r--   0 simon      (501) staff       (20)   551576 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/stl/operant_tray.stl
+-rw-r--r--   0 simon      (501) staff       (20)    67647 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/stl/operant_lever.stl
+-rw-r--r--   0 simon      (501) staff       (20)    92896 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/stl/operant_walls.stl
+-rw-r--r--   0 simon      (501) staff       (20)  4759984 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/stl/grid_floor.stl
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/assets/img/
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-10 23:20:37.000000 Simba-UW-tf-dev-1.62.8/simba/assets/img/.DS_Store
+-rw-r--r--   0 simon      (501) staff       (20)   399272 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/img/about_me.png
+-rw-r--r--   0 simon      (501) staff       (20)   117108 2023-04-10 23:06:31.000000 Simba-UW-tf-dev-1.62.8/simba/assets/img/splash.mp4
+-rw-r--r--   0 simon      (501) staff       (20)   322242 2023-04-06 16:38:51.000000 Simba-UW-tf-dev-1.62.8/simba/assets/img/bg_2.png
+-rw-r--r--   0 simon      (501) staff       (20)    69267 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/img/splash.pptx
+-rw-r--r--   0 simon      (501) staff       (20)   204362 2023-04-06 15:01:45.000000 Simba-UW-tf-dev-1.62.8/simba/assets/img/bg.png
+-rw-r--r--   0 simon      (501) staff       (20)   189004 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/UbuntuMono-Regular.ttf
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/
+-rw-r--r--   0 simon      (501) staff       (20)     1350 2023-03-17 17:59:27.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/factory.png
+-rw-r--r--   0 simon      (501) staff       (20)     1413 2023-03-21 13:03:06.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/cluster.png
+-rw-r--r--   0 simon      (501) staff       (20)     1340 2023-03-17 16:51:08.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/load.png
+-rw-r--r--   0 simon      (501) staff       (20)     4507 2023-03-20 14:13:48.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/gif.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4566 2023-03-18 18:12:27.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/pose.png
+-rw-rw-r--   0 simon      (501) staff       (20)     1943 2023-03-18 18:14:10.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/features.png
+-rw-r--r--   0 simon      (501) staff       (20)     6148 2023-04-05 17:25:36.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/.DS_Store
+-rw-rw-r--   0 simon      (501) staff       (20)     4896 2023-03-17 19:17:29.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/settings.png
+-rw-r--r--   0 simon      (501) staff       (20)     2090 2023-04-22 15:14:17.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/stopwatch.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-03-19 16:48:40.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/link.png
+-rw-r--r--   0 simon      (501) staff       (20)    14250 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/dash_simba.css
+-rw-r--r--   0 simon      (501) staff       (20)      917 2023-04-05 16:43:13.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/documentation.png
+-rw-r--r--   0 simon      (501) staff       (20)     4503 2023-03-20 14:08:00.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/fps.png
+-rw-r--r--   0 simon      (501) staff       (20)     1299 2023-03-21 13:02:07.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/dimensionality_reduction.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4823 2023-03-17 19:03:29.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/roi.png
+-rw-r--r--   0 simon      (501) staff       (20)      920 2023-03-20 14:25:03.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/superimpose.png
+-rw-r--r--   0 simon      (501) staff       (20)     1136 2023-03-18 20:25:31.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/label.png
+-rw-r--r--   0 simon      (501) staff       (20)     1016 2023-03-20 14:28:47.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/change.png
+-rw-r--r--   0 simon      (501) staff       (20)     1124 2023-03-17 18:05:26.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/crop.png
+-rw-r--r--   0 simon      (501) staff       (20)     2146 2023-04-13 14:09:23.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/rotate.png
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-20 14:03:42.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/path.png
+-rw-r--r--   0 simon      (501) staff       (20)      950 2023-03-17 18:07:33.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/clip.png
+-rw-r--r--   0 simon      (501) staff       (20)     2121 2023-04-04 14:37:43.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/restart.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-17 18:11:59.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/calipher.png
+-rw-r--r--   0 simon      (501) staff       (20)     1291 2023-03-21 20:16:55.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/add_on.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4695 2023-03-17 17:57:16.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/create.png
+-rw-r--r--   0 simon      (501) staff       (20)    78182 2023-03-20 16:35:36.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/SimBA_logo.ico
+-rw-r--r--   0 simon      (501) staff       (20)     1067 2023-03-20 14:22:44.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/print.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4653 2023-03-18 20:27:58.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/clf.png
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/concat_icons/
+-rw-r--r--   0 simon      (501) staff       (20)     6027 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/concat_icons/mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     5654 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/concat_icons/vertical.png
+-rw-r--r--   0 simon      (501) staff       (20)     5542 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/concat_icons/horizontal.png
+-rw-r--r--   0 simon      (501) staff       (20)     5939 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/concat_icons/mixed_mosaic.png
+-rw-r--r--   0 simon      (501) staff       (20)     2060 2023-03-20 14:26:12.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/merge.png
+-rw-r--r--   0 simon      (501) staff       (20)     1252 2023-04-07 11:25:59.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/clean.png
+-rw-------   0 simon      (501) staff       (20)     4725 2023-03-18 20:27:47.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/clf_2.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4795 2023-03-17 18:10:10.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/visualize.png
+-rw-r--r--   0 simon      (501) staff       (20)     2142 2023-03-20 14:10:28.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/concat.png
+-rw-r--r--   0 simon      (501) staff       (20)     1474 2023-03-17 19:20:24.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/boris.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4804 2023-03-19 16:43:01.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/frames.png
+-rw-r--r--   0 simon      (501) staff       (20)     2425 2023-03-19 16:44:55.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/video.png
+-rw-r--r--   0 simon      (501) staff       (20)     2089 2023-03-20 14:05:58.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/sample.png
+-rw-r--r--   0 simon      (501) staff       (20)     1471 2023-03-21 13:04:02.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/metrics.png
+-rw-r--r--   0 simon      (501) staff       (20)     4555 2023-03-20 14:21:02.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/grey.png
+-rw-r--r--   0 simon      (501) staff       (20)      930 2023-03-18 18:07:29.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/exit.png
+-rw-r--r--   0 simon      (501) staff       (20)     4751 2023-03-18 20:31:58.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/outlier.png
+-rw-r--r--   0 simon      (501) staff       (20)     4392 2023-03-20 14:16:15.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/clahe.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4637 2023-03-17 19:03:55.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/trash.png
+-rw-r--r--   0 simon      (501) staff       (20)     1239 2023-03-19 16:51:21.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/about.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4666 2023-03-17 18:01:21.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/convert.png
+-rw-r--r--   0 simon      (501) staff       (20)    93229 2023-03-20 16:01:42.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/SimBA_logo.icns
+-rw-r--r--   0 simon      (501) staff       (20)      991 2023-03-20 19:02:33.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/reorganize.png
+-rw-rw-r--   0 simon      (501) staff       (20)     4784 2023-03-17 18:50:35.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/browse.png
+-rw-r--r--   0 simon      (501) staff       (20)    30707 2023-03-20 16:33:38.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/SimBA_logo.png
+-rw-r--r--   0 simon      (501) staff       (20)     2293 2023-03-17 19:24:38.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/ethovision.png
+-rw-r--r--   0 simon      (501) staff       (20)     1018 2023-04-05 15:24:49.000000 Simba-UW-tf-dev-1.62.8/simba/assets/icons/close.png
+-rw-r--r--   0 simon      (501) staff       (20)    13672 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/dash_simba_base.css
+-rw-r--r--   0 simon      (501) staff       (20)    31812 2023-03-10 20:04:56.000000 Simba-UW-tf-dev-1.62.8/simba/assets/TheGoldenLab.PNG
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/Simba_UW_tf_dev.egg-info/
+-rw-rw-r--   0 simon      (501) staff       (20)      579 2023-06-07 20:12:48.000000 Simba-UW-tf-dev-1.62.8/Simba_UW_tf_dev.egg-info/PKG-INFO
+-rw-rw-r--   0 simon      (501) staff       (20)    19299 2023-06-07 20:12:48.000000 Simba-UW-tf-dev-1.62.8/Simba_UW_tf_dev.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       44 2023-06-07 20:12:48.000000 Simba-UW-tf-dev-1.62.8/Simba_UW_tf_dev.egg-info/entry_points.txt
+-rw-rw-r--   0 simon      (501) staff       (20)      639 2023-06-07 20:12:48.000000 Simba-UW-tf-dev-1.62.8/Simba_UW_tf_dev.egg-info/requires.txt
+-rw-rw-r--   0 simon      (501) staff       (20)       12 2023-06-07 20:12:48.000000 Simba-UW-tf-dev-1.62.8/Simba_UW_tf_dev.egg-info/top_level.txt
+-rw-rw-r--   0 simon      (501) staff       (20)        1 2023-06-07 20:12:48.000000 Simba-UW-tf-dev-1.62.8/Simba_UW_tf_dev.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon      (501) staff       (20)     7652 2020-05-13 13:27:38.000000 Simba-UW-tf-dev-1.62.8/LICENSE.md
+-rw-r--r--   0 simon      (501) staff       (20)       89 2023-05-20 17:55:56.000000 Simba-UW-tf-dev-1.62.8/pyproject.toml
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/tests/
+-rw-r--r--   0 simon      (501) staff       (20)     5209 2023-05-28 14:15:24.000000 Simba-UW-tf-dev-1.62.8/tests/test_data_processors.py
+-rw-r--r--   0 simon      (501) staff       (20)     5317 2023-05-31 19:40:16.000000 Simba-UW-tf-dev-1.62.8/tests/test_distance_plotter.py
+-rw-r--r--   0 simon      (501) staff       (20)    12821 2023-06-07 02:40:14.000000 Simba-UW-tf-dev-1.62.8/tests/test_train_model_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.8/tests/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     6757 2023-06-02 12:11:53.000000 Simba-UW-tf-dev-1.62.8/tests/test_feature_extraction_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     8984 2023-06-07 20:11:11.000000 Simba-UW-tf-dev-1.62.8/tests/test_config_reader_mixin.py
+-rw-r--r--   0 simon      (501) staff       (20)     1528 2023-05-25 14:26:19.000000 Simba-UW-tf-dev-1.62.8/tests/test_outlier_correctors.py
+-rw-r--r--   0 simon      (501) staff       (20)     4356 2023-05-29 20:59:49.000000 Simba-UW-tf-dev-1.62.8/tests/test_visualize_directing_animals.py
+-rw-r--r--   0 simon      (501) staff       (20)     1859 2023-05-21 16:40:19.000000 Simba-UW-tf-dev-1.62.8/tests/test_featurizers.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/tests/data/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.8/tests/data/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/tests/data/test_projects/
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/tests/data/test_projects/two_c57/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.8/tests/data/test_projects/two_c57/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/tests/data/test_projects/two_c57/models/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.8/tests/data/test_projects/two_c57/models/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.8/tests/data/test_projects/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/tests/data/test_projects/mouse_open_field/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.8/tests/data/test_projects/mouse_open_field/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/tests/data/test_projects/zebrafish/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-05-20 18:02:57.000000 Simba-UW-tf-dev-1.62.8/tests/data/test_projects/zebrafish/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/tests/data/test_projects/zebrafish/feature_file/
+-rw-rw-r--   0 simon      (501) staff       (20)        0 2020-08-11 16:11:18.000000 Simba-UW-tf-dev-1.62.8/tests/data/test_projects/zebrafish/feature_file/__init__.py
+-rw-rw-r--   0 simon      (501) staff       (20)    14128 2022-04-11 08:07:36.000000 Simba-UW-tf-dev-1.62.8/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py
+-rw-r--r--   0 simon      (501) staff       (20)     3971 2023-05-28 17:20:18.000000 Simba-UW-tf-dev-1.62.8/tests/test_thirdparty_appenders.py
+-rw-r--r--   0 simon      (501) staff       (20)     3090 2023-05-31 15:49:24.000000 Simba-UW-tf-dev-1.62.8/tests/test_validation_clips.py
+-rw-rw-r--   0 simon      (501) staff       (20)      136 2021-04-10 10:44:06.000000 Simba-UW-tf-dev-1.62.8/MANIFEST.in
+-rw-rw-r--   0 simon      (501) staff       (20)     9598 2020-05-13 13:27:40.000000 Simba-UW-tf-dev-1.62.8/README.md
+-rw-rw-r--   0 simon      (501) staff       (20)     1897 2023-06-07 20:12:47.000000 Simba-UW-tf-dev-1.62.8/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-06-07 20:12:49.000000 Simba-UW-tf-dev-1.62.8/setup.cfg
```

### Comparing `Simba-UW-tf-dev-1.62.7/PKG-INFO` & `Simba-UW-tf-dev-1.62.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.62.7
+Version: 1.62.8
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/.DS_Store` & `Simba-UW-tf-dev-1.62.8/simba/ui/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/movement_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/csv_2_parquet_pop_up.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/csv_2_parquet_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/quick_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/quick_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/batch_preprocess_pop_up.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/batch_preprocess_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/heatmap_location_pop_up.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/heatmap_location_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/clf_probability_plot_pop_up.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/clf_probability_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/.DS_Store` & `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/movement_analysis_pop_up.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/movement_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/set_machine_model_parameters_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/clf_plot_pop_up.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/clf_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/path_plot_pop_up.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/remove_roi_features_pop_up.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/remove_roi_features_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/smoothing_interpolation_pop_up.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/smoothing_interpolation_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/visualize_pose_in_dir_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/roi_analysis_pop_up.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/roi_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/outlier_settings_pop_up.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/outlier_settings_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/gantt_pop_up.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/gantt_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/clf_validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/clf_validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/severity_analysis_pop_up.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/severity_analysis_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/fsttc_pop_up.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/fsttc_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/kleinberg_pop_up.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/kleinberg_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/directing_other_animals_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/pose_reorganizer_pop_up.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/pose_reorganizer_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/append_roi_features_animals_pop_up.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/append_roi_features_animals_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/clf_by_timebins_pop_up.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/clf_by_timebins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/heatmap_clf_pop_up.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/heatmap_clf_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/data_plot_pop_up.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/data_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/roi_features_plot_pop_up.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/roi_features_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/pup_retrieval_pop_up.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/pup_retrieval_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/about_simba_pop_up.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/about_simba_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/clf_descriptive_statistics_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/roi_tracking_plot_pop_up.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/roi_tracking_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/append_roi_features_bodypart_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/clf_add_remove_print_pop_up.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/clf_add_remove_print_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/video_processing_pop_up.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/video_processing_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/validation_plot_pop_up.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/validation_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/clf_by_roi_pop_up.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/clf_by_roi_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/make_path_plot_pop_up.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/make_path_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/create_user_defined_pose_configuration_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/archive_files_pop_up.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/archive_files_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/pose_bp_drop_pop_up.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/pose_bp_drop_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/distance_plot_pop_up.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/distance_plot_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/subset_feature_extractor_pop_up.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/subset_feature_extractor_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/third_party_annotator_appender_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/pop_ups/roi_analysis_time_bins_pop_up.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/video_info_ui.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/video_info_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/user_defined_pose_creator.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/user_defined_pose_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/create_project_ui.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/create_project_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/tkinter_functions.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/tkinter_functions.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/ui/machine_model_settings_ui.py` & `Simba-UW-tf-dev-1.62.8/simba/ui/machine_model_settings_ui.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/blob_storage/.DS_Store` & `Simba-UW-tf-dev-1.62.8/simba/blob_storage/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/labelling/.DS_Store` & `Simba-UW-tf-dev-1.62.8/simba/labelling/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/labelling/labelling_interface.py` & `Simba-UW-tf-dev-1.62.8/simba/labelling/labelling_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/labelling/extract_labelled_frames.py` & `Simba-UW-tf-dev-1.62.8/simba/labelling/extract_labelled_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/labelling/labelling_advanced_interface.py` & `Simba-UW-tf-dev-1.62.8/simba/labelling/labelling_advanced_interface.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/labelling/play_annotation_video.py` & `Simba-UW-tf-dev-1.62.8/simba/labelling/play_annotation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/unsupervised/dbcv_calculator.py` & `Simba-UW-tf-dev-1.62.8/simba/unsupervised/dbcv_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/unsupervised/enums.py` & `Simba-UW-tf-dev-1.62.8/simba/unsupervised/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.62.8/simba/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/unsupervised/dataset_creator.py` & `Simba-UW-tf-dev-1.62.8/simba/unsupervised/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/unsupervised/grid_search_visualizers.py` & `Simba-UW-tf-dev-1.62.8/simba/unsupervised/grid_search_visualizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/unsupervised/data_extractor.py` & `Simba-UW-tf-dev-1.62.8/simba/unsupervised/data_extractor.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/unsupervised/ui.py` & `Simba-UW-tf-dev-1.62.8/simba/unsupervised/ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,16 +27,14 @@
 class UnsupervisedGUI(ConfigReader, PopUpMixin):
     """
     Main access to unsupervised interface
     """
     def __init__(self,
                  config_path: str):
 
-
-
         ConfigReader.__init__(self, config_path=config_path)
         PopUpMixin.__init__(self, title="UNSUPERVISED ANALYSIS", config_path=config_path, size=(1000, 800))
         self.main_frm = Toplevel()
         self.main_frm.minsize(1000, 800)
         self.main_frm.wm_title("UNSUPERVISED ANALYSIS")
         self.main_frm.columnconfigure(0, weight=1)
         self.main_frm.rowconfigure(0, weight=1)
```

### Comparing `Simba-UW-tf-dev-1.62.7/simba/unsupervised/umap_embedder.py` & `Simba-UW-tf-dev-1.62.8/simba/unsupervised/umap_embedder.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/unsupervised/pop_up_classes.py` & `Simba-UW-tf-dev-1.62.8/simba/unsupervised/pop_up_classes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/unsupervised/bout_aggregator.py` & `Simba-UW-tf-dev-1.62.8/simba/unsupervised/bout_aggregator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/unsupervised/cluster_statistics.py` & `Simba-UW-tf-dev-1.62.8/simba/unsupervised/cluster_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/unsupervised/data_map.yaml` & `Simba-UW-tf-dev-1.62.8/simba/unsupervised/data_map.yaml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/unsupervised/hdbscan_clusterer.py` & `Simba-UW-tf-dev-1.62.8/simba/unsupervised/hdbscan_clusterer.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
     Methods for grid-search HDBSCAN model fit and transform.
     Defaults to GPU and cuml.cluster.HDBSCAN. If GPU unavailable, then hdbscan.HDBSCAN.
     """
     def __init__(self):
         super().__init__()
 
 
-
     def fit(self,
             data_path: str,
             save_dir: str,
             hyper_parameters: dict):
 
         """
         :param data_path: Path holding pickled unsupervised dimensionality reduction results in ``data_map.yaml`` format
```

### Comparing `Simba-UW-tf-dev-1.62.7/simba/unsupervised/tsne.py` & `Simba-UW-tf-dev-1.62.8/simba/unsupervised/tsne.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/unsupervised/cluster_visualizer.py` & `Simba-UW-tf-dev-1.62.8/simba/unsupervised/cluster_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/bounding_box_tools/.DS_Store` & `Simba-UW-tf-dev-1.62.8/simba/bounding_box_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/bounding_box_tools/agg_boundary_stats.py` & `Simba-UW-tf-dev-1.62.8/simba/bounding_box_tools/agg_boundary_stats.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/bounding_box_tools/boundary_menus.py` & `Simba-UW-tf-dev-1.62.8/simba/bounding_box_tools/boundary_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/bounding_box_tools/boundary_statistics.py` & `Simba-UW-tf-dev-1.62.8/simba/bounding_box_tools/boundary_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/bounding_box_tools/find_boundaries.py` & `Simba-UW-tf-dev-1.62.8/simba/bounding_box_tools/find_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/bounding_box_tools/visualize_boundaries.py` & `Simba-UW-tf-dev-1.62.8/simba/bounding_box_tools/visualize_boundaries.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/.DS_Store` & `Simba-UW-tf-dev-1.62.8/simba/.DS_Store`

 * *Files 2% similar despite different names*

```diff
@@ -764,15 +764,15 @@
 00002fb0: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
 00002fc0: 735b 5368 6f77 5369 6465 6261 7208 0809  s[ShowSidebar...
 00002fd0: 0809 5f10 187b 7b32 302c 2032 3336 7d2c  .._..{{20, 236},
 00002fe0: 207b 3130 3736 2c20 3632 317d 7d09 0817   {1076, 621}}...
 00002ff0: 2531 3d49 606d 797a 7b7c 7d7e 9900 0000  %1=I`myz{|}~....
 00003000: 0000 0001 0000 0000 0000 0010 0000 0005  ................
 00003010: 0075 0074 0069 006c 0073 6c67 3153 636f  .u.t.i.l.slg1Sco
-00003020: 6d70 0000 0000 000b 16bf 0000 0005 0075  mp.............u
+00003020: 6d70 0000 0000 0004 5efa 0000 0005 0075  mp......^......u
 00003030: 0074 0069 006c 0073 6c73 7643 626c 6f62  .t.i.l.slsvCblob
 00003040: 0000 0297 6270 6c69 7374 3030 d801 0203  ....bplist00....
 00003050: 0405 0607 0809 0a0b 1949 4a0a 4c5f 1012  .........IJ.L_..
 00003060: 7669 6577 4f70 7469 6f6e 7356 6572 7369  viewOptionsVersi
 00003070: 6f6e 5f10 0f73 686f 7749 636f 6e50 7265  on_..showIconPre
 00003080: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
 00003090: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
@@ -848,20 +848,20 @@
 000034f0: 3b01 3c01 4501 4701 4801 4a01 4b01 5401  ;.<.E.G.H.J.K.T.
 00003500: 5601 5701 5901 5a01 6301 6501 6601 6801  V.W.Y.Z.c.e.f.h.
 00003510: 6901 7201 7401 7501 7701 7801 8101 8301  i.r.t.u.w.x.....
 00003520: 8401 8701 8801 9101 9201 9301 9401 9d01  ................
 00003530: a201 a300 0000 0000 0002 0100 0000 0000  ................
 00003540: 0000 4900 0000 0000 0000 0000 0000 0000  ..I.............
 00003550: 0001 ac00 0000 0500 7500 7400 6900 6c00  ........u.t.i.l.
-00003560: 736d 6f44 4462 6c6f 6200 0000 0893 f1b8  smoDDblob.......
-00003570: ea20 17c5 4100 0000 0500 7500 7400 6900  . ..A.....u.t.i.
-00003580: 6c00 736d 6f64 4462 6c6f 6200 0000 0893  l.smodDblob.....
-00003590: f1b8 ea20 17c5 4100 0000 0500 7500 7400  ... ..A.....u.t.
+00003560: 736d 6f44 4462 6c6f 6200 0000 08ec 99a1  smoDDblob.......
+00003570: b72d 17c5 4100 0000 0500 7500 7400 6900  .-..A.....u.t.i.
+00003580: 6c00 736d 6f64 4462 6c6f 6200 0000 08a7  l.smodDblob.....
+00003590: e9a3 f026 17c5 4100 0000 0500 7500 7400  ...&..A.....u.t.
 000035a0: 6900 6c00 7370 6831 5363 6f6d 7000 0000  i.l.sph1Scomp...
-000035b0: 0000 0cb0 0000 0000 0500 7500 7400 6900  ..........u.t.i.
+000035b0: 0000 0520 0000 0000 0500 7500 7400 6900  ... ......u.t.i.
 000035c0: 6c00 7376 5372 6e6c 6f6e 6700 0000 0100  l.svSrnlong.....
 000035d0: 0000 1000 7600 6900 6400 6500 6f00 5f00  ....v.i.d.e.o._.
 000035e0: 7000 7200 6f00 6300 6500 7300 7300 6f00  p.r.o.c.e.s.s.o.
 000035f0: 7200 7362 7773 7062 6c6f 6200 0000 c962  r.sbwspblob....b
 00003600: 706c 6973 7430 30d7 0102 0304 0506 0708  plist00.........
 00003610: 080a 080a 0d0a 5d53 686f 7753 7461 7475  ......]ShowStatu
 00003620: 7342 6172 5b53 686f 7750 6174 6862 6172  sBar[ShowPathbar
@@ -1460,16 +1460,16 @@
 00005b30: 0100 0000 0000 0000 4900 0000 0000 0000  ........I.......
 00005b40: 0000 0000 0000 0001 b400 0000 0f00 6400  ..............d.
 00005b50: 6100 7400 6100 5f00 7000 7200 6f00 6300  a.t.a._.p.r.o.c.
 00005b60: 6500 7300 7300 6f00 7200 736d 6f44 4462  e.s.s.o.r.smoDDb
 00005b70: 6c6f 6200 0000 0826 8880 05f4 11c5 4100  lob....&......A.
 00005b80: 0000 0f00 6400 6100 7400 6100 5f00 7000  ....d.a.t.a._.p.
 00005b90: 7200 6f00 6300 6500 7300 7300 6f00 7200  r.o.c.e.s.s.o.r.
-00005ba0: 736d 6f64 4462 6c6f 6200 0000 08b3 69d3  smodDblob.....i.
-00005bb0: 74cd 0fc5 4100 0000 0f00 6400 6100 7400  t...A.....d.a.t.
+00005ba0: 736d 6f64 4462 6c6f 6200 0000 0826 8880  smodDblob....&..
+00005bb0: 05f4 11c5 4100 0000 0f00 6400 6100 7400  ....A.....d.a.t.
 00005bc0: 6100 5f00 7000 7200 6f00 6300 6500 7300  a._.p.r.o.c.e.s.
 00005bd0: 7300 6f00 7200 7370 6831 5363 6f6d 7000  s.o.r.sph1Scomp.
 00005be0: 0000 0000 0480 0000 0000 0f00 6400 6100  ............d.a.
 00005bf0: 7400 6100 5f00 7000 7200 6f00 6300 6500  t.a._.p.r.o.c.e.
 00005c00: 7300 7300 6f00 7200 7376 5372 6e6c 6f6e  s.s.o.r.svSrnlon
 00005c10: 6700 0000 0100 0000 1200 6600 6500 6100  g.........f.e.a.
 00005c20: 7400 7500 7200 6500 5f00 6500 7800 7400  t.u.r.e._.e.x.t.
@@ -1489,15 +1489,15 @@
 00005d00: 000f 0000 0000 0000 0000 0000 0000 0000  ................
 00005d10: 009a 0000 0012 0066 0065 0061 0074 0075  .......f.e.a.t.u
 00005d20: 0072 0065 005f 0065 0078 0074 0072 0061  .r.e._.e.x.t.r.a
 00005d30: 0063 0074 006f 0072 0073 6473 636c 626f  .c.t.o.r.sdsclbo
 00005d40: 6f6c 0000 0000 1200 6600 6500 6100 7400  ol......f.e.a.t.
 00005d50: 7500 7200 6500 5f00 6500 7800 7400 7200  u.r.e._.e.x.t.r.
 00005d60: 6100 6300 7400 6f00 7200 736c 6731 5363  a.c.t.o.r.slg1Sc
-00005d70: 6f6d 7000 0000 0000 0904 0e09 5863 6f6d  omp.........Xcom
+00005d70: 6f6d 7000 0000 0000 0903 6409 5863 6f6d  omp.......d.Xcom
 00005d80: 6d65 6e74 73d4 0d0e 0f10 163e 1640 0810  ments......>.@..
 00005d90: c808 5e64 6174 654c 6173 744f 7065 6e65  ..^dateLastOpene
 00005da0: 64d4 0d0e 0f10 161c 1644 0808 5964 6174  d........D..Ydat
 00005db0: 6541 6464 6564 0823 4028 0000 0000 0000  eAdded.#@(......
 00005dc0: 546e 616d 6523 4030 0000 0000 0000 0900  Tname#@0........
 00005dd0: 0800 1900 2e00 4000 4800 5c00 6500 7000  ......@.H.\.e.p.
 00005de0: 7900 8c00 8e00 8f00 9b00 a400 ac00 b200  y...............
@@ -1700,71 +1700,71 @@
 00006a30: 4462 6c6f 6200 0000 0854 1422 3e3d 0fc5  Dblob....T.">=..
 00006a40: 4100 0000 0900 6c00 6100 6200 6500 6c00  A.....l.a.b.e.l.
 00006a50: 6c00 6900 6e00 6770 6831 5363 6f6d 7000  l.i.n.gph1Scomp.
 00006a60: 0000 0000 01e0 0000 0000 0900 6c00 6100  ............l.a.
 00006a70: 6200 6500 6c00 6c00 6900 6e00 6776 5372  b.e.l.l.i.n.gvSr
 00006a80: 6e6c 6f6e 6700 0000 0100 0000 0600 6d00  nlong.........m.
 00006a90: 6900 7800 6900 6e00 7362 7773 7062 6c6f  i.x.i.n.sbwspblo
-00006aa0: 6200 0000 c962 706c 6973 7430 30d7 0102  b....bplist00...
+00006aa0: 6200 0000 ca62 706c 6973 7430 30d7 0102  b....bplist00...
 00006ab0: 0304 0506 0708 080a 080a 0d0a 5d53 686f  ............]Sho
 00006ac0: 7753 7461 7475 7342 6172 5b53 686f 7750  wStatusBar[ShowP
 00006ad0: 6174 6862 6172 5b53 686f 7754 6f6f 6c62  athbar[ShowToolb
 00006ae0: 6172 5b53 686f 7754 6162 5669 6577 5f10  ar[ShowTabView_.
 00006af0: 1443 6f6e 7461 696e 6572 5368 6f77 5369  .ContainerShowSi
 00006b00: 6465 6261 725c 5769 6e64 6f77 426f 756e  debar\WindowBoun
 00006b10: 6473 5b53 686f 7753 6964 6562 6172 0808  ds[ShowSidebar..
-00006b20: 0908 095f 1018 7b7b 3330 372c 2038 367d  ..._..{{307, 86}
-00006b30: 2c20 7b31 3037 362c 2036 3231 7d7d 0908  , {1076, 621}}..
-00006b40: 1725 313d 4960 6d79 7a7b 7c7d 7e99 0000  .%1=I`myz{|}~...
-00006b50: 0000 0000 0101 0000 0000 0000 000f 0000  ................
-00006b60: 0000 0000 0000 0000 0000 0000 009a 0000  ................
-00006b70: 0006 006d 0069 0078 0069 006e 0073 6c67  ...m.i.x.i.n.slg
-00006b80: 3153 636f 6d70 0000 0000 0009 f692 0000  1Scomp..........
-00006b90: 0006 006d 0069 0078 0069 006e 0073 6c73  ...m.i.x.i.n.sls
-00006ba0: 7643 626c 6f62 0000 0281 6270 6c69 7374  vCblob....bplist
-00006bb0: 3030 d801 0203 0405 0607 0809 0a0b 1646  00.............F
-00006bc0: 4748 0a5f 1012 7669 6577 4f70 7469 6f6e  GH._..viewOption
-00006bd0: 7356 6572 7369 6f6e 5f10 0f73 686f 7749  sVersion_..showI
-00006be0: 636f 6e50 7265 7669 6577 5763 6f6c 756d  conPreviewWcolum
-00006bf0: 6e73 5f10 1163 616c 6375 6c61 7465 416c  ns_..calculateAl
-00006c00: 6c53 697a 6573 5874 6578 7453 697a 655a  lSizesXtextSizeZ
-00006c10: 736f 7274 436f 6c75 6d6e 5869 636f 6e53  sortColumnXiconS
-00006c20: 697a 655f 1010 7573 6552 656c 6174 6976  ize_..useRelativ
-00006c30: 6544 6174 6573 1001 09ab 0c15 1a1f 2328  eDates........#(
-00006c40: 2d32 373c 41d4 0d0e 0f10 1112 0a0a 5a69  -27<A.........Zi
-00006c50: 6465 6e74 6966 6965 7255 7769 6474 6859  dentifierUwidthY
-00006c60: 6173 6365 6e64 696e 6757 7669 7369 626c  ascendingWvisibl
-00006c70: 6554 6e61 6d65 1101 c709 09d4 100e 0f0d  eTname..........
-00006c80: 1617 1619 0810 2308 5875 6269 7175 6974  ......#.Xubiquit
-00006c90: 79d4 0d0e 0f10 1b1c 160a 5c64 6174 654d  y.........\dateM
-00006ca0: 6f64 6966 6965 6410 b508 09d4 0d0e 0f10  odified.........
-00006cb0: 201c 1616 5b64 6174 6543 7265 6174 6564   ...[dateCreated
-00006cc0: 0808 d40d 0e0f 1024 2516 0a54 7369 7a65  .......$%..Tsize
-00006cd0: 1061 0809 d40d 0e0f 1029 2a0a 0a54 6b69  .a.......)*..Tki
-00006ce0: 6e64 1073 0909 d40d 0e0f 102e 2f0a 1655  nd.s......../..U
-00006cf0: 6c61 6265 6c10 6409 08d4 0d0e 0f10 3334  label.d.......34
-00006d00: 0a16 5776 6572 7369 6f6e 104b 0908 d40d  ..Wversion.K....
-00006d10: 0e0f 1038 390a 1658 636f 6d6d 656e 7473  ...89..Xcomments
-00006d20: 1101 2c09 08d4 0d0e 0f10 3d3e 1616 5e64  ..,.......=>..^d
-00006d30: 6174 654c 6173 744f 7065 6e65 6410 c808  ateLastOpened...
-00006d40: 08d4 100e 0f0d 161c 1644 0808 5964 6174  .........D..Ydat
-00006d50: 6541 6464 6564 0823 4028 0000 0000 0000  eAdded.#@(......
-00006d60: 5c64 6174 654d 6f64 6966 6965 6423 4030  \dateModified#@0
-00006d70: 0000 0000 0000 0900 0800 1900 2e00 4000  ..............@.
-00006d80: 4800 5c00 6500 7000 7900 8c00 8e00 8f00  H.\.e.p.y.......
-00006d90: 9b00 a400 af00 b500 bf00 c700 cc00 cf00  ................
-00006da0: d000 d100 da00 db00 dd00 de00 e700 f000  ................
-00006db0: fd00 ff01 0001 0101 0a01 1601 1701 1801  ................
-00006dc0: 2101 2601 2801 2901 2a01 3301 3801 3a01  !.&.(.).*.3.8.:.
-00006dd0: 3b01 3c01 4501 4b01 4d01 4e01 4f01 5801  ;.<.E.K.M.N.O.X.
-00006de0: 6001 6201 6301 6401 6d01 7601 7901 7a01  `.b.c.d.m.v.y.z.
-00006df0: 7b01 8401 9301 9501 9601 9701 a001 a101  {...............
-00006e00: a201 ac01 ad01 b601 c301 cc00 0000 0000  ................
-00006e10: 0002 0100 0000 0000 0000 4a00 0000 0000  ..........J.....
-00006e20: 0000 0000 0000 0000 0001 cd01 4501 4601  ............E.F.
+00006b20: 0908 095f 1019 7b7b 3930 372c 2034 3536  ..._..{{907, 456
+00006b30: 7d2c 207b 3130 3736 2c20 3632 317d 7d09  }, {1076, 621}}.
+00006b40: 0817 2531 3d49 606d 797a 7b7c 7d7e 9a00  ..%1=I`myz{|}~..
+00006b50: 0000 0000 0001 0100 0000 0000 0000 0f00  ................
+00006b60: 0000 0000 0000 0000 0000 0000 0000 9b00  ................
+00006b70: 0000 0600 6d00 6900 7800 6900 6e00 736c  ....m.i.x.i.n.sl
+00006b80: 6731 5363 6f6d 7000 0000 0000 09ff ab00  g1Scomp.........
+00006b90: 0000 0600 6d00 6900 7800 6900 6e00 736c  ....m.i.x.i.n.sl
+00006ba0: 7376 4362 6c6f 6200 0002 8162 706c 6973  svCblob....bplis
+00006bb0: 7430 30d8 0102 0304 0506 0708 090a 0b16  t00.............
+00006bc0: 4647 480a 5f10 1276 6965 774f 7074 696f  FGH._..viewOptio
+00006bd0: 6e73 5665 7273 696f 6e5f 100f 7368 6f77  nsVersion_..show
+00006be0: 4963 6f6e 5072 6576 6965 7757 636f 6c75  IconPreviewWcolu
+00006bf0: 6d6e 735f 1011 6361 6c63 756c 6174 6541  mns_..calculateA
+00006c00: 6c6c 5369 7a65 7358 7465 7874 5369 7a65  llSizesXtextSize
+00006c10: 5a73 6f72 7443 6f6c 756d 6e58 6963 6f6e  ZsortColumnXicon
+00006c20: 5369 7a65 5f10 1075 7365 5265 6c61 7469  Size_..useRelati
+00006c30: 7665 4461 7465 7310 0109 ab0c 151a 1f23  veDates........#
+00006c40: 282d 3237 3c41 d40d 0e0f 1011 120a 0a5a  (-27<A.........Z
+00006c50: 6964 656e 7469 6669 6572 5577 6964 7468  identifierUwidth
+00006c60: 5961 7363 656e 6469 6e67 5776 6973 6962  YascendingWvisib
+00006c70: 6c65 546e 616d 6511 01c7 0909 d410 0e0f  leTname.........
+00006c80: 0d16 1716 1908 1023 0858 7562 6971 7569  .......#.Xubiqui
+00006c90: 7479 d40d 0e0f 101b 1c16 0a5c 6461 7465  ty.........\date
+00006ca0: 4d6f 6469 6669 6564 10b5 0809 d40d 0e0f  Modified........
+00006cb0: 1020 1c16 165b 6461 7465 4372 6561 7465  . ...[dateCreate
+00006cc0: 6408 08d4 0d0e 0f10 2425 160a 5473 697a  d.......$%..Tsiz
+00006cd0: 6510 6108 09d4 0d0e 0f10 292a 0a0a 546b  e.a.......)*..Tk
+00006ce0: 696e 6410 7309 09d4 0d0e 0f10 2e2f 0a16  ind.s......../..
+00006cf0: 556c 6162 656c 1064 0908 d40d 0e0f 1033  Ulabel.d.......3
+00006d00: 340a 1657 7665 7273 696f 6e10 4b09 08d4  4..Wversion.K...
+00006d10: 0d0e 0f10 3839 0a16 5863 6f6d 6d65 6e74  ....89..Xcomment
+00006d20: 7311 012c 0908 d40d 0e0f 103d 3e16 165e  s..,.......=>..^
+00006d30: 6461 7465 4c61 7374 4f70 656e 6564 10c8  dateLastOpened..
+00006d40: 0808 d410 0e0f 0d16 1c16 4408 0859 6461  ..........D..Yda
+00006d50: 7465 4164 6465 6408 2340 2800 0000 0000  teAdded.#@(.....
+00006d60: 005c 6461 7465 4d6f 6469 6669 6564 2340  .\dateModified#@
+00006d70: 3000 0000 0000 0009 0008 0019 002e 0040  0..............@
+00006d80: 0048 005c 0065 0070 0079 008c 008e 008f  .H.\.e.p.y......
+00006d90: 009b 00a4 00af 00b5 00bf 00c7 00cc 00cf  ................
+00006da0: 00d0 00d1 00da 00db 00dd 00de 00e7 00f0  ................
+00006db0: 00fd 00ff 0100 0101 010a 0116 0117 0118  ................
+00006dc0: 0121 0126 0128 0129 012a 0133 0138 013a  .!.&.(.).*.3.8.:
+00006dd0: 013b 013c 0145 014b 014d 014e 014f 0158  .;.<.E.K.M.N.O.X
+00006de0: 0160 0162 0163 0164 016d 0176 0179 017a  .`.b.c.d.m.v.y.z
+00006df0: 017b 0184 0193 0195 0196 0197 01a0 01a1  .{..............
+00006e00: 01a2 01ac 01ad 01b6 01c3 01cc 0000 0000  ................
+00006e10: 0000 0201 0000 0000 0000 004a 0000 0000  ...........J....
+00006e20: 0000 0000 0000 0000 0000 01cd 4501 4601  ............E.F.
 00006e30: 4801 4901 4f01 5801 5901 5b01 5c01 6401  H.I.O.X.Y.[.\.d.
 00006e40: 6d01 6e01 7101 7201 7b01 8401 8501 8701  m.n.q.r.{.......
 00006e50: 8801 9701 a001 a101 a201 ac01 ad01 b601  ................
 00006e60: bb01 c400 0000 0000 0002 0100 0000 0000  ................
 00006e70: 0000 4a00 0000 0000 0000 0000 0000 0000  ..J.............
 00006e80: 0001 c500 0000 0000 0000 0000 0000 0000  ................
 00006e90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -1788,20 +1788,20 @@
 00006fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00006ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007000: 0000 0000 0000 0000 0000 0016 0000 0006  ................
 00007010: 006d 0069 0078 0069 006e 0073 6d6f 4444  .m.i.x.i.n.smoDD
-00007020: 626c 6f62 0000 0008 c6dc 83c4 8916 c541  blob...........A
+00007020: 626c 6f62 0000 0008 9aa5 fb6f 3817 c541  blob.......o8..A
 00007030: 0000 0006 006d 0069 0078 0069 006e 0073  .....m.i.x.i.n.s
-00007040: 6d6f 6444 626c 6f62 0000 0008 c6dc 83c4  modDblob........
-00007050: 8916 c541 0000 0006 006d 0069 0078 0069  ...A.....m.i.x.i
+00007040: 6d6f 6444 626c 6f62 0000 0008 9aa5 fb6f  modDblob.......o
+00007050: 3817 c541 0000 0006 006d 0069 0078 0069  8..A.....m.i.x.i
 00007060: 006e 0073 7068 3153 636f 6d70 0000 0000  .n.sph1Scomp....
-00007070: 000a d000 0000 0006 006d 0069 0078 0069  .........m.i.x.i
+00007070: 000a e000 0000 0006 006d 0069 0078 0069  .........m.i.x.i
 00007080: 006e 0073 7653 726e 6c6f 6e67 0000 0001  .n.svSrnlong....
 00007090: 0000 0005 006d 006f 0064 0065 006c 6277  .....m.o.d.e.lbw
 000070a0: 7370 626c 6f62 0000 00c9 6270 6c69 7374  spblob....bplist
 000070b0: 3030 d701 0203 0405 0607 0808 0a08 0a0d  00..............
 000070c0: 0a5d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
 000070d0: 5368 6f77 5061 7468 6261 725b 5368 6f77  ShowPathbar[Show
 000070e0: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
@@ -1810,16 +1810,16 @@
 00007110: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
 00007120: 6261 7208 0809 0809 5f10 187b 7b33 3037  bar....._..{{307
 00007130: 2c20 3836 7d2c 207b 3130 3736 2c20 3632  , 86}, {1076, 62
 00007140: 317d 7d09 0817 2531 3d49 606d 797a 7b7c  1}}...%1=I`myz{|
 00007150: 7d7e 9900 0000 0000 0001 0100 0000 0000  }~..............
 00007160: 0000 0f00 0000 0000 0000 0000 0000 0000  ................
 00007170: 0000 9a00 0000 0500 6d00 6f00 6400 6500  ........m.o.d.e.
-00007180: 6c6c 6731 5363 6f6d 7000 0000 0000 012d  llg1Scomp......-
-00007190: 2600 0000 0500 6d00 6f00 6400 6500 6c6c  &.....m.o.d.e.ll
+00007180: 6c6c 6731 5363 6f6d 7000 0000 0000 013b  llg1Scomp......;
+00007190: 6b00 0000 0500 6d00 6f00 6400 6500 6c6c  k.....m.o.d.e.ll
 000071a0: 7376 4362 6c6f 6200 0002 7962 706c 6973  svCblob...ybplis
 000071b0: 7430 30d8 0102 0304 0506 0708 090a 0b18  t00.............
 000071c0: 4647 0a49 5869 636f 6e53 697a 655f 100f  FG.IXiconSize_..
 000071d0: 7368 6f77 4963 6f6e 5072 6576 6965 7757  showIconPreviewW
 000071e0: 636f 6c75 6d6e 735f 1011 6361 6c63 756c  columns_..calcul
 000071f0: 6174 6541 6c6c 5369 7a65 7358 7465 7874  ateAllSizesXtext
 00007200: 5369 7a65 5a73 6f72 7443 6f6c 756d 6e5f  SizeZsortColumn_
@@ -1893,19 +1893,19 @@
 00007640: 014e 0150 0159 015a 015b 015d 015f 0168  .N.P.Y.Z.[.]._.h
 00007650: 0169 016a 016c 016e 0177 0178 0179 017b  .i.j.l.n.w.x.y.{
 00007660: 017d 0186 0187 0188 018a 018c 0195 0196  .}..............
 00007670: 0197 019a 019c 019d 01a6 01ab 0000 0000  ................
 00007680: 0000 0201 0000 0000 0000 0049 0000 0000  ...........I....
 00007690: 0000 0000 0000 0000 0000 01ac 0000 0005  ................
 000076a0: 006d 006f 0064 0065 006c 6d6f 4444 626c  .m.o.d.e.lmoDDbl
-000076b0: 6f62 0000 0008 e0f6 2f65 6714 c541 0000  ob....../eg..A..
+000076b0: 6f62 0000 0008 fe1b 754c 3217 c541 0000  ob......uL2..A..
 000076c0: 0005 006d 006f 0064 0065 006c 6d6f 6444  ...m.o.d.e.lmodD
-000076d0: 626c 6f62 0000 0008 32f5 d3ed cc0c c541  blob....2......A
+000076d0: 626c 6f62 0000 0008 fe1b 754c 3217 c541  blob......uL2..A
 000076e0: 0000 0005 006d 006f 0064 0065 006c 7068  .....m.o.d.e.lph
-000076f0: 3153 636f 6d70 0000 0000 0001 6000 0000  1Scomp......`...
+000076f0: 3153 636f 6d70 0000 0000 0001 7000 0000  1Scomp......p...
 00007700: 0005 006d 006f 0064 0065 006c 7653 726e  ...m.o.d.e.lvSrn
 00007710: 6c6f 6e67 0000 0001 0000 000d 006f 0075  long.........o.u
 00007720: 0074 006c 0069 0065 0072 005f 0074 006f  .t.l.i.e.r._.t.o
 00007730: 006f 006c 0073 6277 7370 626c 6f62 0000  .o.l.sbwspblob..
 00007740: 00ca 6270 6c69 7374 3030 d701 0203 0405  ..bplist00......
 00007750: 0607 0808 0a08 0a0d 0a5d 5368 6f77 5374  .........]ShowSt
 00007760: 6174 7573 4261 725b 5368 6f77 5061 7468  atusBar[ShowPath
@@ -2012,16 +2012,16 @@
 00007db0: d301 d400 0000 0000 0002 0100 0000 0000  ................
 00007dc0: 0000 4c00 0000 0000 0000 0000 0000 0000  ..L.............
 00007dd0: 0001 dd00 0000 0d00 6f00 7500 7400 6c00  ........o.u.t.l.
 00007de0: 6900 6500 7200 5f00 7400 6f00 6f00 6c00  i.e.r._.t.o.o.l.
 00007df0: 736d 6f44 4462 6c6f 6200 0000 08aa 2e11  smoDDblob.......
 00007e00: 6564 14c5 4100 0000 0d00 6f00 7500 7400  ed..A.....o.u.t.
 00007e10: 6c00 6900 6500 7200 5f00 7400 6f00 6f00  l.i.e.r._.t.o.o.
-00007e20: 6c00 736d 6f64 4462 6c6f 6200 0000 08be  l.smodDblob.....
-00007e30: a6cf edcc 0cc5 4100 0000 0d00 6f00 7500  ......A.....o.u.
+00007e20: 6c00 736d 6f64 4462 6c6f 6200 0000 08aa  l.smodDblob.....
+00007e30: 2e11 6564 14c5 4100 0000 0d00 6f00 7500  ..ed..A.....o.u.
 00007e40: 7400 6c00 6900 6500 7200 5f00 7400 6f00  t.l.i.e.r._.t.o.
 00007e50: 6f00 6c00 7370 6831 5363 6f6d 7000 0000  o.l.sph1Scomp...
 00007e60: 0000 0150 0000 0000 0d00 6f00 7500 7400  ...P......o.u.t.
 00007e70: 6c00 6900 6500 7200 5f00 7400 6f00 6f00  l.i.e.r._.t.o.o.
 00007e80: 6c00 7376 5372 6e6c 6f6e 6700 0000 0100  l.svSrnlong.....
 00007e90: 0000 0800 7000 6c00 6f00 7400 7400 6900  ....p.l.o.t.t.i.
 00007ea0: 6e00 6762 7773 7062 6c6f 6200 0000 ca62  n.gbwspblob....b
@@ -2035,15 +2035,15 @@
 00007f20: 7753 6964 6562 6172 0808 0908 095f 1019  wSidebar....._..
 00007f30: 7b7b 3238 372c 2031 3036 7d2c 207b 3130  {{287, 106}, {10
 00007f40: 3736 2c20 3632 317d 7d09 0817 2531 3d49  76, 621}}...%1=I
 00007f50: 606d 797a 7b7c 7d7e 9a00 0000 0000 0001  `myz{|}~........
 00007f60: 0100 0000 0000 0000 0f00 0000 0000 0000  ................
 00007f70: 0000 0000 0000 0000 9b00 0000 0800 7000  ..............p.
 00007f80: 6c00 6f00 7400 7400 6900 6e00 676c 6731  l.o.t.t.i.n.glg1
-00007f90: 5363 6f6d 7000 0000 0000 08c2 1e00 0000  Scomp...........
+00007f90: 5363 6f6d 7000 0000 0000 08c5 3600 0000  Scomp.......6...
 00007fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00007ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008000: 0000 0000 0000 0000 0000 0015 0000 0008  ................
@@ -2088,18 +2088,18 @@
 00008270: 7a01 7c01 7d01 7e01 8701 8901 8b01 8c01  z.|.}.~.........
 00008280: 8d01 9601 9801 9a01 9b01 9c01 a501 a701  ................
 00008290: a901 aa01 ab01 b401 b601 b901 ba01 bb01  ................
 000082a0: bc01 c501 ce01 db01 e400 0000 0000 0002  ................
 000082b0: 0100 0000 0000 0000 4c00 0000 0000 0000  ........L.......
 000082c0: 0000 0000 0000 0001 e500 0000 0800 7000  ..............p.
 000082d0: 6c00 6f00 7400 7400 6900 6e00 676d 6f44  l.o.t.t.i.n.gmoD
-000082e0: 4462 6c6f 6200 0000 08c4 1ccf bcd8 13c5  Dblob...........
+000082e0: 4462 6c6f 6200 0000 08a5 6a92 865a 16c5  Dblob.....j..Z..
 000082f0: 4100 0000 0800 7000 6c00 6f00 7400 7400  A.....p.l.o.t.t.
 00008300: 6900 6e00 676d 6f64 4462 6c6f 6200 0000  i.n.gmodDblob...
-00008310: 08e6 e1c8 639f 12c5 4100 0000 0800 7000  ....c...A.....p.
+00008310: 08a5 6a92 865a 16c5 4100 0000 0800 7000  ..j..Z..A.....p.
 00008320: 6c00 6f00 7400 7400 6900 6e00 6770 6831  l.o.t.t.i.n.gph1
 00008330: 5363 6f6d 7000 0000 0000 0ae0 0000 0000  Scomp...........
 00008340: 0800 7000 6c00 6f00 7400 7400 6900 6e00  ..p.l.o.t.t.i.n.
 00008350: 6776 5372 6e6c 6f6e 6700 0000 0100 0000  gvSrnlong.......
 00008360: 1300 7000 6f00 7300 6500 5f00 6300 6f00  ..p.o.s.e._.c.o.
 00008370: 6e00 6600 6900 6700 7500 7200 6100 7400  n.f.i.g.u.r.a.t.
 00008380: 6900 6f00 6e00 7362 7773 7062 6c6f 6200  i.o.n.sbwspblob.
@@ -2268,16 +2268,16 @@
 00008db0: 626f 6f6c 0000 0000 0e00 7000 6f00 7300  bool......p.o.s.
 00008dc0: 6500 5f00 6900 6d00 7000 6f00 7200 7400  e._.i.m.p.o.r.t.
 00008dd0: 6500 7200 736c 6731 5363 6f6d 7000 0000  e.r.slg1Scomp...
 00008de0: 0000 020c 7a00 5f00 7400 6f00 6f00 6c00  ....z._.t.o.o.l.
 00008df0: 736d 6f44 4462 6c6f 6200 0000 08aa 2e11  smoDDblob.......
 00008e00: 6564 14c5 4100 0000 0d00 6f00 7500 7400  ed..A.....o.u.t.
 00008e10: 6c00 6900 6500 7200 5f00 7400 6f00 6f00  l.i.e.r._.t.o.o.
-00008e20: 6c00 736d 6f64 4462 6c6f 6200 0000 08be  l.smodDblob.....
-00008e30: a6cf edcc 0cc5 4100 0000 0d00 6f00 7500  ......A.....o.u.
+00008e20: 6c00 736d 6f64 4462 6c6f 6200 0000 08aa  l.smodDblob.....
+00008e30: 2e11 6564 14c5 4100 0000 0d00 6f00 7500  ..ed..A.....o.u.
 00008e40: 7400 6c00 6900 6500 7200 5f00 7400 6f00  t.l.i.e.r._.t.o.
 00008e50: 6f00 6c00 7370 6831 5363 6f6d 7000 0000  o.l.sph1Scomp...
 00008e60: 0000 0150 0000 0000 0d00 6f00 7500 7400  ...P......o.u.t.
 00008e70: 6c00 6900 6500 7200 5f00 7400 6f00 6f00  l.i.e.r._.t.o.o.
 00008e80: 6c00 7376 5372 6e6c 6f6e 6700 0000 0100  l.svSrnlong.....
 00008e90: 0000 0800 7000 6c00 6f00 7400 7400 6900  ....p.l.o.t.t.i.
 00008ea0: 6e00 6762 7773 7062 6c6f 6200 0000 ca62  n.gbwspblob....b
@@ -2291,15 +2291,15 @@
 00008f20: 7753 6964 6562 6172 0808 0908 095f 1019  wSidebar....._..
 00008f30: 7b7b 3238 372c 2031 3036 7d2c 207b 3130  {{287, 106}, {10
 00008f40: 3736 2c20 3632 317d 7d09 0817 2531 3d49  76, 621}}...%1=I
 00008f50: 606d 797a 7b7c 7d7e 9a00 0000 0000 0001  `myz{|}~........
 00008f60: 0100 0000 0000 0000 0f00 0000 0000 0000  ................
 00008f70: 0000 0000 0000 0000 9b00 0000 0800 7000  ..............p.
 00008f80: 6c00 6f00 7400 7400 6900 6e00 676c 6731  l.o.t.t.i.n.glg1
-00008f90: 5363 6f6d 7000 0000 0000 08c2 1e00 0000  Scomp...........
+00008f90: 5363 6f6d 7000 0000 0000 08c5 3600 0000  Scomp.......6...
 00008fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00008ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009000: 0000 0000 0000 0000 0000 0010 0000 000e  ................
@@ -2547,15 +2547,15 @@
 00009f20: 7753 6964 6562 6172 0808 0908 095f 1019  wSidebar....._..
 00009f30: 7b7b 3238 372c 2031 3036 7d2c 207b 3130  {{287, 106}, {10
 00009f40: 3736 2c20 3632 317d 7d09 0817 2531 3d49  76, 621}}...%1=I
 00009f50: 606d 797a 7b7c 7d7e 9a00 0000 0000 0001  `myz{|}~........
 00009f60: 0100 0000 0000 0000 0f00 0000 0000 0000  ................
 00009f70: 0000 0000 0000 0000 9b00 0000 0800 7000  ..............p.
 00009f80: 6c00 6f00 7400 7400 6900 6e00 676c 6731  l.o.t.t.i.n.glg1
-00009f90: 5363 6f6d 7000 0000 0000 08c2 1e00 0000  Scomp...........
+00009f90: 5363 6f6d 7000 0000 0000 08c5 3600 0000  Scomp.......6...
 00009fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00009ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000a000: 0000 0000 0000 0000 0000 0014 0000 0009  ................
@@ -2707,15 +2707,15 @@
 0000a920: 0908 095f 1019 7b7b 3335 342c 2031 3234  ..._..{{354, 124
 0000a930: 7d2c 207b 3130 3736 2c20 3632 317d 7d09  }, {1076, 621}}.
 0000a940: 0817 2531 3d49 606d 797a 7b7c 7d7e 9a00  ..%1=I`myz{|}~..
 0000a950: 0000 0000 0001 0100 0000 0000 0000 0f00  ................
 0000a960: 0000 0000 0000 0000 0000 0000 0000 9b00  ................
 0000a970: 0000 0200 7500 6964 7363 6c62 6f6f 6c00  ....u.idsclbool.
 0000a980: 0000 0002 0075 0069 6c67 3153 636f 6d70  .....u.ilg1Scomp
-0000a990: 0000 0000 0009 736b 0000 0002 0075 0069  ......sk.....u.i
+0000a990: 0000 0000 0009 7bb3 0000 0002 0075 0069  ......{......u.i
 0000a9a0: 6c73 7643 626c 6f62 0000 0279 6270 6c69  lsvCblob...ybpli
 0000a9b0: 7374 3030 d801 0203 0405 0607 0809 0a0b  st00............
 0000a9c0: 1846 4748 0a5f 1012 7669 6577 4f70 7469  .FGH._..viewOpti
 0000a9d0: 6f6e 7356 6572 7369 6f6e 5f10 0f73 686f  onsVersion_..sho
 0000a9e0: 7749 636f 6e50 7265 7669 6577 5763 6f6c  wIconPreviewWcol
 0000a9f0: 756d 6e73 5f10 1163 616c 6375 6c61 7465  umns_..calculate
 0000aa00: 416c 6c53 697a 6573 5874 6578 7453 697a  AllSizesXtextSiz
@@ -2788,30 +2788,30 @@
 0000ae30: 3701 3801 3a01 4301 4401 4501 4701 5001  7.8.:.C.D.E.G.P.
 0000ae40: 5101 5201 5401 5601 5f01 6001 6101 6301  Q.R.T.V._.`.a.c.
 0000ae50: 6501 6e01 6f01 7001 7201 7401 7d01 7e01  e.n.o.p.r.t.}.~.
 0000ae60: 7f01 8101 8301 8c01 8e01 9101 9201 9301  ................
 0000ae70: 9401 9d01 a201 ab00 0000 0000 0002 0100  ................
 0000ae80: 0000 0000 0000 4900 0000 0000 0000 0000  ......I.........
 0000ae90: 0000 0000 0001 ac00 0000 0200 7500 696d  ............u.im
-0000aea0: 6f44 4462 6c6f 6200 0000 0841 e3d5 bf76  oDDblob....A...v
-0000aeb0: 0ec5 4100 0000 0200 7500 696d 6f64 4462  ..A.....u.imodDb
+0000aea0: 6f44 4462 6c6f 6200 0000 08f4 67a2 b72d  oDDblob.....g..-
+0000aeb0: 17c5 4100 0000 0200 7500 696d 6f64 4462  ..A.....u.imodDb
 0000aec0: 6c6f 6200 0000 0841 e3d5 bf76 0ec5 4100  lob....A...v..A.
 0000aed0: 0000 0200 7500 6970 6831 5363 6f6d 7000  ....u.iph1Scomp.
 0000aee0: 0000 0000 0c90 006f 6c62 6172 5b53 686f  .......olbar[Sho
 0000aef0: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
 0000af00: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
 0000af10: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
 0000af20: 7753 6964 6562 6172 0808 0908 095f 1019  wSidebar....._..
 0000af30: 7b7b 3238 372c 2031 3036 7d2c 207b 3130  {{287, 106}, {10
 0000af40: 3736 2c20 3632 317d 7d09 0817 2531 3d49  76, 621}}...%1=I
 0000af50: 606d 797a 7b7c 7d7e 9a00 0000 0000 0001  `myz{|}~........
 0000af60: 0100 0000 0000 0000 0f00 0000 0000 0000  ................
 0000af70: 0000 0000 0000 0000 9b00 0000 0800 7000  ..............p.
 0000af80: 6c00 6f00 7400 7400 6900 6e00 676c 6731  l.o.t.t.i.n.glg1
-0000af90: 5363 6f6d 7000 0000 0000 08c2 1e00 0000  Scomp...........
+0000af90: 5363 6f6d 7000 0000 0000 08c5 3600 0000  Scomp.......6...
 0000afa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000afb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000afc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000afd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000afe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000aff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000b000: 0000 0000 0000 0000 0000 000a 0000 000c  ................
@@ -2963,15 +2963,15 @@
 0000b920: 0908 095f 1019 7b7b 3335 342c 2031 3234  ..._..{{354, 124
 0000b930: 7d2c 207b 3130 3736 2c20 3632 317d 7d09  }, {1076, 621}}.
 0000b940: 0817 2531 3d49 606d 797a 7b7c 7d7e 9a00  ..%1=I`myz{|}~..
 0000b950: 0000 0000 0001 0100 0000 0000 0000 0f00  ................
 0000b960: 0000 0000 0000 0000 0000 0000 0000 9b00  ................
 0000b970: 0000 0200 7500 6964 7363 6c62 6f6f 6c00  ....u.idsclbool.
 0000b980: 0000 0002 0075 0069 6c67 3153 636f 6d70  .....u.ilg1Scomp
-0000b990: 0000 0000 0009 736b 0000 0002 0075 0069  ......sk.....u.i
+0000b990: 0000 0000 0009 7bb3 0000 0002 0075 0069  ......{......u.i
 0000b9a0: 6c73 7643 626c 6f62 0000 0279 6270 6c69  lsvCblob...ybpli
 0000b9b0: 7374 3030 d801 0203 0405 0607 0809 0a0b  st00............
 0000b9c0: 1846 4748 0a5f 1012 7669 6577 4f70 7469  .FGH._..viewOpti
 0000b9d0: 6f6e 7356 6572 7369 6f6e 5f10 0f73 686f  onsVersion_..sho
 0000b9e0: 7749 636f 6e50 7265 7669 6577 5763 6f6c  wIconPreviewWcol
 0000b9f0: 756d 6e73 5f10 1163 616c 6375 6c61 7465  umns_..calculate
 0000ba00: 416c 6c53 697a 6573 5874 6578 7453 697a  AllSizesXtextSiz
@@ -3044,30 +3044,30 @@
 0000be30: 3701 3801 3a01 4301 4401 4501 4701 5001  7.8.:.C.D.E.G.P.
 0000be40: 5101 5201 5401 5601 5f01 6001 6101 6301  Q.R.T.V._.`.a.c.
 0000be50: 6501 6e01 6f01 7001 7201 7401 7d01 7e01  e.n.o.p.r.t.}.~.
 0000be60: 7f01 8101 8301 8c01 8e01 9101 9201 9301  ................
 0000be70: 9401 9d01 a201 ab00 0000 0000 0002 0100  ................
 0000be80: 0000 0000 0000 4900 0000 0000 0000 0000  ......I.........
 0000be90: 0000 0000 0001 ac00 0000 0200 7500 696d  ............u.im
-0000bea0: 6f44 4462 6c6f 6200 0000 0841 e3d5 bf76  oDDblob....A...v
-0000beb0: 0ec5 4100 0000 0200 7500 696d 6f64 4462  ..A.....u.imodDb
+0000bea0: 6f44 4462 6c6f 6200 0000 08f4 67a2 b72d  oDDblob.....g..-
+0000beb0: 17c5 4100 0000 0200 7500 696d 6f64 4462  ..A.....u.imodDb
 0000bec0: 6c6f 6200 0000 0841 e3d5 bf76 0ec5 4100  lob....A...v..A.
 0000bed0: 0000 0200 7500 6970 6831 5363 6f6d 7000  ....u.iph1Scomp.
 0000bee0: 0000 0000 0c90 006f 6c62 6172 5b53 686f  .......olbar[Sho
 0000bef0: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
 0000bf00: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
 0000bf10: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
 0000bf20: 7753 6964 6562 6172 0808 0908 095f 1019  wSidebar....._..
 0000bf30: 7b7b 3238 372c 2031 3036 7d2c 207b 3130  {{287, 106}, {10
 0000bf40: 3736 2c20 3632 317d 7d09 0817 2531 3d49  76, 621}}...%1=I
 0000bf50: 606d 797a 7b7c 7d7e 9a00 0000 0000 0001  `myz{|}~........
 0000bf60: 0100 0000 0000 0000 0f00 0000 0000 0000  ................
 0000bf70: 0000 0000 0000 0000 9b00 0000 0800 7000  ..............p.
 0000bf80: 6c00 6f00 7400 7400 6900 6e00 676c 6731  l.o.t.t.i.n.glg1
-0000bf90: 5363 6f6d 7000 0000 0000 08c2 1e00 0000  Scomp...........
+0000bf90: 5363 6f6d 7000 0000 0000 08c5 3600 0000  Scomp.......6...
 0000bfa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000bfb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000bfc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000bfd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000bfe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000bff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 0000c000: 0000 0000                                ....
```

### Comparing `Simba-UW-tf-dev-1.62.7/simba/feature_extractors/feature_extractor_14bp.py` & `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/feature_extractor_14bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/feature_extractors/feature_extractor_7bp.py` & `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/feature_extractor_7bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/doctests.py` & `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/doctests.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py` & `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/read_in_mp.py` & `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/read_in_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/peaks.py` & `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/peaks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/fish_feature_extractor_2022.py` & `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/fish_feature_extractor_2022.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/convex_hull_3_scratch_3.py` & `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/convex_hull_3_scratch_3.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/convex_hull_scratch_1.py` & `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/convex_hull_scratch_1.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/.DS_Store` & `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py` & `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/egocentrical_aligner.py` & `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/egocentrical_aligner.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/count_values_in_range.py` & `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/count_values_in_range.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/graph_creator.py` & `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/graph_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/termite_rois.csv` & `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/termite_rois.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/mutual_exclusive.py` & `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/mutual_exclusive.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/video_color.py` & `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/video_color.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/graph_3d_plotter.py` & `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/graph_3d_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/shap_log_mp_2.py` & `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/shap_log_mp_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/video_rotator.py` & `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/video_rotator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/shap_log_mp.py` & `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/shap_log_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/add_probability_cnt_features.py` & `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/add_probability_cnt_features.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/make_splash.py` & `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/make_splash.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py` & `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_5.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/time_stamp_calculator.py` & `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/time_stamp_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/video_rotator_mp.py` & `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/video_rotator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/read_files_mp_2.py` & `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/read_files_mp_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py` & `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/fish_feature_extractor_2023_version_4.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/feature_extractors/misc/convex_hull_scratch_2.py` & `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/misc/convex_hull_scratch_2.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/feature_extractors/feature_extractor_8bps_2_animals.py` & `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/feature_extractor_8bps_2_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/feature_extractors/.DS_Store` & `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/feature_extractors/perimeter_jit.py` & `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/perimeter_jit.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/feature_extractors/feature_subsets.py` & `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/feature_subsets.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/feature_extractors/feature_extractor_user_defined.py` & `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/feature_extractor_user_defined.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/feature_extractors/feature_extractor_16bp.py` & `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/feature_extractor_16bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/feature_extractors/feature_extractor_9bp.py` & `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/feature_extractor_9bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/feature_extractors/feature_extractor_8bp.py` & `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/feature_extractor_8bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/feature_extractors/feature_extractor_4bp.py` & `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/feature_extractor_4bp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/feature_extractors/.idea/features_scripts.iml` & `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/.idea/features_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/feature_extractors/.idea/workspace.xml` & `Simba-UW-tf-dev-1.62.8/simba/feature_extractors/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/requirements.txt` & `Simba-UW-tf-dev-1.62.8/simba/requirements.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/mixins/.DS_Store` & `Simba-UW-tf-dev-1.62.8/simba/mixins/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/mixins/pop_up_mixin.py` & `Simba-UW-tf-dev-1.62.8/simba/mixins/pop_up_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/mixins/config_reader.py` & `Simba-UW-tf-dev-1.62.8/simba/mixins/config_reader.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,19 @@
 import shutil
 import logging
 from configparser import ConfigParser
 import os, glob
 import pandas as pd
 import itertools
 import cv2
-from typing import List, Optional, Tuple, Union, Dict
+from typing import List, Optional, Tuple, Union, Dict, Any
+try:
+    from typing import Literal
+except:
+    from typing_extensions import Literal
 
 
 from simba.utils.enums import (Paths,
                                ConfigKey,
                                Dtypes,
                                Defaults,
                                Keys)
@@ -26,15 +30,16 @@
                                 NotDirectoryError,
                                 InvalidInputError,
                                 DuplicationError,
                                 ParametersFileError)
 from simba.utils.warnings import (NoFileFoundWarning,
                                   BodypartColumnNotFoundWarning,
                                   InvalidValueWarning,
-                                  NoDataFoundWarning)
+                                  NoDataFoundWarning,
+                                  DataHeaderWarning)
 from simba.utils.read_write import (read_project_path_and_file_type,
                                     get_fn_ext,
                                     read_config_file,
                                     find_core_cnt,
                                     get_all_clf_names,
                                     read_df,
                                     write_df)
@@ -166,106 +171,80 @@
             entry_name = 'target_name_{}'.format(str(i + 1))
             model_names.append(self.read_config_entry(self.config, ConfigKey.SML_SETTINGS.value, entry_name, data_type=Dtypes.STR.value))
         return model_names
 
     def insert_column_headers_for_outlier_correction(self,
                                                      data_df: pd.DataFrame,
                                                      new_headers: List[str],
-                                                     filepath: str):
+                                                     filepath: str) -> pd.DataFrame:
         """
         Helper to insert new column headers onto a dataframe.
 
-        Parameters
-        ----------
-        data_df:  pd.DataFrame
-            Dataframe where headers to to-bo replaced.
-        new_headers: list
-            Names of new headers.
-        filepath: str
-            Path to where ``data_df`` is stored on disk
+        :param pd.DataFrame data_df:  Dataframe where headers to to-bo replaced.
+        :param List[str] new_headers:  Names of new headers.
+        :param str filepath:  Path to where ``data_df`` is stored on disk
+        :returns pd.DataFrame: Dataframe with new headers
+        :raises DataHeaderWarning: If new headers are fewer/more than columns in dataframe
 
-        Returns
-        -------
-        data_df: pd.DataFrame
-            Dataframe with new headers
+        :example:
+        >>> df = pd.DataFrame(data=[[1, 2, 3], [1, 2, 3]], columns=['Feature_1', 'Feature_2', 'Feature_3'])
+        >>> ConfigReader.insert_column_headers_for_outlier_correction(data_df=df, new_headers=['Feature_4', 'Feature_5', 'Feature_6'], filepath='test/my_test_file.csv')
         """
 
         if len(new_headers) != len(data_df.columns):
             difference = int(len(data_df.columns) - len(new_headers))
             bp_missing = int(abs(difference) / 3)
             if difference < 0:
-                print(
-                    'SIMBA ERROR: SimBA expects {} columns of data inside the files within project_folder/csv/input_csv directory. However, '
-                    'within file {} file, SimBA found {} columns. Thus, there is {} missing data columns in the imported data, which may represent {} '
-                    'bodyparts if each body-part has an x, y and p value. Either revise the SimBA project pose-configuration with {} less body-part, or '
-                    'include {} more body-part in the imported data'.format(str(len(new_headers)), filepath,
-                                                                            str(len(data_df.columns)),
-                                                                            str(abs(difference)),
-                                                                            str(int(bp_missing)), str(bp_missing),
-                                                                            str(bp_missing)))
+                raise DataHeaderWarning(msg=f'SIMBA ERROR: SimBA expects {len(new_headers)} columns of data inside the files within project_folder/csv/input_csv directory. However, within file {filepath} file, SimBA found {len(data_df.columns)} columns. Thus, there is {abs(difference)} missing data columns in the imported data, which may represent {int(bp_missing)} bodyparts if each body-part has an x, y and p value. Either revise the SimBA project pose-configuration with {bp_missing} less body-part, or include {bp_missing} more body-part in the imported data')
             else:
-                print(
-                    'SIMBA ERROR: SimBA expects {} columns of data inside the files within project_folder/csv/input_csv directory. However, '
-                    'within file {} file, SimBA found {} columns. Thus, there is {} more data columns in the imported data than anticipated, which may represent {} '
-                    'bodyparts if each body-part has an x, y and p value. Either revise the SimBA project pose-configuration with {} more body-part, or '
-                    'include {} less body-part in the imported data'.format(str(len(new_headers)), filepath,
-                                                                            str(len(data_df.columns)),
-                                                                            str(abs(difference)),
-                                                                            str(int(bp_missing)), str(bp_missing),
-                                                                            str(bp_missing)))
-            raise ValueError()
+                raise DataHeaderWarning(msg=f'SIMBA ERROR: SimBA expects {len(new_headers)} columns of data inside the files within project_folder/csv/input_csv directory. However, within file {filepath} file, SimBA found {len(data_df.columns)} columns. Thus, there is {abs(difference)} more data columns in the imported data than anticipated, which may represent {int(bp_missing)} bodyparts if each body-part has an x, y and p value. Either revise the SimBA project pose-configuration with {bp_missing} more body-part, or include {bp_missing} less body-part in the imported data')
         else:
             data_df.columns = new_headers
             return data_df
 
     def get_number_of_header_columns_in_df(self,
                                            df: pd.DataFrame) -> int:
 
         """
-        Helper to find the number of non-numerical rows at the top of a dataframe.
+        Helper to find the count of non-numerical rows at the top of a dataframe.
 
-        Parameters
-        ----------
-        data_df:  pd.DataFrame
+        :param pd.DataFrame data_df: Dataframe to find the count non-numerical header rows in.
+        :returns int
+        :raises DataHeaderError: All rows are non-numerical.
 
-        Returns
-        -------
-        int
+        :example:
+        >>> ConfigReader.get_number_of_header_columns_in_df(df=pd.DataFrame(data=[[1, 2, 3], [1, 2, 3]]))
+        >>> 0
+        >>> ConfigReader.get_number_of_header_columns_in_df(df=pd.DataFrame(data=[['Head_1', 'Body_2', 'Tail_3'], ['Some_nonsense', 'A_mistake', 'Maybe_multi_headers?'], [11, 99, 109], [122, 43, 2091]]))
+        >>> 2
         """
 
         for i in range(len(df)):
             try:
-                temp = df.iloc[i:].apply(pd.to_numeric).reset_index(drop=True)
+                _ = df.iloc[i:].apply(pd.to_numeric).reset_index(drop=True)
                 return i
             except ValueError:
                 pass
         raise DataHeaderError(msg='Could find the count of header columns in dataframe')
 
 
     def find_video_of_file(self,
-                           video_dir: str,
-                           filename: str) -> str:
+                           video_dir: Union[str, os.PathLike],
+                           filename: str) -> Union[str, os.PathLike]:
         """
-        Helper to find the video file that represents a data file.
-
-        Parameters
-        ----------
-        video_dir: str
-            Directory holding putative video file
-        filename: str
-            Data file name, e.g., ``Video_1``.
-
-        Returns
-        -------
-        str
+        Helper to find the video file representing a known data file basename.
 
-        Raises
-        -------
-        NoFileFoundWarning: No video file is found.
+        :param Union[str, os.PathLike] video_dir: Directory holding putative video file.
+        :param str filename: Data file name, e.g., ``Video_1``.
+        :return Union[str, os.PathLike]: Path to video file.
 
+        :example:
+        >>> config_reader = ConfigReader(config_path='My_SimBA_Config')
+        >>> config_reader.find_video_of_file(video_dir=config_reader.video_dir, filename='Video1')
+        >>> '/project_folder/videos/Video1.mp4'
         """
         try:
             all_files_in_video_folder = [f for f in next(os.walk(video_dir))[2] if not f[0] == '.']
         except StopIteration:
             raise NoFilesFoundError(msg=f'No files found in the {video_dir} directory')
         all_files_in_video_folder = [os.path.join(video_dir, x) for x in all_files_in_video_folder]
         return_path = None
@@ -277,25 +256,20 @@
         if return_path is None:
             NoFileFoundWarning(f'SimBA could not find a video file representing {filename} in the project video directory')
         return return_path
 
     def add_missing_ROI_cols(self,
                              shape_df: pd.DataFrame) -> pd.DataFrame:
         """
-        Helper to add missing ROI definitions in ROI info dataframes created by the first version of the SimBA ROI
-        user-interface but analyzed using newer versions of SimBA.
+        Helper to add missing ROI definitions (``Color BGR``, ``Thickness``, ``Color name``) in ROI info
+        dataframes created by the first version of the SimBA ROI user-interface but analyzed using newer versions of SimBA.
 
-        Parameters
-        ----------
-        shape_df: pd.DataFrame
-            Dataframe holding ROI definitions.
 
-        Returns
-        -------
-        pd.DataFrame
+        :param pd.DataFrame shape_df: Dataframe holding ROI definitions.
+        :return pd.DataFrame with ``Color BGR``, ``Thickness``, ``Color name`` fields
         """
 
         if not 'Color BGR' in shape_df.columns:
             shape_df['Color BGR'] = [(255, 255, 255)] * len(shape_df)
         if not 'Thickness' in shape_df.columns:
             shape_df['Thickness'] = [5] * len(shape_df)
         if not 'Color name' in shape_df.columns:
@@ -308,15 +282,26 @@
         """Helper to remove a directory"""
         shutil.rmtree(folder_dir, ignore_errors=True)
 
     def find_animal_name_from_body_part_name(self,
                                              bp_name: str,
                                              bp_dict: dict) -> str:
 
-        """Given body-part name and animal body-part dict, return animal name"""
+        """
+        Given body-part name and animal body-part dict, returns the animal name
+
+        :param str bp_name: Name of the body-part. E.g., ``Ear_1``.
+        :param dict bp_dict: Nested dict holding animal names as keys and body-part names as and coordinates as values. Created by :meth:`simba.mixins.config_reader.ConfigReader.create_body_part_dictionary`
+        :returns str
+
+        :example:
+        >>> config_reader = ConfigReader(config_path='tests/data/test_projects/two_c57/project_folder/project_config.ini')
+        >>> ConfigReader.find_animal_name_from_body_part_name(bp_name='Ear_1', bp_dict=config_reader.animal_bp_dict)
+        >>> 'simon'
+        """
 
         for animal_name, animal_bps in bp_dict.items():
             if bp_name in [x[:-2] for x in animal_bps['X_bps']]:
                 return animal_name
 
     def create_logger(self,
                       path: str) -> None:
@@ -335,34 +320,26 @@
                                     y_cols: List[str],
                                     p_cols: Optional[List[str]] = None,
                                     colors: Optional[List[List[Tuple[int, int, int]]]] = None) -> Dict[str, Union[List[str], List[Tuple]]]:
         """
         Helper to create dict of dict lookup of body-parts where the keys are animal names, and
         values are the body-part names.
 
-        Parameters
-        ----------
-        multi_animal_status: bool
-            If True, it is a multi-animal SimBA project
-        multi_animal_id_lst: list
-            Animal names. Eg., ['Animal_1, 'Animals_2']
-        animal_cnt: int
-            Number of animals in the SimBA project.
-        x_cols: list
-            column names for body-part coordinates on x-axis
-        y_cols: list
-             column names for body-part coordinates on y-axis
-        p_cols: list
-            Column names for body-part pose-estimation probability values
-        colors: list or None
-            bgr colors
+        :param bool multi_animal_status: If True, it is a multi-animal SimBA project.
+        :param List[str] multi_animal_id_lst: Animal names. Eg., ['Simon, 'JJ']. Note: If a single animal project, this will be overridden and set to `Animal_1`.
+        :param int animal_cnt: Number of animals in the SimBA project.
+        :param List[str] x_cols: column names for body-part coordinates on x-axis. Returned by  :meth:`simba.mixins.config_reader.ConfigReader.get_body_part_names`
+        :param List[str] y_cols: column names for body-part coordinates on y-axis. Returned by  :meth:`simba.mixins.config_reader.ConfigReader.get_body_part_names`
+        :param List[str] p_cols: column names for body-part pose-estimation probability values. Returned by  :meth:`simba.mixins.config_reader.ConfigReader.get_body_part_names`
+        :param Optional[List[List[Tuple[int, int, int]]]] colors: Optional bgr colors to associate with the body-parts. Returned by :meth:`simba.utils.data.create_color_palettes`.
+        :returns dict
 
-        Returns
-        -------
-        dict
+        :example:
+        >>> ConfigReader.create_body_part_dictionary(multi_animal_status=True, animal_id_lst=['simon',])
+        >>> {'simon': {'X_bps': ['Nose_1_x', 'Ear_left_1_x', 'Ear_right_1_x', 'Center_1_x', 'Lat_left_1_x', 'Lat_right_1_x', 'Tail_base_1_x', 'Tail_end_1_x'], 'Y_bps': ['Nose_1_y', 'Ear_left_1_y', 'Ear_right_1_y', 'Center_1_y', 'Lat_left_1_y', 'Lat_right_1_y', 'Tail_base_1_y', 'Tail_end_1_y'], 'colors': [[255.0, 0.0, 255.0], [223.125, 31.875, 255.0], [191.25, 63.75, 255.0], [159.375, 95.625, 255.0], [127.5, 127.5, 255.0], [95.625, 159.375, 255.0], [63.75, 191.25, 255.0], [31.875, 223.125, 255.0], [0.0, 255.0, 255.0]], 'P_bps': ['Nose_1_p', 'Ear_left_1_p', 'Ear_right_1_p', 'Center_1_p', 'Lat_left_1_p', 'Lat_right_1_p', 'Tail_base_1_p', 'Tail_end_1_p']}, 'jj': {'X_bps': ['Nose_2_x', 'Ear_left_2_x', 'Ear_right_2_x', 'Center_2_x', 'Lat_left_2_x', 'Lat_right_2_x', 'Tail_base_2_x', 'Tail_end_2_x'], 'Y_bps': ['Nose_2_y', 'Ear_left_2_y', 'Ear_right_2_y', 'Center_2_y', 'Lat_left_2_y', 'Lat_right_2_y', 'Tail_base_2_y', 'Tail_end_2_y'], 'colors': [[102.0, 127.5, 0.0], [102.0, 143.4375, 31.875], [102.0, 159.375, 63.75], [102.0, 175.3125, 95.625], [102.0, 191.25, 127.5], [102.0, 207.1875, 159.375], [102.0, 223.125, 191.25], [102.0, 239.0625, 223.125], [102.0, 255.0, 255.0]], 'P_bps': ['Nose_2_p', 'Ear_left_2_p', 'Ear_right_2_p', 'Center_2_p', 'Lat_left_2_p', 'Lat_right_2_p', 'Tail_base_2_p', 'Tail_end_2_p']}}
         """
 
         animal_bp_dict = {}
         if multi_animal_status:
             for animal in range(animal_cnt):
                 animal_bp_dict[animal_id_lst[animal]] = {}
                 animal_bp_dict[animal_id_lst[animal]]['X_bps'] = [i for i in x_cols if animal_id_lst[animal] in i]
@@ -404,58 +381,83 @@
                     animal_bp_dict['Animal_1']['P_bps'] = [i for i in p_cols]
 
         return animal_bp_dict
 
     def get_body_part_names(self):
         """
         Helper to extract pose-estimation data field names (x, y, p)
+
+        :example:
+        >>> config_reader = ConfigReader(config_path='test/project_config.csv')
+        >>> config_reader.get_body_part_names()
         """
         self.x_cols, self.y_cols, self.p_cols = [], [], []
         for bp in self.body_parts_lst:
             self.x_cols.append(f'{bp}_x'); self.y_cols.append(f'{bp}_y'); self.p_cols.append(f'{bp}_p')
 
     def drop_bp_cords(self,
                       df: pd.DataFrame) -> pd.DataFrame:
 
         """
-        Helper to remove pose-estimation data from dataframe.
+        Helper to remove pose-estimation fields from dataframe.
 
-        Parameters
-        ----------
-        df: pd.DataFrame
-            pandas dataframe containing pose-estimation data
+        :param pd.DataFrame df: pandas dataframe containing pose-estimation fields (body-part x, y, p fields)
+        :return pd.DataFrame: ``df`` without pose-estimation fields
 
+        :example:
+        >>> config_reader = ConfigReader(config_path='test/project_folder/project_config.csv')
+        >>> df = read_df(config_reader.machine_results_paths[0], file_type='csv')
+        >>> df = config_reader.drop_bp_cords(df=df)
         """
-
-
         missing_body_part_fields = list(set(self.bp_col_names) - set(list(df.columns)))
         if len(missing_body_part_fields) > 0:
             BodypartColumnNotFoundWarning(msg=f'SimBA could not drop body-part coordinates, some body-part names are missing in dataframe. SimBA expected the following body-parts, that could not be found inside the file: {missing_body_part_fields}')
         else:
             return df.drop(self.bp_col_names, axis=1)
 
 
     def get_bp_headers(self) -> None:
         """
         Helper to create ordered list of all column header fields for SimBA project dataframes.
+
+        >>> config_reader = ConfigReader(config_path='test/project_folder/project_config.csv')
+        >>> config_reader.get_bp_headers()
         """
         self.bp_headers = []
         for bp in self.body_parts_lst:
             c1, c2, c3 = (f'{bp}_x', f'{bp}_y', f'{bp}_p')
             self.bp_headers.extend((c1, c2, c3))
 
     def read_config_entry(self,
                           config: ConfigParser,
                           section: str,
                           option: str,
-                          data_type: str,
-                          default_value = None,
-                          options = None) -> Union[str, int, float]:
+                          data_type: Literal['str', 'int', 'float', 'folder_path'],
+                          default_value: Optional[Any] = None,
+                          options: Optional[List[Any]] = None) -> Union[str, int, float]:
+
+        """
+        Helper to read entry from a configparser.ConfigParser object
+
+        :param ConfigParser config: Parsed SimBA project config
+        :param str section: Project config section name
+        :param str option: Project config option name
+        :param str data_type: Type of data. E.g., ``str``, ``int``, ``float``, ``folder_path``.
+        :param Optional[Any] default_value: If entry cannot be found, then default to this value.
+        :param Optional[List[Any]] options: If not ``None``, then list of viable entries.
+        :raise InvalidInputError: If returned value is not in ``options``.
+        :raise MissingProjectConfigEntryError: If no entry is found and no ``default_value`` is provided.
+
+        :return Union[str, float, int, os.Pathlike]
 
-        """ Helper to read entry in a configparser.ConfigParser object"""
+        :example:
+        >>> config = ConfigReader(config_path='tests/data/test_projects/two_c57/project_folder/project_config.ini')
+        >>> config.read_config_entry(config=self.config, section='Multi animal IDs', option='id_list', data_type='str')
+        >>> 'simon,jj'
+        """
         try:
             if config.has_option(section, option):
                 if data_type == Dtypes.FLOAT.value:
                     value = config.getfloat(section, option)
                 elif data_type == Dtypes.INT.value:
                     value = config.getint(section, option)
                 elif data_type == Dtypes.STR.value:
@@ -514,17 +516,19 @@
 
     def read_video_info(self,
                         video_name: str,
                         raise_error: Optional[bool] = True) -> (pd.DataFrame, float, float):
         """
         Helper to read the meta-data (pixels per mm, resolution, fps) from the video_info.csv for a single input file.
 
-        :param str video_name: The name of the video without extension to get the meta data for
+        :param str video_name: The name of the video without extension to get the metadata for
         :param Optional[bool] raise_error: If True, raise error if video info for the video name cannot be found. Default: True.
-        :return (pd.DataFrame, float, float)
+        :raise ParametersFileError: If ``raise_error`` and video metadata info is not found
+        :raise DuplicationError: If file contains multiple entries for the same video.
+        :return (pd.DataFrame, float, float) representing all video info, pixels per mm, and fps
         """
 
         video_settings = self.video_info_df.loc[self.video_info_df['Video'] == video_name]
         if len(video_settings) > 1:
             raise DuplicationError(msg=f'SimBA found multiple rows in the project_folder/logs/video_info.csv named {str(video_name)}. Please make sure that each video name is represented ONCE in the video_info.csv')
         elif len(video_settings) < 1:
             if raise_error:
@@ -612,14 +616,18 @@
 
 
             #x = [x for x in self.shape_names if any(x in y or y in x for y in df.colum)]
 
 
 
 
+# config = ConfigReader(config_path='/Users/simon/Desktop/envs/simba_dev/tests/data/test_projects/two_c57/project_folder/project_config.ini', read_video_info=False)
+# config.read_roi_data()
+
+
 # config = ConfigReader(config_path='/Users/simon/Desktop/envs/troubleshooting/Nastacia_unsupervised/project_folder/project_config.ini', read_video_info=False)
 # config.read_roi_data()
 # config.remove_roi_features('/Users/simon/Desktop/envs/troubleshooting/Nastacia_unsupervised/project_folder/csv/features_extracted')
 
         # remove_roi_features(
         #     config_path='/Users/simon/Desktop/envs/troubleshooting/Nastacia_unsupervised/project_folder/project_config.ini',
         #     data_dir='/Users/simon/Desktop/envs/troubleshooting/Nastacia_unsupervised/project_folder/csv/features_extracted')
```

### Comparing `Simba-UW-tf-dev-1.62.7/simba/mixins/pose_importer_mixin.py` & `Simba-UW-tf-dev-1.62.8/simba/mixins/pose_importer_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.nbi` & `Simba-UW-tf-dev-1.62.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi` & `Simba-UW-tf-dev-1.62.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi` & `Simba-UW-tf-dev-1.62.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.nbi`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.1.nbc` & `Simba-UW-tf-dev-1.62.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-334.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc` & `Simba-UW-tf-dev-1.62.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.cdist-333.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc` & `Simba-UW-tf-dev-1.62.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.2.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc` & `Simba-UW-tf-dev-1.62.8/simba/mixins/__pycache__/feature_extraction_mixin.FeatureExtractionMixin.angle3pt-84.py36m.1.nbc`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/mixins/feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.62.8/simba/mixins/feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/mixins/plotting_mixin.py` & `Simba-UW-tf-dev-1.62.8/simba/mixins/plotting_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/mixins/unsupervised_mixin.py` & `Simba-UW-tf-dev-1.62.8/simba/mixins/unsupervised_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/mixins/train_model_mixin.py` & `Simba-UW-tf-dev-1.62.8/simba/mixins/train_model_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,16 @@
                                 FaultyTrainingSetError,
                                 MissingColumnsError,
                                 NoDataError,
                                 SamplingError,
                                 CorruptedFileError,
                                 FeatureNumberMismatchError,
                                 ClassifierInferenceError,
-                                InvalidInputError)
+                                InvalidInputError,
+                                DataHeaderError)
 from simba.utils.warnings import (NotEnoughDataWarning,
                                   NoModuleWarning,
                                   MissingUserInputWarning,
                                   MultiProcessingFailedWarning,
                                   ShapWarning)
 from simba.utils.printing import stdout_success, SimbaTimer
 from simba.utils.lookups import get_meta_data_file_headers
@@ -332,18 +333,18 @@
         results_df = pd.DataFrame()
         results_df['FRACTION TRAIN SIZE'] = np.linspace(0.01, 1.0, dataset_splits)
         results_df['TRAIN_MEAN_F1'] = np.mean(train_scores, axis=1)
         results_df['TEST_MEAN_F1'] = np.mean(test_scores, axis=1)
         results_df['TRAIN_STDEV_F1'] = np.std(train_scores, axis=1)
         results_df['TEST_STDEV_F1'] = np.std(test_scores, axis=1)
         if save_file_no != None:
-            save_file_path = os.path.join(save_dir, clf_name + '_' + str(save_file_no + 1) + '_learning_curve.csv')
+            self.learning_curve_save_path = os.path.join(save_dir, clf_name + '_' + str(save_file_no + 1) + '_learning_curve.csv')
         else:
-            save_file_path = os.path.join(save_dir, clf_name + '_learning_curve.csv')
-        results_df.to_csv(save_file_path, index=False)
+            self.learning_curve_save_path = os.path.join(save_dir, clf_name + '_learning_curve.csv')
+        results_df.to_csv(self.learning_curve_save_path, index=False)
         timer.stop_timer()
         print('Learning curve calculation complete (elapsed time: {}s) ...'.format(timer.elapsed_time_str))
 
     def calc_pr_curve(self,
                       rf_clf: RandomForestClassifier,
                       x_df: pd.DataFrame,
                       y_df: pd.DataFrame,
@@ -370,18 +371,18 @@
         pr_df['PRECISION'] = precision
         pr_df['RECALL'] = recall
         pr_df['F1'] = 2 * pr_df['RECALL'] * pr_df['PRECISION'] / (pr_df['RECALL'] + pr_df['PRECISION'])
         thresholds = list(thresholds)
         thresholds.insert(0, 0.00)
         pr_df['DISCRIMINATION THRESHOLDS'] = thresholds
         if save_file_no != None:
-            save_file_path = os.path.join(save_dir, clf_name + '_' + str(save_file_no + 1) + '_pr_curve.csv')
+            self.pr_save_path = os.path.join(save_dir, clf_name + '_' + str(save_file_no + 1) + '_pr_curve.csv')
         else:
-            save_file_path = os.path.join(save_dir, clf_name + '_pr_curve.csv')
-        pr_df.to_csv(save_file_path, index=False)
+            self.pr_save_path = os.path.join(save_dir, clf_name + '_pr_curve.csv')
+        pr_df.to_csv(self.pr_save_path, index=False)
         timer.stop_timer()
         print('Precision-recall curve calculation complete (elapsed time: {}s) ...'.format(timer.elapsed_time_str))
 
     def create_example_dt(self,
                           rf_clf: RandomForestClassifier,
                           clf_name: str,
                           feature_names: List[str],
@@ -470,18 +471,18 @@
 
         print('Creating feature importance log...')
         importances = list(rf_clf.feature_importances_)
         feature_importances = [(feature, round(importance, 2)) for feature, importance in zip(x_names, importances)]
         df = pd.DataFrame(feature_importances, columns=['FEATURE', 'FEATURE_IMPORTANCE']).sort_values(
             by=['FEATURE_IMPORTANCE'], ascending=False)
         if save_file_no != None:
-            save_file_path = os.path.join(save_dir, clf_name + '_' + str(save_file_no) + '_feature_importance_log.csv')
+            self.f_importance_save_path = os.path.join(save_dir, clf_name + '_' + str(save_file_no) + '_feature_importance_log.csv')
         else:
-            save_file_path = os.path.join(save_dir, clf_name + '_feature_importance_log.csv')
-        df.to_csv(save_file_path, index=False)
+            self.f_importance_save_path = os.path.join(save_dir, clf_name + '_feature_importance_log.csv')
+        df.to_csv(self.f_importance_save_path, index=False)
 
     def create_x_importance_bar_chart(self,
                                       rf_clf: RandomForestClassifier,
                                       x_names: list,
                                       clf_name: str,
                                       save_dir: str,
                                       n_bars: int,
@@ -567,15 +568,15 @@
         return data_arr, obs_per_split
 
 
     def create_shap_log(self,
                         ini_file_path: str,
                         rf_clf: RandomForestClassifier,
                         x_df: pd.DataFrame,
-                        y_df: pd.DataFrame,
+                        y_df: pd.Series,
                         x_names: List[str],
                         clf_name: str,
                         cnt_present: int,
                         cnt_absent: int,
                         save_path: str,
                         save_it: int = 100,
                         save_file_no: Optional[int] = None) -> None:
@@ -607,19 +608,19 @@
 
         """
 
         print('Calculating SHAP values (SINGLE CORE)...')
         shap_timer = SimbaTimer(start=True)
         data_df = pd.concat([x_df, y_df], axis=1)
         if save_file_no == None:
-            out_df_shap_path = os.path.join(save_path, f'SHAP_values_{clf_name}.csv')
-            out_df_raw_path = os.path.join(save_path, f'RAW_SHAP_feature_values_{clf_name}.csv')
+            self.out_df_shap_path = os.path.join(save_path, f'SHAP_values_{clf_name}.csv')
+            self.out_df_raw_path = os.path.join(save_path, f'RAW_SHAP_feature_values_{clf_name}.csv')
         else:
-            out_df_shap_path = os.path.join(save_path, f'SHAP_values_{str(save_file_no)}_{clf_name}.csv')
-            out_df_raw_path = os.path.join(save_path, f'RAW_SHAP_feature_values_{str(save_file_no)}_{clf_name}.csv')
+            self.out_df_shap_path = os.path.join(save_path, f'SHAP_values_{str(save_file_no)}_{clf_name}.csv')
+            self.out_df_raw_path = os.path.join(save_path, f'RAW_SHAP_feature_values_{str(save_file_no)}_{clf_name}.csv')
 
         target_df, nontarget_df = data_df[data_df[y_df.name] == 1], data_df[data_df[y_df.name] == 0]
         if len(target_df) < cnt_present:
             NotEnoughDataWarning(msg=f'Train data contains {str(len(target_df))} behavior-present annotations. This is less the number of frames you specified to calculate shap values for {str(cnt_present)}. SimBA will calculate shap scores for the {str(len(target_df))} behavior-present frames available')
             cnt_present = len(target_df)
         if len(nontarget_df) < cnt_absent:
             NotEnoughDataWarning(msg=f'Train data contains {str(len(nontarget_df))} behavior-absent annotations. This is less the number of frames you specified to calculate shap values for {str(cnt_absent)}. SimBA will calculate shap scores for the {str(len(target_df))} behavior-absent frames available')
@@ -639,16 +640,16 @@
             frame_data = shap_df.iloc[[frame]]
             frame_shap = explainer.shap_values(frame_data, check_additivity=False)[1][0].tolist()
             frame_shap.extend((expected_value, sum(frame_shap), rf_clf.predict_proba(frame_data)[0][1], y_df[cnt]))
             out_df_raw.loc[len(out_df_raw)] = list(shap_df.iloc[frame])
             out_df_shap.loc[len(out_df_shap)] = frame_shap
             if (cnt % save_it == 0) or (cnt == len(shap_df) - 1) and (cnt != 0):
                 print(f'Saving SHAP data after {cnt} iterations...')
-                out_df_shap.to_csv(out_df_shap_path)
-                out_df_raw.to_csv(out_df_raw_path)
+                out_df_shap.to_csv(self.out_df_shap_path)
+                out_df_raw.to_csv(self.out_df_raw_path)
             shap_frm_timer.stop_timer()
             print(f'SHAP frame: {cnt + 1} / {len(shap_df)}, elapsed time: {shap_frm_timer.elapsed_time_str}...')
 
         shap_timer.stop_timer()
         stdout_success(msg='SHAP calculations complete', elapsed_time=shap_timer.elapsed_time_str)
         _ = ShapAggregateStatisticsVisualizer(config_path=ini_file_path,
                                               classifier_name=clf_name,
@@ -761,15 +762,15 @@
                 check_int('minimum_bout_length', model_dict[n]['minimum_bout_length'])
             except ValueError:
                 MissingUserInputWarning(
                     msg=f'Skipping {str(config.get("SML settings", "target_name_" + str(n + 1)))} classifier analysis: missing information (e.g., no discrimination threshold and/or minimum bout set in the project_config.ini')
 
         if len(model_dict.keys()) == 0:
             raise NoDataError(
-                msg=f'There are no models with accurate data specified in the RUN MODELS menu. Speficy the model information to SimBA RUN MODELS menu to use them to analyze videos')
+                msg=f'There are no models with accurate data specified in the RUN MODELS menu. Specify the model information to SimBA RUN MODELS menu to use them to analyze videos')
         else:
             return model_dict
 
     def get_all_clf_names(self,
                           config: configparser.ConfigParser,
                           target_cnt: int) -> List[str]:
         """
@@ -790,48 +791,32 @@
             model_names.append(
                 read_config_entry(config, ConfigKey.SML_SETTINGS.value, entry_name, data_type=Dtypes.STR.value))
         return model_names
 
     def insert_column_headers_for_outlier_correction(self,
                                                      data_df: pd.DataFrame,
                                                      new_headers: List[str],
-                                                     filepath: str) -> pd.DataFrame:
+                                                     filepath: Union[str, os.PathLike]) -> pd.DataFrame:
         """
         Helper to insert new column headers onto a dataframe following outlier correction.
 
         :parameter pd.DataFrame data_df: Dataframe with headers to-be replaced.
         :parameter str filepath: Path to where ``data_df`` is stored on disk.
         :parameter List[str] new_headers: New headers.
         """
 
         if len(new_headers) != len(data_df.columns):
             difference = int(len(data_df.columns) - len(new_headers))
             bp_missing = int(abs(difference) / 3)
             if difference < 0:
-
-                print(
-                    'SIMBA ERROR: SimBA expects {} columns of data inside the files within project_folder/csv/input_csv directory. However, '
-                    'within file {} file, SimBA found {} columns. Thus, there is {} missing data columns in the imported data, which may represent {} '
-                    'bodyparts if each body-part has an x, y and p value. Either revise the SimBA project pose-configuration with {} less body-part, or '
-                    'include {} more body-part in the imported data'.format(str(len(new_headers)), filepath,
-                                                                            str(len(data_df.columns)),
-                                                                            str(abs(difference)),
-                                                                            str(int(bp_missing)), str(bp_missing),
-                                                                            str(bp_missing)))
+                raise DataHeaderError(msg=
+                    f'SimBA expects {len(new_headers)} columns of data inside the files within project_folder/csv/input_csv directory. However, within file {filepath} file, SimBA found {len(data_df.columns)} columns. Thus, there is {abs(difference)} missing data columns in the imported data, which may represent {int(bp_missing)} bodyparts if each body-part has an x, y and p value. Either revise the SimBA project pose-configuration with {str(bp_missing)} less body-part, or include {bp_missing} more body-part in the imported data')
             else:
-                print(
-                    'SIMBA ERROR: SimBA expects {} columns of data inside the files within project_folder/csv/input_csv directory. However, '
-                    'within file {} file, SimBA found {} columns. Thus, there is {} more data columns in the imported data than anticipated, which may represent {} '
-                    'bodyparts if each body-part has an x, y and p value. Either revise the SimBA project pose-configuration with {} more body-part, or '
-                    'include {} less body-part in the imported data'.format(str(len(new_headers)), filepath,
-                                                                            str(len(data_df.columns)),
-                                                                            str(abs(difference)),
-                                                                            str(int(bp_missing)), str(bp_missing),
-                                                                            str(bp_missing)))
-            raise ValueError()
+                raise DataHeaderError(msg=
+                    f'SimBA expects {len(new_headers)} columns of data inside the files within project_folder/csv/input_csv directory. However, within file {filepath} file, SimBA found {len(data_df.columns)} columns. Thus, there is {abs(difference)} more data columns in the imported data than anticipated, which may represent {int(bp_missing)} bodyparts if each body-part has an x, y and p value. Either revise the SimBA project pose-configuration with {str(bp_missing)} more body-part, or include {bp_missing} less body-part in the imported data')
         else:
             data_df.columns = new_headers
             return data_df
 
     def read_pickle(self,
                     file_path: Union[str, os.PathLike]) -> object:
         """
@@ -847,27 +832,32 @@
         except pickle.UnpicklingError:
             raise CorruptedFileError(msg=f'Can not read {file_path} as a classifier file (pickle).')
         return clf
 
     def bout_train_test_splitter(self,
                                  x_df: pd.DataFrame,
                                  y_df: pd.Series,
-                                 test_size: float) -> (np.ndarray, np.ndarray, np.ndarray, np.ndarray):
+                                 test_size: float) -> (pd.DataFrame, pd.DataFrame, pd.Series, pd.Series):
         """
         Helper to split train and test based on annotated `bouts`.
 
 
         :parameter pd.DataFrame x_df: Features
         :parameter pd.Series y_df: Target
         :parameter float test_size: Size of test as ratio of all annotated bouts (e.g., ``0.2``).
 
         :return np.ndarray x_train: Features for training
         :return np.ndarray x_test: Features for testing
         :return np.ndarray y_train: Target for training
         :return np.ndarray y_test: Target for testing
+
+        :examples:
+        >>> x = pd.DataFrame(data=[[11, 23, 12], [87, 65, 76], [23, 73, 27], [10, 29, 2], [12, 32, 42], [32, 73, 2], [21, 83, 98], [98, 1, 1]])
+        >>> y =  pd.Series([0, 0, 1, 1, 0, 0, 1, 1, 0, 0, 1, 1])
+        >>> x_train, x_test, y_train, y_test = TrainModelMixin().bout_train_test_splitter(x_df=x, y_df=y, test_size=0.5)
         """
         print('Using bout sampling...')
         def find_bouts(s: pd.Series, type: str):
             test_bouts_frames, train_bouts_frames = [], []
             bouts = detect_bouts(pd.DataFrame(s), target_lst=pd.DataFrame(s).columns, fps=-1)
             print(f'{str(len(bouts))} {type} bouts found...')
             bouts = list(bouts.apply(lambda x: list(range(int(x['Start_frame']), int(x['End_frame']) + 1)), 1).values)
@@ -877,16 +867,15 @@
                 if i in test_bouts_idx:
                     test_bouts_frames.append(bouts[i])
                 if i in train_bouts_idx:
                     train_bouts_frames.append(bouts[i])
             return [i for s in test_bouts_frames for i in s], [i for s in train_bouts_frames for i in s]
 
         test_bouts_frames, train_bouts_frames = find_bouts(s=y_df, type='behavior present')
-        test_nonbouts_frames, train_nonbouts_frames = find_bouts(s=np.logical_xor(y_df, 1).astype(int),
-                                                                 type='behavior absent')
+        test_nonbouts_frames, train_nonbouts_frames = find_bouts(s=np.logical_xor(y_df, 1).astype(int), type='behavior absent')
         x_train = x_df[x_df.index.isin(train_bouts_frames + train_nonbouts_frames)]
         x_test = x_df[x_df.index.isin(test_bouts_frames + test_nonbouts_frames)]
         y_train = y_df[y_df.index.isin(train_bouts_frames + train_nonbouts_frames)]
         y_test = y_df[y_df.index.isin(test_bouts_frames + test_nonbouts_frames)]
 
         return x_train, x_test, y_train, y_test
 
@@ -1252,25 +1241,27 @@
             cnt_absent = len(nontarget_df)
         non_target_for_shap = nontarget_df.sample(cnt_absent, replace=False)
         targets_for_shap = target_df.sample(cnt_present, replace=False)
         explainer = shap.TreeExplainer(rf_clf, data=None, model_output='raw', feature_perturbation='tree_path_dependent')
         expected_value = explainer.expected_value[1]
         cores, _ = find_core_cnt()
         shap_data_df = pd.concat([targets_for_shap, non_target_for_shap], axis=0)
-        print(f'Computing {len(shap_data_df)} SHAP values (MULTI-CORE, FOLLOW PROGRESS IN OS TERMINAL)...')
         if (len(shap_data_df) / batch_size) < 1:
             batch_size = 1
+        if len(shap_data_df) > 100:
+            batch_size = 100
+        print(f'Computing {len(shap_data_df)} SHAP values (MULTI-CORE BATCH SIZE: {batch_size}, FOLLOW PROGRESS IN OS TERMINAL)...')
         shap_data, _ = self.split_and_group_df(df=shap_data_df, splits=int(len(shap_data_df) / batch_size))
         shap_results, shap_raw = [], []
         try:
             with multiprocessing.Pool(cores, maxtasksperchild=10) as pool:
                 constants = functools.partial(self._create_shap_mp_helper,
                                               explainer=explainer,
                                               clf_name=clf_name)
-                for cnt, result in enumerate(pool.imap_unordered(constants, shap_data, chunksize=10)):
+                for cnt, result in enumerate(pool.imap_unordered(constants, shap_data, chunksize=1)):
                     print(f'Concatenating multi-processed SHAP data (batch {cnt+1}/{len(shap_data)})')
                     proba = rf_clf.predict_proba(result[1])[:, 1].reshape(-1, 1)
                     shap_sum = np.sum(result[0], axis=1).reshape(-1, 1)
                     shap_results.append(np.hstack((result[0], np.full((result[0].shape[0]), expected_value).reshape(-1, 1), shap_sum, proba, result[2])))
                     shap_raw.append(result[1])
             pool.terminate()
             pool.join()
```

### Comparing `Simba-UW-tf-dev-1.62.7/simba/third_party_label_appenders/deepethogram_importer.py` & `Simba-UW-tf-dev-1.62.8/simba/third_party_label_appenders/deepethogram_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/third_party_label_appenders/BORIS_appender.py` & `Simba-UW-tf-dev-1.62.8/simba/third_party_label_appenders/BORIS_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/third_party_label_appenders/observer_importer.py` & `Simba-UW-tf-dev-1.62.8/simba/third_party_label_appenders/observer_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/third_party_label_appenders/tools.py` & `Simba-UW-tf-dev-1.62.8/simba/third_party_label_appenders/tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/third_party_label_appenders/third_party_appender.py` & `Simba-UW-tf-dev-1.62.8/simba/third_party_label_appenders/third_party_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/third_party_label_appenders/ethovision_import.py` & `Simba-UW-tf-dev-1.62.8/simba/third_party_label_appenders/ethovision_import.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/third_party_label_appenders/BENTO_appender.py` & `Simba-UW-tf-dev-1.62.8/simba/third_party_label_appenders/BENTO_appender.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/third_party_label_appenders/solomon_importer.py` & `Simba-UW-tf-dev-1.62.8/simba/third_party_label_appenders/solomon_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/cue_light_tools/.DS_Store` & `Simba-UW-tf-dev-1.62.8/simba/cue_light_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/cue_light_tools/cue_light_clf_statistics.py` & `Simba-UW-tf-dev-1.62.8/simba/cue_light_tools/cue_light_clf_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/cue_light_tools/cue_light_analyzer.py` & `Simba-UW-tf-dev-1.62.8/simba/cue_light_tools/cue_light_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/cue_light_tools/cue_light_menues.py` & `Simba-UW-tf-dev-1.62.8/simba/cue_light_tools/cue_light_menues.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/cue_light_tools/cue_light_tools.py` & `Simba-UW-tf-dev-1.62.8/simba/cue_light_tools/cue_light_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/cue_light_tools/cue_light_visualizer.py` & `Simba-UW-tf-dev-1.62.8/simba/cue_light_tools/cue_light_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/cue_light_tools/cue_light_movement_statistics.py` & `Simba-UW-tf-dev-1.62.8/simba/cue_light_tools/cue_light_movement_statistics.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/utils/config_creator.py` & `Simba-UW-tf-dev-1.62.8/simba/utils/config_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/utils/enums.py` & `Simba-UW-tf-dev-1.62.8/simba/utils/enums.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/utils/.DS_Store` & `Simba-UW-tf-dev-1.62.8/simba/utils/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/utils/warnings.py` & `Simba-UW-tf-dev-1.62.8/simba/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/utils/checks.py` & `Simba-UW-tf-dev-1.62.8/simba/utils/checks.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/utils/read_write.py` & `Simba-UW-tf-dev-1.62.8/simba/utils/read_write.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/utils/lookups.py` & `Simba-UW-tf-dev-1.62.8/simba/utils/lookups.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/utils/cli/cli_tools.py` & `Simba-UW-tf-dev-1.62.8/simba/utils/cli/cli_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/utils/errors.py` & `Simba-UW-tf-dev-1.62.8/simba/utils/errors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/utils/data.py` & `Simba-UW-tf-dev-1.62.8/simba/utils/data.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/utils/printing.py` & `Simba-UW-tf-dev-1.62.8/simba/utils/printing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_processors/reorganize_keypoint.py` & `Simba-UW-tf-dev-1.62.8/simba/pose_processors/reorganize_keypoint.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_processors/remove_keypoints.py` & `Simba-UW-tf-dev-1.62.8/simba/pose_processors/remove_keypoints.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_processors/pose_reset.py` & `Simba-UW-tf-dev-1.62.8/simba/pose_processors/pose_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_processors/reverse_pose.py` & `Simba-UW-tf-dev-1.62.8/simba/pose_processors/reverse_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/plotting/gantt_creator.py` & `Simba-UW-tf-dev-1.62.8/simba/plotting/gantt_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/plotting/tools/tkinter_tools.py` & `Simba-UW-tf-dev-1.62.8/simba/plotting/tools/tkinter_tools.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/plotting/ROI_plotter_mp.py` & `Simba-UW-tf-dev-1.62.8/simba/plotting/ROI_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/plotting/.DS_Store` & `Simba-UW-tf-dev-1.62.8/simba/plotting/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/plotting/shap_agg_stats_visualizer.py` & `Simba-UW-tf-dev-1.62.8/simba/plotting/shap_agg_stats_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/plotting/gantt_creator_mp.py` & `Simba-UW-tf-dev-1.62.8/simba/plotting/gantt_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/plotting/heat_mapper_clf_mp.py` & `Simba-UW-tf-dev-1.62.8/simba/plotting/heat_mapper_clf_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/plotting/probability_plot_creator.py` & `Simba-UW-tf-dev-1.62.8/simba/plotting/probability_plot_creator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/plotting/plot_clf_results.py` & `Simba-UW-tf-dev-1.62.8/simba/plotting/plot_clf_results.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/plotting/plot_clf_results_mp.py` & `Simba-UW-tf-dev-1.62.8/simba/plotting/plot_clf_results_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/plotting/ROI_feature_visualizer.py` & `Simba-UW-tf-dev-1.62.8/simba/plotting/ROI_feature_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/plotting/heat_mapper_location.py` & `Simba-UW-tf-dev-1.62.8/simba/plotting/heat_mapper_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/plotting/probability_plot_creator_mp.py` & `Simba-UW-tf-dev-1.62.8/simba/plotting/probability_plot_creator_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/plotting/interactive_probability_grapher.py` & `Simba-UW-tf-dev-1.62.8/simba/plotting/interactive_probability_grapher.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/plotting/plot_pose_in_dir.py` & `Simba-UW-tf-dev-1.62.8/simba/plotting/plot_pose_in_dir.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/plotting/single_run_model_validation_video.py` & `Simba-UW-tf-dev-1.62.8/simba/plotting/single_run_model_validation_video.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/plotting/frame_mergerer_ffmpeg.py` & `Simba-UW-tf-dev-1.62.8/simba/plotting/frame_mergerer_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/plotting/Directing_animals_visualizer_mp.py` & `Simba-UW-tf-dev-1.62.8/simba/plotting/Directing_animals_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/plotting/clf_validator.py` & `Simba-UW-tf-dev-1.62.8/simba/plotting/clf_validator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/plotting/path_plotter_mp.py` & `Simba-UW-tf-dev-1.62.8/simba/plotting/path_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/plotting/ROI_feature_visualizer_mp.py` & `Simba-UW-tf-dev-1.62.8/simba/plotting/ROI_feature_visualizer_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/plotting/data_plotter.py` & `Simba-UW-tf-dev-1.62.8/simba/plotting/data_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/plotting/path_plotter.py` & `Simba-UW-tf-dev-1.62.8/simba/plotting/path_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/plotting/ez_lineplot.py` & `Simba-UW-tf-dev-1.62.8/simba/plotting/ez_lineplot.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/plotting/distance_plotter_mp.py` & `Simba-UW-tf-dev-1.62.8/simba/plotting/distance_plotter_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/plotting/ROI_plotter.py` & `Simba-UW-tf-dev-1.62.8/simba/plotting/ROI_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/plotting/heat_mapper_clf.py` & `Simba-UW-tf-dev-1.62.8/simba/plotting/heat_mapper_clf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/plotting/distance_plotter.py` & `Simba-UW-tf-dev-1.62.8/simba/plotting/distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/plotting/single_run_model_validation_video_mp.py` & `Simba-UW-tf-dev-1.62.8/simba/plotting/single_run_model_validation_video_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/plotting/Directing_animals_visualizer.py` & `Simba-UW-tf-dev-1.62.8/simba/plotting/Directing_animals_visualizer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/plotting/heat_mapper_location_mp.py` & `Simba-UW-tf-dev-1.62.8/simba/plotting/heat_mapper_location_mp.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/dash_app/SimBA_dash_app.py` & `Simba-UW-tf-dev-1.62.8/simba/dash_app/SimBA_dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/dash_app/run_dash_tkinter.py` & `Simba-UW-tf-dev-1.62.8/simba/dash_app/run_dash_tkinter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/dash_app/dash_app.py` & `Simba-UW-tf-dev-1.62.8/simba/dash_app/dash_app.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/data_processors/agg_clf_calculator.py` & `Simba-UW-tf-dev-1.62.8/simba/data_processors/agg_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/data_processors/severity_bout_based_calculator.py` & `Simba-UW-tf-dev-1.62.8/simba/data_processors/severity_bout_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/data_processors/interpolation_smoothing.py` & `Simba-UW-tf-dev-1.62.8/simba/data_processors/interpolation_smoothing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/data_processors/timebins_clf_calculator.py` & `Simba-UW-tf-dev-1.62.8/simba/data_processors/timebins_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/data_processors/fsttc_calculator.py` & `Simba-UW-tf-dev-1.62.8/simba/data_processors/fsttc_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/data_processors/interpolate_pose.py` & `Simba-UW-tf-dev-1.62.8/simba/data_processors/interpolate_pose.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/data_processors/directing_other_animals_calculator.py` & `Simba-UW-tf-dev-1.62.8/simba/data_processors/directing_other_animals_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/data_processors/timebins_movement_calculator.py` & `Simba-UW-tf-dev-1.62.8/simba/data_processors/timebins_movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/data_processors/severity_calculator.py` & `Simba-UW-tf-dev-1.62.8/simba/data_processors/severity_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/data_processors/pup_retrieval_calculator.py` & `Simba-UW-tf-dev-1.62.8/simba/data_processors/pup_retrieval_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/data_processors/pybursts_calculator.py` & `Simba-UW-tf-dev-1.62.8/simba/data_processors/pybursts_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/data_processors/severity_frame_based_calculator.py` & `Simba-UW-tf-dev-1.62.8/simba/data_processors/severity_frame_based_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/data_processors/kleinberg_calculator.py` & `Simba-UW-tf-dev-1.62.8/simba/data_processors/kleinberg_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/data_processors/movement_calculator.py` & `Simba-UW-tf-dev-1.62.8/simba/data_processors/movement_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store` & `Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store` & `Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png` & `Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png` & `Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png` & `Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png` & `Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/13.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png` & `Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png` & `Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png` & `Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png` & `Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png` & `Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png` & `Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png` & `Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png` & `Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png` & `Simba-UW-tf-dev-1.62.8/simba/pose_configurations_archive/pose_configurations_archive_1/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/model/train_rf.py` & `Simba-UW-tf-dev-1.62.8/simba/model/train_rf.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,14 @@
             if generate_features_importance_log in Options.PERFORM_FLAGS.value:
                 self.create_x_importance_log(self.rf_clf, self.feature_names, self.clf_name, self.eval_out_path)
             if generate_features_importance_bar_graph in Options.PERFORM_FLAGS.value:
                 self.create_x_importance_bar_chart(self.rf_clf, self.feature_names, self.clf_name, self.eval_out_path, feature_importance_bars)
             if generate_example_decision_tree_fancy in Options.PERFORM_FLAGS.value:
                 self.dviz_classification_visualization(self.x_train, self.y_train, self.clf_name, self.class_names, self.eval_out_path)
             if generate_shap_scores in Options.PERFORM_FLAGS.value:
-                print(shap_multiprocess)
                 if not shap_multiprocess in Options.PERFORM_FLAGS.value:
                     self.create_shap_log(ini_file_path=self.config_path,
                                          rf_clf=self.rf_clf,
                                          x_df=self.x_train,
                                          y_df=self.y_train,
                                          x_names=self.feature_names,
                                          clf_name=self.clf_name,
```

### Comparing `Simba-UW-tf-dev-1.62.7/simba/model/.DS_Store` & `Simba-UW-tf-dev-1.62.8/simba/model/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/model/inference_batch.py` & `Simba-UW-tf-dev-1.62.8/simba/model/inference_batch.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/model/grid_search_rf.py` & `Simba-UW-tf-dev-1.62.8/simba/model/grid_search_rf.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/model/inference_validation.py` & `Simba-UW-tf-dev-1.62.8/simba/model/inference_validation.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/roi_tools/ROI_time_bin_calculator.py` & `Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_time_bin_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/roi_tools/ROI_movement_analyzer.py` & `Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_movement_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/roi_tools/.DS_Store` & `Simba-UW-tf-dev-1.62.8/simba/roi_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/roi_tools/ROI_define.py` & `Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_define.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/roi_tools/ROI_reset.py` & `Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_reset.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/roi_tools/ROI_analyzer.py` & `Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/roi_tools/ROI_feature_analyzer.py` & `Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_feature_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/roi_tools/ROI_multiply.py` & `Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_multiply.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/roi_tools/ROI_size_calculations.py` & `Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_size_calculations.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/roi_tools/ROI_zoom.py` & `Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_zoom.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/roi_tools/ROI_directing_analyzer.py` & `Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_directing_analyzer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/roi_tools/ROI_move_shape.py` & `Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_move_shape.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/roi_tools/ROI_menus.py` & `Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/roi_tools/ROI_clf_calculator.py` & `Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_clf_calculator.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/roi_tools/ROI_image.py` & `Simba-UW-tf-dev-1.62.8/simba/roi_tools/ROI_image.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_importers/sleap_csv_importer.py` & `Simba-UW-tf-dev-1.62.8/simba/pose_importers/sleap_csv_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_importers/misc/.DS_Store` & `Simba-UW-tf-dev-1.62.8/simba/pose_importers/misc/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_importers/misc/apt_trk_importer.py` & `Simba-UW-tf-dev-1.62.8/simba/pose_importers/misc/apt_trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_importers/read_DANNCE_mat.py` & `Simba-UW-tf-dev-1.62.8/simba/pose_importers/read_DANNCE_mat.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_importers/.DS_Store` & `Simba-UW-tf-dev-1.62.8/simba/pose_importers/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_importers/sleap_h5_importer.py` & `Simba-UW-tf-dev-1.62.8/simba/pose_importers/sleap_h5_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_importers/madlc_importer.py` & `Simba-UW-tf-dev-1.62.8/simba/pose_importers/madlc_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_importers/sleap_slp_importer.py` & `Simba-UW-tf-dev-1.62.8/simba/pose_importers/sleap_slp_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_importers/import_mars.py` & `Simba-UW-tf-dev-1.62.8/simba/pose_importers/import_mars.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_importers/dlc_importer_csv.py` & `Simba-UW-tf-dev-1.62.8/simba/pose_importers/dlc_importer_csv.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_importers/trk_importer.py` & `Simba-UW-tf-dev-1.62.8/simba/pose_importers/trk_importer.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_configurations/.DS_Store` & `Simba-UW-tf-dev-1.62.8/simba/pose_configurations/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_configurations/bp_names/.DS_Store` & `Simba-UW-tf-dev-1.62.8/simba/pose_configurations/bp_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_configurations/bp_names/bp_names.csv` & `Simba-UW-tf-dev-1.62.8/simba/pose_configurations/bp_names/bp_names.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_configurations/no_animals/.DS_Store` & `Simba-UW-tf-dev-1.62.8/simba/pose_configurations/no_animals/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_configurations/configuration_names/.DS_Store` & `Simba-UW-tf-dev-1.62.8/simba/pose_configurations/configuration_names/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_configurations/schematics/8.png` & `Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/8.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_configurations/schematics/9.png` & `Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/9.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_configurations/schematics/12.png` & `Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/12.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_configurations/schematics/11.png` & `Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/11.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_configurations/schematics/10.png` & `Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/10.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_configurations/schematics/4.png` & `Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/4.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_configurations/schematics/5.png` & `Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/5.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_configurations/schematics/7.png` & `Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/7.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_configurations/schematics/6.png` & `Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/6.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_configurations/schematics/2.png` & `Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_configurations/schematics/3.png` & `Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/3.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/pose_configurations/schematics/1.png` & `Simba-UW-tf-dev-1.62.8/simba/pose_configurations/schematics/1.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/video_processors/video_processing.py` & `Simba-UW-tf-dev-1.62.8/simba/video_processors/video_processing.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/video_processors/.DS_Store` & `Simba-UW-tf-dev-1.62.8/simba/video_processors/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/video_processors/px_to_mm.py` & `Simba-UW-tf-dev-1.62.8/simba/video_processors/px_to_mm.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/video_processors/batch_process_menus.py` & `Simba-UW-tf-dev-1.62.8/simba/video_processors/batch_process_menus.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/video_processors/multi_cropper.py` & `Simba-UW-tf-dev-1.62.8/simba/video_processors/multi_cropper.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/video_processors/extract_frames.py` & `Simba-UW-tf-dev-1.62.8/simba/video_processors/extract_frames.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/video_processors/calculate_px_dist.py` & `Simba-UW-tf-dev-1.62.8/simba/video_processors/calculate_px_dist.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/video_processors/extract_seqframes.py` & `Simba-UW-tf-dev-1.62.8/simba/video_processors/extract_seqframes.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/video_processors/batch_process_create_ffmpeg_commands.py` & `Simba-UW-tf-dev-1.62.8/simba/video_processors/batch_process_create_ffmpeg_commands.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/outlier_tools/outlier_corrector_movement.py` & `Simba-UW-tf-dev-1.62.8/simba/outlier_tools/outlier_corrector_movement.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/outlier_tools/.DS_Store` & `Simba-UW-tf-dev-1.62.8/simba/outlier_tools/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/outlier_tools/outlier_corrector_location.py` & `Simba-UW-tf-dev-1.62.8/simba/outlier_tools/outlier_corrector_location.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/outlier_tools/skip_outlier_correction.py` & `Simba-UW-tf-dev-1.62.8/simba/outlier_tools/skip_outlier_correction.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/outlier_tools/.idea/outlier_scripts.iml` & `Simba-UW-tf-dev-1.62.8/simba/outlier_tools/.idea/outlier_scripts.iml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml` & `Simba-UW-tf-dev-1.62.8/simba/outlier_tools/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/outlier_tools/.idea/workspace.xml` & `Simba-UW-tf-dev-1.62.8/simba/outlier_tools/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/SimBA.py` & `Simba-UW-tf-dev-1.62.8/simba/SimBA.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/unsupervised/.DS_Store` & `Simba-UW-tf-dev-1.62.8/simba/assets/unsupervised/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/unsupervised/model_names.parquet` & `Simba-UW-tf-dev-1.62.8/simba/assets/unsupervised/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/unsupervised/features.csv` & `Simba-UW-tf-dev-1.62.8/simba/assets/unsupervised/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/shap/down_arrow.jpg` & `Simba-UW-tf-dev-1.62.8/simba/assets/shap/down_arrow.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/shap/intruder_shape.jpg` & `Simba-UW-tf-dev-1.62.8/simba/assets/shap/intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/shap/feature_categories/shap_feature_categories.csv` & `Simba-UW-tf-dev-1.62.8/simba/assets/shap/feature_categories/shap_feature_categories.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/shap/.DS_Store` & `Simba-UW-tf-dev-1.62.8/simba/assets/shap/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/shap/resident_shape.jpg` & `Simba-UW-tf-dev-1.62.8/simba/assets/shap/resident_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/shap/resident_intruder_shape.jpg` & `Simba-UW-tf-dev-1.62.8/simba/assets/shap/resident_intruder_shape.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/shap/animal_distances.jpg` & `Simba-UW-tf-dev-1.62.8/simba/assets/shap/animal_distances.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/shap/baseline_scale.jpg` & `Simba-UW-tf-dev-1.62.8/simba/assets/shap/baseline_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/shap/ubuntu.regular.ttf` & `Simba-UW-tf-dev-1.62.8/simba/assets/shap/ubuntu.regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/shap/side_scale.jpg` & `Simba-UW-tf-dev-1.62.8/simba/assets/shap/side_scale.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/shap/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.62.8/simba/assets/shap/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/shap/side_scale_5.jpg` & `Simba-UW-tf-dev-1.62.8/simba/assets/shap/side_scale_5.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/shap/intruder_movement.jpg` & `Simba-UW-tf-dev-1.62.8/simba/assets/shap/intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/shap/resident_movement.jpg` & `Simba-UW-tf-dev-1.62.8/simba/assets/shap/resident_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/shap/color_bar.jpg` & `Simba-UW-tf-dev-1.62.8/simba/assets/shap/color_bar.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/shap/resident_intruder_movement.jpg` & `Simba-UW-tf-dev-1.62.8/simba/assets/shap/resident_intruder_movement.jpg`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/.DS_Store` & `Simba-UW-tf-dev-1.62.8/simba/assets/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/lookups/.DS_Store` & `Simba-UW-tf-dev-1.62.8/simba/assets/lookups/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/lookups/model_names.parquet` & `Simba-UW-tf-dev-1.62.8/simba/assets/lookups/model_names.parquet`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/lookups/feature_extraction_headers.csv` & `Simba-UW-tf-dev-1.62.8/simba/assets/lookups/feature_extraction_headers.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/lookups/features.csv` & `Simba-UW-tf-dev-1.62.8/simba/assets/lookups/features.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/lookups/unsupervised_example_x.csv` & `Simba-UW-tf-dev-1.62.8/simba/assets/lookups/unsupervised_example_x.csv`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/stl/operant_tray.stl` & `Simba-UW-tf-dev-1.62.8/simba/assets/stl/operant_tray.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/stl/operant_lever.stl` & `Simba-UW-tf-dev-1.62.8/simba/assets/stl/operant_lever.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/stl/operant_walls.stl` & `Simba-UW-tf-dev-1.62.8/simba/assets/stl/operant_walls.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/stl/grid_floor.stl` & `Simba-UW-tf-dev-1.62.8/simba/assets/stl/grid_floor.stl`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/img/.DS_Store` & `Simba-UW-tf-dev-1.62.8/simba/assets/img/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/img/about_me.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/img/about_me.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/img/splash.mp4` & `Simba-UW-tf-dev-1.62.8/simba/assets/img/splash.mp4`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/img/bg_2.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/img/bg_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/img/splash.pptx` & `Simba-UW-tf-dev-1.62.8/simba/assets/img/splash.pptx`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/img/bg.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/img/bg.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/UbuntuMono-Regular.ttf` & `Simba-UW-tf-dev-1.62.8/simba/assets/UbuntuMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/factory.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/factory.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/cluster.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/cluster.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/load.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/load.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/gif.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/gif.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/pose.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/pose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/features.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/features.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/.DS_Store` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/.DS_Store`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/settings.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/settings.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/stopwatch.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/stopwatch.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/link.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/link.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/dash_simba.css` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/dash_simba.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/documentation.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/documentation.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/fps.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/fps.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/dimensionality_reduction.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/dimensionality_reduction.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/roi.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/roi.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/superimpose.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/superimpose.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/label.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/label.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/change.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/change.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/crop.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/crop.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/rotate.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/rotate.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/path.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/path.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/clip.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/clip.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/restart.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/restart.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/calipher.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/calipher.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/add_on.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/add_on.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/create.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/create.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/SimBA_logo.ico` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/SimBA_logo.ico`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/print.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/print.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/clf.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/clf.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/concat_icons/mosaic.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/concat_icons/mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/concat_icons/vertical.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/concat_icons/vertical.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/concat_icons/horizontal.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/concat_icons/horizontal.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/concat_icons/mixed_mosaic.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/concat_icons/mixed_mosaic.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/merge.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/merge.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/clean.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/clean.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/clf_2.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/clf_2.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/visualize.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/visualize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/concat.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/concat.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/boris.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/boris.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/frames.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/frames.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/video.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/video.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/sample.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/sample.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/metrics.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/metrics.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/grey.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/grey.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/exit.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/exit.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/outlier.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/outlier.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/clahe.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/clahe.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/trash.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/trash.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/about.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/about.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/convert.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/convert.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/SimBA_logo.icns` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/SimBA_logo.icns`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/reorganize.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/reorganize.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/browse.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/browse.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/SimBA_logo.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/SimBA_logo.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/ethovision.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/ethovision.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/icons/close.png` & `Simba-UW-tf-dev-1.62.8/simba/assets/icons/close.png`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/dash_simba_base.css` & `Simba-UW-tf-dev-1.62.8/simba/assets/dash_simba_base.css`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/simba/assets/TheGoldenLab.PNG` & `Simba-UW-tf-dev-1.62.8/simba/assets/TheGoldenLab.PNG`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/Simba_UW_tf_dev.egg-info/PKG-INFO` & `Simba-UW-tf-dev-1.62.8/Simba_UW_tf_dev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simba-UW-tf-dev
-Version: 1.62.7
+Version: 1.62.8
 Summary: Toolkit for computer classification of complex social behaviors in experimental animals
 Home-page: https://github.com/sgoldenlab/simba
 Author: Simon Nilsson, Jia Jie Choong, Sophia Hwang
 Author-email: sronilsson@gmail.com
 License: GNU Lesser General Public License v3 (LGPLv3)
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Simba-UW-tf-dev-1.62.7/Simba_UW_tf_dev.egg-info/SOURCES.txt` & `Simba-UW-tf-dev-1.62.8/Simba_UW_tf_dev.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -434,14 +434,15 @@
 simba/video_processors/calculate_px_dist.py
 simba/video_processors/extract_frames.py
 simba/video_processors/extract_seqframes.py
 simba/video_processors/multi_cropper.py
 simba/video_processors/px_to_mm.py
 simba/video_processors/video_processing.py
 tests/__init__.py
+tests/test_config_reader_mixin.py
 tests/test_data_processors.py
 tests/test_distance_plotter.py
 tests/test_feature_extraction_mixin.py
 tests/test_featurizers.py
 tests/test_outlier_correctors.py
 tests/test_thirdparty_appenders.py
 tests/test_train_model_mixin.py
```

### Comparing `Simba-UW-tf-dev-1.62.7/Simba_UW_tf_dev.egg-info/requires.txt` & `Simba-UW-tf-dev-1.62.8/Simba_UW_tf_dev.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/LICENSE.md` & `Simba-UW-tf-dev-1.62.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/tests/test_data_processors.py` & `Simba-UW-tf-dev-1.62.8/tests/test_data_processors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/tests/test_distance_plotter.py` & `Simba-UW-tf-dev-1.62.8/tests/test_distance_plotter.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/tests/test_feature_extraction_mixin.py` & `Simba-UW-tf-dev-1.62.8/tests/test_feature_extraction_mixin.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/tests/test_outlier_correctors.py` & `Simba-UW-tf-dev-1.62.8/tests/test_outlier_correctors.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/tests/test_visualize_directing_animals.py` & `Simba-UW-tf-dev-1.62.8/tests/test_visualize_directing_animals.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/tests/test_featurizers.py` & `Simba-UW-tf-dev-1.62.8/tests/test_featurizers.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py` & `Simba-UW-tf-dev-1.62.8/tests/data/test_projects/zebrafish/feature_file/fish_feature_extraction_092221.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/tests/test_thirdparty_appenders.py` & `Simba-UW-tf-dev-1.62.8/tests/test_thirdparty_appenders.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/tests/test_validation_clips.py` & `Simba-UW-tf-dev-1.62.8/tests/test_validation_clips.py`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/README.md` & `Simba-UW-tf-dev-1.62.8/README.md`

 * *Files identical despite different names*

### Comparing `Simba-UW-tf-dev-1.62.7/setup.py` & `Simba-UW-tf-dev-1.62.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Licensed under GNU Lesser General Public License v3.0
 """
 
 import setuptools
 
 setuptools.setup(
     name="Simba-UW-tf-dev",
-    version="1.62.7",
+    version="1.62.8",
     author="Simon Nilsson, Jia Jie Choong, Sophia Hwang",
     author_email="sronilsson@gmail.com",
     description="Toolkit for computer classification of complex social behaviors in experimental animals",
     url="https://github.com/sgoldenlab/simba",
     install_requires=['Pillow == 5.4.1', 'pyyaml == 5.3.1','shapely == 1.7','wxpython == 4.0.4',
               'dtreeviz == 0.8.1','eli5 == 0.10.1','graphviz == 0.11',
               'imblearn == 0.0','imgaug == 0.4.0','imutils == 0.5.2','matplotlib == 3.0.3', 'numpy == 1.18.1',
```

