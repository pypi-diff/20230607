# Comparing `tmp/ase2sprkkr-2.0.3.tar.gz` & `tmp/ase2sprkkr-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ase2sprkkr-2.0.3.tar", last modified: Thu Mar 30 16:26:01 2023, max compression
+gzip compressed data, was "ase2sprkkr-2.0.4.tar", last modified: Wed Jun  7 21:15:52 2023, max compression
```

## Comparing `ase2sprkkr-2.0.3.tar` & `ase2sprkkr-2.0.4.tar`

### file list

```diff
@@ -1,155 +1,159 @@
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-03-30 16:26:01.304369 ase2sprkkr-2.0.3/
--rw-rw-r--   0 logik     (1000) logik     (1000)     1074 2021-09-02 09:12:56.000000 ase2sprkkr-2.0.3/LICENCE
--rw-rw-r--   0 logik     (1000) logik     (1000)      110 2022-03-06 22:35:24.000000 ase2sprkkr-2.0.3/MANIFEST.in
--rw-rw-r--   0 logik     (1000) logik     (1000)     4830 2023-03-30 16:26:01.304369 ase2sprkkr-2.0.3/PKG-INFO
--rw-rw-r--   0 logik     (1000) logik     (1000)     4356 2023-03-30 16:14:13.000000 ase2sprkkr-2.0.3/README.md
--rw-rw-r--   0 logik     (1000) logik     (1000)      104 2021-09-02 09:12:56.000000 ase2sprkkr-2.0.3/pyproject.toml
--rw-rw-r--   0 logik     (1000) logik     (1000)      731 2023-03-30 16:26:01.304369 ase2sprkkr-2.0.3/setup.cfg
--rw-rw-r--   0 logik     (1000) logik     (1000)      256 2022-03-25 10:06:59.000000 ase2sprkkr-2.0.3/setup.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-03-30 16:26:01.276369 ase2sprkkr-2.0.3/src/
--rw-rw-r--   0 logik     (1000) logik     (1000)        0 2021-02-10 09:12:38.000000 ase2sprkkr-2.0.3/src/MANIFEST.in
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-03-30 16:26:01.276369 ase2sprkkr-2.0.3/src/ase2sprkkr/
--rw-rw-r--   0 logik     (1000) logik     (1000)      655 2022-03-25 10:06:59.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/__init__.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-03-30 16:26:01.276369 ase2sprkkr-2.0.3/src/ase2sprkkr/ase/
--rw-rw-r--   0 logik     (1000) logik     (1000)        0 2023-02-11 17:57:59.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/ase/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     8263 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/ase/build.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      286 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/ase/pbc.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     1311 2023-02-20 17:22:04.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/ase/symbols.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2373 2023-02-11 17:57:59.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/ase/visualise.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-03-30 16:26:01.276369 ase2sprkkr-2.0.3/src/ase2sprkkr/bindings/
--rw-rw-r--   0 logik     (1000) logik     (1000)       86 2023-01-27 00:17:47.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/bindings/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     4892 2023-03-30 15:12:03.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/bindings/es_finder.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     8391 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/bindings/spglib.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-03-30 16:26:01.280369 ase2sprkkr-2.0.3/src/ase2sprkkr/common/
--rw-rw-r--   0 logik     (1000) logik     (1000)       66 2022-03-06 17:00:17.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/common/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     1097 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/common/alternative_types.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     5389 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/common/configuration.py
--rw-rw-r--   0 logik     (1000) logik     (1000)    17525 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/common/configuration_containers.py
--rw-rw-r--   0 logik     (1000) logik     (1000)    42000 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/common/configuration_definitions.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     9642 2023-03-30 15:12:03.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/common/decorators.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     1348 2023-03-30 15:12:03.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/common/directory.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      512 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/common/doc.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     1114 2023-01-27 00:17:47.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/common/formats.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2858 2022-12-05 17:02:51.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/common/grammar.py
--rw-rw-r--   0 logik     (1000) logik     (1000)    46421 2023-03-30 15:12:03.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/common/grammar_types.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2804 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/common/init_tests.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     1608 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/common/misc.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2221 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/common/no_output.py
--rw-rw-r--   0 logik     (1000) logik     (1000)    14102 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/common/options.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     6382 2022-09-04 15:14:59.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/common/process_output_reader.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-03-30 16:26:01.280369 ase2sprkkr-2.0.3/src/ase2sprkkr/common/test/
--rw-rw-r--   0 logik     (1000) logik     (1000)        0 2022-03-06 22:35:24.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/common/test/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2804 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/common/test/init_tests.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2893 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/common/test/test_common.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     8125 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/common/test/test_grammar_types.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     6798 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/common/unique_values.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-03-30 16:26:01.280369 ase2sprkkr-2.0.3/src/ase2sprkkr/input_parameters/
--rw-rw-r--   0 logik     (1000) logik     (1000)       78 2022-03-06 22:35:24.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/input_parameters/__init__.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-03-30 16:26:01.284369 ase2sprkkr-2.0.3/src/ase2sprkkr/input_parameters/definitions/
--rw-rw-r--   0 logik     (1000) logik     (1000)      369 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/input_parameters/definitions/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     5030 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/input_parameters/definitions/arpes.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      690 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/input_parameters/definitions/dos.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      659 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/input_parameters/definitions/phagen.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      746 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/input_parameters/definitions/scf.py
--rw-rw-r--   0 logik     (1000) logik     (1000)    10422 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/input_parameters/definitions/sections.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-03-30 16:26:01.284369 ase2sprkkr-2.0.3/src/ase2sprkkr/input_parameters/examples/
--rw-rw-r--   0 logik     (1000) logik     (1000)      726 2022-03-06 17:00:17.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/input_parameters/examples/arpes.in
--rw-rw-r--   0 logik     (1000) logik     (1000)      210 2022-03-06 17:00:17.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/input_parameters/examples/dos.in
--rw-rw-r--   0 logik     (1000) logik     (1000)      266 2022-03-06 17:00:17.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/input_parameters/examples/phagen.in
--rw-rw-r--   0 logik     (1000) logik     (1000)      276 2022-03-06 17:00:17.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/input_parameters/examples/scf.in
--rw-rw-r--   0 logik     (1000) logik     (1000)    13368 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/input_parameters/input_parameters.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     4541 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/input_parameters/input_parameters_definitions.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-03-30 16:26:01.284369 ase2sprkkr-2.0.3/src/ase2sprkkr/input_parameters/test/
--rw-rw-r--   0 logik     (1000) logik     (1000)        0 2022-03-06 17:00:17.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/input_parameters/test/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2804 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/input_parameters/test/init_tests.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2046 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/input_parameters/test/test_definitions.py
--rw-rw-r--   0 logik     (1000) logik     (1000)    12452 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/input_parameters/test/test_input_parameters.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-03-30 16:26:01.284369 ase2sprkkr-2.0.3/src/ase2sprkkr/outputs/
--rw-rw-r--   0 logik     (1000) logik     (1000)       67 2022-03-14 23:27:47.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/outputs/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2128 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/outputs/output_definitions.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-03-30 16:26:01.284369 ase2sprkkr-2.0.3/src/ase2sprkkr/outputs/readers/
--rw-rw-r--   0 logik     (1000) logik     (1000)       50 2022-03-14 23:27:47.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/outputs/readers/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      295 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/outputs/readers/default.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     8303 2023-03-30 15:12:03.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/outputs/readers/scf.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     1649 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/outputs/task_result.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-03-30 16:26:01.284369 ase2sprkkr-2.0.3/src/ase2sprkkr/outputs/test/
--rw-rw-r--   0 logik     (1000) logik     (1000)        0 2022-03-11 17:30:24.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/outputs/test/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2804 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/outputs/test/init_tests.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      985 2022-03-06 22:35:24.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/outputs/test/test_output.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-03-30 16:26:01.288369 ase2sprkkr-2.0.3/src/ase2sprkkr/physics/
--rw-rw-r--   0 logik     (1000) logik     (1000)      101 2023-01-27 00:17:47.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/physics/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     9561 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/physics/lattice_data.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     1865 2023-03-30 15:12:03.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/physics/winger_seitz_radii.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-03-30 16:26:01.288369 ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/
--rw-rw-r--   0 logik     (1000) logik     (1000)       84 2022-03-06 22:35:24.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2989 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/custom_potential_section.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-03-30 16:26:01.288369 ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/definitions/
--rw-rw-r--   0 logik     (1000) logik     (1000)      334 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/definitions/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     3186 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/definitions/potential.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-03-30 16:26:01.292369 ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/definitions/sections/
--rw-rw-r--   0 logik     (1000) logik     (1000)      531 2022-03-11 17:30:24.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/definitions/sections/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      900 2022-09-04 19:42:44.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/definitions/sections/global_system_parameter.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     7295 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/definitions/sections/lattice.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      998 2022-09-04 19:42:44.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/definitions/sections/mesh_information.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2748 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/definitions/sections/occupation.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     1326 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/definitions/sections/reference_system.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2012 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/definitions/sections/sites.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      833 2022-09-04 19:42:44.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/definitions/sections/types.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-03-30 16:26:01.296369 ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/examples/
--rw-rw-r--   0 logik     (1000) logik     (1000)   265591 2022-03-06 22:35:24.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/examples/FePt.new.pot
--rw-rw-r--   0 logik     (1000) logik     (1000)     3894 2022-03-06 22:35:24.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/examples/FePt.pot
--rw-rw-r--   0 logik     (1000) logik     (1000)    22581 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/examples/GeTe.pot
--rw-rw-r--   0 logik     (1000) logik     (1000)   263365 2022-03-06 22:35:24.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/examples/Li_scf.new.pot
--rw-rw-r--   0 logik     (1000) logik     (1000)     9591 2022-03-06 22:35:24.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/examples/fp_basscale0.pot
--rw-rw-r--   0 logik     (1000) logik     (1000)   395148 2022-03-06 22:35:24.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/examples/fp_new.pot
--rw-rw-r--   0 logik     (1000) logik     (1000)     5137 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/potential_definitions.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     5236 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/potential_sections.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     4062 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/potentials.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-03-30 16:26:01.300369 ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/test/
--rw-rw-r--   0 logik     (1000) logik     (1000)        0 2022-03-06 22:35:24.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/test/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2804 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/test/init_tests.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     1156 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/test/test_2D.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2135 2022-03-06 22:35:24.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/test/test_custom_section.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     3880 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/test/test_potential.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     1334 2022-09-04 19:42:44.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/test/test_structure.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-03-30 16:26:01.300369 ase2sprkkr-2.0.3/src/ase2sprkkr/sprkkr/
--rw-rw-r--   0 logik     (1000) logik     (1000)      112 2022-03-06 17:00:17.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/sprkkr/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     6553 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/sprkkr/atomic_types.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     5136 2023-03-30 15:12:03.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/sprkkr/atoms_region.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     3799 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/sprkkr/build.py
--rw-rw-r--   0 logik     (1000) logik     (1000)    33787 2023-03-30 15:12:03.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/sprkkr/calculator.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     4381 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/sprkkr/configuration.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2210 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/sprkkr/io_data.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     7669 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/sprkkr/occupations.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      912 2022-03-14 23:27:47.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/sprkkr/radial_meshes.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      328 2022-03-14 23:18:04.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/sprkkr/reference_systems.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     5323 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/sprkkr/sites.py
--rw-rw-r--   0 logik     (1000) logik     (1000)    13056 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/sprkkr/sprkkr_atoms.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      802 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/sprkkr/sprkkr_grammar_types.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     5647 2023-02-11 17:57:59.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/sprkkr/structure.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     7511 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/sprkkr/sysfile.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-03-30 16:26:01.300369 ase2sprkkr-2.0.3/src/ase2sprkkr/sprkkr/test/
--rw-rw-r--   0 logik     (1000) logik     (1000)        0 2022-03-06 22:35:24.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/sprkkr/test/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2804 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/sprkkr/test/init_tests.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      676 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/sprkkr/test/test_build.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     6989 2023-03-30 15:12:03.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/sprkkr/test/test_calculator.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     1965 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/sprkkr/test/test_sites.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     3824 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/sprkkr/test/test_sprkkr_atoms.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2537 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/sprkkr/test/test_sysfile.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-03-30 16:26:01.300369 ase2sprkkr-2.0.3/src/ase2sprkkr/tools/
--rw-rw-r--   0 logik     (1000) logik     (1000)       55 2022-03-14 23:27:47.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/tools/__init__.py
--rwxrwxr-x   0 logik     (1000) logik     (1000)     2632 2023-02-11 17:57:59.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/tools/a2s_visualise_in_struct.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-03-30 16:26:01.304369 ase2sprkkr-2.0.3/src/ase2sprkkr/tools/test/
--rw-rw-r--   0 logik     (1000) logik     (1000)        0 2023-02-11 17:57:59.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/tools/test/__init__.py
--rw-rw-r--   0 logik     (1000) logik     (1000)     2804 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/tools/test/init_tests.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      750 2023-02-11 17:57:59.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/tools/test/test_tools.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      150 2023-03-30 16:18:17.000000 ase2sprkkr-2.0.3/src/ase2sprkkr/version.py
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-03-30 16:26:01.276369 ase2sprkkr-2.0.3/src/ase2sprkkr.egg-info/
--rw-rw-r--   0 logik     (1000) logik     (1000)     4830 2023-03-30 16:26:01.000000 ase2sprkkr-2.0.3/src/ase2sprkkr.egg-info/PKG-INFO
--rw-rw-r--   0 logik     (1000) logik     (1000)     5253 2023-03-30 16:26:01.000000 ase2sprkkr-2.0.3/src/ase2sprkkr.egg-info/SOURCES.txt
--rw-rw-r--   0 logik     (1000) logik     (1000)        1 2023-03-30 16:26:01.000000 ase2sprkkr-2.0.3/src/ase2sprkkr.egg-info/dependency_links.txt
--rw-rw-r--   0 logik     (1000) logik     (1000)       31 2023-03-30 16:26:01.000000 ase2sprkkr-2.0.3/src/ase2sprkkr.egg-info/requires.txt
--rw-rw-r--   0 logik     (1000) logik     (1000)       11 2023-03-30 16:26:01.000000 ase2sprkkr-2.0.3/src/ase2sprkkr.egg-info/top_level.txt
-drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-03-30 16:26:01.304369 ase2sprkkr-2.0.3/tests/
--rw-rw-r--   0 logik     (1000) logik     (1000)     2838 2021-09-02 09:12:56.000000 ase2sprkkr-2.0.3/tests/test.py
--rw-rw-r--   0 logik     (1000) logik     (1000)      468 2021-09-02 09:12:56.000000 ase2sprkkr-2.0.3/tests/test_inputfile.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.903179 ase2sprkkr-2.0.4/
+-rw-rw-r--   0 logik     (1000) logik     (1000)     1074 2021-09-02 09:12:56.000000 ase2sprkkr-2.0.4/LICENCE
+-rw-rw-r--   0 logik     (1000) logik     (1000)      110 2022-03-06 22:35:24.000000 ase2sprkkr-2.0.4/MANIFEST.in
+-rw-rw-r--   0 logik     (1000) logik     (1000)     4830 2023-06-07 21:15:52.903179 ase2sprkkr-2.0.4/PKG-INFO
+-rw-rw-r--   0 logik     (1000) logik     (1000)     4356 2023-03-30 16:14:13.000000 ase2sprkkr-2.0.4/README.md
+-rw-rw-r--   0 logik     (1000) logik     (1000)      104 2021-09-02 09:12:56.000000 ase2sprkkr-2.0.4/pyproject.toml
+-rw-rw-r--   0 logik     (1000) logik     (1000)      731 2023-06-07 21:15:52.907179 ase2sprkkr-2.0.4/setup.cfg
+-rw-rw-r--   0 logik     (1000) logik     (1000)      256 2023-06-07 19:13:11.000000 ase2sprkkr-2.0.4/setup.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.891179 ase2sprkkr-2.0.4/src/
+-rw-rw-r--   0 logik     (1000) logik     (1000)        0 2021-02-10 09:12:38.000000 ase2sprkkr-2.0.4/src/MANIFEST.in
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.891179 ase2sprkkr-2.0.4/src/ase2sprkkr/
+-rw-rw-r--   0 logik     (1000) logik     (1000)      817 2023-06-07 17:36:39.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/__init__.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.895179 ase2sprkkr-2.0.4/src/ase2sprkkr/ase/
+-rw-rw-r--   0 logik     (1000) logik     (1000)        0 2023-02-11 17:57:59.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/ase/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     8263 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/ase/build.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      286 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/ase/pbc.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     1311 2023-02-20 17:22:04.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/ase/symbols.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2373 2023-02-11 17:57:59.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/ase/visualise.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.895179 ase2sprkkr-2.0.4/src/ase2sprkkr/asr/
+-rw-rw-r--   0 logik     (1000) logik     (1000)       43 2023-06-07 20:32:19.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/asr/__init__.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.895179 ase2sprkkr-2.0.4/src/ase2sprkkr/bindings/
+-rw-rw-r--   0 logik     (1000) logik     (1000)       86 2023-01-27 00:17:47.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/bindings/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     4892 2023-03-30 15:12:03.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/bindings/es_finder.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     8391 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/bindings/spglib.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.895179 ase2sprkkr-2.0.4/src/ase2sprkkr/common/
+-rw-rw-r--   0 logik     (1000) logik     (1000)       66 2022-03-06 17:00:17.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/common/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     1097 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/common/alternative_types.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     5389 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/common/configuration.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)    17525 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/common/configuration_containers.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)    42000 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/common/configuration_definitions.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     9642 2023-03-30 15:12:03.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/common/decorators.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     1348 2023-03-30 15:12:03.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/common/directory.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      512 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/common/doc.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     1114 2023-01-27 00:17:47.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/common/formats.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2858 2022-12-05 17:02:51.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/common/grammar.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)    46421 2023-03-30 15:12:03.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/common/grammar_types.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2804 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/common/init_tests.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     1608 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/common/misc.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2221 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/common/no_output.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)    14102 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/common/options.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     6382 2022-09-04 15:14:59.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/common/process_output_reader.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.895179 ase2sprkkr-2.0.4/src/ase2sprkkr/common/test/
+-rw-rw-r--   0 logik     (1000) logik     (1000)        0 2022-03-06 22:35:24.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/common/test/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2804 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/common/test/init_tests.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2893 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/common/test/test_common.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     8125 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/common/test/test_grammar_types.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     6798 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/common/unique_values.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.899179 ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/
+-rw-rw-r--   0 logik     (1000) logik     (1000)       78 2022-03-06 22:35:24.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/__init__.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.899179 ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/definitions/
+-rw-rw-r--   0 logik     (1000) logik     (1000)      369 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/definitions/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     5030 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/definitions/arpes.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      690 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/definitions/dos.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      659 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/definitions/phagen.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      746 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/definitions/scf.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)    10422 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/definitions/sections.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.899179 ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/examples/
+-rw-rw-r--   0 logik     (1000) logik     (1000)      726 2022-03-06 17:00:17.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/examples/arpes.in
+-rw-rw-r--   0 logik     (1000) logik     (1000)      210 2022-03-06 17:00:17.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/examples/dos.in
+-rw-rw-r--   0 logik     (1000) logik     (1000)      266 2022-03-06 17:00:17.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/examples/phagen.in
+-rw-rw-r--   0 logik     (1000) logik     (1000)      276 2022-03-06 17:00:17.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/examples/scf.in
+-rw-rw-r--   0 logik     (1000) logik     (1000)    13368 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/input_parameters.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     4541 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/input_parameters_definitions.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.899179 ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/test/
+-rw-rw-r--   0 logik     (1000) logik     (1000)        0 2022-03-06 17:00:17.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/test/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2804 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/test/init_tests.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2046 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/test/test_definitions.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)    12452 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/test/test_input_parameters.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.899179 ase2sprkkr-2.0.4/src/ase2sprkkr/outputs/
+-rw-rw-r--   0 logik     (1000) logik     (1000)       67 2022-03-14 23:27:47.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/outputs/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2128 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/outputs/output_definitions.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.899179 ase2sprkkr-2.0.4/src/ase2sprkkr/outputs/readers/
+-rw-rw-r--   0 logik     (1000) logik     (1000)       50 2022-03-14 23:27:47.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/outputs/readers/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      295 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/outputs/readers/default.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     8303 2023-03-30 15:12:03.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/outputs/readers/scf.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     1649 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/outputs/task_result.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.899179 ase2sprkkr-2.0.4/src/ase2sprkkr/outputs/test/
+-rw-rw-r--   0 logik     (1000) logik     (1000)        0 2022-03-11 17:30:24.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/outputs/test/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2804 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/outputs/test/init_tests.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      985 2022-03-06 22:35:24.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/outputs/test/test_output.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.899179 ase2sprkkr-2.0.4/src/ase2sprkkr/physics/
+-rw-rw-r--   0 logik     (1000) logik     (1000)      101 2023-01-27 00:17:47.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/physics/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     9561 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/physics/lattice_data.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     1865 2023-03-30 15:12:03.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/physics/winger_seitz_radii.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.899179 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/
+-rw-rw-r--   0 logik     (1000) logik     (1000)       84 2022-03-06 22:35:24.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2989 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/custom_potential_section.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.899179 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/definitions/
+-rw-rw-r--   0 logik     (1000) logik     (1000)      334 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/definitions/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     3186 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/definitions/potential.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.903179 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/definitions/sections/
+-rw-rw-r--   0 logik     (1000) logik     (1000)      531 2022-03-11 17:30:24.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/definitions/sections/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      900 2022-09-04 19:42:44.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/definitions/sections/global_system_parameter.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     7295 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/definitions/sections/lattice.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      998 2022-09-04 19:42:44.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/definitions/sections/mesh_information.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2748 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/definitions/sections/occupation.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     1326 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/definitions/sections/reference_system.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2012 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/definitions/sections/sites.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      833 2022-09-04 19:42:44.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/definitions/sections/types.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.903179 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/examples/
+-rw-rw-r--   0 logik     (1000) logik     (1000)   265591 2022-03-06 22:35:24.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/examples/FePt.new.pot
+-rw-rw-r--   0 logik     (1000) logik     (1000)     3894 2022-03-06 22:35:24.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/examples/FePt.pot
+-rw-rw-r--   0 logik     (1000) logik     (1000)    22581 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/examples/GeTe.pot
+-rw-rw-r--   0 logik     (1000) logik     (1000)   263365 2022-03-06 22:35:24.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/examples/Li_scf.new.pot
+-rw-rw-r--   0 logik     (1000) logik     (1000)     9591 2022-03-06 22:35:24.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/examples/fp_basscale0.pot
+-rw-rw-r--   0 logik     (1000) logik     (1000)   395148 2022-03-06 22:35:24.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/examples/fp_new.pot
+-rw-rw-r--   0 logik     (1000) logik     (1000)     5137 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/potential_definitions.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     5236 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/potential_sections.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     4062 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/potentials.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.903179 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/test/
+-rw-rw-r--   0 logik     (1000) logik     (1000)        0 2022-03-06 22:35:24.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/test/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2804 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/test/init_tests.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     1156 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/test/test_2D.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2135 2022-03-06 22:35:24.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/test/test_custom_section.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     3880 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/test/test_potential.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     1334 2022-09-04 19:42:44.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/test/test_structure.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.903179 ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/
+-rw-rw-r--   0 logik     (1000) logik     (1000)      112 2022-03-06 17:00:17.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     6553 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/atomic_types.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     5136 2023-03-30 15:12:03.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/atoms_region.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     3799 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/build.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)    33787 2023-03-30 15:12:03.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/calculator.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     4381 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/configuration.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2210 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/io_data.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     7669 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/occupations.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      912 2022-03-14 23:27:47.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/radial_meshes.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      328 2022-03-14 23:18:04.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/reference_systems.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     5323 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/sites.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)    13056 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/sprkkr_atoms.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      802 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/sprkkr_grammar_types.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     5647 2023-02-11 17:57:59.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/structure.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     7511 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/sysfile.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.903179 ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/test/
+-rw-rw-r--   0 logik     (1000) logik     (1000)        0 2022-03-06 22:35:24.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/test/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2804 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/test/init_tests.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      676 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/test/test_build.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     6989 2023-03-30 15:12:03.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/test/test_calculator.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     1965 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/test/test_sites.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     3824 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/test/test_sprkkr_atoms.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2537 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/test/test_sysfile.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.903179 ase2sprkkr-2.0.4/src/ase2sprkkr/tools/
+-rw-rw-r--   0 logik     (1000) logik     (1000)       55 2022-03-14 23:27:47.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/tools/__init__.py
+-rwxrwxr-x   0 logik     (1000) logik     (1000)     2632 2023-02-11 17:57:59.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/tools/a2s_visualise_in_struct.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.903179 ase2sprkkr-2.0.4/src/ase2sprkkr/tools/test/
+-rw-rw-r--   0 logik     (1000) logik     (1000)        0 2023-02-11 17:57:59.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/tools/test/__init__.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2804 2023-03-28 14:31:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/tools/test/init_tests.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      750 2023-02-11 17:57:59.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/tools/test/test_tools.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      150 2023-06-07 21:12:07.000000 ase2sprkkr-2.0.4/src/ase2sprkkr/version.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.895179 ase2sprkkr-2.0.4/src/ase2sprkkr.egg-info/
+-rw-rw-r--   0 logik     (1000) logik     (1000)     4830 2023-06-07 21:15:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr.egg-info/PKG-INFO
+-rw-rw-r--   0 logik     (1000) logik     (1000)     5307 2023-06-07 21:15:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr.egg-info/SOURCES.txt
+-rw-rw-r--   0 logik     (1000) logik     (1000)        1 2023-06-07 21:15:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr.egg-info/dependency_links.txt
+-rw-rw-r--   0 logik     (1000) logik     (1000)       31 2023-06-07 21:15:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr.egg-info/requires.txt
+-rw-rw-r--   0 logik     (1000) logik     (1000)       18 2023-06-07 21:15:52.000000 ase2sprkkr-2.0.4/src/ase2sprkkr.egg-info/top_level.txt
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.903179 ase2sprkkr-2.0.4/src/sprkkr/
+-rw-rw-r--   0 logik     (1000) logik     (1000)       40 2023-06-07 19:12:36.000000 ase2sprkkr-2.0.4/src/sprkkr/__init__.py
+drwxrwxr-x   0 logik     (1000) logik     (1000)        0 2023-06-07 21:15:52.903179 ase2sprkkr-2.0.4/tests/
+-rw-rw-r--   0 logik     (1000) logik     (1000)     2838 2021-09-02 09:12:56.000000 ase2sprkkr-2.0.4/tests/test.py
+-rw-rw-r--   0 logik     (1000) logik     (1000)      468 2021-09-02 09:12:56.000000 ase2sprkkr-2.0.4/tests/test_inputfile.py
```

### Comparing `ase2sprkkr-2.0.3/LICENCE` & `ase2sprkkr-2.0.4/LICENCE`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/PKG-INFO` & `ase2sprkkr-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ase2sprkkr
-Version: 2.0.3
+Version: 2.0.4
 Summary: ASE (atomic simulation environment) interface to SPRKKR
 Home-page: https://ase2sprkkr.github.io/ase2sprkkr/
 Author: Matyáš Novák & Jano Minár
 Author-email: ase2kkr@ntc.zcu.cz
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ase2sprkkr-2.0.3/README.md` & `ase2sprkkr-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/setup.cfg` & `ase2sprkkr-2.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/__init__.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,7 +14,15 @@
 from .potentials.potentials import Potential
 
 """ An extension of ASE atoms object """
 from .sprkkr.sprkkr_atoms import SPRKKRAtoms
 
 """ Version of the package """
 from .version import __version__
+
+def _init():
+   import ase
+   from ase.calculators.calculator import register_calculator_class
+   register_calculator_class('sprkkr', SPRKKR)
+
+_init()
+del _init
```

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/ase/build.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/ase/build.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/ase/symbols.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/ase/symbols.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/ase/visualise.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/ase/visualise.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/bindings/es_finder.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/bindings/es_finder.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/bindings/spglib.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/bindings/spglib.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/common/alternative_types.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/common/alternative_types.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/common/configuration.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/common/configuration.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/common/configuration_containers.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/common/configuration_containers.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/common/configuration_definitions.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/common/configuration_definitions.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/common/decorators.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/common/decorators.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/common/directory.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/common/directory.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/common/doc.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/common/doc.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/common/formats.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/common/formats.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/common/grammar.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/common/grammar.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/common/grammar_types.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/common/grammar_types.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/common/init_tests.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/common/init_tests.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/common/misc.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/common/misc.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/common/no_output.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/common/no_output.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/common/options.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/common/options.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/common/process_output_reader.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/common/process_output_reader.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/common/test/init_tests.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/common/test/init_tests.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/common/test/test_common.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/common/test/test_common.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/common/test/test_grammar_types.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/common/test/test_grammar_types.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/common/unique_values.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/common/unique_values.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/input_parameters/definitions/arpes.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/definitions/arpes.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/input_parameters/definitions/dos.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/definitions/dos.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/input_parameters/definitions/phagen.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/definitions/phagen.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/input_parameters/definitions/scf.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/definitions/scf.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/input_parameters/definitions/sections.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/definitions/sections.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/input_parameters/examples/arpes.in` & `ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/examples/arpes.in`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/input_parameters/input_parameters.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/input_parameters.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/input_parameters/input_parameters_definitions.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/input_parameters_definitions.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/input_parameters/test/init_tests.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/test/init_tests.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/input_parameters/test/test_definitions.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/test/test_definitions.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/input_parameters/test/test_input_parameters.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/input_parameters/test/test_input_parameters.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/outputs/output_definitions.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/outputs/output_definitions.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/outputs/readers/scf.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/outputs/readers/scf.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/outputs/task_result.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/outputs/task_result.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/outputs/test/init_tests.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/outputs/test/init_tests.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/outputs/test/test_output.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/outputs/test/test_output.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/physics/lattice_data.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/physics/lattice_data.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/physics/winger_seitz_radii.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/physics/winger_seitz_radii.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/custom_potential_section.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/custom_potential_section.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/definitions/potential.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/definitions/potential.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/definitions/sections/__init__.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/definitions/sections/__init__.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/definitions/sections/global_system_parameter.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/definitions/sections/global_system_parameter.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/definitions/sections/lattice.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/definitions/sections/lattice.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/definitions/sections/mesh_information.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/definitions/sections/mesh_information.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/definitions/sections/occupation.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/definitions/sections/occupation.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/definitions/sections/reference_system.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/definitions/sections/reference_system.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/definitions/sections/sites.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/definitions/sections/sites.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/definitions/sections/types.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/definitions/sections/types.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/examples/FePt.new.pot` & `ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/examples/FePt.new.pot`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/examples/FePt.pot` & `ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/examples/FePt.pot`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/examples/GeTe.pot` & `ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/examples/GeTe.pot`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/examples/Li_scf.new.pot` & `ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/examples/Li_scf.new.pot`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/examples/fp_basscale0.pot` & `ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/examples/fp_basscale0.pot`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/examples/fp_new.pot` & `ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/examples/fp_new.pot`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/potential_definitions.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/potential_definitions.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/potential_sections.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/potential_sections.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/potentials.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/potentials.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/test/init_tests.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/test/init_tests.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/test/test_2D.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/test/test_2D.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/test/test_custom_section.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/test/test_custom_section.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/test/test_potential.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/test/test_potential.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/potentials/test/test_structure.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/potentials/test/test_structure.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/sprkkr/atomic_types.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/atomic_types.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/sprkkr/atoms_region.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/atoms_region.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/sprkkr/build.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/build.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/sprkkr/calculator.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/calculator.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/sprkkr/configuration.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/configuration.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/sprkkr/io_data.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/io_data.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/sprkkr/occupations.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/occupations.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/sprkkr/radial_meshes.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/radial_meshes.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/sprkkr/sites.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/sites.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/sprkkr/sprkkr_atoms.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/sprkkr_atoms.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/sprkkr/sprkkr_grammar_types.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/sprkkr_grammar_types.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/sprkkr/structure.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/structure.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/sprkkr/sysfile.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/sysfile.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/sprkkr/test/init_tests.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/test/init_tests.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/sprkkr/test/test_build.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/test/test_build.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/sprkkr/test/test_calculator.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/test/test_calculator.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/sprkkr/test/test_sites.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/test/test_sites.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/sprkkr/test/test_sprkkr_atoms.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/test/test_sprkkr_atoms.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/sprkkr/test/test_sysfile.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/sprkkr/test/test_sysfile.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/tools/a2s_visualise_in_struct.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/tools/a2s_visualise_in_struct.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/tools/test/init_tests.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/tools/test/init_tests.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr/tools/test/test_tools.py` & `ase2sprkkr-2.0.4/src/ase2sprkkr/tools/test/test_tools.py`

 * *Files identical despite different names*

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr.egg-info/PKG-INFO` & `ase2sprkkr-2.0.4/src/ase2sprkkr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ase2sprkkr
-Version: 2.0.3
+Version: 2.0.4
 Summary: ASE (atomic simulation environment) interface to SPRKKR
 Home-page: https://ase2sprkkr.github.io/ase2sprkkr/
 Author: Matyáš Novák & Jano Minár
 Author-email: ase2kkr@ntc.zcu.cz
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ase2sprkkr-2.0.3/src/ase2sprkkr.egg-info/SOURCES.txt` & `ase2sprkkr-2.0.4/src/ase2sprkkr.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 src/ase2sprkkr.egg-info/requires.txt
 src/ase2sprkkr.egg-info/top_level.txt
 src/ase2sprkkr/ase/__init__.py
 src/ase2sprkkr/ase/build.py
 src/ase2sprkkr/ase/pbc.py
 src/ase2sprkkr/ase/symbols.py
 src/ase2sprkkr/ase/visualise.py
+src/ase2sprkkr/asr/__init__.py
 src/ase2sprkkr/bindings/__init__.py
 src/ase2sprkkr/bindings/es_finder.py
 src/ase2sprkkr/bindings/spglib.py
 src/ase2sprkkr/common/__init__.py
 src/ase2sprkkr/common/alternative_types.py
 src/ase2sprkkr/common/configuration.py
 src/ase2sprkkr/common/configuration_containers.py
@@ -120,9 +121,10 @@
 src/ase2sprkkr/sprkkr/test/test_sprkkr_atoms.py
 src/ase2sprkkr/sprkkr/test/test_sysfile.py
 src/ase2sprkkr/tools/__init__.py
 src/ase2sprkkr/tools/a2s_visualise_in_struct.py
 src/ase2sprkkr/tools/test/__init__.py
 src/ase2sprkkr/tools/test/init_tests.py
 src/ase2sprkkr/tools/test/test_tools.py
+src/sprkkr/__init__.py
 tests/test.py
 tests/test_inputfile.py
```

### Comparing `ase2sprkkr-2.0.3/tests/test.py` & `ase2sprkkr-2.0.4/tests/test.py`

 * *Files identical despite different names*

