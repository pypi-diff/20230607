# Comparing `tmp/truss-0.4.8rc5.tar.gz` & `tmp/truss-0.4.8rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truss-0.4.8rc5.tar", max compression
+gzip compressed data, was "truss-0.4.8rc7.tar", max compression
```

## Comparing `truss-0.4.8rc5.tar` & `truss-0.4.8rc7.tar`

### file list

```diff
@@ -1,172 +1,172 @@
--rw-r--r--   0        0        0     5483 2023-06-06 22:53:01.352252 truss-0.4.8rc5/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2576 2023-06-06 22:53:01.352252 truss-0.4.8rc5/CONTRIBUTING.md
--rw-r--r--   0        0        0     1064 2023-06-06 22:53:01.356252 truss-0.4.8rc5/LICENSE
--rw-r--r--   0        0        0     5958 2023-06-06 22:53:01.356252 truss-0.4.8rc5/README.md
--rw-r--r--   0        0        0     3077 2023-06-06 22:53:01.356252 truss-0.4.8rc5/ROADMAP.md
--rw-r--r--   0        0        0      820 2023-06-06 22:53:01.356252 truss-0.4.8rc5/context_builder.Dockerfile
--rw-r--r--   0        0        0     2319 2023-06-06 22:53:01.480253 truss-0.4.8rc5/pyproject.toml
--rw-r--r--   0        0        0      330 2023-06-06 22:53:01.480253 truss-0.4.8rc5/truss/__init__.py
--rw-r--r--   0        0        0      252 2023-06-06 22:53:01.480253 truss-0.4.8rc5/truss/blob/blob_backend.py
--rw-r--r--   0        0        0      733 2023-06-06 22:53:01.480253 truss-0.4.8rc5/truss/blob/blob_backend_registry.py
--rw-r--r--   0        0        0      648 2023-06-06 22:53:01.480253 truss-0.4.8rc5/truss/blob/http_public_blob_backend.py
--rw-r--r--   0        0        0    13295 2023-06-06 22:53:01.480253 truss-0.4.8rc5/truss/build.py
--rw-r--r--   0        0        0    10452 2023-06-06 22:53:01.480253 truss-0.4.8rc5/truss/cli.py
--rw-r--r--   0        0        0     2813 2023-06-06 22:53:01.480253 truss-0.4.8rc5/truss/constants.py
--rw-r--r--   0        0        0     1294 2023-06-06 22:53:01.480253 truss-0.4.8rc5/truss/contexts/image_builder/image_builder.py
--rw-r--r--   0        0        0     8411 2023-06-06 22:53:01.480253 truss-0.4.8rc5/truss/contexts/image_builder/serving_image_builder.py
--rw-r--r--   0        0        0     4684 2023-06-06 22:53:01.480253 truss-0.4.8rc5/truss/contexts/image_builder/training_image_builder.py
--rw-r--r--   0        0        0     1896 2023-06-06 22:53:01.480253 truss-0.4.8rc5/truss/contexts/image_builder/util.py
--rw-r--r--   0        0        0     2014 2023-06-06 22:53:01.480253 truss-0.4.8rc5/truss/contexts/local_loader/docker_build_emulator.py
--rw-r--r--   0        0        0     1823 2023-06-06 22:53:01.480253 truss-0.4.8rc5/truss/contexts/local_loader/load_model_local.py
--rw-r--r--   0        0        0     2239 2023-06-06 22:53:01.480253 truss-0.4.8rc5/truss/contexts/local_loader/train_local.py
--rw-r--r--   0        0        0     5801 2023-06-06 22:53:01.480253 truss-0.4.8rc5/truss/contexts/local_loader/truss_module_loader.py
--rw-r--r--   0        0        0      853 2023-06-06 22:53:01.480253 truss-0.4.8rc5/truss/contexts/local_loader/utils.py
--rw-r--r--   0        0        0      436 2023-06-06 22:53:01.480253 truss-0.4.8rc5/truss/contexts/truss_context.py
--rw-r--r--   0        0        0      394 2023-06-06 22:53:01.480253 truss-0.4.8rc5/truss/decorators.py
--rw-r--r--   0        0        0     3641 2023-06-06 22:53:01.480253 truss-0.4.8rc5/truss/docker.py
--rw-r--r--   0        0        0     3759 2023-06-06 22:53:01.480253 truss-0.4.8rc5/truss/environment_inference/requirements_inference.py
--rw-r--r--   0        0        0      643 2023-06-06 22:53:01.480253 truss-0.4.8rc5/truss/errors.py
--rw-r--r--   0        0        0      824 2023-06-06 22:53:01.480253 truss-0.4.8rc5/truss/local/local_config.py
--rw-r--r--   0        0        0     3896 2023-06-06 22:53:01.480253 truss-0.4.8rc5/truss/local/local_config_handler.py
--rw-r--r--   0        0        0     2713 2023-06-06 22:53:01.480253 truss-0.4.8rc5/truss/model_framework.py
--rw-r--r--   0        0        0     1687 2023-06-06 22:53:01.480253 truss-0.4.8rc5/truss/model_frameworks/__init__.py
--rw-r--r--   0        0        0     1895 2023-06-06 22:53:01.480253 truss-0.4.8rc5/truss/model_frameworks/huggingface_transformer.py
--rw-r--r--   0        0        0      918 2023-06-06 22:53:01.480253 truss-0.4.8rc5/truss/model_frameworks/keras.py
--rw-r--r--   0        0        0     1237 2023-06-06 22:53:01.480253 truss-0.4.8rc5/truss/model_frameworks/lightgbm.py
--rw-r--r--   0        0        0     2410 2023-06-06 22:53:01.480253 truss-0.4.8rc5/truss/model_frameworks/mlflow.py
--rw-r--r--   0        0        0     2441 2023-06-06 22:53:01.480253 truss-0.4.8rc5/truss/model_frameworks/pytorch.py
--rw-r--r--   0        0        0     1232 2023-06-06 22:53:01.480253 truss-0.4.8rc5/truss/model_frameworks/sklearn.py
--rw-r--r--   0        0        0     1027 2023-06-06 22:53:01.480253 truss-0.4.8rc5/truss/model_frameworks/xgboost.py
--rw-r--r--   0        0        0     6521 2023-06-06 22:53:01.480253 truss-0.4.8rc5/truss/model_inference.py
--rw-r--r--   0        0        0      510 2023-06-06 22:53:01.480253 truss-0.4.8rc5/truss/notebook.py
--rw-r--r--   0        0        0    11065 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/patch/calc_patch.py
--rw-r--r--   0        0        0      774 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/patch/dir_signature.py
--rw-r--r--   0        0        0     2378 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/patch/hash.py
--rw-r--r--   0        0        0      468 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/patch/signature.py
--rw-r--r--   0        0        0      937 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/patch/types.py
--rw-r--r--   0        0        0      237 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/pytest.ini
--rw-r--r--   0        0        0      705 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/readme_generator.py
--rw-r--r--   0        0        0     2482 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/README.md.jinja
--rw-r--r--   0        0        0        0 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/__init__.py
--rw-r--r--   0        0        0     2310 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/base.Dockerfile.jinja
--rw-r--r--   0        0        0     2190 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/control/control/application.py
--rw-r--r--   0        0        0     4083 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/control/control/endpoints.py
--rw-r--r--   0        0        0      413 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/control/control/helpers/context_managers.py
--rw-r--r--   0        0        0      877 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/control/control/helpers/errors.py
--rw-r--r--   0        0        0     5801 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/control/control/helpers/inference_server_controller.py
--rw-r--r--   0        0        0     2596 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/control/control/helpers/inference_server_process_controller.py
--rw-r--r--   0        0        0     2399 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/control/control/helpers/inference_server_starter.py
--rw-r--r--   0        0        0     5389 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/control/control/helpers/patch_applier.py
--rw-r--r--   0        0        0     3070 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/control/control/helpers/types.py
--rw-r--r--   0        0        0     1843 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/control/control/server.py
--rw-r--r--   0        0        0       86 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/control/requirements.txt
--rw-r--r--   0        0        0       48 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/custom/examples.yaml
--rw-r--r--   0        0        0        0 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/custom/model/__init__.py
--rw-r--r--   0        0        0      534 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/custom/model/model.py
--rw-r--r--   0        0        0      460 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/custom/train/train.py
--rw-r--r--   0        0        0        0 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/huggingface_transformer/model/__init__.py
--rw-r--r--   0        0        0     1827 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/huggingface_transformer/model/model.py
--rw-r--r--   0        0        0       47 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/huggingface_transformer/requirements.txt
--rw-r--r--   0        0        0        0 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/keras/model/__init__.py
--rw-r--r--   0        0        0      728 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/keras/model/model.py
--rw-r--r--   0        0        0        0 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/lightgbm/model/__init__.py
--rw-r--r--   0        0        0     1251 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/lightgbm/model/model.py
--rw-r--r--   0        0        0        0 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/mlflow/model/__init__.py
--rw-r--r--   0        0        0      751 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/mlflow/model/model.py
--rw-r--r--   0        0        0        0 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/pipeline/model/__init__.py
--rw-r--r--   0        0        0      430 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/pipeline/model/model.py
--rw-r--r--   0        0        0        0 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/pytorch/model/__init__.py
--rw-r--r--   0        0        0     1263 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/pytorch/model/model.py
--rw-r--r--   0        0        0        0 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/server/__init__.py
--rw-r--r--   0        0        0       85 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/server/common/__init__.py
--rw-r--r--   0        0        0     2433 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/server/common/errors.py
--rw-r--r--   0        0        0     1352 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/server/common/logging.py
--rw-r--r--   0        0        0     2382 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/server/common/patches/whisper/patch.py
--rw-r--r--   0        0        0     1450 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/server/common/patches.py
--rw-r--r--   0        0        0      593 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/server/common/retry.py
--rw-r--r--   0        0        0     3318 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/server/common/serialization.py
--rw-r--r--   0        0        0     9426 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/server/common/truss_server.py
--rw-r--r--   0        0        0     1445 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/server/common/util.py
--rw-r--r--   0        0        0      727 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/server/inference_server.py
--rw-r--r--   0        0        0     6219 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/server/model_wrapper.py
--rw-r--r--   0        0        0      235 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/server/requirements.txt
--rw-r--r--   0        0        0     2586 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/server.Dockerfile.jinja
--rw-r--r--   0        0        0      138 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/shared/README.md
--rw-r--r--   0        0        0        0 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/shared/__init__.py
--rw-r--r--   0        0        0     1430 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/shared/secrets_resolver.py
--rw-r--r--   0        0        0        0 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/sklearn/model/__init__.py
--rw-r--r--   0        0        0     1221 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/sklearn/model/model.py
--rw-r--r--   0        0        0     3400 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/training/job.py
--rw-r--r--   0        0        0       12 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/training/requirements.txt
--rw-r--r--   0        0        0      491 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/training.Dockerfile.jinja
--rw-r--r--   0        0        0        0 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/xgboost/model/__init__.py
--rw-r--r--   0        0        0     1453 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/templates/xgboost/model/model.py
--rw-r--r--   0        0        0    30286 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/test_data/auto-mpg.data
--rw-r--r--   0        0        0       93 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/test_data/context_builder_image_test/Dockerfile
--rw-r--r--   0        0        0       72 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/test_data/context_builder_image_test/test.py
--rw-r--r--   0        0        0     1394 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/test_data/happy.ipynb
--rw-r--r--   0        0        0     1267 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/test_data/patch_ping_test_server/app.py
--rw-r--r--   0        0        0    23279 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/test_data/pima-indians-diabetes.csv
--rw-r--r--   0        0        0     1586 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/test_data/readme_int_example.md
--rw-r--r--   0        0        0     1607 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/test_data/readme_no_example.md
--rw-r--r--   0        0        0     1726 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/test_data/readme_str_example.md
--rw-r--r--   0        0        0     2067 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/test_data/server.Dockerfile
--rw-r--r--   0        0        0      669 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/test_data/server_conformance_test_truss/config.yaml
--rw-r--r--   0        0        0        0 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/test_data/server_conformance_test_truss/model/__init__.py
--rw-r--r--   0        0        0      597 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/test_data/server_conformance_test_truss/model/model.py
--rw-r--r--   0        0        0      669 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/test_data/test_truss/config.yaml
--rw-r--r--   0        0        0       48 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/test_data/test_truss/examples.yaml
--rw-r--r--   0        0        0        0 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/test_data/test_truss/model/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/test_data/test_truss/model/dummy
--rw-r--r--   0        0        0      534 2023-06-06 22:53:01.484253 truss-0.4.8rc5/truss/test_data/test_truss/model/model.py
--rw-r--r--   0        0        0        0 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/tests/__init__.py
--rw-r--r--   0        0        0    20811 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/tests/conftest.py
--rw-r--r--   0        0        0     1255 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/tests/contexts/image_builder/test_serving_image_builder.py
--rw-r--r--   0        0        0      783 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/tests/contexts/local_loader/test_load_local.py
--rw-r--r--   0        0        0     5337 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/tests/contexts/local_loader/test_truss_module_finder.py
--rw-r--r--   0        0        0      968 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/tests/environments_inference/test_requirements_inference.py
--rw-r--r--   0        0        0        0 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/tests/local/__init__.py
--rw-r--r--   0        0        0     2245 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/tests/local/test_local_config_handler.py
--rw-r--r--   0        0        0        0 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/tests/model_frameworks/__init__.py
--rw-r--r--   0        0        0     3293 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/tests/model_frameworks/test_huggingface_transformer_framework.py
--rw-r--r--   0        0        0     2789 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/tests/model_frameworks/test_keras_framework.py
--rw-r--r--   0        0        0     2409 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/tests/model_frameworks/test_lightgbm_framework.py
--rw-r--r--   0        0        0     1479 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/tests/model_frameworks/test_pytorch_framework.py
--rw-r--r--   0        0        0     2427 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/tests/model_frameworks/test_sklearn_framework.py
--rw-r--r--   0        0        0     2437 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/tests/model_frameworks/test_xgboost_framework.py
--rw-r--r--   0        0        0    11109 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/tests/patch/test_calc_patch.py
--rw-r--r--   0        0        0      487 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/tests/patch/test_dir_signature.py
--rw-r--r--   0        0        0     5983 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/tests/patch/test_hash.py
--rw-r--r--   0        0        0      394 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/tests/patch/test_signature.py
--rw-r--r--   0        0        0      273 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/tests/patch/test_types.py
--rw-r--r--   0        0        0    10415 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/tests/samples.py
--rw-r--r--   0        0        0      283 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/tests/templates/control/control/helpers/test_context_managers.py
--rw-r--r--   0        0        0     1976 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/tests/templates/control/control/helpers/test_patch_applier.py
--rw-r--r--   0        0        0     6931 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/tests/templates/control/control/test_server.py
--rw-r--r--   0        0        0      750 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/tests/templates/core/server/common/test_util.py
--rw-r--r--   0        0        0     1539 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/tests/templates/core/server/test_secrets_resolver.py
--rw-r--r--   0        0        0     2038 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/tests/templates/server/common/test_retry.py
--rw-r--r--   0        0        0     2252 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/tests/templates/server/test_model_wrapper.py
--rw-r--r--   0        0        0     1910 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/tests/test_backward.py
--rw-r--r--   0        0        0     8260 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/tests/test_build.py
--rw-r--r--   0        0        0     3181 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/tests/test_config.py
--rw-r--r--   0        0        0     1188 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/tests/test_context_builder_image.py
--rw-r--r--   0        0        0      517 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/tests/test_docker.py
--rw-r--r--   0        0        0     4905 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/tests/test_model_inference.py
--rw-r--r--   0        0        0      656 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/tests/test_notebooks.py
--rw-r--r--   0        0        0     1483 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/tests/test_testing_utilities_for_other_tests.py
--rw-r--r--   0        0        0     1252 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/tests/test_truss_gatherer.py
--rw-r--r--   0        0        0    33899 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/tests/test_truss_handle.py
--rw-r--r--   0        0        0      434 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/tests/test_truss_util.py
--rw-r--r--   0        0        0     1865 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/tests/test_validation.py
--rw-r--r--   0        0        0    13143 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/truss_config.py
--rw-r--r--   0        0        0     2845 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/truss_gatherer.py
--rw-r--r--   0        0        0    40919 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/truss_handle.py
--rw-r--r--   0        0        0     5671 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/truss_spec.py
--rw-r--r--   0        0        0     2124 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/types.py
--rw-r--r--   0        0        0      227 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/util/data_structures.py
--rw-r--r--   0        0        0      553 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/util/gpu.py
--rw-r--r--   0        0        0      333 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/util/jinja.py
--rw-r--r--   0        0        0     2018 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/util/path.py
--rw-r--r--   0        0        0     2736 2023-06-06 22:53:01.488253 truss-0.4.8rc5/truss/validation.py
--rw-r--r--   0        0        0     7595 1970-01-01 00:00:00.000000 truss-0.4.8rc5/PKG-INFO
+-rw-r--r--   0        0        0     5483 2023-06-07 18:37:55.725275 truss-0.4.8rc7/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2576 2023-06-07 18:37:55.725275 truss-0.4.8rc7/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1064 2023-06-07 18:37:55.725275 truss-0.4.8rc7/LICENSE
+-rw-r--r--   0        0        0     5958 2023-06-07 18:37:55.725275 truss-0.4.8rc7/README.md
+-rw-r--r--   0        0        0     3077 2023-06-07 18:37:55.725275 truss-0.4.8rc7/ROADMAP.md
+-rw-r--r--   0        0        0      820 2023-06-07 18:37:55.725275 truss-0.4.8rc7/context_builder.Dockerfile
+-rw-r--r--   0        0        0     2319 2023-06-07 18:37:55.793276 truss-0.4.8rc7/pyproject.toml
+-rw-r--r--   0        0        0      330 2023-06-07 18:37:55.793276 truss-0.4.8rc7/truss/__init__.py
+-rw-r--r--   0        0        0      252 2023-06-07 18:37:55.793276 truss-0.4.8rc7/truss/blob/blob_backend.py
+-rw-r--r--   0        0        0      733 2023-06-07 18:37:55.793276 truss-0.4.8rc7/truss/blob/blob_backend_registry.py
+-rw-r--r--   0        0        0      648 2023-06-07 18:37:55.793276 truss-0.4.8rc7/truss/blob/http_public_blob_backend.py
+-rw-r--r--   0        0        0    13295 2023-06-07 18:37:55.793276 truss-0.4.8rc7/truss/build.py
+-rw-r--r--   0        0        0    10452 2023-06-07 18:37:55.793276 truss-0.4.8rc7/truss/cli.py
+-rw-r--r--   0        0        0     2813 2023-06-07 18:37:55.793276 truss-0.4.8rc7/truss/constants.py
+-rw-r--r--   0        0        0     1294 2023-06-07 18:37:55.793276 truss-0.4.8rc7/truss/contexts/image_builder/image_builder.py
+-rw-r--r--   0        0        0     8411 2023-06-07 18:37:55.793276 truss-0.4.8rc7/truss/contexts/image_builder/serving_image_builder.py
+-rw-r--r--   0        0        0     4684 2023-06-07 18:37:55.793276 truss-0.4.8rc7/truss/contexts/image_builder/training_image_builder.py
+-rw-r--r--   0        0        0     1896 2023-06-07 18:37:55.793276 truss-0.4.8rc7/truss/contexts/image_builder/util.py
+-rw-r--r--   0        0        0     2111 2023-06-07 18:37:55.793276 truss-0.4.8rc7/truss/contexts/local_loader/docker_build_emulator.py
+-rw-r--r--   0        0        0     1823 2023-06-07 18:37:55.793276 truss-0.4.8rc7/truss/contexts/local_loader/load_model_local.py
+-rw-r--r--   0        0        0     2239 2023-06-07 18:37:55.793276 truss-0.4.8rc7/truss/contexts/local_loader/train_local.py
+-rw-r--r--   0        0        0     5801 2023-06-07 18:37:55.793276 truss-0.4.8rc7/truss/contexts/local_loader/truss_module_loader.py
+-rw-r--r--   0        0        0      853 2023-06-07 18:37:55.793276 truss-0.4.8rc7/truss/contexts/local_loader/utils.py
+-rw-r--r--   0        0        0      436 2023-06-07 18:37:55.793276 truss-0.4.8rc7/truss/contexts/truss_context.py
+-rw-r--r--   0        0        0      394 2023-06-07 18:37:55.793276 truss-0.4.8rc7/truss/decorators.py
+-rw-r--r--   0        0        0     3641 2023-06-07 18:37:55.793276 truss-0.4.8rc7/truss/docker.py
+-rw-r--r--   0        0        0     3759 2023-06-07 18:37:55.793276 truss-0.4.8rc7/truss/environment_inference/requirements_inference.py
+-rw-r--r--   0        0        0      643 2023-06-07 18:37:55.793276 truss-0.4.8rc7/truss/errors.py
+-rw-r--r--   0        0        0      824 2023-06-07 18:37:55.793276 truss-0.4.8rc7/truss/local/local_config.py
+-rw-r--r--   0        0        0     3896 2023-06-07 18:37:55.793276 truss-0.4.8rc7/truss/local/local_config_handler.py
+-rw-r--r--   0        0        0     2713 2023-06-07 18:37:55.793276 truss-0.4.8rc7/truss/model_framework.py
+-rw-r--r--   0        0        0     1687 2023-06-07 18:37:55.793276 truss-0.4.8rc7/truss/model_frameworks/__init__.py
+-rw-r--r--   0        0        0     1895 2023-06-07 18:37:55.793276 truss-0.4.8rc7/truss/model_frameworks/huggingface_transformer.py
+-rw-r--r--   0        0        0      918 2023-06-07 18:37:55.793276 truss-0.4.8rc7/truss/model_frameworks/keras.py
+-rw-r--r--   0        0        0     1237 2023-06-07 18:37:55.793276 truss-0.4.8rc7/truss/model_frameworks/lightgbm.py
+-rw-r--r--   0        0        0     2410 2023-06-07 18:37:55.793276 truss-0.4.8rc7/truss/model_frameworks/mlflow.py
+-rw-r--r--   0        0        0     2441 2023-06-07 18:37:55.793276 truss-0.4.8rc7/truss/model_frameworks/pytorch.py
+-rw-r--r--   0        0        0     1232 2023-06-07 18:37:55.793276 truss-0.4.8rc7/truss/model_frameworks/sklearn.py
+-rw-r--r--   0        0        0     1027 2023-06-07 18:37:55.793276 truss-0.4.8rc7/truss/model_frameworks/xgboost.py
+-rw-r--r--   0        0        0     6521 2023-06-07 18:37:55.793276 truss-0.4.8rc7/truss/model_inference.py
+-rw-r--r--   0        0        0      510 2023-06-07 18:37:55.793276 truss-0.4.8rc7/truss/notebook.py
+-rw-r--r--   0        0        0    11065 2023-06-07 18:37:55.793276 truss-0.4.8rc7/truss/patch/calc_patch.py
+-rw-r--r--   0        0        0      774 2023-06-07 18:37:55.793276 truss-0.4.8rc7/truss/patch/dir_signature.py
+-rw-r--r--   0        0        0     2378 2023-06-07 18:37:55.793276 truss-0.4.8rc7/truss/patch/hash.py
+-rw-r--r--   0        0        0      468 2023-06-07 18:37:55.793276 truss-0.4.8rc7/truss/patch/signature.py
+-rw-r--r--   0        0        0      937 2023-06-07 18:37:55.793276 truss-0.4.8rc7/truss/patch/types.py
+-rw-r--r--   0        0        0      237 2023-06-07 18:37:55.793276 truss-0.4.8rc7/truss/pytest.ini
+-rw-r--r--   0        0        0      705 2023-06-07 18:37:55.793276 truss-0.4.8rc7/truss/readme_generator.py
+-rw-r--r--   0        0        0     2482 2023-06-07 18:37:55.793276 truss-0.4.8rc7/truss/templates/README.md.jinja
+-rw-r--r--   0        0        0        0 2023-06-07 18:37:55.793276 truss-0.4.8rc7/truss/templates/__init__.py
+-rw-r--r--   0        0        0     1925 2023-06-07 18:37:55.793276 truss-0.4.8rc7/truss/templates/base.Dockerfile.jinja
+-rw-r--r--   0        0        0     2190 2023-06-07 18:37:55.793276 truss-0.4.8rc7/truss/templates/control/control/application.py
+-rw-r--r--   0        0        0     4083 2023-06-07 18:37:55.793276 truss-0.4.8rc7/truss/templates/control/control/endpoints.py
+-rw-r--r--   0        0        0      413 2023-06-07 18:37:55.793276 truss-0.4.8rc7/truss/templates/control/control/helpers/context_managers.py
+-rw-r--r--   0        0        0      877 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/control/control/helpers/errors.py
+-rw-r--r--   0        0        0     5801 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/control/control/helpers/inference_server_controller.py
+-rw-r--r--   0        0        0     2596 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/control/control/helpers/inference_server_process_controller.py
+-rw-r--r--   0        0        0     2399 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/control/control/helpers/inference_server_starter.py
+-rw-r--r--   0        0        0     5389 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/control/control/helpers/patch_applier.py
+-rw-r--r--   0        0        0     3070 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/control/control/helpers/types.py
+-rw-r--r--   0        0        0     1861 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/control/control/server.py
+-rw-r--r--   0        0        0       86 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/control/requirements.txt
+-rw-r--r--   0        0        0       48 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/custom/examples.yaml
+-rw-r--r--   0        0        0        0 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/custom/model/__init__.py
+-rw-r--r--   0        0        0      534 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/custom/model/model.py
+-rw-r--r--   0        0        0      460 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/custom/train/train.py
+-rw-r--r--   0        0        0        0 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/huggingface_transformer/model/__init__.py
+-rw-r--r--   0        0        0     1827 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/huggingface_transformer/model/model.py
+-rw-r--r--   0        0        0       47 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/huggingface_transformer/requirements.txt
+-rw-r--r--   0        0        0        0 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/keras/model/__init__.py
+-rw-r--r--   0        0        0      728 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/keras/model/model.py
+-rw-r--r--   0        0        0        0 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/lightgbm/model/__init__.py
+-rw-r--r--   0        0        0     1251 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/lightgbm/model/model.py
+-rw-r--r--   0        0        0        0 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/mlflow/model/__init__.py
+-rw-r--r--   0        0        0      751 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/mlflow/model/model.py
+-rw-r--r--   0        0        0        0 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/pipeline/model/__init__.py
+-rw-r--r--   0        0        0      430 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/pipeline/model/model.py
+-rw-r--r--   0        0        0        0 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/pytorch/model/__init__.py
+-rw-r--r--   0        0        0     1263 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/pytorch/model/model.py
+-rw-r--r--   0        0        0        0 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/server/__init__.py
+-rw-r--r--   0        0        0       85 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/server/common/__init__.py
+-rw-r--r--   0        0        0     2433 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/server/common/errors.py
+-rw-r--r--   0        0        0     1352 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/server/common/logging.py
+-rw-r--r--   0        0        0     2382 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/server/common/patches/whisper/patch.py
+-rw-r--r--   0        0        0     1450 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/server/common/patches.py
+-rw-r--r--   0        0        0      593 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/server/common/retry.py
+-rw-r--r--   0        0        0     3318 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/server/common/serialization.py
+-rw-r--r--   0        0        0     9426 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/server/common/truss_server.py
+-rw-r--r--   0        0        0     1445 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/server/common/util.py
+-rw-r--r--   0        0        0      727 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/server/inference_server.py
+-rw-r--r--   0        0        0     6219 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/server/model_wrapper.py
+-rw-r--r--   0        0        0      235 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/server/requirements.txt
+-rw-r--r--   0        0        0     2769 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/server.Dockerfile.jinja
+-rw-r--r--   0        0        0      138 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/shared/README.md
+-rw-r--r--   0        0        0        0 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/shared/__init__.py
+-rw-r--r--   0        0        0     1430 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/shared/secrets_resolver.py
+-rw-r--r--   0        0        0        0 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/sklearn/model/__init__.py
+-rw-r--r--   0        0        0     1221 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/sklearn/model/model.py
+-rw-r--r--   0        0        0     3400 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/training/job.py
+-rw-r--r--   0        0        0       12 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/training/requirements.txt
+-rw-r--r--   0        0        0      491 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/training.Dockerfile.jinja
+-rw-r--r--   0        0        0        0 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/xgboost/model/__init__.py
+-rw-r--r--   0        0        0     1453 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/templates/xgboost/model/model.py
+-rw-r--r--   0        0        0    30286 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/test_data/auto-mpg.data
+-rw-r--r--   0        0        0       93 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/test_data/context_builder_image_test/Dockerfile
+-rw-r--r--   0        0        0       72 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/test_data/context_builder_image_test/test.py
+-rw-r--r--   0        0        0     1394 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/test_data/happy.ipynb
+-rw-r--r--   0        0        0     1267 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/test_data/patch_ping_test_server/app.py
+-rw-r--r--   0        0        0    23279 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/test_data/pima-indians-diabetes.csv
+-rw-r--r--   0        0        0     1586 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/test_data/readme_int_example.md
+-rw-r--r--   0        0        0     1607 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/test_data/readme_no_example.md
+-rw-r--r--   0        0        0     1726 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/test_data/readme_str_example.md
+-rw-r--r--   0        0        0     1550 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/test_data/server.Dockerfile
+-rw-r--r--   0        0        0      669 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/test_data/server_conformance_test_truss/config.yaml
+-rw-r--r--   0        0        0        0 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/test_data/server_conformance_test_truss/model/__init__.py
+-rw-r--r--   0        0        0      597 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/test_data/server_conformance_test_truss/model/model.py
+-rw-r--r--   0        0        0      669 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/test_data/test_truss/config.yaml
+-rw-r--r--   0        0        0       48 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/test_data/test_truss/examples.yaml
+-rw-r--r--   0        0        0        0 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/test_data/test_truss/model/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/test_data/test_truss/model/dummy
+-rw-r--r--   0        0        0      534 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/test_data/test_truss/model/model.py
+-rw-r--r--   0        0        0        0 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/tests/__init__.py
+-rw-r--r--   0        0        0    20811 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/tests/conftest.py
+-rw-r--r--   0        0        0     1255 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/tests/contexts/image_builder/test_serving_image_builder.py
+-rw-r--r--   0        0        0      783 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/tests/contexts/local_loader/test_load_local.py
+-rw-r--r--   0        0        0     5337 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/tests/contexts/local_loader/test_truss_module_finder.py
+-rw-r--r--   0        0        0      968 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/tests/environments_inference/test_requirements_inference.py
+-rw-r--r--   0        0        0        0 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/tests/local/__init__.py
+-rw-r--r--   0        0        0     2245 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/tests/local/test_local_config_handler.py
+-rw-r--r--   0        0        0        0 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/tests/model_frameworks/__init__.py
+-rw-r--r--   0        0        0     3293 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/tests/model_frameworks/test_huggingface_transformer_framework.py
+-rw-r--r--   0        0        0     2789 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/tests/model_frameworks/test_keras_framework.py
+-rw-r--r--   0        0        0     2409 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/tests/model_frameworks/test_lightgbm_framework.py
+-rw-r--r--   0        0        0     1479 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/tests/model_frameworks/test_pytorch_framework.py
+-rw-r--r--   0        0        0     2427 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/tests/model_frameworks/test_sklearn_framework.py
+-rw-r--r--   0        0        0     2437 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/tests/model_frameworks/test_xgboost_framework.py
+-rw-r--r--   0        0        0    11109 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/tests/patch/test_calc_patch.py
+-rw-r--r--   0        0        0      487 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/tests/patch/test_dir_signature.py
+-rw-r--r--   0        0        0     5983 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/tests/patch/test_hash.py
+-rw-r--r--   0        0        0      394 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/tests/patch/test_signature.py
+-rw-r--r--   0        0        0      273 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/tests/patch/test_types.py
+-rw-r--r--   0        0        0    10415 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/tests/samples.py
+-rw-r--r--   0        0        0      283 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/tests/templates/control/control/helpers/test_context_managers.py
+-rw-r--r--   0        0        0     1976 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/tests/templates/control/control/helpers/test_patch_applier.py
+-rw-r--r--   0        0        0     6931 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/tests/templates/control/control/test_server.py
+-rw-r--r--   0        0        0      750 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/tests/templates/core/server/common/test_util.py
+-rw-r--r--   0        0        0     1539 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/tests/templates/core/server/test_secrets_resolver.py
+-rw-r--r--   0        0        0     2038 2023-06-07 18:37:55.797276 truss-0.4.8rc7/truss/tests/templates/server/common/test_retry.py
+-rw-r--r--   0        0        0     2252 2023-06-07 18:37:55.801276 truss-0.4.8rc7/truss/tests/templates/server/test_model_wrapper.py
+-rw-r--r--   0        0        0     1910 2023-06-07 18:37:55.801276 truss-0.4.8rc7/truss/tests/test_backward.py
+-rw-r--r--   0        0        0     8260 2023-06-07 18:37:55.801276 truss-0.4.8rc7/truss/tests/test_build.py
+-rw-r--r--   0        0        0     3181 2023-06-07 18:37:55.801276 truss-0.4.8rc7/truss/tests/test_config.py
+-rw-r--r--   0        0        0     1188 2023-06-07 18:37:55.801276 truss-0.4.8rc7/truss/tests/test_context_builder_image.py
+-rw-r--r--   0        0        0      517 2023-06-07 18:37:55.801276 truss-0.4.8rc7/truss/tests/test_docker.py
+-rw-r--r--   0        0        0     4905 2023-06-07 18:37:55.801276 truss-0.4.8rc7/truss/tests/test_model_inference.py
+-rw-r--r--   0        0        0      656 2023-06-07 18:37:55.801276 truss-0.4.8rc7/truss/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1483 2023-06-07 18:37:55.801276 truss-0.4.8rc7/truss/tests/test_testing_utilities_for_other_tests.py
+-rw-r--r--   0        0        0     1252 2023-06-07 18:37:55.801276 truss-0.4.8rc7/truss/tests/test_truss_gatherer.py
+-rw-r--r--   0        0        0    33902 2023-06-07 18:37:55.801276 truss-0.4.8rc7/truss/tests/test_truss_handle.py
+-rw-r--r--   0        0        0      434 2023-06-07 18:37:55.801276 truss-0.4.8rc7/truss/tests/test_truss_util.py
+-rw-r--r--   0        0        0     1865 2023-06-07 18:37:55.801276 truss-0.4.8rc7/truss/tests/test_validation.py
+-rw-r--r--   0        0        0    13164 2023-06-07 18:37:55.801276 truss-0.4.8rc7/truss/truss_config.py
+-rw-r--r--   0        0        0     2845 2023-06-07 18:37:55.801276 truss-0.4.8rc7/truss/truss_gatherer.py
+-rw-r--r--   0        0        0    40919 2023-06-07 18:37:55.801276 truss-0.4.8rc7/truss/truss_handle.py
+-rw-r--r--   0        0        0     5671 2023-06-07 18:37:55.801276 truss-0.4.8rc7/truss/truss_spec.py
+-rw-r--r--   0        0        0     2124 2023-06-07 18:37:55.801276 truss-0.4.8rc7/truss/types.py
+-rw-r--r--   0        0        0      227 2023-06-07 18:37:55.801276 truss-0.4.8rc7/truss/util/data_structures.py
+-rw-r--r--   0        0        0      553 2023-06-07 18:37:55.801276 truss-0.4.8rc7/truss/util/gpu.py
+-rw-r--r--   0        0        0      333 2023-06-07 18:37:55.801276 truss-0.4.8rc7/truss/util/jinja.py
+-rw-r--r--   0        0        0     2018 2023-06-07 18:37:55.801276 truss-0.4.8rc7/truss/util/path.py
+-rw-r--r--   0        0        0     2736 2023-06-07 18:37:55.801276 truss-0.4.8rc7/truss/validation.py
+-rw-r--r--   0        0        0     7595 1970-01-01 00:00:00.000000 truss-0.4.8rc7/PKG-INFO
```

### Comparing `truss-0.4.8rc5/CODE_OF_CONDUCT.md` & `truss-0.4.8rc7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/CONTRIBUTING.md` & `truss-0.4.8rc7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/LICENSE` & `truss-0.4.8rc7/LICENSE`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/README.md` & `truss-0.4.8rc7/README.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/ROADMAP.md` & `truss-0.4.8rc7/ROADMAP.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/context_builder.Dockerfile` & `truss-0.4.8rc7/context_builder.Dockerfile`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/pyproject.toml` & `truss-0.4.8rc7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "truss"
-version = "0.4.8rc5"
+version = "0.4.8rc7"
 description = "A seamless bridge from model development to model delivery"
 license = "MIT"
 readme = "README.md"
 authors = ["Pankaj Gupta <pankaj@baseten.co>", "Phil Howes <phil@baseten.co>"]
 include = ["*.txt", "*.Dockerfile", "*.md"]
 repository = "https://github.com/basetenlabs/truss"
 keywords = ["MLOps", "AI", "Model Serving", "Model Deployment", "Machine Learning"]
```

### Comparing `truss-0.4.8rc5/truss/blob/blob_backend_registry.py` & `truss-0.4.8rc7/truss/blob/blob_backend_registry.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/blob/http_public_blob_backend.py` & `truss-0.4.8rc7/truss/blob/http_public_blob_backend.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/build.py` & `truss-0.4.8rc7/truss/build.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/cli.py` & `truss-0.4.8rc7/truss/cli.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/constants.py` & `truss-0.4.8rc7/truss/constants.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/contexts/image_builder/image_builder.py` & `truss-0.4.8rc7/truss/contexts/image_builder/image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/contexts/image_builder/serving_image_builder.py` & `truss-0.4.8rc7/truss/contexts/image_builder/serving_image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/contexts/image_builder/training_image_builder.py` & `truss-0.4.8rc7/truss/contexts/image_builder/training_image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/contexts/image_builder/util.py` & `truss-0.4.8rc7/truss/contexts/image_builder/util.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/contexts/local_loader/docker_build_emulator.py` & `truss-0.4.8rc7/truss/contexts/local_loader/docker_build_emulator.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,14 +40,16 @@
             return key
 
         def _resolve_values(keys: List[str]) -> List[str]:
             return list(map(_resolve_env, keys))
 
         result = DockerBuildEmulatorResult()
         for cmd in self._commands:
+            if cmd.cmd not in ["ENV", "ENTRYPOINT", "COPY", "WORKDIR"]:
+                continue
             values = _resolve_values(cmd.value)
             if cmd.cmd == "ENV":
                 result.env[values[0]] = values[1]
             if cmd.cmd == "ENTRYPOINT":
                 result.entrypoint = list(values)
             if cmd.cmd == "COPY":
                 src, dst = values
```

### Comparing `truss-0.4.8rc5/truss/contexts/local_loader/load_model_local.py` & `truss-0.4.8rc7/truss/contexts/local_loader/load_model_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/contexts/local_loader/train_local.py` & `truss-0.4.8rc7/truss/contexts/local_loader/train_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/contexts/local_loader/truss_module_loader.py` & `truss-0.4.8rc7/truss/contexts/local_loader/truss_module_loader.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/contexts/local_loader/utils.py` & `truss-0.4.8rc7/truss/contexts/local_loader/utils.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/docker.py` & `truss-0.4.8rc7/truss/docker.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/environment_inference/requirements_inference.py` & `truss-0.4.8rc7/truss/environment_inference/requirements_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/errors.py` & `truss-0.4.8rc7/truss/errors.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/local/local_config.py` & `truss-0.4.8rc7/truss/local/local_config.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/local/local_config_handler.py` & `truss-0.4.8rc7/truss/local/local_config_handler.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/model_framework.py` & `truss-0.4.8rc7/truss/model_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/model_frameworks/__init__.py` & `truss-0.4.8rc7/truss/model_frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/model_frameworks/huggingface_transformer.py` & `truss-0.4.8rc7/truss/model_frameworks/huggingface_transformer.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/model_frameworks/keras.py` & `truss-0.4.8rc7/truss/model_frameworks/keras.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/model_frameworks/lightgbm.py` & `truss-0.4.8rc7/truss/model_frameworks/lightgbm.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/model_frameworks/mlflow.py` & `truss-0.4.8rc7/truss/model_frameworks/mlflow.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/model_frameworks/pytorch.py` & `truss-0.4.8rc7/truss/model_frameworks/pytorch.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/model_frameworks/sklearn.py` & `truss-0.4.8rc7/truss/model_frameworks/sklearn.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/model_frameworks/xgboost.py` & `truss-0.4.8rc7/truss/model_frameworks/xgboost.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/model_inference.py` & `truss-0.4.8rc7/truss/model_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/patch/calc_patch.py` & `truss-0.4.8rc7/truss/patch/calc_patch.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/patch/dir_signature.py` & `truss-0.4.8rc7/truss/patch/dir_signature.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/patch/hash.py` & `truss-0.4.8rc7/truss/patch/hash.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/patch/types.py` & `truss-0.4.8rc7/truss/patch/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/readme_generator.py` & `truss-0.4.8rc7/truss/readme_generator.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/templates/README.md.jinja` & `truss-0.4.8rc7/truss/templates/README.md.jinja`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/templates/base.Dockerfile.jinja` & `truss-0.4.8rc7/truss/templates/base.Dockerfile.jinja`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 ARG PYVERSION={{config.python_version}}
 FROM {{base_image_name_and_tag}}
 
 ENV PYTHON_EXECUTABLE {{ config.base_image.python_executable_path or 'python3' }}
 
 {% block fail_fast %}
 RUN grep -w 'ID=debian\|ID_LIKE=debian' /etc/os-release || { echo "ERROR: Supplied base image is not a debian image"; exit 1; }
-RUN pythonVersion=$(echo $($PYTHON_EXECUTABLE --version) | cut -d" " -f2 | cut -d"." -f1,2) \
-    && $PYTHON_EXECUTABLE -c "import sys; sys.exit(0) if sys.version_info.major == 3 and sys.version_info.minor >=8 and sys.version_info.minor <=11 else sys.exit(1)" \
-    && apt-get update && ( apt-get install -y --no-install-recommends python$pythonVersion-venv || apt-get install -y --no-install-recommends python3-venv )  \
-    && apt-get autoremove -y \
-    && apt-get clean -y \
-    && rm -rf /var/lib/apt/lists/* \
+RUN $PYTHON_EXECUTABLE -c "import sys; sys.exit(0) if sys.version_info.major == 3 and sys.version_info.minor >=8 and sys.version_info.minor <=11 else sys.exit(1)" \
     || { echo "ERROR: Supplied base image does not have 3.8 <= python <= 3.11"; exit 1; }
 {% endblock %}
 
 RUN pip install --upgrade pip --no-cache-dir \
     && rm -rf /root/.cache/pip
 
 {% block base_image_patch %}
@@ -44,17 +39,14 @@
 {% block install_requirements %}
     {%- if should_install_requirements %}
 COPY ./requirements.txt requirements.txt
 RUN pip install -r requirements.txt --no-cache-dir && rm -rf /root/.cache/pip
     {%- endif %}
 {% endblock %}
 
-{% block b10cp %}
-{% endblock %}
-
 
 ENV APP_HOME /app
 WORKDIR $APP_HOME
 
 
 {% block app_copy %}
 {% endblock %}
```

### Comparing `truss-0.4.8rc5/truss/templates/control/control/application.py` & `truss-0.4.8rc7/truss/templates/control/control/application.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/templates/control/control/endpoints.py` & `truss-0.4.8rc7/truss/templates/control/control/endpoints.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/templates/control/control/helpers/errors.py` & `truss-0.4.8rc7/truss/templates/control/control/helpers/errors.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/templates/control/control/helpers/inference_server_controller.py` & `truss-0.4.8rc7/truss/templates/control/control/helpers/inference_server_controller.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/templates/control/control/helpers/inference_server_process_controller.py` & `truss-0.4.8rc7/truss/templates/control/control/helpers/inference_server_process_controller.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/templates/control/control/helpers/inference_server_starter.py` & `truss-0.4.8rc7/truss/templates/control/control/helpers/inference_server_starter.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/templates/control/control/helpers/patch_applier.py` & `truss-0.4.8rc7/truss/templates/control/control/helpers/patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/templates/control/control/helpers/types.py` & `truss-0.4.8rc7/truss/templates/control/control/helpers/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/templates/control/control/server.py` & `truss-0.4.8rc7/truss/templates/control/control/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,16 @@
             "inference_server_port": INFERENCE_SERVER_PORT,
         }
     )
 
     # Perform inference server startup flow in background
     Thread(target=inference_server_startup_flow, args=(application,)).start()
 
-    application.logger.info(f"Starting control server on port {CONTROL_SERVER_PORT}")
+    application.logger.info(
+        f"Starting live reload server on port {CONTROL_SERVER_PORT}"
+    )
     server: Union[BaseWSGIServer, MultiSocketServer] = create_server(
         application,
         host=application.config["control_server_host"],
         port=application.config["control_server_port"],
     )
     server.run()
```

### Comparing `truss-0.4.8rc5/truss/templates/custom/model/model.py` & `truss-0.4.8rc7/truss/templates/custom/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/templates/huggingface_transformer/model/model.py` & `truss-0.4.8rc7/truss/templates/huggingface_transformer/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/templates/keras/model/model.py` & `truss-0.4.8rc7/truss/templates/keras/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/templates/lightgbm/model/model.py` & `truss-0.4.8rc7/truss/templates/lightgbm/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/templates/mlflow/model/model.py` & `truss-0.4.8rc7/truss/templates/mlflow/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/templates/pytorch/model/model.py` & `truss-0.4.8rc7/truss/templates/pytorch/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/templates/server/common/errors.py` & `truss-0.4.8rc7/truss/templates/server/common/errors.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/templates/server/common/logging.py` & `truss-0.4.8rc7/truss/templates/server/common/logging.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/templates/server/common/patches/whisper/patch.py` & `truss-0.4.8rc7/truss/templates/server/common/patches/whisper/patch.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/templates/server/common/patches.py` & `truss-0.4.8rc7/truss/templates/server/common/patches.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/templates/server/common/retry.py` & `truss-0.4.8rc7/truss/templates/server/common/retry.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/templates/server/common/serialization.py` & `truss-0.4.8rc7/truss/templates/server/common/serialization.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/templates/server/common/truss_server.py` & `truss-0.4.8rc7/truss/templates/server/common/truss_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/templates/server/common/util.py` & `truss-0.4.8rc7/truss/templates/server/common/util.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/templates/server/inference_server.py` & `truss-0.4.8rc7/truss/templates/server/inference_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/templates/server/model_wrapper.py` & `truss-0.4.8rc7/truss/templates/server/model_wrapper.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/templates/server.Dockerfile.jinja` & `truss-0.4.8rc7/truss/templates/server.Dockerfile.jinja`

 * *Files 10% similar despite different names*

```diff
@@ -17,14 +17,21 @@
     && apt-get clean -y \
     && rm -rf /var/lib/apt/lists/*
 
 COPY ./base_server_requirements.txt base_server_requirements.txt
 RUN pip install -r base_server_requirements.txt --no-cache-dir && rm -rf /root/.cache/pip
 
     {%- if config.live_reload %}
+RUN $PYTHON_EXECUTABLE -m venv -h >/dev/null \
+    || { pythonVersion=$(echo $($PYTHON_EXECUTABLE --version) | cut -d" " -f2 | cut -d"." -f1,2) \
+    && add-apt-repository -y ppa:deadsnakes/ppa \
+    && apt update -y && apt install -y --no-install-recommends python$pythonVersion-venv \
+    && apt-get autoremove -y \
+    && apt-get clean -y \
+    && rm -rf /var/lib/apt/lists/*; }
 # Create symlink for control server to start inference server process with correct python executable
 RUN readlink {{config.base_image.python_executable_path}} &>/dev/null \
     && echo "WARNING: Overwriting existing link at /usr/local/bin/python"
 RUN ln -sf {{config.base_image.python_executable_path}} /usr/local/bin/python
     {%- endif %}
 {% endif %}
 
@@ -34,20 +41,14 @@
     {%- if should_install_server_requirements %}
 COPY ./server_requirements.txt server_requirements.txt
 RUN pip install -r server_requirements.txt --no-cache-dir && rm -rf /root/.cache/pip
     {%- endif %}
 {{ super() }}
 {% endblock %}
 
-{% block b10cp %}
-RUN mkdir -p /app/bin \
-    && curl https://baseten-public.s3.us-west-2.amazonaws.com/bin/b10cp-0.0.2-linux-amd64 -o /app/bin/b10cp \
-    && chmod +x /app/bin/b10cp
-{% endblock %}
-
 {% block app_copy %}
 # Copy data before code for better caching
 {%- if data_dir_exists %}
 COPY ./{{config.data_dir}} /app/data
 {%- endif %}
 
 COPY ./server /app
```

### Comparing `truss-0.4.8rc5/truss/templates/shared/secrets_resolver.py` & `truss-0.4.8rc7/truss/templates/shared/secrets_resolver.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/templates/sklearn/model/model.py` & `truss-0.4.8rc7/truss/templates/sklearn/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/templates/training/job.py` & `truss-0.4.8rc7/truss/templates/training/job.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/templates/xgboost/model/model.py` & `truss-0.4.8rc7/truss/templates/xgboost/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/test_data/auto-mpg.data` & `truss-0.4.8rc7/truss/test_data/auto-mpg.data`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/test_data/happy.ipynb` & `truss-0.4.8rc7/truss/test_data/happy.ipynb`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/test_data/patch_ping_test_server/app.py` & `truss-0.4.8rc7/truss/test_data/patch_ping_test_server/app.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/test_data/pima-indians-diabetes.csv` & `truss-0.4.8rc7/truss/test_data/pima-indians-diabetes.csv`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/test_data/readme_int_example.md` & `truss-0.4.8rc7/truss/test_data/readme_int_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/test_data/readme_no_example.md` & `truss-0.4.8rc7/truss/test_data/readme_no_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/test_data/readme_str_example.md` & `truss-0.4.8rc7/truss/test_data/readme_str_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/test_data/server_conformance_test_truss/config.yaml` & `truss-0.4.8rc7/truss/test_data/server_conformance_test_truss/config.yaml`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/test_data/server_conformance_test_truss/model/model.py` & `truss-0.4.8rc7/truss/test_data/server_conformance_test_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/test_data/test_truss/config.yaml` & `truss-0.4.8rc7/truss/test_data/test_truss/config.yaml`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/test_data/test_truss/model/model.py` & `truss-0.4.8rc7/truss/test_data/test_truss/model/model.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/tests/conftest.py` & `truss-0.4.8rc7/truss/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/tests/contexts/image_builder/test_serving_image_builder.py` & `truss-0.4.8rc7/truss/tests/contexts/image_builder/test_serving_image_builder.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/tests/contexts/local_loader/test_load_local.py` & `truss-0.4.8rc7/truss/tests/contexts/local_loader/test_load_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/tests/contexts/local_loader/test_truss_module_finder.py` & `truss-0.4.8rc7/truss/tests/contexts/local_loader/test_truss_module_finder.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/tests/environments_inference/test_requirements_inference.py` & `truss-0.4.8rc7/truss/tests/environments_inference/test_requirements_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/tests/local/test_local_config_handler.py` & `truss-0.4.8rc7/truss/tests/local/test_local_config_handler.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/tests/model_frameworks/test_huggingface_transformer_framework.py` & `truss-0.4.8rc7/truss/tests/model_frameworks/test_huggingface_transformer_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/tests/model_frameworks/test_keras_framework.py` & `truss-0.4.8rc7/truss/tests/model_frameworks/test_keras_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/tests/model_frameworks/test_lightgbm_framework.py` & `truss-0.4.8rc7/truss/tests/model_frameworks/test_lightgbm_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/tests/model_frameworks/test_pytorch_framework.py` & `truss-0.4.8rc7/truss/tests/model_frameworks/test_pytorch_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/tests/model_frameworks/test_sklearn_framework.py` & `truss-0.4.8rc7/truss/tests/model_frameworks/test_sklearn_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/tests/model_frameworks/test_xgboost_framework.py` & `truss-0.4.8rc7/truss/tests/model_frameworks/test_xgboost_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/tests/patch/test_calc_patch.py` & `truss-0.4.8rc7/truss/tests/patch/test_calc_patch.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/tests/patch/test_hash.py` & `truss-0.4.8rc7/truss/tests/patch/test_hash.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/tests/samples.py` & `truss-0.4.8rc7/truss/tests/samples.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/tests/templates/control/control/helpers/test_patch_applier.py` & `truss-0.4.8rc7/truss/tests/templates/control/control/helpers/test_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/tests/templates/control/control/test_server.py` & `truss-0.4.8rc7/truss/tests/templates/control/control/test_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/tests/templates/core/server/common/test_util.py` & `truss-0.4.8rc7/truss/tests/templates/core/server/common/test_util.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/tests/templates/core/server/test_secrets_resolver.py` & `truss-0.4.8rc7/truss/tests/templates/core/server/test_secrets_resolver.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/tests/templates/server/common/test_retry.py` & `truss-0.4.8rc7/truss/tests/templates/server/common/test_retry.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/tests/templates/server/test_model_wrapper.py` & `truss-0.4.8rc7/truss/tests/templates/server/test_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/tests/test_backward.py` & `truss-0.4.8rc7/truss/tests/test_backward.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/tests/test_build.py` & `truss-0.4.8rc7/truss/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/tests/test_config.py` & `truss-0.4.8rc7/truss/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/tests/test_context_builder_image.py` & `truss-0.4.8rc7/truss/tests/test_context_builder_image.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/tests/test_docker.py` & `truss-0.4.8rc7/truss/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/tests/test_model_inference.py` & `truss-0.4.8rc7/truss/tests/test_model_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/tests/test_notebooks.py` & `truss-0.4.8rc7/truss/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/tests/test_testing_utilities_for_other_tests.py` & `truss-0.4.8rc7/truss/tests/test_testing_utilities_for_other_tests.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/tests/test_truss_gatherer.py` & `truss-0.4.8rc7/truss/tests/test_truss_gatherer.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/tests/test_truss_handle.py` & `truss-0.4.8rc7/truss/tests/test_truss_handle.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     assert image.repo_tags[0] == tag
 
 
 @pytest.mark.integration
 @pytest.mark.parametrize(
     "base_image, path, expected_fail",
     [
-        ("baseten/truss-server-base:3.9-v0.4.3", "/usr/local/bin/python3", False),
+        ("baseten/truss-server-base:3.9-v0.4.8rc4", "/usr/local/bin/python3", False),
         ("python:3.8", "/usr/local/bin/python3", False),
         ("python:3.11", "/usr/local/bin/python3", False),
         ("python:alpine", "/usr/local/bin/python3", True),
         ("python:2.7-slim", "/usr/local/bin/python", True),
         ("python:3.7-slim", "/usr/local/bin/python3", True),
     ],
 )
```

### Comparing `truss-0.4.8rc5/truss/tests/test_validation.py` & `truss-0.4.8rc7/truss/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/truss_config.py` & `truss-0.4.8rc7/truss/truss_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
 
 @dataclass
 class Resources:
     cpu: str = DEFAULT_CPU
     memory: str = DEFAULT_MEMORY
     use_gpu: bool = DEFAULT_USE_GPU
-    accelerator: AcceleratorSpec = AcceleratorSpec()
+    accelerator: AcceleratorSpec = field(default_factory=AcceleratorSpec)
 
     @staticmethod
     def from_dict(d):
         cpu = d.get("cpu", DEFAULT_CPU)
         validate_cpu_spec(cpu)
         memory = d.get("memory", DEFAULT_MEMORY)
         validate_memory_spec(memory)
```

### Comparing `truss-0.4.8rc5/truss/truss_gatherer.py` & `truss-0.4.8rc7/truss/truss_gatherer.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/truss_handle.py` & `truss-0.4.8rc7/truss/truss_handle.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/truss_spec.py` & `truss-0.4.8rc7/truss/truss_spec.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/types.py` & `truss-0.4.8rc7/truss/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/util/gpu.py` & `truss-0.4.8rc7/truss/util/gpu.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/util/path.py` & `truss-0.4.8rc7/truss/util/path.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/truss/validation.py` & `truss-0.4.8rc7/truss/validation.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.8rc5/PKG-INFO` & `truss-0.4.8rc7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: truss
-Version: 0.4.8rc5
+Version: 0.4.8rc7
 Summary: A seamless bridge from model development to model delivery
 Home-page: https://github.com/basetenlabs/truss
 License: MIT
 Keywords: MLOps,AI,Model Serving,Model Deployment,Machine Learning
 Author: Pankaj Gupta
 Author-email: pankaj@baseten.co
 Requires-Python: >=3.8,<3.12
```

