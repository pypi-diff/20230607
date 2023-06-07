# Comparing `tmp/tkwant-1.1.0.tar.gz` & `tmp/tkwant-1.1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tkwant-1.1.0.tar", last modified: Wed Jun  7 11:23:35 2023, max compression
+gzip compressed data, was "dist/tkwant-1.1.0rc2.tar", last modified: Mon May 29 09:53:41 2023, max compression
```

## Comparing `tkwant-1.1.0.tar` & `tkwant-1.1.0rc2.tar`

### file list

```diff
@@ -1,171 +1,171 @@
-drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-06-07 11:23:35.000000 tkwant-1.1.0/
--rw-r--r--   0 cg229074 (65563) big      (30018)     1617 2022-06-04 13:27:44.000000 tkwant-1.1.0/LICENSE.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)     1009 2023-04-15 11:23:22.000000 tkwant-1.1.0/changelog.txt
-drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-06-07 11:23:35.000000 tkwant-1.1.0/tkwant.egg-info/
--rw-r--r--   0 cg229074 (65563) big      (30018)      100 2023-06-07 11:23:28.000000 tkwant-1.1.0/tkwant.egg-info/requires.txt
--rw-r--r--   0 cg229074 (65563) big      (30018)        1 2023-06-07 11:23:28.000000 tkwant-1.1.0/tkwant.egg-info/dependency_links.txt
--rw-r--r--   0 cg229074 (65563) big      (30018)     6506 2023-06-07 11:23:28.000000 tkwant-1.1.0/tkwant.egg-info/PKG-INFO
--rw-r--r--   0 cg229074 (65563) big      (30018)        7 2023-06-07 11:23:28.000000 tkwant-1.1.0/tkwant.egg-info/top_level.txt
--rw-r--r--   0 cg229074 (65563) big      (30018)     4876 2023-06-07 11:23:28.000000 tkwant-1.1.0/tkwant.egg-info/SOURCES.txt
--rw-r--r--   0 cg229074 (65563) big      (30018)      584 2022-06-04 13:27:44.000000 tkwant-1.1.0/conftest.py
--rw-r--r--   0 cg229074 (65563) big      (30018)      252 2022-06-04 13:27:44.000000 tkwant-1.1.0/.coveragerc
--rw-r--r--   0 cg229074 (65563) big      (30018)     5536 2023-05-31 14:50:55.000000 tkwant-1.1.0/INSTALL.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)     5844 2023-06-07 11:23:28.000000 tkwant-1.1.0/MANIFEST.in
-drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-06-07 11:23:35.000000 tkwant-1.1.0/tkwant/
--rw-r--r--   0 cg229074 (65563) big      (30018)     5077 2023-05-02 09:06:37.000000 tkwant-1.1.0/tkwant/integration.py
--rw-r--r--   0 cg229074 (65563) big      (30018)    19503 2023-05-02 09:06:37.000000 tkwant-1.1.0/tkwant/greenfunctions.py
--rw-r--r--   0 cg229074 (65563) big      (30018)   102684 2023-05-02 09:50:34.000000 tkwant-1.1.0/tkwant/manybody.py
--rw-r--r--   0 cg229074 (65563) big      (30018)    24895 2023-04-15 11:20:55.000000 tkwant-1.1.0/tkwant/line_segment.py
--rw-r--r--   0 cg229074 (65563) big      (30018)    11651 2023-05-02 09:50:34.000000 tkwant-1.1.0/tkwant/system.py
--rw-r--r--   0 cg229074 (65563) big      (30018)    11830 2023-05-02 09:50:34.000000 tkwant-1.1.0/tkwant/interaction.py
-drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-06-07 11:23:35.000000 tkwant-1.1.0/tkwant/onebody/
--rw-r--r--   0 cg229074 (65563) big      (30018)    25469 2023-05-02 09:50:34.000000 tkwant-1.1.0/tkwant/onebody/onebody.py
--rw-r--r--   0 cg229074 (65563) big      (30018)      556 2023-05-02 09:06:37.000000 tkwant-1.1.0/tkwant/onebody/kernels.pxd
--rw-r--r--   0 cg229074 (65563) big      (30018)    35369 2023-05-02 15:57:55.000000 tkwant-1.1.0/tkwant/onebody/kernels.pyx
--rw-r--r--   0 cg229074 (65563) big      (30018)     2681 2023-05-02 09:50:34.000000 tkwant-1.1.0/tkwant/onebody/solvers.pyx
--rw-r--r--   0 cg229074 (65563) big      (30018)      914 2023-05-02 09:06:37.000000 tkwant-1.1.0/tkwant/onebody/__init__.py
-drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-06-07 11:23:35.000000 tkwant-1.1.0/tkwant/onebody/tests/
--rw-r--r--   0 cg229074 (65563) big      (30018)    13103 2023-05-02 09:50:34.000000 tkwant-1.1.0/tkwant/onebody/tests/test_kernels.py
--rw-r--r--   0 cg229074 (65563) big      (30018)    41249 2023-05-02 09:06:37.000000 tkwant-1.1.0/tkwant/onebody/tests/test_solvers.py
--rw-r--r--   0 cg229074 (65563) big      (30018)        0 2022-06-04 13:27:44.000000 tkwant-1.1.0/tkwant/onebody/tests/__init__.py
--rw-r--r--   0 cg229074 (65563) big      (30018)   268550 2023-05-02 15:51:48.000000 tkwant-1.1.0/tkwant/onebody/solvers.c
--rw-r--r--   0 cg229074 (65563) big      (30018)  1767336 2023-05-02 15:57:59.000000 tkwant-1.1.0/tkwant/onebody/kernels.c
--rw-r--r--   0 cg229074 (65563) big      (30018)     4738 2023-05-02 09:06:37.000000 tkwant-1.1.0/tkwant/_logging.py
--rw-r--r--   0 cg229074 (65563) big      (30018)     7829 2023-05-02 09:06:37.000000 tkwant-1.1.0/tkwant/mpi.py
--rw-r--r--   0 cg229074 (65563) big      (30018)     1285 2023-05-31 15:55:31.000000 tkwant-1.1.0/tkwant/__init__.py
-drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-06-07 11:23:35.000000 tkwant-1.1.0/tkwant/tests/
--rw-r--r--   0 cg229074 (65563) big      (30018)     1906 2023-05-02 09:06:37.000000 tkwant-1.1.0/tkwant/tests/test_logging.py
--rw-r--r--   0 cg229074 (65563) big      (30018)    11140 2023-05-02 09:50:34.000000 tkwant-1.1.0/tkwant/tests/test_interaction.py
--rw-r--r--   0 cg229074 (65563) big      (30018)     4031 2023-05-02 09:06:37.000000 tkwant-1.1.0/tkwant/tests/common.py
--rw-r--r--   0 cg229074 (65563) big      (30018)     2428 2023-05-02 09:06:37.000000 tkwant-1.1.0/tkwant/tests/test_common.py
--rw-r--r--   0 cg229074 (65563) big      (30018)    30897 2023-05-02 09:50:34.000000 tkwant-1.1.0/tkwant/tests/test_mpi.py
--rw-r--r--   0 cg229074 (65563) big      (30018)       54 2022-06-04 13:27:44.000000 tkwant-1.1.0/tkwant/tests/__init__.py
--rw-r--r--   0 cg229074 (65563) big      (30018)    26381 2023-05-02 09:06:37.000000 tkwant-1.1.0/tkwant/tests/test_leads.py
--rw-r--r--   0 cg229074 (65563) big      (30018)     1497 2023-05-02 09:06:37.000000 tkwant-1.1.0/tkwant/tests/mpi_testdriver.py
--rw-r--r--   0 cg229074 (65563) big      (30018)     2931 2023-05-02 09:06:37.000000 tkwant-1.1.0/tkwant/tests/test_integration.py
--rw-r--r--   0 cg229074 (65563) big      (30018)     6290 2023-05-02 09:06:37.000000 tkwant-1.1.0/tkwant/tests/test_system.py
--rw-r--r--   0 cg229074 (65563) big      (30018)    74588 2023-05-02 09:06:37.000000 tkwant-1.1.0/tkwant/tests/test_manybody.py
--rw-r--r--   0 cg229074 (65563) big      (30018)    10122 2023-05-02 09:06:37.000000 tkwant-1.1.0/tkwant/tests/test_greenfunctions.py
--rw-r--r--   0 cg229074 (65563) big      (30018)     8491 2023-05-02 15:05:07.000000 tkwant-1.1.0/tkwant/special.py
--rw-r--r--   0 cg229074 (65563) big      (30018)    77101 2023-05-02 09:06:37.000000 tkwant-1.1.0/tkwant/leads.py
--rw-r--r--   0 cg229074 (65563) big      (30018)     5073 2023-05-31 14:53:18.000000 tkwant-1.1.0/tkwant/_common.py
--rw-r--r--   0 cg229074 (65563) big      (30018)     6506 2023-06-07 11:23:35.000000 tkwant-1.1.0/PKG-INFO
-drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-06-07 11:23:35.000000 tkwant-1.1.0/docker/
--rw-r--r--   0 cg229074 (65563) big      (30018)     1217 2023-04-15 11:20:55.000000 tkwant-1.1.0/docker/Dockerfile.debian
--rw-r--r--   0 cg229074 (65563) big      (30018)      438 2022-06-04 13:27:44.000000 tkwant-1.1.0/docker/howto_make_and_upload_container.txt
--rw-r--r--   0 cg229074 (65563) big      (30018)       63 2023-06-07 11:23:35.000000 tkwant-1.1.0/setup.cfg
--rw-r--r--   0 cg229074 (65563) big      (30018)      687 2023-04-15 11:20:55.000000 tkwant-1.1.0/AUTHORS.rst
-drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-06-07 11:23:35.000000 tkwant-1.1.0/doc/
-drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-06-07 11:23:35.000000 tkwant-1.1.0/doc/kwantdoctheme/
-drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-06-07 11:23:35.000000 tkwant-1.1.0/doc/kwantdoctheme/static/
--rw-r--r--   0 cg229074 (65563) big      (30018)     3576 2022-06-04 13:27:44.000000 tkwant-1.1.0/doc/kwantdoctheme/static/kwantdoctheme.css
--rw-r--r--   0 cg229074 (65563) big      (30018)      614 2022-06-04 13:27:44.000000 tkwant-1.1.0/doc/kwantdoctheme/theme.conf
-drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-06-07 11:23:35.000000 tkwant-1.1.0/doc/tutorial_source/
--rw-r--r--   0 cg229074 (65563) big      (30018)     7254 2023-04-15 11:23:22.000000 tkwant-1.1.0/doc/tutorial_source/logging.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)     5001 2023-04-15 11:23:22.000000 tkwant-1.1.0/doc/tutorial_source/siam_sudden_switch_plot_results.py
--rw-r--r--   0 cg229074 (65563) big      (30018)     5702 2023-04-15 11:20:55.000000 tkwant-1.1.0/doc/tutorial_source/chem_vs_elec_bias_run_computation.py
--rw-r--r--   0 cg229074 (65563) big      (30018)     3571 2023-05-02 09:50:34.000000 tkwant-1.1.0/doc/tutorial_source/voltage_raise.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)     1764 2023-05-02 09:50:34.000000 tkwant-1.1.0/doc/tutorial_source/plasmon_plot_results.py
--rw-r--r--   0 cg229074 (65563) big      (30018)    12964 2023-04-15 11:20:55.000000 tkwant-1.1.0/doc/tutorial_source/onebody.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)     2481 2023-05-02 09:50:34.000000 tkwant-1.1.0/doc/tutorial_source/open_system.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)     4213 2023-04-15 11:20:55.000000 tkwant-1.1.0/doc/tutorial_source/voltage_raise.py
--rw-r--r--   0 cg229074 (65563) big      (30018)     1949 2023-04-15 11:23:22.000000 tkwant-1.1.0/doc/tutorial_source/chem_vs_elec_bias_plot_results.py
--rw-r--r--   0 cg229074 (65563) big      (30018)    48153 2023-04-15 11:20:55.000000 tkwant-1.1.0/doc/tutorial_source/chem_vs_elec_bias_current.png
--rw-r--r--   0 cg229074 (65563) big      (30018)    81972 2023-04-15 11:23:22.000000 tkwant-1.1.0/doc/tutorial_source/fig_siam_sudden_switch.png
--rw-r--r--   0 cg229074 (65563) big      (30018)    39276 2023-04-15 11:20:55.000000 tkwant-1.1.0/doc/tutorial_source/system_with_lead.png
--rw-r--r--   0 cg229074 (65563) big      (30018)    31413 2023-05-02 09:50:34.000000 tkwant-1.1.0/doc/tutorial_source/adaptive_solver_sketch.png
--rw-r--r--   0 cg229074 (65563) big      (30018)    67397 2023-04-15 11:20:55.000000 tkwant-1.1.0/doc/tutorial_source/fabry_perot_grid.png
--rw-r--r--   0 cg229074 (65563) big      (30018)    53665 2023-05-02 09:50:34.000000 tkwant-1.1.0/doc/tutorial_source/bdg_junction_vj_vs_time.png
--rw-r--r--   0 cg229074 (65563) big      (30018)     6195 2023-05-02 09:50:34.000000 tkwant-1.1.0/doc/tutorial_source/getting_started.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)     2889 2023-04-15 11:20:55.000000 tkwant-1.1.0/doc/tutorial_source/1d_wire_low_level.py
--rw-r--r--   0 cg229074 (65563) big      (30018)    41908 2023-05-02 09:50:34.000000 tkwant-1.1.0/doc/tutorial_source/timescale_decoupling.png
--rw-r--r--   0 cg229074 (65563) big      (30018)    49339 2023-04-15 11:20:55.000000 tkwant-1.1.0/doc/tutorial_source/extended_system.png
--rw-r--r--   0 cg229074 (65563) big      (30018)    30714 2023-04-15 11:20:55.000000 tkwant-1.1.0/doc/tutorial_source/1d_chain_closed.png
--rw-r--r--   0 cg229074 (65563) big      (30018)     2750 2023-04-15 11:20:55.000000 tkwant-1.1.0/doc/tutorial_source/fabry_perot.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)     1025 2023-05-02 09:50:34.000000 tkwant-1.1.0/doc/tutorial_source/bdg_junction_plot_results.py
--rw-r--r--   0 cg229074 (65563) big      (30018)     3004 2023-04-15 11:20:55.000000 tkwant-1.1.0/doc/tutorial_source/faq.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)     7465 2023-04-15 11:23:22.000000 tkwant-1.1.0/doc/tutorial_source/siam_sudden_switch_run_computation.py
--rw-r--r--   0 cg229074 (65563) big      (30018)    12282 2023-05-02 09:06:37.000000 tkwant-1.1.0/doc/tutorial_source/pitfalls.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)    15903 2023-04-15 11:20:55.000000 tkwant-1.1.0/doc/tutorial_source/boundstates.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)    12770 2023-05-02 09:50:34.000000 tkwant-1.1.0/doc/tutorial_source/manybody.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)    11110 2023-05-02 09:50:34.000000 tkwant-1.1.0/doc/tutorial_source/time_dep_system.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)    52097 2023-05-02 17:42:51.000000 tkwant-1.1.0/doc/tutorial_source/green_functions.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)    61574 2023-04-15 11:20:55.000000 tkwant-1.1.0/doc/tutorial_source/scattering_region.png
--rw-r--r--   0 cg229074 (65563) big      (30018)   729086 2023-05-02 09:50:34.000000 tkwant-1.1.0/doc/tutorial_source/junction_lrc_circuit.png
--rw-r--r--   0 cg229074 (65563) big      (30018)    43974 2023-04-15 11:20:55.000000 tkwant-1.1.0/doc/tutorial_source/1d_chain_open.png
--rw-r--r--   0 cg229074 (65563) big      (30018)    14788 2023-05-02 09:50:34.000000 tkwant-1.1.0/doc/tutorial_source/junction_quantum_part.png
--rw-r--r--   0 cg229074 (65563) big      (30018)    81750 2023-05-02 15:05:07.000000 tkwant-1.1.0/doc/tutorial_source/self_consistent.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)     4237 2023-05-02 09:50:34.000000 tkwant-1.1.0/doc/tutorial_source/plasmon_u_0_run_computation.py
--rw-r--r--   0 cg229074 (65563) big      (30018)     2936 2023-04-15 11:20:55.000000 tkwant-1.1.0/doc/tutorial_source/closed_system.py
--rw-r--r--   0 cg229074 (65563) big      (30018)     2187 2023-04-15 11:20:55.000000 tkwant-1.1.0/doc/tutorial_source/1d_wire_onsite.py
--rw-r--r--   0 cg229074 (65563) big      (30018)     1287 2023-05-02 09:50:34.000000 tkwant-1.1.0/doc/tutorial_source/graphene.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)     1856 2023-05-02 09:50:34.000000 tkwant-1.1.0/doc/tutorial_source/closed_system.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)     3651 2023-04-15 11:20:55.000000 tkwant-1.1.0/doc/tutorial_source/introduction.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)    62687 2023-04-15 11:20:55.000000 tkwant-1.1.0/doc/tutorial_source/chem_vs_elec_bias_scheme.png
--rw-r--r--   0 cg229074 (65563) big      (30018)    22142 2023-05-02 09:50:34.000000 tkwant-1.1.0/doc/tutorial_source/chem_vs_elec_bias.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)    68464 2023-05-02 09:50:34.000000 tkwant-1.1.0/doc/tutorial_source/plasmon_propagation.png
--rw-r--r--   0 cg229074 (65563) big      (30018)     4654 2023-05-02 09:50:34.000000 tkwant-1.1.0/doc/tutorial_source/mpi.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)      209 2023-04-15 11:20:55.000000 tkwant-1.1.0/doc/tutorial_source/examples.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)     2773 2023-04-15 11:20:55.000000 tkwant-1.1.0/doc/tutorial_source/open_system.py
--rw-r--r--   0 cg229074 (65563) big      (30018)     4097 2023-05-02 09:50:34.000000 tkwant-1.1.0/doc/tutorial_source/restarting.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)     5340 2023-04-17 20:01:34.000000 tkwant-1.1.0/doc/tutorial_source/onebody_advanced.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)    69615 2023-04-15 11:20:55.000000 tkwant-1.1.0/doc/tutorial_source/toy.png
--rw-r--r--   0 cg229074 (65563) big      (30018)     6670 2023-05-02 09:50:34.000000 tkwant-1.1.0/doc/tutorial_source/bdg_junction_run_computation.py
--rw-r--r--   0 cg229074 (65563) big      (30018)    22533 2023-04-15 11:20:55.000000 tkwant-1.1.0/doc/tutorial_source/manybody_advanced.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)     4641 2023-04-15 11:20:55.000000 tkwant-1.1.0/doc/tutorial_source/alternative_boundary_conditions.py
--rw-r--r--   0 cg229074 (65563) big      (30018)     4677 2023-05-02 09:50:34.000000 tkwant-1.1.0/doc/tutorial_source/plasmon_u_10_run_computation.py
--rw-r--r--   0 cg229074 (65563) big      (30018)     1910 2023-04-15 11:20:55.000000 tkwant-1.1.0/doc/tutorial_source/1d_wire_high_level.py
--rw-r--r--   0 cg229074 (65563) big      (30018)    27261 2023-04-15 11:20:55.000000 tkwant-1.1.0/doc/tutorial_source/boundary_condition.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)      684 2023-05-02 09:50:34.000000 tkwant-1.1.0/doc/tutorial_source/alternative_boundary_conditions.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)     3210 2023-04-15 11:20:55.000000 tkwant-1.1.0/doc/tutorial_source/graphene.py
--rw-r--r--   0 cg229074 (65563) big      (30018)     2718 2023-04-15 11:20:55.000000 tkwant-1.1.0/doc/tutorial_source/fabry_perot.py
-drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-06-07 11:23:35.000000 tkwant-1.1.0/doc/material/
--rw-r--r--   0 cg229074 (65563) big      (30018)     3225 2023-05-02 09:50:34.000000 tkwant-1.1.0/doc/material/make_figure_timescale_decoupling.py
--rw-r--r--   0 cg229074 (65563) big      (30018)   752860 2023-05-02 09:50:34.000000 tkwant-1.1.0/doc/material/adaptive_solver.ai
--rw-r--r--   0 cg229074 (65563) big      (30018)    70147 2023-05-02 09:50:34.000000 tkwant-1.1.0/doc/material/figures_junction_circuit_and_quantum_part.svg
--rw-r--r--   0 cg229074 (65563) big      (30018)     9030 2023-04-15 11:20:55.000000 tkwant-1.1.0/doc/Makefile
-drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-06-07 11:23:35.000000 tkwant-1.1.0/doc/templates/
-drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-06-07 11:23:35.000000 tkwant-1.1.0/doc/templates/autosummary/
--rw-r--r--   0 cg229074 (65563) big      (30018)      550 2022-06-04 13:27:44.000000 tkwant-1.1.0/doc/templates/autosummary/class.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)     1493 2023-04-15 11:20:55.000000 tkwant-1.1.0/doc/templates/layout.html
-drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-06-07 11:23:35.000000 tkwant-1.1.0/doc/sphinxext/
--rw-r--r--   0 cg229074 (65563) big      (30018)     2553 2023-05-02 09:06:37.000000 tkwant-1.1.0/doc/sphinxext/kwantdoc.py
-drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-06-07 11:23:35.000000 tkwant-1.1.0/doc/source/
--rw-r--r--   0 cg229074 (65563) big      (30018)    12046 2023-05-02 09:50:34.000000 tkwant-1.1.0/doc/source/conf.py
-drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-06-07 11:23:35.000000 tkwant-1.1.0/doc/source/extensions/
--rw-r--r--   0 cg229074 (65563) big      (30018)      290 2023-04-15 11:20:55.000000 tkwant-1.1.0/doc/source/extensions/index.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)      235 2023-04-15 11:20:55.000000 tkwant-1.1.0/doc/source/index.rst
-drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-06-07 11:23:35.000000 tkwant-1.1.0/doc/source/tutorial/
--rw-r--r--   0 cg229074 (65563) big      (30018)      307 2023-05-02 15:02:37.000000 tkwant-1.1.0/doc/source/tutorial/index.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)      209 2022-06-04 13:27:44.000000 tkwant-1.1.0/doc/source/tutorial/common.py
-drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-06-07 11:23:35.000000 tkwant-1.1.0/doc/source/pre/
--rw-r--r--   0 cg229074 (65563) big      (30018)      134 2023-04-15 11:23:22.000000 tkwant-1.1.0/doc/source/pre/index.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)       59 2022-06-04 13:27:44.000000 tkwant-1.1.0/doc/source/pre/authors.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)       34 2022-06-04 13:27:44.000000 tkwant-1.1.0/doc/source/pre/installation.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)       95 2023-04-15 11:23:22.000000 tkwant-1.1.0/doc/source/pre/whats_new.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)      477 2023-04-15 11:20:55.000000 tkwant-1.1.0/doc/source/pre/cite.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)       60 2022-06-04 13:27:44.000000 tkwant-1.1.0/doc/source/pre/about.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)       34 2022-06-04 13:27:44.000000 tkwant-1.1.0/doc/source/pre/license.rst
-drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-06-07 11:23:35.000000 tkwant-1.1.0/doc/source/reference/
--rw-r--r--   0 cg229074 (65563) big      (30018)      539 2022-06-04 13:27:44.000000 tkwant-1.1.0/doc/source/reference/index.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)      745 2022-06-04 13:27:44.000000 tkwant-1.1.0/doc/source/reference/tkwant.leads.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)      410 2022-06-04 13:27:44.000000 tkwant-1.1.0/doc/source/reference/tkwant.mpi.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)      387 2022-06-04 13:27:44.000000 tkwant-1.1.0/doc/source/reference/tkwant.onebody.solvers.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)      441 2023-04-15 11:20:55.000000 tkwant-1.1.0/doc/source/reference/tkwant.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)      235 2023-04-15 11:20:55.000000 tkwant-1.1.0/doc/source/reference/tkwant.integrate.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)      717 2022-06-04 13:27:44.000000 tkwant-1.1.0/doc/source/reference/tkwant.manybody.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)      425 2022-06-04 13:27:44.000000 tkwant-1.1.0/doc/source/reference/tkwant.onebody.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)      300 2023-04-15 11:20:55.000000 tkwant-1.1.0/doc/source/reference/tkwant.system.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)      191 2022-06-04 13:27:44.000000 tkwant-1.1.0/doc/source/reference/tkwant.logging.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)      453 2023-04-17 15:38:35.000000 tkwant-1.1.0/doc/source/reference/tkwant.onebody.kernel.rst
-drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-06-07 11:23:35.000000 tkwant-1.1.0/doc/source/_static/
--rw-r--r--   0 cg229074 (65563) big      (30018)      293 2022-06-04 13:27:44.000000 tkwant-1.1.0/doc/source/_static/togglediv.js
--rw-r--r--   0 cg229074 (65563) big      (30018)      294 2022-06-04 13:27:44.000000 tkwant-1.1.0/doc/source/_static/mathconf.js
--rw-r--r--   0 cg229074 (65563) big      (30018)     3017 2022-06-04 13:27:44.000000 tkwant-1.1.0/doc/source/_static/kwant_logo.png
--rw-r--r--   0 cg229074 (65563) big      (30018)     4914 2022-06-04 13:27:44.000000 tkwant-1.1.0/doc/source/_static/sidebar.js
--rw-r--r--   0 cg229074 (65563) big      (30018)     1304 2022-06-04 13:27:44.000000 tkwant-1.1.0/doc/source/_static/kwant.css
--rwxr-xr-x   0 cg229074 (65563) big      (30018)    14343 2023-05-29 08:54:19.000000 tkwant-1.1.0/setup.py
--rw-r--r--   0 cg229074 (65563) big      (30018)      283 2023-04-15 11:20:55.000000 tkwant-1.1.0/environment.yml
--rw-r--r--   0 cg229074 (65563) big      (30018)     4643 2023-05-02 09:06:37.000000 tkwant-1.1.0/README.rst
--rw-r--r--   0 cg229074 (65563) big      (30018)     1959 2023-04-15 11:20:55.000000 tkwant-1.1.0/.gitlab-ci.yml
--rw-r--r--   0 cg229074 (65563) big      (30018)      695 2023-04-15 11:20:55.000000 tkwant-1.1.0/pytest.ini
+drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-05-29 09:53:41.000000 tkwant-1.1.0rc2/
+-rw-r--r--   0 cg229074 (65563) big      (30018)     1617 2022-06-04 13:27:44.000000 tkwant-1.1.0rc2/LICENSE.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)     1009 2023-04-15 11:23:22.000000 tkwant-1.1.0rc2/changelog.txt
+drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-05-29 09:53:41.000000 tkwant-1.1.0rc2/tkwant.egg-info/
+-rw-r--r--   0 cg229074 (65563) big      (30018)      100 2023-05-29 09:53:40.000000 tkwant-1.1.0rc2/tkwant.egg-info/requires.txt
+-rw-r--r--   0 cg229074 (65563) big      (30018)        1 2023-05-29 09:53:40.000000 tkwant-1.1.0rc2/tkwant.egg-info/dependency_links.txt
+-rw-r--r--   0 cg229074 (65563) big      (30018)     6509 2023-05-29 09:53:40.000000 tkwant-1.1.0rc2/tkwant.egg-info/PKG-INFO
+-rw-r--r--   0 cg229074 (65563) big      (30018)        7 2023-05-29 09:53:40.000000 tkwant-1.1.0rc2/tkwant.egg-info/top_level.txt
+-rw-r--r--   0 cg229074 (65563) big      (30018)     4876 2023-05-29 09:53:40.000000 tkwant-1.1.0rc2/tkwant.egg-info/SOURCES.txt
+-rw-r--r--   0 cg229074 (65563) big      (30018)      584 2022-06-04 13:27:44.000000 tkwant-1.1.0rc2/conftest.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)      252 2022-06-04 13:27:44.000000 tkwant-1.1.0rc2/.coveragerc
+-rw-r--r--   0 cg229074 (65563) big      (30018)     7351 2023-04-15 11:20:55.000000 tkwant-1.1.0rc2/INSTALL.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)     5844 2023-05-29 09:53:40.000000 tkwant-1.1.0rc2/MANIFEST.in
+drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-05-29 09:53:41.000000 tkwant-1.1.0rc2/tkwant/
+-rw-r--r--   0 cg229074 (65563) big      (30018)     5077 2023-05-02 09:06:37.000000 tkwant-1.1.0rc2/tkwant/integration.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)    19503 2023-05-02 09:06:37.000000 tkwant-1.1.0rc2/tkwant/greenfunctions.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)   102684 2023-05-02 09:50:34.000000 tkwant-1.1.0rc2/tkwant/manybody.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)    24895 2023-04-15 11:20:55.000000 tkwant-1.1.0rc2/tkwant/line_segment.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)    11651 2023-05-02 09:50:34.000000 tkwant-1.1.0rc2/tkwant/system.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)    11830 2023-05-02 09:50:34.000000 tkwant-1.1.0rc2/tkwant/interaction.py
+drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-05-29 09:53:41.000000 tkwant-1.1.0rc2/tkwant/onebody/
+-rw-r--r--   0 cg229074 (65563) big      (30018)    25469 2023-05-02 09:50:34.000000 tkwant-1.1.0rc2/tkwant/onebody/onebody.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)      556 2023-05-02 09:06:37.000000 tkwant-1.1.0rc2/tkwant/onebody/kernels.pxd
+-rw-r--r--   0 cg229074 (65563) big      (30018)    35369 2023-05-02 15:57:55.000000 tkwant-1.1.0rc2/tkwant/onebody/kernels.pyx
+-rw-r--r--   0 cg229074 (65563) big      (30018)     2681 2023-05-02 09:50:34.000000 tkwant-1.1.0rc2/tkwant/onebody/solvers.pyx
+-rw-r--r--   0 cg229074 (65563) big      (30018)      914 2023-05-02 09:06:37.000000 tkwant-1.1.0rc2/tkwant/onebody/__init__.py
+drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-05-29 09:53:41.000000 tkwant-1.1.0rc2/tkwant/onebody/tests/
+-rw-r--r--   0 cg229074 (65563) big      (30018)    13103 2023-05-02 09:50:34.000000 tkwant-1.1.0rc2/tkwant/onebody/tests/test_kernels.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)    41249 2023-05-02 09:06:37.000000 tkwant-1.1.0rc2/tkwant/onebody/tests/test_solvers.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)        0 2022-06-04 13:27:44.000000 tkwant-1.1.0rc2/tkwant/onebody/tests/__init__.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)   268550 2023-05-02 15:51:48.000000 tkwant-1.1.0rc2/tkwant/onebody/solvers.c
+-rw-r--r--   0 cg229074 (65563) big      (30018)  1767336 2023-05-02 15:57:59.000000 tkwant-1.1.0rc2/tkwant/onebody/kernels.c
+-rw-r--r--   0 cg229074 (65563) big      (30018)     4738 2023-05-02 09:06:37.000000 tkwant-1.1.0rc2/tkwant/_logging.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)     7829 2023-05-02 09:06:37.000000 tkwant-1.1.0rc2/tkwant/mpi.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)     1211 2023-05-05 14:44:14.000000 tkwant-1.1.0rc2/tkwant/__init__.py
+drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-05-29 09:53:41.000000 tkwant-1.1.0rc2/tkwant/tests/
+-rw-r--r--   0 cg229074 (65563) big      (30018)     1906 2023-05-02 09:06:37.000000 tkwant-1.1.0rc2/tkwant/tests/test_logging.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)    11140 2023-05-02 09:50:34.000000 tkwant-1.1.0rc2/tkwant/tests/test_interaction.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)     4031 2023-05-02 09:06:37.000000 tkwant-1.1.0rc2/tkwant/tests/common.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)     2428 2023-05-02 09:06:37.000000 tkwant-1.1.0rc2/tkwant/tests/test_common.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)    30897 2023-05-02 09:50:34.000000 tkwant-1.1.0rc2/tkwant/tests/test_mpi.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)       54 2022-06-04 13:27:44.000000 tkwant-1.1.0rc2/tkwant/tests/__init__.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)    26381 2023-05-02 09:06:37.000000 tkwant-1.1.0rc2/tkwant/tests/test_leads.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)     1497 2023-05-02 09:06:37.000000 tkwant-1.1.0rc2/tkwant/tests/mpi_testdriver.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)     2931 2023-05-02 09:06:37.000000 tkwant-1.1.0rc2/tkwant/tests/test_integration.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)     6290 2023-05-02 09:06:37.000000 tkwant-1.1.0rc2/tkwant/tests/test_system.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)    74588 2023-05-02 09:06:37.000000 tkwant-1.1.0rc2/tkwant/tests/test_manybody.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)    10122 2023-05-02 09:06:37.000000 tkwant-1.1.0rc2/tkwant/tests/test_greenfunctions.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)     8491 2023-05-02 15:05:07.000000 tkwant-1.1.0rc2/tkwant/special.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)    77101 2023-05-02 09:06:37.000000 tkwant-1.1.0rc2/tkwant/leads.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)     5076 2023-05-29 09:03:58.000000 tkwant-1.1.0rc2/tkwant/_common.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)     6509 2023-05-29 09:53:41.000000 tkwant-1.1.0rc2/PKG-INFO
+drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-05-29 09:53:41.000000 tkwant-1.1.0rc2/docker/
+-rw-r--r--   0 cg229074 (65563) big      (30018)     1217 2023-04-15 11:20:55.000000 tkwant-1.1.0rc2/docker/Dockerfile.debian
+-rw-r--r--   0 cg229074 (65563) big      (30018)      438 2022-06-04 13:27:44.000000 tkwant-1.1.0rc2/docker/howto_make_and_upload_container.txt
+-rw-r--r--   0 cg229074 (65563) big      (30018)       63 2023-05-29 09:53:41.000000 tkwant-1.1.0rc2/setup.cfg
+-rw-r--r--   0 cg229074 (65563) big      (30018)      687 2023-04-15 11:20:55.000000 tkwant-1.1.0rc2/AUTHORS.rst
+drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-05-29 09:53:41.000000 tkwant-1.1.0rc2/doc/
+drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-05-29 09:53:41.000000 tkwant-1.1.0rc2/doc/kwantdoctheme/
+drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-05-29 09:53:41.000000 tkwant-1.1.0rc2/doc/kwantdoctheme/static/
+-rw-r--r--   0 cg229074 (65563) big      (30018)     3576 2022-06-04 13:27:44.000000 tkwant-1.1.0rc2/doc/kwantdoctheme/static/kwantdoctheme.css
+-rw-r--r--   0 cg229074 (65563) big      (30018)      614 2022-06-04 13:27:44.000000 tkwant-1.1.0rc2/doc/kwantdoctheme/theme.conf
+drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-05-29 09:53:41.000000 tkwant-1.1.0rc2/doc/tutorial_source/
+-rw-r--r--   0 cg229074 (65563) big      (30018)     7254 2023-04-15 11:23:22.000000 tkwant-1.1.0rc2/doc/tutorial_source/logging.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)     5001 2023-04-15 11:23:22.000000 tkwant-1.1.0rc2/doc/tutorial_source/siam_sudden_switch_plot_results.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)     5702 2023-04-15 11:20:55.000000 tkwant-1.1.0rc2/doc/tutorial_source/chem_vs_elec_bias_run_computation.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)     3571 2023-05-02 09:50:34.000000 tkwant-1.1.0rc2/doc/tutorial_source/voltage_raise.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)     1764 2023-05-02 09:50:34.000000 tkwant-1.1.0rc2/doc/tutorial_source/plasmon_plot_results.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)    12964 2023-04-15 11:20:55.000000 tkwant-1.1.0rc2/doc/tutorial_source/onebody.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)     2481 2023-05-02 09:50:34.000000 tkwant-1.1.0rc2/doc/tutorial_source/open_system.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)     4213 2023-04-15 11:20:55.000000 tkwant-1.1.0rc2/doc/tutorial_source/voltage_raise.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)     1949 2023-04-15 11:23:22.000000 tkwant-1.1.0rc2/doc/tutorial_source/chem_vs_elec_bias_plot_results.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)    48153 2023-04-15 11:20:55.000000 tkwant-1.1.0rc2/doc/tutorial_source/chem_vs_elec_bias_current.png
+-rw-r--r--   0 cg229074 (65563) big      (30018)    81972 2023-04-15 11:23:22.000000 tkwant-1.1.0rc2/doc/tutorial_source/fig_siam_sudden_switch.png
+-rw-r--r--   0 cg229074 (65563) big      (30018)    39276 2023-04-15 11:20:55.000000 tkwant-1.1.0rc2/doc/tutorial_source/system_with_lead.png
+-rw-r--r--   0 cg229074 (65563) big      (30018)    31413 2023-05-02 09:50:34.000000 tkwant-1.1.0rc2/doc/tutorial_source/adaptive_solver_sketch.png
+-rw-r--r--   0 cg229074 (65563) big      (30018)    67397 2023-04-15 11:20:55.000000 tkwant-1.1.0rc2/doc/tutorial_source/fabry_perot_grid.png
+-rw-r--r--   0 cg229074 (65563) big      (30018)    53665 2023-05-02 09:50:34.000000 tkwant-1.1.0rc2/doc/tutorial_source/bdg_junction_vj_vs_time.png
+-rw-r--r--   0 cg229074 (65563) big      (30018)     6195 2023-05-02 09:50:34.000000 tkwant-1.1.0rc2/doc/tutorial_source/getting_started.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)     2889 2023-04-15 11:20:55.000000 tkwant-1.1.0rc2/doc/tutorial_source/1d_wire_low_level.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)    41908 2023-05-02 09:50:34.000000 tkwant-1.1.0rc2/doc/tutorial_source/timescale_decoupling.png
+-rw-r--r--   0 cg229074 (65563) big      (30018)    49339 2023-04-15 11:20:55.000000 tkwant-1.1.0rc2/doc/tutorial_source/extended_system.png
+-rw-r--r--   0 cg229074 (65563) big      (30018)    30714 2023-04-15 11:20:55.000000 tkwant-1.1.0rc2/doc/tutorial_source/1d_chain_closed.png
+-rw-r--r--   0 cg229074 (65563) big      (30018)     2750 2023-04-15 11:20:55.000000 tkwant-1.1.0rc2/doc/tutorial_source/fabry_perot.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)     1025 2023-05-02 09:50:34.000000 tkwant-1.1.0rc2/doc/tutorial_source/bdg_junction_plot_results.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)     3004 2023-04-15 11:20:55.000000 tkwant-1.1.0rc2/doc/tutorial_source/faq.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)     7465 2023-04-15 11:23:22.000000 tkwant-1.1.0rc2/doc/tutorial_source/siam_sudden_switch_run_computation.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)    12282 2023-05-02 09:06:37.000000 tkwant-1.1.0rc2/doc/tutorial_source/pitfalls.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)    15903 2023-04-15 11:20:55.000000 tkwant-1.1.0rc2/doc/tutorial_source/boundstates.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)    12770 2023-05-02 09:50:34.000000 tkwant-1.1.0rc2/doc/tutorial_source/manybody.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)    11110 2023-05-02 09:50:34.000000 tkwant-1.1.0rc2/doc/tutorial_source/time_dep_system.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)    52097 2023-05-02 17:42:51.000000 tkwant-1.1.0rc2/doc/tutorial_source/green_functions.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)    61574 2023-04-15 11:20:55.000000 tkwant-1.1.0rc2/doc/tutorial_source/scattering_region.png
+-rw-r--r--   0 cg229074 (65563) big      (30018)   729086 2023-05-02 09:50:34.000000 tkwant-1.1.0rc2/doc/tutorial_source/junction_lrc_circuit.png
+-rw-r--r--   0 cg229074 (65563) big      (30018)    43974 2023-04-15 11:20:55.000000 tkwant-1.1.0rc2/doc/tutorial_source/1d_chain_open.png
+-rw-r--r--   0 cg229074 (65563) big      (30018)    14788 2023-05-02 09:50:34.000000 tkwant-1.1.0rc2/doc/tutorial_source/junction_quantum_part.png
+-rw-r--r--   0 cg229074 (65563) big      (30018)    81750 2023-05-02 15:05:07.000000 tkwant-1.1.0rc2/doc/tutorial_source/self_consistent.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)     4237 2023-05-02 09:50:34.000000 tkwant-1.1.0rc2/doc/tutorial_source/plasmon_u_0_run_computation.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)     2936 2023-04-15 11:20:55.000000 tkwant-1.1.0rc2/doc/tutorial_source/closed_system.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)     2187 2023-04-15 11:20:55.000000 tkwant-1.1.0rc2/doc/tutorial_source/1d_wire_onsite.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)     1287 2023-05-02 09:50:34.000000 tkwant-1.1.0rc2/doc/tutorial_source/graphene.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)     1856 2023-05-02 09:50:34.000000 tkwant-1.1.0rc2/doc/tutorial_source/closed_system.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)     3651 2023-04-15 11:20:55.000000 tkwant-1.1.0rc2/doc/tutorial_source/introduction.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)    62687 2023-04-15 11:20:55.000000 tkwant-1.1.0rc2/doc/tutorial_source/chem_vs_elec_bias_scheme.png
+-rw-r--r--   0 cg229074 (65563) big      (30018)    22142 2023-05-02 09:50:34.000000 tkwant-1.1.0rc2/doc/tutorial_source/chem_vs_elec_bias.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)    68464 2023-05-02 09:50:34.000000 tkwant-1.1.0rc2/doc/tutorial_source/plasmon_propagation.png
+-rw-r--r--   0 cg229074 (65563) big      (30018)     4654 2023-05-02 09:50:34.000000 tkwant-1.1.0rc2/doc/tutorial_source/mpi.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)      209 2023-04-15 11:20:55.000000 tkwant-1.1.0rc2/doc/tutorial_source/examples.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)     2773 2023-04-15 11:20:55.000000 tkwant-1.1.0rc2/doc/tutorial_source/open_system.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)     4097 2023-05-02 09:50:34.000000 tkwant-1.1.0rc2/doc/tutorial_source/restarting.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)     5340 2023-04-17 20:01:34.000000 tkwant-1.1.0rc2/doc/tutorial_source/onebody_advanced.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)    69615 2023-04-15 11:20:55.000000 tkwant-1.1.0rc2/doc/tutorial_source/toy.png
+-rw-r--r--   0 cg229074 (65563) big      (30018)     6670 2023-05-02 09:50:34.000000 tkwant-1.1.0rc2/doc/tutorial_source/bdg_junction_run_computation.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)    22533 2023-04-15 11:20:55.000000 tkwant-1.1.0rc2/doc/tutorial_source/manybody_advanced.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)     4641 2023-04-15 11:20:55.000000 tkwant-1.1.0rc2/doc/tutorial_source/alternative_boundary_conditions.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)     4677 2023-05-02 09:50:34.000000 tkwant-1.1.0rc2/doc/tutorial_source/plasmon_u_10_run_computation.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)     1910 2023-04-15 11:20:55.000000 tkwant-1.1.0rc2/doc/tutorial_source/1d_wire_high_level.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)    27261 2023-04-15 11:20:55.000000 tkwant-1.1.0rc2/doc/tutorial_source/boundary_condition.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)      684 2023-05-02 09:50:34.000000 tkwant-1.1.0rc2/doc/tutorial_source/alternative_boundary_conditions.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)     3210 2023-04-15 11:20:55.000000 tkwant-1.1.0rc2/doc/tutorial_source/graphene.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)     2718 2023-04-15 11:20:55.000000 tkwant-1.1.0rc2/doc/tutorial_source/fabry_perot.py
+drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-05-29 09:53:41.000000 tkwant-1.1.0rc2/doc/material/
+-rw-r--r--   0 cg229074 (65563) big      (30018)     3225 2023-05-02 09:50:34.000000 tkwant-1.1.0rc2/doc/material/make_figure_timescale_decoupling.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)   752860 2023-05-02 09:50:34.000000 tkwant-1.1.0rc2/doc/material/adaptive_solver.ai
+-rw-r--r--   0 cg229074 (65563) big      (30018)    70147 2023-05-02 09:50:34.000000 tkwant-1.1.0rc2/doc/material/figures_junction_circuit_and_quantum_part.svg
+-rw-r--r--   0 cg229074 (65563) big      (30018)     9030 2023-04-15 11:20:55.000000 tkwant-1.1.0rc2/doc/Makefile
+drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-05-29 09:53:41.000000 tkwant-1.1.0rc2/doc/templates/
+drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-05-29 09:53:41.000000 tkwant-1.1.0rc2/doc/templates/autosummary/
+-rw-r--r--   0 cg229074 (65563) big      (30018)      550 2022-06-04 13:27:44.000000 tkwant-1.1.0rc2/doc/templates/autosummary/class.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)     1493 2023-04-15 11:20:55.000000 tkwant-1.1.0rc2/doc/templates/layout.html
+drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-05-29 09:53:41.000000 tkwant-1.1.0rc2/doc/sphinxext/
+-rw-r--r--   0 cg229074 (65563) big      (30018)     2553 2023-05-02 09:06:37.000000 tkwant-1.1.0rc2/doc/sphinxext/kwantdoc.py
+drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-05-29 09:53:41.000000 tkwant-1.1.0rc2/doc/source/
+-rw-r--r--   0 cg229074 (65563) big      (30018)    12046 2023-05-02 09:50:34.000000 tkwant-1.1.0rc2/doc/source/conf.py
+drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-05-29 09:53:41.000000 tkwant-1.1.0rc2/doc/source/extensions/
+-rw-r--r--   0 cg229074 (65563) big      (30018)      290 2023-04-15 11:20:55.000000 tkwant-1.1.0rc2/doc/source/extensions/index.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)      235 2023-04-15 11:20:55.000000 tkwant-1.1.0rc2/doc/source/index.rst
+drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-05-29 09:53:41.000000 tkwant-1.1.0rc2/doc/source/tutorial/
+-rw-r--r--   0 cg229074 (65563) big      (30018)      307 2023-05-02 15:02:37.000000 tkwant-1.1.0rc2/doc/source/tutorial/index.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)      209 2022-06-04 13:27:44.000000 tkwant-1.1.0rc2/doc/source/tutorial/common.py
+drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-05-29 09:53:41.000000 tkwant-1.1.0rc2/doc/source/pre/
+-rw-r--r--   0 cg229074 (65563) big      (30018)      134 2023-04-15 11:23:22.000000 tkwant-1.1.0rc2/doc/source/pre/index.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)       59 2022-06-04 13:27:44.000000 tkwant-1.1.0rc2/doc/source/pre/authors.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)       34 2022-06-04 13:27:44.000000 tkwant-1.1.0rc2/doc/source/pre/installation.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)       95 2023-04-15 11:23:22.000000 tkwant-1.1.0rc2/doc/source/pre/whats_new.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)      477 2023-04-15 11:20:55.000000 tkwant-1.1.0rc2/doc/source/pre/cite.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)       60 2022-06-04 13:27:44.000000 tkwant-1.1.0rc2/doc/source/pre/about.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)       34 2022-06-04 13:27:44.000000 tkwant-1.1.0rc2/doc/source/pre/license.rst
+drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-05-29 09:53:41.000000 tkwant-1.1.0rc2/doc/source/reference/
+-rw-r--r--   0 cg229074 (65563) big      (30018)      539 2022-06-04 13:27:44.000000 tkwant-1.1.0rc2/doc/source/reference/index.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)      745 2022-06-04 13:27:44.000000 tkwant-1.1.0rc2/doc/source/reference/tkwant.leads.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)      410 2022-06-04 13:27:44.000000 tkwant-1.1.0rc2/doc/source/reference/tkwant.mpi.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)      387 2022-06-04 13:27:44.000000 tkwant-1.1.0rc2/doc/source/reference/tkwant.onebody.solvers.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)      441 2023-04-15 11:20:55.000000 tkwant-1.1.0rc2/doc/source/reference/tkwant.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)      235 2023-04-15 11:20:55.000000 tkwant-1.1.0rc2/doc/source/reference/tkwant.integrate.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)      717 2022-06-04 13:27:44.000000 tkwant-1.1.0rc2/doc/source/reference/tkwant.manybody.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)      425 2022-06-04 13:27:44.000000 tkwant-1.1.0rc2/doc/source/reference/tkwant.onebody.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)      300 2023-04-15 11:20:55.000000 tkwant-1.1.0rc2/doc/source/reference/tkwant.system.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)      191 2022-06-04 13:27:44.000000 tkwant-1.1.0rc2/doc/source/reference/tkwant.logging.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)      453 2023-04-17 15:38:35.000000 tkwant-1.1.0rc2/doc/source/reference/tkwant.onebody.kernel.rst
+drwxr-xr-x   0 cg229074 (65563) big      (30018)        0 2023-05-29 09:53:41.000000 tkwant-1.1.0rc2/doc/source/_static/
+-rw-r--r--   0 cg229074 (65563) big      (30018)      293 2022-06-04 13:27:44.000000 tkwant-1.1.0rc2/doc/source/_static/togglediv.js
+-rw-r--r--   0 cg229074 (65563) big      (30018)      294 2022-06-04 13:27:44.000000 tkwant-1.1.0rc2/doc/source/_static/mathconf.js
+-rw-r--r--   0 cg229074 (65563) big      (30018)     3017 2022-06-04 13:27:44.000000 tkwant-1.1.0rc2/doc/source/_static/kwant_logo.png
+-rw-r--r--   0 cg229074 (65563) big      (30018)     4914 2022-06-04 13:27:44.000000 tkwant-1.1.0rc2/doc/source/_static/sidebar.js
+-rw-r--r--   0 cg229074 (65563) big      (30018)     1304 2022-06-04 13:27:44.000000 tkwant-1.1.0rc2/doc/source/_static/kwant.css
+-rwxr-xr-x   0 cg229074 (65563) big      (30018)    14343 2023-05-29 08:54:19.000000 tkwant-1.1.0rc2/setup.py
+-rw-r--r--   0 cg229074 (65563) big      (30018)      283 2023-04-15 11:20:55.000000 tkwant-1.1.0rc2/environment.yml
+-rw-r--r--   0 cg229074 (65563) big      (30018)     4643 2023-05-02 09:06:37.000000 tkwant-1.1.0rc2/README.rst
+-rw-r--r--   0 cg229074 (65563) big      (30018)     1959 2023-04-15 11:20:55.000000 tkwant-1.1.0rc2/.gitlab-ci.yml
+-rw-r--r--   0 cg229074 (65563) big      (30018)      695 2023-04-15 11:20:55.000000 tkwant-1.1.0rc2/pytest.ini
```

### Comparing `tkwant-1.1.0/LICENSE.rst` & `tkwant-1.1.0rc2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/changelog.txt` & `tkwant-1.1.0rc2/changelog.txt`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/tkwant.egg-info/PKG-INFO` & `tkwant-1.1.0rc2/tkwant.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tkwant
-Version: 1.1.0
+Version: 1.1.0rc2
 Summary: Package for time-dependent quantum transport simulations
 Home-page: https://tkwant.kwant-project.org/
 Author: tkwant authors
 Author-email: tkwant-authors@kwant-project.org
 License: BSD
 Description: Tkwant is a python package to simulate time-dependent quantum dynamics of
         mesoscopic systems. It is the time-dependent generalization of the
```

### Comparing `tkwant-1.1.0/tkwant.egg-info/SOURCES.txt` & `tkwant-1.1.0rc2/tkwant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/conftest.py` & `tkwant-1.1.0rc2/conftest.py`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/MANIFEST.in` & `tkwant-1.1.0rc2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/tkwant/integration.py` & `tkwant-1.1.0rc2/tkwant/integration.py`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/tkwant/greenfunctions.py` & `tkwant-1.1.0rc2/tkwant/greenfunctions.py`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/tkwant/manybody.py` & `tkwant-1.1.0rc2/tkwant/manybody.py`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/tkwant/line_segment.py` & `tkwant-1.1.0rc2/tkwant/line_segment.py`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/tkwant/system.py` & `tkwant-1.1.0rc2/tkwant/system.py`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/tkwant/interaction.py` & `tkwant-1.1.0rc2/tkwant/interaction.py`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/tkwant/onebody/onebody.py` & `tkwant-1.1.0rc2/tkwant/onebody/onebody.py`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/tkwant/onebody/kernels.pxd` & `tkwant-1.1.0rc2/tkwant/onebody/kernels.pxd`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/tkwant/onebody/kernels.pyx` & `tkwant-1.1.0rc2/tkwant/onebody/kernels.pyx`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/tkwant/onebody/solvers.pyx` & `tkwant-1.1.0rc2/tkwant/onebody/solvers.pyx`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/tkwant/onebody/__init__.py` & `tkwant-1.1.0rc2/tkwant/onebody/__init__.py`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/tkwant/onebody/tests/test_kernels.py` & `tkwant-1.1.0rc2/tkwant/onebody/tests/test_kernels.py`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/tkwant/onebody/tests/test_solvers.py` & `tkwant-1.1.0rc2/tkwant/onebody/tests/test_solvers.py`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/tkwant/onebody/solvers.c` & `tkwant-1.1.0rc2/tkwant/onebody/solvers.c`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/tkwant/onebody/kernels.c` & `tkwant-1.1.0rc2/tkwant/onebody/kernels.c`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/tkwant/_logging.py` & `tkwant-1.1.0rc2/tkwant/_logging.py`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/tkwant/mpi.py` & `tkwant-1.1.0rc2/tkwant/mpi.py`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/tkwant/__init__.py` & `tkwant-1.1.0rc2/tkwant/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 tkwant authors.
+# Copyright 2016 tkwant authors.
 #
 # This file is part of tkwant.  It is subject to the license terms in the file
 # LICENSE.rst found in the top-level directory of this distribution and at
 # https://tkwant.kwant-project.org/doc/stable/pre/license.html.
 # A list of tkwant authors can be found in
 # the file AUTHORS.rst at the top-level directory of this distribution and at
 # https://tkwant.kwant-project.org/doc/stable/pre/authors.html.
@@ -25,15 +25,12 @@
 
 del module  # remove cruft from namespace
 
 # set version attribute
 __version__ = TKWANT_VERSION
 
 
-def test(args=None):
-    """Run tkwant's unit tests.
-       Optional command line **args** can be provided as a list of strings."""
+def test(verbose=True):
+    """Run tkwant's unit tests."""
     import pytest
-    command = [os.path.dirname(os.path.realpath(__file__))]
-    if args:
-        command += args
-    return pytest.main(command)
+    return pytest.main([os.path.dirname(os.path.abspath(__file__)), '-s']
+                       + (['-v'] if verbose else []))
```

### Comparing `tkwant-1.1.0/tkwant/tests/test_logging.py` & `tkwant-1.1.0rc2/tkwant/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/tkwant/tests/test_interaction.py` & `tkwant-1.1.0rc2/tkwant/tests/test_interaction.py`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/tkwant/tests/common.py` & `tkwant-1.1.0rc2/tkwant/tests/common.py`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/tkwant/tests/test_common.py` & `tkwant-1.1.0rc2/tkwant/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/tkwant/tests/test_mpi.py` & `tkwant-1.1.0rc2/tkwant/tests/test_mpi.py`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/tkwant/tests/test_leads.py` & `tkwant-1.1.0rc2/tkwant/tests/test_leads.py`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/tkwant/tests/mpi_testdriver.py` & `tkwant-1.1.0rc2/tkwant/tests/mpi_testdriver.py`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/tkwant/tests/test_integration.py` & `tkwant-1.1.0rc2/tkwant/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/tkwant/tests/test_system.py` & `tkwant-1.1.0rc2/tkwant/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/tkwant/tests/test_manybody.py` & `tkwant-1.1.0rc2/tkwant/tests/test_manybody.py`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/tkwant/tests/test_greenfunctions.py` & `tkwant-1.1.0rc2/tkwant/tests/test_greenfunctions.py`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/tkwant/special.py` & `tkwant-1.1.0rc2/tkwant/special.py`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/tkwant/leads.py` & `tkwant-1.1.0rc2/tkwant/leads.py`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/tkwant/_common.py` & `tkwant-1.1.0rc2/tkwant/_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 __all__ = ['version', 'TkwantDeprecationWarning', 'is_type', 'is_type_array',
            'is_not_empty', 'is_zero', 'time_start', 'time_name', 'memoize']
 
 # tkwant's default initial time and time argument name
 time_start = 0
 time_name = 'time'
 
-TKWANT_VERSION = "1.1.0"
+TKWANT_VERSION = "1.1.0rc2"
 
 package_root = os.path.dirname(os.path.realpath(__file__))
 distr_root = os.path.dirname(package_root)
 
 
 class TkwantDeprecationWarning(Warning):
     """Class of warnings about a deprecated feature of tkwant.
```

### Comparing `tkwant-1.1.0/PKG-INFO` & `tkwant-1.1.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tkwant
-Version: 1.1.0
+Version: 1.1.0rc2
 Summary: Package for time-dependent quantum transport simulations
 Home-page: https://tkwant.kwant-project.org/
 Author: tkwant authors
 Author-email: tkwant-authors@kwant-project.org
 License: BSD
 Description: Tkwant is a python package to simulate time-dependent quantum dynamics of
         mesoscopic systems. It is the time-dependent generalization of the
```

### Comparing `tkwant-1.1.0/docker/Dockerfile.debian` & `tkwant-1.1.0rc2/docker/Dockerfile.debian`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/AUTHORS.rst` & `tkwant-1.1.0rc2/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/kwantdoctheme/static/kwantdoctheme.css` & `tkwant-1.1.0rc2/doc/kwantdoctheme/static/kwantdoctheme.css`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/kwantdoctheme/theme.conf` & `tkwant-1.1.0rc2/doc/kwantdoctheme/theme.conf`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/logging.rst` & `tkwant-1.1.0rc2/doc/tutorial_source/logging.rst`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/siam_sudden_switch_plot_results.py` & `tkwant-1.1.0rc2/doc/tutorial_source/siam_sudden_switch_plot_results.py`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/chem_vs_elec_bias_run_computation.py` & `tkwant-1.1.0rc2/doc/tutorial_source/chem_vs_elec_bias_run_computation.py`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/voltage_raise.rst` & `tkwant-1.1.0rc2/doc/tutorial_source/voltage_raise.rst`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/plasmon_plot_results.py` & `tkwant-1.1.0rc2/doc/tutorial_source/plasmon_plot_results.py`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/onebody.rst` & `tkwant-1.1.0rc2/doc/tutorial_source/onebody.rst`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/open_system.rst` & `tkwant-1.1.0rc2/doc/tutorial_source/open_system.rst`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/voltage_raise.py` & `tkwant-1.1.0rc2/doc/tutorial_source/voltage_raise.py`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/chem_vs_elec_bias_plot_results.py` & `tkwant-1.1.0rc2/doc/tutorial_source/chem_vs_elec_bias_plot_results.py`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/chem_vs_elec_bias_current.png` & `tkwant-1.1.0rc2/doc/tutorial_source/chem_vs_elec_bias_current.png`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/fig_siam_sudden_switch.png` & `tkwant-1.1.0rc2/doc/tutorial_source/fig_siam_sudden_switch.png`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/system_with_lead.png` & `tkwant-1.1.0rc2/doc/tutorial_source/system_with_lead.png`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/adaptive_solver_sketch.png` & `tkwant-1.1.0rc2/doc/tutorial_source/adaptive_solver_sketch.png`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/fabry_perot_grid.png` & `tkwant-1.1.0rc2/doc/tutorial_source/fabry_perot_grid.png`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/bdg_junction_vj_vs_time.png` & `tkwant-1.1.0rc2/doc/tutorial_source/bdg_junction_vj_vs_time.png`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/getting_started.rst` & `tkwant-1.1.0rc2/doc/tutorial_source/getting_started.rst`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/1d_wire_low_level.py` & `tkwant-1.1.0rc2/doc/tutorial_source/1d_wire_low_level.py`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/timescale_decoupling.png` & `tkwant-1.1.0rc2/doc/tutorial_source/timescale_decoupling.png`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/extended_system.png` & `tkwant-1.1.0rc2/doc/tutorial_source/extended_system.png`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/1d_chain_closed.png` & `tkwant-1.1.0rc2/doc/tutorial_source/1d_chain_closed.png`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/fabry_perot.rst` & `tkwant-1.1.0rc2/doc/tutorial_source/fabry_perot.rst`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/bdg_junction_plot_results.py` & `tkwant-1.1.0rc2/doc/tutorial_source/bdg_junction_plot_results.py`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/faq.rst` & `tkwant-1.1.0rc2/doc/tutorial_source/faq.rst`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/siam_sudden_switch_run_computation.py` & `tkwant-1.1.0rc2/doc/tutorial_source/siam_sudden_switch_run_computation.py`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/pitfalls.rst` & `tkwant-1.1.0rc2/doc/tutorial_source/pitfalls.rst`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/boundstates.rst` & `tkwant-1.1.0rc2/doc/tutorial_source/boundstates.rst`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/manybody.rst` & `tkwant-1.1.0rc2/doc/tutorial_source/manybody.rst`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/time_dep_system.rst` & `tkwant-1.1.0rc2/doc/tutorial_source/time_dep_system.rst`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/green_functions.rst` & `tkwant-1.1.0rc2/doc/tutorial_source/green_functions.rst`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/scattering_region.png` & `tkwant-1.1.0rc2/doc/tutorial_source/scattering_region.png`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/junction_lrc_circuit.png` & `tkwant-1.1.0rc2/doc/tutorial_source/junction_lrc_circuit.png`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/1d_chain_open.png` & `tkwant-1.1.0rc2/doc/tutorial_source/1d_chain_open.png`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/junction_quantum_part.png` & `tkwant-1.1.0rc2/doc/tutorial_source/junction_quantum_part.png`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/self_consistent.rst` & `tkwant-1.1.0rc2/doc/tutorial_source/self_consistent.rst`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/plasmon_u_0_run_computation.py` & `tkwant-1.1.0rc2/doc/tutorial_source/plasmon_u_0_run_computation.py`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/closed_system.py` & `tkwant-1.1.0rc2/doc/tutorial_source/closed_system.py`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/1d_wire_onsite.py` & `tkwant-1.1.0rc2/doc/tutorial_source/1d_wire_onsite.py`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/graphene.rst` & `tkwant-1.1.0rc2/doc/tutorial_source/graphene.rst`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/closed_system.rst` & `tkwant-1.1.0rc2/doc/tutorial_source/closed_system.rst`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/introduction.rst` & `tkwant-1.1.0rc2/doc/tutorial_source/introduction.rst`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/chem_vs_elec_bias_scheme.png` & `tkwant-1.1.0rc2/doc/tutorial_source/chem_vs_elec_bias_scheme.png`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/chem_vs_elec_bias.rst` & `tkwant-1.1.0rc2/doc/tutorial_source/chem_vs_elec_bias.rst`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/plasmon_propagation.png` & `tkwant-1.1.0rc2/doc/tutorial_source/plasmon_propagation.png`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/mpi.rst` & `tkwant-1.1.0rc2/doc/tutorial_source/mpi.rst`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/open_system.py` & `tkwant-1.1.0rc2/doc/tutorial_source/open_system.py`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/restarting.rst` & `tkwant-1.1.0rc2/doc/tutorial_source/restarting.rst`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/onebody_advanced.rst` & `tkwant-1.1.0rc2/doc/tutorial_source/onebody_advanced.rst`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/toy.png` & `tkwant-1.1.0rc2/doc/tutorial_source/toy.png`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/bdg_junction_run_computation.py` & `tkwant-1.1.0rc2/doc/tutorial_source/bdg_junction_run_computation.py`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/manybody_advanced.rst` & `tkwant-1.1.0rc2/doc/tutorial_source/manybody_advanced.rst`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/alternative_boundary_conditions.py` & `tkwant-1.1.0rc2/doc/tutorial_source/alternative_boundary_conditions.py`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/plasmon_u_10_run_computation.py` & `tkwant-1.1.0rc2/doc/tutorial_source/plasmon_u_10_run_computation.py`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/1d_wire_high_level.py` & `tkwant-1.1.0rc2/doc/tutorial_source/1d_wire_high_level.py`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/boundary_condition.rst` & `tkwant-1.1.0rc2/doc/tutorial_source/boundary_condition.rst`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/alternative_boundary_conditions.rst` & `tkwant-1.1.0rc2/doc/tutorial_source/alternative_boundary_conditions.rst`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/graphene.py` & `tkwant-1.1.0rc2/doc/tutorial_source/graphene.py`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/tutorial_source/fabry_perot.py` & `tkwant-1.1.0rc2/doc/tutorial_source/fabry_perot.py`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/material/make_figure_timescale_decoupling.py` & `tkwant-1.1.0rc2/doc/material/make_figure_timescale_decoupling.py`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/material/adaptive_solver.ai` & `tkwant-1.1.0rc2/doc/material/adaptive_solver.ai`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/material/figures_junction_circuit_and_quantum_part.svg` & `tkwant-1.1.0rc2/doc/material/figures_junction_circuit_and_quantum_part.svg`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/Makefile` & `tkwant-1.1.0rc2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/templates/autosummary/class.rst` & `tkwant-1.1.0rc2/doc/templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/templates/layout.html` & `tkwant-1.1.0rc2/doc/templates/layout.html`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/sphinxext/kwantdoc.py` & `tkwant-1.1.0rc2/doc/sphinxext/kwantdoc.py`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/source/conf.py` & `tkwant-1.1.0rc2/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/source/reference/index.rst` & `tkwant-1.1.0rc2/doc/source/reference/index.rst`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/source/reference/tkwant.leads.rst` & `tkwant-1.1.0rc2/doc/source/reference/tkwant.leads.rst`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/source/reference/tkwant.manybody.rst` & `tkwant-1.1.0rc2/doc/source/reference/tkwant.manybody.rst`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/source/_static/kwant_logo.png` & `tkwant-1.1.0rc2/doc/source/_static/kwant_logo.png`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/source/_static/sidebar.js` & `tkwant-1.1.0rc2/doc/source/_static/sidebar.js`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/doc/source/_static/kwant.css` & `tkwant-1.1.0rc2/doc/source/_static/kwant.css`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/setup.py` & `tkwant-1.1.0rc2/setup.py`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/README.rst` & `tkwant-1.1.0rc2/README.rst`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/.gitlab-ci.yml` & `tkwant-1.1.0rc2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `tkwant-1.1.0/pytest.ini` & `tkwant-1.1.0rc2/pytest.ini`

 * *Files identical despite different names*

