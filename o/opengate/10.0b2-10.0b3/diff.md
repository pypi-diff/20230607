# Comparing `tmp/opengate-10.0b2.tar.gz` & `tmp/opengate-10.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opengate-10.0b2.tar", last modified: Thu Mar 23 16:18:35 2023, max compression
+gzip compressed data, was "opengate-10.0b3.tar", last modified: Wed Jun  7 14:50:38 2023, max compression
```

## Comparing `opengate-10.0b2.tar` & `opengate-10.0b3.tar`

### file list

```diff
@@ -1,343 +1,349 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:18:35.478400 opengate-10.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-03-23 16:16:43.000000 opengate-10.0b2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-03-23 16:16:43.000000 opengate-10.0b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-03-23 16:18:35.478400 opengate-10.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-03-23 16:16:43.000000 opengate-10.0b2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-23 16:16:43.000000 opengate-10.0b2/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:18:35.442400 opengate-10.0b2/core/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:18:35.442400 opengate-10.0b2/core/external/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:18:35.450400 opengate-10.0b2/core/external/fmt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:18:35.450400 opengate-10.0b2/core/external/fmt/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-03-23 16:16:50.000000 opengate-10.0b2/core/external/fmt/.github/issue_template.md
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-03-23 16:16:50.000000 opengate-10.0b2/core/external/fmt/.github/pull_request_template.md
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-03-23 16:16:50.000000 opengate-10.0b2/core/external/fmt/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:18:35.442400 opengate-10.0b2/core/external/fmt/support/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:18:35.450400 opengate-10.0b2/core/external/fmt/support/bazel/
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-03-23 16:16:50.000000 opengate-10.0b2/core/external/fmt/support/bazel/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:18:35.442400 opengate-10.0b2/core/external/fmt/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:18:35.450400 opengate-10.0b2/core/external/fmt/test/fuzzing/
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-03-23 16:16:50.000000 opengate-10.0b2/core/external/fmt/test/fuzzing/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:18:35.442400 opengate-10.0b2/core/external/pybind11/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:18:35.450400 opengate-10.0b2/core/external/pybind11/.github/
--rw-r--r--   0 runner    (1001) docker     (123)    15284 2023-03-23 16:16:50.000000 opengate-10.0b2/core/external/pybind11/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-03-23 16:16:50.000000 opengate-10.0b2/core/external/pybind11/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:18:35.442400 opengate-10.0b2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:18:35.454400 opengate-10.0b2/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)    21081 2023-03-23 16:16:43.000000 opengate-10.0b2/docs/source/developer_guide.md
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-03-23 16:16:43.000000 opengate-10.0b2/docs/source/user_guide.md
--rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-03-23 16:16:43.000000 opengate-10.0b2/docs/source/user_guide_1_intro.md
--rw-r--r--   0 runner    (1001) docker     (123)     9818 2023-03-23 16:16:43.000000 opengate-10.0b2/docs/source/user_guide_2_0_simulation.md
--rw-r--r--   0 runner    (1001) docker     (123)    11717 2023-03-23 16:16:43.000000 opengate-10.0b2/docs/source/user_guide_2_1_volumes.md
--rw-r--r--   0 runner    (1001) docker     (123)     7382 2023-03-23 16:16:43.000000 opengate-10.0b2/docs/source/user_guide_2_2_sources.md
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-03-23 16:16:43.000000 opengate-10.0b2/docs/source/user_guide_2_3_physics.md
--rw-r--r--   0 runner    (1001) docker     (123)    12003 2023-03-23 16:16:43.000000 opengate-10.0b2/docs/source/user_guide_2_4_actors.md
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-03-23 16:16:43.000000 opengate-10.0b2/docs/source/user_guide_3_addons.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:18:35.454400 opengate-10.0b2/opengate/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/EngineBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/ExceptionHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/RunAction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6260 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/Simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)    13235 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/SimulationEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/SimulationOutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/SimulationUserInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/UIsessionSilent.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/UIsessionVerbose.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/UserElement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/UserInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:18:35.458400 opengate-10.0b2/opengate/actor/
--rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/actor/ARFActor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/actor/ARFTrainingDatasetActor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/actor/ActionEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/actor/ActorBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/actor/ActorEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/actor/ActorManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/actor/DigitizerAdderActor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/actor/DigitizerBlurringActor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/actor/DigitizerEnergyWindowsActor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/actor/DigitizerHitsCollectionActor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/actor/DigitizerProjectionActor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/actor/DigitizerReadoutActor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/actor/DigitizerSpatialBlurringActor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10976 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/actor/DoseActor.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/actor/FilterBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/actor/FilterManager.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/actor/KineticEnergyFilter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10241 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/actor/LETActor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/actor/MotionVolumeActor.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/actor/ParticleFilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/actor/PhaseSpaceActor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/actor/SimulationStatisticsActor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/actor/SourceInfoActor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/actor/TestActor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/actor/TrackCreatorProcessFilter.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/actor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/actor/helpers_actor.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/actor/helpers_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:18:35.458400 opengate-10.0b2/opengate/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/bin/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1320 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/bin/dose_rate
--rwxr-xr-x   0 runner    (1001) docker     (123)      107 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/bin/opengate_info
--rwxr-xr-x   0 runner    (1001) docker     (123)     3761 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/bin/opengate_tests
--rwxr-xr-x   0 runner    (1001) docker     (123)     1539 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/bin/opengate_tests_utils
--rwxr-xr-x   0 runner    (1001) docker     (123)      999 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/bin/opengate_user_info
--rwxr-xr-x   0 runner    (1001) docker     (123)     1633 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/bin/opengate_visu
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/bin/readme.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     1155 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/bin/split_spect_projections
--rwxr-xr-x   0 runner    (1001) docker     (123)     1571 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/bin/voxelize_iec_phantom
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:18:35.458400 opengate-10.0b2/opengate/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)    26202 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/contrib/GateMaterials.db
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/contrib/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3166 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/contrib/dose_rate_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/contrib/dose_rate_test1.json
--rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/contrib/linac_elekta_synergy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/contrib/linac_elekta_synergy_materials.db
--rw-r--r--   0 runner    (1001) docker     (123)    11174 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/contrib/pet_philips_vereos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/contrib/pet_siemens_biograph.py
--rw-r--r--   0 runner    (1001) docker     (123)    22685 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/contrib/pet_siemens_biograph_materials.db
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/contrib/phantom_necr.py
--rw-r--r--   0 runner    (1001) docker     (123)    22092 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/contrib/phantom_nema_iec_body.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/contrib/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)    14248 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/contrib/spect_ge_nm670.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/contrib/spect_ge_nm670_materials.db
--rwxr-xr-x   0 runner    (1001) docker     (123)     3654 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/contrib/spect_ideal_timed_reconstruction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:18:35.462400 opengate-10.0b2/opengate/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/geometry/BooleanVolume.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/geometry/BoxVolume.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/geometry/ConsVolume.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/geometry/ElementBuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/geometry/HexagonVolume.py
--rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/geometry/ImageVolume.py
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/geometry/MaterialBuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/geometry/MaterialDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/geometry/PolyhedraVolume.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/geometry/RepeatParametrisedVolume.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/geometry/SolidBuilderBase.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/geometry/SphereVolume.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/geometry/TrapVolume.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/geometry/TrdVolume.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/geometry/TubsVolume.py
--rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/geometry/VolumeBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/geometry/VolumeEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/geometry/VolumeManager.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/geometry/helpers_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    10086 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/geometry/helpers_materials.py
--rw-r--r--   0 runner    (1001) docker     (123)     8987 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/helpers_element.py
--rw-r--r--   0 runner    (1001) docker     (123)    13179 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/helpers_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/helpers_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/helpers_run_timing.py
--rw-r--r--   0 runner    (1001) docker     (123)    35611 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/helpers_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/helpers_tests_root.py
--rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/helpers_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:18:35.462400 opengate-10.0b2/opengate/mac/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/mac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/mac/default_visu_commands.mac
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/mac/default_visu_commands_gdml.mac
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/mac/default_visu_commands_vrml.mac
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:18:35.462400 opengate-10.0b2/opengate/physics/
--rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/physics/PhysicsEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/physics/PhysicsManager.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/physics/PhysicsUserInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/physics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/physics/helpers_physics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:18:35.462400 opengate-10.0b2/opengate/source/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/source/GANPairsSource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/source/GANSource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/source/GANSourceConditionalGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/source/GANSourceConditionalPairsGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/source/GANSourceDefaultGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/source/GANSourceDefaultPairsGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7945 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/source/GenericSource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/source/PencilBeamSource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/source/SourceBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/source/SourceEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/source/SourceManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/source/VoxelizedSourceConditionGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/source/VoxelizedSourcePDFSampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/source/VoxelsSource.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/source/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:18:35.462400 opengate-10.0b2/opengate/source/beta_plus_spectra/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:18:35.462400 opengate-10.0b2/opengate/source/beta_plus_spectra/C11/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/source/beta_plus_spectra/C11/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14172 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/source/beta_plus_spectra/C11/beta+_C11_tot.bs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:18:35.462400 opengate-10.0b2/opengate/source/beta_plus_spectra/F18/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/source/beta_plus_spectra/F18/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14004 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/source/beta_plus_spectra/F18/beta+_F18_tot.bs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:18:35.462400 opengate-10.0b2/opengate/source/beta_plus_spectra/Ga68/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/source/beta_plus_spectra/Ga68/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17616 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/source/beta_plus_spectra/Ga68/beta+_Ga68_tot.bs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:18:35.462400 opengate-10.0b2/opengate/source/beta_plus_spectra/N13/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/source/beta_plus_spectra/N13/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17490 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/source/beta_plus_spectra/N13/beta+_N13_tot.bs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:18:35.466400 opengate-10.0b2/opengate/source/beta_plus_spectra/Na22/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/source/beta_plus_spectra/Na22/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16945 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/source/beta_plus_spectra/Na22/beta+_Na22_tot.bs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:18:35.466400 opengate-10.0b2/opengate/source/beta_plus_spectra/O15/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/source/beta_plus_spectra/O15/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15262 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/source/beta_plus_spectra/O15/beta+_O15_tot.bs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:18:35.466400 opengate-10.0b2/opengate/source/beta_plus_spectra/Rb82/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/source/beta_plus_spectra/Rb82/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15685 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/source/beta_plus_spectra/Rb82/beta+_Rb82_tot.bs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:18:35.466400 opengate-10.0b2/opengate/source/beta_plus_spectra/Zr89/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/source/beta_plus_spectra/Zr89/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13332 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/source/beta_plus_spectra/Zr89/beta+_Zr89_tot.bs
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/source/beta_plus_spectra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/source/helpers_source.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:18:35.466400 opengate-10.0b2/opengate/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-23 16:18:31.000000 opengate-10.0b2/opengate/tests/HEAD
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:18:35.466400 opengate-10.0b2/opengate/tests/log/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/log/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:18:35.466400 opengate-10.0b2/opengate/tests/output/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/output/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:18:35.466400 opengate-10.0b2/opengate/tests/output/output_test035/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/output/output_test035/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:18:35.478400 opengate-10.0b2/opengate/tests/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1851 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test001_G4ThreeVector.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      390 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test002_G4String.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1361 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test003_G4Material.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3918 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test004_simple.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2162 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test004_simple_MT.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1597 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test004_simple_visu.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1640 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test004_simple_visu_gdml.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1702 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test004_simple_visu_vrml.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1599 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test004_simple_visu_wip.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1769 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test004_simulation_stats_actor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1655 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test005_proton.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2520 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test006_runs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4900 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test007_volumes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3262 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test008_dose_actor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6229 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test008_geometry_dose_grid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3038 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test009_voxels.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3764 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test009_voxels_hu.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3928 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test010_generic_source.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3617 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test010_generic_source_confine.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1919 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test011_MT.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2929 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test012_MT_dose_actor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3129 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test013_half_life.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1147 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test013_phys_lists_1.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      893 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test013_phys_lists_2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1178 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test013_phys_lists_3_WIP.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1164 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test013_phys_lists_4.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1162 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test013_phys_lists_5.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test013_phys_lists_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      278 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test014_engine_1.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      454 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test014_engine_2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      324 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test014_engine_3.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      324 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test014_engine_4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test014_engine_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test015_iec_phantom_1.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1654 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test015_iec_phantom_1_visu.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1515 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test015_iec_phantom_2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2269 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test015_iec_phantom_3.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3297 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test015_iec_phantom_4.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3011 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test016_bool_volumes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3322 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test017_repeater.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1715 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test018_pet_WIP.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      173 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test019_linac_phsp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      131 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test019_linac_phsp_MT.py
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test019_linac_phsp_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      404 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test019_linac_phsp_visu.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2931 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test020_profiling.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3607 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test021_voxel_source1.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4291 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test021_voxel_source2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5087 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test021_voxel_source_old_WIP.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4680 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test022_half_life.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      251 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test022_half_life_MT.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3008 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test023_filters.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2520 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test023_filters_iec_phantom.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2482 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test023_filters_material.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1251 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test024_py_actor_WIP.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      193 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test025_hits_collection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      193 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test025_hits_collection_MT.py
--rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test025_hits_collection_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1567 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test026_simple_signal.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4251 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test027_fake_spect_MT.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2255 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test028_ge_nm670_spect_1_colli.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2304 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test028_ge_nm670_spect_1_colli_visu.py
--rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test028_ge_nm670_spect_2_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      422 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test028_ge_nm670_spect_2_hits.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      448 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test028_ge_nm670_spect_2_hits_MT.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      770 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test028_ge_nm670_spect_3_proj.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      590 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test028_ge_nm670_spect_3_proj_MT.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2236 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test028_ge_nm670_spect_3_proj_blur.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      465 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test028_ge_nm670_spect_4_acc_angle_aa_se.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      469 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test028_ge_nm670_spect_4_acc_angle_aa_se_MT.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      493 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test028_ge_nm670_spect_4_acc_angle_aa_ze.py
--rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test028_ge_nm670_spect_4_acc_angle_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      415 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test028_ge_nm670_spect_4_acc_angle_noaa.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1458 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test029_volume_time_rotation_1.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1462 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test029_volume_time_rotation_1_process.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1631 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test029_volume_time_rotation_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test029_volume_time_rotation_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3433 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test030_dose_motion.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5151 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test031_beta+_spectrum.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2683 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test032_create_voxelized_volume.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4226 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test032_voxel_vs_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test033_rotation_spect_aa_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      431 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test033_rotation_spect_aa_se.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      444 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test033_rotation_spect_aa_se_MT.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      431 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test033_rotation_spect_aa_ze.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      482 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test033_rotation_spect_noaa.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3210 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test034_gan_phsp_linac.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1795 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test035_dose_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test036_adder_depth_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      493 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test036_adder_depth_param.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      494 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test036_adder_depth_repeat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      653 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test037_digi_attributes_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test037_pet_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1870 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test037_pet_hits_singles_1.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2004 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test037_pet_hits_singles_1_visu.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2373 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test037_pet_hits_singles_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test037_pet_hits_singles_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      530 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test038_gan_phsp_spect_gan_MT.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2145 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test038_gan_phsp_spect_gan_aa.py
--rw-r--r--   0 runner    (1001) docker     (123)    12933 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test038_gan_phsp_spect_gan_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      598 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test038_gan_phsp_spect_gan_se.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      598 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test038_gan_phsp_spect_gan_ze.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4825 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test038_gan_phsp_spect_training_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      314 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test039_hits_memory_check.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      314 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test039_hits_memory_check_MP_WIP.py
--rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test039_hits_memory_check_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3546 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test040_gan_phsp_pet_aref.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10665 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test040_gan_phsp_pet_gan.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4693 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test040_gan_phsp_pet_training_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3228 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test041_dose_actor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4052 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test042_gauss_gps.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3772 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test043_distances.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3777 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test043_garf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2702 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test043_garf_analog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test043_garf_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3258 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test043_garf_training_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5021 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test044_pbs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5574 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test044_pbs_rot_transl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5114 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test044_pbs_source_to_volume.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5694 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test044_pbs_unFocused.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5258 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test044_pbs_weight.py
--rw-r--r--   0 runner    (1001) docker     (123)    10666 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test045_gan_phsp_pet_gan_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3166 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test045_speedup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2998 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test045_speedup_all.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2152 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test046_rad.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3910 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test047_gan_vox_source_cond.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1359 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test047_voxelization.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1293 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test048_split_spect_projections.py
--rw-r--r--   0 runner    (1001) docker     (123)     5848 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test049_pet_digit_blurring_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1331 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test049_pet_digit_blurring_v1.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1456 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test049_pet_digit_blurring_v2_MT.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2008 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test049_pet_digit_blurring_v3.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2066 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test049_pet_digit_blurring_v4.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5529 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test050_let_actor_letd.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3622 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test051_adder_time_difference.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2663 2023-03-23 16:16:43.000000 opengate-10.0b2/opengate/tests/src/test052_tac_activity_source.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:18:35.454400 opengate-10.0b2/opengate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-03-23 16:18:35.000000 opengate-10.0b2/opengate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12477 2023-03-23 16:18:35.000000 opengate-10.0b2/opengate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 16:18:35.000000 opengate-10.0b2/opengate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-03-23 16:18:35.000000 opengate-10.0b2/opengate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-23 16:18:35.000000 opengate-10.0b2/opengate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 16:18:35.478400 opengate-10.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-03-23 16:16:43.000000 opengate-10.0b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:50:38.941994 opengate-10.0b3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-06-07 14:49:37.000000 opengate-10.0b3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-06-07 14:49:37.000000 opengate-10.0b3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-07 14:49:37.000000 opengate-10.0b3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-06-07 14:50:38.941994 opengate-10.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-07 14:49:37.000000 opengate-10.0b3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-07 14:49:37.000000 opengate-10.0b3/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:50:38.905995 opengate-10.0b3/core/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:50:38.905995 opengate-10.0b3/core/external/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:50:38.913994 opengate-10.0b3/core/external/fmt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:50:38.913994 opengate-10.0b3/core/external/fmt/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-07 14:49:43.000000 opengate-10.0b3/core/external/fmt/.github/issue_template.md
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-07 14:49:43.000000 opengate-10.0b3/core/external/fmt/.github/pull_request_template.md
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-07 14:49:43.000000 opengate-10.0b3/core/external/fmt/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:50:38.905995 opengate-10.0b3/core/external/fmt/support/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:50:38.913994 opengate-10.0b3/core/external/fmt/support/bazel/
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-06-07 14:49:43.000000 opengate-10.0b3/core/external/fmt/support/bazel/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:50:38.905995 opengate-10.0b3/core/external/fmt/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:50:38.913994 opengate-10.0b3/core/external/fmt/test/fuzzing/
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-07 14:49:43.000000 opengate-10.0b3/core/external/fmt/test/fuzzing/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:50:38.905995 opengate-10.0b3/core/external/pybind11/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:50:38.913994 opengate-10.0b3/core/external/pybind11/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)    15284 2023-06-07 14:49:43.000000 opengate-10.0b3/core/external/pybind11/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-07 14:49:43.000000 opengate-10.0b3/core/external/pybind11/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:50:38.905995 opengate-10.0b3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:50:38.917994 opengate-10.0b3/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)    25530 2023-06-07 14:49:37.000000 opengate-10.0b3/docs/source/developer_guide.md
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-07 14:49:37.000000 opengate-10.0b3/docs/source/user_guide.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-06-07 14:49:37.000000 opengate-10.0b3/docs/source/user_guide_1_intro.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9818 2023-06-07 14:49:37.000000 opengate-10.0b3/docs/source/user_guide_2_0_simulation.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11717 2023-06-07 14:49:37.000000 opengate-10.0b3/docs/source/user_guide_2_1_volumes.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-06-07 14:49:37.000000 opengate-10.0b3/docs/source/user_guide_2_2_sources.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-06-07 14:49:37.000000 opengate-10.0b3/docs/source/user_guide_2_3_physics.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12003 2023-06-07 14:49:37.000000 opengate-10.0b3/docs/source/user_guide_2_4_actors.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-07 14:49:37.000000 opengate-10.0b3/docs/source/user_guide_3_addons.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:50:38.917994 opengate-10.0b3/opengate/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/EngineBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/ExceptionHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/RunAction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/Simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13235 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/SimulationEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/SimulationOutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/SimulationUserInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/UIsessionSilent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/UIsessionVerbose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/UserElement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/UserInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:50:38.921995 opengate-10.0b3/opengate/actor/
+-rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/actor/ARFActor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/actor/ARFTrainingDatasetActor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/actor/ActionEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/actor/ActorBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/actor/ActorEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/actor/ActorManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/actor/DigitizerAdderActor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/actor/DigitizerBlurringActor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/actor/DigitizerEnergyWindowsActor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/actor/DigitizerHitsCollectionActor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/actor/DigitizerProjectionActor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/actor/DigitizerReadoutActor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/actor/DigitizerSpatialBlurringActor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10976 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/actor/DoseActor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/actor/FilterBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/actor/FilterManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/actor/KineticEnergyFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10241 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/actor/LETActor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/actor/MotionVolumeActor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/actor/ParticleFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/actor/PhaseSpaceActor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/actor/SimulationStatisticsActor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/actor/SourceInfoActor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/actor/TestActor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/actor/TrackCreatorProcessFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/actor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/actor/helpers_actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/actor/helpers_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:50:38.921995 opengate-10.0b3/opengate/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/bin/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1320 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/bin/dose_rate
+-rwxr-xr-x   0 runner    (1001) docker     (123)      107 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/bin/opengate_info
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4387 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/bin/opengate_tests
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1539 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/bin/opengate_tests_utils
+-rwxr-xr-x   0 runner    (1001) docker     (123)      999 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/bin/opengate_user_info
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1653 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/bin/opengate_visu
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/bin/readme.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1155 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/bin/split_spect_projections
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1571 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/bin/voxelize_iec_phantom
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:50:38.921995 opengate-10.0b3/opengate/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)    26202 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/contrib/GateMaterials.db
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/contrib/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3166 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/contrib/dose_rate_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/contrib/dose_rate_test1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/contrib/linac_elekta_synergy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/contrib/linac_elekta_synergy_materials.db
+-rw-r--r--   0 runner    (1001) docker     (123)    11174 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/contrib/pet_philips_vereos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/contrib/pet_siemens_biograph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22685 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/contrib/pet_siemens_biograph_materials.db
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/contrib/phantom_necr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22092 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/contrib/phantom_nema_iec_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/contrib/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14248 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/contrib/spect_ge_nm670.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/contrib/spect_ge_nm670_materials.db
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3654 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/contrib/spect_ideal_timed_reconstruction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:50:38.925994 opengate-10.0b3/opengate/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/geometry/BooleanVolume.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/geometry/BoxVolume.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/geometry/ConsVolume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/geometry/ElementBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/geometry/HexagonVolume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/geometry/ImageVolume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/geometry/MaterialBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/geometry/MaterialDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/geometry/PolyhedraVolume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/geometry/RepeatParametrisedVolume.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/geometry/SolidBuilderBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/geometry/SphereVolume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/geometry/TrapVolume.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/geometry/TrdVolume.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/geometry/TubsVolume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/geometry/VolumeBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/geometry/VolumeEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/geometry/VolumeManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/geometry/helpers_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10086 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/geometry/helpers_materials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8987 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/helpers_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13179 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/helpers_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/helpers_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/helpers_run_timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35611 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/helpers_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/helpers_tests_root.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/helpers_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:50:38.925994 opengate-10.0b3/opengate/mac/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/mac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/mac/default_visu_commands.mac
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/mac/default_visu_commands_gdml.mac
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/mac/default_visu_commands_vrml.mac
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:50:38.925994 opengate-10.0b3/opengate/physics/
+-rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/physics/PhysicsEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/physics/PhysicsManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/physics/PhysicsUserInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/physics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/physics/helpers_physics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:50:38.925994 opengate-10.0b3/opengate/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/source/GANPairsSource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/source/GANSource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/source/GANSourceConditionalGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/source/GANSourceConditionalPairsGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11083 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/source/GANSourceDefaultGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/source/GANSourceDefaultPairsGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7945 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/source/GenericSource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/source/PencilBeamSource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/source/PhaseSpaceSource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/source/PhaseSpaceSourceGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/source/SourceBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/source/SourceEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/source/SourceManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/source/TemplateSource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/source/VoxelizedSourceConditionGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/source/VoxelizedSourcePDFSampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/source/VoxelsSource.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/source/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:50:38.925994 opengate-10.0b3/opengate/source/beta_plus_spectra/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:50:38.925994 opengate-10.0b3/opengate/source/beta_plus_spectra/C11/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/source/beta_plus_spectra/C11/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14172 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/source/beta_plus_spectra/C11/beta+_C11_tot.bs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:50:38.925994 opengate-10.0b3/opengate/source/beta_plus_spectra/F18/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/source/beta_plus_spectra/F18/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14004 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/source/beta_plus_spectra/F18/beta+_F18_tot.bs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:50:38.925994 opengate-10.0b3/opengate/source/beta_plus_spectra/Ga68/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/source/beta_plus_spectra/Ga68/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17616 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/source/beta_plus_spectra/Ga68/beta+_Ga68_tot.bs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:50:38.925994 opengate-10.0b3/opengate/source/beta_plus_spectra/N13/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/source/beta_plus_spectra/N13/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17490 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/source/beta_plus_spectra/N13/beta+_N13_tot.bs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:50:38.925994 opengate-10.0b3/opengate/source/beta_plus_spectra/Na22/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/source/beta_plus_spectra/Na22/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16945 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/source/beta_plus_spectra/Na22/beta+_Na22_tot.bs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:50:38.929994 opengate-10.0b3/opengate/source/beta_plus_spectra/O15/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/source/beta_plus_spectra/O15/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15262 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/source/beta_plus_spectra/O15/beta+_O15_tot.bs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:50:38.929994 opengate-10.0b3/opengate/source/beta_plus_spectra/Rb82/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/source/beta_plus_spectra/Rb82/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15685 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/source/beta_plus_spectra/Rb82/beta+_Rb82_tot.bs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:50:38.929994 opengate-10.0b3/opengate/source/beta_plus_spectra/Zr89/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/source/beta_plus_spectra/Zr89/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13332 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/source/beta_plus_spectra/Zr89/beta+_Zr89_tot.bs
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/source/beta_plus_spectra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/source/helpers_source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:50:38.929994 opengate-10.0b3/opengate/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-07 14:50:37.000000 opengate-10.0b3/opengate/tests/HEAD
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:50:38.929994 opengate-10.0b3/opengate/tests/log/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/log/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:50:38.929994 opengate-10.0b3/opengate/tests/output/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/output/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:50:38.929994 opengate-10.0b3/opengate/tests/output/output_test035/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/output/output_test035/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:50:38.941994 opengate-10.0b3/opengate/tests/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1851 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test001_G4ThreeVector.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      390 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test002_G4String.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1361 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test003_G4Material.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3918 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test004_simple.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2162 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test004_simple_MT.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1597 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test004_simple_visu.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1640 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test004_simple_visu_gdml.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1702 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test004_simple_visu_vrml.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1599 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test004_simple_visu_wip.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1769 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test004_simulation_stats_actor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1655 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test005_proton.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2520 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test006_runs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4900 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test007_volumes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3262 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test008_dose_actor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6229 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test008_geometry_dose_grid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3038 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test009_voxels.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3764 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test009_voxels_hu.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3928 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test010_generic_source.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3617 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test010_generic_source_confine.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1919 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test011_MT.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2929 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test012_MT_dose_actor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3129 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test013_half_life.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1147 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test013_phys_lists_1.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      893 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test013_phys_lists_2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1178 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test013_phys_lists_3_WIP.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1164 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test013_phys_lists_4.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1166 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test013_phys_lists_5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test013_phys_lists_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      278 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test014_engine_1.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      454 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test014_engine_2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      324 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test014_engine_3.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      324 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test014_engine_4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test014_engine_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test015_iec_phantom_1.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1654 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test015_iec_phantom_1_visu.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1515 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test015_iec_phantom_2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2269 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test015_iec_phantom_3.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3297 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test015_iec_phantom_4.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3011 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test016_bool_volumes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3322 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test017_repeater.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1715 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test018_pet_WIP.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      358 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test019_linac_phsp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      131 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test019_linac_phsp_MT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4708 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test019_linac_phsp_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5515 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test019_linac_phsp_source.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      404 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test019_linac_phsp_visu.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2931 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test020_profiling.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3607 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test021_voxel_source1.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4291 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test021_voxel_source2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5087 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test021_voxel_source_old_WIP.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4680 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test022_half_life.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      251 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test022_half_life_MT.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3008 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test023_filters.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2485 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test023_filters_iec_phantom.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2467 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test023_filters_material.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1251 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test024_py_actor_WIP.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      193 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test025_hits_collection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      193 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test025_hits_collection_MT.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6622 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test025_hits_collection_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1567 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test026_simple_signal.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4251 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test027_fake_spect_MT.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2255 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test028_ge_nm670_spect_1_colli.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2304 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test028_ge_nm670_spect_1_colli_visu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test028_ge_nm670_spect_2_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      422 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test028_ge_nm670_spect_2_hits.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      448 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test028_ge_nm670_spect_2_hits_MT.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      770 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test028_ge_nm670_spect_3_proj.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      590 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test028_ge_nm670_spect_3_proj_MT.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2236 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test028_ge_nm670_spect_3_proj_blur.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      465 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test028_ge_nm670_spect_4_acc_angle_aa_se.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      469 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test028_ge_nm670_spect_4_acc_angle_aa_se_MT.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      493 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test028_ge_nm670_spect_4_acc_angle_aa_ze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test028_ge_nm670_spect_4_acc_angle_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      415 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test028_ge_nm670_spect_4_acc_angle_noaa.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1458 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test029_volume_time_rotation_1.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1462 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test029_volume_time_rotation_1_process.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1631 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test029_volume_time_rotation_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test029_volume_time_rotation_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3433 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test030_dose_motion.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5151 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test031_beta+_spectrum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2683 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test032_create_voxelized_volume.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4226 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test032_voxel_vs_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test033_rotation_spect_aa_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      431 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test033_rotation_spect_aa_se.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      444 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test033_rotation_spect_aa_se_MT.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      431 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test033_rotation_spect_aa_ze.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      482 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test033_rotation_spect_noaa.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3210 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test034_gan_phsp_linac.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1795 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test035_dose_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test036_adder_depth_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      493 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test036_adder_depth_param.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      494 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test036_adder_depth_repeat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      653 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test037_digi_attributes_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test037_pet_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1870 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test037_pet_hits_singles_1.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2004 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test037_pet_hits_singles_1_visu.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2372 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test037_pet_hits_singles_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test037_pet_hits_singles_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      530 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test038_gan_phsp_spect_gan_MT.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2145 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test038_gan_phsp_spect_gan_aa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12933 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test038_gan_phsp_spect_gan_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      598 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test038_gan_phsp_spect_gan_se.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      598 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test038_gan_phsp_spect_gan_ze.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4825 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test038_gan_phsp_spect_training_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      314 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test039_hits_memory_check.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      314 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test039_hits_memory_check_MP_WIP.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test039_hits_memory_check_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3546 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test040_gan_phsp_pet_aref.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10665 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test040_gan_phsp_pet_gan.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4693 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test040_gan_phsp_pet_training_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3228 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test041_dose_actor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4052 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test042_gauss_gps.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3772 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test043_distances.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3777 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test043_garf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2702 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test043_garf_analog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test043_garf_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3258 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test043_garf_training_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5021 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test044_pbs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5574 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test044_pbs_rot_transl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5114 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test044_pbs_source_to_volume.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5694 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test044_pbs_unFocused.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5258 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test044_pbs_weight.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10666 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test045_gan_phsp_pet_gan_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3166 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test045_speedup.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3000 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test045_speedup_all.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2152 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test046_rad.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3910 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test047_gan_vox_source_cond.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1359 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test047_voxelization.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1293 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test048_split_spect_projections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5848 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test049_pet_digit_blurring_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1331 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test049_pet_digit_blurring_v1.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1456 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test049_pet_digit_blurring_v2_MT.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2008 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test049_pet_digit_blurring_v3.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2066 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test049_pet_digit_blurring_v4.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5529 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test050_let_actor_letd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3622 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test051_adder_time_difference.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2663 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test052_tac_activity_source.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1724 2023-06-07 14:49:37.000000 opengate-10.0b3/opengate/tests/src/test056_template_source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:50:38.917994 opengate-10.0b3/opengate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-06-07 14:50:38.000000 opengate-10.0b3/opengate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12697 2023-06-07 14:50:38.000000 opengate-10.0b3/opengate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 14:50:38.000000 opengate-10.0b3/opengate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-07 14:50:38.000000 opengate-10.0b3/opengate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-07 14:50:38.000000 opengate-10.0b3/opengate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 14:50:38.941994 opengate-10.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-07 14:49:37.000000 opengate-10.0b3/setup.py
```

### Comparing `opengate-10.0b2/CHANGELOG.md` & `opengate-10.0b3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/PKG-INFO` & `opengate-10.0b3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: opengate
-Version: 10.0b2
+Version: 10.0b3
 Summary: Simulation for Medical Physics
 Home-page: https://github.com/OpenGATE/opengate
 Author: Opengate collaboration
 Author-email: david.sarrut@creatis.insa-lyon.fr
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
 
 ![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/OpenGATE/opengate?logo=github)
 [![CI](https://github.com/OpenGATE/opengate/actions/workflows/main.yml/badge.svg)](https://github.com/OpenGATE/opengate/actions/workflows/main.yml)
 [![cirrus CI](https://api.cirrus-ci.com/github/OpenGATE/opengate.svg)](https://cirrus-ci.com/github/OpenGATE/opengate)
 [![Read the Docs](https://img.shields.io/readthedocs/opengate-python?logo=read-the-docs&style=plastic)](https://opengate-python.readthedocs.io/)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/OpenGATE/opengate/master.svg)](https://results.pre-commit.ci/latest/github/OpenGATE/opengate/master)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/OpenGATE/gam-gate/c65a0d55c616748454f066470aa836331eb107ac)
@@ -23,21 +24,28 @@
 See the [User Guide](https://opengate-python.readthedocs.io/en/latest/user_guide.html).
 
 # How to install (short version)
 
 First create an environment (not mandatory but highly advised)
 
 ```
+python -m venv opengate_env
+source opengate_env/bin/activate
+```
+
+or you can use the conda environment.
+
+```
 conda create --name opengate_env python=3.9
 conda activate opengate_env
 ```
 
 **Warning** not available for MacOS Intel with python 3.11 yet.
 
-Then install the package opengate. The package opengate_core is automatically downloaded.
+Then install the package opengate. The package opengate_core is automatically downloaded. opengate_core installs Geant4 v11.1.1 librairies.
 ```
 pip install --upgrade pip
 pip install --pre opengate
 ```
 
 If you already installed the packages and want to upgrade to last version:
 
@@ -46,22 +54,24 @@
 ```
 
 Once installed, you can run all tests:
 ````
 opengate_tests
 ````
 
-All tests are in the folder [here](https://github.com/OpenGATE/opengate/tree/master/opengate/tests/src). Some data (binary files) are stored, for technical reasons, in this git: https://gitlab.in2p3.fr/opengate/tests_data (which is stored as a git submodule).
+All tests are in the folder [here](https://github.com/OpenGATE/opengate/tree/master/opengate/tests/src). Some data (binary files) are stored, for technical reasons, in this git: https://gitlab.in2p3.fr/opengamgate/gam_tests_data (which is stored as a git submodule).
 
 **WARNING** some tests (e.g. test034) needs [gaga-phsp](https://github.com/dsarrut/gaga-phsp) which needs [pytorch](https://pytorch.org/) that cannot really be automatically installed by the previous pip install (at least we dont know how to do). So, in order to run those tests, you will have to install both pytorch and gaga-phsp first with
 ````
 pip install torch
 pip install gaga-phsp
 ````
 
 The documentation is here: https://opengate-python.readthedocs.io/en/latest/user_guide.html
 
 # How to install (long version, for developers)
 
 See the documentation : https://opengate-python.readthedocs.io/en/latest/developer_guide.html#installation-for-developers
 
+WARNING : need [Geant4 11.1.1](https://geant4.web.cern.ch/download/11.1.1.html)
+
```

### Comparing `opengate-10.0b2/README.md` & `opengate-10.0b3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -8,21 +8,28 @@
 See the [User Guide](https://opengate-python.readthedocs.io/en/latest/user_guide.html).
 
 # How to install (short version)
 
 First create an environment (not mandatory but highly advised)
 
 ```
+python -m venv opengate_env
+source opengate_env/bin/activate
+```
+
+or you can use the conda environment.
+
+```
 conda create --name opengate_env python=3.9
 conda activate opengate_env
 ```
 
 **Warning** not available for MacOS Intel with python 3.11 yet.
 
-Then install the package opengate. The package opengate_core is automatically downloaded.
+Then install the package opengate. The package opengate_core is automatically downloaded. opengate_core installs Geant4 v11.1.1 librairies.
 ```
 pip install --upgrade pip
 pip install --pre opengate
 ```
 
 If you already installed the packages and want to upgrade to last version:
 
@@ -31,20 +38,22 @@
 ```
 
 Once installed, you can run all tests:
 ````
 opengate_tests
 ````
 
-All tests are in the folder [here](https://github.com/OpenGATE/opengate/tree/master/opengate/tests/src). Some data (binary files) are stored, for technical reasons, in this git: https://gitlab.in2p3.fr/opengate/tests_data (which is stored as a git submodule).
+All tests are in the folder [here](https://github.com/OpenGATE/opengate/tree/master/opengate/tests/src). Some data (binary files) are stored, for technical reasons, in this git: https://gitlab.in2p3.fr/opengamgate/gam_tests_data (which is stored as a git submodule).
 
 **WARNING** some tests (e.g. test034) needs [gaga-phsp](https://github.com/dsarrut/gaga-phsp) which needs [pytorch](https://pytorch.org/) that cannot really be automatically installed by the previous pip install (at least we dont know how to do). So, in order to run those tests, you will have to install both pytorch and gaga-phsp first with
 ````
 pip install torch
 pip install gaga-phsp
 ````
 
 The documentation is here: https://opengate-python.readthedocs.io/en/latest/user_guide.html
 
 # How to install (long version, for developers)
 
 See the documentation : https://opengate-python.readthedocs.io/en/latest/developer_guide.html#installation-for-developers
+
+WARNING : need [Geant4 11.1.1](https://geant4.web.cern.ch/download/11.1.1.html)
```

### Comparing `opengate-10.0b2/core/external/fmt/CONTRIBUTING.md` & `opengate-10.0b3/core/external/fmt/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/core/external/fmt/support/bazel/README.md` & `opengate-10.0b3/core/external/fmt/support/bazel/README.md`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/core/external/fmt/test/fuzzing/README.md` & `opengate-10.0b3/core/external/fmt/test/fuzzing/README.md`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/core/external/pybind11/.github/CONTRIBUTING.md` & `opengate-10.0b3/core/external/pybind11/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/core/external/pybind11/.github/pull_request_template.md` & `opengate-10.0b3/core/external/pybind11/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/docs/source/developer_guide.md` & `opengate-10.0b3/docs/source/developer_guide.md`

 * *Files 10% similar despite different names*

```diff
@@ -20,37 +20,42 @@
 
 Note that you need to also clone the included submodules (pybind11, all data for tests etc). If you forget the `--recurse-submodules` you can still use `git submodule update --init --recursive` after the clone.
 
 First step: compile `opengate_core` (this is the hardest part). You need to set the path to build Geant4 and ITK libraries ; it means you need first to download and compile both [Geant4](https://geant4.web.cern.ch) and [ITK](https://itk.org).
 
 #### STEP 1 - Geant4 and Qt
 
-You must be in the conda environment created before and install qt5 **before** installing Geant4 so that Geant4 can find the correct qt lib:
+Installing QT is optional. Currently, QT visualisation is not working on all architectures.
+
+If you wish to use QT, you must install qt5 **before** installing Geant4 so that Geant4 can find the correct qt lib. It can be done for example with conda:
 
 ```bash
   conda install qt=5
 ```
 
-You must be in the conda environment created before and install qt5 **before** installing Geant4 so that Geant4 can find the correct qt lib:
 For **Geant4**, you need to compile with the following options:
 
 ```bash
-git clone --branch v11.0.2 https://github.com/Geant4/geant4.git --depth 1
+git clone --branch v11.1.0 https://github.com/Geant4/geant4.git --depth 1
 mkdir geant4.11-build
 cd geant4.11-build
 cmake -DCMAKE_CXX_FLAGS=-std=c++17 \
       -DGEANT4_INSTALL_DATA=ON \
       -DGEANT4_INSTALL_DATADIR=$HOME/software/geant4/data \
       -DGEANT4_USE_QT=ON \
       -DGEANT4_USE_OPENGL_X11=ON \
       -DGEANT4_BUILD_MULTITHREADED=ON \
       ../geant4
 make -j 32
 ```
 
+Change the QT flag (GEANT4_USE_QT) to OFF if you did not install QT.
+
+WARNING : from June 2023, [Geant4 11.1.1](https://geant4.web.cern.ch/download/11.1.1.html) is needed.
+
 #### STEP 2 - ITK
 
 For **ITK**, you need to compile with the following options:
 
 ```bash
 git clone --branch v5.1.0 https://github.com/InsightSoftwareConsortium/ITK.git --depth 1
 mkdir build-v5.1.0
@@ -245,15 +250,16 @@
 ## OPENGATE Physics
 
 todo
 
 ---
 ## OPENGATE Source
 
-TODO --> composition py/cpp (while actor = inherit)
+Consider the test056 and the "TemplateSource" as a starting example to create a new type of source.
+
 
 Main files: `SourceManager`, `SourceBase`,\`helper_sources\`, all `XXXSource.py`.
 
 - \[py\] `SourceManager`
 
     - Manages all sources (GateSourceManager) and all threads.
     - `run_timing_intervals` : array of start/end time for all runs
@@ -284,15 +290,15 @@
 
     - Base class for all types of source (cpp side)
     - `GeneratePrimaries`: is the main function that will be called by the source manager
     - `PrepareNextRun` and `PrepareNextTime` must be implemented. Will be called by the SourceManager to determine when this source shoot particles.
 
 The `SourceManager` class manages 1) all sources of particles and 2) the time associated with all runs. The sources are `SourceBase` objects that manage 1) the user properties stored in `user_info` and 2) the corresponding cpp object inheriting from `GateVSource`. The latter are created in the function `build()` by the `create_g4_source()` function and stored in the `self.g4_sources` array to avoid py pointer automatic deletion.
 
-The `GateSourceManager` inherits from G4 `G4VUserPrimaryGeneratorAction`. It manages the generation of events from all sources. The G4 engine call the method `GeneratePrimaries` every time a event should be simulated. The current active source and time of the event is determined a this moment, the source manager choose the next source that will shoot events according to the current simulation time. There are one GateSourceManager per thread.
+The `GateSourceManager` inherits from G4 `G4VUserPrimaryGeneratorAction`. It manages the generation of events from all sources. The G4 engine call the method `GeneratePrimaries` every time a event should be simulated. The current active source and time of the event is determined at this moment, the source manager choose the next source that will shoot events according to the current simulation time. There are one GateSourceManager per thread.
 
 All sources must inherit from `SourceBase` class. It must implement the function `create_g4_source` that will build the corresponding cpp source (that inherit from `GateVSource`). The goal of the py `SourceBase` is to manage the user options of the source and pass them to the cpp side.
 
 ---
 ## OPENGATE Actors
 
 TODO --> inheritance to allow callback ; warning cost trampoline
@@ -422,15 +428,15 @@
 Document is done with [readthedoc](https://docs.readthedocs.io/en/stable/index.html). To build the html pages locally, use `make html` in the `docs/` folder of the source directory. Configuration is in the `docs/source/config.py` file. The current theme is [sphinx_pdj_theme](https://github.com/jucacrispim/sphinx_pdj_theme)
 
 Help with reStructuredText (awful) syntax.
 
 - <https://docutils.sourceforge.io/docs/user/rst/quickref.html>
 - <https://docutils.sourceforge.io/docs/ref/rst/directives.html>
 
-## (draft notes)
+## Notes for developers
 
 ### Pybind11 hints
 
 Below are a list of hints (compared to boost-python).
 
 - <https://github.com/KratosMultiphysics/Kratos/wiki/Porting-to-PyBind11---common-steps>
 - bases is not any longer required. Only its template argument must remain, in the same position of what was there before.
@@ -440,7 +446,41 @@
 - `return_value_policy<reference_existing_object>` --> `py::return_value_policy::reference`
 - `return_internal_reference<>()` --> `py::return_value_policy::reference_internal`
 - `return_value_policy<return_by_value>()` --> `py::return_value_policy::copy`
 - `add_property` --> `.def_readwrite`
 - Overloading methods, i.e.: `py::overload_cast<G4VUserPrimaryGeneratorAction*>(&G4RunManager::SetUserAction))`
 - Pure virtual need a trampoline class <https://pybind11.readthedocs.io/en/stable/advanced/classes.html>
 - Python debug: `python -q -X faulthandler`
+
+
+
+### Geant4 seems to be frozen/sleeping - the GIL is to blame - here is why
+
+So here is what happened to me: While working on a branch, I implemented an alternative binding of the G4MTRunManager. The binding includes the function G4MTRunManager::Initialize(). The naïve implementation is:
+
+      .def("Initialize", &G4MTRunManager::Initialize)
+
+When I tried to run a test with threads>1, Geant4 simply stopped at some point, namely when geometry and physics list were apparently set up. No error, no segfault, no further output, no CPU load, just frozen. Umpf. After a scattering cout's through the Geant4 source could, I understood the problem, and why others, like David S, had used a smarter, less naïve binding of the Initialize() function.
+
+Here is what went wrong: G4MTRunManager::Initialize() function first calls the single thread G4RunManager::Initialize() and then does a fake run by calling BeamOn(0); The argument n–event=zero is internally interpreted as fake run and not all steps are performed as would be in a real BeamOn(). The purpose of the fake run is to set-up the worker run managers. BeamOn(0) does trigger G4RunManager::DoEventLoop() and this in turn triggers G4MTRunManager::InitializeEventLoop (the overridden version from the inherited G4MTRunManager!). At the very end, after creating and starting workers, there is a WaitForReadyWorkers(); This function contains beginOfEventLoopBarrier.Wait(GetNumberActiveThreads()); which essentially waits until all workers release locks. Specifically, it triggers a call to G4MTBarrier::Wait() which contains a while(true) loop to repeatedly check the number of locks on the shared resource, and breaks the loop when the number of locks equals the number of threads.
+
+Now, admittedly, I do not understand every detail here, but it is clear that Geant4’s implementation relies on locks to establish whether workers are ready. So when my simulation_engine (i.e., Gate internally) called g4_RunManager.Initialize(), it ended up stuck in the while loop waiting for the locks to decrease, which never happened. Why?
+
+This is where the so-called Global Interpreter Lock comes into play. Read this to understand the details: https://realpython.com/python-gil/, or don’t if you are smarter than I am. Essentially, at least in the CPython implementation, there is a lock (mutex) on all resources linked to the python interpreter. Historically, the GIL was a pragmatic choice to easily integrate C-extensions into python even if they were not thread-safe. What does that have to do with Gate? Well, many objects such as physics lists, are created in python, and then communicated to the Geant4 RunManager (e.g. via SetUserInitializaition). There is thus a lock on these resources, namely the GIL. The multithread mechanism in Geant4, on the other hand, does not know about the GIL and thus cannot account for this additional lock, so the lock counter never decreases sufficiently to satisfy Geant4. A way to resolve this dilemma, without hacking around in the Geant4 code, is to instruct pybind to release the Global Interpreter Lock within the scope of the call to a C++ function, such as Initialize(). One way to achieve this is to replace the naïve
+
+```
+.def("Initialize", &G4MTRunManager::Initialize)
+```
+
+by
+```
+      .def("Initialize",
+           [](G4MTRunManager *mt) {
+             py::gil_scoped_release release;
+             mt->Initialize();
+           })
+```
+The key here is the “py::gil_scoped_release release” statement. It instructs pybind to release the GIL before calling the function Initialize(). There is actually a useful passage in pybind’s doc: https://pybind11.readthedocs.io/en/stable/advanced/misc.html
+
+I think, in the case of Gate/Geant4, it is safe to release the GIL because we know that Geant4 handles shared resources in a thread-safe way. Quite the contrary: the GIL actually breaks G4’s mechanism.
+
+So what I learned from this: Any Geant4 function which relies on Geant4’s MT mechanism based on locks needs to be bound to python with a “py::gil_scoped_release release” statement as above. The serial version G4RunManager::Initialize() does not need this statement (and should not have it) because it does not check locks at any point.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `opengate-10.0b2/docs/source/user_guide_1_intro.md` & `opengate-10.0b3/docs/source/user_guide_1_intro.md`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,21 @@
 
 You only have to install the Python module with, the --pre option is mandatory to have the latest release:
 
     pip install --pre opengate
 
 Then, you can create a simulation using the opengate module (see below). For **developers**, please look the [developer guide](developer_guide) for the developer installation.
 
-{tip} We highly recommend creating a specific python environment to 1) be sure all dependencies are handled properly and 2) don't mix with your other Python modules. For example, you can use `conda`. Once the environment is created, you need to activate it:
+{tip} We highly recommend creating a specific python environment to 1) be sure all dependencies are handled properly and 2) don't mix with your other Python modules. For example, you can use `venv`. Once the environment is created, you need to activate it:
+
+    python -m venv opengate_env
+    source opengate_env/bin/activate
+    pip install --pre opengate
+
+or with `conda` environment:
 
     conda create --name opengate_env python=3.10
     conda activate opengate_env
     pip install --pre opengate
 
 
 Maybe you need to upgrade the pip module with:
```

### Comparing `opengate-10.0b2/docs/source/user_guide_2_0_simulation.md` & `opengate-10.0b3/docs/source/user_guide_2_0_simulation.md`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/docs/source/user_guide_2_1_volumes.md` & `opengate-10.0b3/docs/source/user_guide_2_1_volumes.md`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/docs/source/user_guide_2_2_sources.md` & `opengate-10.0b3/docs/source/user_guide_2_2_sources.md`

 * *Files 10% similar despite different names*

```diff
@@ -109,14 +109,38 @@
 This code create a voxelized source. The 3D activity distribution is read from the given image. This image is internally normalized such that the sum of all pixels values is 1, leading to a 3D probability distribution. Particles will be randomly located somewhere in the image according to this probability distribution. Note that once an activity voxel is
 chosen from this distribution, the location of the particle inside the voxel is performed uniformly. In the given example, 4 kBq of electrons of 140 keV will be generated.
 
 Like all objects, by default, the source is located according to the coordinate system of its mother volume. For example, if the mother volume is a box, it will be the center of the box. If it is a voxelized volume (typically a CT image), it will the **center** of this image: the image own coordinate system (ITK's origin) is not considered here. If you want to align a voxelized activity with a CT image that have the same coordinate system you should compute the correct translation. This is done by the function  ```gate.get_translation_between_images_center```. See the contrib example ```dose_rate.py```.
 
 ![](figures/image_coord_system.png)
 
+### Phase-Space sources
+
+A phase-space source read particles properties (position, direction, energy, etc) from a root file and use them as events. Here is an example:
+
+```python
+source = sim.add_source("PhaseSpaceSource", "phsp_source")
+source.mother = plane.name
+source.phsp_file = "input.root"
+source.position_key = "PrePositionLocal"
+source.direction_key = "PreDirectionLocal"
+source.global_flag = False
+source.particle = "gamma"
+source.batch_size = 4000
+source.n = 20000
+```
+
+In that case, the key "PrePositionLocal" in the root tree file will be used to define the position of all generated particles. The flag "global_flag" is False so the position will be relative to the mother volume (the plane here) ; otherwise, position is considered as global (in the world coordinate system).
+
+Limitations:
+- The timing is read from the phsp and not considered (yet)
+- It is NOT ready for multithread (yet): for that, we need to define a generate that read the root file in random order to at different starting index for each thread.
+- The type of particle is not read in the phase space but set by user
+
+See test019 as an example.
 
 ### GAN sources (Generative Adversarial Network)
 
 (documentation TODO)
 
 - `test034` : GAN for linac
 - `test038` : GAN for SPECT
```

### Comparing `opengate-10.0b2/docs/source/user_guide_2_3_physics.md` & `opengate-10.0b3/docs/source/user_guide_2_3_physics.md`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/docs/source/user_guide_2_4_actors.md` & `opengate-10.0b3/docs/source/user_guide_2_4_actors.md`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/docs/source/user_guide_3_addons.md` & `opengate-10.0b3/docs/source/user_guide_3_addons.md`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/ExceptionHandler.py` & `opengate-10.0b3/opengate/ExceptionHandler.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/RunAction.py` & `opengate-10.0b3/opengate/RunAction.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/Simulation.py` & `opengate-10.0b3/opengate/Simulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,7 +192,13 @@
     def initialize(self):
         # self.current_engine = gate.SimulationEngine(self, start_new_process=False)
         gate.warning(f"(initialization do nothing)")
 
     def start(self, start_new_process=False):
         se = gate.SimulationEngine(self, start_new_process=start_new_process)
         return se.start()
+
+    def use_multithread(self):
+        return (
+            self.user_info.number_of_threads > 1
+            or self.user_info.force_multithread_mode
+        )
```

### Comparing `opengate-10.0b2/opengate/SimulationEngine.py` & `opengate-10.0b3/opengate/SimulationEngine.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/SimulationOutput.py` & `opengate-10.0b3/opengate/SimulationOutput.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/SimulationUserInfo.py` & `opengate-10.0b3/opengate/SimulationUserInfo.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/UIsessionVerbose.py` & `opengate-10.0b3/opengate/UIsessionVerbose.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/UserElement.py` & `opengate-10.0b3/opengate/UserElement.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/UserInfo.py` & `opengate-10.0b3/opengate/UserInfo.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/__init__.py` & `opengate-10.0b3/opengate/__init__.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/actor/ARFActor.py` & `opengate-10.0b3/opengate/actor/ARFActor.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/actor/ARFTrainingDatasetActor.py` & `opengate-10.0b3/opengate/actor/ARFTrainingDatasetActor.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/actor/ActionEngine.py` & `opengate-10.0b3/opengate/actor/ActionEngine.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/actor/ActorBase.py` & `opengate-10.0b3/opengate/actor/ActorBase.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/actor/ActorEngine.py` & `opengate-10.0b3/opengate/actor/ActorEngine.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/actor/ActorManager.py` & `opengate-10.0b3/opengate/actor/ActorManager.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/actor/DigitizerAdderActor.py` & `opengate-10.0b3/opengate/actor/DigitizerAdderActor.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/actor/DigitizerBlurringActor.py` & `opengate-10.0b3/opengate/actor/DigitizerBlurringActor.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/actor/DigitizerEnergyWindowsActor.py` & `opengate-10.0b3/opengate/actor/DigitizerEnergyWindowsActor.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/actor/DigitizerHitsCollectionActor.py` & `opengate-10.0b3/opengate/actor/DigitizerHitsCollectionActor.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/actor/DigitizerProjectionActor.py` & `opengate-10.0b3/opengate/actor/DigitizerProjectionActor.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/actor/DigitizerReadoutActor.py` & `opengate-10.0b3/opengate/actor/DigitizerReadoutActor.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/actor/DigitizerSpatialBlurringActor.py` & `opengate-10.0b3/opengate/actor/DigitizerSpatialBlurringActor.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/actor/DoseActor.py` & `opengate-10.0b3/opengate/actor/DoseActor.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/actor/FilterBase.py` & `opengate-10.0b3/opengate/actor/FilterBase.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/actor/FilterManager.py` & `opengate-10.0b3/opengate/actor/FilterManager.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/actor/KineticEnergyFilter.py` & `opengate-10.0b3/opengate/actor/KineticEnergyFilter.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/actor/LETActor.py` & `opengate-10.0b3/opengate/actor/LETActor.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/actor/MotionVolumeActor.py` & `opengate-10.0b3/opengate/actor/MotionVolumeActor.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/actor/ParticleFilter.py` & `opengate-10.0b3/opengate/actor/ParticleFilter.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/actor/PhaseSpaceActor.py` & `opengate-10.0b3/opengate/actor/PhaseSpaceActor.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/actor/SimulationStatisticsActor.py` & `opengate-10.0b3/opengate/actor/SimulationStatisticsActor.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/actor/SourceInfoActor.py` & `opengate-10.0b3/opengate/actor/SourceInfoActor.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/actor/TestActor.py` & `opengate-10.0b3/opengate/actor/TestActor.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/actor/TrackCreatorProcessFilter.py` & `opengate-10.0b3/opengate/actor/TrackCreatorProcessFilter.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/actor/helpers_actor.py` & `opengate-10.0b3/opengate/actor/helpers_actor.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/bin/dose_rate` & `opengate-10.0b3/opengate/bin/dose_rate`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/bin/opengate_tests_utils` & `opengate-10.0b3/opengate/bin/opengate_tests_utils`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/bin/opengate_user_info` & `opengate-10.0b3/opengate/bin/opengate_user_info`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/bin/opengate_visu` & `opengate-10.0b3/opengate/bin/opengate_visu`

 * *Files 6% similar despite different names*

```diff
@@ -27,28 +27,28 @@
         except:
             print(
                 "The module pyvista is not installed to be able to visualize vrml files. Execute:"
             )
             print("pip install pyvista")
             return
         pl = pyvista.Plotter()
-        pl.import_vrml(self.simulation.user_info.visu_filename)
+        pl.import_vrml(input)  # self.simulation.user_info.visu_filename)
         pl.add_axes(line_width=5)
         pl.show()
 
     if gdml:
         try:
             import pyg4ometry
         except:
             print(
                 "The module pyg4ometry is not installed to be able to visualize gdml files. Execute:"
             )
             print("pip install pyg4ometry")
             return
-        r = pyg4ometry.gdml.Reader(self.simulation.user_info.visu_filename)
+        r = pyg4ometry.gdml.Reader(input)  # self.simulation.user_info.visu_filename)
         l = r.getRegistry().getWorldVolume()
         v = pyg4ometry.visualisation.VtkViewerColouredMaterial()
         v.addLogicalVolume(l)
         v.view()
 
 
 # --------------------------------------------------------------------------
```

### Comparing `opengate-10.0b2/opengate/bin/split_spect_projections` & `opengate-10.0b3/opengate/bin/split_spect_projections`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/bin/voxelize_iec_phantom` & `opengate-10.0b3/opengate/bin/voxelize_iec_phantom`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/contrib/GateMaterials.db` & `opengate-10.0b3/opengate/contrib/GateMaterials.db`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/contrib/dose_rate_helpers.py` & `opengate-10.0b3/opengate/contrib/dose_rate_helpers.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/contrib/dose_rate_test1.json` & `opengate-10.0b3/opengate/contrib/dose_rate_test1.json`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/contrib/linac_elekta_synergy.py` & `opengate-10.0b3/opengate/contrib/linac_elekta_synergy.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/contrib/linac_elekta_synergy_materials.db` & `opengate-10.0b3/opengate/contrib/linac_elekta_synergy_materials.db`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/contrib/pet_philips_vereos.py` & `opengate-10.0b3/opengate/contrib/pet_philips_vereos.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/contrib/pet_siemens_biograph.py` & `opengate-10.0b3/opengate/contrib/pet_siemens_biograph.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/contrib/pet_siemens_biograph_materials.db` & `opengate-10.0b3/opengate/contrib/pet_siemens_biograph_materials.db`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/contrib/phantom_necr.py` & `opengate-10.0b3/opengate/contrib/phantom_necr.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/contrib/phantom_nema_iec_body.py` & `opengate-10.0b3/opengate/contrib/phantom_nema_iec_body.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/contrib/spect_ge_nm670.py` & `opengate-10.0b3/opengate/contrib/spect_ge_nm670.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/contrib/spect_ge_nm670_materials.db` & `opengate-10.0b3/opengate/contrib/spect_ge_nm670_materials.db`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/contrib/spect_ideal_timed_reconstruction.py` & `opengate-10.0b3/opengate/contrib/spect_ideal_timed_reconstruction.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/geometry/BooleanVolume.py` & `opengate-10.0b3/opengate/geometry/BooleanVolume.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/geometry/ConsVolume.py` & `opengate-10.0b3/opengate/geometry/ConsVolume.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/geometry/ElementBuilder.py` & `opengate-10.0b3/opengate/geometry/ElementBuilder.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/geometry/HexagonVolume.py` & `opengate-10.0b3/opengate/geometry/HexagonVolume.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/geometry/ImageVolume.py` & `opengate-10.0b3/opengate/geometry/ImageVolume.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/geometry/MaterialBuilder.py` & `opengate-10.0b3/opengate/geometry/MaterialBuilder.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/geometry/MaterialDatabase.py` & `opengate-10.0b3/opengate/geometry/MaterialDatabase.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/geometry/PolyhedraVolume.py` & `opengate-10.0b3/opengate/geometry/PolyhedraVolume.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/geometry/RepeatParametrisedVolume.py` & `opengate-10.0b3/opengate/geometry/RepeatParametrisedVolume.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/geometry/SphereVolume.py` & `opengate-10.0b3/opengate/geometry/SphereVolume.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/geometry/TrapVolume.py` & `opengate-10.0b3/opengate/geometry/TrapVolume.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/geometry/TrdVolume.py` & `opengate-10.0b3/opengate/geometry/TrdVolume.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/geometry/TubsVolume.py` & `opengate-10.0b3/opengate/geometry/TubsVolume.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/geometry/VolumeBase.py` & `opengate-10.0b3/opengate/geometry/VolumeBase.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/geometry/VolumeEngine.py` & `opengate-10.0b3/opengate/geometry/VolumeEngine.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/geometry/VolumeManager.py` & `opengate-10.0b3/opengate/geometry/VolumeManager.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/geometry/helpers_geometry.py` & `opengate-10.0b3/opengate/geometry/helpers_geometry.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/geometry/helpers_materials.py` & `opengate-10.0b3/opengate/geometry/helpers_materials.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/helpers.py` & `opengate-10.0b3/opengate/helpers.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/helpers_element.py` & `opengate-10.0b3/opengate/helpers_element.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/helpers_image.py` & `opengate-10.0b3/opengate/helpers_image.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/helpers_log.py` & `opengate-10.0b3/opengate/helpers_log.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/helpers_run_timing.py` & `opengate-10.0b3/opengate/helpers_run_timing.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/helpers_tests.py` & `opengate-10.0b3/opengate/helpers_tests.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/helpers_tests_root.py` & `opengate-10.0b3/opengate/helpers_tests_root.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/helpers_transform.py` & `opengate-10.0b3/opengate/helpers_transform.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/mac/default_visu_commands.mac` & `opengate-10.0b3/opengate/mac/default_visu_commands.mac`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/physics/PhysicsEngine.py` & `opengate-10.0b3/opengate/physics/PhysicsEngine.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/physics/PhysicsManager.py` & `opengate-10.0b3/opengate/physics/PhysicsManager.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/physics/PhysicsUserInfo.py` & `opengate-10.0b3/opengate/physics/PhysicsUserInfo.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/physics/helpers_physics.py` & `opengate-10.0b3/opengate/physics/helpers_physics.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/source/GANPairsSource.py` & `opengate-10.0b3/opengate/source/GANPairsSource.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/source/GANSource.py` & `opengate-10.0b3/opengate/source/GANSource.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/source/GANSourceConditionalGenerator.py` & `opengate-10.0b3/opengate/source/GANSourceConditionalGenerator.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/source/GANSourceConditionalPairsGenerator.py` & `opengate-10.0b3/opengate/source/GANSourceConditionalPairsGenerator.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/source/GANSourceDefaultGenerator.py` & `opengate-10.0b3/opengate/source/GANSourceDefaultGenerator.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/source/GANSourceDefaultPairsGenerator.py` & `opengate-10.0b3/opengate/source/GANSourceDefaultPairsGenerator.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/source/GenericSource.py` & `opengate-10.0b3/opengate/source/GenericSource.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/source/PencilBeamSource.py` & `opengate-10.0b3/opengate/source/PencilBeamSource.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/source/SourceBase.py` & `opengate-10.0b3/opengate/source/SourceBase.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/source/SourceEngine.py` & `opengate-10.0b3/opengate/source/SourceEngine.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/source/SourceManager.py` & `opengate-10.0b3/opengate/source/SourceManager.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/source/VoxelizedSourceConditionGenerator.py` & `opengate-10.0b3/opengate/source/VoxelizedSourceConditionGenerator.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/source/VoxelizedSourcePDFSampler.py` & `opengate-10.0b3/opengate/source/VoxelizedSourcePDFSampler.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/source/VoxelsSource.py` & `opengate-10.0b3/opengate/source/VoxelsSource.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/source/beta_plus_spectra/C11/beta+_C11_tot.bs` & `opengate-10.0b3/opengate/source/beta_plus_spectra/C11/beta+_C11_tot.bs`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/source/beta_plus_spectra/F18/beta+_F18_tot.bs` & `opengate-10.0b3/opengate/source/beta_plus_spectra/F18/beta+_F18_tot.bs`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/source/beta_plus_spectra/Ga68/beta+_Ga68_tot.bs` & `opengate-10.0b3/opengate/source/beta_plus_spectra/Ga68/beta+_Ga68_tot.bs`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/source/beta_plus_spectra/N13/beta+_N13_tot.bs` & `opengate-10.0b3/opengate/source/beta_plus_spectra/N13/beta+_N13_tot.bs`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/source/beta_plus_spectra/Na22/beta+_Na22_tot.bs` & `opengate-10.0b3/opengate/source/beta_plus_spectra/Na22/beta+_Na22_tot.bs`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/source/beta_plus_spectra/O15/beta+_O15_tot.bs` & `opengate-10.0b3/opengate/source/beta_plus_spectra/O15/beta+_O15_tot.bs`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/source/beta_plus_spectra/Rb82/beta+_Rb82_tot.bs` & `opengate-10.0b3/opengate/source/beta_plus_spectra/Rb82/beta+_Rb82_tot.bs`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/source/beta_plus_spectra/Zr89/beta+_Zr89_tot.bs` & `opengate-10.0b3/opengate/source/beta_plus_spectra/Zr89/beta+_Zr89_tot.bs`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/source/helpers_source.py` & `opengate-10.0b3/opengate/source/helpers_source.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 from .VoxelsSource import *
 from .GANSource import *
 from .GANPairsSource import *
 from .PencilBeamSource import *
+from .TemplateSource import *
+from .PhaseSpaceSource import *
 import pathlib
 
 """
     List of source types: Generic, Voxels etc
 
     Energy spectra for beta+ emitters
 """
 
 source_type_names = {
     GenericSource,
     VoxelsSource,
     GANSource,
     GANPairsSource,
     PencilBeamSource,
+    TemplateSource,
+    PhaseSpaceSource,
 }
 source_builders = gate.make_builders(source_type_names)
 
 gate_source_path = pathlib.Path(__file__).parent.resolve()
 
 # http://www.lnhb.fr/nuclear-data/module-lara/
 all_beta_plus_radionuclides = [
```

### Comparing `opengate-10.0b2/opengate/tests/src/test001_G4ThreeVector.py` & `opengate-10.0b3/opengate/tests/src/test001_G4ThreeVector.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test003_G4Material.py` & `opengate-10.0b3/opengate/tests/src/test003_G4Material.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test004_simple.py` & `opengate-10.0b3/opengate/tests/src/test004_simple.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test004_simple_MT.py` & `opengate-10.0b3/opengate/tests/src/test004_simple_MT.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test004_simple_visu.py` & `opengate-10.0b3/opengate/tests/src/test004_simple_visu.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test004_simple_visu_gdml.py` & `opengate-10.0b3/opengate/tests/src/test004_simple_visu_gdml.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test004_simple_visu_vrml.py` & `opengate-10.0b3/opengate/tests/src/test004_simple_visu_vrml.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test004_simple_visu_wip.py` & `opengate-10.0b3/opengate/tests/src/test004_simple_visu_wip.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test004_simulation_stats_actor.py` & `opengate-10.0b3/opengate/tests/src/test004_simulation_stats_actor.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test005_proton.py` & `opengate-10.0b3/opengate/tests/src/test005_proton.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test006_runs.py` & `opengate-10.0b3/opengate/tests/src/test006_runs.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test007_volumes.py` & `opengate-10.0b3/opengate/tests/src/test007_volumes.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test008_dose_actor.py` & `opengate-10.0b3/opengate/tests/src/test008_dose_actor.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test008_geometry_dose_grid.py` & `opengate-10.0b3/opengate/tests/src/test008_geometry_dose_grid.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test009_voxels.py` & `opengate-10.0b3/opengate/tests/src/test009_voxels.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test009_voxels_hu.py` & `opengate-10.0b3/opengate/tests/src/test009_voxels_hu.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test010_generic_source.py` & `opengate-10.0b3/opengate/tests/src/test010_generic_source.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test010_generic_source_confine.py` & `opengate-10.0b3/opengate/tests/src/test010_generic_source_confine.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test011_MT.py` & `opengate-10.0b3/opengate/tests/src/test011_MT.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test012_MT_dose_actor.py` & `opengate-10.0b3/opengate/tests/src/test012_MT_dose_actor.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test013_half_life.py` & `opengate-10.0b3/opengate/tests/src/test013_half_life.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test013_phys_lists_1.py` & `opengate-10.0b3/opengate/tests/src/test013_phys_lists_1.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test013_phys_lists_2.py` & `opengate-10.0b3/opengate/tests/src/test013_phys_lists_2.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test013_phys_lists_3_WIP.py` & `opengate-10.0b3/opengate/tests/src/test013_phys_lists_3_WIP.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test013_phys_lists_4.py` & `opengate-10.0b3/opengate/tests/src/test013_phys_lists_4.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test013_phys_lists_5.py` & `opengate-10.0b3/opengate/tests/src/test013_phys_lists_5.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 p = sim.get_physics_user_info()
 p.physics_list_name = "QGSP_BERT_EMZ"
 p.enable_decay = True
 mm = gate.g4_units("mm")
 cuts = p.production_cuts
 cuts.world.gamma = 5 * mm
 cuts.world.proton = 1 * mm
-cuts.world.electron = -1  # default
+cuts.world.electron = 1 * mm  # default
 cuts.world.positron = 3 * mm
 cuts.waterbox.gamma = 2 * mm
 cuts.b2.electron = 5 * mm
 
 # em parameters
 phys_em_parameters(p)
```

### Comparing `opengate-10.0b2/opengate/tests/src/test013_phys_lists_helpers.py` & `opengate-10.0b3/opengate/tests/src/test013_phys_lists_helpers.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test014_engine_helpers.py` & `opengate-10.0b3/opengate/tests/src/test014_engine_helpers.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test015_iec_phantom_1.py` & `opengate-10.0b3/opengate/tests/src/test015_iec_phantom_1.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test015_iec_phantom_1_visu.py` & `opengate-10.0b3/opengate/tests/src/test015_iec_phantom_1_visu.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test015_iec_phantom_2.py` & `opengate-10.0b3/opengate/tests/src/test015_iec_phantom_2.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test015_iec_phantom_3.py` & `opengate-10.0b3/opengate/tests/src/test015_iec_phantom_3.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test015_iec_phantom_4.py` & `opengate-10.0b3/opengate/tests/src/test015_iec_phantom_4.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test016_bool_volumes.py` & `opengate-10.0b3/opengate/tests/src/test016_bool_volumes.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test017_repeater.py` & `opengate-10.0b3/opengate/tests/src/test017_repeater.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test018_pet_WIP.py` & `opengate-10.0b3/opengate/tests/src/test018_pet_WIP.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test019_linac_phsp_helpers.py` & `opengate-10.0b3/opengate/tests/src/test019_linac_phsp_helpers.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,33 +29,26 @@
     cm = gate.g4_units("cm")
     nm = gate.g4_units("nm")
 
     #  adapt world size
     world = sim.world
     world.size = [1 * m, 1 * m, 1 * m]
 
-    # add a waterbox
-    # waterbox = sim.add_volume('Box', 'Waterbox')
-    # waterbox.size = [30 * cm, 30 * cm, 30 * cm]
-    # waterbox.translation = [0 * cm, 0 * cm, 0 * cm]
-    # waterbox.material = 'G4_WATER'
-    # waterbox.color = [0, 0, 1, 1]  # blue
-
     # add a linac
     linac = gate_linac.add_linac(sim, "linac")
     linac.translation = [0, 0, 0 * m]
 
     # virtual plane for phase space
     plane = sim.add_volume("Tubs", "phase_space_plane")
     plane.mother = world.name
     plane.material = "G4_AIR"
     plane.rmin = 0
-    plane.rmax = 40 * mm
-    plane.dz = 9 * cm  # half height
-    plane.translation = [0, 0, -300 * mm - plane.dz]
+    plane.rmax = 70 * mm
+    plane.dz = 1 * nm  # half height
+    plane.translation = [0, 0, -300.0001 * mm]
     plane.color = [1, 0, 0, 1]  # red
 
     # e- source
     source = sim.add_source("GenericSource", "Default")
     Bq = gate.g4_units("Bq")
     MeV = gate.g4_units("MeV")
     source.particle = "e-"
@@ -78,16 +71,18 @@
     ta2 = sim.add_actor("PhaseSpaceActor", "PhaseSpace")
     ta2.mother = plane.name
     ta2.attributes = [
         "KineticEnergy",
         "Weight",
         "PostPosition",
         "PrePosition",
+        "PrePositionLocal",
         "ParticleName",
         "PreDirection",
+        "PreDirectionLocal",
         "PostDirection",
         "TimeFromBeginOfEvent",
         "GlobalTime",
         "LocalTime",
         "EventPosition",
     ]
     ta2.output = paths.output / "test019_hits.root"
@@ -146,23 +141,19 @@
     print("Reference gate tree : ", fn1)
     print("Checked Tree : ", fn2)
     data_ref, keys_ref, m_ref = phsp.load(fn1)
     data, keys, m = phsp.load(fn2)
     # find the good key's names
     keys1, keys2, scalings, tols = gate.get_keys_correspondence(keys_ref)
     # Do not check some keys
-    tols[keys1.index("Weight")] = 0.002
-    tols[keys1.index("Z")] = 0.09
+    tols[keys1.index("Weight")] = 0.001
     tols[keys1.index("Ekine")] = 0.1
-    tols[keys1.index("Y")] = 1.6
-    tols[keys1.index("X")] = 1.5
-    tols[keys1.index("Z")] = 1.2
-    # the Z position is not the same (plane is translated), and is fixed
-    mm = gate.g4_units("mm")
-    data[:, keys.index("PostPosition_Z")] += 297 * mm
+    tols[keys1.index("Y")] = 2.0
+    tols[keys1.index("X")] = 2.0
+    tols[keys1.index("Z")] = 0.2
     # perform the test
     is_ok = (
         gate.compare_trees(
             data_ref, keys_ref, data, keys, keys1, keys2, tols, scalings, scalings, True
         )
         and is_ok
     )
```

### Comparing `opengate-10.0b2/opengate/tests/src/test020_profiling.py` & `opengate-10.0b3/opengate/tests/src/test020_profiling.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test021_voxel_source1.py` & `opengate-10.0b3/opengate/tests/src/test021_voxel_source1.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test021_voxel_source2.py` & `opengate-10.0b3/opengate/tests/src/test021_voxel_source2.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test021_voxel_source_old_WIP.py` & `opengate-10.0b3/opengate/tests/src/test021_voxel_source_old_WIP.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test022_half_life.py` & `opengate-10.0b3/opengate/tests/src/test022_half_life.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test023_filters.py` & `opengate-10.0b3/opengate/tests/src/test023_filters.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test023_filters_iec_phantom.py` & `opengate-10.0b3/opengate/tests/src/test023_filters_iec_phantom.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import opengate as gate
-import opengate_core as g4
 import pathlib
-import os
 import opengate.contrib.phantom_nema_iec_body as gate_iec
 
 pathFile = pathlib.Path(__file__).parent.resolve()
 
 # create the simulation
 sim = gate.Simulation()
 
 # main options
 ui = sim.user_info
 ui.g4_verbose = False
 ui.g4_verbose_level = 1
 ui.visu = False
-ui.random_seed = 123456
+ui.random_seed = 1234567
 
 # units
 m = gate.g4_units("m")
 cm = gate.g4_units("cm")
 keV = gate.g4_units("keV")
 MeV = gate.g4_units("MeV")
 Bq = gate.g4_units("Bq")
@@ -94,11 +92,11 @@
     pathFile / ".." / "data" / "output_ref" / "test023_stats_iec_phantom.txt"
 )
 is_ok = gate.assert_stats(stat, stats_ref, 0.8)
 is_ok = is_ok and gate.assert_images(
     pathFile / ".." / "data" / "output_ref" / "test023_iec_phantom-edep.mhd",
     pathFile / ".." / "output" / "test023-edep.mhd",
     stat,
-    tolerance=50,
+    tolerance=100,
 )
 
 gate.test_ok(is_ok)
```

### Comparing `opengate-10.0b2/opengate/tests/src/test023_filters_material.py` & `opengate-10.0b3/opengate/tests/src/test023_filters_material.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import opengate as gate
-import opengate_core as g4
 import pathlib
-import os
 
 pathFile = pathlib.Path(__file__).parent.resolve()
 
 # create the simulation
 sim = gate.Simulation()
 sim.add_material_database(pathFile / ".." / "data" / "GateMaterials.db")
 
 # main options
 ui = sim.user_info
 ui.g4_verbose = False
 ui.g4_verbose_level = 1
 ui.visu = False
-ui.random_seed = 123456
+ui.random_seed = 1234567
 
 # units
 m = gate.g4_units("m")
 cm = gate.g4_units("cm")
 MeV = gate.g4_units("MeV")
 Bq = gate.g4_units("Bq")
 nm = gate.g4_units("nm")
@@ -93,11 +91,12 @@
     pathFile / ".." / "data" / "output_ref" / "test023_stats.txt"
 )
 is_ok = gate.assert_stats(stat, stats_ref, 0.8)
 is_ok = is_ok and gate.assert_images(
     pathFile / ".." / "data" / "output_ref" / "test023-edep.mhd",
     pathFile / ".." / "output" / "test023-edep.mhd",
     stat,
+    sum_tolerance=6,
     tolerance=50,
 )
 
 gate.test_ok(is_ok)
```

### Comparing `opengate-10.0b2/opengate/tests/src/test024_py_actor_WIP.py` & `opengate-10.0b3/opengate/tests/src/test024_py_actor_WIP.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test025_hits_collection_helpers.py` & `opengate-10.0b3/opengate/tests/src/test025_hits_collection_helpers.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test026_simple_signal.py` & `opengate-10.0b3/opengate/tests/src/test026_simple_signal.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test027_fake_spect_MT.py` & `opengate-10.0b3/opengate/tests/src/test027_fake_spect_MT.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test028_ge_nm670_spect_1_colli.py` & `opengate-10.0b3/opengate/tests/src/test028_ge_nm670_spect_1_colli.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test028_ge_nm670_spect_1_colli_visu.py` & `opengate-10.0b3/opengate/tests/src/test028_ge_nm670_spect_1_colli_visu.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test028_ge_nm670_spect_2_helpers.py` & `opengate-10.0b3/opengate/tests/src/test028_ge_nm670_spect_2_helpers.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test028_ge_nm670_spect_3_proj.py` & `opengate-10.0b3/opengate/tests/src/test028_ge_nm670_spect_3_proj.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test028_ge_nm670_spect_3_proj_MT.py` & `opengate-10.0b3/opengate/tests/src/test028_ge_nm670_spect_3_proj_MT.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test028_ge_nm670_spect_3_proj_blur.py` & `opengate-10.0b3/opengate/tests/src/test028_ge_nm670_spect_3_proj_blur.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test028_ge_nm670_spect_4_acc_angle_helpers.py` & `opengate-10.0b3/opengate/tests/src/test028_ge_nm670_spect_4_acc_angle_helpers.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test029_volume_time_rotation_1.py` & `opengate-10.0b3/opengate/tests/src/test029_volume_time_rotation_1.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test029_volume_time_rotation_1_process.py` & `opengate-10.0b3/opengate/tests/src/test029_volume_time_rotation_1_process.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test029_volume_time_rotation_2.py` & `opengate-10.0b3/opengate/tests/src/test029_volume_time_rotation_2.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test029_volume_time_rotation_helpers.py` & `opengate-10.0b3/opengate/tests/src/test029_volume_time_rotation_helpers.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test030_dose_motion.py` & `opengate-10.0b3/opengate/tests/src/test030_dose_motion.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test031_beta+_spectrum.py` & `opengate-10.0b3/opengate/tests/src/test031_beta+_spectrum.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test032_create_voxelized_volume.py` & `opengate-10.0b3/opengate/tests/src/test032_create_voxelized_volume.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test032_voxel_vs_volume.py` & `opengate-10.0b3/opengate/tests/src/test032_voxel_vs_volume.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test033_rotation_spect_aa_helpers.py` & `opengate-10.0b3/opengate/tests/src/test033_rotation_spect_aa_helpers.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test034_gan_phsp_linac.py` & `opengate-10.0b3/opengate/tests/src/test034_gan_phsp_linac.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test035_dose_rate.py` & `opengate-10.0b3/opengate/tests/src/test035_dose_rate.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test036_adder_depth_helpers.py` & `opengate-10.0b3/opengate/tests/src/test036_adder_depth_helpers.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test037_digi_attributes_list.py` & `opengate-10.0b3/opengate/tests/src/test037_digi_attributes_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,13 +15,13 @@
 print(
     f"Types are: 3 (ThreeVector), D (double), S (string), I (int), U (unique volume ID)"
 )
 for a in nlist:
     att = am.GetDigiAttributeByName(a)
     print(att.GetDigiAttributeName(), att.GetDigiAttributeType())
 
-n = 38
+n = 39
 is_ok = len(nlist) == n
 
 gate.print_test(is_ok, f"Done for {n} attributes.")
 
 gate.test_ok(is_ok)
```

### Comparing `opengate-10.0b2/opengate/tests/src/test037_pet_helpers.py` & `opengate-10.0b3/opengate/tests/src/test037_pet_helpers.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test037_pet_hits_singles_1.py` & `opengate-10.0b3/opengate/tests/src/test037_pet_hits_singles_1.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test037_pet_hits_singles_1_visu.py` & `opengate-10.0b3/opengate/tests/src/test037_pet_hits_singles_1_visu.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test037_pet_hits_singles_2.py` & `opengate-10.0b3/opengate/tests/src/test037_pet_hits_singles_2.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
 # check stats
 print()
 gate.warning(f"Check stats")
 # p = paths.gate / "output_test1"
 p = paths.gate / "output"
 stats_ref = gate.read_stat_file(p / f"stats{v}.txt")
-is_ok = gate.assert_stats(stats, stats_ref, 0.025)
+is_ok = gate.assert_stats(stats, stats_ref, 0.03)
 
 # check root hits
 hc = output.get_actor("Hits").user_info
 f = p / f"output{v}.root"
 is_ok = check_root_hits(paths, v, f, hc.output) and is_ok
 
 # check root singles
```

### Comparing `opengate-10.0b2/opengate/tests/src/test037_pet_hits_singles_helpers.py` & `opengate-10.0b3/opengate/tests/src/test037_pet_hits_singles_helpers.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test038_gan_phsp_spect_gan_MT.py` & `opengate-10.0b3/opengate/tests/src/test038_gan_phsp_spect_gan_MT.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test038_gan_phsp_spect_gan_aa.py` & `opengate-10.0b3/opengate/tests/src/test038_gan_phsp_spect_gan_aa.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test038_gan_phsp_spect_gan_helpers.py` & `opengate-10.0b3/opengate/tests/src/test038_gan_phsp_spect_gan_helpers.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test038_gan_phsp_spect_gan_se.py` & `opengate-10.0b3/opengate/tests/src/test038_gan_phsp_spect_gan_se.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test038_gan_phsp_spect_gan_ze.py` & `opengate-10.0b3/opengate/tests/src/test038_gan_phsp_spect_gan_ze.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test038_gan_phsp_spect_training_dataset.py` & `opengate-10.0b3/opengate/tests/src/test038_gan_phsp_spect_training_dataset.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test039_hits_memory_check_helpers.py` & `opengate-10.0b3/opengate/tests/src/test039_hits_memory_check_helpers.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test040_gan_phsp_pet_aref.py` & `opengate-10.0b3/opengate/tests/src/test040_gan_phsp_pet_aref.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test040_gan_phsp_pet_gan.py` & `opengate-10.0b3/opengate/tests/src/test040_gan_phsp_pet_gan.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test040_gan_phsp_pet_training_dataset.py` & `opengate-10.0b3/opengate/tests/src/test040_gan_phsp_pet_training_dataset.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test041_dose_actor.py` & `opengate-10.0b3/opengate/tests/src/test041_dose_actor.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test042_gauss_gps.py` & `opengate-10.0b3/opengate/tests/src/test042_gauss_gps.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test043_distances.py` & `opengate-10.0b3/opengate/tests/src/test043_distances.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test043_garf.py` & `opengate-10.0b3/opengate/tests/src/test043_garf.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test043_garf_analog.py` & `opengate-10.0b3/opengate/tests/src/test043_garf_analog.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test043_garf_helpers.py` & `opengate-10.0b3/opengate/tests/src/test043_garf_helpers.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test043_garf_training_dataset.py` & `opengate-10.0b3/opengate/tests/src/test043_garf_training_dataset.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test044_pbs.py` & `opengate-10.0b3/opengate/tests/src/test044_pbs.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test044_pbs_rot_transl.py` & `opengate-10.0b3/opengate/tests/src/test044_pbs_rot_transl.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test044_pbs_source_to_volume.py` & `opengate-10.0b3/opengate/tests/src/test044_pbs_source_to_volume.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test044_pbs_unFocused.py` & `opengate-10.0b3/opengate/tests/src/test044_pbs_unFocused.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test044_pbs_weight.py` & `opengate-10.0b3/opengate/tests/src/test044_pbs_weight.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test045_gan_phsp_pet_gan_helpers.py` & `opengate-10.0b3/opengate/tests/src/test045_gan_phsp_pet_gan_helpers.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test045_speedup.py` & `opengate-10.0b3/opengate/tests/src/test045_speedup.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test045_speedup_all.py` & `opengate-10.0b3/opengate/tests/src/test045_speedup_all.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
     "PostPosition_Y",
     "PostPosition_Z",
     "TotalEnergyDeposit",
     "TrackVolumeCopyNo",
 ]
 tols = [10.0] * len(keys)
 tols[keys.index("GlobalTime")] = 0.04
-tols[keys.index("PostPosition_X")] = 8
+tols[keys.index("PostPosition_X")] = 8.4
 tols[keys.index("PostPosition_Y")] = 13
 tols[keys.index("PostPosition_Z")] = 1.5
 tols[keys.index("TotalEnergyDeposit")] = 0.03
 tols[keys.index("TrackVolumeCopyNo")] = 4.1
 scalings = [1.0] * len(keys)
 scalings[keys.index("GlobalTime")] = 1e-9  # time in ns
 for o in output:
```

### Comparing `opengate-10.0b2/opengate/tests/src/test046_rad.py` & `opengate-10.0b3/opengate/tests/src/test046_rad.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test047_gan_vox_source_cond.py` & `opengate-10.0b3/opengate/tests/src/test047_gan_vox_source_cond.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test047_voxelization.py` & `opengate-10.0b3/opengate/tests/src/test047_voxelization.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test048_split_spect_projections.py` & `opengate-10.0b3/opengate/tests/src/test048_split_spect_projections.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test049_pet_digit_blurring_helpers.py` & `opengate-10.0b3/opengate/tests/src/test049_pet_digit_blurring_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
     p2 = gate.root_compare_param_tree(singles_output, sname, k2)
     # p2.scaling[p2.the_keys.index("GlobalTime")] = 1e-9  # time in ns
     p1.scaling[p1.the_keys.index("time")] = 1e9  # time in ns
     p = gate.root_compare_param(p1.the_keys, paths.output / png_output)
     p.hits_tol = 5  # % tolerance (including the edep zeros)
     p.tols[k1.index("globalPosX")] = 8
     p.tols[k1.index("globalPosY")] = 5
-    p.tols[k1.index("globalPosZ")] = 1.1
+    p.tols[k1.index("globalPosZ")] = 1.2
     p.tols[k1.index("energy")] = 0.0045
     p.tols[k1.index("time")] = 350
 
     is_ok = gate.root_compare4(p1, p2, p)
 
     return is_ok
```

### Comparing `opengate-10.0b2/opengate/tests/src/test049_pet_digit_blurring_v1.py` & `opengate-10.0b3/opengate/tests/src/test049_pet_digit_blurring_v1.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test049_pet_digit_blurring_v2_MT.py` & `opengate-10.0b3/opengate/tests/src/test049_pet_digit_blurring_v2_MT.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test049_pet_digit_blurring_v3.py` & `opengate-10.0b3/opengate/tests/src/test049_pet_digit_blurring_v3.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test049_pet_digit_blurring_v4.py` & `opengate-10.0b3/opengate/tests/src/test049_pet_digit_blurring_v4.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test050_let_actor_letd.py` & `opengate-10.0b3/opengate/tests/src/test050_let_actor_letd.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test051_adder_time_difference.py` & `opengate-10.0b3/opengate/tests/src/test051_adder_time_difference.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate/tests/src/test052_tac_activity_source.py` & `opengate-10.0b3/opengate/tests/src/test052_tac_activity_source.py`

 * *Files identical despite different names*

### Comparing `opengate-10.0b2/opengate.egg-info/PKG-INFO` & `opengate-10.0b3/opengate.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: opengate
-Version: 10.0b2
+Version: 10.0b3
 Summary: Simulation for Medical Physics
 Home-page: https://github.com/OpenGATE/opengate
 Author: Opengate collaboration
 Author-email: david.sarrut@creatis.insa-lyon.fr
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
 
 ![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/OpenGATE/opengate?logo=github)
 [![CI](https://github.com/OpenGATE/opengate/actions/workflows/main.yml/badge.svg)](https://github.com/OpenGATE/opengate/actions/workflows/main.yml)
 [![cirrus CI](https://api.cirrus-ci.com/github/OpenGATE/opengate.svg)](https://cirrus-ci.com/github/OpenGATE/opengate)
 [![Read the Docs](https://img.shields.io/readthedocs/opengate-python?logo=read-the-docs&style=plastic)](https://opengate-python.readthedocs.io/)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/OpenGATE/opengate/master.svg)](https://results.pre-commit.ci/latest/github/OpenGATE/opengate/master)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/OpenGATE/gam-gate/c65a0d55c616748454f066470aa836331eb107ac)
@@ -23,21 +24,28 @@
 See the [User Guide](https://opengate-python.readthedocs.io/en/latest/user_guide.html).
 
 # How to install (short version)
 
 First create an environment (not mandatory but highly advised)
 
 ```
+python -m venv opengate_env
+source opengate_env/bin/activate
+```
+
+or you can use the conda environment.
+
+```
 conda create --name opengate_env python=3.9
 conda activate opengate_env
 ```
 
 **Warning** not available for MacOS Intel with python 3.11 yet.
 
-Then install the package opengate. The package opengate_core is automatically downloaded.
+Then install the package opengate. The package opengate_core is automatically downloaded. opengate_core installs Geant4 v11.1.1 librairies.
 ```
 pip install --upgrade pip
 pip install --pre opengate
 ```
 
 If you already installed the packages and want to upgrade to last version:
 
@@ -46,22 +54,24 @@
 ```
 
 Once installed, you can run all tests:
 ````
 opengate_tests
 ````
 
-All tests are in the folder [here](https://github.com/OpenGATE/opengate/tree/master/opengate/tests/src). Some data (binary files) are stored, for technical reasons, in this git: https://gitlab.in2p3.fr/opengate/tests_data (which is stored as a git submodule).
+All tests are in the folder [here](https://github.com/OpenGATE/opengate/tree/master/opengate/tests/src). Some data (binary files) are stored, for technical reasons, in this git: https://gitlab.in2p3.fr/opengamgate/gam_tests_data (which is stored as a git submodule).
 
 **WARNING** some tests (e.g. test034) needs [gaga-phsp](https://github.com/dsarrut/gaga-phsp) which needs [pytorch](https://pytorch.org/) that cannot really be automatically installed by the previous pip install (at least we dont know how to do). So, in order to run those tests, you will have to install both pytorch and gaga-phsp first with
 ````
 pip install torch
 pip install gaga-phsp
 ````
 
 The documentation is here: https://opengate-python.readthedocs.io/en/latest/user_guide.html
 
 # How to install (long version, for developers)
 
 See the documentation : https://opengate-python.readthedocs.io/en/latest/developer_guide.html#installation-for-developers
 
+WARNING : need [Geant4 11.1.1](https://geant4.web.cern.ch/download/11.1.1.html)
+
```

### Comparing `opengate-10.0b2/opengate.egg-info/SOURCES.txt` & `opengate-10.0b3/opengate.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 CHANGELOG.md
+LICENSE.md
 MANIFEST.in
 README.md
 VERSION
 setup.py
 core/external/fmt/CONTRIBUTING.md
 core/external/fmt/.github/issue_template.md
 core/external/fmt/.github/pull_request_template.md
@@ -131,17 +132,20 @@
 opengate/source/GANSource.py
 opengate/source/GANSourceConditionalGenerator.py
 opengate/source/GANSourceConditionalPairsGenerator.py
 opengate/source/GANSourceDefaultGenerator.py
 opengate/source/GANSourceDefaultPairsGenerator.py
 opengate/source/GenericSource.py
 opengate/source/PencilBeamSource.py
+opengate/source/PhaseSpaceSource.py
+opengate/source/PhaseSpaceSourceGenerator.py
 opengate/source/SourceBase.py
 opengate/source/SourceEngine.py
 opengate/source/SourceManager.py
+opengate/source/TemplateSource.py
 opengate/source/VoxelizedSourceConditionGenerator.py
 opengate/source/VoxelizedSourcePDFSampler.py
 opengate/source/VoxelsSource.py
 opengate/source/__init__.py
 opengate/source/helpers_source.py
 opengate/source/beta_plus_spectra/__init__.py
 opengate/source/beta_plus_spectra/C11/__init__.py
@@ -207,14 +211,15 @@
 opengate/tests/src/test015_iec_phantom_4.py
 opengate/tests/src/test016_bool_volumes.py
 opengate/tests/src/test017_repeater.py
 opengate/tests/src/test018_pet_WIP.py
 opengate/tests/src/test019_linac_phsp.py
 opengate/tests/src/test019_linac_phsp_MT.py
 opengate/tests/src/test019_linac_phsp_helpers.py
+opengate/tests/src/test019_linac_phsp_source.py
 opengate/tests/src/test019_linac_phsp_visu.py
 opengate/tests/src/test020_profiling.py
 opengate/tests/src/test021_voxel_source1.py
 opengate/tests/src/test021_voxel_source2.py
 opengate/tests/src/test021_voxel_source_old_WIP.py
 opengate/tests/src/test022_half_life.py
 opengate/tests/src/test022_half_life_MT.py
@@ -298,8 +303,9 @@
 opengate/tests/src/test049_pet_digit_blurring_helpers.py
 opengate/tests/src/test049_pet_digit_blurring_v1.py
 opengate/tests/src/test049_pet_digit_blurring_v2_MT.py
 opengate/tests/src/test049_pet_digit_blurring_v3.py
 opengate/tests/src/test049_pet_digit_blurring_v4.py
 opengate/tests/src/test050_let_actor_letd.py
 opengate/tests/src/test051_adder_time_difference.py
-opengate/tests/src/test052_tac_activity_source.py
+opengate/tests/src/test052_tac_activity_source.py
+opengate/tests/src/test056_template_source.py
```

### Comparing `opengate-10.0b2/setup.py` & `opengate-10.0b3/setup.py`

 * *Files identical despite different names*

