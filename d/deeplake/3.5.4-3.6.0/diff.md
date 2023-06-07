# Comparing `tmp/deeplake-3.5.4.tar.gz` & `tmp/deeplake-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deeplake-3.5.4.tar", last modified: Thu Jun  1 16:59:07 2023, max compression
+gzip compressed data, was "deeplake-3.6.0.tar", last modified: Wed Jun  7 09:25:49 2023, max compression
```

## Comparing `deeplake-3.5.4.tar` & `deeplake-3.6.0.tar`

### file list

```diff
@@ -1,394 +1,398 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.610155 deeplake-3.5.4/
--rw-r--r--   0 root         (0) root         (0)    15975 2023-06-01 16:57:59.000000 deeplake-3.5.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       36 2023-06-01 16:57:59.000000 deeplake-3.5.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    25286 2023-06-01 16:59:07.610155 deeplake-3.5.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    24579 2023-06-01 16:57:59.000000 deeplake-3.5.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.580155 deeplake-3.5.4/deeplake/
--rw-r--r--   0 root         (0) root         (0)     2662 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.580155 deeplake-3.5.4/deeplake/api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    94609 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/dataset.py
--rw-r--r--   0 root         (0) root         (0)     4693 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/info.py
--rw-r--r--   0 root         (0) root         (0)     1203 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/link.py
--rw-r--r--   0 root         (0) root         (0)     1698 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/link_tiled.py
--rw-r--r--   0 root         (0) root         (0)     2703 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/read.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.580155 deeplake-3.5.4/deeplake/api/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3038 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_access_method.py
--rw-r--r--   0 root         (0) root         (0)     2098 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_agreement.py
--rw-r--r--   0 root         (0) root         (0)    84314 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_api.py
--rw-r--r--   0 root         (0) root         (0)     6968 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_api_tiling.py
--rw-r--r--   0 root         (0) root         (0)    11668 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_api_with_compression.py
--rw-r--r--   0 root         (0) root         (0)     2654 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_chunk_sizes.py
--rw-r--r--   0 root         (0) root         (0)     1797 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_connect_datasets.py
--rw-r--r--   0 root         (0) root         (0)     2997 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1500 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_dicom.py
--rw-r--r--   0 root         (0) root         (0)     6192 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_downsample.py
--rw-r--r--   0 root         (0) root         (0)      953 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_events.py
--rw-r--r--   0 root         (0) root         (0)     5056 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_grayscale.py
--rw-r--r--   0 root         (0) root         (0)      247 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_hosted_datasets.py
--rw-r--r--   0 root         (0) root         (0)     6513 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_info.py
--rw-r--r--   0 root         (0) root         (0)     6911 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_insertion_out_of_order.py
--rw-r--r--   0 root         (0) root         (0)     6823 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_json.py
--rw-r--r--   0 root         (0) root         (0)    23071 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_link.py
--rw-r--r--   0 root         (0) root         (0)     3293 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_link_tiled.py
--rw-r--r--   0 root         (0) root         (0)     1789 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_linking.py
--rw-r--r--   0 root         (0) root         (0)     1024 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_mesh.py
--rw-r--r--   0 root         (0) root         (0)     1235 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_meta.py
--rw-r--r--   0 root         (0) root         (0)     4109 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_nifti.py
--rw-r--r--   0 root         (0) root         (0)     7900 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_none.py
--rw-r--r--   0 root         (0) root         (0)      952 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_partial_upload.py
--rw-r--r--   0 root         (0) root         (0)     1605 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_pickle.py
--rw-r--r--   0 root         (0) root         (0)     5680 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_point_cloud.py
--rw-r--r--   0 root         (0) root         (0)     4249 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_polygons.py
--rw-r--r--   0 root         (0) root         (0)    10559 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_pop.py
--rw-r--r--   0 root         (0) root         (0)     1228 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_readonly.py
--rw-r--r--   0 root         (0) root         (0)    17730 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_rechunk.py
--rw-r--r--   0 root         (0) root         (0)     8477 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_reset.py
--rw-r--r--   0 root         (0) root         (0)     4578 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_sample_info.py
--rw-r--r--   0 root         (0) root         (0)     2982 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_text.py
--rw-r--r--   0 root         (0) root         (0)    14556 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_update_samples.py
--rw-r--r--   0 root         (0) root         (0)     7389 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_video.py
--rw-r--r--   0 root         (0) root         (0)     4153 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tests/test_views.py
--rw-r--r--   0 root         (0) root         (0)     1368 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/api/tiled.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.580155 deeplake-3.5.4/deeplake/auto/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/auto/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.580155 deeplake-3.5.4/deeplake/auto/structured/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/auto/structured/__init__.py
--rw-r--r--   0 root         (0) root         (0)      635 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/auto/structured/base.py
--rw-r--r--   0 root         (0) root         (0)     6666 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/auto/structured/dataframe.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.580155 deeplake-3.5.4/deeplake/auto/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/auto/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7975 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/auto/tests/test_coco_template.py
--rw-r--r--   0 root         (0) root         (0)    12440 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/auto/tests/test_ingestion.py
--rw-r--r--   0 root         (0) root         (0)     5371 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/auto/tests/test_kaggle.py
--rw-r--r--   0 root         (0) root         (0)     5519 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/auto/tests/test_yolo_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.580155 deeplake-3.5.4/deeplake/auto/unstructured/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/auto/unstructured/__init__.py
--rw-r--r--   0 root         (0) root         (0)      537 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/auto/unstructured/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.580155 deeplake-3.5.4/deeplake/auto/unstructured/coco/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/auto/unstructured/coco/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7093 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/auto/unstructured/coco/coco.py
--rw-r--r--   0 root         (0) root         (0)      669 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/auto/unstructured/coco/constants.py
--rw-r--r--   0 root         (0) root         (0)     1709 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/auto/unstructured/coco/convert.py
--rw-r--r--   0 root         (0) root         (0)     5237 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/auto/unstructured/coco/utils.py
--rw-r--r--   0 root         (0) root         (0)     6693 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/auto/unstructured/image_classification.py
--rw-r--r--   0 root         (0) root         (0)     3533 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/auto/unstructured/kaggle.py
--rw-r--r--   0 root         (0) root         (0)     4514 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/auto/unstructured/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.580155 deeplake-3.5.4/deeplake/auto/unstructured/yolo/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/auto/unstructured/yolo/__init__.py
--rw-r--r--   0 root         (0) root         (0)      278 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/auto/unstructured/yolo/constants.py
--rw-r--r--   0 root         (0) root         (0)     7394 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/auto/unstructured/yolo/utils.py
--rw-r--r--   0 root         (0) root         (0)    12937 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/auto/unstructured/yolo/yolo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.590155 deeplake-3.5.4/deeplake/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5913 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/cli/auth.py
--rw-r--r--   0 root         (0) root         (0)      410 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/cli/commands.py
--rw-r--r--   0 root         (0) root         (0)      931 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/cli/test_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.590155 deeplake-3.5.4/deeplake/client/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19270 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/client/client.py
--rw-r--r--   0 root         (0) root         (0)     1301 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/client/config.py
--rw-r--r--   0 root         (0) root         (0)      690 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/client/log.py
--rw-r--r--   0 root         (0) root         (0)     1536 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/client/test_client.py
--rw-r--r--   0 root         (0) root         (0)     3324 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/client/utils.py
--rw-r--r--   0 root         (0) root         (0)     3876 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/compression.py
--rw-r--r--   0 root         (0) root         (0)     6262 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.590155 deeplake-3.5.4/deeplake/core/
--rw-r--r--   0 root         (0) root         (0)       23 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.590155 deeplake-3.5.4/deeplake/core/chunk/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/chunk/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24150 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/chunk/base_chunk.py
--rw-r--r--   0 root         (0) root         (0)    25311 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/chunk/chunk_compressed_chunk.py
--rw-r--r--   0 root         (0) root         (0)     6147 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/chunk/sample_compressed_chunk.py
--rw-r--r--   0 root         (0) root         (0)     4926 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/chunk/test_chunk_compressed.py
--rw-r--r--   0 root         (0) root         (0)     4494 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/chunk/test_sample_compressed.py
--rw-r--r--   0 root         (0) root         (0)     5446 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/chunk/test_uncompressed.py
--rw-r--r--   0 root         (0) root         (0)     9633 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/chunk/uncompressed_chunk.py
--rw-r--r--   0 root         (0) root         (0)   113290 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/chunk_engine.py
--rw-r--r--   0 root         (0) root         (0)    39478 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/compression.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.590155 deeplake-3.5.4/deeplake/core/compute/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/compute/__init__.py
--rw-r--r--   0 root         (0) root         (0)      911 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/compute/process.py
--rw-r--r--   0 root         (0) root         (0)     2332 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/compute/provider.py
--rw-r--r--   0 root         (0) root         (0)      640 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/compute/ray.py
--rw-r--r--   0 root         (0) root         (0)      806 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/compute/serial.py
--rw-r--r--   0 root         (0) root         (0)      576 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/compute/thread.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.590155 deeplake-3.5.4/deeplake/core/dataset/
--rw-r--r--   0 root         (0) root         (0)      903 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)   170900 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/dataset/dataset.py
--rw-r--r--   0 root         (0) root         (0)    14805 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/dataset/deeplake_cloud_dataset.py
--rw-r--r--   0 root         (0) root         (0)    11965 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/dataset/deeplake_query_dataset.py
--rw-r--r--   0 root         (0) root         (0)     5265 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/dataset/deeplake_query_tensor.py
--rw-r--r--   0 root         (0) root         (0)      760 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/dataset/invalid_view.py
--rw-r--r--   0 root         (0) root         (0)     4769 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/dataset/view_entry.py
--rw-r--r--   0 root         (0) root         (0)     4348 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/fast_forwarding.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.590155 deeplake-3.5.4/deeplake/core/index/
--rw-r--r--   0 root         (0) root         (0)      138 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/index/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17507 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/index/index.py
--rw-r--r--   0 root         (0) root         (0)    19800 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/io.py
--rw-r--r--   0 root         (0) root         (0)     4121 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/ipc.py
--rw-r--r--   0 root         (0) root         (0)    11242 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/link_creds.py
--rw-r--r--   0 root         (0) root         (0)    15953 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/linked_chunk_engine.py
--rw-r--r--   0 root         (0) root         (0)     2277 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/linked_sample.py
--rw-r--r--   0 root         (0) root         (0)     2597 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/linked_tiled_sample.py
--rw-r--r--   0 root         (0) root         (0)     8835 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/lock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.590155 deeplake-3.5.4/deeplake/core/meta/
--rw-r--r--   0 root         (0) root         (0)       97 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3595 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/meta/dataset_meta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.590155 deeplake-3.5.4/deeplake/core/meta/encode/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/meta/encode/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25591 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/meta/encode/base_encoder.py
--rw-r--r--   0 root         (0) root         (0)     3915 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/meta/encode/byte_positions.py
--rw-r--r--   0 root         (0) root         (0)    13495 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/meta/encode/chunk_id.py
--rw-r--r--   0 root         (0) root         (0)     1551 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/meta/encode/creds.py
--rw-r--r--   0 root         (0) root         (0)     3972 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/meta/encode/pad.py
--rw-r--r--   0 root         (0) root         (0)      941 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/meta/encode/sequence.py
--rw-r--r--   0 root         (0) root         (0)      683 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/meta/encode/shape.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.590155 deeplake-3.5.4/deeplake/core/meta/encode/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/meta/encode/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      226 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/meta/encode/tests/common.py
--rw-r--r--   0 root         (0) root         (0)     2237 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py
--rw-r--r--   0 root         (0) root         (0)     1452 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py
--rw-r--r--   0 root         (0) root         (0)     2114 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py
--rw-r--r--   0 root         (0) root         (0)     3673 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/meta/encode/tests/test_shape_encoder.py
--rw-r--r--   0 root         (0) root         (0)     2810 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py
--rw-r--r--   0 root         (0) root         (0)     7515 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/meta/encode/tile.py
--rw-r--r--   0 root         (0) root         (0)      503 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/meta/meta.py
--rw-r--r--   0 root         (0) root         (0)    13344 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/meta/tensor_meta.py
--rw-r--r--   0 root         (0) root         (0)      906 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/partial_reader.py
--rw-r--r--   0 root         (0) root         (0)      961 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/partial_sample.py
--rw-r--r--   0 root         (0) root         (0)     5269 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/polygon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.590155 deeplake-3.5.4/deeplake/core/query/
--rw-r--r--   0 root         (0) root         (0)       82 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/query/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12021 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/query/autocomplete.py
--rw-r--r--   0 root         (0) root         (0)    14326 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/query/filter.py
--rw-r--r--   0 root         (0) root         (0)     8905 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/query/query.py
--rw-r--r--   0 root         (0) root         (0)    19976 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/sample.py
--rw-r--r--   0 root         (0) root         (0)    22849 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.590155 deeplake-3.5.4/deeplake/core/storage/
--rw-r--r--   0 root         (0) root         (0)      441 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1053 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/storage/deeplake_memory_object.py
--rw-r--r--   0 root         (0) root         (0)    19080 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/storage/gcs.py
--rw-r--r--   0 root         (0) root         (0)    13053 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/storage/google_drive.py
--rw-r--r--   0 root         (0) root         (0)     8347 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/storage/local.py
--rw-r--r--   0 root         (0) root         (0)    19492 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/storage/lru_cache.py
--rw-r--r--   0 root         (0) root         (0)     3705 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/storage/memory.py
--rw-r--r--   0 root         (0) root         (0)     7111 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/storage/provider.py
--rw-r--r--   0 root         (0) root         (0)    25686 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/storage/s3.py
--rw-r--r--   0 root         (0) root         (0)    50140 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/tensor.py
--rw-r--r--   0 root         (0) root         (0)     7485 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/tensor_link.py
--rw-r--r--   0 root         (0) root         (0)     5152 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/test_serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.590155 deeplake-3.5.4/deeplake/core/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7602 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/tests/test_compression.py
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/tests/test_compute.py
--rw-r--r--   0 root         (0) root         (0)    12386 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/tests/test_deeplake_indra_dataset.py
--rw-r--r--   0 root         (0) root         (0)      913 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/tests/test_io.py
--rw-r--r--   0 root         (0) root         (0)     4164 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/tests/test_locking.py
--rw-r--r--   0 root         (0) root         (0)      654 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/tests/test_readonly.py
--rw-r--r--   0 root         (0) root         (0)     1425 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/tests/test_serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.590155 deeplake-3.5.4/deeplake/core/tiling/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/tiling/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4790 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/tiling/deserialize.py
--rw-r--r--   0 root         (0) root         (0)     1701 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/tiling/optimizer.py
--rw-r--r--   0 root         (0) root         (0)     4731 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/tiling/sample_tiles.py
--rw-r--r--   0 root         (0) root         (0)     2893 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/tiling/serialize.py
--rw-r--r--   0 root         (0) root         (0)     1950 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/tiling/test_optimizer.py
--rw-r--r--   0 root         (0) root         (0)     2367 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/tiling/test_serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.590155 deeplake-3.5.4/deeplake/core/transform/
--rw-r--r--   0 root         (0) root         (0)      111 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/transform/__init__.py
--rw-r--r--   0 root         (0) root         (0)    51192 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/transform/test_transform.py
--rw-r--r--   0 root         (0) root         (0)    29318 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/transform/transform.py
--rw-r--r--   0 root         (0) root         (0)     5860 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/transform/transform_dataset.py
--rw-r--r--   0 root         (0) root         (0)     4391 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/transform/transform_tensor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.590155 deeplake-3.5.4/deeplake/core/vectorstore/
--rw-r--r--   0 root         (0) root         (0)      509 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12123 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/deeplake_vectorstore.py
--rw-r--r--   0 root         (0) root         (0)     5044 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/test_deeplake_vectorstore.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.590155 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.590155 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/dataset/
--rw-r--r--   0 root         (0) root         (0)      246 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8071 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/dataset/dataset.py
--rw-r--r--   0 root         (0) root         (0)     7799 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.590155 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/filter/
--rw-r--r--   0 root         (0) root         (0)      237 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/filter/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3147 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/filter/filter.py
--rw-r--r--   0 root         (0) root         (0)     3352 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/filter/test_filter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.600155 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/indra/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/indra/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1439 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/indra/indra_vector_search.py
--rw-r--r--   0 root         (0) root         (0)     3397 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/indra/query.py
--rw-r--r--   0 root         (0) root         (0)      541 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/indra/remote_engine_search.py
--rw-r--r--   0 root         (0) root         (0)     1799 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/indra/test_indra.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.600155 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/
--rw-r--r--   0 root         (0) root         (0)      275 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/__init__.py
--rw-r--r--   0 root         (0) root         (0)      721 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py
--rw-r--r--   0 root         (0) root         (0)      186 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/order.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.600155 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/ingestion/
--rw-r--r--   0 root         (0) root         (0)       93 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/ingestion/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5964 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py
--rw-r--r--   0 root         (0) root         (0)     1595 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py
--rw-r--r--   0 root         (0) root         (0)     3703 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.600155 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/python/
--rw-r--r--   0 root         (0) root         (0)       85 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/python/__init__.py
--rw-r--r--   0 root         (0) root         (0)      378 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/python/test_vector_search.py
--rw-r--r--   0 root         (0) root         (0)     1464 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/python/vector_search.py
--rw-r--r--   0 root         (0) root         (0)     2010 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/utils.py
--rw-r--r--   0 root         (0) root         (0)     2184 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/vectorstore/vector_search/vector_search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.600155 deeplake-3.5.4/deeplake/core/version_control/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/version_control/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1954 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/version_control/commit_chunk_map.py
--rw-r--r--   0 root         (0) root         (0)     6337 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/version_control/commit_diff.py
--rw-r--r--   0 root         (0) root         (0)     3109 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/version_control/commit_node.py
--rw-r--r--   0 root         (0) root         (0)     4828 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/version_control/dataset_diff.py
--rw-r--r--   0 root         (0) root         (0)    19869 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/version_control/test_merge.py
--rw-r--r--   0 root         (0) root         (0)    84800 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/core/version_control/test_version_control.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.600155 deeplake-3.5.4/deeplake/enterprise/
--rw-r--r--   0 root         (0) root         (0)      257 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/enterprise/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6781 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/enterprise/convert_to_libdeeplake.py
--rw-r--r--   0 root         (0) root         (0)    29584 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/enterprise/dataloader.py
--rw-r--r--   0 root         (0) root         (0)     6010 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/enterprise/dummy_dataloader.py
--rw-r--r--   0 root         (0) root         (0)     4391 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/enterprise/libdeeplake_query.py
--rw-r--r--   0 root         (0) root         (0)    25897 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/enterprise/test_pytorch.py
--rw-r--r--   0 root         (0) root         (0)     1622 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/enterprise/test_query.py
--rw-r--r--   0 root         (0) root         (0)    22353 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/enterprise/test_tensorflow.py
--rw-r--r--   0 root         (0) root         (0)     1595 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/enterprise/util.py
--rw-r--r--   0 root         (0) root         (0)     1590 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/hooks.py
--rw-r--r--   0 root         (0) root         (0)     5050 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/htype.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.600155 deeplake-3.5.4/deeplake/integrations/
--rw-r--r--   0 root         (0) root         (0)       99 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/integrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.600155 deeplake-3.5.4/deeplake/integrations/huggingface/
--rw-r--r--   0 root         (0) root         (0)       44 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/integrations/huggingface/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5463 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/integrations/huggingface/huggingface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.600155 deeplake-3.5.4/deeplake/integrations/mmdet/
--rw-r--r--   0 root         (0) root         (0)      118 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/integrations/mmdet/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62754 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/integrations/mmdet/mmdet_.py
--rw-r--r--   0 root         (0) root         (0)     4739 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/integrations/mmdet/mmdet_runners.py
--rw-r--r--   0 root         (0) root         (0)    19660 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/integrations/mmdet/mmdet_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.600155 deeplake-3.5.4/deeplake/integrations/pytorch/
--rw-r--r--   0 root         (0) root         (0)       40 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/integrations/pytorch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9772 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/integrations/pytorch/common.py
--rw-r--r--   0 root         (0) root         (0)     7140 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/integrations/pytorch/dataset.py
--rw-r--r--   0 root         (0) root         (0)     4245 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/integrations/pytorch/pytorch.py
--rw-r--r--   0 root         (0) root         (0)     6919 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/integrations/pytorch/shuffle_buffer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.600155 deeplake-3.5.4/deeplake/integrations/tf/
--rw-r--r--   0 root         (0) root         (0)      135 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/integrations/tf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1270 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/integrations/tf/common.py
--rw-r--r--   0 root         (0) root         (0)     2453 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/integrations/tf/datasettotensorflow.py
--rw-r--r--   0 root         (0) root         (0)     5330 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/integrations/tf/deeplake_tensorflow_dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.600155 deeplake-3.5.4/deeplake/integrations/wandb/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/integrations/wandb/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12089 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/integrations/wandb/wandb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.600155 deeplake-3.5.4/deeplake/requirements/
--rw-r--r--   0 root         (0) root         (0)      432 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/requirements/common.txt
--rw-r--r--   0 root         (0) root         (0)       71 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/requirements/docs.txt
--rw-r--r--   0 root         (0) root         (0)      381 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/requirements/plugins.txt
--rw-r--r--   0 root         (0) root         (0)      304 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/requirements/tests.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.600155 deeplake-3.5.4/deeplake/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1404 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/tests/cache_fixtures.py
--rw-r--r--   0 root         (0) root         (0)     2559 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/tests/client_fixtures.py
--rw-r--r--   0 root         (0) root         (0)     4072 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/tests/common.py
--rw-r--r--   0 root         (0) root         (0)     3621 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/tests/dataset_fixtures.py
--rw-r--r--   0 root         (0) root         (0)    15328 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/tests/path_fixtures.py
--rw-r--r--   0 root         (0) root         (0)     2248 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/tests/storage_fixtures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.600155 deeplake-3.5.4/deeplake/util/
--rw-r--r--   0 root         (0) root         (0)       86 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3531 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/access_method.py
--rw-r--r--   0 root         (0) root         (0)     1130 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/agreement.py
--rw-r--r--   0 root         (0) root         (0)     1567 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/array_list.py
--rw-r--r--   0 root         (0) root         (0)      619 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/assert_byte_indexes.py
--rw-r--r--   0 root         (0) root         (0)     2961 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/auto.py
--rw-r--r--   0 root         (0) root         (0)     5623 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/bugout_reporter.py
--rw-r--r--   0 root         (0) root         (0)       54 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/bugout_token.py
--rw-r--r--   0 root         (0) root         (0)     3623 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/cache_chain.py
--rw-r--r--   0 root         (0) root         (0)     4494 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/casting.py
--rw-r--r--   0 root         (0) root         (0)      310 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/check_installation.py
--rw-r--r--   0 root         (0) root         (0)     1197 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/check_latest_version.py
--rw-r--r--   0 root         (0) root         (0)     3172 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/chunk_engine.py
--rw-r--r--   0 root         (0) root         (0)     4597 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/class_label.py
--rw-r--r--   0 root         (0) root         (0)      231 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/compression.py
--rw-r--r--   0 root         (0) root         (0)     1197 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/compute.py
--rw-r--r--   0 root         (0) root         (0)     5381 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/connect_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1170 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/dataset.py
--rw-r--r--   0 root         (0) root         (0)      443 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/delete_entry.py
--rw-r--r--   0 root         (0) root         (0)    15912 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/diff.py
--rw-r--r--   0 root         (0) root         (0)     4945 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/downsample.py
--rw-r--r--   0 root         (0) root         (0)       84 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/empty_sample.py
--rw-r--r--   0 root         (0) root         (0)    15682 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/encoder.py
--rw-r--r--   0 root         (0) root         (0)    34711 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2026 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/exif.py
--rw-r--r--   0 root         (0) root         (0)     1819 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/from_tfds.py
--rw-r--r--   0 root         (0) root         (0)      136 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/generate_id.py
--rw-r--r--   0 root         (0) root         (0)      306 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/hash.py
--rw-r--r--   0 root         (0) root         (0)     2799 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/htype.py
--rw-r--r--   0 root         (0) root         (0)     1517 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/image.py
--rw-r--r--   0 root         (0) root         (0)      873 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/invalid_view_op.py
--rw-r--r--   0 root         (0) root         (0)      135 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/iterable_ordered_dict.py
--rw-r--r--   0 root         (0) root         (0)     1001 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/iteration_warning.py
--rw-r--r--   0 root         (0) root         (0)      507 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/join_chunks.py
--rw-r--r--   0 root         (0) root         (0)     6422 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/json.py
--rw-r--r--   0 root         (0) root         (0)     7261 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/keys.py
--rw-r--r--   0 root         (0) root         (0)     2996 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/link.py
--rw-r--r--   0 root         (0) root         (0)     1646 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/logging.py
--rw-r--r--   0 root         (0) root         (0)    37497 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/merge.py
--rw-r--r--   0 root         (0) root         (0)     2426 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/modified.py
--rw-r--r--   0 root         (0) root         (0)      903 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/notebook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.610155 deeplake-3.5.4/deeplake/util/object_3d/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/object_3d/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3374 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/object_3d/mesh.py
--rw-r--r--   0 root         (0) root         (0)      185 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/object_3d/mesh_parser.py
--rw-r--r--   0 root         (0) root         (0)      185 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/object_3d/mesh_reader.py
--rw-r--r--   0 root         (0) root         (0)     1021 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/object_3d/object_base_3d.py
--rw-r--r--   0 root         (0) root         (0)      695 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/object_3d/ply_parser.py
--rw-r--r--   0 root         (0) root         (0)     1323 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/object_3d/ply_parser_base.py
--rw-r--r--   0 root         (0) root         (0)     6188 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/object_3d/ply_parsers.py
--rw-r--r--   0 root         (0) root         (0)     1663 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/object_3d/ply_reader.py
--rw-r--r--   0 root         (0) root         (0)     3221 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/object_3d/ply_reader_base.py
--rw-r--r--   0 root         (0) root         (0)    10213 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/object_3d/ply_readers.py
--rw-r--r--   0 root         (0) root         (0)     7187 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/object_3d/point_cloud.py
--rw-r--r--   0 root         (0) root         (0)     1160 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/object_3d/read_3d_data.py
--rw-r--r--   0 root         (0) root         (0)     3914 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/path.py
--rw-r--r--   0 root         (0) root         (0)     3337 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/pretty_print.py
--rw-r--r--   0 root         (0) root         (0)     2763 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/remove_cache.py
--rw-r--r--   0 root         (0) root         (0)     4127 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/scheduling.py
--rw-r--r--   0 root         (0) root         (0)     2892 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/shape_interval.py
--rw-r--r--   0 root         (0) root         (0)      182 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/shuffle.py
--rw-r--r--   0 root         (0) root         (0)     4224 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/spinner.py
--rw-r--r--   0 root         (0) root         (0)     1153 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/split.py
--rw-r--r--   0 root         (0) root         (0)     8347 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/storage.py
--rw-r--r--   0 root         (0) root         (0)     1131 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/tag.py
--rw-r--r--   0 root         (0) root         (0)      951 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/testing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.610155 deeplake-3.5.4/deeplake/util/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1476 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/tests/test_auto.py
--rw-r--r--   0 root         (0) root         (0)     1757 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/tests/test_connect_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1239 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/tests/test_iterable_ordered_dict.py
--rw-r--r--   0 root         (0) root         (0)      892 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/tests/test_read.py
--rw-r--r--   0 root         (0) root         (0)     1071 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/tests/test_shape_interval.py
--rw-r--r--   0 root         (0) root         (0)      407 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/tests/test_shuffle.py
--rw-r--r--   0 root         (0) root         (0)      698 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/tests/test_split.py
--rw-r--r--   0 root         (0) root         (0)      266 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/tests/test_token.py
--rw-r--r--   0 root         (0) root         (0)     2428 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/tests/test_version_control.py
--rw-r--r--   0 root         (0) root         (0)      276 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/threading.py
--rw-r--r--   0 root         (0) root         (0)      381 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/token.py
--rw-r--r--   0 root         (0) root         (0)    25208 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/transform.py
--rw-r--r--   0 root         (0) root         (0)    31615 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/version_control.py
--rw-r--r--   0 root         (0) root         (0)      927 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/video.py
--rw-r--r--   0 root         (0) root         (0)      167 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/util/warnings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.610155 deeplake-3.5.4/deeplake/visualizer/
--rw-r--r--   0 root         (0) root         (0)       34 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/visualizer/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6466 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/visualizer/video_streaming.py
--rw-r--r--   0 root         (0) root         (0)     6722 2023-06-01 16:57:59.000000 deeplake-3.5.4/deeplake/visualizer/visualizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 16:59:07.580155 deeplake-3.5.4/deeplake.egg-info/
--rw-r--r--   0 root         (0) root         (0)    25286 2023-06-01 16:59:07.000000 deeplake-3.5.4/deeplake.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12524 2023-06-01 16:59:07.000000 deeplake-3.5.4/deeplake.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 16:59:07.000000 deeplake-3.5.4/deeplake.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2023-06-01 16:59:07.000000 deeplake-3.5.4/deeplake.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 16:59:07.000000 deeplake-3.5.4/deeplake.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      978 2023-06-01 16:59:07.000000 deeplake-3.5.4/deeplake.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-01 16:59:07.000000 deeplake-3.5.4/deeplake.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      311 2023-06-01 16:59:07.610155 deeplake-3.5.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3289 2023-06-01 16:57:59.000000 deeplake-3.5.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:25:49.882888 deeplake-3.6.0/
+-rw-r--r--   0 root         (0) root         (0)    15975 2023-06-07 09:24:16.000000 deeplake-3.6.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       36 2023-06-07 09:24:16.000000 deeplake-3.6.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    26080 2023-06-07 09:25:49.882888 deeplake-3.6.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    25351 2023-06-07 09:24:16.000000 deeplake-3.6.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:25:49.852888 deeplake-3.6.0/deeplake/
+-rw-r--r--   0 root         (0) root         (0)     2662 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:25:49.852888 deeplake-3.6.0/deeplake/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    96139 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/api/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4693 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/api/info.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/api/link.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/api/link_tiled.py
+-rw-r--r--   0 root         (0) root         (0)     2703 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/api/read.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:25:49.862888 deeplake-3.6.0/deeplake/api/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/api/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3038 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/api/tests/test_access_method.py
+-rw-r--r--   0 root         (0) root         (0)     2098 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/api/tests/test_agreement.py
+-rw-r--r--   0 root         (0) root         (0)    85001 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/api/tests/test_api.py
+-rw-r--r--   0 root         (0) root         (0)     6968 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/api/tests/test_api_tiling.py
+-rw-r--r--   0 root         (0) root         (0)    11668 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/api/tests/test_api_with_compression.py
+-rw-r--r--   0 root         (0) root         (0)     2654 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/api/tests/test_chunk_sizes.py
+-rw-r--r--   0 root         (0) root         (0)     1797 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/api/tests/test_connect_datasets.py
+-rw-r--r--   0 root         (0) root         (0)     2997 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/api/tests/test_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/api/tests/test_dicom.py
+-rw-r--r--   0 root         (0) root         (0)     6192 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/api/tests/test_downsample.py
+-rw-r--r--   0 root         (0) root         (0)      953 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/api/tests/test_events.py
+-rw-r--r--   0 root         (0) root         (0)     5056 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/api/tests/test_grayscale.py
+-rw-r--r--   0 root         (0) root         (0)      247 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/api/tests/test_hosted_datasets.py
+-rw-r--r--   0 root         (0) root         (0)     6513 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/api/tests/test_info.py
+-rw-r--r--   0 root         (0) root         (0)     6911 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/api/tests/test_insertion_out_of_order.py
+-rw-r--r--   0 root         (0) root         (0)     6823 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/api/tests/test_json.py
+-rw-r--r--   0 root         (0) root         (0)    23489 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/api/tests/test_link.py
+-rw-r--r--   0 root         (0) root         (0)     3293 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/api/tests/test_link_tiled.py
+-rw-r--r--   0 root         (0) root         (0)     1789 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/api/tests/test_linking.py
+-rw-r--r--   0 root         (0) root         (0)     1024 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/api/tests/test_mesh.py
+-rw-r--r--   0 root         (0) root         (0)     1235 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/api/tests/test_meta.py
+-rw-r--r--   0 root         (0) root         (0)     4109 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/api/tests/test_nifti.py
+-rw-r--r--   0 root         (0) root         (0)     7900 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/api/tests/test_none.py
+-rw-r--r--   0 root         (0) root         (0)      952 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/api/tests/test_partial_upload.py
+-rw-r--r--   0 root         (0) root         (0)     1605 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/api/tests/test_pickle.py
+-rw-r--r--   0 root         (0) root         (0)     5680 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/api/tests/test_point_cloud.py
+-rw-r--r--   0 root         (0) root         (0)     4249 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/api/tests/test_polygons.py
+-rw-r--r--   0 root         (0) root         (0)    10559 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/api/tests/test_pop.py
+-rw-r--r--   0 root         (0) root         (0)     1228 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/api/tests/test_readonly.py
+-rw-r--r--   0 root         (0) root         (0)    17730 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/api/tests/test_rechunk.py
+-rw-r--r--   0 root         (0) root         (0)     8477 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/api/tests/test_reset.py
+-rw-r--r--   0 root         (0) root         (0)     4578 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/api/tests/test_sample_info.py
+-rw-r--r--   0 root         (0) root         (0)     2982 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/api/tests/test_text.py
+-rw-r--r--   0 root         (0) root         (0)    14556 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/api/tests/test_update_samples.py
+-rw-r--r--   0 root         (0) root         (0)     7499 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/api/tests/test_video.py
+-rw-r--r--   0 root         (0) root         (0)     4153 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/api/tests/test_views.py
+-rw-r--r--   0 root         (0) root         (0)     1368 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/api/tiled.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:25:49.862888 deeplake-3.6.0/deeplake/auto/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/auto/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:25:49.862888 deeplake-3.6.0/deeplake/auto/structured/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/auto/structured/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      635 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/auto/structured/base.py
+-rw-r--r--   0 root         (0) root         (0)     6666 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/auto/structured/dataframe.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:25:49.862888 deeplake-3.6.0/deeplake/auto/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/auto/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7975 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/auto/tests/test_coco_template.py
+-rw-r--r--   0 root         (0) root         (0)    12440 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/auto/tests/test_ingestion.py
+-rw-r--r--   0 root         (0) root         (0)     5371 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/auto/tests/test_kaggle.py
+-rw-r--r--   0 root         (0) root         (0)     5519 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/auto/tests/test_yolo_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:25:49.862888 deeplake-3.6.0/deeplake/auto/unstructured/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/auto/unstructured/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      537 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/auto/unstructured/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:25:49.862888 deeplake-3.6.0/deeplake/auto/unstructured/coco/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/auto/unstructured/coco/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7093 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/auto/unstructured/coco/coco.py
+-rw-r--r--   0 root         (0) root         (0)      669 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/auto/unstructured/coco/constants.py
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/auto/unstructured/coco/convert.py
+-rw-r--r--   0 root         (0) root         (0)     5237 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/auto/unstructured/coco/utils.py
+-rw-r--r--   0 root         (0) root         (0)     6693 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/auto/unstructured/image_classification.py
+-rw-r--r--   0 root         (0) root         (0)     3533 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/auto/unstructured/kaggle.py
+-rw-r--r--   0 root         (0) root         (0)     4514 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/auto/unstructured/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:25:49.862888 deeplake-3.6.0/deeplake/auto/unstructured/yolo/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/auto/unstructured/yolo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      278 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/auto/unstructured/yolo/constants.py
+-rw-r--r--   0 root         (0) root         (0)     7394 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/auto/unstructured/yolo/utils.py
+-rw-r--r--   0 root         (0) root         (0)    12937 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/auto/unstructured/yolo/yolo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:25:49.862888 deeplake-3.6.0/deeplake/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5913 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/cli/auth.py
+-rw-r--r--   0 root         (0) root         (0)      410 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/cli/commands.py
+-rw-r--r--   0 root         (0) root         (0)      931 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/cli/test_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:25:49.862888 deeplake-3.6.0/deeplake/client/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19099 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     1301 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/client/config.py
+-rw-r--r--   0 root         (0) root         (0)      690 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/client/log.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/client/test_client.py
+-rw-r--r--   0 root         (0) root         (0)     3324 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/client/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3876 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/compression.py
+-rw-r--r--   0 root         (0) root         (0)     7357 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:25:49.862888 deeplake-3.6.0/deeplake/core/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:25:49.862888 deeplake-3.6.0/deeplake/core/chunk/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/chunk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24150 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/chunk/base_chunk.py
+-rw-r--r--   0 root         (0) root         (0)    25311 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/chunk/chunk_compressed_chunk.py
+-rw-r--r--   0 root         (0) root         (0)     6147 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/chunk/sample_compressed_chunk.py
+-rw-r--r--   0 root         (0) root         (0)     4926 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/chunk/test_chunk_compressed.py
+-rw-r--r--   0 root         (0) root         (0)     4494 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/chunk/test_sample_compressed.py
+-rw-r--r--   0 root         (0) root         (0)     5446 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/chunk/test_uncompressed.py
+-rw-r--r--   0 root         (0) root         (0)     9633 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/chunk/uncompressed_chunk.py
+-rw-r--r--   0 root         (0) root         (0)   113335 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/chunk_engine.py
+-rw-r--r--   0 root         (0) root         (0)    39478 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/compression.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:25:49.862888 deeplake-3.6.0/deeplake/core/compute/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/compute/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      911 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/compute/process.py
+-rw-r--r--   0 root         (0) root         (0)     2332 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/compute/provider.py
+-rw-r--r--   0 root         (0) root         (0)      640 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/compute/ray.py
+-rw-r--r--   0 root         (0) root         (0)      806 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/compute/serial.py
+-rw-r--r--   0 root         (0) root         (0)      576 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/compute/thread.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:25:49.862888 deeplake-3.6.0/deeplake/core/dataset/
+-rw-r--r--   0 root         (0) root         (0)      903 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   171173 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/dataset/dataset.py
+-rw-r--r--   0 root         (0) root         (0)    14834 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/dataset/deeplake_cloud_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    11965 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/dataset/deeplake_query_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     5265 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/dataset/deeplake_query_tensor.py
+-rw-r--r--   0 root         (0) root         (0)      760 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/dataset/invalid_view.py
+-rw-r--r--   0 root         (0) root         (0)     4769 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/dataset/view_entry.py
+-rw-r--r--   0 root         (0) root         (0)     4348 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/fast_forwarding.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:25:49.862888 deeplake-3.6.0/deeplake/core/index/
+-rw-r--r--   0 root         (0) root         (0)      138 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/index/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17507 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/index/index.py
+-rw-r--r--   0 root         (0) root         (0)    19800 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/io.py
+-rw-r--r--   0 root         (0) root         (0)     4121 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/ipc.py
+-rw-r--r--   0 root         (0) root         (0)    12418 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/link_creds.py
+-rw-r--r--   0 root         (0) root         (0)    15995 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/linked_chunk_engine.py
+-rw-r--r--   0 root         (0) root         (0)     2277 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/linked_sample.py
+-rw-r--r--   0 root         (0) root         (0)     2597 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/linked_tiled_sample.py
+-rw-r--r--   0 root         (0) root         (0)     8835 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/lock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:25:49.862888 deeplake-3.6.0/deeplake/core/meta/
+-rw-r--r--   0 root         (0) root         (0)       97 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/meta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3595 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/meta/dataset_meta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:25:49.862888 deeplake-3.6.0/deeplake/core/meta/encode/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/meta/encode/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25591 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/meta/encode/base_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     3915 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/meta/encode/byte_positions.py
+-rw-r--r--   0 root         (0) root         (0)    13495 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/meta/encode/chunk_id.py
+-rw-r--r--   0 root         (0) root         (0)     1551 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/meta/encode/creds.py
+-rw-r--r--   0 root         (0) root         (0)     3972 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/meta/encode/pad.py
+-rw-r--r--   0 root         (0) root         (0)      941 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/meta/encode/sequence.py
+-rw-r--r--   0 root         (0) root         (0)      683 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/meta/encode/shape.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:25:49.872888 deeplake-3.6.0/deeplake/core/meta/encode/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/meta/encode/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      226 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/meta/encode/tests/common.py
+-rw-r--r--   0 root         (0) root         (0)     2237 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     1452 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py
+-rw-r--r--   0 root         (0) root         (0)     2114 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     3673 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/meta/encode/tests/test_shape_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     2810 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py
+-rw-r--r--   0 root         (0) root         (0)     7515 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/meta/encode/tile.py
+-rw-r--r--   0 root         (0) root         (0)      503 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/meta/meta.py
+-rw-r--r--   0 root         (0) root         (0)    13344 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/meta/tensor_meta.py
+-rw-r--r--   0 root         (0) root         (0)      906 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/partial_reader.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/partial_sample.py
+-rw-r--r--   0 root         (0) root         (0)     5269 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/polygon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:25:49.872888 deeplake-3.6.0/deeplake/core/query/
+-rw-r--r--   0 root         (0) root         (0)       82 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/query/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12021 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/query/autocomplete.py
+-rw-r--r--   0 root         (0) root         (0)    14326 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/query/filter.py
+-rw-r--r--   0 root         (0) root         (0)     8905 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/query/query.py
+-rw-r--r--   0 root         (0) root         (0)    20658 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/sample.py
+-rw-r--r--   0 root         (0) root         (0)    22849 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:25:49.872888 deeplake-3.6.0/deeplake/core/storage/
+-rw-r--r--   0 root         (0) root         (0)      495 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13705 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/storage/azure.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/storage/deeplake_memory_object.py
+-rw-r--r--   0 root         (0) root         (0)    19080 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/storage/gcs.py
+-rw-r--r--   0 root         (0) root         (0)    13053 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/storage/google_drive.py
+-rw-r--r--   0 root         (0) root         (0)     8347 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/storage/local.py
+-rw-r--r--   0 root         (0) root         (0)    19492 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/storage/lru_cache.py
+-rw-r--r--   0 root         (0) root         (0)     3705 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/storage/memory.py
+-rw-r--r--   0 root         (0) root         (0)     7111 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/storage/provider.py
+-rw-r--r--   0 root         (0) root         (0)    25799 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/storage/s3.py
+-rw-r--r--   0 root         (0) root         (0)    50140 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/tensor.py
+-rw-r--r--   0 root         (0) root         (0)     7485 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/tensor_link.py
+-rw-r--r--   0 root         (0) root         (0)     5152 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/test_serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:25:49.872888 deeplake-3.6.0/deeplake/core/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7602 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/tests/test_compression.py
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/tests/test_compute.py
+-rw-r--r--   0 root         (0) root         (0)    12807 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/tests/test_deeplake_indra_dataset.py
+-rw-r--r--   0 root         (0) root         (0)      913 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/tests/test_io.py
+-rw-r--r--   0 root         (0) root         (0)     4312 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/tests/test_locking.py
+-rw-r--r--   0 root         (0) root         (0)      654 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/tests/test_readonly.py
+-rw-r--r--   0 root         (0) root         (0)     1425 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/tests/test_serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:25:49.872888 deeplake-3.6.0/deeplake/core/tiling/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/tiling/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4790 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/tiling/deserialize.py
+-rw-r--r--   0 root         (0) root         (0)     1701 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/tiling/optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     4731 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/tiling/sample_tiles.py
+-rw-r--r--   0 root         (0) root         (0)     2893 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/tiling/serialize.py
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/tiling/test_optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     2367 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/tiling/test_serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:25:49.872888 deeplake-3.6.0/deeplake/core/transform/
+-rw-r--r--   0 root         (0) root         (0)      111 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/transform/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    51556 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/transform/test_transform.py
+-rw-r--r--   0 root         (0) root         (0)    29645 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/transform/transform.py
+-rw-r--r--   0 root         (0) root         (0)     5860 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/transform/transform_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4391 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/transform/transform_tensor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:25:49.872888 deeplake-3.6.0/deeplake/core/vectorstore/
+-rw-r--r--   0 root         (0) root         (0)      611 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/vectorstore/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24036 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/vectorstore/deeplake_vectorstore.py
+-rw-r--r--   0 root         (0) root         (0)    29778 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/vectorstore/test_deeplake_vectorstore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:25:49.872888 deeplake-3.6.0/deeplake/core/vectorstore/vector_search/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/vectorstore/vector_search/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:25:49.872888 deeplake-3.6.0/deeplake/core/vectorstore/vector_search/dataset/
+-rw-r--r--   0 root         (0) root         (0)      330 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/vectorstore/vector_search/dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11363 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/vectorstore/vector_search/dataset/dataset.py
+-rw-r--r--   0 root         (0) root         (0)    10090 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:25:49.872888 deeplake-3.6.0/deeplake/core/vectorstore/vector_search/filter/
+-rw-r--r--   0 root         (0) root         (0)      286 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/vectorstore/vector_search/filter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3212 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/vectorstore/vector_search/filter/filter.py
+-rw-r--r--   0 root         (0) root         (0)     3542 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/vectorstore/vector_search/filter/test_filter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:25:49.872888 deeplake-3.6.0/deeplake/core/vectorstore/vector_search/indra/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/vectorstore/vector_search/indra/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4510 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/vectorstore/vector_search/indra/query.py
+-rw-r--r--   0 root         (0) root         (0)     2562 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/vectorstore/vector_search/indra/search_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     1795 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/vectorstore/vector_search/indra/test_indra.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:25:49.872888 deeplake-3.6.0/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/
+-rw-r--r--   0 root         (0) root         (0)      275 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      781 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py
+-rw-r--r--   0 root         (0) root         (0)      186 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/order.py
+-rw-r--r--   0 root         (0) root         (0)     1512 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/vectorstore/vector_search/indra/vector_search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:25:49.872888 deeplake-3.6.0/deeplake/core/vectorstore/vector_search/ingestion/
+-rw-r--r--   0 root         (0) root         (0)       93 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/vectorstore/vector_search/ingestion/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6455 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py
+-rw-r--r--   0 root         (0) root         (0)     2022 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py
+-rw-r--r--   0 root         (0) root         (0)     5014 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:25:49.872888 deeplake-3.6.0/deeplake/core/vectorstore/vector_search/python/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/vectorstore/vector_search/python/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1924 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/vectorstore/vector_search/python/search_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     1886 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/vectorstore/vector_search/python/test_vector_search.py
+-rw-r--r--   0 root         (0) root         (0)     1557 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/vectorstore/vector_search/python/vector_search.py
+-rw-r--r--   0 root         (0) root         (0)     8966 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/vectorstore/vector_search/utils.py
+-rw-r--r--   0 root         (0) root         (0)     2667 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/vectorstore/vector_search/vector_search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:25:49.872888 deeplake-3.6.0/deeplake/core/version_control/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/version_control/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1954 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/version_control/commit_chunk_map.py
+-rw-r--r--   0 root         (0) root         (0)     6337 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/version_control/commit_diff.py
+-rw-r--r--   0 root         (0) root         (0)     3109 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/version_control/commit_node.py
+-rw-r--r--   0 root         (0) root         (0)     4828 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/version_control/dataset_diff.py
+-rw-r--r--   0 root         (0) root         (0)    19869 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/version_control/test_merge.py
+-rw-r--r--   0 root         (0) root         (0)    84800 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/core/version_control/test_version_control.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:25:49.872888 deeplake-3.6.0/deeplake/enterprise/
+-rw-r--r--   0 root         (0) root         (0)      257 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/enterprise/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7381 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/enterprise/convert_to_libdeeplake.py
+-rw-r--r--   0 root         (0) root         (0)    29584 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/enterprise/dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     6010 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/enterprise/dummy_dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     4391 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/enterprise/libdeeplake_query.py
+-rw-r--r--   0 root         (0) root         (0)    25897 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/enterprise/test_pytorch.py
+-rw-r--r--   0 root         (0) root         (0)     1622 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/enterprise/test_query.py
+-rw-r--r--   0 root         (0) root         (0)    22353 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/enterprise/test_tensorflow.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/enterprise/util.py
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/hooks.py
+-rw-r--r--   0 root         (0) root         (0)     5050 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/htype.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:25:49.872888 deeplake-3.6.0/deeplake/integrations/
+-rw-r--r--   0 root         (0) root         (0)       99 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/integrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:25:49.872888 deeplake-3.6.0/deeplake/integrations/huggingface/
+-rw-r--r--   0 root         (0) root         (0)       44 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/integrations/huggingface/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5503 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/integrations/huggingface/huggingface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:25:49.872888 deeplake-3.6.0/deeplake/integrations/mmdet/
+-rw-r--r--   0 root         (0) root         (0)      118 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/integrations/mmdet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62754 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/integrations/mmdet/mmdet_.py
+-rw-r--r--   0 root         (0) root         (0)     4739 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/integrations/mmdet/mmdet_runners.py
+-rw-r--r--   0 root         (0) root         (0)    19660 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/integrations/mmdet/mmdet_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:25:49.872888 deeplake-3.6.0/deeplake/integrations/pytorch/
+-rw-r--r--   0 root         (0) root         (0)       40 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/integrations/pytorch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9772 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/integrations/pytorch/common.py
+-rw-r--r--   0 root         (0) root         (0)     7140 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/integrations/pytorch/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4245 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/integrations/pytorch/pytorch.py
+-rw-r--r--   0 root         (0) root         (0)     6919 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/integrations/pytorch/shuffle_buffer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:25:49.872888 deeplake-3.6.0/deeplake/integrations/tf/
+-rw-r--r--   0 root         (0) root         (0)      135 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/integrations/tf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1270 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/integrations/tf/common.py
+-rw-r--r--   0 root         (0) root         (0)     2453 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/integrations/tf/datasettotensorflow.py
+-rw-r--r--   0 root         (0) root         (0)     5330 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/integrations/tf/deeplake_tensorflow_dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:25:49.872888 deeplake-3.6.0/deeplake/integrations/wandb/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/integrations/wandb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12089 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/integrations/wandb/wandb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:25:49.872888 deeplake-3.6.0/deeplake/requirements/
+-rw-r--r--   0 root         (0) root         (0)      476 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/requirements/common.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/requirements/docs.txt
+-rw-r--r--   0 root         (0) root         (0)      381 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/requirements/plugins.txt
+-rw-r--r--   0 root         (0) root         (0)      304 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/requirements/tests.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:25:49.872888 deeplake-3.6.0/deeplake/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1404 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/tests/cache_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     2559 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/tests/client_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     4266 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/tests/common.py
+-rw-r--r--   0 root         (0) root         (0)     4018 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/tests/dataset_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)    16165 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/tests/path_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     2735 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/tests/storage_fixtures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:25:49.882888 deeplake-3.6.0/deeplake/util/
+-rw-r--r--   0 root         (0) root         (0)       86 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3531 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/access_method.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/agreement.py
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/array_list.py
+-rw-r--r--   0 root         (0) root         (0)      619 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/assert_byte_indexes.py
+-rw-r--r--   0 root         (0) root         (0)     2961 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/auto.py
+-rw-r--r--   0 root         (0) root         (0)     5740 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/bugout_reporter.py
+-rw-r--r--   0 root         (0) root         (0)       54 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/bugout_token.py
+-rw-r--r--   0 root         (0) root         (0)     3623 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/cache_chain.py
+-rw-r--r--   0 root         (0) root         (0)     4494 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/casting.py
+-rw-r--r--   0 root         (0) root         (0)      310 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/check_installation.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/check_latest_version.py
+-rw-r--r--   0 root         (0) root         (0)     3172 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/chunk_engine.py
+-rw-r--r--   0 root         (0) root         (0)     4597 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/class_label.py
+-rw-r--r--   0 root         (0) root         (0)      231 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/compression.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/compute.py
+-rw-r--r--   0 root         (0) root         (0)     5404 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/connect_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/dataset.py
+-rw-r--r--   0 root         (0) root         (0)      443 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/delete_entry.py
+-rw-r--r--   0 root         (0) root         (0)    15912 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/diff.py
+-rw-r--r--   0 root         (0) root         (0)     4945 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/downsample.py
+-rw-r--r--   0 root         (0) root         (0)       84 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/empty_sample.py
+-rw-r--r--   0 root         (0) root         (0)    15682 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/encoder.py
+-rw-r--r--   0 root         (0) root         (0)    34711 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2026 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/exif.py
+-rw-r--r--   0 root         (0) root         (0)     1819 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/from_tfds.py
+-rw-r--r--   0 root         (0) root         (0)      136 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/generate_id.py
+-rw-r--r--   0 root         (0) root         (0)      306 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/hash.py
+-rw-r--r--   0 root         (0) root         (0)     2799 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/htype.py
+-rw-r--r--   0 root         (0) root         (0)     1517 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/image.py
+-rw-r--r--   0 root         (0) root         (0)      873 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/invalid_view_op.py
+-rw-r--r--   0 root         (0) root         (0)      135 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/iterable_ordered_dict.py
+-rw-r--r--   0 root         (0) root         (0)     1001 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/iteration_warning.py
+-rw-r--r--   0 root         (0) root         (0)      507 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/join_chunks.py
+-rw-r--r--   0 root         (0) root         (0)     6422 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/json.py
+-rw-r--r--   0 root         (0) root         (0)     7261 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/keys.py
+-rw-r--r--   0 root         (0) root         (0)     2996 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/link.py
+-rw-r--r--   0 root         (0) root         (0)     1646 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/logging.py
+-rw-r--r--   0 root         (0) root         (0)    37497 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/merge.py
+-rw-r--r--   0 root         (0) root         (0)     2426 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/modified.py
+-rw-r--r--   0 root         (0) root         (0)      903 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/notebook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:25:49.882888 deeplake-3.6.0/deeplake/util/object_3d/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/object_3d/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3374 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/object_3d/mesh.py
+-rw-r--r--   0 root         (0) root         (0)      185 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/object_3d/mesh_parser.py
+-rw-r--r--   0 root         (0) root         (0)      185 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/object_3d/mesh_reader.py
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/object_3d/object_base_3d.py
+-rw-r--r--   0 root         (0) root         (0)      695 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/object_3d/ply_parser.py
+-rw-r--r--   0 root         (0) root         (0)     1323 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/object_3d/ply_parser_base.py
+-rw-r--r--   0 root         (0) root         (0)     6188 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/object_3d/ply_parsers.py
+-rw-r--r--   0 root         (0) root         (0)     1663 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/object_3d/ply_reader.py
+-rw-r--r--   0 root         (0) root         (0)     3221 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/object_3d/ply_reader_base.py
+-rw-r--r--   0 root         (0) root         (0)    10213 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/object_3d/ply_readers.py
+-rw-r--r--   0 root         (0) root         (0)     7187 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/object_3d/point_cloud.py
+-rw-r--r--   0 root         (0) root         (0)     1160 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/object_3d/read_3d_data.py
+-rw-r--r--   0 root         (0) root         (0)     3986 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/path.py
+-rw-r--r--   0 root         (0) root         (0)     3337 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/pretty_print.py
+-rw-r--r--   0 root         (0) root         (0)     2763 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/remove_cache.py
+-rw-r--r--   0 root         (0) root         (0)     4127 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/scheduling.py
+-rw-r--r--   0 root         (0) root         (0)     2892 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/shape_interval.py
+-rw-r--r--   0 root         (0) root         (0)      182 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/shuffle.py
+-rw-r--r--   0 root         (0) root         (0)     4204 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/spinner.py
+-rw-r--r--   0 root         (0) root         (0)     1153 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/split.py
+-rw-r--r--   0 root         (0) root         (0)     8435 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/storage.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/tag.py
+-rw-r--r--   0 root         (0) root         (0)     1390 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/tensor_db.py
+-rw-r--r--   0 root         (0) root         (0)      951 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:25:49.882888 deeplake-3.6.0/deeplake/util/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1476 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/tests/test_auto.py
+-rw-r--r--   0 root         (0) root         (0)     1757 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/tests/test_connect_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1239 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/tests/test_iterable_ordered_dict.py
+-rw-r--r--   0 root         (0) root         (0)      892 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/tests/test_read.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/tests/test_shape_interval.py
+-rw-r--r--   0 root         (0) root         (0)      407 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/tests/test_shuffle.py
+-rw-r--r--   0 root         (0) root         (0)      698 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/tests/test_split.py
+-rw-r--r--   0 root         (0) root         (0)      974 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/tests/test_tensor_db.py
+-rw-r--r--   0 root         (0) root         (0)      266 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/tests/test_token.py
+-rw-r--r--   0 root         (0) root         (0)     2428 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/tests/test_version_control.py
+-rw-r--r--   0 root         (0) root         (0)      276 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/threading.py
+-rw-r--r--   0 root         (0) root         (0)      381 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/token.py
+-rw-r--r--   0 root         (0) root         (0)    25235 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/transform.py
+-rw-r--r--   0 root         (0) root         (0)    31615 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/version_control.py
+-rw-r--r--   0 root         (0) root         (0)      927 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/video.py
+-rw-r--r--   0 root         (0) root         (0)      167 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/util/warnings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:25:49.882888 deeplake-3.6.0/deeplake/visualizer/
+-rw-r--r--   0 root         (0) root         (0)       34 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/visualizer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6466 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/visualizer/video_streaming.py
+-rw-r--r--   0 root         (0) root         (0)     6722 2023-06-07 09:24:16.000000 deeplake-3.6.0/deeplake/visualizer/visualizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 09:25:49.852888 deeplake-3.6.0/deeplake.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    26080 2023-06-07 09:25:49.000000 deeplake-3.6.0/deeplake.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12677 2023-06-07 09:25:49.000000 deeplake-3.6.0/deeplake.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 09:25:49.000000 deeplake-3.6.0/deeplake.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       58 2023-06-07 09:25:49.000000 deeplake-3.6.0/deeplake.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 09:25:49.000000 deeplake-3.6.0/deeplake.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-06-07 09:25:49.000000 deeplake-3.6.0/deeplake.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-07 09:25:49.000000 deeplake-3.6.0/deeplake.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      311 2023-06-07 09:25:49.882888 deeplake-3.6.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3357 2023-06-07 09:24:16.000000 deeplake-3.6.0/setup.py
```

### Comparing `deeplake-3.5.4/LICENSE` & `deeplake-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/PKG-INFO` & `deeplake-3.6.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: deeplake
-Version: 3.5.4
+Version: 3.6.0
 Summary: Activeloop Deep Lake
 Home-page: UNKNOWN
 Author: activeloop.ai
 Author-email: support@activeloop.ai
 License: MPL-2.0
 Project-URL: Documentation, https://docs.activeloop.ai/
 Project-URL: Source, https://github.com/activeloopai/deeplake
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: audio
 Provides-Extra: av
+Provides-Extra: azure
 Provides-Extra: dicom
 Provides-Extra: enterprise
 Provides-Extra: gcp
 Provides-Extra: gdrive
 Provides-Extra: medical
 Provides-Extra: point_cloud
 Provides-Extra: video
 Provides-Extra: visualizer
 License-File: LICENSE
 
 <img src="https://static.scarf.sh/a.png?x-pxid=bc3c57b0-9a65-49fe-b8ea-f711c4d35b82" /><p align="center">
      <img src="https://i.postimg.cc/rsjcWc3S/deeplake-logo.png" width="400"/>
 </h1>
     </br>
-    <h1 align="center">Deep Lake: Vector Database for any AI data
+    <h1 align="center">Deep Lake: Database for AI
  </h1>
 <p align="center">
     <a href="https://github.com/activeloopai/Hub/actions/workflows/test-pr-on-label.yml"><img src="https://github.com/activeloopai/Hub/actions/workflows/test-push.yml/badge.svg" alt="PyPI version" height="18"></a>
     <a href="https://pypi.org/project/deeplake/"><img src="https://badge.fury.io/py/deeplake.svg" alt="PyPI version" height="18"></a>
     <a href='https://docs.deeplake.ai/en/latest/?badge=latest'>
      <img src='https://readthedocs.org/projects/deep-lake/badge/?version=latest' alt='Documentation Status' />
      </a>
@@ -52,15 +53,15 @@
  </h3>
  
 
 *Read this in other languages: [简体中文](README.zh-cn.md)*
 
 ## About Deep Lake
 
-Deep Lake is a Vector Database powered by a unique storage format optimized for deep-learning and Large Language Model (LLM) based applications. It simplifies the deployment of enterprise-grade LLM-based products by offering storage for all data types (embeddings, audio, text, videos, images, pdfs, annotations, etc.), querying and vector search, data streaming while training models at scale, data versioning and lineage for all workloads, and integrations with popular tools such as LangChain, LlamaIndex, Weights and Biases, and many more. Deep Lake works with data of any size, it is serverless, and it enables you to store all of your data in once place. Deep Lake is used by Google, Intel, Airbus, Matterport, Red Cross, Yale, & Oxford. 
+Deep Lake is a Database for AI powered by a unique storage format optimized for deep-learning and Large Language Model (LLM) based applications. It simplifies the deployment of enterprise-grade LLM-based products by offering storage for all data types (embeddings, audio, text, videos, images, pdfs, annotations, etc.), querying and vector search, data streaming while training models at scale, data versioning and lineage for all workloads, and integrations with popular tools such as LangChain, LlamaIndex, Weights & Biases, and many more. Deep Lake works with data of any size, it is serverless, and it enables you to store all of your data in once place. Deep Lake is used by Intel, Airbus, Matterport, ZERO Systems, Red Cross, Yale, & Oxford. 
 
 Deep Lake includes the following features:
 
 <details>
   <summary><b>Storage Agnostic API</b></summary>
 Use one API to upload, download, and stream datasets to/from AWS S3/S3-compatible storage, GCP, Activeloop cloud, or local storage.
 </details>
@@ -292,22 +293,15 @@
 * **LLM Apps**
   * Use [Deep Lake as a vector store for LLM apps](https://www.activeloop.ai/resources/ultimate-guide-to-lang-chain-deep-lake-build-chat-gpt-to-answer-questions-on-your-financial-data/). Our integration combines the [Langchain](https://github.com/hwchase17/langchain) [VectorStores API](https://python.langchain.com/en/latest/reference/modules/vectorstore.html?highlight=pinecone#langchain.vectorstores.DeepLake) with Deep Lake datasets as the underlying data storage. The integration is a serverless vector store that can be deployed locally or in a cloud of your choice. 
 
 ## 📚 Documentation
 Getting started guides, examples, tutorials, API reference, and other useful information can be found on our [documentation page](http://docs.activeloop.ai/?utm_source=github&utm_medium=repo&utm_campaign=readme). 
 
 ## 🎓 For Students and Educators
-Deep Lake users can access and visualize a variety of popular datasets through a free integration with Activeloop's Platform. Users can also create and store their own datasets and make them available to the public. Free storage of up to 300 GB is available for students and educators:
-
-| <!-- -->    | <!-- -->    |
-| ---------------------------------------------------- | ------------- |
-| Storage for public datasets hosted by Activeloop     | 200GB Free    |
-| Storage for private datasets hosted by Activeloop    | 100GB Free    |
-
-
+Deep Lake users can access and visualize a variety of popular datasets through a free integration with Activeloop's Platform. Universities can get up to 1TB of data storage and 100,000 monthly queries on the Tensor Database for free per month. Chat in on [our website](https://activeloop.ai): to claim the access!
 
 ## 👩‍💻 Comparisons to Familiar Tools
 
 <details>
   <summary><b>Deep Lake vs Chroma </b></summary>
   
 Both Deep Lake & ChromaDB enable users to store and search vectors (embeddings) and offer integrations with LangChain and LlamaIndex. However, they are architecturally very different. ChromaDB is a Vector Database that can be deployed locally or on a server using Docker and will offer a hosted solution shortly. Deep Lake is a serverless Vector Store deployed on the user’s own cloud, locally, or in-memory. All computations run client-side, which enables users to support lightweight production apps in seconds. Unlike ChromaDB, Deep Lake’s data format can store raw data such as images, videos, and text, in addition to embeddings. ChromaDB is limited to light metadata on top of the embeddings and has no visualization. Deep Lake datasets can be visualized and version controlled. Deep Lake also has a performant dataloader for fine-tuning your Large Language Models. 
@@ -335,14 +329,25 @@
   
 Deep Lake and DVC offer dataset version control similar to git for data, but their methods for storing data differ significantly. Deep Lake converts and stores data as chunked compressed arrays, which enables rapid streaming to ML models, whereas DVC operates on top of data stored in less efficient traditional file structures. The Deep Lake format makes dataset versioning significantly easier compared to traditional file structures by DVC when datasets are composed of many files (i.e., many images). An additional distinction is that DVC primarily uses a command-line interface, whereas Deep Lake is a Python package. Lastly, Deep Lake offers an API to easily connect datasets to ML frameworks and other common ML tools and enables instant dataset visualization through [Activeloop's visualization tool](http://app.activeloop.ai/?utm_source=github&utm_medium=repo&utm_campaign=readme).
 
 </details>
 
 
 <details>
+  <summary><b>Deep Lake vs MosaicML MDS format </b></summary>
+  
+- **Data Storage Format:** Deep Lake operates on a columnar storage format, whereas MDS utilizes a row-wise storage approach. This fundamentally impacts how data is read, written, and organized in each system.
+- **Compression:** Deep Lake offers a more flexible compression scheme, allowing control over both chunk-level and sample-level compression for each column or tensor. This feature eliminates the need for additional compressions like zstd, which would otherwise demand more CPU cycles for decompressing on top of formats like jpeg.
+- **Shuffling:** MDS currently offers more advanced shuffling strategies.
+- **Version Control & Visualization Support:** A notable feature of Deep Lake is its native version control and in-browser data visualization, a feature not present for MosaicML data format. This can provide significant advantages in managing, understanding, and tracking different versions of the data.
+
+</details>
+
+
+<details>
   <summary><b>Deep Lake vs TensorFlow Datasets (TFDS)</b></summary>
   
 Deep Lake and TFDS seamlessly connect popular datasets to ML frameworks. Deep Lake datasets are compatible with both PyTorch and TensorFlow, whereas TFDS are only compatible with TensorFlow. A key difference between Deep Lake and TFDS is that Deep Lake datasets are designed for streaming from the cloud, whereas TFDS must be downloaded locally prior to use. As a result, with Deep Lake, one can import datasets directly from TensorFlow Datasets and stream them either to PyTorch or TensorFlow. In addition to providing access to popular publicly available datasets, Deep Lake also offers powerful tools for creating custom datasets, storing them on a variety of cloud storage providers, and collaborating with others via simple API. TFDS is primarily focused on giving the public easy access to commonly available datasets, and management of custom datasets is not the primary focus. A full comparison article can be found [here](https://www.activeloop.ai/resources/tensor-flow-tf-data-activeloop-hub-how-to-implement-your-tensor-flow-data-pipelines-with-hub/).
 
 </details>
```

#### html2text {}

```diff
@@ -1,45 +1,45 @@
-Metadata-Version: 2.1 Name: deeplake Version: 3.5.4 Summary: Activeloop Deep
+Metadata-Version: 2.1 Name: deeplake Version: 3.6.0 Summary: Activeloop Deep
 Lake Home-page: UNKNOWN Author: activeloop.ai Author-email:
 support@activeloop.ai License: MPL-2.0 Project-URL: Documentation, https://
 docs.activeloop.ai/ Project-URL: Source, https://github.com/activeloopai/
 deeplake Platform: UNKNOWN Classifier: License :: OSI Approved :: Mozilla
 Public License 2.0 (MPL 2.0) Description-Content-Type: text/markdown Provides-
-Extra: all Provides-Extra: audio Provides-Extra: av Provides-Extra: dicom
-Provides-Extra: enterprise Provides-Extra: gcp Provides-Extra: gdrive Provides-
-Extra: medical Provides-Extra: point_cloud Provides-Extra: video Provides-
-Extra: visualizer License-File: LICENSE [https://static.scarf.sh/a.png?x-
-pxid=bc3c57b0-9a65-49fe-b8ea-f711c4d35b82]
+Extra: all Provides-Extra: audio Provides-Extra: av Provides-Extra: azure
+Provides-Extra: dicom Provides-Extra: enterprise Provides-Extra: gcp Provides-
+Extra: gdrive Provides-Extra: medical Provides-Extra: point_cloud Provides-
+Extra: video Provides-Extra: visualizer License-File: LICENSE [https://
+static.scarf.sh/a.png?x-pxid=bc3c57b0-9a65-49fe-b8ea-f711c4d35b82]
                [https://i.postimg.cc/rsjcWc3S/deeplake-logo.png]
-           ****** Deep Lake: Vector Database for any AI data ******
+                   ****** Deep Lake: Database for AI ******
   [PyPI_version] [PyPI_version] [Documentation_Status] [PyPI_version] [GitHub
                                issues] [codecov]
    **** Documentation • Getting_Started • API_Reference • Examples • Blog •
                   Whitepaper • Slack_Community • Twitter ****
 *Read this in other languages: [ç®ä½ä¸­æ](README.zh-cn.md)* ## About Deep
-Lake Deep Lake is a Vector Database powered by a unique storage format
+Lake Deep Lake is a Database for AI powered by a unique storage format
 optimized for deep-learning and Large Language Model (LLM) based applications.
 It simplifies the deployment of enterprise-grade LLM-based products by offering
 storage for all data types (embeddings, audio, text, videos, images, pdfs,
 annotations, etc.), querying and vector search, data streaming while training
 models at scale, data versioning and lineage for all workloads, and
-integrations with popular tools such as LangChain, LlamaIndex, Weights and
+integrations with popular tools such as LangChain, LlamaIndex, Weights &
 Biases, and many more. Deep Lake works with data of any size, it is serverless,
 and it enables you to store all of your data in once place. Deep Lake is used
-by Google, Intel, Airbus, Matterport, Red Cross, Yale, & Oxford. Deep Lake
-includes the following features:  Storage Agnostic API Use one API to upload,
-download, and stream datasets to/from AWS S3/S3-compatible storage, GCP,
-Activeloop cloud, or local storage.   Native Compression with Lazy NumPy-like
-Indexing Store images, audios and videos in their native compression. Slide,
-index, iterate and interact with your data like a collection of NumPy arrays in
-your system's memory. Deep Lake lazily loads data only when needed, e.g., when
-training a model.   Dataset Version Control Commits, branches, checkout -
-Concepts you are already familiar with in your code repositories can now be
-applied to your datasets as well!   Dataloaders for Popular Deep Learning
-Frameworks Deep Lake comes with built-in dataloaders for Pytorch and
+by Intel, Airbus, Matterport, ZERO Systems, Red Cross, Yale, & Oxford. Deep
+Lake includes the following features:  Storage Agnostic API Use one API to
+upload, download, and stream datasets to/from AWS S3/S3-compatible storage,
+GCP, Activeloop cloud, or local storage.   Native Compression with Lazy NumPy-
+like Indexing Store images, audios and videos in their native compression.
+Slide, index, iterate and interact with your data like a collection of NumPy
+arrays in your system's memory. Deep Lake lazily loads data only when needed,
+e.g., when training a model.   Dataset Version Control Commits, branches,
+checkout - Concepts you are already familiar with in your code repositories can
+now be applied to your datasets as well!   Dataloaders for Popular Deep
+Learning Frameworks Deep Lake comes with built-in dataloaders for Pytorch and
 Tensorflow. Train your model with a few lines of code - we even take care of
 dataset shuffling. :)   Integrations with Powerful Tools Deep Lake has
 integrations with Langchain and LLamaIndex as a vector store for LLM apps,
 Weights_&_Biases for data lineage during model training, and MMDetection for
 training object detection models.   Distributed Transformations Rapidly apply
 transformations on your datasets using multi-threading, multi-processing, or
 our built-in Ray integration.  100+ most-popular image, video, and audio
@@ -138,97 +138,107 @@
 Lake datasets as the underlying data storage. The integration is a serverless
 vector store that can be deployed locally or in a cloud of your choice. ## ð
 Documentation Getting started guides, examples, tutorials, API reference, and
 other useful information can be found on our [documentation page](http://
 docs.activeloop.ai/?utm_source=github&utm_medium=repo&utm_campaign=readme). ##
 ð For Students and Educators Deep Lake users can access and visualize a
 variety of popular datasets through a free integration with Activeloop's
-Platform. Users can also create and store their own datasets and make them
-available to the public. Free storage of up to 300 GB is available for students
-and educators: |  |  | | ---------------------------------------------------- |
-------------- | | Storage for public datasets hosted by Activeloop | 200GB Free
-| | Storage for private datasets hosted by Activeloop | 100GB Free | ##
-ð©âð» Comparisons to Familiar Tools  Deep Lake vs Chroma Both Deep Lake &
-ChromaDB enable users to store and search vectors (embeddings) and offer
-integrations with LangChain and LlamaIndex. However, they are architecturally
-very different. ChromaDB is a Vector Database that can be deployed locally or
-on a server using Docker and will offer a hosted solution shortly. Deep Lake is
-a serverless Vector Store deployed on the userâs own cloud, locally, or in-
-memory. All computations run client-side, which enables users to support
-lightweight production apps in seconds. Unlike ChromaDB, Deep Lakeâs data
-format can store raw data such as images, videos, and text, in addition to
-embeddings. ChromaDB is limited to light metadata on top of the embeddings and
-has no visualization. Deep Lake datasets can be visualized and version
-controlled. Deep Lake also has a performant dataloader for fine-tuning your
-Large Language Models.   Deep Lake vs Pinecone Both Deep Lake and Pinecone
-enable users to store and search vectors (embeddings) and offer integrations
-with LangChain and LlamaIndex. However, they are architecturally very
-different. Pinecone is a fully-managed Vector Database that is optimized for
-highly demanding applications requiring search for billions of vectors. Deep
-Lake is a serverless. All computations run client-side, which enables users to
-get started in seconds. Unlike Pinecone, Deep Lakeâs data format can store
-raw data such as images, videos, and text, in addition to embeddings. Deep Lake
-datasets can be visualized and version controlled. Pinecone is limited to light
-metadata on top of the embeddings and has no visualization. Deep Lake also has
-a performant dataloader for fine-tuning your Large Language Models.   Deep Lake
-vs Weaviate Both Deep Lake and Weaviate enable users to store and search
+Platform. Universities can get up to 1TB of data storage and 100,000 monthly
+queries on the Tensor Database for free per month. Chat in on [our website]
+(https://activeloop.ai): to claim the access! ## ð©âð» Comparisons to
+Familiar Tools  Deep Lake vs Chroma Both Deep Lake & ChromaDB enable users to
+store and search vectors (embeddings) and offer integrations with LangChain and
+LlamaIndex. However, they are architecturally very different. ChromaDB is a
+Vector Database that can be deployed locally or on a server using Docker and
+will offer a hosted solution shortly. Deep Lake is a serverless Vector Store
+deployed on the userâs own cloud, locally, or in-memory. All computations run
+client-side, which enables users to support lightweight production apps in
+seconds. Unlike ChromaDB, Deep Lakeâs data format can store raw data such as
+images, videos, and text, in addition to embeddings. ChromaDB is limited to
+light metadata on top of the embeddings and has no visualization. Deep Lake
+datasets can be visualized and version controlled. Deep Lake also has a
+performant dataloader for fine-tuning your Large Language Models.   Deep Lake
+vs Pinecone Both Deep Lake and Pinecone enable users to store and search
 vectors (embeddings) and offer integrations with LangChain and LlamaIndex.
-However, they are architecturally very different. Weaviate is a Vector Database
-that can be deployed in a managed service or by the user via Kubernetes or
-Docker. Deep Lake is serverless. All computations run client-side, which
-enables users to support lightweight production apps in seconds. Unlike
-Weaviate, Deep Lakeâs data format can store raw data such as images, videos,
-and text, in addition to embeddings. Deep Lake datasets can be visualized and
-version controlled. Weaviate is limited to light metadata on top of the
-embeddings and has no visualization. Deep Lake also has a performant dataloader
-for fine-tuning your Large Language Models.   Deep Lake vs DVC Deep Lake and
-DVC offer dataset version control similar to git for data, but their methods
-for storing data differ significantly. Deep Lake converts and stores data as
-chunked compressed arrays, which enables rapid streaming to ML models, whereas
-DVC operates on top of data stored in less efficient traditional file
-structures. The Deep Lake format makes dataset versioning significantly easier
-compared to traditional file structures by DVC when datasets are composed of
-many files (i.e., many images). An additional distinction is that DVC primarily
-uses a command-line interface, whereas Deep Lake is a Python package. Lastly,
-Deep Lake offers an API to easily connect datasets to ML frameworks and other
-common ML tools and enables instant dataset visualization through [Activeloop's
-visualization tool](http://app.activeloop.ai/
-?utm_source=github&utm_medium=repo&utm_campaign=readme).   Deep Lake vs
-TensorFlow Datasets (TFDS) Deep Lake and TFDS seamlessly connect popular
-datasets to ML frameworks. Deep Lake datasets are compatible with both PyTorch
-and TensorFlow, whereas TFDS are only compatible with TensorFlow. A key
-difference between Deep Lake and TFDS is that Deep Lake datasets are designed
-for streaming from the cloud, whereas TFDS must be downloaded locally prior to
-use. As a result, with Deep Lake, one can import datasets directly from
-TensorFlow Datasets and stream them either to PyTorch or TensorFlow. In
-addition to providing access to popular publicly available datasets, Deep Lake
-also offers powerful tools for creating custom datasets, storing them on a
-variety of cloud storage providers, and collaborating with others via simple
-API. TFDS is primarily focused on giving the public easy access to commonly
-available datasets, and management of custom datasets is not the primary focus.
-A full comparison article can be found [here](https://www.activeloop.ai/
-resources/tensor-flow-tf-data-activeloop-hub-how-to-implement-your-tensor-flow-
-data-pipelines-with-hub/).   Deep Lake vs HuggingFace Deep Lake and HuggingFace
-offer access to popular datasets, but Deep Lake primarily focuses on computer
-vision, whereas HuggingFace focuses on natural language processing. HuggingFace
-Transforms and other computational tools for NLP are not analogous to features
-offered by Deep Lake.   Deep Lake vs WebDatasets Deep Lake and WebDatasets both
-offer rapid data streaming across networks. They have nearly identical steaming
-speeds because the underlying network requests and data structures are very
-similar. However, Deep Lake offers superior random access and shuffling, its
-simple API is in python instead of command-line, and Deep Lake enables simple
-indexing and modification of the dataset without having to recreate it.   Deep
-Lake vs Zarr Deep Lake and Zarr both offer storage of data as chunked arrays.
-However, Deep Lake is primarily designed for returning data as arrays using a
-simple API, rather than actually storing raw arrays (even though that's also
-possible). Deep Lake stores data in use-case-optimized formats, such as jpeg or
-png for images, or mp4 for video, and the user treats the data as if it's an
-array, because Deep Lake handles all the data processing in between. Deep Lake
-offers more flexibility for storing arrays with dynamic shape (ragged tensors),
-and it provides several features that are not naively available in Zarr such as
+However, they are architecturally very different. Pinecone is a fully-managed
+Vector Database that is optimized for highly demanding applications requiring
+search for billions of vectors. Deep Lake is a serverless. All computations run
+client-side, which enables users to get started in seconds. Unlike Pinecone,
+Deep Lakeâs data format can store raw data such as images, videos, and text,
+in addition to embeddings. Deep Lake datasets can be visualized and version
+controlled. Pinecone is limited to light metadata on top of the embeddings and
+has no visualization. Deep Lake also has a performant dataloader for fine-
+tuning your Large Language Models.   Deep Lake vs Weaviate Both Deep Lake and
+Weaviate enable users to store and search vectors (embeddings) and offer
+integrations with LangChain and LlamaIndex. However, they are architecturally
+very different. Weaviate is a Vector Database that can be deployed in a managed
+service or by the user via Kubernetes or Docker. Deep Lake is serverless. All
+computations run client-side, which enables users to support lightweight
+production apps in seconds. Unlike Weaviate, Deep Lakeâs data format can
+store raw data such as images, videos, and text, in addition to embeddings.
+Deep Lake datasets can be visualized and version controlled. Weaviate is
+limited to light metadata on top of the embeddings and has no visualization.
+Deep Lake also has a performant dataloader for fine-tuning your Large Language
+Models.   Deep Lake vs DVC Deep Lake and DVC offer dataset version control
+similar to git for data, but their methods for storing data differ
+significantly. Deep Lake converts and stores data as chunked compressed arrays,
+which enables rapid streaming to ML models, whereas DVC operates on top of data
+stored in less efficient traditional file structures. The Deep Lake format
+makes dataset versioning significantly easier compared to traditional file
+structures by DVC when datasets are composed of many files (i.e., many images).
+An additional distinction is that DVC primarily uses a command-line interface,
+whereas Deep Lake is a Python package. Lastly, Deep Lake offers an API to
+easily connect datasets to ML frameworks and other common ML tools and enables
+instant dataset visualization through [Activeloop's visualization tool](http://
+app.activeloop.ai/?utm_source=github&utm_medium=repo&utm_campaign=readme).
+Deep Lake vs MosaicML MDS format - **Data Storage Format:** Deep Lake operates
+on a columnar storage format, whereas MDS utilizes a row-wise storage approach.
+This fundamentally impacts how data is read, written, and organized in each
+system. - **Compression:** Deep Lake offers a more flexible compression scheme,
+allowing control over both chunk-level and sample-level compression for each
+column or tensor. This feature eliminates the need for additional compressions
+like zstd, which would otherwise demand more CPU cycles for decompressing on
+top of formats like jpeg. - **Shuffling:** MDS currently offers more advanced
+shuffling strategies. - **Version Control & Visualization Support:** A notable
+feature of Deep Lake is its native version control and in-browser data
+visualization, a feature not present for MosaicML data format. This can provide
+significant advantages in managing, understanding, and tracking different
+versions of the data.   Deep Lake vs TensorFlow Datasets (TFDS) Deep Lake and
+TFDS seamlessly connect popular datasets to ML frameworks. Deep Lake datasets
+are compatible with both PyTorch and TensorFlow, whereas TFDS are only
+compatible with TensorFlow. A key difference between Deep Lake and TFDS is that
+Deep Lake datasets are designed for streaming from the cloud, whereas TFDS must
+be downloaded locally prior to use. As a result, with Deep Lake, one can import
+datasets directly from TensorFlow Datasets and stream them either to PyTorch or
+TensorFlow. In addition to providing access to popular publicly available
+datasets, Deep Lake also offers powerful tools for creating custom datasets,
+storing them on a variety of cloud storage providers, and collaborating with
+others via simple API. TFDS is primarily focused on giving the public easy
+access to commonly available datasets, and management of custom datasets is not
+the primary focus. A full comparison article can be found [here](https://
+www.activeloop.ai/resources/tensor-flow-tf-data-activeloop-hub-how-to-
+implement-your-tensor-flow-data-pipelines-with-hub/).   Deep Lake vs
+HuggingFace Deep Lake and HuggingFace offer access to popular datasets, but
+Deep Lake primarily focuses on computer vision, whereas HuggingFace focuses on
+natural language processing. HuggingFace Transforms and other computational
+tools for NLP are not analogous to features offered by Deep Lake.   Deep Lake
+vs WebDatasets Deep Lake and WebDatasets both offer rapid data streaming across
+networks. They have nearly identical steaming speeds because the underlying
+network requests and data structures are very similar. However, Deep Lake
+offers superior random access and shuffling, its simple API is in python
+instead of command-line, and Deep Lake enables simple indexing and modification
+of the dataset without having to recreate it.   Deep Lake vs Zarr Deep Lake and
+Zarr both offer storage of data as chunked arrays. However, Deep Lake is
+primarily designed for returning data as arrays using a simple API, rather than
+actually storing raw arrays (even though that's also possible). Deep Lake
+stores data in use-case-optimized formats, such as jpeg or png for images, or
+mp4 for video, and the user treats the data as if it's an array, because Deep
+Lake handles all the data processing in between. Deep Lake offers more
+flexibility for storing arrays with dynamic shape (ragged tensors), and it
+provides several features that are not naively available in Zarr such as
 version control, data streaming, and connecting data to ML Frameworks.  ##
 Community Join our [**Slack community**](https://join.slack.com/t/hubdb/
 shared_invite/zt-ivhsj8sz-GWv9c5FLBDVw8vn~sxRKqQ) to learn more about
 unstructured dataset management using Deep Lake and to get help from the
 Activeloop team and other users. We'd love your feedback by completing our 3-
 minute [**survey**](https://forms.gle/rLi4w33dow6CSMcm9). As always, thanks to
 our amazing contributors! [https://contrib.rocks/image?repo=activeloopai/hub]
```

### Comparing `deeplake-3.5.4/README.md` & `deeplake-3.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <img src="https://static.scarf.sh/a.png?x-pxid=bc3c57b0-9a65-49fe-b8ea-f711c4d35b82" /><p align="center">
      <img src="https://i.postimg.cc/rsjcWc3S/deeplake-logo.png" width="400"/>
 </h1>
     </br>
-    <h1 align="center">Deep Lake: Vector Database for any AI data
+    <h1 align="center">Deep Lake: Database for AI
  </h1>
 <p align="center">
     <a href="https://github.com/activeloopai/Hub/actions/workflows/test-pr-on-label.yml"><img src="https://github.com/activeloopai/Hub/actions/workflows/test-push.yml/badge.svg" alt="PyPI version" height="18"></a>
     <a href="https://pypi.org/project/deeplake/"><img src="https://badge.fury.io/py/deeplake.svg" alt="PyPI version" height="18"></a>
     <a href='https://docs.deeplake.ai/en/latest/?badge=latest'>
      <img src='https://readthedocs.org/projects/deep-lake/badge/?version=latest' alt='Documentation Status' />
      </a>
@@ -26,15 +26,15 @@
  </h3>
  
 
 *Read this in other languages: [简体中文](README.zh-cn.md)*
 
 ## About Deep Lake
 
-Deep Lake is a Vector Database powered by a unique storage format optimized for deep-learning and Large Language Model (LLM) based applications. It simplifies the deployment of enterprise-grade LLM-based products by offering storage for all data types (embeddings, audio, text, videos, images, pdfs, annotations, etc.), querying and vector search, data streaming while training models at scale, data versioning and lineage for all workloads, and integrations with popular tools such as LangChain, LlamaIndex, Weights and Biases, and many more. Deep Lake works with data of any size, it is serverless, and it enables you to store all of your data in once place. Deep Lake is used by Google, Intel, Airbus, Matterport, Red Cross, Yale, & Oxford. 
+Deep Lake is a Database for AI powered by a unique storage format optimized for deep-learning and Large Language Model (LLM) based applications. It simplifies the deployment of enterprise-grade LLM-based products by offering storage for all data types (embeddings, audio, text, videos, images, pdfs, annotations, etc.), querying and vector search, data streaming while training models at scale, data versioning and lineage for all workloads, and integrations with popular tools such as LangChain, LlamaIndex, Weights & Biases, and many more. Deep Lake works with data of any size, it is serverless, and it enables you to store all of your data in once place. Deep Lake is used by Intel, Airbus, Matterport, ZERO Systems, Red Cross, Yale, & Oxford. 
 
 Deep Lake includes the following features:
 
 <details>
   <summary><b>Storage Agnostic API</b></summary>
 Use one API to upload, download, and stream datasets to/from AWS S3/S3-compatible storage, GCP, Activeloop cloud, or local storage.
 </details>
@@ -266,22 +266,15 @@
 * **LLM Apps**
   * Use [Deep Lake as a vector store for LLM apps](https://www.activeloop.ai/resources/ultimate-guide-to-lang-chain-deep-lake-build-chat-gpt-to-answer-questions-on-your-financial-data/). Our integration combines the [Langchain](https://github.com/hwchase17/langchain) [VectorStores API](https://python.langchain.com/en/latest/reference/modules/vectorstore.html?highlight=pinecone#langchain.vectorstores.DeepLake) with Deep Lake datasets as the underlying data storage. The integration is a serverless vector store that can be deployed locally or in a cloud of your choice. 
 
 ## 📚 Documentation
 Getting started guides, examples, tutorials, API reference, and other useful information can be found on our [documentation page](http://docs.activeloop.ai/?utm_source=github&utm_medium=repo&utm_campaign=readme). 
 
 ## 🎓 For Students and Educators
-Deep Lake users can access and visualize a variety of popular datasets through a free integration with Activeloop's Platform. Users can also create and store their own datasets and make them available to the public. Free storage of up to 300 GB is available for students and educators:
-
-| <!-- -->    | <!-- -->    |
-| ---------------------------------------------------- | ------------- |
-| Storage for public datasets hosted by Activeloop     | 200GB Free    |
-| Storage for private datasets hosted by Activeloop    | 100GB Free    |
-
-
+Deep Lake users can access and visualize a variety of popular datasets through a free integration with Activeloop's Platform. Universities can get up to 1TB of data storage and 100,000 monthly queries on the Tensor Database for free per month. Chat in on [our website](https://activeloop.ai): to claim the access!
 
 ## 👩‍💻 Comparisons to Familiar Tools
 
 <details>
   <summary><b>Deep Lake vs Chroma </b></summary>
   
 Both Deep Lake & ChromaDB enable users to store and search vectors (embeddings) and offer integrations with LangChain and LlamaIndex. However, they are architecturally very different. ChromaDB is a Vector Database that can be deployed locally or on a server using Docker and will offer a hosted solution shortly. Deep Lake is a serverless Vector Store deployed on the user’s own cloud, locally, or in-memory. All computations run client-side, which enables users to support lightweight production apps in seconds. Unlike ChromaDB, Deep Lake’s data format can store raw data such as images, videos, and text, in addition to embeddings. ChromaDB is limited to light metadata on top of the embeddings and has no visualization. Deep Lake datasets can be visualized and version controlled. Deep Lake also has a performant dataloader for fine-tuning your Large Language Models. 
@@ -309,14 +302,25 @@
   
 Deep Lake and DVC offer dataset version control similar to git for data, but their methods for storing data differ significantly. Deep Lake converts and stores data as chunked compressed arrays, which enables rapid streaming to ML models, whereas DVC operates on top of data stored in less efficient traditional file structures. The Deep Lake format makes dataset versioning significantly easier compared to traditional file structures by DVC when datasets are composed of many files (i.e., many images). An additional distinction is that DVC primarily uses a command-line interface, whereas Deep Lake is a Python package. Lastly, Deep Lake offers an API to easily connect datasets to ML frameworks and other common ML tools and enables instant dataset visualization through [Activeloop's visualization tool](http://app.activeloop.ai/?utm_source=github&utm_medium=repo&utm_campaign=readme).
 
 </details>
 
 
 <details>
+  <summary><b>Deep Lake vs MosaicML MDS format </b></summary>
+  
+- **Data Storage Format:** Deep Lake operates on a columnar storage format, whereas MDS utilizes a row-wise storage approach. This fundamentally impacts how data is read, written, and organized in each system.
+- **Compression:** Deep Lake offers a more flexible compression scheme, allowing control over both chunk-level and sample-level compression for each column or tensor. This feature eliminates the need for additional compressions like zstd, which would otherwise demand more CPU cycles for decompressing on top of formats like jpeg.
+- **Shuffling:** MDS currently offers more advanced shuffling strategies.
+- **Version Control & Visualization Support:** A notable feature of Deep Lake is its native version control and in-browser data visualization, a feature not present for MosaicML data format. This can provide significant advantages in managing, understanding, and tracking different versions of the data.
+
+</details>
+
+
+<details>
   <summary><b>Deep Lake vs TensorFlow Datasets (TFDS)</b></summary>
   
 Deep Lake and TFDS seamlessly connect popular datasets to ML frameworks. Deep Lake datasets are compatible with both PyTorch and TensorFlow, whereas TFDS are only compatible with TensorFlow. A key difference between Deep Lake and TFDS is that Deep Lake datasets are designed for streaming from the cloud, whereas TFDS must be downloaded locally prior to use. As a result, with Deep Lake, one can import datasets directly from TensorFlow Datasets and stream them either to PyTorch or TensorFlow. In addition to providing access to popular publicly available datasets, Deep Lake also offers powerful tools for creating custom datasets, storing them on a variety of cloud storage providers, and collaborating with others via simple API. TFDS is primarily focused on giving the public easy access to commonly available datasets, and management of custom datasets is not the primary focus. A full comparison article can be found [here](https://www.activeloop.ai/resources/tensor-flow-tf-data-activeloop-hub-how-to-implement-your-tensor-flow-data-pipelines-with-hub/).
 
 </details>
```

#### html2text {}

```diff
@@ -1,35 +1,35 @@
 [https://static.scarf.sh/a.png?x-pxid=bc3c57b0-9a65-49fe-b8ea-f711c4d35b82]
                [https://i.postimg.cc/rsjcWc3S/deeplake-logo.png]
-           ****** Deep Lake: Vector Database for any AI data ******
+                   ****** Deep Lake: Database for AI ******
   [PyPI_version] [PyPI_version] [Documentation_Status] [PyPI_version] [GitHub
                                issues] [codecov]
    **** Documentation • Getting_Started • API_Reference • Examples • Blog •
                   Whitepaper • Slack_Community • Twitter ****
 *Read this in other languages: [ç®ä½ä¸­æ](README.zh-cn.md)* ## About Deep
-Lake Deep Lake is a Vector Database powered by a unique storage format
+Lake Deep Lake is a Database for AI powered by a unique storage format
 optimized for deep-learning and Large Language Model (LLM) based applications.
 It simplifies the deployment of enterprise-grade LLM-based products by offering
 storage for all data types (embeddings, audio, text, videos, images, pdfs,
 annotations, etc.), querying and vector search, data streaming while training
 models at scale, data versioning and lineage for all workloads, and
-integrations with popular tools such as LangChain, LlamaIndex, Weights and
+integrations with popular tools such as LangChain, LlamaIndex, Weights &
 Biases, and many more. Deep Lake works with data of any size, it is serverless,
 and it enables you to store all of your data in once place. Deep Lake is used
-by Google, Intel, Airbus, Matterport, Red Cross, Yale, & Oxford. Deep Lake
-includes the following features:  Storage Agnostic API Use one API to upload,
-download, and stream datasets to/from AWS S3/S3-compatible storage, GCP,
-Activeloop cloud, or local storage.   Native Compression with Lazy NumPy-like
-Indexing Store images, audios and videos in their native compression. Slide,
-index, iterate and interact with your data like a collection of NumPy arrays in
-your system's memory. Deep Lake lazily loads data only when needed, e.g., when
-training a model.   Dataset Version Control Commits, branches, checkout -
-Concepts you are already familiar with in your code repositories can now be
-applied to your datasets as well!   Dataloaders for Popular Deep Learning
-Frameworks Deep Lake comes with built-in dataloaders for Pytorch and
+by Intel, Airbus, Matterport, ZERO Systems, Red Cross, Yale, & Oxford. Deep
+Lake includes the following features:  Storage Agnostic API Use one API to
+upload, download, and stream datasets to/from AWS S3/S3-compatible storage,
+GCP, Activeloop cloud, or local storage.   Native Compression with Lazy NumPy-
+like Indexing Store images, audios and videos in their native compression.
+Slide, index, iterate and interact with your data like a collection of NumPy
+arrays in your system's memory. Deep Lake lazily loads data only when needed,
+e.g., when training a model.   Dataset Version Control Commits, branches,
+checkout - Concepts you are already familiar with in your code repositories can
+now be applied to your datasets as well!   Dataloaders for Popular Deep
+Learning Frameworks Deep Lake comes with built-in dataloaders for Pytorch and
 Tensorflow. Train your model with a few lines of code - we even take care of
 dataset shuffling. :)   Integrations with Powerful Tools Deep Lake has
 integrations with Langchain and LLamaIndex as a vector store for LLM apps,
 Weights_&_Biases for data lineage during model training, and MMDetection for
 training object detection models.   Distributed Transformations Rapidly apply
 transformations on your datasets using multi-threading, multi-processing, or
 our built-in Ray integration.  100+ most-popular image, video, and audio
@@ -128,97 +128,107 @@
 Lake datasets as the underlying data storage. The integration is a serverless
 vector store that can be deployed locally or in a cloud of your choice. ## ð
 Documentation Getting started guides, examples, tutorials, API reference, and
 other useful information can be found on our [documentation page](http://
 docs.activeloop.ai/?utm_source=github&utm_medium=repo&utm_campaign=readme). ##
 ð For Students and Educators Deep Lake users can access and visualize a
 variety of popular datasets through a free integration with Activeloop's
-Platform. Users can also create and store their own datasets and make them
-available to the public. Free storage of up to 300 GB is available for students
-and educators: |  |  | | ---------------------------------------------------- |
-------------- | | Storage for public datasets hosted by Activeloop | 200GB Free
-| | Storage for private datasets hosted by Activeloop | 100GB Free | ##
-ð©âð» Comparisons to Familiar Tools  Deep Lake vs Chroma Both Deep Lake &
-ChromaDB enable users to store and search vectors (embeddings) and offer
-integrations with LangChain and LlamaIndex. However, they are architecturally
-very different. ChromaDB is a Vector Database that can be deployed locally or
-on a server using Docker and will offer a hosted solution shortly. Deep Lake is
-a serverless Vector Store deployed on the userâs own cloud, locally, or in-
-memory. All computations run client-side, which enables users to support
-lightweight production apps in seconds. Unlike ChromaDB, Deep Lakeâs data
-format can store raw data such as images, videos, and text, in addition to
-embeddings. ChromaDB is limited to light metadata on top of the embeddings and
-has no visualization. Deep Lake datasets can be visualized and version
-controlled. Deep Lake also has a performant dataloader for fine-tuning your
-Large Language Models.   Deep Lake vs Pinecone Both Deep Lake and Pinecone
-enable users to store and search vectors (embeddings) and offer integrations
-with LangChain and LlamaIndex. However, they are architecturally very
-different. Pinecone is a fully-managed Vector Database that is optimized for
-highly demanding applications requiring search for billions of vectors. Deep
-Lake is a serverless. All computations run client-side, which enables users to
-get started in seconds. Unlike Pinecone, Deep Lakeâs data format can store
-raw data such as images, videos, and text, in addition to embeddings. Deep Lake
-datasets can be visualized and version controlled. Pinecone is limited to light
-metadata on top of the embeddings and has no visualization. Deep Lake also has
-a performant dataloader for fine-tuning your Large Language Models.   Deep Lake
-vs Weaviate Both Deep Lake and Weaviate enable users to store and search
+Platform. Universities can get up to 1TB of data storage and 100,000 monthly
+queries on the Tensor Database for free per month. Chat in on [our website]
+(https://activeloop.ai): to claim the access! ## ð©âð» Comparisons to
+Familiar Tools  Deep Lake vs Chroma Both Deep Lake & ChromaDB enable users to
+store and search vectors (embeddings) and offer integrations with LangChain and
+LlamaIndex. However, they are architecturally very different. ChromaDB is a
+Vector Database that can be deployed locally or on a server using Docker and
+will offer a hosted solution shortly. Deep Lake is a serverless Vector Store
+deployed on the userâs own cloud, locally, or in-memory. All computations run
+client-side, which enables users to support lightweight production apps in
+seconds. Unlike ChromaDB, Deep Lakeâs data format can store raw data such as
+images, videos, and text, in addition to embeddings. ChromaDB is limited to
+light metadata on top of the embeddings and has no visualization. Deep Lake
+datasets can be visualized and version controlled. Deep Lake also has a
+performant dataloader for fine-tuning your Large Language Models.   Deep Lake
+vs Pinecone Both Deep Lake and Pinecone enable users to store and search
 vectors (embeddings) and offer integrations with LangChain and LlamaIndex.
-However, they are architecturally very different. Weaviate is a Vector Database
-that can be deployed in a managed service or by the user via Kubernetes or
-Docker. Deep Lake is serverless. All computations run client-side, which
-enables users to support lightweight production apps in seconds. Unlike
-Weaviate, Deep Lakeâs data format can store raw data such as images, videos,
-and text, in addition to embeddings. Deep Lake datasets can be visualized and
-version controlled. Weaviate is limited to light metadata on top of the
-embeddings and has no visualization. Deep Lake also has a performant dataloader
-for fine-tuning your Large Language Models.   Deep Lake vs DVC Deep Lake and
-DVC offer dataset version control similar to git for data, but their methods
-for storing data differ significantly. Deep Lake converts and stores data as
-chunked compressed arrays, which enables rapid streaming to ML models, whereas
-DVC operates on top of data stored in less efficient traditional file
-structures. The Deep Lake format makes dataset versioning significantly easier
-compared to traditional file structures by DVC when datasets are composed of
-many files (i.e., many images). An additional distinction is that DVC primarily
-uses a command-line interface, whereas Deep Lake is a Python package. Lastly,
-Deep Lake offers an API to easily connect datasets to ML frameworks and other
-common ML tools and enables instant dataset visualization through [Activeloop's
-visualization tool](http://app.activeloop.ai/
-?utm_source=github&utm_medium=repo&utm_campaign=readme).   Deep Lake vs
-TensorFlow Datasets (TFDS) Deep Lake and TFDS seamlessly connect popular
-datasets to ML frameworks. Deep Lake datasets are compatible with both PyTorch
-and TensorFlow, whereas TFDS are only compatible with TensorFlow. A key
-difference between Deep Lake and TFDS is that Deep Lake datasets are designed
-for streaming from the cloud, whereas TFDS must be downloaded locally prior to
-use. As a result, with Deep Lake, one can import datasets directly from
-TensorFlow Datasets and stream them either to PyTorch or TensorFlow. In
-addition to providing access to popular publicly available datasets, Deep Lake
-also offers powerful tools for creating custom datasets, storing them on a
-variety of cloud storage providers, and collaborating with others via simple
-API. TFDS is primarily focused on giving the public easy access to commonly
-available datasets, and management of custom datasets is not the primary focus.
-A full comparison article can be found [here](https://www.activeloop.ai/
-resources/tensor-flow-tf-data-activeloop-hub-how-to-implement-your-tensor-flow-
-data-pipelines-with-hub/).   Deep Lake vs HuggingFace Deep Lake and HuggingFace
-offer access to popular datasets, but Deep Lake primarily focuses on computer
-vision, whereas HuggingFace focuses on natural language processing. HuggingFace
-Transforms and other computational tools for NLP are not analogous to features
-offered by Deep Lake.   Deep Lake vs WebDatasets Deep Lake and WebDatasets both
-offer rapid data streaming across networks. They have nearly identical steaming
-speeds because the underlying network requests and data structures are very
-similar. However, Deep Lake offers superior random access and shuffling, its
-simple API is in python instead of command-line, and Deep Lake enables simple
-indexing and modification of the dataset without having to recreate it.   Deep
-Lake vs Zarr Deep Lake and Zarr both offer storage of data as chunked arrays.
-However, Deep Lake is primarily designed for returning data as arrays using a
-simple API, rather than actually storing raw arrays (even though that's also
-possible). Deep Lake stores data in use-case-optimized formats, such as jpeg or
-png for images, or mp4 for video, and the user treats the data as if it's an
-array, because Deep Lake handles all the data processing in between. Deep Lake
-offers more flexibility for storing arrays with dynamic shape (ragged tensors),
-and it provides several features that are not naively available in Zarr such as
+However, they are architecturally very different. Pinecone is a fully-managed
+Vector Database that is optimized for highly demanding applications requiring
+search for billions of vectors. Deep Lake is a serverless. All computations run
+client-side, which enables users to get started in seconds. Unlike Pinecone,
+Deep Lakeâs data format can store raw data such as images, videos, and text,
+in addition to embeddings. Deep Lake datasets can be visualized and version
+controlled. Pinecone is limited to light metadata on top of the embeddings and
+has no visualization. Deep Lake also has a performant dataloader for fine-
+tuning your Large Language Models.   Deep Lake vs Weaviate Both Deep Lake and
+Weaviate enable users to store and search vectors (embeddings) and offer
+integrations with LangChain and LlamaIndex. However, they are architecturally
+very different. Weaviate is a Vector Database that can be deployed in a managed
+service or by the user via Kubernetes or Docker. Deep Lake is serverless. All
+computations run client-side, which enables users to support lightweight
+production apps in seconds. Unlike Weaviate, Deep Lakeâs data format can
+store raw data such as images, videos, and text, in addition to embeddings.
+Deep Lake datasets can be visualized and version controlled. Weaviate is
+limited to light metadata on top of the embeddings and has no visualization.
+Deep Lake also has a performant dataloader for fine-tuning your Large Language
+Models.   Deep Lake vs DVC Deep Lake and DVC offer dataset version control
+similar to git for data, but their methods for storing data differ
+significantly. Deep Lake converts and stores data as chunked compressed arrays,
+which enables rapid streaming to ML models, whereas DVC operates on top of data
+stored in less efficient traditional file structures. The Deep Lake format
+makes dataset versioning significantly easier compared to traditional file
+structures by DVC when datasets are composed of many files (i.e., many images).
+An additional distinction is that DVC primarily uses a command-line interface,
+whereas Deep Lake is a Python package. Lastly, Deep Lake offers an API to
+easily connect datasets to ML frameworks and other common ML tools and enables
+instant dataset visualization through [Activeloop's visualization tool](http://
+app.activeloop.ai/?utm_source=github&utm_medium=repo&utm_campaign=readme).
+Deep Lake vs MosaicML MDS format - **Data Storage Format:** Deep Lake operates
+on a columnar storage format, whereas MDS utilizes a row-wise storage approach.
+This fundamentally impacts how data is read, written, and organized in each
+system. - **Compression:** Deep Lake offers a more flexible compression scheme,
+allowing control over both chunk-level and sample-level compression for each
+column or tensor. This feature eliminates the need for additional compressions
+like zstd, which would otherwise demand more CPU cycles for decompressing on
+top of formats like jpeg. - **Shuffling:** MDS currently offers more advanced
+shuffling strategies. - **Version Control & Visualization Support:** A notable
+feature of Deep Lake is its native version control and in-browser data
+visualization, a feature not present for MosaicML data format. This can provide
+significant advantages in managing, understanding, and tracking different
+versions of the data.   Deep Lake vs TensorFlow Datasets (TFDS) Deep Lake and
+TFDS seamlessly connect popular datasets to ML frameworks. Deep Lake datasets
+are compatible with both PyTorch and TensorFlow, whereas TFDS are only
+compatible with TensorFlow. A key difference between Deep Lake and TFDS is that
+Deep Lake datasets are designed for streaming from the cloud, whereas TFDS must
+be downloaded locally prior to use. As a result, with Deep Lake, one can import
+datasets directly from TensorFlow Datasets and stream them either to PyTorch or
+TensorFlow. In addition to providing access to popular publicly available
+datasets, Deep Lake also offers powerful tools for creating custom datasets,
+storing them on a variety of cloud storage providers, and collaborating with
+others via simple API. TFDS is primarily focused on giving the public easy
+access to commonly available datasets, and management of custom datasets is not
+the primary focus. A full comparison article can be found [here](https://
+www.activeloop.ai/resources/tensor-flow-tf-data-activeloop-hub-how-to-
+implement-your-tensor-flow-data-pipelines-with-hub/).   Deep Lake vs
+HuggingFace Deep Lake and HuggingFace offer access to popular datasets, but
+Deep Lake primarily focuses on computer vision, whereas HuggingFace focuses on
+natural language processing. HuggingFace Transforms and other computational
+tools for NLP are not analogous to features offered by Deep Lake.   Deep Lake
+vs WebDatasets Deep Lake and WebDatasets both offer rapid data streaming across
+networks. They have nearly identical steaming speeds because the underlying
+network requests and data structures are very similar. However, Deep Lake
+offers superior random access and shuffling, its simple API is in python
+instead of command-line, and Deep Lake enables simple indexing and modification
+of the dataset without having to recreate it.   Deep Lake vs Zarr Deep Lake and
+Zarr both offer storage of data as chunked arrays. However, Deep Lake is
+primarily designed for returning data as arrays using a simple API, rather than
+actually storing raw arrays (even though that's also possible). Deep Lake
+stores data in use-case-optimized formats, such as jpeg or png for images, or
+mp4 for video, and the user treats the data as if it's an array, because Deep
+Lake handles all the data processing in between. Deep Lake offers more
+flexibility for storing arrays with dynamic shape (ragged tensors), and it
+provides several features that are not naively available in Zarr such as
 version control, data streaming, and connecting data to ML Frameworks.  ##
 Community Join our [**Slack community**](https://join.slack.com/t/hubdb/
 shared_invite/zt-ivhsj8sz-GWv9c5FLBDVw8vn~sxRKqQ) to learn more about
 unstructured dataset management using Deep Lake and to get help from the
 Activeloop team and other users. We'd love your feedback by completing our 3-
 minute [**survey**](https://forms.gle/rLi4w33dow6CSMcm9). As always, thanks to
 our amazing contributors! [https://contrib.rocks/image?repo=activeloopai/hub]
```

### Comparing `deeplake-3.5.4/deeplake/__init__.py` & `deeplake-3.6.0/deeplake/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     "config",
     "delete",
     "copy",
     "rename",
 ]
 
 
-__version__ = "3.5.4"
+__version__ = "3.6.0"
 warn_if_update_required(__version__)
 __encoded_version__ = np.array(__version__)
 config = {"s3": Config(max_pool_connections=50, connect_timeout=300, read_timeout=300)}
 
 
 deeplake_reporter.tags.append(f"version:{__version__}")
 deeplake_reporter.system_report(publish=True)
```

### Comparing `deeplake-3.5.4/deeplake/api/dataset.py` & `deeplake-3.6.0/deeplake/api/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,17 @@
     integrity_check,
 )
 from deeplake.util.spinner import spinner
 from deeplake.util.path import (
     convert_pathlib_to_string_if_needed,
     verify_dataset_name,
     process_dataset_path,
+    get_path_type,
 )
+from deeplake.util.tensor_db import parse_runtime_parameters
 from deeplake.hooks import (
     dataset_created,
     dataset_loaded,
     dataset_written,
     dataset_committed,
 )
 from deeplake.constants import (
@@ -168,15 +170,15 @@
         Raises:
             AgreementError: When agreement is rejected
             UserNotLoggedInException: When user is not logged in
             InvalidTokenException: If the specified token is invalid
             TokenPermissionError: When there are permission or other errors related to token
             CheckoutError: If version address specified in the path cannot be found
             DatasetCorruptError: If loading the dataset failed due to corruption and ``reset`` is not ``True``
-            ValueError: If version is specified in the path when creating a dataset
+            ValueError: If version is specified in the path when creating a dataset or If the org id is provided but dataset is ot local, or If the org id is provided but dataset is ot local
             ReadOnlyModeError: If reset is attempted in read-only mode
             LockedException: When attempting to open a dataset for writing when it is locked by another machine
             Exception: Re-raises caught exception if reset cannot fix the issue
 
         Danger:
             Setting ``overwrite`` to ``True`` will delete all of your data if it exists! Be very careful when setting this parameter.
 
@@ -188,18 +190,21 @@
         """
         access_method, num_workers, scheduler = parse_access_method(access_method)
         check_access_method(access_method, overwrite)
 
         path, address = process_dataset_path(path)
         verify_dataset_name(path)
 
+        if org_id is not None and get_path_type(path) != "local":
+            raise ValueError("org_id parameter can only be used with local datasets")
+
         if creds is None:
             creds = {}
 
-        db_engine = (runtime or {}).get("db_engine", {})
+        db_engine = parse_runtime_parameters(path, runtime)["tensor_db"]
 
         try:
             storage, cache_chain = get_storage_and_cache_chain(
                 path=path,
                 db_engine=db_engine,
                 read_only=read_only,
                 creds=creds,
@@ -341,20 +346,20 @@
         token: Optional[str] = None,
         org_id: Optional[str] = None,
         verbose: bool = True,
     ) -> Dataset:
         """Creates an empty dataset
 
         Args:
-            path (str, pathlib.Path): - The full path to the dataset. Can be:
-                - a Deep Lake cloud path of the form ``hub://username/datasetname``. To write to Deep Lake cloud datasets, ensure that you are logged in to Deep Lake (use 'activeloop login' from command line)
+            path (str, pathlib.Path): - The full path to the dataset. It can be:
+                - a Deep Lake cloud path of the form ``hub://org_id/dataset_name``. Requires registration with Deep Lake.
                 - an s3 path of the form ``s3://bucketname/path/to/dataset``. Credentials are required in either the environment or passed to the creds argument.
                 - a local file system path of the form ``./path/to/dataset`` or ``~/path/to/dataset`` or ``path/to/dataset``.
                 - a memory path of the form ``mem://path/to/dataset`` which doesn't save the dataset but keeps it in memory instead. Should be used only for testing as it does not persist.
-            runtime (dict): Parameters for Activeloop DB Engine. Only applicable for hub:// paths.
+            runtime (dict): Parameters for creating a dataset in the Deep Lake Tensor Database. Only applicable for paths of the form ``hub://org_id/dataset_name`` and runtime  must be ``{"tensor_db": True}``.
             overwrite (bool): If set to ``True`` this overwrites the dataset if it already exists. Defaults to ``False``.
             public (bool): Defines if the dataset will have public access. Applicable only if Deep Lake cloud storage is used and a new Dataset is being created. Defaults to ``False``.
             memory_cache_size (int): The size of the memory cache to be used in MB.
             local_cache_size (int): The size of the local filesystem cache to be used in MB.
             creds (dict, str, optional): The string ``ENV`` or a dictionary containing credentials used to access the dataset at the path.
                 - If 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token' are present, these take precedence over credentials present in the environment or in credentials file. Currently only works with s3 paths.
                 - It supports 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token', 'endpoint_url', 'aws_region', 'profile_name' as keys.
@@ -373,15 +378,19 @@
             TokenPermissionError: When there are permission or other errors related to token
             ValueError: If version is specified in the path
 
         Danger:
             Setting ``overwrite`` to ``True`` will delete all of your data if it exists! Be very careful when setting this parameter.
         """
         path, address = process_dataset_path(path)
-        db_engine = (runtime or {}).get("db_engine", False)
+
+        if org_id is not None and get_path_type(path) != "local":
+            raise ValueError("org_id parameter can only be used with local datasets")
+
+        db_engine = parse_runtime_parameters(path, runtime)["tensor_db"]
 
         if address:
             raise ValueError(
                 "deeplake.empty does not accept version address in the dataset path."
             )
 
         verify_dataset_name(path)
@@ -519,14 +528,15 @@
             InvalidTokenException: If the specified toke is invalid
             TokenPermissionError: When there are permission or other errors related to token
             CheckoutError: If version address specified in the path cannot be found
             DatasetCorruptError: If loading the dataset failed due to corruption and ``reset`` is not ``True``
             ReadOnlyModeError: If reset is attempted in read-only mode
             LockedException: When attempting to open a dataset for writing when it is locked by another machine
             Exception: Re-raises caught exception if reset cannot fix the issue
+            ValueError: If the org id is provided but the dataset is not local
 
         Warning:
             Setting ``access_method`` to download will overwrite the local copy of the dataset if it was previously downloaded.
 
         Note:
             Any changes made to the dataset in download / local mode will only be made to the local copy and will not be reflected in the original dataset.
         """
@@ -534,14 +544,17 @@
         check_access_method(access_method, overwrite=False)
 
         path, address = process_dataset_path(path)
 
         if creds is None:
             creds = {}
 
+        if org_id is not None and get_path_type(path) != "local":
+            raise ValueError("org_id parameter can only be used with local datasets")
+
         try:
             storage, cache_chain = get_storage_and_cache_chain(
                 path=path,
                 read_only=read_only,
                 creds=creds,
                 token=token,
                 memory_cache_size=memory_cache_size,
@@ -807,14 +820,15 @@
         runtime: Optional[Dict] = None,
         tensors: Optional[List[str]] = None,
         overwrite: bool = False,
         creds: Optional[Union[dict, str]] = None,
         token: Optional[str] = None,
         org_id: Optional[str] = None,
         public: bool = False,
+        verbose: bool = True,
     ) -> Dataset:
         """Creates a new dataset by copying the ``source`` dataset's structure to a new location. No samples are copied,
         only the meta/info for the dataset and it's tensors.
 
         Args:
             dest: Empty Dataset or Path where the new dataset will be created.
             src (Union[str, Dataset]): Path or dataset object that will be used as the template for the new dataset.
@@ -824,43 +838,62 @@
             creds (dict, str, optional): The string ``ENV`` or a dictionary containing credentials used to access the dataset at the path.
                 - If 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token' are present, these take precedence over credentials present in the environment or in credentials file. Currently only works with s3 paths.
                 - It supports 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token', 'endpoint_url', 'aws_region', 'profile_name' as keys.
                 - If 'ENV' is passed, credentials are fetched from the environment variables. This is also the case when creds is not passed for cloud datasets. For datasets connected to hub cloud, specifying 'ENV' will override the credentials fetched from Activeloop and use local ones.
             token (str, optional): Activeloop token, used for fetching credentials to the dataset at path if it is a Deep Lake dataset. This is optional, tokens are normally autogenerated.
             org_id (str, Optional): Organization id to be used for enabling enterprise features. Only applicable for local datasets.
             public (bool): Defines if the dataset will have public access. Applicable only if Deep Lake cloud storage is used and a new Dataset is being created. Defaults to False.
+            verbose (bool): If True, logs will be printed. Defaults to ``True``.
+
 
         Returns:
             Dataset: New dataset object.
+
+        Raises:
+            ValueError: If the org id is provided but the dataset is not local
         """
         if isinstance(dest, Dataset):
             path = dest.path
         else:
             path = dest
+
+        if org_id is not None and get_path_type(path) != "local":
+            raise ValueError("org_id parameter can only be used with local datasets")
+
         feature_report_path(
             path,
             "like",
             {"Overwrite": overwrite, "Public": public, "Tensors": tensors},
             token=token,
         )
         return dataset._like(
-            dest, src, runtime, tensors, overwrite, creds, token, org_id, public
+            dest,
+            src,
+            runtime,
+            tensors,
+            overwrite,
+            creds,
+            token,
+            org_id,
+            public,
+            verbose,
         )
 
     @staticmethod
     def _like(  # (No reporting)
         dest,
         src: Union[str, Dataset],
         runtime: Optional[Dict] = None,
         tensors: Optional[List[str]] = None,
         overwrite: bool = False,
         creds: Optional[Union[dict, str]] = None,
         token: Optional[str] = None,
         org_id: Optional[str] = None,
         public: bool = False,
+        verbose: bool = True,
         unlink: Union[List[str], bool] = False,
     ) -> Dataset:
         """Copies the `source` dataset's structure to a new location. No samples are copied, only the meta/info for the dataset and it's tensors.
 
         Args:
             dest: Empty Dataset or Path where the new dataset will be created.
             src (Union[str, Dataset]): Path or dataset object that will be used as the template for the new dataset.
@@ -872,47 +905,52 @@
             creds (dict, str, optional): The string ``ENV`` or a dictionary containing credentials used to access the dataset at the path.
                 - If 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token' are present, these take precedence over credentials present in the environment or in credentials file. Currently only works with s3 paths.
                 - It supports 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token', 'endpoint_url', 'aws_region', 'profile_name' as keys.
                 - If 'ENV' is passed, credentials are fetched from the environment variables. This is also the case when creds is not passed for cloud datasets. For datasets connected to hub cloud, specifying 'ENV' will override the credentials fetched from Activeloop and use local ones.
             token (str, optional): Activeloop token, used for fetching credentials to the dataset at path if it is a Deep Lake dataset. This is optional, tokens are normally autogenerated.
             org_id (str, Optional): Organization id to be used for enabling enterprise features. Only applicable for local datasets.
             public (bool): Defines if the dataset will have public access. Applicable only if Deep Lake cloud storage is used and a new Dataset is being created. Defaults to ``False``.
+            verbose (bool): If True, logs will be printed. Defaults to ``True``.
             unlink (Union[List[str], bool]): List of tensors to be unlinked. If ``True`` passed all tensors will be unlinked. Defaults to ``False``, no tensors are unlinked.
 
         Returns:
             Dataset: New dataset object.
         """
+
+        src = convert_pathlib_to_string_if_needed(src)
+        if isinstance(src, str):
+            source_ds = dataset.load(src, verbose=verbose)
+        else:
+            source_ds = src
+
+        if tensors:
+            tensors = source_ds._resolve_tensor_list(tensors)  # type: ignore
+        else:
+            tensors = source_ds.tensors  # type: ignore
+
         dest = convert_pathlib_to_string_if_needed(dest)
         if isinstance(dest, Dataset):
             destination_ds = dest
             dest_path = dest.path
         else:
             dest_path = dest
             destination_ds = dataset.empty(
                 dest,
                 runtime=runtime,
                 creds=creds,
                 overwrite=overwrite,
                 token=token,
                 org_id=org_id,
                 public=public,
+                verbose=verbose,
             )
+
         feature_report_path(
             dest_path, "like", {"Overwrite": overwrite, "Public": public}, token=token
         )
-        src = convert_pathlib_to_string_if_needed(src)
-        if isinstance(src, str):
-            source_ds = dataset.load(src)
-        else:
-            source_ds = src
-
-        if tensors:
-            tensors = source_ds._resolve_tensor_list(tensors)  # type: ignore
-        else:
-            tensors = source_ds.tensors  # type: ignore
 
         if unlink is True:
             unlink = tensors  # type: ignore
         elif unlink is False:
             unlink = []
         for tensor_name in tensors:  # type: ignore
             if overwrite and tensor_name in destination_ds:
@@ -1087,15 +1125,15 @@
                 "The source dataset is corrupted.",
                 "You can try to fix this by loading the dataset with `reset=True` "
                 "which will attempt to reset uncommitted HEAD changes and load the previous version.",
                 e.__cause__,
             )
         src_storage = get_base_storage(src_ds.storage)
 
-        db_engine = (runtime or {}).get("db_engine", False)
+        db_engine = parse_runtime_parameters(dest, runtime)["tensor_db"]
         dest_storage, cache_chain = get_storage_and_cache_chain(
             dest,
             db_engine=db_engine,
             creds=dest_creds,
             token=token,
             read_only=False,
             memory_cache_size=DEFAULT_MEMORY_CACHE_SIZE,
@@ -1236,26 +1274,27 @@
             >>> # or
             >>> ds = deeplake.connect(src_path="s3://bucket/dataset", org_id="my_org", creds_key="my_managed_credentials_key", token="my_activeloop_token")
 
         Args:
             src_path (str): Cloud path to the source dataset. Can be:
                 an s3 path like ``s3://bucket/path/to/dataset``.
                 a gcs path like ``gcs://bucket/path/to/dataset``.
+                an azure path like ``az://account_name/container/path/to/dataset``.
             creds_key (str): The managed credentials to be used for accessing the source path.
             dest_path (str, optional): The full path to where the connected Deep Lake dataset will reside. Can be:
                 a Deep Lake path like ``hub://organization/dataset``
             org_id (str, optional): The organization to where the connected Deep Lake dataset will be added.
             ds_name (str, optional): The name of the connected Deep Lake dataset. Will be infered from ``dest_path`` or ``src_path`` if not provided.
             token (str, optional): Activeloop token used to fetch the managed credentials.
 
         Returns:
             Dataset: The connected Deep Lake dataset.
 
         Raises:
-            InvalidSourcePathError: If the ``src_path`` is not a valid s3 or gcs path.
+            InvalidSourcePathError: If the ``src_path`` is not a valid s3, gcs or azure path.
             InvalidDestinationPathError: If ``dest_path``, or ``org_id`` and ``ds_name`` do not form a valid Deep Lake path.
         """
         path = connect_dataset_entry(
             src_path=src_path,
             creds_key=creds_key,
             dest_path=dest_path,
             org_id=org_id,
```

### Comparing `deeplake-3.5.4/deeplake/api/info.py` & `deeplake-3.6.0/deeplake/api/info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/api/link.py` & `deeplake-3.6.0/deeplake/api/link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/api/link_tiled.py` & `deeplake-3.6.0/deeplake/api/link_tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/api/read.py` & `deeplake-3.6.0/deeplake/api/read.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/api/tests/test_access_method.py` & `deeplake-3.6.0/deeplake/api/tests/test_access_method.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/api/tests/test_agreement.py` & `deeplake-3.6.0/deeplake/api/tests/test_agreement.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/api/tests/test_api.py` & `deeplake-3.6.0/deeplake/api/tests/test_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -860,20 +860,38 @@
 
         deeplake.delete("test/", large_ok=True)
         assert not os.path.isfile("test/dataset_meta.json")
 
         deeplake.constants.DELETE_SAFETY_SIZE = old_size
 
 
+def test_invalid_token():
+    with pytest.raises(InvalidTokenException):
+        ds = deeplake.load(
+            "hub://activeloop-test/sohas-weapons-train", token="invalid token"
+        )
+
+    with pytest.raises(InvalidTokenException):
+        ds = deeplake.empty(
+            "hub://activeloop-test/sohas-weapons-train", token="invalid token"
+        )
+
+    with pytest.raises(InvalidTokenException):
+        ds = deeplake.dataset(
+            "hub://activeloop-test/sohas-weapons-train", token="invalid token"
+        )
+
+
 @pytest.mark.parametrize(
     ("ds_generator", "path", "hub_token"),
     [
         ("local_ds_generator", "local_path", "hub_cloud_dev_token"),
         ("s3_ds_generator", "s3_path", "hub_cloud_dev_token"),
         ("gcs_ds_generator", "gcs_path", "hub_cloud_dev_token"),
+        ("azure_ds_generator", "azure_path", "hub_cloud_dev_token"),
         ("hub_cloud_ds_generator", "hub_cloud_path", "hub_cloud_dev_token"),
     ],
     indirect=True,
 )
 @pytest.mark.parametrize("convert_to_pathlib", [True, False])
 def test_dataset_rename(ds_generator, path, hub_token, convert_to_pathlib):
     ds = ds_generator()
@@ -898,29 +916,14 @@
     ds = deeplake.rename(ds.path, new_path, token=hub_token)
     assert ds.path == str(new_path)
     assert_array_equal(ds.abc.numpy(), np.array([[1, 2, 3, 4]]))
 
     ds = deeplake.load(new_path, token=hub_token)
     assert_array_equal(ds.abc.numpy(), np.array([[1, 2, 3, 4]]))
 
-    with pytest.raises(InvalidTokenException):
-        ds = deeplake.load(
-            "hub://activeloop-test/sohas-weapons-train", token="invalid token"
-        )
-
-    with pytest.raises(InvalidTokenException):
-        ds = deeplake.empty(
-            "hub://activeloop-test/sohas-weapons-train", token="invalid token"
-        )
-
-    with pytest.raises(InvalidTokenException):
-        ds = deeplake.dataset(
-            "hub://activeloop-test/sohas-weapons-train", token="invalid token"
-        )
-
     deeplake.delete(new_path, token=hub_token)
 
 
 @pytest.mark.parametrize(
     "path,hub_token",
     [
         ["local_path", "hub_cloud_dev_token"],
@@ -2598,7 +2601,26 @@
 def test_shape_squeeze(memory_ds):
     with memory_ds as ds:
         ds.create_tensor("abc")
         ds.abc.extend(np.ones((5, 10, 10, 10)))
         ds.abc.extend(np.ones((5, 10, 12, 20)))
 
     assert ds.abc[5:, :, 9].shape == (5, 10, 20)
+
+
+def test_non_local_org_id():
+    with pytest.raises(ValueError):
+        ds = deeplake.dataset("hub://test/test_dataset", org_id="test")
+
+    with pytest.raises(ValueError):
+        ds = deeplake.empty("hub://test/test_dataset", org_id="test")
+
+    with pytest.raises(ValueError):
+        ds = deeplake.load("hub://test/test_dataset", org_id="test")
+
+    with pytest.raises(ValueError):
+        ds = deeplake.like("hub://test/test_dataset", "test/test_ds", org_id="test")
+
+
+def test_azure_bad_path():
+    with pytest.raises(ValueError):
+        ds = deeplake.empty("az://storage_account")
```

### Comparing `deeplake-3.5.4/deeplake/api/tests/test_api_tiling.py` & `deeplake-3.6.0/deeplake/api/tests/test_api_tiling.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/api/tests/test_api_with_compression.py` & `deeplake-3.6.0/deeplake/api/tests/test_api_with_compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/api/tests/test_chunk_sizes.py` & `deeplake-3.6.0/deeplake/api/tests/test_chunk_sizes.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/api/tests/test_connect_datasets.py` & `deeplake-3.6.0/deeplake/api/tests/test_connect_datasets.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/api/tests/test_dataset.py` & `deeplake-3.6.0/deeplake/api/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/api/tests/test_dicom.py` & `deeplake-3.6.0/deeplake/api/tests/test_dicom.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/api/tests/test_downsample.py` & `deeplake-3.6.0/deeplake/api/tests/test_downsample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/api/tests/test_events.py` & `deeplake-3.6.0/deeplake/api/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/api/tests/test_grayscale.py` & `deeplake-3.6.0/deeplake/api/tests/test_grayscale.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/api/tests/test_info.py` & `deeplake-3.6.0/deeplake/api/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/api/tests/test_insertion_out_of_order.py` & `deeplake-3.6.0/deeplake/api/tests/test_insertion_out_of_order.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/api/tests/test_json.py` & `deeplake-3.6.0/deeplake/api/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/api/tests/test_link.py` & `deeplake-3.6.0/deeplake/api/tests/test_link.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import numpy as np
 import os
 import sys
 import pickle
 import deeplake
 import pytest
 from deeplake.client.client import DeepLakeBackendClient
-from deeplake.constants import GCS_OPT, S3_OPT
+from deeplake.constants import GCS_OPT, S3_OPT, AZURE_OPT
 from deeplake.core.link_creds import LinkCreds
 from deeplake.core.meta.encode.creds import CredsEncoder
 from deeplake.core.storage.gcs import GCSProvider
 from deeplake.core.storage.s3 import S3Provider
+from deeplake.core.storage.azure import AzureProvider
 from deeplake.tests.common import is_opt_true
 from deeplake.util.exceptions import (
     ManagedCredentialsNotFoundError,
     MissingCredsError,
     SampleAppendError,
     TensorMetaInvalidHtype,
     UnableToReadFromUrlError,
@@ -117,14 +118,22 @@
         assert isinstance(link_creds.get_storage_provider("def", "gcs"), GCSProvider)
         assert isinstance(link_creds.get_storage_provider("def", "gcs"), GCSProvider)
         assert isinstance(link_creds.get_storage_provider(None, "gcs"), GCSProvider)
     if is_opt_true(request, S3_OPT):
         assert isinstance(link_creds.get_storage_provider("abc", "s3"), S3Provider)
         assert isinstance(link_creds.get_storage_provider("abc", "s3"), S3Provider)
         assert isinstance(link_creds.get_storage_provider(None, "s3"), S3Provider)
+    if is_opt_true(request, AZURE_OPT):
+        assert isinstance(
+            link_creds.get_storage_provider("abc", "azure"), AzureProvider
+        )
+        assert isinstance(
+            link_creds.get_storage_provider("abc", "azure"), AzureProvider
+        )
+        assert isinstance(link_creds.get_storage_provider(None, "azure"), AzureProvider)
 
     pickled = pickle.dumps(link_creds)
     unpickled_link_creds = pickle.loads(pickled)
 
     assert len(unpickled_link_creds) == 3
     assert unpickled_link_creds.get_creds_key(0) is None
     assert unpickled_link_creds.get_creds_key(1) == "abc"
```

### Comparing `deeplake-3.5.4/deeplake/api/tests/test_link_tiled.py` & `deeplake-3.6.0/deeplake/api/tests/test_link_tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/api/tests/test_linking.py` & `deeplake-3.6.0/deeplake/api/tests/test_linking.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/api/tests/test_mesh.py` & `deeplake-3.6.0/deeplake/api/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/api/tests/test_meta.py` & `deeplake-3.6.0/deeplake/api/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/api/tests/test_nifti.py` & `deeplake-3.6.0/deeplake/api/tests/test_nifti.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/api/tests/test_none.py` & `deeplake-3.6.0/deeplake/api/tests/test_none.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/api/tests/test_partial_upload.py` & `deeplake-3.6.0/deeplake/api/tests/test_partial_upload.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/api/tests/test_pickle.py` & `deeplake-3.6.0/deeplake/api/tests/test_pickle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/api/tests/test_point_cloud.py` & `deeplake-3.6.0/deeplake/api/tests/test_point_cloud.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/api/tests/test_polygons.py` & `deeplake-3.6.0/deeplake/api/tests/test_polygons.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/api/tests/test_pop.py` & `deeplake-3.6.0/deeplake/api/tests/test_pop.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/api/tests/test_readonly.py` & `deeplake-3.6.0/deeplake/api/tests/test_readonly.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/api/tests/test_rechunk.py` & `deeplake-3.6.0/deeplake/api/tests/test_rechunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/api/tests/test_reset.py` & `deeplake-3.6.0/deeplake/api/tests/test_reset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/api/tests/test_sample_info.py` & `deeplake-3.6.0/deeplake/api/tests/test_sample_info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/api/tests/test_text.py` & `deeplake-3.6.0/deeplake/api/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/api/tests/test_update_samples.py` & `deeplake-3.6.0/deeplake/api/tests/test_update_samples.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/api/tests/test_video.py` & `deeplake-3.6.0/deeplake/api/tests/test_video.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,14 +62,15 @@
 @pytest.mark.skipif(
     os.name == "nt" and sys.version_info < (3, 7), reason="requires python 3.7 or above"
 )
 @pytest.mark.parametrize(
     ("vstream_path", "hub_token"),
     [
         ("gcs_vstream_path", "hub_cloud_dev_token"),
+        ("azure_vstream_path", "hub_cloud_dev_token"),
         ("s3_vstream_path", "hub_cloud_dev_token"),
         ("hub_cloud_vstream_path", "hub_cloud_dev_token"),
     ],
     indirect=True,
 )
 def test_video_streaming(vstream_path, hub_token):
     ds = deeplake.load(vstream_path, read_only=True, token=hub_token)
@@ -89,14 +90,15 @@
 @pytest.mark.skipif(
     os.name == "nt" and sys.version_info < (3, 7), reason="requires python 3.7 or above"
 )
 @pytest.mark.parametrize(
     ("vstream_path", "hub_token"),
     [
         ("gcs_vstream_path", "hub_cloud_dev_token"),
+        ("azure_vstream_path", "hub_cloud_dev_token"),
         ("s3_vstream_path", "hub_cloud_dev_token"),
         ("hub_cloud_vstream_path", "hub_cloud_dev_token"),
     ],
     indirect=True,
 )
 def test_video_timestamps(vstream_path, hub_token):
     ds = deeplake.load(vstream_path, read_only=True, token=hub_token)
```

### Comparing `deeplake-3.5.4/deeplake/api/tests/test_views.py` & `deeplake-3.6.0/deeplake/api/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/api/tiled.py` & `deeplake-3.6.0/deeplake/api/tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/auto/structured/base.py` & `deeplake-3.6.0/deeplake/auto/structured/base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/auto/structured/dataframe.py` & `deeplake-3.6.0/deeplake/auto/structured/dataframe.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/auto/tests/test_coco_template.py` & `deeplake-3.6.0/deeplake/auto/tests/test_coco_template.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/auto/tests/test_ingestion.py` & `deeplake-3.6.0/deeplake/auto/tests/test_ingestion.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/auto/tests/test_kaggle.py` & `deeplake-3.6.0/deeplake/auto/tests/test_kaggle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/auto/tests/test_yolo_template.py` & `deeplake-3.6.0/deeplake/auto/tests/test_yolo_template.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/auto/unstructured/base.py` & `deeplake-3.6.0/deeplake/auto/unstructured/base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/auto/unstructured/coco/coco.py` & `deeplake-3.6.0/deeplake/auto/unstructured/coco/coco.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/auto/unstructured/coco/constants.py` & `deeplake-3.6.0/deeplake/auto/unstructured/coco/constants.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/auto/unstructured/coco/convert.py` & `deeplake-3.6.0/deeplake/auto/unstructured/coco/convert.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/auto/unstructured/coco/utils.py` & `deeplake-3.6.0/deeplake/auto/unstructured/coco/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/auto/unstructured/image_classification.py` & `deeplake-3.6.0/deeplake/auto/unstructured/image_classification.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/auto/unstructured/kaggle.py` & `deeplake-3.6.0/deeplake/auto/unstructured/kaggle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/auto/unstructured/util.py` & `deeplake-3.6.0/deeplake/auto/unstructured/util.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/auto/unstructured/yolo/utils.py` & `deeplake-3.6.0/deeplake/auto/unstructured/yolo/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/auto/unstructured/yolo/yolo.py` & `deeplake-3.6.0/deeplake/auto/unstructured/yolo/yolo.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/cli/auth.py` & `deeplake-3.6.0/deeplake/cli/auth.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/cli/test_cli.py` & `deeplake-3.6.0/deeplake/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/client/client.py` & `deeplake-3.6.0/deeplake/client/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import deeplake
 import requests
-from typing import Any, Optional, List, Tuple
+from typing import Any, Optional, Dict
 from deeplake.util.exceptions import (
     AgreementNotAcceptedError,
     AuthorizationException,
     LoginException,
     InvalidPasswordException,
     ManagedCredentialsNotFoundError,
     NotLoggedInAgreementError,
@@ -488,33 +488,26 @@
             endpoint=self.endpoint(),
         ).json()
 
         return response["generated_id"]
 
     def remote_query(
         self, org_id: str, ds_name: str, query_string: str
-    ) -> Tuple[Any, Any]:
+    ) -> Dict[str, Any]:
         """Queries a remote dataset.
 
         Args:
             org_id (str): The organization to which the dataset belongs.
             ds_name (str): The name of the dataset.
             query_string (str): The query string.
 
         Returns:
-            Tuple[Any, Any]: The indices and scores matching the query.
+            Dict[str, Any]: The json response containing matching indicies and data from virtual tensors.
         """
         response = self.request(
             "POST",
             REMOTE_QUERY_SUFFIX.format(org_id, ds_name),
             json={"query": query_string},
             endpoint=self.endpoint(),
         ).json()
 
-        indices = response["indices"]
-        if len(indices) == 0:
-            return [], []
-
-        scores = response.get("score")
-
-        indices = [int(i) for i in indices.split(",")]
-        return indices, scores
+        return response
```

### Comparing `deeplake-3.5.4/deeplake/client/config.py` & `deeplake-3.6.0/deeplake/client/config.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/client/log.py` & `deeplake-3.6.0/deeplake/client/log.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/client/test_client.py` & `deeplake-3.6.0/deeplake/client/test_client.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/client/utils.py` & `deeplake-3.6.0/deeplake/client/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/compression.py` & `deeplake-3.6.0/deeplake/compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/constants.py` & `deeplake-3.6.0/deeplake/constants.py`

 * *Files 18% similar despite different names*

```diff
@@ -78,39 +78,48 @@
 
 ENCODING_DTYPE = np.uint32
 
 # environment variables
 ENV_HUB_DEV_USERNAME = "ACTIVELOOP_HUB_USERNAME"
 ENV_HUB_DEV_PASSWORD = "ACTIVELOOP_HUB_PASSWORD"
 ENV_HUB_DEV_MANAGED_CREDS_KEY = "ACTIVELOOP_HUB_MANAGED_CREDS_KEY"
+
 ENV_KAGGLE_USERNAME = "KAGGLE_USERNAME"
 ENV_KAGGLE_KEY = "KAGGLE_KEY"
+
 ENV_GOOGLE_APPLICATION_CREDENTIALS = "GOOGLE_APPLICATION_CREDENTIALS"
+
+ENV_AZURE_CLIENT_ID = "AZURE_CLIENT_ID"
+ENV_AZURE_TENANT_ID = "AZURE_TENANT_ID"
+ENV_AZURE_SUBSCRIPTION_ID = "AZURE_SUBSCRIPTION_ID"
+
 ENV_GDRIVE_CLIENT_ID = "GDRIVE_CLIENT_ID"
 ENV_GDRIVE_CLIENT_SECRET = "GDRIVE_CLIENT_SECRET"
 ENV_GDRIVE_REFRESH_TOKEN = "GDRIVE_REFRESH_TOKEN"
 
 HUB_CLOUD_DEV_USERNAME = os.getenv(ENV_HUB_DEV_USERNAME)  # type: ignore
 HUB_CLOUD_DEV_PASSWORD = os.getenv(ENV_HUB_DEV_PASSWORD)
 
 # dataset base roots for pytests
 PYTEST_MEMORY_PROVIDER_BASE_ROOT = "mem://hub_pytest"
-PYTEST_LOCAL_PROVIDER_BASE_ROOT = "/tmp/hub_pytest/"  # TODO: may fail for windows
+PYTEST_LOCAL_PROVIDER_BASE_ROOT = "./hub_pytest/"  # TODO: may fail for windows
 PYTEST_S3_PROVIDER_BASE_ROOT = "s3://hub-2.0-tests/"
 PYTEST_GCS_PROVIDER_BASE_ROOT = "gcs://snark-test/"
+PYTEST_AZURE_PROVIDER_BASE_ROOT = "az://activeloopgen2/deeplake-tests/"
 PYTEST_GDRIVE_PROVIDER_BASE_ROOT = "gdrive://hubtest"
 PYTEST_HUB_CLOUD_PROVIDER_BASE_ROOT = (
     None if HUB_CLOUD_DEV_USERNAME is None else f"hub://{HUB_CLOUD_DEV_USERNAME}/"
 )
 
 # pytest options
 MEMORY_OPT = "--memory-skip"
 LOCAL_OPT = "--local"
 S3_OPT = "--s3"
 GCS_OPT = "--gcs"
+AZURE_OPT = "--azure"
 GDRIVE_OPT = "--gdrive"
 HUB_CLOUD_OPT = "--hub-cloud"
 S3_PATH_OPT = "--s3-path"
 GDRIVE_PATH_OPT = "--gdrive-path"
 KEEP_STORAGE_OPT = "--keep-storage"
 KAGGLE_OPT = "--kaggle"
 
@@ -139,15 +148,22 @@
 
 PARTIAL_NUM_SAMPLES = 0.5
 FAST_EXTEND_BAIL = -1
 
 QUERIES_FILENAME = "queries.json"
 QUERIES_LOCK_FILENAME = "queries.lock"
 
-ALL_CLOUD_PREFIXES = ("s3://", "gcs://", "gcp://", "gs://", "gdrive://")
+ALL_CLOUD_PREFIXES = (
+    "s3://",
+    "gcs://",
+    "gcp://",
+    "gs://",
+    "az://",
+    "azure://" "gdrive://",
+)
 
 _ENABLE_HUB_SUB_DATASETS = False
 _ENABLE_RANDOM_ASSIGNMENT = True
 
 # Frequency for sending progress events and writing to vds
 QUERY_PROGRESS_UPDATE_FREQUENCY = 5  # seconds
 
@@ -189,8 +205,40 @@
 # Transform cache sizes
 DEFAULT_TRANSFORM_SAMPLE_CACHE_SIZE = 16
 TRANSFORM_CHUNK_CACHE_SIZE = 64 * MB
 
 DEFAULT_VECTORSTORE_DEEPLAKE_PATH = "./deeplake_vector_store"
 MAX_VECTORSTORE_INGESTION_RETRY_ATTEMPTS = 5
 MAX_CHECKPOINTING_INTERVAL = 100000
-MAX_DATASET_LENGTH_FOR_CACHING = 100000
+VECTORSTORE_EXTEND_MAX_SIZE = 20000
+DEFAULT_VECTORSTORE_TENSORS = [
+    {
+        "name": "text",
+        "htype": "text",
+        "create_id_tensor": False,
+        "create_sample_info_tensor": False,
+        "create_shape_tensor": False,
+    },
+    {
+        "name": "metadata",
+        "htype": "json",
+        "create_id_tensor": False,
+        "create_sample_info_tensor": False,
+        "create_shape_tensor": False,
+    },
+    {
+        "name": "embedding",
+        "htype": "embedding",
+        "dtype": np.float32,
+        "create_id_tensor": False,
+        "create_sample_info_tensor": False,
+        "create_shape_tensor": True,
+        "max_chunk_size": 64 * MB,
+    },
+    {
+        "name": "id",
+        "htype": "text",
+        "create_id_tensor": False,
+        "create_sample_info_tensor": False,
+        "create_shape_tensor": False,
+    },
+]
```

### Comparing `deeplake-3.5.4/deeplake/core/chunk/base_chunk.py` & `deeplake-3.6.0/deeplake/core/chunk/base_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/chunk/chunk_compressed_chunk.py` & `deeplake-3.6.0/deeplake/core/chunk/chunk_compressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/chunk/sample_compressed_chunk.py` & `deeplake-3.6.0/deeplake/core/chunk/sample_compressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/chunk/test_chunk_compressed.py` & `deeplake-3.6.0/deeplake/core/chunk/test_chunk_compressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/chunk/test_sample_compressed.py` & `deeplake-3.6.0/deeplake/core/chunk/test_sample_compressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/chunk/test_uncompressed.py` & `deeplake-3.6.0/deeplake/core/chunk/test_uncompressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/chunk/uncompressed_chunk.py` & `deeplake-3.6.0/deeplake/core/chunk/uncompressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/chunk_engine.py` & `deeplake-3.6.0/deeplake/core/chunk_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from deeplake.core.version_control.commit_diff import CommitDiff
 from deeplake.core.partial_reader import PartialReader
 from deeplake.core.version_control.commit_node import CommitNode  # type: ignore
 from deeplake.core.version_control.commit_chunk_map import CommitChunkMap  # type: ignore
 from typing import Any, Dict, List, Optional, Sequence, Union, Callable
 from deeplake.core.meta.encode.tile import TileEncoder
 from deeplake.core.storage.provider import StorageProvider
-from deeplake.core.storage import S3Provider, GCSProvider
+from deeplake.core.storage import S3Provider, GCSProvider, AzureProvider
 from deeplake.core.tiling.deserialize import (
     combine_chunks,
     translate_slices,
     coalesce_tiles,
 )
 from deeplake.core.tiling.serialize import break_into_tiles
 from deeplake.core.polygon import Polygons
@@ -594,15 +594,15 @@
         """Returns video chunks. Chunk will contain presigned url to the video instead of data if the chunk is large."""
         chunk_name = ChunkIdEncoder.name_from_id(chunk_id)
         chunk_commit_id, tkey = self.get_chunk_commit(chunk_name)
         chunk_key = get_chunk_key(tkey, chunk_name, chunk_commit_id)
 
         base_storage = self.base_storage
         stream = False
-        if isinstance(base_storage, (S3Provider, GCSProvider)):
+        if isinstance(base_storage, (S3Provider, GCSProvider, AzureProvider)):
             chunk_size = base_storage.get_object_size(chunk_key)
             stream = chunk_size > self.min_chunk_size
             if stream:
                 chunk = self.cache.get_deeplake_object(
                     chunk_key, self.chunk_class, meta=self.chunk_args, url=True
                 )
         if not stream:
@@ -1798,15 +1798,15 @@
         chunk_id, row = out[0][0], out[0][1]
 
         worst_case_header_size = 0
         num_samples_in_chunk = -1
         if (
             not fetch_chunks
             and self.chunk_class != ChunkCompressedChunk
-            and isinstance(self.base_storage, (S3Provider, GCSProvider))
+            and isinstance(self.base_storage, (S3Provider, GCSProvider, AzureProvider))
         ):
             prev = int(enc.array[row - 1][LAST_SEEN_INDEX_COLUMN]) if row > 0 else -1
             num_samples_in_chunk = int(enc.array[row][LAST_SEEN_INDEX_COLUMN]) - prev
             worst_case_header_size += HEADER_SIZE_BYTES + 10  # 10 for version
             ENTRY_SIZE = 4
             if self.tensor_meta.max_shape == self.tensor_meta.min_shape:
                 num_shape_entries = 1 * (len(self.tensor_meta.min_shape) + 1)
```

### Comparing `deeplake-3.5.4/deeplake/core/compression.py` & `deeplake-3.6.0/deeplake/core/compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/compute/process.py` & `deeplake-3.6.0/deeplake/core/compute/process.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/compute/provider.py` & `deeplake-3.6.0/deeplake/core/compute/provider.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/compute/ray.py` & `deeplake-3.6.0/deeplake/core/compute/ray.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/compute/serial.py` & `deeplake-3.6.0/deeplake/core/compute/serial.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/compute/thread.py` & `deeplake-3.6.0/deeplake/core/compute/thread.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/dataset/__init__.py` & `deeplake-3.6.0/deeplake/core/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/dataset/dataset.py` & `deeplake-3.6.0/deeplake/core/dataset/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 )
 from deeplake.util.invalid_view_op import invalid_view_op
 from deeplake.util.spinner import spinner
 from deeplake.util.iteration_warning import (
     suppress_iteration_warning,
     check_if_iteration,
 )
+from deeplake.util.tensor_db import parse_runtime_parameters
 from deeplake.api.info import load_info
 from deeplake.client.log import logger
 from deeplake.client.utils import get_user_name
 from deeplake.client.client import DeepLakeBackendClient
 from deeplake.constants import (
     FIRST_COMMIT_ID,
     DEFAULT_MEMORY_CACHE_SIZE,
@@ -48,14 +49,15 @@
 from deeplake.core.meta.dataset_meta import DatasetMeta
 from deeplake.core.storage import (
     LRUCache,
     S3Provider,
     GCSProvider,
     MemoryProvider,
     LocalProvider,
+    AzureProvider,
 )
 from deeplake.core.tensor import Tensor, create_tensor, delete_tensor
 from deeplake.core.version_control.commit_node import CommitNode  # type: ignore
 from deeplake.core.version_control.dataset_diff import load_dataset_diff
 from deeplake.htype import (
     HTYPE_CONFIGURATIONS,
     UNSPECIFIED,
@@ -134,15 +136,15 @@
 from deeplake.core.dataset.invalid_view import InvalidView
 from deeplake.hooks import dataset_read
 from itertools import chain
 import warnings
 import jwt
 
 
-_LOCKABLE_STORAGES = {S3Provider, GCSProvider, LocalProvider}
+_LOCKABLE_STORAGES = {S3Provider, GCSProvider, AzureProvider, LocalProvider}
 
 
 class Dataset:
     def __init__(
         self,
         storage: LRUCache,
         index: Optional[Index] = None,
@@ -2090,29 +2092,29 @@
         dataset_read(self)
         return ret
 
     def query(
         self,
         query_string: str,
         runtime: Optional[Dict] = None,
-        return_indices_and_scores: bool = False,
+        return_data: bool = False,
     ):
         """Returns a sliced :class:`~deeplake.core.dataset.Dataset` with given query results. To use this, install deeplake with ``pip install deeplake[enterprise]``.
 
         It allows to run SQL like queries on dataset and extract results. See supported keywords and the Tensor Query Language documentation
         :ref:`here <tql>`.
 
 
         Args:
             query_string (str): An SQL string adjusted with new functionalities to run on the given :class:`~deeplake.core.dataset.Dataset` object
-            runtime (Optional[Dict]): whether to run query on a remote engine
-            return_indices_and_scores (bool): by default False. Whether to return indices and scores.
+            runtime (Optional[Dict]): Runtime parameters for query execution. Supported keys: {"tensor_db": True or False}.
+            return_data (bool): Defaults to ``False``. Whether to return raw data along with the view.
 
         Raises:
-            ValueError: if return_indices_and_scores is True and runtime is not {"db_engine": true}
+            ValueError: if ``return_data`` is True and runtime is not {"tensor_db": true}
 
         Returns:
             Dataset: A :class:`~deeplake.core.dataset.Dataset` object.
 
         Examples:
 
             Query from dataset all the samples with lables other than ``5``
@@ -2123,36 +2125,44 @@
 
             Query from dataset first appeard ``1000`` samples where the ``categories`` is ``car`` and ``1000`` samples where the ``categories`` is ``motorcycle``
 
             >>> ds_train = deeplake.load('hub://activeloop/coco-train')
             >>> query_ds_train = ds_train.query("(select * where contains(categories, 'car') limit 1000) union (select * where contains(categories, 'motorcycle') limit 1000)")
 
         """
-        if runtime is not None and runtime.get("db_engine", False):
+
+        deeplake_reporter.feature_report(
+            feature_name="query",
+            parameters={
+                "query_string": query_string[0:100],
+                "runtime": runtime,
+            },
+        )
+
+        runtime = parse_runtime_parameters(self.path, runtime)
+        if runtime["tensor_db"]:
             client = DeepLakeBackendClient(token=self._token)
             org_id, ds_name = self.path[6:].split("/")
-            indices, scores = client.remote_query(org_id, ds_name, query_string)
-            if return_indices_and_scores:
-                return indices, scores
-            return self[indices]
+            response = client.remote_query(org_id, ds_name, query_string)
+            indices = response["indices"]
+            view = self[indices]
+
+            if return_data:
+                data = response["data"]
+                return view, data
 
-        if return_indices_and_scores:
+            return view
+
+        if return_data:
             raise ValueError(
-                "return_indices_and_scores is not supported. Please add `runtime = {'db_engine': True}` if you want to return indices and scores"
+                "`return_data` is only applicable when running queries using the Managed Tensor Database. Please specify `runtime = {'tensor_db': True}`"
             )
 
         from deeplake.enterprise import query
 
-        deeplake_reporter.feature_report(
-            feature_name="query",
-            parameters={
-                "query_string": query_string,
-            },
-        )
-
         return query(self, query_string)
 
     def sample_by(
         self,
         weights: Union[str, list, tuple],
         replace: Optional[bool] = True,
         size: Optional[int] = None,
@@ -3802,15 +3812,15 @@
             dest_path (str, optional): The full path to where the connected Deep Lake dataset will reside. Can be:
                 a Deep Lake path like ``hub://organization/dataset``
             org_id (str, optional): The organization to where the connected Deep Lake dataset will be added.
             ds_name (str, optional): The name of the connected Deep Lake dataset. Will be infered from ``dest_path`` or ``src_path`` if not provided.
             token (str, optional): Activeloop token used to fetch the managed credentials.
 
         Raises:
-            InvalidSourcePathError: If the dataset's path is not a valid s3 or gcs path.
+            InvalidSourcePathError: If the dataset's path is not a valid s3, gcs or azure path.
             InvalidDestinationPathError: If ``dest_path``, or ``org_id`` and ``ds_name`` do not form a valid Deep Lake path.
         """
         path = connect_dataset_entry(
             src_path=self.path,
             dest_path=dest_path,
             org_id=org_id,
             ds_name=ds_name,
```

### Comparing `deeplake-3.5.4/deeplake/core/dataset/deeplake_cloud_dataset.py` & `deeplake-3.6.0/deeplake/core/dataset/deeplake_cloud_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         """Get attached token of the dataset"""
         if self._token is None:
             self.__dict__["_token"] = self.client.get_token()
         return self._token
 
     def _set_org_and_name(self):
         if self.is_actually_cloud:
-            if self.org_id is not None:
+            if self.org_id is not None and self.ds_name is not None:
                 return
             _, org_id, ds_name, subdir = process_hub_path(self.path)
             if subdir:
                 ds_name += "/" + subdir
         else:
             # if this dataset isn't actually pointing to a datset in the cloud
             # a.k.a this dataset is trying to simulate a Deep Lake cloud dataset
```

### Comparing `deeplake-3.5.4/deeplake/core/dataset/deeplake_query_dataset.py` & `deeplake-3.6.0/deeplake/core/dataset/deeplake_query_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/dataset/deeplake_query_tensor.py` & `deeplake-3.6.0/deeplake/core/dataset/deeplake_query_tensor.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/dataset/invalid_view.py` & `deeplake-3.6.0/deeplake/core/dataset/invalid_view.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/dataset/view_entry.py` & `deeplake-3.6.0/deeplake/core/dataset/view_entry.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/fast_forwarding.py` & `deeplake-3.6.0/deeplake/core/fast_forwarding.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/index/index.py` & `deeplake-3.6.0/deeplake/core/index/index.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/io.py` & `deeplake-3.6.0/deeplake/core/io.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/ipc.py` & `deeplake-3.6.0/deeplake/core/ipc.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/link_creds.py` & `deeplake-3.6.0/deeplake/core/link_creds.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,26 +8,35 @@
 from deeplake.util.exceptions import (
     ManagedCredentialsNotFoundError,
     MissingCredsError,
     MissingManagedCredsError,
 )
 from deeplake.util.token import expires_in_to_expires_at, is_expired_token
 from deeplake.client.log import logger
+from datetime import datetime, timezone
+
+
+def _is_expired_creds(creds: dict) -> bool:
+    if "expiration" not in creds:
+        return False
+
+    return creds["expiration"] < datetime.now(timezone.utc).timestamp()
 
 
 class LinkCreds(DeepLakeMemoryObject):
     def __init__(self):
         self.creds_keys = []
         self.creds_dict = {}  # keys to actual creds dictionary
         self.creds_mapping = {}  # keys to numbers, for encoding
         self.managed_creds_keys = set()  # keys which are managed
         self.used_creds_keys = set()  # keys which are used by one or more samples
         self.storage_providers = {}
         self.default_s3_provider = None
         self.default_gcs_provider = None
+        self.default_azure_provider = None
         self.client = None
         self.org_id = None
 
     def get_creds(self, key: Optional[str]):
         if key is None:
             return {}
         if key not in self.creds_keys:
@@ -40,15 +49,18 @@
             else:
                 raise MissingManagedCredsError(
                     f"Managed creds key {key} hasn't been fetched."
                 )
         if (
             self.client is not None
             and key in self.managed_creds_keys
-            and is_expired_token(self.creds_dict[key])
+            and (
+                is_expired_token(self.creds_dict[key])
+                or _is_expired_creds(self.creds_dict[key])
+            )
         ):
             self.refresh_managed_creds(key)  # type: ignore
         return self.creds_dict[key]
 
     def refresh_managed_creds(self, creds_key: str):
         if creds_key not in self.managed_creds_keys:
             return False
@@ -59,47 +71,66 @@
     def get_default_provider(self, provider_type: str):
         if provider_type == "s3":
             if self.default_s3_provider is None:
                 self.default_s3_provider = storage_factory(
                     S3Provider, "s3://bucket/path"
                 )
             return self.default_s3_provider
-        else:
+        elif provider_type == "gcs":
             if self.default_gcs_provider is None:
                 from deeplake.core.storage.gcs import GCSProvider
 
                 self.default_gcs_provider = storage_factory(
                     GCSProvider, "gcs://bucket/path"
                 )
             return self.default_gcs_provider
+        elif provider_type == "azure":
+            if self.default_azure_provider is None:
+                from deeplake.core.storage.azure import AzureProvider
+
+                self.default_azure_provider = storage_factory(
+                    AzureProvider, "az://account/container"
+                )
+            return self.default_azure_provider
 
     def get_storage_provider(self, key: Optional[str], provider_type: str):
-        assert provider_type in {"s3", "gcs"}
+        assert provider_type in {"s3", "gcs", "azure"}
         if key is None:
             return self.get_default_provider(provider_type)
 
         provider: StorageProvider
         creds = self.get_creds(key)
 
         if provider_type == "s3":
             if key in self.storage_providers:
                 provider = self.storage_providers[key]
                 if isinstance(provider, S3Provider):
                     return provider
 
             provider = storage_factory(S3Provider, "s3://bucket/path", **creds)
-        else:
+        elif provider_type == "gcs":
             from deeplake.core.storage.gcs import GCSProvider
 
             if key in self.storage_providers:
                 provider = self.storage_providers[key]
                 if isinstance(provider, GCSProvider):
                     return provider
 
             provider = storage_factory(GCSProvider, "gcs://bucket/path", **creds)
+        elif provider_type == "azure":
+            from deeplake.core.storage.azure import AzureProvider
+
+            if key in self.storage_providers:
+                provider = self.storage_providers[key]
+                if isinstance(provider, AzureProvider):
+                    return provider
+
+            provider = storage_factory(
+                AzureProvider, "az://account/container", creds=creds
+            )
         self.storage_providers[key] = provider
         return provider
 
     def add_creds_key(self, creds_key: str, managed: bool = False):
         if creds_key in self.creds_keys:
             raise ValueError(f"Creds key {creds_key} already exists")
         if managed:
```

### Comparing `deeplake-3.5.4/deeplake/core/linked_chunk_engine.py` & `deeplake-3.6.0/deeplake/core/linked_chunk_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     BadLinkError,
     GetDataFromLinkError,
     ReadOnlyModeError,
 )
 from deeplake.util.keys import get_creds_encoder_key
 from deeplake.util.link import get_path_creds_key, save_link_creds
 from deeplake.util.video import normalize_index
+from deeplake.util.path import get_path_type
 import numpy as np
 from typing import Optional, Dict, Any, Tuple, Union
 from PIL import Image  # type: ignore
 from deeplake.core.linked_tiled_sample import LinkedTiledSample
 from math import ceil
 
 
@@ -118,16 +119,16 @@
         )
         return self.link_creds.get_creds_key(sample_creds_encoded)  # type: ignore
 
     def get_video_url(self, global_sample_index):
         sample_path = self.get_path(global_sample_index)
         sample_creds_key = self.creds_key(global_sample_index)
         storage = None
-        if sample_path.startswith(("gcs://", "gcp://", "s3://")):
-            provider_type = "s3" if sample_path.startswith("s3://") else "gcs"
+        if sample_path.startswith(("gcs://", "gcp://", "s3://", "az://", "azure://")):
+            provider_type = get_path_type(sample_path)
             storage = self.link_creds.get_storage_provider(
                 sample_creds_key, provider_type
             )
             url = storage.get_presigned_url(sample_path, full=True)
         else:
             url = sample_path
         return url, sample_path
```

### Comparing `deeplake-3.5.4/deeplake/core/linked_sample.py` & `deeplake-3.6.0/deeplake/core/linked_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/linked_tiled_sample.py` & `deeplake-3.6.0/deeplake/core/linked_tiled_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/lock.py` & `deeplake-3.6.0/deeplake/core/lock.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/meta/dataset_meta.py` & `deeplake-3.6.0/deeplake/core/meta/dataset_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/meta/encode/base_encoder.py` & `deeplake-3.6.0/deeplake/core/meta/encode/base_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/meta/encode/byte_positions.py` & `deeplake-3.6.0/deeplake/core/meta/encode/byte_positions.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/meta/encode/chunk_id.py` & `deeplake-3.6.0/deeplake/core/meta/encode/chunk_id.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/meta/encode/creds.py` & `deeplake-3.6.0/deeplake/core/meta/encode/creds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/meta/encode/pad.py` & `deeplake-3.6.0/deeplake/core/meta/encode/pad.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/meta/encode/sequence.py` & `deeplake-3.6.0/deeplake/core/meta/encode/sequence.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/meta/encode/shape.py` & `deeplake-3.6.0/deeplake/core/meta/encode/shape.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py` & `deeplake-3.6.0/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py` & `deeplake-3.6.0/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py` & `deeplake-3.6.0/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/meta/encode/tests/test_shape_encoder.py` & `deeplake-3.6.0/deeplake/core/meta/encode/tests/test_shape_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py` & `deeplake-3.6.0/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/meta/encode/tile.py` & `deeplake-3.6.0/deeplake/core/meta/encode/tile.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/meta/tensor_meta.py` & `deeplake-3.6.0/deeplake/core/meta/tensor_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/partial_reader.py` & `deeplake-3.6.0/deeplake/core/partial_reader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/partial_sample.py` & `deeplake-3.6.0/deeplake/core/partial_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/polygon.py` & `deeplake-3.6.0/deeplake/core/polygon.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/query/autocomplete.py` & `deeplake-3.6.0/deeplake/core/query/autocomplete.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/query/filter.py` & `deeplake-3.6.0/deeplake/core/query/filter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/query/query.py` & `deeplake-3.6.0/deeplake/core/query/query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/sample.py` & `deeplake-3.6.0/deeplake/core/sample.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,26 +18,28 @@
     VIDEO_COMPRESSION,
     POINT_CLOUD_COMPRESSION,
     MESH_COMPRESSION,
     NIFTI_COMPRESSION,
 )
 from deeplake.util.exceptions import SampleReadError, UnableToReadFromUrlError
 from deeplake.util.exif import getexif
-from deeplake.core.storage.provider import StorageProvider
 from deeplake.util.path import get_path_type, is_remote_path
 import numpy as np
 from typing import Optional, Tuple, Union, Dict
 
 from PIL import Image  # type: ignore
 from PIL.ExifTags import TAGS  # type: ignore
 from io import BytesIO
 
+from deeplake.core.storage.provider import StorageProvider
 from deeplake.core.storage.s3 import S3Provider
-from deeplake.core.storage import storage_factory
+from deeplake.core.storage.gcs import GCSProvider
+from deeplake.core.storage.azure import AzureProvider
 from deeplake.core.storage.google_drive import GDriveProvider
+from deeplake.core.storage import storage_factory
 
 try:
     from deeplake.core.storage.gcs import GCSProvider
 except ImportError:
     GCSProvider = None  # type: ignore
 
 import warnings
@@ -436,14 +438,16 @@
             try:
                 if path_type == "local":
                     self._buffer = self._read_from_local()
                 elif path_type == "gcs":
                     self._buffer = self._read_from_gcs()
                 elif path_type == "s3":
                     self._buffer = self._read_from_s3()
+                elif path_type == "azure":
+                    self._buffer = self._read_from_azure()
                 elif path_type == "gdrive":
                     self._buffer = self._read_from_gdrive()
                 elif path_type == "http":
                     self._buffer = self._read_from_http()
             except Exception as e:
                 raise SampleReadError(self.path) from e  # type: ignore
         return self._buffer  # type: ignore
@@ -480,14 +484,24 @@
             assert isinstance(self.storage, GCSProvider)
             return self.storage.get_object_from_full_url(self.path)
         path = self.path.replace("gcp://", "").replace("gcs://", "")  # type: ignore
         root, key = self._get_root_and_key(path)
         gcs = storage_factory(GCSProvider, root, token=self._creds)
         return gcs[key]
 
+    def _read_from_azure(self) -> bytes:
+        assert self.path is not None
+        if self.storage is not None:
+            assert isinstance(self.storage, AzureProvider)
+            return self.storage.get_object_from_full_url(self.path)
+        path = self.path.replace("az://", "").replace("azure://", "")  # type: ignore
+        root, key = self._get_root_and_key(path)
+        azure = storage_factory(AzureProvider, root, creds=self._creds)
+        return azure[key]
+
     def _read_from_gdrive(self) -> bytes:
         assert self.path is not None
         gdrive = storage_factory(
             GDriveProvider, "gdrive://", token=self._creds, makemap=False
         )
         return gdrive.get_object_from_full_url(self.path)  # type: ignore
```

### Comparing `deeplake-3.5.4/deeplake/core/serialize.py` & `deeplake-3.6.0/deeplake/core/serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/storage/deeplake_memory_object.py` & `deeplake-3.6.0/deeplake/core/storage/deeplake_memory_object.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/storage/gcs.py` & `deeplake-3.6.0/deeplake/core/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/storage/google_drive.py` & `deeplake-3.6.0/deeplake/core/storage/google_drive.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/storage/local.py` & `deeplake-3.6.0/deeplake/core/storage/local.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/storage/lru_cache.py` & `deeplake-3.6.0/deeplake/core/storage/lru_cache.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/storage/memory.py` & `deeplake-3.6.0/deeplake/core/storage/memory.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/storage/provider.py` & `deeplake-3.6.0/deeplake/core/storage/provider.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/storage/s3.py` & `deeplake-3.6.0/deeplake/core/storage/s3.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,15 @@
         aws_access_key_id: Optional[str] = None,
         aws_secret_access_key: Optional[str] = None,
         aws_session_token: Optional[str] = None,
         endpoint_url: Optional[str] = None,
         aws_region: Optional[str] = None,
         profile_name: Optional[str] = None,
         token: Optional[str] = None,
+        **kwargs,
     ):
         """Initializes the S3Provider
 
         Example:
 
             >>> s3_provider = S3Provider("snark-test/benchmarks")
 
@@ -104,14 +105,15 @@
                 authenticate the user.
             endpoint_url (str, optional): The complete URL to use for the constructed client.
                 This needs to be provided for cases in which you're interacting with MinIO, Wasabi, etc.
             aws_region (str, optional): Specifies the AWS Region to send requests to.
             profile_name (str, optional): Specifies the AWS profile name to use.
             token (str, optional): Activeloop token, used for fetching credentials for Deep Lake datasets (if this is underlying storage for Deep Lake dataset).
                 This is optional, tokens are normally autogenerated.
+            **kwargs: Additional arguments to pass to the S3 client. Includes: ``expiration``.
         """
         self.root = root
         self.aws_access_key_id = aws_access_key_id
         self.aws_secret_access_key = aws_secret_access_key
         self.aws_session_token = aws_session_token
         self.aws_region: Optional[str] = aws_region
         self.endpoint_url: Optional[str] = endpoint_url
```

### Comparing `deeplake-3.5.4/deeplake/core/tensor.py` & `deeplake-3.6.0/deeplake/core/tensor.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/tensor_link.py` & `deeplake-3.6.0/deeplake/core/tensor_link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/test_serialize.py` & `deeplake-3.6.0/deeplake/core/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/tests/test_compression.py` & `deeplake-3.6.0/deeplake/core/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/tests/test_compute.py` & `deeplake-3.6.0/deeplake/core/tests/test_compute.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/tests/test_deeplake_indra_dataset.py` & `deeplake-3.6.0/deeplake/core/tests/test_deeplake_indra_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 import deeplake
 import numpy as np
 from deeplake.tests.common import requires_libdeeplake
-from deeplake.util.exceptions import DynamicTensorNumpyError
+from deeplake.util.exceptions import (
+    DynamicTensorNumpyError,
+    EmptyTokenException,
+)
+
+
 from deeplake.core.dataset.deeplake_query_dataset import DeepLakeQueryDataset
 import random
 import pytest
 
 
 @requires_libdeeplake
 def test_indexing(local_ds_generator):
@@ -70,14 +75,27 @@
     assert (
         deeplake_indra_ds.base_storage["queries.json"]
         == deeplake_ds.base_storage["queries.json"]
     )
 
 
 @requires_libdeeplake
+def test_empty_token_exception(local_ds):
+    from deeplake.enterprise.convert_to_libdeeplake import dataset_to_libdeeplake
+
+    with local_ds:
+        local_ds.create_tensor("label", htype="generic", dtype=np.int32)
+
+    loaded = deeplake.load(local_ds.path, token="")
+
+    with pytest.raises(EmptyTokenException):
+        dss = dataset_to_libdeeplake(loaded)
+
+
+@requires_libdeeplake
 def test_load_view(local_ds_generator):
     from deeplake.enterprise.convert_to_libdeeplake import dataset_to_libdeeplake
 
     deeplake_ds = local_ds_generator()
     with deeplake_ds:
         deeplake_ds.create_tensor("label", htype="generic", dtype=np.int32)
         deeplake_ds.create_tensor(
```

### Comparing `deeplake-3.5.4/deeplake/core/tests/test_io.py` & `deeplake-3.6.0/deeplake/core/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/tests/test_locking.py` & `deeplake-3.6.0/deeplake/core/tests/test_locking.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import time
 import warnings
 import json
 from deeplake.tests.dataset_fixtures import (
     enabled_persistent_non_gdrive_dataset_generators,
 )
 from concurrent.futures import ThreadPoolExecutor
+from deeplake.tests.common import requires_non_python11
 import deeplake
 
 _counter = 0
 
 
 class VM(object):
     """
@@ -32,14 +33,15 @@
         deeplake.core.lock._LOCKS.clear()
 
     def __exit__(self, *args, **kwargs):
         uuid.getnode = self._getnode
         deeplake.core.lock._LOCKS.update(self._locks)
 
 
+@requires_non_python11
 @enabled_persistent_non_gdrive_dataset_generators
 def test_dataset_locking(ds_generator):
     deeplake.constants.LOCK_LOCAL_DATASETS = True
     try:
         ds = ds_generator()
         ds.create_tensor("x")
         arr = np.random.random((32, 32))
@@ -61,14 +63,15 @@
                 ds = ds_generator(read_only=True)
                 np.testing.assert_array_equal(arr, ds.x[0].numpy())
             assert not ws
     finally:
         deeplake.constants.LOCK_LOCAL_DATASETS = False
 
 
+@requires_non_python11
 @enabled_persistent_non_gdrive_dataset_generators
 def test_vc_locking(ds_generator):
     deeplake.constants.LOCK_LOCAL_DATASETS = True
     try:
         ds = ds_generator()
         ds.create_tensor("x")
         arr = np.random.random((32, 32))
@@ -80,14 +83,15 @@
                 ds = ds_generator()
             np.testing.assert_array_equal(arr, ds.x[0].numpy())
             assert not ws, str(ws[0])
     finally:
         deeplake.constants.LOCK_LOCAL_DATASETS = False
 
 
+@requires_non_python11
 def test_lock_thread_leaking(s3_ds_generator):
     locks = deeplake.core.lock._LOCKS
     refs = deeplake.core.lock._REFS
     nlocks_previous = len(locks)
 
     def nlocks():
         assert len(locks) == len(refs)
@@ -119,14 +123,15 @@
 
     for i in range(len(views)):
         views[i].__del__()
     del views
     assert nlocks() == 0  # 0 because dataset and all views deleted
 
 
+@requires_non_python11
 def test_concurrent_locking(memory_ds):
     storage = memory_ds.base_storage
 
     def f(i):
         lock = deeplake.core.lock.Lock(storage, "lock.lock")
         with lock:
             byts = storage.get("meta.json")
```

### Comparing `deeplake-3.5.4/deeplake/core/tests/test_readonly.py` & `deeplake-3.6.0/deeplake/core/tests/test_readonly.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/tests/test_serialize.py` & `deeplake-3.6.0/deeplake/core/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/tiling/deserialize.py` & `deeplake-3.6.0/deeplake/core/tiling/deserialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/tiling/optimizer.py` & `deeplake-3.6.0/deeplake/core/tiling/optimizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/tiling/sample_tiles.py` & `deeplake-3.6.0/deeplake/core/tiling/sample_tiles.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/tiling/serialize.py` & `deeplake-3.6.0/deeplake/core/tiling/serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/tiling/test_optimizer.py` & `deeplake-3.6.0/deeplake/core/tiling/test_optimizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/tiling/test_serialize.py` & `deeplake-3.6.0/deeplake/core/tiling/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/transform/test_transform.py` & `deeplake-3.6.0/deeplake/core/transform/test_transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -1372,27 +1372,27 @@
 
 class BadSample:
     # will pass shape check in transform tensor
     shape = (250, 250, 3)
 
 
 @all_schedulers
-@pytest.mark.parametrize("method", ["ds", "multiple"])
+@pytest.mark.parametrize("method", ["ds", "multiple", "checkpointed"])
 @pytest.mark.parametrize("error_at", ["transform", "chunk_engine"])
 def test_ds_append_errors(
     local_path, compressed_image_paths, scheduler, method, error_at
 ):
     @deeplake.compute
     def upload(item, ds):
         images = (
             deeplake.read(item["images"])
             if isinstance(item["images"], str)
             else item["images"]
         )
-        if method == "ds":
+        if method == "ds" or method == "checkpointed":
             ds.append(
                 {
                     "labels": np.zeros(10, dtype=np.uint32),
                     "boxes": np.ones((len(item["boxes"]), 4), dtype=np.float32),
                     "images": images,
                 }
             )
@@ -1413,44 +1413,50 @@
     for i in range(20):
         samples.append({"images": images[i % 2], "boxes": range(i + 1)})
 
     if error_at == "transform":
         # errors out in transform dataset / tensor
         bad_sample = {"images": "bad_path", "boxes": [1, 2, 3]}
         err_msg = re.escape(
-            f"Transform failed at index 17 of the input data on the item: {bad_sample}. See traceback for more details."
+            f"Transform failed at index 17 of the input data on the item: {bad_sample}."
         )
     else:
         # errors out in chunk engine
         bad_sample = {"images": BadSample(), "boxes": [1, 2, 3]}
-        err_msg = re.escape(
-            f"Transform failed at index 17 of the input data. See traceback for more details."
+        err_msg = re.escape(f"Transform failed at index 17 of the input data.")
+
+    if method == "checkpointed":
+        err_msg += re.escape(
+            " Last checkpoint: 10 samples processed. You can slice the input to resume from this point."
         )
+    err_msg += re.escape(" See traceback for more details.")
 
     samples.insert(17, bad_sample)
 
     with pytest.raises(TransformError, match=err_msg) as e:
         upload().eval(
             samples,
             ds,
             num_workers=TRANSFORM_TEST_NUM_WORKERS,
             scheduler=scheduler,
+            checkpoint_interval=10 if method == "checkpointed" else 0,
         )
 
     ds = create_test_ds(local_path)
 
     upload().eval(
         samples,
         ds,
         num_workers=TRANSFORM_TEST_NUM_WORKERS,
         scheduler=scheduler,
         ignore_errors=True,
+        checkpoint_interval=10 if method == "checkpointed" else 0,
     )
 
-    if method == "ds":
+    if method == "ds" or method == "checkpointed":
         assert ds["images"][::2].numpy().shape == (10, *deeplake.read(images[0]).shape)
         assert ds["images"][1::2].numpy().shape == (10, *deeplake.read(images[1]).shape)
 
         assert len(ds["boxes"]) == 20
         assert ds["boxes"].meta.min_shape == [1, 4]
         assert ds["boxes"].meta.max_shape == [20, 4]
```

### Comparing `deeplake-3.5.4/deeplake/core/transform/transform.py` & `deeplake-3.6.0/deeplake/core/transform/transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,14 +136,15 @@
         skip_ok: bool = False,
         check_lengths: bool = True,
         pad_data_in: bool = False,
         read_only_ok: bool = False,
         cache_size: int = DEFAULT_TRANSFORM_SAMPLE_CACHE_SIZE,
         checkpoint_interval: int = 0,
         ignore_errors: bool = False,
+        verbose: bool = True,
         **kwargs,
     ):
         """Evaluates the pipeline on ``data_in`` to produce an output dataset ``ds_out``.
 
         Args:
             data_in: Input passed to the transform to generate output dataset. Should support \__getitem__ and \__len__. Can be a Deep Lake dataset.
             ds_out (Dataset, optional): - The dataset object to which the transform will get written. If this is not provided, ``data_in`` will be overwritten if it is a Deep Lake dataset, otherwise error will be raised.
@@ -161,14 +162,15 @@
                 Defaults to ``False``.
             read_only_ok (bool): If ``True`` and output dataset is same as input dataset, the read-only check is skipped.
                 Defaults to False.
             cache_size (int): Cache size to be used by transform per worker.
             checkpoint_interval (int): If > 0, the transform will be checkpointed with a commit every ``checkpoint_interval`` input samples to avoid restarting full transform due to intermitten failures. If the transform is interrupted, the intermediate data is deleted and the dataset is reset to the last commit.
                 If <= 0, no checkpointing is done. Checkpoint interval should be a multiple of num_workers if num_workers > 0. Defaults to 0.
             ignore_errors (bool): If ``True``, input samples that causes transform to fail will be skipped and the errors will be ignored **if possible**.
+            verbose (bool): If ``True``, prints additional information about the transform.
             **kwargs: Additional arguments.
 
         Raises:
             InvalidInputDataError: If ``data_in`` passed to transform is invalid. It should support \__getitem__ and \__len__ operations. Using scheduler other than "threaded" with deeplake dataset having base storage as memory as ``data_in`` will also raise this.
             InvalidOutputDatasetError: If all the tensors of ``ds_out`` passed to transform don't have the same length. Using scheduler other than "threaded" with deeplake dataset having base storage as memory as ``ds_out`` will also raise this.
             TensorMismatchError: If one or more of the outputs generated during transform contain different tensors than the ones present in 'ds_out' provided to transform.
             UnsupportedSchedulerError: If the scheduler passed is not recognized. Supported values include: 'serial', 'threaded', 'processed' and 'ray'.
@@ -230,15 +232,19 @@
         if not check_lengths or read_only_ok:
             skip_ok = True
 
         checkpointing_enabled = checkpoint_interval > 0
         total_samples = len(data_in)
         if checkpointing_enabled:
             check_checkpoint_interval(
-                data_in, checkpoint_interval, num_workers, overwrite
+                data_in,
+                checkpoint_interval,
+                num_workers,
+                overwrite,
+                verbose,
             )
             datas_in = [
                 data_in[i : i + checkpoint_interval]
                 for i in range(0, len(data_in), checkpoint_interval)
             ]
 
         else:
@@ -296,14 +302,16 @@
                     )
                     target_ds.reset(force=True)
                 target_ds._send_compute_progress(**progress_args, status="failed")
                 close_states(compute_provider, pbar, pqueue)
                 index, sample = None, None
                 if isinstance(e, TransformError):
                     index, sample = e.index, e.sample
+                    if checkpointing_enabled and isinstance(index, int):
+                        index = samples_processed + index
                     e = e.__cause__  # type: ignore
                 if isinstance(e, AllSamplesSkippedError):
                     raise e
                 raise TransformError(
                     index=index,
                     sample=sample,
                     samples_processed=samples_processed,
```

### Comparing `deeplake-3.5.4/deeplake/core/transform/transform_dataset.py` & `deeplake-3.6.0/deeplake/core/transform/transform_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/transform/transform_tensor.py` & `deeplake-3.6.0/deeplake/core/transform/transform_tensor.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/vectorstore/vector_search/dataset/dataset.py` & `deeplake-3.6.0/deeplake/core/vectorstore/vector_search/dataset/dataset.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,262 +1,379 @@
-import deeplake
-from deeplake.constants import MB
-from deeplake.enterprise.util import raise_indra_installation_error
-from deeplake.core.vectorstore.vector_search import utils
-from deeplake.core import tensor as tensor_utils
+import uuid
+from typing import List, Dict, Any
+
+import numpy as np
 
 try:
     from indra import api  # type: ignore
 
     _INDRA_INSTALLED = True  # pragma: no cover
 except ImportError:  # pragma: no cover
     _INDRA_INSTALLED = False  # pragma: no cover
 
-import numpy as np
-
-import uuid
-from typing import Iterable, List, Union, Optional
-
-from deeplake.constants import DEFAULT_VECTORSTORE_DEEPLAKE_PATH
+import deeplake
+from deeplake.constants import MB
+from deeplake.core.vectorstore.vector_search import utils
+from deeplake.core.vectorstore.vector_search import dataset as dataset_utils
+from deeplake.core.vectorstore.vector_search.ingestion import ingest_data
+from deeplake.constants import (
+    DEFAULT_VECTORSTORE_DEEPLAKE_PATH,
+    VECTORSTORE_EXTEND_MAX_SIZE,
+    DEFAULT_VECTORSTORE_TENSORS,
+)
 from deeplake.util.warnings import always_warn
 
 
 def create_or_load_dataset(
-    dataset_path, token, creds, logger, read_only, exec_option, **kwargs
+    tensor_params,
+    dataset_path,
+    token,
+    creds,
+    logger,
+    read_only,
+    exec_option,
+    embedding_function,
+    overwrite,
+    **kwargs,
 ):
     utils.check_indra_installation(
         exec_option=exec_option, indra_installed=_INDRA_INSTALLED
     )
 
-    if "overwrite" in kwargs and kwargs["overwrite"] == False:
-        del kwargs["overwrite"]
+    if not overwrite and dataset_exists(dataset_path, token, creds, **kwargs):
+        if tensor_params is not None and tensor_params != DEFAULT_VECTORSTORE_TENSORS:
+            raise ValueError(
+                "Vector Store is not empty. You shouldn't specify tensor_params if you're loading from existing dataset."
+            )
 
-    if dataset_exists(dataset_path, token, creds, **kwargs):
-        return load_dataset(dataset_path, token, creds, logger, read_only, **kwargs)
+        return load_dataset(
+            dataset_path,
+            token,
+            creds,
+            logger,
+            read_only,
+            **kwargs,
+        )
 
-    return create_dataset(dataset_path, token, exec_option, **kwargs)
+    return create_dataset(
+        logger,
+        tensor_params,
+        dataset_path,
+        token,
+        exec_option,
+        embedding_function,
+        overwrite,
+        **kwargs,
+    )
 
 
 def dataset_exists(dataset_path, token, creds, **kwargs):
     return (
         deeplake.exists(dataset_path, token=token, **creds)
         and "overwrite" not in kwargs
     )
 
 
-def load_dataset(dataset_path, token, creds, logger, read_only, **kwargs):
+def load_dataset(
+    dataset_path,
+    token,
+    creds,
+    logger,
+    read_only,
+    **kwargs,
+):
     if dataset_path == DEFAULT_VECTORSTORE_DEEPLAKE_PATH:
         logger.warning(
             f"The default deeplake path location is used: {DEFAULT_VECTORSTORE_DEEPLAKE_PATH}"
             " and it is not free. All addtionally added data will be added on"
             " top of already existing deeplake dataset."
         )
 
     dataset = deeplake.load(
-        dataset_path, token=token, read_only=read_only, creds=creds, **kwargs
+        dataset_path,
+        token=token,
+        read_only=read_only,
+        creds=creds,
+        verbose=False,
+        **kwargs,
     )
-    create_tensors_if_needed(dataset, logger)
+
+    check_tensors(dataset)
 
     logger.warning(
         f"Deep Lake Dataset in {dataset_path} already exists, "
         f"loading from the storage"
     )
     return dataset
 
 
-def create_tensors_if_needed(dataset, logger):
+def check_tensors(dataset):
     tensors = dataset.tensors
 
-    if "text" not in tensors:
-        warn_and_create_missing_tensor(
-            logger=logger,
-            dataset=dataset,
-            tensor_name="text",
-            htype="text",
-            create_id_tensor=False,
-            create_sample_info_tensor=False,
-            create_shape_tensor=False,
-            chunk_compression="lz4",
-        )
-
-    if "metadata" not in tensors:
-        warn_and_create_missing_tensor(
-            logger=logger,
-            dataset=dataset,
-            tensor_name="metadata",
-            htype="json",
-            create_id_tensor=False,
-            create_sample_info_tensor=False,
-            create_shape_tensor=False,
-            chunk_compression="lz4",
-        )
+    embedding_tensor_exist = False
+    ids_exist = False
 
-    if "embedding" not in tensors:
-        warn_and_create_missing_tensor(
-            logger=logger,
-            dataset=dataset,
-            tensor_name="embedding",
-            htype="embedding",
-            dtype=np.float32,
-            create_id_tensor=False,
-            create_sample_info_tensor=False,
-            max_chunk_size=64 * MB,
-            create_shape_tensor=True,
-        )
+    for tensor in tensors:
+        htype = dataset[tensor].htype
 
-    if "ids" not in tensors:
-        warn_and_create_missing_tensor(
-            logger=logger,
-            dataset=dataset,
-            tensor_name="ids",
-            htype="text",
-            create_id_tensor=False,
-            create_sample_info_tensor=False,
-            create_shape_tensor=False,
-            chunk_compression="lz4",
-        )
+        if tensor in ("id", "ids"):
+            ids_exist = True
 
+        if tensor in ("embedding", "embeddings"):
+            embedding_tensor_exist = True
+
+            # TODO: Add back once old datasets without embedding htype are not in circulation
+            # if htype not in (None, "embedding"):
+            #     raise ValueError(
+            #         f"`{htype}` is not supported htype for embedding tensor. "
+            #         "Supported htype for embedding tensor is: `embedding`"
+            #     )
+
+        if htype == "embedding":
+            if tensor in ("id", "ids"):
+                raise ValueError(
+                    f"`{tensor}` is not valid name for embedding tensor, as the name is preserved for another tensor"
+                )
+
+            embedding_tensor_exist = True
+
+    if not embedding_tensor_exist:
+        raise ValueError("At least one embedding tensor should exist.")
+
+    if not ids_exist:
+        raise ValueError("`id` tensor was not found in the dataset.")
+
+
+def create_dataset(
+    logger,
+    tensor_params,
+    dataset_path,
+    token,
+    exec_option,
+    embedding_function,
+    overwrite,
+    **kwargs,
+):
+    runtime = None
+    if exec_option == "tensor_db":
+        runtime = {"tensor_db": True}
 
-def warn_and_create_missing_tensor(dataset, tensor_name, logger, **kwargs):
-    logger.warning(
-        f"`{tensor_name}` tensor does not exist in the dataset. If you created dataset manually "
-        "and stored text data in another tensor, consider copying the contents of that "
-        f"tensor into `{tensor_name}` tensor and deleting if afterwards. To view dataset content "
-        "run ds.summary()"
-    )
-    dataset.create_tensor(
-        tensor_name,
+    dataset = deeplake.empty(
+        dataset_path,
+        token=token,
+        runtime=runtime,
+        verbose=False,
+        overwrite=overwrite,
         **kwargs,
     )
+    create_tensors(tensor_params, dataset, logger, embedding_function)
 
+    return dataset
 
-def create_dataset(dataset_path, token, exec_option, **kwargs):
-    runtime = None
-    if exec_option == "tensor_db":
-        runtime = {"tensor_db": True}
 
-    dataset = deeplake.empty(dataset_path, token=token, runtime=runtime, **kwargs)
+def create_tensors(tensor_params, dataset, logger, embedding_function):
+    tensor_names = [tensor["name"] for tensor in tensor_params]
+    if "id" not in tensor_names and "ids" not in tensor_names:
+        tensor_params.append(
+            {
+                "name": "id",
+                "htype": "text",
+                "create_id_tensor": False,
+                "create_sample_info_tensor": False,
+                "create_shape_tensor": False,
+                "chunk_compression": "lz4",
+            },
+        )
 
     with dataset:
-        dataset.create_tensor(
-            "text",
-            htype="text",
-            create_id_tensor=False,
-            create_sample_info_tensor=False,
-            create_shape_tensor=False,
-            chunk_compression="lz4",
-        )
-        dataset.create_tensor(
-            "metadata",
-            htype="json",
-            create_id_tensor=False,
-            create_sample_info_tensor=False,
-            create_shape_tensor=False,
-            chunk_compression="lz4",
-        )
-        dataset.create_tensor(
-            "embedding",
-            htype="embedding",
-            dtype=np.float32,
-            create_id_tensor=False,
-            create_sample_info_tensor=False,
-            max_chunk_size=64 * MB,
-            create_shape_tensor=True,
-        )
-        dataset.create_tensor(
-            "ids",
-            htype="text",
-            create_id_tensor=False,
-            create_sample_info_tensor=False,
-            create_shape_tensor=False,
-            chunk_compression="lz4",
-        )
-    return dataset
+        for tensor_args in tensor_params:
+            dataset.create_tensor(**tensor_args)
+
+        update_embedding_info(logger, dataset, embedding_function)
 
 
 def delete_and_commit(dataset, ids):
     with dataset:
         for id in sorted(ids)[::-1]:
             dataset.pop(id)
         dataset.commit(f"deleted {len(ids)} samples", allow_empty=True)
 
 
 def delete_all_samples_if_specified(dataset, delete_all):
     if delete_all:
-        dataset = deeplake.empty(dataset.path, overwrite=True)
+        dataset = deeplake.like(
+            dataset.path,
+            dataset,
+            overwrite=True,
+            verbose=False,
+        )
+
         return dataset, True
     return dataset, False
 
 
-def fetch_embeddings(exec_option, view, logger):
-    if exec_option == "python":
-        logger.warning(
-            "Python implementation fetches all of the dataset's embedding into memory. "
-            "With big datasets this could be quite slow and potentially result in performance issues. "
-            "Use `exec_option = 'tensor_db'` for better performance."
-        )
-        embeddings = view.embedding.numpy()
-    elif exec_option in ("compute_engine", "tensor_db"):
-        embeddings = None
-    return embeddings
+def fetch_embeddings(view, embedding_tensor: str = "embedding"):
+    return view[embedding_tensor].numpy()
 
 
-def get_embedding(embedding, query, embedding_function=None):
-    if embedding is None:
-        if embedding_function is None:
-            raise Exception(
-                "Either embedding array or embedding_function should be specified!"
-            )
-
-    if embedding_function is not None:
-        if embedding is not None:
-            always_warn("both embedding and embedding_function are specified. ")
-        embedding = embedding_function(query)  # type: ignore
+def get_embedding(embedding, embedding_data, embedding_function=None):
+    if embedding is not None and embedding_function:
+        always_warn(
+            "Both embedding data and embedding function were specified."
+            " Already computed `embedding` will be used."
+        )
+    if embedding is None and embedding_function is not None:
+        embedding = embedding_function(embedding_data)  # type: ignore
 
-    if isinstance(embedding, list) or embedding.dtype != "float32":
+    if embedding is not None and (
+        isinstance(embedding, list) or embedding.dtype != "float32"
+    ):
         embedding = np.array(embedding, dtype=np.float32)
 
     return embedding
 
 
-def preprocess_tensors(ids, texts, metadatas, embeddings):
-    if ids is None:
-        ids = [str(uuid.uuid1()) for _ in texts]
+def preprocess_tensors(
+    embedding_data=None, embedding_tensor=None, dataset=None, **tensors
+):
+    first_item = next(iter(tensors))
+    ids_tensor = "ids" if "ids" in tensors else "id"
+    if ids_tensor not in tensors or ids_tensor is None:
+        id = [str(uuid.uuid1()) for _ in tensors[first_item]]
+        tensors[ids_tensor] = id
+
+    processed_tensors = {ids_tensor: tensors[ids_tensor]}
+
+    for tensor_name, tensor_data in tensors.items():
+        if not isinstance(tensor_data, list):
+            tensor_data = list(tensor_data)
+        if dataset and dataset[tensor_name].htype == "image":
+            tensor_data = [
+                deeplake.read(data) if isinstance(data, str) else data
+                for data in tensor_data
+            ]
+        processed_tensors[tensor_name] = tensor_data
+
+    if embedding_data:
+        processed_tensors[embedding_tensor] = embedding_data
 
-    if not isinstance(texts, list):
-        texts = list(texts)
+    return processed_tensors, tensors[ids_tensor]
 
-    if metadatas is None:
-        metadatas = [{}] * len(texts)
 
-    if embeddings is None:
-        embeddings = [None] * len(texts)
+def create_elements(
+    processed_tensors: Dict[str, List[Any]],
+):
+    tensor_names = list(processed_tensors)
+    elements = [
+        {tensor_name: processed_tensors[tensor_name][i] for tensor_name in tensor_names}
+        for i in range(len(processed_tensors[tensor_names[0]]))
+    ]
+    return elements
+
 
-    processed_tensors = {
-        "ids": ids,
-        "texts": texts,
-        "metadatas": metadatas,
-        "embeddings": embeddings,
-    }
+def set_embedding_info(tensor, embedding_function):
+    embedding_info = tensor.info.get("embedding")
+    if embedding_function and not embedding_info:
+        tensor.info["embedding"] = {
+            "model": embedding_function.__dict__.get("model"),
+            "deployment": embedding_function.__dict__.get("deployment"),
+            "embedding_ctx_length": embedding_function.__dict__.get(
+                "embedding_ctx_length"
+            ),
+            "chunk_size": embedding_function.__dict__.get("chunk_size"),
+            "max_retries": embedding_function.__dict__.get("max_retries"),
+        }
 
-    return processed_tensors, ids
 
+def update_embedding_info(logger, dataset, embedding_function):
+    embeddings_tensors = utils.find_embedding_tensors(dataset)
+    num_embedding_tensors = len(embeddings_tensors)
 
-def create_elements(
-    texts: Iterable[str],
-    ids: Optional[List[str]] = None,
-    metadatas: Optional[List[dict]] = None,
-    embeddings: Optional[Union[List[float], np.ndarray]] = None,
+    if num_embedding_tensors == 0:
+        logger.warning(
+            f"No embedding tensors were found, so the embedding function metadata will not be added to any tensor. "
+            "Consider doing that manually using `vector_store.dataset.tensor_name.info. = <embedding_function_info_dictionary>`"
+        )
+        return
+    if num_embedding_tensors > 1:
+        logger.warning(
+            f"{num_embedding_tensors} embedding tensors were found. "
+            f"It is not clear to which tensor the embedding function information should be added, so the embedding function metadata will not be added to any tensor. "
+            "Consider doing that manually using `vector_store.dataset.tensor_name.info = <embedding_function_info_dictionary>`"
+        )
+        return
+
+    set_embedding_info(dataset[embeddings_tensors[0]], embedding_function)
+
+
+def extend_or_ingest_dataset(
+    processed_tensors,
+    dataset,
+    embedding_function,
+    embedding_tensor,
+    embedding_data,
+    ingestion_batch_size,
+    num_workers,
+    total_samples_processed,
+    logger,
 ):
-    processed_tensors, ids = preprocess_tensors(ids, texts, metadatas, embeddings)
-    utils.check_length_of_each_tensor(processed_tensors)
+    first_item = next(iter(processed_tensors))
+    if len(processed_tensors[first_item]) <= VECTORSTORE_EXTEND_MAX_SIZE:
+        if embedding_function:
+            embedded_data = embedding_function(embedding_data)
+            embedded_data = np.array(embedded_data, dtype=np.float32)
+            processed_tensors[embedding_tensor] = embedded_data
+
+        dataset.extend(processed_tensors)
+    else:
+        elements = dataset_utils.create_elements(processed_tensors)
 
-    elements = [
-        {
-            "text": processed_tensors["texts"][i],
-            "id": processed_tensors["ids"][i],
-            "metadata": processed_tensors["metadatas"][i],
-            "embedding": processed_tensors["embeddings"][i],
-        }
-        for i in range(len(processed_tensors["texts"]))
-    ]
-    return elements, ids
+        ingest_data.run_data_ingestion(
+            elements=elements,
+            dataset=dataset,
+            embedding_function=embedding_function,
+            embedding_tensor=embedding_tensor,
+            ingestion_batch_size=ingestion_batch_size,
+            num_workers=num_workers,
+            total_samples_processed=total_samples_processed,
+            logger=logger,
+        )
+
+
+def convert_id_to_row_id(ids, dataset, search_fn, query, exec_option, filter):
+    if ids is None:
+        delete_view = search_fn(
+            filter=filter,
+            query=query,
+            exec_option=exec_option,
+            return_view=True,
+            k=int(1e9),
+        )
+
+    else:
+        # backwards compatibility
+        tensors = dataset.tensors
+        id_tensor = "id"
+        if "ids" in tensors:
+            id_tensor = "ids"
+
+        delete_view = dataset.filter(lambda x: x[id_tensor].data()["value"] in ids)
+
+    row_ids = list(delete_view.sample_indices)
+    return row_ids
+
+
+def check_delete_arguments(ids, filter, query, delete_all, row_ids, exec_option):
+    if (
+        ids is None
+        and filter is None
+        and query is None
+        and delete_all is None
+        and row_ids is None
+    ):
+        raise ValueError(
+            "Either ids, row_ids, filter, query, or delete_all must be specified."
+        )
+    if exec_option not in ("python", "compute_engine", "tensor_db"):
+        raise ValueError(
+            "Invalid `exec_option` it should be either `python`, `compute_engine`."
+        )
```

### Comparing `deeplake-3.5.4/deeplake/core/vectorstore/vector_search/filter/filter.py` & `deeplake-3.6.0/deeplake/core/vectorstore/vector_search/filter/filter.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,50 +1,61 @@
-import deeplake
 from deeplake.constants import MB
-from deeplake.enterprise.util import raise_indra_installation_error
 from deeplake.util.warnings import always_warn
 
 import numpy as np
 
 import uuid
 from functools import partial
 from typing import Optional, Any, Iterable, List, Dict, Callable, Union
 
 
-def dp_filter(x: dict, filter: Dict[str, str]) -> bool:
+def dp_filter_python(x: dict, filter: Dict) -> bool:
     """Filter helper function for Deep Lake"""
-    metadata = x["metadata"].data()["value"]
-    return all(k in metadata and v == metadata[k] for k, v in filter.items())
 
+    result = True
 
-def attribute_based_filtering(view, filter, exec_option):
-    filtering_exception(filter=filter, exec_option=exec_option)
-    # attribute based filtering
+    for tensor in filter.keys():
+        metadata = x[tensor].data()["value"]
+        result = result and all(
+            k in metadata and v == metadata[k] for k, v in filter[tensor].items()
+        )
+
+    return result
+
+
+def attribute_based_filtering_python(
+    view, filter: Optional[Union[Dict, Callable]] = None
+):
+    if len(view) == 0:
+        raise ValueError("specified dataset is empty")
     if filter is not None:
         if isinstance(filter, dict):
-            filter = partial(dp_filter, filter=filter)
+            filter = partial(dp_filter_python, filter=filter)
 
         view = view.filter(filter)
-        if len(view) == 0:
-            raise ValueError(f"No data was found for {filter} metadata.")
+
     return view
 
 
-def filtering_exception(filter, exec_option):
-    if exec_option in ("compute_engine", "tensor_db") and filter is not None:
-        case_specific_exception = ""
-        if "tensor_db":
-            case_specific_exception += "To run filtering set `remote_db=False`."
-        else:
-            case_specific_exception += (
-                """To run filtering set `exec_option="python"`."""
-            )
-        raise NotImplementedError(
-            f"Filtering data is only supported for python implementations. {case_specific_exception}"
-        )
+def attribute_based_filtering_tql(
+    view, filter: Optional[Dict] = None, debug_mode=False, logger=None
+):
+    tql_filter = ""
+
+    if filter is not None:
+        if isinstance(filter, dict):
+            for tensor in filter.keys():
+                for key, value in filter[tensor].items():
+                    val_str = f"'{value}'" if type(value) == str else f"{value}"
+                    tql_filter += f"{tensor}['{key}'] == {val_str} and "
+            tql_filter = tql_filter[:-5]
+
+    if debug_mode and logger is not None:
+        logger.warning(f"Converted tql string is: '{tql_filter}'")  # pragma: no cover
+    return view, tql_filter
 
 
 def exact_text_search(view, query):
     view = view.filter(lambda x: query in x["text"].data()["value"])
     scores = [1.0] * len(view)
 
     if len(view) == 0:
@@ -76,15 +87,15 @@
         if id not in filtered_ids:
             ids_that_doesnt_exist += f"`{id}`, "
     return ids_that_doesnt_exist[:-2]
 
 
 def get_filtered_ids(dataset, filter):
     filtered_ids = None
-    view = dataset.filter(partial(dp_filter, filter=filter))
+    view = dataset.filter(partial(dp_filter_python, filter=filter))
     filtered_ids = list(view.sample_indices)
     if len(filtered_ids) == 0:
         raise ValueError(f"{filter} does not exist in the dataset.")
     return filtered_ids
 
 
 def get_converted_ids(dataset, filter, ids):
```

### Comparing `deeplake-3.5.4/deeplake/core/vectorstore/vector_search/filter/test_filter.py` & `deeplake-3.6.0/deeplake/core/vectorstore/vector_search/filter/test_filter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 import deeplake
 from deeplake.core.vectorstore.vector_search import filter as filter_utils
 
 import pytest
 
 
 def test_attribute_based_filtering():
-    view = deeplake.empty("mem://deeplake_test")
-    view.create_tensor("metadata", htype="json")
-    view.metadata.extend([{"abcd": 1}, {"abcd123": 2}, {"abcd32": 3}, {"abcrd": 4}])
-    exec_otion = "compute_engine"
-    filter_dict = {"abcd": 1}
-
-    with pytest.raises(NotImplementedError):
-        view = filter_utils.attribute_based_filtering(
-            view, filter=filter_dict, exec_option="compute_engine"
-        )
-
-    with pytest.raises(NotImplementedError):
-        view = filter_utils.attribute_based_filtering(
-            view, filter=filter_dict, exec_option="tensor_db"
-        )
+    ds = deeplake.empty("mem://deeplake_test")
+    ds.create_tensor("metadata", htype="json")
+    ds.create_tensor("metadata2", htype="json")
+    ds.metadata.extend([{"k": 1}, {"k": 2}, {"k": 3}, {"k": 4}])
+    ds.metadata2.extend([{"kk": "a"}, {"kk": "b"}, {"kk": "c"}, {"kk": "d"}])
+
+    filter_dict = {"metadata": {"k": 1}, "metadata2": {"kk": "a"}}
+
+    def filter_udf(x):
+        metadata = x["metadata"].data()["value"]
+        return metadata["k"] == 1
 
-    view = filter_utils.attribute_based_filtering(
-        view, filter=filter_dict, exec_option="python"
+    view_dict = filter_utils.attribute_based_filtering_python(ds, filter=filter_dict)
+
+    view_udf = filter_utils.attribute_based_filtering_python(ds, filter=filter_udf)
+
+    view_tql, tql_filter = filter_utils.attribute_based_filtering_tql(
+        ds, filter=filter_dict
     )
 
-    assert view.metadata.data()["value"][0] == filter_dict
+    assert view_dict.metadata.data()["value"][0] == filter_dict["metadata"]
+    assert view_dict.metadata2.data()["value"][0] == filter_dict["metadata2"]
 
-    with pytest.raises(ValueError):
-        view = filter_utils.attribute_based_filtering(
-            view, filter={"aaaccc": 2}, exec_option="python"
-        )
+    assert view_udf.metadata.data()["value"][0] == filter_dict["metadata"]
+
+    assert len(view_tql) == len(ds)
+    assert tql_filter == "metadata['k'] == 1 and metadata2['kk'] == 'a'"
 
 
 def test_exact_text_search():
     view = deeplake.empty("mem://deeplake_test")
     view.create_tensor("text", htype="text")
     view.text.extend(["abcd", "avc", "anv", "abc"])
 
@@ -76,30 +77,30 @@
 
 
 def test_get_filtered_ids():
     view = deeplake.empty("mem://deeplake_test")
     view.create_tensor("metadata", htype="json")
     view.metadata.extend([{"abc": 1}, {"cd": 2}, {"se": 3}])
 
-    ids = filter_utils.get_filtered_ids(view, filter={"se": 3})
+    ids = filter_utils.get_filtered_ids(view, filter={"metadata": {"se": 3}})
     assert ids == [2]
 
     with pytest.raises(ValueError):
-        ids = filter_utils.get_filtered_ids(view, filter={"se0": 3})
+        ids = filter_utils.get_filtered_ids(view, filter={"metadata": {"se0": 3}})
 
 
 def test_get_converted_ids():
     view = deeplake.empty("mem://deeplake_test")
     view.create_tensor("metadata", htype="json")
     view.metadata.extend([{"abc": 1}, {"cd": 2}, {"se": 3}])
     view.create_tensor("ids")
     view.ids.extend(["ac", "bs", "cd"])
 
     ids = ["cd"]
-    filter = {"se": 3}
+    filter = {"metadata": {"se": 3}}
 
     with pytest.raises(ValueError):
         ids = filter_utils.get_converted_ids(view, filter, ids)
 
     ids = filter_utils.get_converted_ids(view, filter=None, ids=ids)
     assert ids == [2]
```

### Comparing `deeplake-3.5.4/deeplake/core/vectorstore/vector_search/indra/indra_vector_search.py` & `deeplake-3.6.0/deeplake/core/vectorstore/vector_search/python/vector_search.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,53 @@
-import numpy as np
-from typing import Union, List, Any, Optional, Tuple
-
-from deeplake.enterprise.convert_to_libdeeplake import dataset_to_libdeeplake
-
-from deeplake.core.vectorstore.vector_search.indra import query
+from deeplake.core import vectorstore
+from deeplake.core.vectorstore.vector_search import dataset as dataset_utils
+from deeplake.core.vectorstore.vector_search import filter as filter_utils
+from deeplake.core.vectorstore.vector_search import utils
 from deeplake.core.dataset import Dataset as DeepLakeDataset
+from typing import Union, Dict
 
 
 def vector_search(
-    query_embedding: np.ndarray,
-    distance_metric: str,
-    deeplake_dataset: DeepLakeDataset,
-    k: int,
-    embedding_tensor: str,
-    **kwargs
-) -> Tuple[List, List]:
-    """Vector Searching algorithm that uses indra.
-
-    Args:
-        query_embedding (Optional[Union[List[float], np.ndarray): embedding representation of the query.
-        distance_metric (str): Distance metric to compute similarity between query embedding and dataset embeddings
-        deeplake_dataset (DeepLakeDataset): DeepLake dataset object.
-        k (int): number of samples to return after the search.
-        embedding_tensor (str): name of the tensor in the dataset with `htype = "embedding"`.
-        **kwargs (Any): Any additional parameters.
-
-    Returns:
-        Tuple[List, List]: tuple representing the indices of the returned embeddings and their respective scores.
-    """
-
-    tql_query = query.parse_query(distance_metric, k, query_embedding, embedding_tensor)
-    indra_ds = dataset_to_libdeeplake(deeplake_dataset)
-
-    view = indra_ds.query(tql_query)
-    indices = view.indexes
-
-    scores = view.score.numpy()
-    return indices, scores
+    query,
+    query_emb,
+    exec_option,
+    dataset,
+    logger,
+    filter,
+    embedding_tensor,
+    distance_metric,
+    k,
+    return_tensors,
+    return_view,
+) -> Union[Dict, DeepLakeDataset]:
+    if query is not None:
+        raise NotImplementedError(
+            f"User-specified TQL queries are not supported for exec_option={exec_option} "
+        )
+
+    view = filter_utils.attribute_based_filtering_python(dataset, filter)
+
+    return_data = {}
+
+    # Only fetch embeddings and run the search algorithm if an embedding query is specified
+    if query_emb is not None:
+        embeddings = dataset_utils.fetch_embeddings(
+            view=view,
+            embedding_tensor=embedding_tensor,
+        )
+
+        view, scores = vectorstore.python_search_algorithm(
+            deeplake_dataset=view,
+            query_embedding=query_emb,
+            embeddings=embeddings,
+            distance_metric=distance_metric.lower(),
+            k=k,
+        )
+
+        return_data["score"] = scores
+
+    if return_view:
+        return view
+    else:
+        for tensor in return_tensors:
+            return_data[tensor] = utils.parse_tensor_return(view[tensor])
+        return return_data
```

### Comparing `deeplake-3.5.4/deeplake/core/vectorstore/vector_search/indra/query.py` & `deeplake-3.6.0/deeplake/core/vectorstore/vector_search/indra/query.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,75 @@
 import numpy as np
 
-from typing import Optional, Union, List
+from typing import List
 
 from deeplake.core.vectorstore.vector_search.indra import tql_distance_metrics
 
 
-def create_query_string(distance_metric: str, limit: int, order: str = "ASC"):
+def create_query_string(
+    distance_metric: str,
+    tql_filter: str,
+    limit: int,
+    order: str,
+    tensor_list: List[str],
+):
     """Function for creating a query string from a distance metric, limit and order.
 
     Args:
         distance_metric (str): distance metric to compute similarity of the query embedding with dataset's embeddings.
+        tql_filter (str): Additional filter using TQL syntax.
         limit (int): number of samples to return after the search.
         order (str): Type of data ordering after computing similarity score. Defaults to "ASC".
+        tensor_list (List[str]): List of tensors to return data for.
+
 
     Returns:
         str: TQL representation of the query string.
     """
-    return f"select *, {distance_metric} as score ORDER BY {distance_metric} {order} LIMIT {limit}"
+
+    tql_filter_str = tql_filter if tql_filter == "" else " where " + tql_filter
+    tensor_list_str = ", ".join(tensor_list)
+    order_str = "" if order is None else f" order by score {order}"
+    distance_metric_str = (
+        "" if distance_metric is None else f", {distance_metric} as score"
+    )
+
+    return f"select * from (select {tensor_list_str}{distance_metric_str}{tql_filter_str}){order_str} limit {limit}"
 
 
 def create_query(
     distance_metric: str,
-    embeddings: str,
+    embedding_tensor: str,
     query_embedding: str,
+    tql_filter: str,
     limit: int,
+    tensor_list: List[str],
 ):
     """Function for creating a query string from a distance metric, embeddings, query_embedding, and limit.
 
     Args:
         distance_metric (str): distance metric to compute similarity of the query embedding with dataset's embeddings.
-        embeddings (str): name of the tensor in the dataset with `htype = "embedding"`.
+        embedding_tensor (str): name of the tensor in the dataset with ``htype = "embedding"``.
         query_embedding (str): embedding representation of the query string converted to str.
+        tql_filter (str): Additional filter using TQL syntax.
         limit (int): number of samples to return after the search.
+        tensor_list (List[str]): List of tensors to return data for.
+
 
     Returns:
         str: TQL representation of the query string.
     """
+
     order = tql_distance_metrics.get_order_type_for_distance_metric(distance_metric)
     tql_distrance_metric = tql_distance_metrics.get_tql_distance_metric(
-        distance_metric, embeddings, query_embedding
+        distance_metric, embedding_tensor, query_embedding
+    )
+    query = create_query_string(
+        tql_distrance_metric, tql_filter, limit, order, tensor_list
     )
-    query = create_query_string(tql_distrance_metric, limit, order)
     return query
 
 
 def convert_tensor_to_str(query_embedding: np.ndarray):
     """Function for converting a query embedding to a string
 
     We need to convert tensor to a string to be able to use tql
@@ -68,24 +93,38 @@
 
 
 def parse_query(
     distance_metric: str,
     limit: int,
     query_embedding: np.ndarray,
     embedding_tensor: str,
+    tql_filter: str,
+    tensor_list: List[str],
 ) -> str:
     """Function for converting query_embedding into tql query.
 
     Args:
         distance_metric (str): distance metric to compute similarity of the query embedding with dataset's embeddings.
         embedding_tensor (str): name of the tensor in the dataset with `htype = "embedding"`.
         query_embedding (np.ndarray]): embedding representation of the query string.
         limit (int): number of samples to return after the search.
+        tql_filter (str): Additional filter using TQL syntax.
+        tensor_list (list[str]): List of tensors to return data for.
+
 
     Returns:
         str: converted tql query string.
     """
-    query_embedding_str = convert_tensor_to_str(query_embedding)
-    tql_query = create_query(
-        distance_metric, embedding_tensor, query_embedding_str, limit
-    )
-    return tql_query
+    if query_embedding is None:
+        return create_query_string(None, tql_filter, limit, None, tensor_list)
+
+    else:
+        query_embedding_str = convert_tensor_to_str(query_embedding)
+
+        return create_query(
+            distance_metric,
+            embedding_tensor,
+            query_embedding_str,
+            tql_filter,
+            limit,
+            tensor_list,
+        )
```

### Comparing `deeplake-3.5.4/deeplake/core/vectorstore/vector_search/indra/test_indra.py` & `deeplake-3.6.0/deeplake/core/vectorstore/vector_search/indra/test_indra.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     "l2": f"L2_NORM(embedding-{array})",
     "cos": f"COSINE_SIMILARITY(embedding, {array})",
     "max": f"LINF_NORM(embedding-{array})",
 }
 
 
 def create_tql_string(metric_function, order="ASC"):
-    return f"select *, {METRIC_FUNC_TO_METRIC_STRING[metric_function]} as score ORDER BY {METRIC_FUNC_TO_METRIC_STRING[metric_function]} {order} LIMIT 10"
+    return f"select * from (select *, {METRIC_FUNC_TO_METRIC_STRING[metric_function]} as score) order by score {order} limit 10"
 
 
 METRIC_FUNC_TO_QUERY_STRING = {
     "l1": create_tql_string("l1", order="ASC"),
     "l2": create_tql_string("l2", order="ASC"),
     "cos": create_tql_string("cos", order="DESC"),
     "max": create_tql_string("max", order="ASC"),
@@ -53,9 +53,11 @@
         "max",
     ],
 )
 def test_tql_metric_to_tql_str(metric, limit=10):
     query_embedding = np.array([[1, 2, 3, 4, 5, 6, 7, 8]], dtype=np.float32)
     embedding_tensor = "embedding"
 
-    parsed_query = query.parse_query(metric, limit, query_embedding, embedding_tensor)
+    parsed_query = query.parse_query(
+        metric, 10, query_embedding, embedding_tensor, "", ["*"]
+    )
     assert parsed_query == METRIC_FUNC_TO_QUERY_STRING[metric]
```

### Comparing `deeplake-3.5.4/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py` & `deeplake-3.6.0/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-def cosine_similarity(embeddings, query_embedding):
-    return f"COSINE_SIMILARITY({embeddings}, {query_embedding})"
+def cosine_similarity(embedding_tensor, query_embedding):
+    return f"COSINE_SIMILARITY({embedding_tensor}, {query_embedding})"
 
 
-def l1_norm(embeddings, query_embedding):
-    return f"L1_NORM({embeddings}-{query_embedding})"
+def l1_norm(embedding_tensor, query_embedding):
+    return f"L1_NORM({embedding_tensor}-{query_embedding})"
 
 
-def l2_norm(embeddings, query_embedding):
-    return f"L2_NORM({embeddings}-{query_embedding})"
+def l2_norm(embedding_tensor, query_embedding):
+    return f"L2_NORM({embedding_tensor}-{query_embedding})"
 
 
-def linf_norm(embeddings, query_embedding):
-    return f"LINF_NORM({embeddings}-{query_embedding})"
+def linf_norm(embedding_tensor, query_embedding):
+    return f"LINF_NORM({embedding_tensor}-{query_embedding})"
 
 
 TQL_METRIC_TO_TQL_QUERY = {
     "l1": l1_norm,
     "l2": l2_norm,
     "cos": cosine_similarity,
     "max": linf_norm,
 }
 
 
-def get_tql_distance_metric(distance_metric, embeddings, query_embedding):
+def get_tql_distance_metric(distance_metric, embedding_tensor, query_embedding):
     metric_fn = TQL_METRIC_TO_TQL_QUERY[distance_metric]
-    return metric_fn(embeddings, query_embedding)
+    return metric_fn(embedding_tensor, query_embedding)
```

### Comparing `deeplake-3.5.4/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py` & `deeplake-3.6.0/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,66 @@
-from typing import Dict, List, Any, Callable, Optional
+from typing import Dict, List, Any, Callable, Optional, Union
 
 import numpy as np
 
 import deeplake
 from deeplake.core.dataset import Dataset as DeepLakeDataset
 from deeplake.core.vectorstore.vector_search import utils
 from deeplake.util.exceptions import TransformError, FailedIngestionError
 from deeplake.constants import (
     MAX_VECTORSTORE_INGESTION_RETRY_ATTEMPTS,
     MAX_CHECKPOINTING_INTERVAL,
-    MAX_DATASET_LENGTH_FOR_CACHING,
 )
 
 
 class DataIngestion:
     def __init__(
         self,
         elements: List[Dict[str, Any]],
         dataset: DeepLakeDataset,
         embedding_function: Optional[Callable],
+        embedding_tensor: Optional[str],
         ingestion_batch_size: int,
         num_workers: int,
         retry_attempt: int,
         total_samples_processed: int,
+        logger,
     ):
         self.elements = elements
         self.dataset = dataset
         self.embedding_function = embedding_function
         self.ingestion_batch_size = ingestion_batch_size
         self.num_workers = num_workers
         self.retry_attempt = retry_attempt
         self.total_samples_processed = total_samples_processed
+        self.embedding_tensor = embedding_tensor
+        self.logger = logger
 
     def collect_batched_data(self, ingestion_batch_size=None):
         ingestion_batch_size = ingestion_batch_size or self.ingestion_batch_size
         batch_size = min(ingestion_batch_size, len(self.elements))
         if batch_size == 0:
             raise ValueError("batch_size must be a positive number greater than zero.")
 
         elements = self.elements
         if self.total_samples_processed:
-            elements = self.elements[self.total_samples_processed * batch_size :]
+            elements = self.elements[self.total_samples_processed :]
 
         batched = [
             elements[i : i + batch_size] for i in range(0, len(elements), batch_size)
         ]
+
+        if self.logger:
+            batch_upload_str = f"Batch upload: {len(elements)} samples are being uploaded in {len(batched)} batches of batch size {batch_size}"
+            if self.total_samples_processed:
+                batch_upload_str = (
+                    f"Batch reupload: {len(self.elements)-len(elements)} samples already uploaded, while "
+                    f"{len(elements)} samples are being uploaded in {len(batched)} batches of batch size {batch_size}"
+                )
+            self.logger.warning(batch_upload_str)
         return batched
 
     def get_num_workers(self, batched):
         return min(self.num_workers, len(batched) // max(self.num_workers, 1))
 
     def get_checkpoint_interval_and_batched_data(self, batched, num_workers):
         checkpoint_interval = max(
@@ -61,32 +73,14 @@
 
         if checkpoint_interval * self.ingestion_batch_size > MAX_CHECKPOINTING_INTERVAL:
             checkpoint_interval = 100
 
         return checkpoint_interval
 
     def run(self):
-        if (
-            len(self.elements) < MAX_DATASET_LENGTH_FOR_CACHING
-            and self.embedding_function
-        ):
-            full_text = [element["text"] for element in self.elements]
-            embeddings = self.embedding_function(full_text)
-
-            self.elements = [
-                {
-                    "text": element["text"],
-                    "id": element["id"],
-                    "metadata": element["metadata"],
-                    "embedding": embeddings[i],
-                }
-                for i, element in enumerate(self.elements)
-            ]
-            self.embedding_function = None
-
         batched_data = self.collect_batched_data()
         num_workers = self.get_num_workers(batched_data)
         checkpoint_interval = self.get_checkpoint_interval_and_batched_data(
             batched_data, num_workers=num_workers
         )
 
         self._ingest(
@@ -98,28 +92,39 @@
     def _ingest(
         self,
         batched,
         num_workers,
         checkpoint_interval,
     ):
         try:
-            ingest(embedding_function=self.embedding_function).eval(
+            ingest(
+                embedding_function=self.embedding_function,
+                embedding_tensor=self.embedding_tensor,
+            ).eval(
                 batched,
                 self.dataset,
                 num_workers=num_workers,
                 checkpoint_interval=checkpoint_interval,
+                verbose=False,
             )
         except Exception as e:
             self.retry_attempt += 1
             last_checkpoint = self.dataset.version_state["commit_node"].parent
-            self.total_samples_processed += last_checkpoint.total_samples_processed
+            self.total_samples_processed += (
+                last_checkpoint.total_samples_processed * self.ingestion_batch_size
+            )
+
+            index = int(self.total_samples_processed / self.ingestion_batch_size)
+            if isinstance(e, TransformError) and e.index is not None:
+                index += e.index
 
             if self.retry_attempt > MAX_VECTORSTORE_INGESTION_RETRY_ATTEMPTS:
                 raise FailedIngestionError(
-                    f"Maximum retry attempts exceeded. You can resume ingestion, from the latest saved checkpoint.\n"
+                    f"Ingestion failed at batch index {index}. Maximum retry attempts exceeded. You can resume ingestion "
+                    "from the latest saved checkpoint.\n"
                     "To do that you should run:\n"
                     "```\n"
                     "deeplake_vector_store.add(\n"
                     "    texts=texts,\n"
                     "    metadatas=metadatas,\n"
                     "    ids=ids,\n"
                     "    embeddings=embeddings,\n"
@@ -132,35 +137,38 @@
                 elements=self.elements,
                 dataset=self.dataset,
                 embedding_function=self.embedding_function,
                 ingestion_batch_size=self.ingestion_batch_size,
                 num_workers=num_workers,
                 retry_attempt=self.retry_attempt,
                 total_samples_processed=self.total_samples_processed,
+                logger=self.logger,
+                embedding_tensor=self.embedding_tensor,
             )
             data_ingestion.run()
 
 
 @deeplake.compute
-def ingest(sample_in: list, sample_out: list, embedding_function) -> None:
-    text_list = [s["text"] for s in sample_in]
-
-    embeds: List[Optional[np.ndarray]] = [None] * len(text_list)
-    if embedding_function is not None:
+def ingest(
+    sample_in: list,
+    sample_out: list,
+    embedding_function,
+    embedding_tensor,
+) -> None:
+    embeds: List[Optional[np.ndarray]] = [None] * len(sample_in)
+    if embedding_function:
         try:
-            embeddings = embedding_function(text_list)
+            embedding_data = [s[embedding_tensor] for s in sample_in]
+            embeddings = embedding_function(embedding_data)
         except Exception as e:
             raise Exception(
                 "Could not use embedding function. Please try again with a different embedding function."
             )
         embeds = [np.array(e, dtype=np.float32) for e in embeddings]
 
     for s, emb in zip(sample_in, embeds):
-        embedding = emb if embedding_function else s["embedding"]
-        sample_out.append(
-            {
-                "text": s["text"],
-                "metadata": s["metadata"],
-                "ids": s["id"],
-                "embedding": np.array(embedding, dtype=np.float32),
-            }
-        )
+        sample_in_i = {tensor_name: s[tensor_name] for tensor_name in s}
+
+        if embedding_function:
+            sample_in_i[embedding_tensor] = np.array(emb, dtype=np.float32)
+
+        sample_out.append(sample_in_i)
```

### Comparing `deeplake-3.5.4/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py` & `deeplake-3.6.0/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,50 @@
-from typing import Dict, List, Any, Callable, Optional
+import logging
+from typing import Dict, List, Any, Callable, Optional, Union
+
+import numpy as np
 
 from deeplake.core.dataset import Dataset as DeepLakeDataset
 from deeplake.core.vectorstore.vector_search.ingestion.data_ingestion import (
     DataIngestion,
 )
 
 
 def run_data_ingestion(
     elements: List[Dict[str, Any]],
     dataset: DeepLakeDataset,
     ingestion_batch_size: int,
     num_workers: int,
     embedding_function: Optional[Callable] = None,
+    embedding_tensor: Optional[str] = None,
     retry_attempt: int = 0,
-    total_samples_processed=0,
+    total_samples_processed: int = 0,
+    logger: Optional[logging.Logger] = None,
 ):
     """Running data ingestion into deeplake dataset.
 
     Args:
         elements (List[Dict[str, Any]]): List of dictionaries. Each dictionary contains mapping of
             names of 4 tensors (i.e. "embedding", "metadata", "ids", "text") to their corresponding values.
         dataset (DeepLakeDataset): deeplake dataset object.
         embedding_function (Optional[Callable]): function used to convert query into an embedding.
+        embedding_tensor (Optional[str]) : tensor name where embedded data will be stored. Defaults to None.
         ingestion_batch_size (int): The batch size to use during ingestion.
         num_workers (int): The number of workers to use for ingesting data in parallel.
         retry_attempt (int): The number of retry attempts already passed.
-        total_samples_processed (int): The number of samples processed before transforms stopped.
+        total_samples_processed (int): The number of samples processed before transforms stopped. Defaults to 0.
+        logger (Optional[logging.Logger]): logger where all warnings are logged. Defaults to None.
     """
 
     data_ingestion = DataIngestion(
         elements=elements,
         dataset=dataset,
         embedding_function=embedding_function,
+        embedding_tensor=embedding_tensor,
         ingestion_batch_size=ingestion_batch_size,
         num_workers=num_workers,
         retry_attempt=retry_attempt,
         total_samples_processed=total_samples_processed,
+        logger=logger,
     )
 
     data_ingestion.run()
```

### Comparing `deeplake-3.5.4/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py` & `deeplake-3.6.0/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,33 +23,33 @@
 
 def test_ingest_data():
     data = [
         {
             "text": "a",
             "id": np.int64(1),
             "metadata": {"a": 1},
-            "embedding": np.array([0.1, 0.2, 0.3, 0.4]),
+            "embedding": np.array([0.1, 0.2, 0.3, 0.4], dtype=np.float32),
         },
         {
             "text": "b",
             "id": np.int64(2),
             "metadata": {"b": 2},
-            "embedding": np.array([0.1, 0.2, 0.3, 0.4]),
+            "embedding": np.array([0.1, 0.2, 0.3, 0.4], dtype=np.float32),
         },
         {
             "text": "c",
             "id": np.int64(3),
             "metadata": {"c": 3},
-            "embedding": np.array([0.1, 0.2, 0.3, 0.4]),
+            "embedding": np.array([0.1, 0.2, 0.3, 0.4], dtype=np.float32),
         },
         {
             "text": "d",
             "id": np.int64(4),
             "metadata": {"d": 4},
-            "embedding": np.array([0.1, 0.2, 0.3, 0.4]),
+            "embedding": np.array([0.1, 0.2, 0.3, 0.4], dtype=np.float32),
         },
     ]
 
     dataset = deeplake.empty("./xyzabc", overwrite=True)
     dataset.create_tensor(
         "text",
         htype="text",
@@ -72,65 +72,115 @@
         dtype=np.float32,
         create_id_tensor=False,
         create_sample_info_tensor=False,
         max_chunk_size=64 * MB,
         create_shape_tensor=True,
     )
     dataset.create_tensor(
-        "ids",
+        "id",
         htype="text",
         create_id_tensor=False,
         create_sample_info_tensor=False,
         create_shape_tensor=False,
         chunk_compression="lz4",
     )
 
     ingest_data.run_data_ingestion(
         dataset=dataset,
         elements=data,
-        embedding_function=None,
         ingestion_batch_size=1024,
         num_workers=2,
+        logger=None,
     )
 
     assert len(dataset) == 4
-    extended_data = data * 5000
-    embedding_function = partial(corrupted_embedding_function, threshold=0.9)
+    extended_data = data * 5001
+    embedding_function = partial(corrupted_embedding_function, threshold=0.95)
+
+    data = [
+        {
+            "text": "a",
+            "id": np.int64(1),
+            "metadata": {"a": 1},
+        },
+        {
+            "text": "b",
+            "id": np.int64(2),
+            "metadata": {"b": 2},
+        },
+        {
+            "text": "c",
+            "id": np.int64(3),
+            "metadata": {"c": 3},
+        },
+        {
+            "text": "d",
+            "id": np.int64(4),
+            "metadata": {"d": 4},
+        },
+    ]
 
     ingest_data.run_data_ingestion(
         dataset=dataset,
         elements=extended_data,
         embedding_function=embedding_function,
         ingestion_batch_size=1024,
         num_workers=2,
+        embedding_tensor="embedding",
     )
-    assert len(dataset) == 20004
+    assert len(dataset) == 20008
 
     extended_data = extended_data * 10
     embedding_function = partial(corrupted_embedding_function, threshold=0.95)
     with pytest.raises(FailedIngestionError):
         ingest_data.run_data_ingestion(
             dataset=dataset,
             elements=extended_data,
             embedding_function=embedding_function,
             ingestion_batch_size=1024,
             num_workers=2,
+            embedding_tensor="embedding",
+        )
+
+    with pytest.raises(FailedIngestionError):
+        data = [
+            {
+                "text": "a",
+                "id": np.int64(1),
+                "metadata": {"a": 1},
+                "embedding": np.zeros(100, dtype=np.float32),
+            },
+        ]
+        data = 25000 * data
+        data[15364] = {
+            "text": "a",
+            "id": np.int64(4),
+            "metadata": {"d": 4},
+            "embedding": "abc",
+        }
+        ingest_data.run_data_ingestion(
+            dataset=dataset,
+            elements=data,
+            ingestion_batch_size=1000,
+            num_workers=2,
         )
 
     extended_data = extended_data * 10
     with pytest.raises(FailedIngestionError):
         ingest_data.run_data_ingestion(
             dataset=dataset,
             elements=extended_data,
             embedding_function=embedding_function,
             ingestion_batch_size=1024,
             num_workers=2,
+            embedding_tensor="embedding",
         )
 
     with pytest.raises(ValueError):
         ingest_data.run_data_ingestion(
             dataset=dataset,
             elements=extended_data,
             embedding_function=corrupted_embedding_function,
             ingestion_batch_size=0,
             num_workers=2,
+            embedding_tensor="embedding",
         )
```

### Comparing `deeplake-3.5.4/deeplake/core/vectorstore/vector_search/vector_search.py` & `deeplake-3.6.0/deeplake/core/vectorstore/vector_search/vector_search.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,59 @@
-import numpy as np
+from typing import Dict, Callable, List, Union
+from deeplake.core.dataset import Dataset as DeepLakeDataset
 
-from typing import Any, Callable, Dict, List, Union
 
-import deeplake
-from deeplake.core.dataset import Dataset as DeepLakeDataset
+import numpy as np
+
 from deeplake.core import vectorstore
+from deeplake.core.dataset import Dataset as DeepLakeDataset
+from deeplake.core.vectorstore.vector_search import dataset as dataset_utils
+from deeplake.core.vectorstore.vector_search import filter as filter_utils
 
 
 EXEC_OPTION_TO_SEARCH_TYPE: Dict[str, Callable] = {
     "compute_engine": vectorstore.indra_vector_search,
     "python": vectorstore.python_vector_search,
-    "tensor_db": vectorstore.remote_engine_vector_search,
+    "tensor_db": vectorstore.indra_vector_search,
 }
 
 
 def search(
+    query,
+    logger,
+    filter,
     query_embedding: Union[List[float], np.ndarray],
-    embedding: Union[List[float], np.ndarray],
     k: int,
     distance_metric: str,
     exec_option: str,
     deeplake_dataset: DeepLakeDataset,
+    return_tensors: List[str],
     embedding_tensor: str = "embedding",
-):
+    return_view: bool = False,
+) -> Union[Dict, DeepLakeDataset]:
     """Searching function
     Args:
         query_embedding (Union[List[float], np.ndarray]) - embedding representation of the query
-        embedding (Union[List[float], np.ndarray) - full embeddings representation of the dataset, used only in python implementation.
         k (int) - number of samples to return after searching
         distance_metric (str, optional): Type of distance metric to use for sorting the data. Avaliable options are: "L1", "L2", "COS", "MAX".
         exec_option (str, optional): Type of query execution. It could be either "python", "compute_engine" or "tensor_db". Defaults to "python".
             ``python`` - runs on the client and can be used for any data stored anywhere. WARNING: using this option with big datasets is discouraged, because it can lead to some memory issues.
             ``compute_engine`` - runs on the client and can be used for any data stored in or connected to Deep Lake.
             ``tensor_db`` - runs on the Deep Lake Managed Database and can be used for any data stored in the Deep Lake Managed.
         deeplake_dataset (DeepLakeDataset): deeplake dataset object.
+        return_tensors (List[str]): List of tensors to return data for.
         embedding_tensor (str): name of the tensor in the dataset with `htype="embedding"`. Defaults to "embedding".
+        return_view (Bool): Return a Deep Lake dataset view that satisfied the search parameters, instead of a dictinary with data. Defaults to False.
     """
     return EXEC_OPTION_TO_SEARCH_TYPE[exec_option](
-        query_embedding=query_embedding,
-        embedding=embedding,
+        query=query,
+        query_emb=query_embedding,
+        exec_option=exec_option,
+        dataset=deeplake_dataset,
+        logger=logger,
+        filter=filter,
+        embedding_tensor=embedding_tensor,
         distance_metric=distance_metric,
-        deeplake_dataset=deeplake_dataset,
         k=k,
-        embedding_tensor=embedding_tensor,
+        return_tensors=return_tensors,
+        return_view=return_view,
     )
```

### Comparing `deeplake-3.5.4/deeplake/core/version_control/commit_chunk_map.py` & `deeplake-3.6.0/deeplake/core/version_control/commit_chunk_map.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/version_control/commit_diff.py` & `deeplake-3.6.0/deeplake/core/version_control/commit_diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/version_control/commit_node.py` & `deeplake-3.6.0/deeplake/core/version_control/commit_node.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/version_control/dataset_diff.py` & `deeplake-3.6.0/deeplake/core/version_control/dataset_diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/version_control/test_merge.py` & `deeplake-3.6.0/deeplake/core/version_control/test_merge.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/core/version_control/test_version_control.py` & `deeplake-3.6.0/deeplake/core/version_control/test_version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/enterprise/convert_to_libdeeplake.py` & `deeplake-3.6.0/deeplake/enterprise/convert_to_libdeeplake.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from deeplake.core.storage.gcs import GCSProvider
 from deeplake.enterprise.util import raise_indra_installation_error  # type: ignore
 from deeplake.core.storage import S3Provider
+from deeplake.core.storage.azure import AzureProvider
+from deeplake.util.remove_cache import get_base_storage
+from deeplake.util.exceptions import EmptyTokenException
 
 from deeplake.util.dataset import try_flushing  # type: ignore
 import importlib
 import jwt
 
 # Load lazy to avoid cycylic import.
 INDRA_API = None
@@ -24,14 +27,115 @@
     except Exception as e:
         raise_indra_installation_error(e)
 
 
 INDRA_INSTALLED = bool(importlib.util.find_spec("indra"))
 
 
+def _get_indra_ds_from_azure_provider(
+    path: str,
+    token: str,
+    provider: AzureProvider,
+):
+    if provider is None:
+        return None
+
+    api = import_indra_api()
+    account_name = provider.account_name
+    account_key = provider.account_key
+    sas_token = provider.get_sas_token()
+    expiration = str(provider.expiration) if provider.expiration else None
+
+    return api.dataset(
+        path,
+        origin_path=provider.root,
+        token=token,
+        account_name=account_name,
+        account_key=account_key,
+        sas_token=sas_token,
+        expiration=expiration,
+    )
+
+
+def _get_indra_ds_from_gcp_provider(
+    path: str,
+    token: str,
+    provider: GCSProvider,
+):
+    if provider is None:
+        return None
+
+    api = import_indra_api()
+    creds = provider.get_creds()
+    anon = creds.get("anon", "")
+    expiration = creds.get("expiration", "")
+    access_token = creds.get("access_token", "")
+    json_credentials = creds.get("json_credentials", "")
+    endpoint_override = creds.get("endpoint_override", "")
+    scheme = creds.get("scheme", "")
+    retry_limit_seconds = creds.get("retry_limit_seconds", "")
+
+    return api.dataset(
+        path,
+        origin_path=provider.root,
+        token=token,
+        anon=anon,
+        expiration=expiration,
+        access_token=access_token,
+        json_credentials=json_credentials,
+        endpoint_override=endpoint_override,
+        scheme=scheme,
+        retry_limit_seconds=retry_limit_seconds,
+    )
+
+
+def _get_indra_ds_from_s3_provider(
+    path: str,
+    token: str,
+    provider: S3Provider,
+):
+    if provider is None:
+        return None
+
+    api = import_indra_api()
+
+    creds_used = provider.creds_used
+    if creds_used == "PLATFORM":
+        provider._check_update_creds()
+        return api.dataset(
+            path,
+            origin_path=provider.root,
+            token=token,
+            aws_access_key_id=provider.aws_access_key_id,
+            aws_secret_access_key=provider.aws_secret_access_key,
+            aws_session_token=provider.aws_session_token,
+            region_name=provider.aws_region,
+            endpoint_url=provider.endpoint_url,
+            expiration=str(provider.expiration),
+        )
+    elif creds_used == "ENV":
+        return api.dataset(
+            path,
+            origin_path=provider.root,
+            token=token,
+            profile_name=provider.profile_name,
+        )
+    elif creds_used == "DICT":
+        return api.dataset(
+            path,
+            origin_path=provider.root,
+            token=token,
+            aws_access_key_id=provider.aws_access_key_id,
+            aws_secret_access_key=provider.aws_secret_access_key,
+            aws_session_token=provider.aws_session_token,
+            region_name=provider.aws_region,
+            endpoint_url=provider.endpoint_url,
+        )
+
+
 def dataset_to_libdeeplake(hub2_dataset):
     """Convert a hub 2.x dataset object to a libdeeplake dataset object."""
     try_flushing(hub2_dataset)
     api = import_indra_api()
     path: str = hub2_dataset.path
     if hub2_dataset.libdeeplake_dataset is None:
         libdeeplake_dataset = None
@@ -39,69 +143,28 @@
             raise ValueError("Gdrive datasets are not supported for libdeeplake")
         elif path.startswith("mem://"):
             raise ValueError("In memory datasets are not supported for libdeeplake")
         elif path.startswith("hub://"):
             token = hub2_dataset._token
             provider = hub2_dataset.storage.next_storage
             if isinstance(provider, S3Provider):
-                creds_used = provider.creds_used
-                if creds_used == "PLATFORM":
-                    provider._check_update_creds()
-                    libdeeplake_dataset = api.dataset(
-                        path,
-                        origin_path=provider.root,
-                        token=token,
-                        aws_access_key_id=provider.aws_access_key_id,
-                        aws_secret_access_key=provider.aws_secret_access_key,
-                        aws_session_token=provider.aws_session_token,
-                        region_name=provider.aws_region,
-                        endpoint_url=provider.endpoint_url,
-                        expiration=str(provider.expiration),
-                    )
-                elif creds_used == "ENV":
-                    libdeeplake_dataset = api.dataset(
-                        path,
-                        origin_path=provider.root,
-                        token=token,
-                        profile_name=provider.profile_name,
-                    )
-                elif creds_used == "DICT":
-                    libdeeplake_dataset = api.dataset(
-                        path,
-                        origin_path=provider.root,
-                        token=token,
-                        aws_access_key_id=provider.aws_access_key_id,
-                        aws_secret_access_key=provider.aws_secret_access_key,
-                        aws_session_token=provider.aws_session_token,
-                        region_name=provider.aws_region,
-                        endpoint_url=provider.endpoint_url,
-                    )
+                libdeeplake_dataset = _get_indra_ds_from_s3_provider(
+                    path=path, token=token, provider=provider
+                )
 
             elif isinstance(provider, GCSProvider):
-                creds = provider.get_creds()
-                anon = creds.get("anon", "")
-                expiration = creds.get("expiration", "")
-                access_token = creds.get("access_token", "")
-                json_credentials = creds.get("json_credentials", "")
-                endpoint_override = creds.get("endpoint_override", "")
-                scheme = creds.get("scheme", "")
-                retry_limit_seconds = creds.get("retry_limit_seconds", "")
-
-                libdeeplake_dataset = api.dataset(
-                    path,
-                    origin_path=provider.root,
-                    token=token,
-                    anon=anon,
-                    expiration=expiration,
-                    access_token=access_token,
-                    json_credentials=json_credentials,
-                    endpoint_override=endpoint_override,
-                    scheme=scheme,
-                    retry_limit_seconds=retry_limit_seconds,
+                libdeeplake_dataset = _get_indra_ds_from_gcp_provider(
+                    path=path, token=token, provider=provider
                 )
+
+            elif isinstance(provider, AzureProvider):
+                libdeeplake_dataset = _get_indra_ds_from_azure_provider(
+                    path=path, token=token, provider=provider
+                )
+
         elif path.startswith("s3://"):
             s3_provider = hub2_dataset.storage.next_storage
             aws_access_key_id = s3_provider.aws_access_key_id
             aws_secret_access_key = s3_provider.aws_secret_access_key
             aws_session_token = s3_provider.aws_session_token
             region_name = s3_provider.aws_region
             endpoint_url = s3_provider.endpoint_url
@@ -113,39 +176,33 @@
                 aws_secret_access_key=aws_secret_access_key,
                 aws_session_token=aws_session_token,
                 region_name=region_name,
                 endpoint_url=endpoint_url,
             )
 
         elif path.startswith(("gcs://", "gs://", "gcp://")):
-            provider = hub2_dataset.storage.next_storage
-            creds = provider.get_creds()
-            anon = creds.get("anon", "")
-            expiration = creds.get("expiration", "")
-            access_token = creds.get("access_token", "")
-            json_credentials = creds.get("json_credentials", "")
-            endpoint_override = creds.get("endpoint_override", "")
-            scheme = creds.get("scheme", "")
-            retry_limit_seconds = creds.get("retry_limit_seconds", "")
+            provider = get_base_storage(hub2_dataset.storage)
 
-            libdeeplake_dataset = api.dataset(
-                path,
-                anon=anon,
-                expiration=expiration,
-                access_token=access_token,
-                json_credentials=json_credentials,
-                endpoint_override=endpoint_override,
-                scheme=scheme,
-                retry_limit_seconds=retry_limit_seconds,
+            libdeeplake_dataset = _get_indra_ds_from_gcp_provider(
+                path=path, token=None, provider=provider
+            )
+
+        elif path.startswith(("az://", "azure://")):
+            az_provider = get_base_storage(hub2_dataset.storage)
+            libdeeplake_dataset = _get_indra_ds_from_azure_provider(
+                path=path, token=None, provider=az_provider
             )
+
         else:
             token = hub2_dataset._token
             org_id = hub2_dataset.org_id
             if token is None:
                 libdeeplake_dataset = api.dataset(path)
+            elif token == "":
+                raise EmptyTokenException
             else:
                 org_id = (
                     org_id
                     or jwt.decode(token, options={"verify_signature": False})["id"]
                 )
                 libdeeplake_dataset = api.dataset(path, token=token, org_id=org_id)
```

### Comparing `deeplake-3.5.4/deeplake/enterprise/dataloader.py` & `deeplake-3.6.0/deeplake/enterprise/dataloader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/enterprise/dummy_dataloader.py` & `deeplake-3.6.0/deeplake/enterprise/dummy_dataloader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/enterprise/libdeeplake_query.py` & `deeplake-3.6.0/deeplake/enterprise/libdeeplake_query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/enterprise/test_pytorch.py` & `deeplake-3.6.0/deeplake/enterprise/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/enterprise/test_query.py` & `deeplake-3.6.0/deeplake/enterprise/test_query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/enterprise/test_tensorflow.py` & `deeplake-3.6.0/deeplake/enterprise/test_tensorflow.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/enterprise/util.py` & `deeplake-3.6.0/deeplake/enterprise/util.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/hooks.py` & `deeplake-3.6.0/deeplake/hooks.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/htype.py` & `deeplake-3.6.0/deeplake/htype.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/integrations/huggingface/huggingface.py` & `deeplake-3.6.0/deeplake/integrations/huggingface/huggingface.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         it will be converted to a Deep Lake :class:`Dataset` with tensors ``['train/data', 'validation/data', 'test/data']``.
 
         Features of the type ``Sequence(feature=Value(dtype='string'))`` are not supported. Columns of such type are skipped.
 
     """
 
     feature_report_path(
-        dest,
+        dest if isinstance(dest, str) else dest.path,
         "ingest_huggingface",
         parameters={},
         token=token,
     )
 
     from datasets import DatasetDict
```

### Comparing `deeplake-3.5.4/deeplake/integrations/mmdet/mmdet_.py` & `deeplake-3.6.0/deeplake/integrations/mmdet/mmdet_.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/integrations/mmdet/mmdet_runners.py` & `deeplake-3.6.0/deeplake/integrations/mmdet/mmdet_runners.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/integrations/mmdet/mmdet_utils.py` & `deeplake-3.6.0/deeplake/integrations/mmdet/mmdet_utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/integrations/pytorch/common.py` & `deeplake-3.6.0/deeplake/integrations/pytorch/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/integrations/pytorch/dataset.py` & `deeplake-3.6.0/deeplake/integrations/pytorch/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/integrations/pytorch/pytorch.py` & `deeplake-3.6.0/deeplake/integrations/pytorch/pytorch.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/integrations/pytorch/shuffle_buffer.py` & `deeplake-3.6.0/deeplake/integrations/pytorch/shuffle_buffer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/integrations/tf/common.py` & `deeplake-3.6.0/deeplake/integrations/tf/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/integrations/tf/datasettotensorflow.py` & `deeplake-3.6.0/deeplake/integrations/tf/datasettotensorflow.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/integrations/tf/deeplake_tensorflow_dataset.py` & `deeplake-3.6.0/deeplake/integrations/tf/deeplake_tensorflow_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/integrations/wandb/wandb.py` & `deeplake-3.6.0/deeplake/integrations/wandb/wandb.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/tests/cache_fixtures.py` & `deeplake-3.6.0/deeplake/tests/cache_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/tests/client_fixtures.py` & `deeplake-3.6.0/deeplake/tests/client_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/tests/common.py` & `deeplake-3.6.0/deeplake/tests/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 )
 from deeplake.core.tensor_link import (
     _register_link_transform,
     _unregister_link_transform,
 )
 
 
-SESSION_ID = str(uuid4())[:4]  # 4 ascii chars should be sufficient
+SESSION_ID = "tmp" + str(uuid4())[:4]  # 4 ascii chars should be sufficient
 
 _THIS_FILE = pathlib.Path(__file__).parent.absolute()
 TENSOR_KEY = "tensor"
 
 SHAPE_PARAM = "shape"
 NUM_BATCHES_PARAM = "num_batches"
 DTYPE_PARAM = "dtype"
@@ -124,14 +124,19 @@
 
 requires_libdeeplake = pytest.mark.skipif(
     sys.platform not in ["darwin", "Darwin"]
     or (sys.version_info[0] == 3 and sys.version_info[1] == 6),
     reason="These tests require libdeeplake to be installed",
 )
 
+requires_non_python11 = pytest.mark.skipif(
+    sys.version_info[0] == 3 and sys.version_info[1] > 10,
+    reason="These tests require to run on all python vestions lover than 3.11",
+)
+
 
 class LinkTransformTestContext:
     def __init__(self, func: Callable, name: str):
         self.func = func
         self.name = name
 
     def __enter__(self):
```

### Comparing `deeplake-3.5.4/deeplake/tests/dataset_fixtures.py` & `deeplake-3.6.0/deeplake/tests/dataset_fixtures.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,60 +1,63 @@
 import pytest
 import deeplake
 from deeplake.constants import HUB_CLOUD_DEV_USERNAME
 
 
 enabled_datasets = pytest.mark.parametrize(
     "ds",
-    ["memory_ds", "local_ds", "s3_ds", "gcs_ds", "gdrive_ds"],
+    ["memory_ds", "local_ds", "s3_ds", "gcs_ds", "azure_ds", "gdrive_ds"],
     indirect=True,
 )
 
 enabled_non_gdrive_datasets = pytest.mark.parametrize(
     "ds",
-    ["memory_ds", "local_ds", "s3_ds", "gcs_ds"],
+    ["memory_ds", "local_ds", "s3_ds", "gcs_ds", "azure_ds"],
     indirect=True,
 )
 
 enabled_non_gcs_datasets = pytest.mark.parametrize(
     "ds",
-    ["memory_ds", "local_ds", "s3_ds", "gdrive_ds"],
+    ["memory_ds", "local_ds", "s3_ds", "azure_ds", "gdrive_ds"],
     indirect=True,
 )
 
 enabled_non_gcs_gdrive_datasets = pytest.mark.parametrize(
-    "ds", ["memory_ds", "local_ds", "s3_ds"], indirect=True
+    "ds", ["memory_ds", "local_ds", "s3_ds", "azure_ds"], indirect=True
 )
 
 enabled_persistent_dataset_generators = pytest.mark.parametrize(
     "ds_generator",
     [
         "local_ds_generator",
         "s3_ds_generator",
         "gcs_ds_generator",
+        "azure_ds_generator",
         "gdrive_ds_generator",
     ],
     indirect=True,
 )
 
 enabled_persistent_non_gdrive_dataset_generators = pytest.mark.parametrize(
     "ds_generator",
     [
         "local_ds_generator",
         "s3_ds_generator",
         "gcs_ds_generator",
+        "azure_ds_generator",
     ],
     indirect=True,
 )
 
 enabled_cloud_dataset_generators = pytest.mark.parametrize(
     "ds_generator",
     [
         "s3_ds_generator",
         "gcs_ds_generator",
+        "azure_ds_generator",
     ],
     indirect=True,
 )
 
 
 @pytest.fixture
 def memory_ds(memory_path):
@@ -110,14 +113,27 @@
     def generate_gcs_ds(**kwargs):
         return deeplake.dataset(gcs_path, creds=gcs_creds, **kwargs)
 
     return generate_gcs_ds
 
 
 @pytest.fixture
+def azure_ds(azure_ds_generator):
+    return azure_ds_generator()
+
+
+@pytest.fixture
+def azure_ds_generator(azure_path):
+    def generate_azure_ds(**kwargs):
+        return deeplake.dataset(azure_path, **kwargs)
+
+    return generate_azure_ds
+
+
+@pytest.fixture
 def hub_cloud_ds(hub_cloud_ds_generator):
     return hub_cloud_ds_generator()
 
 
 @pytest.fixture
 def hub_cloud_ds_generator(hub_cloud_path, hub_cloud_dev_token):
     def generate_hub_cloud_ds(**kwargs):
```

### Comparing `deeplake-3.5.4/deeplake/tests/path_fixtures.py` & `deeplake-3.6.0/deeplake/tests/path_fixtures.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from deeplake.core.storage.gcs import GCSProvider
 from deeplake.core.storage.google_drive import GDriveProvider
 from deeplake.util.storage import storage_provider_from_hub_path
 from deeplake.core.storage.s3 import S3Provider
 from deeplake.core.storage.local import LocalProvider
+from deeplake.core.storage.azure import AzureProvider
 import os
 import deeplake
 from deeplake.constants import (
     HUB_CLOUD_OPT,
     KEEP_STORAGE_OPT,
     LOCAL_OPT,
     MEMORY_OPT,
     PYTEST_GCS_PROVIDER_BASE_ROOT,
+    PYTEST_AZURE_PROVIDER_BASE_ROOT,
     PYTEST_S3_PROVIDER_BASE_ROOT,
     PYTEST_HUB_CLOUD_PROVIDER_BASE_ROOT,
     PYTEST_LOCAL_PROVIDER_BASE_ROOT,
     PYTEST_MEMORY_PROVIDER_BASE_ROOT,
     S3_OPT,
     GCS_OPT,
+    AZURE_OPT,
     GDRIVE_OPT,
     S3_PATH_OPT,
     GDRIVE_PATH_OPT,
     ENV_GOOGLE_APPLICATION_CREDENTIALS,
     ENV_GDRIVE_CLIENT_ID,
     ENV_GDRIVE_CLIENT_SECRET,
     ENV_GDRIVE_REFRESH_TOKEN,
@@ -37,14 +40,15 @@
 
 
 MEMORY = "memory"
 LOCAL = "local"
 S3 = "s3"
 GDRIVE = "gdrive"
 GCS = "gcs"
+AZURE = "azure"
 HUB_CLOUD = "hub_cloud"
 
 _GIT_CLONE_CACHE_DIR = ".test_resources"
 
 _HUB_TEST_RESOURCES_URL = "https://www.github.com/activeloopai/hub-test-resources.git"
 _PILLOW_URL = "https://www.github.com/python-pillow/Pillow.git"
 _MMDET_URL = "https://www.github.com/open-mmlab/mmdetection.git"
@@ -202,14 +206,20 @@
         },
         GCS: {
             "base_root": PYTEST_GCS_PROVIDER_BASE_ROOT,
             "use_id": True,
             "is_id_prefix": True,
             "use_underscores": False,
         },
+        AZURE: {
+            "base_root": PYTEST_AZURE_PROVIDER_BASE_ROOT,
+            "use_id": True,
+            "is_id_prefix": True,
+            "use_underscores": False,
+        },
         HUB_CLOUD: {
             "base_root": PYTEST_HUB_CLOUD_PROVIDER_BASE_ROOT,
             "use_id": True,
             "is_id_prefix": True,
             "use_underscores": True,
         },
     }
@@ -293,27 +303,14 @@
 
 
 @pytest.fixture(scope="session")
 def gcs_creds():
     return os.environ.get(ENV_GOOGLE_APPLICATION_CREDENTIALS, None)
 
 
-@pytest.fixture(scope="session")
-def gdrive_creds():
-    client_id = os.environ.get(ENV_GDRIVE_CLIENT_ID)
-    client_secret = os.environ.get(ENV_GDRIVE_CLIENT_SECRET)
-    refresh_token = os.environ.get(ENV_GDRIVE_REFRESH_TOKEN)
-    creds = {
-        "client_id": client_id,
-        "client_secret": client_secret,
-        "refresh_token": refresh_token,
-    }
-    return creds
-
-
 @pytest.fixture
 def gcs_path(request, gcs_creds):
     if not is_opt_true(request, GCS_OPT):
         pytest.skip()
         return
 
     path = _get_storage_path(request, GCS)
@@ -333,14 +330,51 @@
         return
 
     path = f"{PYTEST_GCS_PROVIDER_BASE_ROOT}vstream_test"
     yield path
 
 
 @pytest.fixture
+def azure_path(request):
+    if not is_opt_true(request, AZURE_OPT):
+        pytest.skip()
+
+    path = _get_storage_path(request, AZURE)
+    AzureProvider(path).clear()
+
+    yield path
+
+    # clear storage unless flagged otherwise
+    if not is_opt_true(request, KEEP_STORAGE_OPT):
+        AzureProvider(path).clear()
+
+
+@pytest.fixture
+def azure_vstream_path(request):
+    if not is_opt_true(request, AZURE_OPT):
+        pytest.skip()
+
+    path = f"{PYTEST_AZURE_PROVIDER_BASE_ROOT}vstream_test"
+    yield path
+
+
+@pytest.fixture(scope="session")
+def gdrive_creds():
+    client_id = os.environ.get(ENV_GDRIVE_CLIENT_ID)
+    client_secret = os.environ.get(ENV_GDRIVE_CLIENT_SECRET)
+    refresh_token = os.environ.get(ENV_GDRIVE_REFRESH_TOKEN)
+    creds = {
+        "client_id": client_id,
+        "client_secret": client_secret,
+        "refresh_token": refresh_token,
+    }
+    return creds
+
+
+@pytest.fixture
 def gdrive_path(request, gdrive_creds):
     if not is_opt_true(request, GDRIVE_OPT):
         pytest.skip()
         return
 
     path = _get_storage_path(request, GDRIVE, with_current_test_name=False)
     GDriveProvider(path, token=gdrive_creds).clear()
```

### Comparing `deeplake-3.5.4/deeplake/tests/storage_fixtures.py` & `deeplake-3.6.0/deeplake/tests/storage_fixtures.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,54 @@
 from deeplake.core.storage.gcs import GCSProvider
 from deeplake.util.storage import storage_provider_from_hub_path
 from deeplake.core.storage.s3 import S3Provider
 from deeplake.core.storage.google_drive import GDriveProvider
 from deeplake.core.storage.local import LocalProvider
 from deeplake.core.storage.memory import MemoryProvider
+from deeplake.core.storage.azure import AzureProvider
 from deeplake.constants import (
     PYTEST_S3_PROVIDER_BASE_ROOT,
     PYTEST_GCS_PROVIDER_BASE_ROOT,
+    PYTEST_AZURE_PROVIDER_BASE_ROOT,
     S3_OPT,
     GCS_OPT,
+    AZURE_OPT,
 )
 from deeplake.tests.common import is_opt_true
 import pytest
 
 
 enabled_storages = pytest.mark.parametrize(
     "storage",
-    ["memory_storage", "local_storage", "s3_storage", "gcs_storage", "gdrive_storage"],
+    [
+        "memory_storage",
+        "local_storage",
+        "s3_storage",
+        "gcs_storage",
+        "azure_storage",
+        "gdrive_storage",
+    ],
     indirect=True,
 )
 
 enabled_persistent_storages = pytest.mark.parametrize(
     "storage",
-    ["local_storage", "s3_storage", "gcs_storage", "gdrive_storage"],
+    ["local_storage", "s3_storage", "gcs_storage", "azure_storage", "gdrive_storage"],
     indirect=True,
 )
 
 
 enabled_remote_storages = pytest.mark.parametrize(
     "storage",
     [
         "s3_storage",
         "gcs_storage",
         "gdrive_storage",
         "gcs_root_storage",
+        "azure_root_storage",
         "s3_root_storage",
     ],
     indirect=True,
 )
 
 
 @pytest.fixture
@@ -62,14 +73,19 @@
 
 @pytest.fixture
 def gcs_storage(gcs_path):
     return GCSProvider(gcs_path)
 
 
 @pytest.fixture
+def azure_storage(azure_path):
+    return AzureProvider(azure_path)
+
+
+@pytest.fixture
 def s3_root_storage(request):
     if not is_opt_true(request, S3_OPT):
         pytest.skip()
         return
 
     return S3Provider(PYTEST_S3_PROVIDER_BASE_ROOT)
 
@@ -80,14 +96,22 @@
         pytest.skip()
         return
 
     return GCSProvider(PYTEST_GCS_PROVIDER_BASE_ROOT, token=gcs_creds)
 
 
 @pytest.fixture
+def azure_root_storage(request):
+    if not is_opt_true(request, AZURE_OPT):
+        pytest.skip()
+
+    return AzureProvider(PYTEST_AZURE_PROVIDER_BASE_ROOT)
+
+
+@pytest.fixture
 def hub_cloud_storage(hub_cloud_path, hub_cloud_dev_token):
     return storage_provider_from_hub_path(hub_cloud_path, token=hub_cloud_dev_token)
 
 
 @pytest.fixture
 def storage(request):
     """Used with parametrize to use all enabled storage fixtures."""
```

### Comparing `deeplake-3.5.4/deeplake/util/access_method.py` & `deeplake-3.6.0/deeplake/util/access_method.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/agreement.py` & `deeplake-3.6.0/deeplake/util/agreement.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/array_list.py` & `deeplake-3.6.0/deeplake/util/array_list.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/assert_byte_indexes.py` & `deeplake-3.6.0/deeplake/util/assert_byte_indexes.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/auto.py` & `deeplake-3.6.0/deeplake/util/auto.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/bugout_reporter.py` & `deeplake-3.6.0/deeplake/util/bugout_reporter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 import json
 import os
 from pathlib import Path
 from platform import machine
-from typing import Any, Dict, Optional
+from typing import Any, Dict, Optional, Union
 import uuid
 
 from deeplake.client.config import REPORTING_CONFIG_FILE_PATH
 from deeplake.client.client import DeepLakeBackendClient
 from deeplake.client.utils import get_user_name
 from deeplake.util.bugout_token import BUGOUT_TOKEN
 from humbug.consent import HumbugConsent
 from humbug.report import HumbugReporter
 
+import pathlib
+
+from deeplake.util.path import (
+    convert_pathlib_to_string_if_needed,
+)
+
 
 def save_reporting_config(
     consent: bool, client_id: Optional[str] = None, username: Optional[str] = None
 ) -> Dict[str, Any]:
     """Modify reporting config.
 
     Args:
@@ -136,23 +142,24 @@
 
 machine_id = bugout_reporting_config.get("machine_id")
 if machine_id is not None:
     deeplake_reporter.tags.append(f"machine_id:{machine_id}")
 
 
 def feature_report_path(
-    path: str,
+    path: Union[str, pathlib.Path],
     feature_name: str,
     parameters: dict,
     starts_with: str = "hub://",
     token: Optional[str] = None,
 ):
     """Helper function for generating humbug feature reports depending on the path"""
-    if not isinstance(path, str):
-        path = str(path)
+
+    path = convert_pathlib_to_string_if_needed(path)
+
     if path.startswith(starts_with):
         parameters["Path"] = path
 
     if token is not None:
         client = DeepLakeBackendClient(token=token)
         username = client.get_user_profile()["name"]
```

### Comparing `deeplake-3.5.4/deeplake/util/cache_chain.py` & `deeplake-3.6.0/deeplake/util/cache_chain.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/casting.py` & `deeplake-3.6.0/deeplake/util/casting.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/check_latest_version.py` & `deeplake-3.6.0/deeplake/util/check_latest_version.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/chunk_engine.py` & `deeplake-3.6.0/deeplake/util/chunk_engine.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/class_label.py` & `deeplake-3.6.0/deeplake/util/class_label.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/compute.py` & `deeplake-3.6.0/deeplake/util/compute.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/connect_dataset.py` & `deeplake-3.6.0/deeplake/util/connect_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 def log_dataset_connection_success(ds_path: str):
     logger.info("Dataset connected successfully.")
     log_visualizer_link(ds_path)
 
 
 def is_path_connectable(path: str) -> bool:
-    return get_path_type(path) in ("s3", "gcs")
+    return get_path_type(path) in ("s3", "gcs", "azure")
 
 
 def connect_dataset_entry(
     src_path: str,
     creds_key: str,
     dest_path: Optional[str] = None,
     org_id: Optional[str] = None,
@@ -76,24 +76,24 @@
 
         self.org_id, self.ds_name = ds_info.get_org_id_and_ds_name()
 
     def validate(self):
         """Validates the attributes to make that dataset at ``src_path`` can be connected.
 
         Raises:
-            InvalidSourcePathError: If the ``src_path`` is not a valid s3 or gcs path.
+            InvalidSourcePathError: If the ``src_path`` is not a valid s3, gcs or azure path.
         """
         if is_hub_cloud_path(self.src_path):
             raise InvalidSourcePathError(
                 "Source dataset is already accessible via a Deep Lake path."
             )
 
         if not is_path_connectable(self.src_path):
             raise InvalidSourcePathError(
-                f"Source path may only be an s3 or gcs path. Got {self.src_path}."
+                f"Source path may only be an s3, gcs or azure path. Got {self.src_path}."
             )
 
     def connect_dataset_entry(self) -> str:
         connected_id = self.client.connect_dataset_entry(
             src_path=self.src_path,
             org_id=self.org_id,
             ds_name=self.ds_name,
```

### Comparing `deeplake-3.5.4/deeplake/util/dataset.py` & `deeplake-3.6.0/deeplake/util/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/diff.py` & `deeplake-3.6.0/deeplake/util/diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/downsample.py` & `deeplake-3.6.0/deeplake/util/downsample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/encoder.py` & `deeplake-3.6.0/deeplake/util/encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/exceptions.py` & `deeplake-3.6.0/deeplake/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/exif.py` & `deeplake-3.6.0/deeplake/util/exif.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/from_tfds.py` & `deeplake-3.6.0/deeplake/util/from_tfds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/htype.py` & `deeplake-3.6.0/deeplake/util/htype.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/image.py` & `deeplake-3.6.0/deeplake/util/image.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/invalid_view_op.py` & `deeplake-3.6.0/deeplake/util/invalid_view_op.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/iteration_warning.py` & `deeplake-3.6.0/deeplake/util/iteration_warning.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/json.py` & `deeplake-3.6.0/deeplake/util/json.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/keys.py` & `deeplake-3.6.0/deeplake/util/keys.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/link.py` & `deeplake-3.6.0/deeplake/util/link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/logging.py` & `deeplake-3.6.0/deeplake/util/logging.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/merge.py` & `deeplake-3.6.0/deeplake/util/merge.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/modified.py` & `deeplake-3.6.0/deeplake/util/modified.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/notebook.py` & `deeplake-3.6.0/deeplake/util/notebook.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/object_3d/mesh.py` & `deeplake-3.6.0/deeplake/util/object_3d/mesh.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/object_3d/object_base_3d.py` & `deeplake-3.6.0/deeplake/util/object_3d/object_base_3d.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/object_3d/ply_parser.py` & `deeplake-3.6.0/deeplake/util/object_3d/ply_parser.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/object_3d/ply_parser_base.py` & `deeplake-3.6.0/deeplake/util/object_3d/ply_parser_base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/object_3d/ply_parsers.py` & `deeplake-3.6.0/deeplake/util/object_3d/ply_parsers.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/object_3d/ply_reader.py` & `deeplake-3.6.0/deeplake/util/object_3d/ply_reader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/object_3d/ply_reader_base.py` & `deeplake-3.6.0/deeplake/util/object_3d/ply_reader_base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/object_3d/ply_readers.py` & `deeplake-3.6.0/deeplake/util/object_3d/ply_readers.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/object_3d/point_cloud.py` & `deeplake-3.6.0/deeplake/util/object_3d/point_cloud.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/object_3d/read_3d_data.py` & `deeplake-3.6.0/deeplake/util/object_3d/read_3d_data.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/path.py` & `deeplake-3.6.0/deeplake/util/path.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,16 @@
         return "hub"
     elif path.startswith(("http://", "https://")):
         return "http"
     elif path.startswith(("gcs://", "gcp://", "gs://")):
         return "gcs"
     elif path.startswith("s3://"):
         return "s3"
+    elif path.startswith(("az://", "azure://")):
+        return "azure"
     elif path.startswith("gdrive://"):
         return "gdrive"
     else:
         return "local"
 
 
 def is_remote_path(path: str) -> bool:
```

### Comparing `deeplake-3.5.4/deeplake/util/pretty_print.py` & `deeplake-3.6.0/deeplake/util/pretty_print.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/remove_cache.py` & `deeplake-3.6.0/deeplake/util/remove_cache.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/scheduling.py` & `deeplake-3.6.0/deeplake/util/scheduling.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/shape_interval.py` & `deeplake-3.6.0/deeplake/util/shape_interval.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/spinner.py` & `deeplake-3.6.0/deeplake/util/spinner.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,14 @@
             with self._stderr_lock:
                 self._hide_event.clear()
                 self._clear_line()
                 self._hide_cursor()
 
     def stop(self):
         self._stop_event.set()
-        self.join()
         self._clear_line()
         self._show_cursor()
 
     def _clear_line(self):
         if self.file.isatty():
             # ANSI Control Sequence EL does not work in Jupyter
             self.file.write("\r\033[K")
```

### Comparing `deeplake-3.5.4/deeplake/util/split.py` & `deeplake-3.6.0/deeplake/util/split.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/storage.py` & `deeplake-3.6.0/deeplake/util/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-from deeplake.core.storage.gcs import GCSProvider
 from deeplake.util.agreement import handle_dataset_agreements
 from deeplake.util.cache_chain import generate_chain
 from deeplake.constants import LOCAL_CACHE_PREFIX, MB
 from deeplake.util.exceptions import AgreementNotAcceptedError
 from deeplake.util.tag import process_hub_path
 from typing import Optional, Union
 from deeplake.core.storage.provider import StorageProvider
 import os
 from deeplake.core.storage import (
     LocalProvider,
     S3Provider,
+    GCSProvider,
+    AzureProvider,
     MemoryProvider,
     GDriveProvider,
 )
 from deeplake.client.client import DeepLakeBackendClient
 import posixpath
 from deeplake.constants import DEFAULT_READONLY
 
@@ -76,14 +77,16 @@
             )
         elif (
             path.startswith("gcp://")
             or path.startswith("gcs://")
             or path.startswith("gs://")
         ):
             storage = GCSProvider(path, creds)
+        elif path.startswith(("az://", "azure://")):
+            storage = AzureProvider(path, creds)
         elif path.startswith("gdrive://"):
             storage = GDriveProvider(path, creds)
         elif path.startswith("mem://"):
             storage = MemoryProvider(path)
         else:
             if not os.path.exists(path) or os.path.isdir(path):
                 storage = LocalProvider(path)
```

### Comparing `deeplake-3.5.4/deeplake/util/tag.py` & `deeplake-3.6.0/deeplake/util/tag.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/testing.py` & `deeplake-3.6.0/deeplake/util/testing.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/tests/test_auto.py` & `deeplake-3.6.0/deeplake/util/tests/test_auto.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/tests/test_connect_dataset.py` & `deeplake-3.6.0/deeplake/util/tests/test_connect_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/tests/test_iterable_ordered_dict.py` & `deeplake-3.6.0/deeplake/util/tests/test_iterable_ordered_dict.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/tests/test_read.py` & `deeplake-3.6.0/deeplake/util/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/tests/test_shape_interval.py` & `deeplake-3.6.0/deeplake/util/tests/test_shape_interval.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/tests/test_split.py` & `deeplake-3.6.0/deeplake/util/tests/test_split.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/tests/test_version_control.py` & `deeplake-3.6.0/deeplake/util/tests/test_version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/transform.py` & `deeplake-3.6.0/deeplake/util/transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -682,24 +682,26 @@
         load_meta(target_ds)
         if completed:
             target_ds.storage.autoflush = initial_autoflush
             if not kwargs.get("disable_rechunk"):
                 rechunk_if_necessary(target_ds)
 
 
-def check_checkpoint_interval(data_in, checkpoint_interval, num_workers, overwrite):
+def check_checkpoint_interval(
+    data_in, checkpoint_interval, num_workers, overwrite, verbose
+):
     if num_workers > 0 and checkpoint_interval % num_workers != 0:
         raise ValueError(
             "checkpoint_interval should be a multiple of num_workers if num_workers > 0"
         )
     if checkpoint_interval > len(data_in):
         raise ValueError(
             "checkpoint_interval should be less than or equal to the length of data_in"
         )
-    if checkpoint_interval < len(data_in) / 10:
+    if checkpoint_interval < len(data_in) / 10 and verbose:
         warnings.warn(
             "checkpoint_interval is less than 10% of the length of data_in, this can lead to too many commits, consider increasing checkpoint_interval."
         )
     if overwrite:
         raise ValueError(
             "checkpoint_interval > 0 and ds_out is None. Cannot checkpoint during inplace transform."
         )
```

### Comparing `deeplake-3.5.4/deeplake/util/version_control.py` & `deeplake-3.6.0/deeplake/util/version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/util/video.py` & `deeplake-3.6.0/deeplake/util/video.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/visualizer/video_streaming.py` & `deeplake-3.6.0/deeplake/visualizer/video_streaming.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake/visualizer/visualizer.py` & `deeplake-3.6.0/deeplake/visualizer/visualizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.5.4/deeplake.egg-info/PKG-INFO` & `deeplake-3.6.0/deeplake.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: deeplake
-Version: 3.5.4
+Version: 3.6.0
 Summary: Activeloop Deep Lake
 Home-page: UNKNOWN
 Author: activeloop.ai
 Author-email: support@activeloop.ai
 License: MPL-2.0
 Project-URL: Documentation, https://docs.activeloop.ai/
 Project-URL: Source, https://github.com/activeloopai/deeplake
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: audio
 Provides-Extra: av
+Provides-Extra: azure
 Provides-Extra: dicom
 Provides-Extra: enterprise
 Provides-Extra: gcp
 Provides-Extra: gdrive
 Provides-Extra: medical
 Provides-Extra: point_cloud
 Provides-Extra: video
 Provides-Extra: visualizer
 License-File: LICENSE
 
 <img src="https://static.scarf.sh/a.png?x-pxid=bc3c57b0-9a65-49fe-b8ea-f711c4d35b82" /><p align="center">
      <img src="https://i.postimg.cc/rsjcWc3S/deeplake-logo.png" width="400"/>
 </h1>
     </br>
-    <h1 align="center">Deep Lake: Vector Database for any AI data
+    <h1 align="center">Deep Lake: Database for AI
  </h1>
 <p align="center">
     <a href="https://github.com/activeloopai/Hub/actions/workflows/test-pr-on-label.yml"><img src="https://github.com/activeloopai/Hub/actions/workflows/test-push.yml/badge.svg" alt="PyPI version" height="18"></a>
     <a href="https://pypi.org/project/deeplake/"><img src="https://badge.fury.io/py/deeplake.svg" alt="PyPI version" height="18"></a>
     <a href='https://docs.deeplake.ai/en/latest/?badge=latest'>
      <img src='https://readthedocs.org/projects/deep-lake/badge/?version=latest' alt='Documentation Status' />
      </a>
@@ -52,15 +53,15 @@
  </h3>
  
 
 *Read this in other languages: [简体中文](README.zh-cn.md)*
 
 ## About Deep Lake
 
-Deep Lake is a Vector Database powered by a unique storage format optimized for deep-learning and Large Language Model (LLM) based applications. It simplifies the deployment of enterprise-grade LLM-based products by offering storage for all data types (embeddings, audio, text, videos, images, pdfs, annotations, etc.), querying and vector search, data streaming while training models at scale, data versioning and lineage for all workloads, and integrations with popular tools such as LangChain, LlamaIndex, Weights and Biases, and many more. Deep Lake works with data of any size, it is serverless, and it enables you to store all of your data in once place. Deep Lake is used by Google, Intel, Airbus, Matterport, Red Cross, Yale, & Oxford. 
+Deep Lake is a Database for AI powered by a unique storage format optimized for deep-learning and Large Language Model (LLM) based applications. It simplifies the deployment of enterprise-grade LLM-based products by offering storage for all data types (embeddings, audio, text, videos, images, pdfs, annotations, etc.), querying and vector search, data streaming while training models at scale, data versioning and lineage for all workloads, and integrations with popular tools such as LangChain, LlamaIndex, Weights & Biases, and many more. Deep Lake works with data of any size, it is serverless, and it enables you to store all of your data in once place. Deep Lake is used by Intel, Airbus, Matterport, ZERO Systems, Red Cross, Yale, & Oxford. 
 
 Deep Lake includes the following features:
 
 <details>
   <summary><b>Storage Agnostic API</b></summary>
 Use one API to upload, download, and stream datasets to/from AWS S3/S3-compatible storage, GCP, Activeloop cloud, or local storage.
 </details>
@@ -292,22 +293,15 @@
 * **LLM Apps**
   * Use [Deep Lake as a vector store for LLM apps](https://www.activeloop.ai/resources/ultimate-guide-to-lang-chain-deep-lake-build-chat-gpt-to-answer-questions-on-your-financial-data/). Our integration combines the [Langchain](https://github.com/hwchase17/langchain) [VectorStores API](https://python.langchain.com/en/latest/reference/modules/vectorstore.html?highlight=pinecone#langchain.vectorstores.DeepLake) with Deep Lake datasets as the underlying data storage. The integration is a serverless vector store that can be deployed locally or in a cloud of your choice. 
 
 ## 📚 Documentation
 Getting started guides, examples, tutorials, API reference, and other useful information can be found on our [documentation page](http://docs.activeloop.ai/?utm_source=github&utm_medium=repo&utm_campaign=readme). 
 
 ## 🎓 For Students and Educators
-Deep Lake users can access and visualize a variety of popular datasets through a free integration with Activeloop's Platform. Users can also create and store their own datasets and make them available to the public. Free storage of up to 300 GB is available for students and educators:
-
-| <!-- -->    | <!-- -->    |
-| ---------------------------------------------------- | ------------- |
-| Storage for public datasets hosted by Activeloop     | 200GB Free    |
-| Storage for private datasets hosted by Activeloop    | 100GB Free    |
-
-
+Deep Lake users can access and visualize a variety of popular datasets through a free integration with Activeloop's Platform. Universities can get up to 1TB of data storage and 100,000 monthly queries on the Tensor Database for free per month. Chat in on [our website](https://activeloop.ai): to claim the access!
 
 ## 👩‍💻 Comparisons to Familiar Tools
 
 <details>
   <summary><b>Deep Lake vs Chroma </b></summary>
   
 Both Deep Lake & ChromaDB enable users to store and search vectors (embeddings) and offer integrations with LangChain and LlamaIndex. However, they are architecturally very different. ChromaDB is a Vector Database that can be deployed locally or on a server using Docker and will offer a hosted solution shortly. Deep Lake is a serverless Vector Store deployed on the user’s own cloud, locally, or in-memory. All computations run client-side, which enables users to support lightweight production apps in seconds. Unlike ChromaDB, Deep Lake’s data format can store raw data such as images, videos, and text, in addition to embeddings. ChromaDB is limited to light metadata on top of the embeddings and has no visualization. Deep Lake datasets can be visualized and version controlled. Deep Lake also has a performant dataloader for fine-tuning your Large Language Models. 
@@ -335,14 +329,25 @@
   
 Deep Lake and DVC offer dataset version control similar to git for data, but their methods for storing data differ significantly. Deep Lake converts and stores data as chunked compressed arrays, which enables rapid streaming to ML models, whereas DVC operates on top of data stored in less efficient traditional file structures. The Deep Lake format makes dataset versioning significantly easier compared to traditional file structures by DVC when datasets are composed of many files (i.e., many images). An additional distinction is that DVC primarily uses a command-line interface, whereas Deep Lake is a Python package. Lastly, Deep Lake offers an API to easily connect datasets to ML frameworks and other common ML tools and enables instant dataset visualization through [Activeloop's visualization tool](http://app.activeloop.ai/?utm_source=github&utm_medium=repo&utm_campaign=readme).
 
 </details>
 
 
 <details>
+  <summary><b>Deep Lake vs MosaicML MDS format </b></summary>
+  
+- **Data Storage Format:** Deep Lake operates on a columnar storage format, whereas MDS utilizes a row-wise storage approach. This fundamentally impacts how data is read, written, and organized in each system.
+- **Compression:** Deep Lake offers a more flexible compression scheme, allowing control over both chunk-level and sample-level compression for each column or tensor. This feature eliminates the need for additional compressions like zstd, which would otherwise demand more CPU cycles for decompressing on top of formats like jpeg.
+- **Shuffling:** MDS currently offers more advanced shuffling strategies.
+- **Version Control & Visualization Support:** A notable feature of Deep Lake is its native version control and in-browser data visualization, a feature not present for MosaicML data format. This can provide significant advantages in managing, understanding, and tracking different versions of the data.
+
+</details>
+
+
+<details>
   <summary><b>Deep Lake vs TensorFlow Datasets (TFDS)</b></summary>
   
 Deep Lake and TFDS seamlessly connect popular datasets to ML frameworks. Deep Lake datasets are compatible with both PyTorch and TensorFlow, whereas TFDS are only compatible with TensorFlow. A key difference between Deep Lake and TFDS is that Deep Lake datasets are designed for streaming from the cloud, whereas TFDS must be downloaded locally prior to use. As a result, with Deep Lake, one can import datasets directly from TensorFlow Datasets and stream them either to PyTorch or TensorFlow. In addition to providing access to popular publicly available datasets, Deep Lake also offers powerful tools for creating custom datasets, storing them on a variety of cloud storage providers, and collaborating with others via simple API. TFDS is primarily focused on giving the public easy access to commonly available datasets, and management of custom datasets is not the primary focus. A full comparison article can be found [here](https://www.activeloop.ai/resources/tensor-flow-tf-data-activeloop-hub-how-to-implement-your-tensor-flow-data-pipelines-with-hub/).
 
 </details>
```

#### html2text {}

```diff
@@ -1,45 +1,45 @@
-Metadata-Version: 2.1 Name: deeplake Version: 3.5.4 Summary: Activeloop Deep
+Metadata-Version: 2.1 Name: deeplake Version: 3.6.0 Summary: Activeloop Deep
 Lake Home-page: UNKNOWN Author: activeloop.ai Author-email:
 support@activeloop.ai License: MPL-2.0 Project-URL: Documentation, https://
 docs.activeloop.ai/ Project-URL: Source, https://github.com/activeloopai/
 deeplake Platform: UNKNOWN Classifier: License :: OSI Approved :: Mozilla
 Public License 2.0 (MPL 2.0) Description-Content-Type: text/markdown Provides-
-Extra: all Provides-Extra: audio Provides-Extra: av Provides-Extra: dicom
-Provides-Extra: enterprise Provides-Extra: gcp Provides-Extra: gdrive Provides-
-Extra: medical Provides-Extra: point_cloud Provides-Extra: video Provides-
-Extra: visualizer License-File: LICENSE [https://static.scarf.sh/a.png?x-
-pxid=bc3c57b0-9a65-49fe-b8ea-f711c4d35b82]
+Extra: all Provides-Extra: audio Provides-Extra: av Provides-Extra: azure
+Provides-Extra: dicom Provides-Extra: enterprise Provides-Extra: gcp Provides-
+Extra: gdrive Provides-Extra: medical Provides-Extra: point_cloud Provides-
+Extra: video Provides-Extra: visualizer License-File: LICENSE [https://
+static.scarf.sh/a.png?x-pxid=bc3c57b0-9a65-49fe-b8ea-f711c4d35b82]
                [https://i.postimg.cc/rsjcWc3S/deeplake-logo.png]
-           ****** Deep Lake: Vector Database for any AI data ******
+                   ****** Deep Lake: Database for AI ******
   [PyPI_version] [PyPI_version] [Documentation_Status] [PyPI_version] [GitHub
                                issues] [codecov]
    **** Documentation • Getting_Started • API_Reference • Examples • Blog •
                   Whitepaper • Slack_Community • Twitter ****
 *Read this in other languages: [ç®ä½ä¸­æ](README.zh-cn.md)* ## About Deep
-Lake Deep Lake is a Vector Database powered by a unique storage format
+Lake Deep Lake is a Database for AI powered by a unique storage format
 optimized for deep-learning and Large Language Model (LLM) based applications.
 It simplifies the deployment of enterprise-grade LLM-based products by offering
 storage for all data types (embeddings, audio, text, videos, images, pdfs,
 annotations, etc.), querying and vector search, data streaming while training
 models at scale, data versioning and lineage for all workloads, and
-integrations with popular tools such as LangChain, LlamaIndex, Weights and
+integrations with popular tools such as LangChain, LlamaIndex, Weights &
 Biases, and many more. Deep Lake works with data of any size, it is serverless,
 and it enables you to store all of your data in once place. Deep Lake is used
-by Google, Intel, Airbus, Matterport, Red Cross, Yale, & Oxford. Deep Lake
-includes the following features:  Storage Agnostic API Use one API to upload,
-download, and stream datasets to/from AWS S3/S3-compatible storage, GCP,
-Activeloop cloud, or local storage.   Native Compression with Lazy NumPy-like
-Indexing Store images, audios and videos in their native compression. Slide,
-index, iterate and interact with your data like a collection of NumPy arrays in
-your system's memory. Deep Lake lazily loads data only when needed, e.g., when
-training a model.   Dataset Version Control Commits, branches, checkout -
-Concepts you are already familiar with in your code repositories can now be
-applied to your datasets as well!   Dataloaders for Popular Deep Learning
-Frameworks Deep Lake comes with built-in dataloaders for Pytorch and
+by Intel, Airbus, Matterport, ZERO Systems, Red Cross, Yale, & Oxford. Deep
+Lake includes the following features:  Storage Agnostic API Use one API to
+upload, download, and stream datasets to/from AWS S3/S3-compatible storage,
+GCP, Activeloop cloud, or local storage.   Native Compression with Lazy NumPy-
+like Indexing Store images, audios and videos in their native compression.
+Slide, index, iterate and interact with your data like a collection of NumPy
+arrays in your system's memory. Deep Lake lazily loads data only when needed,
+e.g., when training a model.   Dataset Version Control Commits, branches,
+checkout - Concepts you are already familiar with in your code repositories can
+now be applied to your datasets as well!   Dataloaders for Popular Deep
+Learning Frameworks Deep Lake comes with built-in dataloaders for Pytorch and
 Tensorflow. Train your model with a few lines of code - we even take care of
 dataset shuffling. :)   Integrations with Powerful Tools Deep Lake has
 integrations with Langchain and LLamaIndex as a vector store for LLM apps,
 Weights_&_Biases for data lineage during model training, and MMDetection for
 training object detection models.   Distributed Transformations Rapidly apply
 transformations on your datasets using multi-threading, multi-processing, or
 our built-in Ray integration.  100+ most-popular image, video, and audio
@@ -138,97 +138,107 @@
 Lake datasets as the underlying data storage. The integration is a serverless
 vector store that can be deployed locally or in a cloud of your choice. ## ð
 Documentation Getting started guides, examples, tutorials, API reference, and
 other useful information can be found on our [documentation page](http://
 docs.activeloop.ai/?utm_source=github&utm_medium=repo&utm_campaign=readme). ##
 ð For Students and Educators Deep Lake users can access and visualize a
 variety of popular datasets through a free integration with Activeloop's
-Platform. Users can also create and store their own datasets and make them
-available to the public. Free storage of up to 300 GB is available for students
-and educators: |  |  | | ---------------------------------------------------- |
-------------- | | Storage for public datasets hosted by Activeloop | 200GB Free
-| | Storage for private datasets hosted by Activeloop | 100GB Free | ##
-ð©âð» Comparisons to Familiar Tools  Deep Lake vs Chroma Both Deep Lake &
-ChromaDB enable users to store and search vectors (embeddings) and offer
-integrations with LangChain and LlamaIndex. However, they are architecturally
-very different. ChromaDB is a Vector Database that can be deployed locally or
-on a server using Docker and will offer a hosted solution shortly. Deep Lake is
-a serverless Vector Store deployed on the userâs own cloud, locally, or in-
-memory. All computations run client-side, which enables users to support
-lightweight production apps in seconds. Unlike ChromaDB, Deep Lakeâs data
-format can store raw data such as images, videos, and text, in addition to
-embeddings. ChromaDB is limited to light metadata on top of the embeddings and
-has no visualization. Deep Lake datasets can be visualized and version
-controlled. Deep Lake also has a performant dataloader for fine-tuning your
-Large Language Models.   Deep Lake vs Pinecone Both Deep Lake and Pinecone
-enable users to store and search vectors (embeddings) and offer integrations
-with LangChain and LlamaIndex. However, they are architecturally very
-different. Pinecone is a fully-managed Vector Database that is optimized for
-highly demanding applications requiring search for billions of vectors. Deep
-Lake is a serverless. All computations run client-side, which enables users to
-get started in seconds. Unlike Pinecone, Deep Lakeâs data format can store
-raw data such as images, videos, and text, in addition to embeddings. Deep Lake
-datasets can be visualized and version controlled. Pinecone is limited to light
-metadata on top of the embeddings and has no visualization. Deep Lake also has
-a performant dataloader for fine-tuning your Large Language Models.   Deep Lake
-vs Weaviate Both Deep Lake and Weaviate enable users to store and search
+Platform. Universities can get up to 1TB of data storage and 100,000 monthly
+queries on the Tensor Database for free per month. Chat in on [our website]
+(https://activeloop.ai): to claim the access! ## ð©âð» Comparisons to
+Familiar Tools  Deep Lake vs Chroma Both Deep Lake & ChromaDB enable users to
+store and search vectors (embeddings) and offer integrations with LangChain and
+LlamaIndex. However, they are architecturally very different. ChromaDB is a
+Vector Database that can be deployed locally or on a server using Docker and
+will offer a hosted solution shortly. Deep Lake is a serverless Vector Store
+deployed on the userâs own cloud, locally, or in-memory. All computations run
+client-side, which enables users to support lightweight production apps in
+seconds. Unlike ChromaDB, Deep Lakeâs data format can store raw data such as
+images, videos, and text, in addition to embeddings. ChromaDB is limited to
+light metadata on top of the embeddings and has no visualization. Deep Lake
+datasets can be visualized and version controlled. Deep Lake also has a
+performant dataloader for fine-tuning your Large Language Models.   Deep Lake
+vs Pinecone Both Deep Lake and Pinecone enable users to store and search
 vectors (embeddings) and offer integrations with LangChain and LlamaIndex.
-However, they are architecturally very different. Weaviate is a Vector Database
-that can be deployed in a managed service or by the user via Kubernetes or
-Docker. Deep Lake is serverless. All computations run client-side, which
-enables users to support lightweight production apps in seconds. Unlike
-Weaviate, Deep Lakeâs data format can store raw data such as images, videos,
-and text, in addition to embeddings. Deep Lake datasets can be visualized and
-version controlled. Weaviate is limited to light metadata on top of the
-embeddings and has no visualization. Deep Lake also has a performant dataloader
-for fine-tuning your Large Language Models.   Deep Lake vs DVC Deep Lake and
-DVC offer dataset version control similar to git for data, but their methods
-for storing data differ significantly. Deep Lake converts and stores data as
-chunked compressed arrays, which enables rapid streaming to ML models, whereas
-DVC operates on top of data stored in less efficient traditional file
-structures. The Deep Lake format makes dataset versioning significantly easier
-compared to traditional file structures by DVC when datasets are composed of
-many files (i.e., many images). An additional distinction is that DVC primarily
-uses a command-line interface, whereas Deep Lake is a Python package. Lastly,
-Deep Lake offers an API to easily connect datasets to ML frameworks and other
-common ML tools and enables instant dataset visualization through [Activeloop's
-visualization tool](http://app.activeloop.ai/
-?utm_source=github&utm_medium=repo&utm_campaign=readme).   Deep Lake vs
-TensorFlow Datasets (TFDS) Deep Lake and TFDS seamlessly connect popular
-datasets to ML frameworks. Deep Lake datasets are compatible with both PyTorch
-and TensorFlow, whereas TFDS are only compatible with TensorFlow. A key
-difference between Deep Lake and TFDS is that Deep Lake datasets are designed
-for streaming from the cloud, whereas TFDS must be downloaded locally prior to
-use. As a result, with Deep Lake, one can import datasets directly from
-TensorFlow Datasets and stream them either to PyTorch or TensorFlow. In
-addition to providing access to popular publicly available datasets, Deep Lake
-also offers powerful tools for creating custom datasets, storing them on a
-variety of cloud storage providers, and collaborating with others via simple
-API. TFDS is primarily focused on giving the public easy access to commonly
-available datasets, and management of custom datasets is not the primary focus.
-A full comparison article can be found [here](https://www.activeloop.ai/
-resources/tensor-flow-tf-data-activeloop-hub-how-to-implement-your-tensor-flow-
-data-pipelines-with-hub/).   Deep Lake vs HuggingFace Deep Lake and HuggingFace
-offer access to popular datasets, but Deep Lake primarily focuses on computer
-vision, whereas HuggingFace focuses on natural language processing. HuggingFace
-Transforms and other computational tools for NLP are not analogous to features
-offered by Deep Lake.   Deep Lake vs WebDatasets Deep Lake and WebDatasets both
-offer rapid data streaming across networks. They have nearly identical steaming
-speeds because the underlying network requests and data structures are very
-similar. However, Deep Lake offers superior random access and shuffling, its
-simple API is in python instead of command-line, and Deep Lake enables simple
-indexing and modification of the dataset without having to recreate it.   Deep
-Lake vs Zarr Deep Lake and Zarr both offer storage of data as chunked arrays.
-However, Deep Lake is primarily designed for returning data as arrays using a
-simple API, rather than actually storing raw arrays (even though that's also
-possible). Deep Lake stores data in use-case-optimized formats, such as jpeg or
-png for images, or mp4 for video, and the user treats the data as if it's an
-array, because Deep Lake handles all the data processing in between. Deep Lake
-offers more flexibility for storing arrays with dynamic shape (ragged tensors),
-and it provides several features that are not naively available in Zarr such as
+However, they are architecturally very different. Pinecone is a fully-managed
+Vector Database that is optimized for highly demanding applications requiring
+search for billions of vectors. Deep Lake is a serverless. All computations run
+client-side, which enables users to get started in seconds. Unlike Pinecone,
+Deep Lakeâs data format can store raw data such as images, videos, and text,
+in addition to embeddings. Deep Lake datasets can be visualized and version
+controlled. Pinecone is limited to light metadata on top of the embeddings and
+has no visualization. Deep Lake also has a performant dataloader for fine-
+tuning your Large Language Models.   Deep Lake vs Weaviate Both Deep Lake and
+Weaviate enable users to store and search vectors (embeddings) and offer
+integrations with LangChain and LlamaIndex. However, they are architecturally
+very different. Weaviate is a Vector Database that can be deployed in a managed
+service or by the user via Kubernetes or Docker. Deep Lake is serverless. All
+computations run client-side, which enables users to support lightweight
+production apps in seconds. Unlike Weaviate, Deep Lakeâs data format can
+store raw data such as images, videos, and text, in addition to embeddings.
+Deep Lake datasets can be visualized and version controlled. Weaviate is
+limited to light metadata on top of the embeddings and has no visualization.
+Deep Lake also has a performant dataloader for fine-tuning your Large Language
+Models.   Deep Lake vs DVC Deep Lake and DVC offer dataset version control
+similar to git for data, but their methods for storing data differ
+significantly. Deep Lake converts and stores data as chunked compressed arrays,
+which enables rapid streaming to ML models, whereas DVC operates on top of data
+stored in less efficient traditional file structures. The Deep Lake format
+makes dataset versioning significantly easier compared to traditional file
+structures by DVC when datasets are composed of many files (i.e., many images).
+An additional distinction is that DVC primarily uses a command-line interface,
+whereas Deep Lake is a Python package. Lastly, Deep Lake offers an API to
+easily connect datasets to ML frameworks and other common ML tools and enables
+instant dataset visualization through [Activeloop's visualization tool](http://
+app.activeloop.ai/?utm_source=github&utm_medium=repo&utm_campaign=readme).
+Deep Lake vs MosaicML MDS format - **Data Storage Format:** Deep Lake operates
+on a columnar storage format, whereas MDS utilizes a row-wise storage approach.
+This fundamentally impacts how data is read, written, and organized in each
+system. - **Compression:** Deep Lake offers a more flexible compression scheme,
+allowing control over both chunk-level and sample-level compression for each
+column or tensor. This feature eliminates the need for additional compressions
+like zstd, which would otherwise demand more CPU cycles for decompressing on
+top of formats like jpeg. - **Shuffling:** MDS currently offers more advanced
+shuffling strategies. - **Version Control & Visualization Support:** A notable
+feature of Deep Lake is its native version control and in-browser data
+visualization, a feature not present for MosaicML data format. This can provide
+significant advantages in managing, understanding, and tracking different
+versions of the data.   Deep Lake vs TensorFlow Datasets (TFDS) Deep Lake and
+TFDS seamlessly connect popular datasets to ML frameworks. Deep Lake datasets
+are compatible with both PyTorch and TensorFlow, whereas TFDS are only
+compatible with TensorFlow. A key difference between Deep Lake and TFDS is that
+Deep Lake datasets are designed for streaming from the cloud, whereas TFDS must
+be downloaded locally prior to use. As a result, with Deep Lake, one can import
+datasets directly from TensorFlow Datasets and stream them either to PyTorch or
+TensorFlow. In addition to providing access to popular publicly available
+datasets, Deep Lake also offers powerful tools for creating custom datasets,
+storing them on a variety of cloud storage providers, and collaborating with
+others via simple API. TFDS is primarily focused on giving the public easy
+access to commonly available datasets, and management of custom datasets is not
+the primary focus. A full comparison article can be found [here](https://
+www.activeloop.ai/resources/tensor-flow-tf-data-activeloop-hub-how-to-
+implement-your-tensor-flow-data-pipelines-with-hub/).   Deep Lake vs
+HuggingFace Deep Lake and HuggingFace offer access to popular datasets, but
+Deep Lake primarily focuses on computer vision, whereas HuggingFace focuses on
+natural language processing. HuggingFace Transforms and other computational
+tools for NLP are not analogous to features offered by Deep Lake.   Deep Lake
+vs WebDatasets Deep Lake and WebDatasets both offer rapid data streaming across
+networks. They have nearly identical steaming speeds because the underlying
+network requests and data structures are very similar. However, Deep Lake
+offers superior random access and shuffling, its simple API is in python
+instead of command-line, and Deep Lake enables simple indexing and modification
+of the dataset without having to recreate it.   Deep Lake vs Zarr Deep Lake and
+Zarr both offer storage of data as chunked arrays. However, Deep Lake is
+primarily designed for returning data as arrays using a simple API, rather than
+actually storing raw arrays (even though that's also possible). Deep Lake
+stores data in use-case-optimized formats, such as jpeg or png for images, or
+mp4 for video, and the user treats the data as if it's an array, because Deep
+Lake handles all the data processing in between. Deep Lake offers more
+flexibility for storing arrays with dynamic shape (ragged tensors), and it
+provides several features that are not naively available in Zarr such as
 version control, data streaming, and connecting data to ML Frameworks.  ##
 Community Join our [**Slack community**](https://join.slack.com/t/hubdb/
 shared_invite/zt-ivhsj8sz-GWv9c5FLBDVw8vn~sxRKqQ) to learn more about
 unstructured dataset management using Deep Lake and to get help from the
 Activeloop team and other users. We'd love your feedback by completing our 3-
 minute [**survey**](https://forms.gle/rLi4w33dow6CSMcm9). As always, thanks to
 our amazing contributors! [https://contrib.rocks/image?repo=activeloopai/hub]
```

### Comparing `deeplake-3.5.4/deeplake.egg-info/SOURCES.txt` & `deeplake-3.6.0/deeplake.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -155,14 +155,15 @@
 deeplake/core/meta/encode/tests/test_shape_encoder.py
 deeplake/core/meta/encode/tests/test_shape_encoder_updates.py
 deeplake/core/query/__init__.py
 deeplake/core/query/autocomplete.py
 deeplake/core/query/filter.py
 deeplake/core/query/query.py
 deeplake/core/storage/__init__.py
+deeplake/core/storage/azure.py
 deeplake/core/storage/deeplake_memory_object.py
 deeplake/core/storage/gcs.py
 deeplake/core/storage/google_drive.py
 deeplake/core/storage/local.py
 deeplake/core/storage/lru_cache.py
 deeplake/core/storage/memory.py
 deeplake/core/storage/provider.py
@@ -196,26 +197,27 @@
 deeplake/core/vectorstore/vector_search/dataset/__init__.py
 deeplake/core/vectorstore/vector_search/dataset/dataset.py
 deeplake/core/vectorstore/vector_search/dataset/test_dataset.py
 deeplake/core/vectorstore/vector_search/filter/__init__.py
 deeplake/core/vectorstore/vector_search/filter/filter.py
 deeplake/core/vectorstore/vector_search/filter/test_filter.py
 deeplake/core/vectorstore/vector_search/indra/__init__.py
-deeplake/core/vectorstore/vector_search/indra/indra_vector_search.py
 deeplake/core/vectorstore/vector_search/indra/query.py
-deeplake/core/vectorstore/vector_search/indra/remote_engine_search.py
+deeplake/core/vectorstore/vector_search/indra/search_algorithm.py
 deeplake/core/vectorstore/vector_search/indra/test_indra.py
+deeplake/core/vectorstore/vector_search/indra/vector_search.py
 deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/__init__.py
 deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py
 deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/order.py
 deeplake/core/vectorstore/vector_search/ingestion/__init__.py
 deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py
 deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py
 deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py
 deeplake/core/vectorstore/vector_search/python/__init__.py
+deeplake/core/vectorstore/vector_search/python/search_algorithm.py
 deeplake/core/vectorstore/vector_search/python/test_vector_search.py
 deeplake/core/vectorstore/vector_search/python/vector_search.py
 deeplake/core/version_control/__init__.py
 deeplake/core/version_control/commit_chunk_map.py
 deeplake/core/version_control/commit_diff.py
 deeplake/core/version_control/commit_node.py
 deeplake/core/version_control/dataset_diff.py
@@ -306,14 +308,15 @@
 deeplake/util/scheduling.py
 deeplake/util/shape_interval.py
 deeplake/util/shuffle.py
 deeplake/util/spinner.py
 deeplake/util/split.py
 deeplake/util/storage.py
 deeplake/util/tag.py
+deeplake/util/tensor_db.py
 deeplake/util/testing.py
 deeplake/util/threading.py
 deeplake/util/token.py
 deeplake/util/transform.py
 deeplake/util/version_control.py
 deeplake/util/video.py
 deeplake/util/warnings.py
@@ -334,12 +337,13 @@
 deeplake/util/tests/test_auto.py
 deeplake/util/tests/test_connect_dataset.py
 deeplake/util/tests/test_iterable_ordered_dict.py
 deeplake/util/tests/test_read.py
 deeplake/util/tests/test_shape_interval.py
 deeplake/util/tests/test_shuffle.py
 deeplake/util/tests/test_split.py
+deeplake/util/tests/test_tensor_db.py
 deeplake/util/tests/test_token.py
 deeplake/util/tests/test_version_control.py
 deeplake/visualizer/__init__.py
 deeplake/visualizer/video_streaming.py
 deeplake/visualizer/visualizer.py
```

### Comparing `deeplake-3.5.4/deeplake.egg-info/requires.txt` & `deeplake-3.6.0/deeplake.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -10,21 +10,24 @@
 
 [:python_version >= "3.7" and sys_platform != "win32"]
 aioboto3>=10.4.0
 nest_asyncio
 
 [all]
 IPython
+azure-cli
+azure-identity
+azure-storage-blob
 flask
 google-api-python-client~=2.31.0
 google-auth-oauthlib~=0.4.5
 google-auth~=2.0.1
 google-cloud-storage~=1.42.0
 laspy
-libdeeplake==0.0.54
+libdeeplake==0.0.55
 nibabel
 oauth2client~=4.1.3
 pydicom
 
 [all:python_version >= "3.7" or sys_platform != "win32"]
 av>=8.1.0
 
@@ -34,20 +37,25 @@
 av>=8.1.0
 
 [av]
 
 [av:python_version >= "3.7" or sys_platform != "win32"]
 av>=8.1.0
 
+[azure]
+azure-cli
+azure-identity
+azure-storage-blob
+
 [dicom]
 nibabel
 pydicom
 
 [enterprise]
-libdeeplake==0.0.54
+libdeeplake==0.0.55
 pyjwt
 
 [gcp]
 google-auth-oauthlib~=0.4.5
 google-auth~=2.0.1
 google-cloud-storage~=1.42.0
```

### Comparing `deeplake-3.5.4/setup.py` & `deeplake-3.6.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
 # Add optional dependencies to this dict without version. Version should be specified in requirements.txt
 extras = {
     "audio": ["av"],
     "video": ["av"],
     "av": ["av"],
     "gcp": ["google-cloud-storage", "google-auth", "google-auth-oauthlib"],
+    "azure": ["azure-cli", "azure-identity", "azure-storage-blob"],
     "dicom": ["pydicom", "nibabel"],
     "medical": ["pydicom", "nibabel"],
     "visualizer": ["IPython", "flask"],
     "gdrive": [
         "google-api-python-client",
         "oauth2client",
         "google-auth",
@@ -65,15 +66,15 @@
 all_extras = {r for v in extras.values() for r in v}
 install_requires = [req_map[r] for r in req_map if r not in all_extras]
 extras_require = {k: [req_map[r] for r in v] for k, v in extras.items()}
 
 extras_require["all"] = [req_map[r] for r in all_extras]
 
 if libdeeplake_availabe():
-    libdeeplake = "libdeeplake==0.0.54"
+    libdeeplake = "libdeeplake==0.0.55"
     extras_require["enterprise"] = [libdeeplake, "pyjwt"]
     extras_require["all"].append(libdeeplake)
 
 init_file = os.path.join(project_name, "__init__.py")
 
 
 def get_property(prop):
```

