# Comparing `tmp/truss-0.4.6rc3.tar.gz` & `tmp/truss-0.4.8rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truss-0.4.6rc3.tar", max compression
+gzip compressed data, was "truss-0.4.8rc4.tar", max compression
```

## Comparing `truss-0.4.6rc3.tar` & `truss-0.4.8rc4.tar`

### file list

```diff
@@ -1,169 +1,174 @@
--rw-r--r--   0        0        0     5483 2023-05-17 18:43:25.064890 truss-0.4.6rc3/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2576 2023-05-17 18:43:25.064890 truss-0.4.6rc3/CONTRIBUTING.md
--rw-r--r--   0        0        0     1064 2023-05-17 18:43:25.064890 truss-0.4.6rc3/LICENSE
--rw-r--r--   0        0        0     5958 2023-05-17 18:43:25.064890 truss-0.4.6rc3/README.md
--rw-r--r--   0        0        0     3316 2023-05-17 18:43:25.064890 truss-0.4.6rc3/ROADMAP.md
--rw-r--r--   0        0        0      625 2023-05-17 18:43:25.064890 truss-0.4.6rc3/context_builder.Dockerfile
--rw-r--r--   0        0        0     2244 2023-05-17 18:43:25.156895 truss-0.4.6rc3/pyproject.toml
--rw-r--r--   0        0        0      330 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/__init__.py
--rw-r--r--   0        0        0      252 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/blob/blob_backend.py
--rw-r--r--   0        0        0      733 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/blob/blob_backend_registry.py
--rw-r--r--   0        0        0      648 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/blob/http_public_blob_backend.py
--rw-r--r--   0        0        0    13295 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/build.py
--rw-r--r--   0        0        0    10452 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/cli.py
--rw-r--r--   0        0        0     2813 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/constants.py
--rw-r--r--   0        0        0     1294 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/contexts/image_builder/image_builder.py
--rw-r--r--   0        0        0     5709 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/contexts/image_builder/serving_image_builder.py
--rw-r--r--   0        0        0     4770 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/contexts/image_builder/training_image_builder.py
--rw-r--r--   0        0        0     1976 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/contexts/image_builder/util.py
--rw-r--r--   0        0        0     1686 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/contexts/local_loader/load_model_local.py
--rw-r--r--   0        0        0     2239 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/contexts/local_loader/train_local.py
--rw-r--r--   0        0        0     5801 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/contexts/local_loader/truss_module_loader.py
--rw-r--r--   0        0        0      853 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/contexts/local_loader/utils.py
--rw-r--r--   0        0        0      436 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/contexts/truss_context.py
--rw-r--r--   0        0        0      394 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/decorators.py
--rw-r--r--   0        0        0     3641 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/docker.py
--rw-r--r--   0        0        0     3759 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/environment_inference/requirements_inference.py
--rw-r--r--   0        0        0      643 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/errors.py
--rw-r--r--   0        0        0      824 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/local/local_config.py
--rw-r--r--   0        0        0     3896 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/local/local_config_handler.py
--rw-r--r--   0        0        0     2713 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/model_framework.py
--rw-r--r--   0        0        0     1687 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/model_frameworks/__init__.py
--rw-r--r--   0        0        0     1895 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/model_frameworks/huggingface_transformer.py
--rw-r--r--   0        0        0      918 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/model_frameworks/keras.py
--rw-r--r--   0        0        0     1237 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/model_frameworks/lightgbm.py
--rw-r--r--   0        0        0     2410 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/model_frameworks/mlflow.py
--rw-r--r--   0        0        0     2441 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/model_frameworks/pytorch.py
--rw-r--r--   0        0        0     1232 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/model_frameworks/sklearn.py
--rw-r--r--   0        0        0     1027 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/model_frameworks/xgboost.py
--rw-r--r--   0        0        0     6565 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/model_inference.py
--rw-r--r--   0        0        0      510 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/notebook.py
--rw-r--r--   0        0        0    11065 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/patch/calc_patch.py
--rw-r--r--   0        0        0      774 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/patch/dir_signature.py
--rw-r--r--   0        0        0     2378 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/patch/hash.py
--rw-r--r--   0        0        0      468 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/patch/signature.py
--rw-r--r--   0        0        0      937 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/patch/types.py
--rw-r--r--   0        0        0      237 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/pytest.ini
--rw-r--r--   0        0        0      705 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/readme_generator.py
--rw-r--r--   0        0        0     2482 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/README.md.jinja
--rw-r--r--   0        0        0        0 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/__init__.py
--rw-r--r--   0        0        0     2170 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/base.Dockerfile.jinja
--rw-r--r--   0        0        0     2190 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/control/control/application.py
--rw-r--r--   0        0        0     4083 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/control/control/endpoints.py
--rw-r--r--   0        0        0      413 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/control/control/helpers/context_managers.py
--rw-r--r--   0        0        0      877 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/control/control/helpers/errors.py
--rw-r--r--   0        0        0     5801 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/control/control/helpers/inference_server_controller.py
--rw-r--r--   0        0        0     2596 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/control/control/helpers/inference_server_process_controller.py
--rw-r--r--   0        0        0     2399 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/control/control/helpers/inference_server_starter.py
--rw-r--r--   0        0        0     5389 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/control/control/helpers/patch_applier.py
--rw-r--r--   0        0        0     3070 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/control/control/helpers/types.py
--rw-r--r--   0        0        0     1849 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/control/control/server.py
--rw-r--r--   0        0        0       82 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/control/requirements.txt
--rw-r--r--   0        0        0       48 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/custom/examples.yaml
--rw-r--r--   0        0        0        0 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/custom/model/__init__.py
--rw-r--r--   0        0        0      534 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/custom/model/model.py
--rw-r--r--   0        0        0      460 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/custom/train/train.py
--rw-r--r--   0        0        0     2616 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/docs/README.md
--rw-r--r--   0        0        0        0 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/huggingface_transformer/model/__init__.py
--rw-r--r--   0        0        0     1827 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/huggingface_transformer/model/model.py
--rw-r--r--   0        0        0       47 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/huggingface_transformer/requirements.txt
--rw-r--r--   0        0        0        0 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/keras/model/__init__.py
--rw-r--r--   0        0        0      728 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/keras/model/model.py
--rw-r--r--   0        0        0        0 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/lightgbm/model/__init__.py
--rw-r--r--   0        0        0     1251 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/lightgbm/model/model.py
--rw-r--r--   0        0        0        0 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/mlflow/model/__init__.py
--rw-r--r--   0        0        0      751 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/mlflow/model/model.py
--rw-r--r--   0        0        0        0 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/pipeline/model/__init__.py
--rw-r--r--   0        0        0      430 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/pipeline/model/model.py
--rw-r--r--   0        0        0        0 2023-05-17 18:43:25.156895 truss-0.4.6rc3/truss/templates/pytorch/model/__init__.py
--rw-r--r--   0        0        0     1263 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/templates/pytorch/model/model.py
--rw-r--r--   0        0        0        0 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/templates/server/__init__.py
--rw-r--r--   0        0        0       85 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/templates/server/common/__init__.py
--rw-r--r--   0        0        0      237 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/templates/server/common/errors.py
--rw-r--r--   0        0        0     1892 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/templates/server/common/external_data_resolver.py
--rw-r--r--   0        0        0     1352 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/templates/server/common/logging.py
--rw-r--r--   0        0        0      593 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/templates/server/common/retry.py
--rw-r--r--   0        0        0     3318 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/templates/server/common/serialization.py
--rw-r--r--   0        0        0     5511 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/templates/server/common/truss_server.py
--rw-r--r--   0        0        0      416 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/templates/server/common/util.py
--rw-r--r--   0        0        0      733 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/templates/server/inference_server.py
--rw-r--r--   0        0        0     5674 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/templates/server/model_wrapper.py
--rw-r--r--   0        0        0      176 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/templates/server/requirements.txt
--rw-r--r--   0        0        0     2327 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/templates/server.Dockerfile.jinja
--rw-r--r--   0        0        0      138 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/templates/shared/README.md
--rw-r--r--   0        0        0        0 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/templates/shared/__init__.py
--rw-r--r--   0        0        0     1430 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/templates/shared/secrets_resolver.py
--rw-r--r--   0        0        0        0 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/templates/sklearn/model/__init__.py
--rw-r--r--   0        0        0     1221 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/templates/sklearn/model/model.py
--rw-r--r--   0        0        0     3400 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/templates/training/job.py
--rw-r--r--   0        0        0       12 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/templates/training/requirements.txt
--rw-r--r--   0        0        0      491 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/templates/training.Dockerfile.jinja
--rw-r--r--   0        0        0        0 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/templates/xgboost/model/__init__.py
--rw-r--r--   0        0        0     1453 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/templates/xgboost/model/model.py
--rw-r--r--   0        0        0    30286 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/test_data/auto-mpg.data
--rw-r--r--   0        0        0      216 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/test_data/context_builder_image_test/Dockerfile
--rw-r--r--   0        0        0     2253 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/test_data/context_builder_image_test/server.Dockerfile
--rw-r--r--   0        0        0       72 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/test_data/context_builder_image_test/test.py
--rw-r--r--   0        0        0     1394 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/test_data/happy.ipynb
--rw-r--r--   0        0        0     1267 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/test_data/patch_ping_test_server/app.py
--rw-r--r--   0        0        0    23279 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/test_data/pima-indians-diabetes.csv
--rw-r--r--   0        0        0     1586 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/test_data/readme_int_example.md
--rw-r--r--   0        0        0     1607 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/test_data/readme_no_example.md
--rw-r--r--   0        0        0     1726 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/test_data/readme_str_example.md
--rw-r--r--   0        0        0      669 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/test_data/test_truss/config.yaml
--rw-r--r--   0        0        0       48 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/test_data/test_truss/examples.yaml
--rw-r--r--   0        0        0        0 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/test_data/test_truss/model/__init__.py
--rw-r--r--   0        0        0        0 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/test_data/test_truss/model/dummy
--rw-r--r--   0        0        0      534 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/test_data/test_truss/model/model.py
--rw-r--r--   0        0        0        0 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/__init__.py
--rw-r--r--   0        0        0    20835 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/conftest.py
--rw-r--r--   0        0        0     1256 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/contexts/image_builder/test_serving_image_builder.py
--rw-r--r--   0        0        0      783 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/contexts/local_loader/test_load_local.py
--rw-r--r--   0        0        0     5337 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/contexts/local_loader/test_truss_module_finder.py
--rw-r--r--   0        0        0      968 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/environments_inference/test_requirements_inference.py
--rw-r--r--   0        0        0        0 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/local/__init__.py
--rw-r--r--   0        0        0     2245 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/local/test_local_config_handler.py
--rw-r--r--   0        0        0        0 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/model_frameworks/__init__.py
--rw-r--r--   0        0        0     3293 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/model_frameworks/test_huggingface_transformer_framework.py
--rw-r--r--   0        0        0     2789 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/model_frameworks/test_keras_framework.py
--rw-r--r--   0        0        0     2409 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/model_frameworks/test_lightgbm_framework.py
--rw-r--r--   0        0        0     1479 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/model_frameworks/test_pytorch_framework.py
--rw-r--r--   0        0        0     2427 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/model_frameworks/test_sklearn_framework.py
--rw-r--r--   0        0        0     2437 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/model_frameworks/test_xgboost_framework.py
--rw-r--r--   0        0        0    11109 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/patch/test_calc_patch.py
--rw-r--r--   0        0        0      487 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/patch/test_dir_signature.py
--rw-r--r--   0        0        0     5983 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/patch/test_hash.py
--rw-r--r--   0        0        0      394 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/patch/test_signature.py
--rw-r--r--   0        0        0      273 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/patch/test_types.py
--rw-r--r--   0        0        0    10415 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/samples.py
--rw-r--r--   0        0        0      283 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/templates/control/control/helpers/test_context_managers.py
--rw-r--r--   0        0        0     1976 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/templates/control/control/helpers/test_patch_applier.py
--rw-r--r--   0        0        0     6937 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/templates/control/control/test_server.py
--rw-r--r--   0        0        0      750 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/templates/core/server/common/test_util.py
--rw-r--r--   0        0        0     1539 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/templates/core/server/test_secrets_resolver.py
--rw-r--r--   0        0        0     2157 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/templates/server/common/test_external_resolver.py
--rw-r--r--   0        0        0     2038 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/templates/server/common/test_retry.py
--rw-r--r--   0        0        0     2252 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/templates/server/test_model_wrapper.py
--rw-r--r--   0        0        0     1910 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/test_backward.py
--rw-r--r--   0        0        0     8260 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/test_build.py
--rw-r--r--   0        0        0     2359 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/test_config.py
--rw-r--r--   0        0        0     1188 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/test_context_builder_image.py
--rw-r--r--   0        0        0      517 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/test_docker.py
--rw-r--r--   0        0        0     2605 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/test_model_inference.py
--rw-r--r--   0        0        0      656 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/test_notebooks.py
--rw-r--r--   0        0        0     1483 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/test_testing_utilities_for_other_tests.py
--rw-r--r--   0        0        0     1252 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/test_truss_gatherer.py
--rw-r--r--   0        0        0    33226 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/test_truss_handle.py
--rw-r--r--   0        0        0      434 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/test_truss_util.py
--rw-r--r--   0        0        0     1865 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/tests/test_validation.py
--rw-r--r--   0        0        0    12200 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/truss_config.py
--rw-r--r--   0        0        0     2845 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/truss_gatherer.py
--rw-r--r--   0        0        0    41070 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/truss_handle.py
--rw-r--r--   0        0        0     5428 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/truss_spec.py
--rw-r--r--   0        0        0     2124 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/types.py
--rw-r--r--   0        0        0      227 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/util/data_structures.py
--rw-r--r--   0        0        0      553 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/util/gpu.py
--rw-r--r--   0        0        0      333 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/util/jinja.py
--rw-r--r--   0        0        0     2018 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/util/path.py
--rw-r--r--   0        0        0     2317 2023-05-17 18:43:25.160895 truss-0.4.6rc3/truss/validation.py
--rw-r--r--   0        0        0     7339 1970-01-01 00:00:00.000000 truss-0.4.6rc3/PKG-INFO
+-rw-r--r--   0        0        0     5483 2023-06-06 22:49:45.311210 truss-0.4.8rc4/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2576 2023-06-06 22:49:45.311210 truss-0.4.8rc4/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1064 2023-06-06 22:49:45.311210 truss-0.4.8rc4/LICENSE
+-rw-r--r--   0        0        0     5958 2023-06-06 22:49:45.311210 truss-0.4.8rc4/README.md
+-rw-r--r--   0        0        0     3077 2023-06-06 22:49:45.311210 truss-0.4.8rc4/ROADMAP.md
+-rw-r--r--   0        0        0      820 2023-06-06 22:49:45.311210 truss-0.4.8rc4/context_builder.Dockerfile
+-rw-r--r--   0        0        0     2319 2023-06-06 22:49:45.391211 truss-0.4.8rc4/pyproject.toml
+-rw-r--r--   0        0        0      330 2023-06-06 22:49:45.391211 truss-0.4.8rc4/truss/__init__.py
+-rw-r--r--   0        0        0      252 2023-06-06 22:49:45.391211 truss-0.4.8rc4/truss/blob/blob_backend.py
+-rw-r--r--   0        0        0      733 2023-06-06 22:49:45.391211 truss-0.4.8rc4/truss/blob/blob_backend_registry.py
+-rw-r--r--   0        0        0      648 2023-06-06 22:49:45.391211 truss-0.4.8rc4/truss/blob/http_public_blob_backend.py
+-rw-r--r--   0        0        0    13295 2023-06-06 22:49:45.391211 truss-0.4.8rc4/truss/build.py
+-rw-r--r--   0        0        0    10452 2023-06-06 22:49:45.391211 truss-0.4.8rc4/truss/cli.py
+-rw-r--r--   0        0        0     2813 2023-06-06 22:49:45.391211 truss-0.4.8rc4/truss/constants.py
+-rw-r--r--   0        0        0     1294 2023-06-06 22:49:45.391211 truss-0.4.8rc4/truss/contexts/image_builder/image_builder.py
+-rw-r--r--   0        0        0     5667 2023-06-06 22:49:45.391211 truss-0.4.8rc4/truss/contexts/image_builder/serving_image_builder.py
+-rw-r--r--   0        0        0     4684 2023-06-06 22:49:45.391211 truss-0.4.8rc4/truss/contexts/image_builder/training_image_builder.py
+-rw-r--r--   0        0        0     1896 2023-06-06 22:49:45.391211 truss-0.4.8rc4/truss/contexts/image_builder/util.py
+-rw-r--r--   0        0        0     2014 2023-06-06 22:49:45.391211 truss-0.4.8rc4/truss/contexts/local_loader/docker_build_emulator.py
+-rw-r--r--   0        0        0     1823 2023-06-06 22:49:45.391211 truss-0.4.8rc4/truss/contexts/local_loader/load_model_local.py
+-rw-r--r--   0        0        0     2239 2023-06-06 22:49:45.391211 truss-0.4.8rc4/truss/contexts/local_loader/train_local.py
+-rw-r--r--   0        0        0     5801 2023-06-06 22:49:45.391211 truss-0.4.8rc4/truss/contexts/local_loader/truss_module_loader.py
+-rw-r--r--   0        0        0      853 2023-06-06 22:49:45.391211 truss-0.4.8rc4/truss/contexts/local_loader/utils.py
+-rw-r--r--   0        0        0      436 2023-06-06 22:49:45.391211 truss-0.4.8rc4/truss/contexts/truss_context.py
+-rw-r--r--   0        0        0      394 2023-06-06 22:49:45.391211 truss-0.4.8rc4/truss/decorators.py
+-rw-r--r--   0        0        0     3641 2023-06-06 22:49:45.391211 truss-0.4.8rc4/truss/docker.py
+-rw-r--r--   0        0        0     3759 2023-06-06 22:49:45.391211 truss-0.4.8rc4/truss/environment_inference/requirements_inference.py
+-rw-r--r--   0        0        0      643 2023-06-06 22:49:45.391211 truss-0.4.8rc4/truss/errors.py
+-rw-r--r--   0        0        0      824 2023-06-06 22:49:45.391211 truss-0.4.8rc4/truss/local/local_config.py
+-rw-r--r--   0        0        0     3896 2023-06-06 22:49:45.391211 truss-0.4.8rc4/truss/local/local_config_handler.py
+-rw-r--r--   0        0        0     2713 2023-06-06 22:49:45.391211 truss-0.4.8rc4/truss/model_framework.py
+-rw-r--r--   0        0        0     1687 2023-06-06 22:49:45.391211 truss-0.4.8rc4/truss/model_frameworks/__init__.py
+-rw-r--r--   0        0        0     1895 2023-06-06 22:49:45.391211 truss-0.4.8rc4/truss/model_frameworks/huggingface_transformer.py
+-rw-r--r--   0        0        0      918 2023-06-06 22:49:45.391211 truss-0.4.8rc4/truss/model_frameworks/keras.py
+-rw-r--r--   0        0        0     1237 2023-06-06 22:49:45.391211 truss-0.4.8rc4/truss/model_frameworks/lightgbm.py
+-rw-r--r--   0        0        0     2410 2023-06-06 22:49:45.391211 truss-0.4.8rc4/truss/model_frameworks/mlflow.py
+-rw-r--r--   0        0        0     2441 2023-06-06 22:49:45.391211 truss-0.4.8rc4/truss/model_frameworks/pytorch.py
+-rw-r--r--   0        0        0     1232 2023-06-06 22:49:45.391211 truss-0.4.8rc4/truss/model_frameworks/sklearn.py
+-rw-r--r--   0        0        0     1027 2023-06-06 22:49:45.391211 truss-0.4.8rc4/truss/model_frameworks/xgboost.py
+-rw-r--r--   0        0        0     6521 2023-06-06 22:49:45.391211 truss-0.4.8rc4/truss/model_inference.py
+-rw-r--r--   0        0        0      510 2023-06-06 22:49:45.391211 truss-0.4.8rc4/truss/notebook.py
+-rw-r--r--   0        0        0    11065 2023-06-06 22:49:45.391211 truss-0.4.8rc4/truss/patch/calc_patch.py
+-rw-r--r--   0        0        0      774 2023-06-06 22:49:45.391211 truss-0.4.8rc4/truss/patch/dir_signature.py
+-rw-r--r--   0        0        0     2378 2023-06-06 22:49:45.391211 truss-0.4.8rc4/truss/patch/hash.py
+-rw-r--r--   0        0        0      468 2023-06-06 22:49:45.391211 truss-0.4.8rc4/truss/patch/signature.py
+-rw-r--r--   0        0        0      937 2023-06-06 22:49:45.391211 truss-0.4.8rc4/truss/patch/types.py
+-rw-r--r--   0        0        0      237 2023-06-06 22:49:45.391211 truss-0.4.8rc4/truss/pytest.ini
+-rw-r--r--   0        0        0      705 2023-06-06 22:49:45.391211 truss-0.4.8rc4/truss/readme_generator.py
+-rw-r--r--   0        0        0     2482 2023-06-06 22:49:45.391211 truss-0.4.8rc4/truss/templates/README.md.jinja
+-rw-r--r--   0        0        0        0 2023-06-06 22:49:45.391211 truss-0.4.8rc4/truss/templates/__init__.py
+-rw-r--r--   0        0        0     2310 2023-06-06 22:49:45.391211 truss-0.4.8rc4/truss/templates/base.Dockerfile.jinja
+-rw-r--r--   0        0        0     2190 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/control/control/application.py
+-rw-r--r--   0        0        0     4083 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/control/control/endpoints.py
+-rw-r--r--   0        0        0      413 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/control/control/helpers/context_managers.py
+-rw-r--r--   0        0        0      877 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/control/control/helpers/errors.py
+-rw-r--r--   0        0        0     5801 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/control/control/helpers/inference_server_controller.py
+-rw-r--r--   0        0        0     2596 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/control/control/helpers/inference_server_process_controller.py
+-rw-r--r--   0        0        0     2399 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/control/control/helpers/inference_server_starter.py
+-rw-r--r--   0        0        0     5389 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/control/control/helpers/patch_applier.py
+-rw-r--r--   0        0        0     3070 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/control/control/helpers/types.py
+-rw-r--r--   0        0        0     1843 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/control/control/server.py
+-rw-r--r--   0        0        0       86 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/control/requirements.txt
+-rw-r--r--   0        0        0       48 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/custom/examples.yaml
+-rw-r--r--   0        0        0        0 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/custom/model/__init__.py
+-rw-r--r--   0        0        0      534 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/custom/model/model.py
+-rw-r--r--   0        0        0      460 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/custom/train/train.py
+-rw-r--r--   0        0        0        0 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/huggingface_transformer/model/__init__.py
+-rw-r--r--   0        0        0     1827 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/huggingface_transformer/model/model.py
+-rw-r--r--   0        0        0       47 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/huggingface_transformer/requirements.txt
+-rw-r--r--   0        0        0        0 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/keras/model/__init__.py
+-rw-r--r--   0        0        0      728 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/keras/model/model.py
+-rw-r--r--   0        0        0        0 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/lightgbm/model/__init__.py
+-rw-r--r--   0        0        0     1251 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/lightgbm/model/model.py
+-rw-r--r--   0        0        0        0 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/mlflow/model/__init__.py
+-rw-r--r--   0        0        0      751 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/mlflow/model/model.py
+-rw-r--r--   0        0        0        0 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/pipeline/model/__init__.py
+-rw-r--r--   0        0        0      430 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/pipeline/model/model.py
+-rw-r--r--   0        0        0        0 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/pytorch/model/__init__.py
+-rw-r--r--   0        0        0     1263 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/pytorch/model/model.py
+-rw-r--r--   0        0        0        0 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/server/__init__.py
+-rw-r--r--   0        0        0       85 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/server/common/__init__.py
+-rw-r--r--   0        0        0     2433 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/server/common/errors.py
+-rw-r--r--   0        0        0     1892 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/server/common/external_data_resolver.py
+-rw-r--r--   0        0        0     1352 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/server/common/logging.py
+-rw-r--r--   0        0        0     2382 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/server/common/patches/whisper/patch.py
+-rw-r--r--   0        0        0     1450 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/server/common/patches.py
+-rw-r--r--   0        0        0      593 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/server/common/retry.py
+-rw-r--r--   0        0        0     3318 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/server/common/serialization.py
+-rw-r--r--   0        0        0     9426 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/server/common/truss_server.py
+-rw-r--r--   0        0        0     1445 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/server/common/util.py
+-rw-r--r--   0        0        0      727 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/server/inference_server.py
+-rw-r--r--   0        0        0     6339 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/server/model_wrapper.py
+-rw-r--r--   0        0        0      235 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/server/requirements.txt
+-rw-r--r--   0        0        0     2586 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/server.Dockerfile.jinja
+-rw-r--r--   0        0        0      138 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/shared/README.md
+-rw-r--r--   0        0        0        0 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/shared/__init__.py
+-rw-r--r--   0        0        0     1430 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/shared/secrets_resolver.py
+-rw-r--r--   0        0        0        0 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/sklearn/model/__init__.py
+-rw-r--r--   0        0        0     1221 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/sklearn/model/model.py
+-rw-r--r--   0        0        0     3400 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/training/job.py
+-rw-r--r--   0        0        0       12 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/training/requirements.txt
+-rw-r--r--   0        0        0      491 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/training.Dockerfile.jinja
+-rw-r--r--   0        0        0        0 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/xgboost/model/__init__.py
+-rw-r--r--   0        0        0     1453 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/templates/xgboost/model/model.py
+-rw-r--r--   0        0        0    30286 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/test_data/auto-mpg.data
+-rw-r--r--   0        0        0       93 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/test_data/context_builder_image_test/Dockerfile
+-rw-r--r--   0        0        0       72 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/test_data/context_builder_image_test/test.py
+-rw-r--r--   0        0        0     1394 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/test_data/happy.ipynb
+-rw-r--r--   0        0        0     1267 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/test_data/patch_ping_test_server/app.py
+-rw-r--r--   0        0        0    23279 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/test_data/pima-indians-diabetes.csv
+-rw-r--r--   0        0        0     1586 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/test_data/readme_int_example.md
+-rw-r--r--   0        0        0     1607 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/test_data/readme_no_example.md
+-rw-r--r--   0        0        0     1726 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/test_data/readme_str_example.md
+-rw-r--r--   0        0        0     2067 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/test_data/server.Dockerfile
+-rw-r--r--   0        0        0      669 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/test_data/server_conformance_test_truss/config.yaml
+-rw-r--r--   0        0        0        0 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/test_data/server_conformance_test_truss/model/__init__.py
+-rw-r--r--   0        0        0      597 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/test_data/server_conformance_test_truss/model/model.py
+-rw-r--r--   0        0        0      669 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/test_data/test_truss/config.yaml
+-rw-r--r--   0        0        0       48 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/test_data/test_truss/examples.yaml
+-rw-r--r--   0        0        0        0 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/test_data/test_truss/model/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/test_data/test_truss/model/dummy
+-rw-r--r--   0        0        0      534 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/test_data/test_truss/model/model.py
+-rw-r--r--   0        0        0        0 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/tests/__init__.py
+-rw-r--r--   0        0        0    20822 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/tests/conftest.py
+-rw-r--r--   0        0        0     1255 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/tests/contexts/image_builder/test_serving_image_builder.py
+-rw-r--r--   0        0        0      783 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/tests/contexts/local_loader/test_load_local.py
+-rw-r--r--   0        0        0     5337 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/tests/contexts/local_loader/test_truss_module_finder.py
+-rw-r--r--   0        0        0      968 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/tests/environments_inference/test_requirements_inference.py
+-rw-r--r--   0        0        0        0 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/tests/local/__init__.py
+-rw-r--r--   0        0        0     2245 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/tests/local/test_local_config_handler.py
+-rw-r--r--   0        0        0        0 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/tests/model_frameworks/__init__.py
+-rw-r--r--   0        0        0     3293 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/tests/model_frameworks/test_huggingface_transformer_framework.py
+-rw-r--r--   0        0        0     2789 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/tests/model_frameworks/test_keras_framework.py
+-rw-r--r--   0        0        0     2409 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/tests/model_frameworks/test_lightgbm_framework.py
+-rw-r--r--   0        0        0     1479 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/tests/model_frameworks/test_pytorch_framework.py
+-rw-r--r--   0        0        0     2427 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/tests/model_frameworks/test_sklearn_framework.py
+-rw-r--r--   0        0        0     2437 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/tests/model_frameworks/test_xgboost_framework.py
+-rw-r--r--   0        0        0    11109 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/tests/patch/test_calc_patch.py
+-rw-r--r--   0        0        0      487 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/tests/patch/test_dir_signature.py
+-rw-r--r--   0        0        0     5983 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/tests/patch/test_hash.py
+-rw-r--r--   0        0        0      394 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/tests/patch/test_signature.py
+-rw-r--r--   0        0        0      273 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/tests/patch/test_types.py
+-rw-r--r--   0        0        0    10415 2023-06-06 22:49:45.395211 truss-0.4.8rc4/truss/tests/samples.py
+-rw-r--r--   0        0        0      283 2023-06-06 22:49:45.399211 truss-0.4.8rc4/truss/tests/templates/control/control/helpers/test_context_managers.py
+-rw-r--r--   0        0        0     1976 2023-06-06 22:49:45.399211 truss-0.4.8rc4/truss/tests/templates/control/control/helpers/test_patch_applier.py
+-rw-r--r--   0        0        0     6931 2023-06-06 22:49:45.399211 truss-0.4.8rc4/truss/tests/templates/control/control/test_server.py
+-rw-r--r--   0        0        0      750 2023-06-06 22:49:45.399211 truss-0.4.8rc4/truss/tests/templates/core/server/common/test_util.py
+-rw-r--r--   0        0        0     1539 2023-06-06 22:49:45.399211 truss-0.4.8rc4/truss/tests/templates/core/server/test_secrets_resolver.py
+-rw-r--r--   0        0        0     2157 2023-06-06 22:49:45.399211 truss-0.4.8rc4/truss/tests/templates/server/common/test_external_resolver.py
+-rw-r--r--   0        0        0     2038 2023-06-06 22:49:45.399211 truss-0.4.8rc4/truss/tests/templates/server/common/test_retry.py
+-rw-r--r--   0        0        0     2252 2023-06-06 22:49:45.399211 truss-0.4.8rc4/truss/tests/templates/server/test_model_wrapper.py
+-rw-r--r--   0        0        0     1910 2023-06-06 22:49:45.399211 truss-0.4.8rc4/truss/tests/test_backward.py
+-rw-r--r--   0        0        0     8260 2023-06-06 22:49:45.399211 truss-0.4.8rc4/truss/tests/test_build.py
+-rw-r--r--   0        0        0     3181 2023-06-06 22:49:45.399211 truss-0.4.8rc4/truss/tests/test_config.py
+-rw-r--r--   0        0        0     1188 2023-06-06 22:49:45.399211 truss-0.4.8rc4/truss/tests/test_context_builder_image.py
+-rw-r--r--   0        0        0      517 2023-06-06 22:49:45.399211 truss-0.4.8rc4/truss/tests/test_docker.py
+-rw-r--r--   0        0        0     4905 2023-06-06 22:49:45.399211 truss-0.4.8rc4/truss/tests/test_model_inference.py
+-rw-r--r--   0        0        0      656 2023-06-06 22:49:45.399211 truss-0.4.8rc4/truss/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1483 2023-06-06 22:49:45.399211 truss-0.4.8rc4/truss/tests/test_testing_utilities_for_other_tests.py
+-rw-r--r--   0        0        0     1252 2023-06-06 22:49:45.399211 truss-0.4.8rc4/truss/tests/test_truss_gatherer.py
+-rw-r--r--   0        0        0    33899 2023-06-06 22:49:45.399211 truss-0.4.8rc4/truss/tests/test_truss_handle.py
+-rw-r--r--   0        0        0      434 2023-06-06 22:49:45.399211 truss-0.4.8rc4/truss/tests/test_truss_util.py
+-rw-r--r--   0        0        0     1865 2023-06-06 22:49:45.399211 truss-0.4.8rc4/truss/tests/test_validation.py
+-rw-r--r--   0        0        0    13143 2023-06-06 22:49:45.399211 truss-0.4.8rc4/truss/truss_config.py
+-rw-r--r--   0        0        0     2845 2023-06-06 22:49:45.399211 truss-0.4.8rc4/truss/truss_gatherer.py
+-rw-r--r--   0        0        0    40919 2023-06-06 22:49:45.399211 truss-0.4.8rc4/truss/truss_handle.py
+-rw-r--r--   0        0        0     5671 2023-06-06 22:49:45.399211 truss-0.4.8rc4/truss/truss_spec.py
+-rw-r--r--   0        0        0     2124 2023-06-06 22:49:45.399211 truss-0.4.8rc4/truss/types.py
+-rw-r--r--   0        0        0      227 2023-06-06 22:49:45.399211 truss-0.4.8rc4/truss/util/data_structures.py
+-rw-r--r--   0        0        0      553 2023-06-06 22:49:45.399211 truss-0.4.8rc4/truss/util/gpu.py
+-rw-r--r--   0        0        0      333 2023-06-06 22:49:45.399211 truss-0.4.8rc4/truss/util/jinja.py
+-rw-r--r--   0        0        0     2018 2023-06-06 22:49:45.399211 truss-0.4.8rc4/truss/util/path.py
+-rw-r--r--   0        0        0     2736 2023-06-06 22:49:45.399211 truss-0.4.8rc4/truss/validation.py
+-rw-r--r--   0        0        0     7595 1970-01-01 00:00:00.000000 truss-0.4.8rc4/PKG-INFO
```

### Comparing `truss-0.4.6rc3/CODE_OF_CONDUCT.md` & `truss-0.4.8rc4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/CONTRIBUTING.md` & `truss-0.4.8rc4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/LICENSE` & `truss-0.4.8rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/README.md` & `truss-0.4.8rc4/README.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/ROADMAP.md` & `truss-0.4.8rc4/ROADMAP.md`

 * *Files 8% similar despite different names*

```diff
@@ -47,18 +47,15 @@
 
 ## Performance
 
 ### Deployment backends
 
 Model deployments are a critical part of machine learning systems. We're working
 on a way to make it easier to deploy models on a variety of platforms. Each
-platform has its own set of performance tradeoffs. Today our model backend is a
-tornado server based heavily on kserve's implementation, and we're working on a
-way to make it easier to deploy models on other backends. This will allow truss
-users to exchange tornado for other API backends.
+platform has its own set of performance tradeoffs.
 
 ### GPU support
 
 Many models benefit from GPU training and inference. There are a few ways in
 which we can optimize support for GPUs at inference time:
 
 - Multi-GPU support
```

### Comparing `truss-0.4.6rc3/context_builder.Dockerfile` & `truss-0.4.8rc4/context_builder.Dockerfile`

 * *Files 20% similar despite different names*

```diff
@@ -11,8 +11,11 @@
     && rm -rf /var/lib/apt/lists/* /tmp/library-scripts/
 
 RUN curl -sSL https://install.python-poetry.org | python -
 
 ENV PATH="/root/.local/bin:${PATH}"
 COPY . .
 
-RUN poetry install --only builder
+# https://python-poetry.org/docs/configuration/#virtualenvsin-project
+# to write to project root .venv file to be used for context builder test
+RUN poetry config virtualenvs.in-project true \
+    && poetry install --only builder
```

### Comparing `truss-0.4.6rc3/pyproject.toml` & `truss-0.4.8rc4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "truss"
-version = "0.4.6rc3"
+version = "0.4.8rc4"
 description = "A seamless bridge from model development to model delivery"
 license = "MIT"
 readme = "README.md"
 authors = ["Pankaj Gupta <pankaj@baseten.co>", "Phil Howes <phil@baseten.co>"]
 include = ["*.txt", "*.Dockerfile", "*.md"]
 repository = "https://github.com/basetenlabs/truss"
 keywords = ["MLOps", "AI", "Model Serving", "Model Deployment", "Machine Learning"]
@@ -12,53 +12,59 @@
 [tool.poetry.urls]
 "Homepage" = "https://truss.baseten.co"
 "Bug Reports" = "https://github.com/basetenlabs/truss/issues"
 "Documentation" = "https://truss.baseten.co"
 "Baseten" = "https://baseten.co"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
+python = ">=3.8,<3.12"
 numpy = "1.23.5"
 msgpack = ">=1.0.2"
 msgpack-numpy = ">=0.4.7.1"
 packaging = "^20.9"
 python-json-logger = ">=2.0.2"
 PyYAML = "^6.0"
 Jinja2 = "^3.1.2"
 python-on-whales = "^0.46.0"
 tenacity = "^8.0.1"
 single-source = "^0.3.0"
 cloudpickle = "^2.2.0"
 blake3 = "^0.3.3"
+fastapi = "^0.95.0"
+uvicorn = "^0.21.1"
+psutil = "^5.9.4"
+joblib = "^1.2.0"
+dockerfile = "^3.2.0"
 
 [tool.poetry.group.builder.dependencies]
-python = ">=3.8,<3.11"
+python = ">=3.8,<3.12"
 packaging = "^20.9"
 python-json-logger = ">=2.0.2"
 PyYAML = "^6.0"
 Jinja2 = "^3.1.2"
 tenacity = "^8.0.1"
 cloudpickle = "^2.2.0"
 single-source = "^0.3.0"
 click = "^8.0.3"
 requests = "^2.28.1"
 blake3 = "^0.3.3"
+fastapi = "^0.95.0"
+uvicorn = "^0.21.1"
+psutil = "^5.9.4"
 
 [tool.poetry.dev-dependencies]
 torch = "^1.9.0"
 ipython = "^7.16"
 pytest = "7.2.0"
 tensorflow = { version = "^2.4.4", markers = "sys_platform == 'linux'" }
 tensorflow-macos = { version = "^2.4.4", markers = "sys_platform == 'darwin'" }
 pre-commit = "^2.18.1"
 scikit-learn = "1.0.2"
 pandas = "1.5.2"
 tensorflow-hub = "^0.12.0"
-# generally discouraged to use an RC version. Will fast follow with 0.10.0 version.
-kserve = "0.10.0rc1"
 isort = "^5.10.1"
 flake8 = "^4.0.1"
 ipdb = "^0.13.9"
 coverage = "^6.4.1"
 pytest-cov = "^3.0.0"
 xgboost = "^1.6.1"
 lightgbm = "^3.3.2"
@@ -71,14 +77,15 @@
 
 [tool.poetry.scripts]
 truss = 'truss.cli:cli_group'
 
 [tool.poetry.group.dev.dependencies]
 mlflow = "^1.29.0"
 mypy = "^1.0.0"
+pytest-split = "^0.8.1"
 
 [build-system]
 requires = ["poetry-core>=1.2.1"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
```

### Comparing `truss-0.4.6rc3/truss/blob/blob_backend_registry.py` & `truss-0.4.8rc4/truss/blob/blob_backend_registry.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/blob/http_public_blob_backend.py` & `truss-0.4.8rc4/truss/blob/http_public_blob_backend.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/build.py` & `truss-0.4.8rc4/truss/build.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/cli.py` & `truss-0.4.8rc4/truss/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,17 +163,17 @@
     type=click.Path(exists=True),
     required=False,
     help="Directory where context is built",
 )
 @click.option("--tag", help="Docker build image tag")
 @click.option("--port", type=int, default=8080, help="Local port used to run image")
 @click.option(
-    "--use-docker",
+    "--no-docker",
     is_flag=True,
-    default=True,
+    default=False,
     help="Flag to run prediction with a docker container",
 )
 @click.option(
     "--request-file",
     type=click.Path(exists=True),
     help="Path to json file containing the request",
 )
@@ -181,15 +181,15 @@
 @echo_output
 def predict(
     target_directory: str,
     request: Union[bytes, str],
     build_dir,
     tag,
     port,
-    use_docker,
+    no_docker,
     request_file,
 ):
     """
     Invokes the packaged model, either locally or in a Docker container.
 
     TARGET_DIRECTORY: A Truss directory. If none, use current directory.
 
@@ -197,33 +197,33 @@
 
     BUILD_DIR: Directory where context is built. If none, a temp directory is created.
 
     TAG: Docker build image tag
 
     PORT: Local port used to run image
 
-    USE_DOCKER: Flag to run prediction with a docker container
+    NO_DOCKER: Flag to run prediction without a docker container
 
     REQUEST_FILE: Path to json file containing the request
     """
     if request is not None:
         request_data = json.loads(request)
     elif request_file is not None:
         with open(request_file) as json_file:
             request_data = json.load(json_file)
     else:
         raise ValueError("At least one of request or request-file must be supplied.")
 
     tr = _get_truss_from_directory(target_directory=target_directory)
-    if use_docker:
+    if no_docker:
+        return tr.server_predict(request_data)
+    else:
         return tr.docker_predict(
             request_data, build_dir=build_dir, tag=tag, local_port=port, detach=True
         )
-    else:
-        return tr.server_predict(request_data)
 
 
 @cli_group.command()
 @click.option("--target_directory", required=False, help="Directory of truss")
 @click.option(
     "--build-dir",
     type=click.Path(exists=True),
```

### Comparing `truss-0.4.6rc3/truss/constants.py` & `truss-0.4.8rc4/truss/constants.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/contexts/image_builder/image_builder.py` & `truss-0.4.8rc4/truss/contexts/image_builder/image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/contexts/image_builder/serving_image_builder.py` & `truss-0.4.8rc4/truss/contexts/image_builder/serving_image_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,21 +111,20 @@
         data_dir = build_dir / config.data_dir
         bundled_packages_dir = build_dir / config.bundled_packages_dir
         dockerfile_template = read_template_from_fs(
             TEMPLATES_DIR, SERVER_DOCKERFILE_TEMPLATE_NAME
         )
         python_version = to_dotted_python_version(config.python_version)
         if config.base_image:
-            base_image_name_and_tag = config.base_image
+            base_image_name_and_tag = config.base_image.image
         else:
             base_image_name = truss_base_image_name(job_type="server")
             tag = truss_base_image_tag(
                 python_version=python_version,
                 use_gpu=config.resources.use_gpu,
-                live_reload=config.live_reload,
                 version_tag=TRUSS_BASE_IMAGE_VERSION_TAG,
             )
             base_image_name_and_tag = f"{base_image_name}:{tag}"
         should_install_system_requirements = file_is_not_empty(
             build_dir / SYSTEM_PACKAGES_TXT_FILENAME
         )
         should_install_python_requirements = file_is_not_empty(
```

### Comparing `truss-0.4.6rc3/truss/contexts/image_builder/training_image_builder.py` & `truss-0.4.8rc4/truss/contexts/image_builder/training_image_builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -97,29 +97,27 @@
         )
         should_install_requirements = file_is_not_empty(
             build_dir / REQUIREMENTS_TXT_FILENAME
         )
         config = self._spec.config
         python_version = to_dotted_python_version(config.python_version)
         if config.base_image:
-            base_image_name_and_tag = config.base_image
+            base_image_name_and_tag = config.base_image.image
         else:
             base_image_name = truss_base_image_name(job_type="training")
             tag = truss_base_image_tag(
                 python_version=python_version,
                 use_gpu=config.resources.use_gpu,
-                live_reload=config.live_reload,
                 version_tag=TRUSS_BASE_IMAGE_VERSION_TAG,
             )
             base_image_name_and_tag = f"{base_image_name}:{tag}"
         dockerfile_contents = dockerfile_template.render(
             base_image_name_and_tag=base_image_name_and_tag,
             config=self._spec.config,
             python_version=python_version,
-            live_reload=config.live_reload,
             bundled_packages_dir_exists=bundled_packages_dir_exists,
             should_install_system_requirements=should_install_system_requirements,
             should_install_requirements=should_install_requirements,
         )
         docker_file_path = build_dir / TRAINING_DOCKERFILE_NAME
         with docker_file_path.open("w") as docker_file:
             docker_file.write(dockerfile_contents)
```

### Comparing `truss-0.4.6rc3/truss/contexts/image_builder/util.py` & `truss-0.4.8rc4/truss/contexts/image_builder/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # manual nature is by design; at this point we want any new base image releases
 # to be reviewed via code change before landing. This value should be typically
 # set to the latest version of truss library.
 #
 # [IMPORTANT] Make sure all images for this version are published to dockerhub
 # before change to this value lands. This value is used to look for base images
 # when building docker image for a truss.
-TRUSS_BASE_IMAGE_VERSION_TAG = "v0.3.4"
+TRUSS_BASE_IMAGE_VERSION_TAG = "v0.4.8rc4"
 
 
 def file_is_empty(path: Path, ignore_hash_style_comments: bool = True) -> bool:
     if not path.exists():
         return True
 
     with path.open() as file:
@@ -39,25 +39,22 @@
 def truss_base_image_name(job_type: str) -> str:
     return f"baseten/truss-{job_type}-base"
 
 
 def truss_base_image_tag(
     python_version: str,
     use_gpu: bool,
-    live_reload: bool,
     version_tag: Optional[str] = None,
 ) -> str:
     if version_tag is None:
         version_tag = f"v{__version__}"
 
     base_tag = python_version
     if use_gpu:
         base_tag = f"{base_tag}-gpu"
-    if live_reload:
-        base_tag = f"{base_tag}-reload"
     return f"{base_tag}-{version_tag}"
 
 
 def to_dotted_python_version(truss_python_version: str) -> str:
     """Converts python version string using in truss config to the conventional dotted form.
 
     e.g. py39 to 3.9
```

### Comparing `truss-0.4.6rc3/truss/contexts/local_loader/load_model_local.py` & `truss-0.4.8rc4/truss/contexts/local_loader/load_model_local.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from truss.contexts.local_loader.truss_module_loader import truss_module_loaded
 from truss.contexts.local_loader.utils import (
     prepare_secrets,
     signature_accepts_keyword_arg,
 )
 from truss.contexts.truss_context import TrussContext
+from truss.templates.server.common.patches import apply_patches
 from truss.truss_spec import TrussSpec
 
 
 class LoadModelLocal(TrussContext):
     """Loads a Truss model locally.
 
     The loaded model can be used to make predictions for quick testing.
@@ -32,11 +33,12 @@
             model_init_params = {}
             if signature_accepts_keyword_arg(model_class_signature, "config"):
                 model_init_params["config"] = spec.config.to_dict()
             if signature_accepts_keyword_arg(model_class_signature, "data_dir"):
                 model_init_params["data_dir"] = truss_dir / "data"
             if signature_accepts_keyword_arg(model_class_signature, "secrets"):
                 model_init_params["secrets"] = prepare_secrets(spec)
+            apply_patches(spec.apply_library_patches, spec.requirements)
             model = model_class(**model_init_params)
             if hasattr(model, "load"):
                 model.load()
             return model
```

### Comparing `truss-0.4.6rc3/truss/contexts/local_loader/train_local.py` & `truss-0.4.8rc4/truss/contexts/local_loader/train_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/contexts/local_loader/truss_module_loader.py` & `truss-0.4.8rc4/truss/contexts/local_loader/truss_module_loader.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/contexts/local_loader/utils.py` & `truss-0.4.8rc4/truss/contexts/local_loader/utils.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/docker.py` & `truss-0.4.8rc4/truss/docker.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/environment_inference/requirements_inference.py` & `truss-0.4.8rc4/truss/environment_inference/requirements_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/errors.py` & `truss-0.4.8rc4/truss/errors.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/local/local_config.py` & `truss-0.4.8rc4/truss/local/local_config.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/local/local_config_handler.py` & `truss-0.4.8rc4/truss/local/local_config_handler.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/model_framework.py` & `truss-0.4.8rc4/truss/model_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/model_frameworks/__init__.py` & `truss-0.4.8rc4/truss/model_frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/model_frameworks/huggingface_transformer.py` & `truss-0.4.8rc4/truss/model_frameworks/huggingface_transformer.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/model_frameworks/keras.py` & `truss-0.4.8rc4/truss/model_frameworks/keras.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/model_frameworks/lightgbm.py` & `truss-0.4.8rc4/truss/model_frameworks/lightgbm.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/model_frameworks/mlflow.py` & `truss-0.4.8rc4/truss/model_frameworks/mlflow.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/model_frameworks/pytorch.py` & `truss-0.4.8rc4/truss/model_frameworks/pytorch.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/model_frameworks/sklearn.py` & `truss-0.4.8rc4/truss/model_frameworks/sklearn.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/model_frameworks/xgboost.py` & `truss-0.4.8rc4/truss/model_frameworks/xgboost.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/model_inference.py` & `truss-0.4.8rc4/truss/model_inference.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 from truss.errors import FrameworkNotSupportedError
 
 # lists of versions supported by the truss+base_images
 PYTHON_VERSIONS = {
     "py37",
     "py38",
     "py39",
+    "py310",
+    "py311",
 }
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 def _infer_model_framework(model_class: Any):
     model_framework, _, _ = model_class.__module__.partition(".")
@@ -84,28 +86,27 @@
     """
     python_major_version = int(python_version[2:3])
     python_minor_version = int(python_version[3:])
 
     if python_major_version > 3:
         raise NotImplementedError("Only python version 3 is supported")
 
-    # TODO(pankaj) Add full support for 3.10 and 3.11, this is stop-gap.
-    if python_minor_version > 9:
+    if python_minor_version > 11:
         logger.info(
             f"Mapping python version {python_major_version}.{python_minor_version}"
-            " to 3.9, the highest version that Truss currently supports."
+            " to 3.11, the highest version that Truss currently supports."
         )
-        return "py39"
+        return "py311"
 
-    if python_minor_version < 7:
+    if python_minor_version < 8:
         logger.info(
             f"Mapping python version {python_major_version}.{python_minor_version}"
-            " to 3.7, the lowest version that Truss currently supports."
+            " to 3.8, the lowest version that Truss currently supports."
         )
-        return "py37"
+        return "py38"
 
     return python_version
 
 
 def infer_model_information(model: Any) -> ModelBuildStageOne:
     model_class = _model_class(model)
     model_framework = _infer_model_framework(model_class)
```

### Comparing `truss-0.4.6rc3/truss/patch/calc_patch.py` & `truss-0.4.8rc4/truss/patch/calc_patch.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/patch/dir_signature.py` & `truss-0.4.8rc4/truss/patch/dir_signature.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/patch/hash.py` & `truss-0.4.8rc4/truss/patch/hash.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/patch/types.py` & `truss-0.4.8rc4/truss/patch/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/readme_generator.py` & `truss-0.4.8rc4/truss/readme_generator.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/templates/README.md.jinja` & `truss-0.4.8rc4/truss/templates/README.md.jinja`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/templates/base.Dockerfile.jinja` & `truss-0.4.8rc4/truss/templates/base.Dockerfile.jinja`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 ARG PYVERSION={{config.python_version}}
 FROM {{base_image_name_and_tag}}
 
+ENV PYTHON_EXECUTABLE {{ config.base_image.python_executable_path or 'python3' }}
+
 {% block fail_fast %}
 RUN grep -w 'ID=debian\|ID_LIKE=debian' /etc/os-release || { echo "ERROR: Supplied base image is not a debian image"; exit 1; }
-RUN pythonVersion=$(echo $(command -v python >/dev/null 2>&1 && python --version || python3 --version) | cut -d" " -f2 | cut -d"." -f1,2) \
-    && echo $pythonVersion | grep -E '3\.[0-9]|10\.[0-9][0-9]' \
+RUN pythonVersion=$(echo $($PYTHON_EXECUTABLE --version) | cut -d" " -f2 | cut -d"." -f1,2) \
+    && $PYTHON_EXECUTABLE -c "import sys; sys.exit(0) if sys.version_info.major == 3 and sys.version_info.minor >=8 and sys.version_info.minor <=11 else sys.exit(1)" \
     && apt-get update && ( apt-get install -y --no-install-recommends python$pythonVersion-venv || apt-get install -y --no-install-recommends python3-venv )  \
     && apt-get autoremove -y \
     && apt-get clean -y \
     && rm -rf /var/lib/apt/lists/* \
-    || { echo "ERROR: Supplied base image does not have 3.8 <= python <= 3.10"; exit 1; }
+    || { echo "ERROR: Supplied base image does not have 3.8 <= python <= 3.11"; exit 1; }
 {% endblock %}
 
 RUN pip install --upgrade pip --no-cache-dir \
     && rm -rf /root/.cache/pip
 
 {% block base_image_patch %}
 {% endblock %}
```

### Comparing `truss-0.4.6rc3/truss/templates/control/control/application.py` & `truss-0.4.8rc4/truss/templates/control/control/application.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/templates/control/control/endpoints.py` & `truss-0.4.8rc4/truss/templates/control/control/endpoints.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/templates/control/control/helpers/errors.py` & `truss-0.4.8rc4/truss/templates/control/control/helpers/errors.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/templates/control/control/helpers/inference_server_controller.py` & `truss-0.4.8rc4/truss/templates/control/control/helpers/inference_server_controller.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/templates/control/control/helpers/inference_server_process_controller.py` & `truss-0.4.8rc4/truss/templates/control/control/helpers/inference_server_process_controller.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/templates/control/control/helpers/inference_server_starter.py` & `truss-0.4.8rc4/truss/templates/control/control/helpers/inference_server_starter.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/templates/control/control/helpers/patch_applier.py` & `truss-0.4.8rc4/truss/templates/control/control/helpers/patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/templates/control/control/helpers/types.py` & `truss-0.4.8rc4/truss/templates/control/control/helpers/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/templates/control/control/server.py` & `truss-0.4.8rc4/truss/templates/control/control/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     application = create_app(
         {
             "inference_server_home": inf_serv_home,
             "inference_server_process_args": [
                 python_executable_path,
                 f"{inf_serv_home}/inference_server.py",
             ],
-            "control_server_host": "0.0.0.0",
+            "control_server_host": "*",
             "control_server_port": CONTROL_SERVER_PORT,
             "inference_server_port": INFERENCE_SERVER_PORT,
         }
     )
 
     # Perform inference server startup flow in background
     Thread(target=inference_server_startup_flow, args=(application,)).start()
```

### Comparing `truss-0.4.6rc3/truss/templates/custom/model/model.py` & `truss-0.4.8rc4/truss/templates/custom/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/templates/huggingface_transformer/model/model.py` & `truss-0.4.8rc4/truss/templates/huggingface_transformer/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/templates/keras/model/model.py` & `truss-0.4.8rc4/truss/templates/keras/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/templates/lightgbm/model/model.py` & `truss-0.4.8rc4/truss/templates/lightgbm/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/templates/mlflow/model/model.py` & `truss-0.4.8rc4/truss/templates/mlflow/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/templates/pytorch/model/model.py` & `truss-0.4.8rc4/truss/templates/pytorch/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/templates/server/common/external_data_resolver.py` & `truss-0.4.8rc4/truss/templates/server/common/external_data_resolver.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/templates/server/common/logging.py` & `truss-0.4.8rc4/truss/templates/server/common/logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import sys
 
 from pythonjsonlogger import jsonlogger
 
 LEVEL: int = logging.INFO
 
-JSON_LOG_HANDLER = logging.StreamHandler(stream=sys.stderr)
+JSON_LOG_HANDLER = logging.StreamHandler(stream=sys.stdout)
 JSON_LOG_HANDLER.set_name("json_logger_handler")
 JSON_LOG_HANDLER.setLevel(LEVEL)
 JSON_LOG_HANDLER.setFormatter(
     jsonlogger.JsonFormatter("%(asctime)s %(levelname)s %(message)s")
 )
```

### Comparing `truss-0.4.6rc3/truss/templates/server/common/retry.py` & `truss-0.4.8rc4/truss/templates/server/common/retry.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/templates/server/common/serialization.py` & `truss-0.4.8rc4/truss/templates/server/common/serialization.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/templates/server/inference_server.py` & `truss-0.4.8rc4/truss/templates/server/inference_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,13 +17,13 @@
     def __init__(self, config_path: str, port: int):
         self._port = port
         with open(config_path, encoding="utf-8") as config_file:
             self._config = yaml.safe_load(config_file)
 
     def start(self):
         server = TrussServer(http_port=self._port, config=self._config)
-        server.start_model()
+        server.start()
 
 
 if __name__ == "__main__":
     env_port = int(os.environ.get("INFERENCE_SERVER_PORT", "8080"))
     ConfiguredTrussServer(CONFIG_FILE, env_port).start()
```

### Comparing `truss-0.4.6rc3/truss/templates/server/model_wrapper.py` & `truss-0.4.8rc4/truss/templates/server/model_wrapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,72 +4,66 @@
 import os
 import sys
 import time
 import traceback
 from enum import Enum
 from pathlib import Path
 from threading import Lock, Thread
-from typing import Dict, Optional, Union
+from typing import Any, Dict, Optional
 
-import kserve
-from cloudevents.http import CloudEvent
-from common.external_data_resolver import download_external_data  # noqa: E402
+from common.external_data_resolver import download_external_data
+from common.patches import apply_patches
 from common.retry import retry
-from kserve.grpc.grpc_predict_v2_pb2 import ModelInferRequest, ModelInferResponse
 from shared.secrets_resolver import SecretsResolver
 
 MODEL_BASENAME = "model"
 
 NUM_LOAD_RETRIES = int(os.environ.get("NUM_LOAD_RETRIES_TRUSS", "3"))
 
 
-class ModelWrapper(kserve.Model):
+class ModelWrapper:
     class Status(Enum):
         NOT_READY = 0
         LOADING = 1
         READY = 2
         FAILED = 3
 
-    _config: Dict
-    _model: object
-    _load_lock: Lock = Lock()
-    _predict_lock: Lock = Lock()
-    _status: Status = Status.NOT_READY
-    _logger: logging.Logger
-    ready: bool
-
     def __init__(self, config: Dict):
-        super().__init__(MODEL_BASENAME)
         self._config = config
-        self.logger = logging.getLogger(__name__)
+        self._logger = logging.getLogger()
+        self.name = MODEL_BASENAME
+        self.ready = False
+        self._load_lock = Lock()
+        self._predict_lock = Lock()
+        self._status = ModelWrapper.Status.NOT_READY
 
     def load(self) -> bool:
         if self.ready:
             return self.ready
 
         # if we are already loading, just pass; our container will return 503 while we're loading
         if not self._load_lock.acquire(blocking=False):
             return False
 
         self._status = ModelWrapper.Status.LOADING
 
-        self.logger.info("Executing model.load()...")
+        self._logger.info("Executing model.load()...")
 
         try:
             start_time = time.perf_counter()
             self.try_load()
             self.ready = True
             self._status = ModelWrapper.Status.READY
-            self.logger.info(
+            self._logger.info(
                 f"Completed model.load() execution in {_elapsed_ms(start_time)} ms"
             )
 
             return self.ready
         except Exception:
-            self.logger.exception("Exception while loading model")
+            self._logger.exception("Exception while loading model")
             self._status = ModelWrapper.Status.FAILED
         finally:
             self._load_lock.release()
 
         return self.ready
 
     def start_load(self):
@@ -108,59 +102,92 @@
         model_init_params = {}
         if _signature_accepts_keyword_arg(model_class_signature, "config"):
             model_init_params["config"] = self._config
         if _signature_accepts_keyword_arg(model_class_signature, "data_dir"):
             model_init_params["data_dir"] = data_dir
         if _signature_accepts_keyword_arg(model_class_signature, "secrets"):
             model_init_params["secrets"] = SecretsResolver.get_secrets(self._config)
+        apply_patches(
+            self._config.get("apply_library_patches", True),
+            self._config["requirements"],
+        )
         self._model = model_class(**model_init_params)
 
         if hasattr(self._model, "load"):
             retry(
                 self._model.load,
                 NUM_LOAD_RETRIES,
-                self.logger.warn,
+                self._logger.warn,
                 "Failed to load model.",
                 gap_seconds=1.0,
             )
 
     def preprocess(
         self,
-        payload: Union[Dict, CloudEvent, ModelInferRequest],
+        payload: Any,
         headers: Optional[Dict[str, str]] = None,
-    ) -> Union[Dict, ModelInferRequest]:
+    ) -> Any:
         if not hasattr(self._model, "preprocess"):
             return payload
         return self._model.preprocess(payload)  # type: ignore
 
     def postprocess(
         self,
-        response: Union[Dict, ModelInferResponse],
+        response: Any,
         headers: Optional[Dict[str, str]] = None,
-    ) -> Dict:
+    ) -> Any:
         if not hasattr(self._model, "postprocess"):
             return response
         return self._model.postprocess(response)  # type: ignore
 
     def predict(
         self,
-        payload: Union[Dict, ModelInferRequest],
+        payload: Any,
         headers: Optional[Dict[str, str]] = None,
-    ) -> Union[Dict, ModelInferResponse]:
+    ) -> Any:
         try:
             self._predict_lock.acquire()
             return self._model.predict(payload)  # type: ignore
         except Exception:
             response = {}
             logging.exception("Exception while running predict")
             response["error"] = {"traceback": traceback.format_exc()}
             return response
         finally:
             self._predict_lock.release()
 
+    async def __call__(
+        self, body: Any, headers: Optional[Dict[str, str]] = None
+    ) -> Dict:
+        """Method to call predictor or explainer with the given input.
+
+        Args:
+            body (Any): Request payload body.
+            headers (Dict): Request headers.
+
+        Returns:
+            Dict: Response output from preprocess -> predictor -> postprocess
+        """
+
+        payload = (
+            await self.preprocess(body, headers)
+            if inspect.iscoroutinefunction(self.preprocess)
+            else self.preprocess(body, headers)
+        )
+
+        response = (
+            (await self.predict(payload, headers))
+            if inspect.iscoroutinefunction(self.predict)
+            else self.predict(payload, headers)
+        )
+
+        response = self.postprocess(response, headers)
+
+        return response
+
 
 def _signature_accepts_keyword_arg(signature: inspect.Signature, kwarg: str) -> bool:
     return kwarg in signature.parameters or _signature_accepts_kwargs(signature)
 
 
 def _signature_accepts_kwargs(signature: inspect.Signature) -> bool:
     for param in signature.parameters.values():
```

### Comparing `truss-0.4.6rc3/truss/templates/server.Dockerfile.jinja` & `truss-0.4.8rc4/truss/templates/server.Dockerfile.jinja`

 * *Files 20% similar despite different names*

```diff
@@ -16,26 +16,20 @@
     && apt-get autoremove -y \
     && apt-get clean -y \
     && rm -rf /var/lib/apt/lists/*
 
 COPY ./base_server_requirements.txt base_server_requirements.txt
 RUN pip install -r base_server_requirements.txt --no-cache-dir && rm -rf /root/.cache/pip
 
-# This is a hack, kfserving uses table_logger, which doesn't work well with
-# numpy 1.24 onwards, where np.float and np.int have been remove.
-# https://github.com/AleksTk/table-logger/blob/v0.3.6/table_logger/table_logger.py#L80
-# Monkey patch table_logger here. Ultimately we should move away from kfserving,
-# perhaps to kserve.
-RUN find /usr/local/lib/ -name table_logger.py -exec sed -i '/np\.int:/d;/np\.float:/d' {} \;
-
-{% if live_reload %}
-COPY ./control /control
-RUN python3 -m venv /control/.env \
-    && /control/.env/bin/pip3 install -r /control/requirements.txt
-{% endif %}
+    {%- if config.live_reload %}
+# Create symlink for control server to start inference server process with correct python executable
+RUN readlink {{config.base_image.python_executable_path}} &>/dev/null \
+    && echo "WARNING: Overwriting existing link at /usr/local/bin/python"
+RUN ln -sf {{config.base_image.python_executable_path}} /usr/local/bin/python
+    {%- endif %}
 {% endif %}
 
 {% endblock %}
 
 {% block install_requirements %}
     {%- if should_install_server_requirements %}
 COPY ./server_requirements.txt server_requirements.txt
@@ -47,27 +41,36 @@
 {% block b10cp %}
 RUN mkdir -p /app/bin \
     && curl https://baseten-public.s3.us-west-2.amazonaws.com/bin/b10cp-0.0.2-linux-amd64 -o /app/bin/b10cp \
     && chmod +x /app/bin/b10cp
 {% endblock %}
 
 {% block app_copy %}
+# Copy data before code for better caching
+{%- if data_dir_exists %}
+COPY ./{{config.data_dir}} /app/data
+{%- endif %}
+
 COPY ./server /app
 COPY ./{{ config.model_module_dir }} /app/model
 COPY ./config.yaml /app/config.yaml
-    {%- if data_dir_exists %}
-COPY ./{{config.data_dir}} /app/data
+    {%- if config.live_reload %}
+COPY ./control /control
+RUN python3 -m venv /control/.env \
+    && /control/.env/bin/pip3 install -r /control/requirements.txt
     {%- endif %}
 {% endblock %}
 
 
 {% block run %}
     {%- if config.live_reload %}
 ENV HASH_TRUSS {{truss_hash}}
 ENV CONTROL_SERVER_PORT 8080
 ENV INFERENCE_SERVER_PORT 8090
-CMD exec /control/.env/bin/python3 /control/control/server.py
+ENV SERVER_START_CMD="/control/.env/bin/python3 /control/control/server.py"
+ENTRYPOINT ["/control/.env/bin/python3", "/control/control/server.py"]
     {%- else %}
 ENV INFERENCE_SERVER_PORT 8080
-CMD exec python3 /app/inference_server.py
+ENV SERVER_START_CMD="{{(config.base_image.python_executable_path or "python3") ~ " /app/inference_server.py"}}"
+ENTRYPOINT ["{{config.base_image.python_executable_path or "python3"}}", "/app/inference_server.py"]
     {%- endif %}
 {% endblock %}
```

### Comparing `truss-0.4.6rc3/truss/templates/shared/secrets_resolver.py` & `truss-0.4.8rc4/truss/templates/shared/secrets_resolver.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/templates/sklearn/model/model.py` & `truss-0.4.8rc4/truss/templates/sklearn/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/templates/training/job.py` & `truss-0.4.8rc4/truss/templates/training/job.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/templates/xgboost/model/model.py` & `truss-0.4.8rc4/truss/templates/xgboost/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/test_data/auto-mpg.data` & `truss-0.4.8rc4/truss/test_data/auto-mpg.data`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/test_data/context_builder_image_test/server.Dockerfile` & `truss-0.4.8rc4/truss/test_data/server.Dockerfile`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 ARG PYVERSION=py39
 FROM baseten/truss-server-base:3.9-v0.4.3
 
+ENV PYTHON_EXECUTABLE /usr/local/bin/python3
+
 RUN grep -w 'ID=debian\|ID_LIKE=debian' /etc/os-release || { echo "ERROR: Supplied base image is not a debian image"; exit 1; }
-RUN pythonVersion=$(echo $(command -v python >/dev/null 2>&1 && python --version || python3 --version) | cut -d" " -f2 | cut -d"." -f1,2) \
-    && echo $pythonVersion | grep -E '3\.[0-9]|10\.[0-9][0-9]' \
+RUN pythonVersion=$(echo $($PYTHON_EXECUTABLE --version) | cut -d" " -f2 | cut -d"." -f1,2) \
+    && $PYTHON_EXECUTABLE -c "import sys; sys.exit(0) if sys.version_info.major == 3 and sys.version_info.minor >=8 and sys.version_info.minor <=11 else sys.exit(1)" \
     && apt-get update && ( apt-get install -y --no-install-recommends python$pythonVersion-venv || apt-get install -y --no-install-recommends python3-venv )  \
     && apt-get autoremove -y \
     && apt-get clean -y \
     && rm -rf /var/lib/apt/lists/* \
-    || { echo "ERROR: Supplied base image does not have 3.8 <= python <= 3.10"; exit 1; }
-
+    || { echo "ERROR: Supplied base image does not have 3.8 <= python <= 3.11"; exit 1; }
 
 RUN pip install --upgrade pip --no-cache-dir \
     && rm -rf /root/.cache/pip
 
 # If user base image is supplied in config, apply build commands from truss base image
 ENV PYTHONUNBUFFERED True
 ENV DEBIAN_FRONTEND=noninteractive
@@ -28,30 +29,25 @@
     && apt-get autoremove -y \
     && apt-get clean -y \
     && rm -rf /var/lib/apt/lists/*
 
 COPY ./base_server_requirements.txt base_server_requirements.txt
 RUN pip install -r base_server_requirements.txt --no-cache-dir && rm -rf /root/.cache/pip
 
-# This is a hack, kfserving uses table_logger, which doesn't work well with
-# numpy 1.24 onwards, where np.float and np.int have been remove.
-# https://github.com/AleksTk/table-logger/blob/v0.3.6/table_logger/table_logger.py#L80
-# Monkey patch table_logger here. Ultimately we should move away from kfserving,
-# perhaps to kserve.
-RUN find /usr/local/lib/ -name table_logger.py -exec sed -i '/np\.int:/d;/np\.float:/d' {} \;
-
 RUN mkdir -p /app/bin \
     && curl https://baseten-public.s3.us-west-2.amazonaws.com/bin/b10cp-0.0.2-linux-amd64 -o /app/bin/b10cp \
     && chmod +x /app/bin/b10cp
 
 ENV APP_HOME /app
 WORKDIR $APP_HOME
 
+# Copy data before code for better caching
+COPY ./data /app/data
 COPY ./server /app
 COPY ./model /app/model
 COPY ./config.yaml /app/config.yaml
-COPY ./data /app/data
 
 COPY ./packages /packages
 
 ENV INFERENCE_SERVER_PORT 8080
-CMD exec python3 /app/inference_server.py
+ENV SERVER_START_CMD="/usr/local/bin/python3 /app/inference_server.py"
+ENTRYPOINT ["/usr/local/bin/python3", "/app/inference_server.py"]
```

### Comparing `truss-0.4.6rc3/truss/test_data/happy.ipynb` & `truss-0.4.8rc4/truss/test_data/happy.ipynb`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/test_data/patch_ping_test_server/app.py` & `truss-0.4.8rc4/truss/test_data/patch_ping_test_server/app.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/test_data/pima-indians-diabetes.csv` & `truss-0.4.8rc4/truss/test_data/pima-indians-diabetes.csv`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/test_data/readme_int_example.md` & `truss-0.4.8rc4/truss/test_data/readme_int_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/test_data/readme_no_example.md` & `truss-0.4.8rc4/truss/test_data/readme_no_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/test_data/readme_str_example.md` & `truss-0.4.8rc4/truss/test_data/readme_str_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/test_data/test_truss/config.yaml` & `truss-0.4.8rc4/truss/test_data/server_conformance_test_truss/config.yaml`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/test_data/test_truss/model/model.py` & `truss-0.4.8rc4/truss/test_data/test_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/tests/conftest.py` & `truss-0.4.8rc4/truss/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 import tensorflow as tf
 from sklearn.datasets import load_iris
 from sklearn.ensemble import RandomForestClassifier
 from tensorflow.keras import layers
 from tensorflow.keras.layers.experimental import preprocessing
 from transformers import AutoModelWithLMHead, AutoTokenizer, pipeline
 from truss.build import create, init
+from truss.contexts.image_builder.serving_image_builder import (
+    ServingImageBuilderContext,
+)
+from truss.contexts.local_loader.docker_build_emulator import DockerBuildEmulator
 from truss.truss_config import DEFAULT_BUNDLED_PACKAGES_DIR
 from truss.types import Example
 from xgboost import XGBClassifier
 
 PYTORCH_MODEL_FILE_CONTENTS = """
 import torch
 import torch.nn as nn
@@ -351,15 +355,15 @@
 @pytest.fixture
 def custom_model_external_data_access_tuple_fixture(tmp_path: Path):
     content = "test"
     filename = "test.txt"
     (tmp_path / filename).write_text(content)
     port = 9089
     proc = subprocess.Popen(
-        ["python", "-m", "http.server", str(port), "--bind", "0.0.0.0"],
+        ["python", "-m", "http.server", str(port), "--bind", "*"],
         cwd=tmp_path,
     )
     try:
         url = f"http://host.docker.internal:{port}/{filename}"
         # Add arbitrary get params to get that they don't cause issues, the
         # server above ignores them.
         # url_with_get_params = f"{url}?foo=bar&baz=bla"
@@ -688,33 +692,27 @@
     handle.add_secret("secret_name", "default_secret_value")
     handle.spec.model_class_filepath.write_text(CUSTOM_MODEL_CODE_FOR_SECRETS_TESTING)
     yield dir_path
 
 
 @pytest.fixture
 def truss_container_fs(tmp_path):
-    ROOT = str(Path(__file__).parent.parent.parent.resolve())
-    subprocess.run(["truss", "run-image", "truss/test_data/test_truss"], cwd=ROOT)
+    ROOT = Path(__file__).parent.parent.parent.resolve()
     truss_fs = tmp_path / "truss_fs"
     truss_fs.mkdir()
-
-    ps_output = subprocess.check_output(
-        [
-            "docker",
-            "ps",
-            "--filter",
-            "label=truss_dir=truss/test_data/test_truss",
-            "--format",
-            "'{{.Names}},{{.Image}}'",
-        ]
+    truss_build_dir = tmp_path / "truss_fs_build"
+    truss_build_dir.mkdir()
+    image_builder = ServingImageBuilderContext.run(
+        ROOT / "truss" / "test_data" / "test_truss",
     )
-    container_name, image = ps_output.decode("utf-8").strip()[1:-1].split(",")
-    subprocess.run(["docker", "cp", f"{container_name}:/app", str(truss_fs / "app")])
-    subprocess.run(["docker", "kill", container_name])
-    subprocess.run(["docker", "rmi", image, "-f"])
+    image_builder.prepare_image_build_dir(truss_build_dir)
+    dockerfile_path = truss_build_dir / "Dockerfile"
+
+    docker_build_emulator = DockerBuildEmulator(dockerfile_path, truss_build_dir)
+    docker_build_emulator.run(truss_fs)
     return truss_fs
 
 
 @pytest.fixture
 def patch_ping_test_server():
     port = "5001"
     proc = subprocess.Popen(
```

### Comparing `truss-0.4.6rc3/truss/tests/contexts/image_builder/test_serving_image_builder.py` & `truss-0.4.8rc4/truss/tests/contexts/image_builder/test_serving_image_builder.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 from truss.truss_handle import TrussHandle
 
 BASE_DIR = Path(__file__).parent
 
 
 def test_serving_image_dockerfile_from_user_base_image(custom_model_truss_dir):
     th = TrussHandle(custom_model_truss_dir)
-    th.set_base_image("baseten/truss-server-base:3.9-v0.4.3")
+    th.set_base_image("baseten/truss-server-base:3.9-v0.4.3", "/usr/local/bin/python3")
     builder_context = ServingImageBuilderContext
     image_builder = builder_context.run(th.spec.truss_dir)
     with TemporaryDirectory() as tmp_dir:
         tmp_path = Path(tmp_dir)
         image_builder.prepare_image_build_dir(tmp_path)
         with open(tmp_path / "Dockerfile", "r") as f:
             gen_docker_lines = f.readlines()
         with open(
-            f"{BASE_DIR}/../../../test_data/context_builder_image_test/server.Dockerfile",
+            f"{BASE_DIR}/../../../test_data/server.Dockerfile",
             "r",
         ) as f:
             server_docker_lines = f.readlines()
 
         def filter_empty_lines(lines):
             return list(filter(lambda x: x and x != "\n", lines))
```

### Comparing `truss-0.4.6rc3/truss/tests/contexts/local_loader/test_load_local.py` & `truss-0.4.8rc4/truss/tests/contexts/local_loader/test_load_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/tests/contexts/local_loader/test_truss_module_finder.py` & `truss-0.4.8rc4/truss/tests/contexts/local_loader/test_truss_module_finder.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/tests/environments_inference/test_requirements_inference.py` & `truss-0.4.8rc4/truss/tests/environments_inference/test_requirements_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/tests/local/test_local_config_handler.py` & `truss-0.4.8rc4/truss/tests/local/test_local_config_handler.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/tests/model_frameworks/test_huggingface_transformer_framework.py` & `truss-0.4.8rc4/truss/tests/model_frameworks/test_huggingface_transformer_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/tests/model_frameworks/test_keras_framework.py` & `truss-0.4.8rc4/truss/tests/model_frameworks/test_keras_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/tests/model_frameworks/test_lightgbm_framework.py` & `truss-0.4.8rc4/truss/tests/model_frameworks/test_lightgbm_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/tests/model_frameworks/test_pytorch_framework.py` & `truss-0.4.8rc4/truss/tests/model_frameworks/test_pytorch_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/tests/model_frameworks/test_sklearn_framework.py` & `truss-0.4.8rc4/truss/tests/model_frameworks/test_sklearn_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/tests/model_frameworks/test_xgboost_framework.py` & `truss-0.4.8rc4/truss/tests/model_frameworks/test_xgboost_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/tests/patch/test_calc_patch.py` & `truss-0.4.8rc4/truss/tests/patch/test_calc_patch.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/tests/patch/test_hash.py` & `truss-0.4.8rc4/truss/tests/patch/test_hash.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/tests/samples.py` & `truss-0.4.8rc4/truss/tests/samples.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/tests/templates/control/control/helpers/test_patch_applier.py` & `truss-0.4.8rc4/truss/tests/templates/control/control/helpers/test_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/tests/templates/control/control/test_server.py` & `truss-0.4.8rc4/truss/tests/templates/control/control/test_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 def app(truss_container_fs, truss_original_hash):
     with _env_var({"HASH_TRUSS": truss_original_hash}):
         inf_serv_home = truss_container_fs / "app"
         control_app = create_app(
             {
                 "inference_server_home": inf_serv_home,
                 "inference_server_process_args": ["python", "inference_server.py"],
-                "control_server_host": "0.0.0.0",
+                "control_server_host": "*",
                 "control_server_port": 8081,
                 "inference_server_port": 8082,
                 "oversee_inference_server": False,
                 "pip_path": "pip",
             }
         )
         inference_server_controller = control_app.config["inference_server_controller"]
```

### Comparing `truss-0.4.6rc3/truss/tests/templates/core/server/common/test_util.py` & `truss-0.4.8rc4/truss/tests/templates/core/server/common/test_util.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/tests/templates/core/server/test_secrets_resolver.py` & `truss-0.4.8rc4/truss/tests/templates/core/server/test_secrets_resolver.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/tests/templates/server/common/test_external_resolver.py` & `truss-0.4.8rc4/truss/tests/templates/server/common/test_external_resolver.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/tests/templates/server/common/test_retry.py` & `truss-0.4.8rc4/truss/tests/templates/server/common/test_retry.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/tests/templates/server/test_model_wrapper.py` & `truss-0.4.8rc4/truss/tests/templates/server/test_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/tests/test_backward.py` & `truss-0.4.8rc4/truss/tests/test_backward.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/tests/test_build.py` & `truss-0.4.8rc4/truss/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/tests/test_context_builder_image.py` & `truss-0.4.8rc4/truss/tests/test_context_builder_image.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/tests/test_docker.py` & `truss-0.4.8rc4/truss/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/tests/test_notebooks.py` & `truss-0.4.8rc4/truss/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/tests/test_testing_utilities_for_other_tests.py` & `truss-0.4.8rc4/truss/tests/test_testing_utilities_for_other_tests.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/tests/test_truss_gatherer.py` & `truss-0.4.8rc4/truss/tests/test_truss_gatherer.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/tests/test_truss_handle.py` & `truss-0.4.8rc4/truss/tests/test_truss_handle.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,47 +92,61 @@
     tag = "test-build-image-tag:0.0.1"
     image = th.build_serving_docker_image(tag=tag)
     assert image.repo_tags[0] == tag
 
 
 @pytest.mark.integration
 @pytest.mark.parametrize(
-    "base_image, expected_fail",
+    "base_image, path, expected_fail",
     [
-        ("baseten/truss-server-base:3.9-v0.4.3", False),
-        ("python:3.8", False),
-        ("alpine", True),
-        ("python:2.7-slim", True),
-        ("python:3.5-slim", True),
+        ("baseten/truss-server-base:3.9-v0.4.3", "/usr/local/bin/python3", False),
+        ("python:3.8", "/usr/local/bin/python3", False),
+        ("python:3.11", "/usr/local/bin/python3", False),
+        ("python:alpine", "/usr/local/bin/python3", True),
+        ("python:2.7-slim", "/usr/local/bin/python", True),
+        ("python:3.7-slim", "/usr/local/bin/python3", True),
     ],
 )
 def test_build_serving_docker_image_from_user_base_image_live_reload(
-    custom_model_truss_dir, base_image, expected_fail
+    custom_model_truss_dir, base_image, path, expected_fail
 ):
     th = TrussHandle(custom_model_truss_dir)
-    th.set_base_image(base_image)
+    th.set_base_image(base_image, path)
     th.live_reload()
     try:
         th.build_serving_docker_image(cache=False)
     except DockerException as exc:
         assert expected_fail is True
         assert "It returned with code 1" in str(exc)
 
 
 @pytest.mark.integration
 def test_build_training_docker_image_from_user_base_image(custom_model_truss_dir):
     th = TrussHandle(custom_model_truss_dir)
-    th.set_base_image("baseten/truss-training-base:3.9-v0.4.3")
+    th.set_base_image(
+        "baseten/truss-training-base:3.9-v0.4.3", "/usr/local/bin/python3"
+    )
     th.build_training_docker_image()
 
 
 @pytest.mark.integration
 def test_docker_predict_custom_base_image(custom_model_truss_dir_with_pre_and_post):
     th = TrussHandle(custom_model_truss_dir_with_pre_and_post)
-    th.set_base_image("pytorch/pytorch")
+    th.set_base_image("pytorch/pytorch", "/opt/conda/bin/python")
+    with ensure_kill_all():
+        result = th.docker_predict([1, 2])
+        assert result == {"predictions": [4, 5]}
+
+
+@pytest.mark.integration
+def test_docker_predict_custom_base_image_with_python_executable_path(
+    custom_model_truss_dir_with_pre_and_post,
+):
+    th = TrussHandle(custom_model_truss_dir_with_pre_and_post)
+    th.set_base_image("pytorch/pytorch", "/opt/conda/bin/python")
     with ensure_kill_all():
         result = th.docker_predict([1, 2])
         assert result == {"predictions": [4, 5]}
 
 
 @pytest.mark.integration
 def test_build_docker_image_gpu(custom_model_truss_dir_for_gpu, tmp_path):
```

### Comparing `truss-0.4.6rc3/truss/tests/test_validation.py` & `truss-0.4.8rc4/truss/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/truss_config.py` & `truss-0.4.8rc4/truss/truss_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from truss.constants import HTTP_PUBLIC_BLOB_BACKEND
 from truss.errors import ValidationError
 from truss.types import ModelFrameworkType
 from truss.util.data_structures import transform_optional
 from truss.validation import (
     validate_cpu_spec,
     validate_memory_spec,
+    validate_python_executable_path,
     validate_secret_name,
 )
 
 DEFAULT_MODEL_FRAMEWORK_TYPE = ModelFrameworkType.CUSTOM
 DEFAULT_MODEL_TYPE = "Model"
 DEFAULT_MODEL_MODULE_DIR = "model"
 DEFAULT_BUNDLED_PACKAGES_DIR = "packages"
@@ -211,14 +212,36 @@
         return ExternalData([ExternalDataItem.from_dict(item) for item in items])
 
     def to_list(self) -> List[Dict[str, str]]:
         return [item.to_dict() for item in self.items]
 
 
 @dataclass
+class BaseImage:
+    image: str = ""
+    python_executable_path: str = ""
+
+    @staticmethod
+    def from_dict(d):
+        image = d.get("image", "")
+        python_executable_path = d.get("python_executable_path", "")
+        validate_python_executable_path(python_executable_path)
+        return BaseImage(
+            image=image,
+            python_executable_path=python_executable_path,
+        )
+
+    def to_dict(self):
+        return {
+            "image": self.image,
+            "python_executable_path": self.python_executable_path,
+        }
+
+
+@dataclass
 class TrussConfig:
     model_framework: ModelFrameworkType = DEFAULT_MODEL_FRAMEWORK_TYPE
     model_type: str = DEFAULT_MODEL_TYPE
     model_name: Optional[str] = None
 
     model_module_dir: str = DEFAULT_MODEL_MODULE_DIR
     model_class_filename: str = DEFAULT_MODEL_CLASS_FILENAME
@@ -237,18 +260,19 @@
     python_version: str = DEFAULT_PYTHON_VERSION
     examples_filename: str = DEFAULT_EXAMPLES_FILENAME
     secrets: Dict[str, str] = field(default_factory=dict)
     description: Optional[str] = None
     bundled_packages_dir: str = DEFAULT_BUNDLED_PACKAGES_DIR
     external_package_dirs: List[str] = field(default_factory=list)
     live_reload: bool = False
+    apply_library_patches: bool = True
     # spec_version is a version string
     spec_version: str = DEFAULT_SPEC_VERSION
     train: Train = field(default_factory=Train)
-    base_image: Optional[str] = None
+    base_image: Optional[BaseImage] = None
 
     @property
     def canonical_python_version(self) -> str:
         return {
             "py39": "3.9",
             "py38": "3.8",
             "py37": "3.7",
@@ -283,19 +307,20 @@
             secrets=d.get("secrets", {}),
             description=d.get("description", None),
             bundled_packages_dir=d.get(
                 "bundled_packages_dir", DEFAULT_BUNDLED_PACKAGES_DIR
             ),
             external_package_dirs=d.get("external_package_dirs", []),
             live_reload=d.get("live_reload", False),
+            apply_library_patches=d.get("apply_library_patches", True),
             train=Train.from_dict(d.get("train", {})),
             external_data=transform_optional(
                 d.get("external_data"), ExternalData.from_list
             ),
-            base_image=d.get("base_image", None),
+            base_image=transform_optional(d.get("base_image"), BaseImage.from_dict),
         )
         config.validate()
         return config
 
     @staticmethod
     def from_yaml(yaml_path: Path):
         with yaml_path.open() as yaml_file:
@@ -324,21 +349,25 @@
             "examples_filename": self.examples_filename,
             "secrets": self.secrets,
             "description": self.description,
             "bundled_packages_dir": self.bundled_packages_dir,
             "external_package_dirs": self.external_package_dirs,
             "live_reload": self.live_reload,
             "spec_version": self.spec_version,
+            "apply_library_patches": self.apply_library_patches,
             "train": self.train.to_dict(),
-            "base_image": self.base_image,
         }
         if self.external_data is not None:
             d["external_data"] = transform_optional(
                 self.external_data, lambda data: data.to_list()
             )
+        if self.base_image is not None:
+            d["base_image"] = transform_optional(
+                self.base_image, lambda data: data.to_dict()
+            )
         return d
 
     def clone(self):
         return TrussConfig.from_dict(self.to_dict())
 
     def validate(self):
         for secret_name in self.secrets:
```

### Comparing `truss-0.4.6rc3/truss/truss_gatherer.py` & `truss-0.4.8rc4/truss/truss_gatherer.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/truss_handle.py` & `truss-0.4.8rc4/truss/truss_handle.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 from truss.patch.signature import calc_truss_signature
 from truss.patch.types import TrussSignature
 from truss.readme_generator import generate_readme
 from truss.templates.server.common.serialization import (
     truss_msgpack_deserialize,
     truss_msgpack_serialize,
 )
-from truss.truss_config import ExternalData, ExternalDataItem, TrussConfig
+from truss.truss_config import BaseImage, ExternalData, ExternalDataItem, TrussConfig
 from truss.truss_spec import TrussSpec
 from truss.types import Example, PatchDetails
 from truss.util.path import copy_file_path, copy_tree_path, get_max_modified_time_of_dir
 from truss.validation import validate_secret_name
 
 logger: logging.Logger = logging.getLogger(__name__)
 
@@ -165,27 +165,29 @@
     def docker_run(
         self,
         build_dir: Optional[Path] = None,
         tag: Optional[str] = None,
         local_port: int = INFERENCE_SERVER_PORT,
         detach=True,
         patch_ping_url: Optional[str] = None,
+        wait_for_server_ready: bool = True,
     ):
         """
         Builds a docker image and runs it as a container. For control trusses,
         tries to patch.
 
         Args:
             build_dir: Directory to use for creating docker build context.
             tag: Tags to apply to docker image.
             local_port: Local port to forward inference server to.
             detach: Run docker container in detached mode.
             patch_ping_url:  Mostly for testing, if supplied then a live
                              reload capable truss queries for truss changes
                              by hitting this url.
+            wait_for_server_ready: If true, wait for server to pass readiness probe before returning.
 
         Returns:
             Container, which can be used to get information about the running,
             including its id. The id can be used to kill the container.
         """
         container_if_patched = self._try_patch()
         if container_if_patched is not None:
@@ -220,15 +222,15 @@
                 add_hosts=[("host.docker.internal", "host-gateway")],
             )
             logger.info(
                 f"Model server started on port {local_port}, docker container id {container.id}"
             )
         model_base_url = f"http://localhost:{local_port}/v1/models/model"
         try:
-            wait_for_truss(model_base_url, container)
+            wait_for_truss(model_base_url, container, wait_for_server_ready)
         except ContainerNotFoundError as err:
             raise err
         except (ContainerIsDownError, HTTPError, ConnectionError) as err:
             logger.error(self.serving_container_logs(follow=False, stream=False))
             raise err
 
         return container
@@ -689,17 +691,32 @@
 
         def enable_gpu_fn(conf: TrussConfig):
             new_resources = replace(conf.resources, use_gpu=True)
             return replace(conf, resources=new_resources)
 
         self._update_config(enable_gpu_fn)
 
-    def set_base_image(self, base_image: str):
+    def set_base_image(self, image: str, python_executable_path: str):
         """Set the base image for a given truss"""
-        self._update_config(lambda conf: replace(conf, base_image=base_image))
+
+        def define_base_image_fn(conf: TrussConfig):
+            if conf.base_image:
+                new_base_image = replace(
+                    conf.base_image,
+                    image=image,
+                    python_executable_path=python_executable_path,
+                )
+                return replace(conf, base_image=new_base_image)
+            new_base_image = BaseImage(
+                image,
+                python_executable_path,
+            )
+            return replace(conf, base_image=new_base_image)
+
+        self._update_config(define_base_image_fn)
 
     @proxy_to_shadow_if_scattered
     def patch_container(self, patch_request: Dict):
         """Patch changes onto the container running this Truss.
 
         Useful for local incremental development.
         TODO(pankaj): Turn patch_request into a dataclass
@@ -1024,52 +1041,24 @@
                     raise RuntimeError(
                         f"Truss referes to external package at "
                         f"{path.resolve()} but that path does not exist."
                     )
 
 
 def _prediction_flow(model, request: Dict):
-    """This flow attempts to mimic the request life-cycle of a kserve server"""
-    _validate_request_input(request)
-    _map_instances_inputs(request)
+    """This flow attempts to mimic the request life-cycle of a server"""
+    # TODO: can we just call ModelWrapper directly here?
     if hasattr(model, "preprocess"):
         request = model.preprocess(request)
     response = model.predict(request)
     if hasattr(model, "postprocess"):
         response = model.postprocess(response)
     return response
 
 
-def _map_instances_inputs(request: Dict) -> Dict[str, Any]:
-    # TODO(pankaj) Share this code with baseten deployed code
-    if "instances" in request and "inputs" not in request:
-        request["inputs"] = request["instances"]
-    elif "inputs" in request and "instances" not in request:
-        request["instances"] = request["inputs"]
-    return request
-
-
-def _validate_request_input(request: Dict) -> None:
-    # TODO(pankaj) Should these checks be there?
-    if _is_invalid_list_input_prop(request, "instances") or _is_invalid_list_input_prop(
-        request, "inputs"
-    ):
-        raise Exception('Expected "instances" or "inputs" to be a list')
-
-
-def _is_invalid_list_input_prop(request: Dict, prop: str) -> bool:
-    return prop in request and not _is_valid_list_type(request[prop])
-
-
-def _is_valid_list_type(obj) -> bool:
-    import numpy as np
-
-    return isinstance(obj, (list, np.ndarray))
-
-
 def _wait_for_docker_build(container) -> None:
     for attempt in Retrying(stop=stop_after_attempt(5), wait=wait_fixed(2)):
         state = get_container_state(container)
         logger.info(f"Container state: {state}")
         if state == DockerStates.OOMKILLED or state == DockerStates.DEAD:
             raise ContainerIsDownError(f"Container errored out in state: {state}.")
         with attempt:
@@ -1085,25 +1074,27 @@
         | retry_if_exception_type(exceptions.ConnectionError)
     ),
 )
 def _wait_for_model_server(url: str) -> Response:
     return requests.get(url)
 
 
-def wait_for_truss(url: str, container) -> None:
+def wait_for_truss(
+    url: str, container: str, wait_for_server_ready: bool = True
+) -> None:
     from python_on_whales.exceptions import NoSuchContainer
 
     try:
         _wait_for_docker_build(container)
     except NoSuchContainer:
         raise ContainerNotFoundError(message=f"Container {container} was not found")
     except RetryError as retry_err:
         retry_err.reraise()
-
-    _wait_for_model_server(url)
+    if wait_for_server_ready:
+        _wait_for_model_server(url)
 
 
 def _prepare_secrets_mount_dir() -> Path:
     LocalConfigHandler.sync_secrets_mount_dir()
     return LocalConfigHandler.secrets_dir_path()
```

### Comparing `truss-0.4.6rc3/truss/truss_spec.py` & `truss-0.4.8rc4/truss/truss_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,13 +181,21 @@
         return self._config.description
 
     @property
     def live_reload(self) -> bool:
         return self._config.live_reload
 
     @property
-    def base_image(self) -> Optional[str]:
-        return self._config.base_image
+    def base_image_name(self) -> Optional[str]:
+        return self._config.base_image.image
+
+    @property
+    def python_executable_path(self) -> str:
+        return self._config.base_image.python_executable_path
+
+    @property
+    def apply_library_patches(self) -> bool:
+        return self._config.apply_library_patches
 
 
 def _join_lines(lines: List[str]) -> str:
     return "\n".join(lines) + "\n"
```

### Comparing `truss-0.4.6rc3/truss/types.py` & `truss-0.4.8rc4/truss/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/util/gpu.py` & `truss-0.4.8rc4/truss/util/gpu.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/util/path.py` & `truss-0.4.8rc4/truss/util/path.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.6rc3/truss/validation.py` & `truss-0.4.8rc4/truss/validation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+from pathlib import Path
 from typing import Pattern, Set
 
 from truss.errors import ValidationError
 
 SECRET_NAME_MATCH_REGEX: Pattern[str] = re.compile(r"^[-._a-zA-Z0-9]+$")
 MILLI_CPU_REGEX: Pattern[str] = re.compile(r"^[0-9.]*m$")
 MEMORY_REGEX: Pattern[str] = re.compile(r"^[0-9.]*(\w*)$")
@@ -68,7 +69,18 @@
 
 def _is_numeric(number_like: str) -> bool:
     try:
         float(number_like)
         return True
     except ValueError:
         return False
+
+
+def validate_python_executable_path(path: str) -> None:
+    """
+    This python executable path determines the python executable
+    used to run the inference server - check to see that it is an absolute path
+    """
+    if path and not Path(path).is_absolute():
+        raise ValidationError(
+            f"Invalid relative python executable path {path}. Provide an absolute path"
+        )
```

### Comparing `truss-0.4.6rc3/PKG-INFO` & `truss-0.4.8rc4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 Metadata-Version: 2.1
 Name: truss
-Version: 0.4.6rc3
+Version: 0.4.8rc4
 Summary: A seamless bridge from model development to model delivery
 Home-page: https://github.com/basetenlabs/truss
 License: MIT
 Keywords: MLOps,AI,Model Serving,Model Deployment,Machine Learning
 Author: Pankaj Gupta
 Author-email: pankaj@baseten.co
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: blake3 (>=0.3.3,<0.4.0)
 Requires-Dist: cloudpickle (>=2.2.0,<3.0.0)
+Requires-Dist: dockerfile (>=3.2.0,<4.0.0)
+Requires-Dist: fastapi (>=0.95.0,<0.96.0)
+Requires-Dist: joblib (>=1.2.0,<2.0.0)
 Requires-Dist: msgpack (>=1.0.2)
 Requires-Dist: msgpack-numpy (>=0.4.7.1)
 Requires-Dist: numpy (==1.23.5)
 Requires-Dist: packaging (>=20.9,<21.0)
+Requires-Dist: psutil (>=5.9.4,<6.0.0)
 Requires-Dist: python-json-logger (>=2.0.2)
 Requires-Dist: python-on-whales (>=0.46.0,<0.47.0)
 Requires-Dist: single-source (>=0.3.0,<0.4.0)
 Requires-Dist: tenacity (>=8.0.1,<9.0.0)
+Requires-Dist: uvicorn (>=0.21.1,<0.22.0)
 Project-URL: Bug Reports, https://github.com/basetenlabs/truss/issues
 Project-URL: Baseten, https://baseten.co
 Project-URL: Documentation, https://truss.baseten.co
 Project-URL: Homepage, https://truss.baseten.co
 Project-URL: Repository, https://github.com/basetenlabs/truss
 Description-Content-Type: text/markdown
```

