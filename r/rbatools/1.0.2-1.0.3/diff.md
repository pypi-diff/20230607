# Comparing `tmp/rbatools-1.0.2.tar.gz` & `tmp/rbatools-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rbatools-1.0.2.tar", last modified: Wed Mar 22 13:16:28 2023, max compression
+gzip compressed data, was "dist/rbatools-1.0.3.tar", last modified: Wed Jun  7 11:23:33 2023, max compression
```

## Comparing `rbatools-1.0.2.tar` & `rbatools-1.0.3.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2023-03-22 13:16:28.000000 rbatools-1.0.2/
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     1554 2023-03-22 13:16:28.000000 rbatools-1.0.2/PKG-INFO
-drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2023-03-22 13:16:28.000000 rbatools-1.0.2/rbatools/
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     4566 2022-10-03 13:32:48.000000 rbatools-1.0.2/rbatools/target_block.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     7594 2022-09-16 15:26:00.000000 rbatools-1.0.2/rbatools/macromolecule_block.py
--rwxr-xr-x   0 oliverbodeit   (501) staff       (20)    69585 2022-11-16 13:45:49.000000 rbatools-1.0.2/rbatools/rba_model_structure.py
--rwxr-xr-x   0 oliverbodeit   (501) staff       (20)     6652 2022-09-16 15:26:00.000000 rbatools-1.0.2/rbatools/enzyme_block.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     6925 2023-03-22 13:15:09.000000 rbatools-1.0.2/rbatools/rba_problem_matrix.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)    17550 2022-11-22 21:15:38.000000 rbatools-1.0.2/rbatools/fba_problem.py
--rwxr-xr-x   0 oliverbodeit   (501) staff       (20)     9404 2022-09-26 11:55:01.000000 rbatools-1.0.2/rbatools/protein_block.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)        8 2023-03-22 13:15:29.000000 rbatools-1.0.2/rbatools/_version.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     7953 2022-09-16 15:26:00.000000 rbatools-1.0.2/rbatools/rba_simulation_parameters.py
--rwxr-xr-x   0 oliverbodeit   (501) staff       (20)     1292 2022-09-16 15:26:00.000000 rbatools-1.0.2/rbatools/metabolite_constraint_block.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)    27793 2023-03-22 13:15:09.000000 rbatools-1.0.2/rbatools/rba_problem.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)    44603 2023-03-22 13:15:09.000000 rbatools-1.0.2/rbatools/rba_lp.py
--rwxr-xr-x   0 oliverbodeit   (501) staff       (20)      715 2022-11-24 15:34:09.000000 rbatools-1.0.2/rbatools/__init__.py
--rwxr-xr-x   0 oliverbodeit   (501) staff       (20)     2450 2022-11-23 10:45:57.000000 rbatools-1.0.2/rbatools/statistics_block.py
--rwxr-xr-x   0 oliverbodeit   (501) staff       (20)     3744 2022-09-16 15:26:00.000000 rbatools-1.0.2/rbatools/information_block.py
-drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2023-03-22 13:16:28.000000 rbatools-1.0.2/rbatools/cli/
--rw-r--r--   0 oliverbodeit   (501) staff       (20)        0 2022-10-02 12:32:24.000000 rbatools-1.0.2/rbatools/cli/__init__.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     1227 2022-11-24 15:29:36.000000 rbatools-1.0.2/rbatools/cli/generate_sbtab_of_model_for_html.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     1914 2022-11-24 15:29:57.000000 rbatools-1.0.2/rbatools/cli/run_growth_rate_optimization.py
--rwxr-xr-x   0 oliverbodeit   (501) staff       (20)     8182 2022-09-26 11:55:01.000000 rbatools-1.0.2/rbatools/metabolite_block.py
--rwxr-xr-x   0 oliverbodeit   (501) staff       (20)     1729 2022-09-16 15:26:00.000000 rbatools-1.0.2/rbatools/description_block.py
--rwxr-xr-x   0 oliverbodeit   (501) staff       (20)     5430 2022-09-16 15:26:00.000000 rbatools-1.0.2/rbatools/process_block.py
--rwxr-xr-x   0 oliverbodeit   (501) staff       (20)     2042 2022-09-16 15:26:00.000000 rbatools-1.0.2/rbatools/compartment_block.py
--rwxr-xr-x   0 oliverbodeit   (501) staff       (20)     2419 2022-10-03 13:32:48.000000 rbatools-1.0.2/rbatools/density_constraint_block.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)   115613 2023-03-22 13:15:09.000000 rbatools-1.0.2/rbatools/rba_session.py
--rwxr-xr-x   0 oliverbodeit   (501) staff       (20)     2808 2022-10-03 13:32:48.000000 rbatools-1.0.2/rbatools/enzyme_constraint_block.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)      147 2022-09-16 15:26:00.000000 rbatools-1.0.2/rbatools/_warnings_and_errors.py
--rwxr-xr-x   0 oliverbodeit   (501) staff       (20)     3123 2022-10-03 13:32:48.000000 rbatools-1.0.2/rbatools/process_constraint_block.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)       54 2022-10-02 12:32:24.000000 rbatools-1.0.2/rbatools/_authors.py
--rwxr-xr-x   0 oliverbodeit   (501) staff       (20)    14244 2022-09-26 11:55:01.000000 rbatools-1.0.2/rbatools/reaction_block.py
--rwxr-xr-x   0 oliverbodeit   (501) staff       (20)     6904 2022-09-16 15:26:00.000000 rbatools-1.0.2/rbatools/info_matrix.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)    25488 2023-03-22 13:15:09.000000 rbatools-1.0.2/rbatools/_auxiliary_functions.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     1500 2022-09-16 15:26:00.000000 rbatools-1.0.2/rbatools/parameter_block.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     2096 2022-09-16 15:26:00.000000 rbatools-1.0.2/rbatools/data_block.py
--rwxr-xr-x   0 oliverbodeit   (501) staff       (20)    49501 2022-11-23 14:00:52.000000 rbatools-1.0.2/rbatools/rba_simulation_data.py
--rwxr-xr-x   0 oliverbodeit   (501) staff       (20)     1707 2022-09-16 15:26:00.000000 rbatools-1.0.2/rbatools/module_block.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)        3 2022-10-02 12:32:24.000000 rbatools-1.0.2/rbatools/_credits.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)       78 2022-11-23 10:49:46.000000 rbatools-1.0.2/requirements.txt
-drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2023-03-22 13:16:28.000000 rbatools-1.0.2/rbatools.egg-info/
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     1554 2023-03-22 13:16:28.000000 rbatools-1.0.2/rbatools.egg-info/PKG-INFO
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     4367 2023-03-22 13:16:28.000000 rbatools-1.0.2/rbatools.egg-info/SOURCES.txt
--rw-r--r--   0 oliverbodeit   (501) staff       (20)      183 2023-03-22 13:16:28.000000 rbatools-1.0.2/rbatools.egg-info/entry_points.txt
--rw-r--r--   0 oliverbodeit   (501) staff       (20)       44 2023-03-22 13:16:28.000000 rbatools-1.0.2/rbatools.egg-info/requires.txt
--rw-r--r--   0 oliverbodeit   (501) staff       (20)        9 2023-03-22 13:16:28.000000 rbatools-1.0.2/rbatools.egg-info/top_level.txt
--rw-r--r--   0 oliverbodeit   (501) staff       (20)        1 2023-03-22 13:16:28.000000 rbatools-1.0.2/rbatools.egg-info/dependency_links.txt
--rw-r--r--   0 oliverbodeit   (501) staff       (20)       98 2022-09-26 12:06:09.000000 rbatools-1.0.2/pyproject.toml
--rw-r--r--   0 oliverbodeit   (501) staff       (20)       64 2022-09-26 12:06:09.000000 rbatools-1.0.2/MANIFEST.in
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     5651 2023-03-22 13:15:09.000000 rbatools-1.0.2/README.md
-drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2023-03-22 13:16:28.000000 rbatools-1.0.2/figure_for_manuscript/
--rw-r--r--   0 oliverbodeit   (501) staff       (20)   166885 2023-03-22 13:15:09.000000 rbatools-1.0.2/figure_for_manuscript/LocalSensitivities_all_enzymes_1percent.csv
--rw-r--r--   0 oliverbodeit   (501) staff       (20)    50612 2023-03-22 13:15:09.000000 rbatools-1.0.2/figure_for_manuscript/Figures_reviewed_article.ipynb
--rw-r--r--   0 oliverbodeit   (501) staff       (20)   105593 2023-03-22 13:15:09.000000 rbatools-1.0.2/figure_for_manuscript/LocalSensitivitiesEnzymes_001.csv
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     2996 2023-02-24 20:41:19.000000 rbatools-1.0.2/setup.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     1218 2022-11-24 13:00:21.000000 rbatools-1.0.2/.gitignore
-drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2023-03-22 13:16:28.000000 rbatools-1.0.2/scripts/
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     1227 2022-11-24 15:29:36.000000 rbatools-1.0.2/scripts/generate_sbtab_of_model_for_html.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     1914 2022-11-24 15:29:57.000000 rbatools-1.0.2/scripts/run_growth_rate_optimization.py
-drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2023-03-22 13:16:28.000000 rbatools-1.0.2/tutorials/
-drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2023-03-22 13:16:28.000000 rbatools-1.0.2/tutorials/jupyter_notebooks/
--rw-r--r--   0 oliverbodeit   (501) staff       (20)    10992 2023-03-22 13:15:09.000000 rbatools-1.0.2/tutorials/jupyter_notebooks/Linear_optimization_with_rbatools.ipynb
-drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2023-03-22 13:16:28.000000 rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/
--rw-r--r--   0 oliverbodeit   (501) staff       (20)      485 2023-03-22 13:15:10.000000 rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/sample_model_loader.py
-drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2023-03-22 13:16:28.000000 rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     3118 2023-03-22 13:15:10.000000 rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/rnas.xml
--rw-r--r--   0 oliverbodeit   (501) staff       (20)      802 2023-03-22 13:15:10.000000 rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/dna.xml
--rw-r--r--   0 oliverbodeit   (501) staff       (20)      136 2023-03-22 13:15:09.000000 rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/ModelInformation.csv
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     5404 2023-03-22 13:15:10.000000 rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/targets.xml
--rw-r--r--   0 oliverbodeit   (501) staff       (20)    14641 2023-03-22 13:15:10.000000 rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/enzymes.out
--rw-r--r--   0 oliverbodeit   (501) staff       (20)      240 2023-03-22 13:15:09.000000 rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/density.xml
--rw-r--r--   0 oliverbodeit   (501) staff       (20)  3368922 2023-03-22 13:15:10.000000 rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/uniprot.csv
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     1418 2023-03-22 13:15:10.000000 rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/params.in
--rw-r--r--   0 oliverbodeit   (501) staff       (20)      931 2023-03-22 13:15:10.000000 rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/medium.tsv
--rw-r--r--   0 oliverbodeit   (501) staff       (20)   950277 2023-03-22 13:15:10.000000 rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/proteins.xml
--rw-r--r--   0 oliverbodeit   (501) staff       (20)   231014 2023-03-22 13:15:10.000000 rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/enzymes.xml
--rw-r--r--   0 oliverbodeit   (501) staff       (20)      177 2023-03-22 13:15:10.000000 rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/process_machineries.out
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     3949 2023-03-22 13:15:09.000000 rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/README.md
--rw-r--r--   0 oliverbodeit   (501) staff       (20)       11 2023-03-22 13:15:09.000000 rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/.gitignore
--rw-r--r--   0 oliverbodeit   (501) staff       (20)  6415232 2023-03-22 13:15:09.000000 rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/ModelStructure.json
--rw-r--r--   0 oliverbodeit   (501) staff       (20)   465910 2023-03-22 13:15:10.000000 rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/sbml.xml
--rw-r--r--   0 oliverbodeit   (501) staff       (20)   348791 2023-03-22 13:15:10.000000 rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/parameters.xml
--rw-r--r--   0 oliverbodeit   (501) staff       (20)   132671 2023-03-22 13:15:10.000000 rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/processes.xml
-drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2023-03-22 13:16:28.000000 rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/data/
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     2108 2023-03-22 13:15:09.000000 rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/data/trnas.fasta
--rw-r--r--   0 oliverbodeit   (501) staff       (20)  3368922 2023-03-22 13:15:09.000000 rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/data/uniprot.csv
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     2956 2023-03-22 13:15:09.000000 rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/data/chaperones.fasta
--rw-r--r--   0 oliverbodeit   (501) staff       (20)    20988 2023-03-22 13:15:09.000000 rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/data/catalytic_activity_medium_2.csv
--rw-r--r--   0 oliverbodeit   (501) staff       (20)   465910 2023-03-22 13:15:09.000000 rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/data/sbml.xml
--rw-r--r--   0 oliverbodeit   (501) staff       (20)    23227 2023-03-22 13:15:09.000000 rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/data/ribosome.fasta
--rw-r--r--   0 oliverbodeit   (501) staff       (20)     1923 2023-03-22 13:15:10.000000 rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/generate_model.py
--rw-r--r--   0 oliverbodeit   (501) staff       (20)    12083 2023-03-22 13:15:10.000000 rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/reactions.out
--rw-r--r--   0 oliverbodeit   (501) staff       (20)      328 2023-03-22 13:15:09.000000 rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/changeable_parameters.csv
--rw-r--r--   0 oliverbodeit   (501) staff       (20)   308650 2023-03-22 13:15:10.000000 rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/metabolism.xml
--rw-r--r--   0 oliverbodeit   (501) staff       (20)    13340 2023-03-22 13:15:09.000000 rbatools-1.0.2/tutorials/jupyter_notebooks/Model_components_information_access.ipynb
--rw-r--r--   0 oliverbodeit   (501) staff       (20)      328 2022-11-28 10:41:11.000000 rbatools-1.0.2/tutorials/jupyter_notebooks/README.md
--rw-r--r--   0 oliverbodeit   (501) staff       (20)    27543 2022-11-24 13:02:10.000000 rbatools-1.0.2/tutorials/jupyter_notebooks/Example_workflows_rba_tools_Ecoli.ipynb
--rw-r--r--   0 oliverbodeit   (501) staff       (20)   326640 2023-03-22 13:15:09.000000 rbatools-1.0.2/tutorials/jupyter_notebooks/Example_workflows_rba_tools.ipynb
--rw-r--r--   0 oliverbodeit   (501) staff       (20)    14628 2023-03-22 13:15:09.000000 rbatools-1.0.2/tutorials/jupyter_notebooks/Adding_custom_constraint_to_RBA_problem.ipynb
--rw-r--r--   0 oliverbodeit   (501) staff       (20)      600 2023-03-22 13:15:09.000000 rbatools-1.0.2/README.txt
--rw-r--r--   0 oliverbodeit   (501) staff       (20)       67 2023-03-22 13:16:28.000000 rbatools-1.0.2/setup.cfg
--rw-r--r--   0 oliverbodeit   (501) staff       (20)    35149 2022-09-26 12:06:09.000000 rbatools-1.0.2/LICENSE.txt
+drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2023-06-07 11:23:33.000000 rbatools-1.0.3/
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     1554 2023-06-07 11:23:33.000000 rbatools-1.0.3/PKG-INFO
+drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2023-06-07 11:23:32.000000 rbatools-1.0.3/rbatools/
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     4566 2022-10-03 13:32:48.000000 rbatools-1.0.3/rbatools/target_block.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     7594 2022-09-16 15:26:00.000000 rbatools-1.0.3/rbatools/macromolecule_block.py
+-rwxr-xr-x   0 oliverbodeit   (501) staff       (20)    69585 2023-05-15 11:56:35.000000 rbatools-1.0.3/rbatools/rba_model_structure.py
+-rwxr-xr-x   0 oliverbodeit   (501) staff       (20)     6652 2022-09-16 15:26:00.000000 rbatools-1.0.3/rbatools/enzyme_block.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     6925 2023-05-22 11:59:34.000000 rbatools-1.0.3/rbatools/rba_problem_matrix.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)    17550 2022-11-22 21:15:38.000000 rbatools-1.0.3/rbatools/fba_problem.py
+-rwxr-xr-x   0 oliverbodeit   (501) staff       (20)     9719 2023-06-07 11:19:31.000000 rbatools-1.0.3/rbatools/protein_block.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)        8 2023-06-07 11:19:31.000000 rbatools-1.0.3/rbatools/_version.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     7953 2022-09-16 15:26:00.000000 rbatools-1.0.3/rbatools/rba_simulation_parameters.py
+-rwxr-xr-x   0 oliverbodeit   (501) staff       (20)     1292 2022-09-16 15:26:00.000000 rbatools-1.0.3/rbatools/metabolite_constraint_block.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)    27793 2023-05-22 11:59:34.000000 rbatools-1.0.3/rbatools/rba_problem.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)    44603 2023-05-22 11:59:34.000000 rbatools-1.0.3/rbatools/rba_lp.py
+-rwxr-xr-x   0 oliverbodeit   (501) staff       (20)      715 2022-11-24 15:34:09.000000 rbatools-1.0.3/rbatools/__init__.py
+-rwxr-xr-x   0 oliverbodeit   (501) staff       (20)     2450 2022-11-23 10:45:57.000000 rbatools-1.0.3/rbatools/statistics_block.py
+-rwxr-xr-x   0 oliverbodeit   (501) staff       (20)     3744 2022-09-16 15:26:00.000000 rbatools-1.0.3/rbatools/information_block.py
+drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2023-06-07 11:23:32.000000 rbatools-1.0.3/rbatools/cli/
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)        0 2022-10-02 12:32:24.000000 rbatools-1.0.3/rbatools/cli/__init__.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     1227 2022-11-24 15:29:36.000000 rbatools-1.0.3/rbatools/cli/generate_sbtab_of_model_for_html.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     1914 2022-11-24 15:29:57.000000 rbatools-1.0.3/rbatools/cli/run_growth_rate_optimization.py
+-rwxr-xr-x   0 oliverbodeit   (501) staff       (20)     8182 2022-09-26 11:55:01.000000 rbatools-1.0.3/rbatools/metabolite_block.py
+-rwxr-xr-x   0 oliverbodeit   (501) staff       (20)     1729 2022-09-16 15:26:00.000000 rbatools-1.0.3/rbatools/description_block.py
+-rwxr-xr-x   0 oliverbodeit   (501) staff       (20)     5430 2022-09-16 15:26:00.000000 rbatools-1.0.3/rbatools/process_block.py
+-rwxr-xr-x   0 oliverbodeit   (501) staff       (20)     2042 2022-09-16 15:26:00.000000 rbatools-1.0.3/rbatools/compartment_block.py
+-rwxr-xr-x   0 oliverbodeit   (501) staff       (20)     2419 2022-10-03 13:32:48.000000 rbatools-1.0.3/rbatools/density_constraint_block.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)   115613 2023-05-22 11:59:34.000000 rbatools-1.0.3/rbatools/rba_session.py
+-rwxr-xr-x   0 oliverbodeit   (501) staff       (20)     2808 2022-10-03 13:32:48.000000 rbatools-1.0.3/rbatools/enzyme_constraint_block.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)      147 2022-09-16 15:26:00.000000 rbatools-1.0.3/rbatools/_warnings_and_errors.py
+-rwxr-xr-x   0 oliverbodeit   (501) staff       (20)     3123 2022-10-03 13:32:48.000000 rbatools-1.0.3/rbatools/process_constraint_block.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)       54 2022-10-02 12:32:24.000000 rbatools-1.0.3/rbatools/_authors.py
+-rwxr-xr-x   0 oliverbodeit   (501) staff       (20)    14244 2022-09-26 11:55:01.000000 rbatools-1.0.3/rbatools/reaction_block.py
+-rwxr-xr-x   0 oliverbodeit   (501) staff       (20)     6904 2022-09-16 15:26:00.000000 rbatools-1.0.3/rbatools/info_matrix.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)    25488 2023-05-22 11:59:34.000000 rbatools-1.0.3/rbatools/_auxiliary_functions.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     1500 2022-09-16 15:26:00.000000 rbatools-1.0.3/rbatools/parameter_block.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     2096 2022-09-16 15:26:00.000000 rbatools-1.0.3/rbatools/data_block.py
+-rwxr-xr-x   0 oliverbodeit   (501) staff       (20)    49501 2022-11-23 14:00:52.000000 rbatools-1.0.3/rbatools/rba_simulation_data.py
+-rwxr-xr-x   0 oliverbodeit   (501) staff       (20)     1707 2022-09-16 15:26:00.000000 rbatools-1.0.3/rbatools/module_block.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)        3 2022-10-02 12:32:24.000000 rbatools-1.0.3/rbatools/_credits.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)       78 2023-06-07 11:22:09.000000 rbatools-1.0.3/requirements.txt
+drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2023-06-07 11:23:32.000000 rbatools-1.0.3/rbatools.egg-info/
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     1554 2023-06-07 11:23:31.000000 rbatools-1.0.3/rbatools.egg-info/PKG-INFO
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     4370 2023-06-07 11:23:32.000000 rbatools-1.0.3/rbatools.egg-info/SOURCES.txt
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)      183 2023-06-07 11:23:31.000000 rbatools-1.0.3/rbatools.egg-info/entry_points.txt
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)       44 2023-06-07 11:23:31.000000 rbatools-1.0.3/rbatools.egg-info/requires.txt
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)        9 2023-06-07 11:23:31.000000 rbatools-1.0.3/rbatools.egg-info/top_level.txt
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)        1 2023-06-07 11:23:31.000000 rbatools-1.0.3/rbatools.egg-info/dependency_links.txt
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)       98 2022-09-26 12:06:09.000000 rbatools-1.0.3/pyproject.toml
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)       64 2022-09-26 12:06:09.000000 rbatools-1.0.3/MANIFEST.in
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     5960 2023-06-07 10:29:16.000000 rbatools-1.0.3/README.md
+drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2023-06-07 11:23:32.000000 rbatools-1.0.3/figure_for_manuscript/
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)   166885 2023-05-22 11:59:34.000000 rbatools-1.0.3/figure_for_manuscript/LocalSensitivities_all_enzymes_1percent.csv
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)    41736 2023-05-22 11:59:34.000000 rbatools-1.0.3/figure_for_manuscript/RBAtools_FigSamples_stdevlog_0.1.csv
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)    50578 2023-05-22 11:59:34.000000 rbatools-1.0.3/figure_for_manuscript/Figures_reviewed_article.ipynb
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     2996 2023-06-07 11:21:52.000000 rbatools-1.0.3/setup.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     1218 2022-11-24 13:00:21.000000 rbatools-1.0.3/.gitignore
+drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2023-06-07 11:23:32.000000 rbatools-1.0.3/scripts/
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     1227 2022-11-24 15:29:36.000000 rbatools-1.0.3/scripts/generate_sbtab_of_model_for_html.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     1914 2022-11-24 15:29:57.000000 rbatools-1.0.3/scripts/run_growth_rate_optimization.py
+drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2023-06-07 11:23:32.000000 rbatools-1.0.3/tutorials/
+drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2023-06-07 11:23:32.000000 rbatools-1.0.3/tutorials/jupyter_notebooks/
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)    10992 2023-05-22 11:59:34.000000 rbatools-1.0.3/tutorials/jupyter_notebooks/Linear_optimization_with_rbatools.ipynb
+drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2023-06-07 11:23:32.000000 rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)      485 2023-05-22 11:59:35.000000 rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/sample_model_loader.py
+drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2023-06-07 11:23:33.000000 rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     3118 2023-05-22 11:59:35.000000 rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/rnas.xml
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)      802 2023-05-22 11:59:34.000000 rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/dna.xml
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)      136 2023-05-22 11:59:34.000000 rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/ModelInformation.csv
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     5404 2023-05-22 11:59:35.000000 rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/targets.xml
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)    14641 2023-05-22 11:59:34.000000 rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/enzymes.out
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)      240 2023-05-22 11:59:34.000000 rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/density.xml
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)  3368922 2023-05-22 11:59:35.000000 rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/uniprot.csv
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     1418 2023-05-22 11:59:35.000000 rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/params.in
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)      931 2023-05-22 11:59:35.000000 rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/medium.tsv
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)   950277 2023-05-22 11:59:35.000000 rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/proteins.xml
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)   231014 2023-05-22 11:59:34.000000 rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/enzymes.xml
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)      177 2023-05-22 11:59:35.000000 rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/process_machineries.out
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     3949 2023-05-22 11:59:34.000000 rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/README.md
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)       11 2023-05-22 11:59:34.000000 rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/.gitignore
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)  6415232 2023-05-22 11:59:34.000000 rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/ModelStructure.json
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)   465910 2023-05-22 11:59:35.000000 rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/sbml.xml
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)   348791 2023-05-22 11:59:35.000000 rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/parameters.xml
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)   132671 2023-05-22 11:59:35.000000 rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/processes.xml
+drwxr-xr-x   0 oliverbodeit   (501) staff       (20)        0 2023-06-07 11:23:33.000000 rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/data/
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     2108 2023-05-22 11:59:34.000000 rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/data/trnas.fasta
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)  3368922 2023-05-22 11:59:34.000000 rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/data/uniprot.csv
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     2956 2023-05-22 11:59:34.000000 rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/data/chaperones.fasta
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)    20988 2023-05-22 11:59:34.000000 rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/data/catalytic_activity_medium_2.csv
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)   465910 2023-05-22 11:59:34.000000 rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/data/sbml.xml
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)    23227 2023-05-22 11:59:34.000000 rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/data/ribosome.fasta
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)     1923 2023-05-22 11:59:35.000000 rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/generate_model.py
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)    12083 2023-05-22 11:59:35.000000 rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/reactions.out
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)      328 2023-05-22 11:59:34.000000 rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/changeable_parameters.csv
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)   308650 2023-05-22 11:59:35.000000 rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/metabolism.xml
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)    13340 2023-05-22 11:59:34.000000 rbatools-1.0.3/tutorials/jupyter_notebooks/Model_components_information_access.ipynb
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)      328 2022-11-28 10:41:11.000000 rbatools-1.0.3/tutorials/jupyter_notebooks/README.md
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)    27543 2022-11-24 13:02:10.000000 rbatools-1.0.3/tutorials/jupyter_notebooks/Example_workflows_rba_tools_Ecoli.ipynb
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)   326640 2023-05-22 11:59:34.000000 rbatools-1.0.3/tutorials/jupyter_notebooks/Example_workflows_rba_tools.ipynb
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)    14628 2023-05-22 11:59:34.000000 rbatools-1.0.3/tutorials/jupyter_notebooks/Adding_custom_constraint_to_RBA_problem.ipynb
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)      600 2023-05-22 11:59:34.000000 rbatools-1.0.3/README.txt
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)       67 2023-06-07 11:23:33.000000 rbatools-1.0.3/setup.cfg
+-rw-r--r--   0 oliverbodeit   (501) staff       (20)    35149 2022-09-26 12:06:09.000000 rbatools-1.0.3/LICENSE.txt
```

### Comparing `rbatools-1.0.2/PKG-INFO` & `rbatools-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rbatools
-Version: 1.0.2
+Version: 1.0.3
 Summary: Programming interface to resource allocation modelling with the Resource Balance Analysis (RBA) method.
 Home-page: https://rba.inrae.fr
 Author: Oliver Bodeit, Anne Goelzer & Wolfram Liebermeister
 Author-email: anne.goelzer@inrae.fr, wolfram.liebermeister@inrae.fr
 License: GPLv3
 Keywords: metabolism,resource allocation modellingResource Balance Analysis,molecular biology,cell biology,biochemistry,systems biology,computational biology,mathematical modeling,numerical simulation
 Platform: UNKNOWN
```

### Comparing `rbatools-1.0.2/rbatools/target_block.py` & `rbatools-1.0.3/rbatools/target_block.py`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/rbatools/macromolecule_block.py` & `rbatools-1.0.3/rbatools/macromolecule_block.py`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/rbatools/rba_model_structure.py` & `rbatools-1.0.3/rbatools/rba_model_structure.py`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/rbatools/enzyme_block.py` & `rbatools-1.0.3/rbatools/enzyme_block.py`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/rbatools/rba_problem_matrix.py` & `rbatools-1.0.3/rbatools/rba_problem_matrix.py`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/rbatools/fba_problem.py` & `rbatools-1.0.3/rbatools/fba_problem.py`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/rbatools/protein_block.py` & `rbatools-1.0.3/rbatools/protein_block.py`

 * *Files 7% similar despite different names*

```diff
@@ -121,16 +121,18 @@
 
 def _mine_uniprot_file(UniprotData, IDmap, protein):
     differentIDs = {}
     function = ''
     name = ''
     length = numpy.nan
     mass = numpy.nan
-    IDlist = [' ' + m + ' ' + str(n) + ' ' for m,
-              n in zip(list(UniprotData['Entry']), list(UniprotData['Gene names']))]
+    if 'Gene names' in list(UniprotData.columns):
+        IDlist = [' ' + m + ' ' + str(n) + ' ' for m,n in zip(list(UniprotData['Entry']), list(UniprotData['Gene names']))]
+    elif 'Gene Names' in list(UniprotData.columns):
+        IDlist = [' ' + m + ' ' + str(n) + ' ' for m,n in zip(list(UniprotData['Entry']), list(UniprotData['Gene Names']))]
     ProteinRowList = [i for i, s in enumerate(IDlist) if str(' ' + protein + ' ') in s]
     if len(ProteinRowList) > 0:
         ProteinRow = ProteinRowList[0]
         uniprotID = UniprotData['Entry'][ProteinRow]
         differentIDs.update({'UniprotID': uniprotID})
         if UniprotData['Length'][ProteinRow] is not numpy.nan:
             length = UniprotData['Length'][ProteinRow]
@@ -164,19 +166,20 @@
 
 
 def _get_protein_composition(model, protein):
     out = {}
     numberAA = 0
     MacroMolecules = model.proteins.macromolecules._elements
     for a in range(len(MacroMolecules[protein].composition._elements)):
-        out[MacroMolecules[protein].composition._elements[a].component] = int(
-            round(MacroMolecules[protein].composition._elements[a].stoichiometry, 3))  # round(...,3) added#
-        numberAA += MacroMolecules[protein].composition._elements[a].stoichiometry
+        component_id=MacroMolecules[protein].composition._elements[a].component
+        if model.proteins.components._elements_by_id[component_id].type in ['amino_acid']:
+            out[component_id] = MacroMolecules[protein].composition._elements[a].stoichiometry  # round(...,3) added#
+            numberAA += MacroMolecules[protein].composition._elements[a].stoichiometry
     out = {'AAcomp': out,
-           'AAnum': int(numberAA)}
+           'AAnum': numberAA}
     return(out)
 
 
 def _get_process_requirements(model, protein):
     out1 = []
     out2 = []
     Processes = model.processes.processes._elements
```

### Comparing `rbatools-1.0.2/rbatools/rba_simulation_parameters.py` & `rbatools-1.0.3/rbatools/rba_simulation_parameters.py`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/rbatools/metabolite_constraint_block.py` & `rbatools-1.0.3/rbatools/metabolite_constraint_block.py`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/rbatools/rba_problem.py` & `rbatools-1.0.3/rbatools/rba_problem.py`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/rbatools/rba_lp.py` & `rbatools-1.0.3/rbatools/rba_lp.py`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/rbatools/__init__.py` & `rbatools-1.0.3/rbatools/__init__.py`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/rbatools/statistics_block.py` & `rbatools-1.0.3/rbatools/statistics_block.py`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/rbatools/information_block.py` & `rbatools-1.0.3/rbatools/information_block.py`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/rbatools/cli/generate_sbtab_of_model_for_html.py` & `rbatools-1.0.3/rbatools/cli/generate_sbtab_of_model_for_html.py`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/rbatools/cli/run_growth_rate_optimization.py` & `rbatools-1.0.3/rbatools/cli/run_growth_rate_optimization.py`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/rbatools/metabolite_block.py` & `rbatools-1.0.3/rbatools/metabolite_block.py`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/rbatools/description_block.py` & `rbatools-1.0.3/rbatools/description_block.py`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/rbatools/process_block.py` & `rbatools-1.0.3/rbatools/process_block.py`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/rbatools/compartment_block.py` & `rbatools-1.0.3/rbatools/compartment_block.py`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/rbatools/density_constraint_block.py` & `rbatools-1.0.3/rbatools/density_constraint_block.py`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/rbatools/rba_session.py` & `rbatools-1.0.3/rbatools/rba_session.py`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/rbatools/enzyme_constraint_block.py` & `rbatools-1.0.3/rbatools/enzyme_constraint_block.py`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/rbatools/process_constraint_block.py` & `rbatools-1.0.3/rbatools/process_constraint_block.py`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/rbatools/reaction_block.py` & `rbatools-1.0.3/rbatools/reaction_block.py`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/rbatools/info_matrix.py` & `rbatools-1.0.3/rbatools/info_matrix.py`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/rbatools/_auxiliary_functions.py` & `rbatools-1.0.3/rbatools/_auxiliary_functions.py`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/rbatools/parameter_block.py` & `rbatools-1.0.3/rbatools/parameter_block.py`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/rbatools/data_block.py` & `rbatools-1.0.3/rbatools/data_block.py`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/rbatools/rba_simulation_data.py` & `rbatools-1.0.3/rbatools/rba_simulation_data.py`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/rbatools/module_block.py` & `rbatools-1.0.3/rbatools/module_block.py`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/rbatools.egg-info/PKG-INFO` & `rbatools-1.0.3/rbatools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rbatools
-Version: 1.0.2
+Version: 1.0.3
 Summary: Programming interface to resource allocation modelling with the Resource Balance Analysis (RBA) method.
 Home-page: https://rba.inrae.fr
 Author: Oliver Bodeit, Anne Goelzer & Wolfram Liebermeister
 Author-email: anne.goelzer@inrae.fr, wolfram.liebermeister@inrae.fr
 License: GPLv3
 Keywords: metabolism,resource allocation modellingResource Balance Analysis,molecular biology,cell biology,biochemistry,systems biology,computational biology,mathematical modeling,numerical simulation
 Platform: UNKNOWN
```

### Comparing `rbatools-1.0.2/rbatools.egg-info/SOURCES.txt` & `rbatools-1.0.3/rbatools.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 README.md
 README.txt
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 figure_for_manuscript/Figures_reviewed_article.ipynb
-figure_for_manuscript/LocalSensitivitiesEnzymes_001.csv
 figure_for_manuscript/LocalSensitivities_all_enzymes_1percent.csv
+figure_for_manuscript/RBAtools_FigSamples_stdevlog_0.1.csv
 rbatools/__init__.py
 rbatools/_authors.py
 rbatools/_auxiliary_functions.py
 rbatools/_credits.py
 rbatools/_version.py
 rbatools/_warnings_and_errors.py
 rbatools/compartment_block.py
```

### Comparing `rbatools-1.0.2/README.md` & `rbatools-1.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -109,14 +109,19 @@
 
 The Example_workflow_rba_tools notebook requires the previosly mentioned Bacterial-RBA-models repository to be placed in the same location, as this repository.
 
 ## Authors
 
 Bodeit, O., Liebermeister, W. and Goelzer A.
 
+## Citation
+
+If you use RBAtools for scientific publications, please cite our article: Bodeit O., Ben Samir I., Karr J.R., Liebermeister W., Goelzer A. (2023), "RBAtools: a programming interface for Resource Balance Analysis models", Bioinformatics Advances 3 (2023). https://doi.org/10.1093/bioadv/vbad056
+
+
 ## License
 
 Copyright (c) 2022 INRAE - MaIAGE - France.
 
 rbatools is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
```

### Comparing `rbatools-1.0.2/figure_for_manuscript/LocalSensitivities_all_enzymes_1percent.csv` & `rbatools-1.0.3/figure_for_manuscript/LocalSensitivities_all_enzymes_1percent.csv`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/figure_for_manuscript/Figures_reviewed_article.ipynb` & `rbatools-1.0.3/figure_for_manuscript/Figures_reviewed_article.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995748299319728%*

 * *Differences: {"'cells'": "{12: {'source': ['# import from repo:\\n', "*

 * *            '\'#sampling_results=pandas.read_csv("RBAtools_FigSamples_stdevlog_0.1.csv",index_col=0)\']}, '*

 * *            "25: {'source': {insert: [(0, '# import from repo:\\n')], delete: [0]}}}"}*

```diff
@@ -180,16 +180,16 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# import path from local machine:\n",
-                "#sampling_results=pandas.read_csv(\"../../RBAtools_FigSamples_stdevlog_0.1.csv\",index_col=0)"
+                "# import from repo:\n",
+                "#sampling_results=pandas.read_csv(\"RBAtools_FigSamples_stdevlog_0.1.csv\",index_col=0)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Pareto"
@@ -369,15 +369,15 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "# import path from local machine:\n",
+                "# import from repo:\n",
                 "#Local_sensitivities_001=pandas.read_csv(\"LocalSensitivities_all_enzymes_1percent.csv\",index_col=0)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
```

### Comparing `rbatools-1.0.2/setup.py` & `rbatools-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     # You can just specify the packages manually here if your project is
     # simple. Or you can use find_packages().
     packages=find_packages(),
     #packages=find_packages(where="src"),
     install_requires=[
         'rbapy',
         'swiglpk',
-        'sbtab>=1.0.6',
+        'sbtab==1.0.6',
         'jxmlease',
         'urllib3',
     ],
     # List run-time dependencies here.  These will be installed by pip when
     # your project is installed. For an analysis of "install_requires" vs pip's
     # requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
```

### Comparing `rbatools-1.0.2/.gitignore` & `rbatools-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/scripts/generate_sbtab_of_model_for_html.py` & `rbatools-1.0.3/scripts/generate_sbtab_of_model_for_html.py`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/scripts/run_growth_rate_optimization.py` & `rbatools-1.0.3/scripts/run_growth_rate_optimization.py`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/tutorials/jupyter_notebooks/Linear_optimization_with_rbatools.ipynb` & `rbatools-1.0.3/tutorials/jupyter_notebooks/Linear_optimization_with_rbatools.ipynb`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/rnas.xml` & `rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/rnas.xml`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/dna.xml` & `rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/dna.xml`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/targets.xml` & `rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/targets.xml`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/enzymes.out` & `rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/enzymes.out`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/uniprot.csv` & `rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/uniprot.csv`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/params.in` & `rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/params.in`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/medium.tsv` & `rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/medium.tsv`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/proteins.xml` & `rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/proteins.xml`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/enzymes.xml` & `rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/enzymes.xml`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/README.md` & `rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/README.md`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/ModelStructure.json` & `rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/ModelStructure.json`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/sbml.xml` & `rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/sbml.xml`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/parameters.xml` & `rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/parameters.xml`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/processes.xml` & `rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/processes.xml`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/data/trnas.fasta` & `rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/data/trnas.fasta`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/data/uniprot.csv` & `rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/data/uniprot.csv`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/data/chaperones.fasta` & `rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/data/chaperones.fasta`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/data/catalytic_activity_medium_2.csv` & `rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/data/catalytic_activity_medium_2.csv`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/data/sbml.xml` & `rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/data/sbml.xml`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/data/ribosome.fasta` & `rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/data/ribosome.fasta`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/generate_model.py` & `rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/generate_model.py`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/reactions.out` & `rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/reactions.out`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/metabolism.xml` & `rbatools-1.0.3/tutorials/jupyter_notebooks/sample_models/Bacillus-subtilis-168-WT/metabolism.xml`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/tutorials/jupyter_notebooks/Model_components_information_access.ipynb` & `rbatools-1.0.3/tutorials/jupyter_notebooks/Model_components_information_access.ipynb`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/tutorials/jupyter_notebooks/Example_workflows_rba_tools_Ecoli.ipynb` & `rbatools-1.0.3/tutorials/jupyter_notebooks/Example_workflows_rba_tools_Ecoli.ipynb`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/tutorials/jupyter_notebooks/Example_workflows_rba_tools.ipynb` & `rbatools-1.0.3/tutorials/jupyter_notebooks/Example_workflows_rba_tools.ipynb`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/tutorials/jupyter_notebooks/Adding_custom_constraint_to_RBA_problem.ipynb` & `rbatools-1.0.3/tutorials/jupyter_notebooks/Adding_custom_constraint_to_RBA_problem.ipynb`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/README.txt` & `rbatools-1.0.3/README.txt`

 * *Files identical despite different names*

### Comparing `rbatools-1.0.2/LICENSE.txt` & `rbatools-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

