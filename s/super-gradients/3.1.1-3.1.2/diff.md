# Comparing `tmp/super_gradients-3.1.1-py3-none-any.whl.zip` & `tmp/super_gradients-3.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,559 +1,569 @@
-Zip file size: 964207 bytes, number of entries: 557
--rw-r--r--  2.0 unx      711 b- defN 23-May-03 19:50 super_gradients/__init__.py
--rw-r--r--  2.0 unx     1657 b- defN 23-May-03 19:50 super_gradients/evaluate_checkpoint.py
--rw-r--r--  2.0 unx     1807 b- defN 23-May-03 19:50 super_gradients/evaluate_from_recipe.py
--rw-r--r--  2.0 unx      702 b- defN 23-May-03 19:50 super_gradients/qat_from_recipe.py
--rwxr-xr-x  2.0 unx       44 b- defN 23-May-03 19:50 super_gradients/requirements.pro.txt
--rwxr-xr-x  2.0 unx      729 b- defN 23-May-03 19:50 super_gradients/requirements.txt
--rw-r--r--  2.0 unx      537 b- defN 23-May-03 19:50 super_gradients/resume_experiment.py
--rw-r--r--  2.0 unx      693 b- defN 23-May-03 19:50 super_gradients/train_from_kd_recipe.py
--rw-r--r--  2.0 unx      650 b- defN 23-May-03 19:50 super_gradients/train_from_recipe.py
--rw-r--r--  2.0 unx     1098 b- defN 23-May-03 19:50 super_gradients/common/__init__.py
--rw-r--r--  2.0 unx    15339 b- defN 23-May-03 19:50 super_gradients/common/object_names.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/common/abstractions/__init__.py
--rw-r--r--  2.0 unx      879 b- defN 23-May-03 19:50 super_gradients/common/abstractions/abstract_logger.py
--rw-r--r--  2.0 unx     3129 b- defN 23-May-03 19:50 super_gradients/common/abstractions/mute_processes.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/common/auto_logging/__init__.py
--rw-r--r--  2.0 unx     4846 b- defN 23-May-03 19:50 super_gradients/common/auto_logging/auto_logger.py
--rw-r--r--  2.0 unx     6625 b- defN 23-May-03 19:50 super_gradients/common/auto_logging/console_logging.py
--rw-r--r--  2.0 unx      142 b- defN 23-May-03 19:50 super_gradients/common/aws_connection/__init__.py
--rw-r--r--  2.0 unx     4182 b- defN 23-May-03 19:50 super_gradients/common/aws_connection/aws_connector.py
--rw-r--r--  2.0 unx     7198 b- defN 23-May-03 19:50 super_gradients/common/aws_connection/aws_secrets_manager_connector.py
--rw-r--r--  2.0 unx      119 b- defN 23-May-03 19:50 super_gradients/common/crash_handler/__init__.py
--rw-r--r--  2.0 unx      669 b- defN 23-May-03 19:50 super_gradients/common/crash_handler/crash_handler.py
--rw-r--r--  2.0 unx    11775 b- defN 23-May-03 19:50 super_gradients/common/crash_handler/crash_tips.py
--rw-r--r--  2.0 unx      886 b- defN 23-May-03 19:50 super_gradients/common/crash_handler/crash_tips_setup.py
--rw-r--r--  2.0 unx     1740 b- defN 23-May-03 19:50 super_gradients/common/crash_handler/exception.py
--rw-r--r--  2.0 unx     2357 b- defN 23-May-03 19:50 super_gradients/common/crash_handler/exception_monitoring_setup.py
--rw-r--r--  2.0 unx      789 b- defN 23-May-03 19:50 super_gradients/common/crash_handler/utils.py
--rw-r--r--  2.0 unx      140 b- defN 23-May-03 19:50 super_gradients/common/data_connection/__init__.py
--rw-r--r--  2.0 unx    17959 b- defN 23-May-03 19:50 super_gradients/common/data_connection/s3_connector.py
--rw-r--r--  2.0 unx      325 b- defN 23-May-03 19:50 super_gradients/common/data_interface/__init__.py
--rw-r--r--  2.0 unx     9699 b- defN 23-May-03 19:50 super_gradients/common/data_interface/adnn_model_repository_data_interface.py
--rw-r--r--  2.0 unx     2050 b- defN 23-May-03 19:50 super_gradients/common/data_interface/dataset_data_interface.py
--rw-r--r--  2.0 unx      220 b- defN 23-May-03 19:50 super_gradients/common/data_types/__init__.py
--rw-r--r--  2.0 unx      597 b- defN 23-May-03 19:50 super_gradients/common/data_types/enum/__init__.py
--rw-r--r--  2.0 unx      309 b- defN 23-May-03 19:50 super_gradients/common/data_types/enum/deep_learning_task.py
--rw-r--r--  2.0 unx      108 b- defN 23-May-03 19:50 super_gradients/common/data_types/enum/downsample_mode.py
--rw-r--r--  2.0 unx      317 b- defN 23-May-03 19:50 super_gradients/common/data_types/enum/evaluation_type.py
--rw-r--r--  2.0 unx     1025 b- defN 23-May-03 19:50 super_gradients/common/data_types/enum/multi_gpu_mode.py
--rw-r--r--  2.0 unx     1200 b- defN 23-May-03 19:50 super_gradients/common/data_types/enum/strict_load.py
--rw-r--r--  2.0 unx      202 b- defN 23-May-03 19:50 super_gradients/common/data_types/enum/upsample_mode.py
--rw-r--r--  2.0 unx      257 b- defN 23-May-03 19:50 super_gradients/common/decorators/__init__.py
--rw-r--r--  2.0 unx     1567 b- defN 23-May-03 19:50 super_gradients/common/decorators/code_save_decorator.py
--rw-r--r--  2.0 unx     3663 b- defN 23-May-03 19:50 super_gradients/common/decorators/deci_logger.py
--rw-r--r--  2.0 unx     2921 b- defN 23-May-03 19:50 super_gradients/common/decorators/explicit_params_validator.py
--rw-r--r--  2.0 unx     1315 b- defN 23-May-03 19:50 super_gradients/common/decorators/factory_decorator.py
--rw-r--r--  2.0 unx     1132 b- defN 23-May-03 19:50 super_gradients/common/decorators/singleton.py
--rw-r--r--  2.0 unx      202 b- defN 23-May-03 19:50 super_gradients/common/environment/__init__.py
--rw-r--r--  2.0 unx      993 b- defN 23-May-03 19:50 super_gradients/common/environment/argparse_utils.py
--rw-r--r--  2.0 unx     9170 b- defN 23-May-03 19:50 super_gradients/common/environment/cfg_utils.py
--rw-r--r--  2.0 unx     4218 b- defN 23-May-03 19:50 super_gradients/common/environment/checkpoints_dir_utils.py
--rw-r--r--  2.0 unx     2682 b- defN 23-May-03 19:50 super_gradients/common/environment/ddp_utils.py
--rw-r--r--  2.0 unx      752 b- defN 23-May-03 19:50 super_gradients/common/environment/device_utils.py
--rw-r--r--  2.0 unx     1147 b- defN 23-May-03 19:50 super_gradients/common/environment/env_variables.py
--rw-r--r--  2.0 unx     4047 b- defN 23-May-03 19:50 super_gradients/common/environment/omegaconf_utils.py
--rw-r--r--  2.0 unx      459 b- defN 23-May-03 19:50 super_gradients/common/environment/path_utils.py
--rw-r--r--  2.0 unx      112 b- defN 23-May-03 19:50 super_gradients/common/environment/monitoring/__init__.py
--rw-r--r--  2.0 unx      153 b- defN 23-May-03 19:50 super_gradients/common/environment/monitoring/cpu.py
--rw-r--r--  2.0 unx     2517 b- defN 23-May-03 19:50 super_gradients/common/environment/monitoring/data_models.py
--rw-r--r--  2.0 unx     1025 b- defN 23-May-03 19:50 super_gradients/common/environment/monitoring/disk.py
--rw-r--r--  2.0 unx     5427 b- defN 23-May-03 19:50 super_gradients/common/environment/monitoring/monitoring.py
--rw-r--r--  2.0 unx      948 b- defN 23-May-03 19:50 super_gradients/common/environment/monitoring/network.py
--rw-r--r--  2.0 unx      629 b- defN 23-May-03 19:50 super_gradients/common/environment/monitoring/utils.py
--rw-r--r--  2.0 unx      145 b- defN 23-May-03 19:50 super_gradients/common/environment/monitoring/virtual_memory.py
--rw-r--r--  2.0 unx      681 b- defN 23-May-03 19:50 super_gradients/common/environment/monitoring/gpu/__init__.py
--rw-r--r--  2.0 unx     2270 b- defN 23-May-03 19:50 super_gradients/common/environment/monitoring/gpu/gpu.py
--rw-r--r--  2.0 unx   121647 b- defN 23-May-03 19:50 super_gradients/common/environment/monitoring/gpu/pynvml.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/common/exceptions/__init__.py
--rw-r--r--  2.0 unx      926 b- defN 23-May-03 19:50 super_gradients/common/exceptions/factory_exceptions.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/common/factories/__init__.py
--rw-r--r--  2.0 unx     1715 b- defN 23-May-03 19:50 super_gradients/common/factories/activations_type_factory.py
--rw-r--r--  2.0 unx     2881 b- defN 23-May-03 19:50 super_gradients/common/factories/base_factory.py
--rw-r--r--  2.0 unx      258 b- defN 23-May-03 19:50 super_gradients/common/factories/bbox_format_factory.py
--rw-r--r--  2.0 unx      232 b- defN 23-May-03 19:50 super_gradients/common/factories/callbacks_factory.py
--rw-r--r--  2.0 unx      263 b- defN 23-May-03 19:50 super_gradients/common/factories/collate_functions_factory.py
--rw-r--r--  2.0 unx      292 b- defN 23-May-03 19:50 super_gradients/common/factories/context_modules_factory.py
--rw-r--r--  2.0 unx      321 b- defN 23-May-03 19:50 super_gradients/common/factories/data_formats_factory.py
--rw-r--r--  2.0 unx      237 b- defN 23-May-03 19:50 super_gradients/common/factories/datasets_factory.py
--rw-r--r--  2.0 unx     1014 b- defN 23-May-03 19:50 super_gradients/common/factories/detection_modules_factory.py
--rw-r--r--  2.0 unx      572 b- defN 23-May-03 19:50 super_gradients/common/factories/list_factory.py
--rw-r--r--  2.0 unx      223 b- defN 23-May-03 19:50 super_gradients/common/factories/losses_factory.py
--rw-r--r--  2.0 unx      226 b- defN 23-May-03 19:50 super_gradients/common/factories/metrics_factory.py
--rw-r--r--  2.0 unx      467 b- defN 23-May-03 19:50 super_gradients/common/factories/optimizers_type_factory.py
--rw-r--r--  2.0 unx      271 b- defN 23-May-03 19:50 super_gradients/common/factories/pre_launch_callbacks_factory.py
--rw-r--r--  2.0 unx      623 b- defN 23-May-03 19:50 super_gradients/common/factories/processing_factory.py
--rw-r--r--  2.0 unx      229 b- defN 23-May-03 19:50 super_gradients/common/factories/samplers_factory.py
--rw-r--r--  2.0 unx      263 b- defN 23-May-03 19:50 super_gradients/common/factories/target_generator_factory.py
--rw-r--r--  2.0 unx     1873 b- defN 23-May-03 19:50 super_gradients/common/factories/transforms_factory.py
--rw-r--r--  2.0 unx     2377 b- defN 23-May-03 19:50 super_gradients/common/factories/type_factory.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/common/plugins/__init__.py
--rw-r--r--  2.0 unx    10974 b- defN 23-May-03 19:50 super_gradients/common/plugins/deci_client.py
--rw-r--r--  2.0 unx      271 b- defN 23-May-03 19:50 super_gradients/common/registry/__init__.py
--rw-r--r--  2.0 unx     1231 b- defN 23-May-03 19:50 super_gradients/common/registry/albumentation.py
--rw-r--r--  2.0 unx     6006 b- defN 23-May-03 19:50 super_gradients/common/registry/registry.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/common/registry/registry_utils.py
--rw-r--r--  2.0 unx      508 b- defN 23-May-03 19:50 super_gradients/common/sg_loggers/__init__.py
--rw-r--r--  2.0 unx     7355 b- defN 23-May-03 19:50 super_gradients/common/sg_loggers/abstract_sg_logger.py
--rw-r--r--  2.0 unx    14980 b- defN 23-May-03 19:50 super_gradients/common/sg_loggers/base_sg_logger.py
--rw-r--r--  2.0 unx    10055 b- defN 23-May-03 19:50 super_gradients/common/sg_loggers/clearml_sg_logger.py
--rw-r--r--  2.0 unx    10103 b- defN 23-May-03 19:50 super_gradients/common/sg_loggers/dagshub_sg_logger.py
--rw-r--r--  2.0 unx     6618 b- defN 23-May-03 19:50 super_gradients/common/sg_loggers/deci_platform_sg_logger.py
--rw-r--r--  2.0 unx    13073 b- defN 23-May-03 19:50 super_gradients/common/sg_loggers/wandb_sg_logger.py
--rw-r--r--  2.0 unx    85509 b- defN 23-May-03 19:50 super_gradients/examples/SG_Walkthrough.ipynb
--rw-r--r--  2.0 unx    69618 b- defN 23-May-03 19:50 super_gradients/examples/SG_quickstart_classification.ipynb
--rw-r--r--  2.0 unx    54966 b- defN 23-May-03 19:50 super_gradients/examples/SG_quickstart_model_upload_deci_lab.ipynb
--rw-r--r--  2.0 unx    65090 b- defN 23-May-03 19:50 super_gradients/examples/SG_quickstart_tensorboard_logger.ipynb
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/examples/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/examples/cifar10_training_torch_objects/__init__.py
--rw-r--r--  2.0 unx     2526 b- defN 23-May-03 19:50 super_gradients/examples/cifar10_training_torch_objects/cifar10_training_torch_objects_example.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/examples/convert_recipe_example/__init__.py
--rw-r--r--  2.0 unx      870 b- defN 23-May-03 19:50 super_gradients/examples/convert_recipe_example/convert_recipe_example.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/examples/ddrnet_imagenet/__init__.py
--rw-r--r--  2.0 unx     3114 b- defN 23-May-03 19:50 super_gradients/examples/ddrnet_imagenet/ddrnet_classification_example.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/examples/deci_lab_export_example/__init__.py
--rw-r--r--  2.0 unx     3562 b- defN 23-May-03 19:50 super_gradients/examples/deci_lab_export_example/deci_lab_export_example.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/examples/early_stop/__init__.py
--rw-r--r--  2.0 unx     1596 b- defN 23-May-03 19:50 super_gradients/examples/early_stop/early_stop_example.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/examples/evaluate_checkpoint_example/__init__.py
--rw-r--r--  2.0 unx      289 b- defN 23-May-03 19:50 super_gradients/examples/evaluate_checkpoint_example/evaluate_checkpoint.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/examples/evaluate_from_recipe_example/__init__.py
--rw-r--r--  2.0 unx      292 b- defN 23-May-03 19:50 super_gradients/examples/evaluate_from_recipe_example/evaluate_from_recipe.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/examples/loggers_examples/__init__.py
--rw-r--r--  2.0 unx     1206 b- defN 23-May-03 19:50 super_gradients/examples/loggers_examples/clearml_logger_example.py
--rw-r--r--  2.0 unx     1088 b- defN 23-May-03 19:50 super_gradients/examples/loggers_examples/deci_platform_logger_example.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/examples/qat_from_recipe_example/__init__.py
--rw-r--r--  2.0 unx      277 b- defN 23-May-03 19:50 super_gradients/examples/qat_from_recipe_example/qat_from_recipe.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/examples/quantization/__init__.py
--rw-r--r--  2.0 unx     1104 b- defN 23-May-03 19:50 super_gradients/examples/quantization/non_default_calibrators_example.py
--rw-r--r--  2.0 unx     2310 b- defN 23-May-03 19:50 super_gradients/examples/quantization/ptq_e2e_example.py
--rw-r--r--  2.0 unx     1850 b- defN 23-May-03 19:50 super_gradients/examples/quantization/register_quantization_mapping_with_decorator_example.py
--rw-r--r--  2.0 unx     4732 b- defN 23-May-03 19:50 super_gradients/examples/quantization/resnet_qat_example.py
--rw-r--r--  2.0 unx     1163 b- defN 23-May-03 19:50 super_gradients/examples/quantization/skipping_quantization_example.py
--rw-r--r--  2.0 unx      832 b- defN 23-May-03 19:50 super_gradients/examples/quantization/vanilla_quantize_all_example.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/examples/regseg_transfer_learning_example/__init__.py
--rw-r--r--  2.0 unx     2379 b- defN 23-May-03 19:50 super_gradients/examples/regseg_transfer_learning_example/regseg_transfer_learning_example.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/examples/resume_experiment_example/__init__.py
--rw-r--r--  2.0 unx      283 b- defN 23-May-03 19:50 super_gradients/examples/resume_experiment_example/resume_experiment.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/examples/train_from_kd_recipe_example/__init__.py
--rw-r--r--  2.0 unx      292 b- defN 23-May-03 19:50 super_gradients/examples/train_from_kd_recipe_example/train_from_kd_recipe.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/examples/train_from_recipe_example/__init__.py
--rw-r--r--  2.0 unx      283 b- defN 23-May-03 19:50 super_gradients/examples/train_from_recipe_example/train_from_recipe.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/examples/train_from_recipe_with_dataset_registry/__init__.py
--rw-r--r--  2.0 unx     1334 b- defN 23-May-03 19:50 super_gradients/examples/train_from_recipe_with_dataset_registry/train.py
--rw-r--r--  2.0 unx     1643 b- defN 23-May-03 19:50 super_gradients/examples/train_from_recipe_with_dataset_registry/user_dataset.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/examples/train_from_recipe_with_user_objects/__init__.py
--rw-r--r--  2.0 unx     1326 b- defN 23-May-03 19:50 super_gradients/examples/train_from_recipe_with_user_objects/train.py
--rw-r--r--  2.0 unx     2548 b- defN 23-May-03 19:50 super_gradients/examples/train_from_recipe_with_user_objects/user_dataset.py
--rw-r--r--  2.0 unx      174 b- defN 23-May-03 19:50 super_gradients/module_interfaces/__init__.py
--rw-r--r--  2.0 unx     2043 b- defN 23-May-03 19:50 super_gradients/module_interfaces/module_interfaces.py
--rw-r--r--  2.0 unx     3366 b- defN 23-May-03 19:50 super_gradients/modules/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/modules/all_detection_modules.py
--rw-r--r--  2.0 unx      617 b- defN 23-May-03 19:50 super_gradients/modules/anti_alias.py
--rw-r--r--  2.0 unx      776 b- defN 23-May-03 19:50 super_gradients/modules/base_modules.py
--rw-r--r--  2.0 unx     3054 b- defN 23-May-03 19:50 super_gradients/modules/conv_bn_act_block.py
--rw-r--r--  2.0 unx     1976 b- defN 23-May-03 19:50 super_gradients/modules/conv_bn_relu_block.py
--rw-r--r--  2.0 unx    14805 b- defN 23-May-03 19:50 super_gradients/modules/detection_modules.py
--rw-r--r--  2.0 unx     2143 b- defN 23-May-03 19:50 super_gradients/modules/head_replacement_utils.py
--rw-r--r--  2.0 unx     4362 b- defN 23-May-03 19:50 super_gradients/modules/multi_output_modules.py
--rw-r--r--  2.0 unx      860 b- defN 23-May-03 19:50 super_gradients/modules/pixel_shuffle.py
--rw-r--r--  2.0 unx     3953 b- defN 23-May-03 19:50 super_gradients/modules/pose_estimation_modules.py
--rw-r--r--  2.0 unx    11773 b- defN 23-May-03 19:50 super_gradients/modules/qarepvgg_block.py
--rw-r--r--  2.0 unx     8699 b- defN 23-May-03 19:50 super_gradients/modules/repvgg_block.py
--rw-r--r--  2.0 unx     2138 b- defN 23-May-03 19:50 super_gradients/modules/sampling.py
--rw-r--r--  2.0 unx     1459 b- defN 23-May-03 19:50 super_gradients/modules/se_blocks.py
--rw-r--r--  2.0 unx     1403 b- defN 23-May-03 19:50 super_gradients/modules/skip_connections.py
--rw-r--r--  2.0 unx     2968 b- defN 23-May-03 19:50 super_gradients/modules/utils.py
--rw-r--r--  2.0 unx      716 b- defN 23-May-03 19:50 super_gradients/modules/quantization/__init__.py
--rw-r--r--  2.0 unx     2649 b- defN 23-May-03 19:50 super_gradients/modules/quantization/quantized_skip_connections.py
--rw-r--r--  2.0 unx     4604 b- defN 23-May-03 19:50 super_gradients/modules/quantization/quantized_stdc_blocks.py
--rw-r--r--  2.0 unx     1281 b- defN 23-May-03 19:50 super_gradients/modules/quantization/resnet_bottleneck.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/recipes/__init__.py
--rw-r--r--  2.0 unx     1136 b- defN 23-May-03 19:50 super_gradients/recipes/cifar10_resnet.yaml
--rw-r--r--  2.0 unx     3502 b- defN 23-May-03 19:50 super_gradients/recipes/cityscapes_ddrnet.yaml
--rw-r--r--  2.0 unx     3754 b- defN 23-May-03 19:50 super_gradients/recipes/cityscapes_kd_base.yaml
--rw-r--r--  2.0 unx     3354 b- defN 23-May-03 19:50 super_gradients/recipes/cityscapes_pplite_seg50.yaml
--rw-r--r--  2.0 unx     3253 b- defN 23-May-03 19:50 super_gradients/recipes/cityscapes_pplite_seg75.yaml
--rw-r--r--  2.0 unx     2498 b- defN 23-May-03 19:50 super_gradients/recipes/cityscapes_regseg48.yaml
--rw-r--r--  2.0 unx     4020 b- defN 23-May-03 19:50 super_gradients/recipes/cityscapes_segformer.yaml
--rw-r--r--  2.0 unx      618 b- defN 23-May-03 19:50 super_gradients/recipes/cityscapes_stdc_base.yaml
--rw-r--r--  2.0 unx     2862 b- defN 23-May-03 19:50 super_gradients/recipes/cityscapes_stdc_seg50.yaml
--rw-r--r--  2.0 unx     3055 b- defN 23-May-03 19:50 super_gradients/recipes/cityscapes_stdc_seg75.yaml
--rw-r--r--  2.0 unx     1830 b- defN 23-May-03 19:50 super_gradients/recipes/coco2017_pose_ddrnet39.yaml
--rw-r--r--  2.0 unx     3549 b- defN 23-May-03 19:50 super_gradients/recipes/coco2017_pose_dekr_w32_no_dc.yaml
--rw-r--r--  2.0 unx     1998 b- defN 23-May-03 19:50 super_gradients/recipes/coco2017_pose_pppose_l.yaml
--rw-r--r--  2.0 unx     1996 b- defN 23-May-03 19:50 super_gradients/recipes/coco2017_ppyoloe_l.yaml
--rw-r--r--  2.0 unx     1996 b- defN 23-May-03 19:50 super_gradients/recipes/coco2017_ppyoloe_m.yaml
--rw-r--r--  2.0 unx     1882 b- defN 23-May-03 19:50 super_gradients/recipes/coco2017_ppyoloe_s.yaml
--rw-r--r--  2.0 unx     1975 b- defN 23-May-03 19:50 super_gradients/recipes/coco2017_ppyoloe_x.yaml
--rw-r--r--  2.0 unx     1889 b- defN 23-May-03 19:50 super_gradients/recipes/coco2017_ssd_lite_mobilenet_v2.yaml
--rw-r--r--  2.0 unx     1385 b- defN 23-May-03 19:50 super_gradients/recipes/coco2017_yolo_nas_s.yaml
--rw-r--r--  2.0 unx     2583 b- defN 23-May-03 19:50 super_gradients/recipes/coco2017_yolox.yaml
--rw-r--r--  2.0 unx     1376 b- defN 23-May-03 19:50 super_gradients/recipes/coco_segmentation_shelfnet_lw.yaml
--rw-r--r--  2.0 unx     1145 b- defN 23-May-03 19:50 super_gradients/recipes/imagenet_efficientnet.yaml
--rw-r--r--  2.0 unx     1129 b- defN 23-May-03 19:50 super_gradients/recipes/imagenet_mobilenetv2.yaml
--rw-r--r--  2.0 unx      507 b- defN 23-May-03 19:50 super_gradients/recipes/imagenet_mobilenetv3_base.yaml
--rw-r--r--  2.0 unx      719 b- defN 23-May-03 19:50 super_gradients/recipes/imagenet_mobilenetv3_large.yaml
--rw-r--r--  2.0 unx      719 b- defN 23-May-03 19:50 super_gradients/recipes/imagenet_mobilenetv3_small.yaml
--rw-r--r--  2.0 unx     1997 b- defN 23-May-03 19:50 super_gradients/recipes/imagenet_regnetY.yaml
--rw-r--r--  2.0 unx     1246 b- defN 23-May-03 19:50 super_gradients/recipes/imagenet_repvgg.yaml
--rw-r--r--  2.0 unx     1169 b- defN 23-May-03 19:50 super_gradients/recipes/imagenet_resnet50.yaml
--rw-r--r--  2.0 unx     2722 b- defN 23-May-03 19:50 super_gradients/recipes/imagenet_resnet50_kd.yaml
--rw-r--r--  2.0 unx     1136 b- defN 23-May-03 19:50 super_gradients/recipes/imagenet_vit_base.yaml
--rw-r--r--  2.0 unx     1010 b- defN 23-May-03 19:50 super_gradients/recipes/imagenet_vit_large.yaml
--rw-r--r--  2.0 unx     2007 b- defN 23-May-03 19:50 super_gradients/recipes/roboflow_ppyoloe.yaml
--rw-r--r--  2.0 unx     2347 b- defN 23-May-03 19:50 super_gradients/recipes/roboflow_yolo_nas_m.yaml
--rw-r--r--  2.0 unx     2347 b- defN 23-May-03 19:50 super_gradients/recipes/roboflow_yolo_nas_s.yaml
--rw-r--r--  2.0 unx      473 b- defN 23-May-03 19:50 super_gradients/recipes/roboflow_yolo_nas_s_qat.yaml
--rw-r--r--  2.0 unx     1915 b- defN 23-May-03 19:50 super_gradients/recipes/roboflow_yolox.yaml
--rw-r--r--  2.0 unx     1246 b- defN 23-May-03 19:50 super_gradients/recipes/supervisely_unet.yaml
--rw-r--r--  2.0 unx     1672 b- defN 23-May-03 19:50 super_gradients/recipes/user_recipe_mnist_as_external_dataset_example.yaml
--rw-r--r--  2.0 unx     2133 b- defN 23-May-03 19:50 super_gradients/recipes/user_recipe_mnist_example.yaml
--rw-r--r--  2.0 unx     2000 b- defN 23-May-03 19:50 super_gradients/recipes/variable_setup.yaml
--rw-r--r--  2.0 unx     2222 b- defN 23-May-03 19:50 super_gradients/recipes/anchors/ssd_anchors.yaml
--rw-r--r--  2.0 unx      563 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/efficientnet_arch_params.yaml
--rw-r--r--  2.0 unx      104 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/efficientnet_b0_arch_params.yaml
--rw-r--r--  2.0 unx      103 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/efficientnet_b1_arch_params.yaml
--rw-r--r--  2.0 unx      103 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/efficientnet_b2_arch_params.yaml
--rw-r--r--  2.0 unx      103 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/efficientnet_b3_arch_params.yaml
--rw-r--r--  2.0 unx      103 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/efficientnet_b4_arch_params.yaml
--rw-r--r--  2.0 unx      103 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/efficientnet_b5_arch_params.yaml
--rw-r--r--  2.0 unx      103 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/efficientnet_b6_arch_params.yaml
--rw-r--r--  2.0 unx      103 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/efficientnet_b7_arch_params.yaml
--rw-r--r--  2.0 unx      103 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/efficientnet_b8_arch_params.yaml
--rw-r--r--  2.0 unx      103 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/efficientnet_l2_arch_params.yaml
--rw-r--r--  2.0 unx      194 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/mobilenet_v2_arch_params.yaml
--rw-r--r--  2.0 unx      156 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/mobilenet_v3_arch_params.yaml
--rw-r--r--  2.0 unx      409 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/mobilenet_v3_large_arch_params.yaml
--rw-r--r--  2.0 unx      356 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/mobilenet_v3_small_arch_params.yaml
--rw-r--r--  2.0 unx      281 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/pose_ddrnet39_arch_params.yaml
--rw-r--r--  2.0 unx     1245 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/pose_dekr_w32_no_dc_arch_params.yaml
--rw-r--r--  2.0 unx      985 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/pose_pppose_l_arch_params.yaml
--rw-r--r--  2.0 unx     1112 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/ppyoloe_arch_params.yaml
--rw-r--r--  2.0 unx      196 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/ppyoloe_l_arch_params.yaml
--rw-r--r--  2.0 unx      198 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/ppyoloe_m_arch_params.yaml
--rw-r--r--  2.0 unx      198 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/ppyoloe_s_arch_params.yaml
--rw-r--r--  2.0 unx      198 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/ppyoloe_x_arch_params.yaml
--rw-r--r--  2.0 unx      204 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/regnetY_arch_params.yaml
--rw-r--r--  2.0 unx      352 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/repvgg_arch_params.yaml
--rw-r--r--  2.0 unx       98 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/repvgga0_arch_params.yaml
--rw-r--r--  2.0 unx       89 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/repvgga1_arch_params.yaml
--rw-r--r--  2.0 unx       95 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/repvgga2_arch_params.yaml
--rw-r--r--  2.0 unx       88 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/repvggb0_arch_params.yaml
--rw-r--r--  2.0 unx       86 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/repvggb1_arch_params.yaml
--rw-r--r--  2.0 unx       92 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/repvggb2_arch_params.yaml
--rw-r--r--  2.0 unx       15 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/resnet18_cifar_arch_params.yaml
--rw-r--r--  2.0 unx       17 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/resnet50_arch_params.yaml
--rw-r--r--  2.0 unx       32 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/shelfnet34_lw_arch_params.yaml
--rw-r--r--  2.0 unx      655 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/ssd_lite_mobilenetv2_arch_params.yaml
--rw-r--r--  2.0 unx      605 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/ssd_mobilenetv1_arch_params.yaml
--rw-r--r--  2.0 unx     1369 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/unet_arch_params.yaml
--rw-r--r--  2.0 unx     3031 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/unet_default_arch_params.yaml
--rw-r--r--  2.0 unx       63 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/vit_base_arch_params.yaml
--rw-r--r--  2.0 unx     2393 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/yolo_arch_params.yaml
--rw-r--r--  2.0 unx     2337 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/yolo_nas_l_arch_params.yaml
--rw-r--r--  2.0 unx     2346 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/yolo_nas_m_arch_params.yaml
--rw-r--r--  2.0 unx     2341 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/yolo_nas_s_arch_params.yaml
--rw-r--r--  2.0 unx      235 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/yolox_l_arch_params.yaml
--rw-r--r--  2.0 unx      237 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/yolox_m_arch_params.yaml
--rw-r--r--  2.0 unx      237 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/yolox_nano_arch_params.yaml
--rw-r--r--  2.0 unx      237 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/yolox_s_arch_params.yaml
--rw-r--r--  2.0 unx      229 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/yolox_tiny_arch_params.yaml
--rw-r--r--  2.0 unx      228 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/yolox_x_arch_params.yaml
--rw-r--r--  2.0 unx      611 b- defN 23-May-03 19:50 super_gradients/recipes/checkpoint_params/default_checkpoint_params.yaml
--rw-r--r--  2.0 unx       72 b- defN 23-May-03 19:50 super_gradients/recipes/checkpoint_params/vit_base_imagenet_checkpoint_params.yaml
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/recipes/conversion_params/__init__.py
--rw-r--r--  2.0 unx     1807 b- defN 23-May-03 19:50 super_gradients/recipes/conversion_params/cifar10_conversion_params.yaml
--rw-r--r--  2.0 unx     2040 b- defN 23-May-03 19:50 super_gradients/recipes/conversion_params/default_conversion_params.yaml
--rw-r--r--  2.0 unx      869 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/cifar100_dataset_params.yaml
--rw-r--r--  2.0 unx     1530 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/cifar10_albumentations_dataset_params.yaml
--rw-r--r--  2.0 unx     1056 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/cifar10_dataset_params.yaml
--rw-r--r--  2.0 unx      615 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/cityscapes_dataset_params.yaml
--rw-r--r--  2.0 unx      525 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/cityscapes_ddrnet_dataset_params.yaml
--rw-r--r--  2.0 unx      706 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/cityscapes_ppliteseg_seg75_dataset_params.yaml
--rw-r--r--  2.0 unx      644 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/cityscapes_regseg48_dataset_params.yaml
--rw-r--r--  2.0 unx      721 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/cityscapes_segformer_dataset_params.yaml
--rw-r--r--  2.0 unx      709 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/cityscapes_stdc_seg50_dataset_params.yaml
--rw-r--r--  2.0 unx      708 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/cityscapes_stdc_seg75_dataset_params.yaml
--rw-r--r--  2.0 unx     3946 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/coco_detection_dataset_params.yaml
--rw-r--r--  2.0 unx     4202 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/coco_detection_ppyoloe_dataset_params.yaml
--rw-r--r--  2.0 unx     3590 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/coco_detection_ssd_lite_mobilenet_v2_dataset_params.yaml
--rw-r--r--  2.0 unx     5568 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/coco_detection_yolo_format_base_dataset_params.yaml
--rw-r--r--  2.0 unx     3646 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/coco_detection_yolo_nas_dataset_params.yaml
--rw-r--r--  2.0 unx     2461 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/coco_pose_estimation_dataset_params.yaml
--rw-r--r--  2.0 unx      405 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/coco_pose_estimation_dekr_dataset_params.yaml
--rw-r--r--  2.0 unx     1466 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/coco_segmentation_dataset_params.yaml
--rw-r--r--  2.0 unx      931 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/imagenet_dataset_params.yaml
--rw-r--r--  2.0 unx      732 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/imagenet_efficientnet_dataset_params.yaml
--rw-r--r--  2.0 unx      794 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/imagenet_mobilenetv2_dataset_params.yaml
--rw-r--r--  2.0 unx      142 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/imagenet_mobilenetv3_dataset_params.yaml
--rw-r--r--  2.0 unx      734 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/imagenet_regnetY_dataset_params.yaml
--rw-r--r--  2.0 unx     1059 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/imagenet_resnet50_dataset_params.yaml
--rw-r--r--  2.0 unx     1093 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/imagenet_resnet50_kd_dataset_params.yaml
--rw-r--r--  2.0 unx      845 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/imagenet_vit_base_dataset_params.yaml
--rw-r--r--  2.0 unx     1762 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/mapillary_dataset_params.yaml
--rw-r--r--  2.0 unx      149 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/pascal_aug_segmentation_dataset_params.yaml
--rw-r--r--  2.0 unx     1571 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/pascal_voc_detection_dataset_params.yaml
--rw-r--r--  2.0 unx     1414 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/pascal_voc_segmentation_dataset_params.yaml
--rw-r--r--  2.0 unx     4112 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/roboflow_detection_dataset_params.yaml
--rw-r--r--  2.0 unx      961 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/supervisely_persons_dataset_params.yaml
--rw-r--r--  2.0 unx      559 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/tiny_imagenet_dataset_params.yaml
--rw-r--r--  2.0 unx     1155 b- defN 23-May-03 19:50 super_gradients/recipes/quantization_params/default_quantization_params.yaml
--rw-r--r--  2.0 unx      591 b- defN 23-May-03 19:50 super_gradients/recipes/training_hyperparams/cifar10_resnet_train_params.yaml
--rw-r--r--  2.0 unx      700 b- defN 23-May-03 19:50 super_gradients/recipes/training_hyperparams/cityscapes_default_train_params.yaml
--rw-r--r--  2.0 unx      877 b- defN 23-May-03 19:50 super_gradients/recipes/training_hyperparams/coco2017_dekr_pose_train_params.yaml
--rw-r--r--  2.0 unx     1302 b- defN 23-May-03 19:50 super_gradients/recipes/training_hyperparams/coco2017_ppyoloe_train_params.yaml
--rw-r--r--  2.0 unx      723 b- defN 23-May-03 19:50 super_gradients/recipes/training_hyperparams/coco2017_ssd_lite_mobilenet_v2_train_params.yaml
--rw-r--r--  2.0 unx     1121 b- defN 23-May-03 19:50 super_gradients/recipes/training_hyperparams/coco2017_yolo_nas_train_params.yaml
--rw-r--r--  2.0 unx      956 b- defN 23-May-03 19:50 super_gradients/recipes/training_hyperparams/coco2017_yolox_train_params.yaml
--rw-r--r--  2.0 unx      461 b- defN 23-May-03 19:50 super_gradients/recipes/training_hyperparams/coco_segmentation_shelfnet_lw_train_params.yaml
--rw-r--r--  2.0 unx     5459 b- defN 23-May-03 19:50 super_gradients/recipes/training_hyperparams/default_train_params.yaml
--rw-r--r--  2.0 unx      794 b- defN 23-May-03 19:50 super_gradients/recipes/training_hyperparams/imagenet_efficientnet_train_params.yaml
--rw-r--r--  2.0 unx      742 b- defN 23-May-03 19:50 super_gradients/recipes/training_hyperparams/imagenet_mobilenetv2_train_params.yaml
--rw-r--r--  2.0 unx      549 b- defN 23-May-03 19:50 super_gradients/recipes/training_hyperparams/imagenet_mobilenetv3_train_params.yaml
--rw-r--r--  2.0 unx      795 b- defN 23-May-03 19:50 super_gradients/recipes/training_hyperparams/imagenet_regnetY_train_params.yaml
--rw-r--r--  2.0 unx      476 b- defN 23-May-03 19:50 super_gradients/recipes/training_hyperparams/imagenet_repvgg_train_params.yaml
--rw-r--r--  2.0 unx      484 b- defN 23-May-03 19:50 super_gradients/recipes/training_hyperparams/imagenet_resnet50_kd_train_params.yaml
--rw-r--r--  2.0 unx      522 b- defN 23-May-03 19:50 super_gradients/recipes/training_hyperparams/imagenet_resnet50_train_params.yaml
--rw-r--r--  2.0 unx      602 b- defN 23-May-03 19:50 super_gradients/recipes/training_hyperparams/imagenet_vit_train_params.yaml
--rw-r--r--  2.0 unx      519 b- defN 23-May-03 19:50 super_gradients/recipes/training_hyperparams/supervisely_default_train_params.yaml
--rw-r--r--  2.0 unx      107 b- defN 23-May-03 19:50 super_gradients/sanity_check/__init__.py
--rw-r--r--  2.0 unx     5262 b- defN 23-May-03 19:50 super_gradients/sanity_check/env_sanity_check.py
--rw-r--r--  2.0 unx      666 b- defN 23-May-03 19:50 super_gradients/training/__init__.py
--rw-r--r--  2.0 unx     4155 b- defN 23-May-03 19:50 super_gradients/training/params.py
--rw-r--r--  2.0 unx     4301 b- defN 23-May-03 19:50 super_gradients/training/pretrained_models.py
--rw-r--r--  2.0 unx     3224 b- defN 23-May-03 19:50 super_gradients/training/dataloaders/__init__.py
--rw-r--r--  2.0 unx    32361 b- defN 23-May-03 19:50 super_gradients/training/dataloaders/dataloaders.py
--rw-r--r--  2.0 unx     1811 b- defN 23-May-03 19:50 super_gradients/training/datasets/__init__.py
--rw-r--r--  2.0 unx    14162 b- defN 23-May-03 19:50 super_gradients/training/datasets/auto_augment.py
--rw-r--r--  2.0 unx     3705 b- defN 23-May-03 19:50 super_gradients/training/datasets/data_augmentation.py
--rw-r--r--  2.0 unx     3484 b- defN 23-May-03 19:50 super_gradients/training/datasets/datasets_conf.py
--rw-r--r--  2.0 unx    30279 b- defN 23-May-03 19:50 super_gradients/training/datasets/datasets_utils.py
--rw-r--r--  2.0 unx    14663 b- defN 23-May-03 19:50 super_gradients/training/datasets/mixup.py
--rw-r--r--  2.0 unx    11746 b- defN 23-May-03 19:50 super_gradients/training/datasets/sg_dataset.py
--rw-r--r--  2.0 unx      252 b- defN 23-May-03 19:50 super_gradients/training/datasets/classification_datasets/__init__.py
--rw-r--r--  2.0 unx     3096 b- defN 23-May-03 19:50 super_gradients/training/datasets/classification_datasets/cifar.py
--rw-r--r--  2.0 unx     1706 b- defN 23-May-03 19:50 super_gradients/training/datasets/classification_datasets/imagenet_dataset.py
--rw-r--r--  2.0 unx      862 b- defN 23-May-03 19:50 super_gradients/training/datasets/data_formats/__init__.py
--rw-r--r--  2.0 unx     3927 b- defN 23-May-03 19:50 super_gradients/training/datasets/data_formats/default_formats.py
--rw-r--r--  2.0 unx     3071 b- defN 23-May-03 19:50 super_gradients/training/datasets/data_formats/format_converter.py
--rw-r--r--  2.0 unx     7928 b- defN 23-May-03 19:50 super_gradients/training/datasets/data_formats/formats.py
--rw-r--r--  2.0 unx     1044 b- defN 23-May-03 19:50 super_gradients/training/datasets/data_formats/bbox_formats/__init__.py
--rw-r--r--  2.0 unx     2674 b- defN 23-May-03 19:50 super_gradients/training/datasets/data_formats/bbox_formats/bbox_format.py
--rw-r--r--  2.0 unx     5094 b- defN 23-May-03 19:50 super_gradients/training/datasets/data_formats/bbox_formats/cxcywh.py
--rw-r--r--  2.0 unx     2089 b- defN 23-May-03 19:50 super_gradients/training/datasets/data_formats/bbox_formats/normalized_cxcywh.py
--rw-r--r--  2.0 unx     2043 b- defN 23-May-03 19:50 super_gradients/training/datasets/data_formats/bbox_formats/normalized_xywh.py
--rw-r--r--  2.0 unx     5043 b- defN 23-May-03 19:50 super_gradients/training/datasets/data_formats/bbox_formats/normalized_xyxy.py
--rw-r--r--  2.0 unx     2948 b- defN 23-May-03 19:50 super_gradients/training/datasets/data_formats/bbox_formats/xywh.py
--rw-r--r--  2.0 unx      575 b- defN 23-May-03 19:50 super_gradients/training/datasets/data_formats/bbox_formats/xyxy.py
--rw-r--r--  2.0 unx     1792 b- defN 23-May-03 19:50 super_gradients/training/datasets/data_formats/bbox_formats/yxyx.py
--rw-r--r--  2.0 unx       92 b- defN 23-May-03 19:50 super_gradients/training/datasets/data_formats/output_adapters/__init__.py
--rw-r--r--  2.0 unx     8373 b- defN 23-May-03 19:50 super_gradients/training/datasets/data_formats/output_adapters/detection_adapter.py
--rw-r--r--  2.0 unx      683 b- defN 23-May-03 19:50 super_gradients/training/datasets/detection_datasets/__init__.py
--rw-r--r--  2.0 unx     2505 b- defN 23-May-03 19:50 super_gradients/training/datasets/detection_datasets/coco_detection.py
--rw-r--r--  2.0 unx     9258 b- defN 23-May-03 19:50 super_gradients/training/datasets/detection_datasets/coco_format_detection.py
--rw-r--r--  2.0 unx    26159 b- defN 23-May-03 19:50 super_gradients/training/datasets/detection_datasets/detection_dataset.py
--rw-r--r--  2.0 unx    11353 b- defN 23-May-03 19:50 super_gradients/training/datasets/detection_datasets/pascal_voc_detection.py
--rw-r--r--  2.0 unx    11120 b- defN 23-May-03 19:50 super_gradients/training/datasets/detection_datasets/yolo_format_detection.py
--rw-r--r--  2.0 unx      328 b- defN 23-May-03 19:50 super_gradients/training/datasets/detection_datasets/roboflow/__init__.py
--rw-r--r--  2.0 unx    18882 b- defN 23-May-03 19:50 super_gradients/training/datasets/detection_datasets/roboflow/metadata.py
--rw-r--r--  2.0 unx     3504 b- defN 23-May-03 19:50 super_gradients/training/datasets/detection_datasets/roboflow/roboflow100.py
--rw-r--r--  2.0 unx     1997 b- defN 23-May-03 19:50 super_gradients/training/datasets/detection_datasets/roboflow/utils.py
--rw-r--r--  2.0 unx      502 b- defN 23-May-03 19:50 super_gradients/training/datasets/pose_estimation_datasets/__init__.py
--rw-r--r--  2.0 unx     4910 b- defN 23-May-03 19:50 super_gradients/training/datasets/pose_estimation_datasets/base_keypoints.py
--rw-r--r--  2.0 unx     9066 b- defN 23-May-03 19:50 super_gradients/training/datasets/pose_estimation_datasets/coco_keypoints.py
--rw-r--r--  2.0 unx     5929 b- defN 23-May-03 19:50 super_gradients/training/datasets/pose_estimation_datasets/coco_utils.py
--rw-r--r--  2.0 unx    10167 b- defN 23-May-03 19:50 super_gradients/training/datasets/pose_estimation_datasets/target_generators.py
--rw-r--r--  2.0 unx      278 b- defN 23-May-03 19:50 super_gradients/training/datasets/samplers/__init__.py
--rw-r--r--  2.0 unx     4809 b- defN 23-May-03 19:50 super_gradients/training/datasets/samplers/repeated_augmentation_sampler.py
--rw-r--r--  2.0 unx     1037 b- defN 23-May-03 19:50 super_gradients/training/datasets/segmentation_datasets/__init__.py
--rw-r--r--  2.0 unx     6714 b- defN 23-May-03 19:50 super_gradients/training/datasets/segmentation_datasets/cityscape_segmentation.py
--rw-r--r--  2.0 unx     7717 b- defN 23-May-03 19:50 super_gradients/training/datasets/segmentation_datasets/coco_segmentation.py
--rw-r--r--  2.0 unx     5518 b- defN 23-May-03 19:50 super_gradients/training/datasets/segmentation_datasets/mapillary_dataset.py
--rw-r--r--  2.0 unx    11146 b- defN 23-May-03 19:50 super_gradients/training/datasets/segmentation_datasets/pascal_voc_segmentation.py
--rw-r--r--  2.0 unx     8470 b- defN 23-May-03 19:50 super_gradients/training/datasets/segmentation_datasets/segmentation_dataset.py
--rw-r--r--  2.0 unx     3062 b- defN 23-May-03 19:50 super_gradients/training/datasets/segmentation_datasets/supervisely_persons_segmentation.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/training/exceptions/__init__.py
--rw-r--r--  2.0 unx     1761 b- defN 23-May-03 19:50 super_gradients/training/exceptions/dataset_exceptions.py
--rw-r--r--  2.0 unx     2826 b- defN 23-May-03 19:50 super_gradients/training/exceptions/kd_trainer_exceptions.py
--rw-r--r--  2.0 unx      946 b- defN 23-May-03 19:50 super_gradients/training/exceptions/loss_exceptions.py
--rw-r--r--  2.0 unx     1268 b- defN 23-May-03 19:50 super_gradients/training/exceptions/sg_trainer_exceptions.py
--rw-r--r--  2.0 unx      132 b- defN 23-May-03 19:50 super_gradients/training/kd_trainer/__init__.py
--rw-r--r--  2.0 unx    16582 b- defN 23-May-03 19:50 super_gradients/training/kd_trainer/kd_trainer.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/training/legacy/__init__.py
--rw-r--r--  2.0 unx     4198 b- defN 23-May-03 19:50 super_gradients/training/legacy/utils.py
--rw-r--r--  2.0 unx     1476 b- defN 23-May-03 19:50 super_gradients/training/losses/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/training/losses/all_losses.py
--rw-r--r--  2.0 unx     1219 b- defN 23-May-03 19:50 super_gradients/training/losses/bce_dice_loss.py
--rw-r--r--  2.0 unx      419 b- defN 23-May-03 19:50 super_gradients/training/losses/bce_loss.py
--rw-r--r--  2.0 unx     2374 b- defN 23-May-03 19:50 super_gradients/training/losses/cwd_loss.py
--rw-r--r--  2.0 unx     2525 b- defN 23-May-03 19:50 super_gradients/training/losses/ddrnet_loss.py
--rw-r--r--  2.0 unx     3377 b- defN 23-May-03 19:50 super_gradients/training/losses/dekr_loss.py
--rw-r--r--  2.0 unx     5618 b- defN 23-May-03 19:50 super_gradients/training/losses/dice_ce_edge_loss.py
--rw-r--r--  2.0 unx     5208 b- defN 23-May-03 19:50 super_gradients/training/losses/dice_loss.py
--rw-r--r--  2.0 unx     1214 b- defN 23-May-03 19:50 super_gradients/training/losses/focal_loss.py
--rw-r--r--  2.0 unx     5051 b- defN 23-May-03 19:50 super_gradients/training/losses/iou_loss.py
--rw-r--r--  2.0 unx     2176 b- defN 23-May-03 19:50 super_gradients/training/losses/kd_losses.py
--rw-r--r--  2.0 unx     4177 b- defN 23-May-03 19:50 super_gradients/training/losses/label_smoothing_cross_entropy_loss.py
--rw-r--r--  2.0 unx      550 b- defN 23-May-03 19:50 super_gradients/training/losses/loss_utils.py
--rw-r--r--  2.0 unx     3854 b- defN 23-May-03 19:50 super_gradients/training/losses/mask_loss.py
--rw-r--r--  2.0 unx     4129 b- defN 23-May-03 19:50 super_gradients/training/losses/ohem_ce_loss.py
--rw-r--r--  2.0 unx    41319 b- defN 23-May-03 19:50 super_gradients/training/losses/ppyolo_loss.py
--rw-r--r--  2.0 unx     1010 b- defN 23-May-03 19:50 super_gradients/training/losses/r_squared_loss.py
--rw-r--r--  2.0 unx     3453 b- defN 23-May-03 19:50 super_gradients/training/losses/seg_kd_loss.py
--rw-r--r--  2.0 unx     1650 b- defN 23-May-03 19:50 super_gradients/training/losses/shelfnet_ohem_loss.py
--rw-r--r--  2.0 unx     1949 b- defN 23-May-03 19:50 super_gradients/training/losses/shelfnet_semantic_encoding_loss.py
--rw-r--r--  2.0 unx     8794 b- defN 23-May-03 19:50 super_gradients/training/losses/ssd_loss.py
--rw-r--r--  2.0 unx     9721 b- defN 23-May-03 19:50 super_gradients/training/losses/stdc_loss.py
--rw-r--r--  2.0 unx     5771 b- defN 23-May-03 19:50 super_gradients/training/losses/structure_loss.py
--rw-r--r--  2.0 unx    50149 b- defN 23-May-03 19:50 super_gradients/training/losses/yolox_loss.py
--rw-r--r--  2.0 unx     1052 b- defN 23-May-03 19:50 super_gradients/training/metrics/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/training/metrics/all_metrics.py
--rw-r--r--  2.0 unx     3262 b- defN 23-May-03 19:50 super_gradients/training/metrics/classification_metrics.py
--rw-r--r--  2.0 unx    10741 b- defN 23-May-03 19:50 super_gradients/training/metrics/detection_metrics.py
--rw-r--r--  2.0 unx     3973 b- defN 23-May-03 19:50 super_gradients/training/metrics/metric_utils.py
--rw-r--r--  2.0 unx    15346 b- defN 23-May-03 19:50 super_gradients/training/metrics/pose_estimation_metrics.py
--rw-r--r--  2.0 unx    11454 b- defN 23-May-03 19:50 super_gradients/training/metrics/pose_estimation_utils.py
--rw-r--r--  2.0 unx    11935 b- defN 23-May-03 19:50 super_gradients/training/metrics/segmentation_metrics.py
--rw-r--r--  2.0 unx     8617 b- defN 23-May-03 19:50 super_gradients/training/models/__init__.py
--rw-r--r--  2.0 unx     1226 b- defN 23-May-03 19:50 super_gradients/training/models/arch_params_factory.py
--rw-r--r--  2.0 unx     7060 b- defN 23-May-03 19:50 super_gradients/training/models/conversion.py
--rw-r--r--  2.0 unx    11875 b- defN 23-May-03 19:50 super_gradients/training/models/model_factory.py
--rw-r--r--  2.0 unx    10986 b- defN 23-May-03 19:50 super_gradients/training/models/prediction_results.py
--rw-r--r--  2.0 unx     2054 b- defN 23-May-03 19:50 super_gradients/training/models/predictions.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/training/models/results.py
--rw-r--r--  2.0 unx     2998 b- defN 23-May-03 19:50 super_gradients/training/models/sg_module.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/training/models/classification_models/__init__.py
--rw-r--r--  2.0 unx    20025 b- defN 23-May-03 19:50 super_gradients/training/models/classification_models/beit.py
--rw-r--r--  2.0 unx     7472 b- defN 23-May-03 19:50 super_gradients/training/models/classification_models/densenet.py
--rw-r--r--  2.0 unx     3707 b- defN 23-May-03 19:50 super_gradients/training/models/classification_models/dpn.py
--rw-r--r--  2.0 unx    36745 b- defN 23-May-03 19:50 super_gradients/training/models/classification_models/efficientnet.py
--rw-r--r--  2.0 unx     8862 b- defN 23-May-03 19:50 super_gradients/training/models/classification_models/googlenet.py
--rw-r--r--  2.0 unx      798 b- defN 23-May-03 19:50 super_gradients/training/models/classification_models/lenet.py
--rw-r--r--  2.0 unx     2407 b- defN 23-May-03 19:50 super_gradients/training/models/classification_models/mobilenet.py
--rw-r--r--  2.0 unx     9472 b- defN 23-May-03 19:50 super_gradients/training/models/classification_models/mobilenetv2.py
--rw-r--r--  2.0 unx     8696 b- defN 23-May-03 19:50 super_gradients/training/models/classification_models/mobilenetv3.py
--rw-r--r--  2.0 unx     4339 b- defN 23-May-03 19:50 super_gradients/training/models/classification_models/pnasnet.py
--rw-r--r--  2.0 unx     4209 b- defN 23-May-03 19:50 super_gradients/training/models/classification_models/preact_resnet.py
--rw-r--r--  2.0 unx    13599 b- defN 23-May-03 19:50 super_gradients/training/models/classification_models/regnet.py
--rw-r--r--  2.0 unx     7924 b- defN 23-May-03 19:50 super_gradients/training/models/classification_models/repvgg.py
--rw-r--r--  2.0 unx    15025 b- defN 23-May-03 19:50 super_gradients/training/models/classification_models/resnet.py
--rw-r--r--  2.0 unx     6294 b- defN 23-May-03 19:50 super_gradients/training/models/classification_models/resnext.py
--rw-r--r--  2.0 unx     4134 b- defN 23-May-03 19:50 super_gradients/training/models/classification_models/senet.py
--rw-r--r--  2.0 unx     3660 b- defN 23-May-03 19:50 super_gradients/training/models/classification_models/shufflenet.py
--rw-r--r--  2.0 unx     9768 b- defN 23-May-03 19:50 super_gradients/training/models/classification_models/shufflenetv2.py
--rw-r--r--  2.0 unx     1538 b- defN 23-May-03 19:50 super_gradients/training/models/classification_models/vgg.py
--rw-r--r--  2.0 unx     9210 b- defN 23-May-03 19:50 super_gradients/training/models/classification_models/vit.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/training/models/detection_models/__init__.py
--rw-r--r--  2.0 unx     9130 b- defN 23-May-03 19:50 super_gradients/training/models/detection_models/csp_darknet53.py
--rw-r--r--  2.0 unx     9814 b- defN 23-May-03 19:50 super_gradients/training/models/detection_models/csp_resnet.py
--rw-r--r--  2.0 unx     9120 b- defN 23-May-03 19:50 super_gradients/training/models/detection_models/customizable_detector.py
--rw-r--r--  2.0 unx     4746 b- defN 23-May-03 19:50 super_gradients/training/models/detection_models/darknet53.py
--rw-r--r--  2.0 unx     2315 b- defN 23-May-03 19:50 super_gradients/training/models/detection_models/ssd.py
--rw-r--r--  2.0 unx    29459 b- defN 23-May-03 19:50 super_gradients/training/models/detection_models/yolo_base.py
--rw-r--r--  2.0 unx     2459 b- defN 23-May-03 19:50 super_gradients/training/models/detection_models/yolox.py
--rw-r--r--  2.0 unx      251 b- defN 23-May-03 19:50 super_gradients/training/models/detection_models/pp_yolo_e/__init__.py
--rw-r--r--  2.0 unx     7000 b- defN 23-May-03 19:50 super_gradients/training/models/detection_models/pp_yolo_e/pan.py
--rw-r--r--  2.0 unx     3487 b- defN 23-May-03 19:50 super_gradients/training/models/detection_models/pp_yolo_e/post_prediction_callback.py
--rw-r--r--  2.0 unx     8243 b- defN 23-May-03 19:50 super_gradients/training/models/detection_models/pp_yolo_e/pp_yolo_e.py
--rw-r--r--  2.0 unx    12397 b- defN 23-May-03 19:50 super_gradients/training/models/detection_models/pp_yolo_e/pp_yolo_head.py
--rw-r--r--  2.0 unx      756 b- defN 23-May-03 19:50 super_gradients/training/models/detection_models/yolo_nas/__init__.py
--rw-r--r--  2.0 unx    12084 b- defN 23-May-03 19:50 super_gradients/training/models/detection_models/yolo_nas/dfl_heads.py
--rw-r--r--  2.0 unx     2646 b- defN 23-May-03 19:50 super_gradients/training/models/detection_models/yolo_nas/panneck.py
--rw-r--r--  2.0 unx     4124 b- defN 23-May-03 19:50 super_gradients/training/models/detection_models/yolo_nas/yolo_nas_variants.py
--rw-r--r--  2.0 unx    13329 b- defN 23-May-03 19:50 super_gradients/training/models/detection_models/yolo_nas/yolo_stages.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/training/models/kd_modules/__init__.py
--rw-r--r--  2.0 unx     3553 b- defN 23-May-03 19:50 super_gradients/training/models/kd_modules/kd_module.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/training/models/pose_estimation_models/__init__.py
--rw-r--r--  2.0 unx    21231 b- defN 23-May-03 19:50 super_gradients/training/models/pose_estimation_models/dekr_hrnet.py
--rw-r--r--  2.0 unx     1294 b- defN 23-May-03 19:50 super_gradients/training/models/pose_estimation_models/pose_ddrnet39.py
--rw-r--r--  2.0 unx     1335 b- defN 23-May-03 19:50 super_gradients/training/models/pose_estimation_models/pose_ppyolo.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/training/models/segmentation_models/__init__.py
--rw-r--r--  2.0 unx      964 b- defN 23-May-03 19:50 super_gradients/training/models/segmentation_models/common.py
--rw-r--r--  2.0 unx     5139 b- defN 23-May-03 19:50 super_gradients/training/models/segmentation_models/context_modules.py
--rw-r--r--  2.0 unx    27896 b- defN 23-May-03 19:50 super_gradients/training/models/segmentation_models/ddrnet.py
--rw-r--r--  2.0 unx     2439 b- defN 23-May-03 19:50 super_gradients/training/models/segmentation_models/ddrnet_backbones.py
--rw-r--r--  2.0 unx    21760 b- defN 23-May-03 19:50 super_gradients/training/models/segmentation_models/laddernet.py
--rw-r--r--  2.0 unx    15648 b- defN 23-May-03 19:50 super_gradients/training/models/segmentation_models/ppliteseg.py
--rw-r--r--  2.0 unx    14424 b- defN 23-May-03 19:50 super_gradients/training/models/segmentation_models/regseg.py
--rw-r--r--  2.0 unx    20334 b- defN 23-May-03 19:50 super_gradients/training/models/segmentation_models/segformer.py
--rw-r--r--  2.0 unx     2256 b- defN 23-May-03 19:50 super_gradients/training/models/segmentation_models/segmentation_module.py
--rw-r--r--  2.0 unx    24833 b- defN 23-May-03 19:50 super_gradients/training/models/segmentation_models/shelfnet.py
--rw-r--r--  2.0 unx    29005 b- defN 23-May-03 19:50 super_gradients/training/models/segmentation_models/stdc.py
--rw-r--r--  2.0 unx      260 b- defN 23-May-03 19:50 super_gradients/training/models/segmentation_models/unet/__init__.py
--rw-r--r--  2.0 unx    12324 b- defN 23-May-03 19:50 super_gradients/training/models/segmentation_models/unet/unet.py
--rw-r--r--  2.0 unx    10718 b- defN 23-May-03 19:50 super_gradients/training/models/segmentation_models/unet/unet_decoder.py
--rw-r--r--  2.0 unx    13292 b- defN 23-May-03 19:50 super_gradients/training/models/segmentation_models/unet/unet_encoder.py
--rw-r--r--  2.0 unx      119 b- defN 23-May-03 19:50 super_gradients/training/models/user_models/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/training/pipelines/__init__.py
--rw-r--r--  2.0 unx    14562 b- defN 23-May-03 19:50 super_gradients/training/pipelines/pipelines.py
--rw-r--r--  2.0 unx      393 b- defN 23-May-03 19:50 super_gradients/training/pre_launch_callbacks/__init__.py
--rw-r--r--  2.0 unx    13955 b- defN 23-May-03 19:50 super_gradients/training/pre_launch_callbacks/pre_launch_callbacks.py
--rw-r--r--  2.0 unx      517 b- defN 23-May-03 19:50 super_gradients/training/processing/__init__.py
--rw-r--r--  2.0 unx    13177 b- defN 23-May-03 19:50 super_gradients/training/processing/processing.py
--rw-r--r--  2.0 unx       98 b- defN 23-May-03 19:50 super_gradients/training/qat_trainer/__init__.py
--rw-r--r--  2.0 unx     9701 b- defN 23-May-03 19:50 super_gradients/training/qat_trainer/qat_trainer.py
--rw-r--r--  2.0 unx      184 b- defN 23-May-03 19:50 super_gradients/training/sg_trainer/__init__.py
--rw-r--r--  2.0 unx    96749 b- defN 23-May-03 19:50 super_gradients/training/sg_trainer/sg_trainer.py
--rw-r--r--  2.0 unx     1685 b- defN 23-May-03 19:50 super_gradients/training/training_hyperparams/__init__.py
--rw-r--r--  2.0 unx     3774 b- defN 23-May-03 19:50 super_gradients/training/training_hyperparams/training_hyperparams.py
--rw-r--r--  2.0 unx     1024 b- defN 23-May-03 19:50 super_gradients/training/transforms/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/training/transforms/all_transforms.py
--rw-r--r--  2.0 unx    16193 b- defN 23-May-03 19:50 super_gradients/training/transforms/keypoint_transforms.py
--rw-r--r--  2.0 unx     1134 b- defN 23-May-03 19:50 super_gradients/training/transforms/pipeline_adaptors.py
--rw-r--r--  2.0 unx    55089 b- defN 23-May-03 19:50 super_gradients/training/transforms/transforms.py
--rw-r--r--  2.0 unx     6048 b- defN 23-May-03 19:50 super_gradients/training/transforms/utils.py
--rw-r--r--  2.0 unx     1104 b- defN 23-May-03 19:50 super_gradients/training/utils/__init__.py
--rw-r--r--  2.0 unx     1673 b- defN 23-May-03 19:50 super_gradients/training/utils/activations_utils.py
--rw-r--r--  2.0 unx     1111 b- defN 23-May-03 19:50 super_gradients/training/utils/bbox_utils.py
--rw-r--r--  2.0 unx    15315 b- defN 23-May-03 19:50 super_gradients/training/utils/checkpoint_utils.py
--rw-r--r--  2.0 unx     9794 b- defN 23-May-03 19:50 super_gradients/training/utils/config_utils.py
--rw-r--r--  2.0 unx     1132 b- defN 23-May-03 19:50 super_gradients/training/utils/deprecated_utils.py
--rw-r--r--  2.0 unx    53278 b- defN 23-May-03 19:50 super_gradients/training/utils/detection_utils.py
--rw-r--r--  2.0 unx    16195 b- defN 23-May-03 19:50 super_gradients/training/utils/distributed_training_utils.py
--rw-r--r--  2.0 unx     6352 b- defN 23-May-03 19:50 super_gradients/training/utils/early_stopping.py
--rw-r--r--  2.0 unx     9322 b- defN 23-May-03 19:50 super_gradients/training/utils/ema.py
--rw-r--r--  2.0 unx     2610 b- defN 23-May-03 19:50 super_gradients/training/utils/ema_decay_schedules.py
--rw-r--r--  2.0 unx     1072 b- defN 23-May-03 19:50 super_gradients/training/utils/export_utils.py
--rw-r--r--  2.0 unx     7508 b- defN 23-May-03 19:50 super_gradients/training/utils/get_model_stats.py
--rw-r--r--  2.0 unx      771 b- defN 23-May-03 19:50 super_gradients/training/utils/kd_trainer_utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/training/utils/load_image.py
--rw-r--r--  2.0 unx     5827 b- defN 23-May-03 19:50 super_gradients/training/utils/optimizer_utils.py
--rw-r--r--  2.0 unx      839 b- defN 23-May-03 19:50 super_gradients/training/utils/regularization_utils.py
--rw-r--r--  2.0 unx    10388 b- defN 23-May-03 19:50 super_gradients/training/utils/segmentation_utils.py
--rw-r--r--  2.0 unx    19625 b- defN 23-May-03 19:50 super_gradients/training/utils/sg_trainer_utils.py
--rw-r--r--  2.0 unx     6272 b- defN 23-May-03 19:50 super_gradients/training/utils/ssd_utils.py
--rw-r--r--  2.0 unx    18273 b- defN 23-May-03 19:50 super_gradients/training/utils/utils.py
--rw-r--r--  2.0 unx      303 b- defN 23-May-03 19:50 super_gradients/training/utils/version_utils.py
--rw-r--r--  2.0 unx     6209 b- defN 23-May-03 19:50 super_gradients/training/utils/weight_averaging_utils.py
--rw-r--r--  2.0 unx     2030 b- defN 23-May-03 19:50 super_gradients/training/utils/callbacks/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/training/utils/callbacks/all_callbacks.py
--rw-r--r--  2.0 unx    20126 b- defN 23-May-03 19:50 super_gradients/training/utils/callbacks/base_callbacks.py
--rw-r--r--  2.0 unx    32630 b- defN 23-May-03 19:50 super_gradients/training/utils/callbacks/callbacks.py
--rw-r--r--  2.0 unx     1169 b- defN 23-May-03 19:50 super_gradients/training/utils/callbacks/ppyoloe_switch_callback.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/training/utils/media/__init__.py
--rw-r--r--  2.0 unx     5880 b- defN 23-May-03 19:50 super_gradients/training/utils/media/image.py
--rw-r--r--  2.0 unx     4046 b- defN 23-May-03 19:50 super_gradients/training/utils/media/stream.py
--rw-r--r--  2.0 unx     6926 b- defN 23-May-03 19:50 super_gradients/training/utils/media/video.py
--rw-r--r--  2.0 unx      396 b- defN 23-May-03 19:50 super_gradients/training/utils/optimizers/__init__.py
--rw-r--r--  2.0 unx     9760 b- defN 23-May-03 19:50 super_gradients/training/utils/optimizers/lamb.py
--rw-r--r--  2.0 unx     3008 b- defN 23-May-03 19:50 super_gradients/training/utils/optimizers/lion.py
--rw-r--r--  2.0 unx     6834 b- defN 23-May-03 19:50 super_gradients/training/utils/optimizers/rmsprop_tf.py
--rw-r--r--  2.0 unx      213 b- defN 23-May-03 19:50 super_gradients/training/utils/pose_estimation/__init__.py
--rw-r--r--  2.0 unx    11167 b- defN 23-May-03 19:50 super_gradients/training/utils/pose_estimation/dekr_decode_callbacks.py
--rw-r--r--  2.0 unx     7140 b- defN 23-May-03 19:50 super_gradients/training/utils/pose_estimation/dekr_visualization_callbacks.py
--rw-r--r--  2.0 unx      387 b- defN 23-May-03 19:50 super_gradients/training/utils/quantization/__init__.py
--rw-r--r--  2.0 unx     6271 b- defN 23-May-03 19:50 super_gradients/training/utils/quantization/calibrator.py
--rw-r--r--  2.0 unx     8417 b- defN 23-May-03 19:50 super_gradients/training/utils/quantization/core.py
--rw-r--r--  2.0 unx     2196 b- defN 23-May-03 19:50 super_gradients/training/utils/quantization/export.py
--rw-r--r--  2.0 unx    17062 b- defN 23-May-03 19:50 super_gradients/training/utils/quantization/selective_quantization_utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/training/utils/visualization/__init__.py
--rw-r--r--  2.0 unx     1698 b- defN 23-May-03 19:50 super_gradients/training/utils/visualization/detection.py
--rw-r--r--  2.0 unx     2847 b- defN 23-May-03 19:50 super_gradients/training/utils/visualization/utils.py
--rw-r--r--  2.0 unx     2218 b- defN 23-May-03 19:50 super_gradients-3.1.1.dist-info/LICENSE.YOLONAS.md
--rw-r--r--  2.0 unx    11341 b- defN 23-May-03 19:50 super_gradients-3.1.1.dist-info/LICENSE.md
--rw-r--r--  2.0 unx    36095 b- defN 23-May-03 19:50 super_gradients-3.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-03 19:50 super_gradients-3.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-May-03 19:50 super_gradients-3.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    64233 b- defN 23-May-03 19:50 super_gradients-3.1.1.dist-info/RECORD
-557 files, 2815305 bytes uncompressed, 856289 bytes compressed:  69.6%
+Zip file size: 983193 bytes, number of entries: 567
+-rw-r--r--  2.0 unx      916 b- defN 23-Jun-07 12:02 super_gradients/__init__.py
+-rw-r--r--  2.0 unx     1657 b- defN 23-Jun-07 12:02 super_gradients/evaluate_checkpoint.py
+-rw-r--r--  2.0 unx     1807 b- defN 23-Jun-07 12:02 super_gradients/evaluate_from_recipe.py
+-rw-r--r--  2.0 unx      639 b- defN 23-Jun-07 12:02 super_gradients/qat_from_recipe.py
+-rwxr-xr-x  2.0 unx       28 b- defN 23-Jun-07 12:03 super_gradients/requirements.pro.txt
+-rwxr-xr-x  2.0 unx      729 b- defN 23-Jun-07 12:03 super_gradients/requirements.txt
+-rw-r--r--  2.0 unx      537 b- defN 23-Jun-07 12:02 super_gradients/resume_experiment.py
+-rw-r--r--  2.0 unx      693 b- defN 23-Jun-07 12:02 super_gradients/train_from_kd_recipe.py
+-rw-r--r--  2.0 unx      650 b- defN 23-Jun-07 12:02 super_gradients/train_from_recipe.py
+-rw-r--r--  2.0 unx     1098 b- defN 23-Jun-07 12:02 super_gradients/common/__init__.py
+-rw-r--r--  2.0 unx    15566 b- defN 23-Jun-07 12:02 super_gradients/common/object_names.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/common/abstractions/__init__.py
+-rw-r--r--  2.0 unx      879 b- defN 23-Jun-07 12:02 super_gradients/common/abstractions/abstract_logger.py
+-rw-r--r--  2.0 unx     3129 b- defN 23-Jun-07 12:02 super_gradients/common/abstractions/mute_processes.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/common/auto_logging/__init__.py
+-rw-r--r--  2.0 unx     4846 b- defN 23-Jun-07 12:02 super_gradients/common/auto_logging/auto_logger.py
+-rw-r--r--  2.0 unx     6625 b- defN 23-Jun-07 12:02 super_gradients/common/auto_logging/console_logging.py
+-rw-r--r--  2.0 unx      142 b- defN 23-Jun-07 12:02 super_gradients/common/aws_connection/__init__.py
+-rw-r--r--  2.0 unx     4182 b- defN 23-Jun-07 12:02 super_gradients/common/aws_connection/aws_connector.py
+-rw-r--r--  2.0 unx     7198 b- defN 23-Jun-07 12:02 super_gradients/common/aws_connection/aws_secrets_manager_connector.py
+-rw-r--r--  2.0 unx      119 b- defN 23-Jun-07 12:02 super_gradients/common/crash_handler/__init__.py
+-rw-r--r--  2.0 unx      669 b- defN 23-Jun-07 12:02 super_gradients/common/crash_handler/crash_handler.py
+-rw-r--r--  2.0 unx    11775 b- defN 23-Jun-07 12:02 super_gradients/common/crash_handler/crash_tips.py
+-rw-r--r--  2.0 unx      886 b- defN 23-Jun-07 12:02 super_gradients/common/crash_handler/crash_tips_setup.py
+-rw-r--r--  2.0 unx     1740 b- defN 23-Jun-07 12:02 super_gradients/common/crash_handler/exception.py
+-rw-r--r--  2.0 unx     2397 b- defN 23-Jun-07 12:02 super_gradients/common/crash_handler/exception_monitoring_setup.py
+-rw-r--r--  2.0 unx      789 b- defN 23-Jun-07 12:02 super_gradients/common/crash_handler/utils.py
+-rw-r--r--  2.0 unx      140 b- defN 23-Jun-07 12:02 super_gradients/common/data_connection/__init__.py
+-rw-r--r--  2.0 unx    17959 b- defN 23-Jun-07 12:02 super_gradients/common/data_connection/s3_connector.py
+-rw-r--r--  2.0 unx      325 b- defN 23-Jun-07 12:02 super_gradients/common/data_interface/__init__.py
+-rw-r--r--  2.0 unx     9699 b- defN 23-Jun-07 12:02 super_gradients/common/data_interface/adnn_model_repository_data_interface.py
+-rw-r--r--  2.0 unx     2050 b- defN 23-Jun-07 12:02 super_gradients/common/data_interface/dataset_data_interface.py
+-rw-r--r--  2.0 unx      220 b- defN 23-Jun-07 12:02 super_gradients/common/data_types/__init__.py
+-rw-r--r--  2.0 unx      597 b- defN 23-Jun-07 12:02 super_gradients/common/data_types/enum/__init__.py
+-rw-r--r--  2.0 unx      309 b- defN 23-Jun-07 12:02 super_gradients/common/data_types/enum/deep_learning_task.py
+-rw-r--r--  2.0 unx      108 b- defN 23-Jun-07 12:02 super_gradients/common/data_types/enum/downsample_mode.py
+-rw-r--r--  2.0 unx      317 b- defN 23-Jun-07 12:02 super_gradients/common/data_types/enum/evaluation_type.py
+-rw-r--r--  2.0 unx     1025 b- defN 23-Jun-07 12:02 super_gradients/common/data_types/enum/multi_gpu_mode.py
+-rw-r--r--  2.0 unx     1200 b- defN 23-Jun-07 12:02 super_gradients/common/data_types/enum/strict_load.py
+-rw-r--r--  2.0 unx      202 b- defN 23-Jun-07 12:02 super_gradients/common/data_types/enum/upsample_mode.py
+-rw-r--r--  2.0 unx      257 b- defN 23-Jun-07 12:02 super_gradients/common/decorators/__init__.py
+-rw-r--r--  2.0 unx     1567 b- defN 23-Jun-07 12:02 super_gradients/common/decorators/code_save_decorator.py
+-rw-r--r--  2.0 unx     3663 b- defN 23-Jun-07 12:02 super_gradients/common/decorators/deci_logger.py
+-rw-r--r--  2.0 unx     2921 b- defN 23-Jun-07 12:02 super_gradients/common/decorators/explicit_params_validator.py
+-rw-r--r--  2.0 unx     1315 b- defN 23-Jun-07 12:02 super_gradients/common/decorators/factory_decorator.py
+-rw-r--r--  2.0 unx     1132 b- defN 23-Jun-07 12:02 super_gradients/common/decorators/singleton.py
+-rw-r--r--  2.0 unx      202 b- defN 23-Jun-07 12:02 super_gradients/common/environment/__init__.py
+-rw-r--r--  2.0 unx      993 b- defN 23-Jun-07 12:02 super_gradients/common/environment/argparse_utils.py
+-rw-r--r--  2.0 unx     9170 b- defN 23-Jun-07 12:02 super_gradients/common/environment/cfg_utils.py
+-rw-r--r--  2.0 unx     4383 b- defN 23-Jun-07 12:02 super_gradients/common/environment/checkpoints_dir_utils.py
+-rw-r--r--  2.0 unx     2682 b- defN 23-Jun-07 12:02 super_gradients/common/environment/ddp_utils.py
+-rw-r--r--  2.0 unx      752 b- defN 23-Jun-07 12:02 super_gradients/common/environment/device_utils.py
+-rw-r--r--  2.0 unx      927 b- defN 23-Jun-07 12:02 super_gradients/common/environment/env_variables.py
+-rw-r--r--  2.0 unx     4047 b- defN 23-Jun-07 12:02 super_gradients/common/environment/omegaconf_utils.py
+-rw-r--r--  2.0 unx      459 b- defN 23-Jun-07 12:02 super_gradients/common/environment/path_utils.py
+-rw-r--r--  2.0 unx      112 b- defN 23-Jun-07 12:02 super_gradients/common/environment/monitoring/__init__.py
+-rw-r--r--  2.0 unx      153 b- defN 23-Jun-07 12:02 super_gradients/common/environment/monitoring/cpu.py
+-rw-r--r--  2.0 unx     2517 b- defN 23-Jun-07 12:02 super_gradients/common/environment/monitoring/data_models.py
+-rw-r--r--  2.0 unx     1025 b- defN 23-Jun-07 12:02 super_gradients/common/environment/monitoring/disk.py
+-rw-r--r--  2.0 unx     5427 b- defN 23-Jun-07 12:02 super_gradients/common/environment/monitoring/monitoring.py
+-rw-r--r--  2.0 unx      948 b- defN 23-Jun-07 12:02 super_gradients/common/environment/monitoring/network.py
+-rw-r--r--  2.0 unx      629 b- defN 23-Jun-07 12:02 super_gradients/common/environment/monitoring/utils.py
+-rw-r--r--  2.0 unx      145 b- defN 23-Jun-07 12:02 super_gradients/common/environment/monitoring/virtual_memory.py
+-rw-r--r--  2.0 unx      681 b- defN 23-Jun-07 12:02 super_gradients/common/environment/monitoring/gpu/__init__.py
+-rw-r--r--  2.0 unx     2270 b- defN 23-Jun-07 12:02 super_gradients/common/environment/monitoring/gpu/gpu.py
+-rw-r--r--  2.0 unx   121647 b- defN 23-Jun-07 12:02 super_gradients/common/environment/monitoring/gpu/pynvml.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/common/exceptions/__init__.py
+-rw-r--r--  2.0 unx      926 b- defN 23-Jun-07 12:02 super_gradients/common/exceptions/factory_exceptions.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/common/factories/__init__.py
+-rw-r--r--  2.0 unx     1715 b- defN 23-Jun-07 12:02 super_gradients/common/factories/activations_type_factory.py
+-rw-r--r--  2.0 unx     2881 b- defN 23-Jun-07 12:02 super_gradients/common/factories/base_factory.py
+-rw-r--r--  2.0 unx      258 b- defN 23-Jun-07 12:02 super_gradients/common/factories/bbox_format_factory.py
+-rw-r--r--  2.0 unx      232 b- defN 23-Jun-07 12:02 super_gradients/common/factories/callbacks_factory.py
+-rw-r--r--  2.0 unx      263 b- defN 23-Jun-07 12:02 super_gradients/common/factories/collate_functions_factory.py
+-rw-r--r--  2.0 unx      292 b- defN 23-Jun-07 12:02 super_gradients/common/factories/context_modules_factory.py
+-rw-r--r--  2.0 unx      321 b- defN 23-Jun-07 12:02 super_gradients/common/factories/data_formats_factory.py
+-rw-r--r--  2.0 unx      237 b- defN 23-Jun-07 12:02 super_gradients/common/factories/datasets_factory.py
+-rw-r--r--  2.0 unx     1014 b- defN 23-Jun-07 12:02 super_gradients/common/factories/detection_modules_factory.py
+-rw-r--r--  2.0 unx      572 b- defN 23-Jun-07 12:02 super_gradients/common/factories/list_factory.py
+-rw-r--r--  2.0 unx      223 b- defN 23-Jun-07 12:02 super_gradients/common/factories/losses_factory.py
+-rw-r--r--  2.0 unx      226 b- defN 23-Jun-07 12:02 super_gradients/common/factories/metrics_factory.py
+-rw-r--r--  2.0 unx      467 b- defN 23-Jun-07 12:02 super_gradients/common/factories/optimizers_type_factory.py
+-rw-r--r--  2.0 unx      271 b- defN 23-Jun-07 12:02 super_gradients/common/factories/pre_launch_callbacks_factory.py
+-rw-r--r--  2.0 unx      623 b- defN 23-Jun-07 12:02 super_gradients/common/factories/processing_factory.py
+-rw-r--r--  2.0 unx      229 b- defN 23-Jun-07 12:02 super_gradients/common/factories/samplers_factory.py
+-rw-r--r--  2.0 unx      263 b- defN 23-Jun-07 12:02 super_gradients/common/factories/target_generator_factory.py
+-rw-r--r--  2.0 unx     1873 b- defN 23-Jun-07 12:02 super_gradients/common/factories/transforms_factory.py
+-rw-r--r--  2.0 unx     2377 b- defN 23-Jun-07 12:02 super_gradients/common/factories/type_factory.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/common/plugins/__init__.py
+-rw-r--r--  2.0 unx    12245 b- defN 23-Jun-07 12:02 super_gradients/common/plugins/deci_client.py
+-rw-r--r--  2.0 unx      143 b- defN 23-Jun-07 12:02 super_gradients/common/plugins/wandb/__init__.py
+-rw-r--r--  2.0 unx     2329 b- defN 23-Jun-07 12:02 super_gradients/common/plugins/wandb/log_predictions.py
+-rw-r--r--  2.0 unx      271 b- defN 23-Jun-07 12:02 super_gradients/common/registry/__init__.py
+-rw-r--r--  2.0 unx     1231 b- defN 23-Jun-07 12:02 super_gradients/common/registry/albumentation.py
+-rw-r--r--  2.0 unx     6006 b- defN 23-Jun-07 12:02 super_gradients/common/registry/registry.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/common/registry/registry_utils.py
+-rw-r--r--  2.0 unx      508 b- defN 23-Jun-07 12:02 super_gradients/common/sg_loggers/__init__.py
+-rw-r--r--  2.0 unx     7460 b- defN 23-Jun-07 12:02 super_gradients/common/sg_loggers/abstract_sg_logger.py
+-rw-r--r--  2.0 unx    15095 b- defN 23-Jun-07 12:02 super_gradients/common/sg_loggers/base_sg_logger.py
+-rw-r--r--  2.0 unx    10055 b- defN 23-Jun-07 12:02 super_gradients/common/sg_loggers/clearml_sg_logger.py
+-rw-r--r--  2.0 unx    10103 b- defN 23-Jun-07 12:02 super_gradients/common/sg_loggers/dagshub_sg_logger.py
+-rw-r--r--  2.0 unx     6618 b- defN 23-Jun-07 12:02 super_gradients/common/sg_loggers/deci_platform_sg_logger.py
+-rw-r--r--  2.0 unx    15000 b- defN 23-Jun-07 12:02 super_gradients/common/sg_loggers/wandb_sg_logger.py
+-rw-r--r--  2.0 unx    85509 b- defN 23-Jun-07 12:02 super_gradients/examples/SG_Walkthrough.ipynb
+-rw-r--r--  2.0 unx    69618 b- defN 23-Jun-07 12:02 super_gradients/examples/SG_quickstart_classification.ipynb
+-rw-r--r--  2.0 unx    54966 b- defN 23-Jun-07 12:02 super_gradients/examples/SG_quickstart_model_upload_deci_lab.ipynb
+-rw-r--r--  2.0 unx    65090 b- defN 23-Jun-07 12:02 super_gradients/examples/SG_quickstart_tensorboard_logger.ipynb
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/examples/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/examples/cifar10_training_torch_objects/__init__.py
+-rw-r--r--  2.0 unx     2526 b- defN 23-Jun-07 12:02 super_gradients/examples/cifar10_training_torch_objects/cifar10_training_torch_objects_example.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/examples/convert_recipe_example/__init__.py
+-rw-r--r--  2.0 unx      870 b- defN 23-Jun-07 12:02 super_gradients/examples/convert_recipe_example/convert_recipe_example.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/examples/ddrnet_imagenet/__init__.py
+-rw-r--r--  2.0 unx     3114 b- defN 23-Jun-07 12:02 super_gradients/examples/ddrnet_imagenet/ddrnet_classification_example.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/examples/deci_lab_export_example/__init__.py
+-rw-r--r--  2.0 unx     3036 b- defN 23-Jun-07 12:02 super_gradients/examples/deci_lab_export_example/deci_lab_export_example.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/examples/early_stop/__init__.py
+-rw-r--r--  2.0 unx     1596 b- defN 23-Jun-07 12:02 super_gradients/examples/early_stop/early_stop_example.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/examples/evaluate_checkpoint_example/__init__.py
+-rw-r--r--  2.0 unx      289 b- defN 23-Jun-07 12:02 super_gradients/examples/evaluate_checkpoint_example/evaluate_checkpoint.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/examples/evaluate_from_recipe_example/__init__.py
+-rw-r--r--  2.0 unx      292 b- defN 23-Jun-07 12:02 super_gradients/examples/evaluate_from_recipe_example/evaluate_from_recipe.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/examples/loggers_examples/__init__.py
+-rw-r--r--  2.0 unx     1206 b- defN 23-Jun-07 12:02 super_gradients/examples/loggers_examples/clearml_logger_example.py
+-rw-r--r--  2.0 unx     1088 b- defN 23-Jun-07 12:02 super_gradients/examples/loggers_examples/deci_platform_logger_example.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/examples/qat_from_recipe_example/__init__.py
+-rw-r--r--  2.0 unx      277 b- defN 23-Jun-07 12:02 super_gradients/examples/qat_from_recipe_example/qat_from_recipe.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/examples/quantization/__init__.py
+-rw-r--r--  2.0 unx     1104 b- defN 23-Jun-07 12:02 super_gradients/examples/quantization/non_default_calibrators_example.py
+-rw-r--r--  2.0 unx     2310 b- defN 23-Jun-07 12:02 super_gradients/examples/quantization/ptq_e2e_example.py
+-rw-r--r--  2.0 unx     1850 b- defN 23-Jun-07 12:02 super_gradients/examples/quantization/register_quantization_mapping_with_decorator_example.py
+-rw-r--r--  2.0 unx     4732 b- defN 23-Jun-07 12:02 super_gradients/examples/quantization/resnet_qat_example.py
+-rw-r--r--  2.0 unx     1163 b- defN 23-Jun-07 12:02 super_gradients/examples/quantization/skipping_quantization_example.py
+-rw-r--r--  2.0 unx      832 b- defN 23-Jun-07 12:02 super_gradients/examples/quantization/vanilla_quantize_all_example.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/examples/regseg_transfer_learning_example/__init__.py
+-rw-r--r--  2.0 unx     2379 b- defN 23-Jun-07 12:02 super_gradients/examples/regseg_transfer_learning_example/regseg_transfer_learning_example.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/examples/resume_experiment_example/__init__.py
+-rw-r--r--  2.0 unx      283 b- defN 23-Jun-07 12:02 super_gradients/examples/resume_experiment_example/resume_experiment.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/examples/train_from_kd_recipe_example/__init__.py
+-rw-r--r--  2.0 unx      292 b- defN 23-Jun-07 12:02 super_gradients/examples/train_from_kd_recipe_example/train_from_kd_recipe.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/examples/train_from_recipe_example/__init__.py
+-rw-r--r--  2.0 unx      283 b- defN 23-Jun-07 12:02 super_gradients/examples/train_from_recipe_example/train_from_recipe.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/examples/train_from_recipe_with_dataset_registry/__init__.py
+-rw-r--r--  2.0 unx     1334 b- defN 23-Jun-07 12:02 super_gradients/examples/train_from_recipe_with_dataset_registry/train.py
+-rw-r--r--  2.0 unx     1643 b- defN 23-Jun-07 12:02 super_gradients/examples/train_from_recipe_with_dataset_registry/user_dataset.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/examples/train_from_recipe_with_user_objects/__init__.py
+-rw-r--r--  2.0 unx     1326 b- defN 23-Jun-07 12:02 super_gradients/examples/train_from_recipe_with_user_objects/train.py
+-rw-r--r--  2.0 unx     2548 b- defN 23-Jun-07 12:02 super_gradients/examples/train_from_recipe_with_user_objects/user_dataset.py
+-rw-r--r--  2.0 unx      174 b- defN 23-Jun-07 12:02 super_gradients/module_interfaces/__init__.py
+-rw-r--r--  2.0 unx     2043 b- defN 23-Jun-07 12:02 super_gradients/module_interfaces/module_interfaces.py
+-rw-r--r--  2.0 unx     3366 b- defN 23-Jun-07 12:02 super_gradients/modules/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/modules/all_detection_modules.py
+-rw-r--r--  2.0 unx      617 b- defN 23-Jun-07 12:02 super_gradients/modules/anti_alias.py
+-rw-r--r--  2.0 unx      776 b- defN 23-Jun-07 12:02 super_gradients/modules/base_modules.py
+-rw-r--r--  2.0 unx     3054 b- defN 23-Jun-07 12:02 super_gradients/modules/conv_bn_act_block.py
+-rw-r--r--  2.0 unx     1976 b- defN 23-Jun-07 12:02 super_gradients/modules/conv_bn_relu_block.py
+-rw-r--r--  2.0 unx    14805 b- defN 23-Jun-07 12:02 super_gradients/modules/detection_modules.py
+-rw-r--r--  2.0 unx     2143 b- defN 23-Jun-07 12:02 super_gradients/modules/head_replacement_utils.py
+-rw-r--r--  2.0 unx     4362 b- defN 23-Jun-07 12:02 super_gradients/modules/multi_output_modules.py
+-rw-r--r--  2.0 unx      860 b- defN 23-Jun-07 12:02 super_gradients/modules/pixel_shuffle.py
+-rw-r--r--  2.0 unx     3927 b- defN 23-Jun-07 12:02 super_gradients/modules/pose_estimation_modules.py
+-rw-r--r--  2.0 unx    12250 b- defN 23-Jun-07 12:02 super_gradients/modules/qarepvgg_block.py
+-rw-r--r--  2.0 unx     8699 b- defN 23-Jun-07 12:02 super_gradients/modules/repvgg_block.py
+-rw-r--r--  2.0 unx     2138 b- defN 23-Jun-07 12:02 super_gradients/modules/sampling.py
+-rw-r--r--  2.0 unx     1459 b- defN 23-Jun-07 12:02 super_gradients/modules/se_blocks.py
+-rw-r--r--  2.0 unx     1403 b- defN 23-Jun-07 12:02 super_gradients/modules/skip_connections.py
+-rw-r--r--  2.0 unx     2968 b- defN 23-Jun-07 12:02 super_gradients/modules/utils.py
+-rw-r--r--  2.0 unx      716 b- defN 23-Jun-07 12:02 super_gradients/modules/quantization/__init__.py
+-rw-r--r--  2.0 unx     2649 b- defN 23-Jun-07 12:02 super_gradients/modules/quantization/quantized_skip_connections.py
+-rw-r--r--  2.0 unx     4604 b- defN 23-Jun-07 12:02 super_gradients/modules/quantization/quantized_stdc_blocks.py
+-rw-r--r--  2.0 unx     1281 b- defN 23-Jun-07 12:02 super_gradients/modules/quantization/resnet_bottleneck.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/recipes/__init__.py
+-rw-r--r--  2.0 unx     1136 b- defN 23-Jun-07 12:02 super_gradients/recipes/cifar10_resnet.yaml
+-rw-r--r--  2.0 unx     2727 b- defN 23-Jun-07 12:02 super_gradients/recipes/cityscapes_al_ddrnet.yaml
+-rw-r--r--  2.0 unx     3502 b- defN 23-Jun-07 12:02 super_gradients/recipes/cityscapes_ddrnet.yaml
+-rw-r--r--  2.0 unx     3754 b- defN 23-Jun-07 12:02 super_gradients/recipes/cityscapes_kd_base.yaml
+-rw-r--r--  2.0 unx     3354 b- defN 23-Jun-07 12:02 super_gradients/recipes/cityscapes_pplite_seg50.yaml
+-rw-r--r--  2.0 unx     3253 b- defN 23-Jun-07 12:02 super_gradients/recipes/cityscapes_pplite_seg75.yaml
+-rw-r--r--  2.0 unx     2498 b- defN 23-Jun-07 12:02 super_gradients/recipes/cityscapes_regseg48.yaml
+-rw-r--r--  2.0 unx     4020 b- defN 23-Jun-07 12:02 super_gradients/recipes/cityscapes_segformer.yaml
+-rw-r--r--  2.0 unx      618 b- defN 23-Jun-07 12:02 super_gradients/recipes/cityscapes_stdc_base.yaml
+-rw-r--r--  2.0 unx     2862 b- defN 23-Jun-07 12:02 super_gradients/recipes/cityscapes_stdc_seg50.yaml
+-rw-r--r--  2.0 unx     3055 b- defN 23-Jun-07 12:02 super_gradients/recipes/cityscapes_stdc_seg75.yaml
+-rw-r--r--  2.0 unx     1620 b- defN 23-Jun-07 12:02 super_gradients/recipes/coco2017_pose_dekr_rescoring.yaml
+-rw-r--r--  2.0 unx     2992 b- defN 23-Jun-07 12:02 super_gradients/recipes/coco2017_pose_dekr_w32_no_dc.yaml
+-rw-r--r--  2.0 unx     1996 b- defN 23-Jun-07 12:02 super_gradients/recipes/coco2017_ppyoloe_l.yaml
+-rw-r--r--  2.0 unx     1996 b- defN 23-Jun-07 12:02 super_gradients/recipes/coco2017_ppyoloe_m.yaml
+-rw-r--r--  2.0 unx     1882 b- defN 23-Jun-07 12:02 super_gradients/recipes/coco2017_ppyoloe_s.yaml
+-rw-r--r--  2.0 unx     1975 b- defN 23-Jun-07 12:02 super_gradients/recipes/coco2017_ppyoloe_x.yaml
+-rw-r--r--  2.0 unx     1889 b- defN 23-Jun-07 12:02 super_gradients/recipes/coco2017_ssd_lite_mobilenet_v2.yaml
+-rw-r--r--  2.0 unx     1385 b- defN 23-Jun-07 12:02 super_gradients/recipes/coco2017_yolo_nas_s.yaml
+-rw-r--r--  2.0 unx     2583 b- defN 23-Jun-07 12:02 super_gradients/recipes/coco2017_yolox.yaml
+-rw-r--r--  2.0 unx     1376 b- defN 23-Jun-07 12:02 super_gradients/recipes/coco_segmentation_shelfnet_lw.yaml
+-rw-r--r--  2.0 unx     1145 b- defN 23-Jun-07 12:02 super_gradients/recipes/imagenet_efficientnet.yaml
+-rw-r--r--  2.0 unx     1129 b- defN 23-Jun-07 12:02 super_gradients/recipes/imagenet_mobilenetv2.yaml
+-rw-r--r--  2.0 unx      507 b- defN 23-Jun-07 12:02 super_gradients/recipes/imagenet_mobilenetv3_base.yaml
+-rw-r--r--  2.0 unx      719 b- defN 23-Jun-07 12:02 super_gradients/recipes/imagenet_mobilenetv3_large.yaml
+-rw-r--r--  2.0 unx      719 b- defN 23-Jun-07 12:02 super_gradients/recipes/imagenet_mobilenetv3_small.yaml
+-rw-r--r--  2.0 unx     1997 b- defN 23-Jun-07 12:02 super_gradients/recipes/imagenet_regnetY.yaml
+-rw-r--r--  2.0 unx     1246 b- defN 23-Jun-07 12:02 super_gradients/recipes/imagenet_repvgg.yaml
+-rw-r--r--  2.0 unx     1169 b- defN 23-Jun-07 12:02 super_gradients/recipes/imagenet_resnet50.yaml
+-rw-r--r--  2.0 unx     2722 b- defN 23-Jun-07 12:02 super_gradients/recipes/imagenet_resnet50_kd.yaml
+-rw-r--r--  2.0 unx     1136 b- defN 23-Jun-07 12:02 super_gradients/recipes/imagenet_vit_base.yaml
+-rw-r--r--  2.0 unx     1010 b- defN 23-Jun-07 12:02 super_gradients/recipes/imagenet_vit_large.yaml
+-rw-r--r--  2.0 unx     2007 b- defN 23-Jun-07 12:02 super_gradients/recipes/roboflow_ppyoloe.yaml
+-rw-r--r--  2.0 unx     2347 b- defN 23-Jun-07 12:02 super_gradients/recipes/roboflow_yolo_nas_m.yaml
+-rw-r--r--  2.0 unx     2347 b- defN 23-Jun-07 12:02 super_gradients/recipes/roboflow_yolo_nas_s.yaml
+-rw-r--r--  2.0 unx      473 b- defN 23-Jun-07 12:02 super_gradients/recipes/roboflow_yolo_nas_s_qat.yaml
+-rw-r--r--  2.0 unx     1915 b- defN 23-Jun-07 12:02 super_gradients/recipes/roboflow_yolox.yaml
+-rw-r--r--  2.0 unx     1344 b- defN 23-Jun-07 12:02 super_gradients/recipes/script_generate_rescoring_data_dekr_coco2017.yaml
+-rw-r--r--  2.0 unx     1246 b- defN 23-Jun-07 12:02 super_gradients/recipes/supervisely_unet.yaml
+-rw-r--r--  2.0 unx     1672 b- defN 23-Jun-07 12:02 super_gradients/recipes/user_recipe_mnist_as_external_dataset_example.yaml
+-rw-r--r--  2.0 unx     2133 b- defN 23-Jun-07 12:02 super_gradients/recipes/user_recipe_mnist_example.yaml
+-rw-r--r--  2.0 unx     2000 b- defN 23-Jun-07 12:02 super_gradients/recipes/variable_setup.yaml
+-rw-r--r--  2.0 unx     2222 b- defN 23-Jun-07 12:02 super_gradients/recipes/anchors/ssd_anchors.yaml
+-rw-r--r--  2.0 unx      563 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/efficientnet_arch_params.yaml
+-rw-r--r--  2.0 unx      104 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/efficientnet_b0_arch_params.yaml
+-rw-r--r--  2.0 unx      103 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/efficientnet_b1_arch_params.yaml
+-rw-r--r--  2.0 unx      103 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/efficientnet_b2_arch_params.yaml
+-rw-r--r--  2.0 unx      103 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/efficientnet_b3_arch_params.yaml
+-rw-r--r--  2.0 unx      103 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/efficientnet_b4_arch_params.yaml
+-rw-r--r--  2.0 unx      103 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/efficientnet_b5_arch_params.yaml
+-rw-r--r--  2.0 unx      103 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/efficientnet_b6_arch_params.yaml
+-rw-r--r--  2.0 unx      103 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/efficientnet_b7_arch_params.yaml
+-rw-r--r--  2.0 unx      103 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/efficientnet_b8_arch_params.yaml
+-rw-r--r--  2.0 unx      103 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/efficientnet_l2_arch_params.yaml
+-rw-r--r--  2.0 unx      194 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/mobilenet_v2_arch_params.yaml
+-rw-r--r--  2.0 unx      156 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/mobilenet_v3_arch_params.yaml
+-rw-r--r--  2.0 unx      409 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/mobilenet_v3_large_arch_params.yaml
+-rw-r--r--  2.0 unx      356 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/mobilenet_v3_small_arch_params.yaml
+-rw-r--r--  2.0 unx      324 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/pose_dekr_coco_rescoring_arch_params.yaml
+-rw-r--r--  2.0 unx     1113 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/pose_dekr_w32_no_dc_arch_params.yaml
+-rw-r--r--  2.0 unx      985 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/pose_pppose_l_arch_params.yaml
+-rw-r--r--  2.0 unx     1112 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/ppyoloe_arch_params.yaml
+-rw-r--r--  2.0 unx      196 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/ppyoloe_l_arch_params.yaml
+-rw-r--r--  2.0 unx      198 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/ppyoloe_m_arch_params.yaml
+-rw-r--r--  2.0 unx      198 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/ppyoloe_s_arch_params.yaml
+-rw-r--r--  2.0 unx      198 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/ppyoloe_x_arch_params.yaml
+-rw-r--r--  2.0 unx      204 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/regnetY_arch_params.yaml
+-rw-r--r--  2.0 unx      352 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/repvgg_arch_params.yaml
+-rw-r--r--  2.0 unx       98 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/repvgga0_arch_params.yaml
+-rw-r--r--  2.0 unx       89 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/repvgga1_arch_params.yaml
+-rw-r--r--  2.0 unx       95 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/repvgga2_arch_params.yaml
+-rw-r--r--  2.0 unx       88 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/repvggb0_arch_params.yaml
+-rw-r--r--  2.0 unx       86 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/repvggb1_arch_params.yaml
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/repvggb2_arch_params.yaml
+-rw-r--r--  2.0 unx       15 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/resnet18_cifar_arch_params.yaml
+-rw-r--r--  2.0 unx       17 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/resnet50_arch_params.yaml
+-rw-r--r--  2.0 unx       32 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/shelfnet34_lw_arch_params.yaml
+-rw-r--r--  2.0 unx      655 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/ssd_lite_mobilenetv2_arch_params.yaml
+-rw-r--r--  2.0 unx      605 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/ssd_mobilenetv1_arch_params.yaml
+-rw-r--r--  2.0 unx     1369 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/unet_arch_params.yaml
+-rw-r--r--  2.0 unx     3031 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/unet_default_arch_params.yaml
+-rw-r--r--  2.0 unx       63 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/vit_base_arch_params.yaml
+-rw-r--r--  2.0 unx     2393 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/yolo_arch_params.yaml
+-rw-r--r--  2.0 unx     2353 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/yolo_nas_l_arch_params.yaml
+-rw-r--r--  2.0 unx     2362 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/yolo_nas_m_arch_params.yaml
+-rw-r--r--  2.0 unx     2357 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/yolo_nas_s_arch_params.yaml
+-rw-r--r--  2.0 unx      235 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/yolox_l_arch_params.yaml
+-rw-r--r--  2.0 unx      237 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/yolox_m_arch_params.yaml
+-rw-r--r--  2.0 unx      237 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/yolox_nano_arch_params.yaml
+-rw-r--r--  2.0 unx      237 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/yolox_s_arch_params.yaml
+-rw-r--r--  2.0 unx      229 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/yolox_tiny_arch_params.yaml
+-rw-r--r--  2.0 unx      228 b- defN 23-Jun-07 12:02 super_gradients/recipes/arch_params/yolox_x_arch_params.yaml
+-rw-r--r--  2.0 unx      622 b- defN 23-Jun-07 12:02 super_gradients/recipes/checkpoint_params/default_checkpoint_params.yaml
+-rw-r--r--  2.0 unx       72 b- defN 23-Jun-07 12:02 super_gradients/recipes/checkpoint_params/vit_base_imagenet_checkpoint_params.yaml
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/recipes/conversion_params/__init__.py
+-rw-r--r--  2.0 unx     1807 b- defN 23-Jun-07 12:02 super_gradients/recipes/conversion_params/cifar10_conversion_params.yaml
+-rw-r--r--  2.0 unx     2040 b- defN 23-Jun-07 12:02 super_gradients/recipes/conversion_params/default_conversion_params.yaml
+-rw-r--r--  2.0 unx      869 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/cifar100_dataset_params.yaml
+-rw-r--r--  2.0 unx     1530 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/cifar10_albumentations_dataset_params.yaml
+-rw-r--r--  2.0 unx     1056 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/cifar10_dataset_params.yaml
+-rw-r--r--  2.0 unx     1328 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/cityscapes_al_dataset_params.yaml
+-rw-r--r--  2.0 unx      615 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/cityscapes_dataset_params.yaml
+-rw-r--r--  2.0 unx      525 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/cityscapes_ddrnet_dataset_params.yaml
+-rw-r--r--  2.0 unx      706 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/cityscapes_ppliteseg_seg75_dataset_params.yaml
+-rw-r--r--  2.0 unx      644 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/cityscapes_regseg48_dataset_params.yaml
+-rw-r--r--  2.0 unx      721 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/cityscapes_segformer_dataset_params.yaml
+-rw-r--r--  2.0 unx      709 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/cityscapes_stdc_seg50_dataset_params.yaml
+-rw-r--r--  2.0 unx      708 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/cityscapes_stdc_seg75_dataset_params.yaml
+-rw-r--r--  2.0 unx     3946 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/coco_detection_dataset_params.yaml
+-rw-r--r--  2.0 unx     4202 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/coco_detection_ppyoloe_dataset_params.yaml
+-rw-r--r--  2.0 unx     3590 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/coco_detection_ssd_lite_mobilenet_v2_dataset_params.yaml
+-rw-r--r--  2.0 unx     5568 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/coco_detection_yolo_format_base_dataset_params.yaml
+-rw-r--r--  2.0 unx     3684 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/coco_detection_yolo_nas_dataset_params.yaml
+-rw-r--r--  2.0 unx     2700 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/coco_pose_estimation_dataset_params.yaml
+-rw-r--r--  2.0 unx      405 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/coco_pose_estimation_dekr_dataset_params.yaml
+-rw-r--r--  2.0 unx      842 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/coco_pose_estimation_rescoring_dataset_params.yaml
+-rw-r--r--  2.0 unx     1466 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/coco_segmentation_dataset_params.yaml
+-rw-r--r--  2.0 unx      931 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/imagenet_dataset_params.yaml
+-rw-r--r--  2.0 unx      732 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/imagenet_efficientnet_dataset_params.yaml
+-rw-r--r--  2.0 unx      794 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/imagenet_mobilenetv2_dataset_params.yaml
+-rw-r--r--  2.0 unx      142 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/imagenet_mobilenetv3_dataset_params.yaml
+-rw-r--r--  2.0 unx      734 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/imagenet_regnetY_dataset_params.yaml
+-rw-r--r--  2.0 unx     1059 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/imagenet_resnet50_dataset_params.yaml
+-rw-r--r--  2.0 unx     1093 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/imagenet_resnet50_kd_dataset_params.yaml
+-rw-r--r--  2.0 unx      845 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/imagenet_vit_base_dataset_params.yaml
+-rw-r--r--  2.0 unx     1762 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/mapillary_dataset_params.yaml
+-rw-r--r--  2.0 unx      149 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/pascal_aug_segmentation_dataset_params.yaml
+-rw-r--r--  2.0 unx     1571 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/pascal_voc_detection_dataset_params.yaml
+-rw-r--r--  2.0 unx     1414 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/pascal_voc_segmentation_dataset_params.yaml
+-rw-r--r--  2.0 unx     4112 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/roboflow_detection_dataset_params.yaml
+-rw-r--r--  2.0 unx      961 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/supervisely_persons_dataset_params.yaml
+-rw-r--r--  2.0 unx      559 b- defN 23-Jun-07 12:02 super_gradients/recipes/dataset_params/tiny_imagenet_dataset_params.yaml
+-rw-r--r--  2.0 unx     1155 b- defN 23-Jun-07 12:02 super_gradients/recipes/quantization_params/default_quantization_params.yaml
+-rw-r--r--  2.0 unx      591 b- defN 23-Jun-07 12:02 super_gradients/recipes/training_hyperparams/cifar10_resnet_train_params.yaml
+-rw-r--r--  2.0 unx      700 b- defN 23-Jun-07 12:02 super_gradients/recipes/training_hyperparams/cityscapes_default_train_params.yaml
+-rw-r--r--  2.0 unx     2063 b- defN 23-Jun-07 12:02 super_gradients/recipes/training_hyperparams/coco2017_dekr_pose_train_params.yaml
+-rw-r--r--  2.0 unx     1302 b- defN 23-Jun-07 12:02 super_gradients/recipes/training_hyperparams/coco2017_ppyoloe_train_params.yaml
+-rw-r--r--  2.0 unx      771 b- defN 23-Jun-07 12:02 super_gradients/recipes/training_hyperparams/coco2017_rescoring_train_params.yaml
+-rw-r--r--  2.0 unx      723 b- defN 23-Jun-07 12:02 super_gradients/recipes/training_hyperparams/coco2017_ssd_lite_mobilenet_v2_train_params.yaml
+-rw-r--r--  2.0 unx     1121 b- defN 23-Jun-07 12:02 super_gradients/recipes/training_hyperparams/coco2017_yolo_nas_train_params.yaml
+-rw-r--r--  2.0 unx      956 b- defN 23-Jun-07 12:02 super_gradients/recipes/training_hyperparams/coco2017_yolox_train_params.yaml
+-rw-r--r--  2.0 unx      461 b- defN 23-Jun-07 12:02 super_gradients/recipes/training_hyperparams/coco_segmentation_shelfnet_lw_train_params.yaml
+-rw-r--r--  2.0 unx     6081 b- defN 23-Jun-07 12:02 super_gradients/recipes/training_hyperparams/default_train_params.yaml
+-rw-r--r--  2.0 unx      794 b- defN 23-Jun-07 12:02 super_gradients/recipes/training_hyperparams/imagenet_efficientnet_train_params.yaml
+-rw-r--r--  2.0 unx      742 b- defN 23-Jun-07 12:02 super_gradients/recipes/training_hyperparams/imagenet_mobilenetv2_train_params.yaml
+-rw-r--r--  2.0 unx      549 b- defN 23-Jun-07 12:02 super_gradients/recipes/training_hyperparams/imagenet_mobilenetv3_train_params.yaml
+-rw-r--r--  2.0 unx      795 b- defN 23-Jun-07 12:02 super_gradients/recipes/training_hyperparams/imagenet_regnetY_train_params.yaml
+-rw-r--r--  2.0 unx      476 b- defN 23-Jun-07 12:02 super_gradients/recipes/training_hyperparams/imagenet_repvgg_train_params.yaml
+-rw-r--r--  2.0 unx      484 b- defN 23-Jun-07 12:02 super_gradients/recipes/training_hyperparams/imagenet_resnet50_kd_train_params.yaml
+-rw-r--r--  2.0 unx      522 b- defN 23-Jun-07 12:02 super_gradients/recipes/training_hyperparams/imagenet_resnet50_train_params.yaml
+-rw-r--r--  2.0 unx      602 b- defN 23-Jun-07 12:02 super_gradients/recipes/training_hyperparams/imagenet_vit_train_params.yaml
+-rw-r--r--  2.0 unx      519 b- defN 23-Jun-07 12:02 super_gradients/recipes/training_hyperparams/supervisely_default_train_params.yaml
+-rw-r--r--  2.0 unx      107 b- defN 23-Jun-07 12:02 super_gradients/sanity_check/__init__.py
+-rw-r--r--  2.0 unx     5267 b- defN 23-Jun-07 12:02 super_gradients/sanity_check/env_sanity_check.py
+-rw-r--r--  2.0 unx      775 b- defN 23-Jun-07 12:02 super_gradients/training/__init__.py
+-rw-r--r--  2.0 unx     4715 b- defN 23-Jun-07 12:02 super_gradients/training/params.py
+-rw-r--r--  2.0 unx     4518 b- defN 23-Jun-07 12:02 super_gradients/training/pretrained_models.py
+-rw-r--r--  2.0 unx     3344 b- defN 23-Jun-07 12:02 super_gradients/training/dataloaders/__init__.py
+-rw-r--r--  2.0 unx    36154 b- defN 23-Jun-07 12:02 super_gradients/training/dataloaders/dataloaders.py
+-rw-r--r--  2.0 unx     1867 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/__init__.py
+-rw-r--r--  2.0 unx    14162 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/auto_augment.py
+-rw-r--r--  2.0 unx     3705 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/data_augmentation.py
+-rw-r--r--  2.0 unx     3484 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/datasets_conf.py
+-rw-r--r--  2.0 unx    29577 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/datasets_utils.py
+-rw-r--r--  2.0 unx    14663 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/mixup.py
+-rw-r--r--  2.0 unx    11746 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/sg_dataset.py
+-rw-r--r--  2.0 unx      252 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/classification_datasets/__init__.py
+-rw-r--r--  2.0 unx     3096 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/classification_datasets/cifar.py
+-rw-r--r--  2.0 unx     1706 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/classification_datasets/imagenet_dataset.py
+-rw-r--r--  2.0 unx      862 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/data_formats/__init__.py
+-rw-r--r--  2.0 unx     3927 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/data_formats/default_formats.py
+-rw-r--r--  2.0 unx     3071 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/data_formats/format_converter.py
+-rw-r--r--  2.0 unx     7928 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/data_formats/formats.py
+-rw-r--r--  2.0 unx     1044 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/data_formats/bbox_formats/__init__.py
+-rw-r--r--  2.0 unx     2674 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/data_formats/bbox_formats/bbox_format.py
+-rw-r--r--  2.0 unx     5131 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/data_formats/bbox_formats/cxcywh.py
+-rw-r--r--  2.0 unx     2089 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/data_formats/bbox_formats/normalized_cxcywh.py
+-rw-r--r--  2.0 unx     2043 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/data_formats/bbox_formats/normalized_xywh.py
+-rw-r--r--  2.0 unx     5043 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/data_formats/bbox_formats/normalized_xyxy.py
+-rw-r--r--  2.0 unx     2948 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/data_formats/bbox_formats/xywh.py
+-rw-r--r--  2.0 unx      575 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/data_formats/bbox_formats/xyxy.py
+-rw-r--r--  2.0 unx     1792 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/data_formats/bbox_formats/yxyx.py
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/data_formats/output_adapters/__init__.py
+-rw-r--r--  2.0 unx     8373 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/data_formats/output_adapters/detection_adapter.py
+-rw-r--r--  2.0 unx      683 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/detection_datasets/__init__.py
+-rw-r--r--  2.0 unx     2505 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/detection_datasets/coco_detection.py
+-rw-r--r--  2.0 unx     9258 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/detection_datasets/coco_format_detection.py
+-rw-r--r--  2.0 unx    26566 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/detection_datasets/detection_dataset.py
+-rw-r--r--  2.0 unx    11353 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/detection_datasets/pascal_voc_detection.py
+-rw-r--r--  2.0 unx    11120 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/detection_datasets/yolo_format_detection.py
+-rw-r--r--  2.0 unx      328 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/detection_datasets/roboflow/__init__.py
+-rw-r--r--  2.0 unx    18882 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/detection_datasets/roboflow/metadata.py
+-rw-r--r--  2.0 unx     3503 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/detection_datasets/roboflow/roboflow100.py
+-rw-r--r--  2.0 unx     1997 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/detection_datasets/roboflow/utils.py
+-rw-r--r--  2.0 unx      502 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/pose_estimation_datasets/__init__.py
+-rw-r--r--  2.0 unx     4910 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/pose_estimation_datasets/base_keypoints.py
+-rw-r--r--  2.0 unx     9088 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/pose_estimation_datasets/coco_keypoints.py
+-rw-r--r--  2.0 unx     5929 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/pose_estimation_datasets/coco_utils.py
+-rw-r--r--  2.0 unx     3736 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/pose_estimation_datasets/rescoring_dataset.py
+-rw-r--r--  2.0 unx    10281 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/pose_estimation_datasets/target_generators.py
+-rw-r--r--  2.0 unx      385 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/samplers/__init__.py
+-rw-r--r--  2.0 unx      738 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/samplers/infinite_sampler.py
+-rw-r--r--  2.0 unx     4809 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/samplers/repeated_augmentation_sampler.py
+-rw-r--r--  2.0 unx     1093 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/segmentation_datasets/__init__.py
+-rw-r--r--  2.0 unx     8304 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/segmentation_datasets/cityscape_segmentation.py
+-rw-r--r--  2.0 unx     7757 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/segmentation_datasets/coco_segmentation.py
+-rw-r--r--  2.0 unx     5518 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/segmentation_datasets/mapillary_dataset.py
+-rw-r--r--  2.0 unx    11146 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/segmentation_datasets/pascal_voc_segmentation.py
+-rw-r--r--  2.0 unx     8572 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/segmentation_datasets/segmentation_dataset.py
+-rw-r--r--  2.0 unx     3062 b- defN 23-Jun-07 12:02 super_gradients/training/datasets/segmentation_datasets/supervisely_persons_segmentation.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/training/exceptions/__init__.py
+-rw-r--r--  2.0 unx     1761 b- defN 23-Jun-07 12:02 super_gradients/training/exceptions/dataset_exceptions.py
+-rw-r--r--  2.0 unx     2826 b- defN 23-Jun-07 12:02 super_gradients/training/exceptions/kd_trainer_exceptions.py
+-rw-r--r--  2.0 unx      946 b- defN 23-Jun-07 12:02 super_gradients/training/exceptions/loss_exceptions.py
+-rw-r--r--  2.0 unx     1268 b- defN 23-Jun-07 12:02 super_gradients/training/exceptions/sg_trainer_exceptions.py
+-rw-r--r--  2.0 unx      132 b- defN 23-Jun-07 12:02 super_gradients/training/kd_trainer/__init__.py
+-rw-r--r--  2.0 unx    16582 b- defN 23-Jun-07 12:02 super_gradients/training/kd_trainer/kd_trainer.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/training/legacy/__init__.py
+-rw-r--r--  2.0 unx     4198 b- defN 23-Jun-07 12:02 super_gradients/training/legacy/utils.py
+-rw-r--r--  2.0 unx     1570 b- defN 23-Jun-07 12:02 super_gradients/training/losses/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/training/losses/all_losses.py
+-rw-r--r--  2.0 unx     1219 b- defN 23-Jun-07 12:02 super_gradients/training/losses/bce_dice_loss.py
+-rw-r--r--  2.0 unx      419 b- defN 23-Jun-07 12:02 super_gradients/training/losses/bce_loss.py
+-rw-r--r--  2.0 unx     2374 b- defN 23-Jun-07 12:02 super_gradients/training/losses/cwd_loss.py
+-rw-r--r--  2.0 unx     2525 b- defN 23-Jun-07 12:02 super_gradients/training/losses/ddrnet_loss.py
+-rw-r--r--  2.0 unx     4038 b- defN 23-Jun-07 12:02 super_gradients/training/losses/dekr_loss.py
+-rw-r--r--  2.0 unx     5618 b- defN 23-Jun-07 12:02 super_gradients/training/losses/dice_ce_edge_loss.py
+-rw-r--r--  2.0 unx     5208 b- defN 23-Jun-07 12:02 super_gradients/training/losses/dice_loss.py
+-rw-r--r--  2.0 unx     1214 b- defN 23-Jun-07 12:02 super_gradients/training/losses/focal_loss.py
+-rw-r--r--  2.0 unx     5051 b- defN 23-Jun-07 12:02 super_gradients/training/losses/iou_loss.py
+-rw-r--r--  2.0 unx     2176 b- defN 23-Jun-07 12:02 super_gradients/training/losses/kd_losses.py
+-rw-r--r--  2.0 unx     4177 b- defN 23-Jun-07 12:02 super_gradients/training/losses/label_smoothing_cross_entropy_loss.py
+-rw-r--r--  2.0 unx      550 b- defN 23-Jun-07 12:02 super_gradients/training/losses/loss_utils.py
+-rw-r--r--  2.0 unx     4004 b- defN 23-Jun-07 12:02 super_gradients/training/losses/mask_loss.py
+-rw-r--r--  2.0 unx     4129 b- defN 23-Jun-07 12:02 super_gradients/training/losses/ohem_ce_loss.py
+-rw-r--r--  2.0 unx    41319 b- defN 23-Jun-07 12:02 super_gradients/training/losses/ppyolo_loss.py
+-rw-r--r--  2.0 unx     1010 b- defN 23-Jun-07 12:02 super_gradients/training/losses/r_squared_loss.py
+-rw-r--r--  2.0 unx      665 b- defN 23-Jun-07 12:02 super_gradients/training/losses/rescoring_loss.py
+-rw-r--r--  2.0 unx     3453 b- defN 23-Jun-07 12:02 super_gradients/training/losses/seg_kd_loss.py
+-rw-r--r--  2.0 unx     1650 b- defN 23-Jun-07 12:02 super_gradients/training/losses/shelfnet_ohem_loss.py
+-rw-r--r--  2.0 unx     1949 b- defN 23-Jun-07 12:02 super_gradients/training/losses/shelfnet_semantic_encoding_loss.py
+-rw-r--r--  2.0 unx     8794 b- defN 23-Jun-07 12:02 super_gradients/training/losses/ssd_loss.py
+-rw-r--r--  2.0 unx     9721 b- defN 23-Jun-07 12:02 super_gradients/training/losses/stdc_loss.py
+-rw-r--r--  2.0 unx     5771 b- defN 23-Jun-07 12:02 super_gradients/training/losses/structure_loss.py
+-rw-r--r--  2.0 unx    50149 b- defN 23-Jun-07 12:02 super_gradients/training/losses/yolox_loss.py
+-rw-r--r--  2.0 unx     1052 b- defN 23-Jun-07 12:02 super_gradients/training/metrics/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/training/metrics/all_metrics.py
+-rw-r--r--  2.0 unx     3262 b- defN 23-Jun-07 12:02 super_gradients/training/metrics/classification_metrics.py
+-rw-r--r--  2.0 unx    10741 b- defN 23-Jun-07 12:02 super_gradients/training/metrics/detection_metrics.py
+-rw-r--r--  2.0 unx     3973 b- defN 23-Jun-07 12:02 super_gradients/training/metrics/metric_utils.py
+-rw-r--r--  2.0 unx    15404 b- defN 23-Jun-07 12:02 super_gradients/training/metrics/pose_estimation_metrics.py
+-rw-r--r--  2.0 unx    11536 b- defN 23-Jun-07 12:02 super_gradients/training/metrics/pose_estimation_utils.py
+-rw-r--r--  2.0 unx    11935 b- defN 23-Jun-07 12:02 super_gradients/training/metrics/segmentation_metrics.py
+-rw-r--r--  2.0 unx    11245 b- defN 23-Jun-07 12:02 super_gradients/training/models/__init__.py
+-rw-r--r--  2.0 unx     1226 b- defN 23-Jun-07 12:02 super_gradients/training/models/arch_params_factory.py
+-rw-r--r--  2.0 unx    12587 b- defN 23-Jun-07 12:02 super_gradients/training/models/conversion.py
+-rw-r--r--  2.0 unx    11887 b- defN 23-Jun-07 12:02 super_gradients/training/models/model_factory.py
+-rw-r--r--  2.0 unx    10997 b- defN 23-Jun-07 12:02 super_gradients/training/models/prediction_results.py
+-rw-r--r--  2.0 unx     2054 b- defN 23-Jun-07 12:02 super_gradients/training/models/predictions.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/training/models/results.py
+-rw-r--r--  2.0 unx     2998 b- defN 23-Jun-07 12:02 super_gradients/training/models/sg_module.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/training/models/classification_models/__init__.py
+-rw-r--r--  2.0 unx    20025 b- defN 23-Jun-07 12:02 super_gradients/training/models/classification_models/beit.py
+-rw-r--r--  2.0 unx     7472 b- defN 23-Jun-07 12:02 super_gradients/training/models/classification_models/densenet.py
+-rw-r--r--  2.0 unx     3707 b- defN 23-Jun-07 12:02 super_gradients/training/models/classification_models/dpn.py
+-rw-r--r--  2.0 unx    36745 b- defN 23-Jun-07 12:02 super_gradients/training/models/classification_models/efficientnet.py
+-rw-r--r--  2.0 unx     8862 b- defN 23-Jun-07 12:02 super_gradients/training/models/classification_models/googlenet.py
+-rw-r--r--  2.0 unx      798 b- defN 23-Jun-07 12:02 super_gradients/training/models/classification_models/lenet.py
+-rw-r--r--  2.0 unx     2407 b- defN 23-Jun-07 12:02 super_gradients/training/models/classification_models/mobilenet.py
+-rw-r--r--  2.0 unx     9472 b- defN 23-Jun-07 12:02 super_gradients/training/models/classification_models/mobilenetv2.py
+-rw-r--r--  2.0 unx     8696 b- defN 23-Jun-07 12:02 super_gradients/training/models/classification_models/mobilenetv3.py
+-rw-r--r--  2.0 unx     4339 b- defN 23-Jun-07 12:02 super_gradients/training/models/classification_models/pnasnet.py
+-rw-r--r--  2.0 unx     4209 b- defN 23-Jun-07 12:02 super_gradients/training/models/classification_models/preact_resnet.py
+-rw-r--r--  2.0 unx    13599 b- defN 23-Jun-07 12:02 super_gradients/training/models/classification_models/regnet.py
+-rw-r--r--  2.0 unx     7924 b- defN 23-Jun-07 12:02 super_gradients/training/models/classification_models/repvgg.py
+-rw-r--r--  2.0 unx    15067 b- defN 23-Jun-07 12:02 super_gradients/training/models/classification_models/resnet.py
+-rw-r--r--  2.0 unx     6294 b- defN 23-Jun-07 12:02 super_gradients/training/models/classification_models/resnext.py
+-rw-r--r--  2.0 unx     4134 b- defN 23-Jun-07 12:02 super_gradients/training/models/classification_models/senet.py
+-rw-r--r--  2.0 unx     3660 b- defN 23-Jun-07 12:02 super_gradients/training/models/classification_models/shufflenet.py
+-rw-r--r--  2.0 unx     9768 b- defN 23-Jun-07 12:02 super_gradients/training/models/classification_models/shufflenetv2.py
+-rw-r--r--  2.0 unx     1538 b- defN 23-Jun-07 12:02 super_gradients/training/models/classification_models/vgg.py
+-rw-r--r--  2.0 unx     9210 b- defN 23-Jun-07 12:02 super_gradients/training/models/classification_models/vit.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/training/models/detection_models/__init__.py
+-rw-r--r--  2.0 unx     9130 b- defN 23-Jun-07 12:02 super_gradients/training/models/detection_models/csp_darknet53.py
+-rw-r--r--  2.0 unx     9814 b- defN 23-Jun-07 12:02 super_gradients/training/models/detection_models/csp_resnet.py
+-rw-r--r--  2.0 unx     9986 b- defN 23-Jun-07 12:02 super_gradients/training/models/detection_models/customizable_detector.py
+-rw-r--r--  2.0 unx     4746 b- defN 23-Jun-07 12:02 super_gradients/training/models/detection_models/darknet53.py
+-rw-r--r--  2.0 unx     2315 b- defN 23-Jun-07 12:02 super_gradients/training/models/detection_models/ssd.py
+-rw-r--r--  2.0 unx    30262 b- defN 23-Jun-07 12:02 super_gradients/training/models/detection_models/yolo_base.py
+-rw-r--r--  2.0 unx     2459 b- defN 23-Jun-07 12:02 super_gradients/training/models/detection_models/yolox.py
+-rw-r--r--  2.0 unx      251 b- defN 23-Jun-07 12:02 super_gradients/training/models/detection_models/pp_yolo_e/__init__.py
+-rw-r--r--  2.0 unx     7000 b- defN 23-Jun-07 12:02 super_gradients/training/models/detection_models/pp_yolo_e/pan.py
+-rw-r--r--  2.0 unx     3487 b- defN 23-Jun-07 12:02 super_gradients/training/models/detection_models/pp_yolo_e/post_prediction_callback.py
+-rw-r--r--  2.0 unx     9023 b- defN 23-Jun-07 12:02 super_gradients/training/models/detection_models/pp_yolo_e/pp_yolo_e.py
+-rw-r--r--  2.0 unx    12397 b- defN 23-Jun-07 12:02 super_gradients/training/models/detection_models/pp_yolo_e/pp_yolo_head.py
+-rw-r--r--  2.0 unx      756 b- defN 23-Jun-07 12:02 super_gradients/training/models/detection_models/yolo_nas/__init__.py
+-rw-r--r--  2.0 unx    12084 b- defN 23-Jun-07 12:02 super_gradients/training/models/detection_models/yolo_nas/dfl_heads.py
+-rw-r--r--  2.0 unx     2646 b- defN 23-Jun-07 12:02 super_gradients/training/models/detection_models/yolo_nas/panneck.py
+-rw-r--r--  2.0 unx     4166 b- defN 23-Jun-07 12:02 super_gradients/training/models/detection_models/yolo_nas/yolo_nas_variants.py
+-rw-r--r--  2.0 unx    13329 b- defN 23-Jun-07 12:02 super_gradients/training/models/detection_models/yolo_nas/yolo_stages.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/training/models/kd_modules/__init__.py
+-rw-r--r--  2.0 unx     3553 b- defN 23-Jun-07 12:02 super_gradients/training/models/kd_modules/kd_module.py
+-rw-r--r--  2.0 unx      179 b- defN 23-Jun-07 12:02 super_gradients/training/models/pose_estimation_models/__init__.py
+-rw-r--r--  2.0 unx    23096 b- defN 23-Jun-07 12:02 super_gradients/training/models/pose_estimation_models/dekr_hrnet.py
+-rw-r--r--  2.0 unx     4298 b- defN 23-Jun-07 12:02 super_gradients/training/models/pose_estimation_models/rescoring_net.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/training/models/segmentation_models/__init__.py
+-rw-r--r--  2.0 unx      964 b- defN 23-Jun-07 12:02 super_gradients/training/models/segmentation_models/common.py
+-rw-r--r--  2.0 unx     5139 b- defN 23-Jun-07 12:02 super_gradients/training/models/segmentation_models/context_modules.py
+-rw-r--r--  2.0 unx    28514 b- defN 23-Jun-07 12:02 super_gradients/training/models/segmentation_models/ddrnet.py
+-rw-r--r--  2.0 unx     2439 b- defN 23-Jun-07 12:02 super_gradients/training/models/segmentation_models/ddrnet_backbones.py
+-rw-r--r--  2.0 unx    21760 b- defN 23-Jun-07 12:02 super_gradients/training/models/segmentation_models/laddernet.py
+-rw-r--r--  2.0 unx    15648 b- defN 23-Jun-07 12:02 super_gradients/training/models/segmentation_models/ppliteseg.py
+-rw-r--r--  2.0 unx    14424 b- defN 23-Jun-07 12:02 super_gradients/training/models/segmentation_models/regseg.py
+-rw-r--r--  2.0 unx    20334 b- defN 23-Jun-07 12:02 super_gradients/training/models/segmentation_models/segformer.py
+-rw-r--r--  2.0 unx     2256 b- defN 23-Jun-07 12:02 super_gradients/training/models/segmentation_models/segmentation_module.py
+-rw-r--r--  2.0 unx    24851 b- defN 23-Jun-07 12:02 super_gradients/training/models/segmentation_models/shelfnet.py
+-rw-r--r--  2.0 unx    29091 b- defN 23-Jun-07 12:02 super_gradients/training/models/segmentation_models/stdc.py
+-rw-r--r--  2.0 unx      260 b- defN 23-Jun-07 12:02 super_gradients/training/models/segmentation_models/unet/__init__.py
+-rw-r--r--  2.0 unx    12324 b- defN 23-Jun-07 12:02 super_gradients/training/models/segmentation_models/unet/unet.py
+-rw-r--r--  2.0 unx    10718 b- defN 23-Jun-07 12:02 super_gradients/training/models/segmentation_models/unet/unet_decoder.py
+-rw-r--r--  2.0 unx    13292 b- defN 23-Jun-07 12:02 super_gradients/training/models/segmentation_models/unet/unet_encoder.py
+-rw-r--r--  2.0 unx      119 b- defN 23-Jun-07 12:02 super_gradients/training/models/user_models/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/training/pipelines/__init__.py
+-rw-r--r--  2.0 unx    15639 b- defN 23-Jun-07 12:02 super_gradients/training/pipelines/pipelines.py
+-rw-r--r--  2.0 unx      445 b- defN 23-Jun-07 12:02 super_gradients/training/pre_launch_callbacks/__init__.py
+-rw-r--r--  2.0 unx    21020 b- defN 23-Jun-07 12:02 super_gradients/training/pre_launch_callbacks/pre_launch_callbacks.py
+-rw-r--r--  2.0 unx      517 b- defN 23-Jun-07 12:02 super_gradients/training/processing/__init__.py
+-rw-r--r--  2.0 unx    13177 b- defN 23-Jun-07 12:02 super_gradients/training/processing/processing.py
+-rw-r--r--  2.0 unx       98 b- defN 23-Jun-07 12:02 super_gradients/training/qat_trainer/__init__.py
+-rw-r--r--  2.0 unx      608 b- defN 23-Jun-07 12:02 super_gradients/training/qat_trainer/qat_trainer.py
+-rw-r--r--  2.0 unx      184 b- defN 23-Jun-07 12:02 super_gradients/training/sg_trainer/__init__.py
+-rw-r--r--  2.0 unx   116430 b- defN 23-Jun-07 12:02 super_gradients/training/sg_trainer/sg_trainer.py
+-rw-r--r--  2.0 unx     1685 b- defN 23-Jun-07 12:02 super_gradients/training/training_hyperparams/__init__.py
+-rw-r--r--  2.0 unx     3774 b- defN 23-Jun-07 12:02 super_gradients/training/training_hyperparams/training_hyperparams.py
+-rw-r--r--  2.0 unx     1024 b- defN 23-Jun-07 12:02 super_gradients/training/transforms/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/training/transforms/all_transforms.py
+-rw-r--r--  2.0 unx    16193 b- defN 23-Jun-07 12:02 super_gradients/training/transforms/keypoint_transforms.py
+-rw-r--r--  2.0 unx     1134 b- defN 23-Jun-07 12:02 super_gradients/training/transforms/pipeline_adaptors.py
+-rw-r--r--  2.0 unx    55587 b- defN 23-Jun-07 12:02 super_gradients/training/transforms/transforms.py
+-rw-r--r--  2.0 unx     6048 b- defN 23-Jun-07 12:02 super_gradients/training/transforms/utils.py
+-rw-r--r--  2.0 unx     1179 b- defN 23-Jun-07 12:02 super_gradients/training/utils/__init__.py
+-rw-r--r--  2.0 unx     1673 b- defN 23-Jun-07 12:02 super_gradients/training/utils/activations_utils.py
+-rw-r--r--  2.0 unx     1111 b- defN 23-Jun-07 12:02 super_gradients/training/utils/bbox_utils.py
+-rw-r--r--  2.0 unx    15712 b- defN 23-Jun-07 12:02 super_gradients/training/utils/checkpoint_utils.py
+-rw-r--r--  2.0 unx     9794 b- defN 23-Jun-07 12:02 super_gradients/training/utils/config_utils.py
+-rw-r--r--  2.0 unx     1132 b- defN 23-Jun-07 12:02 super_gradients/training/utils/deprecated_utils.py
+-rw-r--r--  2.0 unx    53289 b- defN 23-Jun-07 12:02 super_gradients/training/utils/detection_utils.py
+-rw-r--r--  2.0 unx    16195 b- defN 23-Jun-07 12:02 super_gradients/training/utils/distributed_training_utils.py
+-rw-r--r--  2.0 unx     6352 b- defN 23-Jun-07 12:02 super_gradients/training/utils/early_stopping.py
+-rw-r--r--  2.0 unx     9322 b- defN 23-Jun-07 12:02 super_gradients/training/utils/ema.py
+-rw-r--r--  2.0 unx     2610 b- defN 23-Jun-07 12:02 super_gradients/training/utils/ema_decay_schedules.py
+-rw-r--r--  2.0 unx     1072 b- defN 23-Jun-07 12:02 super_gradients/training/utils/export_utils.py
+-rw-r--r--  2.0 unx     7508 b- defN 23-Jun-07 12:02 super_gradients/training/utils/get_model_stats.py
+-rw-r--r--  2.0 unx      771 b- defN 23-Jun-07 12:02 super_gradients/training/utils/kd_trainer_utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/training/utils/load_image.py
+-rw-r--r--  2.0 unx     5827 b- defN 23-Jun-07 12:02 super_gradients/training/utils/optimizer_utils.py
+-rw-r--r--  2.0 unx      839 b- defN 23-Jun-07 12:02 super_gradients/training/utils/regularization_utils.py
+-rw-r--r--  2.0 unx    10388 b- defN 23-Jun-07 12:02 super_gradients/training/utils/segmentation_utils.py
+-rw-r--r--  2.0 unx    19625 b- defN 23-Jun-07 12:02 super_gradients/training/utils/sg_trainer_utils.py
+-rw-r--r--  2.0 unx     6272 b- defN 23-Jun-07 12:02 super_gradients/training/utils/ssd_utils.py
+-rw-r--r--  2.0 unx    20438 b- defN 23-Jun-07 12:02 super_gradients/training/utils/utils.py
+-rw-r--r--  2.0 unx      303 b- defN 23-Jun-07 12:02 super_gradients/training/utils/version_utils.py
+-rw-r--r--  2.0 unx     5687 b- defN 23-Jun-07 12:02 super_gradients/training/utils/weight_averaging_utils.py
+-rw-r--r--  2.0 unx     2030 b- defN 23-Jun-07 12:02 super_gradients/training/utils/callbacks/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/training/utils/callbacks/all_callbacks.py
+-rw-r--r--  2.0 unx    20126 b- defN 23-Jun-07 12:02 super_gradients/training/utils/callbacks/base_callbacks.py
+-rw-r--r--  2.0 unx    33409 b- defN 23-Jun-07 12:02 super_gradients/training/utils/callbacks/callbacks.py
+-rw-r--r--  2.0 unx     1169 b- defN 23-Jun-07 12:02 super_gradients/training/utils/callbacks/ppyoloe_switch_callback.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/training/utils/media/__init__.py
+-rw-r--r--  2.0 unx     5880 b- defN 23-Jun-07 12:02 super_gradients/training/utils/media/image.py
+-rw-r--r--  2.0 unx     4046 b- defN 23-Jun-07 12:02 super_gradients/training/utils/media/stream.py
+-rw-r--r--  2.0 unx     6926 b- defN 23-Jun-07 12:02 super_gradients/training/utils/media/video.py
+-rw-r--r--  2.0 unx      396 b- defN 23-Jun-07 12:02 super_gradients/training/utils/optimizers/__init__.py
+-rw-r--r--  2.0 unx      422 b- defN 23-Jun-07 12:02 super_gradients/training/utils/optimizers/all_optimizers.py
+-rw-r--r--  2.0 unx     9760 b- defN 23-Jun-07 12:02 super_gradients/training/utils/optimizers/lamb.py
+-rw-r--r--  2.0 unx     3008 b- defN 23-Jun-07 12:02 super_gradients/training/utils/optimizers/lion.py
+-rw-r--r--  2.0 unx     6834 b- defN 23-Jun-07 12:02 super_gradients/training/utils/optimizers/rmsprop_tf.py
+-rw-r--r--  2.0 unx      324 b- defN 23-Jun-07 12:02 super_gradients/training/utils/pose_estimation/__init__.py
+-rw-r--r--  2.0 unx    11309 b- defN 23-Jun-07 12:02 super_gradients/training/utils/pose_estimation/dekr_decode_callbacks.py
+-rw-r--r--  2.0 unx     7140 b- defN 23-Jun-07 12:02 super_gradients/training/utils/pose_estimation/dekr_visualization_callbacks.py
+-rw-r--r--  2.0 unx      920 b- defN 23-Jun-07 12:02 super_gradients/training/utils/pose_estimation/rescoring_callback.py
+-rw-r--r--  2.0 unx      387 b- defN 23-Jun-07 12:02 super_gradients/training/utils/quantization/__init__.py
+-rw-r--r--  2.0 unx     6271 b- defN 23-Jun-07 12:02 super_gradients/training/utils/quantization/calibrator.py
+-rw-r--r--  2.0 unx     8417 b- defN 23-Jun-07 12:02 super_gradients/training/utils/quantization/core.py
+-rw-r--r--  2.0 unx     2504 b- defN 23-Jun-07 12:02 super_gradients/training/utils/quantization/export.py
+-rw-r--r--  2.0 unx    17062 b- defN 23-Jun-07 12:02 super_gradients/training/utils/quantization/selective_quantization_utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 12:02 super_gradients/training/utils/visualization/__init__.py
+-rw-r--r--  2.0 unx     1698 b- defN 23-Jun-07 12:02 super_gradients/training/utils/visualization/detection.py
+-rw-r--r--  2.0 unx     2847 b- defN 23-Jun-07 12:02 super_gradients/training/utils/visualization/utils.py
+-rw-r--r--  2.0 unx     2218 b- defN 23-Jun-07 12:03 super_gradients-3.1.2.dist-info/LICENSE.YOLONAS.md
+-rw-r--r--  2.0 unx    11341 b- defN 23-Jun-07 12:03 super_gradients-3.1.2.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx    35552 b- defN 23-Jun-07 12:03 super_gradients-3.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-07 12:03 super_gradients-3.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-07 12:03 super_gradients-3.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    65481 b- defN 23-Jun-07 12:03 super_gradients-3.1.2.dist-info/RECORD
+567 files, 2880515 bytes uncompressed, 873153 bytes compressed:  69.7%
```

## zipnote {}

```diff
@@ -264,14 +264,20 @@
 
 Filename: super_gradients/common/plugins/__init__.py
 Comment: 
 
 Filename: super_gradients/common/plugins/deci_client.py
 Comment: 
 
+Filename: super_gradients/common/plugins/wandb/__init__.py
+Comment: 
+
+Filename: super_gradients/common/plugins/wandb/log_predictions.py
+Comment: 
+
 Filename: super_gradients/common/registry/__init__.py
 Comment: 
 
 Filename: super_gradients/common/registry/albumentation.py
 Comment: 
 
 Filename: super_gradients/common/registry/registry.py
@@ -507,14 +513,17 @@
 
 Filename: super_gradients/recipes/__init__.py
 Comment: 
 
 Filename: super_gradients/recipes/cifar10_resnet.yaml
 Comment: 
 
+Filename: super_gradients/recipes/cityscapes_al_ddrnet.yaml
+Comment: 
+
 Filename: super_gradients/recipes/cityscapes_ddrnet.yaml
 Comment: 
 
 Filename: super_gradients/recipes/cityscapes_kd_base.yaml
 Comment: 
 
 Filename: super_gradients/recipes/cityscapes_pplite_seg50.yaml
@@ -534,23 +543,20 @@
 
 Filename: super_gradients/recipes/cityscapes_stdc_seg50.yaml
 Comment: 
 
 Filename: super_gradients/recipes/cityscapes_stdc_seg75.yaml
 Comment: 
 
-Filename: super_gradients/recipes/coco2017_pose_ddrnet39.yaml
+Filename: super_gradients/recipes/coco2017_pose_dekr_rescoring.yaml
 Comment: 
 
 Filename: super_gradients/recipes/coco2017_pose_dekr_w32_no_dc.yaml
 Comment: 
 
-Filename: super_gradients/recipes/coco2017_pose_pppose_l.yaml
-Comment: 
-
 Filename: super_gradients/recipes/coco2017_ppyoloe_l.yaml
 Comment: 
 
 Filename: super_gradients/recipes/coco2017_ppyoloe_m.yaml
 Comment: 
 
 Filename: super_gradients/recipes/coco2017_ppyoloe_s.yaml
@@ -615,14 +621,17 @@
 
 Filename: super_gradients/recipes/roboflow_yolo_nas_s_qat.yaml
 Comment: 
 
 Filename: super_gradients/recipes/roboflow_yolox.yaml
 Comment: 
 
+Filename: super_gradients/recipes/script_generate_rescoring_data_dekr_coco2017.yaml
+Comment: 
+
 Filename: super_gradients/recipes/supervisely_unet.yaml
 Comment: 
 
 Filename: super_gradients/recipes/user_recipe_mnist_as_external_dataset_example.yaml
 Comment: 
 
 Filename: super_gradients/recipes/user_recipe_mnist_example.yaml
@@ -675,15 +684,15 @@
 
 Filename: super_gradients/recipes/arch_params/mobilenet_v3_large_arch_params.yaml
 Comment: 
 
 Filename: super_gradients/recipes/arch_params/mobilenet_v3_small_arch_params.yaml
 Comment: 
 
-Filename: super_gradients/recipes/arch_params/pose_ddrnet39_arch_params.yaml
+Filename: super_gradients/recipes/arch_params/pose_dekr_coco_rescoring_arch_params.yaml
 Comment: 
 
 Filename: super_gradients/recipes/arch_params/pose_dekr_w32_no_dc_arch_params.yaml
 Comment: 
 
 Filename: super_gradients/recipes/arch_params/pose_pppose_l_arch_params.yaml
 Comment: 
@@ -801,14 +810,17 @@
 
 Filename: super_gradients/recipes/dataset_params/cifar10_albumentations_dataset_params.yaml
 Comment: 
 
 Filename: super_gradients/recipes/dataset_params/cifar10_dataset_params.yaml
 Comment: 
 
+Filename: super_gradients/recipes/dataset_params/cityscapes_al_dataset_params.yaml
+Comment: 
+
 Filename: super_gradients/recipes/dataset_params/cityscapes_dataset_params.yaml
 Comment: 
 
 Filename: super_gradients/recipes/dataset_params/cityscapes_ddrnet_dataset_params.yaml
 Comment: 
 
 Filename: super_gradients/recipes/dataset_params/cityscapes_ppliteseg_seg75_dataset_params.yaml
@@ -843,14 +855,17 @@
 
 Filename: super_gradients/recipes/dataset_params/coco_pose_estimation_dataset_params.yaml
 Comment: 
 
 Filename: super_gradients/recipes/dataset_params/coco_pose_estimation_dekr_dataset_params.yaml
 Comment: 
 
+Filename: super_gradients/recipes/dataset_params/coco_pose_estimation_rescoring_dataset_params.yaml
+Comment: 
+
 Filename: super_gradients/recipes/dataset_params/coco_segmentation_dataset_params.yaml
 Comment: 
 
 Filename: super_gradients/recipes/dataset_params/imagenet_dataset_params.yaml
 Comment: 
 
 Filename: super_gradients/recipes/dataset_params/imagenet_efficientnet_dataset_params.yaml
@@ -906,14 +921,17 @@
 
 Filename: super_gradients/recipes/training_hyperparams/coco2017_dekr_pose_train_params.yaml
 Comment: 
 
 Filename: super_gradients/recipes/training_hyperparams/coco2017_ppyoloe_train_params.yaml
 Comment: 
 
+Filename: super_gradients/recipes/training_hyperparams/coco2017_rescoring_train_params.yaml
+Comment: 
+
 Filename: super_gradients/recipes/training_hyperparams/coco2017_ssd_lite_mobilenet_v2_train_params.yaml
 Comment: 
 
 Filename: super_gradients/recipes/training_hyperparams/coco2017_yolo_nas_train_params.yaml
 Comment: 
 
 Filename: super_gradients/recipes/training_hyperparams/coco2017_yolox_train_params.yaml
@@ -1086,20 +1104,26 @@
 
 Filename: super_gradients/training/datasets/pose_estimation_datasets/coco_keypoints.py
 Comment: 
 
 Filename: super_gradients/training/datasets/pose_estimation_datasets/coco_utils.py
 Comment: 
 
+Filename: super_gradients/training/datasets/pose_estimation_datasets/rescoring_dataset.py
+Comment: 
+
 Filename: super_gradients/training/datasets/pose_estimation_datasets/target_generators.py
 Comment: 
 
 Filename: super_gradients/training/datasets/samplers/__init__.py
 Comment: 
 
+Filename: super_gradients/training/datasets/samplers/infinite_sampler.py
+Comment: 
+
 Filename: super_gradients/training/datasets/samplers/repeated_augmentation_sampler.py
 Comment: 
 
 Filename: super_gradients/training/datasets/segmentation_datasets/__init__.py
 Comment: 
 
 Filename: super_gradients/training/datasets/segmentation_datasets/cityscape_segmentation.py
@@ -1197,14 +1221,17 @@
 
 Filename: super_gradients/training/losses/ppyolo_loss.py
 Comment: 
 
 Filename: super_gradients/training/losses/r_squared_loss.py
 Comment: 
 
+Filename: super_gradients/training/losses/rescoring_loss.py
+Comment: 
+
 Filename: super_gradients/training/losses/seg_kd_loss.py
 Comment: 
 
 Filename: super_gradients/training/losses/shelfnet_ohem_loss.py
 Comment: 
 
 Filename: super_gradients/training/losses/shelfnet_semantic_encoding_loss.py
@@ -1395,18 +1422,15 @@
 
 Filename: super_gradients/training/models/pose_estimation_models/__init__.py
 Comment: 
 
 Filename: super_gradients/training/models/pose_estimation_models/dekr_hrnet.py
 Comment: 
 
-Filename: super_gradients/training/models/pose_estimation_models/pose_ddrnet39.py
-Comment: 
-
-Filename: super_gradients/training/models/pose_estimation_models/pose_ppyolo.py
+Filename: super_gradients/training/models/pose_estimation_models/rescoring_net.py
 Comment: 
 
 Filename: super_gradients/training/models/segmentation_models/__init__.py
 Comment: 
 
 Filename: super_gradients/training/models/segmentation_models/common.py
 Comment: 
@@ -1605,14 +1629,17 @@
 
 Filename: super_gradients/training/utils/media/video.py
 Comment: 
 
 Filename: super_gradients/training/utils/optimizers/__init__.py
 Comment: 
 
+Filename: super_gradients/training/utils/optimizers/all_optimizers.py
+Comment: 
+
 Filename: super_gradients/training/utils/optimizers/lamb.py
 Comment: 
 
 Filename: super_gradients/training/utils/optimizers/lion.py
 Comment: 
 
 Filename: super_gradients/training/utils/optimizers/rmsprop_tf.py
@@ -1623,14 +1650,17 @@
 
 Filename: super_gradients/training/utils/pose_estimation/dekr_decode_callbacks.py
 Comment: 
 
 Filename: super_gradients/training/utils/pose_estimation/dekr_visualization_callbacks.py
 Comment: 
 
+Filename: super_gradients/training/utils/pose_estimation/rescoring_callback.py
+Comment: 
+
 Filename: super_gradients/training/utils/quantization/__init__.py
 Comment: 
 
 Filename: super_gradients/training/utils/quantization/calibrator.py
 Comment: 
 
 Filename: super_gradients/training/utils/quantization/core.py
@@ -1647,26 +1677,26 @@
 
 Filename: super_gradients/training/utils/visualization/detection.py
 Comment: 
 
 Filename: super_gradients/training/utils/visualization/utils.py
 Comment: 
 
-Filename: super_gradients-3.1.1.dist-info/LICENSE.YOLONAS.md
+Filename: super_gradients-3.1.2.dist-info/LICENSE.YOLONAS.md
 Comment: 
 
-Filename: super_gradients-3.1.1.dist-info/LICENSE.md
+Filename: super_gradients-3.1.2.dist-info/LICENSE.md
 Comment: 
 
-Filename: super_gradients-3.1.1.dist-info/METADATA
+Filename: super_gradients-3.1.2.dist-info/METADATA
 Comment: 
 
-Filename: super_gradients-3.1.1.dist-info/WHEEL
+Filename: super_gradients-3.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: super_gradients-3.1.1.dist-info/top_level.txt
+Filename: super_gradients-3.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: super_gradients-3.1.1.dist-info/RECORD
+Filename: super_gradients-3.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## super_gradients/__init__.py

```diff
@@ -1,12 +1,13 @@
 from super_gradients.common import init_trainer, is_distributed, object_names
 from super_gradients.training import losses, utils, datasets_utils, DataAugmentation, Trainer, KDTrainer, QATTrainer
 from super_gradients.common.registry.registry import ARCHITECTURES
 from super_gradients.sanity_check import env_sanity_check
 from super_gradients.training.utils.distributed_training_utils import setup_device
+from super_gradients.training.pre_launch_callbacks import AutoTrainBatchSizeSelectionCallback, QATRecipeModificationCallback
 
 __all__ = [
     "ARCHITECTURES",
     "losses",
     "utils",
     "datasets_utils",
     "DataAugmentation",
@@ -14,12 +15,14 @@
     "KDTrainer",
     "QATTrainer",
     "object_names",
     "init_trainer",
     "is_distributed",
     "env_sanity_check",
     "setup_device",
+    "QATRecipeModificationCallback",
+    "AutoTrainBatchSizeSelectionCallback",
 ]
 
-__version__ = "3.1.1"
+__version__ = "3.1.2"
 
 env_sanity_check()
```

## super_gradients/qat_from_recipe.py

```diff
@@ -4,21 +4,20 @@
 General use: python -m super_gradients.qat_from_recipe --config-name="DESIRED_RECIPE".
 For recipe's specific instructions and details refer to the recipe's configuration file in the recipes directory.
 """
 
 import hydra
 from omegaconf import DictConfig
 
-from super_gradients import init_trainer
-from super_gradients.training.qat_trainer.qat_trainer import QATTrainer
+from super_gradients import init_trainer, Trainer
 
 
 @hydra.main(config_path="recipes", version_base="1.2")
 def _main(cfg: DictConfig) -> None:
-    QATTrainer.train_from_config(cfg)
+    Trainer.quantize_from_config(cfg)
 
 
 def main():
     init_trainer()  # `init_trainer` needs to be called before `@hydra.main`
     _main()
```

## super_gradients/requirements.pro.txt

```diff
@@ -1,2 +1 @@
-deci-lab-client==4.17.0
-deci-common==3.15.0
+deci-platform-client>=5.0.0
```

## super_gradients/requirements.txt

```diff
@@ -1,8 +1,8 @@
-torch>=1.9.0,<1.14
+torch>=1.9.0
 tqdm>=4.57.0
 boto3>=1.17.15
 jsonschema>=3.2.0
 Deprecated>=1.2.11
 opencv-python>=4.5.1
 scipy>=1.6.1
 matplotlib>=3.3.4
@@ -10,23 +10,23 @@
 tensorboard>=2.4.1
 setuptools>=21.0.0
 coverage~=5.3.1
 torchvision>=0.10.0
 sphinx~=4.0.2
 sphinx-rtd-theme
 torchmetrics==0.8
-pillow>=9.2.0
 hydra-core>=1.2.0
 omegaconf
 onnxruntime==1.13.1
 onnx==1.13.0
+pillow>=5.3.0,!=8.3
 pip-tools>=6.12.1
 pyparsing==2.4.5
 einops==0.3.2
-pycocotools==2.0.4
+pycocotools==2.0.6
 protobuf==3.20.3
 treelib==1.6.1
 termcolor==1.1.0
 packaging>=20.4
 # not directly required, pinned by Snyk to avoid a vulnerability
 wheel>=0.38.0
 # not directly required, pinned by Snyk to avoid a vulnerability
```

## super_gradients/common/object_names.py

```diff
@@ -11,14 +11,15 @@
     YOLOX_FAST_LOSS = "yolox_fast_loss"
     SSD_LOSS = "ssd_loss"
     STDC_LOSS = "stdc_loss"
     BCE_DICE_LOSS = "bce_dice_loss"
     KD_LOSS = "kd_loss"
     DICE_CE_EDGE_LOSS = "dice_ce_edge_loss"
     DEKR_LOSS = "dekr_loss"
+    RESCORING_LOSS = "rescoring_loss"
 
 
 class Metrics:
     """Static class holding all the supported metric names"""
 
     ACCURACY = "Accuracy"
     TOP5 = "Top5"
@@ -297,19 +298,19 @@
     SEGFORMER_B2 = "segformer_b2"
     SEGFORMER_B3 = "segformer_b3"
     SEGFORMER_B4 = "segformer_b4"
     SEGFORMER_B5 = "segformer_b5"
 
     DEKR_CUSTOM = "dekr_custom"
     DEKR_W32_NO_DC = "dekr_w32_no_dc"
-    POSE_PP_YOLO_L = "pose_ppyolo_l"
-    POSE_DDRNET_39 = "pose_ddrnet39"
     YOLO_NAS_S = "yolo_nas_s"
     YOLO_NAS_M = "yolo_nas_m"
     YOLO_NAS_L = "yolo_nas_l"
+    POSE_RESCORING = "pose_rescoring_custom"
+    POSE_RESCORING_COCO = "pose_rescoring_coco"
 
 
 class ConcatenatedTensorFormats:
     XYXY_LABEL = "XYXY_LABEL"
     XYWH_LABEL = "XYWH_LABEL"
     CXCYWH_LABEL = "CXCYWH_LABEL"
     LABEL_XYXY = "LABEL_XYXY"
@@ -334,14 +335,16 @@
     COCO2017_VAL_PPYOLOE = "coco2017_val_ppyoloe"
     COCO2017_TRAIN_SSD_LITE_MOBILENET_V2 = "coco2017_train_ssd_lite_mobilenet_v2"
     COCO2017_VAL_SSD_LITE_MOBILENET_V2 = "coco2017_val_ssd_lite_mobilenet_v2"
     COCO2017_POSE_TRAIN = "coco2017_pose_train"
     COCO2017_POSE_VAL = "coco2017_pose_val"
     COCO_DETECTION_YOLO_FORMAT_TRAIN = "coco_detection_yolo_format_train"
     COCO_DETECTION_YOLO_FORMAT_VAL = "coco_detection_yolo_format_val"
+    COCO2017_RESCORING_TRAIN = "coco2017_rescoring_train"
+    COCO2017_RESCORING_VAL = "coco2017_rescoring_val"
     IMAGENET_TRAIN = "imagenet_train"
     IMAGENET_VAL = "imagenet_val"
     IMAGENET_EFFICIENTNET_TRAIN = "imagenet_efficientnet_train"
     IMAGENET_EFFICIENTNET_VAL = "imagenet_efficientnet_val"
     IMAGENET_MOBILENETV2_TRAIN = "imagenet_mobilenetv2_train"
     IMAGENET_MOBILENETV2_VAL = "imagenet_mobilenetv2_val"
     IMAGENET_MOBILENETV3_TRAIN = "imagenet_mobilenetv3_train"
@@ -394,14 +397,15 @@
     DETECTION_DATASET = "DetectionDataset"
     PASCAL_VOC_DETECTION_DATASET = "PascalVOCDetectionDataset"
     SEGMENTATION_DATASET = "SegmentationDataSet"
     COCO_SEGMENTATION_DATASET = "CoCoSegmentationDataSet"
     PASCAL_AUG_2012_SEGMENTATION_DATASET = "PascalAUG2012SegmentationDataSet"
     PASCAL_VOC_2012_SEGMENTATION_DATASET = "PascalVOC2012SegmentationDataSet"
     CITYSCAPES_DATASET = "CityscapesDataset"
+    CITYSCAPES_CONCAT_DATASET = "CityscapesConcatDataset"
     MAPILLARY_DATASET = "MapillaryDataset"
     SUPERVISELY_PERSONS_DATASET = "SuperviselyPersonsDataset"
     PASCAL_VOC_AND_AUG_UNIFIED_DATASET = "PascalVOCAndAUGUnifiedDataset"
     COCO_KEY_POINTS_DATASET = "COCOKeypointsDataset"
 
 
 class Processings:
```

## super_gradients/common/crash_handler/exception_monitoring_setup.py

```diff
@@ -28,16 +28,18 @@
 
 
 @multi_process_safe
 def setup_pro_user_monitoring() -> bool:
     """Setup the pro user environment for error logging and monitoring"""
     if client_enabled:
         if env_variables.UPLOAD_LOGS:
-            logger.info("deci-lab-client package detected. activating automatic log uploading")
-            logger.info("If you do not have a deci-lab-client credentials or you wish to disable this feature, please set the env variable UPLOAD_LOGS=FALSE")
+            logger.info("deci-platform-client package detected. activating automatic log uploading")
+            logger.info(
+                "If you do not have a deci-platform-client credentials or you wish to disable this feature, please set the env variable UPLOAD_LOGS=FALSE"
+            )
 
             # This prevents hydra.main to catch errors that happen in the decorated function
             # (which leads sys.excepthook to never be called)
             os.environ["HYDRA_FULL_ERROR"] = "1"
 
             logger.info("Connecting to the deci platform ...")
             platform_client = DeciClient()
```

## super_gradients/common/environment/checkpoints_dir_utils.py

```diff
@@ -54,29 +54,33 @@
     """
     ckpt_root_dir = ckpt_root_dir or PKG_CHECKPOINTS_DIR or get_project_checkpoints_dir_path()
     if ckpt_root_dir is None:
         raise ValueError("Illegal checkpoints directory: please set ckpt_root_dir")
     return os.path.join(ckpt_root_dir, experiment_name)
 
 
-def get_ckpt_local_path(source_ckpt_folder_name: str, experiment_name: str, ckpt_name: str, external_checkpoint_path: str):
+def get_ckpt_local_path(experiment_name: str, ckpt_name: str, external_checkpoint_path: str, ckpt_root_dir: str = None) -> str:
     """
     Gets the local path to the checkpoint file, which will be:
-        - By default: YOUR_REPO_ROOT/super_gradients/checkpoints/experiment_name.
+        - By default: YOUR_REPO_ROOT/super_gradients/checkpoints/experiment_name/ckpt_name.
+        - external_checkpoint_path when external_checkpoint_path != None
+        - ckpt_root_dir/experiment_name/ckpt_name when ckpt_root_dir != None.
         - if the checkpoint file is remotely located:
             when overwrite_local_checkpoint=True then it will be saved in a temporary path which will be returned,
             otherwise it will be downloaded to YOUR_REPO_ROOT/super_gradients/checkpoints/experiment_name and overwrite
             YOUR_REPO_ROOT/super_gradients/checkpoints/experiment_name/ckpt_name if such file exists.
-        - external_checkpoint_path when external_checkpoint_path != None
 
-    :param source_ckpt_folder_name: The folder where the checkpoint is saved. When set to None- uses the experiment_name.
-    :param experiment_name: experiment name attr in trainer
-    :param ckpt_name: checkpoint filename
-    :param external_checkpoint_path: full path to checkpoint file (that might be located outside of super_gradients/checkpoints directory)
-    :return:
+
+    :param experiment_name: experiment name attr in trainer :param ckpt_name: checkpoint filename
+    :param external_checkpoint_path: full path to checkpoint file (that might be located outside of
+    super_gradients/checkpoints directory)
+    :param ckpt_root_dir: Local root directory path where all experiment
+     logging directories will reside. When None, it is assumed that pkg_resources.resource_filename(
+    'checkpoints', "") exists and will be used.
+
+     :return: local path of the checkpoint file (Str)
     """
     if external_checkpoint_path:
         return external_checkpoint_path
     else:
-        checkpoints_folder_name = source_ckpt_folder_name or experiment_name
-        checkpoints_dir_path = get_checkpoints_dir_path(checkpoints_folder_name)
+        checkpoints_dir_path = get_checkpoints_dir_path(experiment_name, ckpt_root_dir)
         return os.path.join(checkpoints_dir_path, ckpt_name)
```

## super_gradients/common/environment/env_variables.py

```diff
@@ -1,17 +1,14 @@
 import os
 
 
 class EnvironmentVariables:
     """Class to dynamically get any environment variables."""
 
     # Infra
-    @property
-    def DECI_PLATFORM_TOKEN(self) -> str:
-        return os.getenv("DECI_PLATFORM_TOKEN")
 
     @property
     def WANDB_BASE_URL(self) -> str:
         return os.getenv("WANDB_BASE_URL")
 
     @property
     def AWS_PROFILE(self) -> str:
@@ -28,18 +25,14 @@
         return os.getenv("CRASH_HANDLER", "TRUE")
 
     @property
     def UPLOAD_LOGS(self) -> bool:
         return os.getenv("UPLOAD_LOGS", "TRUE") == "TRUE"
 
     @property
-    def DECI_API_HOST(self) -> str:
-        return os.getenv("DECI_API_HOST", default="api.deci.ai")
-
-    @property
     def FILE_LOG_LEVEL(self) -> str:
         return os.getenv("FILE_LOG_LEVEL", default="DEBUG").upper()
 
     @property
     def CONSOLE_LOG_LEVEL(self) -> str:
         return os.getenv("CONSOLE_LOG_LEVEL", default="INFO").upper()
```

## super_gradients/common/plugins/deci_client.py

```diff
@@ -1,80 +1,121 @@
 import os
 import json
 import sys
 import shutil
+import urllib
 from zipfile import ZipFile
-from typing import List, Optional, Any
+import socket
+import urllib.error
+from urllib.request import urlretrieve
+from typing import List, Optional, Sequence
 
 import importlib.util
+
+import torch.hub
 from omegaconf import DictConfig
 from torch import nn
 
 import super_gradients
-from super_gradients.common.environment.env_variables import env_variables
 from super_gradients.common.abstractions.abstract_logger import get_logger
 from super_gradients.common.environment.cfg_utils import load_arch_params, load_recipe
+from super_gradients.common.environment.path_utils import normalize_path
 
 logger = get_logger(__name__)
 
 client_enabled = True
 try:
-    from deci_lab_client.client import DeciPlatformClient
-    from deci_lab_client.types import S3SignedUrl
-    from deci_lab_client.models import ModelBenchmarkState
-    from deci_common.data_interfaces.files_data_interface import FilesDataInterface
-    from deci_lab_client.models import AutoNACFileName
-    from deci_lab_client import ApiException, BodyRegisterUserArchitecture
+    from deci_platform_client import DeciPlatformClient
+    from deci_platform_client.types import S3SignedUrl
+    from deci_platform_client.models import (
+        ModelBenchmarkState,
+        SentryLevel,
+        FrameworkType,
+        HardwareType,
+        QuantizationLevel,
+    )
+    from deci_common.data_interfaces.files_data_interface import FileDownloadFailedException
+    from deci_platform_client.models import AutoNACFileName
+    from deci_platform_client.exceptions import ApiException, ApiTypeError
 
 except (ImportError, NameError):
     client_enabled = False
 
+DOWNLOAD_MODEL_TIMEOUT_SECONDS = 5 * 60
+
 
 class DeciClient:
     """
     A client to deci platform and model zoo.
     requires credentials for connection
     """
 
     def __init__(self):
         if not client_enabled:
             logger.error(
-                "deci-lab-client or deci-common are not installed. Model cannot be loaded from deci lab."
-                "Please install deci-lab-client>=2.55.0 and deci-common>=3.4.1"
+                "deci-platform-client or deci-common are not installed. Model cannot be loaded from deci lab."
+                "Please install deci-platform-client>=5.0.0 and deci-common>=12.0.0"
             )
             return
 
-        self.api_host = env_variables.DECI_API_HOST
-        self.lab_client = DeciPlatformClient(api_host=self.api_host)
-        self.lab_client.login(token=env_variables.DECI_PLATFORM_TOKEN)
+        self.lab_client = DeciPlatformClient()
 
-    def _get_file(self, model_name: str, file_name: str) -> Optional[str]:
+    def _get_file(self, model_name: str, file_name: "AutoNACFileName") -> Optional[str]:
         """Get a file from the DeciPlatform if it exists, otherwise returns None
         :param model_name:      Name of the model to download from, as saved in the platform.
         :param file_name:       Name of the file to download
         :return:            Path were the downloaded file was saved to. None if not found.
         """
         try:
-            response = self.lab_client.get_autonac_model_file_link(
-                model_name=model_name, file_name=file_name, super_gradients_version=super_gradients.__version__
+            download_link, etag = self.lab_client.get_autonac_model_file_link(
+                model_name=model_name,
+                file_name=file_name,
+                super_gradients_version=super_gradients.__version__,
             )
-            download_link = response.data
         except ApiException as e:
             if e.status == 401:
                 logger.error(
-                    "Unauthorized. wrong token or token was not defined. please login to deci-lab-client " "by calling DeciPlatformClient().login(<token>)"
+                    "Unauthorized. wrong credentials or credentials not defined. "
+                    "Please provide credentials via environment variables (DECI_CLIENT_ID, DECI_CLIENT_SECRET)"
                 )
             elif e.status == 400 and e.body is not None and "message" in e.body:
                 logger.error(f"Deci client: {json.loads(e.body)['message']}")
             else:
                 logger.debug(e.body)
             return None
+        cache_dir = os.path.join(torch.hub.get_dir(), "deci")
+        file_path = os.path.join(cache_dir, etag or "", os.path.basename(file_name))
+        file_path = normalize_path(file_path)
+
+        os.makedirs(os.path.dirname(file_path), exist_ok=True)
+        if os.path.isfile(file_path):
+            return file_path
+
+        file_path = self._download_file_to_cache_dir(
+            file_url=download_link,
+            file_path=file_path,
+        )
+        return file_path
 
-        file_path = FilesDataInterface.download_temporary_file(file_url=download_link)
-
+    def _download_file_to_cache_dir(self, file_url: str, file_path: str, timeout_seconds: Optional[int] = DOWNLOAD_MODEL_TIMEOUT_SECONDS):
+        """
+        Download a file from a url to a cache dir. The file will be saved in a subfolder named by the etag.
+        This allow us to save multiple versions of the same file and cache them, so when a file with the same etag is
+        requested, we can return the cached file.
+
+        :param file_url:  Url to download the file from.
+        :param file_path: Path to save the file to.
+        :return:        Path were the downloaded file was saved to. (same as file_path)
+        """
+        # TODO: Use requests with stream and limit the file size and timeouts.
+        socket.setdefaulttimeout(timeout_seconds)
+        try:
+            urlretrieve(file_url, file_path)
+        except urllib.error.ContentTooShortError as ex:
+            raise FileDownloadFailedException("File download did not finish correctly " + str(ex))
         return file_path
 
     def get_model_arch_params(self, model_name: str) -> Optional[DictConfig]:
         """Get the model arch_params from DeciPlatform.
         :param model_name:  Name of the model as saved in the platform.
         :return:            arch_params. None if arch_params were not found for this specific model on this SG version."""
         arch_params_file = self._get_file(model_name, AutoNACFileName.STRUCTURE_YAML)
@@ -142,92 +183,84 @@
 
             logger.info(
                 f"*** IMPORTANT ***: files required for the model {model_name} were downloaded and added to your code in:\n{package_path}\n"
                 f"These files will be downloaded to the same location each time the model is fetched from the deci-client.\n"
                 f"you can override this by passing models.get(... download_required_code=False) and importing the files yourself"
             )
 
-    def upload_model(self, model: nn.Module, model_meta_data, optimization_request_form):
+    def upload_model(
+        self,
+        model: nn.Module,
+        name: str,
+        input_dimensions: "Sequence[int]",
+        target_hardware_types: "Optional[List[HardwareType]]" = None,
+        target_quantization_level: "Optional[QuantizationLevel]" = None,
+        target_batch_size: "Optional[int]" = None,
+    ):
         """
         This function will upload the trained model to the Deci Lab
 
-        :param model:                     The resulting model from the training process
-        :param model_meta_data:           Metadata to accompany the model
-        :param optimization_request_form: The optimization parameters
-        """
-        self.lab_client.add_model(
-            add_model_request=model_meta_data,
-            optimization_request=optimization_request_form,
-            local_loaded_model=model,
+        :param model:                            The resulting model from the training process
+        :param name:                             The model's name
+        :param input_dimensions:                 The model's input dimensions
+        :param target_hardware_types:            List of hardware types to optimize the model for
+        :param target_quantization_level:        The quantization level to optimize the model for
+        :param target_batch_size:                The batch size to optimize the model for
+        """
+        model_id = self.lab_client.register_model(
+            model=model,
+            name=name,
+            framework=FrameworkType.PYTORCH,
+            input_dimensions=input_dimensions,
         )
+        if target_hardware_types:
+            kwargs = {}
+            if target_quantization_level:
+                kwargs["quantization_level"] = target_quantization_level
+            if target_batch_size:
+                kwargs["batch_size"] = target_batch_size
+            self.lab_client.optimize_model(model_id=model_id, hardware_types=target_hardware_types, **kwargs)
 
     def is_model_benchmarking(self, name: str) -> bool:
         """Check if a given model is still benchmarking or not.
         :param name: The mode name.
         """
-        benchmark_state = self.lab_client.get_model_by_name(name=name).data.benchmark_state
+        benchmark_state = self.lab_client.get_model(name=name)[0]["benchmarkState"]
         return benchmark_state in [ModelBenchmarkState.IN_PROGRESS, ModelBenchmarkState.PENDING]
 
     def register_experiment(self, name: str, model_name: str, resume: bool):
         """Registers a training experiment in Deci's backend.
         :param name:        Name of the experiment to register
         :param model_name:  Name of the model architecture to connect the experiment to
         """
         try:
-            self.lab_client.register_user_architecture(BodyRegisterUserArchitecture(architecture_name=model_name))
-        except ApiException as e:
-            if e.status == 422:
-                logger.debug(f"The model was already registered, or validation error: {e.body}")
-            else:
-                raise e
+            self.lab_client.register_user_architecture(name=model_name)
+        except (ApiException, ApiTypeError) as e:
+            logger.debug(f"The model was already registered, or validation error: {e}")
 
         self.lab_client.register_experiment(name=name, model_name=model_name, resume=resume)
 
     def save_experiment_file(self, file_path: str):
         """
         Uploads a training related file to Deci's location in S3. This can be a TensorBoard file or a log
         :params file_path: The local path of the file to be uploaded
         """
         self.lab_client.save_experiment_file(file_path=file_path)
 
-    def upload_file_to_s3(self, tag: str, level: str, from_path: str):
+    def upload_file_to_s3(self, tag: str, level: "SentryLevel", from_path: str):
         """Upload a file to the platform S3 bucket.
 
         :param tag:         Tag that will be associated to the file.
         :param level:       Logging level that will be used to notify the monitoring system that the file was uploaded.
         :param from_path:   Path of the file to upload.
         """
         data = self.lab_client.upload_log_url(tag=tag, level=level)
-        signed_url = S3SignedUrl(**data.data)
+        signed_url = S3SignedUrl(**data)
         self.lab_client.upload_file_to_s3(from_path=from_path, s3_signed_url=signed_url)
 
-    def add_model(
-        self,
-        model_metadata,
-        hardware_types: List[str],
-        model_path: Optional[str] = None,
-        model: Optional[nn.Module] = None,
-        **kwargs: Any,
-    ):
-        """Adds a new model to the company's model repository.
-        :param model_metadata: The model metadata.
-        :param hardware_types: The hardware types you want to benchmark the model on.
-        :param model_path:      The path of the model on the local operating system.
-        :param model:           Pytorch loaded model object.
-                                If your model's framework is pytorch you may pass the following parameters as kwargs in order to control the conversion to onnx
-        :param kwargs: Extra arguments to be passed to the PyTorch to ONNX conversion, for example:
-            opset_version
-            do_constant_folding
-            dynamic_axes
-            input_names
-            output_names
-        """
-
-        self.lab_client.add_model_v2(model_metadata=model_metadata, hardware_types=hardware_types, model_path=model_path, model=model, **kwargs)
-
 
 def _move_file_to_folder(src_file_path: str, dest_dir_name: str) -> str:
     """Move a file to a newly created folder in the same directory.
 
     :param src_file_path:   Path of the file to be moved.
     :param dest_dir_name:   Name of the destination folder.
     :return:                The path of the moved file.
```

## super_gradients/common/sg_loggers/abstract_sg_logger.py

```diff
@@ -166,7 +166,11 @@
     @abstractmethod
     def local_dir(self) -> str:
         """
         A getter for the full/absolute path where all files are saved locally
         :return:
         """
         raise NotImplementedError
+
+    def download_remote_ckpt(self, ckpt_name: str, *args, **kwargs):
+
+        raise NotImplementedError
```

## super_gradients/common/sg_loggers/base_sg_logger.py

```diff
@@ -13,15 +13,15 @@
 from super_gradients.common.registry.registry import register_sg_logger
 from super_gradients.common.data_interface.adnn_model_repository_data_interface import ADNNModelRepositoryDataInterfaces
 from super_gradients.common.abstractions.abstract_logger import get_logger
 from super_gradients.common.decorators.code_save_decorator import saved_codes
 from super_gradients.common.environment.ddp_utils import multi_process_safe
 from super_gradients.common.sg_loggers.abstract_sg_logger import AbstractSGLogger
 from super_gradients.training.params import TrainingParams
-from super_gradients.training.utils import sg_trainer_utils
+from super_gradients.training.utils import sg_trainer_utils, get_param
 from super_gradients.common.environment.monitoring import SystemMonitor
 from super_gradients.common.auto_logging.auto_logger import AutoLoggerConfig
 from super_gradients.common.auto_logging.console_logging import ConsoleSink
 
 logger = get_logger(__name__)
 
 EXPERIMENT_LOGS_PREFIX = "experiment_logs"
@@ -97,14 +97,15 @@
 
         if launch_tensorboard:
             self._launch_tensorboard(port=tensorboard_port)
 
         self._init_system_monitor(monitor_system)
 
         self._save_code()
+        self._resume_from_remote_sg_logger = get_param(training_params, "resume_from_remote_sg_logger")
 
     @multi_process_safe
     def _launch_tensorboard(self, port):
         self.tensor_board_process, _ = sg_trainer_utils.launch_tensorboard_process(self._local_dir, port=port)
 
     @multi_process_safe
     def _init_tensorboard(self, resumed, tb_files_user_prompt):
```

## super_gradients/common/sg_loggers/wandb_sg_logger.py

```diff
@@ -42,14 +42,15 @@
         save_checkpoints_remote: bool = True,
         save_tensorboard_remote: bool = True,
         save_logs_remote: bool = True,
         entity: Optional[str] = None,
         api_server: Optional[str] = None,
         save_code: bool = False,
         monitor_system: bool = None,
+        save_checkpoint_as_artifact: bool = False,
         **kwargs,
     ):
         """
 
         :param experiment_name:         Name used for logging and loading purposes
         :param storage_location:        If set to 's3' (i.e. s3://my-bucket) saves the Checkpoints in AWS S3 otherwise saves the Checkpoints Locally
         :param resumed:                 If true, then old tensorboard files will **NOT** be deleted when tb_files_user_prompt=True
@@ -59,14 +60,17 @@
         :param launch_tensorboard:      Whether to launch a TensorBoard process.
         :param tensorboard_port:        Specific port number for the tensorboard to use when launched (when set to None, some free port number will be used)
         :param save_checkpoints_remote: Saves checkpoints in s3.
         :param save_tensorboard_remote: Saves tensorboard in s3.
         :param save_logs_remote:        Saves log files in s3.
         :param monitor_system:          Not Available for WandB logger. Save the system statistics (GPU utilization, CPU, ...) in the tensorboard
         :param save_code:               Save current code to wandb
+        :save_checkpoint_as_artifact:   Save model checkpoint using Weights & Biases Artifact. Note that setting this option to True would save model
+                                        checkpoints every epoch as a versioned artifact, which will result in use of increased storage usage on
+                                        Weights & Biases.
         """
         if monitor_system is not None:
             logger.warning("monitor_system not available on WandBSGLogger. To remove this warning, please don't set monitor_system in your logger parameters")
 
         self.s3_location_available = storage_location.startswith("s3")
         super().__init__(
             project_name=project_name,
@@ -87,28 +91,43 @@
         if api_server is not None:
             if api_server != env_variables.WANDB_BASE_URL:
                 logger.warning(f"WANDB_BASE_URL environment parameter not set to {api_server}. Setting the parameter")
                 os.environ["WANDB_BASE_URL"] = api_server
 
         # allow passing an arbitrary pre-defined wandb_id
         wandb_id = kwargs.pop("wandb_id", None)
+
         self.resumed = resumed
         if self.resumed:
-            if wandb_id is not None:
-                logger.warning("Resuming the run with a previous WandB ID instead of the one from logger params")
-            wandb_id = self._get_wandb_id()
+            if wandb_id is None:
+                if self._resume_from_remote_sg_logger:
+                    raise RuntimeError(
+                        "For WandB loggers, when training_params.resume_from_remote_sg_logger=True "
+                        "pass the run id through the wandb_id arg in sg_logger_params"
+                    )
+                wandb_id = self._get_wandb_id()
+
+        if wandb.run is None:
+            run = wandb.init(project=project_name, name=experiment_name, entity=entity, resume=resumed, id=wandb_id, **kwargs)
+        else:
+            logger.warning(
+                "A Weights & Biases run was initialized before initializing `WandBSGLogger`. "
+                "This means that `super-gradients` cannot control the run ID to which this session will be logged."
+            )
+            logger.warning(f"In order to resume this run please call `wandb.init(id={wandb.run.id}, resume='must')` before reinitializing `WandBSGLogger`.")
+            run = wandb.run
 
-        run = wandb.init(project=project_name, name=experiment_name, entity=entity, resume=resumed, id=wandb_id, **kwargs)
         if save_code:
             self._save_code_lines()
 
         self._set_wandb_id(run.id)
         self.save_checkpoints_wandb = save_checkpoints_remote
         self.save_tensorboard_wandb = save_tensorboard_remote
         self.save_logs_wandb = save_logs_remote
+        self.save_checkpoint_as_artifact = save_checkpoint_as_artifact
 
     @multi_process_safe
     def _save_code_lines(self):
         """
         Save the current code to wandb.
         If a file named .wandbinclude is avilable in the root dir of the project the settings will be taken from the file.
         Otherwise, all python file in the current working dir (recursively) will be saved.
@@ -225,27 +244,43 @@
 
         if self.save_tensorboard_wandb:
             wandb.save(glob_str=self._get_tensorboard_file_name(), base_path=self._local_dir, policy="now")
 
         if self.save_logs_wandb:
             wandb.save(glob_str=self.experiment_log_path, base_path=self._local_dir, policy="now")
 
+    def _save_wandb_artifact(self, path):
+        """Upload a file or a directory as a Weights & Biases Artifact.
+        Note that this function can be called only after wandb.init()
+
+        :param path: the local full path to the pth file to be uploaded
+        """
+        artifact = wandb.Artifact(f"{wandb.run.id}-checkpoint", type="model")
+        if os.path.isdir(path):
+            artifact.add_dir(path)
+        elif os.path.isfile(path):
+            artifact.add_file(path)
+        wandb.log_artifact(artifact)
+
     @multi_process_safe
     def add_checkpoint(self, tag: str, state_dict: dict, global_step: int = 0):
         name = f"ckpt_{global_step}.pth" if tag is None else tag
         if not name.endswith(".pth"):
             name += ".pth"
 
         path = os.path.join(self._local_dir, name)
         torch.save(state_dict, path)
 
         if self.save_checkpoints_wandb:
             if self.s3_location_available:
                 self.model_checkpoints_data_interface.save_remote_checkpoints_file(self.experiment_name, self._local_dir, name)
-            wandb.save(glob_str=path, base_path=self._local_dir, policy="now")
+            if self.save_checkpoint_as_artifact:
+                self._save_wandb_artifact(path)
+            else:
+                wandb.save(glob_str=path, base_path=self._local_dir, policy="now")
 
     def _get_tensorboard_file_name(self):
         try:
             tb_file_path = self.tensorboard_writer.file_writer.event_writer._file_name
         except RuntimeError:
             logger.warning("tensorboard file could not be located for ")
             return None
@@ -312,7 +347,10 @@
                     return os.path.join(cur_dir, file_name)
                 else:
                     cur_dir = os.path.dirname(cur_dir)
         except RuntimeError:
             return None
 
         return None
+
+    def download_remote_ckpt(self, *args, **kwargs):
+        wandb.restore("ckpt_latest.pth", replace=True, root=self.local_dir())
```

## super_gradients/examples/deci_lab_export_example/deci_lab_export_example.py

```diff
@@ -7,71 +7,52 @@
 import os
 from super_gradients.training import models
 
 from super_gradients import Trainer
 from super_gradients.training.dataloaders.dataloaders import classification_test_dataloader
 from super_gradients.training.metrics import Accuracy, Top5
 from super_gradients.training.utils.callbacks import DeciLabUploadCallback, ModelConversionCheckCallback
-from deci_lab_client.models import (
-    Metric,
-    QuantizationLevel,
-    ModelMetadata,
-    OptimizationRequestForm,
-    HardwareType,
-    FrameworkType,
-)
+from deci_platform_client.models import QuantizationLevel, HardwareType
 
 
 def main(architecture_name: str):
     # Empty on purpose so that it can be fit to the trainer use case
     checkpoint_dir = ""
 
-    os.environ["DECI_PLATFORM_TOKEN"] = "YOUR_API_TOKEN_HERE"  # You can also set your token as environment variable using the commandline or your IDE.
+    # You can also set your token as environment variable using the commandline or your IDE.
+    os.environ["DECI_CLIENT_ID"] = "YOUR_CLIENT_ID_HERE"
+    os.environ["DECI_CLIENT_SECRET"] = "YOUR_SECRET_KEY_HERE"
     trainer = Trainer(
         f"lab_optimization_{architecture_name}_example",
         model_checkpoints_location="local",
         ckpt_root_dir=checkpoint_dir,
     )
 
     model = models.get(architecture=architecture_name, arch_params={"use_aux_heads": True})
 
     # CREATE META-DATA, AND OPTIMIZATION REQUEST FORM FOR DECI PLATFORM POST TRAINING CALLBACK
     model_name = f"{architecture_name}_for_deci_lab_export_example"
-    model_meta_data = ModelMetadata(
-        name=model_name,
-        primary_batch_size=1,
-        architecture=architecture_name.title(),
-        framework=FrameworkType.PYTORCH,
-        dl_task="classification",
-        input_dimensions=(3, 320, 320),
-        primary_hardware=HardwareType.K80,
-        dataset_name="ImageNet",
-        description=f"{architecture_name} deci.ai Test",
-        tags=["imagenet", architecture_name],
-    )
-
-    optimization_request_form = OptimizationRequestForm(
-        target_hardware=HardwareType.T4,
-        target_batch_size=1,
-        target_metric=Metric.LATENCY,
-        optimize_model_size=True,
-        quantization_level=QuantizationLevel.FP16,
-        optimize_autonac=True,
-    )
 
     # IT IS ALSO RECOMMENDED TO USE A PRE TRAINING MODEL CONVERSION CHECK CALLBACK, SO THAT ANY CONVERSION
     # ERRORS WON'T APPEAR FOR THE FIRST TIME ONLY AT THE END OF TRAINING:
 
     phase_callbacks = [
-        ModelConversionCheckCallback(model_meta_data=model_meta_data, opset_version=11),
-        DeciLabUploadCallback(
-            model_meta_data=model_meta_data,
-            optimization_request_form=optimization_request_form,
+        ModelConversionCheckCallback(
+            model_name=model_name,
+            input_dimensions=(3, 320, 320),
+            primary_batch_size=1,
             opset_version=11,
         ),
+        DeciLabUploadCallback(
+            model_name=model_name,
+            input_dimensions=(3, 320, 320),
+            target_hardware_types=[HardwareType.T4],
+            target_batch_size=1,
+            target_quantization_level=QuantizationLevel.FP16,
+        ),
     ]
 
     # DEFINE TRAINING PARAMETERS
     train_params = {
         "max_epochs": 2,
         "lr_updates": [1],
         "lr_decay_factor": 0.1,
@@ -86,12 +67,17 @@
         "metric_to_watch": "Accuracy",
         "greater_metric_to_watch_is_better": True,
         "phase_callbacks": phase_callbacks,
     }
 
     # RUN TRAINING. ONCE ALL EPOCHS ARE DONE THE OPTIMIZED MODEL FILE WILL BE LOCATED IN THE EXPERIMENT'S
     # CHECKPOINT DIRECTORY
-    trainer.train(model=model, training_params=train_params, train_loader=classification_test_dataloader(), valid_loader=classification_test_dataloader())
+    trainer.train(
+        model=model,
+        training_params=train_params,
+        train_loader=classification_test_dataloader(),
+        valid_loader=classification_test_dataloader(),
+    )
 
 
 if __name__ == "__main__":
     main(architecture_name="efficientnet_b0")
```

## super_gradients/modules/pose_estimation_modules.py

```diff
@@ -54,15 +54,14 @@
             nn.BatchNorm2d(heatmap_channels),
             activation(inplace=True),
             nn.Conv2d(heatmap_channels, heatmap_channels, kernel_size=3, padding=1, bias=False),
             nn.BatchNorm2d(heatmap_channels),
             activation(inplace=True),
             nn.UpsamplingBilinear2d(scale_factor=upscale_factor) if upscale_factor > 1 else nn.Identity(),
             nn.Conv2d(heatmap_channels, self.num_joints + 1, kernel_size=1, padding=0),
-            nn.Sigmoid(),
         )
 
         self.transition_offset = nn.Sequential(
             nn.Conv2d(in_channels, self.num_joints * offset_channels_per_joint, kernel_size=1, padding=0, bias=False),
             nn.BatchNorm2d(self.num_joints * offset_channels_per_joint),
             activation(inplace=True),
             nn.UpsamplingBilinear2d(scale_factor=upscale_factor) if upscale_factor > 1 else nn.Identity(),
```

## super_gradients/modules/qarepvgg_block.py

```diff
@@ -312,9 +312,20 @@
         # no need to fuse post_bn prematurely if it is there
         # call self.full_fusion() if you need it
         self.partial_fusion()
 
     def from_repvgg(self, src: RepVGGBlock):
         raise NotImplementedError
 
-    def prep_model_for_conversion(self, input_size: Optional[Union[tuple, list]] = None, **kwargs):
-        self.partial_fusion()
+    def prep_model_for_conversion(self, input_size: Optional[Union[tuple, list]] = None, full_fusion: bool = True, **kwargs):
+        """Prepare the QARepVGGBlock for conversion.
+
+        :WARNING: the default `full_fusion=True` will make the block non-trainable.
+
+        :param full_fusion: If True, performs full fusion, converting the block into a non-trainable, fully fused block.
+                            If False, performs partial fusion, slower for inference but still trainable.
+        """
+
+        if full_fusion:
+            self.full_fusion()
+        else:
+            self.partial_fusion()
```

## super_gradients/recipes/coco2017_pose_dekr_w32_no_dc.yaml

```diff
@@ -1,54 +1,60 @@
 #  DEKR training example with COCO dataset.
 #  Reproduction and refinement of paper: Bottom-Up Human Pose Estimation Via Disentangled Keypoint Regression.
 #
-#  Recipe runs with batch size = 8 X 8 gpus = 64.
+#  Note: Original DEKR architecture using deformable convolutions. This recipe uses standard convolutions to enable
+#  model be exportable to ONNX.
+#
+#  Recipe runs with batch size = 24 X 8 gpus = 192.
 #
 #  Instructions:
 #   0. Make sure that the data is stored in dataset_params.dataset_dir or add "dataset_params.data_dir=<PATH-TO-DATASET>" at the end of the command below (feel free to check ReadMe)
 #   1. Move to the project root (where you will find the ReadMe and src folder)
-#   2. Run the command:
-#       DEKR-W32: python -m super_gradients.train_from_recipe --config-name=coco2017_pose_dekr_w32_no_dc
-#  NOTE: Add "checkpoint_params.checkpoint_path=<hrnet-pretrained-path>" to use pretrained backbone (See line 55).
+#   2. Make sure you've downloaded pretrained backbone weights from https://1drv.ms/u/s!Aus8VCZ_C_33dYBMemi9xOUFR0w to project root (See line 55).
+#   3. Run the command:
+#       DEKR-W32-NO-DC: python -m super_gradients.train_from_recipe --config-name=coco2017_pose_dekr_w32_no_dc checkpoint_params.checkpoint_path=hrnetv2_w32_imagenet_pretrained.pth
+#
 #
+#  Validation AP (Without flip augmentation and rescoring) - COCO, training time:
+#      DEKR-W32-NO-DC:    input-size: [640, 640]     AP: 63.08 (Regular training)   8 X RTX A5000 - 21h
 #
-#  Validation AP (Without multiscale & flip augmentation) - COCO, training time:
-#      DEKR-W32:    input-size: [640, 640]     AP: TBD    8 X RTX A5000
+#  Scores with flip TTA and rescoring (Using best model from above):
+#      DEKR-W32-NO-DC:    input-size: [640, 640]     AP: 64.96 (With Flip TTA)
+#      DEKR-W32-NO-DC:    input-size: [640, 640]     AP: 67.34 (With Flip TTA and Rescoring)
 #
+#  Rescoring:
+#      See `coco2017_pose_dekr_rescoring.yaml` recipe and `documentation/source/PoseEstimation.md#Rescoring` section of the documentation.
 #
 #  Official git repo:
 #      https://github.com/HRNet/DEKR
 #  Paper:
 #      https://arxiv.org/abs/2104.02300
 #
 #
 #  Comments:
 #      * Pretrained backbones were used.
-#      * Results with Deci code are higher than original implementation, mostly thanks to changes in Detail loss and
-#          module, different auxiliary feature maps and different loss weights.
+#      * In DEKR-W32-NO-DC A suffix "NO-DC" stands for "No deformable convolutions".
 
 defaults:
   - training_hyperparams: coco2017_dekr_pose_train_params
   - dataset_params: coco_pose_estimation_dekr_dataset_params
   - arch_params: pose_dekr_w32_no_dc_arch_params
   - checkpoint_params: default_checkpoint_params
   - _self_
   - variable_setup
 
-resume: False
-
 architecture: dekr_w32_no_dc
 
 multi_gpu: DDP
 num_gpus: 8
 
 experiment_suffix: ""
-experiment_name: coco2017_pose_${architecture}_${experiment_suffix}
-
+experiment_name: coco2017_pose_${architecture}${experiment_suffix}
 
+ckpt_root_dir:
 
 train_dataloader: coco2017_pose_train
 val_dataloader: coco2017_pose_val
 
 arch_params:
   num_classes: ${dataset_params.num_joints}
 
@@ -60,38 +66,11 @@
   checkpoint_path: # <location of the downloaded hrnetv2_w32_imagenet_pretrained.pth>
   strict_load:
     _target_: super_gradients.training.sg_trainer.StrictLoad
     value: key_matching
 
 dataset_params:
   train_dataloader_params:
-    batch_size: 8
+    batch_size: 24
 
   val_dataloader_params:
-    batch_size: 16
-
-training_hyperparams:
-  resume: ${resume}
-  phase_callbacks: []
-#   Note: You can uncomment following block to enable visualization of intermediate results during training.
-#   When enabled, these callbacks will save first batch from training & validation to Tensorboard.
-#   This is helpful for debugging and doing visual checks whether predictions are reasonable and transforms are
-#   working as expected.
-#   The only downside is that it tend to bloat Tensorboard logs (Up to ten Gigs for long training regimes).
-#  phase_callbacks:
-#    - DEKRVisualizationCallback:
-#        phase:
-#          _target_: super_gradients.training.utils.callbacks.callbacks.Phase
-#          value: TRAIN_BATCH_END
-#        prefix: "train_"
-#        mean: [ 0.485, 0.456, 0.406 ]
-#        std: [ 0.229, 0.224, 0.225 ]
-#        apply_sigmoid: False
-#
-#    - DEKRVisualizationCallback:
-#        phase:
-#          _target_: super_gradients.training.utils.callbacks.callbacks.Phase
-#          value: VALIDATION_BATCH_END
-#        prefix: "val_"
-#        mean: [ 0.485, 0.456, 0.406 ]
-#        std: [ 0.229, 0.224, 0.225 ]
-#        apply_sigmoid: False
+    batch_size: 32
```

## super_gradients/recipes/arch_params/pose_dekr_w32_no_dc_arch_params.yaml

```diff
@@ -29,16 +29,15 @@
     - SUM
     - SUM
   HEAD_HEATMAP:
     BLOCK: BASIC
     NUM_BLOCKS: 1
     NUM_CHANNELS: 32
     DILATION_RATE: 1
-    # We do also apply sigmoid to the heatmap output to restrict the output to [0, 1] range (Original paper does not apply sigmoid).
-    HEATMAP_APPLY_SIGMOID: True
+    HEATMAP_APPLY_SIGMOID: False
 
   HEAD_OFFSET:
     # Note we replace ADAPTIVE conv with BASIC conv since deformable conv is not supported in TensorRT,
     # and we want the model to be exportable.
     # Instead, we set dilation rate to 5 to mimic the effect of ADAPTIVE conv.
     # Original recipe uses ADAPTIVE conv:
     # BLOCK: ADAPTIVE
```

## super_gradients/recipes/arch_params/yolo_nas_l_arch_params.yaml

```diff
@@ -1,7 +1,9 @@
+in_channels: 3
+
 backbone:
   NStageBackbone:
 
     stem:
       YoloNASStem:
         out_channels: 48
```

## super_gradients/recipes/arch_params/yolo_nas_m_arch_params.yaml

```diff
@@ -1,7 +1,9 @@
+in_channels: 3
+
 backbone:
   NStageBackbone:
 
     stem:
       YoloNASStem:
         out_channels: 48
```

## super_gradients/recipes/arch_params/yolo_nas_s_arch_params.yaml

```diff
@@ -1,7 +1,9 @@
+in_channels: 3
+
 backbone:
   NStageBackbone:
 
     stem:
       YoloNASStem:
         out_channels: 48
```

## super_gradients/recipes/checkpoint_params/default_checkpoint_params.yaml

```diff
@@ -1,9 +1,9 @@
 load_checkpoint: False # whether to load checkpoint
 load_backbone: False # whether to load only backbone part of checkpoint
 checkpoint_path: # checkpoint path that is located in super_gradients/checkpoints
 external_checkpoint_path: # checkpoint path that is not located in super_gradients/checkpoints
 source_ckpt_folder_name: # dirname for checkpoint loading
 strict_load: # key matching strictness for loading checkpoint's weights
   _target_: super_gradients.training.sg_trainer.StrictLoad
-  value: True
+  value: no_key_matching
 pretrained_weights: # a string describing the dataset of the pretrained weights (for example "imagenent").
```

## super_gradients/recipes/dataset_params/coco_detection_yolo_nas_dataset_params.yaml

```diff
@@ -27,15 +27,15 @@
         prob: 0.5                       # probability to apply horizontal flip
     - DetectionMixup:
         input_dim:
         mixup_scale: [ 0.5, 1.5 ]         # random rescale range for the additional sample in mixup
         prob: 0.5                       # probability to apply per-sample mixup
         flip_prob: 0.5                  # probability to apply horizontal flip
     - DetectionPaddedRescale:
-        input_dim: [640, 640]
+        input_dim: ${dataset_params.train_dataset_params.input_dim}
         max_targets: 120
         pad_value: 114
     - DetectionStandardize:
         max_value: 255.
     - DetectionTargetsFormatTransform:
         max_targets: 256
         output_format: LABEL_CXCYWH
```

## super_gradients/recipes/dataset_params/coco_pose_estimation_dataset_params.yaml

```diff
@@ -1,19 +1,44 @@
 num_joints: 17
 
 # OKs sigma values take from https://github.com/cocodataset/cocoapi/blob/master/PythonAPI/pycocotools/cocoeval.py#L523
 oks_sigmas: [0.026, 0.025, 0.025, 0.035, 0.035, 0.079, 0.079, 0.072, 0.072, 0.062, 0.062, 1.007, 1.007, 0.087, 0.087, 0.089, 0.089]
 
+flip_indexes_heatmap: [ 0, 2, 1, 4, 3, 6, 5, 8, 7, 10, 9, 12, 11, 14, 13, 16, 15, 17]
+flip_indexes_offset: [ 0, 2, 1, 4, 3, 6, 5, 8, 7, 10, 9, 12, 11, 14, 13, 16, 15,]
+
+joint_links:
+  - [0, 1]
+  - [0, 2]
+  - [1, 2]
+  - [1, 3]
+  - [2, 4]
+  - [3, 5]
+  - [4, 6]
+  - [5, 6]
+  - [5, 7]
+  - [5, 11]
+  - [6, 8]
+  - [6, 12]
+  - [7, 9]
+  - [8, 10]
+  - [11, 12]
+  - [11, 13]
+  - [12, 14]
+  - [13, 15]
+  - [14, 16]
+
+
 train_dataset_params:
   data_dir: /data/coco # root path to coco data
   images_dir: images/train2017
   json_file: annotations/person_keypoints_train2017.json
 
   include_empty_samples: False
-  min_instance_area: 128
+  min_instance_area: 64
 
   transforms:
     - KeypointsLongestMaxSize:
         max_height: 640
         max_width: 640
 
     - KeypointsPadIfNeeded:
@@ -25,20 +50,20 @@
     - KeypointsRandomHorizontalFlip:
         # Note these indexes are COCO-specific. If you're using a different dataset, you'll need to change these accordingly.
         flip_index: [ 0, 2, 1, 4, 3, 6, 5, 8, 7, 10, 9, 12, 11, 14, 13, 16, 15 ]
         prob: 0.5
 
     - KeypointsRandomAffineTransform:
         max_rotation: 30
-        min_scale: 0.75
-        max_scale: 1.5
+        min_scale: 0.5
+        max_scale: 2
         max_translate: 0.2
         image_pad_value: [ 127, 127, 127 ]
         mask_pad_value: 1
-        prob: 0.5
+        prob: 0.75
 
     - KeypointsImageToTensor
 
     - KeypointsImageNormalize:
         mean: [ 0.485, 0.456, 0.406 ]
         std: [ 0.229, 0.224, 0.225 ]
 
@@ -69,17 +94,14 @@
 
 
 train_dataloader_params:
   shuffle: True
   batch_size: 8
   num_workers: 8
   drop_last: True
-  worker_init_fn:
-    _target_: super_gradients.training.utils.utils.load_func
-    dotpath: super_gradients.training.datasets.datasets_utils.worker_init_reset_seed
   collate_fn:
     _target_: super_gradients.training.datasets.pose_estimation_datasets.KeypointsCollate
 
 val_dataloader_params:
   batch_size: 24
   num_workers: 8
   drop_last: False
```

## super_gradients/recipes/training_hyperparams/coco2017_dekr_pose_train_params.yaml

```diff
@@ -1,38 +1,72 @@
 defaults:
   - default_train_params
 
-ema: True
-max_epochs: 400
+ema: False
+ema_params:
+  decay: 0.9997
+  decay_type: exp
+  beta: 20
+
+max_epochs: 150
 lr_mode: cosine
-cosine_final_lr_ratio: 0.01
+cosine_final_lr_ratio: 0.1
 batch_accumulate: 1
-initial_lr: 0.001
+initial_lr: 1e-3
 loss: dekr_loss
 
 criterion_params:
+  heatmap_loss: qfl
   heatmap_loss_factor: 1.0
-  offset_loss_factor: 0.03
+  offset_loss_factor: 0.1
 
+mixed_precision: True
 
 optimizer: AdamW
 optimizer_params:
-  weight_decay: 0.0005
+  weight_decay: 0.0001
 lr_warmup_steps: 256
 warmup_initial_lr: 1e-06
 
 valid_metrics_list:
   - PoseEstimationMetrics:
       num_joints: ${dataset_params.num_joints}
       oks_sigmas: ${dataset_params.oks_sigmas}
-      max_objects_per_image: 20
+      max_objects_per_image: 30
       post_prediction_callback:
         _target_: super_gradients.training.utils.pose_estimation.DEKRPoseEstimationDecodeCallback
-        max_num_people: 20
+        max_num_people: 30
         keypoint_threshold: 0.05
         nms_threshold: 0.05
         nms_num_threshold: 8
         output_stride: 4
-        apply_sigmoid: False
+        apply_sigmoid: True
+
+
+phase_callbacks: []
+#   Note: You can uncomment following block to enable visualization of intermediate results during training.
+#   When enabled, these callbacks will save first batch from training & validation to Tensorboard.
+#   This is helpful for debugging and doing visual checks whether predictions are reasonable and transforms are
+#   working as expected.
+#   The only downside is that it tend to bloat Tensorboard logs (Up to ten Gigs for long training regimes).
+#  phase_callbacks:
+#    - DEKRVisualizationCallback:
+#        phase:
+#          _target_: super_gradients.training.utils.callbacks.callbacks.Phase
+#          value: TRAIN_BATCH_END
+#        prefix: "train_"
+#        mean: [ 0.485, 0.456, 0.406 ]
+#        std: [ 0.229, 0.224, 0.225 ]
+#        apply_sigmoid: True
+#
+#    - DEKRVisualizationCallback:
+#        phase:
+#          _target_: super_gradients.training.utils.callbacks.callbacks.Phase
+#          value: VALIDATION_BATCH_END
+#        prefix: "val_"
+#        mean: [ 0.485, 0.456, 0.406 ]
+#        std: [ 0.229, 0.224, 0.225 ]
+#        apply_sigmoid: True
+
 
 metric_to_watch: 'AP'
 greater_metric_to_watch_is_better: True
```

## super_gradients/recipes/training_hyperparams/default_train_params.yaml

```diff
@@ -1,9 +1,18 @@
 resume: False # whether to continue training from ckpt with the same experiment name.
 resume_path: # Explicit checkpoint path (.pth file) to use to resume training.
+
+resume_from_remote_sg_logger: False # bool (default=False), When true, ckpt_name (checkpoint filename
+#        to resume i.e ckpt_latest.pth bydefault) will be downloaded into the experiment checkpoints directory
+#        prior to loading weights, then training is resumed from that checkpoint. The source is unique to
+#        every logger, and currently supported for WandB loggers only.
+#
+#        IMPORTANT: Only works for experiments that were ran with sg_logger_params.save_checkpoints_remote=True.
+#        IMPORTANT: For WandB loggers, one must also pass the run id through the wandb_id arg in sg_logger_params.
+
 ckpt_name: ckpt_latest.pth  # The checkpoint (.pth file) filename in CKPT_ROOT_DIR/EXPERIMENT_NAME/ to use when resume=True and resume_path=None
 lr_mode: # Learning rate scheduling policy, one of ['step','poly','cosine','function']
 lr_schedule_function: # Learning rate scheduling function to be used when `lr_mode` is 'function'.
 lr_warmup_epochs: 0 # number of epochs for learning rate warm up - see https://arxiv.org/pdf/1706.02677.pdf (Section 2.2).
 lr_warmup_steps: 0  # number of warmup steps (Used when warmup_mode=linear_batch_step)
 lr_cooldown_epochs: 0 # epochs to cooldown LR (i.e the last epoch from scheduling view point=max_epochs-cooldown)
 warmup_initial_lr: # Initial lr for linear_epoch_step/linear_batch_step. When none is given, initial_lr/(warmup_epochs+1) will be used.
```

## super_gradients/sanity_check/env_sanity_check.py

```diff
@@ -74,15 +74,15 @@
 def check_packages():
     """Check that all installed libs respect the requirement.txt, and requirements.pro.txt if relevant.
     Note: We only log an error
     """
     test_name = "installed packages"
 
     installed_packages = {package.key.lower(): package.version for package in pkg_resources.working_set}
-    requirements = get_requirements(use_pro_requirements="deci-lab-client" in installed_packages)
+    requirements = get_requirements(use_pro_requirements="deci-platform-client" in installed_packages)
 
     if requirements is None:
         logger.info(msg='Library check is not supported when super_gradients installed through "git+https://github.com/..." command')
         return
 
     for requirement in pkg_resources.parse_requirements(requirements):
         package_name = requirement.name.lower()
```

## super_gradients/training/__init__.py

```diff
@@ -1,19 +1,21 @@
 # PACKAGE IMPORTS FOR EXTERNAL USAGE
 import super_gradients.training.utils.distributed_training_utils as distributed_training_utils
 from super_gradients.training.datasets import datasets_utils, DataAugmentation
 from super_gradients.training.sg_trainer import Trainer
 from super_gradients.training.kd_trainer import KDTrainer
 from super_gradients.training.qat_trainer import QATTrainer
 from super_gradients.common import MultiGPUMode, StrictLoad, EvaluationType
+from super_gradients.training.pre_launch_callbacks import modify_params_for_qat
 
 __all__ = [
     "distributed_training_utils",
     "datasets_utils",
     "DataAugmentation",
     "Trainer",
     "KDTrainer",
     "QATTrainer",
     "MultiGPUMode",
     "StrictLoad",
     "EvaluationType",
+    "modify_params_for_qat",
 ]
```

## super_gradients/training/params.py

```diff
@@ -60,14 +60,19 @@
     "resume_strict_load": False,
     "sync_bn": False,
     "kill_ddp_pgroup_on_end": True,  # Whether to kill the DDP process group in the end of training.
     "max_train_batches": None,  # For debug- when not None- will break out of inner train loop
     # (i.e iterating over train_loader) when reaching this number of batches.
     "max_valid_batches": None,  # For debug- when not None- will break out of inner valid loop
     # (i.e iterating over valid_loader) when reaching this number of batches.
+    "resume_from_remote_sg_logger": False  # When true, ckpt_name (checkpoint filename to resume, ckpt_latest.pth by
+    # default) will be downloaded into the experiment checkpoints directory prior to loading weights, then resumed
+    # from that checkpoint. The source is unique to every logger, and currently supported for WandB loggers only.
+    # Note that for this to work, the experiment must be ran with sg_logger_params.save_checkpoints_remote=True. For
+    # WandB loggers, one must also pass the run id through the wandb_id arg in sg_logger_params.
 }
 
 DEFAULT_OPTIMIZER_PARAMS_SGD = {"weight_decay": 1e-4, "momentum": 0.9}
 
 DEFAULT_OPTIMIZER_PARAMS_ADAM = {"weight_decay": 1e-4}
 
 DEFAULT_OPTIMIZER_PARAMS_RMSPROP = {"weight_decay": 1e-4, "momentum": 0.9}
```

## super_gradients/training/pretrained_models.py

```diff
@@ -43,18 +43,21 @@
     "ppyoloe_s_coco": "https://sghub.deci.ai/models/ppyoloe_s_coco.pth",
     "ppyoloe_m_coco": "https://sghub.deci.ai/models/ppyoloe_m_coco.pth",
     "ppyoloe_l_coco": "https://sghub.deci.ai/models/ppyoloe_l_coco.pth",
     "ppyoloe_x_coco": "https://sghub.deci.ai/models/ppyoloe_x_coco.pth",
     "yolo_nas_s_coco": "https://sghub.deci.ai/models/yolo_nas_s_coco.pth",
     "yolo_nas_m_coco": "https://sghub.deci.ai/models/yolo_nas_m_coco.pth",
     "yolo_nas_l_coco": "https://sghub.deci.ai/models/yolo_nas_l_coco.pth",
+    "dekr_w32_no_dc_coco_pose": "https://sghub.deci.ai/models/dekr_w32_no_dc_coco_pose.pth",
+    "pose_rescoring_coco_coco_pose": "https://sghub.deci.ai/models/pose_rescoring_coco_coco_pose.pth",
 }
 
 
 PRETRAINED_NUM_CLASSES = {
     "imagenet": 1000,
     "imagenet21k": 21843,
     "coco_segmentation_subclass": 21,
     "cityscapes": 19,
     "coco": 80,
+    "coco_pose": 17,
     "cifar10": 10,
 }
```

## super_gradients/training/dataloaders/__init__.py

```diff
@@ -7,14 +7,16 @@
     coco2017_val_ssd_lite_mobilenet_v2,
     coco2017_train_ppyoloe,
     coco2017_val_ppyoloe,
     coco2017_pose_train,
     coco2017_pose_val,
     coco2017_train_yolo_nas,
     coco2017_val_yolo_nas,
+    coco2017_rescoring_val,
+    coco2017_rescoring_train,
     imagenet_train,
     imagenet_val,
     imagenet_efficientnet_train,
     imagenet_efficientnet_val,
     imagenet_mobilenetv2_train,
     imagenet_mobilenetv2_val,
     imagenet_mobilenetv3_train,
@@ -66,14 +68,16 @@
     "coco2017_val_ssd_lite_mobilenet_v2",
     "coco2017_train_ppyoloe",
     "coco2017_val_ppyoloe",
     "coco2017_pose_train",
     "coco2017_pose_val",
     "coco2017_train_yolo_nas",
     "coco2017_val_yolo_nas",
+    "coco2017_rescoring_train",
+    "coco2017_rescoring_val",
     "imagenet_train",
     "imagenet_val",
     "imagenet_efficientnet_train",
     "imagenet_efficientnet_val",
     "imagenet_mobilenetv2_train",
     "imagenet_mobilenetv2_val",
     "imagenet_mobilenetv3_train",
```

## super_gradients/training/dataloaders/dataloaders.py

```diff
@@ -1,12 +1,13 @@
 from typing import Dict, Mapping
 
 import hydra
 import numpy as np
 import torch
+from omegaconf import OmegaConf, UnsupportedValueType, DictConfig, open_dict
 from torch.utils.data import BatchSampler, DataLoader, TensorDataset, RandomSampler
 
 import super_gradients
 from super_gradients.common.abstractions.abstract_logger import get_logger
 from super_gradients.common.registry.registry import register_dataloader, ALL_DATALOADERS
 from super_gradients.common.factories.collate_functions_factory import CollateFunctionsFactory
 from super_gradients.common.factories.datasets_factory import DatasetsFactory
@@ -19,14 +20,16 @@
 )
 from super_gradients.training.datasets.detection_datasets import COCODetectionDataset, RoboflowDetectionDataset, YoloDarknetFormatDetectionDataset
 from super_gradients.training.datasets.detection_datasets.pascal_voc_detection import (
     PascalVOCUnifiedDetectionTrainDataset,
     PascalVOCDetectionDataset,
 )
 from super_gradients.training.datasets.pose_estimation_datasets import COCOKeypointsDataset
+from super_gradients.training.datasets.pose_estimation_datasets.rescoring_dataset import TrainRescoringDataset, ValTrainRescoringDataset
+from super_gradients.training.datasets.samplers import RepeatAugSampler
 from super_gradients.training.datasets.segmentation_datasets import (
     CityscapesDataset,
     CoCoSegmentationDataSet,
     PascalVOC2012SegmentationDataSet,
     PascalVOCAndAUGUnifiedDataset,
     SuperviselyPersonsDataset,
     MapillaryDataset,
@@ -34,14 +37,15 @@
 from super_gradients.training.utils import get_param
 from super_gradients.training.utils.distributed_training_utils import (
     wait_for_the_master,
     get_local_rank,
 )
 from super_gradients.training.utils.utils import override_default_params_without_nones
 from super_gradients.common.environment.cfg_utils import load_dataset_params
+import torch.distributed as dist
 
 
 logger = get_logger(__name__)
 
 
 def get_data_loader(config_name: str, dataset_cls: object, train: bool, dataset_params: Mapping = None, dataloader_params: Mapping = None) -> DataLoader:
     """
@@ -76,22 +80,55 @@
     dataloader_params = _process_dataloader_params(cfg, dataloader_params, dataset, train)
 
     dataloader = DataLoader(dataset=dataset, **dataloader_params)
     dataloader.dataloader_params = dataloader_params
     return dataloader
 
 
-def _process_dataset_params(cfg, dataset_params, train):
-    default_dataset_params = cfg.train_dataset_params if train else cfg.val_dataset_params
-    default_dataset_params = hydra.utils.instantiate(default_dataset_params)
-    for key, val in default_dataset_params.items():
-        if key not in dataset_params.keys() or dataset_params[key] is None:
-            dataset_params[key] = val
+def _process_dataset_params(cfg, dataset_params, train: bool):
+    """
+    Merge the default dataset config with the user-provided overrides.
+    This function handles variable interpolation in the dataset config.
 
-    return dataset_params
+    :param cfg: Default dataset config
+    :param dataset_params: User-provided overrides
+    :param train: boolean flag indicating whether we are processing train or val dataset params
+    :return: New dataset params (merged defaults and overrides, where overrides take precedence)
+    """
+
+    try:
+        # No, we can't simplify the following lines to:
+        # >>> default_dataset_params = cfg.train_dataset_params if train else cfg.val_dataset_params
+        # >>> dataset_params = OmegaConf.merge(default_dataset_params, dataset_params)
+        # >>> return hydra.utils.instantiate(dataset_params)
+        # For some reason this breaks interpolation :shrug:
+        if not isinstance(dataset_params, DictConfig):
+            dataset_params = OmegaConf.create(dataset_params)
+        if train:
+            train_dataset_params = cfg.train_dataset_params
+            with open_dict(train_dataset_params):
+                train_dataset_params.merge_with(dataset_params)
+            cfg.train_dataset_params = train_dataset_params
+            return hydra.utils.instantiate(cfg.train_dataset_params)
+        else:
+            val_dataset_params = cfg.val_dataset_params
+            with open_dict(val_dataset_params):
+                val_dataset_params.merge_with(dataset_params)
+            cfg.val_dataset_params = val_dataset_params
+            return hydra.utils.instantiate(cfg.val_dataset_params)
+
+    except UnsupportedValueType:
+        # This is somewhat ugly fallback for the case when the user provides overrides for the dataset params
+        # that contains non-primitive types (E.g instantiated transforms).
+        # In this case interpolation is not possible so we just override the default params with the user-provided ones.
+        default_dataset_params = hydra.utils.instantiate(cfg.train_dataset_params if train else cfg.val_dataset_params)
+        for key, val in default_dataset_params.items():
+            if key not in dataset_params.keys() or dataset_params[key] is None:
+                dataset_params[key] = val
+        return dataset_params
 
 
 def _process_dataloader_params(cfg, dataloader_params, dataset, train):
     default_dataloader_params = cfg.train_dataloader_params if train else cfg.val_dataloader_params
     default_dataloader_params = hydra.utils.instantiate(default_dataloader_params)
     dataloader_params = _process_sampler_params(dataloader_params, dataset, default_dataloader_params)
     dataloader_params = _process_collate_fn_params(dataloader_params)
@@ -118,14 +155,26 @@
     is_dist = super_gradients.is_distributed()
     dataloader_params = override_default_params_without_nones(dataloader_params, default_dataloader_params)
     if get_param(dataloader_params, "sampler") is not None:
         dataloader_params = _instantiate_sampler(dataset, dataloader_params)
     elif is_dist:
         dataloader_params["sampler"] = {"DistributedSampler": {}}
         dataloader_params = _instantiate_sampler(dataset, dataloader_params)
+        if get_param(dataloader_params, "min_samples") is not None:
+            min_samples = dataloader_params.pop("min_samples")
+            if len(dataset) < min_samples:
+                world_size = dist.get_world_size()
+                num_repeats = min_samples / len(dataset)
+                selected_ratio = world_size / num_repeats
+
+                # WE SET selected_ratio = world_size / num_repeats SO THAT IN RepeatAugSampler THE NUMBER OF SAMPLES
+                # PER EPOCH PER RANK WILL BE DETERMINED BY
+                # int(math.ceil(len(self.dataset) / selected_ratio)) =  min_samples / world_size
+
+                dataloader_params["sampler"] = RepeatAugSampler(dataset=dataset, num_repeats=num_repeats, selected_round=0, selected_ratio=selected_ratio)
     elif get_param(dataloader_params, "min_samples") is not None:
         min_samples = dataloader_params.pop("min_samples")
         if len(dataset) < min_samples:
             dataloader_params["sampler"] = RandomSampler(dataset, replacement=True, num_samples=min_samples)
             if "shuffle" in dataloader_params.keys():
                 dataloader_params.pop("shuffle")
             logger.info(f"Using min_samples={min_samples}")
@@ -784,14 +833,36 @@
         dataset_cls=COCOKeypointsDataset,
         train=False,
         dataset_params=dataset_params,
         dataloader_params=dataloader_params,
     )
 
 
+@register_dataloader(Dataloaders.COCO2017_RESCORING_TRAIN)
+def coco2017_rescoring_train(dataset_params: Dict = None, dataloader_params: Dict = None) -> DataLoader:
+    return get_data_loader(
+        config_name="coco_pose_estimation_rescoring_dataset_params",
+        dataset_cls=TrainRescoringDataset,
+        train=True,
+        dataset_params=dataset_params,
+        dataloader_params=dataloader_params,
+    )
+
+
+@register_dataloader(Dataloaders.COCO2017_RESCORING_VAL)
+def coco2017_rescoring_val(dataset_params: Dict = None, dataloader_params: Dict = None) -> DataLoader:
+    return get_data_loader(
+        config_name="coco_pose_estimation_rescoring_dataset_params",
+        dataset_cls=ValTrainRescoringDataset,
+        train=False,
+        dataset_params=dataset_params,
+        dataloader_params=dataloader_params,
+    )
+
+
 def get(name: str = None, dataset_params: Dict = None, dataloader_params: Dict = None, dataset: torch.utils.data.Dataset = None) -> DataLoader:
     """
     Get DataLoader of the recipe-configured dataset defined by name in ALL_DATALOADERS.
 
     :param name: dataset name in ALL_DATALOADERS.
     :param dataset_params: dataset params that override the yaml configured defaults, then passed to the dataset_cls.__init__.
     :param dataloader_params: DataLoader params that override the yaml configured defaults, then passed to the DataLoader.__init__
```

## super_gradients/training/datasets/__init__.py

```diff
@@ -12,28 +12,29 @@
 )
 from super_gradients.training.datasets.segmentation_datasets.segmentation_dataset import SegmentationDataSet
 from super_gradients.training.datasets.segmentation_datasets.pascal_voc_segmentation import (
     PascalVOC2012SegmentationDataSet,
     PascalAUG2012SegmentationDataSet,
     PascalVOCAndAUGUnifiedDataset,
 )
-from super_gradients.training.datasets.segmentation_datasets.cityscape_segmentation import CityscapesDataset
+from super_gradients.training.datasets.segmentation_datasets.cityscape_segmentation import CityscapesDataset, CityscapesConcatDataset
 from super_gradients.training.datasets.segmentation_datasets.coco_segmentation import CoCoSegmentationDataSet
 from super_gradients.training.datasets.segmentation_datasets.supervisely_persons_segmentation import SuperviselyPersonsDataset
 from super_gradients.training.datasets.pose_estimation_datasets import COCOKeypointsDataset
 
 cv2.setNumThreads(0)
 
 
 __all__ = [
     "DataAugmentation",
     "ListDataset",
     "DirectoryDataSet",
     "SegmentationDataSet",
     "CityscapesDataset",
+    "CityscapesConcatDataset",
     "PascalVOC2012SegmentationDataSet",
     "PascalAUG2012SegmentationDataSet",
     "PascalVOCAndAUGUnifiedDataset",
     "CoCoSegmentationDataSet",
     "DetectionDataset",
     "COCODetectionDataset",
     "YoloDarknetFormatDetectionDataset",
```

## super_gradients/training/datasets/datasets_utils.py

```diff
@@ -9,15 +9,14 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import torch
 import torch.distributed as dist
 import torch.nn.functional as F
 import torchvision
 from PIL import Image
-from deprecate import deprecated
 from matplotlib.patches import Rectangle
 from torchvision.datasets import ImageFolder
 from torchvision.transforms import transforms, InterpolationMode, RandomResizedCrop
 from tqdm import tqdm
 
 from super_gradients.common.abstractions.abstract_logger import get_logger
 from super_gradients.common.object_names import Callbacks, Transforms
@@ -70,34 +69,14 @@
         else:
             chsum += (inputs - mean).pow(2).sum(dim=(0, 2, 3), keepdim=True)
     std = torch.sqrt(chsum / (len(trainset) * h * w - 1))
     print(f"std: {std.view(-1)}")
     return mean.view(-1).cpu().numpy().tolist(), std.view(-1).cpu().numpy().tolist()
 
 
-@deprecated(target=get_mean_and_std_torch, deprecated_in="2.1.0", remove_in="3.0.0")
-def get_mean_and_std(dataset):
-    """Compute the mean and std value of dataset."""
-    dataloader = torch.utils.data.DataLoader(dataset, batch_size=1, shuffle=True, num_workers=1)
-    mean = torch.zeros(3)
-    std = torch.zeros(3)
-    print("==> Computing mean and std..")
-    j = 0
-    for inputs, targets in dataloader:
-        if j % 10 == 0:
-            print(j)
-        j += 1
-        for i in range(3):
-            mean[i] += inputs[:, i, :, :].mean()
-            std[i] += inputs[:, i, :, :].std()
-    mean.div_(len(dataset))
-    std.div_(len(dataset))
-    return mean, std
-
-
 class AbstractCollateFunction(ABC):
     """
     A collate function (for torch DataLoader)
     """
 
     @abstractmethod
     def __call__(self, batch):
```

## super_gradients/training/datasets/data_formats/bbox_formats/cxcywh.py

```diff
@@ -94,15 +94,15 @@
     """
     if not torch.jit.is_scripting():
         if torch.is_tensor(bboxes) and not torch.is_floating_point(bboxes):
             warnings.warn(
                 f"Detected non floating-point ({bboxes.dtype}) input to xyxy_to_cxcywh_inplace function. This may cause rounding errors and lose of precision. "
                 "You may want to convert your array to floating-point precision first."
             )
-        if not is_floating_point_array(bboxes):
+        elif isinstance(bboxes, np.ndarray) and not is_floating_point_array(bboxes):
             warnings.warn(
                 f"Detected non floating-point input ({bboxes.dtype}) to xyxy_to_cxcywh_inplace function. This may cause rounding errors and lose of precision. "
                 "You may want to convert your array to floating-point precision first."
             )
     bboxes[..., 2:4] -= bboxes[..., 0:2]  # x2y2 - x1y2 -> wh
     bboxes[..., 0:2] += bboxes[..., 2:4] * 0.5  # cxcywh
     return bboxes
```

## super_gradients/training/datasets/detection_datasets/detection_dataset.py

```diff
@@ -20,14 +20,15 @@
 from super_gradients.common.abstractions.abstract_logger import get_logger
 from super_gradients.training.transforms.transforms import DetectionTransform, DetectionTargetsFormatTransform, DetectionTargetsFormat
 from super_gradients.training.exceptions.dataset_exceptions import EmptyDatasetException, DatasetValidationException
 from super_gradients.common.factories.list_factory import ListFactory
 from super_gradients.common.factories.transforms_factory import TransformsFactory
 from super_gradients.training.datasets.data_formats.default_formats import XYXY_LABEL
 from super_gradients.training.datasets.data_formats.formats import ConcatenatedTensorFormat
+from super_gradients.training.utils.utils import ensure_is_tuple_of_two
 
 logger = get_logger(__name__)
 
 
 @register_dataset(Datasets.DETECTION_DATASET)
 class DetectionDataset(Dataset):
     """Detection dataset.
@@ -72,28 +73,31 @@
     def __init__(
         self,
         data_dir: str,
         original_target_format: Union[ConcatenatedTensorFormat, DetectionTargetsFormat],
         max_num_samples: int = None,
         cache: bool = False,
         cache_dir: str = None,
-        input_dim: Optional[Tuple[int, int]] = None,
+        input_dim: Union[int, Tuple[int, int], None] = None,
         transforms: List[DetectionTransform] = [],
         all_classes_list: Optional[List[str]] = [],
         class_inclusion_list: Optional[List[str]] = None,
         ignore_empty_annotations: bool = True,
         target_fields: List[str] = None,
         output_fields: List[str] = None,
         verbose: bool = True,
         show_all_warnings: bool = False,
     ):
         """Detection dataset.
 
         :param data_dir:                Where the data is stored
-        :param input_dim:               Image size (when loaded, before transforms).
+        :param input_dim:               Image size (when loaded, before transforms). Can be None, scalar or tuple (rows, cols).
+                                        None means that the image will be loaded as is.
+                                        Scalar (size) - Image will be resized to (size, size)
+                                        Tuple (rows,cols) - Image will be resized to (rows, cols)
         :param original_target_format:  Format of targets stored on disk. raw data format, the output format might
                                         differ based on transforms.
         :param max_num_samples:         If not None, set the maximum size of the dataset by only indexing the first n annotations/images.
         :param cache:                   Whether to cache images or not.
         :param cache_dir:              Path to the directory where cached images will be stored in an optimized format.
         :param transforms:              List of transforms to apply sequentially on sample.
         :param all_classes_list:        All the class names.
@@ -125,15 +129,15 @@
             raise RuntimeError(f"data_dir={data_dir} not found. Please make sure that data_dir points toward your dataset.")
 
         # Number of images that are available (regardless of ignored images)
         self.n_available_samples = self._setup_data_source()
         if not isinstance(self.n_available_samples, int) or self.n_available_samples < 1:
             raise ValueError(f"_setup_data_source() should return the number of available samples but got {self.n_available_samples}")
 
-        self.input_dim = input_dim
+        self.input_dim = ensure_is_tuple_of_two(input_dim)
         self.original_target_format = original_target_format
         self.max_num_samples = max_num_samples
 
         if len(all_classes_list) != len(set(all_classes_list)):
             raise DatasetValidationException(f"all_classes_list contains duplicate class names: {collections.Counter(all_classes_list)}")
 
         if class_inclusion_list is not None and len(class_inclusion_list) != len(set(class_inclusion_list)):
@@ -287,19 +291,18 @@
             NUM_THREADs = min(8, os.cpu_count())
             loaded_images = ThreadPool(NUM_THREADs).imap(func=lambda x: self._load_resized_img(x), iterable=range(len(self)))
 
             # Initialize placeholder for images
             cached_imgs = np.memmap(str(img_resized_cache_path), shape=(len(self), max_h, max_w, 3), dtype=np.uint8, mode="w+")
 
             # Store images in the placeholder
-            loaded_images_pbar = tqdm(enumerate(loaded_images), total=len(self), disable=not self.verbose)
-            for i, image in loaded_images_pbar:
-                cached_imgs[i][: image.shape[0], : image.shape[1], :] = image.copy()
-            cached_imgs.flush()
-            loaded_images_pbar.close()
+            with tqdm(enumerate(loaded_images), total=len(self), disable=not self.verbose) as loaded_images_pbar:
+                for i, image in loaded_images_pbar:
+                    cached_imgs[i][: image.shape[0], : image.shape[1], :] = image.copy()
+                cached_imgs.flush()
         else:
             logger.warning("You are using cached imgs!")
 
         logger.info("Loading cached imgs...")
         cached_imgs = np.memmap(str(img_resized_cache_path), shape=(len(self), max_h, max_w, 3), dtype=np.uint8, mode="r+")
         return cached_imgs
```

## super_gradients/training/datasets/detection_datasets/roboflow/roboflow100.py

```diff
@@ -13,15 +13,15 @@
     Checkout the datasets at https://universe.roboflow.com/roboflow-100?ref=blog.roboflow.com
 
     To use this Dataset you need to:
 
         - Follow the official instructions to download Roboflow100: https://github.com/roboflow/roboflow-100-benchmark?ref=roboflow-blog
             //!\\ To use this dataset, you have to download the "coco" format, NOT the yolov5.
 
-        - Your dataset should loook like this:
+        - Your dataset should look like this:
             rf100
             ├── 4-fold-defect
             │      ├─ train
             │      │    ├─ 000000000001.jpg
             │      │    ├─ ...
             │      │    └─ _annotations.coco.json
             │      ├─ valid
```

## super_gradients/training/datasets/pose_estimation_datasets/coco_keypoints.py

```diff
@@ -75,15 +75,15 @@
         img, mask, gt_joints, gt_areas, gt_bboxes, gt_iscrowd = self.load_sample(index)
         img, mask, gt_joints, gt_areas, gt_bboxes = self.transforms(img, mask, gt_joints, areas=gt_areas, bboxes=gt_bboxes)
 
         image_shape = img.size(1), img.size(2)
         gt_joints, gt_areas, gt_bboxes, gt_iscrowd = self.filter_joints(image_shape, gt_joints, gt_areas, gt_bboxes, gt_iscrowd)
 
         targets = self.target_generator(img, gt_joints, mask)
-        return img, targets, {"gt_joints": gt_joints, "gt_bboxes": gt_bboxes, "gt_iscrowd": gt_iscrowd}
+        return img, targets, {"gt_joints": gt_joints, "gt_bboxes": gt_bboxes, "gt_iscrowd": gt_iscrowd, "gt_areas": gt_areas}
 
     def load_sample(self, index):
         img_id = self.ids[index]
         image_info = self.coco.loadImgs(img_id)[0]
         file_name = image_info["file_name"]
         file_path = os.path.join(self.images_dir, file_name)
         ann_ids = self.coco.getAnnIds(imgIds=img_id)
```

## super_gradients/training/datasets/pose_estimation_datasets/target_generators.py

```diff
@@ -184,14 +184,16 @@
                     joint_rg[joint_rg.shape[0] // 2, joint_rg.shape[1] // 2] = 1
 
                     heatmaps[idx, aa:bb, cc:dd] = np.maximum(heatmaps[idx, aa:bb, cc:dd], joint_rg)
                     # print(heatmaps[-1, 0, 0])
                     ignored_hms[idx, aa:bb, cc:dd] = 1.0
 
         for person_id, p in enumerate(joints):
+            person_area = area[person_id]
+            offset_weight_factor = 1.0 / np.clip(np.sqrt(person_area), a_min=1, a_max=None)
             ct_x = int(p[-1, 0])
             ct_y = int(p[-1, 1])
             ct_v = int(p[-1, 2])
             if ct_v < 1 or ct_x < 0 or ct_y < 0 or ct_x >= output_cols or ct_y >= output_rows:
                 continue
 
             for idx, pt in enumerate(p[:-1]):
@@ -208,16 +210,16 @@
                     for pos_x in range(start_x, end_x):
                         for pos_y in range(start_y, end_y):
                             offset_x = pos_x - x
                             offset_y = pos_y - y
 
                             offset_map[idx * 2, pos_y, pos_x] = offset_x
                             offset_map[idx * 2 + 1, pos_y, pos_x] = offset_y
-                            offset_weight[idx * 2, pos_y, pos_x] = 1.0 / np.sqrt(area[person_id])
-                            offset_weight[idx * 2 + 1, pos_y, pos_x] = 1.0 / np.sqrt(area[person_id])
+                            offset_weight[idx * 2, pos_y, pos_x] = offset_weight_factor
+                            offset_weight[idx * 2 + 1, pos_y, pos_x] = offset_weight_factor
 
         ignored_hms[ignored_hms == 2] = self.bg_weight
 
         mask = cv2.resize(mask, dsize=(output_cols, output_rows), interpolation=cv2.INTER_LINEAR)
         mask = (mask > 0).astype(np.float32)
         mask = mask * ignored_hms
```

## super_gradients/training/datasets/samplers/__init__.py

```diff
@@ -1,6 +1,7 @@
+from super_gradients.training.datasets.samplers.infinite_sampler import InfiniteSampler
 from super_gradients.training.datasets.samplers.repeated_augmentation_sampler import RepeatAugSampler
 from super_gradients.common.object_names import Samplers
 from super_gradients.common.registry.registry import SAMPLERS
 
 
-__all__ = ["SAMPLERS", "Samplers", "RepeatAugSampler"]
+__all__ = ["SAMPLERS", "Samplers", "InfiniteSampler", "RepeatAugSampler"]
```

## super_gradients/training/datasets/segmentation_datasets/__init__.py

```diff
@@ -1,8 +1,8 @@
-from super_gradients.training.datasets.segmentation_datasets.cityscape_segmentation import CityscapesDataset
+from super_gradients.training.datasets.segmentation_datasets.cityscape_segmentation import CityscapesDataset, CityscapesConcatDataset
 from super_gradients.training.datasets.segmentation_datasets.coco_segmentation import CoCoSegmentationDataSet
 from super_gradients.training.datasets.segmentation_datasets.mapillary_dataset import MapillaryDataset
 from super_gradients.training.datasets.segmentation_datasets.pascal_voc_segmentation import (
     PascalVOC2012SegmentationDataSet,
     PascalVOCAndAUGUnifiedDataset,
     PascalAUG2012SegmentationDataSet,
 )
@@ -11,11 +11,12 @@
 
 __all__ = [
     "SegmentationDataSet",
     "CoCoSegmentationDataSet",
     "PascalAUG2012SegmentationDataSet",
     "PascalVOC2012SegmentationDataSet",
     "CityscapesDataset",
+    "CityscapesConcatDataset",
     "SuperviselyPersonsDataset",
     "PascalVOCAndAUGUnifiedDataset",
     "MapillaryDataset",
 ]
```

## super_gradients/training/datasets/segmentation_datasets/cityscape_segmentation.py

```diff
@@ -1,18 +1,18 @@
+from typing import List
 import os
 import cv2
 import numpy as np
 from PIL import Image, ImageColor
+from torch.utils.data import ConcatDataset
 
 from super_gradients.common.object_names import Datasets
 from super_gradients.common.registry.registry import register_dataset
 from super_gradients.training.datasets.segmentation_datasets.segmentation_dataset import SegmentationDataSet
 
-# TODO - ADD COARSE DATA - right now cityscapes dataset includes fine annotations. It's optional to use extra coarse
-#  annotations.
 
 # label for background and labels to ignore during training and evaluation.
 CITYSCAPES_IGNORE_LABEL = 19
 
 
 @register_dataset(Datasets.CITYSCAPES_DATASET)
 class CityscapesDataset(SegmentationDataSet):
@@ -71,15 +71,15 @@
 
     Example:
         >> CityscapesDataset(root_dir='.../root_dir', list_file='lists/train.lst', labels_csv_path='lists/labels.csv', ...)
     """
 
     def __init__(self, root_dir: str, list_file: str, labels_csv_path: str, **kwargs):
         """
-        :param root:            Absolute path to root directory of the dataset.
+        :param root_dir:        Absolute path to root directory of the dataset.
         :param list_file:       List file that contains names of images to load, line format: <image_path> <label_path>. The path is relative to root.
         :param labels_csv_path: Path to csv file, with labels metadata and mapping. The path is relative to root.
         :param kwargs:          Any hyper params required for the dataset, i.e img_size, crop_size, cache_images
         """
 
         self.root_dir = root_dir
         super().__init__(root_dir, list_file=list_file, **kwargs)
@@ -144,7 +144,43 @@
 
             :param target: The target mask to transform
             :return:       The transformed target mask
         """
         out = SegmentationDataSet.target_transform(target)
         out[out == 255] = CITYSCAPES_IGNORE_LABEL
         return out
+
+
+@register_dataset(Datasets.CITYSCAPES_CONCAT_DATASET)
+class CityscapesConcatDataset(ConcatDataset):
+    """
+    Support building a Cityscapes dataset which includes multiple group of samples from several list files.
+    i.e to initiate a trainval dataset:
+    >>> trainval_set = CityscapesConcatDataset(
+    >>>    root_dir='/data', list_files=['lists/train.lst', 'lists/val.lst'], labels_csv_path='lists/labels.csv', ...
+    >>> )
+
+    i.e to initiate a combination of the train-set with AutoLabelling-set:
+    >>> train_al_set = CityscapesConcatDataset(
+    >>>    root_dir='/data', list_files=['lists/train.lst', 'lists/auto_labelling.lst'], labels_csv_path='lists/labels.csv', ...
+    >>> )
+    """
+
+    def __init__(self, root_dir: str, list_files: List[str], labels_csv_path: str, **kwargs):
+        """
+        :param root_dir:        Absolute path to root directory of the dataset.
+        :param list_files:      List of list files that contains names of images to load,
+                                line format: <image_path> <label_path>. The path is relative to root.
+        :param labels_csv_path: Path to csv file, with labels metadata and mapping. The path is relative to root.
+        :param kwargs:          Any hyper params required for the dataset, i.e img_size, crop_size, cache_images
+        """
+        super().__init__(
+            datasets=[
+                CityscapesDataset(
+                    root_dir=root_dir,
+                    list_file=list_file,
+                    labels_csv_path=labels_csv_path,
+                    **kwargs,
+                )
+                for list_file in list_files
+            ]
+        )
```

## super_gradients/training/datasets/segmentation_datasets/coco_segmentation.py

```diff
@@ -137,23 +137,24 @@
                                 self._generate_segmentation_mask that uses the sub-classes inclusion tuple to keep only
                                 the annotations that are relevant to the sub-classes selected when instantiating the class
             :param  sub_dataset_image_ids_file_path: The path to save the sub-dataset in for future loading
             :return:            All of the ids with enough pixel data after the sub-classing
         """
         print("Creating sub-dataset , this will take a while but don't worry, it only runs once and caches the results")
         all_coco_image_ids = list(self.coco.imgs.keys())
-        tbar = tqdm(all_coco_image_ids, desc="Generating sub-dataset image ids")
         sub_dataset_image_ids = []
-        for i, img_id in enumerate(tbar):
-            coco_target_annotations = self.coco.loadAnns(self.coco.getAnnIds(imgIds=img_id))
-            img_metadata = self.coco.loadImgs(img_id)[0]
 
-            mask = self._generate_coco_segmentation_mask(coco_target_annotations, img_metadata["height"], img_metadata["width"])
+        with tqdm(all_coco_image_ids, desc="Generating sub-dataset image ids") as tbar:
+            for i, img_id in enumerate(tbar):
+                coco_target_annotations = self.coco.loadAnns(self.coco.getAnnIds(imgIds=img_id))
+                img_metadata = self.coco.loadImgs(img_id)[0]
 
-            # MAKE SURE THERE IS ENOUGH INPUT IN THE IMAGE (MORE THAN 1K PIXELS) AFTER SUB-CLASSES FILTRATION
-            if (mask > 0).sum() > 1000:
-                sub_dataset_image_ids.append(img_id)
+                mask = self._generate_coco_segmentation_mask(coco_target_annotations, img_metadata["height"], img_metadata["width"])
 
-            tbar.set_description("Processed images: {}/{}, generated {} qualified images".format(i, len(all_coco_image_ids), len(sub_dataset_image_ids)))
+                # MAKE SURE THERE IS ENOUGH INPUT IN THE IMAGE (MORE THAN 1K PIXELS) AFTER SUB-CLASSES FILTRATION
+                if (mask > 0).sum() > 1000:
+                    sub_dataset_image_ids.append(img_id)
+
+                tbar.set_description("Processed images: {}/{}, generated {} qualified images".format(i, len(all_coco_image_ids), len(sub_dataset_image_ids)))
         print("Number of images in sub-dataset: ", len(sub_dataset_image_ids))
         torch.save(sub_dataset_image_ids, sub_dataset_image_ids_file_path)
         return sub_dataset_image_ids
```

## super_gradients/training/datasets/segmentation_datasets/segmentation_dataset.py

```diff
@@ -151,51 +151,51 @@
         image_indices_to_remove = []
 
         # CACHE IMAGES INTO MEMORY FOR FASTER TRAINING (WARNING: LARGE DATASETS MAY EXCEED SYSTEM RAM)
         if self.cache_images:
             # CREATE AN EMPTY LIST FOR THE LABELS
             self.imgs = len(self) * [None]
             cached_images_mem_in_gb = 0.0
-            pbar = tqdm(image_files, desc="Caching images")
-            for i, img_path in enumerate(pbar):
-                img = self.sample_loader(img_path)
-                if img is None:
-                    image_indices_to_remove.append(i)
+            with tqdm(image_files, desc="Caching images") as pbar:
+                for i, img_path in enumerate(pbar):
+                    img = self.sample_loader(img_path)
+                    if img is None:
+                        image_indices_to_remove.append(i)
 
-                cached_images_mem_in_gb += os.path.getsize(image_files[i]) / 1024.0**3.0
+                    cached_images_mem_in_gb += os.path.getsize(image_files[i]) / 1024.0**3.0
 
-                self.imgs[i] = img
-                pbar.desc = "Caching images (%.1fGB)" % (cached_images_mem_in_gb)
+                    self.imgs[i] = img
+                    pbar.desc = "Caching images (%.1fGB)" % (cached_images_mem_in_gb)
             self.img_files = [e for i, e in enumerate(image_files) if i not in image_indices_to_remove]
             self.imgs = [e for i, e in enumerate(self.imgs) if i not in image_indices_to_remove]
 
         # CACHE LABELS INTO MEMORY FOR FASTER TRAINING - RELEVANT FOR EFFICIENT VALIDATION RUNS DURING TRAINING
         if self.cache_labels:
             # CREATE AN EMPTY LIST FOR THE LABELS
             self.labels = len(self) * [None]
-            pbar = tqdm(label_files, desc="Caching labels")
-            missing_labels, found_labels, duplicate_labels = 0, 0, 0
+            with tqdm(label_files, desc="Caching labels") as pbar:
+                missing_labels, found_labels, duplicate_labels = 0, 0, 0
 
-            for i, file in enumerate(pbar):
-                labels = self.target_loader(file)
+                for i, file in enumerate(pbar):
+                    labels = self.target_loader(file)
 
-                if labels is None:
-                    missing_labels += 1
-                    image_indices_to_remove.append(i)
-                    continue
-
-                self.labels[i] = labels
-                found_labels += 1
-
-                pbar.desc = "Caching labels (%g found, %g missing, %g duplicate, for %g images)" % (
-                    found_labels,
-                    missing_labels,
-                    duplicate_labels,
-                    len(image_files),
-                )
+                    if labels is None:
+                        missing_labels += 1
+                        image_indices_to_remove.append(i)
+                        continue
+
+                    self.labels[i] = labels
+                    found_labels += 1
+
+                    pbar.desc = "Caching labels (%g found, %g missing, %g duplicate, for %g images)" % (
+                        found_labels,
+                        missing_labels,
+                        duplicate_labels,
+                        len(image_files),
+                    )
             assert found_labels > 0, "No labels found."
 
             #  REMOVE THE IRRELEVANT ENTRIES FROM THE DATA
             self.label_files = [e for i, e in enumerate(label_files) if i not in image_indices_to_remove]
             self.labels = [e for i, e in enumerate(self.labels) if i not in image_indices_to_remove]
 
     def _transform_image_and_mask(self, image, mask) -> tuple:
```

## super_gradients/training/losses/__init__.py

```diff
@@ -7,14 +7,15 @@
 from super_gradients.training.losses.yolox_loss import YoloXDetectionLoss, YoloXFastDetectionLoss
 from super_gradients.training.losses.ssd_loss import SSDLoss
 from super_gradients.training.losses.bce_dice_loss import BCEDiceLoss
 from super_gradients.training.losses.dice_ce_edge_loss import DiceCEEdgeLoss
 from super_gradients.training.losses.ppyolo_loss import PPYoloELoss
 from super_gradients.training.losses.dekr_loss import DEKRLoss
 from super_gradients.training.losses.stdc_loss import STDCLoss
+from super_gradients.training.losses.rescoring_loss import RescoringLoss
 
 from super_gradients.common.object_names import Losses
 from super_gradients.common.registry.registry import LOSSES
 
 __all__ = [
     "LOSSES",
     "Losses",
@@ -28,8 +29,9 @@
     "SSDLoss",
     "BCEDiceLoss",
     "KDLogitsLoss",
     "DiceCEEdgeLoss",
     "PPYoloELoss",
     "DEKRLoss",
     "STDCLoss",
+    "RescoringLoss",
 ]
```

## super_gradients/training/losses/dekr_loss.py

```diff
@@ -12,25 +12,28 @@
     """
     Implementation of the loss function from the "Bottom-Up Human Pose Estimation Via Disentangled Keypoint Regression"
     paper (https://arxiv.org/abs/2104.02300)
 
     This loss should be used in conjunction with DEKRTargetsGenerator.
     """
 
-    def __init__(self, heatmap_loss_factor: float = 1.0, offset_loss_factor: float = 0.1):
+    def __init__(self, heatmap_loss_factor: float = 1.0, offset_loss_factor: float = 0.1, heatmap_loss: str = "mse"):
         """
         Instantiate the DEKR loss function. It is two-component loss function, consisting of a heatmap (MSE) loss and an offset (Smooth L1) losses.
         The total loss is the sum of the two individual losses, weighted by the corresponding factors.
 
         :param heatmap_loss_factor: Weighting factor for heatmap loss
         :param offset_loss_factor: Weighting factor for offset loss
+        :param heatmap_loss: Type of heatmap loss to use. Can be "mse" (Used in DEKR paper) or "qfl" (Quality Focal Loss).
+                             We use QFL in our recipe as it produces better results.
         """
         super().__init__()
         self.heatmap_loss_factor = float(heatmap_loss_factor)
         self.offset_loss_factor = float(offset_loss_factor)
+        self.heatmap_loss = {"mse": self.heatmap_mse_loss, "qfl": self.heatmap_qfl_loss}[heatmap_loss]
 
     @property
     def component_names(self):
         """
         Names of individual loss components for logging during training.
         """
         return ["heatmap", "offset", "total"]
@@ -65,19 +68,25 @@
                 offset_loss.unsqueeze(0),
                 loss.unsqueeze(0),
             )
         ).detach()
 
         return loss, components
 
-    def heatmap_loss(self, pred_heatmap, true_heatmap, mask):
+    def heatmap_mse_loss(self, pred_heatmap, true_heatmap, mask):
         loss = torch.nn.functional.mse_loss(pred_heatmap, true_heatmap, reduction="none") * mask
         loss = loss.mean()
         return loss
 
+    def heatmap_qfl_loss(self, pred_heatmap, true_heatmap, mask):
+        scale_factor = (true_heatmap - pred_heatmap.sigmoid()).abs().pow(2)
+        loss = torch.nn.functional.binary_cross_entropy_with_logits(pred_heatmap, true_heatmap, reduction="none") * scale_factor
+        loss = loss.mean()
+        return loss
+
     def offset_loss(self, pred_offsets, true_offsets, weights):
         num_pos = torch.nonzero(weights > 0).size()[0]
         loss = torch.nn.functional.smooth_l1_loss(pred_offsets, true_offsets, reduction="none", beta=1.0 / 9) * weights
         if num_pos == 0:
             num_pos = 1.0
         loss = loss.sum() / num_pos
         return loss
```

## super_gradients/training/losses/mask_loss.py

```diff
@@ -39,14 +39,17 @@
 
         mask = self._broadcast_mask(mask, criterion_loss.size())
         mask_loss = criterion_loss * mask
 
         if self.reduction == LossReduction.NONE.value:
             return criterion_loss * self.loss_weights[0] + mask_loss * self.loss_weights[1]
         mask_loss = mask_loss[mask == 1]  # consider only mask samples for mask loss computing
+        # If mask doesn't include foreground values, set mask_loss as 0.
+        if mask_loss.numel() == 0:
+            mask_loss = torch.tensor(0.0)
 
         mask_loss = apply_reduce(mask_loss, self.reduction)
         criterion_loss = apply_reduce(criterion_loss, self.reduction)
 
         loss = criterion_loss * self.loss_weights[0] + mask_loss * self.loss_weights[1]
         return loss
```

## super_gradients/training/metrics/pose_estimation_metrics.py

```diff
@@ -7,14 +7,15 @@
 from torchmetrics import Metric
 
 from super_gradients.common.abstractions.abstract_logger import get_logger
 from super_gradients.common.environment.ddp_utils import is_distributed
 from super_gradients.common.object_names import Metrics
 from super_gradients.common.registry.registry import register_metric
 from super_gradients.training.metrics.pose_estimation_utils import compute_img_keypoint_matching, compute_visible_bbox_xywh
+from super_gradients.training.utils import convert_to_tensor
 from super_gradients.training.utils.detection_utils import compute_detection_metrics_per_cls
 
 logger = get_logger(__name__)
 
 __all__ = ["PoseEstimationMetrics"]
 
 
@@ -115,16 +116,17 @@
         self.post_prediction_callback = post_prediction_callback
         self.is_distributed = is_distributed()
         self.world_size = None
         self.rank = None
         self.add_state("predictions", default=[], dist_reduce_fx=None)
 
     def reset(self) -> None:
-        self.predictions = []
+        self.predictions.clear()
 
+    @torch.no_grad()
     def update(
         self,
         preds,
         target,
         gt_joints: List[np.ndarray],
         gt_iscrowd: List[np.ndarray] = None,
         gt_bboxes: List[np.ndarray] = None,
@@ -167,62 +169,62 @@
             gt_areas = [bboxes[:, 2] * bboxes[:, 3] for bboxes in gt_bboxes]
 
         if gt_iscrowd is None:
             gt_iscrowd = [[False] * len(x) for x in gt_joints]
 
         for i in range(len(predicted_poses)):
             self.update_single_image(
-                predicted_poses[i], predicted_scores[i], gt_joints[i], gt_areas=gt_areas[i], gt_bboxes=gt_bboxes[i], gt_is_crowd=gt_iscrowd[i]
+                predicted_poses[i], predicted_scores[i], gt_joints[i], gt_areas=gt_areas[i], gt_bboxes=gt_bboxes[i], gt_iscrowd=gt_iscrowd[i]
             )
 
     def update_single_image(
         self,
         predicted_poses: Union[Tensor, np.ndarray],
         predicted_scores: Union[Tensor, np.ndarray],
         groundtruths: Union[Tensor, np.ndarray],
         gt_bboxes: Union[Tensor, np.ndarray],
         gt_areas: Union[Tensor, np.ndarray],
-        gt_is_crowd: Union[Tensor, np.ndarray, List[bool]],
+        gt_iscrowd: Union[Tensor, np.ndarray, List[bool]],
     ):
         if len(predicted_poses) == 0 and len(groundtruths) == 0:
             return
         if len(predicted_poses) != len(predicted_scores):
             raise ValueError("Length of predicted poses and scores should be equal. Got {} and {}".format(len(predicted_poses), len(predicted_scores)))
-        if len(groundtruths) != len(gt_areas) != len(gt_bboxes) != len(gt_is_crowd):
+        if len(groundtruths) != len(gt_areas) != len(gt_bboxes) != len(gt_iscrowd):
             raise ValueError(
                 "Length of groundtruths, areas, bboxes and iscrowd should be equal. Got {} and {} and {} and {}".format(
-                    len(groundtruths), len(gt_areas), len(gt_bboxes), len(gt_is_crowd)
+                    len(groundtruths), len(gt_areas), len(gt_bboxes), len(gt_iscrowd)
                 )
             )
 
-        predicted_poses = torch.tensor(predicted_poses, dtype=torch.float, device=self.device)
-        predicted_scores = torch.tensor(predicted_scores, dtype=torch.float, device=self.device)
+        predicted_poses = convert_to_tensor(predicted_poses, dtype=torch.float32, device=self.device)
+        predicted_scores = convert_to_tensor(predicted_scores, dtype=torch.float32, device=self.device)
 
-        gt_keypoints = torch.tensor(groundtruths, dtype=torch.float, device=self.device)
-        gt_areas = torch.tensor(gt_areas, dtype=torch.float, device=self.device)
-        gt_bboxes = torch.tensor(gt_bboxes, dtype=torch.float, device=self.device)
+        gt_keypoints = convert_to_tensor(groundtruths, dtype=torch.float32, device=self.device)
+        gt_areas = convert_to_tensor(gt_areas, dtype=torch.float32, device=self.device)
+        gt_bboxes = convert_to_tensor(gt_bboxes, dtype=torch.float32, device=self.device)
+        gt_iscrowd = convert_to_tensor(gt_iscrowd, dtype=torch.bool, device=self.device)
 
         gt_keypoints_xy = gt_keypoints[:, :, 0:2]
         gt_keypoints_visibility = gt_keypoints[:, :, 2]
         gt_all_kpts_invisible = gt_keypoints_visibility.eq(0).all(dim=1)
-        gt_is_crowd = torch.tensor(gt_is_crowd, dtype=torch.bool, device=self.device)
-        gt_is_ignore = gt_all_kpts_invisible | gt_is_crowd
+        gt_is_ignore = gt_all_kpts_invisible | gt_iscrowd
 
         targets = gt_keypoints_xy[~gt_is_ignore] if len(groundtruths) else []
         targets_visibilities = gt_keypoints_visibility[~gt_is_ignore] if len(groundtruths) else []
         targets_areas = gt_areas[~gt_is_ignore] if len(groundtruths) else []
         targets_bboxes = gt_bboxes[~gt_is_ignore]
         targets_ignored = gt_is_ignore[~gt_is_ignore]
 
         crowd_targets = gt_keypoints_xy[gt_is_ignore] if len(groundtruths) else []
         crowd_visibilities = gt_keypoints_visibility[gt_is_ignore] if len(groundtruths) else []
         crowd_targets_areas = gt_areas[gt_is_ignore]
         crowd_targets_bboxes = gt_bboxes[gt_is_ignore]
 
-        preds_matched, preds_to_ignore, preds_scores, num_targets = compute_img_keypoint_matching(
+        mr = compute_img_keypoint_matching(
             predicted_poses,
             predicted_scores,
             #
             targets=targets,
             targets_visibilities=targets_visibilities,
             targets_areas=targets_areas,
             targets_bboxes=targets_bboxes,
@@ -234,15 +236,15 @@
             crowd_targets_bboxes=crowd_targets_bboxes,
             #
             iou_thresholds=self.iou_thresholds.to(self.device),
             sigmas=self.oks_sigmas.to(self.device),
             top_k=self.max_objects_per_image,
         )
 
-        self.predictions.append((preds_matched, preds_to_ignore, preds_scores, num_targets))
+        self.predictions.append((mr.preds_matched.cpu(), mr.preds_to_ignore.cpu(), mr.preds_scores.cpu(), int(mr.num_targets)))
 
     def _sync_dist(self, dist_sync_fn=None, process_group=None):
         """
         When in distributed mode, stats are aggregated after each forward pass to the metric state. Since these have all
         different sizes we override the synchronization function since it works only for tensors (and use
         all_gather_object)
         :param dist_sync_fn:
@@ -252,15 +254,14 @@
             self.world_size = torch.distributed.get_world_size() if self.is_distributed else -1
         if self.rank is None:
             self.rank = torch.distributed.get_rank() if self.is_distributed else -1
 
         if self.is_distributed:
             local_state_dict = self.predictions
             gathered_state_dicts = [None] * self.world_size
-            torch.distributed.barrier()
             torch.distributed.all_gather_object(gathered_state_dicts, local_state_dict)
             self.predictions = list(itertools.chain(*gathered_state_dicts))
 
     def compute(self) -> Dict[str, Union[float, torch.Tensor]]:
         """Compute the metrics for all the accumulated results.
         :return: Metrics of interest
         """
```

## super_gradients/training/metrics/pose_estimation_utils.py

```diff
@@ -1,8 +1,8 @@
-from typing import Tuple
+import dataclasses
 
 import numpy as np
 import torch
 from torch import Tensor
 
 
 def compute_visible_bbox_xywh(joints: Tensor, visibility_mask: Tensor) -> np.ndarray:
@@ -92,14 +92,22 @@
             if k1 > 0:
                 e = e[gt_keypoint_visibility > 0]
             ious[pred_index, gt_index] = torch.sum(torch.exp(-e)) / e.shape[0]
 
     return ious
 
 
+@dataclasses.dataclass
+class ImageKeypointMatchingResult:
+    preds_matched: Tensor
+    preds_to_ignore: Tensor
+    preds_scores: Tensor
+    num_targets: int
+
+
 def compute_img_keypoint_matching(
     preds: Tensor,
     pred_scores: Tensor,
     targets: Tensor,
     targets_visibilities: Tensor,
     targets_areas: Tensor,
     targets_bboxes: Tensor,
@@ -107,15 +115,15 @@
     crowd_targets: Tensor,
     crowd_visibilities: Tensor,
     crowd_targets_areas: Tensor,
     crowd_targets_bboxes: Tensor,
     iou_thresholds: torch.Tensor,
     sigmas: Tensor,
     top_k: int,
-) -> Tuple[Tensor, Tensor, Tensor, int]:
+) -> ImageKeypointMatchingResult:
     """
     Match predictions and the targets (ground truth) with respect to IoU and confidence score for a given image.
 
     :param preds:            Tensor of shape (K, NumJoints, 3) - Array of predicted skeletons.
                              Last dimension encode X,Y and confidence score of each joint
 
     :param pred_scores:      Tensor of shape (K) - Confidence scores for each pose
@@ -161,25 +169,28 @@
 
         :num_targets:       Number of groundtruth targets (total num targets minus number of ignored)
 
     """
     num_iou_thresholds = len(iou_thresholds)
 
     device = preds.device if torch.is_tensor(preds) else (targets.device if torch.is_tensor(targets) else "cpu")
-
-    if preds is None or len(preds) == 0:
-        preds_matched = torch.zeros((0, num_iou_thresholds), dtype=torch.bool, device=device)
-        preds_to_ignore = torch.zeros((0, num_iou_thresholds), dtype=torch.bool, device=device)
-        preds_scores = torch.zeros((0,), dtype=torch.float, device=device)
-        return preds_matched, preds_to_ignore, preds_scores, len(targets)
+    num_targets = len(targets) - torch.count_nonzero(targets_ignored)
 
     preds_matched = torch.zeros(len(preds), num_iou_thresholds, dtype=torch.bool, device=device)
     targets_matched = torch.zeros(len(targets), num_iou_thresholds, dtype=torch.bool, device=device)
     preds_to_ignore = torch.zeros(len(preds), num_iou_thresholds, dtype=torch.bool, device=device)
 
+    if preds is None or len(preds) == 0:
+        return ImageKeypointMatchingResult(
+            preds_matched=preds_matched,
+            preds_to_ignore=preds_to_ignore,
+            preds_scores=pred_scores,
+            num_targets=num_targets.item(),
+        )
+
     # Ignore all but the predictions that were top_k
     k = min(top_k, len(pred_scores))
     preds_idx_to_use = torch.topk(pred_scores, k=k, sorted=True, largest=True).indices
     preds_to_ignore[:, :] = True
     preds_to_ignore[preds_idx_to_use] = False
 
     if len(targets) > 0:
@@ -240,10 +251,13 @@
 
         # If a prediction has IoA higher than threshold (with any target of same class), then there is a match
         # shape = (n_preds_to_use x iou_thresholds)
         is_matching_with_crowd = best_ioa.view(-1, 1) > iou_thresholds.view(1, -1)
 
         preds_to_ignore[preds_idx_to_use] = torch.logical_or(preds_to_ignore[preds_idx_to_use], is_matching_with_crowd)
 
-    # return preds_matched, preds_to_ignore, pred_scores, len(targets)
-    num_targets = len(targets) - torch.count_nonzero(targets_ignored)
-    return preds_matched[preds_idx_to_use], preds_to_ignore[preds_idx_to_use], pred_scores[preds_idx_to_use], num_targets.item()
+    return ImageKeypointMatchingResult(
+        preds_matched=preds_matched[preds_idx_to_use],
+        preds_to_ignore=preds_to_ignore[preds_idx_to_use],
+        preds_scores=pred_scores[preds_idx_to_use],
+        num_targets=num_targets.item(),
+    )
```

## super_gradients/training/models/__init__.py

```diff
@@ -1,7 +1,9 @@
+import warnings
+
 from .sg_module import SgModule
 
 # Classification models
 from super_gradients.training.models.classification_models.beit import Beit, BeitLargePatch16_224, BeitBasePatch16_224
 from super_gradients.training.models.classification_models.densenet import DenseNet, CustomizedDensnet, DenseNet121, DenseNet161, DenseNet169, DenseNet201
 from super_gradients.training.models.classification_models.dpn import DPN, DPN26, DPN92
 from super_gradients.training.models.classification_models.efficientnet import (
@@ -29,14 +31,16 @@
     PreActResNet18,
     PreActResNet34,
     PreActResNet50,
     PreActResNet101,
     PreActResNet152,
 )
 from super_gradients.training.models.classification_models.resnet import (
+    Bottleneck as NewBottleneck,
+    BasicResNetBlock,
     ResNet,
     ResNet18,
     ResNet34,
     ResNet50,
     ResNet101,
     ResNet152,
     ResNet18Cifar,
@@ -105,33 +109,85 @@
     STDCClassification,
     STDC1Classification,
     STDCClassificationBase,
     STDC2Classification,
     STDCSegmentationBase,
     CustomSTDCSegmentation,
 )
+from super_gradients.training.models.segmentation_models.segformer import SegFormerB0, SegFormerB1, SegFormerB2, SegFormerB3, SegFormerB4, SegFormerB5
+from super_gradients.training.models.segmentation_models.ddrnet_backbones import DDRNet39Backbone
 
 # Pose estimation
-from super_gradients.training.models.pose_estimation_models.pose_ppyolo import PosePPYoloL
-from super_gradients.training.models.pose_estimation_models.pose_ddrnet39 import PoseDDRNet39
-from super_gradients.training.models.pose_estimation_models.dekr_hrnet import DEKRPoseEstimationModel, DEKRW32
+from super_gradients.training.models.pose_estimation_models.dekr_hrnet import DEKRPoseEstimationModel, DEKRW32NODC
 
 # KD
 from super_gradients.training.models.kd_modules.kd_module import KDModule
 
 import super_gradients.training.models.user_models as user_models
 from super_gradients.training.models.model_factory import get, get_model_name
 from super_gradients.training.models.arch_params_factory import get_arch_params
-from super_gradients.training.models.conversion import convert_to_onnx, convert_from_config
+from super_gradients.training.models.conversion import convert_to_coreml, convert_to_onnx, convert_from_config
 
 
 from super_gradients.common.object_names import Models
 from super_gradients.common.registry.registry import ARCHITECTURES
 
+from super_gradients.training.utils import make_divisible as _make_divisible_current_version, HpmStruct as CurrVersionHpmStruct
+
+
+def make_deprecated(func, reason):
+    def inner(*args, **kwargs):
+        with warnings.catch_warnings():
+            warnings.simplefilter("once", DeprecationWarning)
+            warnings.warn(reason, category=DeprecationWarning, stacklevel=2)
+        warnings.warn(reason, DeprecationWarning)
+        return func(*args, **kwargs)
+
+    return inner
+
+
+make_divisible = make_deprecated(
+    func=_make_divisible_current_version,
+    reason="You're importing `make_divisible` from `super_gradients.training.models`. This is deprecated since SuperGradients 3.1.0.\n"
+    "Please update your code to import it as follows:\n"
+    "[-] from super_gradients.training.models import make_divisible\n"
+    "[+] from super_gradients.training.utils import make_divisible\n",
+)
+
+
+BasicBlock = make_deprecated(
+    func=BasicResNetBlock,
+    reason="You're importing `BasicBlock` class from `super_gradients.training.models`. This is deprecated since SuperGradients 3.1.0.\n"
+    "This block was renamed to BasicResNetBlock for better clarity.\n"
+    "Please update your code to import it as follows:\n"
+    "[-] from super_gradients.training.models import BasicBlock\n"
+    "[+] from super_gradients.training.models import BasicResNetBlock\n",
+)
+
+Bottleneck = make_deprecated(
+    func=NewBottleneck,
+    reason="You're importing `Bottleneck` class from `super_gradients.training.models`. This is deprecated since SuperGradients 3.1.0.\n"
+    "This block was renamed to BasicResNetBlock for better clarity.\n"
+    "Please update your code to import it as follows:\n"
+    "[-] from super_gradients.training.models import Bottleneck\n"
+    "[+] from super_gradients.training.models.classification_models.resnet import Bottleneck\n",
+)
+
+HpmStruct = make_deprecated(
+    func=CurrVersionHpmStruct,
+    reason="You're importing `HpmStruct` class from `super_gradients.training.models`. This is deprecated since SuperGradients 3.1.0.\n"
+    "Please update your code to import it as follows:\n"
+    "[-] from super_gradients.training.models import HpmStruct\n"
+    "[+] from super_gradients.training.utils import HpmStruct\n",
+)
+
+
 __all__ = [
+    "HpmStruct",
+    "Bottleneck",
     "SPP",
     "YoloNAS_S",
     "YoloNAS_M",
     "YoloNAS_L",
     "YoloNASStage",
     "YoloNASUpStage",
     "YoloNASStem",
@@ -266,21 +322,30 @@
     "STDC2Seg",
     "STDCClassification",
     "STDC1Classification",
     "STDCClassificationBase",
     "STDC2Classification",
     "STDCSegmentationBase",
     "CustomSTDCSegmentation",
-    "PosePPYoloL",
-    "PoseDDRNet39",
     "DEKRPoseEstimationModel",
-    "DEKRW32",
+    "DEKRW32NODC",
     "KDModule",
     "get",
     "get_model_name",
     "get_arch_params",
+    "convert_to_coreml",
     "convert_to_onnx",
     "convert_from_config",
     "ARCHITECTURES",
     "Models",
     "user_models",
+    "SegFormerB0",
+    "SegFormerB1",
+    "SegFormerB2",
+    "SegFormerB3",
+    "SegFormerB4",
+    "SegFormerB5",
+    "DDRNet39Backbone",
+    "make_divisible",
+    "BasicResNetBlock",
+    "BasicBlock",
 ]
```

## super_gradients/training/models/conversion.py

```diff
@@ -1,30 +1,38 @@
+import os
+import pathlib
 from pathlib import Path
 
 import hydra
+import numpy as np
+import onnx
 import torch
 from omegaconf import DictConfig
-import numpy as np
+from onnxsim import simplify
 from torch.nn import Identity
 
 from super_gradients.common.abstractions.abstract_logger import get_logger
 from super_gradients.common.decorators.factory_decorator import resolve_param
+from super_gradients.common.environment.cfg_utils import load_experiment_cfg
+from super_gradients.common.environment.checkpoints_dir_utils import get_checkpoints_dir_path
 from super_gradients.common.factories.transforms_factory import TransformsFactory
 from super_gradients.training import models
-from super_gradients.common.environment.checkpoints_dir_utils import get_checkpoints_dir_path
-from super_gradients.common.environment.cfg_utils import load_experiment_cfg
 from super_gradients.training.utils.sg_trainer_utils import parse_args
-import os
-import pathlib
-
-from onnxsim import simplify
-import onnx
 
 logger = get_logger(__name__)
 
+ct = None
+
+try:
+    import coremltools as coreml_tools
+
+    ct = coreml_tools
+except (ImportError, ModuleNotFoundError):
+    pass
+
 
 class ConvertableCompletePipelineModel(torch.nn.Module):
     """
     Exportable nn.Module that wraps the model, preprocessing and postprocessing.
 
     :param model: torch.nn.Module, the main model. takes input from pre_process' output, and feeds pre_process.
     :param pre_process: torch.nn.Module, preprocessing module, its output will be model's input. When none (default), set to Identity().
@@ -46,14 +54,115 @@
 
     def forward(self, x):
         return self.post_process(self.model(self.pre_process(x)))
 
 
 @resolve_param("pre_process", TransformsFactory())
 @resolve_param("post_process", TransformsFactory())
+def convert_to_coreml(
+    model: torch.nn.Module,
+    out_path: str,
+    input_size: tuple = None,
+    pre_process: torch.nn.Module = None,
+    post_process: torch.nn.Module = None,
+    prep_model_for_conversion_kwargs=None,
+    export_as_ml_program=False,
+    torch_trace_kwargs=None,
+):
+    """
+        Exports a given SG model to CoreML mlprogram or package.
+
+        :param model: torch.nn.Module, model to export to CoreML.
+        :param out_path: str, destination path for the .mlmodel file.
+        :param input_size: Input shape without batch dimensions ([C,H,W]). Batch size assumed to be 1.
+        :param pre_process: torch.nn.Module, preprocessing pipeline, will be resolved by TransformsFactory()
+        :param post_process: torch.nn.Module, postprocessing pipeline, will be resolved by TransformsFactory()
+        :param prep_model_for_conversion_kwargs: dict, for SgModules- args to be passed to model.prep_model_for_conversion
+         prior to ct.convert call. Supported keys are:
+        - input_size - Shape of inputs with batch dimension, [C,H,W] for image inputs.
+        :param export_as_ml_program: Whether to convert to the new program format (better) or legacy coreml proto file
+                            (Supports more iOS versions and devices, but this format will be deprecated at some point).
+        :param torch_trace_kwargs: kwargs for torch.jit.trace
+    :return: Path
+    """
+    if ct is None:
+        raise ImportError(
+            '"coremltools" is required for CoreML export, but is not installed. Please install CoreML Tools using:\n'
+            '   "python3 -m pip install coremltools" and try again (Tested with version 6.3.0);'
+        )
+
+    logger.debug("Building model...")
+    logger.debug(model)
+    logger.debug("Model child nodes:")
+    logger.debug(next(model.named_children()))
+
+    if not os.path.isdir(pathlib.Path(out_path).parent.resolve()):
+        raise FileNotFoundError(f"Could not find destination directory {out_path} for the CoreML file.")
+    torch_trace_kwargs = torch_trace_kwargs or dict()
+    prep_model_for_conversion_kwargs = prep_model_for_conversion_kwargs or dict()
+
+    if input_size is not None:
+        input_size = (1, *input_size)
+        logger.warning(
+            f"input_shape is deprecated and will be removed in the next major release."
+            f"Use the convert_to_coreml(..., prep_model_for_conversion_kwargs(input_size={input_size})) instead"
+        )
+        prep_model_for_conversion_kwargs["input_size"] = input_size
+
+    if "input_size" not in prep_model_for_conversion_kwargs:
+        raise KeyError("input_size must be provided in prep_model_for_conversion_kwargs")
+
+    input_size = prep_model_for_conversion_kwargs["input_size"]
+
+    # TODO: support more than 1 input when prep_for_conversoin will support it.
+    example_inputs = [torch.Tensor(np.zeros(input_size))]
+
+    if not out_path.endswith(".mlpackage") and not out_path.endswith(".mlmodel"):
+        out_path += ".mlpackage" if export_as_ml_program else ".mlmodel"
+
+    complete_model = ConvertableCompletePipelineModel(model, pre_process, post_process, **prep_model_for_conversion_kwargs)
+
+    # Set the model in evaluation mode.
+    complete_model.eval()
+
+    logger.info("Creating torch jit trace...")
+    traced_model = torch.jit.trace(complete_model, example_inputs, **torch_trace_kwargs)
+    logger.info("Tracing the model with the provided inputs...")
+    out = traced_model(*example_inputs)  # using * because example_inputs is a list
+    logger.info(f"Inferred output shapes: {[o.shape for o in out]}")
+    if export_as_ml_program:
+        coreml_model = ct.convert(
+            traced_model, convert_to="mlprogram", inputs=[ct.ImageType(name=f"x_{i + 1}", shape=_.shape) for i, _ in enumerate(example_inputs)]
+        )
+    else:
+        coreml_model = ct.convert(traced_model, inputs=[ct.ImageType(name=f"x_{i + 1}", shape=_.shape) for i, _ in enumerate(example_inputs)])
+
+    spec = coreml_model.get_spec()
+    logger.debug(spec.description)
+
+    # Changing the input names:
+    #   In CoreML, the input name is compiled into classes (named keyword argument in predict).
+    #   We want to re-use the same names among different models to make research easier.
+    #   We normalize the inputs names to be x_1, x_2, etc.
+    for i, _input in enumerate(spec.description.input):
+        new_input_name = "x_" + str(i + 1)
+        logger.info(f"Renaming input {_input.name} to {new_input_name}")
+        ct.utils.rename_feature(spec, _input.name, new_input_name)
+
+    # Re-Initializing the model with the new spec
+    coreml_model = ct.models.MLModel(spec, weights_dir=coreml_model.weights_dir)
+
+    # Saving the model
+    coreml_model.save(out_path)
+    logger.info(f"CoreML model successfully save to {os.path.abspath(out_path)}")
+    return out_path
+
+
+@resolve_param("pre_process", TransformsFactory())
+@resolve_param("post_process", TransformsFactory())
 def convert_to_onnx(
     model: torch.nn.Module,
     out_path: str,
     input_shape: tuple = None,
     pre_process: torch.nn.Module = None,
     post_process: torch.nn.Module = None,
     prep_model_for_conversion_kwargs=None,
@@ -61,38 +170,46 @@
     simplify: bool = True,
 ):
     """
     Exports model to ONNX.
 
     :param model: torch.nn.Module, model to export to ONNX.
     :param out_path: str, destination path for the .onnx file.
-    :param input_shape: DEPRECATED USE input_size KWARG IN prep_model_for_conversion_kwargs INSTEAD.
+    :param input_shape: Input shape without batch dimensions ([C,H,W]). Batch size assumed to be 1.
+    DEPRECATED USE input_size KWARG IN prep_model_for_conversion_kwargs INSTEAD.
     :param pre_process: torch.nn.Module, preprocessing pipeline, will be resolved by TransformsFactory()
     :param post_process: torch.nn.Module, postprocessing pipeline, will be resolved by TransformsFactory()
     :param prep_model_for_conversion_kwargs: dict, for SgModules- args to be passed to model.prep_model_for_conversion
-     prior to torch.onnx.export call.
+     prior to torch.onnx.export call. Supported keys are:
+    - input_size - Shape of inputs with batch dimension, [C,H,W] for image inputs.
     :param torch_onnx_export_kwargs: kwargs (EXCLUDING: FIRST 3 KWARGS- MODEL, F, ARGS). to be unpacked in torch.onnx.export call
     :param simplify: bool,whether to apply onnx simplifier method, same as `python -m onnxsim onnx_path onnx_sim_path.
      When true, the simplified model will be saved in out_path (default=True).
 
     :return: out_path
     """
     if not os.path.isdir(pathlib.Path(out_path).parent.resolve()):
         raise FileNotFoundError(f"Could not find destination directory {out_path} for the ONNX file.")
     torch_onnx_export_kwargs = torch_onnx_export_kwargs or dict()
     prep_model_for_conversion_kwargs = prep_model_for_conversion_kwargs or dict()
 
     if input_shape is not None:
+        input_size = (1, *input_shape)
         logger.warning(
-            "input_shape is deprecated and will be removed in the next major release." " Use the input_size kwarg in prep_model_for_conversion_kwargs instead"
+            f"input_shape is deprecated and will be removed in the next major release."
+            f"Use the convert_to_onnx(..., prep_model_for_conversion_kwargs(input_size={input_size})) instead"
         )
+        prep_model_for_conversion_kwargs["input_size"] = input_size
+
+    if "input_size" not in prep_model_for_conversion_kwargs:
+        raise KeyError("input_size must be provided in prep_model_for_conversion_kwargs")
 
-    prep_model_for_conversion_kwargs["input_size"] = (1, *input_shape)
+    input_size = prep_model_for_conversion_kwargs["input_size"]
 
-    onnx_input = torch.Tensor(np.zeros([1, *input_shape]))
+    onnx_input = torch.Tensor(np.zeros(input_size))
     if not out_path.endswith(".onnx"):
         out_path = out_path + ".onnx"
     complete_model = ConvertableCompletePipelineModel(model, pre_process, post_process, **prep_model_for_conversion_kwargs)
 
     torch.onnx.export(model=complete_model, args=onnx_input, f=out_path, **torch_onnx_export_kwargs)
     if simplify:
         onnx_simplify(out_path, out_path)
```

## super_gradients/training/models/model_factory.py

```diff
@@ -173,15 +173,15 @@
     """
     :param model_name:          Defines the model's architecture from models/ALL_ARCHITECTURES
     :param arch_params:         Architecture hyper parameters. e.g.: block, num_blocks, etc.
     :param num_classes:         Number of classes (defines the net's structure).
                                     If None is given, will try to derrive from pretrained_weight's corresponding dataset.
     :param strict_load:         See super_gradients.common.data_types.enum.strict_load.StrictLoad class documentation for details
                                     (default=NO_KEY_MATCHING to suport SG trained checkpoints)
-    :param checkpoint_path:     The path to the external checkpoint to be loaded. Can be absolute or relative (ie: path/to/checkpoint.pth).
+    :param checkpoint_path:     The path to the external checkpoint to be loaded. Can be absolute or relative (ie: path/to/checkpoint.pth) path or URL.
                                     If provided, will automatically attempt to load the checkpoint.
     :param pretrained_weights:  Describe the dataset of the pretrained weights (for example "imagenent").
     :param load_backbone:       Load the provided checkpoint to model.backbone instead of model.
     :param download_required_code: if model is not found in SG and is downloaded from a remote client, overriding this parameter with False
                                     will prevent additional code from being downloaded. This affects only models from remote client.
     :param checkpoint_num_classes:  num_classes of checkpoint_path/ pretrained_weights, when checkpoint_path is not None.
      Used when num_classes != checkpoint_num_class. In this case, the module will be initialized with checkpoint_num_class, then weights will be loaded. Finaly
```

## super_gradients/training/models/prediction_results.py

```diff
@@ -62,15 +62,15 @@
         :param color_mapping:   List of tuples representing the colors for each class.
                                 Default is None, which generates a default color mapping based on the number of class names.
         :return:                Image with predicted bboxes. Note that this does not modify the original image.
         """
         image = self.image.copy()
         color_mapping = color_mapping or generate_color_mapping(len(self.class_names))
 
-        for pred_i in range(len(self.prediction)):
+        for pred_i in np.argsort(self.prediction.confidence):
 
             class_id = int(self.prediction.labels[pred_i])
             score = "" if not show_confidence else str(round(self.prediction.confidence[pred_i], 2))
 
             image = draw_bbox(
                 image=image,
                 title=f"{self.class_names[class_id]} {score}",
```

## super_gradients/training/models/classification_models/resnet.py

```diff
@@ -18,17 +18,17 @@
 from super_gradients.training.models import SgModule
 from super_gradients.training.utils import get_param
 from super_gradients.training.utils.regularization_utils import DropPath
 from super_gradients.common.registry.registry import register_model
 from super_gradients.common.object_names import Models
 
 
-class BasicBlock(nn.Module):
+class BasicResNetBlock(nn.Module):
     def __init__(self, in_planes, planes, stride=1, expansion=1, final_relu=True, droppath_prob=0.0):
-        super(BasicBlock, self).__init__()
+        super(BasicResNetBlock, self).__init__()
         self.expansion = expansion
         self.conv1 = nn.Conv2d(in_planes, planes, kernel_size=3, stride=stride, padding=1, bias=False)
         self.bn1 = nn.BatchNorm2d(planes)
         self.conv2 = nn.Conv2d(planes, planes, kernel_size=3, stride=1, padding=1, bias=False)
         self.bn2 = nn.BatchNorm2d(planes)
         self.final_relu = final_relu
 
@@ -232,33 +232,33 @@
             self.linear = nn.Linear(width_multiplier(512, self.width_mult) * self.expansion, new_num_classes)
 
 
 @register_model(Models.RESNET18)
 class ResNet18(ResNet):
     def __init__(self, arch_params, num_classes=None):
         super().__init__(
-            BasicBlock,
+            BasicResNetBlock,
             [2, 2, 2, 2],
             num_classes=num_classes or arch_params.num_classes,
             droppath_prob=get_param(arch_params, "droppath_prob", 0),
             backbone_mode=get_param(arch_params, "backbone_mode", False),
         )
 
 
 @register_model(Models.RESNET18_CIFAR)
 class ResNet18Cifar(CifarResNet):
     def __init__(self, arch_params, num_classes=None):
-        super().__init__(BasicBlock, [2, 2, 2, 2], num_classes=num_classes or arch_params.num_classes)
+        super().__init__(BasicResNetBlock, [2, 2, 2, 2], num_classes=num_classes or arch_params.num_classes)
 
 
 @register_model(Models.RESNET34)
 class ResNet34(ResNet):
     def __init__(self, arch_params, num_classes=None):
         super().__init__(
-            BasicBlock,
+            BasicResNetBlock,
             [3, 4, 6, 3],
             num_classes=num_classes or arch_params.num_classes,
             droppath_prob=get_param(arch_params, "droppath_prob", 0),
             backbone_mode=get_param(arch_params, "backbone_mode", False),
         )
 
 
@@ -313,28 +313,28 @@
             expansion=4,
         )
 
 
 @register_model(Models.CUSTOM_RESNET_CIFAR)
 class CustomizedResnetCifar(CifarResNet):
     def __init__(self, arch_params, num_classes=None):
-        super().__init__(BasicBlock, arch_params.structure, width_mult=arch_params.width_mult, num_classes=num_classes or arch_params.num_classes)
+        super().__init__(BasicResNetBlock, arch_params.structure, width_mult=arch_params.width_mult, num_classes=num_classes or arch_params.num_classes)
 
 
 @register_model(Models.CUSTOM_RESNET50_CIFAR)
 class CustomizedResnet50Cifar(CifarResNet):
     def __init__(self, arch_params, num_classes=None):
         super().__init__(Bottleneck, arch_params.structure, width_mult=arch_params.width_mult, num_classes=num_classes or arch_params.num_classes, expansion=4)
 
 
 @register_model(Models.CUSTOM_RESNET)
 class CustomizedResnet(ResNet):
     def __init__(self, arch_params, num_classes=None):
         super().__init__(
-            BasicBlock,
+            BasicResNetBlock,
             arch_params.structure,
             width_mult=arch_params.width_mult,
             num_classes=num_classes or arch_params.num_classes,
             droppath_prob=get_param(arch_params, "droppath_prob", 0),
             backbone_mode=get_param(arch_params, "backbone_mode", False),
         )
```

## super_gradients/training/models/detection_models/customizable_detector.py

```diff
@@ -2,23 +2,25 @@
 A base for a detection network built according to the following scheme:
  * constructed from nested arch_params;
  * inside arch_params each nested level (module) has an explicit type and its required parameters
  * each module accepts in_channels and other parameters
  * each module defines out_channels property on construction
 """
 from typing import Union, Optional, List
+from functools import lru_cache
 
+import torch
 from torch import nn
 from omegaconf import DictConfig
 
 from super_gradients.common.decorators.factory_decorator import resolve_param
 from super_gradients.common.factories.processing_factory import ProcessingFactory
 from super_gradients.module_interfaces import SupportsReplaceNumClasses
 from super_gradients.modules.head_replacement_utils import replace_num_classes_with_random_weights
-from super_gradients.training.utils.utils import HpmStruct
+from super_gradients.training.utils.utils import HpmStruct, arch_params_deprecated
 from super_gradients.training.models.sg_module import SgModule
 import super_gradients.common.factories.detection_modules_factory as det_factory
 from super_gradients.training.models.prediction_results import ImagesDetectionPrediction
 from super_gradients.training.pipelines.pipelines import DetectionPipeline
 from super_gradients.training.processing.processing import Processing
 from super_gradients.training.utils.detection_utils import DetectionPostPredictionCallback
 from super_gradients.training.utils.media.image import ImageSource
@@ -27,14 +29,15 @@
 class CustomizableDetector(SgModule):
     """
     A customizable detector with backbone -> neck -> heads
     Each submodule with its parameters must be defined explicitly.
     Modules should follow the interface of BaseDetectionModule
     """
 
+    @arch_params_deprecated
     def __init__(
         self,
         backbone: Union[str, dict, HpmStruct, DictConfig],
         heads: Union[str, dict, HpmStruct, DictConfig],
         neck: Optional[Union[str, dict, HpmStruct, DictConfig]] = None,
         num_classes: int = None,
         bn_eps: Optional[float] = None,
@@ -132,50 +135,59 @@
         :param conf:            (Optional) Below the confidence threshold, prediction are discarded
         """
         self._class_names = class_names or self._class_names
         self._image_processor = image_processor or self._image_processor
         self._default_nms_iou = iou or self._default_nms_iou
         self._default_nms_conf = conf or self._default_nms_conf
 
-    def _get_pipeline(self, iou: Optional[float] = None, conf: Optional[float] = None) -> DetectionPipeline:
+    @lru_cache(maxsize=1)
+    def _get_pipeline(self, iou: Optional[float] = None, conf: Optional[float] = None, fuse_model: bool = True) -> DetectionPipeline:
         """Instantiate the prediction pipeline of this model.
 
         :param iou:     (Optional) IoU threshold for the nms algorithm. If None, the default value associated to the training is used.
         :param conf:    (Optional) Below the confidence threshold, prediction are discarded.
                         If None, the default value associated to the training is used.
+        :param fuse_model: If True, create a copy of the model, and fuse some of its layers to increase performance. This increases memory usage.
         """
         if None in (self._class_names, self._image_processor, self._default_nms_iou, self._default_nms_conf):
             raise RuntimeError(
                 "You must set the dataset processing parameters before calling predict.\n" "Please call `model.set_dataset_processing_params(...)` first."
             )
 
         iou = iou or self._default_nms_iou
         conf = conf or self._default_nms_conf
-
         pipeline = DetectionPipeline(
             model=self,
             image_processor=self._image_processor,
             post_prediction_callback=self.get_post_prediction_callback(iou=iou, conf=conf),
             class_names=self._class_names,
+            fuse_model=fuse_model,
         )
         return pipeline
 
-    def predict(self, images: ImageSource, iou: Optional[float] = None, conf: Optional[float] = None) -> ImagesDetectionPrediction:
+    def predict(self, images: ImageSource, iou: Optional[float] = None, conf: Optional[float] = None, fuse_model: bool = True) -> ImagesDetectionPrediction:
         """Predict an image or a list of images.
 
         :param images:  Images to predict.
         :param iou:     (Optional) IoU threshold for the nms algorithm. If None, the default value associated to the training is used.
         :param conf:    (Optional) Below the confidence threshold, prediction are discarded.
                         If None, the default value associated to the training is used.
+        :param fuse_model: If True, create a copy of the model, and fuse some of its layers to increase performance. This increases memory usage.
         """
-        pipeline = self._get_pipeline(iou=iou, conf=conf)
+        pipeline = self._get_pipeline(iou=iou, conf=conf, fuse_model=fuse_model)
         return pipeline(images)  # type: ignore
 
-    def predict_webcam(self, iou: Optional[float] = None, conf: Optional[float] = None):
+    def predict_webcam(self, iou: Optional[float] = None, conf: Optional[float] = None, fuse_model: bool = True):
         """Predict using webcam.
 
         :param iou:     (Optional) IoU threshold for the nms algorithm. If None, the default value associated to the training is used.
         :param conf:    (Optional) Below the confidence threshold, prediction are discarded.
                         If None, the default value associated to the training is used.
+        :param fuse_model: If True, create a copy of the model, and fuse some of its layers to increase performance. This increases memory usage.
         """
-        pipeline = self._get_pipeline(iou=iou, conf=conf)
+        pipeline = self._get_pipeline(iou=iou, conf=conf, fuse_model=fuse_model)
         pipeline.predict_webcam()
+
+    def train(self, mode: bool = True):
+        self._get_pipeline.cache_clear()
+        torch.cuda.empty_cache()
+        return super().train(mode)
```

## super_gradients/training/models/detection_models/yolo_base.py

```diff
@@ -1,9 +1,10 @@
 import math
 from typing import Union, Type, List, Tuple, Optional
+from functools import lru_cache
 
 import torch
 import torch.nn as nn
 
 from super_gradients.common.decorators.factory_decorator import resolve_param
 from super_gradients.common.factories.processing_factory import ProcessingFactory
 from super_gradients.modules import CrossModelSkipConnection, Conv
@@ -14,14 +15,15 @@
 from super_gradients.training.utils.detection_utils import non_max_suppression, matrix_non_max_suppression, NMS_Type, DetectionPostPredictionCallback, Anchors
 from super_gradients.training.utils.utils import HpmStruct, check_img_size_divisibility, get_param
 from super_gradients.training.models.prediction_results import ImagesDetectionPrediction
 from super_gradients.training.pipelines.pipelines import DetectionPipeline
 from super_gradients.training.processing.processing import Processing
 from super_gradients.training.utils.media.image import ImageSource
 
+
 COCO_DETECTION_80_CLASSES_BBOX_ANCHORS = Anchors(
     [[10, 13, 16, 30, 33, 23], [30, 61, 62, 45, 59, 119], [116, 90, 156, 198, 373, 326]], strides=[8, 16, 32]
 )  # output strides of all yolo outputs
 
 ANCHORSLESS_DUMMY_ANCHORS = Anchors([[0, 0], [0, 0], [0, 0]], strides=[8, 16, 32])
 
 
@@ -443,58 +445,68 @@
         :param conf:            (Optional) Below the confidence threshold, prediction are discarded
         """
         self._class_names = class_names or self._class_names
         self._image_processor = image_processor or self._image_processor
         self._default_nms_iou = iou or self._default_nms_iou
         self._default_nms_conf = conf or self._default_nms_conf
 
-    def _get_pipeline(self, iou: Optional[float] = None, conf: Optional[float] = None) -> DetectionPipeline:
+    @lru_cache(maxsize=1)
+    def _get_pipeline(self, iou: Optional[float] = None, conf: Optional[float] = None, fuse_model: bool = True) -> DetectionPipeline:
         """Instantiate the prediction pipeline of this model.
 
         :param iou:     (Optional) IoU threshold for the nms algorithm. If None, the default value associated to the training is used.
         :param conf:    (Optional) Below the confidence threshold, prediction are discarded.
                         If None, the default value associated to the training is used.
+        :param fuse_model: If True, create a copy of the model, and fuse some of its layers to increase performance. This increases memory usage.
         """
         if None in (self._class_names, self._image_processor, self._default_nms_iou, self._default_nms_conf):
             raise RuntimeError(
                 "You must set the dataset processing parameters before calling predict.\n" "Please call `model.set_dataset_processing_params(...)` first."
             )
 
         iou = iou or self._default_nms_iou
         conf = conf or self._default_nms_conf
 
         pipeline = DetectionPipeline(
             model=self,
             image_processor=self._image_processor,
             post_prediction_callback=self.get_post_prediction_callback(iou=iou, conf=conf),
             class_names=self._class_names,
+            fuse_model=fuse_model,
         )
         return pipeline
 
-    def predict(self, images: ImageSource, iou: Optional[float] = None, conf: Optional[float] = None) -> ImagesDetectionPrediction:
+    def predict(self, images: ImageSource, iou: Optional[float] = None, conf: Optional[float] = None, fuse_model: bool = True) -> ImagesDetectionPrediction:
         """Predict an image or a list of images.
 
         :param images:  Images to predict.
         :param iou:     (Optional) IoU threshold for the nms algorithm. If None, the default value associated to the training is used.
         :param conf:    (Optional) Below the confidence threshold, prediction are discarded.
                         If None, the default value associated to the training is used.
+        :param fuse_model: If True, create a copy of the model, and fuse some of its layers to increase performance. This increases memory usage.
         """
-        pipeline = self._get_pipeline(iou=iou, conf=conf)
+        pipeline = self._get_pipeline(iou=iou, conf=conf, fuse_model=fuse_model)
         return pipeline(images)  # type: ignore
 
-    def predict_webcam(self, iou: Optional[float] = None, conf: Optional[float] = None):
+    def predict_webcam(self, iou: Optional[float] = None, conf: Optional[float] = None, fuse_model: bool = True):
         """Predict using webcam.
 
         :param iou:     (Optional) IoU threshold for the nms algorithm. If None, the default value associated to the training is used.
         :param conf:    (Optional) Below the confidence threshold, prediction are discarded.
                         If None, the default value associated to the training is used.
+        :param fuse_model: If True, create a copy of the model, and fuse some of its layers to increase performance. This increases memory usage.
         """
-        pipeline = self._get_pipeline(iou=iou, conf=conf)
+        pipeline = self._get_pipeline(iou=iou, conf=conf, fuse_model=fuse_model)
         pipeline.predict_webcam()
 
+    def train(self, mode: bool = True):
+        self._get_pipeline.cache_clear()
+        torch.cuda.empty_cache()
+        return super().train(mode)
+
     def forward(self, x):
         out = self._backbone(x)
         out = self._head(out)
         # THIS HAS NO EFFECT IF add_nms() WAS NOT DONE
         out = self._nms(out)
         return out
```

## super_gradients/training/models/detection_models/pp_yolo_e/pp_yolo_e.py

```diff
@@ -1,9 +1,11 @@
 from typing import Union, Optional, List
+from functools import lru_cache
 
+import torch
 from torch import Tensor
 
 from super_gradients.common.decorators.factory_decorator import resolve_param
 from super_gradients.common.factories.processing_factory import ProcessingFactory
 from super_gradients.common.registry.registry import register_model
 from super_gradients.common.object_names import Models
 from super_gradients.modules import RepVGGBlock
@@ -55,20 +57,22 @@
         :param conf:            (Optional) Below the confidence threshold, prediction are discarded
         """
         self._class_names = class_names or self._class_names
         self._image_processor = image_processor or self._image_processor
         self._default_nms_iou = iou or self._default_nms_iou
         self._default_nms_conf = conf or self._default_nms_conf
 
-    def _get_pipeline(self, iou: Optional[float] = None, conf: Optional[float] = None) -> DetectionPipeline:
+    @lru_cache(maxsize=1)
+    def _get_pipeline(self, iou: Optional[float] = None, conf: Optional[float] = None, fuse_model: bool = True) -> DetectionPipeline:
         """Instantiate the prediction pipeline of this model.
 
         :param iou:     (Optional) IoU threshold for the nms algorithm. If None, the default value associated to the training is used.
         :param conf:    (Optional) Below the confidence threshold, prediction are discarded.
                         If None, the default value associated to the training is used.
+        :param fuse_model: If True, create a copy of the model, and fuse some of its layers to increase performance. This increases memory usage.
         """
         if None in (self._class_names, self._image_processor, self._default_nms_iou, self._default_nms_conf):
             raise RuntimeError(
                 "You must set the dataset processing parameters before calling predict.\n" "Please call `model.set_dataset_processing_params(...)` first."
             )
 
         iou = iou or self._default_nms_iou
@@ -78,35 +82,42 @@
             model=self,
             image_processor=self._image_processor,
             post_prediction_callback=self.get_post_prediction_callback(iou=iou, conf=conf),
             class_names=self._class_names,
         )
         return pipeline
 
-    def predict(self, images: ImageSource, iou: Optional[float] = None, conf: Optional[float] = None) -> ImagesDetectionPrediction:
+    def predict(self, images: ImageSource, iou: Optional[float] = None, conf: Optional[float] = None, fuse_model: bool = True) -> ImagesDetectionPrediction:
         """Predict an image or a list of images.
 
         :param images:  Images to predict.
         :param iou:     (Optional) IoU threshold for the nms algorithm. If None, the default value associated to the training is used.
         :param conf:    (Optional) Below the confidence threshold, prediction are discarded.
                         If None, the default value associated to the training is used.
+        :param fuse_model: If True, create a copy of the model, and fuse some of its layers to increase performance. This increases memory usage.
         """
-        pipeline = self._get_pipeline(iou=iou, conf=conf)
+        pipeline = self._get_pipeline(iou=iou, conf=conf, fuse_model=fuse_model)
         return pipeline(images)  # type: ignore
 
-    def predict_webcam(self, iou: Optional[float] = None, conf: Optional[float] = None):
+    def predict_webcam(self, iou: Optional[float] = None, conf: Optional[float] = None, fuse_model: bool = True):
         """Predict using webcam.
 
         :param iou:     (Optional) IoU threshold for the nms algorithm. If None, the default value associated to the training is used.
         :param conf:    (Optional) Below the confidence threshold, prediction are discarded.
                         If None, the default value associated to the training is used.
+        :param fuse_model: If True, create a copy of the model, and fuse some of its layers to increase performance. This increases memory usage.
         """
-        pipeline = self._get_pipeline(iou=iou, conf=conf)
+        pipeline = self._get_pipeline(iou=iou, conf=conf, fuse_model=fuse_model)
         pipeline.predict_webcam()
 
+    def train(self, mode: bool = True):
+        self._get_pipeline.cache_clear()
+        torch.cuda.empty_cache()
+        return super().train(mode)
+
     def forward(self, x: Tensor):
         features = self.backbone(x)
         features = self.neck(features)
         return self.head(features)
 
     def prep_model_for_conversion(self, input_size: Union[tuple, list] = None, **kwargs):
         """
```

## super_gradients/training/models/detection_models/yolo_nas/yolo_nas_variants.py

```diff
@@ -10,24 +10,24 @@
 from super_gradients.training.utils import HpmStruct, get_param
 
 from super_gradients.training.models.detection_models.pp_yolo_e import PPYoloEPostPredictionCallback
 
 
 @register_model(Models.YOLO_NAS_S)
 class YoloNAS_S(CustomizableDetector):
-    def __init__(self, arch_params: Union[HpmStruct, DictConfig], in_channels: int = 3):
+    def __init__(self, arch_params: Union[HpmStruct, DictConfig]):
         default_arch_params = get_arch_params("yolo_nas_s_arch_params")
         merged_arch_params = HpmStruct(**copy.deepcopy(default_arch_params))
         merged_arch_params.override(**arch_params.to_dict())
         super().__init__(
             backbone=merged_arch_params.backbone,
             neck=merged_arch_params.neck,
             heads=merged_arch_params.heads,
             num_classes=get_param(merged_arch_params, "num_classes", None),
-            in_channels=in_channels,
+            in_channels=get_param(merged_arch_params, "in_channels", 3),
             bn_momentum=get_param(merged_arch_params, "bn_momentum", None),
             bn_eps=get_param(merged_arch_params, "bn_eps", None),
             inplace_act=get_param(merged_arch_params, "inplace_act", None),
         )
 
     @staticmethod
     def get_post_prediction_callback(conf: float, iou: float) -> PPYoloEPostPredictionCallback:
@@ -36,24 +36,24 @@
     @property
     def num_classes(self):
         return self.heads.num_classes
 
 
 @register_model(Models.YOLO_NAS_M)
 class YoloNAS_M(CustomizableDetector):
-    def __init__(self, arch_params: Union[HpmStruct, DictConfig], in_channels: int = 3):
+    def __init__(self, arch_params: Union[HpmStruct, DictConfig]):
         default_arch_params = get_arch_params("yolo_nas_m_arch_params")
         merged_arch_params = HpmStruct(**copy.deepcopy(default_arch_params))
         merged_arch_params.override(**arch_params.to_dict())
         super().__init__(
             backbone=merged_arch_params.backbone,
             neck=merged_arch_params.neck,
             heads=merged_arch_params.heads,
             num_classes=get_param(merged_arch_params, "num_classes", None),
-            in_channels=in_channels,
+            in_channels=get_param(merged_arch_params, "in_channels", 3),
             bn_momentum=get_param(merged_arch_params, "bn_momentum", None),
             bn_eps=get_param(merged_arch_params, "bn_eps", None),
             inplace_act=get_param(merged_arch_params, "inplace_act", None),
         )
 
     @staticmethod
     def get_post_prediction_callback(conf: float, iou: float) -> PPYoloEPostPredictionCallback:
@@ -62,24 +62,24 @@
     @property
     def num_classes(self):
         return self.heads.num_classes
 
 
 @register_model(Models.YOLO_NAS_L)
 class YoloNAS_L(CustomizableDetector):
-    def __init__(self, arch_params: Union[HpmStruct, DictConfig], in_channels: int = 3):
+    def __init__(self, arch_params: Union[HpmStruct, DictConfig]):
         default_arch_params = get_arch_params("yolo_nas_l_arch_params")
         merged_arch_params = HpmStruct(**copy.deepcopy(default_arch_params))
         merged_arch_params.override(**arch_params.to_dict())
         super().__init__(
             backbone=merged_arch_params.backbone,
             neck=merged_arch_params.neck,
             heads=merged_arch_params.heads,
             num_classes=get_param(merged_arch_params, "num_classes", None),
-            in_channels=in_channels,
+            in_channels=get_param(merged_arch_params, "in_channels", 3),
             bn_momentum=get_param(merged_arch_params, "bn_momentum", None),
             bn_eps=get_param(merged_arch_params, "bn_eps", None),
             inplace_act=get_param(merged_arch_params, "inplace_act", None),
         )
 
     @staticmethod
     def get_post_prediction_callback(conf: float, iou: float) -> PPYoloEPostPredictionCallback:
```

## super_gradients/training/models/pose_estimation_models/__init__.py

```diff
@@ -0,0 +1,12 @@
+00000000: 6672 6f6d 202e 7265 7363 6f72 696e 675f  from .rescoring_
+00000010: 6e65 7420 696d 706f 7274 2050 6f73 6552  net import PoseR
+00000020: 6573 636f 7269 6e67 4e65 740a 6672 6f6d  escoringNet.from
+00000030: 202e 6465 6b72 5f68 726e 6574 2069 6d70   .dekr_hrnet imp
+00000040: 6f72 7420 4445 4b52 506f 7365 4573 7469  ort DEKRPoseEsti
+00000050: 6d61 7469 6f6e 4d6f 6465 6c2c 2044 454b  mationModel, DEK
+00000060: 5257 3332 4e4f 4443 0a0a 5f5f 616c 6c5f  RW32NODC..__all_
+00000070: 5f20 3d20 5b22 506f 7365 5265 7363 6f72  _ = ["PoseRescor
+00000080: 696e 674e 6574 222c 2022 4445 4b52 506f  ingNet", "DEKRPo
+00000090: 7365 4573 7469 6d61 7469 6f6e 4d6f 6465  seEstimationMode
+000000a0: 6c22 2c20 2244 454b 5257 3332 4e4f 4443  l", "DEKRW32NODC
+000000b0: 225d 0a                                  "].
```

## super_gradients/training/models/pose_estimation_models/dekr_hrnet.py

```diff
@@ -20,15 +20,15 @@
 
 from super_gradients.common.registry.registry import register_model
 from super_gradients.common.object_names import Models
 from super_gradients.common.abstractions.abstract_logger import get_logger
 from super_gradients.training.models.sg_module import SgModule
 from super_gradients.training.models.arch_params_factory import get_arch_params
 
-__all__ = ["DEKRPoseEstimationModel", "DEKRW32"]
+__all__ = ["DEKRPoseEstimationModel", "DEKRW32NODC"]
 
 from super_gradients.training.utils import HpmStruct
 
 logger = get_logger(__name__)
 
 
 class BasicBlock(nn.Module):
@@ -521,16 +521,67 @@
                     nn.init.constant_(m.translation_conv.bias, 0)
 
 
 POSE_DEKR_W32_NO_DC_ARCH_PARAMS = get_arch_params("pose_dekr_w32_no_dc_arch_params")
 
 
 @register_model(Models.DEKR_W32_NO_DC)
-class DEKRW32(DEKRPoseEstimationModel):
+class DEKRW32NODC(DEKRPoseEstimationModel):
     """
     DEKR-W32 model for pose estimation without deformable convolutions.
     """
 
     def __init__(self, arch_params):
         merged_arch_params = HpmStruct(**copy.deepcopy(POSE_DEKR_W32_NO_DC_ARCH_PARAMS))
         merged_arch_params.override(**arch_params.to_dict())
         super().__init__(merged_arch_params)
+
+
+class DEKRWrapper(nn.Module):
+    def __init__(self, model: DEKRPoseEstimationModel, apply_sigmoid=False):
+        super().__init__()
+        self.model = model
+        self.apply_sigmoid = apply_sigmoid
+
+    def forward(self, inputs):
+        heatmap, offsets = self.model(inputs)
+
+        if self.apply_sigmoid:
+            heatmap = torch.sigmoid(heatmap)
+
+        return heatmap, offsets
+
+
+class DEKRHorisontalFlipWrapper(nn.Module):
+    def __init__(self, model: DEKRPoseEstimationModel, flip_indexes_heatmap, flip_indexes_offset, apply_sigmoid=False):
+        super().__init__()
+        self.model = model
+        self.flip_indexes_heatmap = torch.tensor(flip_indexes_heatmap).long()
+        self.flip_indexes_offset = torch.tensor(flip_indexes_offset).long()
+        self.apply_sigmoid = apply_sigmoid
+
+    def forward(self, inputs):
+
+        input_flip = inputs.flip(3)
+        input_flip[:, :, :, :-3] = input_flip[:, :, :, 3:]
+
+        heatmap, offsets = self.model(inputs)
+        heatmap_flip, offset_flip = self.model(input_flip)
+
+        heatmap_deaugment = heatmap_flip[:, self.flip_indexes_heatmap, :, :]
+
+        batch_size, num_offsets, rows, cols = offset_flip.size()
+
+        offset_flip = offset_flip.reshape(offset_flip.size(0), offset_flip.size(1) // 2, 2, offset_flip.size(2), offset_flip.size(3))
+        offset_flip = offset_flip[:, self.flip_indexes_offset, :, :, :]
+        offset_flip[:, :, 0, :, :] *= -1
+
+        offset_deaugment = offset_flip.reshape(batch_size, num_offsets, rows, cols)
+
+        if self.apply_sigmoid:
+            heatmap = torch.sigmoid(heatmap)
+            heatmap_deaugment = torch.sigmoid(heatmap_deaugment)
+
+        averaged_heatmap = (heatmap + heatmap_deaugment.flip(3)) * 0.5
+        averaged_offsets = (offsets + offset_deaugment.flip(3)) * 0.5
+
+        return averaged_heatmap, averaged_offsets
```

## super_gradients/training/models/segmentation_models/ddrnet.py

```diff
@@ -1,15 +1,17 @@
+import warnings
+
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from collections import OrderedDict
 
 from super_gradients.common.registry.registry import register_model
 from super_gradients.common.object_names import Models
-from super_gradients.training.models.classification_models.resnet import BasicBlock, Bottleneck
+from super_gradients.training.models.classification_models.resnet import BasicResNetBlock, Bottleneck
 from super_gradients.training.models.segmentation_models.segmentation_module import SegmentationModule
 from super_gradients.training.utils import get_param, HpmStruct
 
 """
 paper: Deep Dual-resolution Networks for Real-time and
 Accurate Semantic Segmentation of Road Scenes ( https://arxiv.org/pdf/2101.06085.pdf )
 code from git repo: https://github.com/ydhongHIT/DDRNet
@@ -208,15 +210,15 @@
         output_shapes["layer3"] = x.shape[1]
         x = self.layer4(x)
         output_shapes["layer4"] = x.shape[1]
         return output_shapes
 
 
 class BasicDDRBackBone(DDRBackBoneBase):
-    def __init__(self, block: nn.Module.__class__, width: int, layers: list, input_channels: int, layer3_repeats: int):
+    def __init__(self, block: nn.Module.__class__, width: int, layers: list, input_channels: int, layer3_repeats: int = 1):
         super().__init__()
         self.input_channels = input_channels
         self.stem = nn.Sequential(
             ConvBN(in_channels=input_channels, out_channels=width, kernel_size=3, stride=2, padding=1, add_relu=True),
             ConvBN(in_channels=width, out_channels=width, kernel_size=3, stride=2, padding=1, add_relu=True),
         )
         self.layer1 = _make_layer(block=block, in_planes=width, planes=width, num_blocks=layers[0])
@@ -503,39 +505,50 @@
                 multiply_lr_params[name] = param
         return multiply_lr_params.items(), no_multiply_params.items()
 
 
 class DDRNetCustom(DDRNet):
     def __init__(self, arch_params: HpmStruct):
         """Parse arch_params and translate the parameters to build the original DDRNet architecture"""
+        if get_param(arch_params, "aux_heads") is not None:
+            message = "arch_params.aux_heads is deprecated in 3.1.1 and will be removed in 3.2.0."
+            if get_param(arch_params, "use_aux_heads") is not None:
+                message += "\n using arch_params.use_aux_heads instead."
+
+            else:
+                message += "\n use arch_params.use_aux_heads instead."
+            warnings.warn(message, DeprecationWarning)
+            use_aux_heads = get_param(arch_params, "aux_heads")
+        else:
+            use_aux_heads = get_param(arch_params, "use_aux_heads")
         super().__init__(
             backbone=arch_params.backbone,
             additional_layers=arch_params.additional_layers,
             upscale_module=arch_params.upscale_module,
             num_classes=arch_params.num_classes,
             highres_planes=arch_params.highres_planes,
             spp_width=arch_params.spp_planes,
             head_width=arch_params.head_planes,
-            use_aux_heads=arch_params.use_aux_heads,
+            use_aux_heads=use_aux_heads,
             ssp_inter_mode=arch_params.ssp_inter_mode,
             segmentation_inter_mode=arch_params.segmentation_inter_mode,
             skip_block=arch_params.skip_block,
             layer5_block=arch_params.layer5_block,
             layer5_bottleneck_expansion=arch_params.layer5_bottleneck_expansion,
             classification_mode=arch_params.classification_mode,
             spp_kernel_sizes=arch_params.spp_kernel_sizes,
             spp_strides=arch_params.spp_strides,
             layer3_repeats=arch_params.layer3_repeats,
         )
 
 
 DEFAULT_DDRNET_23_PARAMS = {
     "input_channels": 3,
-    "block": BasicBlock,
-    "skip_block": BasicBlock,
+    "block": BasicResNetBlock,
+    "skip_block": BasicResNetBlock,
     "layer5_block": Bottleneck,
     "layer5_bottleneck_expansion": 2,
     "layers": [2, 2, 2, 2, 1, 2, 2, 1],
     "upscale_module": UpscaleOnline(),
     "planes": 64,
     "highres_planes": 128,
     "head_planes": 128,
```

## super_gradients/training/models/segmentation_models/shelfnet.py

```diff
@@ -9,15 +9,15 @@
 import torch.nn as nn
 import torch.nn.functional as F
 
 from super_gradients.training.models.sg_module import SgModule
 from super_gradients.training.utils import HpmStruct
 from super_gradients.common.registry.registry import register_model
 from super_gradients.common.object_names import Models
-from super_gradients.training.models.classification_models.resnet import BasicBlock, ResNet, Bottleneck
+from super_gradients.training.models.classification_models.resnet import BasicResNetBlock, ResNet, Bottleneck
 
 
 class FCNHead(nn.Module):
     def __init__(self, in_channels, out_channels):
         super().__init__()
         inter_channels = in_channels // 4
         self.fcn = nn.Sequential(
@@ -89,20 +89,20 @@
         feat16 = self.layer3(feat8)  # 1/16
         feat32 = self.layer4(feat16)  # 1/32
         return feat4, feat8, feat16, feat32
 
 
 class ShelfResNetBackBone18(ShelfResNetBackBone):
     def __init__(self, num_classes: int):
-        super().__init__(BasicBlock, [2, 2, 2, 2], num_classes=num_classes)
+        super().__init__(BasicResNetBlock, [2, 2, 2, 2], num_classes=num_classes)
 
 
 class ShelfResNetBackBone34(ShelfResNetBackBone):
     def __init__(self, num_classes: int):
-        super().__init__(BasicBlock, [3, 4, 6, 3], num_classes=num_classes)
+        super().__init__(BasicResNetBlock, [3, 4, 6, 3], num_classes=num_classes)
 
 
 class ShelfResNetBackBone503343(ShelfResNetBackBone):
     def __init__(self, num_classes: int):
         super().__init__(Bottleneck, [3, 3, 4, 3], num_classes=num_classes)
```

## super_gradients/training/models/segmentation_models/stdc.py

```diff
@@ -580,14 +580,15 @@
                 no_multiply_params[name] = param
             else:
                 multiply_lr_params[name] = param
         return multiply_lr_params.items(), no_multiply_params.items()
 
 
 @register_model(Models.STDC_CUSTOM)
+@register_model("custom_stdc")  # deprecated naming convention. will be dropped in v4
 class CustomSTDCSegmentation(STDCSegmentationBase):
     """
     Fully customized STDC Segmentation factory module.
     """
 
     def __init__(self, arch_params: HpmStruct):
         super().__init__(
```

## super_gradients/training/pipelines/pipelines.py

```diff
@@ -1,7 +1,8 @@
+import copy
 from abc import ABC, abstractmethod
 from typing import List, Optional, Tuple, Union, Iterable
 from contextlib import contextmanager
 from tqdm import tqdm
 
 import numpy as np
 import torch
@@ -25,44 +26,59 @@
 
 
 logger = get_logger(__name__)
 
 
 @contextmanager
 def eval_mode(model: SgModule) -> None:
-    """Set a model in evaluation mode and deactivate gradient computation, undo at the end.
+    """Set a model in evaluation mode, undo at the end.
 
     :param model: The model to set in evaluation mode.
     """
     _starting_mode = model.training
     model.eval()
-    with torch.no_grad():
-        yield
+    yield
     model.train(mode=_starting_mode)
 
 
 class Pipeline(ABC):
     """An abstract base class representing a processing pipeline for a specific task.
     The pipeline includes loading images, preprocessing, prediction, and postprocessing.
 
     :param model:           The model used for making predictions.
     :param image_processor: A single image processor or a list of image processors for preprocessing and postprocessing the images.
     :param device:          The device on which the model will be run. If None, will run on current model device. Use "cuda" for GPU support.
+    :param fuse_model:                  If True, create a copy of the model, and fuse some of its layers to increase performance. This increases memory usage.
     """
 
-    def __init__(self, model: SgModule, image_processor: Union[Processing, List[Processing]], class_names: List[str], device: Optional[str] = None):
-        super().__init__()
+    def __init__(
+        self,
+        model: SgModule,
+        image_processor: Union[Processing, List[Processing]],
+        class_names: List[str],
+        device: Optional[str] = None,
+        fuse_model: bool = True,
+    ):
         self.device = device or next(model.parameters()).device
         self.model = model.to(self.device)
         self.class_names = class_names
 
         if isinstance(image_processor, list):
             image_processor = ComposeProcessing(image_processor)
         self.image_processor = image_processor
 
+        self.fuse_model = fuse_model  # If True, the model will be fused in the first forward pass, to make sure it gets the right input_size
+
+    def _fuse_model(self, input_example: torch.Tensor):
+        logger.info("Fusing some of the model's layers. If this takes too much memory, you can deactivate it by setting `fuse_model=False`")
+        self.model = copy.deepcopy(self.model)
+        self.model.eval()
+        self.model.prep_model_for_conversion(input_size=input_example.shape[-2:])
+        self.fuse_model = False
+
     def __call__(self, inputs: Union[str, ImageSource, List[ImageSource]], batch_size: Optional[int] = 32) -> ImagesPredictions:
         """Predict an image or a list of images.
 
         Supported types include:
             - str:              A string representing either a video, an image or an URL.
             - numpy.ndarray:    A numpy array representing the image
             - torch.Tensor:     A PyTorch tensor representing the image
@@ -149,16 +165,18 @@
         preprocessed_images, processing_metadatas = [], []
         for image in images:
             preprocessed_image, processing_metadata = self.image_processor.preprocess_image(image=image.copy())
             preprocessed_images.append(preprocessed_image)
             processing_metadatas.append(processing_metadata)
 
         # Predict
-        with eval_mode(self.model):
-            torch_inputs = torch.Tensor(np.array(preprocessed_images)).to(self.device)
+        with eval_mode(self.model), torch.no_grad(), torch.cuda.amp.autocast():
+            torch_inputs = torch.from_numpy(np.array(preprocessed_images)).to(self.device)
+            if self.fuse_model:
+                self._fuse_model(torch_inputs)
             model_output = self.model(torch_inputs)
             predictions = self._decode_model_output(model_output, model_input=torch_inputs)
 
         # Postprocess
         postprocessed_predictions = []
         for image, prediction, processing_metadata in zip(images, predictions, processing_metadatas):
             prediction = self.image_processor.postprocess_predictions(predictions=prediction, metadata=processing_metadata)
@@ -217,25 +235,27 @@
     The pipeline includes loading images, preprocessing, prediction, and postprocessing.
 
     :param model:                       The object detection model (instance of SgModule) used for making predictions.
     :param class_names:                 List of class names corresponding to the model's output classes.
     :param post_prediction_callback:    Callback function to process raw predictions from the model.
     :param image_processor:             Single image processor or a list of image processors for preprocessing and postprocessing the images.
     :param device:                      The device on which the model will be run. If None, will run on current model device. Use "cuda" for GPU support.
+    :param fuse_model:                  If True, create a copy of the model, and fuse some of its layers to increase performance. This increases memory usage.
     """
 
     def __init__(
         self,
         model: SgModule,
         class_names: List[str],
         post_prediction_callback: DetectionPostPredictionCallback,
         device: Optional[str] = None,
         image_processor: Optional[Processing] = None,
+        fuse_model: bool = True,
     ):
-        super().__init__(model=model, device=device, image_processor=image_processor, class_names=class_names)
+        super().__init__(model=model, device=device, image_processor=image_processor, class_names=class_names, fuse_model=fuse_model)
         self.post_prediction_callback = post_prediction_callback
 
     def _decode_model_output(self, model_output: Union[List, Tuple, torch.Tensor], model_input: np.ndarray) -> List[DetectionPrediction]:
         """Decode the model output, by applying post prediction callback. This includes NMS.
 
         :param model_output:    Direct output of the model, without any post-processing.
         :param model_input:     Model input (i.e. images after preprocessing).
@@ -263,15 +283,15 @@
         return ImageDetectionPrediction(image=image, prediction=prediction, class_names=self.class_names)
 
     def _combine_image_prediction_to_images(
         self, images_predictions: Iterable[ImageDetectionPrediction], n_images: Optional[int] = None
     ) -> ImagesDetectionPrediction:
         if n_images is not None and n_images == 1:
             # Do not show tqdm progress bar if there is only one image
-            pass
+            images_predictions = [next(iter(images_predictions))]
         else:
             images_predictions = [image_predictions for image_predictions in tqdm(images_predictions, total=n_images, desc="Predicting Images")]
 
         return ImagesDetectionPrediction(_images_prediction_lst=images_predictions)
 
     def _combine_image_prediction_to_video(
         self, images_predictions: Iterable[ImageDetectionPrediction], fps: float, n_images: Optional[int] = None
```

## super_gradients/training/pre_launch_callbacks/__init__.py

```diff
@@ -1,8 +1,9 @@
 from super_gradients.training.pre_launch_callbacks.pre_launch_callbacks import (
     PreLaunchCallback,
     AutoTrainBatchSizeSelectionCallback,
     QATRecipeModificationCallback,
+    modify_params_for_qat,
 )
 from super_gradients.common.registry.registry import ALL_PRE_LAUNCH_CALLBACKS
 
-__all__ = ["PreLaunchCallback", "AutoTrainBatchSizeSelectionCallback", "QATRecipeModificationCallback", "ALL_PRE_LAUNCH_CALLBACKS"]
+__all__ = ["PreLaunchCallback", "AutoTrainBatchSizeSelectionCallback", "QATRecipeModificationCallback", "ALL_PRE_LAUNCH_CALLBACKS", "modify_params_for_qat"]
```

## super_gradients/training/pre_launch_callbacks/pre_launch_callbacks.py

```diff
@@ -1,22 +1,25 @@
 import copy
 from copy import deepcopy
 from typing import Union
 
 from omegaconf import DictConfig
 import torch
 
+from super_gradients.common.environment.cfg_utils import load_recipe
 from super_gradients.common.registry.registry import register_pre_launch_callback
 from super_gradients import is_distributed
 from super_gradients.common.abstractions.abstract_logger import get_logger
 from super_gradients.training import models
 from torch.distributed import barrier
 import cv2
 import numpy as np
 
+from super_gradients.training.utils import get_param
+
 logger = get_logger(__name__)
 
 
 class PreLaunchCallback:
     """
     PreLaunchCallback
 
@@ -99,22 +102,22 @@
             arch_params=cfg.arch_params,
             strict_load=cfg.checkpoint_params.strict_load,
             pretrained_weights=cfg.checkpoint_params.pretrained_weights,
             checkpoint_path=cfg.checkpoint_params.checkpoint_path,
             load_backbone=cfg.checkpoint_params.load_backbone,
         )
         tmp_cfg = deepcopy(cfg)
-        tmp_cfg.training_hyperparams.batch_accumulate = 1
-        tmp_cfg.training_hyperparams.max_train_batches = self.num_forward_passes
-        tmp_cfg.training_hyperparams.run_validation_freq = 2
-        tmp_cfg.training_hyperparams.silent_mode = True
-        tmp_cfg.training_hyperparams.save_model = False
-        tmp_cfg.training_hyperparams.max_epochs = 1
-        tmp_cfg.training_hyperparams.average_best_models = False
-        tmp_cfg.training_hyperparams.kill_ddp_pgroup_on_end = False
+        tmp_cfg.training_hyperparamsbatch_accumulate = 1
+        tmp_cfg.training_hyperparamsmax_train_batches = self.num_forward_passes
+        tmp_cfg.training_hyperparamsrun_validation_freq = 2
+        tmp_cfg.training_hyperparamssilent_mode = True
+        tmp_cfg.training_hyperparamssave_model = False
+        tmp_cfg.training_hyperparamsmax_epochs = 1
+        tmp_cfg.training_hyperparamsaverage_best_models = False
+        tmp_cfg.training_hyperparamskill_ddp_pgroup_on_end = False
         tmp_cfg.pre_launch_callbacks_list = []
 
         fastest_batch_time = np.inf
         fastest_batch_size = curr_batch_size
 
         bs_found = False
 
@@ -176,14 +179,159 @@
                 del p.grad  # free some memory
         torch.cuda.empty_cache()
         # WAIT FOR ALL PROCESSES TO CLEAR THEIR MEMORY BEFORE MOVING ON
         if is_distributed():
             barrier()
 
 
+def modify_params_for_qat(
+    training_hyperparams,
+    train_dataset_params,
+    val_dataset_params,
+    train_dataloader_params,
+    val_dataloader_params,
+    quantization_params=None,
+    batch_size_divisor: int = 2,
+    max_epochs_divisor: int = 10,
+    lr_decay_factor: float = 0.01,
+    warmup_epochs_divisor: int = 10,
+    cosine_final_lr_ratio: float = 0.01,
+    disable_phase_callbacks: bool = True,
+    disable_augmentations: bool = False,
+):
+    """
+
+    This method modifies the recipe for QAT to implement rules of thumb based on the regular non-qat recipe.
+    It does so by manipulating the training_hyperparams, train_dataloader_params, val_dataloader_params, train_dataset_params, val_dataset_params.
+    Usage:
+        trainer = Trainer("test_launch_qat_with_minimal_changes")
+        net = ResNet18(num_classes=10, arch_params={})
+        train_params = {...}
+
+        train_dataset_params = {
+            "transforms": [...
+            ]
+        }
+
+        train_dataloader_params = {"batch_size": 256}
+
+        val_dataset_params = {"transforms": [ToTensor(), Normalize(mean=[0.4914, 0.4822, 0.4465], std=[0.2023, 0.1994, 0.2010])]}
+
+        val_dataloader_params = {"batch_size": 256}
+
+        train_loader = cifar10_train(dataset_params=train_dataset_params, dataloader_params=train_dataloader_params)
+        valid_loader = cifar10_val(dataset_params=val_dataset_params, dataloader_params=val_dataloader_params)
+
+        trainer.train(
+            model=net,
+            training_params=train_params,
+            train_loader=train_loader,
+            valid_loader=valid_loader,
+        )
+
+        train_params, train_dataset_params, val_dataset_params, train_dataloader_params, val_dataloader_params = modify_params_for_qat(
+            train_params, train_dataset_params, val_dataset_params, train_dataloader_params, val_dataloader_params
+        )
+
+        train_loader = cifar10_train(dataset_params=train_dataset_params, dataloader_params=train_dataloader_params)
+        valid_loader = cifar10_val(dataset_params=val_dataset_params, dataloader_params=val_dataloader_params)
+
+        trainer.qat(
+            model=net,
+            training_params=train_params,
+            train_loader=train_loader,
+            valid_loader=valid_loader,
+            calib_loader=train_loader,
+        )
+
+    :param val_dataset_params: Dict, validation dataset_params to be passed to dataloaders.get(...) when instantiating the train dataloader.
+    :param train_dataset_params: Dict, train dataset_params to be passed to dataloaders.get(...) when instantiating the validation dataloader.
+    :param val_dataloader_params: Dict, validation dataloader_params to be passed to dataloaders.get(...) when instantiating the validation dataloader.
+    :param train_dataloader_params: Dict, train dataloader_params to be passed to dataloaders.get(...) when instantiating the train dataloader.
+    :param training_hyperparams: Dict, train parameters passed to Trainer.qat(...)
+    :param quantization_params: Dict, quantization parameters as passed to Trainer.qat(...). When None, will use the
+     default parameters in super_gradients/recipes/quantization_params/default_quantization_params.yaml
+    :param int batch_size_divisor: Divisor used to calculate the batch size. Default value is 2.
+    :param int max_epochs_divisor: Divisor used to calculate the maximum number of epochs. Default value is 10.
+    :param float lr_decay_factor: Factor used to decay the learning rate, weight decay and warmup. Default value is 0.01.
+    :param int warmup_epochs_divisor: Divisor used to calculate the number of warm-up epochs. Default value is 10.
+    :param float cosine_final_lr_ratio: Ratio used to determine the final learning rate in a cosine annealing schedule. Default value is 0.01.
+    :param bool disable_phase_callbacks: Flag to control to disable phase callbacks, which can interfere with QAT. Default value is True.
+    :param bool disable_augmentations: Flag to control to disable phase augmentations, which can interfere with QAT. Default value is False.
+    :return: modified (copy) training_hyperparams, train_dataset_params, val_dataset_params, train_dataloader_params, val_dataloader_params
+    """
+    if quantization_params is None:
+        quantization_params = load_recipe("quantization_params/default_quantization_params").quantization_params
+
+    quantization_params = deepcopy(quantization_params)
+    training_hyperparams = deepcopy(training_hyperparams)
+    train_dataloader_params = deepcopy(train_dataloader_params)
+    val_dataloader_params = deepcopy(val_dataloader_params)
+    train_dataset_params = deepcopy(train_dataset_params)
+    val_dataset_params = deepcopy(val_dataset_params)
+
+    if "max_epochs" not in training_hyperparams.keys():
+        raise ValueError("max_epochs is a required field in training_hyperparams for QAT modification.")
+
+    if "initial_lr" not in training_hyperparams.keys():
+        raise ValueError("initial_lr is a required field in training_hyperparams for QAT modification.")
+
+    if "optimizer_params" not in training_hyperparams.keys():
+        raise ValueError("optimizer_params is a required field in training_hyperparams for QAT modification.")
+
+    if "weight_decay" not in training_hyperparams["optimizer_params"].keys():
+        raise ValueError("weight_decay is a required field in training_hyperparams['optimizer_params'] for QAT modification.")
+
+    # Q/DQ Layers take a lot of space for activations in training mode
+    if get_param(quantization_params, "selective_quantizer_params") and get_param(quantization_params["selective_quantizer_params"], "learn_amax"):
+        train_dataloader_params["batch_size"] //= batch_size_divisor
+        val_dataloader_params["batch_size"] //= batch_size_divisor
+
+        logger.warning(f"New dataset_params.train_dataloader_params.batch_size: {train_dataloader_params['batch_size']}")
+        logger.warning(f"New dataset_params.val_dataloader_params.batch_size: {val_dataloader_params['batch_size']}")
+    training_hyperparams["max_epochs"] //= max_epochs_divisor
+    logger.warning(f"New number of epochs: {training_hyperparams['max_epochs']}")
+    training_hyperparams["initial_lr"] *= lr_decay_factor
+    if get_param(training_hyperparams, "warmup_initial_lr") is not None:
+        training_hyperparams["warmup_initial_lr"] *= lr_decay_factor
+    else:
+        training_hyperparams["warmup_initial_lr"] = training_hyperparams["initial_lr"] * 0.01
+    training_hyperparams["optimizer_params"]["weight_decay"] *= lr_decay_factor
+    logger.warning(f"New learning rate: {training_hyperparams['initial_lr']}")
+    logger.warning(f"New weight decay: {training_hyperparams['optimizer_params']['weight_decay']}")
+    # as recommended by pytorch-quantization docs
+    if get_param(training_hyperparams, "lr_mode") != "cosine":
+        training_hyperparams["lr_mode"] = "cosine"
+    training_hyperparams["cosine_final_lr_ratio"] = cosine_final_lr_ratio
+    logger.warning(
+        f"lr_mode will be set to cosine for QAT run instead of {get_param(training_hyperparams, 'lr_mode')} with "
+        f"cosine_final_lr_ratio={cosine_final_lr_ratio}"
+    )
+
+    training_hyperparams["lr_warmup_epochs"] = (training_hyperparams["max_epochs"] // warmup_epochs_divisor) or 1
+    logger.warning(f"New lr_warmup_epochs: {training_hyperparams['lr_warmup_epochs']}")
+
+    # do mess with Q/DQ
+    if get_param(training_hyperparams, "ema"):
+        logger.warning("EMA will be disabled for QAT run.")
+        training_hyperparams["ema"] = False
+    if get_param(training_hyperparams, "sync_bn"):
+        logger.warning("SyncBatchNorm will be disabled for QAT run.")
+        training_hyperparams["sync_bn"] = False
+    if disable_phase_callbacks and get_param(training_hyperparams, "phase_callbacks") is not None and len(training_hyperparams["phase_callbacks"]) > 0:
+        logger.warning(f"Recipe contains {len(training_hyperparams['phase_callbacks'])} phase callbacks. All of them will be disabled.")
+        training_hyperparams["phase_callbacks"] = []
+    # no augmentations
+    if disable_augmentations and "transforms" in val_dataset_params:
+        logger.warning("Augmentations will be disabled for QAT run. Using validation transforms instead.")
+        train_dataset_params["transforms"] = val_dataset_params["transforms"]
+
+    return training_hyperparams, train_dataset_params, val_dataset_params, train_dataloader_params, val_dataloader_params
+
+
 @register_pre_launch_callback()
 class QATRecipeModificationCallback(PreLaunchCallback):
     """
      QATRecipeModificationCallback(PreLaunchCallback)
 
     This callback modifies the recipe for QAT to implement rules of thumb based on the regular non-qat recipe.
 
@@ -205,15 +353,15 @@
             max_epochs_divisor: 10
             lr_decay_factor: 0.01
             warmup_epochs_divisor: 10
             cosine_final_lr_ratio: 0.01
             disable_phase_callbacks: True
             disable_augmentations: False
 
-    USE THIS CALLBACK ONLY WITH QATTrainer!
+    USE THIS CALLBACK ONLY WITH Trainer.quantize_from_config
     """
 
     def __init__(
         self,
         batch_size_divisor: int = 2,
         max_epochs_divisor: int = 10,
         lr_decay_factor: float = 0.01,
@@ -231,58 +379,35 @@
         self.batch_size_divisor = batch_size_divisor
 
     def __call__(self, cfg: Union[dict, DictConfig]) -> Union[dict, DictConfig]:
         logger.info("Modifying recipe to suit QAT rules of thumb. Remove QATRecipeModificationCallback to disable.")
 
         cfg = copy.deepcopy(cfg)
 
-        # Q/DQ Layers take a lot of space for activations in training mode
-        if cfg.quantization_params.selective_quantizer_params.learn_amax:
-            cfg.dataset_params.train_dataloader_params.batch_size //= self.batch_size_divisor
-            cfg.dataset_params.val_dataloader_params.batch_size //= self.batch_size_divisor
-
-            logger.warning(f"New dataset_params.train_dataloader_params.batch_size: {cfg.dataset_params.train_dataloader_params.batch_size}")
-            logger.warning(f"New dataset_params.val_dataloader_params.batch_size: {cfg.dataset_params.val_dataloader_params.batch_size}")
-
-        cfg.training_hyperparams.max_epochs //= self.max_epochs_divisor
-        logger.warning(f"New number of epochs: {cfg.training_hyperparams.max_epochs}")
-
-        cfg.training_hyperparams.initial_lr *= self.lr_decay_factor
-        if cfg.training_hyperparams.warmup_initial_lr is not None:
-            cfg.training_hyperparams.warmup_initial_lr *= self.lr_decay_factor
-        else:
-            cfg.training_hyperparams.warmup_initial_lr = cfg.training_hyperparams.initial_lr * 0.01
-
-        cfg.training_hyperparams.optimizer_params.weight_decay *= self.lr_decay_factor
-
-        logger.warning(f"New learning rate: {cfg.training_hyperparams.initial_lr}")
-        logger.warning(f"New weight decay: {cfg.training_hyperparams.optimizer_params.weight_decay}")
-
-        # as recommended by pytorch-quantization docs
-        cfg.training_hyperparams.lr_mode = "cosine"
-        cfg.training_hyperparams.lr_warmup_epochs = (cfg.training_hyperparams.max_epochs // self.warmup_epochs_divisor) or 1
-        cfg.training_hyperparams.cosine_final_lr_ratio = self.cosine_final_lr_ratio
-
-        # do mess with Q/DQ
-        if cfg.training_hyperparams.ema:
-            logger.warning("EMA will be disabled for QAT run.")
-            cfg.training_hyperparams.ema = False
-
-        if cfg.training_hyperparams.sync_bn:
-            logger.warning("SyncBatchNorm will be disabled for QAT run.")
-            cfg.training_hyperparams.sync_bn = False
-
-        if self.disable_phase_callbacks and len(cfg.training_hyperparams.phase_callbacks) > 0:
-            logger.warning(f"Recipe contains {len(cfg.training_hyperparams.phase_callbacks)} phase callbacks. All of them will be disabled.")
-            cfg.training_hyperparams.phase_callbacks = []
+        (
+            cfg.training_hyperparams,
+            cfg.dataset_params.train_dataset_params,
+            cfg.dataset_params.val_dataset_params,
+            cfg.dataset_params.train_dataloader_params,
+            cfg.dataset_params.val_dataloader_params,
+        ) = modify_params_for_qat(
+            training_hyperparams=cfg.training_hyperparams,
+            train_dataset_params=cfg.dataset_params.train_dataset_params,
+            train_dataloader_params=cfg.dataset_params.train_dataloader_params,
+            val_dataset_params=cfg.dataset_params.val_dataset_params,
+            val_dataloader_params=cfg.dataset_params.val_dataloader_params,
+            quantization_params=cfg.quantization_params,
+            batch_size_divisor=self.batch_size_divisor,
+            disable_phase_callbacks=self.disable_phase_callbacks,
+            cosine_final_lr_ratio=self.cosine_final_lr_ratio,
+            warmup_epochs_divisor=self.warmup_epochs_divisor,
+            lr_decay_factor=self.lr_decay_factor,
+            max_epochs_divisor=self.max_epochs_divisor,
+            disable_augmentations=self.disable_augmentations,
+        )
 
         if cfg.multi_gpu != "OFF" or cfg.num_gpus != 1:
             logger.warning(f"Recipe requests multi_gpu={cfg.multi_gpu} and num_gpus={cfg.num_gpus}. Changing to multi_gpu=OFF and num_gpus=1")
             cfg.multi_gpu = "OFF"
             cfg.num_gpus = 1
 
-        # no augmentations
-        if self.disable_augmentations and "transforms" in cfg.dataset_params.val_dataset_params:
-            logger.warning("Augmentations will be disabled for QAT run.")
-            cfg.dataset_params.train_dataset_params.transforms = cfg.dataset_params.val_dataset_params.transforms
-
         return cfg
```

## super_gradients/training/qat_trainer/qat_trainer.py

```diff
@@ -1,201 +1,17 @@
-import os
 from typing import Union, Tuple
 
-import copy
-import hydra
-import torch.cuda
+from deprecated import deprecated
 from omegaconf import DictConfig
-from omegaconf import OmegaConf
 from torch import nn
 
 from super_gradients.common.abstractions.abstract_logger import get_logger
-from super_gradients.common.environment.device_utils import device_config
-from super_gradients.training import utils as core_utils, models, dataloaders
 from super_gradients.training.sg_trainer import Trainer
-from super_gradients.training.utils import get_param
-from super_gradients.training.utils.distributed_training_utils import setup_device
-from super_gradients.modules.repvgg_block import fuse_repvgg_blocks_residual_branches
 
 logger = get_logger(__name__)
-try:
-    from super_gradients.training.utils.quantization.calibrator import QuantizationCalibrator
-    from super_gradients.training.utils.quantization.export import export_quantized_module_to_onnx
-    from super_gradients.training.utils.quantization.selective_quantization_utils import SelectiveQuantizer
-
-    _imported_pytorch_quantization_failure = None
-
-except (ImportError, NameError, ModuleNotFoundError) as import_err:
-    logger.debug("Failed to import pytorch_quantization:")
-    logger.debug(import_err)
-    _imported_pytorch_quantization_failure = import_err
 
 
 class QATTrainer(Trainer):
     @classmethod
-    def train_from_config(cls, cfg: Union[DictConfig, dict]) -> Tuple[nn.Module, Tuple]:
-        """
-        Perform quantization aware training (QAT) according to a recipe configuration.
-
-        This method will instantiate all the objects specified in the recipe, build and quantize the model,
-        and calibrate the quantized model. The resulting quantized model and the output of the trainer.train()
-        method will be returned.
-
-        The quantized model will be exported to ONNX along with other checkpoints.
-
-        :param cfg: The parsed DictConfig object from yaml recipe files or a dictionary.
-        :return: A tuple containing the quantized model and the output of trainer.train() method.
-        :rtype: Tuple[nn.Module, Tuple]
-
-        :raises ValueError: If the recipe does not have the required key `quantization_params` or
-        `checkpoint_params.checkpoint_path` in it.
-        :raises NotImplementedError: If the recipe requests multiple GPUs or num_gpus is not equal to 1.
-        :raises ImportError: If pytorch-quantization import was unsuccessful
-
-        """
-        if _imported_pytorch_quantization_failure is not None:
-            raise _imported_pytorch_quantization_failure
-
-        # INSTANTIATE ALL OBJECTS IN CFG
-        cfg = hydra.utils.instantiate(cfg)
-
-        # TRIGGER CFG MODIFYING CALLBACKS
-        cfg = cls._trigger_cfg_modifying_callbacks(cfg)
-
-        if "quantization_params" not in cfg:
-            raise ValueError("Your recipe does not have quantization_params. Add them to use QAT.")
-
-        if "checkpoint_path" not in cfg.checkpoint_params:
-            raise ValueError("Starting checkpoint is a must for QAT finetuning.")
-
-        num_gpus = core_utils.get_param(cfg, "num_gpus")
-        multi_gpu = core_utils.get_param(cfg, "multi_gpu")
-        device = core_utils.get_param(cfg, "device")
-        if num_gpus != 1:
-            raise NotImplementedError(
-                f"Recipe requests multi_gpu={cfg.multi_gpu} and num_gpus={cfg.num_gpus}. QAT is proven to work correctly only with multi_gpu=OFF and num_gpus=1"
-            )
-
-        setup_device(device=device, multi_gpu=multi_gpu, num_gpus=num_gpus)
-
-        # INSTANTIATE DATA LOADERS
-        train_dataloader = dataloaders.get(
-            name=get_param(cfg, "train_dataloader"),
-            dataset_params=copy.deepcopy(cfg.dataset_params.train_dataset_params),
-            dataloader_params=copy.deepcopy(cfg.dataset_params.train_dataloader_params),
-        )
-
-        val_dataloader = dataloaders.get(
-            name=get_param(cfg, "val_dataloader"),
-            dataset_params=copy.deepcopy(cfg.dataset_params.val_dataset_params),
-            dataloader_params=copy.deepcopy(cfg.dataset_params.val_dataloader_params),
-        )
-
-        if "calib_dataloader" in cfg:
-            calib_dataloader_name = get_param(cfg, "calib_dataloader")
-            calib_dataloader_params = copy.deepcopy(cfg.dataset_params.calib_dataloader_params)
-            calib_dataset_params = copy.deepcopy(cfg.dataset_params.calib_dataset_params)
-        else:
-            calib_dataloader_name = get_param(cfg, "train_dataloader")
-            calib_dataloader_params = copy.deepcopy(cfg.dataset_params.train_dataloader_params)
-            calib_dataset_params = copy.deepcopy(cfg.dataset_params.train_dataset_params)
-
-            # if we use whole dataloader for calibration, don't shuffle it
-            # HistogramCalibrator collection routine is sensitive to order of batches and produces slightly different results
-            # if we use several batches, we don't want it to be from one class if it's sequential in dataloader
-            # model is in eval mode, so BNs will not be affected
-            calib_dataloader_params.shuffle = cfg.quantization_params.calib_params.num_calib_batches is not None
-            # we don't need training transforms during calibration, distribution of activations will be skewed
-            calib_dataset_params.transforms = cfg.dataset_params.val_dataset_params.transforms
-
-        calib_dataloader = dataloaders.get(
-            name=calib_dataloader_name,
-            dataset_params=calib_dataset_params,
-            dataloader_params=calib_dataloader_params,
-        )
-
-        # BUILD MODEL
-        model = models.get(
-            model_name=cfg.arch_params.get("model_name", None) or cfg.architecture,
-            num_classes=cfg.get("num_classes", None) or cfg.arch_params.num_classes,
-            arch_params=cfg.arch_params,
-            strict_load=cfg.checkpoint_params.strict_load,
-            pretrained_weights=cfg.checkpoint_params.pretrained_weights,
-            checkpoint_path=cfg.checkpoint_params.checkpoint_path,
-            load_backbone=False,
-        )
-        model.to(device_config.device)
-
-        # QUANTIZE MODEL
-        model.eval()
-        fuse_repvgg_blocks_residual_branches(model)
-
-        q_util = SelectiveQuantizer(
-            default_quant_modules_calibrator_weights=cfg.quantization_params.selective_quantizer_params.calibrator_w,
-            default_quant_modules_calibrator_inputs=cfg.quantization_params.selective_quantizer_params.calibrator_i,
-            default_per_channel_quant_weights=cfg.quantization_params.selective_quantizer_params.per_channel,
-            default_learn_amax=cfg.quantization_params.selective_quantizer_params.learn_amax,
-            verbose=cfg.quantization_params.calib_params.verbose,
-        )
-        q_util.register_skip_quantization(layer_names=cfg.quantization_params.selective_quantizer_params.skip_modules)
-        q_util.quantize_module(model)
-
-        # CALIBRATE MODEL
-        logger.info("Calibrating model...")
-        calibrator = QuantizationCalibrator(
-            verbose=cfg.quantization_params.calib_params.verbose,
-            torch_hist=True,
-        )
-        calibrator.calibrate_model(
-            model,
-            method=cfg.quantization_params.calib_params.histogram_calib_method,
-            calib_data_loader=calib_dataloader,
-            num_calib_batches=cfg.quantization_params.calib_params.num_calib_batches or len(train_dataloader),
-            percentile=get_param(cfg.quantization_params.calib_params, "percentile", 99.99),
-        )
-        calibrator.reset_calibrators(model)  # release memory taken by calibrators
-
-        # VALIDATE PTQ MODEL AND PRINT SUMMARY
-        logger.info("Validating PTQ model...")
-        trainer = Trainer(experiment_name=cfg.experiment_name, ckpt_root_dir=get_param(cfg, "ckpt_root_dir", default_val=None))
-        valid_metrics_dict = trainer.test(model=model, test_loader=val_dataloader, test_metrics_list=cfg.training_hyperparams.valid_metrics_list)
-        results = ["PTQ Model Validation Results"]
-        results += [f"   - {metric:10}: {value}" for metric, value in valid_metrics_dict.items()]
-        logger.info("\n".join(results))
-
-        # TRAIN
-        if cfg.quantization_params.ptq_only:
-            logger.info("cfg.quantization_params.ptq_only=True. Performing PTQ only!")
-            suffix = "ptq"
-            res = None
-        else:
-            model.train()
-            recipe_logged_cfg = {"recipe_config": OmegaConf.to_container(cfg, resolve=True)}
-            trainer = Trainer(experiment_name=cfg.experiment_name, ckpt_root_dir=get_param(cfg, "ckpt_root_dir", default_val=None))
-            torch.cuda.empty_cache()
-
-            res = trainer.train(
-                model=model,
-                train_loader=train_dataloader,
-                valid_loader=val_dataloader,
-                training_params=cfg.training_hyperparams,
-                additional_configs_to_log=recipe_logged_cfg,
-            )
-            suffix = "qat"
-
-        # EXPORT QUANTIZED MODEL TO ONNX
-        input_shape = next(iter(val_dataloader))[0].shape
-        os.makedirs(trainer.checkpoints_dir_path, exist_ok=True)
-
-        qdq_onnx_path = os.path.join(trainer.checkpoints_dir_path, f"{cfg.experiment_name}_{'x'.join((str(x) for x in input_shape))}_{suffix}.onnx")
-        # TODO: modify SG's convert_to_onnx for quantized models and use it instead
-        export_quantized_module_to_onnx(
-            model=model.cpu(),
-            onnx_filename=qdq_onnx_path,
-            input_shape=input_shape,
-            input_size=input_shape,
-            train=False,
-        )
-
-        logger.info(f"Exported {suffix.upper()} ONNX to {qdq_onnx_path}")
-
-        return model, res
+    @deprecated(version="3.2.0", reason="QATTrainer is deprecated and will be removed in future release, use Trainer " "class instead.")
+    def quantize_from_config(cls, cfg: Union[DictConfig, dict]) -> Tuple[nn.Module, Tuple]:
+        return Trainer.quantize_from_config(cfg)
```

## super_gradients/training/sg_trainer/sg_trainer.py

```diff
@@ -1,28 +1,32 @@
+import copy
 import inspect
 import os
 from copy import deepcopy
 from pathlib import Path
-from typing import Union, Tuple, Mapping, Dict, Any
+from typing import Union, Tuple, Mapping, Dict, Any, List
 
 import hydra
 import numpy as np
 import torch
-from omegaconf import DictConfig
-from omegaconf import OmegaConf
+import torch.cuda
+import torch.nn
+import torchmetrics
+from omegaconf import DictConfig, OmegaConf
 from piptools.scripts.sync import _get_installed_distributions
 from torch import nn
 from torch.cuda.amp import GradScaler, autocast
 from torch.utils.data import DataLoader, SequentialSampler
 from torch.utils.data.distributed import DistributedSampler
-from torchmetrics import MetricCollection
+from torchmetrics import MetricCollection, Metric
 from tqdm import tqdm
 
 from super_gradients.common.environment.checkpoints_dir_utils import get_checkpoints_dir_path, get_ckpt_local_path
 from super_gradients.module_interfaces import HasPreprocessingParams, HasPredict
+from super_gradients.modules.repvgg_block import fuse_repvgg_blocks_residual_branches
 
 from super_gradients.training.utils.sg_trainer_utils import get_callable_param_names
 from super_gradients.common.abstractions.abstract_logger import get_logger
 from super_gradients.common.sg_loggers.abstract_sg_logger import AbstractSGLogger
 from super_gradients.common.sg_loggers.base_sg_logger import BaseSGLogger
 from super_gradients.common.data_types.enum import MultiGPUMode, StrictLoad, EvaluationType
 from super_gradients.common.decorators.factory_decorator import resolve_param
@@ -79,21 +83,34 @@
     MetricsUpdateCallback,
     ContextSgMethods,
     LRCallbackBase,
 )
 from super_gradients.common.registry.registry import LR_SCHEDULERS_CLS_DICT, LR_WARMUP_CLS_DICT
 from super_gradients.common.environment.device_utils import device_config
 from super_gradients.training.utils import HpmStruct
-from super_gradients.common.environment.cfg_utils import load_experiment_cfg, add_params_to_cfg
+from super_gradients.common.environment.cfg_utils import load_experiment_cfg, add_params_to_cfg, load_recipe
 from super_gradients.common.factories.pre_launch_callbacks_factory import PreLaunchCallbacksFactory
 from super_gradients.training.params import TrainingParams
 
 logger = get_logger(__name__)
 
 
+try:
+    from super_gradients.training.utils.quantization.calibrator import QuantizationCalibrator
+    from super_gradients.training.utils.quantization.export import export_quantized_module_to_onnx
+    from super_gradients.training.utils.quantization.selective_quantization_utils import SelectiveQuantizer
+
+    _imported_pytorch_quantization_failure = None
+
+except (ImportError, NameError, ModuleNotFoundError) as import_err:
+    logger.debug("Failed to import pytorch_quantization:")
+    logger.debug(import_err)
+    _imported_pytorch_quantization_failure = import_err
+
+
 class Trainer:
     """
     SuperGradient Model - Base Class for Sg Models
 
     Methods
     -------
     train(max_epochs : int, initial_epoch : int, save_model : bool)
@@ -129,14 +146,15 @@
             )
 
         if require_ddp_setup():
             raise DDPNotSetupException()
 
         # SET THE EMPTY PROPERTIES
         self.net, self.architecture, self.arch_params, self.dataset_interface = None, None, None, None
+        self.train_loader, self.valid_loader = None, None
         self.ema = None
         self.ema_model = None
         self.sg_logger = None
         self.update_param_groups = None
         self.criterion = None
         self.training_params = None
         self.scaler = None
@@ -147,15 +165,14 @@
         # SET THE DEFAULT PROPERTIES
         self.half_precision = False
         self.load_checkpoint = False
         self.load_backbone = False
         self.load_weights_only = False
         self.ddp_silent_mode = is_ddp_subprocess()
 
-        self.source_ckpt_folder_name = None
         self.model_weight_averaging = None
         self.average_model_checkpoint_filename = "average_model.pth"
         self.start_epoch = 0
         self.best_metric = np.inf
         self.external_checkpoint_path = None
         self.strict_load = StrictLoad.ON
         self.load_ema_as_net = False
@@ -394,82 +411,83 @@
         train_epoch - A single epoch training procedure
             :param optimizer:   The optimizer for the network
             :param epoch:       The current epoch
             :param silent_mode: No verbosity
         """
         # SET THE MODEL IN training STATE
         self.net.train()
+
         # THE DISABLE FLAG CONTROLS WHETHER THE PROGRESS BAR IS SILENT OR PRINTS THE LOGS
-        progress_bar_train_loader = tqdm(self.train_loader, bar_format="{l_bar}{bar:10}{r_bar}", dynamic_ncols=True, disable=silent_mode)
-        progress_bar_train_loader.set_description(f"Train epoch {epoch}")
+        with tqdm(self.train_loader, bar_format="{l_bar}{bar:10}{r_bar}", dynamic_ncols=True, disable=silent_mode) as progress_bar_train_loader:
+            progress_bar_train_loader.set_description(f"Train epoch {epoch}")
 
-        # RESET/INIT THE METRIC LOGGERS
-        self._reset_metrics()
+            # RESET/INIT THE METRIC LOGGERS
+            self._reset_metrics()
 
-        self.train_metrics.to(device_config.device)
-        loss_avg_meter = core_utils.utils.AverageMeter()
+            self.train_metrics.to(device_config.device)
+            loss_avg_meter = core_utils.utils.AverageMeter()
 
-        context = PhaseContext(
-            epoch=epoch,
-            optimizer=self.optimizer,
-            metrics_compute_fn=self.train_metrics,
-            loss_avg_meter=loss_avg_meter,
-            criterion=self.criterion,
-            device=device_config.device,
-            lr_warmup_epochs=self.training_params.lr_warmup_epochs,
-            sg_logger=self.sg_logger,
-            train_loader=self.train_loader,
-            context_methods=self._get_context_methods(Phase.TRAIN_BATCH_END),
-            ddp_silent_mode=self.ddp_silent_mode,
-        )
+            context = PhaseContext(
+                epoch=epoch,
+                optimizer=self.optimizer,
+                metrics_compute_fn=self.train_metrics,
+                loss_avg_meter=loss_avg_meter,
+                criterion=self.criterion,
+                device=device_config.device,
+                lr_warmup_epochs=self.training_params.lr_warmup_epochs,
+                sg_logger=self.sg_logger,
+                train_loader=self.train_loader,
+                context_methods=self._get_context_methods(Phase.TRAIN_BATCH_END),
+                ddp_silent_mode=self.ddp_silent_mode,
+            )
 
-        for batch_idx, batch_items in enumerate(progress_bar_train_loader):
-            batch_items = core_utils.tensor_container_to_device(batch_items, device_config.device, non_blocking=True)
-            inputs, targets, additional_batch_items = sg_trainer_utils.unpack_batch_items(batch_items)
+            for batch_idx, batch_items in enumerate(progress_bar_train_loader):
+                batch_items = core_utils.tensor_container_to_device(batch_items, device_config.device, non_blocking=True)
+                inputs, targets, additional_batch_items = sg_trainer_utils.unpack_batch_items(batch_items)
 
-            if self.pre_prediction_callback is not None:
-                inputs, targets = self.pre_prediction_callback(inputs, targets, batch_idx)
+                if self.pre_prediction_callback is not None:
+                    inputs, targets = self.pre_prediction_callback(inputs, targets, batch_idx)
 
-            context.update_context(batch_idx=batch_idx, inputs=inputs, target=targets, **additional_batch_items)
-            self.phase_callback_handler.on_train_batch_start(context)
+                context.update_context(batch_idx=batch_idx, inputs=inputs, target=targets, **additional_batch_items)
+                self.phase_callback_handler.on_train_batch_start(context)
 
-            # AUTOCAST IS ENABLED ONLY IF self.training_params.mixed_precision - IF enabled=False AUTOCAST HAS NO EFFECT
-            with autocast(enabled=self.training_params.mixed_precision):
-                # FORWARD PASS TO GET NETWORK'S PREDICTIONS
-                outputs = self.net(inputs)
+                # AUTOCAST IS ENABLED ONLY IF self.training_params.mixed_precision - IF enabled=False AUTOCAST HAS NO EFFECT
+                with autocast(enabled=self.training_params.mixed_precision):
+                    # FORWARD PASS TO GET NETWORK'S PREDICTIONS
+                    outputs = self.net(inputs)
 
-                # COMPUTE THE LOSS FOR BACK PROP + EXTRA METRICS COMPUTED DURING THE LOSS FORWARD PASS
-                loss, loss_log_items = self._get_losses(outputs, targets)
+                    # COMPUTE THE LOSS FOR BACK PROP + EXTRA METRICS COMPUTED DURING THE LOSS FORWARD PASS
+                    loss, loss_log_items = self._get_losses(outputs, targets)
 
-            context.update_context(preds=outputs, loss_log_items=loss_log_items)
-            self.phase_callback_handler.on_train_batch_loss_end(context)
+                context.update_context(preds=outputs, loss_log_items=loss_log_items)
+                self.phase_callback_handler.on_train_batch_loss_end(context)
 
-            if not self.ddp_silent_mode and batch_idx == 0:
-                self._epoch_start_logging_values = self._get_epoch_start_logging_values()
+                if not self.ddp_silent_mode and batch_idx == 0:
+                    self._epoch_start_logging_values = self._get_epoch_start_logging_values()
 
-            self._backward_step(loss, epoch, batch_idx, context)
+                self._backward_step(loss, epoch, batch_idx, context)
 
-            # COMPUTE THE RUNNING USER METRICS AND LOSS RUNNING ITEMS. RESULT TUPLE IS THEIR CONCATENATION.
-            logging_values = loss_avg_meter.average + get_metrics_results_tuple(self.train_metrics)
-            gpu_memory_utilization = get_gpu_mem_utilization() / 1e9 if torch.cuda.is_available() else 0
+                # COMPUTE THE RUNNING USER METRICS AND LOSS RUNNING ITEMS. RESULT TUPLE IS THEIR CONCATENATION.
+                logging_values = loss_avg_meter.average + get_metrics_results_tuple(self.train_metrics)
+                gpu_memory_utilization = get_gpu_mem_utilization() / 1e9 if torch.cuda.is_available() else 0
 
-            # RENDER METRICS PROGRESS
-            pbar_message_dict = get_train_loop_description_dict(
-                logging_values, self.train_metrics, self.loss_logging_items_names, gpu_mem=gpu_memory_utilization
-            )
+                # RENDER METRICS PROGRESS
+                pbar_message_dict = get_train_loop_description_dict(
+                    logging_values, self.train_metrics, self.loss_logging_items_names, gpu_mem=gpu_memory_utilization
+                )
 
-            progress_bar_train_loader.set_postfix(**pbar_message_dict)
-            self.phase_callback_handler.on_train_batch_end(context)
+                progress_bar_train_loader.set_postfix(**pbar_message_dict)
+                self.phase_callback_handler.on_train_batch_end(context)
 
-            if self.max_train_batches is not None and self.max_train_batches - 1 <= batch_idx:
-                break
+                if self.max_train_batches is not None and self.max_train_batches - 1 <= batch_idx:
+                    break
 
-        self.train_monitored_values = sg_trainer_utils.update_monitored_values_dict(
-            monitored_values_dict=self.train_monitored_values, new_values_dict=pbar_message_dict
-        )
+            self.train_monitored_values = sg_trainer_utils.update_monitored_values_dict(
+                monitored_values_dict=self.train_monitored_values, new_values_dict=pbar_message_dict
+            )
 
         return logging_values
 
     def _get_losses(self, outputs: torch.Tensor, targets: torch.Tensor) -> Tuple[torch.Tensor, tuple]:
         # GET THE OUTPUT OF THE LOSS FUNCTION
         loss = self.criterion(outputs, targets)
         if isinstance(loss, tuple):
@@ -510,17 +528,16 @@
 
         self.results_titles = ["Train_" + t for t in self.loss_logging_items_names + get_metrics_titles(self.train_metrics)] + [
             "Valid_" + t for t in self.loss_logging_items_names + get_metrics_titles(self.valid_metrics)
         ]
 
         if self.training_params.average_best_models:
             self.model_weight_averaging = ModelWeightAveraging(
-                self.checkpoints_dir_path,
+                ckpt_dir=self.checkpoints_dir_path,
                 greater_is_better=self.greater_metric_to_watch_is_better,
-                source_ckpt_folder_name=self.source_ckpt_folder_name,
                 metric_to_watch=self.metric_to_watch,
                 metric_idx=self.metric_idx_in_results_tuple,
                 load_checkpoint=self.load_checkpoint,
             )
 
     def _backward_step(self, loss: torch.Tensor, epoch: int, batch_idx: int, context: PhaseContext, *args, **kwargs) -> None:
         """
@@ -637,17 +654,17 @@
         self.update_param_groups = hasattr(self.net.module, "update_param_groups")
 
         self.checkpoint = {}
         self.strict_load = core_utils.get_param(self.training_params, "resume_strict_load", StrictLoad.ON)
         self.load_ema_as_net = False
         self.load_checkpoint = core_utils.get_param(self.training_params, "resume", False)
         self.external_checkpoint_path = core_utils.get_param(self.training_params, "resume_path")
-        self.load_checkpoint = self.load_checkpoint or self.external_checkpoint_path is not None
         self.ckpt_name = core_utils.get_param(self.training_params, "ckpt_name", "ckpt_latest.pth")
-        self._load_checkpoint_to_model()
+        self.resume_from_remote_sg_logger = core_utils.get_param(self.training_params, "resume_from_remote_sg_logger", False)
+        self.load_checkpoint = self.load_checkpoint or self.external_checkpoint_path is not None or self.resume_from_remote_sg_logger
 
     def _init_arch_params(self) -> None:
         default_arch_params = HpmStruct()
         arch_params = getattr(self.net, "arch_params", default_arch_params)
         self.arch_params = default_arch_params
         if arch_params is not None:
             self.arch_params.override(**arch_params.to_dict())
@@ -986,23 +1003,38 @@
 
                 -   `max_train_batches`: int, for debug- when not None- will break out of inner train loop (i.e iterating over
                       train_loader) when reaching this number of batches. Usefull for debugging (default=None).
 
                 -   `max_valid_batches`: int, for debug- when not None- will break out of inner valid loop (i.e iterating over
                       valid_loader) when reaching this number of batches. Usefull for debugging (default=None).
 
+                -   `resume_from_remote_sg_logger`: bool (default=False),  bool (default=False), When true, ckpt_name (checkpoint filename
+                       to resume i.e ckpt_latest.pth bydefault) will be downloaded into the experiment checkpoints directory
+                       prior to loading weights, then training is resumed from that checkpoint. The source is unique to
+                       every logger, and currently supported for WandB loggers only.
+
+                       IMPORTANT: Only works for experiments that were ran with sg_logger_params.save_checkpoints_remote=True.
+                       IMPORTANT: For WandB loggers, one must also pass the run id through the wandb_id arg in sg_logger_params.
+
 
 
         :return:
         """
         global logger
         if training_params is None:
             training_params = dict()
-        self.train_loader = train_loader or self.train_loader
-        self.valid_loader = valid_loader or self.valid_loader
+
+        self.train_loader = train_loader if train_loader is not None else self.train_loader
+        self.valid_loader = valid_loader if valid_loader is not None else self.valid_loader
+
+        if self.train_loader is None:
+            raise ValueError("No `train_loader` found. Please provide a value for `train_loader`")
+
+        if self.valid_loader is None:
+            raise ValueError("No `valid_loader` found. Please provide a value for `valid_loader`")
 
         if hasattr(self.train_loader, "batch_sampler") and self.train_loader.batch_sampler is not None:
             batch_size = self.train_loader.batch_sampler.batch_size
         else:
             batch_size = self.train_loader.batch_size
 
         if len(self.train_loader.dataset) % batch_size != 0 and not self.train_loader.drop_last:
@@ -1023,14 +1055,17 @@
                     "If it doesnt, please use one of the following sampler: DistributedSampler, RepeatAugSampler"
                 )
         self.training_params = TrainingParams()
         self.training_params.override(**training_params)
 
         self.net = model
         self._prep_net_for_train()
+        if not self.ddp_silent_mode:
+            self._initialize_sg_logger_objects(additional_configs_to_log)
+        self._load_checkpoint_to_model()
 
         # SET RANDOM SEED
         random_seed(is_ddp=device_config.multi_gpu == MultiGPUMode.DISTRIBUTED_DATA_PARALLEL, device=device_config.device, seed=self.training_params.seed)
 
         silent_mode = self.training_params.silent_mode or self.ddp_silent_mode
         # METRICS
         self._set_train_metrics(train_metrics_list=self.training_params.train_metrics_list)
@@ -1120,16 +1155,14 @@
 
         self._add_metrics_update_callback(Phase.TRAIN_BATCH_END)
         self._add_metrics_update_callback(Phase.VALIDATION_BATCH_END)
 
         self.phase_callback_handler = CallbackHandler(callbacks=self.phase_callbacks)
 
         if not self.ddp_silent_mode:
-            self._initialize_sg_logger_objects(additional_configs_to_log)
-
             if self.training_params.dataset_statistics:
                 dataset_statistics_logger = DatasetStatisticsTensorboardLogger(self.sg_logger)
                 dataset_statistics_logger.analyze(self.train_loader, all_classes=self.classes, title="Train-set", anchors=self.net.module.arch_params.anchors)
                 dataset_statistics_logger.analyze(self.valid_loader, all_classes=self.classes, title="val-set")
 
         sg_trainer_utils.log_uncaught_exceptions(logger)
 
@@ -1476,24 +1509,27 @@
     def _load_checkpoint_to_model(self):  # noqa: C901 - too complex
         """
         Copies the source checkpoint to a local folder and loads the checkpoint's data to the model using the
          attributes:
 
          strict:           See StrictLoad class documentation for details.
          load_backbone:    loads the provided checkpoint to self.net.backbone instead of self.net
-         source_ckpt_folder_name: The folder where the checkpoint is saved. By default uses the self.experiment_name
 
         NOTE: 'acc', 'epoch', 'optimizer_state_dict' and the logs are NOT loaded if self.zeroize_prev_train_params
          is True
         """
+        with wait_for_the_master(get_local_rank()):
+            if self.resume_from_remote_sg_logger and not self.ddp_silent_mode:
+                self.sg_logger.download_remote_ckpt(ckpt_name=self.ckpt_name)
 
         if self.load_checkpoint or self.external_checkpoint_path:
             # GET LOCAL PATH TO THE CHECKPOINT FILE FIRST
+            ckpt_root_dir = str(Path(self.checkpoints_dir_path).parent)
             ckpt_local_path = get_ckpt_local_path(
-                source_ckpt_folder_name=self.source_ckpt_folder_name,
+                ckpt_root_dir=ckpt_root_dir,
                 experiment_name=self.experiment_name,
                 ckpt_name=self.ckpt_name,
                 external_checkpoint_path=self.external_checkpoint_path,
             )
 
             # LOAD CHECKPOINT TO MODEL
             self.checkpoint = load_checkpoint_to_model(
@@ -1781,100 +1817,101 @@
         :param metrics_progress_verbose: (bool) controls the verbosity of metrics progress (default=False).
             Slows down the program significantly.
 
         :return: results tuple (tuple) containing the loss items and metric values.
         """
 
         # THE DISABLE FLAG CONTROLS WHETHER THE PROGRESS BAR IS SILENT OR PRINTS THE LOGS
-        progress_bar_data_loader = tqdm(data_loader, bar_format="{l_bar}{bar:10}{r_bar}", dynamic_ncols=True, disable=silent_mode)
         loss_avg_meter = core_utils.utils.AverageMeter()
         logging_values = None
-        loss_tuple = None
+
         lr_warmup_epochs = self.training_params.lr_warmup_epochs if self.training_params else None
         context = PhaseContext(
             epoch=epoch,
             metrics_compute_fn=metrics,
             loss_avg_meter=loss_avg_meter,
             criterion=self.criterion,
             device=device_config.device,
             lr_warmup_epochs=lr_warmup_epochs,
             sg_logger=self.sg_logger,
             context_methods=self._get_context_methods(Phase.VALIDATION_BATCH_END),
         )
 
-        if not silent_mode:
-            # PRINT TITLES
-            pbar_start_msg = f"Validation epoch {epoch}" if evaluation_type == EvaluationType.VALIDATION else "Test"
-            progress_bar_data_loader.set_description(pbar_start_msg)
-
-        with torch.no_grad():
-            for batch_idx, batch_items in enumerate(progress_bar_data_loader):
-                batch_items = core_utils.tensor_container_to_device(batch_items, device_config.device, non_blocking=True)
-                inputs, targets, additional_batch_items = sg_trainer_utils.unpack_batch_items(batch_items)
-
-                # TRIGGER PHASE CALLBACKS CORRESPONDING TO THE EVALUATION TYPE
-                context.update_context(batch_idx=batch_idx, inputs=inputs, target=targets, **additional_batch_items)
-                if evaluation_type == EvaluationType.VALIDATION:
-                    self.phase_callback_handler.on_validation_batch_start(context)
-                else:
-                    self.phase_callback_handler.on_test_batch_start(context)
+        with tqdm(data_loader, bar_format="{l_bar}{bar:10}{r_bar}", dynamic_ncols=True, disable=silent_mode) as progress_bar_data_loader:
 
-                output = self.net(inputs)
-                context.update_context(preds=output)
-
-                if self.criterion is not None:
-                    # STORE THE loss_items ONLY, THE 1ST RETURNED VALUE IS THE loss FOR BACKPROP DURING TRAINING
-                    loss_tuple = self._get_losses(output, targets)[1].cpu()
-                    context.update_context(loss_log_items=loss_tuple)
-
-                # TRIGGER PHASE CALLBACKS CORRESPONDING TO THE EVALUATION TYPE
-                if evaluation_type == EvaluationType.VALIDATION:
-                    self.phase_callback_handler.on_validation_batch_end(context)
-                else:
-                    self.phase_callback_handler.on_test_batch_end(context)
-
-                # COMPUTE METRICS IF PROGRESS VERBOSITY IS SET
-                if metrics_progress_verbose and not silent_mode:
-                    # COMPUTE THE RUNNING USER METRICS AND LOSS RUNNING ITEMS. RESULT TUPLE IS THEIR CONCATENATION.
-                    logging_values = get_logging_values(loss_avg_meter, metrics, self.criterion)
-                    pbar_message_dict = get_train_loop_description_dict(logging_values, metrics, self.loss_logging_items_names)
-
-                    progress_bar_data_loader.set_postfix(**pbar_message_dict)
+            if not silent_mode:
+                # PRINT TITLES
+                pbar_start_msg = f"Validation epoch {epoch}" if evaluation_type == EvaluationType.VALIDATION else "Test"
+                progress_bar_data_loader.set_description(pbar_start_msg)
+
+            with torch.no_grad():
+                for batch_idx, batch_items in enumerate(progress_bar_data_loader):
+                    batch_items = core_utils.tensor_container_to_device(batch_items, device_config.device, non_blocking=True)
+                    inputs, targets, additional_batch_items = sg_trainer_utils.unpack_batch_items(batch_items)
+
+                    # TRIGGER PHASE CALLBACKS CORRESPONDING TO THE EVALUATION TYPE
+                    context.update_context(batch_idx=batch_idx, inputs=inputs, target=targets, **additional_batch_items)
+                    if evaluation_type == EvaluationType.VALIDATION:
+                        self.phase_callback_handler.on_validation_batch_start(context)
+                    else:
+                        self.phase_callback_handler.on_test_batch_start(context)
+
+                    output = self.net(inputs)
+                    context.update_context(preds=output)
+
+                    if self.criterion is not None:
+                        # STORE THE loss_items ONLY, THE 1ST RETURNED VALUE IS THE loss FOR BACKPROP DURING TRAINING
+                        loss_tuple = self._get_losses(output, targets)[1].cpu()
+                        context.update_context(loss_log_items=loss_tuple)
+
+                    # TRIGGER PHASE CALLBACKS CORRESPONDING TO THE EVALUATION TYPE
+                    if evaluation_type == EvaluationType.VALIDATION:
+                        self.phase_callback_handler.on_validation_batch_end(context)
+                    else:
+                        self.phase_callback_handler.on_test_batch_end(context)
+
+                    # COMPUTE METRICS IF PROGRESS VERBOSITY IS SET
+                    if metrics_progress_verbose and not silent_mode:
+                        # COMPUTE THE RUNNING USER METRICS AND LOSS RUNNING ITEMS. RESULT TUPLE IS THEIR CONCATENATION.
+                        logging_values = get_logging_values(loss_avg_meter, metrics, self.criterion)
+                        pbar_message_dict = get_train_loop_description_dict(logging_values, metrics, self.loss_logging_items_names)
+
+                        progress_bar_data_loader.set_postfix(**pbar_message_dict)
+
+                    if evaluation_type == EvaluationType.VALIDATION and self.max_valid_batches is not None and self.max_valid_batches - 1 <= batch_idx:
+                        break
+
+            # NEED TO COMPUTE METRICS FOR THE FIRST TIME IF PROGRESS VERBOSITY IS NOT SET
+            if not metrics_progress_verbose:
+                # COMPUTE THE RUNNING USER METRICS AND LOSS RUNNING ITEMS. RESULT TUPLE IS THEIR CONCATENATION.
+                logging_values = get_logging_values(loss_avg_meter, metrics, self.criterion)
+                pbar_message_dict = get_train_loop_description_dict(logging_values, metrics, self.loss_logging_items_names)
+
+                progress_bar_data_loader.set_postfix(**pbar_message_dict)
+
+            # TODO: SUPPORT PRINTING AP PER CLASS- SINCE THE METRICS ARE NOT HARD CODED ANYMORE (as done in
+            #  calc_batch_prediction_accuracy_per_class in metric_utils.py), THIS IS ONLY RELEVANT WHEN CHOOSING
+            #  DETECTIONMETRICS, WHICH ALREADY RETURN THE METRICS VALUEST HEMSELVES AND NOT THE ITEMS REQUIRED FOR SUCH
+            #  COMPUTATION. ALSO REMOVE THE BELOW LINES BY IMPLEMENTING CRITERION AS A TORCHMETRIC.
 
-                if evaluation_type == EvaluationType.VALIDATION and self.max_valid_batches is not None and self.max_valid_batches - 1 <= batch_idx:
-                    break
+            if device_config.multi_gpu == MultiGPUMode.DISTRIBUTED_DATA_PARALLEL:
+                logging_values = reduce_results_tuple_for_ddp(logging_values, next(self.net.parameters()).device)
 
-        # NEED TO COMPUTE METRICS FOR THE FIRST TIME IF PROGRESS VERBOSITY IS NOT SET
-        if not metrics_progress_verbose:
-            # COMPUTE THE RUNNING USER METRICS AND LOSS RUNNING ITEMS. RESULT TUPLE IS THEIR CONCATENATION.
-            logging_values = get_logging_values(loss_avg_meter, metrics, self.criterion)
             pbar_message_dict = get_train_loop_description_dict(logging_values, metrics, self.loss_logging_items_names)
 
-            progress_bar_data_loader.set_postfix(**pbar_message_dict)
-
-        # TODO: SUPPORT PRINTING AP PER CLASS- SINCE THE METRICS ARE NOT HARD CODED ANYMORE (as done in
-        #  calc_batch_prediction_accuracy_per_class in metric_utils.py), THIS IS ONLY RELEVANT WHEN CHOOSING
-        #  DETECTIONMETRICS, WHICH ALREADY RETURN THE METRICS VALUEST HEMSELVES AND NOT THE ITEMS REQUIRED FOR SUCH
-        #  COMPUTATION. ALSO REMOVE THE BELOW LINES BY IMPLEMENTING CRITERION AS A TORCHMETRIC.
-
-        if device_config.multi_gpu == MultiGPUMode.DISTRIBUTED_DATA_PARALLEL:
-            logging_values = reduce_results_tuple_for_ddp(logging_values, next(self.net.parameters()).device)
-
-        pbar_message_dict = get_train_loop_description_dict(logging_values, metrics, self.loss_logging_items_names)
-
-        self.valid_monitored_values = sg_trainer_utils.update_monitored_values_dict(
-            monitored_values_dict=self.valid_monitored_values, new_values_dict=pbar_message_dict
-        )
-
-        if not silent_mode and evaluation_type == EvaluationType.VALIDATION:
-            progress_bar_data_loader.write("===========================================================")
-            sg_trainer_utils.display_epoch_summary(
-                epoch=context.epoch, n_digits=4, train_monitored_values=self.train_monitored_values, valid_monitored_values=self.valid_monitored_values
+            self.valid_monitored_values = sg_trainer_utils.update_monitored_values_dict(
+                monitored_values_dict=self.valid_monitored_values, new_values_dict=pbar_message_dict
             )
-            progress_bar_data_loader.write("===========================================================")
+
+            if not silent_mode and evaluation_type == EvaluationType.VALIDATION:
+                progress_bar_data_loader.write("===========================================================")
+                sg_trainer_utils.display_epoch_summary(
+                    epoch=context.epoch, n_digits=4, train_monitored_values=self.train_monitored_values, valid_monitored_values=self.valid_monitored_values
+                )
+                progress_bar_data_loader.write("===========================================================")
 
         return logging_values
 
     def _instantiate_net(
         self, architecture: Union[torch.nn.Module, SgModule.__class__, str], arch_params: dict, checkpoint_params: dict, *args, **kwargs
     ) -> tuple:
         """
@@ -1994,7 +2031,341 @@
 
         if component_names is not None:
             self.loss_logging_items_names = [criterion_name + "/" + component_name for component_name in component_names]
             if self.metric_to_watch in component_names:
                 self.metric_to_watch = criterion_name + "/" + self.metric_to_watch
         else:
             self.loss_logging_items_names = [criterion_name]
+
+    @classmethod
+    def quantize_from_config(cls, cfg: Union[DictConfig, dict]) -> Tuple[nn.Module, Tuple]:
+        """
+        Perform quantization aware training (QAT) according to a recipe configuration.
+
+        This method will instantiate all the objects specified in the recipe, build and quantize the model,
+        and calibrate the quantized model. The resulting quantized model and the output of the trainer.train()
+        method will be returned.
+
+        The quantized model will be exported to ONNX along with other checkpoints.
+
+        The call to self.quantize (see docs in the next method) is done with the created
+         train_loader and valid_loader. If no calibration data loader is passed through cfg.calib_loader,
+         a train data laoder with the validation transforms is used for calibration.
+
+        :param cfg: The parsed DictConfig object from yaml recipe files or a dictionary.
+        :return: A tuple containing the quantized model and the output of trainer.train() method.
+
+        :raises ValueError: If the recipe does not have the required key `quantization_params` or
+        `checkpoint_params.checkpoint_path` in it.
+        :raises NotImplementedError: If the recipe requests multiple GPUs or num_gpus is not equal to 1.
+        :raises ImportError: If pytorch-quantization import was unsuccessful
+
+        """
+        if _imported_pytorch_quantization_failure is not None:
+            raise _imported_pytorch_quantization_failure
+
+        # INSTANTIATE ALL OBJECTS IN CFG
+        cfg = hydra.utils.instantiate(cfg)
+
+        # TRIGGER CFG MODIFYING CALLBACKS
+        cfg = cls._trigger_cfg_modifying_callbacks(cfg)
+
+        quantization_params = get_param(cfg, "quantization_params")
+
+        if quantization_params is None:
+            raise logger.warning("Your recipe does not include quantization_params. Using default quantization params.")
+
+        if get_param(cfg.checkpoint_params, "checkpoint_path") is None and get_param(cfg.checkpoint_params, "pretrained_weights") is None:
+            raise ValueError("Starting checkpoint / pretrained weights are a must for QAT finetuning.")
+
+        num_gpus = core_utils.get_param(cfg, "num_gpus")
+        multi_gpu = core_utils.get_param(cfg, "multi_gpu")
+        device = core_utils.get_param(cfg, "device")
+        if num_gpus != 1:
+            raise NotImplementedError(
+                f"Recipe requests multi_gpu={cfg.multi_gpu} and num_gpus={cfg.num_gpus}. QAT is proven to work correctly only with multi_gpu=OFF and num_gpus=1"
+            )
+
+        setup_device(device=device, multi_gpu=multi_gpu, num_gpus=num_gpus)
+
+        # INSTANTIATE DATA LOADERS
+        train_dataloader = dataloaders.get(
+            name=get_param(cfg, "train_dataloader"),
+            dataset_params=copy.deepcopy(cfg.dataset_params.train_dataset_params),
+            dataloader_params=copy.deepcopy(cfg.dataset_params.train_dataloader_params),
+        )
+
+        val_dataloader = dataloaders.get(
+            name=get_param(cfg, "val_dataloader"),
+            dataset_params=copy.deepcopy(cfg.dataset_params.val_dataset_params),
+            dataloader_params=copy.deepcopy(cfg.dataset_params.val_dataloader_params),
+        )
+
+        if "calib_dataloader" in cfg:
+            calib_dataloader_name = get_param(cfg, "calib_dataloader")
+            calib_dataloader_params = copy.deepcopy(cfg.dataset_params.calib_dataloader_params)
+            calib_dataset_params = copy.deepcopy(cfg.dataset_params.calib_dataset_params)
+        else:
+            calib_dataloader_name = get_param(cfg, "train_dataloader")
+            calib_dataloader_params = copy.deepcopy(cfg.dataset_params.train_dataloader_params)
+            calib_dataset_params = copy.deepcopy(cfg.dataset_params.train_dataset_params)
+
+            # if we use whole dataloader for calibration, don't shuffle it
+            # HistogramCalibrator collection routine is sensitive to order of batches and produces slightly different results
+            # if we use several batches, we don't want it to be from one class if it's sequential in dataloader
+            # model is in eval mode, so BNs will not be affected
+            calib_dataloader_params.shuffle = cfg.quantization_params.calib_params.num_calib_batches is not None
+            # we don't need training transforms during calibration, distribution of activations will be skewed
+            calib_dataset_params.transforms = cfg.dataset_params.val_dataset_params.transforms
+
+        calib_dataloader = dataloaders.get(
+            name=calib_dataloader_name,
+            dataset_params=calib_dataset_params,
+            dataloader_params=calib_dataloader_params,
+        )
+
+        # BUILD MODEL
+        model = models.get(
+            model_name=cfg.arch_params.get("model_name", None) or cfg.architecture,
+            num_classes=cfg.get("num_classes", None) or cfg.arch_params.num_classes,
+            arch_params=cfg.arch_params,
+            strict_load=cfg.checkpoint_params.strict_load,
+            pretrained_weights=cfg.checkpoint_params.pretrained_weights,
+            checkpoint_path=cfg.checkpoint_params.checkpoint_path,
+            load_backbone=False,
+        )
+
+        recipe_logged_cfg = {"recipe_config": OmegaConf.to_container(cfg, resolve=True)}
+        trainer = Trainer(experiment_name=cfg.experiment_name, ckpt_root_dir=get_param(cfg, "ckpt_root_dir"))
+
+        if quantization_params.ptq_only:
+            res = trainer.ptq(
+                calib_loader=calib_dataloader,
+                model=model,
+                quantization_params=quantization_params,
+                valid_loader=val_dataloader,
+                valid_metrics_list=cfg.training_hyperparams.valid_metrics_list,
+            )
+        else:
+            res = trainer.qat(
+                model=model,
+                quantization_params=quantization_params,
+                calib_loader=calib_dataloader,
+                valid_loader=val_dataloader,
+                train_loader=train_dataloader,
+                training_params=cfg.training_hyperparams,
+                additional_qat_configs_to_log=recipe_logged_cfg,
+            )
+
+        return model, res
+
+    def qat(
+        self,
+        calib_loader: DataLoader,
+        model: torch.nn.Module,
+        valid_loader: DataLoader,
+        train_loader: DataLoader,
+        training_params: Mapping = None,
+        quantization_params: Mapping = None,
+        additional_qat_configs_to_log: Dict = None,
+        valid_metrics_list: List[Metric] = None,
+    ):
+        """
+        Performs post-training quantization (PTQ), and then quantization-aware training (QAT).
+        Exports the ONNX models (ckpt_best.pth of QAT and the calibrated model) to the checkpoints directory.
+
+        :param calib_loader: DataLoader, data loader for calibration.
+
+        :param model: torch.nn.Module, Model to perform QAT/PTQ on. When None, will try to use the network from
+        previous self.train call(that is, if there was one - will try to use self.ema_model.ema if EMA was used,
+        otherwise self.net)
+
+
+        :param valid_loader: DataLoader, data loader for validation. Used both for validating the calibrated model after PTQ and during QAT.
+            When None, will try to use self.valid_loader if it was set in previous self.train(..) call (default=None).
+
+        :param train_loader: DataLoader, data loader for QA training, can be ignored when quantization_params["ptq_only"]=True (default=None).
+
+        :param quantization_params: Mapping, with the following entries:defaults-
+            selective_quantizer_params:
+              calibrator_w: "max"        # calibrator type for weights, acceptable types are ["max", "histogram"]
+              calibrator_i: "histogram"  # calibrator type for inputs acceptable types are ["max", "histogram"]
+              per_channel: True          # per-channel quantization of weights, activations stay per-tensor by default
+              learn_amax: False          # enable learnable amax in all TensorQuantizers using straight-through estimator
+              skip_modules:              # optional list of module names (strings) to skip from quantization
+
+            calib_params:
+              histogram_calib_method: "percentile"  # calibration method for all "histogram" calibrators,
+                                                                # acceptable types are ["percentile", "entropy", mse"],
+                                                                # "max" calibrators always use "max"
+
+              percentile: 99.99                     # percentile for all histogram calibrators with method "percentile",
+                                                    # other calibrators are not affected
+
+              num_calib_batches:                    # number of batches to use for calibration, if None, 512 / batch_size will be used
+              verbose: False                        # if calibrator should be verbose
+
+
+              When None, the above default config is used (default=None)
+
+
+        :param training_params: Mapping, training hyper parameters for QAT, same as in super.train(...). When None, will try to use self.training_params
+         which is set in previous self.train(..) call (default=None).
+
+        :param additional_qat_configs_to_log: Dict, Optional dictionary containing configs that will be added to the QA training's
+         sg_logger. Format should be {"Config_title_1": {...}, "Config_title_2":{..}}.
+
+        :param valid_metrics_list:  (list(torchmetrics.Metric)) metrics list for evaluation of the calibrated model.
+        When None, the validation metrics from training_params are used). (default=None).
+
+        :return: Validation results of the QAT model in case quantization_params['ptq_only']=False and of the PTQ
+        model otherwise.
+        """
+
+        if quantization_params is None:
+            quantization_params = load_recipe("quantization_params/default_quantization_params").quantization_params
+            logger.info(f"Using default quantization params: {quantization_params}")
+        valid_metrics_list = valid_metrics_list or get_param(training_params, "valid_metrics_list")
+
+        _ = self.ptq(
+            calib_loader=calib_loader,
+            model=model,
+            quantization_params=quantization_params,
+            valid_loader=valid_loader,
+            valid_metrics_list=valid_metrics_list,
+            deepcopy_model_for_export=True,
+        )
+        # TRAIN
+        model.train()
+        torch.cuda.empty_cache()
+
+        res = self.train(
+            model=model,
+            train_loader=train_loader,
+            valid_loader=valid_loader,
+            training_params=training_params,
+            additional_configs_to_log=additional_qat_configs_to_log,
+        )
+
+        # EXPORT QUANTIZED MODEL TO ONNX
+        input_shape = next(iter(valid_loader))[0].shape
+        os.makedirs(self.checkpoints_dir_path, exist_ok=True)
+        qdq_onnx_path = os.path.join(self.checkpoints_dir_path, f"{self.experiment_name}_{'x'.join((str(x) for x in input_shape))}_qat.onnx")
+
+        # TODO: modify SG's convert_to_onnx for quantized models and use it instead
+        export_quantized_module_to_onnx(
+            model=model.cpu(),
+            onnx_filename=qdq_onnx_path,
+            input_shape=input_shape,
+            input_size=input_shape,
+            train=False,
+        )
+        logger.info(f"Exported QAT ONNX to {qdq_onnx_path}")
+        return res
+
+    def ptq(
+        self,
+        calib_loader: DataLoader,
+        model: nn.Module,
+        valid_loader: DataLoader,
+        valid_metrics_list: List[torchmetrics.Metric],
+        quantization_params: Dict = None,
+        deepcopy_model_for_export: bool = False,
+    ):
+        """
+        Performs post-training quantization (calibration of the model)..
+
+        :param calib_loader: DataLoader, data loader for calibration.
+
+        :param model: torch.nn.Module, Model to perform calibration on. When None, will try to use self.net which is
+        set in previous self.train(..) call (default=None).
+
+        :param valid_loader: DataLoader, data loader for validation. Used both for validating the calibrated model.
+            When None, will try to use self.valid_loader if it was set in previous self.train(..) call (default=None).
+
+        :param quantization_params: Mapping, with the following entries:defaults-
+            selective_quantizer_params:
+              calibrator_w: "max"        # calibrator type for weights, acceptable types are ["max", "histogram"]
+              calibrator_i: "histogram"  # calibrator type for inputs acceptable types are ["max", "histogram"]
+              per_channel: True          # per-channel quantization of weights, activations stay per-tensor by default
+              learn_amax: False          # enable learnable amax in all TensorQuantizers using straight-through estimator
+              skip_modules:              # optional list of module names (strings) to skip from quantization
+
+            calib_params:
+              histogram_calib_method: "percentile"  # calibration method for all "histogram" calibrators,
+                                                                # acceptable types are ["percentile", "entropy", mse"],
+                                                                # "max" calibrators always use "max"
+
+              percentile: 99.99                     # percentile for all histogram calibrators with method "percentile",
+                                                    # other calibrators are not affected
+
+              num_calib_batches:                    # number of batches to use for calibration, if None, 512 / batch_size will be used
+              verbose: False                        # if calibrator should be verbose
+
+
+              When None, the above default config is used (default=None)
+
+
+
+        :param valid_metrics_list:  (list(torchmetrics.Metric)) metrics list for evaluation of the calibrated model.
+
+        :param deepcopy_model_for_export: bool, Whether to export deepcopy(model). Necessary in case further training is
+            performed and prep_model_for_conversion makes the network un-trainable (i.e RepVGG blocks).
+
+        :return: Validation results of the calibrated model.
+        """
+
+        if quantization_params is None:
+            quantization_params = load_recipe("quantization_params/default_quantization_params").quantization_params
+            logger.info(f"Using default quantization params: {quantization_params}")
+
+        selective_quantizer_params = get_param(quantization_params, "selective_quantizer_params")
+        calib_params = get_param(quantization_params, "calib_params")
+        model.to(device_config.device)
+        # QUANTIZE MODEL
+        model.eval()
+        fuse_repvgg_blocks_residual_branches(model)
+        q_util = SelectiveQuantizer(
+            default_quant_modules_calibrator_weights=get_param(selective_quantizer_params, "calibrator_w"),
+            default_quant_modules_calibrator_inputs=get_param(selective_quantizer_params, "calibrator_i"),
+            default_per_channel_quant_weights=get_param(selective_quantizer_params, "per_channel"),
+            default_learn_amax=get_param(selective_quantizer_params, "learn_amax"),
+            verbose=get_param(calib_params, "verbose"),
+        )
+        q_util.register_skip_quantization(layer_names=get_param(selective_quantizer_params, "skip_modules"))
+        q_util.quantize_module(model)
+        # CALIBRATE MODEL
+        logger.info("Calibrating model...")
+        calibrator = QuantizationCalibrator(
+            verbose=get_param(calib_params, "verbose"),
+            torch_hist=True,
+        )
+        calibrator.calibrate_model(
+            model,
+            method=get_param(calib_params, "histogram_calib_method"),
+            calib_data_loader=calib_loader,
+            num_calib_batches=get_param(calib_params, "num_calib_batches") or len(calib_loader),
+            percentile=get_param(calib_params, "percentile", 99.99),
+        )
+        calibrator.reset_calibrators(model)  # release memory taken by calibrators
+        # VALIDATE PTQ MODEL AND PRINT SUMMARY
+        logger.info("Validating PTQ model...")
+        valid_metrics_dict = self.test(model=model, test_loader=valid_loader, test_metrics_list=valid_metrics_list)
+        results = ["PTQ Model Validation Results"]
+        results += [f"   - {metric:10}: {value}" for metric, value in valid_metrics_dict.items()]
+        logger.info("\n".join(results))
+
+        input_shape = next(iter(valid_loader))[0].shape
+        os.makedirs(self.checkpoints_dir_path, exist_ok=True)
+        qdq_onnx_path = os.path.join(self.checkpoints_dir_path, f"{self.experiment_name}_{'x'.join((str(x) for x in input_shape))}_ptq.onnx")
+
+        # TODO: modify SG's convert_to_onnx for quantized models and use it instead
+        export_quantized_module_to_onnx(
+            model=model.cpu(),
+            onnx_filename=qdq_onnx_path,
+            input_shape=input_shape,
+            input_size=input_shape,
+            train=False,
+            deepcopy_model=deepcopy_model_for_export,
+        )
+
+        return valid_metrics_dict
```

## super_gradients/training/transforms/transforms.py

```diff
@@ -24,14 +24,15 @@
     _rescale_image,
     _rescale_bboxes,
     _get_center_padding_coordinates,
     _pad_image,
     _shift_bboxes,
     _rescale_xyxy_bboxes,
 )
+from super_gradients.training.utils.utils import ensure_is_tuple_of_two
 
 IMAGE_RESAMPLE_MODE = Image.BILINEAR
 MASK_RESAMPLE_MODE = Image.NEAREST
 
 logger = get_logger(__name__)
 
 
@@ -455,18 +456,18 @@
 
     :param input_dim:       Input dimension.
     :param prob:            Probability of applying mosaic.
     :param enable_mosaic:   Whether to apply mosaic at all (regardless of prob).
     :param border_value:    Value for filling borders after applying transforms.
     """
 
-    def __init__(self, input_dim: tuple, prob: float = 1.0, enable_mosaic: bool = True, border_value=114):
+    def __init__(self, input_dim: Union[int, Tuple[int, int]], prob: float = 1.0, enable_mosaic: bool = True, border_value=114):
         super(DetectionMosaic, self).__init__(additional_samples_count=3)
         self.prob = prob
-        self.input_dim = input_dim
+        self.input_dim = ensure_is_tuple_of_two(input_dim)
         self.enable_mosaic = enable_mosaic
         self.border_value = border_value
 
     def close(self):
         self.additional_samples_count = 0
         self.enable_mosaic = False
 
@@ -562,27 +563,27 @@
 
     def __init__(
         self,
         degrees: Union[tuple, float] = 10,
         translate: Union[tuple, float] = 0.1,
         scales: Union[tuple, float] = 0.1,
         shear: Union[tuple, float] = 10,
-        target_size: Optional[Tuple[int, int]] = (640, 640),
+        target_size: Union[int, Tuple[int, int], None] = (640, 640),
         filter_box_candidates: bool = False,
         wh_thr: float = 2,
         ar_thr: float = 20,
         area_thr: float = 0.1,
         border_value: int = 114,
     ):
         super(DetectionRandomAffine, self).__init__()
         self.degrees = degrees
         self.translate = translate
         self.scale = scales
         self.shear = shear
-        self.target_size = target_size
+        self.target_size = ensure_is_tuple_of_two(target_size)
         self.enable = True
         self.filter_box_candidates = filter_box_candidates
         self.wh_thr = wh_thr
         self.ar_thr = ar_thr
         self.area_thr = area_thr
         self.border_value = border_value
 
@@ -620,17 +621,25 @@
     :param mixup_scale:      Scale range for the additional loaded image for mixup.
     :param prob:             Probability of applying mixup.
     :param enable_mixup:     Whether to apply mixup at all (regardless of prob).
     :param flip_prob:        Probability to apply horizontal flip to the additional sample.
     :param border_value:     Value for filling borders after applying transform.
     """
 
-    def __init__(self, input_dim: tuple, mixup_scale: tuple, prob: float = 1.0, enable_mixup: bool = True, flip_prob: float = 0.5, border_value: int = 114):
+    def __init__(
+        self,
+        input_dim: Union[int, Tuple[int, int], None],
+        mixup_scale: tuple,
+        prob: float = 1.0,
+        enable_mixup: bool = True,
+        flip_prob: float = 0.5,
+        border_value: int = 114,
+    ):
         super(DetectionMixup, self).__init__(additional_samples_count=1, non_empty_targets=True)
-        self.input_dim = input_dim
+        self.input_dim = ensure_is_tuple_of_two(input_dim)
         self.mixup_scale = mixup_scale
         self.prob = prob
         self.enable_mixup = enable_mixup
         self.flip_prob = flip_prob
         self.border_value = border_value
 
     def close(self):
@@ -732,23 +741,23 @@
     """
     Preprocessing transform to pad image and bboxes to `input_dim` shape (rows, cols).
     Transform does center padding, so that input image with bboxes located in the center of the produced image.
 
     Note: This transformation assume that dimensions of input image is equal or less than `output_size`.
     """
 
-    def __init__(self, output_size: Tuple[int, int], pad_value: int):
+    def __init__(self, output_size: Union[int, Tuple[int, int], None], pad_value: int):
         """
         Constructor for DetectionPadToSize transform.
 
         :param output_size: Output image size (rows, cols)
         :param pad_value: Padding value for image
         """
         super().__init__()
-        self.output_size = output_size
+        self.output_size = ensure_is_tuple_of_two(output_size)
         self.pad_value = pad_value
 
     def __call__(self, sample: dict) -> dict:
         image, targets, crowd_targets = sample["image"], sample["target"], sample.get("crowd_target")
         padding_coordinates = _get_center_padding_coordinates(input_shape=image.shape, output_shape=self.output_size)
 
         sample["image"] = _pad_image(image=image, padding_coordinates=padding_coordinates, pad_value=self.pad_value)
@@ -771,17 +780,17 @@
 
     :param input_dim:   Final input dimension (default=(640,640))
     :param swap:        Image axis's to be rearranged.
     :param max_targets:
     :param pad_value:   Padding value for image.
     """
 
-    def __init__(self, input_dim: Tuple, swap: Tuple[int, ...] = (2, 0, 1), max_targets: int = 50, pad_value: int = 114):
+    def __init__(self, input_dim: Union[int, Tuple[int, int], None], swap: Tuple[int, ...] = (2, 0, 1), max_targets: int = 50, pad_value: int = 114):
         self.swap = swap
-        self.input_dim = input_dim
+        self.input_dim = ensure_is_tuple_of_two(input_dim)
         self.max_targets = max_targets
         self.pad_value = pad_value
 
     def __call__(self, sample: dict) -> dict:
         img, targets, crowd_targets = sample["image"], sample["target"], sample.get("crowd_target")
         img, r = _rescale_and_pad_to_size(img, self.input_dim, self.swap, self.pad_value)
 
@@ -830,31 +839,31 @@
 class DetectionRescale(DetectionTransform):
     """
     Resize image and bounding boxes to given image dimensions without preserving aspect ratio
 
     :param output_shape: (rows, cols)
     """
 
-    def __init__(self, output_shape: Tuple[int, int]):
+    def __init__(self, output_shape: Union[int, Tuple[int, int]]):
         super().__init__()
-        self.output_shape = output_shape
+        self.output_shape = ensure_is_tuple_of_two(output_shape)
 
     def __call__(self, sample: dict) -> dict:
         image, targets, crowd_targets = sample["image"], sample["target"], sample.get("crowd_target")
 
-        sy, sx = (self.output_shape[0] / image.shape[0], self.output_shape[1] / image.shape[1])
+        sy, sx = float(self.output_shape[0]) / float(image.shape[0]), float(self.output_shape[1]) / float(image.shape[1])
 
         sample["image"] = _rescale_image(image=image, target_shape=self.output_shape)
         sample["target"] = _rescale_bboxes(targets, scale_factors=(sy, sx))
         if crowd_targets is not None:
             sample["crowd_target"] = _rescale_bboxes(crowd_targets, scale_factors=(sy, sx))
         return sample
 
     def get_equivalent_preprocessing(self) -> List[Dict]:
-        return [{Processings.DetectionRescale: {"output_shape": self.output_size}}]
+        return [{Processings.DetectionRescale: {"output_shape": self.output_shape}}]
 
 
 @register_transform(Transforms.DetectionRandomRotate90)
 class DetectionRandomRotate90(DetectionTransform):
     def __init__(self, prob: float = 0.5):
         super().__init__()
         self.prob = prob
@@ -1006,15 +1015,15 @@
     :param max_targets:        Max objects in single image, padding target to this size.
     """
 
     @resolve_param("input_format", ConcatenatedTensorFormatFactory())
     @resolve_param("output_format", ConcatenatedTensorFormatFactory())
     def __init__(
         self,
-        input_dim: Optional[tuple] = None,
+        input_dim: Union[int, Tuple[int, int], None] = None,
         input_format: ConcatenatedTensorFormat = XYXY_LABEL,
         output_format: ConcatenatedTensorFormat = LABEL_CXCYWH,
         min_bbox_edge_size: float = 1,
         max_targets: int = 120,
     ):
         super(DetectionTargetsFormatTransform, self).__init__()
         if isinstance(input_format, DetectionTargetsFormat) or isinstance(output_format, DetectionTargetsFormat):
@@ -1027,14 +1036,15 @@
         self.input_format = input_format
         self.output_format = output_format
         self.max_targets = max_targets
         self.min_bbox_edge_size = min_bbox_edge_size
         self.input_dim = None
 
         if input_dim is not None:
+            input_dim = ensure_is_tuple_of_two(input_dim)
             self._setup_input_dim_related_params(input_dim)
 
     def _setup_input_dim_related_params(self, input_dim: tuple):
         """Setup all the parameters that are related to input_dim."""
         self.input_dim = input_dim
         self.min_bbox_edge_size = self.min_bbox_edge_size / max(input_dim) if self.output_format.bboxes_format.format.normalized else self.min_bbox_edge_size
         self.targets_format_converter = ConcatenatedTensorFormatConverter(
```

## super_gradients/training/utils/__init__.py

```diff
@@ -1,8 +1,17 @@
-from super_gradients.training.utils.utils import Timer, HpmStruct, WrappedModel, convert_to_tensor, get_param, tensor_container_to_device, random_seed
+from super_gradients.training.utils.utils import (
+    Timer,
+    HpmStruct,
+    WrappedModel,
+    convert_to_tensor,
+    get_param,
+    tensor_container_to_device,
+    random_seed,
+    make_divisible,
+)
 from super_gradients.training.utils.checkpoint_utils import adapt_state_dict_to_fit_model_layer_names, raise_informative_runtime_error
 from super_gradients.training.utils.version_utils import torch_version_is_greater_or_equal
 from super_gradients.training.utils.config_utils import raise_if_unused_params, warn_if_unused_params
 from super_gradients.training.utils.early_stopping import EarlyStop
 from super_gradients.training.utils.pose_estimation import DEKRPoseEstimationDecodeCallback, DEKRVisualizationCallback
 
 __all__ = [
@@ -17,8 +26,9 @@
     "random_seed",
     "torch_version_is_greater_or_equal",
     "raise_if_unused_params",
     "warn_if_unused_params",
     "EarlyStop",
     "DEKRPoseEstimationDecodeCallback",
     "DEKRVisualizationCallback",
+    "make_divisible",
 ]
```

## super_gradients/training/utils/checkpoint_utils.py

```diff
@@ -1,22 +1,23 @@
+import collections
 import os
 import tempfile
+from typing import Union, Mapping
+
 import pkg_resources
-import collections
 import torch
+from torch import nn, Tensor
 
 from super_gradients.common.abstractions.abstract_logger import get_logger
 from super_gradients.common.data_interface.adnn_model_repository_data_interface import ADNNModelRepositoryDataInterfaces
+from super_gradients.common.data_types import StrictLoad
 from super_gradients.common.decorators.explicit_params_validator import explicit_params_validation
 from super_gradients.module_interfaces import HasPredict
 from super_gradients.training.pretrained_models import MODEL_URLS
-from super_gradients.common.data_types import StrictLoad
-
-from torch import nn, Tensor
-from typing import Union, Mapping
+from super_gradients.training.utils.distributed_training_utils import get_local_rank, wait_for_the_master
 
 try:
     from torch.hub import download_url_to_file, load_state_dict_from_url
 except (ModuleNotFoundError, ImportError, NameError):
     from torch.hub import _download_url_to_file as download_url_to_file
 
 
@@ -116,29 +117,39 @@
             model_checkpoints_data_interface.load_all_remote_log_files(
                 model_name=remote_ckpt_source_dir, model_checkpoint_local_dir=download_ckpt_destination_dir
             )
 
     if path_src == "url":
         ckpt_file_full_local_path = download_ckpt_destination_dir + os.path.sep + ckpt_filename
         # DOWNLOAD THE FILE FROM URL TO THE DESTINATION FOLDER
-        download_url_to_file(remote_ckpt_source_dir, ckpt_file_full_local_path, progress=True)
+        with wait_for_the_master(get_local_rank()):
+            download_url_to_file(remote_ckpt_source_dir, ckpt_file_full_local_path, progress=True)
 
     return ckpt_file_full_local_path
 
 
-def read_ckpt_state_dict(ckpt_path: str, device="cpu"):
-    if not os.path.exists(ckpt_path):
-        raise FileNotFoundError(f"Incorrect Checkpoint path: {ckpt_path} (This should be an absolute path)")
+def read_ckpt_state_dict(ckpt_path: str, device="cpu") -> Mapping[str, torch.Tensor]:
+    """
+    Reads a checkpoint state dict from a given path or url
 
-    if device == "cuda":
-        state_dict = torch.load(ckpt_path)
+    :param ckpt_path: Checkpoint path or url
+    :param device: Target devide where tensors should be loaded
+    :return: Checkpoint state dict object
+    """
 
+    if ckpt_path.startswith("https://"):
+        with wait_for_the_master(get_local_rank()):
+            state_dict = load_state_dict_from_url(ckpt_path, progress=False, map_location=device)
+        return state_dict
     else:
-        state_dict = torch.load(ckpt_path, map_location=lambda storage, loc: storage)
-    return state_dict
+        if not os.path.exists(ckpt_path):
+            raise FileNotFoundError(f"Incorrect Checkpoint path: {ckpt_path} (This should be an absolute path)")
+
+        state_dict = torch.load(ckpt_path, map_location=device)
+        return state_dict
 
 
 def adapt_state_dict_to_fit_model_layer_names(model_state_dict: dict, source_ckpt: dict, exclude: list = [], solver: callable = None):
     """
     Given a model state dict and source checkpoints, the method tries to correct the keys in the model_state_dict to fit
     the ckpt in order to properly load the weights into the model. If unsuccessful - returns None
         :param model_state_dict:               the model state_dict
@@ -202,18 +213,14 @@
     :param load_processing_params: Whether to call set_dataset_processing_params on "processing_params" entry inside the
      checkpoint file (default=False).
     :return:
     """
     if isinstance(strict, str):
         strict = StrictLoad(strict)
 
-    if ckpt_local_path is None or not os.path.exists(ckpt_local_path):
-        error_msg = "Error - loading Model Checkpoint: Path {} does not exist".format(ckpt_local_path)
-        raise RuntimeError(error_msg)
-
     if load_backbone and not hasattr(net, "backbone"):
         raise ValueError("No backbone attribute in net - Can't load backbone weights")
 
     # LOAD THE LOCAL CHECKPOINT PATH INTO A state_dict OBJECT
     checkpoint = read_ckpt_state_dict(ckpt_path=ckpt_local_path)
 
     if load_ema_as_net:
@@ -304,15 +311,16 @@
             "License Notification: YOLO-NAS pre-trained weights are subjected to the specific license terms and conditions detailed in \n"
             "https://github.com/Deci-AI/super-gradients/blob/master/LICENSE.YOLONAS.md\n"
             "By downloading the pre-trained weight files you agree to comply with these terms."
         )
 
     unique_filename = url.split("https://sghub.deci.ai/models/")[1].replace("/", "_").replace(" ", "_")
     map_location = torch.device("cpu")
-    pretrained_state_dict = load_state_dict_from_url(url=url, map_location=map_location, file_name=unique_filename)
+    with wait_for_the_master(get_local_rank()):
+        pretrained_state_dict = load_state_dict_from_url(url=url, map_location=map_location, file_name=unique_filename)
     _load_weights(architecture, model, pretrained_state_dict)
 
 
 def _load_weights(architecture, model, pretrained_state_dict):
     if "ema_net" in pretrained_state_dict.keys():
         pretrained_state_dict["net"] = pretrained_state_dict["ema_net"]
     solver = _yolox_ckpt_solver if "yolox" in architecture else None
```

## super_gradients/training/utils/detection_utils.py

```diff
@@ -387,15 +387,15 @@
         class_name = class_names[class_id]
 
         if is_target:
             title = f"[GT] {class_name}"
         else:
             title = f'[Pred] {class_name}  {str(round(pred_conf, 2)) if pred_conf is not None else ""}'
 
-        draw_bbox(image=image_np, title=title, x1=x1, y1=y1, x2=x2, y2=y2, box_thickness=box_thickness, color=color)
+        image_np = draw_bbox(image=image_np, title=title, x1=x1, y1=y1, x2=x2, y2=y2, box_thickness=box_thickness, color=color)
         return image_np
 
     @staticmethod
     def _visualize_image(
         image_np: np.ndarray,
         pred_boxes: np.ndarray,
         target_boxes: np.ndarray,
```

## super_gradients/training/utils/utils.py

```diff
@@ -1,44 +1,49 @@
+import collections
+import math
 import os
-import tarfile
+import random
 import re
-import math
+import tarfile
 import time
-from functools import lru_cache
+import inspect
+from functools import lru_cache, wraps
+from importlib import import_module
+from itertools import islice
+
 from pathlib import Path
 from typing import Mapping, Optional, Tuple, Union, List, Dict, Any, Iterable
 from zipfile import ZipFile
-from jsonschema import validate
-from itertools import islice
 
-from PIL import Image, ExifTags
+import numpy as np
 import torch
 import torch.nn as nn
-
-# These functions changed from torch 1.2 to torch 1.3
-
-import random
-import numpy as np
-from importlib import import_module
+from PIL import Image, ExifTags
+from jsonschema import validate
 
 from super_gradients.common.abstractions.abstract_logger import get_logger
 
+# These functions changed from torch 1.2 to torch 1.3
+
 logger = get_logger(__name__)
 
 
 def empty_list():
     """Instantiate an empty list. This is a workaround to generate a list with a function call in hydra, instead of the "[]"."""
     return list()
 
 
-def convert_to_tensor(array):
+def convert_to_tensor(array, dtype=None, device=None):
     """Converts numpy arrays and lists to Torch tensors before calculation losses
     :param array: torch.tensor / Numpy array / List
     """
-    return torch.FloatTensor(array) if type(array) != torch.Tensor else array
+    if not torch.is_tensor(array):
+        array = torch.tensor(array)
+
+    return array.to(device=device, dtype=dtype)
 
 
 class HpmStruct:
     def __init__(self, **entries):
         self.__dict__.update(entries)
         self.schema = None
 
@@ -77,14 +82,52 @@
         super(WrappedModel, self).__init__()
         self.module = module  # that I actually define.
 
     def forward(self, x):
         return self.module(x)
 
 
+def arch_params_deprecated(func):
+    """
+    Since initialization of arch_params is deprecated and will be removed, this decorator will be used to wrap the _init_
+    function of some models. It will unwrap the parameters of the function and will log a warning.
+    """
+
+    @wraps(func)
+    def wrapper(*args, **kwargs):
+
+        func_args = inspect.getfullargspec(func).args
+        _args = []
+        if "arch_params" in kwargs:
+            _arch_params = kwargs.get("arch_params", kwargs).to_dict()
+        elif len(args) > 1 and isinstance(args[1], HpmStruct):
+            _arch_params = args[1].to_dict()  # when called from inheritance
+            _args.append(args[0])
+        elif len(args) > 0 and isinstance(args[0], HpmStruct):
+            _arch_params = args[0].to_dict()
+        else:
+            return func(*args, **kwargs)
+
+        _kwargs = dict()
+        for param_name in func_args:
+            if param_name in _arch_params:
+                _kwargs[param_name] = _arch_params[param_name]
+            if param_name in kwargs:
+                _kwargs[param_name] = kwargs[param_name]
+
+        logger.warning(
+            f"The {func.__qualname__} received `arch_params` argument which is deprecated and will be removed in next versions. "
+            f"Please change the signature of the __init__ method to take explicit list arguments instead: "
+            f"{func.__qualname__}({', '.join(_kwargs.keys())})"
+        )
+        return func(*_args, **_kwargs)
+
+    return wrapper
+
+
 class Timer:
     """A class to measure time handling both GPU & CPU processes
     Returns time in milliseconds"""
 
     def __init__(self, device: str):
         """
         :param device: str
@@ -534,7 +577,23 @@
     it = iter(iterable)
     while True:
         batch = tuple(islice(it, batch_size))
         if batch:
             yield batch
         else:
             return
+
+
+def ensure_is_tuple_of_two(inputs: Union[Any, Iterable[Any], None]) -> Union[Tuple[Any, Any], None]:
+    """
+    Checks input and converts it to a tuple of length two. If input is None returns None.
+    :param inputs: Input argument, either a number or a tuple of two numbers.
+    :return: Tuple of two numbers if input is not None, otherwise - None.
+    """
+    if inputs is None:
+        return None
+
+    if isinstance(inputs, collections.Iterable) and not isinstance(inputs, str):
+        a, b = inputs
+        return a, b
+
+    return inputs, inputs
```

## super_gradients/training/utils/weight_averaging_utils.py

```diff
@@ -1,12 +1,11 @@
 import os
 import torch
 import numpy as np
-import pkg_resources
-from super_gradients.training import utils as core_utils
+from super_gradients.training.utils.checkpoint_utils import read_ckpt_state_dict
 from super_gradients.training.utils.utils import move_state_dict_to_device
 
 
 class ModelWeightAveraging:
     """
     Utils class for managing the averaging of the best several snapshots into a single model.
     A snapshot dictionary file and the average model will be saved / updated at every epoch and evaluated only when
@@ -14,57 +13,47 @@
     The snapshot dict will be managed on cpu.
     """
 
     def __init__(
         self,
         ckpt_dir,
         greater_is_better,
-        source_ckpt_folder_name=None,
         metric_to_watch="acc",
         metric_idx=1,
         load_checkpoint=False,
         number_of_models_to_average=10,
     ):
         """
         Init the ModelWeightAveraging
-        :param checkpoint_dir: the directory where the checkpoints are saved
+        :param ckpt_dir: the directory where the checkpoints are saved
         :param metric_to_watch: monitoring loss or acc, will be identical to that which determines best_model
         :param metric_idx:
         :param load_checkpoint: whether to load pre-existing snapshot dict.
         :param number_of_models_to_average: number of models to average
         """
 
-        if source_ckpt_folder_name is not None:
-            source_ckpt_file = os.path.join(source_ckpt_folder_name, "averaging_snapshots.pkl")
-            source_ckpt_file = pkg_resources.resource_filename("checkpoints", source_ckpt_file)
         self.averaging_snapshots_file = os.path.join(ckpt_dir, "averaging_snapshots.pkl")
         self.number_of_models_to_average = number_of_models_to_average
         self.metric_to_watch = metric_to_watch
         self.metric_idx = metric_idx
         self.greater_is_better = greater_is_better
 
         # if continuing training, copy previous snapshot dict if exist
-        if load_checkpoint and source_ckpt_folder_name is not None and os.path.isfile(source_ckpt_file):
-            averaging_snapshots_dict = core_utils.load_checkpoint(
-                ckpt_destination_dir=ckpt_dir,
-                source_ckpt_folder_name=source_ckpt_folder_name,
-                ckpt_filename="averaging_snapshots.pkl",
-                load_weights_only=False,
-                overwrite_local_ckpt=True,
-            )
+        if load_checkpoint and ckpt_dir is not None and os.path.isfile(self.averaging_snapshots_file):
+            averaging_snapshots_dict = read_ckpt_state_dict(self.averaging_snapshots_file)
 
         else:
             averaging_snapshots_dict = {"snapshot" + str(i): None for i in range(self.number_of_models_to_average)}
             # if metric to watch is acc, hold a zero array, if loss hold inf array
             if self.greater_is_better:
                 averaging_snapshots_dict["snapshots_metric"] = -1 * np.inf * np.ones(self.number_of_models_to_average)
             else:
                 averaging_snapshots_dict["snapshots_metric"] = np.inf * np.ones(self.number_of_models_to_average)
 
-        torch.save(averaging_snapshots_dict, self.averaging_snapshots_file)
+            torch.save(averaging_snapshots_dict, self.averaging_snapshots_file)
 
     def update_snapshots_dict(self, model, validation_results_tuple):
         """
         Update the snapshot dict and returns the updated average model for saving
         :param model: the latest model
         :param validation_results_tuple: performance of the latest model
         """
```

## super_gradients/training/utils/callbacks/callbacks.py

```diff
@@ -1,21 +1,21 @@
 import copy
 import math
 import os
 import signal
 import time
-from typing import List, Union, Optional
+from typing import List, Union, Optional, Sequence
 
 import csv
 import cv2
 import numpy as np
 import onnx
 import onnxruntime
 import torch
-from deprecate import deprecated
+from deprecated import deprecated
 
 from super_gradients.common.abstractions.abstract_logger import get_logger
 from super_gradients.common.plugins.deci_client import DeciClient
 from super_gradients.common.registry.registry import register_lr_scheduler, register_lr_warmup, register_callback
 from super_gradients.common.object_names import LRSchedulers, LRWarmups, Callbacks
 from super_gradients.training.utils.callbacks.base_callbacks import PhaseCallback, PhaseContext, Phase, Callback
 from super_gradients.training.utils.detection_utils import DetectionVisualization, DetectionPostPredictionCallback
@@ -40,29 +40,33 @@
 @register_callback(Callbacks.MODEL_CONVERSION_CHECK)
 class ModelConversionCheckCallback(PhaseCallback):
     """
     Pre-training callback that verifies model conversion to onnx given specified conversion parameters.
 
     The model is converted, then inference is applied with onnx runtime.
 
-    Use this callback wit hthe same args as DeciPlatformCallback to prevent conversion fails at the end of training.
+    Use this callback with the same args as DeciPlatformCallback to prevent conversion fails at the end of training.
 
-    :param model_meta_data:         Model's meta-data object. Type: ModelMetadata/
+    :param model_name:              Model's name
+    :param input_dimensions:        Model's input dimensions
+    :param primary_batch_size:      Model's primary batch size
     :param opset_version:           (default=11)
     :param do_constant_folding:     (default=True)
     :param dynamic_axes:            (default={'input': {0: 'batch_size'}, 'output': {0: 'batch_size'}})
     :param input_names:             (default=["input"])
     :param output_names:            (default=["output"])
     :param rtol:                    (default=1e-03)
     :param atol:                    (default=1e-05)
     """
 
-    def __init__(self, model_meta_data, **kwargs):
+    def __init__(self, model_name: str, input_dimensions: Sequence[int], primary_batch_size: int, **kwargs):
         super(ModelConversionCheckCallback, self).__init__(phase=Phase.PRE_TRAINING)
-        self.model_meta_data = model_meta_data
+        self.model_name = model_name
+        self.input_dimensions = input_dimensions
+        self.primary_batch_size = primary_batch_size
 
         self.opset_version = kwargs.get("opset_version", 10)
         self.do_constant_folding = kwargs.get("do_constant_folding", None) if kwargs.get("do_constant_folding", None) else True
         self.input_names = kwargs.get("input_names") or ["input"]
         self.output_names = kwargs.get("output_names") or ["output"]
         self.dynamic_axes = kwargs.get("dynamic_axes") or {"input": {0: "batch_size"}, "output": {0: "batch_size"}}
 
@@ -71,19 +75,19 @@
 
     def __call__(self, context: PhaseContext):
         model = copy.deepcopy(context.net.module)
         model = model.cpu()
         model.eval()  # Put model into eval mode
 
         if hasattr(model, "prep_model_for_conversion"):
-            model.prep_model_for_conversion(input_size=self.model_meta_data.input_dimensions)
+            model.prep_model_for_conversion(input_size=self.input_dimensions)
 
-        x = torch.randn(self.model_meta_data.primary_batch_size, *self.model_meta_data.input_dimensions, requires_grad=False)
+        x = torch.randn(self.primary_batch_size, *self.input_dimensions, requires_grad=False)
 
-        tmp_model_path = os.path.join(context.ckpt_dir, self.model_meta_data.name + "_tmp.onnx")
+        tmp_model_path = os.path.join(context.ckpt_dir, self.model_name + "_tmp.onnx")
 
         with torch.no_grad():
             torch_out = model(x)
 
         torch.onnx.export(
             model,  # Model being run
             x,  # Model input (or a tuple for multiple inputs)
@@ -122,32 +126,51 @@
     Post-training callback for uploading and optimizing a model.
 
     :param model_meta_data:             Model's meta-data object. Type: ModelMetadata
     :param optimization_request_form:   Optimization request form object. Type: OptimizationRequestForm
     :param ckpt_name:                   Checkpoint filename, inside the checkpoint directory.
     """
 
-    def __init__(self, model_meta_data, optimization_request_form, ckpt_name: str = "ckpt_best.pth", **kwargs):
+    def __init__(
+        self,
+        model_name: str,
+        input_dimensions: Sequence[int],
+        target_hardware_types: "Optional[List[str]]" = None,
+        target_batch_size: "Optional[int]" = None,
+        target_quantization_level: "Optional[str]" = None,
+        ckpt_name: str = "ckpt_best.pth",
+        **kwargs,
+    ):
         super().__init__(phase=Phase.POST_TRAINING)
-        self.model_meta_data = model_meta_data
-        self.optimization_request_form = optimization_request_form
+        self.input_dimensions = input_dimensions
+        self.model_name = model_name
+        self.target_hardware_types = target_hardware_types
+        self.target_batch_size = target_batch_size
+        self.target_quantization_level = target_quantization_level
         self.ckpt_name = ckpt_name
         self.platform_client = DeciClient()
 
     @staticmethod
     def log_optimization_failed():
         logger.info("We couldn't finish your model optimization. Visit https://console.deci.ai for details")
 
     def upload_model(self, model):
         """
         This function will upload the trained model to the Deci Lab
 
         :param model: The resulting model from the training process
         """
-        self.platform_client.upload_model(model=model, model_meta_data=self.model_meta_data, optimization_request_form=self.optimization_request_form)
+        self.platform_client.upload_model(
+            model=model,
+            name=self.model_name,
+            input_dimensions=self.input_dimensions,
+            target_hardware_types=self.target_hardware_types,
+            target_batch_size=self.target_batch_size,
+            target_quantization_level=self.target_quantization_level,
+        )
 
     def get_optimization_status(self, optimized_model_name: str):
         """
         This function will do fetch the optimized version of the trained model and check on its benchmark status.
         The status will be checked against the server every 30 seconds and the process will timeout after 30 minutes
         or log about the successful optimization - whichever happens first.
 
@@ -183,18 +206,18 @@
             model = copy.deepcopy(context.net)
             model_state_dict_path = os.path.join(context.ckpt_dir, self.ckpt_name)
             model_state_dict = torch.load(model_state_dict_path)["net"]
             model.load_state_dict(state_dict=model_state_dict)
 
             model = model.module.cpu()
             if hasattr(model, "prep_model_for_conversion"):
-                model.prep_model_for_conversion(input_size=self.model_meta_data.input_dimensions)
+                model.prep_model_for_conversion(input_size=self.input_dimensions)
 
             self.upload_model(model=model)
-            model_name = self.model_meta_data.name
+            model_name = self.model_name
             logger.info(f"Successfully added {model_name} to the model repository")
 
             optimized_model_name = f"{model_name}_1_1"
             logger.info("We'll wait for the scheduled optimization to finish. Please don't close this window")
             success = self.get_optimization_status(optimized_model_name=optimized_model_name)
             if success:
                 logger.info("Successfully finished your model optimization. Visit https://console.deci.ai for details")
@@ -472,15 +495,15 @@
 
 @register_lr_scheduler(LRSchedulers.FUNCTION)
 class FunctionLRCallback(LRCallbackBase):
     """
     Hard coded rate scheduling for user defined lr scheduling function.
     """
 
-    @deprecated(target=None, deprecated_in="3.6.0", remove_in="4.0.0")
+    @deprecated(version="3.2.0", reason="This callback is deprecated and will be removed in future versions.")
     def __init__(self, max_epochs, lr_schedule_function, **kwargs):
         super(FunctionLRCallback, self).__init__(Phase.TRAIN_BATCH_STEP, **kwargs)
         assert callable(lr_schedule_function), "self.lr_function must be callable"
         self.lr_schedule_function = lr_schedule_function
         self.max_epochs = max_epochs
 
     def is_lr_scheduling_enabled(self, context):
```

## super_gradients/training/utils/pose_estimation/__init__.py

```diff
@@ -1,4 +1,5 @@
 from .dekr_decode_callbacks import DEKRPoseEstimationDecodeCallback
 from .dekr_visualization_callbacks import DEKRVisualizationCallback
+from .rescoring_callback import RescoringPoseEstimationDecodeCallback
 
-__all__ = ["DEKRPoseEstimationDecodeCallback", "DEKRVisualizationCallback"]
+__all__ = ["DEKRPoseEstimationDecodeCallback", "DEKRVisualizationCallback", "RescoringPoseEstimationDecodeCallback"]
```

## super_gradients/training/utils/pose_estimation/dekr_decode_callbacks.py

```diff
@@ -172,18 +172,19 @@
     :return Tuple of (poses, scores)
     """
     assert len(poses) == 1
 
     pose_score = torch.cat([pose[:, :, 2:] for pose in poses], dim=0)
     pose_coord = torch.cat([pose[:, :, :2] for pose in poses], dim=0)
 
-    if pose_coord.shape[0] == 0:
-        return [], []
-
     num_people, num_joints, _ = pose_coord.shape
+
+    if num_people == 0:
+        return np.zeros((0, num_joints, 3), dtype=np.float32), np.zeros((0,), dtype=np.float32)
+
     heatval = _get_heat_value(pose_coord, heatmap_avg[0])
     heat_score = (torch.sum(heatval, dim=1) / num_joints)[:, 0]
 
     pose_score = pose_score * heatval
     poses = torch.cat([pose_coord.cpu(), pose_score.cpu()], dim=2)
 
     keep_pose_inds = _nms_core(pose_coord, heat_score, nms_threshold=nms_threshold, nms_num_threshold=nms_num_threshold)
@@ -194,15 +195,15 @@
         heat_score, topk_inds = torch.topk(heat_score, max_num_people)
         poses = poses[topk_inds]
 
     poses = poses.numpy()
     if len(poses):
         scores = poses[:, :, 2].mean(axis=1)
     else:
-        scores = []
+        return np.zeros((0, num_joints, 3), dtype=np.float32), np.zeros((0,), dtype=np.float32)
     return poses, scores
 
 
 def aggregate_results(heatmap: Tensor, posemap: Tensor, output_stride: int, keypoint_threshold: float, max_num_people: int) -> Tuple[Tensor, List[Tensor]]:
     """
     Get initial pose proposals and aggregate the results of all scale.
     Not this implementation works only for batch size of 1.
```

## super_gradients/training/utils/quantization/export.py

```diff
@@ -1,7 +1,9 @@
+from copy import deepcopy
+
 import torch
 from torch.onnx import TrainingMode
 
 from super_gradients.common.abstractions.abstract_logger import get_logger
 
 logger = get_logger(__name__)
 
@@ -10,27 +12,34 @@
 
     _imported_pytorch_quantization_failure = None
 except (ImportError, NameError, ModuleNotFoundError) as import_err:
     logger.warning("Failed to import pytorch_quantization")
     _imported_pytorch_quantization_failure = import_err
 
 
-def export_quantized_module_to_onnx(model: torch.nn.Module, onnx_filename: str, input_shape: tuple, train: bool = False, to_cpu: bool = True, **kwargs):
+def export_quantized_module_to_onnx(
+    model: torch.nn.Module, onnx_filename: str, input_shape: tuple, train: bool = False, to_cpu: bool = True, deepcopy_model=False, **kwargs
+):
     """
     Method for exporting onnx after QAT.
 
     :param to_cpu: transfer model to CPU before converting to ONNX, dirty workaround when model's tensors are on different devices
     :param train: export model in training mode
     :param model: torch.nn.Module, model to export
     :param onnx_filename: str, target path for the onnx file,
     :param input_shape: tuple, input shape (usually BCHW)
+    :param deepcopy_model: Whether to export deepcopy(model). Necessary in case further training is performed and
+     prep_model_for_conversion makes the network un-trainable (i.e RepVGG blocks).
     """
     if _imported_pytorch_quantization_failure is not None:
         raise _imported_pytorch_quantization_failure
 
+    if deepcopy_model:
+        model = deepcopy(model)
+
     use_fb_fake_quant_state = quant_nn.TensorQuantizer.use_fb_fake_quant
     quant_nn.TensorQuantizer.use_fb_fake_quant = True
 
     # Export ONNX for multiple batch sizes
     logger.info("Creating ONNX file: " + onnx_filename)
 
     if train:
```

## Comparing `super_gradients/recipes/coco2017_pose_pppose_l.yaml` & `super_gradients/recipes/cityscapes_al_ddrnet.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,66 +1,89 @@
-#  TODO Fill in the description of the recipe.
+# Instructions:
+#   0. Make sure that the data is stored in dataset_params.dataset_dir or add "dataset_params.data_dir=<PATH-TO-DATASET>" at the end of the command below (feel free to check ReadMe)
+#   1. Prepare the Cityscapes AutoLabelling dataset as described in `src/super_gradients/training/datasets/Dataset_Setup_Instructions.md`.
+#   2. Move to the project root (where you will find the ReadMe and src folder)
+#   3. Run the command:
+#      DDRNet39:        python -m super_gradients.train_from_recipe --config-name=cityscapes_ddrnet architecture=ddrnet_39
+# Note: add "checkpoint_params.checkpoint_path=<ddrnet39-backbone-pretrained-path>" to use pretrained backbone
+#
+#  Validation mIoU - Cityscapes, training time:
+#      DDRNet39:        input-size: [1024, 2048]     mIoU: 85.17    4 X RTX A5000, 38 H
+#
+#  Pretrained checkpoints:
+#      Backbones- downloaded from the author's official repo.
+#       https://deci-pretrained-models.s3.amazonaws.com/ddrnet/imagenet_pt_backbones/ddrnet39_bb_imagenet.pth
+#
+#      Network checkpoints:
+#       DDRNet39:       https://sghub.deci.ai/models/ddrnet_39_cityscapes.pth
+#
+#  Learning rate and batch size parameters, using 4 RTX A5000 with DDP:
+#      DDRNet39:        input-size: [1024, 1024]     initial_lr: 0.0075    batch-size: 6 * 4gpus = 24
+#
+#  Comments:
+#      * Pretrained backbones were used.
 
 defaults:
-  - training_hyperparams: coco2017_dekr_pose_train_params
-  - dataset_params: coco_pose_estimation_dekr_dataset_params
-  - arch_params: pose_pppose_l_arch_params
+  - training_hyperparams: cityscapes_default_train_params
+  - dataset_params: cityscapes_al_dataset_params
   - checkpoint_params: default_checkpoint_params
   - _self_
   - variable_setup
 
-resume: False
-
-architecture: pose_ppyolo_l
-
-multi_gpu: DDP
-num_gpus: 8
-
-experiment_suffix: ""
-experiment_name: coco2017_${architecture}${experiment_suffix}
-
+architecture: ddrnet_39
 
+dataset_params:
+  train_dataloader_params:
+    batch_size: 6
+  val_dataloader_params:
+    batch_size: 3
+  train_dataset_params:
+    transforms:
+      - SegColorJitter:
+          brightness: 0.5
+          contrast: 0.5
+          saturation: 0.5
+
+      - SegRandomFlip:
+          prob: 0.5
+
+      - SegRandomRescale:
+          scales: [ 0.5, 2. ]
+
+      - SegPadShortToCropSize:
+          crop_size: [ 1024, 1024 ]
+          fill_mask: 19
+
+      - SegCropImageAndMask:
+          crop_size: [ 1024, 1024 ]
+          mode: random
 
-train_dataloader: coco2017_pose_train
-val_dataloader: coco2017_pose_val
+training_hyperparams:
+  max_epochs: 200
+  initial_lr: 0.0075   # batch size 24
+  loss:
+    dice_ce_edge_loss:
+      num_classes: 19
+      ignore_index: 19
+      num_aux_heads: 1
+      num_detail_heads: 0
+      weights: [ 1., 0.4 ]
+      dice_ce_weights: [ 1., 1. ]
+      ce_edge_weights: [ .5, .5 ]
+      edge_kernel: 5
+  sync_bn: True
 
 arch_params:
-  num_classes: ${dataset_params.num_joints}
+  num_classes: 19
+  use_aux_heads: True
 
-  backbone:
-    CSPResNetBackbone:
-      pretrained_weights: https://deci-pretrained-models.s3.amazonaws.com/ppyolo_e/CSPResNetb_l_pretrained.pth
-
-dataset_params:
-  train_dataloader_params:
-    batch_size: 12
+load_checkpoint: False
+checkpoint_params:
+  load_checkpoint: ${load_checkpoint}
+  checkpoint_path: ???
+  load_backbone: True
+  strict_load: no_key_matching
 
-  val_dataloader_params:
-    batch_size: 16
+experiment_name: ${architecture}_cityscapes_al
 
-training_hyperparams:
-  initial_lr: 0.0001
-  resume: ${resume}
-  phase_callbacks: []
-#   Note: You can uncomment following block to enable visualization of intermediate results during training.
-#   When enabled, these callbacks will save first batch from training & validation to Tensorboard.
-#   This is helpful for debugging and doing visual checks whether predictions are reasonable and transforms are
-#   working as expected.
-#   The only downside is that it tend to bloat Tensorboard logs (Up to ten Gigs for long training regimes).
-#  phase_callbacks:
-#    - DEKRVisualizationCallback:
-#        phase:
-#          _target_: super_gradients.training.utils.callbacks.callbacks.Phase
-#          value: TRAIN_BATCH_END
-#        prefix: "train_"
-#        mean: [ 0.485, 0.456, 0.406 ]
-#        std: [ 0.229, 0.224, 0.225 ]
-#        apply_sigmoid: False
-#
-#    - DEKRVisualizationCallback:
-#        phase:
-#          _target_: super_gradients.training.utils.callbacks.callbacks.Phase
-#          value: VALIDATION_BATCH_END
-#        prefix: "val_"
-#        mean: [ 0.485, 0.456, 0.406 ]
-#        std: [ 0.229, 0.224, 0.225 ]
-#        apply_sigmoid: False
+multi_gpu: DDP
+num_gpus: 4
```

## Comparing `super_gradients-3.1.1.dist-info/LICENSE.YOLONAS.md` & `super_gradients-3.1.2.dist-info/LICENSE.YOLONAS.md`

 * *Files identical despite different names*

## Comparing `super_gradients-3.1.1.dist-info/LICENSE.md` & `super_gradients-3.1.2.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `super_gradients-3.1.1.dist-info/METADATA` & `super_gradients-3.1.2.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: super-gradients
-Version: 3.1.1
+Version: 3.1.2
 Summary: SuperGradients
 Home-page: https://docs.deci.ai/super-gradients/documentation/source/welcome.html
 Author: Deci AI
 Author-email: rnd@deci.ai
-License: UNKNOWN
 Keywords: Deci,AI,Training,Deep Learning,Computer Vision,PyTorch,SOTA,Recipes,Pre Trained,Models
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
-Requires-Dist: torch (<1.14,>=1.9.0)
+License-File: LICENSE.YOLONAS.md
+License-File: LICENSE.md
+Requires-Dist: torch (>=1.9.0)
 Requires-Dist: tqdm (>=4.57.0)
 Requires-Dist: boto3 (>=1.17.15)
 Requires-Dist: jsonschema (>=3.2.0)
 Requires-Dist: Deprecated (>=1.2.11)
 Requires-Dist: opencv-python (>=4.5.1)
 Requires-Dist: scipy (>=1.6.1)
 Requires-Dist: matplotlib (>=3.3.4)
@@ -21,42 +21,41 @@
 Requires-Dist: tensorboard (>=2.4.1)
 Requires-Dist: setuptools (>=21.0.0)
 Requires-Dist: coverage (~=5.3.1)
 Requires-Dist: torchvision (>=0.10.0)
 Requires-Dist: sphinx (~=4.0.2)
 Requires-Dist: sphinx-rtd-theme
 Requires-Dist: torchmetrics (==0.8)
-Requires-Dist: pillow (>=9.2.0)
 Requires-Dist: hydra-core (>=1.2.0)
 Requires-Dist: omegaconf
 Requires-Dist: onnxruntime (==1.13.1)
 Requires-Dist: onnx (==1.13.0)
+Requires-Dist: pillow (!=8.3,>=5.3.0)
 Requires-Dist: pip-tools (>=6.12.1)
 Requires-Dist: pyparsing (==2.4.5)
 Requires-Dist: einops (==0.3.2)
-Requires-Dist: pycocotools (==2.0.4)
+Requires-Dist: pycocotools (==2.0.6)
 Requires-Dist: protobuf (==3.20.3)
 Requires-Dist: treelib (==1.6.1)
 Requires-Dist: termcolor (==1.1.0)
 Requires-Dist: packaging (>=20.4)
 Requires-Dist: wheel (>=0.38.0)
 Requires-Dist: pygments (>=2.7.4)
 Requires-Dist: stringcase (>=1.2.0)
 Requires-Dist: numpy (<=1.23)
 Requires-Dist: rapidfuzz
 Requires-Dist: json-tricks (==3.16.1)
 Requires-Dist: onnx-simplifier (<1.0,>=0.3.6)
 Provides-Extra: pro
-Requires-Dist: deci-lab-client (==4.17.0) ; extra == 'pro'
-Requires-Dist: deci-common (==3.15.0) ; extra == 'pro'
+Requires-Dist: deci-platform-client (>=5.0.0) ; extra == 'pro'
 
 <div align="center" markdown="1">
   <img src="docs/assets/SG_img/SG - Horizontal Glow 2.png" width="600"/>
  <br/><br/>
-
+  
 **Build, train, and fine-tune production-ready deep learning  SOTA vision models**
 [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Easily%20train%20or%20fine-tune%20SOTA%20computer%20vision%20models%20from%20one%20training%20repository&url=https://github.com/Deci-AI/super-gradients&via=deci_ai&hashtags=AI,deeplearning,computervision,training,opensource)
 
 #### Version 3 is out! Notebooks have been updated!
 ______________________________________________________________________
 </div>  
 <div align="center">
@@ -128,15 +127,15 @@
 </div>
 
 
 ### Easy to train SOTA Models
 
 Easily load and fine-tune production-ready, pre-trained SOTA models that incorporate best practices and validated hyper-parameters for achieving best-in-class accuracy. 
 For more information on how to do it go to [Getting Started](#getting-started)
-
+    
 
 #### Plug and play recipes
 ```bash
 python -m super_gradients.train_from_recipe architecture=regnetY800 dataset_interface.data_dir=<YOUR_Imagenet_LOCAL_PATH> ckpt_root_dir=<CHEKPOINT_DIRECTORY>
 ```
 More example on how and why to use recipes can be found in [Recipes](#recipes)
 
@@ -150,33 +149,37 @@
 
 model = models.get(Models.YOLO_NAS_M, pretrained_weights="coco")
 
 # Prepare model for conversion
 # Input size is in format of [Batch x Channels x Width x Height] where 640 is the standard COCO dataset dimensions
 model.eval()
 model.prep_model_for_conversion(input_size=[1, 3, 640, 640])
-
+    
 # Create dummy_input
 
 # Convert model to onnx
 torch.onnx.export(model, dummy_input,  "yolo_nas_m.onnx")
 ```
 More information on how to take your model to production can be found in [Getting Started](#getting-started) notebooks
 
 ## Quick Installation
 
 __________________________________________________________________________________________________________
 
-
+ 
 ```bash
 pip install super-gradients
 ```
 
-## What's New - Version 3.1.1 (May 3rd)
+## What's New
 __________________________________________________________________________________________________________
+30th of May
+* [Quantization Aware Training YoloNAS on Custom Dataset](https://bit.ly/3MIKdTy)
+
+Version 3.1.1 (May 3rd)
 * [YOLO-NAS](https://bit.ly/41WeNPZ)
 * New [predict function](https://bit.ly/3oZfaea) (predict on any image, video, url, path, stream)
 * [RoboFlow100](https://bit.ly/40YOJ5z) datasets integration 
 * A new [Documentation Hub](https://docs.deci.ai/super-gradients/documentation/source/welcome.html)
 * Integration with [DagsHub for experiment monitoring](https://bit.ly/3ALFUkQ)
 * Support [Darknet/Yolo format detection dataset](https://bit.ly/41VX6Qu) (used by Yolo v5, v6, v7, v8) 
 * [Segformer](https://bit.ly/3oYu6Jp) model and recipe 
@@ -224,15 +227,15 @@
 python -m super_gradients.train_from_recipe --config-name=imagenet_regnetY architecture=regnetY800 dataset_interface.data_dir=<YOUR_Imagenet_LOCAL_PATH> ckpt_root_dir=<CHEKPOINT_DIRECTORY>
 ```
 ### Quickly Load Pre-Trained Weights for Your Desired Model with SOTA Performance
 Want to try our pre-trained models on your machine? Import SuperGradients, initialize your Trainer, and load your desired architecture and pre-trained weights from our [SOTA model zoo](http://bit.ly/41dkt89)
 
 ```python
 # The pretrained_weights argument will load a pre-trained architecture on the provided dataset
-
+    
 import super_gradients
 
 model = models.get("model-name", pretrained_weights="pretrained-model-name")
 
 ```   
 ###  Classification
 
@@ -251,128 +254,109 @@
 ###  Semantic Segmentation
 
 ####  Quick Start 
 <table class="tfo-notebook-buttons" align="left">
  <td width="500">
 <a target="_blank" href="https://bit.ly/3qKx9m8"><img src="./docs/assets/SG_img/colab_logo.png" /> Segmentation Quick Start</a>
  </td>
- <td width="200">
-<a target="_blank" href="https://bit.ly/3qJjxYq"><img src="./docs/assets/SG_img/GitHub_logo.png" /> GitHub source </a>
- </td>
 </table>
  </br></br>
 
 
-
+ 
  ####  Transfer Learning 
 <table class="tfo-notebook-buttons" align="left">
  <td width="500">
 <a target="_blank" href="https://bit.ly/3qKwMbe"><img src="./docs/assets/SG_img/colab_logo.png" /> Segmentation Transfer Learning</a>
  </td>
- <td width="200">
-<a target="_blank" href="https://bit.ly/3ShJlXn"><img src="./docs/assets/SG_img/GitHub_logo.png" /> GitHub source</a>
- </td>
 </table>
  </br></br>
 
 
 
 ####  How to Connect Custom Dataset 
   <table class="tfo-notebook-buttons" align="left">
  <td width="500"> 
 <a target="_blank" href="https://bit.ly/3QQBVJp"><img src="./docs/assets/SG_img/colab_logo.png" /> Segmentation How to Connect Custom Dataset</a>
    </td>
- <td width="200">
- <a target="_blank" href="https://bit.ly/3Us2WGi"><img src="./docs/assets/SG_img/GitHub_logo.png" /> GitHub source</a>
- </td>
 </table>
  </br></br>
 
 
 
 ###  Object Detection
 
 
 #### Transfer Learning
   <table class="tfo-notebook-buttons" align="left">
  <td width="500">   
 <a target="_blank" href="https://bit.ly/3SkMohx"><img src="./docs/assets/SG_img/colab_logo.png" /> Detection Transfer Learning</a>
    </td>
- <td width="200">   
-<a target="_blank" href="https://bit.ly/3DF8siG"><img src="./docs/assets/SG_img/GitHub_logo.png" /> GitHub source</a>
- </td>
 </table>
  </br></br>
 
 #### How to Connect Custom Dataset 
   <table class="tfo-notebook-buttons" align="left">
  <td width="500">  
   <a target="_blank" href="https://bit.ly/3dqDlg3"><img src="./docs/assets/SG_img/colab_logo.png" /> Detection How to Connect Custom Dataset</a>
   </td>
- <td width="200">      
-<a target="_blank" href="https://bit.ly/3xBlcmq"><img src="./docs/assets/SG_img/GitHub_logo.png" /> GitHub source</a>
- </td>
 </table>
  </br></br>
 
 
 
 ### How to Predict Using Pre-trained Model
 
 #### Segmentation, Detection and Classification Prediction 
   <table class="tfo-notebook-buttons" align="left">
  <td width="500">    
 <a target="_blank" href="https://bit.ly/3f4mssd"><img src="./docs/assets/SG_img/colab_logo.png" /> How to Predict Using Pre-trained Model</a>
   </td>
- <td width="200">   
-<a target="_blank" href="https://bit.ly/3Sf59Tr"><img src="./docs/assets/SG_img/GitHub_logo.png" /> GitHub source</a>
- </td>
 </table>
  </br></br>
 
 
 ## Advanced Features
 __________________________________________________________________________________________________________
 ### Post Training Quantization and Quantization Aware Training
 Quantization involves representing weights and biases in lower precision, resulting in reduced memory and computational requirements, making it useful for deploying models on devices with limited resources. The process can be done during training, called Quantization aware training, or after training, called post-training quantization. A full tutorial can be found [here](http://bit.ly/41hC8uI).
   <table class=“tfo-notebook-buttons” align=“left”>
  <td width=“500”>
    <a target="_blank" href="http://bit.ly/3KrN6an"><img src="./docs/assets/SG_img/colab_logo.png" /> Post Training Quantization and Quantization Aware Training</a>
   </td>
- <td width=“200”>
-<a target="_blank" href="http://bit.ly/3nUGzxb"><img src="./docs/assets/SG_img/GitHub_logo.png" /> GitHub source</a>
- </td>
+</table>
+
+### Quantization Aware Training YoloNAS on Custom Dataset
+This tutorial provides a comprehensive guide on how to fine-tune a YoloNAS model using a custom dataset. It also demonstrates how to utilize SG's QAT (Quantization-Aware Training) support. Additionally, it offers step-by-step instructions on deploying the model and performing benchmarking.
+  <table class=“tfo-notebook-buttons” align=“left”>
+ <td width=“500”>
+   <a target="_blank" href="https://bit.ly/3MIKdTy"><img src="./docs/assets/SG_img/colab_logo.png" /> Quantization Aware Training YoloNAS on Custom Dataset</a>
+  </td>
 </table>
 
 ### Knowledge Distillation Training
 Knowledge Distillation is a training technique that uses a large model, teacher model, to improve the performance of a smaller model, the student model.
 Learn more about SuperGradients knowledge distillation training with our pre-trained BEiT base teacher model and Resnet18 student model on CIFAR10 example notebook on Google Colab for an easy to use tutorial using free GPU hardware
   <table class="tfo-notebook-buttons" align="left">
  <td width="500">   
    <a target="_blank" href="https://bit.ly/3BLA5oR"><img src="./docs/assets/SG_img/colab_logo.png" /> Knowledge Distillation Training</a>
   </td>
- <td width="200">   
-<a target="_blank" href="https://bit.ly/3S9UlG4"><img src="./docs/assets/SG_img/GitHub_logo.png" /> GitHub source</a>
- </td>
 </table>
  </br></br>
 
 ### Recipes
 To train a model, it is necessary to configure 4 main components. These components are aggregated into a single "main" recipe `.yaml` file that inherits the aforementioned dataset, architecture, raining and checkpoint params. It is also possible (and recomended for flexibility) to override default settings with custom ones.
 All recipes can be found [here](http://bit.ly/3gfLw07)
 </br>
 Recipes support out of the box every model, metric or loss that is implemented in SuperGradients, but you can easily extend this to any custom object that you need by "registering it". Check out [this](http://bit.ly/3TQ4iZB) tutorial for more information.
 
   <table class="tfo-notebook-buttons" align="left">
  <td width="500">   
    <a target="_blank" href="https://bit.ly/3UiY5ab"><img src="./docs/assets/SG_img/colab_logo.png" /> How to Use Recipes</a>
   </td>
- <td width="200">  
-<a target="_blank" href="https://bit.ly/3QSrHbm"><img src="./docs/assets/SG_img/GitHub_logo.png" /> GitHub source</a>
- </td>
 </table>
  </br></br>
 
  </br>
 <details markdown="1">
   <summary><h3>Using Distributed Data Parallel (DDP) </h3></summary>
 
@@ -444,15 +428,15 @@
 from super_gradients.common.environment.env_helpers import multi_process_safe
 
 class Upload3TrainImagesCalbback(PhaseCallback):
     def __init__(
         self,
     ):
         super().__init__(phase=Phase.TRAIN_BATCH_END)
-
+    
     @multi_process_safe
     def __call__(self, context: PhaseContext):
         batch_imgs = context.inputs.cpu().detach().numpy()
         tag = "batch_" + str(context.batch_idx) + "_images"
         context.sg_logger.add_images(tag=tag, images=batch_imgs[: 3], global_step=context.epoch)
 
 ```
@@ -502,15 +486,15 @@
 ```
 
 </details>
 
 <details markdown="1">
 
 <summary><h3> Using phase callbacks </h3></summary>  
-
+  
 ```python
 from super_gradients import Trainer
 from torch.optim.lr_scheduler import ReduceLROnPlateau
 from super_gradients.training.utils.callbacks import Phase, LRSchedulerCallback
 from super_gradients.training.metrics.classification_metrics import Accuracy
 
 # define PyTorch train and validation loaders and optimizer
@@ -558,15 +542,15 @@
 ```
 
 </details>
 
 <details>
 
 <summary><h3> Integration to Weights and Biases </h3></summary>    
-
+  
 
 ```python
 from super_gradients import Trainer
 
 # create a trainer object, look the declaration for more parameters
 trainer = Trainer("experiment_name")
 
@@ -583,15 +567,15 @@
 ```
 
 </details>
 
 <details markdown="1">
 
 <summary><h3> Integration to ClearML </h3></summary>    
-
+    
 ```python
 from super_gradients import Trainer
 
 # create a trainer object, look the declaration for more parameters
 trainer = Trainer("experiment_name")
 
 train_params = { ... # training parameters
@@ -609,51 +593,51 @@
   </details>
 
 
 ## Installation Methods
 __________________________________________________________________________________________________________
 ### Prerequisites
 <details markdown="1">
-
+  
 <summary>General requirements</summary>
-
+  
 - Python 3.7, 3.8 or 3.9 installed.
 - 1.9.0 <= torch < 1.14 
   - https://pytorch.org/get-started/locally/
 - The python packages that are specified in requirements.txt;
 
 </details>
-
+    
 <details markdown="1">
-
+  
 <summary>To train on nvidia GPUs</summary>
-
+  
 - [Nvidia CUDA Toolkit >= 11.2](https://developer.nvidia.com/cuda-11.2.0-download-archive?target_os=Linux&target_arch=x86_64&target_distro=Ubuntu)
 - CuDNN >= 8.1.x
 - Nvidia Driver with CUDA >= 11.2 support (≥460.x)
-
+  
 </details>
-
+    
 ### Quick Installation
 
 <details markdown="1">
-
+  
 <summary>Install stable version using PyPi</summary>
 
 See in [PyPi](https://pypi.org/project/super-gradients/)
 ```bash
 pip install super-gradients
 ```
 
 That's it !
 
 </details>
-
+    
 <details markdown="1">
-
+  
 <summary>Install using GitHub</summary>
 
 
 ```bash
 pip install git+https://github.com/Deci-AI/super-gradients.git@stable
 ```
 
@@ -664,15 +648,15 @@
 __________________________________________________________________________________________________________
 
 All Computer Vision Models - Pretrained Checkpoints can be found in the [Model Zoo](http://bit.ly/41dkt89)
 
 Detailed list can be found [here](http://bit.ly/3GnJwgZ) 
 
 ### Image Classification
-
+  
 - [DensNet (Densely Connected Convolutional Networks)](https://github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/models/classification_models/densenet.py) 
 - [DPN](https://github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/models/classification_models/dpn.py) 
 - [EfficientNet](https://github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/models/classification_models/efficientnet.py)
 - [LeNet](https://github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/models/classification_models/lenet.py) 
 - [MobileNet](https://github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/models/classification_models/mobilenet.py)
 - [MobileNet v2](https://github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/models/classification_models/mobilenetv2.py)  
 - [MobileNet v3](https://github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/models/classification_models/mobilenetv3.py) 
@@ -682,76 +666,76 @@
 - [RepVGG](https://github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/models/classification_models/repvgg.py)  
 - [ResNet](https://github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/models/classification_models/resnet.py)
 - [ResNeXt](https://github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/models/classification_models/resnext.py) 
 - [SENet ](https://github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/models/classification_models/senet.py)
 - [ShuffleNet](https://github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/models/classification_models/shufflenet.py)
 - [ShuffleNet v2](https://github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/models/classification_models/shufflenetv2.py)
 - [VGG](https://github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/models/classification_models/vgg.py)
-
+  
 ### Semantic Segmentation 
 
 - [PP-LiteSeg](https://bit.ly/3RrtMMO)
 - [DDRNet (Deep Dual-resolution Networks)](https://github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/models/segmentation_models/ddrnet.py) 
 - [LadderNet](https://github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/models/segmentation_models/laddernet.py)
 - [RegSeg](https://github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/models/segmentation_models/regseg.py)
 - [ShelfNet](https://github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/models/segmentation_models/shelfnet.py) 
 - [STDC](https://github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/models/segmentation_models/stdc.py)
-
+  
 
 ### Object Detection
-
+  
 - [CSP DarkNet](https://github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/models/detection_models/csp_darknet53.py)
 - [DarkNet-53](https://github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/models/detection_models/darknet53.py)
 - [SSD (Single Shot Detector)](https://github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/models/detection_models/ssd.py) 
 - [YOLOX](https://github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/models/detection_models/yolox.py)
-
-
+  
+  
 
 __________________________________________________________________________________________________________
 
 ## Implemented Datasets 
 __________________________________________________________________________________________________________
 
 Deci provides implementation for various datasets. If you need to download any of the dataset, you can 
 [find instructions](https://github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/datasets/Dataset_Setup_Instructions.md). 
 
 ### Image Classification
-
+  
 - [Cifar10](https://github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/datasets/classification_datasets/cifar.py) 
 - [ImageNet](https://github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/datasets/classification_datasets/imagenet_dataset.py) 
-
+  
 ### Semantic Segmentation 
 
 - [Cityscapes](https://github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/datasets/segmentation_datasets/cityscape_segmentation.py)
 - [Coco](https://github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/datasets/segmentation_datasets/coco_segmentation.py) 
 - [PascalVOC 2012 / PascalAUG 2012](https://github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/datasets/segmentation_datasets/pascal_voc_segmentation.py)
 - [SuperviselyPersons](https://github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/datasets/segmentation_datasets/supervisely_persons_segmentation.py)
 - [Mapillary Vistas Dataset](https://github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/datasets/segmentation_datasets/mapillary_dataset.py)
 
 
 ### Object Detection
-
+  
 - [Coco](https://github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/datasets/detection_datasets/coco_detection.py)
 - [PascalVOC 2007 & 2012](https://github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/datasets/detection_datasets/pascal_voc_detection.py)
-
-
+  
+  
 
 __________________________________________________________________________________________________________
 
 
 ## Documentation
 
 Check SuperGradients [Docs](https://docs.deci.ai/super-gradients/documentation/source/welcome.html) for full documentation, user guide, and examples.
-
+  
 ## Contributing
 
 To learn about making a contribution to SuperGradients, please see our [Contribution page](CONTRIBUTING.md).
 
 Our awesome contributors:
-
+    
 <a href="https://github.com/Deci-AI/super-gradients/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=Deci-AI/super-gradients" />
 </a>
 
 
 <br/>Made with [contrib.rocks](https://contrib.rocks).
 
@@ -762,26 +746,26 @@
 ## Community
 
 If you want to be a part of SuperGradients growing community, hear about all the exciting news and updates, need help, request for advanced features,
     or want to file a bug or issue report, we would love to welcome you aboard!
 
 * Discord is the place to be and ask questions about SuperGradients and get support. [Click here to join our Discord Community](
   https://discord.gg/2v6cEGMREN)
-
+    
 * To report a bug, [file an issue](https://github.com/Deci-AI/super-gradients/issues) on GitHub.
 
 * Join the [SG Newsletter](https://www.supergradients.com/#Newsletter)
   for staying up to date with new features and models, important announcements, and upcoming events.
 
 * For a short meeting with us, use this [link](https://calendly.com/ofer-baratz-deci/15min) and choose your preferred time.
 
 ## License
 
 This project is released under the [Apache 2.0 license](LICENSE).
-
+    
 ## Citing
 
 ### BibTeX
 
 ```bibtex
 
 @misc{supergradients,
@@ -795,15 +779,15 @@
 }
 ```
 
 ### Latest DOI
 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7789328.svg)](https://doi.org/10.5281/zenodo.7789328)
 
-
+    
 __________________________________________________________________________________________________________
 
 
 ## Deci Platform
 
 Deci Platform is our end to end platform for building, optimizing and deploying deep learning models to production.
 
@@ -815,9 +799,7 @@
 - Gain up to 10X improvement in throughput, latency, memory and model size. 
 - Easily benchmark your models’ performance on different hardware and batch sizes.
 - Invite co-workers to collaborate on models and communicate your progress.
 - Deci supports all common frameworks and Hardware, from Intel CPUs to Nvidia's GPUs and Jetsons.
 ֿ
 
 Request free trial [here](https://bit.ly/3qO3icq) 
-
-
```

### html2text {}

```diff
@@ -1,31 +1,30 @@
-Metadata-Version: 2.1 Name: super-gradients Version: 3.1.1 Summary:
+Metadata-Version: 2.1 Name: super-gradients Version: 3.1.2 Summary:
 SuperGradients Home-page: https://docs.deci.ai/super-gradients/documentation/
-source/welcome.html Author: Deci AI Author-email: rnd@deci.ai License: UNKNOWN
-Keywords: Deci,AI,Training,Deep Learning,Computer
-Vision,PyTorch,SOTA,Recipes,Pre Trained,Models Platform: UNKNOWN Description-
-Content-Type: text/markdown Requires-Dist: torch (<1.14,>=1.9.0) Requires-Dist:
-tqdm (>=4.57.0) Requires-Dist: boto3 (>=1.17.15) Requires-Dist: jsonschema
-(>=3.2.0) Requires-Dist: Deprecated (>=1.2.11) Requires-Dist: opencv-python
-(>=4.5.1) Requires-Dist: scipy (>=1.6.1) Requires-Dist: matplotlib (>=3.3.4)
-Requires-Dist: psutil (>=5.8.0) Requires-Dist: tensorboard (>=2.4.1) Requires-
-Dist: setuptools (>=21.0.0) Requires-Dist: coverage (~=5.3.1) Requires-Dist:
-torchvision (>=0.10.0) Requires-Dist: sphinx (~=4.0.2) Requires-Dist: sphinx-
-rtd-theme Requires-Dist: torchmetrics (==0.8) Requires-Dist: pillow (>=9.2.0)
-Requires-Dist: hydra-core (>=1.2.0) Requires-Dist: omegaconf Requires-Dist:
-onnxruntime (==1.13.1) Requires-Dist: onnx (==1.13.0) Requires-Dist: pip-tools
-(>=6.12.1) Requires-Dist: pyparsing (==2.4.5) Requires-Dist: einops (==0.3.2)
-Requires-Dist: pycocotools (==2.0.4) Requires-Dist: protobuf (==3.20.3)
-Requires-Dist: treelib (==1.6.1) Requires-Dist: termcolor (==1.1.0) Requires-
-Dist: packaging (>=20.4) Requires-Dist: wheel (>=0.38.0) Requires-Dist:
-pygments (>=2.7.4) Requires-Dist: stringcase (>=1.2.0) Requires-Dist: numpy
-(<=1.23) Requires-Dist: rapidfuzz Requires-Dist: json-tricks (==3.16.1)
-Requires-Dist: onnx-simplifier (<1.0,>=0.3.6) Provides-Extra: pro Requires-
-Dist: deci-lab-client (==4.17.0) ; extra == 'pro' Requires-Dist: deci-common
-(==3.15.0) ; extra == 'pro'
+source/welcome.html Author: Deci AI Author-email: rnd@deci.ai Keywords:
+Deci,AI,Training,Deep Learning,Computer Vision,PyTorch,SOTA,Recipes,Pre
+Trained,Models Description-Content-Type: text/markdown License-File:
+LICENSE.YOLONAS.md License-File: LICENSE.md Requires-Dist: torch (>=1.9.0)
+Requires-Dist: tqdm (>=4.57.0) Requires-Dist: boto3 (>=1.17.15) Requires-Dist:
+jsonschema (>=3.2.0) Requires-Dist: Deprecated (>=1.2.11) Requires-Dist:
+opencv-python (>=4.5.1) Requires-Dist: scipy (>=1.6.1) Requires-Dist:
+matplotlib (>=3.3.4) Requires-Dist: psutil (>=5.8.0) Requires-Dist: tensorboard
+(>=2.4.1) Requires-Dist: setuptools (>=21.0.0) Requires-Dist: coverage
+(~=5.3.1) Requires-Dist: torchvision (>=0.10.0) Requires-Dist: sphinx (~=4.0.2)
+Requires-Dist: sphinx-rtd-theme Requires-Dist: torchmetrics (==0.8) Requires-
+Dist: hydra-core (>=1.2.0) Requires-Dist: omegaconf Requires-Dist: onnxruntime
+(==1.13.1) Requires-Dist: onnx (==1.13.0) Requires-Dist: pillow (!=8.3,>=5.3.0)
+Requires-Dist: pip-tools (>=6.12.1) Requires-Dist: pyparsing (==2.4.5)
+Requires-Dist: einops (==0.3.2) Requires-Dist: pycocotools (==2.0.6) Requires-
+Dist: protobuf (==3.20.3) Requires-Dist: treelib (==1.6.1) Requires-Dist:
+termcolor (==1.1.0) Requires-Dist: packaging (>=20.4) Requires-Dist: wheel
+(>=0.38.0) Requires-Dist: pygments (>=2.7.4) Requires-Dist: stringcase
+(>=1.2.0) Requires-Dist: numpy (<=1.23) Requires-Dist: rapidfuzz Requires-Dist:
+json-tricks (==3.16.1) Requires-Dist: onnx-simplifier (<1.0,>=0.3.6) Provides-
+Extra: pro Requires-Dist: deci-platform-client (>=5.0.0) ; extra == 'pro'
                [docs/assets/SG_img/SG - Horizontal Glow 2.png]
 
    **Build, train, and fine-tune production-ready deep learning SOTA vision
           models** [![Tweet](https://img.shields.io/twitter/url/http/
            shields.io.svg?style=social)](https://twitter.com/intent/
                     tweet?text=Easily%20train%20or%20fine-
 tune%20SOTA%20computer%20vision%20models%20from%20one%20training%20repository&url=https:
@@ -83,26 +82,27 @@
 Input size is in format of [Batch x Channels x Width x Height] where 640 is the
 standard COCO dataset dimensions model.eval() model.prep_model_for_conversion
 (input_size=[1, 3, 640, 640]) # Create dummy_input # Convert model to onnx
 torch.onnx.export(model, dummy_input, "yolo_nas_m.onnx") ``` More information
 on how to take your model to production can be found in [Getting Started]
 (#getting-started) notebooks ## Quick Installation
 __________________________________________________________________________________________________________
-```bash pip install super-gradients ``` ## What's New - Version 3.1.1 (May 3rd)
+```bash pip install super-gradients ``` ## What's New
 __________________________________________________________________________________________________________
-* [YOLO-NAS](https://bit.ly/41WeNPZ) * New [predict function](https://bit.ly/
-3oZfaea) (predict on any image, video, url, path, stream) * [RoboFlow100]
-(https://bit.ly/40YOJ5z) datasets integration * A new [Documentation Hub]
-(https://docs.deci.ai/super-gradients/documentation/source/welcome.html) *
-Integration with [DagsHub for experiment monitoring](https://bit.ly/3ALFUkQ) *
-Support [Darknet/Yolo format detection dataset](https://bit.ly/41VX6Qu) (used
-by Yolo v5, v6, v7, v8) * [Segformer](https://bit.ly/3oYu6Jp) model and recipe
-* Post Training Quantization and Quantization Aware Training - [notebooks]
-(http://bit.ly/3KrN6an) Check out SG full [release notes](https://github.com/
-Deci-AI/super-gradients/releases). ## Coming soon
+30th of May * [Quantization Aware Training YoloNAS on Custom Dataset](https://
+bit.ly/3MIKdTy) Version 3.1.1 (May 3rd) * [YOLO-NAS](https://bit.ly/41WeNPZ) *
+New [predict function](https://bit.ly/3oZfaea) (predict on any image, video,
+url, path, stream) * [RoboFlow100](https://bit.ly/40YOJ5z) datasets integration
+* A new [Documentation Hub](https://docs.deci.ai/super-gradients/documentation/
+source/welcome.html) * Integration with [DagsHub for experiment monitoring]
+(https://bit.ly/3ALFUkQ) * Support [Darknet/Yolo format detection dataset]
+(https://bit.ly/41VX6Qu) (used by Yolo v5, v6, v7, v8) * [Segformer](https://
+bit.ly/3oYu6Jp) model and recipe * Post Training Quantization and Quantization
+Aware Training - [notebooks](http://bit.ly/3KrN6an) Check out SG full [release
+notes](https://github.com/Deci-AI/super-gradients/releases). ## Coming soon
 __________________________________________________________________________________________________________
 - [ ] Pre-trained pose estimation model - [ ] Test Time Augmentations (TTA) -
 [ ] Recipe to train DEKR model(convertable to TRT) - [ ] Key-points Rescoring
 for Pose estimation - [ ] LR finder - [ ] Data analysis tools ## Table of
 Content
 __________________________________________________________________________________________________________
 - [Getting Started](#getting-started) - [Advanced Features](#advanced-features)
@@ -141,14 +141,19 @@
 ### Post Training Quantization and Quantization Aware Training Quantization
 involves representing weights and biases in lower precision, resulting in
 reduced memory and computational requirements, making it useful for deploying
 models on devices with limited resources. The process can be done during
 training, called Quantization aware training, or after training, called post-
 training quantization. A full tutorial can be found [here](http://bit.ly/
 41hC8uI).
+### Quantization Aware Training YoloNAS on Custom Dataset This tutorial
+provides a comprehensive guide on how to fine-tune a YoloNAS model using a
+custom dataset. It also demonstrates how to utilize SG's QAT (Quantization-
+Aware Training) support. Additionally, it offers step-by-step instructions on
+deploying the model and performing benchmarking.
 ### Knowledge Distillation Training Knowledge Distillation is a training
 technique that uses a large model, teacher model, to improve the performance of
 a smaller model, the student model. Learn more about SuperGradients knowledge
 distillation training with our pre-trained BEiT base teacher model and Resnet18
 student model on CIFAR10 example notebook on Google Colab for an easy to use
 tutorial using free GPU hardware
  ### Recipes To train a model, it is necessary to configure 4 main components.
```

## Comparing `super_gradients-3.1.1.dist-info/RECORD` & `super_gradients-3.1.2.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-super_gradients/__init__.py,sha256=T2_OhgYgFhdmsAJSTvLMXKYOFL8asv3oPZANEq9w-7A,711
+super_gradients/__init__.py,sha256=0AjXNZu1bTNLAS1rBwo-NMblkVGnsF5M5fWofoSoqh8,916
 super_gradients/evaluate_checkpoint.py,sha256=cAB8pjlpxrpyJ2RhDp9jtV90TRvih7Axl0D2HVbfFKA,1657
 super_gradients/evaluate_from_recipe.py,sha256=aEUFWz0ue8tI55ChEivtABxUe7lhLCqT9aOywoenYfM,1807
-super_gradients/qat_from_recipe.py,sha256=Jb355vmclhurcOYN8Qgr6DFRMnnoxRB6N1uI5RLT9cM,702
-super_gradients/requirements.pro.txt,sha256=N4SNm12LMYBhOwA5ShEQlihV_6nJoveWkbEo1037idI,44
-super_gradients/requirements.txt,sha256=-hJEsVtZGOENWHmv4jiAUp-doNLwlJ_Ld4uhVULJf-U,729
+super_gradients/qat_from_recipe.py,sha256=AL7V8rS14iBwY3hH-BPXCwpa-Y1U1M3tCOy8o1yZnbY,639
+super_gradients/requirements.pro.txt,sha256=aYAzKlErZArFhx1DFYdxhMz3onw7QFKCy87VSfuEAT0,28
+super_gradients/requirements.txt,sha256=mvNAxH_Y4kSVvluGB_HaI7RFl_BvuH0mBbspC-DnQwI,729
 super_gradients/resume_experiment.py,sha256=VSmGBGaFOdz6hOTRkHm7un0MHolUk4_CvXfu2jtjGZM,537
 super_gradients/train_from_kd_recipe.py,sha256=OpRZsmleqXWQyFeaLzcnIooa_YEYEHFhkHr63Cs_QU8,693
 super_gradients/train_from_recipe.py,sha256=ZdCUpUlLPiCejcKff2FTfg33_TjZF0CwvZ-eaQlVyrA,650
 super_gradients/common/__init__.py,sha256=1F7pRDWoGs7wMWpbBw3iaTPWpeegxOroNPqUO3nzEMw,1098
-super_gradients/common/object_names.py,sha256=XdIY0xm9zurs5xjZ_RPh0f6RCJxmtpKreDaEHt-dVJk,15339
+super_gradients/common/object_names.py,sha256=l6PvK87ZrPzyeAv9-kZY0dE0VIO8NOETcllT7or9-XY,15566
 super_gradients/common/abstractions/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/common/abstractions/abstract_logger.py,sha256=MpEjg7PihMZb_qLBKC-R58wWFqNJdPJMlOkxEU25hCU,879
 super_gradients/common/abstractions/mute_processes.py,sha256=JxC3ofVySoiL7U7x9QYhzWLVYArkgqKQB2Kp3HyPOyE,3129
 super_gradients/common/auto_logging/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/common/auto_logging/auto_logger.py,sha256=WtlKaj5p8Ayx3gJ9XcRkuIG7oVicTs3K_X_gVeEfZOI,4846
 super_gradients/common/auto_logging/console_logging.py,sha256=PEPSfHQ8incS13dkM9gzlWBeRdwbodo9qVqRSk32s_E,6625
 super_gradients/common/aws_connection/__init__.py,sha256=cZCFSeQHk8E6TTZHTjnAhezGATF5iSKiFR2dBof8vqg,142
 super_gradients/common/aws_connection/aws_connector.py,sha256=2wHpTZubxc54tAqE5FaNIbC0LwtLFMkDS_rmx9x3XXg,4182
 super_gradients/common/aws_connection/aws_secrets_manager_connector.py,sha256=RUyDEx96sC4pGI3lH_z_Eo0dwP5QxZ0Qpy-ZFxQ6mz4,7198
 super_gradients/common/crash_handler/__init__.py,sha256=BWse71cn7bDfvpw52Rhpr0WtQyoxN9KmzEWX3w__ElE,119
 super_gradients/common/crash_handler/crash_handler.py,sha256=cZokQPUpTtlXJ6Y8QzviF4fpXulmHvEnVCl6pRKipVY,669
 super_gradients/common/crash_handler/crash_tips.py,sha256=sbBzMKnPMMvQv8ba7MV1w1tyOyaSS-p4bE7DV1yUHdw,11775
 super_gradients/common/crash_handler/crash_tips_setup.py,sha256=uDE_aY7xQshk4ucKOs7wBi0iT_xTwWF-yQB-qR0kcM4,886
 super_gradients/common/crash_handler/exception.py,sha256=PaLwJLDq4KdueZ_Wf5KSE-FG-hp1KPVuQiwZajG_T7w,1740
-super_gradients/common/crash_handler/exception_monitoring_setup.py,sha256=0AhCwUakzPqqHaCnWMqnNKvE0Kh7kCDKWj-r1RVdn0A,2357
+super_gradients/common/crash_handler/exception_monitoring_setup.py,sha256=ToUhaU3onvANU2CSMWZpdRAhIgS-XevLdTBXdUhEwU4,2397
 super_gradients/common/crash_handler/utils.py,sha256=OAjrEOiXHm_8132LvAEO1oth_XqJu99a6GjADFnBoA4,789
 super_gradients/common/data_connection/__init__.py,sha256=oqRApzhTEhJdobpEsWIrXdPtjRtZ9GJrMVUIozTYw5Y,140
 super_gradients/common/data_connection/s3_connector.py,sha256=gm4pkKXahin_gr-Zx3RnU9x4Y1bI-6BRtCCPuYGYQ5w,17959
 super_gradients/common/data_interface/__init__.py,sha256=BZSmA95LR2q7nznQwOf9TQkMgeaLzU92wsru-ITSTEQ,325
 super_gradients/common/data_interface/adnn_model_repository_data_interface.py,sha256=FeS1SI-RloadiCysdeBumm6kf9tqsysRjeyQI3LrbtE,9699
 super_gradients/common/data_interface/dataset_data_interface.py,sha256=nyXQSfY-43XtW6wWG5_aM68vePkZzZ1KvB9NK41XTaw,2050
 super_gradients/common/data_types/__init__.py,sha256=YfKs8C4Jtz2ZL-Y7ZKaTMKO0VSr1zWTK90CfVtgdXP4,220
@@ -43,18 +43,18 @@
 super_gradients/common/decorators/deci_logger.py,sha256=vyvodC1QCdLp_S05ELnBDnK1vCHBjtbvCsLRVnIdYHc,3663
 super_gradients/common/decorators/explicit_params_validator.py,sha256=EtW4ebI18tgPCBsA6v0Go3RY87iiqEEiQUQrujOb-y0,2921
 super_gradients/common/decorators/factory_decorator.py,sha256=PPHORVS_3fHGMqy7jbfTRwrHhDtXtHwWjR6hQe4J41s,1315
 super_gradients/common/decorators/singleton.py,sha256=6lVKPFSidDVRMOLeQ2YK-c7FRcxQEhrWU_AbuC7JXSc,1132
 super_gradients/common/environment/__init__.py,sha256=ljbYwQPDh8G0dCHjA6EGPSX5guFcsj-tUB6Ks0mHR-A,202
 super_gradients/common/environment/argparse_utils.py,sha256=c-XT11eDEZ42bWu2eKr4e6i30SF-OlM0a8xxgD08ob4,993
 super_gradients/common/environment/cfg_utils.py,sha256=_jUmcZ6HG7NK2R0H7edjNM62rDNzCTeRXBdAH2FFbq4,9170
-super_gradients/common/environment/checkpoints_dir_utils.py,sha256=UMQbSQ8tuZzYfTmwrqNef3KHElbZ3DC69B2L_hbGqNw,4218
+super_gradients/common/environment/checkpoints_dir_utils.py,sha256=0tYx8KMDRFINdpzEM7YZgXjJSzz8GzevGay3xD513sY,4383
 super_gradients/common/environment/ddp_utils.py,sha256=JMEzTKSrQ5pG9MGLd0xaIGIlg4Rlexh4soXhi0r6nzY,2682
 super_gradients/common/environment/device_utils.py,sha256=wV1pK5rjB4IShktrVdo9vx5mg_tF4XHIrRFssl2ftZA,752
-super_gradients/common/environment/env_variables.py,sha256=OxUpZ6aDt16d3rHPfw9u6wn-cmvdV4Zp67FIVc6n01c,1147
+super_gradients/common/environment/env_variables.py,sha256=BHuwlhzAOxMxLvgWj616eOwEhnFvbliEdyrrDiYUA2Y,927
 super_gradients/common/environment/omegaconf_utils.py,sha256=ycjvwGWxhhnBUwWXljqcSw-IJ8UH1BW1E3AznUSNN60,4047
 super_gradients/common/environment/path_utils.py,sha256=p6fBTLBdxdpsALaD0lanM2jEtZcbSdthuEXSoOmgT5Q,459
 super_gradients/common/environment/monitoring/__init__.py,sha256=QmJWRpVWwHOK0qjNPV6PlA5ZzKjgumxNbSoYDnhUzzo,112
 super_gradients/common/environment/monitoring/cpu.py,sha256=eGHnEDbci_jku-RTzgROxt_kPy9bUdydk_bUMin3Kxc,153
 super_gradients/common/environment/monitoring/data_models.py,sha256=t3Hky9Iu-qLKATdzyqb76j_6QxEVxamC7gnjh7Te5xk,2517
 super_gradients/common/environment/monitoring/disk.py,sha256=2XI7426eWGk_z3O_Fy_LWoVwUkLdK7ee7D8rqE6lmWE,1025
 super_gradients/common/environment/monitoring/monitoring.py,sha256=7c2anfycW-cHauTphi-ZaRH6CYVuEPLsGCbLz7BjHSQ,5427
@@ -83,39 +83,41 @@
 super_gradients/common/factories/pre_launch_callbacks_factory.py,sha256=qjd2jvcn95jRNcmJRBa0IWnGSkxNPJf-Xn66j-4H6MY,271
 super_gradients/common/factories/processing_factory.py,sha256=t-IEuzn6SxR7gDLQQ_WMp8-zPiq7UCjlDuONTnplWpk,623
 super_gradients/common/factories/samplers_factory.py,sha256=pdsa9My_0aF63vBgHLQtzobw8-ykz-dFbDemMizJrdI,229
 super_gradients/common/factories/target_generator_factory.py,sha256=LZXQUxMI-jz_QPj0Bfi9FccLgX3Ky2MjU1llqxHFvOE,263
 super_gradients/common/factories/transforms_factory.py,sha256=TrwGexN9y33eAw0wQRFDgM5a26FKhCOzQvyC-fp2kfM,1873
 super_gradients/common/factories/type_factory.py,sha256=HwIiWskEfoHZiEkN8batqIxATs_20TJqq8qR9W0_Has,2377
 super_gradients/common/plugins/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-super_gradients/common/plugins/deci_client.py,sha256=CP0H4tvynauOmLOWmPLjTvu3ho-Cugu8gLhofFY08HA,10974
+super_gradients/common/plugins/deci_client.py,sha256=88QA4_kEGwLwQkvPJa3N2R7WbVqRcoHHN6mywf_V7HI,12245
+super_gradients/common/plugins/wandb/__init__.py,sha256=J6rwLbKUtKgQIwYVJayBaXx0Tb77I7ZDE_5pEkQvFi4,143
+super_gradients/common/plugins/wandb/log_predictions.py,sha256=YiUKIYGsWfJxFaBLiZYITS0lYYEM_X3LXeawWD1EZvE,2329
 super_gradients/common/registry/__init__.py,sha256=gYkyLBFQN2kIgt0YFzGJl7lXKyOHBHE67B-1_C_JS8I,271
 super_gradients/common/registry/albumentation.py,sha256=MU7ZkXX-qSM5A_2l2apl6njJECwuUn4U1bo22yovOIY,1231
 super_gradients/common/registry/registry.py,sha256=XNgmvUY3kV3oF7i-yz4aZqyoM42EG4cV_mwS1EIyNFw,6006
 super_gradients/common/registry/registry_utils.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/common/sg_loggers/__init__.py,sha256=MJ9Gte7Zs_gGGge3zH7Tqv8iMm6Pic03YBHtrNqZUfc,508
-super_gradients/common/sg_loggers/abstract_sg_logger.py,sha256=OoGxOvQXwDfycg4A9wt_jgxI1zTS5XIS8GPFBQmY5rM,7355
-super_gradients/common/sg_loggers/base_sg_logger.py,sha256=W5IBmftH8M9b85t-F-mWsnRIo34_6CQ_vQd9owslUN8,14980
+super_gradients/common/sg_loggers/abstract_sg_logger.py,sha256=t76j41J_a4Lt1ab7UyNkt_gsEJOuxaudnShKgDoPyyI,7460
+super_gradients/common/sg_loggers/base_sg_logger.py,sha256=ae331wSsQzJ4VTA97YqKa_C6lP5qzgTZL3dkMJ3UhcM,15095
 super_gradients/common/sg_loggers/clearml_sg_logger.py,sha256=BWAJzubNT974xgcsOVckRsU8KLsYW2NLJ5x65tCeQ6w,10055
 super_gradients/common/sg_loggers/dagshub_sg_logger.py,sha256=H0DJKzKQoL3ooXWvvx3fnidRTkuhTcL7tzQ5-mW9TaI,10103
 super_gradients/common/sg_loggers/deci_platform_sg_logger.py,sha256=XLanzH_CwW4Nw6Mx-m4tS6rFkDH3xZ9P8rCIyYIxoGs,6618
-super_gradients/common/sg_loggers/wandb_sg_logger.py,sha256=DnGC3OmBcMSpK_wQ00KW0e7SLsgZ9vhDbhNhJYHRAtE,13073
+super_gradients/common/sg_loggers/wandb_sg_logger.py,sha256=GHdZMjsM2FeZ72XQoE6DSb_9CPXNnMTUvE4s2wtMIOc,15000
 super_gradients/examples/SG_Walkthrough.ipynb,sha256=bhJ62ERSAchiroY49KiQiycgyDjlgPgHeXLwcZdUuNY,85509
 super_gradients/examples/SG_quickstart_classification.ipynb,sha256=aMGQCqFss-flEKvUaVj5WiKStr0S8TRKUsHwoyFcuko,69618
 super_gradients/examples/SG_quickstart_model_upload_deci_lab.ipynb,sha256=M9YZY9VpKJNFHxBz-IGSRvdAACQJ1n-wTQgWSpZVW78,54966
 super_gradients/examples/SG_quickstart_tensorboard_logger.ipynb,sha256=Gyx6LjKAwHwUdJsGiSiBn-AdbcgTdpD2DvRWB7IaGYk,65090
 super_gradients/examples/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/examples/cifar10_training_torch_objects/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/examples/cifar10_training_torch_objects/cifar10_training_torch_objects_example.py,sha256=1tKhBpRwHWi4foJVVW1Ol3IlaJdJ2O3AGT3NKVsJr9k,2526
 super_gradients/examples/convert_recipe_example/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/examples/convert_recipe_example/convert_recipe_example.py,sha256=qL9jrzpSIgXr0lRV9WrsM0tvqrPIBIM6QkV-ys7g8hQ,870
 super_gradients/examples/ddrnet_imagenet/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/examples/ddrnet_imagenet/ddrnet_classification_example.py,sha256=K0p9d0iJFpGTGqYXjxaODIoTH6MZeGOJLMeqJK8B0JA,3114
 super_gradients/examples/deci_lab_export_example/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-super_gradients/examples/deci_lab_export_example/deci_lab_export_example.py,sha256=k7XkE--u_YOQrGmaowbWRjbceX6BHbI9QysMwKtKiHE,3562
+super_gradients/examples/deci_lab_export_example/deci_lab_export_example.py,sha256=b1RBkw8nw0k6QgN_O21jH4-Qfjd4Ovpy4PxVflo8T3E,3036
 super_gradients/examples/early_stop/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/examples/early_stop/early_stop_example.py,sha256=QH3mQGObo3BmkZ7EQ394eDVmaABMmtEy3n9A51DfaOk,1596
 super_gradients/examples/evaluate_checkpoint_example/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/examples/evaluate_checkpoint_example/evaluate_checkpoint.py,sha256=MNCuzc90O3d0TSVsFJZUSZQt-8V903pSHNUD7CdJ5Xo,289
 super_gradients/examples/evaluate_from_recipe_example/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/examples/evaluate_from_recipe_example/evaluate_from_recipe.py,sha256=IipK4OmfwP77IaGpnhOaiHdzY9sE0KF3WZJ58ZtFLHU,292
 super_gradients/examples/loggers_examples/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -152,39 +154,39 @@
 super_gradients/modules/base_modules.py,sha256=OhcjlGzj6vKjQkxQP40A2C535ScwVo9eU5DiQGrEB2I,776
 super_gradients/modules/conv_bn_act_block.py,sha256=uJgtSZbW_km3zvlS9hh2PzxgmHjeiINtNEC9RlffD6Y,3054
 super_gradients/modules/conv_bn_relu_block.py,sha256=pZ0OazMsoP7PxjV6-ltgR8IytjsF6tsC71GH4kRgEgE,1976
 super_gradients/modules/detection_modules.py,sha256=srfbJXd4tWk4UL92Wu2Lq2l6qI3YvzSP_Khjtsn9fS0,14805
 super_gradients/modules/head_replacement_utils.py,sha256=sDXb1CiJN08-mpjrdzyY46s_FEG72yFx2YsF2Rl22Xw,2143
 super_gradients/modules/multi_output_modules.py,sha256=YLofR05Z56k4iHM460KRO-GQ4jMcP1MrrrgT-aOcew4,4362
 super_gradients/modules/pixel_shuffle.py,sha256=Rcka24mhF8fR5OuG3jgIGV1yUllaEOWZU4qFjKMheIg,860
-super_gradients/modules/pose_estimation_modules.py,sha256=PjYY28XkAz52KgREnCupoIbCCFM6TBYu1Shudmq7xxs,3953
-super_gradients/modules/qarepvgg_block.py,sha256=k5w_gvJyFfPiwPFEOJ909Rmq6x3IVS9qTM30o-Hg3iE,11773
+super_gradients/modules/pose_estimation_modules.py,sha256=hrrxk7FOF6-chFQPudJpgciUx_NNEspHbFVN2z3ZD6U,3927
+super_gradients/modules/qarepvgg_block.py,sha256=llTOYC01wH0wMvtiAyyF4iaCipC2gLQax0Z-29boWwg,12250
 super_gradients/modules/repvgg_block.py,sha256=RIc3Iq7Ce1JwatM-acmpWCYV8gpMtu9AXV1lo5BkFEw,8699
 super_gradients/modules/sampling.py,sha256=xcGx0oIvQGyPjtZFGQko_vybYYtQk-mL2AFA0G4MULs,2138
 super_gradients/modules/se_blocks.py,sha256=itIUGGoqKNBYhAyj20aKcRKQlK_HdD0sqCsfK-a8yE4,1459
 super_gradients/modules/skip_connections.py,sha256=QR1V7AG9_4eK3xgywanDU4NpK5HMiv_jy2AMOgH0di4,1403
 super_gradients/modules/utils.py,sha256=B3h8_ABd15fS6yaozvG7xsAc0VfuDNmGBKm3ty-Yejg,2968
 super_gradients/modules/quantization/__init__.py,sha256=YNuNoitnDrNS30BBeadjiGZfqOTdZu_GPTbiHyLmPV4,716
 super_gradients/modules/quantization/quantized_skip_connections.py,sha256=0NaQ63tdFC9s7YL1VV9VLheUYaN4pb29kjw_etmzR_g,2649
 super_gradients/modules/quantization/quantized_stdc_blocks.py,sha256=aahisE-qutTEnfVH2rfRKhUYEKssuTJTPnuBIq7lYHY,4604
 super_gradients/modules/quantization/resnet_bottleneck.py,sha256=QxcKN-ogzI1lDD8EeYjD006mCNouFfyekLvIjnhnffs,1281
 super_gradients/recipes/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/recipes/cifar10_resnet.yaml,sha256=iwUtqtF5OU3Hm59HTZUGa6sw6bUmNYdV6HWsr5PJ7kA,1136
+super_gradients/recipes/cityscapes_al_ddrnet.yaml,sha256=kQmDHkxbYrwSyGtiP1baLRBq9nbeaJXtXGRcTqOnKCc,2727
 super_gradients/recipes/cityscapes_ddrnet.yaml,sha256=vPqkLwq9wpdXDqI7EUyPWgsUjjdK_k4Qckvj-jjErsE,3502
 super_gradients/recipes/cityscapes_kd_base.yaml,sha256=xOLxh4xcZigl6b1tQMV_IgMV37q6sKbo5j6RNxHbx9o,3754
 super_gradients/recipes/cityscapes_pplite_seg50.yaml,sha256=_iADDPmvD18DzmbgTMp-r2n3DFt3pJer7FFG4i_MOok,3354
 super_gradients/recipes/cityscapes_pplite_seg75.yaml,sha256=febqi42cSfZ4om7H0lRh2Ow8W1wxIbobcUWbiQt4t_8,3253
 super_gradients/recipes/cityscapes_regseg48.yaml,sha256=4PryJjKoJThIUZpsjesGr69i0fAThS3JDBBjYfQ-raA,2498
 super_gradients/recipes/cityscapes_segformer.yaml,sha256=DFy2Ir5L0NsB8zG1QD4FevUzVRDCQmTUmGu0M4XSQto,4020
 super_gradients/recipes/cityscapes_stdc_base.yaml,sha256=FwZUsUiS75o2RTauG-r1LEVB8I7xYJhKr_0fJhUh4Vs,618
 super_gradients/recipes/cityscapes_stdc_seg50.yaml,sha256=lCxKTpftQbIwz00q3t6Tukl2hALIny8hkrAB4KJkAqQ,2862
 super_gradients/recipes/cityscapes_stdc_seg75.yaml,sha256=s3H7De5muLfu6kNjRbAOccF2_mHkch98HppPnDmSNig,3055
-super_gradients/recipes/coco2017_pose_ddrnet39.yaml,sha256=sfAmnASFeFoS0QQI-ou9BnsxjOP2xSvfslG9HdfWQQM,1830
-super_gradients/recipes/coco2017_pose_dekr_w32_no_dc.yaml,sha256=cOdwPOV46ISu8fEI690_nO0gsbgTwFqb5Z6lpUfzrEA,3549
-super_gradients/recipes/coco2017_pose_pppose_l.yaml,sha256=r3Y_9Mat5vsmQ4_Aq4sUz37rGuGe6ydHcwOo3H8O0-c,1998
+super_gradients/recipes/coco2017_pose_dekr_rescoring.yaml,sha256=x5sSxB4_ANfmoNO_-VGQ20J8kwJ2P5xwGVsnuYf1cik,1620
+super_gradients/recipes/coco2017_pose_dekr_w32_no_dc.yaml,sha256=LSLNHa42z9-O41o6lIZcjCr-HpXZ9mFhh2N6BEH_8vc,2992
 super_gradients/recipes/coco2017_ppyoloe_l.yaml,sha256=bW0yA0E4P91lqF3-9G-dQfVB3GZNaI40okJtgZ-F7O4,1996
 super_gradients/recipes/coco2017_ppyoloe_m.yaml,sha256=HV8O7WVRjgz33aD62zYPIBOErNW1sbSEMyusQoy7QkQ,1996
 super_gradients/recipes/coco2017_ppyoloe_s.yaml,sha256=a9LHnLPYKntNr50nZaNw6DAhBMOpqUrgjYdsjv_tNR0,1882
 super_gradients/recipes/coco2017_ppyoloe_x.yaml,sha256=9FfoIZzlzCjvzeif8N6Vr90IRclWzfE1V6i4p_3voDk,1975
 super_gradients/recipes/coco2017_ssd_lite_mobilenet_v2.yaml,sha256=xbz3qng4_jBT0YeBImpmSWoXwYGY2X0USbfFRaArNOY,1889
 super_gradients/recipes/coco2017_yolo_nas_s.yaml,sha256=2_FpHOih3btRm7gX7Hok2W1ItpokXxTUHh6fp8b6yZI,1385
 super_gradients/recipes/coco2017_yolox.yaml,sha256=pLonL8nqJ87OAwNkbTP1VtPDlRN_4x1JbZ0z1INVPKs,2583
@@ -201,14 +203,15 @@
 super_gradients/recipes/imagenet_vit_base.yaml,sha256=dnvr4h7-d1XHhF09Q9dZWoNLGZvdCZZys32siTH1Ta8,1136
 super_gradients/recipes/imagenet_vit_large.yaml,sha256=QuI6OVc5XAUcIUsOfnFpcO76jZ79HMhhwnk8Aq_azaU,1010
 super_gradients/recipes/roboflow_ppyoloe.yaml,sha256=ukl-e8Qze0hZ-ENcD93PTql5xaNHtcVIItzDJF3yGWI,2007
 super_gradients/recipes/roboflow_yolo_nas_m.yaml,sha256=qpOIQmV3mwelxK5Xn8RXPFhE6Cb2dlIPm42WlvP-eok,2347
 super_gradients/recipes/roboflow_yolo_nas_s.yaml,sha256=Gj1L8Ky92PcX8pQ5wKKgc353HGzJYun4xuoQkMgGfpk,2347
 super_gradients/recipes/roboflow_yolo_nas_s_qat.yaml,sha256=-zTGn37Y59d_9_z4HSsNfcEZ7eNr8j4Zi-VAv3-l3so,473
 super_gradients/recipes/roboflow_yolox.yaml,sha256=d6Y-nv_7p9SX63d8kJ1oiPS-U6Znu6DLye5IvIP9ypk,1915
+super_gradients/recipes/script_generate_rescoring_data_dekr_coco2017.yaml,sha256=D6OvC2Qz14mqHe3hfNHk4V8cfhG4f1h4u28eE5TwXkc,1344
 super_gradients/recipes/supervisely_unet.yaml,sha256=L1bl1QsgThj9iv5dEZSSGMBYFR1SmW9Mgr7cddaXOoE,1246
 super_gradients/recipes/user_recipe_mnist_as_external_dataset_example.yaml,sha256=XR86Cg1sGjgoT8RHjdpnhJA01tFXYTz3QqiLYmLO46E,1672
 super_gradients/recipes/user_recipe_mnist_example.yaml,sha256=JtzZebnnTPGQUgsqu6i73zb5uF0l6_LPNnuh2q3UYD4,2133
 super_gradients/recipes/variable_setup.yaml,sha256=189UzdcCcHLw37-W1XF0W-j1k80IGMcMd8JkHwBXI9E,2000
 super_gradients/recipes/anchors/ssd_anchors.yaml,sha256=iRsfDXt3bWyCvmZtOQK-Y2maAJEgfgXVWF5sos6r7RU,2222
 super_gradients/recipes/arch_params/efficientnet_arch_params.yaml,sha256=dEn_jgEn_NA80xaugB6lY1mdRRjVcOTwnckMlVmdbXE,563
 super_gradients/recipes/arch_params/efficientnet_b0_arch_params.yaml,sha256=jQfnMGb1kcprnr6UnUbmYaNwslEn728j-8Ci5NpX63E,104
@@ -221,16 +224,16 @@
 super_gradients/recipes/arch_params/efficientnet_b7_arch_params.yaml,sha256=QtyQb5EY_dUZydU94t39111d82vV5mAp4Wbq2JZlrKI,103
 super_gradients/recipes/arch_params/efficientnet_b8_arch_params.yaml,sha256=ALS6kf1BY3eBeFHTvoMVgp9ZVZ1vPXNgzTVn3scZEAo,103
 super_gradients/recipes/arch_params/efficientnet_l2_arch_params.yaml,sha256=AKCehy-NKiRXMCjmHs8u9-F4QtQGH7NxjTLtuvGybNU,103
 super_gradients/recipes/arch_params/mobilenet_v2_arch_params.yaml,sha256=aV7XQ9mFxZwsf2DHPuy3gJp2ScA2Z9wPHti4al341Co,194
 super_gradients/recipes/arch_params/mobilenet_v3_arch_params.yaml,sha256=NJe2vbIFbe9__tf1LuEMykNkHxF_5ofWNWMi4rsXSig,156
 super_gradients/recipes/arch_params/mobilenet_v3_large_arch_params.yaml,sha256=ky9f9lsQLJAcF0sUN-tYiZbMRpVIZAtwQTlrjPrpYpc,409
 super_gradients/recipes/arch_params/mobilenet_v3_small_arch_params.yaml,sha256=tAx0Wqeg0e0-rRjKPZyqB4Jvehe29u_ubJNX0cA3y6c,356
-super_gradients/recipes/arch_params/pose_ddrnet39_arch_params.yaml,sha256=9sUcs_iO7PPj6-NXuAZfrlmZ3IkF7qhRtoZv90iEyaI,281
-super_gradients/recipes/arch_params/pose_dekr_w32_no_dc_arch_params.yaml,sha256=xaZliOTrJ3SVwC5BCW5_BSKU9U2QG-Y_fsPS3YuO208,1245
+super_gradients/recipes/arch_params/pose_dekr_coco_rescoring_arch_params.yaml,sha256=0Ypq4caGTdodre32LZQz3970M-V_Wu06nmnABrKc8Uk,324
+super_gradients/recipes/arch_params/pose_dekr_w32_no_dc_arch_params.yaml,sha256=PXIq_uMnPqfTa4IxfvhTFxYmaZEigFpFUAKBTxs0zqA,1113
 super_gradients/recipes/arch_params/pose_pppose_l_arch_params.yaml,sha256=qn1K7oUioAXHtNlg8gWqhkRWlXdF357eWSO8BhafJPY,985
 super_gradients/recipes/arch_params/ppyoloe_arch_params.yaml,sha256=l2jwsHzlQgb6mGMspWRMk2G0WA7VXVjSsioAVB_6rHU,1112
 super_gradients/recipes/arch_params/ppyoloe_l_arch_params.yaml,sha256=FzRo92_R5fXhHIbKYjKt_gcN97fl4sk4T-2SH6SVnaI,196
 super_gradients/recipes/arch_params/ppyoloe_m_arch_params.yaml,sha256=hTogCyoRf0tHU71NAxxW_lY1_6cK5dKBNra0pwnAlHM,198
 super_gradients/recipes/arch_params/ppyoloe_s_arch_params.yaml,sha256=KSbtJ6yeajB_PIvkGyCR6UFwXJB6VzH1NQbJa4m1EOM,198
 super_gradients/recipes/arch_params/ppyoloe_x_arch_params.yaml,sha256=wSVUpGaOQy74g9HqzHRqO0zOZIe4KkjzK-m9ocQcoM0,198
 super_gradients/recipes/arch_params/regnetY_arch_params.yaml,sha256=Ji34AM3NJDmxOzm1288GQ5jn9rRcYKd0z2BGZNxx0d8,204
@@ -246,45 +249,47 @@
 super_gradients/recipes/arch_params/shelfnet34_lw_arch_params.yaml,sha256=DIfTJiaYSnb9HiQ67sV4I0TRRz3bGjUIif3Enm5fmC0,32
 super_gradients/recipes/arch_params/ssd_lite_mobilenetv2_arch_params.yaml,sha256=mgc7pa4Do5BNpjklXwH5zYPPw9_fGU_U2O8CzT8Md_8,655
 super_gradients/recipes/arch_params/ssd_mobilenetv1_arch_params.yaml,sha256=HiuGU1M0fDqQVVJWkx5VpZJaO4XYShwQyzpPxqJO0Oo,605
 super_gradients/recipes/arch_params/unet_arch_params.yaml,sha256=U-7HSXzOXXr2-d6xQjNJF-8oD1KLhD1WqqaThI0atUk,1369
 super_gradients/recipes/arch_params/unet_default_arch_params.yaml,sha256=ONkf6v0Msq4b9Ucxkv3TZWgW_RXmvhomkmo_5HeXzaY,3031
 super_gradients/recipes/arch_params/vit_base_arch_params.yaml,sha256=Y6skbVr98NRSf5Ts4c47JPwsDMudqygFu5W4ZQiXkLo,63
 super_gradients/recipes/arch_params/yolo_arch_params.yaml,sha256=GroGr-T0l_puiM3nPIT3Y_RzuwhNrv3U5s4g5y1Pijo,2393
-super_gradients/recipes/arch_params/yolo_nas_l_arch_params.yaml,sha256=yYHct24_5vEwR4XuZwxhuSqMn3tZGV70NiIKiR8gaW4,2337
-super_gradients/recipes/arch_params/yolo_nas_m_arch_params.yaml,sha256=83LcAgVeVv1PZjf3_fOOs4b27Y0PUpoHT2zLWBZCCWA,2346
-super_gradients/recipes/arch_params/yolo_nas_s_arch_params.yaml,sha256=IGC8VN-OuFCasSMUTEOKoukSQDt6N_-b9VUrc7mVZNU,2341
+super_gradients/recipes/arch_params/yolo_nas_l_arch_params.yaml,sha256=e9ukkOP7iTaSyXiF-Oku2uFysjBQ4qEQg3r1CB-Zb_s,2353
+super_gradients/recipes/arch_params/yolo_nas_m_arch_params.yaml,sha256=3CepP0eA8mWgpmayuEEw1ud4IDBc96wJ22wEPqLv_Hg,2362
+super_gradients/recipes/arch_params/yolo_nas_s_arch_params.yaml,sha256=GG_-WGuyIaE0t4lTkcXNASdNVKbEtM-iZTmXvyqc9fg,2357
 super_gradients/recipes/arch_params/yolox_l_arch_params.yaml,sha256=lmtcOUvHlhQf9anw1ybaks25GETvHu2QpH2D9jJqEUg,235
 super_gradients/recipes/arch_params/yolox_m_arch_params.yaml,sha256=atByNWwQqnpaZ7SXEW2Q5cKo0T99V447xLhh1NoShFs,237
 super_gradients/recipes/arch_params/yolox_nano_arch_params.yaml,sha256=1yJcwDkZwKlL_6MeWjyypFtsPyyC9CdNWquRG7gQoXI,237
 super_gradients/recipes/arch_params/yolox_s_arch_params.yaml,sha256=J2qgjwp6VxRcNsRomCyZtdV5Ht3RruMZmYJagtlzttU,237
 super_gradients/recipes/arch_params/yolox_tiny_arch_params.yaml,sha256=rxYvMOUeT5jnGhZ9-OTZ4ohHgheLDdHyNJ4_-m6JSQU,229
 super_gradients/recipes/arch_params/yolox_x_arch_params.yaml,sha256=Wsg5AnPiqHZTnbTLFGUr90eS5a45F9ko0dfT8XTZbPQ,228
-super_gradients/recipes/checkpoint_params/default_checkpoint_params.yaml,sha256=XpQsqckADGZgsZHxW6bc0vF971bRz0kpyuP_1dH6aRI,611
+super_gradients/recipes/checkpoint_params/default_checkpoint_params.yaml,sha256=2QEGvJGtvJKu5abLEaVCz-PEzqZ4iQytBFesTKFWOuc,622
 super_gradients/recipes/checkpoint_params/vit_base_imagenet_checkpoint_params.yaml,sha256=VYKzkX1jD8sB9NH9rLHc2KFCPx83Zn9c8SptLYSDjpM,72
 super_gradients/recipes/conversion_params/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/recipes/conversion_params/cifar10_conversion_params.yaml,sha256=GEM_wvMaJqERXYOkKgz2G0vUUpzo3NV_DuARpkBYkww,1807
 super_gradients/recipes/conversion_params/default_conversion_params.yaml,sha256=u2CB5clR_aud10_nDsoqGinb2W1dJK-_8w46BbMFkhg,2040
 super_gradients/recipes/dataset_params/cifar100_dataset_params.yaml,sha256=fg_lvX7KrY8XEuUwfC2PP2vcfXLmX2YTdu7twh4fzjI,869
 super_gradients/recipes/dataset_params/cifar10_albumentations_dataset_params.yaml,sha256=t3w9oe7aIUSBNhQWnPClAtFs77m8QCijbO4qKGpnr08,1530
 super_gradients/recipes/dataset_params/cifar10_dataset_params.yaml,sha256=Uz3J9LB42eM6n08Dz7m9BG5VIWM2lnPrXy2eOySa6gs,1056
+super_gradients/recipes/dataset_params/cityscapes_al_dataset_params.yaml,sha256=JLF78e6Q-eD_-0A4ng4apYaHrMBVRN7EoaQrk1hQzv4,1328
 super_gradients/recipes/dataset_params/cityscapes_dataset_params.yaml,sha256=1NjXHAMg_znj2v-UHR57daxXpzLPvN3ZIMLKwsH5Zso,615
 super_gradients/recipes/dataset_params/cityscapes_ddrnet_dataset_params.yaml,sha256=HUr8IaV0IIfuxK-fibY42yKUHe04kUCBFnYAE5E3rGI,525
 super_gradients/recipes/dataset_params/cityscapes_ppliteseg_seg75_dataset_params.yaml,sha256=CKSennwvRG1a-swVvL1he18vdtNRnCStH3LFhruGSnQ,706
 super_gradients/recipes/dataset_params/cityscapes_regseg48_dataset_params.yaml,sha256=dtbvoxt9IR9cBaslNOWCcsX7s_gjHRnWK5Ayl1ElzmI,644
 super_gradients/recipes/dataset_params/cityscapes_segformer_dataset_params.yaml,sha256=i7l9LXea216Y2RB8e3FxhlGNBR_a1tLJKCg2Ix8JsTI,721
 super_gradients/recipes/dataset_params/cityscapes_stdc_seg50_dataset_params.yaml,sha256=WK7UH73r-nuHMKepBVyykR0tf306s-P5NgQNGI-dZWk,709
 super_gradients/recipes/dataset_params/cityscapes_stdc_seg75_dataset_params.yaml,sha256=wBHhYk6Q6kdmLDk9tTi0vpREr0fhTz4r1Zh0ybrRPGw,708
 super_gradients/recipes/dataset_params/coco_detection_dataset_params.yaml,sha256=x8wk7EC6eKGlxSyaBTxKGJidss5BbgX1MTG9KLCnU0M,3946
 super_gradients/recipes/dataset_params/coco_detection_ppyoloe_dataset_params.yaml,sha256=GeCdBxnGf5WqQ165WIVCg4jz4vmjqT2LzofdvXB6bAs,4202
 super_gradients/recipes/dataset_params/coco_detection_ssd_lite_mobilenet_v2_dataset_params.yaml,sha256=PqQ6fBINO3sHHAAGx4rHKz4PAURkd67qPrVLWu1WM5Y,3590
 super_gradients/recipes/dataset_params/coco_detection_yolo_format_base_dataset_params.yaml,sha256=kbFd4bvfi8bhpX1qALfyjLZ3At9eHdC0J80w-a3OUkM,5568
-super_gradients/recipes/dataset_params/coco_detection_yolo_nas_dataset_params.yaml,sha256=un_vfACn98dmTwPXS1AlpC6I3uRnZKTlE4MbZUGITsY,3646
-super_gradients/recipes/dataset_params/coco_pose_estimation_dataset_params.yaml,sha256=qHBh-kCmrXr5ICR0Ww_C1B2RywSEOz4nVSZSt96K-aU,2461
+super_gradients/recipes/dataset_params/coco_detection_yolo_nas_dataset_params.yaml,sha256=Nex5fWsHcmS5KJSkb32HNFaiXHVdovNKJMliXnLzg3U,3684
+super_gradients/recipes/dataset_params/coco_pose_estimation_dataset_params.yaml,sha256=T7GkJR2HFNeJYZzkHvAINP7ubHtN5xdhVNekPh4oZ84,2700
 super_gradients/recipes/dataset_params/coco_pose_estimation_dekr_dataset_params.yaml,sha256=q8s65W76DEu9XWRY_gR9fyr5Xp5HH1vLh8eG9ZvR7fA,405
+super_gradients/recipes/dataset_params/coco_pose_estimation_rescoring_dataset_params.yaml,sha256=FOP_E-fLf3stEg8TNpDRfwLbWq_NvvVTXge6GcNyTeo,842
 super_gradients/recipes/dataset_params/coco_segmentation_dataset_params.yaml,sha256=SC_nc2CyZqQ7R-z4pcqoTyZlBZB7JlmT_5hzgMjHCRc,1466
 super_gradients/recipes/dataset_params/imagenet_dataset_params.yaml,sha256=9JnbyZjCkZ3ZdMHj0CwVkQdzi7QBevwmoK1KQlxlymU,931
 super_gradients/recipes/dataset_params/imagenet_efficientnet_dataset_params.yaml,sha256=CILfhTGk4ne0wk0L7gbD95EjBTKGGTR8UjCaTW79Joc,732
 super_gradients/recipes/dataset_params/imagenet_mobilenetv2_dataset_params.yaml,sha256=lp64i0smov-lT6Xko9-fzVsxWO0UWdimXQnwrx0D3sY,794
 super_gradients/recipes/dataset_params/imagenet_mobilenetv3_dataset_params.yaml,sha256=YH7UxRgDjcR3qWs0yifxlgHsckHRqEYWx-kYRwNhPVo,142
 super_gradients/recipes/dataset_params/imagenet_regnetY_dataset_params.yaml,sha256=Hf9BHIs4N2oRWpph7xr7x5AOZtBbV5eEaMOlShORjQg,734
 super_gradients/recipes/dataset_params/imagenet_resnet50_dataset_params.yaml,sha256=SiPRDxzkwoOMDtKqzM7p0c5M658dQNEMQRvFH24K3aA,1059
@@ -296,133 +301,137 @@
 super_gradients/recipes/dataset_params/pascal_voc_segmentation_dataset_params.yaml,sha256=eIHwt4ZsVYKtpQbNSk1ZbsdneEZ6twlZkpxVG9LLt84,1414
 super_gradients/recipes/dataset_params/roboflow_detection_dataset_params.yaml,sha256=k9D4xbYMsuJv88r6m7MOeB3vQ37sUSnD94BQMMMExSM,4112
 super_gradients/recipes/dataset_params/supervisely_persons_dataset_params.yaml,sha256=GshRG6Jqdb1S9uoBjWbckkSajIPo6Avuf46WXFMcC5w,961
 super_gradients/recipes/dataset_params/tiny_imagenet_dataset_params.yaml,sha256=4_4HkNjzZDKFHpgSV1-S0s9rRrZJUj5S-7zUk1wOFaY,559
 super_gradients/recipes/quantization_params/default_quantization_params.yaml,sha256=OVewy7FMpSUpheoL7_eAzbJVpcfy5O2eIwpEri0tUc8,1155
 super_gradients/recipes/training_hyperparams/cifar10_resnet_train_params.yaml,sha256=jZV1VVe3Lda96Mq-hb8zHfR3EATHt0kSGLOpcdxssFg,591
 super_gradients/recipes/training_hyperparams/cityscapes_default_train_params.yaml,sha256=NUOLRusDJ9H6Nxp-NGVsie7tPuRXKE493jwzI_U8rqE,700
-super_gradients/recipes/training_hyperparams/coco2017_dekr_pose_train_params.yaml,sha256=vh7Ej8ViU6qH7B87femqWgoxkE2WYxYhTFNsR-8JzK0,877
+super_gradients/recipes/training_hyperparams/coco2017_dekr_pose_train_params.yaml,sha256=JkLfCz7y-H0jOXzXvxHuqS--uFHfAj7ENwKLixblpmA,2063
 super_gradients/recipes/training_hyperparams/coco2017_ppyoloe_train_params.yaml,sha256=Ah9iuCKngV2Bri_R0PPB-p5SB0oPpVYGs38yG83X-kU,1302
+super_gradients/recipes/training_hyperparams/coco2017_rescoring_train_params.yaml,sha256=EwmB6KWcfozUG885htJHZxlr9tbF5N_nBelFBESVQ0o,771
 super_gradients/recipes/training_hyperparams/coco2017_ssd_lite_mobilenet_v2_train_params.yaml,sha256=vuTXdVTzwM52w1n44mGBB-kJKluXtmxymgmbdLg85Jw,723
 super_gradients/recipes/training_hyperparams/coco2017_yolo_nas_train_params.yaml,sha256=wjpqncCxlCxTg2zH30OoqqdctXYcoWz8nDOkD7DPTyM,1121
 super_gradients/recipes/training_hyperparams/coco2017_yolox_train_params.yaml,sha256=hMDTZejrlTXQxuSJPXyW6jdxTrd5De5IoilzpP-Fmis,956
 super_gradients/recipes/training_hyperparams/coco_segmentation_shelfnet_lw_train_params.yaml,sha256=4k8cytIVPZH37ALyCqhziIA9i8HDrSwyvK1nrk1et8w,461
-super_gradients/recipes/training_hyperparams/default_train_params.yaml,sha256=ZR6x6QR1Bc0YGwj-dKPITmxM7Qkava0du6RGhUC8n4s,5459
+super_gradients/recipes/training_hyperparams/default_train_params.yaml,sha256=iZclyubNwwIUwHeEeadZjvyZztDD1yCqqQEcrdm1ZdM,6081
 super_gradients/recipes/training_hyperparams/imagenet_efficientnet_train_params.yaml,sha256=ueqNFnlvkCj78yA70mPDPp0n6AcikQkfCl35XLLE12c,794
 super_gradients/recipes/training_hyperparams/imagenet_mobilenetv2_train_params.yaml,sha256=xrCPTtKoJ85TjCART4sOLWMc7b5p2X2ZARt41WYScj0,742
 super_gradients/recipes/training_hyperparams/imagenet_mobilenetv3_train_params.yaml,sha256=xLXjLxQUyh6RJzBEtvrBPhKRAZre7OuVSZyAvErk3XA,549
 super_gradients/recipes/training_hyperparams/imagenet_regnetY_train_params.yaml,sha256=A5j4hUflhQHwIPR8awxs64GuEH3AAFJbWT-Wo3g_nAs,795
 super_gradients/recipes/training_hyperparams/imagenet_repvgg_train_params.yaml,sha256=XH-fzy5kx9HmMW6pA-0nmnWMxpcpdrIcTQ-Imyy8tsM,476
 super_gradients/recipes/training_hyperparams/imagenet_resnet50_kd_train_params.yaml,sha256=ebSVisdQvy4Shvzh95tKkXMD6VQkkrPLhBKuR-jOBVw,484
 super_gradients/recipes/training_hyperparams/imagenet_resnet50_train_params.yaml,sha256=DO5N9jxrfn-jEoJS74JMghZB5ZN_nvLA3llRLe7NTLY,522
 super_gradients/recipes/training_hyperparams/imagenet_vit_train_params.yaml,sha256=_-n1iLYFwhEDBxCnO8L5OTa8A5gKvVgTPC19g5wVx9A,602
 super_gradients/recipes/training_hyperparams/supervisely_default_train_params.yaml,sha256=NoLNnoAVy7-P7IJAymyPY7sjhiNuy973WHttv_Hh8eI,519
 super_gradients/sanity_check/__init__.py,sha256=IrTB1Lxw15cKFjxV8bGraUxj5d_pmEqYk7FHa01nuvk,107
-super_gradients/sanity_check/env_sanity_check.py,sha256=2_55JKDSsL1krMuXrWbF_qpz3Ob5SHP8lTYvSO5Ie-Q,5262
-super_gradients/training/__init__.py,sha256=LaqXsoTNBBFvGcV14K7tjt0iMbQdEy5NINJEycpcrPw,666
-super_gradients/training/params.py,sha256=I62jGc85o5YZeQDfvv9uUDyDKFeUnwXpR_i5rSZ2aZs,4155
-super_gradients/training/pretrained_models.py,sha256=I1cVvTBgbZj4gTvFxm55BrREuBJhAr7JlJa_KkoGyw4,4301
-super_gradients/training/dataloaders/__init__.py,sha256=fnGUu4drH1B6VLb2efrJLV0s4DnoTEbyKHDcHmEH5qA,3224
-super_gradients/training/dataloaders/dataloaders.py,sha256=7Qvjr9-aSiXmHpD6anjCiwHzCklCJVnJP0FR-XCeLSE,32361
-super_gradients/training/datasets/__init__.py,sha256=nptSnL6f7srktNihvAqw5polrwp4K-IrhTWPQ9vFLEM,1811
+super_gradients/sanity_check/env_sanity_check.py,sha256=bq20O4wh04bPeRo1xv9-xDFaeU6_EOtXCd-PP7Fb9tc,5267
+super_gradients/training/__init__.py,sha256=dBnpzi4Z1qNEMKpPhupeACBpSh6bXWoTwXyWn8cOC8I,775
+super_gradients/training/params.py,sha256=33QsbQo384OfUmKzA6x04Wf0cNJHiu-5yFcfG_rXzxQ,4715
+super_gradients/training/pretrained_models.py,sha256=GXfv3BW9msTEU_KZetZHDjHyxs3tQTtWXORG8TngBh8,4518
+super_gradients/training/dataloaders/__init__.py,sha256=AeUX5aLgSkFmOUGdwBe-JnBYoNc3dqT9h4ofK9dHvuw,3344
+super_gradients/training/dataloaders/dataloaders.py,sha256=Lgb6GmFyoRIJIHdDPtHfwNRFshUXXq3ySXDNbniD1NM,36154
+super_gradients/training/datasets/__init__.py,sha256=_8d9MmxGw3IFxOtZlbf7-ZYnlmyxpmZiTl9cbMyUNt0,1867
 super_gradients/training/datasets/auto_augment.py,sha256=VHw-Wq4ecHSKcqe9l63RUGpNa6JygUP3N7B6hbnTPxg,14162
 super_gradients/training/datasets/data_augmentation.py,sha256=TJOIT7j6ZWaNW6E4VvkJ-ARIWBY7Y4210NqrZbzKJJ8,3705
 super_gradients/training/datasets/datasets_conf.py,sha256=U2FTTYwCFp3cFZkzliWSGCHuCUUrns57AX7uS5Wn5NY,3484
-super_gradients/training/datasets/datasets_utils.py,sha256=oZnyLGBkfibkczYP2t69xf2OtqPU8ixyWDlc3iXQJh0,30279
+super_gradients/training/datasets/datasets_utils.py,sha256=FXaIOEoYEJ-eeWoh63kZRNwc6XdBs94JMAkDkCd9tns,29577
 super_gradients/training/datasets/mixup.py,sha256=WDHoqTFbq-PGemKxE0eZ10Q03mpH8GIj-vFBNIZEg1U,14663
 super_gradients/training/datasets/sg_dataset.py,sha256=xVqf-7vvGk96TkshGHIcqiQfIVXdOCs12U1fcJjWrX0,11746
 super_gradients/training/datasets/classification_datasets/__init__.py,sha256=LcdaPeIQxwDM_qRb-sEwVswsjSveuZcdndpZKusGGsQ,252
 super_gradients/training/datasets/classification_datasets/cifar.py,sha256=lH_iBhC2igE_KQEJb_Lc1FpKvs4QsnuCxzOTIE0qNUw,3096
 super_gradients/training/datasets/classification_datasets/imagenet_dataset.py,sha256=idY9fSwXxrgqJt9lJOaLFsQS0hz5qX6BIbXHBW_TIrU,1706
 super_gradients/training/datasets/data_formats/__init__.py,sha256=V2Sioujv6egladjkcsgceQ-goRUpja2Ey0ma-DDihWc,862
 super_gradients/training/datasets/data_formats/default_formats.py,sha256=GbP2UWXISbkfKtP7rjV2Qag3Q5BrlwU_RDzdM8DJuDk,3927
 super_gradients/training/datasets/data_formats/format_converter.py,sha256=yMJj-9REVJ_T-JkPB34IJsQzpxWOhhnlxxRNRhMUSqU,3071
 super_gradients/training/datasets/data_formats/formats.py,sha256=Aa3odNETBnS5_ZC3TcKOevqr89gw_qWZKZpS9Gb_wPo,7928
 super_gradients/training/datasets/data_formats/bbox_formats/__init__.py,sha256=p9pa3hZA3tzVf7xCWqnTRlKr03i4NjxIbUic_IHt7U8,1044
 super_gradients/training/datasets/data_formats/bbox_formats/bbox_format.py,sha256=ID3k0HeqcWUWBqyFMvyKkiAtY44u-3q5lSe6m0EprZE,2674
-super_gradients/training/datasets/data_formats/bbox_formats/cxcywh.py,sha256=V1-2q4ULIIyc2XO1e3MENu0XbOcR9riVh2L9t0XvdMo,5094
+super_gradients/training/datasets/data_formats/bbox_formats/cxcywh.py,sha256=Vn5dKuIrqOihq9Cc8oDm3k3WBanNB3QDjzt_gfUgy3k,5131
 super_gradients/training/datasets/data_formats/bbox_formats/normalized_cxcywh.py,sha256=OzZJc6ZUMcJXiVeEulmAAVYt67yznNRPik0NE6bMESM,2089
 super_gradients/training/datasets/data_formats/bbox_formats/normalized_xywh.py,sha256=NaVEMg1EEC71ZK509wyts-rHND6DYnSlqxc2wRk6t7E,2043
 super_gradients/training/datasets/data_formats/bbox_formats/normalized_xyxy.py,sha256=a8BhAyUPCLuFbLTkE1uU0rOwQxRzOUaRVSU0GzAwSL8,5043
 super_gradients/training/datasets/data_formats/bbox_formats/xywh.py,sha256=VhtZmqnW1cxeo1azP-zPNcMYMPCzc4ZBBokkFWioqPw,2948
 super_gradients/training/datasets/data_formats/bbox_formats/xyxy.py,sha256=nCCohobPvCOtQ_SF2BAyyVyuSV68ZjjxrUurGfwNXMs,575
 super_gradients/training/datasets/data_formats/bbox_formats/yxyx.py,sha256=LChhVCXQ9-d9Zp3sa_PzAOrUBa15f_QKtxHdW51ocwg,1792
 super_gradients/training/datasets/data_formats/output_adapters/__init__.py,sha256=n7aH5WQzk_awjpei_GY-yOktBTw7LtzekY-gHJ8_AKE,92
 super_gradients/training/datasets/data_formats/output_adapters/detection_adapter.py,sha256=qH0LPewt8hvKE5jVaZl0HunzONd7UHErbBcCuK_rjZk,8373
 super_gradients/training/datasets/detection_datasets/__init__.py,sha256=g86eRhqJoDs-9snO7QR6zejTmqhF2Amq71O-ZZQLPZc,683
 super_gradients/training/datasets/detection_datasets/coco_detection.py,sha256=EUTVRS0igoBFeUDhXg_tqxJSDhGUEU45jdL8YYko2ng,2505
 super_gradients/training/datasets/detection_datasets/coco_format_detection.py,sha256=OJ0JEQLClxRgdMZlUpuVEH0jxRqwfTbhOZnHK4rzjuY,9258
-super_gradients/training/datasets/detection_datasets/detection_dataset.py,sha256=x5vDIU_XP2764cTm2EV6btQ76UALTWO9cFGv8Opsv8I,26159
+super_gradients/training/datasets/detection_datasets/detection_dataset.py,sha256=9BG__DvgmOmHSR_vgF1A9uKoFMwcgpzZFTBi_svZiK8,26566
 super_gradients/training/datasets/detection_datasets/pascal_voc_detection.py,sha256=pAtuVBRVO_Y0Q-diaHQz3tWyjW7U3xR04ohzPx-vkbo,11353
 super_gradients/training/datasets/detection_datasets/yolo_format_detection.py,sha256=ZP8zw0vvQ5CK-RkZ7EOGaLyLCAAzjuEev34SJQYVxag,11120
 super_gradients/training/datasets/detection_datasets/roboflow/__init__.py,sha256=Kw_KF41iHBr9tHrg6I6T6gdy8fgKLlG0NLCtXOyNpEs,328
 super_gradients/training/datasets/detection_datasets/roboflow/metadata.py,sha256=Ccxl7kt5F3E58oU4qJftnxIRaOc2iRyfCiyz_X4_lBc,18882
-super_gradients/training/datasets/detection_datasets/roboflow/roboflow100.py,sha256=9UEctKh8WxBLxdRP8wqfg3KDFq_KDYTr5AX4qD2Om7I,3504
+super_gradients/training/datasets/detection_datasets/roboflow/roboflow100.py,sha256=PkQ5CJdQ_jd9gYy4HcZTiODGbhH_IibXcNp_1k4cnAA,3503
 super_gradients/training/datasets/detection_datasets/roboflow/utils.py,sha256=_7mtuGnTHUVqfUqWlC9zpKGutBdaYJCGGj9pSbItfxI,1997
 super_gradients/training/datasets/pose_estimation_datasets/__init__.py,sha256=BeCVpXLn0FV9Oo_8iWtHz9n1GxdhXqTzymGT97_bdCA,502
 super_gradients/training/datasets/pose_estimation_datasets/base_keypoints.py,sha256=6xNszBrqqOOdIKgM2ZFOZ4Crwssfh096_AcLZL5R1q4,4910
-super_gradients/training/datasets/pose_estimation_datasets/coco_keypoints.py,sha256=aADh3OLNLBLCk-3_nxLHjrrHniqr-tfbIHjKzJf-REA,9066
+super_gradients/training/datasets/pose_estimation_datasets/coco_keypoints.py,sha256=WK7FD6fV_iDZSjvH4REc-8ZJkSBtOQq2_Fwgw35nWlw,9088
 super_gradients/training/datasets/pose_estimation_datasets/coco_utils.py,sha256=uMq0vV22npZqz21L_preyhbyKSHiBqS14Mp2UuEb-_4,5929
-super_gradients/training/datasets/pose_estimation_datasets/target_generators.py,sha256=McVUG3sWR9Lxgk_ca8ECqvYieQwZApsFRfLNABES51Q,10167
-super_gradients/training/datasets/samplers/__init__.py,sha256=CfddXWvnsVLbQyYkUGyBwdl98U8wj7-MfNPbGjZjl8g,278
+super_gradients/training/datasets/pose_estimation_datasets/rescoring_dataset.py,sha256=uDZYe4yuDANJNN7IseXKAunYwqL7d73wvOhB9TBuxMk,3736
+super_gradients/training/datasets/pose_estimation_datasets/target_generators.py,sha256=D7r0pXrv95zy_BFf9X-u26zsCaGuGcMQcVVPlus-eWM,10281
+super_gradients/training/datasets/samplers/__init__.py,sha256=bsLNxxZ61qQx2DbmGzsfd_6jDo4UYPkYNswoTOQtjrE,385
+super_gradients/training/datasets/samplers/infinite_sampler.py,sha256=ihUYmPJPKF0Z3lLdnQbGdlsB0jBmBxJvyySlXDbjyko,738
 super_gradients/training/datasets/samplers/repeated_augmentation_sampler.py,sha256=dnYh_2wWCFPlWVwnEhUEwhAaRpJGIGtoIbNiXSRAfq4,4809
-super_gradients/training/datasets/segmentation_datasets/__init__.py,sha256=5zkvFQ4Av5Ceydrnkq9jS19xp9axFBF7M-41K6DXBFU,1037
-super_gradients/training/datasets/segmentation_datasets/cityscape_segmentation.py,sha256=tRPCnl07gmducqFp9nm_ks5ZkRAZnIG5bQQTVKhweLs,6714
-super_gradients/training/datasets/segmentation_datasets/coco_segmentation.py,sha256=ehn6K8hMAItoGPA9NRa8T23z-oDeCQ-6jADRyBmu8i0,7717
+super_gradients/training/datasets/segmentation_datasets/__init__.py,sha256=JBkaU-0CwYInI7sdF_lbbFR8PPUFczMqF3Ose8wFaDo,1093
+super_gradients/training/datasets/segmentation_datasets/cityscape_segmentation.py,sha256=3hDw12hReFgaQelft0mXIhw70ccpnb-w1s4hMBSH9ho,8304
+super_gradients/training/datasets/segmentation_datasets/coco_segmentation.py,sha256=MqWN9UVMBcodqXm7LuC21MOazCsbBtL4ue7GXZgN80k,7757
 super_gradients/training/datasets/segmentation_datasets/mapillary_dataset.py,sha256=DcRz59FNdX3koBCth09AT1EEHn77xXoxBX-yaWa-fmo,5518
 super_gradients/training/datasets/segmentation_datasets/pascal_voc_segmentation.py,sha256=uQJyztsrnSHbxvzitYqixVeNeXN52UYZ66L__Pkcgbc,11146
-super_gradients/training/datasets/segmentation_datasets/segmentation_dataset.py,sha256=5uYUtLVaCj5J-Khw9xNazADAEAj6VvfZgRLOg1V9O6A,8470
+super_gradients/training/datasets/segmentation_datasets/segmentation_dataset.py,sha256=_nYIvWd9g0tyCg29t7UgN1LQvbpRj0VuOQcN0qQsg-g,8572
 super_gradients/training/datasets/segmentation_datasets/supervisely_persons_segmentation.py,sha256=rG5w5hu0hqjzhhMutygfF9zegTM4nbUU-89St1F6Rh0,3062
 super_gradients/training/exceptions/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/training/exceptions/dataset_exceptions.py,sha256=csxJGdEunAi7XZAryqelr0NiZN5d4MxPFbZXklPyoDU,1761
 super_gradients/training/exceptions/kd_trainer_exceptions.py,sha256=KD3rgit7YCxwoQPK7aamFVpOLEHhbLaQI8NsqIoVSFQ,2826
 super_gradients/training/exceptions/loss_exceptions.py,sha256=IOw4_QUfupjz1JkJXLQ_gGfzE60f5v7KInbAGw_IeA8,946
 super_gradients/training/exceptions/sg_trainer_exceptions.py,sha256=cGdofjAzqQmqH5QKpQP4-25JAIbakgQ9jv8uHTFS5bo,1268
 super_gradients/training/kd_trainer/__init__.py,sha256=Ah4RhtFt2KzmN41c815uedwo7CyfBlX1zusR1w2LTEU,132
 super_gradients/training/kd_trainer/kd_trainer.py,sha256=DiobuDsXfaX4wY1Lj91H8opxlCFVDbgzsRgXfwnUu0Q,16582
 super_gradients/training/legacy/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/training/legacy/utils.py,sha256=30Kcx8FOBARF_9y4K9Tue8aLUsv7HS0OrnIHL9-TV0Y,4198
-super_gradients/training/losses/__init__.py,sha256=FQs7jZgVyXfS26m4P__S47ybTUAfJuQq3ep0CdEJBlk,1476
+super_gradients/training/losses/__init__.py,sha256=ZH-dcE3zjpnMBj3_MOFx4DlYFmP_EEcLcPois6Krxiw,1570
 super_gradients/training/losses/all_losses.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/training/losses/bce_dice_loss.py,sha256=uBqTiQDgBCzd62lcZN_fLEmPOyuCbh9r6BYLlFiCPns,1219
 super_gradients/training/losses/bce_loss.py,sha256=F7oXzO08RJVjVfglKszaJ3j3CaqO2T6tVaSBdCgUFpw,419
 super_gradients/training/losses/cwd_loss.py,sha256=1jO8qdoGd9NKdZbWvc-2hAuN5Cn9U8Vk-3rIQt2bGj4,2374
 super_gradients/training/losses/ddrnet_loss.py,sha256=tfSfllVAW9HoPq0W3vbFEH3taznQR1WCpwaXKo33XLg,2525
-super_gradients/training/losses/dekr_loss.py,sha256=SBDKparvpTGysGkWUY0346aN-IJAag_EiVgIlrF2GBQ,3377
+super_gradients/training/losses/dekr_loss.py,sha256=6ETx8SIQFew5r96iLPEMqiFmki4IoM2HLlZ3VE8_hZ8,4038
 super_gradients/training/losses/dice_ce_edge_loss.py,sha256=1TM7s822Ik4IkKT27U4VCd8lVwoy3ClemCFpktxgx04,5618
 super_gradients/training/losses/dice_loss.py,sha256=hcVfl6Jrf0SKTDUf8dEWD15np99XU_I9yv9rR7G142I,5208
 super_gradients/training/losses/focal_loss.py,sha256=-mrmypTdwa5XcSCas-4Hk2wsc_oIaJjvhqY6FHyJ0Go,1214
 super_gradients/training/losses/iou_loss.py,sha256=ON_fJAatqVH4_XVNCrSd9gLNkYlPLEhizUPaJ9jwvT8,5051
 super_gradients/training/losses/kd_losses.py,sha256=-CGP7dWa1B-Ni2MnCQQLARRWxg5ajIUay81xQag-ZUI,2176
 super_gradients/training/losses/label_smoothing_cross_entropy_loss.py,sha256=74uR2HNtiC7h59ywLCjb1NL_3DPtLuNHx3fcxHXGLcs,4177
 super_gradients/training/losses/loss_utils.py,sha256=E23MWbrXOsyF-DexK-tnCB2XyMajI0LHhtPXX9t1FT0,550
-super_gradients/training/losses/mask_loss.py,sha256=Co9_ugt0A3422AJX8PgYdVgcbt-BRAFFhN_tDkenPnE,3854
+super_gradients/training/losses/mask_loss.py,sha256=w7kxBZGHAXp3y-EB5FE6RKE1slxnYSvfIWpNJOQP1lg,4004
 super_gradients/training/losses/ohem_ce_loss.py,sha256=g-6Sltb2N_RBLyuWLBfFOWAQWeq7wrsMydoh9zOZX5w,4129
 super_gradients/training/losses/ppyolo_loss.py,sha256=ZryjBfWsxxUPhmflYFfCh_Eq_DW68h0aD8hiR68ZGdA,41319
 super_gradients/training/losses/r_squared_loss.py,sha256=O1YCoeAwHTNNU2-qTLXlqE-hS2rro0DYaXkgtoDPmRA,1010
+super_gradients/training/losses/rescoring_loss.py,sha256=tmm3kNdBFRoEITEugq2wCW7EddXxBTQluTZqpr-SKqE,665
 super_gradients/training/losses/seg_kd_loss.py,sha256=IDUfzdaBpaOyhQFRSa4OZdmg_KYF2Mf1Xb65P6Qogjk,3453
 super_gradients/training/losses/shelfnet_ohem_loss.py,sha256=Qvova3DBVFpVjpho6Er79OSR61Jf_15yB0rU6L4ttM8,1650
 super_gradients/training/losses/shelfnet_semantic_encoding_loss.py,sha256=o9kw_HPv8QZltQrVOJLdo4Q2G57lmxKsPGZySj5M7SA,1949
 super_gradients/training/losses/ssd_loss.py,sha256=Cou0Bqg0CzPq-d2zLocW7BkhKNB6xOq4FBJjk7cGlsc,8794
 super_gradients/training/losses/stdc_loss.py,sha256=l0TGotIYU3Ka4YnEl0xY1xtWOpZ5PC_8hOlvFUqjCyo,9721
 super_gradients/training/losses/structure_loss.py,sha256=w42pFyv69m7zrbnymPHFgOMvA30esbvn5FrGjWMG9F0,5771
 super_gradients/training/losses/yolox_loss.py,sha256=YvVIYTN6nl1PW5rH72u11O3gYVl8OMFbdeoFkk_mM2M,50149
 super_gradients/training/metrics/__init__.py,sha256=_EHNYpE89jPWTWQsODGYnzQEIlefbh5cvfdOIbWsGpU,1052
 super_gradients/training/metrics/all_metrics.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/training/metrics/classification_metrics.py,sha256=Zopby8WBumdoJxZLJv5YgL7W_ZQODN4hKs55UJKO_H0,3262
 super_gradients/training/metrics/detection_metrics.py,sha256=XXneeuIzFCMwQfiGQcZZCN9cWhD6v3Cj_25HJTZ93nE,10741
 super_gradients/training/metrics/metric_utils.py,sha256=WT1TmuARbVKDLhw4Z1rJt38JM6jnSLAqO6gJa8rKWWY,3973
-super_gradients/training/metrics/pose_estimation_metrics.py,sha256=rw2gFnRSe1tET_TD4rdvt-8DWAvfSoAZwTaT5FZY_og,15346
-super_gradients/training/metrics/pose_estimation_utils.py,sha256=aOv42gu29NiWLihv6kmDBoFBXf0heVUsICF75dmM0l4,11454
+super_gradients/training/metrics/pose_estimation_metrics.py,sha256=SVsug8LaLfrDg7lX04MJnwqNe0Ym3z0V8QhHoDe1roQ,15404
+super_gradients/training/metrics/pose_estimation_utils.py,sha256=GZnpT--sJUmdwmPPtS_JVslNp4mEx-G0p71N00OpiR0,11536
 super_gradients/training/metrics/segmentation_metrics.py,sha256=B24ivTj53cF2COHeyDutxGohDLYcFT_eiKEqXpjDMXk,11935
-super_gradients/training/models/__init__.py,sha256=fz3k7vfa380OiiUMDnP9RA1XrAAOqU9ZWOmHGfg-3uA,8617
+super_gradients/training/models/__init__.py,sha256=ikB1pTl2acFGlntQk8AoTluVEQlZl4B5oOARA6htfn0,11245
 super_gradients/training/models/arch_params_factory.py,sha256=ufy6mCMPUm1b9s3wm-AVMIbX2irytPoZpeXELgtCROs,1226
-super_gradients/training/models/conversion.py,sha256=kucMPr5HGUVn_xL06BaQU7vXzcgvUaqjZF5jiGgupqE,7060
-super_gradients/training/models/model_factory.py,sha256=z2vsf1_zjK2wgWYimHxRxA-bpOHG3ZQx2bC1o0Nhz6s,11875
-super_gradients/training/models/prediction_results.py,sha256=YX2P0ENHNZODBQRKN-GwrszMn3tD1C-DFFIlX5PlT2s,10986
+super_gradients/training/models/conversion.py,sha256=p5b6ioRN749Z5GlJE8azAjzlUMMv-Uc72VKRYgDGo44,12587
+super_gradients/training/models/model_factory.py,sha256=BJzz9K4rhFrmU7O0roix_0_VLbGuX3aQRqfrfqdgd48,11887
+super_gradients/training/models/prediction_results.py,sha256=TDsTihNB5pJgk0bTbvOo4cWNc4tkprtc_jwTr3SdK9Y,10997
 super_gradients/training/models/predictions.py,sha256=-i4fUfLThPPTpSPiyFj-3TS_MRQWwXwQm5QZG1GD754,2054
 super_gradients/training/models/results.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/training/models/sg_module.py,sha256=JalNA0oIrW5IqV6Fl-SkAaq1qmcdLcAS8jx9QC84zMk,2998
 super_gradients/training/models/classification_models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/training/models/classification_models/beit.py,sha256=kAq50cBeBteSF3uE3SW4TwYqfVn6edxPNXQEvOXc1Xg,20025
 super_gradients/training/models/classification_models/densenet.py,sha256=kDFzSB95Zk9OES501IiAyZmUlOnT03M3BEDaxlFONjM,7472
 super_gradients/training/models/classification_models/dpn.py,sha256=B5wPjPhPGp2PhTRxbC3w4VheCqVVs_8s9swqtwWnNKQ,3707
@@ -432,126 +441,127 @@
 super_gradients/training/models/classification_models/mobilenet.py,sha256=JuABaCD_b6_Sh1EzigrBKqOniTTnI9RQ-a1V_YGaS6g,2407
 super_gradients/training/models/classification_models/mobilenetv2.py,sha256=V8FF_9Ibrn9LCf_4ybvQVKr5wVs1LEhpbXOff_XE0pY,9472
 super_gradients/training/models/classification_models/mobilenetv3.py,sha256=2aVzTJOufcdqthtSbjVHE7ViT3iaZcvvwTE9l-GiiKA,8696
 super_gradients/training/models/classification_models/pnasnet.py,sha256=DAo76uXefiCtOUTJ8uiuwAKSDN0nasSSOsCHg-sCkP0,4339
 super_gradients/training/models/classification_models/preact_resnet.py,sha256=24X4Zz00jj3Tj_l3BlLZOl-Z-dLJQ17mf7WKcpYcMtw,4209
 super_gradients/training/models/classification_models/regnet.py,sha256=TqBLs0lkE8yot9CEwtus16KPRHwn5X-HToqF9UGfU3A,13599
 super_gradients/training/models/classification_models/repvgg.py,sha256=gh9vB8y6ZUF8t-dUzxjy5_vpL8RMy6NbzYAYppL4ZoA,7924
-super_gradients/training/models/classification_models/resnet.py,sha256=_P09wEFC_MPfTaVpXFGhjvoVhmoN3iDkSE5T5NVpTTQ,15025
+super_gradients/training/models/classification_models/resnet.py,sha256=nT1IgjRKRPibtIvyJSePYRWLd9esf-cPmP1HuYvIIGU,15067
 super_gradients/training/models/classification_models/resnext.py,sha256=oK78roHfDVm0dZA88ZaLgx8ml9tQkvwU95kRGtfsyGI,6294
 super_gradients/training/models/classification_models/senet.py,sha256=QypzG-XPOvY7HzannhLaT2wtyDeLhT5PZReopJRqgAA,4134
 super_gradients/training/models/classification_models/shufflenet.py,sha256=-57ZOa75ul4eEUMi3fnNbEff2AJGCXJaXQ9npLzETa4,3660
 super_gradients/training/models/classification_models/shufflenetv2.py,sha256=hHMYew6ET-QV8bYhwyCfCoXwIGn1uAJjSyQ9F6EJ9Kw,9768
 super_gradients/training/models/classification_models/vgg.py,sha256=byU29VjwL79efNtIC_ETLXhBLSe8qn_4Wm2RJ4BQYlo,1538
 super_gradients/training/models/classification_models/vit.py,sha256=NwtBiuhcO8dFTXwRb7h66phGDyrQuztdAM_nO5--1UA,9210
 super_gradients/training/models/detection_models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/training/models/detection_models/csp_darknet53.py,sha256=4EIj_ptbYiRu1hNYDPut9cQcUwetuVplpilj4sQHkpk,9130
 super_gradients/training/models/detection_models/csp_resnet.py,sha256=OVL-DXEWj7e5B873jujeKxYvhs7Nhy6ViXOcLDHr49E,9814
-super_gradients/training/models/detection_models/customizable_detector.py,sha256=WuI9niU0ndl41fFA4vYeAcPtrCLgo52vZZan86pZmfE,9120
+super_gradients/training/models/detection_models/customizable_detector.py,sha256=MaE05_09QYoCGFJjitsqqxkSTrIxidAHgk2eqgCkc9o,9986
 super_gradients/training/models/detection_models/darknet53.py,sha256=FBFqJjU01A1l94HW7u7gCBmnRhSUvRVjlXZCsqyR4X8,4746
 super_gradients/training/models/detection_models/ssd.py,sha256=wvl6t3ltL6y5tjwqiFzBl8KmkwBOyUh07VS_7yVDfjs,2315
-super_gradients/training/models/detection_models/yolo_base.py,sha256=8HlHamlhgCaj0kstQfzs87D4WsZ81VtspGwEvMjOmHw,29459
+super_gradients/training/models/detection_models/yolo_base.py,sha256=Uy0RPUc-8sQBRXdL4SANIJEkKu08awHLr8SWRRH-laQ,30262
 super_gradients/training/models/detection_models/yolox.py,sha256=Wjz2H7NwX3j_YkUzLWMSmcDbnEqee59dCXLrd4jRJ-Q,2459
 super_gradients/training/models/detection_models/pp_yolo_e/__init__.py,sha256=kdGGMgi8qmk8vjKKGVk5Ap46e1yjdNmtdQFALb8eiFo,251
 super_gradients/training/models/detection_models/pp_yolo_e/pan.py,sha256=zndJicizLwqjLdAtfWsKd2GnuPv2IoTf4YZW3wcjV1U,7000
 super_gradients/training/models/detection_models/pp_yolo_e/post_prediction_callback.py,sha256=D4V9FAX5_VoxoPcwbuvYDtxaTfPRxFfvM5Ds0frO6js,3487
-super_gradients/training/models/detection_models/pp_yolo_e/pp_yolo_e.py,sha256=5tD_49PK3Ll30jlcrB7YQJ1QtP8HHCoGxoKkZN5Kx1w,8243
+super_gradients/training/models/detection_models/pp_yolo_e/pp_yolo_e.py,sha256=qr__SoXa4QNtBpX0x40byPmKzvTcygdFPI0pYMqpuD8,9023
 super_gradients/training/models/detection_models/pp_yolo_e/pp_yolo_head.py,sha256=lSKZgvbXW2sD0Kd6ImzeOLN7d-kEiBjlB8dDsWc4cKM,12397
 super_gradients/training/models/detection_models/yolo_nas/__init__.py,sha256=TJ9gQeZO8gmsZm0K-hyGxXyIZA8fwYuEaDheRMbXLUk,756
 super_gradients/training/models/detection_models/yolo_nas/dfl_heads.py,sha256=P0TqYiqLgpQpJcaMeGIkT_A9jZrikQ6pVwxzzP_iTlI,12084
 super_gradients/training/models/detection_models/yolo_nas/panneck.py,sha256=qt0ChEAfmYU7Yc5Om7qQW4JMpRVQhMYW9hb-bLWsx2Q,2646
-super_gradients/training/models/detection_models/yolo_nas/yolo_nas_variants.py,sha256=eZWuODf8QttWJAR_WYyH9j7GjTzoR6jpC-24Pa_QZaw,4124
+super_gradients/training/models/detection_models/yolo_nas/yolo_nas_variants.py,sha256=ZiIarpR5IavXvR7DgrFwzRD1bwx3U_qX7yvq5SB_RPs,4166
 super_gradients/training/models/detection_models/yolo_nas/yolo_stages.py,sha256=yEPlfJoqCAHtFhKebaj89vIt2DMjM5VHg5zqaiX6-bo,13329
 super_gradients/training/models/kd_modules/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/training/models/kd_modules/kd_module.py,sha256=urOyHbsubq615UiGJo4-CAFpKvdKxHLrTFMzp1TlM5c,3553
-super_gradients/training/models/pose_estimation_models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-super_gradients/training/models/pose_estimation_models/dekr_hrnet.py,sha256=1WeqAspQseBaECT42iGbKnVfFJ2hHPx-63eublI_dgQ,21231
-super_gradients/training/models/pose_estimation_models/pose_ddrnet39.py,sha256=vQUuvQO6JDdW4tNKYL7k_iDfRf1h28j7aj-n_Xr0UPo,1294
-super_gradients/training/models/pose_estimation_models/pose_ppyolo.py,sha256=pLLHoTF_V2rJKmJ0gLQmcQC0wt7TSfb9RrFA4VoYSaU,1335
+super_gradients/training/models/pose_estimation_models/__init__.py,sha256=MI9kzASiHp7WNv9_5JT_TdnHWzuYjHYzNlstf4QOv9M,179
+super_gradients/training/models/pose_estimation_models/dekr_hrnet.py,sha256=pNuaQHLz-bR90el2KscdrvOIc1B0DeUsUAA04ivVaso,23096
+super_gradients/training/models/pose_estimation_models/rescoring_net.py,sha256=KcAtuW4AWVNkXme_KYyZrtdM0u4tz63kGcW9R_3Rsxg,4298
 super_gradients/training/models/segmentation_models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/training/models/segmentation_models/common.py,sha256=58mVuAE3Hds_5f_5hr3a-ovHzYoGMslKBlwQRhl_5dY,964
 super_gradients/training/models/segmentation_models/context_modules.py,sha256=CcUiqpDPW2iyBuzzcpFGEYu50slxXenRrKdPVJ-zhTo,5139
-super_gradients/training/models/segmentation_models/ddrnet.py,sha256=ta4b4urUI0zazPNYUKk3p6Rf1sb61H87XSveJPccAa0,27896
+super_gradients/training/models/segmentation_models/ddrnet.py,sha256=3pSTLluvZnR2DMslt4t2GKRnbf2V1uihvdu27Ta-r_g,28514
 super_gradients/training/models/segmentation_models/ddrnet_backbones.py,sha256=tLHTnh590-QIg_Jyw87uLgGPt_yM2djx9pqilaAG7hk,2439
 super_gradients/training/models/segmentation_models/laddernet.py,sha256=aQAwG7h_AinfT6r-LvYqdzkWDzcKV0YqzQMNbRcOMmU,21760
 super_gradients/training/models/segmentation_models/ppliteseg.py,sha256=tuwPCaE8CyDU4OX0SqZyJ4B8JD377rOBC7Tgr8F20Qk,15648
 super_gradients/training/models/segmentation_models/regseg.py,sha256=V-Vc4zZcoigUlFD8-p4K9_p-BLuhYWmrPyZX8di8_QI,14424
 super_gradients/training/models/segmentation_models/segformer.py,sha256=hNSunP6CtOcwxczuwQRQxY1sZdc0R1OnxatCW2aHBPA,20334
 super_gradients/training/models/segmentation_models/segmentation_module.py,sha256=ypc_zQRfeuP6YEoY3Kc-tcRRVLLuOaY0uJuWpQRTzKo,2256
-super_gradients/training/models/segmentation_models/shelfnet.py,sha256=bcSLs0d1ulhjWUbgAtdmG6hR_vN4IXMXCkwK0r2Dp98,24833
-super_gradients/training/models/segmentation_models/stdc.py,sha256=m2oXqSvRV-lM8Rl_51ebP_6xcQt0pX8imkL59nzJp6A,29005
+super_gradients/training/models/segmentation_models/shelfnet.py,sha256=WaN6RmDLv4U2rrGvzZyWgMA4IoM5-mLu6c-Nc3LO_TY,24851
+super_gradients/training/models/segmentation_models/stdc.py,sha256=rph_dQY3M-dvgPPkc7tpVIRC9w0RDZhLv6abDzggPRQ,29091
 super_gradients/training/models/segmentation_models/unet/__init__.py,sha256=WZp8BByl8QZpdPlnLwvW7QF5qfODj_-yo4UbtoScPng,260
 super_gradients/training/models/segmentation_models/unet/unet.py,sha256=x5Zu2Z7rw6i4LXyxcyxfL2uOzt3DuofWo7uKX_utTCw,12324
 super_gradients/training/models/segmentation_models/unet/unet_decoder.py,sha256=nqwXOlJkAddqNHBQOgaBIJQdPExMwNWZQrlEqUMP8ME,10718
 super_gradients/training/models/segmentation_models/unet/unet_encoder.py,sha256=auTtUn6jkKWUOdW_wKvOyKC9DpVSi7Y-LjoZY1POA3g,13292
 super_gradients/training/models/user_models/__init__.py,sha256=WNfXGheDVebPB3XmC9ce-wkyh0qXHRlINW43JIdnY6E,119
 super_gradients/training/pipelines/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-super_gradients/training/pipelines/pipelines.py,sha256=5RBdZVCQkjSeuwyfDmuHccOO5F_R3Hn73Gc8exL9aR4,14562
-super_gradients/training/pre_launch_callbacks/__init__.py,sha256=SZtn0Kq5PJ_GIMfFT5bBb0Pck6r5mAnBAfgpDaX5Cdk,393
-super_gradients/training/pre_launch_callbacks/pre_launch_callbacks.py,sha256=E3UsNalAFR0-7pwga-OjFCTp4m7SuO9BEy04Lwt18kk,13955
+super_gradients/training/pipelines/pipelines.py,sha256=_X3NBJ2xtklz3Wiyjl-rHWNww8Q6vOeMS-n1i0zLG2I,15639
+super_gradients/training/pre_launch_callbacks/__init__.py,sha256=xL5z1cJdr_uGuNyBt8PHiQ8g7lwY3mZyYWwtnspQ-C0,445
+super_gradients/training/pre_launch_callbacks/pre_launch_callbacks.py,sha256=vKkUAaRwsATmFc_B021a_ik3Lf4QO03rd8dphubI0iE,21020
 super_gradients/training/processing/__init__.py,sha256=L_S3KapcujiBTXjHcMZxQz5aCwJM9Xxurbhs08oy0_o,517
 super_gradients/training/processing/processing.py,sha256=xx6q2nO2VXC-FGX4rYVp9Otbipbv43gToYepKe0jQyk,13177
 super_gradients/training/qat_trainer/__init__.py,sha256=GZRdCf6P1Ximp-eoVw8kHv5Zb4AjBqxV0E2NwO1OmNo,98
-super_gradients/training/qat_trainer/qat_trainer.py,sha256=wrdK5ao9S1EJpufOtg_rJjI-qExzlHUa_ybsTNOVdTA,9701
+super_gradients/training/qat_trainer/qat_trainer.py,sha256=MoWilDaeWBj6CRQsmObIaB5K4QHIDA2uyWNgdnfGmW8,608
 super_gradients/training/sg_trainer/__init__.py,sha256=dug-p1erLN2SzYFQytJzPWDLOCmfvE94kFtcFLOTqj0,184
-super_gradients/training/sg_trainer/sg_trainer.py,sha256=22Pvj4ZKntAcC1oU-SKSJAyX7drtf06r1TX6qJ1B0OU,96749
+super_gradients/training/sg_trainer/sg_trainer.py,sha256=4rMNageVk4D3zP67Irl6IUmvBwHDQ7PlaB-qoChwGDM,116430
 super_gradients/training/training_hyperparams/__init__.py,sha256=R5pvZNSQgDNxRp23qAlAAhGdPT7u_e78QiztqQDqosc,1685
 super_gradients/training/training_hyperparams/training_hyperparams.py,sha256=pZIOz9L6vf-tgCMUbvf2WLch1zCCfDevhfYPnL3QR7A,3774
 super_gradients/training/transforms/__init__.py,sha256=SMLfPEp8zqooiV6mB4byOzk5SprUUo77LIUNgTTB7A8,1024
 super_gradients/training/transforms/all_transforms.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/training/transforms/keypoint_transforms.py,sha256=-lTR8tHtWGmK6THZvyI52OpH5yhWXDGJeUJM_FwcZhE,16193
 super_gradients/training/transforms/pipeline_adaptors.py,sha256=ukVHjcx-XaCEGZ3I_afIb9Uj73vwYtkmgrLJw9jr7oU,1134
-super_gradients/training/transforms/transforms.py,sha256=uDbuGhNmEL0Mo_FvO4R9NhUf3nH9yQygGIxSgciqV60,55089
+super_gradients/training/transforms/transforms.py,sha256=nqOwUZzuWhFVLO43e_eBk5m46IFxZHNVshtmhCCpbkM,55587
 super_gradients/training/transforms/utils.py,sha256=WkgT9-2hZm7IBS_HZzy1kOE0EOb-k0t8gypuPhpC5Z4,6048
-super_gradients/training/utils/__init__.py,sha256=hveHoDSb03rQ0jXc0SLWD7Pvwd9gCnaISEgc_oikTOE,1104
+super_gradients/training/utils/__init__.py,sha256=ygVj0ne8ck50XC4PvBrSANZB4QwBBRV6OtNVC_ppsMQ,1179
 super_gradients/training/utils/activations_utils.py,sha256=LNgR7SUWOehjBbvtHvU8PtgazsbxX9ztvIUNAQ4nB64,1673
 super_gradients/training/utils/bbox_utils.py,sha256=tvDIJ5TkShshteJAzXVtQZaZFMtIHrYS98U5bpcc0sU,1111
-super_gradients/training/utils/checkpoint_utils.py,sha256=A3d7dhAhHqwDG_39iK1e4QcWNEfC5k3IFrJWFudIrGo,15315
+super_gradients/training/utils/checkpoint_utils.py,sha256=J4N5jXb37w-JCTGoEYNkx79ZWi5r45KMjHaGYpRrk3U,15712
 super_gradients/training/utils/config_utils.py,sha256=jDS_SaRfIEvAXzPB5ZerzVtKaDxD8mgKesUI4M2ERdo,9794
 super_gradients/training/utils/deprecated_utils.py,sha256=YtKScFu62sn2IDBtzC2cPmdSFQ_UfeQZ3CrPDuOZpO4,1132
-super_gradients/training/utils/detection_utils.py,sha256=heb7irv25BHi8erxfS5msqI9yA_VH28qk1zJa0PMgOA,53278
+super_gradients/training/utils/detection_utils.py,sha256=cAsBoQ5fsCN1hZMBgxs4rG-axC5lp47xdrnoC1PiaJA,53289
 super_gradients/training/utils/distributed_training_utils.py,sha256=1hUkc_OE3CCvBtcWlUsGbB8kmgjAUWtgXFJs9QORX-I,16195
 super_gradients/training/utils/early_stopping.py,sha256=FGv-bFT6N1WrtEmZ2Q0xmmijmOI_IKoTvxQcua0LK9g,6352
 super_gradients/training/utils/ema.py,sha256=xPjihYYtpKqrOth0KoRyTeFarCTEH-AVnh0J9M767PM,9322
 super_gradients/training/utils/ema_decay_schedules.py,sha256=lV9zLoVvfPPWJajPpNBnkn8d5ahLJIAjHtv3rZsDU1E,2610
 super_gradients/training/utils/export_utils.py,sha256=Ci9yz8OiK0oVEBHaG74-YuPqBANciWpFf17w-IVYvRc,1072
 super_gradients/training/utils/get_model_stats.py,sha256=nMKVdVxsLPSKDXD7qnTWk60f0B3F1-Ct-XdZchFbsJM,7508
 super_gradients/training/utils/kd_trainer_utils.py,sha256=j-RWPU7_0rKX-4Cf9RiyGk3GuH6j7_cGeBLKYhuXYOk,771
 super_gradients/training/utils/load_image.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/training/utils/optimizer_utils.py,sha256=tB-M7Iv9SqRMyzTpk_5tL1gNTk7tpeVPRyEhI_5tqY0,5827
 super_gradients/training/utils/regularization_utils.py,sha256=apNkV4g-9-mA0m6aSGVz6M5Y6MisplfmcdkYwDnFIyA,839
 super_gradients/training/utils/segmentation_utils.py,sha256=otlxMRGq63cNsSj39lTQtNLyDvM9UrU7LVPlHHYxbRI,10388
 super_gradients/training/utils/sg_trainer_utils.py,sha256=wnH6njXa_0eENF9QpznsYi81lfUrOLzbBqaOVAbSd50,19625
 super_gradients/training/utils/ssd_utils.py,sha256=n31g0sdpHM96PWJGrJlXK5EGMb0t1nRgAE5sI17XXM4,6272
-super_gradients/training/utils/utils.py,sha256=EWcR6vxmbKJNAVLrO4hpJhhaZHvquDdEX7gEHKCepcw,18273
+super_gradients/training/utils/utils.py,sha256=LLQ_W5d3sNaUY01q92-C368SUPBMwvv_CARpCSjile8,20438
 super_gradients/training/utils/version_utils.py,sha256=lzIg-vB-ok6tF2HfzFNkIEpq1XB3_cVqoaaNikGR1PE,303
-super_gradients/training/utils/weight_averaging_utils.py,sha256=a9rw30CWTfp-QCDysObSC-yd-W_XQYJeX12SfvyH8TQ,6209
+super_gradients/training/utils/weight_averaging_utils.py,sha256=3e5RpP8vasmEiY1ZJP5stbSFEbq97wbRJj89rwB4dfE,5687
 super_gradients/training/utils/callbacks/__init__.py,sha256=IW4hEmiLvmSqcvYMQn6D0e8qcI-avUnHUcMI8Mv9gvg,2030
 super_gradients/training/utils/callbacks/all_callbacks.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/training/utils/callbacks/base_callbacks.py,sha256=pCMNK9iUQm8jqSAm5elZrG9Oy3AYD62L-_qj8e9du8U,20126
-super_gradients/training/utils/callbacks/callbacks.py,sha256=UCHS-mkHzEqqoORL2OiVa23Zab1inMLfytJnnioOkkE,32630
+super_gradients/training/utils/callbacks/callbacks.py,sha256=0jrto6bqX5yMxb92mhHWsAplhtjXGRiJRgkRVkYK-zc,33409
 super_gradients/training/utils/callbacks/ppyoloe_switch_callback.py,sha256=7-EaXO3ipczQw9H6NIGqZ-3cR3n-ZN6oAEcnCsv-VtE,1169
 super_gradients/training/utils/media/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/training/utils/media/image.py,sha256=CZ6_K-yifXXNqGe3grp1e5hl-Ug_0lFUGH5CIm_1Glo,5880
 super_gradients/training/utils/media/stream.py,sha256=wgVafnzRXnZvSxaiquNXUC6PqSMlLI4A6YS6_b4A04Y,4046
 super_gradients/training/utils/media/video.py,sha256=DC9xdQX5g2JCWalBeHAGh3VWtvBRvxOs3dIgIuqURtw,6926
 super_gradients/training/utils/optimizers/__init__.py,sha256=Z-kZTiqwHe-KFYP0BTFsX0TNms8-CfRrc6iKEfewopM,396
+super_gradients/training/utils/optimizers/all_optimizers.py,sha256=9oPneh_UFmDWb-NWBKWa3X7EaYTVN8KYxc_LE7D2n94,422
 super_gradients/training/utils/optimizers/lamb.py,sha256=zdvmfKHGen7_rwMohoEs6DOSDEH95ELFCKezD1fN1v0,9760
 super_gradients/training/utils/optimizers/lion.py,sha256=ivMkwLg0vpOyfD4h226wScYXYDwTdCh0o_zkOeyrdcs,3008
 super_gradients/training/utils/optimizers/rmsprop_tf.py,sha256=5gzx0uy3x4c8G8UgfDnOTLjASwT1enBAcfUkgzrOOJU,6834
-super_gradients/training/utils/pose_estimation/__init__.py,sha256=V0xjHNxc1OeJUE2QOTlAV298wmQwgRWwXLx5Pq6p5Gw,213
-super_gradients/training/utils/pose_estimation/dekr_decode_callbacks.py,sha256=1y-85e33A9mKokm4ER_HpwuRqWpbY2pjm6gAjjy4WXc,11167
+super_gradients/training/utils/pose_estimation/__init__.py,sha256=-gXj3fMnEXjfmj_3NCeMtEsddOMSSxVzXWA72Slh5tw,324
+super_gradients/training/utils/pose_estimation/dekr_decode_callbacks.py,sha256=6p4vxEx1mqP_ziGUR22foG1Bb5_9H0P9yFJV97iCLFo,11309
 super_gradients/training/utils/pose_estimation/dekr_visualization_callbacks.py,sha256=HEdNaksgnzoXh1RWRvB5rd_tniZWkk6Ro-6D2-Abv1Q,7140
+super_gradients/training/utils/pose_estimation/rescoring_callback.py,sha256=kwWbyJ6C6hY8G072gSYqUh0uGB7K3bM-heIDwIU0KyA,920
 super_gradients/training/utils/quantization/__init__.py,sha256=FsLDGZR4MT_1tTIcnyOhIqUTfCf178tU7Y72och-Fws,387
 super_gradients/training/utils/quantization/calibrator.py,sha256=vfXnyPxLdHjk5e5CF3-lBwofRDjX-ZCyDaRreuu6_h4,6271
 super_gradients/training/utils/quantization/core.py,sha256=CYykLasziH9YT0h_utxWj6WZ6tXi4KUSKaiBf1N2YZM,8417
-super_gradients/training/utils/quantization/export.py,sha256=GW22x2GMQJMEp1iZcJ63qcxev6Etay_FI6taKbJpmv8,2196
+super_gradients/training/utils/quantization/export.py,sha256=EpP1RQ--B2YnleMv54cpGURpv_MpbOx-CKPjfspSVF0,2504
 super_gradients/training/utils/quantization/selective_quantization_utils.py,sha256=hQ8uZliyAK21pguj0aSybxINffXrj0R2YCHCWIRV7Z4,17062
 super_gradients/training/utils/visualization/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/training/utils/visualization/detection.py,sha256=348rm6aggC_RLn9Zsnr9FC0AJu5zieHVhTzQGJs6sfk,1698
 super_gradients/training/utils/visualization/utils.py,sha256=LXh2fmdauApUJEn62a0yEXwKQ6G1ySlWvqkK9Ap8ybU,2847
-super_gradients-3.1.1.dist-info/LICENSE.YOLONAS.md,sha256=mPgPXAN-RoGSYLzisdBu2uJx2HyJHd8enqEUlpO5mmQ,2218
-super_gradients-3.1.1.dist-info/LICENSE.md,sha256=jWCBQN-JmCX0hwvn3MqItDj18W3riP4zda31ncMkcfA,11341
-super_gradients-3.1.1.dist-info/METADATA,sha256=APFfugaXHwe_gu19_wXwrq5gFJ2kO015ihom34VXe9c,36095
-super_gradients-3.1.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-super_gradients-3.1.1.dist-info/top_level.txt,sha256=k8ZbuOXtbEm0O2O3MCG-rnUyDilV2FYLXMbeXUspUXI,16
-super_gradients-3.1.1.dist-info/RECORD,,
+super_gradients-3.1.2.dist-info/LICENSE.YOLONAS.md,sha256=mPgPXAN-RoGSYLzisdBu2uJx2HyJHd8enqEUlpO5mmQ,2218
+super_gradients-3.1.2.dist-info/LICENSE.md,sha256=jWCBQN-JmCX0hwvn3MqItDj18W3riP4zda31ncMkcfA,11341
+super_gradients-3.1.2.dist-info/METADATA,sha256=1E7tnIGPTD38zi6t2ghWa6xHwXZ9_oUWEjvtANEILkQ,35552
+super_gradients-3.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+super_gradients-3.1.2.dist-info/top_level.txt,sha256=k8ZbuOXtbEm0O2O3MCG-rnUyDilV2FYLXMbeXUspUXI,16
+super_gradients-3.1.2.dist-info/RECORD,,
```

